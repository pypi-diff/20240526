# Comparing `tmp/contact-location-local-0.0.8.tar.gz` & `tmp/contact-location-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact-location-local-0.0.8.tar", last modified: Tue Mar 19 15:20:03 2024, max compression
+gzip compressed data, was "contact-location-local-0.0.9.tar", last modified: Fri Mar 29 15:39:46 2024, max compression
```

## Comparing `contact-location-local-0.0.8.tar` & `contact-location-local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:20:03.760400 contact-location-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-19 15:20:03.760400 contact-location-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-19 15:19:33.000000 contact-location-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:20:03.756400 contact-location-local-0.0.8/contact_location_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:20:03.756400 contact-location-local-0.0.8/contact_location_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:33.000000 contact-location-local-0.0.8/contact_location_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17826 2024-03-19 15:19:33.000000 contact-location-local-0.0.8/contact_location_local/src/contact_location_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-19 15:19:33.000000 contact-location-local-0.0.8/contact_location_local/src/contact_location_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:20:03.760400 contact-location-local-0.0.8/contact_location_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-19 15:20:03.000000 contact-location-local-0.0.8/contact_location_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-19 15:20:03.000000 contact-location-local-0.0.8/contact_location_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 15:20:03.000000 contact-location-local-0.0.8/contact_location_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-19 15:20:03.000000 contact-location-local-0.0.8/contact_location_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-19 15:20:03.000000 contact-location-local-0.0.8/contact_location_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-19 15:19:33.000000 contact-location-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 15:20:03.760400 contact-location-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-19 15:19:33.000000 contact-location-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:39:46.041058 contact-location-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-29 15:39:46.041058 contact-location-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-29 15:39:18.000000 contact-location-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:39:46.037058 contact-location-local-0.0.9/contact_location_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:39:46.041058 contact-location-local-0.0.9/contact_location_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 15:39:18.000000 contact-location-local-0.0.9/contact_location_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17685 2024-03-29 15:39:18.000000 contact-location-local-0.0.9/contact_location_local/src/contact_location_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-29 15:39:18.000000 contact-location-local-0.0.9/contact_location_local/src/contact_location_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:39:46.041058 contact-location-local-0.0.9/contact_location_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-29 15:39:46.000000 contact-location-local-0.0.9/contact_location_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-29 15:39:46.000000 contact-location-local-0.0.9/contact_location_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 15:39:46.000000 contact-location-local-0.0.9/contact_location_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-29 15:39:46.000000 contact-location-local-0.0.9/contact_location_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-29 15:39:46.000000 contact-location-local-0.0.9/contact_location_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-29 15:39:18.000000 contact-location-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 15:39:46.041058 contact-location-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-29 15:39:18.000000 contact-location-local-0.0.9/setup.py
```

### Comparing `contact-location-local-0.0.8/PKG-INFO` & `contact-location-local-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-location-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles contact-location-local Python
 Home-page: https://github.com/circles-zone/contact-location-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact-location-local-0.0.8/contact_location_local/src/contact_location_local.py` & `contact-location-local-0.0.9/contact_location_local/src/contact_location_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         :return: country_id: int, country_data: dict
         """
         if not self.__validate_method_arguments(country_name, coordinate):
             logger.warning("country_name or coordinate is None",
                            object={"country_name": country_name, "coordinate": coordinate})
             return None, None
         country_data = {}
-        country_id = Country.get_country_id_by_country_name(country_name=country_name)
+        country_id = Country().get_country_id_by_country_name(country_name=country_name)
         if country_id is None:
             country_information = self.get_country_information(
                 country_name=country_name)
             country_data.update({
                 'coordinate': coordinate,
                 'iso': country_information.get("alpha_2"),
                 'name': country_name,
@@ -211,25 +211,24 @@
         :param coordinate: coordinate
         :return: state_id: int
         """
         if not self.__validate_method_arguments(state_name, country_id):
             logger.warning("state_name or country_id is None",
                            object={"state_name": state_name, "country_id": country_id})
             return None
-        state_id = State.get_state_id_by_state_name(
-            state_name=state_name, country_id=country_id)
+        state_id = State().get_state_id_by_state_name(
+            state_name=state_name)
         if state_id is None:
             group_id = self.get_or_create_group_id(
                 group_name=state_name, group_category_id=STATE_THEY_LIVE_IN_GROUP_CATEGORY,
                 is_test_data=self.is_test_data, profile_id=self.profile_id)
             state_lang_code = LangCode.detect_lang_code(text=state_name)
             state_id = State().insert(
                 state=state_name,
                 lang_code=state_lang_code,
-                country_id=country_id,
                 group_id=group_id)
         return state_id
 
     def __process_city(self, city_name: str, country_id: int, coordinate: Point) -> int:
         """
         Process city information
         :param city_name: city name
@@ -237,16 +236,16 @@
         :param coordinate: coordinate
         :return: city_id: int
         """
         if not self.__validate_method_arguments(city_name, country_id):
             logger.error("city_name or country_id is None",
                          object={"city_name": city_name, "country_id": country_id})
             return None
-        city_id = City.get_city_id_by_city_name_state_id(
-            city_name=city_name, country_id=country_id)
+        city_id = City().get_city_id_by_city_name(
+            city_name=city_name)
         if city_id is None:
             group_id = self.get_or_create_group_id(
                 group_name=city_name, group_category_id=CITY_THEY_LIVE_IN_GROUP_CATEGORY,
                 is_test_data=self.is_test_data, profile_id=self.profile_id)
             city_lang_code = LangCode.detect_lang_code(text=city_name)
             city_id = City().insert(city=city_name, lang_code=city_lang_code,
                                     coordinate=coordinate, group_id=group_id)
@@ -260,16 +259,16 @@
         :param coordinate: coordinate
         :return: county_id: int
         """
         if not self.__validate_method_arguments(county_name, state_id):
             logger.warning("county_name or state_id is None",
                            object={"county_name": county_name, "state_id": state_id})
             return None
-        county_id = County.get_county_id_by_county_name_state_id(
-            county_name=county_name, state_id=state_id)
+        county_id = County().get_county_id_by_county_name_state_id(
+            county_name=county_name)
         if county_id is None:
             group_id = self.get_or_create_group_id(
                 group_name=county_name, group_category_id=None,
                 is_test_data=self.is_test_data, profile_id=self.profile_id)
 
             county_lang_code = LangCode.detect_lang_code(text=county_name)
             county_id = County().insert(county=county_name, lang_code=county_lang_code,
@@ -284,16 +283,16 @@
         :param coordinate: coordinate
         :return: region_id: int
         """
         if not self.__validate_method_arguments(region_name, country_id):
             logger.warning("region_name or country_id is None",
                            object={"region_name": region_name, "country_id": country_id})
             return None
-        region_id = Region.get_region_id_by_region_name(
-            region_name=region_name, country_id=country_id)
+        region_id = Region().get_region_id_by_region_name(
+            region_name=region_name)
         if region_id is None:
             group_id = self.get_or_create_group_id(
                 group_name=region_name, group_category_id=None,
                 is_test_data=self.is_test_data, profile_id=self.profile_id)
 
             region_lang_code = LangCode.detect_lang_code(text=region_name)
             region_id = Region().insert(region=region_name,
@@ -311,16 +310,16 @@
         :param coordinate: coordinate
         :return: neighborhood_id: int
         """
         if not self.__validate_method_arguments(neighborhood_name, city_id):
             logger.warning("neighborhood_name or city_id is None",
                            object={"neighborhood_name": neighborhood_name, "city_id": city_id, "coordinate": coordinate})
             return None
-        neighborhood_id = Neighborhood.get_neighborhood_id_by_neighborhood_name(
-            neighborhood_name=neighborhood_name, city_id=city_id)
+        neighborhood_id = Neighborhood().get_neighborhood_id_by_neighborhood_name(
+            neighborhood_name=neighborhood_name)
         if neighborhood_id is None:
             group_id = self.get_or_create_group_id(
                 group_name=neighborhood_name, group_category_id=None,
                 is_test_data=self.is_test_data, profile_id=self.profile_id)
 
             neighborhood_lang_code = LangCode.detect_lang_code(text=neighborhood_name)
             neighborhood_id = Neighborhood().insert(neighborhood=neighborhood_name,
```

### Comparing `contact-location-local-0.0.8/contact_location_local/src/contact_location_local_constants.py` & `contact-location-local-0.0.9/contact_location_local/src/contact_location_local_constants.py`

 * *Files identical despite different names*

### Comparing `contact-location-local-0.0.8/contact_location_local.egg-info/PKG-INFO` & `contact-location-local-0.0.9/contact_location_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-location-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles contact-location-local Python
 Home-page: https://github.com/circles-zone/contact-location-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact-location-local-0.0.8/setup.py` & `contact-location-local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "contact-location-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # update only the minor version each time # https://pypi.org/project/contact-location-local/
+    version='0.0.9',  # update only the minor version each time # https://pypi.org/project/contact-location-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-location-local Python",
     long_description="PyPI Package for Circles contact-location-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/contact-location-local-python-package",
     packages=[package_dir],
```

