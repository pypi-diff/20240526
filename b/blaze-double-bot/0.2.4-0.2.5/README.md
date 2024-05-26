# Comparing `tmp/blaze_double_bot-0.2.4.tar.gz` & `tmp/blaze_double_bot-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaze_double_bot-0.2.4.tar", last modified: Sun May 26 01:13:03 2024, max compression
+gzip compressed data, was "blaze_double_bot-0.2.5.tar", last modified: Sun May 26 01:22:32 2024, max compression
```

## Comparing `blaze_double_bot-0.2.4.tar` & `blaze_double_bot-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 01:13:03.426732 blaze_double_bot-0.2.4/
--rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     3401 2024-05-26 01:13:03.414414 blaze_double_bot-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2907 2024-05-26 00:39:45.000000 blaze_double_bot-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 01:13:03.271438 blaze_double_bot-0.2.4/blaze_double_bot/
--rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.2.4/blaze_double_bot/__init__.py
--rw-rw-rw-   0        0        0    12470 2024-05-26 01:10:37.000000 blaze_double_bot-0.2.4/blaze_double_bot/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-26 01:13:03.414414 blaze_double_bot-0.2.4/blaze_double_bot.egg-info/
--rw-rw-rw-   0        0        0     3401 2024-05-26 01:13:02.000000 blaze_double_bot-0.2.4/blaze_double_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-26 01:13:03.000000 blaze_double_bot-0.2.4/blaze_double_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 01:13:02.000000 blaze_double_bot-0.2.4/blaze_double_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 01:13:02.000000 blaze_double_bot-0.2.4/blaze_double_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-26 01:13:03.000000 blaze_double_bot-0.2.4/blaze_double_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 01:13:03.428574 blaze_double_bot-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-05-26 01:11:30.000000 blaze_double_bot-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:22:32.581004 blaze_double_bot-0.2.5/
+-rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     3401 2024-05-26 01:22:32.575937 blaze_double_bot-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2907 2024-05-26 00:39:45.000000 blaze_double_bot-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 01:22:32.507765 blaze_double_bot-0.2.5/blaze_double_bot/
+-rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.2.5/blaze_double_bot/__init__.py
+-rw-rw-rw-   0        0        0    12471 2024-05-26 01:21:34.000000 blaze_double_bot-0.2.5/blaze_double_bot/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:22:32.572317 blaze_double_bot-0.2.5/blaze_double_bot.egg-info/
+-rw-rw-rw-   0        0        0     3401 2024-05-26 01:22:32.000000 blaze_double_bot-0.2.5/blaze_double_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-26 01:22:32.000000 blaze_double_bot-0.2.5/blaze_double_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 01:22:32.000000 blaze_double_bot-0.2.5/blaze_double_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 01:22:32.000000 blaze_double_bot-0.2.5/blaze_double_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-26 01:22:32.000000 blaze_double_bot-0.2.5/blaze_double_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 01:22:32.581519 blaze_double_bot-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-26 01:20:52.000000 blaze_double_bot-0.2.5/setup.py
```

### Comparing `blaze_double_bot-0.2.4/LICENSE` & `blaze_double_bot-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.2.4/PKG-INFO` & `blaze_double_bot-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.2.4
+Version: 0.2.5
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blaze_double_bot-0.2.4/README.md` & `blaze_double_bot-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.2.4/blaze_double_bot/bot.py` & `blaze_double_bot-0.2.5/blaze_double_bot/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
                                     
                             self.print_bet_result(history, color)
                             sleep(8)
                             self.current_balance = self.get_balance()
                             print(self.get_text('Balance: $'),self.current_balance)
                             print(datetime.now().strftime("%m/%d/%Y %H:%M"))
                             if self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
-                                print(f'{self.get_text("Waiting seconds to restart analysis ...")\n')
+                                print(f'{self.get_text("Waiting seconds to restart analysis ...")\n}')
                                 sleep(self.wait_after_bet)
                                 print(50*'*')
                                 print(self.get_text('Analyzes restarted! ->'),datetime.now().strftime("%m/%d/%Y %H:%M"))
                     
                             
                 else:
                     self.print_final_text()
```

### Comparing `blaze_double_bot-0.2.4/blaze_double_bot.egg-info/PKG-INFO` & `blaze_double_bot-0.2.5/blaze_double_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.2.4
+Version: 0.2.5
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blaze_double_bot-0.2.4/setup.py` & `blaze_double_bot-0.2.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r') as f:
           readme =f.read()
 
 setup(
     name='blaze_double_bot',
     licence='MIT License',
-    version='0.2.4',
+    version='0.2.5',
     author='ror74559',
     long_description=readme,
     long_description_content_type='text/markdown',
     author_email='ror74559@gmail.com',
     keywords='blaze double bot',
     description='This Python library automates the betting process on the Blaze Double',
     packages=['blaze_double_bot'],
```

