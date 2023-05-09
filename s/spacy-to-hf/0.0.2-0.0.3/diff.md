# Comparing `tmp/spacy-to-hf-0.0.2.tar.gz` & `tmp/spacy-to-hf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-to-hf-0.0.2.tar", last modified: Mon May  8 17:33:10 2023, max compression
+gzip compressed data, was "spacy-to-hf-0.0.3.tar", last modified: Tue May  9 15:33:00 2023, max compression
```

## Comparing `spacy-to-hf-0.0.2.tar` & `spacy-to-hf-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:33:10.385719 spacy-to-hf-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-08 17:33:10.385719 spacy-to-hf-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-08 17:33:10.385719 spacy-to-hf-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:33:10.385719 spacy-to-hf-0.0.2/spacy_to_hf/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/spacy_to_hf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/spacy_to_hf/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/spacy_to_hf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:33:10.385719 spacy-to-hf-0.0.2/spacy_to_hf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-08 17:33:10.000000 spacy-to-hf-0.0.2/spacy_to_hf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-08 17:33:10.000000 spacy-to-hf-0.0.2/spacy_to_hf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:33:10.000000 spacy-to-hf-0.0.2/spacy_to_hf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-08 17:33:10.000000 spacy-to-hf-0.0.2/spacy_to_hf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 17:33:10.000000 spacy-to-hf-0.0.2/spacy_to_hf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:33:10.385719 spacy-to-hf-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-08 17:32:49.000000 spacy-to-hf-0.0.2/tests/test_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:33:00.655087 spacy-to-hf-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 15:32:34.000000 spacy-to-hf-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-09 15:33:00.655087 spacy-to-hf-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-09 15:32:34.000000 spacy-to-hf-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-09 15:32:34.000000 spacy-to-hf-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-09 15:33:00.655087 spacy-to-hf-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:33:00.655087 spacy-to-hf-0.0.3/spacy_to_hf/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-09 15:32:34.000000 spacy-to-hf-0.0.3/spacy_to_hf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-09 15:32:34.000000 spacy-to-hf-0.0.3/spacy_to_hf/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-09 15:32:34.000000 spacy-to-hf-0.0.3/spacy_to_hf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:33:00.655087 spacy-to-hf-0.0.3/spacy_to_hf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-09 15:33:00.000000 spacy-to-hf-0.0.3/spacy_to_hf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-09 15:33:00.000000 spacy-to-hf-0.0.3/spacy_to_hf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:33:00.000000 spacy-to-hf-0.0.3/spacy_to_hf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-09 15:33:00.000000 spacy-to-hf-0.0.3/spacy_to_hf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 15:33:00.000000 spacy-to-hf-0.0.3/spacy_to_hf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:33:00.655087 spacy-to-hf-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-09 15:32:34.000000 spacy-to-hf-0.0.3/tests/test_conversion.py
```

### Comparing `spacy-to-hf-0.0.2/LICENSE` & `spacy-to-hf-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-to-hf-0.0.2/PKG-INFO` & `spacy-to-hf-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-to-hf
-Version: 0.0.2
+Version: 0.0.3
 Summary: Spacy to HF converter
 Author-email: Ben Epstein <ben.epstein97+spacy-hf@gmail.com>
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/ben-epstein/spacy-to-hf
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `spacy-to-hf-0.0.2/README.md` & `spacy-to-hf-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spacy-to-hf-0.0.2/pyproject.toml` & `spacy-to-hf-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spacy-to-hf-0.0.2/spacy_to_hf/conversion.py` & `spacy-to-hf-0.0.3/spacy_to_hf/conversion.py`

 * *Files identical despite different names*

### Comparing `spacy-to-hf-0.0.2/spacy_to_hf/utils.py` & `spacy-to-hf-0.0.3/spacy_to_hf/utils.py`

 * *Files identical despite different names*

### Comparing `spacy-to-hf-0.0.2/spacy_to_hf.egg-info/PKG-INFO` & `spacy-to-hf-0.0.3/spacy_to_hf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-to-hf
-Version: 0.0.2
+Version: 0.0.3
 Summary: Spacy to HF converter
 Author-email: Ben Epstein <ben.epstein97+spacy-hf@gmail.com>
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/ben-epstein/spacy-to-hf
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `spacy-to-hf-0.0.2/tests/test_conversion.py` & `spacy-to-hf-0.0.3/tests/test_conversion.py`

 * *Files identical despite different names*

