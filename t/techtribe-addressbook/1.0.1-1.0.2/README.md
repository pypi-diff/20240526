# Comparing `tmp/techtribe_addressbook-1.0.1.tar.gz` & `tmp/techtribe_addressbook-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "techtribe_addressbook-1.0.1.tar", last modified: Sat May 25 18:56:12 2024, max compression
+gzip compressed data, was "techtribe_addressbook-1.0.2.tar", last modified: Sat May 25 19:29:24 2024, max compression
```

## Comparing `techtribe_addressbook-1.0.1.tar` & `techtribe_addressbook-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,32 @@
-drwxr-xr-x   0 graf       (501) staff       (20)        0 2024-05-25 18:56:12.919487 techtribe_addressbook-1.0.1/
--rw-r--r--   0 graf       (501) staff       (20)     1081 2024-05-25 17:12:03.000000 techtribe_addressbook-1.0.1/LICENSE
--rw-r--r--   0 graf       (501) staff       (20)     4109 2024-05-25 18:56:12.919257 techtribe_addressbook-1.0.1/PKG-INFO
--rw-r--r--   0 graf       (501) staff       (20)     2429 2024-05-24 19:04:04.000000 techtribe_addressbook-1.0.1/README.md
--rw-r--r--   0 graf       (501) staff       (20)      647 2024-05-25 18:49:40.000000 techtribe_addressbook-1.0.1/pyproject.toml
--rw-r--r--   0 graf       (501) staff       (20)       38 2024-05-25 18:56:12.919542 techtribe_addressbook-1.0.1/setup.cfg
--rw-r--r--   0 graf       (501) staff       (20)      503 2024-05-25 18:31:43.000000 techtribe_addressbook-1.0.1/setup.py
-drwxr-xr-x   0 graf       (501) staff       (20)        0 2024-05-25 18:56:12.918997 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/
--rw-r--r--   0 graf       (501) staff       (20)     4109 2024-05-25 18:56:12.000000 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/PKG-INFO
--rw-r--r--   0 graf       (501) staff       (20)      313 2024-05-25 18:56:12.000000 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/SOURCES.txt
--rw-r--r--   0 graf       (501) staff       (20)        1 2024-05-25 18:56:12.000000 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/dependency_links.txt
--rw-r--r--   0 graf       (501) staff       (20)       55 2024-05-25 18:56:12.000000 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/entry_points.txt
--rw-r--r--   0 graf       (501) staff       (20)       39 2024-05-25 18:56:12.000000 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/requires.txt
--rw-r--r--   0 graf       (501) staff       (20)        1 2024-05-25 18:56:12.000000 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/top_level.txt
+drwxr-xr-x   0 graf       (501) staff       (20)        0 2024-05-25 19:29:24.357605 techtribe_addressbook-1.0.2/
+-rw-r--r--   0 graf       (501) staff       (20)     1081 2024-05-25 17:12:03.000000 techtribe_addressbook-1.0.2/LICENSE
+-rw-r--r--   0 graf       (501) staff       (20)       25 2024-05-25 19:26:13.000000 techtribe_addressbook-1.0.2/MANIFEST.in
+-rw-r--r--   0 graf       (501) staff       (20)     4058 2024-05-25 19:29:24.357370 techtribe_addressbook-1.0.2/PKG-INFO
+-rw-r--r--   0 graf       (501) staff       (20)     2429 2024-05-24 19:04:04.000000 techtribe_addressbook-1.0.2/README.md
+drwxr-xr-x   0 graf       (501) staff       (20)        0 2024-05-25 19:29:24.353195 techtribe_addressbook-1.0.2/TechTribe/
+-rw-r--r--   0 graf       (501) staff       (20)      496 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/decorator.py
+drwxr-xr-x   0 graf       (501) staff       (20)        0 2024-05-25 19:29:24.354577 techtribe_addressbook-1.0.2/TechTribe/dialogs/
+-rw-r--r--   0 graf       (501) staff       (20)      136 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/dialogs/__init__.py
+-rw-r--r--   0 graf       (501) staff       (20)     1296 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/dialogs/ask_command_dialog.py
+-rw-r--r--   0 graf       (501) staff       (20)      407 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/dialogs/ask_dialog_usage.py
+-rw-r--r--   0 graf       (501) staff       (20)      370 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/dialogs/print_text.py
+-rw-r--r--   0 graf       (501) staff       (20)     8729 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/handlers.py
+-rw-r--r--   0 graf       (501) staff       (20)     5114 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/main.py
+drwxr-xr-x   0 graf       (501) staff       (20)        0 2024-05-25 19:29:24.356132 techtribe_addressbook-1.0.2/TechTribe/models/
+-rw-r--r--   0 graf       (501) staff       (20)      162 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/models/__init__.py
+-rw-r--r--   0 graf       (501) staff       (20)     7164 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/models/address_book.py
+-rw-r--r--   0 graf       (501) staff       (20)      381 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/models/colors.py
+-rw-r--r--   0 graf       (501) staff       (20)    10798 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/models/commands.py
+-rw-r--r--   0 graf       (501) staff       (20)      386 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/models/field.py
+-rw-r--r--   0 graf       (501) staff       (20)     3108 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/models/fields.py
+-rw-r--r--   0 graf       (501) staff       (20)     3192 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.2/TechTribe/models/record.py
+-rw-r--r--   0 graf       (501) staff       (20)      647 2024-05-25 19:24:05.000000 techtribe_addressbook-1.0.2/pyproject.toml
+-rw-r--r--   0 graf       (501) staff       (20)       38 2024-05-25 19:29:24.357650 techtribe_addressbook-1.0.2/setup.cfg
+-rw-r--r--   0 graf       (501) staff       (20)       38 2024-05-25 19:23:04.000000 techtribe_addressbook-1.0.2/setup.py
+drwxr-xr-x   0 graf       (501) staff       (20)        0 2024-05-25 19:29:24.357097 techtribe_addressbook-1.0.2/techtribe_addressbook.egg-info/
+-rw-r--r--   0 graf       (501) staff       (20)     4058 2024-05-25 19:29:24.000000 techtribe_addressbook-1.0.2/techtribe_addressbook.egg-info/PKG-INFO
+-rw-r--r--   0 graf       (501) staff       (20)      726 2024-05-25 19:29:24.000000 techtribe_addressbook-1.0.2/techtribe_addressbook.egg-info/SOURCES.txt
+-rw-r--r--   0 graf       (501) staff       (20)        1 2024-05-25 19:29:24.000000 techtribe_addressbook-1.0.2/techtribe_addressbook.egg-info/dependency_links.txt
+-rw-r--r--   0 graf       (501) staff       (20)       55 2024-05-25 19:29:24.000000 techtribe_addressbook-1.0.2/techtribe_addressbook.egg-info/entry_points.txt
+-rw-r--r--   0 graf       (501) staff       (20)       39 2024-05-25 19:29:24.000000 techtribe_addressbook-1.0.2/techtribe_addressbook.egg-info/requires.txt
+-rw-r--r--   0 graf       (501) staff       (20)       10 2024-05-25 19:29:24.000000 techtribe_addressbook-1.0.2/techtribe_addressbook.egg-info/top_level.txt
```

### Comparing `techtribe_addressbook-1.0.1/LICENSE` & `techtribe_addressbook-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `techtribe_addressbook-1.0.1/PKG-INFO` & `techtribe_addressbook-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: techtribe-addressbook
-Version: 1.0.1
+Version: 1.0.2
 Summary: Save your data easy and convenient
-Home-page: https://github.com/Oldestgraf/TechTribe
 License: The MIT License (MIT)
         Copyright © 2024 TechTribe
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

#### html2text {}

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1 Name: techtribe-addressbook Version: 1.0.1 Summary: Save
-your data easy and convenient Home-page: https://github.com/Oldestgraf/
-TechTribe License: The MIT License (MIT) Copyright Â© 2024 TechTribe Permission
-is hereby granted, free of charge, to any person obtaining a copy of this
-software and associated documentation files (the âSoftwareâ), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions: The above copyright notice and this
-permission notice shall be included in all copies or substantial portions of
-the Software. THE SOFTWARE IS PROVIDED âAS ISâ, WITHOUT WARRANTY OF ANY
-KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
-EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
-OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/Oldestgraf/
-TechTribe Keywords: addressbook,techtribe Classifier: License :: OSI Approved
-:: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
-Operating System :: OS Independent Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: prompt-toolkit==3.0.43 Requires-Dist:
-wcwidth==0.2.13 # TechTribe Final project for Python Programming: Foundations
-and Best Practices 2.0 ## Description A terminal application that allows users
-to create, read, update, and delete contacts. Users can also view all contacts,
-view contact by name, and search for contacts by keyword. Also implemented
-opportunity to save notes separate from contacts. User can save, edit, delete
-and search note by title. Also added opportunity to add tags to any note,
-delete tag and find note by tag. ## Installation 1. Clone the repository 2.
-Create a virtual environment in the project directory: python -m venv .venv 3.
-Activate the virtual environment: source .venv/bin/activate 4. Install the
-required packages: pip install -r requirements.txt 5. Run the application:
-python main.py ## Usage Write a command in the terminal to interact with the
-application User can use the next commands: - `add ` to add a new contact -
-`add_birthday ` to add a birthday to a contact - `add_address ` to add an
-address to a contact - `edit_address ` to edit an address for a contact -
-`add_email ` to add an email to a contact - `edit_email ` to edit an email for
-a contact - `remove_email ` to remove an email from a contact - `show_contact `
-to show contact - `find_contacts ` to find contacts by multiple queries -
-`show_birthday ` to show birthday for a contact - `birthdays ` to show the
-upcoming birthdays in the next days, default days is `7` - `change ` to change
-the phone number of a contact - `phone ` to show the phone numbers of a contact
-- `all` to show all contacts - `delete` to delete contact - `delete_all` to
-delete all contacts - `delete_address ` to delete address - `delete_note
+Metadata-Version: 2.1 Name: techtribe-addressbook Version: 1.0.2 Summary: Save
+your data easy and convenient License: The MIT License (MIT) Copyright Â© 2024
+TechTribe Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+âSoftwareâ), to deal in the Software without restriction, including without
+limitation the rights to use, copy, modify, merge, publish, distribute,
+sublicense, and/or sell copies of the Software, and to permit persons to whom
+the Software is furnished to do so, subject to the following conditions: The
+above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED âAS
+ISâ, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
+LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
+AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Homepage,
+https://github.com/Oldestgraf/TechTribe Keywords: addressbook,techtribe
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+prompt-toolkit==3.0.43 Requires-Dist: wcwidth==0.2.13 # TechTribe Final project
+for Python Programming: Foundations and Best Practices 2.0 ## Description A
+terminal application that allows users to create, read, update, and delete
+contacts. Users can also view all contacts, view contact by name, and search
+for contacts by keyword. Also implemented opportunity to save notes separate
+from contacts. User can save, edit, delete and search note by title. Also added
+opportunity to add tags to any note, delete tag and find note by tag. ##
+Installation 1. Clone the repository 2. Create a virtual environment in the
+project directory: python -m venv .venv 3. Activate the virtual environment:
+source .venv/bin/activate 4. Install the required packages: pip install -
+r requirements.txt 5. Run the application: python main.py ## Usage Write a
+command in the terminal to interact with the application User can use the next
+commands: - `add ` to add a new contact - `add_birthday ` to add a birthday to
+a contact - `add_address ` to add an address to a contact - `edit_address ` to
+edit an address for a contact - `add_email ` to add an email to a contact -
+`edit_email ` to edit an email for a contact - `remove_email ` to remove an
+email from a contact - `show_contact ` to show contact - `find_contacts ` to
+find contacts by multiple queries - `show_birthday ` to show birthday for a
+contact - `birthdays ` to show the upcoming birthdays in the next days, default
+days is `7` - `change ` to change the phone number of a contact - `phone ` to
+show the phone numbers of a contact - `all` to show all contacts - `delete` to
+delete contact - `delete_all` to delete all contacts - `delete_address ` to
+delete address - `delete_note
```

### Comparing `techtribe_addressbook-1.0.1/README.md` & `techtribe_addressbook-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `techtribe_addressbook-1.0.1/pyproject.toml` & `techtribe_addressbook-1.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "techtribe-addressbook"
-version = "1.0.1"
+version = "1.0.2"
 description = "Save your data easy and convenient"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

### Comparing `techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/PKG-INFO` & `techtribe_addressbook-1.0.2/techtribe_addressbook.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: techtribe-addressbook
-Version: 1.0.1
+Version: 1.0.2
 Summary: Save your data easy and convenient
-Home-page: https://github.com/Oldestgraf/TechTribe
 License: The MIT License (MIT)
         Copyright © 2024 TechTribe
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

#### html2text {}

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1 Name: techtribe-addressbook Version: 1.0.1 Summary: Save
-your data easy and convenient Home-page: https://github.com/Oldestgraf/
-TechTribe License: The MIT License (MIT) Copyright Â© 2024 TechTribe Permission
-is hereby granted, free of charge, to any person obtaining a copy of this
-software and associated documentation files (the âSoftwareâ), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions: The above copyright notice and this
-permission notice shall be included in all copies or substantial portions of
-the Software. THE SOFTWARE IS PROVIDED âAS ISâ, WITHOUT WARRANTY OF ANY
-KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
-EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
-OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/Oldestgraf/
-TechTribe Keywords: addressbook,techtribe Classifier: License :: OSI Approved
-:: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
-Operating System :: OS Independent Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: prompt-toolkit==3.0.43 Requires-Dist:
-wcwidth==0.2.13 # TechTribe Final project for Python Programming: Foundations
-and Best Practices 2.0 ## Description A terminal application that allows users
-to create, read, update, and delete contacts. Users can also view all contacts,
-view contact by name, and search for contacts by keyword. Also implemented
-opportunity to save notes separate from contacts. User can save, edit, delete
-and search note by title. Also added opportunity to add tags to any note,
-delete tag and find note by tag. ## Installation 1. Clone the repository 2.
-Create a virtual environment in the project directory: python -m venv .venv 3.
-Activate the virtual environment: source .venv/bin/activate 4. Install the
-required packages: pip install -r requirements.txt 5. Run the application:
-python main.py ## Usage Write a command in the terminal to interact with the
-application User can use the next commands: - `add ` to add a new contact -
-`add_birthday ` to add a birthday to a contact - `add_address ` to add an
-address to a contact - `edit_address ` to edit an address for a contact -
-`add_email ` to add an email to a contact - `edit_email ` to edit an email for
-a contact - `remove_email ` to remove an email from a contact - `show_contact `
-to show contact - `find_contacts ` to find contacts by multiple queries -
-`show_birthday ` to show birthday for a contact - `birthdays ` to show the
-upcoming birthdays in the next days, default days is `7` - `change ` to change
-the phone number of a contact - `phone ` to show the phone numbers of a contact
-- `all` to show all contacts - `delete` to delete contact - `delete_all` to
-delete all contacts - `delete_address ` to delete address - `delete_note
+Metadata-Version: 2.1 Name: techtribe-addressbook Version: 1.0.2 Summary: Save
+your data easy and convenient License: The MIT License (MIT) Copyright Â© 2024
+TechTribe Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+âSoftwareâ), to deal in the Software without restriction, including without
+limitation the rights to use, copy, modify, merge, publish, distribute,
+sublicense, and/or sell copies of the Software, and to permit persons to whom
+the Software is furnished to do so, subject to the following conditions: The
+above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED âAS
+ISâ, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
+LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
+AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Homepage,
+https://github.com/Oldestgraf/TechTribe Keywords: addressbook,techtribe
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+prompt-toolkit==3.0.43 Requires-Dist: wcwidth==0.2.13 # TechTribe Final project
+for Python Programming: Foundations and Best Practices 2.0 ## Description A
+terminal application that allows users to create, read, update, and delete
+contacts. Users can also view all contacts, view contact by name, and search
+for contacts by keyword. Also implemented opportunity to save notes separate
+from contacts. User can save, edit, delete and search note by title. Also added
+opportunity to add tags to any note, delete tag and find note by tag. ##
+Installation 1. Clone the repository 2. Create a virtual environment in the
+project directory: python -m venv .venv 3. Activate the virtual environment:
+source .venv/bin/activate 4. Install the required packages: pip install -
+r requirements.txt 5. Run the application: python main.py ## Usage Write a
+command in the terminal to interact with the application User can use the next
+commands: - `add ` to add a new contact - `add_birthday ` to add a birthday to
+a contact - `add_address ` to add an address to a contact - `edit_address ` to
+edit an address for a contact - `add_email ` to add an email to a contact -
+`edit_email ` to edit an email for a contact - `remove_email ` to remove an
+email from a contact - `show_contact ` to show contact - `find_contacts ` to
+find contacts by multiple queries - `show_birthday ` to show birthday for a
+contact - `birthdays ` to show the upcoming birthdays in the next days, default
+days is `7` - `change ` to change the phone number of a contact - `phone ` to
+show the phone numbers of a contact - `all` to show all contacts - `delete` to
+delete contact - `delete_all` to delete all contacts - `delete_address ` to
+delete address - `delete_note
```

