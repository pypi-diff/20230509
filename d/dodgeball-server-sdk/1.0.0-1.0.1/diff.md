# Comparing `tmp/dodgeball_server_sdk-1.0.0.tar.gz` & `tmp/dodgeball_server_sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodgeball_server_sdk-1.0.0.tar", max compression
+gzip compressed data, was "dodgeball_server_sdk-1.0.1.tar", max compression
```

## Comparing `dodgeball_server_sdk-1.0.0.tar` & `dodgeball_server_sdk-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-04-27 04:44:36.319320 dodgeball_server_sdk-1.0.0/LICENSE
--rw-r--r--   0        0        0    17676 2023-05-04 15:19:04.152375 dodgeball_server_sdk-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-02 04:21:23.248082 dodgeball_server_sdk-1.0.0/dodgeball/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 09:14:02.297361 dodgeball_server_sdk-1.0.0/dodgeball/api/__init__.py
--rw-r--r--   0        0        0    12914 2023-05-07 09:16:31.721813 dodgeball_server_sdk-1.0.0/dodgeball/api/dodgeball.py
--rw-r--r--   0        0        0      444 2023-05-04 09:28:16.878189 dodgeball_server_sdk-1.0.0/dodgeball/api/dodgeball_config.py
--rw-r--r--   0        0        0        0 2023-05-03 02:31:59.011754 dodgeball_server_sdk-1.0.0/dodgeball/interfaces/__init__.py
--rw-r--r--   0        0        0     1664 2023-05-07 09:32:08.644370 dodgeball_server_sdk-1.0.0/dodgeball/interfaces/api_types.py
--rw-r--r--   0        0        0        0 2023-05-02 18:28:40.020058 dodgeball_server_sdk-1.0.0/dodgeball/utils/__init__.py
--rw-r--r--   0        0        0      613 2023-05-04 09:44:54.544731 dodgeball_server_sdk-1.0.0/dodgeball/utils/logging.py
--rw-r--r--   0        0        0     6634 2023-05-07 09:34:07.402596 dodgeball_server_sdk-1.0.0/dodgeball/utils/query_utils.py
--rw-r--r--   0        0        0      574 2023-05-08 03:44:04.294053 dodgeball_server_sdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    18464 1970-01-01 00:00:00.000000 dodgeball_server_sdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-27 04:44:36.319320 dodgeball_server_sdk-1.0.1/LICENSE
+-rw-r--r--   0        0        0    17676 2023-05-04 15:19:04.152375 dodgeball_server_sdk-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 04:21:23.248082 dodgeball_server_sdk-1.0.1/dodgeball/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 09:14:02.297361 dodgeball_server_sdk-1.0.1/dodgeball/api/__init__.py
+-rw-r--r--   0        0        0    12914 2023-05-09 04:05:52.367118 dodgeball_server_sdk-1.0.1/dodgeball/api/dodgeball.py
+-rw-r--r--   0        0        0      444 2023-05-04 09:28:16.878189 dodgeball_server_sdk-1.0.1/dodgeball/api/dodgeball_config.py
+-rw-r--r--   0        0        0        0 2023-05-03 02:31:59.011754 dodgeball_server_sdk-1.0.1/dodgeball/interfaces/__init__.py
+-rw-r--r--   0        0        0     1684 2023-05-09 04:05:52.367612 dodgeball_server_sdk-1.0.1/dodgeball/interfaces/api_types.py
+-rw-r--r--   0        0        0        0 2023-05-02 18:28:40.020058 dodgeball_server_sdk-1.0.1/dodgeball/utils/__init__.py
+-rw-r--r--   0        0        0      613 2023-05-04 09:44:54.544731 dodgeball_server_sdk-1.0.1/dodgeball/utils/logging.py
+-rw-r--r--   0        0        0     6634 2023-05-09 04:05:52.368436 dodgeball_server_sdk-1.0.1/dodgeball/utils/query_utils.py
+-rw-r--r--   0        0        0      574 2023-05-09 04:06:27.506182 dodgeball_server_sdk-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    18464 1970-01-01 00:00:00.000000 dodgeball_server_sdk-1.0.1/PKG-INFO
```

### Comparing `dodgeball_server_sdk-1.0.0/LICENSE` & `dodgeball_server_sdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dodgeball_server_sdk-1.0.0/README.md` & `dodgeball_server_sdk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dodgeball_server_sdk-1.0.0/dodgeball/api/dodgeball.py` & `dodgeball_server_sdk-1.0.1/dodgeball/api/dodgeball.py`

 * *Files identical despite different names*

### Comparing `dodgeball_server_sdk-1.0.0/dodgeball/interfaces/api_types.py` & `dodgeball_server_sdk-1.0.1/dodgeball/interfaces/api_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,11 +74,11 @@
     stepData: Optional[VerificationStepData]
     nextSteps: Optional[List[VerificationStep]]
     error: Optional[DodgeballError]
 
 
 class DodgeballCheckpointResponse(DodgeballResponse):
     success: bool
-    errors: List[DodgeballError]
-    version: str
+    errors: Optional[List[DodgeballError]]
+    version: Optional[str]
     verification: Optional[DodgeballVerification]
     isTimeout: Optional[bool]
```

### Comparing `dodgeball_server_sdk-1.0.0/dodgeball/utils/logging.py` & `dodgeball_server_sdk-1.0.1/dodgeball/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dodgeball_server_sdk-1.0.0/dodgeball/utils/query_utils.py` & `dodgeball_server_sdk-1.0.1/dodgeball/utils/query_utils.py`

 * *Files identical despite different names*

### Comparing `dodgeball_server_sdk-1.0.0/pyproject.toml` & `dodgeball_server_sdk-1.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dodgeball-server-sdk"
-version = "1.0.0"
+version = "1.0.1"
 description = "The Dodgeball Trust Server SDK for Python"
 authors = ["Andrew Schwartz <tools@dodgeballhq.com>",
 "Patrick Teague <sdk@dodgeballhq.com>"]
 readme = "README.md"
 packages = [{include = "dodgeball"}]
 
 [tool.poetry.dependencies]
```

### Comparing `dodgeball_server_sdk-1.0.0/PKG-INFO` & `dodgeball_server_sdk-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dodgeball-server-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: The Dodgeball Trust Server SDK for Python
 Author: Andrew Schwartz
 Author-email: tools@dodgeballhq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

