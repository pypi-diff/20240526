# Comparing `tmp/workutils-0.0.7.tar.gz` & `tmp/workutils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workutils-0.0.7.tar", last modified: Tue Mar 12 15:04:27 2024, max compression
+gzip compressed data, was "workutils-0.0.8.tar", last modified: Sun May 26 10:49:05 2024, max compression
```

## Comparing `workutils-0.0.7.tar` & `workutils-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 15:04:27.861191 workutils-0.0.7/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-03-12 13:14:37.000000 workutils-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4907 2024-03-12 15:04:27.861191 workutils-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4277 2024-03-12 14:51:40.000000 workutils-0.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-12 15:04:27.861191 workutils-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2167 2024-03-12 15:03:32.000000 workutils-0.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 15:04:27.861191 workutils-0.0.7/workutils/
--rw-r--r--   0 root         (0) root         (0)       24 2024-03-12 13:14:37.000000 workutils-0.0.7/workutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7963 2024-03-12 15:02:38.000000 workutils-0.0.7/workutils/workutils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 15:04:27.861191 workutils-0.0.7/workutils.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     4907 2024-03-12 15:04:27.000000 workutils-0.0.7/workutils.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      271 2024-03-12 15:04:27.000000 workutils-0.0.7/workutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-03-12 15:04:27.000000 workutils-0.0.7/workutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       55 2024-03-12 15:04:27.000000 workutils-0.0.7/workutils.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2024-03-12 15:04:27.000000 workutils-0.0.7/workutils.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-03-12 15:04:27.000000 workutils-0.0.7/workutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 10:49:05.218398 workutils-0.0.8/
+-rwxrwxrwx   0 root         (0) root         (0)     1066 2024-03-13 12:08:57.000000 workutils-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6254 2024-05-26 10:49:05.218398 workutils-0.0.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5624 2024-05-26 10:42:24.000000 workutils-0.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-26 10:49:05.218398 workutils-0.0.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2167 2024-05-26 10:38:20.000000 workutils-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 10:49:05.214398 workutils-0.0.8/workutils/
+-rwxrwxrwx   0 root         (0) root         (0)       24 2024-03-13 12:08:57.000000 workutils-0.0.8/workutils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10534 2024-05-26 10:30:13.000000 workutils-0.0.8/workutils/workutils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 10:49:05.218398 workutils-0.0.8/workutils.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     6254 2024-05-26 10:49:05.000000 workutils-0.0.8/workutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-26 10:49:05.000000 workutils-0.0.8/workutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-26 10:49:05.000000 workutils-0.0.8/workutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       55 2024-05-26 10:49:05.000000 workutils-0.0.8/workutils.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2024-05-26 10:49:05.000000 workutils-0.0.8/workutils.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-05-26 10:49:05.000000 workutils-0.0.8/workutils.egg-info/top_level.txt
```

### Comparing `workutils-0.0.7/LICENSE` & `workutils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `workutils-0.0.7/README.md` & `workutils-0.0.8/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,108 @@
 # workutils
-A tool to solve daily work
+A tool to solve daily work including file encoding conversion, keyword search, and file type analysis.
 
 ## Installation
-You can install, upgrade, uninstall workutils with these commands(without $):
+You can install, upgrade, or uninstall workutils with these commands:
 ```shell
 $ pip install workutils
 $ pip install --upgrade workutils
-$ pip unstall workutils
+$ pip uninstall workutils
 ```
 
 ## Help
 
 ```shell
 $ workutils -h
-usage: workutils [-h] [-s SUFFIX] [-k KEYWORDS] [-a] [-o OUTPUT] directory
-
+usage: workutils [-h] {convert,query,analyze} ...
 A tool for daily work
 
+optional arguments:
+  -h, --help            show this help message and exit
+
+subcommands:
+  {convert,query,analyze}
+    convert             Convert the encoding of all files in the specified directory and its subdirectories.
+    query               Query the encoding of a specified file.
+    analyze             Analyze the file types and keyword occurrences in the specified directory and its subdirectories.
+```
+
+### Convert the encoding of files
+
+```shell
+$ workutils convert -h
+usage: workutils convert [-h] [-s SUFFIX] directory target_encoding
+
 positional arguments:
-  directory             Folder path to analyze
+  directory             The directory to process
+  target_encoding       The target encoding format, e.g., 'utf-8'
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -s SUFFIX, --suffix SUFFIX
-                        File suffix to analyze
+                        Specify the file extension to process, e.g., '.txt'
+```
+
+### Query the encoding of a file
+
+```shell
+$ workutils query -h
+usage: workutils query [-h] file_path
+
+positional arguments:
+  file_path             The file path to query
+
+optional arguments:
+  -h, --help            show this help message and exit
+```
+
+### Analyze file types and keyword occurrences
+
+```shell
+$ workutils analyze -h
+usage: workutils analyze [-h] [-s SUFFIX] [-k KEYWORDS] [-a] [-o OUTPUT] directory
+
+positional arguments:
+  directory             The directory to analyze
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -s SUFFIX, --suffix SUFFIX
+                        Specify the file extension to analyze
   -k KEYWORDS, --keywords KEYWORDS
-                        Count Keywords in all files, such as 'key word1','key word2'
+                        Count keywords in all files, such as 'keyword1,keyword2'
   -a, --all-files       Traverse all files, including hidden files
   -o OUTPUT, --output OUTPUT
-                        File path to save the result
-
+                        The file path to save the result
 ```
 
 ## Examples
 
-1. Select the folder path to analyze
+### Convert the encoding of files
+
+1. **Convert all `.txt` files in a directory to `utf-8` encoding**:
+
+```shell
+$ workutils convert ./directory utf-8 -s .txt
+```
+
+### Query the encoding of a file
+
+2. **Query the encoding of a specific file**:
+
+```shell
+$ workutils query /path/to/file.txt
+```
+
+### Analyze file types and keyword occurrences
+
+3. **Analyze the file types in a directory**:
 
 ```shell
-$ workutils ../
+$ workutils analyze ../
 E:\workutils\a.txt
 E:\workutils\LICENSE
 E:\workutils\README.md
 E:\workutils\workutils\workutils.py
 E:\workutils\workutils\__init__.py
 ========================================
 Suffix    Counts
@@ -49,37 +110,35 @@
 .txt      1
           1
 .md       1
 .py       2
 ----------------------------------------
 Total     5
 ========================================
-$
 ```
 
-2. Select the folder path and specify the files with a certain suffix to analyze.
+4. **Select the folder path and specify the file suffix to analyze**:
 
 ```shell
-$ workutils ../ -s py
+$ workutils analyze ../ -s py
 E:\workutils\workutils\workutils.py
 E:\workutils\workutils\__init__.py
 ========================================
 Suffix    Counts
 ----------------------------------------
 .py       2
 ----------------------------------------
 Total     2
 ========================================
-$ 
 ```
 
-3. Traverse all files, including hidden files
+5. **Traverse all files, including hidden files**:
 
 ```shell
-$ workutils ../ -a   
+$ workutils analyze ../ -a   
 E:\workutils\a.txt
 E:\workutils\LICENSE
 E:\workutils\README.md
 E:\workutils\.git\config
 ...
 E:\workutils\.git\refs\remotes\origin\HEAD
 E:\workutils\workutils\workutils.py
@@ -93,63 +152,56 @@
 .sample   13
 .idx      1
 .pack     1
 .py       2
 ----------------------------------------
 Total     34
 ========================================
-PS $ 
-
 ```
 
-4. Input result file path to save the result
+6. **Save the result to a file**:
 
 ```shell
-$ workutils ../ -s py -o result.txt
+$ workutils analyze ../ -s py -o result.txt
 E:\workutils\workutils\workutils.py
 E:\workutils\workutils\__init__.py
 ========================================
 Suffix    Counts
 ----------------------------------------
 .py       2
 ----------------------------------------
 Total     2
 ========================================
 The result has been saved to the E:\workutils\workutils\result.txt file.
-$ 
 ```
 
-result.txt
+Content of `result.txt`:
 ```text
 E:\workutils\workutils\workutils.py
 E:\workutils\workutils\__init__.py
-
 ```
 
-5. Find keywords and count occurrences in all files
+7. **Find keywords and count occurrences in all files**:
 
 ```shell
-$ workutils ./ -s log -k 'AS0100504GN_2' -o a.txt
+$ workutils analyze ./ -s log -k 'AS0100504GN_2' -o a.txt
 E:\workutils\workutils\1111.log
 E:\workutils\workutils\a\a.log
 E:\workutils\workutils\b\test.log
 E:\workutils\workutils\c\c.log
 ==================================================
 Suffix              Counts
 --------------------------------------------------
 .log                4
 --------------------------------------------------
 Total               4
 ==================================================
 
-
-100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 4/4 [00:00<00:00,  3.76it/s]
+100%|████████████████████████████████████████████| 4/4 [00:00<00:00,  3.76it/s]
 ==================================================
 Keyword             Matches             File Name
 --------------------------------------------------
 AS0100504GN_2       32                  1111.log
 --------------------------------------------------
 ==================================================
-
 The result has been saved to the E:\workutils\workutils\a.txt file.
-$ 
 ```
```

### Comparing `workutils-0.0.7/setup.py` & `workutils-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Package meta-data.
 NAME = 'workutils'
 DESCRIPTION = 'A tool to solve daily work.'
 URL = 'https://github.com/ldspdvsun/workutils'
 EMAIL = 'ldspdvsun@gmail.com'
 AUTHOR = 'MengYue Sun'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = ['chardet','tqdm']
 
 # What packages are optional?
 EXTRAS = {}
```

