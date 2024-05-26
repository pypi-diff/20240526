# Comparing `tmp/mkdocs_torillic-2.3.0.tar.gz` & `tmp/mkdocs_torillic-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_torillic-2.3.0.tar", last modified: Sun May 26 17:52:39 2024, max compression
+gzip compressed data, was "mkdocs_torillic-2.3.1.tar", last modified: Sun May 26 21:21:35 2024, max compression
```

## Comparing `mkdocs_torillic-2.3.0.tar` & `mkdocs_torillic-2.3.1.tar`

### file list

```diff
@@ -1,12 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:52:39.217221 mkdocs_torillic-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-26 17:52:27.000000 mkdocs_torillic-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-26 17:52:39.217221 mkdocs_torillic-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-26 17:52:27.000000 mkdocs_torillic-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:52:39.217221 mkdocs_torillic-2.3.0/mkdocs_torillic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-26 17:52:39.000000 mkdocs_torillic-2.3.0/mkdocs_torillic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-26 17:52:39.000000 mkdocs_torillic-2.3.0/mkdocs_torillic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 17:52:39.000000 mkdocs_torillic-2.3.0/mkdocs_torillic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-26 17:52:39.000000 mkdocs_torillic-2.3.0/mkdocs_torillic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 17:52:39.000000 mkdocs_torillic-2.3.0/mkdocs_torillic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-26 17:52:27.000000 mkdocs_torillic-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 17:52:39.217221 mkdocs_torillic-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:35.810456 mkdocs_torillic-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-26 21:21:22.000000 mkdocs_torillic-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-26 21:21:35.810456 mkdocs_torillic-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-26 21:21:22.000000 mkdocs_torillic-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:35.794456 mkdocs_torillic-2.3.1/mkdocs_torillic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:22.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:35.798456 mkdocs_torillic-2.3.1/mkdocs_torillic/css/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:35.798456 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:35.798456 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/attrib.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:35.806456 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/coins/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/coins/copper.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/coins/electrum.png
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/coins/gold.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/coins/platinum.png
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/coins/silver.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:35.794456 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:35.806456 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/Alegreya/
+-rw-r--r--   0 runner    (1001) docker     (127)   258792 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/Alegreya/Alegreya-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   257292 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/Alegreya/Alegreya-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   254808 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/Alegreya/Alegreya-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   256112 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/Alegreya/Alegreya-Regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:35.806456 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/CrimsonText/
+-rw-r--r--   0 runner    (1001) docker     (127)   112116 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/CrimsonText/CrimsonText-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   114268 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/CrimsonText/CrimsonText-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   109440 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/CrimsonText/CrimsonText-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   106512 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/CrimsonText/CrimsonText-Regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:35.810456 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/SourceCodePro/
+-rw-r--r--   0 runner    (1001) docker     (127)   120316 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/SourceCodePro/SourceCodePro-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   101956 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/SourceCodePro/SourceCodePro-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   102004 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/SourceCodePro/SourceCodePro-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   120456 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/fonts/SourceCodePro/SourceCodePro-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   291485 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/paper-texture.png
+-rw-r--r--   0 runner    (1001) docker     (127)   129962 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)  4661906 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/assets/torillic-bg.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-26 21:21:23.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic/torillic.css
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-26 21:21:22.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/css/torillic.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-26 21:21:22.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 21:21:22.000000 mkdocs_torillic-2.3.1/mkdocs_torillic/mkdocs_theme.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:35.810456 mkdocs_torillic-2.3.1/mkdocs_torillic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-26 21:21:35.000000 mkdocs_torillic-2.3.1/mkdocs_torillic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-26 21:21:35.000000 mkdocs_torillic-2.3.1/mkdocs_torillic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:21:35.000000 mkdocs_torillic-2.3.1/mkdocs_torillic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-26 21:21:35.000000 mkdocs_torillic-2.3.1/mkdocs_torillic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 21:21:35.000000 mkdocs_torillic-2.3.1/mkdocs_torillic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-26 21:21:22.000000 mkdocs_torillic-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 21:21:35.810456 mkdocs_torillic-2.3.1/setup.cfg
```

### Comparing `mkdocs_torillic-2.3.0/LICENSE` & `mkdocs_torillic-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_torillic-2.3.0/PKG-INFO` & `mkdocs_torillic-2.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mkdocs-torillic
-Version: 2.3.0
+Version: 2.3.1
 Summary: Implementation of the Torillic theme for mkdocs. Convert your markdown TTRPG notes into beautiful HTML!
 Author-email: Todd Parsons <todd.e.parsons@gmail.com>
-Project-URL: Homepage, https://TEParsons.github.io/torillic
-Project-URL: Download, https://github.com/TEParsons/torillic/torillic/
+Project-URL: Homepage, https://TEParsons.github.io/mkdocs-torillic
+Project-URL: Download, https://github.com/TEParsons/mkdocs-torillic/releases
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Torillic
 > Magic is distilled laziness
 
 This theme, named after the fantasy setting of [Dungeons & Dragons](https://www.dndbeyond.com/), is designed with tabletop RPG players in mind. The theme allows beautiful HTML exports designed to look like a professionally made tabletop resource, whilst remaining easy to edit in code view and in small windows, thanks to CSS media queries.
```

### Comparing `mkdocs_torillic-2.3.0/README.md` & `mkdocs_torillic-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_torillic-2.3.0/mkdocs_torillic.egg-info/PKG-INFO` & `mkdocs_torillic-2.3.1/mkdocs_torillic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mkdocs-torillic
-Version: 2.3.0
+Version: 2.3.1
 Summary: Implementation of the Torillic theme for mkdocs. Convert your markdown TTRPG notes into beautiful HTML!
 Author-email: Todd Parsons <todd.e.parsons@gmail.com>
-Project-URL: Homepage, https://TEParsons.github.io/torillic
-Project-URL: Download, https://github.com/TEParsons/torillic/torillic/
+Project-URL: Homepage, https://TEParsons.github.io/mkdocs-torillic
+Project-URL: Download, https://github.com/TEParsons/mkdocs-torillic/releases
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Torillic
 > Magic is distilled laziness
 
 This theme, named after the fantasy setting of [Dungeons & Dragons](https://www.dndbeyond.com/), is designed with tabletop RPG players in mind. The theme allows beautiful HTML exports designed to look like a professionally made tabletop resource, whilst remaining easy to edit in code view and in small windows, thanks to CSS media queries.
```

### Comparing `mkdocs_torillic-2.3.0/pyproject.toml` & `mkdocs_torillic-2.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "mkdocs-torillic"
-version = "2.3.0"
+version = "2.3.1"
 authors = [
     {name = "Todd Parsons", email = "todd.e.parsons@gmail.com"}
 ]
 description = "Implementation of the Torillic theme for mkdocs. Convert your markdown TTRPG notes into beautiful HTML!"
 readme = "README.md"
 
 [project.urls]
-Homepage = "https://TEParsons.github.io/torillic"
-Download = "https://github.com/TEParsons/torillic/torillic/"
+Homepage = "https://TEParsons.github.io/mkdocs-torillic"
+Download = "https://github.com/TEParsons/mkdocs-torillic/releases"
 
 [tool.setuptools]
-py-modules = ["mkdocs_torillic"]
+packages = ["mkdocs_torillic"]
 
 [tool.setuptools.package-data]
 mkdocs_torillic = ["**/*.html", "**/*.css", "**/*.yml", "**/*.jpg", "**/*.png", "**/*.json", "**/*.ttf"]
 
 [project.entry-points."mkdocs.themes"]
 torillic = "mkdocs_torillic"
```

