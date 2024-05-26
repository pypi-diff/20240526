# Comparing `tmp/blaze_double_bot-0.2.2.tar.gz` & `tmp/blaze_double_bot-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaze_double_bot-0.2.2.tar", last modified: Fri May 24 23:55:16 2024, max compression
+gzip compressed data, was "blaze_double_bot-0.2.3.tar", last modified: Sun May 26 00:41:49 2024, max compression
```

## Comparing `blaze_double_bot-0.2.2.tar` & `blaze_double_bot-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 23:55:16.146523 blaze_double_bot-0.2.2/
--rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     3183 2024-05-24 23:55:16.146523 blaze_double_bot-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2692 2024-05-24 23:53:24.000000 blaze_double_bot-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 23:55:16.099330 blaze_double_bot-0.2.2/blaze_double_bot/
--rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.2.2/blaze_double_bot/__init__.py
--rw-rw-rw-   0        0        0     9929 2024-05-24 23:41:07.000000 blaze_double_bot-0.2.2/blaze_double_bot/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-24 23:55:16.139585 blaze_double_bot-0.2.2/blaze_double_bot.egg-info/
--rw-rw-rw-   0        0        0     3183 2024-05-24 23:55:15.000000 blaze_double_bot-0.2.2/blaze_double_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-24 23:55:15.000000 blaze_double_bot-0.2.2/blaze_double_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 23:55:15.000000 blaze_double_bot-0.2.2/blaze_double_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 23:55:15.000000 blaze_double_bot-0.2.2/blaze_double_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-24 23:55:15.000000 blaze_double_bot-0.2.2/blaze_double_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 23:55:16.146523 blaze_double_bot-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-05-24 23:54:42.000000 blaze_double_bot-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 00:41:49.603030 blaze_double_bot-0.2.3/
+-rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     3401 2024-05-26 00:41:49.603030 blaze_double_bot-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2907 2024-05-26 00:39:45.000000 blaze_double_bot-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 00:41:49.330401 blaze_double_bot-0.2.3/blaze_double_bot/
+-rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.2.3/blaze_double_bot/__init__.py
+-rw-rw-rw-   0        0        0    12372 2024-05-26 00:26:56.000000 blaze_double_bot-0.2.3/blaze_double_bot/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-26 00:41:49.603030 blaze_double_bot-0.2.3/blaze_double_bot.egg-info/
+-rw-rw-rw-   0        0        0     3401 2024-05-26 00:41:46.000000 blaze_double_bot-0.2.3/blaze_double_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-26 00:41:46.000000 blaze_double_bot-0.2.3/blaze_double_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 00:41:46.000000 blaze_double_bot-0.2.3/blaze_double_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 00:41:46.000000 blaze_double_bot-0.2.3/blaze_double_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-26 00:41:46.000000 blaze_double_bot-0.2.3/blaze_double_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 00:41:49.603030 blaze_double_bot-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-26 00:27:39.000000 blaze_double_bot-0.2.3/setup.py
```

### Comparing `blaze_double_bot-0.2.2/LICENSE` & `blaze_double_bot-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.2.2/PKG-INFO` & `blaze_double_bot-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.2.2
+Version: 0.2.3
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -40,14 +40,16 @@
 {
     "username": "your blaze username",
     "password": "your blaze password",
     "bet_amount":0.1,
     "stop_loss_ratio":0.9,
     "stop_win_ratio":1.1,
     "wait_after_bet":150,
+    "martingale":2,
+    "language":"en",
     "strategies": {
         "red": [
             ["B", "R", "B", "R", "B"],
             ["B", "B", "B", "B", "B"]
         ],
         "black": [
             ["R", "B", "R", "B", "R"],
@@ -60,14 +62,16 @@
 
 - **username**: Your username or email registered on Blaze Double.
 - **password**: Your password to access Blaze Double.
 - **bet_amount**: The amount of the bet to be placed in each round.
 - **stop_loss_ratio**: The multiplication factor of the initial balance indicating the loss limit. The bot will stop betting if the balance drops below this limit.
 - **stop_win_ratio**: The multiplication factor of the initial balance indicating the win limit. The bot will stop betting if the balance reaches or exceeds this limit.
 - **wait_after_bet**: Waiting time, in seconds, to restart analyzes after the bet result.
+- **martingale**: MartinGale's strategy doubles the bet after a loss. The bot will do this procedure if the value is different from 0. If the value is 1 it will do the procedure 1 time, if 2 it will do it 2 times and so on. Be very careful with this strategy.
+- **language**: "en" (English) and "pt" (Portuguese).
 - **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.Lists must be the same length and have a maximum of 20 items.
 
 2. **Create a `blazeBot.py` file** with the following content:
 
 ```python
 
 from blaze_double_bot import BlazeDoubleBot
@@ -78,15 +82,14 @@
         config = json.load(f)
 
 bot = BlazeDoubleBot(config)
 
 bot.run()
 
 ```
-# The bot follows MartinGale's strategy of doubling the bet after a loss. The bot will repeat this procedure 2 times, or 1 time if it wins.
 ---
 
 ## Support This Project
 
 If you find this project helpful, consider supporting it by making a donation. Your contribution will help me maintain and improve this bot.
 
 [Donate via PayPal](https://www.paypal.com/donate/?hosted_button_id=928TRAX74TYSA)
```

### Comparing `blaze_double_bot-0.2.2/README.md` & `blaze_double_bot-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 {
     "username": "your blaze username",
     "password": "your blaze password",
     "bet_amount":0.1,
     "stop_loss_ratio":0.9,
     "stop_win_ratio":1.1,
     "wait_after_bet":150,
+    "martingale":2,
+    "language":"en",
     "strategies": {
         "red": [
             ["B", "R", "B", "R", "B"],
             ["B", "B", "B", "B", "B"]
         ],
         "black": [
             ["R", "B", "R", "B", "R"],
@@ -46,14 +48,16 @@
 
 - **username**: Your username or email registered on Blaze Double.
 - **password**: Your password to access Blaze Double.
 - **bet_amount**: The amount of the bet to be placed in each round.
 - **stop_loss_ratio**: The multiplication factor of the initial balance indicating the loss limit. The bot will stop betting if the balance drops below this limit.
 - **stop_win_ratio**: The multiplication factor of the initial balance indicating the win limit. The bot will stop betting if the balance reaches or exceeds this limit.
 - **wait_after_bet**: Waiting time, in seconds, to restart analyzes after the bet result.
+- **martingale**: MartinGale's strategy doubles the bet after a loss. The bot will do this procedure if the value is different from 0. If the value is 1 it will do the procedure 1 time, if 2 it will do it 2 times and so on. Be very careful with this strategy.
+- **language**: "en" (English) and "pt" (Portuguese).
 - **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.Lists must be the same length and have a maximum of 20 items.
 
 2. **Create a `blazeBot.py` file** with the following content:
 
 ```python
 
 from blaze_double_bot import BlazeDoubleBot
@@ -64,15 +68,14 @@
         config = json.load(f)
 
 bot = BlazeDoubleBot(config)
 
 bot.run()
 
 ```
-# The bot follows MartinGale's strategy of doubling the bet after a loss. The bot will repeat this procedure 2 times, or 1 time if it wins.
 ---
 
 ## Support This Project
 
 If you find this project helpful, consider supporting it by making a donation. Your contribution will help me maintain and improve this bot.
 
 [Donate via PayPal](https://www.paypal.com/donate/?hosted_button_id=928TRAX74TYSA)
```

### Comparing `blaze_double_bot-0.2.2/blaze_double_bot.egg-info/PKG-INFO` & `blaze_double_bot-0.2.3/blaze_double_bot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.2.2
+Version: 0.2.3
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -40,14 +40,16 @@
 {
     "username": "your blaze username",
     "password": "your blaze password",
     "bet_amount":0.1,
     "stop_loss_ratio":0.9,
     "stop_win_ratio":1.1,
     "wait_after_bet":150,
+    "martingale":2,
+    "language":"en",
     "strategies": {
         "red": [
             ["B", "R", "B", "R", "B"],
             ["B", "B", "B", "B", "B"]
         ],
         "black": [
             ["R", "B", "R", "B", "R"],
@@ -60,14 +62,16 @@
 
 - **username**: Your username or email registered on Blaze Double.
 - **password**: Your password to access Blaze Double.
 - **bet_amount**: The amount of the bet to be placed in each round.
 - **stop_loss_ratio**: The multiplication factor of the initial balance indicating the loss limit. The bot will stop betting if the balance drops below this limit.
 - **stop_win_ratio**: The multiplication factor of the initial balance indicating the win limit. The bot will stop betting if the balance reaches or exceeds this limit.
 - **wait_after_bet**: Waiting time, in seconds, to restart analyzes after the bet result.
+- **martingale**: MartinGale's strategy doubles the bet after a loss. The bot will do this procedure if the value is different from 0. If the value is 1 it will do the procedure 1 time, if 2 it will do it 2 times and so on. Be very careful with this strategy.
+- **language**: "en" (English) and "pt" (Portuguese).
 - **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.Lists must be the same length and have a maximum of 20 items.
 
 2. **Create a `blazeBot.py` file** with the following content:
 
 ```python
 
 from blaze_double_bot import BlazeDoubleBot
@@ -78,15 +82,14 @@
         config = json.load(f)
 
 bot = BlazeDoubleBot(config)
 
 bot.run()
 
 ```
-# The bot follows MartinGale's strategy of doubling the bet after a loss. The bot will repeat this procedure 2 times, or 1 time if it wins.
 ---
 
 ## Support This Project
 
 If you find this project helpful, consider supporting it by making a donation. Your contribution will help me maintain and improve this bot.
 
 [Donate via PayPal](https://www.paypal.com/donate/?hosted_button_id=928TRAX74TYSA)
```

