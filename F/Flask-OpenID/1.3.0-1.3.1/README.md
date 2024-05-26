# Comparing `tmp/Flask-OpenID-1.3.0.tar.gz` & `tmp/flask_openid-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-OpenID-1.3.0.tar", last modified: Wed Sep  8 21:28:18 2021, max compression
+gzip compressed data, was "flask_openid-1.3.1.tar", last modified: Sun May 26 15:47:46 2024, max compression
```

## Comparing `Flask-OpenID-1.3.0.tar` & `flask_openid-1.3.1.tar`

### file list

```diff
@@ -1,52 +1,36 @@
-drwxrwxr-x   0 jarek     (1000) jarek     (1000)        0 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/
-drwxrwxr-x   0 jarek     (1000) jarek     (1000)        0 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/Flask_OpenID.egg-info/
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     1461 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/Flask_OpenID.egg-info/PKG-INFO
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     1025 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/Flask_OpenID.egg-info/SOURCES.txt
--rw-rw-r--   0 jarek     (1000) jarek     (1000)        1 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/Flask_OpenID.egg-info/dependency_links.txt
--rw-rw-r--   0 jarek     (1000) jarek     (1000)        1 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/Flask_OpenID.egg-info/not-zip-safe
--rw-rw-r--   0 jarek     (1000) jarek     (1000)       34 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/Flask_OpenID.egg-info/requires.txt
--rw-rw-r--   0 jarek     (1000) jarek     (1000)       13 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/Flask_OpenID.egg-info/top_level.txt
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     1723 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/LICENSE
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      240 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/MANIFEST.in
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     1461 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/PKG-INFO
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      357 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/README.rst
-drwxrwxr-x   0 jarek     (1000) jarek     (1000)        0 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/docs/
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     4569 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/docs/Makefile
-drwxrwxr-x   0 jarek     (1000) jarek     (1000)        0 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/docs/_static/
--rw-rw-r--   0 jarek     (1000) jarek     (1000)    13828 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/docs/_static/flask-openid.png
-drwxrwxr-x   0 jarek     (1000) jarek     (1000)        0 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/docs/_themes/
--rw-rw-r--   0 jarek     (1000) jarek     (1000)       40 2021-09-08 21:27:51.000000 Flask-OpenID-1.3.0/docs/_themes/.git
--rw-rw-r--   0 jarek     (1000) jarek     (1000)       22 2021-09-08 21:27:51.000000 Flask-OpenID-1.3.0/docs/_themes/.gitignore
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     1789 2021-09-08 21:27:51.000000 Flask-OpenID-1.3.0/docs/_themes/LICENSE
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     1093 2021-09-08 21:27:51.000000 Flask-OpenID-1.3.0/docs/_themes/README
-drwxrwxr-x   0 jarek     (1000) jarek     (1000)        0 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/docs/_themes/flask/
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      582 2021-09-08 21:27:51.000000 Flask-OpenID-1.3.0/docs/_themes/flask/layout.html
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      590 2021-09-08 21:27:51.000000 Flask-OpenID-1.3.0/docs/_themes/flask/relations.html
-drwxrwxr-x   0 jarek     (1000) jarek     (1000)        0 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/docs/_themes/flask/static/
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     6233 2021-09-08 21:27:51.000000 Flask-OpenID-1.3.0/docs/_themes/flask/static/flasky.css_t
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      976 2021-09-08 21:27:51.000000 Flask-OpenID-1.3.0/docs/_themes/flask/static/small_flask.css
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      122 2021-09-08 21:27:51.000000 Flask-OpenID-1.3.0/docs/_themes/flask/theme.conf
-drwxrwxr-x   0 jarek     (1000) jarek     (1000)        0 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/docs/_themes/flask_small/
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      683 2021-09-08 21:27:51.000000 Flask-OpenID-1.3.0/docs/_themes/flask_small/layout.html
-drwxrwxr-x   0 jarek     (1000) jarek     (1000)        0 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/docs/_themes/flask_small/static/
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     4609 2021-09-08 21:27:51.000000 Flask-OpenID-1.3.0/docs/_themes/flask_small/static/flasky.css_t
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      184 2021-09-08 21:27:51.000000 Flask-OpenID-1.3.0/docs/_themes/flask_small/theme.conf
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     4875 2021-09-08 21:27:51.000000 Flask-OpenID-1.3.0/docs/_themes/flask_theme_support.py
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     7105 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/docs/conf.py
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     9985 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/docs/index.rst
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     4106 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/docs/make.bat
-drwxrwxr-x   0 jarek     (1000) jarek     (1000)        0 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/example/
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      140 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/example/README
--rwxrwxr-x   0 jarek     (1000) jarek     (1000)     5703 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/example/example.py
-drwxrwxr-x   0 jarek     (1000) jarek     (1000)        0 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/example/static/
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      433 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/example/static/openid.png
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      648 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/example/static/style.css
-drwxrwxr-x   0 jarek     (1000) jarek     (1000)        0 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/example/templates/
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      742 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/example/templates/create_profile.html
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      473 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/example/templates/edit_profile.html
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      213 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/example/templates/index.html
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      642 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/example/templates/layout.html
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      406 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/example/templates/login.html
--rw-rw-r--   0 jarek     (1000) jarek     (1000)    22474 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/flask_openid.py
--rw-rw-r--   0 jarek     (1000) jarek     (1000)      249 2021-09-08 21:28:18.000000 Flask-OpenID-1.3.0/setup.cfg
--rw-rw-r--   0 jarek     (1000) jarek     (1000)     2058 2021-09-08 21:27:31.000000 Flask-OpenID-1.3.0/setup.py
+drwxr-xr-x   0 jarek      (501) staff       (20)        0 2024-05-26 15:47:46.618013 flask_openid-1.3.1/
+drwxr-xr-x   0 jarek      (501) staff       (20)        0 2024-05-26 15:47:46.617690 flask_openid-1.3.1/Flask_OpenID.egg-info/
+-rw-r--r--   0 jarek      (501) staff       (20)     1633 2024-05-26 15:47:46.000000 flask_openid-1.3.1/Flask_OpenID.egg-info/PKG-INFO
+-rw-r--r--   0 jarek      (501) staff       (20)      632 2024-05-26 15:47:46.000000 flask_openid-1.3.1/Flask_OpenID.egg-info/SOURCES.txt
+-rw-r--r--   0 jarek      (501) staff       (20)        1 2024-05-26 15:47:46.000000 flask_openid-1.3.1/Flask_OpenID.egg-info/dependency_links.txt
+-rw-r--r--   0 jarek      (501) staff       (20)        1 2024-05-26 15:44:18.000000 flask_openid-1.3.1/Flask_OpenID.egg-info/not-zip-safe
+-rw-r--r--   0 jarek      (501) staff       (20)       34 2024-05-26 15:47:46.000000 flask_openid-1.3.1/Flask_OpenID.egg-info/requires.txt
+-rw-r--r--   0 jarek      (501) staff       (20)       13 2024-05-26 15:47:46.000000 flask_openid-1.3.1/Flask_OpenID.egg-info/top_level.txt
+-rw-r--r--   0 jarek      (501) staff       (20)     1723 2024-05-26 15:27:33.000000 flask_openid-1.3.1/LICENSE
+-rw-r--r--   0 jarek      (501) staff       (20)      240 2024-05-26 15:27:33.000000 flask_openid-1.3.1/MANIFEST.in
+-rw-r--r--   0 jarek      (501) staff       (20)     1633 2024-05-26 15:47:46.617947 flask_openid-1.3.1/PKG-INFO
+-rw-r--r--   0 jarek      (501) staff       (20)      584 2024-05-26 15:36:38.000000 flask_openid-1.3.1/README.rst
+drwxr-xr-x   0 jarek      (501) staff       (20)        0 2024-05-26 15:47:46.615917 flask_openid-1.3.1/docs/
+-rw-r--r--   0 jarek      (501) staff       (20)     4569 2024-05-26 15:27:33.000000 flask_openid-1.3.1/docs/Makefile
+drwxr-xr-x   0 jarek      (501) staff       (20)        0 2024-05-26 15:47:46.616046 flask_openid-1.3.1/docs/_static/
+-rw-r--r--   0 jarek      (501) staff       (20)    13828 2024-05-26 15:27:33.000000 flask_openid-1.3.1/docs/_static/flask-openid.png
+drwxr-xr-x   0 jarek      (501) staff       (20)        0 2024-05-26 15:47:46.616222 flask_openid-1.3.1/docs/_themes/
+-rw-r--r--   0 jarek      (501) staff       (20)        0 2024-05-26 15:43:22.000000 flask_openid-1.3.1/docs/_themes/README
+-rw-r--r--   0 jarek      (501) staff       (20)     7105 2024-05-26 15:27:33.000000 flask_openid-1.3.1/docs/conf.py
+-rw-r--r--   0 jarek      (501) staff       (20)     9981 2024-05-26 15:27:33.000000 flask_openid-1.3.1/docs/index.rst
+-rw-r--r--   0 jarek      (501) staff       (20)     4106 2024-05-26 15:27:33.000000 flask_openid-1.3.1/docs/make.bat
+drwxr-xr-x   0 jarek      (501) staff       (20)        0 2024-05-26 15:47:46.616430 flask_openid-1.3.1/example/
+-rw-r--r--   0 jarek      (501) staff       (20)      140 2024-05-26 15:27:33.000000 flask_openid-1.3.1/example/README
+-rwxr-xr-x   0 jarek      (501) staff       (20)     5703 2024-05-26 15:27:33.000000 flask_openid-1.3.1/example/example.py
+drwxr-xr-x   0 jarek      (501) staff       (20)        0 2024-05-26 15:47:46.616671 flask_openid-1.3.1/example/static/
+-rw-r--r--   0 jarek      (501) staff       (20)      433 2024-05-26 15:27:33.000000 flask_openid-1.3.1/example/static/openid.png
+-rw-r--r--   0 jarek      (501) staff       (20)      648 2024-05-26 15:27:33.000000 flask_openid-1.3.1/example/static/style.css
+drwxr-xr-x   0 jarek      (501) staff       (20)        0 2024-05-26 15:47:46.617525 flask_openid-1.3.1/example/templates/
+-rw-r--r--   0 jarek      (501) staff       (20)      742 2024-05-26 15:27:33.000000 flask_openid-1.3.1/example/templates/create_profile.html
+-rw-r--r--   0 jarek      (501) staff       (20)      473 2024-05-26 15:27:33.000000 flask_openid-1.3.1/example/templates/edit_profile.html
+-rw-r--r--   0 jarek      (501) staff       (20)      213 2024-05-26 15:27:33.000000 flask_openid-1.3.1/example/templates/index.html
+-rw-r--r--   0 jarek      (501) staff       (20)      642 2024-05-26 15:27:33.000000 flask_openid-1.3.1/example/templates/layout.html
+-rw-r--r--   0 jarek      (501) staff       (20)      406 2024-05-26 15:27:33.000000 flask_openid-1.3.1/example/templates/login.html
+-rw-r--r--   0 jarek      (501) staff       (20)    22461 2024-05-26 15:27:33.000000 flask_openid-1.3.1/flask_openid.py
+-rw-r--r--   0 jarek      (501) staff       (20)      249 2024-05-26 15:47:46.618291 flask_openid-1.3.1/setup.cfg
+-rw-r--r--   0 jarek      (501) staff       (20)     2058 2024-05-26 15:32:04.000000 flask_openid-1.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Flask-OpenID-1.3.0/Flask_OpenID.egg-info/PKG-INFO` & `flask_openid-1.3.1/Flask_OpenID.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 Metadata-Version: 2.1
 Name: Flask-OpenID
-Version: 1.3.0
+Version: 1.3.1
 Summary: OpenID support for Flask
 Home-page: http://github.com/mitsuhiko/flask-openid/
 Author: Armin Ronacher, Patrick Uiterwijk, Jarek Potiuk, Jason R. Coombs, Emmanuel Bavoux
 Author-email: armin.ronacher@active-4.com, puiterwijk@redhat.com, jarek@potiuk.com, jaraco@jaraco.com, emmanuel.bavoux@free2move.com
 License: BSD
-Description: Flask-OpenID
-        ============
-        
-        Adds support for OpenID to flask applications.  Check out the
-        example for more information.
-        
-        Documentation: http://packages.python.org/Flask-OpenID/
-        
-        
-        CHANGELOG
-        ---------
-        
-        * 1.3.0 Version: 8, September 2021
-        
-        Python 3-only compatible version with 2to3 removed to satisfy
-        setuptools removal of 2to3 configuration option of setup.py
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.0
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: Flask>=0.10.1
+Requires-Dist: python3-openid>=2.0
+
+Flask-OpenID
+============
+
+Adds support for OpenID to flask applications.  Check out the
+example for more information.
+
+Documentation: http://packages.python.org/Flask-OpenID/
+
+Note that this library is for a very old and outdated version of OpenID.
+Almost no-one uses this Open ID protocol, the OpenID Connect protocol is
+the current standard.
+
+CHANGELOG
+---------
+
+* 1.3.1 Version: 26, May 2024
+
+Import quote from urllib.
+
+
+* 1.3.0 Version: 8, September 2021
+
+Python 3-only compatible version with 2to3 removed to satisfy
+setuptools removal of 2to3 configuration option of setup.py
```

### Comparing `Flask-OpenID-1.3.0/LICENSE` & `flask_openid-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-OpenID-1.3.0/PKG-INFO` & `flask_openid-1.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 Metadata-Version: 2.1
 Name: Flask-OpenID
-Version: 1.3.0
+Version: 1.3.1
 Summary: OpenID support for Flask
 Home-page: http://github.com/mitsuhiko/flask-openid/
 Author: Armin Ronacher, Patrick Uiterwijk, Jarek Potiuk, Jason R. Coombs, Emmanuel Bavoux
 Author-email: armin.ronacher@active-4.com, puiterwijk@redhat.com, jarek@potiuk.com, jaraco@jaraco.com, emmanuel.bavoux@free2move.com
 License: BSD
-Description: Flask-OpenID
-        ============
-        
-        Adds support for OpenID to flask applications.  Check out the
-        example for more information.
-        
-        Documentation: http://packages.python.org/Flask-OpenID/
-        
-        
-        CHANGELOG
-        ---------
-        
-        * 1.3.0 Version: 8, September 2021
-        
-        Python 3-only compatible version with 2to3 removed to satisfy
-        setuptools removal of 2to3 configuration option of setup.py
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.0
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: Flask>=0.10.1
+Requires-Dist: python3-openid>=2.0
+
+Flask-OpenID
+============
+
+Adds support for OpenID to flask applications.  Check out the
+example for more information.
+
+Documentation: http://packages.python.org/Flask-OpenID/
+
+Note that this library is for a very old and outdated version of OpenID.
+Almost no-one uses this Open ID protocol, the OpenID Connect protocol is
+the current standard.
+
+CHANGELOG
+---------
+
+* 1.3.1 Version: 26, May 2024
+
+Import quote from urllib.
+
+
+* 1.3.0 Version: 8, September 2021
+
+Python 3-only compatible version with 2to3 removed to satisfy
+setuptools removal of 2to3 configuration option of setup.py
```

### Comparing `Flask-OpenID-1.3.0/docs/Makefile` & `flask_openid-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-OpenID-1.3.0/docs/_static/flask-openid.png` & `flask_openid-1.3.1/docs/_static/flask-openid.png`

 * *Files identical despite different names*

### Comparing `Flask-OpenID-1.3.0/docs/conf.py` & `flask_openid-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-OpenID-1.3.0/docs/index.rst` & `flask_openid-1.3.1/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 How to Use
 ----------
 
 To integrate Flask-OpenID into your application you need to create an
 instance of the :class:`OpenID` object first::
 
-    from flask.ext.openid import OpenID
+    from flask_openid import OpenID
     oid = OpenID(app, '/path/to/store', safe_roots=[])
 
 By default it will use the filesystem as store for information needed by
 OpenID for the authentication process.  You can alternatively implement
 your own store that uses the database or a no-sql server.  For more
 information about that, consult the python-openid documentation.
```

### Comparing `Flask-OpenID-1.3.0/docs/make.bat` & `flask_openid-1.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-OpenID-1.3.0/example/example.py` & `flask_openid-1.3.1/example/example.py`

 * *Files identical despite different names*

### Comparing `Flask-OpenID-1.3.0/example/static/style.css` & `flask_openid-1.3.1/example/static/style.css`

 * *Files identical despite different names*

### Comparing `Flask-OpenID-1.3.0/example/templates/create_profile.html` & `flask_openid-1.3.1/example/templates/create_profile.html`

 * *Files identical despite different names*

### Comparing `Flask-OpenID-1.3.0/example/templates/layout.html` & `flask_openid-1.3.1/example/templates/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-OpenID-1.3.0/flask_openid.py` & `flask_openid-1.3.1/flask_openid.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pickle
 import tempfile
 from functools import wraps
 from datetime import date
 import base64
 
 from flask import request, session, redirect, current_app, url_for
-from werkzeug.urls import url_quote
+import urllib
 
 from openid.store.filestore import FileOpenIDStore
 from openid.extensions import ax
 from openid.extensions.sreg import SRegRequest, SRegResponse
 from openid.consumer.consumer import Consumer, SUCCESS, CANCEL, FAILURE, \
     SETUP_NEEDED
 from openid.consumer import discover
@@ -433,15 +433,15 @@
         for safe_root in self.safe_roots:
             if url.startswith(safe_root):
                 return url
         return None
 
     def get_current_url(self):
         """the current URL + next."""
-        return request.base_url + '?next=' + url_quote(self.get_next_url())
+        return request.base_url + '?next=' + urllib.parse.quote(self.get_next_url())
 
     def get_success_url(self):
         """Return the internal success URL.
 
         :internal:
         """
         return self.get_current_url() + '&openid_complete=yes'
```

### Comparing `Flask-OpenID-1.3.0/setup.py` & `flask_openid-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         print(' - git submodule update')
     else:
         print('You seem to be using a release. Please use the release tarball from PyPI instead of the archive from GitHub')
     sys.exit(1)
 
 setup(
     name='Flask-OpenID',
-    version='1.3.0',
+    version='1.3.1',
     url='http://github.com/mitsuhiko/flask-openid/',
     license='BSD',
     author='Armin Ronacher, Patrick Uiterwijk, Jarek Potiuk, Jason R. Coombs, Emmanuel Bavoux',
     author_email='armin.ronacher@active-4.com, puiterwijk@redhat.com, jarek@potiuk.com, '
                  'jaraco@jaraco.com, emmanuel.bavoux@free2move.com',
     description='OpenID support for Flask',
     py_modules=['flask_openid'],
```

