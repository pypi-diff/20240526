# Comparing `tmp/contact_phone_local-0.0.18.tar.gz` & `tmp/contact_phone_local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_phone_local-0.0.18.tar", last modified: Sun May 26 21:42:59 2024, max compression
+gzip compressed data, was "contact_phone_local-0.0.9.tar", last modified: Tue May  7 15:33:35 2024, max compression
```

## Comparing `contact_phone_local-0.0.18.tar` & `contact_phone_local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:42:59.032971 contact_phone_local-0.0.18/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-26 21:42:59.032971 contact_phone_local-0.0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-26 21:42:27.000000 contact_phone_local-0.0.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:42:59.032971 contact_phone_local-0.0.18/contact_phone_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:42:59.032971 contact_phone_local-0.0.18/contact_phone_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:42:27.000000 contact_phone_local-0.0.18/contact_phone_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-26 21:42:27.000000 contact_phone_local-0.0.18/contact_phone_local/src/contact_phone_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-26 21:42:27.000000 contact_phone_local-0.0.18/contact_phone_local/src/contact_phone_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:42:59.032971 contact_phone_local-0.0.18/contact_phone_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-26 21:42:59.000000 contact_phone_local-0.0.18/contact_phone_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-26 21:42:59.000000 contact_phone_local-0.0.18/contact_phone_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:42:59.000000 contact_phone_local-0.0.18/contact_phone_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-26 21:42:59.000000 contact_phone_local-0.0.18/contact_phone_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 21:42:59.000000 contact_phone_local-0.0.18/contact_phone_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-26 21:42:33.000000 contact_phone_local-0.0.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 21:42:59.032971 contact_phone_local-0.0.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-26 21:42:27.000000 contact_phone_local-0.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:33:35.277199 contact_phone_local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-07 15:33:35.277199 contact_phone_local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 15:33:14.000000 contact_phone_local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:33:35.277199 contact_phone_local-0.0.9/contact_phone_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:33:35.277199 contact_phone_local-0.0.9/contact_phone_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:33:14.000000 contact_phone_local-0.0.9/contact_phone_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-05-07 15:33:14.000000 contact_phone_local-0.0.9/contact_phone_local/src/contact_phones_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-07 15:33:14.000000 contact_phone_local-0.0.9/contact_phone_local/src/contact_phones_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:33:35.277199 contact_phone_local-0.0.9/contact_phone_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-07 15:33:35.000000 contact_phone_local-0.0.9/contact_phone_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 15:33:35.000000 contact_phone_local-0.0.9/contact_phone_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:33:35.000000 contact_phone_local-0.0.9/contact_phone_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 15:33:35.000000 contact_phone_local-0.0.9/contact_phone_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 15:33:35.000000 contact_phone_local-0.0.9/contact_phone_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-07 15:33:14.000000 contact_phone_local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:33:35.277199 contact_phone_local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-07 15:33:14.000000 contact_phone_local-0.0.9/setup.py
```

### Comparing `contact_phone_local-0.0.18/contact_phone_local/src/contact_phone_local.py` & `contact_phone_local-0.0.9/contact_phone_local/src/contact_phones_local.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,111 @@
+from .contact_phones_local_constants import CONTACT_PHONES_PYTHON_PACKAGE_CODE_LOGGER_OBJECT
+from logger_local.Logger import Logger
 from database_mysql_local.generic_mapping import GenericMapping
-from logger_local.MetaLogger import MetaLogger
-from phones_local.phones_local import PhonesLocal
-
-from .contact_phone_local_constants import CONTACT_PHONE_PYTHON_PACKAGE_CODE_LOGGER_OBJECT
+from phone_local.phones_local import PhonesLocal
+from phonenumbers import (NumberParseException, PhoneNumberFormat,
+                          format_number, parse)
 
 DEFAULT_SCHEMA_NAME = 'contact_phone'
 DEFAULT_ENTITY_NAME1 = 'contact'
 DEFAULT_ENTITY_NAME2 = 'phone'
 DEFAULT_ID_COLUMN_NAME = 'contact_phone_id'
 DEFAULT_TABLE_NAME = 'contact_phone_table'
 DEFAULT_VIEW_TABLE_NAME = 'contact_phone_view'
 
 
-class ContactPhoneLocal(GenericMapping, metaclass=MetaLogger, object=CONTACT_PHONE_PYTHON_PACKAGE_CODE_LOGGER_OBJECT):
-    def __init__(self, is_test_data: bool = False):
-
-        GenericMapping.__init__(self, default_schema_name=DEFAULT_SCHEMA_NAME,
-                                default_entity_name1=DEFAULT_ENTITY_NAME1,
-                                default_entity_name2=DEFAULT_ENTITY_NAME2, default_column_name=DEFAULT_ID_COLUMN_NAME,
-                                default_table_name=DEFAULT_TABLE_NAME, default_view_table_name=DEFAULT_VIEW_TABLE_NAME,
-                                is_test_data=is_test_data)
+class ContactPhonesLocal(GenericMapping):
+    def __init__(self, default_schema_name: str = DEFAULT_SCHEMA_NAME, default_entity_name1: str = DEFAULT_ENTITY_NAME1,
+                 default_entity_name2: str = DEFAULT_ENTITY_NAME2, default_id_column_name: str = DEFAULT_ID_COLUMN_NAME,
+                 default_table_name: str = DEFAULT_TABLE_NAME, default_view_table_name: str = DEFAULT_VIEW_TABLE_NAME,
+                 is_test_data: bool = False):
+
+        super().__init__(default_schema_name=default_schema_name, default_entity_name1=default_entity_name1,
+                         default_entity_name2=default_entity_name2, default_id_column_name=default_id_column_name,
+                         default_table_name=default_table_name, default_view_table_name=default_view_table_name,
+                         is_test_data=is_test_data)
         self.phones_local = PhonesLocal()
+        self.logger = Logger.create_logger(object=CONTACT_PHONES_PYTHON_PACKAGE_CODE_LOGGER_OBJECT)
 
     # UPSERT
     # TODO Why do we have region as a parameter? - Should be able to extract it from the phone or contact_id
     # TODO Expected phone_number is original_phone_number of processed_phone_number?
-    # TODO: contact_dict not used
-    def insert_contact_and_link_to_existing_or_new_phone(
-            self, *, contact_dict: dict, phone_number: str, contact_id: int, region: str = None) -> int:
+    def insert_contact_and_link_to_existing_or_new_phone(self, contact_dict: dict, phone_number: str,
+                                                         contact_id: int, region: str = None) -> int:
         """
         Insert contact and link to existing or new phone
         :param contact_dict: contact dict
         :param phone_number: phone number
         :param contact_id: contact id
         :param region: region (For example, 'US' stands for the United States, 'GB' for the United Kingdom)
         :return: contact_phone_id
         """
+        self.logger.start(object={"contact_dict": contact_dict, "phone_number": phone_number,
+                                  "contact_id": contact_id, "region": region})
 
         # phone = new PhoneLocal( phone_number );
+                                                           
+        proccessed_phone_number = self.process_phone_number(original_number=phone_number, region=region)
 
-        proccessed_phone_number = PhonesLocal.normalize_phone_number(original_number=phone_number, region=region)
-        full_number_normalized = proccessed_phone_number.get("full_number_normalized")
-        local_number_normalized = proccessed_phone_number.get("local_number_normalized")
-        if not full_number_normalized or not local_number_normalized:
-            raise Exception(f"Invalid phone number: {phone_number}")
-
-        # Add the people(person/contact/profile/user) to the Country Group based on their phone internationa_dialing_code
+        # Add the people(person/contact/profile/user) to the Country Group based on their phone internationa_dialing_code                                                   
         # TODO call process_people_phone_number( entity_name='Contact', phone) from phone-local-python-package
 
         # I would recommend moving this code to the PhoneLocal class and calling it in the Phone constructor
         # TODO Can we replace this by UPSERT?
         phone_id_tuple = self.phones_local.select_one_tuple_by_where(
             select_clause_value="phone_id",
-            where="number_original = %s OR full_number_normalized = %s OR local_number_normalized = %s",
-            params=(phone_number, full_number_normalized, local_number_normalized)
+            where="full_number_normalized = %s",
+            params=(proccessed_phone_number['full_number_normalized'],)
         )
-
         if not phone_id_tuple:
             # create new phone and add it to phone_table
-            self.logger.info("phone_id is None, adding new phone")
-            phone_compare_data_dict = {
+            self.logger.info(log_message="phone_id is None, adding new phone")
+            phone_compare_data_json = {
                 "number_original": proccessed_phone_number.get("number_original"),
-                "full_number_normalized": proccessed_phone_number.get("full_number_normalized"),
-                "local_number_normalized": proccessed_phone_number.get("local_number_normalized"),
             }
-            phone_id = self.phones_local.upsert(data_dict=proccessed_phone_number,
-                                                data_dict_compare=phone_compare_data_dict,
-                                                view_table_name="phone_view", table_name="phone_table",
-                                                compare_with_or=True)
+            phone_id = self.phones_local.upsert(data_json=proccessed_phone_number, data_json_compare=phone_compare_data_json,
+                                                view_table_name="phone_view", table_name="phone_table")
             contact_phone_id = self.insert_mapping(entity_name1=self.default_entity_name1,
                                                    entity_name2=self.default_entity_name2,
-                                                   entity_id1=contact_id, entity_id2=phone_id,
-                                                   ignore_duplicate=True)
+                                                   entity_id1=contact_id, entity_id2=phone_id)
         else:
             # link to existing phone
-            self.logger.info("phone_id is not None, linking to existing phone")
+            self.logger.info(log_message="phone_id is not None, linking to existing phone")
             phone_id = phone_id_tuple[0]
             mapping_tuple = self.select_multi_mapping_tuple_by_id(entity_name1=self.default_entity_name1,
                                                                   entity_name2=self.default_entity_name2,
                                                                   entity_id1=contact_id, entity_id2=phone_id)
             if not mapping_tuple:
-                self.logger.info("mapping_tuple is None, creating new mapping")
+                self.logger.info(log_message="mapping_tuple is None, creating new mapping")
                 contact_phone_id = self.insert_mapping(entity_name1=self.default_entity_name1,
                                                        entity_name2=self.default_entity_name2,
-                                                       entity_id1=contact_id, entity_id2=phone_id,
-                                                       ignore_duplicate=True)
+                                                       entity_id1=contact_id, entity_id2=phone_id)
             else:
-                self.logger.info("mapping_tuple is not None")
+                self.logger.info(log_message="mapping_tuple is not None")
                 contact_phone_id = mapping_tuple[0][0]
 
+        self.logger.end(object={"contact_phone_id": contact_phone_id})
         return contact_phone_id
+
+    # TODO: Move this to PhoneLocal
+    def process_phone_number(self, original_number: str, region: str = None) -> dict:
+        try:
+            parsed_number = parse(original_number, region)
+            international_code = parsed_number.country_code
+            full_number_normalized = format_number(parsed_number, PhoneNumberFormat.E164)
+            if full_number_normalized.startswith("+"):
+                full_number_normalized = full_number_normalized[1:]
+            local_number_normalized = str(parsed_number.national_number)
+            # TODO: Shall we add area_code? what shall it be? How can we do it?
+            # TODO Can we move number_info to data member in PhoneLocal class
+            number_info = {
+                "number_original": original_number,
+                "international_code": international_code,
+                "full_number_normalized": full_number_normalized,
+                "local_number_normalized": local_number_normalized,
+            }
+            return number_info
+        #TODO e -> exception
+        except NumberParseException as e:
+            self.logger.error(
+                # TODO Add a second parameter with exception and all parameters of the method
+                f"Invalid phone number: {original_number}. Exception: {str(e)}")
```

### Comparing `contact_phone_local-0.0.18/contact_phone_local/src/contact_phone_local_constants.py` & `contact_phone_local-0.0.9/contact_phone_local/src/contact_phones_local_constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
-CONTACT_PHONE_LOCAL_PYTHON_COMPONENT_ID = 278
-CONTACT_PHONE_LOCAL_PYTHON_COMPONENT_NAME = "contact-phone-local-python-package"
+
+CONTACT_PHONES_LOCAL_PYTHON_COMPONENT_ID = 278
+CONTACT_PHONES_LOCAL_PYTHON_COMPONENT_NAME = "contact-phones-local-python-package"
 DEVELOPER_EMAIL = "tal.g@circ.zone"
-CONTACT_PHONE_PYTHON_PACKAGE_CODE_LOGGER_OBJECT = {
-    'component_id': CONTACT_PHONE_LOCAL_PYTHON_COMPONENT_ID,
-    'component_name': CONTACT_PHONE_LOCAL_PYTHON_COMPONENT_NAME,
+CONTACT_PHONES_PYTHON_PACKAGE_CODE_LOGGER_OBJECT = {
+    'component_id': CONTACT_PHONES_LOCAL_PYTHON_COMPONENT_ID,
+    'component_name': CONTACT_PHONES_LOCAL_PYTHON_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     'developer_email': DEVELOPER_EMAIL
 }
 
-CONTACT_PHONE_PYTHON_PACKAGE_TEST_LOGGER_OBJECT = {
-    'component_id': CONTACT_PHONE_LOCAL_PYTHON_COMPONENT_ID,
-    'component_name': CONTACT_PHONE_LOCAL_PYTHON_COMPONENT_NAME,
+CONTACT_PHONES_PYTHON_PACKAGE_TEST_LOGGER_OBJECT = {
+    'component_id': CONTACT_PHONES_LOCAL_PYTHON_COMPONENT_ID,
+    'component_name': CONTACT_PHONES_LOCAL_PYTHON_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Unit_Test.value,
     'testing_framework': LoggerComponentEnum.testingFramework.pytest.value,
     'developer_email': DEVELOPER_EMAIL
 }
```

