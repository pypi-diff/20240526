# Comparing `tmp/contacts_assistant-0.0.8.tar.gz` & `tmp/contacts_assistant-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contacts_assistant-0.0.8.tar", last modified: Sun May 26 14:18:24 2024, max compression
+gzip compressed data, was "contacts_assistant-0.0.9.tar", last modified: Sun May 26 14:35:12 2024, max compression
```

## Comparing `contacts_assistant-0.0.8.tar` & `contacts_assistant-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 14:18:24.232776 contacts_assistant-0.0.8/
--rw-rw-rw-   0        0        0     1095 2024-05-22 08:53:23.000000 contacts_assistant-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     4406 2024-05-26 14:18:24.231778 contacts_assistant-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-26 14:18:24.232776 contacts_assistant-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1523 2024-05-26 14:17:33.000000 contacts_assistant-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:18:24.211776 contacts_assistant-0.0.8/src/
--rw-rw-rw-   0        0        0     1219 2024-05-26 09:46:28.000000 contacts_assistant-0.0.8/src/Email.py
--rw-rw-rw-   0        0        0        0 2024-05-26 09:34:04.000000 contacts_assistant-0.0.8/src/__init__.py
--rw-rw-rw-   0        0        0     2144 2024-05-26 09:46:01.000000 contacts_assistant-0.0.8/src/address.py
--rw-rw-rw-   0        0        0     1338 2024-05-26 09:46:13.000000 contacts_assistant-0.0.8/src/birthday.py
--rw-rw-rw-   0        0        0     1199 2024-05-26 09:34:44.000000 contacts_assistant-0.0.8/src/command_completer.py
--rw-rw-rw-   0        0        0      837 2024-05-26 12:09:13.000000 contacts_assistant-0.0.8/src/constants.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:18:24.231778 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/
--rw-rw-rw-   0        0        0     4406 2024-05-26 14:18:24.000000 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2024-05-26 14:18:24.000000 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 14:18:24.000000 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-26 14:18:24.000000 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2024-05-26 14:18:24.000000 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0      144 2024-05-26 14:18:24.000000 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8543 2024-05-26 12:07:21.000000 contacts_assistant-0.0.8/src/contacts_book.py
--rw-rw-rw-   0        0        0     1989 2024-05-26 09:46:19.000000 contacts_assistant-0.0.8/src/date_helpers.py
--rw-rw-rw-   0        0        0      853 2024-05-26 09:28:57.000000 contacts_assistant-0.0.8/src/field.py
--rw-rw-rw-   0        0        0    17056 2024-05-26 12:06:31.000000 contacts_assistant-0.0.8/src/handler.py
--rw-rw-rw-   0        0        0     7499 2024-05-26 09:36:07.000000 contacts_assistant-0.0.8/src/menu.py
--rw-rw-rw-   0        0        0      595 2024-05-26 09:46:53.000000 contacts_assistant-0.0.8/src/name.py
--rw-rw-rw-   0        0        0     3286 2024-05-26 09:46:56.000000 contacts_assistant-0.0.8/src/note.py
--rw-rw-rw-   0        0        0     8400 2024-05-26 09:36:23.000000 contacts_assistant-0.0.8/src/notebook.py
--rw-rw-rw-   0        0        0     1508 2024-05-26 09:47:03.000000 contacts_assistant-0.0.8/src/phone.py
--rw-rw-rw-   0        0        0     6518 2024-05-26 09:47:09.000000 contacts_assistant-0.0.8/src/record.py
--rw-rw-rw-   0        0        0      549 2024-05-26 09:28:57.000000 contacts_assistant-0.0.8/src/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:35:12.577521 contacts_assistant-0.0.9/
+-rw-rw-rw-   0        0        0     1095 2024-05-22 08:53:23.000000 contacts_assistant-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4410 2024-05-26 14:35:12.576522 contacts_assistant-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-26 14:35:12.577521 contacts_assistant-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1523 2024-05-26 14:34:15.000000 contacts_assistant-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:35:12.550519 contacts_assistant-0.0.9/src/
+-rw-rw-rw-   0        0        0        0 2024-05-26 14:25:45.000000 contacts_assistant-0.0.9/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:35:12.558520 contacts_assistant-0.0.9/src/contacts_assistant/
+-rw-rw-rw-   0        0        0     1234 2024-05-26 14:25:02.000000 contacts_assistant-0.0.9/src/contacts_assistant/Email.py
+-rw-rw-rw-   0        0        0        0 2024-05-26 09:34:04.000000 contacts_assistant-0.0.9/src/contacts_assistant/__init__.py
+-rw-rw-rw-   0        0        0     2159 2024-05-26 14:25:02.000000 contacts_assistant-0.0.9/src/contacts_assistant/address.py
+-rw-rw-rw-   0        0        0     1368 2024-05-26 14:25:02.000000 contacts_assistant-0.0.9/src/contacts_assistant/birthday.py
+-rw-rw-rw-   0        0        0     1199 2024-05-26 09:34:44.000000 contacts_assistant-0.0.9/src/contacts_assistant/command_completer.py
+-rw-rw-rw-   0        0        0      835 2024-05-26 14:31:19.000000 contacts_assistant-0.0.9/src/contacts_assistant/constants.py
+-rw-rw-rw-   0        0        0     8558 2024-05-26 14:25:02.000000 contacts_assistant-0.0.9/src/contacts_assistant/contacts_book.py
+-rw-rw-rw-   0        0        0     2004 2024-05-26 14:25:02.000000 contacts_assistant-0.0.9/src/contacts_assistant/date_helpers.py
+-rw-rw-rw-   0        0        0      853 2024-05-26 09:28:57.000000 contacts_assistant-0.0.9/src/contacts_assistant/field.py
+-rw-rw-rw-   0        0        0    17191 2024-05-26 14:25:02.000000 contacts_assistant-0.0.9/src/contacts_assistant/handler.py
+-rw-rw-rw-   0        0        0     7529 2024-05-26 14:25:02.000000 contacts_assistant-0.0.9/src/contacts_assistant/menu.py
+-rw-rw-rw-   0        0        0      610 2024-05-26 14:25:02.000000 contacts_assistant-0.0.9/src/contacts_assistant/name.py
+-rw-rw-rw-   0        0        0     3301 2024-05-26 14:25:02.000000 contacts_assistant-0.0.9/src/contacts_assistant/note.py
+-rw-rw-rw-   0        0        0     8415 2024-05-26 14:25:02.000000 contacts_assistant-0.0.9/src/contacts_assistant/notebook.py
+-rw-rw-rw-   0        0        0     1523 2024-05-26 14:25:02.000000 contacts_assistant-0.0.9/src/contacts_assistant/phone.py
+-rw-rw-rw-   0        0        0     6593 2024-05-26 14:25:02.000000 contacts_assistant-0.0.9/src/contacts_assistant/record.py
+-rw-rw-rw-   0        0        0      549 2024-05-26 09:28:57.000000 contacts_assistant-0.0.9/src/contacts_assistant/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:35:12.575522 contacts_assistant-0.0.9/src/contacts_assistant.egg-info/
+-rw-rw-rw-   0        0        0     4410 2024-05-26 14:35:12.000000 contacts_assistant-0.0.9/src/contacts_assistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2024-05-26 14:35:12.000000 contacts_assistant-0.0.9/src/contacts_assistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:35:12.000000 contacts_assistant-0.0.9/src/contacts_assistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-26 14:35:12.000000 contacts_assistant-0.0.9/src/contacts_assistant.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-05-26 14:35:12.000000 contacts_assistant-0.0.9/src/contacts_assistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2024-05-26 14:35:12.000000 contacts_assistant-0.0.9/src/contacts_assistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2307 2024-05-26 14:25:02.000000 contacts_assistant-0.0.9/src/main.py
```

### Comparing `contacts_assistant-0.0.8/LICENSE` & `contacts_assistant-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.8/PKG-INFO` & `contacts_assistant-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contacts_assistant
-Version: 0.0.8
+Version: 0.0.9
 Summary: Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.
 Home-page: https://github.com/Bignichok/Python-ContactsAssistant
 Author: Mykyta Samoilenko
 Author-email: inikita546@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 ## Initialization
   ### locally
   1. Initialize virtual environment
      - .venv\Scripts\activate.bat - Windows у командному рядку (CMD)
      - .venv\Scripts\Activate.ps1 - Windows у PowerShell
      - source .venv/bin/activate - macOS та Linux
   2. pip install -r requirements.txt
-  3. python main.py
+  3. python src\main.py
   4. use one of commands presented below (bot will suggest you commands and named arguments that you need)
   ### installed package
   1. Initialize virtual environment
      - .venv\Scripts\activate.bat - Windows у командному рядку (CMD)
      - .venv\Scripts\Activate.ps1 - Windows у PowerShell
      - source .venv/bin/activate - macOS та Linux
   2. pip install contacts-assistant
```

### Comparing `contacts_assistant-0.0.8/setup.py` & `contacts_assistant-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     encoding = result['encoding']
 
 with open("requirements.txt", "r", encoding=encoding) as fh:
     requirements = fh.read().splitlines()
 
 setuptools.setup(
     name="contacts_assistant",
-    version="0.0.8",
+    version="0.0.9",
     include_package_data=True,
     author="Mykyta Samoilenko",
     author_email="inikita546@gmail.com",
     description="Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bignichok/Python-ContactsAssistant",
```

### Comparing `contacts_assistant-0.0.8/src/Email.py` & `contacts_assistant-0.0.9/src/contacts_assistant/Email.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from src.field import Field
+from contacts_assistant.field import Field
 
 class Email(Field):
     """
     A class to represent and validate an email.
 
     Attributes:
         value (str): The validated email.
```

### Comparing `contacts_assistant-0.0.8/src/address.py` & `contacts_assistant-0.0.9/src/contacts_assistant/address.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Module containing classes to represent addresses and related enums.
 """
 
 from enum import Enum
-from src.field import Field
+from contacts_assistant.field import Field
 
 
 class AddressType(Enum):
     """
     Enumeration class for address types.
     """
```

### Comparing `contacts_assistant-0.0.8/src/birthday.py` & `contacts_assistant-0.0.9/src/contacts_assistant/birthday.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 
-from src.field import Field
-from src.constants import DATE_FORMAT
+from contacts_assistant.field import Field
+from contacts_assistant.constants import DATE_FORMAT
 
 class Birthday(Field):
     """
     A class to represent and validate a birthday.
 
     Inherits from Field to provide a consistent interface for different types of fields.
```

### Comparing `contacts_assistant-0.0.8/src/command_completer.py` & `contacts_assistant-0.0.9/src/contacts_assistant/command_completer.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.8/src/constants.py` & `contacts_assistant-0.0.9/src/contacts_assistant/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 DATE_FORMAT = "%d.%m.%Y"
-CONTACTS_BOOK_FILENAME = "../contacts_book.pkl"
-NOTEBOOK_FILENAME = "../notebook.json"
+CONTACTS_BOOK_FILENAME = "./contacts_book.pkl"
+NOTEBOOK_FILENAME = "./notebook.json"
 MENU_BORDER = f"{'-'*72}\n"
 DEMO_CONTACTS = 10
 GREETING_BANNER = """
   ___          _     _              _     _           _   
  / _ \        (_)   | |            | |   | |         | |  
 / /_\ \___ ___ _ ___| |_ __ _ _ __ | |_  | |__   ___ | |_ 
 |  _  / __/ __| / __| __/ _` | '_ \| __| | '_ \ / _ \| __|
```

### Comparing `contacts_assistant-0.0.8/src/contacts_assistant.egg-info/PKG-INFO` & `contacts_assistant-0.0.9/src/contacts_assistant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contacts_assistant
-Version: 0.0.8
+Version: 0.0.9
 Summary: Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.
 Home-page: https://github.com/Bignichok/Python-ContactsAssistant
 Author: Mykyta Samoilenko
 Author-email: inikita546@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 ## Initialization
   ### locally
   1. Initialize virtual environment
      - .venv\Scripts\activate.bat - Windows у командному рядку (CMD)
      - .venv\Scripts\Activate.ps1 - Windows у PowerShell
      - source .venv/bin/activate - macOS та Linux
   2. pip install -r requirements.txt
-  3. python main.py
+  3. python src\main.py
   4. use one of commands presented below (bot will suggest you commands and named arguments that you need)
   ### installed package
   1. Initialize virtual environment
      - .venv\Scripts\activate.bat - Windows у командному рядку (CMD)
      - .venv\Scripts\Activate.ps1 - Windows у PowerShell
      - source .venv/bin/activate - macOS та Linux
   2. pip install contacts-assistant
```

### Comparing `contacts_assistant-0.0.8/src/contacts_book.py` & `contacts_assistant-0.0.9/src/contacts_assistant/contacts_book.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import date
 from collections import UserDict
 import pickle
 
-from src.date_helpers import DateHelper
+from contacts_assistant.date_helpers import DateHelper
 
 
 def is_weekend_day(day: int) -> bool:
     """
     Checks if a given day is a weekend.
 
     Args:
```

### Comparing `contacts_assistant-0.0.8/src/date_helpers.py` & `contacts_assistant-0.0.9/src/contacts_assistant/date_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module provides helper functions for date manipulation,
 including formatting workdays and calculating the next birthday.
 """
 
 from datetime import date as dt_date
 from datetime import timedelta
 
-from src.constants import DATE_FORMAT
+from contacts_assistant.constants import DATE_FORMAT
 
 
 class DateHelper:
     """
     A helper class for date-related operations.
     """
```

### Comparing `contacts_assistant-0.0.8/src/field.py` & `contacts_assistant-0.0.9/src/contacts_assistant/field.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.8/src/handler.py` & `contacts_assistant-0.0.9/src/contacts_assistant/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Handler module"""
 
-from src.address import AddressType
-from src.command_completer import CommandCompleter
-from src.constants import GREETING_BANNER, CONTACTS_BOOK_FILENAME, NOTEBOOK_FILENAME
-from src.menu import Menu
-from src.utils import format_greeting
-from src.contacts_book import ContactsBook
-from src.record import Record
-from src.notebook import Notebook
-from src.note import Note
+from contacts_assistant.address import AddressType
+from contacts_assistant.command_completer import CommandCompleter
+from contacts_assistant.constants import GREETING_BANNER, CONTACTS_BOOK_FILENAME, NOTEBOOK_FILENAME
+from contacts_assistant.menu import Menu
+from contacts_assistant.utils import format_greeting
+from contacts_assistant.contacts_book import ContactsBook
+from contacts_assistant.record import Record
+from contacts_assistant.notebook import Notebook
+from contacts_assistant.note import Note
 
 NOT_FOUND_MESSAGE = "Contact does not exist, you can add it"
 
 
 def handle_error(func):
     """
     Decorator to handle exceptions in the wrapped function.
```

### Comparing `contacts_assistant-0.0.8/src/menu.py` & `contacts_assistant-0.0.9/src/contacts_assistant/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Class Menu module"""
 
 import difflib
 import argparse
 from enum import Enum
 from collections import namedtuple
 
-from src.constants import MENU_BORDER
-from src.utils import format_cmd, format_param
+from contacts_assistant.constants import MENU_BORDER
+from contacts_assistant.utils import format_cmd, format_param
 
 Command = namedtuple("Command", ["min_required_params", "param_list", "hint"])
 Parametr = namedtuple(
     "Parametr",
     ["name", "required", "hint", "choices"],
     defaults=(None, False, None, None),
 )
```

### Comparing `contacts_assistant-0.0.8/src/name.py` & `contacts_assistant-0.0.9/src/contacts_assistant/name.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.field import Field
+from contacts_assistant.field import Field
 
 class Name(Field):
     """
     A class to represent and validate a name.
 
     Inherits from Field to provide a consistent interface for different types of fields.
```

### Comparing `contacts_assistant-0.0.8/src/note.py` & `contacts_assistant-0.0.9/src/contacts_assistant/note.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from datetime import datetime
 
-from src.constants import DATE_FORMAT
+from contacts_assistant.constants import DATE_FORMAT
 
 class Note:
     def __init__(self, title, content, tags=None, due_date=None):
         """
         Initialize a Note instance.
 
         Args:
```

### Comparing `contacts_assistant-0.0.8/src/notebook.py` & `contacts_assistant-0.0.9/src/contacts_assistant/notebook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from datetime import datetime, timedelta
 
-from src.note import Note
+from contacts_assistant.note import Note
 
 class Notebook:
     def __init__(self):
         """
         Initialize a Notebook instance.
         """
         self.notes = []
```

### Comparing `contacts_assistant-0.0.8/src/phone.py` & `contacts_assistant-0.0.9/src/contacts_assistant/phone.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.field import Field
+from contacts_assistant.field import Field
 
 class Phone(Field):
     """
     A class to represent and validate a phone number.
 
     Inherits from Field to provide a consistent interface for different types of fields.
```

### Comparing `contacts_assistant-0.0.8/src/record.py` & `contacts_assistant-0.0.9/src/contacts_assistant/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from src.phone import Phone
-from src.name import Name
-from src.birthday import Birthday
-from src.Email import Email
-from src.address import Address, AddressType
+from contacts_assistant.phone import Phone
+from contacts_assistant.name import Name
+from contacts_assistant.birthday import Birthday
+from contacts_assistant.Email import Email
+from contacts_assistant.address import Address, AddressType
 
 
 class Record:
     """
     A class to represent a contact record.
 
     Attributes:
```

### Comparing `contacts_assistant-0.0.8/src/utils.py` & `contacts_assistant-0.0.9/src/contacts_assistant/utils.py`

 * *Files identical despite different names*

