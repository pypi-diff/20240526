# Comparing `tmp/brianmechanisms-0.1.4.tar.gz` & `tmp/brianmechanisms-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brianmechanisms-0.1.4.tar", last modified: Sun May 26 09:41:19 2024, max compression
+gzip compressed data, was "brianmechanisms-0.1.5.tar", last modified: Sun May 26 16:03:09 2024, max compression
```

## Comparing `brianmechanisms-0.1.4.tar` & `brianmechanisms-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:41:19.347919 brianmechanisms-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-05-26 09:41:19.347919 brianmechanisms-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 09:41:19.347919 brianmechanisms-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:41:19.343919 brianmechanisms-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:41:19.347919 brianmechanisms-0.1.4/src/brianmechanisms/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/src/brianmechanisms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/src/brianmechanisms/appproximateStraightLineMechanisms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/src/brianmechanisms/locii.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/src/brianmechanisms/mirror.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/src/brianmechanisms/straightLineMechanisms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:41:19.347919 brianmechanisms-0.1.4/src/brianmechanisms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-05-26 09:41:19.000000 brianmechanisms-0.1.4/src/brianmechanisms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-26 09:41:19.000000 brianmechanisms-0.1.4/src/brianmechanisms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 09:41:19.000000 brianmechanisms-0.1.4/src/brianmechanisms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-26 09:41:19.000000 brianmechanisms-0.1.4/src/brianmechanisms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 09:41:19.000000 brianmechanisms-0.1.4/src/brianmechanisms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:03:09.144506 brianmechanisms-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-05-26 16:02:55.000000 brianmechanisms-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-26 16:03:09.144506 brianmechanisms-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-05-26 16:02:55.000000 brianmechanisms-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-26 16:02:55.000000 brianmechanisms-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 16:03:09.144506 brianmechanisms-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:03:09.140506 brianmechanisms-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:03:09.140506 brianmechanisms-0.1.5/src/brianmechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-26 16:02:55.000000 brianmechanisms-0.1.5/src/brianmechanisms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-05-26 16:02:55.000000 brianmechanisms-0.1.5/src/brianmechanisms/appproximateStraightLineMechanisms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-26 16:02:55.000000 brianmechanisms-0.1.5/src/brianmechanisms/locii.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-26 16:02:55.000000 brianmechanisms-0.1.5/src/brianmechanisms/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-26 16:02:55.000000 brianmechanisms-0.1.5/src/brianmechanisms/straightLineMechanisms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:03:09.144506 brianmechanisms-0.1.5/src/brianmechanisms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-26 16:03:09.000000 brianmechanisms-0.1.5/src/brianmechanisms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-26 16:03:09.000000 brianmechanisms-0.1.5/src/brianmechanisms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 16:03:09.000000 brianmechanisms-0.1.5/src/brianmechanisms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-26 16:03:09.000000 brianmechanisms-0.1.5/src/brianmechanisms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 16:03:09.000000 brianmechanisms-0.1.5/src/brianmechanisms.egg-info/top_level.txt
```

### Comparing `brianmechanisms-0.1.4/LICENSE` & `brianmechanisms-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.4/PKG-INFO` & `brianmechanisms-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brianmechanisms
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python module for designing mechanisms and robots
 Home-page: https://brianmechanisms.github.io
 Author: Brian Onang'o
 Author-email: surgbc@gmail.com
 Project-URL: Homepage, https://github.com/brianmechanisms/brianmechanisms-designer
 Project-URL: Issues, https://github.com/brianmechanisms/brianmechanisms-designer/issues
 Classifier: Programming Language :: Python :: 3
@@ -150,7 +150,22 @@
 
 -`ax`: Specifies the Matplotlib axes object to use for plotting. If not provided, a new axes object will be created.
 - `fig`: Specifies the Matplotlib figure object to use for the plot. This allows you to add the plot to an existing figure.
 - `legend`: A boolean flag that controls whether a legend should be displayed on the plot. If set to False, no legend will be shown.
 - `axes`: A boolean flag that controls whether the axes should be displayed on the plot. If set to False, the axes will be hidden.
 - `mechanism_theta`: Specifies the angle (in degrees) at which the mechanism should be drawn. This setting allows you to visualize the mechanism at a specific angle.
 - `ani`: A boolean flag that indicates whether the plot should be animated. If set to True, the animation will be enabled.
+
+
+## Hypocycloids
+
+![Tusi Couple](examples/TusiCouple.gif)
+
+![Tusi Couple](examples/TusiCouple.gif)
+
+![Hypocycloids](examples/hypocycloids.png)
+
+![Hypoctrochoids](examples/hypotrochoids.png)
+
+![Epictrochoids](examples/epitrochoids.png)
+
+
```

### Comparing `brianmechanisms-0.1.4/README.md` & `brianmechanisms-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -130,8 +130,23 @@
 The `plotConfig` dictionary allows you to customize various aspects of your plot and animation. Here are the key settings you can use:
 
 -`ax`: Specifies the Matplotlib axes object to use for plotting. If not provided, a new axes object will be created.
 - `fig`: Specifies the Matplotlib figure object to use for the plot. This allows you to add the plot to an existing figure.
 - `legend`: A boolean flag that controls whether a legend should be displayed on the plot. If set to False, no legend will be shown.
 - `axes`: A boolean flag that controls whether the axes should be displayed on the plot. If set to False, the axes will be hidden.
 - `mechanism_theta`: Specifies the angle (in degrees) at which the mechanism should be drawn. This setting allows you to visualize the mechanism at a specific angle.
-- `ani`: A boolean flag that indicates whether the plot should be animated. If set to True, the animation will be enabled.
+- `ani`: A boolean flag that indicates whether the plot should be animated. If set to True, the animation will be enabled.
+
+
+## Hypocycloids
+
+![Tusi Couple](examples/TusiCouple.gif)
+
+![Tusi Couple](examples/TusiCouple.gif)
+
+![Hypocycloids](examples/hypocycloids.png)
+
+![Hypoctrochoids](examples/hypotrochoids.png)
+
+![Epictrochoids](examples/epitrochoids.png)
+
+
```

### Comparing `brianmechanisms-0.1.4/src/brianmechanisms/appproximateStraightLineMechanisms.py` & `brianmechanisms-0.1.5/src/brianmechanisms/appproximateStraightLineMechanisms.py`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.4/src/brianmechanisms/locii.py` & `brianmechanisms-0.1.5/src/brianmechanisms/locii.py`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.4/src/brianmechanisms.egg-info/PKG-INFO` & `brianmechanisms-0.1.5/src/brianmechanisms.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brianmechanisms
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python module for designing mechanisms and robots
 Home-page: https://brianmechanisms.github.io
 Author: Brian Onang'o
 Author-email: surgbc@gmail.com
 Project-URL: Homepage, https://github.com/brianmechanisms/brianmechanisms-designer
 Project-URL: Issues, https://github.com/brianmechanisms/brianmechanisms-designer/issues
 Classifier: Programming Language :: Python :: 3
@@ -150,7 +150,22 @@
 
 -`ax`: Specifies the Matplotlib axes object to use for plotting. If not provided, a new axes object will be created.
 - `fig`: Specifies the Matplotlib figure object to use for the plot. This allows you to add the plot to an existing figure.
 - `legend`: A boolean flag that controls whether a legend should be displayed on the plot. If set to False, no legend will be shown.
 - `axes`: A boolean flag that controls whether the axes should be displayed on the plot. If set to False, the axes will be hidden.
 - `mechanism_theta`: Specifies the angle (in degrees) at which the mechanism should be drawn. This setting allows you to visualize the mechanism at a specific angle.
 - `ani`: A boolean flag that indicates whether the plot should be animated. If set to True, the animation will be enabled.
+
+
+## Hypocycloids
+
+![Tusi Couple](examples/TusiCouple.gif)
+
+![Tusi Couple](examples/TusiCouple.gif)
+
+![Hypocycloids](examples/hypocycloids.png)
+
+![Hypoctrochoids](examples/hypotrochoids.png)
+
+![Epictrochoids](examples/epitrochoids.png)
+
+
```

