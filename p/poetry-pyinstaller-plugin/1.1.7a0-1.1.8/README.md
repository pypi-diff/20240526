# Comparing `tmp/poetry_pyinstaller_plugin-1.1.7a0.tar.gz` & `tmp/poetry_pyinstaller_plugin-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_pyinstaller_plugin-1.1.7a0.tar", max compression
+gzip compressed data, was "poetry_pyinstaller_plugin-1.1.8.tar", max compression
```

## Comparing `poetry_pyinstaller_plugin-1.1.7a0.tar` & `poetry_pyinstaller_plugin-1.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-02-23 22:51:16.999128 poetry_pyinstaller_plugin-1.1.7a0/LICENSE
--rw-r--r--   0        0        0     5302 2024-03-15 08:21:38.610088 poetry_pyinstaller_plugin-1.1.7a0/README.md
--rw-r--r--   0        0        0     1993 2024-02-23 22:51:16.999128 poetry_pyinstaller_plugin-1.1.7a0/poetry_pyinstaller_plugin/__init__.py
--rw-r--r--   0        0        0    11495 2024-03-20 20:23:27.443614 poetry_pyinstaller_plugin-1.1.7a0/poetry_pyinstaller_plugin/plugin.py
--rw-r--r--   0        0        0     1259 2024-03-20 20:24:22.275228 poetry_pyinstaller_plugin-1.1.7a0/pyproject.toml
--rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 poetry_pyinstaller_plugin-1.1.7a0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-02-23 22:51:16.999128 poetry_pyinstaller_plugin-1.1.8/LICENSE
+-rw-r--r--   0        0        0     6819 2024-04-11 19:18:03.567478 poetry_pyinstaller_plugin-1.1.8/README.md
+-rw-r--r--   0        0        0     1993 2024-04-11 19:07:28.415027 poetry_pyinstaller_plugin-1.1.8/poetry_pyinstaller_plugin/__init__.py
+-rw-r--r--   0        0        0    12729 2024-04-11 19:07:39.767389 poetry_pyinstaller_plugin-1.1.8/poetry_pyinstaller_plugin/plugin.py
+-rw-r--r--   0        0        0     1257 2024-04-11 19:06:25.021006 poetry_pyinstaller_plugin-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     8213 1970-01-01 00:00:00.000000 poetry_pyinstaller_plugin-1.1.8/PKG-INFO
```

### Comparing `poetry_pyinstaller_plugin-1.1.7a0/LICENSE` & `poetry_pyinstaller_plugin-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_pyinstaller_plugin-1.1.7a0/README.md` & `poetry_pyinstaller_plugin-1.1.8/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -35,14 +35,22 @@
     * `all` (list): Collect all submodules, data files, and binaries for specified package(s) or module(s)
 
 `PyinstallerTarget` spec:
 * `source` (string): Path to your program entrypoint
 * `type` (string, **default:** `onedir`): Type of distribution format. Must be one of `onefile`, `onedir`
 * `bundle` (boolean, **default:** `false`): Include executable binary onto wheel
 * `noupx` (boolean, **default:** `false`) : Disable UPX archiving
+* `strip` (boolean, **default** `false`) : Apply a symbol-table strip to the executable and shared libs (not recommended for Windows)
+* `console` (boolean, **default** `false`) : Open a console window for standard i/o (default). On Windows this option has no effect if the first script is a ‘.pyw’ file.
+* `windowed` (boolean, **default** `false`) : Windows and Mac OS X: do not provide a console window for standard i/o. On Mac OS this also triggers building a Mac OS .app bundle. On Windows this option is automatically set if the first script is a ‘.pyw’ file. This option is ignored on *NIX systems.
+* `icon` (Path, **default** PyInstaller’s icon) : FILE.ico: apply the icon to a Windows executable. FILE.exe,ID: extract the icon with ID from an exe. FILE.icns: apply the icon to the .app bundle on Mac OS. Use “NONE” to not apply any icon, thereby making the OS to show some default
+* `uac_admin` (boolean, **default** `false`) : Using this option creates a Manifest that will request elevation upon application start.
+* `uac_uiaccess` (boolean, **default** `false`) : Using this option allows an elevated application to work with Remote Desktop.
+* `argv_emulation` (boolean, **default** `false`) : Enable argv emulation for macOS app bundles. If enabled, the initial open document/URL event is processed by the bootloader and the passed file paths or URLs are appended to sys.argv.
+* `arch` (string, **default** `null`) : Target architecture (macOS only; valid values: x86_64, arm64, universal2).
 
 ### Examples
 
 ```toml
 [tool.poetry-pyinstaller-plugin.scripts]
 hello-world = "my_package/main.py"
 # Equivalent to
```

### Comparing `poetry_pyinstaller_plugin-1.1.7a0/poetry_pyinstaller_plugin/__init__.py` & `poetry_pyinstaller_plugin-1.1.8/poetry_pyinstaller_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_pyinstaller_plugin-1.1.7a0/poetry_pyinstaller_plugin/plugin.py` & `poetry_pyinstaller_plugin-1.1.8/poetry_pyinstaller_plugin/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import glob
 import logging
 import os
 import sys
 import textwrap
 from importlib import reload
 from pathlib import Path
-from typing import List, Dict
+from typing import List, Dict, Optional
 
 # Reload logging after PyInstaller import (conflicts with poetry logging)
 reload(logging)
 
 from cleo.events.console_command_event import ConsoleCommandEvent
 from cleo.events.console_events import COMMAND, TERMINATE
 from cleo.events.event_dispatcher import EventDispatcher
@@ -59,20 +59,44 @@
 
     @property
     def pyinst_flags(self):
         return f"--{self.value}"
 
 
 class PyInstallerTarget(object):
-    def __init__(self, prog: str, source: str, type: str = "onedir", bundle: bool = False, noupx=False):
+    def __init__(self,
+        prog: str,
+        source: str,
+        type: str = "onedir",
+        bundle: bool = False,
+        strip: bool = False,
+        noupx: bool = False,
+        console: bool = False,
+        windowed: bool = False,
+        icon: Optional[str] = None,
+        uac_admin: bool = False,
+        uac_uiaccess: bool = False,
+        argv_emulation: bool = False,
+        arch: Optional[str] = None,
+    ):
         self.prog = prog
         self.source = Path(source).resolve()
         self.type = self._validate_type(type)
+
         self.bundled = bundle
+        self.strip = strip
         self.noupx = noupx
+        self.console = console
+        self.windowed = windowed
+        self.icon = icon
+        self.uac_admin = uac_admin
+        self.uac_uiaccess = uac_uiaccess
+        self.argv_emulation = argv_emulation
+        self.arch = arch
+
         self._platform = None
 
     def _validate_type(self, type: str):
         if type not in PyinstDistType.list():
             raise ValueError(
                 f"ValueError: Unsupported distribution type for target '{self.prog}', "
                 f"'{type}' not in {PyinstDistType.list()}."
@@ -103,16 +127,34 @@
             if collect_type in ["submodules", "data", "datas", "binaries", "all"]:
                 for module in modules:
                     collect_args.append(f"--collect-{collect_type}")
                     collect_args.append(module)
 
         args += collect_args
 
+        if self.strip:
+            args.append("--strip")
         if self.noupx:
             args.append("--noupx")
+        if self.console:
+            args.append("--console")
+        if self.windowed:
+            args.append("--windowed")
+        if self.icon:
+            args.append("--icon")
+            args.append(self.icon)
+        if self.uac_admin:
+            args.append("--uac-admin")
+        if self.uac_uiaccess:
+            args.append("--uac-uiaccess")
+        if self.argv_emulation:
+            args.append("--argv-emulation")
+        if self.arch:
+            args.append("--target-arch")
+            args.append(self.arch)
 
         venv.run(str(Path(venv.script_dirs[0]) / "pyinstaller"), *args)
 
     def bundle_wheel(self, io):
         wheels = glob.glob("*-py3-none-any.whl", root_dir="dist")
         for wheel in wheels:
             folder_to_add = Path("dist", "pyinstaller", self._platform, self.prog)
@@ -126,62 +168,65 @@
     _app: Application = None
 
     _targets: List[PyInstallerTarget]
 
     def __init__(self):
         self._targets = []
 
+    @property
     def scripts_opt_block(self) -> Dict:
         """
         Get plugins scripts options block
         :return: Dictionary of { "program": Path | Dictionary }
         """
         data = self._app.poetry.pyproject.data
         if data:
             return data.get("tool", {}).get("poetry-pyinstaller-plugin", {}).get("scripts", {})
         raise RuntimeError("Error while retrieving pyproject.toml data.")
 
+    @property
     def certifi_opt_block(self) -> Dict:
         """
         Get certifi config
         """
         data = self._app.poetry.pyproject.data
         if data:
             return data.get("tool", {}).get("poetry-pyinstaller-plugin", {}).get("certifi", {})
         raise RuntimeError("Error while retrieving pyproject.toml data.")
 
+    @property
     def collect_opt_block(self) -> Dict:
         """
         Get collect config
         """
         data = self._app.poetry.pyproject.data
         if data:
             return data.get("tool", {}).get("poetry-pyinstaller-plugin", {}).get("collect", {})
         raise RuntimeError("Error while retrieving pyproject.toml data.")
 
+    @property
     def _use_bundle(self):
         return True in [t.bundled for t in self._targets]
 
     def activate(self, application: Application) -> None:
         """
         Activation method for ApplicationPlugin
         """
         self._app = application
-        self._targets = self._parse_targets()
 
         application.event_dispatcher.add_listener(COMMAND, self._build_binaries)
         application.event_dispatcher.add_listener(TERMINATE, self._bundle_wheels)
 
     def _parse_targets(self) -> List[PyInstallerTarget]:
         """
         Parse PyInstallerTarget from pyproject.toml
         :return: List of PyInstallerTarget objects
         """
         targets = []
-        for prog_name, content in self.scripts_opt_block().items():
+        for prog_name, content in self.scripts_opt_block.items():
             # Simplest binding: prog_name = "package.source"
             if isinstance(content, str):
                 targets.append(PyInstallerTarget(prog=prog_name, source=content))
             elif isinstance(content, dict):
                 targets.append(PyInstallerTarget(prog=prog_name, **content))
         return targets
 
@@ -211,14 +256,15 @@
         command = event.command
 
         if not isinstance(command, BuildCommand):
             return
 
         io = event.io
 
+        self._targets = self._parse_targets()
         if len(self._targets) > 0:
 
             extra_indexes = {s.name: s.url for s in self._app.poetry.get_sources()}
             platform = WheelBuilder(self._app.poetry)._get_sys_tags()[0].split("-")[-1]
 
             if command.env.is_venv():
                 venv = command.env
@@ -254,15 +300,15 @@
                         *extra_index_url,
                         pip_r,
                     )
 
             if event.io.is_debug():
                 io.write_line(f"<debug>{venv_pip}</debug>")
 
-            for cert in self.certifi_opt_block().get('append', []):
+            for cert in self.certifi_opt_block.get('append', []):
                 cert_path = (self._app.poetry.pyproject_path.parent / cert).relative_to(
                     self._app.poetry.pyproject_path.parent)
 
                 io.write_line(f"  - Adding <c1>{cert_path}</c1> to certifi")
                 venv.run_python_script(textwrap.dedent(f"""
                 import certifi
                 print(certifi.where())
@@ -271,25 +317,25 @@
                         cert.write(include.read())
                 """))
 
             io.write_line(
                 f"Building <c1>binaries</c1> with PyInstaller <c1>Python {venv.version_info[0]}.{venv.version_info[1]}</c1> <debug>[{platform}]</debug>")
             for t in self._targets:
                 io.write_line(f"  - Building <info>{t.prog}</info> <debug>{t.type.name}{' BUNDLED' if t.bundled else ''}{' NOUPX' if t.noupx else ''}</debug>")
-                t.build(venv=venv, platform=platform, collect_config=self.collect_opt_block())
+                t.build(venv=venv, platform=platform, collect_config=self.collect_opt_block)
                 io.write_line(f"  - Built <success>{t.prog}</success> -> <success>'{Path('dist', 'pyinstaller', platform, t.prog)}'</success>")
 
     def _bundle_wheels(self, event: ConsoleCommandEvent, event_name: str, dispatcher: EventDispatcher) -> None:
         """
         Include binaries in wheels under data/scripts. Performed on completion of `poetry build` command.
         """
         command = event.command
         if not isinstance(command, BuildCommand):
             return
 
         io = event.io
-        if self._use_bundle():
+        if self._use_bundle:
             for t in self._targets:
                 if t.bundled:
                     t.bundle_wheel(io)
 
             self._update_wheel_platform_tag(io)
```

### Comparing `poetry_pyinstaller_plugin-1.1.7a0/pyproject.toml` & `poetry_pyinstaller_plugin-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-pyinstaller-plugin"
-version = "1.1.7a0"
+version = "1.1.8"
 description = "Poetry plugin to build and/or bundle executable binaries with PyInstaller"
 authors = ["Thomas Mahé <contact@tmahe.dev>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/thmahe/poetry-pyinstaller-plugin"
 keywords = ["poetry", "plugin", "pyinstaller", "binary"]
 classifiers = [
```

