# Comparing `tmp/VisualShape3D-1.1.2.tar.gz` & `tmp/VisualShape3D-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisualShape3D-1.1.2.tar", last modified: Sat Mar 16 07:35:39 2024, max compression
+gzip compressed data, was "VisualShape3D-1.1.3.tar", last modified: Sun May 26 14:31:32 2024, max compression
```

## Comparing `VisualShape3D-1.1.2.tar` & `VisualShape3D-1.1.3.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 07:35:39.001453 VisualShape3D-1.1.2/
--rw-rw-rw-   0        0        0     1091 2023-12-31 14:32:40.000000 VisualShape3D-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     4883 2024-03-16 07:35:39.001453 VisualShape3D-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4510 2024-03-09 23:58:48.000000 VisualShape3D-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-16 07:35:38.997429 VisualShape3D-1.1.2/VisualShape3D/
--rw-rw-rw-   0        0        0     2460 2024-03-09 20:37:08.000000 VisualShape3D-1.1.2/VisualShape3D/VisualShape3D.py
--rw-rw-rw-   0        0        0        2 2024-02-03 06:58:08.000000 VisualShape3D-1.1.2/VisualShape3D/__init__.py
--rw-rw-rw-   0        0        0    24713 2024-03-09 20:55:48.000000 VisualShape3D-1.1.2/VisualShape3D/geometry.py
--rw-rw-rw-   0        0        0    23528 2024-02-03 06:58:08.000000 VisualShape3D-1.1.2/VisualShape3D/geomutils.py
--rw-rw-rw-   0        0        0     8234 2024-02-03 06:58:08.000000 VisualShape3D-1.1.2/VisualShape3D/mathutils.py
--rw-rw-rw-   0        0        0    18002 2024-02-03 06:58:08.000000 VisualShape3D-1.1.2/VisualShape3D/models.py
--rw-rw-rw-   0        0        0      334 2024-02-03 06:58:08.000000 VisualShape3D-1.1.2/VisualShape3D/plot.py
--rw-rw-rw-   0        0        0    11233 2024-03-03 01:22:16.000000 VisualShape3D-1.1.2/VisualShape3D/plotable.py
--rw-rw-rw-   0        0        0    27209 2024-02-03 06:58:08.000000 VisualShape3D-1.1.2/VisualShape3D/rooms.py
--rw-rw-rw-   0        0        0    10071 2024-03-09 19:57:42.000000 VisualShape3D-1.1.2/VisualShape3D/shapes.py
-drwxrwxrwx   0        0        0        0 2024-03-16 07:35:39.001453 VisualShape3D-1.1.2/VisualShape3D.egg-info/
--rw-rw-rw-   0        0        0     4883 2024-03-16 07:35:38.000000 VisualShape3D-1.1.2/VisualShape3D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2024-03-16 07:35:38.000000 VisualShape3D-1.1.2/VisualShape3D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 07:35:38.000000 VisualShape3D-1.1.2/VisualShape3D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-16 07:35:38.000000 VisualShape3D-1.1.2/VisualShape3D.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-16 07:35:38.000000 VisualShape3D-1.1.2/VisualShape3D.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-16 07:35:39.002956 VisualShape3D-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1327 2024-03-16 07:33:23.000000 VisualShape3D-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:31:32.524736 VisualShape3D-1.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-12-31 14:32:39.000000 VisualShape3D-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4497 2024-05-26 14:31:32.523713 VisualShape3D-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4126 2024-05-26 03:21:32.000000 VisualShape3D-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 14:31:32.518584 VisualShape3D-1.1.3/VisualShape3D/
+-rw-rw-rw-   0        0        0    11437 2024-03-23 08:00:33.000000 VisualShape3D-1.1.3/VisualShape3D/VisualModels.py
+-rw-rw-rw-   0        0        0        2 2024-02-03 06:58:07.000000 VisualShape3D-1.1.3/VisualShape3D/__init__.py
+-rw-rw-rw-   0        0        0    27211 2024-03-11 09:53:54.000000 VisualShape3D-1.1.3/VisualShape3D/examples.py
+-rw-rw-rw-   0        0        0    24701 2024-04-24 01:47:26.000000 VisualShape3D-1.1.3/VisualShape3D/geometry.py
+-rw-rw-rw-   0        0        0    23528 2024-02-03 06:58:07.000000 VisualShape3D-1.1.3/VisualShape3D/geomutils.py
+-rw-rw-rw-   0        0        0     8234 2024-02-03 06:58:07.000000 VisualShape3D-1.1.3/VisualShape3D/mathutils.py
+-rw-rw-rw-   0        0        0    11596 2024-03-18 14:52:13.000000 VisualShape3D-1.1.3/VisualShape3D/plotable.py
+-rw-rw-rw-   0        0        0    10194 2024-05-04 04:37:28.000000 VisualShape3D-1.1.3/VisualShape3D/shapes.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:31:32.522710 VisualShape3D-1.1.3/VisualShape3D.egg-info/
+-rw-rw-rw-   0        0        0     4497 2024-05-26 14:31:32.000000 VisualShape3D-1.1.3/VisualShape3D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2024-05-26 14:31:32.000000 VisualShape3D-1.1.3/VisualShape3D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:31:32.000000 VisualShape3D-1.1.3/VisualShape3D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-26 14:31:32.000000 VisualShape3D-1.1.3/VisualShape3D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-26 14:31:32.000000 VisualShape3D-1.1.3/VisualShape3D.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 14:31:32.524736 VisualShape3D-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1327 2024-05-26 14:23:19.000000 VisualShape3D-1.1.3/setup.py
```

### Comparing `VisualShape3D-1.1.2/LICENSE` & `VisualShape3D-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `VisualShape3D-1.1.2/PKG-INFO` & `VisualShape3D-1.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: VisualShape3D
-Version: 1.1.2
+Version: 1.1.3
 Author: Liqun He
 Author-email: heliqun2007@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
 
 # VisualShape3D
 
 ## VisualShape3D
 
-VisualShape3D is an easy-to-use Python wrapper of matplotlib, designed to facilitate the creation of 3D polygons for educational purposes. The package allows the user to create a view, add shapes into it, and display them all together in the end.
+VisualShape3D is a simple library of geometry designed to quickly build a 3D model with its functions. It starts with creating a viewport at first, followed by adding each 3D shape to it, and finally showing them all at once. There are three shapes: Point, PolyLine, and Polygon. A 3D polygon is created by first defining a 2D shape on the yz plane and then transforms it with both new position and orientation, while its bottom is limited to motion in XY plane. 
 
-There three shapes to have been defined in VisualShape3D : Point, PolyLine, and Polygon. To create a 3D shape, one follows a two-step process: 1) creating a 2D shape in the yz plane; 2) transforming it to desired position to form a 3D shape. During the transformation,  translate the reference point to a new position (X,Y,Z), and then turn its facet to  a new orientation. By default, the first vertex of a shape acts as its reference point, and the orientation is set by two angles (alpha, beta). alpha refers to the angle from y to y' on xy plane , while beta means the other angle from z to z' in xz plane. They are positive anticlockwise.
-
-Besides these features, VisualShape3D also offers the ability to calculate the intersection of a line with a polygon, that is , PolyLine and Polygon. The function serves as a first step towards a more useful tool.
+As seen in the following examples, VisualShape3D is capable of calculating line intersections with polygons, as well as rotating/translating a shape to building a 3D body.
 
 ## Core Features
-* Shapes : Point, Segment锛孭olylines, Polygon, and Shape.
-* It can check whether or not a point is inside a segment or polygon, by using the magic functions __contains__.
-* __hash__ and __eq__, also overloaded for Point, Segment and Polygon.
-* __neg__ overloaded for polygon when one wants to know the list of vertices on its other side.
+* Shapes : Point, Polylines, and Polygon.
+* It can check whether or not a point is inside a segment or polygon.
+* __hash__ and __eq__, also overloaded for ordering and logical equal the three shapes.
+* For a shape, __neg__ is overloaded for one to get thevertices in the order viewed from its other side.
 
 ## Requirements
 
 * [Python](http://www.python.org) 3 
 * Matplotlib is needed.
 
 ## Documentation
@@ -39,73 +37,74 @@
 ## Installation
 ```bash
 pip install VisualShape3D
 ```
 
 ## Usage 
 
-* case 1 : building a box.  
-from VisualShape3D import VisualShape3D as vs3d
-from VisualShape3D.geometry import Shape 
-
-A,B,C = 6,6,3
-P1,P2,P3,P4 = (A,0,0),(A,B,0),(A,B,C),(A,0,C)
-P5,P6,P7,P8 = (0,0,0),(0,B,0),(0,B,C),(0,0,C)
-V = [P1,P2,P3,P4,P5,P6,P7,P8]
-shape1 = Shape("Polygon",vertices = [V[0],V[1],V[2],V[3]])
-shape2 = Shape("Polygon",vertices = [V[1],V[2],V[6],V[5]])
-shape3 = Shape("Polygon",vertices = [V[5],V[4],V[7],V[6]])
-shape4 = Shape("Polygon",vertices = [V[4],V[0],V[3],V[7]])
-shape5 = Shape("Polygon",vertices = [V[3],V[2],V[6],V[7]])
+* case 1 : building a box.
+from VisualShape3D.VisualModels import VisualShape3D as vs3d 
+from VisualShape3D.geometry import Shape
+A,B,C = 6,6,3 
+P1,P2,P3,P4 = (A,0,0),(A,B,0),(A,B,C),(A,0,C) 
+P5,P6,P7,P8 = (0,0,0),(0,B,0),(0,B,C),(0,0,C) 
+V = [P1,P2,P3,P4,P5,P6,P7,P8] 
+shape1 = Shape("Polygon",vertices = [V[0],V[1],V[2],V[3]]) 
+shape2 = Shape("Polygon",vertices = [V[1],V[2],V[6],V[5]]) 
+shape3 = Shape("Polygon",vertices = [V[5],V[4],V[7],V[6]]) 
+shape4 = Shape("Polygon",vertices = [V[4],V[0],V[3],V[7]]) 
+shape5 = Shape("Polygon",vertices = [V[3],V[2],V[6],V[7]]) 
 shape6 = Shape("Polygon",vertices = [V[4],V[5],V[1],V[0]])
 
-body = vs3d.VisualShape3D({'facecolor':'yellow','alpha':0.7})
-body.add_shape(shape1,{'facecolor':'red','alpha':0.7})
-body.add_shape(shape2)
-body.add_shape(shape3)
-body.add_shape(shape4)
-body.add_shape(shape5)
-body.add_shape(shape6)
+body = vs3d({'facecolor':'yellow','alpha':0.7}) 
+body.add_shape(shape1,{'facecolor':'red','alpha':0.7}) 
+body.add_shape(shape2) 
+body.add_shape(shape3) 
+body.add_shape(shape4) 
+body.add_shape(shape5) 
+body.add_shape(shape6) 
 body.show()
 
-* case 2 : rotating a shape
-from VisualShape3D import VisualShape3D as vs3d
-from VisualShape3D.geometry import Shape 
-
-A,B,C = 6,6,3
-P1,P2,P3,P4 = (A,0,0),(A,B,0),(A,B,C),(A,0,C)
-P5,P6,P7,P8 = (0,0,0),(0,B,0),(0,B,C),(0,0,C)
-V = [P1,P2,P3,P4,P5,P6,P7,P8]
+* case 2 : rotating a shape 
+from VisualShape3D.VisualModels import VisualShape3D as vs3d 
+from VisualShape3D.geometry import Shape
+A,B,C = 6,6,3 
+P1,P2,P3,P4 = (A,0,0),(A,B,0),(A,B,C),(A,0,C) 
+P5,P6,P7,P8 = (0,0,0),(0,B,0),(0,B,C),(0,0,C) 
+V = [P1,P2,P3,P4,P5,P6,P7,P8] 
 shape1 = Shape("Polygon",vertices = [V[0],V[1],V[2],V[3]])
 
-shape11 = shape1
-shape12 = shape11.transform(angles = (90,0))
-shape13 = shape12.transform(angles = (90,0))
+shape11 = shape1 
+shape12 = shape11.transform(angles = (90,0)) 
+shape13 = shape12.transform(angles = (90,0)) 
 shape14 = shape13.transform(angles = (90,0))
 
-body = vs3d.VisualShape3D({'facecolor':'yellow','alpha':0.7})
-body.add_shape(shape11,{'facecolor':'red','alpha':0.7})
-body.add_shape(shape12)
-body.add_shape(shape13)
-body.add_shape(shape14)
+body = vs3d({'facecolor':'yellow','alpha':0.7}) 
+body.add_shape(shape11,{'facecolor':'red','alpha':0.7}) 
+body.add_shape(shape12) 
+body.add_shape(shape13) 
+body.add_shape(shape14) 
 body.show()
 
-* case 3 : roating and translating a shape
-shape11 = shape1
-shape12 = shape11.transform(to = shape11[1],angles = (90,0))
-shape13 = shape12.transform(to = shape12[1],angles = (90,0))
+* case 3 : roating and translating a shape 
+from VisualShape3D.VisualModels import VisualShape3D as vs3d
+from VisualShape3D.geometry import Shape
+
+shape11 = shape1 
+shape12 = shape11.transform(to = shape11[1],angles = (90,0)) 
+shape13 = shape12.transform(to = shape12[1],angles = (90,0)) 
 shape14 = shape13.transform(to = shape13[1],angles = (90,0))
-
-body = vs3d.VisualShape3D({'facecolor':'yellow','alpha':0.7})
-body.add_shape(shape11,{'facecolor':'red','alpha':0.7})
-body.add_shape(shape12)
-body.add_shape(shape13)
-body.add_shape(shape14)
+body = vs3d({'facecolor':'yellow','alpha':0.7}) 
+body.add_shape(shape11,{'facecolor':'red','alpha':0.7}) 
+body.add_shape(shape12) 
+body.add_shape(shape13) 
+body.add_shape(shape14) 
 body.show()
 
+
 ## Change Log
 
 [changelog.md](changelog.md)
 
 ## License
 
     This program is free software: you can redistribute it and/or modify
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `VisualShape3D-1.1.2/README.md` & `VisualShape3D-1.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # VisualShape3D
 
 ## VisualShape3D
 
-VisualShape3D is an easy-to-use Python wrapper of matplotlib, designed to facilitate the creation of 3D polygons for educational purposes. The package allows the user to create a view, add shapes into it, and display them all together in the end.
+VisualShape3D is a simple library of geometry designed to quickly build a 3D model with its functions. It starts with creating a viewport at first, followed by adding each 3D shape to it, and finally showing them all at once. There are three shapes: Point, PolyLine, and Polygon. A 3D polygon is created by first defining a 2D shape on the yz plane and then transforms it with both new position and orientation, while its bottom is limited to motion in XY plane. 
 
-There three shapes to have been defined in VisualShape3D : Point, PolyLine, and Polygon. To create a 3D shape, one follows a two-step process: 1) creating a 2D shape in the yz plane; 2) transforming it to desired position to form a 3D shape. During the transformation,  translate the reference point to a new position (X,Y,Z), and then turn its facet to  a new orientation. By default, the first vertex of a shape acts as its reference point, and the orientation is set by two angles (alpha, beta). alpha refers to the angle from y to y' on xy plane , while beta means the other angle from z to z' in xz plane. They are positive anticlockwise.
-
-Besides these features, VisualShape3D also offers the ability to calculate the intersection of a line with a polygon, that is , PolyLine and Polygon. The function serves as a first step towards a more useful tool.
+As seen in the following examples, VisualShape3D is capable of calculating line intersections with polygons, as well as rotating/translating a shape to building a 3D body.
 
 ## Core Features
-* Shapes : Point, Segment，Polylines, Polygon, and Shape.
-* It can check whether or not a point is inside a segment or polygon, by using the magic functions __contains__.
-* __hash__ and __eq__, also overloaded for Point, Segment and Polygon.
-* __neg__ overloaded for polygon when one wants to know the list of vertices on its other side.
+* Shapes : Point, Polylines, and Polygon.
+* It can check whether or not a point is inside a segment or polygon.
+* __hash__ and __eq__, also overloaded for ordering and logical equal the three shapes.
+* For a shape, __neg__ is overloaded for one to get thevertices in the order viewed from its other side.
 
 ## Requirements
 
 * [Python](http://www.python.org) 3 
 * Matplotlib is needed.
 
 ## Documentation
@@ -26,73 +24,74 @@
 ## Installation
 ```bash
 pip install VisualShape3D
 ```
 
 ## Usage 
 
-* case 1 : building a box.  
-from VisualShape3D import VisualShape3D as vs3d
-from VisualShape3D.geometry import Shape 
-
-A,B,C = 6,6,3
-P1,P2,P3,P4 = (A,0,0),(A,B,0),(A,B,C),(A,0,C)
-P5,P6,P7,P8 = (0,0,0),(0,B,0),(0,B,C),(0,0,C)
-V = [P1,P2,P3,P4,P5,P6,P7,P8]
-shape1 = Shape("Polygon",vertices = [V[0],V[1],V[2],V[3]])
-shape2 = Shape("Polygon",vertices = [V[1],V[2],V[6],V[5]])
-shape3 = Shape("Polygon",vertices = [V[5],V[4],V[7],V[6]])
-shape4 = Shape("Polygon",vertices = [V[4],V[0],V[3],V[7]])
-shape5 = Shape("Polygon",vertices = [V[3],V[2],V[6],V[7]])
+* case 1 : building a box.
+from VisualShape3D.VisualModels import VisualShape3D as vs3d 
+from VisualShape3D.geometry import Shape
+A,B,C = 6,6,3 
+P1,P2,P3,P4 = (A,0,0),(A,B,0),(A,B,C),(A,0,C) 
+P5,P6,P7,P8 = (0,0,0),(0,B,0),(0,B,C),(0,0,C) 
+V = [P1,P2,P3,P4,P5,P6,P7,P8] 
+shape1 = Shape("Polygon",vertices = [V[0],V[1],V[2],V[3]]) 
+shape2 = Shape("Polygon",vertices = [V[1],V[2],V[6],V[5]]) 
+shape3 = Shape("Polygon",vertices = [V[5],V[4],V[7],V[6]]) 
+shape4 = Shape("Polygon",vertices = [V[4],V[0],V[3],V[7]]) 
+shape5 = Shape("Polygon",vertices = [V[3],V[2],V[6],V[7]]) 
 shape6 = Shape("Polygon",vertices = [V[4],V[5],V[1],V[0]])
 
-body = vs3d.VisualShape3D({'facecolor':'yellow','alpha':0.7})
-body.add_shape(shape1,{'facecolor':'red','alpha':0.7})
-body.add_shape(shape2)
-body.add_shape(shape3)
-body.add_shape(shape4)
-body.add_shape(shape5)
-body.add_shape(shape6)
+body = vs3d({'facecolor':'yellow','alpha':0.7}) 
+body.add_shape(shape1,{'facecolor':'red','alpha':0.7}) 
+body.add_shape(shape2) 
+body.add_shape(shape3) 
+body.add_shape(shape4) 
+body.add_shape(shape5) 
+body.add_shape(shape6) 
 body.show()
 
-* case 2 : rotating a shape
-from VisualShape3D import VisualShape3D as vs3d
-from VisualShape3D.geometry import Shape 
-
-A,B,C = 6,6,3
-P1,P2,P3,P4 = (A,0,0),(A,B,0),(A,B,C),(A,0,C)
-P5,P6,P7,P8 = (0,0,0),(0,B,0),(0,B,C),(0,0,C)
-V = [P1,P2,P3,P4,P5,P6,P7,P8]
+* case 2 : rotating a shape 
+from VisualShape3D.VisualModels import VisualShape3D as vs3d 
+from VisualShape3D.geometry import Shape
+A,B,C = 6,6,3 
+P1,P2,P3,P4 = (A,0,0),(A,B,0),(A,B,C),(A,0,C) 
+P5,P6,P7,P8 = (0,0,0),(0,B,0),(0,B,C),(0,0,C) 
+V = [P1,P2,P3,P4,P5,P6,P7,P8] 
 shape1 = Shape("Polygon",vertices = [V[0],V[1],V[2],V[3]])
 
-shape11 = shape1
-shape12 = shape11.transform(angles = (90,0))
-shape13 = shape12.transform(angles = (90,0))
+shape11 = shape1 
+shape12 = shape11.transform(angles = (90,0)) 
+shape13 = shape12.transform(angles = (90,0)) 
 shape14 = shape13.transform(angles = (90,0))
 
-body = vs3d.VisualShape3D({'facecolor':'yellow','alpha':0.7})
-body.add_shape(shape11,{'facecolor':'red','alpha':0.7})
-body.add_shape(shape12)
-body.add_shape(shape13)
-body.add_shape(shape14)
+body = vs3d({'facecolor':'yellow','alpha':0.7}) 
+body.add_shape(shape11,{'facecolor':'red','alpha':0.7}) 
+body.add_shape(shape12) 
+body.add_shape(shape13) 
+body.add_shape(shape14) 
 body.show()
 
-* case 3 : roating and translating a shape
-shape11 = shape1
-shape12 = shape11.transform(to = shape11[1],angles = (90,0))
-shape13 = shape12.transform(to = shape12[1],angles = (90,0))
+* case 3 : roating and translating a shape 
+from VisualShape3D.VisualModels import VisualShape3D as vs3d
+from VisualShape3D.geometry import Shape
+
+shape11 = shape1 
+shape12 = shape11.transform(to = shape11[1],angles = (90,0)) 
+shape13 = shape12.transform(to = shape12[1],angles = (90,0)) 
 shape14 = shape13.transform(to = shape13[1],angles = (90,0))
-
-body = vs3d.VisualShape3D({'facecolor':'yellow','alpha':0.7})
-body.add_shape(shape11,{'facecolor':'red','alpha':0.7})
-body.add_shape(shape12)
-body.add_shape(shape13)
-body.add_shape(shape14)
+body = vs3d({'facecolor':'yellow','alpha':0.7}) 
+body.add_shape(shape11,{'facecolor':'red','alpha':0.7}) 
+body.add_shape(shape12) 
+body.add_shape(shape13) 
+body.add_shape(shape14) 
 body.show()
 
+
 ## Change Log
 
 [changelog.md](changelog.md)
 
 ## License
 
     This program is free software: you can redistribute it and/or modify
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `VisualShape3D-1.1.2/VisualShape3D/geometry.py` & `VisualShape3D-1.1.3/VisualShape3D/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             raise ValueError('Polygon : needs vertices as a list/np.array !!!')   
         
         if Points.shape[1] == 2:
             # from Utilities import add_col
             Points = np.hstack((Points,add_col(Points.shape[0])*0))
             
         self.vertices = Points
-        self.R0 = self.vertices[0,:]
+        self.R0 = self.vertices[0]
         self.n  = self.getNormal()
         self.area = self.getArea()
   
         # Optional processing
         self.path = None
         self.parametric = None
         self.shapely = None
@@ -298,15 +298,15 @@
         """
         :returns: opposite vertices of the bounding prism for this object.
         :       ndarray([min], [max])
         """
 
         # Min/max along the column
         return np.array([self.vertices.min(axis=0),  # min (x,y,z)
-                          self.vertices.max(axis=0)]) # max (x,y,z)
+                         self.vertices.max(axis=0)]) # max (x,y,z)
 
     def iplot(self, style, ax, **kwargs):
 
         plotable3d = self.__get_plotable_data()
 
         facecolor = self.facecolor  
         edgecolor = self.edgecolor  
@@ -645,25 +645,25 @@
         if (isinstance(shape, str) and isDefaultShape(shape)) or shape is None:
             vertices = self.createVertices(shape or 'rectangle', *args, **kwargs)
                 
         # 如果shape是列表或NumPy数组，直接使用这些顶点
         elif isinstance(shape, (list, np.ndarray)):
             vertices = np.asarray(shape)
             if vertices.shape[1] == 2:
-                vertices = np.hstack((arange_col(vertices.shape[0])*0, vertices)) 
+                vertices = np.hstack((add_col(vertices.shape[0])*0, vertices)) 
                 
             self.shapeName = 'polygon'  # 如果直接给定顶点，形状类型设置为多边形
             self.input_str = f"'Polygon', vertices = {self.listThem(vertices)}"
         else:
             # 如果shape是新的字符串命，根据 W 所含数据创建顶点
             if isinstance(shape, str) and isinstance(W, (list, np.ndarray)):
                 self.shapeName = shape.lower()
                 vertices = np.asarray(W)
                 if vertices.shape[1] == 2:
-                    vertices = np.hstack((arange_col(vertices.shape[0])*0, vertices)) 
+                    vertices = np.hstack((add_col(vertices.shape[0])*0, vertices)) 
                 
                 self.input_str = f"'{self.shapeName}', vertices = {self.listThem(vertices)}"
             else :
                 raise ValueError(f"Unsupported shape type: {type(shape)}")
             
         points = np.asarray(vertices)
         super().__init__(points)      
@@ -705,15 +705,15 @@
             dict_str = getShapeInputDict(self.shapeName,*args_)
             self.input_str = format_dict(dict_str)
  
         vertices = createShape(self.shapeName,*args_)
 
         # Adapt 2D/3D
         if vertices.shape[1] == 2:
-            vertices = np.hstack((arange_col(vertices.shape[0])*0, vertices))
+            vertices = np.hstack((add_col(vertices.shape[0])*0, vertices))
             
         return vertices
     
     def __str__(self):
         return f"{len(self.vertices)} vertices :\n{self.vertices}"
 
     def __repr__(self):
```

### Comparing `VisualShape3D-1.1.2/VisualShape3D/geomutils.py` & `VisualShape3D-1.1.3/VisualShape3D/geomutils.py`

 * *Files identical despite different names*

### Comparing `VisualShape3D-1.1.2/VisualShape3D/mathutils.py` & `VisualShape3D-1.1.3/VisualShape3D/mathutils.py`

 * *Files identical despite different names*

### Comparing `VisualShape3D-1.1.2/VisualShape3D/plotable.py` & `VisualShape3D-1.1.3/VisualShape3D/plotable.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,25 +63,34 @@
         self.linewidth  = 1
         self.linestyle ="solid"
         self.alpha      = 1
         self.marker     ='o'
         self.label = None
         self.entity_title = self.__class__.__name__
 
+    
+    def set_fig(self, fig):
+        Plotable._fig = fig
+
+    def get_fig(self):
+        return Plotable._fig
+
     def set_ax(self, ax):
         Plotable._ax = ax
 
     def get_ax(self):
         return Plotable._ax
 
     def clear_ax(self):
         self.set_ax(None)
 
     def close(self):
-        plt.close()
+        plt.close(Plotable._fig)
+        self.clear_ax()
+        self.set_fig(None)
 
     def get_title(self):
         return self.entity_title
 
     def set_title(self, str):
         self.entity_title = str
 
@@ -112,14 +121,27 @@
         style['linewidth'] = self.linewidth
         style['linestyle'] = self.linestyle
         style['alpha']     = self.alpha    
         style['color']     = self.color    
         style['marker']    = self.marker   
         return style
 
+    def adjust_style(self,style):
+        if 'facecolor' not in style : style['facecolor'] = 'default' 
+        if 'edgecolor' not in style : style['edgecolor'] = 'default' 
+        if 'linewidth' not in style : style['linewidth'] = 'default' 
+        if 'alpha'     not in style : style['alpha']     = 'default' 
+
+        if style['facecolor'] == 'default' : style['facecolor'] = self.facecolor
+        if style['edgecolor'] == 'default' : style['edgecolor'] = self.edgecolor
+        if style['linewidth'] == 'default' : style['linewidth'] = self.linewidth
+        if style['alpha']     == 'default' : style['alpha']     = self.alpha    
+
+        return style
+
 ### Functions
     def show(self, elev= 20.0, azim = -80.0, hideAxes = False, origin = False):
         ax = self.get_ax()
 
         if ax is None :
             return
       
@@ -132,17 +154,15 @@
             R0 = Origin()
             self.add_plot(R0)
 
         plt.show()
 
         return ax
 
-
-    def plot(self, style = {'facecolor':'default','edgecolor':'default','linewidth':'default','alpha':'default'}, ax = None, 
-                   hideAxes = False, **kwargs):
+    def plot(self, style = {}, ax = None, hideAxes = False, **kwargs):
         """
         it will plot geometry in the settings as follow 
   
          1) style :
               style = {'facecolor','edgecolor','linewidth','alpha','node','nodemarker','nodecolor'}
               It matters differently for line and polygon 
                 = (edge color, line width, alpha) for segement, line, polyline and Ray
@@ -160,37 +180,56 @@
             plt.show() activates all plots.
         """
 
         bAdjustViewport = True     # to hold new geometries
         if ax is None:
             if self.get_ax() is None : 
                 
-                # it is the very first plot of one alone application
+                # it is at the very first time for plotting
                 fig = plt.figure()
                 ax = fig.add_subplot(111, projection='3d')
                 self.set_ax(ax)
                 bAdjustViewport = False
                 
-            else :          # or it plot in the ax of an GUI app
-                pass        
+            else :  # plotting in the exisitng ax of an GUI app
+                raise ValueError('instance.plot( ..., ax = ax, ... ) !!!')        
 
         # fetch the instance of a geometry
         # instance = self.__class__(**self.get_seed())
         instance = self.get_instance()
-
         if instance is None : # in the case for an instance of Plotable itself.
             return  
 
         # print(f" instance = {type(instance)}")
         # print(f" self = {type(self)}")
         # print(f" ax = {type(ax)}")
 
-        # adjust viewport to hold the instance 
-        domain = instance.get_domain()
+        # Plot instance
+        style = self.adjust_style(style)
+        instance.iplot(style = style, ax = ax, **kwargs)
+
+        # adjust viewport
+        self.adjust_viewport(ax, instance, bAdjustViewport)
+
+        if hideAxes :
+            ax.set_axis_off()
+            # self.draw_origin()
+
+        else :
+            ax.set_xlabel('x')
+            ax.set_ylabel('y')
+            ax.set_zlabel('z')
+
+        return ax
+
+
 
+    def adjust_viewport(self, ax, instance, bAdjustViewport):
+        
+        domain = instance.get_domain()
         bound = np.max(domain[1]-domain[0])
         centroid = instance.get_centroid()
         pos = np.vstack((centroid-bound/2, centroid+bound/2))
         pos[0,2] = domain[0,2]
         pos[1,2] = pos[0,2] + bound
         
         # Overlap the existing plots 
@@ -198,106 +237,79 @@
             old_pos = np.array([ax.get_xbound(),
                                 ax.get_ybound(),
                                 ax.get_zbound()]).T
             pos = np.dstack((pos, old_pos))
             pos = np.array([np.min(pos[0, :, :], axis=1),
                             np.max(pos[1, :, :], axis=1)])
 
-
-        # Plot instance
-        if 'facecolor' not in style : style['facecolor'] = 'default' 
-        if 'edgecolor' not in style : style['edgecolor'] = 'default' 
-        if 'linewidth' not in style : style['linewidth'] = 'default' 
-        if 'alpha'     not in style : style['alpha']     = 'default' 
-
-        if style['facecolor'] == 'default' : style['facecolor'] = self.facecolor
-        if style['edgecolor'] == 'default' : style['edgecolor'] = self.edgecolor
-        if style['linewidth'] == 'default' : style['linewidth'] = self.linewidth
-        if style['alpha']     == 'default' : style['alpha']     = self.alpha    
-
-        instance.iplot(style = style, ax = ax, **kwargs)
-
-        # Axis limits
         ax.set_xlim3d(left   = pos[0,0], right = pos[1,0])
         ax.set_ylim3d(bottom = pos[0,1], top   = pos[1,1])
         ax.set_zlim3d(bottom = pos[0,2], top   = pos[1,2])
 
-        if hideAxes :
-            ax.set_axis_off()
-            # self.draw_origin()
-
-        else :
-            ax.set_xlabel('x')
-            ax.set_ylabel('y')
-            ax.set_zlabel('z')
-
-        return ax
-
 
-    def add_plot(self, shape, 
-                 style = {'facecolor':'default','edgecolor':'default','linewidth':'default','alpha':'default'},
-                 hideAxes = False, **kwargs):
-
-        if not isinstance(shape, Plotable):
-            return None
-
-        return shape.plot(style = style, ax = self.get_ax(), hideAxes=hideAxes,**kwargs)
+    def get_domain(self) :
+        ax = self.get_ax()
+        domain = np.array([ax.get_xbound(), 
+                           ax.get_ybound(),
+                           ax.get_zbound()]).T
+        return domain
 
- 
     def get_centroid(self):
         """
         The centroid refers to the center of the circumscribed
         paralellepiped, not its mass center.
         
         it returns a ndarray of (x, y, z).
         
         """
         return self.get_domain().mean(axis=0)
 
-### Custom get_instance()/iplot()/get_domain()
+    def add_plot(self, shape, 
+                 style = {'facecolor':'default','edgecolor':'default','linewidth':'default','alpha':'default'},
+                 hideAxes = False, **kwargs):
+        if not isinstance(shape, Plotable):
+            return None
+        return shape.plot(style = style, ax = self.get_ax(), hideAxes=hideAxes,**kwargs)
+
+### visual infrastructure ::  get_instance()/iplot()/get_domain()
     def get_instance(self): 
         return self
 
     def iplot(self, style, ax, **kwargs):
         if ax is None:
             ax = self.get_ax()
 
         R0 = Origin()
         R0.iplot(style, ax, **kwargs)
 
-    def get_domain(self) :
 
-        ax = self.get_ax()
-        domain = np.array([ax.get_xbound(), 
-                           ax.get_ybound(),
-                           ax.get_zbound()])
-        return domain.T
  
 class OpenView(Plotable):
 ### Initialization
-    def __init__(self, ax=None):
+    def __init__(self, ax = None):
         super().__init__()
+
         if self.get_ax() is not None:
             self.clear_ax()
 
         if ax is None :
             # it is the very first plot of the application
             fig = plt.figure()
+            self.set_fig(fig)
             ax = fig.add_subplot(111, projection='3d')
             
         self.set_ax(ax)
 
 
 class Origin(Plotable):
     def __init__(self):
         super().__init__()    
 
 ### Custom get_instance()/iplot()/get_domain()
     def get_instance(self): return self
-
     def iplot(self, style, ax, **kwargs):
         if ax is None:
             ax = self.get_ax()
 
         xmin, xmax = ax.get_xlim()
         ymin, ymax = ax.get_ylim()
         zmin, zmax = ax.get_zlim()
```

### Comparing `VisualShape3D-1.1.2/VisualShape3D/rooms.py` & `VisualShape3D-1.1.3/VisualShape3D/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import VisualShape3D.geometry as vs
 import VisualShape3D.plotable as rd
 import numpy as np
 
+
 highEfficiencyMode = False  # 高效率模式下，会减少一些边，从而提高预览速率
 
 
 class room():  # 右侧的带遮阳棚小屋
     def __init__(self, xSize, ySize, zSize, roomNumber, style):
         self.xSize = xSize  # 房间的长
         self.ySize = ySize  # 房间的宽
```

### Comparing `VisualShape3D-1.1.2/VisualShape3D/shapes.py` & `VisualShape3D-1.1.3/VisualShape3D/shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,16 +291,18 @@
 
     U = tranMatrix(alpha,beta)
     facet_new = U.dot(facet) + dR
 
     return facet_new.transpose()
 
 # row-based calculation : V * U  + V0
-def transform(shape = rectangle(1.0,1.0), reference = None, to = None, angles = (0.0,0.0)):
-    alpha, beta = angles
+def transform(shape = rectangle(1.0,1.0), reference = None, to = None, by = None, angles = (0.0,0.0)):
+    alpha, beta = angles[0], angles[1]
+    if by is not None :
+        alpha, beta = by[0], by[1]    #  Outdated, obsolete parameters 
     U = tranMatrix(alpha, beta)
 
     vertices = shape
     if vertices.shape[1] == 2:
         vertices = np.hstack((add_col(vertices.shape[0])*0, vertices))    
 
     if reference is None : reference = vertices[0,:]
```

### Comparing `VisualShape3D-1.1.2/VisualShape3D.egg-info/PKG-INFO` & `VisualShape3D-1.1.3/VisualShape3D.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: VisualShape3D
-Version: 1.1.2
+Version: 1.1.3
 Author: Liqun He
 Author-email: heliqun2007@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
 
 # VisualShape3D
 
 ## VisualShape3D
 
-VisualShape3D is an easy-to-use Python wrapper of matplotlib, designed to facilitate the creation of 3D polygons for educational purposes. The package allows the user to create a view, add shapes into it, and display them all together in the end.
+VisualShape3D is a simple library of geometry designed to quickly build a 3D model with its functions. It starts with creating a viewport at first, followed by adding each 3D shape to it, and finally showing them all at once. There are three shapes: Point, PolyLine, and Polygon. A 3D polygon is created by first defining a 2D shape on the yz plane and then transforms it with both new position and orientation, while its bottom is limited to motion in XY plane. 
 
-There three shapes to have been defined in VisualShape3D : Point, PolyLine, and Polygon. To create a 3D shape, one follows a two-step process: 1) creating a 2D shape in the yz plane; 2) transforming it to desired position to form a 3D shape. During the transformation,  translate the reference point to a new position (X,Y,Z), and then turn its facet to  a new orientation. By default, the first vertex of a shape acts as its reference point, and the orientation is set by two angles (alpha, beta). alpha refers to the angle from y to y' on xy plane , while beta means the other angle from z to z' in xz plane. They are positive anticlockwise.
-
-Besides these features, VisualShape3D also offers the ability to calculate the intersection of a line with a polygon, that is , PolyLine and Polygon. The function serves as a first step towards a more useful tool.
+As seen in the following examples, VisualShape3D is capable of calculating line intersections with polygons, as well as rotating/translating a shape to building a 3D body.
 
 ## Core Features
-* Shapes : Point, Segment锛孭olylines, Polygon, and Shape.
-* It can check whether or not a point is inside a segment or polygon, by using the magic functions __contains__.
-* __hash__ and __eq__, also overloaded for Point, Segment and Polygon.
-* __neg__ overloaded for polygon when one wants to know the list of vertices on its other side.
+* Shapes : Point, Polylines, and Polygon.
+* It can check whether or not a point is inside a segment or polygon.
+* __hash__ and __eq__, also overloaded for ordering and logical equal the three shapes.
+* For a shape, __neg__ is overloaded for one to get thevertices in the order viewed from its other side.
 
 ## Requirements
 
 * [Python](http://www.python.org) 3 
 * Matplotlib is needed.
 
 ## Documentation
@@ -39,73 +37,74 @@
 ## Installation
 ```bash
 pip install VisualShape3D
 ```
 
 ## Usage 
 
-* case 1 : building a box.  
-from VisualShape3D import VisualShape3D as vs3d
-from VisualShape3D.geometry import Shape 
-
-A,B,C = 6,6,3
-P1,P2,P3,P4 = (A,0,0),(A,B,0),(A,B,C),(A,0,C)
-P5,P6,P7,P8 = (0,0,0),(0,B,0),(0,B,C),(0,0,C)
-V = [P1,P2,P3,P4,P5,P6,P7,P8]
-shape1 = Shape("Polygon",vertices = [V[0],V[1],V[2],V[3]])
-shape2 = Shape("Polygon",vertices = [V[1],V[2],V[6],V[5]])
-shape3 = Shape("Polygon",vertices = [V[5],V[4],V[7],V[6]])
-shape4 = Shape("Polygon",vertices = [V[4],V[0],V[3],V[7]])
-shape5 = Shape("Polygon",vertices = [V[3],V[2],V[6],V[7]])
+* case 1 : building a box.
+from VisualShape3D.VisualModels import VisualShape3D as vs3d 
+from VisualShape3D.geometry import Shape
+A,B,C = 6,6,3 
+P1,P2,P3,P4 = (A,0,0),(A,B,0),(A,B,C),(A,0,C) 
+P5,P6,P7,P8 = (0,0,0),(0,B,0),(0,B,C),(0,0,C) 
+V = [P1,P2,P3,P4,P5,P6,P7,P8] 
+shape1 = Shape("Polygon",vertices = [V[0],V[1],V[2],V[3]]) 
+shape2 = Shape("Polygon",vertices = [V[1],V[2],V[6],V[5]]) 
+shape3 = Shape("Polygon",vertices = [V[5],V[4],V[7],V[6]]) 
+shape4 = Shape("Polygon",vertices = [V[4],V[0],V[3],V[7]]) 
+shape5 = Shape("Polygon",vertices = [V[3],V[2],V[6],V[7]]) 
 shape6 = Shape("Polygon",vertices = [V[4],V[5],V[1],V[0]])
 
-body = vs3d.VisualShape3D({'facecolor':'yellow','alpha':0.7})
-body.add_shape(shape1,{'facecolor':'red','alpha':0.7})
-body.add_shape(shape2)
-body.add_shape(shape3)
-body.add_shape(shape4)
-body.add_shape(shape5)
-body.add_shape(shape6)
+body = vs3d({'facecolor':'yellow','alpha':0.7}) 
+body.add_shape(shape1,{'facecolor':'red','alpha':0.7}) 
+body.add_shape(shape2) 
+body.add_shape(shape3) 
+body.add_shape(shape4) 
+body.add_shape(shape5) 
+body.add_shape(shape6) 
 body.show()
 
-* case 2 : rotating a shape
-from VisualShape3D import VisualShape3D as vs3d
-from VisualShape3D.geometry import Shape 
-
-A,B,C = 6,6,3
-P1,P2,P3,P4 = (A,0,0),(A,B,0),(A,B,C),(A,0,C)
-P5,P6,P7,P8 = (0,0,0),(0,B,0),(0,B,C),(0,0,C)
-V = [P1,P2,P3,P4,P5,P6,P7,P8]
+* case 2 : rotating a shape 
+from VisualShape3D.VisualModels import VisualShape3D as vs3d 
+from VisualShape3D.geometry import Shape
+A,B,C = 6,6,3 
+P1,P2,P3,P4 = (A,0,0),(A,B,0),(A,B,C),(A,0,C) 
+P5,P6,P7,P8 = (0,0,0),(0,B,0),(0,B,C),(0,0,C) 
+V = [P1,P2,P3,P4,P5,P6,P7,P8] 
 shape1 = Shape("Polygon",vertices = [V[0],V[1],V[2],V[3]])
 
-shape11 = shape1
-shape12 = shape11.transform(angles = (90,0))
-shape13 = shape12.transform(angles = (90,0))
+shape11 = shape1 
+shape12 = shape11.transform(angles = (90,0)) 
+shape13 = shape12.transform(angles = (90,0)) 
 shape14 = shape13.transform(angles = (90,0))
 
-body = vs3d.VisualShape3D({'facecolor':'yellow','alpha':0.7})
-body.add_shape(shape11,{'facecolor':'red','alpha':0.7})
-body.add_shape(shape12)
-body.add_shape(shape13)
-body.add_shape(shape14)
+body = vs3d({'facecolor':'yellow','alpha':0.7}) 
+body.add_shape(shape11,{'facecolor':'red','alpha':0.7}) 
+body.add_shape(shape12) 
+body.add_shape(shape13) 
+body.add_shape(shape14) 
 body.show()
 
-* case 3 : roating and translating a shape
-shape11 = shape1
-shape12 = shape11.transform(to = shape11[1],angles = (90,0))
-shape13 = shape12.transform(to = shape12[1],angles = (90,0))
+* case 3 : roating and translating a shape 
+from VisualShape3D.VisualModels import VisualShape3D as vs3d
+from VisualShape3D.geometry import Shape
+
+shape11 = shape1 
+shape12 = shape11.transform(to = shape11[1],angles = (90,0)) 
+shape13 = shape12.transform(to = shape12[1],angles = (90,0)) 
 shape14 = shape13.transform(to = shape13[1],angles = (90,0))
-
-body = vs3d.VisualShape3D({'facecolor':'yellow','alpha':0.7})
-body.add_shape(shape11,{'facecolor':'red','alpha':0.7})
-body.add_shape(shape12)
-body.add_shape(shape13)
-body.add_shape(shape14)
+body = vs3d({'facecolor':'yellow','alpha':0.7}) 
+body.add_shape(shape11,{'facecolor':'red','alpha':0.7}) 
+body.add_shape(shape12) 
+body.add_shape(shape13) 
+body.add_shape(shape14) 
 body.show()
 
+
 ## Change Log
 
 [changelog.md](changelog.md)
 
 ## License
 
     This program is free software: you can redistribute it and/or modify
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `VisualShape3D-1.1.2/setup.py` & `VisualShape3D-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
  
 setuptools.setup(
     # Here is the module name.
     name="VisualShape3D",
  
     # version of the module
-    version="1.1.2",
+    version="1.1.3",
  
     # Name of Author
     author="Liqun He",
  
     # your Email address
     author_email="heliqun2007@gmail.com",
```

