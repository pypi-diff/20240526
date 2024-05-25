# Comparing `tmp/gdpc-7.1.0.tar.gz` & `tmp/gdpc-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdpc-7.1.0.tar", last modified: Fri Apr 19 20:44:48 2024, max compression
+gzip compressed data, was "gdpc-7.2.0.tar", last modified: Sat May 25 22:18:37 2024, max compression
```

## Comparing `gdpc-7.1.0.tar` & `gdpc-7.2.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-04-19 20:44:48.611605 gdpc-7.1.0/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1157 2024-03-25 17:37:02.000000 gdpc-7.1.0/LICENSE
--rw-r--r--   0 arthur    (1000) arthur    (1000)     8890 2024-04-19 20:44:48.611605 gdpc-7.1.0/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     7087 2024-03-25 17:37:02.000000 gdpc-7.1.0/README.md
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-04-19 20:44:48.607605 gdpc-7.1.0/gdpc/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1138 2024-04-19 20:39:32.000000 gdpc-7.1.0/gdpc/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4478 2023-03-24 01:05:49.000000 gdpc-7.1.0/gdpc/block.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     7343 2023-02-01 16:21:53.000000 gdpc-7.1.0/gdpc/block_state_tools.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    24845 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/editor.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     6164 2024-03-25 17:37:02.000000 gdpc-7.1.0/gdpc/editor_tools.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      505 2023-02-01 00:45:52.000000 gdpc-7.1.0/gdpc/exceptions.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     9321 2023-03-24 01:05:49.000000 gdpc-7.1.0/gdpc/geometry.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    13828 2024-04-19 20:36:27.000000 gdpc-7.1.0/gdpc/interface.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)   121425 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/lookup.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     9748 2024-03-25 17:37:02.000000 gdpc-7.1.0/gdpc/minecraft_tools.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2575 2023-03-24 01:05:49.000000 gdpc-7.1.0/gdpc/model.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2042 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/nbt_tools.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     7814 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/transform.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4536 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/utils.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    48614 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/vector_tools.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    14199 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/world_slice.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-04-19 20:44:48.611605 gdpc-7.1.0/gdpc.egg-info/
--rw-r--r--   0 arthur    (1000) arthur    (1000)     8890 2024-04-19 20:44:48.000000 gdpc-7.1.0/gdpc.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      498 2024-04-19 20:44:48.000000 gdpc-7.1.0/gdpc.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2024-04-19 20:44:48.000000 gdpc-7.1.0/gdpc.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-02-27 18:17:38.000000 gdpc-7.1.0/gdpc.egg-info/not-zip-safe
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      140 2024-04-19 20:44:48.000000 gdpc-7.1.0/gdpc.egg-info/requires.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        5 2024-04-19 20:44:48.000000 gdpc-7.1.0/gdpc.egg-info/top_level.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      104 2022-09-29 15:44:28.000000 gdpc-7.1.0/pyproject.toml
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2024-04-19 20:44:48.611605 gdpc-7.1.0/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2869 2024-03-22 21:29:37.000000 gdpc-7.1.0/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-25 22:18:37.414239 gdpc-7.2.0/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1157 2024-04-30 17:00:22.000000 gdpc-7.2.0/LICENSE
+-rw-r--r--   0 arthur    (1000) arthur    (1000)     8881 2024-05-25 22:18:37.414239 gdpc-7.2.0/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     7083 2024-05-25 20:15:19.000000 gdpc-7.2.0/README.md
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      104 2022-09-24 23:42:54.000000 gdpc-7.2.0/pyproject.toml
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2024-05-25 22:18:37.414239 gdpc-7.2.0/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2985 2024-05-25 20:15:19.000000 gdpc-7.2.0/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-25 22:18:37.410239 gdpc-7.2.0/src/
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-25 22:18:37.414239 gdpc-7.2.0/src/gdpc/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1138 2024-05-25 22:14:00.000000 gdpc-7.2.0/src/gdpc/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4478 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/block.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     7343 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/block_state_tools.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    24845 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/editor.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     6164 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/editor_tools.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      505 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/exceptions.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     9321 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/geometry.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    13828 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/interface.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)   121425 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/lookup.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     9748 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/minecraft_tools.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2575 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/model.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2042 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/nbt_tools.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     7814 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/transform.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4536 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/utils.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    54468 2024-05-25 22:01:31.000000 gdpc-7.2.0/src/gdpc/vector_tools.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    14199 2024-05-25 20:15:19.000000 gdpc-7.2.0/src/gdpc/world_slice.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-25 22:18:37.414239 gdpc-7.2.0/src/gdpc.egg-info/
+-rw-r--r--   0 arthur    (1000) arthur    (1000)     8881 2024-05-25 22:18:37.000000 gdpc-7.2.0/src/gdpc.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      586 2024-05-25 22:18:37.000000 gdpc-7.2.0/src/gdpc.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2024-05-25 22:18:37.000000 gdpc-7.2.0/src/gdpc.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2024-04-30 17:05:59.000000 gdpc-7.2.0/src/gdpc.egg-info/not-zip-safe
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      140 2024-05-25 22:18:37.000000 gdpc-7.2.0/src/gdpc.egg-info/requires.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        5 2024-05-25 22:18:37.000000 gdpc-7.2.0/src/gdpc.egg-info/top_level.txt
```

### Comparing `gdpc-7.1.0/LICENSE` & `gdpc-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/PKG-INFO` & `gdpc-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: gdpc
-Version: 7.1.0
+Version: 7.2.0
 Summary: The Generative Design Python Client (GDPC) is a Python-based interface for the Minecraft GDMC HTTP Interface mod.\nIt was created for use in the Generative Design in Minecraft Competition (GDMC).
 Home-page: https://github.com/avdstaaij/gdpc
 Author: Arthur van der Staaij, Blinkenlights, Nils Gawlik
 Author-email: arthurvanderstaaij@gmail.com, blinkenlights@pm.me, nilsgawlik@gmx.de
 Maintainer: Arthur van der Staaij
 Maintainer-email: arthurvanderstaaij@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/avdstaaij/gdpc/issues
 Project-URL: Changelog, https://github.com/avdstaaij/gdpc/blob/master/CHANGELOG.md
-Project-URL: Official Competition Website, https://gendesignmc.engineering.nyu.edu
+Project-URL: Official Competition wiki, https://gendesignmc.wikidot.com/start
 Project-URL: Chat about it on Discord, https://discord.gg/YwpPCRQWND
 Project-URL: Source, https://github.com/avdstaaij/gdpc
 Keywords: GDMC,generative design,Minecraft,HTTP,development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -37,15 +37,15 @@
 Requires-Dist: scipy
 Requires-Dist: termcolor
 Requires-Dist: typing_extensions
 
 # GDPC
 
 GDPC (Generative Design Python Client) is a Python framework for use in conjunction with the [GDMC-HTTP](https://github.com/Niels-NTG/gdmc_http_interface) mod for Minecraft Java edition.
-It is designed for the [Generative Design in Minecraft Competition (GDMC)](https://gendesignmc.engineering.nyu.edu).
+It is designed for the [Generative Design in Minecraft Competition (GDMC)](https://gendesignmc.wikidot.com/start).
 
 You need to be playing in a Minecraft world with the mod installed to use the framework.
 
 The latest version of GDPC is compatible with GDMC-HTTP versions **>=1.0.0, <2.0.0** and Minecraft **1.20.2** (see [note](#note-on-supported-minecraft-version)).
 
 
 ## Quick example
@@ -65,15 +65,15 @@
 geometry.placeCuboid(editor, (0,80,2), (2,82,4), Block("oak_planks"))
 ```
 
 ## What's the difference between GDMC, GDMC-HTTP and GDPC?
 
 These abbreviations are all very similar, but refer to different things.
 
-**GDMC:** Short for the [Generative Design in Minecraft Competition](https://gendesignmc.engineering.nyu.edu), a yearly competition for generative AI systems in Minecraft.
+**GDMC:** Short for the [Generative Design in Minecraft Competition](https://gendesignmc.wikidot.com/start), a yearly competition for generative AI systems in Minecraft.
 The challenge is to write an algorithm that creates a settlement while adapting to the pre-existing terrain. The competition also has a [Discord server](https://discord.gg/YwpPCRQWND).
 
 **GDMC-HTTP:** A [Minecraft Forge mod](https://github.com/Niels-NTG/gdmc_http_interface) that provides a HTTP interface to edit the world.
 It allows you to modify the world live, while you're playing in it. This makes it possible to iterate quickly on generator algorithms.
 The mod is an official submission method for the competition.
 
 **GDPC:** This repository (notice the "P"). A Python framework for interacting with the GDMC-HTTP interface.
```

### Comparing `gdpc-7.1.0/README.md` & `gdpc-7.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # GDPC
 
 GDPC (Generative Design Python Client) is a Python framework for use in conjunction with the [GDMC-HTTP](https://github.com/Niels-NTG/gdmc_http_interface) mod for Minecraft Java edition.
-It is designed for the [Generative Design in Minecraft Competition (GDMC)](https://gendesignmc.engineering.nyu.edu).
+It is designed for the [Generative Design in Minecraft Competition (GDMC)](https://gendesignmc.wikidot.com/start).
 
 You need to be playing in a Minecraft world with the mod installed to use the framework.
 
 The latest version of GDPC is compatible with GDMC-HTTP versions **>=1.0.0, <2.0.0** and Minecraft **1.20.2** (see [note](#note-on-supported-minecraft-version)).
 
 
 ## Quick example
@@ -25,15 +25,15 @@
 geometry.placeCuboid(editor, (0,80,2), (2,82,4), Block("oak_planks"))
 ```
 
 ## What's the difference between GDMC, GDMC-HTTP and GDPC?
 
 These abbreviations are all very similar, but refer to different things.
 
-**GDMC:** Short for the [Generative Design in Minecraft Competition](https://gendesignmc.engineering.nyu.edu), a yearly competition for generative AI systems in Minecraft.
+**GDMC:** Short for the [Generative Design in Minecraft Competition](https://gendesignmc.wikidot.com/start), a yearly competition for generative AI systems in Minecraft.
 The challenge is to write an algorithm that creates a settlement while adapting to the pre-existing terrain. The competition also has a [Discord server](https://discord.gg/YwpPCRQWND).
 
 **GDMC-HTTP:** A [Minecraft Forge mod](https://github.com/Niels-NTG/gdmc_http_interface) that provides a HTTP interface to edit the world.
 It allows you to modify the world live, while you're playing in it. This makes it possible to iterate quickly on generator algorithms.
 The mod is an official submission method for the competition.
 
 **GDPC:** This repository (notice the "P"). A Python framework for interacting with the GDMC-HTTP interface.
```

### Comparing `gdpc-7.1.0/gdpc/__init__.py` & `gdpc-7.2.0/src/gdpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 __url__              = "https://github.com/avdstaaij/gdpc"
 __author__           = "Arthur van der Staaij, Blinkenlights, Nils Gawlik"
 __author_email__     = "arthurvanderstaaij@gmail.com, blinkenlights@pm.me, nilsgawlik@gmx.de"
 __maintainer__       = "Arthur van der Staaij"
 __maintainer_email__ = "arthurvanderstaaij@gmail.com"
 __license__          = "MIT"
 __copyright__        = "Copyright 2022-2024 Arthur van der Staaij, Copyright 2021-2022 Blinkenlights, Copyright 2020-2021 Nils Gawlik"
-__version__          = "7.1.0"
+__version__          = "7.2.0"
 
 
 from .vector_tools import Rect, Box
 from .transform import Transform
 from .block import Block
 from .world_slice import WorldSlice
 from .editor import Editor
```

### Comparing `gdpc-7.1.0/gdpc/block.py` & `gdpc-7.2.0/src/gdpc/block.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/gdpc/block_state_tools.py` & `gdpc-7.2.0/src/gdpc/block_state_tools.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/gdpc/editor.py` & `gdpc-7.2.0/src/gdpc/editor.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/gdpc/editor_tools.py` & `gdpc-7.2.0/src/gdpc/editor_tools.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/gdpc/geometry.py` & `gdpc-7.2.0/src/gdpc/geometry.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/gdpc/interface.py` & `gdpc-7.2.0/src/gdpc/interface.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/gdpc/lookup.py` & `gdpc-7.2.0/src/gdpc/lookup.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/gdpc/minecraft_tools.py` & `gdpc-7.2.0/src/gdpc/minecraft_tools.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/gdpc/model.py` & `gdpc-7.2.0/src/gdpc/model.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/gdpc/nbt_tools.py` & `gdpc-7.2.0/src/gdpc/nbt_tools.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/gdpc/transform.py` & `gdpc-7.2.0/src/gdpc/transform.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/gdpc/utils.py` & `gdpc-7.2.0/src/gdpc/utils.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/gdpc/vector_tools.py` & `gdpc-7.2.0/src/gdpc/vector_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,304 +1,431 @@
 """Various vector utilities"""
 
-
-from typing import Iterator, Any, Iterable, List, Optional, Set, Tuple, Union
-from typing_extensions import Protocol
-from dataclasses import dataclass
 import math
+from dataclasses import dataclass
+from itertools import product as iterproduct
+from typing import (
+    Any,
+    Generator,
+    Iterable,
+    Iterator,
+    List,
+    Literal,
+    Optional,
+    Set,
+    Tuple,
+    Union,
+)
 
-from more_itertools import powerset
+import glm
 import numpy as np
-from scipy import ndimage
 import skimage.segmentation
-import glm
-from glm import ivec2, ivec3, vec2, vec3, bvec2, bvec3
+from glm import bvec2, bvec3, ivec2, ivec3, vec2, vec3
+from more_itertools import powerset
+from scipy import ndimage
+from typing_extensions import Protocol
 
 from .utils import nonZeroSign
 
-
 # ==================================================================================================
 # VecLike Protocols
 # ==================================================================================================
 
+
 class Vec2iLike(Protocol):
     """Protocol for a vector that contains two integers."""
+
     def __getitem__(self, __i: int) -> int: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[int]: ...
 
+
 class Vec3iLike(Protocol):
     """Protocol for a vector that contains three integers."""
+
     def __getitem__(self, __i: int) -> int: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[int]: ...
 
+
 class Vec2bLike(Protocol):
     """Protocol for a vector that contains two bools."""
+
     def __getitem__(self, __i: int) -> bool: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[bool]: ...
 
+
 class Vec3bLike(Protocol):
     """Protocol for a vector that contains three bools."""
+
     def __getitem__(self, __i: int) -> bool: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[bool]: ...
 
 
 # ==================================================================================================
 # Constants
 # ==================================================================================================
 
+# ==== 2D values ====
 
-UP    = ivec3( 0, 1, 0)
-DOWN  = ivec3( 0,-1, 0)
-EAST  = ivec3( 1, 0, 0)
-WEST  = ivec3(-1, 0, 0)
-NORTH = ivec3( 0, 0,-1)
-SOUTH = ivec3( 0, 0, 1)
-X     = ivec3( 1, 0, 0)
-Y     = ivec3( 0, 1, 0)
-Z     = ivec3( 0, 0, 1)
-XY    = ivec3( 1, 1, 0)
-XZ    = ivec3( 1, 0, 1)
-YZ    = ivec3( 0, 1, 1)
-XYZ   = ivec3( 1, 1, 1)
-
-DIAGONALS_2D = (
-    ivec2( 1,  1),
-    ivec2( 1, -1),
-    ivec2(-1,  1),
-    ivec2(-1, -1),
-)
-
-DIAGONALS_3D = (
-    ivec3( 1,  1,  0),
-    ivec3( 1,  0,  1),
-    ivec3( 0,  1,  1),
-    ivec3( 1, -1,  0),
-    ivec3( 1,  0, -1),
-    ivec3( 0,  1, -1),
-    ivec3(-1,  1,  0),
-    ivec3(-1,  0,  1),
-    ivec3( 0, -1,  1),
-    ivec3(-1, -1,  0),
-    ivec3(-1,  0, -1),
-    ivec3( 0, -1, -1),
-    ivec3( 1,  1,  1),
-    ivec3( 1,  1, -1),
-    ivec3( 1, -1,  1),
-    ivec3(-1,  1,  1),
-    ivec3( 1, -1, -1),
-    ivec3(-1, -1,  1),
-    ivec3(-1,  1, -1),
-    ivec3(-1, -1, -1),
-)
+X_2D = ivec2(1, 0)
+Y_2D = ivec2(0, 1)
+XY_2D: ivec2 = X_2D + Y_2D
+
+EAST_2D:  ivec2 = X_2D
+WEST_2D:  ivec2 = -EAST_2D
+SOUTH_2D: ivec2 = Y_2D
+NORTH_2D: ivec2 = -SOUTH_2D
+
+NORTHWEST_2D: ivec2 = NORTH_2D + WEST_2D
+NORTHEAST_2D: ivec2 = NORTH_2D + EAST_2D
+SOUTHEAST_2D: ivec2 = SOUTH_2D + EAST_2D
+SOUTHWEST_2D: ivec2 = SOUTH_2D + WEST_2D
+
+CARDINALS_2D:               Set[ivec2] = {NORTH_2D, SOUTH_2D, EAST_2D, WEST_2D}
+INTERCARDINALS_2D:          Set[ivec2] = {NORTHEAST_2D, NORTHWEST_2D, SOUTHEAST_2D, SOUTHWEST_2D}
+CARDINALS_AND_DIAGONALS_2D: Set[ivec2] = CARDINALS_2D | INTERCARDINALS_2D
+DIAGONALS_2D              = tuple(INTERCARDINALS_2D)  # NOTE: Legacy format
+
+# ==== 3D values ====
+
+X_3D = ivec3(1, 0, 0)
+Y_3D = ivec3(0, 1, 0)
+Z_3D = ivec3(0, 0, 1)
+
+XY_3D: ivec3 = X_3D + Y_3D
+XZ_3D: ivec3 = X_3D + Z_3D
+YZ_3D: ivec3 = Y_3D + Z_3D
+
+XYZ_3D: ivec3 = X_3D + Y_3D + Z_3D
+
+UP_3D:    ivec3 = Y_3D
+DOWN_3D:  ivec3 = -UP_3D
+EAST_3D:  ivec3 = X_3D
+WEST_3D:  ivec3 = -EAST_3D
+SOUTH_3D: ivec3 = Z_3D
+NORTH_3D: ivec3 = -SOUTH_3D
+
+NORTHEAST_3D: ivec3 = NORTH_3D + EAST_3D
+NORTHWEST_3D: ivec3 = NORTH_3D + WEST_3D
+SOUTHWEST_3D: ivec3 = SOUTH_3D + WEST_3D
+SOUTHEAST_3D: ivec3 = SOUTH_3D + EAST_3D
+
+CARDINALS_3D:               Set[ivec3] = {NORTH_3D, SOUTH_3D, EAST_3D, WEST_3D}
+INTERCARDINALS_3D:          Set[ivec3] = {NORTHEAST_3D, NORTHWEST_3D, SOUTHEAST_3D, SOUTHWEST_3D}
+CARDINALS_AND_DIAGONALS_3D: Set[ivec3] = CARDINALS_3D | INTERCARDINALS_3D
+
+DIRECTIONS_3D:     Set[ivec3] = CARDINALS_3D | {UP_3D, DOWN_3D}
+EDGE_DIAGONALS_3D: Set[ivec3] = INTERCARDINALS_3D | {
+    verticality + cardinal
+    for verticality, cardinal in iterproduct((UP_3D, DOWN_3D), CARDINALS_3D)
+}
+DIRECTIONS_AND_EDGE_DIAGONALS_3D: Set[ivec3] = DIRECTIONS_3D | EDGE_DIAGONALS_3D
+CORNER_DIAGONALS_3D:              Set[ivec3] = {
+    verticality + cardinal
+    for verticality, cardinal in iterproduct((UP_3D, DOWN_3D), INTERCARDINALS_3D)
+}
+DIRECTIONS_AND_ALL_DIAGONALS_3D: Set[ivec3] = DIRECTIONS_AND_EDGE_DIAGONALS_3D | CORNER_DIAGONALS_3D
+# TODO: tuple() for backwards compatibility. Remove on major release.
+DIAGONALS_3D                   = tuple(EDGE_DIAGONALS_3D | CORNER_DIAGONALS_3D)
+
+# ==== aliases ====
+
+X: ivec3 = X_3D
+Y: ivec3 = Y_3D
+Z: ivec3 = Z_3D
+XY: ivec3 = XY_3D
+XZ: ivec3 = XZ_3D
+YZ: ivec3 = YZ_3D
+XYZ: ivec3 = XYZ_3D
+UP : ivec3= UP_3D
+DOWN: ivec3 = DOWN_3D
+EAST: ivec3 = EAST_3D
+WEST: ivec3 = WEST_3D
+SOUTH: ivec3 = SOUTH_3D
+NORTH: ivec3 = NORTH_3D
+NORTHEAST: ivec3 = NORTHEAST_3D
+NORTHWEST: ivec3 = NORTHWEST_3D
+SOUTHWEST: ivec3 = SOUTHWEST_3D
+SOUTHEAST: ivec3 = SOUTHEAST_3D
+CARDINALS: Set[ivec3] = CARDINALS_3D
+INTERCARDINALS: Set[ivec3] = INTERCARDINALS_3D
+CARDINALS_AND_DIAGONALS: Set[ivec3] = CARDINALS_AND_DIAGONALS_3D
+EDGE_DIAGONALS: Set[ivec3] = EDGE_DIAGONALS_3D
+CORNER_DIAGONALS: Set[ivec3] = CORNER_DIAGONALS_3D
+DIAGONALS: tuple = DIAGONALS_3D
+DIRECTIONS: Set[ivec3] = DIRECTIONS_3D
+DIRECTIONS_AND_EDGE_DIAGONALS: Set[ivec3] = DIRECTIONS_AND_EDGE_DIAGONALS_3D
+DIRECTIONS_AND_ALL_DIAGONALS: Set[ivec3] = DIRECTIONS_AND_ALL_DIAGONALS_3D
 
 
 # ==================================================================================================
 # General
 # ==================================================================================================
 
 
-def dropDimension(vec: Vec3iLike, dimension: int):
+def dropDimension(vec: Vec3iLike, dimension: int) -> ivec2:
     """Returns <vec> without its <dimension>-th component"""
     if dimension == 0: return ivec2(vec[1], vec[2])
     if dimension == 1: return ivec2(vec[0], vec[2])
     if dimension == 2: return ivec2(vec[0], vec[1])
     raise ValueError(f'Invalid dimension "{dimension}"')
 
 
-def addDimension(vec: Vec2iLike, dimension: int, value=0):
+def addDimension(vec: Vec2iLike, dimension: int, value: int = 0) -> ivec3:
     """Inserts <value> into <vec> at <dimension> and returns the resulting 3D vector"""
+    # NOTE: Should be adjusted to only support 2D -> 3D, or all ivec dimensions
     l = list(vec)
     return ivec3(*l[:dimension], value, *l[dimension:])
 
 
-def dropY(vec: Vec3iLike):
+def dropY(vec: Vec3iLike) -> ivec2:
     """Returns [vec] without its y-component (i.e., projected on the XZ-plane)"""
     return ivec2(vec[0], vec[2])
 
 
-def addY(vec: Vec2iLike, y=0):
+def addY(vec: Vec2iLike, y=0) -> ivec3:
     """Returns a 3D vector (vec[0], y, vec[1])"""
     return ivec3(vec[0], y, vec[1])
 
 
-def setY(vec: Vec3iLike, y=0):
+def setY(vec: Vec3iLike, y=0) -> ivec3:
     """Returns [vec] with its y-component set to [y]"""
     return ivec3(vec[0], y, vec[2])
 
 
-def trueMod2D(vec: Vec2iLike, modulus: int):
+def trueMod2D(vec: Vec2iLike, modulus: int) -> ivec2:
     """Returns <v> modulo <modulus>.\n
     Negative numbers are handled just like Python's built-in integer modulo."""
     return ivec2(vec[0] % modulus, vec[1] % modulus)
 
-def trueMod3D(vec: Vec3iLike, modulus: int):
+
+def trueMod3D(vec: Vec3iLike, modulus: int) -> ivec3:
     """Returns <v> modulo <modulus>.\n
     Negative numbers are handled just like Python's built-in integer modulo."""
     return ivec3(vec[0] % modulus, vec[1] % modulus, vec[2] % modulus)
 
 
-def perpendicular(vec: Vec2iLike):
+def perpendicular(vec: Vec2iLike) -> ivec2:
     """Returns the vector perpendicular to [vec] that points to the right of [vec] and has the same
     length as [vec]."""
     return ivec2(vec[1], -vec[0])
 
 
-def rotate2D(vec: Vec2iLike, rotation: int):
-    """Returns [vec], rotated by [rotation]"""
+def rotate2D(vec: Vec2iLike, rotation: int) -> ivec2:
+    """Returns [vec], rotated clockwise by [rotation] quarters."""
     if rotation == 0: return ivec2(*vec)
     if rotation == 1: return ivec2(-vec[1],  vec[0])
     if rotation == 2: return ivec2(-vec[0], -vec[1])
     if rotation == 3: return ivec2( vec[1], -vec[0])
     raise ValueError("Rotation must be in {0,1,2,3}")
 
 
-def rotate3D(vec: Vec3iLike, rotation: int):
-    """Returns [vec], rotated in the XZ-plane by [rotation]"""
+def rotate3D(vec: Vec3iLike, rotation: int) -> ivec3:
+    """Returns [vec], rotated clockwise in the XZ-plane by [rotation] quarters."""
     return addY(rotate2D(dropY(vec), rotation), vec[1])
 
 
-def flipRotation2D(rotation: int, flip: Vec2bLike):
+def rotate2Ddeg(vec: Vec2iLike, degrees: int) -> ivec2:
+    """
+    Rotate a 2D vector clockwise by a specified number of degrees.
+
+    Args:
+        vec: The 2D vector to rotate.
+        degrees: The number of degrees to rotate the vector by. Only ±90°-rotations and their multiples are valid.
+
+    Returns:
+        The rotated 2D vector.
+
+    Raises:
+        ValueError: If degrees is not a multiple of 90.
+
+    Examples:
+        vec = ivec2(0, 1)
+        rotated_vec = rotate2Ddeg(vec, -90)
+    """
+
+    if degrees % 90 != 0:
+        raise ValueError("Only ±90°-rotations and their multiples are valid!")
+
+    rotation: int = (degrees // 90) % 4  # Convert to quarter-turns
+
+    return rotate2D(vec, rotation)
+
+
+def rotate3Ddeg(vec: Vec3iLike, degrees: int) -> ivec3:
+    """
+    Rotate a 3D vector clockwise by a specified number of degrees through the Y axis.
+
+    Args:
+        vec: The 3D vector to rotate.
+        degrees: The number of degrees to rotate the vector by through the Y axis. Only ±90°-rotations and their multiples are valid.
+
+    Returns:
+        The rotated 3D vector.
+
+    Raises:
+        ValueError: If degrees is not a multiple of 90.
+
+    Examples:
+        vec = ivec3(0, 1)
+        rotated_vec = rotate3Ddeg(vec, -90)
+    """
+    return addY(rotate2Ddeg(dropY(vec), degrees), vec[1])
+
+
+def flipRotation2D(rotation: int, flip: Vec2bLike) -> int:
     """Returns rotation such that applying rotation after <flip> is equivalent to applying <flip>
     after <rotation>."""
-    scale = flipToScale2D(flip)
+    scale: ivec2 = flipToScale2D(flip)
     return (rotation * scale.x * scale.y + 4) % 4
 
-def flipRotation3D(rotation: int, flip: Vec3bLike):
+
+def flipRotation3D(rotation: int, flip: Vec3bLike) -> int:
     """Returns rotation such that applying rotation after <flip> is equivalent to applying <flip>
     after <rotation>"""
     return flipRotation2D(rotation, dropY(flip))
 
 
-def rotateSize2D(size: Vec2iLike, rotation: int):
+def rotateSize2D(size: Vec2iLike, rotation: int) -> Vec2iLike:
     """Returns the effective size of a rect of size [size] that has been rotated in the XZ-plane by
     [rotation]."""
-    return ivec2(size[1], size[0]) if rotation in [1, 3] else size
+    return ivec2(size[1], size[0]) if rotation in {1, 3} else size
 
 
-def rotateSize3D(size: Vec3iLike, rotation: int):
+def rotateSize3D(size: Vec3iLike, rotation: int) -> ivec3:
     """Returns the effective size of a box of size [size] that has been rotated in the XZ-plane by
     [rotation]."""
     return addY(rotateSize2D(dropY(size), rotation), size[1])
 
 
-def flipToScale2D(flip: Vec2bLike):
+def flipToScale2D(flip: Vec2bLike) -> ivec2:
     """Returns a vector with a 1 where <flip> is false, and -1 where <flip> is true"""
-    return 1 - 2*ivec2(*flip)
+    return 1 - 2 * ivec2(*flip)
+
 
-def flipToScale3D(flip: Vec3bLike):
+def flipToScale3D(flip: Vec3bLike) -> ivec3:
     """Returns a vector with a 1 where <flip> is false, and -1 where <flip> is true"""
-    return 1 - 2*ivec3(*flip)
+    return 1 - 2 * ivec3(*flip)
 
 
-def scaleToFlip2D(scale: Vec2iLike):
+def scaleToFlip2D(scale: Vec2iLike) -> bvec2:
     """Returns whether [scale] flips space in each axis"""
     return bvec2(scale[0] < 0, scale[1] < 0)
 
-def scaleToFlip3D(scale: Vec3iLike):
+
+def scaleToFlip3D(scale: Vec3iLike) -> bvec3:
     """Returns whether [scale] flips space in each axis"""
     return bvec3(scale[0] < 0, scale[1] < 0, scale[2] < 0)
 
 
-def toAxisVector2D(vec: Vec2iLike):
+def toAxisVector2D(vec: Vec2iLike) -> ivec2:
     """Returns the axis-aligned unit vector closest to [vec]"""
-    if abs(vec[0]) > abs(vec[1]): # pylint: disable=no-else-return
+    if abs(vec[0]) > abs(vec[1]):  # pylint: disable=no-else-return
         return ivec2(nonZeroSign(vec[0]), 0)
     else:
         return ivec2(0, nonZeroSign(vec[1]))
 
 
-def directionToRotation(direction: Vec2iLike):
+def directionToRotation(direction: Vec2iLike) -> Union[Literal[0], Literal[1], Literal[2], Literal[3]]:
     """Returns the rotation that rotates (0,-1) closest to [direction]"""
     vec = toAxisVector2D(direction)
     if vec[1] < 0: return 0
     if vec[0] > 0: return 1
     if vec[1] > 0: return 2
     if vec[0] < 0: return 3
     raise ValueError()
 
 
 # For some reason, glm's length, length2, distance, distance2 and l1Norm refuse to work with integer
 # vectors. We provide some wrappers.
 
-def length(vec: Union[Vec2iLike, Vec3iLike]):
+
+def length(vec: Union[Vec2iLike, Vec3iLike]) -> float:
     """Returns the length of [vec]"""
     if len(vec) == 2: return glm.length(vec2(*vec))
     if len(vec) == 3: return glm.length(vec3(*vec))
     raise ValueError()
 
-def length2(vec: Union[Vec2iLike, Vec3iLike]):
+
+def length2(vec: Union[Vec2iLike, Vec3iLike]) -> int:
     """Returns the squared length of [vec]"""
     if len(vec) == 2: return int(glm.length2(vec2(*vec)))
     if len(vec) == 3: return int(glm.length2(vec3(*vec)))
     raise ValueError()
 
+
 def distance(vecA: Union[Vec2iLike, Vec3iLike], vecB: Union[Vec2iLike, Vec3iLike]) -> float:
     """Returns the distance between [vecA] and [vecB]"""
     if len(vecA) == 2 and len(vecB) == 2: return glm.distance(vec2(*vecA), vec2(*vecB))
     if len(vecA) == 3 and len(vecB) == 3: return glm.distance(vec3(*vecA), vec3(*vecB))
     raise ValueError()
 
-def distance2(vecA: Union[Vec2iLike, Vec3iLike], vecB: Union[Vec2iLike, Vec3iLike]):
+
+def distance2(vecA: Union[Vec2iLike, Vec3iLike], vecB: Union[Vec2iLike, Vec3iLike]) -> int:
     """Returns the squared distance between [vecA] and [vecB]"""
     if len(vecA) == 2 and len(vecB) == 2: return int(glm.distance2(vec2(*vecA), vec2(*vecB)))
     if len(vecA) == 3 and len(vecB) == 3: return int(glm.distance2(vec3(*vecA), vec3(*vecB)))
     raise ValueError()
 
-def l1Norm(vec: Union[Vec2iLike, Vec3iLike]):
+
+def l1Norm(vec: Union[Vec2iLike, Vec3iLike]) -> int:
     """Returns the L1 norm of [vec]"""
     return sum(abs(n) for n in vec)
 
-def l1Distance(vecA: Union[Vec2iLike, Vec3iLike], vecB: Union[Vec2iLike, Vec3iLike]):
+
+def l1Distance(vecA: Union[Vec2iLike, Vec3iLike], vecB: Union[Vec2iLike, Vec3iLike]) -> int:
     """Returns the L1 norm distance between [vecA] and [vecB]"""
     return l1Norm(vecA - vecB)
 
 
-def orderedCorners2D(corner1: Vec2iLike, corner2: Vec2iLike):
+# End of glm wrappers.
+
+
+def orderedCorners2D(corner1: Vec2iLike, corner2: Vec2iLike) -> Tuple[ivec2, ivec2]:
     """Returns two corners of the rectangle defined by <corner1> and <corner2>, such that the first
     corner is smaller than the second corner in each axis"""
     return (
         ivec2(
             corner1[0] if corner1[0] <= corner2[0] else corner2[0],
             corner1[1] if corner1[1] <= corner2[1] else corner2[1],
         ),
         ivec2(
             corner1[0] if corner1[0] > corner2[0] else corner2[0],
             corner1[1] if corner1[1] > corner2[1] else corner2[1],
-        )
+        ),
     )
 
 
-def orderedCorners3D(corner1: Vec3iLike, corner2: Vec3iLike):
+def orderedCorners3D(corner1: Vec3iLike, corner2: Vec3iLike) -> Tuple[ivec3, ivec3]:
     """Returns two corners of the box defined by <corner1> and <corner2>, such that the first
     corner is smaller than the second corner in each axis"""
     return (
         ivec3(
             corner1[0] if corner1[0] <= corner2[0] else corner2[0],
             corner1[1] if corner1[1] <= corner2[1] else corner2[1],
             corner1[2] if corner1[2] <= corner2[2] else corner2[2],
         ),
         ivec3(
             corner1[0] if corner1[0] > corner2[0] else corner2[0],
             corner1[1] if corner1[1] > corner2[1] else corner2[1],
             corner1[2] if corner1[2] > corner2[2] else corner2[2],
-        )
+        ),
     )
 
 
 def getDimensionality(corner1: Union[Vec2iLike, Vec3iLike], corner2: Union[Vec2iLike, Vec3iLike]) -> Tuple[int, List[str]]:
     """Determines the number of dimensions for which <corner1> and <corner2> are in general
     position, i.e. the number of dimensions for which the volume they define is not flat.\n
     Returns (dimensionality, list of indices of dimensions for which the volume is flat).
     For example: (2, [0,2]) means that the volume is flat in the x and z axes."""
     difference = np.array(corner1) - np.array(corner2)
-    flatSides = np.argwhere(difference == 0).flatten()
+    flatSides: np.ndarray[Any, np.dtype[np.signedinteger[Any]]] = np.argwhere(difference == 0).flatten()
     return int(len(corner1) - np.sum(flatSides)), list(flatSides)
 
 
 # ==================================================================================================
 # Rect and Box
 # ==================================================================================================
 
@@ -307,599 +434,684 @@
 
 
 @dataclass
 class Rect:
     """A rectangle, defined by an offset and a size"""
 
     _offset: ivec2
-    _size:   ivec2
+    _size: ivec2
 
-    def __init__(self, offset: Vec2iLike = (0,0), size: Vec2iLike = (0,0)):
+    def __init__(self, offset: Vec2iLike = (0, 0), size: Vec2iLike = (0, 0)) -> None:
         self._offset = ivec2(*offset)
-        self._size   = ivec2(*size)
+        self._size = ivec2(*size)
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash((self.offset, self.size))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"Rect({tuple(self._offset)}, {tuple(self._size)})"
 
     @property
-    def offset(self):
+    def offset(self) -> ivec2:
         """This Rect's offset"""
         return self._offset
 
     @offset.setter
-    def offset(self, value: Vec2iLike):
+    def offset(self, value: Vec2iLike) -> None:
         self._offset = ivec2(*value)
 
     @property
-    def size(self):
+    def size(self) -> ivec2:
         """This Rect's size"""
         return self._size
 
     @size.setter
-    def size(self, value: Vec2iLike):
+    def size(self, value: Vec2iLike) -> None:
         self._size = ivec2(*value)
 
     @property
-    def begin(self):
+    def begin(self) -> ivec2:
         """Equivalent to self.offset. Setting will modify self.offset."""
         return self._offset
 
     @begin.setter
-    def begin(self, value: Vec2iLike):
+    def begin(self, value: Vec2iLike) -> None:
         self._offset = ivec2(*value)
 
     @property
-    def end(self):
+    def end(self) -> ivec2:
         """Equivalent to self.offset + self.size. Setting will modify self.size."""
         return self.begin + self._size
 
     @end.setter
-    def end(self, value: Vec2iLike):
+    def end(self, value: Vec2iLike) -> None:
         self._size = ivec2(*value) - self.begin
 
     @property
-    def last(self):
+    def last(self) -> ivec2:
         """Equivalent to self.offset + self.size - 1. Setting will modify self.size."""
         return self._offset + self._size - 1
 
     @last.setter
-    def last(self, value: Vec2iLike):
+    def last(self, value: Vec2iLike) -> None:
         self._size = ivec2(*value) - self._offset + 1
 
     @property
-    def middle(self):
+    def middle(self) -> ivec2:
         """This Rect's middle point, rounded down"""
         return self._offset + self._size // 2
 
     @property
-    def center(self):
+    def center(self) -> ivec2:
         """Equivalent to .middle"""
         return self.middle
 
     @property
-    def inner(self):
+    def inner(self) -> Generator[ivec2, None, None]:
         """Yields all points contained in this Rect"""
         return (
             ivec2(x, y)
             for x in range(self.begin.x, self.end.x)
             for y in range(self.begin.y, self.end.y)
         )
 
     @property
-    def area(self):
+    def area(self) -> int:
         """This Rect's surface area"""
-        return self._size.x*self._size.y
+        return self._size.x * self._size.y
 
     @property
-    def corners(self):
+    def corners(self) -> Generator[ivec2, None, None]:
         """Yields this Rect's corner points"""
         return (
             self._offset + sum(subset)
-            for subset in powerset([ivec2(self._size.x-1, 0), ivec2(0, self._size.y-1)])
+            for subset in powerset(
+                [ivec2(self._size.x - 1, 0), ivec2(0, self._size.y - 1)]
+            )
         )
 
-    def contains(self, vec: Vec2iLike):
+    def contains(self, vec: Vec2iLike) -> bool:
         """Returns whether this Rect contains [vec]"""
         return (
-            self.begin.x <= vec[0] < self.end.x and
-            self.begin.y <= vec[1] < self.end.y
+            self.begin.x <= vec[0] < self.end.x and self.begin.y <= vec[1] < self.end.y
         )
 
-    def collides(self, other: 'Rect'):
+    def collides(self, other: "Rect") -> bool:
         """Returns whether this Rect and [other] have any overlap"""
         return (
-            self.begin.x <= other.end  .x and
-            self.end  .x >= other.begin.x and
-            self.begin.y <= other.end  .y and
-            self.end  .y >= other.begin.y
+                self.begin.x <= other.end  .x
+            and self.end  .x >= other.begin.x
+            and self.begin.y <= other.end  .y
+            and self.end  .y >= other.begin.y
         )
 
-    def squaredDistanceToVec(self, vec: Vec2iLike):
+    def squaredDistanceToVec(self, vec: Vec2iLike) -> int:
         """Returns the squared distance between this Rect and [vec]"""
-        dx = max(self.begin.x - vec[0], 0, vec[0] - (self.end[0] - 1))
-        dy = max(self.begin.y - vec[1], 0, vec[1] - (self.end[1] - 1))
-        return dx*dx + dy*dy
+        dx: int = max(self.begin.x - vec[0], 0, vec[0] - (self.end[0] - 1))
+        dy: int = max(self.begin.y - vec[1], 0, vec[1] - (self.end[1] - 1))
+        return dx**2 + dy**2
 
-    def distanceToVec(self, vec: Vec2iLike):
+    def distanceToVec(self, vec: Vec2iLike) -> float:
         """Returns the distance between this Rect and [vec]"""
         return math.sqrt(self.squaredDistanceToVec(vec))
 
-    def translated(self, translation: Union[Vec2iLike, int]):
+    def translated(self, translation: Union[Vec2iLike, int]) -> "Rect":
         """Returns a copy of this Rect, translated by [translation]"""
         return Rect(self._offset + ivec2(*translation), self._size)
 
-    def dilate(self, dilation: int = 1):
+    def dilate(self, dilation: int = 1) -> None:
         """Morphologically dilates this rect by [dilation]"""
-        self._offset  -= dilation
-        self._size    += dilation*2
+        self._offset -= dilation
+        self._size += dilation * 2
 
-    def dilated(self, dilation: int = 1):
+    def dilated(self, dilation: int = 1) -> "Rect":
         """Returns a copy of this Rect, morphologically dilated by [dilation]"""
-        return Rect(self._offset - dilation, self._size + dilation*2)
+        return Rect(self._offset - dilation, self._size + dilation * 2)
 
-    def erode(self, erosion: int = 1):
+    def erode(self, erosion: int = 1) -> None:
         """Morphologically erodes this rect by [erosion]"""
         self.dilate(-erosion)
 
-    def eroded(self, erosion: int = 1):
+    def eroded(self, erosion: int = 1) -> "Rect":
         """Returns a copy of this Rect, morphologically eroded by [erosion]"""
         return self.dilated(-erosion)
 
-    def centeredSubRectOffset(self, size: Vec2iLike):
+    def centeredSubRectOffset(self, size: Vec2iLike) -> ivec2:
         """Returns an offset such that Rect(offset, [size]).middle == self.middle"""
-        difference = self._size - ivec2(*size)
-        return self._offset + difference/2
+        difference: ivec2 = self._size - ivec2(*size)
+        return self._offset + difference / 2
 
-    def centeredSubRect(self, size: Vec2iLike):
+    def centeredSubRect(self, size: Vec2iLike) -> "Rect":
         """Returns a rect of size [size] with the same middle as this rect"""
         return Rect(self.centeredSubRectOffset(size), size)
 
     @staticmethod
-    def between(cornerA: Vec2iLike, cornerB: Vec2iLike):
+    def between(cornerA: Vec2iLike, cornerB: Vec2iLike) -> "Rect":
         """Returns the Rect between [cornerA] and [cornerB] (inclusive),
         which may be any opposing corners."""
         first, last = orderedCorners2D(cornerA, cornerB)
         return Rect(first, (last - first) + 1)
 
     @staticmethod
-    def bounding(points: Iterable[Vec2iLike]):
+    def bounding(points: Iterable[Vec2iLike]) -> "Rect":
         """Returns the smallest Rect containing all [points]"""
         pointArray = np.fromiter(points, dtype=np.dtype((int, 2)))
         minPoint = np.min(pointArray, axis=0)
         maxPoint = np.max(pointArray, axis=0)
         return Rect(minPoint, maxPoint - minPoint + 1)
 
-    def toBox(self, offsetY = 0, sizeY = 0):
+    def toBox(self, offsetY=0, sizeY=0) -> "Box":
         """Returns a corresponding Box"""
         return Box(addY(self.offset, offsetY), addY(self._size, sizeY))
 
     @property
-    def outline(self):
+    def outline(self) -> Generator[ivec2, Any, None]:
         """Yields this Rect's outline points"""
         # It's surprisingly difficult to get this right without duplicates. (Think of the corners!)
         first = self.begin
-        last  = self.end - 1
-        yield from loop2D(ivec2(first.x, first.y), ivec2(last.x  -1, first.y   ) + 1)
-        yield from loop2D(ivec2(last.x,  first.y), ivec2(last.x,     last.y  -1) + 1)
-        yield from loop2D(ivec2(last.x,  last.y),  ivec2(first.x +1, last.y    ) - 1)
-        yield from loop2D(ivec2(first.x, last.y),  ivec2(first.x,    first.y +1) - 1)
+        last = self.end - 1
+        yield from loop2D(ivec2(first.x, first.y), ivec2(last.x  - 1, first.y    ) + 1)
+        yield from loop2D(ivec2(last.x,  first.y), ivec2(last.x,      last.y  - 1) + 1)
+        yield from loop2D(ivec2(last.x,  last.y ), ivec2(first.x + 1, last.y     ) - 1)
+        yield from loop2D(ivec2(first.x, last.y ), ivec2(first.x,     first.y + 1) - 1)
 
 
 @dataclass()
 class Box:
     """A box, defined by an offset and a size"""
 
     _offset: ivec3
-    _size:   ivec3
+    _size: ivec3
 
-    def __init__(self, offset: Vec3iLike = (0,0,0), size: Vec3iLike = (0,0,0)):
+    def __init__(self, offset: Vec3iLike = (0, 0, 0), size: Vec3iLike = (0, 0, 0)) -> None:
         self._offset = ivec3(*offset)
-        self._size   = ivec3(*size)
+        self._size = ivec3(*size)
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash((self.offset, self.size))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"Box({tuple(self._offset)}, {tuple(self._size)})"
 
     @property
-    def offset(self):
+    def offset(self) -> ivec3:
         """This Box's offset"""
         return self._offset
 
     @offset.setter
-    def offset(self, value: Vec3iLike):
+    def offset(self, value: Vec3iLike) -> None:
         self._offset = ivec3(*value)
 
     @property
-    def size(self):
+    def size(self) -> ivec3:
         """This Box's size"""
         return self._size
 
     @size.setter
-    def size(self, value: Vec3iLike):
+    def size(self, value: Vec3iLike) -> None:
         self._size = ivec3(*value)
 
     @property
-    def begin(self):
+    def begin(self) -> ivec3:
         """Equivalent to self.offset. Setting will modify self.offset."""
         return self._offset
 
     @begin.setter
-    def begin(self, value: Vec3iLike):
+    def begin(self, value: Vec3iLike) -> None:
         self._offset = ivec3(*value)
 
     @property
-    def end(self):
+    def end(self) -> ivec3:
         """Equivalent to self.offset + self.size. Setting will modify self.size."""
         return self.begin + self._size
 
     @end.setter
-    def end(self, value: Vec3iLike):
+    def end(self, value: Vec3iLike) -> None:
         self._size = ivec3(*value) - self.begin
 
     @property
-    def last(self):
+    def last(self) -> ivec3:
         """Equivalent to self.offset + self.size - 1. Setting will modify self.size."""
         return self._offset + self._size - 1
 
     @last.setter
-    def last(self, value: Vec3iLike):
+    def last(self, value: Vec3iLike) -> None:
         self._size = ivec3(*value) - self._offset + 1
 
     @property
-    def middle(self):
+    def middle(self) -> ivec3:
         """This Box's middle point, rounded down"""
         return self.begin + self._size // 2
 
     @property
-    def center(self):
+    def center(self) -> ivec3:
         """Equivalent to .middle"""
         return self.middle
 
     @property
-    def inner(self):
+    def inner(self) -> Generator[ivec3, None, None]:
         """Yields all points contained in this Box"""
         return (
             ivec3(x, y, z)
             for x in range(self.begin.x, self.end.x)
             for y in range(self.begin.y, self.end.y)
             for z in range(self.begin.z, self.end.z)
         )
 
     @property
-    def volume(self):
+    def volume(self) -> int:
         """This Box's volume"""
-        return self._size.x*self._size.y*self._size.z
+        return self._size.x * self._size.y * self._size.z
 
     @property
-    def corners(self):
+    def corners(self) -> List[ivec3]:
         """Yields this Box's corner points"""
         return [
             self._offset + sum(subset)
-            for subset in powerset([ivec3(self._size.x-1, 0, 0), ivec3(0, self._size.y-1, 0), ivec3(0, 0, self._size.z-1)])
+            for subset in powerset(
+                [
+                    ivec3(self._size.x - 1, 0, 0),
+                    ivec3(0, self._size.y - 1, 0),
+                    ivec3(0, 0, self._size.z - 1),
+                ]
+            )
         ]
 
-    def contains(self, vec: Vec3iLike):
+    def contains(self, vec: Vec3iLike) -> bool:
         """Returns whether this Box contains [vec]"""
         return (
-            self.begin.x <= vec[0] < self.end.x and
-            self.begin.y <= vec[1] < self.end.y and
-            self.begin.z <= vec[2] < self.end.z
+                self.begin.x <= vec[0] < self.end.x
+            and self.begin.y <= vec[1] < self.end.y
+            and self.begin.z <= vec[2] < self.end.z
         )
 
-    def collides(self, other: 'Box'):
+    def collides(self, other: "Box") -> bool:
         """Returns whether this Box and [other] have any overlap"""
         return (
-            self.begin.x <= other.end  .x and
-            self.end  .x >= other.begin.x and
-            self.begin.y <= other.end  .y and
-            self.end  .y >= other.begin.y and
-            self.begin.z <= other.end  .z and
-            self.end  .z >= other.begin.z
+                self.begin.x <= other.end  .x
+            and self.end  .x >= other.begin.x
+            and self.begin.y <= other.end  .y
+            and self.end  .y >= other.begin.y
+            and self.begin.z <= other.end  .z
+            and self.end  .z >= other.begin.z
         )
 
-    def squaredDistanceToVec(self, vec: Vec3iLike):
+    def squaredDistanceToVec(self, vec: Vec3iLike) -> int:
         """Returns the squared distance between this Box and [vec]"""
-        dx = max(self.begin.x - vec[0], 0, vec[0] - (self.end.x - 1))
-        dy = max(self.begin.y - vec[1], 0, vec[1] - (self.end.y - 1))
-        dz = max(self.begin.z - vec[2], 0, vec[2] - (self.end.z - 1))
-        return dx*dx + dy*dy + dz*dz
+        dx: int = max(self.begin.x - vec[0], 0, vec[0] - (self.end.x - 1))
+        dy: int = max(self.begin.y - vec[1], 0, vec[1] - (self.end.y - 1))
+        dz: int = max(self.begin.z - vec[2], 0, vec[2] - (self.end.z - 1))
+        return dx**2 + dy**2 + dz**2
 
-    def distanceToVec(self, vec: Vec3iLike):
+    def distanceToVec(self, vec: Vec3iLike) -> float:
         """Returns the distance between this Box and [vec]"""
         return math.sqrt(self.squaredDistanceToVec(vec))
 
-    def translated(self, translation: Union[Vec3iLike, int]):
+    def translated(self, translation: Union[Vec3iLike, int]) -> "Box":
         """Returns a copy of this Box, translated by [translation]"""
         return Box(self._offset + ivec3(*translation), self._size)
 
-    def dilate(self, dilation: int = 1):
+    def dilate(self, dilation: int = 1) -> None:
         """Morphologically dilates this box by [dilation]"""
         self._offset -= dilation
-        self._size   += dilation*2
+        self._size += dilation * 2
 
-    def dilated(self, dilation: int = 1):
+    def dilated(self, dilation: int = 1) -> "Box":
         """Returns a copy of this Box, morphologically dilated by [dilation]"""
-        return Box(self._offset - dilation, self._size + dilation*2)
+        return Box(self._offset - dilation, self._size + dilation * 2)
 
-    def erode(self, erosion: int = 1):
+    def erode(self, erosion: int = 1) -> None:
         """Morphologically erodes this box by [erosion]"""
         self.dilate(-erosion)
 
-    def eroded(self, erosion: int = 1):
+    def eroded(self, erosion: int = 1) -> "Box":
         """Returns a copy of this Box, morphologically eroded by [erosion]"""
         return self.dilated(-erosion)
 
-    def centeredSubBoxOffset(self, size: Vec3iLike):
+    def centeredSubBoxOffset(self, size: Vec3iLike) -> ivec3:
         """Returns an offset such that Box(offset, [size]).middle == self.middle"""
-        difference = self._size - ivec3(*size)
-        return self._offset + difference/2
+        difference: ivec3 = self._size - ivec3(*size)
+        return self._offset + difference / 2
 
-    def centeredSubBox(self, size: Vec3iLike):
+    def centeredSubBox(self, size: Vec3iLike) -> "Box":
         """Returns an box of size [size] with the same middle as this box"""
         return Box(self.centeredSubBoxOffset(size), size)
 
     @staticmethod
-    def between(cornerA: Vec3iLike, cornerB: Vec3iLike):
+    def between(cornerA: Vec3iLike, cornerB: Vec3iLike) -> "Box":
         """Returns the Box between [cornerA] and [cornerB] (both inclusive),
         which may be any opposing corners"""
         first, last = orderedCorners3D(cornerA, cornerB)
         return Box(first, last - first + 1)
 
     @staticmethod
-    def bounding(points: Iterable[Vec3iLike]):
+    def bounding(points: Iterable[Vec3iLike]) -> "Box":
         """Returns the smallest Box containing all [points]"""
         pointArray = np.fromiter(points, dtype=np.dtype((int, 3)))
-        minPoint = np.min(pointArray, axis=0)
-        maxPoint = np.max(pointArray, axis=0)
+        minPoint: np.ndarray = np.min(pointArray, axis=0)
+        maxPoint: np.ndarray = np.max(pointArray, axis=0)
         return Box(minPoint, maxPoint - minPoint + 1)
 
-    def toRect(self):
+    def toRect(self) -> Rect:
         """Returns this Box's XZ-plane as a Rect"""
         return Rect(dropY(self._offset), dropY(self._size))
 
     @property
-    def shell(self):
+    def shell(self) -> Generator[ivec3, Any, None]:
         """Yields all points on this Box's surface"""
         # It's surprisingly difficult to get this right without duplicates. (Think of the corners!)
-        first = self.begin
-        last  = self.end - 1
+        first: ivec3 = self.begin
+        last: ivec3 = self.end - 1
         # Bottom face
-        yield from loop3D(ivec3(first.x, first.y, first.z), ivec3(last.x, first.y, last.z) + 1)
+        yield from loop3D(
+            ivec3(first.x, first.y, first.z),
+            ivec3(last.x, first.y, last.z) + 1,
+        )
         # Top face
-        yield from loop3D(ivec3(first.x, last.y, first.z), ivec3(last.x, last.y, last.z) + 1)
+        yield from loop3D(
+            ivec3(first.x, last.y, first.z),
+            ivec3(last.x, last.y, last.z) + 1,
+        )
         # Sides
         if self._size.y < 3:
             return
-        yield from loop3D(ivec3(first.x, first.y+1, first.z), ivec3(last.x -1,  last.y-1, first.z   ) + 1)
-        yield from loop3D(ivec3(last.x,  first.y+1, first.z), ivec3(last.x,     last.y-1, last.z  -1) + 1)
-        yield from loop3D(ivec3(last.x,  first.y+1, last.z ), ivec3(first.x +1, last.y+1, last.z    ) - 1)
-        yield from loop3D(ivec3(first.x, first.y+1, last.z ), ivec3(first.x,    last.y+1, first.z +1) - 1)
+        yield from loop3D(
+            ivec3(first.x, first.y + 1, first.z),
+            ivec3(last.x - 1, last.y - 1, first.z) + 1,
+        )
+        yield from loop3D(
+            ivec3(last.x, first.y + 1, first.z),
+            ivec3(last.x, last.y - 1, last.z - 1) + 1,
+        )
+        yield from loop3D(
+            ivec3(last.x, first.y + 1, last.z),
+            ivec3(first.x + 1, last.y + 1, last.z) - 1,
+        )
+        yield from loop3D(
+            ivec3(first.x, first.y + 1, last.z),
+            ivec3(first.x, last.y + 1, first.z + 1) - 1,
+        )
 
     @property
-    def wireframe(self):
+    def wireframe(self) -> Generator[ivec3, Any, None]:
         """Yields all points on this Box's edges"""
         # It's surprisingly difficult to get this right without duplicates. (Think of the corners!)
-        first = self.begin
-        last  = self.end - 1
+        first: ivec3 = self.begin
+        last: ivec3 = self.end - 1
         # Bottom face
-        yield from loop3D(ivec3(first.x, first.y, first.z), ivec3(last.x -1,  first.y, first.z   ) + 1)
-        yield from loop3D(ivec3(last.x,  first.y, first.z), ivec3(last.x,     first.y, last.z  -1) + 1)
-        yield from loop3D(ivec3(last.x,  first.y, last.z ), ivec3(first.x +1, first.y, last.z    ) - 1)
-        yield from loop3D(ivec3(first.x, first.y, last.z ), ivec3(first.x,    first.y, first.z +1) - 1)
+        yield from loop3D(
+            ivec3(first.x, first.y, first.z),
+            ivec3(last.x - 1, first.y, first.z) + 1,
+        )
+        yield from loop3D(
+            ivec3(last.x, first.y, first.z),
+            ivec3(last.x, first.y, last.z - 1) + 1,
+        )
+        yield from loop3D(
+            ivec3(last.x, first.y, last.z),
+            ivec3(first.x + 1, first.y, last.z) - 1,
+        )
+        yield from loop3D(
+            ivec3(first.x, first.y, last.z),
+            ivec3(first.x, first.y, first.z + 1) - 1,
+        )
         # top face
-        yield from loop3D(ivec3(first.x, last.y,  first.z), ivec3(last.x -1,  last.y,  first.z   ) + 1)
-        yield from loop3D(ivec3(last.x,  last.y,  first.z), ivec3(last.x,     last.y,  last.z  -1) + 1)
-        yield from loop3D(ivec3(last.x,  last.y,  last.z ), ivec3(first.x +1, last.y,  last.z    ) - 1)
-        yield from loop3D(ivec3(first.x, last.y,  last.z ), ivec3(first.x,    last.y,  first.z +1) - 1)
+        yield from loop3D(
+            ivec3(first.x, last.y, first.z),
+            ivec3(last.x - 1, last.y, first.z) + 1,
+        )
+        yield from loop3D(
+            ivec3(last.x, last.y, first.z),
+            ivec3(last.x, last.y, last.z - 1) + 1,
+        )
+        yield from loop3D(
+            ivec3(last.x, last.y, last.z),
+            ivec3(first.x + 1, last.y, last.z) - 1,
+        )
+        yield from loop3D(
+            ivec3(first.x, last.y, last.z),
+            ivec3(first.x, last.y, first.z + 1) - 1,
+        )
         # sides
         if self._size.y < 3:
             return
-        yield from loop3D(ivec3(first.x, first.y+1, first.z), ivec3(first.x, last.y-1, first.z) + 1)
-        yield from loop3D(ivec3(last.x,  first.y+1, first.z), ivec3(last.x,  last.y-1, first.z) + 1)
-        yield from loop3D(ivec3(last.x,  first.y+1, last.z ), ivec3(last.x,  last.y-1, last.z ) + 1)
-        yield from loop3D(ivec3(first.x, first.y+1, last.z ), ivec3(first.x, last.y-1, last.z ) + 1)
+        yield from loop3D(
+            ivec3(first.x, first.y + 1, first.z),
+            ivec3(first.x, last.y - 1, first.z) + 1,
+        )
+        yield from loop3D(
+            ivec3(last.x, first.y + 1, first.z),
+            ivec3(last.x, last.y - 1, first.z) + 1,
+        )
+        yield from loop3D(
+            ivec3(last.x, first.y + 1, last.z),
+            ivec3(last.x, last.y - 1, last.z) + 1,
+        )
+        yield from loop3D(
+            ivec3(first.x, first.y + 1, last.z),
+            ivec3(first.x, last.y - 1, last.z) + 1,
+        )
 
 
-def rectSlice(array: np.ndarray, rect: Rect):
+def rectSlice(array: np.ndarray, rect: Rect) -> np.ndarray:
     """Returns the slice from [array] defined by [rect]"""
-    return array[rect.begin.x:rect.end.x, rect.begin.y:rect.end.y]
+    return array[rect.begin.x : rect.end.x, rect.begin.y : rect.end.y]
 
 
-def setRectSlice(array: np.ndarray, rect: Rect, value: Any):
+def setRectSlice(array: np.ndarray, rect: Rect, value: Any) -> None:
     """Sets the slice from [array] defined by [rect] to [value]"""
-    array[rect.begin.x:rect.end.x, rect.begin.y:rect.end.y] = value
+    array[rect.begin.x : rect.end.x, rect.begin.y : rect.end.y] = value
 
 
-def boxSlice(array: np.ndarray, box: Box):
+def boxSlice(array: np.ndarray, box: Box) -> np.ndarray:
     """Returns the slice from [array] defined by [box]"""
-    return array[box.begin.x:box.end.x, box.begin.y:box.end.y, box.begin.z:box.end.z]
+    return array[box.begin.x : box.end.x, box.begin.y : box.end.y, box.begin.z : box.end.z]
 
 
-def setBoxSlice(array: np.ndarray, box: Box, value: Any):
+def setBoxSlice(array: np.ndarray, box: Box, value: Any) -> None:
     """Sets the slice from [array] defined by [box] to [value]"""
-    array[box.begin.x:box.end.x, box.begin.y:box.end.y, box.begin.z:box.end.z] = value
+    array[box.begin.x : box.end.x, box.begin.y : box.end.y, box.begin.z : box.end.z] = value
 
 
 # ==================================================================================================
 # Point generation
 # ==================================================================================================
 
 
-def loop2D(begin: Vec2iLike, end: Optional[Vec2iLike] = None):
+def loop2D(begin: Vec2iLike, end: Optional[Vec2iLike] = None) -> Generator[ivec2, Any, None]:
     """Yields all points between <begin> and <end> (end-exclusive).\n
     If <end> is not given, yields all points between (0,0) and <begin>."""
-    if end is None:
-        begin, end = (0, 0), begin
+    if end is None: begin, end = (0, 0), begin
 
     for x in range(begin[0], end[0], nonZeroSign(end[0] - begin[0])):
         for y in range(begin[1], end[1], nonZeroSign(end[1] - begin[1])):
             yield ivec2(x, y)
 
 
-def loop3D(begin: Vec3iLike, end: Optional[Vec3iLike] = None):
+def loop3D(begin: Vec3iLike, end: Optional[Vec3iLike] = None) -> Generator[ivec3, Any, None]:
     """Yields all points between <begin> and <end> (end-exclusive).\n
     If <end> is not given, yields all points between (0,0,0) and <begin>."""
     if end is None:
         begin, end = (0, 0, 0), begin
 
     for x in range(begin[0], end[0], nonZeroSign(end[0] - begin[0])):
         for y in range(begin[1], end[1], nonZeroSign(end[1] - begin[1])):
             for z in range(begin[2], end[2], nonZeroSign(end[2] - begin[2])):
                 yield ivec3(x, y, z)
 
 
-def cuboid2D(corner1: Vec2iLike, corner2: Vec2iLike):
+def cuboid2D(corner1: Vec2iLike, corner2: Vec2iLike) -> Generator[ivec2, None, None]:
     """Yields all points in the rectangle between <corner1> and <corner2> (inclusive)."""
     return Rect.between(corner1, corner2).inner
 
 
-def cuboid3D(corner1: Vec3iLike, corner2: Vec3iLike):
+def cuboid3D(corner1: Vec3iLike, corner2: Vec3iLike) -> Generator[ivec3, None, None]:
     """Yields all points in the box between <corner1> and <corner2> (inclusive)."""
     return Box.between(corner1, corner2).inner
 
 
-def filled2DArray(points: Iterable[Vec2iLike], seedPoint: Vec2iLike, boundingRect: Optional[Rect] = None, includeInputPoints=True) -> np.ndarray:
+def filled2DArray(
+    points: Iterable[Vec2iLike],
+    seedPoint: Vec2iLike,
+    boundingRect: Optional[Rect] = None,
+    includeInputPoints=True,
+) -> np.ndarray:
     """Fills the shape defined by <points>, starting at <seedPoint> and returns a (n,2) numpy array
     containing the resulting points.\n
     <boundingRect> should contain all <points>. If not provided, it is calculated."""
     if boundingRect is None:
         boundingRect = Rect.bounding(points)
 
-    pointMap = np.zeros(boundingRect.size, dtype=int)
-    pointMap[tuple(np.transpose(np.fromiter(points, dtype=np.dtype((int, 2))) - np.array(boundingRect.offset)))] = 1
-    filled = skimage.segmentation.flood_fill(pointMap, tuple(ivec2(*seedPoint) - boundingRect.offset), 1, footprint=np.array([[0,1,0],[1,1,1],[0,1,0]]))
+    pointMap = np.zeros(boundingRect.size.to_tuple(), dtype=int)
+    pointMap[
+        tuple(np.transpose(np.fromiter(points, dtype=np.dtype((int, 2))) - np.array(boundingRect.offset)))] = 1
+    filled = skimage.segmentation.flood_fill(pointMap, tuple(ivec2(*seedPoint) - boundingRect.offset),1, footprint=np.array([[0, 1, 0], [1, 1, 1], [0, 1, 0]]))
     if not includeInputPoints:
         filled -= pointMap
     return np.argwhere(filled) + np.array(boundingRect.offset)
 
 
-def filled2D(points: Iterable[Vec2iLike], seedPoint: Vec2iLike, boundingRect: Optional[Rect] = None, includeInputPoints=True):
+def filled2D(
+    points: Iterable[Vec2iLike],
+    seedPoint: Vec2iLike,
+    boundingRect: Optional[Rect] = None,
+    includeInputPoints=True,
+) -> Generator[ivec2, None, None]:
     """Fills the shape defined by <points>, starting at <seedPoint> and yields the resulting points.\n
     <boundingRect> should contain all <points>. If not provided, it is calculated."""
-    return (ivec2(*point) for point in filled2DArray(points, seedPoint, boundingRect, includeInputPoints))
+    return (
+        ivec2(*point)
+        for point in filled2DArray(points, seedPoint, boundingRect, includeInputPoints)
+    )
 
 
-def filled3DArray(points: Iterable[Vec3iLike], seedPoint: Vec3iLike, boundingBox: Optional[Box] = None, includeInputPoints=True) -> np.ndarray:
+def filled3DArray(
+    points: Iterable[Vec3iLike],
+    seedPoint: Vec3iLike,
+    boundingBox: Optional[Box] = None,
+    includeInputPoints=True,
+) -> np.ndarray:
     """Fills the shape defined by <points>, starting at <seedPoint> and returns a (n,3) numpy array
     containing the resulting points.\n
     <boundingBox> should contain all <points>. If not provided, it is calculated."""
     if boundingBox is None:
         boundingBox = Box.bounding(points)
 
-    pointMap = np.zeros(boundingBox.size, dtype=int)
+    pointMap = np.zeros(boundingBox.size.to_tuple(), dtype=int)
     pointMap[tuple(np.transpose(np.fromiter(points, dtype=np.dtype((int, 3))) - np.array(boundingBox.offset)))] = 1
     filled = skimage.segmentation.flood_fill(pointMap, tuple(ivec3(*seedPoint) - boundingBox.offset), 1, connectivity=1)
     if not includeInputPoints:
         filled -= pointMap
     return np.argwhere(filled) + np.array(boundingBox.offset)
 
 
-def filled3D(points: Iterable[Vec3iLike], seedPoint: Vec3iLike, boundingBox: Optional[Box] = None, includeInputPoints=True):
+def filled3D(
+    points: Iterable[Vec3iLike],
+    seedPoint: Vec3iLike,
+    boundingBox: Optional[Box] = None,
+    includeInputPoints=True,
+) -> Generator[ivec3, None, None]:
     """Fills the shape defined by <points>, starting at <seedPoint> and yields the resulting points.\n
     <boundingBox> should contain all <points>. If not provided, it is calculated."""
-    return (ivec3(*point) for point in filled3DArray(points, seedPoint, boundingBox, includeInputPoints))
+    return (
+        ivec3(*point)
+        for point in filled3DArray(points, seedPoint, boundingBox, includeInputPoints)
+    )
 
 
 # TODO: separate out thickening code?
 def _lineArray(begin: Union[Vec2iLike, Vec3iLike], end: Union[Vec2iLike, Vec3iLike], width: int = 1) -> np.ndarray:
-    begin: np.ndarray = np.array(begin)
-    end:   np.ndarray = np.array(end)
+    begin = np.array(begin)
+    end = np.array(end)
     delta = end - begin
     maxDelta = int(max(abs(delta)))
     if maxDelta == 0:
         return np.array([])
-    points = delta[np.newaxis,:] * np.arange(maxDelta + 1)[:,np.newaxis] / maxDelta + np.array(begin)
+    points = delta[np.newaxis, :] * np.arange(maxDelta + 1)[:, np.newaxis] / maxDelta + np.array(begin)
     points = np.rint(points).astype(np.signedinteger)
 
     if width > 1:
         minPoint = np.minimum(begin, end)
 
         # convert point array to a map
-        array_width = maxDelta + width*2
-        array = np.zeros([array_width]*len(begin), dtype=int)
+        array_width: int = maxDelta + width * 2
+        array = np.zeros([array_width] * len(begin), dtype=int)
         array[tuple(np.transpose(points - minPoint + width))] = 1
 
-        # dilate map (make it thick)
-        if width > 1:
-            array = ndimage.binary_dilation(array, iterations = width - 1)
+        array = ndimage.binary_dilation(array, iterations=width - 1)
 
         # rebuild point array from map
         points = np.argwhere(array) + minPoint - width
 
     return points
 
 
-def line2DArray(begin: Vec2iLike, end: Vec2iLike, width: int = 1):
+def line2DArray(begin: Vec2iLike, end: Vec2iLike, width: int = 1) -> np.ndarray:
     """Returns (n,2) numpy array of points on the line between [begin] and [end] (inclusive)"""
     return _lineArray(begin, end, width)
 
 
-def line2D(begin: Vec2iLike, end: Vec2iLike, width: int = 1):
+def line2D(begin: Vec2iLike, end: Vec2iLike, width: int = 1) -> Generator[ivec2, None, None]:
     """Yields the points on the line between [begin] and [end] (inclusive)"""
     return (ivec2(*point) for point in _lineArray(begin, end, width))
 
 
-def line3Darray(begin: Vec3iLike, end: Vec3iLike, width: int = 1):
+def line3Darray(begin: Vec3iLike, end: Vec3iLike, width: int = 1) -> np.ndarray:
     """Returns (n,3) numpy array of points on the line between [begin] and [end] (inclusive)"""
     return _lineArray(begin, end, width)
 
 
-def line3D(begin: Vec3iLike, end: Vec3iLike, width: int = 1):
+def line3D(begin: Vec3iLike, end: Vec3iLike, width: int = 1) -> Generator[ivec3, None, None]:
     """Yields the points on the line between [begin] and [end] (inclusive)"""
     return (ivec3(*point) for point in _lineArray(begin, end, width))
 
 
-def lineSequence2D(points: Iterable[Vec2iLike], closed=False):
+def lineSequence2D(points: Iterable[Vec2iLike], closed=False) -> Generator[ivec2, Any, None]:
     """Yields all points on the lines that connect <points>"""
     pointList = list(points)
-    for i in range((-1 if closed else 0), len(pointList)-1):
-        yield from line2D(pointList[i], pointList[i+1])
+    for i in range((-1 if closed else 0), len(pointList) - 1):
+        yield from line2D(pointList[i], pointList[i + 1])
 
 
-def lineSequence3D(points: Iterable[Vec3iLike], closed=False):
+def lineSequence3D(points: Iterable[Vec3iLike], closed=False) -> Generator[ivec3, Any, None]:
     """Yields all points on the lines that connect <points>"""
     pointList = list(points)
-    for i in range((-1 if closed else 0), len(pointList)-1):
-        yield from line3D(pointList[i], pointList[i+1])
+    for i in range((-1 if closed else 0), len(pointList) - 1):
+        yield from line3D(pointList[i], pointList[i + 1])
 
 
 def circle(center: Vec2iLike, diameter: int, filled=False):
     """Yields the points of the specified circle.\n
     If <diameter> is even, <center> will be the bottom left center point."""
 
     # With 'inspiration' from:
     # https://www.geeksforgeeks.org/bresenhams-circle-drawing-algorithm/
 
     center: ivec2 = ivec2(*center)
 
     if diameter == 0:
         empty: List[ivec2] = []
-        return (point for point in empty)
+        return iter(empty)
 
-    e = 1 - (diameter % 2) # for even centers
+    e: int = 1 - (diameter % 2)  # for even centers
     points: Set[ivec2] = set()
 
     def eightPoints(x: int, y: int):
         points.add(center + ivec2(e + x, e + y))
         points.add(center + ivec2(0 - x, e + y))
         points.add(center + ivec2(e + x, 0 - y))
         points.add(center + ivec2(0 - x, 0 - y))
         points.add(center + ivec2(e + y, e + x))
         points.add(center + ivec2(0 - y, e + x))
         points.add(center + ivec2(e + y, 0 - x))
         points.add(center + ivec2(0 - y, 0 - x))
 
-    radius = (diameter-1) // 2
+    radius: int = (diameter - 1) // 2
     x, y = 0, radius
-    d = 3 - 2 * radius
+    d: int = 3 - 2 * radius
     eightPoints(x, y)
     while y >= x:
         # for each pixel we will
         # draw all eight pixels
 
         x += 1
 
@@ -910,86 +1122,91 @@
             y -= 1
             d = d + 4 * (x - y) + 10
         else:
             d = d + 4 * x + 6
         eightPoints(x, y)
 
     if filled:
-        return filled2D(points, center, Rect(center - radius, ivec2(diameter, diameter)))
-    return (point for point in points)
+        return filled2D(
+            points, center, Rect(center - radius, ivec2(diameter, diameter))
+        )
+    return iter(points)
 
 
 def fittingCircle(corner1: Vec2iLike, corner2: Vec2iLike, filled=False):
     """Yields the points of the largest circle that fits between <corner1> and <corner2>.\n
     The circle will be centered in the larger axis."""
     corner1_, corner2_ = orderedCorners2D(corner1, corner2)
-    diameter = min(corner2_ - corner1_) + 1
+    diameter: int = min(corner2_ - corner1_) + 1
     return circle((corner1_ + corner2_) // 2, diameter, filled)
 
 
 def ellipse(center: Vec2iLike, diameters: Vec2iLike, filled=False):
     """Yields the points of the specified ellipse.\n
     If <diameter>[axis] is even, <center>[axis] will be the lower center point in that axis."""
 
     # Modified version 'inspired' by chandan_jnu from
     # https://www.geeksforgeeks.org/midpoint-ellipse-drawing-algorithm/
 
-    center:    ivec2 = ivec2(*center)
+    center: ivec2 = ivec2(*center)
     diameters: ivec2 = ivec2(*diameters)
 
     if diameters.x == 0 or diameters.y == 0:
         empty: List[ivec2] = []
-        return (point for point in empty)
+        return iter(empty)
 
     if diameters.x == diameters.y:
         return circle(center, diameters.x, filled)
 
-    e = 1 - (diameters % 2)
+    e: ivec2 = 1 - (diameters % 2)
 
     points: Set[ivec2] = set()
 
-    def fourpoints(x, y):
+    def fourpoints(x, y) -> None:
         points.add(center + ivec2(e.x + x, e.y + y))
-        points.add(center + ivec2(0   - x, e.y + y))
-        points.add(center + ivec2(e.x + x, 0   - y))
-        points.add(center + ivec2(0   - x, 0   - y))
+        points.add(center + ivec2(    - x, e.y + y))
+        points.add(center + ivec2(e.x + x,     - y))
+        points.add(center + ivec2(    - x,     - y))
 
         if filled:
-            points.update(line2D(center + ivec2(0 - x, e.y + y), center + ivec2(e.x + x, e.y + y)))
-            points.update(line2D(center + ivec2(0 - x, 0   - y), center + ivec2(e.x + x, 0   - y)))
+            points.update(line2D(center + ivec2(-x, e.y + y), center + ivec2(e.x + x, e.y + y)))
+            points.update(line2D(center + ivec2(-x,     - y), center + ivec2(e.x + x,     - y)))
 
-    rx, ry = (diameters-1) // 2
+    rx, ry = (diameters - 1) // 2
 
     x, y = 0, ry
 
     # Initial decision parameter of region 1
-    d1 = ((ry * ry) - (rx * rx * ry) + (0.25 * rx * rx))
-    dx = 2 * ry * ry * x
-    dy = 2 * rx * rx * y
+    d1: float = (ry**2) - (rx**2 * ry) + (0.25 * rx**2)
+    dx: int = 2 * ry**2 * x
+    dy: int = 2 * rx**2 * y
 
     # For region 1
     while dx < dy:
         fourpoints(x, y)
 
         # Checking and updating value of
         # decision parameter based on algorithm
         if d1 < 0:
             x += 1
-            dx = dx + (2 * ry * ry)
-            d1 = d1 + dx + (ry * ry)
+            dx += (2 * ry**2)
+            d1 += dx + (ry**2)
         else:
             x += 1
             y -= 1
-            dx = dx + (2 * ry * ry)
-            dy = dy - (2 * rx * rx)
-            d1 = d1 + dx - dy + (ry * ry)
+            dx += (2 * ry**2)
+            dy -= (2 * rx**2)
+            d1 = d1 + dx - dy + (ry**2)
 
     # Decision parameter of region 2
-    d2 = (((ry * ry) * ((x + 0.5) * (x + 0.5)))
-          + ((rx * rx) * ((y - 1) * (y - 1))) - (rx * rx * ry * ry))
+    d2: float = (
+        ((ry**2) * ((x + 0.5) * (x + 0.5)))
+        + ((rx**2) * ((y - 1) * (y - 1)))
+        - (rx**2 * ry**2)
+    )
 
     # Plotting points of region 2
     while y >= 0:
         fourpoints(x, y)
 
         # Checking and updating parameter
         # value based on algorithm
@@ -1000,105 +1217,126 @@
         else:
             y -= 1
             x += 1
             dx = dx + (2 * ry * ry)
             dy = dy - (2 * rx * rx)
             d2 = d2 + dx - dy + (rx * rx)
 
-    return (point for point in points)
+    return iter(points)
 
 
 def fittingEllipse(corner1: Vec2iLike, corner2: Vec2iLike, filled=False):
     """Yields the points of the largest ellipse that fits between <corner1> and <corner2>."""
     _corner1, _corner2 = orderedCorners2D(corner1, corner2)
-    diameters = (_corner2 - _corner1) + 1
+    diameters: ivec2 = (_corner2 - _corner1) + 1
     return ellipse((_corner1 + _corner2) // 2, diameters, filled)
 
 
-def cylinder(baseCenter: Vec3iLike, diameters: Union[Vec2iLike, int], length: int, axis=1, tube=False, hollow=False):
+def cylinder(
+    baseCenter: Vec3iLike,
+    diameters: Union[Vec2iLike, int],
+    length: int,
+    axis=1,
+    tube=False,
+    hollow=False,
+):
     """Yields the points from the specified cylinder.\n
     If a <diameter> is even, <center> will be the lower center point in that axis.\n
     <tube> has precedence over <hollow>."""
 
-    diameters:  ivec2 = ivec2(diameters) if isinstance(diameters, int) else ivec2(*diameters)
+    diameters: ivec2 = (
+        ivec2(diameters) if isinstance(diameters, int) else ivec2(*diameters)
+    )
     baseCenter: ivec3 = ivec3(*baseCenter)
 
     if diameters.x == 0 or diameters.y == 0 or length == 0:
         empty: List[ivec3] = []
-        return (point for point in empty)
+        return iter(empty)
 
-    corner1 = baseCenter - addDimension((diameters-1)/2, axis, 0)
-    corner2 = corner1 + addDimension(diameters-1, axis, length-1)
+    corner1 = baseCenter - addDimension((diameters - 1) / 2, axis, 0)
+    corner2 = corner1 + addDimension(diameters - 1, axis, length - 1)
     return fittingCylinder(corner1, corner2, axis, tube, hollow)
 
 
-def fittingCylinder(corner1: Vec3iLike, corner2: Vec3iLike, axis=1, tube=False, hollow=False):
+def fittingCylinder(
+    corner1: Vec3iLike, corner2: Vec3iLike, axis=1, tube=False, hollow=False
+):
     """Yields the points of the largest cylinder that fits between <corner1> and <corner2>.\n
     <tube> has precedence over <hollow>."""
 
     _corner1, _corner2 = orderedCorners3D(corner1, corner2)
     dimensionality, flatSides = getDimensionality(_corner1, _corner2)
 
     if dimensionality == 0:
         yield _corner1
         return
 
-    if (dimensionality == 1 or (dimensionality == 2 and flatSides[0] != axis)):
+    if dimensionality == 1 or (dimensionality == 2 and flatSides[0] != axis):
         yield from cuboid3D(_corner1, _corner2)
         return
 
-    baseCorner1 = dropDimension(_corner1, axis)
-    baseCorner2 = dropDimension(_corner2, axis)
-    h0 = _corner1[axis]
-    hn = _corner2[axis]
+    baseCorner1: ivec2 = dropDimension(_corner1, axis)
+    baseCorner2: ivec2 = dropDimension(_corner2, axis)
+    h0: int = _corner1[axis]
+    hn: int = _corner2[axis]
 
     ellipsePoints2D = list(fittingEllipse(baseCorner1, baseCorner2, filled=False))
-    ellipsePoints3D = [addDimension(point, axis, h0) for point in ellipsePoints2D]
+    ellipsePoints3D: List[ivec3] = [addDimension(point, axis, h0) for point in ellipsePoints2D]
 
-    if tube:
-        basePoints = ellipsePoints3D
-        bodyPoints = ellipsePoints3D
-    else:
-        basePoints = [addDimension(point, axis, h0) for point in filled2D(ellipsePoints2D, (baseCorner1 + baseCorner2) // 2, Rect.between(baseCorner1, baseCorner2))]
+    basePoints: List[ivec3] = ellipsePoints3D
+    bodyPoints: List[ivec3] = ellipsePoints3D
+
+    if not tube:
+        basePoints = [
+            addDimension(point, axis, h0)
+            for point in filled2D(
+                ellipsePoints2D,
+                (baseCorner1 + baseCorner2) // 2,
+                Rect.between(baseCorner1, baseCorner2),
+            )
+        ]
         bodyPoints = ellipsePoints3D if hollow else basePoints
 
     yield from basePoints
     if hn != h0:
-        direction = ivec3(0,0,0)
+        direction = ivec3(0, 0, 0)
         direction[axis] = 1
-        yield from (point + (hn - h0)*direction for point in basePoints)
-        yield from (point + i*direction for i in range(1, hn-h0) for point in bodyPoints)
+        yield from (point + (hn - h0) * direction for point in basePoints)
+        yield from (
+            point + i * direction
+            for i in range(1, hn - h0)
+            for point in bodyPoints
+        )
 
 
-def ellipsoid(center: Vec3iLike, diameters: Vec3iLike, hollow: bool = False):
+def ellipsoid(center: Vec3iLike, diameters: Vec3iLike, hollow: bool = False) -> Generator[ivec3, Any, None]:
     """Yields the points of an ellipsoid centered on <center> with diameters <diameters>.\n
     If <diameter>[axis] is even, <center>[axis] will be the lower center point in that axis."""
 
     # Convert the center and diameters to ivec3
     center: ivec3 = ivec3(*center)
     diameters: ivec3 = ivec3(*diameters)
 
     # Calculate the correction
-    e = 1 - (diameters % 2)
+    e: ivec3 = 1 - (diameters % 2)
 
-    def are_points_in_line(center: Vec3iLike, point: Vec3iLike):
+    def are_points_in_line(center: Vec3iLike, point: Vec3iLike) -> bool:
         """Checks if two 3D points are the same on 2 or more axis"""
         count = 0
         for i in range(3):
-            if point[i] == center[i]:
-                count += 1
+            if point[i] == center[i]: count += 1
         return count >= 2
 
-    def generate_octants(center: Vec3iLike, point: Vec3iLike):
+    def generate_octants(center: Vec3iLike, point: Vec3iLike) -> List[ivec3]:
         """Generates octants for a point around a center"""
         x0, y0, z0 = center
         x, y, z = point
         dx, dy, dz = x - x0, y - y0, z - z0
 
-        octants = [
+        octants: List[ivec3] = [
             ivec3(x0 + e.x + dx, y0 + e.y + dy, z0 + e.z + dz),
             ivec3(x0       - dx, y0 + e.y + dy, z0 + e.z + dz),
             ivec3(x0 + e.x + dx, y0       - dy, z0 + e.z + dz),
             ivec3(x0       - dx, y0       - dy, z0 + e.z + dz),
             ivec3(x0 + e.x + dx, y0 + e.y + dy, z0       - dz),
             ivec3(x0       - dx, y0 + e.y + dy, z0       - dz),
             ivec3(x0 + e.x + dx, y0       - dy, z0       - dz),
@@ -1108,144 +1346,143 @@
         return octants
 
     # Extract the x, y, and z coordinates of the center point
     x0, y0, z0 = center
     # Extract the radii of the ellipsoid along the x, y, and z axes
     rx, ry, rz = ((diameters) // 2) + (1 - e)
 
-    solid_points = np.zeros((rx + 2, ry + 2, rz + 2), dtype=bool)
+    solid_points: np.ndarray[Any, np.dtype[bool]] = np.zeros((rx + 2, ry + 2, rz + 2), dtype=bool)
 
     # Loop over all points within the bounding box of the ellipsoid
-    for x in range(solid_points.shape[0]):
-        for y in range(solid_points.shape[1]):
-            for z in range(solid_points.shape[2]):
-
-                # Compute the ellipsoid equation for the current point
-                e_val = (
-                    (x ** 2 / rx**2)
-                    + (y ** 2 / ry**2)
-                    + (z ** 2 / rz**2)
-                )
-                # Check if it is in-line with the center point
-                in_line_with_center = are_points_in_line(center, (x + x0, y + y0, z + z0))
+    for x, y, z in iterproduct(*(range(n) for n in solid_points.shape)):
 
-                # If the point satisfies the ellipsoid equation
-                if e_val <= 1 and (not in_line_with_center or e_val < 1):
-                    # If it should be hollow, add the point to the point array
-                    if hollow:
-                        solid_points[x, y, z] = True
-                    # Otherwise, yield it for all octants
-                    else:
-                        yield from generate_octants(center, ivec3(x + x0, y + y0, z + z0))
+        # Compute the ellipsoid equation for the current point
+        e_val: float = (x**2 / rx**2) + (y**2 / ry**2) + (z**2 / rz**2)
+        # Check if it is in-line with the center point
+        in_line_with_center: bool = are_points_in_line(
+            center, (x + x0, y + y0, z + z0)
+        )
+
+        # If the point satisfies the ellipsoid equation
+        if e_val <= 1 and (not in_line_with_center or e_val < 1):
+            # If it should be hollow, add the point to the point array
+            if hollow: solid_points[x, y, z] = True
+            # Otherwise, yield it for all octants
+            else:
+                yield from generate_octants(
+                    center, ivec3(x + x0, y + y0, z + z0)
+                )
 
     # If the ellipsoid should be hollow
     if hollow:
         # Iterate through every point in the array, except the outer faces
-        for x in range(solid_points.shape[0] - 1):
-            for y in range(solid_points.shape[1] - 1):
-                for z in range(solid_points.shape[2] - 1):
-
-                    # A point is considered part of the "shell" if it meets the following conditions: (Thanks to @Jandhi#5234 on discord)
-                    # - It is part of the solid ellipsoid
-                    # - At least one of it's adjacent points isn't (we only have to check 3/6 because of octants)
-                    shell = solid_points[x, y, z] and (
-                        not solid_points[x + 1, y, z] or
-                        not solid_points[x, y + 1, z] or
-                        not solid_points[x, y, z + 1]
-                    )
-
-                    # If a point is part of the shell, yield it for all octants
-                    if shell:
-                        yield from generate_octants(center, ivec3(x + x0, y + y0, z + z0))
+        for x, y, z in iterproduct(*(range(n-1) for n in solid_points.shape)):
+
+            # A point is considered part of the "shell" if it meets the following conditions: (Thanks to @Jandhi#5234 on discord)
+            # - It is part of the solid ellipsoid
+            # - At least one of it's adjacent points isn't (we only have to check 3/6 because of octants)
+            shell: bool = solid_points[x, y, z] and (
+                not solid_points[x + 1, y, z]
+                or not solid_points[x, y + 1, z]
+                or not solid_points[x, y, z + 1]
+            )
 
+            # If a point is part of the shell, yield it for all octants
+            if shell: yield from generate_octants(center, ivec3(x + x0, y + y0, z + z0))
 
-def fittingEllipsoid(corner1: Vec3iLike, corner2: Vec3iLike, hollow: bool = False):
+
+def fittingEllipsoid(corner1: Vec3iLike, corner2: Vec3iLike, hollow: bool = False) -> Generator[ivec3, Any, None]:
     """Yields the points of the largest ellipsoid that fits between <corner1> and <corner2>."""
     corner1_, corner2_ = orderedCorners3D(corner1, corner2)
-    diameters = corner2_ - corner1_ + 1
-    center = (corner1_ + corner2_) // 2
+    diameters: ivec3 = corner2_ - corner1_ + 1
+    center: ivec3 = (corner1_ + corner2_) // 2
     return ellipsoid(center, diameters, hollow)
 
 
-def sphere(center: Vec3iLike, diameter: int, hollow: bool = False):
+def sphere(center: Vec3iLike, diameter: int, hollow: bool = False) -> Generator[ivec3, Any, None]:
     """Yields the points of a sphere centered on <center> with diameter <diameter>.\n
     If <diameter> is even, <center> will be the lower center point in every axis."""
     return ellipsoid(center, (diameter, diameter, diameter), hollow)
 
 
-def fittingSphere(corner1: Vec3iLike, corner2: Vec3iLike, hollow: bool = False):
+def fittingSphere(corner1: Vec3iLike, corner2: Vec3iLike, hollow: bool = False) -> Generator[ivec3, Any, None]:
     """Yields the points of the largest sphere that fits between <corner1> and <corner2>.\n
     The circle will be centered in the non-minimum axes."""
     corner1_, corner2_ = orderedCorners3D(corner1, corner2)
-    diameter = min(corner2_ - corner1_) + 1
-    center = (corner1_ + corner2_) // 2
+    diameter: int = min(corner2_ - corner1_) + 1
+    center: ivec3 = (corner1_ + corner2_) // 2
     return sphere(center, diameter, hollow)
 
 
-def neighbors2D(point: Vec2iLike, boundingRect: Rect, diagonal: bool = False, stride: int = 1):
+def neighbors2D(point: Vec2iLike, boundingRect: Rect, diagonal: bool = False, stride: int = 1) -> Generator[ivec2, Any, None]:
     """Yields the neighbors of [point] within [bounding_rect].\n
     Useful for pathfinding."""
 
-    end = boundingRect.end
+    if type(point) is not ivec2:
+        point = ivec2(*point)
 
-    left  = point[0] - stride >= boundingRect.offset.x
-    down  = point[1] - stride >= boundingRect.offset.y
-    right = point[0] + stride <  end.x
-    up    = point[1] + stride <  end.y
-
-    if left:   yield ivec2(point[0] - stride, point[1]         )
-    if down:   yield ivec2(point[0]         , point[1] - stride)
-    if right:  yield ivec2(point[0] + stride, point[1]         )
-    if up:     yield ivec2(point[0]         , point[1] + stride)
+    end: ivec2 = boundingRect.end
 
-    if not diagonal:
-        return
+    west:  bool = point[0] - stride >= boundingRect.offset.x
+    north: bool = point[1] - stride >= boundingRect.offset.y
+    east:  bool = point[0] + stride <  end.x
+    south: bool = point[1] + stride <  end.y
+
+    if west:  yield point + stride * WEST_2D
+    if north: yield point + stride * NORTH_2D
+    if east:  yield point + stride * EAST_2D
+    if south: yield point + stride * SOUTH_2D
 
-    if left  and down: yield ivec2(point[0] - stride, point[1] - stride)
-    if left  and up:   yield ivec2(point[0] - stride, point[1] + stride)
-    if right and down: yield ivec2(point[0] + stride, point[1] - stride)
-    if right and up:   yield ivec2(point[0] + stride, point[1] + stride)
+    if not diagonal: return
 
+    if west and north: yield point + stride * (WEST_2D + NORTH_2D)
+    if west and south: yield point + stride * (WEST_2D + SOUTH_2D)
+    if east and north: yield point + stride * (EAST_2D + NORTH_2D)
+    if east and south: yield point + stride * (EAST_2D + SOUTH_2D)
 
-def neighbors3D(point: Vec3iLike, boundingBox: Box, diagonal: bool = False, stride: int = 1):
+
+def neighbors3D(point: Vec3iLike, boundingBox: Box, diagonal: bool = False, stride: int = 1) -> Generator[ivec3, Any, None]:
     """Yields the neighbors of [point] within [bounding_box].\n
     Useful for pathfinding."""
 
-    end = boundingBox.end
-
-    left  = point[0] - stride >= boundingBox.offset.x
-    down  = point[1] - stride >= boundingBox.offset.y
-    back  = point[2] - stride >= boundingBox.offset.z
-    right = point[0] + stride <  end.x
-    up    = point[1] + stride <  end.y
-    front = point[2] + stride <  end.z
-
-    if left:  yield ivec3(point[0] - stride, point[1]         , point[2]         )
-    if down:  yield ivec3(point[0]         , point[1] - stride, point[2]         )
-    if back:  yield ivec3(point[0]         , point[1]         , point[2] - stride)
-    if right: yield ivec3(point[0] + stride, point[1]         , point[2]         )
-    if up:    yield ivec3(point[0]         , point[1] + stride, point[2]         )
-    if front: yield ivec3(point[0]         , point[1]         , point[2] + stride)
+    if type(point) is not ivec3:
+        point = ivec3(*point)
 
-    if not diagonal:
-        return
+    end: ivec3 = boundingBox.end
 
-    if left  and down:           yield ivec3(point[0] - stride, point[1] - stride, point[2]         )
-    if left  and back:           yield ivec3(point[0] - stride, point[1]         , point[2] - stride)
-    if left  and up:             yield ivec3(point[0] - stride, point[1] + stride, point[2]         )
-    if left  and front:          yield ivec3(point[0] - stride, point[1]         , point[2] + stride)
-    if right and down:           yield ivec3(point[0] + stride, point[1] - stride, point[2]         )
-    if right and back:           yield ivec3(point[0] + stride, point[1]         , point[2] - stride)
-    if right and up:             yield ivec3(point[0] + stride, point[1] + stride, point[2]         )
-    if right and front:          yield ivec3(point[0] + stride, point[1]         , point[2] + stride)
-    if down  and back:           yield ivec3(point[0]         , point[1] - stride, point[2] - stride)
-    if down  and front:          yield ivec3(point[0]         , point[1] - stride, point[2] + stride)
-    if up    and back:           yield ivec3(point[0]         , point[1] + stride, point[2] - stride)
-    if up    and front:          yield ivec3(point[0]         , point[1] + stride, point[2] + stride)
-    if left  and down and back:  yield ivec3(point[0] - stride, point[1] - stride, point[2] - stride)
-    if left  and down and front: yield ivec3(point[0] - stride, point[1] - stride, point[2] + stride)
-    if left  and up   and back:  yield ivec3(point[0] - stride, point[1] + stride, point[2] - stride)
-    if left  and up   and front: yield ivec3(point[0] - stride, point[1] + stride, point[2] + stride)
-    if right and down and back:  yield ivec3(point[0] + stride, point[1] - stride, point[2] - stride)
-    if right and down and front: yield ivec3(point[0] + stride, point[1] - stride, point[2] + stride)
-    if right and up   and back:  yield ivec3(point[0] + stride, point[1] + stride, point[2] - stride)
-    if right and up   and front: yield ivec3(point[0] + stride, point[1] + stride, point[2] + stride)
+    west:  bool = point[0] - stride >= boundingBox.offset.x
+    down:  bool = point[1] - stride >= boundingBox.offset.y
+    north: bool = point[2] - stride >= boundingBox.offset.z
+    east:  bool = point[0] + stride <  end.x
+    up:    bool = point[1] + stride <  end.y
+    south: bool = point[2] + stride <  end.z
+
+
+    if west:  yield point + stride * WEST_3D
+    if down:  yield point + stride * DOWN_3D
+    if north: yield point + stride * NORTH_3D
+    if east:  yield point + stride * EAST_3D
+    if up:    yield point + stride * UP_3D
+    if south: yield point + stride * SOUTH_3D
+
+    if not diagonal: return
+
+    if west and down          : yield point + stride * (WEST_3D + DOWN_3D           )
+    if west and up            : yield point + stride * (WEST_3D + UP_3D             )
+    if east and down          : yield point + stride * (EAST_3D + DOWN_3D           )
+    if east and up            : yield point + stride * (EAST_3D + UP_3D             )
+    if west          and north: yield point + stride * (WEST_3D           + NORTH_3D)
+    if west          and south: yield point + stride * (WEST_3D           + SOUTH_3D)
+    if east          and north: yield point + stride * (EAST_3D           + NORTH_3D)
+    if east          and south: yield point + stride * (EAST_3D           + SOUTH_3D)
+    if          down and north: yield point + stride * (          DOWN_3D + NORTH_3D)
+    if          down and south: yield point + stride * (          DOWN_3D + SOUTH_3D)
+    if          up   and north: yield point + stride * (          UP_3D   + NORTH_3D)
+    if          up   and south: yield point + stride * (          UP_3D   + SOUTH_3D)
+    if west and down and north: yield point + stride * (WEST_3D + DOWN_3D + NORTH_3D)
+    if west and down and south: yield point + stride * (WEST_3D + DOWN_3D + SOUTH_3D)
+    if west and up   and north: yield point + stride * (WEST_3D + UP_3D   + NORTH_3D)
+    if west and up   and south: yield point + stride * (WEST_3D + UP_3D   + SOUTH_3D)
+    if east and down and north: yield point + stride * (EAST_3D + UP_3D   + NORTH_3D)
+    if east and down and south: yield point + stride * (EAST_3D + DOWN_3D + SOUTH_3D)
+    if east and up   and north: yield point + stride * (EAST_3D + UP_3D   + NORTH_3D)
+    if east and up   and south: yield point + stride * (EAST_3D + UP_3D   + SOUTH_3D)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gdpc-7.1.0/gdpc/world_slice.py` & `gdpc-7.2.0/src/gdpc/world_slice.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.1.0/gdpc.egg-info/PKG-INFO` & `gdpc-7.2.0/src/gdpc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: gdpc
-Version: 7.1.0
+Version: 7.2.0
 Summary: The Generative Design Python Client (GDPC) is a Python-based interface for the Minecraft GDMC HTTP Interface mod.\nIt was created for use in the Generative Design in Minecraft Competition (GDMC).
 Home-page: https://github.com/avdstaaij/gdpc
 Author: Arthur van der Staaij, Blinkenlights, Nils Gawlik
 Author-email: arthurvanderstaaij@gmail.com, blinkenlights@pm.me, nilsgawlik@gmx.de
 Maintainer: Arthur van der Staaij
 Maintainer-email: arthurvanderstaaij@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/avdstaaij/gdpc/issues
 Project-URL: Changelog, https://github.com/avdstaaij/gdpc/blob/master/CHANGELOG.md
-Project-URL: Official Competition Website, https://gendesignmc.engineering.nyu.edu
+Project-URL: Official Competition wiki, https://gendesignmc.wikidot.com/start
 Project-URL: Chat about it on Discord, https://discord.gg/YwpPCRQWND
 Project-URL: Source, https://github.com/avdstaaij/gdpc
 Keywords: GDMC,generative design,Minecraft,HTTP,development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -37,15 +37,15 @@
 Requires-Dist: scipy
 Requires-Dist: termcolor
 Requires-Dist: typing_extensions
 
 # GDPC
 
 GDPC (Generative Design Python Client) is a Python framework for use in conjunction with the [GDMC-HTTP](https://github.com/Niels-NTG/gdmc_http_interface) mod for Minecraft Java edition.
-It is designed for the [Generative Design in Minecraft Competition (GDMC)](https://gendesignmc.engineering.nyu.edu).
+It is designed for the [Generative Design in Minecraft Competition (GDMC)](https://gendesignmc.wikidot.com/start).
 
 You need to be playing in a Minecraft world with the mod installed to use the framework.
 
 The latest version of GDPC is compatible with GDMC-HTTP versions **>=1.0.0, <2.0.0** and Minecraft **1.20.2** (see [note](#note-on-supported-minecraft-version)).
 
 
 ## Quick example
@@ -65,15 +65,15 @@
 geometry.placeCuboid(editor, (0,80,2), (2,82,4), Block("oak_planks"))
 ```
 
 ## What's the difference between GDMC, GDMC-HTTP and GDPC?
 
 These abbreviations are all very similar, but refer to different things.
 
-**GDMC:** Short for the [Generative Design in Minecraft Competition](https://gendesignmc.engineering.nyu.edu), a yearly competition for generative AI systems in Minecraft.
+**GDMC:** Short for the [Generative Design in Minecraft Competition](https://gendesignmc.wikidot.com/start), a yearly competition for generative AI systems in Minecraft.
 The challenge is to write an algorithm that creates a settlement while adapting to the pre-existing terrain. The competition also has a [Discord server](https://discord.gg/YwpPCRQWND).
 
 **GDMC-HTTP:** A [Minecraft Forge mod](https://github.com/Niels-NTG/gdmc_http_interface) that provides a HTTP interface to edit the world.
 It allows you to modify the world live, while you're playing in it. This makes it possible to iterate quickly on generator algorithms.
 The mod is an official submission method for the competition.
 
 **GDPC:** This repository (notice the "P"). A Python framework for interacting with the GDMC-HTTP interface.
```

### Comparing `gdpc-7.1.0/setup.py` & `gdpc-7.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import setup
 
 
 SCRIPT_DIR         = os.path.abspath(os.path.dirname(__file__))
-METADATA_FILE_PATH = os.path.join(SCRIPT_DIR, "gdpc/__init__.py")
+METADATA_FILE_PATH = os.path.join(SCRIPT_DIR, "src/gdpc/__init__.py")
 
 
 # Based on https://github.com/pypa/pip/blob/9aa422da16e11b8e56d3597f34551f983ba9fbfd/setup.py
 def get_metadata(name: str) -> str:
     with open(METADATA_FILE_PATH) as file:
         contents = file.read()
     for line in contents.splitlines():
@@ -32,14 +32,15 @@
     url                           = get_metadata("url"),
     author                        = get_metadata("author"),
     author_email                  = get_metadata("author_email"),
     maintainer                    = get_metadata("maintainer"),
     maintainer_email              = get_metadata("maintainer_email"),
     license                       = get_metadata("license"),
     packages = ["gdpc"], # Note: subpackages must be listed explicitly
+    package_dir={"": "src"},
     install_requires=[
         "matplotlib",
         "more-itertools",
         "NBT",
         "numpy",
         "opencv_python",
         "PyGLM >= 2.7.0",
@@ -61,13 +62,14 @@
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Version Control :: Git",
     ],
     keywords="GDMC, generative design, Minecraft, HTTP, development",
     project_urls={
         "Bug Reports":                  "https://github.com/avdstaaij/gdpc/issues",
         "Changelog":                    "https://github.com/avdstaaij/gdpc/blob/master/CHANGELOG.md",
-        "Official Competition Website": "https://gendesignmc.engineering.nyu.edu",
+        # "Official Competition Website": "https://gendesignmc.engineering.nyu.edu",
+        "Official Competition wiki":    "https://gendesignmc.wikidot.com/start",
         "Chat about it on Discord":     "https://discord.gg/YwpPCRQWND",
         "Source":                       "https://github.com/avdstaaij/gdpc",
     },
     zip_safe=False
 )
```

