# Comparing `tmp/AkvoResponseGrouper-1.3.0a0.tar.gz` & `tmp/AkvoResponseGrouper-1.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AkvoResponseGrouper-1.3.0a0.tar", last modified: Tue May  9 04:40:26 2023, max compression
+gzip compressed data, was "AkvoResponseGrouper-1.3.1a0.tar", last modified: Tue May  9 06:05:26 2023, max compression
```

## Comparing `AkvoResponseGrouper-1.3.0a0.tar` & `AkvoResponseGrouper-1.3.1a0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.237294 AkvoResponseGrouper-1.3.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/checker_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/generate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/response_grouper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-09 04:40:26.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 04:40:26.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:40:26.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 04:40:26.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 04:40:26.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 04:40:26.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/tests/test_category_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/tests/test_category_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.493058 AkvoResponseGrouper-1.3.1a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.493058 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/checker_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/generate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/response_grouper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-09 06:05:26.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 06:05:26.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:05:26.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 06:05:26.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 06:05:26.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 06:05:26.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/tests/test_category_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/tests/test_category_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/tests/test_example.py
```

### Comparing `AkvoResponseGrouper-1.3.0a0/LICENSE` & `AkvoResponseGrouper-1.3.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/PKG-INFO` & `AkvoResponseGrouper-1.3.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoResponseGrouper
-Version: 1.3.0a0
+Version: 1.3.1a0
 Summary: Fast-API Response catalog for pre-computed query
 Home-page: https://github.com/akvo/Akvo-ResponseGrouper
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-ResponseGrouper
 Project-URL: Bug Reports, https://github.com/akvo/Akvo-ResponseGrouper/issues
 Project-URL: Source Code, https://github.com/akvo/Akvo-ResponseGrouper
```

### Comparing `AkvoResponseGrouper-1.3.0a0/README.md` & `AkvoResponseGrouper-1.3.1a0/README.md`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/setup.py` & `AkvoResponseGrouper-1.3.1a0/setup.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/checker.py` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/checker.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/checker_db.py` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/checker_db.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,16 +24,15 @@
                         }
                     )
             if not check_from_db:
                 errors.append(
                     {
                         "error": "question",
                         "form": frm,
-                        "question": qs["id"],
-                        "diff": [qs["id"]],
+                        "question": qs["id"]
                     }
                 )
     return errors
 
 
 def get_error_messages(
     value: int, form: int = None, question: int = None
```

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/generate_schema.py` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/generate_schema.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/migrate.py` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/migrate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import os
 import shutil
 from sqlalchemy import create_engine
 from sqlalchemy.sql import text
 from sqlalchemy.exc import ArgumentError
 from .generate_schema import generate_schema
-from ..db import view_exist, drop_view
+from ..db import view_exist, drop_view, get_questions
 from .checker import check_config
 from .checker_db import check_questions, print_error_questions
 from ..utils import flatten_list
 
 parser = argparse.ArgumentParser("akvo-responsegrouper")
 parser.add_argument(
     "-c",
@@ -106,17 +106,22 @@
     engine = check()
     if args.config:
         errors, questions, duplicates = check_config(file_config=args.config)
         qls = flatten_list(ld=questions)
         schema = generate_schema(file_config=args.config)
         with engine.connect() as connection:
             with connection.begin():
-                error_qs = check_questions(
-                    connection=connection, questions=qls
-                )
+                error_qs = []
+                # make sure questions are available before checking
+                # the questions and options from category.json
+                gq = get_questions(connection=connection)
+                if len(gq):
+                    error_qs = check_questions(
+                        connection=connection, questions=qls
+                    )
                 if len(error_qs):
                     print_error_questions(errors=error_qs)
                 if len(errors) or len(duplicates) and not len(error_qs):
                     for dup in duplicates:
                         print(dup, "\n=======================")
                     exit(0)
                 if not len(error_qs) and not len(errors):
```

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/db.py` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,7 +59,11 @@
             options=tuple(options) if options else [],
             question=question,
             form=form,
         )
         return [d[0] for d in res.fetchall()]
     except Exception:
         return False
+
+
+def get_questions(connection):
+    return connection.execute(text("SELECT * FROM question")).fetchall()
```

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/models.py` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/models.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/routes.py` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/routes.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/conftest.py` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/utils.py` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/utils.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/views.py` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/views.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/PKG-INFO` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoResponseGrouper
-Version: 1.3.0a0
+Version: 1.3.1a0
 Summary: Fast-API Response catalog for pre-computed query
 Home-page: https://github.com/akvo/Akvo-ResponseGrouper
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-ResponseGrouper
 Project-URL: Bug Reports, https://github.com/akvo/Akvo-ResponseGrouper/issues
 Project-URL: Source Code, https://github.com/akvo/Akvo-ResponseGrouper
```

### Comparing `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt` & `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/tests/test_category_checker.py` & `AkvoResponseGrouper-1.3.1a0/tests/test_category_checker.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.0a0/tests/test_category_data_frame.py` & `AkvoResponseGrouper-1.3.1a0/tests/test_category_data_frame.py`

 * *Files identical despite different names*

