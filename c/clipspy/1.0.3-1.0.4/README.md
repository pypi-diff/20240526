# Comparing `tmp/clipspy-1.0.3.tar.gz` & `tmp/clipspy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipspy-1.0.3.tar", last modified: Sun Feb 18 21:47:40 2024, max compression
+gzip compressed data, was "clipspy-1.0.4.tar", last modified: Sun May 26 20:03:22 2024, max compression
```

## Comparing `clipspy-1.0.3.tar` & `clipspy-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-18 21:47:40.903352 clipspy-1.0.3/
--rw-r--r--   0 runner     (501) staff       (20)     1490 2024-02-18 21:45:52.000000 clipspy-1.0.3/LICENSE.txt
--rw-r--r--   0 runner     (501) staff       (20)       30 2024-02-18 21:45:52.000000 clipspy-1.0.3/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     3650 2024-02-18 21:47:40.903134 clipspy-1.0.3/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3088 2024-02-18 21:45:52.000000 clipspy-1.0.3/README.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-18 21:47:40.898793 clipspy-1.0.3/clips/
--rw-r--r--   0 runner     (501) staff       (20)     2474 2024-02-18 21:45:52.000000 clipspy-1.0.3/clips/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12531 2024-02-18 21:45:52.000000 clipspy-1.0.3/clips/agenda.py
--rw-r--r--   0 runner     (501) staff       (20)    28087 2024-02-18 21:45:52.000000 clipspy-1.0.3/clips/classes.py
--rw-r--r--   0 runner     (501) staff       (20)     2364 2024-02-18 21:45:52.000000 clipspy-1.0.3/clips/clips_build.py
--rw-r--r--   0 runner     (501) staff       (20)     7437 2024-02-18 21:45:52.000000 clipspy-1.0.3/clips/common.py
--rw-r--r--   0 runner     (501) staff       (20)     6501 2024-02-18 21:45:52.000000 clipspy-1.0.3/clips/environment.py
--rw-r--r--   0 runner     (501) staff       (20)    20255 2024-02-18 21:45:53.000000 clipspy-1.0.3/clips/facts.py
--rw-r--r--   0 runner     (501) staff       (20)    15175 2024-02-18 21:45:53.000000 clipspy-1.0.3/clips/functions.py
--rw-r--r--   0 runner     (501) staff       (20)     8139 2024-02-18 21:45:53.000000 clipspy-1.0.3/clips/modules.py
--rw-r--r--   0 runner     (501) staff       (20)     9674 2024-02-18 21:45:53.000000 clipspy-1.0.3/clips/routers.py
--rw-r--r--   0 runner     (501) staff       (20)     6285 2024-02-18 21:45:53.000000 clipspy-1.0.3/clips/values.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-18 21:47:40.902477 clipspy-1.0.3/clipspy.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3650 2024-02-18 21:47:40.000000 clipspy-1.0.3/clipspy.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      415 2024-02-18 21:47:40.000000 clipspy-1.0.3/clipspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-02-18 21:47:40.000000 clipspy-1.0.3/clipspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       12 2024-02-18 21:47:40.000000 clipspy-1.0.3/clipspy.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       13 2024-02-18 21:47:40.000000 clipspy-1.0.3/clipspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-18 21:47:40.901821 clipspy-1.0.3/lib/
--rw-r--r--   0 runner     (501) staff       (20)    21860 2024-02-18 21:45:53.000000 clipspy-1.0.3/lib/clips.cdef
--rw-r--r--   0 runner     (501) staff       (20)      107 2024-02-18 21:47:40.903924 clipspy-1.0.3/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     2819 2024-02-18 21:45:53.000000 clipspy-1.0.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 20:03:22.619621 clipspy-1.0.4/
+-rw-r--r--   0 runner     (501) staff       (20)     1490 2024-05-26 20:02:35.000000 clipspy-1.0.4/LICENSE.txt
+-rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-26 20:02:35.000000 clipspy-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     3650 2024-05-26 20:03:22.619029 clipspy-1.0.4/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3088 2024-05-26 20:02:35.000000 clipspy-1.0.4/README.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 20:03:22.614357 clipspy-1.0.4/clips/
+-rw-r--r--   0 runner     (501) staff       (20)     2474 2024-05-26 20:02:35.000000 clipspy-1.0.4/clips/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12636 2024-05-26 20:02:35.000000 clipspy-1.0.4/clips/agenda.py
+-rw-r--r--   0 runner     (501) staff       (20)    28087 2024-05-26 20:02:35.000000 clipspy-1.0.4/clips/classes.py
+-rw-r--r--   0 runner     (501) staff       (20)     2364 2024-05-26 20:02:35.000000 clipspy-1.0.4/clips/clips_build.py
+-rw-r--r--   0 runner     (501) staff       (20)     7437 2024-05-26 20:02:35.000000 clipspy-1.0.4/clips/common.py
+-rw-r--r--   0 runner     (501) staff       (20)     6501 2024-05-26 20:02:35.000000 clipspy-1.0.4/clips/environment.py
+-rw-r--r--   0 runner     (501) staff       (20)    20255 2024-05-26 20:02:35.000000 clipspy-1.0.4/clips/facts.py
+-rw-r--r--   0 runner     (501) staff       (20)    15175 2024-05-26 20:02:35.000000 clipspy-1.0.4/clips/functions.py
+-rw-r--r--   0 runner     (501) staff       (20)     8139 2024-05-26 20:02:35.000000 clipspy-1.0.4/clips/modules.py
+-rw-r--r--   0 runner     (501) staff       (20)     9674 2024-05-26 20:02:35.000000 clipspy-1.0.4/clips/routers.py
+-rw-r--r--   0 runner     (501) staff       (20)     6285 2024-05-26 20:02:35.000000 clipspy-1.0.4/clips/values.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 20:03:22.618385 clipspy-1.0.4/clipspy.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3650 2024-05-26 20:03:22.000000 clipspy-1.0.4/clipspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      415 2024-05-26 20:03:22.000000 clipspy-1.0.4/clipspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-26 20:03:22.000000 clipspy-1.0.4/clipspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       12 2024-05-26 20:03:22.000000 clipspy-1.0.4/clipspy.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       13 2024-05-26 20:03:22.000000 clipspy-1.0.4/clipspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 20:03:22.617651 clipspy-1.0.4/lib/
+-rw-r--r--   0 runner     (501) staff       (20)    21860 2024-05-26 20:02:35.000000 clipspy-1.0.4/lib/clips.cdef
+-rw-r--r--   0 runner     (501) staff       (20)      107 2024-05-26 20:03:22.620252 clipspy-1.0.4/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     2819 2024-05-26 20:02:35.000000 clipspy-1.0.4/setup.py
```

### Comparing `clipspy-1.0.3/LICENSE.txt` & `clipspy-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clipspy-1.0.3/PKG-INFO` & `clipspy-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipspy
-Version: 1.0.3
+Version: 1.0.4
 Summary: CLIPS Python bindings
 Home-page: https://github.com/noxdafox/clipspy
 Author: Matteo Cafasso
 Author-email: noxdafox@gmail.com
 License: BSD
 Keywords: clips python cffi expert-system
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clipspy-1.0.3/README.rst` & `clipspy-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `clipspy-1.0.3/clips/__init__.py` & `clipspy-1.0.4/clips/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE,
 # EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 __author__ = 'Matteo Cafasso'
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 __license__ = 'BSD-3'
 
 
 __all__ = ('CLIPSError',
            'Environment',
            'Router',
            'LoggingRouter',
```

### Comparing `clipspy-1.0.3/clips/agenda.py` & `clipspy-1.0.4/clips/agenda.py`

 * *Files 4% similar despite different names*

```diff
@@ -272,17 +272,21 @@
     @property
     def focus(self) -> Module:
         """The module associated with the current focus.
 
         Equivalent to the CLIPS (get-focus) function.
 
         """
-        name = ffi.string(lib.DefmoduleName(lib.GetFocus(self._env))).decode()
+        current_focus = lib.GetFocus(self._env)
+        if current_focus != ffi.NULL:
+            name = ffi.string(lib.DefmoduleName(current_focus)).decode()
 
-        return Module(self._env, name)
+            return Module(self._env, name)
+
+        return None
 
     @focus.setter
     def focus(self, module: Module):
         """The module associated with the current focus.
 
         Equivalent to the CLIPS (get-focus) function.
```

### Comparing `clipspy-1.0.3/clips/classes.py` & `clipspy-1.0.4/clips/classes.py`

 * *Files identical despite different names*

### Comparing `clipspy-1.0.3/clips/clips_build.py` & `clipspy-1.0.4/clips/clips_build.py`

 * *Files identical despite different names*

### Comparing `clipspy-1.0.3/clips/common.py` & `clipspy-1.0.4/clips/common.py`

 * *Files identical despite different names*

### Comparing `clipspy-1.0.3/clips/environment.py` & `clipspy-1.0.4/clips/environment.py`

 * *Files identical despite different names*

### Comparing `clipspy-1.0.3/clips/facts.py` & `clipspy-1.0.4/clips/facts.py`

 * *Files identical despite different names*

### Comparing `clipspy-1.0.3/clips/functions.py` & `clipspy-1.0.4/clips/functions.py`

 * *Files identical despite different names*

### Comparing `clipspy-1.0.3/clips/modules.py` & `clipspy-1.0.4/clips/modules.py`

 * *Files identical despite different names*

### Comparing `clipspy-1.0.3/clips/routers.py` & `clipspy-1.0.4/clips/routers.py`

 * *Files identical despite different names*

### Comparing `clipspy-1.0.3/clips/values.py` & `clipspy-1.0.4/clips/values.py`

 * *Files identical despite different names*

### Comparing `clipspy-1.0.3/clipspy.egg-info/PKG-INFO` & `clipspy-1.0.4/clipspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipspy
-Version: 1.0.3
+Version: 1.0.4
 Summary: CLIPS Python bindings
 Home-page: https://github.com/noxdafox/clipspy
 Author: Matteo Cafasso
 Author-email: noxdafox@gmail.com
 License: BSD
 Keywords: clips python cffi expert-system
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clipspy-1.0.3/lib/clips.cdef` & `clipspy-1.0.4/lib/clips.cdef`

 * *Files identical despite different names*

### Comparing `clipspy-1.0.3/setup.py` & `clipspy-1.0.4/setup.py`

 * *Files identical despite different names*

