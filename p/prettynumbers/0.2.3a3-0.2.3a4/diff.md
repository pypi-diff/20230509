# Comparing `tmp/prettynumbers-0.2.3a3.tar.gz` & `tmp/prettynumbers-0.2.3a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettynumbers-0.2.3a3.tar", max compression
+gzip compressed data, was "prettynumbers-0.2.3a4.tar", max compression
```

## Comparing `prettynumbers-0.2.3a3.tar` & `prettynumbers-0.2.3a4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    14849 2016-07-14 20:10:07.000000 prettynumbers-0.2.3a3/LICENSE.txt
--rw-r--r--   0        0        0     1138 2023-05-09 14:21:39.562989 prettynumbers-0.2.3a3/README.md
--rw-r--r--   0        0        0      114 2023-05-09 14:21:39.564690 prettynumbers-0.2.3a3/pretty_numbers/__init__.py
--rwxr-xr-x   0        0        0     1915 2023-05-09 14:21:39.565413 prettynumbers-0.2.3a3/pretty_numbers/pretty_numbers.py
--rw-r--r--   0        0        0        0 2023-05-09 14:21:39.565816 prettynumbers-0.2.3a3/pretty_numbers/py.typed
--rwxr-xr-x   0        0        0     3303 2023-05-09 14:21:39.567517 prettynumbers-0.2.3a3/pretty_numbers/test_pretty_numbers.py
--rw-r--r--   0        0        0      754 2023-05-09 16:08:12.243430 prettynumbers-0.2.3a3/pyproject.toml
--rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 prettynumbers-0.2.3a3/PKG-INFO
+-rw-r--r--   0        0        0    14849 2023-05-09 16:39:42.248501 prettynumbers-0.2.3a4/LICENSE.txt
+-rw-r--r--   0        0        0     1138 2023-05-09 16:39:42.248501 prettynumbers-0.2.3a4/README.md
+-rw-r--r--   0        0        0      114 2023-05-09 16:39:42.248501 prettynumbers-0.2.3a4/pretty_numbers/__init__.py
+-rwxr-xr-x   0        0        0     1915 2023-05-09 16:39:42.248501 prettynumbers-0.2.3a4/pretty_numbers/pretty_numbers.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:39:42.248501 prettynumbers-0.2.3a4/pretty_numbers/py.typed
+-rwxr-xr-x   0        0        0     3303 2023-05-09 16:39:42.248501 prettynumbers-0.2.3a4/pretty_numbers/test_pretty_numbers.py
+-rw-r--r--   0        0        0      754 2023-05-09 16:39:42.248501 prettynumbers-0.2.3a4/pyproject.toml
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 prettynumbers-0.2.3a4/setup.py
+-rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 prettynumbers-0.2.3a4/PKG-INFO
```

### Comparing `prettynumbers-0.2.3a3/LICENSE.txt` & `prettynumbers-0.2.3a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.2.3a3/README.md` & `prettynumbers-0.2.3a4/README.md`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.2.3a3/pretty_numbers/pretty_numbers.py` & `prettynumbers-0.2.3a4/pretty_numbers/pretty_numbers.py`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.2.3a3/pretty_numbers/test_pretty_numbers.py` & `prettynumbers-0.2.3a4/pretty_numbers/test_pretty_numbers.py`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.2.3a3/pyproject.toml` & `prettynumbers-0.2.3a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prettynumbers"
-version = "0.2.3a3"
+version = "0.2.3a4"
 authors = ["gerardk <gerardk@gmail.com>"]
 description="Display a range of numbers in a human readable way"
 license="GNU GENERAL PUBLIC LICENSE"
 packages = [{include = "pretty_numbers"}]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `prettynumbers-0.2.3a3/PKG-INFO` & `prettynumbers-0.2.3a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.2.3a3
+Version: 0.2.3a4
 Summary: Display a range of numbers in a human readable way
 License: GNU GENERAL PUBLIC LICENSE
 Author: gerardk
 Author-email: gerardk@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

