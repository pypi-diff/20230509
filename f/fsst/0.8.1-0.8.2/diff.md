# Comparing `tmp/fsst-0.8.1.tar.gz` & `tmp/fsst-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsst-0.8.1.tar", last modified: Tue May  9 19:41:43 2023, max compression
+gzip compressed data, was "fsst-0.8.2.tar", last modified: Tue May  9 20:12:51 2023, max compression
```

## Comparing `fsst-0.8.1.tar` & `fsst-0.8.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 19:41:43.267390 fsst-0.8.1/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 19:41:43.267390 fsst-0.8.1/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.1/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 19:41:43.267390 fsst-0.8.1/fsst.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 19:41:42.000000 fsst-0.8.1/fsst.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-05-09 19:41:43.000000 fsst-0.8.1/fsst.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-09 19:41:42.000000 fsst-0.8.1/fsst.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-05-09 19:41:42.000000 fsst-0.8.1/fsst.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.1/fsst.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       80 2023-05-09 19:41:43.000000 fsst-0.8.1/fsst.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-05-09 19:41:43.000000 fsst-0.8.1/fsst.egg-info/top_level.txt
--rwxrwxr-x   0 rob       (1000) rob       (1000)   116353 2023-05-09 19:40:45.000000 fsst-0.8.1/fsst.py
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-09 19:41:43.267390 fsst-0.8.1/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)     1162 2023-05-09 19:40:12.000000 fsst-0.8.1/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 20:12:51.428821 fsst-0.8.2/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 20:12:51.428821 fsst-0.8.2/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.2/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 20:12:51.428821 fsst-0.8.2/fsst.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 20:12:50.000000 fsst-0.8.2/fsst.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-05-09 20:12:51.000000 fsst-0.8.2/fsst.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-09 20:12:50.000000 fsst-0.8.2/fsst.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-05-09 20:12:51.000000 fsst-0.8.2/fsst.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.2/fsst.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       88 2023-05-09 20:12:51.000000 fsst-0.8.2/fsst.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-05-09 20:12:51.000000 fsst-0.8.2/fsst.egg-info/top_level.txt
+-rwxrwxr-x   0 rob       (1000) rob       (1000)   116353 2023-05-09 19:40:45.000000 fsst-0.8.2/fsst.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-09 20:12:51.428821 fsst-0.8.2/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1170 2023-05-09 20:11:58.000000 fsst-0.8.2/setup.py
```

### Comparing `fsst-0.8.1/PKG-INFO` & `fsst-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.1
+Version: 0.8.2
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.1/README.md` & `fsst-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `fsst-0.8.1/fsst.egg-info/PKG-INFO` & `fsst-0.8.2/fsst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.1
+Version: 0.8.2
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.1/fsst.py` & `fsst-0.8.2/fsst.py`

 * *Files identical despite different names*

### Comparing `fsst-0.8.1/setup.py` & `fsst-0.8.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='fsst',
-    version="0.8.1",
+    version="0.8.2",
     description="Fluree Schema Scenario Tool",
     long_description="Testing tool for schema and smart function unit tests for FlureeDB",
     author='Rob Meijer',
     author_email='pibara@gmail.com',
     url='https://github.com/pibara/fluree-schema-scenario-tool',
     license='BSD',
     py_modules=['fsst'],
@@ -25,10 +25,10 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    install_requires=["base58", "aioflureedb>=0.6.4", "requests"],
+    install_requires=["base58", "aioflureedb>=0.6.4", "requests<=2.28.1"],
     extras_require={'domainapi': ['jsonata>=0.2.3'], 'docker': ['docker']}
 )
```

