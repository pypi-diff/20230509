# Comparing `tmp/prettynumbers-0.2.2.tar.gz` & `tmp/prettynumbers-0.2.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettynumbers-0.2.2.tar", last modified: Tue May  9 13:57:56 2023, max compression
+gzip compressed data, was "prettynumbers-0.2.3a3.tar", max compression
```

## Comparing `prettynumbers-0.2.2.tar` & `prettynumbers-0.2.3a3.tar`

### file list

```diff
@@ -1,18 +1,8 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 13:57:56.989126 prettynumbers-0.2.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14849 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-09 13:57:56.989126 prettynumbers-0.2.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1138 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      500 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 13:57:56.989126 prettynumbers-0.2.2/pretty_numbers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/pretty_numbers/__init__.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1915 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/pretty_numbers/pretty_numbers.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     3303 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/pretty_numbers/test_pretty_numbers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 13:57:56.989126 prettynumbers-0.2.2/prettynumbers.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-09 13:57:56.000000 prettynumbers-0.2.2/prettynumbers.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      324 2023-05-09 13:57:56.000000 prettynumbers-0.2.2/prettynumbers.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-09 13:57:56.000000 prettynumbers-0.2.2/prettynumbers.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-05-09 13:57:56.000000 prettynumbers-0.2.2/prettynumbers.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-05-09 13:57:56.989126 prettynumbers-0.2.2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2023-05-09 13:57:51.000000 prettynumbers-0.2.2/setup.py
+-rw-r--r--   0        0        0    14849 2016-07-14 20:10:07.000000 prettynumbers-0.2.3a3/LICENSE.txt
+-rw-r--r--   0        0        0     1138 2023-05-09 14:21:39.562989 prettynumbers-0.2.3a3/README.md
+-rw-r--r--   0        0        0      114 2023-05-09 14:21:39.564690 prettynumbers-0.2.3a3/pretty_numbers/__init__.py
+-rwxr-xr-x   0        0        0     1915 2023-05-09 14:21:39.565413 prettynumbers-0.2.3a3/pretty_numbers/pretty_numbers.py
+-rw-r--r--   0        0        0        0 2023-05-09 14:21:39.565816 prettynumbers-0.2.3a3/pretty_numbers/py.typed
+-rwxr-xr-x   0        0        0     3303 2023-05-09 14:21:39.567517 prettynumbers-0.2.3a3/pretty_numbers/test_pretty_numbers.py
+-rw-r--r--   0        0        0      754 2023-05-09 16:08:12.243430 prettynumbers-0.2.3a3/pyproject.toml
+-rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 prettynumbers-0.2.3a3/PKG-INFO
```

### Comparing `prettynumbers-0.2.2/LICENSE.txt` & `prettynumbers-0.2.3a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.2.2/README.md` & `prettynumbers-0.2.3a3/README.md`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.2.2/pretty_numbers/pretty_numbers.py` & `prettynumbers-0.2.3a3/pretty_numbers/pretty_numbers.py`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.2.2/pretty_numbers/test_pretty_numbers.py` & `prettynumbers-0.2.3a3/pretty_numbers/test_pretty_numbers.py`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.2.2/pyproject.toml` & `prettynumbers-0.2.3a3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [tool.poetry]
 name = "prettynumbers"
-version = "0.1.1"
+version = "0.2.3a3"
 authors = ["gerardk <gerardk@gmail.com>"]
 description="Display a range of numbers in a human readable way"
 license="GNU GENERAL PUBLIC LICENSE"
+packages = [{include = "pretty_numbers"}]
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.3"
 isort = "^5.12.0"
```

