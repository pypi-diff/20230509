# Comparing `tmp/air-df-0.0.9.tar.gz` & `tmp/air-df-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\air-df-0.0.9.tar", last modified: Mon Dec 27 03:25:18 2021, max compression
+gzip compressed data, was "dist\air-df-0.1.1.tar", last modified: Tue May  9 02:52:48 2023, max compression
```

## Comparing `air-df-0.0.9.tar` & `air-df-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2021-12-27 03:25:18.115346 air-df-0.0.9/
--rw-rw-rw-   0        0        0     1919 2021-12-27 03:25:18.114345 air-df-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1170 2021-12-24 06:22:45.000000 air-df-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2021-12-27 03:25:18.103345 air-df-0.0.9/air/
--rw-rw-rw-   0        0        0      292 2021-12-27 03:24:04.000000 air-df-0.0.9/air/__init__.py
--rw-rw-rw-   0        0        0     3037 2021-12-27 03:18:48.000000 air-df-0.0.9/air/base_handler.py
--rw-rw-rw-   0        0        0    22233 2021-12-24 08:52:04.000000 air-df-0.0.9/air/plugins.py
-drwxrwxrwx   0        0        0        0 2021-12-27 03:25:18.113343 air-df-0.0.9/air_df.egg-info/
--rw-rw-rw-   0        0        0     1919 2021-12-27 03:25:17.000000 air-df-0.0.9/air_df.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2021-12-27 03:25:17.000000 air-df-0.0.9/air_df.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-27 03:25:17.000000 air-df-0.0.9/air_df.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2021-12-27 03:25:17.000000 air-df-0.0.9/air_df.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2021-12-27 03:25:17.000000 air-df-0.0.9/air_df.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-12-27 03:25:18.115346 air-df-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      883 2021-12-27 03:24:41.000000 air-df-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:52:48.097839 air-df-0.1.1/
+-rw-rw-rw-   0        0        0     1916 2023-05-09 02:52:48.096842 air-df-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1170 2023-05-09 02:45:52.000000 air-df-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 02:52:48.074901 air-df-0.1.1/air/
+-rw-rw-rw-   0        0        0      292 2021-12-27 05:36:01.000000 air-df-0.1.1/air/__init__.py
+-rw-rw-rw-   0        0        0     3037 2021-12-27 05:36:01.000000 air-df-0.1.1/air/base_handler.py
+-rw-rw-rw-   0        0        0    23523 2023-05-09 02:51:45.000000 air-df-0.1.1/air/plugins.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:52:48.093850 air-df-0.1.1/air_df.egg-info/
+-rw-rw-rw-   0        0        0     1916 2023-05-09 02:52:47.000000 air-df-0.1.1/air_df.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-05-09 02:52:47.000000 air-df-0.1.1/air_df.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 02:52:47.000000 air-df-0.1.1/air_df.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-05-09 02:52:47.000000 air-df-0.1.1/air_df.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-09 02:52:47.000000 air-df-0.1.1/air_df.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 02:52:48.098837 air-df-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2023-05-09 02:50:34.000000 air-df-0.1.1/setup.py
```

### Comparing `air-df-0.0.9/PKG-INFO` & `air-df-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: air-df
-Version: 0.0.9
+Version: 0.1.1
 Summary: 常用插件
 Home-page: https://github.com/Air-df
 Author: Damon
-Author-email: 527439841@qq.com
+Author-email: 527439@qq.com
 License: UNKNOWN
 Description: ## base_handler -- tornado handler 基类
         
         >主要提供参数检查，并初始化get、post、delete、option等方法
         
         ## plugins -- 插件集合
```

### Comparing `air-df-0.0.9/README.md` & `air-df-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `air-df-0.0.9/air/base_handler.py` & `air-df-0.1.1/air/base_handler.py`

 * *Files identical despite different names*

### Comparing `air-df-0.0.9/air/plugins.py` & `air-df-0.1.1/air/plugins.py`

 * *Files 8% similar despite different names*

```diff
@@ -138,14 +138,38 @@
     def delete(self, key, path=None):
         """
         :return: 1：删除成功； None：键不存在
         """
         return self.conn.delete(f'{path}:{key}') if path else self.conn.delete(key)
 
 
+class RedisLock():
+    """redis 分布式锁"""
+    def __init__(self, lock_name='lock_name', lock_value='lock', expire_sec=30, **kwargs):
+        self.lock_name = lock_name
+        self.lock_value = lock_value
+        self.expire_sec = expire_sec
+        self.r = RedisClient()
+        self.conn = self.r.conn
+        self.result = False
+
+    def __enter__(self):
+        while 1:
+            result = self.conn.setnx(self.lock_name, self.lock_value)
+            self.conn.expire(self.lock_name, self.expire_sec)
+            # result为1，设置成功，result为0，等待继续获取
+            if result:
+                self.result = True
+                return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.conn.delete(self.lock_name)
+        self.result = False
+
+
 class LocalFaker:
     """
     生成随机数据
     """
 
     def __init__(self):
         self.f = Faker(locale='zh_CN')
@@ -236,14 +260,30 @@
     @staticmethod
     def encode(bytestring, k=16):
         l = len(bytestring.encode('utf-8'))
         val = k - (l % k)
         return bytes(bytestring, 'utf-8') + bytes([val] * val)
 
 
+class PKCS5Encoder(object):
+    @staticmethod
+    def decode(bytestring, k=16):
+        val = bytestring[-1]
+        if val > k:
+            raise ValueError('Input is not padded or padding is corrupt')
+        l = len(bytestring) - val
+        return bytestring[:l]
+
+    @staticmethod
+    def encode(bytestring, k=16):
+        l = len(bytestring.encode('utf-8'))
+        val = k - (l % k)
+        return bytes(bytestring, 'utf-8') + bytes([val] * val)
+
+
 class CryptoHelper:
     def __init__(self, key='12345678900000001234567890000000', iv='1234567890000000'):
         self.KEY = bytes(key, 'utf8')
         self.IV = bytes(iv, 'utf8')
 
     @staticmethod
     def encrypt_md5(text):
@@ -608,8 +648,7 @@
     #     s.excute('select * from dbo.Dict t')
     #     results = s.fetchall()
     # for item in results:
     #     print(item)
 
     # with PgClientOrm() as s:
     #     pass
-
```

### Comparing `air-df-0.0.9/air_df.egg-info/PKG-INFO` & `air-df-0.1.1/air_df.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: air-df
-Version: 0.0.9
+Version: 0.1.1
 Summary: 常用插件
 Home-page: https://github.com/Air-df
 Author: Damon
-Author-email: 527439841@qq.com
+Author-email: 527439@qq.com
 License: UNKNOWN
 Description: ## base_handler -- tornado handler 基类
         
         >主要提供参数检查，并初始化get、post、delete、option等方法
         
         ## plugins -- 插件集合
```

### Comparing `air-df-0.0.9/setup.py` & `air-df-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-#!/usr/bin/env python3
-# _*_ coding: utf-8 _*_
-
 import setuptools
 
 with open("README.md", 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 with open("requirements.txt", 'r', encoding='utf-8') as f:
     requirements = f.read().split()
 
 setuptools.setup(
-    name="air-df",  # pip install name
-    version="0.0.9",
+    name="air-df",  					# pip install name
+    version="0.1.1",					# 版本，每次更新需修改，否则无法上传
     author="Damon",
-    author_email="527439841@qq.com",
+    author_email="527439@qq.com",
     description="常用插件",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/Air-df",  # 项目地址
-    packages=['air'],
-    install_requires=requirements,
+    url="https://github.com/Air-df",  	# git-hup 项目地址, 这里只放了主页地址，这个参数不重要
+    packages=['air'],					# 文件夹名
+    install_requires=requirements,  	# 依赖库,发布后，pip install过程中自动安装该参数下的依赖
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    py_modules=[
+    py_modules=[						# 打包的具体文件
         'air.base_handler', 'air.plugins'
     ]
 )
```

