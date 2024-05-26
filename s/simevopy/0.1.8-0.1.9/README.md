# Comparing `tmp/simevopy-0.1.8.tar.gz` & `tmp/simevopy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simevopy-0.1.8.tar", last modified: Thu May 16 19:27:03 2024, max compression
+gzip compressed data, was "simevopy-0.1.9.tar", last modified: Tue May 21 09:02:33 2024, max compression
```

## Comparing `simevopy-0.1.8.tar` & `simevopy-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.031912 simevopy-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 19:26:48.000000 simevopy-0.1.8/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-16 19:26:48.000000 simevopy-0.1.8/.clangd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.027912 simevopy-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.027912 simevopy-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-16 19:26:48.000000 simevopy-0.1.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 19:26:48.000000 simevopy-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-16 19:26:48.000000 simevopy-0.1.8/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 19:26:48.000000 simevopy-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-05-16 19:27:03.031912 simevopy-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-05-16 19:26:48.000000 simevopy-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.027912 simevopy-0.1.8/bindings/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-16 19:26:48.000000 simevopy-0.1.8/bindings/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.027912 simevopy-0.1.8/bindings/core/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-16 19:26:48.000000 simevopy-0.1.8/bindings/core/genes_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-16 19:26:48.000000 simevopy-0.1.8/bindings/core/organism_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-16 19:26:48.000000 simevopy-0.1.8/bindings/pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-16 19:26:48.000000 simevopy-0.1.8/bindings/python_bindings.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)      856 2024-05-16 19:26:48.000000 simevopy-0.1.8/bump_version.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.031912 simevopy-0.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:26:48.000000 simevopy-0.1.8/examples/size_awareness.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 19:26:48.000000 simevopy-0.1.8/examples/speed_food.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.027912 simevopy-0.1.8/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.031912 simevopy-0.1.8/include/core/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-16 19:26:48.000000 simevopy-0.1.8/include/core/Environment.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-16 19:26:48.000000 simevopy-0.1.8/include/core/Food.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-16 19:26:48.000000 simevopy-0.1.8/include/core/Genes.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-16 19:26:48.000000 simevopy-0.1.8/include/core/Organism.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.031912 simevopy-0.1.8/include/index/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-16 19:26:48.000000 simevopy-0.1.8/include/index/ISpatialIndex.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 19:26:48.000000 simevopy-0.1.8/include/index/ISpatialObject.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-16 19:26:48.000000 simevopy-0.1.8/include/index/SpatialIndex.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-16 19:26:48.000000 simevopy-0.1.8/include/index/SpatialObjectWrapper.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.031912 simevopy-0.1.8/include/test/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-16 19:26:48.000000 simevopy-0.1.8/include/test/Dummy.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-16 19:26:48.000000 simevopy-0.1.8/include/test/SpatialIndexTest.hpp
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:27:03.031912 simevopy-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-16 19:27:01.000000 simevopy-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.031912 simevopy-0.1.8/simevopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-05-16 19:27:02.000000 simevopy-0.1.8/simevopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-16 19:27:02.000000 simevopy-0.1.8/simevopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:27:02.000000 simevopy-0.1.8/simevopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:27:02.000000 simevopy-0.1.8/simevopy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.031912 simevopy-0.1.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-16 19:26:48.000000 simevopy-0.1.8/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.031912 simevopy-0.1.8/src/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-16 19:26:48.000000 simevopy-0.1.8/src/core/Environment.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-16 19:26:48.000000 simevopy-0.1.8/src/core/Genes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-16 19:26:48.000000 simevopy-0.1.8/src/core/Organism.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.031912 simevopy-0.1.8/src/index/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-16 19:26:48.000000 simevopy-0.1.8/src/index/DefaultSpatialIndex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-16 19:26:48.000000 simevopy-0.1.8/src/index/OptimizedSpatialIndex.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.027912 simevopy-0.1.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:03.031912 simevopy-0.1.8/tests/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-16 19:26:48.000000 simevopy-0.1.8/tests/cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-16 19:26:48.000000 simevopy-0.1.8/tests/cpp/SpatialIndexTest.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-16 19:26:48.000000 simevopy-0.1.8/tests/cpp/gtest.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.953746 simevopy-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-21 09:02:13.000000 simevopy-0.1.9/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-21 09:02:13.000000 simevopy-0.1.9/.clangd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.945746 simevopy-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-21 09:02:13.000000 simevopy-0.1.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-21 09:02:13.000000 simevopy-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-21 09:02:13.000000 simevopy-0.1.9/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-21 09:02:13.000000 simevopy-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-05-21 09:02:33.953746 simevopy-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-05-21 09:02:13.000000 simevopy-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-21 09:02:13.000000 simevopy-0.1.9/bindings/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/bindings/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-21 09:02:13.000000 simevopy-0.1.9/bindings/core/genes_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-21 09:02:13.000000 simevopy-0.1.9/bindings/core/organism_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-21 09:02:13.000000 simevopy-0.1.9/bindings/pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-21 09:02:13.000000 simevopy-0.1.9/bindings/python_bindings.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      843 2024-05-21 09:02:13.000000 simevopy-0.1.9/bump_version.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:13.000000 simevopy-0.1.9/examples/size_awareness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-21 09:02:13.000000 simevopy-0.1.9/examples/speed_food.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.945746 simevopy-0.1.9/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/include/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/core/Environment.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/core/Food.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/core/Genes.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/core/Organism.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/include/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/index/ISpatialIndex.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/index/ISpatialObject.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/index/SpatialIndex.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/index/SpatialObjectWrapper.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/include/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/test/Dummy.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/test/SpatialIndexTest.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:02:33.953746 simevopy-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-21 09:02:32.000000 simevopy-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/simevopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-05-21 09:02:33.000000 simevopy-0.1.9/simevopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-21 09:02:33.000000 simevopy-0.1.9/simevopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:02:33.000000 simevopy-0.1.9/simevopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:02:33.000000 simevopy-0.1.9/simevopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-21 09:02:13.000000 simevopy-0.1.9/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.953746 simevopy-0.1.9/src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-21 09:02:13.000000 simevopy-0.1.9/src/core/Environment.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-21 09:02:13.000000 simevopy-0.1.9/src/core/Genes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-21 09:02:13.000000 simevopy-0.1.9/src/core/Organism.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.953746 simevopy-0.1.9/src/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-21 09:02:13.000000 simevopy-0.1.9/src/index/DefaultSpatialIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-21 09:02:13.000000 simevopy-0.1.9/src/index/OptimizedSpatialIndex.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.945746 simevopy-0.1.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.953746 simevopy-0.1.9/tests/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-21 09:02:13.000000 simevopy-0.1.9/tests/cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-21 09:02:13.000000 simevopy-0.1.9/tests/cpp/SpatialIndexTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-21 09:02:13.000000 simevopy-0.1.9/tests/cpp/gtest.cmake
```

### Comparing `simevopy-0.1.8/.github/workflows/ci.yml` & `simevopy-0.1.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/CMakeLists.txt` & `simevopy-0.1.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/LICENSE` & `simevopy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/PKG-INFO` & `simevopy-0.1.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: simevopy
-Version: 0.1.8
+Version: 0.1.9
 Summary: SimEvo Python bindings
 Home-page: https://github.com/YJack0000/SimEvo
 Author: YJack0000
 Author-email: yjack0000.cs12@nycu.edu.tw
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 SimEvo: A Simple Python Library for Simulations of Natural Selection
 ---
 
+[![CodeFactor](https://www.codefactor.io/repository/github/yjack0000/simevo/badge)](https://www.codefactor.io/repository/github/yjack0000/simevo)
+![GitHub](https://img.shields.io/github/license/YJack0000/SimEvo)
+![GitHub repo size](https://img.shields.io/github/repo-size/YJack0000/SimEvo)
+
 ## Basic Information
 
 > **Project Overview:** Simulating Natural Selection in Ecosystems using C++ and Python
 
 SimSel leverages the computational efficiency of C++ for the core simulation engine and offers an intuitive Python interface for ease of use and accessibility. It models ecosystems composed of organisms with genetically determined traits, interacting within an environment that includes resources like food. The simulation observes the principles of natural selection, with organism survival and reproduction influenced by their traits and environmental factors.
 
 - 📂 **GitHub Repository**: [https://github.com/YJack0000/SimEvo](https://github.com/YJack0000/SimEvo)
@@ -92,15 +96,15 @@
 
 
 ### Python Script Examples
 
 The script sets up a SimSel simulation in a 500x500 space, initializing 10 "ABCD" gene organisms and distributing food to model resource scarcity. Operating in an "optimize" mode for efficiency, it cycles through 100 generations, each time scattering food and advancing the simulation to observe natural selection as organisms interact, feed, and reproduce based on genetic traits.
 
 ```python
-from SimSel import Environment, Organism, Genes
+from SimEvo.core import Environment, Organism, Genes
 import random
 
 def setup_base_organism(env, count=10):
     for _ in range(count):
         x = random.randint(0, env.width - 1)
         y = random.randint(0, env.height - 1)
         env.add_organism(Organism(Genes("ABCD")), x, y)
@@ -117,58 +121,8 @@
 
 for i in range(100):
     print(f"Gen {i} th")
     distribute_food_randomly(env, 100)
     env.simulate_iteration(50)
 ```
 
-## Engineering Infrastructure
-
-- **Automatic Build System**:
-    - [GNU make](https://www.gnu.org/software/make/manual/make.html)
-- **Version Control**:
-    - Git
-    - Github
-- **Testing Framework**:
-    - C++: [Google Test](https://github.com/google/googletest)
-    - Python: [pytest](https://docs.pytest.org/en/7.4.x/)
-- **Documentation**:
-    - Markdown
-- **Continuous Integration**
-  - [Github Actions](https://github.com/features/actions)
-
-## Schedule
-
-Week 1 (4/8):
-- Set up and model the basic C++ environment.
-- Studying the relevant field knowledge and adjust the existing interface accordingly.
-- Set up a CI pipeline for unit testing.
-
-Week 2 (4/15):
-- Implement genetic traits and organism dynamics.
-- Develop pybind11 wrappers.
-- Write unit tests for both implementations.
-
-Week 3 (4/22):
-- Implement the Environment with detailed simulation logic.
-- Implement the DefaultSpatialIndex and possibly adjust some interfaces.
-- Develop pybind11 wrappers.
-- Write unit tests for the implementations.
-
-Week 4 (4/29):
-- Allocate this week as flexible time to address potential issues from last week's development.
-
-Week 5 (5/6):
-- Implement a higher performance data structure, currently planned to be Quadtree.
-- Write unit tests for the new implementation.
-
-Week 6 (5/13):
-- Set up a CI pipeline for performance evaluation.
-- Create documentation and update example scripts.
-
-Week 7 (5/20):
-- Prepare for the paper presentation.
-
-Week 8 (5/27):
-- Designate as flexible time for any overflow tasks or final adjustments.
-
```

### Comparing `simevopy-0.1.8/README.md` & `simevopy-0.1.9/simevopy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,26 @@
+Metadata-Version: 2.1
+Name: simevopy
+Version: 0.1.9
+Summary: SimEvo Python bindings
+Home-page: https://github.com/YJack0000/SimEvo
+Author: YJack0000
+Author-email: yjack0000.cs12@nycu.edu.tw
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 SimEvo: A Simple Python Library for Simulations of Natural Selection
 ---
 
+[![CodeFactor](https://www.codefactor.io/repository/github/yjack0000/simevo/badge)](https://www.codefactor.io/repository/github/yjack0000/simevo)
+![GitHub](https://img.shields.io/github/license/YJack0000/SimEvo)
+![GitHub repo size](https://img.shields.io/github/repo-size/YJack0000/SimEvo)
+
 ## Basic Information
 
 > **Project Overview:** Simulating Natural Selection in Ecosystems using C++ and Python
 
 SimSel leverages the computational efficiency of C++ for the core simulation engine and offers an intuitive Python interface for ease of use and accessibility. It models ecosystems composed of organisms with genetically determined traits, interacting within an environment that includes resources like food. The simulation observes the principles of natural selection, with organism survival and reproduction influenced by their traits and environmental factors.
 
 - 📂 **GitHub Repository**: [https://github.com/YJack0000/SimEvo](https://github.com/YJack0000/SimEvo)
@@ -80,15 +96,15 @@
 
 
 ### Python Script Examples
 
 The script sets up a SimSel simulation in a 500x500 space, initializing 10 "ABCD" gene organisms and distributing food to model resource scarcity. Operating in an "optimize" mode for efficiency, it cycles through 100 generations, each time scattering food and advancing the simulation to observe natural selection as organisms interact, feed, and reproduce based on genetic traits.
 
 ```python
-from SimSel import Environment, Organism, Genes
+from SimEvo.core import Environment, Organism, Genes
 import random
 
 def setup_base_organism(env, count=10):
     for _ in range(count):
         x = random.randint(0, env.width - 1)
         y = random.randint(0, env.height - 1)
         env.add_organism(Organism(Genes("ABCD")), x, y)
@@ -105,56 +121,8 @@
 
 for i in range(100):
     print(f"Gen {i} th")
     distribute_food_randomly(env, 100)
     env.simulate_iteration(50)
 ```
 
-## Engineering Infrastructure
-
-- **Automatic Build System**:
-    - [GNU make](https://www.gnu.org/software/make/manual/make.html)
-- **Version Control**:
-    - Git
-    - Github
-- **Testing Framework**:
-    - C++: [Google Test](https://github.com/google/googletest)
-    - Python: [pytest](https://docs.pytest.org/en/7.4.x/)
-- **Documentation**:
-    - Markdown
-- **Continuous Integration**
-  - [Github Actions](https://github.com/features/actions)
-
-## Schedule
-
-Week 1 (4/8):
-- Set up and model the basic C++ environment.
-- Studying the relevant field knowledge and adjust the existing interface accordingly.
-- Set up a CI pipeline for unit testing.
-
-Week 2 (4/15):
-- Implement genetic traits and organism dynamics.
-- Develop pybind11 wrappers.
-- Write unit tests for both implementations.
-
-Week 3 (4/22):
-- Implement the Environment with detailed simulation logic.
-- Implement the DefaultSpatialIndex and possibly adjust some interfaces.
-- Develop pybind11 wrappers.
-- Write unit tests for the implementations.
-
-Week 4 (4/29):
-- Allocate this week as flexible time to address potential issues from last week's development.
-
-Week 5 (5/6):
-- Implement a higher performance data structure, currently planned to be Quadtree.
-- Write unit tests for the new implementation.
-
-Week 6 (5/13):
-- Set up a CI pipeline for performance evaluation.
-- Create documentation and update example scripts.
-
-Week 7 (5/20):
-- Prepare for the paper presentation.
 
-Week 8 (5/27):
-- Designate as flexible time for any overflow tasks or final adjustments.
```

### Comparing `simevopy-0.1.8/bindings/core/organism_bindings.cpp` & `simevopy-0.1.9/bindings/core/organism_bindings.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/bump_version.sh` & `simevopy-0.1.9/bump_version.sh`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,15 @@
   sed -i '' "s/version='$VERSION'/version='$NEW_VERSION'/" setup.py
 else
   # Linux
   sed -i "s/version='$VERSION'/version='$NEW_VERSION'/" setup.py
 fi
 
 # Ensure the version was updated
-grep "version='$NEW_VERSION'" setup.py
-if [ $? -eq 0 ]; then
+if grep "version='$NEW_VERSION'" setup.py; then
     echo "Version updated successfully"
 else
     echo "Failed to update version"
     exit 1  # Exit with an error
 fi
 
 # Output the new version
```

### Comparing `simevopy-0.1.8/examples/speed_food.py` & `simevopy-0.1.9/examples/speed_food.py`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/include/core/Environment.hpp` & `simevopy-0.1.9/include/core/Environment.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/include/core/Organism.hpp` & `simevopy-0.1.9/include/core/Organism.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/include/index/SpatialIndex.hpp` & `simevopy-0.1.9/include/index/SpatialIndex.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/include/index/SpatialObjectWrapper.hpp` & `simevopy-0.1.9/include/index/SpatialObjectWrapper.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/include/test/SpatialIndexTest.hpp` & `simevopy-0.1.9/include/test/SpatialIndexTest.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/setup.py` & `simevopy-0.1.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="simevopy",
-    version='0.1.8',
+    version='0.1.9',
     description="SimEvo Python bindings",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     cmake_source_dir=".",
     url='https://github.com/YJack0000/SimEvo',
     author='YJack0000',
```

### Comparing `simevopy-0.1.8/simevopy.egg-info/PKG-INFO` & `simevopy-0.1.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,14 @@
-Metadata-Version: 2.1
-Name: simevopy
-Version: 0.1.8
-Summary: SimEvo Python bindings
-Home-page: https://github.com/YJack0000/SimEvo
-Author: YJack0000
-Author-email: yjack0000.cs12@nycu.edu.tw
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 SimEvo: A Simple Python Library for Simulations of Natural Selection
 ---
 
+[![CodeFactor](https://www.codefactor.io/repository/github/yjack0000/simevo/badge)](https://www.codefactor.io/repository/github/yjack0000/simevo)
+![GitHub](https://img.shields.io/github/license/YJack0000/SimEvo)
+![GitHub repo size](https://img.shields.io/github/repo-size/YJack0000/SimEvo)
+
 ## Basic Information
 
 > **Project Overview:** Simulating Natural Selection in Ecosystems using C++ and Python
 
 SimSel leverages the computational efficiency of C++ for the core simulation engine and offers an intuitive Python interface for ease of use and accessibility. It models ecosystems composed of organisms with genetically determined traits, interacting within an environment that includes resources like food. The simulation observes the principles of natural selection, with organism survival and reproduction influenced by their traits and environmental factors.
 
 - 📂 **GitHub Repository**: [https://github.com/YJack0000/SimEvo](https://github.com/YJack0000/SimEvo)
@@ -92,15 +84,15 @@
 
 
 ### Python Script Examples
 
 The script sets up a SimSel simulation in a 500x500 space, initializing 10 "ABCD" gene organisms and distributing food to model resource scarcity. Operating in an "optimize" mode for efficiency, it cycles through 100 generations, each time scattering food and advancing the simulation to observe natural selection as organisms interact, feed, and reproduce based on genetic traits.
 
 ```python
-from SimSel import Environment, Organism, Genes
+from SimEvo.core import Environment, Organism, Genes
 import random
 
 def setup_base_organism(env, count=10):
     for _ in range(count):
         x = random.randint(0, env.width - 1)
         y = random.randint(0, env.height - 1)
         env.add_organism(Organism(Genes("ABCD")), x, y)
@@ -116,59 +108,7 @@
 setup_base_organism(env)
 
 for i in range(100):
     print(f"Gen {i} th")
     distribute_food_randomly(env, 100)
     env.simulate_iteration(50)
 ```
-
-## Engineering Infrastructure
-
-- **Automatic Build System**:
-    - [GNU make](https://www.gnu.org/software/make/manual/make.html)
-- **Version Control**:
-    - Git
-    - Github
-- **Testing Framework**:
-    - C++: [Google Test](https://github.com/google/googletest)
-    - Python: [pytest](https://docs.pytest.org/en/7.4.x/)
-- **Documentation**:
-    - Markdown
-- **Continuous Integration**
-  - [Github Actions](https://github.com/features/actions)
-
-## Schedule
-
-Week 1 (4/8):
-- Set up and model the basic C++ environment.
-- Studying the relevant field knowledge and adjust the existing interface accordingly.
-- Set up a CI pipeline for unit testing.
-
-Week 2 (4/15):
-- Implement genetic traits and organism dynamics.
-- Develop pybind11 wrappers.
-- Write unit tests for both implementations.
-
-Week 3 (4/22):
-- Implement the Environment with detailed simulation logic.
-- Implement the DefaultSpatialIndex and possibly adjust some interfaces.
-- Develop pybind11 wrappers.
-- Write unit tests for the implementations.
-
-Week 4 (4/29):
-- Allocate this week as flexible time to address potential issues from last week's development.
-
-Week 5 (5/6):
-- Implement a higher performance data structure, currently planned to be Quadtree.
-- Write unit tests for the new implementation.
-
-Week 6 (5/13):
-- Set up a CI pipeline for performance evaluation.
-- Create documentation and update example scripts.
-
-Week 7 (5/20):
-- Prepare for the paper presentation.
-
-Week 8 (5/27):
-- Designate as flexible time for any overflow tasks or final adjustments.
-
-
```

### Comparing `simevopy-0.1.8/simevopy.egg-info/SOURCES.txt` & `simevopy-0.1.9/simevopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/src/core/Environment.cpp` & `simevopy-0.1.9/src/core/Environment.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/src/core/Genes.cpp` & `simevopy-0.1.9/src/core/Genes.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/src/core/Organism.cpp` & `simevopy-0.1.9/src/core/Organism.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/src/index/DefaultSpatialIndex.cpp` & `simevopy-0.1.9/src/index/DefaultSpatialIndex.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/src/index/OptimizedSpatialIndex.cpp` & `simevopy-0.1.9/src/index/OptimizedSpatialIndex.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/tests/cpp/CMakeLists.txt` & `simevopy-0.1.9/tests/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.8/tests/cpp/SpatialIndexTest.cpp` & `simevopy-0.1.9/tests/cpp/SpatialIndexTest.cpp`

 * *Files identical despite different names*

