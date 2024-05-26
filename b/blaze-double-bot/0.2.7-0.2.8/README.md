# Comparing `tmp/blaze_double_bot-0.2.7.tar.gz` & `tmp/blaze_double_bot-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaze_double_bot-0.2.7.tar", last modified: Sun May 26 12:54:57 2024, max compression
+gzip compressed data, was "blaze_double_bot-0.2.8.tar", last modified: Sun May 26 16:24:07 2024, max compression
```

## Comparing `blaze_double_bot-0.2.7.tar` & `blaze_double_bot-0.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 12:54:57.938259 blaze_double_bot-0.2.7/
--rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     3401 2024-05-26 12:54:57.934852 blaze_double_bot-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     2907 2024-05-26 00:39:45.000000 blaze_double_bot-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 12:54:57.836648 blaze_double_bot-0.2.7/blaze_double_bot/
--rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.2.7/blaze_double_bot/__init__.py
--rw-rw-rw-   0        0        0    12486 2024-05-26 12:49:53.000000 blaze_double_bot-0.2.7/blaze_double_bot/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-26 12:54:57.924471 blaze_double_bot-0.2.7/blaze_double_bot.egg-info/
--rw-rw-rw-   0        0        0     3401 2024-05-26 12:54:57.000000 blaze_double_bot-0.2.7/blaze_double_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-26 12:54:57.000000 blaze_double_bot-0.2.7/blaze_double_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 12:54:57.000000 blaze_double_bot-0.2.7/blaze_double_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 12:54:57.000000 blaze_double_bot-0.2.7/blaze_double_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-26 12:54:57.000000 blaze_double_bot-0.2.7/blaze_double_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 12:54:57.938259 blaze_double_bot-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-05-26 12:53:27.000000 blaze_double_bot-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:24:07.914755 blaze_double_bot-0.2.8/
+-rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0     3500 2024-05-26 16:24:07.914755 blaze_double_bot-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3004 2024-05-26 16:19:44.000000 blaze_double_bot-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 16:24:07.843583 blaze_double_bot-0.2.8/blaze_double_bot/
+-rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.2.8/blaze_double_bot/__init__.py
+-rw-rw-rw-   0        0        0    12655 2024-05-26 16:20:20.000000 blaze_double_bot-0.2.8/blaze_double_bot/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:24:07.914755 blaze_double_bot-0.2.8/blaze_double_bot.egg-info/
+-rw-rw-rw-   0        0        0     3500 2024-05-26 16:24:07.000000 blaze_double_bot-0.2.8/blaze_double_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-26 16:24:07.000000 blaze_double_bot-0.2.8/blaze_double_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 16:24:07.000000 blaze_double_bot-0.2.8/blaze_double_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 16:24:07.000000 blaze_double_bot-0.2.8/blaze_double_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-26 16:24:07.000000 blaze_double_bot-0.2.8/blaze_double_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 16:24:07.914755 blaze_double_bot-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-26 16:20:32.000000 blaze_double_bot-0.2.8/setup.py
```

### Comparing `blaze_double_bot-0.2.7/LICENSE` & `blaze_double_bot-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.2.7/PKG-INFO` & `blaze_double_bot-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.2.7
+Version: 0.2.8
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,14 +41,15 @@
     "username": "your blaze username",
     "password": "your blaze password",
     "bet_amount":0.1,
     "stop_loss_ratio":0.9,
     "stop_win_ratio":1.1,
     "wait_after_bet":150,
     "martingale":2,
+    "headless": True,
     "language":"en",
     "strategies": {
         "red": [
             ["B", "R", "B", "R", "B"],
             ["B", "B", "B", "B", "B"]
         ],
         "black": [
@@ -63,14 +64,15 @@
 - **username**: Your username or email registered on Blaze Double.
 - **password**: Your password to access Blaze Double.
 - **bet_amount**: The amount of the bet to be placed in each round.
 - **stop_loss_ratio**: The multiplication factor of the initial balance indicating the loss limit. The bot will stop betting if the balance drops below this limit.
 - **stop_win_ratio**: The multiplication factor of the initial balance indicating the win limit. The bot will stop betting if the balance reaches or exceeds this limit.
 - **wait_after_bet**: Waiting time, in seconds, to restart analyzes after the bet result.
 - **martingale**: MartinGale's strategy doubles the bet after a loss. The bot will do this procedure if the value is different from 0. If the value is 1 it will do the procedure 1 time, if 2 it will do it 2 times and so on. Be very careful with this strategy.
+- **headless**: receives True or False. True the browser will be invisible
 - **language**: "en" (English) and "pt" (Portuguese).
 - **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.Lists must be the same length and have a maximum of 20 items.
 
 2. **Create a `blazeBot.py` file** with the following content:
 
 ```python
```

### Comparing `blaze_double_bot-0.2.7/README.md` & `blaze_double_bot-0.2.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "username": "your blaze username",
     "password": "your blaze password",
     "bet_amount":0.1,
     "stop_loss_ratio":0.9,
     "stop_win_ratio":1.1,
     "wait_after_bet":150,
     "martingale":2,
+    "headless": True,
     "language":"en",
     "strategies": {
         "red": [
             ["B", "R", "B", "R", "B"],
             ["B", "B", "B", "B", "B"]
         ],
         "black": [
@@ -49,14 +50,15 @@
 - **username**: Your username or email registered on Blaze Double.
 - **password**: Your password to access Blaze Double.
 - **bet_amount**: The amount of the bet to be placed in each round.
 - **stop_loss_ratio**: The multiplication factor of the initial balance indicating the loss limit. The bot will stop betting if the balance drops below this limit.
 - **stop_win_ratio**: The multiplication factor of the initial balance indicating the win limit. The bot will stop betting if the balance reaches or exceeds this limit.
 - **wait_after_bet**: Waiting time, in seconds, to restart analyzes after the bet result.
 - **martingale**: MartinGale's strategy doubles the bet after a loss. The bot will do this procedure if the value is different from 0. If the value is 1 it will do the procedure 1 time, if 2 it will do it 2 times and so on. Be very careful with this strategy.
+- **headless**: receives True or False. True the browser will be invisible
 - **language**: "en" (English) and "pt" (Portuguese).
 - **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.Lists must be the same length and have a maximum of 20 items.
 
 2. **Create a `blazeBot.py` file** with the following content:
 
 ```python
```

### Comparing `blaze_double_bot-0.2.7/blaze_double_bot/bot.py` & `blaze_double_bot-0.2.8/blaze_double_bot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,27 @@
         self.password = config['password']
         self.bet_amount = config['bet_amount']
         self.stop_loss_ratio = config['stop_loss_ratio']
         self.stop_win_ratio = config['stop_win_ratio']
         self.wait_after_bet = config['wait_after_bet']
         self.martingale = config['martingale']
         self.strategies = config['strategies']
-        self.language = config.get('language', 'en')  
+        self.language = config.get('language', 'en')
+        self.headless = config['headless']
 
         self.color_dict = {'black': 'B', 'red': 'R', 'white': 'W'}
         print(self.get_text('Initializing the robot ...'))
         chrome_options = Options()
-        chrome_options.add_argument("--headless=new")
-        self.driver = uc.Chrome(options=chrome_options)
+        
+        if self.headless:
+            chrome_options.add_argument("--headless=new")
+        else:
+            chrome_options.add_argument("--headless=old")
+            
+        self.driver = uc.Chrome(options=chrome_options)    
         print(self.get_text('Accessing website ...'))
         self.driver.get('https://blaze1.space/nt/games/double')
         sleep(10)
         print(self.get_text('Logging in ...'))
         self.login()
         sleep(10)
         print(self.get_text('Logged ...'))
```

### Comparing `blaze_double_bot-0.2.7/blaze_double_bot.egg-info/PKG-INFO` & `blaze_double_bot-0.2.8/blaze_double_bot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.2.7
+Version: 0.2.8
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,14 +41,15 @@
     "username": "your blaze username",
     "password": "your blaze password",
     "bet_amount":0.1,
     "stop_loss_ratio":0.9,
     "stop_win_ratio":1.1,
     "wait_after_bet":150,
     "martingale":2,
+    "headless": True,
     "language":"en",
     "strategies": {
         "red": [
             ["B", "R", "B", "R", "B"],
             ["B", "B", "B", "B", "B"]
         ],
         "black": [
@@ -63,14 +64,15 @@
 - **username**: Your username or email registered on Blaze Double.
 - **password**: Your password to access Blaze Double.
 - **bet_amount**: The amount of the bet to be placed in each round.
 - **stop_loss_ratio**: The multiplication factor of the initial balance indicating the loss limit. The bot will stop betting if the balance drops below this limit.
 - **stop_win_ratio**: The multiplication factor of the initial balance indicating the win limit. The bot will stop betting if the balance reaches or exceeds this limit.
 - **wait_after_bet**: Waiting time, in seconds, to restart analyzes after the bet result.
 - **martingale**: MartinGale's strategy doubles the bet after a loss. The bot will do this procedure if the value is different from 0. If the value is 1 it will do the procedure 1 time, if 2 it will do it 2 times and so on. Be very careful with this strategy.
+- **headless**: receives True or False. True the browser will be invisible
 - **language**: "en" (English) and "pt" (Portuguese).
 - **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.Lists must be the same length and have a maximum of 20 items.
 
 2. **Create a `blazeBot.py` file** with the following content:
 
 ```python
```

### Comparing `blaze_double_bot-0.2.7/setup.py` & `blaze_double_bot-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r') as f:
           readme =f.read()
 
 setup(
     name='blaze_double_bot',
     licence='MIT License',
-    version='0.2.7',
+    version='0.2.8',
     author='ror74559',
     long_description=readme,
     long_description_content_type='text/markdown',
     author_email='ror74559@gmail.com',
     keywords='blaze double bot',
     description='This Python library automates the betting process on the Blaze Double',
     packages=['blaze_double_bot'],
```

