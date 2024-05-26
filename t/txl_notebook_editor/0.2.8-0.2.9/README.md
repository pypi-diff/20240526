# Comparing `tmp/txl_notebook_editor-0.2.8.tar.gz` & `tmp/txl_notebook_editor-0.2.9.tar.gz`

## Comparing `txl_notebook_editor-0.2.8.tar` & `txl_notebook_editor-0.2.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.8/txl_notebook_editor/__init__.py
--rw-r--r--   0        0        0    15206 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.8/txl_notebook_editor/components.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.8/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.8/LICENSE.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.8/README.md
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.9/txl_notebook_editor/__init__.py
+-rw-r--r--   0        0        0    16153 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.9/txl_notebook_editor/components.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.9/LICENSE.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.9/README.md
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 txl_notebook_editor-0.2.9/PKG-INFO
```

### Comparing `txl_notebook_editor-0.2.8/txl_notebook_editor/components.py` & `txl_notebook_editor-0.2.9/txl_notebook_editor/components.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 from functools import partial
 from importlib.metadata import entry_points
 from typing import Any
 
 import anyio
 from asphalt.core import Component, Context
 from httpx import AsyncClient
+from textual.app import RenderResult
 from textual.containers import VerticalScroll
 from textual.events import Event
 from textual.keys import Keys
+from textual.reactive import Reactive
+from textual.widget import Widget
 from textual.widgets import Select
 
 from txl.base import (
     CellFactory,
     Contents,
     Editor,
     Editors,
@@ -23,14 +26,41 @@
     Launcher,
     MainArea,
 )
 
 ydocs = {ep.name: ep.load() for ep in entry_points(group="jupyter_ydoc")}
 
 
+class TopBar(Widget):
+    DEFAULT_CSS = """
+    TopBar {
+        dock: top;
+        width: 100%;
+        background: $foreground 5%;
+        text-align: right;
+        color: $text;
+        height: 1;
+    }
+    """
+    _busy_indicator = Reactive("○")
+    _busy = False
+
+    @property
+    def busy(self) -> bool:
+        return self._busy
+
+    @busy.setter
+    def busy(self, value: bool):
+        self._busy = value
+        self._busy_indicator = "◉" if value else "○"
+
+    def render(self) -> RenderResult:
+        return self._busy_indicator
+
+
 class NotebookEditorMeta(type(Editor), type(VerticalScroll)):
     pass
 
 
 class NotebookEditor(Editor, VerticalScroll, metaclass=NotebookEditorMeta):
     def __init__(
         self,
@@ -51,14 +81,19 @@
         self.kernel = None
         self.cells = []
         self.cell_i = 0
         self.cell_copy = None
         self.edit_mode = False
         self.nb_change_target = asyncio.Queue()
         self.nb_change_events = asyncio.Queue()
+        self.top_bar = TopBar()
+        self.mount(self.top_bar)
+
+    async def watch_busy(self, event):
+        self.top_bar.busy = event.busy
 
     async def on_open(self, event: FileOpenEvent) -> None:
         await self.open(event.path)
 
     async def select_kernel(self) -> str:
         select = Select((name, name) for name in self.kernelspecs["kernelspecs"])
 
@@ -119,14 +154,15 @@
     def update(self):
         ipynb = self.ynb.source
         self.language = ipynb.get("metadata", {}).get("kernelspec", {}).get("language", None)
         if self.kernel is None:
             kernel_name = ipynb.get("metadata", {}).get("kernelspec", {}).get("name")
             if kernel_name:
                 self.kernel = self.kernels(kernel_name)
+                self.kernel.kernel.busy.connect(self.watch_busy)
         for i_cell in range(self.ynb.cell_number):
             cell = self.cell_factory(
                 self.ynb.ycells[i_cell], self.language, self.kernel
             )
             self.mount(cell)
             self.cells.append(cell)
         if self.cells:
@@ -148,14 +184,15 @@
                     for cell in self.cells:
                         if cell.ycell["cell_type"] == "code":
                             cell.language = self.language
                     if self.kernel is None:
                         kernel_name = kernelspec.get("name")
                         if kernel_name:
                             self.kernel = self.kernels(kernel_name)
+                            self.kernel.kernel.busy.connect(self.watch_busy)
             elif target == "state":
                 if "dirty" in events.keys:
                     dirty = events.keys["dirty"]["newValue"]
                     if dirty:
                         self.main_area.set_dirty(self)
                     else:
                         self.main_area.clear_dirty(self)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `txl_notebook_editor-0.2.8/LICENSE.txt` & `txl_notebook_editor-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `txl_notebook_editor-0.2.8/pyproject.toml` & `txl_notebook_editor-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `txl_notebook_editor-0.2.8/PKG-INFO` & `txl_notebook_editor-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txl_notebook_editor
-Version: 0.2.8
+Version: 0.2.9
 Summary: TXL plugin for a notebook editor
 Project-URL: Source, https://github.com/davidbrochart/jpterm/plugins/notebook_editor
 Author-email: David Brochart <david.brochart@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

