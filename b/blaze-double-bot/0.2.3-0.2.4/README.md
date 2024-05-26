# Comparing `tmp/blaze_double_bot-0.2.3.tar.gz` & `tmp/blaze_double_bot-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaze_double_bot-0.2.3.tar", last modified: Sun May 26 00:41:49 2024, max compression
+gzip compressed data, was "blaze_double_bot-0.2.4.tar", last modified: Sun May 26 01:13:03 2024, max compression
```

## Comparing `blaze_double_bot-0.2.3.tar` & `blaze_double_bot-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 00:41:49.603030 blaze_double_bot-0.2.3/
--rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     3401 2024-05-26 00:41:49.603030 blaze_double_bot-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2907 2024-05-26 00:39:45.000000 blaze_double_bot-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 00:41:49.330401 blaze_double_bot-0.2.3/blaze_double_bot/
--rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.2.3/blaze_double_bot/__init__.py
--rw-rw-rw-   0        0        0    12372 2024-05-26 00:26:56.000000 blaze_double_bot-0.2.3/blaze_double_bot/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-26 00:41:49.603030 blaze_double_bot-0.2.3/blaze_double_bot.egg-info/
--rw-rw-rw-   0        0        0     3401 2024-05-26 00:41:46.000000 blaze_double_bot-0.2.3/blaze_double_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-26 00:41:46.000000 blaze_double_bot-0.2.3/blaze_double_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 00:41:46.000000 blaze_double_bot-0.2.3/blaze_double_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 00:41:46.000000 blaze_double_bot-0.2.3/blaze_double_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-26 00:41:46.000000 blaze_double_bot-0.2.3/blaze_double_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 00:41:49.603030 blaze_double_bot-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-05-26 00:27:39.000000 blaze_double_bot-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:13:03.426732 blaze_double_bot-0.2.4/
+-rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     3401 2024-05-26 01:13:03.414414 blaze_double_bot-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2907 2024-05-26 00:39:45.000000 blaze_double_bot-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 01:13:03.271438 blaze_double_bot-0.2.4/blaze_double_bot/
+-rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.2.4/blaze_double_bot/__init__.py
+-rw-rw-rw-   0        0        0    12470 2024-05-26 01:10:37.000000 blaze_double_bot-0.2.4/blaze_double_bot/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:13:03.414414 blaze_double_bot-0.2.4/blaze_double_bot.egg-info/
+-rw-rw-rw-   0        0        0     3401 2024-05-26 01:13:02.000000 blaze_double_bot-0.2.4/blaze_double_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-26 01:13:03.000000 blaze_double_bot-0.2.4/blaze_double_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 01:13:02.000000 blaze_double_bot-0.2.4/blaze_double_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 01:13:02.000000 blaze_double_bot-0.2.4/blaze_double_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-26 01:13:03.000000 blaze_double_bot-0.2.4/blaze_double_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 01:13:03.428574 blaze_double_bot-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-26 01:11:30.000000 blaze_double_bot-0.2.4/setup.py
```

### Comparing `blaze_double_bot-0.2.3/LICENSE` & `blaze_double_bot-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.2.3/PKG-INFO` & `blaze_double_bot-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.2.3
+Version: 0.2.4
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blaze_double_bot-0.2.3/README.md` & `blaze_double_bot-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.2.3/blaze_double_bot/bot.py` & `blaze_double_bot-0.2.4/blaze_double_bot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,23 +54,24 @@
             'Bet on Red': {'en': 'Bet on Red', 'pt': 'Apostar no Vermelho'},
             'Bet on Black': {'en': 'Bet on Black', 'pt': 'Apostar no Preto'},
             'Completed': {'en': 'Completed', 'pt': 'Concluído'},
             'Waiting for result ...': {'en': 'Waiting for result ...', 'pt': 'Esperando o resultado ...'},
             'Win ->': {'en': 'Win ->', 'pt': 'Ganhou ->'},
             'Loss ->': {'en': 'Loss ->', 'pt': 'Perdeu ->'},
             'Balance: $': {'en': 'Balance: $', 'pt': 'Saldo: $'},
-            'Waiting seconds to restart analysis ...': {'en': 'Waiting seconds to restart analysis ...', 'pt': 'Esperando segundos para reiniciar a análise ...'},
+            'Waiting seconds to restart analysis ...': {'en': f'Waiting {self.wait_after_bet} seconds to restart analysis ...', 'pt': f'Esperando {self.wait_after_bet} segundos para reiniciar a análise ...'},
             'Analyzes restarted! ->': {'en': 'Analyzes restarted! ->', 'pt': 'Análises reiniciadas! ->'},
             'Initial Balance: $': {'en': 'Initial Balance: $', 'pt': 'Saldo Inicial: $'},
             'Stop Loss: $': {'en': 'Stop Loss: $', 'pt': 'Stop Loss: $'},
             'Stop Win: $': {'en': 'Stop Win: $', 'pt': 'Stop Win: $'},
             'Bet Amount: $': {'en': 'Bet Amount: $', 'pt': 'Quantia de Aposta: $'},
             'Final Balance: $': {'en': 'Final Balance: $', 'pt': 'Saldo Final: $'},
             'Blaze Double Bet Bot Started': {'en': 'Blaze Double Bet Bot Started', 'pt': 'Robô de Aposta Blaze Double Iniciado'},
             'Blaze Double Bet Bot Finished': {'en': 'Blaze Double Bet Bot Finished', 'pt': 'Robô de Aposta Blaze Double Finalizado'},
+            'Betting strategy -> ':{'en':'Betting strategy -> ','pt':'Estratégia de aposta -> '}
         }
         return texts.get(text, {}).get(self.language, text)
 
     def login(self):
         sleep(5)
         self.driver.find_element(By.XPATH, "//a[@class='link']").click()
         print(self.get_text('Clicking to login'))
@@ -247,15 +248,15 @@
                                     
                             self.print_bet_result(history, color)
                             sleep(8)
                             self.current_balance = self.get_balance()
                             print(self.get_text('Balance: $'),self.current_balance)
                             print(datetime.now().strftime("%m/%d/%Y %H:%M"))
                             if self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
-                                print(f'{self.get_text("Waiting seconds to restart analysis ...").replace("seconds", str(self.wait_after_bet))}\n')
+                                print(f'{self.get_text("Waiting seconds to restart analysis ...")\n')
                                 sleep(self.wait_after_bet)
                                 print(50*'*')
                                 print(self.get_text('Analyzes restarted! ->'),datetime.now().strftime("%m/%d/%Y %H:%M"))
                     
                             
                 else:
                     self.print_final_text()
```

### Comparing `blaze_double_bot-0.2.3/blaze_double_bot.egg-info/PKG-INFO` & `blaze_double_bot-0.2.4/blaze_double_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.2.3
+Version: 0.2.4
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blaze_double_bot-0.2.3/setup.py` & `blaze_double_bot-0.2.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r') as f:
           readme =f.read()
 
 setup(
     name='blaze_double_bot',
     licence='MIT License',
-    version='0.2.3',
+    version='0.2.4',
     author='ror74559',
     long_description=readme,
     long_description_content_type='text/markdown',
     author_email='ror74559@gmail.com',
     keywords='blaze double bot',
     description='This Python library automates the betting process on the Blaze Double',
     packages=['blaze_double_bot'],
```

