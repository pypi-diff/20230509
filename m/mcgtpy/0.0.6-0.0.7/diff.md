# Comparing `tmp/mcgtpy-0.0.6.tar.gz` & `tmp/mcgtpy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcgtpy-0.0.6.tar", last modified: Fri May  5 22:07:37 2023, max compression
+gzip compressed data, was "mcgtpy-0.0.7.tar", last modified: Tue May  9 21:09:21 2023, max compression
```

## Comparing `mcgtpy-0.0.6.tar` & `mcgtpy-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 22:07:37.413311 mcgtpy-0.0.6/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 22:07:37.413311 mcgtpy-0.0.6/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-05 22:07:36.000000 mcgtpy-0.0.6/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 22:07:37.409311 mcgtpy-0.0.6/mcgtpy/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2023-05-05 22:07:36.000000 mcgtpy-0.0.6/mcgtpy/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-05 22:07:36.000000 mcgtpy-0.0.6/mcgtpy/database.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1262 2023-05-05 22:07:36.000000 mcgtpy-0.0.6/mcgtpy/helper_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1545 2023-05-05 22:07:36.000000 mcgtpy-0.0.6/mcgtpy/my_stats.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 22:07:37.413311 mcgtpy-0.0.6/mcgtpy.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 22:07:37.000000 mcgtpy-0.0.6/mcgtpy.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      251 2023-05-05 22:07:37.000000 mcgtpy-0.0.6/mcgtpy.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 22:07:37.000000 mcgtpy-0.0.6/mcgtpy.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-05-05 22:07:37.000000 mcgtpy-0.0.6/mcgtpy.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2023-05-05 22:07:37.000000 mcgtpy-0.0.6/mcgtpy.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-05 22:07:37.413311 mcgtpy-0.0.6/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2023-05-05 22:07:36.000000 mcgtpy-0.0.6/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 21:09:21.215692 mcgtpy-0.0.7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-09 21:09:21.215692 mcgtpy-0.0.7/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-05-09 21:09:20.000000 mcgtpy-0.0.7/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 21:09:21.215692 mcgtpy-0.0.7/mcgtpy/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2023-05-09 21:09:20.000000 mcgtpy-0.0.7/mcgtpy/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2023-05-09 21:09:20.000000 mcgtpy-0.0.7/mcgtpy/database.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1207 2023-05-09 21:09:20.000000 mcgtpy-0.0.7/mcgtpy/helper_functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1545 2023-05-09 21:09:20.000000 mcgtpy-0.0.7/mcgtpy/my_stats.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 21:09:21.215692 mcgtpy-0.0.7/mcgtpy.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-09 21:09:21.000000 mcgtpy-0.0.7/mcgtpy.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      251 2023-05-09 21:09:21.000000 mcgtpy-0.0.7/mcgtpy.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-09 21:09:21.000000 mcgtpy-0.0.7/mcgtpy.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-05-09 21:09:21.000000 mcgtpy-0.0.7/mcgtpy.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2023-05-09 21:09:21.000000 mcgtpy-0.0.7/mcgtpy.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-09 21:09:21.215692 mcgtpy-0.0.7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2023-05-09 21:09:20.000000 mcgtpy-0.0.7/setup.py
```

### Comparing `mcgtpy-0.0.6/mcgtpy/my_stats.py` & `mcgtpy-0.0.7/mcgtpy/my_stats.py`

 * *Files identical despite different names*

### Comparing `mcgtpy-0.0.6/setup.py` & `mcgtpy-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'My first Python Package!'
 LONG_DESCRIPTION = 'This package will have everything I use on a daily basis to make life easier when coding in Python.'
 
 author_name = "Myles Thomas"
 author_email = "mylescgthomas@gmail.com"
 
 setup(
```

