# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.886.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.887.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.886.tar", last modified: Mon May  8 03:39:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.887.tar", last modified: Tue May  9 03:10:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.886.tar` & `tencentcloud-sdk-python-ocr-3.0.887.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   108933 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   505378 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:39:21.000000 tencentcloud-sdk-python-ocr-3.0.886/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   112684 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   505378 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:10:44.000000 tencentcloud-sdk-python-ocr-3.0.887/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.886/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.887/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.886/README.rst` & `tencentcloud-sdk-python-ocr-3.0.887/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.887/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1428,18 +1428,119 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def RecognizeGeneralInvoice(self, request):
-        """本接口支持 单张、多张、多类型 票据的混合识别，同时支持自选需要识别的票据类型，已支持票种包括：增值税发票（专票、普票、卷票）、全电发票、非税发票、定额发票、通用机打发票、购车发票、火车票、出租车发票、机票行程单、汽车票、轮船票、过路过桥费发票共14种标准报销发票，并支持其他类发票的识别。
+        """本接口支持 PDF多页、一页中单张、多张、类型票据的混合识别，同时支持单选识别某类票据，已支持票种包括：增值税发票（专票、普票、卷票、区块链发票、通行费发票）、全电发票（专票、普票）、非税发票（通用票据、统一缴纳书）、定额发票、通用机打发票、购车发票（机动车销售发票、二手车发票）、火车票、出租车发票、机票行程单、汽车票、轮船票、过路过桥费发票共14种标准报销发票，并支持非上述类型的其他发票的智能识别。
 
         默认接口请求频率限制：5次/秒。
 
+
+        支持的细项目子票种SubType、子票种中文TypeDescription 返回说明如下列表：
+        <table style="width:715px">
+              <thead>
+                <tr>
+                  <th style="width:200px">SubType 子票种英文</th>
+                  <th >TypeDescription子票种中文</th>
+                </tr>
+              </thead>
+              <tbody>
+                <tr>
+                  <td> VatSpecialInvoice</td>
+                  <td> 增值税专用发票 </td>
+                </tr>
+                <tr>
+                  <td> VatCommonInvoice</td>
+                  <td> 增值税普通发票 </td>
+                </tr>
+                <tr>
+                  <td> VatElectronicCommonInvoice </td>
+                  <td> 增值税电子普通发票 </td>
+                </tr>
+                <tr>
+                  <td> VatElectronicSpecialInvoice </td>
+                  <td> 增值税电子专用发票 </td>
+                </tr>
+                <tr>
+                  <td> VatElectronicInvoiceBlockchain</td>
+                  <td> 区块链电子发票 </td>
+                </tr>
+                <tr>
+                  <td> VatElectronicSpecialInvoiceFull</td>
+                  <td> 增值税电子普通发票(通行费)</td>
+                </tr>
+                <tr>
+                  <td> VatElectronicSpecialInvoiceFull</td>
+                  <td> 电子发票(专用发票)</td>
+                </tr>
+                <tr>
+                  <td> VatElectronicSpecialInvoiceFull</td>
+                  <td> 电子发票(普通发票) </td>
+                </tr>
+                <tr>
+                  <td> MotorVehicleSaleInvoice </td>
+                  <td> 机动车销售统一发票 </td>
+                </tr>
+                <tr>
+                  <td> UsedCarPurchaseInvoice </td>
+                  <td> 二手车销售统一发票 </td>
+                </tr>
+                <tr>
+                  <td> VatInvoiceRoll </td>
+                  <td> 增值税普通发票(卷票) </td>
+                </tr>
+                <tr>
+                  <td> TaxiTicket </td>
+                  <td> 出租车发票 </td>
+                </tr>
+                <tr>
+                  <td> QuotaInvoice </td>
+                  <td> 定额发票 </td>
+                </tr>
+                <tr>
+                  <td> TrainTicket </td>
+                  <td> 火车票 </td>
+                </tr>
+                <tr>
+                  <td> AirTransport </td>
+                  <td> 机票行程单 </td>
+                </tr>
+                <tr>
+                  <td> MachinePrintedInvoice </td>
+                  <td> 通用机打发票 </td>
+                </tr>
+                <tr>
+                  <td> BusInvoice </td>
+                  <td> 汽车票 </td>
+                </tr>
+                <tr>
+                  <td> ShippingInvoice </td>
+                  <td> 轮船票 </td>
+                </tr>
+                <tr>
+                  <td> NonTaxIncomeGeneralBill </td>
+                  <td> 非税收入通用票据 </td>
+                </tr>
+                <tr>
+                  <td> NonTaxIncomeElectronicBill </td>
+                  <td> 非税收入一般缴款书(电子) </td>
+                </tr>
+                <tr>
+                  <td> TollInvoice </td>
+                  <td> 过路过桥费发票 </td>
+                </tr>
+                <tr>
+                  <td> OtherInvoice </td>
+                  <td> 其他发票 </td>
+                </tr>
+              </tbody>
+            </table>
+
         :param request: Request instance for RecognizeGeneralInvoice.
         :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizeGeneralInvoiceRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.RecognizeGeneralInvoiceResponse`
 
         """
         try:
             params = request._serialize()
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.887/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.887/tencentcloud/ocr/v20181119/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.886/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.887/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.886/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.887/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.886/setup.py` & `tencentcloud-sdk-python-ocr-3.0.887/setup.py`

 * *Files identical despite different names*

