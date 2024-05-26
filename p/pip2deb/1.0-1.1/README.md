# Comparing `tmp/pip2deb-1.0.tar.gz` & `tmp/pip2deb-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip2deb-1.0.tar", last modified: Sun May 26 11:26:28 2024, max compression
+gzip compressed data, was "pip2deb-1.1.tar", last modified: Sun May 26 16:16:15 2024, max compression
```

## Comparing `pip2deb-1.0.tar` & `pip2deb-1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 11:26:28.423688 pip2deb-1.0/
--rw-r--r--   0 whoami    (1002) whoami    (1002)      911 2024-05-26 11:26:28.423688 pip2deb-1.0/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      146 2024-05-26 11:26:10.000000 pip2deb-1.0/README.rst
--rwxr-xr-x   0 whoami    (1002) whoami    (1002)     1270 2024-05-26 11:17:14.000000 pip2deb-1.0/pip2deb
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 11:26:28.423688 pip2deb-1.0/pip2deb.egg-info/
--rw-r--r--   0 whoami    (1002) whoami    (1002)      911 2024-05-26 11:26:28.000000 pip2deb-1.0/pip2deb.egg-info/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      151 2024-05-26 11:26:28.000000 pip2deb-1.0/pip2deb.egg-info/SOURCES.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 11:26:28.000000 pip2deb-1.0/pip2deb.egg-info/dependency_links.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 11:26:28.000000 pip2deb-1.0/pip2deb.egg-info/top_level.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-26 11:26:28.423688 pip2deb-1.0/setup.cfg
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1009 2024-05-26 11:24:57.000000 pip2deb-1.0/setup.py
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 16:16:15.232004 pip2deb-1.1/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      911 2024-05-26 16:16:15.232004 pip2deb-1.1/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      146 2024-05-26 11:26:10.000000 pip2deb-1.1/README.rst
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     1423 2024-05-26 16:15:27.000000 pip2deb-1.1/pip2deb
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 16:16:15.232004 pip2deb-1.1/pip2deb.egg-info/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      911 2024-05-26 16:16:15.000000 pip2deb-1.1/pip2deb.egg-info/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      151 2024-05-26 16:16:15.000000 pip2deb-1.1/pip2deb.egg-info/SOURCES.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 16:16:15.000000 pip2deb-1.1/pip2deb.egg-info/dependency_links.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 16:16:15.000000 pip2deb-1.1/pip2deb.egg-info/top_level.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-26 16:16:15.232004 pip2deb-1.1/setup.cfg
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1009 2024-05-26 16:15:57.000000 pip2deb-1.1/setup.py
```

### Comparing `pip2deb-1.0/PKG-INFO` & `pip2deb-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 1.0
+Version: 1.1
 Summary: Package PIP Module as .deb, and this in under 1.5 minutes
 Home-page: https://github.com/pacspedd
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pip2deb-1.0/pip2deb` & `pip2deb-1.1/pip2deb`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 #!/bin/bash
 
 modul="$1"
 
-prefix='/usr/lib/python3.12/dist-packages'
+typ="$2"
 
-debian="${modul}/DEBIAN"
-control="${debian}/control"
+case "${typ}" in
+	debian)
+		prefix="/usr"
+		depends="python3 python3-venv python3-pip"
+		site="/lib/python3/dist-packages" ;;
+	termux)
+		prefix='/data/data/com.termux/files/usr'
+		depends='python python-pip'
+		site='/lib/python3.11/site-packages' ;;
+	*)
+		echo "[*] Invalid Distribution" ;;
+esac
 
-if [ "$#" -eq 2 ]; then
-        prefix="$2"
-fi
-
-target="${prefix}"
+target="${prefix}${site}"
 
 build_target="${modul}${target}"
 
 python3 -m venv .venv
 
 source .venv/bin/activate
 
@@ -35,26 +41,26 @@
 
 cat <<EOF > "${control}"
 Package: ${name}
 Version: ${version}
 Section: utils
 Architecture: $(dpkg --print-architecture)
 Priority: important
-Depends: python3, python3-venv, python3-pip
+Depends: ${depends}
 Maintainer: ${maintainer} <${email}>
 Description: ${description}
 EOF
 
 chmod 755 "${debian}"
 
 dpkg-deb -b "${modul}"
 
 deactivate
 
 rm -rf .venv
 
-mv "${modul}.deb" "python3-${modul}_v.${version}_$(dpkg --print-architecture).deb"
+mv "${modul}.deb" "pacspedd-python3-${modul}_v.${version}_$(dpkg --print-architecture).deb"
 
 rm -rf "${modul}"
 
 echo "[*] Build pip modul: ${modul} as Package, successful"
```

### Comparing `pip2deb-1.0/pip2deb.egg-info/PKG-INFO` & `pip2deb-1.1/pip2deb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip2deb
-Version: 1.0
+Version: 1.1
 Summary: Package PIP Module as .deb, and this in under 1.5 minutes
 Home-page: https://github.com/pacspedd
 Author: PacSpedd
 Author-email: pacspedd@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pip2deb-1.0/setup.py` & `pip2deb-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def readme():
     with open('README.rst', 'r') as f:
         content = f.read()
     return content
 
 setup(
     name='pip2deb',
-    version='1.0',
+    version='1.1',
     license='MIT',
     description='Package PIP Module as .deb, and this in under 1.5 minutes',
     long_description=readme(),
     long_description_content_type='text/x-rst',
     author='PacSpedd',
     author_email='pacspedd@outlook.com',
     url='https://github.com/pacspedd',
```

