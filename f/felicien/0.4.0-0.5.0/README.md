# Comparing `tmp/felicien-0.4.0.tar.gz` & `tmp/felicien-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felicien-0.4.0.tar", max compression
+gzip compressed data, was "felicien-0.5.0.tar", max compression
```

## Comparing `felicien-0.4.0.tar` & `felicien-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1095 2024-04-25 22:03:26.094113 felicien-0.4.0/LICENSE
--rw-r--r--   0        0        0     2558 2024-04-25 22:03:26.094113 felicien-0.4.0/README.md
--rw-r--r--   0        0        0      142 2024-04-25 22:03:26.099113 felicien-0.4.0/felicien/__init__.py
--rw-r--r--   0        0        0     6409 2024-04-25 22:03:26.099113 felicien-0.4.0/felicien/feliconnector.py
--rw-r--r--   0        0        0    10153 2024-04-25 22:03:26.099113 felicien-0.4.0/felicien/felits.py
--rw-r--r--   0        0        0      999 2024-04-25 22:03:26.100113 felicien-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 felicien-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-26 15:49:47.210403 felicien-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2599 2024-05-26 15:49:47.210403 felicien-0.5.0/README.md
+-rw-r--r--   0        0        0      142 2024-05-26 15:49:47.216403 felicien-0.5.0/felicien/__init__.py
+-rw-r--r--   0        0        0     6505 2024-05-26 15:49:47.216403 felicien-0.5.0/felicien/feliconnector.py
+-rw-r--r--   0        0        0    12839 2024-05-26 15:49:47.216403 felicien-0.5.0/felicien/felits.py
+-rw-r--r--   0        0        0     1067 2024-05-26 15:49:47.217403 felicien-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 felicien-0.5.0/PKG-INFO
```

### Comparing `felicien-0.4.0/LICENSE` & `felicien-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `felicien-0.4.0/README.md` & `felicien-0.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -67,11 +67,12 @@
 - Connect to a TSDB, and check connectivity
 - Get a timeserie and store it in a Pandas Series
 - Estimate frequency of a timeserie
 - Trim a timeserie by date or by size
 - Transform the timeserie in a pandas.DataFrame
 - Delete a timeserie in a TSDB
 - Import a timeserie into a TSDB
+- Normalize a timeserie on its frequency
 
 ## License
 
 [MIT](LICENSE)
```

### Comparing `felicien-0.4.0/felicien/feliconnector.py` & `felicien-0.5.0/felicien/feliconnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
                 else:
                     raise KeyError(f"{k} is an invalid option for requests")
 
         # test connection to the TSDB
         r = requests.get(
             f"{self.base_url}/{API_TSDB_HEALTH[self.tsdb]}",
             **self._options,  # type: ignore
+            timeout=60,
         )
         if not (r.status_code == 200 and r.json().get("status") == "success"):
             raise ConnectionError(f"unable to reach TSDB API: {r.status_code}")
 
     def __repr__(self) -> str:
         return f"FeliConnector([{self.tsdb}]{{{self.base_url}}})"
 
@@ -127,14 +128,15 @@
         """
         payload = {"query": metric}
 
         r = requests.get(
             f"{self.base_url}/{API_TSDB_QUERY[self.tsdb]}",
             **self._options,  # type: ignore
             params=payload,
+            timeout=60,
         )
         if not (r.status_code == 200 and r.json().get("status") == "success"):
             raise ConnectionError(f"unable to get timeserie: {r.status_code}")
 
         # connection is successful
         if len(r.json().get("data", {}).get("result")) > 1:
             raise OverflowError("query returns more than one timeserie")
@@ -170,14 +172,15 @@
         method = "GET" if self.tsdb == "victoriametrics" else "POST"
 
         r = requests.request(
             method=method,
             url=f"{self.base_url}/{API_TSDB_QUERY[self.tsdb]}",
             params=payload,
             **self._options,  # type: ignore
+            timeout=60,
         )
         if not r.status_code == 204:
             raise ConnectionError(
                 f"unable to delete timeserie: {r.status_code}"
             )
 
         return True
@@ -196,14 +199,15 @@
         """
         payload = ts.as_prometheus()
 
         r = requests.post(
             url=f"{self.base_url}/{API_TSDB_IMPORT[self.tsdb]}",
             data=payload,
             **self._options,  # type: ignore
+            timeout=60,
         )
         if r.status_code not in [200, 204]:
             raise ConnectionError(
                 f"unable to import timeserie: {r.status_code}"
             )
 
         return True
```

### Comparing `felicien-0.4.0/felicien/felits.py` & `felicien-0.5.0/felicien/felits.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
 
 import pandas as pd
+import itertools
 import datetime as dt
 import matplotlib.pyplot as plt
 import json
 
 
 # Smallest frequency should be seen at least 10% of the Serie to be considered
 # as the Serie frequency
@@ -166,15 +167,15 @@
         elif frequencies.size > 1:
             # multiple frequencies: return the lowest one that is occuring
             # more than 10% of the time
             for i in range(frequencies.size):
                 if (frequencies / self.data.size).sort_index().iloc[
                     i
                 ] > MIN_FREQUENCY_REPRESENTATION:
-                    return frequencies[i:].idxmax()
+                    return frequencies[i:].sort_index().idxmax()
 
         # all other cases seem wrong
         return dt.timedelta()
 
     @property
     def size(self) -> int:
         """Expose the size to the timeseries
@@ -303,7 +304,81 @@
             label=self.name,
             linestyle="solid",
         )
         plt.xticks(rotation=60, fontsize=10)
         plt.title(f"{self.name}{{{self.labels_string}}}")
         plt.show()
         plt.close()
+
+    def normalize(self, inplace: bool = False) -> pd.Series:
+        """Normalize the timeserie, filling missing points with NaN values
+        but making sure the index respect the frequency.
+
+        Important: points not aligned on the frequency will be dropped, while
+            missing points on frequency will be added as NaN
+
+        Args:
+            inplace (bool, optional): Control if the trim should be applied
+                to the current object, or just get the trimmed timeserie.
+                Defaults to False.
+
+        Returns:
+            pd.Series: The normalized timeserie
+
+        Raises:
+            ValueError if the timeserie has no frequency (such as single point
+                timeserie)
+
+        """
+        if self.frequency == dt.timedelta():
+            raise ValueError("Can't determine frequency")
+
+        if inplace:
+            self.data = self.data.asfreq(freq=self.frequency)
+            return self.data
+
+        return self.data.asfreq(freq=self.frequency)
+
+    def longest_continuous_segment(self, position: str = "last") -> pd.Series:
+        """Extract the longest continuous segment, which is the longest
+            segment of the timeserie respecting the frequency, without any
+            missing point
+
+        Args:
+            position (str, optional): Which longest segment to return, in case
+                multiple segment exist
+                Defaults to last.
+
+        Returns:
+            pd.Series: the extract of the timeserie
+
+        Raises:
+            ValueError if the position argument is not "first" or "last"
+        """
+        # create an array stating if two points are separated by
+        # exactly 1 frequency
+        segments = self.data.index.diff() == self.frequency  # type: ignore
+
+        # estimate the size of the longest segment
+        longest_length = max(
+            len(list(y)) for (_, y) in itertools.groupby(segments)
+        )
+
+        # finding the position of the longest segment (first or last)
+        start_position = 0
+        cursor = 0
+        for is_freq, segment in itertools.groupby(segments):
+            # case where the frequency matches and the length of
+            # the segment is the longest
+            if is_freq and len(list(segment)) == longest_length:
+                start_position = cursor
+
+                # in case we found the first longest segment
+                if position == "first":
+                    break
+
+            # move current cursor along the serie
+            cursor += len(list(segment))
+
+        return self.data.iloc[
+            start_position - 1 : start_position + longest_length  # noqa E203
+        ]
```

### Comparing `felicien-0.4.0/pyproject.toml` & `felicien-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "felicien"
-version = "0.4.0"
+version = "0.5.0"
 description = "Felicien is you companion to retrieve timeseries from a TSDB, to transform it in various format and to push it to a TSDB."
 authors = ["Julien Andrieux <chilladx@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "felicien" },
 ]
@@ -27,17 +27,22 @@
 safety = "^3.1.0"
 pyflakes = "^3.2.0"
 pytest-cov = "^5.0.0"
 requests-mock = "^1.12.1"
 mypy = "^1.9.0"
 sphinx = "^7.3.7"
 sphinx-rtd-theme = "^2.0.0"
+bandit = "^1.7.8"
+vulture = "^2.11"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 python_version = 3.11
 disallow_untyped_defs = true
 no_implicit_optional = false
-exclude = "tests|docs"
+exclude = "tests|docs"
+
+[tool.black]
+line-length = 79
```

### Comparing `felicien-0.4.0/PKG-INFO` & `felicien-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felicien
-Version: 0.4.0
+Version: 0.5.0
 Summary: Felicien is you companion to retrieve timeseries from a TSDB, to transform it in various format and to push it to a TSDB.
 License: MIT
 Author: Julien Andrieux
 Author-email: chilladx@pm.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -87,12 +87,13 @@
 - Connect to a TSDB, and check connectivity
 - Get a timeserie and store it in a Pandas Series
 - Estimate frequency of a timeserie
 - Trim a timeserie by date or by size
 - Transform the timeserie in a pandas.DataFrame
 - Delete a timeserie in a TSDB
 - Import a timeserie into a TSDB
+- Normalize a timeserie on its frequency
 
 ## License
 
 [MIT](LICENSE)
```

