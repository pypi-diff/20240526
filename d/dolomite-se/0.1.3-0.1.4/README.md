# Comparing `tmp/dolomite_se-0.1.3.tar.gz` & `tmp/dolomite_se-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolomite_se-0.1.3.tar", last modified: Tue May 21 20:11:39 2024, max compression
+gzip compressed data, was "dolomite_se-0.1.4.tar", last modified: Sun May 26 01:07:06 2024, max compression
```

## Comparing `dolomite_se-0.1.3.tar` & `dolomite_se-0.1.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:11:39.172897 dolomite_se-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:11:39.160897 dolomite_se-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:11:39.164897 dolomite_se-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-21 20:11:39.172897 dolomite_se-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:11:39.164897 dolomite_se-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:11:39.164897 dolomite_se-0.1.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-21 20:11:39.172897 dolomite_se-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:11:39.160897 dolomite_se-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:11:39.168897 dolomite_se-0.1.3/src/dolomite_se/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/src/dolomite_se/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/src/dolomite_se/read_ranged_summarized_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/src/dolomite_se/read_summarized_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/src/dolomite_se/save_ranged_summarized_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/src/dolomite_se/save_summarized_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/src/dolomite_se/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:11:39.168897 dolomite_se-0.1.3/src/dolomite_se.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-21 20:11:39.000000 dolomite_se-0.1.3/src/dolomite_se.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-21 20:11:39.000000 dolomite_se-0.1.3/src/dolomite_se.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:11:39.000000 dolomite_se-0.1.3/src/dolomite_se.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:11:38.000000 dolomite_se-0.1.3/src/dolomite_se.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-21 20:11:39.000000 dolomite_se-0.1.3/src/dolomite_se.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-21 20:11:39.000000 dolomite_se-0.1.3/src/dolomite_se.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:11:39.168897 dolomite_se-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/tests/test_range_summarized_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/tests/test_summarized_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-21 20:10:33.000000 dolomite_se-0.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:07:06.851133 dolomite_se-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:07:06.839133 dolomite_se-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:07:06.843133 dolomite_se-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-26 01:07:06.851133 dolomite_se-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:07:06.847133 dolomite_se-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:07:06.847133 dolomite_se-0.1.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-26 01:07:06.851133 dolomite_se-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:07:06.839133 dolomite_se-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:07:06.847133 dolomite_se-0.1.4/src/dolomite_se/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/src/dolomite_se/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/src/dolomite_se/read_ranged_summarized_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/src/dolomite_se/read_summarized_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/src/dolomite_se/save_ranged_summarized_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/src/dolomite_se/save_summarized_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/src/dolomite_se/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:07:06.847133 dolomite_se-0.1.4/src/dolomite_se.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-26 01:07:06.000000 dolomite_se-0.1.4/src/dolomite_se.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-26 01:07:06.000000 dolomite_se-0.1.4/src/dolomite_se.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:07:06.000000 dolomite_se-0.1.4/src/dolomite_se.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:07:06.000000 dolomite_se-0.1.4/src/dolomite_se.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-26 01:07:06.000000 dolomite_se-0.1.4/src/dolomite_se.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 01:07:06.000000 dolomite_se-0.1.4/src/dolomite_se.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:07:06.847133 dolomite_se-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/tests/test_range_summarized_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/tests/test_summarized_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-26 01:06:00.000000 dolomite_se-0.1.4/tox.ini
```

### Comparing `dolomite_se-0.1.3/.coveragerc` & `dolomite_se-0.1.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/.github/workflows/pypi-publish.yml` & `dolomite_se-0.1.4/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/.github/workflows/pypi-test.yml` & `dolomite_se-0.1.4/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/.gitignore` & `dolomite_se-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/.readthedocs.yml` & `dolomite_se-0.1.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/CONTRIBUTING.md` & `dolomite_se-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/LICENSE.txt` & `dolomite_se-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/PKG-INFO` & `dolomite_se-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolomite-se
-Version: 0.1.3
+Version: 0.1.4
 Summary: Save and load summarized experiments in the dolomite framework!
 Home-page: https://github.com/ArtifactDB/dolomite-se
 Author: LTLA
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/dolomite-se
 Platform: any
```

### Comparing `dolomite_se-0.1.3/README.md` & `dolomite_se-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/docs/Makefile` & `dolomite_se-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/docs/conf.py` & `dolomite_se-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/docs/index.md` & `dolomite_se-0.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/setup.cfg` & `dolomite_se-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/setup.py` & `dolomite_se-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/src/dolomite_se/__init__.py` & `dolomite_se-0.1.4/src/dolomite_se/__init__.py`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/src/dolomite_se/read_ranged_summarized_experiment.py` & `dolomite_se-0.1.4/src/dolomite_se/read_ranged_summarized_experiment.py`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/src/dolomite_se/read_summarized_experiment.py` & `dolomite_se-0.1.4/src/dolomite_se/read_summarized_experiment.py`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/src/dolomite_se/save_ranged_summarized_experiment.py` & `dolomite_se-0.1.4/src/dolomite_se/save_ranged_summarized_experiment.py`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/src/dolomite_se/save_summarized_experiment.py` & `dolomite_se-0.1.4/src/dolomite_se/save_summarized_experiment.py`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/src/dolomite_se/utils.py` & `dolomite_se-0.1.4/src/dolomite_se/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         with open(os.path.join(_assays_path, "names.json"), "w") as handle:
             json.dump(_assay_names, handle)
 
         for _aidx, _aname in enumerate(_assay_names):
             _assay_save_path = os.path.join(_assays_path, str(_aidx))
             try:
                 dl.alt_save_object(
-                    x.assays[_aname], path=_assay_save_path, **assay_args
+                    x.assays[_aname], path=_assay_save_path, **assay_args, **kwargs
                 )
             except Exception as ex:
                 raise RuntimeError(
                     "failed to stage assay '"
                     + _aname
                     + "' for "
                     + str(type(x))
```

### Comparing `dolomite_se-0.1.3/src/dolomite_se.egg-info/PKG-INFO` & `dolomite_se-0.1.4/src/dolomite_se.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolomite-se
-Version: 0.1.3
+Version: 0.1.4
 Summary: Save and load summarized experiments in the dolomite framework!
 Home-page: https://github.com/ArtifactDB/dolomite-se
 Author: LTLA
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/dolomite-se
 Platform: any
```

### Comparing `dolomite_se-0.1.3/src/dolomite_se.egg-info/SOURCES.txt` & `dolomite_se-0.1.4/src/dolomite_se.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/tests/test_range_summarized_experiment.py` & `dolomite_se-0.1.4/tests/test_range_summarized_experiment.py`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/tests/test_summarized_experiment.py` & `dolomite_se-0.1.4/tests/test_summarized_experiment.py`

 * *Files identical despite different names*

### Comparing `dolomite_se-0.1.3/tox.ini` & `dolomite_se-0.1.4/tox.ini`

 * *Files identical despite different names*

