# Comparing `tmp/snakemake_testing-0.0.2.tar.gz` & `tmp/snakemake_testing-0.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_testing-0.0.2.tar", max compression
+gzip compressed data, was "snakemake_testing-0.0.3rc1.tar", max compression
```

## Comparing `snakemake_testing-0.0.2.tar` & `snakemake_testing-0.0.3rc1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-05-09 19:41:30.250199 snakemake_testing-0.0.2/LICENSE
--rw-r--r--   0        0        0       95 2023-05-09 19:41:30.250199 snakemake_testing-0.0.2/README.md
--rw-r--r--   0        0        0      993 2023-05-09 19:41:43.762900 snakemake_testing-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      721 2023-05-09 19:41:30.250199 snakemake_testing-0.0.2/src/snakemake_testing/__init__.py
--rw-r--r--   0        0        0     6994 2023-05-09 19:41:30.250199 snakemake_testing-0.0.2/src/snakemake_testing/runner.py
--rw-r--r--   0        0        0       22 2023-05-09 19:41:30.250199 snakemake_testing-0.0.2/src/snakemake_testing/version.py
--rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 snakemake_testing-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 19:57:46.125331 snakemake_testing-0.0.3rc1/LICENSE
+-rw-r--r--   0        0        0       95 2023-05-09 19:57:46.125331 snakemake_testing-0.0.3rc1/README.md
+-rw-r--r--   0        0        0      998 2023-05-09 19:57:57.726030 snakemake_testing-0.0.3rc1/pyproject.toml
+-rw-r--r--   0        0        0      721 2023-05-09 19:57:46.125331 snakemake_testing-0.0.3rc1/src/snakemake_testing/__init__.py
+-rw-r--r--   0        0        0     6994 2023-05-09 19:57:46.125331 snakemake_testing-0.0.3rc1/src/snakemake_testing/runner.py
+-rw-r--r--   0        0        0       22 2023-05-09 19:57:46.125331 snakemake_testing-0.0.3rc1/src/snakemake_testing/version.py
+-rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 snakemake_testing-0.0.3rc1/PKG-INFO
```

### Comparing `snakemake_testing-0.0.2/LICENSE` & `snakemake_testing-0.0.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_testing-0.0.2/pyproject.toml` & `snakemake_testing-0.0.3rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-testing"
-version = "0.0.2"
+version = "0.0.3-rc.1"
 description = "Tools for testing Snakemake workflows"
 authors = ["Dan Foreman-Mackey <foreman.mackey@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "snakemake_testing", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `snakemake_testing-0.0.2/src/snakemake_testing/__init__.py` & `snakemake_testing-0.0.3rc1/src/snakemake_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake_testing-0.0.2/src/snakemake_testing/runner.py` & `snakemake_testing-0.0.3rc1/src/snakemake_testing/runner.py`

 * *Files identical despite different names*

### Comparing `snakemake_testing-0.0.2/PKG-INFO` & `snakemake_testing-0.0.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-testing
-Version: 0.0.2
+Version: 0.0.3rc1
 Summary: Tools for testing Snakemake workflows
 Author: Dan Foreman-Mackey
 Author-email: foreman.mackey@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

