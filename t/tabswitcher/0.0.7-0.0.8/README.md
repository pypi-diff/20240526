# Comparing `tmp/tabswitcher-0.0.7.tar.gz` & `tmp/tabswitcher-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabswitcher-0.0.7.tar", last modified: Sat May 25 21:11:25 2024, max compression
+gzip compressed data, was "tabswitcher-0.0.8.tar", last modified: Sat May 25 21:40:28 2024, max compression
```

## Comparing `tabswitcher-0.0.7.tar` & `tabswitcher-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:11:25.378234 tabswitcher-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-25 21:11:25.378234 tabswitcher-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 21:11:25.378234 tabswitcher-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:11:25.370233 tabswitcher-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:11:25.374234 tabswitcher-0.0.7/src/tabswitcher/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/NetworkImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/SearchInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/TabList.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:11:25.378234 tabswitcher-0.0.7/src/tabswitcher/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/assets/Icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/assets/brotab_service.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/assets/install.bat
--rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/assets/sans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/assets/searchIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/assets/tabswitcher_service.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/brotab.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/fuzzySearch.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/loadBookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-25 21:11:13.000000 tabswitcher-0.0.7/src/tabswitcher/logTabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:11:25.378234 tabswitcher-0.0.7/tabswitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-25 21:11:25.000000 tabswitcher-0.0.7/tabswitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-25 21:11:25.000000 tabswitcher-0.0.7/tabswitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 21:11:25.000000 tabswitcher-0.0.7/tabswitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-25 21:11:25.000000 tabswitcher-0.0.7/tabswitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 21:11:25.000000 tabswitcher-0.0.7/tabswitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 21:11:25.000000 tabswitcher-0.0.7/tabswitcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:40:28.908347 tabswitcher-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-25 21:40:28.908347 tabswitcher-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 21:40:28.908347 tabswitcher-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:40:28.904347 tabswitcher-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:40:28.904347 tabswitcher-0.0.8/src/tabswitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/NetworkImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/SearchInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/TabList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:40:28.908347 tabswitcher-0.0.8/src/tabswitcher/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/assets/Icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/assets/brotab_service.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/assets/install.bat
+-rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/assets/sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/assets/searchIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/assets/tabswitcher_service.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/brotab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/fuzzySearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/loadBookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/logTabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:40:28.908347 tabswitcher-0.0.8/tabswitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-25 21:40:28.000000 tabswitcher-0.0.8/tabswitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-25 21:40:28.000000 tabswitcher-0.0.8/tabswitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 21:40:28.000000 tabswitcher-0.0.8/tabswitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-25 21:40:28.000000 tabswitcher-0.0.8/tabswitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 21:40:28.000000 tabswitcher-0.0.8/tabswitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 21:40:28.000000 tabswitcher-0.0.8/tabswitcher.egg-info/top_level.txt
```

### Comparing `tabswitcher-0.0.7/LICENCE` & `tabswitcher-0.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/PKG-INFO` & `tabswitcher-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tabswitcher-0.0.7/README.md` & `tabswitcher-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/setup.py` & `tabswitcher-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tabswitcher',
-    version='0.0.7',
+    version='0.0.8',
     packages=['tabswitcher'],
     package_dir={'tabswitcher': 'src/tabswitcher'},
     package_data={'tabswitcher': ['assets/*']},
     description="A tool for efficient browser tab switching outside the browser",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='YukiGasai',
```

### Comparing `tabswitcher-0.0.7/src/tabswitcher/NetworkImage.py` & `tabswitcher-0.0.8/src/tabswitcher/NetworkImage.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/src/tabswitcher/SearchInput.py` & `tabswitcher-0.0.8/src/tabswitcher/SearchInput.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/src/tabswitcher/Settings.py` & `tabswitcher-0.0.8/src/tabswitcher/Settings.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/src/tabswitcher/Tab.py` & `tabswitcher-0.0.8/src/tabswitcher/Tab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/src/tabswitcher/TabList.py` & `tabswitcher-0.0.8/src/tabswitcher/TabList.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/src/tabswitcher/__main__.py` & `tabswitcher-0.0.8/src/tabswitcher/__main__.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/src/tabswitcher/assets/Icon.ico` & `tabswitcher-0.0.8/src/tabswitcher/assets/Icon.ico`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/src/tabswitcher/assets/brotab_service.xml` & `tabswitcher-0.0.8/src/tabswitcher/assets/brotab_service.xml`

 * *Files 6% similar despite different names*

```diff
@@ -24,20 +24,13 @@
     <Enabled>true</Enabled>
     <Hidden>true</Hidden>
     <RunOnlyIfIdle>false</RunOnlyIfIdle>
     <WakeToRun>false</WakeToRun>
     <ExecutionTimeLimit>PT0S</ExecutionTimeLimit>
     <Priority>7</Priority>
   </Settings>
-  <Principals>
-    <Principal id="Author">
-      <UserId>S-1-5-18</UserId>
-      <LogonType>S4U</LogonType>
-      <RunLevel>HighestAvailable</RunLevel>
-    </Principal>
-  </Principals>
   <Actions Context="Author">
     <Exec>
       <Command>bt_mediator</Command>
     </Exec>
   </Actions>
 </Task>
```

### Comparing `tabswitcher-0.0.7/src/tabswitcher/assets/install.bat` & `tabswitcher-0.0.8/src/tabswitcher/assets/install.bat`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/src/tabswitcher/assets/sans.ttf` & `tabswitcher-0.0.8/src/tabswitcher/assets/sans.ttf`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/src/tabswitcher/assets/tabswitcher_service.xml` & `tabswitcher-0.0.8/src/tabswitcher/assets/tabswitcher_service.xml`

 * *Files 3% similar despite different names*

```diff
@@ -24,21 +24,14 @@
     <Enabled>true</Enabled>
     <Hidden>true</Hidden>
     <RunOnlyIfIdle>false</RunOnlyIfIdle>
     <WakeToRun>false</WakeToRun>
     <ExecutionTimeLimit>PT0S</ExecutionTimeLimit>
     <Priority>7</Priority>
   </Settings>
-  <Principals>
-    <Principal id="Author">
-      <UserId>S-1-5-18</UserId>
-      <LogonType>S4U</LogonType> <!-- Add this line -->
-      <RunLevel>HighestAvailable</RunLevel>
-    </Principal>
-  </Principals>
   <Actions Context="Author">
     <Exec>
       <Command>tabswitcher</Command>
       <Arguments>--startlogger</Arguments>
     </Exec>
   </Actions>
 </Task>
```

### Comparing `tabswitcher-0.0.7/src/tabswitcher/brotab.py` & `tabswitcher-0.0.8/src/tabswitcher/brotab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/src/tabswitcher/colors.py` & `tabswitcher-0.0.8/src/tabswitcher/colors.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/src/tabswitcher/fuzzySearch.py` & `tabswitcher-0.0.8/src/tabswitcher/fuzzySearch.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/src/tabswitcher/logTabs.py` & `tabswitcher-0.0.8/src/tabswitcher/logTabs.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.7/tabswitcher.egg-info/PKG-INFO` & `tabswitcher-0.0.8/tabswitcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tabswitcher-0.0.7/tabswitcher.egg-info/SOURCES.txt` & `tabswitcher-0.0.8/tabswitcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

