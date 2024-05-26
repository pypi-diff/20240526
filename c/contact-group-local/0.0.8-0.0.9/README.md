# Comparing `tmp/contact-group-local-0.0.8.tar.gz` & `tmp/contact-group-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact-group-local-0.0.8.tar", last modified: Wed Jan 24 20:25:11 2024, max compression
+gzip compressed data, was "contact-group-local-0.0.9.tar", last modified: Wed Jan 31 13:57:47 2024, max compression
```

## Comparing `contact-group-local-0.0.8.tar` & `contact-group-local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:25:11.151067 contact-group-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-24 20:25:11.151067 contact-group-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-01-24 20:24:47.000000 contact-group-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:25:11.147066 contact-group-local-0.0.8/contact_group_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:25:11.151067 contact-group-local-0.0.8/contact_group_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 20:24:47.000000 contact-group-local-0.0.8/contact_group_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-01-24 20:24:47.000000 contact-group-local-0.0.8/contact_group_local/src/contact_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-01-24 20:24:47.000000 contact-group-local-0.0.8/contact_group_local/src/contact_group_constans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:25:11.151067 contact-group-local-0.0.8/contact_group_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-24 20:25:11.000000 contact-group-local-0.0.8/contact_group_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-01-24 20:25:11.000000 contact-group-local-0.0.8/contact_group_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 20:25:11.000000 contact-group-local-0.0.8/contact_group_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-24 20:25:11.000000 contact-group-local-0.0.8/contact_group_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-24 20:25:11.000000 contact-group-local-0.0.8/contact_group_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-24 20:24:47.000000 contact-group-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 20:25:11.151067 contact-group-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-01-24 20:24:47.000000 contact-group-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:57:47.915031 contact-group-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-31 13:57:47.915031 contact-group-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-01-31 13:57:24.000000 contact-group-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:57:47.911031 contact-group-local-0.0.9/contact_group_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:57:47.915031 contact-group-local-0.0.9/contact_group_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 13:57:24.000000 contact-group-local-0.0.9/contact_group_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-01-31 13:57:24.000000 contact-group-local-0.0.9/contact_group_local/src/contact_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-01-31 13:57:24.000000 contact-group-local-0.0.9/contact_group_local/src/contact_group_constans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:57:47.915031 contact-group-local-0.0.9/contact_group_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-31 13:57:47.000000 contact-group-local-0.0.9/contact_group_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-01-31 13:57:47.000000 contact-group-local-0.0.9/contact_group_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 13:57:47.000000 contact-group-local-0.0.9/contact_group_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-31 13:57:47.000000 contact-group-local-0.0.9/contact_group_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-31 13:57:47.000000 contact-group-local-0.0.9/contact_group_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-31 13:57:24.000000 contact-group-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 13:57:47.915031 contact-group-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-01-31 13:57:24.000000 contact-group-local-0.0.9/setup.py
```

### Comparing `contact-group-local-0.0.8/PKG-INFO` & `contact-group-local-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-group-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles contact-group-local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact-group-local-0.0.8/README.md` & `contact-group-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `contact-group-local-0.0.8/contact_group_local/src/contact_group.py` & `contact-group-local-0.0.9/contact_group_local/src/contact_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,24 +26,27 @@
 
         super().__init__(default_schema_name=default_schema_name, default_entity_name1=default_entity_name1,
                          default_entity_name2=default_entity_name2, default_id_column_name=default_id_column_name,
                          default_table_name=default_table_name, default_view_table_name=default_view_table_name)
         self.group_remote = GroupsRemote()
 
     def insert_contact_and_link_to_existing_or_new_group(self, contact_dict: dict, contact_id: int,
-                                                         is_test_data: bool = False) -> list[tuple]:
+                                                         groups: list, is_test_data: bool = False) -> list[tuple]:
         logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id, "is_test_data": is_test_data})
 
         # TODO: Shall we also add the arguments is_interest, parent_group_id and title_lang_code?
+        all_groups_linked = []
+        for group in groups:
+            groups_linked = self.add_update_group_and_link_to_contact(entity_name=group,
+                                                                      contact_id=contact_id,
+                                                                      title=group,
+                                                                      is_test_data=self.is_test_data)
+            all_groups_linked.append(groups_linked)
 
-        groups_linked = self.add_update_group_and_link_to_contact(entity_name=contact_dict["organization"],
-                                                                  contact_id=contact_id,
-                                                                  title=contact_dict["organization"],
-                                                                  is_test_data=self.is_test_data)
-        logger.end(object={"groups_linked": groups_linked})
+        logger.end(object={"all_groups_linked": all_groups_linked})
         return groups_linked
 
     def normalize_group_name(self, group_name: str) -> str:
         """
         Normalize group name
         Remove any special characters and spaces from group name and convert it to lowercase
         :param group_name: group name
```

### Comparing `contact-group-local-0.0.8/contact_group_local/src/contact_group_constans.py` & `contact-group-local-0.0.9/contact_group_local/src/contact_group_constans.py`

 * *Files identical despite different names*

### Comparing `contact-group-local-0.0.8/contact_group_local.egg-info/PKG-INFO` & `contact-group-local-0.0.9/contact_group_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-group-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles contact-group-local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact-group-local-0.0.8/pyproject.toml` & `contact-group-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `contact-group-local-0.0.8/setup.py` & `contact-group-local-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # with open('README.md') as f:
 #    readme = f.read()
   
 setuptools.setup(
     # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix).
     # Only lowercase, no underlines.
     name=PACKAGE_NAME,
-    version='0.0.8',  # update only the minor version each time # https://pypi.org/project/contact-group-local
+    version='0.0.9',  # update only the minor version each time # https://pypi.org/project/contact-group-local
     author="Circles",
     author_email="info@circlez.ai",
     # TODO: Please update the description and delete this line
     description="PyPI Package for Circles contact-group-local Python",
     # long_description=open('README.md').read(),
     long_description="",
     long_description_content_type='text/markdown',
```

