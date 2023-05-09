# Comparing `tmp/bnipython-0.6.3.tar.gz` & `tmp/bnipython-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ikowirya/Documents/BNI/APM/SDK/bni-python/dist/.tmp-z9ikt7mw/bnipython-0.6.3.tar", last modified: Tue Apr 18 07:41:55 2023, max compression
+gzip compressed data, was "/Users/ikowirya/Documents/BNI/APM/SDK/bni-python/dist/.tmp-jehf8h1b/bnipython-0.6.4.tar", last modified: Tue May  9 06:44:45 2023, max compression
```

## Comparing `bnipython-0.6.3.tar` & `bnipython-0.6.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.294249 bnipython-0.6.3/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1064 2022-09-12 08:55:19.000000 bnipython-0.6.3/LICENSE
--rw-r--r--   0 ikowirya   (501) staff       (20)    12395 2023-04-18 07:41:55.293815 bnipython-0.6.3/PKG-INFO
--rw-r--r--   0 ikowirya   (501) staff       (20)    11599 2023-04-18 07:38:12.000000 bnipython-0.6.3/README.md
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.279668 bnipython-0.6.3/bnipython/
--rw-r--r--   0 ikowirya   (501) staff       (20)      276 2023-04-14 08:10:12.000000 bnipython-0.6.3/bnipython/__init__.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.282934 bnipython-0.6.3/bnipython/lib/
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.284536 bnipython-0.6.3/bnipython/lib/api/
--rw-r--r--   0 ikowirya   (501) staff       (20)     9174 2023-04-18 07:21:08.000000 bnipython-0.6.3/bnipython/lib/api/oneGatePayment.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    25259 2023-04-14 08:10:12.000000 bnipython-0.6.3/bnipython/lib/api/snapBI.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     1140 2023-04-18 06:59:40.000000 bnipython-0.6.3/bnipython/lib/bniClient.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.286029 bnipython-0.6.3/bnipython/lib/net/
--rw-r--r--   0 ikowirya   (501) staff       (20)     3284 2023-04-18 06:59:48.000000 bnipython-0.6.3/bnipython/lib/net/httpClient.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.289053 bnipython-0.6.3/bnipython/lib/util/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1312 2023-04-18 04:24:59.000000 bnipython-0.6.3/bnipython/lib/util/constants.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     1255 2023-04-18 07:30:10.000000 bnipython-0.6.3/bnipython/lib/util/response.py
--rw-r--r--   0 ikowirya   (501) staff       (20)     2464 2023-04-18 06:59:40.000000 bnipython-0.6.3/bnipython/lib/util/utils.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.282046 bnipython-0.6.3/bnipython.egg-info/
--rw-r--r--   0 ikowirya   (501) staff       (20)    12395 2023-04-18 07:41:55.000000 bnipython-0.6.3/bnipython.egg-info/PKG-INFO
--rw-r--r--   0 ikowirya   (501) staff       (20)      523 2023-04-18 07:41:55.000000 bnipython-0.6.3/bnipython.egg-info/SOURCES.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)        1 2023-04-18 07:41:55.000000 bnipython-0.6.3/bnipython.egg-info/dependency_links.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       17 2023-04-18 07:41:55.000000 bnipython-0.6.3/bnipython.egg-info/requires.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       10 2023-04-18 07:41:55.000000 bnipython-0.6.3/bnipython.egg-info/top_level.txt
--rw-r--r--   0 ikowirya   (501) staff       (20)       38 2023-04-18 07:41:55.294651 bnipython-0.6.3/setup.cfg
--rw-r--r--   0 ikowirya   (501) staff       (20)     1297 2023-04-18 07:39:28.000000 bnipython-0.6.3/setup.py
-drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-04-18 07:41:55.293032 bnipython-0.6.3/tests/
--rw-r--r--   0 ikowirya   (501) staff       (20)     1937 2023-04-18 06:59:40.000000 bnipython-0.6.3/tests/test_bni_client.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    10315 2023-04-18 07:37:16.000000 bnipython-0.6.3/tests/test_one_gate_payment.py
--rw-r--r--   0 ikowirya   (501) staff       (20)    18061 2023-04-14 08:10:12.000000 bnipython-0.6.3/tests/test_snap_bi.py
--rw-r--r--   0 ikowirya   (501) staff       (20)      892 2023-04-14 08:10:12.000000 bnipython-0.6.3/tests/test_util.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.198294 bnipython-0.6.4/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1064 2022-09-12 08:55:19.000000 bnipython-0.6.4/LICENSE
+-rw-r--r--   0 ikowirya   (501) staff       (20)    12395 2023-05-09 06:44:45.196762 bnipython-0.6.4/PKG-INFO
+-rw-r--r--   0 ikowirya   (501) staff       (20)    11599 2023-04-18 07:38:12.000000 bnipython-0.6.4/README.md
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.157608 bnipython-0.6.4/bnipython/
+-rw-r--r--   0 ikowirya   (501) staff       (20)      276 2023-04-14 08:10:12.000000 bnipython-0.6.4/bnipython/__init__.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.170124 bnipython-0.6.4/bnipython/lib/
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.173490 bnipython-0.6.4/bnipython/lib/api/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     9174 2023-04-18 07:21:08.000000 bnipython-0.6.4/bnipython/lib/api/oneGatePayment.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    25259 2023-04-14 08:10:12.000000 bnipython-0.6.4/bnipython/lib/api/snapBI.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1140 2023-04-18 06:59:40.000000 bnipython-0.6.4/bnipython/lib/bniClient.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.176941 bnipython-0.6.4/bnipython/lib/net/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     3284 2023-05-05 03:23:06.000000 bnipython-0.6.4/bnipython/lib/net/httpClient.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.185860 bnipython-0.6.4/bnipython/lib/util/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1312 2023-04-18 04:24:59.000000 bnipython-0.6.4/bnipython/lib/util/constants.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1255 2023-04-18 07:30:10.000000 bnipython-0.6.4/bnipython/lib/util/response.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)     2448 2023-05-05 03:25:19.000000 bnipython-0.6.4/bnipython/lib/util/utils.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.168767 bnipython-0.6.4/bnipython.egg-info/
+-rw-r--r--   0 ikowirya   (501) staff       (20)    12395 2023-05-09 06:44:45.000000 bnipython-0.6.4/bnipython.egg-info/PKG-INFO
+-rw-r--r--   0 ikowirya   (501) staff       (20)      523 2023-05-09 06:44:45.000000 bnipython-0.6.4/bnipython.egg-info/SOURCES.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)        1 2023-05-09 06:44:45.000000 bnipython-0.6.4/bnipython.egg-info/dependency_links.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       17 2023-05-09 06:44:45.000000 bnipython-0.6.4/bnipython.egg-info/requires.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       10 2023-05-09 06:44:45.000000 bnipython-0.6.4/bnipython.egg-info/top_level.txt
+-rw-r--r--   0 ikowirya   (501) staff       (20)       38 2023-05-09 06:44:45.198708 bnipython-0.6.4/setup.cfg
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1297 2023-05-09 06:40:06.000000 bnipython-0.6.4/setup.py
+drwxr-xr-x   0 ikowirya   (501) staff       (20)        0 2023-05-09 06:44:45.193564 bnipython-0.6.4/tests/
+-rw-r--r--   0 ikowirya   (501) staff       (20)     1937 2023-04-18 06:59:40.000000 bnipython-0.6.4/tests/test_bni_client.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    10315 2023-04-18 07:37:16.000000 bnipython-0.6.4/tests/test_one_gate_payment.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)    18061 2023-05-05 03:44:48.000000 bnipython-0.6.4/tests/test_snap_bi.py
+-rw-r--r--   0 ikowirya   (501) staff       (20)      892 2023-04-14 08:10:12.000000 bnipython-0.6.4/tests/test_util.py
```

### Comparing `bnipython-0.6.3/LICENSE` & `bnipython-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.3/PKG-INFO` & `bnipython-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnipython
-Version: 0.6.3
+Version: 0.6.4
 Summary: Official  BNI API SDK for Python
 Home-page: https://github.com/bni-api/bni-python/
 Author: BNI API
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bnipython-0.6.3/README.md` & `bnipython-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.3/bnipython/lib/api/oneGatePayment.py` & `bnipython-0.6.4/bnipython/lib/api/oneGatePayment.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.3/bnipython/lib/api/snapBI.py` & `bnipython-0.6.4/bnipython/lib/api/snapBI.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.3/bnipython/lib/bniClient.py` & `bnipython-0.6.4/bnipython/lib/bniClient.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.3/bnipython/lib/net/httpClient.py` & `bnipython-0.6.4/bnipython/lib/net/httpClient.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.3/bnipython/lib/util/constants.py` & `bnipython-0.6.4/bnipython/lib/util/constants.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.3/bnipython/lib/util/response.py` & `bnipython-0.6.4/bnipython/lib/util/response.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.3/bnipython/lib/util/utils.py` & `bnipython-0.6.4/bnipython/lib/util/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 def getTimestamp():
     return datetime.now(pytz.timezone('Asia/Jakarta')).strftime('%Y-%m-%dT%H:%M:%S+07:00')
 
 
 def generateTokenSignature(params={'privateKeyPath', 'clientId', 'timeStamp'}):
     privateKeyPath = params['privateKeyPath']
     rsaPrivate = privateKeyPath.replace('./', '')
-    keyFile = open(f'./bnipython/lib/{rsaPrivate}', 'rb')
+    keyFile = open(f'{rsaPrivate}', 'rb')
     key = keyFile.read()
     keyFile.close()
 
     pkey = crypto.load_privatekey(crypto.FILETYPE_PEM, key)
     clienId = params['clientId']
     times = params['timeStamp']
     data = f"{clienId}|{times}"
```

### Comparing `bnipython-0.6.3/bnipython.egg-info/PKG-INFO` & `bnipython-0.6.4/bnipython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnipython
-Version: 0.6.3
+Version: 0.6.4
 Summary: Official  BNI API SDK for Python
 Home-page: https://github.com/bni-api/bni-python/
 Author: BNI API
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bnipython-0.6.3/bnipython.egg-info/SOURCES.txt` & `bnipython-0.6.4/bnipython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.3/setup.py` & `bnipython-0.6.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 test_req = pkg_req + [
     'pytest>=3.0.6'
 ]
 
 setup(
     name="bnipython",
-    version="0.6.3",
+    version="0.6.4",
     author="BNI API",
     author_email="",
     license='MIT',
     description="Official  BNI API SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bni-api/bni-python/",
```

### Comparing `bnipython-0.6.3/tests/test_bni_client.py` & `bnipython-0.6.4/tests/test_bni_client.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.3/tests/test_one_gate_payment.py` & `bnipython-0.6.4/tests/test_one_gate_payment.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.3/tests/test_snap_bi.py` & `bnipython-0.6.4/tests/test_snap_bi.py`

 * *Files identical despite different names*

### Comparing `bnipython-0.6.3/tests/test_util.py` & `bnipython-0.6.4/tests/test_util.py`

 * *Files identical despite different names*

