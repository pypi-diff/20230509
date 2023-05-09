# Comparing `tmp/TremendousClient-0.0.5.tar.gz` & `tmp/TremendousClient-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TremendousClient-0.0.5.tar", last modified: Wed Apr 26 20:23:23 2023, max compression
+gzip compressed data, was "TremendousClient-0.0.6.tar", last modified: Tue May  9 14:39:26 2023, max compression
```

## Comparing `TremendousClient-0.0.5.tar` & `TremendousClient-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 20:23:23.584374 TremendousClient-0.0.5/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 TremendousClient-0.0.5/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2548 2023-04-26 20:23:23.584232 TremendousClient-0.0.5/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2022 2023-04-26 20:23:13.000000 TremendousClient-0.0.5/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 20:23:23.582347 TremendousClient-0.0.5/TremendousClient.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2548 2023-04-26 20:23:23.000000 TremendousClient-0.0.5/TremendousClient.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      404 2023-04-26 20:23:23.000000 TremendousClient-0.0.5/TremendousClient.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-04-26 20:23:23.000000 TremendousClient-0.0.5/TremendousClient.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-04-26 20:23:23.000000 TremendousClient-0.0.5/TremendousClient.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       11 2023-04-26 20:23:23.000000 TremendousClient-0.0.5/TremendousClient.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-04-26 20:23:23.584416 TremendousClient-0.0.5/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      888 2023-04-26 20:17:58.000000 TremendousClient-0.0.5/setup.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 20:23:23.583136 TremendousClient-0.0.5/tremendous/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      161 2023-04-26 20:18:04.000000 TremendousClient-0.0.5/tremendous/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      337 2023-04-26 20:05:55.000000 TremendousClient-0.0.5/tremendous/exception.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2022-05-12 10:14:01.000000 TremendousClient-0.0.5/tremendous/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 20:23:23.583921 TremendousClient-0.0.5/tremendous/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       50 2023-04-26 18:53:09.000000 TremendousClient-0.0.5/tremendous/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1136 2023-04-26 19:58:25.000000 TremendousClient-0.0.5/tremendous/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1683 2023-04-26 20:17:52.000000 TremendousClient-0.0.5/tremendous/service/tremendous_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-05-09 14:39:26.517658 TremendousClient-0.0.6/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 TremendousClient-0.0.6/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2548 2023-05-09 14:39:26.517443 TremendousClient-0.0.6/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2022 2023-04-26 20:23:13.000000 TremendousClient-0.0.6/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-05-09 14:39:26.515378 TremendousClient-0.0.6/TremendousClient.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2548 2023-05-09 14:39:26.000000 TremendousClient-0.0.6/TremendousClient.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      404 2023-05-09 14:39:26.000000 TremendousClient-0.0.6/TremendousClient.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-05-09 14:39:26.000000 TremendousClient-0.0.6/TremendousClient.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-05-09 14:39:26.000000 TremendousClient-0.0.6/TremendousClient.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       11 2023-05-09 14:39:26.000000 TremendousClient-0.0.6/TremendousClient.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-05-09 14:39:26.517713 TremendousClient-0.0.6/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      888 2023-05-09 14:38:58.000000 TremendousClient-0.0.6/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-05-09 14:39:26.516080 TremendousClient-0.0.6/tremendous/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      161 2023-05-09 14:39:04.000000 TremendousClient-0.0.6/tremendous/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      337 2023-04-26 20:05:55.000000 TremendousClient-0.0.6/tremendous/exception.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2022-05-12 10:14:01.000000 TremendousClient-0.0.6/tremendous/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-05-09 14:39:26.517021 TremendousClient-0.0.6/tremendous/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       50 2023-04-26 18:53:09.000000 TremendousClient-0.0.6/tremendous/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1136 2023-04-26 19:58:25.000000 TremendousClient-0.0.6/tremendous/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1981 2023-05-09 14:38:58.000000 TremendousClient-0.0.6/tremendous/service/tremendous_service.py
```

### Comparing `TremendousClient-0.0.5/LICENSE` & `TremendousClient-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `TremendousClient-0.0.5/PKG-INFO` & `TremendousClient-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TremendousClient
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tremendous Api Client Python package
 Home-page: https://github.com/blueromans/Tremendous.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/Tremendous/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TremendousClient-0.0.5/README.md` & `TremendousClient-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `TremendousClient-0.0.5/TremendousClient.egg-info/PKG-INFO` & `TremendousClient-0.0.6/TremendousClient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TremendousClient
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tremendous Api Client Python package
 Home-page: https://github.com/blueromans/Tremendous.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/Tremendous/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TremendousClient-0.0.5/setup.py` & `TremendousClient-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='TremendousClient',
-    version="0.0.5",
+    version="0.0.6",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='Tremendous Api Client Python package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/Tremendous.git',
     project_urls={
```

### Comparing `TremendousClient-0.0.5/tremendous/service/http_service.py` & `TremendousClient-0.0.6/tremendous/service/http_service.py`

 * *Files identical despite different names*

### Comparing `TremendousClient-0.0.5/tremendous/service/tremendous_service.py` & `TremendousClient-0.0.6/tremendous/service/tremendous_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,21 @@
 
     def getFundingSource(self):
         return self.getRequest('funding_sources')
 
     def getProducts(self):
         return self.getRequest('products')
 
+    def getProduct(self, product_id):
+        endpoint = f'/api/v2/products/{product_id}'
+        response = self.connect('GET', endpoint, headers=self.headers)
+        if 'product' not in response:
+            raise AttributeError(ErrorCodes.INVALID_ATTRIBUTE)
+        return response['product']
+
     def createOrder(self, body):
         key = 'order'
         endpoint = '/api/v2/orders'
         response = self.connect('POST', endpoint, body, headers=self.headers)
         if key not in response:
             raise AttributeError(ErrorCodes.INVALID_ATTRIBUTE)
         return response[key]
```

