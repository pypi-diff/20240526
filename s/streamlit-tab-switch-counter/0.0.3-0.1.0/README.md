# Comparing `tmp/streamlit_tab_switch_counter-0.0.3.tar.gz` & `tmp/streamlit_tab_switch_counter-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_tab_switch_counter-0.0.3.tar", last modified: Sun May 26 10:16:09 2024, max compression
+gzip compressed data, was "streamlit_tab_switch_counter-0.1.0.tar", last modified: Sun May 26 10:20:24 2024, max compression
```

## Comparing `streamlit_tab_switch_counter-0.0.3.tar` & `streamlit_tab_switch_counter-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 10:16:09.273058 streamlit_tab_switch_counter-0.0.3/
--rw-rw-rw-   0        0        0     1082 2024-05-26 01:17:46.000000 streamlit_tab_switch_counter-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       55 2024-05-26 01:51:46.000000 streamlit_tab_switch_counter-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      974 2024-05-26 10:16:09.269027 streamlit_tab_switch_counter-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-05-26 01:17:46.000000 streamlit_tab_switch_counter-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 10:16:09.273058 streamlit_tab_switch_counter-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1085 2024-05-26 10:16:06.000000 streamlit_tab_switch_counter-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:16:09.266377 streamlit_tab_switch_counter-0.0.3/streamlit_tab_switch_counter.egg-info/
--rw-rw-rw-   0        0        0      974 2024-05-26 10:16:09.000000 streamlit_tab_switch_counter-0.0.3/streamlit_tab_switch_counter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      708 2024-05-26 10:16:09.000000 streamlit_tab_switch_counter-0.0.3/streamlit_tab_switch_counter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 10:16:09.000000 streamlit_tab_switch_counter-0.0.3/streamlit_tab_switch_counter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-05-26 10:16:09.000000 streamlit_tab_switch_counter-0.0.3/streamlit_tab_switch_counter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-26 10:16:09.000000 streamlit_tab_switch_counter-0.0.3/streamlit_tab_switch_counter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-26 10:16:09.212849 streamlit_tab_switch_counter-0.0.3/tab_switch_counter/
--rw-rw-rw-   0        0        0     1905 2024-05-26 10:11:05.000000 streamlit_tab_switch_counter-0.0.3/tab_switch_counter/__init__.py
--rw-rw-rw-   0        0        0     1207 2024-05-26 01:17:46.000000 streamlit_tab_switch_counter-0.0.3/tab_switch_counter/example.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:16:09.180608 streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/
-drwxrwxrwx   0        0        0        0 2024-05-26 10:16:09.219904 streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-05-26 10:10:03.000000 streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-05-26 01:17:46.000000 streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2024-05-26 10:10:03.000000 streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-05-26 10:16:09.181956 streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-05-26 10:16:09.257717 streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/build/static/js/
--rw-rw-rw-   0        0        0   317777 2024-05-26 10:10:03.000000 streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/build/static/js/main.80f17556.js
--rw-rw-rw-   0        0        0     1293 2024-05-26 10:10:03.000000 streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/build/static/js/main.80f17556.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1247302 2024-05-26 10:10:03.000000 streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/build/static/js/main.80f17556.js.map
+drwxrwxrwx   0        0        0        0 2024-05-26 10:20:24.152608 streamlit_tab_switch_counter-0.1.0/
+-rw-rw-rw-   0        0        0     1082 2024-05-26 01:17:46.000000 streamlit_tab_switch_counter-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       55 2024-05-26 01:51:46.000000 streamlit_tab_switch_counter-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1030 2024-05-26 10:20:24.147817 streamlit_tab_switch_counter-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2024-05-26 10:20:19.000000 streamlit_tab_switch_counter-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 10:20:24.153148 streamlit_tab_switch_counter-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2024-05-26 10:16:51.000000 streamlit_tab_switch_counter-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:20:24.143565 streamlit_tab_switch_counter-0.1.0/streamlit_tab_switch_counter.egg-info/
+-rw-rw-rw-   0        0        0     1030 2024-05-26 10:20:23.000000 streamlit_tab_switch_counter-0.1.0/streamlit_tab_switch_counter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2024-05-26 10:20:23.000000 streamlit_tab_switch_counter-0.1.0/streamlit_tab_switch_counter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 10:20:23.000000 streamlit_tab_switch_counter-0.1.0/streamlit_tab_switch_counter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-05-26 10:20:23.000000 streamlit_tab_switch_counter-0.1.0/streamlit_tab_switch_counter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-26 10:20:23.000000 streamlit_tab_switch_counter-0.1.0/streamlit_tab_switch_counter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 10:20:24.108693 streamlit_tab_switch_counter-0.1.0/tab_switch_counter/
+-rw-rw-rw-   0        0        0     1905 2024-05-26 10:11:05.000000 streamlit_tab_switch_counter-0.1.0/tab_switch_counter/__init__.py
+-rw-rw-rw-   0        0        0     1207 2024-05-26 01:17:46.000000 streamlit_tab_switch_counter-0.1.0/tab_switch_counter/example.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:20:24.057028 streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/
+drwxrwxrwx   0        0        0        0 2024-05-26 10:20:24.118823 streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-05-26 10:10:03.000000 streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-05-26 01:17:46.000000 streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      492 2024-05-26 10:10:03.000000 streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-05-26 10:20:24.058394 streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-05-26 10:20:24.129058 streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   317777 2024-05-26 10:10:03.000000 streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/build/static/js/main.80f17556.js
+-rw-rw-rw-   0        0        0     1293 2024-05-26 10:10:03.000000 streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/build/static/js/main.80f17556.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1247302 2024-05-26 10:10:03.000000 streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/build/static/js/main.80f17556.js.map
```

### Comparing `streamlit_tab_switch_counter-0.0.3/LICENSE` & `streamlit_tab_switch_counter-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_tab_switch_counter-0.0.3/setup.py` & `streamlit_tab_switch_counter-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-tab-switch-counter",
-    version="0.0.3",
+    version="0.1.0",
     author="John Smith",
     author_email="john@example.com",
     description="Streamlit component that allows you to do X",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_tab_switch_counter-0.0.3/streamlit_tab_switch_counter.egg-info/SOURCES.txt` & `streamlit_tab_switch_counter-0.1.0/streamlit_tab_switch_counter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamlit_tab_switch_counter-0.0.3/tab_switch_counter/__init__.py` & `streamlit_tab_switch_counter-0.1.0/tab_switch_counter/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_tab_switch_counter-0.0.3/tab_switch_counter/example.py` & `streamlit_tab_switch_counter-0.1.0/tab_switch_counter/example.py`

 * *Files identical despite different names*

### Comparing `streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/build/bootstrap.min.css` & `streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/build/static/js/main.80f17556.js` & `streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/build/static/js/main.80f17556.js`

 * *Files identical despite different names*

### Comparing `streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/build/static/js/main.80f17556.js.LICENSE.txt` & `streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/build/static/js/main.80f17556.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_tab_switch_counter-0.0.3/tab_switch_counter/frontend/build/static/js/main.80f17556.js.map` & `streamlit_tab_switch_counter-0.1.0/tab_switch_counter/frontend/build/static/js/main.80f17556.js.map`

 * *Files identical despite different names*

