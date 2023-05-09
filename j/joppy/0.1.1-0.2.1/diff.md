# Comparing `tmp/joppy-0.1.1.tar.gz` & `tmp/joppy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joppy-0.1.1.tar", last modified: Sat Feb 25 09:39:19 2023, max compression
+gzip compressed data, was "joppy-0.2.1.tar", last modified: Tue May  9 13:06:41 2023, max compression
```

## Comparing `joppy-0.1.1.tar` & `joppy-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:39:19.331636 joppy-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-02-25 09:39:09.000000 joppy-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-02-25 09:39:19.331636 joppy-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-02-25 09:39:09.000000 joppy-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:39:19.331636 joppy-0.1.1/joppy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 09:39:09.000000 joppy-0.1.1/joppy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15906 2023-02-25 09:39:09.000000 joppy-0.1.1/joppy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-02-25 09:39:09.000000 joppy-0.1.1/joppy/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 09:39:09.000000 joppy-0.1.1/joppy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-25 09:39:09.000000 joppy-0.1.1/joppy/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:39:19.331636 joppy-0.1.1/joppy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-02-25 09:39:19.000000 joppy-0.1.1/joppy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-25 09:39:19.000000 joppy-0.1.1/joppy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 09:39:19.000000 joppy-0.1.1/joppy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-25 09:39:19.000000 joppy-0.1.1/joppy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-25 09:39:19.000000 joppy-0.1.1/joppy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-25 09:39:19.331636 joppy-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-25 09:39:09.000000 joppy-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:39:19.331636 joppy-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    35438 2023-02-25 09:39:09.000000 joppy-0.1.1/test/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:06:41.226225 joppy-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-09 13:06:26.000000 joppy-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-05-09 13:06:41.226225 joppy-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-05-09 13:06:26.000000 joppy-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:06:41.222224 joppy-0.2.1/joppy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:06:26.000000 joppy-0.2.1/joppy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15906 2023-05-09 13:06:26.000000 joppy-0.2.1/joppy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-05-09 13:06:26.000000 joppy-0.2.1/joppy/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:06:26.000000 joppy-0.2.1/joppy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-09 13:06:26.000000 joppy-0.2.1/joppy/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:06:41.226225 joppy-0.2.1/joppy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-05-09 13:06:41.000000 joppy-0.2.1/joppy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-09 13:06:41.000000 joppy-0.2.1/joppy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:06:41.000000 joppy-0.2.1/joppy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 13:06:41.000000 joppy-0.2.1/joppy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 13:06:41.000000 joppy-0.2.1/joppy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-09 13:06:41.226225 joppy-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-09 13:06:26.000000 joppy-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:06:41.226225 joppy-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    35532 2023-05-09 13:06:26.000000 joppy-0.2.1/test/test_api.py
```

### Comparing `joppy-0.1.1/LICENSE` & `joppy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `joppy-0.1.1/PKG-INFO` & `joppy-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: joppy
-Version: 0.1.1
+Version: 0.2.1
 Summary: Python API for Joplin
 Home-page: https://github.com/marph91/joppy
 Author: Martin Dörfelt
 Author-email: martin.d@andix.de
 License: Mozilla Public License version 2.0
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # joppy
 
 Python interface for the [Joplin data API](https://joplinapp.org/api/references/rest_api/).
 
 [![build](https://github.com/marph91/joppy/actions/workflows/build.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/build.yml)
 [![lint](https://github.com/marph91/joppy/actions/workflows/lint.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/lint.yml)
 [![tests](https://github.com/marph91/joppy/actions/workflows/tests.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/marph91/joppy/branch/master/graph/badge.svg?token=97E6IX792A)](https://codecov.io/gh/marph91/joppy)
 
-[![https://img.shields.io/badge/Joplin-2.9.17-blueviolet](https://img.shields.io/badge/Joplin-2.9.17-blueviolet)](https://github.com/laurent22/joplin)
+[![https://img.shields.io/badge/Joplin-2.10.17-blueviolet](https://img.shields.io/badge/Joplin-2.10.17-blueviolet)](https://github.com/laurent22/joplin)
 [![Python version](https://img.shields.io/pypi/pyversions/joppy.svg)](https://pypi.python.org/pypi/joppy/)
 
 ## :computer: Installation
 
 From pypi:
 
 ```bash
```

### Comparing `joppy-0.1.1/README.md` & `joppy-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Python interface for the [Joplin data API](https://joplinapp.org/api/references/rest_api/).
 
 [![build](https://github.com/marph91/joppy/actions/workflows/build.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/build.yml)
 [![lint](https://github.com/marph91/joppy/actions/workflows/lint.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/lint.yml)
 [![tests](https://github.com/marph91/joppy/actions/workflows/tests.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/marph91/joppy/branch/master/graph/badge.svg?token=97E6IX792A)](https://codecov.io/gh/marph91/joppy)
 
-[![https://img.shields.io/badge/Joplin-2.9.17-blueviolet](https://img.shields.io/badge/Joplin-2.9.17-blueviolet)](https://github.com/laurent22/joplin)
+[![https://img.shields.io/badge/Joplin-2.10.17-blueviolet](https://img.shields.io/badge/Joplin-2.10.17-blueviolet)](https://github.com/laurent22/joplin)
 [![Python version](https://img.shields.io/pypi/pyversions/joppy.svg)](https://pypi.python.org/pypi/joppy/)
 
 ## :computer: Installation
 
 From pypi:
 
 ```bash
```

### Comparing `joppy-0.1.1/joppy/api.py` & `joppy-0.2.1/joppy/api.py`

 * *Files identical despite different names*

### Comparing `joppy-0.1.1/joppy/data_types.py` & `joppy-0.2.1/joppy/data_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,20 +85,25 @@
                 "conflict_original_id",
                 "master_key_id",
                 "item_id",
             ):
                 # Exclude integer and empty string IDs.
                 if value and isinstance(value, str) and not is_id_valid(value):
                     raise ValueError("Invalid ID:", value)
-            elif field_.name.endswith("_time") or field_.name == "todo_due":
-                setattr(self, field_.name, datetime.fromtimestamp(value / 1000.0))
+            elif field_.name.endswith("_time") or field_.name in (
+                "todo_due",
+                "todo_completed",
+            ):
+                casted_value = (
+                    None if value == 0 else datetime.fromtimestamp(value / 1000.0)
+                )
+                setattr(self, field_.name, casted_value)
             elif field_.name in (
                 "is_conflict",
                 "is_todo",
-                "todo_completed",
                 "encryption_applied",
                 "is_shared",
                 "encryption_blob_encrypted",
             ):
                 setattr(self, field_.name, bool(value))
             elif field_.name == "latitude":
                 if not (-90 <= value <= 90):
@@ -147,15 +152,15 @@
     latitude: Optional[float] = None
     longitude: Optional[float] = None
     altitude: Optional[float] = None
     author: Optional[str] = None
     source_url: Optional[str] = None
     is_todo: Optional[bool] = None
     todo_due: Optional[datetime] = None
-    todo_completed: Optional[bool] = None
+    todo_completed: Optional[datetime] = None
     source: Optional[str] = None
     source_application: Optional[str] = None
     application_data: Optional[str] = None
     order: Optional[float] = None
     user_created_time: Optional[datetime] = None
     user_updated_time: Optional[datetime] = None
     encryption_cipher_text: Optional[str] = None
```

### Comparing `joppy-0.1.1/joppy.egg-info/PKG-INFO` & `joppy-0.2.1/joppy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: joppy
-Version: 0.1.1
+Version: 0.2.1
 Summary: Python API for Joplin
 Home-page: https://github.com/marph91/joppy
 Author: Martin Dörfelt
 Author-email: martin.d@andix.de
 License: Mozilla Public License version 2.0
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # joppy
 
 Python interface for the [Joplin data API](https://joplinapp.org/api/references/rest_api/).
 
 [![build](https://github.com/marph91/joppy/actions/workflows/build.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/build.yml)
 [![lint](https://github.com/marph91/joppy/actions/workflows/lint.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/lint.yml)
 [![tests](https://github.com/marph91/joppy/actions/workflows/tests.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/marph91/joppy/branch/master/graph/badge.svg?token=97E6IX792A)](https://codecov.io/gh/marph91/joppy)
 
-[![https://img.shields.io/badge/Joplin-2.9.17-blueviolet](https://img.shields.io/badge/Joplin-2.9.17-blueviolet)](https://github.com/laurent22/joplin)
+[![https://img.shields.io/badge/Joplin-2.10.17-blueviolet](https://img.shields.io/badge/Joplin-2.10.17-blueviolet)](https://github.com/laurent22/joplin)
 [![Python version](https://img.shields.io/pypi/pyversions/joppy.svg)](https://pypi.python.org/pypi/joppy/)
 
 ## :computer: Installation
 
 From pypi:
 
 ```bash
```

### Comparing `joppy-0.1.1/setup.cfg` & `joppy-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `joppy-0.1.1/test/test_api.py` & `joppy-0.2.1/test/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,20 +268,23 @@
         with self.assertRaises(ValueError):
             self.api.get_notes(notebook_id="1", tag_id="2")
 
     def test_get_notes_valid_properties(self):
         """Try to get specific properties of a note."""
         self.api.add_notebook()
         self.api.add_note()
-        # TODO: Some of the fields yield HTTP 500.
         selected_fields = dt.NoteData.fields() - {
+            # TODO: Some of the fields yield HTTP 500.
             "body_html",
             "base_url",
             "image_data_url",
             "crop_rect",
+            # todo timestamps can be None
+            "todo_due",
+            "todo_completed",
         }
         property_combinations = self.get_combinations(selected_fields)
         for properties in property_combinations:
             notes = self.api.get_notes(fields=",".join(properties))
             for note in notes.items:
                 self.assertEqual(note.assigned_fields(), set(properties))
 
@@ -838,41 +841,38 @@
         # TODO: Use "assertIsNotNone()" when
         # https://github.com/python/mypy/issues/5528 is resolved.
         assert matches is not None
         self.assertEqual(len(matches.groups()), 1)
         return matches.groups()[0]
 
     def test_get_all_notes(self):
-
         note_count = 3
         self.api.add_notebook()
         for _ in range(note_count):
             self.api.add_note()
 
         # Execute the example code. The local variables are stored in "locals_dict".
         code = self.get_example_code("get_all_notes")
         locals_dict: Mapping[str, Any] = {}
         exec(code, None, locals_dict)
 
         self.assertEqual(len(locals_dict["notes"]), note_count)
 
     def test_add_tag_to_note(self):
-
         code = self.get_example_code("add_tag_to_note")
         exec(code)
 
         tags = self.api.get_all_tags()
         self.assertEqual(len(tags), 1)
 
         assert tags[0].id is not None
         notes = self.api.get_all_notes(tag_id=tags[0].id)
         self.assertEqual(len(notes), 1)
 
     def test_add_resource_to_note(self):
-
         code = self.get_example_code("add_resource_to_note")
         code = code.replace("path/to/image.png", "test/grant_authorization_button.png")
         exec(code)
 
         notes = self.api.get_all_notes()
         self.assertEqual(len(notes), 2)
 
@@ -882,44 +882,41 @@
         # Each note should reference to exactly one resource.
         for note in notes:
             assert note.id is not None
             resources = self.api.get_all_resources(note_id=note.id)
             self.assertEqual(len(resources), 1)
 
     def test_remove_tags(self):
-
         self.api.add_tag(title="Title")
         self.api.add_tag(title="! Another Title")
         self.api.add_tag(title="!_third_title")
 
         code = self.get_example_code("remove_tags")
         exec(code)
 
         # All tags starting with "!" should be removed.
         tags = self.api.get_all_tags()
         self.assertEqual(len(tags), 1)
         self.assertEqual(tags[0].title, "title")  # tags are always lower case
 
     def test_remove_spaces_from_tags(self):
-
         self.api.add_tag(title="tag with spaces")
         self.api.add_tag(title="another tag with spaces")
 
         code = self.get_example_code("remove_spaces_from_tags")
         exec(code)
 
         all_tags = self.api.get_all_tags()
         self.assertEqual(len(all_tags), 2)
         for tag in all_tags:
             assert tag.title is not None
             self.assertNotIn(" ", tag.title)
 
     @with_resource
     def test_remove_orphaned_resources(self, filename):
-
         self.api.add_notebook()
         for i in range(2):
             note_id = self.api.add_note()
             resource_id = self.api.add_resource(
                 filename=filename, title=f"resource {i}"
             )
             self.api.add_resource_to_note(resource_id=resource_id, note_id=note_id)
```

