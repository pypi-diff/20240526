# Comparing `tmp/xarizmi-0.3.1.tar.gz` & `tmp/xarizmi-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarizmi-0.3.1.tar", last modified: Tue May 21 00:07:23 2024, max compression
+gzip compressed data, was "xarizmi-0.3.2.tar", last modified: Sun May 26 06:56:10 2024, max compression
```

## Comparing `xarizmi-0.3.1.tar` & `xarizmi-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-21 00:07:23.516584 xarizmi-0.3.1/
--rw-r--r--   0 javad      (501) staff       (20)    11345 2024-05-19 03:25:40.000000 xarizmi-0.3.1/LICENSE
--rw-r--r--   0 javad      (501) staff       (20)      760 2024-05-21 00:07:23.516502 xarizmi-0.3.1/PKG-INFO
--rw-r--r--   0 javad      (501) staff       (20)      377 2024-05-21 00:05:39.000000 xarizmi-0.3.1/README.md
--rw-r--r--   0 javad      (501) staff       (20)       30 2024-05-19 03:25:40.000000 xarizmi-0.3.1/pyproject.toml
--rw-r--r--   0 javad      (501) staff       (20)      280 2024-05-21 00:07:23.516844 xarizmi-0.3.1/setup.cfg
--rw-r--r--   0 javad      (501) staff       (20)      849 2024-05-19 07:14:04.000000 xarizmi-0.3.1/setup.py
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-21 00:07:23.515266 xarizmi-0.3.1/tests/
--rw-r--r--   0 javad      (501) staff       (20)     2175 2024-05-21 00:04:22.000000 xarizmi-0.3.1/tests/test_candlestick.py
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-21 00:07:23.515599 xarizmi-0.3.1/xarizmi/
--rw-r--r--   0 javad      (501) staff       (20)       22 2024-05-21 00:05:09.000000 xarizmi-0.3.1/xarizmi/__init__.py
--rw-r--r--   0 javad      (501) staff       (20)      426 2024-05-21 00:01:04.000000 xarizmi-0.3.1/xarizmi/candlestick.py
--rw-r--r--   0 javad      (501) staff       (20)     1339 2024-05-21 00:00:36.000000 xarizmi-0.3.1/xarizmi/enums.py
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-21 00:07:23.516277 xarizmi-0.3.1/xarizmi.egg-info/
--rw-r--r--   0 javad      (501) staff       (20)      760 2024-05-21 00:07:23.000000 xarizmi-0.3.1/xarizmi.egg-info/PKG-INFO
--rw-r--r--   0 javad      (501) staff       (20)      261 2024-05-21 00:07:23.000000 xarizmi-0.3.1/xarizmi.egg-info/SOURCES.txt
--rw-r--r--   0 javad      (501) staff       (20)        1 2024-05-21 00:07:23.000000 xarizmi-0.3.1/xarizmi.egg-info/dependency_links.txt
--rw-r--r--   0 javad      (501) staff       (20)        8 2024-05-21 00:07:23.000000 xarizmi-0.3.1/xarizmi.egg-info/top_level.txt
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-26 06:56:10.105701 xarizmi-0.3.2/
+-rw-r--r--   0 javad      (501) staff       (20)    11345 2024-05-19 03:25:40.000000 xarizmi-0.3.2/LICENSE
+-rw-r--r--   0 javad      (501) staff       (20)      760 2024-05-26 06:56:10.105625 xarizmi-0.3.2/PKG-INFO
+-rw-r--r--   0 javad      (501) staff       (20)      377 2024-05-21 00:05:39.000000 xarizmi-0.3.2/README.md
+-rw-r--r--   0 javad      (501) staff       (20)       30 2024-05-19 03:25:40.000000 xarizmi-0.3.2/pyproject.toml
+-rw-r--r--   0 javad      (501) staff       (20)      280 2024-05-26 06:56:10.105956 xarizmi-0.3.2/setup.cfg
+-rw-r--r--   0 javad      (501) staff       (20)      849 2024-05-19 07:14:04.000000 xarizmi-0.3.2/setup.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-26 06:56:10.103690 xarizmi-0.3.2/tests/
+-rw-r--r--   0 javad      (501) staff       (20)     3298 2024-05-26 06:53:42.000000 xarizmi-0.3.2/tests/test_candlestick.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-26 06:56:10.104042 xarizmi-0.3.2/xarizmi/
+-rw-r--r--   0 javad      (501) staff       (20)       22 2024-05-26 06:54:57.000000 xarizmi-0.3.2/xarizmi/__init__.py
+-rw-r--r--   0 javad      (501) staff       (20)      933 2024-05-26 06:44:40.000000 xarizmi-0.3.2/xarizmi/candlestick.py
+-rw-r--r--   0 javad      (501) staff       (20)     1339 2024-05-21 00:00:36.000000 xarizmi-0.3.2/xarizmi/enums.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-26 06:56:10.104728 xarizmi-0.3.2/xarizmi/mctools/
+-rw-r--r--   0 javad      (501) staff       (20)        0 2024-05-25 06:00:01.000000 xarizmi-0.3.2/xarizmi/mctools/__init__.py
+-rw-r--r--   0 javad      (501) staff       (20)      412 2024-05-26 00:06:22.000000 xarizmi-0.3.2/xarizmi/mctools/candlestick.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-26 06:56:10.105243 xarizmi-0.3.2/xarizmi/models/
+-rw-r--r--   0 javad      (501) staff       (20)        0 2024-05-25 05:06:36.000000 xarizmi-0.3.2/xarizmi/models/__init__.py
+-rw-r--r--   0 javad      (501) staff       (20)     1308 2024-05-26 06:28:26.000000 xarizmi-0.3.2/xarizmi/models/actors.py
+-rw-r--r--   0 javad      (501) staff       (20)      132 2024-05-25 05:39:20.000000 xarizmi-0.3.2/xarizmi/models/currency.py
+-rw-r--r--   0 javad      (501) staff       (20)     1821 2024-05-25 05:49:07.000000 xarizmi-0.3.2/xarizmi/models/symbol.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-26 06:56:10.105402 xarizmi-0.3.2/xarizmi.egg-info/
+-rw-r--r--   0 javad      (501) staff       (20)      760 2024-05-26 06:56:10.000000 xarizmi-0.3.2/xarizmi.egg-info/PKG-INFO
+-rw-r--r--   0 javad      (501) staff       (20)      424 2024-05-26 06:56:10.000000 xarizmi-0.3.2/xarizmi.egg-info/SOURCES.txt
+-rw-r--r--   0 javad      (501) staff       (20)        1 2024-05-26 06:56:10.000000 xarizmi-0.3.2/xarizmi.egg-info/dependency_links.txt
+-rw-r--r--   0 javad      (501) staff       (20)        8 2024-05-26 06:56:10.000000 xarizmi-0.3.2/xarizmi.egg-info/top_level.txt
```

### Comparing `xarizmi-0.3.1/LICENSE` & `xarizmi-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xarizmi-0.3.1/PKG-INFO` & `xarizmi-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarizmi
-Version: 0.3.1
+Version: 0.3.2
 Summary: Xarizmi (read Khwarizmi) project is an educational project thatcontains tools for technical analysis in Python.
 Home-page: https://github.com/javadebadi/xarizmi
 Author: Javad Ebadi
 Author-email: javad@javadebadi.com
 License: Apache 2.0
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `xarizmi-0.3.1/setup.py` & `xarizmi-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `xarizmi-0.3.1/tests/test_candlestick.py` & `xarizmi-0.3.2/tests/test_candlestick.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,39 +8,69 @@
 class TestCandlestick:
     def test(self) -> None:
         data = {
             "close": 2.5,
             "open": 1,
             "low": 0.5,
             "high": 3,
+            "volume": 100,
+            "amount": 150,
         }
         candle = Candlestick(**data)
         assert candle.close == 2.5
         assert candle.open == 1
         assert candle.low == 0.5
         assert candle.high == 3
+        assert candle.range == 2.5
 
         assert candle.model_dump() == pytest.approx(
             {
                 "close": 2.5,
                 "open": 1,
                 "low": 0.5,
                 "high": 3,
                 "interval_type": None,
                 "interval": None,
+                "symbol": None,
+                "volume": 100,
+                "amount": 150,
             }
         )
 
+    def test_intrinsic_rang(self) -> None:
+        zero_data = {
+            "close": 0,
+            "open": 0,
+            "low": 0,
+            "high": 0,
+            "volume": 0,
+            "amount": 0,
+        }
+        candle = Candlestick(**zero_data)
+        assert candle.intrinsic_range == 0
+        data = {
+            "close": 2.5,
+            "open": 1,
+            "low": 0.5,
+            "high": 3,
+            "volume": 100,
+            "amount": 150,
+        }
+        candle = Candlestick(**data)
+        assert candle.intrinsic_range == 2.5 / 3.5
+
     def test_negative_price(self) -> None:
         # Given a data with negative price
         data = {
             "close": -2.5,
             "open": 1,
             "low": 0.5,
             "high": 3,
+            "volume": 100,
+            "amount": 150,
         }
         # When Candlestick constructor is called
         # Then I should see ValidationError
         with pytest.raises(ValidationError):
             Candlestick(**data)
 
 
@@ -52,30 +82,39 @@
                 {
                     "low": 0.61873,
                     "high": 0.727,
                     "close": 0.714,
                     "open": 0.71075,
                     "interval_type": "1week",
                     "interval": 604800,
+                    "symbol": None,
+                    "volume": 100,
+                    "amount": 150,
                 },
                 {
                     "low": 0.65219,
                     "high": 0.75,
                     "close": 0.70238,
                     "open": 0.71075,
                     "interval_type": "1week",
                     "interval": 604800,
+                    "symbol": None,
+                    "volume": 100,
+                    "amount": 150,
                 },
                 {
                     "low": 0.64801,
                     "high": 0.92,
                     "close": 0.8404,
                     "open": 0.70238,
                     "interval_type": "1week",
                     "interval": 604800,
+                    "symbol": None,
+                    "volume": 100,
+                    "amount": 150,
                 },
             ]
         }
 
         chart = CandlestickChart(**data)
 
         assert chart.model_dump() == pytest.approx(data)
```

### Comparing `xarizmi-0.3.1/xarizmi/enums.py` & `xarizmi-0.3.2/xarizmi/enums.py`

 * *Files identical despite different names*

### Comparing `xarizmi-0.3.1/xarizmi.egg-info/PKG-INFO` & `xarizmi-0.3.2/xarizmi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarizmi
-Version: 0.3.1
+Version: 0.3.2
 Summary: Xarizmi (read Khwarizmi) project is an educational project thatcontains tools for technical analysis in Python.
 Home-page: https://github.com/javadebadi/xarizmi
 Author: Javad Ebadi
 Author-email: javad@javadebadi.com
 License: Apache 2.0
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

