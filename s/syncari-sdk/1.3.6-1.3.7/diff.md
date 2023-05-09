# Comparing `tmp/syncari-sdk-1.3.6.tar.gz` & `tmp/syncari-sdk-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncari-sdk-1.3.6.tar", last modified: Thu May  4 23:36:04 2023, max compression
+gzip compressed data, was "dist/syncari-sdk-1.3.7.tar", last modified: Tue May  9 19:34:30 2023, max compression
```

## Comparing `syncari-sdk-1.3.6.tar` & `syncari-sdk-1.3.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.868011 syncari-sdk-1.3.6/
--rw-r--r--   0 blesson    (501) staff       (20)      338 2023-05-04 23:36:04.867882 syncari-sdk-1.3.6/PKG-INFO
--rw-r--r--   0 blesson    (501) staff       (20)       78 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/README.md
--rw-r--r--   0 blesson    (501) staff       (20)       38 2023-05-04 23:36:04.868048 syncari-sdk-1.3.6/setup.cfg
--rwxr-xr-x   0 blesson    (501) staff       (20)      562 2023-05-04 23:35:07.000000 syncari-sdk-1.3.6/setup.py
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.860679 syncari-sdk-1.3.6/syncari/
--rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/__init__.py
--rw-r--r--   0 blesson    (501) staff       (20)      699 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/logger.py
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.861587 syncari-sdk-1.3.6/syncari/models/
--rw-r--r--   0 blesson    (501) staff       (20)       64 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/models/__init__.py
--rw-r--r--   0 blesson    (501) staff       (20)     3935 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/models/core.py
--rw-r--r--   0 blesson    (501) staff       (20)     2505 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/models/request.py
--rw-r--r--   0 blesson    (501) staff       (20)     2273 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/models/schema.py
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.861841 syncari-sdk-1.3.6/syncari/rest/
--rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/rest/__init__.py
--rw-r--r--   0 blesson    (501) staff       (20)     4010 2023-05-04 23:35:13.000000 syncari-sdk-1.3.6/syncari/rest/client.py
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.862562 syncari-sdk-1.3.6/syncari/synapse/
--rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/synapse/__init__.py
--rw-r--r--   0 blesson    (501) staff       (20)    10308 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/synapse/abstract_synapse.py
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.863263 syncari-sdk-1.3.6/syncari_sdk.egg-info/
--rw-r--r--   0 blesson    (501) staff       (20)      338 2023-05-04 23:36:04.000000 syncari-sdk-1.3.6/syncari_sdk.egg-info/PKG-INFO
--rw-r--r--   0 blesson    (501) staff       (20)      569 2023-05-04 23:36:04.000000 syncari-sdk-1.3.6/syncari_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 blesson    (501) staff       (20)        1 2023-05-04 23:36:04.000000 syncari-sdk-1.3.6/syncari_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 blesson    (501) staff       (20)       47 2023-05-04 23:36:04.000000 syncari-sdk-1.3.6/syncari_sdk.egg-info/requires.txt
--rw-r--r--   0 blesson    (501) staff       (20)       19 2023-05-04 23:36:04.000000 syncari-sdk-1.3.6/syncari_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.867687 syncari-sdk-1.3.6/unit_tests/
--rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/unit_tests/__init__.py
--rw-r--r--   0 blesson    (501) staff       (20)     7319 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/unit_tests/test_mock_synapse.py
--rw-r--r--   0 blesson    (501) staff       (20)     6299 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/unit_tests/test_response_validations.py
--rw-r--r--   0 blesson    (501) staff       (20)     1962 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/unit_tests/test_rest_client.py
+drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/
+-rw-r--r--   0 vraman     (501) staff       (20)      373 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/PKG-INFO
+drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari/
+-rw-r--r--   0 vraman     (501) staff       (20)        0 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/__init__.py
+drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari/models/
+-rw-r--r--   0 vraman     (501) staff       (20)     2505 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/models/request.py
+-rw-r--r--   0 vraman     (501) staff       (20)       64 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/models/__init__.py
+-rw-r--r--   0 vraman     (501) staff       (20)     3935 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/models/core.py
+-rw-r--r--   0 vraman     (501) staff       (20)     2273 2023-05-09 06:49:08.000000 syncari-sdk-1.3.7/syncari/models/schema.py
+-rw-r--r--   0 vraman     (501) staff       (20)      699 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/logger.py
+drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari/synapse/
+-rw-r--r--   0 vraman     (501) staff       (20)        0 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/synapse/__init__.py
+-rw-r--r--   0 vraman     (501) staff       (20)    10308 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/synapse/abstract_synapse.py
+drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari/rest/
+-rw-r--r--   0 vraman     (501) staff       (20)     3938 2023-05-09 18:36:03.000000 syncari-sdk-1.3.7/syncari/rest/client.py
+-rw-r--r--   0 vraman     (501) staff       (20)        0 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/rest/__init__.py
+drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/unit_tests/
+-rw-r--r--   0 vraman     (501) staff       (20)     7319 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/unit_tests/test_mock_synapse.py
+-rw-r--r--   0 vraman     (501) staff       (20)        0 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/unit_tests/__init__.py
+-rw-r--r--   0 vraman     (501) staff       (20)     6299 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/unit_tests/test_response_validations.py
+-rw-r--r--   0 vraman     (501) staff       (20)     2809 2023-05-09 18:36:58.000000 syncari-sdk-1.3.7/unit_tests/test_rest_client.py
+-rw-r--r--   0 vraman     (501) staff       (20)       78 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/README.md
+-rwxr-xr-x   0 vraman     (501) staff       (20)      562 2023-05-09 15:33:05.000000 syncari-sdk-1.3.7/setup.py
+drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari_sdk.egg-info/
+-rw-r--r--   0 vraman     (501) staff       (20)      373 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 vraman     (501) staff       (20)      569 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vraman     (501) staff       (20)       47 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari_sdk.egg-info/requires.txt
+-rw-r--r--   0 vraman     (501) staff       (20)       19 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari_sdk.egg-info/top_level.txt
+-rw-r--r--   0 vraman     (501) staff       (20)        1 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vraman     (501) staff       (20)       38 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `syncari-sdk-1.3.6/setup.py` & `syncari-sdk-1.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='syncari-sdk',
-    version='1.3.6',
+    version='1.3.7',
     description='Syncari Synapse Development Kit',
     author='Syncari',
     author_email='dev@syncari.com',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='TBD',
     packages=find_packages(exclude=('unittests')),
```

### Comparing `syncari-sdk-1.3.6/syncari/logger.py` & `syncari-sdk-1.3.7/syncari/logger.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.6/syncari/models/core.py` & `syncari-sdk-1.3.7/syncari/models/core.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.6/syncari/models/request.py` & `syncari-sdk-1.3.7/syncari/models/request.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.6/syncari/models/schema.py` & `syncari-sdk-1.3.7/syncari/models/schema.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.6/syncari/rest/client.py` & `syncari-sdk-1.3.7/syncari/rest/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,27 +21,29 @@
 class SyncariRestClient:
 
     success_responses=[200,201,202,204]
 
     """
         Default Syncari Rest Client
     """
-    def __init__(self, base_url, auth_config):
+    def __init__(self, base_url, auth_config, numRetries=5, backoff_factor=2):
         self.auth_config = auth_config
         self.rest_url = base_url
         self._session = requests.Session()
 
         retry_strategy = Retry(
-            total=3,
+            total=numRetries,
             status_forcelist=[429, 500, 502, 503, 504],
-            allowed_methods=["HEAD", "GET", "OPTIONS"]
+            backoff_factor=backoff_factor,
+            allowed_methods=["HEAD", "GET", "POST", "OPTIONS"],
+            raise_on_status=False
         )
-        adapter = HTTPAdapter(max_retries=retry_strategy)
+        #adapter = HTTPAdapter(max_retries=retry_strategy)
 
-        adapter = requests.adapters.HTTPAdapter(max_retries=3)
+        adapter = requests.adapters.HTTPAdapter(max_retries=retry_strategy)
         self._session.mount('https://', adapter)
 
     def get(self, path, **kwargs):
         """
             A default get request
         """
         return self.rest_request('GET', path, **kwargs)
@@ -81,18 +83,14 @@
             resp = self._session.send(req, stream=stream)
             logger.info("%s: HTTP %s %s",resp.status_code, method, url)
         except Exception as e:
             logger.error("Request to %s failed, payload %s error %s", url,
                          kwargs, e)
             raise SyncariException(error_response=ErrorResponse(message=err_msg, detail=str(e), status_code=500))
 
-        if resp.status_code == 500:
-            logger.error("Request to %s failed with status code %s, payload %s response %s",url, resp.status_code,kwargs, resp.text)
-            raise RetryableException(resp)
-
         if resp.status_code not in self.success_responses:
             logger.error("Request to %s failed with status code %s, payload %s response %s",url, resp.status_code,kwargs, resp.text)
             error_resp = ErrorResponse(message=err_msg, detail=self.__get_error_response_details(resp), status_code=resp.status_code)
             raise SyncariException(error_response=error_resp)
 
         return resp
```

### Comparing `syncari-sdk-1.3.6/syncari/synapse/abstract_synapse.py` & `syncari-sdk-1.3.7/syncari/synapse/abstract_synapse.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.6/syncari_sdk.egg-info/SOURCES.txt` & `syncari-sdk-1.3.7/syncari_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.6/unit_tests/test_mock_synapse.py` & `syncari-sdk-1.3.7/unit_tests/test_mock_synapse.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.6/unit_tests/test_response_validations.py` & `syncari-sdk-1.3.7/unit_tests/test_response_validations.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.6/unit_tests/test_rest_client.py` & `syncari-sdk-1.3.7/unit_tests/test_rest_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pylint: disable=missing-class-docstring, import-error, missing-function-docstring
 import pytest
 from pytest import fail
 from syncari.rest.client import SyncariException, SyncariRestClient
 from syncari.logger import SyncariLogger
+from requests.adapters import HTTPAdapter
 
 logger = SyncariLogger.get_logger('test_router')
 
 def test_get():
     rest_client = SyncariRestClient('http://universities.hipolabs.com/', None)
     resp = rest_client.get('search?country=United+States')
     assert resp.status_code == 200
@@ -38,7 +39,30 @@
         resp = rest_client.get('search?country=United+States')
     except SyncariException as e:
         assert e.error_response.status_code == 500
         assert e.error_response.message == 'Failed to execute GET on url:http://universities.hipolabs.comsearch?country=United+States'
     except Exception as e:
         fail('Invalid exception thrown from SyncariRestClient')
 
+
+def test_retry_strategy():
+    # missing / in the host.
+    rest_client = SyncariRestClient('https://httpstat.us', None, 2, 1)
+    adapter = rest_client._session.get_adapter("https://httpstat.us")
+    adapter.__class__ = HTTPAdapter
+    retryStrategy = adapter.max_retries
+    assert retryStrategy.total == 2
+    assert retryStrategy.backoff_factor == 1
+
+    try:
+        resp = rest_client.get('/500')
+    except SyncariException as e:
+        assert e.error_response.status_code == 500
+    except Exception as e:
+        fail('Invalid exception thrown from SyncariRestClient')
+
+    try:
+        resp = rest_client.get('/503')
+    except SyncariException as e:
+        assert e.error_response.status_code == 503
+    except Exception as e:
+        fail('Invalid exception thrown from SyncariRestClient')
```

