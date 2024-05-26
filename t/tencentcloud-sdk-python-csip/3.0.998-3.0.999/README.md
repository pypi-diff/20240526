# Comparing `tmp/tencentcloud-sdk-python-csip-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-csip-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-csip-3.0.998.tar", last modified: Fri Oct 13 00:25:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-csip-3.0.999.tar", last modified: Mon Oct 16 00:24:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-csip-3.0.998.tar` & `tencentcloud-sdk-python-csip-3.0.999.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud/csip/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud/csip/v20221121/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud/csip/v20221121/__init__.py
--rw-r--r--   0 root         (0) root         (0)   341879 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud/csip/v20221121/models.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud/csip/v20221121/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28721 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud/csip/v20221121/csip_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud/csip/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud_sdk_python_csip.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud_sdk_python_csip.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud_sdk_python_csip.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud_sdk_python_csip.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      506 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud_sdk_python_csip.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/tencentcloud_sdk_python_csip.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/README.rst
--rw-r--r--   0 root         (0) root         (0)       88 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1074 2023-10-13 00:25:15.000000 tencentcloud-sdk-python-csip-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud/csip/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud/csip/v20221121/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud/csip/v20221121/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   342265 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud/csip/v20221121/models.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud/csip/v20221121/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28721 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud/csip/v20221121/csip_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud/csip/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud_sdk_python_csip.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud_sdk_python_csip.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud_sdk_python_csip.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud_sdk_python_csip.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      506 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud_sdk_python_csip.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/tencentcloud_sdk_python_csip.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/README.rst
+-rw-r--r--   0 root         (0) root         (0)       88 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-10-16 00:24:27.000000 tencentcloud-sdk-python-csip-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-csip-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-csip-3.0.999/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.998'
+__version__ = '3.0.999'
```

### Comparing `tencentcloud-sdk-python-csip-3.0.998/tencentcloud/csip/v20221121/models.py` & `tencentcloud-sdk-python-csip-3.0.999/tencentcloud/csip/v20221121/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3347,26 +3347,29 @@
         :type ScanPlanType: int
         :param _Assets: 扫描资产信息列表
         :type Assets: list of TaskAssetObject
         :param _ScanPlanContent: 扫描计划详情
         :type ScanPlanContent: str
         :param _SelfDefiningAssets: ip/域名/url数组
         :type SelfDefiningAssets: list of str
+        :param _ScanFrom: 请求发起源，默认为vss表示漏洞扫描服务，云安全中心的用户请填充csip
+        :type ScanFrom: str
         :param _TaskAdvanceCFG: 高级配置
         :type TaskAdvanceCFG: :class:`tencentcloud.csip.v20221121.models.TaskAdvanceCFG`
         :param _TaskMode: 体检模式，0-标准模式，1-快速模式，2-高级模式，默认标准模式
         :type TaskMode: int
         """
         self._TaskName = None
         self._ScanAssetType = None
         self._ScanItem = None
         self._ScanPlanType = None
         self._Assets = None
         self._ScanPlanContent = None
         self._SelfDefiningAssets = None
+        self._ScanFrom = None
         self._TaskAdvanceCFG = None
         self._TaskMode = None
 
     @property
     def TaskName(self):
         return self._TaskName
 
@@ -3419,14 +3422,22 @@
         return self._SelfDefiningAssets
 
     @SelfDefiningAssets.setter
     def SelfDefiningAssets(self, SelfDefiningAssets):
         self._SelfDefiningAssets = SelfDefiningAssets
 
     @property
+    def ScanFrom(self):
+        return self._ScanFrom
+
+    @ScanFrom.setter
+    def ScanFrom(self, ScanFrom):
+        self._ScanFrom = ScanFrom
+
+    @property
     def TaskAdvanceCFG(self):
         return self._TaskAdvanceCFG
 
     @TaskAdvanceCFG.setter
     def TaskAdvanceCFG(self, TaskAdvanceCFG):
         self._TaskAdvanceCFG = TaskAdvanceCFG
 
@@ -3448,14 +3459,15 @@
             self._Assets = []
             for item in params.get("Assets"):
                 obj = TaskAssetObject()
                 obj._deserialize(item)
                 self._Assets.append(obj)
         self._ScanPlanContent = params.get("ScanPlanContent")
         self._SelfDefiningAssets = params.get("SelfDefiningAssets")
+        self._ScanFrom = params.get("ScanFrom")
         if params.get("TaskAdvanceCFG") is not None:
             self._TaskAdvanceCFG = TaskAdvanceCFG()
             self._TaskAdvanceCFG._deserialize(params.get("TaskAdvanceCFG"))
         self._TaskMode = params.get("TaskMode")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
```

### Comparing `tencentcloud-sdk-python-csip-3.0.998/tencentcloud/csip/v20221121/errorcodes.py` & `tencentcloud-sdk-python-csip-3.0.999/tencentcloud/csip/v20221121/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csip-3.0.998/tencentcloud/csip/v20221121/csip_client.py` & `tencentcloud-sdk-python-csip-3.0.999/tencentcloud/csip/v20221121/csip_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csip-3.0.998/tencentcloud_sdk_python_csip.egg-info/PKG-INFO` & `tencentcloud-sdk-python-csip-3.0.999/tencentcloud_sdk_python_csip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csip
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Csip SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csip-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-csip-3.0.999/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csip
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Csip SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csip-3.0.998/README.rst` & `tencentcloud-sdk-python-csip-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csip-3.0.998/setup.py` & `tencentcloud-sdk-python-csip-3.0.999/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-csip',
-    install_requires=["tencentcloud-sdk-python-common==3.0.998"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.999"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Csip SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

