# Comparing `tmp/AlgoGrade-1.0.9.tar.gz` & `tmp/AlgoGrade-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgoGrade-1.0.9.tar", last modified: Thu Apr  4 20:05:33 2024, max compression
+gzip compressed data, was "algograde-1.1.0.tar", last modified: Sun May 26 15:27:41 2024, max compression
```

## Comparing `AlgoGrade-1.0.9.tar` & `AlgoGrade-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.839846 AlgoGrade-1.0.9/
-drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.545574 AlgoGrade-1.0.9/AlgoGrade/
--rw-rw-rw-   0        0        0        0 2023-06-26 14:08:55.000000 AlgoGrade-1.0.9/AlgoGrade/__init__.py
--rw-rw-rw-   0        0        0    11276 2024-04-04 19:51:21.000000 AlgoGrade-1.0.9/AlgoGrade/adapters.py
--rw-rw-rw-   0        0        0     8524 2024-01-22 20:26:01.000000 AlgoGrade-1.0.9/AlgoGrade/core.py
--rw-rw-rw-   0        0        0     6613 2024-04-04 18:51:54.000000 AlgoGrade-1.0.9/AlgoGrade/dynamic_hull.py
--rw-rw-rw-   0        0        0     5905 2024-03-20 13:04:49.000000 AlgoGrade-1.0.9/AlgoGrade/graham.py
--rw-rw-rw-   0        0        0      483 2024-01-16 17:07:12.000000 AlgoGrade-1.0.9/AlgoGrade/parsers.py
--rw-rw-rw-   0        0        0     2858 2024-04-04 19:35:58.000000 AlgoGrade-1.0.9/AlgoGrade/preparata.py
--rw-rw-rw-   0        0        0     2938 2024-04-04 19:54:30.000000 AlgoGrade-1.0.9/AlgoGrade/quickhull.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.832754 AlgoGrade-1.0.9/AlgoGrade.egg-info/
--rw-rw-rw-   0        0        0     1049 2024-04-04 20:05:33.000000 AlgoGrade-1.0.9/AlgoGrade.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1085 2024-04-04 20:05:33.000000 AlgoGrade-1.0.9/AlgoGrade.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 20:05:33.000000 AlgoGrade-1.0.9/AlgoGrade.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      247 2024-04-04 20:05:33.000000 AlgoGrade-1.0.9/AlgoGrade.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-04 20:05:33.000000 AlgoGrade-1.0.9/AlgoGrade.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1104 2023-06-22 12:18:56.000000 AlgoGrade-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     1049 2024-04-04 20:05:33.835791 AlgoGrade-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       59 2024-04-04 20:03:37.000000 AlgoGrade-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 20:05:33.839867 AlgoGrade-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      928 2024-04-04 20:01:58.000000 AlgoGrade-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.737756 AlgoGrade-1.0.9/tests/
--rw-rw-rw-   0        0        0        0 2023-06-26 14:09:13.000000 AlgoGrade-1.0.9/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.760195 AlgoGrade-1.0.9/tests/adapters/
--rw-rw-rw-   0        0        0        0 2024-01-22 18:31:53.000000 AlgoGrade-1.0.9/tests/adapters/__init__.py
--rw-rw-rw-   0        0        0     5834 2024-04-04 20:04:19.000000 AlgoGrade-1.0.9/tests/adapters/test_basic_adapters.py
--rw-rw-rw-   0        0        0     3852 2024-04-04 19:00:06.000000 AlgoGrade-1.0.9/tests/adapters/test_dynamic_hull.py
--rw-rw-rw-   0        0        0     2044 2024-04-04 19:06:11.000000 AlgoGrade-1.0.9/tests/adapters/test_graham.py
--rw-rw-rw-   0        0        0     2324 2024-01-11 17:35:02.000000 AlgoGrade-1.0.9/tests/adapters/test_interlibrary_converters.py
--rw-rw-rw-   0        0        0     1949 2024-04-04 19:34:56.000000 AlgoGrade-1.0.9/tests/adapters/test_preparata.py
--rw-rw-rw-   0        0        0     1894 2024-04-04 19:55:52.000000 AlgoGrade-1.0.9/tests/adapters/test_quickhull.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.779865 AlgoGrade-1.0.9/tests/answers/
--rw-rw-rw-   0        0        0        0 2024-01-22 18:32:01.000000 AlgoGrade-1.0.9/tests/answers/__init__.py
--rw-rw-rw-   0        0        0     1174 2024-01-22 20:42:24.000000 AlgoGrade-1.0.9/tests/answers/test_dynamic_hull.py
--rw-rw-rw-   0        0        0     1228 2024-03-20 13:07:18.000000 AlgoGrade-1.0.9/tests/answers/test_graham.py
--rw-rw-rw-   0        0        0     1014 2024-04-04 19:37:16.000000 AlgoGrade-1.0.9/tests/answers/test_preparata.py
--rw-rw-rw-   0        0        0      935 2024-04-04 20:01:03.000000 AlgoGrade-1.0.9/tests/answers/test_quickhull.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.811093 AlgoGrade-1.0.9/tests/graders/
--rw-rw-rw-   0        0        0        0 2024-01-22 18:32:08.000000 AlgoGrade-1.0.9/tests/graders/__init__.py
--rw-rw-rw-   0        0        0    19233 2024-01-23 07:10:12.000000 AlgoGrade-1.0.9/tests/graders/test_dynamic_hull.py
--rw-rw-rw-   0        0        0    11795 2024-03-20 12:49:53.000000 AlgoGrade-1.0.9/tests/graders/test_graham.py
--rw-rw-rw-   0        0        0     3218 2024-01-22 18:18:09.000000 AlgoGrade-1.0.9/tests/graders/test_mock.py
--rw-rw-rw-   0        0        0    14182 2024-04-04 19:51:37.000000 AlgoGrade-1.0.9/tests/graders/test_preparata.py
--rw-rw-rw-   0        0        0     8640 2024-01-22 20:34:35.000000 AlgoGrade-1.0.9/tests/graders/test_quickhull.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.824595 AlgoGrade-1.0.9/tests/parsers/
--rw-rw-rw-   0        0        0        0 2024-01-22 18:32:30.000000 AlgoGrade-1.0.9/tests/parsers/__init__.py
--rw-rw-rw-   0        0        0      387 2024-01-16 17:08:13.000000 AlgoGrade-1.0.9/tests/parsers/test_point_list_and_target_point_parser.py
--rw-rw-rw-   0        0        0      292 2024-01-16 17:08:41.000000 AlgoGrade-1.0.9/tests/parsers/test_point_list_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:27:41.476183 algograde-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-26 15:27:41.391740 algograde-1.1.0/AlgoGrade/
+-rw-rw-rw-   0        0        0        0 2023-06-26 14:08:55.000000 algograde-1.1.0/AlgoGrade/__init__.py
+-rw-rw-rw-   0        0        0    15456 2024-05-26 15:21:06.000000 algograde-1.1.0/AlgoGrade/core.py
+-rw-rw-rw-   0        0        0     3766 2024-05-26 15:21:03.000000 algograde-1.1.0/AlgoGrade/dynamic_hull.py
+-rw-rw-rw-   0        0        0     4733 2024-05-26 15:21:03.000000 algograde-1.1.0/AlgoGrade/graham.py
+-rw-rw-rw-   0        0        0      471 2024-05-26 15:21:03.000000 algograde-1.1.0/AlgoGrade/parsers.py
+-rw-rw-rw-   0        0        0     2493 2024-05-26 15:21:03.000000 algograde-1.1.0/AlgoGrade/preparata.py
+-rw-rw-rw-   0        0        0     1876 2024-05-26 15:21:03.000000 algograde-1.1.0/AlgoGrade/quickhull.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:27:41.473183 algograde-1.1.0/AlgoGrade.egg-info/
+-rw-rw-rw-   0        0        0     1081 2024-05-26 15:27:41.000000 algograde-1.1.0/AlgoGrade.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      855 2024-05-26 15:27:41.000000 algograde-1.1.0/AlgoGrade.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 15:27:41.000000 algograde-1.1.0/AlgoGrade.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      248 2024-05-26 15:27:41.000000 algograde-1.1.0/AlgoGrade.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-26 15:27:41.000000 algograde-1.1.0/AlgoGrade.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1104 2023-06-22 12:18:56.000000 algograde-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1081 2024-05-26 15:27:41.475181 algograde-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2024-04-04 20:03:37.000000 algograde-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 15:27:41.476183 algograde-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      943 2024-05-26 15:26:04.000000 algograde-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:27:41.445115 algograde-1.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-26 14:09:13.000000 algograde-1.1.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:27:41.456962 algograde-1.1.0/tests/answers/
+-rw-rw-rw-   0        0        0        0 2024-01-22 18:32:01.000000 algograde-1.1.0/tests/answers/__init__.py
+-rw-rw-rw-   0        0        0     1045 2024-05-26 15:21:03.000000 algograde-1.1.0/tests/answers/test_dynamic_hull.py
+-rw-rw-rw-   0        0        0     1141 2024-05-26 15:21:03.000000 algograde-1.1.0/tests/answers/test_graham.py
+-rw-rw-rw-   0        0        0     1205 2024-05-26 15:21:03.000000 algograde-1.1.0/tests/answers/test_preparata.py
+-rw-rw-rw-   0        0        0      854 2024-05-26 15:21:03.000000 algograde-1.1.0/tests/answers/test_quickhull.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:27:41.466710 algograde-1.1.0/tests/graders/
+-rw-rw-rw-   0        0        0        0 2024-01-22 18:32:08.000000 algograde-1.1.0/tests/graders/__init__.py
+-rw-rw-rw-   0        0        0    16410 2024-05-26 15:21:03.000000 algograde-1.1.0/tests/graders/test_dynamic_hull.py
+-rw-rw-rw-   0        0        0    28972 2024-05-26 15:21:03.000000 algograde-1.1.0/tests/graders/test_grade_methods.py
+-rw-rw-rw-   0        0        0    12007 2024-05-26 15:21:03.000000 algograde-1.1.0/tests/graders/test_graham.py
+-rw-rw-rw-   0        0        0     2537 2024-05-26 15:21:03.000000 algograde-1.1.0/tests/graders/test_mock.py
+-rw-rw-rw-   0        0        0    31486 2024-05-26 15:21:03.000000 algograde-1.1.0/tests/graders/test_preparata.py
+-rw-rw-rw-   0        0        0     7368 2024-05-26 15:21:03.000000 algograde-1.1.0/tests/graders/test_quickhull.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:27:41.472182 algograde-1.1.0/tests/parsers/
+-rw-rw-rw-   0        0        0        0 2024-01-22 18:32:30.000000 algograde-1.1.0/tests/parsers/__init__.py
+-rw-rw-rw-   0        0        0      388 2024-05-26 15:21:03.000000 algograde-1.1.0/tests/parsers/test_point_list_and_target_point_parser.py
+-rw-rw-rw-   0        0        0      289 2024-05-26 15:21:03.000000 algograde-1.1.0/tests/parsers/test_point_list_parser.py
```

### Comparing `AlgoGrade-1.0.9/AlgoGrade/graham.py` & `algograde-1.1.0/AlgoGrade/graham.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,44 @@
-from typing import ClassVar
-from PyCompGeomAlgorithms.graham import graham, GrahamStepsTableRow, GrahamStepsTable
-from .adapters import pycga_to_pydantic, pydantic_to_pycga, PydanticAdapter, PointPydanticAdapter
+from algogears.core import Point
+from algogears.graham import graham, GrahamStepsTableRow, GrahamStepsTable
 from .core import Task, Grader, Mistake, Answers
 from .parsers import PointListGivenJSONParser
 
 
 class GrahamGrader(Grader):
     @classmethod
     def grade_methods(cls):
         return [
-            cls.grade_default,
+            cls.grade_object,
             cls.grade_iterable,
-            cls.grade_default,
+            cls.grade_object,
             cls.grade_iterable,
             cls.grade_iterable,
             cls.grade_angles_less_than_pi,
             cls.grade_angles_greater_than_or_equal_to_pi,
             cls.grade_finalization
         ]
     
     @classmethod
     def grade_angles_less_than_pi(cls, answer, correct_answer, scorings):
         return [
             Mistake(scorings)
-            for row, next_row in zip(answer, answer[1:])
+            for row, next_row in zip(answer.rows, answer.rows[1:])
             if row.is_angle_less_than_pi and (
                 row.point_triple[1] != next_row.point_triple[0] or
                 row.point_triple[2] != next_row.point_triple[1] or
                 next_row.point_triple[2] != cls._next_point(answer.ordered_points, row.point_triple[2])
             )
         ]
     
     @classmethod
     def grade_angles_greater_than_or_equal_to_pi(cls, answer, correct_answer, scorings):
         return [
             Mistake(scorings)
-            for row, next_row in zip(answer, answer[1:])
+            for row, next_row in zip(answer.rows, answer.rows[1:])
             if not row.is_angle_less_than_pi and (
                 (
                     row.point_triple[0] != next_row.point_triple[0] or
                     row.point_triple[2] != next_row.point_triple[1] or
                     next_row.point_triple[2] != cls._next_point(answer.ordered_points, next_row.point_triple[1])
                 ) if row.point_triple[0] == answer.ordered_points[0] else
                 (
@@ -50,15 +49,15 @@
             )
         ]
 
     @classmethod
     def grade_finalization(cls, answer, correct_answer, scorings):
         return [
             Mistake(scorings)
-            for row in answer
+            for row in answer.rows
             if row.point_triple[1] == answer.ordered_points[0]
         ]
     
     @staticmethod
     def _prev_point(rows, row):
         i = rows.index(row)
 
@@ -71,48 +70,20 @@
     def _next_point(ordered_points, point):
         try:
             return ordered_points[(ordered_points.index(point)+1) % len(ordered_points)]
         except (IndexError, ValueError):
             return None
 
 
-class GrahamStepsTableRowPydanticAdapter(PydanticAdapter):
-    regular_class: ClassVar[type] = GrahamStepsTableRow
-    point_triple: tuple[PointPydanticAdapter, PointPydanticAdapter, PointPydanticAdapter]
-    is_angle_less_than_pi: bool
-
-    @classmethod
-    def from_regular_object(cls, obj: GrahamStepsTableRow, **kwargs):
-        return cls(
-            point_triple=pycga_to_pydantic(obj.point_triple),
-            is_angle_less_than_pi=obj.is_angle_less_than_pi,
-            **kwargs
-        )
-
-
-class GrahamStepsTablePydanticAdapter(PydanticAdapter):
-    regular_class: ClassVar[type] = GrahamStepsTable
-    ordered_points: list[PointPydanticAdapter]
-    rows: list[GrahamStepsTableRowPydanticAdapter]
-
-    @classmethod
-    def from_regular_object(cls, obj: GrahamStepsTable, **kwargs):
-        return cls(
-            ordered_points=pycga_to_pydantic(obj.ordered_points),
-            rows=pycga_to_pydantic(obj.rows),
-            **kwargs
-        )
-
-
 class GrahamAnswers(Answers):
-    centroid: PointPydanticAdapter
-    ordered_points: list[PointPydanticAdapter]
-    origin: PointPydanticAdapter
-    steps_table: GrahamStepsTablePydanticAdapter
-    point_triples_: list[tuple[PointPydanticAdapter, PointPydanticAdapter, PointPydanticAdapter]] | None = None
+    centroid: Point
+    ordered_points: list[Point]
+    origin: Point
+    steps_table: GrahamStepsTable
+    point_triples_: list[tuple[Point, Point, Point]] | None = None
     are_angles_less_than_pi_: list[bool] | None = None
 
     @classmethod
     def from_iterable(cls, iterable):
         centroid, ordered_points, origin, point_triples, are_angles_less_than_pi, steps_table, *rest = iterable        
         return cls(centroid=centroid, ordered_points=ordered_points, origin=origin, steps_table=steps_table, point_triples_=point_triples, are_angles_less_than_pi_=are_angles_less_than_pi)
 
@@ -120,15 +91,15 @@
     def point_triples(self):
         return self.point_triples_ or [row.point_triple for row in self.steps_table.rows]
 
     @property
     def are_angles_less_than_pi(self):
         return self.are_angles_less_than_pi_ or [row.is_angle_less_than_pi for row in self.steps_table.rows]
 
-    def to_pydantic_list(self):
+    def to_algogears_list(self):
         return [
             self.centroid, self.ordered_points, self.origin, self.point_triples,
             self.are_angles_less_than_pi, self.steps_table, self.steps_table, self.steps_table
         ]
     
     def __eq__(self, other):
         if isinstance(other, self.__class__):
```

### Comparing `AlgoGrade-1.0.9/AlgoGrade.egg-info/PKG-INFO` & `algograde-1.1.0/AlgoGrade.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: AlgoGrade
-Version: 1.0.9
-Summary: A library for automated grading of algorithmic tasks with grading of their intermediate stages. The grading of some computational geometry tasks are provided out of the box.
+Version: 1.1.0
+Summary: A library for automated grading of algorithm-based assignments with grading of their intermediate stages. The grading of some computational geometry assignments is provided out of the box.
 Author: artandfi (Artem Fisunenko)
 Author-email: artyom.fisunenko@gmail.com
 Keywords: Python3,automated grading,computational geometry,convex hull,region search,geometric search,point location,proximity,closest pair,closest points
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
+Requires-Dist: algogears==1.1.2
 Requires-Dist: annotated-types==0.5.0
+Requires-Dist: build==1.2.1
 Requires-Dist: colorama==0.4.6
 Requires-Dist: exceptiongroup==1.1.1
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: packaging==23.1
 Requires-Dist: pluggy==1.2.0
-Requires-Dist: PyCompGeomAlgorithms==1.0.20
 Requires-Dist: pydantic==2.0
 Requires-Dist: pydantic_core==2.0.1
 Requires-Dist: pyproject_hooks==1.0.0
 Requires-Dist: pytest==7.4.0
 Requires-Dist: tomli==2.0.1
 Requires-Dist: typing_extensions==4.8.0
```

### Comparing `AlgoGrade-1.0.9/AlgoGrade.egg-info/SOURCES.txt` & `algograde-1.1.0/AlgoGrade.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 LICENSE
 README.md
 setup.py
 AlgoGrade/__init__.py
-AlgoGrade/adapters.py
 AlgoGrade/core.py
 AlgoGrade/dynamic_hull.py
 AlgoGrade/graham.py
 AlgoGrade/parsers.py
 AlgoGrade/preparata.py
 AlgoGrade/quickhull.py
 AlgoGrade.egg-info/PKG-INFO
 AlgoGrade.egg-info/SOURCES.txt
 AlgoGrade.egg-info/dependency_links.txt
 AlgoGrade.egg-info/requires.txt
 AlgoGrade.egg-info/top_level.txt
 tests/__init__.py
-tests/adapters/__init__.py
-tests/adapters/test_basic_adapters.py
-tests/adapters/test_dynamic_hull.py
-tests/adapters/test_graham.py
-tests/adapters/test_interlibrary_converters.py
-tests/adapters/test_preparata.py
-tests/adapters/test_quickhull.py
 tests/answers/__init__.py
 tests/answers/test_dynamic_hull.py
 tests/answers/test_graham.py
 tests/answers/test_preparata.py
 tests/answers/test_quickhull.py
 tests/graders/__init__.py
 tests/graders/test_dynamic_hull.py
+tests/graders/test_grade_methods.py
 tests/graders/test_graham.py
 tests/graders/test_mock.py
 tests/graders/test_preparata.py
 tests/graders/test_quickhull.py
 tests/parsers/__init__.py
 tests/parsers/test_point_list_and_target_point_parser.py
 tests/parsers/test_point_list_parser.py
```

### Comparing `AlgoGrade-1.0.9/LICENSE` & `algograde-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AlgoGrade-1.0.9/PKG-INFO` & `algograde-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: AlgoGrade
-Version: 1.0.9
-Summary: A library for automated grading of algorithmic tasks with grading of their intermediate stages. The grading of some computational geometry tasks are provided out of the box.
+Version: 1.1.0
+Summary: A library for automated grading of algorithm-based assignments with grading of their intermediate stages. The grading of some computational geometry assignments is provided out of the box.
 Author: artandfi (Artem Fisunenko)
 Author-email: artyom.fisunenko@gmail.com
 Keywords: Python3,automated grading,computational geometry,convex hull,region search,geometric search,point location,proximity,closest pair,closest points
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
+Requires-Dist: algogears==1.1.2
 Requires-Dist: annotated-types==0.5.0
+Requires-Dist: build==1.2.1
 Requires-Dist: colorama==0.4.6
 Requires-Dist: exceptiongroup==1.1.1
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: packaging==23.1
 Requires-Dist: pluggy==1.2.0
-Requires-Dist: PyCompGeomAlgorithms==1.0.20
 Requires-Dist: pydantic==2.0
 Requires-Dist: pydantic_core==2.0.1
 Requires-Dist: pyproject_hooks==1.0.0
 Requires-Dist: pytest==7.4.0
 Requires-Dist: tomli==2.0.1
 Requires-Dist: typing_extensions==4.8.0
```

### Comparing `AlgoGrade-1.0.9/setup.py` & `algograde-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="AlgoGrade",
-    version="1.0.9",
+    version="1.1.0",
     author="artandfi (Artem Fisunenko)",
     author_email="artyom.fisunenko@gmail.com",
-    description="A library for automated grading of algorithmic tasks with grading of their intermediate stages. "
-    "The grading of some computational geometry tasks are provided out of the box.",
+    description="A library for automated grading of algorithm-based assignments with grading of their intermediate stages. "
+    "The grading of some computational geometry assignments is provided out of the box.",
     packages=find_packages(),
     install_requires=[line.strip() for line in open("requirements.txt", "r").readlines()],
     keywords=[
         "Python3",
         "automated grading",
         "computational geometry",
         "convex hull",
```

### Comparing `AlgoGrade-1.0.9/tests/answers/test_dynamic_hull.py` & `algograde-1.1.0/tests/answers/test_dynamic_hull.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from PyCompGeomAlgorithms.dynamic_hull import PathDirection
-from AlgoGrade.adapters import PointPydanticAdapter, pydantic_to_pycga
-from AlgoGrade.dynamic_hull import DynamicHullAnswers, DynamicHullNodePydanticAdapter, DynamicHullTreePydanticAdapter
+from algogears.core import Point
+from algogears.dynamic_hull import PathDirection, DynamicHullNode, DynamicHullTree
+from AlgoGrade.dynamic_hull import DynamicHullAnswers
 
 
 def test_dynamic_hull_answers():
-    point = PointPydanticAdapter(coords=(1, 1))
+    point = Point(coords=(1, 1))
     hull = [point]
-    root = DynamicHullNodePydanticAdapter(
+    root = DynamicHullNode(
         data=point,
-        subhull_points=hull,
+        subhull=hull,
         left_supporting=point,
         right_supporting=point
     )
     leaves = [root]
-    tree = DynamicHullTreePydanticAdapter(root=root)
+    tree = DynamicHullTree(root=root)
     optimized_tree = tree
     path = [PathDirection.right]
     modified_tree = tree
 
     answers_model = DynamicHullAnswers(
         leaves=leaves, tree=tree, optimized_tree=optimized_tree,
         path=path, modified_tree=modified_tree, hull=hull
     )
     answers_list = [leaves, tree, tree, tree, tree, optimized_tree, path, (modified_tree, hull)]
 
-    assert answers_model.to_pydantic_list() == answers_list
-    assert answers_model.to_pycga_list() == pydantic_to_pycga(answers_list)
-    assert DynamicHullAnswers.from_iterable(answers_list) == answers_model
+    assert answers_model.to_algogears_list() == answers_list
+    assert DynamicHullAnswers.from_iterable(answers_list) == answers_model
+    assert DynamicHullAnswers(**answers_model.model_dump()) == answers_model
```

### Comparing `AlgoGrade-1.0.9/tests/answers/test_quickhull.py` & `algograde-1.1.0/tests/answers/test_quickhull.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from AlgoGrade.adapters import PointPydanticAdapter, pydantic_to_pycga
-from AlgoGrade.quickhull import QuickhullAnswers, QuickhullNodePydanticAdapter, QuickhullTreePydanticAdapter
+from algogears.core import Point
+from algogears.quickhull import QuickhullNode, QuickhullTree
+from AlgoGrade.quickhull import QuickhullAnswers
 
 
 def test_quickhull_answers():
-    point = PointPydanticAdapter(coords=(1, 1))
+    point = Point(coords=(1, 1))
     leftmost_point, rightmost_point = point, point
     subset1, subset2 = [point], [point]
-    tree = QuickhullTreePydanticAdapter(root=QuickhullNodePydanticAdapter(data=[point]))
+    tree = QuickhullTree(root=QuickhullNode(data=[point]))
 
     answers_model = QuickhullAnswers(
         leftmost_point=leftmost_point, rightmost_point=rightmost_point,
         subset1=subset1, subset2=subset2, tree=tree
     )
     answers_list = [(leftmost_point, rightmost_point, subset1, subset2), tree, tree, tree, tree]
 
-    assert answers_model.to_pydantic_list() == answers_list
-    assert answers_model.to_pycga_list() == pydantic_to_pycga(answers_list)
+    assert answers_model.to_algogears_list() == answers_list
     assert QuickhullAnswers.from_iterable(answers_list) == answers_model
+    assert QuickhullAnswers(**answers_model.model_dump()) == answers_model
```

### Comparing `AlgoGrade-1.0.9/tests/graders/test_graham.py` & `algograde-1.1.0/tests/graders/test_graham.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,283 +1,259 @@
 from copy import deepcopy
 from math import isclose
-from PyCompGeomAlgorithms.core import Point
-from PyCompGeomAlgorithms.graham import GrahamStepsTable, GrahamStepsTableRow
+from algogears.core import Point
+from algogears.graham import GrahamStepsTable, GrahamStepsTableRow
 from AlgoGrade.graham import GrahamGrader, GrahamTask, GrahamAnswers
-from AlgoGrade.adapters import pycga_to_pydantic
 from AlgoGrade.core import Scoring
 
 
 points = [
-    Point(2, 8),
-    Point(5, 6),
-    Point(7, 8),
-    Point(8, 11),
-    Point(7, 5),
-    Point(10, 7),
-    Point(11, 5),
-    Point(8, 2),
-    Point(1, 3),
-    Point(5, 2),
+    Point.new(2, 8),
+    Point.new(5, 6),
+    Point.new(7, 8),
+    Point.new(8, 11),
+    Point.new(7, 5),
+    Point.new(10, 7),
+    Point.new(11, 5),
+    Point.new(8, 2),
+    Point.new(1, 3),
+    Point.new(5, 2),
 ]
 givens = (points,)
 task_class = GrahamTask
 scorings = [
     Scoring(max_grade=0.25, fine=0.25),
     Scoring(max_grade=0.25, fine=0.25),
     Scoring(max_grade=0.25, fine=0.25),
     Scoring(max_grade=0.15, fine=0.15),
     Scoring(max_grade=0.15, fine=0.15),
     Scoring(max_grade=0.25, fine=0.25),
     Scoring(max_grade=0.6, fine=0.3, repeat_fine=0.6),
     Scoring(max_grade=0.1, fine=0.25)
 ]
-correct_pycga_answers = task_class.solve_as_pycga_list(givens)
-correct_pydantic_answers = task_class.solve_as_pydantic_list(givens)
+correct_algogears_answers = task_class.solve_as_algogears_list(givens)
 correct_answers_wrapper = task_class.solve_as_answers_wrapper(givens)
 
 
 def test_graham_grader_all_correct():
-    centroid = Point(4.6667, 7.3333)
+    centroid = Point.new(4.6667, 7.3333)
     ordered = [
-        Point(8, 2),
-        Point(7, 5),
-        Point(11, 5),
-        Point(10, 7),
-        Point(7, 8),
-        Point(8, 11),
-        Point(2, 8),
-        Point(1, 3),
-        Point(5, 2),
-        Point(5, 6)
+        Point.new(8, 2),
+        Point.new(7, 5),
+        Point.new(11, 5),
+        Point.new(10, 7),
+        Point.new(7, 8),
+        Point.new(8, 11),
+        Point.new(2, 8),
+        Point.new(1, 3),
+        Point.new(5, 2),
+        Point.new(5, 6)
     ]
-    origin = Point(8, 2)
-    steps_table = GrahamStepsTable(ordered)
+    origin = Point.new(8, 2)
+    steps_table = GrahamStepsTable(ordered_points=ordered)
     steps_table.extend([
-        GrahamStepsTableRow((ordered[0], ordered[1], ordered[2]), False),
-        GrahamStepsTableRow((ordered[0], ordered[2], ordered[3]), True),
-        GrahamStepsTableRow((ordered[2], ordered[3], ordered[4]), True),
-        GrahamStepsTableRow((ordered[3], ordered[4], ordered[5]), False),
-        GrahamStepsTableRow((ordered[2], ordered[3], ordered[5]), False),
-        GrahamStepsTableRow((ordered[0], ordered[2], ordered[5]), True),
-        GrahamStepsTableRow((ordered[2], ordered[5], ordered[6]), True),
-        GrahamStepsTableRow((ordered[5], ordered[6], ordered[7]), True),
-        GrahamStepsTableRow((ordered[6], ordered[7], ordered[8]), True),
-        GrahamStepsTableRow((ordered[7], ordered[8], ordered[9]), True),
-        GrahamStepsTableRow((ordered[8], ordered[9], ordered[0]), False),
-        GrahamStepsTableRow((ordered[7], ordered[8], ordered[0]), True)
+        GrahamStepsTableRow(point_triple=(ordered[0], ordered[1], ordered[2]), is_angle_less_than_pi=False),
+        GrahamStepsTableRow(point_triple=(ordered[0], ordered[2], ordered[3]), is_angle_less_than_pi=True),
+        GrahamStepsTableRow(point_triple=(ordered[2], ordered[3], ordered[4]), is_angle_less_than_pi=True),
+        GrahamStepsTableRow(point_triple=(ordered[3], ordered[4], ordered[5]), is_angle_less_than_pi=False),
+        GrahamStepsTableRow(point_triple=(ordered[2], ordered[3], ordered[5]), is_angle_less_than_pi=False),
+        GrahamStepsTableRow(point_triple=(ordered[0], ordered[2], ordered[5]), is_angle_less_than_pi=True),
+        GrahamStepsTableRow(point_triple=(ordered[2], ordered[5], ordered[6]), is_angle_less_than_pi=True),
+        GrahamStepsTableRow(point_triple=(ordered[5], ordered[6], ordered[7]), is_angle_less_than_pi=True),
+        GrahamStepsTableRow(point_triple=(ordered[6], ordered[7], ordered[8]), is_angle_less_than_pi=True),
+        GrahamStepsTableRow(point_triple=(ordered[7], ordered[8], ordered[9]), is_angle_less_than_pi=True),
+        GrahamStepsTableRow(point_triple=(ordered[8], ordered[9], ordered[0]), is_angle_less_than_pi=False),
+        GrahamStepsTableRow(point_triple=(ordered[7], ordered[8], ordered[0]), is_angle_less_than_pi=True)
     ])
-    triples = [row.point_triple for row in steps_table]
-    are_angles_less_than_pi = [row.is_angle_less_than_pi for row in steps_table]
+    triples = [row.point_triple for row in steps_table.rows]
+    are_angles_less_than_pi = [row.is_angle_less_than_pi for row in steps_table.rows]
 
-    pycga_answers = [
+    algogears_answers = [
         centroid,
         ordered,
         origin,
         triples,
         are_angles_less_than_pi,
         steps_table,
         steps_table,
         steps_table
     ]
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = GrahamAnswers.from_iterable(pydantic_answers)
+    answers_wrapper = GrahamAnswers.from_iterable(algogears_answers)
 
-    total_grade, answer_grades = GrahamGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
-    assert isclose(total_grade, 2)
-
-    total_grade, answer_grades = GrahamGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 2)
 
     total_grade, answer_grades = GrahamGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 2)
 
 
 def test_graham_grader_incorrect_centroid():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    pycga_answers[0] = Point(100, 100)
-
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = GrahamAnswers.from_iterable(pydantic_answers)
+    algogears_answers = deepcopy(correct_algogears_answers)
+    algogears_answers[0] = Point.new(100, 100)
+    answers_wrapper = GrahamAnswers.from_iterable(algogears_answers)
 
-    total_grade, answer_grades = GrahamGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.75)
 
-    total_grade, answer_grades = GrahamGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.75)
 
     total_grade, answer_grades = GrahamGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1.75)
 
 
 def test_graham_grader_incorrect_ordered_points():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    pycga_answers[1] = [
-        Point(2000, 2000),
-        Point(5000, 5000),
-        Point(11, 5),
-        Point(10, 7),
-        Point(7, 8),
-        Point(8, 11),
-        Point(2, 8),
-        Point(3000, 3000),
-        Point(5, 2),
-        Point(5, 6)
+    algogears_answers = deepcopy(correct_algogears_answers)
+    algogears_answers[1] = [
+        Point.new(2000, 2000),
+        Point.new(5000, 5000),
+        Point.new(11, 5),
+        Point.new(10, 7),
+        Point.new(7, 8),
+        Point.new(8, 11),
+        Point.new(2, 8),
+        Point.new(3000, 3000),
+        Point.new(5, 2),
+        Point.new(5, 6)
     ]
+    answers_wrapper = GrahamAnswers.from_iterable(algogears_answers)
 
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = GrahamAnswers.from_iterable(pydantic_answers)
-
-    total_grade, answer_grades = GrahamGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.75)
 
-    total_grade, answer_grades = GrahamGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.75)
 
     total_grade, answer_grades = GrahamGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1.75)
 
 
 def test_graham_grader_incorrect_origin():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    pycga_answers[2] = Point(100, 100)
-
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = GrahamAnswers.from_iterable(pydantic_answers)
+    algogears_answers = deepcopy(correct_algogears_answers)
+    algogears_answers[2] = Point.new(100, 100)
+    answers_wrapper = GrahamAnswers.from_iterable(algogears_answers)
 
-    total_grade, answer_grades = GrahamGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.75)
 
-    total_grade, answer_grades = GrahamGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.75)
 
     total_grade, answer_grades = GrahamGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1.75)
 
 
 def test_graham_grader_incorrect_triples():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    ordered = pycga_answers[1]
-    pycga_answers[3] = [
+    algogears_answers = deepcopy(correct_algogears_answers)
+    ordered = algogears_answers[1]
+    algogears_answers[3] = [
         (ordered[0], ordered[0], ordered[0]),
         (ordered[0], ordered[0], ordered[0]),
         (ordered[2], ordered[3], ordered[4]),
         (ordered[3], ordered[4], ordered[5]),
         (ordered[2], ordered[3], ordered[5]),
         (ordered[0], ordered[2], ordered[5]),
         (ordered[2], ordered[5], ordered[6]),
         (ordered[5], ordered[6], ordered[7]),
         (ordered[6], ordered[7], ordered[8]),
         (ordered[7], ordered[8], ordered[9]),
         (ordered[8], ordered[9], ordered[0]),
         (ordered[7], ordered[8], ordered[0])
     ]
+    answers_wrapper = GrahamAnswers.from_iterable(algogears_answers)
 
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = GrahamAnswers.from_iterable(pydantic_answers)
-
-    total_grade, answer_grades = GrahamGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.85)
 
-    total_grade, answer_grades = GrahamGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.85)
 
     total_grade, answer_grades = GrahamGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1.85)
 
 
 def test_graham_grader_incorrect_are_angles_less_than_pi():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    pycga_answers[4] = [False for _ in pycga_answers[4]]
-
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = GrahamAnswers.from_iterable(pydantic_answers)
+    algogears_answers = deepcopy(correct_algogears_answers)
+    algogears_answers[4] = [False for _ in algogears_answers[4]]
+    answers_wrapper = GrahamAnswers.from_iterable(algogears_answers)
 
-    total_grade, answer_grades = GrahamGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.85)
 
-    total_grade, answer_grades = GrahamGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.85)
 
     total_grade, answer_grades = GrahamGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1.85)
 
 
 def test_graham_grader_incorrect_rows_with_angles_less_than_pi():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    ordered = pycga_answers[1]
-    incorrect_point = Point(1000, 1000)
+    algogears_answers = deepcopy(correct_algogears_answers)
+    ordered = algogears_answers[1]
+    incorrect_point = Point.new(1000, 1000)
 
-    pycga_answers[5][7] = GrahamStepsTableRow((ordered[5], ordered[6], incorrect_point), True)
-    pycga_answers[5][8] = GrahamStepsTableRow((ordered[6], ordered[7], incorrect_point), True)
-    
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = GrahamAnswers.from_iterable(pydantic_answers)
+    algogears_answers[5][7] = GrahamStepsTableRow(point_triple=(ordered[5], ordered[6], incorrect_point), is_angle_less_than_pi=True)
+    algogears_answers[5][8] = GrahamStepsTableRow(point_triple=(ordered[6], ordered[7], incorrect_point), is_angle_less_than_pi=True)
+    answers_wrapper = GrahamAnswers.from_iterable(algogears_answers)
 
-    total_grade, answer_grades = GrahamGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.75)
 
-    total_grade, answer_grades = GrahamGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.75)
 
     total_grade, answer_grades = GrahamGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1.75)
 
 
 def test_graham_grader_incorrect_rows_with_angles_not_less_than_pi_single():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    ordered = pycga_answers[1]
-    incorrect_point = Point(1000, 1000)
-
-    pycga_answers[5][1] = GrahamStepsTableRow((ordered[0], ordered[2], incorrect_point), True)
-    
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = GrahamAnswers.from_iterable(pydantic_answers)
+    algogears_answers = deepcopy(correct_algogears_answers)
+    ordered = algogears_answers[1]
+    incorrect_point = Point.new(1000, 1000)
 
-    total_grade, answer_grades = GrahamGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
+    algogears_answers[5][1] = GrahamStepsTableRow(point_triple=(ordered[0], ordered[2], incorrect_point), is_angle_less_than_pi=True)
+    answers_wrapper = GrahamAnswers.from_iterable(algogears_answers)
+
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.45) # also triggers "rows with angles < pi" grading
 
-    total_grade, answer_grades = GrahamGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.45)
 
     total_grade, answer_grades = GrahamGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1.45)
 
 
 def test_graham_grader_incorrect_rows_with_angles_not_less_than_pi_repeated():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    incorrect_point = Point(1000, 1000)
+    algogears_answers = deepcopy(correct_algogears_answers)
+    incorrect_point = Point.new(1000, 1000)
 
-    pycga_answers[5][1] = GrahamStepsTableRow((incorrect_point, incorrect_point, incorrect_point), True)
-    pycga_answers[5][5] = GrahamStepsTableRow((incorrect_point, incorrect_point, incorrect_point), True)
-    
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = GrahamAnswers.from_iterable(pydantic_answers)
+    algogears_answers[5][1] = GrahamStepsTableRow(point_triple=(incorrect_point, incorrect_point, incorrect_point), is_angle_less_than_pi=True)
+    algogears_answers[5][5] = GrahamStepsTableRow(point_triple=(incorrect_point, incorrect_point, incorrect_point), is_angle_less_than_pi=True)
+    answers_wrapper = GrahamAnswers.from_iterable(algogears_answers)
 
-    total_grade, answer_grades = GrahamGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.15) # also triggers "rows with angles < pi" grading
 
-    total_grade, answer_grades = GrahamGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.15)
 
     total_grade, answer_grades = GrahamGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1.15)
 
 
 def test_graham_grader_incorrect_finalization():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    ordered = pycga_answers[1]
-    pycga_answers[6][7] = GrahamStepsTableRow((ordered[5], ordered[0], ordered[7]), True)
-
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = GrahamAnswers.from_iterable(pydantic_answers)
+    algogears_answers = deepcopy(correct_algogears_answers)
+    ordered = algogears_answers[1]
+    algogears_answers[6][7] = GrahamStepsTableRow(point_triple=(ordered[5], ordered[0], ordered[7]), is_angle_less_than_pi=True)
+    answers_wrapper = GrahamAnswers.from_iterable(algogears_answers)
 
-    total_grade, answer_grades = GrahamGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.5) # also triggers "rows with angles < pi" grading
 
-    total_grade, answer_grades = GrahamGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = GrahamGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.5)
 
     total_grade, answer_grades = GrahamGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1.5)
```

### Comparing `AlgoGrade-1.0.9/tests/graders/test_quickhull.py` & `algograde-1.1.0/tests/graders/test_quickhull.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 from math import isclose
 from copy import deepcopy
-from PyCompGeomAlgorithms.core import Point
-from PyCompGeomAlgorithms.quickhull import QuickhullNode, QuickhullTree
+from algogears.core import Point
+from algogears.quickhull import QuickhullNode, QuickhullTree
 from AlgoGrade.quickhull import QuickhullGrader, QuickhullTask, QuickhullAnswers
-from AlgoGrade.adapters import pycga_to_pydantic
 from AlgoGrade.core import Scoring
 
 
 points = [
-    Point(0, 6),
-    Point(8, 11),
-    Point(10, 4),
-    Point(7, 13),
-    Point(6, 3),
-    Point(3, 0),
-    Point(4, 2),
-    Point(12, 1),
-    Point(14, 10),
-    Point(5, 9),
-    Point(3, 11),
-    Point(1, 4),
+    Point.new(0, 6),
+    Point.new(8, 11),
+    Point.new(10, 4),
+    Point.new(7, 13),
+    Point.new(6, 3),
+    Point.new(3, 0),
+    Point.new(4, 2),
+    Point.new(12, 1),
+    Point.new(14, 10),
+    Point.new(5, 9),
+    Point.new(3, 11),
+    Point.new(1, 4),
 ]
 givens = (points,)
 hull = [points[0], points[10], points[3], points[8], points[7], points[5]]
 task_class = QuickhullTask
 scorings = [
     Scoring(max_grade=0.25, fine=0.25),
     Scoring(max_grade=0.25, fine=0.25, repeat_fine=0.5),
     Scoring(max_grade=0.25, fine=0.25),
     Scoring(max_grade=0.25, fine=0.25),
     Scoring(max_grade=1, fine=1)
 ]
-correct_pycga_answers = task_class.solve_as_pycga_list(givens)
-correct_pydantic_answers = task_class.solve_as_pydantic_list(givens)
+correct_algogears_answers = task_class.solve_as_algogears_list(givens)
 correct_answers_wrapper = task_class.solve_as_answers_wrapper(givens)
 
 
 def test_quickhull_grader_all_correct():
     tree = QuickhullTree(
-        QuickhullNode(
-            [
+        root=QuickhullNode(
+            data=[
                 points[0],
                 points[10],
                 points[9],
                 points[3],
                 points[1],
                 points[8],
                 points[7],
@@ -54,151 +52,117 @@
                 points[11],
             ],
             subhull=hull
         )
     )
 
     tree.root.left = QuickhullNode(
-        [points[0], points[10], points[9], points[3], points[1], points[8]],
+        data=[points[0], points[10], points[9], points[3], points[1], points[8]],
         h=points[3],
         subhull=[points[0], points[10], points[3], points[8]]
     )
     tree.root.right = QuickhullNode(
-        [points[8], points[7], points[2], points[4], points[6], points[5], points[11], points[0]],
+        data=[points[8], points[7], points[2], points[4], points[6], points[5], points[11], points[0]],
         h=points[7],
         subhull=[points[8], points[7], points[5], points[0]]
     )
 
-    tree.root.left.left = QuickhullNode([points[0], points[10], points[3]], h=points[10], subhull=[points[0], points[10], points[3]])
-    tree.root.left.right = QuickhullNode([points[3], points[8]], subhull=[points[3], points[8]])
-    tree.root.left.left.left = QuickhullNode([points[0], points[10]], subhull=[points[0], points[10]])
-    tree.root.left.left.right = QuickhullNode([points[10], points[3]], subhull=[points[10], points[3]])
+    tree.root.left.left = QuickhullNode(data=[points[0], points[10], points[3]], h=points[10], subhull=[points[0], points[10], points[3]])
+    tree.root.left.right = QuickhullNode(data=[points[3], points[8]], subhull=[points[3], points[8]])
+    tree.root.left.left.left = QuickhullNode(data=[points[0], points[10]], subhull=[points[0], points[10]])
+    tree.root.left.left.right = QuickhullNode(data=[points[10], points[3]], subhull=[points[10], points[3]])
 
-    tree.root.right.left = QuickhullNode([points[8], points[7]], subhull=[points[8], points[7]])
+    tree.root.right.left = QuickhullNode(data=[points[8], points[7]], subhull=[points[8], points[7]])
     tree.root.right.right = QuickhullNode(
-        [points[7], points[4], points[6], points[5], points[11], points[0]],
+        data=[points[7], points[4], points[6], points[5], points[11], points[0]],
         h=points[5],
         subhull=[points[7], points[5], points[0]]
     )
-    tree.root.right.right.left = QuickhullNode([points[7], points[5]], subhull=[points[7], points[5]])
-    tree.root.right.right.right = QuickhullNode([points[5], points[0]], subhull=[points[5], points[0]])
+    tree.root.right.right.left = QuickhullNode(data=[points[7], points[5]], subhull=[points[7], points[5]])
+    tree.root.right.right.right = QuickhullNode(data=[points[5], points[0]], subhull=[points[5], points[0]])
 
     leftmost_point, rightmost_point = points[0], points[8]
     s1, s2 = tree.root.left.points, tree.root.right.points
 
-    pycga_answers = [(leftmost_point, rightmost_point, s1, s2), tree, tree, tree, tree]
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = QuickhullAnswers.from_iterable(pydantic_answers)
+    algogears_answers = [(leftmost_point, rightmost_point, s1, s2), tree, tree, tree, tree]
+    answers_wrapper = QuickhullAnswers.from_iterable(algogears_answers)
 
-    total_grade, answer_grades = QuickhullGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
-    assert isclose(total_grade, 2)
-
-    total_grade, answer_grades = QuickhullGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = QuickhullGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 2)
 
     total_grade, answer_grades = QuickhullGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 2)
 
 
 def test_quickhull_grader_incorrect_first_step():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    first_step_list = list(pycga_answers[0])
-    first_step_list[0] = Point(100, 100)
-    pycga_answers[0] = tuple(first_step_list)
-
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = QuickhullAnswers.from_iterable(pydantic_answers)
+    algogears_answers = deepcopy(correct_algogears_answers)
+    first_step_list = list(algogears_answers[0])
+    first_step_list[0] = Point.new(100, 100)
+    algogears_answers[0] = tuple(first_step_list)
+    answers_wrapper = QuickhullAnswers.from_iterable(algogears_answers)
 
-    total_grade, answer_grades = QuickhullGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
-    assert isclose(total_grade, 1.75)
-
-    total_grade, answer_grades = QuickhullGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = QuickhullGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.75)
 
     total_grade, answer_grades = QuickhullGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1.75)
 
 
 def test_quickhull_grader_incorrect_h_single():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    pycga_answers[1].root.h = Point(100, 100)
-
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = QuickhullAnswers.from_iterable(pydantic_answers)
+    algogears_answers = deepcopy(correct_algogears_answers)
+    algogears_answers[1].root.h = Point.new(100, 100)
+    answers_wrapper = QuickhullAnswers.from_iterable(algogears_answers)
 
-    total_grade, answer_grades = QuickhullGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
-    assert isclose(total_grade, 1.75)
-
-    total_grade, answer_grades = QuickhullGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = QuickhullGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.75)
 
     total_grade, answer_grades = QuickhullGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1.75)
 
 
 def test_quickhull_grader_incorrect_h_repeated():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    pycga_answers[1].root.h = Point(100, 100)
-    pycga_answers[1].root.left.h = Point(100, 100)
-
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = QuickhullAnswers.from_iterable(pydantic_answers)
-
-    total_grade, answer_grades = QuickhullGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
-    assert isclose(total_grade, 1.5)
+    algogears_answers = deepcopy(correct_algogears_answers)
+    algogears_answers[1].root.h = Point.new(100, 100)
+    algogears_answers[1].root.left.h = Point.new(100, 100)
+    answers_wrapper = QuickhullAnswers.from_iterable(algogears_answers)
 
-    total_grade, answer_grades = QuickhullGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = QuickhullGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.5)
 
     total_grade, answer_grades = QuickhullGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1.5)
 
 
 def test_quickhull_grader_incorrect_points():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    pycga_answers[2].root.left.left.points[0] = Point(100, 100)
+    algogears_answers = deepcopy(correct_algogears_answers)
+    algogears_answers[2].root.left.left.points[0] = Point.new(100, 100)
+    answers_wrapper = QuickhullAnswers.from_iterable(algogears_answers)
 
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = QuickhullAnswers.from_iterable(pydantic_answers)
-
-    total_grade, answer_grades = QuickhullGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
-    assert isclose(total_grade, 1.75)
-
-    total_grade, answer_grades = QuickhullGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = QuickhullGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1.75)
 
     total_grade, answer_grades = QuickhullGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1.75)
 
 
 def test_quickhull_grader_incorrect_finalization():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    pycga_answers[3].root.left.right.left = QuickhullNode([]) # leaf node w/ 2 points is now not a leaf
+    algogears_answers = deepcopy(correct_algogears_answers)
+    algogears_answers[3].root.left.right.left = QuickhullNode(data=[]) # leaf node w/ 2 points is now not a leaf
+    answers_wrapper = QuickhullAnswers.from_iterable(algogears_answers)
 
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = QuickhullAnswers.from_iterable(pydantic_answers)
-
-    total_grade, answer_grades = QuickhullGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
-    assert isclose(total_grade, 1.75)
-
-    total_grade, answer_grades = QuickhullGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
-    assert isclose(total_grade, 1.75)
+    total_grade, answer_grades = QuickhullGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
+    assert isclose(total_grade, 0.25) # this test also triggers four node-related gradings: 0.25, 0.25, 0.25, 1
 
     total_grade, answer_grades = QuickhullGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
-    assert isclose(total_grade, 1.75)
+    assert isclose(total_grade, 0.25)
 
 
 def test_quickhull_grader_incorrect_merge():
-    pycga_answers = deepcopy(correct_pycga_answers)
-    pycga_answers[4].root.left.right.subhull = [Point(100, 100)]
-
-    pydantic_answers = pycga_to_pydantic(pycga_answers)
-    answers_wrapper = QuickhullAnswers.from_iterable(pydantic_answers)
-
-    total_grade, answer_grades = QuickhullGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
-    assert isclose(total_grade, 1)
+    algogears_answers = deepcopy(correct_algogears_answers)
+    algogears_answers[4].root.left.right.subhull = [Point.new(100, 100)]
+    answers_wrapper = QuickhullAnswers.from_iterable(algogears_answers)
 
-    total_grade, answer_grades = QuickhullGrader.grade_pydantic(pydantic_answers, correct_pydantic_answers, scorings)
+    total_grade, answer_grades = QuickhullGrader.grade_algogears(algogears_answers, correct_algogears_answers, scorings)
     assert isclose(total_grade, 1)
 
     total_grade, answer_grades = QuickhullGrader.grade_answers_wrapper(answers_wrapper, correct_answers_wrapper, scorings)
     assert isclose(total_grade, 1)
```

