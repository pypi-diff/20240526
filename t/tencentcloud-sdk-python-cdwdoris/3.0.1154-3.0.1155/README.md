# Comparing `tmp/tencentcloud-sdk-python-cdwdoris-3.0.1154.tar.gz` & `tmp/tencentcloud-sdk-python-cdwdoris-3.0.1155.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdwdoris-3.0.1154.tar", last modified: Thu May 23 20:27:06 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdwdoris-3.0.1155.tar", last modified: Sun May 26 20:34:30 2024, max compression
```

## Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1154.tar` & `tencentcloud-sdk-python-cdwdoris-3.0.1155.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud/cdwdoris/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud/cdwdoris/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud/cdwdoris/v20211228/
--rw-r--r--   0 root         (0) root         (0)    16479 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud/cdwdoris/v20211228/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud/cdwdoris/v20211228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   132125 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud/cdwdoris/v20211228/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud_sdk_python_cdwdoris.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud_sdk_python_cdwdoris.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud_sdk_python_cdwdoris.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud_sdk_python_cdwdoris.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      550 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1685 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/README.rst
--rw-r--r--   0 root         (0) root         (0)     1083 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1685 2024-05-23 20:27:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1154/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud/cdwdoris/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud/cdwdoris/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud/cdwdoris/v20211228/
+-rw-r--r--   0 root         (0) root         (0)    16479 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud/cdwdoris/v20211228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud/cdwdoris/v20211228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   132418 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud/cdwdoris/v20211228/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud_sdk_python_cdwdoris.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud_sdk_python_cdwdoris.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud_sdk_python_cdwdoris.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud_sdk_python_cdwdoris.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      550 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-05-26 20:34:30.000000 tencentcloud-sdk-python-cdwdoris-3.0.1155/PKG-INFO
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1154'
+__version__ = '3.0.1155'
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud/cdwdoris/v20211228/errorcodes.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud/cdwdoris/v20211228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud/cdwdoris/v20211228/models.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud/cdwdoris/v20211228/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2137,24 +2137,27 @@
         :type Sql: str
         :param _ReadRows: 排序参数
         :type ReadRows: str
         :param _ResultBytes: 排序参数
         :type ResultBytes: str
         :param _MemoryUsage: 排序参数
         :type MemoryUsage: str
+        :param _IsQuery: IsQuery条件
+        :type IsQuery: int
         """
         self._InstanceId = None
         self._QueryDurationMs = None
         self._StartTime = None
         self._EndTime = None
         self._DurationMs = None
         self._Sql = None
         self._ReadRows = None
         self._ResultBytes = None
         self._MemoryUsage = None
+        self._IsQuery = None
 
     @property
     def InstanceId(self):
         return self._InstanceId
 
     @InstanceId.setter
     def InstanceId(self, InstanceId):
@@ -2220,25 +2223,34 @@
     def MemoryUsage(self):
         return self._MemoryUsage
 
     @MemoryUsage.setter
     def MemoryUsage(self, MemoryUsage):
         self._MemoryUsage = MemoryUsage
 
+    @property
+    def IsQuery(self):
+        return self._IsQuery
+
+    @IsQuery.setter
+    def IsQuery(self, IsQuery):
+        self._IsQuery = IsQuery
+
 
     def _deserialize(self, params):
         self._InstanceId = params.get("InstanceId")
         self._QueryDurationMs = params.get("QueryDurationMs")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._DurationMs = params.get("DurationMs")
         self._Sql = params.get("Sql")
         self._ReadRows = params.get("ReadRows")
         self._ResultBytes = params.get("ResultBytes")
         self._MemoryUsage = params.get("MemoryUsage")
+        self._IsQuery = params.get("IsQuery")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1154/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdwdoris-3.0.1155/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwdoris
-Version: 3.0.1154
+Version: 3.0.1155
 Summary: Tencent Cloud Cdwdoris SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1154/README.rst` & `tencentcloud-sdk-python-cdwdoris-3.0.1155/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1154/setup.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1155/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cdwdoris',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1154"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1155"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cdwdoris SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1154/PKG-INFO` & `tencentcloud-sdk-python-cdwdoris-3.0.1155/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwdoris
-Version: 3.0.1154
+Version: 3.0.1155
 Summary: Tencent Cloud Cdwdoris SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

