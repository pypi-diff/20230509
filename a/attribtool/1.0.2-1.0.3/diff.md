# Comparing `tmp/attribtool-1.0.2.tar.gz` & `tmp/attribtool-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attribtool-1.0.2.tar", max compression
+gzip compressed data, was "attribtool-1.0.3.tar", max compression
```

## Comparing `attribtool-1.0.2.tar` & `attribtool-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1081 2023-05-07 20:48:57.095800 attribtool-1.0.2/LICENSE
--rw-r--r--   0        0        0     1691 2023-05-08 17:43:58.399227 attribtool-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-05-07 09:06:36.254156 attribtool-1.0.2/attribtool/__init__.py
--rw-r--r--   0        0        0      780 2023-05-08 18:12:08.012527 attribtool-1.0.2/attribtool/ndattrib.py
--rw-r--r--   0        0        0     1382 2023-05-09 19:06:46.806355 attribtool-1.0.2/attribtool/nnattrib.py
--rw-r--r--   0        0        0      853 2023-05-09 19:04:16.948710 attribtool-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 attribtool-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-07 20:48:57.095800 attribtool-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1691 2023-05-08 17:43:58.399227 attribtool-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 09:06:36.254156 attribtool-1.0.3/attribtool/__init__.py
+-rw-r--r--   0        0        0      780 2023-05-08 18:12:08.012527 attribtool-1.0.3/attribtool/ndattrib.py
+-rw-r--r--   0        0        0     1382 2023-05-09 19:06:46.806355 attribtool-1.0.3/attribtool/nnattrib.py
+-rw-r--r--   0        0        0        0 2023-05-09 19:20:30.410450 attribtool-1.0.3/attribtool/py.typed
+-rw-r--r--   0        0        0      853 2023-05-09 19:21:24.763042 attribtool-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 attribtool-1.0.3/PKG-INFO
```

### Comparing `attribtool-1.0.2/LICENSE` & `attribtool-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `attribtool-1.0.2/README.md` & `attribtool-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `attribtool-1.0.2/attribtool/ndattrib.py` & `attribtool-1.0.3/attribtool/ndattrib.py`

 * *Files identical despite different names*

### Comparing `attribtool-1.0.2/attribtool/nnattrib.py` & `attribtool-1.0.3/attribtool/nnattrib.py`

 * *Files identical despite different names*

### Comparing `attribtool-1.0.2/pyproject.toml` & `attribtool-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "attribtool"
-version = "1.0.2"
+version = "1.0.3"
 description = "Base classes for restricting the creation of dynamic attributes on instances of derived types."
 authors = ["Jacek Kotlarski <szumak@virthost.pl>"]
 maintainers = ["Jacek Kotlarski <szumak@virthost.pl>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Szumak75/AttribTool"
 classifiers = [
```

### Comparing `attribtool-1.0.2/PKG-INFO` & `attribtool-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attribtool
-Version: 1.0.2
+Version: 1.0.3
 Summary: Base classes for restricting the creation of dynamic attributes on instances of derived types.
 Home-page: https://github.com/Szumak75/AttribTool
 License: MIT
 Author: Jacek Kotlarski
 Author-email: szumak@virthost.pl
 Maintainer: Jacek Kotlarski
 Maintainer-email: szumak@virthost.pl
```

