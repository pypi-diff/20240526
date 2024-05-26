# Comparing `tmp/filedgr-ipfs-libs-0.0.2b4.tar.gz` & `tmp/filedgr_ipfs_libs-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filedgr-ipfs-libs-0.0.2b4.tar", last modified: Mon Dec 11 00:48:00 2023, max compression
+gzip compressed data, was "filedgr_ipfs_libs-0.1.0b1.tar", last modified: Sun May 26 20:25:06 2024, max compression
```

## Comparing `filedgr-ipfs-libs-0.0.2b4.tar` & `filedgr_ipfs_libs-0.1.0b1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2023-12-11 00:48:00.055107 filedgr-ipfs-libs-0.0.2b4/
--rw-r--r--   0 ericfalk   (501) staff       (20)     1063 2022-06-18 17:54:13.000000 filedgr-ipfs-libs-0.0.2b4/LICENSE
--rw-r--r--   0 ericfalk   (501) staff       (20)      975 2023-12-11 00:48:00.054990 filedgr-ipfs-libs-0.0.2b4/PKG-INFO
--rw-r--r--   0 ericfalk   (501) staff       (20)       83 2022-11-12 18:36:02.000000 filedgr-ipfs-libs-0.0.2b4/README.md
--rw-r--r--   0 ericfalk   (501) staff       (20)     1384 2023-12-11 00:47:25.000000 filedgr-ipfs-libs-0.0.2b4/pyproject.toml
--rw-r--r--   0 ericfalk   (501) staff       (20)      142 2023-12-11 00:48:00.055540 filedgr-ipfs-libs-0.0.2b4/setup.cfg
-drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2023-12-11 00:48:00.047345 filedgr-ipfs-libs-0.0.2b4/src/
-drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2023-12-11 00:48:00.053741 filedgr-ipfs-libs-0.0.2b4/src/filedgr_ipfs_libs.egg-info/
--rw-r--r--   0 ericfalk   (501) staff       (20)      975 2023-12-11 00:48:00.000000 filedgr-ipfs-libs-0.0.2b4/src/filedgr_ipfs_libs.egg-info/PKG-INFO
--rw-r--r--   0 ericfalk   (501) staff       (20)      441 2023-12-11 00:48:00.000000 filedgr-ipfs-libs-0.0.2b4/src/filedgr_ipfs_libs.egg-info/SOURCES.txt
--rw-r--r--   0 ericfalk   (501) staff       (20)        1 2023-12-11 00:48:00.000000 filedgr-ipfs-libs-0.0.2b4/src/filedgr_ipfs_libs.egg-info/dependency_links.txt
--rw-r--r--   0 ericfalk   (501) staff       (20)       96 2023-12-11 00:48:00.000000 filedgr-ipfs-libs-0.0.2b4/src/filedgr_ipfs_libs.egg-info/requires.txt
--rw-r--r--   0 ericfalk   (501) staff       (20)       17 2023-12-11 00:48:00.000000 filedgr-ipfs-libs-0.0.2b4/src/filedgr_ipfs_libs.egg-info/top_level.txt
-drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2023-12-11 00:48:00.051793 filedgr-ipfs-libs-0.0.2b4/src/filedgr_lib_ipfs/
--rw-r--r--   0 ericfalk   (501) staff       (20)        0 2023-07-19 15:06:05.000000 filedgr-ipfs-libs-0.0.2b4/src/filedgr_lib_ipfs/__init__.py
--rw-r--r--   0 ericfalk   (501) staff       (20)     3168 2023-12-11 00:44:13.000000 filedgr-ipfs-libs-0.0.2b4/src/filedgr_lib_ipfs/ipfs_client.py
-drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2023-12-11 00:48:00.052464 filedgr-ipfs-libs-0.0.2b4/src/filedgr_lib_ipfs/my_io/
--rw-r--r--   0 ericfalk   (501) staff       (20)        0 2022-06-18 17:23:43.000000 filedgr-ipfs-libs-0.0.2b4/src/filedgr_lib_ipfs/my_io/__init__.py
--rw-r--r--   0 ericfalk   (501) staff       (20)      508 2022-06-18 17:40:10.000000 filedgr-ipfs-libs-0.0.2b4/src/filedgr_lib_ipfs/my_io/my_file_io.py
-drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2023-12-11 00:48:00.053312 filedgr-ipfs-libs-0.0.2b4/tests/
--rw-r--r--   0 ericfalk   (501) staff       (20)     1174 2023-12-11 00:44:48.000000 filedgr-ipfs-libs-0.0.2b4/tests/test_ipfs_client.py
+drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2024-05-26 20:25:06.696710 filedgr_ipfs_libs-0.1.0b1/
+-rw-r--r--   0 ericfalk   (501) staff       (20)     1063 2022-06-18 17:54:13.000000 filedgr_ipfs_libs-0.1.0b1/LICENSE
+-rw-r--r--   0 ericfalk   (501) staff       (20)      975 2024-05-26 20:25:06.696563 filedgr_ipfs_libs-0.1.0b1/PKG-INFO
+-rw-r--r--   0 ericfalk   (501) staff       (20)       83 2022-11-12 18:36:02.000000 filedgr_ipfs_libs-0.1.0b1/README.md
+-rw-r--r--   0 ericfalk   (501) staff       (20)     1384 2024-05-26 20:23:56.000000 filedgr_ipfs_libs-0.1.0b1/pyproject.toml
+-rw-r--r--   0 ericfalk   (501) staff       (20)      142 2024-05-26 20:25:06.697320 filedgr_ipfs_libs-0.1.0b1/setup.cfg
+drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2024-05-26 20:25:06.688748 filedgr_ipfs_libs-0.1.0b1/src/
+drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2024-05-26 20:25:06.695027 filedgr_ipfs_libs-0.1.0b1/src/filedgr_ipfs_libs.egg-info/
+-rw-r--r--   0 ericfalk   (501) staff       (20)      975 2024-05-26 20:25:06.000000 filedgr_ipfs_libs-0.1.0b1/src/filedgr_ipfs_libs.egg-info/PKG-INFO
+-rw-r--r--   0 ericfalk   (501) staff       (20)      441 2024-05-26 20:25:06.000000 filedgr_ipfs_libs-0.1.0b1/src/filedgr_ipfs_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 ericfalk   (501) staff       (20)        1 2024-05-26 20:25:06.000000 filedgr_ipfs_libs-0.1.0b1/src/filedgr_ipfs_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 ericfalk   (501) staff       (20)       96 2024-05-26 20:25:06.000000 filedgr_ipfs_libs-0.1.0b1/src/filedgr_ipfs_libs.egg-info/requires.txt
+-rw-r--r--   0 ericfalk   (501) staff       (20)       17 2024-05-26 20:25:06.000000 filedgr_ipfs_libs-0.1.0b1/src/filedgr_ipfs_libs.egg-info/top_level.txt
+drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2024-05-26 20:25:06.693066 filedgr_ipfs_libs-0.1.0b1/src/filedgr_lib_ipfs/
+-rw-r--r--   0 ericfalk   (501) staff       (20)        0 2023-07-19 15:06:05.000000 filedgr_ipfs_libs-0.1.0b1/src/filedgr_lib_ipfs/__init__.py
+-rw-r--r--   0 ericfalk   (501) staff       (20)     3168 2023-12-11 00:44:13.000000 filedgr_ipfs_libs-0.1.0b1/src/filedgr_lib_ipfs/ipfs_client.py
+drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2024-05-26 20:25:06.693833 filedgr_ipfs_libs-0.1.0b1/src/filedgr_lib_ipfs/my_io/
+-rw-r--r--   0 ericfalk   (501) staff       (20)        0 2022-06-18 17:23:43.000000 filedgr_ipfs_libs-0.1.0b1/src/filedgr_lib_ipfs/my_io/__init__.py
+-rw-r--r--   0 ericfalk   (501) staff       (20)      508 2022-06-18 17:40:10.000000 filedgr_ipfs_libs-0.1.0b1/src/filedgr_lib_ipfs/my_io/my_file_io.py
+drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2024-05-26 20:25:06.694335 filedgr_ipfs_libs-0.1.0b1/tests/
+-rw-r--r--   0 ericfalk   (501) staff       (20)     1265 2023-12-11 15:20:29.000000 filedgr_ipfs_libs-0.1.0b1/tests/test_ipfs_client.py
```

### Comparing `filedgr-ipfs-libs-0.0.2b4/LICENSE` & `filedgr_ipfs_libs-0.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `filedgr-ipfs-libs-0.0.2b4/PKG-INFO` & `filedgr_ipfs_libs-0.1.0b1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: filedgr-ipfs-libs
-Version: 0.0.2b4
+Version: 0.1.0b1
 Summary: Python libs to interact with the IPFS node
 Author-email: Filedgr <code@filedgr.com>
 Project-URL: repository, https://github.com/Filedgr/filedgr-python-lib-ipfs
 Keywords: filedgr,ipfs,lib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp==3.8.2
-Requires-Dist: aiodns==3.0.0
+Requires-Dist: aiohttp>=3.9.5
+Requires-Dist: aiodns>=3.2.0
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `filedgr-ipfs-libs-0.0.2b4/pyproject.toml` & `filedgr_ipfs_libs-0.1.0b1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "filedgr-ipfs-libs"
-version = "0.0.2-beta.4"
+version = "0.1.0-beta.1"
 requires-python = ">=3.9"
 description = "Python libs to interact with the IPFS node"
 readme = "README.md"
 authors = [{ name = "Filedgr", email = "code@filedgr.com" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["filedgr", "ipfs", "lib"]
 dependencies = [
-    "aiohttp==3.8.2",
-    "aiodns==3.0.0"]
+    "aiohttp>=3.9.5",
+    "aiodns>=3.2.0"]
 
 [project.optional-dependencies]
 build = ["build", "twine"]
 dev = ["black", "bumpver", "isort", "mypy", "pytest", "flake8"]
 
 [project.urls]
 repository = "https://github.com/Filedgr/filedgr-python-lib-ipfs"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 exclude = ["tests*"]
 
 [tool.bumpver]
-current_version = "0.0.1-beta.3"
+current_version = "0.1.0-beta.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `filedgr-ipfs-libs-0.0.2b4/src/filedgr_ipfs_libs.egg-info/PKG-INFO` & `filedgr_ipfs_libs-0.1.0b1/src/filedgr_ipfs_libs.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: filedgr-ipfs-libs
-Version: 0.0.2b4
+Version: 0.1.0b1
 Summary: Python libs to interact with the IPFS node
 Author-email: Filedgr <code@filedgr.com>
 Project-URL: repository, https://github.com/Filedgr/filedgr-python-lib-ipfs
 Keywords: filedgr,ipfs,lib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp==3.8.2
-Requires-Dist: aiodns==3.0.0
+Requires-Dist: aiohttp>=3.9.5
+Requires-Dist: aiodns>=3.2.0
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `filedgr-ipfs-libs-0.0.2b4/src/filedgr_lib_ipfs/ipfs_client.py` & `filedgr_ipfs_libs-0.1.0b1/src/filedgr_lib_ipfs/ipfs_client.py`

 * *Files identical despite different names*

### Comparing `filedgr-ipfs-libs-0.0.2b4/tests/test_ipfs_client.py` & `filedgr_ipfs_libs-0.1.0b1/tests/test_ipfs_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         self.assertIn('Hash', res)
         self.assertIn('Name', res)
         self.assertIn('Size', res)
 
     async def test_add_directory(self):
         res = await self.client.add_directory(path="/Users/ericfalk/ws_filedgr/filedgr-python-lib-ipfs/tests/testdir",
                                               remove_prefix="/Users/ericfalk/ws_filedgr/filedgr-python-lib-ipfs/tests/")
+        result = [entry for entry in res if entry["Name"] == "testdir/testdircontent.txt"]
         print(f"The result of the add file call: {res}")
         self.assertIn('Hash', res)
         self.assertIn('Name', res)
         self.assertIn('Size', res)
 
     async def test_ls_directory(self):
         res = await self.client.ls()
```

