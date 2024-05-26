# Comparing `tmp/sym_metanet-1.1.0.tar.gz` & `tmp/sym_metanet-1.1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sym_metanet-1.1.0.tar", last modified: Tue Oct 17 18:37:18 2023, max compression
+gzip compressed data, was "sym_metanet-1.1.0.post1.tar", last modified: Sun May 26 16:54:20 2024, max compression
```

## Comparing `sym_metanet-1.1.0.tar` & `sym_metanet-1.1.0.post1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-10-17 18:37:18.796335 sym_metanet-1.1.0/
--rw-rw-rw-   0        0        0     1093 2022-10-27 09:27:26.000000 sym_metanet-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     6191 2023-10-17 18:37:18.792344 sym_metanet-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5291 2023-08-29 07:29:52.000000 sym_metanet-1.1.0/README.md
--rw-rw-rw-   0        0        0     1059 2023-10-17 18:36:00.000000 sym_metanet-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-17 18:37:18.796335 sym_metanet-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-10-17 18:37:18.675258 sym_metanet-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-10-17 18:37:18.708525 sym_metanet-1.1.0/src/sym_metanet/
--rw-rw-rw-   0        0        0     1186 2023-08-14 09:40:06.000000 sym_metanet-1.1.0/src/sym_metanet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-17 18:37:18.748045 sym_metanet-1.1.0/src/sym_metanet/blocks/
--rw-rw-rw-   0        0        0     4452 2023-10-17 18:17:55.000000 sym_metanet-1.1.0/src/sym_metanet/blocks/base.py
--rw-rw-rw-   0        0        0     4368 2023-10-17 18:17:56.000000 sym_metanet-1.1.0/src/sym_metanet/blocks/destinations.py
--rw-rw-rw-   0        0        0    13518 2023-10-17 18:17:56.000000 sym_metanet-1.1.0/src/sym_metanet/blocks/links.py
--rw-rw-rw-   0        0        0     5021 2023-10-17 18:17:56.000000 sym_metanet-1.1.0/src/sym_metanet/blocks/nodes.py
--rw-rw-rw-   0        0        0    15869 2023-10-17 18:17:56.000000 sym_metanet-1.1.0/src/sym_metanet/blocks/origins.py
-drwxrwxrwx   0        0        0        0 2023-10-17 18:37:18.762594 sym_metanet-1.1.0/src/sym_metanet/engines/
--rw-rw-rw-   0        0        0      153 2022-11-28 11:51:22.000000 sym_metanet-1.1.0/src/sym_metanet/engines/__init__.py
--rw-rw-rw-   0        0        0    17404 2023-10-17 18:17:56.000000 sym_metanet-1.1.0/src/sym_metanet/engines/casadi.py
--rw-rw-rw-   0        0        0    19904 2023-10-17 18:17:56.000000 sym_metanet-1.1.0/src/sym_metanet/engines/core.py
--rw-rw-rw-   0        0        0     9670 2023-10-17 18:17:55.000000 sym_metanet-1.1.0/src/sym_metanet/engines/numpy.py
--rw-rw-rw-   0        0        0      557 2022-11-28 11:51:22.000000 sym_metanet-1.1.0/src/sym_metanet/errors.py
--rw-rw-rw-   0        0        0    20718 2023-10-17 18:17:56.000000 sym_metanet-1.1.0/src/sym_metanet/network.py
-drwxrwxrwx   0        0        0        0 2023-10-17 18:37:18.770444 sym_metanet-1.1.0/src/sym_metanet/util/
--rw-rw-rw-   0        0        0     3642 2023-10-17 18:17:56.000000 sym_metanet-1.1.0/src/sym_metanet/util/funcs.py
--rw-rw-rw-   0        0        0      909 2022-12-30 15:45:07.000000 sym_metanet-1.1.0/src/sym_metanet/util/types.py
--rw-rw-rw-   0        0        0     2030 2023-10-17 18:17:56.000000 sym_metanet-1.1.0/src/sym_metanet/views.py
-drwxrwxrwx   0        0        0        0 2023-10-17 18:37:18.727579 sym_metanet-1.1.0/src/sym_metanet.egg-info/
--rw-rw-rw-   0        0        0     6191 2023-10-17 18:37:18.000000 sym_metanet-1.1.0/src/sym_metanet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      783 2023-10-17 18:37:18.000000 sym_metanet-1.1.0/src/sym_metanet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-17 18:37:18.000000 sym_metanet-1.1.0/src/sym_metanet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-10-17 18:37:18.000000 sym_metanet-1.1.0/src/sym_metanet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-10-17 18:37:18.000000 sym_metanet-1.1.0/src/sym_metanet.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-10-17 18:37:18.784683 sym_metanet-1.1.0/tests/
--rw-rw-rw-   0        0        0     5220 2023-01-11 13:34:26.000000 sym_metanet-1.1.0/tests/test_blocks.py
--rw-rw-rw-   0        0        0    15004 2023-10-17 18:17:55.000000 sym_metanet-1.1.0/tests/test_engines.py
--rw-rw-rw-   0        0        0    11725 2023-10-17 18:17:55.000000 sym_metanet-1.1.0/tests/test_examples.py
--rw-rw-rw-   0        0        0    11709 2023-10-17 18:17:53.000000 sym_metanet-1.1.0/tests/test_network.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:54:20.923343 sym_metanet-1.1.0.post1/
+-rw-rw-rw-   0        0        0     1093 2022-10-27 09:27:26.000000 sym_metanet-1.1.0.post1/LICENSE
+-rw-rw-rw-   0        0        0     6260 2024-05-26 16:54:20.921334 sym_metanet-1.1.0.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     5291 2024-05-26 16:45:55.000000 sym_metanet-1.1.0.post1/README.md
+-rw-rw-rw-   0        0        0     1586 2024-05-26 16:53:07.000000 sym_metanet-1.1.0.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 16:54:20.923343 sym_metanet-1.1.0.post1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 16:54:20.856678 sym_metanet-1.1.0.post1/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 16:54:20.875206 sym_metanet-1.1.0.post1/src/sym_metanet/
+-rw-rw-rw-   0        0        0     1217 2024-05-26 16:54:14.000000 sym_metanet-1.1.0.post1/src/sym_metanet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:54:20.897430 sym_metanet-1.1.0.post1/src/sym_metanet/blocks/
+-rw-rw-rw-   0        0        0     4452 2023-10-17 18:40:43.000000 sym_metanet-1.1.0.post1/src/sym_metanet/blocks/base.py
+-rw-rw-rw-   0        0        0     4368 2023-10-17 18:40:43.000000 sym_metanet-1.1.0.post1/src/sym_metanet/blocks/destinations.py
+-rw-rw-rw-   0        0        0    13518 2024-05-26 16:45:55.000000 sym_metanet-1.1.0.post1/src/sym_metanet/blocks/links.py
+-rw-rw-rw-   0        0        0     5020 2024-05-26 16:46:05.000000 sym_metanet-1.1.0.post1/src/sym_metanet/blocks/nodes.py
+-rw-rw-rw-   0        0        0    15869 2024-05-26 16:45:55.000000 sym_metanet-1.1.0.post1/src/sym_metanet/blocks/origins.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:54:20.906101 sym_metanet-1.1.0.post1/src/sym_metanet/engines/
+-rw-rw-rw-   0        0        0      153 2022-11-28 11:51:22.000000 sym_metanet-1.1.0.post1/src/sym_metanet/engines/__init__.py
+-rw-rw-rw-   0        0        0    17404 2024-05-26 16:45:55.000000 sym_metanet-1.1.0.post1/src/sym_metanet/engines/casadi.py
+-rw-rw-rw-   0        0        0    19904 2024-05-26 16:45:55.000000 sym_metanet-1.1.0.post1/src/sym_metanet/engines/core.py
+-rw-rw-rw-   0        0        0     9670 2024-05-26 16:45:55.000000 sym_metanet-1.1.0.post1/src/sym_metanet/engines/numpy.py
+-rw-rw-rw-   0        0        0      557 2022-11-28 11:51:22.000000 sym_metanet-1.1.0.post1/src/sym_metanet/errors.py
+-rw-rw-rw-   0        0        0    20718 2023-10-17 18:40:43.000000 sym_metanet-1.1.0.post1/src/sym_metanet/network.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:54:20.909109 sym_metanet-1.1.0.post1/src/sym_metanet/util/
+-rw-rw-rw-   0        0        0     3642 2023-10-17 18:40:43.000000 sym_metanet-1.1.0.post1/src/sym_metanet/util/funcs.py
+-rw-rw-rw-   0        0        0      909 2022-12-30 15:45:07.000000 sym_metanet-1.1.0.post1/src/sym_metanet/util/types.py
+-rw-rw-rw-   0        0        0     2030 2024-05-26 16:45:55.000000 sym_metanet-1.1.0.post1/src/sym_metanet/views.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:54:20.918764 sym_metanet-1.1.0.post1/src/sym_metanet.egg-info/
+-rw-rw-rw-   0        0        0     6260 2024-05-26 16:54:20.000000 sym_metanet-1.1.0.post1/src/sym_metanet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      783 2024-05-26 16:54:20.000000 sym_metanet-1.1.0.post1/src/sym_metanet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 16:54:20.000000 sym_metanet-1.1.0.post1/src/sym_metanet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-26 16:54:20.000000 sym_metanet-1.1.0.post1/src/sym_metanet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-26 16:54:20.000000 sym_metanet-1.1.0.post1/src/sym_metanet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 16:54:20.917631 sym_metanet-1.1.0.post1/tests/
+-rw-rw-rw-   0        0        0     5220 2023-01-11 13:34:26.000000 sym_metanet-1.1.0.post1/tests/test_blocks.py
+-rw-rw-rw-   0        0        0    15004 2023-10-17 18:40:43.000000 sym_metanet-1.1.0.post1/tests/test_engines.py
+-rw-rw-rw-   0        0        0    11725 2023-10-17 18:40:43.000000 sym_metanet-1.1.0.post1/tests/test_examples.py
+-rw-rw-rw-   0        0        0    11709 2023-10-17 18:40:43.000000 sym_metanet-1.1.0.post1/tests/test_network.py
```

### Comparing `sym_metanet-1.1.0/LICENSE` & `sym_metanet-1.1.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/PKG-INFO` & `sym_metanet-1.1.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sym_metanet
-Version: 1.1.0
+Version: 1.1.0.post1
 Summary: Symbolic Modelling of Highway Traffic Networks with METANET
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/sym-metanet
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/sym-metanet/issues
+Keywords: highway-traffic,highway-network,modelling-framework
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.9
```

### Comparing `sym_metanet-1.1.0/README.md` & `sym_metanet-1.1.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/src/sym_metanet/__init__.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__version__ = "1.1.0.post1"
+
 __all__ = [
     "engines",
     "CongestedDestination",
     "Destination",
     "EngineNotFoundWarning",
     "EngineNotFoundError",
     "InvalidNetworkError",
```

### Comparing `sym_metanet-1.1.0/src/sym_metanet/blocks/base.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/blocks/base.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/src/sym_metanet/blocks/destinations.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/blocks/destinations.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/src/sym_metanet/blocks/links.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/blocks/links.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/src/sym_metanet/blocks/nodes.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/blocks/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         # if no destination, then there must be 1 or more exiting links
         links_down: Collection[tuple["Node", "Node", "Link[Variable]"]] = net.out_links(
             self
         )
         if len(links_down) == 1:
             return first(links_down)[-1].states["rho"][0]
         rho_firsts = engine.vcat(
-            *(dlink.states["rho"][-1] for _, _, dlink in links_down)
+            *(dlink.states["rho"][0] for _, _, dlink in links_down)
         )
         return engine.nodes.get_downstream_density(rho_firsts)
 
     def get_upstream_speed_and_flow(
         self,
         net: "Network",
         link: "Link[VarType]",
```

### Comparing `sym_metanet-1.1.0/src/sym_metanet/blocks/origins.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/blocks/origins.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/src/sym_metanet/engines/casadi.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/engines/casadi.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/src/sym_metanet/engines/core.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/engines/core.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/src/sym_metanet/engines/numpy.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/engines/numpy.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/src/sym_metanet/errors.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/errors.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/src/sym_metanet/network.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/network.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/src/sym_metanet/util/funcs.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/util/funcs.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/src/sym_metanet/util/types.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/util/types.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/src/sym_metanet/views.py` & `sym_metanet-1.1.0.post1/src/sym_metanet/views.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/src/sym_metanet.egg-info/PKG-INFO` & `sym_metanet-1.1.0.post1/src/sym_metanet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: sym-metanet
-Version: 1.1.0
+Name: sym_metanet
+Version: 1.1.0.post1
 Summary: Symbolic Modelling of Highway Traffic Networks with METANET
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/sym-metanet
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/sym-metanet/issues
+Keywords: highway-traffic,highway-network,modelling-framework
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.9
```

### Comparing `sym_metanet-1.1.0/src/sym_metanet.egg-info/SOURCES.txt` & `sym_metanet-1.1.0.post1/src/sym_metanet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/tests/test_blocks.py` & `sym_metanet-1.1.0.post1/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/tests/test_engines.py` & `sym_metanet-1.1.0.post1/tests/test_engines.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/tests/test_examples.py` & `sym_metanet-1.1.0.post1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.1.0/tests/test_network.py` & `sym_metanet-1.1.0.post1/tests/test_network.py`

 * *Files identical despite different names*

