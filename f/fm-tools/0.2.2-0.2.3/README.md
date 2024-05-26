# Comparing `tmp/fm_tools-0.2.2.tar.gz` & `tmp/fm_tools-0.2.3.tar.gz`

## Comparing `fm_tools-0.2.2.tar` & `fm_tools-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fm_tools-0.2.2/.gitlab-ci.yml
--rwxr-xr-x   0        0        0     1425 2020-02-02 00:00:00.000000 fm_tools-0.2.2/minor_release.sh
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fm_tools-0.2.2/.reuse/templates/header.jinja2
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 fm_tools-0.2.2/LICENSES/MIT.txt
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fm_tools-0.2.2/src/fm_tools/__init__.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 fm_tools-0.2.2/src/fm_tools/benchexec_helper.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 fm_tools-0.2.2/src/fm_tools/download.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fm_tools-0.2.2/src/fm_tools/exceptions.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fm_tools-0.2.2/src/fm_tools/files.py
--rw-r--r--   0        0        0    10289 2020-02-02 00:00:00.000000 fm_tools-0.2.2/src/fm_tools/fmdata.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 fm_tools-0.2.2/src/fm_tools/run.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 fm_tools-0.2.2/src/fm_tools/types.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 fm_tools-0.2.2/src/fm_tools/zenodo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fm_tools-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 fm_tools-0.2.2/tests/test_command.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 fm_tools-0.2.2/tests/test_download.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fm_tools-0.2.2/tests/test_unzip.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fm_tools-0.2.2/tests/resources/archive.zip
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fm_tools-0.2.2/tests/resources/archive.zip.license
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 fm_tools-0.2.2/.gitignore
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fm_tools-0.2.2/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 fm_tools-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 fm_tools-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fm_tools-0.2.3/.gitlab-ci.yml
+-rwxr-xr-x   0        0        0     1425 2020-02-02 00:00:00.000000 fm_tools-0.2.3/minor_release.sh
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fm_tools-0.2.3/.reuse/templates/header.jinja2
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 fm_tools-0.2.3/LICENSES/MIT.txt
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fm_tools-0.2.3/src/fm_tools/__init__.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 fm_tools-0.2.3/src/fm_tools/benchexec_helper.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 fm_tools-0.2.3/src/fm_tools/download.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fm_tools-0.2.3/src/fm_tools/exceptions.py
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fm_tools-0.2.3/src/fm_tools/files.py
+-rw-r--r--   0        0        0    10327 2020-02-02 00:00:00.000000 fm_tools-0.2.3/src/fm_tools/fmdata.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 fm_tools-0.2.3/src/fm_tools/run.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 fm_tools-0.2.3/src/fm_tools/types.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 fm_tools-0.2.3/src/fm_tools/zenodo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fm_tools-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 fm_tools-0.2.3/tests/test_command.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 fm_tools-0.2.3/tests/test_download.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fm_tools-0.2.3/tests/test_unzip.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fm_tools-0.2.3/tests/resources/archive.zip
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fm_tools-0.2.3/tests/resources/archive.zip.license
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 fm_tools-0.2.3/.gitignore
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fm_tools-0.2.3/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 fm_tools-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 fm_tools-0.2.3/PKG-INFO
```

### Comparing `fm_tools-0.2.2/.gitlab-ci.yml` & `fm_tools-0.2.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/minor_release.sh` & `fm_tools-0.2.3/minor_release.sh`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/LICENSES/MIT.txt` & `fm_tools-0.2.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/src/fm_tools/benchexec_helper.py` & `fm_tools-0.2.3/src/fm_tools/benchexec_helper.py`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/src/fm_tools/download.py` & `fm_tools-0.2.3/src/fm_tools/download.py`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/src/fm_tools/exceptions.py` & `fm_tools-0.2.3/src/fm_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/src/fm_tools/files.py` & `fm_tools-0.2.3/src/fm_tools/files.py`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/src/fm_tools/fmdata.py` & `fm_tools-0.2.3/src/fm_tools/fmdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,16 @@
 
     def make_available(self):
         """
         Make the resolved tool-info-module available for import.
         If necessary the tool-info-module is downloaded into a temporary file.
         """
         self.resolve()
-        sys.path.insert(0, str(self._target_location.parent))
+        if self._target_location:
+            sys.path.insert(0, str(self._target_location.parent))
 
     def __str__(self):
         return self.resolved or self.raw
 
     def __del__(self):
         if self._propagate_delete:
             shutil.rmtree(self._target_location.parent)
```

### Comparing `fm_tools-0.2.2/src/fm_tools/run.py` & `fm_tools-0.2.3/src/fm_tools/run.py`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/src/fm_tools/types.py` & `fm_tools-0.2.3/src/fm_tools/types.py`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/src/fm_tools/zenodo.py` & `fm_tools-0.2.3/src/fm_tools/zenodo.py`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/tests/test_command.py` & `fm_tools-0.2.3/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/tests/test_download.py` & `fm_tools-0.2.3/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/tests/test_unzip.py` & `fm_tools-0.2.3/tests/test_unzip.py`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/tests/resources/archive.zip` & `fm_tools-0.2.3/tests/resources/archive.zip`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/README.md` & `fm_tools-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/pyproject.toml` & `fm_tools-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fm_tools-0.2.2/PKG-INFO` & `fm_tools-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fm-tools
-Version: 0.2.2
+Version: 0.2.3
 Author-email: Henrik Wachowitz <henrik.wachowitz@ifi.lmu.de>
 Maintainer-email: Henrik Wachowitz <henrik.wachowitz@ifi.lmu.de>, Dirk Beyer <dirk.beyer@sosy-lab.org>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

