# Comparing `tmp/k2hr3_osnl-1.0.5.tar.gz` & `tmp/k2hr3_osnl-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k2hr3_osnl-1.0.5.tar", last modified: Tue May  9 07:12:26 2023, max compression
+gzip compressed data, was "k2hr3_osnl-1.0.6.tar", last modified: Tue May  9 09:48:17 2023, max compression
```

## Comparing `k2hr3_osnl-1.0.5.tar` & `k2hr3_osnl-1.0.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:12:26.797877 k2hr3_osnl-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-05-09 07:12:26.797877 k2hr3_osnl-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:12:26.793877 k2hr3_osnl-1.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:12:26.789877 k2hr3_osnl-1.0.5/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:12:26.789877 k2hr3_osnl-1.0.5/docs/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:12:26.793877 k2hr3_osnl-1.0.5/docs/_build/html/_images/
--rw-r--r--   0 runner    (1001) docker     (123)   162483 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/docs/_build/html/_images/k2hr3_osnl_configure.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:12:26.793877 k2hr3_osnl-1.0.5/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-09 07:11:48.000000 k2hr3_osnl-1.0.5/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 07:11:48.000000 k2hr3_osnl-1.0.5/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 07:11:48.000000 k2hr3_osnl-1.0.5/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5151 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-09 07:12:12.000000 k2hr3_osnl-1.0.5/docs/k2hr3_osnl.rst
--rw-r--r--   0 runner    (1001) docker     (123)   162483 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/docs/k2hr3_osnl_configure.png
--rw-r--r--   0 runner    (1001) docker     (123)   174217 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/docs/k2hr3_osnl_overview.png
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-09 07:12:12.000000 k2hr3_osnl-1.0.5/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:12:26.793877 k2hr3_osnl-1.0.5/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/etc/k2hr3-osnl.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:12:26.793877 k2hr3_osnl-1.0.5/k2hr3_osnl/
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/k2hr3_osnl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/k2hr3_osnl/cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/k2hr3_osnl/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/k2hr3_osnl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/k2hr3_osnl/httpresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/k2hr3_osnl/useragent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:12:26.793877 k2hr3_osnl-1.0.5/k2hr3_osnl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-05-09 07:12:26.000000 k2hr3_osnl-1.0.5/k2hr3_osnl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-09 07:12:26.000000 k2hr3_osnl-1.0.5/k2hr3_osnl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:12:26.000000 k2hr3_osnl-1.0.5/k2hr3_osnl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 07:12:26.000000 k2hr3_osnl-1.0.5/k2hr3_osnl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:12:26.000000 k2hr3_osnl-1.0.5/k2hr3_osnl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-09 07:12:26.000000 k2hr3_osnl-1.0.5/k2hr3_osnl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 07:12:26.000000 k2hr3_osnl-1.0.5/k2hr3_osnl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-09 07:12:26.797877 k2hr3_osnl-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:12:26.797877 k2hr3_osnl-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/tests/k2hr3-osnl.conf_broken
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/tests/test_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/tests/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/tests/test_useragent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18017 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/tests/test_zendpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-05-09 07:10:54.000000 k2hr3_osnl-1.0.5/tests/test_zinit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:48:17.142791 k2hr3_osnl-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-05-09 09:48:17.142791 k2hr3_osnl-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:48:17.134791 k2hr3_osnl-1.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:48:17.130791 k2hr3_osnl-1.0.6/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:48:17.130791 k2hr3_osnl-1.0.6/docs/_build/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:48:17.134791 k2hr3_osnl-1.0.6/docs/_build/html/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   162483 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/docs/_build/html/_images/k2hr3_osnl_configure.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:48:17.138791 k2hr3_osnl-1.0.6/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-09 09:47:29.000000 k2hr3_osnl-1.0.6/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 09:47:29.000000 k2hr3_osnl-1.0.6/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 09:47:29.000000 k2hr3_osnl-1.0.6/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5151 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-09 09:47:59.000000 k2hr3_osnl-1.0.6/docs/k2hr3_osnl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   162483 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/docs/k2hr3_osnl_configure.png
+-rw-r--r--   0 runner    (1001) docker     (123)   174217 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/docs/k2hr3_osnl_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-09 09:47:59.000000 k2hr3_osnl-1.0.6/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:48:17.138791 k2hr3_osnl-1.0.6/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/etc/k2hr3-osnl.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:48:17.142791 k2hr3_osnl-1.0.6/k2hr3_osnl/
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/k2hr3_osnl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/k2hr3_osnl/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/k2hr3_osnl/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/k2hr3_osnl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/k2hr3_osnl/httpresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/k2hr3_osnl/useragent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:48:17.142791 k2hr3_osnl-1.0.6/k2hr3_osnl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-05-09 09:48:17.000000 k2hr3_osnl-1.0.6/k2hr3_osnl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-09 09:48:17.000000 k2hr3_osnl-1.0.6/k2hr3_osnl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:48:17.000000 k2hr3_osnl-1.0.6/k2hr3_osnl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 09:48:17.000000 k2hr3_osnl-1.0.6/k2hr3_osnl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:48:17.000000 k2hr3_osnl-1.0.6/k2hr3_osnl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-09 09:48:17.000000 k2hr3_osnl-1.0.6/k2hr3_osnl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 09:48:17.000000 k2hr3_osnl-1.0.6/k2hr3_osnl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-09 09:48:17.146791 k2hr3_osnl-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:48:17.142791 k2hr3_osnl-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/tests/k2hr3-osnl.conf_broken
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/tests/test_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/tests/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/tests/test_useragent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18017 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/tests/test_zendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-05-09 09:46:25.000000 k2hr3_osnl-1.0.6/tests/test_zinit.py
```

### Comparing `k2hr3_osnl-1.0.5/CONTRIBUTING.rst` & `k2hr3_osnl-1.0.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/HISTORY.rst` & `k2hr3_osnl-1.0.6/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+1.0.6 (2023-05-09)
+-------------------
+
+* Fixes the release build error
+
 1.0.5 (2023-05-09)
 -------------------
 
 * Fixes the inconsistency of the default python version
 * Updates the versions of dependent packages
 
 1.0.4 (2023-05-09)
```

### Comparing `k2hr3_osnl-1.0.5/LICENSE` & `k2hr3_osnl-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/PKG-INFO` & `k2hr3_osnl-1.0.6/k2hr3_osnl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: k2hr3_osnl
-Version: 1.0.5
+Name: k2hr3-osnl
+Version: 1.0.6
 Summary: An OpenStack notification listener for the K2HR3 role-based ACL system
 Home-page: https://github.com/yahoojapan/k2hr3_osnl
 Author: Hirotaka Wakabayashi
 Author-email: hiwakaba@yahoo-corp.jp
 License: MIT license
 Project-URL: Bugs, https://github.com/yahoojapan/k2hr3_osnl/issues
 Project-URL: Docs, https://k2hr3-osnl.readthedocs.io/en/latest/
@@ -207,14 +207,19 @@
 
 
 
 =======
 History
 =======
 
+1.0.6 (2023-05-09)
+-------------------
+
+* Fixes the release build error
+
 1.0.5 (2023-05-09)
 -------------------
 
 * Fixes the inconsistency of the default python version
 * Updates the versions of dependent packages
 
 1.0.4 (2023-05-09)
```

### Comparing `k2hr3_osnl-1.0.5/README.rst` & `k2hr3_osnl-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/docs/Makefile` & `k2hr3_osnl-1.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/docs/_build/html/_images/k2hr3_osnl_configure.png` & `k2hr3_osnl-1.0.6/docs/_build/html/_images/k2hr3_osnl_configure.png`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/docs/conf.py` & `k2hr3_osnl-1.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/docs/installation.rst` & `k2hr3_osnl-1.0.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/docs/k2hr3_osnl.rst` & `k2hr3_osnl-1.0.6/docs/k2hr3_osnl.rst`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/docs/k2hr3_osnl_configure.png` & `k2hr3_osnl-1.0.6/docs/k2hr3_osnl_configure.png`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/docs/k2hr3_osnl_overview.png` & `k2hr3_osnl-1.0.6/docs/k2hr3_osnl_overview.png`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/docs/make.bat` & `k2hr3_osnl-1.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/docs/usage.rst` & `k2hr3_osnl-1.0.6/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/etc/k2hr3-osnl.conf` & `k2hr3_osnl-1.0.6/etc/k2hr3-osnl.conf`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/k2hr3_osnl/__init__.py` & `k2hr3_osnl-1.0.6/k2hr3_osnl/__init__.py`

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
-__version__ = '1.0.5'
+__version__ = '1.0.6'
 
 import argparse
 import logging
 from logging.handlers import TimedRotatingFileHandler
 from logging import StreamHandler
 from pathlib import Path
 import sys
```

### Comparing `k2hr3_osnl-1.0.5/k2hr3_osnl/cfg.py` & `k2hr3_osnl-1.0.6/k2hr3_osnl/cfg.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/k2hr3_osnl/endpoint.py` & `k2hr3_osnl-1.0.6/k2hr3_osnl/endpoint.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/k2hr3_osnl/exceptions.py` & `k2hr3_osnl-1.0.6/k2hr3_osnl/exceptions.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/k2hr3_osnl/httpresponse.py` & `k2hr3_osnl-1.0.6/k2hr3_osnl/httpresponse.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/k2hr3_osnl/useragent.py` & `k2hr3_osnl-1.0.6/k2hr3_osnl/useragent.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/k2hr3_osnl.egg-info/PKG-INFO` & `k2hr3_osnl-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: k2hr3-osnl
-Version: 1.0.5
+Name: k2hr3_osnl
+Version: 1.0.6
 Summary: An OpenStack notification listener for the K2HR3 role-based ACL system
 Home-page: https://github.com/yahoojapan/k2hr3_osnl
 Author: Hirotaka Wakabayashi
 Author-email: hiwakaba@yahoo-corp.jp
 License: MIT license
 Project-URL: Bugs, https://github.com/yahoojapan/k2hr3_osnl/issues
 Project-URL: Docs, https://k2hr3-osnl.readthedocs.io/en/latest/
@@ -207,14 +207,19 @@
 
 
 
 =======
 History
 =======
 
+1.0.6 (2023-05-09)
+-------------------
+
+* Fixes the release build error
+
 1.0.5 (2023-05-09)
 -------------------
 
 * Fixes the inconsistency of the default python version
 * Updates the versions of dependent packages
 
 1.0.4 (2023-05-09)
```

### Comparing `k2hr3_osnl-1.0.5/k2hr3_osnl.egg-info/SOURCES.txt` & `k2hr3_osnl-1.0.6/k2hr3_osnl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/pyproject.toml` & `k2hr3_osnl-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/setup.py` & `k2hr3_osnl-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/tests/__init__.py` & `k2hr3_osnl-1.0.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/tests/test_cfg.py` & `k2hr3_osnl-1.0.6/tests/test_cfg.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/tests/test_useragent.py` & `k2hr3_osnl-1.0.6/tests/test_useragent.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/tests/test_useragent_response.py` & `k2hr3_osnl-1.0.6/tests/test_useragent_response.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/tests/test_zendpoint.py` & `k2hr3_osnl-1.0.6/tests/test_zendpoint.py`

 * *Files identical despite different names*

### Comparing `k2hr3_osnl-1.0.5/tests/test_zinit.py` & `k2hr3_osnl-1.0.6/tests/test_zinit.py`

 * *Files identical despite different names*

