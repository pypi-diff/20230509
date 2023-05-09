# Comparing `tmp/vijay-access_control-0.1.tar.gz` & `tmp/vijay-access_control-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vijay-access_control-0.1.tar", last modified: Tue May  9 05:41:49 2023, max compression
+gzip compressed data, was "vijay-access_control-0.2.tar", last modified: Tue May  9 06:41:43 2023, max compression
```

## Comparing `vijay-access_control-0.1.tar` & `vijay-access_control-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-09 05:41:49.678887 vijay-access_control-0.1/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       97 2023-05-09 05:41:49.678887 vijay-access_control-0.1/PKG-INFO
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-09 05:41:49.678887 vijay-access_control-0.1/access_control/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      106 2023-05-09 04:57:25.000000 vijay-access_control-0.1/access_control/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1210 2023-05-09 04:27:09.000000 vijay-access_control-0.1/access_control/s3_access_control_plugin.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-09 05:41:49.678887 vijay-access_control-0.1/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      195 2023-05-09 05:41:42.000000 vijay-access_control-0.1/setup.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-09 05:41:49.678887 vijay-access_control-0.1/vijay_access_control.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       97 2023-05-09 05:41:49.000000 vijay-access_control-0.1/vijay_access_control.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      254 2023-05-09 05:41:49.000000 vijay-access_control-0.1/vijay_access_control.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-09 05:41:49.000000 vijay-access_control-0.1/vijay_access_control.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       15 2023-05-09 05:41:49.000000 vijay-access_control-0.1/vijay_access_control.egg-info/top_level.txt
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-09 06:41:43.951716 vijay-access_control-0.2/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       97 2023-05-09 06:41:43.951716 vijay-access_control-0.2/PKG-INFO
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-09 06:41:43.951716 vijay-access_control-0.2/access_control/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      106 2023-05-09 04:57:25.000000 vijay-access_control-0.2/access_control/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1249 2023-05-09 06:39:44.000000 vijay-access_control-0.2/access_control/s3_access_control_plugin.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-09 06:41:43.951716 vijay-access_control-0.2/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      195 2023-05-09 06:41:39.000000 vijay-access_control-0.2/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-09 06:41:43.951716 vijay-access_control-0.2/vijay_access_control.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       97 2023-05-09 06:41:43.000000 vijay-access_control-0.2/vijay_access_control.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      254 2023-05-09 06:41:43.000000 vijay-access_control-0.2/vijay_access_control.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-09 06:41:43.000000 vijay-access_control-0.2/vijay_access_control.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       15 2023-05-09 06:41:43.000000 vijay-access_control-0.2/vijay_access_control.egg-info/top_level.txt
```

### Comparing `vijay-access_control-0.1/access_control/s3_access_control_plugin.py` & `vijay-access_control-0.2/access_control/s3_access_control_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import boto3
 import os
 
 class s3_wrapper:
-    def __init__(self):
+    def __init__(self, bucket):
         self.s3 = boto3.client('s3')
         self.s3_resource = boto3.resource('s3')
-        self.bucket_name ='vijaysagemakerbucket'
-    
+       # self.bucket_name ='vijaysagemakerbucket'
+        self.bucket_name = bucket
+
     def get_object(self, key):
         obj = self.s3.get_object(Bucket=self.bucket_name, Key=key)
         return obj['Body'].read().decode('utf-8')
 
     def put_object(self, key, body):
         self.s3.put_object(Bucket=self.bucket_name, Key=key, Body=body)
```

