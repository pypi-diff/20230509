# Comparing `tmp/skytek-utils-0.1.0.tar.gz` & `tmp/skytek-utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytek-utils-0.1.0.tar", last modified: Thu Apr 20 11:57:34 2023, max compression
+gzip compressed data, was "skytek-utils-0.2.0.tar", last modified: Tue May  9 19:05:07 2023, max compression
```

## Comparing `skytek-utils-0.1.0.tar` & `skytek-utils-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:57:34.245043 skytek-utils-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-20 11:57:34.245043 skytek-utils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 11:57:34.245043 skytek-utils-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:57:34.241043 skytek-utils-0.1.0/skytek_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 11:57:27.000000 skytek-utils-0.1.0/skytek_utils/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/skytek_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/skytek_utils/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/skytek_utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:57:34.245043 skytek-utils-0.1.0/skytek_utils/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/skytek_utils/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/skytek_utils/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/skytek_utils/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/skytek_utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/skytek_utils/json_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/skytek_utils/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:57:34.245043 skytek-utils-0.1.0/skytek_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-20 11:57:34.000000 skytek-utils-0.1.0/skytek_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-20 11:57:34.000000 skytek-utils-0.1.0/skytek_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:57:34.000000 skytek-utils-0.1.0/skytek_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:57:34.000000 skytek-utils-0.1.0/skytek_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 11:57:34.000000 skytek-utils-0.1.0/skytek_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:57:34.245043 skytek-utils-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-20 11:57:24.000000 skytek-utils-0.1.0/tests/test_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:05:07.795386 skytek-utils-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-09 19:05:07.795386 skytek-utils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:05:07.795386 skytek-utils-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:05:07.791386 skytek-utils-0.2.0/skytek_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 19:04:57.000000 skytek-utils-0.2.0/skytek_utils/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:05:07.795386 skytek-utils-0.2.0/skytek_utils/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/json_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:05:07.795386 skytek-utils-0.2.0/skytek_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-09 19:05:07.000000 skytek-utils-0.2.0/skytek_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-09 19:05:07.000000 skytek-utils-0.2.0/skytek_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:05:07.000000 skytek-utils-0.2.0/skytek_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:05:07.000000 skytek-utils-0.2.0/skytek_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 19:05:07.000000 skytek-utils-0.2.0/skytek_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:05:07.795386 skytek-utils-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/tests/test_iter.py
```

### Comparing `skytek-utils-0.1.0/LICENSE` & `skytek-utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.1.0/PKG-INFO` & `skytek-utils-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: skytek-utils - a set of small util functions
 Home-page: http://github.com/Skytek/skytek-utils
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek-utils-0.1.0/setup.py` & `skytek-utils-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.1.0/skytek_utils/celery.py` & `skytek-utils-0.2.0/skytek_utils/celery.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.1.0/skytek_utils/datetime.py` & `skytek-utils-0.2.0/skytek_utils/datetime.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.1.0/skytek_utils/json_stream.py` & `skytek-utils-0.2.0/skytek_utils/json_stream.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.1.0/skytek_utils/monitoring.py` & `skytek-utils-0.2.0/skytek_utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.1.0/skytek_utils.egg-info/PKG-INFO` & `skytek-utils-0.2.0/skytek_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: skytek-utils - a set of small util functions
 Home-page: http://github.com/Skytek/skytek-utils
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek-utils-0.1.0/skytek_utils.egg-info/SOURCES.txt` & `skytek-utils-0.2.0/skytek_utils.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.py
 skytek_utils/VERSION
 skytek_utils/__init__.py
 skytek_utils/celery.py
 skytek_utils/datetime.py
+skytek_utils/files.py
 skytek_utils/iter.py
 skytek_utils/json_stream.py
 skytek_utils/monitoring.py
 skytek_utils.egg-info/PKG-INFO
 skytek_utils.egg-info/SOURCES.txt
 skytek_utils.egg-info/dependency_links.txt
 skytek_utils.egg-info/not-zip-safe
```

### Comparing `skytek-utils-0.1.0/tests/test_iter.py` & `skytek-utils-0.2.0/tests/test_iter.py`

 * *Files identical despite different names*

