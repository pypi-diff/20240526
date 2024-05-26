# Comparing `tmp/ansar_connect-0.1.264.tar.gz` & `tmp/ansar_connect-0.1.265.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.264.tar", last modified: Sat May 25 17:56:27 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.265.tar", last modified: Sun May 26 07:30:06 2024, max compression
```

## Comparing `ansar_connect-0.1.264.tar` & `ansar_connect-0.1.265.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.264/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/PKG-INFO
--rwxrwxr-x   0 scott     (1000) scott     (1000)      577 2024-05-23 01:07:25.000000 ansar_connect-0.1.264/README.md
--rwxrwxr-x   0 scott     (1000) scott     (1000)      764 2024-05-24 13:44:08.000000 ansar_connect-0.1.264/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/setup.cfg
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2251 2024-05-24 13:44:00.000000 ansar_connect-0.1.264/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.264/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.264/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.264/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.264/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-25 17:56:24.000000 ansar_connect-0.1.264/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.264/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    88764 2024-05-24 02:37:42.000000 ansar_connect-0.1.264/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.264/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.264/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.264/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    15853 2024-05-20 01:19:54.000000 ansar_connect-0.1.264/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.264/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.264/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.264/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9715 2024-05-24 13:42:13.000000 ansar_connect-0.1.264/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.264/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.264/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.264/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    42423 2024-05-25 17:54:22.000000 ansar_connect-0.1.264/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.264/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.264/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.264/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.264/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-25 17:56:27.000000 ansar_connect-0.1.264/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-25 17:56:27.000000 ansar_connect-0.1.264/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-25 17:56:27.000000 ansar_connect-0.1.264/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-25 17:56:27.000000 ansar_connect-0.1.264/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-25 17:56:27.000000 ansar_connect-0.1.264/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-25 17:56:27.000000 ansar_connect-0.1.264/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:30:06.895354 ansar_connect-0.1.265/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.265/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-26 07:30:06.895354 ansar_connect-0.1.265/PKG-INFO
+-rwxrwxr-x   0 scott     (1000) scott     (1000)      577 2024-05-23 01:07:25.000000 ansar_connect-0.1.265/README.md
+-rwxrwxr-x   0 scott     (1000) scott     (1000)      764 2024-05-26 07:28:48.000000 ansar_connect-0.1.265/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-26 07:30:06.895354 ansar_connect-0.1.265/setup.cfg
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2251 2024-05-26 07:28:40.000000 ansar_connect-0.1.265/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:30:06.891354 ansar_connect-0.1.265/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:30:06.891354 ansar_connect-0.1.265/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:30:06.891354 ansar_connect-0.1.265/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.265/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.265/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.265/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.265/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:30:06.891354 ansar_connect-0.1.265/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-26 07:30:03.000000 ansar_connect-0.1.265/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.265/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    88764 2024-05-24 02:37:42.000000 ansar_connect-0.1.265/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.265/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.265/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.265/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    15853 2024-05-20 01:19:54.000000 ansar_connect-0.1.265/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.265/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.265/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.265/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9715 2024-05-24 13:42:13.000000 ansar_connect-0.1.265/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.265/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.265/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.265/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    42336 2024-05-26 07:25:14.000000 ansar_connect-0.1.265/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.265/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.265/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.265/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.265/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-26 07:30:06.895354 ansar_connect-0.1.265/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-26 07:30:06.000000 ansar_connect-0.1.265/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-26 07:30:06.000000 ansar_connect-0.1.265/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-26 07:30:06.000000 ansar_connect-0.1.265/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-26 07:30:06.000000 ansar_connect-0.1.265/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-26 07:30:06.000000 ansar_connect-0.1.265/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-26 07:30:06.000000 ansar_connect-0.1.265/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.264/LICENSE` & `ansar_connect-0.1.265/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/PKG-INFO` & `ansar_connect-0.1.265/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.264
+Version: 0.1.265
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi>=1.16.0
 Requires-Dist: PyNaCl>=1.5.0
-Requires-Dist: ansar-create>=0.1.97
+Requires-Dist: ansar-create>=0.1.98
 
 # ansar-connect
 
 The **ansar-connect** library implements clear and concise network messaging for a wide range
 of networking requirements. From multi-processing within a single host through to messaging
 beween different LANs on the Internet. There is a single send method that does it all.
```

### Comparing `ansar_connect-0.1.264/README.md` & `ansar_connect-0.1.265/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/pyproject.toml` & `ansar_connect-0.1.265/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 	"Operating System :: OS Independent",
 	"Topic :: Software Development :: Libraries"
 ]
 dynamic = ["description", "version", "scripts"]
 dependencies = [
     "cffi>=1.16.0",
     "PyNaCl>=1.5.0",
-    "ansar-create>=0.1.97"
+    "ansar-create>=0.1.98"
 ]
 
 [project.urls]
 Documentation = "https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html"
```

### Comparing `ansar_connect-0.1.264/setup.py` & `ansar_connect-0.1.265/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 with open("DOC_LATEST_LINK", "r", encoding="utf-8") as f:
     d = f.read()
 DOC_LINK = d[:-1]
 
 REQUIRES = [
     "cffi>=1.16.0",
     "PyNaCl>=1.5.0",
-    "ansar-create>=0.1.97",
+    "ansar-create>=0.1.98",
 ]
 
 setuptools.setup(
     name=PACKAGE,
     version=VERSION,
     author="Scott Woods",
     author_email="scott.18.ansar@gmail.com.com",
```

### Comparing `ansar_connect-0.1.264/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.265/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.265/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.265/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.265/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/__init__.py` & `ansar_connect-0.1.265/src/ansar/connect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 8882f193a8d2735e5e8b6a2203b52ca05f800335
-Version: 0.1.263 (2024-05-26@05:56:24+NZST)
+Commit: 17398607d16ea49e8b7e55afe3d9ddb1bf27afd8
+Version: 0.1.264 (2024-05-26@19:30:03+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.264/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.265/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/directory.py` & `ansar_connect-0.1.265/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.265/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.265/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/group_if.py` & `ansar_connect-0.1.265/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/grouping.py` & `ansar_connect-0.1.265/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/moving.py` & `ansar_connect-0.1.265/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/networking.py` & `ansar_connect-0.1.265/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.265/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/node.py` & `ansar_connect-0.1.265/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.265/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/procedure.py` & `ansar_connect-0.1.265/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/product.py` & `ansar_connect-0.1.265/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/socketry.py` & `ansar_connect-0.1.265/src/ansar/connect/socketry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1209,26 +1209,22 @@
 		value = ar.Faulted(condition='cannot stream outbound', explanation=str(e))
 		self.warning(str(value))
 		close_session(stream, value, s)
 		return
 
 	try:
 		self.sending.remove(s)
-	except KeyError:
+	except ValueError:
 		pass
 
 # A network transport for the purpose of exchanging
 # messages between machines.
 
 def TcpStream_ReceiveBlock(self, stream, s):
 	try:
-		if stream.closing:
-			end_of_session(self, stream, s, 'receive on closing')
-			return
-
 		scrap = s.recv(TCP_RECV)
 		if not scrap:
 			end_of_session(self, stream, s, 'empty socket')
 			return
 
 		try:
 			stream.receive_and_route(scrap, self)
```

### Comparing `ansar_connect-0.1.264/src/ansar/connect/standard.py` & `ansar_connect-0.1.265/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/transporting.py` & `ansar_connect-0.1.265/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.265/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar/connect/wan.py` & `ansar_connect-0.1.265/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.264/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.265/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.264
+Version: 0.1.265
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi>=1.16.0
 Requires-Dist: PyNaCl>=1.5.0
-Requires-Dist: ansar-create>=0.1.97
+Requires-Dist: ansar-create>=0.1.98
 
 # ansar-connect
 
 The **ansar-connect** library implements clear and concise network messaging for a wide range
 of networking requirements. From multi-processing within a single host through to messaging
 beween different LANs on the Internet. There is a single send method that does it all.
```

### Comparing `ansar_connect-0.1.264/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.265/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

