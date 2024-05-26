# Comparing `tmp/findanywhere-1.0.0.tar.gz` & `tmp/findanywhere-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findanywhere-1.0.0.tar", max compression
+gzip compressed data, was "findanywhere-1.0.1.tar", max compression
```

## Comparing `findanywhere-1.0.0.tar` & `findanywhere-1.0.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1496 2024-05-20 11:00:15.359287 findanywhere-1.0.0/LICENSE
--rw-r--r--   0        0        0     3621 2024-05-26 12:35:41.100676 findanywhere-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-05-08 17:42:21.640505 findanywhere-1.0.0/findanywhere/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 17:44:07.424377 findanywhere-1.0.0/findanywhere/adapters/__init__.py
--rw-r--r--   0        0        0      187 2024-05-08 19:00:14.593812 findanywhere-1.0.0/findanywhere/adapters/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      352 2024-05-26 12:35:41.108676 findanywhere-1.0.0/findanywhere/adapters/evaluation/__init__.py
--rw-r--r--   0        0        0      718 2024-05-26 12:35:41.415679 findanywhere-1.0.0/findanywhere/adapters/evaluation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5856 2024-05-26 12:35:41.416679 findanywhere-1.0.0/findanywhere/adapters/evaluation/__pycache__/string_distance.cpython-311.pyc
--rw-r--r--   0        0        0     3434 2024-05-26 12:35:41.147677 findanywhere-1.0.0/findanywhere/adapters/evaluation/string_distance.py
--rw-r--r--   0        0        0      402 2024-05-26 12:35:41.054676 findanywhere-1.0.0/findanywhere/adapters/source/__init__.py
--rw-r--r--   0        0        0      774 2024-05-26 12:35:41.377679 findanywhere-1.0.0/findanywhere/adapters/source/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5931 2024-05-26 12:35:41.391679 findanywhere-1.0.0/findanywhere/adapters/source/__pycache__/tabular.cpython-311.pyc
--rw-r--r--   0        0        0     6107 2024-05-26 12:35:41.377679 findanywhere-1.0.0/findanywhere/adapters/source/__pycache__/text.cpython-311.pyc
--rw-r--r--   0        0        0     3430 2024-05-26 12:35:41.125676 findanywhere-1.0.0/findanywhere/adapters/source/tabular.py
--rw-r--r--   0        0        0     3740 2024-05-26 12:35:41.088676 findanywhere-1.0.0/findanywhere/adapters/source/text.py
--rw-r--r--   0        0        0        0 2024-05-20 10:27:18.968764 findanywhere-1.0.0/findanywhere/algorithms/__init__.py
--rw-r--r--   0        0        0      189 2024-05-20 10:29:17.917054 findanywhere-1.0.0/findanywhere/algorithms/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3102 2024-05-25 14:09:44.516764 findanywhere-1.0.0/findanywhere/algorithms/__pycache__/strings.cpython-311.pyc
--rw-r--r--   0        0        0     1946 2024-05-25 14:09:44.443763 findanywhere-1.0.0/findanywhere/algorithms/strings.py
--rw-r--r--   0        0        0        0 2024-05-08 17:44:02.344335 findanywhere-1.0.0/findanywhere/ports/__init__.py
--rw-r--r--   0        0        0      184 2024-05-08 19:00:14.617812 findanywhere-1.0.0/findanywhere/ports/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3349 2024-05-26 12:35:41.392679 findanywhere-1.0.0/findanywhere/ports/__pycache__/evaluation.cpython-311.pyc
--rw-r--r--   0        0        0     3366 2024-05-26 12:35:41.384679 findanywhere-1.0.0/findanywhere/ports/__pycache__/source.cpython-311.pyc
--rw-r--r--   0        0        0     2143 2024-05-26 12:35:41.133676 findanywhere-1.0.0/findanywhere/ports/evaluation.py
--rw-r--r--   0        0        0     1939 2024-05-26 12:35:41.084676 findanywhere-1.0.0/findanywhere/ports/source.py
--rw-r--r--   0        0        0     8133 2024-05-26 12:35:41.120676 findanywhere-1.0.0/findanywhere/schema.py
--rw-r--r--   0        0        0      318 2024-05-26 12:35:41.097676 findanywhere-1.0.0/findanywhere/scores/__init__.py
--rw-r--r--   0        0        0      673 2024-05-26 12:35:41.426679 findanywhere-1.0.0/findanywhere/scores/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2148 2024-05-26 12:35:41.426679 findanywhere-1.0.0/findanywhere/scores/__pycache__/deduction.cpython-311.pyc
--rw-r--r--   0        0        0     1345 2024-05-26 12:35:41.137677 findanywhere-1.0.0/findanywhere/scores/deduction.py
--rw-r--r--   0        0        0        0 2024-05-08 19:27:30.026829 findanywhere-1.0.0/findanywhere/search/__init__.py
--rw-r--r--   0        0        0      185 2024-05-08 19:59:50.195437 findanywhere-1.0.0/findanywhere/search/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7961 2024-05-26 12:35:41.427679 findanywhere-1.0.0/findanywhere/search/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     3804 2024-05-26 12:35:41.428679 findanywhere-1.0.0/findanywhere/search/__pycache__/parallel.cpython-311.pyc
--rw-r--r--   0        0        0     2103 2024-05-26 12:35:41.431679 findanywhere-1.0.0/findanywhere/search/__pycache__/sequential.cpython-311.pyc
--rw-r--r--   0        0        0     6060 2024-05-26 12:35:41.079676 findanywhere-1.0.0/findanywhere/search/base.py
--rw-r--r--   0        0        0     2405 2024-05-26 12:35:41.163677 findanywhere-1.0.0/findanywhere/search/parallel.py
--rw-r--r--   0        0        0     1426 2024-05-26 12:35:41.159677 findanywhere-1.0.0/findanywhere/search/sequential.py
--rw-r--r--   0        0        0      996 2024-05-26 12:35:41.062676 findanywhere-1.0.0/findanywhere/similarity/__init__.py
--rw-r--r--   0        0        0     1937 2024-05-26 12:35:41.416679 findanywhere-1.0.0/findanywhere/similarity/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2556 2024-05-26 12:35:41.417679 findanywhere-1.0.0/findanywhere/similarity/__pycache__/common.cpython-311.pyc
--rw-r--r--   0        0        0     5524 2024-05-26 12:35:41.418679 findanywhere-1.0.0/findanywhere/similarity/__pycache__/token.cpython-311.pyc
--rw-r--r--   0        0        0     1773 2024-05-26 12:35:41.039676 findanywhere-1.0.0/findanywhere/similarity/common.py
--rw-r--r--   0        0        0     3615 2024-05-26 12:35:41.071676 findanywhere-1.0.0/findanywhere/similarity/token.py
--rw-r--r--   0        0        0      378 2024-05-26 12:35:41.143677 findanywhere-1.0.0/findanywhere/thresholds/__init__.py
--rw-r--r--   0        0        0      724 2024-05-26 12:35:41.431679 findanywhere-1.0.0/findanywhere/thresholds/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3306 2024-05-26 12:35:41.432679 findanywhere-1.0.0/findanywhere/thresholds/__pycache__/basic.cpython-311.pyc
--rw-r--r--   0        0        0     2173 2024-05-26 12:35:41.044676 findanywhere-1.0.0/findanywhere/thresholds/basic.py
--rw-r--r--   0        0        0        0 2024-05-08 17:43:06.743877 findanywhere-1.0.0/findanywhere/types/__init__.py
--rw-r--r--   0        0        0      184 2024-05-08 19:00:14.644813 findanywhere-1.0.0/findanywhere/types/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1178 2024-05-25 14:18:32.167222 findanywhere-1.0.0/findanywhere/types/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     7465 2024-05-25 14:18:32.168222 findanywhere-1.0.0/findanywhere/types/__pycache__/factory.cpython-311.pyc
--rw-r--r--   0        0        0     4722 2024-05-25 14:18:32.177222 findanywhere-1.0.0/findanywhere/types/__pycache__/input_data.cpython-311.pyc
--rw-r--r--   0        0        0     4918 2024-05-26 12:35:41.393679 findanywhere-1.0.0/findanywhere/types/__pycache__/similarity.cpython-311.pyc
--rw-r--r--   0        0        0      568 2024-05-25 14:08:35.015154 findanywhere-1.0.0/findanywhere/types/entry.py
--rw-r--r--   0        0        0     4416 2024-05-25 14:08:34.955154 findanywhere-1.0.0/findanywhere/types/factory.py
--rw-r--r--   0        0        0     2833 2024-05-25 14:08:34.936154 findanywhere-1.0.0/findanywhere/types/input_data.py
--rw-r--r--   0        0        0     2681 2024-05-26 12:35:41.172677 findanywhere-1.0.0/findanywhere/types/similarity.py
--rw-r--r--   0        0        0        0 2024-05-09 10:19:42.473640 findanywhere-1.0.0/findanywhere/ui/__init__.py
--rw-r--r--   0        0        0      181 2024-05-09 10:57:56.733493 findanywhere-1.0.0/findanywhere/ui/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3888 2024-05-26 12:35:41.473680 findanywhere-1.0.0/findanywhere/ui/__pycache__/console.cpython-311.pyc
--rw-r--r--   0        0        0     2029 2024-05-26 12:35:41.116676 findanywhere-1.0.0/findanywhere/ui/console.py
--rw-r--r--   0        0        0     1490 2024-05-26 12:42:48.297992 findanywhere-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4829 1970-01-01 00:00:00.000000 findanywhere-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1496 2024-05-20 11:00:15.359287 findanywhere-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3621 2024-05-26 12:35:41.100676 findanywhere-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 17:42:21.640505 findanywhere-1.0.1/findanywhere/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:44:07.424377 findanywhere-1.0.1/findanywhere/adapters/__init__.py
+-rw-r--r--   0        0        0      187 2024-05-08 19:00:14.593812 findanywhere-1.0.1/findanywhere/adapters/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      352 2024-05-26 12:35:41.108676 findanywhere-1.0.1/findanywhere/adapters/evaluation/__init__.py
+-rw-r--r--   0        0        0      718 2024-05-26 12:35:41.415679 findanywhere-1.0.1/findanywhere/adapters/evaluation/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5856 2024-05-26 12:35:41.416679 findanywhere-1.0.1/findanywhere/adapters/evaluation/__pycache__/string_distance.cpython-311.pyc
+-rw-r--r--   0        0        0     3434 2024-05-26 12:35:41.147677 findanywhere-1.0.1/findanywhere/adapters/evaluation/string_distance.py
+-rw-r--r--   0        0        0      402 2024-05-26 12:35:41.054676 findanywhere-1.0.1/findanywhere/adapters/source/__init__.py
+-rw-r--r--   0        0        0      774 2024-05-26 12:35:41.377679 findanywhere-1.0.1/findanywhere/adapters/source/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5931 2024-05-26 12:35:41.391679 findanywhere-1.0.1/findanywhere/adapters/source/__pycache__/tabular.cpython-311.pyc
+-rw-r--r--   0        0        0     6107 2024-05-26 12:35:41.377679 findanywhere-1.0.1/findanywhere/adapters/source/__pycache__/text.cpython-311.pyc
+-rw-r--r--   0        0        0     3430 2024-05-26 12:35:41.125676 findanywhere-1.0.1/findanywhere/adapters/source/tabular.py
+-rw-r--r--   0        0        0     3740 2024-05-26 12:35:41.088676 findanywhere-1.0.1/findanywhere/adapters/source/text.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:27:18.968764 findanywhere-1.0.1/findanywhere/algorithms/__init__.py
+-rw-r--r--   0        0        0      189 2024-05-20 10:29:17.917054 findanywhere-1.0.1/findanywhere/algorithms/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3102 2024-05-25 14:09:44.516764 findanywhere-1.0.1/findanywhere/algorithms/__pycache__/strings.cpython-311.pyc
+-rw-r--r--   0        0        0     1946 2024-05-25 14:09:44.443763 findanywhere-1.0.1/findanywhere/algorithms/strings.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:44:02.344335 findanywhere-1.0.1/findanywhere/ports/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-08 19:00:14.617812 findanywhere-1.0.1/findanywhere/ports/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3349 2024-05-26 12:35:41.392679 findanywhere-1.0.1/findanywhere/ports/__pycache__/evaluation.cpython-311.pyc
+-rw-r--r--   0        0        0     3366 2024-05-26 12:35:41.384679 findanywhere-1.0.1/findanywhere/ports/__pycache__/source.cpython-311.pyc
+-rw-r--r--   0        0        0     2143 2024-05-26 12:35:41.133676 findanywhere-1.0.1/findanywhere/ports/evaluation.py
+-rw-r--r--   0        0        0     1939 2024-05-26 12:35:41.084676 findanywhere-1.0.1/findanywhere/ports/source.py
+-rw-r--r--   0        0        0     8133 2024-05-26 12:35:41.120676 findanywhere-1.0.1/findanywhere/schema.py
+-rw-r--r--   0        0        0      318 2024-05-26 12:35:41.097676 findanywhere-1.0.1/findanywhere/scores/__init__.py
+-rw-r--r--   0        0        0      673 2024-05-26 12:35:41.426679 findanywhere-1.0.1/findanywhere/scores/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2148 2024-05-26 12:35:41.426679 findanywhere-1.0.1/findanywhere/scores/__pycache__/deduction.cpython-311.pyc
+-rw-r--r--   0        0        0     1345 2024-05-26 12:35:41.137677 findanywhere-1.0.1/findanywhere/scores/deduction.py
+-rw-r--r--   0        0        0        0 2024-05-08 19:27:30.026829 findanywhere-1.0.1/findanywhere/search/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-08 19:59:50.195437 findanywhere-1.0.1/findanywhere/search/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7961 2024-05-26 12:35:41.427679 findanywhere-1.0.1/findanywhere/search/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     3804 2024-05-26 12:35:41.428679 findanywhere-1.0.1/findanywhere/search/__pycache__/parallel.cpython-311.pyc
+-rw-r--r--   0        0        0     2103 2024-05-26 12:35:41.431679 findanywhere-1.0.1/findanywhere/search/__pycache__/sequential.cpython-311.pyc
+-rw-r--r--   0        0        0     6060 2024-05-26 12:35:41.079676 findanywhere-1.0.1/findanywhere/search/base.py
+-rw-r--r--   0        0        0     2405 2024-05-26 12:35:41.163677 findanywhere-1.0.1/findanywhere/search/parallel.py
+-rw-r--r--   0        0        0     1426 2024-05-26 12:35:41.159677 findanywhere-1.0.1/findanywhere/search/sequential.py
+-rw-r--r--   0        0        0      996 2024-05-26 12:35:41.062676 findanywhere-1.0.1/findanywhere/similarity/__init__.py
+-rw-r--r--   0        0        0     1937 2024-05-26 12:35:41.416679 findanywhere-1.0.1/findanywhere/similarity/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2556 2024-05-26 12:35:41.417679 findanywhere-1.0.1/findanywhere/similarity/__pycache__/common.cpython-311.pyc
+-rw-r--r--   0        0        0     5524 2024-05-26 12:35:41.418679 findanywhere-1.0.1/findanywhere/similarity/__pycache__/token.cpython-311.pyc
+-rw-r--r--   0        0        0     1773 2024-05-26 12:35:41.039676 findanywhere-1.0.1/findanywhere/similarity/common.py
+-rw-r--r--   0        0        0     3615 2024-05-26 12:35:41.071676 findanywhere-1.0.1/findanywhere/similarity/token.py
+-rw-r--r--   0        0        0      378 2024-05-26 12:35:41.143677 findanywhere-1.0.1/findanywhere/thresholds/__init__.py
+-rw-r--r--   0        0        0      724 2024-05-26 12:35:41.431679 findanywhere-1.0.1/findanywhere/thresholds/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3306 2024-05-26 12:35:41.432679 findanywhere-1.0.1/findanywhere/thresholds/__pycache__/basic.cpython-311.pyc
+-rw-r--r--   0        0        0     2173 2024-05-26 12:35:41.044676 findanywhere-1.0.1/findanywhere/thresholds/basic.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:43:06.743877 findanywhere-1.0.1/findanywhere/types/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-08 19:00:14.644813 findanywhere-1.0.1/findanywhere/types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1178 2024-05-25 14:18:32.167222 findanywhere-1.0.1/findanywhere/types/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     7465 2024-05-25 14:18:32.168222 findanywhere-1.0.1/findanywhere/types/__pycache__/factory.cpython-311.pyc
+-rw-r--r--   0        0        0     4722 2024-05-25 14:18:32.177222 findanywhere-1.0.1/findanywhere/types/__pycache__/input_data.cpython-311.pyc
+-rw-r--r--   0        0        0     4918 2024-05-26 12:35:41.393679 findanywhere-1.0.1/findanywhere/types/__pycache__/similarity.cpython-311.pyc
+-rw-r--r--   0        0        0      568 2024-05-25 14:08:35.015154 findanywhere-1.0.1/findanywhere/types/entry.py
+-rw-r--r--   0        0        0     4416 2024-05-25 14:08:34.955154 findanywhere-1.0.1/findanywhere/types/factory.py
+-rw-r--r--   0        0        0     2833 2024-05-25 14:08:34.936154 findanywhere-1.0.1/findanywhere/types/input_data.py
+-rw-r--r--   0        0        0     2681 2024-05-26 12:35:41.172677 findanywhere-1.0.1/findanywhere/types/similarity.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:19:42.473640 findanywhere-1.0.1/findanywhere/ui/__init__.py
+-rw-r--r--   0        0        0      181 2024-05-09 10:57:56.733493 findanywhere-1.0.1/findanywhere/ui/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3888 2024-05-26 12:35:41.473680 findanywhere-1.0.1/findanywhere/ui/__pycache__/console.cpython-311.pyc
+-rw-r--r--   0        0        0     2029 2024-05-26 12:35:41.116676 findanywhere-1.0.1/findanywhere/ui/console.py
+-rw-r--r--   0        0        0     1590 2024-05-26 12:53:14.409245 findanywhere-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4929 1970-01-01 00:00:00.000000 findanywhere-1.0.1/PKG-INFO
```

### Comparing `findanywhere-1.0.0/LICENSE` & `findanywhere-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/README.md` & `findanywhere-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/adapters/evaluation/__pycache__/__init__.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/adapters/evaluation/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/adapters/evaluation/__pycache__/string_distance.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/adapters/evaluation/__pycache__/string_distance.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/adapters/evaluation/string_distance.py` & `findanywhere-1.0.1/findanywhere/adapters/evaluation/string_distance.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/adapters/source/__pycache__/__init__.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/adapters/source/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/adapters/source/__pycache__/tabular.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/adapters/source/__pycache__/tabular.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/adapters/source/__pycache__/text.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/adapters/source/__pycache__/text.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/adapters/source/tabular.py` & `findanywhere-1.0.1/findanywhere/adapters/source/tabular.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/adapters/source/text.py` & `findanywhere-1.0.1/findanywhere/adapters/source/text.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/algorithms/__pycache__/strings.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/algorithms/__pycache__/strings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/algorithms/strings.py` & `findanywhere-1.0.1/findanywhere/algorithms/strings.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/ports/__pycache__/evaluation.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/ports/__pycache__/evaluation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/ports/__pycache__/source.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/ports/__pycache__/source.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/ports/evaluation.py` & `findanywhere-1.0.1/findanywhere/ports/evaluation.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/ports/source.py` & `findanywhere-1.0.1/findanywhere/ports/source.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/schema.py` & `findanywhere-1.0.1/findanywhere/schema.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/scores/__pycache__/__init__.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/scores/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/scores/__pycache__/deduction.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/scores/__pycache__/deduction.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/scores/deduction.py` & `findanywhere-1.0.1/findanywhere/scores/deduction.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/search/__pycache__/base.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/search/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/search/__pycache__/parallel.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/search/__pycache__/parallel.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/search/__pycache__/sequential.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/search/__pycache__/sequential.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/search/base.py` & `findanywhere-1.0.1/findanywhere/search/base.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/search/parallel.py` & `findanywhere-1.0.1/findanywhere/search/parallel.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/search/sequential.py` & `findanywhere-1.0.1/findanywhere/search/sequential.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/similarity/__init__.py` & `findanywhere-1.0.1/findanywhere/similarity/__init__.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/similarity/__pycache__/__init__.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/similarity/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/similarity/__pycache__/common.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/similarity/__pycache__/common.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/similarity/__pycache__/token.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/similarity/__pycache__/token.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/similarity/common.py` & `findanywhere-1.0.1/findanywhere/similarity/common.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/similarity/token.py` & `findanywhere-1.0.1/findanywhere/similarity/token.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/thresholds/__pycache__/__init__.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/thresholds/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/thresholds/__pycache__/basic.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/thresholds/__pycache__/basic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/thresholds/basic.py` & `findanywhere-1.0.1/findanywhere/thresholds/basic.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/types/__pycache__/entry.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/types/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/types/__pycache__/factory.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/types/__pycache__/factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/types/__pycache__/input_data.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/types/__pycache__/input_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/types/__pycache__/similarity.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/types/__pycache__/similarity.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/types/entry.py` & `findanywhere-1.0.1/findanywhere/types/entry.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/types/factory.py` & `findanywhere-1.0.1/findanywhere/types/factory.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/types/input_data.py` & `findanywhere-1.0.1/findanywhere/types/input_data.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/types/similarity.py` & `findanywhere-1.0.1/findanywhere/types/similarity.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/ui/__pycache__/console.cpython-311.pyc` & `findanywhere-1.0.1/findanywhere/ui/__pycache__/console.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/findanywhere/ui/console.py` & `findanywhere-1.0.1/findanywhere/ui/console.py`

 * *Files identical despite different names*

### Comparing `findanywhere-1.0.0/pyproject.toml` & `findanywhere-1.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "findanywhere"
-version = "1.0.0"
-description = ""
+version = "1.0.1"
+description = "Tool for searching data in possible malformed input data as preprocessing step for further analysis."
 authors = ["voidpointercast <voidpointercast@justmail.de>"]
 classifiers = [
     "Development Status :: 4 - Beta", "Environment :: Console", "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License", "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows :: Windows 11", "Topic :: Scientific/Engineering :: Information Analysis",
     "Programming Language :: Python :: 3.11", "Programming Language :: Python :: 3.12"
 ]
```

### Comparing `findanywhere-1.0.0/PKG-INFO` & `findanywhere-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: findanywhere
-Version: 1.0.0
-Summary: 
+Version: 1.0.1
+Summary: Tool for searching data in possible malformed input data as preprocessing step for further analysis.
 Home-page: https://gitlab.com/patrick.daniel.gress/findanywhere
 License: BSD License (BSD)
 Keywords: search,fuzzy_search,preprocessing
 Author: voidpointercast
 Author-email: voidpointercast@justmail.de
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

