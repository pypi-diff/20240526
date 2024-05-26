# Comparing `tmp/HSPiPy-0.2.tar.gz` & `tmp/hspipy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HSPiPy-0.2.tar", last modified: Sun Jan 28 20:50:09 2024, max compression
+gzip compressed data, was "hspipy-0.3.tar", last modified: Sun May 26 13:17:19 2024, max compression
```

## Comparing `HSPiPy-0.2.tar` & `hspipy-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-01-28 20:50:09.632641 HSPiPy-0.2/
-drwxrwxrwx   0        0        0        0 2024-01-28 20:50:09.624641 HSPiPy-0.2/HSPiPy.egg-info/
--rw-rw-rw-   0        0        0      774 2024-01-28 20:50:09.000000 HSPiPy-0.2/HSPiPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-01-28 20:50:09.000000 HSPiPy-0.2/HSPiPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-28 20:50:09.000000 HSPiPy-0.2/HSPiPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-01-28 20:50:09.000000 HSPiPy-0.2/HSPiPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-01-28 20:50:09.000000 HSPiPy-0.2/HSPiPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-12-06 15:48:34.000000 HSPiPy-0.2/LICENSE
--rw-rw-rw-   0        0        0      774 2024-01-28 20:50:09.632641 HSPiPy-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       49 2023-12-07 11:35:46.000000 HSPiPy-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-01-28 20:50:09.616088 HSPiPy-0.2/hspipy/
--rw-rw-rw-   0        0        0       26 2023-12-31 12:01:36.000000 HSPiPy-0.2/hspipy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-28 20:50:09.624641 HSPiPy-0.2/hspipy/src/
--rw-rw-rw-   0        0        0        0 2023-12-06 15:48:34.000000 HSPiPy-0.2/hspipy/src/__init__.py
--rw-rw-rw-   0        0        0     4563 2024-01-21 15:55:20.000000 HSPiPy-0.2/hspipy/src/hsp.py
--rw-rw-rw-   0        0        0       42 2024-01-28 20:50:09.632641 HSPiPy-0.2/setup.cfg
--rw-rw-rw-   0        0        0      976 2024-01-28 20:48:09.000000 HSPiPy-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 13:17:19.882645 hspipy-0.3/
+drwxrwxrwx   0        0        0        0 2024-05-26 13:17:19.878078 hspipy-0.3/HSPiPy.egg-info/
+-rw-rw-rw-   0        0        0     5592 2024-05-26 13:17:19.000000 hspipy-0.3/HSPiPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-26 13:17:19.000000 hspipy-0.3/HSPiPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 13:17:19.000000 hspipy-0.3/HSPiPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-26 13:17:19.000000 hspipy-0.3/HSPiPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 13:17:19.000000 hspipy-0.3/HSPiPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-12-06 15:48:34.000000 hspipy-0.3/LICENSE
+-rw-rw-rw-   0        0        0     5592 2024-05-26 13:17:19.879743 hspipy-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4858 2024-05-26 13:01:12.000000 hspipy-0.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-26 13:17:19.873251 hspipy-0.3/hspipy/
+-rw-rw-rw-   0        0        0       26 2023-12-31 12:01:36.000000 hspipy-0.3/hspipy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 13:17:19.875247 hspipy-0.3/hspipy/src/
+-rw-rw-rw-   0        0        0        0 2023-12-06 15:48:34.000000 hspipy-0.3/hspipy/src/__init__.py
+-rw-rw-rw-   0        0        0     4939 2024-05-03 16:49:36.000000 hspipy-0.3/hspipy/src/hsp.py
+-rw-rw-rw-   0        0        0       42 2024-05-26 13:17:19.882645 hspipy-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      919 2024-05-26 12:48:30.000000 hspipy-0.3/setup.py
```

### Comparing `HSPiPy-0.2/LICENSE` & `hspipy-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `HSPiPy-0.2/hspipy/src/hsp.py` & `hspipy-0.3/hspipy/src/hsp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import pandas as pd
 import numpy as np
 from hspcore import get_hsp, split_grid
 import matplotlib.pyplot as plt
 
-def WireframeSphere(centre=[0.,0.,0.], radius=1.,
-                    n_meridians=40, n_circles_latitude=None):
+
+def WireframeSphere(
+    centre=[0.0, 0.0, 0.0], radius=1.0, n_meridians=40, n_circles_latitude=None
+):
     """
     Create the arrays of values to plot the wireframe of a sphere.
 
     Parameters
     ----------
     centre: array like
         A point, defined as an iterable of three numerical values.
@@ -24,94 +26,116 @@
     Returns
     -------
     sphere_x, sphere_y, sphere_z: arrays
         The arrays with the coordinates of the points to make the wireframe.
         Their shape is (n_meridians, n_circles_latitude).
     """
     if n_circles_latitude is None:
-        n_circles_latitude = max(n_meridians/2, 4)
-    u, v = np.mgrid[0:2*np.pi:n_meridians*1j, 0:np.pi:n_circles_latitude*1j]
+        n_circles_latitude = max(n_meridians / 2, 4)
+    u, v = np.mgrid[
+        0 : 2 * np.pi : n_meridians * 1j, 0 : np.pi : n_circles_latitude * 1j
+    ]
     sphere_x = centre[0] + radius * np.cos(u) * np.sin(v)
     sphere_y = centre[1] + radius * np.sin(u) * np.sin(v)
     sphere_z = centre[2] + radius * np.cos(v)
     return sphere_x, sphere_y, sphere_z
 
+
 def get_solvent_points(grid):
-    x=[]
-    y=[]
-    z=[]
+    x = []
+    y = []
+    z = []
     for solvent, D, P, H, score in grid:
         x.append(H)
         y.append(D)
         z.append(P)
-    return x,y,z
+    return x, y, z
+
 
 class HSP:
-    def read(self,path):
+    def read(self, path):
         self.grid = pd.read_csv(path)
-    def get(self,inside_limit=1):
-        if hasattr(self, 'grid'):
-            hsp_grid = self.grid[['Solvent','D','P','H','Score']].to_numpy()
-            hsp,radius,error = get_hsp(hsp_grid,inside_limit)
-            inside,outside = split_grid(hsp_grid,inside_limit)
+
+    def get(self, inside_limit=1):
+        if hasattr(self, "grid"):
+            hsp_grid = self.grid[["Solvent", "D", "P", "H", "Score"]].to_numpy()
+            hsp, radius, error = get_hsp(hsp_grid, inside_limit)
+            inside, outside = split_grid(hsp_grid, inside_limit)
             self.d = hsp[0]
             self.p = hsp[1]
             self.h = hsp[2]
-            self.hsp=hsp
+            self.hsp = hsp
             self.radius = radius
             self.error = error
             self.inside = inside
             self.outside = outside
-            formatted_hsp = [ '%.2f' % elem for elem in hsp ]
-            print('HSP: ' + ', '.join(map(str, formatted_hsp)) + '\n'+
-                  'Radius: ' + str('%.3f' % radius)+'\n'+
-                  'error: ' + str('%.4f' % error))
+            formatted_hsp = ["%.2f" % elem for elem in hsp]
+            print(
+                "HSP: "
+                + ", ".join(map(str, formatted_hsp))
+                + "\n"
+                + "Radius: "
+                + str("%.3f" % radius)
+                + "\n"
+                + "error: "
+                + str("%.4f" % error)
+            )
             return
-        print('Your HSP has no grid, you can use the read function to import an HSP grid from a file')
+        print(
+            "Your HSP has no grid, you can use the read function to import an HSP grid from a file"
+        )
+
     def plot_3d(self):
         fig = plt.figure()
-        fig.suptitle('3D HSP Plot')
-        ax = plt.axes(projection='3d')
+        fig.suptitle("3D HSP Plot")
+        ax = plt.axes(projection="3d")
         ax.invert_yaxis()
-        ax.set_xlabel('H')
-        ax.set_ylabel('D')
-        ax.set_zlabel('P')
-        ax.zaxis.labelpad=-2 
-        
+        ax.set_xlabel("H")
+        ax.set_ylabel("D")
+        ax.set_zlabel("P")
+        ax.zaxis.labelpad = -2
+
         # draw sphere
-        x,y,z = WireframeSphere([self.h,self.d,self.p],self.radius)
-        #ax.contour3D(x, y, z, 50, cmap='binary')
+        x, y, z = WireframeSphere([self.h, self.d, self.p], self.radius)
+        # ax.contour3D(x, y, z, 50, cmap='binary')
         ax.plot_wireframe(x, y, z, color="g", linewidth=0.5)
         # draw a points
         ax.scatter([self.h], [self.d], [self.p], color="g", s=50)
-        good_x,good_y,good_z = get_solvent_points(self.inside)
+        good_x, good_y, good_z = get_solvent_points(self.inside)
         ax.scatter(good_x, good_y, good_z, color="b", s=50)
-        bad_x,bad_y,bad_z = get_solvent_points(self.outside)
+        bad_x, bad_y, bad_z = get_solvent_points(self.outside)
         ax.scatter(bad_x, bad_y, bad_z, color="r", s=50)
+
     def plot_2d(self):
-        fig, (ax1, ax2, ax3) = plt.subplots(ncols=3,figsize=(10,3))
-        fig.suptitle('2D HSP Subplots')
-        good_x,good_y,good_z = get_solvent_points(self.inside)
-        bad_x,bad_y,bad_z = get_solvent_points(self.outside)
-        
+        fig, (ax1, ax2, ax3) = plt.subplots(ncols=3, figsize=(12, 3.5))
+        fig.suptitle("2D HSP Subplots")
+        good_x, good_y, good_z = get_solvent_points(self.inside)
+        bad_x, bad_y, bad_z = get_solvent_points(self.outside)
+
         # P vs H
-        circle1 = plt.Circle((self.p, self.h), self.radius, color='g', fill = False)
+        circle1 = plt.Circle((self.p, self.h), self.radius, color="g", fill=False)
         ax1.scatter(good_z, good_x, color="b")
-        ax1.scatter(bad_z, bad_x,color="r")
-        ax1.scatter(self.p, self.h,color="g")
+        ax1.scatter(bad_z, bad_x, color="r")
+        ax1.scatter(self.p, self.h, color="g")
         ax1.add_patch(circle1)
+        ax1.set_xlabel("P")
+        ax1.set_ylabel("H")
         # H vs D
-        circle2 = plt.Circle((self.h,self.d), self.radius, color='g', fill = False)
+        circle2 = plt.Circle((self.h, self.d), self.radius, color="g", fill=False)
         ax2.scatter(good_z, good_x, color="b")
-        ax2.scatter(bad_z, bad_x,color="r")
-        ax2.scatter(self.h, self.d,color="g")
+        ax2.scatter(bad_z, bad_x, color="r")
+        ax2.scatter(self.h, self.d, color="g")
         ax2.add_patch(circle2)
+        ax2.set_xlabel("H")
+        ax2.set_ylabel("D")
         # P vs D
-        circle3 = plt.Circle((self.p,self.d), self.radius, color='g', fill = False)
+        circle3 = plt.Circle((self.p, self.d), self.radius, color="g", fill=False)
         ax3.scatter(good_z, good_x, color="b")
-        ax3.scatter(bad_z, bad_x,color="r")
-        ax3.scatter(self.p, self.d,color="g")
+        ax3.scatter(bad_z, bad_x, color="r")
+        ax3.scatter(self.p, self.d, color="g")
         ax3.add_patch(circle3)
+        ax3.set_xlabel("P")
+        ax3.set_ylabel("D")
+
     def plots(self):
         self.plot_3d()
         self.plot_2d()
-
```

### Comparing `HSPiPy-0.2/setup.py` & `hspipy-0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup
 
-# read the contents of your README file
-from pathlib import Path
-this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
+
+with open("README.rst", "r") as description:
+    long_description = description.read()
 
 setup(
     name="HSPiPy",
-    version="0.2",
-    author="Alejandro Gutierrez",
-    author_email="agutierrez@g-npd.com",
+    version="0.3",
+    license="MIT",
     description="Hansen Solubility Parameters in Python",
+    long_description_content_type="text/x-rst",
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    author="Alejandro Gutierrez",
+    author_email="agutierrez@g-npd.com",
     url="https://github.com/Gnpd/HSPiPy",
-    download_url="https://github.com/Gnpd/HSPiPy/archive/refs/tags/v_0.2.tar.gz",
+    download_url="https://github.com/Gnpd/HSPiPy/archive/refs/tags/v_0.3.tar.gz",
+    install_requires=["hspcore", "pandas", "matplotlib", "numpy"],
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.11',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.11",
     ],
-    install_requires=['hspcore','pandas','matplotlib','numpy'],
-    python_requires='>=3.6',
-)
+    python_requires=">=3.6",
+)
```

