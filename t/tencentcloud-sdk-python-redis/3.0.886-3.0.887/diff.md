# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.886.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.887.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.886.tar", last modified: Mon May  8 03:48:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.887.tar", last modified: Tue May  9 03:11:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.886.tar` & `tencentcloud-sdk-python-redis-3.0.887.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud/redis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)    86757 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   292174 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:48:28.000000 tencentcloud-sdk-python-redis-3.0.886/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    86832 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   295067 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud_sdk_python_redis.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-redis-3.0.886/README.rst` & `tencentcloud-sdk-python-redis-3.0.887/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.886/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/redis_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ChangeReplicaToMaster(self, request):
-        """该接口仅支持多AZ实例副本组提主和单AZ副本提主
+        """本接口（ChangeReplicaToMaster）适用于实例副本组提主或副本提主。
 
         :param request: Request instance for ChangeReplicaToMaster.
         :type request: :class:`tencentcloud.redis.v20180412.models.ChangeReplicaToMasterRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.ChangeReplicaToMasterResponse`
 
         """
         try:
@@ -1265,15 +1265,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeTaskList(self, request):
-        """查询任务列表信息
+        """本接口（DescribeTaskList）用于查询指定实例的任务列表信息。
 
         :param request: Request instance for DescribeTaskList.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeTaskListRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.DescribeTaskListResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-redis-3.0.886/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.886/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,17 +513,18 @@
 class ChangeReplicaToMasterRequest(AbstractModel):
     """ChangeReplicaToMaster请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例Id
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
+
         :type InstanceId: str
-        :param GroupId: 副本组Id，多AZ实例必填
+        :param GroupId: 副本节点组 ID，请通过接口[DescribeInstanceZoneInfo](https://cloud.tencent.com/document/product/239/50312)获取多 AZ备节点组的 ID 信息。单 AZ，则无需配置该参数。
         :type GroupId: int
         """
         self.InstanceId = None
         self.GroupId = None
 
 
     def _deserialize(self, params):
@@ -541,15 +542,15 @@
 class ChangeReplicaToMasterResponse(AbstractModel):
     """ChangeReplicaToMaster返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TaskId: 异步任务ID
+        :param TaskId: 异步任务ID。
         :type TaskId: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TaskId = None
         self.RequestId = None
 
@@ -3072,15 +3073,25 @@
         :type TypeVersion: int
         :param EngineName: 存储引擎信息。可设置为Redis-2.8、Redis-4.0、Redis-5.0、Redis-6.0 或者 CKV。
         :type EngineName: str
         :param AutoRenew: 续费模式。<ul><li>0：手动续费。</li><li>1：自动续费。</li><li>2：到期不再续费。</ul>
         :type AutoRenew: list of int
         :param BillingMode: 计费模式。<ul><li>postpaid：按量计费。</li><li>prepaid：包年包月。</li></ul>
         :type BillingMode: str
-        :param Type: 实例类型。<ul><li>1：Redis 老集群版。</li><li>2：Redis 2.8 主从版。</li><li>3：CKV 主从版。</li><li>4：CKV 集群版。</li><li>5：Redis 2.8 单机版。</li><li>6：Redis 4.0主从版。</li><li>7：Redis 4.0 集群版。</li><li>8：Redis 5.0 主从版。</li><li>9：Redis 5.0 集群版。</li></ul>
+        :param Type: 实例类型。
+- 2：Redis 2.8内存版（标准架构）。
+- 3：CKV 3.2内存版（标准架构）。
+- 4：CKV 3.2内存版（集群架构）。
+- 5：Redis 2.8内存版（单机）。
+- 6：Redis 4.0内存版（标准架构）。
+- 7：Redis 4.0内存版（集群架构）。
+- 8：Redis 5.0内存版（标准架构）。
+- 9：Redis 5.0内存版（集群架构）。
+- 15：Redis 6.2内存版（标准架构）。
+- 16：Redis 6.2内存版（集群架构）。
         :type Type: int
         :param SearchKeys: 设置搜索关键字数组，可根据实例ID、实例名称、完整IP地址查询实例。
         :type SearchKeys: list of str
         :param TypeList: 内部参数，用户可忽略。
         :type TypeList: list of int
         :param MonitorVersion: 内部参数，用户可忽略。
         :type MonitorVersion: str
@@ -3893,37 +3904,60 @@
 class DescribeTaskListRequest(AbstractModel):
     """DescribeTaskList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例Id
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
         :type InstanceId: str
-        :param InstanceName: 实例名称
+        :param InstanceName: 实例名称。
         :type InstanceName: str
-        :param Limit: 分页大小,默认20，上限不大于100
+        :param Limit: 每页输出的任务列表大小。默认为 20，最多输出100条。
         :type Limit: int
-        :param Offset: 偏移量，取Limit整数倍（自动向下取整）
+        :param Offset: 分页偏移量，取Limit整数倍。计算公式：offset=limit*(页码-1)。
         :type Offset: int
-        :param ProjectIds: 项目Id
+        :param ProjectIds: 项目 ID。登录 [Redis 控制台](https://console.cloud.tencent.com/redis)，在右上角的账号信息下拉菜单中，选择**项目管理**，即可获取对应的项目 ID。
         :type ProjectIds: list of int
-        :param TaskTypes: 任务类型
+        :param TaskTypes: 任务类型。
+- FLOW_CREATE：创建实例。
+- FLOW_MODIFYCONNECTIONCONFIG：调整带宽连接数。
+- FLOW_MODIFYINSTANCEPASSWORDFREE：免密变更流程。
+- FLOW_CLEARNETWORK：VPC退还中。
+- FLOW_SETPWD：设置访问密码。
+- FLOW_EXPORSHR：扩缩容流程。
+- FLOW_UpgradeArch：实例架构升级流程。
+- FLOW_MODIFYINSTANCEPARAMS：修改实例参数。
+- FLOW_MODIFYINSTACEREADONLY：只读变更流程。
+- FLOW_CLOSE：关闭实例。
+- FLOW_DELETE：删除实例。
+- FLOW_OPEN_WAN：开启外网。
+- FLOW_CLEAN：清空实例。      
+- FLOW_MODIFYINSTANCEACCOUNT：修改实例账号。
+- FLOW_ENABLEINSTANCE_REPLICATE：开启副本只读。
+- FLOW_DISABLEINSTANCE_REPLICATE: 关闭副本只读。
+- FLOW_SWITCHINSTANCEVIP：交换实例 VIP。
+- FLOW_CHANGE_REPLICA_TO_MSTER：副本节点升主节点。
+- FLOW_BACKUPINSTANCE：备份实例。
         :type TaskTypes: list of str
-        :param BeginTime: 起始时间
+        :param BeginTime: 任务执行的起始时间。格式如：2021-12-30 00:00:00。
         :type BeginTime: str
-        :param EndTime: 终止时间
+        :param EndTime: 任务运行的终止时间。格式如：2021-12-30 20:59:35
         :type EndTime: str
-        :param TaskStatus: 任务状态
+        :param TaskStatus: 该参数为内部使用，请忽略。
         :type TaskStatus: list of int
-        :param Result: 任务状态
+        :param Result: 任务执行状态。
+- 0：任务初始化。
+- 1：执行中。
+- 2：完成。
+- 4：失败。
         :type Result: list of int
-        :param OperatorUin: 操作者Uin，该字段已废弃，使用OperateUin代替
+        :param OperatorUin: 该字段已废弃，使用OperateUin代替，请忽略。
         :type OperatorUin: list of int
-        :param OperateUin: 操作者Uin
+        :param OperateUin: 操作者账号 ID，UIN。
         :type OperateUin: list of str
         """
         self.InstanceId = None
         self.InstanceName = None
         self.Limit = None
         self.Offset = None
         self.ProjectIds = None
@@ -3961,17 +3995,17 @@
 class DescribeTaskListResponse(AbstractModel):
     """DescribeTaskList返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TotalCount: 任务总数
+        :param TotalCount: 任务总数。
         :type TotalCount: int
-        :param Tasks: 任务详细信息
+        :param Tasks: 任务详细信息。
         :type Tasks: list of TaskInfoDetail
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TotalCount = None
         self.Tasks = None
         self.RequestId = None
@@ -7883,39 +7917,63 @@
 class TaskInfoDetail(AbstractModel):
     """任务信息详情
 
     """
 
     def __init__(self):
         r"""
-        :param TaskId: 任务Id
+        :param TaskId: 任务 ID。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TaskId: int
-        :param StartTime: 开始时间
+        :param StartTime: 任务开始时间。
 注意：此字段可能返回 null，表示取不到有效值。
         :type StartTime: str
-        :param TaskType: 任务类型
+        :param TaskType: 任务类型。
+- FLOW_CREATE：创建实例。
+- FLOW_MODIFYCONNECTIONCONFIG：调整带宽连接数。
+- FLOW_MODIFYINSTANCEPASSWORDFREE：免密变更流程。
+- FLOW_CLEARNETWORK：VPC退还中。
+- FLOW_SETPWD：设置访问密码。
+- FLOW_EXPORSHR：扩缩容流程。
+- FLOW_UpgradeArch：实例架构升级流程。
+- FLOW_MODIFYINSTANCEPARAMS：修改实例参数。
+- FLOW_MODIFYINSTACEREADONLY：只读变更流程。
+- FLOW_CLOSE：关闭实例。
+- FLOW_DELETE：删除实例。
+- FLOW_OPEN_WAN：开启外网。
+- FLOW_CLEAN：清空实例。      
+- FLOW_MODIFYINSTANCEACCOUNT：修改实例账号。
+- FLOW_ENABLEINSTANCE_REPLICATE：开启副本只读。
+- FLOW_DISABLEINSTANCE_REPLICATE: 关闭副本只读。
+- FLOW_SWITCHINSTANCEVIP：交换实例 VIP。
+- FLOW_CHANGE_REPLICA_TO_MSTER：副本节点升主节点。
+- FLOW_BACKUPINSTANCE：备份实例。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TaskType: str
-        :param InstanceName: 实例名称
+        :param InstanceName: 实例名称。
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceName: str
-        :param InstanceId: 实例Id
+        :param InstanceId: 实例 ID。
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceId: str
-        :param ProjectId: 项目Id
+        :param ProjectId: 项目 ID。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ProjectId: int
-        :param Progress: 任务进度
+        :param Progress: 任务进度。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Progress: float
-        :param EndTime: 结束时间
+        :param EndTime: 任务执行结束时间。
 注意：此字段可能返回 null，表示取不到有效值。
         :type EndTime: str
-        :param Result: 任务状态
+        :param Result: 任务执行状态。
+
+0：任务初始化。
+1：执行中。
+2：完成。
+4：失败。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Result: int
         """
         self.TaskId = None
         self.StartTime = None
         self.TaskType = None
         self.InstanceName = None
```

### Comparing `tencentcloud-sdk-python-redis-3.0.886/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.887/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.886'
+__version__ = '3.0.887'
```

### Comparing `tencentcloud-sdk-python-redis-3.0.886/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.887/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.886/setup.py` & `tencentcloud-sdk-python-redis-3.0.887/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.886/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.887/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

