# Comparing `tmp/pyerualjetwork-1.2.4.tar.gz` & `tmp/pyerualjetwork-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.2.4.tar", last modified: Sun May 26 16:13:30 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.2.5.tar", last modified: Sun May 26 16:18:14 2024, max compression
```

## Comparing `pyerualjetwork-1.2.4.tar` & `pyerualjetwork-1.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 16:13:30.359182 pyerualjetwork-1.2.4/
--rw-rw-rw-   0        0        0      511 2024-05-26 16:13:30.358185 pyerualjetwork-1.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-26 16:13:30.343646 pyerualjetwork-1.2.4/plan/
--rw-rw-rw-   0        0        0      368 2024-05-26 15:58:07.000000 pyerualjetwork-1.2.4/plan/__init__.py
--rw-rw-rw-   0        0        0    40168 2024-05-26 16:12:52.000000 pyerualjetwork-1.2.4/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:13:30.356189 pyerualjetwork-1.2.4/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      511 2024-05-26 16:13:30.000000 pyerualjetwork-1.2.4/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-26 16:13:30.000000 pyerualjetwork-1.2.4/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 16:13:30.000000 pyerualjetwork-1.2.4/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-26 16:13:30.000000 pyerualjetwork-1.2.4/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 16:13:30.359182 pyerualjetwork-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      687 2024-05-26 16:13:21.000000 pyerualjetwork-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:18:14.426377 pyerualjetwork-1.2.5/
+-rw-rw-rw-   0        0        0      511 2024-05-26 16:18:14.425329 pyerualjetwork-1.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 16:18:14.408401 pyerualjetwork-1.2.5/plan/
+-rw-rw-rw-   0        0        0      368 2024-05-26 15:58:07.000000 pyerualjetwork-1.2.5/plan/__init__.py
+-rw-rw-rw-   0        0        0    40176 2024-05-26 16:17:40.000000 pyerualjetwork-1.2.5/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:18:14.422623 pyerualjetwork-1.2.5/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      511 2024-05-26 16:18:14.000000 pyerualjetwork-1.2.5/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-26 16:18:14.000000 pyerualjetwork-1.2.5/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 16:18:14.000000 pyerualjetwork-1.2.5/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-26 16:18:14.000000 pyerualjetwork-1.2.5/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 16:18:14.427394 pyerualjetwork-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      687 2024-05-26 16:17:50.000000 pyerualjetwork-1.2.5/setup.py
```

### Comparing `pyerualjetwork-1.2.4/plan/plan.py` & `pyerualjetwork-1.2.5/plan/plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1045,9 +1045,9 @@
     
 def GetAcc():
         
     return 2
 
 def GetAllFromLoad():
     
-    return 0,1,2,3,4,5
+     return [0, 1, 2, 3, 4, 5]
```

### Comparing `pyerualjetwork-1.2.4/setup.py` & `pyerualjetwork-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "1.2.4",
+      version = "1.2.5",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
       description= "Advanced python deep learning library.UPDATED TO 1.2.2 NEW FEATURES: GetWeights() func for TrainPLAN, TestPLAN and LoadPLAN, GetPreds() and GetAcc() funcs for TrainPLAN and TestPLAN, GetAllFromLoad() func for LoadPLAN, GetDf() for LoadPLAN (Documentation in desc. Examples in GİTHUB: HCB06)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks']
       
       )
```

