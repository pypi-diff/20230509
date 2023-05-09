# Comparing `tmp/attribtool-1.0.1.tar.gz` & `tmp/attribtool-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attribtool-1.0.1.tar", max compression
+gzip compressed data, was "attribtool-1.0.2.tar", max compression
```

## Comparing `attribtool-1.0.1.tar` & `attribtool-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1081 2023-05-07 20:48:57.095800 attribtool-1.0.1/LICENSE
--rw-r--r--   0        0        0     1691 2023-05-08 17:43:58.399227 attribtool-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-07 09:06:36.254156 attribtool-1.0.1/attribtool/__init__.py
--rw-r--r--   0        0        0      780 2023-05-08 18:12:08.012527 attribtool-1.0.1/attribtool/ndattrib.py
--rw-r--r--   0        0        0     1303 2023-05-08 18:13:21.401434 attribtool-1.0.1/attribtool/nnattrib.py
--rw-r--r--   0        0        0      853 2023-05-08 17:44:58.816167 attribtool-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 attribtool-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-07 20:48:57.095800 attribtool-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1691 2023-05-08 17:43:58.399227 attribtool-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 09:06:36.254156 attribtool-1.0.2/attribtool/__init__.py
+-rw-r--r--   0        0        0      780 2023-05-08 18:12:08.012527 attribtool-1.0.2/attribtool/ndattrib.py
+-rw-r--r--   0        0        0     1382 2023-05-09 19:06:46.806355 attribtool-1.0.2/attribtool/nnattrib.py
+-rw-r--r--   0        0        0      853 2023-05-09 19:04:16.948710 attribtool-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 attribtool-1.0.2/PKG-INFO
```

### Comparing `attribtool-1.0.1/LICENSE` & `attribtool-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `attribtool-1.0.1/README.md` & `attribtool-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `attribtool-1.0.1/attribtool/ndattrib.py` & `attribtool-1.0.2/attribtool/ndattrib.py`

 * *Files identical despite different names*

### Comparing `attribtool-1.0.1/attribtool/nnattrib.py` & `attribtool-1.0.2/attribtool/nnattrib.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,19 +6,20 @@
   Purpose: NoNewAttributes class for restricting the creation of dynamic
   attributes on instances of derived types.
 
   The solution idea published in: Python Cookbook (2004), A. Martelli,
   A. Ravenscroft, D. Ascher
 """
 
-from types import FunctionType
-from typing import Any
+from typing import Any, Callable
 
 
-def _no_new_attributes(wrapped_setattr: Any) -> FunctionType:
+def _no_new_attributes(
+    wrapped_setattr: Any,
+) -> Callable[[Any, str, Any], None]:
     """Internal function for use in the current module only."""
 
     def __setattr__(self, name: str, value: Any) -> None:
         """Check if the attribute is defined, throw an exception if not."""
         if hasattr(self, name):
             wrapped_setattr(self, name, value)
         else:
@@ -32,14 +33,18 @@
 class NoNewAttributes:
     """NoNewAttributes - base class.
 
     Class for restricting the creation of dynamic attributes on instances
     of derived types.
     """
 
-    __setattr__: FunctionType = _no_new_attributes(object.__setattr__)
+    __setattr__: Callable[[Any, str, Any], None] = _no_new_attributes(
+        object.__setattr__
+    )
 
     class __metaclass__(type):
-        __setattr__: FunctionType = _no_new_attributes(type.__setattr__)
+        __setattr__: Callable[[Any, str, Any], None] = _no_new_attributes(
+            type.__setattr__
+        )
 
 
 # #[EOF]#######################################################################
```

### Comparing `attribtool-1.0.1/pyproject.toml` & `attribtool-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "attribtool"
-version = "1.0.1"
+version = "1.0.2"
 description = "Base classes for restricting the creation of dynamic attributes on instances of derived types."
 authors = ["Jacek Kotlarski <szumak@virthost.pl>"]
 maintainers = ["Jacek Kotlarski <szumak@virthost.pl>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Szumak75/AttribTool"
 classifiers = [
```

### Comparing `attribtool-1.0.1/PKG-INFO` & `attribtool-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attribtool
-Version: 1.0.1
+Version: 1.0.2
 Summary: Base classes for restricting the creation of dynamic attributes on instances of derived types.
 Home-page: https://github.com/Szumak75/AttribTool
 License: MIT
 Author: Jacek Kotlarski
 Author-email: szumak@virthost.pl
 Maintainer: Jacek Kotlarski
 Maintainer-email: szumak@virthost.pl
```

