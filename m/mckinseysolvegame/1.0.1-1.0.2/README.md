# Comparing `tmp/mckinseysolvegame-1.0.1.tar.gz` & `tmp/mckinseysolvegame-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mckinseysolvegame-1.0.1.tar", last modified: Sat Apr 27 16:10:11 2024, max compression
+gzip compressed data, was "mckinseysolvegame-1.0.2.tar", last modified: Sun May 26 13:48:16 2024, max compression
```

## Comparing `mckinseysolvegame-1.0.1.tar` & `mckinseysolvegame-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:10:11.937461 mckinseysolvegame-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    14975 2024-04-27 16:10:11.937461 mckinseysolvegame-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14091 2024-04-27 16:10:04.000000 mckinseysolvegame-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:10:11.933461 mckinseysolvegame-1.0.1/mckinseysolvegame/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-27 16:10:04.000000 mckinseysolvegame-1.0.1/mckinseysolvegame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 16:10:04.000000 mckinseysolvegame-1.0.1/mckinseysolvegame/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:10:11.933461 mckinseysolvegame-1.0.1/mckinseysolvegame/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 16:10:04.000000 mckinseysolvegame-1.0.1/mckinseysolvegame/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-27 16:10:04.000000 mckinseysolvegame-1.0.1/mckinseysolvegame/domain/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:10:11.937461 mckinseysolvegame-1.0.1/mckinseysolvegame/domain/services/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-27 16:10:04.000000 mckinseysolvegame-1.0.1/mckinseysolvegame/domain/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-27 16:10:04.000000 mckinseysolvegame-1.0.1/mckinseysolvegame/domain/services/optimization_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:10:11.937461 mckinseysolvegame-1.0.1/mckinseysolvegame/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 16:10:04.000000 mckinseysolvegame-1.0.1/mckinseysolvegame/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-27 16:10:04.000000 mckinseysolvegame-1.0.1/mckinseysolvegame/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    30532 2024-04-27 16:10:04.000000 mckinseysolvegame-1.0.1/mckinseysolvegame/tests/test_optimization_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:10:11.937461 mckinseysolvegame-1.0.1/mckinseysolvegame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14975 2024-04-27 16:10:11.000000 mckinseysolvegame-1.0.1/mckinseysolvegame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-27 16:10:11.000000 mckinseysolvegame-1.0.1/mckinseysolvegame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:10:11.000000 mckinseysolvegame-1.0.1/mckinseysolvegame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-27 16:10:11.000000 mckinseysolvegame-1.0.1/mckinseysolvegame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 16:10:11.000000 mckinseysolvegame-1.0.1/mckinseysolvegame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-27 16:10:04.000000 mckinseysolvegame-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 16:10:11.937461 mckinseysolvegame-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-27 16:10:04.000000 mckinseysolvegame-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:48:16.366020 mckinseysolvegame-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    14975 2024-05-26 13:48:16.366020 mckinseysolvegame-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14091 2024-05-26 13:48:12.000000 mckinseysolvegame-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:48:16.366020 mckinseysolvegame-1.0.2/mckinseysolvegame/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-26 13:48:12.000000 mckinseysolvegame-1.0.2/mckinseysolvegame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 13:48:12.000000 mckinseysolvegame-1.0.2/mckinseysolvegame/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:48:16.366020 mckinseysolvegame-1.0.2/mckinseysolvegame/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-26 13:48:12.000000 mckinseysolvegame-1.0.2/mckinseysolvegame/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-26 13:48:12.000000 mckinseysolvegame-1.0.2/mckinseysolvegame/domain/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:48:16.366020 mckinseysolvegame-1.0.2/mckinseysolvegame/domain/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-26 13:48:12.000000 mckinseysolvegame-1.0.2/mckinseysolvegame/domain/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-26 13:48:12.000000 mckinseysolvegame-1.0.2/mckinseysolvegame/domain/services/optimization_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:48:16.366020 mckinseysolvegame-1.0.2/mckinseysolvegame/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 13:48:12.000000 mckinseysolvegame-1.0.2/mckinseysolvegame/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-05-26 13:48:12.000000 mckinseysolvegame-1.0.2/mckinseysolvegame/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30484 2024-05-26 13:48:12.000000 mckinseysolvegame-1.0.2/mckinseysolvegame/tests/test_optimization_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:48:16.366020 mckinseysolvegame-1.0.2/mckinseysolvegame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14975 2024-05-26 13:48:16.000000 mckinseysolvegame-1.0.2/mckinseysolvegame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-26 13:48:16.000000 mckinseysolvegame-1.0.2/mckinseysolvegame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:48:16.000000 mckinseysolvegame-1.0.2/mckinseysolvegame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-26 13:48:16.000000 mckinseysolvegame-1.0.2/mckinseysolvegame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 13:48:16.000000 mckinseysolvegame-1.0.2/mckinseysolvegame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-26 13:48:12.000000 mckinseysolvegame-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-26 13:48:16.366020 mckinseysolvegame-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-26 13:48:12.000000 mckinseysolvegame-1.0.2/setup.py
```

### Comparing `mckinseysolvegame-1.0.1/PKG-INFO` & `mckinseysolvegame-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mckinseysolvegame
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python library for solving the McKinsey Solve Game
 Home-page: https://github.com/SebastienEveno/mckinseysolvegame
 Author: Sebastien Eveno
 Author-email: sebastien.louis.eveno@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mckinseysolvegame Version: 1.0.1 Summary: Python
+Metadata-Version: 2.1 Name: mckinseysolvegame Version: 1.0.2 Summary: Python
 library for solving the McKinsey Solve Game Home-page: https://github.com/
 SebastienEveno/mckinseysolvegame Author: Sebastien Eveno Author-email:
 sebastien.louis.eveno@gmail.com License: MIT Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Software Development Classifier: Topic ::
```

### Comparing `mckinseysolvegame-1.0.1/README.md` & `mckinseysolvegame-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-1.0.1/mckinseysolvegame/domain/models.py` & `mckinseysolvegame-1.0.2/mckinseysolvegame/domain/models.py`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-1.0.1/mckinseysolvegame/domain/services/optimization_service.py` & `mckinseysolvegame-1.0.2/mckinseysolvegame/domain/services/optimization_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 from mckinseysolvegame.domain.models import Species, OptimizationResult
 
 
 class Solver:
 
     @staticmethod
     def find_sustainable_food_chain(species: List[Species]) -> OptimizationResult:
+        maximum_food_chain_length = 8
         species_copy = copy.deepcopy(species)
         if not species_copy:
             return OptimizationResult([])
 
         populate_food_sources(species_copy)
 
         species_copy.sort(key=lambda x: x.depth_range)
         grouped_species = {key: list(group) for key, group in groupby(
             species_copy, key=lambda x: x.depth_range)}
 
         longest_sustainable_chain_per_depth_range = {}
         for depth_range, species_copy in grouped_species.items():
-            n = len(species_copy)
+            n = min(maximum_food_chain_length, len(species_copy))
             species_copy.sort(key=lambda x: x.calories_provided, reverse=True)
 
             optimal_list = []
             for length in range(1, n + 1):
                 for combination in combinations(species_copy, length):
                     combination = list(combination)
                     if is_sustainable(combination) and len(combination) > len(optimal_list):
```

### Comparing `mckinseysolvegame-1.0.1/mckinseysolvegame/tests/test_models.py` & `mckinseysolvegame-1.0.2/mckinseysolvegame/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-1.0.1/mckinseysolvegame/tests/test_optimization_service.py` & `mckinseysolvegame-1.0.2/mckinseysolvegame/tests/test_optimization_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -692,17 +692,17 @@
                         temperature_range="28.3-30",
                         food_sources=[
                             "Queen Parrotfish"
                         ]
                         )
             ],
             [
-                'Purple Hydrocoral', 'Stalked Kelp', 'Blue Shark', 'Rock Weed',
-                'Powder Blue Tang', 'Flame Angelfish', 'Swordfish', 'Bicolour Angelfish',
-                'Northern Red Snapper', 'Eyestripe Surgeonfish'
+                'Fire Coral', 'Widgeon Grass', 'Common Eel Grass', 
+                'Queen Parrotfish', 'Blue Striped Angelfish', 'Queen Angelfish', 
+                'Wahoo', 'Gem Tang'
             ]
         )
     ]
 )
 def test_find_sustainable_food_chain(species, expected_output):
     result = Solver.find_sustainable_food_chain(species)
     assert result.species == expected_output
```

### Comparing `mckinseysolvegame-1.0.1/mckinseysolvegame.egg-info/PKG-INFO` & `mckinseysolvegame-1.0.2/mckinseysolvegame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mckinseysolvegame
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python library for solving the McKinsey Solve Game
 Home-page: https://github.com/SebastienEveno/mckinseysolvegame
 Author: Sebastien Eveno
 Author-email: sebastien.louis.eveno@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mckinseysolvegame Version: 1.0.1 Summary: Python
+Metadata-Version: 2.1 Name: mckinseysolvegame Version: 1.0.2 Summary: Python
 library for solving the McKinsey Solve Game Home-page: https://github.com/
 SebastienEveno/mckinseysolvegame Author: Sebastien Eveno Author-email:
 sebastien.louis.eveno@gmail.com License: MIT Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Software Development Classifier: Topic ::
```

### Comparing `mckinseysolvegame-1.0.1/mckinseysolvegame.egg-info/SOURCES.txt` & `mckinseysolvegame-1.0.2/mckinseysolvegame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mckinseysolvegame-1.0.1/setup.py` & `mckinseysolvegame-1.0.2/setup.py`

 * *Files identical despite different names*

