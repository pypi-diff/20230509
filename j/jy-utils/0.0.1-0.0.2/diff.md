# Comparing `tmp/jy_utils-0.0.1.tar.gz` & `tmp/jy_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jy_utils-0.0.1.tar", last modified: Tue May  9 06:26:11 2023, max compression
+gzip compressed data, was "dist/jy_utils-0.0.2.tar", last modified: Tue May  9 07:56:35 2023, max compression
```

## Comparing `jy_utils-0.0.1.tar` & `jy_utils-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 heng.ping  (1004) heng.ping  (1004)        0 2023-05-09 06:26:11.000000 jy_utils-0.0.1/
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      430 2023-05-09 06:26:11.000000 jy_utils-0.0.1/PKG-INFO
-drwxrwxr-x   0 heng.ping  (1004) heng.ping  (1004)        0 2023-05-09 06:26:11.000000 jy_utils-0.0.1/jy_utils.egg-info/
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      256 2023-05-09 06:26:11.000000 jy_utils-0.0.1/jy_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      430 2023-05-09 06:26:11.000000 jy_utils-0.0.1/jy_utils.egg-info/PKG-INFO
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       34 2023-05-09 06:26:11.000000 jy_utils-0.0.1/jy_utils.egg-info/requires.txt
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)        9 2023-05-09 06:26:11.000000 jy_utils-0.0.1/jy_utils.egg-info/top_level.txt
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)        1 2023-05-09 06:26:11.000000 jy_utils-0.0.1/jy_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       38 2023-05-09 06:26:11.000000 jy_utils-0.0.1/setup.cfg
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)     1088 2023-05-09 06:18:12.000000 jy_utils-0.0.1/LICENSE
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      692 2023-05-09 06:19:18.000000 jy_utils-0.0.1/setup.py
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       23 2023-05-09 06:15:28.000000 jy_utils-0.0.1/README.md
-drwxrwxr-x   0 heng.ping  (1004) heng.ping  (1004)        0 2023-05-09 06:26:11.000000 jy_utils-0.0.1/jy_utils/
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      962 2023-05-09 02:33:08.000000 jy_utils-0.0.1/jy_utils/nacos_client.py
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       17 2023-05-09 06:02:26.000000 jy_utils-0.0.1/jy_utils/__init__.py
--rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)     1879 2023-05-09 02:33:58.000000 jy_utils-0.0.1/jy_utils/redis_client.py
+drwxrwxr-x   0 heng.ping  (1004) heng.ping  (1004)        0 2023-05-09 07:56:35.000000 jy_utils-0.0.2/
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      430 2023-05-09 07:56:35.000000 jy_utils-0.0.2/PKG-INFO
+drwxrwxr-x   0 heng.ping  (1004) heng.ping  (1004)        0 2023-05-09 07:56:35.000000 jy_utils-0.0.2/jy_utils.egg-info/
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      256 2023-05-09 07:56:35.000000 jy_utils-0.0.2/jy_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      430 2023-05-09 07:56:35.000000 jy_utils-0.0.2/jy_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       45 2023-05-09 07:56:35.000000 jy_utils-0.0.2/jy_utils.egg-info/requires.txt
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)        9 2023-05-09 07:56:35.000000 jy_utils-0.0.2/jy_utils.egg-info/top_level.txt
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)        1 2023-05-09 07:56:35.000000 jy_utils-0.0.2/jy_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       38 2023-05-09 07:56:35.000000 jy_utils-0.0.2/setup.cfg
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)     1088 2023-05-09 06:18:12.000000 jy_utils-0.0.2/LICENSE
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      705 2023-05-09 07:55:55.000000 jy_utils-0.0.2/setup.py
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       23 2023-05-09 06:15:28.000000 jy_utils-0.0.2/README.md
+drwxrwxr-x   0 heng.ping  (1004) heng.ping  (1004)        0 2023-05-09 07:56:35.000000 jy_utils-0.0.2/jy_utils/
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)      962 2023-05-09 02:33:08.000000 jy_utils-0.0.2/jy_utils/nacos_client.py
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)       17 2023-05-09 06:02:26.000000 jy_utils-0.0.2/jy_utils/__init__.py
+-rw-rw-r--   0 heng.ping  (1004) heng.ping  (1004)     1879 2023-05-09 02:33:58.000000 jy_utils-0.0.2/jy_utils/redis_client.py
```

### Comparing `jy_utils-0.0.1/LICENSE` & `jy_utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jy_utils-0.0.1/setup.py` & `jy_utils-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jy_utils",
-    version="0.0.1",
+    version="0.0.2",
     author="heng.ping",
     author_email="heng.ping@jiyuncorp.com",
     description="jiyuncorp python package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'nacos',
+        'nacos-sdk-python',
         'yaml',
         'redis-py-cluster',
         'redis'
     ],
-)
+)
```

### Comparing `jy_utils-0.0.1/jy_utils/nacos_client.py` & `jy_utils-0.0.2/jy_utils/nacos_client.py`

 * *Files identical despite different names*

### Comparing `jy_utils-0.0.1/jy_utils/redis_client.py` & `jy_utils-0.0.2/jy_utils/redis_client.py`

 * *Files identical despite different names*

