# Comparing `tmp/people-local-0.0.8.tar.gz` & `tmp/people-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "people-local-0.0.8.tar", last modified: Mon Feb 19 15:38:39 2024, max compression
+gzip compressed data, was "people-local-0.0.9.tar", last modified: Mon Feb 19 15:43:27 2024, max compression
```

## Comparing `people-local-0.0.8.tar` & `people-local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:38:39.773487 people-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-19 15:38:39.773487 people-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-02-19 15:38:16.000000 people-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:38:39.769487 people-local-0.0.8/people_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:38:39.773487 people-local-0.0.8/people_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:38:16.000000 people-local-0.0.8/people_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-02-19 15:38:16.000000 people-local-0.0.8/people_local/src/people.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-19 15:38:16.000000 people-local-0.0.8/people_local/src/people_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:38:39.773487 people-local-0.0.8/people_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-19 15:38:39.000000 people-local-0.0.8/people_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-19 15:38:39.000000 people-local-0.0.8/people_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 15:38:39.000000 people-local-0.0.8/people_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-19 15:38:39.000000 people-local-0.0.8/people_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-19 15:38:39.000000 people-local-0.0.8/people_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-19 15:38:16.000000 people-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 15:38:39.773487 people-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-02-19 15:38:16.000000 people-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:43:27.659336 people-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-19 15:43:27.659336 people-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-02-19 15:42:56.000000 people-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:43:27.651336 people-local-0.0.9/people_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:43:27.659336 people-local-0.0.9/people_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:42:56.000000 people-local-0.0.9/people_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9841 2024-02-19 15:42:56.000000 people-local-0.0.9/people_local/src/people.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-19 15:42:56.000000 people-local-0.0.9/people_local/src/people_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:43:27.659336 people-local-0.0.9/people_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-19 15:43:27.000000 people-local-0.0.9/people_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-19 15:43:27.000000 people-local-0.0.9/people_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 15:43:27.000000 people-local-0.0.9/people_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-19 15:43:27.000000 people-local-0.0.9/people_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-19 15:43:27.000000 people-local-0.0.9/people_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-19 15:42:56.000000 people-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 15:43:27.659336 people-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-02-19 15:42:56.000000 people-local-0.0.9/setup.py
```

### Comparing `people-local-0.0.8/PKG-INFO` & `people-local-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: people-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles people-local Python
 Home-page: https://github.com/circles-zone/people-local-python-package/
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `people-local-0.0.8/README.md` & `people-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `people-local-0.0.8/people_local/src/people.py` & `people-local-0.0.9/people_local/src/people.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,35 +11,35 @@
     object=PeopleLocalConstants.PEOPLE_LOCAL_PYTHON_PACKAGE_CODE_LOGGER_OBJECT)
 
 
 # TODO: When fields such as firstname, lastname, organization, job_title, group_name, city ... contains "?" then is_sure=false
 # TODO Should person, profile, contact and user inherit PeopleLocal or not?
 class PeopleLocal():
     def __init__(self, first_name_original: str = None, last_names_original: list = None,
-                 original_organization_names: list = None, short_organization_names: list = None,
+                 organizations_names_original: list = None, short_organization_names: list = None,
                  email_addresses: list = None, urls: list = None):
         logger.start(
             object={
                 'first_name_original': first_name_original, 'last_names_original': last_names_original,
-                'original_organization_names': original_organization_names,
+                'organizations_names_original': organizations_names_original,
                 'short_organization_names': short_organization_names, 
                 'email_addresses': email_addresses, 'urls': urls}
         )
         self.first_name_original = first_name_original
         self.last_names_original = last_names_original
         self.normalized_first_name = None
         self.normalized_last_names = []
-        self.original_organization_names = original_organization_names or []
+        self.organizations_names_original = organizations_names_original or []
         self.short_organization_names = short_organization_names or []
         self.email_addresses = email_addresses or []
         self.urls = urls or []
         self.__extract_first_name_from_email_address()
         self.__extract_organization_str_from_email_addresses_str()
         self.__extract_organization_strs_from_urls_str()
-        self.__extract_short_organization_names_from_original_organization_names()
+        self.__extract_short_organization_names_from_organizations_names_original()
         self.normalize_names()
         logger.end()
 
     def _process_first_name_str(self, add_people_to_a_group_function, **kwargs) -> str:
         logger.start()
         if not self.normalized_first_name:
             logger.warning(log_message="normalized_first_name is None")
@@ -91,20 +91,20 @@
         # TODO Create a group to the family and add this contact/profile to the group
 
         return results
 
     def _process_organizations_str(self, add_people_to_a_group_function, **kwargs) -> list:
         logger.start()
         results = []
-        for organization_name in self.original_organization_names:
+        for organization_name in self.organizations_names_original:
             try:
                 kwargs['groups'] = [organization_name]
                 # TODO: if there's "Ventures" in the organization name, shall we add
                 # GroupsLocalConstants.VENTURE_CAPITAL_GROUP_ID as parent_group_id
-                # to all groups in self.original_organization_names?
+                # to all groups in self.organizations_names_original?
                 if "Ventures" in organization_name:
                     kwargs['parent_group_id'] = GroupsLocalConstants.VENTURE_CAPITAL_GROUP_ID
                 if "?" in organization_name:
                     kwargs["mapping_data_json"] = {
                         "is_sure": False
                     }
                 result = add_people_to_a_group_function(**kwargs)
@@ -124,27 +124,27 @@
         if self.email_addresses == []:
             logger.warning(log_message="email address is None")
             return []
         for email_address in self.email_addresses:
             domain_part = email_address.split('@')[-1]
             organization_name_parts = domain_part.rsplit('.', 1)[0]
             organization_name = ' '.join(part for part in organization_name_parts.split('.'))
-            self.original_organization_names = self.__append_if_not_exists(
-                lst=self.original_organization_names, item=organization_name.capitalize()
+            self.organizations_names_original = self.__append_if_not_exists(
+                lst=self.organizations_names_original, item=organization_name.capitalize()
             )
-        logger.end(object={'original_organization_names': self.original_organization_names})
+        logger.end(object={'organizations_names_original': self.organizations_names_original})
 
-    #  short_organization_names is original_organization_names without "Ltd", "Inc" ...
-    def __extract_short_organization_names_from_original_organization_names(self):
+    #  short_organization_names is organizations_names_original without "Ltd", "Inc" ...
+    def __extract_short_organization_names_from_organizations_names_original(self):
         logger.start()
-        if self.original_organization_names == []:
-            logger.warning(log_message="original_organization_names is None")
+        if self.organizations_names_original == []:
+            logger.warning(log_message="organizations_names_original is None")
             return []
         short_organization_names = []
-        for organization_name in self.original_organization_names:
+        for organization_name in self.organizations_names_original:
             pattern = re.compile(r'\b(?:Ltd|Inc|Corporation|Corp|LLC|L.L.C.|GmbH|AG|S.A.|SARL)\b\.?', re.IGNORECASE)
             short_organization_name = re.sub(pattern, '', organization_name).strip()
             short_organization_name = re.sub(r',\s*$', '', short_organization_name).strip()
             self.short_organization_names = self.__append_if_not_exists(
                 lst=self.short_organization_names, item=short_organization_name
             )
         logger.end(object={'short_organization_names': short_organization_names})
@@ -156,18 +156,18 @@
             return []
         for url in self.urls:
             if url is None:
                 continue
             stripped_url = url.replace('http://', '').replace('https://', '').replace('www.', '')
             organization_name = stripped_url.split('.')[0]
             organization_name_capitalized = organization_name.capitalize()
-            self.original_organization_names = self.__append_if_not_exists(
-                lst=self.original_organization_names, item=organization_name_capitalized
+            self.organizations_names_original = self.__append_if_not_exists(
+                lst=self.organizations_names_original, item=organization_name_capitalized
             )
-        logger.end(object={'original_organization_names': self.original_organization_names})
+        logger.end(object={'organizations_names_original': self.organizations_names_original})
 
     def __extract_first_name_from_email_address(self):
         logger.start()
         if self.email_addresses == []:
             logger.warning(log_message="email addresses are empty")
             return []
         email_address = self.email_addresses[0]
```

### Comparing `people-local-0.0.8/people_local/src/people_constants.py` & `people-local-0.0.9/people_local/src/people_constants.py`

 * *Files identical despite different names*

### Comparing `people-local-0.0.8/people_local.egg-info/PKG-INFO` & `people-local-0.0.9/people_local.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: people-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles people-local Python
 Home-page: https://github.com/circles-zone/people-local-python-package/
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `people-local-0.0.8/setup.py` & `people-local-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "people-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # update only the minor version each time # https://pypi.org/project/people-local
+    version='0.0.9',  # update only the minor version each time # https://pypi.org/project/people-local
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles people-local Python",
     long_description="PyPI Package for Circles people-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/people-local-python-package/",
     packages=[package_dir],
```

