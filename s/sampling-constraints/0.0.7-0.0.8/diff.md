# Comparing `tmp/sampling-constraints-0.0.7.tar.gz` & `tmp/sampling-constraints-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampling-constraints-0.0.7.tar", last modified: Tue May  9 00:00:45 2023, max compression
+gzip compressed data, was "sampling-constraints-0.0.8.tar", last modified: Tue May  9 03:12:03 2023, max compression
```

## Comparing `sampling-constraints-0.0.7.tar` & `sampling-constraints-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 00:00:45.769673 sampling-constraints-0.0.7/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     1067 2023-05-07 21:44:12.000000 sampling-constraints-0.0.7/LICENSE
--rw-r--r--   0 isaac     (1000) isaac     (1000)      625 2023-05-09 00:00:45.769673 sampling-constraints-0.0.7/PKG-INFO
--rw-r--r--   0 isaac     (1000) isaac     (1000)      115 2023-05-08 23:11:28.000000 sampling-constraints-0.0.7/README.md
--rw-r--r--   0 isaac     (1000) isaac     (1000)      723 2023-05-08 23:23:16.000000 sampling-constraints-0.0.7/pyproject.toml
--rw-r--r--   0 isaac     (1000) isaac     (1000)       38 2023-05-09 00:00:45.769673 sampling-constraints-0.0.7/setup.cfg
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 00:00:45.769673 sampling-constraints-0.0.7/src/
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 00:00:45.769673 sampling-constraints-0.0.7/src/sampling_constraints.egg-info/
--rw-r--r--   0 isaac     (1000) isaac     (1000)      625 2023-05-09 00:00:45.000000 sampling-constraints-0.0.7/src/sampling_constraints.egg-info/PKG-INFO
--rw-r--r--   0 isaac     (1000) isaac     (1000)      393 2023-05-09 00:00:45.000000 sampling-constraints-0.0.7/src/sampling_constraints.egg-info/SOURCES.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-09 00:00:45.000000 sampling-constraints-0.0.7/src/sampling_constraints.egg-info/dependency_links.txt
--rw-r--r--   0 isaac     (1000) isaac     (1000)        4 2023-05-09 00:00:45.000000 sampling-constraints-0.0.7/src/sampling_constraints.egg-info/top_level.txt
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 00:00:45.769673 sampling-constraints-0.0.7/src/scs/
--rw-r--r--   0 isaac     (1000) isaac     (1000)        0 2023-05-07 20:06:06.000000 sampling-constraints-0.0.7/src/scs/__init__.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 00:00:45.769673 sampling-constraints-0.0.7/src/scs/constraint/
--rw-r--r--   0 isaac     (1000) isaac     (1000)      582 2023-05-07 20:17:09.000000 sampling-constraints-0.0.7/src/scs/constraint/__init__.py
--rw-r--r--   0 isaac     (1000) isaac     (1000)      162 2023-05-07 21:01:04.000000 sampling-constraints-0.0.7/src/scs/constraint/json.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 00:00:45.769673 sampling-constraints-0.0.7/src/scs/incremental_parse/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     1240 2023-05-07 21:11:34.000000 sampling-constraints-0.0.7/src/scs/incremental_parse/__init__.py
--rw-r--r--   0 isaac     (1000) isaac     (1000)    11667 2023-05-09 00:00:15.000000 sampling-constraints-0.0.7/src/scs/incremental_parse/json.py
-drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 00:00:45.769673 sampling-constraints-0.0.7/tests/
--rw-r--r--   0 isaac     (1000) isaac     (1000)     5694 2023-05-08 23:59:54.000000 sampling-constraints-0.0.7/tests/test_json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     1067 2023-05-07 21:44:12.000000 sampling-constraints-0.0.8/LICENSE
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      625 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/PKG-INFO
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      115 2023-05-08 23:11:28.000000 sampling-constraints-0.0.8/README.md
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      723 2023-05-09 03:11:57.000000 sampling-constraints-0.0.8/pyproject.toml
+-rw-r--r--   0 isaac     (1000) isaac     (1000)       38 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/setup.cfg
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.472585 sampling-constraints-0.0.8/src/
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/src/sampling_constraints.egg-info/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      625 2023-05-09 03:12:03.000000 sampling-constraints-0.0.8/src/sampling_constraints.egg-info/PKG-INFO
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      393 2023-05-09 03:12:03.000000 sampling-constraints-0.0.8/src/sampling_constraints.egg-info/SOURCES.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        1 2023-05-09 03:12:03.000000 sampling-constraints-0.0.8/src/sampling_constraints.egg-info/dependency_links.txt
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        4 2023-05-09 03:12:03.000000 sampling-constraints-0.0.8/src/sampling_constraints.egg-info/top_level.txt
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/src/scs/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)        0 2023-05-07 20:06:06.000000 sampling-constraints-0.0.8/src/scs/__init__.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/src/scs/constraint/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      582 2023-05-07 20:17:09.000000 sampling-constraints-0.0.8/src/scs/constraint/__init__.py
+-rw-r--r--   0 isaac     (1000) isaac     (1000)      162 2023-05-07 21:01:04.000000 sampling-constraints-0.0.8/src/scs/constraint/json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/src/scs/incremental_parse/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     1240 2023-05-07 21:11:34.000000 sampling-constraints-0.0.8/src/scs/incremental_parse/__init__.py
+-rw-r--r--   0 isaac     (1000) isaac     (1000)    11908 2023-05-09 02:43:26.000000 sampling-constraints-0.0.8/src/scs/incremental_parse/json.py
+drwxr-xr-x   0 isaac     (1000) isaac     (1000)        0 2023-05-09 03:12:03.482581 sampling-constraints-0.0.8/tests/
+-rw-r--r--   0 isaac     (1000) isaac     (1000)     6133 2023-05-09 02:41:23.000000 sampling-constraints-0.0.8/tests/test_json.py
```

### Comparing `sampling-constraints-0.0.7/LICENSE` & `sampling-constraints-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.7/PKG-INFO` & `sampling-constraints-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampling-constraints
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library of incremental parsers used to force syntax constraints on next-token predictions during language model generation
 Author-email: Isaac Rehg <isaacrehg@gmail.com>
 Project-URL: Homepage, https://github.com/IsaacRe/Syntactically-Constrained-Sampling
 Project-URL: Bug Tracker, https://github.com/IsaacRe/Syntactically-Constrained-Sampling/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sampling-constraints-0.0.7/pyproject.toml` & `sampling-constraints-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sampling-constraints"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name = "Isaac Rehg", email = "isaacrehg@gmail.com" },
 ]
 description = "Library of incremental parsers used to force syntax constraints on next-token predictions during language model generation"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `sampling-constraints-0.0.7/src/sampling_constraints.egg-info/PKG-INFO` & `sampling-constraints-0.0.8/src/sampling_constraints.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampling-constraints
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library of incremental parsers used to force syntax constraints on next-token predictions during language model generation
 Author-email: Isaac Rehg <isaacrehg@gmail.com>
 Project-URL: Homepage, https://github.com/IsaacRe/Syntactically-Constrained-Sampling
 Project-URL: Bug Tracker, https://github.com/IsaacRe/Syntactically-Constrained-Sampling/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sampling-constraints-0.0.7/src/scs/constraint/__init__.py` & `sampling-constraints-0.0.8/src/scs/constraint/__init__.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.7/src/scs/incremental_parse/__init__.py` & `sampling-constraints-0.0.8/src/scs/incremental_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `sampling-constraints-0.0.7/src/scs/incremental_parse/json.py` & `sampling-constraints-0.0.8/src/scs/incremental_parse/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,16 @@
         if isinstance(self._active_subparser, NumberParser) and not self._active_subparser.closing_char.isspace():
             # infer current parse state based on how number parser was terminated
             self._parsed += self._active_subparser.closing_char
             if self._active_subparser.closing_char == SpecialChar.COMMA.value:
                 self._parse_status = ObjectParseStatus.AWAITING_KEY
             elif self._active_subparser.closing_char == SpecialChar.CLOSE_OBJECT.value:
                 self._parse_status = ObjectParseStatus.PARSE_COMPLETE
+            else:
+                raise ParseFailure(f"Expected ',' or '}}', got {self._active_subparser.closing_char}")
         elif self._parse_status == ObjectParseStatus.IN_VALUE_SUBPARSER:
             self._parse_status = ObjectParseStatus.FINISHED_VALUE
         else:
             self._parse_status = ObjectParseStatus.FINISHED_KEY
         self._active_subparser = None
 
     def _append(self, char: str) -> bool:
@@ -170,14 +172,16 @@
         if isinstance(self._active_subparser, NumberParser) and not self._active_subparser.closing_char.isspace():
             # infer current parse state based on how number parsing was terminated
             self._parsed += self._active_subparser.closing_char
             if self._active_subparser.closing_char == SpecialChar.COMMA.value:
                 self._parse_status = ObjectParseStatus.AWAITING_VALUE
             elif self._active_subparser.closing_char == SpecialChar.CLOSE_ARRAY.value:
                 self._parse_status = ObjectParseStatus.PARSE_COMPLETE
+            else:
+                raise ParseFailure(f"Expected ',' or ']', got {self._active_subparser.closing_char}")
         else:
             self._parse_status = ObjectParseStatus.FINISHED_VALUE
         self._active_subparser = None
 
     def _append(self, char: str) -> bool:
         if self._parse_status == ObjectParseStatus.IN_VALUE_SUBPARSER:
             done = self._active_subparser._append(char)
```

### Comparing `sampling-constraints-0.0.7/tests/test_json.py` & `sampling-constraints-0.0.8/tests/test_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,14 +99,26 @@
             parser.append(test_data)
 
     def test_parse_array_with_extra(self):
         parser = JSONParser()
         test_data = list('["apple", "banana", "cherry"]') + list("extra data")
         with self.assertRaises(ParseFailure):
             parser.append(test_data)
+
+    def test_parse_object_with_space_after_number(self):
+        parser = JSONParser()
+        test_data = list('{"name": "John Smith", "age": 35]')
+        with self.assertRaises(ParseFailure):
+            parser.append(test_data)
+
+    def test_parse_invalid_array_close_after_number(self):
+        parser = JSONParser()
+        test_data = list('[35}')
+        with self.assertRaises(ParseFailure):
+            parser.append(test_data)
         
 
 class TestJSONConstraint(unittest.TestCase):
 
     def test_update_parser(self):
         test_data = '{"name": "John Smith", "ag', 'e": 35, "city": "New York"}'
         constraint = valid_json()
```

