# Comparing `tmp/imas_tools-0.4.5.tar.gz` & `tmp/imas_tools-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imas_tools-0.4.5.tar", max compression
+gzip compressed data, was "imas_tools-0.4.6.tar", max compression
```

## Comparing `imas_tools-0.4.5.tar` & `imas_tools-0.4.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.4.5/imas_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 13:36:34.820658 imas_tools-0.4.5/imas_tools/portal/__init__.py
--rw-r--r--   0        0        0     4772 2024-04-19 15:23:32.617350 imas_tools-0.4.5/imas_tools/portal/article.py
--rw-r--r--   0        0        0     2363 2024-04-18 15:56:10.247192 imas_tools-0.4.5/imas_tools/portal/interfaces.py
--rw-r--r--   0        0        0     4126 2024-04-13 12:27:59.670781 imas_tools-0.4.5/imas_tools/recochoku.py
--rw-r--r--   0        0        0        0 2024-05-20 16:09:08.603881 imas_tools-0.4.5/imas_tools/story/__init__.py
--rw-r--r--   0        0        0     2889 2024-05-23 14:43:59.886176 imas_tools-0.4.5/imas_tools/story/adapter.py
--rw-r--r--   0        0        0     2673 2024-05-23 14:04:07.150308 imas_tools-0.4.5/imas_tools/story/gakuen_parser.py
--rw-r--r--   0        0        0     1842 2024-05-23 14:32:30.221320 imas_tools-0.4.5/imas_tools/story/story_csv.py
--rw-r--r--   0        0        0      517 2024-05-23 15:15:28.635463 imas_tools-0.4.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.4.5/README.md
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 imas_tools-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.4.6/imas_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:36:34.820658 imas_tools-0.4.6/imas_tools/portal/__init__.py
+-rw-r--r--   0        0        0     4772 2024-04-19 15:23:32.617350 imas_tools-0.4.6/imas_tools/portal/article.py
+-rw-r--r--   0        0        0     2363 2024-04-18 15:56:10.247192 imas_tools-0.4.6/imas_tools/portal/interfaces.py
+-rw-r--r--   0        0        0     4126 2024-04-13 12:27:59.670781 imas_tools-0.4.6/imas_tools/recochoku.py
+-rw-r--r--   0        0        0        0 2024-05-20 16:09:08.603881 imas_tools-0.4.6/imas_tools/story/__init__.py
+-rw-r--r--   0        0        0     3617 2024-05-26 09:23:47.755662 imas_tools-0.4.6/imas_tools/story/adapter.py
+-rw-r--r--   0        0        0     2673 2024-05-23 14:04:07.150308 imas_tools-0.4.6/imas_tools/story/gakuen_parser.py
+-rw-r--r--   0        0        0     2508 2024-05-26 04:31:48.152566 imas_tools-0.4.6/imas_tools/story/story_csv.py
+-rw-r--r--   0        0        0      517 2024-05-26 09:37:20.949793 imas_tools-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.4.6/README.md
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 imas_tools-0.4.6/PKG-INFO
```

### Comparing `imas_tools-0.4.5/imas_tools/portal/article.py` & `imas_tools-0.4.6/imas_tools/portal/article.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.4.5/imas_tools/portal/interfaces.py` & `imas_tools-0.4.6/imas_tools/portal/interfaces.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.4.5/imas_tools/recochoku.py` & `imas_tools-0.4.6/imas_tools/recochoku.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.4.5/imas_tools/story/adapter.py` & `imas_tools-0.4.6/imas_tools/story/adapter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,50 @@
 from typing import Callable, Optional, Union
 from .gakuen_parser import parse_messages, encode_messages
 from .story_csv import StoryCsv
 
 
 def gakuen_txt_to_sc_csv(gakuen_txt: str, txt_name_without_ext: str) -> str:
     parsed = parse_messages(gakuen_txt)
-    sc_csv = "id,name,text,trans\n"
+    sc_csv = StoryCsv.new_empty_csv(f"{txt_name_without_ext}.txt")
     for line in parsed:
         if line["__tag__"] == "message":
-            if line.get("text"):
-                sc_csv += f"0000000000000,{line.get('name')},{line['text']},\n"
+            if line.get("text") is not None and line.get("name") is not None:
+                sc_csv.append_line(
+                    {
+                        "id": "0000000000000",
+                        "name": line.get("name"),
+                        "text": line.get("text"),
+                        "trans": "",
+                    } # type: ignore
+                )
         if line["__tag__"] == "choicegroup":
             if isinstance(line["choices"], list):
                 for choice in line["choices"]:
-                    sc_csv += f"select,,{choice['text']},\n"
+                    sc_csv.append_line(
+                        {
+                            "id": "select",
+                            "name": "",
+                            "text": choice["text"],
+                            "trans": "",
+                        }
+                    )
             elif isinstance(line["choices"], dict):
-                sc_csv += f"select,,{line['choices']['text']},\n"
+                sc_csv.append_line(
+                    {
+                        "id": "select",
+                        "name": "",
+                        "text": line["choices"]["text"],
+                        "trans": "",
+                    }
+                )
             else:
                 raise ValueError(f"Unknown choice type: {line['choices']}")
-    sc_csv += f"info,{txt_name_without_ext}.txt,,\n"
-    sc_csv += f"译者,,,\n"
-    return sc_csv
+
+    return str(sc_csv)
 
 
 def trivial_translation_merger(
     original_text: str,
     translated_text: str,
     validation_original_text: Optional[str] = None,
 ):
@@ -44,15 +64,17 @@
     translated_text: str,
     validation_original_text: Optional[str] = None,
 ):
     raise NotImplementedError
 
 
 def merge_translated_csv_into_txt(
-    csv_text: Union[str, list[str]], gakuen_txt: str, merger: Callable[[str, str, Optional[str]], str]
+    csv_text: Union[str, list[str]],
+    gakuen_txt: str,
+    merger: Callable[[str, str, Optional[str]], str],
 ) -> str:
     story_csv = StoryCsv(csv_text)
     parsed = parse_messages(gakuen_txt)
     iterator = iter(story_csv.data)
 
     for line in parsed:
         if line["__tag__"] == "message":
@@ -65,13 +87,14 @@
             if isinstance(line["choices"], list):
                 for choice in line["choices"]:
                     next_csv_line = next(iterator)
                     choice["text"] = merger(
                         choice["text"], next_csv_line["trans"], next_csv_line["text"]
                     )
             elif isinstance(line["choices"], dict):
+                next_csv_line = next(iterator)
                 line["choices"]["text"] = merger(
                     line["choices"]["text"],
                     next_csv_line["trans"],
                     next_csv_line["text"],
                 )
     return encode_messages(parsed)
```

### Comparing `imas_tools-0.4.5/imas_tools/story/gakuen_parser.py` & `imas_tools-0.4.6/imas_tools/story/gakuen_parser.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.4.5/pyproject.toml` & `imas_tools-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imas-tools"
-version = "0.4.5"
+version = "0.4.6"
 description = ""
 authors = ["darwintree <17946284+darwintree@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 beautifulsoup4 = "^4.12.3"
```

### Comparing `imas_tools-0.4.5/PKG-INFO` & `imas_tools-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imas-tools
-Version: 0.4.5
+Version: 0.4.6
 Summary: 
 Author: darwintree
 Author-email: 17946284+darwintree@users.noreply.github.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

