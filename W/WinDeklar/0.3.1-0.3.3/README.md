# Comparing `tmp/windeklar-0.3.1.tar.gz` & `tmp/windeklar-0.3.3.tar.gz`

## Comparing `windeklar-0.3.1.tar` & `windeklar-0.3.3.tar`

### file list

```diff
@@ -1,31 +1,50 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.3.1/requirements.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.3.1/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.3.1/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.3.1/.idea/.name
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.3.1/.idea/WinDeklar.iml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.3.1/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.3.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.3.1/.idea/vcs.xml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.3.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.3.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/__init__.py
--rwxr-xr-x   0        0        0    17131 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/QTAux.py
--rw-r--r--   0        0        0    47364 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/WindowForm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/__init__.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/graph_aux.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/points_box.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/record.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/signal_aux.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/test_animation.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/test_pyqt.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/view_animation.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/view_animation.yaml
--rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/view_example.py
--rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/view_example.yaml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/view_simple_graph.py
--rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.3.1/src/WinDeklar/yaml_functions.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.3.1/LICENSE
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 windeklar-0.3.1/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 windeklar-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.3.3/requirements.txt
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 windeklar-0.3.3/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.3.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.3.3/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.3.3/.idea/.name
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.3.3/.idea/WinDeklar.iml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.3.3/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.3.3/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.3.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.3.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.3.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 windeklar-0.3.3/WinDeklar.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 windeklar-0.3.3/WinDeklar.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 windeklar-0.3.3/WinDeklar.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 windeklar-0.3.3/WinDeklar.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/__init__.py
+-rw-r--r--   0        0        0    17131 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0    47367 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/WinDeklar/view_simple_graph.py
+-rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.3.3/build/lib/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/__init__.py
+-rwxr-xr-x   0        0        0    17131 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/UploadProcedure.md
+-rw-r--r--   0        0        0    47367 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/view_animation.yaml
+-rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/view_example.yaml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/view_simple_graph.py
+-rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.3.3/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 windeklar-0.3.3/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 windeklar-0.3.3/PKG-INFO
```

### Comparing `windeklar-0.3.1/.github/workflows/python-publish.yml` & `windeklar-0.3.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/.idea/inspectionProfiles/Project_Default.xml` & `windeklar-0.3.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/src/WinDeklar/QTAux.py` & `windeklar-0.3.3/build/lib/src/WinDeklar/QTAux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/src/WinDeklar/WindowForm.py` & `windeklar-0.3.3/build/lib/src/WinDeklar/WindowForm.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,39 +19,40 @@
     Given the file path of the program that handle the form logic, loads and exec the corresponding WinForm
     :param form_file_path: most common value is __file__
     :param provider:       subclass of HostModel
     :param ext:            extension of the WinForm definition
     :return:
     """
     win_config_name = yaml.get_file_name_with_other_extension(form_file_path, ext)
-    ConfigurableWindow(win_config_name, provider)
+    win_config      = get_win_config(win_config_name)
+    ConfigurableWindow(win_config, provider)
 
 
 class ConfigurableWindow(QtWidgets.QMainWindow):
     """
     Defines a WinForm with many components inside in a declarative manner in a config file
     Notes:
         - a config_file_name is a yaml that has the definition (see view_example.yaml)
         - a typical windows has some widgets in the left and a Figure in the right (like a graph or a map)
     """
 
-    def __init__(self, config_file_name, provider):
+    def __init__(self, win_config, provider):
         """
         Init
-        :param config_file_name: name of the file containing the window definition
+        :param win_config: dict containing the window definition
         :param provider: handles all the form logic, usually a subclass of HostModel
         """
         super(ConfigurableWindow, self).__init__(parent=None)
 
         self.widgets   = []
         self.fig_views = []
         self.provider  = provider
         self.provider.set_main_window(self)
 
-        self.win_config = get_win_config(config_file_name)
+        self.win_config = win_config
 
         # status bar logic
         self.statusbar    = create_status_bar(self.win_config, self)
         self.progress_bar = GeneralProgressBar(widget=self.statusbar, stretch=1, visible=False)
 
         # menu bar
         menu_bar = create_menu_bar(self.win_config, self, self.provider)
```

### Comparing `windeklar-0.3.1/src/WinDeklar/graph_aux.py` & `windeklar-0.3.3/build/lib/src/WinDeklar/graph_aux.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,71 @@
 import numpy as np
 import random
 import math
 import matplotlib.lines as mlines
 
 
 class RealTimeDataProvider(object):
+    """
+    Base class used displaying data in an animated graph
+    """
+
     def __init__(self, dt=0.1, min_y=0.0, max_y=10.0, color='Red'):
+        """
+
+        :param dt:     delta time to increase in each cycle
+        :param min_y:  min value in the y-axis
+        :param max_y:  max value in the y-axis
+        :param color:  color of the line in the graph
+        """
+
         self.min_y = min_y
         self.max_y = max_y
         self.color = color
         self.dt    = dt
-        self.t     = 0.0
+        self.t     = 0.0     # current time
 
     def get_bounds(self):
         return self.min_y, self.max_y
 
     def get_min_y(self):
         return self.min_y
 
     def get_max_y(self):
         return self.max_y
 
     def get_next_values(self, i):
+        """
+        Returns the next point in the graph
+        :param i: number of iteration :type integer
+        :return:  next point (x, y)
+        """
         x      = self.t
         self.t += self.dt
         y      = i
         return x, y
 
 
 class RealTimeRandomDataProvider(RealTimeDataProvider):
     """
-    Returns a random number between min_y and max_y
+    Returns a random number between min_y and max_y each time
     """
+
     def __init__(self, dt=0.1, min_y=0.0, max_y=10.0, color='Red'):
         super(RealTimeRandomDataProvider, self).__init__(dt=dt, min_y=min_y, max_y=max_y, color=color)
 
     def get_next_values(self, i):
         x      = self.t
         self.t += self.dt
         return x, np.random.uniform(self.min_y, self.max_y)
 
 
 class RealTimeFunctionDataProvider(RealTimeDataProvider):
     """
-    Returns the result of applying a given function (function)
+    Returns the result of applying a given function
     """
 
     def __init__(self, dt=0.1, min_y=-1.2, max_y=1.2, function=np.sin, inc=np.radians(10), color='Red'):
         self.function = function
         self.inc      = inc
         self.last_r   = 0.0
         super(RealTimeFunctionDataProvider, self).__init__(dt=dt, min_y=min_y, max_y=max_y, color=color)
@@ -57,14 +75,17 @@
         self.t += self.dt
         y = self.function(self.last_r)
         self.last_r += self.inc
         return x, y
 
 
 class RealTimeConstantDataProvider(RealTimeDataProvider):
+    """
+    Returns a constant value every time (but can be changed with sef_reference)
+    """
     def __init__(self, dt=0.1, min_y=0.0, max_y=10.0, color='Black'):
         self.reference = 0.0
         super(RealTimeConstantDataProvider, self).__init__(dt=dt, min_y=min_y, max_y=max_y, color=color)
 
     def set_reference(self, new_reference):
         self.reference = new_reference
```

### Comparing `windeklar-0.3.1/src/WinDeklar/points_box.py` & `windeklar-0.3.3/build/lib/src/WinDeklar/points_box.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/src/WinDeklar/record.py` & `windeklar-0.3.3/build/lib/src/WinDeklar/record.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/src/WinDeklar/signal_aux.py` & `windeklar-0.3.3/build/lib/src/WinDeklar/signal_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/src/WinDeklar/test_animation.py` & `windeklar-0.3.3/build/lib/src/WinDeklar/test_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/src/WinDeklar/test_pyqt.py` & `windeklar-0.3.3/build/lib/src/WinDeklar/test_pyqt.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/src/WinDeklar/view_animation.py` & `windeklar-0.3.3/build/lib/src/WinDeklar/view_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/src/WinDeklar/view_animation.yaml` & `windeklar-0.3.3/src/WinDeklar/view_animation.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/src/WinDeklar/view_example.py` & `windeklar-0.3.3/build/lib/src/WinDeklar/view_example.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/src/WinDeklar/view_example.yaml` & `windeklar-0.3.3/src/WinDeklar/view_example.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/src/WinDeklar/view_simple_graph.py` & `windeklar-0.3.3/build/lib/src/WinDeklar/view_simple_graph.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/src/WinDeklar/yaml_functions.py` & `windeklar-0.3.3/build/lib/src/WinDeklar/yaml_functions.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/LICENSE` & `windeklar-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/README.md` & `windeklar-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `windeklar-0.3.1/pyproject.toml` & `windeklar-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name    = "WinDeklar"
-version = "0.3.1"
+version = "0.3.3"
 authors = [
   { name="Nicolas Jodal", email="jnj@genexus.com" },
 ]
 description = "Create winforms in an easy, declarative way. Specially suited for Robotics applications"
 readme      = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `windeklar-0.3.1/PKG-INFO` & `windeklar-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: WinDeklar
-Version: 0.3.1
+Version: 0.3.3
 Summary: Create winforms in an easy, declarative way. Specially suited for Robotics applications
 Project-URL: Homepage, https://github.com/njodal/WinDeklar
 Project-URL: Bug Tracker, https://github.com/njodal/WinDeklar/issues
 Author-email: Nicolas Jodal <jnj@genexus.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

