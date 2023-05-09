# Comparing `tmp/tencentcloud-sdk-python-postgres-3.0.886.tar.gz` & `tmp/tencentcloud-sdk-python-postgres-3.0.887.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.886.tar", last modified: Mon May  8 03:42:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.887.tar", last modified: Tue May  9 03:11:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-postgres-3.0.886.tar` & `tencentcloud-sdk-python-postgres-3.0.887.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud/postgres/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)    84591 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud/postgres/v20170312/postgres_client.py
--rw-r--r--   0 root         (0) root         (0)    20657 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud/postgres/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   277276 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud_sdk_python_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:42:52.000000 tencentcloud-sdk-python-postgres-3.0.886/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud/postgres/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    84591 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud/postgres/v20170312/postgres_client.py
+-rw-r--r--   0 root         (0) root         (0)    20657 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud/postgres/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   277276 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud_sdk_python_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:11:21.000000 tencentcloud-sdk-python-postgres-3.0.887/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.886/README.rst` & `tencentcloud-sdk-python-postgres-3.0.887/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.886/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-postgres-3.0.887/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.886/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-postgres-3.0.887/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.886/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-postgres-3.0.887/tencentcloud/postgres/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.886/tencentcloud/__init__.py` & `tencentcloud-sdk-python-postgres-3.0.887/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-postgres-3.0.886/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.887/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.886/setup.py` & `tencentcloud-sdk-python-postgres-3.0.887/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.886/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.887/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```
