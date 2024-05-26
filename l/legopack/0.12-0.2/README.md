# Comparing `tmp/legopack-0.12.tar.gz` & `tmp/legopack-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legopack-0.12.tar", last modified: Thu May 23 15:08:15 2024, max compression
+gzip compressed data, was "legopack-0.2.tar", last modified: Sun May 26 16:04:14 2024, max compression
```

## Comparing `legopack-0.12.tar` & `legopack-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-05-23 15:08:15.480304 legopack-0.12/
--rwxrwxrwx   0 remi      (1000) remi      (1000)      257 2024-05-23 15:08:15.478302 legopack-0.12/PKG-INFO
--rwxrwxrwx   0 remi      (1000) remi      (1000)       29 2024-01-24 07:43:04.000000 legopack-0.12/README.md
-drwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-05-23 15:08:15.268394 legopack-0.12/legopack/
--rwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-01-24 07:51:07.000000 legopack-0.12/legopack/__init__.py
-drwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-05-23 15:08:15.452302 legopack-0.12/legopack/models/
--rwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-01-24 08:06:16.000000 legopack-0.12/legopack/models/__init__.py
--rwxrwxrwx   0 remi      (1000) remi      (1000)     2738 2024-03-12 13:16:21.000000 legopack-0.12/legopack/models/adaptators.py
--rwxrwxrwx   0 remi      (1000) remi      (1000)    13272 2024-05-17 15:00:04.000000 legopack-0.12/legopack/models/custom.py
--rwxrwxrwx   0 remi      (1000) remi      (1000)     3907 2024-03-25 10:52:20.000000 legopack-0.12/legopack/tools.py
-drwxrwxrwx   0 remi      (1000) remi      (1000)        0 2024-05-23 15:08:15.352301 legopack-0.12/legopack.egg-info/
--rwxrwxrwx   0 remi      (1000) remi      (1000)      257 2024-05-23 15:08:15.000000 legopack-0.12/legopack.egg-info/PKG-INFO
--rwxrwxrwx   0 remi      (1000) remi      (1000)      331 2024-05-23 15:08:15.000000 legopack-0.12/legopack.egg-info/SOURCES.txt
--rwxrwxrwx   0 remi      (1000) remi      (1000)        1 2024-05-23 15:08:15.000000 legopack-0.12/legopack.egg-info/dependency_links.txt
--rwxrwxrwx   0 remi      (1000) remi      (1000)        1 2024-01-24 08:32:20.000000 legopack-0.12/legopack.egg-info/not-zip-safe
--rwxrwxrwx   0 remi      (1000) remi      (1000)       28 2024-05-23 15:08:15.000000 legopack-0.12/legopack.egg-info/requires.txt
--rwxrwxrwx   0 remi      (1000) remi      (1000)        9 2024-05-23 15:08:15.000000 legopack-0.12/legopack.egg-info/top_level.txt
--rwxrwxrwx   0 remi      (1000) remi      (1000)       38 2024-05-23 15:08:15.481302 legopack-0.12/setup.cfg
--rwxrwxrwx   0 remi      (1000) remi      (1000)      424 2024-05-23 15:06:38.000000 legopack-0.12/setup.py
+drwxr-xr-x   0 zeugy     (1000) users      (100)        0 2024-05-26 16:04:14.150865 legopack-0.2/
+-rw-r--r--   0 zeugy     (1000) users      (100)      182 2024-05-26 16:04:14.150865 legopack-0.2/PKG-INFO
+-rw-r--r--   0 zeugy     (1000) users      (100)       29 2024-05-26 14:58:16.000000 legopack-0.2/README.md
+drwxr-xr-x   0 zeugy     (1000) users      (100)        0 2024-05-26 16:04:14.146865 legopack-0.2/legopack/
+-rw-r--r--   0 zeugy     (1000) users      (100)        0 2024-05-26 14:58:16.000000 legopack-0.2/legopack/__init__.py
+drwxr-xr-x   0 zeugy     (1000) users      (100)        0 2024-05-26 16:04:14.150865 legopack-0.2/legopack/models/
+-rw-r--r--   0 zeugy     (1000) users      (100)        0 2024-05-26 14:58:16.000000 legopack-0.2/legopack/models/__init__.py
+-rw-r--r--   0 zeugy     (1000) users      (100)     3719 2024-05-26 14:57:11.000000 legopack-0.2/legopack/models/adaptators.py
+-rw-r--r--   0 zeugy     (1000) users      (100)    13272 2024-05-26 14:58:16.000000 legopack-0.2/legopack/models/custom.py
+-rw-r--r--   0 zeugy     (1000) users      (100)     3907 2024-05-26 14:58:16.000000 legopack-0.2/legopack/tools.py
+drwxr-xr-x   0 zeugy     (1000) users      (100)        0 2024-05-26 16:04:14.146865 legopack-0.2/legopack.egg-info/
+-rw-r--r--   0 zeugy     (1000) users      (100)      182 2024-05-26 16:04:14.000000 legopack-0.2/legopack.egg-info/PKG-INFO
+-rw-r--r--   0 zeugy     (1000) users      (100)      331 2024-05-26 16:04:14.000000 legopack-0.2/legopack.egg-info/SOURCES.txt
+-rw-r--r--   0 zeugy     (1000) users      (100)        1 2024-05-26 16:04:14.000000 legopack-0.2/legopack.egg-info/dependency_links.txt
+-rw-r--r--   0 zeugy     (1000) users      (100)        1 2024-05-26 14:58:16.000000 legopack-0.2/legopack.egg-info/not-zip-safe
+-rw-r--r--   0 zeugy     (1000) users      (100)       28 2024-05-26 16:04:14.000000 legopack-0.2/legopack.egg-info/requires.txt
+-rw-r--r--   0 zeugy     (1000) users      (100)        9 2024-05-26 16:04:14.000000 legopack-0.2/legopack.egg-info/top_level.txt
+-rw-r--r--   0 zeugy     (1000) users      (100)       38 2024-05-26 16:04:14.150865 legopack-0.2/setup.cfg
+-rw-r--r--   0 zeugy     (1000) users      (100)      628 2024-05-26 16:04:08.000000 legopack-0.2/setup.py
```

### Comparing `legopack-0.12/legopack/models/adaptators.py` & `legopack-0.2/legopack/models/adaptators.py`

 * *Files 11% similar despite different names*

```diff
@@ -68,7 +68,30 @@
                 else:
                     self.predictions.append(False)
             except TypeError:
                 self.predictions.append(False)
             self.anomalies_scores.append(score)
         end = time.perf_counter_ns()
         self.last_inference_time = (end - start) / 1e6 / len(data_to_scores)
+
+
+class HSTreeAdaptator(AbstractAD):
+    def __init__(self, model, high_threshold=85000, low_threshold=1200, initialization: int = 500) -> None:
+        super().__init__(model, initialization)
+        self.high_threshold = high_threshold
+        self.low_threshold = low_threshold
+
+    def update(self, data: np.ndarray):
+        start = time.perf_counter_ns()
+        data_to_scores = data
+        for x in data_to_scores:
+            score = self.model.fit_score(x)
+            try:
+                if (score > self.high_threshold) & (score < self.low_threshold) & (len(self.anomalies_scores) > self.initialization):
+                    self.predictions.append(True)
+                else:
+                    self.predictions.append(False)
+            except TypeError:
+                self.predictions.append(False)
+            self.anomalies_scores.append(score)
+        end = time.perf_counter_ns()
+        self.last_inference_time = (end - start) / 1e6 / len(data_to_scores)
```

### Comparing `legopack-0.12/legopack/models/custom.py` & `legopack-0.2/legopack/models/custom.py`

 * *Files identical despite different names*

### Comparing `legopack-0.12/legopack/tools.py` & `legopack-0.2/legopack/tools.py`

 * *Files identical despite different names*

