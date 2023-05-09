# Comparing `tmp/pine_client-0.1.2.tar.gz` & `tmp/pine_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pine_client-0.1.2.tar", max compression
+gzip compressed data, was "pine_client-0.1.3.tar", max compression
```

## Comparing `pine_client-0.1.2.tar` & `pine_client-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       95 2023-05-08 14:55:52.000000 pine_client-0.1.2/README.md
--rw-r--r--   0        0        0       60 2023-05-08 14:55:52.000000 pine_client-0.1.2/pine_client/__init__.py
--rw-r--r--   0        0        0    32326 2023-05-08 14:55:52.000000 pine_client-0.1.2/pine_client/client.py
--rw-r--r--   0        0        0     2659 2023-05-08 14:55:52.000000 pine_client-0.1.2/pine_client/utils.py
--rw-r--r--   0        0        0      505 2023-05-08 14:56:04.000000 pine_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 pine_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       95 2023-05-09 17:02:12.000000 pine_client-0.1.3/README.md
+-rw-r--r--   0        0        0       60 2023-05-09 17:02:12.000000 pine_client-0.1.3/pine_client/__init__.py
+-rw-r--r--   0        0        0    32329 2023-05-09 17:02:12.000000 pine_client-0.1.3/pine_client/client.py
+-rw-r--r--   0        0        0     2659 2023-05-09 17:02:12.000000 pine_client-0.1.3/pine_client/utils.py
+-rw-r--r--   0        0        0      505 2023-05-09 17:02:27.000000 pine_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 pine_client-0.1.3/PKG-INFO
```

### Comparing `pine_client-0.1.2/pine_client/client.py` & `pine_client-0.1.3/pine_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -860,15 +860,15 @@
 
         post_params: Params = {**remaining_params, "body": {**id, **body}}
 
         try:
             return self.post(post_params)
         except Exception as e:
             is_unique_violation_response = False
-            if re.search(r"unique", e.body, re.IGNORECASE):  # type: ignore
+            if re.search(r"unique", e.message, re.IGNORECASE):  # type: ignore
                 if e.status_code == 409:  # type: ignore
                     is_unique_violation_response = True
 
             if not is_unique_violation_response:
                 raise e
 
             options = remaining_params.get("options", {})
```

### Comparing `pine_client-0.1.2/pine_client/utils.py` & `pine_client-0.1.3/pine_client/utils.py`

 * *Files identical despite different names*

### Comparing `pine_client-0.1.2/PKG-INFO` & `pine_client-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pine-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: This module provides the core layer for python interface for the pinejs API
 Author: Balena
 Author-email: info@balena.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

