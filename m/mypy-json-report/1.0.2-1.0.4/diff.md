# Comparing `tmp/mypy_json_report-1.0.2.tar.gz` & `tmp/mypy_json_report-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_json_report-1.0.2.tar", max compression
+gzip compressed data, was "mypy_json_report-1.0.4.tar", max compression
```

## Comparing `mypy_json_report-1.0.2.tar` & `mypy_json_report-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10702 2023-04-10 22:00:28.927009 mypy_json_report-1.0.2/LICENSE
--rw-r--r--   0        0        0     2331 2023-04-10 22:00:28.927009 mypy_json_report-1.0.2/README.md
--rw-r--r--   0        0        0     9626 2023-04-10 22:00:28.927009 mypy_json_report-1.0.2/mypy_json_report.py
--rw-r--r--   0        0        0     1300 2023-04-10 22:00:28.927009 mypy_json_report-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 mypy_json_report-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    10702 2023-05-09 09:12:14.895967 mypy_json_report-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2331 2023-05-09 09:12:14.895967 mypy_json_report-1.0.4/README.md
+-rw-r--r--   0        0        0     9630 2023-05-09 09:12:14.895967 mypy_json_report-1.0.4/mypy_json_report.py
+-rw-r--r--   0        0        0     1490 2023-05-09 09:12:14.895967 mypy_json_report-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 mypy_json_report-1.0.4/PKG-INFO
```

### Comparing `mypy_json_report-1.0.2/LICENSE` & `mypy_json_report-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_json_report-1.0.2/README.md` & `mypy_json_report-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mypy_json_report-1.0.2/mypy_json_report.py` & `mypy_json_report-1.0.4/mypy_json_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         message_group = list(messages)
         for processor in processors:
             processor.process_messages(filename, message_group)
 
     for processor in processors:
         error_code = processor.write_report()
         if error_code is not None:
-            exit(error_code)
+            sys.exit(error_code)
 
 
 def _no_command(args: argparse.Namespace) -> None:
     """
     Handle the lack of an explicit command.
 
     This will be hit when the program is called without arguments.
```

### Comparing `mypy_json_report-1.0.2/pyproject.toml` & `mypy_json_report-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mypy-json-report"
-version = "1.0.2"
+version = "1.0.4"
 description = "Generate a JSON report from your mypy output"
 authors = ["Charlie Denton <charlie@meshy.co.uk>"]
 license = "Apache-2.0"
 repository = "https://github.com/memrise/mypy-json-report"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
@@ -13,14 +13,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development",
     "Topic :: Utilities",
 ]
 
 [project.urls]
 Source = "https://github.com/memrise/mypy-json-report"
 
@@ -36,12 +37,23 @@
 [tool.poetry.scripts]
 mypy-json-report = "mypy_json_report:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.isort]
-combine_as_imports = true
-known_first_party = ["mypy_json_report"]
-lines_after_imports = 2
-profile = "black"
+[tool.ruff]
+target-version = "py37"
+select = [
+    "E",  # pycodestyle
+    "F",  # Pyflakes
+    "I",  # isort
+    "PL",  # Pylint
+    "UP",  # pyupgrade
+]
+ignore = [
+    "E501",  # Line too long
+]
+
+[tool.ruff.isort]
+combine-as-imports = true
+lines-after-imports = 2
```

### Comparing `mypy_json_report-1.0.2/PKG-INFO` & `mypy_json_report-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy-json-report
-Version: 1.0.2
+Version: 1.0.4
 Summary: Generate a JSON report from your mypy output
 Home-page: https://github.com/memrise/mypy-json-report
 License: Apache-2.0
 Author: Charlie Denton
 Author-email: charlie@meshy.co.uk
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Project-URL: Repository, https://github.com/memrise/mypy-json-report
 Description-Content-Type: text/markdown
```

