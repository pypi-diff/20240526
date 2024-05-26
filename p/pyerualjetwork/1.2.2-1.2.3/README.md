# Comparing `tmp/pyerualjetwork-1.2.2.tar.gz` & `tmp/pyerualjetwork-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.2.2.tar", last modified: Sun May 26 15:58:41 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.2.3.tar", last modified: Sun May 26 16:05:01 2024, max compression
```

## Comparing `pyerualjetwork-1.2.2.tar` & `pyerualjetwork-1.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 15:58:41.306411 pyerualjetwork-1.2.2/
--rw-rw-rw-   0        0        0      511 2024-05-26 15:58:41.305414 pyerualjetwork-1.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-26 15:58:41.291395 pyerualjetwork-1.2.2/plan/
--rw-rw-rw-   0        0        0      368 2024-05-26 15:58:07.000000 pyerualjetwork-1.2.2/plan/__init__.py
--rw-rw-rw-   0        0        0    40174 2024-05-26 15:20:16.000000 pyerualjetwork-1.2.2/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:58:41.302870 pyerualjetwork-1.2.2/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      511 2024-05-26 15:58:40.000000 pyerualjetwork-1.2.2/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-26 15:58:41.000000 pyerualjetwork-1.2.2/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 15:58:40.000000 pyerualjetwork-1.2.2/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-26 15:58:40.000000 pyerualjetwork-1.2.2/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 15:58:41.306411 pyerualjetwork-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      687 2024-05-26 15:58:30.000000 pyerualjetwork-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:05:01.759179 pyerualjetwork-1.2.3/
+-rw-rw-rw-   0        0        0      511 2024-05-26 16:05:01.758179 pyerualjetwork-1.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 16:05:01.741397 pyerualjetwork-1.2.3/plan/
+-rw-rw-rw-   0        0        0      368 2024-05-26 15:58:07.000000 pyerualjetwork-1.2.3/plan/__init__.py
+-rw-rw-rw-   0        0        0    40159 2024-05-26 16:03:41.000000 pyerualjetwork-1.2.3/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:05:01.755954 pyerualjetwork-1.2.3/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      511 2024-05-26 16:05:01.000000 pyerualjetwork-1.2.3/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-26 16:05:01.000000 pyerualjetwork-1.2.3/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 16:05:01.000000 pyerualjetwork-1.2.3/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-26 16:05:01.000000 pyerualjetwork-1.2.3/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 16:05:01.759179 pyerualjetwork-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      687 2024-05-26 16:04:51.000000 pyerualjetwork-1.2.3/setup.py
```

### Comparing `pyerualjetwork-1.2.2/plan/plan.py` & `pyerualjetwork-1.2.3/plan/plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1029,25 +1029,25 @@
         return 'e'
         
    return BalancedInputs, BalancedLabels
    
    
 def GetWeights():
         
-    return[0]
+    return 0
     
 def GetDf():
         
-    return[6]
+    return 6
     
 def GetPreds():
         
-    return[1]
+    return 1
     
 def GetAcc():
         
-    return[2]
+    return 2
 
 def GetAllFromLoad():
     
-    return[0],[1],[2],[3],[4],[5]
+    return 0,1,2,3,4,5
```

### Comparing `pyerualjetwork-1.2.2/setup.py` & `pyerualjetwork-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "1.2.2",
+      version = "1.2.3",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
       description= "Advanced python deep learning library.UPDATED TO 1.2.2 NEW FEATURES: GetWeights() func for TrainPLAN, TestPLAN and LoadPLAN, GetPreds() and GetAcc() funcs for TrainPLAN and TestPLAN, GetAllFromLoad() func for LoadPLAN, GetDf() for LoadPLAN (Documentation in desc. Examples in GİTHUB: HCB06)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks']
       
       )
```

