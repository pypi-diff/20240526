# Comparing `tmp/algogears-1.1.0.tar.gz` & `tmp/algogears-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algogears-1.1.0.tar", last modified: Sun May 12 16:52:31 2024, max compression
+gzip compressed data, was "algogears-1.1.1.tar", last modified: Sun May 26 10:14:19 2024, max compression
```

## Comparing `algogears-1.1.0.tar` & `algogears-1.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 16:52:31.263229 algogears-1.1.0/
--rw-rw-rw-   0        0        0     1104 2024-01-11 15:42:09.000000 algogears-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1071 2024-05-12 16:52:31.262233 algogears-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2697 2024-05-12 16:50:08.000000 algogears-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 16:52:31.215803 algogears-1.1.0/algogears/
--rw-rw-rw-   0        0        0        0 2023-07-23 17:47:02.000000 algogears-1.1.0/algogears/__init__.py
--rw-rw-rw-   0        0        0    19479 2024-05-12 16:40:34.000000 algogears-1.1.0/algogears/core.py
--rw-rw-rw-   0        0        0    10842 2024-05-11 19:23:10.000000 algogears-1.1.0/algogears/dynamic_hull.py
--rw-rw-rw-   0        0        0     3282 2024-01-16 07:50:39.000000 algogears-1.1.0/algogears/graham.py
--rw-rw-rw-   0        0        0      920 2023-06-22 10:15:40.000000 algogears-1.1.0/algogears/jarvis.py
--rw-rw-rw-   0        0        0     2536 2023-06-22 08:22:43.000000 algogears-1.1.0/algogears/kd_tree.py
--rw-rw-rw-   0        0        0     3554 2024-05-02 07:51:52.000000 algogears-1.1.0/algogears/preparata.py
--rw-rw-rw-   0        0        0     2646 2024-05-05 12:11:13.000000 algogears-1.1.0/algogears/quickhull.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:52:31.261236 algogears-1.1.0/algogears.egg-info/
--rw-rw-rw-   0        0        0     1071 2024-05-12 16:52:31.000000 algogears-1.1.0/algogears.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      767 2024-05-12 16:52:31.000000 algogears-1.1.0/algogears.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 16:52:31.000000 algogears-1.1.0/algogears.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-12 16:52:31.000000 algogears-1.1.0/algogears.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2023-06-22 19:12:11.000000 algogears-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 16:52:31.263229 algogears-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1366 2024-05-12 16:45:48.000000 algogears-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:52:31.238078 algogears-1.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:57:15.000000 algogears-1.1.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:52:31.252452 algogears-1.1.0/tests/algorithms/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:57:09.000000 algogears-1.1.0/tests/algorithms/__init__.py
--rw-rw-rw-   0        0        0    13303 2024-05-12 16:27:17.000000 algogears-1.1.0/tests/algorithms/test_dynamic_hull.py
--rw-rw-rw-   0        0        0     5304 2024-05-12 16:27:16.000000 algogears-1.1.0/tests/algorithms/test_graham.py
--rw-rw-rw-   0        0        0      583 2024-05-12 16:27:16.000000 algogears-1.1.0/tests/algorithms/test_jarvis.py
--rw-rw-rw-   0        0        0     2499 2024-05-12 16:27:15.000000 algogears-1.1.0/tests/algorithms/test_kd_tree.py
--rw-rw-rw-   0        0        0     5081 2024-05-12 16:27:15.000000 algogears-1.1.0/tests/algorithms/test_preparata.py
--rw-rw-rw-   0        0        0     3300 2024-05-12 16:27:14.000000 algogears-1.1.0/tests/algorithms/test_quickhull.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:52:31.259243 algogears-1.1.0/tests/entities/
--rw-rw-rw-   0        0        0        0 2023-06-26 14:32:45.000000 algogears-1.1.0/tests/entities/__init__.py
--rw-rw-rw-   0        0        0     7352 2024-05-12 16:27:14.000000 algogears-1.1.0/tests/entities/test_avl_tree.py
--rw-rw-rw-   0        0        0     1472 2024-05-12 16:27:13.000000 algogears-1.1.0/tests/entities/test_bin_tree.py
--rw-rw-rw-   0        0        0      595 2024-05-12 16:27:13.000000 algogears-1.1.0/tests/entities/test_bin_tree_node.py
--rw-rw-rw-   0        0        0     1855 2024-05-12 16:27:12.000000 algogears-1.1.0/tests/entities/test_threaded_bin_tree.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:14:19.443118 algogears-1.1.1/
+-rw-rw-rw-   0        0        0     1104 2024-01-11 15:42:09.000000 algogears-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1071 2024-05-26 10:14:19.441629 algogears-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2697 2024-05-12 16:50:08.000000 algogears-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 10:14:19.393146 algogears-1.1.1/algogears/
+-rw-rw-rw-   0        0        0        0 2023-07-23 17:47:02.000000 algogears-1.1.1/algogears/__init__.py
+-rw-rw-rw-   0        0        0    19561 2024-05-26 09:09:56.000000 algogears-1.1.1/algogears/core.py
+-rw-rw-rw-   0        0        0    10727 2024-05-26 09:04:16.000000 algogears-1.1.1/algogears/dynamic_hull.py
+-rw-rw-rw-   0        0        0     3449 2024-05-25 13:49:24.000000 algogears-1.1.1/algogears/graham.py
+-rw-rw-rw-   0        0        0      920 2023-06-22 10:15:40.000000 algogears-1.1.1/algogears/jarvis.py
+-rw-rw-rw-   0        0        0     3113 2024-05-25 15:50:32.000000 algogears-1.1.1/algogears/kd_tree.py
+-rw-rw-rw-   0        0        0     4028 2024-05-25 15:58:43.000000 algogears-1.1.1/algogears/preparata.py
+-rw-rw-rw-   0        0        0     3193 2024-05-25 15:50:54.000000 algogears-1.1.1/algogears/quickhull.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:14:19.440613 algogears-1.1.1/algogears.egg-info/
+-rw-rw-rw-   0        0        0     1071 2024-05-26 10:14:19.000000 algogears-1.1.1/algogears.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2024-05-26 10:14:19.000000 algogears-1.1.1/algogears.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 10:14:19.000000 algogears-1.1.1/algogears.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-26 10:14:19.000000 algogears-1.1.1/algogears.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-06-22 19:12:11.000000 algogears-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 10:14:19.443118 algogears-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1366 2024-05-26 10:11:28.000000 algogears-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:14:19.421625 algogears-1.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:57:15.000000 algogears-1.1.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:14:19.426517 algogears-1.1.1/tests/algorithms/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:57:09.000000 algogears-1.1.1/tests/algorithms/__init__.py
+-rw-rw-rw-   0        0        0    15076 2024-05-26 10:09:31.000000 algogears-1.1.1/tests/algorithms/test_dynamic_hull.py
+-rw-rw-rw-   0        0        0     5734 2024-05-25 13:50:07.000000 algogears-1.1.1/tests/algorithms/test_graham.py
+-rw-rw-rw-   0        0        0      655 2024-05-25 14:06:04.000000 algogears-1.1.1/tests/algorithms/test_jarvis.py
+-rw-rw-rw-   0        0        0     2803 2024-05-25 15:46:19.000000 algogears-1.1.1/tests/algorithms/test_kd_tree.py
+-rw-rw-rw-   0        0        0     5365 2024-05-25 15:25:02.000000 algogears-1.1.1/tests/algorithms/test_preparata.py
+-rw-rw-rw-   0        0        0     3450 2024-05-25 14:04:37.000000 algogears-1.1.1/tests/algorithms/test_quickhull.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:14:19.439614 algogears-1.1.1/tests/entities/
+-rw-rw-rw-   0        0        0        0 2023-06-26 14:32:45.000000 algogears-1.1.1/tests/entities/__init__.py
+-rw-rw-rw-   0        0        0     7938 2024-05-25 12:59:05.000000 algogears-1.1.1/tests/entities/test_avl_tree.py
+-rw-rw-rw-   0        0        0     1459 2024-05-25 13:02:25.000000 algogears-1.1.1/tests/entities/test_bin_tree.py
+-rw-rw-rw-   0        0        0      699 2024-05-25 13:00:51.000000 algogears-1.1.1/tests/entities/test_bin_tree_node.py
+-rw-rw-rw-   0        0        0     1955 2024-05-25 13:03:09.000000 algogears-1.1.1/tests/entities/test_threaded_bin_tree.py
```

### Comparing `algogears-1.1.0/LICENSE` & `algogears-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `algogears-1.1.0/PKG-INFO` & `algogears-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algogears
-Version: 1.1.0
+Version: 1.1.1
 Summary: This library contains implementations of computational geometry algorithms in Python3 adapted for educational purposes.
 Author: artandfi (Artem Fisunenko)
 Author-email: artem.fisunenko@hotmail.com
 Keywords: Python3,computational geometry,convex hull,region search,geometric search,point location,proximity,closest pair,closest points
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `algogears-1.1.0/README.md` & `algogears-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `algogears-1.1.0/algogears/core.py` & `algogears-1.1.1/algogears/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from enum import Enum
 from math import inf, pi, acos, atan2, isclose
 from typing import Iterable, Generator, Any, ClassVar
 from pydantic import BaseModel
 
 
 class Vector(BaseModel):
-    coords: Iterable[float]
+    coords: list[float]
     
     @property
     def x(self) -> float:
         return self.coords[0]
     
     @property
     def y(self) -> float:
@@ -57,31 +57,35 @@
         self.coords = tuple(c / self.norm(metric) for c in self.coords)
     
     def __str__(self) -> str:
         return f"({', '.join(str(c) for c in self.coords)})"
 
 
 class Point(BaseModel):
-    coords: Iterable[float]
+    coords: tuple[float, ...]
     
+    @classmethod
+    def new(cls, *coords):
+        return cls(coords=coords)
+
     @property
     def x(self) -> float:
         return self.coords[0]
     
     @property
     def y(self) -> float:
         return self.coords[1]
     
     @property
     def z(self) -> float:
         return self.coords[2]
     
     @classmethod
     def centroid(cls, *points: Iterable[Point]) -> Point:
-        return cls(*(sum(coord) / len(coord) for coord in zip(*points)))
+        return cls.new(*(sum(coords) / len(coords) for coords in zip(*[p.coords for p in points])))
     
     @staticmethod
     def angle(point1: Point, point2: Point, point3: Point) -> float:
         v1 = Vector.from_points(point2, point1)
         v2 = Vector.from_points(point2, point3)
         v1.normalize()
         v2.normalize()
@@ -169,21 +173,21 @@
         
         return self > other or self == other
 
     def __add__(self, other: Point) -> bool:
         if not isinstance(other, self.__class__):
             raise TypeError(f"right operand of addition must be of {self.__class__} type")
         
-        return self.__class__(*(c1 + c2 for c1, c2 in zip(self.coords, other.coords)))
+        return self.__class__.new(*(c1 + c2 for c1, c2 in zip(self.coords, other.coords)))
     
     def __sub__(self, other: Point) -> bool:
         if not isinstance(other, self.__class__):
             raise TypeError(f"right operand of subtraction must be of {self.__class__} type")
         
-        return self.__class__(*(c1 - c2 for c1, c2 in zip(self.coords, other.coords)))
+        return self.__class__.new(*(c1 - c2 for c1, c2 in zip(self.coords, other.coords)))
     
     def __hash__(self) -> int:
         return hash(self.coords)
     
     def __str__(self) -> str:
         return f"({', '.join(str(c) for c in self.coords)})"
 
@@ -329,35 +333,32 @@
             and self.left == other.left
             and self.right == other.right
         )
     
 
 class BinTree(BaseModel):
     node_class: ClassVar[type] = BinTreeNode
-    root: BinTreeNode
+    root: BinTreeNode | None = None
 
-    def __init__(self, root):
-        self.root = root
-    
     @classmethod
     def from_iterable(cls, iterable: Iterable) -> BinTree:
         if isinstance(iterable, Generator):
             iterable = list(iterable)
         
-        return cls(root=cls._from_iterable(iterable)) if iterable else cls(None)
+        return cls(root=cls._from_iterable(iterable)) if iterable else cls(root=None)
     
     @classmethod
     def _from_iterable(cls, iterable: Iterable, left: int = 0, right: int | None = None) -> BinTreeNode:
         if right is None:
             right = len(iterable) - 1
         if left > right:
             return None
         
         mid = (left + right) // 2
-        node = cls.node_class(iterable[mid])
+        node = cls.node_class(data=iterable[mid])
         node.left = cls._from_iterable(iterable, left, mid-1)
         node.right = cls._from_iterable(iterable, mid+1, right)
         node.set_height()
 
         return node
     
     @classmethod
@@ -405,15 +406,15 @@
             starting_node = self.root
 
         self.root = self._delete(data, starting_node)
 
     def _insert(self, data: Any, node: BinTreeNode | None = None) -> BinTreeNode:
         data_is_node = isinstance(data, self.node_class)
         if node is None:
-            return data if data_is_node else BinTreeNode(data)
+            return data if data_is_node else BinTreeNode(data=data)
         
         value = data.data if data_is_node else data
         if value < node.data:
             node.left = self._insert(data, node.left)
         else:
             node.right = self._insert(data, node.right)
```

### Comparing `algogears-1.1.0/algogears/graham.py` & `algogears-1.1.1/algogears/graham.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,110 +1,104 @@
 from math import pi
-from .core import PyCGAObject, Point
+from typing import Iterable
+from pydantic import BaseModel, Field
+from .core import Point
 
 
-class GrahamStepsTableRow(PyCGAObject):
-    def __init__(self, point_triple, is_angle_less_than_pi):
-        self.point_triple = point_triple
-        self.is_angle_less_than_pi = is_angle_less_than_pi
-
+class GrahamStepsTableRow(BaseModel):
+    point_triple: tuple[Point, Point, Point]
+    is_angle_less_than_pi: bool
+    
     def __eq__(self, other):
         return (
             isinstance(other, self.__class__) and
             self.point_triple == other.point_triple and
             self.is_angle_less_than_pi == other.is_angle_less_than_pi
         )
-    
-    def __str__(self):
+
+    def __str__(self) -> str:
         return f"[{str(self.point_triple)}, {str(self.is_angle_less_than_pi)}]"
-    
-    def __repr__(self):
-        return str(self)
 
 
-class GrahamStepsTable(PyCGAObject):
-    def __init__(self, ordered_points, rows=None):
-        super().__init__()
-        self.ordered_points = ordered_points
-        self.rows = rows if rows else []
+class GrahamStepsTable(BaseModel):
+    ordered_points: list[Point]
+    rows: list[GrahamStepsTableRow] = Field(default_factory=list)
     
-    def append(self, item):
+    def append(self, item: GrahamStepsTableRow) -> None:
         self.rows.append(item)
     
-    def extend(self, iterable):
+    def extend(self, iterable: Iterable[GrahamStepsTableRow]) -> None:
         self.rows.extend(iterable)
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: int) -> GrahamStepsTableRow:
         return self.rows[key]
     
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: int, value: GrahamStepsTableRow) -> None:
         self.rows[key] = value
 
     def __eq__(self, other):
         return (
             isinstance(other, self.__class__) and
             self.ordered_points == other.ordered_points and
             self.rows == other.rows
         )
 
     def __str__(self):
         return f"[{', '.join(str(row) for row in self)}]"
-    
-    def __repr__(self):
-        return str(self)
 
 
-def graham(points):
+def graham(points: Iterable[Point]):
     if len(points) < 3:
         yield sorted(points, key=lambda p: (p.y, -p.x))
     else:
         i = 2
         while Point.direction(points[0], points[1], points[i]) == 0:
             i += 1
         
         centroid = Point.centroid(points[0], points[1], points[i])
         yield centroid
 
         origin = min(points, key=lambda p: (p.y, -p.x))
-        ordered_points = sort_points(points, centroid, origin)
+        ordered_points = sorted_points(points, centroid, origin)
         yield ordered_points
         yield origin
 
         ordered_points.append(origin)
-        steps_table = GrahamStepsTable(ordered_points)
+        steps_table = GrahamStepsTable(ordered_points=ordered_points)
         hull = make_hull(steps_table, ordered_points)
         ordered_points.pop()
+        steps_table.ordered_points.pop()
         
-        yield [row.point_triple for row in steps_table]
-        yield [row.is_angle_less_than_pi for row in steps_table]
+        yield [row.point_triple for row in steps_table.rows]
+        yield [row.is_angle_less_than_pi for row in steps_table.rows]
         yield steps_table
         yield steps_table
         yield steps_table
         
         yield hull
 
 
-def sort_points(points, centroid, origin):
+def sorted_points(points: list[Point], centroid: Point, origin: Point) -> list[Point]:
     min_angle = Point.polar_angle(origin, centroid)
 
     def angle_and_dist(p):
         p_angle = Point.polar_angle(p, centroid)
         angle = p_angle if p_angle >= min_angle else 2 * pi + p_angle
         return (angle, Point.dist(p, centroid))
 
     return sorted(points, key=angle_and_dist)
 
 
-def make_hull(steps_table, ordered_points):
+def make_hull(steps_table: GrahamStepsTable, ordered_points: list[Point]) -> list[Point]:
     res = ordered_points[:2]
 
     for point in ordered_points[2:]:
         while len(res) > 1 and Point.direction(res[-2], res[-1], point) >= 0:
-            steps_table.append(GrahamStepsTableRow((res[-2], res[-1], point), False))
+            steps_table.append(GrahamStepsTableRow(point_triple=(res[-2], res[-1], point), is_angle_less_than_pi=False))
             res.pop()
 
         if len(res) > 1:
-            steps_table.append(GrahamStepsTableRow((res[-2], res[-1], point), True))
+            steps_table.append(GrahamStepsTableRow(point_triple=(res[-2], res[-1], point), is_angle_less_than_pi=True))
         
         res.append(point)
 
     return res[:-1]
```

### Comparing `algogears-1.1.0/algogears/jarvis.py` & `algogears-1.1.1/algogears/jarvis.py`

 * *Files identical despite different names*

### Comparing `algogears-1.1.0/algogears/preparata.py` & `algogears-1.1.1/algogears/preparata.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,38 @@
+from __future__ import annotations
+from typing import Any, ClassVar, Iterable
 from .core import Point, ThreadedBinTreeNode, ThreadedBinTree, PointType, PathDirection
 
 
 class PreparataNode(ThreadedBinTreeNode):
+    data: Point
+    left: PreparataNode | None = None
+    right: PreparataNode | None = None
+    prev: PreparataNode | None = None
+    next: PreparataNode | None = None
+
     @property
-    def point(self):
+    def point(self) -> Point:
         return self.data
     
     @point.setter
-    def point(self, value):
+    def point(self, value: Point) -> None:
         self.data = value
     
     @point.deleter
-    def point(self):
+    def point(self) -> None:
         del self.data
 
 
 class PreparataThreadedBinTree(ThreadedBinTree):
-    node_class = PreparataNode
+    node_class: ClassVar[type] = PreparataNode
+    root: PreparataNode | None = None
 
 
-def preparata(points):
+def preparata(points: Iterable):
     points.sort()
 
     if len(points) < 3:
         yield points
     else:
         # Find first three non-collinear points
         i = 2
@@ -63,29 +72,29 @@
         yield hulls[0], trees[0]
         yield (left_paths, left_supporting_points), (right_paths, right_supporting_points)
         yield deleted_points
         yield hulls[1:], trees[1:]
         yield hull
 
 
-def find_path_to_supporting_point(tree, point, search_left_supporting):
+def find_path_to_supporting_point(tree: PreparataThreadedBinTree, point: Point, search_left_supporting: bool) -> tuple[list[PathDirection], Point]:
     path = []
     node, prev = tree.root, None
     
     while prev != node:
         prev = node
         node = find_next_node(node, point, search_left_supporting)
         
         if node is not prev:
             path.append(PathDirection.left if node is prev.prev else PathDirection.right)
     
     return path, node.point
 
 
-def find_next_node(node, point, search_left_supporting):
+def find_next_node(node: PreparataNode, point: Point, search_left_supporting: bool) -> PreparataNode:
     point_type = PointType.by_points(point, node.point, node.prev.point, node.next.point)
     match point_type:
         case PointType.convex:
             return node.next if search_left_supporting else node.prev
         case PointType.reflex:
             return node.prev if search_left_supporting else node.next
         case PointType.left_supporting:
```

### Comparing `algogears-1.1.0/algogears.egg-info/PKG-INFO` & `algogears-1.1.1/algogears.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algogears
-Version: 1.1.0
+Version: 1.1.1
 Summary: This library contains implementations of computational geometry algorithms in Python3 adapted for educational purposes.
 Author: artandfi (Artem Fisunenko)
 Author-email: artem.fisunenko@hotmail.com
 Keywords: Python3,computational geometry,convex hull,region search,geometric search,point location,proximity,closest pair,closest points
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `algogears-1.1.0/algogears.egg-info/SOURCES.txt` & `algogears-1.1.1/algogears.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `algogears-1.1.0/setup.py` & `algogears-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="algogears",
-    version="1.1.0",
+    version="1.1.1",
     author="artandfi (Artem Fisunenko)",
     author_email="artem.fisunenko@hotmail.com",
     description="This library contains implementations of computational geometry algorithms in Python3 adapted for educational purposes.",
     long_description="AlgoGEARS (Algorithms of (Computational) Geometry with Entities Available for Reuse and Serialization) is a library that provides implementations of certain computational geometry algorithms adapted for educational purposes." 
                      "The basic entities it uses, such as geometric objects and binary trees, are constructed as Pydantic models that can be easily reused and serialized."
                      "This library is a continuation of PyCompGeomAlgorithms https://pypi.org/project/PyCompGeomAlgorithms/, a library by the same author as this one--artandfi (Artem Fisunenko).",
     packages=find_packages(),
```

### Comparing `algogears-1.1.0/tests/algorithms/test_dynamic_hull.py` & `algogears-1.1.1/tests/algorithms/test_dynamic_hull.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,93 @@
 from copy import deepcopy
 from algogears.core import Point
 from algogears.dynamic_hull import DynamicHullNode, SubhullThreadedBinTree, DynamicHullTree, PathDirection, upper_dynamic_hull, merge
 
 
 def test_dynamic_hull1():
-    p2, p1, p3 = Point(3, 3), Point(1, 1), Point(5, 0)
+    p2, p1, p3 = Point.new(3, 3), Point.new(1, 1), Point.new(5, 0)
     pts = [p2, p1, p3]
-    root = DynamicHullNode(p2, [p1, p2, p3], 1)
-    root.left = DynamicHullNode(p1, [p1, p2])
+    root = DynamicHullNode(data=p2, subhull=[p1, p2, p3], left_supporting_index=1, left_supporting=p2, right_supporting=p3)
+    root.left = DynamicHullNode(data=p1, subhull=[p1, p2], left_supporting=p1, right_supporting=p2)
     root.left.left = DynamicHullNode.leaf(p1)
     root.left.right = DynamicHullNode.leaf(p2)
     root.right = DynamicHullNode.leaf(p3)
-    tree = DynamicHullTree(root)
+    tree = DynamicHullTree(root=root)
     
     tree.root.optimized_subhull = tree.root.subhull
-    tree.root.left.optimized_subhull = SubhullThreadedBinTree.empty()
-    tree.root.left.left.optimized_subhull = SubhullThreadedBinTree.empty()
-    tree.root.left.right.optimized_subhull = SubhullThreadedBinTree.empty()
-    tree.root.right.optimized_subhull = SubhullThreadedBinTree.empty()
     
     leaves = [root.left.left, root.left.right, root.right]
     path = [PathDirection.right]
-    point_to_insert = Point(4, 3)
+    point_to_insert = Point.new(4, 3)
     hull = [p1, p2, point_to_insert, p3]
 
     ans = upper_dynamic_hull(pts, point_to_insert)
 
     assert leaves == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert path == next(ans)
 
-    tree.root.subhull = SubhullThreadedBinTree.from_iterable(hull)
-    tree.root.optimized_subhull = tree.root.subhull
-    tree.root.right = DynamicHullNode(point_to_insert, [point_to_insert, p3])
-    tree.root.right.optimized_subhull = SubhullThreadedBinTree.empty()
+    tree.root.subhull = hull
+    tree.root.optimized_subhull = hull
+    tree.root.right_supporting = point_to_insert
+    tree.root.right = DynamicHullNode(data=point_to_insert, subhull=[point_to_insert, p3], left_supporting=point_to_insert, right_supporting=p3)
     tree.root.right.left = DynamicHullNode.leaf(point_to_insert)
-    tree.root.right.left.optimized_subhull = SubhullThreadedBinTree.empty()
     tree.root.right.right = DynamicHullNode.leaf(p3)
-    tree.root.right.right.optimized_subhull = SubhullThreadedBinTree.empty()
 
     assert (tree, hull) == next(ans)
     assert hull == next(ans)
 
 
 def test_dynamic_hull2():
     pts = p5, p9, p4, p2, p6, p8, p3, p10, p7, p1, p11 = [
-        Point(3, 10),
-        Point(6, 8),
-        Point(3, 5),
-        Point(2, 8),
-        Point(4, 8),
-        Point(5, 5),
-        Point(3, 3),
-        Point(7, 7),
-        Point(5, 0),
-        Point(0, 0),
-        Point(10, 3)
+        Point.new(3, 10),
+        Point.new(6, 8),
+        Point.new(3, 5),
+        Point.new(2, 8),
+        Point.new(4, 8),
+        Point.new(5, 5),
+        Point.new(3, 3),
+        Point.new(7, 7),
+        Point.new(5, 0),
+        Point.new(0, 0),
+        Point.new(10, 3)
     ]
-    root = DynamicHullNode(p6, [p1, p2, p5, p9, p10, p11], 2)
-    root.left = DynamicHullNode(p3, [p1, p2, p5, p6], 1)
-    root.left.left = DynamicHullNode(p2, [p1, p2, p3], 1)
-    root.left.left.left = DynamicHullNode(p1, [p1, p2])
+    root = DynamicHullNode(data=p6, subhull=[p1, p2, p5, p9, p10, p11], left_supporting_index=2, left_supporting=p5, right_supporting=p9)
+    root.left = DynamicHullNode(data=p3, subhull=[p1, p2, p5, p6], left_supporting_index=1, left_supporting=p2, right_supporting=p5)
+    root.left.left = DynamicHullNode(data=p2, subhull=[p1, p2, p3], left_supporting_index=1, left_supporting=p2, right_supporting=p3)
+    root.left.left.left = DynamicHullNode(data=p1, subhull=[p1, p2], left_supporting=p1, right_supporting=p2)
     root.left.left.left.left = DynamicHullNode.leaf(p1)
     root.left.left.left.right = DynamicHullNode.leaf(p2)
     root.left.left.right = DynamicHullNode.leaf(p3)
-    root.left.right = DynamicHullNode(p5, [p5, p6])
-    root.left.right.left = DynamicHullNode(p4, [p5])
+    root.left.right = DynamicHullNode(data=p5, subhull=[p5, p6], left_supporting=p5, right_supporting=p6)
+    root.left.right.left = DynamicHullNode(data=p4, subhull=[p5], left_supporting=p5, right_supporting=p5)
     root.left.right.left.left = DynamicHullNode.leaf(p4)
     root.left.right.left.right = DynamicHullNode.leaf(p5)
     root.left.right.right = DynamicHullNode.leaf(p6)
-    root.right = DynamicHullNode(p9, [p8, p9, p10, p11], 1)
-    root.right.left = DynamicHullNode(p8, [p8, p9])
-    root.right.left.left = DynamicHullNode(p7, [p8])
+    root.right = DynamicHullNode(data=p9, subhull=[p8, p9, p10, p11], left_supporting_index=1, left_supporting=p9, right_supporting=p10)
+    root.right.left = DynamicHullNode(data=p8, subhull=[p8, p9], left_supporting=p8, right_supporting=p9)
+    root.right.left.left = DynamicHullNode(data=p7, subhull=[p8], left_supporting=p8, right_supporting=p8)
     root.right.left.left.left = DynamicHullNode.leaf(p7)
     root.right.left.left.right = DynamicHullNode.leaf(p8)
     root.right.left.right = DynamicHullNode.leaf(p9)
-    root.right.right = DynamicHullNode(p10, [p10, p11])
+    root.right.right = DynamicHullNode(data=p10, subhull=[p10, p11], left_supporting=p10, right_supporting=p11)
     root.right.right.left = DynamicHullNode.leaf(p10)
     root.right.right.right = DynamicHullNode.leaf(p11)
-    tree = DynamicHullTree(root)
+    tree = DynamicHullTree(root=root)
 
     tree.root.optimized_subhull = tree.root.subhull
-    tree.root.left.optimized_subhull = SubhullThreadedBinTree.from_iterable([p6])
-    tree.root.left.left.optimized_subhull = SubhullThreadedBinTree.from_iterable([p3])
-    tree.root.left.right.left.left.optimized_subhull = SubhullThreadedBinTree.from_iterable([p4])
-    tree.root.right.optimized_subhull = SubhullThreadedBinTree.from_iterable([p8])
-    tree.root.right.left.left.left.optimized_subhull = SubhullThreadedBinTree.from_iterable([p7])
+    tree.root.left.optimized_subhull = [p6]
+    tree.root.left.left.optimized_subhull = [p3]
+    tree.root.left.right.left.left.optimized_subhull = [p4]
+    tree.root.right.optimized_subhull = [p8]
+    tree.root.right.left.left.left.optimized_subhull = [p7]
 
     leaves = tree.leaves_inorder()
     path = [PathDirection.left, PathDirection.right, PathDirection.left, PathDirection.right]
     point_to_delete = p5
     hull = [p1, p2, p9, p10, p11]
 
     ans = upper_dynamic_hull(pts, point_to_delete)
@@ -102,230 +96,245 @@
     assert tree == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert path == next(ans)
 
-    tree.root.subhull = SubhullThreadedBinTree.from_iterable([p1, p2, p9, p10, p11])
+    tree.root.subhull = [p1, p2, p9, p10, p11]
     tree.root.optimized_subhull = tree.root.subhull
     tree.root.left_supporting_index = 1
+    tree.root.left_supporting = p2
+    tree.root.right_supporting = p9
     
-    tree.root.left.subhull = SubhullThreadedBinTree.from_iterable([p1, p2, p6])
+    tree.root.left.subhull = [p1, p2, p6]
+    tree.root.left.right_supporting = p6
+
     tree.root.left.right.left.right = tree.root.left.right.right
     tree.root.left.right = tree.root.left.right.left
-    tree.root.left.right.subhull = SubhullThreadedBinTree.from_iterable([p4, p6])
-    tree.root.left.right.optimized_subhull = SubhullThreadedBinTree.from_iterable([p4])
-    tree.root.left.right.left.optimized_subhull = SubhullThreadedBinTree.empty()
+    tree.root.left.right.subhull = [p4, p6]
+    tree.root.left.right.optimized_subhull = [p4]
+    tree.root.left.right.left_supporting = p4
+    tree.root.left.right.right_supporting = p6
+
+    tree.root.left.right.left.optimized_subhull = []
 
     assert (tree, hull) == next(ans)
     assert hull == next(ans)
 
 
 def test_dynamic_hull3():
     """Vertical line, only upper point"""
-    pts = p1, p2, p3, p4, p5 = [Point(0, i) for i in range(5)]
-    root = DynamicHullNode(p3, [p5])
-    root.left = DynamicHullNode(p2, [p3])
-    root.left.left = DynamicHullNode(p1, [p2])
+    pts = p1, p2, p3, p4, p5 = [Point.new(0, i) for i in range(5)]
+    root = DynamicHullNode(data=p3, subhull=[p5], left_supporting=p5, right_supporting=p5)
+    root.left = DynamicHullNode(data=p2, subhull=[p3], left_supporting=p3, right_supporting=p3)
+    root.left.left = DynamicHullNode(data=p1, subhull=[p2], left_supporting=p2, right_supporting=p2)
     root.left.left.left = DynamicHullNode.leaf(p1)
     root.left.left.right = DynamicHullNode.leaf(p2)
     root.left.right = DynamicHullNode.leaf(p3)
-    root.right = DynamicHullNode(p4, [p5])
+    root.right = DynamicHullNode(data=p4, subhull=[p5], left_supporting=p5, right_supporting=p5)
     root.right.left = DynamicHullNode.leaf(p4)
     root.right.right = DynamicHullNode.leaf(p5)
-    tree = DynamicHullTree(root)
+    tree = DynamicHullTree(root=root)
 
     tree.root.optimized_subhull = tree.root.subhull
     tree.root.left.optimized_subhull = tree.root.left.subhull
     tree.root.left.left.optimized_subhull = tree.root.left.left.subhull
     tree.root.left.left.left.optimized_subhull = tree.root.left.left.left.subhull
     tree.root.right.left.optimized_subhull = tree.root.right.left.subhull
 
     leaves = tree.leaves_inorder()
     path = [PathDirection.right] * 2
-    point_to_insert = Point(0, 6)
+    point_to_insert = Point.new(0, 6)
     hull = [point_to_insert]
 
     ans = upper_dynamic_hull(pts, point_to_insert)
 
     assert leaves == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert path == next(ans)
 
-    tree.root.subhull = SubhullThreadedBinTree.from_iterable([point_to_insert])
+    tree.root.subhull = [point_to_insert]
     tree.root.optimized_subhull = tree.root.subhull
-    tree.root.right.subhull = SubhullThreadedBinTree.from_iterable([point_to_insert])
-    tree.root.right.right = DynamicHullNode(p5, [point_to_insert])
-    tree.root.right.right.left = DynamicHullNode(p5, [p5])
-    tree.root.right.right.left.optimized_subhull = tree.root.right.right.left.subhull
-    tree.root.right.right.right = DynamicHullNode(point_to_insert, [point_to_insert])
+    tree.root.left_supporting = point_to_insert
+    tree.root.right_supporting = point_to_insert
+
+    tree.root.right.subhull = [point_to_insert]
+    tree.root.right.left_supporting = point_to_insert
+    tree.root.right.right_supporting = point_to_insert
+
+    tree.root.right.right = DynamicHullNode(data=p5, subhull=[point_to_insert], left_supporting=point_to_insert, right_supporting=point_to_insert)
+    tree.root.right.right.left = DynamicHullNode.leaf(p5)
+    tree.root.right.right.left.optimized_subhull = [p5]
+    
+    tree.root.right.right.right = DynamicHullNode.leaf(point_to_insert)
     
     assert (tree, hull) == next(ans)
     assert hull == next(ans)
 
 
 def test_dynamic_hull4():
     """Horizontal line, segment of only extreme left and right points"""
-    pts = p1, p2, p3, p4, p5 = [Point(i, 0) for i in range(1, 6)]
-    root = DynamicHullNode(p3, [p1, p5])
-    root.left = DynamicHullNode(p2, [p1, p3])
-    root.left.left = DynamicHullNode(p1, [p1, p2])
+    pts = p1, p2, p3, p4, p5 = [Point.new(i, 0) for i in range(1, 6)]
+    root = DynamicHullNode(data=p3, subhull=[p1, p5], left_supporting=p1, right_supporting=p5)
+    root.left = DynamicHullNode(data=p2, subhull=[p1, p3], left_supporting=p1, right_supporting=p3)
+    root.left.left = DynamicHullNode(data=p1, subhull=[p1, p2], left_supporting=p1, right_supporting=p2)
     root.left.left.left = DynamicHullNode.leaf(p1)
     root.left.left.right = DynamicHullNode.leaf(p2)
     root.left.right = DynamicHullNode.leaf(p3)
-    root.right = DynamicHullNode(p4, [p4, p5])
+    root.right = DynamicHullNode(data=p4, subhull=[p4, p5], left_supporting=p4, right_supporting=p5)
     root.right.left = DynamicHullNode.leaf(p4)
     root.right.right = DynamicHullNode.leaf(p5)
-    tree = DynamicHullTree(root)
+    tree = DynamicHullTree(root=root)
 
     tree.root.optimized_subhull = tree.root.subhull
-    tree.root.left.optimized_subhull = SubhullThreadedBinTree.from_iterable([p3])
-    tree.root.left.left.optimized_subhull = SubhullThreadedBinTree.from_iterable([p2])
-    tree.root.right.optimized_subhull = SubhullThreadedBinTree.from_iterable([p4])
+    tree.root.left.optimized_subhull = [p3]
+    tree.root.left.left.optimized_subhull = [p2]
+    tree.root.right.optimized_subhull = [p4]
 
     leaves = tree.leaves_inorder()
     path = [PathDirection.left] * 3
-    point_to_insert = Point(0, 0)
+    point_to_insert = Point.new(0, 0)
     hull = [point_to_insert, p5]
 
     ans = upper_dynamic_hull(pts, point_to_insert)
 
     assert leaves == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert tree == next(ans)
     assert path == next(ans)
 
-    tree.root.subhull = SubhullThreadedBinTree.from_iterable(hull)
+    tree.root.subhull = hull
     tree.root.optimized_subhull = tree.root.subhull
+    tree.root.left_supporting = point_to_insert
 
-    tree.root.left = DynamicHullNode(p1, [point_to_insert, p3], optimized_subhull_points=[p3])
-    tree.root.left.left = DynamicHullNode(point_to_insert, [point_to_insert, p1], optimized_subhull_points=[p1])
+    tree.root.left = DynamicHullNode(data=p1, subhull=[point_to_insert, p3], optimized_subhull=[p3], left_supporting=point_to_insert, right_supporting=p3)
+    tree.root.left.left = DynamicHullNode(data=point_to_insert, subhull=[point_to_insert, p1], optimized_subhull=[p1], left_supporting=point_to_insert, right_supporting=p1)
     tree.root.left.left.left = DynamicHullNode.leaf(point_to_insert)
     tree.root.left.left.right = DynamicHullNode.leaf(p1)
-    tree.root.left.right = DynamicHullNode(p2, [p2, p3], optimized_subhull_points=[p2])
+    tree.root.left.right = DynamicHullNode(data=p2, subhull=[p2, p3], optimized_subhull=[p2], left_supporting=p2, right_supporting=p3)
     tree.root.left.right.left = DynamicHullNode.leaf(p2)
     tree.root.left.right.right = DynamicHullNode.leaf(p3)
 
     assert (tree, hull) == next(ans)
     assert hull == next(ans)
 
 
 def make_two_segment_nodes(points):
     p1, p2, p3, p4 = points
     n1, n2, n3, n4 = [DynamicHullNode.leaf(p) for p in points]
 
-    segment_node1 = DynamicHullNode(p1, [p1, p2])
+    segment_node1 = DynamicHullNode(data=p1, subhull=[p1, p2], left_supporting=p1, right_supporting=p2)
     segment_node1.left, segment_node1.right = n1, n2
-    segment_node2 = DynamicHullNode(p3, [p3, p4])
+    segment_node2 = DynamicHullNode(data=p3, subhull=[p3, p4], left_supporting=p3, right_supporting=p4)
     segment_node2.left, segment_node2.right = n3, n4
     
     return segment_node1, segment_node2
 
 
 def test_merge_segments1():
     """Hull is p1-p4"""
-    pts = [Point(0, 2), Point(1, 0), Point(3, 1), Point(4, 3)]
+    pts = [Point.new(0, 2), Point.new(1, 0), Point.new(3, 1), Point.new(4, 3)]
     p1, p2, p3, p4 = pts
 
     segment_node1, segment_node2 = make_two_segment_nodes(pts)
-    joint_node = DynamicHullNode(p2, [p1, p4])
+    joint_node = DynamicHullNode(data=p2, subhull=[p1, p4], left_supporting=p1, right_supporting=p4)
     joint_node.left, joint_node.right = segment_node1, segment_node2
 
     assert joint_node == merge(segment_node1, segment_node2)
 
 
 def test_merge_segments2():
     """Hull is p1-p2-p4, p3 is below p1-p4"""
-    pts = [Point(1, 1), Point(2, 4), Point(3, 1), Point(4, 2)]
+    pts = [Point.new(1, 1), Point.new(2, 4), Point.new(3, 1), Point.new(4, 2)]
     p1, p2, p3, p4 = pts
 
     segment_node1, segment_node2 = make_two_segment_nodes(pts)
-    joint_node = DynamicHullNode(p2, [p1, p2, p4], 1)
+    joint_node = DynamicHullNode(data=p2, subhull=[p1, p2, p4], left_supporting_index=1, left_supporting=p2, right_supporting=p4)
     joint_node.left, joint_node.right = segment_node1, segment_node2
 
     assert joint_node == merge(segment_node1, segment_node2)
 
 
 def test_merge_segments3():
     """Hull is p1-p2-p4, p3 is above p1-p4"""
-    pts = [Point(1, 1), Point(2, 4), Point(3, 2), Point(4, 2)]
+    pts = [Point.new(1, 1), Point.new(2, 4), Point.new(3, 2), Point.new(4, 2)]
     p1, p2, p3, p4 = pts
 
     segment_node1, segment_node2 = make_two_segment_nodes(pts)
-    joint_node = DynamicHullNode(p2, [p1, p2, p4], 1)
+    joint_node = DynamicHullNode(data=p2, subhull=[p1, p2, p4], left_supporting_index=1, left_supporting=p2, right_supporting=p4)
     joint_node.left, joint_node.right = segment_node1, segment_node2
 
     assert joint_node == merge(segment_node1, segment_node2)
 
 
 def test_merge_segments4():
     """Hull is p1-p3-p4, p2 is below p1-p4"""
-    pts = [Point(1, 3), Point(2, 1), Point(3, 3), Point(4, 1)]
+    pts = [Point.new(1, 3), Point.new(2, 1), Point.new(3, 3), Point.new(4, 1)]
     p1, p2, p3, p4 = pts
 
     segment_node1, segment_node2 = make_two_segment_nodes(pts)
-    joint_node = DynamicHullNode(p2, [p1, p3, p4])
+    joint_node = DynamicHullNode(data=p2, subhull=[p1, p3, p4], left_supporting=p1, right_supporting=p3)
     joint_node.left, joint_node.right = segment_node1, segment_node2
 
     assert joint_node == merge(segment_node1, segment_node2)
 
 
 def test_merge_segments5():
     """Hull is p1-p3-p4, p2 is above p1-p4"""
-    pts = [Point(1, 3), Point(2, 3), Point(3, 4), Point(4, 1)]
+    pts = [Point.new(1, 3), Point.new(2, 3), Point.new(3, 4), Point.new(4, 1)]
     p1, p2, p3, p4 = pts
 
     segment_node1, segment_node2 = make_two_segment_nodes(pts)
-    joint_node = DynamicHullNode(p2, [p1, p3, p4])
+    joint_node = DynamicHullNode(data=p2, subhull=[p1, p3, p4], left_supporting=p1, right_supporting=p3)
     joint_node.left, joint_node.right = segment_node1, segment_node2
 
     assert joint_node == merge(segment_node1, segment_node2)
 
 
 def test_merge_segments6():
     """Hull is p1-p2-p3-p4"""
-    pts = [Point(1, 1), Point(2, 3), Point(3, 3), Point(4, 1)]
+    pts = [Point.new(1, 1), Point.new(2, 3), Point.new(3, 3), Point.new(4, 1)]
     p1, p2, p3, p4 = pts
 
     segment_node1, segment_node2 = make_two_segment_nodes(pts)
-    joint_node = DynamicHullNode(p2, [p1, p2, p3, p4], 1)
+    joint_node = DynamicHullNode(data=p2, subhull=[p1, p2, p3, p4], left_supporting_index=1, left_supporting=p2, right_supporting=p3)
     joint_node.left, joint_node.right = segment_node1, segment_node2
 
     assert joint_node == merge(segment_node1, segment_node2)
 
 
 def test_merge_segment_and_point1():
     """Segment p1-p2 and point p3, where p2 is above p1-p3."""
-    pts = [Point(0, 1), Point(2, 0), Point(5, 5)]
+    pts = [Point.new(0, 1), Point.new(2, 0), Point.new(5, 5)]
     p1, p2, p3 = pts
     n1, n2, n3 = [DynamicHullNode.leaf(p) for p in pts]
-    segment_node = DynamicHullNode(p1, [p1, p2])
+    segment_node = DynamicHullNode(data=p1, subhull=[p1, p2], left_supporting=p1, right_supporting=p2)
     segment_node.left, segment_node.right = n1, n2
-    point_node = DynamicHullNode(p3, [p3])
+    point_node = DynamicHullNode.leaf(p3)
 
-    joint_node = DynamicHullNode(p2, [p1, p3])
+    joint_node = DynamicHullNode(data=p2, subhull=[p1, p3], left_supporting=p1, right_supporting=p3)
     joint_node.left, joint_node.right = segment_node, n3
 
     assert joint_node == merge(segment_node, point_node)
 
 
 def test_merge_segment_and_point2():
     """Segment p1-p2 and point p3, where p2 is above p1-p3."""
-    pts = [Point(0, 1), Point(2, 3), Point(5, 0)]
+    pts = [Point.new(0, 1), Point.new(2, 3), Point.new(5, 0)]
     p1, p2, p3 = pts
     n1, n2, n3 = [DynamicHullNode.leaf(p) for p in pts]
-    segment_node = DynamicHullNode(p1, [p1, p2])
+    segment_node = DynamicHullNode(data=p1, subhull=[p1, p2], left_supporting=p1, right_supporting=p2)
     segment_node.left, segment_node.right = n1, n2
-    point_node = DynamicHullNode(p3, [p3])
+    point_node = DynamicHullNode.leaf(p3)
 
-    joint_node = DynamicHullNode(p2, [p1, p2, p3], 1)
+    joint_node = DynamicHullNode(data=p2, subhull=[p1, p2, p3], left_supporting_index=1, left_supporting=p2, right_supporting=p3)
     joint_node.left, joint_node.right = segment_node, n3
 
     assert joint_node == merge(segment_node, point_node)
```

### Comparing `algogears-1.1.0/tests/algorithms/test_preparata.py` & `algogears-1.1.1/tests/algorithms/test_preparata.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,125 +1,125 @@
 from algogears.core import Point, PathDirection
 from algogears.preparata import preparata, PreparataThreadedBinTree
 
 
 def test_preparata1():
-    points = [Point(3, 2), Point(2, 4), Point(1, 1), Point(6, 2)]
-    hull0 = [Point(1, 1), Point(2, 4), Point(3, 2)]
-    hull = [Point(1, 1), Point(2, 4), Point(6, 2)]
+    points = [Point.new(3, 2), Point.new(2, 4), Point.new(1, 1), Point.new(6, 2)]
+    hull0 = [Point.new(1, 1), Point.new(2, 4), Point.new(3, 2)]
+    hull = [Point.new(1, 1), Point.new(2, 4), Point.new(6, 2)]
     tree0 = PreparataThreadedBinTree.from_iterable(hull0)
     left_paths = [[PathDirection.right, PathDirection.right]]
     right_paths = [[]]
-    left_supporting_points = [Point(1, 1)]
-    right_supporting_points = [Point(2, 4)]
-    deleted_points = [[Point(3, 2)]]
+    left_supporting_points = [Point.new(1, 1)]
+    right_supporting_points = [Point.new(2, 4)]
+    deleted_points = [[Point.new(3, 2)]]
     hulls = [hull]
     trees = []
     
     ans = preparata(points)
     assert next(ans) == (hull0, tree0)
     assert next(ans) == ((left_paths, left_supporting_points), (right_paths, right_supporting_points))
 
     assert next(ans) == deleted_points
     assert next(ans) == (hulls, trees)
     assert next(ans) == hull
 
 
 def test_preparata2():
     # Corner case for convex (>--X) where one of the angles is equal to pi
-    points = [Point(2, 2), Point(0, 1), Point(4, 3), Point(1, 0)]
-    hull0 = [Point(0, 1), Point(2, 2), Point(1, 0)]
-    hull = [Point(0, 1), Point(4, 3), Point(1, 0)]
+    points = [Point.new(2, 2), Point.new(0, 1), Point.new(4, 3), Point.new(1, 0)]
+    hull0 = [Point.new(0, 1), Point.new(2, 2), Point.new(1, 0)]
+    hull = [Point.new(0, 1), Point.new(4, 3), Point.new(1, 0)]
     tree0 = PreparataThreadedBinTree.from_iterable(hull0)
     left_paths = [[PathDirection.right]]
     right_paths = [[PathDirection.left]]
-    left_supporting_points = [Point(1, 0)]
-    right_supporting_points = [Point(0, 1)]
-    deleted_points = [[Point(2, 2)]]
+    left_supporting_points = [Point.new(1, 0)]
+    right_supporting_points = [Point.new(0, 1)]
+    deleted_points = [[Point.new(2, 2)]]
     hulls = [hull]
     trees = []
 
     ans = preparata(points)
     assert next(ans) == (hull0, tree0)
     assert next(ans) == ((left_paths, left_supporting_points), (right_paths, right_supporting_points))
     assert next(ans) == deleted_points
     assert next(ans) == (hulls, trees)
     assert next(ans) == hull
 
 
 def test_preparata3():
     # Corner case for convex (>--X) where one of the angles is equal to pi
-    points = [Point(1, 2), Point(0, 0), Point(3, 0), Point(5, 0)]
-    hull0 = [Point(0, 0), Point(1, 2), Point(3, 0)]
-    hull = [Point(0, 0), Point(1, 2), Point(5, 0)]
+    points = [Point.new(1, 2), Point.new(0, 0), Point.new(3, 0), Point.new(5, 0)]
+    hull0 = [Point.new(0, 0), Point.new(1, 2), Point.new(3, 0)]
+    hull = [Point.new(0, 0), Point.new(1, 2), Point.new(5, 0)]
     tree0 = PreparataThreadedBinTree.from_iterable(hull0)
     left_paths = [[PathDirection.right, PathDirection.right]]
     right_paths = [[]]
-    left_supporting_points = [Point(0, 0)]
-    right_supporting_points = [Point(1, 2)]
-    deleted_points = [[Point(3, 0)]]
+    left_supporting_points = [Point.new(0, 0)]
+    right_supporting_points = [Point.new(1, 2)]
+    deleted_points = [[Point.new(3, 0)]]
     hulls = [hull]
     trees = []
 
     ans = preparata(points)
     assert next(ans) == (hull0, tree0)
     assert next(ans) == ((left_paths, left_supporting_points), (right_paths, right_supporting_points))
     assert next(ans) == deleted_points
     assert next(ans) == (hulls, trees)
     assert next(ans) == hull
 
 
 def test_preparata4():
     # Corner cases for collinear first points and left and right supporting where one of the angles is 0
-    points = [Point(1, 1), Point(1, 5), Point(5, 3), Point(1, 11), Point(6, 1), Point(10, 1)]
-    hull0 = [Point(1, 1), Point(1, 5), Point(5, 3)]
-    hull = [Point(1, 1), Point(1, 11), Point(10, 1)]
+    points = [Point.new(1, 1), Point.new(1, 5), Point.new(5, 3), Point.new(1, 11), Point.new(6, 1), Point.new(10, 1)]
+    hull0 = [Point.new(1, 1), Point.new(1, 5), Point.new(5, 3)]
+    hull = [Point.new(1, 1), Point.new(1, 11), Point.new(10, 1)]
     tree0 = PreparataThreadedBinTree.from_iterable(hull0)
     left_paths = [
         [PathDirection.right],
         [PathDirection.right, PathDirection.right],
         [PathDirection.right, PathDirection.right]
     ]
     right_paths = [
         [PathDirection.left],
         [],
         []
     ]
     left_supporting_points = [
-        Point(5, 3),
-        Point(1, 1),
-        Point(1, 1)
+        Point.new(5, 3),
+        Point.new(1, 1),
+        Point.new(1, 1)
     ]
     right_supporting_points = [
-        Point(1, 1),
-        Point(1, 11),
-        Point(1, 11)
+        Point.new(1, 1),
+        Point.new(1, 11),
+        Point.new(1, 11)
     ]
-    deleted_points = [[Point(1, 5)], [Point(5, 3)], [Point(6, 1)]]
+    deleted_points = [[Point.new(1, 5)], [Point.new(5, 3)], [Point.new(6, 1)]]
     hulls = [
-        [Point(1, 1), Point(1, 11), Point(5, 3)],
-        [Point(1, 1), Point(1, 11), Point(6, 1)],
+        [Point.new(1, 1), Point.new(1, 11), Point.new(5, 3)],
+        [Point.new(1, 1), Point.new(1, 11), Point.new(6, 1)],
         hull
     ]
     trees = [PreparataThreadedBinTree.from_iterable(hulls[0]), PreparataThreadedBinTree.from_iterable(hulls[1])]
 
     ans = preparata(points)
     assert next(ans) == (hull0, tree0)
     assert next(ans) == ((left_paths, left_supporting_points), (right_paths, right_supporting_points))
     assert next(ans) == deleted_points
     assert next(ans) == (hulls, trees)
     assert next(ans) == hull
 
 
 def test_preparata5():
-    p1 = Point(7, 0)
-    p2 = Point(3, 3)
-    p3 = Point(0, 0)
-    p4 = Point(10, 8)
-    p5 = Point(7, 9)
+    p1 = Point.new(7, 0)
+    p2 = Point.new(3, 3)
+    p3 = Point.new(0, 0)
+    p4 = Point.new(10, 8)
+    p5 = Point.new(7, 9)
     points = [p1, p2, p3, p4, p5]
     hull0 = [p3, p2, p1]
     hull = [p3, p5, p4, p1]
     tree0 = PreparataThreadedBinTree.from_iterable(hull0)
     left_paths = [
         [PathDirection.right],
         [PathDirection.right]
```

### Comparing `algogears-1.1.0/tests/algorithms/test_quickhull.py` & `algogears-1.1.1/tests/algorithms/test_quickhull.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from algogears.core import Point
 from algogears.quickhull import QuickhullNode, QuickhullTree, quickhull
 
 
 def test_quickhull1():
-    pts = [Point(3, 4), Point(0, 0), Point(7, 2)]
+    pts = [Point.new(3, 4), Point.new(0, 0), Point.new(7, 2)]
     hull = [pts[1], pts[0], pts[2]]
-    tree = QuickhullTree(QuickhullNode([pts[1], pts[0], pts[2]], subhull=hull))
-    tree.root.left = QuickhullNode([pts[1], pts[0], pts[2]], h=pts[0], subhull=hull)
-    tree.root.right = QuickhullNode([pts[2], pts[1]], subhull=[pts[2], pts[1]])
-    tree.root.left.left = QuickhullNode([pts[1], pts[0]], subhull=[pts[1], pts[0]])
-    tree.root.left.right = QuickhullNode([pts[0], pts[2]], subhull=[pts[0], pts[2]])
+    tree = QuickhullTree(root=QuickhullNode(data=[pts[1], pts[0], pts[2]], subhull=hull))
+    tree.root.left = QuickhullNode(data=[pts[1], pts[0], pts[2]], h=pts[0], subhull=hull)
+    tree.root.right = QuickhullNode(data=[pts[2], pts[1]], subhull=[pts[2], pts[1]])
+    tree.root.left.left = QuickhullNode(data=[pts[1], pts[0]], subhull=[pts[1], pts[0]])
+    tree.root.left.right = QuickhullNode(data=[pts[0], pts[2]], subhull=[pts[0], pts[2]])
 
     ans = quickhull(pts)
     lp, rp, s1, s2 = next(ans)
     
     assert (lp, rp) == (pts[1], pts[2])
     assert (s1, s2) == ([pts[1], pts[0], pts[2]], [pts[2], pts[1]])
     assert next(ans) == tree
@@ -21,31 +21,31 @@
     assert next(ans) == tree
     assert next(ans) == tree
     assert next(ans) == hull
 
 
 def test_quickhull2():
     pts = [
-        Point(0, 6),
-        Point(8, 11),
-        Point(10, 4),
-        Point(7, 13),
-        Point(6, 3),
-        Point(3, 0),
-        Point(4, 2),
-        Point(12, 1),
-        Point(14, 10),
-        Point(5, 9),
-        Point(3, 11),
-        Point(1, 4),
+        Point.new(0, 6),
+        Point.new(8, 11),
+        Point.new(10, 4),
+        Point.new(7, 13),
+        Point.new(6, 3),
+        Point.new(3, 0),
+        Point.new(4, 2),
+        Point.new(12, 1),
+        Point.new(14, 10),
+        Point.new(5, 9),
+        Point.new(3, 11),
+        Point.new(1, 4),
     ]
     hull = [pts[0], pts[10], pts[3], pts[8], pts[7], pts[5]]
     tree = QuickhullTree(
-        QuickhullNode(
-            [
+        root=QuickhullNode(
+            data=[
                 pts[0],
                 pts[10],
                 pts[9],
                 pts[3],
                 pts[1],
                 pts[8],
                 pts[7],
@@ -56,37 +56,37 @@
                 pts[11],
             ],
             subhull=hull
         )
     )
 
     tree.root.left = QuickhullNode(
-        [pts[0], pts[10], pts[9], pts[3], pts[1], pts[8]],
+        data=[pts[0], pts[10], pts[9], pts[3], pts[1], pts[8]],
         h=pts[3],
         subhull=[pts[0], pts[10], pts[3], pts[8]]
     )
     tree.root.right = QuickhullNode(
-        [pts[8], pts[7], pts[2], pts[4], pts[6], pts[5], pts[11], pts[0]],
+        data=[pts[8], pts[7], pts[2], pts[4], pts[6], pts[5], pts[11], pts[0]],
         h=pts[7],
         subhull=[pts[8], pts[7], pts[5], pts[0]]
     )
 
-    tree.root.left.left = QuickhullNode([pts[0], pts[10], pts[3]], h=pts[10], subhull=[pts[0], pts[10], pts[3]])
-    tree.root.left.right = QuickhullNode([pts[3], pts[8]], subhull=[pts[3], pts[8]])
-    tree.root.left.left.left = QuickhullNode([pts[0], pts[10]], subhull=[pts[0], pts[10]])
-    tree.root.left.left.right = QuickhullNode([pts[10], pts[3]], subhull=[pts[10], pts[3]])
+    tree.root.left.left = QuickhullNode(data=[pts[0], pts[10], pts[3]], h=pts[10], subhull=[pts[0], pts[10], pts[3]])
+    tree.root.left.right = QuickhullNode(data=[pts[3], pts[8]], subhull=[pts[3], pts[8]])
+    tree.root.left.left.left = QuickhullNode(data=[pts[0], pts[10]], subhull=[pts[0], pts[10]])
+    tree.root.left.left.right = QuickhullNode(data=[pts[10], pts[3]], subhull=[pts[10], pts[3]])
 
-    tree.root.right.left = QuickhullNode([pts[8], pts[7]], subhull=[pts[8], pts[7]])
+    tree.root.right.left = QuickhullNode(data=[pts[8], pts[7]], subhull=[pts[8], pts[7]])
     tree.root.right.right = QuickhullNode(
-        [pts[7], pts[4], pts[6], pts[5], pts[11], pts[0]],
+        data=[pts[7], pts[4], pts[6], pts[5], pts[11], pts[0]],
         h=pts[5],
         subhull=[pts[7], pts[5], pts[0]]
     )
-    tree.root.right.right.left = QuickhullNode([pts[7], pts[5]], subhull=[pts[7], pts[5]])
-    tree.root.right.right.right = QuickhullNode([pts[5], pts[0]], subhull=[pts[5], pts[0]])
+    tree.root.right.right.left = QuickhullNode(data=[pts[7], pts[5]], subhull=[pts[7], pts[5]])
+    tree.root.right.right.right = QuickhullNode(data=[pts[5], pts[0]], subhull=[pts[5], pts[0]])
 
     ans = quickhull(pts)
     lp, rp, s1, s2 = next(ans)
 
     assert (lp, rp) == (pts[0], pts[8])
     assert (s1, s2) == (tree.root.left.points, tree.root.right.points)
     assert next(ans) == tree
```

### Comparing `algogears-1.1.0/tests/entities/test_bin_tree_node.py` & `algogears-1.1.1/tests/entities/test_bin_tree_node.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from algogears.core import BinTreeNode
 
 
 def test_bin_tree_node_weak_eq():
-    root1 = BinTreeNode(1, BinTreeNode(2), BinTreeNode(3))
-    root2 = BinTreeNode(1, BinTreeNode(2), BinTreeNode(3))
+    root1 = BinTreeNode(data=1, left=BinTreeNode(data=2), right=BinTreeNode(data=3))
+    root2 = BinTreeNode(data=1, left=BinTreeNode(data=2), right=BinTreeNode(data=3))
 
     assert root1.weak_equal(root2)
     assert root1.left.weak_equal(root2.left)
     assert root1.right.weak_equal(root2.right)
 
 
 def test_bin_tree_node_strong_eq():
-    root1 = BinTreeNode(1, BinTreeNode(2), BinTreeNode(3))
-    root2 = BinTreeNode(1, BinTreeNode(2), BinTreeNode(3))
+    root1 = BinTreeNode(data=1, left=BinTreeNode(data=2), right=BinTreeNode(data=3))
+    root2 = BinTreeNode(data=1, left=BinTreeNode(data=2), right=BinTreeNode(data=3))
 
     assert root1 == root2
     assert root1.left == root2.left
     assert root1.right == root2.right
```

### Comparing `algogears-1.1.0/tests/entities/test_threaded_bin_tree.py` & `algogears-1.1.1/tests/entities/test_threaded_bin_tree.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from copy import deepcopy
 from algogears.core import ThreadedBinTreeNode, ThreadedBinTree
 
 
 def test_threaded_bin_trees_eq():
-    f = root = ThreadedBinTreeNode("F")
-    b = root.left = ThreadedBinTreeNode("B")
-    a = root.left.left = ThreadedBinTreeNode("A")
-    d = root.left.right = ThreadedBinTreeNode("D")
-    c = root.left.right.left = ThreadedBinTreeNode("C")
-    e = root.left.right.right = ThreadedBinTreeNode("E")
-    g = root.right = ThreadedBinTreeNode("G")
-    i = root.right.right = ThreadedBinTreeNode("I")
-    h = root.right.right.left = ThreadedBinTreeNode("H")
+    f = root = ThreadedBinTreeNode(data="F")
+    b = root.left = ThreadedBinTreeNode(data="B")
+    a = root.left.left = ThreadedBinTreeNode(data="A")
+    d = root.left.right = ThreadedBinTreeNode(data="D")
+    c = root.left.right.left = ThreadedBinTreeNode(data="C")
+    e = root.left.right.right = ThreadedBinTreeNode(data="E")
+    g = root.right = ThreadedBinTreeNode(data="G")
+    i = root.right.right = ThreadedBinTreeNode(data="I")
+    h = root.right.right.left = ThreadedBinTreeNode(data="H")
 
     root2 = deepcopy(root)
-    tree = ThreadedBinTree(root2)
+    tree = ThreadedBinTree(root=root2)
 
     a.prev, a.next = i, b
     b.prev, b.next = a, c
     c.prev, c.next = b, d
     d.prev, d.next = c, e
     e.prev, e.next = d, f
     f.prev, f.next = e, g
@@ -27,34 +27,34 @@
     i.prev, i.next = h, a
 
     assert root == tree.root
 
 
 def test_threaded_bin_tree_from_iterable():
     lst = ["A", "B", "C", "D", "E"]
-    c = root = ThreadedBinTreeNode("C")
-    a = root.left = ThreadedBinTreeNode("A")
-    b = root.left.right = ThreadedBinTreeNode("B")
-    d = root.right = ThreadedBinTreeNode("D")
-    e = root.right.right = ThreadedBinTreeNode("E")
+    c = root = ThreadedBinTreeNode(data="C")
+    a = root.left = ThreadedBinTreeNode(data="A")
+    b = root.left.right = ThreadedBinTreeNode(data="B")
+    d = root.right = ThreadedBinTreeNode(data="D")
+    e = root.right.right = ThreadedBinTreeNode(data="E")
 
     a.prev, a.next = e, b
     b.prev, b.next = a, c
     c.prev, c.next = b, d
     d.prev, d.next = c, e
     e.prev, e.next = d, a
 
-    tree = ThreadedBinTree(root)
+    tree = ThreadedBinTree(root=root)
     assert tree == ThreadedBinTree.from_iterable(lst)
 
 
 def test_threaded_bin_tree_non_circular():
-    b = root = ThreadedBinTreeNode("B")
-    a = root.left = ThreadedBinTreeNode("A")
-    c = root.right = ThreadedBinTreeNode("C")
+    b = root = ThreadedBinTreeNode(data="B")
+    a = root.left = ThreadedBinTreeNode(data="A")
+    c = root.right = ThreadedBinTreeNode(data="C")
 
     a.next = b
     b.prev, b.next = a, c
     c.prev = b
     
-    tree = ThreadedBinTree(root)
+    tree = ThreadedBinTree(root=root)
     assert tree == ThreadedBinTree.from_iterable(["A", "B", "C"], circular=False)
```

