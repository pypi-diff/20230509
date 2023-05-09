# Comparing `tmp/py-racoon-0.1.3.tar.gz` & `tmp/py-racoon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-racoon-0.1.3.tar", last modified: Tue May  9 16:22:04 2023, max compression
+gzip compressed data, was "py-racoon-0.1.4.tar", last modified: Tue May  9 16:22:03 2023, max compression
```

## Comparing `py-racoon-0.1.3.tar` & `py-racoon-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:22:04.286573 py-racoon-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-09 16:21:56.000000 py-racoon-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 16:21:56.000000 py-racoon-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-09 16:22:04.286573 py-racoon-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-09 16:21:56.000000 py-racoon-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-09 16:21:56.000000 py-racoon-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-09 16:22:04.286573 py-racoon-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-09 16:21:56.000000 py-racoon-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:22:04.286573 py-racoon-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:22:04.286573 py-racoon-0.1.3/src/py_racoon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-09 16:22:04.000000 py-racoon-0.1.3/src/py_racoon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-09 16:22:04.000000 py-racoon-0.1.3/src/py_racoon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:22:04.000000 py-racoon-0.1.3/src/py_racoon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-09 16:22:04.000000 py-racoon-0.1.3/src/py_racoon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-09 16:22:04.000000 py-racoon-0.1.3/src/py_racoon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 16:22:04.000000 py-racoon-0.1.3/src/py_racoon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:22:04.286573 py-racoon-0.1.3/src/racoon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:21:56.000000 py-racoon-0.1.3/src/racoon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-09 16:21:56.000000 py-racoon-0.1.3/src/racoon/argument_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-09 16:21:56.000000 py-racoon-0.1.3/src/racoon/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-09 16:21:56.000000 py-racoon-0.1.3/src/racoon/github_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-09 16:21:56.000000 py-racoon-0.1.3/src/racoon/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-09 16:21:56.000000 py-racoon-0.1.3/src/racoon/template_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 16:22:01.000000 py-racoon-0.1.3/src/racoon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:22:03.213276 py-racoon-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-09 16:21:55.000000 py-racoon-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 16:21:55.000000 py-racoon-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-09 16:22:03.213276 py-racoon-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-09 16:21:55.000000 py-racoon-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-09 16:21:55.000000 py-racoon-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-09 16:22:03.213276 py-racoon-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-09 16:21:55.000000 py-racoon-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:22:03.209276 py-racoon-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:22:03.213276 py-racoon-0.1.4/src/py_racoon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-09 16:22:03.000000 py-racoon-0.1.4/src/py_racoon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-09 16:22:03.000000 py-racoon-0.1.4/src/py_racoon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:22:03.000000 py-racoon-0.1.4/src/py_racoon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-09 16:22:03.000000 py-racoon-0.1.4/src/py_racoon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-09 16:22:03.000000 py-racoon-0.1.4/src/py_racoon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 16:22:03.000000 py-racoon-0.1.4/src/py_racoon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:22:03.213276 py-racoon-0.1.4/src/racoon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:21:55.000000 py-racoon-0.1.4/src/racoon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-09 16:21:55.000000 py-racoon-0.1.4/src/racoon/argument_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-09 16:21:55.000000 py-racoon-0.1.4/src/racoon/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-09 16:21:55.000000 py-racoon-0.1.4/src/racoon/github_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-09 16:21:55.000000 py-racoon-0.1.4/src/racoon/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-09 16:21:55.000000 py-racoon-0.1.4/src/racoon/template_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 16:22:01.000000 py-racoon-0.1.4/src/racoon/version.py
```

### Comparing `py-racoon-0.1.3/LICENSE` & `py-racoon-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-racoon-0.1.3/PKG-INFO` & `py-racoon-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-racoon
-Version: 0.1.3
+Version: 0.1.4
 Summary: Racoon
 Home-page: https://github.com/nymann/racoon
 Maintainer: Kristian Nymann Jakobsen
 Maintainer-email: kristian@nymann.dev
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `py-racoon-0.1.3/README.md` & `py-racoon-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `py-racoon-0.1.3/setup.cfg` & `py-racoon-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `py-racoon-0.1.3/src/py_racoon.egg-info/PKG-INFO` & `py-racoon-0.1.4/src/py_racoon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-racoon
-Version: 0.1.3
+Version: 0.1.4
 Summary: Racoon
 Home-page: https://github.com/nymann/racoon
 Maintainer: Kristian Nymann Jakobsen
 Maintainer-email: kristian@nymann.dev
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `py-racoon-0.1.3/src/racoon/github_integration.py` & `py-racoon-0.1.4/src/racoon/github_integration.py`

 * *Files identical despite different names*

### Comparing `py-racoon-0.1.3/src/racoon/main.py` & `py-racoon-0.1.4/src/racoon/main.py`

 * *Files identical despite different names*

### Comparing `py-racoon-0.1.3/src/racoon/template_generation.py` & `py-racoon-0.1.4/src/racoon/template_generation.py`

 * *Files identical despite different names*

