# Comparing `tmp/basic_math_operations-1.0.159.tar.gz` & `tmp/basic_math_operations-1.0.160.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_math_operations-1.0.159.tar", last modified: Mon May  8 20:23:12 2023, max compression
+gzip compressed data, was "basic_math_operations-1.0.160.tar", last modified: Tue May  9 15:09:42 2023, max compression
```

## Comparing `basic_math_operations-1.0.159.tar` & `basic_math_operations-1.0.160.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:23:12.782687 basic_math_operations-1.0.159/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 20:22:53.000000 basic_math_operations-1.0.159/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-08 20:23:12.782687 basic_math_operations-1.0.159/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-08 20:22:53.000000 basic_math_operations-1.0.159/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:23:12.778687 basic_math_operations-1.0.159/basic_math_operations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-08 20:23:12.000000 basic_math_operations-1.0.159/basic_math_operations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-08 20:23:12.000000 basic_math_operations-1.0.159/basic_math_operations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:23:12.000000 basic_math_operations-1.0.159/basic_math_operations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 20:23:12.000000 basic_math_operations-1.0.159/basic_math_operations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:23:12.782687 basic_math_operations-1.0.159/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-08 20:22:53.000000 basic_math_operations-1.0.159/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:23:12.774687 basic_math_operations-1.0.159/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:23:12.782687 basic_math_operations-1.0.159/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)    75064 2023-05-08 20:23:12.000000 basic_math_operations-1.0.159/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-08 20:22:53.000000 basic_math_operations-1.0.159/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 20:23:12.000000 basic_math_operations-1.0.159/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:09:42.078750 basic_math_operations-1.0.160/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 15:09:07.000000 basic_math_operations-1.0.160/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-09 15:09:42.078750 basic_math_operations-1.0.160/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-09 15:09:07.000000 basic_math_operations-1.0.160/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:09:42.078750 basic_math_operations-1.0.160/basic_math_operations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-09 15:09:41.000000 basic_math_operations-1.0.160/basic_math_operations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-09 15:09:42.000000 basic_math_operations-1.0.160/basic_math_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:09:41.000000 basic_math_operations-1.0.160/basic_math_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-09 15:09:41.000000 basic_math_operations-1.0.160/basic_math_operations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 15:09:42.078750 basic_math_operations-1.0.160/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-09 15:09:07.000000 basic_math_operations-1.0.160/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:09:42.078750 basic_math_operations-1.0.160/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:09:42.078750 basic_math_operations-1.0.160/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)    75064 2023-05-09 15:09:41.000000 basic_math_operations-1.0.160/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-09 15:09:07.000000 basic_math_operations-1.0.160/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 15:09:41.000000 basic_math_operations-1.0.160/src/python-module/version.txt
```

### Comparing `basic_math_operations-1.0.159/LICENSE` & `basic_math_operations-1.0.160/LICENSE`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.159/README.md` & `basic_math_operations-1.0.160/README.md`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.159/setup.py` & `basic_math_operations-1.0.160/setup.py`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.159/src/python-module/libbasic_math_operations.a` & `basic_math_operations-1.0.160/src/python-module/libbasic_math_operations.a`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.159/src/python-module/module.c` & `basic_math_operations-1.0.160/src/python-module/module.c`

 * *Files identical despite different names*

