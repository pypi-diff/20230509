# Comparing `tmp/tencentcloud-sdk-python-thpc-3.0.886.tar.gz` & `tmp/tencentcloud-sdk-python-thpc-3.0.887.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.886.tar", last modified: Mon May  8 04:10:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.887.tar", last modified: Tue May  9 03:22:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-thpc-3.0.886.tar` & `tencentcloud-sdk-python-thpc-3.0.887.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20220401/
--rw-r--r--   0 root         (0) root         (0)     4733 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20220401/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20220401/__init__.py
--rw-r--r--   0 root         (0) root         (0)    97393 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20220401/models.py
--rw-r--r--   0 root         (0) root         (0)    16733 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20220401/thpc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20211109/
--rw-r--r--   0 root         (0) root         (0)     2035 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20211109/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20211109/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43727 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20211109/models.py
--rw-r--r--   0 root         (0) root         (0)     4612 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20211109/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20230321/
--rw-r--r--   0 root         (0) root         (0)     4248 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20230321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20230321/__init__.py
--rw-r--r--   0 root         (0) root         (0)   101533 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20230321/models.py
--rw-r--r--   0 root         (0) root         (0)    16736 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20230321/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud_sdk_python_thpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      781 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 04:10:53.000000 tencentcloud-sdk-python-thpc-3.0.886/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20220401/
+-rw-r--r--   0 root         (0) root         (0)     4733 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20220401/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20220401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    97393 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20220401/models.py
+-rw-r--r--   0 root         (0) root         (0)    16733 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20220401/thpc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20211109/
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20211109/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20211109/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43727 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20211109/models.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20211109/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20230321/
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20230321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20230321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   103105 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20230321/models.py
+-rw-r--r--   0 root         (0) root         (0)    17699 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20230321/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud_sdk_python_thpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      781 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:22:02.000000 tencentcloud-sdk-python-thpc-3.0.887/setup.cfg
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/README.rst` & `tencentcloud-sdk-python-thpc-3.0.887/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20220401/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20220401/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20220401/models.py` & `tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20220401/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20220401/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20220401/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20211109/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20211109/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20211109/models.py` & `tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20211109/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20211109/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20211109/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20230321/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20230321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20230321/models.py` & `tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20230321/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1161,14 +1161,65 @@
                 obj = ClusterOverview()
                 obj._deserialize(item)
                 self.ClusterSet.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeInitNodeScriptsRequest(AbstractModel):
+    """DescribeInitNodeScripts请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID。
+        :type ClusterId: str
+        """
+        self.ClusterId = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeInitNodeScriptsResponse(AbstractModel):
+    """DescribeInitNodeScripts返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InitNodeScriptSet: 节点初始化脚本列表。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InitNodeScriptSet: list of NodeScript
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.InitNodeScriptSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("InitNodeScriptSet") is not None:
+            self.InitNodeScriptSet = []
+            for item in params.get("InitNodeScriptSet"):
+                obj = NodeScript()
+                obj._deserialize(item)
+                self.InitNodeScriptSet.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeNodesRequest(AbstractModel):
     """DescribeNodes请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/thpc/v20230321/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/thpc/v20230321/thpc_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -305,14 +305,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeInitNodeScripts(self, request):
+        """本接口 (DescribeInitNodeScripts) 用于查询节点初始化脚本列表。
+
+        :param request: Request instance for DescribeInitNodeScripts.
+        :type request: :class:`tencentcloud.thpc.v20230321.models.DescribeInitNodeScriptsRequest`
+        :rtype: :class:`tencentcloud.thpc.v20230321.models.DescribeInitNodeScriptsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeInitNodeScripts", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeInitNodeScriptsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeNodes(self, request):
         """本接口 (DescribeNodes) 用于查询指定集群节点概览信息列表。
 
         :param request: Request instance for DescribeNodes.
         :type request: :class:`tencentcloud.thpc.v20230321.models.DescribeNodesRequest`
         :rtype: :class:`tencentcloud.thpc.v20230321.models.DescribeNodesResponse`
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/tencentcloud/__init__.py` & `tencentcloud-sdk-python-thpc-3.0.887/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-thpc-3.0.887/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.887/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.887/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.886/setup.py` & `tencentcloud-sdk-python-thpc-3.0.887/setup.py`

 * *Files identical despite different names*

