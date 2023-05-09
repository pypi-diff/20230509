# Comparing `tmp/nonebot-plugin-mcqq-1.2.0.tar.gz` & `tmp/nonebot-plugin-mcqq-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcqq-1.2.0.tar", last modified: Mon May  8 07:10:35 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcqq-1.2.1.tar", last modified: Tue May  9 03:14:47 2023, max compression
```

## Comparing `nonebot-plugin-mcqq-1.2.0.tar` & `nonebot-plugin-mcqq-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:35.503512 nonebot-plugin-mcqq-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-08 07:10:29.000000 nonebot-plugin-mcqq-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-08 07:10:35.503512 nonebot-plugin-mcqq-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-08 07:10:29.000000 nonebot-plugin-mcqq-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:10:35.503512 nonebot-plugin-mcqq-1.2.0/nonebot_plugin_mcqq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-08 07:10:35.000000 nonebot-plugin-mcqq-1.2.0/nonebot_plugin_mcqq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-08 07:10:35.000000 nonebot-plugin-mcqq-1.2.0/nonebot_plugin_mcqq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:10:35.000000 nonebot-plugin-mcqq-1.2.0/nonebot_plugin_mcqq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-08 07:10:35.000000 nonebot-plugin-mcqq-1.2.0/nonebot_plugin_mcqq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 07:10:35.000000 nonebot-plugin-mcqq-1.2.0/nonebot_plugin_mcqq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 07:10:35.503512 nonebot-plugin-mcqq-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-08 07:10:29.000000 nonebot-plugin-mcqq-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:14:47.557895 nonebot-plugin-mcqq-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-09 03:14:40.000000 nonebot-plugin-mcqq-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-09 03:14:47.557895 nonebot-plugin-mcqq-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-09 03:14:40.000000 nonebot-plugin-mcqq-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:14:47.557895 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-09 03:14:40.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-09 03:14:40.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-09 03:14:40.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:14:47.557895 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-09 03:14:47.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-09 03:14:47.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:14:47.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-09 03:14:47.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 03:14:47.000000 nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 03:14:47.557895 nonebot-plugin-mcqq-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-09 03:14:40.000000 nonebot-plugin-mcqq-1.2.1/setup.py
```

### Comparing `nonebot-plugin-mcqq-1.2.0/LICENSE` & `nonebot-plugin-mcqq-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.0/PKG-INFO` & `nonebot-plugin-mcqq-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.2.0
+Version: 1.2.1
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.2.0/README.md` & `nonebot-plugin-mcqq-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.0/nonebot_plugin_mcqq.egg-info/PKG-INFO` & `nonebot-plugin-mcqq-1.2.1/nonebot_plugin_mcqq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.2.0
+Version: 1.2.1
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.2.0/setup.py` & `nonebot-plugin-mcqq-1.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-mcqq",
-    version="1.2.0",
+    version="1.2.1",
     author="17TheWord",
     author_email="17theword@gmail.com",
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通插件",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/17TheWord/nonebot-plugin-mcqq",
-    py_modules=['nonebot_plugin_mcqq'],
-    packages=[],
+    packages=["nonebot_plugin_mcqq"],
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent"
     ],
     install_requires=[
         'mcqq-tool>=0.0.5',
```

