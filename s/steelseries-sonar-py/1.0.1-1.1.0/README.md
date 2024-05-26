# Comparing `tmp/steelseries-sonar-py-1.0.1.tar.gz` & `tmp/steelseries_sonar_py-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steelseries-sonar-py-1.0.1.tar", last modified: Wed Jan  3 16:07:19 2024, max compression
+gzip compressed data, was "steelseries_sonar_py-1.1.0.tar", last modified: Sun May 26 10:57:20 2024, max compression
```

## Comparing `steelseries-sonar-py-1.0.1.tar` & `steelseries_sonar_py-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 16:07:19.347101 steelseries-sonar-py-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 16:07:19.343101 steelseries-sonar-py-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 16:07:19.343101 steelseries-sonar-py-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-01-03 16:07:09.000000 steelseries-sonar-py-1.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-01-03 16:07:09.000000 steelseries-sonar-py-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-03 16:07:09.000000 steelseries-sonar-py-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-01-03 16:07:19.347101 steelseries-sonar-py-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-01-03 16:07:09.000000 steelseries-sonar-py-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-03 16:07:09.000000 steelseries-sonar-py-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-03 16:07:19.347101 steelseries-sonar-py-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-01-03 16:07:09.000000 steelseries-sonar-py-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 16:07:19.343101 steelseries-sonar-py-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 16:07:19.347101 steelseries-sonar-py-1.0.1/src/steelseries_sonar_py/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-03 16:07:09.000000 steelseries-sonar-py-1.0.1/src/steelseries_sonar_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-01-03 16:07:09.000000 steelseries-sonar-py-1.0.1/src/steelseries_sonar_py/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-01-03 16:07:09.000000 steelseries-sonar-py-1.0.1/src/steelseries_sonar_py/sonar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 16:07:19.347101 steelseries-sonar-py-1.0.1/src/steelseries_sonar_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-01-03 16:07:19.000000 steelseries-sonar-py-1.0.1/src/steelseries_sonar_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-03 16:07:19.000000 steelseries-sonar-py-1.0.1/src/steelseries_sonar_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 16:07:19.000000 steelseries-sonar-py-1.0.1/src/steelseries_sonar_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-03 16:07:19.000000 steelseries-sonar-py-1.0.1/src/steelseries_sonar_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-03 16:07:19.000000 steelseries-sonar-py-1.0.1/src/steelseries_sonar_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-03 16:07:09.000000 steelseries-sonar-py-1.0.1/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:57:20.608956 steelseries_sonar_py-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:57:20.604956 steelseries_sonar_py-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:57:20.604956 steelseries_sonar_py-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-26 10:57:13.000000 steelseries_sonar_py-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-26 10:57:13.000000 steelseries_sonar_py-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-26 10:57:13.000000 steelseries_sonar_py-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-26 10:57:20.604956 steelseries_sonar_py-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-26 10:57:13.000000 steelseries_sonar_py-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-26 10:57:13.000000 steelseries_sonar_py-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 10:57:20.608956 steelseries_sonar_py-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-26 10:57:13.000000 steelseries_sonar_py-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:57:20.604956 steelseries_sonar_py-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:57:20.604956 steelseries_sonar_py-1.1.0/src/steelseries_sonar_py/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 10:57:13.000000 steelseries_sonar_py-1.1.0/src/steelseries_sonar_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-26 10:57:13.000000 steelseries_sonar_py-1.1.0/src/steelseries_sonar_py/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-26 10:57:13.000000 steelseries_sonar_py-1.1.0/src/steelseries_sonar_py/sonar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:57:20.604956 steelseries_sonar_py-1.1.0/src/steelseries_sonar_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-26 10:57:20.000000 steelseries_sonar_py-1.1.0/src/steelseries_sonar_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-26 10:57:20.000000 steelseries_sonar_py-1.1.0/src/steelseries_sonar_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 10:57:20.000000 steelseries_sonar_py-1.1.0/src/steelseries_sonar_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-26 10:57:20.000000 steelseries_sonar_py-1.1.0/src/steelseries_sonar_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 10:57:20.000000 steelseries_sonar_py-1.1.0/src/steelseries_sonar_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-26 10:57:13.000000 steelseries_sonar_py-1.1.0/test.py
```

### Comparing `steelseries-sonar-py-1.0.1/.github/workflows/publish.yml` & `steelseries_sonar_py-1.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `steelseries-sonar-py-1.0.1/.gitignore` & `steelseries_sonar_py-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `steelseries-sonar-py-1.0.1/LICENSE` & `steelseries_sonar_py-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `steelseries-sonar-py-1.0.1/PKG-INFO` & `steelseries_sonar_py-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steelseries-sonar-py
-Version: 1.0.1
+Version: 1.1.0
 Summary: Simple Python wrapper for the SteelSeries Sonar API
 Home-page: https://github.com/Mark7888/steelseries-sonar-py
 Author: Mark7888
 Author-email: l.mark7888@gmail.com
 Project-URL: Documentation, https://github.com/Mark7888/steelseries-sonar-py/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/Mark7888/steelseries-sonar-py/issues
 Project-URL: Source Code, https://github.com/Mark7888/steelseries-sonar-py
@@ -29,21 +29,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
+[![publish](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml/badge.svg?event=push)](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml)
+[![Downloads](https://static.pepy.tech/badge/steelseries-sonar-py)](https://pepy.tech/project/steelseries-sonar-py)
+
 # SteelSeries Sonar Python API
-[![publish](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml/badge.svg)](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml)
 
 ## Overview
 
-This Python package provides a convenient interface for interacting with the [SteelSeries Sonar](https://steelseries.com/gg/sonar) application API. The Sonar application allows users to control and display volumes for various audio channels.
-You can check the project [PyPI site](https://pypi.org/project/steelseries-sonar-py/) here!
+This Python package provides a convenient interface for interacting with the SteelSeries Sonar application API. The Sonar application allows users to control and display volumes for various audio channels.
 
 ## Installation
 
 To use this package, follow these steps:
 
 1. Install the package using pip:
 
@@ -92,20 +93,29 @@
 
 ### Muting/Unmuting a Channel
 
 Toggle mute status for a specific channel. The `channel` parameter should be one of the following: `master`, `game`, `chatRender`, `media`, `aux`, `chatCapture`. The `muted` parameter should be a boolean indicating whether to mute (`True`) or unmute (`False`) the channel:
 
 ```python
 channel = "game"
-muted = `True`
+muted = True
 
 result = sonar.mute_channel(channel, muted)
 print(result)
 ```
 
+### Chatmix
+
+Chatmix value between `-1 and 1` to focus sound from the `game` or `chatRender` channel:
+
+```python
+result = sonar.chat_mix(0.5)
+print(result)
+```
+
 ## Exceptions
 
 The package introduces a set of exceptions that might be raised during usage. It is advisable to handle these exceptions accordingly in your code. You can import them from `steelseries_sonar_py.exceptions`. Here is the list of potential exceptions:
 
 - `EnginePathNotFoundError`: Raised when SteelSeries Engine 3 is not installed or not in the default location.
 - `ServerNotAccessibleError`: Raised when the SteelSeries server is not accessible. Provides the HTTP status code.
 - `SonarNotEnabledError`: Raised when SteelSeries Sonar is not enabled.
@@ -138,11 +148,15 @@
 channel = "master"
 volume = 0.8
 result = sonar.set_volume(channel, volume)
 print(f"Set volume for {channel}:", result)
 
 # Mute the 'game' channel
 channel = "game"
-muted = `True`
+muted = True
 result = sonar.mute_channel(channel, muted)
 print(f"Mute {channel}:", result)
 ```
+
+## Special Thanks
+
+Thanks to two contributors who made this package possible - [wex](https://github.com/wex/sonar-rev) for figuring out the API and [TotalPanther317](https://github.com/TotalPanther317/steelseries-sonar-py) for understanding streamer mode. Grateful for their efforts!
```

### Comparing `steelseries-sonar-py-1.0.1/README.md` & `steelseries_sonar_py-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+[![publish](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml/badge.svg?event=push)](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml)
+[![Downloads](https://static.pepy.tech/badge/steelseries-sonar-py)](https://pepy.tech/project/steelseries-sonar-py)
+
 # SteelSeries Sonar Python API
-[![publish](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml/badge.svg)](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml)
 
 ## Overview
 
-This Python package provides a convenient interface for interacting with the [SteelSeries Sonar](https://steelseries.com/gg/sonar) application API. The Sonar application allows users to control and display volumes for various audio channels.
-You can check the project [PyPI site](https://pypi.org/project/steelseries-sonar-py/) here!
+This Python package provides a convenient interface for interacting with the SteelSeries Sonar application API. The Sonar application allows users to control and display volumes for various audio channels.
 
 ## Installation
 
 To use this package, follow these steps:
 
 1. Install the package using pip:
 
@@ -57,20 +58,29 @@
 
 ### Muting/Unmuting a Channel
 
 Toggle mute status for a specific channel. The `channel` parameter should be one of the following: `master`, `game`, `chatRender`, `media`, `aux`, `chatCapture`. The `muted` parameter should be a boolean indicating whether to mute (`True`) or unmute (`False`) the channel:
 
 ```python
 channel = "game"
-muted = `True`
+muted = True
 
 result = sonar.mute_channel(channel, muted)
 print(result)
 ```
 
+### Chatmix
+
+Chatmix value between `-1 and 1` to focus sound from the `game` or `chatRender` channel:
+
+```python
+result = sonar.chat_mix(0.5)
+print(result)
+```
+
 ## Exceptions
 
 The package introduces a set of exceptions that might be raised during usage. It is advisable to handle these exceptions accordingly in your code. You can import them from `steelseries_sonar_py.exceptions`. Here is the list of potential exceptions:
 
 - `EnginePathNotFoundError`: Raised when SteelSeries Engine 3 is not installed or not in the default location.
 - `ServerNotAccessibleError`: Raised when the SteelSeries server is not accessible. Provides the HTTP status code.
 - `SonarNotEnabledError`: Raised when SteelSeries Sonar is not enabled.
@@ -103,11 +113,15 @@
 channel = "master"
 volume = 0.8
 result = sonar.set_volume(channel, volume)
 print(f"Set volume for {channel}:", result)
 
 # Mute the 'game' channel
 channel = "game"
-muted = `True`
+muted = True
 result = sonar.mute_channel(channel, muted)
 print(f"Mute {channel}:", result)
 ```
+
+## Special Thanks
+
+Thanks to two contributors who made this package possible - [wex](https://github.com/wex/sonar-rev) for figuring out the API and [TotalPanther317](https://github.com/TotalPanther317/steelseries-sonar-py) for understanding streamer mode. Grateful for their efforts!
```

### Comparing `steelseries-sonar-py-1.0.1/setup.py` & `steelseries_sonar_py-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `steelseries-sonar-py-1.0.1/src/steelseries_sonar_py/exceptions.py` & `steelseries_sonar_py-1.1.0/src/steelseries_sonar_py/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,7 +41,14 @@
 
 class InvalidVolumeError(Exception):
     def __init__(self, volume):
         self.volume = volume
 
     def __str__(self):
         return f"Invalid volume '{self.volume}'! Value must be between 0 and 1!"
+
+class InvalidMixVolumeError(Exception):
+    def __init__(self, mix_volume):
+        self.mix_volume = mix_volume
+
+    def __str__(self):
+        return f"Invalid mix volume '{self.mix_volume}'! Value must be between -1 and 1!"
```

### Comparing `steelseries-sonar-py-1.0.1/src/steelseries_sonar_py/sonar.py` & `steelseries_sonar_py-1.1.0/src/steelseries_sonar_py/sonar.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,7 +86,17 @@
 
         muted = muted == True
 
         url = f"{self.web_server_address}{self.volume_path}/{channel}/Mute/{json.dumps(muted)}"
         mute_data = requests.put(url)
 
         return json.loads(mute_data.text)
+
+    def chat_mix(self, mix_volume):
+        if mix_volume < -1 or mix_volume > 1:
+            raise ex.InvalidMixVolumeError(mix_volume)
+        
+        url = f"{self.web_server_address}/chatMix?balance={json.dumps(mix_volume)}"
+        print(url)
+        volume_data = requests.put(url)
+
+        return json.loads(volume_data.text)
```

### Comparing `steelseries-sonar-py-1.0.1/src/steelseries_sonar_py.egg-info/PKG-INFO` & `steelseries_sonar_py-1.1.0/src/steelseries_sonar_py.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steelseries-sonar-py
-Version: 1.0.1
+Version: 1.1.0
 Summary: Simple Python wrapper for the SteelSeries Sonar API
 Home-page: https://github.com/Mark7888/steelseries-sonar-py
 Author: Mark7888
 Author-email: l.mark7888@gmail.com
 Project-URL: Documentation, https://github.com/Mark7888/steelseries-sonar-py/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/Mark7888/steelseries-sonar-py/issues
 Project-URL: Source Code, https://github.com/Mark7888/steelseries-sonar-py
@@ -29,21 +29,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
+[![publish](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml/badge.svg?event=push)](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml)
+[![Downloads](https://static.pepy.tech/badge/steelseries-sonar-py)](https://pepy.tech/project/steelseries-sonar-py)
+
 # SteelSeries Sonar Python API
-[![publish](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml/badge.svg)](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml)
 
 ## Overview
 
-This Python package provides a convenient interface for interacting with the [SteelSeries Sonar](https://steelseries.com/gg/sonar) application API. The Sonar application allows users to control and display volumes for various audio channels.
-You can check the project [PyPI site](https://pypi.org/project/steelseries-sonar-py/) here!
+This Python package provides a convenient interface for interacting with the SteelSeries Sonar application API. The Sonar application allows users to control and display volumes for various audio channels.
 
 ## Installation
 
 To use this package, follow these steps:
 
 1. Install the package using pip:
 
@@ -92,20 +93,29 @@
 
 ### Muting/Unmuting a Channel
 
 Toggle mute status for a specific channel. The `channel` parameter should be one of the following: `master`, `game`, `chatRender`, `media`, `aux`, `chatCapture`. The `muted` parameter should be a boolean indicating whether to mute (`True`) or unmute (`False`) the channel:
 
 ```python
 channel = "game"
-muted = `True`
+muted = True
 
 result = sonar.mute_channel(channel, muted)
 print(result)
 ```
 
+### Chatmix
+
+Chatmix value between `-1 and 1` to focus sound from the `game` or `chatRender` channel:
+
+```python
+result = sonar.chat_mix(0.5)
+print(result)
+```
+
 ## Exceptions
 
 The package introduces a set of exceptions that might be raised during usage. It is advisable to handle these exceptions accordingly in your code. You can import them from `steelseries_sonar_py.exceptions`. Here is the list of potential exceptions:
 
 - `EnginePathNotFoundError`: Raised when SteelSeries Engine 3 is not installed or not in the default location.
 - `ServerNotAccessibleError`: Raised when the SteelSeries server is not accessible. Provides the HTTP status code.
 - `SonarNotEnabledError`: Raised when SteelSeries Sonar is not enabled.
@@ -138,11 +148,15 @@
 channel = "master"
 volume = 0.8
 result = sonar.set_volume(channel, volume)
 print(f"Set volume for {channel}:", result)
 
 # Mute the 'game' channel
 channel = "game"
-muted = `True`
+muted = True
 result = sonar.mute_channel(channel, muted)
 print(f"Mute {channel}:", result)
 ```
+
+## Special Thanks
+
+Thanks to two contributors who made this package possible - [wex](https://github.com/wex/sonar-rev) for figuring out the API and [TotalPanther317](https://github.com/TotalPanther317/steelseries-sonar-py) for understanding streamer mode. Grateful for their efforts!
```

