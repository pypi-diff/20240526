# Comparing `tmp/pip2deb-1.3.tar.gz` & `tmp/pip2deb-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip2deb-1.3.tar", last modified: Sun May 26 20:13:52 2024, max compression
+gzip compressed data, was "pip2deb-1.4.tar", last modified: Sun May 26 21:11:29 2024, max compression
```

## Comparing `pip2deb-1.3.tar` & `pip2deb-1.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 20:13:51.996651 pip2deb-1.3/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-1.3/LICENSE
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-26 20:13:51.996651 pip2deb-1.3/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-1.3/README.rst
--rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2518 2024-05-26 19:58:08.000000 pip2deb-1.3/pip2deb
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 20:13:51.996651 pip2deb-1.3/pip2deb.egg-info/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-26 20:13:51.000000 pip2deb-1.3/pip2deb.egg-info/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      159 2024-05-26 20:13:51.000000 pip2deb-1.3/pip2deb.egg-info/SOURCES.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 20:13:51.000000 pip2deb-1.3/pip2deb.egg-info/dependency_links.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 20:13:51.000000 pip2deb-1.3/pip2deb.egg-info/top_level.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-26 20:13:51.996651 pip2deb-1.3/setup.cfg
--rw-r--r--   0 whoami    (1002) whoami    (1002)      788 2024-05-26 20:13:43.000000 pip2deb-1.3/setup.py
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 21:11:29.972333 pip2deb-1.4/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-1.4/LICENSE
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-26 21:11:29.972333 pip2deb-1.4/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-1.4/README.rst
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2761 2024-05-26 21:10:14.000000 pip2deb-1.4/pip2deb
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2590 2024-05-26 21:06:10.000000 pip2deb-1.4/pip2deb-sub
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 21:11:29.972333 pip2deb-1.4/pip2deb.egg-info/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-26 21:11:29.000000 pip2deb-1.4/pip2deb.egg-info/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      171 2024-05-26 21:11:29.000000 pip2deb-1.4/pip2deb.egg-info/SOURCES.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 21:11:29.000000 pip2deb-1.4/pip2deb.egg-info/dependency_links.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 21:11:29.000000 pip2deb-1.4/pip2deb.egg-info/top_level.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-26 21:11:29.972333 pip2deb-1.4/setup.cfg
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      803 2024-05-26 21:11:18.000000 pip2deb-1.4/setup.py
```

### Comparing `pip2deb-1.3/LICENSE` & `pip2deb-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pip2deb-1.3/PKG-INFO` & `pip2deb-1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 1.3
+Version: 1.4
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-1.3/README.rst` & `pip2deb-1.4/README.rst`

 * *Files identical despite different names*

### Comparing `pip2deb-1.3/pip2deb` & `pip2deb-1.4/pip2deb-sub`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 # Grep Meta Data from Modul
 msg "[*] Grep Meta Data from Modul"
 package=$(pip show ${name} | grep -E '^Name: ' | cut -d' ' -f2)
 version=$(pip show ${name} | grep -E '^Version: ' | cut -d' ' -f2)
 summary=$(pip show ${name} | grep -E '^Summary: ' | cut -d' ' -f2)
 author=$(pip show ${name} | grep -E '^Author: ' | cut -d' ' -f2)
 email=$(pip show ${name} | grep -E '^Author-email: ' | cut -d' ' -f2)
+pip_depends=$(pip show ${name} | grep -E '^Requires: ' | cut -d' ' -f2)
 arch=$(dpkg --print-architecture)
 
 #Struct Package
 msg "[*] Struct Package"
 build_dir="${name}${pythonpath}"
 build_prefix="${name}${prefix}"
 debian_dir="${name}/DEBIAN"
```

### Comparing `pip2deb-1.3/pip2deb.egg-info/PKG-INFO` & `pip2deb-1.4/pip2deb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 1.3
+Version: 1.4
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-1.3/setup.py` & `pip2deb-1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 def readme():
     with open('README.rst', 'r') as f:
         content = f.read()
     return content
 
 setup(
     name="pip2deb",
-    version="1.3",
+    version="1.4",
     decription="A Simple Tool to Pack Python Project into a Debian Package, For Debian/Ubuntu and Termux",
     long_description=readme(),
     url='https://github.com/pacspedd/pip2deb',
     author="PacSpedd",
     author_email="pacspedd@outlook.com",
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.8'
     ],
     packages=find_packages(),
-    scripts=['pip2deb']
+    scripts=['pip2deb', 'pip2deb-sub']
 )
```

