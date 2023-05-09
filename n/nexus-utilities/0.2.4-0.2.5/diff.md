# Comparing `tmp/nexus-utilities-0.2.4.tar.gz` & `tmp/nexus-utilities-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.2.4.tar", last modified: Tue May  9 16:27:29 2023, max compression
+gzip compressed data, was "nexus-utilities-0.2.5.tar", last modified: Tue May  9 16:30:19 2023, max compression
```

## Comparing `nexus-utilities-0.2.4.tar` & `nexus-utilities-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:27:29.845853 nexus-utilities-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-09 16:27:15.000000 nexus-utilities-0.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-09 16:27:29.845853 nexus-utilities-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-05-09 16:27:15.000000 nexus-utilities-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:27:29.845853 nexus-utilities-0.2.4/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-09 16:27:29.000000 nexus-utilities-0.2.4/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-09 16:27:29.000000 nexus-utilities-0.2.4/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:27:29.000000 nexus-utilities-0.2.4/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-09 16:27:29.000000 nexus-utilities-0.2.4/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 16:27:29.000000 nexus-utilities-0.2.4/nexus_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:27:29.845853 nexus-utilities-0.2.4/nexus_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 16:27:15.000000 nexus-utilities-0.2.4/nexus_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-09 16:27:15.000000 nexus-utilities-0.2.4/nexus_utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-05-09 16:27:15.000000 nexus-utilities-0.2.4/nexus_utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-09 16:27:15.000000 nexus-utilities-0.2.4/nexus_utils/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-09 16:27:15.000000 nexus-utilities-0.2.4/nexus_utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-09 16:27:15.000000 nexus-utilities-0.2.4/nexus_utils/password_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:27:29.845853 nexus-utilities-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-09 16:27:15.000000 nexus-utilities-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:30:19.610163 nexus-utilities-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-09 16:30:07.000000 nexus-utilities-0.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-09 16:30:19.610163 nexus-utilities-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-05-09 16:30:07.000000 nexus-utilities-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:30:19.606163 nexus-utilities-0.2.5/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-09 16:30:19.000000 nexus-utilities-0.2.5/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-09 16:30:19.000000 nexus-utilities-0.2.5/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:30:19.000000 nexus-utilities-0.2.5/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-09 16:30:19.000000 nexus-utilities-0.2.5/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 16:30:19.000000 nexus-utilities-0.2.5/nexus_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:30:19.610163 nexus-utilities-0.2.5/nexus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 16:30:07.000000 nexus-utilities-0.2.5/nexus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-09 16:30:07.000000 nexus-utilities-0.2.5/nexus_utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-09 16:30:07.000000 nexus-utilities-0.2.5/nexus_utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-09 16:30:07.000000 nexus-utilities-0.2.5/nexus_utils/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-09 16:30:07.000000 nexus-utilities-0.2.5/nexus_utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-09 16:30:07.000000 nexus-utilities-0.2.5/nexus_utils/password_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:30:19.610163 nexus-utilities-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-09 16:30:07.000000 nexus-utilities-0.2.5/setup.py
```

### Comparing `nexus-utilities-0.2.4/LICENSE.txt` & `nexus-utilities-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.4/PKG-INFO` & `nexus-utilities-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.2.4
+Version: 0.2.5
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.2.4/README.md` & `nexus-utilities-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.4/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.2.5/nexus_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.2.4
+Version: 0.2.5
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.2.4/nexus_utils/config_utils.py` & `nexus-utilities-0.2.5/nexus_utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.4/nexus_utils/database_utils.py` & `nexus-utilities-0.2.5/nexus_utils/database_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import re
 
 # pylint: disable=line-too-long
 # pylint: disable=trailing-whitespace
 
 #%%
 # def build_engine(config_path, config_entry, password_method="keyring"):
-def build_engine(connect_type, server_address, server_port, database_name, user_name, password)#, schema=None):
+def build_engine(connect_type, server_address, server_port, database_name, user_name, password):#, schema=None):
     """Build SQL Alchemy Engine based on input parameters"""
 
     # db_config = cr.read_config_file(config_path)
     # connect_type = db_config[config_entry]['connect_type']
     # #environment = db_config[config_entry]['environment']
     # server_address = db_config[config_entry]['server_address']
     # server_port = db_config[config_entry]['server_port']
```

### Comparing `nexus-utilities-0.2.4/nexus_utils/datetime_utils.py` & `nexus-utilities-0.2.5/nexus_utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.4/nexus_utils/package_utils.py` & `nexus-utilities-0.2.5/nexus_utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.4/nexus_utils/password_utils.py` & `nexus-utilities-0.2.5/nexus_utils/password_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.4/setup.py` & `nexus-utilities-0.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.2.4',
+    version='0.2.5',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus-utilities',
     packages=['nexus_utils'],
```

