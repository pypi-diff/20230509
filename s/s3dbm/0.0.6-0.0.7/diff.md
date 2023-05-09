# Comparing `tmp/s3dbm-0.0.6.tar.gz` & `tmp/s3dbm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3dbm-0.0.6.tar", last modified: Mon May  8 22:11:05 2023, max compression
+gzip compressed data, was "s3dbm-0.0.7.tar", last modified: Tue May  9 09:04:44 2023, max compression
```

## Comparing `s3dbm-0.0.6.tar` & `s3dbm-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:11:05.876578 s3dbm-0.0.6/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-05 20:34:52.000000 s3dbm-0.0.6/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 22:11:05.876578 s3dbm-0.0.6/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-05-07 22:33:06.000000 s3dbm-0.0.6/README.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-06 23:57:50.000000 s3dbm-0.0.6/pyproject.toml
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:11:05.876578 s3dbm-0.0.6/s3dbm/
--rw-rw-r--   0 mike      (1000) mike      (1000)      111 2023-05-08 01:40:14.000000 s3dbm-0.0.6/s3dbm/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    12766 2023-05-08 21:20:08.000000 s3dbm-0.0.6/s3dbm/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:11:05.876578 s3dbm-0.0.6/s3dbm/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-06 23:57:50.000000 s3dbm-0.0.6/s3dbm/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    13755 2023-05-08 22:04:58.000000 s3dbm-0.0.6/s3dbm/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:11:05.876578 s3dbm-0.0.6/s3dbm.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 22:11:05.000000 s3dbm-0.0.6/s3dbm.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      267 2023-05-08 22:11:05.000000 s3dbm-0.0.6/s3dbm.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-08 22:11:05.000000 s3dbm-0.0.6/s3dbm.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       36 2023-05-08 22:11:05.000000 s3dbm-0.0.6/s3dbm.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-05-08 22:11:05.000000 s3dbm-0.0.6/s3dbm.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-08 22:11:05.876578 s3dbm-0.0.6/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7162 2023-05-08 22:10:31.000000 s3dbm-0.0.6/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-09 09:04:44.275023 s3dbm-0.0.7/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-05 20:34:52.000000 s3dbm-0.0.7/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-09 09:04:44.275023 s3dbm-0.0.7/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-05-07 22:33:06.000000 s3dbm-0.0.7/README.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-06 23:57:50.000000 s3dbm-0.0.7/pyproject.toml
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-09 09:04:44.275023 s3dbm-0.0.7/s3dbm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      111 2023-05-08 01:40:14.000000 s3dbm-0.0.7/s3dbm/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    12695 2023-05-09 09:03:06.000000 s3dbm-0.0.7/s3dbm/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-09 09:04:44.275023 s3dbm-0.0.7/s3dbm/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-06 23:57:50.000000 s3dbm-0.0.7/s3dbm/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    13937 2023-05-09 09:03:17.000000 s3dbm-0.0.7/s3dbm/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-09 09:04:44.275023 s3dbm-0.0.7/s3dbm.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-09 09:04:44.000000 s3dbm-0.0.7/s3dbm.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      267 2023-05-09 09:04:44.000000 s3dbm-0.0.7/s3dbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-09 09:04:44.000000 s3dbm-0.0.7/s3dbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       36 2023-05-09 09:04:44.000000 s3dbm-0.0.7/s3dbm.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-05-09 09:04:44.000000 s3dbm-0.0.7/s3dbm.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-09 09:04:44.275023 s3dbm-0.0.7/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7162 2023-05-09 09:04:31.000000 s3dbm-0.0.7/setup.py
```

### Comparing `s3dbm-0.0.6/LICENSE` & `s3dbm-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `s3dbm-0.0.6/PKG-INFO` & `s3dbm-0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3dbm
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python dbm-style interface to S3
 Home-page: https://github.com/mullenkamp/s3dbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3dbm-0.0.6/s3dbm/main.py` & `s3dbm-0.0.7/s3dbm/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,25 +57,25 @@
         self._threads = threads
         self._cache = cache
 
         self._executor = concurrent.futures.ThreadPoolExecutor(max_workers=threads)
 
 
     def keys(self, prefix: str='', start_after: str='', delimiter: str=''):
-        continuation_token = ''
+        params = utils.build_params(self._bucket, start_after=start_after, prefix=prefix)
 
         while True:
-            js1 = self._client.list_objects_v2(Bucket=self._bucket, Prefix=prefix, StartAfter=start_after, Delimiter=delimiter, ContinuationToken=continuation_token)
+            js1 = self._client.list_objects_v2(**params)
 
             if 'Contents' in js1:
                 for k in js1['Contents']:
                     yield k['Key']
 
                 if 'NextContinuationToken' in js1:
-                    continuation_token = js1['NextContinuationToken']
+                    params['ContinuationToken'] = js1['NextContinuationToken']
                 else:
                     break
             else:
                 break
 
 
     def items(self, keys: List[str]=None, prefix: str='', start_after: str='', delimiter: str=''):
@@ -108,25 +108,26 @@
     def __iter__(self):
         return self.keys()
 
     def __len__(self):
         """
         There really should be a better way for this...
         """
-        continuation_token = ''
+        params = {'Bucket': self._bucket}
+
         count = 0
 
         while True:
-            js1 = self._client.list_objects_v2(Bucket=self._bucket, ContinuationToken=continuation_token)
+            js1 = self._client.list_objects_v2(**params)
 
             if 'Contents' in js1:
                 count += len(js1['Contents'])
 
                 if 'NextContinuationToken' in js1:
-                    continuation_token = js1['NextContinuationToken']
+                    params['ContinuationToken'] = js1['NextContinuationToken']
                 else:
                     break
             else:
                 break
 
         return count
```

### Comparing `s3dbm-0.0.6/s3dbm/utils.py` & `s3dbm-0.0.7/s3dbm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from collections.abc import Mapping, MutableMapping
 
 ############################################
 ### Parameters
 
 public_key_patterns = {'b2': '{base_url}/{bucket}/{obj_key}',
                        'contabo': '{base_url}:{bucket}/{obj_key}',
-                       'r2': '{bucket}.{base_url}/{obj_key}',
+                       'r2': 'https://{bucket}.{base_url}/{obj_key}',
                        }
 
 s3_url_base = 's3://{bucket}/{key}'
 
 multipart_size = 2**24
 
 ############################################
@@ -73,14 +73,18 @@
 
 def create_public_s3_url(base_url, bucket, obj_key, provider: str=None):
     """
     This should be updated as more S3 providers are added!
     """
     if provider is not None:
         if provider in public_key_patterns:
+            if provider == 'r2':
+                if '://' in base_url:
+                    base_url = base_url.split('://')[1]
+
             key = public_key_patterns[provider].format(base_url=base_url.rstrip('/'), bucket=bucket, obj_key=obj_key)
         else:
             raise ValueError(provider + ' not available')
     elif 'contabo' in base_url:
         key = public_key_patterns['contabo'].format(base_url=base_url.rstrip('/'), bucket=bucket, obj_key=obj_key)
     else:
         key = public_key_patterns['b2'].format(base_url=base_url.rstrip('/'), bucket=bucket, obj_key=obj_key)
@@ -313,15 +317,15 @@
         else:
             chunk = file_obj.read(buffer_size)
             while chunk:
                 f.write(chunk)
                 chunk = file_obj.read(buffer_size)
 
 
-def list_objects_s3(s3: botocore.client.BaseClient, bucket: str, prefix: str=None, start_after: str=None, delimiter: str=None, max_keys: int=None, continuation_token: str=''):
+def list_objects_s3(s3: botocore.client.BaseClient, bucket: str, prefix: str=None, start_after: str=None, delimiter: str=None, max_keys: int=None, continuation_token: str=None):
     """
     Wrapper S3 function around the list_objects_v2 base function with a Pandas DataFrame output.
 
     Parameters
     ----------
     s3 : boto3.client
         A boto3 client object
@@ -339,15 +343,17 @@
         If the object key has a date in it, pass a date format string to parse and add a column called KeyDate.
 
     Returns
     -------
     DataFrame
     """
     params = build_params(bucket, start_after=start_after, prefix=prefix, delimiter=delimiter, max_keys=max_keys)
-    params['ContinuationToken'] = continuation_token
+
+    if continuation_token is not None:
+        params['ContinuationToken'] = continuation_token
 
     js = []
     while True:
         js1 = s3.list_objects_v2(**params)
 
         if 'Contents' in js1:
             js.extend(js1['Contents'])
```

### Comparing `s3dbm-0.0.6/s3dbm.egg-info/PKG-INFO` & `s3dbm-0.0.7/s3dbm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3dbm
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python dbm-style interface to S3
 Home-page: https://github.com/mullenkamp/s3dbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3dbm-0.0.6/setup.py` & `s3dbm-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 's3dbm'
 main_package = 's3dbm'
-version = '0.0.6'
+version = '0.0.7'
 descrip = 'A python dbm-style interface to S3'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

