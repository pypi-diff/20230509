# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.886.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.887.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.886.tar", last modified: Mon May  8 03:36:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.887.tar", last modified: Tue May  9 03:06:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.886.tar` & `tencentcloud-sdk-python-lighthouse-3.0.887.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/
--rw-r--r--   0 root         (0) root         (0)      758 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    24695 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    88751 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   231682 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:36:11.000000 tencentcloud-sdk-python-lighthouse-3.0.886/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)    25647 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89637 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   236708 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.886/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.887/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 # 操作失败。
 FAILEDOPERATION = 'FailedOperation'
 
 # 创建镜像失败。
 FAILEDOPERATION_CREATEBLUEPRINTFAILED = 'FailedOperation.CreateBlueprintFailed'
 
+# 创建云硬盘失败。
+FAILEDOPERATION_CREATEDISKSFAILED = 'FailedOperation.CreateDisksFailed'
+
 # 创建实例失败。
 FAILEDOPERATION_CREATEINSTANCESFAILED = 'FailedOperation.CreateInstancesFailed'
 
 # 对密钥对的创建操作失败。
 FAILEDOPERATION_CREATEKEYPAIRFAILED = 'FailedOperation.CreateKeyPairFailed'
 
 # 对密钥对的删除操作失败。
@@ -214,14 +217,17 @@
 
 # 参数值非法，云硬盘备份点 ID 格式非法。
 INVALIDPARAMETERVALUE_DISKBACKUPIDMALFORMED = 'InvalidParameterValue.DiskBackupIdMalformed'
 
 # 指定的云盘备份点名称不可大于最大长度。
 INVALIDPARAMETERVALUE_DISKBACKUPNAMETOOLONG = 'InvalidParameterValue.DiskBackupNameTooLong'
 
+# 云硬盘的可用区与实例的可用区不匹配。
+INVALIDPARAMETERVALUE_DISKINSTANCEZONENOTMATCH = 'InvalidParameterValue.DiskInstanceZoneNotMatch'
+
 # 磁盘名称长度超出限制。
 INVALIDPARAMETERVALUE_DISKNAMETOOLONG = 'InvalidParameterValue.DiskNameTooLong'
 
 # 磁盘大小发生改变。
 INVALIDPARAMETERVALUE_DISKSIZENOTMATCH = 'InvalidParameterValue.DiskSizeNotMatch'
 
 # 参数 `KeyName` 已经存在且重复。
@@ -256,14 +262,17 @@
 
 # 控制台显示类型不合法。
 INVALIDPARAMETERVALUE_INVALIDCONSOLEDISPLAYTYPES = 'InvalidParameterValue.InvalidConsoleDisplayTypes'
 
 # 参数值非法，磁盘 ID 格式非法。
 INVALIDPARAMETERVALUE_INVALIDDISKIDMALFORMED = 'InvalidParameterValue.InvalidDiskIdMalformed'
 
+# 云硬盘类型非法。
+INVALIDPARAMETERVALUE_INVALIDDISKTYPE = 'InvalidParameterValue.InvalidDiskType'
+
 # 设置是否使用默认密钥对登录的值不正确。
 INVALIDPARAMETERVALUE_INVALIDINSTANCELOGINKEYPAIRPERMITLOGIN = 'InvalidParameterValue.InvalidInstanceLoginKeyPairPermitLogin'
 
 # 参数值非法，IP 地址格式非法。
 INVALIDPARAMETERVALUE_INVALIDIPFORMAT = 'InvalidParameterValue.InvalidIpFormat'
 
 # 参数值非法。
@@ -307,14 +316,20 @@
 
 # 不允许改变平台类型。
 INVALIDPARAMETERVALUE_NOTALLOWTOCHANGEPLATFORMTYPE = 'InvalidParameterValue.NotAllowToChangePlatformType'
 
 # 参数值非法，不在合法范围内。
 INVALIDPARAMETERVALUE_OUTOFRANGE = 'InvalidParameterValue.OutOfRange'
 
+# 实例操作系统不支持该文件系统。
+INVALIDPARAMETERVALUE_PLATFORMTYPENOTSUPPORTFILESYSTEM = 'InvalidParameterValue.PlatformTypeNotSupportFileSystem'
+
+# 实例操作系统不支持指定挂载点。
+INVALIDPARAMETERVALUE_PLATFORMTYPENOTSUPPORTMOUNTPOINT = 'InvalidParameterValue.PlatformTypeNotSupportMountPoint'
+
 # 地域不存在。
 INVALIDPARAMETERVALUE_REGIONNOTFOUND = 'InvalidParameterValue.RegionNotFound'
 
 # 地域不匹配。
 INVALIDPARAMETERVALUE_REGIONNOTMATCH = 'InvalidParameterValue.RegionNotMatch'
 
 # 不支持的地域。
@@ -343,14 +358,17 @@
 
 # 配额不足，当前自定义镜像配额不允许创建新的自定义镜像。
 LIMITEXCEEDED_BLUEPRINTQUOTALIMITEXCEEDED = 'LimitExceeded.BlueprintQuotaLimitExceeded'
 
 # 超过磁盘备份点配额限制。
 LIMITEXCEEDED_DISKBACKUPQUOTALIMITEXCEEDED = 'LimitExceeded.DiskBackupQuotaLimitExceeded'
 
+# 当前配额不足，无法创建新的云硬盘。
+LIMITEXCEEDED_DISKQUOTALIMITEXCEEDED = 'LimitExceeded.DiskQuotaLimitExceeded'
+
 # 超过防火墙规则配额。
 LIMITEXCEEDED_FIREWALLRULESLIMITEXCEEDED = 'LimitExceeded.FirewallRulesLimitExceeded'
 
 # 超过实例配额。
 LIMITEXCEEDED_INSTANCEQUOTALIMITEXCEEDED = 'LimitExceeded.InstanceQuotaLimitExceeded'
 
 # 退还资源数量超出限制。
@@ -583,12 +601,15 @@
 
 # 快照忙。
 UNSUPPORTEDOPERATION_SNAPSHOTBUSY = 'UnsupportedOperation.SnapshotBusy'
 
 # 系统忙。
 UNSUPPORTEDOPERATION_SYSTEMBUSY = 'UnsupportedOperation.SystemBusy'
 
+# 实例上腾讯云助手 agent 不在线。
+UNSUPPORTEDOPERATION_TATAGENTNOTONLINE = 'UnsupportedOperation.TatAgentNotOnline'
+
 # Windows实例不支持绑定密钥对。
 UNSUPPORTEDOPERATION_WINDOWSNOTALLOWTOASSOCIATEKEYPAIR = 'UnsupportedOperation.WindowsNotAllowToAssociateKeyPair'
 
 # windows类型实例不支持密钥对功能。
 UNSUPPORTEDOPERATION_WINDOWSNOTSUPPORTKEYPAIR = 'UnsupportedOperation.WindowsNotSupportKeyPair'
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,14 +198,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateDisks(self, request):
+        """本接口(CreateDisks)用于创建一个或多个云硬盘。
+
+        :param request: Request instance for CreateDisks.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.CreateDisksRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.CreateDisksResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateDisks", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateDisksResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateFirewallRules(self, request):
         """本接口（CreateFirewallRules）用于在实例上添加防火墙规则。
 
 
         * FirewallVersion 为防火墙版本号，用户每次更新防火墙规则版本会自动加1，防止您更新的规则已过期，不填不考虑冲突。
 
         在 FirewallRules 参数中：
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,46 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class AutoMountConfiguration(AbstractModel):
+    """自动挂载并初始化该数据盘。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 待挂载的实例ID。指定的实例必须处于“运行中”状态。
+        :type InstanceId: str
+        :param MountPoint: 实例内的挂载点。仅Linux操作系统的实例可传入该参数, 不传则默认挂载在“/data/disk”路径下。
+        :type MountPoint: str
+        :param FileSystemType: 文件系统类型。取值: “ext4”、“xfs”。仅Linux操作系统的实例可传入该参数, 不传则默认为“ext4”。
+        :type FileSystemType: str
+        """
+        self.InstanceId = None
+        self.MountPoint = None
+        self.FileSystemType = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.MountPoint = params.get("MountPoint")
+        self.FileSystemType = params.get("FileSystemType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class Blueprint(AbstractModel):
     """描述了镜像信息。
 
     """
 
     def __init__(self):
         r"""
@@ -744,14 +776,97 @@
 
 
     def _deserialize(self, params):
         self.DiskBackupId = params.get("DiskBackupId")
         self.RequestId = params.get("RequestId")
 
 
+class CreateDisksRequest(AbstractModel):
+    """CreateDisks请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Zone: 可用区。可通过[DescribeZones](https://cloud.tencent.com/document/product/1207/57513)返回值中的Zone获取。
+        :type Zone: str
+        :param DiskSize: 云硬盘大小, 单位: GB。
+        :type DiskSize: int
+        :param DiskType: 云硬盘介质类型。取值: "CLOUD_PREMIUM"(高性能云盘), "CLOUD_SSD"(SSD云硬盘)。
+        :type DiskType: str
+        :param DiskChargePrepaid: 云硬盘包年包月相关参数设置。
+        :type DiskChargePrepaid: :class:`tencentcloud.lighthouse.v20200324.models.DiskChargePrepaid`
+        :param DiskName: 云硬盘名称。最大长度60。
+        :type DiskName: str
+        :param DiskCount: 云硬盘个数。取值范围: [1, 30]。默认值: 1。
+        :type DiskCount: int
+        :param DiskBackupQuota: 指定云硬盘备份点配额，不传时默认为不带备份点配额。目前只支持不带或设置1个云硬盘备份点配额。
+        :type DiskBackupQuota: int
+        :param AutoVoucher: 是否自动使用代金券。默认不使用。
+        :type AutoVoucher: bool
+        :param AutoMountConfiguration: 自动挂载并初始化数据盘。
+        :type AutoMountConfiguration: :class:`tencentcloud.lighthouse.v20200324.models.AutoMountConfiguration`
+        """
+        self.Zone = None
+        self.DiskSize = None
+        self.DiskType = None
+        self.DiskChargePrepaid = None
+        self.DiskName = None
+        self.DiskCount = None
+        self.DiskBackupQuota = None
+        self.AutoVoucher = None
+        self.AutoMountConfiguration = None
+
+
+    def _deserialize(self, params):
+        self.Zone = params.get("Zone")
+        self.DiskSize = params.get("DiskSize")
+        self.DiskType = params.get("DiskType")
+        if params.get("DiskChargePrepaid") is not None:
+            self.DiskChargePrepaid = DiskChargePrepaid()
+            self.DiskChargePrepaid._deserialize(params.get("DiskChargePrepaid"))
+        self.DiskName = params.get("DiskName")
+        self.DiskCount = params.get("DiskCount")
+        self.DiskBackupQuota = params.get("DiskBackupQuota")
+        self.AutoVoucher = params.get("AutoVoucher")
+        if params.get("AutoMountConfiguration") is not None:
+            self.AutoMountConfiguration = AutoMountConfiguration()
+            self.AutoMountConfiguration._deserialize(params.get("AutoMountConfiguration"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateDisksResponse(AbstractModel):
+    """CreateDisks返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DiskIdSet: 当通过本接口来创建云硬盘时会返回该参数，表示一个或多个云硬盘ID。返回云硬盘ID列表并不代表云硬盘创建成功。
+
+可根据 [DescribeDisks](https://cloud.tencent.com/document/product/1207/66093) 接口查询返回的DiskSet中对应云硬盘的ID的状态来判断创建是否完成；如果云硬盘状态由“PENDING”变为“UNATTACHED”或“ATTACHED”，则为创建成功。
+        :type DiskIdSet: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DiskIdSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.DiskIdSet = params.get("DiskIdSet")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateFirewallRulesRequest(AbstractModel):
     """CreateFirewallRules请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5684,19 +5799,19 @@
     """折扣详情信息。
 
     """
 
     def __init__(self):
         r"""
         :param UserDiscount: 用户折扣。
-        :type UserDiscount: int
+        :type UserDiscount: float
         :param CommonDiscount: 公共折扣。
-        :type CommonDiscount: int
+        :type CommonDiscount: float
         :param FinalDiscount: 最终折扣。
-        :type FinalDiscount: int
+        :type FinalDiscount: float
         :param ActivityDiscount: 活动折扣。取值为null，表示无有效值，即没有折扣。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ActivityDiscount: float
         :param DiscountType: 折扣类型。
 user：用户折扣; common：官网折扣; activity：活动折扣。 取值为null，表示无有效值，即没有折扣。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DiscountType: str
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.886/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.886/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.887/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.886/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.887/setup.py`

 * *Files identical despite different names*

