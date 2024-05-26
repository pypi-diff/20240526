# Comparing `tmp/indicparser-0.0.9.tar.gz` & `tmp/indicparser-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indicparser-0.0.9.tar", last modified: Sat Dec 31 06:25:00 2022, max compression
+gzip compressed data, was "indicparser-0.1.0.tar", last modified: Sun May 26 17:01:09 2024, max compression
```

## Comparing `indicparser-0.0.9.tar` & `indicparser-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2022-12-31 06:25:00.570121 indicparser-0.0.9/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      835 2022-12-31 06:23:59.000000 indicparser-0.0.9/CHANGELOG.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     1067 2022-02-12 02:06:32.000000 indicparser-0.0.9/LICENSE
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       25 2022-02-12 04:15:33.000000 indicparser-0.0.9/MANIFEST.in
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     3483 2022-12-31 06:25:00.570121 indicparser-0.0.9/PKG-INFO
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     2057 2022-12-31 06:23:18.000000 indicparser-0.0.9/README.md
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2022-12-31 06:25:00.546123 indicparser-0.0.9/indicparser/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      799 2022-02-12 02:01:58.000000 indicparser-0.0.9/indicparser/__init__.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     7217 2022-12-31 06:19:18.000000 indicparser-0.0.9/indicparser/langs.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     5138 2022-10-21 00:40:49.000000 indicparser-0.0.9/indicparser/parser.py
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2022-12-31 06:25:00.546123 indicparser-0.0.9/indicparser.egg-info/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     3483 2022-12-31 06:25:00.000000 indicparser-0.0.9/indicparser.egg-info/PKG-INFO
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      435 2022-12-31 06:25:00.000000 indicparser-0.0.9/indicparser.egg-info/SOURCES.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)        1 2022-12-31 06:25:00.000000 indicparser-0.0.9/indicparser.egg-info/dependency_links.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       12 2022-12-31 06:25:00.000000 indicparser-0.0.9/indicparser.egg-info/top_level.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       38 2022-12-31 06:25:00.570121 indicparser-0.0.9/setup.cfg
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     1003 2022-12-31 06:23:30.000000 indicparser-0.0.9/setup.py
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2022-12-31 06:25:00.546123 indicparser-0.0.9/tests/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     1814 2022-02-13 22:42:08.000000 indicparser-0.0.9/tests/test.py
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2022-12-31 06:25:00.566121 indicparser-0.0.9/tests/vocab/
--rwxrwxrwx   0 ansary    (1000) ansary    (1000)   285796 2022-02-13 20:45:08.000000 indicparser-0.0.9/tests/vocab/bangla.txt
--rwxrwxrwx   0 ansary    (1000) ansary    (1000)   236486 2022-02-13 20:45:40.000000 indicparser-0.0.9/tests/vocab/gujrati.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)   210297 2022-02-13 20:46:08.000000 indicparser-0.0.9/tests/vocab/hindi.txt
--rwxrwxrwx   0 ansary    (1000) ansary    (1000)   461552 2022-02-13 20:45:55.000000 indicparser-0.0.9/tests/vocab/malyalam.txt
--rwxrwxrwx   0 ansary    (1000) ansary    (1000)   302857 2022-02-13 20:46:17.000000 indicparser-0.0.9/tests/vocab/odiya.txt
--rwxrwxrwx   0 ansary    (1000) ansary    (1000)   200576 2022-02-13 20:46:29.000000 indicparser-0.0.9/tests/vocab/panjabi.txt
--rwxrwxrwx   0 ansary    (1000) ansary    (1000)   403618 2022-02-13 20:45:27.000000 indicparser-0.0.9/tests/vocab/tamil.txt
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-05-26 17:01:09.557949 indicparser-0.1.0/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      981 2024-05-26 16:59:57.000000 indicparser-0.1.0/CHANGELOG.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     1067 2024-05-26 16:58:40.000000 indicparser-0.1.0/LICENSE
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       25 2024-05-26 16:58:40.000000 indicparser-0.1.0/MANIFEST.in
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     5561 2024-05-26 17:01:09.557949 indicparser-0.1.0/PKG-INFO
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     4009 2024-05-26 17:00:52.000000 indicparser-0.1.0/README.md
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-05-26 17:01:09.553951 indicparser-0.1.0/indicparser/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      799 2024-05-26 16:58:40.000000 indicparser-0.1.0/indicparser/__init__.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     7245 2024-05-26 16:58:40.000000 indicparser-0.1.0/indicparser/langs.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     5138 2024-05-26 16:58:40.000000 indicparser-0.1.0/indicparser/parser.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-05-26 17:01:09.553951 indicparser-0.1.0/indicparser.egg-info/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     5561 2024-05-26 17:01:09.000000 indicparser-0.1.0/indicparser.egg-info/PKG-INFO
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      435 2024-05-26 17:01:09.000000 indicparser-0.1.0/indicparser.egg-info/SOURCES.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)        1 2024-05-26 17:01:09.000000 indicparser-0.1.0/indicparser.egg-info/dependency_links.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       12 2024-05-26 17:01:09.000000 indicparser-0.1.0/indicparser.egg-info/top_level.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       38 2024-05-26 17:01:09.557949 indicparser-0.1.0/setup.cfg
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     1003 2024-05-26 16:59:22.000000 indicparser-0.1.0/setup.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-05-26 17:01:09.553951 indicparser-0.1.0/tests/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     1814 2024-05-26 16:58:40.000000 indicparser-0.1.0/tests/test.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-05-26 17:01:09.553951 indicparser-0.1.0/tests/vocab/
+-rwxrwxr-x   0 ansary    (1000) ansary    (1000)   285796 2024-05-26 16:58:40.000000 indicparser-0.1.0/tests/vocab/bangla.txt
+-rwxrwxr-x   0 ansary    (1000) ansary    (1000)   236486 2024-05-26 16:58:40.000000 indicparser-0.1.0/tests/vocab/gujrati.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)   210297 2024-05-26 16:58:40.000000 indicparser-0.1.0/tests/vocab/hindi.txt
+-rwxrwxr-x   0 ansary    (1000) ansary    (1000)   461552 2024-05-26 16:58:40.000000 indicparser-0.1.0/tests/vocab/malyalam.txt
+-rwxrwxr-x   0 ansary    (1000) ansary    (1000)   302857 2024-05-26 16:58:40.000000 indicparser-0.1.0/tests/vocab/odiya.txt
+-rwxrwxr-x   0 ansary    (1000) ansary    (1000)   200576 2024-05-26 16:58:40.000000 indicparser-0.1.0/tests/vocab/panjabi.txt
+-rwxrwxr-x   0 ansary    (1000) ansary    (1000)   403618 2024-05-26 16:58:40.000000 indicparser-0.1.0/tests/vocab/tamil.txt
```

### Comparing `indicparser-0.0.9/CHANGELOG.txt` & `indicparser-0.1.0/CHANGELOG.txt`

 * *Files 4% similar despite different names*

```diff
@@ -39,8 +39,16 @@
 
 0.0.8 (21/10/2022)
 -------------------
 - allow middle Connector
 
 0.0.9 (31/12/2022)
 -------------------
-- added sylheti nagri
+- added sylheti nagri
+
+0.0.10 (31/12/2022)
+-------------------
+- added sylheti nagri alternate hosonto
+
+0.1.0 (26/05/2024)
+-------------------
+- added proper citation
```

### Comparing `indicparser-0.0.9/LICENSE` & `indicparser-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `indicparser-0.0.9/indicparser/__init__.py` & `indicparser-0.1.0/indicparser/__init__.py`

 * *Files identical despite different names*

### Comparing `indicparser-0.0.9/indicparser/langs.py` & `indicparser-0.1.0/indicparser/langs.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 #------------------------------------------------------------------------------------------------------------------------------------------------------
 #######################################################################################################################################################
 #------------------------------------------------------------------------------------------------------------------------------------------------------
 class nagri:
     iden                  =      "nagri"
     # for grapheme decomp
     vowel_diacritics       =    ['ꠣ', 'ꠤ', 'ꠥ', 'ꠦ', 'ꠧ']
-    consonant_diacritics   =    ['ꠋ', 'ꠂ'] 
+    consonant_diacritics   =    ['ꠋ', 'ꠂ']+['꠬'] # alternate hosonto 
     connector              =    '꠆'
     
 #------------------------------------------------------------------------------------------------------------------------------------------------------
 #######################################################################################################################################################
 #------------------------------------------------------------------------------------------------------------------------------------------------------
 #----------------------------------------- add all language info-------------------------------------------------------------
 languages={}
```

### Comparing `indicparser-0.0.9/indicparser/parser.py` & `indicparser-0.1.0/indicparser/parser.py`

 * *Files identical despite different names*

### Comparing `indicparser-0.0.9/setup.py` & `indicparser-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='indicparser',
-  version='0.0.9',
+  version='0.1.0',
   description='Grapheme Parser for indic languages',
   long_description=open('README.md',encoding="utf-8").read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/mnansary/indicparser',  
   author='Bengali.AI',
   author_email='research.bengaliai@gmail.com',
   license='MIT',
```

### Comparing `indicparser-0.0.9/tests/test.py` & `indicparser-0.1.0/tests/test.py`

 * *Files identical despite different names*

### Comparing `indicparser-0.0.9/tests/vocab/bangla.txt` & `indicparser-0.1.0/tests/vocab/bangla.txt`

 * *Files identical despite different names*

### Comparing `indicparser-0.0.9/tests/vocab/gujrati.txt` & `indicparser-0.1.0/tests/vocab/gujrati.txt`

 * *Files identical despite different names*

### Comparing `indicparser-0.0.9/tests/vocab/hindi.txt` & `indicparser-0.1.0/tests/vocab/hindi.txt`

 * *Files identical despite different names*

### Comparing `indicparser-0.0.9/tests/vocab/malyalam.txt` & `indicparser-0.1.0/tests/vocab/malyalam.txt`

 * *Files identical despite different names*

### Comparing `indicparser-0.0.9/tests/vocab/odiya.txt` & `indicparser-0.1.0/tests/vocab/odiya.txt`

 * *Files identical despite different names*

### Comparing `indicparser-0.0.9/tests/vocab/panjabi.txt` & `indicparser-0.1.0/tests/vocab/panjabi.txt`

 * *Files identical despite different names*

### Comparing `indicparser-0.0.9/tests/vocab/tamil.txt` & `indicparser-0.1.0/tests/vocab/tamil.txt`

 * *Files identical despite different names*

