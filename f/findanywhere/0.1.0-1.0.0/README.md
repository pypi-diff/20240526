# Comparing `tmp/findanywhere-0.1.0.tar.gz` & `tmp/findanywhere-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findanywhere-0.1.0.tar", max compression
+gzip compressed data, was "findanywhere-1.0.0.tar", max compression
```

## Comparing `findanywhere-0.1.0.tar` & `findanywhere-1.0.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1496 2024-05-20 11:00:15.359287 findanywhere-0.1.0/LICENSE
--rw-r--r--   0        0        0     3615 2024-05-20 14:02:02.143535 findanywhere-0.1.0/README.md
--rw-r--r--   0        0        0     1431 2024-05-25 15:59:09.043469 findanywhere-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-08 17:42:21.640505 findanywhere-0.1.0/whereisit/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 17:44:07.424377 findanywhere-0.1.0/whereisit/adapters/__init__.py
--rw-r--r--   0        0        0      187 2024-05-08 19:00:14.593812 findanywhere-0.1.0/whereisit/adapters/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      343 2024-05-09 11:05:38.505078 findanywhere-0.1.0/whereisit/adapters/evaluation/__init__.py
--rw-r--r--   0        0        0      706 2024-05-09 11:05:39.180082 findanywhere-0.1.0/whereisit/adapters/evaluation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5838 2024-05-25 14:18:32.206222 findanywhere-0.1.0/whereisit/adapters/evaluation/__pycache__/string_distance.cpython-311.pyc
--rw-r--r--   0        0        0     3419 2024-05-25 14:18:16.308089 findanywhere-0.1.0/whereisit/adapters/evaluation/string_distance.py
--rw-r--r--   0        0        0      390 2024-05-25 14:18:16.303089 findanywhere-0.1.0/whereisit/adapters/source/__init__.py
--rw-r--r--   0        0        0      759 2024-05-25 14:18:32.157222 findanywhere-0.1.0/whereisit/adapters/source/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5919 2024-05-25 14:18:32.175222 findanywhere-0.1.0/whereisit/adapters/source/__pycache__/tabular.cpython-311.pyc
--rw-r--r--   0        0        0     6095 2024-05-25 14:18:32.158222 findanywhere-0.1.0/whereisit/adapters/source/__pycache__/text.cpython-311.pyc
--rw-r--r--   0        0        0     3421 2024-05-25 14:18:16.297089 findanywhere-0.1.0/whereisit/adapters/source/tabular.py
--rw-r--r--   0        0        0     3731 2024-05-25 14:18:16.314089 findanywhere-0.1.0/whereisit/adapters/source/text.py
--rw-r--r--   0        0        0        0 2024-05-20 10:27:18.968764 findanywhere-0.1.0/whereisit/algorithms/__init__.py
--rw-r--r--   0        0        0      189 2024-05-20 10:29:17.917054 findanywhere-0.1.0/whereisit/algorithms/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3102 2024-05-25 14:09:44.516764 findanywhere-0.1.0/whereisit/algorithms/__pycache__/strings.cpython-311.pyc
--rw-r--r--   0        0        0     1946 2024-05-25 14:09:44.443763 findanywhere-0.1.0/whereisit/algorithms/strings.py
--rw-r--r--   0        0        0        0 2024-05-08 17:44:02.344335 findanywhere-0.1.0/whereisit/ports/__init__.py
--rw-r--r--   0        0        0      184 2024-05-08 19:00:14.617812 findanywhere-0.1.0/whereisit/ports/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3337 2024-05-25 14:18:32.177222 findanywhere-0.1.0/whereisit/ports/__pycache__/evaluation.cpython-311.pyc
--rw-r--r--   0        0        0     3357 2024-05-25 14:18:32.166222 findanywhere-0.1.0/whereisit/ports/__pycache__/source.cpython-311.pyc
--rw-r--r--   0        0        0     2134 2024-05-25 14:08:34.995154 findanywhere-0.1.0/whereisit/ports/evaluation.py
--rw-r--r--   0        0        0     1933 2024-05-25 14:08:35.010154 findanywhere-0.1.0/whereisit/ports/source.py
--rw-r--r--   0        0        0     8109 2024-05-25 14:18:16.263088 findanywhere-0.1.0/whereisit/schema.py
--rw-r--r--   0        0        0      309 2024-05-09 11:51:26.001359 findanywhere-0.1.0/whereisit/scores/__init__.py
--rw-r--r--   0        0        0      661 2024-05-09 11:51:28.651372 findanywhere-0.1.0/whereisit/scores/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2133 2024-05-25 14:18:32.213222 findanywhere-0.1.0/whereisit/scores/__pycache__/deduction.cpython-311.pyc
--rw-r--r--   0        0        0     1333 2024-05-25 14:08:35.005154 findanywhere-0.1.0/whereisit/scores/deduction.py
--rw-r--r--   0        0        0        0 2024-05-08 19:27:30.026829 findanywhere-0.1.0/whereisit/search/__init__.py
--rw-r--r--   0        0        0      185 2024-05-08 19:59:50.195437 findanywhere-0.1.0/whereisit/search/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7946 2024-05-25 14:18:32.215222 findanywhere-0.1.0/whereisit/search/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     3787 2024-05-25 14:18:32.216222 findanywhere-0.1.0/whereisit/search/__pycache__/parallel.cpython-311.pyc
--rw-r--r--   0        0        0     2089 2024-05-25 14:18:32.219222 findanywhere-0.1.0/whereisit/search/__pycache__/sequential.cpython-311.pyc
--rw-r--r--   0        0        0     6048 2024-05-25 13:36:03.229642 findanywhere-0.1.0/whereisit/search/base.py
--rw-r--r--   0        0        0     2393 2024-05-25 14:34:49.736591 findanywhere-0.1.0/whereisit/search/parallel.py
--rw-r--r--   0        0        0     1417 2024-05-25 14:34:48.472580 findanywhere-0.1.0/whereisit/search/sequential.py
--rw-r--r--   0        0        0      984 2024-05-20 10:22:13.755726 findanywhere-0.1.0/whereisit/similarity/__init__.py
--rw-r--r--   0        0        0     1922 2024-05-20 10:22:13.971727 findanywhere-0.1.0/whereisit/similarity/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2547 2024-05-25 14:18:32.207222 findanywhere-0.1.0/whereisit/similarity/__pycache__/common.cpython-311.pyc
--rw-r--r--   0        0        0     5512 2024-05-25 14:18:32.208222 findanywhere-0.1.0/whereisit/similarity/__pycache__/token.cpython-311.pyc
--rw-r--r--   0        0        0     1767 2024-05-25 14:08:34.960154 findanywhere-0.1.0/whereisit/similarity/common.py
--rw-r--r--   0        0        0     3606 2024-05-25 14:09:16.903522 findanywhere-0.1.0/whereisit/similarity/token.py
--rw-r--r--   0        0        0      369 2024-05-19 13:15:07.059802 findanywhere-0.1.0/whereisit/thresholds/__init__.py
--rw-r--r--   0        0        0      712 2024-05-19 13:36:48.952830 findanywhere-0.1.0/whereisit/thresholds/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3294 2024-05-25 14:18:32.220222 findanywhere-0.1.0/whereisit/thresholds/__pycache__/basic.cpython-311.pyc
--rw-r--r--   0        0        0     2164 2024-05-25 14:08:34.965154 findanywhere-0.1.0/whereisit/thresholds/basic.py
--rw-r--r--   0        0        0        0 2024-05-08 17:43:06.743877 findanywhere-0.1.0/whereisit/types/__init__.py
--rw-r--r--   0        0        0      184 2024-05-08 19:00:14.644813 findanywhere-0.1.0/whereisit/types/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1178 2024-05-25 14:18:32.167222 findanywhere-0.1.0/whereisit/types/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     7465 2024-05-25 14:18:32.168222 findanywhere-0.1.0/whereisit/types/__pycache__/factory.cpython-311.pyc
--rw-r--r--   0        0        0     4722 2024-05-25 14:18:32.177222 findanywhere-0.1.0/whereisit/types/__pycache__/input_data.cpython-311.pyc
--rw-r--r--   0        0        0     4909 2024-05-25 14:18:32.179222 findanywhere-0.1.0/whereisit/types/__pycache__/similarity.cpython-311.pyc
--rw-r--r--   0        0        0      568 2024-05-25 14:08:35.015154 findanywhere-0.1.0/whereisit/types/entry.py
--rw-r--r--   0        0        0     4416 2024-05-25 14:08:34.955154 findanywhere-0.1.0/whereisit/types/factory.py
--rw-r--r--   0        0        0     2833 2024-05-25 14:08:34.936154 findanywhere-0.1.0/whereisit/types/input_data.py
--rw-r--r--   0        0        0     2675 2024-05-25 14:08:35.023154 findanywhere-0.1.0/whereisit/types/similarity.py
--rw-r--r--   0        0        0        0 2024-05-09 10:19:42.473640 findanywhere-0.1.0/whereisit/ui/__init__.py
--rw-r--r--   0        0        0      181 2024-05-09 10:57:56.733493 findanywhere-0.1.0/whereisit/ui/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3867 2024-05-25 14:18:32.271223 findanywhere-0.1.0/whereisit/ui/__pycache__/console.cpython-311.pyc
--rw-r--r--   0        0        0     2011 2024-05-25 14:18:16.276089 findanywhere-0.1.0/whereisit/ui/console.py
--rw-r--r--   0        0        0     4817 1970-01-01 00:00:00.000000 findanywhere-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1496 2024-05-20 11:00:15.359287 findanywhere-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3621 2024-05-26 12:35:41.100676 findanywhere-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 17:42:21.640505 findanywhere-1.0.0/findanywhere/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:44:07.424377 findanywhere-1.0.0/findanywhere/adapters/__init__.py
+-rw-r--r--   0        0        0      187 2024-05-08 19:00:14.593812 findanywhere-1.0.0/findanywhere/adapters/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      352 2024-05-26 12:35:41.108676 findanywhere-1.0.0/findanywhere/adapters/evaluation/__init__.py
+-rw-r--r--   0        0        0      718 2024-05-26 12:35:41.415679 findanywhere-1.0.0/findanywhere/adapters/evaluation/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5856 2024-05-26 12:35:41.416679 findanywhere-1.0.0/findanywhere/adapters/evaluation/__pycache__/string_distance.cpython-311.pyc
+-rw-r--r--   0        0        0     3434 2024-05-26 12:35:41.147677 findanywhere-1.0.0/findanywhere/adapters/evaluation/string_distance.py
+-rw-r--r--   0        0        0      402 2024-05-26 12:35:41.054676 findanywhere-1.0.0/findanywhere/adapters/source/__init__.py
+-rw-r--r--   0        0        0      774 2024-05-26 12:35:41.377679 findanywhere-1.0.0/findanywhere/adapters/source/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5931 2024-05-26 12:35:41.391679 findanywhere-1.0.0/findanywhere/adapters/source/__pycache__/tabular.cpython-311.pyc
+-rw-r--r--   0        0        0     6107 2024-05-26 12:35:41.377679 findanywhere-1.0.0/findanywhere/adapters/source/__pycache__/text.cpython-311.pyc
+-rw-r--r--   0        0        0     3430 2024-05-26 12:35:41.125676 findanywhere-1.0.0/findanywhere/adapters/source/tabular.py
+-rw-r--r--   0        0        0     3740 2024-05-26 12:35:41.088676 findanywhere-1.0.0/findanywhere/adapters/source/text.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:27:18.968764 findanywhere-1.0.0/findanywhere/algorithms/__init__.py
+-rw-r--r--   0        0        0      189 2024-05-20 10:29:17.917054 findanywhere-1.0.0/findanywhere/algorithms/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3102 2024-05-25 14:09:44.516764 findanywhere-1.0.0/findanywhere/algorithms/__pycache__/strings.cpython-311.pyc
+-rw-r--r--   0        0        0     1946 2024-05-25 14:09:44.443763 findanywhere-1.0.0/findanywhere/algorithms/strings.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:44:02.344335 findanywhere-1.0.0/findanywhere/ports/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-08 19:00:14.617812 findanywhere-1.0.0/findanywhere/ports/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3349 2024-05-26 12:35:41.392679 findanywhere-1.0.0/findanywhere/ports/__pycache__/evaluation.cpython-311.pyc
+-rw-r--r--   0        0        0     3366 2024-05-26 12:35:41.384679 findanywhere-1.0.0/findanywhere/ports/__pycache__/source.cpython-311.pyc
+-rw-r--r--   0        0        0     2143 2024-05-26 12:35:41.133676 findanywhere-1.0.0/findanywhere/ports/evaluation.py
+-rw-r--r--   0        0        0     1939 2024-05-26 12:35:41.084676 findanywhere-1.0.0/findanywhere/ports/source.py
+-rw-r--r--   0        0        0     8133 2024-05-26 12:35:41.120676 findanywhere-1.0.0/findanywhere/schema.py
+-rw-r--r--   0        0        0      318 2024-05-26 12:35:41.097676 findanywhere-1.0.0/findanywhere/scores/__init__.py
+-rw-r--r--   0        0        0      673 2024-05-26 12:35:41.426679 findanywhere-1.0.0/findanywhere/scores/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2148 2024-05-26 12:35:41.426679 findanywhere-1.0.0/findanywhere/scores/__pycache__/deduction.cpython-311.pyc
+-rw-r--r--   0        0        0     1345 2024-05-26 12:35:41.137677 findanywhere-1.0.0/findanywhere/scores/deduction.py
+-rw-r--r--   0        0        0        0 2024-05-08 19:27:30.026829 findanywhere-1.0.0/findanywhere/search/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-08 19:59:50.195437 findanywhere-1.0.0/findanywhere/search/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7961 2024-05-26 12:35:41.427679 findanywhere-1.0.0/findanywhere/search/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     3804 2024-05-26 12:35:41.428679 findanywhere-1.0.0/findanywhere/search/__pycache__/parallel.cpython-311.pyc
+-rw-r--r--   0        0        0     2103 2024-05-26 12:35:41.431679 findanywhere-1.0.0/findanywhere/search/__pycache__/sequential.cpython-311.pyc
+-rw-r--r--   0        0        0     6060 2024-05-26 12:35:41.079676 findanywhere-1.0.0/findanywhere/search/base.py
+-rw-r--r--   0        0        0     2405 2024-05-26 12:35:41.163677 findanywhere-1.0.0/findanywhere/search/parallel.py
+-rw-r--r--   0        0        0     1426 2024-05-26 12:35:41.159677 findanywhere-1.0.0/findanywhere/search/sequential.py
+-rw-r--r--   0        0        0      996 2024-05-26 12:35:41.062676 findanywhere-1.0.0/findanywhere/similarity/__init__.py
+-rw-r--r--   0        0        0     1937 2024-05-26 12:35:41.416679 findanywhere-1.0.0/findanywhere/similarity/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2556 2024-05-26 12:35:41.417679 findanywhere-1.0.0/findanywhere/similarity/__pycache__/common.cpython-311.pyc
+-rw-r--r--   0        0        0     5524 2024-05-26 12:35:41.418679 findanywhere-1.0.0/findanywhere/similarity/__pycache__/token.cpython-311.pyc
+-rw-r--r--   0        0        0     1773 2024-05-26 12:35:41.039676 findanywhere-1.0.0/findanywhere/similarity/common.py
+-rw-r--r--   0        0        0     3615 2024-05-26 12:35:41.071676 findanywhere-1.0.0/findanywhere/similarity/token.py
+-rw-r--r--   0        0        0      378 2024-05-26 12:35:41.143677 findanywhere-1.0.0/findanywhere/thresholds/__init__.py
+-rw-r--r--   0        0        0      724 2024-05-26 12:35:41.431679 findanywhere-1.0.0/findanywhere/thresholds/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3306 2024-05-26 12:35:41.432679 findanywhere-1.0.0/findanywhere/thresholds/__pycache__/basic.cpython-311.pyc
+-rw-r--r--   0        0        0     2173 2024-05-26 12:35:41.044676 findanywhere-1.0.0/findanywhere/thresholds/basic.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:43:06.743877 findanywhere-1.0.0/findanywhere/types/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-08 19:00:14.644813 findanywhere-1.0.0/findanywhere/types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1178 2024-05-25 14:18:32.167222 findanywhere-1.0.0/findanywhere/types/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     7465 2024-05-25 14:18:32.168222 findanywhere-1.0.0/findanywhere/types/__pycache__/factory.cpython-311.pyc
+-rw-r--r--   0        0        0     4722 2024-05-25 14:18:32.177222 findanywhere-1.0.0/findanywhere/types/__pycache__/input_data.cpython-311.pyc
+-rw-r--r--   0        0        0     4918 2024-05-26 12:35:41.393679 findanywhere-1.0.0/findanywhere/types/__pycache__/similarity.cpython-311.pyc
+-rw-r--r--   0        0        0      568 2024-05-25 14:08:35.015154 findanywhere-1.0.0/findanywhere/types/entry.py
+-rw-r--r--   0        0        0     4416 2024-05-25 14:08:34.955154 findanywhere-1.0.0/findanywhere/types/factory.py
+-rw-r--r--   0        0        0     2833 2024-05-25 14:08:34.936154 findanywhere-1.0.0/findanywhere/types/input_data.py
+-rw-r--r--   0        0        0     2681 2024-05-26 12:35:41.172677 findanywhere-1.0.0/findanywhere/types/similarity.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:19:42.473640 findanywhere-1.0.0/findanywhere/ui/__init__.py
+-rw-r--r--   0        0        0      181 2024-05-09 10:57:56.733493 findanywhere-1.0.0/findanywhere/ui/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3888 2024-05-26 12:35:41.473680 findanywhere-1.0.0/findanywhere/ui/__pycache__/console.cpython-311.pyc
+-rw-r--r--   0        0        0     2029 2024-05-26 12:35:41.116676 findanywhere-1.0.0/findanywhere/ui/console.py
+-rw-r--r--   0        0        0     1490 2024-05-26 12:42:48.297992 findanywhere-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4829 1970-01-01 00:00:00.000000 findanywhere-1.0.0/PKG-INFO
```

### Comparing `findanywhere-0.1.0/LICENSE` & `findanywhere-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `findanywhere-0.1.0/README.md` & `findanywhere-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -67,25 +67,25 @@
     constant: 0.9
   name: constant
 ````
 
 Run the tool against your datasets using the defined schema:
 
 ````shell
-whereisit schema.yml search_data.json garbage.csv --out result.json_line
+findanywhere schema.yml search_data.json garbage.csv --out result.json_line
 ````
 
 Results will be stored in result.json_line. For additional commands and options, use the --help flag.
 
 ## Installation
 
 Install **WhereIsIt** easily using pip:
 
 ````shell
-pip install whereisit
+pip install findanywhere
 ````
 
 
 ## Key Features
 
 - **Robust Malformed File Handling:** Efficiently processes CSV files with irregular column structures or misplaced data entries.
 - **Fuzzy Matching Capabilities:** Utilizes advanced algorithms to match data points based on similarity, accommodating various types of data discrepancies.
```

### Comparing `findanywhere-0.1.0/pyproject.toml` & `findanywhere-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [tool.poetry]
 name = "findanywhere"
-version = "0.1.0"
+version = "1.0.0"
 description = ""
 authors = ["voidpointercast <voidpointercast@justmail.de>"]
 classifiers = [
     "Development Status :: 4 - Beta", "Environment :: Console", "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License", "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows :: Windows 11", "Topic :: Scientific/Engineering :: Information Analysis",
     "Programming Language :: Python :: 3.11", "Programming Language :: Python :: 3.12"
 ]
 license = "BSD License (BSD)"
 readme = "README.md"
 documentation = "https://whereisit.readthedocs.io/en/latest/"
-repository = "https://gitlab.com/patrick.daniel.gress/whereisit"
-homepage = "https://gitlab.com/patrick.daniel.gress/whereisit"
+repository = "https://gitlab.com/patrick.daniel.gress/findanywhere"
+homepage = "https://gitlab.com/patrick.daniel.gress/findanywhere"
 keywords = ["search", "fuzzy_search", "preprocessing"]
-packages = [{include = "whereisit"}]
 
 
 [tool.poetry.scripts]
 whereisit = "whereisit.ui.console:main"
 whereisit_schema = "whereisit.schema:main"
+findanywhere = "whereisit.ui.console:main"
+findanywhere_schema = "whereisit.schema:main"
+
 
 [tool.poetry.dependencies]
 python = "^3.11"
 toolz = "^0.12.1"
 jellyfish = "^1.0.3"
 dacite = "^1.8.1"
 pyyaml = "^6.0.1"
```

### Comparing `findanywhere-0.1.0/whereisit/adapters/evaluation/__pycache__/string_distance.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/adapters/evaluation/__pycache__/string_distance.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x28f35166 (Sat May 25 14:18:16 2024 UTC)
-files sz: 3419
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 3434
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
       0x97005500640064016c006d015a016d025a020100640064026c036d045a
@@ -81,57 +81,57 @@
                 92 IMPORT_NAME             15 (jellyfish)
                 94 IMPORT_FROM             16 (jaro_winkler_similarity)
                 96 STORE_NAME              16 (jaro_winkler_similarity)
                 98 POP_TOP
    
     10         100 LOAD_CONST               0 (0)
                102 LOAD_CONST               8 (('InputData', 'Evaluation', 'ScoredEntry', 'get_best_with', 'EvaluationAdapter'))
-               104 IMPORT_NAME             17 (whereisit.ports.evaluation)
+               104 IMPORT_NAME             17 (findanywhere.ports.evaluation)
                106 IMPORT_FROM             18 (InputData)
                108 STORE_NAME              18 (InputData)
                110 IMPORT_FROM             19 (Evaluation)
                112 STORE_NAME              19 (Evaluation)
                114 IMPORT_FROM             20 (ScoredEntry)
                116 STORE_NAME              20 (ScoredEntry)
                118 IMPORT_FROM             21 (get_best_with)
                120 STORE_NAME              21 (get_best_with)
                122 IMPORT_FROM             22 (EvaluationAdapter)
                124 STORE_NAME              22 (EvaluationAdapter)
                126 POP_TOP
    
     11         128 LOAD_CONST               0 (0)
                130 LOAD_CONST               9 (('Position', 'Entry'))
-               132 IMPORT_NAME             23 (whereisit.ports.source)
+               132 IMPORT_NAME             23 (findanywhere.ports.source)
                134 IMPORT_FROM             24 (Position)
                136 STORE_NAME              24 (Position)
                138 IMPORT_FROM             25 (Entry)
                140 STORE_NAME              25 (Entry)
                142 POP_TOP
    
     12         144 LOAD_CONST               0 (0)
                146 LOAD_CONST              10 (('get_similarity_factory', 'get_aggregate_by_name'))
-               148 IMPORT_NAME             26 (whereisit.similarity)
+               148 IMPORT_NAME             26 (findanywhere.similarity)
                150 IMPORT_FROM             27 (get_similarity_factory)
                152 STORE_NAME              27 (get_similarity_factory)
                154 IMPORT_FROM             28 (get_aggregate_by_name)
                156 STORE_NAME              28 (get_aggregate_by_name)
                158 POP_TOP
    
     13         160 LOAD_CONST               0 (0)
                162 LOAD_CONST              11 (('as_factory', 'Config'))
-               164 IMPORT_NAME             29 (whereisit.types.factory)
+               164 IMPORT_NAME             29 (findanywhere.types.factory)
                166 IMPORT_FROM             30 (as_factory)
                168 STORE_NAME              30 (as_factory)
                170 IMPORT_FROM             31 (Config)
                172 STORE_NAME              31 (Config)
                174 POP_TOP
    
     14         176 LOAD_CONST               0 (0)
                178 LOAD_CONST              12 (('Similarity',))
-               180 IMPORT_NAME             32 (whereisit.types.similarity)
+               180 IMPORT_NAME             32 (findanywhere.types.similarity)
                182 IMPORT_FROM             33 (Similarity)
                184 STORE_NAME              33 (Similarity)
                186 POP_TOP
    
     17         188 LOAD_CONST              13 ('similarity')
    
     18         190 LOAD_NAME               33 (Similarity)
@@ -178,15 +178,15 @@
     22         314 LOAD_NAME               19 (Evaluation)
                316 LOAD_NAME               24 (Position)
                318 LOAD_NAME               34 (str)
                320 BUILD_TUPLE              2
                322 BINARY_SUBSCR
    
     17         332 BUILD_TUPLE             10
-               334 LOAD_CONST              18 (<code object evaluate_by_similarity, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/evaluation/string_distance.py", line 17>)
+               334 LOAD_CONST              18 (<code object evaluate_by_similarity, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/evaluation/string_distance.py", line 17>)
                336 MAKE_FUNCTION            4 (annotations)
                338 STORE_NAME              36 (evaluate_by_similarity)
    
     46         340 PUSH_NULL
                342 LOAD_NAME                7 (partial)
    
     47         344 LOAD_NAME               36 (evaluate_by_similarity)
@@ -208,15 +208,15 @@
                392 LOAD_CONST              20 (True)
                394 KW_NAMES                21
                396 PRECALL                  1
                400 CALL                     1
    
     51         410 PUSH_NULL
                412 LOAD_BUILD_CLASS
-               414 LOAD_CONST              22 (<code object StringBasedEvaluationConfig, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/evaluation/string_distance.py", line 50>)
+               414 LOAD_CONST              22 (<code object StringBasedEvaluationConfig, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/evaluation/string_distance.py", line 50>)
                416 MAKE_FUNCTION            0
                418 LOAD_CONST              23 ('StringBasedEvaluationConfig')
                420 LOAD_NAME               31 (Config)
                422 PRECALL                  3
                426 CALL                     3
    
     50         436 PRECALL                  0
@@ -235,15 +235,15 @@
     69         476 LOAD_CONST              26 ('config')
                478 LOAD_NAME               40 (StringBasedEvaluationConfig)
                480 LOAD_CONST              17 ('return')
                482 LOAD_NAME               22 (EvaluationAdapter)
                484 LOAD_NAME               34 (str)
                486 BINARY_SUBSCR
                496 BUILD_TUPLE              4
-               498 LOAD_CONST              27 (<code object evaluate_by_similarity_using, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/evaluation/string_distance.py", line 68>)
+               498 LOAD_CONST              27 (<code object evaluate_by_similarity_using, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/evaluation/string_distance.py", line 68>)
                500 MAKE_FUNCTION            4 (annotations)
    
     68         502 PRECALL                  0
                506 CALL                     0
    
     69         516 STORE_NAME              41 (evaluate_by_similarity_using)
                518 LOAD_CONST              28 (None)
@@ -289,15 +289,15 @@
          
           17           4 RESUME                   0
          
           36           6 LOAD_GLOBAL              1 (NULL + sorted)
          
           37          18 LOAD_CLOSURE             0 (similarity)
                       20 BUILD_TUPLE              1
-                      22 LOAD_CONST               1 (<code object <genexpr>, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/evaluation/string_distance.py", line 37>)
+                      22 LOAD_CONST               1 (<code object <genexpr>, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/evaluation/string_distance.py", line 37>)
                       24 MAKE_FUNCTION            8 (closure)
          
           39          26 LOAD_GLOBAL              3 (NULL + product)
                       38 LOAD_FAST                2 (reference)
                       40 LOAD_ATTR                2 (fields)
                       50 LOAD_METHOD              3 (items)
                       72 PRECALL                  0
@@ -322,15 +322,15 @@
          
           41         164 LOAD_GLOBAL             11 (NULL + Evaluation)
                      176 LOAD_FAST                2 (reference)
                      178 LOAD_ATTR                6 (id)
                      188 LOAD_GLOBAL             15 (NULL + dict)
                      200 LOAD_CLOSURE             1 (aggregate)
                      202 BUILD_TUPLE              1
-                     204 LOAD_CONST               4 (<code object <genexpr>, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/evaluation/string_distance.py", line 41>)
+                     204 LOAD_CONST               4 (<code object <genexpr>, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/evaluation/string_distance.py", line 41>)
                      206 MAKE_FUNCTION            8 (closure)
          
           43         208 LOAD_GLOBAL             17 (NULL + groupby)
                      220 LOAD_FAST                4 (scores)
                      222 LOAD_GLOBAL              9 (NULL + itemgetter)
                      234 LOAD_CONST               2 (0)
                      236 PRECALL                  1
@@ -399,15 +399,15 @@
                            122 RETURN_VALUE
                consts
                   None
                names      ('ScoredEntry', 'position', 'value')
                varnames   ('.0', 'field_', 'value', 'entry')
                freevars   ('similarity',)
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/evaluation/string_distance.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/evaluation/string_distance.py'
                name       '<genexpr>'
                firstlineno 37
                lnotab 0x0c020eff56ff
             0
             ('key',)
             code
                argcount  : 1
@@ -455,23 +455,23 @@
                consts
                   1
                   None
                names      ('get_best_with', 'map', 'itemgetter')
                varnames   ('.0', 'field_', 'field_scores')
                freevars   ('aggregate',)
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/evaluation/string_distance.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/evaluation/string_distance.py'
                name       '<genexpr>'
                firstlineno 41
                lnotab 0x0c0160ff
          names      ('sorted', 'product', 'fields', 'items', 'itemgetter', 'Evaluation', 'id', 'dict', 'groupby')
          varnames   ('similarity', 'aggregate', 'reference', 'entries', 'scores')
          freevars   ()
          cellvars   ('similarity', 'aggregate')
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/evaluation/string_distance.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/evaluation/string_distance.py'
          name       'evaluate_by_similarity'
          firstlineno 17
          lnotab 0x06130c0108024cfe10021cfd12052c023afe
       'evaluate_by_similarity_default'
       True
       ('frozen',)
       code
@@ -535,15 +535,15 @@
             'max'
             'aggregate'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'similarity', 'str', '__annotations__', 'field', 'dict', 'similarity_parameter', 'Any', 'aggregate')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/evaluation/string_distance.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/evaluation/string_distance.py'
          name       'StringBasedEvaluationConfig'
          firstlineno 50
          lnotab 0x0c02040c0e013201
       'StringBasedEvaluationConfig'
       'string_based_evaluation'
       ('using',)
       'config'
@@ -598,23 +598,23 @@
                      216 RETURN_VALUE
          consts
             '\n    Evaluates similarity using a given configuration.\n\n    Args:\n        config: The configuration for the string-based evaluation.\n\n    Returns:\n        An EvaluationAdapter that can be used to evaluate similarity.\n\n    '
          names      ('partial', 'evaluate_by_similarity', 'get_similarity_factory', 'str', 'similarity', 'from_dict', 'similarity_parameter', 'get_aggregate_by_name', 'aggregate')
          varnames   ('config',)
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/evaluation/string_distance.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/evaluation/string_distance.py'
          name       'evaluate_by_similarity_using'
          firstlineno 68
          lnotab 0x020c0c010c010c0126ff0e02300140fb
       None
-   names      ('collections.abc', 'Sequence', 'Callable', 'dataclasses', 'dataclass', 'field', 'functools', 'partial', 'itertools', 'product', 'groupby', 'operator', 'itemgetter', 'typing', 'Any', 'jellyfish', 'jaro_winkler_similarity', 'whereisit.ports.evaluation', 'InputData', 'Evaluation', 'ScoredEntry', 'get_best_with', 'EvaluationAdapter', 'whereisit.ports.source', 'Position', 'Entry', 'whereisit.similarity', 'get_similarity_factory', 'get_aggregate_by_name', 'whereisit.types.factory', 'as_factory', 'Config', 'whereisit.types.similarity', 'Similarity', 'str', 'float', 'evaluate_by_similarity', 'max', 'evaluate_by_similarity_default', '__annotations__', 'StringBasedEvaluationConfig', 'evaluate_by_similarity_using')
+   names      ('collections.abc', 'Sequence', 'Callable', 'dataclasses', 'dataclass', 'field', 'functools', 'partial', 'itertools', 'product', 'groupby', 'operator', 'itemgetter', 'typing', 'Any', 'jellyfish', 'jaro_winkler_similarity', 'findanywhere.ports.evaluation', 'InputData', 'Evaluation', 'ScoredEntry', 'get_best_with', 'EvaluationAdapter', 'findanywhere.ports.source', 'Position', 'Entry', 'findanywhere.similarity', 'get_similarity_factory', 'get_aggregate_by_name', 'findanywhere.types.factory', 'as_factory', 'Config', 'findanywhere.types.similarity', 'Similarity', 'str', 'float', 'evaluate_by_similarity', 'max', 'evaluate_by_similarity_default', '__annotations__', 'StringBasedEvaluationConfig', 'evaluate_by_similarity_using')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/evaluation/string_distance.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/evaluation/string_distance.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201120110010c0110010c010c020c021c011001100110010c0302
       0128ff020220fe02030efd02041efc020512fb081d040106ff260416011a
       ff0e01021118011aff0e01
```

### Comparing `findanywhere-0.1.0/whereisit/adapters/evaluation/string_distance.py` & `findanywhere-1.0.0/findanywhere/adapters/evaluation/string_distance.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from functools import partial
 from itertools import product, groupby
 from operator import itemgetter
 from typing import Any
 
 from jellyfish import jaro_winkler_similarity
 
-from whereisit.ports.evaluation import InputData, Evaluation, ScoredEntry, get_best_with, EvaluationAdapter
-from whereisit.ports.source import Position, Entry
-from whereisit.similarity import get_similarity_factory, get_aggregate_by_name
-from whereisit.types.factory import as_factory, Config
-from whereisit.types.similarity import Similarity
+from findanywhere.ports.evaluation import InputData, Evaluation, ScoredEntry, get_best_with, EvaluationAdapter
+from findanywhere.ports.source import Position, Entry
+from findanywhere.similarity import get_similarity_factory, get_aggregate_by_name
+from findanywhere.types.factory import as_factory, Config
+from findanywhere.types.similarity import Similarity
 
 
 def evaluate_by_similarity(
         similarity: Similarity[str] | Callable[[str, str], float],
         aggregate: Callable[[Sequence[float]], float],
         reference: InputData[str],
         entries: Sequence[Entry[Position, str]]
```

### Comparing `findanywhere-0.1.0/whereisit/adapters/source/__pycache__/tabular.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/adapters/source/__pycache__/tabular.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x28f35166 (Sat May 25 14:18:16 2024 UTC)
-files sz: 3421
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 3430
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 14
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -61,45 +61,45 @@
                 58 IMPORT_NAME              9 (pathlib)
                 60 IMPORT_FROM             10 (Path)
                 62 STORE_NAME              10 (Path)
                 64 POP_TOP
    
      7          66 LOAD_CONST               0 (0)
                 68 LOAD_CONST               6 (('SourceAdapter', 'SourceConfig'))
-                70 IMPORT_NAME             11 (whereisit.ports.source)
+                70 IMPORT_NAME             11 (findanywhere.ports.source)
                 72 IMPORT_FROM             12 (SourceAdapter)
                 74 STORE_NAME              12 (SourceAdapter)
                 76 IMPORT_FROM             13 (SourceConfig)
                 78 STORE_NAME              13 (SourceConfig)
                 80 POP_TOP
    
      8          82 LOAD_CONST               0 (0)
                 84 LOAD_CONST               7 (('Entry',))
-                86 IMPORT_NAME             14 (whereisit.types.entry)
+                86 IMPORT_NAME             14 (findanywhere.types.entry)
                 88 IMPORT_FROM             15 (Entry)
                 90 STORE_NAME              15 (Entry)
                 92 POP_TOP
    
      9          94 LOAD_CONST               0 (0)
                 96 LOAD_CONST               8 (('as_factory',))
-                98 IMPORT_NAME             16 (whereisit.types.factory)
+                98 IMPORT_NAME             16 (findanywhere.types.factory)
                100 IMPORT_FROM             17 (as_factory)
                102 STORE_NAME              17 (as_factory)
                104 POP_TOP
    
     12         106 PUSH_NULL
                108 LOAD_NAME                4 (dataclass)
                110 LOAD_CONST               9 (True)
                112 KW_NAMES                10
                114 PRECALL                  1
                118 CALL                     1
    
     13         128 PUSH_NULL
                130 LOAD_BUILD_CLASS
-               132 LOAD_CONST              11 (<code object TablePosition, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py", line 12>)
+               132 LOAD_CONST              11 (<code object TablePosition, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py", line 12>)
                134 MAKE_FUNCTION            0
                136 LOAD_CONST              12 ('TablePosition')
                138 PRECALL                  2
                142 CALL                     2
    
     12         152 PRECALL                  0
                156 CALL                     0
@@ -125,15 +125,15 @@
                228 LOAD_NAME               19 (tuple)
                230 LOAD_NAME               20 (str)
                232 LOAD_NAME               20 (str)
                234 BUILD_TUPLE              2
                236 BINARY_SUBSCR
                246 BINARY_SUBSCR
                256 BUILD_TUPLE              4
-               258 LOAD_CONST              16 (<code object _handle_extra_columns, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py", line 27>)
+               258 LOAD_CONST              16 (<code object _handle_extra_columns, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py", line 27>)
                260 MAKE_FUNCTION            4 (annotations)
                262 STORE_NAME              22 (_handle_extra_columns)
    
     39         264 LOAD_CONST              17 ('encoding')
    
     40         266 LOAD_NAME               20 (str)
    
@@ -158,28 +158,28 @@
                290 LOAD_NAME               20 (str)
                292 BUILD_TUPLE              2
                294 BINARY_SUBSCR
                304 BINARY_SUBSCR
                314 BINARY_SUBSCR
    
     39         324 BUILD_TUPLE             10
-               326 LOAD_CONST              21 (<code object load_tabular_source, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py", line 39>)
+               326 LOAD_CONST              21 (<code object load_tabular_source, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py", line 39>)
                328 MAKE_FUNCTION            4 (annotations)
                330 STORE_NAME              23 (load_tabular_source)
    
     69         332 PUSH_NULL
                334 LOAD_NAME                4 (dataclass)
                336 LOAD_CONST               9 (True)
                338 KW_NAMES                10
                340 PRECALL                  1
                344 CALL                     1
    
     70         354 PUSH_NULL
                356 LOAD_BUILD_CLASS
-               358 LOAD_CONST              22 (<code object TabularSourceConfig, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py", line 69>)
+               358 LOAD_CONST              22 (<code object TabularSourceConfig, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py", line 69>)
                360 MAKE_FUNCTION            0
                362 LOAD_CONST              23 ('TabularSourceConfig')
                364 LOAD_NAME               13 (SourceConfig)
                366 LOAD_NAME               10 (Path)
                368 BINARY_SUBSCR
                378 PRECALL                  3
                382 CALL                     3
@@ -205,15 +205,15 @@
                436 LOAD_NAME               12 (SourceAdapter)
                438 LOAD_NAME               10 (Path)
                440 LOAD_NAME               18 (TablePosition)
                442 LOAD_NAME               20 (str)
                444 BUILD_TUPLE              3
                446 BINARY_SUBSCR
                456 BUILD_TUPLE              4
-               458 LOAD_CONST              26 (<code object load_tabular_source_using, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py", line 88>)
+               458 LOAD_CONST              26 (<code object load_tabular_source_using, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py", line 88>)
                460 MAKE_FUNCTION            4 (annotations)
    
     88         462 PRECALL                  0
                466 CALL                     0
    
     92         476 STORE_NAME              25 (load_tabular_source_using)
                478 LOAD_CONST              14 (None)
@@ -265,15 +265,15 @@
             'line'
             'column'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'int', '__annotations__', 'str')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py'
          name       'TablePosition'
          firstlineno 12
          lnotab 0x0c0204090a01
       'TablePosition'
       'items'
       None
       'return'
@@ -350,15 +350,15 @@
             None
             1
             '_extra_column_'
          names      ('isinstance', 'list', 'str')
          varnames   ('items', 'extra_column_count', 'column', 'value', 'extra_value')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py'
          name       '_handle_extra_columns'
          firstlineno 27
          lnotab 0x060104010e012a01080112010cfe020428fa
       'encoding'
       'errors'
       'delimiter'
       'location'
@@ -412,15 +412,15 @@
                      122 UNPACK_SEQUENCE          2
                      126 STORE_DEREF              7 (line_no)
                      128 STORE_FAST               6 (row)
          
           63         130 LOAD_GLOBAL              7 (NULL + tuple)
                      142 LOAD_CLOSURE             7 (line_no)
                      144 BUILD_TUPLE              1
-                     146 LOAD_CONST               3 (<code object <genexpr>, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py", line 63>)
+                     146 LOAD_CONST               3 (<code object <genexpr>, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py", line 63>)
                      148 MAKE_FUNCTION            8 (closure)
          
           65         150 LOAD_GLOBAL              9 (NULL + _handle_extra_columns)
                      162 LOAD_FAST                6 (row)
                      164 LOAD_METHOD              5 (items)
                      186 PRECALL                  0
                      190 CALL                     0
@@ -513,24 +513,24 @@
                            124 RETURN_VALUE
                consts
                   None
                names      ('Entry', 'TablePosition', 'str')
                varnames   ('.0', 'column', 'value')
                freevars   ('line_no',)
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py'
                name       '<genexpr>'
                firstlineno 63
                lnotab 0x0c0208ff5eff
             None
          names      ('open', 'DictReader', 'enumerate', 'tuple', '_handle_extra_columns', 'items')
          varnames   ('encoding', 'errors', 'delimiter', 'location', 'src', 'reader', 'row')
          freevars   ()
          cellvars   ('line_no',)
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py'
          name       'load_tabular_source'
          firstlineno 39
          lnotab 0x0815300122012801140240fe26ff02fe
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
@@ -574,15 +574,15 @@
           83          58 LOAD_NAME                9 (classmethod)
          
           84          60 LOAD_CONST               8 ('return')
                       62 LOAD_NAME               10 (type)
                       64 LOAD_NAME               11 (Path)
                       66 BINARY_SUBSCR
                       76 BUILD_TUPLE              2
-                      78 LOAD_CONST               9 (<code object location_type, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py", line 83>)
+                      78 LOAD_CONST               9 (<code object location_type, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py", line 83>)
                       80 MAKE_FUNCTION            4 (annotations)
          
           83          82 PRECALL                  0
                       86 CALL                     0
          
           84          96 STORE_NAME              12 (location_type)
                       98 LOAD_CONST              10 (None)
@@ -609,24 +609,24 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('Path',)
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py'
                name       'location_type'
                firstlineno 83
                lnotab 0x0202
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'encoding', 'str', '__annotations__', 'errors', 'delimiter', 'classmethod', 'type', 'Path', 'location_type')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py'
          name       'TabularSourceConfig'
          firstlineno 69
          lnotab 0x0c0204080e010e010e02020116ff0e01
       'TabularSourceConfig'
       'tabular'
       'config'
       code
@@ -653,22 +653,22 @@
                       76 RETURN_VALUE
          consts
             '\n    Load tabular source using the given configuration.\n\n    Args:\n        config (TabularSourceConfig): The configuration for loading the tabular source.\n\n    Returns:\n        SourceAdapter[Path, TablePosition, str]: A source adapter for loading tabular source.\n    '
          names      ('partial', 'load_tabular_source', 'encoding', 'errors', 'delimiter')
          varnames   ('config',)
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py'
          name       'load_tabular_source_using'
          firstlineno 88
          lnotab 0x020e
-   names      ('collections.abc', 'Iterable', 'Sequence', 'dataclasses', 'dataclass', 'csv', 'DictReader', 'functools', 'partial', 'pathlib', 'Path', 'whereisit.ports.source', 'SourceAdapter', 'SourceConfig', 'whereisit.types.entry', 'Entry', 'whereisit.types.factory', 'as_factory', 'TablePosition', 'tuple', 'str', 'list', '_handle_extra_columns', 'load_tabular_source', 'TabularSourceConfig', 'load_tabular_source_using')
+   names      ('collections.abc', 'Iterable', 'Sequence', 'dataclasses', 'dataclass', 'csv', 'DictReader', 'functools', 'partial', 'pathlib', 'Path', 'findanywhere.ports.source', 'SourceAdapter', 'SourceConfig', 'findanywhere.types.entry', 'Entry', 'findanywhere.types.factory', 'as_factory', 'TablePosition', 'tuple', 'str', 'list', '_handle_extra_columns', 'load_tabular_source', 'TabularSourceConfig', 'load_tabular_source_using')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/tabular.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/tabular.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020110010c010c010c010c0210010c010c03160118ff0e01020e60
       0c020102ff020202fe020302fd020402fc02052afb081e160126ff0e0102
       120401020102fe0e0420fc0e04
```

### Comparing `findanywhere-0.1.0/whereisit/adapters/source/__pycache__/text.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/adapters/source/__pycache__/text.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x28f35166 (Sat May 25 14:18:16 2024 UTC)
-files sz: 3731
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 3740
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 17
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -70,49 +70,49 @@
                 74 IMPORT_NAME             12 (toolz)
                 76 IMPORT_FROM             13 (compose)
                 78 STORE_NAME              13 (compose)
                 80 POP_TOP
    
      9          82 LOAD_CONST               0 (0)
                 84 LOAD_CONST               7 (('tokenize',))
-                86 IMPORT_NAME             14 (whereisit.algorithms.strings)
+                86 IMPORT_NAME             14 (findanywhere.algorithms.strings)
                 88 IMPORT_FROM             15 (tokenize)
                 90 STORE_NAME              15 (tokenize)
                 92 POP_TOP
    
     10          94 LOAD_CONST               0 (0)
                 96 LOAD_CONST               8 (('SourceAdapter', 'Entry', 'everything', 'SourceConfig'))
-                98 IMPORT_NAME             16 (whereisit.ports.source)
+                98 IMPORT_NAME             16 (findanywhere.ports.source)
                100 IMPORT_FROM             17 (SourceAdapter)
                102 STORE_NAME              17 (SourceAdapter)
                104 IMPORT_FROM             18 (Entry)
                106 STORE_NAME              18 (Entry)
                108 IMPORT_FROM             19 (everything)
                110 STORE_NAME              19 (everything)
                112 IMPORT_FROM             20 (SourceConfig)
                114 STORE_NAME              20 (SourceConfig)
                116 POP_TOP
    
     11         118 LOAD_CONST               0 (0)
                120 LOAD_CONST               9 (('as_factory',))
-               122 IMPORT_NAME             21 (whereisit.types.factory)
+               122 IMPORT_NAME             21 (findanywhere.types.factory)
                124 IMPORT_FROM             22 (as_factory)
                126 STORE_NAME              22 (as_factory)
                128 POP_TOP
    
     14         130 PUSH_NULL
                132 LOAD_NAME                5 (dataclass)
                134 LOAD_CONST              10 (True)
                136 KW_NAMES                11
                138 PRECALL                  1
                142 CALL                     1
    
     15         152 PUSH_NULL
                154 LOAD_BUILD_CLASS
-               156 LOAD_CONST              12 (<code object TextPosition, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/text.py", line 14>)
+               156 LOAD_CONST              12 (<code object TextPosition, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/text.py", line 14>)
                158 MAKE_FUNCTION            0
                160 LOAD_CONST              13 ('TextPosition')
                162 PRECALL                  2
                166 CALL                     2
    
     14         176 PRECALL                  0
                180 CALL                     0
@@ -167,28 +167,28 @@
                288 LOAD_NAME               24 (str)
                290 BUILD_TUPLE              2
                292 BINARY_SUBSCR
                302 BINARY_SUBSCR
                312 BINARY_SUBSCR
    
     27         322 BUILD_TUPLE             12
-               324 LOAD_CONST              21 (<code object load_text_source, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/text.py", line 27>)
+               324 LOAD_CONST              21 (<code object load_text_source, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/text.py", line 27>)
                326 MAKE_FUNCTION            6 (kwdefaults, annotations)
                328 STORE_NAME              27 (load_text_source)
    
     64         330 PUSH_NULL
                332 LOAD_NAME                5 (dataclass)
                334 LOAD_CONST              10 (True)
                336 KW_NAMES                11
                338 PRECALL                  1
                342 CALL                     1
    
     65         352 PUSH_NULL
                354 LOAD_BUILD_CLASS
-               356 LOAD_CONST              22 (<code object TextSourceConfig, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/text.py", line 64>)
+               356 LOAD_CONST              22 (<code object TextSourceConfig, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/text.py", line 64>)
                358 MAKE_FUNCTION            0
                360 LOAD_CONST              23 ('TextSourceConfig')
                362 LOAD_NAME               20 (SourceConfig)
                364 LOAD_NAME               11 (Path)
                366 BINARY_SUBSCR
                376 PRECALL                  3
                380 CALL                     3
@@ -211,15 +211,15 @@
                434 LOAD_NAME               17 (SourceAdapter)
                436 LOAD_NAME               11 (Path)
                438 LOAD_NAME               23 (TextPosition)
                440 LOAD_NAME               24 (str)
                442 BUILD_TUPLE              3
                444 BINARY_SUBSCR
                454 BUILD_TUPLE              4
-               456 LOAD_CONST              26 (<code object load_text_source_using, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/text.py", line 87>)
+               456 LOAD_CONST              26 (<code object load_text_source_using, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/text.py", line 87>)
                458 MAKE_FUNCTION            4 (annotations)
    
     87         460 PRECALL                  0
                464 CALL                     0
    
     88         474 STORE_NAME              29 (load_text_source_using)
                476 LOAD_CONST              27 (None)
@@ -272,15 +272,15 @@
             'line'
             'token'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'int', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/text.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/text.py'
          name       'TextPosition'
          firstlineno 14
          lnotab 0x0c0204070a01
       'TextPosition'
       ('predicate', 'tokenize')
       'encoding'
       'errors'
@@ -343,15 +343,15 @@
                      148 PRECALL                  1
                      152 CALL                     1
                      162 PRECALL                  2
                      166 CALL                     2
          
           59         176 LOAD_CLOSURE             7 (line_no)
                      178 BUILD_TUPLE              1
-                     180 LOAD_CONST               3 (<code object <genexpr>, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/text.py", line 59>)
+                     180 LOAD_CONST               3 (<code object <genexpr>, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/text.py", line 59>)
                      182 MAKE_FUNCTION            8 (closure)
                      184 LOAD_GLOBAL              3 (NULL + enumerate)
                      196 PUSH_NULL
                      198 LOAD_FAST                4 (tokenize)
                      200 LOAD_FAST                6 (line)
                      202 PRECALL                  1
                      206 CALL                     1
@@ -439,24 +439,24 @@
                             88 RETURN_VALUE
                consts
                   None
                names      ('Entry', 'TextPosition')
                varnames   ('.0', 'token_no', 'token')
                freevars   ('line_no',)
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/text.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/text.py'
                name       '<genexpr>'
                firstlineno 59
                lnotab 0x
             None
          names      ('open', 'enumerate', 'tuple', 'filter', 'compose', 'attrgetter')
          varnames   ('encoding', 'errors', 'location', 'predicate', 'tokenize', 'src', 'line')
          freevars   ()
          cellvars   ('line_no',)
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/text.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/text.py'
          name       'load_text_source'
          firstlineno 27
          lnotab 0x081b300128010c010c01380146fe0eff16ff02ff
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
@@ -505,15 +505,15 @@
           81          76 LOAD_NAME               10 (classmethod)
          
           82          78 LOAD_CONST               8 ('return')
                       80 LOAD_NAME               11 (type)
                       82 LOAD_NAME               12 (Path)
                       84 BINARY_SUBSCR
                       94 BUILD_TUPLE              2
-                      96 LOAD_CONST               9 (<code object location_type, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/text.py", line 81>)
+                      96 LOAD_CONST               9 (<code object location_type, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/text.py", line 81>)
                       98 MAKE_FUNCTION            4 (annotations)
          
           81         100 PRECALL                  0
                      104 CALL                     0
          
           82         114 STORE_NAME              13 (location_type)
                      116 LOAD_CONST               6 (None)
@@ -540,23 +540,23 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('Path',)
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/text.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/text.py'
                name       'location_type'
                firstlineno 81
                lnotab 0x0202
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'encoding', 'str', '__annotations__', 'errors', 'token_separators', 'list', 'classmethod', 'type', 'Path', 'location_type')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/text.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/text.py'
          name       'TextSourceConfig'
          firstlineno 64
          lnotab 0x0c02040b0e010e012002020116ff0e01
       'TextSourceConfig'
       'textfile'
       'config'
       code
@@ -609,23 +609,23 @@
             '\n    Args:\n        config: The configuration object that contains various parameters for loading the text source.\n\n    Returns:\n        SourceAdapter[Path, TextPosition, str]: The source adapter that can be used to load and process the text source.\n\n    Raises:\n        None\n    '
             ('delimiters',)
             ('tokenize',)
          names      ('str', 'split', 'token_separators', 'partial', 'tokenize', 'set', 'load_text_source', 'encoding', 'errors')
          varnames   ('config', 'tokenizer')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/text.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/text.py'
          name       'load_text_source_using'
          firstlineno 87
          lnotab 0x020c18010e015001
       None
-   names      ('collections.abc', 'Callable', 'Sequence', 'Iterable', 'dataclasses', 'dataclass', 'functools', 'partial', 'operator', 'attrgetter', 'pathlib', 'Path', 'toolz', 'compose', 'whereisit.algorithms.strings', 'tokenize', 'whereisit.ports.source', 'SourceAdapter', 'Entry', 'everything', 'SourceConfig', 'whereisit.types.factory', 'as_factory', 'TextPosition', 'str', 'split', 'bool', 'load_text_source', 'TextSourceConfig', 'load_text_source_using')
+   names      ('collections.abc', 'Callable', 'Sequence', 'Iterable', 'dataclasses', 'dataclass', 'functools', 'partial', 'operator', 'attrgetter', 'pathlib', 'Path', 'toolz', 'compose', 'findanywhere.algorithms.strings', 'tokenize', 'findanywhere.ports.source', 'SourceAdapter', 'Entry', 'everything', 'SourceConfig', 'findanywhere.types.factory', 'as_factory', 'TextPosition', 'str', 'split', 'bool', 'load_text_source', 'TextSourceConfig', 'load_text_source_using')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/adapters/source/text.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/adapters/source/text.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020114010c010c010c010c020c020c0118010c03160118ff0e0102
       1102010cfa060102ff020202fe020302fd020514fb020620fa02072af908
       25160126ff0e010216160120ff0e01
```

### Comparing `findanywhere-0.1.0/whereisit/adapters/source/tabular.py` & `findanywhere-1.0.0/findanywhere/adapters/source/tabular.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections.abc import Iterable, Sequence
 from dataclasses import dataclass
 from csv import DictReader
 from functools import partial
 from pathlib import Path
 
-from whereisit.ports.source import SourceAdapter, SourceConfig
-from whereisit.types.entry import Entry
-from whereisit.types.factory import as_factory
+from findanywhere.ports.source import SourceAdapter, SourceConfig
+from findanywhere.types.entry import Entry
+from findanywhere.types.factory import as_factory
 
 
 @dataclass(frozen=True)
 class TablePosition:
     """
 
     TablePosition represents the position of a table in a document.
```

### Comparing `findanywhere-0.1.0/whereisit/adapters/source/text.py` & `findanywhere-1.0.0/findanywhere/adapters/source/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from dataclasses import dataclass
 from functools import partial
 from operator import attrgetter
 from pathlib import Path
 
 from toolz import compose
 
-from whereisit.algorithms.strings import tokenize
-from whereisit.ports.source import SourceAdapter, Entry, everything, SourceConfig
-from whereisit.types.factory import as_factory
+from findanywhere.algorithms.strings import tokenize
+from findanywhere.ports.source import SourceAdapter, Entry, everything, SourceConfig
+from findanywhere.types.factory import as_factory
 
 
 @dataclass(frozen=True)
 class TextPosition:
     """
     Dataclass representing a position in a text document.
```

### Comparing `findanywhere-0.1.0/whereisit/algorithms/__pycache__/strings.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/algorithms/__pycache__/strings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-0.1.0/whereisit/algorithms/strings.py` & `findanywhere-1.0.0/findanywhere/algorithms/strings.py`

 * *Files identical despite different names*

### Comparing `findanywhere-0.1.0/whereisit/ports/__pycache__/source.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/ports/__pycache__/source.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xe3f05166 (Sat May 25 14:08:35 2024 UTC)
-files sz: 1933
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 1939
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x97005500640064016c006d015a016d025a026d035a030100640064026c
@@ -50,22 +50,22 @@
                 52 STORE_NAME               9 (TypeAlias)
                 54 IMPORT_FROM             10 (Generic)
                 56 STORE_NAME              10 (Generic)
                 58 POP_TOP
    
      5          60 LOAD_CONST               0 (0)
                 62 LOAD_CONST               4 (('Entry',))
-                64 IMPORT_NAME             11 (whereisit.types.entry)
+                64 IMPORT_NAME             11 (findanywhere.types.entry)
                 66 IMPORT_FROM             12 (Entry)
                 68 STORE_NAME              12 (Entry)
                 70 POP_TOP
    
      6          72 LOAD_CONST               0 (0)
                 74 LOAD_CONST               5 (('Config',))
-                76 IMPORT_NAME             13 (whereisit.types.factory)
+                76 IMPORT_NAME             13 (findanywhere.types.factory)
                 78 IMPORT_FROM             14 (Config)
                 80 STORE_NAME              14 (Config)
                 82 POP_TOP
    
      8          84 PUSH_NULL
                 86 LOAD_NAME                7 (TypeVar)
                 88 LOAD_CONST               6 ('Location')
@@ -90,21 +90,21 @@
                152 STORE_NAME              17 (DataType)
    
     13         154 LOAD_CONST              11 ('_')
                156 LOAD_NAME               16 (Position)
                158 LOAD_CONST              12 ('return')
                160 LOAD_NAME               18 (bool)
                162 BUILD_TUPLE              4
-               164 LOAD_CONST              13 (<code object everything, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/ports/source.py", line 13>)
+               164 LOAD_CONST              13 (<code object everything, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ports/source.py", line 13>)
                166 MAKE_FUNCTION            4 (annotations)
                168 STORE_NAME              19 (everything)
    
     25         170 PUSH_NULL
                172 LOAD_BUILD_CLASS
-               174 LOAD_CONST              14 (<code object SourcePort, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/ports/source.py", line 25>)
+               174 LOAD_CONST              14 (<code object SourcePort, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ports/source.py", line 25>)
                176 MAKE_FUNCTION            0
                178 LOAD_CONST              15 ('SourcePort')
                180 LOAD_NAME                8 (Protocol)
                182 LOAD_NAME               15 (Location)
                184 LOAD_NAME               16 (Position)
                186 LOAD_NAME               17 (DataType)
                188 BUILD_TUPLE              3
@@ -125,15 +125,15 @@
                234 LOAD_CONST               7 (True)
                236 KW_NAMES                17
                238 PRECALL                  1
                242 CALL                     1
    
     49         252 PUSH_NULL
                254 LOAD_BUILD_CLASS
-               256 LOAD_CONST              18 (<code object SourceConfig, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/ports/source.py", line 48>)
+               256 LOAD_CONST              18 (<code object SourceConfig, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ports/source.py", line 48>)
                258 MAKE_FUNCTION            0
                260 LOAD_CONST              19 ('SourceConfig')
                262 LOAD_NAME               14 (Config)
                264 LOAD_NAME               10 (Generic)
                266 LOAD_NAME               15 (Location)
                268 BINARY_SUBSCR
                278 PRECALL                  4
@@ -172,15 +172,15 @@
          consts
             '\n    Args:\n        _: The Position object to be checked for evaluation.\n\n    Returns:\n        bool: Returns True.\n\n    '
             True
          names      ()
          varnames   ('_',)
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/ports/source.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ports/source.py'
          name       'everything'
          firstlineno 13
          lnotab 0x0209
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
@@ -224,15 +224,15 @@
                       54 LOAD_NAME               12 (DataType)
                       56 BUILD_TUPLE              2
                       58 BINARY_SUBSCR
                       68 BINARY_SUBSCR
                       78 BINARY_SUBSCR
          
           29          88 BUILD_TUPLE              6
-                      90 LOAD_CONST               5 (<code object __call__, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/ports/source.py", line 29>)
+                      90 LOAD_CONST               5 (<code object __call__, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ports/source.py", line 29>)
                       92 MAKE_FUNCTION            5 (defaults, annotations)
                       94 STORE_NAME              13 (__call__)
                       96 LOAD_CONST               6 (None)
                       98 RETURN_VALUE
          consts
             'SourcePort'
             '\n    Retrieves a sequence of Entry objects based on the given location and optional predicate.\n    '
@@ -252,24 +252,24 @@
                consts
                   '\n        Args:\n            location: A Location object that specifies the location to search for entries.\n            predicate: A Callable object that takes a Position object as input and returns a boolean value.\n            The predicate is used to filter entries based on specific criteria. If not provided, the default predicate\n            (everything) will be used.\n\n        Returns:\n            An iterable sequence of Entry objects, where each entry contains a Position object and a DataType object.\n        '
                   None
                names      ()
                varnames   ('self', 'location', 'predicate')
                freevars   ()
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/ports/source.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ports/source.py'
                name       '__call__'
                firstlineno 29
                lnotab 0x020d
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'everything', 'Location', 'Callable', 'Position', 'bool', 'Iterable', 'Sequence', 'Entry', 'DataType', '__call__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/ports/source.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ports/source.py'
          name       'SourcePort'
          firstlineno 25
          lnotab 0x0a01040402ff040102ff020114ff02022afe
       'SourcePort'
       'SourceAdapter'
       ('frozen',)
       code
@@ -292,15 +292,15 @@
           53          14 LOAD_NAME                4 (classmethod)
          
           54          16 LOAD_CONST               2 ('return')
                       18 LOAD_NAME                5 (type)
                       20 LOAD_NAME                6 (Location)
                       22 BINARY_SUBSCR
                       32 BUILD_TUPLE              2
-                      34 LOAD_CONST               3 (<code object location_type, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/ports/source.py", line 53>)
+                      34 LOAD_CONST               3 (<code object location_type, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ports/source.py", line 53>)
                       36 MAKE_FUNCTION            4 (annotations)
          
           53          38 PRECALL                  0
                       42 CALL                     0
          
           54          52 STORE_NAME               7 (location_type)
                       54 LOAD_CONST               4 (None)
@@ -325,32 +325,32 @@
                             28 RAISE_VARARGS            1
                consts
                   "\n        Returns the type of the 'Location' class.\n\n        Returns:\n            The type of the 'Location' class.\n\n        Raises:\n            NotImplementedError: Subclasses should implement this method.\n        "
                names      ('NotImplementedError',)
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/ports/source.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ports/source.py'
                name       'location_type'
                firstlineno 53
                lnotab 0x020b
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'classmethod', 'type', 'Location', 'location_type')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/ports/source.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ports/source.py'
          name       'SourceConfig'
          firstlineno 48
          lnotab 0x0a020403020116ff0e01
       'SourceConfig'
       None
-   names      ('collections.abc', 'Iterable', 'Callable', 'Sequence', 'dataclasses', 'dataclass', 'typing', 'TypeVar', 'Protocol', 'TypeAlias', 'Generic', 'whereisit.types.entry', 'Entry', 'whereisit.types.factory', 'Config', 'Location', 'Position', 'DataType', 'bool', 'everything', 'SourcePort', 'SourceAdapter', '__annotations__', 'SourceConfig')
+   names      ('collections.abc', 'Iterable', 'Callable', 'Sequence', 'dataclasses', 'dataclass', 'typing', 'TypeVar', 'Protocol', 'TypeAlias', 'Generic', 'findanywhere.types.entry', 'Entry', 'findanywhere.types.factory', 'Config', 'Location', 'Position', 'DataType', 'bool', 'everything', 'SourcePort', 'SourceAdapter', '__annotations__', 'SourceConfig')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/ports/source.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ports/source.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020116010c0118020c010c021a0116011603100c2e140e03160128
       ff0e01
```

### Comparing `findanywhere-0.1.0/whereisit/ports/evaluation.py` & `findanywhere-1.0.0/findanywhere/ports/evaluation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Sequence, Callable, Iterable
 from dataclasses import replace
 from operator import attrgetter
 from typing import Protocol, TypeAlias, TypeVar
 
-from whereisit.ports.source import Position, DataType, Entry
-from whereisit.types.input_data import InputData
-from whereisit.types.similarity import Evaluation, ScoredEntry
+from findanywhere.ports.source import Position, DataType, Entry
+from findanywhere.types.input_data import InputData
+from findanywhere.types.similarity import Evaluation, ScoredEntry
 
 _T = TypeVar('_T')
 
 
 class EvaluationPort(Protocol[DataType]):
     """
     Class representing an evaluation port.
```

### Comparing `findanywhere-0.1.0/whereisit/ports/source.py` & `findanywhere-1.0.0/findanywhere/ports/source.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections.abc import Iterable, Callable, Sequence
 from dataclasses import dataclass
 from typing import TypeVar, Protocol, TypeAlias, Generic
 
-from whereisit.types.entry import Entry
-from whereisit.types.factory import Config
+from findanywhere.types.entry import Entry
+from findanywhere.types.factory import Config
 
 Location = TypeVar('Location', contravariant=True)
 Position = TypeVar('Position')
 DataType = TypeVar('DataType')
 
 
 def everything(_: Position) -> bool:
```

### Comparing `findanywhere-0.1.0/whereisit/schema.py` & `findanywhere-1.0.0/findanywhere/schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from dataclasses import dataclass, asdict
 from pathlib import Path
 from typing import TypeVar, Any, Generic
 
 from dacite import from_dict
 from yaml import dump, unsafe_load
 
-from whereisit.adapters.evaluation import EVALUATION_FACTORIES
-from whereisit.adapters.source import SOURCE_FACTORIES
-from whereisit.ports.evaluation import EvaluationAdapter
-from whereisit.ports.source import SourceAdapter, SourceConfig
-from whereisit.scores import DEDUCTION_FACTORIES, DEFAULT_DEDUCTION
-from whereisit.thresholds import THRESHOLD_FACTORIES, DEFAULT_THRESHOLD
-from whereisit.types.factory import Config, FactoryMap
-from whereisit.types.similarity import DeduceScore, ThresholdFilter
+from findanywhere.adapters.evaluation import EVALUATION_FACTORIES
+from findanywhere.adapters.source import SOURCE_FACTORIES
+from findanywhere.ports.evaluation import EvaluationAdapter
+from findanywhere.ports.source import SourceAdapter, SourceConfig
+from findanywhere.scores import DEDUCTION_FACTORIES, DEFAULT_DEDUCTION
+from findanywhere.thresholds import THRESHOLD_FACTORIES, DEFAULT_THRESHOLD
+from findanywhere.types.factory import Config, FactoryMap
+from findanywhere.types.similarity import DeduceScore, ThresholdFilter
 
 _T = TypeVar('_T')
 _C = TypeVar('_C', bound=Config)
 
 
 @dataclass(frozen=True)
 class AdapterConfig(Generic[_C]):
```

### Comparing `findanywhere-0.1.0/whereisit/scores/__pycache__/deduction.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/scores/__pycache__/deduction.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xe3f05166 (Sat May 25 14:08:35 2024 UTC)
-files sz: 1333
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 1345
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -21,38 +21,38 @@
                  6 IMPORT_NAME              0 (operator)
                  8 IMPORT_FROM              1 (attrgetter)
                 10 STORE_NAME               1 (attrgetter)
                 12 POP_TOP
    
      3          14 LOAD_CONST               0 (0)
                 16 LOAD_CONST               2 (('Position',))
-                18 IMPORT_NAME              2 (whereisit.ports.source)
+                18 IMPORT_NAME              2 (findanywhere.ports.source)
                 20 IMPORT_FROM              3 (Position)
                 22 STORE_NAME               3 (Position)
                 24 POP_TOP
    
      4          26 LOAD_CONST               0 (0)
                 28 LOAD_CONST               3 (('DataType',))
-                30 IMPORT_NAME              4 (whereisit.types.entry)
+                30 IMPORT_NAME              4 (findanywhere.types.entry)
                 32 IMPORT_FROM              5 (DataType)
                 34 STORE_NAME               5 (DataType)
                 36 POP_TOP
    
      5          38 LOAD_CONST               0 (0)
                 40 LOAD_CONST               4 (('as_factory', 'Config'))
-                42 IMPORT_NAME              6 (whereisit.types.factory)
+                42 IMPORT_NAME              6 (findanywhere.types.factory)
                 44 IMPORT_FROM              7 (as_factory)
                 46 STORE_NAME               7 (as_factory)
                 48 IMPORT_FROM              8 (Config)
                 50 STORE_NAME               8 (Config)
                 52 POP_TOP
    
      6          54 LOAD_CONST               0 (0)
                 56 LOAD_CONST               5 (('Evaluation', 'ScoredEvaluation', 'DeduceScore'))
-                58 IMPORT_NAME              9 (whereisit.types.similarity)
+                58 IMPORT_NAME              9 (findanywhere.types.similarity)
                 60 IMPORT_FROM             10 (Evaluation)
                 62 STORE_NAME              10 (Evaluation)
                 64 IMPORT_FROM             11 (ScoredEvaluation)
                 66 STORE_NAME              11 (ScoredEvaluation)
                 68 IMPORT_FROM             12 (DeduceScore)
                 70 STORE_NAME              12 (DeduceScore)
                 72 POP_TOP
@@ -66,15 +66,15 @@
                 94 LOAD_CONST               7 ('return')
                 96 LOAD_NAME               11 (ScoredEvaluation)
                 98 LOAD_NAME                3 (Position)
                100 LOAD_NAME                5 (DataType)
                102 BUILD_TUPLE              2
                104 BINARY_SUBSCR
                114 BUILD_TUPLE              4
-               116 LOAD_CONST               8 (<code object average_score, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/scores/deduction.py", line 9>)
+               116 LOAD_CONST               8 (<code object average_score, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/scores/deduction.py", line 9>)
                118 MAKE_FUNCTION            4 (annotations)
                120 STORE_NAME              13 (average_score)
    
     24         122 PUSH_NULL
                124 LOAD_NAME                7 (as_factory)
                126 LOAD_CONST               9 ('average')
                128 LOAD_NAME               13 (average_score)
@@ -87,15 +87,15 @@
                150 LOAD_CONST               7 ('return')
                152 LOAD_NAME               12 (DeduceScore)
                154 LOAD_NAME                3 (Position)
                156 LOAD_NAME                5 (DataType)
                158 BUILD_TUPLE              2
                160 BINARY_SUBSCR
                170 BUILD_TUPLE              4
-               172 LOAD_CONST              12 (<code object create_average_score, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/scores/deduction.py", line 24>)
+               172 LOAD_CONST              12 (<code object create_average_score, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/scores/deduction.py", line 24>)
                174 MAKE_FUNCTION            4 (annotations)
    
     24         176 PRECALL                  0
                180 CALL                     0
    
     25         190 STORE_NAME              14 (create_average_score)
                192 LOAD_CONST              13 (None)
@@ -170,15 +170,15 @@
             '\n    Calculate the average score of an evaluation.\n\n    Args:\n        evaluation: An Evaluation object containing the best matches and their similarities.\n\n    Returns:\n        A ScoredEvaluation object with the original evaluation, best matches, and the average score.\n    '
             'similarity'
             0.0
          names      ('sum', 'map', 'attrgetter', 'best_matches', 'values', 'len', 'ScoredEvaluation', 'of')
          varnames   ('evaluation', 'score_sum', 'score')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/scores/deduction.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/scores/deduction.py'
          name       'average_score'
          firstlineno 9
          lnotab 0x020a82014001
       'average'
       ('using',)
       'config'
       code
@@ -193,20 +193,20 @@
                       14 RETURN_VALUE
          consts
             '\n    Args:\n        config: The configuration object that contains the necessary information to create the average score.\n\n    Returns:\n        An instance of the DeduceScore class with the average_score function as the implementation.\n\n    Raises:\n        None\n    '
          names      ('average_score',)
          varnames   ('config',)
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/scores/deduction.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/scores/deduction.py'
          name       'create_average_score'
          firstlineno 24
          lnotab 0x020c
       None
-   names      ('operator', 'attrgetter', 'whereisit.ports.source', 'Position', 'whereisit.types.entry', 'DataType', 'whereisit.types.factory', 'as_factory', 'Config', 'whereisit.types.similarity', 'Evaluation', 'ScoredEvaluation', 'DeduceScore', 'average_score', 'create_average_score')
+   names      ('operator', 'attrgetter', 'findanywhere.ports.source', 'Position', 'findanywhere.types.entry', 'DataType', 'findanywhere.types.factory', 'as_factory', 'Config', 'findanywhere.types.similarity', 'Evaluation', 'ScoredEvaluation', 'DeduceScore', 'average_score', 'create_average_score')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/scores/deduction.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/scores/deduction.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c020c010c0110011403300f18011eff0e01
```

### Comparing `findanywhere-0.1.0/whereisit/scores/deduction.py` & `findanywhere-1.0.0/findanywhere/scores/deduction.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from operator import attrgetter
 
-from whereisit.ports.source import Position
-from whereisit.types.entry import DataType
-from whereisit.types.factory import as_factory, Config
-from whereisit.types.similarity import Evaluation, ScoredEvaluation, DeduceScore
+from findanywhere.ports.source import Position
+from findanywhere.types.entry import DataType
+from findanywhere.types.factory import as_factory, Config
+from findanywhere.types.similarity import Evaluation, ScoredEvaluation, DeduceScore
 
 
 def average_score(evaluation: Evaluation[Position, DataType]) -> ScoredEvaluation[Position, DataType]:
     """
     Calculate the average score of an evaluation.
 
     Args:
```

### Comparing `findanywhere-0.1.0/whereisit/search/__pycache__/base.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/search/__pycache__/base.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x43e95166 (Sat May 25 13:36:03 2024 UTC)
-files sz: 6048
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 6060
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 15
    flags     : 0
    code
       0x970064005a00640164026c016d025a026d035a030100640164036c046d
@@ -73,40 +73,40 @@
                 78 IMPORT_NAME             13 (uuid)
                 80 IMPORT_FROM             14 (uuid4)
                 82 STORE_NAME              14 (uuid4)
                 84 POP_TOP
    
     23          86 LOAD_CONST               1 (0)
                 88 LOAD_CONST               8 (('EvaluationAdapter', 'Position'))
-                90 IMPORT_NAME             15 (whereisit.ports.evaluation)
+                90 IMPORT_NAME             15 (findanywhere.ports.evaluation)
                 92 IMPORT_FROM             16 (EvaluationAdapter)
                 94 STORE_NAME              16 (EvaluationAdapter)
                 96 IMPORT_FROM             17 (Position)
                 98 STORE_NAME              17 (Position)
                100 POP_TOP
    
     24         102 LOAD_CONST               1 (0)
                104 LOAD_CONST               9 (('Entry',))
-               106 IMPORT_NAME             18 (whereisit.types.entry)
+               106 IMPORT_NAME             18 (findanywhere.types.entry)
                108 IMPORT_FROM             19 (Entry)
                110 STORE_NAME              19 (Entry)
                112 POP_TOP
    
     25         114 LOAD_CONST               1 (0)
                116 LOAD_CONST              10 (('InputData', 'DataType'))
-               118 IMPORT_NAME             20 (whereisit.types.input_data)
+               118 IMPORT_NAME             20 (findanywhere.types.input_data)
                120 IMPORT_FROM             21 (InputData)
                122 STORE_NAME              21 (InputData)
                124 IMPORT_FROM             22 (DataType)
                126 STORE_NAME              22 (DataType)
                128 POP_TOP
    
     26         130 LOAD_CONST               1 (0)
                132 LOAD_CONST              11 (('DeduceScore', 'ThresholdFilter', 'ScoredEvaluation'))
-               134 IMPORT_NAME             23 (whereisit.types.similarity)
+               134 IMPORT_NAME             23 (findanywhere.types.similarity)
                136 IMPORT_FROM             24 (DeduceScore)
                138 STORE_NAME              24 (DeduceScore)
                140 IMPORT_FROM             25 (ThresholdFilter)
                142 STORE_NAME              25 (ThresholdFilter)
                144 IMPORT_FROM             26 (ScoredEvaluation)
                146 STORE_NAME              26 (ScoredEvaluation)
                148 POP_TOP
@@ -158,35 +158,35 @@
                272 LOAD_NAME               17 (Position)
                274 LOAD_NAME               22 (DataType)
                276 BUILD_TUPLE              2
                278 BINARY_SUBSCR
                288 BINARY_SUBSCR
    
     29         298 BUILD_TUPLE             12
-               300 LOAD_CONST              18 (<code object search, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/base.py", line 29>)
+               300 LOAD_CONST              18 (<code object search, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/base.py", line 29>)
                302 MAKE_FUNCTION            4 (annotations)
                304 STORE_NAME              27 (search)
    
     63         306 PUSH_NULL
                308 LOAD_BUILD_CLASS
-               310 LOAD_CONST              19 (<code object Search, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/base.py", line 63>)
+               310 LOAD_CONST              19 (<code object Search, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/base.py", line 63>)
                312 MAKE_FUNCTION            0
                314 LOAD_CONST              20 ('Search')
                316 LOAD_NAME               11 (Protocol)
                318 LOAD_NAME               17 (Position)
                320 LOAD_NAME               22 (DataType)
                322 BUILD_TUPLE              2
                324 BINARY_SUBSCR
                334 PRECALL                  3
                338 CALL                     3
                348 STORE_NAME              28 (Search)
    
     84         350 PUSH_NULL
                352 LOAD_BUILD_CLASS
-               354 LOAD_CONST              21 (<code object SearchPattern, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/base.py", line 84>)
+               354 LOAD_CONST              21 (<code object SearchPattern, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/base.py", line 84>)
                356 MAKE_FUNCTION            0
                358 LOAD_CONST              22 ('SearchPattern')
                360 LOAD_NAME               11 (Protocol)
                362 LOAD_NAME               17 (Position)
                364 LOAD_NAME               22 (DataType)
                366 BUILD_TUPLE              2
                368 BINARY_SUBSCR
@@ -225,15 +225,15 @@
                468 BINARY_SUBSCR
    
    114         478 LOAD_CONST              17 ('return')
    
    119         480 LOAD_NAME                9 (Path)
    
    114         482 BUILD_TUPLE             10
-               484 LOAD_CONST              25 (<code object buffered_search, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/base.py", line 114>)
+               484 LOAD_CONST              25 (<code object buffered_search, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/base.py", line 114>)
                486 MAKE_FUNCTION            4 (annotations)
                488 STORE_NAME              30 (buffered_search)
                490 LOAD_CONST              26 (None)
                492 RETURN_VALUE
    consts
       '\nThis module contains the core search functionality of the application.\nIt provides two key functions: `search` and `buffered_search`.\n\n`search` is a generic function that evaluates input data against a set of entries\nusing the provided evaluation and scoring mechanisms. It filters the results based on a threshold filter.\n\n`buffered_search` function performs a search, using an instance of the `search` function,\non the provided input data and entries. The results are stored in a buffer file created\nin the specified directory. The buffer file contains the search results in a JSON line\nformat (each search result is a separate JSON object).\n\nTogether, these functions enable flexible and efficient searching within the context of the application.\n'
       0
@@ -302,15 +302,15 @@
          consts
             '\n    Evaluates the input data against a set of entries using the provided evaluation and scoring mechanisms,\n    and filters the results based on a threshold filter. The function is generic and can work in different contexts\n    matching/searching tasks.\n\n    Args:\n        evaluate: An instance of EvaluationAdapter[DataType], used to evaluate the search data against the entries.\n        deduce_score: An instance of DeduceScore[Position, DataType], used to calculate the score based on the search\n        data evaluation.\n        threshold: An instance of ThresholdFilter[Position, DataType], used to filter the scored evaluations based on a\n        threshold.\n        input_data: A sequence of InputData[DataType] objects, representing the search data for which evaluations need\n        to be generated.\n        entries: A sequence of Entry[Position, DataType] objects, representing the entries against which the search data\n        is evaluated.\n\n    Returns:\n        An iterable of ScoredEvaluation[Position, DataType] objects, containing the scored evaluations that pass the\n        threshold filter.\n\n    '
             None
          names      ()
          varnames   ('evaluate', 'deduce_score', 'threshold', 'input_data', 'entries', 'search_data', 'scored_evaluation')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/base.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/base.py'
          name       'search'
          firstlineno 29
          lnotab 0x061c08012a0116010afd
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
@@ -354,15 +354,15 @@
                       80 LOAD_NAME                8 (Position)
                       82 LOAD_NAME                6 (DataType)
                       84 BUILD_TUPLE              2
                       86 BINARY_SUBSCR
                       96 BINARY_SUBSCR
          
           68         106 BUILD_TUPLE              6
-                     108 LOAD_CONST               5 (<code object __call__, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/base.py", line 68>)
+                     108 LOAD_CONST               5 (<code object __call__, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/base.py", line 68>)
                      110 MAKE_FUNCTION            4 (annotations)
                      112 STORE_NAME              11 (__call__)
                      114 LOAD_CONST               6 (None)
                      116 RETURN_VALUE
          consts
             'Search'
             '\n    A generic class representing a search algorithm.\n    '
@@ -382,24 +382,24 @@
                consts
                   '\n        Args:\n            input_data: A sequence of InputData objects representing the input data for evaluation.\n            entries: A sequence of Entry objects representing the entries to be evaluated.\n\n        Returns:\n            An iterable of ScoredEvaluation objects representing the evaluation results.\n        '
                   None
                names      ()
                varnames   ('self', 'input_data', 'entries')
                freevars   ()
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/base.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/base.py'
                name       '__call__'
                firstlineno 68
                lnotab 0x020d
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Sequence', 'InputData', 'DataType', 'Entry', 'Position', 'Iterable', 'ScoredEvaluation', '__call__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/base.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/base.py'
          name       'Search'
          firstlineno 63
          lnotab 0x0a01040402021afe02031efd02041efc
       'Search'
       code
          argcount  : 0
          nlocals   : 0
@@ -462,15 +462,15 @@
                      132 LOAD_NAME               14 (Any)
                      134 BUILD_TUPLE              2
                      136 BINARY_SUBSCR
                      146 BINARY_OP                7 (|)
                      150 BINARY_SUBSCR
          
           94         160 BUILD_TUPLE              8
-                     162 LOAD_CONST               6 (<code object __call__, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/base.py", line 94>)
+                     162 LOAD_CONST               6 (<code object __call__, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/base.py", line 94>)
                      164 MAKE_FUNCTION            4 (annotations)
                      166 STORE_NAME              15 (__call__)
                      168 LOAD_CONST               7 (None)
                      170 RETURN_VALUE
          consts
             'SearchPattern'
             '\n    A class representing a search pattern.\n\n    The SearchPattern class is a callable protocol that defines the behavior of a search pattern. It takes in input data\n    , a search algorithm, and a set of entries to evaluate. It returns an iterable of scored\n    evaluations or dictionaries.\n\n    '
@@ -491,24 +491,24 @@
                consts
                   '\n        Args:\n            input_data: A sequence of InputData objects, representing the input data to be evaluated.\n            search_: A Search object, representing the search algorithm to be used.\n            entries: An iterable of sequences of Entry objects, representing the entries to be evaluated.\n\n        Returns:\n            An iterable of ScoredEvaluation objects or dictionaries. Each ScoredEvaluation object represents the result\n            of evaluating an entry and contains the position and data type scores. Each dictionary represents the result\n             of evaluating an entry and contains additional information.\n        '
                   None
                names      ()
                varnames   ('self', 'input_data', 'search_', 'entries')
                freevars   ()
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/base.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/base.py'
                name       '__call__'
                firstlineno 94
                lnotab 0x0211
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Sequence', 'InputData', 'DataType', 'Search', 'Position', 'Iterable', 'Entry', 'ScoredEvaluation', 'dict', 'str', 'Any', '__call__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/base.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/base.py'
          name       'SearchPattern'
          firstlineno 84
          lnotab 0x0a01040902021afe020312fd02042afc020534fb
       'SearchPattern'
       'search_'
       'directory'
       code
@@ -607,23 +607,23 @@
             'surrogateescape'
             ('encoding', 'errors')
             None
          names      ('joinpath', 'uuid4', 'open', 'dump', 'asdict')
          varnames   ('search_', 'directory', 'input_data', 'entries', 'buffer_file', 'out', 'result')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/base.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/base.py'
          name       'buffered_search'
          firstlineno 114
          lnotab 0x0215480132011c013cff02ff2e03
       None
-   names      ('__doc__', 'collections.abc', 'Sequence', 'Iterable', 'dataclasses', 'asdict', 'json', 'dump', 'pathlib', 'Path', 'typing', 'Protocol', 'Any', 'uuid', 'uuid4', 'whereisit.ports.evaluation', 'EvaluationAdapter', 'Position', 'whereisit.types.entry', 'Entry', 'whereisit.types.input_data', 'InputData', 'DataType', 'whereisit.types.similarity', 'DeduceScore', 'ThresholdFilter', 'ScoredEvaluation', 'search', 'Search', 'SearchPattern', 'buffered_search')
+   names      ('__doc__', 'collections.abc', 'Sequence', 'Iterable', 'dataclasses', 'asdict', 'json', 'dump', 'pathlib', 'Path', 'typing', 'Protocol', 'Any', 'uuid', 'uuid4', 'findanywhere.ports.evaluation', 'EvaluationAdapter', 'Position', 'findanywhere.types.entry', 'Entry', 'findanywhere.types.input_data', 'InputData', 'DataType', 'findanywhere.types.similarity', 'DeduceScore', 'ThresholdFilter', 'ScoredEvaluation', 'search', 'Search', 'SearchPattern', 'buffered_search')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/base.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/base.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201040f10010c010c010c0110010c0210010c011001140302010e
       ff020212fe020312fd02041afc02051efb02061efa08222c152c1e020112
       ff020202fe02031afd02041efc020502fb
```

### Comparing `findanywhere-0.1.0/whereisit/search/__pycache__/parallel.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/search/__pycache__/parallel.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x45ea5166 (Sat May 25 13:40:21 2024 UTC)
-files sz: 2390
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 2405
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 16
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -76,40 +76,40 @@
                 94 IMPORT_NAME             15 (typing)
                 96 IMPORT_FROM             16 (Any)
                 98 STORE_NAME              16 (Any)
                100 POP_TOP
    
     10         102 LOAD_CONST               0 (0)
                104 LOAD_CONST               9 (('Position', 'DataType'))
-               106 IMPORT_NAME             17 (whereisit.ports.source)
+               106 IMPORT_NAME             17 (findanywhere.ports.source)
                108 IMPORT_FROM             18 (Position)
                110 STORE_NAME              18 (Position)
                112 IMPORT_FROM             19 (DataType)
                114 STORE_NAME              19 (DataType)
                116 POP_TOP
    
     11         118 LOAD_CONST               0 (0)
                120 LOAD_CONST              10 (('Search', 'buffered_search'))
-               122 IMPORT_NAME             20 (whereisit.search.base)
+               122 IMPORT_NAME             20 (findanywhere.search.base)
                124 IMPORT_FROM             21 (Search)
                126 STORE_NAME              21 (Search)
                128 IMPORT_FROM             22 (buffered_search)
                130 STORE_NAME              22 (buffered_search)
                132 POP_TOP
    
     12         134 LOAD_CONST               0 (0)
                136 LOAD_CONST              11 (('Entry',))
-               138 IMPORT_NAME             23 (whereisit.types.entry)
+               138 IMPORT_NAME             23 (findanywhere.types.entry)
                140 IMPORT_FROM             24 (Entry)
                142 STORE_NAME              24 (Entry)
                144 POP_TOP
    
     13         146 LOAD_CONST               0 (0)
                148 LOAD_CONST              12 (('InputData',))
-               150 IMPORT_NAME             25 (whereisit.types.input_data)
+               150 IMPORT_NAME             25 (findanywhere.types.input_data)
                152 IMPORT_FROM             26 (InputData)
                154 STORE_NAME              26 (InputData)
                156 POP_TOP
    
     20         158 PUSH_NULL
                160 LOAD_NAME                8 (cpu_count)
                162 PRECALL                  0
@@ -122,15 +122,15 @@
    
     17         182 LOAD_NAME                1 (Sequence)
                184 LOAD_NAME               26 (InputData)
                186 LOAD_NAME               19 (DataType)
                188 BINARY_SUBSCR
                198 BINARY_SUBSCR
    
-    16         208 LOAD_CONST              15 ('search')
+    16         208 LOAD_CONST              15 ('search_')
    
     18         210 LOAD_NAME               21 (Search)
                212 LOAD_NAME               18 (Position)
                214 LOAD_NAME               19 (DataType)
                216 BUILD_TUPLE              2
                218 BINARY_SUBSCR
    
@@ -161,15 +161,15 @@
                286 LOAD_NAME               29 (str)
                288 LOAD_NAME               16 (Any)
                290 BUILD_TUPLE              2
                292 BINARY_SUBSCR
                302 BINARY_SUBSCR
    
     16         312 BUILD_TUPLE             12
-               314 LOAD_CONST              20 (<code object parallel_search, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/parallel.py", line 16>)
+               314 LOAD_CONST              20 (<code object parallel_search, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/parallel.py", line 16>)
                316 MAKE_FUNCTION            5 (defaults, annotations)
                318 STORE_NAME              30 (parallel_search)
                320 LOAD_CONST              21 (None)
                322 RETURN_VALUE
    consts
       0
       ('Sequence', 'Iterable')
@@ -182,15 +182,15 @@
       ('Any',)
       ('Position', 'DataType')
       ('Search', 'buffered_search')
       ('Entry',)
       ('InputData',)
       1000
       'input_data'
-      'search'
+      'search_'
       'entries'
       'processes'
       'chunk_size'
       'return'
       code
          argcount  : 5
          nlocals   : 11
@@ -236,15 +236,15 @@
                       96 STORE_FAST               7 (buffer_dir)
          
           44          98 LOAD_FAST                5 (pool)
                      100 LOAD_METHOD              3 (imap_unordered)
          
           45         122 LOAD_GLOBAL              9 (NULL + partial)
                      134 LOAD_GLOBAL             10 (buffered_search)
-                     146 LOAD_FAST                1 (search)
+                     146 LOAD_FAST                1 (search_)
                      148 LOAD_FAST                7 (buffer_dir)
                      150 LOAD_FAST                0 (input_data)
                      152 PRECALL                  4
                      156 CALL                     4
          
           46         166 LOAD_FAST                2 (entries)
          
@@ -359,34 +359,34 @@
            372 to 378 -> 380 [4] lasti
            380 to 384 -> 420 [1] lasti
            386 to 386 -> 380 [4] lasti
            388 to 392 -> 420 [1] lasti
            420 to 426 -> 428 [3] lasti
            434 to 434 -> 428 [3] lasti
          consts
-            '\n    Performs parallel search on given input data using a specified search algorithm, and\n    outputs the result in chunks. This function is useful for large datasets where searching\n    needs to be distributed among multiple processor cores for optimized performance.\n\n    Args:\n        input_data (Sequence[InputData[DataType]]): The input data sequence to perform the search on.\n        search (Search[Position, DataType]): The search algorithm to use.\n        entries (Iterable[Sequence[Entry[Position, DataType]]]): An iterable of entries to search from.\n        processes (int, optional): The number of worker processes to use. If not provided,\n                        it defaults to the number of processors on the machine.\n        chunk_size (int, optional): The number of tasks each worker process will be assigned at one time.\n                        Large chunk sizes are more efficient for large tasks (due to reduced overhead),\n                        but can lead to imbalanced workloads. The default value is 1000.\n\n    Returns:\n        Iterable[dict[str, Any]]: An iterable of the results.\n    '
+            '\n    Performs parallel search on given input data using a specified search algorithm, and\n    outputs the result in chunks. This function is useful for large datasets where searching\n    needs to be distributed among multiple processor cores for optimized performance.\n\n    Args:\n        input_data (Sequence[InputData[DataType]]): The input data sequence to perform the search on.\n        search_ (Search[Position, DataType]): The search algorithm to use.\n        entries (Iterable[Sequence[Entry[Position, DataType]]]): An iterable of entries to search from.\n        processes (int, optional): The number of worker processes to use. If not provided,\n                        it defaults to the number of processors on the machine.\n        chunk_size (int, optional): The number of tasks each worker process will be assigned at one time.\n                        Large chunk sizes are more efficient for large tasks (due to reduced overhead),\n                        but can lead to imbalanced workloads. The default value is 1000.\n\n    Returns:\n        Iterable[dict[str, Any]]: An iterable of the results.\n    '
             ('chunksize',)
             'utf-8'
             'surrogateescape'
             ('encoding', 'errors')
             None
          names      ('Pool', 'TemporaryDirectory', 'Path', 'imap_unordered', 'partial', 'buffered_search', 'open', 'map', 'loads')
-         varnames   ('input_data', 'search', 'entries', 'processes', 'chunk_size', 'pool', 'temp_dir', 'buffer_dir', 'result_file', 'src', 'result')
+         varnames   ('input_data', 'search_', 'entries', 'processes', 'chunk_size', 'pool', 'temp_dir', 'buffer_dir', 'result_file', 'src', 'result')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/parallel.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/parallel.py'
          name       'parallel_search'
          firstlineno 16
          lnotab
             0x061920011e011e0118012c01020102fd160530012e010aff02ff30fb02
             fe2eff
       None
-   names      ('collections.abc', 'Sequence', 'Iterable', 'functools', 'partial', 'json', 'loads', 'multiprocessing', 'cpu_count', 'multiprocessing.pool', 'Pool', 'pathlib', 'Path', 'tempfile', 'TemporaryDirectory', 'typing', 'Any', 'whereisit.ports.source', 'Position', 'DataType', 'whereisit.search.base', 'Search', 'buffered_search', 'whereisit.types.entry', 'Entry', 'whereisit.types.input_data', 'InputData', 'int', 'dict', 'str', 'parallel_search')
+   names      ('collections.abc', 'Sequence', 'Iterable', 'functools', 'partial', 'json', 'loads', 'multiprocessing', 'cpu_count', 'multiprocessing.pool', 'Pool', 'pathlib', 'Path', 'tempfile', 'TemporaryDirectory', 'typing', 'Any', 'findanywhere.ports.source', 'Position', 'DataType', 'findanywhere.search.base', 'Search', 'buffered_search', 'findanywhere.types.entry', 'Entry', 'findanywhere.types.input_data', 'InputData', 'int', 'dict', 'str', 'parallel_search')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/parallel.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/parallel.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020110010c010c010c010c010c010c010c02100110010c010c0712
       0102fb04011aff020212fe02032afd020402fc020502fb02061efa
```

### Comparing `findanywhere-0.1.0/whereisit/search/__pycache__/sequential.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/search/__pycache__/sequential.cpython-311.pyc`

 * *Files 25% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xe3f05166 (Sat May 25 14:08:35 2024 UTC)
-files sz: 1414
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 1426
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -38,29 +38,29 @@
                 34 IMPORT_NAME              5 (typing)
                 36 IMPORT_FROM              6 (Any)
                 38 STORE_NAME               6 (Any)
                 40 POP_TOP
    
      5          42 LOAD_CONST               0 (0)
                 44 LOAD_CONST               4 (('Search',))
-                46 IMPORT_NAME              7 (whereisit.search.base)
+                46 IMPORT_NAME              7 (findanywhere.search.base)
                 48 IMPORT_FROM              8 (Search)
                 50 STORE_NAME               8 (Search)
                 52 POP_TOP
    
      6          54 LOAD_CONST               0 (0)
                 56 LOAD_CONST               5 (('Entry',))
-                58 IMPORT_NAME              9 (whereisit.types.entry)
+                58 IMPORT_NAME              9 (findanywhere.types.entry)
                 60 IMPORT_FROM             10 (Entry)
                 62 STORE_NAME              10 (Entry)
                 64 POP_TOP
    
      7          66 LOAD_CONST               0 (0)
                 68 LOAD_CONST               6 (('InputData', 'DataType', 'Position'))
-                70 IMPORT_NAME             11 (whereisit.types.input_data)
+                70 IMPORT_NAME             11 (findanywhere.types.input_data)
                 72 IMPORT_FROM             12 (InputData)
                 74 STORE_NAME              12 (InputData)
                 76 IMPORT_FROM             13 (DataType)
                 78 STORE_NAME              13 (DataType)
                 80 IMPORT_FROM             14 (Position)
                 82 STORE_NAME              14 (Position)
                 84 POP_TOP
@@ -69,15 +69,15 @@
    
     11          88 LOAD_NAME                1 (Sequence)
                 90 LOAD_NAME               12 (InputData)
                 92 LOAD_NAME               13 (DataType)
                 94 BINARY_SUBSCR
                104 BINARY_SUBSCR
    
-    10         114 LOAD_CONST               8 ('search')
+    10         114 LOAD_CONST               8 ('search_')
    
     12         116 LOAD_NAME                8 (Search)
                118 LOAD_NAME               14 (Position)
                120 LOAD_NAME               13 (DataType)
                122 BUILD_TUPLE              2
                124 BINARY_SUBSCR
    
@@ -100,29 +100,29 @@
                184 LOAD_NAME               16 (str)
                186 LOAD_NAME                6 (Any)
                188 BUILD_TUPLE              2
                190 BINARY_SUBSCR
                200 BINARY_SUBSCR
    
     10         210 BUILD_TUPLE              8
-               212 LOAD_CONST              11 (<code object sequential_search, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/sequential.py", line 10>)
+               212 LOAD_CONST              11 (<code object sequential_search, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/sequential.py", line 10>)
                214 MAKE_FUNCTION            4 (annotations)
                216 STORE_NAME              17 (sequential_search)
                218 LOAD_CONST              12 (None)
                220 RETURN_VALUE
    consts
       0
       ('Sequence', 'Iterable')
       ('asdict',)
       ('Any',)
       ('Search',)
       ('Entry',)
       ('InputData', 'DataType', 'Position')
       'input_data'
-      'search'
+      'search_'
       'entries'
       'return'
       code
          argcount  : 3
          nlocals   : 5
          stacksize : 8
          flags     : 35
@@ -139,15 +139,15 @@
                        8 GET_ITER
                  >>   10 FOR_ITER                40 (to 92)
                       12 STORE_FAST               3 (entry)
          
           32          14 LOAD_GLOBAL              1 (NULL + map)
                       26 LOAD_GLOBAL              2 (asdict)
                       38 PUSH_NULL
-                      40 LOAD_FAST                1 (search)
+                      40 LOAD_FAST                1 (search_)
                       42 LOAD_FAST                0 (input_data)
                       44 LOAD_FAST                3 (entry)
                       46 PRECALL                  2
                       50 CALL                     2
                       60 PRECALL                  2
                       64 CALL                     2
                       74 GET_ITER
@@ -161,28 +161,28 @@
                       88 JUMP_BACKWARD            7 (to 76)
          
           32     >>   90 JUMP_BACKWARD           41 (to 10)
          
           31     >>   92 LOAD_CONST               1 (None)
                       94 RETURN_VALUE
          consts
-            '\n    Perform sequential search on the given input data using the specified search algorithm.\n\n    Unlike parallel search, this function processes the input data and entries sequentially,\n    which could be better for small data sets or for systems with single or limited processor cores.\n\n    Args:\n        input_data: A sequence of InputData objects containing data of a specific type.\n        search: A search function that takes input_data and an entry as parameters and returns a sequence of matches.\n        entries: An iterable of sequences of Entry objects containing positions and data to search for.\n\n    Returns:\n        An iterable of dictionaries, where each dictionary represents a match found by the search function. The\n        dictionaries contain attributes and values corresponding to the matched Entry objects.\n\n    '
+            '\n    Perform sequential search on the given input data using the specified search algorithm.\n\n    Unlike parallel search, this function processes the input data and entries sequentially,\n    which could be better for small data sets or for systems with single or limited processor cores.\n\n    Args:\n        input_data: A sequence of InputData objects containing data of a specific type.\n        search_: A search function that takes input_data and an entry as parameters and returns a sequence of matches.\n        entries: An iterable of sequences of Entry objects containing positions and data to search for.\n\n    Returns:\n        An iterable of dictionaries, where each dictionary represents a match found by the search function. The\n        dictionaries contain attributes and values corresponding to the matched Entry objects.\n\n    '
             None
          names      ('map', 'asdict')
-         varnames   ('input_data', 'search', 'entries', 'entry', 'result')
+         varnames   ('input_data', 'search_', 'entries', 'entry', 'result')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/sequential.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/sequential.py'
          name       'sequential_search'
          firstlineno 10
          lnotab 0x0615080142010aff02ff
       None
-   names      ('collections.abc', 'Sequence', 'Iterable', 'dataclasses', 'asdict', 'typing', 'Any', 'whereisit.search.base', 'Search', 'whereisit.types.entry', 'Entry', 'whereisit.types.input_data', 'InputData', 'DataType', 'Position', 'dict', 'str', 'sequential_search')
+   names      ('collections.abc', 'Sequence', 'Iterable', 'dataclasses', 'asdict', 'typing', 'Any', 'findanywhere.search.base', 'Search', 'findanywhere.types.entry', 'Entry', 'findanywhere.types.input_data', 'InputData', 'DataType', 'Position', 'dict', 'str', 'sequential_search')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/search/sequential.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/search/sequential.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020110010c010c020c010c01140302011aff020212fe02032afd02
       041efc
```

### Comparing `findanywhere-0.1.0/whereisit/search/base.py` & `findanywhere-1.0.0/findanywhere/search/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 from collections.abc import Sequence, Iterable
 from dataclasses import asdict
 from json import dump
 from pathlib import Path
 from typing import Protocol, Any
 from uuid import uuid4
 
-from whereisit.ports.evaluation import EvaluationAdapter, Position
-from whereisit.types.entry import Entry
-from whereisit.types.input_data import InputData, DataType
-from whereisit.types.similarity import DeduceScore, ThresholdFilter, ScoredEvaluation
+from findanywhere.ports.evaluation import EvaluationAdapter, Position
+from findanywhere.types.entry import Entry
+from findanywhere.types.input_data import InputData, DataType
+from findanywhere.types.similarity import DeduceScore, ThresholdFilter, ScoredEvaluation
 
 
 def search(
         evaluate: EvaluationAdapter[DataType],
         deduce_score: DeduceScore[Position, DataType],
         threshold: ThresholdFilter[Position, DataType],
         input_data: Sequence[InputData[DataType]],
```

### Comparing `findanywhere-0.1.0/whereisit/search/parallel.py` & `findanywhere-1.0.0/findanywhere/search/parallel.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from json import loads
 from multiprocessing import cpu_count
 from multiprocessing.pool import Pool
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any
 
-from whereisit.ports.source import Position, DataType
-from whereisit.search.base import Search, buffered_search
-from whereisit.types.entry import Entry
-from whereisit.types.input_data import InputData
+from findanywhere.ports.source import Position, DataType
+from findanywhere.search.base import Search, buffered_search
+from findanywhere.types.entry import Entry
+from findanywhere.types.input_data import InputData
 
 
 def parallel_search(
         input_data: Sequence[InputData[DataType]],
         search_: Search[Position, DataType],
         entries: Iterable[Sequence[Entry[Position, DataType]]],
         processes: int = cpu_count(),
```

### Comparing `findanywhere-0.1.0/whereisit/search/sequential.py` & `findanywhere-1.0.0/findanywhere/search/sequential.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections.abc import Sequence, Iterable
 from dataclasses import asdict
 from typing import Any
 
-from whereisit.search.base import Search
-from whereisit.types.entry import Entry
-from whereisit.types.input_data import InputData, DataType, Position
+from findanywhere.search.base import Search
+from findanywhere.types.entry import Entry
+from findanywhere.types.input_data import InputData, DataType, Position
 
 
 def sequential_search(
     input_data: Sequence[InputData[DataType]],
     search_: Search[Position, DataType],
     entries: Iterable[Sequence[Entry[Position, DataType]]],
 ) -> Iterable[dict[str, Any]]:
```

### Comparing `findanywhere-0.1.0/whereisit/similarity/__init__.py` & `findanywhere-1.0.0/findanywhere/similarity/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections.abc import Callable, Sequence
 
-from whereisit.similarity.common import inverted_levenshtein_distance_with, jaro_winkler_similarity_with
-from whereisit.similarity.token import token_best_fit_similarity_with, token_best_fit_mulit_separator_similarity_with
-from whereisit.types.factory import FactoryMap, Factory, Config
-from whereisit.types.similarity import Similarity
+from findanywhere.similarity.common import inverted_levenshtein_distance_with, jaro_winkler_similarity_with
+from findanywhere.similarity.token import token_best_fit_similarity_with, token_best_fit_mulit_separator_similarity_with
+from findanywhere.types.factory import FactoryMap, Factory, Config
+from findanywhere.types.similarity import Similarity
 
 
 SIMILARITY_FACTORIES: FactoryMap[Similarity[str]] = FactoryMap[Similarity[str]](
     [
         inverted_levenshtein_distance_with, jaro_winkler_similarity_with,
         token_best_fit_similarity_with, token_best_fit_mulit_separator_similarity_with
     ]
```

### Comparing `findanywhere-0.1.0/whereisit/similarity/__pycache__/__init__.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/similarity/__pycache__/__init__.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x55244b66 (Mon May 20 10:22:13 2024 UTC)
-files sz: 984
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 996
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x97005500640064016c006d015a016d025a020100640064026c036d045a
@@ -29,44 +29,44 @@
                 12 STORE_NAME               1 (Callable)
                 14 IMPORT_FROM              2 (Sequence)
                 16 STORE_NAME               2 (Sequence)
                 18 POP_TOP
    
      3          20 LOAD_CONST               0 (0)
                 22 LOAD_CONST               2 (('inverted_levenshtein_distance_with', 'jaro_winkler_similarity_with'))
-                24 IMPORT_NAME              3 (whereisit.similarity.common)
+                24 IMPORT_NAME              3 (findanywhere.similarity.common)
                 26 IMPORT_FROM              4 (inverted_levenshtein_distance_with)
                 28 STORE_NAME               4 (inverted_levenshtein_distance_with)
                 30 IMPORT_FROM              5 (jaro_winkler_similarity_with)
                 32 STORE_NAME               5 (jaro_winkler_similarity_with)
                 34 POP_TOP
    
      4          36 LOAD_CONST               0 (0)
                 38 LOAD_CONST               3 (('token_best_fit_similarity_with', 'token_best_fit_mulit_separator_similarity_with'))
-                40 IMPORT_NAME              6 (whereisit.similarity.token)
+                40 IMPORT_NAME              6 (findanywhere.similarity.token)
                 42 IMPORT_FROM              7 (token_best_fit_similarity_with)
                 44 STORE_NAME               7 (token_best_fit_similarity_with)
                 46 IMPORT_FROM              8 (token_best_fit_mulit_separator_similarity_with)
                 48 STORE_NAME               8 (token_best_fit_mulit_separator_similarity_with)
                 50 POP_TOP
    
      5          52 LOAD_CONST               0 (0)
                 54 LOAD_CONST               4 (('FactoryMap', 'Factory', 'Config'))
-                56 IMPORT_NAME              9 (whereisit.types.factory)
+                56 IMPORT_NAME              9 (findanywhere.types.factory)
                 58 IMPORT_FROM             10 (FactoryMap)
                 60 STORE_NAME              10 (FactoryMap)
                 62 IMPORT_FROM             11 (Factory)
                 64 STORE_NAME              11 (Factory)
                 66 IMPORT_FROM             12 (Config)
                 68 STORE_NAME              12 (Config)
                 70 POP_TOP
    
      6          72 LOAD_CONST               0 (0)
                 74 LOAD_CONST               5 (('Similarity',))
-                76 IMPORT_NAME             13 (whereisit.types.similarity)
+                76 IMPORT_NAME             13 (findanywhere.types.similarity)
                 78 IMPORT_FROM             14 (Similarity)
                 80 STORE_NAME              14 (Similarity)
                 82 POP_TOP
    
      9          84 PUSH_NULL
                 86 LOAD_NAME               10 (FactoryMap)
                 88 LOAD_NAME               14 (Similarity)
@@ -92,15 +92,15 @@
                154 BINARY_SUBSCR
                164 LOAD_NAME               17 (__annotations__)
                166 LOAD_CONST               6 ('SIMILARITY_FACTORIES')
                168 STORE_SUBSCR
    
     17         172 PUSH_NULL
                174 LOAD_NAME               18 (dict)
-               176 LOAD_CONST               7 (<code object <genexpr>, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/__init__.py", line 17>)
+               176 LOAD_CONST               7 (<code object <genexpr>, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/__init__.py", line 17>)
                178 MAKE_FUNCTION            0
    
     19         180 LOAD_NAME               19 (max)
                182 LOAD_NAME               20 (min)
                184 BUILD_TUPLE              2
    
     17         186 GET_ITER
@@ -130,15 +130,15 @@
                278 LOAD_CONST              10 ('return')
                280 LOAD_NAME               11 (Factory)
                282 LOAD_NAME               14 (Similarity)
                284 LOAD_NAME               12 (Config)
                286 BUILD_TUPLE              2
                288 BINARY_SUBSCR
                298 BUILD_TUPLE              4
-               300 LOAD_CONST              11 (<code object get_similarity_factory, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/__init__.py", line 23>)
+               300 LOAD_CONST              11 (<code object get_similarity_factory, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/__init__.py", line 23>)
                302 MAKE_FUNCTION            4 (annotations)
                304 STORE_NAME              23 (get_similarity_factory)
    
     28         306 LOAD_CONST               9 ('name')
                308 LOAD_NAME               15 (str)
                310 LOAD_CONST              10 ('return')
                312 LOAD_NAME                1 (Callable)
@@ -146,15 +146,15 @@
                316 LOAD_NAME               22 (float)
                318 BINARY_SUBSCR
                328 BUILD_LIST               1
                330 LOAD_NAME               22 (float)
                332 BUILD_TUPLE              2
                334 BINARY_SUBSCR
                344 BUILD_TUPLE              4
-               346 LOAD_CONST              12 (<code object get_aggregate_by_name, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/__init__.py", line 28>)
+               346 LOAD_CONST              12 (<code object get_aggregate_by_name, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/__init__.py", line 28>)
                348 MAKE_FUNCTION            4 (annotations)
                350 STORE_NAME              24 (get_aggregate_by_name)
                352 LOAD_CONST              13 (None)
                354 RETURN_VALUE
    consts
       0
       ('Callable', 'Sequence')
@@ -192,15 +192,15 @@
                       38 RETURN_VALUE
          consts
             None
          names      ('__name__',)
          varnames   ('.0', 'func')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/__init__.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/__init__.py'
          name       '<genexpr>'
          firstlineno 17
          lnotab 0x0a0202ff10ff
       '_AGGREGATES'
       'name'
       'return'
       code
@@ -217,15 +217,15 @@
                       26 RETURN_VALUE
          consts
             None
          names      ('SIMILARITY_FACTORIES',)
          varnames   ('name',)
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/__init__.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/__init__.py'
          name       'get_similarity_factory'
          firstlineno 23
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
@@ -239,22 +239,22 @@
                       26 RETURN_VALUE
          consts
             None
          names      ('_AGGREGATES',)
          varnames   ('name',)
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/__init__.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/__init__.py'
          name       'get_aggregate_by_name'
          firstlineno 28
          lnotab 0x0201
       None
-   names      ('collections.abc', 'Callable', 'Sequence', 'whereisit.similarity.common', 'inverted_levenshtein_distance_with', 'jaro_winkler_similarity_with', 'whereisit.similarity.token', 'token_best_fit_similarity_with', 'token_best_fit_mulit_separator_similarity_with', 'whereisit.types.factory', 'FactoryMap', 'Factory', 'Config', 'whereisit.types.similarity', 'Similarity', 'str', 'SIMILARITY_FACTORIES', '__annotations__', 'dict', 'max', 'min', '_AGGREGATES', 'float', 'get_similarity_factory', 'get_aggregate_by_name')
+   names      ('collections.abc', 'Callable', 'Sequence', 'findanywhere.similarity.common', 'inverted_levenshtein_distance_with', 'jaro_winkler_similarity_with', 'findanywhere.similarity.token', 'token_best_fit_similarity_with', 'token_best_fit_mulit_separator_similarity_with', 'findanywhere.types.factory', 'FactoryMap', 'Factory', 'Config', 'findanywhere.types.similarity', 'Similarity', 'str', 'SIMILARITY_FACTORIES', '__annotations__', 'dict', 'max', 'min', '_AGGREGATES', 'float', 'get_similarity_factory', 'get_aggregate_by_name')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/__init__.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020112021001100114010c031c02040104fe02ff3208080206fe58
       062005
```

### Comparing `findanywhere-0.1.0/whereisit/similarity/__pycache__/common.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/similarity/__pycache__/common.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xe2f05166 (Sat May 25 14:08:34 2024 UTC)
-files sz: 1767
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 1773
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a046d
@@ -24,36 +24,36 @@
                 10 STORE_NAME               1 (jaro_winkler_similarity)
                 12 IMPORT_FROM              2 (levenshtein_distance)
                 14 STORE_NAME               2 (levenshtein_distance)
                 16 POP_TOP
    
      3          18 LOAD_CONST               0 (0)
                 20 LOAD_CONST               2 (('as_factory', 'Config'))
-                22 IMPORT_NAME              3 (whereisit.types.factory)
+                22 IMPORT_NAME              3 (findanywhere.types.factory)
                 24 IMPORT_FROM              4 (as_factory)
                 26 STORE_NAME               4 (as_factory)
                 28 IMPORT_FROM              5 (Config)
                 30 STORE_NAME               5 (Config)
                 32 POP_TOP
    
      4          34 LOAD_CONST               0 (0)
                 36 LOAD_CONST               3 (('Similarity',))
-                38 IMPORT_NAME              6 (whereisit.types.similarity)
+                38 IMPORT_NAME              6 (findanywhere.types.similarity)
                 40 IMPORT_FROM              7 (Similarity)
                 42 STORE_NAME               7 (Similarity)
                 44 POP_TOP
    
      7          46 LOAD_CONST               4 ('left')
                 48 LOAD_NAME                8 (str)
                 50 LOAD_CONST               5 ('right')
                 52 LOAD_NAME                8 (str)
                 54 LOAD_CONST               6 ('return')
                 56 LOAD_NAME                9 (float)
                 58 BUILD_TUPLE              6
-                60 LOAD_CONST               7 (<code object jaro_winkler, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/common.py", line 7>)
+                60 LOAD_CONST               7 (<code object jaro_winkler, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/common.py", line 7>)
                 62 MAKE_FUNCTION            4 (annotations)
                 64 STORE_NAME              10 (jaro_winkler)
    
     21          66 PUSH_NULL
                 68 LOAD_NAME                4 (as_factory)
                 70 LOAD_CONST               8 ('jaro_winkler')
                 72 LOAD_NAME               10 (jaro_winkler)
@@ -64,30 +64,30 @@
     22          90 LOAD_CONST              10 ('config')
                 92 LOAD_NAME                5 (Config)
                 94 LOAD_CONST               6 ('return')
                 96 LOAD_NAME                7 (Similarity)
                 98 LOAD_NAME                8 (str)
                100 BINARY_SUBSCR
                110 BUILD_TUPLE              4
-               112 LOAD_CONST              11 (<code object jaro_winkler_similarity_with, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/common.py", line 21>)
+               112 LOAD_CONST              11 (<code object jaro_winkler_similarity_with, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/common.py", line 21>)
                114 MAKE_FUNCTION            4 (annotations)
    
     21         116 PRECALL                  0
                120 CALL                     0
    
     22         130 STORE_NAME              11 (jaro_winkler_similarity_with)
    
     35         132 LOAD_CONST               4 ('left')
                134 LOAD_NAME                8 (str)
                136 LOAD_CONST               5 ('right')
                138 LOAD_NAME                8 (str)
                140 LOAD_CONST               6 ('return')
                142 LOAD_NAME                9 (float)
                144 BUILD_TUPLE              6
-               146 LOAD_CONST              12 (<code object inverted_levenshtein_distance, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/common.py", line 35>)
+               146 LOAD_CONST              12 (<code object inverted_levenshtein_distance, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/common.py", line 35>)
                148 MAKE_FUNCTION            4 (annotations)
                150 STORE_NAME              12 (inverted_levenshtein_distance)
    
     49         152 PUSH_NULL
                154 LOAD_NAME                4 (as_factory)
                156 LOAD_CONST              13 ('inverted_levenshtein')
                158 LOAD_NAME               12 (inverted_levenshtein_distance)
@@ -98,15 +98,15 @@
     50         176 LOAD_CONST              10 ('config')
                178 LOAD_NAME                5 (Config)
                180 LOAD_CONST               6 ('return')
                182 LOAD_NAME                7 (Similarity)
                184 LOAD_NAME                8 (str)
                186 BINARY_SUBSCR
                196 BUILD_TUPLE              4
-               198 LOAD_CONST              14 (<code object inverted_levenshtein_distance_with, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/common.py", line 49>)
+               198 LOAD_CONST              14 (<code object inverted_levenshtein_distance_with, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/common.py", line 49>)
                200 MAKE_FUNCTION            4 (annotations)
    
     49         202 PRECALL                  0
                206 CALL                     0
    
     50         216 STORE_NAME              13 (inverted_levenshtein_distance_with)
                218 LOAD_CONST              15 (None)
@@ -137,15 +137,15 @@
                       32 RETURN_VALUE
          consts
             '\n    Jaro-Winkler Similarity using the parameters and implementation of the library jellyfish\n\n    Args:\n        left: String to search\n        right: String to compare\n\n    Returns:\n        Value from [0.0, 1.0] with higher values indicating higher similarities.\n    '
          names      ('jaro_winkler_similarity',)
          varnames   ('left', 'right')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/common.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/common.py'
          name       'jaro_winkler'
          firstlineno 7
          lnotab 0x020b
       'jaro_winkler'
       ('using',)
       'config'
       code
@@ -160,15 +160,15 @@
                       14 RETURN_VALUE
          consts
             '\n    Args:\n        config: The configuration object that contains the necessary information for calculating Jaro-Winkler\n        similarity.\n\n    Returns:\n        Similarity[str]: The calculated Jaro-Winkler similarity between two strings.\n\n    '
          names      ('jaro_winkler',)
          varnames   ('config',)
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/common.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/common.py'
          name       'jaro_winkler_similarity_with'
          firstlineno 21
          lnotab 0x020b
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
@@ -189,15 +189,15 @@
          consts
             '\n    Negative Levenshtein Distance.\n\n    Args:\n        left: String to search\n        right: String to compare\n\n    Returns:\n        Value from ]-infinity, 0.0] with higher values indicating higher similarities.\n    '
             -1
          names      ('levenshtein_distance',)
          varnames   ('left', 'right')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/common.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/common.py'
          name       'inverted_levenshtein_distance'
          firstlineno 35
          lnotab 0x020b
       'inverted_levenshtein'
       code
          argcount  : 1
          nlocals   : 1
@@ -210,20 +210,20 @@
                       14 RETURN_VALUE
          consts
             '\n    Args:\n        config: The configuration object that contains the necessary parameters for calculating the inverted Levenshtein\n        distance.\n\n    Returns:\n        Similarity[str]: A similarity object calculating the inverted Levenshtein distance value.\n\n    '
          names      ('inverted_levenshtein_distance',)
          varnames   ('config',)
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/common.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/common.py'
          name       'inverted_levenshtein_distance_with'
          firstlineno 49
          lnotab 0x020b
       None
-   names      ('jellyfish', 'jaro_winkler_similarity', 'levenshtein_distance', 'whereisit.types.factory', 'as_factory', 'Config', 'whereisit.types.similarity', 'Similarity', 'str', 'float', 'jaro_winkler', 'jaro_winkler_similarity_with', 'inverted_levenshtein_distance', 'inverted_levenshtein_distance_with')
+   names      ('jellyfish', 'jaro_winkler_similarity', 'levenshtein_distance', 'findanywhere.types.factory', 'as_factory', 'Config', 'findanywhere.types.similarity', 'Similarity', 'str', 'float', 'jaro_winkler', 'jaro_winkler_similarity_with', 'inverted_levenshtein_distance', 'inverted_levenshtein_distance_with')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/common.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/common.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201100210010c03140e18011aff0e01020d140e18011aff0e01
```

### Comparing `findanywhere-0.1.0/whereisit/similarity/__pycache__/token.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/similarity/__pycache__/token.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x0cf15166 (Sat May 25 14:09:16 2024 UTC)
-files sz: 3606
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 3615
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a0401
@@ -59,31 +59,31 @@
                 58 IMPORT_NAME              9 (jellyfish)
                 60 IMPORT_FROM             10 (jaro_winkler_similarity)
                 62 STORE_NAME              10 (jaro_winkler_similarity)
                 64 POP_TOP
    
      8          66 LOAD_CONST               0 (0)
                 68 LOAD_CONST               6 (('split',))
-                70 IMPORT_NAME             11 (whereisit.algorithms.strings)
+                70 IMPORT_NAME             11 (findanywhere.algorithms.strings)
                 72 IMPORT_FROM             12 (split)
                 74 STORE_NAME              12 (split)
                 76 POP_TOP
    
      9          78 LOAD_CONST               0 (0)
                 80 LOAD_CONST               7 (('as_factory', 'Config'))
-                82 IMPORT_NAME             13 (whereisit.types.factory)
+                82 IMPORT_NAME             13 (findanywhere.types.factory)
                 84 IMPORT_FROM             14 (as_factory)
                 86 STORE_NAME              14 (as_factory)
                 88 IMPORT_FROM             15 (Config)
                 90 STORE_NAME              15 (Config)
                 92 POP_TOP
    
     10          94 LOAD_CONST               0 (0)
                 96 LOAD_CONST               8 (('Similarity',))
-                98 IMPORT_NAME             16 (whereisit.types.similarity)
+                98 IMPORT_NAME             16 (findanywhere.types.similarity)
                100 IMPORT_FROM             17 (Similarity)
                102 STORE_NAME              17 (Similarity)
                104 POP_TOP
    
     20         106 LOAD_CONST               9 (None)
    
     16         108 LOAD_CONST              10 (('delimiter',))
@@ -103,28 +103,28 @@
                126 BINARY_OP                7 (|)
    
     16         130 LOAD_CONST              14 ('return')
    
     21         132 LOAD_NAME               19 (float)
    
     16         134 BUILD_TUPLE              8
-               136 LOAD_CONST              15 (<code object token_best_fit_similarity, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py", line 16>)
+               136 LOAD_CONST              15 (<code object token_best_fit_similarity, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py", line 16>)
                138 MAKE_FUNCTION            6 (kwdefaults, annotations)
                140 STORE_NAME              20 (token_best_fit_similarity)
    
     56         142 PUSH_NULL
                144 LOAD_NAME                3 (dataclass)
                146 LOAD_CONST              16 (True)
                148 KW_NAMES                17
                150 PRECALL                  1
                154 CALL                     1
    
     57         164 PUSH_NULL
                166 LOAD_BUILD_CLASS
-               168 LOAD_CONST              18 (<code object TokenBestFitConfig, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py", line 56>)
+               168 LOAD_CONST              18 (<code object TokenBestFitConfig, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py", line 56>)
                170 MAKE_FUNCTION            0
                172 LOAD_CONST              19 ('TokenBestFitConfig')
                174 LOAD_NAME               15 (Config)
                176 PRECALL                  3
                180 CALL                     3
    
     56         190 PRECALL                  0
@@ -143,15 +143,15 @@
     71         230 LOAD_CONST              22 ('config')
                232 LOAD_NAME               21 (TokenBestFitConfig)
                234 LOAD_CONST              14 ('return')
                236 LOAD_NAME               17 (Similarity)
                238 LOAD_NAME               18 (str)
                240 BINARY_SUBSCR
                250 BUILD_TUPLE              4
-               252 LOAD_CONST              23 (<code object token_best_fit_similarity_with, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py", line 70>)
+               252 LOAD_CONST              23 (<code object token_best_fit_similarity_with, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py", line 70>)
                254 MAKE_FUNCTION            4 (annotations)
    
     70         256 PRECALL                  0
                260 CALL                     0
    
     71         270 STORE_NAME              22 (token_best_fit_similarity_with)
    
@@ -174,28 +174,28 @@
                292 BINARY_SUBSCR
    
     78         302 LOAD_CONST              14 ('return')
    
     83         304 LOAD_NAME               19 (float)
    
     78         306 BUILD_TUPLE              8
-               308 LOAD_CONST              26 (<code object token_best_fit_multi_separator_similarity, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py", line 78>)
+               308 LOAD_CONST              26 (<code object token_best_fit_multi_separator_similarity, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py", line 78>)
                310 MAKE_FUNCTION            6 (kwdefaults, annotations)
                312 STORE_NAME              23 (token_best_fit_multi_separator_similarity)
    
     94         314 PUSH_NULL
                316 LOAD_NAME                3 (dataclass)
                318 LOAD_CONST              16 (True)
                320 KW_NAMES                17
                322 PRECALL                  1
                326 CALL                     1
    
     95         336 PUSH_NULL
                338 LOAD_BUILD_CLASS
-               340 LOAD_CONST              27 (<code object TokenBestFitMultiSeparatorConfig, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py", line 94>)
+               340 LOAD_CONST              27 (<code object TokenBestFitMultiSeparatorConfig, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py", line 94>)
                342 MAKE_FUNCTION            0
                344 LOAD_CONST              28 ('TokenBestFitMultiSeparatorConfig')
                346 LOAD_NAME               15 (Config)
                348 PRECALL                  3
                352 CALL                     3
    
     94         362 PRECALL                  0
@@ -213,15 +213,15 @@
    100         400 LOAD_CONST              22 ('config')
                402 LOAD_NAME               24 (TokenBestFitMultiSeparatorConfig)
                404 LOAD_CONST              14 ('return')
                406 LOAD_NAME               17 (Similarity)
                408 LOAD_NAME               18 (str)
                410 BINARY_SUBSCR
                420 BUILD_TUPLE              4
-               422 LOAD_CONST              30 (<code object token_best_fit_mulit_separator_similarity_with, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py", line 99>)
+               422 LOAD_CONST              30 (<code object token_best_fit_mulit_separator_similarity_with, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py", line 99>)
                424 MAKE_FUNCTION            4 (annotations)
    
     99         426 PRECALL                  0
                430 CALL                     0
    
    100         440 STORE_NAME              25 (token_best_fit_mulit_separator_similarity_with)
                442 LOAD_CONST               9 (None)
@@ -317,15 +317,15 @@
             0.0
             1.0
             ('default',)
          names      ('split', 'max', 'map', 'partial', 'jaro_winkler_similarity', 'len')
          varnames   ('left', 'right', 'delimiter', 'left_tokens', 'right_tokens', 'similarity', 'token')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py'
          name       'token_best_fit_similarity'
          firstlineno 16
          lnotab 0x021e2001200104010401040108016c01
       True
       ('frozen',)
       code
          argcount  : 0
@@ -360,15 +360,15 @@
             '\n\n    The TokenBestFitConfig class is a configuration class that inherits from the Config base class. It is used to\n    specify the configuration for the token best fit algorithm.\n\n    Attributes:\n    - delimiter (str | None): The delimiter used for tokenization. It can be a string or None if whitespace.\n\n    '
             None
             'delimiter'
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'delimiter', 'str', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py'
          name       'TokenBestFitConfig'
          firstlineno 56
          lnotab 0x0c020409
       'TokenBestFitConfig'
       'token_best_fit_similarity'
       ('using',)
       'config'
@@ -396,15 +396,15 @@
          consts
             None
             ('delimiter',)
          names      ('partial', 'token_best_fit_similarity', 'delimiter')
          varnames   ('config',)
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py'
          name       'token_best_fit_similarity_with'
          firstlineno 70
          lnotab 0x02020c010c010cfe
       ('delimiters',)
       'delimiters'
       code
          argcount  : 2
@@ -489,15 +489,15 @@
             0.0
             1.0
             ('default',)
          names      ('split', 'set', 'max', 'map', 'partial', 'jaro_winkler_similarity', 'len')
          varnames   ('left', 'right', 'delimiters', 'left_tokens', 'right_tokens', 'similarity', 'token')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py'
          name       'token_best_fit_multi_separator_similarity'
          firstlineno 78
          lnotab 0x02063a013a0104010401040108016c01
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
@@ -511,15 +511,15 @@
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('TokenBestFitMultiSeparatorConfig')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
           96          12 PUSH_NULL
                       14 LOAD_NAME                3 (field)
-                      16 LOAD_CONST               1 (<code object <lambda>, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py", line 96>)
+                      16 LOAD_CONST               1 (<code object <lambda>, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py", line 96>)
                       18 MAKE_FUNCTION            0
                       20 KW_NAMES                 2
                       22 PRECALL                  1
                       26 CALL                     1
                       36 STORE_NAME               4 (delimiters)
                       38 LOAD_NAME                5 (str)
                       40 LOAD_NAME                6 (list)
@@ -549,26 +549,26 @@
                             40 RETURN_VALUE
                consts
                   None
                names      ('list', 'whitespace')
                varnames   ()
                freevars   ()
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py'
                name       '<lambda>'
                firstlineno 96
                lnotab 0x
             ('default_factory',)
             'delimiters'
             None
          names      ('__name__', '__module__', '__qualname__', 'field', 'delimiters', 'str', 'list', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py'
          name       'TokenBestFitMultiSeparatorConfig'
          firstlineno 94
          lnotab 0x0c02
       'TokenBestFitMultiSeparatorConfig'
       'token_best_fit_multi_separator_similarity'
       code
          argcount  : 1
@@ -591,23 +591,23 @@
          consts
             None
             ('delimiters',)
          names      ('partial', 'token_best_fit_multi_separator_similarity', 'delimiters')
          varnames   ('config',)
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py'
          name       'token_best_fit_mulit_separator_similarity_with'
          firstlineno 99
          lnotab 0x0202
-   names      ('collections.abc', 'Iterable', 'dataclasses', 'dataclass', 'field', 'functools', 'partial', 'string', 'whitespace', 'jellyfish', 'jaro_winkler_similarity', 'whereisit.algorithms.strings', 'split', 'whereisit.types.factory', 'as_factory', 'Config', 'whereisit.types.similarity', 'Similarity', 'str', 'float', 'token_best_fit_similarity', 'TokenBestFitConfig', 'token_best_fit_similarity_with', 'token_best_fit_multi_separator_similarity', 'TokenBestFitMultiSeparatorConfig', 'token_best_fit_mulit_separator_similarity_with')
+   names      ('collections.abc', 'Iterable', 'dataclasses', 'dataclass', 'field', 'functools', 'partial', 'string', 'whitespace', 'jellyfish', 'jaro_winkler_similarity', 'findanywhere.algorithms.strings', 'split', 'findanywhere.types.factory', 'as_factory', 'Config', 'findanywhere.types.similarity', 'Similarity', 'str', 'float', 'token_best_fit_similarity', 'TokenBestFitConfig', 'token_best_fit_similarity_with', 'token_best_fit_multi_separator_similarity', 'TokenBestFitMultiSeparatorConfig', 'token_best_fit_mulit_separator_similarity_with')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/similarity/token.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/similarity/token.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c0110010c010c020c020c0110010c0a02fc060102ff020202
       fe020408fc020502fb082816011aff0e01020d18011aff0e01020b02fc06
       0102ff020202fe02040efc020502fb081016011aff0e01020416011aff0e
       01
```

### Comparing `findanywhere-0.1.0/whereisit/similarity/common.py` & `findanywhere-1.0.0/findanywhere/similarity/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from jellyfish import jaro_winkler_similarity, levenshtein_distance
 
-from whereisit.types.factory import as_factory, Config
-from whereisit.types.similarity import Similarity
+from findanywhere.types.factory import as_factory, Config
+from findanywhere.types.similarity import Similarity
 
 
 def jaro_winkler(left: str, right: str) -> float:
     """
     Jaro-Winkler Similarity using the parameters and implementation of the library jellyfish
 
     Args:
```

### Comparing `findanywhere-0.1.0/whereisit/similarity/token.py` & `findanywhere-1.0.0/findanywhere/similarity/token.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from collections.abc import Iterable
 from dataclasses import dataclass, field
 from functools import partial
 from string import whitespace
 
 from jellyfish import jaro_winkler_similarity
 
-from whereisit.algorithms.strings import split
-from whereisit.types.factory import as_factory, Config
-from whereisit.types.similarity import Similarity
+from findanywhere.algorithms.strings import split
+from findanywhere.types.factory import as_factory, Config
+from findanywhere.types.similarity import Similarity
 
 
 
 
 
 def token_best_fit_similarity(
         left: str,
```

### Comparing `findanywhere-0.1.0/whereisit/thresholds/__pycache__/basic.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/thresholds/__pycache__/basic.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xe2f05166 (Sat May 25 14:08:34 2024 UTC)
-files sz: 2164
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 2173
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -32,33 +32,33 @@
                 18 IMPORT_NAME              2 (functools)
                 20 IMPORT_FROM              3 (partial)
                 22 STORE_NAME               3 (partial)
                 24 POP_TOP
    
      4          26 LOAD_CONST               0 (0)
                 28 LOAD_CONST               3 (('Position', 'DataType'))
-                30 IMPORT_NAME              4 (whereisit.types.entry)
+                30 IMPORT_NAME              4 (findanywhere.types.entry)
                 32 IMPORT_FROM              5 (Position)
                 34 STORE_NAME               5 (Position)
                 36 IMPORT_FROM              6 (DataType)
                 38 STORE_NAME               6 (DataType)
                 40 POP_TOP
    
      5          42 LOAD_CONST               0 (0)
                 44 LOAD_CONST               4 (('as_factory', 'Config'))
-                46 IMPORT_NAME              7 (whereisit.types.factory)
+                46 IMPORT_NAME              7 (findanywhere.types.factory)
                 48 IMPORT_FROM              8 (as_factory)
                 50 STORE_NAME               8 (as_factory)
                 52 IMPORT_FROM              9 (Config)
                 54 STORE_NAME               9 (Config)
                 56 POP_TOP
    
      6          58 LOAD_CONST               0 (0)
                 60 LOAD_CONST               5 (('ScoredEvaluation', 'ThresholdFilter'))
-                62 IMPORT_NAME             10 (whereisit.types.similarity)
+                62 IMPORT_NAME             10 (findanywhere.types.similarity)
                 64 IMPORT_FROM             11 (ScoredEvaluation)
                 66 STORE_NAME              11 (ScoredEvaluation)
                 68 IMPORT_FROM             12 (ThresholdFilter)
                 70 STORE_NAME              12 (ThresholdFilter)
                 72 POP_TOP
    
      9          74 LOAD_CONST               6 ('evaluation')
@@ -66,30 +66,30 @@
                 78 LOAD_NAME                5 (Position)
                 80 LOAD_NAME                6 (DataType)
                 82 BUILD_TUPLE              2
                 84 BINARY_SUBSCR
                 94 LOAD_CONST               7 ('return')
                 96 LOAD_NAME               13 (bool)
                 98 BUILD_TUPLE              4
-               100 LOAD_CONST               8 (<code object no_threshold, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/thresholds/basic.py", line 9>)
+               100 LOAD_CONST               8 (<code object no_threshold, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/thresholds/basic.py", line 9>)
                102 MAKE_FUNCTION            4 (annotations)
                104 STORE_NAME              14 (no_threshold)
    
     20         106 LOAD_CONST               9 ('constant')
                108 LOAD_NAME               15 (float)
                110 LOAD_CONST               6 ('evaluation')
                112 LOAD_NAME               11 (ScoredEvaluation)
                114 LOAD_NAME                5 (Position)
                116 LOAD_NAME                6 (DataType)
                118 BUILD_TUPLE              2
                120 BINARY_SUBSCR
                130 LOAD_CONST               7 ('return')
                132 LOAD_NAME               13 (bool)
                134 BUILD_TUPLE              6
-               136 LOAD_CONST              10 (<code object constant_threshold, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/thresholds/basic.py", line 20>)
+               136 LOAD_CONST              10 (<code object constant_threshold, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/thresholds/basic.py", line 20>)
                138 MAKE_FUNCTION            4 (annotations)
                140 STORE_NAME              16 (constant_threshold)
    
     32         142 PUSH_NULL
                144 LOAD_NAME                8 (as_factory)
                146 LOAD_CONST              11 ('no')
                148 LOAD_NAME               14 (no_threshold)
@@ -98,15 +98,15 @@
                156 CALL                     2
    
     33         166 LOAD_CONST              13 ('config')
                168 LOAD_NAME                9 (Config)
                170 LOAD_CONST               7 ('return')
                172 LOAD_NAME               12 (ThresholdFilter)
                174 BUILD_TUPLE              4
-               176 LOAD_CONST              14 (<code object no_threshold_using, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/thresholds/basic.py", line 32>)
+               176 LOAD_CONST              14 (<code object no_threshold_using, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/thresholds/basic.py", line 32>)
                178 MAKE_FUNCTION            4 (annotations)
    
     32         180 PRECALL                  0
                184 CALL                     0
    
     33         194 STORE_NAME              17 (no_threshold_using)
    
@@ -115,15 +115,15 @@
                200 LOAD_CONST              15 (True)
                202 KW_NAMES                16
                204 PRECALL                  1
                208 CALL                     1
    
     48         218 PUSH_NULL
                220 LOAD_BUILD_CLASS
-               222 LOAD_CONST              17 (<code object ConstantThresholdConfig, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/thresholds/basic.py", line 47>)
+               222 LOAD_CONST              17 (<code object ConstantThresholdConfig, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/thresholds/basic.py", line 47>)
                224 MAKE_FUNCTION            0
                226 LOAD_CONST              18 ('ConstantThresholdConfig')
                228 LOAD_NAME                9 (Config)
                230 PRECALL                  3
                234 CALL                     3
    
     47         244 PRECALL                  0
@@ -140,15 +140,15 @@
                274 CALL                     2
    
     62         284 LOAD_CONST              13 ('config')
                286 LOAD_NAME               18 (ConstantThresholdConfig)
                288 LOAD_CONST               7 ('return')
                290 LOAD_NAME               12 (ThresholdFilter)
                292 BUILD_TUPLE              4
-               294 LOAD_CONST              19 (<code object constant_threshold_using, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/thresholds/basic.py", line 61>)
+               294 LOAD_CONST              19 (<code object constant_threshold_using, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/thresholds/basic.py", line 61>)
                296 MAKE_FUNCTION            4 (annotations)
    
     61         298 PRECALL                  0
                302 CALL                     0
    
     62         312 STORE_NAME              19 (constant_threshold_using)
                314 LOAD_CONST              20 (None)
@@ -175,15 +175,15 @@
          consts
             '\n    Args:\n        evaluation: A scored evaluation of a position with some data type.\n\n    Returns:\n        bool: Always returns True.\n    '
             True
          names      ()
          varnames   ('evaluation',)
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/thresholds/basic.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/thresholds/basic.py'
          name       'no_threshold'
          firstlineno 9
          lnotab 0x0208
       'constant'
       code
          argcount  : 2
          nlocals   : 2
@@ -199,15 +199,15 @@
                       22 RETURN_VALUE
          consts
             '\n    Args:\n        constant: A float representing the threshold value.\n        evaluation: A ScoredEvaluation object containing the score to be evaluated.\n\n    Returns:\n        A boolean value indicating whether the score is greater than or equal to the constant threshold.\n    '
          names      ('score',)
          varnames   ('constant', 'evaluation')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/thresholds/basic.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/thresholds/basic.py'
          name       'constant_threshold'
          firstlineno 20
          lnotab 0x0209
       'no'
       ('using',)
       'config'
       code
@@ -222,15 +222,15 @@
                       14 RETURN_VALUE
          consts
             '\n    Create a `no_threshold_using` method that uses the `no_threshold` method to create a `ThresholdFilter` object.\n\n    Args:\n        config: A `Config` object that provides the necessary configuration for creating the `ThresholdFilter` object.\n\n    Returns:\n        A `ThresholdFilter` object created using the `no_threshold` method.\n\n    '
          names      ('no_threshold',)
          varnames   ('config',)
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/thresholds/basic.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/thresholds/basic.py'
          name       'no_threshold_using'
          firstlineno 32
          lnotab 0x020c
       True
       ('frozen',)
       code
          argcount  : 0
@@ -264,15 +264,15 @@
             0.8
             'constant'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'constant', 'float', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/thresholds/basic.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/thresholds/basic.py'
          name       'ConstantThresholdConfig'
          firstlineno 47
          lnotab 0x0c020409
       'ConstantThresholdConfig'
       code
          argcount  : 1
          nlocals   : 1
@@ -292,22 +292,22 @@
                       52 RETURN_VALUE
          consts
             'Apply a constant threshold using the specified configuration.\n\n    Args:\n        config: The configuration for the constant threshold.\n\n    Returns:\n        A partial function that applies the constant threshold filter.\n\n    '
          names      ('partial', 'constant_threshold', 'constant')
          varnames   ('config',)
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/thresholds/basic.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/thresholds/basic.py'
          name       'constant_threshold_using'
          firstlineno 61
          lnotab 0x020b
       None
-   names      ('dataclasses', 'dataclass', 'functools', 'partial', 'whereisit.types.entry', 'Position', 'DataType', 'whereisit.types.factory', 'as_factory', 'Config', 'whereisit.types.similarity', 'ScoredEvaluation', 'ThresholdFilter', 'bool', 'no_threshold', 'float', 'constant_threshold', 'no_threshold_using', 'ConstantThresholdConfig', 'constant_threshold_using')
+   names      ('dataclasses', 'dataclass', 'functools', 'partial', 'findanywhere.types.entry', 'Position', 'DataType', 'findanywhere.types.factory', 'as_factory', 'Config', 'findanywhere.types.similarity', 'ScoredEvaluation', 'ThresholdFilter', 'bool', 'no_threshold', 'float', 'constant_threshold', 'no_threshold_using', 'ConstantThresholdConfig', 'constant_threshold_using')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/thresholds/basic.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/thresholds/basic.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c010c02100110011003200b240c18010eff0e01020e16011a
       ff0e01020d18010eff0e01
```

### Comparing `findanywhere-0.1.0/whereisit/thresholds/basic.py` & `findanywhere-1.0.0/findanywhere/thresholds/basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from functools import partial
 
-from whereisit.types.entry import Position, DataType
-from whereisit.types.factory import as_factory, Config
-from whereisit.types.similarity import ScoredEvaluation, ThresholdFilter
+from findanywhere.types.entry import Position, DataType
+from findanywhere.types.factory import as_factory, Config
+from findanywhere.types.similarity import ScoredEvaluation, ThresholdFilter
 
 
 def no_threshold(evaluation: ScoredEvaluation[Position, DataType]) -> bool:
     """
     Args:
         evaluation: A scored evaluation of a position with some data type.
```

### Comparing `findanywhere-0.1.0/whereisit/types/__pycache__/entry.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/types/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-0.1.0/whereisit/types/__pycache__/factory.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/types/__pycache__/factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-0.1.0/whereisit/types/__pycache__/input_data.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/types/__pycache__/input_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-0.1.0/whereisit/types/__pycache__/similarity.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/types/__pycache__/similarity.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xe3f05166 (Sat May 25 14:08:35 2024 UTC)
-files sz: 2675
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 2681
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
@@ -41,26 +41,26 @@
                 26 STORE_NAME               4 (Protocol)
                 28 IMPORT_FROM              5 (Generic)
                 30 STORE_NAME               5 (Generic)
                 32 POP_TOP
    
      4          34 LOAD_CONST               0 (0)
                 36 LOAD_CONST               3 (('Entry', 'Position', 'DataType'))
-                38 IMPORT_NAME              6 (whereisit.types.entry)
+                38 IMPORT_NAME              6 (findanywhere.types.entry)
                 40 IMPORT_FROM              7 (Entry)
                 42 STORE_NAME               7 (Entry)
                 44 IMPORT_FROM              8 (Position)
                 46 STORE_NAME               8 (Position)
                 48 IMPORT_FROM              9 (DataType)
                 50 STORE_NAME               9 (DataType)
                 52 POP_TOP
    
      5          54 LOAD_CONST               0 (0)
                 56 LOAD_CONST               4 (('InputID',))
-                58 IMPORT_NAME             10 (whereisit.types.input_data)
+                58 IMPORT_NAME             10 (findanywhere.types.input_data)
                 60 IMPORT_FROM             11 (InputID)
                 62 STORE_NAME              11 (InputID)
                 64 POP_TOP
    
      7          66 PUSH_NULL
                 68 LOAD_NAME                3 (TypeVar)
                 70 LOAD_CONST               5 ('_T')
@@ -68,15 +68,15 @@
                 74 KW_NAMES                 7
                 76 PRECALL                  2
                 80 CALL                     2
                 90 STORE_NAME              12 (_T)
    
     10          92 PUSH_NULL
                 94 LOAD_BUILD_CLASS
-                96 LOAD_CONST               8 (<code object Similarity, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py", line 10>)
+                96 LOAD_CONST               8 (<code object Similarity, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py", line 10>)
                 98 MAKE_FUNCTION            0
                100 LOAD_CONST               9 ('Similarity')
                102 LOAD_NAME                4 (Protocol)
                104 LOAD_NAME               12 (_T)
                106 BINARY_SUBSCR
                116 PRECALL                  3
                120 CALL                     3
@@ -87,15 +87,15 @@
                136 LOAD_CONST               6 (True)
                138 KW_NAMES                10
                140 PRECALL                  1
                144 CALL                     1
    
     21         154 PUSH_NULL
                156 LOAD_BUILD_CLASS
-               158 LOAD_CONST              11 (<code object ScoredEntry, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py", line 20>)
+               158 LOAD_CONST              11 (<code object ScoredEntry, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py", line 20>)
                160 MAKE_FUNCTION            0
                162 LOAD_CONST              12 ('ScoredEntry')
                164 LOAD_NAME                7 (Entry)
                166 LOAD_NAME                8 (Position)
                168 LOAD_NAME                9 (DataType)
                170 BUILD_TUPLE              2
                172 BINARY_SUBSCR
@@ -112,15 +112,15 @@
                216 LOAD_CONST               6 (True)
                218 KW_NAMES                10
                220 PRECALL                  1
                224 CALL                     1
    
     33         234 PUSH_NULL
                236 LOAD_BUILD_CLASS
-               238 LOAD_CONST              13 (<code object Evaluation, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py", line 32>)
+               238 LOAD_CONST              13 (<code object Evaluation, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py", line 32>)
                240 MAKE_FUNCTION            0
                242 LOAD_CONST              14 ('Evaluation')
                244 LOAD_NAME                5 (Generic)
                246 LOAD_NAME                8 (Position)
                248 LOAD_NAME                9 (DataType)
                250 BUILD_TUPLE              2
                252 BINARY_SUBSCR
@@ -137,15 +137,15 @@
                296 LOAD_CONST               6 (True)
                298 KW_NAMES                10
                300 PRECALL                  1
                304 CALL                     1
    
     50         314 PUSH_NULL
                316 LOAD_BUILD_CLASS
-               318 LOAD_CONST              15 (<code object ScoredEvaluation, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py", line 49>)
+               318 LOAD_CONST              15 (<code object ScoredEvaluation, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py", line 49>)
                320 MAKE_FUNCTION            0
                322 LOAD_CONST              16 ('ScoredEvaluation')
                324 LOAD_NAME               15 (Evaluation)
                326 LOAD_NAME                8 (Position)
                328 LOAD_NAME                9 (DataType)
                330 BUILD_TUPLE              2
                332 BINARY_SUBSCR
@@ -155,29 +155,29 @@
     49         356 PRECALL                  0
                360 CALL                     0
    
     50         370 STORE_NAME              16 (ScoredEvaluation)
    
     61         372 PUSH_NULL
                374 LOAD_BUILD_CLASS
-               376 LOAD_CONST              17 (<code object DeduceScore, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py", line 61>)
+               376 LOAD_CONST              17 (<code object DeduceScore, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py", line 61>)
                378 MAKE_FUNCTION            0
                380 LOAD_CONST              18 ('DeduceScore')
                382 LOAD_NAME                4 (Protocol)
                384 LOAD_NAME                8 (Position)
                386 LOAD_NAME                9 (DataType)
                388 BUILD_TUPLE              2
                390 BINARY_SUBSCR
                400 PRECALL                  3
                404 CALL                     3
                414 STORE_NAME              17 (DeduceScore)
    
     83         416 PUSH_NULL
                418 LOAD_BUILD_CLASS
-               420 LOAD_CONST              19 (<code object ThresholdFilter, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py", line 83>)
+               420 LOAD_CONST              19 (<code object ThresholdFilter, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py", line 83>)
                422 MAKE_FUNCTION            0
                424 LOAD_CONST              20 ('ThresholdFilter')
                426 LOAD_NAME                4 (Protocol)
                428 LOAD_NAME                8 (Position)
                430 LOAD_NAME                9 (DataType)
                432 BUILD_TUPLE              2
                434 BINARY_SUBSCR
@@ -215,15 +215,15 @@
           16          14 LOAD_CONST               2 ('left')
                       16 LOAD_NAME                4 (_T)
                       18 LOAD_CONST               3 ('right')
                       20 LOAD_NAME                4 (_T)
                       22 LOAD_CONST               4 ('return')
                       24 LOAD_NAME                5 (float)
                       26 BUILD_TUPLE              6
-                      28 LOAD_CONST               5 (<code object __call__, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py", line 16>)
+                      28 LOAD_CONST               5 (<code object __call__, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py", line 16>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               6 (__call__)
                       34 LOAD_CONST               6 (None)
                       36 RETURN_VALUE
          consts
             'Similarity'
             '\n    Function that calculates the similarity of two values. Higher values indicate more similar values. Usually\n    similarity ratings range from 0 to 1, but other ratings are possible, too.\n    '
@@ -242,24 +242,24 @@
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'left', 'right')
                freevars   ()
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py'
                name       '__call__'
                firstlineno 16
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', '_T', 'float', '__call__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py'
          name       'Similarity'
          firstlineno 10
          lnotab 0x0a010405
       'Similarity'
       ('frozen',)
       code
          argcount  : 0
@@ -290,15 +290,15 @@
             '\n    Represents a scored entry with a similarity value.\n\n    Attributes:\n        similarity (float): The similarity value of the scored entry.\n\n    '
             'similarity'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'float', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py'
          name       'ScoredEntry'
          firstlineno 20
          lnotab 0x0c020407
       'ScoredEntry'
       code
          argcount  : 0
          nlocals   : 0
@@ -343,15 +343,15 @@
             'of'
             'best_matches'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'InputID', '__annotations__', 'dict', 'str', 'ScoredEntry', 'Position', 'DataType')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py'
          name       'Evaluation'
          firstlineno 32
          lnotab 0x0c02040b0a01
       'Evaluation'
       code
          argcount  : 0
          nlocals   : 0
@@ -381,15 +381,15 @@
             '\n    Class representing a scored evaluation.\n\n    Attributes:\n        score (float): The score of the evaluation.\n\n    '
             'score'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'float', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py'
          name       'ScoredEvaluation'
          firstlineno 49
          lnotab 0x0c020407
       'ScoredEvaluation'
       code
          argcount  : 0
          nlocals   : 0
@@ -417,15 +417,15 @@
                       34 LOAD_CONST               3 ('return')
                       36 LOAD_NAME                7 (ScoredEvaluation)
                       38 LOAD_NAME                5 (Position)
                       40 LOAD_NAME                6 (DataType)
                       42 BUILD_TUPLE              2
                       44 BINARY_SUBSCR
                       54 BUILD_TUPLE              4
-                      56 LOAD_CONST               4 (<code object __call__, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py", line 70>)
+                      56 LOAD_CONST               4 (<code object __call__, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py", line 70>)
                       58 MAKE_FUNCTION            4 (annotations)
                       60 STORE_NAME               8 (__call__)
                       62 LOAD_CONST               5 (None)
                       64 RETURN_VALUE
          consts
             'DeduceScore'
             '\n\n    This class represents a function-like object that takes an evaluation object and returns a scored evaluation object.\n\n    Methods:\n        __call__: Executes the function-like object.\n\n    '
@@ -444,24 +444,24 @@
                consts
                   '\n        Args:\n            evaluation: An instance of the Evaluation class with generic types `Position` and `DataType`. It represents\n            the evaluation result.\n\n        Returns:\n            An instance of the ScoredEvaluation class with generic types `Position` and `DataType`. It represents the\n            scored evaluation result.\n        '
                   None
                names      ()
                varnames   ('self', 'evaluation')
                freevars   ()
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py'
                name       '__call__'
                firstlineno 70
                lnotab 0x020a
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Evaluation', 'Position', 'DataType', 'ScoredEvaluation', '__call__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py'
          name       'DeduceScore'
          firstlineno 61
          lnotab 0x0a010408
       'DeduceScore'
       code
          argcount  : 0
          nlocals   : 0
@@ -484,15 +484,15 @@
                       18 LOAD_NAME                5 (Position)
                       20 LOAD_NAME                6 (DataType)
                       22 BUILD_TUPLE              2
                       24 BINARY_SUBSCR
                       34 LOAD_CONST               3 ('return')
                       36 LOAD_NAME                7 (bool)
                       38 BUILD_TUPLE              4
-                      40 LOAD_CONST               4 (<code object __call__, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py", line 88>)
+                      40 LOAD_CONST               4 (<code object __call__, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py", line 88>)
                       42 MAKE_FUNCTION            4 (annotations)
                       44 STORE_NAME               8 (__call__)
                       46 LOAD_CONST               5 (None)
                       48 RETURN_VALUE
          consts
             'ThresholdFilter'
             '\n\n    This class represents a filter that determines whether a scored evaluation passes a threshold.\n    '
@@ -511,32 +511,32 @@
                consts
                   '\n        Args:\n            evaluation: The scored evaluation of the position with its data type.\n\n        Returns:\n            bool: True if the method is called successfully, False otherwise.\n        '
                   None
                names      ()
                varnames   ('self', 'evaluation')
                freevars   ()
                cellvars   ()
-               filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py'
+               filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py'
                name       '__call__'
                firstlineno 88
                lnotab 0x0208
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'ScoredEvaluation', 'Position', 'DataType', 'bool', '__call__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py'
          name       'ThresholdFilter'
          firstlineno 83
          lnotab 0x0a010404
       'ThresholdFilter'
       None
-   names      ('dataclasses', 'dataclass', 'typing', 'TypeVar', 'Protocol', 'Generic', 'whereisit.types.entry', 'Entry', 'Position', 'DataType', 'whereisit.types.input_data', 'InputID', '_T', 'Similarity', 'ScoredEntry', 'Evaluation', 'ScoredEvaluation', 'DeduceScore', 'ThresholdFilter')
+   names      ('dataclasses', 'dataclass', 'typing', 'TypeVar', 'Protocol', 'Generic', 'findanywhere.types.entry', 'Entry', 'Position', 'DataType', 'findanywhere.types.input_data', 'InputID', '_T', 'Similarity', 'ScoredEntry', 'Evaluation', 'ScoredEvaluation', 'DeduceScore', 'ThresholdFilter')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/types/similarity.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/types/similarity.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c01140214010c021a03280a16012aff0e01020b16012aff0e
       01021016012aff0e01020b2c16
```

### Comparing `findanywhere-0.1.0/whereisit/types/entry.py` & `findanywhere-1.0.0/findanywhere/types/entry.py`

 * *Files identical despite different names*

### Comparing `findanywhere-0.1.0/whereisit/types/factory.py` & `findanywhere-1.0.0/findanywhere/types/factory.py`

 * *Files identical despite different names*

### Comparing `findanywhere-0.1.0/whereisit/types/input_data.py` & `findanywhere-1.0.0/findanywhere/types/input_data.py`

 * *Files identical despite different names*

### Comparing `findanywhere-0.1.0/whereisit/types/similarity.py` & `findanywhere-1.0.0/findanywhere/types/similarity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import TypeVar, Protocol, Generic
 
-from whereisit.types.entry import Entry, Position, DataType
-from whereisit.types.input_data import InputID
+from findanywhere.types.entry import Entry, Position, DataType
+from findanywhere.types.input_data import InputID
 
 _T = TypeVar('_T', contravariant=True)
 
 
 class Similarity(Protocol[_T]):
     """
     Function that calculates the similarity of two values. Higher values indicate more similar values. Usually
```

### Comparing `findanywhere-0.1.0/whereisit/ui/__pycache__/console.cpython-311.pyc` & `findanywhere-1.0.0/findanywhere/ui/__pycache__/console.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x28f35166 (Sat May 25 14:18:16 2024 UTC)
-files sz: 2011
+moddate:  0x9d2c5366 (Sun May 26 12:35:41 2024 UTC)
+files sz: 2029
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -57,62 +57,62 @@
                 70 IMPORT_NAME             11 (typing)
                 72 IMPORT_FROM             12 (cast)
                 74 STORE_NAME              12 (cast)
                 76 POP_TOP
    
      8          78 LOAD_CONST               0 (0)
                 80 LOAD_CONST               7 (('SourceAdapter',))
-                82 IMPORT_NAME             13 (whereisit.ports.source)
+                82 IMPORT_NAME             13 (findanywhere.ports.source)
                 84 IMPORT_FROM             14 (SourceAdapter)
                 86 STORE_NAME              14 (SourceAdapter)
                 88 POP_TOP
    
      9          90 LOAD_CONST               0 (0)
                 92 LOAD_CONST               8 (('load_schema', 'SearchSchema'))
-                94 IMPORT_NAME             15 (whereisit.schema)
+                94 IMPORT_NAME             15 (findanywhere.schema)
                 96 IMPORT_FROM             16 (load_schema)
                 98 STORE_NAME              16 (load_schema)
                100 IMPORT_FROM             17 (SearchSchema)
                102 STORE_NAME              17 (SearchSchema)
                104 POP_TOP
    
     10         106 LOAD_CONST               0 (0)
                108 LOAD_CONST               9 (('Search', 'search', 'SearchPattern'))
-               110 IMPORT_NAME             18 (whereisit.search.base)
+               110 IMPORT_NAME             18 (findanywhere.search.base)
                112 IMPORT_FROM             19 (Search)
                114 STORE_NAME              19 (Search)
                116 IMPORT_FROM             20 (search)
                118 STORE_NAME              20 (search)
                120 IMPORT_FROM             21 (SearchPattern)
                122 STORE_NAME              21 (SearchPattern)
                124 POP_TOP
    
     11         126 LOAD_CONST               0 (0)
                128 LOAD_CONST              10 (('parallel_search',))
-               130 IMPORT_NAME             22 (whereisit.search.parallel)
+               130 IMPORT_NAME             22 (findanywhere.search.parallel)
                132 IMPORT_FROM             23 (parallel_search)
                134 STORE_NAME              23 (parallel_search)
                136 POP_TOP
    
     12         138 LOAD_CONST               0 (0)
                140 LOAD_CONST              11 (('sequential_search',))
-               142 IMPORT_NAME             24 (whereisit.search.sequential)
+               142 IMPORT_NAME             24 (findanywhere.search.sequential)
                144 IMPORT_FROM             25 (sequential_search)
                146 STORE_NAME              25 (sequential_search)
                148 POP_TOP
    
     13         150 LOAD_CONST               0 (0)
                152 LOAD_CONST              12 (('InputData',))
-               154 IMPORT_NAME             26 (whereisit.types.input_data)
+               154 IMPORT_NAME             26 (findanywhere.types.input_data)
                156 IMPORT_FROM             27 (InputData)
                158 STORE_NAME              27 (InputData)
                160 POP_TOP
    
     16         162 LOAD_CONST              16 (('return', None))
-               164 LOAD_CONST              15 (<code object main, file "/home/voidpointercast/PycharmProjects/whereisit/whereisit/ui/console.py", line 16>)
+               164 LOAD_CONST              15 (<code object main, file "/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ui/console.py", line 16>)
                166 MAKE_FUNCTION            4 (annotations)
                168 STORE_NAME              28 (main)
                170 LOAD_CONST              14 (None)
                172 RETURN_VALUE
    consts
       0
       ('ArgumentParser', 'Namespace')
@@ -427,22 +427,22 @@
             ('ensure_ascii', 'default')
             '\n'
             None
          names      ('ArgumentParser', 'add_argument', 'Path', 'int', 'cpu_count', 'bool', 'parse_known_args', 'load_schema', 'schema', 'source', 'config', 'location_type', 'parse_args', 'partial', 'search', 'evaluation_adapter', 'create_deduction', 'create_threshold', 'source_adapter', 'sequential', 'cast', 'SearchPattern', 'parallel_search', 'processes', 'sequential_search', 'open', 'out', 'InputData', 'from_json', 'input_data', 'location', 'dump', 'str', 'write')
          varnames   ('parser', 'primary_args', 'schema', 'args', 'search_', 'source_adapter', 'search_style', 'out', 'result')
          freevars   ()
          cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/ui/console.py'
+         filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ui/console.py'
          name       'main'
          firstlineno 16
          lnotab
             0x02041e013a013a01520154013c0134022801660128029a0228040cfe26
             0118ff20020cfe02043201680130012cfe02ff
       ('return', None)
-   names      ('argparse', 'ArgumentParser', 'Namespace', 'functools', 'partial', 'json', 'dump', 'multiprocessing', 'cpu_count', 'pathlib', 'Path', 'typing', 'cast', 'whereisit.ports.source', 'SourceAdapter', 'whereisit.schema', 'load_schema', 'SearchSchema', 'whereisit.search.base', 'Search', 'search', 'SearchPattern', 'whereisit.search.parallel', 'parallel_search', 'whereisit.search.sequential', 'sequential_search', 'whereisit.types.input_data', 'InputData', 'main')
+   names      ('argparse', 'ArgumentParser', 'Namespace', 'functools', 'partial', 'json', 'dump', 'multiprocessing', 'cpu_count', 'pathlib', 'Path', 'typing', 'cast', 'findanywhere.ports.source', 'SourceAdapter', 'findanywhere.schema', 'load_schema', 'SearchSchema', 'findanywhere.search.base', 'Search', 'search', 'SearchPattern', 'findanywhere.search.parallel', 'parallel_search', 'findanywhere.search.sequential', 'sequential_search', 'findanywhere.types.input_data', 'InputData', 'main')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/voidpointercast/PycharmProjects/whereisit/whereisit/ui/console.py'
+   filename   '/home/voidpointercast/PycharmProjects/whereisit/findanywhere/ui/console.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020110010c010c010c010c010c020c01100114010c010c010c03
```

### Comparing `findanywhere-0.1.0/whereisit/ui/console.py` & `findanywhere-1.0.0/findanywhere/ui/console.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from argparse import ArgumentParser, Namespace
 from functools import partial
 from json import dump
 from multiprocessing import cpu_count
 from pathlib import Path
 from typing import cast
 
-from whereisit.ports.source import SourceAdapter
-from whereisit.schema import load_schema, SearchSchema
-from whereisit.search.base import Search, search, SearchPattern
-from whereisit.search.parallel import parallel_search
-from whereisit.search.sequential import sequential_search
-from whereisit.types.input_data import InputData
+from findanywhere.ports.source import SourceAdapter
+from findanywhere.schema import load_schema, SearchSchema
+from findanywhere.search.base import Search, search, SearchPattern
+from findanywhere.search.parallel import parallel_search
+from findanywhere.search.sequential import sequential_search
+from findanywhere.types.input_data import InputData
 
 
 def main() -> None:
     """
     Main method for searching data in a data set using a schema.
     """
     parser: ArgumentParser = ArgumentParser('Search for data in a data set using a schema')
```

### Comparing `findanywhere-0.1.0/PKG-INFO` & `findanywhere-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: findanywhere
-Version: 0.1.0
+Version: 1.0.0
 Summary: 
-Home-page: https://gitlab.com/patrick.daniel.gress/whereisit
+Home-page: https://gitlab.com/patrick.daniel.gress/findanywhere
 License: BSD License (BSD)
 Keywords: search,fuzzy_search,preprocessing
 Author: voidpointercast
 Author-email: voidpointercast@justmail.de
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Dist: dacite (>=1.8.1,<2.0.0)
 Requires-Dist: jellyfish (>=1.0.3,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: toolz (>=0.12.1,<0.13.0)
 Project-URL: Documentation, https://whereisit.readthedocs.io/en/latest/
-Project-URL: Repository, https://gitlab.com/patrick.daniel.gress/whereisit
+Project-URL: Repository, https://gitlab.com/patrick.daniel.gress/findanywhere
 Description-Content-Type: text/markdown
 
 **WhereIsIt** is a tool designed for data analysts and developers facing the challenge of extracting meaningful 
 information from poorly structured or malformed CSV files. 
 This tool simplifies the process of filtering and analyzing data by allowing users to prefilter large datasets without 
 needing to correct their format first, focusing efforts on smaller, more relevant subsets.
 
@@ -96,25 +96,25 @@
     constant: 0.9
   name: constant
 ````
 
 Run the tool against your datasets using the defined schema:
 
 ````shell
-whereisit schema.yml search_data.json garbage.csv --out result.json_line
+findanywhere schema.yml search_data.json garbage.csv --out result.json_line
 ````
 
 Results will be stored in result.json_line. For additional commands and options, use the --help flag.
 
 ## Installation
 
 Install **WhereIsIt** easily using pip:
 
 ````shell
-pip install whereisit
+pip install findanywhere
 ````
 
 
 ## Key Features
 
 - **Robust Malformed File Handling:** Efficiently processes CSV files with irregular column structures or misplaced data entries.
 - **Fuzzy Matching Capabilities:** Utilizes advanced algorithms to match data points based on similarity, accommodating various types of data discrepancies.
```

