# Comparing `tmp/inline_snapshot-0.8.2.tar.gz` & `tmp/inline_snapshot-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inline_snapshot-0.8.2.tar", max compression
+gzip compressed data, was "inline_snapshot-0.9.0.tar", max compression
```

## Comparing `inline_snapshot-0.8.2.tar` & `inline_snapshot-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1082 2024-02-18 19:11:48.706993 inline_snapshot-0.8.2/LICENSE
--rw-r--r--   0        0        0     4642 2024-04-24 07:01:03.261658 inline_snapshot-0.8.2/README.md
--rw-r--r--   0        0        0      176 2024-04-24 19:10:05.207071 inline_snapshot-0.8.2/inline_snapshot/__init__.py
--rw-r--r--   0        0        0     1400 2024-04-09 10:01:00.849766 inline_snapshot-0.8.2/inline_snapshot/_align.py
--rw-r--r--   0        0        0     5733 2024-04-21 20:44:07.304452 inline_snapshot-0.8.2/inline_snapshot/_change.py
--rw-r--r--   0        0        0      539 2024-02-27 18:46:50.343219 inline_snapshot-0.8.2/inline_snapshot/_config.py
--rw-r--r--   0        0        0     4944 2024-04-21 20:44:07.304452 inline_snapshot-0.8.2/inline_snapshot/_external.py
--rw-r--r--   0        0        0     2779 2024-04-21 20:44:07.304452 inline_snapshot-0.8.2/inline_snapshot/_find_external.py
--rw-r--r--   0        0        0      372 2024-02-27 18:46:50.343219 inline_snapshot-0.8.2/inline_snapshot/_format.py
--rw-r--r--   0        0        0    22110 2024-04-24 19:10:02.339013 inline_snapshot-0.8.2/inline_snapshot/_inline_snapshot.py
--rw-r--r--   0        0        0      452 2024-04-09 10:01:00.849766 inline_snapshot-0.8.2/inline_snapshot/_location.py
--rw-r--r--   0        0        0     5911 2024-04-21 20:44:07.304452 inline_snapshot-0.8.2/inline_snapshot/_rewrite_code.py
--rw-r--r--   0        0        0       64 2024-04-09 10:01:00.849766 inline_snapshot-0.8.2/inline_snapshot/_sentinels.py
--rw-r--r--   0        0        0     3565 2024-04-09 10:01:00.849766 inline_snapshot-0.8.2/inline_snapshot/_utils.py
--rw-r--r--   0        0        0        0 2024-02-27 18:46:50.343219 inline_snapshot-0.8.2/inline_snapshot/py.typed
--rw-r--r--   0        0        0     6417 2024-04-24 19:10:02.339013 inline_snapshot-0.8.2/inline_snapshot/pytest_plugin.py
--rw-r--r--   0        0        0     2640 2024-04-24 19:10:05.223071 inline_snapshot-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 inline_snapshot-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-02-18 19:11:48.706993 inline_snapshot-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4642 2024-05-06 19:50:37.275128 inline_snapshot-0.9.0/README.md
+-rw-r--r--   0        0        0      176 2024-05-07 18:43:24.361519 inline_snapshot-0.9.0/inline_snapshot/__init__.py
+-rw-r--r--   0        0        0     1400 2024-04-09 10:01:00.849766 inline_snapshot-0.9.0/inline_snapshot/_align.py
+-rw-r--r--   0        0        0     5733 2024-05-02 21:08:12.260879 inline_snapshot-0.9.0/inline_snapshot/_change.py
+-rw-r--r--   0        0        0      539 2024-02-27 18:46:50.343219 inline_snapshot-0.9.0/inline_snapshot/_config.py
+-rw-r--r--   0        0        0     5006 2024-05-07 18:42:23.320255 inline_snapshot-0.9.0/inline_snapshot/_external.py
+-rw-r--r--   0        0        0     2779 2024-05-02 21:08:12.260879 inline_snapshot-0.9.0/inline_snapshot/_find_external.py
+-rw-r--r--   0        0        0      372 2024-02-27 18:46:50.343219 inline_snapshot-0.9.0/inline_snapshot/_format.py
+-rw-r--r--   0        0        0    22110 2024-05-02 21:08:12.260879 inline_snapshot-0.9.0/inline_snapshot/_inline_snapshot.py
+-rw-r--r--   0        0        0      452 2024-04-09 10:01:00.849766 inline_snapshot-0.9.0/inline_snapshot/_location.py
+-rw-r--r--   0        0        0     5911 2024-05-02 21:08:12.260879 inline_snapshot-0.9.0/inline_snapshot/_rewrite_code.py
+-rw-r--r--   0        0        0       64 2024-04-09 10:01:00.849766 inline_snapshot-0.9.0/inline_snapshot/_sentinels.py
+-rw-r--r--   0        0        0     3902 2024-05-07 18:42:16.688118 inline_snapshot-0.9.0/inline_snapshot/_utils.py
+-rw-r--r--   0        0        0        0 2024-02-27 18:46:50.343219 inline_snapshot-0.9.0/inline_snapshot/py.typed
+-rw-r--r--   0        0        0     6944 2024-05-07 18:42:23.320255 inline_snapshot-0.9.0/inline_snapshot/pytest_plugin.py
+-rw-r--r--   0        0        0     2640 2024-05-07 18:43:24.381520 inline_snapshot-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 inline_snapshot-0.9.0/PKG-INFO
```

### Comparing `inline_snapshot-0.8.2/LICENSE` & `inline_snapshot-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.2/README.md` & `inline_snapshot-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.2/inline_snapshot/_align.py` & `inline_snapshot-0.9.0/inline_snapshot/_align.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.2/inline_snapshot/_change.py` & `inline_snapshot-0.9.0/inline_snapshot/_change.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.2/inline_snapshot/_config.py` & `inline_snapshot-0.9.0/inline_snapshot/_config.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.2/inline_snapshot/_external.py` & `inline_snapshot-0.9.0/inline_snapshot/_external.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,18 @@
     def list(self) -> Set[str]:
         if self.directory.exists():
             return {item.name for item in self.directory.iterdir()} - {".gitignore"}
         else:
             return set()
 
     def persist(self, name):
-        file = self._lookup_path(name)
+        try:
+            file = self._lookup_path(name)
+        except HashError:
+            return
         if file.stem.endswith("-new"):
             stem = file.stem[:-4]
             file.rename(file.with_name(stem + file.suffix))
 
     def _lookup_path(self, name) -> pathlib.Path:
         files = list(self.directory.glob(name))
```

### Comparing `inline_snapshot-0.8.2/inline_snapshot/_find_external.py` & `inline_snapshot-0.9.0/inline_snapshot/_find_external.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.2/inline_snapshot/_inline_snapshot.py` & `inline_snapshot-0.9.0/inline_snapshot/_inline_snapshot.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.2/inline_snapshot/_rewrite_code.py` & `inline_snapshot-0.9.0/inline_snapshot/_rewrite_code.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.2/inline_snapshot/_utils.py` & `inline_snapshot-0.9.0/inline_snapshot/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,21 +22,21 @@
                 current_string = ast.literal_eval(t.string)
             else:
                 current_string += ast.literal_eval(t.string)
 
             continue
 
         if current_string is not None:
-            yield (token.STRING, repr(current_string))
+            yield simple_token(token.STRING, repr(current_string))
             current_string = None
 
         yield t
 
     if current_string is not None:
-        yield (token.STRING, repr(current_string))
+        yield simple_token(token.STRING, repr(current_string))
 
 
 ignore_tokens = (token.NEWLINE, token.ENDMARKER, token.NL)
 
 
 # based on ast.unparse
 def _str_literal_helper(string, *, quote_types):
@@ -86,15 +86,23 @@
 
     if not string.endswith("\n"):
         string = string + "\\\n"
 
     return f"{quote_type}{string}{quote_type}"
 
 
-simple_token = namedtuple("simple_token", "type,string")
+class simple_token(namedtuple("simple_token", "type,string")):
+
+    def __eq__(self, other):
+        if self.type == other.type == 3:
+            return ast.literal_eval(self.string) == ast.literal_eval(
+                other.string
+            ) and self.string.replace("'", '"') == other.string.replace("'", '"')
+        else:
+            return super().__eq__(other)
 
 
 def value_to_token(value):
     input = io.StringIO(repr(value))
 
     def map_string(tok):
         """Convert strings with newlines in triple quoted strings."""
```

### Comparing `inline_snapshot-0.8.2/inline_snapshot/pytest_plugin.py` & `inline_snapshot-0.9.0/inline_snapshot/pytest_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,24 +31,36 @@
         "--inline-snapshot-disable",
         action="store_true",
         dest="inline_snapshot_disable",
         help="disable snapshot logic",
     )
 
 
+def xdist_running(config):
+    return (
+        hasattr(config.option, "numprocesses")
+        and config.option.numprocesses is not None
+    )
+
+
 def pytest_configure(config):
     flags = config.option.inline_snapshot.split(",")
     flags = [flag for flag in flags if flag]
 
     if config.option.inline_snapshot_disable and flags:
         raise pytest.UsageError(
             f"--inline-snapshot-disable can not be combined with other flags ({','.join(flags)})"
         )
 
-    _inline_snapshot._active = not config.option.inline_snapshot_disable
+    if xdist_running(config) and flags:
+        raise pytest.UsageError(f"inline-snapshot can not be combined with xdist")
+
+    _inline_snapshot._active = not (
+        config.option.inline_snapshot_disable or xdist_running(config)
+    )
 
     _inline_snapshot._update_flags = _inline_snapshot.Flags(set(flags))
 
     snapshot_path = Path(config.rootpath) / ".inline-snapshot/external"
     _external.storage = _external.DiscStorage(snapshot_path)
 
     _config.config = _config.read_config(config.rootpath / "pyproject.toml")
@@ -112,14 +124,22 @@
         )
 
     if results:
         return results[0]
 
 
 def pytest_terminal_summary(terminalreporter, exitstatus, config):
+
+    if xdist_running(config):
+        terminalreporter.section("inline snapshot")
+        terminalreporter.write(
+            "INFO: inline-snapshot was disabled because you used xdist\n"
+        )
+        return
+
     if not _inline_snapshot._active:
         return
 
     recorder = ChangeRecorder.current
 
     terminalreporter.section("inline snapshot")
 
@@ -153,14 +173,15 @@
 
     report(
         "update",
         "Info: {num} snapshots changed their representation (--inline-snapshot=update)",
     )
 
     if _inline_snapshot._update_flags.change_something():
+
         count = {"create": 0, "fix": 0, "trim": 0, "update": 0}
 
         for snapshot in _inline_snapshot.snapshots.values():
             for flag in snapshot._flags:
                 assert flag in ("create", "fix", "trim", "update"), flag
                 count[flag] += 1
             snapshot._change()
```

### Comparing `inline_snapshot-0.8.2/pyproject.toml` & `inline_snapshot-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 ]
 description = "golden master/snapshot/approval testing library which puts the values right into your source code"
 keywords = ["pytest", "testing", "snapshot", "approval", "golden-master"]
 license = "MIT"
 name = "inline-snapshot"
 readme = "README.md"
 repository = "https://github.com/15r10nk/inline-snapshots"
-version = "0.8.2"
+version = "0.9.0"
 
 [tool.poetry.dependencies]
 asttokens = ">=2.0.5"
 black = ">=23.3.0"
 click = ">=8.1.4"
 executing = ">=2.0.0"
 python = ">=3.7"
```

### Comparing `inline_snapshot-0.8.2/PKG-INFO` & `inline_snapshot-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inline-snapshot
-Version: 0.8.2
+Version: 0.9.0
 Summary: golden master/snapshot/approval testing library which puts the values right into your source code
 Home-page: https://github.com/15r10nk/inline-snapshots
 License: MIT
 Keywords: pytest,testing,snapshot,approval,golden-master
 Author: Frank Hoffmann
 Author-email: 15r10nk@polarbit.de
 Requires-Python: >=3.7
```

