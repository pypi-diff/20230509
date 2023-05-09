# Comparing `tmp/liteindex-0.0.1.dev6.tar.gz` & `tmp/liteindex-0.0.1.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteindex-0.0.1.dev6.tar", last modified: Tue May  9 03:55:59 2023, max compression
+gzip compressed data, was "liteindex-0.0.1.dev7.tar", last modified: Tue May  9 03:59:25 2023, max compression
```

## Comparing `liteindex-0.0.1.dev6.tar` & `liteindex-0.0.1.dev7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:59.237019 liteindex-0.0.1.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 03:55:59.237019 liteindex-0.0.1.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:59.233019 liteindex-0.0.1.dev6/liteindex/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/liteindex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/liteindex/any_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/liteindex/defined_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/liteindex/dict_index_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/liteindex/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/liteindex/number_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:59.237019 liteindex-0.0.1.dev6/liteindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 03:55:59.000000 liteindex-0.0.1.dev6/liteindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 03:55:59.000000 liteindex-0.0.1.dev6/liteindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:55:59.000000 liteindex-0.0.1.dev6/liteindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 03:55:59.000000 liteindex-0.0.1.dev6/liteindex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 03:55:59.000000 liteindex-0.0.1.dev6/liteindex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 03:55:59.237019 liteindex-0.0.1.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:59:25.519761 liteindex-0.0.1.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 03:59:25.519761 liteindex-0.0.1.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:59:25.519761 liteindex-0.0.1.dev7/liteindex/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/liteindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/liteindex/any_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/liteindex/defined_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/liteindex/dict_index_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/liteindex/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/liteindex/number_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:59:25.519761 liteindex-0.0.1.dev7/liteindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 03:59:25.000000 liteindex-0.0.1.dev7/liteindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 03:59:25.000000 liteindex-0.0.1.dev7/liteindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:59:25.000000 liteindex-0.0.1.dev7/liteindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 03:59:25.000000 liteindex-0.0.1.dev7/liteindex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 03:59:25.000000 liteindex-0.0.1.dev7/liteindex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 03:59:25.519761 liteindex-0.0.1.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/setup.py
```

### Comparing `liteindex-0.0.1.dev6/LICENSE` & `liteindex-0.0.1.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev6/PKG-INFO` & `liteindex-0.0.1.dev7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteindex
-Version: 0.0.1.dev6
+Version: 0.0.1.dev7
 Summary: SQLite based queryable python indexes for dicts and lists
 Home-page: https://github.com/notAI-tech/liteindex
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `liteindex-0.0.1.dev6/README.md` & `liteindex-0.0.1.dev7/README.md`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev6/liteindex/any_index.py` & `liteindex-0.0.1.dev7/liteindex/any_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev6/liteindex/defined_index.py` & `liteindex-0.0.1.dev7/liteindex/defined_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev6/liteindex/dict_index_helpers.py` & `liteindex-0.0.1.dev7/liteindex/dict_index_helpers.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev6/liteindex/file_index.py` & `liteindex-0.0.1.dev7/liteindex/file_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev6/liteindex/number_index.py` & `liteindex-0.0.1.dev7/liteindex/number_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev6/liteindex.egg-info/PKG-INFO` & `liteindex-0.0.1.dev7/liteindex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteindex
-Version: 0.0.1.dev6
+Version: 0.0.1.dev7
 Summary: SQLite based queryable python indexes for dicts and lists
 Home-page: https://github.com/notAI-tech/liteindex
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `liteindex-0.0.1.dev6/setup.py` & `liteindex-0.0.1.dev7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "liteindex"
 DESCRIPTION = "SQLite based queryable python indexes for dicts and lists"
 URL = "https://github.com/notAI-tech/liteindex"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev6"
+VERSION = "0.0.1.dev7"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
 ]
 
 # What packages are optional?
 EXTRAS = {
```

