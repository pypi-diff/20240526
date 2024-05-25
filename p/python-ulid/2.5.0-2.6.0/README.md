# Comparing `tmp/python_ulid-2.5.0.tar.gz` & `tmp/python_ulid-2.6.0.tar.gz`

## Comparing `python_ulid-2.5.0.tar` & `python_ulid-2.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 python_ulid-2.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 python_ulid-2.5.0/.readthedocs.yml
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 python_ulid-2.5.0/CHANGELOG.rst
--rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 python_ulid-2.5.0/README.rst
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 python_ulid-2.5.0/logo.png
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 python_ulid-2.5.0/.github/workflows/lint-and-test.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_ulid-2.5.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 python_ulid-2.5.0/docs/Makefile
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_ulid-2.5.0/docs/requirements.txt
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 python_ulid-2.5.0/docs/source/api.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 python_ulid-2.5.0/docs/source/changelog.rst
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 python_ulid-2.5.0/docs/source/conf.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 python_ulid-2.5.0/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.5.0/tests/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 python_ulid-2.5.0/tests/test_base32.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 python_ulid-2.5.0/tests/test_cli.py
--rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 python_ulid-2.5.0/tests/test_ulid.py
--rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 python_ulid-2.5.0/ulid/__init__.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 python_ulid-2.5.0/ulid/__main__.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 python_ulid-2.5.0/ulid/base32.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 python_ulid-2.5.0/ulid/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.5.0/ulid/py.typed
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 python_ulid-2.5.0/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 python_ulid-2.5.0/LICENSE
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 python_ulid-2.5.0/hatch.toml
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 python_ulid-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 python_ulid-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 python_ulid-2.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 python_ulid-2.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0     5430 2020-02-02 00:00:00.000000 python_ulid-2.6.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 python_ulid-2.6.0/README.rst
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 python_ulid-2.6.0/logo.png
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 python_ulid-2.6.0/.github/workflows/lint-and-test.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_ulid-2.6.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 python_ulid-2.6.0/docs/Makefile
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_ulid-2.6.0/docs/requirements.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 python_ulid-2.6.0/docs/source/api.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 python_ulid-2.6.0/docs/source/changelog.rst
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 python_ulid-2.6.0/docs/source/conf.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 python_ulid-2.6.0/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 python_ulid-2.6.0/tests/test_base32.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 python_ulid-2.6.0/tests/test_cli.py
+-rw-r--r--   0        0        0     6070 2020-02-02 00:00:00.000000 python_ulid-2.6.0/tests/test_ulid.py
+-rw-r--r--   0        0        0     9929 2020-02-02 00:00:00.000000 python_ulid-2.6.0/ulid/__init__.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 python_ulid-2.6.0/ulid/__main__.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 python_ulid-2.6.0/ulid/base32.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 python_ulid-2.6.0/ulid/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.6.0/ulid/py.typed
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 python_ulid-2.6.0/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 python_ulid-2.6.0/LICENSE
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 python_ulid-2.6.0/hatch.toml
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 python_ulid-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 python_ulid-2.6.0/PKG-INFO
```

### Comparing `python_ulid-2.5.0/CHANGELOG.rst` & `python_ulid-2.6.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 .. _changelog:
 
 Changelog
 =========
 
 Versions follow `Semantic Versioning <http://www.semver.org>`_
 
+`2.6.0`_ - 2024-05-26
+---------------------
+Changed
+~~~~~~~
+* Provide more sophisticated validation when creating ``ULID``s from user input. When using
+  ``ULID.from_str`` we will check if the characters match the base32 alphabet. In general, it is
+  ensured that the timestamp part of the ULID is not out of range.
+
 `2.5.0`_ - 2024-04-26
 ---------------------
 
 Changed
 ~~~~~~~
 * Generate a more accurate JSON schema with Pydantic's ``BaseModel.model_json_schema()``. This
   includes a specification for string and byte representations.
@@ -155,14 +163,15 @@
     >>> ULID().hex
     '0171caa5459a8631a6894d072c8550a8'
 
 * Equality checks and ordering now also work with ``str``-instances.
 * The package now has no external dependencies.
 * The test-coverage has been raised to 100%.
 
+.. _2.6.0: https://github.com/mdomke/python-ulid/compare/2.5.0...2.6.0
 .. _2.5.0: https://github.com/mdomke/python-ulid/compare/2.4.0...2.5.0
 .. _2.4.0: https://github.com/mdomke/python-ulid/compare/2.3.0...2.4.0
 .. _2.3.0: https://github.com/mdomke/python-ulid/compare/2.2.0...2.3.0
 .. _2.2.0: https://github.com/mdomke/python-ulid/compare/2.1.0...2.2.0
 .. _2.1.0: https://github.com/mdomke/python-ulid/compare/2.0.0...2.1.0
 .. _2.0.0: https://github.com/mdomke/python-ulid/compare/1.1.0...2.0.0
 .. _1.1.0: https://github.com/mdomke/python-ulid/compare/1.0.3...1.1.0
```

### Comparing `python_ulid-2.5.0/README.rst` & `python_ulid-2.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `python_ulid-2.5.0/logo.png` & `python_ulid-2.6.0/logo.png`

 * *Files identical despite different names*

### Comparing `python_ulid-2.5.0/.github/workflows/lint-and-test.yml` & `python_ulid-2.6.0/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `python_ulid-2.5.0/.github/workflows/publish.yml` & `python_ulid-2.6.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `python_ulid-2.5.0/docs/Makefile` & `python_ulid-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_ulid-2.5.0/docs/source/conf.py` & `python_ulid-2.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.5.0/docs/source/index.rst` & `python_ulid-2.6.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `python_ulid-2.5.0/tests/test_base32.py` & `python_ulid-2.6.0/tests/test_base32.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.5.0/tests/test_cli.py` & `python_ulid-2.6.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.5.0/tests/test_ulid.py` & `python_ulid-2.6.0/tests/test_ulid.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,23 +145,25 @@
 
 Params = Union[bytes, str, int, float]
 
 
 @pytest.mark.parametrize(
     ("constructor", "value"),
     [
-        (ULID, b"sdf"),
-        (ULID.from_timestamp, b"not-a-timestamp"),
-        (ULID.from_datetime, time.time()),
-        (ULID.from_bytes, b"not-enough"),
-        (ULID.from_bytes, 123),
-        (ULID.from_str, "not-enough"),
-        (ULID.from_str, 123),
-        (ULID.from_int, "not-an-int"),
-        (ULID.from_uuid, "not-a-uuid"),
+        (ULID, b"sdf"),  # invalid length
+        (ULID.from_timestamp, b"not-a-timestamp"),  # invalid type
+        (ULID.from_datetime, time.time()),  # invalid type
+        (ULID.from_bytes, b"not-enough"),  # invalid length
+        (ULID.from_bytes, 123),  # invalid type
+        (ULID.from_str, "not-enough"),  # invalid length
+        (ULID.from_str, 123),  # inavlid type
+        (ULID.from_str, "notavalidulidnotavalidulid"),  # invalid alphabet
+        (ULID.from_str, "Z" * 26),  # invalid timestamp
+        (ULID.from_int, "not-an-int"),  # invalid type
+        (ULID.from_uuid, "not-a-uuid"),  # invalid type
     ],
 )
 def test_ulid_invalid_input(constructor: Callable[[Params], ULID], value: Params) -> None:
     with pytest.raises(ValueError):  # noqa: PT011
         constructor(value)
```

### Comparing `python_ulid-2.5.0/ulid/__init__.py` & `python_ulid-2.6.0/ulid/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,22 +67,34 @@
     You usually create a new :class:`ULID`-object by calling the default constructor with no
     arguments. In that case it will fill the timestamp part with the current datetime. To encode the
     object you usually convert it to a string:
 
         >>> ulid = ULID()
         >>> str(ulid)
         '01E75PVKXA3GFABX1M1J9NZZNF'
+
+    Args:
+        value (bytes, None):  A sequence of 16 bytes representing an encoded ULID.
+        validate (bool): If set to `True` validate if the timestamp part is valid.
+
+    Raises:
+        ValueError: If the provided value is not a valid encoded ULID.
     """
 
-    def __init__(self, value: bytes | None = None) -> None:
+    def __init__(self, value: bytes | None = None, validate: bool = True) -> None:
         if value is not None and len(value) != constants.BYTES_LEN:
             raise ValueError("ULID has to be exactly 16 bytes long.")
         self.bytes: bytes = (
             value or ULID.from_timestamp(time.time_ns() // constants.NANOSECS_IN_MILLISECS).bytes
         )
+        if value is not None and validate:
+            try:
+                self.datetime  # noqa: B018
+            except ValueError as err:
+                raise ValueError("ULID timestamp is out of range.") from err
 
     @classmethod
     @validate_type(datetime)
     def from_datetime(cls: type[U], value: datetime) -> U:
         """Create a new :class:`ULID`-object from a :class:`datetime`. The timestamp part of the
         `ULID` will be set to the corresponding timestamp of the datetime.
 
@@ -121,15 +133,15 @@
 
         Examples:
 
             >>> from uuid import uuid4
             >>> ULID.from_uuid(uuid4())
             ULID(27Q506DP7E9YNRXA0XVD8Z5YSG)
         """
-        return cls(value.bytes)
+        return cls(value.bytes, validate=False)
 
     @classmethod
     @validate_type(bytes)
     def from_bytes(cls: type[U], bytes_: bytes) -> U:
         """Create a new :class:`ULID`-object from sequence of 16 bytes."""
         return cls(bytes_)
```

### Comparing `python_ulid-2.5.0/ulid/__main__.py` & `python_ulid-2.6.0/ulid/__main__.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.5.0/ulid/base32.py` & `python_ulid-2.6.0/ulid/base32.py`

 * *Files 5% similar despite different names*

```diff
@@ -194,14 +194,16 @@
         ]
     )
 
 
 def decode(encoded: str) -> bytes:
     if len(encoded) != constants.REPR_LEN:
         raise ValueError("Encoded ULID has to be exactly 26 characters long.")
+    if any((c not in ENCODE) for c in encoded):
+        raise ValueError(f"Encoded ULID can only consist of letters in {ENCODE}.")
     return decode_timestamp(encoded[: constants.TIMESTAMP_REPR_LEN]) + decode_randomness(
         encoded[constants.TIMESTAMP_REPR_LEN :]
     )
 
 
 def decode_timestamp(encoded: str) -> bytes:
     if len(encoded) != constants.TIMESTAMP_REPR_LEN:
```

### Comparing `python_ulid-2.5.0/LICENSE` & `python_ulid-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ulid-2.5.0/hatch.toml` & `python_ulid-2.6.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `python_ulid-2.5.0/pyproject.toml` & `python_ulid-2.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_ulid-2.5.0/PKG-INFO` & `python_ulid-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-ulid
-Version: 2.5.0
+Version: 2.6.0
 Summary: Universally unique lexicographically sortable identifier
 Project-URL: Homepage, https://github.com/mdomke/python-ulid
 Project-URL: Documentation, https://python-ulid.readthedocs.io
 Project-URL: Changelog, https://python-ulid.readthedocs.io/en/latest/changelog.html
 Project-URL: Issues, https://github.com/mdomke/python-ulid/issues
 Project-URL: CI, https://github.com/mdomke/python-ulid/actions
 Project-URL: Repository, https://github.com/mdomke/python-ulid
```

