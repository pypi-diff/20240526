# Comparing `tmp/yandex_query_magic-0.1.7.tar.gz` & `tmp/yandex_query_magic-0.1.8.tar.gz`

## Comparing `yandex_query_magic-0.1.7.tar` & `yandex_query_magic-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0   157105 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/screenshot.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/src/yandex_query_magic/__init__.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/src/yandex_query_magic/ipythondisplay.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/src/yandex_query_magic/jinja_template.py
--rw-r--r--   0        0        0    13597 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/src/yandex_query_magic/magics.py
--rw-r--r--   0        0        0    12205 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/src/yandex_query_magic/main.py
--rw-r--r--   0        0        0     9729 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/src/yandex_query_magic/query_results.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/src/yandex_query_magic/sqltext_parser.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/src/yandex_query_magic/yq_results.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/tests/test_formats.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/tests/test_jinja2.py
--rw-r--r--   0        0        0    25037 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/tests/test_main.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/tests/test_sqlparser.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/LICENSE.md
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/README.md
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0   157105 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/screenshot.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/src/yandex_query_magic/__init__.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/src/yandex_query_magic/ipythondisplay.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/src/yandex_query_magic/jinja_template.py
+-rw-r--r--   0        0        0    13648 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/src/yandex_query_magic/magics.py
+-rw-r--r--   0        0        0    12205 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/src/yandex_query_magic/main.py
+-rw-r--r--   0        0        0     9729 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/src/yandex_query_magic/query_results.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/src/yandex_query_magic/sqltext_parser.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/src/yandex_query_magic/yq_results.py
+-rw-r--r--   0        0        0    21582 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/tests/Untitled.ipynb
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/tests/test_formats.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/tests/test_jinja2.py
+-rw-r--r--   0        0        0    25037 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/tests/test_main.py
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/tests/test_sqlparser.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/tests/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/README.md
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 yandex_query_magic-0.1.8/PKG-INFO
```

### Comparing `yandex_query_magic-0.1.7/screenshot.png` & `yandex_query_magic-0.1.8/screenshot.png`

 * *Files identical despite different names*

### Comparing `yandex_query_magic-0.1.7/src/yandex_query_magic/jinja_template.py` & `yandex_query_magic-0.1.8/src/yandex_query_magic/jinja_template.py`

 * *Files identical despite different names*

### Comparing `yandex_query_magic-0.1.7/src/yandex_query_magic/magics.py` & `yandex_query_magic-0.1.8/src/yandex_query_magic/magics.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,21 +242,20 @@
 
         if result is not None:
             if as_dataframe:
                 result = result.to_dataframes(None)
                 if not all_results:
                     if isinstance(result, list):
                         if len(result) > 1:
-                            several_datasets_label.value = f"{len(result)} result sets returned. Displaying first one"
+                            several_datasets_label.value = f"{len(result)} result sets returned. Displaying first one. " \
+                                                            "Use --all-results to get all result sets"
                             several_datasets_label.layout.display = 'block'
 
                         if len(result) >= 1:
                             result = result[0]
-                else:
-                    return result
             else:
                 result = result.raw_results
 
         # Write results to external variable
         if variable is not None:
             self.shell.user_ns[variable] = result
             return result
```

### Comparing `yandex_query_magic-0.1.7/src/yandex_query_magic/main.py` & `yandex_query_magic-0.1.8/src/yandex_query_magic/main.py`

 * *Files identical despite different names*

### Comparing `yandex_query_magic-0.1.7/src/yandex_query_magic/query_results.py` & `yandex_query_magic-0.1.8/src/yandex_query_magic/query_results.py`

 * *Files identical despite different names*

### Comparing `yandex_query_magic-0.1.7/src/yandex_query_magic/sqltext_parser.py` & `yandex_query_magic-0.1.8/src/yandex_query_magic/sqltext_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,18 +107,20 @@
         key_types = set()
         value_types = set()
         for key, value in dict_value.items():
             key_types.add(type(key))
             value_types.add(type(value))
 
         if len(key_types) > 1:
-            raise Exception(f"All key types must be of one type. Found several {key_types}")
+            raise Exception(f"All key types must be of one type. "
+                            f"Found several {sorted([str(key_type) for key_type in key_types])}")
 
         if len(value_types) > 1:
-            raise Exception(f"All value types must be of one type. Found several {value_types}")
+            raise Exception(f"All value types must be of one type. "
+                            f"Found several {sorted([str(value_type) for value_type in value_types])}")
 
         for key, value in dict_value.items():
             key = SqlParser.render_value(key)
             value = SqlParser.render_value(value)
 
             as_dict_cols.append(f"asTuple({key}, {value})")
```

### Comparing `yandex_query_magic-0.1.7/src/yandex_query_magic/yq_results.py` & `yandex_query_magic-0.1.8/src/yandex_query_magic/yq_results.py`

 * *Files identical despite different names*

### Comparing `yandex_query_magic-0.1.7/tests/test_formats.py` & `yandex_query_magic-0.1.8/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `yandex_query_magic-0.1.7/tests/test_jinja2.py` & `yandex_query_magic-0.1.8/tests/test_jinja2.py`

 * *Files identical despite different names*

### Comparing `yandex_query_magic-0.1.7/tests/test_main.py` & `yandex_query_magic-0.1.8/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `yandex_query_magic-0.1.7/tests/test_sqlparser.py` & `yandex_query_magic-0.1.8/tests/test_sqlparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from yandex_query_magic import SqlParser
 import pandas as pd
 from datetime import datetime
 import pytest
+import re
 
 
 def test_sqlrender_noop():
     test_str = "select * from a"
     parser = SqlParser()
     assert parser.reformat("select * from a", {}) == test_str
 
@@ -70,25 +71,25 @@
     parser = SqlParser()
     formatted = parser.reformat(test_str, {"a": a})
     print(formatted)
     assert formatted == 'select DictHasItems(ToDict(AsList(asTuple("a", 1l),asTuple("b", 2l),asTuple("c", 3l))))'  # noqa
 
 
 def test_sqlrender_dict_distinct_value():
-    with pytest.raises(Exception, match="All value types must be of one type. Found several {<class 'datetime.datetime'>, <class 'str'>, <class 'int'>, <class 'float'>}"):  # noqa
+    with pytest.raises(Exception, match=re.escape("All value types must be of one type. Found several [\"<class 'datetime.datetime'>\", \"<class 'float'>\", \"<class 'int'>\", \"<class 'str'>\"]")):  # noqa
         test_str = "select * from {{a}}"
         a = {"a": 1, "b": 2.0, "c": "test", "d": datetime(2022, 2, 2, 21, 12, 12)}
         parser = SqlParser()
         formatted = parser.reformat(test_str, {"a": a})
         print(formatted)
         assert formatted == 'select * from AS_TABLE(AsList(AsStruct(1l as `a`,2.0 as `b`,"test" as `c`,DateTime::MakeTimestamp(DateTime::Parse("%Y-%m-%d %H:%M:%S")("2022-02-02 21:12:12.000000")) as `d`))) as `a`'  # noqa
 
 
 def test_sqlrender_dict_distinct_keys():
-    with pytest.raises(Exception, match="All key types must be of one type. Found several {<class 'str'>, <class 'datetime.datetime'>}"):  # noqa
+    with pytest.raises(Exception, match=re.escape("All key types must be of one type. Found several [\"<class 'datetime.datetime'>\", \"<class 'str'>\"]")):  # noqa
         test_str = "select * from {{a}}"
         a = {"a": 1, "b": 1, "c": 1, datetime.now(): 1}
         parser = SqlParser()
         formatted = parser.reformat(test_str, {"a": a})
         print(formatted)
         assert formatted == 'select * from AS_TABLE(AsList(AsStruct(1l as `a`,2.0 as `b`,"test" as `c`,DateTime::MakeTimestamp(DateTime::Parse("%Y-%m-%d %H:%M:%S")("2022-02-02 21:12:12.000000")) as `d`))) as `a`'  # noqa
```

### Comparing `yandex_query_magic-0.1.7/LICENSE.md` & `yandex_query_magic-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yandex_query_magic-0.1.7/README.md` & `yandex_query_magic-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `yandex_query_magic-0.1.7/pyproject.toml` & `yandex_query_magic-0.1.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "yandex-query-magic"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { email="cloud@support.yandex.ru" },
 ]
 description = "The Yandex Query official Jupyter Notebook plugin"
 readme = "README.md"
 license="MIT"
 requires-python = ">=3.10"
```

### Comparing `yandex_query_magic-0.1.7/PKG-INFO` & `yandex_query_magic-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: yandex-query-magic
-Version: 0.1.7
+Version: 0.1.8
 Summary: The Yandex Query official Jupyter Notebook plugin
 Project-URL: Homepage, https://github.com/yandex-cloud/yandex-query-magics
 Project-URL: Issues, https://github.com/yandex-cloud/yandex-query-magics/issues
 Author-email: cloud@support.yandex.ru
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
```

