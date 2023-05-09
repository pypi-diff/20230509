# Comparing `tmp/circuitpython-styles-0.6.3.tar.gz` & `tmp/circuitpython-styles-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-styles-0.6.3.tar", last modified: Tue Jan 31 00:08:26 2023, max compression
+gzip compressed data, was "circuitpython-styles-0.7.0.tar", last modified: Tue May  9 01:53:11 2023, max compression
```

## Comparing `circuitpython-styles-0.6.3.tar` & `circuitpython-styles-0.7.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:08:26.083691 circuitpython-styles-0.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:08:26.079690 circuitpython-styles-0.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:08:26.083691 circuitpython-styles-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:08:26.083691 circuitpython-styles-0.6.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-01-31 00:08:26.083691 circuitpython-styles-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:08:26.083691 circuitpython-styles-0.6.3/circuitpython_styles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-01-31 00:08:26.000000 circuitpython-styles-0.6.3/circuitpython_styles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-31 00:08:26.000000 circuitpython-styles-0.6.3/circuitpython_styles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 00:08:26.000000 circuitpython-styles-0.6.3/circuitpython_styles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-31 00:08:26.000000 circuitpython-styles-0.6.3/circuitpython_styles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-31 00:08:26.000000 circuitpython-styles-0.6.3/circuitpython_styles.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:08:26.083691 circuitpython-styles-0.6.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:08:26.083691 circuitpython-styles-0.6.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)    12511 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/docs/styles.gif
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/docs/styles.gif.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:08:26.083691 circuitpython-styles-0.6.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-01-31 00:08:18.000000 circuitpython-styles-0.6.3/examples/styles_advanced_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-31 00:08:18.000000 circuitpython-styles-0.6.3/examples/styles_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-01-31 00:08:18.000000 circuitpython-styles-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-31 00:08:09.000000 circuitpython-styles-0.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 00:08:26.083691 circuitpython-styles-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-01-31 00:08:18.000000 circuitpython-styles-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 00:08:26.083691 circuitpython-styles-0.6.3/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-01-31 00:08:18.000000 circuitpython-styles-0.6.3/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-01-31 00:08:18.000000 circuitpython-styles-0.6.3/styles/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.459164 circuitpython-styles-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.451164 circuitpython-styles-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.455164 circuitpython-styles-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.455164 circuitpython-styles-0.7.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-09 01:53:11.459164 circuitpython-styles-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.455164 circuitpython-styles-0.7.0/circuitpython_styles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-09 01:53:11.000000 circuitpython-styles-0.7.0/circuitpython_styles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-09 01:53:11.000000 circuitpython-styles-0.7.0/circuitpython_styles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 01:53:11.000000 circuitpython-styles-0.7.0/circuitpython_styles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 01:53:11.000000 circuitpython-styles-0.7.0/circuitpython_styles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 01:53:11.000000 circuitpython-styles-0.7.0/circuitpython_styles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.455164 circuitpython-styles-0.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.455164 circuitpython-styles-0.7.0/docs/_static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4414 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/index.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12511 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/styles.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/styles.gif.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.459164 circuitpython-styles-0.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/examples/styles_advanced_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/examples/styles_list_select_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/examples/styles_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 01:53:11.459164 circuitpython-styles-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.459164 circuitpython-styles-0.7.0/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/styles/styles.py
```

### Comparing `circuitpython-styles-0.6.3/.pre-commit-config.yaml` & `circuitpython-styles-0.7.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
     rev: 22.3.0
     hooks:
       - id: black
-  - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
-    hooks:
-      - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
```

### Comparing `circuitpython-styles-0.6.3/.pylintrc` & `circuitpython-styles-0.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.6.3/CODE_OF_CONDUCT.md` & `circuitpython-styles-0.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.6.3/LICENSE` & `circuitpython-styles-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.6.3/LICENSES/CC-BY-4.0.txt` & `circuitpython-styles-0.7.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.6.3/LICENSES/MIT.txt` & `circuitpython-styles-0.7.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.6.3/LICENSES/Unlicense.txt` & `circuitpython-styles-0.7.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.6.3/PKG-INFO` & `circuitpython-styles-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-styles
-Version: 0.6.3
+Version: 0.7.0
 Summary: Dynamic style helper for CircuitPython graphical elements
 Home-page: https://github.com/jposada202020/CircuitPython_styles.git
 Author: Jose David M.
 Author-email: "Jose D. Montoya" <styles@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_styles.git
 Keywords: hardware,micropython,circuitpython,graphic,styles,widget,displayio,color,widget,themes
@@ -27,14 +27,22 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_styles/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_styles/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-styles.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-styles
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-styles?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-styles
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Library helper to add styles to CircuitPython display functions
 CircuitPython widgets supported:
```

### Comparing `circuitpython-styles-0.6.3/README.rst` & `circuitpython-styles-0.7.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,22 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_styles/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_styles/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-styles.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-styles
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-styles?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-styles
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Library helper to add styles to CircuitPython display functions
 CircuitPython widgets supported:
```

### Comparing `circuitpython-styles-0.6.3/circuitpython_styles.egg-info/PKG-INFO` & `circuitpython-styles-0.7.0/circuitpython_styles.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-styles
-Version: 0.6.3
+Version: 0.7.0
 Summary: Dynamic style helper for CircuitPython graphical elements
 Home-page: https://github.com/jposada202020/CircuitPython_styles.git
 Author: Jose David M.
 Author-email: "Jose D. Montoya" <styles@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_styles.git
 Keywords: hardware,micropython,circuitpython,graphic,styles,widget,displayio,color,widget,themes
@@ -27,14 +27,22 @@
     :alt: Documentation Status
 
 
 .. image:: https://github.com/jposada202020/CircuitPython_styles/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_styles/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-styles.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-styles
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-styles?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-styles
+
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Library helper to add styles to CircuitPython display functions
 CircuitPython widgets supported:
```

### Comparing `circuitpython-styles-0.6.3/circuitpython_styles.egg-info/SOURCES.txt` & `circuitpython-styles-0.7.0/circuitpython_styles.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -28,10 +28,11 @@
 docs/index.rst
 docs/index.rst.license
 docs/styles.gif
 docs/styles.gif.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/styles_advanced_example.py
+examples/styles_list_select_example.py
 examples/styles_simpletest.py
 styles/__init__.py
 styles/styles.py
```

### Comparing `circuitpython-styles-0.6.3/docs/_static/favicon.ico` & `circuitpython-styles-0.7.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.6.3/docs/conf.py` & `circuitpython-styles-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.6.3/docs/styles.gif` & `circuitpython-styles-0.7.0/docs/styles.gif`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.6.3/examples/styles_advanced_example.py` & `circuitpython-styles-0.7.0/examples/styles_advanced_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.6.3/pyproject.toml` & `circuitpython-styles-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-styles"
 description = "Dynamic style helper for CircuitPython graphical elements"
-version = "0.6.3"
+version = "0.7.0"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "styles@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_styles.git"}
 keywords = [
     "hardware",
@@ -38,12 +38,12 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["CircuitPython_Styles"]
+packages = ["styles"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies = {optional = {file = ["optional_requirements.txt"]}}
```

### Comparing `circuitpython-styles-0.6.3/setup.py` & `circuitpython-styles-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.6.3/styles/__init__.py` & `circuitpython-styles-0.7.0/styles/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 try:
     from typing import Any, Tuple, List
 except ImportError:
     pass
 
-
+# pylint: disable=protected-access
 def apply_style(target, style):
     """
     :param target: widget object
     :param style: Style to apply
 
 
     apply_style could be used in certain libraries that provide access to the color setter.
@@ -43,22 +43,26 @@
      .. code-block:: python
 
         apply_style(text_area, DarkAmber)
 
     The function will verify the object and apply the changes according to the features available
 
     """
+    list_select = ["ListSelect"]
     text_display = ["Label", "Bitmap_label", "ScrollingLabel"]
     annotation_widget = ["Annotation"]
     progress_bar = ["HorizontalProgressBar"]
     buttons = ["Button"]
 
     identifier = target.__class__.__name__
 
-    if identifier in text_display:
+    if identifier in list_select:
+        target._label.color = style["TEXT"]
+        target._label.background_color = style["BACKGROUND"]
+    elif identifier in text_display:
         target.color = style["TEXT"]
         target.background_color = style["BACKGROUND"]
     elif identifier in annotation_widget:
         target.text_color = style["TEXT"]
     elif identifier in progress_bar:
         target.bar_color = style["BACKGROUND"]
         target.border_color = style["LINE_COLOR"]
```

### Comparing `circuitpython-styles-0.6.3/styles/styles.py` & `circuitpython-styles-0.7.0/styles/styles.py`

 * *Files identical despite different names*

