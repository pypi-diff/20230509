# Comparing `tmp/rape_identification-0.1.1.tar.gz` & `tmp/rape_identification-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rape_identification-0.1.1.tar", last modified: Tue May  9 10:49:41 2023, max compression
+gzip compressed data, was "rape_identification-0.1.2.tar", last modified: Tue May  9 10:55:55 2023, max compression
```

## Comparing `rape_identification-0.1.1.tar` & `rape_identification-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:49:41.909010 rape_identification-0.1.1/
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 10:49:41.909010 rape_identification-0.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:49:41.909010 rape_identification-0.1.1/rape_identification/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.1/rape_identification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:49:41.909010 rape_identification-0.1.1/rape_identification/config/
--rw-rw-r--   0 root         (0) root         (0)      454 2023-05-09 09:48:54.000000 rape_identification-0.1.1/rape_identification/config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2428 2023-05-09 09:48:54.000000 rape_identification-0.1.1/rape_identification/config/default.py
--rw-rw-r--   0 root         (0) root         (0)     1895 2023-05-09 09:48:54.000000 rape_identification-0.1.1/rape_identification/config/default_test.py
--rw-rw-r--   0 root         (0) root         (0)      706 2023-05-09 09:48:54.000000 rape_identification-0.1.1/rape_identification/inference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:49:41.909010 rape_identification-0.1.1/rape_identification.egg-info/
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 10:49:41.000000 rape_identification-0.1.1/rape_identification.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-09 10:49:41.000000 rape_identification-0.1.1/rape_identification.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 10:49:41.000000 rape_identification-0.1.1/rape_identification.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-09 10:49:41.000000 rape_identification-0.1.1/rape_identification.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-09 10:49:41.000000 rape_identification-0.1.1/rape_identification.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 10:49:41.909010 rape_identification-0.1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      937 2023-05-09 10:49:19.000000 rape_identification-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:55:55.790207 rape_identification-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 10:55:55.790207 rape_identification-0.1.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:55:55.790207 rape_identification-0.1.2/rape_identification/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:55:55.790207 rape_identification-0.1.2/rape_identification/config/
+-rw-rw-r--   0 root         (0) root         (0)      454 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2428 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/config/default.py
+-rw-rw-r--   0 root         (0) root         (0)     1895 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/config/default_test.py
+-rw-rw-r--   0 root         (0) root         (0)      706 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/inference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:55:55.790207 rape_identification-0.1.2/rape_identification/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 10:54:56.000000 rape_identification-0.1.2/rape_identification/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2764 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/utils/convert2uint8.py
+-rw-rw-r--   0 root         (0) root         (0)      866 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/utils/segment.py
+-rw-rw-r--   0 root         (0) root         (0)     4089 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/utils/test.py
+-rw-rw-r--   0 root         (0) root         (0)    13774 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:55:55.790207 rape_identification-0.1.2/rape_identification.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 10:55:55.000000 rape_identification-0.1.2/rape_identification.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      604 2023-05-09 10:55:55.000000 rape_identification-0.1.2/rape_identification.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 10:55:55.000000 rape_identification-0.1.2/rape_identification.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-09 10:55:55.000000 rape_identification-0.1.2/rape_identification.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-09 10:55:55.000000 rape_identification-0.1.2/rape_identification.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 10:55:55.790207 rape_identification-0.1.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      937 2023-05-09 10:55:40.000000 rape_identification-0.1.2/setup.py
```

### Comparing `rape_identification-0.1.1/PKG-INFO` & `rape_identification-0.1.2/rape_identification.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rape_identification
-Version: 0.1.1
+Name: rape-identification
+Version: 0.1.2
 Summary: Segmentation any rape
 Author: PingYang
 Author-email: PingYang97@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rape_identification-0.1.1/rape_identification/config/default.py` & `rape_identification-0.1.2/rape_identification/config/default.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.1/rape_identification/config/default_test.py` & `rape_identification-0.1.2/rape_identification/config/default_test.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.1/rape_identification/inference.py` & `rape_identification-0.1.2/rape_identification/inference.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.1/rape_identification.egg-info/PKG-INFO` & `rape_identification-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rape-identification
-Version: 0.1.1
+Name: rape_identification
+Version: 0.1.2
 Summary: Segmentation any rape
 Author: PingYang
 Author-email: PingYang97@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rape_identification-0.1.1/setup.py` & `rape_identification-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rape_identification',  # 与项目文件夹结构中的包名相同
-    version='0.1.1',
+    version='0.1.2',
     description='Segmentation any rape',
     author='PingYang',
     author_email='PingYang97@163.com',
     # url='https://github.com/yourusername/your_project',
     packages=find_packages(),
     install_requires=[
         # Add your project's dependencies here, e.g., 'numpy', 'pandas', etc.
```

