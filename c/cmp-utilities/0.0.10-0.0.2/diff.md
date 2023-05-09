# Comparing `tmp/cmp_utilities-0.0.10.tar.gz` & `tmp/cmp_utilities-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmp_utilities-0.0.10.tar", last modified: Thu Apr 13 08:41:35 2023, max compression
+gzip compressed data, was "cmp_utilities-0.0.2.tar", last modified: Thu Apr  6 07:05:14 2023, max compression
```

## Comparing `cmp_utilities-0.0.10.tar` & `cmp_utilities-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxr-xr-x   0 jheelpatel   (502) staff       (20)        0 2023-04-13 08:41:35.848452 cmp_utilities-0.0.10/
--rw-r--r--   0 jheelpatel   (502) staff       (20)    11357 2023-03-29 06:25:46.000000 cmp_utilities-0.0.10/LICENSE
--rw-r--r--   0 jheelpatel   (502) staff       (20)      581 2023-04-13 08:41:35.848138 cmp_utilities-0.0.10/PKG-INFO
--rw-r--r--   0 jheelpatel   (502) staff       (20)        0 2023-03-29 05:59:10.000000 cmp_utilities-0.0.10/README.md
--rw-r--r--   0 jheelpatel   (502) staff       (20)      911 2023-04-13 08:41:20.000000 cmp_utilities-0.0.10/pyproject.toml
--rw-r--r--   0 jheelpatel   (502) staff       (20)       38 2023-04-13 08:41:35.848515 cmp_utilities-0.0.10/setup.cfg
-drwxr-xr-x   0 jheelpatel   (502) staff       (20)        0 2023-04-13 08:41:35.836959 cmp_utilities-0.0.10/src/
-drwxr-xr-x   0 jheelpatel   (502) staff       (20)        0 2023-04-13 08:41:35.844438 cmp_utilities-0.0.10/src/cmp_utilities/
--rw-r--r--   0 jheelpatel   (502) staff       (20)        0 2023-03-29 05:43:34.000000 cmp_utilities-0.0.10/src/cmp_utilities/__init__.py
--rw-r--r--   0 jheelpatel   (502) staff       (20)     3470 2023-04-13 08:23:18.000000 cmp_utilities-0.0.10/src/cmp_utilities/bigquery.py
--rw-r--r--   0 jheelpatel   (502) staff       (20)     1276 2023-04-13 07:15:54.000000 cmp_utilities-0.0.10/src/cmp_utilities/credential.py
--rw-r--r--   0 jheelpatel   (502) staff       (20)      321 2023-04-13 08:40:23.000000 cmp_utilities-0.0.10/src/cmp_utilities/datetime_utils.py
--rw-r--r--   0 jheelpatel   (502) staff       (20)     1273 2023-04-06 04:01:20.000000 cmp_utilities-0.0.10/src/cmp_utilities/logging.py
--rw-r--r--   0 jheelpatel   (502) staff       (20)      887 2023-04-13 07:16:31.000000 cmp_utilities-0.0.10/src/cmp_utilities/monitoring.py
--rw-r--r--   0 jheelpatel   (502) staff       (20)      702 2023-04-06 06:25:10.000000 cmp_utilities-0.0.10/src/cmp_utilities/secret_manager.py
-drwxr-xr-x   0 jheelpatel   (502) staff       (20)        0 2023-04-13 08:41:35.847638 cmp_utilities-0.0.10/src/cmp_utilities.egg-info/
--rw-r--r--   0 jheelpatel   (502) staff       (20)      581 2023-04-13 08:41:35.000000 cmp_utilities-0.0.10/src/cmp_utilities.egg-info/PKG-INFO
--rw-r--r--   0 jheelpatel   (502) staff       (20)      461 2023-04-13 08:41:35.000000 cmp_utilities-0.0.10/src/cmp_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 jheelpatel   (502) staff       (20)        1 2023-04-13 08:41:35.000000 cmp_utilities-0.0.10/src/cmp_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 jheelpatel   (502) staff       (20)      181 2023-04-13 08:41:35.000000 cmp_utilities-0.0.10/src/cmp_utilities.egg-info/requires.txt
--rw-r--r--   0 jheelpatel   (502) staff       (20)       14 2023-04-13 08:41:35.000000 cmp_utilities-0.0.10/src/cmp_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 jheelpatel   (502) staff       (20)        0 2023-04-06 07:05:14.768112 cmp_utilities-0.0.2/
+-rw-r--r--   0 jheelpatel   (502) staff       (20)    11357 2023-03-29 06:25:46.000000 cmp_utilities-0.0.2/LICENSE
+-rw-r--r--   0 jheelpatel   (502) staff       (20)      580 2023-04-06 07:05:14.767826 cmp_utilities-0.0.2/PKG-INFO
+-rw-r--r--   0 jheelpatel   (502) staff       (20)        0 2023-03-29 05:59:10.000000 cmp_utilities-0.0.2/README.md
+-rw-r--r--   0 jheelpatel   (502) staff       (20)      785 2023-04-06 07:03:57.000000 cmp_utilities-0.0.2/pyproject.toml
+-rw-r--r--   0 jheelpatel   (502) staff       (20)       38 2023-04-06 07:05:14.768203 cmp_utilities-0.0.2/setup.cfg
+drwxr-xr-x   0 jheelpatel   (502) staff       (20)        0 2023-04-06 07:05:14.762828 cmp_utilities-0.0.2/src/
+drwxr-xr-x   0 jheelpatel   (502) staff       (20)        0 2023-04-06 07:05:14.765546 cmp_utilities-0.0.2/src/cmp_utilities/
+-rw-r--r--   0 jheelpatel   (502) staff       (20)        0 2023-03-29 05:43:34.000000 cmp_utilities-0.0.2/src/cmp_utilities/__init__.py
+-rw-r--r--   0 jheelpatel   (502) staff       (20)     1147 2023-03-29 06:45:36.000000 cmp_utilities-0.0.2/src/cmp_utilities/credential.py
+-rw-r--r--   0 jheelpatel   (502) staff       (20)     1273 2023-04-06 04:01:20.000000 cmp_utilities-0.0.2/src/cmp_utilities/logging.py
+-rw-r--r--   0 jheelpatel   (502) staff       (20)      702 2023-04-06 06:25:10.000000 cmp_utilities-0.0.2/src/cmp_utilities/secret_manager.py
+drwxr-xr-x   0 jheelpatel   (502) staff       (20)        0 2023-04-06 07:05:14.767396 cmp_utilities-0.0.2/src/cmp_utilities.egg-info/
+-rw-r--r--   0 jheelpatel   (502) staff       (20)      580 2023-04-06 07:05:14.000000 cmp_utilities-0.0.2/src/cmp_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 jheelpatel   (502) staff       (20)      363 2023-04-06 07:05:14.000000 cmp_utilities-0.0.2/src/cmp_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 jheelpatel   (502) staff       (20)        1 2023-04-06 07:05:14.000000 cmp_utilities-0.0.2/src/cmp_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 jheelpatel   (502) staff       (20)       84 2023-04-06 07:05:14.000000 cmp_utilities-0.0.2/src/cmp_utilities.egg-info/requires.txt
+-rw-r--r--   0 jheelpatel   (502) staff       (20)       14 2023-04-06 07:05:14.000000 cmp_utilities-0.0.2/src/cmp_utilities.egg-info/top_level.txt
```

### Comparing `cmp_utilities-0.0.10/LICENSE` & `cmp_utilities-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmp_utilities-0.0.10/PKG-INFO` & `cmp_utilities-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmp_utilities
-Version: 0.0.10
+Version: 0.0.2
 Summary: Utility modules for Cloud Management Platform
 Author-email: Jheel Patel <jheelpatelscientist@gmail.com>
 Project-URL: Homepage, https://github.com/extremize/CloudManagementPlatformPublic
 Project-URL: Bug Tracker, https://github.com/extremize/CloudManagementPlatformPublic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `cmp_utilities-0.0.10/src/cmp_utilities/credential.py` & `cmp_utilities-0.0.2/src/cmp_utilities/credential.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,11 @@
     def get_default_credentials(self):
         self.__credentials, project = default(
             quota_project_id=self.api_quota_project, scopes=self.scopes
         )
         return self.__credentials
 
     def get_auth_header(self):
-        self.__credentials, project = default(
-            quota_project_id=self.api_quota_project, scopes=self.scopes
-        )
         self.__credentials.refresh(Request())
         self.__auth_token = self.__credentials.token
         self.__auth_header = {"Authorization": f"Bearer {self.__auth_token}"}
         return self.__auth_header, self.__auth_token
```

### Comparing `cmp_utilities-0.0.10/src/cmp_utilities/logging.py` & `cmp_utilities-0.0.2/src/cmp_utilities/logging.py`

 * *Files identical despite different names*

### Comparing `cmp_utilities-0.0.10/src/cmp_utilities/secret_manager.py` & `cmp_utilities-0.0.2/src/cmp_utilities/secret_manager.py`

 * *Files identical despite different names*

### Comparing `cmp_utilities-0.0.10/src/cmp_utilities.egg-info/PKG-INFO` & `cmp_utilities-0.0.2/src/cmp_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmp-utilities
-Version: 0.0.10
+Version: 0.0.2
 Summary: Utility modules for Cloud Management Platform
 Author-email: Jheel Patel <jheelpatelscientist@gmail.com>
 Project-URL: Homepage, https://github.com/extremize/CloudManagementPlatformPublic
 Project-URL: Bug Tracker, https://github.com/extremize/CloudManagementPlatformPublic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

