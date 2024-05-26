# Comparing `tmp/python_contest_template-0.0.5.tar.gz` & `tmp/python_contest_template-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_contest_template-0.0.5.tar", last modified: Sun May 26 07:44:41 2024, max compression
+gzip compressed data, was "python_contest_template-0.0.6.tar", last modified: Sun May 26 07:51:17 2024, max compression
```

## Comparing `python_contest_template-0.0.5.tar` & `python_contest_template-0.0.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/
--rw-rw-r--   0 zty       (1000) zty       (1000)    11357 2023-04-10 07:05:07.000000 python_contest_template-0.0.5/LICENSE
--rw-r--r--   0 zty       (1000) zty       (1000)     2339 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/PKG-INFO
--rw-rw-r--   0 zty       (1000) zty       (1000)     1601 2023-12-04 12:24:01.000000 python_contest_template-0.0.5/README.md
--rw-rw-r--   0 zty       (1000) zty       (1000)      739 2024-05-26 07:43:01.000000 python_contest_template-0.0.5/pyproject.toml
--rw-rw-r--   0 zty       (1000) zty       (1000)       82 2023-04-19 03:45:15.000000 python_contest_template-0.0.5/requirements.txt
--rw-rw-r--   0 zty       (1000) zty       (1000)       38 2024-05-26 07:44:41.194645 python_contest_template-0.0.5/setup.cfg
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.186646 python_contest_template-0.0.5/src/
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/basic/
--rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-20 07:48:34.000000 python_contest_template-0.0.5/src/basic/__init__.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     3983 2023-09-28 04:58:49.000000 python_contest_template-0.0.5/src/basic/array_of_difference.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     1687 2023-08-31 08:48:44.000000 python_contest_template-0.0.5/src/basic/binary_lifting.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     1661 2023-09-14 02:22:27.000000 python_contest_template-0.0.5/src/basic/binary_search.py
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/data_structure/
--rw-rw-r--   0 zty       (1000) zty       (1000)     2273 2023-11-13 06:56:41.000000 python_contest_template-0.0.5/src/data_structure/bit.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     1577 2024-04-10 07:27:24.000000 python_contest_template-0.0.5/src/data_structure/dsu.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     2533 2023-10-27 06:13:23.000000 python_contest_template-0.0.5/src/data_structure/monotonic_queue.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     3941 2023-11-02 03:50:49.000000 python_contest_template-0.0.5/src/data_structure/monotonic_stack.py
--rw-rw-r--   0 zty       (1000) zty       (1000)    10346 2024-05-26 07:44:30.000000 python_contest_template-0.0.5/src/data_structure/segment_tree.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      461 2023-08-31 02:58:26.000000 python_contest_template-0.0.5/src/data_structure/stack.py
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/dynamic_programming/
--rw-rw-r--   0 zty       (1000) zty       (1000)     1878 2023-08-31 03:16:36.000000 python_contest_template-0.0.5/src/dynamic_programming/digital_dp.py
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/graph/
--rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-17 07:05:43.000000 python_contest_template-0.0.5/src/graph/__init__.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     2421 2023-05-28 03:10:31.000000 python_contest_template-0.0.5/src/graph/bfs.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     2477 2023-09-04 03:35:24.000000 python_contest_template-0.0.5/src/graph/binary_search_tree.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      651 2023-09-04 02:58:45.000000 python_contest_template-0.0.5/src/graph/binary_tree.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     1494 2024-04-25 14:14:45.000000 python_contest_template-0.0.5/src/graph/find_circle.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     3591 2024-05-06 01:25:34.000000 python_contest_template-0.0.5/src/graph/km_algorithm.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     2757 2023-08-31 11:23:15.000000 python_contest_template-0.0.5/src/graph/lca.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     1983 2023-09-01 06:22:44.000000 python_contest_template-0.0.5/src/graph/minimum_spanning_tree.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     3986 2023-08-31 02:58:26.000000 python_contest_template-0.0.5/src/graph/smallest_routes.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     1200 2023-09-12 03:12:29.000000 python_contest_template-0.0.5/src/graph/topological_sorting.py
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/mathematic/
--rw-rw-r--   0 zty       (1000) zty       (1000)      780 2023-12-04 12:23:21.000000 python_contest_template-0.0.5/src/mathematic/combinatorics.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      176 2023-05-28 03:10:31.000000 python_contest_template-0.0.5/src/mathematic/common_formula.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      788 2023-05-28 03:10:31.000000 python_contest_template-0.0.5/src/mathematic/fast_power.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      513 2023-04-17 13:32:44.000000 python_contest_template-0.0.5/src/mathematic/fermat_little_theorem.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      317 2023-09-02 07:27:30.000000 python_contest_template-0.0.5/src/mathematic/filter_prime.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      937 2023-04-18 03:26:25.000000 python_contest_template-0.0.5/src/mathematic/find_prime_factor.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      768 2023-05-28 03:10:31.000000 python_contest_template-0.0.5/src/mathematic/greatest_common_divisor.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      460 2023-04-18 03:38:50.000000 python_contest_template-0.0.5/src/mathematic/judge_prime.py
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/misc/
--rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-05-28 03:10:31.000000 python_contest_template-0.0.5/src/misc/__init__.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     3444 2023-09-28 05:34:55.000000 python_contest_template-0.0.5/src/misc/discretization.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     2822 2023-05-28 03:10:31.000000 python_contest_template-0.0.5/src/misc/double_pointer.py
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/python_contest_template/
--rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-10 06:53:27.000000 python_contest_template-0.0.5/src/python_contest_template/__init__.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     1141 2022-10-30 07:19:15.000000 python_contest_template-0.0.5/src/python_contest_template/binary_tree.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      587 2022-10-13 06:09:27.000000 python_contest_template-0.0.5/src/python_contest_template/single_linked_list.py
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/python_contest_template.egg-info/
--rw-r--r--   0 zty       (1000) zty       (1000)     2339 2024-05-26 07:44:41.000000 python_contest_template-0.0.5/src/python_contest_template.egg-info/PKG-INFO
--rw-rw-r--   0 zty       (1000) zty       (1000)     1463 2024-05-26 07:44:41.000000 python_contest_template-0.0.5/src/python_contest_template.egg-info/SOURCES.txt
--rw-rw-r--   0 zty       (1000) zty       (1000)        1 2024-05-26 07:44:41.000000 python_contest_template-0.0.5/src/python_contest_template.egg-info/dependency_links.txt
--rw-rw-r--   0 zty       (1000) zty       (1000)       83 2024-05-26 07:44:41.000000 python_contest_template-0.0.5/src/python_contest_template.egg-info/requires.txt
--rw-rw-r--   0 zty       (1000) zty       (1000)      101 2024-05-26 07:44:41.000000 python_contest_template-0.0.5/src/python_contest_template.egg-info/top_level.txt
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/search/
--rw-rw-r--   0 zty       (1000) zty       (1000)     4267 2023-09-12 06:12:31.000000 python_contest_template-0.0.5/src/search/backtrace.py
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/string/
--rw-rw-r--   0 zty       (1000) zty       (1000)      371 2024-05-26 07:39:17.000000 python_contest_template-0.0.5/src/string/prefix_function.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      469 2024-05-26 07:40:17.000000 python_contest_template-0.0.5/src/string/z_function.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:51:17.863115 python_contest_template-0.0.6/
+-rw-rw-r--   0 zty       (1000) zty       (1000)    11357 2023-04-10 07:05:07.000000 python_contest_template-0.0.6/LICENSE
+-rw-r--r--   0 zty       (1000) zty       (1000)     2339 2024-05-26 07:51:17.863115 python_contest_template-0.0.6/PKG-INFO
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1601 2023-12-04 12:24:01.000000 python_contest_template-0.0.6/README.md
+-rw-rw-r--   0 zty       (1000) zty       (1000)      739 2024-05-26 07:51:02.000000 python_contest_template-0.0.6/pyproject.toml
+-rw-rw-r--   0 zty       (1000) zty       (1000)       82 2023-04-19 03:45:15.000000 python_contest_template-0.0.6/requirements.txt
+-rw-rw-r--   0 zty       (1000) zty       (1000)       38 2024-05-26 07:51:17.863115 python_contest_template-0.0.6/setup.cfg
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:51:17.859115 python_contest_template-0.0.6/src/
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:51:17.859115 python_contest_template-0.0.6/src/basic_algorithm/
+-rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-20 07:48:34.000000 python_contest_template-0.0.6/src/basic_algorithm/__init__.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     3983 2023-09-28 04:58:49.000000 python_contest_template-0.0.6/src/basic_algorithm/array_of_difference.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1687 2023-08-31 08:48:44.000000 python_contest_template-0.0.6/src/basic_algorithm/binary_lifting.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1661 2023-09-14 02:22:27.000000 python_contest_template-0.0.6/src/basic_algorithm/binary_search.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:51:17.859115 python_contest_template-0.0.6/src/character_string/
+-rw-rw-r--   0 zty       (1000) zty       (1000)      371 2024-05-26 07:39:17.000000 python_contest_template-0.0.6/src/character_string/prefix_function.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      469 2024-05-26 07:40:17.000000 python_contest_template-0.0.6/src/character_string/z_function.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:51:17.859115 python_contest_template-0.0.6/src/data_structure/
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2273 2023-11-13 06:56:41.000000 python_contest_template-0.0.6/src/data_structure/bit.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1577 2024-04-10 07:27:24.000000 python_contest_template-0.0.6/src/data_structure/dsu.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2533 2023-10-27 06:13:23.000000 python_contest_template-0.0.6/src/data_structure/monotonic_queue.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     3941 2023-11-02 03:50:49.000000 python_contest_template-0.0.6/src/data_structure/monotonic_stack.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)    10346 2024-05-26 07:44:30.000000 python_contest_template-0.0.6/src/data_structure/segment_tree.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      461 2023-08-31 02:58:26.000000 python_contest_template-0.0.6/src/data_structure/stack.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:51:17.859115 python_contest_template-0.0.6/src/dynamic_programming/
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1878 2023-08-31 03:16:36.000000 python_contest_template-0.0.6/src/dynamic_programming/digital_dp.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:51:17.859115 python_contest_template-0.0.6/src/graph/
+-rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-17 07:05:43.000000 python_contest_template-0.0.6/src/graph/__init__.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2421 2023-05-28 03:10:31.000000 python_contest_template-0.0.6/src/graph/bfs.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2477 2023-09-04 03:35:24.000000 python_contest_template-0.0.6/src/graph/binary_search_tree.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      651 2023-09-04 02:58:45.000000 python_contest_template-0.0.6/src/graph/binary_tree.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1494 2024-04-25 14:14:45.000000 python_contest_template-0.0.6/src/graph/find_circle.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     3591 2024-05-06 01:25:34.000000 python_contest_template-0.0.6/src/graph/km_algorithm.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2757 2023-08-31 11:23:15.000000 python_contest_template-0.0.6/src/graph/lca.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1983 2023-09-01 06:22:44.000000 python_contest_template-0.0.6/src/graph/minimum_spanning_tree.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     3986 2023-08-31 02:58:26.000000 python_contest_template-0.0.6/src/graph/smallest_routes.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1200 2023-09-12 03:12:29.000000 python_contest_template-0.0.6/src/graph/topological_sorting.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:51:17.863115 python_contest_template-0.0.6/src/mathematic/
+-rw-rw-r--   0 zty       (1000) zty       (1000)      780 2023-12-04 12:23:21.000000 python_contest_template-0.0.6/src/mathematic/combinatorics.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      176 2023-05-28 03:10:31.000000 python_contest_template-0.0.6/src/mathematic/common_formula.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      788 2023-05-28 03:10:31.000000 python_contest_template-0.0.6/src/mathematic/fast_power.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      513 2023-04-17 13:32:44.000000 python_contest_template-0.0.6/src/mathematic/fermat_little_theorem.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      317 2023-09-02 07:27:30.000000 python_contest_template-0.0.6/src/mathematic/filter_prime.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      937 2023-04-18 03:26:25.000000 python_contest_template-0.0.6/src/mathematic/find_prime_factor.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      768 2023-05-28 03:10:31.000000 python_contest_template-0.0.6/src/mathematic/greatest_common_divisor.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      460 2023-04-18 03:38:50.000000 python_contest_template-0.0.6/src/mathematic/judge_prime.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:51:17.863115 python_contest_template-0.0.6/src/misc/
+-rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-05-28 03:10:31.000000 python_contest_template-0.0.6/src/misc/__init__.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     3444 2023-09-28 05:34:55.000000 python_contest_template-0.0.6/src/misc/discretization.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2822 2023-05-28 03:10:31.000000 python_contest_template-0.0.6/src/misc/double_pointer.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:51:17.863115 python_contest_template-0.0.6/src/python_contest_template/
+-rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-10 06:53:27.000000 python_contest_template-0.0.6/src/python_contest_template/__init__.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1141 2022-10-30 07:19:15.000000 python_contest_template-0.0.6/src/python_contest_template/binary_tree.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      587 2022-10-13 06:09:27.000000 python_contest_template-0.0.6/src/python_contest_template/single_linked_list.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:51:17.863115 python_contest_template-0.0.6/src/python_contest_template.egg-info/
+-rw-r--r--   0 zty       (1000) zty       (1000)     2339 2024-05-26 07:51:17.000000 python_contest_template-0.0.6/src/python_contest_template.egg-info/PKG-INFO
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1523 2024-05-26 07:51:17.000000 python_contest_template-0.0.6/src/python_contest_template.egg-info/SOURCES.txt
+-rw-rw-r--   0 zty       (1000) zty       (1000)        1 2024-05-26 07:51:17.000000 python_contest_template-0.0.6/src/python_contest_template.egg-info/dependency_links.txt
+-rw-rw-r--   0 zty       (1000) zty       (1000)       83 2024-05-26 07:51:17.000000 python_contest_template-0.0.6/src/python_contest_template.egg-info/requires.txt
+-rw-rw-r--   0 zty       (1000) zty       (1000)      121 2024-05-26 07:51:17.000000 python_contest_template-0.0.6/src/python_contest_template.egg-info/top_level.txt
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:51:17.863115 python_contest_template-0.0.6/src/search/
+-rw-rw-r--   0 zty       (1000) zty       (1000)     4267 2023-09-12 06:12:31.000000 python_contest_template-0.0.6/src/search/backtrace.py
```

### Comparing `python_contest_template-0.0.5/LICENSE` & `python_contest_template-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/PKG-INFO` & `python_contest_template-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_contest_template
-Version: 0.0.5
+Version: 0.0.6
 Summary: python template for contest
 Author-email: zhangtingyu11 <zhangty21@mails.jlu.edu.cn>
 Project-URL: Homepage, https://github.com/zhangtingyu11/python_contest_template
 Project-URL: Bug Tracker, https://github.com/zhangtingyu11/python_contest_template/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_contest_template-0.0.5/README.md` & `python_contest_template-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/pyproject.toml` & `python_contest_template-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python_contest_template"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="zhangtingyu11", email="zhangty21@mails.jlu.edu.cn" },
 ]
 description = "python template for contest"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_contest_template-0.0.5/src/basic/array_of_difference.py` & `python_contest_template-0.0.6/src/basic_algorithm/array_of_difference.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/basic/binary_lifting.py` & `python_contest_template-0.0.6/src/basic_algorithm/binary_lifting.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/basic/binary_search.py` & `python_contest_template-0.0.6/src/basic_algorithm/binary_search.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/data_structure/bit.py` & `python_contest_template-0.0.6/src/data_structure/bit.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/data_structure/dsu.py` & `python_contest_template-0.0.6/src/data_structure/dsu.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/data_structure/monotonic_queue.py` & `python_contest_template-0.0.6/src/data_structure/monotonic_queue.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/data_structure/monotonic_stack.py` & `python_contest_template-0.0.6/src/data_structure/monotonic_stack.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/data_structure/segment_tree.py` & `python_contest_template-0.0.6/src/data_structure/segment_tree.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/dynamic_programming/digital_dp.py` & `python_contest_template-0.0.6/src/dynamic_programming/digital_dp.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/graph/bfs.py` & `python_contest_template-0.0.6/src/graph/bfs.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/graph/binary_search_tree.py` & `python_contest_template-0.0.6/src/graph/binary_search_tree.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/graph/binary_tree.py` & `python_contest_template-0.0.6/src/graph/binary_tree.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/graph/find_circle.py` & `python_contest_template-0.0.6/src/graph/find_circle.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/graph/km_algorithm.py` & `python_contest_template-0.0.6/src/graph/km_algorithm.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/graph/lca.py` & `python_contest_template-0.0.6/src/graph/lca.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/graph/minimum_spanning_tree.py` & `python_contest_template-0.0.6/src/graph/minimum_spanning_tree.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/graph/smallest_routes.py` & `python_contest_template-0.0.6/src/graph/smallest_routes.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/graph/topological_sorting.py` & `python_contest_template-0.0.6/src/graph/topological_sorting.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/mathematic/combinatorics.py` & `python_contest_template-0.0.6/src/mathematic/combinatorics.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/mathematic/fast_power.py` & `python_contest_template-0.0.6/src/mathematic/fast_power.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/mathematic/fermat_little_theorem.py` & `python_contest_template-0.0.6/src/mathematic/fermat_little_theorem.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/mathematic/find_prime_factor.py` & `python_contest_template-0.0.6/src/mathematic/find_prime_factor.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/mathematic/greatest_common_divisor.py` & `python_contest_template-0.0.6/src/mathematic/greatest_common_divisor.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/misc/discretization.py` & `python_contest_template-0.0.6/src/misc/discretization.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/misc/double_pointer.py` & `python_contest_template-0.0.6/src/misc/double_pointer.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/python_contest_template/binary_tree.py` & `python_contest_template-0.0.6/src/python_contest_template/binary_tree.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/python_contest_template/single_linked_list.py` & `python_contest_template-0.0.6/src/python_contest_template/single_linked_list.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.5/src/python_contest_template.egg-info/PKG-INFO` & `python_contest_template-0.0.6/src/python_contest_template.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_contest_template
-Version: 0.0.5
+Version: 0.0.6
 Summary: python template for contest
 Author-email: zhangtingyu11 <zhangty21@mails.jlu.edu.cn>
 Project-URL: Homepage, https://github.com/zhangtingyu11/python_contest_template
 Project-URL: Bug Tracker, https://github.com/zhangtingyu11/python_contest_template/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_contest_template-0.0.5/src/python_contest_template.egg-info/SOURCES.txt` & `python_contest_template-0.0.6/src/python_contest_template.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
-src/basic/__init__.py
-src/basic/array_of_difference.py
-src/basic/binary_lifting.py
-src/basic/binary_search.py
+src/basic_algorithm/__init__.py
+src/basic_algorithm/array_of_difference.py
+src/basic_algorithm/binary_lifting.py
+src/basic_algorithm/binary_search.py
+src/character_string/prefix_function.py
+src/character_string/z_function.py
 src/data_structure/bit.py
 src/data_structure/dsu.py
 src/data_structure/monotonic_queue.py
 src/data_structure/monotonic_stack.py
 src/data_structure/segment_tree.py
 src/data_structure/stack.py
 src/dynamic_programming/digital_dp.py
@@ -38,10 +40,8 @@
 src/python_contest_template/binary_tree.py
 src/python_contest_template/single_linked_list.py
 src/python_contest_template.egg-info/PKG-INFO
 src/python_contest_template.egg-info/SOURCES.txt
 src/python_contest_template.egg-info/dependency_links.txt
 src/python_contest_template.egg-info/requires.txt
 src/python_contest_template.egg-info/top_level.txt
-src/search/backtrace.py
-src/string/prefix_function.py
-src/string/z_function.py
+src/search/backtrace.py
```

### Comparing `python_contest_template-0.0.5/src/search/backtrace.py` & `python_contest_template-0.0.6/src/search/backtrace.py`

 * *Files identical despite different names*

