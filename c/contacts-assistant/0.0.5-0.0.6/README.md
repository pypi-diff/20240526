# Comparing `tmp/contacts_assistant-0.0.5.tar.gz` & `tmp/contacts_assistant-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contacts_assistant-0.0.5.tar", last modified: Fri May 24 20:52:08 2024, max compression
+gzip compressed data, was "contacts_assistant-0.0.6.tar", last modified: Sun May 26 12:14:43 2024, max compression
```

## Comparing `contacts_assistant-0.0.5.tar` & `contacts_assistant-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 20:52:08.884966 contacts_assistant-0.0.5/
--rw-rw-rw-   0        0        0     1095 2024-05-22 08:53:23.000000 contacts_assistant-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     4080 2024-05-24 20:52:08.883963 contacts_assistant-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3313 2024-05-24 13:50:38.000000 contacts_assistant-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 20:52:08.884966 contacts_assistant-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1629 2024-05-24 20:51:58.000000 contacts_assistant-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:52:08.842962 contacts_assistant-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-24 20:52:08.852964 contacts_assistant-0.0.5/src/contacts_assistant/
--rw-rw-rw-   0        0        0     1330 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/Birthday.py
--rw-rw-rw-   0        0        0     1217 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/Email.py
--rw-rw-rw-   0        0        0      853 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/Field.py
--rw-rw-rw-   0        0        0      591 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/Name.py
--rw-rw-rw-   0        0        0     1504 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/Phone.py
--rw-rw-rw-   0        0        0     6498 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/Record.py
--rw-rw-rw-   0        0        0        0 2024-05-24 20:13:39.000000 contacts_assistant-0.0.5/src/contacts_assistant/__init__.py
--rw-rw-rw-   0        0        0     2248 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/__main__.py
--rw-rw-rw-   0        0        0     2140 2024-05-24 20:18:37.000000 contacts_assistant-0.0.5/src/contacts_assistant/address.py
--rw-rw-rw-   0        0        0     1201 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/command_completer.py
--rw-rw-rw-   0        0        0      834 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/constants.py
--rw-rw-rw-   0        0        0     8535 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/contactsBook.py
--rw-rw-rw-   0        0        0     1983 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/datehelper.py
--rw-rw-rw-   0        0        0    16904 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/handler.py
--rw-rw-rw-   0        0        0     6995 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/menu.py
--rw-rw-rw-   0        0        0     3280 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/note.py
--rw-rw-rw-   0        0        0     8394 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/notebook.py
--rw-rw-rw-   0        0        0      549 2024-05-24 20:10:40.000000 contacts_assistant-0.0.5/src/contacts_assistant/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:52:08.882964 contacts_assistant-0.0.5/src/contacts_assistant.egg-info/
--rw-rw-rw-   0        0        0     4080 2024-05-24 20:52:08.000000 contacts_assistant-0.0.5/src/contacts_assistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      922 2024-05-24 20:52:08.000000 contacts_assistant-0.0.5/src/contacts_assistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 20:52:08.000000 contacts_assistant-0.0.5/src/contacts_assistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-05-24 20:52:08.000000 contacts_assistant-0.0.5/src/contacts_assistant.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2024-05-24 20:52:08.000000 contacts_assistant-0.0.5/src/contacts_assistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-24 20:52:08.000000 contacts_assistant-0.0.5/src/contacts_assistant.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 12:14:43.405184 contacts_assistant-0.0.6/
+-rw-rw-rw-   0        0        0     1095 2024-05-22 08:53:23.000000 contacts_assistant-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4095 2024-05-26 12:14:43.404184 contacts_assistant-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-26 12:14:43.406186 contacts_assistant-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1523 2024-05-26 12:14:41.000000 contacts_assistant-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:14:43.382182 contacts_assistant-0.0.6/src/
+-rw-rw-rw-   0        0        0     1219 2024-05-26 09:46:28.000000 contacts_assistant-0.0.6/src/Email.py
+-rw-rw-rw-   0        0        0        0 2024-05-26 09:34:04.000000 contacts_assistant-0.0.6/src/__init__.py
+-rw-rw-rw-   0        0        0     2144 2024-05-26 09:46:01.000000 contacts_assistant-0.0.6/src/address.py
+-rw-rw-rw-   0        0        0     1338 2024-05-26 09:46:13.000000 contacts_assistant-0.0.6/src/birthday.py
+-rw-rw-rw-   0        0        0     1199 2024-05-26 09:34:44.000000 contacts_assistant-0.0.6/src/command_completer.py
+-rw-rw-rw-   0        0        0      837 2024-05-26 12:09:13.000000 contacts_assistant-0.0.6/src/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:14:43.403183 contacts_assistant-0.0.6/src/contacts_assistant.egg-info/
+-rw-rw-rw-   0        0        0     4095 2024-05-26 12:14:43.000000 contacts_assistant-0.0.6/src/contacts_assistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2024-05-26 12:14:43.000000 contacts_assistant-0.0.6/src/contacts_assistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 12:14:43.000000 contacts_assistant-0.0.6/src/contacts_assistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-26 12:14:43.000000 contacts_assistant-0.0.6/src/contacts_assistant.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-05-26 12:14:43.000000 contacts_assistant-0.0.6/src/contacts_assistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      144 2024-05-26 12:14:43.000000 contacts_assistant-0.0.6/src/contacts_assistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8543 2024-05-26 12:07:21.000000 contacts_assistant-0.0.6/src/contacts_book.py
+-rw-rw-rw-   0        0        0     1989 2024-05-26 09:46:19.000000 contacts_assistant-0.0.6/src/date_helpers.py
+-rw-rw-rw-   0        0        0      853 2024-05-26 09:28:57.000000 contacts_assistant-0.0.6/src/field.py
+-rw-rw-rw-   0        0        0    17056 2024-05-26 12:06:31.000000 contacts_assistant-0.0.6/src/handler.py
+-rw-rw-rw-   0        0        0     7499 2024-05-26 09:36:07.000000 contacts_assistant-0.0.6/src/menu.py
+-rw-rw-rw-   0        0        0      595 2024-05-26 09:46:53.000000 contacts_assistant-0.0.6/src/name.py
+-rw-rw-rw-   0        0        0     3286 2024-05-26 09:46:56.000000 contacts_assistant-0.0.6/src/note.py
+-rw-rw-rw-   0        0        0     8400 2024-05-26 09:36:23.000000 contacts_assistant-0.0.6/src/notebook.py
+-rw-rw-rw-   0        0        0     1508 2024-05-26 09:47:03.000000 contacts_assistant-0.0.6/src/phone.py
+-rw-rw-rw-   0        0        0     6518 2024-05-26 09:47:09.000000 contacts_assistant-0.0.6/src/record.py
+-rw-rw-rw-   0        0        0      549 2024-05-26 09:28:57.000000 contacts_assistant-0.0.6/src/utils.py
```

### Comparing `contacts_assistant-0.0.5/LICENSE` & `contacts_assistant-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.5/PKG-INFO` & `contacts_assistant-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contacts_assistant
-Version: 0.0.5
+Version: 0.0.6
 Summary: Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.
 Home-page: https://github.com/Bignichok/Python-ContactsAssistant
 Author: Mykyta Samoilenko
 Author-email: inikita546@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,93 +39,93 @@
   - *Save the current state and stop the bot assistant*
   - **Arguments**: None
 
 - **"add_contact"**: 
   - *Add a contact to the address book or update an existing contact*
   - **Arguments**: `name`, `phone`, `email`, `birthday`
 
-- **"update_contact"**: 
+- **"update_phone"**: 
   - *Change the phone number of an existing contact*
   - **Arguments**: `name`, `oldphone`, `newphone`
 
 - **"delete_contact"**: 
   - *Delete contact by name*
   - **Arguments**: `name`
 
-- **"set_contact_birthday"**: 
+- **"set_birthday"**: 
   - *Add a birthday to a contact*
   - **Arguments**: `name`, `date %d.%m.%Y`
 
-- **"get_contact_birthday"**: 
+- **"show_birthday"**: 
   - *Show the birthday of a contact*
   - **Arguments**: `name`
 
-- **"get_contact_by_name"**: 
+- **"find_contact_by_name"**: 
   - *Find contact by name*
   - **Arguments**: `name`
 
-- **"get_contact_by_phone"**: 
+- **"find_contact_by_phone"**: 
   - *Find contact by phone*
   - **Arguments**: `phone`
 
-- **"get_contact_by_email"**: 
+- **"find_contact_by_email"**: 
   - *Find contact by email*
   - **Arguments**: `email`
 
-- **"get_all_contacts"**: 
+- **"show_all_contacts"**: 
   - *Returns a string representation of the address book*
   - **Arguments**: None
 
-- **"get_upcoming_birthdays"**: 
-  - *Returns a list of upcoming birthdays within the next 7 days*
-  - **Arguments**: None
+- **"upcoming_birthdays"**: 
+  - *Returns a list of upcoming birthdays within the specified number of days*
+  - **Arguments**: `days`
 
-- **"update_contact_email"**: 
+- **"update_email"**: 
   - *Update contact email*
   - **Arguments**: `name`, `email`
 
 - **"add_address"**: 
-  - *Update contact address*
+  - *Add or update the address of a contact*
   - **Arguments**: `name`, `addresstype`, `street`, `city`, `postalcode`, `country`
 
-- **"delete_address"**: 
-  - *Delete contact address*
+- **"remove_address"**: 
+  - *Remove the address of a contact*
   - **Arguments**: `name`, `addresstype`
 
 ### NoteBook
 - **"add_note"**: 
-  - *Add note*
+  - *Add a new note*
   - **Arguments**: None
 
 - **"find_note"**: 
-  - *Find note by title*
+  - *Find a note by title*
   - **Arguments**: `title`
 
 - **"delete_note"**: 
-  - *Delete note by title*
+  - *Delete a note by title*
   - **Arguments**: `title`
 
 - **"delete_all_notes"**: 
-  - *Delete note by title*
+  - *Delete all notes*
   - **Arguments**: None
 
 - **"update_note"**: 
-  - *Update note by title*
+  - *Update a note by title*
   - **Arguments**: `title`
 
 - **"search_notes"**: 
-  - *Search for notes containing the query in their title or content.*
+  - *Search for notes containing the query in their title or content*
   - **Arguments**: `query`
 
 - **"filter_notes_by_tag"**: 
-  - *Filter notes by tag.*
+  - *Filter notes by tag*
   - **Arguments**: `tag`
 
-- **"get_notes_in_days"**: 
-  - *Get notes that are due in the next specified number of days.*
+- **"notes_due_in_days"**: 
+  - *Show notes that are due within the next specified number of days*
   - **Arguments**: `days`
 
-- **"get_all_notes"**: 
-  - *to view a full notes list*
+- **"show_all_notes"**: 
+  - *Show all notes*
   - **Arguments**: None
 
 These commands help you manage and retrieve contact information and notes efficiently. Use them to keep your contacts book organized and up-to-date.
```

### Comparing `contacts_assistant-0.0.5/setup.py` & `contacts_assistant-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,15 @@
     encoding = result['encoding']
 
 with open("requirements.txt", "r", encoding=encoding) as fh:
     requirements = fh.read().splitlines()
 
 setuptools.setup(
     name="contacts_assistant",
-    version="0.0.5",
-    package_dir={'': 'src'},
-    packages=setuptools.find_packages(where='src'),
+    version="0.0.6",
     include_package_data=True,
     author="Mykyta Samoilenko",
     author_email="inikita546@gmail.com",
     description="Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bignichok/Python-ContactsAssistant",
@@ -36,11 +34,11 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
     entry_points={
         'console_scripts': [
-            'contacts-assistant=contacts_assistant.__main__:main'
+            'contacts-assistant=main:main'
         ]
     },
 )
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/Birthday.py` & `contacts_assistant-0.0.6/src/birthday.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 
-from Field import Field
-from constants import DATE_FORMAT
+from src.field import Field
+from src.constants import DATE_FORMAT
 
 class Birthday(Field):
     """
     A class to represent and validate a birthday.
 
     Inherits from Field to provide a consistent interface for different types of fields.
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/Email.py` & `contacts_assistant-0.0.6/src/Email.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 
-from Field import Field
-
+from src.field import Field
 
 class Email(Field):
     """
     A class to represent and validate an email.
 
     Attributes:
         value (str): The validated email.
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/Field.py` & `contacts_assistant-0.0.6/src/field.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/Name.py` & `contacts_assistant-0.0.6/src/name.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Field import Field
+from src.field import Field
 
 class Name(Field):
     """
     A class to represent and validate a name.
 
     Inherits from Field to provide a consistent interface for different types of fields.
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/Phone.py` & `contacts_assistant-0.0.6/src/phone.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Field import Field
+from src.field import Field
 
 class Phone(Field):
     """
     A class to represent and validate a phone number.
 
     Inherits from Field to provide a consistent interface for different types of fields.
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/Record.py` & `contacts_assistant-0.0.6/src/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from Phone import Phone
-from Name import Name
-from Birthday import Birthday
-from Email import Email
-from address import Address, AddressType
+from src.phone import Phone
+from src.name import Name
+from src.birthday import Birthday
+from src.Email import Email
+from src.address import Address, AddressType
 
 
 class Record:
     """
     A class to represent a contact record.
 
     Attributes:
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/address.py` & `contacts_assistant-0.0.6/src/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Module containing classes to represent addresses and related enums.
 """
 
 from enum import Enum
-from Field import Field
+from src.field import Field
 
 
 class AddressType(Enum):
     """
     Enumeration class for address types.
     """
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/command_completer.py` & `contacts_assistant-0.0.6/src/command_completer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from prompt_toolkit.completion import Completer, Completion
 
-
 class CommandCompleter(Completer):
     def __init__(self, command_args, book):
         super().__init__()
         self.command_args = command_args
         self.book = book
 
     def get_completions(self, document, complete_event):
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/constants.py` & `contacts_assistant-0.0.6/src/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 DATE_FORMAT = "%d.%m.%Y"
-CONTACTS_BOOK_FILENAME = "./contactsbook.pkl"
-NOTEBOOK_FILENAME = "./notebook.json"
+CONTACTS_BOOK_FILENAME = "../contacts_book.pkl"
+NOTEBOOK_FILENAME = "../notebook.json"
 MENU_BORDER = f"{'-'*72}\n"
 DEMO_CONTACTS = 10
 GREETING_BANNER = """
   ___          _     _              _     _           _   
  / _ \        (_)   | |            | |   | |         | |  
 / /_\ \___ ___ _ ___| |_ __ _ _ __ | |_  | |__   ___ | |_ 
 |  _  / __/ __| / __| __/ _` | '_ \| __| | '_ \ / _ \| __|
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/contactsBook.py` & `contacts_assistant-0.0.6/src/contacts_book.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import date
 from collections import UserDict
 import pickle
-from datehelper import DateHelper
+
+from src.date_helpers import DateHelper
 
 
 def is_weekend_day(day: int) -> bool:
     """
     Checks if a given day is a weekend.
 
     Args:
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/datehelper.py` & `contacts_assistant-0.0.6/src/date_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 This module provides helper functions for date manipulation,
 including formatting workdays and calculating the next birthday.
 """
 
 from datetime import date as dt_date
 from datetime import timedelta
-from constants import DATE_FORMAT
+
+from src.constants import DATE_FORMAT
 
 
 class DateHelper:
     """
     A helper class for date-related operations.
     """
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/handler.py` & `contacts_assistant-0.0.6/src/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Handler module"""
 
-from address import AddressType
-from command_completer import CommandCompleter
-from constants import GREETING_BANNER, CONTACTS_BOOK_FILENAME, NOTEBOOK_FILENAME
-from menu import Menu
-from utils import format_greeting
-from contactsBook import ContactsBook
-from Record import Record
-from notebook import Notebook
-from note import Note
+from src.address import AddressType
+from src.command_completer import CommandCompleter
+from src.constants import GREETING_BANNER, CONTACTS_BOOK_FILENAME, NOTEBOOK_FILENAME
+from src.menu import Menu
+from src.utils import format_greeting
+from src.contacts_book import ContactsBook
+from src.record import Record
+from src.notebook import Notebook
+from src.note import Note
 
 NOT_FOUND_MESSAGE = "Contact does not exist, you can add it"
 
 
 def handle_error(func):
     """
     Decorator to handle exceptions in the wrapped function.
@@ -49,15 +49,14 @@
         if not self.contact_book:
             self.contact_book = ContactsBook()
 
         self.completer = CommandCompleter(
             Menu.get_commands_witn_args(), self.contact_book
         )
 
-
     def greeting(self) -> str:
         """Print greeting message"""
         res = f"{format_greeting(GREETING_BANNER)}\n"
         res += f"Welcome to the assistant bot!\n{Menu.pretty_print()}"
         return res
 
     def hello(self) -> str:
@@ -94,15 +93,15 @@
             record.add_email(email)
         if birthday:
             record.add_birthday(birthday)
 
         return message
 
     @handle_error
-    def update_contact(self, args):
+    def update_phone(self, args):
         """
         Change the phone number of an existing contact.
 
         Args:
             args (Namespace): Namespace containing name, old phone number, and new phone number.
             book (ContactsBook): The address book containing the contact.
 
@@ -282,55 +281,60 @@
         Args:
             args (Namespace): Namespace containing the (name, phone, or email) of the contact.
             search_by (str): The type of search ('name', 'phone', 'email')
 
         Returns:
             str or Record: The contact's record or a message indicating the contact was not found.
         """
-        if search_by == 'name':
+        if search_by == "name":
             record = self.contact_book.find_by_name(args.name)
-        elif search_by == 'phone':
+        elif search_by == "phone":
             record = self.contact_book.find_by_phone(args.phone)
-        elif search_by == 'email':
+        elif search_by == "email":
             record = self.contact_book.find_by_email(args.email)
         else:
             return "Invalid search type specified"
-            
+
         if record is None:
             return NOT_FOUND_MESSAGE
         return record
 
     @handle_error
     def get_contact_by_name(self, args):
         return self.get_contact(args, "name")
 
     @handle_error
     def get_contact_by_phone(self, args):
-        return self.get_contact(args,  "phone")
+        return self.get_contact(args, "phone")
 
     @handle_error
     def get_contact_by_email(self, args):
         return self.get_contact(args, "email")
-    
+
     @handle_error
     def add_note(self, args):
         """
         Add a note to the notebook via user prompt.
 
         Returns:
             str: Message indicating whether the note was added or not.
         """
         title = input("Enter title: ")
         content = input("Enter content: ")
         tags = input("Enter tags (comma-separated): ").split(",")
         due_date = input("Enter due date (DD.MM.YYYY, optional): ").strip()
         due_date = due_date if due_date else None
-        note = Note(title=title, content=content, tags=[tag.strip() for tag in tags], due_date=due_date)
+        note = Note(
+            title=title,
+            content=content,
+            tags=[tag.strip() for tag in tags],
+            due_date=due_date,
+        )
         return self.notebook.add(note)
-    
+
     @handle_error
     def find_note(self, args):
         """
         Find and Show the details of a note.
         Args:
             args (Namespace): Namespace containing the title of the note.
         Returns:
@@ -339,39 +343,39 @@
 
         title = args.title
         notes = self.notebook.search(title)
         if notes:
             return self.notebook.format_notes_with_frame(notes)
         else:
             return f"Note {title} not found."
-        
+
     @handle_error
     def delete_note(self, args):
         """
         Delete a note from the notebook.
         Args:
             args (Namespace): Namespace containing the title of the note.
         Returns:
             str: Message indicating whether the note was deleted or not.
         """
 
         return self.notebook.remove(args.title)
-    
+
     @handle_error
     def delete_all_notes(self, args):
         """
         Delete all notes from the notebook.
         Args:
             args (Namespace): Namespace of arguments.
             notebook (Notebook): The notebook containing the notes.
         Returns:
             str: Message indicating whether the notes were deleted or not.
         """
         return self.notebook.remove_all()
-    
+
     @handle_error
     def update_note_prompt(self, args):
         """
         Update a note by title in the notebook via user prompt.
         Args:
             args (Namespace): Namespace containing the title of the note.
         Returns:
@@ -379,17 +383,22 @@
         """
 
         title = args.title
         content = input("Enter new content: ")
         tags = input("Enter new tags (comma-separated): ").split(",")
         due_date = input("Enter new due date (DD.MM.YYYY, optional): ").strip()
         due_date = due_date if due_date else None
-        new_note = Note(title=title, content=content, tags=[tag.strip() for tag in tags], due_date=due_date)
+        new_note = Note(
+            title=title,
+            content=content,
+            tags=[tag.strip() for tag in tags],
+            due_date=due_date,
+        )
         return self.notebook.update(title, new_note)
-    
+
     @handle_error
     def search_notes(self, args):
         """
         Search for notes containing the query in their title or content.
         Args:
             args (Namespace): Namespace containing the search query.
         Returns:
@@ -398,15 +407,15 @@
 
         query = args.query
         results = self.notebook.search(query)
         if results:
             return self.notebook.format_notes_with_frame(results)
         else:
             return f"No notes found containing '{query}'."
-        
+
     @handle_error
     def filter_notes(self, args):
         """
         Filter notes by tag.
         Args:
             args (Namespace): Namespace containing the tag to filter by.
         Returns:
@@ -415,15 +424,15 @@
 
         tag = args.tag
         results = self.notebook.filter_by_tag(tag)
         if results:
             return self.notebook.format_notes_with_frame(results)
         else:
             return f"No notes found with tag '{tag}'."
-        
+
     @handle_error
     def get_notes_in_days(self, args):
         """
         Get notes that are due in the next specified number of days.
         Args:
             args (Namespace): Namespace containing the number of days to look ahead.
         Returns:
@@ -432,15 +441,15 @@
 
         days = int(args.days)
         results = self.notebook.notes_due_in_days(days)
         if results:
             return self.notebook.format_notes_with_frame(results)
         else:
             return f"No notes due in the next {days} days."
-        
+
     @handle_error
     def print_all_notes(self, args):
         """
         Print all notes in the notebook.
         Returns:
             str: String representation of all notes.
         """
@@ -453,41 +462,41 @@
 
         return "Good bye!"
 
     def __compliance_list(self) -> dict:
         """Return fuction list"""
         return {
             Menu.ADD_CONTACT: self.add_contact,
-            Menu.UPDATE_CONTACT: self.update_contact,
+            Menu.UPDATE_PHONE: self.update_phone,
             Menu.DELETE_CONTACT: self.delete_contact,
-            Menu.SET_CONTACT_BIRTHDAY: self.set_contact_birthday,
-            Menu.GET_CONTACT_BIRTHDAY: self.get_contact_birthday,
-            Menu.GET_CONTACT_BY_NAME: self.get_contact_by_name,
-            Menu.GET_CONTACT_BY_PHONE: self.get_contact_by_phone,
-            Menu.GET_CONTACT_BY_EMAIL: self.get_contact_by_email,
-            Menu.GET_UPCOMING_BIRTHDAYS: self.get_upcoming_birthdays,
-            Menu.UPDATE_CONTACT_EMAIL: self.update_contact_email,
+            Menu.SET_BIRTHDAY: self.set_contact_birthday,
+            Menu.SHOW_BIRTHDAY: self.get_contact_birthday,
+            Menu.FIND_CONTACT_BY_NAME: self.get_contact_by_name,
+            Menu.FIND_CONTACT_BY_PHONE: self.get_contact_by_phone,
+            Menu.FIND_CONTACT_BY_EMAIL: self.get_contact_by_email,
+            Menu.UPCOMING_BIRTHDAYS: self.get_upcoming_birthdays,
+            Menu.UPDATE_EMAIL: self.update_contact_email,
             Menu.ADD_ADDRESS: self.add_address,
-            Menu.DELETE_ADDRESS: self.remove_address,
+            Menu.REMOVE_ADDRESS: self.remove_address,
             Menu.ADD_NOTE: self.add_note,
             Menu.FIND_NOTE: self.find_note,
             Menu.DELETE_NOTE: self.delete_note,
             Menu.DELETE_ALL_NOTES: self.delete_all_notes,
             Menu.UPDATE_NOTE: self.update_note_prompt,
             Menu.SEARCH_NOTES: self.search_notes,
             Menu.FILTER_NOTES_BY_TAG: self.filter_notes,
-            Menu.GET_NOTES_IN_DAYS: self.get_notes_in_days,
-            Menu.GET_ALL_NOTES: self.print_all_notes
+            Menu.NOTES_DUE_IN_DAYS: self.get_notes_in_days,
+            Menu.SHOW_ALL_NOTES: self.print_all_notes,
         }
 
     def __without_params_commands(self) -> dict:
         """Return fuction list"""
         return {
-            Menu.HELLO: self.hello,
-            Menu.GET_ALL_CONTACTS: self.contact_book.__str__,
+            Menu.SHOW_COMMANDS: self.hello,
+            Menu.SHOW_ALL_CONTACTS: self.contact_book.__str__,
             Menu.EXIT: self.close,
             Menu.CLOSE: self.close,
         }
 
     @handle_error
     def execute(self, command, args: list) -> str:
         """
@@ -499,11 +508,14 @@
 
         Returns:
             str: Result message of the handle function execution.
         """
         if command is None:
             return ""
 
+        if len(command.value.param_list) != 0 and args is None:
+            return ""
+
         if command in self.__without_params_commands():
             return self.__without_params_commands().get(command)()
-        else:
-            return self.__compliance_list().get(command)(args)
+
+        return self.__compliance_list().get(command)(args)
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/menu.py` & `contacts_assistant-0.0.6/src/menu.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,134 +1,176 @@
 """Class Menu module"""
 
 import difflib
 import argparse
 from enum import Enum
 from collections import namedtuple
-from constants import MENU_BORDER
-from utils import format_cmd, format_param
+
+from src.constants import MENU_BORDER
+from src.utils import format_cmd, format_param
 
 Command = namedtuple("Command", ["min_required_params", "param_list", "hint"])
 Parametr = namedtuple(
     "Parametr",
     ["name", "required", "hint", "choices"],
     defaults=(None, False, None, None),
 )
 
 
 class Menu(Enum):
     """Class"""
 
-    HELLO = Command(0, [], "to show command list")
+    SHOW_COMMANDS = Command(0, [], "Show the list of available commands")
+
     ADD_CONTACT = Command(
         2,
         [
-            Parametr("name", True, "contact name"),
-            Parametr("phone", True, "contact phone number in format XXXXXXXXXX"),
-            Parametr("email", False, "contact email address"),
-            Parametr("birthday", False, "contact birthday"),
+            Parametr("name", True, "Name of the contact"),
+            Parametr("phone", True, "Phone number of the contact (format: XXXXXXXXXX)"),
+            Parametr("email", False, "Email address of the contact"),
+            Parametr("birthday", False, "Birthday of the contact"),
         ],
-        "to add a new contact",
+        "Add a new contact or update an existing contact",
     )
-    UPDATE_CONTACT = Command(
+
+    UPDATE_PHONE = Command(
         3,
         [
-            Parametr("name", True, "contact name"),
-            Parametr("oldphone", True, "old phone number"),
-            Parametr("newphone", True, "new phone number in format XXXXXXXXXX"),
+            Parametr("name", True, "Name of the contact"),
+            Parametr("oldphone", True, "Old phone number"),
+            Parametr("newphone", True, "New phone number (format: XXXXXXXXXX)"),
         ],
-        "to update a phone",
+        "Update the phone number of a contact",
     )
+
     DELETE_CONTACT = Command(
-        1, [Parametr("name", True, "contact name")], "to delete contact"
+        1, [Parametr("name", True, "Name of the contact")], "Delete a contact"
     )
-    SET_CONTACT_BIRTHDAY = Command(
+
+    SET_BIRTHDAY = Command(
         2,
         [
-            Parametr("name", True, "contact name"),
-            Parametr("birthday", True, "contact birthday"),
+            Parametr("name", True, "Name of the contact"),
+            Parametr("birthday", True, "Birthday of the contact"),
         ],
-        "to set birthday",
+        "Set the birthday of a contact",
     )
 
-    GET_CONTACT_BIRTHDAY = Command(
-        1, [Parametr("name", True, "contact name")], "to show birthday"
+    SHOW_BIRTHDAY = Command(
+        1,
+        [Parametr("name", True, "Name of the contact")],
+        "Show the birthday of a contact",
     )
-    GET_CONTACT_BY_NAME = Command(
-        1, [Parametr("name", True, "contact name")], "to find a contact by name"
+
+    FIND_CONTACT_BY_NAME = Command(
+        1, [Parametr("name", True, "Name of the contact")], "Find a contact by name"
     )
-    GET_CONTACT_BY_PHONE = Command(
+
+    FIND_CONTACT_BY_PHONE = Command(
         1,
-        [Parametr("phone", True, "phone number")],
-        'text": "to find a contact by phone',
+        [Parametr("phone", True, "Phone number of the contact")],
+        "Find a contact by phone number",
     )
-    GET_CONTACT_BY_EMAIL = Command(
+
+    FIND_CONTACT_BY_EMAIL = Command(
         1,
-        [Parametr("email", True, "email address")],
-        'text": "to find a contact by email',
+        [Parametr("email", True, "Email address of the contact")],
+        "Find a contact by email address",
     )
-    GET_ALL_CONTACTS = Command(0, [], "to view a full contact list")
-    GET_UPCOMING_BIRTHDAYS = Command(
+
+    SHOW_ALL_CONTACTS = Command(0, [], "Show all contacts")
+
+    UPCOMING_BIRTHDAYS = Command(
         0,
         [
             Parametr(
-                "days", False, "The number of days to look ahead for upcoming birthdays"
+                "days", False, "Number of days to look ahead for upcoming birthdays"
             )
         ],
-        "Get a list of upcoming birthdays within the specified number of days.",
+        "Show upcoming birthdays within the specified number of days",
     )
-    UPDATE_CONTACT_EMAIL = Command(
+
+    UPDATE_EMAIL = Command(
         2,
         [
-            Parametr("name", True, "contact name"),
-            Parametr("email", True, "email address"),
+            Parametr("name", True, "Name of the contact"),
+            Parametr("email", True, "New email address of the contact"),
         ],
-        "to update email",
+        "Update the email address of a contact",
     )
+
     ADD_ADDRESS = Command(
         2,
         [
-            Parametr("name", True, "contact name"),
+            Parametr("name", True, "Name of the contact"),
             Parametr(
                 "addresstype",
                 False,
-                "address type (Home,Work,Other)",
+                "Type of address (Home, Work, Other)",
                 ["Home", "Work", "Other"],
             ),
-            Parametr("street", False, "street"),
-            Parametr("city", False, "street"),
-            Parametr("postalcode", False, "street"),
-            Parametr("country", False, "street"),
+            Parametr("street", False, "Street address"),
+            Parametr("city", False, "City"),
+            Parametr("postalcode", False, "Postal code"),
+            Parametr("country", False, "Country"),
         ],
-        "add or edit contact address",
+        "Add or update the address of a contact",
     )
-    DELETE_ADDRESS = Command(
+
+    REMOVE_ADDRESS = Command(
         2,
         [
-            Parametr("name", True, "contact name"),
+            Parametr("name", True, "Name of the contact"),
             Parametr(
                 "addresstype",
                 False,
-                "address type (Home,Work,Other)",
+                "Type of address (Home, Work, Other)",
                 ["Home", "Work", "Other"],
             ),
         ],
-        "remove the contact address",
+        "Remove the address of a contact",
+    )
+
+    ADD_NOTE = Command(0, [], "Add a new note")
+
+    FIND_NOTE = Command(
+        1, [Parametr("title", True, "Title of the note")], "Find a note by title"
     )
-    ADD_NOTE = Command(0, [], "to add note")
-    FIND_NOTE = Command(1, [Parametr("title", True, "note title")], "to find note by title")
-    DELETE_NOTE = Command(1, [Parametr("title", True, "note title")], "to delete note")
-    DELETE_ALL_NOTES = Command(0, [], "to delete all notes")
-    UPDATE_NOTE = Command(1, [Parametr("title", True, "note title")], "to update note by title")
-    SEARCH_NOTES = Command(1, [Parametr("query", True, "search query")], "Search for notes containing the query in their title or content.")
-    FILTER_NOTES_BY_TAG = Command(1, [Parametr("tag", True, "tag to filer")], "Filter notes by tag.")
-    GET_NOTES_IN_DAYS = Command(1, [Parametr("days", True, "note subject")], "Get notes that are due in the next specified number of days.",)
-    GET_ALL_NOTES = Command(0, [], "to view a full notes list")
-    EXIT = Command(0, [], "to app close")
-    CLOSE = Command(0, [], "to close application")
+
+    DELETE_NOTE = Command(
+        1, [Parametr("title", True, "Title of the note")], "Delete a note"
+    )
+
+    DELETE_ALL_NOTES = Command(0, [], "Delete all notes")
+
+    UPDATE_NOTE = Command(
+        1, [Parametr("title", True, "Title of the note")], "Update a note by title"
+    )
+
+    SEARCH_NOTES = Command(
+        1,
+        [Parametr("query", True, "Search query")],
+        "Search for notes containing the query in their title or content",
+    )
+
+    FILTER_NOTES_BY_TAG = Command(
+        1, [Parametr("tag", True, "Tag to filter notes by")], "Filter notes by tag"
+    )
+
+    NOTES_DUE_IN_DAYS = Command(
+        1,
+        [Parametr("days", True, "Number of days to look ahead for due notes")],
+        "Show notes that are due within the next specified number of days",
+    )
+
+    SHOW_ALL_NOTES = Command(0, [], "Show all notes")
+
+    EXIT = Command(0, [], "Exit the application")
+
+    CLOSE = Command(0, [], "Close the application")
 
     @classmethod
     def pretty_print(cls):
         """Print all menu items"""
         res = ""
         res += MENU_BORDER
         for k, v in {x.name.lower(): x.value for x in cls}.items():
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/note.py` & `contacts_assistant-0.0.6/src/note.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 from datetime import datetime
-from constants import DATE_FORMAT
+
+from src.constants import DATE_FORMAT
 
 class Note:
     def __init__(self, title, content, tags=None, due_date=None):
         """
         Initialize a Note instance.
 
         Args:
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/notebook.py` & `contacts_assistant-0.0.6/src/notebook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 from datetime import datetime, timedelta
-from note import Note
+
+from src.note import Note
 
 class Notebook:
     def __init__(self):
         """
         Initialize a Notebook instance.
         """
         self.notes = []
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant/utils.py` & `contacts_assistant-0.0.6/src/utils.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant.egg-info/PKG-INFO` & `contacts_assistant-0.0.6/src/contacts_assistant.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contacts_assistant
-Version: 0.0.5
+Version: 0.0.6
 Summary: Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.
 Home-page: https://github.com/Bignichok/Python-ContactsAssistant
 Author: Mykyta Samoilenko
 Author-email: inikita546@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,93 +39,93 @@
   - *Save the current state and stop the bot assistant*
   - **Arguments**: None
 
 - **"add_contact"**: 
   - *Add a contact to the address book or update an existing contact*
   - **Arguments**: `name`, `phone`, `email`, `birthday`
 
-- **"update_contact"**: 
+- **"update_phone"**: 
   - *Change the phone number of an existing contact*
   - **Arguments**: `name`, `oldphone`, `newphone`
 
 - **"delete_contact"**: 
   - *Delete contact by name*
   - **Arguments**: `name`
 
-- **"set_contact_birthday"**: 
+- **"set_birthday"**: 
   - *Add a birthday to a contact*
   - **Arguments**: `name`, `date %d.%m.%Y`
 
-- **"get_contact_birthday"**: 
+- **"show_birthday"**: 
   - *Show the birthday of a contact*
   - **Arguments**: `name`
 
-- **"get_contact_by_name"**: 
+- **"find_contact_by_name"**: 
   - *Find contact by name*
   - **Arguments**: `name`
 
-- **"get_contact_by_phone"**: 
+- **"find_contact_by_phone"**: 
   - *Find contact by phone*
   - **Arguments**: `phone`
 
-- **"get_contact_by_email"**: 
+- **"find_contact_by_email"**: 
   - *Find contact by email*
   - **Arguments**: `email`
 
-- **"get_all_contacts"**: 
+- **"show_all_contacts"**: 
   - *Returns a string representation of the address book*
   - **Arguments**: None
 
-- **"get_upcoming_birthdays"**: 
-  - *Returns a list of upcoming birthdays within the next 7 days*
-  - **Arguments**: None
+- **"upcoming_birthdays"**: 
+  - *Returns a list of upcoming birthdays within the specified number of days*
+  - **Arguments**: `days`
 
-- **"update_contact_email"**: 
+- **"update_email"**: 
   - *Update contact email*
   - **Arguments**: `name`, `email`
 
 - **"add_address"**: 
-  - *Update contact address*
+  - *Add or update the address of a contact*
   - **Arguments**: `name`, `addresstype`, `street`, `city`, `postalcode`, `country`
 
-- **"delete_address"**: 
-  - *Delete contact address*
+- **"remove_address"**: 
+  - *Remove the address of a contact*
   - **Arguments**: `name`, `addresstype`
 
 ### NoteBook
 - **"add_note"**: 
-  - *Add note*
+  - *Add a new note*
   - **Arguments**: None
 
 - **"find_note"**: 
-  - *Find note by title*
+  - *Find a note by title*
   - **Arguments**: `title`
 
 - **"delete_note"**: 
-  - *Delete note by title*
+  - *Delete a note by title*
   - **Arguments**: `title`
 
 - **"delete_all_notes"**: 
-  - *Delete note by title*
+  - *Delete all notes*
   - **Arguments**: None
 
 - **"update_note"**: 
-  - *Update note by title*
+  - *Update a note by title*
   - **Arguments**: `title`
 
 - **"search_notes"**: 
-  - *Search for notes containing the query in their title or content.*
+  - *Search for notes containing the query in their title or content*
   - **Arguments**: `query`
 
 - **"filter_notes_by_tag"**: 
-  - *Filter notes by tag.*
+  - *Filter notes by tag*
   - **Arguments**: `tag`
 
-- **"get_notes_in_days"**: 
-  - *Get notes that are due in the next specified number of days.*
+- **"notes_due_in_days"**: 
+  - *Show notes that are due within the next specified number of days*
   - **Arguments**: `days`
 
-- **"get_all_notes"**: 
-  - *to view a full notes list*
+- **"show_all_notes"**: 
+  - *Show all notes*
   - **Arguments**: None
 
 These commands help you manage and retrieve contact information and notes efficiently. Use them to keep your contacts book organized and up-to-date.
```

### Comparing `contacts_assistant-0.0.5/src/contacts_assistant.egg-info/SOURCES.txt` & `contacts_assistant-0.0.6/src/contacts_assistant.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 LICENSE
-README.md
 setup.py
-src/contacts_assistant/Birthday.py
-src/contacts_assistant/Email.py
-src/contacts_assistant/Field.py
-src/contacts_assistant/Name.py
-src/contacts_assistant/Phone.py
-src/contacts_assistant/Record.py
-src/contacts_assistant/__init__.py
-src/contacts_assistant/__main__.py
-src/contacts_assistant/address.py
-src/contacts_assistant/command_completer.py
-src/contacts_assistant/constants.py
-src/contacts_assistant/contactsBook.py
-src/contacts_assistant/datehelper.py
-src/contacts_assistant/handler.py
-src/contacts_assistant/menu.py
-src/contacts_assistant/note.py
-src/contacts_assistant/notebook.py
-src/contacts_assistant/utils.py
+src/Email.py
+src/__init__.py
+src/address.py
+src/birthday.py
+src/command_completer.py
+src/constants.py
+src/contacts_book.py
+src/date_helpers.py
+src/field.py
+src/handler.py
+src/menu.py
+src/name.py
+src/note.py
+src/notebook.py
+src/phone.py
+src/record.py
+src/utils.py
 src/contacts_assistant.egg-info/PKG-INFO
 src/contacts_assistant.egg-info/SOURCES.txt
 src/contacts_assistant.egg-info/dependency_links.txt
 src/contacts_assistant.egg-info/entry_points.txt
 src/contacts_assistant.egg-info/requires.txt
 src/contacts_assistant.egg-info/top_level.txt
```

