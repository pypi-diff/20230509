# Comparing `tmp/k2hr3_osnl-1.0.2.tar.gz` & `tmp/k2hr3_osnl-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k2hr3_osnl-1.0.2.tar", last modified: Fri Jan 13 10:36:27 2023, max compression
+gzip compressed data, was "k2hr3_osnl-1.0.3.tar", last modified: Tue May  9 00:21:50 2023, max compression
```

## Comparing `k2hr3_osnl-1.0.2.tar` & `k2hr3_osnl-1.0.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 10:36:27.762941 k2hr3_osnl-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-01-13 10:36:27.762941 k2hr3_osnl-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 10:36:27.758941 k2hr3_osnl-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 10:36:27.754941 k2hr3_osnl-1.0.2/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 10:36:27.754941 k2hr3_osnl-1.0.2/docs/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 10:36:27.758941 k2hr3_osnl-1.0.2/docs/_build/html/_images/
--rw-r--r--   0 runner    (1001) docker     (123)   162483 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/docs/_build/html/_images/k2hr3_osnl_configure.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 10:36:27.758941 k2hr3_osnl-1.0.2/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-13 10:35:40.000000 k2hr3_osnl-1.0.2/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-13 10:35:40.000000 k2hr3_osnl-1.0.2/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-13 10:35:40.000000 k2hr3_osnl-1.0.2/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5151 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-13 10:36:08.000000 k2hr3_osnl-1.0.2/docs/k2hr3_osnl.rst
--rw-r--r--   0 runner    (1001) docker     (123)   162483 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/docs/k2hr3_osnl_configure.png
--rw-r--r--   0 runner    (1001) docker     (123)   174217 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/docs/k2hr3_osnl_overview.png
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-13 10:36:08.000000 k2hr3_osnl-1.0.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 10:36:27.758941 k2hr3_osnl-1.0.2/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/etc/k2hr3-osnl.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 10:36:27.758941 k2hr3_osnl-1.0.2/k2hr3_osnl/
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/k2hr3_osnl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/k2hr3_osnl/cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/k2hr3_osnl/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/k2hr3_osnl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/k2hr3_osnl/httpresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/k2hr3_osnl/useragent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 10:36:27.762941 k2hr3_osnl-1.0.2/k2hr3_osnl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-01-13 10:36:27.000000 k2hr3_osnl-1.0.2/k2hr3_osnl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-13 10:36:27.000000 k2hr3_osnl-1.0.2/k2hr3_osnl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 10:36:27.000000 k2hr3_osnl-1.0.2/k2hr3_osnl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-13 10:36:27.000000 k2hr3_osnl-1.0.2/k2hr3_osnl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 10:36:27.000000 k2hr3_osnl-1.0.2/k2hr3_osnl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-13 10:36:27.000000 k2hr3_osnl-1.0.2/k2hr3_osnl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-13 10:36:27.000000 k2hr3_osnl-1.0.2/k2hr3_osnl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-13 10:36:27.762941 k2hr3_osnl-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 10:36:27.762941 k2hr3_osnl-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/tests/k2hr3-osnl.conf_broken
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/tests/test_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/tests/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/tests/test_useragent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18017 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/tests/test_zendpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-01-13 10:34:40.000000 k2hr3_osnl-1.0.2/tests/test_zinit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:21:50.560405 k2hr3_osnl-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-05-09 00:21:50.560405 k2hr3_osnl-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:21:50.556405 k2hr3_osnl-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:21:50.552405 k2hr3_osnl-1.0.3/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:21:50.552405 k2hr3_osnl-1.0.3/docs/_build/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:21:50.556405 k2hr3_osnl-1.0.3/docs/_build/html/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   162483 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/docs/_build/html/_images/k2hr3_osnl_configure.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:21:50.556405 k2hr3_osnl-1.0.3/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-09 00:20:59.000000 k2hr3_osnl-1.0.3/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 00:20:59.000000 k2hr3_osnl-1.0.3/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 00:20:59.000000 k2hr3_osnl-1.0.3/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5151 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-09 00:21:30.000000 k2hr3_osnl-1.0.3/docs/k2hr3_osnl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   162483 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/docs/k2hr3_osnl_configure.png
+-rw-r--r--   0 runner    (1001) docker     (123)   174217 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/docs/k2hr3_osnl_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-09 00:21:30.000000 k2hr3_osnl-1.0.3/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:21:50.556405 k2hr3_osnl-1.0.3/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/etc/k2hr3-osnl.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:21:50.556405 k2hr3_osnl-1.0.3/k2hr3_osnl/
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/k2hr3_osnl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/k2hr3_osnl/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/k2hr3_osnl/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/k2hr3_osnl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/k2hr3_osnl/httpresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/k2hr3_osnl/useragent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:21:50.560405 k2hr3_osnl-1.0.3/k2hr3_osnl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-05-09 00:21:50.000000 k2hr3_osnl-1.0.3/k2hr3_osnl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-09 00:21:50.000000 k2hr3_osnl-1.0.3/k2hr3_osnl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:21:50.000000 k2hr3_osnl-1.0.3/k2hr3_osnl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 00:21:50.000000 k2hr3_osnl-1.0.3/k2hr3_osnl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:21:50.000000 k2hr3_osnl-1.0.3/k2hr3_osnl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-09 00:21:50.000000 k2hr3_osnl-1.0.3/k2hr3_osnl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 00:21:50.000000 k2hr3_osnl-1.0.3/k2hr3_osnl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-09 00:21:50.560405 k2hr3_osnl-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:21:50.560405 k2hr3_osnl-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/tests/k2hr3-osnl.conf_broken
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/tests/test_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/tests/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/tests/test_useragent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18017 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/tests/test_zendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-05-09 00:19:27.000000 k2hr3_osnl-1.0.3/tests/test_zinit.py
```

### Comparing `k2hr3_osnl-1.0.2/CONTRIBUTING.rst` & `k2hr3_osnl-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/HISTORY.rst` & `k2hr3_osnl-1.0.3/HISTORY.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+1.0.3 (2023-05-08)
+-------------------
+
+* Fixes the build errors
+* Sets the default python verison 3.9 in GitHubActions
+
 1.0.2 (2023-01-13)
 -------------------
 
 * Fixes the environment settings
 
 1.0.1 (2023-01-13)
 -------------------
```

### Comparing `k2hr3_osnl-1.0.2/LICENSE` & `k2hr3_osnl-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/PKG-INFO` & `k2hr3_osnl-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k2hr3_osnl
-Version: 1.0.2
+Version: 1.0.3
 Summary: An OpenStack notification listener for the K2HR3 role-based ACL system
 Home-page: https://github.com/yahoojapan/k2hr3_osnl
 Author: Hirotaka Wakabayashi
 Author-email: hiwakaba@yahoo-corp.jp
 License: MIT license
 Project-URL: Bugs, https://github.com/yahoojapan/k2hr3_osnl/issues
 Project-URL: Docs, https://k2hr3-osnl.readthedocs.io/en/latest/
@@ -207,14 +207,20 @@
 
 
 
 =======
 History
 =======
 
+1.0.3 (2023-05-08)
+-------------------
+
+* Fixes the build errors
+* Sets the default python verison 3.9 in GitHubActions
+
 1.0.2 (2023-01-13)
 -------------------
 
 * Fixes the environment settings
 
 1.0.1 (2023-01-13)
 -------------------
```

### Comparing `k2hr3_osnl-1.0.2/README.rst` & `k2hr3_osnl-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/docs/Makefile` & `k2hr3_osnl-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/docs/_build/html/_images/k2hr3_osnl_configure.png` & `k2hr3_osnl-1.0.3/docs/_build/html/_images/k2hr3_osnl_configure.png`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/docs/conf.py` & `k2hr3_osnl-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/docs/installation.rst` & `k2hr3_osnl-1.0.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/docs/k2hr3_osnl.rst` & `k2hr3_osnl-1.0.3/docs/k2hr3_osnl.rst`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/docs/k2hr3_osnl_configure.png` & `k2hr3_osnl-1.0.3/docs/k2hr3_osnl_configure.png`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/docs/k2hr3_osnl_overview.png` & `k2hr3_osnl-1.0.3/docs/k2hr3_osnl_overview.png`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/docs/make.bat` & `k2hr3_osnl-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/docs/usage.rst` & `k2hr3_osnl-1.0.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/etc/k2hr3-osnl.conf` & `k2hr3_osnl-1.0.3/etc/k2hr3-osnl.conf`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/k2hr3_osnl/__init__.py` & `k2hr3_osnl-1.0.3/k2hr3_osnl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     'K2hr3NotificationEndpoint',
     'K2hr3NotificationEndpointError',
     'listen',
     'main',
     'version',
 ]
 __author__ = 'Hirotaka Wakabayashi <hiwakaba@yahoo-corp.jp>'
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 
 import argparse
 import logging
 from logging.handlers import TimedRotatingFileHandler
 from logging import StreamHandler
 from pathlib import Path
 import sys
```

### Comparing `k2hr3_osnl-1.0.2/k2hr3_osnl/cfg.py` & `k2hr3_osnl-1.0.3/k2hr3_osnl/cfg.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/k2hr3_osnl/endpoint.py` & `k2hr3_osnl-1.0.3/k2hr3_osnl/endpoint.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/k2hr3_osnl/exceptions.py` & `k2hr3_osnl-1.0.3/k2hr3_osnl/exceptions.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/k2hr3_osnl/httpresponse.py` & `k2hr3_osnl-1.0.3/k2hr3_osnl/httpresponse.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/k2hr3_osnl/useragent.py` & `k2hr3_osnl-1.0.3/k2hr3_osnl/useragent.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/k2hr3_osnl.egg-info/PKG-INFO` & `k2hr3_osnl-1.0.3/k2hr3_osnl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k2hr3-osnl
-Version: 1.0.2
+Version: 1.0.3
 Summary: An OpenStack notification listener for the K2HR3 role-based ACL system
 Home-page: https://github.com/yahoojapan/k2hr3_osnl
 Author: Hirotaka Wakabayashi
 Author-email: hiwakaba@yahoo-corp.jp
 License: MIT license
 Project-URL: Bugs, https://github.com/yahoojapan/k2hr3_osnl/issues
 Project-URL: Docs, https://k2hr3-osnl.readthedocs.io/en/latest/
@@ -207,14 +207,20 @@
 
 
 
 =======
 History
 =======
 
+1.0.3 (2023-05-08)
+-------------------
+
+* Fixes the build errors
+* Sets the default python verison 3.9 in GitHubActions
+
 1.0.2 (2023-01-13)
 -------------------
 
 * Fixes the environment settings
 
 1.0.1 (2023-01-13)
 -------------------
```

### Comparing `k2hr3_osnl-1.0.2/k2hr3_osnl.egg-info/SOURCES.txt` & `k2hr3_osnl-1.0.3/k2hr3_osnl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/pyproject.toml` & `k2hr3_osnl-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/setup.py` & `k2hr3_osnl-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/tests/__init__.py` & `k2hr3_osnl-1.0.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/tests/test_cfg.py` & `k2hr3_osnl-1.0.3/tests/test_cfg.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/tests/test_useragent.py` & `k2hr3_osnl-1.0.3/tests/test_useragent.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/tests/test_useragent_response.py` & `k2hr3_osnl-1.0.3/tests/test_useragent_response.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/tests/test_zendpoint.py` & `k2hr3_osnl-1.0.3/tests/test_zendpoint.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.2/tests/test_zinit.py` & `k2hr3_osnl-1.0.3/tests/test_zinit.py`

 * *Files identical despite different names*

