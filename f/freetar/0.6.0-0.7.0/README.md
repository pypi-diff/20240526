# Comparing `tmp/freetar-0.6.0.tar.gz` & `tmp/freetar-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freetar-0.6.0.tar", max compression
+gzip compressed data, was "freetar-0.7.0.tar", max compression
```

## Comparing `freetar-0.6.0.tar` & `freetar-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-04-01 10:41:21.264981 freetar-0.6.0/LICENSE
--rw-r--r--   0        0        0     1599 2024-02-25 18:23:02.601532 freetar-0.6.0/README.md
--rw-r--r--   0        0        0     1763 2024-03-05 12:56:50.683556 freetar-0.6.0/freetar/backend.py
--rw-r--r--   0        0        0     4033 2024-03-05 12:56:55.046899 freetar-0.6.0/freetar/static/custom.js
--rw-r--r--   0        0        0    26135 2023-08-05 19:56:02.105488 freetar-0.6.0/freetar/static/guitar.png
--rw-r--r--   0        0        0     2168 2024-03-05 12:56:55.046899 freetar-0.6.0/freetar/static/scroll.js
--rw-r--r--   0        0        0     2853 2024-03-05 12:56:55.046899 freetar-0.6.0/freetar/templates/base.html
--rw-r--r--   0        0        0     5501 2024-01-24 07:50:25.115439 freetar-0.6.0/freetar/templates/index.html
--rw-r--r--   0        0        0     4761 2024-03-05 12:56:55.046899 freetar-0.6.0/freetar/templates/tab.html
--rw-r--r--   0        0        0     7216 2024-02-25 18:23:02.601532 freetar-0.6.0/freetar/ug.py
--rw-r--r--   0        0        0      580 2024-03-05 12:57:43.800342 freetar-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 freetar-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-01 10:41:21.264981 freetar-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1599 2024-02-25 18:23:02.601532 freetar-0.7.0/README.md
+-rw-r--r--   0        0        0     1763 2024-03-05 12:56:50.683556 freetar-0.7.0/freetar/backend.py
+-rw-r--r--   0        0        0     4033 2024-03-05 12:56:55.046899 freetar-0.7.0/freetar/static/custom.js
+-rw-r--r--   0        0        0    26135 2023-08-05 19:56:02.105488 freetar-0.7.0/freetar/static/guitar.png
+-rw-r--r--   0        0        0     2168 2024-03-05 12:56:55.046899 freetar-0.7.0/freetar/static/scroll.js
+-rw-r--r--   0        0        0     2853 2024-03-05 12:56:55.046899 freetar-0.7.0/freetar/templates/base.html
+-rw-r--r--   0        0        0     5501 2024-01-24 07:50:25.115439 freetar-0.7.0/freetar/templates/index.html
+-rw-r--r--   0        0        0     4761 2024-03-05 12:56:55.046899 freetar-0.7.0/freetar/templates/tab.html
+-rw-r--r--   0        0        0     7257 2024-05-26 15:14:48.322188 freetar-0.7.0/freetar/ug.py
+-rw-r--r--   0        0        0      580 2024-05-26 15:14:59.587495 freetar-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 freetar-0.7.0/PKG-INFO
```

### Comparing `freetar-0.6.0/LICENSE` & `freetar-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freetar-0.6.0/README.md` & `freetar-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `freetar-0.6.0/freetar/backend.py` & `freetar-0.7.0/freetar/backend.py`

 * *Files identical despite different names*

### Comparing `freetar-0.6.0/freetar/static/custom.js` & `freetar-0.7.0/freetar/static/custom.js`

 * *Files identical despite different names*

### Comparing `freetar-0.6.0/freetar/static/guitar.png` & `freetar-0.7.0/freetar/static/guitar.png`

 * *Files identical despite different names*

### Comparing `freetar-0.6.0/freetar/static/scroll.js` & `freetar-0.7.0/freetar/static/scroll.js`

 * *Files identical despite different names*

### Comparing `freetar-0.6.0/freetar/templates/base.html` & `freetar-0.7.0/freetar/templates/base.html`

 * *Files identical despite different names*

### Comparing `freetar-0.6.0/freetar/templates/index.html` & `freetar-0.7.0/freetar/templates/index.html`

 * *Files identical despite different names*

### Comparing `freetar-0.6.0/freetar/templates/tab.html` & `freetar-0.7.0/freetar/templates/tab.html`

 * *Files identical despite different names*

### Comparing `freetar-0.6.0/freetar/ug.py` & `freetar-0.7.0/freetar/ug.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 
     def __repr__(self):
         return f"{self.artist_name} - {self.song_name}"
 
     def fix_tab(self):
         tab = self.tab
         tab = tab.replace("\r\n", "<br/>")
+        tab = tab.replace("\n", "<br/>")
         tab = tab.replace(" ", "&nbsp;")
         tab = tab.replace("[tab]", "")
         tab = tab.replace("[/tab]", "")
 
         # (?P<root>[A-Ga-g](#|b)?) : Chord root is any letter A - G with an optional sharp or flat at the end
         # (?P<quality>[^[/]+)?  : Chord quality is anything after the root, but before the `/` for the base note
         # (?P<bass>/[A-Ga-g](#|b)?)? :  Chord quality is anything after the root, including parens in the case of 'm(maj7)'
```

### Comparing `freetar-0.6.0/pyproject.toml` & `freetar-0.7.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "freetar"
-version = "0.6.0"
+version = "0.7.0"
 description = ""
 authors = ["kmille <github@androidloves.me>"]
 readme = "README.md"
 repository = "https://github.com/kmille/freetar"
 homepage = "https://github.com/kmille/freetar"
```

### Comparing `freetar-0.6.0/PKG-INFO` & `freetar-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freetar
-Version: 0.6.0
+Version: 0.7.0
 Summary: 
 Home-page: https://github.com/kmille/freetar
 Author: kmille
 Author-email: github@androidloves.me
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

