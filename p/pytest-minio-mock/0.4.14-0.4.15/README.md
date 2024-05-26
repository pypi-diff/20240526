# Comparing `tmp/pytest_minio_mock-0.4.14.tar.gz` & `tmp/pytest_minio_mock-0.4.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_minio_mock-0.4.14.tar", last modified: Sun May 19 11:02:29 2024, max compression
+gzip compressed data, was "pytest_minio_mock-0.4.15.tar", last modified: Sun May 26 09:50:33 2024, max compression
```

## Comparing `pytest_minio_mock-0.4.14.tar` & `pytest_minio_mock-0.4.15.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:02:29.624246 pytest_minio_mock-0.4.14/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-19 11:02:29.624246 pytest_minio_mock-0.4.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:02:29.624246 pytest_minio_mock-0.4.14/pytest_minio_mock/
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/pytest_minio_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49707 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/pytest_minio_mock/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:02:29.624246 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-19 11:02:29.000000 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-19 11:02:29.000000 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:02:29.000000 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 11:02:29.000000 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-19 11:02:29.000000 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:02:29.000000 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:02:29.624246 pytest_minio_mock-0.4.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:02:29.624246 pytest_minio_mock-0.4.14/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    19719 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/tests/test_minio_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:50:33.443352 pytest_minio_mock-0.4.15/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-26 09:50:29.000000 pytest_minio_mock-0.4.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 09:50:29.000000 pytest_minio_mock-0.4.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-26 09:50:33.443352 pytest_minio_mock-0.4.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-26 09:50:29.000000 pytest_minio_mock-0.4.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:50:33.439351 pytest_minio_mock-0.4.15/pytest_minio_mock/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-26 09:50:29.000000 pytest_minio_mock-0.4.15/pytest_minio_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49715 2024-05-26 09:50:29.000000 pytest_minio_mock-0.4.15/pytest_minio_mock/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:50:33.439351 pytest_minio_mock-0.4.15/pytest_minio_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-26 09:50:33.000000 pytest_minio_mock-0.4.15/pytest_minio_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-26 09:50:33.000000 pytest_minio_mock-0.4.15/pytest_minio_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 09:50:33.000000 pytest_minio_mock-0.4.15/pytest_minio_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-26 09:50:33.000000 pytest_minio_mock-0.4.15/pytest_minio_mock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-26 09:50:33.000000 pytest_minio_mock-0.4.15/pytest_minio_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 09:50:33.000000 pytest_minio_mock-0.4.15/pytest_minio_mock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 09:50:33.443352 pytest_minio_mock-0.4.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-26 09:50:29.000000 pytest_minio_mock-0.4.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:50:33.439351 pytest_minio_mock-0.4.15/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19765 2024-05-26 09:50:29.000000 pytest_minio_mock-0.4.15/tests/test_minio_mock.py
```

### Comparing `pytest_minio_mock-0.4.14/LICENSE` & `pytest_minio_mock-0.4.15/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_minio_mock-0.4.14/PKG-INFO` & `pytest_minio_mock-0.4.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-minio-mock
-Version: 0.4.14
+Version: 0.4.15
 Summary: A pytest plugin for mocking Minio S3 interactions
 Home-page: https://github.com/oussjarrousse/pytest-minio-mock
 Author: Oussama Jarrousse
 Author-email: oussama@jarrousse.org
 License: MIT
 Project-URL: Source, https://github.com/oussjarrousse/pytest-minio-mock/
 Project-URL: Tracker, https://github.com/oussjarrousse/pytest-minio-mock/issues
```

### Comparing `pytest_minio_mock-0.4.14/README.md` & `pytest_minio_mock-0.4.15/README.md`

 * *Files identical despite different names*

### Comparing `pytest_minio_mock-0.4.14/pytest_minio_mock/__init__.py` & `pytest_minio_mock-0.4.15/pytest_minio_mock/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 
 For more information and usage examples, please refer to the project's README.md.
 
 """
 
 __title__ = "pytest-minio-mock"
 __description__ = "A pytest plugin for mocking Minio S3 interactions"
-__version__ = "0.4.14"
+__version__ = "0.4.15"
 __status__ = "Production"
 __license__ = "MIT"
 __author__ = "Oussama Jarrousse"
 __maintainer__ = "Oussama Jarrousse"
 __email__ = "oussama@jarrousse.org"
-__credits__ = ["Gustavo Satheler", "@cottephi", "Wouter van Atteveldt"]
+__credits__ = ["Gustavo Satheler", "@cottephi", "Wouter van Atteveldt", "@KelvinHong"]
```

### Comparing `pytest_minio_mock-0.4.14/pytest_minio_mock/plugin.py` & `pytest_minio_mock-0.4.15/pytest_minio_mock/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
         except KeyError as exc:
             raise S3Error(
                 message="The specified key does not exist.",
                 resource=f"/{self.bucket_name}/{object_name}",
                 request_id=None,
                 host_id=None,
                 response="mocked_response",
-                code=404,
+                code="NoSuchKey",
                 bucket_name=self.bucket_name,
                 object_name=object_name,
             ) from exc
 
         try:
             the_object_version = the_object.get_object(version_id, self.versioning)
         except S3Error as e:
```

### Comparing `pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/PKG-INFO` & `pytest_minio_mock-0.4.15/pytest_minio_mock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-minio-mock
-Version: 0.4.14
+Version: 0.4.15
 Summary: A pytest plugin for mocking Minio S3 interactions
 Home-page: https://github.com/oussjarrousse/pytest-minio-mock
 Author: Oussama Jarrousse
 Author-email: oussama@jarrousse.org
 License: MIT
 Project-URL: Source, https://github.com/oussjarrousse/pytest-minio-mock/
 Project-URL: Tracker, https://github.com/oussjarrousse/pytest-minio-mock/issues
```

### Comparing `pytest_minio_mock-0.4.14/setup.py` & `pytest_minio_mock-0.4.15/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     python_requires=">=3.8",
     install_requires=["pytest>=5.0.0", "minio", "pytest-mock", "validators"],
     url="https://github.com/oussjarrousse/pytest-minio-mock",
     license="MIT",
     author="Oussama Jarrousse",
     author_email="oussama@jarrousse.org",
     description="A pytest plugin for mocking Minio S3 interactions",
-    long_description=open("README.md").read(),
+    long_description=open("README.md", encoding="utf-8").read(),
     keywords="pytest minio mock",
     extras_require={"dev": ["pre-commit", "tox"]},
-    version="0.4.14",
+    version="0.4.15",
     long_description_content_type="text/markdown",
     classifiers=[
         "Framework :: Pytest",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
```

### Comparing `pytest_minio_mock-0.4.14/tests/test_minio_mock.py` & `pytest_minio_mock-0.4.15/tests/test_minio_mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     client.remove_bucket(bucket_name)
     buckets = client.list_buckets()
     assert buckets == original_buckets
 
 
 @pytest.mark.API
 @pytest.mark.FUNC
-def test_putting_and_removing_objects_no_versionning(minio_mock):
+def test_putting_and_removing_objects_no_versioning(minio_mock):
     # simple thing
     bucket_name = "test-bucket"
     object_name = "test-object"
     file_path = "tests/fixtures/maya.jpeg"
 
     client = Minio("http://local.host:9000")
     client.make_bucket(bucket_name)
@@ -106,15 +106,16 @@
     # even if include version is True nothing should change because versioning is OFF
     objects = list(client.list_objects(bucket_name, include_version=True))
     assert len(objects) == 0
 
     # test retrieving object after it has been removed
     with pytest.raises(S3Error) as error:
         _ = client.get_object(bucket_name, object_name)
-    assert "The specified key does not exist" in str(error.value)
+    assert error.value.message == "The specified key does not exist."
+    assert error.value.code == "NoSuchKey"
 
 
 @pytest.mark.API
 @pytest.mark.FUNC
 def test_putting_objects_with_versionning_enabled(minio_mock):
     client = Minio("http://local.host:9000")
     bucket_name = "test-bucket"
```

