# Comparing `tmp/deposit-1.4.41.tar.gz` & `tmp/deposit-1.4.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deposit-1.4.41.tar", last modified: Wed Feb 28 13:44:30 2024, max compression
+gzip compressed data, was "deposit-1.4.42.tar", last modified: Sun May 26 18:28:50 2024, max compression
```

## Comparing `deposit-1.4.41.tar` & `deposit-1.4.42.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 13:44:30.970775 deposit-1.4.41/
--rw-rw-rw-   0        0        0    35821 2022-11-10 14:20:31.000000 deposit-1.4.41/LICENSE
--rw-rw-rw-   0        0        0     4499 2024-02-28 13:44:30.970775 deposit-1.4.41/PKG-INFO
--rw-rw-rw-   0        0        0     3386 2022-11-10 14:20:31.000000 deposit-1.4.41/README.md
--rw-rw-rw-   0        0        0       97 2022-11-10 14:20:31.000000 deposit-1.4.41/pyproject.toml
--rw-rw-rw-   0        0        0       81 2024-02-28 13:44:30.970775 deposit-1.4.41/setup.cfg
--rw-rw-rw-   0        0        0     1631 2024-02-28 13:21:28.000000 deposit-1.4.41/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-28 13:44:30.808009 deposit-1.4.41/src/
-drwxrwxrwx   0        0        0        0 2024-02-28 13:44:30.823634 deposit-1.4.41/src/deposit/
--rw-rw-rw-   0        0        0      364 2024-02-28 13:23:06.000000 deposit-1.4.41/src/deposit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 13:44:30.892665 deposit-1.4.41/src/deposit/datasource/
--rw-rw-rw-   0        0        0      288 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/datasource/__init__.py
--rw-rw-rw-   0        0        0     1223 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/datasource/abstract_datasource.py
--rw-rw-rw-   0        0        0     9932 2023-02-26 20:42:39.000000 deposit-1.4.41/src/deposit/datasource/abstract_dbsource.py
--rw-rw-rw-   0        0        0     4768 2022-12-09 14:04:33.000000 deposit-1.4.41/src/deposit/datasource/abstract_filesource.py
--rw-rw-rw-   0        0        0    14890 2023-02-26 21:22:41.000000 deposit-1.4.41/src/deposit/datasource/db.py
--rw-rw-rw-   0        0        0    25585 2023-02-26 21:18:12.000000 deposit-1.4.41/src/deposit/datasource/db_rel.py
--rw-rw-rw-   0        0        0     1421 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/datasource/json.py
--rw-rw-rw-   0        0        0      759 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/datasource/memory.py
--rw-rw-rw-   0        0        0     1946 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/datasource/pickle.py
-drwxrwxrwx   0        0        0        0 2024-02-28 13:44:30.908290 deposit-1.4.41/src/deposit/externalsource/
--rw-rw-rw-   0        0        0      217 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/externalsource/__init__.py
--rw-rw-rw-   0        0        0     2094 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/externalsource/abstract_externalsource.py
--rw-rw-rw-   0        0        0     2259 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/externalsource/csv.py
--rw-rw-rw-   0        0        0     5826 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/externalsource/shp.py
--rw-rw-rw-   0        0        0     2924 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/externalsource/xlsx.py
-drwxrwxrwx   0        0        0        0 2024-02-28 13:44:30.908290 deposit-1.4.41/src/deposit/query/
--rw-rw-rw-   0        0        0        0 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/query/__init__.py
--rw-rw-rw-   0        0        0    13702 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/query/parse.py
--rw-rw-rw-   0        0        0    15919 2023-02-07 22:46:23.000000 deposit-1.4.41/src/deposit/query/query.py
-drwxrwxrwx   0        0        0        0 2024-02-28 13:44:30.923922 deposit-1.4.41/src/deposit/store/
--rw-rw-rw-   0        0        0        0 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/store/__init__.py
--rw-rw-rw-   0        0        0      135 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/store/abstract_delement.py
--rw-rw-rw-   0        0        0      841 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/store/abstract_dtype.py
--rw-rw-rw-   0        0        0     7819 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/store/dclass.py
--rw-rw-rw-   0        0        0     1137 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/store/ddatetime.py
--rw-rw-rw-   0        0        0       97 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/store/ddict.py
--rw-rw-rw-   0        0        0     2391 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/store/dgeometry.py
--rw-rw-rw-   0        0        0    18472 2022-11-18 23:17:30.000000 deposit-1.4.41/src/deposit/store/dgraph.py
--rw-rw-rw-   0        0        0    10167 2024-02-28 12:35:45.000000 deposit-1.4.41/src/deposit/store/dobject.py
--rw-rw-rw-   0        0        0     1828 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/store/dresource.py
--rw-rw-rw-   0        0        0    38612 2024-02-28 13:13:12.000000 deposit-1.4.41/src/deposit/store/store.py
-drwxrwxrwx   0        0        0        0 2024-02-28 13:44:30.939531 deposit-1.4.41/src/deposit/utils/
--rw-rw-rw-   0        0        0        0 2022-11-10 14:20:31.000000 deposit-1.4.41/src/deposit/utils/__init__.py
--rw-rw-rw-   0        0        0     8230 2024-02-27 12:04:20.000000 deposit-1.4.41/src/deposit/utils/fnc_files.py
--rw-rw-rw-   0        0        0     4583 2023-01-03 17:14:40.000000 deposit-1.4.41/src/deposit/utils/fnc_geometry.py
--rw-rw-rw-   0        0        0    16545 2022-12-09 14:36:38.000000 deposit-1.4.41/src/deposit/utils/fnc_serialize.py
-drwxrwxrwx   0        0        0        0 2024-02-28 13:44:30.970775 deposit-1.4.41/src/deposit.egg-info/
--rw-rw-rw-   0        0        0     4499 2024-02-28 13:44:30.000000 deposit-1.4.41/src/deposit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1366 2024-02-28 13:44:30.000000 deposit-1.4.41/src/deposit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 13:44:30.000000 deposit-1.4.41/src/deposit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2024-02-28 13:44:30.000000 deposit-1.4.41/src/deposit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-28 13:44:30.000000 deposit-1.4.41/src/deposit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-28 13:44:30.955185 deposit-1.4.41/tests/
--rw-rw-rw-   0        0        0     7521 2022-11-10 14:20:31.000000 deposit-1.4.41/tests/test_query.py
--rw-rw-rw-   0        0        0    17718 2023-02-26 21:19:08.000000 deposit-1.4.41/tests/test_store.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:28:50.775036 deposit-1.4.42/
+-rw-rw-rw-   0        0        0    35821 2022-11-10 14:20:31.000000 deposit-1.4.42/LICENSE
+-rw-rw-rw-   0        0        0     4499 2024-05-26 18:28:50.775036 deposit-1.4.42/PKG-INFO
+-rw-rw-rw-   0        0        0     3386 2022-11-10 14:20:31.000000 deposit-1.4.42/README.md
+-rw-rw-rw-   0        0        0       97 2022-11-10 14:20:31.000000 deposit-1.4.42/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-05-26 18:28:50.775036 deposit-1.4.42/setup.cfg
+-rw-rw-rw-   0        0        0     1976 2024-05-04 22:15:15.000000 deposit-1.4.42/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:28:50.706043 deposit-1.4.42/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:28:50.706043 deposit-1.4.42/src/deposit/
+-rw-rw-rw-   0        0        0      364 2024-05-26 18:03:54.000000 deposit-1.4.42/src/deposit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:28:50.728167 deposit-1.4.42/src/deposit/datasource/
+-rw-rw-rw-   0        0        0      288 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/datasource/__init__.py
+-rw-rw-rw-   0        0        0     1223 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/datasource/abstract_datasource.py
+-rw-rw-rw-   0        0        0     9932 2023-02-26 20:42:39.000000 deposit-1.4.42/src/deposit/datasource/abstract_dbsource.py
+-rw-rw-rw-   0        0        0     4768 2022-12-09 14:04:33.000000 deposit-1.4.42/src/deposit/datasource/abstract_filesource.py
+-rw-rw-rw-   0        0        0    14890 2023-02-26 21:22:41.000000 deposit-1.4.42/src/deposit/datasource/db.py
+-rw-rw-rw-   0        0        0    25585 2023-02-26 21:18:12.000000 deposit-1.4.42/src/deposit/datasource/db_rel.py
+-rw-rw-rw-   0        0        0     1421 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/datasource/json.py
+-rw-rw-rw-   0        0        0      759 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/datasource/memory.py
+-rw-rw-rw-   0        0        0     1946 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/datasource/pickle.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:28:50.743793 deposit-1.4.42/src/deposit/externalsource/
+-rw-rw-rw-   0        0        0      217 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/externalsource/__init__.py
+-rw-rw-rw-   0        0        0     2094 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/externalsource/abstract_externalsource.py
+-rw-rw-rw-   0        0        0     2259 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/externalsource/csv.py
+-rw-rw-rw-   0        0        0     5826 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/externalsource/shp.py
+-rw-rw-rw-   0        0        0     2924 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/externalsource/xlsx.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:28:50.743793 deposit-1.4.42/src/deposit/query/
+-rw-rw-rw-   0        0        0        0 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/query/__init__.py
+-rw-rw-rw-   0        0        0    14781 2024-05-26 18:01:10.000000 deposit-1.4.42/src/deposit/query/parse.py
+-rw-rw-rw-   0        0        0    17226 2024-05-26 18:12:20.000000 deposit-1.4.42/src/deposit/query/query.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:28:50.759415 deposit-1.4.42/src/deposit/store/
+-rw-rw-rw-   0        0        0        0 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/store/__init__.py
+-rw-rw-rw-   0        0        0      135 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/store/abstract_delement.py
+-rw-rw-rw-   0        0        0      841 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/store/abstract_dtype.py
+-rw-rw-rw-   0        0        0     7819 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/store/dclass.py
+-rw-rw-rw-   0        0        0     1137 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/store/ddatetime.py
+-rw-rw-rw-   0        0        0       97 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/store/ddict.py
+-rw-rw-rw-   0        0        0     2391 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/store/dgeometry.py
+-rw-rw-rw-   0        0        0    18983 2024-05-26 18:13:40.000000 deposit-1.4.42/src/deposit/store/dgraph.py
+-rw-rw-rw-   0        0        0    10193 2024-05-26 14:15:48.000000 deposit-1.4.42/src/deposit/store/dobject.py
+-rw-rw-rw-   0        0        0     1828 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/store/dresource.py
+-rw-rw-rw-   0        0        0    39449 2024-05-26 17:52:35.000000 deposit-1.4.42/src/deposit/store/store.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:28:50.775036 deposit-1.4.42/src/deposit/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-10 14:20:31.000000 deposit-1.4.42/src/deposit/utils/__init__.py
+-rw-rw-rw-   0        0        0     8230 2024-02-27 12:04:20.000000 deposit-1.4.42/src/deposit/utils/fnc_files.py
+-rw-rw-rw-   0        0        0     4583 2023-01-03 17:14:40.000000 deposit-1.4.42/src/deposit/utils/fnc_geometry.py
+-rw-rw-rw-   0        0        0    16545 2022-12-09 14:36:38.000000 deposit-1.4.42/src/deposit/utils/fnc_serialize.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:28:50.775036 deposit-1.4.42/src/deposit.egg-info/
+-rw-rw-rw-   0        0        0     4499 2024-05-26 18:28:50.000000 deposit-1.4.42/src/deposit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1366 2024-05-26 18:28:50.000000 deposit-1.4.42/src/deposit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:28:50.000000 deposit-1.4.42/src/deposit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2024-05-26 18:28:50.000000 deposit-1.4.42/src/deposit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 18:28:50.000000 deposit-1.4.42/src/deposit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 18:28:50.775036 deposit-1.4.42/tests/
+-rw-rw-rw-   0        0        0     7521 2022-11-10 14:20:31.000000 deposit-1.4.42/tests/test_query.py
+-rw-rw-rw-   0        0        0    17718 2023-02-26 21:19:08.000000 deposit-1.4.42/tests/test_store.py
```

### Comparing `deposit-1.4.41/LICENSE` & `deposit-1.4.42/LICENSE`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/PKG-INFO` & `deposit-1.4.42/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deposit
-Version: 1.4.41
+Version: 1.4.42
 Summary: Graph database focused on scientific data collection.
 Home-page: https://github.com/demjanp/deposit
 Author: Peter Demján
 Author-email: peter.demjan@gmail.com
 Keywords: database,graph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `deposit-1.4.41/README.md` & `deposit-1.4.42/README.md`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/setup.py` & `deposit-1.4.42/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # -*- coding: utf-8 -*-
 #!/usr/bin/env python
 #
 
 from setuptools import setup, find_packages
 import pathlib
 
+import ast
+import os
+
+def get_version():
+	with open(os.path.join(os.path.dirname(__file__), 'src', 'deposit', '__init__.py')) as f:
+		tree = ast.parse(f.read())
+		for node in tree.body:
+			if isinstance(node, ast.Assign):
+				if node.targets[0].id == 'version_info':
+					return '.'.join(map(str, ast.literal_eval(node.value)))
+
 try:
 	from wheel.bdist_wheel import bdist_wheel as _bdist_wheel
 	class bdist_wheel(_bdist_wheel):
 		def finalize_options(self):
 			_bdist_wheel.finalize_options(self)
 			self.root_is_pure = False
 except ImportError:
@@ -16,15 +27,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
 	name="deposit",
-	version="1.4.41",
+	version=get_version(),
 	description="Graph database focused on scientific data collection.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/demjanp/deposit",
 	author="Peter Demján",
 	author_email="peter.demjan@gmail.com",
 	classifiers=[
```

### Comparing `deposit-1.4.41/src/deposit/datasource/abstract_datasource.py` & `deposit-1.4.42/src/deposit/datasource/abstract_datasource.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/datasource/abstract_dbsource.py` & `deposit-1.4.42/src/deposit/datasource/abstract_dbsource.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/datasource/abstract_filesource.py` & `deposit-1.4.42/src/deposit/datasource/abstract_filesource.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/datasource/db.py` & `deposit-1.4.42/src/deposit/datasource/db.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/datasource/db_rel.py` & `deposit-1.4.42/src/deposit/datasource/db_rel.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/datasource/json.py` & `deposit-1.4.42/src/deposit/datasource/json.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/datasource/memory.py` & `deposit-1.4.42/src/deposit/datasource/memory.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/datasource/pickle.py` & `deposit-1.4.42/src/deposit/datasource/pickle.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/externalsource/abstract_externalsource.py` & `deposit-1.4.42/src/deposit/externalsource/abstract_externalsource.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/externalsource/csv.py` & `deposit-1.4.42/src/deposit/externalsource/csv.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/externalsource/shp.py` & `deposit-1.4.42/src/deposit/externalsource/shp.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/externalsource/xlsx.py` & `deposit-1.4.42/src/deposit/externalsource/xlsx.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/query/parse.py` & `deposit-1.4.42/src/deposit/query/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,16 +65,20 @@
 	
 	bracketed = {}
 	done = {}
 	
 	substr_cleaned = substr
 	names = []  # [[i, j, text, is_bracketed], ...]
 	
+	where_index = substr_cleaned.find("WHERE")
+	
 	for m in re.finditer(r"OBJ+\(.*?\)", substr_cleaned):
 		i, j = m.start(0), m.end(0)
+		if i > where_index:
+			continue
 		ids = [id_.strip() for id_ in substr_cleaned[i+4:j-1].split(",")]
 		if not False in [id_.isdigit() for id_ in ids]:
 			names.append([i, j, tuple([int(id_) for id_ in ids]), True])
 			substr_cleaned = substr_cleaned[:i] + (j-i)*" " + substr_cleaned[j:]
 			substr_cleaned = process_found(substr_cleaned, i, j, names)
 	
 	for clsname in sorted(list(classes), key = lambda name: len(name))[::-1]:
@@ -269,28 +273,29 @@
 	tree = ast.parse(substr)
 	# find and replace Class.Descriptor occurences in substr
 	transformer = SelectsToVarsTransformer1(substr, classes.union(classless), descriptors, bracketed_selects)
 	tree = transformer.visit(tree)
 	# find and replace Class occurences in substr
 	transformer = SelectsToVarsTransformer2(substr, classes.union(classless), descriptors, bracketed_selects)
 	tree = transformer.visit(tree)
+	
 	expr = ast.unparse(tree)
 	vars = transformer.selects.copy()
 	
 	for name in vars:
 		if vars[name][0] in classless:
 			cls, descr = vars[name]
 			vars[name] = ("!*", descr)
 	
 	return expr, vars
 
 
 class Parse(object):
 	
-	KEYWORDS = ["SELECT", "COUNT", "SUM", "AS", "RELATED", "WHERE", "GROUP BY"]
+	KEYWORDS = ["SELECT", "COUNT", "SUM", "AS", "WHERE", "GROUP BY"]
 
 	def __init__(self, querystr, classes, descriptors):
 		# classes = {name, ...}
 		# descriptors = {name, ...}
 		# querystr = "SELECT [select1], [select2], COUNT([select1]) AS [alias], SUM([select1]) AS [alias], ... RELATED [relation1], [relation2], ... WHERE [conditions expression] GROUP BY [select1], [select2], ..."
 		#	select = Class or Class.Descriptor
 		#	relation = Class1.Relation.Class2
@@ -311,14 +316,37 @@
 		self.where_vars = {}  # {name: (class, descriptor), ...}
 		self.classes_used = []  # [name, ...]
 		
 		querystr, quoted = remove_quoted(self.querystr)
 		querystr, bracketed_selects = remove_bracketed_selects(querystr, self.classes, self.descriptors)
 		querystr, bracketed_other = remove_bracketed_all(querystr)
 		
+		# convert old-style RELATED segments to WHERE RELATED() format
+		relations = []
+		i, j, k = 0, 0, 0
+		for m in re.finditer(r"(?i)\bRELATED\b", querystr):
+			i = m.start(0)
+			j = m.end(0)
+			for keyword in self.KEYWORDS:
+				k = querystr.find(keyword, j)
+				if k != -1:
+					break
+			else:
+				k = len(querystr)
+			substr = querystr[j:k].strip().strip(",").strip()
+			for chain in substr.split(","):
+				chain = chain.strip().split(".")
+				if len(chain) == 3:
+					relations.append(chain)
+		where_txt = None
+		where_found = False
+		if relations:
+			where_txt = "(%s)" % " and ".join(["RELATED(%s, %s, '%s')" % (chain[0], chain[2], chain[1]) for chain in relations])
+			querystr = querystr[:i] + querystr[k:]
+		
 		collect = []
 		for keyword in self.KEYWORDS:
 			for m in re.finditer(r"(?i)\b%s\b" % (keyword), querystr):
 				i, j = m.start(0), m.end(0)
 				collect.append((i, j, keyword))
 		collect = sorted(collect)
 		collect2 = []
@@ -362,36 +390,37 @@
 					alias = alias.strip().strip(",").strip()
 					class_name, descriptor_name, alias = [(item.strip("[]") if item else None) for item in [class_name, descriptor_name, alias]]
 					if keyword == "COUNT":
 						self.counts.append((alias, class_name, descriptor_name))
 					else:
 						self.sums.append((alias, class_name, descriptor_name))
 					self.columns.append((None, alias))
-			
-			elif keyword == "RELATED":
-				for chain in substr.split(","):
-					chain = str_to_key(chain.strip())
-					if len(chain) == 3:
-						relation = []
-						for item in chain:
-							if item in bracketed_other:
-								relation.append(bracketed_other[item])
-								if isinstance(relation[-1], str):
-									relation[-1] = relation[-1].strip("[]")
-							else:
-								relation.append(item.strip("[]"))
-						self.relations.append(tuple(relation))
-			
 			elif keyword == "WHERE":
+				if where_txt:
+					substr = "%s and (%s)" % (where_txt, substr)
+				where_found = True
 				substr = replace_bracketed(substr, bracketed_other)
 				self.where_expr, self.where_vars = extract_expr_vars(substr, self.classes, self.descriptors, bracketed_selects)
 		
+		if where_txt and not where_found:
+			substr = replace_bracketed(where_txt, bracketed_other)
+			self.where_expr, self.where_vars = extract_expr_vars(substr, self.classes, self.descriptors, bracketed_selects)
+		
 		for key in quoted:
 			self.where_expr = self.where_expr.replace(key, quoted[key])
 		
+		# Find the patterns "RELATED(Class1, Class2, Relation)" in self.where_expr and add them to self.relations
+		for m in re.finditer(r"RELATED\((.*?), (.*?), '(.*?)'\)", self.where_expr):
+			class1, class2, _ = m.groups()
+			if class1 in self.where_vars:
+				class1 = self.where_vars[class1][0]
+			if class2 in self.where_vars:
+				class2 = self.where_vars[class2][0]
+			self.relations.append((class1, "*", class2))
+		
 		for class_name, _ in self.selects + self.group_by:
 			if (class_name is not None) and (class_name not in self.classes_used):
 				self.classes_used.append(class_name)
 		for _, class_name, _ in self.counts + self.sums:
 			if (class_name is not None) and (class_name not in self.classes_used):
 				self.classes_used.append(class_name)
 		for class_name1, _, class_name2 in self.relations:
```

### Comparing `deposit-1.4.41/src/deposit/query/query.py` & `deposit-1.4.42/src/deposit/query/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,14 +106,52 @@
 			self._process()
 		except:
 			_, exc_value, _ = sys.exc_info()
 			self._store.callback_error(
 				"QUERY ERROR in \"%s\": %s" % (self.querystr, str(exc_value))
 			)
 	
+	def _obj_func(self, *args):
+		# Function to handle OBJ(*args) in the query
+		# Accepts one or more object ids
+		# Returns a list of objects or None
+		
+		obj_ids = [self._store.get_object(obj_id) for obj_id in args]
+		obj_ids = [obj_id for obj_id in obj_ids if obj_id is not None]
+		return obj_ids
+	
+	def _has_relation(self, elements1, elements2, label, chained=False):
+		# Function to handle _RELATED(elements1, elements2, label, chained) in the query
+		# elements can be a list of Objects or a single Object ID
+		# If chained==True, look for chained relations
+		
+		def _elements_to_objects(elements):
+			objs = elements
+			if isinstance(elements, int):
+				objs = []
+				obj = self._store.get_object(elements)
+				if obj is not None:
+					objs = [obj]
+			return objs
+		
+		def _find_relation(el1, elements2, label, chained):
+			for el2 in elements2:
+				if el1.has_relation(el2, label, chained):
+					return True
+			return False
+		
+		elements1 = _elements_to_objects(elements1)
+		elements2 = _elements_to_objects(elements2)
+		if (not elements1) or (not elements2):
+			return False
+		for el1 in elements1:
+			if _find_relation(el1, elements2, label, chained):
+				return True
+		return False
+	
 	def _process(self):
 		
 		self.hash = []
 		self._rows = []
 		self._columns = []
 		self._column_idxs = {}
 		self._classes = []
@@ -129,15 +167,14 @@
 		selects = []
 		for class_name, descriptor_name in self.parse.selects:
 			if (class_name not in self.parse.classes) and (class_name not in ["*", "!*"]) and (not isinstance(class_name, tuple)):
 				continue
 			if (descriptor_name not in self.parse.descriptors) and (descriptor_name not in [None, "*"]):
 				continue
 			selects.append((class_name, descriptor_name))
-		
 		if not selects:
 			return
 		
 		self._main_class = selects[0][0]
 		
 		keys = set()  # {(class_name, descriptor_name), ...}
 		for class_name, descriptor_name in selects:
@@ -231,14 +268,16 @@
 						if class_name == "!*":
 							class_name = None
 						if (not isinstance(class_name, tuple)) and class_names and (class_name not in class_names):
 							continue
 						value = self._get_descriptor_value(obj_id, class_name, descriptor_name, class_lookup, descr_lookup, obj_if_none = True)
 						if value is not None:
 							values[name] = value
+				values["OBJ"] = self._obj_func
+				values["RELATED"] = self._has_relation
 				if not eval(self.parse.where_expr, values):
 					continue
 			
 			# collect descriptor values according to SELECT, COUNT, SUM
 			data = {}  # {key: value, ...}; key = (class_name, descriptor_name)
 			for obj_id in path:
 				self._objects.add(obj_id)
```

### Comparing `deposit-1.4.41/src/deposit/store/abstract_dtype.py` & `deposit-1.4.42/src/deposit/store/abstract_dtype.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/store/dclass.py` & `deposit-1.4.42/src/deposit/store/dclass.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/store/ddatetime.py` & `deposit-1.4.42/src/deposit/store/ddatetime.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/store/dgeometry.py` & `deposit-1.4.42/src/deposit/store/dgeometry.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/store/dgraph.py` & `deposit-1.4.42/src/deposit/store/dgraph.py`

 * *Files 8% similar despite different names*

```diff
@@ -127,24 +127,39 @@
 		tgt_id = self._GOR_lookup[tgt_id]
 		
 		if not self._GOR.hasEdge(src_id, tgt_id):
 			self._GOR.addEdge(src_id, tgt_id)
 			self._GOR_labels[(src_id, tgt_id)] = {}
 		self._GOR_labels[(src_id, tgt_id)][label] = weight
 	
-	def has_object_relation(self, src_id, tgt_id, label):
+	def has_object_relation(self, src_id, tgt_id, label, chained = False):
 		
 		src_id = self._GOR_lookup[src_id]
 		tgt_id = self._GOR_lookup[tgt_id]
+		done = set()
 		
-		if not self._GOR.hasEdge(src_id, tgt_id):
+		def _has_relation(src_id, tgt_id, label, chained, done):
+			
+			if (src_id, tgt_id) in done:
+				return False
+			done.add((src_id, tgt_id))
+			if self._GOR.hasEdge(src_id, tgt_id):
+				if label == "*":
+					return True
+				if label in self._GOR_labels[(src_id, tgt_id)]:
+					return True
+			if chained:
+				for node_id in self._GOR.iterNeighbors(src_id):
+					if (label != "*") and (label not in self._GOR_labels[(src_id, node_id)]):
+						continue
+					if _has_relation(node_id, tgt_id, label, chained, done):
+						return True
 			return False
-		if label == "*":
-			return True
-		return label in self._GOR_labels[(src_id, tgt_id)]
+		
+		return _has_relation(src_id, tgt_id, label, chained, done)
 	
 	def get_object_relation_weight(self, src_id, tgt_id, label):
 		
 		src_id = self._GOR_lookup[src_id]
 		tgt_id = self._GOR_lookup[tgt_id]
 		
 		if not self._GOR.hasEdge(src_id, tgt_id):
```

### Comparing `deposit-1.4.41/src/deposit/store/dobject.py` & `deposit-1.4.42/src/deposit/store/dobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,19 +262,19 @@
 		obj_id_src, obj_id_tgt, label = self._store._check_inverse_rel(obj_id_src, obj_id_tgt, label)
 		self._store.G.add_object_relation(obj_id_src, obj_id_tgt, label, weight)
 		self._store.G.add_object_relation(obj_id_tgt, obj_id_src, "~" + label, weight)
 		self._store._on_relation_added(label)
 		obj = self._store.G.get_object_data(obj_id_tgt)
 		self._store.callback_changed([self, obj])
 	
-	def has_relation(self, obj_id_tgt, label):
+	def has_relation(self, obj_id_tgt, label, chained = False):
 		
 		if isinstance(obj_id_tgt, DObject):
 			obj_id_tgt = obj_id_tgt.id
-		return self._store.G.has_object_relation(self.id, obj_id_tgt, label)
+		return self._store.G.has_object_relation(self.id, obj_id_tgt, label, chained)
 	
 	def get_relations(self, obj_id_tgt = None):
 		# returns [(DObject, label), ...]
 		
 		if isinstance(obj_id_tgt, DObject):
 			obj_id_tgt = obj_id_tgt.id
```

### Comparing `deposit-1.4.41/src/deposit/store/dresource.py` & `deposit-1.4.42/src/deposit/store/dresource.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/store/store.py` & `deposit-1.4.42/src/deposit/store/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -785,21 +785,32 @@
 			return label[1:]
 		return "~" + label
 	
 	def get_class_connections(self, classes, relations, progress = None):
 		# classes = [class_name, ...]
 		# relations = [(class1, label, class2), ...]
 		
+		def _cls_is_objs(class_name):
+			
+			if isinstance(class_name, str):
+				return False
+			if not isinstance(class_name, tuple):
+				raise Exception("Unexpected Class name: %s" % (str(class_name)))
+			for c_ in list(class_name):
+				if not isinstance(c_, int):
+					raise Exception("Unexpected Class name: %s" % (str(class_name)))
+			return True
+		
 		def _get_class_members(class_name, leave_names = False):
 			
 			if class_name == "*":
 				return set([obj.id for obj in self.get_objects()])
 			if class_name == "!*":
 				return set([obj.id for obj in self.get_objects() if not obj.has_class()])
-			if isinstance(class_name, tuple):
+			if _cls_is_objs(class_name):
 				return set(list(class_name))
 			cls = self.get_class(class_name)
 			if cls is None:
 				return set()
 			if leave_names:
 				return class_name
 			return set([obj.id for obj in cls.get_members()])
@@ -825,15 +836,14 @@
 			clss2 = _get_class_names(cls2)
 			return clss1.intersection(clss2)
 		
 		def _get_paths(
 			obj_id0, cls_lookup, rels, within_cls_rels, 
 			asterisk_rels, classes, connecting, mandatory_classes,
 		):
-			
 			'''
 			Get all paths from obj_id0 to objects from specified classes.
 			1. If classes or relations contains object specifications OBJ(1, ...)
 			require each path to contain one of those objects
 			2. If a cls1.*.cls2 relation is specified, the path must contain an 
 			edge between cls1 and cls2.
 			3. The paths cannot have within-class edges unless explicitly
@@ -851,14 +861,21 @@
 				if not mandatory_classes:
 					rule1 = True
 				if (len(found_classes) < len(classes)) or within_cls_rels:
 					
 					src = path[-1]
 					clss_src = cls_lookup.get(src, None)
 					
+					# check if source is from connecting set
+					src_within_cls_rels = None
+					if clss_src is not None:
+						common = clss_src.intersection(within_cls_rels.keys())
+						if common:
+							src_within_cls_rels = within_cls_rels[common.pop()]
+					
 					# rule 1 - first stage, source
 					if (not rule1) and (clss_src is not None) and \
 						clss_src.intersection(mandatory_classes):
 							rule1 = True
 					
 					for tgt, label in self.G.iter_object_relations(src):
 						
@@ -895,15 +912,17 @@
 							common = found_classes_.intersection(clss_tgt)
 							if common:
 								if (not rule3) and (clss_src is not None):
 									for cls in clss_src:
 										if (cls in within_cls_rels) and (within_cls_rels[cls].intersection([label, "*"])):
 											rule3 = True
 											break
-								continue
+								if not (src_within_cls_rels and ((label in src_within_cls_rels) or ('*' in src_within_cls_rels)) and clss_tgt.intersection(clss_src)):
+									# within-class relation not allowed
+									continue
 						
 						# rule 1 - first stage, target
 						if clss_tgt is not None:
 							if (not rule1) and clss_tgt.intersection(mandatory_classes):
 								rule1 = True
 						
 						# rule 4
@@ -960,17 +979,17 @@
 		
 		rels = defaultdict(set)  # {(class1, class2): set(label, ...), ...}
 		within_cls_rels = defaultdict(set)  # {class: set(label, ...), ...}
 		asterisk_rels = set()  # set((class1, class2), ...)
 		mandatory_classes = set() # set(class, ...)
 		for cls1, lbl, cls2 in relations:
 			if isinstance(cls1, tuple):
-				mandatory_classes.add(cls1)
+				mandatory_classes.add(cls1[0])
 			if isinstance(cls2, tuple):
-				mandatory_classes.add(cls2)
+				mandatory_classes.add(cls2[0])
 			if lbl == "*":
 				asterisk_rels.add((cls1, cls2))
 				asterisk_rels.add((cls2, cls1))
 			clss = _get_within_class_rel(cls1, cls2)
 			if clss:
 				within_cls_rels[cls1].add(lbl)
 			else:
@@ -983,17 +1002,17 @@
 			# no objects found in the first specified class
 			return set()
 		
 		cls_lookup = defaultdict(set)
 		collect = []
 		for cls in classes:
 			if isinstance(cls, tuple):
-				mandatory_classes.add(cls)
+				mandatory_classes.add(cls[0])
 			objs = objects0 if (cls == cls0) else _get_class_members(cls)
-			if objs:
+			if objs and not _cls_is_objs(cls):
 				collect.append(cls)
 				for obj_id in objs:
 					cls_lookup[obj_id].add(cls)
 		classes = collect
 		
 		if (len(classes) == 1) and (classes[0] not in within_cls_rels):
 			# only one class and no within-class relations apply
@@ -1016,15 +1035,15 @@
 		cmax = len(objects0)
 		cnt = 1
 		if progress is not None:
 			progress.update_state(value = 0, maximum = cmax)
 		for obj_id0 in objects0:
 			if (progress is not None) and (cnt % 100 == 0):
 				if progress.cancel_pressed():
-					return []
+					return set()
 				progress.update_state(value = cnt)
 			cnt += 1
 			paths_ = _get_paths(
 				obj_id0, cls_lookup, rels, within_cls_rels, 
 				asterisk_rels, classes, connecting, mandatory_classes,
 			)
 			if paths_:
```

### Comparing `deposit-1.4.41/src/deposit/utils/fnc_files.py` & `deposit-1.4.42/src/deposit/utils/fnc_files.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/utils/fnc_geometry.py` & `deposit-1.4.42/src/deposit/utils/fnc_geometry.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit/utils/fnc_serialize.py` & `deposit-1.4.42/src/deposit/utils/fnc_serialize.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/src/deposit.egg-info/PKG-INFO` & `deposit-1.4.42/src/deposit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deposit
-Version: 1.4.41
+Version: 1.4.42
 Summary: Graph database focused on scientific data collection.
 Home-page: https://github.com/demjanp/deposit
 Author: Peter Demján
 Author-email: peter.demjan@gmail.com
 Keywords: database,graph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `deposit-1.4.41/src/deposit.egg-info/SOURCES.txt` & `deposit-1.4.42/src/deposit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/tests/test_query.py` & `deposit-1.4.42/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `deposit-1.4.41/tests/test_store.py` & `deposit-1.4.42/tests/test_store.py`

 * *Files identical despite different names*

