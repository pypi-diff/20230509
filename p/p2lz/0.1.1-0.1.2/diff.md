# Comparing `tmp/p2lz-0.1.1.tar.gz` & `tmp/p2lz-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2lz-0.1.1.tar", last modified: Mon May  8 16:30:59 2023, max compression
+gzip compressed data, was "p2lz-0.1.2.tar", last modified: Tue May  9 01:33:13 2023, max compression
```

## Comparing `p2lz-0.1.1.tar` & `p2lz-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:59.643376 p2lz-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:59.643376 p2lz-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:59.643376 p2lz-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-08 16:30:46.000000 p2lz-0.1.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 16:30:46.000000 p2lz-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 16:30:46.000000 p2lz-0.1.1/.tool-versions
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-08 16:30:46.000000 p2lz-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-08 16:30:46.000000 p2lz-0.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-08 16:30:59.643376 p2lz-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-08 16:30:46.000000 p2lz-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-08 16:30:46.000000 p2lz-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:30:59.643376 p2lz-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:59.643376 p2lz-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:59.643376 p2lz-0.1.1/src/p2lz/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 16:30:59.000000 p2lz-0.1.1/src/p2lz/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-08 16:30:46.000000 p2lz-0.1.1/src/p2lz/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-08 16:30:46.000000 p2lz-0.1.1/src/p2lz/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 16:30:46.000000 p2lz-0.1.1/src/p2lz/tools_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:59.643376 p2lz-0.1.1/src/p2lz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-08 16:30:59.000000 p2lz-0.1.1/src/p2lz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-08 16:30:59.000000 p2lz-0.1.1/src/p2lz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:30:59.000000 p2lz-0.1.1/src/p2lz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 16:30:59.000000 p2lz-0.1.1/src/p2lz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 16:30:59.000000 p2lz-0.1.1/src/p2lz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:33:13.016212 p2lz-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:33:13.012212 p2lz-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:33:13.012212 p2lz-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-09 01:32:57.000000 p2lz-0.1.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-09 01:32:57.000000 p2lz-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 01:32:57.000000 p2lz-0.1.2/.tool-versions
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-09 01:32:57.000000 p2lz-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-09 01:32:57.000000 p2lz-0.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-09 01:33:13.012212 p2lz-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 01:32:57.000000 p2lz-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-09 01:32:57.000000 p2lz-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 01:33:13.016212 p2lz-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:33:13.012212 p2lz-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:33:13.012212 p2lz-0.1.2/src/p2lz/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 01:33:12.000000 p2lz-0.1.2/src/p2lz/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-09 01:32:57.000000 p2lz-0.1.2/src/p2lz/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-09 01:32:57.000000 p2lz-0.1.2/src/p2lz/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-09 01:32:57.000000 p2lz-0.1.2/src/p2lz/tools_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:33:13.012212 p2lz-0.1.2/src/p2lz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-09 01:33:12.000000 p2lz-0.1.2/src/p2lz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-09 01:33:13.000000 p2lz-0.1.2/src/p2lz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 01:33:12.000000 p2lz-0.1.2/src/p2lz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 01:33:12.000000 p2lz-0.1.2/src/p2lz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 01:33:12.000000 p2lz-0.1.2/src/p2lz.egg-info/top_level.txt
```

### Comparing `p2lz-0.1.1/.github/workflows/publish.yaml` & `p2lz-0.1.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `p2lz-0.1.1/LICENSE.txt` & `p2lz-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `p2lz-0.1.1/src/p2lz/dynamodb.py` & `p2lz-0.1.2/src/p2lz/dynamodb.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import boto3
 
 
 class DynamoDB():
-    def __init__(self, table_name: str, dynamodb: boto3.resource('dynamodb')):
-        self.dynamodb = boto3.resource('dynamodb')
-        self.table = dynamodb.Table(table_name)
+    def __init__(self, table_name: str, dynamodb: boto3.resource = boto3.resource('dynamodb', region_name='ap-northeast-1')) -> None:
+        self.dynamodb = dynamodb
+        self.table = self.dynamodb.Table(table_name)
 
     @classmethod
     def table(cls, table_name: str):
-        dynamodb = boto3.resource('dynamodb')
-        return cls(table_name, dynamodb)
+        return cls(table_name)
 
     def query(self, **kwargs):
         while True:
             response = self.table.query(**kwargs)
             if 'Items' in response:
                 for item in response['Items']:
                     yield item
@@ -37,7 +36,10 @@
 
     def put_item(self, **kwargs):
         return self.table.put_item(**kwargs)
 
     def get_item(self, **kwargs):
         resp = self.table.get_item(**kwargs)
         return resp['Item']
+
+    def delete_item(self, **kwargs):
+        return self.table.delete_item(**kwargs)
```

### Comparing `p2lz-0.1.1/src/p2lz/tools.py` & `p2lz-0.1.2/src/p2lz/tools.py`

 * *Files identical despite different names*

