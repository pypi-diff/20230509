# Comparing `tmp/prompt_wrangler-0.4.0.tar.gz` & `tmp/prompt_wrangler-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_wrangler-0.4.0.tar", last modified: Tue May  2 17:13:05 2023, max compression
+gzip compressed data, was "prompt_wrangler-0.5.0.tar", last modified: Tue May  9 20:35:06 2023, max compression
```

## Comparing `prompt_wrangler-0.4.0.tar` & `prompt_wrangler-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,21 @@
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-02 17:13:05.765128 prompt_wrangler-0.4.0/
--rw-r--r--   0 maxshaw    (501) staff       (20)     3088 2023-05-02 16:50:16.000000 prompt_wrangler-0.4.0/.gitignore
--rw-r--r--   0 maxshaw    (501) staff       (20)     2032 2023-05-02 17:13:05.764977 prompt_wrangler-0.4.0/PKG-INFO
--rw-r--r--   0 maxshaw    (501) staff       (20)     1360 2023-05-02 16:49:04.000000 prompt_wrangler-0.4.0/README.md
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-02 17:13:05.762897 prompt_wrangler-0.4.0/__pycache__/
--rw-r--r--   0 maxshaw    (501) staff       (20)     1818 2023-05-02 17:03:17.000000 prompt_wrangler-0.4.0/__pycache__/test_mock.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 maxshaw    (501) staff       (20)     1883 2023-05-02 16:49:04.000000 prompt_wrangler-0.4.0/__pycache__/test_prompt_wrangler.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 maxshaw    (501) staff       (20)     1985 2023-05-02 17:13:00.000000 prompt_wrangler-0.4.0/__pycache__/test_real.cpython-310-pytest-7.2.2.pyc
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-02 17:13:05.763463 prompt_wrangler-0.4.0/prompt_wrangler/
--rw-r--r--   0 maxshaw    (501) staff       (20)       73 2023-05-02 17:03:07.000000 prompt_wrangler-0.4.0/prompt_wrangler/__init__.py
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-02 17:13:05.764730 prompt_wrangler-0.4.0/prompt_wrangler/__pycache__/
--rw-r--r--   0 maxshaw    (501) staff       (20)      290 2023-05-02 17:03:18.000000 prompt_wrangler-0.4.0/prompt_wrangler/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 maxshaw    (501) staff       (20)     4342 2023-05-02 17:11:31.000000 prompt_wrangler-0.4.0/prompt_wrangler/__pycache__/client.cpython-310.pyc
--rw-r--r--   0 maxshaw    (501) staff       (20)     4027 2023-05-02 17:09:04.000000 prompt_wrangler-0.4.0/prompt_wrangler/client.py
--rw-r--r--   0 maxshaw    (501) staff       (20)      560 2023-05-02 17:02:57.000000 prompt_wrangler-0.4.0/prompt_wrangler/client.pyi
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-02 17:13:05.764382 prompt_wrangler-0.4.0/prompt_wrangler.egg-info/
--rw-r--r--   0 maxshaw    (501) staff       (20)     2032 2023-05-02 17:13:05.000000 prompt_wrangler-0.4.0/prompt_wrangler.egg-info/PKG-INFO
--rw-r--r--   0 maxshaw    (501) staff       (20)      623 2023-05-02 17:13:05.000000 prompt_wrangler-0.4.0/prompt_wrangler.egg-info/SOURCES.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)        1 2023-05-02 17:13:05.000000 prompt_wrangler-0.4.0/prompt_wrangler.egg-info/dependency_links.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)        9 2023-05-02 17:13:05.000000 prompt_wrangler-0.4.0/prompt_wrangler.egg-info/requires.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)       16 2023-05-02 17:13:05.000000 prompt_wrangler-0.4.0/prompt_wrangler.egg-info/top_level.txt
--rwxr-xr-x   0 maxshaw    (501) staff       (20)      866 2023-05-02 16:49:04.000000 prompt_wrangler-0.4.0/publish.sh
--rw-r--r--   0 maxshaw    (501) staff       (20)        0 2023-05-02 16:49:04.000000 prompt_wrangler-0.4.0/run_prompt.py
--rw-r--r--   0 maxshaw    (501) staff       (20)       38 2023-05-02 17:13:05.765187 prompt_wrangler-0.4.0/setup.cfg
--rw-r--r--   0 maxshaw    (501) staff       (20)     1062 2023-05-02 17:13:05.000000 prompt_wrangler-0.4.0/setup.py
--rw-r--r--   0 maxshaw    (501) staff       (20)      918 2023-05-02 17:03:15.000000 prompt_wrangler-0.4.0/test_mock.py
--rw-r--r--   0 maxshaw    (501) staff       (20)      971 2023-05-02 17:07:40.000000 prompt_wrangler-0.4.0/test_real.py
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-09 20:35:06.331799 prompt_wrangler-0.5.0/
+-rw-r--r--   0 maxshaw    (501) staff       (20)     3088 2023-05-02 16:50:16.000000 prompt_wrangler-0.5.0/.gitignore
+-rw-r--r--   0 maxshaw    (501) staff       (20)     2032 2023-05-09 20:35:06.331644 prompt_wrangler-0.5.0/PKG-INFO
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1360 2023-05-02 16:49:04.000000 prompt_wrangler-0.5.0/README.md
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-09 20:35:06.330543 prompt_wrangler-0.5.0/prompt_wrangler/
+-rw-r--r--   0 maxshaw    (501) staff       (20)       73 2023-05-07 20:37:59.000000 prompt_wrangler-0.5.0/prompt_wrangler/__init__.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)     4484 2023-05-09 20:34:28.000000 prompt_wrangler-0.5.0/prompt_wrangler/client.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)      560 2023-05-07 20:37:59.000000 prompt_wrangler-0.5.0/prompt_wrangler/client.pyi
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-09 20:35:06.331392 prompt_wrangler-0.5.0/prompt_wrangler.egg-info/
+-rw-r--r--   0 maxshaw    (501) staff       (20)     2032 2023-05-09 20:35:06.000000 prompt_wrangler-0.5.0/prompt_wrangler.egg-info/PKG-INFO
+-rw-r--r--   0 maxshaw    (501) staff       (20)      365 2023-05-09 20:35:06.000000 prompt_wrangler-0.5.0/prompt_wrangler.egg-info/SOURCES.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)        1 2023-05-09 20:35:06.000000 prompt_wrangler-0.5.0/prompt_wrangler.egg-info/dependency_links.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)        9 2023-05-09 20:35:06.000000 prompt_wrangler-0.5.0/prompt_wrangler.egg-info/requires.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)       16 2023-05-09 20:35:06.000000 prompt_wrangler-0.5.0/prompt_wrangler.egg-info/top_level.txt
+-rwxr-xr-x   0 maxshaw    (501) staff       (20)      866 2023-05-02 16:49:04.000000 prompt_wrangler-0.5.0/publish.sh
+-rw-r--r--   0 maxshaw    (501) staff       (20)        0 2023-05-02 16:49:04.000000 prompt_wrangler-0.5.0/run_prompt.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)       38 2023-05-09 20:35:06.331856 prompt_wrangler-0.5.0/setup.cfg
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1062 2023-05-09 20:35:05.000000 prompt_wrangler-0.5.0/setup.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)        0 2023-05-07 20:37:59.000000 prompt_wrangler-0.5.0/test.json
+-rw-r--r--   0 maxshaw    (501) staff       (20)      918 2023-05-07 20:37:59.000000 prompt_wrangler-0.5.0/test_mock.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)      971 2023-05-07 20:37:59.000000 prompt_wrangler-0.5.0/test_real.py
```

### Comparing `prompt_wrangler-0.4.0/.gitignore` & `prompt_wrangler-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.4.0/PKG-INFO` & `prompt_wrangler-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt_wrangler
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python wrapper for the Prompt Wrangler REST API.
 Home-page: UNKNOWN
 Author: Max Shaw
 Author-email: max@exit38.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prompt_wrangler-0.4.0/README.md` & `prompt_wrangler-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.4.0/prompt_wrangler/client.py` & `prompt_wrangler-0.5.0/prompt_wrangler/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 import requests
 from typing import Any, Dict, Optional
 import os
+from tenacity import (
+    retry,
+    stop_after_attempt,
+    wait_exponential,
+    retry_if_exception_type,
+)
 
 
 class APIException(Exception):
     def __init__(self, response):
         self.status_code = response.status_code
         self.reason = response.reason
         self.text = response.text
         super().__init__(
             f"Status code: {self.status_code}, Reason: {self.reason}, Response body: {self.text}"
         )
 
 
+class APIException5xx(APIException):
+    """Exception raised for 5xx status codes."""
+
+
+@retry(
+    stop=stop_after_attempt(3),
+    wait=wait_exponential(multiplier=1, min=1, max=10),
+    retry=retry_if_exception_type(APIException5xx),
+)
 def make_request(url, method="GET", headers=None, params=None, data=None):
     if method.upper() == "GET":
         response = requests.get(url, headers=headers, params=params)
     elif method.upper() == "POST":
         response = requests.post(url, headers=headers, params=params, json=data)
     else:
         raise ValueError(f"Unsupported method: {method}")
@@ -27,15 +42,18 @@
     else:
         # Print response details
         print(
             f"Status code: {response.status_code}, Reason: {response.reason}, Response body: {response.text}"
         )
 
         # Raise custom exception with response details
-        raise APIException(response)
+        if 500 <= response.status_code < 600:
+            raise APIException5xx(response)
+        else:
+            raise APIException(response)
 
 
 class PromptWrangler:
     """Prompt Wrangler client."""
 
     def __init__(self, base_url: str = "https://prompt-wrangler.com/api") -> None:
         """
```

### Comparing `prompt_wrangler-0.4.0/prompt_wrangler/client.pyi` & `prompt_wrangler-0.5.0/prompt_wrangler/client.pyi`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.4.0/prompt_wrangler.egg-info/PKG-INFO` & `prompt_wrangler-0.5.0/prompt_wrangler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-wrangler
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python wrapper for the Prompt Wrangler REST API.
 Home-page: UNKNOWN
 Author: Max Shaw
 Author-email: max@exit38.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prompt_wrangler-0.4.0/publish.sh` & `prompt_wrangler-0.5.0/publish.sh`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.4.0/setup.py` & `prompt_wrangler-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="prompt_wrangler",
-    version="0.4.0",
+    version="0.5.0",
     author="Max Shaw",
     author_email="max@exit38.org",
     description="A Python wrapper for the Prompt Wrangler REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/exit38/prompt_wrangler",
     packages=find_packages(),
```

### Comparing `prompt_wrangler-0.4.0/test_mock.py` & `prompt_wrangler-0.5.0/test_mock.py`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.4.0/test_real.py` & `prompt_wrangler-0.5.0/test_real.py`

 * *Files identical despite different names*

