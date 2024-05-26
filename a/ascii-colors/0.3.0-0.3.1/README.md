# Comparing `tmp/ascii_colors-0.3.0.tar.gz` & `tmp/ascii_colors-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii_colors-0.3.0.tar", last modified: Sat May 25 20:16:01 2024, max compression
+gzip compressed data, was "ascii_colors-0.3.1.tar", last modified: Sat May 25 20:35:36 2024, max compression
```

## Comparing `ascii_colors-0.3.0.tar` & `ascii_colors-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 20:16:01.588034 ascii_colors-0.3.0/
--rw-rw-rw-   0        0        0    11558 2023-10-29 12:12:16.000000 ascii_colors-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      922 2024-05-25 20:16:01.586033 ascii_colors-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3634 2023-10-29 12:12:16.000000 ascii_colors-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 20:16:01.567939 ascii_colors-0.3.0/ascii_colors/
--rw-rw-rw-   0        0        0    11242 2024-05-25 20:12:43.000000 ascii_colors-0.3.0/ascii_colors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 20:16:01.585035 ascii_colors-0.3.0/ascii_colors.egg-info/
--rw-rw-rw-   0        0        0      922 2024-05-25 20:16:01.000000 ascii_colors-0.3.0/ascii_colors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-05-25 20:16:01.000000 ascii_colors-0.3.0/ascii_colors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 20:16:01.000000 ascii_colors-0.3.0/ascii_colors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-25 20:16:01.000000 ascii_colors-0.3.0/ascii_colors.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 20:16:01.588034 ascii_colors-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1251 2024-05-25 20:12:43.000000 ascii_colors-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:35:36.992378 ascii_colors-0.3.1/
+-rw-rw-rw-   0        0        0    11558 2023-10-29 12:12:16.000000 ascii_colors-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      922 2024-05-25 20:35:36.991376 ascii_colors-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4113 2024-05-25 20:35:21.000000 ascii_colors-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 20:35:36.974377 ascii_colors-0.3.1/ascii_colors/
+-rw-rw-rw-   0        0        0    11242 2024-05-25 20:12:43.000000 ascii_colors-0.3.1/ascii_colors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:35:36.990375 ascii_colors-0.3.1/ascii_colors.egg-info/
+-rw-rw-rw-   0        0        0      922 2024-05-25 20:35:36.000000 ascii_colors-0.3.1/ascii_colors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-05-25 20:35:36.000000 ascii_colors-0.3.1/ascii_colors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 20:35:36.000000 ascii_colors-0.3.1/ascii_colors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-25 20:35:36.000000 ascii_colors-0.3.1/ascii_colors.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 20:35:36.993376 ascii_colors-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1251 2024-05-25 20:35:27.000000 ascii_colors-0.3.1/setup.py
```

### Comparing `ascii_colors-0.3.0/LICENSE` & `ascii_colors-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii_colors-0.3.0/PKG-INFO` & `ascii_colors-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii_colors
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python library for pretty console printing with colors and styles
 Home-page: https://github.com/ParisNeo/console_tools
 Author: Saifeddine ALOUI (ParisNeo)
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ascii_colors-0.3.0/README.md` & `ascii_colors-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Sure, here's a README.md documentation template for your ASCIIColors utility:
-
 # ASCIIColors
 
 ASCIIColors is a Python utility that provides an easy way to add color and style to text output in the console. It offers a simple interface for printing text with various colors and styles, making it especially useful for enhancing the readability of console-based applications or adding emphasis to specific messages.
 
 ## Table of Contents
 
 - [Installation](#installation)
@@ -87,16 +85,38 @@
 
 # Print a warning message
 ASCIIColors.warning("Warning: This action cannot be undone")
 
 # Print text in bold and underline style
 ASCIIColors.bold("Important message", ASCIIColors.color_bright_blue)
 ASCIIColors.underline("Underlined text", ASCIIColors.color_bright_green)
+
+# Use specific colors directly
+ASCIIColors.yellow("Yellow text")
+ASCIIColors.red("Red text")
+ASCIIColors.green("Green text")
+ASCIIColors.cyan("Cyan text")
+
+ASCIIColors.multicolor(["Green text","red text","yellow text"],[ASCIIColors.color_green, ASCIIColors.color_red, ASCIIColors.color_yellow])
+```
+
+Trace and color your exceptions using `trace_exception`: 
+
+```python
+# Trace all your exceptions using:
+from asciicolors import trace_exception
+
+try:
+    #some nasty stuff that can crush
+except Exception as ex:
+    trace_exception(ex)
+
 ```
 
+
 ## Contributing
 
 Contributions to ASCIIColors are welcome! If you have ideas for improvements or new features, please feel free to open an issue or submit a pull request. Make sure to follow the [contribution guidelines](CONTRIBUTING.md).
 
 ## License
 
 ASCIIColors is licensed under the [Apache License 2.0](LICENSE). You are free to use, modify, and distribute this utility as per the terms of the license.
```

### Comparing `ascii_colors-0.3.0/ascii_colors/__init__.py` & `ascii_colors-0.3.1/ascii_colors/__init__.py`

 * *Files identical despite different names*

### Comparing `ascii_colors-0.3.0/ascii_colors.egg-info/PKG-INFO` & `ascii_colors-0.3.1/ascii_colors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii_colors
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python library for pretty console printing with colors and styles
 Home-page: https://github.com/ParisNeo/console_tools
 Author: Saifeddine ALOUI (ParisNeo)
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ascii_colors-0.3.0/setup.py` & `ascii_colors-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ascii_colors',
-    version='0.3.0',
+    version='0.3.1',
     description='A Python library for pretty console printing with colors and styles',
     long_description='A Python library for displaying text on the console with colors, styles, and exception handling.',
     author='Saifeddine ALOUI (ParisNeo)',
     author_email='aloui.saifeddine@gmail.com',
     url='https://github.com/ParisNeo/console_tools',
     packages=find_packages(),
     classifiers=[
```

