# Comparing `tmp/prototools-0.1.8.tar.gz` & `tmp/prototools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Projects\Python\prototools_implementando\dist\tmpp_e0tpu6\prototools-0.1.8.tar", last modified: Thu Oct 21 15:12:37 2021, max compression
+gzip compressed data, was "D:\Projects\Python\prototools_implementando\dist\tmplbi7invr\prototools-0.1.9.tar", last modified: Thu Oct 21 16:48:00 2021, max compression
```

## Comparing `prototools-0.1.8.tar` & `prototools-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2021-10-21 15:12:37.000000 prototools-0.1.8/
--rw-rw-rw-   0        0        0     1092 2021-09-19 22:58:10.000000 prototools-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     2242 2021-10-21 15:12:37.000000 prototools-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1341 2021-08-12 22:27:37.000000 prototools-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2021-10-21 15:12:37.000000 prototools-0.1.8/prototools/
--rw-rw-rw-   0        0        0        0 2021-07-28 17:42:06.000000 prototools-0.1.8/prototools/__init__.py
--rw-rw-rw-   0        0        0     3753 2021-08-12 23:37:25.000000 prototools-0.1.8/prototools/algo.py
--rw-rw-rw-   0        0        0     2195 2021-08-05 18:04:55.000000 prototools-0.1.8/prototools/color.py
--rw-rw-rw-   0        0        0    28839 2021-08-03 04:44:42.000000 prototools-0.1.8/prototools/componentes.py
--rw-rw-rw-   0        0        0     1891 2021-09-09 23:40:22.000000 prototools-0.1.8/prototools/components.py
--rw-rw-rw-   0        0        0     4289 2021-09-09 22:23:53.000000 prototools-0.1.8/prototools/config.py
--rw-rw-rw-   0        0        0     1625 2021-07-29 04:22:20.000000 prototools-0.1.8/prototools/constantes.py
--rw-rw-rw-   0        0        0    20114 2021-10-21 15:07:50.000000 prototools-0.1.8/prototools/entradas.py
--rw-rw-rw-   0        0        0     5296 2021-08-12 23:03:56.000000 prototools-0.1.8/prototools/experimental.py
--rw-rw-rw-   0        0        0    12733 2021-09-06 05:37:45.000000 prototools-0.1.8/prototools/menu.py
--rw-rw-rw-   0        0        0    18016 2021-09-09 22:27:29.000000 prototools-0.1.8/prototools/utils.py
--rw-rw-rw-   0        0        0    20007 2021-08-12 22:06:21.000000 prototools-0.1.8/prototools/validaciones.py
-drwxrwxrwx   0        0        0        0 2021-10-21 15:12:37.000000 prototools-0.1.8/prototools.egg-info/
--rw-rw-rw-   0        0        0     2242 2021-10-21 15:12:37.000000 prototools-0.1.8/prototools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2021-10-21 15:12:37.000000 prototools-0.1.8/prototools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-21 15:12:37.000000 prototools-0.1.8/prototools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2021-10-21 15:12:37.000000 prototools-0.1.8/prototools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-07-23 01:22:18.000000 prototools-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2021-10-21 15:12:37.000000 prototools-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1175 2021-10-21 15:12:16.000000 prototools-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-10-21 15:12:37.000000 prototools-0.1.8/test/
--rw-rw-rw-   0        0        0     2326 2021-08-05 20:10:45.000000 prototools-0.1.8/test/test_menu.py
--rw-rw-rw-   0        0        0     1812 2021-08-01 05:17:42.000000 prototools-0.1.8/test/test_pantalla.py
--rw-rw-rw-   0        0        0     2491 2021-08-09 18:14:09.000000 prototools-0.1.8/test/test_validaciones.py
+drwxrwxrwx   0        0        0        0 2021-10-21 16:48:00.000000 prototools-0.1.9/
+-rw-rw-rw-   0        0        0     1092 2021-09-19 22:58:10.000000 prototools-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     2242 2021-10-21 16:48:00.000000 prototools-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1341 2021-08-12 22:27:37.000000 prototools-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2021-10-21 16:48:00.000000 prototools-0.1.9/prototools/
+-rw-rw-rw-   0        0        0        0 2021-07-28 17:42:06.000000 prototools-0.1.9/prototools/__init__.py
+-rw-rw-rw-   0        0        0     3753 2021-08-12 23:37:25.000000 prototools-0.1.9/prototools/algo.py
+-rw-rw-rw-   0        0        0     2195 2021-08-05 18:04:55.000000 prototools-0.1.9/prototools/color.py
+-rw-rw-rw-   0        0        0    28839 2021-08-03 04:44:42.000000 prototools-0.1.9/prototools/componentes.py
+-rw-rw-rw-   0        0        0     1891 2021-09-09 23:40:22.000000 prototools-0.1.9/prototools/components.py
+-rw-rw-rw-   0        0        0     4289 2021-09-09 22:23:53.000000 prototools-0.1.9/prototools/config.py
+-rw-rw-rw-   0        0        0     1625 2021-07-29 04:22:20.000000 prototools-0.1.9/prototools/constantes.py
+-rw-rw-rw-   0        0        0    20140 2021-10-21 16:46:56.000000 prototools-0.1.9/prototools/entradas.py
+-rw-rw-rw-   0        0        0     5296 2021-08-12 23:03:56.000000 prototools-0.1.9/prototools/experimental.py
+-rw-rw-rw-   0        0        0    12733 2021-09-06 05:37:45.000000 prototools-0.1.9/prototools/menu.py
+-rw-rw-rw-   0        0        0    18016 2021-09-09 22:27:29.000000 prototools-0.1.9/prototools/utils.py
+-rw-rw-rw-   0        0        0    20007 2021-08-12 22:06:21.000000 prototools-0.1.9/prototools/validaciones.py
+drwxrwxrwx   0        0        0        0 2021-10-21 16:48:00.000000 prototools-0.1.9/prototools.egg-info/
+-rw-rw-rw-   0        0        0     2242 2021-10-21 16:48:00.000000 prototools-0.1.9/prototools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2021-10-21 16:48:00.000000 prototools-0.1.9/prototools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-10-21 16:48:00.000000 prototools-0.1.9/prototools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2021-10-21 16:48:00.000000 prototools-0.1.9/prototools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-07-23 01:22:18.000000 prototools-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2021-10-21 16:48:00.000000 prototools-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2021-10-21 16:47:28.000000 prototools-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-10-21 16:48:00.000000 prototools-0.1.9/test/
+-rw-rw-rw-   0        0        0     2326 2021-08-05 20:10:45.000000 prototools-0.1.9/test/test_menu.py
+-rw-rw-rw-   0        0        0     1812 2021-08-01 05:17:42.000000 prototools-0.1.9/test/test_pantalla.py
+-rw-rw-rw-   0        0        0     2491 2021-08-09 18:14:09.000000 prototools-0.1.9/test/test_validaciones.py
```

### Comparing `prototools-0.1.8/LICENSE` & `prototools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/PKG-INFO` & `prototools-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prototools
-Version: 0.1.8
+Version: 0.1.9
 Summary: console toolbox
 Home-page: https://proto-tools.github.io/prototools-docs/
 Author: Miguel Kanashiro
 Author-email: leugimkm@systrien.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/leugimkm/prototools-docs/issues
 Platform: UNKNOWN
```

### Comparing `prototools-0.1.8/README.md` & `prototools-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/prototools/algo.py` & `prototools-0.1.9/prototools/algo.py`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/prototools/color.py` & `prototools-0.1.9/prototools/color.py`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/prototools/componentes.py` & `prototools-0.1.9/prototools/componentes.py`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/prototools/components.py` & `prototools-0.1.9/prototools/components.py`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/prototools/config.py` & `prototools-0.1.9/prototools/config.py`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/prototools/constantes.py` & `prototools-0.1.9/prototools/constantes.py`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/prototools/entradas.py` & `prototools-0.1.9/prototools/entradas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from prototools.componentes import Elemento
 import time
+import datetime
 from builtins import input
 from typing import Any, Callable, Optional, Sequence, Union
 
 import prototools.validaciones as v
 
 
 class _EntradaExcepcion(Exception):
@@ -653,12 +654,12 @@
         str: La hora en formato HH:MM
     """
     while True:
         try:
             entrada = input(indicacion)
             hora, minutos = [int(n) for n in entrada.split(":")]
             if (hora >= h_min and hora <= h_max) and (minutos >= m_min and minutos <= m_max):
-                return time(hour=hora, minute=minutos)
+                return datetime.time(hour=hora, minute=minutos)
             else:
                 print(defecto)
         except ValueError:
             print(error)
```

### Comparing `prototools-0.1.8/prototools/experimental.py` & `prototools-0.1.9/prototools/experimental.py`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/prototools/menu.py` & `prototools-0.1.9/prototools/menu.py`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/prototools/utils.py` & `prototools-0.1.9/prototools/utils.py`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/prototools/validaciones.py` & `prototools-0.1.9/prototools/validaciones.py`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/prototools.egg-info/PKG-INFO` & `prototools-0.1.9/prototools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prototools
-Version: 0.1.8
+Version: 0.1.9
 Summary: console toolbox
 Home-page: https://proto-tools.github.io/prototools-docs/
 Author: Miguel Kanashiro
 Author-email: leugimkm@systrien.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/leugimkm/prototools-docs/issues
 Platform: UNKNOWN
```

### Comparing `prototools-0.1.8/prototools.egg-info/SOURCES.txt` & `prototools-0.1.9/prototools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/setup.py` & `prototools-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="prototools",
-    version="0.1.8",
+    version="0.1.9",
     url="https://proto-tools.github.io/prototools-docs/",
     project_urls={
         "Bug Tracker": "https://github.com/leugimkm/prototools-docs/issues",
     },
     license="MIT",
     author="Miguel Kanashiro",
     author_email="leugimkm@systrien.com",
```

### Comparing `prototools-0.1.8/test/test_menu.py` & `prototools-0.1.9/test/test_menu.py`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/test/test_pantalla.py` & `prototools-0.1.9/test/test_pantalla.py`

 * *Files identical despite different names*

### Comparing `prototools-0.1.8/test/test_validaciones.py` & `prototools-0.1.9/test/test_validaciones.py`

 * *Files identical despite different names*

