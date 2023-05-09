# Comparing `tmp/tencentcloud-sdk-python-ims-3.0.885.tar.gz` & `tmp/tencentcloud-sdk-python-ims-3.0.887.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ims-3.0.885.tar", last modified: Mon May  1 00:42:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ims-3.0.887.tar", last modified: Tue May  9 03:03:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ims-3.0.885.tar` & `tencentcloud-sdk-python-ims-3.0.887.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20200713/
--rw-r--r--   0 root         (0) root         (0)     3507 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20200713/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20200713/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27418 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20200713/models.py
--rw-r--r--   0 root         (0) root         (0)     3224 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20200713/ims_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20201229/
--rw-r--r--   0 root         (0) root         (0)     3618 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20201229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20201229/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47151 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20201229/models.py
--rw-r--r--   0 root         (0) root         (0)     8549 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20201229/ims_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud_sdk_python_ims.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud_sdk_python_ims.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud_sdk_python_ims.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud_sdk_python_ims.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/tencentcloud_sdk_python_ims.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:42:21.000000 tencentcloud-sdk-python-ims-3.0.885/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20200713/
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20200713/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20200713/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30860 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20200713/models.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20200713/ims_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20201229/
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20201229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20201229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47385 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20201229/models.py
+-rw-r--r--   0 root         (0) root         (0)     8549 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20201229/ims_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud_sdk_python_ims.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud_sdk_python_ims.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud_sdk_python_ims.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud_sdk_python_ims.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/tencentcloud_sdk_python_ims.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:03:11.000000 tencentcloud-sdk-python-ims-3.0.887/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ims-3.0.885/README.rst` & `tencentcloud-sdk-python-ims-3.0.887/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20200713/errorcodes.py` & `tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20200713/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 # 图片内容参数为空。
 INVALIDPARAMETERVALUE_EMPTYIMAGECONTENT = 'InvalidParameterValue.EmptyImageContent'
 
 # 图片分辨率太低。
 INVALIDPARAMETERVALUE_IMAGESIZETOOSMALL = 'InvalidParameterValue.ImageSizeTooSmall'
 
-# FileContent和FileUrl为空。
+# FileContent和FileUrl为空或base64编码错误。
 INVALIDPARAMETERVALUE_INVALIDCONTENT = 'InvalidParameterValue.InvalidContent'
 
 # DataId格式错误。
 INVALIDPARAMETERVALUE_INVALIDDATAID = 'InvalidParameterValue.InvalidDataId'
 
 # 图片文件内容大小异常。
 INVALIDPARAMETERVALUE_INVALIDFILECONTENTSIZE = 'InvalidParameterValue.InvalidFileContentSize'
```

### Comparing `tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20200713/models.py` & `tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20200713/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -164,14 +164,17 @@
         :type DataId: str
         :param BizType: 您在入参时所填入的Biztype参数。 -- 该字段暂未开放。
         :type BizType: str
         :param Extra: 扩展字段，用于特定信息返回，不同客户/Biztype下返回信息不同。
 注意：此字段可能返回 null，表示取不到有效值。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Extra: str
+        :param RecognitionResults: 该字段用于返回仅识别图片元素的模型结果；包括：场景模型命中的标签、置信度和位置信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RecognitionResults: list of RecognitionResult
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.HitFlag = None
         self.Suggestion = None
         self.Label = None
         self.SubLabel = None
@@ -179,14 +182,15 @@
         self.LabelResults = None
         self.ObjectResults = None
         self.OcrResults = None
         self.LibResults = None
         self.DataId = None
         self.BizType = None
         self.Extra = None
+        self.RecognitionResults = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.HitFlag = params.get("HitFlag")
         self.Suggestion = params.get("Suggestion")
         self.Label = params.get("Label")
@@ -215,14 +219,20 @@
             for item in params.get("LibResults"):
                 obj = LibResult()
                 obj._deserialize(item)
                 self.LibResults.append(obj)
         self.DataId = params.get("DataId")
         self.BizType = params.get("BizType")
         self.Extra = params.get("Extra")
+        if params.get("RecognitionResults") is not None:
+            self.RecognitionResults = []
+            for item in params.get("RecognitionResults"):
+                obj = RecognitionResult()
+                obj._deserialize(item)
+                self.RecognitionResults.append(obj)
         self.RequestId = params.get("RequestId")
 
 
 class LabelDetailItem(AbstractModel):
     """分类模型命中子标签结果
 
     """
@@ -470,32 +480,42 @@
         :type Value: str
         :param Score: 分数
         :type Score: int
         :param Location: 检测框坐标
         :type Location: :class:`tencentcloud.ims.v20200713.models.Location`
         :param SubLabel: 二级标签名称
         :type SubLabel: str
+        :param GroupId: 图库或人脸库id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GroupId: str
+        :param ObjectId: 图或人脸id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ObjectId: str
         """
         self.Id = None
         self.Name = None
         self.Value = None
         self.Score = None
         self.Location = None
         self.SubLabel = None
+        self.GroupId = None
+        self.ObjectId = None
 
 
     def _deserialize(self, params):
         self.Id = params.get("Id")
         self.Name = params.get("Name")
         self.Value = params.get("Value")
         self.Score = params.get("Score")
         if params.get("Location") is not None:
             self.Location = Location()
             self.Location._deserialize(params.get("Location"))
         self.SubLabel = params.get("SubLabel")
+        self.GroupId = params.get("GroupId")
+        self.ObjectId = params.get("ObjectId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -671,14 +691,86 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class RecognitionResult(AbstractModel):
+    """识别类型标签结果信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Label: 当前可能的取值：Scene（图片场景模型）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Label: str
+        :param Tags: Label对应模型下的识别标签信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tags: list of RecognitionTag
+        """
+        self.Label = None
+        self.Tags = None
+
+
+    def _deserialize(self, params):
+        self.Label = params.get("Label")
+        if params.get("Tags") is not None:
+            self.Tags = []
+            for item in params.get("Tags"):
+                obj = RecognitionTag()
+                obj._deserialize(item)
+                self.Tags.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RecognitionTag(AbstractModel):
+    """识别类型标签信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 标签名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param Score: 置信分：0～100，数值越大表示置信度越高
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Score: int
+        :param Location: 标签位置信息，若模型无位置信息，则可能为零值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Location: :class:`tencentcloud.ims.v20200713.models.Location`
+        """
+        self.Name = None
+        self.Score = None
+        self.Location = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.Score = params.get("Score")
+        if params.get("Location") is not None:
+            self.Location = Location()
+            self.Location._deserialize(params.get("Location"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class User(AbstractModel):
     """User结果
 
     """
```

### Comparing `tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20200713/ims_client.py` & `tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20200713/ims_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20201229/errorcodes.py` & `tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20201229/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 # 图片分辨率太低。
 INVALIDPARAMETERVALUE_IMAGESIZETOOSMALL = 'InvalidParameterValue.ImageSizeTooSmall'
 
 # 回调地址错误。
 INVALIDPARAMETERVALUE_INVALIDCALLBACKURL = 'InvalidParameterValue.InvalidCallbackUrl'
 
-# FileContent和FileUrl为空。
+# FileContent和FileUrl为空或base64编码错误。
 INVALIDPARAMETERVALUE_INVALIDCONTENT = 'InvalidParameterValue.InvalidContent'
 
 # DataId格式错误。
 INVALIDPARAMETERVALUE_INVALIDDATAID = 'InvalidParameterValue.InvalidDataId'
 
 # 图片文件内容大小异常。
 INVALIDPARAMETERVALUE_INVALIDFILECONTENTSIZE = 'InvalidParameterValue.InvalidFileContentSize'
```

### Comparing `tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20201229/models.py` & `tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20201229/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,32 +549,37 @@
         :type Value: str
         :param Score: 该参数用于返回对应实体标签命中的分值，取值为**0-100**，如：*QrCode 99* 则代表相应识别内容命中二维码场景标签的概率非常高。
         :type Score: int
         :param Location: 该字段用于返回实体检测框的坐标位置（左上角xy坐标、长宽、旋转角度）以方便快速定位实体的相关信息。
         :type Location: :class:`tencentcloud.ims.v20201229.models.Location`
         :param SubLabel: 该参数用于返回命中的实体二级标签。
         :type SubLabel: str
+        :param ObjectId: 该参数用于返回命中的人脸id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ObjectId: str
         """
         self.Id = None
         self.Name = None
         self.Value = None
         self.Score = None
         self.Location = None
         self.SubLabel = None
+        self.ObjectId = None
 
 
     def _deserialize(self, params):
         self.Id = params.get("Id")
         self.Name = params.get("Name")
         self.Value = params.get("Value")
         self.Score = params.get("Score")
         if params.get("Location") is not None:
             self.Location = Location()
             self.Location._deserialize(params.get("Location"))
         self.SubLabel = params.get("SubLabel")
+        self.ObjectId = params.get("ObjectId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ims-3.0.885/tencentcloud/ims/v20201229/ims_client.py` & `tencentcloud-sdk-python-ims-3.0.887/tencentcloud/ims/v20201229/ims_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.885/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ims-3.0.887/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.885'
+__version__ = '3.0.887'
```

### Comparing `tencentcloud-sdk-python-ims-3.0.885/tencentcloud_sdk_python_ims.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-ims-3.0.887/tencentcloud_sdk_python_ims.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.885/tencentcloud_sdk_python_ims.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ims-3.0.887/tencentcloud_sdk_python_ims.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ims
-Version: 3.0.885
+Version: 3.0.887
 Summary: Tencent Cloud Ims SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ims-3.0.885/PKG-INFO` & `tencentcloud-sdk-python-ims-3.0.887/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ims
-Version: 3.0.885
+Version: 3.0.887
 Summary: Tencent Cloud Ims SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ims-3.0.885/setup.py` & `tencentcloud-sdk-python-ims-3.0.887/setup.py`

 * *Files identical despite different names*

