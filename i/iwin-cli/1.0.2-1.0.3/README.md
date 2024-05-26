# Comparing `tmp/iwin-cli-1.0.2.tar.gz` & `tmp/iwin_cli-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iwin-cli-1.0.2.tar", last modified: Mon Jul  4 04:34:55 2022, max compression
+gzip compressed data, was "iwin_cli-1.0.3.tar", last modified: Sat May 25 15:21:06 2024, max compression
```

## Comparing `iwin-cli-1.0.2.tar` & `iwin_cli-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-07-04 04:34:55.444643 iwin-cli-1.0.2/
--rw-rw-rw-   0        0        0      880 2022-07-04 04:34:55.444643 iwin-cli-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      506 2022-07-03 14:20:28.000000 iwin-cli-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-07-04 04:34:55.425732 iwin-cli-1.0.2/iwin_cli/
--rw-rw-rw-   0        0        0       19 2022-07-04 04:28:44.000000 iwin-cli-1.0.2/iwin_cli/__init__.py
--rw-rw-rw-   0        0        0     1697 2022-06-30 07:10:26.000000 iwin-cli-1.0.2/iwin_cli/__main__.py
--rw-rw-rw-   0        0        0     2382 2022-06-30 07:36:27.000000 iwin-cli-1.0.2/iwin_cli/classconfig.py
--rw-rw-rw-   0        0        0     5688 2022-07-03 14:25:54.000000 iwin-cli-1.0.2/iwin_cli/simulation.py
--rw-rw-rw-   0        0        0     2857 2022-07-03 14:29:09.000000 iwin-cli-1.0.2/iwin_cli/utils.py
--rw-rw-rw-   0        0        0     2107 2022-07-03 15:06:06.000000 iwin-cli-1.0.2/iwin_cli/zip.py
-drwxrwxrwx   0        0        0        0 2022-07-04 04:34:55.441641 iwin-cli-1.0.2/iwin_cli.egg-info/
--rw-rw-rw-   0        0        0      880 2022-07-04 04:34:55.000000 iwin-cli-1.0.2/iwin_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2022-07-04 04:34:55.000000 iwin-cli-1.0.2/iwin_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-04 04:34:55.000000 iwin-cli-1.0.2/iwin_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2022-07-04 04:34:55.000000 iwin-cli-1.0.2/iwin_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2022-07-04 04:34:55.000000 iwin-cli-1.0.2/iwin_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-07-04 04:34:55.000000 iwin-cli-1.0.2/iwin_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-04 04:34:55.445645 iwin-cli-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1006 2022-07-04 04:28:25.000000 iwin-cli-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:21:06.677093 iwin_cli-1.0.3/
+-rw-rw-rw-   0        0        0     1029 2024-05-25 15:21:06.674583 iwin_cli-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2024-05-24 13:11:52.000000 iwin_cli-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 15:21:06.634864 iwin_cli-1.0.3/iwin_cli/
+-rw-rw-rw-   0        0        0       19 2024-05-25 15:03:26.000000 iwin_cli-1.0.3/iwin_cli/__init__.py
+-rw-rw-rw-   0        0        0     1697 2024-05-24 13:11:52.000000 iwin_cli-1.0.3/iwin_cli/__main__.py
+-rw-rw-rw-   0        0        0     2382 2024-05-24 13:11:52.000000 iwin_cli-1.0.3/iwin_cli/classconfig.py
+-rw-rw-rw-   0        0        0     5688 2024-05-24 13:11:52.000000 iwin_cli-1.0.3/iwin_cli/simulation.py
+-rw-rw-rw-   0        0        0     2857 2024-05-24 13:11:52.000000 iwin_cli-1.0.3/iwin_cli/utils.py
+-rw-rw-rw-   0        0        0     2145 2024-05-25 15:04:51.000000 iwin_cli-1.0.3/iwin_cli/zip.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:21:06.667220 iwin_cli-1.0.3/iwin_cli.egg-info/
+-rw-rw-rw-   0        0        0     1029 2024-05-25 15:21:06.000000 iwin_cli-1.0.3/iwin_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-05-25 15:21:06.000000 iwin_cli-1.0.3/iwin_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 15:21:06.000000 iwin_cli-1.0.3/iwin_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-25 15:21:06.000000 iwin_cli-1.0.3/iwin_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-25 15:21:06.000000 iwin_cli-1.0.3/iwin_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 15:21:06.000000 iwin_cli-1.0.3/iwin_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 15:21:06.677093 iwin_cli-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1006 2024-05-24 13:11:52.000000 iwin_cli-1.0.3/setup.py
```

### Comparing `iwin-cli-1.0.2/PKG-INFO` & `iwin_cli-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: iwin-cli
-Version: 1.0.2
+Version: 1.0.3
 Summary: iwin commandline tool
 Home-page: https://iwin2.3thinking.cn
 Author: Learner Chen
 Author-email: learner.chen@icloud.com
 License: NO-DISTRIBUTION
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+Requires-Dist: et-xmlfile
+Requires-Dist: numpy
+Requires-Dist: openpyxl
+Requires-Dist: pandas
+Requires-Dist: XlsxWriter
+Requires-Dist: Pillow
+Requires-Dist: colorama
 
 # iWin 模拟的配置命令行工具
 
 ## 功能
 
 - 用于检查配置文件的合法性
 - 压缩图片文件，改进加载速度
@@ -32,9 +38,7 @@
 
 ```shell
 iwin-cli -s <Simulation配置文件夹路径> -c <班级数据的xlsx文件名>
 ```
 
 输入相应的目录名，或文件名。然后根据提示一步一步操作即可。
 
-
-
```

### Comparing `iwin-cli-1.0.2/iwin_cli/__main__.py` & `iwin_cli-1.0.3/iwin_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `iwin-cli-1.0.2/iwin_cli/classconfig.py` & `iwin_cli-1.0.3/iwin_cli/classconfig.py`

 * *Files identical despite different names*

### Comparing `iwin-cli-1.0.2/iwin_cli/simulation.py` & `iwin_cli-1.0.3/iwin_cli/simulation.py`

 * *Files identical despite different names*

### Comparing `iwin-cli-1.0.2/iwin_cli/utils.py` & `iwin_cli-1.0.3/iwin_cli/utils.py`

 * *Files identical despite different names*

### Comparing `iwin-cli-1.0.2/iwin_cli/zip.py` & `iwin_cli-1.0.3/iwin_cli/zip.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,16 +50,16 @@
                 file_type = "json"
             if file_type is None:
                 continue
 
             item = createItem(f, root, file_type, start_path)
             # print(f'item:{item}')
             list.append(item)
-        json_data = json.dumps(data, indent=4)
-        with open(json_fn, "w") as outfile:
+        json_data = json.dumps(data, indent=4, ensure_ascii=False)
+        with open(json_fn, "w", encoding='utf-8') as outfile:
             outfile.write(json_data)
             
         createConfig(path, config_file)
 
 def generateConfigZip(simulation_path):
     yes = input("需要生成压缩的模拟配置文件吗？[y/n?]") or 'n'
     if yes in ['y', 'Y', 'yes', 'Yes', 'YES']:
```

### Comparing `iwin-cli-1.0.2/iwin_cli.egg-info/PKG-INFO` & `iwin_cli-1.0.3/iwin_cli.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: iwin-cli
-Version: 1.0.2
+Version: 1.0.3
 Summary: iwin commandline tool
 Home-page: https://iwin2.3thinking.cn
 Author: Learner Chen
 Author-email: learner.chen@icloud.com
 License: NO-DISTRIBUTION
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+Requires-Dist: et-xmlfile
+Requires-Dist: numpy
+Requires-Dist: openpyxl
+Requires-Dist: pandas
+Requires-Dist: XlsxWriter
+Requires-Dist: Pillow
+Requires-Dist: colorama
 
 # iWin 模拟的配置命令行工具
 
 ## 功能
 
 - 用于检查配置文件的合法性
 - 压缩图片文件，改进加载速度
@@ -32,9 +38,7 @@
 
 ```shell
 iwin-cli -s <Simulation配置文件夹路径> -c <班级数据的xlsx文件名>
 ```
 
 输入相应的目录名，或文件名。然后根据提示一步一步操作即可。
 
-
-
```

### Comparing `iwin-cli-1.0.2/setup.py` & `iwin_cli-1.0.3/setup.py`

 * *Files identical despite different names*

