# Comparing `tmp/tencentcloud-sdk-python-cam-3.0.886.tar.gz` & `tmp/tencentcloud-sdk-python-cam-3.0.887.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cam-3.0.886.tar", last modified: Mon May  8 02:54:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cam-3.0.887.tar", last modified: Tue May  9 02:29:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cam-3.0.886.tar` & `tencentcloud-sdk-python-cam-3.0.887.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud/cam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud/cam/v20190116/
--rw-r--r--   0 root         (0) root         (0)    78006 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud/cam/v20190116/cam_client.py
--rw-r--r--   0 root         (0) root         (0)    10965 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud/cam/v20190116/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud/cam/v20190116/__init__.py
--rw-r--r--   0 root         (0) root         (0)   188126 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud/cam/v20190116/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud/cam/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud_sdk_python_cam.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud_sdk_python_cam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud_sdk_python_cam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud_sdk_python_cam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 02:54:11.000000 tencentcloud-sdk-python-cam-3.0.886/tencentcloud_sdk_python_cam.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/
+-rw-r--r--   0 root         (0) root         (0)    78006 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/cam_client.py
+-rw-r--r--   0 root         (0) root         (0)    10965 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   188126 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud_sdk_python_cam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud_sdk_python_cam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud_sdk_python_cam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud_sdk_python_cam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud_sdk_python_cam.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cam-3.0.886/README.rst` & `tencentcloud-sdk-python-cam-3.0.887/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.886/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cam-3.0.887/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cam-3.0.886/tencentcloud/cam/v20190116/cam_client.py` & `tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/cam_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.886/tencentcloud/cam/v20190116/errorcodes.py` & `tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.886/tencentcloud/cam/v20190116/models.py` & `tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.886/PKG-INFO` & `tencentcloud-sdk-python-cam-3.0.887/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cam
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Cam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cam-3.0.886/setup.py` & `tencentcloud-sdk-python-cam-3.0.887/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.886/tencentcloud_sdk_python_cam.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cam-3.0.887/tencentcloud_sdk_python_cam.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cam
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Cam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

