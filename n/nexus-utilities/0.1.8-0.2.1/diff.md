# Comparing `tmp/nexus-utilities-0.1.8.tar.gz` & `tmp/nexus-utilities-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.1.8.tar", last modified: Tue May  2 15:49:36 2023, max compression
+gzip compressed data, was "nexus-utilities-0.2.1.tar", last modified: Tue May  9 14:14:28 2023, max compression
```

## Comparing `nexus-utilities-0.1.8.tar` & `nexus-utilities-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:49:36.154986 nexus-utilities-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-02 15:49:16.000000 nexus-utilities-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 15:49:36.154986 nexus-utilities-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-02 15:49:16.000000 nexus-utilities-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:49:36.154986 nexus-utilities-0.1.8/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 15:49:35.000000 nexus-utilities-0.1.8/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-02 15:49:36.000000 nexus-utilities-0.1.8/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:49:35.000000 nexus-utilities-0.1.8/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 15:49:35.000000 nexus-utilities-0.1.8/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 15:49:35.000000 nexus-utilities-0.1.8/nexus_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:49:36.154986 nexus-utilities-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-02 15:49:16.000000 nexus-utilities-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:49:36.154986 nexus-utilities-0.1.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:49:16.000000 nexus-utilities-0.1.8/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:14:28.138808 nexus-utilities-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-09 14:14:10.000000 nexus-utilities-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-09 14:14:28.138808 nexus-utilities-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-05-09 14:14:10.000000 nexus-utilities-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:14:28.134807 nexus-utilities-0.2.1/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-09 14:14:27.000000 nexus-utilities-0.2.1/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-09 14:14:28.000000 nexus-utilities-0.2.1/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:14:27.000000 nexus-utilities-0.2.1/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-09 14:14:27.000000 nexus-utilities-0.2.1/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 14:14:27.000000 nexus-utilities-0.2.1/nexus_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:14:28.138808 nexus-utilities-0.2.1/nexus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 14:14:10.000000 nexus-utilities-0.2.1/nexus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-09 14:14:10.000000 nexus-utilities-0.2.1/nexus_utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-09 14:14:10.000000 nexus-utilities-0.2.1/nexus_utils/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-09 14:14:10.000000 nexus-utilities-0.2.1/nexus_utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-09 14:14:10.000000 nexus-utilities-0.2.1/nexus_utils/password_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:14:28.138808 nexus-utilities-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-09 14:14:10.000000 nexus-utilities-0.2.1/setup.py
```

### Comparing `nexus-utilities-0.1.8/LICENSE.txt` & `nexus-utilities-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.1.8/PKG-INFO` & `nexus-utilities-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.1.8
+Version: 0.2.1
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.1.8/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.2.1/nexus_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.1.8
+Version: 0.2.1
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.1.8/setup.py` & `nexus-utilities-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.1.8',
+    version='0.2.1',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus-utilities',
-    packages=find_packages(),
+    packages=['nexus_utils'],
     install_requires=[
         'boto3>=1.26.45',
+        'configparser >=5.3.0',
+        'sqlalchemy>=1.4.44',
+        'keyring>=23.13.1',
+        'chardet>=3.0.4',
         'twine>=3.4.0'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

