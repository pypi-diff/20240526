# Comparing `tmp/desktop_shop-1.0.5.tar.gz` & `tmp/desktop_shop-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop_shop-1.0.5.tar", last modified: Sun Jan 22 19:54:15 2023, max compression
+gzip compressed data, was "desktop_shop-1.1.0.tar", last modified: Sun May 26 15:30:13 2024, max compression
```

## Comparing `desktop_shop-1.0.5.tar` & `desktop_shop-1.1.0.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 19:54:15.065555 desktop_shop-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-01-22 19:54:15.065555 desktop_shop-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 19:54:15.065555 desktop_shop-1.0.5/desktop_shop/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 19:54:15.065555 desktop_shop-1.0.5/desktop_shop/datagen/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/datagen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/datagen/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/datagen/generate_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 19:54:15.065555 desktop_shop-1.0.5/desktop_shop/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/gui/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/gui/components.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/gui/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/gui/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 19:54:15.065555 desktop_shop-1.0.5/desktop_shop/gui/views/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/gui/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/gui/views/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/gui/views/home.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/gui/views/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/gui/views/main_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/gui/views/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/gui/views/register.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/desktop_shop/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 19:54:15.065555 desktop_shop-1.0.5/desktop_shop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-01-22 19:54:15.000000 desktop_shop-1.0.5/desktop_shop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-22 19:54:15.000000 desktop_shop-1.0.5/desktop_shop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 19:54:15.000000 desktop_shop-1.0.5/desktop_shop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 19:54:14.000000 desktop_shop-1.0.5/desktop_shop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-22 19:54:15.000000 desktop_shop-1.0.5/desktop_shop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-22 19:54:15.000000 desktop_shop-1.0.5/desktop_shop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-22 19:54:15.065555 desktop_shop-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-01-22 19:54:05.000000 desktop_shop-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:30:13.198609 desktop_shop-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-26 15:30:13.198609 desktop_shop-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:30:13.198609 desktop_shop-1.1.0/desktop_shop/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:30:13.194609 desktop_shop-1.1.0/desktop_shop/datagen/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/datagen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/datagen/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/datagen/generate_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:30:13.198609 desktop_shop-1.1.0/desktop_shop/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/gui/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/gui/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/gui/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/gui/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:30:13.198609 desktop_shop-1.1.0/desktop_shop/gui/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/gui/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/gui/views/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/gui/views/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/gui/views/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/gui/views/main_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/gui/views/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/gui/views/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/desktop_shop/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:30:13.198609 desktop_shop-1.1.0/desktop_shop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-26 15:30:13.000000 desktop_shop-1.1.0/desktop_shop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-26 15:30:13.000000 desktop_shop-1.1.0/desktop_shop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 15:30:13.000000 desktop_shop-1.1.0/desktop_shop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 15:30:13.000000 desktop_shop-1.1.0/desktop_shop.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-26 15:30:13.000000 desktop_shop-1.1.0/desktop_shop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 15:30:13.000000 desktop_shop-1.1.0/desktop_shop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 15:30:13.198609 desktop_shop-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-26 15:30:02.000000 desktop_shop-1.1.0/setup.py
```

### Comparing `desktop_shop-1.0.5/LICENSE` & `desktop_shop-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop_shop-1.0.5/PKG-INFO` & `desktop_shop-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: desktop_shop
-Version: 1.0.5
-Summary: Desktop shop application
-Home-page: https://github.com/rbaltrusch/desktop_shop
-Author: Richard Baltrusch
-License: MIT
-Keywords: python
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Unit tests](https://github.com/rbaltrusch/desktop_shop/actions/workflows/pytest-unit-tests.yml/badge.svg)](https://github.com/rbaltrusch/desktop_shop/actions/workflows/pytest-unit-tests.yml)
 [![Pylint](https://github.com/rbaltrusch/desktop_shop/actions/workflows/pylint.yml/badge.svg)](https://github.com/rbaltrusch/desktop_shop/actions/workflows/pylint.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](https://opensource.org/licenses/MIT)
 
 # Desktop Shop
 
 This is a mock shop application, running completely offline on a desktop. The graphical interface connects with a generated, local database of customers, products and transactions (Python / SQLite3). As the application runs completely offline, it does away with any networking or server complexity and showcases a bare implementation of an application interfacing with a production database.
@@ -40,14 +18,24 @@
 Run the shop application by installing the package using pip, then calling it:
 
     python -m pip install desktop_shop
     python -m desktop_shop
 
 Note that the first time the package is called, it automatically generates a fresh database filled with random data. This make take a few seconds.
 
+## ⚠️ State of the repository ⚠️
+
+This repository is unlikely to receive new features in the future, although maintenance and small fixes will still be done.
+
+This means that some features that are missing now will stay missing (but feel free to submit a pull request to add them!), and non-optimal aspects of the codebase or the application are unlikely to get fixed. Some of these include:
+- No admin panel
+- A user cannot see the transactions that he has placed in the past
+- The application asking for gender is a violation of the EU GDPR, as this user data is not required with the application as is (the same potentially applies to collecting date of birth).
+- The interface to the database is not ideal, as typing is missing for the most part, it is somewhat internally inconsistent, and is using lists or tuples instead of objects.
+
 ## Contributions
 
 To contribute to this repository, please read the [contribution guidelines](https://github.com/rbaltrusch/desktop_shop/blob/master/CONTRIBUTING.md).
 
 ## Python
 
 Written in Python 3.8.3.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `desktop_shop-1.0.5/desktop_shop/__main__.py` & `desktop_shop-1.1.0/desktop_shop/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,21 +7,25 @@
 import os
 
 from desktop_shop import DATABASE_NAME
 from desktop_shop.datagen import generate_data
 
 # fast db generation if not present
 if not os.path.exists(DATABASE_NAME):
+    print("Generating database...")
     generate_data.generate(
         DATABASE_NAME, hash_iterations=1, transactions=100_000, users=10_000, products=20
     )
+    print("Done generating.")
 
 # pylint: disable=wrong-import-position
 from desktop_shop.gui import app, db_conn, init
 
+print("Starting GUI...")
 try:
     init.init()
     app.views_dict["main_menu"].pack()
     app.views_dict["home"].pack()
     app.mainloop()
 finally:
     db_conn.close()
+print("Shutdown.")
```

### Comparing `desktop_shop-1.0.5/desktop_shop/crypto.py` & `desktop_shop-1.1.0/desktop_shop/crypto.py`

 * *Files identical despite different names*

### Comparing `desktop_shop-1.0.5/desktop_shop/datagen/data.py` & `desktop_shop-1.1.0/desktop_shop/datagen/data.py`

 * *Files identical despite different names*

### Comparing `desktop_shop-1.0.5/desktop_shop/datagen/generate_data.py` & `desktop_shop-1.1.0/desktop_shop/datagen/generate_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 @author: Korean_Crimson
 """
 import logging
 import random
 import sqlite3
 from typing import List, Protocol, Set
 
-from desktop_shop import crypto, database, util
+from desktop_shop import crypto, util
+from desktop_shop.database import database
 from desktop_shop.datagen import data
 
 # combined with every salt for extra security in pw hashing
 PEPPER = "secret"
 
 
 class TableDataGenerator(Protocol):  # pylint: disable=missing-class-docstring
@@ -56,16 +57,16 @@
             password = self._generate_new_password()
             database.add_user(cursor, user_data, password, PEPPER, iterations=self.hash_iterations)
 
     def _generate_random_user_data(self, first_names, last_names):
         first_name = random.choice(list(first_names.keys()))
         last_name = random.choice(last_names)
         gender = first_names[first_name]
-        join_date = data.get_random_date(start=[2014, 6, 1], end=[2020, 11, 1])
-        dob = data.get_random_date(start=[1920, 1, 1], end=[2004, 6, 1])
+        join_date = data.get_random_date(start=(2014, 6, 1), end=(2020, 11, 1))
+        dob = data.get_random_date(start=(1920, 1, 1), end=(2004, 6, 1))
         email_address = self._generate_random_email_address(first_name, last_name, dob)
         return [first_name, last_name, gender, dob, email_address, join_date]
 
     def _generate_random_email_address(self, first_name, last_name, dob):
         """generates unique email using _email_cache storing all generated emails"""
         email_address = ""
         domains = [
@@ -148,15 +149,15 @@
         transactions = [cls._generate_random_transaction_data(user_ids) for _ in range(amount)]
         product_ids = [cls._generate_random_chosen_product_ids(product_ids) for _ in range(amount)]
         database.add_transactions(cursor, transactions, product_ids)
 
     @staticmethod
     def _generate_random_transaction_data(user_ids):
         user_id = random.choice(user_ids)
-        date = data.get_random_date(start=[2004, 6, 1], end=[2020, 11, 1])
+        date = data.get_random_date(start=(2004, 6, 1), end=(2020, 11, 1))
 
         transaction_data = [user_id, date]
         return transaction_data
 
     @staticmethod
     def _generate_random_chosen_product_ids(product_ids):
         number_of_products = random.randint(1, 5)
```

### Comparing `desktop_shop-1.0.5/desktop_shop/gui/callbacks.py` & `desktop_shop-1.1.0/desktop_shop/gui/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 # -*- coding: utf-8 -*-
 """
 Created on Mon Feb  1 09:53:07 2021
 
 @author: Korean_Crimson
 """
+
+# mypy: ignore-errors
+
+from typing import Collection, Optional
 import re
 
 from desktop_shop import gui, server, user, util
 
 # pylint: disable=E1123,E1124
 
 
-def login(password=None, email=None):
+def login(password: Optional[str] = None, email: Optional[str] = None):
     """Tries to get a fresh session id from the server by sending password and
     user_email to it. If a new session is granted (password and user_email match),
     gui switches to logged-in home view (login/register button hide, logged-in-as shows)
     """
     password = gui.app["login"]["pw_entry"].get() if password is None else password
     user_email = gui.app["login"]["email_entry"].get() if email is None else email
     with gui.db_conn as cursor:
-        session_id = server.login(cursor, user_email, password)
+        session_id = server.login(cursor, user_email, str(password))
 
     if session_id is None:
         gui.app.views_dict["login"].unhide_components("login_failed_label")
         return
 
     gui.app.data["session_id"] = session_id
     gui.app["login"].hide_components("login_failed_label")
     switch_to_home()
 
     # pylint: disable=unbalanced-tuple-unpacking
     with gui.db_conn as cursor:
         session_id, user_data = server.query_user_data(
-            cursor, user_email, user_email=user_email, session_id=session_id
+            cursor, user_email, session=server.Session(session_id, user_email)
         )
 
     gui.app.data["session_id"] = session_id
     store_user_data(user_data)
     gui.app["main_menu"].unhide_components("logged_in_as_frame")
     gui.app["main_menu"].hide_components("message_frame", "login_button", "register_button")
     set_logged_in_as_user_text()
@@ -46,15 +50,15 @@
 def sign_out():
     """Signs out the currently logged in user. clears the user data, login data,
     register data, checkout basket and returns to not-logged-in home view
     (unhides register/login buttons, hides logged-in-as message)
     """
     gui.app.data = {
         "session_id": None,
-        "user_data": user.UserSignUpData(),
+        "user_data": None,
         "pw_hash": "",
         "cart": [],
     }
     gui.app["login"].clear_entries()
     gui.app["register"].clear_entries()
     gui.app["checkout"].clear()
     gui.app["main_menu"].hide_components("logged_in_as_frame", "message_frame", "checkout_button")
@@ -69,26 +73,30 @@
 
 
 def register():
     """Gets all data entered in the register view and validates it. If valid,
     send the data and the current date to the server and add it to a new user
     in the database, else show an error message
     """
-    user_data = gui.app["register"].get_user_data()
+    user_data: user.UserData = gui.app["register"].get_user_data()
     valid_data = validate_user_data(user_data)
 
     password = gui.app["register"]["pw_entry"].get_var()
     confirm_password = gui.app["register"]["confirm_pw_entry"].get_var()
     valid_password = validate_password(password, confirm_password)
 
     if not valid_data or not valid_password:
         return
 
     with gui.db_conn as cursor:
-        session_id = server.add_user(cursor, user_data, password)
+        try:
+            session_id = server.add_user(cursor, user_data, password)
+        except server.DuplicateUserError:
+            show_error_message("You cannot use the supplied email.")
+            return
 
     gui.app.data["session_id"] = session_id
     if session_id is not None:
         login(password, user_data.email)
         gui.app["register"].clear_entries()
     else:
         show_error_message("Failed to register.")
@@ -97,30 +105,29 @@
 def edit_user_data():
     """Edits the user data (callback for edit in profile view). Gets all user
     data from the text entries and validates it using validate_user_data. If
     valid, the data is sent to the server. If the server does not respond with
     a valid new session id, the changes failed and a corresponding error message
     is shown.
     """
-    user_data = gui.app["profile"].get_user_data()
+    user_data: user.UserData = gui.app["profile"].get_user_data()
     valid_data = validate_user_data(user_data)
     if not valid_data:
         return
 
     session_id = gui.app.data["session_id"]
 
     with gui.db_conn as cursor:
         user_data_ = user_data[:-1]  # ignore join date
         # pylint: disable=unpacking-non-sequence
         new_session_id, *_ = server.update_user(
             cursor,
             user_data_,
             user_data.email,
-            user_email=user_data.email,
-            session_id=session_id,
+            session=server.Session(session_id, user_data.email),
         )
 
     gui.app.data["session_id"] = new_session_id
     gui.app.data["user_data"] = user_data
     populate_profile_with_user_data()
     if not new_session_id:
         show_error_message("Failed to edit data.")
@@ -141,49 +148,49 @@
 
     session_id = gui.app.data["session_id"]
     user_email = gui.app.data["user_data"].email
 
     with gui.db_conn as cursor:
         # pylint: disable=unpacking-non-sequence
         new_session_id, *_ = server.update_user_password(
-            cursor, password, user_email, user_email=user_email, session_id=session_id
+            cursor, password, user_email, session=server.Session(session_id, user_email)
         )
 
     gui.app.data["session_id"] = new_session_id
     if not new_session_id:
         show_error_message("Failed to edit password.")
         return
 
     show_message("Set new password successfully.")
     gui.app["profile"]["confirm_pw_entry"].set_var("")
     gui.app["profile"]["pw_entry"].set_var("")
     gui.app["profile"].hide_components("password_change_frame")
     gui.app["profile"].unhide_components("password_change_frame_button")
 
 
-def validate_user_data(user_data):
+def validate_user_data(user_data: user.UserData):
     """Validates all the data entered in the register view. Validates that the
     email is in the correct format, validates that the first and last name are
     alphabetic and not empty, validates that the gender is either m or f and
     validates that the date of birth is a valid date and is not empty
     """
     # validate email
     found_email = re.findall(".+?@.+\\..+", user_data.email)
     if not found_email:
         show_error_message("Email needs to be of the format address@domain.")
         return False
 
     # validate first_name
-    found_first_name = re.match("[a-zA-Z]+$", user_data.first_name)
+    found_first_name = re.match(r"[^\W_0-9]+$", user_data.first_name)
     if not found_first_name:
         show_error_message("First name needs to be alphabetic.")
         return False
 
     # validate last_name
-    found_last_name = re.match("[a-zA-Z]+$", user_data.last_name)
+    found_last_name = re.match(r"[^\W__0-9]+$", user_data.last_name)
     if not found_last_name:
         show_error_message("Last name needs to be alphabetic.")
         return False
 
     # validate gender
     found_gender = re.match("[mf]$", user_data.gender)
     if user_data.gender and not found_gender:
@@ -194,51 +201,51 @@
     if user_data.dob and not util.validate_date_string(user_data.dob):
         show_error_message("Date of birth needs to be in the format YYYY-MM-DD.")
         return False
 
     return True
 
 
-def validate_password(password, confirm_password):
+def validate_password(password: str, confirm_password: str):
     """Validates that the passwords match and are longer than 8 characters (returns bool)"""
     if len(password) < 8:
         show_error_message("Password needs to be at least 8 characters long.")
         return False
 
     if not password == confirm_password:
         show_error_message("Passwords don't match.")
         return False
 
     return True
 
 
-def show_message(message):
+def show_message(message: str):
     """Shows the specified message in the main menu view"""
     gui.app["main_menu"]["message_label"].set_var(message)
     gui.app["main_menu"].hide_components("error_message_label")
     gui.app["main_menu"].unhide_components("message_label", "message_frame")
 
 
-def show_error_message(message):
+def show_error_message(message: str):
     """Shows the specified error message in the main menu view"""
     gui.app["main_menu"]["error_message_label"].set_var(message)
     gui.app["main_menu"].hide_components("message_frame")
     gui.app["main_menu"].unhide_components("error_message_label", "message_frame")
 
 
 def show_password_change_frame():
     """Callback for change password button in profile view, unhides the password change frame"""
     gui.app["profile"].unhide_components("password_change_frame")
     gui.app["profile"].hide_components("password_change_frame_button")
 
 
-def store_user_data(user_data):
+def store_user_data(user_data: Optional[Collection[str]]):
     """Stores the passed user data in the appropriate gui data fields"""
-    if len(user_data) == 6:
-        gui.app.data["user_data"] = user.UserSignUpData(*user_data)
+    if user_data and len(user_data) == 6:
+        gui.app.data["user_data"] = user.UserSignUpData(*user_data)  # type: ignore
     else:
         sign_out()
         show_error_message("Something went wrong while logging in. 2")
 
 
 def switch_to_home():
     """Switches to home view"""
@@ -265,15 +272,15 @@
 
 def switch_to_profile():
     """Switches to the profile view after populating it with the currently logged in user data"""
     populate_profile_with_user_data()
     gui.app.switch_to("profile", "main_menu")
 
 
-def activate_profile_entry(entry_name):
+def activate_profile_entry(entry_name: str):
     """Callback for edit button for the respective field in the user data profile view"""
     gui.app["profile"][entry_name].config(state="normal")
     gui.app["profile"]["edit_user_data_button"].config(state="normal")
 
 
 def on_dropdown_value_write_event(*_):
     """Callback for options dropdown selection, either switches to profile view or signs out"""
```

### Comparing `desktop_shop-1.0.5/desktop_shop/gui/components.py` & `desktop_shop-1.1.0/desktop_shop/gui/components.py`

 * *Files identical despite different names*

### Comparing `desktop_shop-1.0.5/desktop_shop/gui/config.py` & `desktop_shop-1.1.0/desktop_shop/gui/config.py`

 * *Files identical despite different names*

### Comparing `desktop_shop-1.0.5/desktop_shop/gui/init.py` & `desktop_shop-1.1.0/desktop_shop/gui/init.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Created on Mon Feb  1 10:00:48 2021
 
 @author: Korean_Crimson
 """
 import tkinter as tk
 from typing import Dict
 
-from desktop_shop import gui, user
+from desktop_shop import gui
 from desktop_shop.gui import components, config
 from desktop_shop.gui.components import Builder, Component, EntryFactory, Factory, Frame
 from desktop_shop.gui.views import views
 
 
 def _set_transparent_colour():
     # this apparently fails on linux for no particular reason
@@ -58,12 +58,12 @@
 def init():
     """Init function that needs to be called before gui is started"""
     init_root()
     gui.app.builder = init_builder()
     gui.app.views_dict = init_views(gui.root, gui.app.builder)
     gui.app.data = {
         "session_id": None,
-        "user_data": user.UserSignUpData(),
+        "user_data": None,
         "pw_hash": "",
         "cart": [],
     }
-    gui.app["home"].init_product_data(gui.root, gui.app.builder)
+    gui.app["home"].init_product_data(gui.root, gui.app.builder)  # type: ignore
```

### Comparing `desktop_shop-1.0.5/desktop_shop/gui/views/checkout.py` & `desktop_shop-1.1.0/desktop_shop/gui/views/checkout.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,16 +101,15 @@
                 # pylint: disable=redundant-keyword-arg
                 # pylint: disable=unexpected-keyword-arg
                 # pylint: disable=unpacking-non-sequence
                 new_session_id, _ = server.add_transaction(
                     cursor,
                     user_email,
                     chosen_product_ids,
-                    user_email=user_email,
-                    session_id=session_id,
+                    session=server.Session(session_id, user_email),
                 )
 
             gui.app.data["session_id"] = new_session_id
             if new_session_id is not None:
                 callbacks.show_message("We have placed your order.")
                 gui.app.data["cart"] = []
                 gui.app.views_dict["checkout"].clear()
```

### Comparing `desktop_shop-1.0.5/desktop_shop/gui/views/home.py` & `desktop_shop-1.1.0/desktop_shop/gui/views/home.py`

 * *Files identical despite different names*

### Comparing `desktop_shop-1.0.5/desktop_shop/gui/views/login.py` & `desktop_shop-1.1.0/desktop_shop/gui/views/login.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
         # password
         builder.create("label", text="Password").place(row=2, col=0)
         edit = builder.create("entry", name="pw", textvariable=tk.StringVar(), show="*")
         edit.place(row=2, col=1, sticky="nsew")
 
         builder.create("button2", text="Log in", command=callbacks.login).place(row=3, col=1)
+        frame.component.tk_component.bind("<Return>", lambda *_: callbacks.login())
 
         # login unsuccessful
         message = "Logging in has failed. Please check your credentials."
         label = builder.create("label2", name="login_failed", text=message)
         label.place(row=4, col=0, col_span=3)
         builder.view.hide_components("login_failed_label")
```

### Comparing `desktop_shop-1.0.5/desktop_shop/gui/views/main_menu.py` & `desktop_shop-1.1.0/desktop_shop/gui/views/main_menu.py`

 * *Files identical despite different names*

### Comparing `desktop_shop-1.0.5/desktop_shop/gui/views/profile.py` & `desktop_shop-1.1.0/desktop_shop/gui/views/profile.py`

 * *Files identical despite different names*

### Comparing `desktop_shop-1.0.5/desktop_shop/gui/views/register.py` & `desktop_shop-1.1.0/desktop_shop/gui/views/register.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         # confirm pw
         builder.create("label", text="*Confirm Password").place(row=7, col=0)
         entry = builder.create("entry", name="confirm_pw", textvariable=tk.StringVar(), show="*")
         entry.place(row=7, col=1, sticky="nsew")
 
         builder.create("label", text="*required").place(row=8, col=1)
         builder.create("button2", text="Register", command=callbacks.register).place(row=9, col=1)
+        frame.component.tk_component.bind("<Return>", lambda *_: callbacks.register())
         return builder.view
 
     def clear_entries(self):
         """Clears all entries in the register view"""
         for entry in self.filter("entry"):
             entry.set_var("")
```

### Comparing `desktop_shop-1.0.5/desktop_shop/user.py` & `desktop_shop-1.1.0/desktop_shop/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,21 +7,18 @@
 
 from dataclasses import dataclass
 
 
 # pylint: disable=function-redefined
 @dataclass
 class UserData:
-    """Stores user data
+    """Stores user data"""
 
-    FIXME: crashes when first_name or last_name are accessed without being set.
-    """
-
-    first_name: str = ""
-    last_name: str = ""
+    first_name: str  # type: ignore
+    last_name: str  # type: ignore
     gender: str = ""
     dob: str = ""  # date of birth
     email: str = ""
 
     def __getitem__(self, value):
         return list(self)[value]
```

### Comparing `desktop_shop-1.0.5/desktop_shop/util.py` & `desktop_shop-1.1.0/desktop_shop/util.py`

 * *Files identical despite different names*

### Comparing `desktop_shop-1.0.5/desktop_shop.egg-info/PKG-INFO` & `desktop_shop-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 Metadata-Version: 2.1
-Name: desktop-shop
-Version: 1.0.5
+Name: desktop_shop
+Version: 1.1.0
 Summary: Desktop shop application
 Home-page: https://github.com/rbaltrusch/desktop_shop
 Author: Richard Baltrusch
 License: MIT
 Keywords: python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Desktop Environment
+Classifier: Topic :: Education
+Classifier: Topic :: Education :: Testing
+Classifier: Topic :: Office/Business
+Classifier: Topic :: Office/Business :: Financial :: Point-Of-Sale
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: wikipedia==1.4.0
+Requires-Dist: requests==2.30.0
+Requires-Dist: beautifulsoup4==4.12.2
 
 [![Unit tests](https://github.com/rbaltrusch/desktop_shop/actions/workflows/pytest-unit-tests.yml/badge.svg)](https://github.com/rbaltrusch/desktop_shop/actions/workflows/pytest-unit-tests.yml)
 [![Pylint](https://github.com/rbaltrusch/desktop_shop/actions/workflows/pylint.yml/badge.svg)](https://github.com/rbaltrusch/desktop_shop/actions/workflows/pylint.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](https://opensource.org/licenses/MIT)
 
 # Desktop Shop
 
@@ -40,14 +51,24 @@
 Run the shop application by installing the package using pip, then calling it:
 
     python -m pip install desktop_shop
     python -m desktop_shop
 
 Note that the first time the package is called, it automatically generates a fresh database filled with random data. This make take a few seconds.
 
+## ⚠️ State of the repository ⚠️
+
+This repository is unlikely to receive new features in the future, although maintenance and small fixes will still be done.
+
+This means that some features that are missing now will stay missing (but feel free to submit a pull request to add them!), and non-optimal aspects of the codebase or the application are unlikely to get fixed. Some of these include:
+- No admin panel
+- A user cannot see the transactions that he has placed in the past
+- The application asking for gender is a violation of the EU GDPR, as this user data is not required with the application as is (the same potentially applies to collecting date of birth).
+- The interface to the database is not ideal, as typing is missing for the most part, it is somewhat internally inconsistent, and is using lists or tuples instead of objects.
+
 ## Contributions
 
 To contribute to this repository, please read the [contribution guidelines](https://github.com/rbaltrusch/desktop_shop/blob/master/CONTRIBUTING.md).
 
 ## Python
 
 Written in Python 3.8.3.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `desktop_shop-1.0.5/desktop_shop.egg-info/SOURCES.txt` & `desktop_shop-1.1.0/desktop_shop.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 ./desktop_shop/__init__.py
 ./desktop_shop/__main__.py
 ./desktop_shop/crypto.py
-./desktop_shop/database.py
 ./desktop_shop/py.typed
 ./desktop_shop/server.py
 ./desktop_shop/user.py
 ./desktop_shop/util.py
 ./desktop_shop/datagen/__init__.py
 ./desktop_shop/datagen/data.py
 ./desktop_shop/datagen/generate_data.py
```

### Comparing `desktop_shop-1.0.5/pyproject.toml` & `desktop_shop-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `desktop_shop-1.0.5/setup.py` & `desktop_shop-1.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 project_dir = Path(__file__).parent
 
 setuptools.setup(
     name="desktop_shop",
-    version="1.0.5",
+    version="1.1.0",
     description="Desktop shop application",
     long_description=project_dir.joinpath("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     keywords=["python"],
     author="Richard Baltrusch",
     url="https://github.com/rbaltrusch/desktop_shop",
     packages=setuptools.find_packages("."),
@@ -26,17 +26,25 @@
     .read_text(encoding="utf-8")
     .split("\n"),
     zip_safe=False,
     license="MIT",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
+        "Intended Audience :: Education",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Topic :: Desktop Environment",
+        "Topic :: Education",
+        "Topic :: Education :: Testing",
+        "Topic :: Office/Business",
+        "Topic :: Office/Business :: Financial :: Point-Of-Sale",
         "Typing :: Typed",
     ],
 )
```

