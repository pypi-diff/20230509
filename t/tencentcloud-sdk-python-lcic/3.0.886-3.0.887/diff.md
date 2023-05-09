# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.886.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.887.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.886.tar", last modified: Mon May  8 03:36:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.887.tar", last modified: Tue May  9 03:04:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.886.tar` & `tencentcloud-sdk-python-lcic-3.0.887.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud/lcic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud/lcic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)     4332 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)   139745 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)    47779 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:36:04.000000 tencentcloud-sdk-python-lcic-3.0.886/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud/lcic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud/lcic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)     4332 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   139844 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)    47779 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:04:32.000000 tencentcloud-sdk-python-lcic-3.0.887/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.886/README.rst` & `tencentcloud-sdk-python-lcic-3.0.887/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.886/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.887/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.886/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.887/tencentcloud/lcic/v20220817/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -963,21 +963,23 @@
 1 禁止录制
 注：如果该配置取值为0，录制将从上课后开始，课堂结束后停止。
         :type DisableRecord: int
         :param Assistants: 助教Id列表。通过[注册用户]接口获取的UserId。指定后该用户在房间内拥有助教权限。
         :type Assistants: list of str
         :param RTCAudienceNumber: rtc人数。
         :type RTCAudienceNumber: int
-        :param AudienceType: 观看类型。0未知，1互动，2cdn或直播。 目前仅支持互动类型
+        :param AudienceType: 观看类型，互动直播（默认）。
         :type AudienceType: int
         :param RecordLayout: 录制布局。录制模板枚举值参考：https://cloud.tencent.com/document/product/1639/89744
         :type RecordLayout: int
         :param GroupId: 房间绑定的群组ID,非空时限制组成员进入
         :type GroupId: str
-        :param EnableDirectControl: 打开学生麦克风/摄像头的授权开关
+        :param EnableDirectControl: 是否允许老师/助教直接控制学生的摄像头/麦克风。可以有以下取值：
+0 不允许直接控制（需同意，默认值）
+1 允许直接控制（无需同意）
         :type EnableDirectControl: int
         """
         self.Name = None
         self.StartTime = None
         self.EndTime = None
         self.SdkAppId = None
         self.Resolution = None
@@ -1601,15 +1603,15 @@
 class DescribeDeveloperResponse(AbstractModel):
     """DescribeDeveloper返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param DeveloperId: 服务商ID
+        :param DeveloperId: 开发商ID
         :type DeveloperId: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.DeveloperId = None
         self.RequestId = None
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.886/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.887/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,15 +575,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDeveloper(self, request):
-        """服务商信息获取
+        """开发商信息获取
 
         :param request: Request instance for DescribeDeveloper.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeDeveloperRequest`
         :rtype: :class:`tencentcloud.lcic.v20220817.models.DescribeDeveloperResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.886/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.887/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lcic-3.0.886/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.887/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.886/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.887/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.886/setup.py` & `tencentcloud-sdk-python-lcic-3.0.887/setup.py`

 * *Files identical despite different names*

