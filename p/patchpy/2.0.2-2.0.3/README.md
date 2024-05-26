# Comparing `tmp/patchpy-2.0.2.tar.gz` & `tmp/patchpy-2.0.3.tar.gz`

## Comparing `patchpy-2.0.2.tar` & `patchpy-2.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 patchpy-2.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 patchpy-2.0.2/.python-version
--rw-r--r--   0        0        0    15936 2020-02-02 00:00:00.000000 patchpy-2.0.2/patchpy.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 patchpy-2.0.2/requirements-dev.lock
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 patchpy-2.0.2/requirements.lock
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 patchpy-2.0.2/test_patchpy.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 patchpy-2.0.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 patchpy-2.0.2/LICENSE.txt
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 patchpy-2.0.2/README.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 patchpy-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 patchpy-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 patchpy-2.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 patchpy-2.0.3/.python-version
+-rw-r--r--   0        0        0    15961 2020-02-02 00:00:00.000000 patchpy-2.0.3/patchpy.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 patchpy-2.0.3/requirements-dev.lock
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 patchpy-2.0.3/requirements.lock
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 patchpy-2.0.3/test_patchpy.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 patchpy-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 patchpy-2.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 patchpy-2.0.3/README.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 patchpy-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 patchpy-2.0.3/PKG-INFO
```

### Comparing `patchpy-2.0.2/.pre-commit-config.yaml` & `patchpy-2.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.2/patchpy.py` & `patchpy-2.0.3/patchpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         source = next(lines).removeprefix('--- ')
         if not lines or not lines.peek().startswith('+++ '):
             raise PatchPyError(f'Invalid patch header: {line}')
         target = next(lines).removeprefix('+++ ')
         source = cls._decode_path(source)
         target = cls._decode_path(target)
         kind = ModificationKind.REGULAR
-        if header and header[0].startswith('diff --git'):
+        if header and re.search(r'^diff --git ', '\n'.join(header), re.MULTILINE):
             source = source.removeprefix('a/') if source else None
             target = target.removeprefix('b/') if target else None
             kind = ModificationKind.GIT
         hunks = []
         while lines and lines.peek().startswith('@@ '):
             hunks.append(Hunk._parse(lines))
         return cls(kind=kind, header=header, source=source, target=target, hunks=hunks)
```

### Comparing `patchpy-2.0.2/requirements-dev.lock` & `patchpy-2.0.3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.2/test_patchpy.py` & `patchpy-2.0.3/test_patchpy.py`

 * *Files 9% similar despite different names*

```diff
@@ -226,7 +226,37 @@
     assert mod.target == 'sample.txt'
     assert len(mod.hunks) == 1
     # Apply the diff
     with tempfile.TemporaryDirectory() as tempdir:
         diff_file.apply(root=tempdir)
         sample_path = Path(tempdir) / 'sample.txt'
         assert sample_path.read_text() == 'Line 1\nLine 2\nLine 3\nLine 4\n'
+
+
+def test_git_commit_diff():
+    diff_file = DiffFile.from_string(
+        """From 83db48f7b3b3b7b3b7b3b7b3b7b3b7b3b7b3b7b3 Mon Sep 17 00:00:00 2001
+From: Author <123456+abc@users.no-reply.github.com>
+Date: Fri, 1 Jan 2021 00:00:00 +0000
+Subject: [PATCH] Commit message
+
+---------
+
+Co-authored-by: Co-author <123456+def@users.no-reply.github.com>
+---
+ sample.txt | 1 +
+1 file changed, 1 insertion(+)
+
+diff --git a/sample.txt b/sample.txt
+index 83db48f..f735c3d 100644
+--- a/sample.txt
++++ b/sample.txt
+@@ -1,3 +1,4 @@
+ Line 1
+ Line 2
+ Line 3
++Line 4
+"""
+    )
+    assert len(diff_file.modifications) == 1
+    assert diff_file.modifications[0].kind == ModificationKind.GIT
+    assert diff_file.modifications[0].source == 'sample.txt'
```

### Comparing `patchpy-2.0.2/LICENSE.txt` & `patchpy-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.2/README.md` & `patchpy-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.2/pyproject.toml` & `patchpy-2.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "patchpy"
-version = "2.0.2"
+version = "2.0.3"
 description = "A modern Python library for patch file parsing (diff file parsing)"
 authors = [
     { name = "Matthew D. Scholefield", email = "matthew331199@gmail.com" },
 ]
 dependencies = ["more-itertools>=10.2.0"]
 readme = "README.md"
 requires-python = ">= 3.9"
```

### Comparing `patchpy-2.0.2/PKG-INFO` & `patchpy-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: patchpy
-Version: 2.0.2
+Version: 2.0.3
 Summary: A modern Python library for patch file parsing (diff file parsing)
 Author-email: "Matthew D. Scholefield" <matthew331199@gmail.com>
 License: MIT
 License-File: LICENSE.txt
 Requires-Python: >=3.9
 Requires-Dist: more-itertools>=10.2.0
 Description-Content-Type: text/markdown
```

