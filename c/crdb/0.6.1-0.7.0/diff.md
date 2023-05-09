# Comparing `tmp/crdb-0.6.1.tar.gz` & `tmp/crdb-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crdb-0.6.1.tar", last modified: Fri May  5 09:38:57 2023, max compression
+gzip compressed data, was "crdb-0.7.0.tar", last modified: Tue May  9 09:28:48 2023, max compression
```

## Comparing `crdb-0.6.1.tar` & `crdb-0.7.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.976195 crdb-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-05 09:38:49.000000 crdb-0.6.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.972195 crdb-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.972195 crdb-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-05 09:38:49.000000 crdb-0.6.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-05 09:38:49.000000 crdb-0.6.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-05 09:38:49.000000 crdb-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-05 09:38:49.000000 crdb-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-05 09:38:49.000000 crdb-0.6.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-05 09:38:49.000000 crdb-0.6.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-05 09:38:49.000000 crdb-0.6.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-05 09:38:49.000000 crdb-0.6.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-05 09:38:49.000000 crdb-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 09:38:49.000000 crdb-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-05 09:38:57.976195 crdb-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-05 09:38:49.000000 crdb-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.976195 crdb-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/build.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-05 09:38:49.000000 crdb-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 09:38:57.976195 crdb-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.972195 crdb-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.976195 crdb-0.6.1/src/crdb/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21293 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/crdb_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/mpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/solarsystem_abundances2003.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.976195 crdb-0.6.1/src/crdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-05 09:38:57.000000 crdb-0.6.1/src/crdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-05 09:38:57.000000 crdb-0.6.1/src/crdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:38:57.000000 crdb-0.6.1/src/crdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 09:38:57.000000 crdb-0.6.1/src/crdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 09:38:57.000000 crdb-0.6.1/src/crdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 09:38:57.000000 crdb-0.6.1/src/crdb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.976195 crdb-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-05 09:38:49.000000 crdb-0.6.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-05 09:38:49.000000 crdb-0.6.1/tests/test_experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-05 09:38:49.000000 crdb-0.6.1/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 09:38:49.000000 crdb-0.6.1/tests/test_mpl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.842773 crdb-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-09 09:28:36.000000 crdb-0.7.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.834773 crdb-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.838773 crdb-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-09 09:28:36.000000 crdb-0.7.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-09 09:28:36.000000 crdb-0.7.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-09 09:28:36.000000 crdb-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-09 09:28:36.000000 crdb-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-09 09:28:36.000000 crdb-0.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-09 09:28:36.000000 crdb-0.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 09:28:36.000000 crdb-0.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-09 09:28:36.000000 crdb-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-09 09:28:36.000000 crdb-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-09 09:28:36.000000 crdb-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-09 09:28:48.842773 crdb-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-09 09:28:36.000000 crdb-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.838773 crdb-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-09 09:28:36.000000 crdb-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-09 09:28:48.842773 crdb-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.834773 crdb-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.838773 crdb-0.7.0/src/crdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21678 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/crdb_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/mpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/solarsystem_abundances2003.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.842773 crdb-0.7.0/src/crdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-09 09:28:48.000000 crdb-0.7.0/src/crdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-09 09:28:48.000000 crdb-0.7.0/src/crdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:28:48.000000 crdb-0.7.0/src/crdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 09:28:48.000000 crdb-0.7.0/src/crdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-09 09:28:48.000000 crdb-0.7.0/src/crdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 09:28:48.000000 crdb-0.7.0/src/crdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.842773 crdb-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-09 09:28:36.000000 crdb-0.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-09 09:28:36.000000 crdb-0.7.0/tests/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-09 09:28:36.000000 crdb-0.7.0/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-09 09:28:36.000000 crdb-0.7.0/tests/test_mpl.py
```

### Comparing `crdb-0.6.1/.github/workflows/publish.yml` & `crdb-0.7.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `crdb-0.6.1/.github/workflows/test.yml` & `crdb-0.7.0/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -5,37 +5,41 @@
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.head_ref }}
   cancel-in-progress: true
 
 jobs:
   test:
-    name: ${{ matrix.py }} ${{ matrix.os }} ${{ matrix.arch }}
+    name: ${{ matrix.python }} ${{ matrix.os }} ${{ matrix.arch }}
     runs-on: ${{ matrix.os }}
     timeout-minutes: 30
     strategy:
       fail-fast: false
       matrix:
         include:
-          # Broken for some reason not related to us
-          # - python: 'pypy-3.8'
-          #   python_arch: 'x64'
-          #   os: 'ubuntu-latest'
-          - python: '3.9'
-            python_arch: 'x64'
+          - python: '3.8'
+            arch: 'x64'
             os: 'windows-latest'
           - python: '3.10'
-            python_arch: 'x64'
+            arch: 'x64'
             os: 'macos-latest'
           - python: '3.11'
-            python_arch: 'x64'
+            arch: 'x64'
             os: 'ubuntu-latest'
+        # Broken for some reason not related to us
+        # - python: 'pypy-3.8'
+        #   arch: 'x64'
+        #   os: 'ubuntu-latest'
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
+    - uses: actions/cache@v3
+      with:
+        path: ~/.cachier
+        key: ${{ runner.os }}-cachier
     - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python }}
-        architecture: ${{ matrix.python_arch }}
+        architecture: ${{ matrix.arch }}
     - run: python -m pip install --progress-bar=off --prefer-binary -e .[test]
     - run: python -m pytest
```

### Comparing `crdb-0.6.1/.gitignore` & `crdb-0.7.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -66,9 +66,9 @@
 .cache
 .pytest
 .benchmarks
 .bootstrap
 .appveyor.token
 *.bak
 
-# Mypy Cache
 .mypy_cache/
+.ruff_cache/
```

### Comparing `crdb-0.6.1/CONTRIBUTING.rst` & `crdb-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `crdb-0.6.1/LICENSE` & `crdb-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crdb-0.6.1/PKG-INFO` & `crdb-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crdb
-Version: 0.6.1
+Version: 0.7.0
 Summary: CRDB Python frontend
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/crdb-project/crdb
 Project-URL: documentation, https://lpsc.in2p3.fr/crdb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `crdb-0.6.1/README.rst` & `crdb-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `crdb-0.6.1/docs/conf.py` & `crdb-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `crdb-0.6.1/pyproject.toml` & `crdb-0.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -57,25 +57,37 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools_scm]
 
 [tool.mypy]
-strict = true
-no_implicit_optional = false
-allow_redefinition = true
 ignore_missing_imports = true
-show_error_codes = true
+allow_redefinition = true
+files = ["src"]
+plugins = "numpy.typing.mypy_plugin"
+pretty = true
+no_implicit_optional = false
 
 [tool.black]
-line-length = 90
 target-version = ['py38']
 skip-string-normalization = true
 
+[tool.ruff]
+select = ["E", "F", "D"]
+extend-ignore = ["D203", "D212"]
+
+[tool.ruff.pydocstyle]
+convention = "numpy"
+
+[tool.ruff.per-file-ignores]
+"test_*.py" = ["B", "D"]
+"docs/*.py" = ["D"]
+"setup.py" = ["D"]
+
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--strict-config --strict-markers --doctest-modules -q -ra --ff --tb=short"
 testpaths = ["tests"]
 log_cli_level = "INFO"
 xfail_strict = true
 filterwarnings = [
```

### Comparing `crdb-0.6.1/src/crdb/_lib.py` & `crdb-0.7.0/src/crdb/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+"""Core library functions."""
 from __future__ import annotations
 
-import datetime
+import csv
+from datetime import datetime, timedelta
 import re
 import ssl
 import tempfile
 import urllib.request as rq
 from pathlib import Path
 from typing import Dict
 from typing import List
@@ -327,14 +329,55 @@
     "Tibet",
     "Trek",
     "UHECR-LDEF",
     "Ulysses",
     "Voyager",
 )
 
+_CSV_FIELDS = (
+    ("quantity", "U32"),  # DATA-QTY
+    ("sub_exp", "U100"),  # SUBEXP-NAME
+    ("e_type", "U4"),  # DATA-EAXIS
+    ("e", "f8"),  # DATA-E_MEAN
+    ("e_bin", "f8", (2,)),  # EBIN_LOW, EBIN_HIGH
+    ("value", "f8"),  # QUANTITY VALUE
+    ("err_sta", "f8", (2,)),  # ERR_STAT-,  ERR_STAT+
+    ("err_sys", "f8", (2,)),  # ERR_SYST-, ERR_SYST+
+    ("ads", "U32"),  # ADS URL FOR PAPER REF
+    ("phi", "f8"),  # phi [MV]
+    ("distance", "f8"),  # DISTANCE [AU]
+    ("datetime", "U256"),  # DATIMES
+    ("is_upper_limit", "?"),  # IS UPPER LIMIT
+)
+
+# fields set to None here are skipped during parsing
+_CSV_ASIMPORT_FIELDS = (
+    ("exp", "U64"),  # EXP-NAME
+    ("exp_type", "U16"),  # EXP-TYPE
+    None,  # EXP-HTML
+    None,  # EXP-STARTYEAR
+    ("sub_exp", "U100"),  # SUBEXP-NAME
+    None,  # SUBEXP-DESCRIPTION
+    ("e_relerr", "f8"),  # SUBEXP-ESCALE_RELERR
+    None,  # SUBEXP-INFO
+    ("distance", "f8"),  # SUBEXP-DISTANCE
+    ("datetime", "U256"),  # SUBEXP-DATES
+    ("ads", "U32"),  # PUBLI-HTML
+    None,  # PUBLI-DATAORIGIN
+    ("quantity", "U32"),  # DATA-QTY
+    ("e_type", "U4"),  # DATA-EAXIS
+    ("e", "f8"),  # DATA-E_MEAN
+    ("e_bin", "f8", (2,)),  # DATA-E_BIN_L, DATA-E_BIN_U
+    ("value", "f8"),  # DATA-VAL
+    ("err_sta", "f8", (2,)),  # DATA-VAL_ERRSTAT_L, DATA-VAL_ERRSTAT_U
+    ("err_sys", "f8", (2,)),  # DATA-VAL_ERRSYST_L, DATA-VAL_ERRSYST_U
+    ("is_upper_limit", "?"),  # DATA-ISUPPERLIM
+    ("phi", "f8"),  # phi [MV]
+)
+
 
 def query(
     quantity: Union[str, Sequence[str]],
     *,
     energy_type: str = "R",
     combo_level: int = 1,
     energy_convert_level: int = 1,
@@ -344,15 +387,15 @@
     energy_stop: float = 0.0,
     time_start: str = "",
     time_stop: str = "",
     time_series: str = "",
     modulation: str = "",
     timeout: int = 120,
     server_url: str = "http://lpsc.in2p3.fr/crdb",
-):
+) -> np.recarray:
     """
     Query CRDB and return table as a numpy array.
 
     See http://lpsc.in2p3.fr/crdb for documentation which parameters are accepted.
 
     Parameters
     ----------
@@ -365,16 +408,16 @@
         Energy unit for the requested quantity. Default is R.
         Valid values: EKN, EK, R, ETOT, ETOTN.
     combo_level: int, optional
         One of 0, 1, 2. Default is 1. Add combinations (ratio, products) of native data
         (from the same sub-exp at the same energy) that match quantities in list (e.g.
         compute B/C from native B and C). Three levels of combos are enabled: 0 (native
         data only, no combo), 1 (exact combos), or 2 (exact and approximate combos): in
-        level 1, the mean energy (or energy bin) of the two quantities must be within 5%,
-        whereas for level 2, it must be within 20%.
+        level 1, the mean energy (or energy bin) of the two quantities must be within
+        5%, whereas for level 2, it must be within 20%.
     energy_convert_level: int, optional
         One of 0, 1, 2. Default is 1. Add data obtained from an exact or approximate
         energy_type conversion (from native to queried). Three levels of conversion are
         enabled: 0 (native data only, no conversion), 1 (exact conversion only, which
         applies to isotopic and leptonic fluxes), and 2 (exact and approximate
         conversions, the later applying to flux of elements and of groups of elements).
     flux_rescaling: float, optional
@@ -399,32 +442,29 @@
         Timeout for server response in seconds. Default is 60.
     server_url: str, optional
         URL to send the request to. Default is http://lpsc.in2p3.fr/crdb). This is an
         expert option, users do not need to change this.
 
     Returns
     -------
-
     numpy record array with the database content
 
     Energies are in GeV or GV. Solar modulation values are in MV. Distances are in
     AU. Fluxes are in sr s m2 energy_unit.
 
     Raises
     ------
-
     ValueError
         An invalid parameter value triggers a ValueError.
 
     TimeoutError
         If the server does not respond within the timeout time.
 
     Notes
     -----
-
     This function caches identical queries for 30 days. If you need to reset the cache,
     do::
 
         from crdb import clear_cache
 
         clear_cache()
     """
@@ -444,40 +484,40 @@
                 time_series=time_series,
                 modulation=modulation,
                 server_url=server_url,
                 timeout=timeout,
             )
             for q in quantity
         ]
-        return np.concatenate(results).view(np.recarray)
+        return np.concatenate(results).view(np.recarray)  # type:ignore
 
     url = _url(
         quantity=quantity,
         energy_type=energy_type,
         combo_level=combo_level,
         energy_convert_level=energy_convert_level,
         flux_rescaling=flux_rescaling,
         exp_dates=exp_dates,
         energy_start=energy_start,
         energy_stop=energy_stop,
         time_start=time_start,
         time_stop=time_stop,
         time_series=time_series,
-        format="csv",
+        format="csv-asimport",
         modulation=modulation,
         server_url=server_url,
     )
 
     data = _server_request(url, timeout)
 
     # check for errors and display them
     if len(data) == 1:
         raise ValueError(data[0])
 
-    table = _convert(data)
+    table = _convert_csv(data, _CSV_ASIMPORT_FIELDS)
 
     return table
 
 
 def _url(
     quantity: str,
     energy_type: str = "R",
@@ -489,19 +529,16 @@
     energy_stop: float = 0.0,
     time_start: str = "",
     time_stop: str = "",
     time_series: str = "",
     format: str = "",
     modulation: str = "",
     server_url: str = "http://lpsc.in2p3.fr/crdb",
-):
-    """
-    Build a query URL for the CRDB server.
-    """
-
+) -> str:
+    """Build a query URL for the CRDB server."""
     num, *rest = quantity.split("/")
     if len(rest) > 1:
         raise ValueError("ratio contains more than one / operator")
 
     num = num.strip()
     den = rest[0].strip() if rest else ""
 
@@ -533,15 +570,15 @@
     if format and format not in ("usine", "galprop", "csv", "csv-asimport"):
         raise ValueError(f"invalid format {format}")
 
     if modulation and modulation not in ("USO05", "USO17", "GHE17"):
         raise ValueError(f"invalid modulation {modulation}")
 
     # do the query
-    kwargs = {
+    kwargs: Dict[str, Union[str, float, int]] = {
         "num": num,
         "energy_type": energy_type.upper(),
     }
     if den:
         kwargs["den"] = den
     if combo_level != 1:
         kwargs["combo_level"] = combo_level
@@ -567,22 +604,22 @@
         kwargs["modulation"] = modulation
 
     return f"{server_url}/rest.php?" + "&".join(
         ["{0}={1}".format(k, v) for (k, v) in kwargs.items()]
     )
 
 
-@cachier.cachier(stale_after=datetime.timedelta(days=30))
+@cachier.cachier(stale_after=timedelta(days=30))
 def _server_request(url: str, timeout: int) -> List[str]:
     # if there is a timeout error, we hide original long traceback from the internal
     # libs and instead show a simple traceback
     try:
         context = ssl._create_unverified_context()
         with rq.urlopen(url, timeout=timeout, context=context) as u:
-            data = u.read().decode("utf-8").split("\n")
+            data: List[str] = u.read().decode("utf-8").split("\n")
         timeout_error = False
     except TimeoutError:
         timeout_error = True
 
     if timeout_error:
         raise TimeoutError(
             f"server did not respond within timeout={timeout} to url={url}"
@@ -590,99 +627,38 @@
 
     if not data:
         raise ValueError("empty server response")
 
     return data
 
 
-def _convert(data: List[str]) -> NDArray:
+def _convert_csv(
+    data: List[str],
+    fields: Sequence[Union[None, Tuple[str, str], Tuple[str, str, Tuple[int]]]],
+) -> np.recarray:
     # convert text to numpy record array
-
-    # Use this for csv-asimport or csv-extended when it becomes available
-    # fields set to None here are skipped during parsing
-    # fields = [
-    #     ("exp", "U64"),  # EXP-NAME
-    #     ("exp_type", "U16"),  # EXP-TYPE
-    #     None,  # EXP-HTML
-    #     None,  # EXP-STARTYEAR
-    #     ("sub_exp", "U100"),  # SUBEXP-NAME
-    #     None,  # SUBEXP-DESCRIPTION
-    #     ("e_relerr", "f8"),  # SUBEXP-ESCALE_RELERR
-    #     None,  # SUBEXP-INFO
-    #     ("distance", "f8"),  # SUBEXP-DISTANCE
-    #     ("datetime", "U64"),  # SUBEXP-DATES
-    #     ("ads", "U32"),  # PUBLI-HTML
-    #     None,  # PUBLI-DATAORIGIN
-    #     ("quantity", "U32"),  # DATA-QTY
-    #     ("e_axis", "U4"),  # DATA-EAXIS
-    #     ("e_mean", "f8"),  # DATA-E_MEAN
-    #     ("e_low", "f8"),  #  DATA-E_BIN_L
-    #     ("e_high", "f8"),  # DATA-E_BIN_U
-    #     ("value", "f8"),  # DATA-VAL
-    #     ("err_stat_minus", "f8"),  # DATA-VAL_ERRSTAT_L
-    #     ("err_stat_plus", "f8"),  # DATA-VAL_ERRSTAT_U
-    #     ("err_sys_minus", "f8"),  # DATA-VAL_ERRSYST_L
-    #     ("err_sys_plus", "f8"),  # DATA-VAL_ERRSYST_U
-    #     ("is_upper_limit", "?"),  # DATA-ISUPPERLIM
-    #     # ("phi", "f8"),
-    # ]
-
-    fields = [
-        ("quantity", "U32"),  # DATA-QTY
-        ("sub_exp", "U100"),  # SUBEXP-NAME
-        ("e_type", "U4"),  # DATA-EAXIS
-        ("e", "f8"),  # DATA-E_MEAN
-        ("e_bin", "f8", (2,)),  # EBIN_LOW, EBIN_HIGH
-        ("value", "f8"),  # QUANTITY VALUE
-        ("err_sta", "f8", (2,)),  # ERR_STAT-,  ERR_STAT+
-        ("err_sys", "f8", (2,)),  # ERR_SYST-, ERR_SYST+
-        ("ads", "U32"),  # ADS URL FOR PAPER REF
-        ("phi", "f8"),  # phi [MV]
-        ("distance", "f8"),  # DISTANCE [AU]
-        ("datetime", "U256"),  # DATIMES
-        ("is_upper_limit", "?"),  # IS UPPER LIMIT
-    ]
-
-    mapping = []
+    mapping: List[Union[None, str, Tuple[str, int]]] = []
     for f in fields:
         if f is None:
             mapping.append(None)
-        if len(f) == 3:
-            for k in range(f[2][0]):
+        elif len(f) == 3:
+            (n,) = f[2]  # type:ignore
+            for k in range(n):
                 mapping.append((f[0], k))
         else:
             mapping.append(f[0])
     fields = [x for x in fields if x is not None]
 
-    # workaround for invalid CSV format,
-    # to be replaced by standard parser
-    data2 = []
-    for iline, line in enumerate(data):
-        try:
-            line = line.strip()
-            if not line or line.startswith("#"):
-                continue
-            items = []
-            inquote = False
-            start = 0
-            for i, c in enumerate(line):
-                if c == '"':
-                    if inquote:
-                        items.append(line[start + 1 : i])
-                    else:
-                        start = i
-                    inquote = not inquote
-            data2.append(items)
-        except ValueError as e:
-            msg = f"{e.args[0]}\nCould not parse line {iline} {line}"
-            e.args = (msg,)
-            raise
-
-    table = np.recarray(len(data2), fields)
-    for idx, row in enumerate(data2):
+    for start, line in enumerate(data):
+        if not line.startswith("#"):
+            break
+
+    table = np.recarray(len(data) - start - 1, fields)
+    for idx, row in enumerate(csv.reader(data[start:-1])):
+        val: Union[str, int]
         for val, key in zip(row, mapping):
             if key is None:
                 continue
             if isinstance(key, tuple):
                 key, pos = key
                 table[idx][key][pos] = val
             else:
@@ -703,16 +679,44 @@
     for x in ("sta", "sys"):
         field = f"err_{x}"
         table[field] = np.abs(table[field])
 
     return table
 
 
+def get_mean_datetime(timerange: str) -> Tuple[datetime, timedelta]:
+    """
+    Return the average time for a given time range.
+
+    Parameters
+    ----------
+    timerange : string
+        CRDB time range in "YYYY/MM/DD-HHMMSS:YYYY/MM/DD-HHMMSS" format.
+
+    Returns
+    -------
+    Datetime
+        Center of the time range.
+
+    Raises
+    ------
+    ValueError
+        Raised if the argument contains multiple time ranges.
+    """
+    if ";" in timerange:
+        raise ValueError("argument contains multiple time ranges")
+
+    s1, s2 = timerange.split(":")
+    dt1 = datetime.strptime(s1, "%Y/%m/%d-%H%M%S")
+    dt2 = datetime.strptime(s2, "%Y/%m/%d-%H%M%S")
+    return dt1 + (dt2 - dt1) / 2, (dt2 - dt1) / 2
+
+
 def experiment_masks(
-    table: NDArray, combine: Sequence[str] = COMBINE
+    table: np.recarray, combine: Sequence[str] = COMBINE
 ) -> Dict[str, NDArray]:
     """
     Generate masks which select all points from each experiment.
 
     Different data taking campains are joined. Optionally, one can also
     join different experiments with the same name, e.g. AEASOP00, AESOP02, ...
 
@@ -745,31 +749,28 @@
         if c not in result:
             result[c] = np.zeros(len(table), dtype=bool)
         result[c][i] = True
     return result
 
 
 def clear_cache() -> None:
-    """
-    Delete the local CRDB cache.
-    """
+    """Delete the local CRDB cache."""
     _server_request.clear_cache()
+    _all_request.clear_cache()
 
 
-def reference_urls(table: NDArray) -> List[str]:
-    """
-    Return list of URLs to entries in the ADSABS database for datasets in table.
-    """
+def reference_urls(table: np.recarray) -> List[str]:
+    """Return list of URLs to entries in the ADSABS database for datasets in table."""
     result = []
     for key in sorted(np.unique(table.ads)):
         result.append(f"https://ui.adsabs.harvard.edu/abs/{key}")
     return result
 
 
-def bibliography(table: NDArray) -> Dict[str, str]:
+def bibliography(table: np.recarray) -> Dict[str, str]:
     """
     Return dictionary that maps ADSABS keys in table to BibTex entries.
 
     This requires the external library `autobib`.
     """
     try:
         from autobib.util import get_entry_online
@@ -781,19 +782,17 @@
     for adskey in sorted(np.unique(table.ads)):
         k, *r = get_entry_online(adskey)
         result[k] = "".join(r)
 
     return result
 
 
-@cachier.cachier(stale_after=datetime.timedelta(days=30))
-def all() -> NDArray:
-    """
-    Return the full raw CRDB database as a table.
-    """
+@cachier.cachier(stale_after=timedelta(days=30))
+def _all_request() -> List[str]:
+    # url = "https://lpsc.in2p3.fr/crdb/_export_all_data.php?format=csv-asimport"
     url = "https://lpsc.in2p3.fr/crdb/_export_all_data.php?format=csv"
 
     try:
         context = ssl._create_unverified_context()
         response = rq.urlopen(url, context=context)
         connection_error = False
     except Exception:
@@ -821,15 +820,24 @@
                 break
             f.write(chunk.decode())
         print()
         f.flush()
         f.seek(0)
         data = f.readlines()
 
-    return _convert(data)
+    if not data:
+        raise ValueError("empty server response")
+
+    return data
+
+
+def all() -> NDArray:
+    """Return the full raw CRDB database as a table."""
+    data = _all_request()
+    return _convert_csv(data, _CSV_FIELDS)
 
 
 def solar_system_composition() -> Dict[str, List[Tuple[int, float]]]:
     """
     Return a dict with the isotope composition in the solar system.
 
     Data are taken from:
@@ -838,18 +846,18 @@
 
     Returns
     -------
     Dictionary that maps element names to lists of isotope abundances. Isotopes are
     described by the tuple (A, F), where A is the number of nucleons, and F is the
     abundance in arbitrary units.
     """
-    result = {}
+    result: Dict[str, List[Tuple[int, float]]] = {}
     with open(Path(__file__).parent / "solarsystem_abundances2003.dat") as f:
         for line in f:
             m = re.match(r"^ *([0-9]+)([A-Za-z]+)\s*[0-9\.]+\s*([0-9\.e]+)", line)
             if not m:
                 continue
             a = int(m.group(1))
             elem = m.group(2)
-            f = float(m.group(3))
-            result.setdefault(elem, []).append((a, f))
+            abundance = float(m.group(3))
+            result.setdefault(elem, []).append((a, abundance))
     return result
```

### Comparing `crdb-0.6.1/src/crdb/cli.py` & `crdb-0.7.0/src/crdb/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,40 @@
+"""Command line interface for CRDB."""
 import argparse
 import inspect
 import re
 import sys
 import traceback
 
 import crdb
-from crdb._lib import _server_request
-from crdb._lib import _url
-from crdb._lib import query
+from crdb.core import _server_request
+from crdb.core import _url
+from crdb.core import query
+from typing import Optional, List
 
 
-def main(args=None):
+def main(args: Optional[List[str]] = None) -> None:
     """
     Command line interface for CRDB.
 
     Returns unprocessed DB output to stdout.
     """
     parser = argparse.ArgumentParser(description=main.__doc__)
 
+    assert isinstance(query.__doc__, str)
     descriptions = {
         k: re.sub(r"\s+", " ", v.strip())
         for (k, v) in re.findall(
             r"^ {4}([a-z_]+): *[a-z, ]+\n((?: {8}.+\n)+)", query.__doc__, re.MULTILINE
         )
     }
-    descriptions[
-        "format"
-    ] = "Output format; one of 'usine', 'galprop', 'csv'. Default is 'usine'."
+    descriptions["format"] = (
+        "Output format; one of 'usine', 'galprop', 'csv', 'csv-asimport'. "
+        "Default is 'csv-asimport'."
+    )
 
     for name, par in inspect.signature(_url).parameters.items():
         name2 = name.replace("_", "-")
         h = descriptions.get(name, "").replace("%", "%%")
         tp = par.annotation
         if isinstance(tp, str):
             tp = eval(tp)
@@ -56,11 +60,11 @@
     )
 
     args = parser.parse_args(args=args)
     kwargs = {k.replace("-", "_"): v for (k, v) in vars(args).items() if k != "timeout"}
     try:
         url = _url(**kwargs)
     except ValueError as e:
-        sys.stderr.write("".join(traceback.format_exception_only(e)))
+        sys.stderr.write("".join(traceback.format_exception_only(e)))  # type:ignore
         sys.exit(1)
     data = _server_request(url, timeout=args.timeout)
     print("\n".join(data))
```

### Comparing `crdb-0.6.1/src/crdb/crdb_logo.png` & `crdb-0.7.0/src/crdb/crdb_logo.png`

 * *Files identical despite different names*

### Comparing `crdb-0.6.1/src/crdb/experimental.py` & `crdb-0.7.0/src/crdb/experimental.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,70 @@
 """
 Experimental utilitites for the crdb Python package.
 
 The functions in this module are not stable and their API can
 change at any time. Use with caution.
 """
+from typing import Dict, Tuple, Union
+
 import numpy as np
 from numpy.typing import NDArray
 
 from crdb import ELEMENTS
 from crdb import VALID_NAMES
 from crdb import solar_system_composition
 
 NUCLEON_MASS = 0.9389187543299999  # GeV
 ELECTRON_MASS = 0.51099895e-3  # GeV
 
 
-def energy_conversion_numbers():
+def energy_conversion_numbers() -> Dict[str, Tuple[int, float]]:
+    """
+    Return dict with energy conversion numbers.
+
+    Returns
+    -------
+    dict
+        Maps the quantity name to a tuple (Z, A), where Z is the atomic number and A is
+        the number of nucleons. Returns (1, NaN) for electrons and positrons.
+    """
     comp = solar_system_composition()
     result = {k: (1, np.nan) for k in ("e-", "e+", "e-+e+")}
     for key, z in ELEMENTS.items():
         if key in comp:
-            asum = 0
-            wsum = 0
-            for a, w in comp[key]:
-                asum += a * w
-                wsum += w
-            a = asum / wsum
+            a, w = np.transpose(comp[key])
+            a_mean = np.average(a, weights=w)
         else:
-            a = np.nan
-        result[key] = (z, a)
+            a_mean = np.nan
+        result[key] = (z, a_mean)
 
     for key in VALID_NAMES:
         if key.endswith("-bar") and key[:-4] in result:
             result[key] = result[key[:-4]]
 
     return result
 
 
-def convert_energy(table: NDArray, target="EKN", approximate=True) -> NDArray:
+def convert_energy(
+    table: np.recarray, target: str = "EKN", approximate: bool = True
+) -> np.recarray:
     """
-    Converts e_axis of all convertible quantities and removes the rest.
+    Convert e_type of all convertible quantities to target and removes the rest.
 
     Parameters
     ----------
     table : array
         CRDB table.
     target : str, optional
         What to convert the e_axis to.
     approximate : bool, optional
         Whether approximate conversion is allowed. An approximate conversion
         happens when an elemental flux with an unknown isotopic composition
         is converted and the effective number of nucleons is required.
-        Default is false.
+        Default is true.
 
     Returns
     -------
     Converted table.
     """
     ecn = energy_conversion_numbers()
 
@@ -95,15 +104,17 @@
                 pass
             else:
                 assert False
 
     return result[~np.isnan(result.value) & (result.e_type == target)]
 
 
-def _convert_energy(tab, mask, f):
+def _convert_energy(
+    tab: np.recarray, mask: Union[int, NDArray], f: Union[float, NDArray]
+) -> None:
     if np.ndim(f) > 0:
-        f.shape = (len(f), 1)
+        f.shape = (len(f), 1)  # type:ignore
     tab[mask].e *= f
     tab[mask].e_bin *= f
     tab[mask].value /= f
     tab[mask].err_sta /= f
     tab[mask].err_sys /= f
```

### Comparing `crdb-0.6.1/src/crdb/mpl.py` & `crdb-0.7.0/src/crdb/mpl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-from pathlib import Path
+"""Helper functions to draw plots from tables with matplotlib."""
 
+import warnings
+from pathlib import Path
 import numpy as np
+from typing import Any, Optional
 from matplotlib import pyplot as plt
-from numpy.typing import NDArray
+from matplotlib.lines import Line2D
+from crdb.core import get_mean_datetime
 
 
-def draw_table(table, factor=1.0, label=None, sys_lw=5, **kwargs):
+def draw_table(
+    table: np.recarray,
+    factor: float = 1.0,
+    label: Optional[str] = None,
+    sys_lw: float = 5,
+    **kwargs: Any,
+) -> Line2D:
     """
     Draw table with statistical and systematic error bars.
 
     Parameters
     ----------
     table : array
         CRDB table.
@@ -38,20 +48,82 @@
         color=lines.get_color(),
         alpha=0.5,
         **kwargs,
     )
     return lines
 
 
+def draw_timeseries(
+    table: np.recarray,
+    factor: float = 1.0,
+    label: Optional[str] = None,
+    sys_lw: float = 5,
+    **kwargs: Any,
+) -> Line2D:
+    """
+    Draw table as a time series with statistical and systematic error bars.
+
+    Parameters
+    ----------
+    table : array
+        CRDB table.
+    factor : array-like, optional
+        Optional scaling factor for the y-coordinates. Default is 1.
+    label : str, optional
+        Optional label for the plot.
+    sys_lw : float, optional
+        Line width for the error bar that represents systematic uncertainties.
+    """
+    mask = []
+    x = []
+    xrange = []
+    for dt in table.datetime:
+        if ";" in dt:
+            mask.append(False)
+        else:
+            mask.append(True)
+            x1, x2 = get_mean_datetime(dt)
+            x.append(x1)
+            xrange.append(x2)
+    mask = np.array(mask)
+    n_invalid = np.sum(~mask)
+    if n_invalid:
+        msg = (
+            f"input contains {n_invalid} points with multiple time ranges, "
+            "which are ignored"
+        )
+        warnings.warn(msg, RuntimeWarning)
+        table = table[mask]
+    y = table.value * factor
+    ye1 = np.transpose(table.err_sta) * factor
+    ye2 = np.transpose(table.err_sys) * factor
+    lines = plt.errorbar(x, y, ye1, xerr=xrange, ls="none", label=label, **kwargs)[0]
+    for key in ("color", "alpha", "lw", "marker"):
+        if key in kwargs:
+            del kwargs[key]
+    plt.errorbar(
+        x,
+        y,
+        ye2,
+        marker="none",
+        ls="none",
+        lw=sys_lw,
+        color=lines.get_color(),
+        alpha=0.5,
+        **kwargs,
+    )
+    return lines
+
+
 def draw_references(
-    table: NDArray,
+    table: np.recarray,
     color: str = "0.5",
     fontsize: str = "xx-small",
-    **kwargs,
-):
+    **kwargs: Any,
+) -> None:
     """
     List references for table in columns using a modified Legend artist.
 
     The references are drawn using a legend artist, but the normal legend is
     not overridden.
 
     Parameters
@@ -82,15 +154,17 @@
         title_fontproperties={"size": fontsize},
         **kwargs,
     )
     leg.get_title().set_color(color)
     plt.gcf().add_artist(leg)
 
 
-def draw_logo(x, y, height=0.1, zorder=None):
+def draw_logo(
+    x: float, y: float, height: float = 0.1, zorder: Optional[int] = None
+) -> None:
     """
     Draw the CRDB logo.
 
     Parameters
     ----------
     x : float
         Left edge of image box in axes coordinates.
```

### Comparing `crdb-0.6.1/src/crdb/solarsystem_abundances2003.dat` & `crdb-0.7.0/src/crdb/solarsystem_abundances2003.dat`

 * *Files identical despite different names*

### Comparing `crdb-0.6.1/src/crdb.egg-info/PKG-INFO` & `crdb-0.7.0/src/crdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crdb
-Version: 0.6.1
+Version: 0.7.0
 Summary: CRDB Python frontend
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/crdb-project/crdb
 Project-URL: documentation, https://lpsc.in2p3.fr/crdb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `crdb-0.6.1/src/crdb.egg-info/SOURCES.txt` & `crdb-0.7.0/src/crdb.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/reference.rst
 docs/spelling_wordlist.txt
 src/crdb/__init__.py
 src/crdb/__main__.py
-src/crdb/_lib.py
 src/crdb/cli.py
+src/crdb/core.py
 src/crdb/crdb_logo.png
 src/crdb/experimental.py
 src/crdb/mpl.py
 src/crdb/solarsystem_abundances2003.dat
 src/crdb.egg-info/PKG-INFO
 src/crdb.egg-info/SOURCES.txt
 src/crdb.egg-info/dependency_links.txt
```

### Comparing `crdb-0.6.1/tests/test_experimental.py` & `crdb-0.7.0/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `crdb-0.6.1/tests/test_lib.py` & `crdb-0.7.0/tests/test_lib.py`

 * *Files identical despite different names*

