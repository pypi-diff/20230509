# Comparing `tmp/jy_utils-0.0.3.tar.gz` & `tmp/jy_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jy_utils-0.0.3.tar", last modified: Tue May  9 08:01:58 2023, max compression
+gzip compressed data, was "dist/jy_utils-0.0.4.tar", last modified: Tue May  9 08:22:23 2023, max compression
```

## Comparing `jy_utils-0.0.3.tar` & `jy_utils-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 heng.ping  (1004) heng.ping  (1004)        0 2023-05-09 08:01:58.000000 jy_utils-0.0.3/
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      430 2023-05-09 08:01:58.000000 jy_utils-0.0.3/PKG-INFO
-drwxrwxr-x   0 heng.ping  (1004) heng.ping  (1004)        0 2023-05-09 08:01:58.000000 jy_utils-0.0.3/jy_utils.egg-info/
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      256 2023-05-09 08:01:58.000000 jy_utils-0.0.3/jy_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      430 2023-05-09 08:01:58.000000 jy_utils-0.0.3/jy_utils.egg-info/PKG-INFO
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       47 2023-05-09 08:01:58.000000 jy_utils-0.0.3/jy_utils.egg-info/requires.txt
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)        9 2023-05-09 08:01:58.000000 jy_utils-0.0.3/jy_utils.egg-info/top_level.txt
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)        1 2023-05-09 08:01:58.000000 jy_utils-0.0.3/jy_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       38 2023-05-09 08:01:58.000000 jy_utils-0.0.3/setup.cfg
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)     1088 2023-05-09 06:18:12.000000 jy_utils-0.0.3/LICENSE
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      707 2023-05-09 08:01:54.000000 jy_utils-0.0.3/setup.py
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       23 2023-05-09 06:15:28.000000 jy_utils-0.0.3/README.md
-drwxrwxr-x   0 heng.ping  (1004) heng.ping  (1004)        0 2023-05-09 08:01:58.000000 jy_utils-0.0.3/jy_utils/
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      962 2023-05-09 02:33:08.000000 jy_utils-0.0.3/jy_utils/nacos_client.py
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       17 2023-05-09 06:02:26.000000 jy_utils-0.0.3/jy_utils/__init__.py
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)     1879 2023-05-09 02:33:58.000000 jy_utils-0.0.3/jy_utils/redis_client.py
+drwxrwxr-x   0 heng.ping  (1004) heng.ping  (1004)        0 2023-05-09 08:22:23.000000 jy_utils-0.0.4/
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      430 2023-05-09 08:22:23.000000 jy_utils-0.0.4/PKG-INFO
+drwxrwxr-x   0 heng.ping  (1004) heng.ping  (1004)        0 2023-05-09 08:22:23.000000 jy_utils-0.0.4/jy_utils.egg-info/
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      256 2023-05-09 08:22:23.000000 jy_utils-0.0.4/jy_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      430 2023-05-09 08:22:23.000000 jy_utils-0.0.4/jy_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       47 2023-05-09 08:22:23.000000 jy_utils-0.0.4/jy_utils.egg-info/requires.txt
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)        9 2023-05-09 08:22:23.000000 jy_utils-0.0.4/jy_utils.egg-info/top_level.txt
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)        1 2023-05-09 08:22:23.000000 jy_utils-0.0.4/jy_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       38 2023-05-09 08:22:23.000000 jy_utils-0.0.4/setup.cfg
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)     1088 2023-05-09 06:18:12.000000 jy_utils-0.0.4/LICENSE
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      707 2023-05-09 08:22:08.000000 jy_utils-0.0.4/setup.py
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       23 2023-05-09 06:15:28.000000 jy_utils-0.0.4/README.md
+drwxrwxr-x   0 heng.ping  (1004) heng.ping  (1004)        0 2023-05-09 08:22:23.000000 jy_utils-0.0.4/jy_utils/
+-rw-r--r--   0 heng.ping  (1004) heng.ping  (1004)     1304 2023-05-09 08:19:49.000000 jy_utils-0.0.4/jy_utils/nacos_client.py
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       17 2023-05-09 06:02:26.000000 jy_utils-0.0.4/jy_utils/__init__.py
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)     1879 2023-05-09 02:33:58.000000 jy_utils-0.0.4/jy_utils/redis_client.py
```

### Comparing `jy_utils-0.0.3/LICENSE` & `jy_utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jy_utils-0.0.3/setup.py` & `jy_utils-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jy_utils",
-    version="0.0.3",
+    version="0.0.4",
     author="heng.ping",
     author_email="heng.ping@jiyuncorp.com",
     description="jiyuncorp python package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `jy_utils-0.0.3/jy_utils/nacos_client.py` & `jy_utils-0.0.4/jy_utils/nacos_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # -*- coding: utf-8 -*-
 import nacos
 import yaml
+import os
 
 class NacosClient:
-    def __init__(self, server_addresses, name_space, data_id, group="DEFAULT_GROUP"):
+    def __init__(self, config={}):
         # Nacos服务地址 例: nacos-cluster.devops.svc.cluster.local:8848
-        self.server_addresses = server_addresses
+        self.server_addresses = config["server_addresses"] if "server_addresses" in config else \
+            os.environ.get("NACOS_HOST", "nacos-cluster.devops.svc.cluster.local:8848")
         # Nacos命名空间 例: c8200628-e060-407c-bc61-e0827908e3ed
-        self.name_space = name_space
+        self.name_space = config["name_space"] if "name_space" in config else \
+            os.environ.get("NACOS_NAMESPACE", "c8200628-e060-407c-bc61-e0827908e3ed")
         # 配置文件名 例: jiyuncorp-common.yaml
-        self.data_id = data_id
+        self.data_id = config["data_id"] if "data_id" in config else "jiyuncorp-common.yaml"
         # 配置文件组 例如: DEFAULT_GROUP
-        self.group = group
+        self.group = config["group"] if "group" in config else "DEFAULT_GROUP"
 
     def get_nacos(self):
         try:
             client = nacos.NacosClient(self.server_addresses, namespace=self.name_space)
             # 全局服务配置
             server_config = yaml.full_load(client.get_config(self.data_id, self.group))
         except Exception as e:
```

### Comparing `jy_utils-0.0.3/jy_utils/redis_client.py` & `jy_utils-0.0.4/jy_utils/redis_client.py`

 * *Files identical despite different names*

