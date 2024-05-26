# Comparing `tmp/txl_jpterm-0.2.8.tar.gz` & `tmp/txl_jpterm-0.2.9.tar.gz`

## Comparing `txl_jpterm-0.2.8.tar` & `txl_jpterm-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 txl_jpterm-0.2.8/txl_jpterm/__init__.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 txl_jpterm-0.2.8/txl_jpterm/components.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 txl_jpterm-0.2.8/txl_jpterm/footer.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 txl_jpterm-0.2.8/txl_jpterm/header.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 txl_jpterm-0.2.8/txl_jpterm/jpterm.css
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 txl_jpterm-0.2.8/txl_jpterm/main_area.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 txl_jpterm-0.2.8/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 txl_jpterm-0.2.8/LICENSE.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 txl_jpterm-0.2.8/README.md
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 txl_jpterm-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 txl_jpterm-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 txl_jpterm-0.2.9/txl_jpterm/__init__.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 txl_jpterm-0.2.9/txl_jpterm/components.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 txl_jpterm-0.2.9/txl_jpterm/footer.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 txl_jpterm-0.2.9/txl_jpterm/header.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 txl_jpterm-0.2.9/txl_jpterm/jpterm.css
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 txl_jpterm-0.2.9/txl_jpterm/main_area.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 txl_jpterm-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 txl_jpterm-0.2.9/LICENSE.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 txl_jpterm-0.2.9/README.md
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 txl_jpterm-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 txl_jpterm-0.2.9/PKG-INFO
```

### Comparing `txl_jpterm-0.2.8/txl_jpterm/components.py` & `txl_jpterm-0.2.9/txl_jpterm/components.py`

 * *Files identical despite different names*

### Comparing `txl_jpterm-0.2.8/txl_jpterm/footer.py` & `txl_jpterm-0.2.9/txl_jpterm/footer.py`

 * *Files identical despite different names*

### Comparing `txl_jpterm-0.2.8/txl_jpterm/main_area.py` & `txl_jpterm-0.2.9/txl_jpterm/main_area.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,60 +12,64 @@
 
 class MainArea(Widget, AbstractMainArea, metaclass=MainAreaMeta):
     def __init__(self):
         super().__init__(id="main-view")
         self.mounted = []
         self.shown = None
         self.tabs = None
-        self.widgets = {}
+        self.widget_to_tab = {}
         self.title = 0
 
     def show(self, widget: Widget, title: Optional[str] = None):
         if widget not in self.mounted:
             if title is None:
                 title = self.title
                 self.title += 1
             tab = Tab(str(title))
             if self.tabs is None:
                 self.tabs = Tabs(tab)
                 self.mount(self.tabs)
             else:
                 self.tabs.add_tab(tab)
                 self.tabs.active = tab.id
-            self.widgets[tab] = widget
+            self.widget_to_tab[widget] = (tab, False)
             self.mounted.append(widget)
             self.mount(widget)
         else:
-            tab = list(self.widgets.keys())[list(self.widgets.values()).index(widget)]
+            tab, dirty = self.widget_to_tab[widget]
             self.tabs.active = tab.id
 
     def get_label(self) -> str:
         tab = self.tabs.active_tab
         return tab.label_text
 
     def set_label(self, title: str) -> None:
         tab = self.tabs.active_tab
         tab.label = title
 
     def set_dirty(self, widget: Widget) -> None:
         if widget not in self.mounted:
             return
 
-        tab = list(self.widgets.keys())[list(self.widgets.values()).index(widget)]
-        if not tab.label_text.startswith("+ "):
+        tab, dirty = self.widget_to_tab[widget]
+        if not dirty:
+            self.widget_to_tab[widget] = (tab, True)
             tab.label = "+ " + tab.label_text
 
     def clear_dirty(self, widget: Widget) -> None:
         if widget not in self.mounted:
             return
 
-        tab = list(self.widgets.keys())[list(self.widgets.values()).index(widget)]
-        if tab.label_text.startswith("+ "):
+        tab, dirty = self.widget_to_tab[widget]
+        if dirty:
+            self.widget_to_tab[widget] = (tab, False)
             tab.label = tab.label_text[2:]
 
     def on_tabs_tab_activated(self, event: Tabs.TabActivated) -> None:
-        widget = self.widgets[event.tab]
+        widgets = list(self.widget_to_tab.keys())
+        tabs = [tab for tab, dirty in self.widget_to_tab.values()]
+        widget = widgets[tabs.index(event.tab)]
         if self.shown is not None:
             self.shown.display = False
         self.shown = widget
         widget.display = True
         widget.focus()
```

### Comparing `txl_jpterm-0.2.8/LICENSE.txt` & `txl_jpterm-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `txl_jpterm-0.2.8/pyproject.toml` & `txl_jpterm-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `txl_jpterm-0.2.8/PKG-INFO` & `txl_jpterm-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txl_jpterm
-Version: 0.2.8
+Version: 0.2.9
 Summary: TXL plugin for the jpterm app
 Project-URL: Source, https://github.com/davidbrochart/jpterm/plugins/jpterm
 Author-email: David Brochart <david.brochart@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

