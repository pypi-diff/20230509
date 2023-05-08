# Comparing `tmp/s3dbm-0.0.5.tar.gz` & `tmp/s3dbm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3dbm-0.0.5.tar", last modified: Mon May  8 08:23:55 2023, max compression
+gzip compressed data, was "s3dbm-0.0.6.tar", last modified: Mon May  8 22:11:05 2023, max compression
```

## Comparing `s3dbm-0.0.5.tar` & `s3dbm-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 08:23:55.567186 s3dbm-0.0.5/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-05 20:34:52.000000 s3dbm-0.0.5/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 08:23:55.567186 s3dbm-0.0.5/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-05-07 22:33:06.000000 s3dbm-0.0.5/README.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-06 23:57:50.000000 s3dbm-0.0.5/pyproject.toml
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 08:23:55.567186 s3dbm-0.0.5/s3dbm/
--rw-rw-r--   0 mike      (1000) mike      (1000)      111 2023-05-08 01:40:14.000000 s3dbm-0.0.5/s3dbm/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    12767 2023-05-08 01:40:08.000000 s3dbm-0.0.5/s3dbm/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 08:23:55.567186 s3dbm-0.0.5/s3dbm/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-06 23:57:50.000000 s3dbm-0.0.5/s3dbm/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    13755 2023-05-08 08:23:10.000000 s3dbm-0.0.5/s3dbm/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 08:23:55.567186 s3dbm-0.0.5/s3dbm.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 08:23:55.000000 s3dbm-0.0.5/s3dbm.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      267 2023-05-08 08:23:55.000000 s3dbm-0.0.5/s3dbm.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-08 08:23:55.000000 s3dbm-0.0.5/s3dbm.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       36 2023-05-08 08:23:55.000000 s3dbm-0.0.5/s3dbm.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-05-08 08:23:55.000000 s3dbm-0.0.5/s3dbm.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-08 08:23:55.567186 s3dbm-0.0.5/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7162 2023-05-08 08:23:36.000000 s3dbm-0.0.5/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:11:05.876578 s3dbm-0.0.6/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-05 20:34:52.000000 s3dbm-0.0.6/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 22:11:05.876578 s3dbm-0.0.6/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-05-07 22:33:06.000000 s3dbm-0.0.6/README.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-06 23:57:50.000000 s3dbm-0.0.6/pyproject.toml
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:11:05.876578 s3dbm-0.0.6/s3dbm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      111 2023-05-08 01:40:14.000000 s3dbm-0.0.6/s3dbm/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    12766 2023-05-08 21:20:08.000000 s3dbm-0.0.6/s3dbm/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:11:05.876578 s3dbm-0.0.6/s3dbm/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-06 23:57:50.000000 s3dbm-0.0.6/s3dbm/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    13755 2023-05-08 22:04:58.000000 s3dbm-0.0.6/s3dbm/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:11:05.876578 s3dbm-0.0.6/s3dbm.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      591 2023-05-08 22:11:05.000000 s3dbm-0.0.6/s3dbm.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      267 2023-05-08 22:11:05.000000 s3dbm-0.0.6/s3dbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-08 22:11:05.000000 s3dbm-0.0.6/s3dbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       36 2023-05-08 22:11:05.000000 s3dbm-0.0.6/s3dbm.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-05-08 22:11:05.000000 s3dbm-0.0.6/s3dbm.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-08 22:11:05.876578 s3dbm-0.0.6/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7162 2023-05-08 22:10:31.000000 s3dbm-0.0.6/setup.py
```

### Comparing `s3dbm-0.0.5/LICENSE` & `s3dbm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `s3dbm-0.0.5/PKG-INFO` & `s3dbm-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3dbm
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python dbm-style interface to S3
 Home-page: https://github.com/mullenkamp/s3dbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3dbm-0.0.5/s3dbm/main.py` & `s3dbm-0.0.6/s3dbm/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 
 class S3DBM(MutableMapping):
     """
 
     """
-    def __init__(self, bucket: str, client: botocore.client.BaseClient=None, connection_config: utils.ConnectionConfig=None, public_url: HttpUrl=None, flag: str = "r", buffer_size: int=524288, retries: int=3, read_timeout: int=120, provider: str=None, threads: int=30, compression=True, cache: MutableMapping=None):
+    def __init__(self, bucket: str, client: botocore.client.BaseClient=None, connection_config: utils.ConnectionConfig=None, public_url: HttpUrl=None, flag: str = "r", buffer_size: int=512000, retries: int=3, read_timeout: int=120, provider: str=None, threads: int=30, compression=True, cache: MutableMapping=None):
         """
 
         """
         if client is not None:
             pass
         elif connection_config is not None:
             client = utils.s3_client(connection_config, threads, retries, read_timeout=read_timeout)
@@ -254,15 +254,15 @@
         if self._write:
             self._executor.shutdown()
             del self._executor
             self._executor = concurrent.futures.ThreadPoolExecutor(max_workers=self._threads)
 
 
 def open(
-    bucket: str, client: botocore.client.BaseClient=None, connection_config: utils.ConnectionConfig=None, public_url: HttpUrl=None, flag: str = "r", buffer_size: int=524288, retries: int=3, read_timeout: int=120, provider: str=None, threads: int=30, compression: bool=True, cache: MutableMapping=None):
+    bucket: str, client: botocore.client.BaseClient=None, connection_config: utils.ConnectionConfig=None, public_url: HttpUrl=None, flag: str = "r", buffer_size: int=512000, retries: int=3, read_timeout: int=120, provider: str=None, threads: int=30, compression: bool=True, cache: MutableMapping=None):
     """
     Open an S3 dbm-style database. This allows the user to interact with an S3 bucket like a MutableMapping (python dict) object. Lots of options including read caching.
 
     Parameters
     -----------
     bucket : str
         The S3 bucket with the objects.
@@ -276,15 +276,15 @@
     public_url : HttpUrl or None
         If the S3 bucket is publicly accessible, then supplying the public_url will download objects via normal http. The provider parameter is associated with public_url to specify the provider's public url style.
 
     flag : str
         Flag associated with how the file is opened according to the dbm style. See below for details.
 
     buffer_size : int
-        The buffer memory size used for reading and writing. Defaults to 524288.
+        The buffer memory size used for reading and writing. Defaults to 512000.
 
     retries : int
         The number of http retries for reads and writes. Defaults to 3.
 
     read_timeout : int
         The http read timeout in seconds. Defaults to 120.
 
@@ -319,9 +319,8 @@
     |         | creating it if it doesn't exist           |
     +---------+-------------------------------------------+
     | ``'n'`` | Always create a new, empty database, open |
     |         | for reading and writing                   |
     +---------+-------------------------------------------+
 
     """
-
     return S3DBM(bucket, client, connection_config, public_url, flag, buffer_size, retries, read_timeout, provider, threads, compression, cache)
```

### Comparing `s3dbm-0.0.5/s3dbm/utils.py` & `s3dbm-0.0.6/s3dbm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,41 +126,41 @@
     else:
         s3_config.update({'config': botocore.config.Config(max_pool_connections=max_pool_connections, retries={'mode': retry_mode, 'max_attempts': max_attempts}, read_timeout=read_timeout)})
         s3 = boto3.client(**s3_config)
 
     return s3
 
 
-def zstd_stream_reader(stream, buffer_size: int=524288):
+def zstd_stream_reader(stream, buffer_size: int=512000):
     """
 
     """
     if hasattr(stream, '_buffer_size'):
         buffer_size = stream._buffer_size
     dctx = zstd.ZstdDecompressor()
     reader = dctx.stream_reader(stream, read_size=buffer_size)
     # reader._buffer_size = buffer_size
 
     return reader
 
 
-def zstd_stream_writer(stream, buffer_size: int=524288):
+def zstd_stream_writer(stream, buffer_size: int=512000):
     """
 
     """
     if hasattr(stream, '_buffer_size'):
         buffer_size = stream._buffer_size
     dctx = zstd.ZstdCompressor(1)
     writer = dctx.stream_writer(stream, write_size=buffer_size)
     writer._buffer_size = buffer_size
 
     return writer
 
 
-def url_to_stream(url: HttpUrl, buffer_size: int=524288, read_timeout: int=120):
+def url_to_stream(url: HttpUrl, buffer_size: int=512000, read_timeout: int=120):
     """
     Function to create a file object from a file stored via http(s). This function will return a file object of the object in the url location. This file object does not contain any data until data is read from it, which ensures large files are not completely read into memory.
 
     Parameters
     ----------
     url: http str
         The http url to the file.
@@ -184,15 +184,15 @@
         file_obj._buffer_size = buffer_size
     except Exception as err:
         file_obj = None
 
     return file_obj
 
 
-def get_object_s3(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, public_url: HttpUrl=None, buffer_size: int=524288, read_timeout: int=120, provider: str=None):
+def get_object_s3(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, public_url: HttpUrl=None, buffer_size: int=512000, read_timeout: int=120, provider: str=None):
     """
     General function to get an object from an S3 bucket. One of s3, connection_config, or public_url must be used. This function will return a file object of the object in the S3 (or url) location. This file object does not contain any data until data is read from it, which ensures large files are not completely read into memory.
 
     Parameters
     ----------
     obj_key : str
         The object key in the S3 bucket.
@@ -236,15 +236,15 @@
 
     else:
         raise TypeError('One of client or public_url needs to be correctly defined.')
 
     return file_obj
 
 
-def get_object_final(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, public_url: HttpUrl=None, buffer_size: int=524288, read_timeout: int=120, provider: str=None, compression: bool=True, cache: MutableMapping=None):
+def get_object_final(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, public_url: HttpUrl=None, buffer_size: int=512000, read_timeout: int=120, provider: str=None, compression: bool=True, cache: MutableMapping=None):
     """
 
     """
     if cache is not None:
         if hasattr(cache, '_buffer_size'):
             buffer_size = cache._buffer_size
         try:
@@ -261,15 +261,15 @@
         if compression:
             if obj_key.endswith('.zstd') or obj_key.endswith('.zst'):
                 file_obj = zstd_stream_reader(file_obj, buffer_size)
 
     return file_obj
 
 
-def put_object_s3(s3: botocore.client.BaseClient, bucket: str, obj_key: str, file_obj: io.BufferedIOBase, buffer_size: int=524288, compression=True):
+def put_object_s3(s3: botocore.client.BaseClient, bucket: str, obj_key: str, file_obj: io.BufferedIOBase, buffer_size: int=512000, compression=True):
     """
     Function to upload data to an S3 bucket. This function will iteratively write the input file_obj in chunks ensuring that little memory is needed writing the object.
 
     Parameters
     ----------
     s3 : boto3.client
         A boto3 client object
```

### Comparing `s3dbm-0.0.5/s3dbm.egg-info/PKG-INFO` & `s3dbm-0.0.6/s3dbm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3dbm
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python dbm-style interface to S3
 Home-page: https://github.com/mullenkamp/s3dbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3dbm-0.0.5/setup.py` & `s3dbm-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 's3dbm'
 main_package = 's3dbm'
-version = '0.0.5'
+version = '0.0.6'
 descrip = 'A python dbm-style interface to S3'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

