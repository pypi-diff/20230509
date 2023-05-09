# Comparing `tmp/firestone_lib-0.1.5.tar.gz` & `tmp/firestone_lib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestone_lib-0.1.5.tar", max compression
+gzip compressed data, was "firestone_lib-0.1.6.tar", max compression
```

## Comparing `firestone_lib-0.1.5.tar` & `firestone_lib-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/LICENSE
--rw-r--r--   0        0        0      311 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/__init__.py
--rw-r--r--   0        0        0     4047 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/cli.py
--rw-r--r--   0        0        0     1419 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/resource.py
--rw-r--r--   0        0        0        0 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/resources/logging/__init__.py
--rw-r--r--   0        0        0      396 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/resources/logging/cli.conf
--rw-r--r--   0        0        0      318 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/utils.py
--rw-r--r--   0        0        0      970 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 firestone_lib-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/LICENSE
+-rw-r--r--   0        0        0      311 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/__init__.py
+-rw-r--r--   0        0        0     4917 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/cli.py
+-rw-r--r--   0        0        0     1419 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/resource.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/resources/logging/__init__.py
+-rw-r--r--   0        0        0      396 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/resources/logging/cli.conf
+-rw-r--r--   0        0        0      319 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/firestone_lib/utils.py
+-rw-r--r--   0        0        0      970 2023-05-09 00:25:21.070340 firestone_lib-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 firestone_lib-0.1.6/PKG-INFO
```

### Comparing `firestone_lib-0.1.5/LICENSE` & `firestone_lib-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `firestone_lib-0.1.5/firestone_lib/cli.py` & `firestone_lib-0.1.6/firestone_lib/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 import logging
 import logging.config
 import re
 import time
 
 import click
 import pkg_resources
+import yaml
+
+try:
+    from yaml import CLoader as Loader
+except ImportError:
+    from yaml import Loader
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def init_logging(pkg: str, name: str) -> None:
     """Initialize a logging config file for logging.
 
@@ -51,37 +57,54 @@
 
         try:
             return [self.item_type.convert(item, param, ctx) for item in value.split(",")]
         except AttributeError:
             self.fail(f"{value} is not comma-delimited", param, ctx)
 
 
-class FromJSON(click.ParamType):
-    """Converts a string from the CLI as a parameter to JSON object."""
+class FromJsonOrYaml(click.ParamType):
+    """Converts a string from the CLI as a parameter to JSON or YAML object."""
 
-    name = "String to JSON object, optionally via a file, using @file.json"
+    name = "String to JSON or YAML object, optionally via a file, using @file.json"
 
     def __init__(self, decoder=None):
         self.decoder = decoder or json.JSONDecoder()
 
     def convert(self, value, param, ctx):
         """Convert a string from the CLI as a parameter to JSON object."""
         if value == "-":
             return "-"
         if not isinstance(value, str):
             return value
 
         if value.startswith("@"):
             filename = value[1:]
-            _LOGGER.debug(f"Reading JSON data from file {filename}")
+            _LOGGER.debug(f"Reading data from file {filename}...")
             with io.open(filename, "r", encoding="utf-8") as fh:
-                return json.load(fh)
+                try:
+                    _LOGGER.debug("Trying json.load")
+                    print("trying json")
+                    return json.load(fh)
+                # pylint: disable=broad-exception-caught
+                except Exception:
+                    pass
+                try:
+                    _LOGGER.debug("Trying yaml.load")
+                    return yaml.load(fh, Loader=Loader)
+                # pylint: disable=broad-exception-caught
+                except Exception:
+                    self.fail(f"{value} is not in JSON or YAML format", param, ctx)
 
         raw_str = rf"{value}"
-        return self.decoder.decode(raw_str)
+        try:
+            return self.decoder.decode(raw_str)
+        except json.decoder.JSONDecodeError:
+            pass
+
+        return yaml.load(value, Loader=Loader)
 
 
 class KeyValue(click.ParamType):
     """A custom click parameter type tha takes key/value items."""
 
     name = "Key and value click type" ""
 
@@ -92,15 +115,15 @@
         self.outer_sep = outer_sep
 
     # pylint: disable=inconsistent-return-statements
     def convert(self, value: str, param: str, ctx):
         """Convert this param value to a dict, given the str."""
         if value and isinstance(value, str) and value.startswith("{"):
             try:
-                json_param_type = FromJSON()
+                json_param_type = FromJsonOrYaml()
                 return json_param_type.convert(value, param, ctx)
             # pylint: disable=broad-except
             except Exception:
                 pass
 
         if value == "-":
             return "-"
@@ -124,11 +147,20 @@
 
 PathList = CommaDelimitedList(item_type=click.Path(exists=True))
 
 StrList = CommaDelimitedList()
 
 StrDict = KeyValue()
 
-AnyDict = FromJSON()
+AnyDict = FromJsonOrYaml()
 
 
-__all__ = ["init_logging", "KeyValue", "IntList", "PathList", "StrList", "StrDict"]
+__all__ = [
+    "init_logging",
+    "KeyValue",
+    "FromJsonOrYaml",
+    "IntList",
+    "PathList",
+    "StrList",
+    "StrDict",
+    "AnyDict",
+]
```

### Comparing `firestone_lib-0.1.5/firestone_lib/resource.py` & `firestone_lib-0.1.6/firestone_lib/resource.py`

 * *Files identical despite different names*

### Comparing `firestone_lib-0.1.5/pyproject.toml` & `firestone_lib-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "firestone-lib"
-version = "0.1.5"
-description = "Library to help build OpneAPI, AsyncAPI and gRPC specs based off one or more resource json schema files"
+version = "0.1.6"
+description = "Library to help build OpenAPI, AsyncAPI and gRPC specs based off one or more resource json schema files"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [
     { include = "firestone_lib" }
 ]
```

### Comparing `firestone_lib-0.1.5/PKG-INFO` & `firestone_lib-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: firestone-lib
-Version: 0.1.5
-Summary: Library to help build OpneAPI, AsyncAPI and gRPC specs based off one or more resource json schema files
+Version: 0.1.6
+Summary: Library to help build OpenAPI, AsyncAPI and gRPC specs based off one or more resource json schema files
 License: Apache 2.0
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

