# Comparing `tmp/contacts_assistant-0.0.7.tar.gz` & `tmp/contacts_assistant-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contacts_assistant-0.0.7.tar", last modified: Sun May 26 14:14:31 2024, max compression
+gzip compressed data, was "contacts_assistant-0.0.8.tar", last modified: Sun May 26 14:18:24 2024, max compression
```

## Comparing `contacts_assistant-0.0.7.tar` & `contacts_assistant-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 14:14:31.566201 contacts_assistant-0.0.7/
--rw-rw-rw-   0        0        0     1095 2024-05-22 08:53:23.000000 contacts_assistant-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     4406 2024-05-26 14:14:31.565201 contacts_assistant-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-26 14:14:31.566201 contacts_assistant-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1518 2024-05-26 14:14:22.000000 contacts_assistant-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:14:31.550203 contacts_assistant-0.0.7/src/
--rw-rw-rw-   0        0        0     1219 2024-05-26 09:46:28.000000 contacts_assistant-0.0.7/src/Email.py
--rw-rw-rw-   0        0        0        0 2024-05-26 09:34:04.000000 contacts_assistant-0.0.7/src/__init__.py
--rw-rw-rw-   0        0        0     2144 2024-05-26 09:46:01.000000 contacts_assistant-0.0.7/src/address.py
--rw-rw-rw-   0        0        0     1338 2024-05-26 09:46:13.000000 contacts_assistant-0.0.7/src/birthday.py
--rw-rw-rw-   0        0        0     1199 2024-05-26 09:34:44.000000 contacts_assistant-0.0.7/src/command_completer.py
--rw-rw-rw-   0        0        0      837 2024-05-26 12:09:13.000000 contacts_assistant-0.0.7/src/constants.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:14:31.564202 contacts_assistant-0.0.7/src/contacts_assistant.egg-info/
--rw-rw-rw-   0        0        0     4406 2024-05-26 14:14:31.000000 contacts_assistant-0.0.7/src/contacts_assistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2024-05-26 14:14:31.000000 contacts_assistant-0.0.7/src/contacts_assistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 14:14:31.000000 contacts_assistant-0.0.7/src/contacts_assistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-26 14:14:31.000000 contacts_assistant-0.0.7/src/contacts_assistant.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2024-05-26 14:14:31.000000 contacts_assistant-0.0.7/src/contacts_assistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0      144 2024-05-26 14:14:31.000000 contacts_assistant-0.0.7/src/contacts_assistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8543 2024-05-26 12:07:21.000000 contacts_assistant-0.0.7/src/contacts_book.py
--rw-rw-rw-   0        0        0     1989 2024-05-26 09:46:19.000000 contacts_assistant-0.0.7/src/date_helpers.py
--rw-rw-rw-   0        0        0      853 2024-05-26 09:28:57.000000 contacts_assistant-0.0.7/src/field.py
--rw-rw-rw-   0        0        0    17056 2024-05-26 12:06:31.000000 contacts_assistant-0.0.7/src/handler.py
--rw-rw-rw-   0        0        0     7499 2024-05-26 09:36:07.000000 contacts_assistant-0.0.7/src/menu.py
--rw-rw-rw-   0        0        0      595 2024-05-26 09:46:53.000000 contacts_assistant-0.0.7/src/name.py
--rw-rw-rw-   0        0        0     3286 2024-05-26 09:46:56.000000 contacts_assistant-0.0.7/src/note.py
--rw-rw-rw-   0        0        0     8400 2024-05-26 09:36:23.000000 contacts_assistant-0.0.7/src/notebook.py
--rw-rw-rw-   0        0        0     1508 2024-05-26 09:47:03.000000 contacts_assistant-0.0.7/src/phone.py
--rw-rw-rw-   0        0        0     6518 2024-05-26 09:47:09.000000 contacts_assistant-0.0.7/src/record.py
--rw-rw-rw-   0        0        0      549 2024-05-26 09:28:57.000000 contacts_assistant-0.0.7/src/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:18:24.232776 contacts_assistant-0.0.8/
+-rw-rw-rw-   0        0        0     1095 2024-05-22 08:53:23.000000 contacts_assistant-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     4406 2024-05-26 14:18:24.231778 contacts_assistant-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-26 14:18:24.232776 contacts_assistant-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1523 2024-05-26 14:17:33.000000 contacts_assistant-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:18:24.211776 contacts_assistant-0.0.8/src/
+-rw-rw-rw-   0        0        0     1219 2024-05-26 09:46:28.000000 contacts_assistant-0.0.8/src/Email.py
+-rw-rw-rw-   0        0        0        0 2024-05-26 09:34:04.000000 contacts_assistant-0.0.8/src/__init__.py
+-rw-rw-rw-   0        0        0     2144 2024-05-26 09:46:01.000000 contacts_assistant-0.0.8/src/address.py
+-rw-rw-rw-   0        0        0     1338 2024-05-26 09:46:13.000000 contacts_assistant-0.0.8/src/birthday.py
+-rw-rw-rw-   0        0        0     1199 2024-05-26 09:34:44.000000 contacts_assistant-0.0.8/src/command_completer.py
+-rw-rw-rw-   0        0        0      837 2024-05-26 12:09:13.000000 contacts_assistant-0.0.8/src/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:18:24.231778 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/
+-rw-rw-rw-   0        0        0     4406 2024-05-26 14:18:24.000000 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2024-05-26 14:18:24.000000 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:18:24.000000 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-26 14:18:24.000000 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-05-26 14:18:24.000000 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      144 2024-05-26 14:18:24.000000 contacts_assistant-0.0.8/src/contacts_assistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8543 2024-05-26 12:07:21.000000 contacts_assistant-0.0.8/src/contacts_book.py
+-rw-rw-rw-   0        0        0     1989 2024-05-26 09:46:19.000000 contacts_assistant-0.0.8/src/date_helpers.py
+-rw-rw-rw-   0        0        0      853 2024-05-26 09:28:57.000000 contacts_assistant-0.0.8/src/field.py
+-rw-rw-rw-   0        0        0    17056 2024-05-26 12:06:31.000000 contacts_assistant-0.0.8/src/handler.py
+-rw-rw-rw-   0        0        0     7499 2024-05-26 09:36:07.000000 contacts_assistant-0.0.8/src/menu.py
+-rw-rw-rw-   0        0        0      595 2024-05-26 09:46:53.000000 contacts_assistant-0.0.8/src/name.py
+-rw-rw-rw-   0        0        0     3286 2024-05-26 09:46:56.000000 contacts_assistant-0.0.8/src/note.py
+-rw-rw-rw-   0        0        0     8400 2024-05-26 09:36:23.000000 contacts_assistant-0.0.8/src/notebook.py
+-rw-rw-rw-   0        0        0     1508 2024-05-26 09:47:03.000000 contacts_assistant-0.0.8/src/phone.py
+-rw-rw-rw-   0        0        0     6518 2024-05-26 09:47:09.000000 contacts_assistant-0.0.8/src/record.py
+-rw-rw-rw-   0        0        0      549 2024-05-26 09:28:57.000000 contacts_assistant-0.0.8/src/utils.py
```

### Comparing `contacts_assistant-0.0.7/LICENSE` & `contacts_assistant-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/PKG-INFO` & `contacts_assistant-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contacts_assistant
-Version: 0.0.7
+Version: 0.0.8
 Summary: Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.
 Home-page: https://github.com/Bignichok/Python-ContactsAssistant
 Author: Mykyta Samoilenko
 Author-email: inikita546@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `contacts_assistant-0.0.7/setup.py` & `contacts_assistant-0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     encoding = result['encoding']
 
 with open("requirements.txt", "r", encoding=encoding) as fh:
     requirements = fh.read().splitlines()
 
 setuptools.setup(
     name="contacts_assistant",
-    version="0.0.7",
+    version="0.0.8",
     include_package_data=True,
     author="Mykyta Samoilenko",
     author_email="inikita546@gmail.com",
     description="Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bignichok/Python-ContactsAssistant",
@@ -34,11 +34,11 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
     entry_points={
         'console_scripts': [
-            'contacts_assistant=main'
+            'contacts_assistant=main:main'
         ]
     },
 )
```

### Comparing `contacts_assistant-0.0.7/src/Email.py` & `contacts_assistant-0.0.8/src/Email.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/address.py` & `contacts_assistant-0.0.8/src/address.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/birthday.py` & `contacts_assistant-0.0.8/src/birthday.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/command_completer.py` & `contacts_assistant-0.0.8/src/command_completer.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/constants.py` & `contacts_assistant-0.0.8/src/constants.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/contacts_assistant.egg-info/PKG-INFO` & `contacts_assistant-0.0.8/src/contacts_assistant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contacts_assistant
-Version: 0.0.7
+Version: 0.0.8
 Summary: Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.
 Home-page: https://github.com/Bignichok/Python-ContactsAssistant
 Author: Mykyta Samoilenko
 Author-email: inikita546@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `contacts_assistant-0.0.7/src/contacts_assistant.egg-info/SOURCES.txt` & `contacts_assistant-0.0.8/src/contacts_assistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/contacts_book.py` & `contacts_assistant-0.0.8/src/contacts_book.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/date_helpers.py` & `contacts_assistant-0.0.8/src/date_helpers.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/field.py` & `contacts_assistant-0.0.8/src/field.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/handler.py` & `contacts_assistant-0.0.8/src/handler.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/menu.py` & `contacts_assistant-0.0.8/src/menu.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/name.py` & `contacts_assistant-0.0.8/src/name.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/note.py` & `contacts_assistant-0.0.8/src/note.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/notebook.py` & `contacts_assistant-0.0.8/src/notebook.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/phone.py` & `contacts_assistant-0.0.8/src/phone.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/record.py` & `contacts_assistant-0.0.8/src/record.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.7/src/utils.py` & `contacts_assistant-0.0.8/src/utils.py`

 * *Files identical despite different names*
