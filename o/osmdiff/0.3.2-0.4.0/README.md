# Comparing `tmp/osmdiff-0.3.2.tar.gz` & `tmp/osmdiff-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "osmdiff-0.4.0.tar", last modified: Sat May 25 23:42:51 2024, max compression
```

## Comparing `osmdiff-0.3.2.tar` & `osmdiff-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,19 @@
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 osmdiff-0.3.2/setup.cfg
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 osmdiff-0.3.2/setup.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 osmdiff-0.3.2/.github/dependabot.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 osmdiff-0.3.2/.vscode/settings.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 osmdiff-0.3.2/src/osmdiff/__init__.py
--rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 osmdiff-0.3.2/src/osmdiff/augmenteddiff.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 osmdiff-0.3.2/src/osmdiff/osmchange.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 osmdiff-0.3.2/src/osmdiff/osm/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 osmdiff-0.3.2/src/osmdiff/osm/osm.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 osmdiff-0.3.2/tests/test_api.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 osmdiff-0.3.2/tests/test_node.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 osmdiff-0.3.2/tests/test_osmchange.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 osmdiff-0.3.2/tests/test_relation.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 osmdiff-0.3.2/tests/test_way.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 osmdiff-0.3.2/tests/try.py
--rw-r--r--   0        0        0  4935683 2020-02-02 00:00:00.000000 osmdiff-0.3.2/tests/fixtures/test_adiff.xml
--rw-r--r--   0        0        0   855655 2020-02-02 00:00:00.000000 osmdiff-0.3.2/tests/fixtures/test_osmchange.xml
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 osmdiff-0.3.2/.gitignore
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 osmdiff-0.3.2/LICENSE
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 osmdiff-0.3.2/README.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 osmdiff-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 osmdiff-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      562 2024-05-25 23:42:36.374372 osmdiff-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3504 2024-05-25 23:42:36.374372 osmdiff-0.4.0/README.md
+-rw-r--r--   0        0        0     1170 2024-05-25 23:42:51.542408 osmdiff-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      357 2024-05-25 23:42:36.374372 osmdiff-0.4.0/src/osmdiff/__init__.py
+-rw-r--r--   0        0        0     4611 2024-05-25 23:42:36.374372 osmdiff-0.4.0/src/osmdiff/augmenteddiff.py
+-rw-r--r--   0        0        0       48 2024-05-25 23:42:36.374372 osmdiff-0.4.0/src/osmdiff/osm/__init__.py
+-rw-r--r--   0        0        0     3052 2024-05-25 23:42:36.374372 osmdiff-0.4.0/src/osmdiff/osm/osm.py
+-rw-r--r--   0        0        0     5054 2024-05-25 23:42:36.374372 osmdiff-0.4.0/src/osmdiff/osmchange.py
+-rw-r--r--   0        0        0      188 2024-05-25 23:42:36.374372 osmdiff-0.4.0/src/osmdiff/settings.py
+-rw-r--r--   0        0        0        0 2024-05-25 23:42:36.374372 osmdiff-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      342 2024-05-25 23:42:36.374372 osmdiff-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0  4935683 2024-05-25 23:42:36.390372 osmdiff-0.4.0/tests/data/test_adiff.xml
+-rw-r--r--   0        0        0   855655 2024-05-25 23:42:36.390372 osmdiff-0.4.0/tests/data/test_osmchange.xml
+-rw-r--r--   0        0        0      860 2024-05-25 23:42:36.390372 osmdiff-0.4.0/tests/test_api.py
+-rw-r--r--   0        0        0      506 2024-05-25 23:42:36.390372 osmdiff-0.4.0/tests/test_node.py
+-rw-r--r--   0        0        0     1689 2024-05-25 23:42:36.390372 osmdiff-0.4.0/tests/test_osmchange.py
+-rw-r--r--   0        0        0      586 2024-05-25 23:42:36.390372 osmdiff-0.4.0/tests/test_relation.py
+-rw-r--r--   0        0        0      502 2024-05-25 23:42:36.394372 osmdiff-0.4.0/tests/test_way.py
+-rw-r--r--   0        0        0     4189 1970-01-01 00:00:00.000000 osmdiff-0.4.0/PKG-INFO
```

### Comparing `osmdiff-0.3.2/src/osmdiff/augmenteddiff.py` & `osmdiff-0.4.0/src/osmdiff/augmenteddiff.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-import os
+from posixpath import join as urljoin
 from xml.etree import cElementTree
 
 import dateutil.parser
 import requests
 
 from .osm import OSMObject
 
-OVERPASS_URL = "http://overpass-api.de/api"
+from osmdiff.settings import DEFAULT_OVERPASS_URL
 
 
 class AugmentedDiff(object):
-    base_url = OVERPASS_URL
+    """
+    Class to represent an Augmented Diff object.
+    """
+
+    base_url = DEFAULT_OVERPASS_URL
     minlon = None
     minlat = None
     maxlon = None
     maxlat = None
     timestamp = None
-    debug = False
+    remarks = []
 
     def __init__(
         self,
         minlon=None,
         minlat=None,
         maxlon=None,
         maxlat=None,
-        debug=False,
         file=None,
         sequence_number=None,
         timestamp=None,
     ):
-        self.debug = debug
         self.create = []
         self.modify = []
         self.delete = []
         if file:
             with open(file, "r") as file_handle:
                 self._parse_stream(file_handle)
         else:
@@ -45,17 +47,15 @@
                     self.maxlon = maxlon
                     self.maxlat = maxlat
                 else:
                     raise Exception("invalid bbox.")
 
     def get_state(self):
         """Get the current state from the OSM API"""
-        state_url = os.path.join(self.base_url, "augmented_diff_status")
-        if self.debug:
-            print("getting state from", state_url)
+        state_url = urljoin(self.base_url, "augmented_diff_status")
         response = requests.get(state_url, timeout=5)
         if response.status_code != 200:
             return False
         self.sequence_number = int(response.text)
         return True
 
     def _build_adiff_url(self):
@@ -65,74 +65,83 @@
         if self.minlon and self.minlat and self.maxlon and self.maxlat:
             url += "&bbox={minlon},{minlat},{maxlon},{maxlat}".format(
                 minlon=self.minlon,
                 minlat=self.minlat,
                 maxlon=self.maxlon,
                 maxlat=self.maxlat,
             )
-        if self.debug:
-            print(url)
         return url
 
     def _build_action(self, elem):
         if elem.attrib["type"] == "create":
             for child in elem:
                 e = OSMObject.from_xml(child)
                 self.__getattribute__("create").append(e)
-                if self.debug:
-                    print(elem.attrib["type"], e)
         else:
             new = elem.find("new")
             old = elem.find("old")
             osm_obj_old = None
             osm_obj_new = None
             for child in old:
                 osm_obj_old = OSMObject.from_xml(child)
             for child in new:
                 osm_obj_new = OSMObject.from_xml(child)
-            if self.debug:
-                print(elem.attrib["type"], ": old", osm_obj_old, ", new", osm_obj_new)
             self.__getattribute__(elem.attrib["type"]).append(
                 {"old": osm_obj_old, "new": osm_obj_new}
             )
 
     def _parse_stream(self, stream):
         for event, elem in cElementTree.iterparse(stream):
-            # if self.debug:
-            #     print(event, elem)
             if elem.tag == "remark":
-                raise Exception("Augmented Diff API returned an error:", elem.text)
+                self.remarks.append(elem.text)
             if elem.tag == "meta":
                 timestamp = dateutil.parser.parse(elem.attrib.get("osm_base"))
                 self.timestamp = timestamp
             if elem.tag == "action":
                 self._build_action(elem)
 
-    def retrieve(self, clear_cache=False) -> int:
+    def retrieve(self, clear_cache=False, timeout=30) -> int:
         """
         Retrieve the Augmented diff corresponding to the sequence_number.
         """
         if not self.sequence_number:
             raise Exception("invalid sequence number")
         if clear_cache:
             self.create, self.modify, self.delete = ([], [], [])
         url = self._build_adiff_url()
-        if self.debug:
-            print("retrieving...")
         try:
-            r = requests.get(url, stream=True, timeout=30)
+            r = requests.get(url, stream=True, timeout=timeout)
             if r.status_code != 200:
                 return r.status_code
             r.raw.decode_content = True
-            if self.debug:
-                print("parsing...")
             self._parse_stream(r.raw)
             return r.status_code
         except ConnectionError:
             # FIXME should we catch instead?
             return 0
 
+    @property
+    def remarks(self):
+        return self._remarks
+
+    @property
+    def timestamp(self):
+        return self._timestamp
+
+    @property
+    def sequence_number(self):
+        return self._sequence_number
+
+    @sequence_number.setter
+    def sequence_number(self, value):
+        try:
+            self._sequence_number = int(value)
+        except ValueError:
+            raise ValueError(
+                "sequence_number must be an integer or parsable as an integer"
+            )
+
     def __repr__(self):
         return "AugmentedDiff ({create} created, {modify} modified, \
 {delete} deleted)".format(
             create=len(self.create), modify=len(self.modify), delete=len(self.delete)
         )
```

### Comparing `osmdiff-0.3.2/src/osmdiff/osm/osm.py` & `osmdiff-0.4.0/src/osmdiff/osm/osm.py`

 * *Files identical despite different names*

### Comparing `osmdiff-0.3.2/tests/test_api.py` & `osmdiff-0.4.0/tests/test_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+import pytest
 from osmdiff import AugmentedDiff, OSMChange
 from typing_extensions import assert_type
 
 
 class TestApi:
     "tests for API calls"
 
     state = None
 
+    @pytest.mark.integration
     def test_osm_diff_api(self):
         "Test getting state from OSM API"
         osm_change = OSMChange()
         assert osm_change.get_state()
         self.state = osm_change.sequence_number
         assert_type(self.state, int)
         status = osm_change.retrieve()
         assert status == 200
 
+    @pytest.mark.integration
     def test_augmented_diff_api(self):
         "Test getting augmented diff from Overpass API"
         augmented_diff = AugmentedDiff()
         assert augmented_diff.get_state()
         self.state = augmented_diff.sequence_number
         assert_type(self.state, int)
         status = augmented_diff.retrieve()
```

### Comparing `osmdiff-0.3.2/tests/test_osmchange.py` & `osmdiff-0.4.0/tests/test_osmchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-from pathlib import Path
-
 from osmdiff import Node, OSMChange, Relation, Way
 from typing_extensions import assert_type
 
 
 class TestOSMChange:
     "tests for OSMChange object"
 
-    osmchange_file_path = (
-        Path(__file__).parent / "fixtures/test_osmchange.xml"
-    ).resolve()
-
     def test_init_osmchange(self):
         "Test OSMChange init"
         osmchange = OSMChange()
         assert_type(osmchange, OSMChange)
         assert_type(osmchange.create, list)
         assert_type(osmchange.modify, list)
         assert_type(osmchange.delete, list)
@@ -27,20 +21,20 @@
         osm_change = OSMChange()
         assert not osm_change.sequence_number
         osm_change.sequence_number = 12345
         assert osm_change.sequence_number == 12345
         osm_change.sequence_number = "12345"
         assert osm_change.sequence_number == 12345
 
-    def test_3_readfromfile(self):
-        "Test initializing from file"
-        osmchange = OSMChange.from_xml(self.osmchange_file_path)
-        assert len(osmchange.create) == 831
-        assert len(osmchange.modify) == 368
-        assert len(osmchange.delete) == 3552
+    def test_read_changeset_from_xml_file(self, osmchange_file_path):
+        "Test initializing from an XML object"
+        osmchange = OSMChange.from_xml_file(osmchange_file_path)
+        assert len(osmchange.create) == 1004
+        assert len(osmchange.modify) == 585
+        assert len(osmchange.delete) == 3800
         nodes_created = [o for o in osmchange.create if isinstance(o, Node)]
         ways_created = [o for o in osmchange.create if isinstance(o, Way)]
         rels_created = [o for o in osmchange.create if isinstance(o, Relation)]
-        assert len(nodes_created) == 699
-        assert len(ways_created) == 132
+        assert len(nodes_created) == 858
+        assert len(ways_created) == 146
         assert len(rels_created) == 0
         assert len(nodes_created + ways_created + rels_created) == len(osmchange.create)
```

### Comparing `osmdiff-0.3.2/tests/test_relation.py` & `osmdiff-0.4.0/tests/test_relation.py`

 * *Files identical despite different names*

### Comparing `osmdiff-0.3.2/tests/fixtures/test_adiff.xml` & `osmdiff-0.4.0/tests/data/test_adiff.xml`

 * *Files identical despite different names*

### Comparing `osmdiff-0.3.2/tests/fixtures/test_osmchange.xml` & `osmdiff-0.4.0/tests/data/test_osmchange.xml`

 * *Files identical despite different names*

### Comparing `osmdiff-0.3.2/LICENSE` & `osmdiff-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osmdiff-0.3.2/README.md` & `osmdiff-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-> I am considering moving my open source repos to sourcehut. For now, I mirror this repo at sourcehut, and issues are still on here. The plan is to move the issue tracker to sourcehut next, and then archive this repo. No, I don't have a timeline.
-
 # osmdiff
 
+[![build and test](https://github.com/mvexel/osmdiff/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/mvexel/osmdiff/actions/workflows/build_and_test.yml)
+
 A read-only interface to OpenStreetMap change APIs and files. See also [pyosm](https://github.com/iandees/pyosm) which can do similar things. 
 
 Python 3.7+
 
 ## Installing
 
 `pip install osmdiff`
@@ -14,16 +14,15 @@
 
 ### Reading
 
 Retrieve the latest replication diff from the OSM API:
 
 ```python
 >>> from osmdiff import OSMChange
->>> o = OSMChange()
->>> o.frequency = "minute"  # the default
+>>> o = OSMChange(frequency="minute")  # minute is the default frequency
 >>> o.get_state()  # retrieve current sequence ID
 >>> o.sequence_number
 2704451
 >>> o.retrieve()  # retrieve from API
 >>> o
 OSMChange (677 created, 204 modified, 14 deleted)
 ```
@@ -94,8 +93,16 @@
 {'highway': 'residential'}
 >>> w[0].attribs
 {'id': '452218081', 'version': '2', 'timestamp': '2017-11-10T13:52:01Z', 'changeset': '53667190', 'uid': '2352517', 'user': 'carths81'}
 >>> w[0].attribs
 {'id': '452218081', 'version': '2', 'timestamp': '2017-11-10T13:52:01Z', 'changeset': '53667190', 'uid': '2352517', 'user': 'carths81'}
 >>> w[0].bounds
 ['12.8932677', '43.3575917', '12.8948117', '43.3585947']
-```
+```
+
+## Contributing
+
+I welcome your contributions in code, documentation and suggestions for enhancements.
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+If you find `osmdiff` useful, or you use it in commercial software, please consider sponsoring this project.
```

### Comparing `osmdiff-0.3.2/PKG-INFO` & `osmdiff-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: osmdiff
-Version: 0.3.2
-Summary: A read-only API to OpenStreetMap diffs
-Project-URL: Homepage, https://github.com/osmlab/osmdiff
-Project-URL: Bug Tracker, https://github.com/osmlab/osmdiff/issues
-Author-email: Martijn van Exel <m@rtijn.org>
-License-File: LICENSE
+Version: 0.4.0
+Summary: A read-only interface to OpenStreetMap change APIs and files
+Keywords: openstreetmap,osm,diff,changeset,api
+Author-Email: Martijn van Exel <m@rtijn.org>
+Maintainer-Email: Martijn van Exel <m@rtijn.org>
+License: MIT
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: python-dateutil==2.8.2
+Project-URL: Homepage, https://github.com/mvexel/osmdiff
+Project-URL: Bug tracker, https://github.com/mvexel/osmdiff/issues
+Requires-Python: >=3.8
+Requires-Dist: python-dateutil==2.9.0.post0
 Requires-Dist: requests==2.28.1
-Provides-Extra: test
-Requires-Dist: pytest==7.1.3; extra == 'test'
-Requires-Dist: python-dateutil==2.8.2; extra == 'test'
 Description-Content-Type: text/markdown
 
-> I am considering moving my open source repos to sourcehut. For now, I mirror this repo at sourcehut, and issues are still on here. The plan is to move the issue tracker to sourcehut next, and then archive this repo. No, I don't have a timeline.
-
 # osmdiff
 
+[![build and test](https://github.com/mvexel/osmdiff/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/mvexel/osmdiff/actions/workflows/build_and_test.yml)
+
 A read-only interface to OpenStreetMap change APIs and files. See also [pyosm](https://github.com/iandees/pyosm) which can do similar things. 
 
 Python 3.7+
 
 ## Installing
 
 `pip install osmdiff`
@@ -33,16 +32,15 @@
 
 ### Reading
 
 Retrieve the latest replication diff from the OSM API:
 
 ```python
 >>> from osmdiff import OSMChange
->>> o = OSMChange()
->>> o.frequency = "minute"  # the default
+>>> o = OSMChange(frequency="minute")  # minute is the default frequency
 >>> o.get_state()  # retrieve current sequence ID
 >>> o.sequence_number
 2704451
 >>> o.retrieve()  # retrieve from API
 >>> o
 OSMChange (677 created, 204 modified, 14 deleted)
 ```
@@ -113,8 +111,16 @@
 {'highway': 'residential'}
 >>> w[0].attribs
 {'id': '452218081', 'version': '2', 'timestamp': '2017-11-10T13:52:01Z', 'changeset': '53667190', 'uid': '2352517', 'user': 'carths81'}
 >>> w[0].attribs
 {'id': '452218081', 'version': '2', 'timestamp': '2017-11-10T13:52:01Z', 'changeset': '53667190', 'uid': '2352517', 'user': 'carths81'}
 >>> w[0].bounds
 ['12.8932677', '43.3575917', '12.8948117', '43.3585947']
-```
+```
+
+## Contributing
+
+I welcome your contributions in code, documentation and suggestions for enhancements.
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+If you find `osmdiff` useful, or you use it in commercial software, please consider sponsoring this project.
```

