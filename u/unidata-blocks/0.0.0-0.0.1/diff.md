# Comparing `tmp/unidata-blocks-0.0.0.tar.gz` & `tmp/unidata-blocks-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unidata-blocks-0.0.0.tar", last modified: Mon May  8 17:35:45 2023, max compression
+gzip compressed data, was "unidata-blocks-0.0.1.tar", last modified: Tue May  9 10:56:51 2023, max compression
```

## Comparing `unidata-blocks-0.0.0.tar` & `unidata-blocks-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:35:45.048596 unidata-blocks-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 17:35:33.000000 unidata-blocks-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-08 17:35:45.048596 unidata-blocks-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 17:35:33.000000 unidata-blocks-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-08 17:35:33.000000 unidata-blocks-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 17:35:45.048596 unidata-blocks-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:35:45.048596 unidata-blocks-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:35:45.048596 unidata-blocks-0.0.0/src/unidata_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:35:33.000000 unidata-blocks-0.0.0/src/unidata_blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:35:45.048596 unidata-blocks-0.0.0/src/unidata_blocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-08 17:35:45.000000 unidata-blocks-0.0.0/src/unidata_blocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-08 17:35:45.000000 unidata-blocks-0.0.0/src/unidata_blocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:35:45.000000 unidata-blocks-0.0.0/src/unidata_blocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 17:35:45.000000 unidata-blocks-0.0.0/src/unidata_blocks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:35:45.048596 unidata-blocks-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 17:35:33.000000 unidata-blocks-0.0.0/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:56:51.746225 unidata-blocks-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-09 10:56:40.000000 unidata-blocks-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-09 10:56:51.746225 unidata-blocks-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-09 10:56:40.000000 unidata-blocks-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 10:56:40.000000 unidata-blocks-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:56:51.746225 unidata-blocks-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:56:51.742226 unidata-blocks-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:56:51.742226 unidata-blocks-0.0.1/src/unidata_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-09 10:56:40.000000 unidata-blocks-0.0.1/src/unidata_blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:56:51.746225 unidata-blocks-0.0.1/src/unidata_blocks/unidata/
+-rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-05-09 10:56:40.000000 unidata-blocks-0.0.1/src/unidata_blocks/unidata/Blocks.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:56:51.746225 unidata-blocks-0.0.1/src/unidata_blocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-09 10:56:51.000000 unidata-blocks-0.0.1/src/unidata_blocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-09 10:56:51.000000 unidata-blocks-0.0.1/src/unidata_blocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:56:51.000000 unidata-blocks-0.0.1/src/unidata_blocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 10:56:51.000000 unidata-blocks-0.0.1/src/unidata_blocks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:56:51.746225 unidata-blocks-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-09 10:56:40.000000 unidata-blocks-0.0.1/tests/test_query.py
```

### Comparing `unidata-blocks-0.0.0/LICENSE` & `unidata-blocks-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.0/pyproject.toml` & `unidata-blocks-0.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "unidata-blocks"
-version = "0.0.0"
+version = "0.0.1"
 description = "A library that helps query unicode blocks by Blocks.txt."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
@@ -19,11 +19,14 @@
 ]
 
 [project.urls]
 homepage = "https://github.com/TakWolf/unidata-blocks"
 source = "https://github.com/TakWolf/unidata-blocks"
 issues = "https://github.com/TakWolf/unidata-blocks/issues"
 
+[tool.setuptools]
+package-data = { "unidata_blocks" = ["unidata/*.txt"] }
+
 [tool.pytest.ini_options]
 pythonpath = [
     "src",
 ]
```

