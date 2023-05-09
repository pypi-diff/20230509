# Comparing `tmp/AkvoResponseGrouper-1.2.9a0.tar.gz` & `tmp/AkvoResponseGrouper-1.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AkvoResponseGrouper-1.2.9a0.tar", last modified: Thu Apr 20 05:41:51 2023, max compression
+gzip compressed data, was "AkvoResponseGrouper-1.3.0a0.tar", last modified: Tue May  9 04:40:26 2023, max compression
```

## Comparing `AkvoResponseGrouper-1.2.9a0.tar` & `AkvoResponseGrouper-1.3.0a0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.565846 AkvoResponseGrouper-1.2.9a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/checker_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/generate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/response_grouper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-20 05:41:51.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 05:41:51.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 05:41:51.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 05:41:51.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 05:41:51.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 05:41:51.000000 AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:41:51.569846 AkvoResponseGrouper-1.2.9a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/tests/test_category_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/tests/test_category_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 05:41:40.000000 AkvoResponseGrouper-1.2.9a0/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.237294 AkvoResponseGrouper-1.3.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/checker_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/generate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/response_grouper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-09 04:40:26.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 04:40:26.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:40:26.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 04:40:26.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 04:40:26.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 04:40:26.000000 AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:40:26.241294 AkvoResponseGrouper-1.3.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/tests/test_category_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/tests/test_category_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-09 04:40:14.000000 AkvoResponseGrouper-1.3.0a0/tests/test_example.py
```

### Comparing `AkvoResponseGrouper-1.2.9a0/LICENSE` & `AkvoResponseGrouper-1.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/PKG-INFO` & `AkvoResponseGrouper-1.3.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoResponseGrouper
-Version: 1.2.9a0
+Version: 1.3.0a0
 Summary: Fast-API Response catalog for pre-computed query
 Home-page: https://github.com/akvo/Akvo-ResponseGrouper
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-ResponseGrouper
 Project-URL: Bug Reports, https://github.com/akvo/Akvo-ResponseGrouper/issues
 Project-URL: Source Code, https://github.com/akvo/Akvo-ResponseGrouper
```

### Comparing `AkvoResponseGrouper-1.2.9a0/README.md` & `AkvoResponseGrouper-1.3.0a0/README.md`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/setup.py` & `AkvoResponseGrouper-1.3.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/checker.py` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/checker.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/checker_db.py` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/checker_db.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 import itertools
-from ..db import get_option_by_questions
+from ..db import validate_question_options
 
 
-def check_options(rows, questions: list) -> list:
+def check_questions(connection, questions: list) -> list:
     errors = []
-    ls = [{"question": row["qid"], "option": row["name"]} for row in rows]
-    for key, group in itertools.groupby(ls, key=lambda x: x["question"]):
-        options = [o["option"] for o in list(group) if o["option"] is not None]
-        fq = list(filter(lambda x: x["id"] == key, questions))
-        if len(fq) and len(options):
-            cg_items = set(fq[0]["options"])
-            db_items = set(options)
-            isec = set.intersection(cg_items, db_items)
-            diff = list(cg_items - isec)
-            if len(diff):
+    for frm, qs in itertools.groupby(questions, key=lambda x: x["form"]):
+        for qs in list(qs):
+            check_from_db = validate_question_options(
+                connection=connection,
+                options=qs["options"],
+                question=qs["id"],
+                form=frm,
+            )
+            if check_from_db and qs["options"]:
+                diff = set.difference(set(qs["options"]), set(check_from_db))
+                if len(diff):
+                    errors.append(
+                        {
+                            "error": "options",
+                            "form": frm,
+                            "question": qs["id"],
+                            "diff": diff,
+                        }
+                    )
+            if not check_from_db:
                 errors.append(
                     {
-                        "error": "options",
-                        "form": fq[0]["form"],
-                        "question": fq[0]["id"],
-                        "diff": diff,
+                        "error": "question",
+                        "form": frm,
+                        "question": qs["id"],
+                        "diff": [qs["id"]],
                     }
                 )
     return errors
 
 
-def check_questions(connection, questions: list) -> list:
-    errors = []
-    for frm, qs in itertools.groupby(questions, key=lambda x: x["form"]):
-        lqs = list(qs)
-        ids = [q["id"] for q in lqs]
-        res = get_option_by_questions(connection=connection, questions=ids)
-        if res:
-            dbqs = list(set([lt["qid"] for lt in list(res)]))
-            diff = list(set(ids) - set(dbqs))
-            if len(diff):
-                errors.append({"error": "question", "diff": diff})
-            errors += check_options(rows=res, questions=lqs)
-    return errors
-
-
 def get_error_messages(
     value: int, form: int = None, question: int = None
 ) -> str:
     msg = f"QUESTION: {value} not found"
     if form and question:
         msg = (
             f"OPTION : {value} is not part of FORM: {form} | QUESTION:"
```

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/generate_schema.py` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/generate_schema.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/cli/migrate.py` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/db.py` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/db.py`

 * *Files 25% similar despite different names*

```diff
@@ -32,21 +32,34 @@
         return engine.has_table(table_name="ar_category")
 
 
 def drop_view(connection):
     return connection.execute(text("DROP MATERIALIZED VIEW ar_category"))
 
 
-def get_option_by_questions(connection, questions: list):
+def validate_question_options(
+    connection, question, form, options: list = None
+):
     try:
         query = text(
-            "select option.*, question.id as qid, question.form as form"
-            " from option "
-            + "right join question on option.question = question.id "
-            + "where question.id in :questions"
+            "SELECT COUNT(*) as count FROM question "
+            + "where id = :question AND "
+            + "form = :form"
         )
-        return connection.execute(
+        if options:
+            query = text(
+                "SELECT option.name FROM option "
+                "JOIN question ON option.question = question.id "
+                + "where option.name IN :options AND "
+                + "option.question = :question AND "
+                + "question.form = :form"
+            )
+
+        res = connection.execute(
             query,
-            questions=tuple(questions),
-        ).fetchall()
+            options=tuple(options) if options else [],
+            question=question,
+            form=form,
+        )
+        return [d[0] for d in res.fetchall()]
     except Exception:
-        return None
+        return False
```

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/models.py` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/models.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/routes.py` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/routes.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/conftest.py` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/utils.py` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/utils.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper/views.py` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper/views.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/PKG-INFO` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoResponseGrouper
-Version: 1.2.9a0
+Version: 1.3.0a0
 Summary: Fast-API Response catalog for pre-computed query
 Home-page: https://github.com/akvo/Akvo-ResponseGrouper
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-ResponseGrouper
 Project-URL: Bug Reports, https://github.com/akvo/Akvo-ResponseGrouper/issues
 Project-URL: Source Code, https://github.com/akvo/Akvo-ResponseGrouper
```

### Comparing `AkvoResponseGrouper-1.2.9a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt` & `AkvoResponseGrouper-1.3.0a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/tests/test_category_checker.py` & `AkvoResponseGrouper-1.3.0a0/tests/test_category_checker.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.2.9a0/tests/test_category_data_frame.py` & `AkvoResponseGrouper-1.3.0a0/tests/test_category_data_frame.py`

 * *Files identical despite different names*

