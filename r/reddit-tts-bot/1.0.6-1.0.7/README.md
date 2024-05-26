# Comparing `tmp/reddit_tts_bot-1.0.6.tar.gz` & `tmp/reddit_tts_bot-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_tts_bot-1.0.6.tar", last modified: Sat May 25 14:47:53 2024, max compression
+gzip compressed data, was "reddit_tts_bot-1.0.7.tar", last modified: Sun May 26 10:09:42 2024, max compression
```

## Comparing `reddit_tts_bot-1.0.6.tar` & `reddit_tts_bot-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:47:53.287547 reddit_tts_bot-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 14:47:49.000000 reddit_tts_bot-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-25 14:47:53.287547 reddit_tts_bot-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-25 14:47:49.000000 reddit_tts_bot-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:47:53.287547 reddit_tts_bot-1.0.6/reddit_tts_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-25 14:47:49.000000 reddit_tts_bot-1.0.6/reddit_tts_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-25 14:47:49.000000 reddit_tts_bot-1.0.6/reddit_tts_bot/narrative.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-25 14:47:49.000000 reddit_tts_bot-1.0.6/reddit_tts_bot/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-25 14:47:49.000000 reddit_tts_bot-1.0.6/reddit_tts_bot/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:47:53.287547 reddit_tts_bot-1.0.6/reddit_tts_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-25 14:47:53.000000 reddit_tts_bot-1.0.6/reddit_tts_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-25 14:47:53.000000 reddit_tts_bot-1.0.6/reddit_tts_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 14:47:53.000000 reddit_tts_bot-1.0.6/reddit_tts_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-25 14:47:53.000000 reddit_tts_bot-1.0.6/reddit_tts_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 14:47:53.000000 reddit_tts_bot-1.0.6/reddit_tts_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 14:47:53.287547 reddit_tts_bot-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-25 14:47:49.000000 reddit_tts_bot-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:09:42.132384 reddit_tts_bot-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-26 10:09:38.000000 reddit_tts_bot-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-26 10:09:42.132384 reddit_tts_bot-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-26 10:09:38.000000 reddit_tts_bot-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:09:42.132384 reddit_tts_bot-1.0.7/reddit_tts_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-26 10:09:38.000000 reddit_tts_bot-1.0.7/reddit_tts_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-05-26 10:09:38.000000 reddit_tts_bot-1.0.7/reddit_tts_bot/narrative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-26 10:09:38.000000 reddit_tts_bot-1.0.7/reddit_tts_bot/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-26 10:09:38.000000 reddit_tts_bot-1.0.7/reddit_tts_bot/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:09:42.132384 reddit_tts_bot-1.0.7/reddit_tts_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-26 10:09:42.000000 reddit_tts_bot-1.0.7/reddit_tts_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-26 10:09:42.000000 reddit_tts_bot-1.0.7/reddit_tts_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 10:09:42.000000 reddit_tts_bot-1.0.7/reddit_tts_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-26 10:09:42.000000 reddit_tts_bot-1.0.7/reddit_tts_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-26 10:09:42.000000 reddit_tts_bot-1.0.7/reddit_tts_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 10:09:42.132384 reddit_tts_bot-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-26 10:09:38.000000 reddit_tts_bot-1.0.7/setup.py
```

### Comparing `reddit_tts_bot-1.0.6/LICENSE` & `reddit_tts_bot-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.6/PKG-INFO` & `reddit_tts_bot-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit_tts_bot
-Version: 1.0.6
+Version: 1.0.7
 Summary: A module that facilitates the creation of short form content from Reddit posts.
 Home-page: https://github.com/jacksoneshbaugh/reddit-tts-bot
 Author: Jackson Eshbaugh
 Author-email: jacksoneshbaugh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `reddit_tts_bot-1.0.6/README.md` & `reddit_tts_bot-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.6/reddit_tts_bot/narrative.py` & `reddit_tts_bot-1.0.7/reddit_tts_bot/narrative.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Jackson Eshbaugh"
-__version__ = "05/23/2024"
+__version__ = "05/26/2024"
 """
 This file contains code pertaining to narrative generation for the Reddit TTS Bot (including scraping from Reddit).
 """
 
 import os
 import random
 import time
@@ -129,15 +129,15 @@
 
             # Get the articles
             posts: list[WebElement] = driver.find_elements(By.TAG_NAME, 'article')
 
             # Choose a random post
             post: WebElement = random.choice(posts)
 
-            while post.get_attribute('aria-label') in open("narrative_names.txt").read():
+            while post.get_attribute('aria-label').replace(":", "-").replace("/", "-") in open("narrative_names.txt").read():
                 # Scroll the page a bit to load more content
                 driver.execute_script("window.scrollTo(0, document.body.scrollHeight);")
                 time.sleep(SCROLL_PAUSE_TIME)
                 posts = driver.find_elements(By.TAG_NAME, 'article')
                 post = random.choice(posts)
 
             # Get the title (stored in the aria-label attribute of each post)
```

### Comparing `reddit_tts_bot-1.0.6/reddit_tts_bot/tts.py` & `reddit_tts_bot-1.0.7/reddit_tts_bot/tts.py`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.6/reddit_tts_bot/video.py` & `reddit_tts_bot-1.0.7/reddit_tts_bot/video.py`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.6/reddit_tts_bot.egg-info/PKG-INFO` & `reddit_tts_bot-1.0.7/reddit_tts_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit_tts_bot
-Version: 1.0.6
+Version: 1.0.7
 Summary: A module that facilitates the creation of short form content from Reddit posts.
 Home-page: https://github.com/jacksoneshbaugh/reddit-tts-bot
 Author: Jackson Eshbaugh
 Author-email: jacksoneshbaugh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `reddit_tts_bot-1.0.6/reddit_tts_bot.egg-info/requires.txt` & `reddit_tts_bot-1.0.7/reddit_tts_bot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `reddit_tts_bot-1.0.6/setup.py` & `reddit_tts_bot-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __author__ = "Jackson Eshbaugh"
-__version__ = "05/24/2024"
+__version__ = "05/26/2024"
 
 import os
 
 from setuptools import setup, find_packages
 
 setup(
     name='reddit_tts_bot',
-    version='1.0.6',
+    version='1.0.7',
     packages=find_packages(),
     description='A module that facilitates the creation of short form content from Reddit posts.',
     long_description=open(os.path.dirname(__file__) + os.sep + 'README.md').read(),
     long_description_content_type='text/markdown',
     author='Jackson Eshbaugh',
     author_email='jacksoneshbaugh@gmail.com',
     url='https://github.com/jacksoneshbaugh/reddit-tts-bot',
```

