# Comparing `tmp/python_contest_template-0.0.4.tar.gz` & `tmp/python_contest_template-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_contest_template-0.0.4.tar", last modified: Mon Apr 17 11:14:12 2023, max compression
+gzip compressed data, was "python_contest_template-0.0.5.tar", last modified: Sun May 26 07:44:41 2024, max compression
```

## Comparing `python_contest_template-0.0.4.tar` & `python_contest_template-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,61 @@
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 11:14:12.492137 python_contest_template-0.0.4/
--rw-rw-r--   0 zty       (1000) zty       (1000)    11357 2023-04-10 07:05:07.000000 python_contest_template-0.0.4/LICENSE
--rw-rw-r--   0 zty       (1000) zty       (1000)      673 2023-04-17 11:14:12.492137 python_contest_template-0.0.4/PKG-INFO
--rw-rw-r--   0 zty       (1000) zty       (1000)      108 2023-04-17 09:05:18.000000 python_contest_template-0.0.4/README.md
--rw-rw-r--   0 zty       (1000) zty       (1000)      638 2023-04-17 11:14:04.000000 python_contest_template-0.0.4/pyproject.toml
--rw-rw-r--   0 zty       (1000) zty       (1000)       38 2023-04-17 11:14:12.492137 python_contest_template-0.0.4/setup.cfg
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 11:14:12.492137 python_contest_template-0.0.4/src/
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 11:14:12.492137 python_contest_template-0.0.4/src/graph/
--rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-17 07:05:43.000000 python_contest_template-0.0.4/src/graph/__init__.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     3794 2023-04-17 09:46:56.000000 python_contest_template-0.0.4/src/graph/smallest_routes.py
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 11:14:12.492137 python_contest_template-0.0.4/src/python_contest_template/
--rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-10 06:53:27.000000 python_contest_template-0.0.4/src/python_contest_template/__init__.py
--rw-rw-r--   0 zty       (1000) zty       (1000)     1141 2022-10-30 07:19:15.000000 python_contest_template-0.0.4/src/python_contest_template/binary_tree.py
--rw-rw-r--   0 zty       (1000) zty       (1000)      587 2022-10-13 06:09:27.000000 python_contest_template-0.0.4/src/python_contest_template/single_linked_list.py
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 11:14:12.492137 python_contest_template-0.0.4/src/python_contest_template.egg-info/
--rw-rw-r--   0 zty       (1000) zty       (1000)      673 2023-04-17 11:14:12.000000 python_contest_template-0.0.4/src/python_contest_template.egg-info/PKG-INFO
--rw-rw-r--   0 zty       (1000) zty       (1000)      450 2023-04-17 11:14:12.000000 python_contest_template-0.0.4/src/python_contest_template.egg-info/SOURCES.txt
--rw-rw-r--   0 zty       (1000) zty       (1000)        1 2023-04-17 11:14:12.000000 python_contest_template-0.0.4/src/python_contest_template.egg-info/dependency_links.txt
--rw-rw-r--   0 zty       (1000) zty       (1000)       30 2023-04-17 11:14:12.000000 python_contest_template-0.0.4/src/python_contest_template.egg-info/top_level.txt
-drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2023-04-17 11:14:12.492137 python_contest_template-0.0.4/tests/
--rw-rw-r--   0 zty       (1000) zty       (1000)     2666 2023-04-17 09:47:40.000000 python_contest_template-0.0.4/tests/test_smallest_routes.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/
+-rw-rw-r--   0 zty       (1000) zty       (1000)    11357 2023-04-10 07:05:07.000000 python_contest_template-0.0.5/LICENSE
+-rw-r--r--   0 zty       (1000) zty       (1000)     2339 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/PKG-INFO
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1601 2023-12-04 12:24:01.000000 python_contest_template-0.0.5/README.md
+-rw-rw-r--   0 zty       (1000) zty       (1000)      739 2024-05-26 07:43:01.000000 python_contest_template-0.0.5/pyproject.toml
+-rw-rw-r--   0 zty       (1000) zty       (1000)       82 2023-04-19 03:45:15.000000 python_contest_template-0.0.5/requirements.txt
+-rw-rw-r--   0 zty       (1000) zty       (1000)       38 2024-05-26 07:44:41.194645 python_contest_template-0.0.5/setup.cfg
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.186646 python_contest_template-0.0.5/src/
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/basic/
+-rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-20 07:48:34.000000 python_contest_template-0.0.5/src/basic/__init__.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     3983 2023-09-28 04:58:49.000000 python_contest_template-0.0.5/src/basic/array_of_difference.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1687 2023-08-31 08:48:44.000000 python_contest_template-0.0.5/src/basic/binary_lifting.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1661 2023-09-14 02:22:27.000000 python_contest_template-0.0.5/src/basic/binary_search.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/data_structure/
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2273 2023-11-13 06:56:41.000000 python_contest_template-0.0.5/src/data_structure/bit.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1577 2024-04-10 07:27:24.000000 python_contest_template-0.0.5/src/data_structure/dsu.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2533 2023-10-27 06:13:23.000000 python_contest_template-0.0.5/src/data_structure/monotonic_queue.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     3941 2023-11-02 03:50:49.000000 python_contest_template-0.0.5/src/data_structure/monotonic_stack.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)    10346 2024-05-26 07:44:30.000000 python_contest_template-0.0.5/src/data_structure/segment_tree.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      461 2023-08-31 02:58:26.000000 python_contest_template-0.0.5/src/data_structure/stack.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/dynamic_programming/
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1878 2023-08-31 03:16:36.000000 python_contest_template-0.0.5/src/dynamic_programming/digital_dp.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/graph/
+-rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-17 07:05:43.000000 python_contest_template-0.0.5/src/graph/__init__.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2421 2023-05-28 03:10:31.000000 python_contest_template-0.0.5/src/graph/bfs.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2477 2023-09-04 03:35:24.000000 python_contest_template-0.0.5/src/graph/binary_search_tree.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      651 2023-09-04 02:58:45.000000 python_contest_template-0.0.5/src/graph/binary_tree.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1494 2024-04-25 14:14:45.000000 python_contest_template-0.0.5/src/graph/find_circle.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     3591 2024-05-06 01:25:34.000000 python_contest_template-0.0.5/src/graph/km_algorithm.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2757 2023-08-31 11:23:15.000000 python_contest_template-0.0.5/src/graph/lca.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1983 2023-09-01 06:22:44.000000 python_contest_template-0.0.5/src/graph/minimum_spanning_tree.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     3986 2023-08-31 02:58:26.000000 python_contest_template-0.0.5/src/graph/smallest_routes.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1200 2023-09-12 03:12:29.000000 python_contest_template-0.0.5/src/graph/topological_sorting.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/mathematic/
+-rw-rw-r--   0 zty       (1000) zty       (1000)      780 2023-12-04 12:23:21.000000 python_contest_template-0.0.5/src/mathematic/combinatorics.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      176 2023-05-28 03:10:31.000000 python_contest_template-0.0.5/src/mathematic/common_formula.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      788 2023-05-28 03:10:31.000000 python_contest_template-0.0.5/src/mathematic/fast_power.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      513 2023-04-17 13:32:44.000000 python_contest_template-0.0.5/src/mathematic/fermat_little_theorem.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      317 2023-09-02 07:27:30.000000 python_contest_template-0.0.5/src/mathematic/filter_prime.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      937 2023-04-18 03:26:25.000000 python_contest_template-0.0.5/src/mathematic/find_prime_factor.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      768 2023-05-28 03:10:31.000000 python_contest_template-0.0.5/src/mathematic/greatest_common_divisor.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      460 2023-04-18 03:38:50.000000 python_contest_template-0.0.5/src/mathematic/judge_prime.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/misc/
+-rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-05-28 03:10:31.000000 python_contest_template-0.0.5/src/misc/__init__.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     3444 2023-09-28 05:34:55.000000 python_contest_template-0.0.5/src/misc/discretization.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     2822 2023-05-28 03:10:31.000000 python_contest_template-0.0.5/src/misc/double_pointer.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/python_contest_template/
+-rw-rw-r--   0 zty       (1000) zty       (1000)        0 2023-04-10 06:53:27.000000 python_contest_template-0.0.5/src/python_contest_template/__init__.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1141 2022-10-30 07:19:15.000000 python_contest_template-0.0.5/src/python_contest_template/binary_tree.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      587 2022-10-13 06:09:27.000000 python_contest_template-0.0.5/src/python_contest_template/single_linked_list.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/python_contest_template.egg-info/
+-rw-r--r--   0 zty       (1000) zty       (1000)     2339 2024-05-26 07:44:41.000000 python_contest_template-0.0.5/src/python_contest_template.egg-info/PKG-INFO
+-rw-rw-r--   0 zty       (1000) zty       (1000)     1463 2024-05-26 07:44:41.000000 python_contest_template-0.0.5/src/python_contest_template.egg-info/SOURCES.txt
+-rw-rw-r--   0 zty       (1000) zty       (1000)        1 2024-05-26 07:44:41.000000 python_contest_template-0.0.5/src/python_contest_template.egg-info/dependency_links.txt
+-rw-rw-r--   0 zty       (1000) zty       (1000)       83 2024-05-26 07:44:41.000000 python_contest_template-0.0.5/src/python_contest_template.egg-info/requires.txt
+-rw-rw-r--   0 zty       (1000) zty       (1000)      101 2024-05-26 07:44:41.000000 python_contest_template-0.0.5/src/python_contest_template.egg-info/top_level.txt
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/search/
+-rw-rw-r--   0 zty       (1000) zty       (1000)     4267 2023-09-12 06:12:31.000000 python_contest_template-0.0.5/src/search/backtrace.py
+drwxrwxr-x   0 zty       (1000) zty       (1000)        0 2024-05-26 07:44:41.190645 python_contest_template-0.0.5/src/string/
+-rw-rw-r--   0 zty       (1000) zty       (1000)      371 2024-05-26 07:39:17.000000 python_contest_template-0.0.5/src/string/prefix_function.py
+-rw-rw-r--   0 zty       (1000) zty       (1000)      469 2024-05-26 07:40:17.000000 python_contest_template-0.0.5/src/string/z_function.py
```

### Comparing `python_contest_template-0.0.4/LICENSE` & `python_contest_template-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.4/src/graph/smallest_routes.py` & `python_contest_template-0.0.5/src/graph/smallest_routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
      
      
 """
 #! Dijkstra算法
 #! 优点: 可以不用计算两两点之间的最短路径, 可以求出某一起点开始的最短路径
 #! 缺点: 不能处理负权
 #! 时间复杂度: O(n^2), 如果求两两点之间的最短路, 也是O(n^3)
+#! Dijkstra算法可以保证在跑一次算法中每个点只遇到一次, 也就是说从起点到已经遍历到的点的路径在后续更新最短路的过程中, 其最短路不会变化
 """
 def common_dijkstra(g: List[List[List[int]]], start: int) -> List[int]:
     """dijkstra算法
     本质上是个贪心, 选择当前权值最小的路径
 
     Args:
         g (List[List[List[int]]]): 图, g[x]存储两个值(x, w)构成的列表, y表示相邻的节点, w表示x和y相连的这条边的权重
@@ -51,15 +52,15 @@
     Returns:
         List[int]: 返回当前起点到其他节点的最短路径
     """
     n = len(g)
     dis = [inf] * n
     dis[start] = 0
     vis = [False]*n #* 标记已经被更新成最短路的点
-    for j in range(n):
+    for i in range(n):
         x = -1
         for j in range(n):
             if(not vis[j] and (x<0 or dis[j] < dis[x])):   #* 如果没有被标记过且当前的最短路, 那么就用x来更新其他点
                 x = j
         vis[x] = True
         for y, w in g[x]:
             if(dis[y] > dis[x] + w):
@@ -103,8 +104,7 @@
 
                 
                 
     
     
                 
 
-
```

### Comparing `python_contest_template-0.0.4/src/python_contest_template/binary_tree.py` & `python_contest_template-0.0.5/src/python_contest_template/binary_tree.py`

 * *Files identical despite different names*

### Comparing `python_contest_template-0.0.4/src/python_contest_template/single_linked_list.py` & `python_contest_template-0.0.5/src/python_contest_template/single_linked_list.py`

 * *Files identical despite different names*

