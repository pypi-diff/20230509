# Comparing `tmp/mlflow_token-1.0.0a1.tar.gz` & `tmp/mlflow_token-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_token-1.0.0a1.tar", max compression
+gzip compressed data, was "mlflow_token-1.1.0.tar", max compression
```

## Comparing `mlflow_token-1.0.0a1.tar` & `mlflow_token-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1491 2023-02-17 13:57:46.444835 mlflow_token-1.0.0a1/LICENSE
--rw-r--r--   0        0        0      471 2023-02-17 16:58:55.350515 mlflow_token-1.0.0a1/README.md
--rw-r--r--   0        0        0        0 2023-02-17 15:54:09.550488 mlflow_token-1.0.0a1/mlflow_token/__init__.py
--rw-r--r--   0        0        0     1855 2023-02-17 16:56:58.974861 mlflow_token-1.0.0a1/mlflow_token/mlflow_token.py
--rw-r--r--   0        0        0      549 2023-02-17 17:00:35.388127 mlflow_token-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 mlflow_token-1.0.0a1/setup.py
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 mlflow_token-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-02-17 13:57:46.444835 mlflow_token-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1017 2023-05-09 02:07:09.423735 mlflow_token-1.1.0/README.md
+-rw-r--r--   0        0        0       52 2023-05-09 02:07:09.424607 mlflow_token-1.1.0/mlflow_token/__init__.py
+-rw-r--r--   0        0        0     2959 2023-05-09 02:07:09.425291 mlflow_token-1.1.0/mlflow_token/mlflow_token.py
+-rw-r--r--   0        0        0      541 2023-05-09 02:07:09.426885 mlflow_token-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 mlflow_token-1.1.0/setup.py
+-rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 mlflow_token-1.1.0/PKG-INFO
```

### Comparing `mlflow_token-1.0.0a1/LICENSE` & `mlflow_token-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlflow_token-1.0.0a1/pyproject.toml` & `mlflow_token-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlflow-token"
-version = "1.0.0-alpha.1"
+version = "1.1.0"
 description = "Command line tool to retreive access token for mlflow instance"
 authors = ["Ben Galewsky <bengal1@illinois.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/ncsa/mlflow-token"
 packages = [{include = "mlflow_token"}]
```

