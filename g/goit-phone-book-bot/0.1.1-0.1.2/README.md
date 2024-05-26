# Comparing `tmp/goit_phone_book_bot-0.1.1.tar.gz` & `tmp/goit_phone_book_bot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goit_phone_book_bot-0.1.1.tar", last modified: Sun May 26 14:41:53 2024, max compression
+gzip compressed data, was "goit_phone_book_bot-0.1.2.tar", last modified: Sun May 26 14:45:22 2024, max compression
```

## Comparing `goit_phone_book_bot-0.1.1.tar` & `goit_phone_book_bot-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:41:53.588266 goit_phone_book_bot-0.1.1/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit_phone_book_bot-0.1.1/LICENSE
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      740 2024-05-26 14:41:53.588048 goit_phone_book_bot-0.1.1/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-25 18:13:42.000000 goit_phone_book_bot-0.1.1/README.md
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:41:53.587834 goit_phone_book_bot-0.1.1/goit_phone_book_bot.egg-info/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      740 2024-05-26 14:41:53.000000 goit_phone_book_bot-0.1.1/goit_phone_book_bot.egg-info/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      314 2024-05-26 14:41:53.000000 goit_phone_book_bot-0.1.1/goit_phone_book_bot.egg-info/SOURCES.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-26 14:41:53.000000 goit_phone_book_bot-0.1.1/goit_phone_book_bot.egg-info/dependency_links.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       54 2024-05-26 14:41:53.000000 goit_phone_book_bot-0.1.1/goit_phone_book_bot.egg-info/entry_points.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-26 14:41:53.000000 goit_phone_book_bot-0.1.1/goit_phone_book_bot.egg-info/requires.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-26 14:41:53.000000 goit_phone_book_bot-0.1.1/goit_phone_book_bot.egg-info/top_level.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-26 14:41:53.588312 goit_phone_book_bot-0.1.1/setup.cfg
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      822 2024-05-26 14:41:49.000000 goit_phone_book_bot-0.1.1/setup.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:41:53.587432 goit_phone_book_bot-0.1.1/src/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:38:25.000000 goit_phone_book_bot-0.1.1/src/__init__.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4400 2024-05-26 14:30:42.000000 goit_phone_book_bot-0.1.1/src/main.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:45:22.227930 goit_phone_book_bot-0.1.2/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit_phone_book_bot-0.1.2/LICENSE
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      740 2024-05-26 14:45:22.227708 goit_phone_book_bot-0.1.2/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-25 18:13:42.000000 goit_phone_book_bot-0.1.2/README.md
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:45:22.227459 goit_phone_book_bot-0.1.2/goit_phone_book_bot.egg-info/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      740 2024-05-26 14:45:22.000000 goit_phone_book_bot-0.1.2/goit_phone_book_bot.egg-info/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      314 2024-05-26 14:45:22.000000 goit_phone_book_bot-0.1.2/goit_phone_book_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-26 14:45:22.000000 goit_phone_book_bot-0.1.2/goit_phone_book_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       54 2024-05-26 14:45:22.000000 goit_phone_book_bot-0.1.2/goit_phone_book_bot.egg-info/entry_points.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-26 14:45:22.000000 goit_phone_book_bot-0.1.2/goit_phone_book_bot.egg-info/requires.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-26 14:45:22.000000 goit_phone_book_bot-0.1.2/goit_phone_book_bot.egg-info/top_level.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-26 14:45:22.227975 goit_phone_book_bot-0.1.2/setup.cfg
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      822 2024-05-26 14:45:20.000000 goit_phone_book_bot-0.1.2/setup.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:45:22.227009 goit_phone_book_bot-0.1.2/src/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:38:25.000000 goit_phone_book_bot-0.1.2/src/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4394 2024-05-26 14:44:57.000000 goit_phone_book_bot-0.1.2/src/main.py
```

### Comparing `goit_phone_book_bot-0.1.1/LICENSE` & `goit_phone_book_bot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.1.1/PKG-INFO` & `goit_phone_book_bot-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.1.1
+Version: 0.1.2
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `goit_phone_book_bot-0.1.1/goit_phone_book_bot.egg-info/PKG-INFO` & `goit_phone_book_bot-0.1.2/goit_phone_book_bot.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.1.1
+Version: 0.1.2
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `goit_phone_book_bot-0.1.1/setup.py` & `goit_phone_book_bot-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='goit-phone-book-bot',
-    version='0.1.1',
+    version='0.1.2',
     author='Vasyl Martyniv',
     author_email='doc.people97@gmail.com',
     description='Phone Book bot developed by team #5 - CREATORS',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VasylMartyniv/GoIT_Phone_Book_bot',
     packages=find_packages(),
```

### Comparing `goit_phone_book_bot-0.1.1/src/main.py` & `goit_phone_book_bot-0.1.2/src/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import readline
 
-from src.classes.notes_book import NotesBook
-from src.utils.utils import *
+from .classes.notes_book import NotesBook
+from .utils.utils import *
 
 
 # Функція для автодоповнення команд
 def completer(text, state):
     options = [cmd for cmd in commands.keys() if cmd.startswith(text)]
     if state < len(options):
         return options[state]
```

