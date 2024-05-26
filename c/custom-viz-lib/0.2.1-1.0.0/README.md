# Comparing `tmp/custom_viz_lib-0.2.1.tar.gz` & `tmp/custom_viz_lib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_viz_lib-0.2.1.tar", last modified: Sat May 25 18:52:18 2024, max compression
+gzip compressed data, was "custom_viz_lib-1.0.0.tar", last modified: Sat May 25 19:04:24 2024, max compression
```

## Comparing `custom_viz_lib-0.2.1.tar` & `custom_viz_lib-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,17 @@
-drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 18:52:18.318616 custom_viz_lib-0.2.1/
--rw-r--r--   0 okadaaso   (501) staff       (20)     1542 2024-05-25 18:52:18.318460 custom_viz_lib-0.2.1/PKG-INFO
--rw-r--r--   0 okadaaso   (501) staff       (20)     1123 2024-05-25 18:38:35.000000 custom_viz_lib-0.2.1/README.md
-drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 18:52:18.315839 custom_viz_lib-0.2.1/custom_viz_lib/
--rw-r--r--   0 okadaaso   (501) staff       (20)      123 2024-05-25 18:04:26.000000 custom_viz_lib-0.2.1/custom_viz_lib/__init__.py
--rw-r--r--   0 okadaaso   (501) staff       (20)     1171 2024-05-25 18:04:46.000000 custom_viz_lib-0.2.1/custom_viz_lib/chart.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      247 2024-05-25 18:05:12.000000 custom_viz_lib-0.2.1/custom_viz_lib/data_loader.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      163 2024-05-25 18:05:02.000000 custom_viz_lib-0.2.1/custom_viz_lib/theme.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      289 2024-05-25 18:05:21.000000 custom_viz_lib-0.2.1/custom_viz_lib/utils.py
-drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 18:52:18.316929 custom_viz_lib-0.2.1/custom_viz_lib.egg-info/
--rw-r--r--   0 okadaaso   (501) staff       (20)     1542 2024-05-25 18:52:17.000000 custom_viz_lib-0.2.1/custom_viz_lib.egg-info/PKG-INFO
--rw-r--r--   0 okadaaso   (501) staff       (20)      440 2024-05-25 18:52:18.000000 custom_viz_lib-0.2.1/custom_viz_lib.egg-info/SOURCES.txt
--rw-r--r--   0 okadaaso   (501) staff       (20)        1 2024-05-25 18:52:18.000000 custom_viz_lib-0.2.1/custom_viz_lib.egg-info/dependency_links.txt
--rw-r--r--   0 okadaaso   (501) staff       (20)       26 2024-05-25 18:52:18.000000 custom_viz_lib-0.2.1/custom_viz_lib.egg-info/requires.txt
--rw-r--r--   0 okadaaso   (501) staff       (20)       21 2024-05-25 18:52:18.000000 custom_viz_lib-0.2.1/custom_viz_lib.egg-info/top_level.txt
--rw-r--r--   0 okadaaso   (501) staff       (20)       38 2024-05-25 18:52:18.318672 custom_viz_lib-0.2.1/setup.cfg
--rw-r--r--   0 okadaaso   (501) staff       (20)      651 2024-05-25 18:52:04.000000 custom_viz_lib-0.2.1/setup.py
-drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 18:52:18.318109 custom_viz_lib-0.2.1/tests/
--rw-r--r--   0 okadaaso   (501) staff       (20)       38 2024-05-25 18:06:04.000000 custom_viz_lib-0.2.1/tests/__init__.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      668 2024-05-25 18:06:12.000000 custom_viz_lib-0.2.1/tests/test_chart.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      290 2024-05-25 18:06:33.000000 custom_viz_lib-0.2.1/tests/test_data_loader.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      334 2024-05-25 18:06:23.000000 custom_viz_lib-0.2.1/tests/test_theme.py
--rw-r--r--   0 okadaaso   (501) staff       (20)      304 2024-05-25 18:06:44.000000 custom_viz_lib-0.2.1/tests/test_utils.py
+drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 19:04:24.750238 custom_viz_lib-1.0.0/
+-rw-r--r--   0 okadaaso   (501) staff       (20)     2928 2024-05-25 19:04:24.750057 custom_viz_lib-1.0.0/PKG-INFO
+-rw-r--r--   0 okadaaso   (501) staff       (20)     2509 2024-05-25 19:04:09.000000 custom_viz_lib-1.0.0/README.md
+drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 19:04:24.748848 custom_viz_lib-1.0.0/custom_viz_lib/
+-rw-r--r--   0 okadaaso   (501) staff       (20)      123 2024-05-25 18:04:26.000000 custom_viz_lib-1.0.0/custom_viz_lib/__init__.py
+-rw-r--r--   0 okadaaso   (501) staff       (20)     1171 2024-05-25 18:04:46.000000 custom_viz_lib-1.0.0/custom_viz_lib/chart.py
+-rw-r--r--   0 okadaaso   (501) staff       (20)      247 2024-05-25 18:05:12.000000 custom_viz_lib-1.0.0/custom_viz_lib/data_loader.py
+-rw-r--r--   0 okadaaso   (501) staff       (20)      163 2024-05-25 18:05:02.000000 custom_viz_lib-1.0.0/custom_viz_lib/theme.py
+-rw-r--r--   0 okadaaso   (501) staff       (20)      289 2024-05-25 18:05:21.000000 custom_viz_lib-1.0.0/custom_viz_lib/utils.py
+drwxr-xr-x   0 okadaaso   (501) staff       (20)        0 2024-05-25 19:04:24.749731 custom_viz_lib-1.0.0/custom_viz_lib.egg-info/
+-rw-r--r--   0 okadaaso   (501) staff       (20)     2928 2024-05-25 19:04:24.000000 custom_viz_lib-1.0.0/custom_viz_lib.egg-info/PKG-INFO
+-rw-r--r--   0 okadaaso   (501) staff       (20)      336 2024-05-25 19:04:24.000000 custom_viz_lib-1.0.0/custom_viz_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 okadaaso   (501) staff       (20)        1 2024-05-25 19:04:24.000000 custom_viz_lib-1.0.0/custom_viz_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 okadaaso   (501) staff       (20)       26 2024-05-25 19:04:24.000000 custom_viz_lib-1.0.0/custom_viz_lib.egg-info/requires.txt
+-rw-r--r--   0 okadaaso   (501) staff       (20)       15 2024-05-25 19:04:24.000000 custom_viz_lib-1.0.0/custom_viz_lib.egg-info/top_level.txt
+-rw-r--r--   0 okadaaso   (501) staff       (20)       38 2024-05-25 19:04:24.750297 custom_viz_lib-1.0.0/setup.cfg
+-rw-r--r--   0 okadaaso   (501) staff       (20)      651 2024-05-25 19:01:41.000000 custom_viz_lib-1.0.0/setup.py
```

### Comparing `custom_viz_lib-0.2.1/PKG-INFO` & `custom_viz_lib-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom_viz_lib
-Version: 0.2.1
+Version: 1.0.0
 Summary: A customizable data visualization library
 Author: Aso Okada
 Author-email: s2222083@stu.musashino-u.ac.jp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,24 +41,76 @@
 
 # チャートの作成
 bar_chart = chart.BarChart(data)
 bar_chart.apply_theme(theme.DarkTheme())
 bar_chart.show()
 ```
 
-## 使用例（Google Colabで使用する場合）
+## 使用例1（Google Colabで使用し、バーチャートの作成する）
 ```python
 !pip install custom_viz_lib
 
 from custom_viz_lib.chart import BarChart
 from custom_viz_lib.theme import DarkTheme
 
 # サンプルデータ
 data = [1, 2, 3, 4, 5]
 chart = BarChart(data)
 chart.apply_theme(DarkTheme())
 chart.show()
 ```
 
+## 使用例2（Google Colabで使用し、ラインチャートの作成する）
+```python
+!pip install custom_viz_lib
+
+from custom_viz_lib.chart import LineChart
+from custom_viz_lib.theme import LightTheme
+
+# サンプルデータ
+data = [10, 20, 15, 25, 30]
+chart = LineChart(data)
+chart.apply_theme(LightTheme())
+chart.show()
+```
+
+## 使用例3（Google Colabで使用し、CSVファイルからデータを読み込んでバーチャートを作成する）
+```python
+!pip install custom_viz_lib
+
+import pandas as pd
+from custom_viz_lib.chart import BarChart
+from custom_viz_lib.theme import DarkTheme
+from custom_viz_lib.data_loader import load_csv
+
+# CSVファイルのパス
+file_path = 'path/to/your/data.csv'
+
+# データの読み込み
+data = load_csv(file_path)['column_name'].tolist()
+chart = BarChart(data)
+chart.apply_theme(DarkTheme())
+chart.show()
+```
+
+## 使用例4（Google Colabで使用し、データを正規化してラインチャートを作成する）
+```python
+!pip install custom_viz_lib
+
+from custom_viz_lib.chart import LineChart
+from custom_viz_lib.theme import LightTheme
+from custom_viz_lib.utils import normalize_data
+
+# サンプルデータ
+data = [10, 20, 15, 25, 30]
+
+# データの正規化
+normalized_data = normalize_data(data)
+chart = LineChart(normalized_data)
+chart.apply_theme(LightTheme())
+
+chart.show()
+```
+
 ## ライセンス
 This project is licensed under the MIT License.
```

### Comparing `custom_viz_lib-0.2.1/custom_viz_lib/chart.py` & `custom_viz_lib-1.0.0/custom_viz_lib/chart.py`

 * *Files identical despite different names*

### Comparing `custom_viz_lib-0.2.1/custom_viz_lib.egg-info/PKG-INFO` & `custom_viz_lib-1.0.0/custom_viz_lib.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-viz-lib
-Version: 0.2.1
+Version: 1.0.0
 Summary: A customizable data visualization library
 Author: Aso Okada
 Author-email: s2222083@stu.musashino-u.ac.jp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,24 +41,76 @@
 
 # チャートの作成
 bar_chart = chart.BarChart(data)
 bar_chart.apply_theme(theme.DarkTheme())
 bar_chart.show()
 ```
 
-## 使用例（Google Colabで使用する場合）
+## 使用例1（Google Colabで使用し、バーチャートの作成する）
 ```python
 !pip install custom_viz_lib
 
 from custom_viz_lib.chart import BarChart
 from custom_viz_lib.theme import DarkTheme
 
 # サンプルデータ
 data = [1, 2, 3, 4, 5]
 chart = BarChart(data)
 chart.apply_theme(DarkTheme())
 chart.show()
 ```
 
+## 使用例2（Google Colabで使用し、ラインチャートの作成する）
+```python
+!pip install custom_viz_lib
+
+from custom_viz_lib.chart import LineChart
+from custom_viz_lib.theme import LightTheme
+
+# サンプルデータ
+data = [10, 20, 15, 25, 30]
+chart = LineChart(data)
+chart.apply_theme(LightTheme())
+chart.show()
+```
+
+## 使用例3（Google Colabで使用し、CSVファイルからデータを読み込んでバーチャートを作成する）
+```python
+!pip install custom_viz_lib
+
+import pandas as pd
+from custom_viz_lib.chart import BarChart
+from custom_viz_lib.theme import DarkTheme
+from custom_viz_lib.data_loader import load_csv
+
+# CSVファイルのパス
+file_path = 'path/to/your/data.csv'
+
+# データの読み込み
+data = load_csv(file_path)['column_name'].tolist()
+chart = BarChart(data)
+chart.apply_theme(DarkTheme())
+chart.show()
+```
+
+## 使用例4（Google Colabで使用し、データを正規化してラインチャートを作成する）
+```python
+!pip install custom_viz_lib
+
+from custom_viz_lib.chart import LineChart
+from custom_viz_lib.theme import LightTheme
+from custom_viz_lib.utils import normalize_data
+
+# サンプルデータ
+data = [10, 20, 15, 25, 30]
+
+# データの正規化
+normalized_data = normalize_data(data)
+chart = LineChart(normalized_data)
+chart.apply_theme(LightTheme())
+
+chart.show()
+```
+
 ## ライセンス
 This project is licensed under the MIT License.
```

### Comparing `custom_viz_lib-0.2.1/setup.py` & `custom_viz_lib-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='custom_viz_lib',
-    version='0.2.1',
+    version='1.0.0',
     description='A customizable data visualization library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Aso Okada',
     author_email='s2222083@stu.musashino-u.ac.jp',
     packages=find_packages(),
     install_requires=[
```

