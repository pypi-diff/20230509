# Comparing `tmp/integra-0.0.1.tar.gz` & `tmp/integra-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integra-0.0.1.tar", last modified: Tue May  9 14:40:53 2023, max compression
+gzip compressed data, was "integra-0.0.2.tar", last modified: Tue May  9 14:48:59 2023, max compression
```

## Comparing `integra-0.0.1.tar` & `integra-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,13 @@
-drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 14:40:53.235842 integra-0.0.1/
--rw-rw-r--   0 pmus      (1000) pmus      (1000)     1089 2023-05-08 23:32:21.000000 integra-0.0.1/LICENSE
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      397 2023-05-09 14:40:53.235842 integra-0.0.1/PKG-INFO
--rwxrwxr-x   0 pmus      (1000) pmus      (1000)      533 2023-05-08 23:12:48.000000 integra-0.0.1/pyproject.toml
--rw-rw-r--   0 pmus      (1000) pmus      (1000)       38 2023-05-09 14:40:53.235842 integra-0.0.1/setup.cfg
-drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 14:40:53.235842 integra-0.0.1/src/
--rwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-08 23:12:48.000000 integra-0.0.1/src/__init__.py
-drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 14:40:53.235842 integra-0.0.1/src/integra.egg-info/
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      397 2023-05-09 14:40:53.000000 integra-0.0.1/src/integra.egg-info/PKG-INFO
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      399 2023-05-09 14:40:53.000000 integra-0.0.1/src/integra.egg-info/SOURCES.txt
--rw-rw-r--   0 pmus      (1000) pmus      (1000)        1 2023-05-09 14:40:53.000000 integra-0.0.1/src/integra.egg-info/dependency_links.txt
--rw-rw-r--   0 pmus      (1000) pmus      (1000)       39 2023-05-09 14:40:53.000000 integra-0.0.1/src/integra.egg-info/top_level.txt
--rwxrwxr-x   0 pmus      (1000) pmus      (1000)     9198 2023-05-09 13:07:47.000000 integra-0.0.1/src/integra.py
-drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 14:40:53.235842 integra-0.0.1/src/old_tests/
--rw-rw-r--   0 pmus      (1000) pmus      (1000)     1163 2023-05-09 09:20:30.000000 integra-0.0.1/src/old_tests/bench_hard.py
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      554 2023-05-09 09:20:30.000000 integra-0.0.1/src/old_tests/test_error.py
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      547 2023-05-09 09:20:30.000000 integra-0.0.1/src/old_tests/test_timeout.py
-drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 14:40:53.235842 integra-0.0.1/src/tests/
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      823 2023-05-09 10:10:03.000000 integra-0.0.1/src/tests/bench-recv.py
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      845 2023-05-09 10:10:03.000000 integra-0.0.1/src/tests/infinite-recv.py
--rwxrwxr-x   0 pmus      (1000) pmus      (1000)      485 2023-05-08 23:12:48.000000 integra-0.0.1/src/tests/receive.py
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      886 2023-05-09 10:10:03.000000 integra-0.0.1/src/tests/serve-localhost.py
--rwxrwxr-x   0 pmus      (1000) pmus      (1000)      857 2023-05-09 12:47:09.000000 integra-0.0.1/src/tests/serve.py
+drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 14:48:59.400924 integra-0.0.2/
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)     1089 2023-05-08 23:32:21.000000 integra-0.0.2/LICENSE
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)      405 2023-05-09 14:48:59.400924 integra-0.0.2/PKG-INFO
+-rwxrwxr-x   0 pmus      (1000) pmus      (1000)      541 2023-05-09 14:48:39.000000 integra-0.0.2/pyproject.toml
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)       38 2023-05-09 14:48:59.400924 integra-0.0.2/setup.cfg
+drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 14:48:59.400924 integra-0.0.2/src/
+-rwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-08 23:12:48.000000 integra-0.0.2/src/__init__.py
+drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 14:48:59.400924 integra-0.0.2/src/integra.egg-info/
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)      405 2023-05-09 14:48:59.000000 integra-0.0.2/src/integra.egg-info/PKG-INFO
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)      193 2023-05-09 14:48:59.000000 integra-0.0.2/src/integra.egg-info/SOURCES.txt
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)        1 2023-05-09 14:48:59.000000 integra-0.0.2/src/integra.egg-info/dependency_links.txt
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)       17 2023-05-09 14:48:59.000000 integra-0.0.2/src/integra.egg-info/top_level.txt
+-rwxrwxr-x   0 pmus      (1000) pmus      (1000)     9198 2023-05-09 13:07:47.000000 integra-0.0.2/src/integra.py
```

### Comparing `integra-0.0.1/LICENSE` & `integra-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `integra-0.0.1/pyproject.toml` & `integra-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0", "loguru==0.7.0", "pyzmq==25.0.2", "zeroconf==0.62.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "integra"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="pmus", email="pmus.me@yandex.ru" },
 ]
 description = "ZeroMQ Zeroconf RPC"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/pmus"
+"Homepage" = "https://github.com/pmus/integra"
```

### Comparing `integra-0.0.1/src/integra.py` & `integra-0.0.2/src/integra.py`

 * *Files identical despite different names*

