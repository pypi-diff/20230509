# Comparing `tmp/sampling-constraints-0.0.5.tar.gz` & `tmp/sampling-constraints-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampling-constraints-0.0.5.tar", last modified: Mon May  8 00:22:27 2023, max compression
+gzip compressed data, was "sampling-constraints-0.0.6.tar", last modified: Mon May  8 23:10:35 2023, max compression
```

## Comparing `sampling-constraints-0.0.5.tar` & `sampling-constraints-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     1067 2023-05-07 21:44:12.000000 sampling-constraints-0.0.5/LICENSE
--rw-r--r--   0 isaac     (1000) isaac     (1000)      566 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/PKG-INFO
--rw-r--r--   0 isaac     (1000) isaac     (1000)       57 2023-05-07 20:35:15.000000 sampling-constraints-0.0.5/README.md
--rw-r--r--   0 isaac     (1000) isaac     (1000)      632 2023-05-08 00:22:08.000000 sampling-constraints-0.0.5/pyproject.toml
--rw-r--r--   0 isaac     (1000) isaac     (1000)       38 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/setup.cfg
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/src/
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/src/sampling_constraints.egg-info/
--rw-r--r--   0 isaac     (1000) isaac     (1000)      566 2023-05-08 00:22:27.000000 sampling-constraints-0.0.5/src/sampling_constraints.egg-info/PKG-INFO
--rw-r--r--   0 isaac     (1000) isaac     (1000)      393 2023-05-08 00:22:27.000000 sampling-constraints-0.0.5/src/sampling_constraints.egg-info/SOURCES.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-08 00:22:27.000000 sampling-constraints-0.0.5/src/sampling_constraints.egg-info/dependency_links.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)        4 2023-05-08 00:22:27.000000 sampling-constraints-0.0.5/src/sampling_constraints.egg-info/top_level.txt
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/src/scs/
--rw-r--r--   0 isaac     (1000) isaac     (1000)        0 2023-05-07 20:06:06.000000 sampling-constraints-0.0.5/src/scs/__init__.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/src/scs/constraint/
--rw-r--r--   0 isaac     (1000) isaac     (1000)      582 2023-05-07 20:17:09.000000 sampling-constraints-0.0.5/src/scs/constraint/__init__.py
--rw-r--r--   0 isaac     (1000) isaac     (1000)      162 2023-05-07 21:01:04.000000 sampling-constraints-0.0.5/src/scs/constraint/json.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/src/scs/incremental_parse/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     1240 2023-05-07 21:11:34.000000 sampling-constraints-0.0.5/src/scs/incremental_parse/__init__.py
--rw-r--r--   0 isaac     (1000) isaac     (1000)    11411 2023-05-07 22:27:06.000000 sampling-constraints-0.0.5/src/scs/incremental_parse/json.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 00:22:27.345585 sampling-constraints-0.0.5/tests/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     4660 2023-05-08 00:18:23.000000 sampling-constraints-0.0.5/tests/test_json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 23:10:35.127023 sampling-constraints-0.0.6/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     1067 2023-05-07 21:44:12.000000 sampling-constraints-0.0.6/LICENSE
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      566 2023-05-08 23:10:35.127023 sampling-constraints-0.0.6/PKG-INFO
+-rw-r--r--   0 isaac     (1000) isaac     (1000)       57 2023-05-07 20:35:15.000000 sampling-constraints-0.0.6/README.md
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      723 2023-05-08 23:09:27.000000 sampling-constraints-0.0.6/pyproject.toml
+-rw-r--r--   0 isaac     (1000) isaac     (1000)       38 2023-05-08 23:10:35.127023 sampling-constraints-0.0.6/setup.cfg
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 23:10:35.127023 sampling-constraints-0.0.6/src/
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 23:10:35.127023 sampling-constraints-0.0.6/src/sampling_constraints.egg-info/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      566 2023-05-08 23:10:35.000000 sampling-constraints-0.0.6/src/sampling_constraints.egg-info/PKG-INFO
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      393 2023-05-08 23:10:35.000000 sampling-constraints-0.0.6/src/sampling_constraints.egg-info/SOURCES.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-08 23:10:35.000000 sampling-constraints-0.0.6/src/sampling_constraints.egg-info/dependency_links.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        4 2023-05-08 23:10:35.000000 sampling-constraints-0.0.6/src/sampling_constraints.egg-info/top_level.txt
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 23:10:35.127023 sampling-constraints-0.0.6/src/scs/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        0 2023-05-07 20:06:06.000000 sampling-constraints-0.0.6/src/scs/__init__.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 23:10:35.127023 sampling-constraints-0.0.6/src/scs/constraint/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      582 2023-05-07 20:17:09.000000 sampling-constraints-0.0.6/src/scs/constraint/__init__.py
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      162 2023-05-07 21:01:04.000000 sampling-constraints-0.0.6/src/scs/constraint/json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 23:10:35.127023 sampling-constraints-0.0.6/src/scs/incremental_parse/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     1240 2023-05-07 21:11:34.000000 sampling-constraints-0.0.6/src/scs/incremental_parse/__init__.py
+-rw-r--r--   0 isaac     (1000) isaac     (1000)    11444 2023-05-08 06:23:08.000000 sampling-constraints-0.0.6/src/scs/incremental_parse/json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-08 23:10:35.127023 sampling-constraints-0.0.6/tests/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     4660 2023-05-08 00:18:23.000000 sampling-constraints-0.0.6/tests/test_json.py
```

### Comparing `sampling-constraints-0.0.5/LICENSE` & `sampling-constraints-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.5/PKG-INFO` & `sampling-constraints-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampling-constraints
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library of incremental parsers used to force syntax constraints on next-token predictions during language model generation
 Author-email: Isaac Rehg <isaacrehg@gmail.com>
 Project-URL: Homepage, https://github.com/IsaacRe/Syntactically-Constrained-Sampling
 Project-URL: Bug Tracker, https://github.com/IsaacRe/Syntactically-Constrained-Sampling/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sampling-constraints-0.0.5/pyproject.toml` & `sampling-constraints-0.0.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sampling-constraints"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name = "Isaac Rehg", email = "isaacrehg@gmail.com" },
 ]
 description = "Library of incremental parsers used to force syntax constraints on next-token predictions during language model generation"
 readme = "README.md"
 requires-python = ">=3.8"
 
 [project.urls]
 "Homepage" = "https://github.com/IsaacRe/Syntactically-Constrained-Sampling"
 "Bug Tracker" = "https://github.com/IsaacRe/Syntactically-Constrained-Sampling/issues"
 
 [tool.setuptools.packages.find]
-where = ["src"]
+where = ["src"]
+
+[tool.pytest.ini_options]
+pythonpath = "src"
+addopts = [
+    "--import-mode=importlib",
+]
```

### Comparing `sampling-constraints-0.0.5/src/sampling_constraints.egg-info/PKG-INFO` & `sampling-constraints-0.0.6/src/sampling_constraints.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampling-constraints
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library of incremental parsers used to force syntax constraints on next-token predictions during language model generation
 Author-email: Isaac Rehg <isaacrehg@gmail.com>
 Project-URL: Homepage, https://github.com/IsaacRe/Syntactically-Constrained-Sampling
 Project-URL: Bug Tracker, https://github.com/IsaacRe/Syntactically-Constrained-Sampling/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sampling-constraints-0.0.5/src/scs/constraint/__init__.py` & `sampling-constraints-0.0.6/src/scs/constraint/__init__.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.5/src/scs/incremental_parse/__init__.py` & `sampling-constraints-0.0.6/src/scs/incremental_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.5/src/scs/incremental_parse/json.py` & `sampling-constraints-0.0.6/src/scs/incremental_parse/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     def __init__(self):
         super().__init__()
         self._subparser = None
         self._complete = False
 
     def _copy_from(self, other: "JSONParser"):
         super()._copy_from(other)
-        self._subparser = other._subparser.copy()
+        if other._subparser:
+            self._subparser = other._subparser.copy()
         self._complete = other._complete
     
     def _append(self, char: Union[str, SpecialToken]) -> bool:
         if self._subparser is None:
             if char == SpecialChar.OPEN_ARRAY.value:
                 self._subparser = ArrayParser()
             elif char == SpecialChar.OPEN_OBJECT.value:
```

### Comparing `sampling-constraints-0.0.5/tests/test_json.py` & `sampling-constraints-0.0.6/tests/test_json.py`

 * *Files identical despite different names*

