# Comparing `tmp/pycompete-0.0.4.tar.gz` & `tmp/pycompete-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompete-0.0.4.tar", last modified: Fri May  5 12:18:58 2023, max compression
+gzip compressed data, was "pycompete-0.0.5.tar", last modified: Tue May  9 08:37:50 2023, max compression
```

## Comparing `pycompete-0.0.4.tar` & `pycompete-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.625822 pycompete-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-05 12:18:44.000000 pycompete-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-05 12:18:44.000000 pycompete-0.0.4/.github/workflows/syntax.yml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 12:18:44.000000 pycompete-0.0.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-05 12:18:44.000000 pycompete-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-05 12:18:44.000000 pycompete-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-05 12:18:44.000000 pycompete-0.0.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-05 12:18:58.629822 pycompete-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-05 12:18:44.000000 pycompete-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-05 12:18:44.000000 pycompete-0.0.4/notebooks/Untitled.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/pycompete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:44.000000 pycompete-0.0.4/pycompete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 12:18:58.000000 pycompete-0.0.4/pycompete/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/pycompete/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-05 12:18:44.000000 pycompete-0.0.4/pycompete/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/pycompete/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-05 12:18:44.000000 pycompete-0.0.4/pycompete/model_selection/cv_splitters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/pycompete.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-05 12:18:58.000000 pycompete-0.0.4/pycompete.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-05 12:18:58.000000 pycompete-0.0.4/pycompete.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:18:58.000000 pycompete-0.0.4/pycompete.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 12:18:58.000000 pycompete-0.0.4/pycompete.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 12:18:58.000000 pycompete-0.0.4/pycompete.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-05 12:18:44.000000 pycompete-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 12:18:44.000000 pycompete-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:18:58.629822 pycompete-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:18:44.000000 pycompete-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.625822 pycompete-0.0.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.625822 pycompete-0.0.4/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/tests/unit/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-05 12:18:44.000000 pycompete-0.0.4/tests/unit/evaluation/test_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.101942 pycompete-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 08:37:37.000000 pycompete-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-09 08:37:37.000000 pycompete-0.0.5/.github/workflows/syntax.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-09 08:37:37.000000 pycompete-0.0.5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-09 08:37:37.000000 pycompete-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-09 08:37:37.000000 pycompete-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 08:37:37.000000 pycompete-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-09 08:37:37.000000 pycompete-0.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-09 08:37:50.101942 pycompete-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-09 08:37:37.000000 pycompete-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-09 08:37:37.000000 pycompete-0.0.5/notebooks/Untitled.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/pycompete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:37.000000 pycompete-0.0.5/pycompete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 08:37:49.000000 pycompete-0.0.5/pycompete/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.101942 pycompete-0.0.5/pycompete/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-09 08:37:37.000000 pycompete-0.0.5/pycompete/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.101942 pycompete-0.0.5/pycompete/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-09 08:37:37.000000 pycompete-0.0.5/pycompete/features/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.101942 pycompete-0.0.5/pycompete/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-09 08:37:37.000000 pycompete-0.0.5/pycompete/model_selection/cv_splitters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/pycompete.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-09 08:37:50.000000 pycompete-0.0.5/pycompete.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-09 08:37:50.000000 pycompete-0.0.5/pycompete.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 08:37:50.000000 pycompete-0.0.5/pycompete.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 08:37:50.000000 pycompete-0.0.5/pycompete.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 08:37:50.000000 pycompete-0.0.5/pycompete.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-09 08:37:37.000000 pycompete-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 08:37:37.000000 pycompete-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 08:37:50.101942 pycompete-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 08:37:37.000000 pycompete-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.101942 pycompete-0.0.5/tests/unit/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-09 08:37:37.000000 pycompete-0.0.5/tests/unit/evaluation/test_metric.py
```

### Comparing `pycompete-0.0.4/.github/workflows/tests.yml` & `pycompete-0.0.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.4/.gitignore` & `pycompete-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.4/LICENSE.txt` & `pycompete-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.4/PKG-INFO` & `pycompete-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,21 @@
-Metadata-Version: 2.1
-Name: pycompete
-Version: 0.0.4
-Summary: Tools to support the training and evalaution of models for the CrunchDAO project.
-Author: Francis P Chmiel
-License: MIT license
-Keywords: crunchdao
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # pycompete
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)![GitHub](https://img.shields.io/github/license/FChmiel/pycompete)
 
 pycompete provides tools to support the training and evaluation of models for the [CrunchDAO competition](https://www.crunchdao.com/).
 
+## Installing pycompete
+
+`pip install pycompete`
+
 ## Interacting with the CrunchDAO tournament
 
 We recommend using the open-source [CrunchDAO Python](https://github.com/uuazed/crunchdao/tree/main) API for pulling data and submitting predictions.
 
 To interact with the API, you need set your API key as the `CRUNCH_API_KEY` environment variable:
 
 `export CRUNCH_API_KEY = YOUR_API_KEY`
 
 ## Contributing
 
-Contributions are welcome.
+Contributions are welcome! Please feel free to raise a PR adding any functionality you think may be useful to other CrunchDAO competitors. If you find a bug please raise an issue and we will try and address.
```

### Comparing `pycompete-0.0.4/notebooks/Untitled.ipynb` & `pycompete-0.0.5/notebooks/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.4/pycompete/evaluation/metrics.py` & `pycompete-0.0.5/pycompete/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.4/pycompete/model_selection/cv_splitters.py` & `pycompete-0.0.5/pycompete/model_selection/cv_splitters.py`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.4/pycompete.egg-info/SOURCES.txt` & `pycompete-0.0.5/pycompete.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+CONTRIBUTING.md
 LICENSE.txt
 Makefile
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 .github/workflows/publish.yml
@@ -13,9 +14,10 @@
 pycompete/_version.py
 pycompete.egg-info/PKG-INFO
 pycompete.egg-info/SOURCES.txt
 pycompete.egg-info/dependency_links.txt
 pycompete.egg-info/requires.txt
 pycompete.egg-info/top_level.txt
 pycompete/evaluation/metrics.py
+pycompete/features/transformers.py
 pycompete/model_selection/cv_splitters.py
 tests/unit/evaluation/test_metric.py
```

### Comparing `pycompete-0.0.4/pyproject.toml` & `pycompete-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.4/tests/unit/evaluation/test_metric.py` & `pycompete-0.0.5/tests/unit/evaluation/test_metric.py`

 * *Files identical despite different names*

