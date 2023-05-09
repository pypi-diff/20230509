# Comparing `tmp/biocommons.example-0.0.2.tar.gz` & `tmp/biocommons.example-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biocommons.example-0.0.2.tar", last modified: Thu Feb 23 05:44:10 2023, max compression
+gzip compressed data, was "biocommons.example-0.0.3.tar", last modified: Tue May  9 03:04:26 2023, max compression
```

## Comparing `biocommons.example-0.0.2.tar` & `biocommons.example-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:44:10.008484 biocommons.example-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:44:10.004484 biocommons.example-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:44:10.004484 biocommons.example-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-02-23 05:44:10.008484 biocommons.example-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:44:10.004484 biocommons.example-0.0.2/sbin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/sbin/makefile-extract-documentation
--rwxr-xr-x   0 runner    (1001) docker     (123)     1342 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/sbin/rename-package
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-02-23 05:44:10.008484 biocommons.example-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:44:10.004484 biocommons.example-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:44:10.004484 biocommons.example-0.0.2/src/biocommons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:44:10.008484 biocommons.example-0.0.2/src/biocommons/example/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/src/biocommons/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/src/biocommons/example/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/src/biocommons/example/marvin.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/src/biocommons/example/marvin_adjacent_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/src/biocommons/example/quotes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:44:10.008484 biocommons.example-0.0.2/src/biocommons/example/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/src/biocommons/example/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/src/biocommons/example/tests/marvin_subdir_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:44:10.004484 biocommons.example-0.0.2/src/biocommons.example.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-02-23 05:44:09.000000 biocommons.example-0.0.2/src/biocommons.example.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-23 05:44:10.000000 biocommons.example-0.0.2/src/biocommons.example.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 05:44:09.000000 biocommons.example-0.0.2/src/biocommons.example.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-23 05:44:09.000000 biocommons.example-0.0.2/src/biocommons.example.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-23 05:44:09.000000 biocommons.example-0.0.2/src/biocommons.example.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-23 05:44:09.000000 biocommons.example-0.0.2/src/biocommons.example.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 05:44:09.000000 biocommons.example-0.0.2/src/biocommons.example.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:44:10.008484 biocommons.example-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/tests/test_marvin.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-23 05:43:48.000000 biocommons.example-0.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:04:26.220461 biocommons.example-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:04:26.216461 biocommons.example-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:04:26.216461 biocommons.example-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-09 03:04:26.220461 biocommons.example-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:04:26.216461 biocommons.example-0.0.3/sbin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/sbin/makefile-extract-documentation
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1342 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/sbin/rename-package
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-09 03:04:26.220461 biocommons.example-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:04:26.216461 biocommons.example-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:04:26.216461 biocommons.example-0.0.3/src/biocommons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:04:26.220461 biocommons.example-0.0.3/src/biocommons/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/src/biocommons/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/src/biocommons/example/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/src/biocommons/example/marvin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/src/biocommons/example/marvin_adjacent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/src/biocommons/example/quotes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:04:26.220461 biocommons.example-0.0.3/src/biocommons/example/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/src/biocommons/example/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/src/biocommons/example/tests/marvin_subdir_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:04:26.216461 biocommons.example-0.0.3/src/biocommons.example.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-09 03:04:26.000000 biocommons.example-0.0.3/src/biocommons.example.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-09 03:04:26.000000 biocommons.example-0.0.3/src/biocommons.example.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:04:26.000000 biocommons.example-0.0.3/src/biocommons.example.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-09 03:04:26.000000 biocommons.example-0.0.3/src/biocommons.example.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-09 03:04:26.000000 biocommons.example-0.0.3/src/biocommons.example.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 03:04:26.000000 biocommons.example-0.0.3/src/biocommons.example.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:04:25.000000 biocommons.example-0.0.3/src/biocommons.example.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:04:26.220461 biocommons.example-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/tests/test_marvin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-09 03:04:09.000000 biocommons.example-0.0.3/tox.ini
```

### Comparing `biocommons.example-0.0.2/.github/workflows/python-package.yml` & `biocommons.example-0.0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `biocommons.example-0.0.2/Makefile` & `biocommons.example-0.0.3/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,21 @@
 	python -m build
 
 
 ############################################################################
 #= TESTING
 # see test configuration in setup.cfg
 
+#=> cqa: execute code quality tests
+cqa:
+	flake8 src --count --select=E9,F63,F7,F82 --show-source --statistics
+	isort --profile black --check src
+	black --check src
+	bandit -ll -r src
+
 #=> test: execute tests
 #=> test-code: test code (including embedded doctests)
 #=> test-docs: test example code in docs
 .PHONY: test test-code test-docs
 test:
 	pytest
 test-code:
```

### Comparing `biocommons.example-0.0.2/pyproject.toml` & `biocommons.example-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biocommons.example-0.0.2/sbin/makefile-extract-documentation` & `biocommons.example-0.0.3/sbin/makefile-extract-documentation`

 * *Files identical despite different names*

### Comparing `biocommons.example-0.0.2/sbin/rename-package` & `biocommons.example-0.0.3/sbin/rename-package`

 * *Files identical despite different names*

### Comparing `biocommons.example-0.0.2/setup.cfg` & `biocommons.example-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `biocommons.example-0.0.2/src/biocommons/example/__main__.py` & `biocommons.example-0.0.3/src/biocommons/example/__main__.py`

 * *Files identical despite different names*

### Comparing `biocommons.example-0.0.2/src/biocommons/example/marvin.py` & `biocommons.example-0.0.3/src/biocommons/example/marvin.py`

 * *Files identical despite different names*

### Comparing `biocommons.example-0.0.2/src/biocommons/example/quotes.yaml` & `biocommons.example-0.0.3/src/biocommons/example/quotes.yaml`

 * *Files identical despite different names*

### Comparing `biocommons.example-0.0.2/src/biocommons.example.egg-info/SOURCES.txt` & `biocommons.example-0.0.3/src/biocommons.example.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 Makefile
 README.md
 pyproject.toml
 setup.cfg
 tox.ini
+.github/CODEOWNERS
 .github/workflows/python-package.yml
 sbin/makefile-extract-documentation
 sbin/rename-package
 src/biocommons.example.egg-info/PKG-INFO
 src/biocommons.example.egg-info/SOURCES.txt
 src/biocommons.example.egg-info/dependency_links.txt
 src/biocommons.example.egg-info/entry_points.txt
```

