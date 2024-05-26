# Comparing `tmp/pip2deb-1.4.tar.gz` & `tmp/pip2deb-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip2deb-1.4.tar", last modified: Sun May 26 21:11:29 2024, max compression
+gzip compressed data, was "pip2deb-1.5.tar", last modified: Sun May 26 21:15:58 2024, max compression
```

## Comparing `pip2deb-1.4.tar` & `pip2deb-1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 21:11:29.972333 pip2deb-1.4/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-1.4/LICENSE
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-26 21:11:29.972333 pip2deb-1.4/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-1.4/README.rst
--rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2761 2024-05-26 21:10:14.000000 pip2deb-1.4/pip2deb
--rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2590 2024-05-26 21:06:10.000000 pip2deb-1.4/pip2deb-sub
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 21:11:29.972333 pip2deb-1.4/pip2deb.egg-info/
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-26 21:11:29.000000 pip2deb-1.4/pip2deb.egg-info/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      171 2024-05-26 21:11:29.000000 pip2deb-1.4/pip2deb.egg-info/SOURCES.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 21:11:29.000000 pip2deb-1.4/pip2deb.egg-info/dependency_links.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 21:11:29.000000 pip2deb-1.4/pip2deb.egg-info/top_level.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-26 21:11:29.972333 pip2deb-1.4/setup.cfg
--rw-r--r--   0 whoami    (1002) whoami    (1002)      803 2024-05-26 21:11:18.000000 pip2deb-1.4/setup.py
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 21:15:58.732110 pip2deb-1.5/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-1.5/LICENSE
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-26 21:15:58.732110 pip2deb-1.5/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-1.5/README.rst
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2759 2024-05-26 21:15:27.000000 pip2deb-1.5/pip2deb
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2759 2024-05-26 21:15:49.000000 pip2deb-1.5/pip2deb-sub
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 21:15:58.732110 pip2deb-1.5/pip2deb.egg-info/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-26 21:15:58.000000 pip2deb-1.5/pip2deb.egg-info/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      171 2024-05-26 21:15:58.000000 pip2deb-1.5/pip2deb.egg-info/SOURCES.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 21:15:58.000000 pip2deb-1.5/pip2deb.egg-info/dependency_links.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 21:15:58.000000 pip2deb-1.5/pip2deb.egg-info/top_level.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-26 21:15:58.732110 pip2deb-1.5/setup.cfg
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      803 2024-05-26 21:15:20.000000 pip2deb-1.5/setup.py
```

### Comparing `pip2deb-1.4/LICENSE` & `pip2deb-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pip2deb-1.4/PKG-INFO` & `pip2deb-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 1.4
+Version: 1.5
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-1.4/README.rst` & `pip2deb-1.5/README.rst`

 * *Files identical despite different names*

### Comparing `pip2deb-1.4/pip2deb` & `pip2deb-1.5/pip2deb`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 else
     msg "[*] Bin Folder Not Foun"
 fi
 
 # Install Requires Seperate
 msg "[*] Install Requirements Seperate"
 for dep in ${pip_depends}; do
-    ./pip2deb-sub ${dep} ${distro}
+    pip2deb-sub ${dep} ${distro}
     rm -rf ${build_dir}/${dep}*
 done
 
 # Create Control File and Give him Correct Rights
 msg "[*] Create Control File and Give Rights"
 cat <<EOF > ${control_file}
 Package: ${name}
```

### Comparing `pip2deb-1.4/pip2deb-sub` & `pip2deb-1.5/pip2deb-sub`

 * *Files 8% similar despite different names*

```diff
@@ -67,14 +67,21 @@
     mkdir -p ${build_prefix}/bin
     cp -rf ${build_dir}/bin/* ${build_prefix}/bin
     rm -rf ${build_dir}/bin
 else
     msg "[*] Bin Folder Not Foun"
 fi
 
+# Install Requires Seperate
+msg "[*] Install Requirements Seperate"
+for dep in ${pip_depends}; do
+    pip2deb-sub ${dep} ${distro}
+    rm -rf ${build_dir}/${dep}*
+done
+
 # Create Control File and Give him Correct Rights
 msg "[*] Create Control File and Give Rights"
 cat <<EOF > ${control_file}
 Package: ${name}
 Version: ${version}
 Architecture: ${arch}
 Maintainer: ${author} <${email}>
```

### Comparing `pip2deb-1.4/pip2deb.egg-info/PKG-INFO` & `pip2deb-1.5/pip2deb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 1.4
+Version: 1.5
 Home-page: https://github.com/pacspedd/pip2deb
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pip2deb-1.4/setup.py` & `pip2deb-1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def readme():
     with open('README.rst', 'r') as f:
         content = f.read()
     return content
 
 setup(
     name="pip2deb",
-    version="1.4",
+    version="1.5",
     decription="A Simple Tool to Pack Python Project into a Debian Package, For Debian/Ubuntu and Termux",
     long_description=readme(),
     url='https://github.com/pacspedd/pip2deb',
     author="PacSpedd",
     author_email="pacspedd@outlook.com",
     license='MIT',
     classifiers=[
```

