# Comparing `tmp/quiffen-2.0.8.tar.gz` & `tmp/quiffen-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiffen-2.0.8.tar", max compression
+gzip compressed data, was "quiffen-2.0.9.tar", max compression
```

## Comparing `quiffen-2.0.8.tar` & `quiffen-2.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1074 2023-06-08 20:15:13.884314 quiffen-2.0.8/LICENSE
--rw-r--r--   0        0        0     4192 2023-04-02 10:05:40.430967 quiffen-2.0.8/README.rst
--rw-r--r--   0        0        0     1275 2023-06-23 18:54:34.887773 quiffen-2.0.8/pyproject.toml
--rw-r--r--   0        0        0      837 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/__init__.py
--rw-r--r--   0        0        0     8684 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/account.py
--rw-r--r--   0        0        0     3189 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/base.py
--rw-r--r--   0        0        0    17647 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/category.py
--rw-r--r--   0        0        0     3027 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/class_type.py
--rw-r--r--   0        0        0     7288 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/investment.py
--rw-r--r--   0        0        0    20096 2023-06-23 18:54:18.217776 quiffen-2.0.8/quiffen/core/qif.py
--rw-r--r--   0        0        0     4487 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/security.py
--rw-r--r--   0        0        0     4147 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/split.py
--rw-r--r--   0        0        0    20693 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/transaction.py
--rw-r--r--   0        0        0     4517 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/utils.py
--rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 quiffen-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-19 16:08:49.135723 quiffen-2.0.9/LICENSE
+-rw-r--r--   0        0        0     4192 2023-07-19 16:08:49.135723 quiffen-2.0.9/README.rst
+-rw-r--r--   0        0        0     1275 2023-07-19 17:27:26.880679 quiffen-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-07-19 16:08:49.195723 quiffen-2.0.9/quiffen/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 16:08:49.195723 quiffen-2.0.9/quiffen/core/__init__.py
+-rw-r--r--   0        0        0     8684 2023-07-19 16:08:49.195723 quiffen-2.0.9/quiffen/core/account.py
+-rw-r--r--   0        0        0     3189 2023-07-19 16:08:49.195723 quiffen-2.0.9/quiffen/core/base.py
+-rw-r--r--   0        0        0    17647 2023-07-19 16:08:49.195723 quiffen-2.0.9/quiffen/core/category.py
+-rw-r--r--   0        0        0     3027 2023-07-19 16:08:49.195723 quiffen-2.0.9/quiffen/core/class_type.py
+-rw-r--r--   0        0        0     7288 2023-07-19 16:08:49.195723 quiffen-2.0.9/quiffen/core/investment.py
+-rw-r--r--   0        0        0    20096 2023-07-19 16:08:49.195723 quiffen-2.0.9/quiffen/core/qif.py
+-rw-r--r--   0        0        0     4487 2023-07-19 16:08:49.195723 quiffen-2.0.9/quiffen/core/security.py
+-rw-r--r--   0        0        0     4147 2023-07-19 16:08:49.195723 quiffen-2.0.9/quiffen/core/split.py
+-rw-r--r--   0        0        0    20772 2023-07-19 17:27:26.880679 quiffen-2.0.9/quiffen/core/transaction.py
+-rw-r--r--   0        0        0     4827 2023-07-19 17:27:26.880679 quiffen-2.0.9/quiffen/utils.py
+-rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 quiffen-2.0.9/PKG-INFO
```

### Comparing `quiffen-2.0.8/LICENSE` & `quiffen-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.8/README.rst` & `quiffen-2.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.8/pyproject.toml` & `quiffen-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quiffen"
-version = "2.0.8"
+version = "2.0.9"
 description = "Quiffen"
 authors = ["Isaac Harris-Holt <isaac@harris-holt.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 homepage = "https://github.com/isaacharrisholt/quiffen"
 repository = "https://github.com/isaacharrisholt/quiffen"
 documentation = "https://quiffen.readthedocs.io/en/latest/"
```

### Comparing `quiffen-2.0.8/quiffen/__init__.py` & `quiffen-2.0.9/quiffen/__init__.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.8/quiffen/core/account.py` & `quiffen-2.0.9/quiffen/core/account.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.8/quiffen/core/base.py` & `quiffen-2.0.9/quiffen/core/base.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.8/quiffen/core/category.py` & `quiffen-2.0.9/quiffen/core/category.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.8/quiffen/core/class_type.py` & `quiffen-2.0.9/quiffen/core/class_type.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.8/quiffen/core/investment.py` & `quiffen-2.0.9/quiffen/core/investment.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.8/quiffen/core/qif.py` & `quiffen-2.0.9/quiffen/core/qif.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.8/quiffen/core/security.py` & `quiffen-2.0.9/quiffen/core/security.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.8/quiffen/core/split.py` & `quiffen-2.0.9/quiffen/core/split.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.8/quiffen/core/transaction.py` & `quiffen-2.0.9/quiffen/core/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,26 +384,26 @@
                     logger.warning(
                         f"No split yet given for memo '{field_info}', skipping"
                     )
                 else:
                     current_split.memo = field_info
             elif line_code in {"$", "£"}:
                 if current_split:
-                    current_split.amount = Decimal(field_info.replace(",", ""))
+                    current_split.amount = utils.parse_decimal(field_info)
             elif line_code == "%":
                 if current_split:
-                    current_split.percent = Decimal(
-                        field_info.split(" ")[0].replace("%", "")
+                    current_split.percent = utils.parse_decimal(
+                        field_info.split(" ")[0]
                     )
             elif line_code in {"T", "U"}:
-                amount = field_info.replace(",", "")
+                amount = utils.parse_decimal(field_info)
                 if not splits:
                     kwargs["amount"] = amount
                 elif current_split:
-                    current_split.amount = Decimal(amount)
+                    current_split.amount = amount
             elif line_code == "M":
                 if not splits:
                     kwargs["memo"] = field_info
                 elif current_split:
                     current_split.memo = field_info
             elif line_code == "C":
                 if not splits:
@@ -476,26 +476,28 @@
             else:
                 raise ValueError(f"Unknown line code: {line_code}")
 
         if line_number is not None:
             kwargs["line_number"] = line_number
 
         # Set splits percentage if they don't already have one
-        total = Decimal(kwargs.get("amount", 0))
+        total = utils.parse_decimal(kwargs.get("amount", 0))
         if splits and total:
             for split in splits:
                 if split.percent is None and split.amount is not None:
-                    split.percent = Decimal(round(split.amount / total * 100, 2))
+                    split.percent = utils.parse_decimal(
+                        round(split.amount / total * 100, 2)
+                    )
                 # Check if the split percentage is correct
                 elif (
                     split.percent is not None
                     and split.amount is not None
                     and not (
-                        Decimal(round(split.percent, 2))
-                        == Decimal(
+                        utils.parse_decimal(round(split.percent, 2))
+                        == utils.parse_decimal(
                             round(
                                 split.amount / total * 100,
                                 2,
                             )
                         )
                     )
                 ):
```

### Comparing `quiffen-2.0.8/quiffen/utils.py` & `quiffen-2.0.9/quiffen/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from pydantic import ValidationError, parse_obj_as
 
 from quiffen.core.base import Field
 
 ZERO_SEPARATED_DATE = re.compile(
     r"^(\d{2}|\d{4}|[a-zA-Z]+)0(\d{2}|[a-zA-Z]+)0(\d{2}|\d{4})$",
 )
+INVALID_AMOUNT_CHARACTERS = re.compile(
+    r"[^\d\.-]",
+)
 
 
 def parse_date(date_string: str, day_first: bool = False) -> datetime:
     """Parse a string date of an unknown format and return a datetime object.
 
     Parameters
     ----------
@@ -146,7 +149,14 @@
                 date_format,
                 stringify=True,
             ): apply_csv_formatting_to_container(value, date_format)
             for key, value in obj.items()
         }
     else:
         return apply_csv_formatting_to_scalar(obj, date_format)
+
+
+def parse_decimal(value: Union[str, Decimal]) -> Decimal:
+    """Parse a decimal from a string, removing non-numeric characters."""
+    if isinstance(value, Decimal):
+        return value
+    return Decimal(INVALID_AMOUNT_CHARACTERS.sub("", value))
```

### Comparing `quiffen-2.0.8/PKG-INFO` & `quiffen-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quiffen
-Version: 2.0.8
+Version: 2.0.9
 Summary: Quiffen
 Home-page: https://github.com/isaacharrisholt/quiffen
 License: GPL-3.0-or-later
 Keywords: qif,finance,data processing
 Author: Isaac Harris-Holt
 Author-email: isaac@harris-holt.com
 Requires-Python: >=3.8,<4.0
```

