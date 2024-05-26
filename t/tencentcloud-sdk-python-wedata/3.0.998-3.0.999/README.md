# Comparing `tmp/tencentcloud-sdk-python-wedata-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-wedata-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.998.tar", last modified: Fri Oct 13 00:41:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.999.tar", last modified: Mon Oct 16 00:39:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wedata-3.0.998.tar` & `tencentcloud-sdk-python-wedata-3.0.999.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud/wedata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud/wedata/v20210820/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1976966 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)     3640 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   276930 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud/wedata/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud_sdk_python_wedata.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud_sdk_python_wedata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      528 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1078 2023-10-13 00:41:06.000000 tencentcloud-sdk-python-wedata-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud/wedata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  2024031 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   284129 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud/wedata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud_sdk_python_wedata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud_sdk_python_wedata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      528 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-10-16 00:39:55.000000 tencentcloud-sdk-python-wedata-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.998/tencentcloud/wedata/v20210820/models.py` & `tencentcloud-sdk-python-wedata-3.0.999/tencentcloud/wedata/v20210820/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,14 +307,23 @@
         :type MessageId: str
         :param _Operator: 阈值计算算子，1 : 大于 2 ：小于
 注意：此字段可能返回 null，表示取不到有效值。
         :type Operator: int
         :param _RegularId: 告警规则ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegularId: str
+        :param _AlarmRecipientName: 告警接收人昵称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AlarmRecipientName: str
+        :param _TaskType: 告警任务类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskType: int
+        :param _SendResult: 发送结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SendResult: str
         """
         self._AlarmId = None
         self._AlarmTime = None
         self._TaskId = None
         self._RegularName = None
         self._AlarmLevel = None
         self._AlarmWay = None
@@ -326,14 +335,17 @@
         self._EstimatedTime = None
         self._InstanceId = None
         self._TaskName = None
         self._IsSendSuccess = None
         self._MessageId = None
         self._Operator = None
         self._RegularId = None
+        self._AlarmRecipientName = None
+        self._TaskType = None
+        self._SendResult = None
 
     @property
     def AlarmId(self):
         return self._AlarmId
 
     @AlarmId.setter
     def AlarmId(self, AlarmId):
@@ -471,14 +483,38 @@
     def RegularId(self):
         return self._RegularId
 
     @RegularId.setter
     def RegularId(self, RegularId):
         self._RegularId = RegularId
 
+    @property
+    def AlarmRecipientName(self):
+        return self._AlarmRecipientName
+
+    @AlarmRecipientName.setter
+    def AlarmRecipientName(self, AlarmRecipientName):
+        self._AlarmRecipientName = AlarmRecipientName
+
+    @property
+    def TaskType(self):
+        return self._TaskType
+
+    @TaskType.setter
+    def TaskType(self, TaskType):
+        self._TaskType = TaskType
+
+    @property
+    def SendResult(self):
+        return self._SendResult
+
+    @SendResult.setter
+    def SendResult(self, SendResult):
+        self._SendResult = SendResult
+
 
     def _deserialize(self, params):
         self._AlarmId = params.get("AlarmId")
         self._AlarmTime = params.get("AlarmTime")
         self._TaskId = params.get("TaskId")
         self._RegularName = params.get("RegularName")
         self._AlarmLevel = params.get("AlarmLevel")
@@ -491,14 +527,17 @@
         self._EstimatedTime = params.get("EstimatedTime")
         self._InstanceId = params.get("InstanceId")
         self._TaskName = params.get("TaskName")
         self._IsSendSuccess = params.get("IsSendSuccess")
         self._MessageId = params.get("MessageId")
         self._Operator = params.get("Operator")
         self._RegularId = params.get("RegularId")
+        self._AlarmRecipientName = params.get("AlarmRecipientName")
+        self._TaskType = params.get("TaskType")
+        self._SendResult = params.get("SendResult")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -7942,17 +7981,17 @@
 class CreateCustomFunctionRequest(AbstractModel):
     """CreateCustomFunction请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Type: 类型：HIVE、SPARK
+        :param _Type: 枚举值：HIVE、SPARK、DLC
         :type Type: str
-        :param _Kind: 分类：窗口函数、聚合函数、日期函数......
+        :param _Kind: 枚举值：ANALYSIS(函数)、ENCRYPTION(加密函数)、AGGREGATE(聚合函数)、LOGIC(逻辑函数)、DATE_AND_TIME(日期与时间函数)、MATH(数学函数)、CONVERSION(转换函数)、STRING(字符串函数)、IP_AND_DOMAIN(IP和域名函数)、WINDOW(窗口函数)、OTHER(其他函数)
         :type Kind: str
         :param _Name: 函数名称
         :type Name: str
         :param _ClusterIdentifier: 集群实例引擎 ID
         :type ClusterIdentifier: str
         :param _DbName: 数据库名称
         :type DbName: str
@@ -8342,14 +8381,109 @@
 
 
     def _deserialize(self, params):
         self._Data = params.get("Data")
         self._RequestId = params.get("RequestId")
 
 
+class CreateDsFolderRequest(AbstractModel):
+    """CreateDsFolder请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目Id
+        :type ProjectId: str
+        :param _FolderName: 文件夹名称
+        :type FolderName: str
+        :param _ParentsFolderId: 父文件夹ID
+        :type ParentsFolderId: str
+        """
+        self._ProjectId = None
+        self._FolderName = None
+        self._ParentsFolderId = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def FolderName(self):
+        return self._FolderName
+
+    @FolderName.setter
+    def FolderName(self, FolderName):
+        self._FolderName = FolderName
+
+    @property
+    def ParentsFolderId(self):
+        return self._ParentsFolderId
+
+    @ParentsFolderId.setter
+    def ParentsFolderId(self, ParentsFolderId):
+        self._ParentsFolderId = ParentsFolderId
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._FolderName = params.get("FolderName")
+        self._ParentsFolderId = params.get("ParentsFolderId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateDsFolderResponse(AbstractModel):
+    """CreateDsFolder返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 文件夹Id，null则创建失败
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Data: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Data = params.get("Data")
+        self._RequestId = params.get("RequestId")
+
+
 class CreateFolderRequest(AbstractModel):
     """CreateFolder请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8852,15 +8986,15 @@
 
     def __init__(self):
         r"""
         :param _NodeInfo: 集成节点信息
         :type NodeInfo: :class:`tencentcloud.wedata.v20210820.models.IntegrationNodeInfo`
         :param _ProjectId: 项目id
         :type ProjectId: str
-        :param _TaskType: 任务类型
+        :param _TaskType: 任务类型，201为实时任务，202为离线任务
         :type TaskType: int
         """
         self._NodeInfo = None
         self._ProjectId = None
         self._TaskType = None
 
     @property
@@ -12301,14 +12435,96 @@
 
 
     def _deserialize(self, params):
         self._Data = params.get("Data")
         self._RequestId = params.get("RequestId")
 
 
+class DeleteDsFolderRequest(AbstractModel):
+    """DeleteDsFolder请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目Id
+        :type ProjectId: str
+        :param _FolderId: 文件夹ID
+        :type FolderId: str
+        """
+        self._ProjectId = None
+        self._FolderId = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def FolderId(self):
+        return self._FolderId
+
+    @FolderId.setter
+    def FolderId(self, FolderId):
+        self._FolderId = FolderId
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._FolderId = params.get("FolderId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteDsFolderResponse(AbstractModel):
+    """DeleteDsFolder返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: true代表删除成功，false代表删除失败
+        :type Data: bool
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Data = params.get("Data")
+        self._RequestId = params.get("RequestId")
+
+
 class DeleteFilePathRequest(AbstractModel):
     """DeleteFilePath请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -18500,14 +18716,272 @@
             for item in params.get("Data"):
                 obj = DrInstanceOpsDto()
                 obj._deserialize(item)
                 self._Data.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeDsFolderTreeRequest(AbstractModel):
+    """DescribeDsFolderTree请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目id
+        :type ProjectId: str
+        :param _FirstLevelPull: 是否一级拉取
+        :type FirstLevelPull: bool
+        :param _FolderId: 文件夹ID
+        :type FolderId: str
+        :param _WorkflowId: 工作流ID
+        :type WorkflowId: str
+        :param _Keyword: 关键字搜索
+        :type Keyword: str
+        :param _IncludeWorkflow: 是否包含工作流
+        :type IncludeWorkflow: bool
+        :param _IncludeTask: 是否包含任务
+        :type IncludeTask: bool
+        """
+        self._ProjectId = None
+        self._FirstLevelPull = None
+        self._FolderId = None
+        self._WorkflowId = None
+        self._Keyword = None
+        self._IncludeWorkflow = None
+        self._IncludeTask = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def FirstLevelPull(self):
+        return self._FirstLevelPull
+
+    @FirstLevelPull.setter
+    def FirstLevelPull(self, FirstLevelPull):
+        self._FirstLevelPull = FirstLevelPull
+
+    @property
+    def FolderId(self):
+        return self._FolderId
+
+    @FolderId.setter
+    def FolderId(self, FolderId):
+        self._FolderId = FolderId
+
+    @property
+    def WorkflowId(self):
+        return self._WorkflowId
+
+    @WorkflowId.setter
+    def WorkflowId(self, WorkflowId):
+        self._WorkflowId = WorkflowId
+
+    @property
+    def Keyword(self):
+        return self._Keyword
+
+    @Keyword.setter
+    def Keyword(self, Keyword):
+        self._Keyword = Keyword
+
+    @property
+    def IncludeWorkflow(self):
+        return self._IncludeWorkflow
+
+    @IncludeWorkflow.setter
+    def IncludeWorkflow(self, IncludeWorkflow):
+        self._IncludeWorkflow = IncludeWorkflow
+
+    @property
+    def IncludeTask(self):
+        return self._IncludeTask
+
+    @IncludeTask.setter
+    def IncludeTask(self, IncludeTask):
+        self._IncludeTask = IncludeTask
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._FirstLevelPull = params.get("FirstLevelPull")
+        self._FolderId = params.get("FolderId")
+        self._WorkflowId = params.get("WorkflowId")
+        self._Keyword = params.get("Keyword")
+        self._IncludeWorkflow = params.get("IncludeWorkflow")
+        self._IncludeTask = params.get("IncludeTask")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDsFolderTreeResponse(AbstractModel):
+    """DescribeDsFolderTree返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 统一树结构返回属性列表
+        :type Data: list of PathNodeDsVO
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = []
+            for item in params.get("Data"):
+                obj = PathNodeDsVO()
+                obj._deserialize(item)
+                self._Data.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeDsParentFolderTreeRequest(AbstractModel):
+    """DescribeDsParentFolderTree请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目id
+        :type ProjectId: str
+        :param _FolderId: 文件夹ID
+        :type FolderId: str
+        :param _WorkflowId: 工作流ID
+        :type WorkflowId: str
+        :param _TaskId: 任务id
+        :type TaskId: str
+        """
+        self._ProjectId = None
+        self._FolderId = None
+        self._WorkflowId = None
+        self._TaskId = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def FolderId(self):
+        return self._FolderId
+
+    @FolderId.setter
+    def FolderId(self, FolderId):
+        self._FolderId = FolderId
+
+    @property
+    def WorkflowId(self):
+        return self._WorkflowId
+
+    @WorkflowId.setter
+    def WorkflowId(self, WorkflowId):
+        self._WorkflowId = WorkflowId
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._FolderId = params.get("FolderId")
+        self._WorkflowId = params.get("WorkflowId")
+        self._TaskId = params.get("TaskId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDsParentFolderTreeResponse(AbstractModel):
+    """DescribeDsParentFolderTree返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 统一树结构返回属性列表
+        :type Data: list of PathNodeDsVO
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = []
+            for item in params.get("Data"):
+                obj = PathNodeDsVO()
+                obj._deserialize(item)
+                self._Data.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeEventCasesRequest(AbstractModel):
     """DescribeEventCases请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -24046,14 +24520,16 @@
         :type SourceServiceType: str
         :param _TargetServiceId: （仅针对离线同步任务）目标数据源id
         :type TargetServiceId: str
         :param _TargetServiceType: （仅针对离线同步任务）目标数据源类型
         :type TargetServiceType: str
         :param _AlarmType: 告警类型，多个类型以逗号分隔
         :type AlarmType: str
+        :param _ExecutorGroupIdList: 资源组id,多个资源组id之间以英文字符逗号分隔
+        :type ExecutorGroupIdList: str
         """
         self._ProjectId = None
         self._FolderIdList = None
         self._WorkFlowIdList = None
         self._WorkFlowNameList = None
         self._TaskNameList = None
         self._TaskIdList = None
@@ -24067,14 +24543,15 @@
         self._TaskCycleUnitList = None
         self._ProductNameList = None
         self._SourceServiceId = None
         self._SourceServiceType = None
         self._TargetServiceId = None
         self._TargetServiceType = None
         self._AlarmType = None
+        self._ExecutorGroupIdList = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
@@ -24228,14 +24705,22 @@
     def AlarmType(self):
         return self._AlarmType
 
     @AlarmType.setter
     def AlarmType(self, AlarmType):
         self._AlarmType = AlarmType
 
+    @property
+    def ExecutorGroupIdList(self):
+        return self._ExecutorGroupIdList
+
+    @ExecutorGroupIdList.setter
+    def ExecutorGroupIdList(self, ExecutorGroupIdList):
+        self._ExecutorGroupIdList = ExecutorGroupIdList
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
         self._FolderIdList = params.get("FolderIdList")
         self._WorkFlowIdList = params.get("WorkFlowIdList")
         self._WorkFlowNameList = params.get("WorkFlowNameList")
         self._TaskNameList = params.get("TaskNameList")
@@ -24250,14 +24735,15 @@
         self._TaskCycleUnitList = params.get("TaskCycleUnitList")
         self._ProductNameList = params.get("ProductNameList")
         self._SourceServiceId = params.get("SourceServiceId")
         self._SourceServiceType = params.get("SourceServiceType")
         self._TargetServiceId = params.get("TargetServiceId")
         self._TargetServiceType = params.get("TargetServiceType")
         self._AlarmType = params.get("AlarmType")
+        self._ExecutorGroupIdList = params.get("ExecutorGroupIdList")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -26043,17 +26529,17 @@
 class DescribeRealTimeTaskMetricOverviewRequest(AbstractModel):
     """DescribeRealTimeTaskMetricOverview请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TaskId: 要查看的实时任务的任务Id
+        :param _TaskId: 要查看的实时任务的任务ID，可在任务列表页面中获得
         :type TaskId: str
-        :param _ProjectId: 无
+        :param _ProjectId: 要查看的项目ID
         :type ProjectId: str
         :param _StartTime: 开始时间
         :type StartTime: int
         :param _EndTime: 结束时间
         :type EndTime: int
         """
         self._TaskId = None
@@ -30516,24 +31002,27 @@
         :type Container: str
         :param _Limit: 条数
         :type Limit: int
         :param _OrderType: 排序类型 desc asc
         :type OrderType: str
         :param _RunningOrderId: 作业运行的实例ID
         :type RunningOrderId: int
+        :param _Keyword: 关键字
+        :type Keyword: str
         """
         self._ProjectId = None
         self._TaskId = None
         self._JobId = None
         self._EndTime = None
         self._StartTime = None
         self._Container = None
         self._Limit = None
         self._OrderType = None
         self._RunningOrderId = None
+        self._Keyword = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
@@ -30599,25 +31088,34 @@
     def RunningOrderId(self):
         return self._RunningOrderId
 
     @RunningOrderId.setter
     def RunningOrderId(self, RunningOrderId):
         self._RunningOrderId = RunningOrderId
 
+    @property
+    def Keyword(self):
+        return self._Keyword
+
+    @Keyword.setter
+    def Keyword(self, Keyword):
+        self._Keyword = Keyword
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
         self._TaskId = params.get("TaskId")
         self._JobId = params.get("JobId")
         self._EndTime = params.get("EndTime")
         self._StartTime = params.get("StartTime")
         self._Container = params.get("Container")
         self._Limit = params.get("Limit")
         self._OrderType = params.get("OrderType")
         self._RunningOrderId = params.get("RunningOrderId")
+        self._Keyword = params.get("Keyword")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -37451,14 +37949,90 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class FindAllFolderRequest(AbstractModel):
+    """FindAllFolder请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目ID
+        :type ProjectId: str
+        """
+        self._ProjectId = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class FindAllFolderResponse(AbstractModel):
+    """FindAllFolder返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _FolderList: 文件夹列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FolderList: list of FolderDsDto
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._FolderList = None
+        self._RequestId = None
+
+    @property
+    def FolderList(self):
+        return self._FolderList
+
+    @FolderList.setter
+    def FolderList(self, FolderList):
+        self._FolderList = FolderList
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("FolderList") is not None:
+            self._FolderList = []
+            for item in params.get("FolderList"):
+                obj = FolderDsDto()
+                obj._deserialize(item)
+                self._FolderList.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class Folder(AbstractModel):
     """文件夹信息
 
     """
 
     def __init__(self):
         r"""
@@ -37532,14 +38106,188 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class FolderDsDto(AbstractModel):
+    """文件夹属性
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: 文件夹id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: str
+        :param _CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param _Name: 文件夹名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param _ProjectId: 所属项目id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProjectId: str
+        :param _UpdateTime: 更新时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdateTime: str
+        :param _ParentsFolderId: 父文件夹id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ParentsFolderId: str
+        :param _Total: 工作流总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Total: int
+        :param _Workflows: 工作流列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Workflows: list of WorkflowCanvasOpsDto
+        :param _TotalFolders: 子文件夹总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalFolders: int
+        :param _Folders: 子文件夹列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Folders: list of FolderDsDto
+        :param _FindType: 搜索类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FindType: str
+        """
+        self._Id = None
+        self._CreateTime = None
+        self._Name = None
+        self._ProjectId = None
+        self._UpdateTime = None
+        self._ParentsFolderId = None
+        self._Total = None
+        self._Workflows = None
+        self._TotalFolders = None
+        self._Folders = None
+        self._FindType = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def UpdateTime(self):
+        return self._UpdateTime
+
+    @UpdateTime.setter
+    def UpdateTime(self, UpdateTime):
+        self._UpdateTime = UpdateTime
+
+    @property
+    def ParentsFolderId(self):
+        return self._ParentsFolderId
+
+    @ParentsFolderId.setter
+    def ParentsFolderId(self, ParentsFolderId):
+        self._ParentsFolderId = ParentsFolderId
+
+    @property
+    def Total(self):
+        return self._Total
+
+    @Total.setter
+    def Total(self, Total):
+        self._Total = Total
+
+    @property
+    def Workflows(self):
+        return self._Workflows
+
+    @Workflows.setter
+    def Workflows(self, Workflows):
+        self._Workflows = Workflows
+
+    @property
+    def TotalFolders(self):
+        return self._TotalFolders
+
+    @TotalFolders.setter
+    def TotalFolders(self, TotalFolders):
+        self._TotalFolders = TotalFolders
+
+    @property
+    def Folders(self):
+        return self._Folders
+
+    @Folders.setter
+    def Folders(self, Folders):
+        self._Folders = Folders
+
+    @property
+    def FindType(self):
+        return self._FindType
+
+    @FindType.setter
+    def FindType(self, FindType):
+        self._FindType = FindType
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        self._CreateTime = params.get("CreateTime")
+        self._Name = params.get("Name")
+        self._ProjectId = params.get("ProjectId")
+        self._UpdateTime = params.get("UpdateTime")
+        self._ParentsFolderId = params.get("ParentsFolderId")
+        self._Total = params.get("Total")
+        if params.get("Workflows") is not None:
+            self._Workflows = []
+            for item in params.get("Workflows"):
+                obj = WorkflowCanvasOpsDto()
+                obj._deserialize(item)
+                self._Workflows.append(obj)
+        self._TotalFolders = params.get("TotalFolders")
+        if params.get("Folders") is not None:
+            self._Folders = []
+            for item in params.get("Folders"):
+                obj = FolderDsDto()
+                obj._deserialize(item)
+                self._Folders.append(obj)
+        self._FindType = params.get("FindType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class FolderOpsDto(AbstractModel):
     """文件夹属性
 
     """
 
     def __init__(self):
         r"""
@@ -39445,14 +40193,20 @@
         :type CvmAgentStatusList: list of CvmAgentStatus
         :param _AgentTotal: agent数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type AgentTotal: int
         :param _LifeDays: 生命周期
 注意：此字段可能返回 null，表示取不到有效值。
         :type LifeDays: int
+        :param _ClusterId: 集群ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterId: str
+        :param _AgentRegion: agent地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AgentRegion: str
         """
         self._AgentId = None
         self._AgentName = None
         self._Status = None
         self._StatusDesc = None
         self._AgentType = None
         self._Source = None
@@ -39460,14 +40214,16 @@
         self._ExecutorGroupId = None
         self._ExecutorGroupName = None
         self._TaskCount = None
         self._AgentGroupId = None
         self._CvmAgentStatusList = None
         self._AgentTotal = None
         self._LifeDays = None
+        self._ClusterId = None
+        self._AgentRegion = None
 
     @property
     def AgentId(self):
         return self._AgentId
 
     @AgentId.setter
     def AgentId(self, AgentId):
@@ -39573,14 +40329,30 @@
     def LifeDays(self):
         return self._LifeDays
 
     @LifeDays.setter
     def LifeDays(self, LifeDays):
         self._LifeDays = LifeDays
 
+    @property
+    def ClusterId(self):
+        return self._ClusterId
+
+    @ClusterId.setter
+    def ClusterId(self, ClusterId):
+        self._ClusterId = ClusterId
+
+    @property
+    def AgentRegion(self):
+        return self._AgentRegion
+
+    @AgentRegion.setter
+    def AgentRegion(self, AgentRegion):
+        self._AgentRegion = AgentRegion
+
 
     def _deserialize(self, params):
         self._AgentId = params.get("AgentId")
         self._AgentName = params.get("AgentName")
         self._Status = params.get("Status")
         self._StatusDesc = params.get("StatusDesc")
         self._AgentType = params.get("AgentType")
@@ -39594,14 +40366,16 @@
             self._CvmAgentStatusList = []
             for item in params.get("CvmAgentStatusList"):
                 obj = CvmAgentStatus()
                 obj._deserialize(item)
                 self._CvmAgentStatusList.append(obj)
         self._AgentTotal = params.get("AgentTotal")
         self._LifeDays = params.get("LifeDays")
+        self._ClusterId = params.get("ClusterId")
+        self._AgentRegion = params.get("AgentRegion")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -39846,14 +40620,16 @@
         :type DagDependent: str
         :param _DagDepth: dag深度 默认为1，取值 1-6
         :type DagDepth: int
         :param _TenantId: 租户id
         :type TenantId: str
         :param _DataTimeCycle: 根据当前数据时间或者是下一个数据时间查询, 默认当前数据时间
         :type DataTimeCycle: str
+        :param _ExecutorGroupIdList: 资源组id,多个资源组id用英文逗号分隔
+        :type ExecutorGroupIdList: list of str
         """
         self._Instance = None
         self._SortCol = None
         self._TaskIdList = None
         self._TaskNameList = None
         self._FolderList = None
         self._Sort = None
@@ -39877,14 +40653,15 @@
         self._InstanceType = None
         self._DagDeal = None
         self._DagType = None
         self._DagDependent = None
         self._DagDepth = None
         self._TenantId = None
         self._DataTimeCycle = None
+        self._ExecutorGroupIdList = None
 
     @property
     def Instance(self):
         return self._Instance
 
     @Instance.setter
     def Instance(self, Instance):
@@ -40118,14 +40895,22 @@
     def DataTimeCycle(self):
         return self._DataTimeCycle
 
     @DataTimeCycle.setter
     def DataTimeCycle(self, DataTimeCycle):
         self._DataTimeCycle = DataTimeCycle
 
+    @property
+    def ExecutorGroupIdList(self):
+        return self._ExecutorGroupIdList
+
+    @ExecutorGroupIdList.setter
+    def ExecutorGroupIdList(self, ExecutorGroupIdList):
+        self._ExecutorGroupIdList = ExecutorGroupIdList
+
 
     def _deserialize(self, params):
         if params.get("Instance") is not None:
             self._Instance = InstanceOpsDto()
             self._Instance._deserialize(params.get("Instance"))
         self._SortCol = params.get("SortCol")
         self._TaskIdList = params.get("TaskIdList")
@@ -40157,14 +40942,15 @@
         self._InstanceType = params.get("InstanceType")
         self._DagDeal = params.get("DagDeal")
         self._DagType = params.get("DagType")
         self._DagDependent = params.get("DagDependent")
         self._DagDepth = params.get("DagDepth")
         self._TenantId = params.get("TenantId")
         self._DataTimeCycle = params.get("DataTimeCycle")
+        self._ExecutorGroupIdList = params.get("ExecutorGroupIdList")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -41262,14 +42048,20 @@
         :type ProjectName: str
         :param _TenantId: 租户id
 注意：此字段可能返回 null，表示取不到有效值。
         :type TenantId: str
         :param _InstanceKey: 实例标识
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceKey: str
+        :param _ExecutorGroupId: 资源组id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorGroupId: str
+        :param _ExecutorGroupName: 资源组名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorGroupName: str
         """
         self._TaskId = None
         self._TaskName = None
         self._WorkflowId = None
         self._WorkflowName = None
         self._InCharge = None
         self._CycleType = None
@@ -41315,14 +42107,16 @@
         self._FirstSubmitTime = None
         self._FirstRunTime = None
         self._ProjectId = None
         self._ProjectIdent = None
         self._ProjectName = None
         self._TenantId = None
         self._InstanceKey = None
+        self._ExecutorGroupId = None
+        self._ExecutorGroupName = None
 
     @property
     def TaskId(self):
         return self._TaskId
 
     @TaskId.setter
     def TaskId(self, TaskId):
@@ -41732,14 +42526,30 @@
     def InstanceKey(self):
         return self._InstanceKey
 
     @InstanceKey.setter
     def InstanceKey(self, InstanceKey):
         self._InstanceKey = InstanceKey
 
+    @property
+    def ExecutorGroupId(self):
+        return self._ExecutorGroupId
+
+    @ExecutorGroupId.setter
+    def ExecutorGroupId(self, ExecutorGroupId):
+        self._ExecutorGroupId = ExecutorGroupId
+
+    @property
+    def ExecutorGroupName(self):
+        return self._ExecutorGroupName
+
+    @ExecutorGroupName.setter
+    def ExecutorGroupName(self, ExecutorGroupName):
+        self._ExecutorGroupName = ExecutorGroupName
+
 
     def _deserialize(self, params):
         self._TaskId = params.get("TaskId")
         self._TaskName = params.get("TaskName")
         self._WorkflowId = params.get("WorkflowId")
         self._WorkflowName = params.get("WorkflowName")
         self._InCharge = params.get("InCharge")
@@ -41788,14 +42598,16 @@
         self._FirstSubmitTime = params.get("FirstSubmitTime")
         self._FirstRunTime = params.get("FirstRunTime")
         self._ProjectId = params.get("ProjectId")
         self._ProjectIdent = params.get("ProjectIdent")
         self._ProjectName = params.get("ProjectName")
         self._TenantId = params.get("TenantId")
         self._InstanceKey = params.get("InstanceKey")
+        self._ExecutorGroupId = params.get("ExecutorGroupId")
+        self._ExecutorGroupName = params.get("ExecutorGroupName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -46727,14 +47539,120 @@
 
 
     def _deserialize(self, params):
         self._Data = params.get("Data")
         self._RequestId = params.get("RequestId")
 
 
+class ModifyDsFolderRequest(AbstractModel):
+    """ModifyDsFolder请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目Id
+        :type ProjectId: str
+        :param _FolderName: 文件夹名称
+        :type FolderName: str
+        :param _FolderId: 文件夹Id
+        :type FolderId: str
+        :param _ParentsFolderId: 父文件夹ID
+        :type ParentsFolderId: str
+        """
+        self._ProjectId = None
+        self._FolderName = None
+        self._FolderId = None
+        self._ParentsFolderId = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def FolderName(self):
+        return self._FolderName
+
+    @FolderName.setter
+    def FolderName(self, FolderName):
+        self._FolderName = FolderName
+
+    @property
+    def FolderId(self):
+        return self._FolderId
+
+    @FolderId.setter
+    def FolderId(self, FolderId):
+        self._FolderId = FolderId
+
+    @property
+    def ParentsFolderId(self):
+        return self._ParentsFolderId
+
+    @ParentsFolderId.setter
+    def ParentsFolderId(self, ParentsFolderId):
+        self._ParentsFolderId = ParentsFolderId
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._FolderName = params.get("FolderName")
+        self._FolderId = params.get("FolderId")
+        self._ParentsFolderId = params.get("ParentsFolderId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyDsFolderResponse(AbstractModel):
+    """ModifyDsFolder返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: true代表成功，false代表失败
+        :type Data: bool
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Data = params.get("Data")
+        self._RequestId = params.get("RequestId")
+
+
 class ModifyExecStrategyRequest(AbstractModel):
     """ModifyExecStrategy请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -51252,14 +52170,131 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class PathNodeDsVO(AbstractModel):
+    """数据开发-统一树结构返回属性
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: PathNode ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: str
+        :param _Title: PathNode 名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Title: str
+        :param _Type: PathNode 类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Type: str
+        :param _ParentId: 父节点唯一标识
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ParentId: str
+        :param _IsLeaf: 是否叶子节点
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsLeaf: bool
+        :param _Children: 子节点列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Children: list of PathNodeDsVO
+        :param _Params: 业务参数 ,base64编译的json串，获取具体参数需要base64反编译
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Params: str
+        """
+        self._Id = None
+        self._Title = None
+        self._Type = None
+        self._ParentId = None
+        self._IsLeaf = None
+        self._Children = None
+        self._Params = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def Title(self):
+        return self._Title
+
+    @Title.setter
+    def Title(self, Title):
+        self._Title = Title
+
+    @property
+    def Type(self):
+        return self._Type
+
+    @Type.setter
+    def Type(self, Type):
+        self._Type = Type
+
+    @property
+    def ParentId(self):
+        return self._ParentId
+
+    @ParentId.setter
+    def ParentId(self, ParentId):
+        self._ParentId = ParentId
+
+    @property
+    def IsLeaf(self):
+        return self._IsLeaf
+
+    @IsLeaf.setter
+    def IsLeaf(self, IsLeaf):
+        self._IsLeaf = IsLeaf
+
+    @property
+    def Children(self):
+        return self._Children
+
+    @Children.setter
+    def Children(self, Children):
+        self._Children = Children
+
+    @property
+    def Params(self):
+        return self._Params
+
+    @Params.setter
+    def Params(self, Params):
+        self._Params = Params
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        self._Title = params.get("Title")
+        self._Type = params.get("Type")
+        self._ParentId = params.get("ParentId")
+        self._IsLeaf = params.get("IsLeaf")
+        if params.get("Children") is not None:
+            self._Children = []
+            for item in params.get("Children"):
+                obj = PathNodeDsVO()
+                obj._deserialize(item)
+                self._Children.append(obj)
+        self._Params = params.get("Params")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ProdSchedulerTask(AbstractModel):
     """数据质量生产调度任务业务实体
 
     """
 
     def __init__(self):
         r"""
@@ -56977,14 +58012,584 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RunForceSucScheduleInstancesRequest(AbstractModel):
+    """RunForceSucScheduleInstances请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Instances: 实例列表
+        :type Instances: list of InstanceOpsDto
+        :param _CheckFather: 检查父任务类型, true: 检查父任务; false: 不检查父任务 
+        :type CheckFather: bool
+        :param _RerunType: 重跑类型, 1: 自身; 3: 孩子; 2: 自身以及孩子 
+        :type RerunType: str
+        :param _DependentWay: 实例依赖方式, 1: 自依赖; 2: 任务依赖; 3: 自依赖及父子依赖 
+        :type DependentWay: str
+        :param _SkipEventListening: 重跑忽略事件监听与否 
+        :type SkipEventListening: bool
+        :param _SonInstanceType: 下游实例范围 1: 所在工作流 2: 所在项目 3: 所有跨工作流依赖的项目
+        :type SonInstanceType: str
+        :param _SearchCondition: 查询条件
+        :type SearchCondition: :class:`tencentcloud.wedata.v20210820.models.InstanceApiOpsRequest`
+        :param _OptType: 访问类型
+        :type OptType: str
+        :param _OperatorName: 操作者名称
+        :type OperatorName: str
+        :param _OperatorId: 操作者id
+        :type OperatorId: str
+        :param _ProjectId: 项目id
+        :type ProjectId: str
+        :param _ProjectIdent: 项目标志
+        :type ProjectIdent: str
+        :param _ProjectName: 项目名称
+        :type ProjectName: str
+        :param _PageIndex: 索引页码
+        :type PageIndex: int
+        :param _PageSize: 页面大小
+        :type PageSize: int
+        :param _Count: 数据总数
+        :type Count: int
+        :param _RequestBaseInfo: 基础请求信息
+        :type RequestBaseInfo: :class:`tencentcloud.wedata.v20210820.models.ProjectBaseInfoOpsRequest`
+        :param _IsCount: 是否计算总数
+        :type IsCount: bool
+        """
+        self._Instances = None
+        self._CheckFather = None
+        self._RerunType = None
+        self._DependentWay = None
+        self._SkipEventListening = None
+        self._SonInstanceType = None
+        self._SearchCondition = None
+        self._OptType = None
+        self._OperatorName = None
+        self._OperatorId = None
+        self._ProjectId = None
+        self._ProjectIdent = None
+        self._ProjectName = None
+        self._PageIndex = None
+        self._PageSize = None
+        self._Count = None
+        self._RequestBaseInfo = None
+        self._IsCount = None
+
+    @property
+    def Instances(self):
+        return self._Instances
+
+    @Instances.setter
+    def Instances(self, Instances):
+        self._Instances = Instances
+
+    @property
+    def CheckFather(self):
+        return self._CheckFather
+
+    @CheckFather.setter
+    def CheckFather(self, CheckFather):
+        self._CheckFather = CheckFather
+
+    @property
+    def RerunType(self):
+        return self._RerunType
+
+    @RerunType.setter
+    def RerunType(self, RerunType):
+        self._RerunType = RerunType
+
+    @property
+    def DependentWay(self):
+        return self._DependentWay
+
+    @DependentWay.setter
+    def DependentWay(self, DependentWay):
+        self._DependentWay = DependentWay
+
+    @property
+    def SkipEventListening(self):
+        return self._SkipEventListening
+
+    @SkipEventListening.setter
+    def SkipEventListening(self, SkipEventListening):
+        self._SkipEventListening = SkipEventListening
+
+    @property
+    def SonInstanceType(self):
+        return self._SonInstanceType
+
+    @SonInstanceType.setter
+    def SonInstanceType(self, SonInstanceType):
+        self._SonInstanceType = SonInstanceType
+
+    @property
+    def SearchCondition(self):
+        return self._SearchCondition
+
+    @SearchCondition.setter
+    def SearchCondition(self, SearchCondition):
+        self._SearchCondition = SearchCondition
+
+    @property
+    def OptType(self):
+        return self._OptType
+
+    @OptType.setter
+    def OptType(self, OptType):
+        self._OptType = OptType
+
+    @property
+    def OperatorName(self):
+        return self._OperatorName
+
+    @OperatorName.setter
+    def OperatorName(self, OperatorName):
+        self._OperatorName = OperatorName
+
+    @property
+    def OperatorId(self):
+        return self._OperatorId
+
+    @OperatorId.setter
+    def OperatorId(self, OperatorId):
+        self._OperatorId = OperatorId
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def ProjectIdent(self):
+        return self._ProjectIdent
+
+    @ProjectIdent.setter
+    def ProjectIdent(self, ProjectIdent):
+        self._ProjectIdent = ProjectIdent
+
+    @property
+    def ProjectName(self):
+        return self._ProjectName
+
+    @ProjectName.setter
+    def ProjectName(self, ProjectName):
+        self._ProjectName = ProjectName
+
+    @property
+    def PageIndex(self):
+        return self._PageIndex
+
+    @PageIndex.setter
+    def PageIndex(self, PageIndex):
+        self._PageIndex = PageIndex
+
+    @property
+    def PageSize(self):
+        return self._PageSize
+
+    @PageSize.setter
+    def PageSize(self, PageSize):
+        self._PageSize = PageSize
+
+    @property
+    def Count(self):
+        return self._Count
+
+    @Count.setter
+    def Count(self, Count):
+        self._Count = Count
+
+    @property
+    def RequestBaseInfo(self):
+        return self._RequestBaseInfo
+
+    @RequestBaseInfo.setter
+    def RequestBaseInfo(self, RequestBaseInfo):
+        self._RequestBaseInfo = RequestBaseInfo
+
+    @property
+    def IsCount(self):
+        return self._IsCount
+
+    @IsCount.setter
+    def IsCount(self, IsCount):
+        self._IsCount = IsCount
+
+
+    def _deserialize(self, params):
+        if params.get("Instances") is not None:
+            self._Instances = []
+            for item in params.get("Instances"):
+                obj = InstanceOpsDto()
+                obj._deserialize(item)
+                self._Instances.append(obj)
+        self._CheckFather = params.get("CheckFather")
+        self._RerunType = params.get("RerunType")
+        self._DependentWay = params.get("DependentWay")
+        self._SkipEventListening = params.get("SkipEventListening")
+        self._SonInstanceType = params.get("SonInstanceType")
+        if params.get("SearchCondition") is not None:
+            self._SearchCondition = InstanceApiOpsRequest()
+            self._SearchCondition._deserialize(params.get("SearchCondition"))
+        self._OptType = params.get("OptType")
+        self._OperatorName = params.get("OperatorName")
+        self._OperatorId = params.get("OperatorId")
+        self._ProjectId = params.get("ProjectId")
+        self._ProjectIdent = params.get("ProjectIdent")
+        self._ProjectName = params.get("ProjectName")
+        self._PageIndex = params.get("PageIndex")
+        self._PageSize = params.get("PageSize")
+        self._Count = params.get("Count")
+        if params.get("RequestBaseInfo") is not None:
+            self._RequestBaseInfo = ProjectBaseInfoOpsRequest()
+            self._RequestBaseInfo._deserialize(params.get("RequestBaseInfo"))
+        self._IsCount = params.get("IsCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RunForceSucScheduleInstancesResponse(AbstractModel):
+    """RunForceSucScheduleInstances返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 结果
+        :type Data: :class:`tencentcloud.wedata.v20210820.models.BatchOperateResultOpsDto`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = BatchOperateResultOpsDto()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
+class RunRerunScheduleInstancesRequest(AbstractModel):
+    """RunRerunScheduleInstances请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Instances: 实例列表
+        :type Instances: list of InstanceOpsDto
+        :param _CheckFather: 检查父任务类型, true: 检查父任务; false: 不检查父任务 
+        :type CheckFather: bool
+        :param _RerunType: 重跑类型, 1: 自身; 3: 孩子; 2: 自身以及孩子 
+        :type RerunType: str
+        :param _DependentWay: 实例依赖方式, 1: 自依赖; 2: 任务依赖; 3: 自依赖及父子依赖 
+        :type DependentWay: str
+        :param _SkipEventListening: 重跑忽略事件监听与否 
+        :type SkipEventListening: bool
+        :param _SonInstanceType: 下游实例范围 1: 所在工作流 2: 所在项目 3: 所有跨工作流依赖的项目
+        :type SonInstanceType: str
+        :param _SearchCondition: 查询条件
+        :type SearchCondition: :class:`tencentcloud.wedata.v20210820.models.InstanceApiOpsRequest`
+        :param _OptType: 访问类型
+        :type OptType: str
+        :param _OperatorName: 操作者名称
+        :type OperatorName: str
+        :param _OperatorId: 操作者id
+        :type OperatorId: str
+        :param _ProjectId: 项目id
+        :type ProjectId: str
+        :param _ProjectIdent: 项目标志
+        :type ProjectIdent: str
+        :param _ProjectName: 项目名称
+        :type ProjectName: str
+        :param _PageIndex: 索引页码
+        :type PageIndex: int
+        :param _PageSize: 页面大小
+        :type PageSize: int
+        :param _Count: 数据总数
+        :type Count: int
+        :param _RequestBaseInfo: 基础请求信息
+        :type RequestBaseInfo: :class:`tencentcloud.wedata.v20210820.models.ProjectBaseInfoOpsRequest`
+        :param _IsCount: 是否计算总数
+        :type IsCount: bool
+        """
+        self._Instances = None
+        self._CheckFather = None
+        self._RerunType = None
+        self._DependentWay = None
+        self._SkipEventListening = None
+        self._SonInstanceType = None
+        self._SearchCondition = None
+        self._OptType = None
+        self._OperatorName = None
+        self._OperatorId = None
+        self._ProjectId = None
+        self._ProjectIdent = None
+        self._ProjectName = None
+        self._PageIndex = None
+        self._PageSize = None
+        self._Count = None
+        self._RequestBaseInfo = None
+        self._IsCount = None
+
+    @property
+    def Instances(self):
+        return self._Instances
+
+    @Instances.setter
+    def Instances(self, Instances):
+        self._Instances = Instances
+
+    @property
+    def CheckFather(self):
+        return self._CheckFather
+
+    @CheckFather.setter
+    def CheckFather(self, CheckFather):
+        self._CheckFather = CheckFather
+
+    @property
+    def RerunType(self):
+        return self._RerunType
+
+    @RerunType.setter
+    def RerunType(self, RerunType):
+        self._RerunType = RerunType
+
+    @property
+    def DependentWay(self):
+        return self._DependentWay
+
+    @DependentWay.setter
+    def DependentWay(self, DependentWay):
+        self._DependentWay = DependentWay
+
+    @property
+    def SkipEventListening(self):
+        return self._SkipEventListening
+
+    @SkipEventListening.setter
+    def SkipEventListening(self, SkipEventListening):
+        self._SkipEventListening = SkipEventListening
+
+    @property
+    def SonInstanceType(self):
+        return self._SonInstanceType
+
+    @SonInstanceType.setter
+    def SonInstanceType(self, SonInstanceType):
+        self._SonInstanceType = SonInstanceType
+
+    @property
+    def SearchCondition(self):
+        return self._SearchCondition
+
+    @SearchCondition.setter
+    def SearchCondition(self, SearchCondition):
+        self._SearchCondition = SearchCondition
+
+    @property
+    def OptType(self):
+        return self._OptType
+
+    @OptType.setter
+    def OptType(self, OptType):
+        self._OptType = OptType
+
+    @property
+    def OperatorName(self):
+        return self._OperatorName
+
+    @OperatorName.setter
+    def OperatorName(self, OperatorName):
+        self._OperatorName = OperatorName
+
+    @property
+    def OperatorId(self):
+        return self._OperatorId
+
+    @OperatorId.setter
+    def OperatorId(self, OperatorId):
+        self._OperatorId = OperatorId
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def ProjectIdent(self):
+        return self._ProjectIdent
+
+    @ProjectIdent.setter
+    def ProjectIdent(self, ProjectIdent):
+        self._ProjectIdent = ProjectIdent
+
+    @property
+    def ProjectName(self):
+        return self._ProjectName
+
+    @ProjectName.setter
+    def ProjectName(self, ProjectName):
+        self._ProjectName = ProjectName
+
+    @property
+    def PageIndex(self):
+        return self._PageIndex
+
+    @PageIndex.setter
+    def PageIndex(self, PageIndex):
+        self._PageIndex = PageIndex
+
+    @property
+    def PageSize(self):
+        return self._PageSize
+
+    @PageSize.setter
+    def PageSize(self, PageSize):
+        self._PageSize = PageSize
+
+    @property
+    def Count(self):
+        return self._Count
+
+    @Count.setter
+    def Count(self, Count):
+        self._Count = Count
+
+    @property
+    def RequestBaseInfo(self):
+        return self._RequestBaseInfo
+
+    @RequestBaseInfo.setter
+    def RequestBaseInfo(self, RequestBaseInfo):
+        self._RequestBaseInfo = RequestBaseInfo
+
+    @property
+    def IsCount(self):
+        return self._IsCount
+
+    @IsCount.setter
+    def IsCount(self, IsCount):
+        self._IsCount = IsCount
+
+
+    def _deserialize(self, params):
+        if params.get("Instances") is not None:
+            self._Instances = []
+            for item in params.get("Instances"):
+                obj = InstanceOpsDto()
+                obj._deserialize(item)
+                self._Instances.append(obj)
+        self._CheckFather = params.get("CheckFather")
+        self._RerunType = params.get("RerunType")
+        self._DependentWay = params.get("DependentWay")
+        self._SkipEventListening = params.get("SkipEventListening")
+        self._SonInstanceType = params.get("SonInstanceType")
+        if params.get("SearchCondition") is not None:
+            self._SearchCondition = InstanceApiOpsRequest()
+            self._SearchCondition._deserialize(params.get("SearchCondition"))
+        self._OptType = params.get("OptType")
+        self._OperatorName = params.get("OperatorName")
+        self._OperatorId = params.get("OperatorId")
+        self._ProjectId = params.get("ProjectId")
+        self._ProjectIdent = params.get("ProjectIdent")
+        self._ProjectName = params.get("ProjectName")
+        self._PageIndex = params.get("PageIndex")
+        self._PageSize = params.get("PageSize")
+        self._Count = params.get("Count")
+        if params.get("RequestBaseInfo") is not None:
+            self._RequestBaseInfo = ProjectBaseInfoOpsRequest()
+            self._RequestBaseInfo._deserialize(params.get("RequestBaseInfo"))
+        self._IsCount = params.get("IsCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RunRerunScheduleInstancesResponse(AbstractModel):
+    """RunRerunScheduleInstances返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 结果
+        :type Data: :class:`tencentcloud.wedata.v20210820.models.BatchOperateResultOpsDto`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = BatchOperateResultOpsDto()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
 class RunTaskRequest(AbstractModel):
     """RunTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -65366,14 +66971,20 @@
         :type TargetServiceType: str
         :param _TasksStr: 子任务列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type TasksStr: str
         :param _Submit: 任务版本是否已提交
 注意：此字段可能返回 null，表示取不到有效值。
         :type Submit: bool
+        :param _ExecutorGroupId: 资源组id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorGroupId: str
+        :param _ExecutorGroupName: 资源组名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorGroupName: str
         """
         self._TaskId = None
         self._VirtualTaskId = None
         self._VirtualFlag = None
         self._TaskName = None
         self._WorkflowId = None
         self._RealWorkflowId = None
@@ -65447,14 +67058,16 @@
         self._Layer = None
         self._SourceServiceId = None
         self._SourceServiceType = None
         self._TargetServiceId = None
         self._TargetServiceType = None
         self._TasksStr = None
         self._Submit = None
+        self._ExecutorGroupId = None
+        self._ExecutorGroupName = None
 
     @property
     def TaskId(self):
         return self._TaskId
 
     @TaskId.setter
     def TaskId(self, TaskId):
@@ -66088,14 +67701,30 @@
     def Submit(self):
         return self._Submit
 
     @Submit.setter
     def Submit(self, Submit):
         self._Submit = Submit
 
+    @property
+    def ExecutorGroupId(self):
+        return self._ExecutorGroupId
+
+    @ExecutorGroupId.setter
+    def ExecutorGroupId(self, ExecutorGroupId):
+        self._ExecutorGroupId = ExecutorGroupId
+
+    @property
+    def ExecutorGroupName(self):
+        return self._ExecutorGroupName
+
+    @ExecutorGroupName.setter
+    def ExecutorGroupName(self, ExecutorGroupName):
+        self._ExecutorGroupName = ExecutorGroupName
+
 
     def _deserialize(self, params):
         self._TaskId = params.get("TaskId")
         self._VirtualTaskId = params.get("VirtualTaskId")
         self._VirtualFlag = params.get("VirtualFlag")
         self._TaskName = params.get("TaskName")
         self._WorkflowId = params.get("WorkflowId")
@@ -66174,14 +67803,16 @@
         self._Layer = params.get("Layer")
         self._SourceServiceId = params.get("SourceServiceId")
         self._SourceServiceType = params.get("SourceServiceType")
         self._TargetServiceId = params.get("TargetServiceId")
         self._TargetServiceType = params.get("TargetServiceType")
         self._TasksStr = params.get("TasksStr")
         self._Submit = params.get("Submit")
+        self._ExecutorGroupId = params.get("ExecutorGroupId")
+        self._ExecutorGroupName = params.get("ExecutorGroupName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.998/tencentcloud/wedata/v20210820/errorcodes.py` & `tencentcloud-sdk-python-wedata-3.0.999/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.998/tencentcloud/wedata/v20210820/wedata_client.py` & `tencentcloud-sdk-python-wedata-3.0.999/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -808,14 +808,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def CreateDsFolder(self, request):
+        """编排空间-创建文件夹
+
+        :param request: Request instance for CreateDsFolder.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.CreateDsFolderRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.CreateDsFolderResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateDsFolder", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateDsFolderResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def CreateFolder(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         创建文件夹
 
         :param request: Request instance for CreateFolder.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateFolderRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.CreateFolderResponse`
@@ -1249,14 +1272,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DeleteDsFolder(self, request):
+        """编排空间-删除文件夹
+
+        :param request: Request instance for DeleteDsFolder.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteDsFolderRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.DeleteDsFolderResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteDsFolder", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteDsFolderResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DeleteFile(self, request):
         """删除文件
 
         :param request: Request instance for DeleteFile.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteFileRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.DeleteFileResponse`
 
@@ -2405,14 +2451,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeDsFolderTree(self, request):
+        """查询目录树
+
+        :param request: Request instance for DescribeDsFolderTree.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeDsFolderTreeRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.DescribeDsFolderTreeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDsFolderTree", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDsFolderTreeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeDsParentFolderTree(self, request):
+        """查询父目录树，用于工作流、任务定位
+
+        :param request: Request instance for DescribeDsParentFolderTree.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeDsParentFolderTreeRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.DescribeDsParentFolderTreeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDsParentFolderTree", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDsParentFolderTreeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeEvent(self, request):
         """根据项目ID和事件名称查看事件详情
 
         :param request: Request instance for DescribeEvent.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeEventRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.DescribeEventResponse`
 
@@ -3283,15 +3375,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKafkaTopicInfo(self, request):
-        """获取kafka的topic信息
+        """没用到
+
+        获取kafka的topic信息
 
         :param request: Request instance for DescribeKafkaTopicInfo.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeKafkaTopicInfoRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.DescribeKafkaTopicInfoResponse`
 
         """
         try:
@@ -5335,14 +5429,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def FindAllFolder(self, request):
+        """查找全部的文件夹
+
+        :param request: Request instance for FindAllFolder.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.FindAllFolderRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.FindAllFolderResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("FindAllFolder", params, headers=headers)
+            response = json.loads(body)
+            model = models.FindAllFolderResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def ForceSucInstances(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         实例批量置成功
 
         :param request: Request instance for ForceSucInstances.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ForceSucInstancesRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.ForceSucInstancesResponse`
@@ -5850,14 +5967,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def ModifyDsFolder(self, request):
+        """数据开发模块-文件夹更新
+
+        :param request: Request instance for ModifyDsFolder.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyDsFolderRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.ModifyDsFolderResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyDsFolder", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyDsFolderResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def ModifyExecStrategy(self, request):
         """更新规则组执行策略
 
         :param request: Request instance for ModifyExecStrategy.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyExecStrategyRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.ModifyExecStrategyResponse`
 
@@ -6409,14 +6549,60 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def RunForceSucScheduleInstances(self, request):
+        """实例强制成功
+
+        :param request: Request instance for RunForceSucScheduleInstances.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.RunForceSucScheduleInstancesRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.RunForceSucScheduleInstancesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RunForceSucScheduleInstances", params, headers=headers)
+            response = json.loads(body)
+            model = models.RunForceSucScheduleInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def RunRerunScheduleInstances(self, request):
+        """实例批量重跑
+
+        :param request: Request instance for RunRerunScheduleInstances.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.RunRerunScheduleInstancesRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.RunRerunScheduleInstancesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RunRerunScheduleInstances", params, headers=headers)
+            response = json.loads(body)
+            model = models.RunRerunScheduleInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RunTask(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         运行任务
 
         :param request: Request instance for RunTask.
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wedata-3.0.999/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wedata-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.999/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.998/README.rst` & `tencentcloud-sdk-python-wedata-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.998/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.999/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.998/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-wedata-3.0.999/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.998/setup.py` & `tencentcloud-sdk-python-wedata-3.0.999/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-wedata',
-    install_requires=["tencentcloud-sdk-python-common==3.0.998"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.999"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Wedata SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

