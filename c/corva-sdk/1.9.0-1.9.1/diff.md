# Comparing `tmp/corva-sdk-1.9.0.tar.gz` & `tmp/corva-sdk-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corva-sdk-1.9.0.tar", last modified: Mon Mar  6 12:28:52 2023, max compression
+gzip compressed data, was "corva-sdk-1.9.1.tar", last modified: Tue May  9 15:49:07 2023, max compression
```

## Comparing `corva-sdk-1.9.0.tar` & `corva-sdk-1.9.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:28:52.725754 corva-sdk-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-03-06 12:28:52.725754 corva-sdk-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-06 12:28:52.725754 corva-sdk-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:28:52.717754 corva-sdk-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:28:52.721754 corva-sdk-1.9.0/src/corva/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/cache_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:28:52.721754 corva-sdk-1.9.0/src/corva/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/rerun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:28:52.721754 corva-sdk-1.9.0/src/corva/models/scheduled/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/scheduled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/scheduled/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/scheduled/scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/scheduled/scheduler_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:28:52.725754 corva-sdk-1.9.0/src/corva/models/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/stream/initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/stream/log_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/stream/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/models/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:28:52.725754 corva-sdk-1.9.0/src/corva/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/service/api_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/service/cache_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/service/service.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/corva/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:28:52.725754 corva-sdk-1.9.0/src/corva_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-03-06 12:28:52.000000 corva-sdk-1.9.0/src/corva_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-06 12:28:52.000000 corva-sdk-1.9.0/src/corva_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 12:28:52.000000 corva-sdk-1.9.0/src/corva_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-06 12:28:52.000000 corva-sdk-1.9.0/src/corva_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-06 12:28:52.000000 corva-sdk-1.9.0/src/corva_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-06 12:28:52.000000 corva-sdk-1.9.0/src/corva_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-06 12:28:45.000000 corva-sdk-1.9.0/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:49:07.480038 corva-sdk-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-05-09 15:49:07.480038 corva-sdk-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-09 15:49:07.480038 corva-sdk-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:49:07.476038 corva-sdk-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:49:07.476038 corva-sdk-1.9.1/src/corva/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/cache_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:49:07.476038 corva-sdk-1.9.1/src/corva/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/rerun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:49:07.476038 corva-sdk-1.9.1/src/corva/models/scheduled/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/scheduled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/scheduled/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/scheduled/scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/scheduled/scheduler_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:49:07.476038 corva-sdk-1.9.1/src/corva/models/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/stream/initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/stream/log_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/stream/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/models/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:49:07.476038 corva-sdk-1.9.1/src/corva/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/service/api_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/service/cache_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/corva/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:49:07.480038 corva-sdk-1.9.1/src/corva_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-05-09 15:49:07.000000 corva-sdk-1.9.1/src/corva_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-09 15:49:07.000000 corva-sdk-1.9.1/src/corva_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:49:07.000000 corva-sdk-1.9.1/src/corva_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 15:49:07.000000 corva-sdk-1.9.1/src/corva_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-09 15:49:07.000000 corva-sdk-1.9.1/src/corva_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 15:49:07.000000 corva-sdk-1.9.1/src/corva_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 15:49:03.000000 corva-sdk-1.9.1/src/version.py
```

### Comparing `corva-sdk-1.9.0/PKG-INFO` & `corva-sdk-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corva-sdk
-Version: 1.9.0
+Version: 1.9.1
 Summary: SDK for building Corva DevCenter Python apps.
 Home-page: https://github.com/corva-ai/python-sdk
 Author: Jordan Ambra
 Author-email: jordan.ambra@corva.ai
 License: The Unlicense
 Keywords: corva,sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,14 +44,20 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [1.9.1] - 2023-05-09
+
+### Fixed
+- `urllib3` v2 not supported by AWS Lambda.
+
+
 ## [1.9.0] - 2023-03-06
 
 ### Added
 - `log_identifier` field to stream depth events.
 
 ### Changed
 - Reraise exceptions in `task` apps
@@ -366,15 +372,16 @@
 - `ScheduledApp` to build scheduled apps.
 - `TaskApp` to build task apps.
 - `Api` class to access Platform and Data Corva APIs.
 - `Cache` class to share data between app invokes.
 - Event classes: `StreamEvent`, `ScheduledEvent` and `TaskEvent`.
 
 
-[Unreleased] https://github.com/corva-ai/python-sdk/compare/v1.9.0...master
+[Unreleased] https://github.com/corva-ai/python-sdk/compare/v1.9.1...master
+[1.9.1] https://github.com/corva-ai/python-sdk/compare/v1.9.0...v1.9.1
 [1.9.0] https://github.com/corva-ai/python-sdk/compare/v1.8.1...v1.9.0
 [1.8.1] https://github.com/corva-ai/python-sdk/compare/v1.8.0...v1.8.1
 [1.8.0] https://github.com/corva-ai/python-sdk/compare/v1.7.0...v1.8.0
 [1.7.0] https://github.com/corva-ai/python-sdk/compare/v1.6.0...v1.7.0
 [1.6.0] https://github.com/corva-ai/python-sdk/compare/v1.5.3...v1.6.0
 [1.5.3] https://github.com/corva-ai/python-sdk/compare/v1.5.2...v1.5.3
 [1.5.2] https://github.com/corva-ai/python-sdk/compare/v1.5.1...v1.5.2
```

### Comparing `corva-sdk-1.9.0/setup.cfg` & `corva-sdk-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/setup.py` & `corva-sdk-1.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,12 +39,13 @@
     packages=setuptools.find_packages("src"),
     package_dir={"": "src"},
     install_requires=[
         "fakeredis[lua] >=1.4.5, <2.0.0",
         "pydantic >=1.8.2, <2.0.0",
         "redis >=3.5.3, <4.0.0",
         "requests >=2.25.0, <3.0.0",
+        "urllib3 <2",  # lambda doesnt support version 2 yet
     ],
     python_requires='>=3.8, <4.0',
     license='The Unlicense',
     entry_points={"pytest11": ["corva = plugin"]},
 )
```

### Comparing `corva-sdk-1.9.0/src/corva/__init__.py` & `corva-sdk-1.9.1/src/corva/__init__.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/api.py` & `corva-sdk-1.9.1/src/corva/api.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/cache_adapter.py` & `corva-sdk-1.9.1/src/corva/cache_adapter.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/configuration.py` & `corva-sdk-1.9.1/src/corva/configuration.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/handlers.py` & `corva-sdk-1.9.1/src/corva/handlers.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/logger.py` & `corva-sdk-1.9.1/src/corva/logger.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/models/context.py` & `corva-sdk-1.9.1/src/corva/models/context.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/models/rerun.py` & `corva-sdk-1.9.1/src/corva/models/rerun.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/models/scheduled/raw.py` & `corva-sdk-1.9.1/src/corva/models/scheduled/raw.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/models/scheduled/scheduled.py` & `corva-sdk-1.9.1/src/corva/models/scheduled/scheduled.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/models/scheduled/scheduler_type.py` & `corva-sdk-1.9.1/src/corva/models/scheduled/scheduler_type.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/models/stream/log_type.py` & `corva-sdk-1.9.1/src/corva/models/stream/log_type.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/models/stream/raw.py` & `corva-sdk-1.9.1/src/corva/models/stream/raw.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/models/stream/stream.py` & `corva-sdk-1.9.1/src/corva/models/stream/stream.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/models/task.py` & `corva-sdk-1.9.1/src/corva/models/task.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/service/api_sdk.py` & `corva-sdk-1.9.1/src/corva/service/api_sdk.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/service/cache_sdk.py` & `corva-sdk-1.9.1/src/corva/service/cache_sdk.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/service/service.py` & `corva-sdk-1.9.1/src/corva/service/service.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva/testing.py` & `corva-sdk-1.9.1/src/corva/testing.py`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/corva_sdk.egg-info/PKG-INFO` & `corva-sdk-1.9.1/src/corva_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corva-sdk
-Version: 1.9.0
+Version: 1.9.1
 Summary: SDK for building Corva DevCenter Python apps.
 Home-page: https://github.com/corva-ai/python-sdk
 Author: Jordan Ambra
 Author-email: jordan.ambra@corva.ai
 License: The Unlicense
 Keywords: corva,sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,14 +44,20 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [1.9.1] - 2023-05-09
+
+### Fixed
+- `urllib3` v2 not supported by AWS Lambda.
+
+
 ## [1.9.0] - 2023-03-06
 
 ### Added
 - `log_identifier` field to stream depth events.
 
 ### Changed
 - Reraise exceptions in `task` apps
@@ -366,15 +372,16 @@
 - `ScheduledApp` to build scheduled apps.
 - `TaskApp` to build task apps.
 - `Api` class to access Platform and Data Corva APIs.
 - `Cache` class to share data between app invokes.
 - Event classes: `StreamEvent`, `ScheduledEvent` and `TaskEvent`.
 
 
-[Unreleased] https://github.com/corva-ai/python-sdk/compare/v1.9.0...master
+[Unreleased] https://github.com/corva-ai/python-sdk/compare/v1.9.1...master
+[1.9.1] https://github.com/corva-ai/python-sdk/compare/v1.9.0...v1.9.1
 [1.9.0] https://github.com/corva-ai/python-sdk/compare/v1.8.1...v1.9.0
 [1.8.1] https://github.com/corva-ai/python-sdk/compare/v1.8.0...v1.8.1
 [1.8.0] https://github.com/corva-ai/python-sdk/compare/v1.7.0...v1.8.0
 [1.7.0] https://github.com/corva-ai/python-sdk/compare/v1.6.0...v1.7.0
 [1.6.0] https://github.com/corva-ai/python-sdk/compare/v1.5.3...v1.6.0
 [1.5.3] https://github.com/corva-ai/python-sdk/compare/v1.5.2...v1.5.3
 [1.5.2] https://github.com/corva-ai/python-sdk/compare/v1.5.1...v1.5.2
```

### Comparing `corva-sdk-1.9.0/src/corva_sdk.egg-info/SOURCES.txt` & `corva-sdk-1.9.1/src/corva_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `corva-sdk-1.9.0/src/plugin.py` & `corva-sdk-1.9.1/src/plugin.py`

 * *Files identical despite different names*

