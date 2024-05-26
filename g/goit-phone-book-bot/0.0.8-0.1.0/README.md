# Comparing `tmp/goit-phone-book-bot-0.0.8.tar.gz` & `tmp/goit_phone_book_bot-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goit-phone-book-bot-0.0.8.tar", last modified: Fri May 24 16:56:58 2024, max compression
+gzip compressed data, was "goit_phone_book_bot-0.1.0.tar", last modified: Sun May 26 14:32:40 2024, max compression
```

## Comparing `goit-phone-book-bot-0.0.8.tar` & `goit_phone_book_bot-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:56:58.496279 goit-phone-book-bot-0.0.8/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit-phone-book-bot-0.0.8/LICENSE
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 16:56:58.496106 goit-phone-book-bot-0.0.8/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-23 10:25:17.000000 goit-phone-book-bot-0.0.8/README.md
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:56:58.495928 goit-phone-book-bot-0.0.8/goit_phone_book_bot.egg-info/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 16:56:58.000000 goit-phone-book-bot-0.0.8/goit_phone_book_bot.egg-info/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      286 2024-05-24 16:56:58.000000 goit-phone-book-bot-0.0.8/goit_phone_book_bot.egg-info/SOURCES.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-24 16:56:58.000000 goit-phone-book-bot-0.0.8/goit_phone_book_bot.egg-info/dependency_links.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       55 2024-05-24 16:56:58.000000 goit-phone-book-bot-0.0.8/goit_phone_book_bot.egg-info/entry_points.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-24 16:56:58.000000 goit-phone-book-bot-0.0.8/goit_phone_book_bot.egg-info/requires.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-24 16:56:58.000000 goit-phone-book-bot-0.0.8/goit_phone_book_bot.egg-info/top_level.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-24 16:56:58.496319 goit-phone-book-bot-0.0.8/setup.cfg
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      822 2024-05-24 16:56:52.000000 goit-phone-book-bot-0.0.8/setup.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:32:40.256032 goit_phone_book_bot-0.1.0/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit_phone_book_bot-0.1.0/LICENSE
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      740 2024-05-26 14:32:40.255818 goit_phone_book_bot-0.1.0/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-25 18:13:42.000000 goit_phone_book_bot-0.1.0/README.md
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:32:40.255613 goit_phone_book_bot-0.1.0/goit_phone_book_bot.egg-info/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      740 2024-05-26 14:32:40.000000 goit_phone_book_bot-0.1.0/goit_phone_book_bot.egg-info/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      286 2024-05-26 14:32:40.000000 goit_phone_book_bot-0.1.0/goit_phone_book_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-26 14:32:40.000000 goit_phone_book_bot-0.1.0/goit_phone_book_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       54 2024-05-26 14:32:40.000000 goit_phone_book_bot-0.1.0/goit_phone_book_bot.egg-info/entry_points.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-26 14:32:40.000000 goit_phone_book_bot-0.1.0/goit_phone_book_bot.egg-info/requires.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-26 14:32:40.000000 goit_phone_book_bot-0.1.0/goit_phone_book_bot.egg-info/top_level.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-26 14:32:40.256070 goit_phone_book_bot-0.1.0/setup.cfg
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      822 2024-05-26 14:29:27.000000 goit_phone_book_bot-0.1.0/setup.py
```

### Comparing `goit-phone-book-bot-0.0.8/LICENSE` & `goit_phone_book_bot-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `goit-phone-book-bot-0.0.8/PKG-INFO` & `goit_phone_book_bot-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.0.8
+Version: 0.1.0
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyreadline3
+Requires-Dist: tabulate
 
 
 # Installing and launching the application
 
 - Clone 
 - python -m venv venv
 - venv\Scripts\activate
 - pip install -r requirements.txt
 - py main.py
 
 #### To select a command, a letter followed by a TAB and ENTER
 
 
 
-
-
```

### Comparing `goit-phone-book-bot-0.0.8/goit_phone_book_bot.egg-info/PKG-INFO` & `goit_phone_book_bot-0.1.0/goit_phone_book_bot.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.0.8
+Version: 0.1.0
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyreadline3
+Requires-Dist: tabulate
 
 
 # Installing and launching the application
 
 - Clone 
 - python -m venv venv
 - venv\Scripts\activate
 - pip install -r requirements.txt
 - py main.py
 
 #### To select a command, a letter followed by a TAB and ENTER
 
 
 
-
-
```

### Comparing `goit-phone-book-bot-0.0.8/setup.py` & `goit_phone_book_bot-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='goit-phone-book-bot',
-    version='0.0.8',
+    version='0.1.0',
     author='Vasyl Martyniv',
     author_email='doc.people97@gmail.com',
     description='Phone Book bot developed by team #5 - CREATORS',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VasylMartyniv/GoIT_Phone_Book_bot',
     packages=find_packages(),
```

