# Comparing `tmp/phones_local-0.0.26.tar.gz` & `tmp/phones_local-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones_local-0.0.26.tar", last modified: Thu May 23 11:47:57 2024, max compression
+gzip compressed data, was "phones_local-0.0.27.tar", last modified: Sun May 26 21:32:41 2024, max compression
```

## Comparing `phones_local-0.0.26.tar` & `phones_local-0.0.27.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:57.624759 phones_local-0.0.26/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-23 11:47:57.624759 phones_local-0.0.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-23 11:47:32.000000 phones_local-0.0.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:57.620759 phones_local-0.0.26/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:57.620759 phones_local-0.0.26/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:32.000000 phones_local-0.0.26/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-23 11:47:32.000000 phones_local-0.0.26/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-05-23 11:47:32.000000 phones_local-0.0.26/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:57.620759 phones_local-0.0.26/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-23 11:47:57.000000 phones_local-0.0.26/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-23 11:47:57.000000 phones_local-0.0.26/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:47:57.000000 phones_local-0.0.26/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-23 11:47:57.000000 phones_local-0.0.26/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 11:47:57.000000 phones_local-0.0.26/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-23 11:47:32.000000 phones_local-0.0.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:47:57.624759 phones_local-0.0.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-23 11:47:32.000000 phones_local-0.0.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:32:41.175127 phones_local-0.0.27/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-26 21:32:41.175127 phones_local-0.0.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-26 21:32:13.000000 phones_local-0.0.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:32:41.171127 phones_local-0.0.27/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:32:41.175127 phones_local-0.0.27/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:32:13.000000 phones_local-0.0.27/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-26 21:32:13.000000 phones_local-0.0.27/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-05-26 21:32:13.000000 phones_local-0.0.27/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:32:41.175127 phones_local-0.0.27/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-26 21:32:41.000000 phones_local-0.0.27/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-26 21:32:41.000000 phones_local-0.0.27/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:32:41.000000 phones_local-0.0.27/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-26 21:32:41.000000 phones_local-0.0.27/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 21:32:41.000000 phones_local-0.0.27/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-26 21:32:20.000000 phones_local-0.0.27/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 21:32:41.175127 phones_local-0.0.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 21:32:13.000000 phones_local-0.0.27/setup.py
```

### Comparing `phones_local-0.0.26/PKG-INFO` & `phones_local-0.0.27/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.26
+Version: 0.0.27
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.26/README.md` & `phones_local-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.26/phones_local/src/phone_local_constans.py` & `phones_local-0.0.27/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.26/phones_local/src/phones_local.py` & `phones_local-0.0.27/phones_local/src/phones_local.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,34 +16,34 @@
                          default_table_name="phone_table",
                          default_view_table_name="phone_view",
                          default_column_name="phone_id")
 
     def get_normalized_phone_number_by_phone_id(self, phone_id: int) -> int:
         logger.start(object={"phone_id": phone_id})
         data = self.select_one_dict_by_column_and_value(select_clause_value="local_number_normalized",
-                                          column_value=phone_id)
+                                                        column_value=phone_id)
         if not data:
             logger.end("No phone number found for phone_id " +
                        str(phone_id))
         else:
             phone_number = int(data["local_number_normalized"])
             logger.end("Return Phone Number of a specific phone id",
                        object={'phone_number': phone_number})
             return phone_number  # TODO: should we add area_code?
 
     def verify_phone_number(self, phone_number: int) -> None:
         logger.start(object={"phone_number": phone_number})
         self.update_by_column_and_value(column_value=phone_number,
-                          data_dict={"is_verified": 1})
+                                        data_dict={"is_verified": 1})
         logger.end()
 
     def is_verified(self, phone_number: int) -> bool:
         logger.start(object={"phone_number": phone_number})
         data = self.select_one_dict_by_column_and_value(select_clause_value="is_verified",
-                                          column_value=phone_number)
+                                                        column_value=phone_number)
         if not data:
             logger.end("No phone number found for phone_number " +
                        str(phone_number))
             return False
         is_verified = data["is_verified"]
         logger.end("Return is_verified of a specific phone id",
                    object={'is_verified': is_verified})
@@ -65,18 +65,24 @@
             "full_number_normalized": "+972549338666"
         }
         """
         try:
             parsed_number = parse(original_number, region)
             international_code = parsed_number.country_code
             full_number_normalized = format_number(parsed_number, PhoneNumberFormat.E164)
+            # if full_number_normalized.startswith("+"):
+            #     full_number_normalized = full_number_normalized[1:]
             # parsed_number example: original_number='0687473298' -> PhoneNumber(country_code=972, national_number=687473298, extension=None, italian_leading_zero=None, number_of_leading_zeros=None, country_code_source=0, preferred_domestic_carrier_code=None)
+            # TODO: Shall we add area_code? what shall it be? How can we do it?
+            # TODO Can we move number_info to data member in PhoneLocal class
             number_info = {
+                "number_original": original_number,
                 "international_code": international_code,
                 "full_number_normalized": full_number_normalized,
+                "local_number_normalized": parsed_number.national_number,
                 "extension": parsed_number.extension,
             }
             return number_info
         except NumberParseException as e:
             logger.exception(f"Invalid phone number: {original_number}.", object=e)
             raise e
 
@@ -128,14 +134,15 @@
             'number_original': original_phone_number,
             'international_code': normalized_phone_number['international_code'],
             'full_number_normalized': normalized_phone_number['full_number_normalized'],
             'local_number_normalized': int(str(normalized_phone_number['full_number_normalized'])
                                            .replace(str(normalized_phone_number['international_code']), '')),
             'created_user_id': logger.user_context.get_effective_user_id(),
         }
+        # TODO phone_data -> phone_dict
         phone_id = self.insert(data_dict=phone_data)
 
         # link phone to profile
         profile_id = user_context.get_effective_profile_id()
         if profile_id:
             phone_profile_id = self.insert_mapping(
                 schema_name='phone_profile',
@@ -177,8 +184,9 @@
             'number_original': number_original,
             'local_number_normalized': int(number_original[3:]),  # must be unique
             'full_number_normalized': f'+{international_code}{number_original[1:]}',
             'international_code': international_code,
             'area_code': int(number_original[1:3]),
             'extension': number_original[3],
         }
-        return self.insert_phone(phone_data=phone_data)
+        test_phone_id = self.insert_phone(phone_data=phone_data)
+        return test_phone_id
```

### Comparing `phones_local-0.0.26/phones_local.egg-info/PKG-INFO` & `phones_local-0.0.27/phones_local.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.26
+Version: 0.0.27
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.26/pyproject.toml` & `phones_local-0.0.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 # TODO: Please update the name, similar to storage-local (suffix -local)
 name = "<project-name>"
 # I believe we are still using the version from setup.py and not from here until potery will work
-version = "0.0.1" # https://pypi.org/project/<project-name> i.e. https://pypi.org/project/storage-local/
+version = "0.0.2" # https://pypi.org/project/<project-name> i.e. https://pypi.org/project/storage-local/
 description = "<project-name> Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
```

### Comparing `phones_local-0.0.26/setup.py` & `phones_local-0.0.27/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.26',  # https://pypi.org/project/phones-local/
+    version='0.0.27',  # https://pypi.org/project/phones-local/
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="PyPI Package for Circles phone local Python",
```

