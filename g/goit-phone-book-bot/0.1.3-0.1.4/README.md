# Comparing `tmp/goit_phone_book_bot-0.1.3.tar.gz` & `tmp/goit_phone_book_bot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goit_phone_book_bot-0.1.3.tar", last modified: Sun May 26 14:47:48 2024, max compression
+gzip compressed data, was "goit_phone_book_bot-0.1.4.tar", last modified: Sun May 26 14:49:03 2024, max compression
```

## Comparing `goit_phone_book_bot-0.1.3.tar` & `goit_phone_book_bot-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:47:48.328241 goit_phone_book_bot-0.1.3/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit_phone_book_bot-0.1.3/LICENSE
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      740 2024-05-26 14:47:48.328017 goit_phone_book_bot-0.1.3/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-25 18:13:42.000000 goit_phone_book_bot-0.1.3/README.md
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:47:48.327769 goit_phone_book_bot-0.1.3/goit_phone_book_bot.egg-info/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      740 2024-05-26 14:47:48.000000 goit_phone_book_bot-0.1.3/goit_phone_book_bot.egg-info/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      585 2024-05-26 14:47:48.000000 goit_phone_book_bot-0.1.3/goit_phone_book_bot.egg-info/SOURCES.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-26 14:47:48.000000 goit_phone_book_bot-0.1.3/goit_phone_book_bot.egg-info/dependency_links.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       54 2024-05-26 14:47:48.000000 goit_phone_book_bot-0.1.3/goit_phone_book_bot.egg-info/entry_points.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-26 14:47:48.000000 goit_phone_book_bot-0.1.3/goit_phone_book_bot.egg-info/requires.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-26 14:47:48.000000 goit_phone_book_bot-0.1.3/goit_phone_book_bot.egg-info/top_level.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-26 14:47:48.328289 goit_phone_book_bot-0.1.3/setup.cfg
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      822 2024-05-26 14:47:33.000000 goit_phone_book_bot-0.1.3/setup.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:47:48.324370 goit_phone_book_bot-0.1.3/src/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:38:25.000000 goit_phone_book_bot-0.1.3/src/__init__.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:47:48.327005 goit_phone_book_bot-0.1.3/src/classes/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:46:19.000000 goit_phone_book_bot-0.1.3/src/classes/__init__.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      408 2024-05-25 18:33:44.000000 goit_phone_book_bot-0.1.3/src/classes/address.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4492 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.1.3/src/classes/address_book.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1703 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.1.3/src/classes/birthday.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      915 2024-05-25 22:34:07.000000 goit_phone_book_bot-0.1.3/src/classes/email.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      126 2024-05-25 18:13:46.000000 goit_phone_book_bot-0.1.3/src/classes/field.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      251 2024-05-23 17:44:13.000000 goit_phone_book_bot-0.1.3/src/classes/note.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     3102 2024-05-25 18:58:18.000000 goit_phone_book_bot-0.1.3/src/classes/notes_book.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1240 2024-05-25 22:34:07.000000 goit_phone_book_bot-0.1.3/src/classes/phone.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4245 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.1.3/src/classes/record.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4394 2024-05-26 14:46:56.000000 goit_phone_book_bot-0.1.3/src/main.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:47:48.327374 goit_phone_book_bot-0.1.3/src/utils/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:46:28.000000 goit_phone_book_bot-0.1.3/src/utils/__init__.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)    10711 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.1.3/src/utils/utils.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:49:03.233195 goit_phone_book_bot-0.1.4/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit_phone_book_bot-0.1.4/LICENSE
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      740 2024-05-26 14:49:03.232970 goit_phone_book_bot-0.1.4/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-25 18:13:42.000000 goit_phone_book_bot-0.1.4/README.md
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:49:03.232717 goit_phone_book_bot-0.1.4/goit_phone_book_bot.egg-info/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      740 2024-05-26 14:49:03.000000 goit_phone_book_bot-0.1.4/goit_phone_book_bot.egg-info/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      637 2024-05-26 14:49:03.000000 goit_phone_book_bot-0.1.4/goit_phone_book_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-26 14:49:03.000000 goit_phone_book_bot-0.1.4/goit_phone_book_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       54 2024-05-26 14:49:03.000000 goit_phone_book_bot-0.1.4/goit_phone_book_bot.egg-info/entry_points.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-26 14:49:03.000000 goit_phone_book_bot-0.1.4/goit_phone_book_bot.egg-info/requires.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-26 14:49:03.000000 goit_phone_book_bot-0.1.4/goit_phone_book_bot.egg-info/top_level.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-26 14:49:03.233236 goit_phone_book_bot-0.1.4/setup.cfg
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      822 2024-05-26 14:48:59.000000 goit_phone_book_bot-0.1.4/setup.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:49:03.225452 goit_phone_book_bot-0.1.4/src/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:38:25.000000 goit_phone_book_bot-0.1.4/src/__init__.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:49:03.228234 goit_phone_book_bot-0.1.4/src/classes/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:46:19.000000 goit_phone_book_bot-0.1.4/src/classes/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      408 2024-05-25 18:33:44.000000 goit_phone_book_bot-0.1.4/src/classes/address.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4492 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.1.4/src/classes/address_book.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1703 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.1.4/src/classes/birthday.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      915 2024-05-25 22:34:07.000000 goit_phone_book_bot-0.1.4/src/classes/email.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      126 2024-05-25 18:13:46.000000 goit_phone_book_bot-0.1.4/src/classes/field.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      251 2024-05-23 17:44:13.000000 goit_phone_book_bot-0.1.4/src/classes/note.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     3102 2024-05-25 18:58:18.000000 goit_phone_book_bot-0.1.4/src/classes/notes_book.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1240 2024-05-25 22:34:07.000000 goit_phone_book_bot-0.1.4/src/classes/phone.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4245 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.1.4/src/classes/record.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:49:03.230316 goit_phone_book_bot-0.1.4/src/constants/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:48:38.000000 goit_phone_book_bot-0.1.4/src/constants/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     2001 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.1.4/src/constants/commands.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4394 2024-05-26 14:46:56.000000 goit_phone_book_bot-0.1.4/src/main.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:49:03.230683 goit_phone_book_bot-0.1.4/src/utils/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:46:28.000000 goit_phone_book_bot-0.1.4/src/utils/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)    10711 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.1.4/src/utils/utils.py
```

### Comparing `goit_phone_book_bot-0.1.3/LICENSE` & `goit_phone_book_bot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.1.3/PKG-INFO` & `goit_phone_book_bot-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.1.3
+Version: 0.1.4
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `goit_phone_book_bot-0.1.3/goit_phone_book_bot.egg-info/PKG-INFO` & `goit_phone_book_bot-0.1.4/goit_phone_book_bot.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.1.3
+Version: 0.1.4
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `goit_phone_book_bot-0.1.3/goit_phone_book_bot.egg-info/SOURCES.txt` & `goit_phone_book_bot-0.1.4/goit_phone_book_bot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,9 +15,11 @@
 src/classes/birthday.py
 src/classes/email.py
 src/classes/field.py
 src/classes/note.py
 src/classes/notes_book.py
 src/classes/phone.py
 src/classes/record.py
+src/constants/__init__.py
+src/constants/commands.py
 src/utils/__init__.py
 src/utils/utils.py
```

### Comparing `goit_phone_book_bot-0.1.3/setup.py` & `goit_phone_book_bot-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='goit-phone-book-bot',
-    version='0.1.3',
+    version='0.1.4',
     author='Vasyl Martyniv',
     author_email='doc.people97@gmail.com',
     description='Phone Book bot developed by team #5 - CREATORS',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VasylMartyniv/GoIT_Phone_Book_bot',
     packages=find_packages(),
```

### Comparing `goit_phone_book_bot-0.1.3/src/classes/address_book.py` & `goit_phone_book_bot-0.1.4/src/classes/address_book.py`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.1.3/src/classes/birthday.py` & `goit_phone_book_bot-0.1.4/src/classes/birthday.py`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.1.3/src/classes/email.py` & `goit_phone_book_bot-0.1.4/src/classes/email.py`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.1.3/src/classes/notes_book.py` & `goit_phone_book_bot-0.1.4/src/classes/notes_book.py`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.1.3/src/classes/phone.py` & `goit_phone_book_bot-0.1.4/src/classes/phone.py`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.1.3/src/classes/record.py` & `goit_phone_book_bot-0.1.4/src/classes/record.py`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.1.3/src/main.py` & `goit_phone_book_bot-0.1.4/src/main.py`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.1.3/src/utils/utils.py` & `goit_phone_book_bot-0.1.4/src/utils/utils.py`

 * *Files identical despite different names*

