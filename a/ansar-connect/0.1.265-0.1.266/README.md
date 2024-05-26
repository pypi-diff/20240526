# Comparing `tmp/ansar_connect-0.1.265.tar.gz` & `tmp/ansar_connect-0.1.266.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.265.tar", last modified: Sun May 26 07:30:06 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.266.tar", last modified: Sun May 26 07:38:09 2024, max compression
```

## Comparing `ansar_connect-0.1.265.tar` & `ansar_connect-0.1.266.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:30:06.895354 ansar_connect-0.1.265/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.265/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-26 07:30:06.895354 ansar_connect-0.1.265/PKG-INFO
--rwxrwxr-x   0 scott     (1000) scott     (1000)      577 2024-05-23 01:07:25.000000 ansar_connect-0.1.265/README.md
--rwxrwxr-x   0 scott     (1000) scott     (1000)      764 2024-05-26 07:28:48.000000 ansar_connect-0.1.265/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-26 07:30:06.895354 ansar_connect-0.1.265/setup.cfg
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2251 2024-05-26 07:28:40.000000 ansar_connect-0.1.265/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:30:06.891354 ansar_connect-0.1.265/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:30:06.891354 ansar_connect-0.1.265/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:30:06.891354 ansar_connect-0.1.265/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.265/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.265/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.265/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.265/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:30:06.891354 ansar_connect-0.1.265/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-26 07:30:03.000000 ansar_connect-0.1.265/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.265/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    88764 2024-05-24 02:37:42.000000 ansar_connect-0.1.265/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.265/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.265/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.265/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    15853 2024-05-20 01:19:54.000000 ansar_connect-0.1.265/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.265/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.265/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.265/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9715 2024-05-24 13:42:13.000000 ansar_connect-0.1.265/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.265/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.265/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.265/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    42336 2024-05-26 07:25:14.000000 ansar_connect-0.1.265/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.265/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.265/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.265/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.265/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:30:06.895354 ansar_connect-0.1.265/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-26 07:30:06.000000 ansar_connect-0.1.265/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-26 07:30:06.000000 ansar_connect-0.1.265/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-26 07:30:06.000000 ansar_connect-0.1.265/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-26 07:30:06.000000 ansar_connect-0.1.265/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-26 07:30:06.000000 ansar_connect-0.1.265/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-26 07:30:06.000000 ansar_connect-0.1.265/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:38:09.155658 ansar_connect-0.1.266/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.266/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-26 07:38:09.155658 ansar_connect-0.1.266/PKG-INFO
+-rwxrwxr-x   0 scott     (1000) scott     (1000)      577 2024-05-23 01:07:25.000000 ansar_connect-0.1.266/README.md
+-rwxrwxr-x   0 scott     (1000) scott     (1000)      764 2024-05-26 07:28:48.000000 ansar_connect-0.1.266/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-26 07:38:09.155658 ansar_connect-0.1.266/setup.cfg
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2251 2024-05-26 07:28:40.000000 ansar_connect-0.1.266/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:38:09.151658 ansar_connect-0.1.266/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:38:09.151658 ansar_connect-0.1.266/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:38:09.151658 ansar_connect-0.1.266/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.266/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.266/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.266/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.266/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:38:09.151658 ansar_connect-0.1.266/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-26 07:38:06.000000 ansar_connect-0.1.266/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.266/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    88764 2024-05-24 02:37:42.000000 ansar_connect-0.1.266/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.266/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.266/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.266/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    15853 2024-05-20 01:19:54.000000 ansar_connect-0.1.266/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.266/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.266/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.266/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9679 2024-05-26 07:36:57.000000 ansar_connect-0.1.266/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.266/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.266/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.266/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    42336 2024-05-26 07:25:14.000000 ansar_connect-0.1.266/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.266/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.266/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.266/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.266/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:38:09.155658 ansar_connect-0.1.266/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-26 07:38:09.000000 ansar_connect-0.1.266/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-26 07:38:09.000000 ansar_connect-0.1.266/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-26 07:38:09.000000 ansar_connect-0.1.266/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-26 07:38:09.000000 ansar_connect-0.1.266/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-26 07:38:09.000000 ansar_connect-0.1.266/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-26 07:38:09.000000 ansar_connect-0.1.266/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.265/LICENSE` & `ansar_connect-0.1.266/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/PKG-INFO` & `ansar_connect-0.1.266/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.265
+Version: 0.1.266
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.265/README.md` & `ansar_connect-0.1.266/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/pyproject.toml` & `ansar_connect-0.1.266/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/setup.py` & `ansar_connect-0.1.266/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.266/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.266/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.266/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.266/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/__init__.py` & `ansar_connect-0.1.266/src/ansar/connect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 17398607d16ea49e8b7e55afe3d9ddb1bf27afd8
-Version: 0.1.264 (2024-05-26@19:30:03+NZST)
+Commit: fefa41b6bd9182a9d813f24c0b5168016251bc66
+Version: 0.1.265 (2024-05-26@19:38:06+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.265/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.266/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/directory.py` & `ansar_connect-0.1.266/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.266/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.266/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/group_if.py` & `ansar_connect-0.1.266/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/grouping.py` & `ansar_connect-0.1.266/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/moving.py` & `ansar_connect-0.1.266/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/networking.py` & `ansar_connect-0.1.266/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.266/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/node.py` & `ansar_connect-0.1.266/src/ansar/connect/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 import sys
 import signal
 import uuid
 import time
 
 import ansar.create as ar
 import ansar.create.point as ap
-import ansar.create.object as aco
 from .socketry import *
 from .directory_if import *
 from .directory import *
 from .wan import *
 from .transporting import *
 
 __all__ = [
@@ -185,15 +184,15 @@
 	self.trace('Class threads (%d) %s' % (len(ap.pt.thread_classes), ','.join(name_counts)))
 
 	# One source of directory information.
 	# Persistent.
 	p = role.properties
 
 	def return_signal(value):
-		ar.co.signal_received = aco.SIGNAL_KILL
+		ar.co.signal_received = signal.SIGKILL
 		return value
 
 	# Start with the scope enumeration passed through from
 	# create_node().
 	scope = node_settings.node_scope
 	if scope is None:
 		return ar.Failed(node_scope=(None, 'scope is undefined'))
@@ -238,15 +237,15 @@
 			m = self.select(ar.Completed, ar.Stop, ar.Pause, ar.Resume)
 
 			if isinstance(m, ar.Completed):
 				# Do a "fake" signaling. Sidestep all the platform machinery
 				# and just set a global. It does avoid any complexities
 				# arising from overlapping events. Spent far too much time
 				# trying to untangle signals, exceptions and interrupted i/o.
-				ar.co.signal_received = aco.SIGNAL_KILL
+				ar.co.signal_received = signal.SIGKILL
 				return m.value
 			elif isinstance(m, ar.Stop):
 				# Received a Stop.
 				self.send(m, a)
 				m = self.select(ar.Completed)
 				return m.value
```

### Comparing `ansar_connect-0.1.265/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.266/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/procedure.py` & `ansar_connect-0.1.266/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/product.py` & `ansar_connect-0.1.266/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/socketry.py` & `ansar_connect-0.1.266/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/standard.py` & `ansar_connect-0.1.266/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/transporting.py` & `ansar_connect-0.1.266/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.266/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar/connect/wan.py` & `ansar_connect-0.1.266/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.265/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.266/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.265
+Version: 0.1.266
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.265/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.266/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

