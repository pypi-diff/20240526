# Comparing `tmp/pyremotechrome-0.1.1.tar.gz` & `tmp/pyremotechrome-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyremotechrome-0.1.1.tar", last modified: Sat May 25 05:58:27 2024, max compression
+gzip compressed data, was "pyremotechrome-0.1.2.tar", last modified: Sun May 26 09:48:54 2024, max compression
```

## Comparing `pyremotechrome-0.1.1.tar` & `pyremotechrome-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,42 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:58:27.628933 pyremotechrome-0.1.1/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.1.1/LICENSE
--rw-r--r--   0 wes       (1000) wes       (1000)      979 2024-05-25 05:58:27.624933 pyremotechrome-0.1.1/PKG-INFO
--rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.1.1/README.md
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:58:27.604933 pyremotechrome-0.1.1/dist/
--rw-rw-r--   0 wes       (1000) wes       (1000)    40160 2024-05-24 16:20:02.000000 pyremotechrome-0.1.1/dist/pyremotechrome-0.0.16-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)    26002 2024-05-24 16:20:00.000000 pyremotechrome-0.1.1/dist/pyremotechrome-0.0.16.tar.gz
--rw-rw-r--   0 wes       (1000) wes       (1000)    93722 2024-05-25 05:51:18.000000 pyremotechrome-0.1.1/dist/pyremotechrome-0.1.0-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)    80215 2024-05-25 05:51:00.000000 pyremotechrome-0.1.1/dist/pyremotechrome-0.1.0.tar.gz
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1094 2024-05-25 05:58:21.000000 pyremotechrome-0.1.1/pyproject.toml
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:58:27.608933 pyremotechrome-0.1.1/pyremotechrome/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.1.1/pyremotechrome/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1846 2024-05-24 06:21:51.000000 pyremotechrome-0.1.1/pyremotechrome/__main__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:58:27.612933 pyremotechrome-0.1.1/pyremotechrome/config/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1131 2024-05-24 04:08:11.000000 pyremotechrome-0.1.1/pyremotechrome/config/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2099 2024-05-25 05:57:55.000000 pyremotechrome-0.1.1/pyremotechrome/config/config.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:58:27.616933 pyremotechrome-0.1.1/pyremotechrome/server/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.1.1/pyremotechrome/server/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.1.1/pyremotechrome/server/favicon.ico
--rw-rw-r--   0 wes       (1000) wes       (1000)     8051 2024-05-24 09:03:10.000000 pyremotechrome-0.1.1/pyremotechrome/server/manager.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     5228 2024-05-24 03:50:21.000000 pyremotechrome-0.1.1/pyremotechrome/server/server.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:58:27.616933 pyremotechrome-0.1.1/pyremotechrome/session/
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1179 2024-05-24 03:49:59.000000 pyremotechrome-0.1.1/pyremotechrome/session/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)    17071 2024-05-24 15:55:35.000000 pyremotechrome-0.1.1/pyremotechrome/session/base.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     2942 2024-05-24 16:19:20.000000 pyremotechrome-0.1.1/pyremotechrome/session/mega.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:58:27.620933 pyremotechrome-0.1.1/pyremotechrome/session/monitor/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.1.1/pyremotechrome/session/monitor/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     7026 2024-05-24 12:41:55.000000 pyremotechrome-0.1.1/pyremotechrome/session/monitor/audio.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     5258 2024-05-24 11:01:10.000000 pyremotechrome-0.1.1/pyremotechrome/session/monitor/display.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:58:27.600933 pyremotechrome-0.1.1/pyremotechrome/session/support/
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:58:27.620933 pyremotechrome-0.1.1/pyremotechrome/session/support/common/
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1344 2024-05-24 03:49:59.000000 pyremotechrome-0.1.1/pyremotechrome/session/support/common/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     2435 2024-05-24 03:49:59.000000 pyremotechrome-0.1.1/pyremotechrome/session/support/common/directory.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1752 2024-05-24 03:49:59.000000 pyremotechrome-0.1.1/pyremotechrome/session/support/common/info.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1451 2024-05-24 03:49:59.000000 pyremotechrome-0.1.1/pyremotechrome/session/support/common/result.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1713 2024-05-24 03:49:59.000000 pyremotechrome-0.1.1/pyremotechrome/session/support/common/vector.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:58:27.624933 pyremotechrome-0.1.1/pyremotechrome/session/support/options/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1167 2024-05-24 03:49:59.000000 pyremotechrome-0.1.1/pyremotechrome/session/support/options/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1493 2024-05-24 03:49:59.000000 pyremotechrome-0.1.1/pyremotechrome/session/support/options/ffmpeg.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     3524 2024-05-24 09:05:03.000000 pyremotechrome-0.1.1/pyremotechrome/util.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:58:27.624933 pyremotechrome-0.1.1/pyremotechrome/wave/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-22 09:17:54.000000 pyremotechrome-0.1.1/pyremotechrome/wave/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      396 2024-05-22 11:11:18.000000 pyremotechrome-0.1.1/pyremotechrome/wave/index.html
--rw-rw-r--   0 wes       (1000) wes       (1000)   882078 2024-05-21 11:12:02.000000 pyremotechrome-0.1.1/pyremotechrome/wave/loop.wav
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-25 05:58:27.624933 pyremotechrome-0.1.1/pyremotechrome.egg-info/
--rw-r--r--   0 wes       (1000) wes       (1000)      979 2024-05-25 05:58:27.000000 pyremotechrome-0.1.1/pyremotechrome.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1308 2024-05-25 05:58:27.000000 pyremotechrome-0.1.1/pyremotechrome.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-25 05:58:27.000000 pyremotechrome-0.1.1/pyremotechrome.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-25 05:58:27.000000 pyremotechrome-0.1.1/pyremotechrome.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-25 05:58:27.000000 pyremotechrome-0.1.1/pyremotechrome.egg-info/top_level.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-25 05:58:27.628933 pyremotechrome-0.1.1/setup.cfg
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.072851 pyremotechrome-0.1.2/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.1.2/LICENSE
+-rw-r--r--   0 wes       (1000) wes       (1000)      979 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/PKG-INFO
+-rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.1.2/README.md
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1094 2024-05-26 09:47:54.000000 pyremotechrome-0.1.2/pyproject.toml
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.064851 pyremotechrome-0.1.2/pyremotechrome/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.1.2/pyremotechrome/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1846 2024-05-24 06:21:51.000000 pyremotechrome-0.1.2/pyremotechrome/__main__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.064851 pyremotechrome-0.1.2/pyremotechrome/config/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1131 2024-05-24 04:08:11.000000 pyremotechrome-0.1.2/pyremotechrome/config/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2099 2024-05-25 05:57:55.000000 pyremotechrome-0.1.2/pyremotechrome/config/config.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/pyremotechrome/server/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.1.2/pyremotechrome/server/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.1.2/pyremotechrome/server/favicon.ico
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7348 2024-05-26 09:19:02.000000 pyremotechrome-0.1.2/pyremotechrome/server/manager.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4635 2024-05-26 06:59:33.000000 pyremotechrome-0.1.2/pyremotechrome/server/server.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/pyremotechrome/session/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1179 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)    16367 2024-05-26 09:35:44.000000 pyremotechrome-0.1.2/pyremotechrome/session/base.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     2893 2024-05-26 09:19:08.000000 pyremotechrome-0.1.2/pyremotechrome/session/mega.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/pyremotechrome/session/monitor/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.1.2/pyremotechrome/session/monitor/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7026 2024-05-26 06:59:48.000000 pyremotechrome-0.1.2/pyremotechrome/session/monitor/audio.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     7462 2024-05-26 09:26:18.000000 pyremotechrome-0.1.2/pyremotechrome/session/monitor/display.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.064851 pyremotechrome-0.1.2/pyremotechrome/session/support/
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/pyremotechrome/session/support/common/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1344 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/common/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     2435 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/common/directory.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1752 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/common/info.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1451 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/common/result.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1713 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/common/vector.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/pyremotechrome/session/support/options/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1167 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/options/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1493 2024-05-24 03:49:59.000000 pyremotechrome-0.1.2/pyremotechrome/session/support/options/ffmpeg.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     3797 2024-05-26 04:51:07.000000 pyremotechrome-0.1.2/pyremotechrome/util.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-26 09:48:54.068851 pyremotechrome-0.1.2/pyremotechrome.egg-info/
+-rw-r--r--   0 wes       (1000) wes       (1000)      979 2024-05-26 09:48:54.000000 pyremotechrome-0.1.2/pyremotechrome.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1062 2024-05-26 09:48:54.000000 pyremotechrome-0.1.2/pyremotechrome.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-26 09:48:54.000000 pyremotechrome-0.1.2/pyremotechrome.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-26 09:48:54.000000 pyremotechrome-0.1.2/pyremotechrome.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-26 09:48:54.000000 pyremotechrome-0.1.2/pyremotechrome.egg-info/top_level.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-26 09:48:54.072851 pyremotechrome-0.1.2/setup.cfg
```

### Comparing `pyremotechrome-0.1.1/LICENSE` & `pyremotechrome-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/PKG-INFO` & `pyremotechrome-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyRemoteChrome
 Author-email: Wes-KW <dotdotdashdash2024@hotmail.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyremotechrome-0.1.1/pyproject.toml` & `pyremotechrome-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [metadata]
 name = "pyremotechrome"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.setuptools.packages]
 find = {}  # Scan the project directory with the default parameters
 
 [tool.setuptools.package-data]
 "*" = ["*.*"] # Include resources
 
 [project]
 name = "pyremotechrome"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Wes-KW", email="dotdotdashdash2024@hotmail.com" },
 ]
 dependencies = [
   "selenium>=4.19.0",
   "psutil>=5.9.8",
   "PyVirtualDisplay>=3.0",
```

### Comparing `pyremotechrome-0.1.1/pyremotechrome/__main__.py` & `pyremotechrome-0.1.2/pyremotechrome/__main__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/pyremotechrome/config/__init__.py` & `pyremotechrome-0.1.2/pyremotechrome/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/pyremotechrome/config/config.py` & `pyremotechrome-0.1.2/pyremotechrome/config/config.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/pyremotechrome/server/favicon.ico` & `pyremotechrome-0.1.2/pyremotechrome/server/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/pyremotechrome/server/manager.py` & `pyremotechrome-0.1.2/pyremotechrome/server/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-from inspect import signature
+from ast import literal_eval
 from urllib.parse import urlparse
 from urllib.parse import parse_qs
 from pyremotechrome.config import Conf
 from pyremotechrome.session import MegaBase
 from pyremotechrome.session.support.common import Directory
 from pyremotechrome.session.support.common import Vector
 from pyremotechrome.session.support.common import Result
 from pyremotechrome.session.support.options import FFMpegOptions
 from pyremotechrome.util import print_exception
 from pyremotechrome.util import get_value_in_dict
 from pyremotechrome.util import filter_rules
+from pyremotechrome.util import atob
 
 # load the following from config.json
 c = Conf()
 
 # Session
 session = c.session
 size = session.size
@@ -61,31 +62,28 @@
 __AUDIO_ITSOFFSET__ = ffmpeg.audio_itsoffset
 __MAXRATE__ = ffmpeg.maxrate
 __BUFSIZE__ = ffmpeg.bufsize
 __CRF__ = ffmpeg.constant_rate_factor
 
 # Server
 server = c.server
-url = server.url
-__WAVE_URL__ = f"{url.scheme}://{url.name}:{url.port}/wave/"
 __DEBUG__ = server.debug
 
 
 class RemoteSession(MegaBase):
 
     def __init__(self, id: str, user_agent: str = __USER_AGENT__) -> None:
 
         super().__init__(
             id=id,
             scale=__DEFAULT_SCALE__,
             data_dir=f"{__DATA_DIR__}/{id}",
             default_url=__DEFAULT_URL__,
             size=Vector(__DEFAULT_WIDTH__, __DEFAULT_HEIGHT__),
             screen_size=Vector(__SCREEN_WIDTH__, __SCREEN_HEIGHT__),
-            wave_url=__WAVE_URL__,
             user_agent=user_agent,
             webdriver_exec=__WEBDRIVER_EXEC__,
             ffmpeg_options=FFMpegOptions(
                 ffmpeg_exec=__FFMPEG_EXEC__,
                 probesize=__PROBESIZE__,
                 segment_time=__SEGMENT_TIME__,
                 frame_per_second=__FRAME_PER_SEC__,
@@ -115,41 +113,27 @@
         If the Remote Session is not created, create a Remote Session and
         store it in an array. Then return a Result object with
         the first window_handle.
         """
 
         if session_id not in self._sessions:
             self._sessions[session_id] = RemoteSession(session_id)
-            window_handle = self._sessions[session_id].get_current_window_handle()
+            window_handle = self._sessions[session_id].get_current_window()
             return Result(True, "", {"window_handle": window_handle})
         else:
-            return Result(False, f"session `{session_id}` already exists.")
-
-    def get_session_info(self, session_id: str) -> Result:
-        """Return Session Result containing window_handles, _title and _icon"""
-
-        if session_id in self._sessions:
-            title = self._sessions[session_id].get_title()
-            icon = self._sessions[session_id].get_icon()
-            all_handles = self._sessions[session_id].get_window_handles()
-            spec_handles = self._sessions[session_id].spec_handles
-            handles = list(set(all_handles).difference(set(spec_handles)))
-            res = {"title": title, "icon": icon, "handles": handles, "spec_handles": spec_handles}
-            return Result(True, "", res)
-        else:
-            return Result(False, f"session `{session_id}` doesn't exists.")
+            return Result(False, "SESSION_ALREADY_CREATED")
 
     def destroy_session(self, session_id: str) -> Result:
         """DOCSTRING"""
         if session_id in self._sessions:
             self._sessions[session_id].quit()
             self._sessions.pop(session_id)
             return Result(True)
         else:
-            return Result(False, f"session `{session_id}` doesn't exist.")
+            return Result(False, "INVALID_SESSION_ID")
 
     def _call_from_url(self, url: str) -> Result:
         """DOCSTRING"""
         query = parse_qs(urlparse(url).query)
         if "request" not in query or query["request"][0] != "pyapi":
             return Result(False, "INVALID_API_REQUEST")
 
@@ -159,41 +143,48 @@
             print_exception("EMPTY_SESSION_ID")
             return Result(False, "EMPTY_SESSION_ID")
         elif action is None:
             print_exception("EMPTY_API_ACTION")
             return Result(False, "EMPTY_API_ACTION")
         else:
             action = action[0]
-            try:
-                filter_rules(action, __ACTION_ALLOW_RULES__, __ACTION_DENY_RULES__)
-            except Exception:
-                print_exception("DENIED_API_ACTION")
-                return Result(False, "DENIED_API_ACTION")
-
             session_id = session_id[0]
+
+            if action == "create_session":
+                return self.create_session(session_id)
+            elif action == "destroy_session":
+                return self.destroy_session(session_id)
+
             if session_id not in self._sessions:
                 print_exception("INVALID_SESSION_ID")
                 return Result(False, "INVALID_SESSION_ID")
 
             sess = self._sessions[session_id]
             func = getattr(sess, action, None)
+
             if not callable(func):
                 print_exception("INVALID_API_ACTION")
                 return Result(False, "INVALID_API_ACTION")
             else:
-                arguments = list(signature(func).parameters.keys())[1:]
-                for argument in arguments:
-                    if argument not in query:
-                        print_exception("INVALID_API_ACTION_PARAMETERS")
-                        return Result(False, "INVALID_API_ACTION_PARAMETERS")
+                try:
+                    filter_rules(action, __ACTION_ALLOW_RULES__, __ACTION_DENY_RULES__)
+                except Exception:
+                    print_exception("DENIED_API_ACTION")
+                    return Result(False, "DENIED_API_ACTION")                
 
                 query.pop("request")
                 query.pop("action")
+                query.pop("session_id")
+
                 for q in query:
-                    query[q] = query[q][0]
+                    query[q] = literal_eval(query[q][0])
+
+                if get_value_in_dict(query, "encoded_url") is not None:
+                    query["url"] = atob(query["encoded_url"])
+                    query.pop("encoded_url")
 
                 res = func(**query)
                 return Result(True, "" , res)
 
     def call_from_url(self, url: str) -> Result:
         """DOCSTRING"""
         try:
```

### Comparing `pyremotechrome-0.1.1/pyremotechrome/server/server.py` & `pyremotechrome-0.1.2/pyremotechrome/server/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,16 +46,15 @@
 __ICON_PATH__ = f"{__ROOT__}/server/favicon.ico"
 __WAVE_DIR__ = f"{__ROOT__}/wave/"
 
 # load the following from config.json
 c = Conf()
 
 # Server
-server = c.server
-url = server.url
+url = c.server.url
 __SERVER_SCHEME__ = url.scheme
 __SERVER_NAME__ = url.name
 __SERVER_PORT__ = url.port
 
 ips = set(url.ips)
 ips.add(f"{url.name}:{url.port}")
 __SERVER_NAMES__ = set(url.ips)
@@ -109,26 +108,14 @@
 
         elif is_http and path == "/favicon.ico":
             # Allow favicon.ico
             self.send_h(200, "image/x-icon")
             with open(__ICON_PATH__, 'rb') as f:
                 self.wfile.write(f.read())
 
-        elif is_http and path.startswith("/wave/"):
-            list = ["/wave/index.html", "/wave/"]
-            if any(path == x for x in list):
-                self.send_h(200, "text/html")
-                with open(f"{__WAVE_DIR__}/index.html", "rb") as f:
-                    self.wfile.write(f.read())
-            elif path == "/wave/loop.wav":
-                self.send_h(200, "audio/x-wav")
-                with open(f"{__WAVE_DIR__}/loop.wav", "rb") as f:
-                    self.wfile.write(f.read())
-            else:
-                self.send_h(403, "text/plain")
         else:
             # Deny permission to other files
             self.send_h(403, "text/plain")
 
     def get_url(self):
         """DOCSTRING"""
         return f"{__SERVER_SCHEME__}://{__SERVER_NAME__}:{__SERVER_PORT__}{self.path}"
```

### Comparing `pyremotechrome-0.1.1/pyremotechrome/session/__init__.py` & `pyremotechrome-0.1.2/pyremotechrome/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/pyremotechrome/session/base.py` & `pyremotechrome-0.1.2/pyremotechrome/session/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,54 +46,44 @@
     _cursor: Vector
     _position: Vector
     _border_width: Vector
     _scale: Numbers
     _data_dir: Directory
     _default_url: str
     display: BrowserDisplay
-    special_handles: list[str]
     info: Info
     allow_rules: list[str]
     deny_rules: list[str]
 
     def __init__(
         self,
         id: str,
         scale: Numbers,
         data_dir: str,
         default_url: str,
         size: Vector,
         screen_size: Vector,
-        wave_url: str,
         user_agent: str,
         webdriver_exec: str,
         ffmpeg_options: FFMpegOptions,
         allow_rules: list[str] = [],
         deny_rules: list[str] = []
     ) -> None:
 
         """Initialize a chrome with video capturing enabled"""
         if id == "":
             raise ValueError()
 
-        url = wave_url.split("/")
-        url.pop()
-        try:
-            requests_get("/".join(url), timeout=60)
-        except Exception:
-            raise Exception("SERVER_NO_RESPONSE")
-
         self._id = id
         self.info = Info()
         self._cursor = Vector(0, 0)
         self._position = Vector(0, 0)
         self._scale = scale
         self._data_dir = Directory(data_dir)
         self._default_url = default_url
-        self.special_handles = []
         self.allow_rules = allow_rules
         self.deny_rules = deny_rules
 
         _, log_dir = self._data_dir.set_dir("log", "log/ffmpeg")
         _, video_dir = self._data_dir.set_dir("video", "video")
         screen_width, screen_height = screen_size()
         screen_width = int(screen_width * self._scale)
@@ -127,28 +117,21 @@
             return [
                 w.outerWidth - w.innerWidth,
                 w.outerHeight - w.innerHeight
             ];
         """)
         bh += __CHROME_AUTOMATION_LABEL_HEIGHT__
         self._border_width = Vector(bw, bh)
-        
+
         width, height = size()
         self.set_window_size(width, height)
         self.set_window_position(0, 0)
         self.set_page_load_timeout(60)
         self.zoom()
 
-        self.get(wave_url)
-        self.left_click()
-        self.execute_script("document.getElementById('loop_player').play();")
-        self.special_handles.append(self.get_current_window())
-
-        self.set_current_window(self.open_tab())
-        self.get(self._default_url)
         self.display.init_audio(self.service.process.pid)
         self.display.init_ffmpeg(ffmpeg_options)
         self.display.start_capturing(bw, bh, width, height)
 
     # Zoom
     def zoom(self) -> None:
         super().get("chrome://settings/")
@@ -235,17 +218,15 @@
         """
         Close the tab at the specified tab_index
 
         Preconditions:
             - window_handle in self.window_handles
         """
 
-        spec_handles = set(self.special_handles)
-        non_spec_handles = set(self.window_handles).difference(spec_handles)
-        if len(non_spec_handles) > 1:
+        if len(self.window_handles) > 1:
             self.close()
         else:
             self.get(self._default_url)
 
     def quit(self, clear_cache: bool = False) -> None:
         """Quit webdriver"""
         del self.display
@@ -339,15 +320,15 @@
         """Emulate pressing a sequence of keys"""
         for keys in key_seqs:
             self.key(keys)
 
     # Copy and Paste
     def _create_clipboard(self) -> WebElement:
         """Create an invisble text_area"""
-        textarea_id = f"pyremotechrome-clipboard-{self._id}-{self.get_current_window_handle()}"
+        textarea_id = f"pyremotechrome-clipboard-{self._id}-{self.get_current_window()}"
         css_selector = f"textarea#{textarea_id}"
         try:
             self.select(css_selector)
         except NoSuchElementException:
             self.execute_script(f"""
                 input = document.createElement('textarea');
                 input.style.width = '0px';
@@ -385,17 +366,14 @@
         self.key(["", value])
 
     # Capture Screenshot
     def capture_screenshot(self) -> str:
         """
         Capture screenshot and save to the file path
         """
-        if self.get_current_window() in self.special_handles:
-            return ""
-
         display_dir, save_dir = self._data_dir.set_dir('current_window', f"cache/{self.get_current_window()}")
         display_path = f"{display_dir}/screenshot.png"
         save_path = f"{save_dir}/screenshot.png"
         self.get_screenshot_as_file(save_path)
         return display_path
 
     # DOM Element
@@ -446,19 +424,19 @@
                     handler.write(img_data)
 
                 return display_path
             except Exception:
                 # No favicon is found
                 return ""
 
-    def update_and_get_info(self) -> dict[str, dict[str, str]]:
+    def get_session_info(self) -> dict[str, dict[str, str]]:
         """reset and get title, icon and url"""
-        self.info.update("title", self.get_current_title())
-        self.info.update("icon", self.get_current_icon())
-        self.info.update("url", self.get_current_url())
+        self.info.update("title", self.current_window_handle, self.get_current_title())
+        self.info.update("icon", self.current_window_handle, self.get_current_icon())
+        self.info.update("url", self.current_window_handle, self.get_current_url())
         return self.info.to_dict()
 
     # Other methods
     def reset_audio(self) -> None:
         """DOCSTRING"""
         self.display.audio_manager.get_monitor()
```

### Comparing `pyremotechrome-0.1.1/pyremotechrome/session/mega.py` & `pyremotechrome-0.1.2/pyremotechrome/session/mega.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         self,
         id: str,
         scale: Numbers,
         data_dir: str,
         default_url: str,
         size: Vector,
         screen_size: Vector,
-        wave_url: str,
         user_agent: str,
         webdriver_exec: str,
         ffmpeg_options: FFMpegOptions,
         allow_rules: list[str] = [],
         deny_rules: list[str] = []
     ) -> None:
 
@@ -70,15 +69,14 @@
             Base(
                 id,
                 scale,
                 data_dir,
                 default_url,
                 size,
                 screen_size,
-                wave_url,
                 user_agent,
                 webdriver_exec,
                 ffmpeg_options,
                 allow_rules,
                 deny_rules
             ),
             _EventListener()
```

### Comparing `pyremotechrome-0.1.1/pyremotechrome/session/monitor/audio.py` & `pyremotechrome-0.1.2/pyremotechrome/session/monitor/audio.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/pyremotechrome/session/support/common/__init__.py` & `pyremotechrome-0.1.2/pyremotechrome/session/support/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/pyremotechrome/session/support/common/directory.py` & `pyremotechrome-0.1.2/pyremotechrome/session/support/common/directory.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/pyremotechrome/session/support/common/info.py` & `pyremotechrome-0.1.2/pyremotechrome/session/support/common/info.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/pyremotechrome/session/support/common/result.py` & `pyremotechrome-0.1.2/pyremotechrome/session/support/common/result.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/pyremotechrome/session/support/common/vector.py` & `pyremotechrome-0.1.2/pyremotechrome/session/support/common/vector.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/pyremotechrome/session/support/options/__init__.py` & `pyremotechrome-0.1.2/pyremotechrome/session/support/options/__init__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/pyremotechrome/session/support/options/ffmpeg.py` & `pyremotechrome-0.1.2/pyremotechrome/session/support/options/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.1.1/pyremotechrome/util.py` & `pyremotechrome-0.1.2/pyremotechrome/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 from __future__ import annotations
 from re import search
+from base64 import b64decode, b64encode
 from typing import Any
 from typing import Union
 from datetime import datetime
 from pytz import timezone
 from urllib.parse import urlparse
 
 
@@ -99,7 +100,15 @@
     for rule in deny_rules:
         if search(rule, arg) is not None:
             filter_arg = ""
             break
 
     if filter_arg == "" and not suppress:
         raise Exception("ARGUMENT_DENIED")
+
+def btoa(decoded: str) -> str:
+    """Encode ASCII string"""
+    return b64encode(decoded.encode("utf-8")).decode('utf-8')
+
+def atob(encoded: str) -> str:
+    """Decode base64 string"""
+    return b64decode(encoded).decode("utf-8")
```

### Comparing `pyremotechrome-0.1.1/pyremotechrome.egg-info/PKG-INFO` & `pyremotechrome-0.1.2/pyremotechrome.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyRemoteChrome
 Author-email: Wes-KW <dotdotdashdash2024@hotmail.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyremotechrome-0.1.1/pyremotechrome.egg-info/SOURCES.txt` & `pyremotechrome-0.1.2/pyremotechrome.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-dist/pyremotechrome-0.0.16-py3-none-any.whl
-dist/pyremotechrome-0.0.16.tar.gz
-dist/pyremotechrome-0.1.0-py3-none-any.whl
-dist/pyremotechrome-0.1.0.tar.gz
 pyremotechrome/__init__.py
 pyremotechrome/__main__.py
 pyremotechrome/util.py
 pyremotechrome.egg-info/PKG-INFO
 pyremotechrome.egg-info/SOURCES.txt
 pyremotechrome.egg-info/dependency_links.txt
 pyremotechrome.egg-info/requires.txt
@@ -27,11 +23,8 @@
 pyremotechrome/session/monitor/display.py
 pyremotechrome/session/support/common/__init__.py
 pyremotechrome/session/support/common/directory.py
 pyremotechrome/session/support/common/info.py
 pyremotechrome/session/support/common/result.py
 pyremotechrome/session/support/common/vector.py
 pyremotechrome/session/support/options/__init__.py
-pyremotechrome/session/support/options/ffmpeg.py
-pyremotechrome/wave/__init__.py
-pyremotechrome/wave/index.html
-pyremotechrome/wave/loop.wav
+pyremotechrome/session/support/options/ffmpeg.py
```

