# Comparing `tmp/pyrqlite-2.2.2.tar.gz` & `tmp/pyrqlite-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrqlite-2.2.2.tar", last modified: Mon Jan 22 02:02:11 2024, max compression
+gzip compressed data, was "pyrqlite-2.2.3.tar", last modified: Sun May 26 04:10:50 2024, max compression
```

## Comparing `pyrqlite-2.2.2.tar` & `pyrqlite-2.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 02:02:11.262105 pyrqlite-2.2.2/
--rw-rw-r--   0 root         (0) root         (0)     1077 2024-01-03 15:42:59.000000 pyrqlite-2.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1917 2024-01-22 02:02:11.261105 pyrqlite-2.2.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2559 2024-01-11 01:34:14.000000 pyrqlite-2.2.2/README.rst
--rw-rw-r--   0 root         (0) root         (0)      686 2024-01-22 01:59:00.000000 pyrqlite-2.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-22 02:02:11.262105 pyrqlite-2.2.2/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     3219 2024-01-22 01:57:36.000000 pyrqlite-2.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 02:02:11.251105 pyrqlite-2.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 02:02:11.258105 pyrqlite-2.2.2/src/pyrqlite/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-03 15:42:59.000000 pyrqlite-2.2.2/src/pyrqlite/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3284 2024-01-03 15:42:59.000000 pyrqlite-2.2.2/src/pyrqlite/_ephemeral.py
--rw-rw-r--   0 root         (0) root         (0)     5963 2024-01-03 15:42:59.000000 pyrqlite-2.2.2/src/pyrqlite/connections.py
--rw-rw-r--   0 root         (0) root         (0)      273 2024-01-03 15:42:59.000000 pyrqlite-2.2.2/src/pyrqlite/constants.py
--rw-rw-r--   0 root         (0) root         (0)    11398 2024-01-03 15:42:59.000000 pyrqlite-2.2.2/src/pyrqlite/cursors.py
--rw-rw-r--   0 root         (0) root         (0)     1124 2024-01-03 15:42:59.000000 pyrqlite-2.2.2/src/pyrqlite/dbapi2.py
--rw-rw-r--   0 root         (0) root         (0)      207 2024-01-03 15:42:59.000000 pyrqlite-2.2.2/src/pyrqlite/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     7551 2024-01-03 15:42:59.000000 pyrqlite-2.2.2/src/pyrqlite/extensions.py
--rw-rw-r--   0 root         (0) root         (0)     2065 2024-01-11 19:03:18.000000 pyrqlite-2.2.2/src/pyrqlite/row.py
--rw-rw-r--   0 root         (0) root         (0)      346 2024-01-03 15:42:59.000000 pyrqlite-2.2.2/src/pyrqlite/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 02:02:11.261105 pyrqlite-2.2.2/src/pyrqlite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1917 2024-01-22 02:02:11.000000 pyrqlite-2.2.2/src/pyrqlite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-22 02:02:11.000000 pyrqlite-2.2.2/src/pyrqlite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-22 02:02:11.000000 pyrqlite-2.2.2/src/pyrqlite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-01-22 02:02:11.000000 pyrqlite-2.2.2/src/pyrqlite.egg-info/top_level.txt
+drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2024-05-26 04:10:50.299583 pyrqlite-2.2.3/
+-rw-rw-r--   0 zmedico   (1000) zmedico   (1000)     1077 2024-01-03 15:42:59.000000 pyrqlite-2.2.3/LICENSE
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)     1917 2024-05-26 04:10:50.299583 pyrqlite-2.2.3/PKG-INFO
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)     2841 2024-05-25 20:16:41.000000 pyrqlite-2.2.3/README.rst
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)      686 2024-05-26 04:10:00.000000 pyrqlite-2.2.3/pyproject.toml
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)       38 2024-05-26 04:10:50.299583 pyrqlite-2.2.3/setup.cfg
+-rwxr-xr-x   0 zmedico   (1000) zmedico   (1000)     3219 2024-05-25 20:22:50.000000 pyrqlite-2.2.3/setup.py
+drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2024-05-26 04:10:50.292583 pyrqlite-2.2.3/src/
+drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2024-05-26 04:10:50.296583 pyrqlite-2.2.3/src/pyrqlite/
+-rw-rw-r--   0 zmedico   (1000) zmedico   (1000)        0 2024-01-03 15:42:59.000000 pyrqlite-2.2.3/src/pyrqlite/__init__.py
+-rw-rw-r--   0 zmedico   (1000) zmedico   (1000)     3284 2024-01-03 15:42:59.000000 pyrqlite-2.2.3/src/pyrqlite/_ephemeral.py
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)     6560 2024-03-24 19:18:09.000000 pyrqlite-2.2.3/src/pyrqlite/connections.py
+-rw-rw-r--   0 zmedico   (1000) zmedico   (1000)      273 2024-01-03 15:42:59.000000 pyrqlite-2.2.3/src/pyrqlite/constants.py
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)    11398 2024-05-26 03:58:46.000000 pyrqlite-2.2.3/src/pyrqlite/cursors.py
+-rw-rw-r--   0 zmedico   (1000) zmedico   (1000)     1124 2024-01-03 15:42:59.000000 pyrqlite-2.2.3/src/pyrqlite/dbapi2.py
+-rw-rw-r--   0 zmedico   (1000) zmedico   (1000)      207 2024-01-03 15:42:59.000000 pyrqlite-2.2.3/src/pyrqlite/exceptions.py
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)     7578 2024-05-25 20:22:54.000000 pyrqlite-2.2.3/src/pyrqlite/extensions.py
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)     2065 2024-01-22 02:07:16.000000 pyrqlite-2.2.3/src/pyrqlite/row.py
+-rw-rw-r--   0 zmedico   (1000) zmedico   (1000)      346 2024-01-03 15:42:59.000000 pyrqlite-2.2.3/src/pyrqlite/types.py
+drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2024-05-26 04:10:50.298583 pyrqlite-2.2.3/src/pyrqlite.egg-info/
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)     1917 2024-05-26 04:10:50.000000 pyrqlite-2.2.3/src/pyrqlite.egg-info/PKG-INFO
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)      435 2024-05-26 04:10:50.000000 pyrqlite-2.2.3/src/pyrqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)        1 2024-05-26 04:10:50.000000 pyrqlite-2.2.3/src/pyrqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)        9 2024-05-26 04:10:50.000000 pyrqlite-2.2.3/src/pyrqlite.egg-info/top_level.txt
```

### Comparing `pyrqlite-2.2.2/LICENSE` & `pyrqlite-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrqlite-2.2.2/PKG-INFO` & `pyrqlite-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrqlite
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python rqlite client library
 Home-page: https://github.com/rqlite/pyrqlite/
 Author: Zac Medico
 Author-email: Zac Medico <zmedico@gmail.com>, Philip O'Toole <philip.otoole@yahoo.com>
 Maintainer: Zac Medico
 Maintainer-email: zmedico@gmail.com
 License: The MIT License (MIT)
```

### Comparing `pyrqlite-2.2.2/README.rst` & `pyrqlite-2.2.3/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-=======
+-------------
 pyrqlite
-=======
+-------------
+
 .. image:: https://circleci.com/gh/rqlite/pyrqlite.svg?style=svg
     :target: https://circleci.com/gh/rqlite/pyrqlite
 
 This package contains a pure-Python rqlite client library.
 
 .. contents::
 
@@ -21,23 +22,31 @@
 Installation
 ------------
 
 The last stable release is available on github and can be installed with ``pip``::
 
     $ pip install git+https://github.com/rqlite/pyrqlite.git
 
-Alternatively (e.g. if ``pip`` is not available), a tarball can be downloaded
+You can also just clone the repo and install it from source::
+
+    $ git clone https://github.com/rqlite/pyrqlite.git
+    $ cd pyrqlite
+    $ python setup.py install
+
+Finally (e.g. if ``pip`` is not available), a tarball can be downloaded
 from GitHub and installed with Setuptools::
 
-    $ # X.X is the desired pyrqlite version (e.g. 0.5 or 0.6).
-    $ curl -L https://github.com/rqlite/tarball/pyrqlite-X.X | tar xz
+    $ # X.Y.Z is the desired pyrqlite version (e.g. 2.2.1).
+    $ curl -L https://github.com/rqlite/pyrqlite/archive/refs/tags/vX.Y.Z.tar.gz | tar xz
     $ cd pyrqlite*
     $ python setup.py install
     $ # The folder pyrqlite* can be safely removed now.
 
+You mean need to run the installation process with ``root`` privileges.
+
 Test Suite
 ----------
 
 To run all the tests, execute the script ``setup.py``::
 
     $ python setup.py test
 
@@ -83,23 +92,23 @@
 This example will print:
 
 
     (1, 'a')
     (2, 'b')
     
 Paramstyle
----------
+-------------
 
 Only qmark and named paramstyles (as defined in PEP 249) are supported. 
 
 Limitations
----------
+-------------
 Transactions are not supported.
 
 Resources
----------
+-------------
 DB-API 2.0: http://www.python.org/dev/peps/pep-0249
 
 
 License
--------
+-------------
 pyrqlite is released under the MIT License. See LICENSE for more information.
```

### Comparing `pyrqlite-2.2.2/setup.py` & `pyrqlite-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyrqlite-2.2.2/src/pyrqlite/_ephemeral.py` & `pyrqlite-2.2.3/src/pyrqlite/_ephemeral.py`

 * *Files identical despite different names*

### Comparing `pyrqlite-2.2.2/src/pyrqlite/connections.py` & `pyrqlite-2.2.3/src/pyrqlite/connections.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 from __future__ import unicode_literals
 
 import codecs
 import logging
+import warnings
 
 try:
     from http.client import HTTPConnection, HTTPSConnection
 except ImportError:
     # pylint: disable=import-error
     from httplib import HTTPConnection, HTTPSConnection
 
@@ -36,42 +37,68 @@
         OperationalError,
         IntegrityError,
         InternalError,
         ProgrammingError,
         NotSupportedError,
     )
 
-    def __init__(self, scheme='http', host='localhost', port=4001, ssl_context=None,
-                 user=None, password=None, connect_timeout=None,
-                 detect_types=0, max_redirects=UNLIMITED_REDIRECTS):
+    def __init__(
+        self,
+        scheme="http",
+        host="localhost",
+        port=4001,
+        ssl_context=None,
+        user=None,
+        password=None,
+        connect_timeout=DeprecationWarning,
+        timeout=None,
+        detect_types=0,
+        max_redirects=UNLIMITED_REDIRECTS,
+    ):
 
         self.messages = []
         self.scheme = scheme
         self.host = host
         self.port = port
         self.ssl_context = ssl_context
         self._headers = {}
         if not (user is None or password is None):
             self._headers['Authorization'] = 'Basic ' + \
                 codecs.encode('{}:{}'.format(user, password).encode('utf-8'),
                               'base64').decode('utf-8').rstrip('\n')
 
-        self.connect_timeout = connect_timeout
+        if connect_timeout is not DeprecationWarning:
+            warnings.warn(
+                "connect_timeout parameter is deprecated and renamed to timeout",
+                DeprecationWarning,
+                stacklevel=1,
+            )
+            timeout = connect_timeout
+        self.timeout = timeout
         self.max_redirects = max_redirects
         self.detect_types = detect_types
         self.parse_decltypes = detect_types & PARSE_DECLTYPES
         self.parse_colnames = detect_types & PARSE_COLNAMES
         self._ephemeral = None
         if scheme == ':memory:':
             self._ephemeral = _EphemeralRqlited().__enter__()
             self.host, self.port = self._ephemeral.http
         self._connection = self._init_connection()
 
+    @property
+    def connect_timeout(self):
+        warnings.warn(
+            "connect_timeout attribute is deprecated and renamed to timeout",
+            DeprecationWarning,
+            stacklevel=1,
+        )
+        return self.timeout
+
     def _init_connection(self):
-        timeout = None if self.connect_timeout is None else float(self.connect_timeout)
+        timeout = None if self.timeout is None else float(self.timeout)
         if self.scheme in ('http', ':memory:'):
             return HTTPConnection(self.host, port=self.port, timeout=timeout)
         elif self.scheme == 'https':
             return HTTPSConnection(self.host, port=self.port, context=self.ssl_context,
                                    timeout=timeout)
         else:
             raise Connection.ProgrammingError('Unsupported scheme %r' % self.scheme)
```

### Comparing `pyrqlite-2.2.2/src/pyrqlite/cursors.py` & `pyrqlite-2.2.3/src/pyrqlite/cursors.py`

 * *Files identical despite different names*

### Comparing `pyrqlite-2.2.2/src/pyrqlite/dbapi2.py` & `pyrqlite-2.2.3/src/pyrqlite/dbapi2.py`

 * *Files identical despite different names*

### Comparing `pyrqlite-2.2.2/src/pyrqlite/extensions.py` & `pyrqlite-2.2.3/src/pyrqlite/extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     'INTEGER': functools.partial(_null_wrapper, int),
     'BOOL': functools.partial(_null_wrapper, bool),
     'FLOAT': functools.partial(_null_wrapper, float),
     'REAL': functools.partial(_null_wrapper, float),
     'NULL': lambda x: None,
     'BLOB': lambda x: x,
     'DATE': functools.partial(_null_wrapper, _convert_date),
-    'DATETIME': lambda x: x.replace('T', ' ').rstrip('Z'),
+    'DATETIME': lambda x: x.replace('T', ' ').rstrip('Z') if x is not None else None,
     'TIMESTAMP': functools.partial(_null_wrapper, _convert_timestamp),
 }
 
 # Non-native converters will be decoded from base64 before fed into converter
 _native_converters = ('BOOL', 'FLOAT', 'INTEGER', 'REAL', 'NUMBER', 'NULL', 'DATE', 'DATETIME', 'TIMESTAMP')
 
 # SQLite TEXT affinity: https://www.sqlite.org/datatype3.html
```

### Comparing `pyrqlite-2.2.2/src/pyrqlite/row.py` & `pyrqlite-2.2.3/src/pyrqlite/row.py`

 * *Files identical despite different names*

### Comparing `pyrqlite-2.2.2/src/pyrqlite.egg-info/PKG-INFO` & `pyrqlite-2.2.3/src/pyrqlite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrqlite
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python rqlite client library
 Home-page: https://github.com/rqlite/pyrqlite/
 Author: Zac Medico
 Author-email: Zac Medico <zmedico@gmail.com>, Philip O'Toole <philip.otoole@yahoo.com>
 Maintainer: Zac Medico
 Maintainer-email: zmedico@gmail.com
 License: The MIT License (MIT)
```

