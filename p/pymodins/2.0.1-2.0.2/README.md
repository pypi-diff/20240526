# Comparing `tmp/pymodins-2.0.1.tar.gz` & `tmp/pymodins-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-ba8qa7wy\pymodins-2.0.1.tar", last modified: Mon May 20 12:12:23 2024, max compression
+gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-x1jnk81n\pymodins-2.0.2.tar", last modified: Sun May 26 08:02:31 2024, max compression
```

## Comparing `pymodins-2.0.1.tar` & `pymodins-2.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 12:12:23.340501 pymodins-2.0.1/
--rw-rw-rw-   0        0        0     1085 2024-05-17 08:05:08.000000 pymodins-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     3863 2024-05-20 12:12:23.338506 pymodins-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3232 2024-05-20 10:01:59.000000 pymodins-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 12:12:23.327306 pymodins-2.0.1/pymodins/
--rw-rw-rw-   0        0        0      335 2024-05-20 12:11:48.000000 pymodins-2.0.1/pymodins/__init__.py
--rw-rw-rw-   0        0        0    55054 2024-05-20 12:11:45.000000 pymodins-2.0.1/pymodins/installer.py
-drwxrwxrwx   0        0        0        0 2024-05-20 12:12:23.337508 pymodins-2.0.1/pymodins.egg-info/
--rw-rw-rw-   0        0        0     3863 2024-05-20 12:12:23.000000 pymodins-2.0.1/pymodins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-05-20 12:12:23.000000 pymodins-2.0.1/pymodins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 12:12:23.000000 pymodins-2.0.1/pymodins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-20 12:12:23.000000 pymodins-2.0.1/pymodins.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-20 12:12:23.000000 pymodins-2.0.1/pymodins.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-20 12:12:23.000000 pymodins-2.0.1/pymodins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 12:12:23.340501 pymodins-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      934 2024-05-20 12:11:25.000000 pymodins-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 08:02:31.223269 pymodins-2.0.2/
+-rw-rw-rw-   0        0        0     1085 2024-05-17 08:05:08.000000 pymodins-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-05-26 08:02:31.220091 pymodins-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3232 2024-05-20 10:01:59.000000 pymodins-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 08:02:31.193446 pymodins-2.0.2/pymodins/
+-rw-rw-rw-   0        0        0      335 2024-05-26 08:02:18.000000 pymodins-2.0.2/pymodins/__init__.py
+-rw-rw-rw-   0        0        0    55881 2024-05-26 08:01:52.000000 pymodins-2.0.2/pymodins/installer.py
+drwxrwxrwx   0        0        0        0 2024-05-26 08:02:31.219091 pymodins-2.0.2/pymodins.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-05-26 08:02:31.000000 pymodins-2.0.2/pymodins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-26 08:02:31.000000 pymodins-2.0.2/pymodins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 08:02:31.000000 pymodins-2.0.2/pymodins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-26 08:02:31.000000 pymodins-2.0.2/pymodins.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-26 08:02:31.000000 pymodins-2.0.2/pymodins.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-26 08:02:31.000000 pymodins-2.0.2/pymodins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 08:02:31.223269 pymodins-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      934 2024-05-26 08:02:23.000000 pymodins-2.0.2/setup.py
```

### Comparing `pymodins-2.0.1/LICENSE` & `pymodins-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodins-2.0.1/PKG-INFO` & `pymodins-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 2.0.1
+Version: 2.0.2
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com 
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymodins-2.0.1/README.md` & `pymodins-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pymodins-2.0.1/pymodins/installer.py` & `pymodins-2.0.2/pymodins/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import getpass
 import sys
+import re
 import urllib.request
 from datetime import datetime
 import subprocess
 import ctypes
 import webbrowser
 import pymsgbox
 from rich.console import Console
@@ -37,18 +38,35 @@
 |_____|    |______|  |_____||_____|`.___.'|______.'|_____||_____|\____| \______.' 
                                                                                 
     """
     console.print(ascii_art, style="bold yellow")
     console.print("Creator: Nandhan K", style="bold cyan")
     console.print("Github: @github.com/Nandhan-KA", style="bold yellow")
 
-
 def sys_info():
     print("System Platform:", sys.platform)
     print("Python verion:", sys.version)
+    try:
+        pip_version = subprocess.check_output(['pip', '--version']).decode().strip()
+        print("pip version:", pip_version)
+    except Exception as e:
+        print("Error:", e,"Reinstall Python with PIP and add PIP to the System PATH")
+import subprocess
+import pip
+
+def upgrade_pip():
+    try:
+        installed_version = pip.__version__
+
+        latest_pip_version_output = subprocess.check_output(['pip', 'install', '--upgrade', 'pip']).decode().strip()
+        print("Latest pip version output:", latest_pip_version_output)
+
+        print("pip is already up to date" if installed_version == pip.__version__ else f"pip upgraded from version {installed_version} to version {pip.__version__}")
+    except Exception as e:
+        print("Error:", e)
 
 def clear():
     return os.system('cls')
 
 def log_mod(module_type, module_name, python_folder):
     timestamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     log_entry = f"{timestamp} - Installed {module_name} from {module_type} in {python_folder}"
@@ -186,18 +204,19 @@
 jupyter_modules = [
     'jupyter',
     'notebook', 'jupyterlab', 'nbconvert', 'nbformat', 'ipywidgets', 'ipykernel', 'voila', 'jupyter_contrib_nbextensions', 'jupyter_dash', 'jupyter_bokeh', 'jupytext', 'jupyterhub', 'jupyter_client', 'qtconsole'
 ]
 
 def installer():
     if internet():
+        upgrade_pip()
         clear()
         banner()
         sys_info()
-
+        
         module_types = [
             'Basic Modules', 'Advanced Modules', 'Science Modules', 'Computer Vision Modules',
             'Machine Learning Modules', 'Deep Learning Modules', 'Full Stack Development Modules',
             'Network Modules', 'Build Modules', 'Jupyter Modules'
         ]
 
         print("\nPlease select the type of modules you want to install:\n")
@@ -1335,8 +1354,9 @@
             os.system(command)
 
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
-                installer()
+                installer()
+run()
```

### Comparing `pymodins-2.0.1/pymodins.egg-info/PKG-INFO` & `pymodins-2.0.2/pymodins.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 2.0.1
+Version: 2.0.2
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com 
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymodins-2.0.1/setup.py` & `pymodins-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pymodins",
-    version="2.0.1",
+    version="2.0.2",
     packages=find_packages(),
     install_requires=[
         "rich",
         "pymsgbox"
     ],
     entry_points={
         "console_scripts": [
```

