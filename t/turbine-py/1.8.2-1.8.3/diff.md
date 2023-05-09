# Comparing `tmp/turbine-py-1.8.2.tar.gz` & `tmp/turbine-py-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbine-py-1.8.2.tar", last modified: Mon May  8 20:24:54 2023, max compression
+gzip compressed data, was "turbine-py-1.8.3.tar", last modified: Tue May  9 16:47:05 2023, max compression
```

## Comparing `turbine-py-1.8.2.tar` & `turbine-py-1.8.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.303597 turbine-py-1.8.2/
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-08 20:24:42.000000 turbine-py-1.8.2/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      161 2023-05-08 20:24:42.000000 turbine-py-1.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8663 2023-05-08 20:24:54.303597 turbine-py-1.8.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8098 2023-05-08 20:24:42.000000 turbine-py-1.8.2/README.md
--rw-r--r--   0 root         (0) root         (0)      315 2023-05-08 20:24:42.000000 turbine-py-1.8.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1148 2023-05-08 20:24:54.303597 turbine-py-1.8.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.291597 turbine-py-1.8.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.291597 turbine-py-1.8.2/src/turbine/
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-08 20:24:43.000000 turbine-py-1.8.2/src/turbine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.295597 turbine-py-1.8.2/src/turbine/function_deploy/
--rw-r--r--   0 root         (0) root         (0)      548 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/function_deploy/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/function_deploy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.295597 turbine-py-1.8.2/src/turbine/function_deploy/data_app/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/function_deploy/data_app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.295597 turbine-py-1.8.2/src/turbine/function_deploy/function_app/
--rw-r--r--   0 root         (0) root         (0)     2460 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/function_deploy/function_app/README.md
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/function_deploy/function_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3142 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/function_deploy/function_app/function_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.295597 turbine-py-1.8.2/src/turbine/function_deploy/function_app/protos/
--rw-r--r--   0 root         (0) root         (0)      406 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/function_deploy/function_app/protos/service.proto
--rw-r--r--   0 root         (0) root         (0)     1023 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/function_deploy/function_app/record.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/function_deploy/function_app/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2895 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/function_deploy/function_app/service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2498 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/function_deploy/function_app/service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.295597 turbine-py-1.8.2/src/turbine/runner/
--rw-r--r--   0 root         (0) root         (0)      153 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/runner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/runner/app_generate.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/runner/baserunner.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/runner/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.299597 turbine-py-1.8.2/src/turbine/runtime/
--rw-r--r--   0 root         (0) root         (0)      780 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/runtime/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1835 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/runtime/info.py
--rw-r--r--   0 root         (0) root         (0)     3924 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/runtime/intermediate.py
--rw-r--r--   0 root         (0) root         (0)     2865 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/runtime/local.py
--rw-r--r--   0 root         (0) root         (0)    11804 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/runtime/platform.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/runtime/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.291597 turbine-py-1.8.2/src/turbine/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.299597 turbine-py-1.8.2/src/turbine/templates/python/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/templates/python/.gitignore
--rw-r--r--   0 root         (0) root         (0)     6438 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/templates/python/README.md
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/templates/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/templates/python/app.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.299597 turbine-py-1.8.2/src/turbine/templates/python/fixtures/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/templates/python/fixtures/.gitkeep
--rw-r--r--   0 root         (0) root         (0)     8360 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/templates/python/fixtures/demo-cdc.json
--rw-r--r--   0 root         (0) root         (0)     4691 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/templates/python/fixtures/demo-no-cdc.json
--rw-r--r--   0 root         (0) root         (0)     3128 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/templates/python/main.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-08 20:24:42.000000 turbine-py-1.8.2/src/turbine/templates/python/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.303597 turbine-py-1.8.2/src/turbine_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8663 2023-05-08 20:24:54.000000 turbine-py-1.8.2/src/turbine_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1637 2023-05-08 20:24:54.000000 turbine-py-1.8.2/src/turbine_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 20:24:54.000000 turbine-py-1.8.2/src/turbine_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-08 20:24:54.000000 turbine-py-1.8.2/src/turbine_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-08 20:24:54.000000 turbine-py-1.8.2/src/turbine_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-08 20:24:54.000000 turbine-py-1.8.2/src/turbine_py.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:24:54.303597 turbine-py-1.8.2/tests/
--rw-r--r--   0 root         (0) root         (0)     3822 2023-05-08 20:24:42.000000 turbine-py-1.8.2/tests/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.668176 turbine-py-1.8.3/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-09 16:46:55.000000 turbine-py-1.8.3/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      161 2023-05-09 16:46:55.000000 turbine-py-1.8.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8663 2023-05-09 16:47:05.668176 turbine-py-1.8.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8098 2023-05-09 16:46:55.000000 turbine-py-1.8.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      315 2023-05-09 16:46:55.000000 turbine-py-1.8.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-05-09 16:47:05.668176 turbine-py-1.8.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.660176 turbine-py-1.8.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.660176 turbine-py-1.8.3/src/turbine/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.660176 turbine-py-1.8.3/src/turbine/function_deploy/
+-rw-r--r--   0 root         (0) root         (0)      548 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.660176 turbine-py-1.8.3/src/turbine/function_deploy/data_app/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/data_app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.664176 turbine-py-1.8.3/src/turbine/function_deploy/function_app/
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/README.md
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/function_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.664176 turbine-py-1.8.3/src/turbine/function_deploy/function_app/protos/
+-rw-r--r--   0 root         (0) root         (0)      406 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/protos/service.proto
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/record.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2895 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.664176 turbine-py-1.8.3/src/turbine/runner/
+-rw-r--r--   0 root         (0) root         (0)      153 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runner/app_generate.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runner/baserunner.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runner/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.664176 turbine-py-1.8.3/src/turbine/runtime/
+-rw-r--r--   0 root         (0) root         (0)      780 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runtime/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runtime/info.py
+-rw-r--r--   0 root         (0) root         (0)     3924 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runtime/intermediate.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runtime/local.py
+-rw-r--r--   0 root         (0) root         (0)    11804 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runtime/platform.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runtime/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.656176 turbine-py-1.8.3/src/turbine/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.664176 turbine-py-1.8.3/src/turbine/templates/python/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     6438 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/README.md
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/app.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.668176 turbine-py-1.8.3/src/turbine/templates/python/fixtures/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/fixtures/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)     8360 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/fixtures/demo-cdc.json
+-rw-r--r--   0 root         (0) root         (0)     4691 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/fixtures/demo-no-cdc.json
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/main.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.668176 turbine-py-1.8.3/src/turbine_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8663 2023-05-09 16:47:05.000000 turbine-py-1.8.3/src/turbine_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-05-09 16:47:05.000000 turbine-py-1.8.3/src/turbine_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 16:47:05.000000 turbine-py-1.8.3/src/turbine_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-09 16:47:05.000000 turbine-py-1.8.3/src/turbine_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-09 16:47:05.000000 turbine-py-1.8.3/src/turbine_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-09 16:47:05.000000 turbine-py-1.8.3/src/turbine_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.668176 turbine-py-1.8.3/tests/
+-rw-r--r--   0 root         (0) root         (0)     3822 2023-05-09 16:46:55.000000 turbine-py-1.8.3/tests/test_cli.py
```

### Comparing `turbine-py-1.8.2/PKG-INFO` & `turbine-py-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbine-py
-Version: 1.8.2
+Version: 1.8.3
 Summary: Meroxa Turbine data application framework
 Home-page: https://meroxa.io/
 Author: Eric Cheatham
 Author-email: eric@meroxa.io
 License: MIT
 Project-URL: Source Code, https://github.com/meroxa/turbine-py/
 Project-URL: Issue Tracker, https://github.com/meroxa/turbine-py/issues
```

### Comparing `turbine-py-1.8.2/README.md` & `turbine-py-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/setup.cfg` & `turbine-py-1.8.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/cli.py` & `turbine-py-1.8.3/src/turbine/cli.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/function_deploy/Dockerfile` & `turbine-py-1.8.3/src/turbine/function_deploy/Dockerfile`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/function_deploy/function_app/README.md` & `turbine-py-1.8.3/src/turbine/function_deploy/function_app/README.md`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/function_deploy/function_app/function_server.py` & `turbine-py-1.8.3/src/turbine/function_deploy/function_app/function_server.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/function_deploy/function_app/record.py` & `turbine-py-1.8.3/src/turbine/function_deploy/function_app/record.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/function_deploy/function_app/service_pb2.py` & `turbine-py-1.8.3/src/turbine/function_deploy/function_app/service_pb2.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/function_deploy/function_app/service_pb2_grpc.py` & `turbine-py-1.8.3/src/turbine/function_deploy/function_app/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/runner/app_generate.py` & `turbine-py-1.8.3/src/turbine/runner/app_generate.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/runner/baserunner.py` & `turbine-py-1.8.3/src/turbine/runner/baserunner.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/runner/runner.py` & `turbine-py-1.8.3/src/turbine/runner/runner.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/runtime/__init__.py` & `turbine-py-1.8.3/src/turbine/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/runtime/info.py` & `turbine-py-1.8.3/src/turbine/runtime/info.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/runtime/intermediate.py` & `turbine-py-1.8.3/src/turbine/runtime/intermediate.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/runtime/local.py` & `turbine-py-1.8.3/src/turbine/runtime/local.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/runtime/platform.py` & `turbine-py-1.8.3/src/turbine/runtime/platform.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/runtime/types.py` & `turbine-py-1.8.3/src/turbine/runtime/types.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/templates/python/README.md` & `turbine-py-1.8.3/src/turbine/templates/python/README.md`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/templates/python/fixtures/demo-cdc.json` & `turbine-py-1.8.3/src/turbine/templates/python/fixtures/demo-cdc.json`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/templates/python/fixtures/demo-no-cdc.json` & `turbine-py-1.8.3/src/turbine/templates/python/fixtures/demo-no-cdc.json`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine/templates/python/main.py` & `turbine-py-1.8.3/src/turbine/templates/python/main.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/src/turbine_py.egg-info/PKG-INFO` & `turbine-py-1.8.3/src/turbine_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbine-py
-Version: 1.8.2
+Version: 1.8.3
 Summary: Meroxa Turbine data application framework
 Home-page: https://meroxa.io/
 Author: Eric Cheatham
 Author-email: eric@meroxa.io
 License: MIT
 Project-URL: Source Code, https://github.com/meroxa/turbine-py/
 Project-URL: Issue Tracker, https://github.com/meroxa/turbine-py/issues
```

### Comparing `turbine-py-1.8.2/src/turbine_py.egg-info/SOURCES.txt` & `turbine-py-1.8.3/src/turbine_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.2/tests/test_cli.py` & `turbine-py-1.8.3/tests/test_cli.py`

 * *Files identical despite different names*

