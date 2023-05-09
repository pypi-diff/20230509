# Comparing `tmp/rmmbr-0.0.3.tar.gz` & `tmp/rmmbr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmmbr-0.0.3.tar", last modified: Tue Apr 18 14:55:24 2023, max compression
+gzip compressed data, was "rmmbr-0.0.4.tar", last modified: Tue May  9 13:05:15 2023, max compression
```

## Comparing `rmmbr-0.0.3.tar` & `rmmbr-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:24.496362 rmmbr-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-18 14:55:24.496362 rmmbr-0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:24.496362 rmmbr-0.0.3/rmmbr/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-18 14:55:16.000000 rmmbr-0.0.3/rmmbr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-18 14:55:16.000000 rmmbr-0.0.3/rmmbr/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-18 14:55:16.000000 rmmbr-0.0.3/rmmbr/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:55:24.496362 rmmbr-0.0.3/rmmbr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-18 14:55:24.000000 rmmbr-0.0.3/rmmbr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 14:55:24.000000 rmmbr-0.0.3/rmmbr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:55:24.000000 rmmbr-0.0.3/rmmbr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-18 14:55:24.000000 rmmbr-0.0.3/rmmbr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 14:55:24.000000 rmmbr-0.0.3/rmmbr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 14:55:24.000000 rmmbr-0.0.3/rmmbr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:55:24.496362 rmmbr-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-18 14:55:16.000000 rmmbr-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:05:15.798818 rmmbr-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-09 13:05:15.798818 rmmbr-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:05:15.798818 rmmbr-0.0.4/rmmbr/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 13:05:03.000000 rmmbr-0.0.4/rmmbr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-09 13:05:03.000000 rmmbr-0.0.4/rmmbr/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-09 13:05:03.000000 rmmbr-0.0.4/rmmbr/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-09 13:05:03.000000 rmmbr-0.0.4/rmmbr/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 13:05:03.000000 rmmbr-0.0.4/rmmbr/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:05:15.798818 rmmbr-0.0.4/rmmbr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-09 13:05:15.000000 rmmbr-0.0.4/rmmbr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-09 13:05:15.000000 rmmbr-0.0.4/rmmbr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:05:15.000000 rmmbr-0.0.4/rmmbr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-09 13:05:15.000000 rmmbr-0.0.4/rmmbr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-09 13:05:15.000000 rmmbr-0.0.4/rmmbr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 13:05:15.000000 rmmbr-0.0.4/rmmbr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:05:15.798818 rmmbr-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-09 13:05:03.000000 rmmbr-0.0.4/setup.py
```

### Comparing `rmmbr-0.0.3/PKG-INFO` & `rmmbr-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmmbr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple persistent caching.
 Home-page: https://github.com/uriva/rmmbr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
@@ -42,14 +42,26 @@
 const cacher = cloudCache({
   token: "service-token",
   url: "https://uriva-rmmbr.deno.dev",
   ttl: 60 * 60 * 24, // Values will expire after one day, omission of this field implies max.
 });
 ```
 
+If your data is sensitive, you can encrypt it by adding an `encryptionKey` parameter:
+
+```js
+const cacher = cloudCache({
+  token: "service-token",
+  url: "https://uriva-rmmbr.deno.dev",
+  encryptionKey: "eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee",
+});
+```
+
+Note that this is implemented as e2e encryption.
+
 At the moment this service is with no guarantees, but we are working on a production tier as well. Please contact us or post an issue if you want to try it out!
 
 We also accept issues for feature requests 👩‍🔧
 
 ## Python
 
 ```sh
```

### Comparing `rmmbr-0.0.3/rmmbr/main_test.py` & `rmmbr-0.0.4/rmmbr/main_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from rmmbr import cloud_cache, local_cache, mem_cache
-import redis.asyncio as redis
-
 import asyncio
-import dotenv
 import pathlib
 
+import dotenv
+import redis.asyncio as redis
+
+from rmmbr import cloud_cache, local_cache, mem_cache
+
 
 def _cache_test_helper(instance_implies_new_cache: bool, expires_after_2_seconds: bool):
     async def inner(cacher):
         n_called = 0
 
         async def f(x):
             nonlocal n_called
@@ -58,25 +59,38 @@
 async def _clean_redis():
     redis_client = await redis.Redis(
         password=_env_param("REDIS_PASSWORD"),
         host=_env_param("REDIS_URL"),
         port=int(_env_param("REDIS_PORT")),
     )
     await redis_client.flushall()
+    await redis_client.set("api-token:some-token", "testing|my-uid")
 
 
 _port = _env_param("PORT")
 _mock_backend_url = f"http://localhost:{_port}"
 
 
 async def test_cloud_cache():
     await _clean_redis()
     await _cache_test_helper(False, False)(
-        cloud_cache("some-token", _mock_backend_url, None)
+        cloud_cache("some-token", _mock_backend_url, None, None)
     )
 
 
 async def test_cloud_cache_expiration():
     await _clean_redis()
     await _cache_test_helper(False, True)(
-        cloud_cache("some-token", _mock_backend_url, 1)
+        cloud_cache("some-token", _mock_backend_url, 1, None)
+    )
+
+
+async def test_cloud_cache_encryption():
+    await _clean_redis()
+    await _cache_test_helper(False, False)(
+        cloud_cache(
+            "some-token",
+            _mock_backend_url,
+            None,
+            "Cqq33cbHu9AEUaP_wS3LCDQN7wy40XKWzALoPHbU5S8=",
+        )
     )
```

### Comparing `rmmbr-0.0.3/rmmbr.egg-info/PKG-INFO` & `rmmbr-0.0.4/rmmbr.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmmbr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple persistent caching.
 Home-page: https://github.com/uriva/rmmbr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
@@ -42,14 +42,26 @@
 const cacher = cloudCache({
   token: "service-token",
   url: "https://uriva-rmmbr.deno.dev",
   ttl: 60 * 60 * 24, // Values will expire after one day, omission of this field implies max.
 });
 ```
 
+If your data is sensitive, you can encrypt it by adding an `encryptionKey` parameter:
+
+```js
+const cacher = cloudCache({
+  token: "service-token",
+  url: "https://uriva-rmmbr.deno.dev",
+  encryptionKey: "eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee",
+});
+```
+
+Note that this is implemented as e2e encryption.
+
 At the moment this service is with no guarantees, but we are working on a production tier as well. Please contact us or post an issue if you want to try it out!
 
 We also accept issues for feature requests 👩‍🔧
 
 ## Python
 
 ```sh
```

### Comparing `rmmbr-0.0.3/setup.py` & `rmmbr-0.0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from setuptools import setup, find_packages
-import pathlib
 import os
+import pathlib
+
+from setuptools import find_packages, setup
 
 _repo_dir = os.environ.get("GITHUB_WORKSPACE")
 assert _repo_dir
 setup(
     name="rmmbr",
-    version="0.0.3",
+    version="0.0.4",
     description="Simple persistent caching.",
     long_description=(pathlib.Path(_repo_dir) / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/uriva/rmmbr",
     packages=find_packages(),
     install_requires=[
         "redis>=3.5.3",
         "python-dotenv>=0.17.1",
+        "cryptography>=40.0.2",
         "pytest",
         "httpx",
         "aiofiles",
         "pytest-asyncio",
     ],
     entry_points={"console_scripts": ["cache=cache.cli:main"]},
     classifiers=[
```

