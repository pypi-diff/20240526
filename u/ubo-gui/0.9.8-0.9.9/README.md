# Comparing `tmp/ubo_gui-0.9.8.tar.gz` & `tmp/ubo_gui-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubo_gui-0.9.8.tar", max compression
+gzip compressed data, was "ubo_gui-0.9.9.tar", max compression
```

## Comparing `ubo_gui-0.9.8.tar` & `ubo_gui-0.9.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11357 2024-03-14 01:19:29.226963 ubo_gui-0.9.8/LICENSE
--rw-r--r--   0        0        0     1785 2024-03-14 01:19:29.226963 ubo_gui-0.9.8/README.md
--rw-r--r--   0        0        0     1647 2024-03-14 01:19:29.226963 ubo_gui-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      907 2024-03-14 01:19:29.226963 ubo_gui-0.9.8/ubo_gui/__init__.py
--rw-r--r--   0        0        0     2231 2024-03-14 01:19:29.226963 ubo_gui-0.9.8/ubo_gui/animated_slider/__init__.py
--rw-r--r--   0        0        0     2786 2024-03-14 01:19:29.226963 ubo_gui-0.9.8/ubo_gui/app/__init__.py
--rw-r--r--   0        0        0      409 2024-03-14 01:19:29.226963 ubo_gui-0.9.8/ubo_gui/app/app.kv
--rw-r--r--   0        0        0  8322328 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/assets/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].ttf
--rw-r--r--   0        0        0      489 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/constants.py
--rw-r--r--   0        0        0      723 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/gauge/__init__.py
--rw-r--r--   0        0        0     1163 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/gauge/gauge_widget.kv
--rw-r--r--   0        0        0     1706 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/logger.py
--rw-r--r--   0        0        0    22245 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/menu/__init__.py
--rw-r--r--   0        0        0      305 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/menu/constants.py
--rw-r--r--   0        0        0      504 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/menu/menu.kv
--rw-r--r--   0        0        0     4912 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/menu/transitions.py
--rw-r--r--   0        0        0     5999 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/menu/types.py
--rw-r--r--   0        0        0       41 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/menu/widgets/__init__.py
--rw-r--r--   0        0        0      872 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/menu/widgets/header_menu_page_widget.kv
--rw-r--r--   0        0        0     2012 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/menu/widgets/header_menu_page_widget.py
--rw-r--r--   0        0        0     1066 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/menu/widgets/item_widget.kv
--rw-r--r--   0        0        0     3973 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/menu/widgets/item_widget.py
--rw-r--r--   0        0        0      454 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/menu/widgets/normal_menu_page_widget.kv
--rw-r--r--   0        0        0      362 2024-03-14 01:19:29.274963 ubo_gui-0.9.8/ubo_gui/menu/widgets/normal_menu_page_widget.py
--rw-r--r--   0        0        0     2293 2024-03-14 01:19:29.278962 ubo_gui-0.9.8/ubo_gui/notification/__init__.py
--rw-r--r--   0        0        0     2173 2024-03-14 01:19:29.278962 ubo_gui-0.9.8/ubo_gui/notification/notification_widget.kv
--rw-r--r--   0        0        0     2558 2024-03-14 01:19:29.278962 ubo_gui-0.9.8/ubo_gui/page/__init__.py
--rw-r--r--   0        0        0     4341 2024-03-14 01:19:29.278962 ubo_gui-0.9.8/ubo_gui/prompt/__init__.py
--rw-r--r--   0        0        0      858 2024-03-14 01:19:29.278962 ubo_gui-0.9.8/ubo_gui/prompt/prompt_widget.kv
--rw-r--r--   0        0        0      699 2024-03-14 01:19:29.278962 ubo_gui-0.9.8/ubo_gui/qrcode/__init__.py
--rw-r--r--   0        0        0      616 2024-03-14 01:19:29.278962 ubo_gui-0.9.8/ubo_gui/volume/__init__.py
--rw-r--r--   0        0        0      860 2024-03-14 01:19:29.278962 ubo_gui-0.9.8/ubo_gui/volume/volume_widget.kv
--rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 ubo_gui-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-14 23:03:35.041165 ubo_gui-0.9.9/LICENSE
+-rw-r--r--   0        0        0     1785 2024-03-14 23:03:35.041165 ubo_gui-0.9.9/README.md
+-rw-r--r--   0        0        0     1647 2024-03-14 23:03:35.041165 ubo_gui-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      907 2024-03-14 23:03:35.041165 ubo_gui-0.9.9/ubo_gui/__init__.py
+-rw-r--r--   0        0        0     2231 2024-03-14 23:03:35.041165 ubo_gui-0.9.9/ubo_gui/animated_slider/__init__.py
+-rw-r--r--   0        0        0     2786 2024-03-14 23:03:35.041165 ubo_gui-0.9.9/ubo_gui/app/__init__.py
+-rw-r--r--   0        0        0      409 2024-03-14 23:03:35.041165 ubo_gui-0.9.9/ubo_gui/app/app.kv
+-rw-r--r--   0        0        0  8322328 2024-03-14 23:03:35.089166 ubo_gui-0.9.9/ubo_gui/assets/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].ttf
+-rw-r--r--   0        0        0      489 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/constants.py
+-rw-r--r--   0        0        0      723 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/gauge/__init__.py
+-rw-r--r--   0        0        0     1163 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/gauge/gauge_widget.kv
+-rw-r--r--   0        0        0     1706 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/logger.py
+-rw-r--r--   0        0        0    22245 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/menu/__init__.py
+-rw-r--r--   0        0        0      305 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/menu/constants.py
+-rw-r--r--   0        0        0      504 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/menu/menu.kv
+-rw-r--r--   0        0        0     4912 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/menu/transitions.py
+-rw-r--r--   0        0        0     5999 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/menu/types.py
+-rw-r--r--   0        0        0       41 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/menu/widgets/__init__.py
+-rw-r--r--   0        0        0      872 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/menu/widgets/header_menu_page_widget.kv
+-rw-r--r--   0        0        0     2012 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/menu/widgets/header_menu_page_widget.py
+-rw-r--r--   0        0        0     1066 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/menu/widgets/item_widget.kv
+-rw-r--r--   0        0        0     3973 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/menu/widgets/item_widget.py
+-rw-r--r--   0        0        0      454 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/menu/widgets/normal_menu_page_widget.kv
+-rw-r--r--   0        0        0      362 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/menu/widgets/normal_menu_page_widget.py
+-rw-r--r--   0        0        0     2293 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/notification/__init__.py
+-rw-r--r--   0        0        0     2173 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/notification/notification_widget.kv
+-rw-r--r--   0        0        0     2558 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/page/__init__.py
+-rw-r--r--   0        0        0     4341 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/prompt/__init__.py
+-rw-r--r--   0        0        0      858 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/prompt/prompt_widget.kv
+-rw-r--r--   0        0        0      699 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/qrcode/__init__.py
+-rw-r--r--   0        0        0      616 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/volume/__init__.py
+-rw-r--r--   0        0        0      860 2024-03-14 23:03:35.093165 ubo_gui-0.9.9/ubo_gui/volume/volume_widget.kv
+-rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 ubo_gui-0.9.9/PKG-INFO
```

### Comparing `ubo_gui-0.9.8/LICENSE` & `ubo_gui-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/README.md` & `ubo_gui-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/pyproject.toml` & `ubo_gui-0.9.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ubo-gui"
-version = "0.9.8"
+version = "0.9.9"
 description = "GUI sdk for Ubo Pod"
 authors = ["Sassan Haradji <sassanh@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "ubo_gui" }]
 include = ['ubo_gui/assets/fonts/*']
 
 [tool.poetry.dependencies]
 python = "^3.11"
 headless-kivy-pi = [
-  { version = "^0.7.0", markers = "extra=='default'", extras = [
+  { version = "^0.7.1", markers = "extra=='default'", extras = [
     'default',
   ] },
-  { version = "^0.7.0", markers = "extra=='dev'", extras = [
+  { version = "^0.7.1", markers = "extra=='dev'", extras = [
     'dev',
   ] },
 ]
 python-immutable = "^1.0.2"
 qrcode = "^7.4.2"
 
 [tool.poetry.group.dev]
```

### Comparing `ubo_gui-0.9.8/ubo_gui/__init__.py` & `ubo_gui-0.9.9/ubo_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/animated_slider/__init__.py` & `ubo_gui-0.9.9/ubo_gui/animated_slider/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/app/__init__.py` & `ubo_gui-0.9.9/ubo_gui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/assets/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].ttf` & `ubo_gui-0.9.9/ubo_gui/assets/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].ttf`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/gauge/__init__.py` & `ubo_gui-0.9.9/ubo_gui/gauge/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/gauge/gauge_widget.kv` & `ubo_gui-0.9.9/ubo_gui/gauge/gauge_widget.kv`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/logger.py` & `ubo_gui-0.9.9/ubo_gui/logger.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/menu/__init__.py` & `ubo_gui-0.9.9/ubo_gui/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/menu/transitions.py` & `ubo_gui-0.9.9/ubo_gui/menu/transitions.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/menu/types.py` & `ubo_gui-0.9.9/ubo_gui/menu/types.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/menu/widgets/header_menu_page_widget.kv` & `ubo_gui-0.9.9/ubo_gui/menu/widgets/header_menu_page_widget.kv`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/menu/widgets/header_menu_page_widget.py` & `ubo_gui-0.9.9/ubo_gui/menu/widgets/header_menu_page_widget.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/menu/widgets/item_widget.kv` & `ubo_gui-0.9.9/ubo_gui/menu/widgets/item_widget.kv`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/menu/widgets/item_widget.py` & `ubo_gui-0.9.9/ubo_gui/menu/widgets/item_widget.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/notification/__init__.py` & `ubo_gui-0.9.9/ubo_gui/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/notification/notification_widget.kv` & `ubo_gui-0.9.9/ubo_gui/notification/notification_widget.kv`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/page/__init__.py` & `ubo_gui-0.9.9/ubo_gui/page/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/prompt/__init__.py` & `ubo_gui-0.9.9/ubo_gui/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/prompt/prompt_widget.kv` & `ubo_gui-0.9.9/ubo_gui/prompt/prompt_widget.kv`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/qrcode/__init__.py` & `ubo_gui-0.9.9/ubo_gui/qrcode/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/volume/__init__.py` & `ubo_gui-0.9.9/ubo_gui/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/ubo_gui/volume/volume_widget.kv` & `ubo_gui-0.9.9/ubo_gui/volume/volume_widget.kv`

 * *Files identical despite different names*

### Comparing `ubo_gui-0.9.8/PKG-INFO` & `ubo_gui-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ubo-gui
-Version: 0.9.8
+Version: 0.9.9
 Summary: GUI sdk for Ubo Pod
 License: Apache-2.0
 Author: Sassan Haradji
 Author-email: sassanh@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: default
 Provides-Extra: dev
-Requires-Dist: headless-kivy-pi[default] (>=0.7.0,<0.8.0) ; extra == "default"
-Requires-Dist: headless-kivy-pi[dev] (>=0.7.0,<0.8.0) ; extra == "dev"
+Requires-Dist: headless-kivy-pi[default] (>=0.7.1,<0.8.0) ; extra == "default"
+Requires-Dist: headless-kivy-pi[dev] (>=0.7.1,<0.8.0) ; extra == "dev"
 Requires-Dist: python-immutable (>=1.0.2,<2.0.0)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Description-Content-Type: text/markdown
 
 # Ubo GUI
 
 GUI sdk for [Ubo Pod](https://github.com/ubopod)
```

