# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.886.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.887.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.886.tar", last modified: Mon May  8 04:11:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.887.tar", last modified: Tue May  9 03:22:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.886.tar` & `tencentcloud-sdk-python-tione-3.0.887.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)    51024 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)    10734 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   333554 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)    22010 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91250 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 04:11:39.000000 tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    51024 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)    10835 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   333554 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)    22010 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91250 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tione-3.0.886/README.rst` & `tencentcloud-sdk-python-tione-3.0.887/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,17 @@
 
 # 数据库执行错误。
 FAILEDOPERATION_EXECDATABASEFAIL = 'FailedOperation.ExecDatabaseFail'
 
 # 标签操作失败。
 FAILEDOPERATION_EXECTAGFAIL = 'FailedOperation.ExecTagFail'
 
+# 余额不足冻结失败。
+FAILEDOPERATION_FREEZEBILLFAILED = 'FailedOperation.FreezeBillFailed'
+
 # 白名单免费配额不足。
 FAILEDOPERATION_INSUFFICIENTWHITELISTQUOTA = 'FailedOperation.InsufficientWhitelistQuota'
 
 # 操作失败，用户类型异常。
 FAILEDOPERATION_INVALIDUSERTYPE = 'FailedOperation.InvalidUserType'
 
 # 密钥管理系统服务未开通，请先开通腾讯云密钥管理系统服务。
```

### Comparing `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8579,15 +8579,15 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type FailureReason: str
         :param UpdateTime: 更新时间
         :type UpdateTime: str
         :param EndTime: 训练结束时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type EndTime: str
-        :param BillingInfo: 计费金额信息，eg：2.00元/小时 (for后付费)
+        :param BillingInfo: 计费金额信息，eg：2.00元/小时 (按量计费)
 注意：此字段可能返回 null，表示取不到有效值。
         :type BillingInfo: str
         :param ResourceGroupName: 预付费专用资源组名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourceGroupName: str
         :param Message: 任务信息
 注意：此字段可能返回 null，表示取不到有效值。
@@ -8761,15 +8761,15 @@
         :param Output: 训练输出
         :type Output: :class:`tencentcloud.tione.v20211111.models.CosPathInfo`
         :param FailureReason: 失败原因
 注意：此字段可能返回 null，表示取不到有效值。
         :type FailureReason: str
         :param UpdateTime: 更新时间
         :type UpdateTime: str
-        :param BillingInfo: 计费金额信息，eg：2.00元/小时 (for后付费)
+        :param BillingInfo: 计费金额信息，eg：2.00元/小时 (按量计费)
         :type BillingInfo: str
         :param ResourceGroupName: 预付费专用资源组名称
         :type ResourceGroupName: str
         :param ImageInfo: 自定义镜像信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type ImageInfo: :class:`tencentcloud.tione.v20211111.models.ImageInfo`
         :param Message: 任务信息
```

### Comparing `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.886/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.886/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.887/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.886/setup.py` & `tencentcloud-sdk-python-tione-3.0.887/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.886/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

