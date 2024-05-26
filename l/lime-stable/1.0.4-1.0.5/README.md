# Comparing `tmp/lime-stable-1.0.4.tar.gz` & `tmp/lime-stable-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lime-stable-1.0.4.tar", last modified: Fri May 17 20:31:12 2024, max compression
+gzip compressed data, was "lime-stable-1.0.5.tar", last modified: Sat May 25 23:59:36 2024, max compression
```

## Comparing `lime-stable-1.0.4.tar` & `lime-stable-1.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-17 20:31:12.112697 lime-stable-1.0.4/
--rw-rw-r--   0 vital     (1000) vital     (1000)    35608 2024-04-25 13:12:45.000000 lime-stable-1.0.4/LICENSE.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)       63 2024-04-25 13:06:20.000000 lime-stable-1.0.4/MANIFEST.in
--rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-17 20:31:12.112697 lime-stable-1.0.4/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)     2647 2024-04-25 13:09:22.000000 lime-stable-1.0.4/README.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)     1148 2024-05-17 20:01:34.000000 lime-stable-1.0.4/pyproject.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      433 2024-05-17 20:31:12.112697 lime-stable-1.0.4/setup.cfg
--rw-rw-r--   0 vital     (1000) vital     (1000)     1187 2024-04-25 13:12:39.000000 lime-stable-1.0.4/setup.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-17 20:31:12.108698 lime-stable-1.0.4/src/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-17 20:31:12.112697 lime-stable-1.0.4/src/lime/
--rw-rw-r--   0 vital     (1000) vital     (1000)     1307 2024-04-25 21:14:21.000000 lime-stable-1.0.4/src/lime/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    12833 2024-05-17 20:01:34.000000 lime-stable-1.0.4/src/lime/config.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)    31483 2024-05-03 20:18:23.000000 lime-stable-1.0.4/src/lime/io.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     2795 2024-04-24 14:30:56.000000 lime-stable-1.0.4/src/lime/logo.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    38372 2024-04-29 17:41:51.000000 lime-stable-1.0.4/src/lime/model.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    73354 2024-05-01 22:06:07.000000 lime-stable-1.0.4/src/lime/observations.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    82245 2024-05-17 14:34:08.000000 lime-stable-1.0.4/src/lime/plots.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    70645 2024-05-17 20:14:58.000000 lime-stable-1.0.4/src/lime/plots_interactive.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    33794 2024-05-17 19:51:29.000000 lime-stable-1.0.4/src/lime/read_fits.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    24985 2024-05-01 23:08:37.000000 lime-stable-1.0.4/src/lime/recognition.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-17 20:31:12.112697 lime-stable-1.0.4/src/lime/resources/
--rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:04:12.000000 lime-stable-1.0.4/src/lime/resources/parent_bands.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:03:27.000000 lime-stable-1.0.4/src/lime/resources/parent_bands_BackUp.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    10111 2024-04-22 21:42:02.000000 lime-stable-1.0.4/src/lime/resources/types_params.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    14146 2024-04-25 13:02:58.000000 lime-stable-1.0.4/src/lime/tables.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    34917 2024-05-17 14:54:27.000000 lime-stable-1.0.4/src/lime/tools.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    29081 2024-04-25 14:14:19.000000 lime-stable-1.0.4/src/lime/transitions.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    37147 2024-04-29 02:03:22.000000 lime-stable-1.0.4/src/lime/workflow.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-17 20:31:12.112697 lime-stable-1.0.4/src/lime_stable.egg-info/
--rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-17 20:31:12.000000 lime-stable-1.0.4/src/lime_stable.egg-info/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)      853 2024-05-17 20:31:12.000000 lime-stable-1.0.4/src/lime_stable.egg-info/SOURCES.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-17 20:31:12.000000 lime-stable-1.0.4/src/lime_stable.egg-info/dependency_links.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      252 2024-05-17 20:31:12.000000 lime-stable-1.0.4/src/lime_stable.egg-info/requires.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        5 2024-05-17 20:31:12.000000 lime-stable-1.0.4/src/lime_stable.egg-info/top_level.txt
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-17 20:31:12.112697 lime-stable-1.0.4/tests/
--rw-rw-r--   0 vital     (1000) vital     (1000)      994 2024-04-24 14:46:28.000000 lime-stable-1.0.4/tests/test_astro.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     7088 2024-04-16 20:37:49.000000 lime-stable-1.0.4/tests/test_cube.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     3550 2024-04-24 14:46:41.000000 lime-stable-1.0.4/tests/test_io.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     7795 2024-04-24 16:03:41.000000 lime-stable-1.0.4/tests/test_line.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4345 2024-04-25 13:05:21.000000 lime-stable-1.0.4/tests/test_model.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     7374 2024-05-17 19:54:25.000000 lime-stable-1.0.4/tests/test_read_fits.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     2013 2024-04-10 16:19:13.000000 lime-stable-1.0.4/tests/test_sample.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    11180 2024-04-24 14:43:43.000000 lime-stable-1.0.4/tests/test_spectrum.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    13391 2024-04-24 14:25:22.000000 lime-stable-1.0.4/tests/test_tools.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-25 23:59:36.969235 lime-stable-1.0.5/
+-rw-rw-r--   0 vital     (1000) vital     (1000)    35608 2024-04-25 13:12:45.000000 lime-stable-1.0.5/LICENSE.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)       63 2024-04-25 13:06:20.000000 lime-stable-1.0.5/MANIFEST.in
+-rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-25 23:59:36.969235 lime-stable-1.0.5/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2647 2024-04-25 13:09:22.000000 lime-stable-1.0.5/README.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1148 2024-05-25 23:52:06.000000 lime-stable-1.0.5/pyproject.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      433 2024-05-25 23:59:36.969235 lime-stable-1.0.5/setup.cfg
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1187 2024-04-25 13:12:39.000000 lime-stable-1.0.5/setup.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-25 23:59:36.965235 lime-stable-1.0.5/src/
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-25 23:59:36.969235 lime-stable-1.0.5/src/lime/
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1307 2024-04-25 21:14:21.000000 lime-stable-1.0.5/src/lime/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    12833 2024-05-25 23:52:06.000000 lime-stable-1.0.5/src/lime/config.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)    31483 2024-05-03 20:18:23.000000 lime-stable-1.0.5/src/lime/io.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2795 2024-04-24 14:30:56.000000 lime-stable-1.0.5/src/lime/logo.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    38372 2024-04-29 17:41:51.000000 lime-stable-1.0.5/src/lime/model.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    73354 2024-05-01 22:06:07.000000 lime-stable-1.0.5/src/lime/observations.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    82245 2024-05-17 14:34:08.000000 lime-stable-1.0.5/src/lime/plots.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    70645 2024-05-17 20:14:58.000000 lime-stable-1.0.5/src/lime/plots_interactive.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    33794 2024-05-17 19:51:29.000000 lime-stable-1.0.5/src/lime/read_fits.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    24985 2024-05-01 23:08:37.000000 lime-stable-1.0.5/src/lime/recognition.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-25 23:59:36.969235 lime-stable-1.0.5/src/lime/resources/
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:04:12.000000 lime-stable-1.0.5/src/lime/resources/parent_bands.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:03:27.000000 lime-stable-1.0.5/src/lime/resources/parent_bands_BackUp.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10111 2024-04-22 21:42:02.000000 lime-stable-1.0.5/src/lime/resources/types_params.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    14146 2024-04-25 13:02:58.000000 lime-stable-1.0.5/src/lime/tables.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    34917 2024-05-17 14:54:27.000000 lime-stable-1.0.5/src/lime/tools.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    29081 2024-04-25 14:14:19.000000 lime-stable-1.0.5/src/lime/transitions.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    37143 2024-05-25 23:38:39.000000 lime-stable-1.0.5/src/lime/workflow.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-25 23:59:36.969235 lime-stable-1.0.5/src/lime_stable.egg-info/
+-rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-25 23:59:36.000000 lime-stable-1.0.5/src/lime_stable.egg-info/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)      853 2024-05-25 23:59:36.000000 lime-stable-1.0.5/src/lime_stable.egg-info/SOURCES.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-25 23:59:36.000000 lime-stable-1.0.5/src/lime_stable.egg-info/dependency_links.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      252 2024-05-25 23:59:36.000000 lime-stable-1.0.5/src/lime_stable.egg-info/requires.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        5 2024-05-25 23:59:36.000000 lime-stable-1.0.5/src/lime_stable.egg-info/top_level.txt
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-25 23:59:36.969235 lime-stable-1.0.5/tests/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      994 2024-04-24 14:46:28.000000 lime-stable-1.0.5/tests/test_astro.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7088 2024-04-16 20:37:49.000000 lime-stable-1.0.5/tests/test_cube.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     3550 2024-04-24 14:46:41.000000 lime-stable-1.0.5/tests/test_io.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7795 2024-04-24 16:03:41.000000 lime-stable-1.0.5/tests/test_line.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4345 2024-04-25 13:05:21.000000 lime-stable-1.0.5/tests/test_model.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7374 2024-05-17 19:54:25.000000 lime-stable-1.0.5/tests/test_read_fits.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2013 2024-04-10 16:19:13.000000 lime-stable-1.0.5/tests/test_sample.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    11180 2024-04-24 14:43:43.000000 lime-stable-1.0.5/tests/test_spectrum.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    13391 2024-04-24 14:25:22.000000 lime-stable-1.0.5/tests/test_tools.py
```

### Comparing `lime-stable-1.0.4/LICENSE.rst` & `lime-stable-1.0.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/PKG-INFO` & `lime-stable-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 1.0.4
+Version: 1.0.5
 Summary: Line measuring algorithm for astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lime-stable-1.0.4/README.rst` & `lime-stable-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/pyproject.toml` & `lime-stable-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lime-stable"
-version = "1.0.4"
+version = "1.0.5"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "COPYING"}
 authors = [{name = "Vital Fernández", email = "vgf@umich.edu"}]
 description = "Line measuring algorithm for astronomical spectra"
 
 dependencies = ["asdf~=3.0",
```

### Comparing `lime-stable-1.0.4/setup.py` & `lime-stable-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/__init__.py` & `lime-stable-1.0.5/src/lime/__init__.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/config.toml` & `lime-stable-1.0.5/src/lime/config.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = 'lime-stable'
-version = '1.0.4'
+version = '1.0.5'
 
 [colors] #Default theme
 default.bg = '#FFFFFF'
 default.fg = '#000000'
 default.cont_band = '#8c564b'
 default.line_band = '#b5bd61'
 default.color_cycle = ['#279e68', '#d62728', '#aa40fc', '#8c564b',  '#e377c2', '#7f7f7f',
```

### Comparing `lime-stable-1.0.4/src/lime/io.py` & `lime-stable-1.0.5/src/lime/io.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/logo.py` & `lime-stable-1.0.5/src/lime/logo.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/model.py` & `lime-stable-1.0.5/src/lime/model.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/observations.py` & `lime-stable-1.0.5/src/lime/observations.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/plots.py` & `lime-stable-1.0.5/src/lime/plots.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/plots_interactive.py` & `lime-stable-1.0.5/src/lime/plots_interactive.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/read_fits.py` & `lime-stable-1.0.5/src/lime/read_fits.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/recognition.py` & `lime-stable-1.0.5/src/lime/recognition.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/resources/parent_bands.txt` & `lime-stable-1.0.5/src/lime/resources/parent_bands.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/resources/parent_bands_BackUp.txt` & `lime-stable-1.0.5/src/lime/resources/parent_bands_BackUp.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/resources/types_params.txt` & `lime-stable-1.0.5/src/lime/resources/types_params.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/tables.py` & `lime-stable-1.0.5/src/lime/tables.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/tools.py` & `lime-stable-1.0.5/src/lime/tools.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/transitions.py` & `lime-stable-1.0.5/src/lime/transitions.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/src/lime/workflow.py` & `lime-stable-1.0.5/src/lime/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
                 bands = bands.loc[idcs]
 
             # Load configuration
             input_conf = check_fit_conf(fit_conf, default_conf_prefix, id_conf_prefix)
 
             # Line detection if requested
             if line_detection:
-                cont_fit_conf = input_conf.get('continuum_fit', {})
+                cont_fit_conf = input_conf.get('continuum', {})
                 self._spec.fit.continuum(**cont_fit_conf)
 
                 detect_conf = input_conf.get('line_detection', {})
                 bands = self._spec.line_detection(bands, **detect_conf)
 
             # Define lines to treat through the lines
             label_list = bands.index.to_numpy()
```

### Comparing `lime-stable-1.0.4/src/lime_stable.egg-info/PKG-INFO` & `lime-stable-1.0.5/src/lime_stable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 1.0.4
+Version: 1.0.5
 Summary: Line measuring algorithm for astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lime-stable-1.0.4/src/lime_stable.egg-info/SOURCES.txt` & `lime-stable-1.0.5/src/lime_stable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/tests/test_astro.py` & `lime-stable-1.0.5/tests/test_astro.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/tests/test_cube.py` & `lime-stable-1.0.5/tests/test_cube.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/tests/test_io.py` & `lime-stable-1.0.5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/tests/test_line.py` & `lime-stable-1.0.5/tests/test_line.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/tests/test_model.py` & `lime-stable-1.0.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/tests/test_read_fits.py` & `lime-stable-1.0.5/tests/test_read_fits.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/tests/test_sample.py` & `lime-stable-1.0.5/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/tests/test_spectrum.py` & `lime-stable-1.0.5/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.4/tests/test_tools.py` & `lime-stable-1.0.5/tests/test_tools.py`

 * *Files identical despite different names*

