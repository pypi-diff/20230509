# Comparing `tmp/enhancedocs-0.5.5.tar.gz` & `tmp/enhancedocs-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhancedocs-0.5.5.tar", max compression
+gzip compressed data, was "enhancedocs-0.5.6.tar", max compression
```

## Comparing `enhancedocs-0.5.5.tar` & `enhancedocs-0.5.6.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0    11341 2023-05-06 12:36:54.418693 enhancedocs-0.5.5/LICENSE
--rw-r--r--   0        0        0     1030 2023-05-06 12:36:54.418693 enhancedocs-0.5.5/README.md
--rw-r--r--   0        0        0      474 2023-05-06 12:36:54.418693 enhancedocs-0.5.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-06 12:36:54.418693 enhancedocs-0.5.5/src/enhancedocs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 12:36:54.418693 enhancedocs-0.5.5/src/enhancedocs/commands/__init__.py
--rw-r--r--   0        0        0     2802 2023-05-06 12:36:54.418693 enhancedocs-0.5.5/src/enhancedocs/commands/ask.py
--rw-r--r--   0        0        0     1315 2023-05-06 12:36:54.418693 enhancedocs-0.5.5/src/enhancedocs/commands/build.py
--rw-r--r--   0        0        0     1842 2023-05-06 12:36:54.418693 enhancedocs-0.5.5/src/enhancedocs/commands/push.py
--rw-r--r--   0        0        0     1151 2023-05-06 12:36:54.418693 enhancedocs-0.5.5/src/enhancedocs/config.py
--rw-r--r--   0        0        0      611 2023-05-06 12:36:54.418693 enhancedocs-0.5.5/src/enhancedocs/main.py
--rw-r--r--   0        0        0     1212 2023-05-06 12:36:54.418693 enhancedocs-0.5.5/src/enhancedocs/utils.py
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 enhancedocs-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-05-09 17:22:36.892544 enhancedocs-0.5.6/LICENSE
+-rw-r--r--   0        0        0     1030 2023-05-09 17:22:36.892544 enhancedocs-0.5.6/README.md
+-rw-r--r--   0        0        0      474 2023-05-09 17:22:36.892544 enhancedocs-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 17:22:36.892544 enhancedocs-0.5.6/src/enhancedocs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 17:22:36.892544 enhancedocs-0.5.6/src/enhancedocs/commands/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-09 17:22:36.892544 enhancedocs-0.5.6/src/enhancedocs/commands/alpha/__init__.py
+-rw-r--r--   0        0        0      148 2023-05-09 17:22:36.892544 enhancedocs-0.5.6/src/enhancedocs/commands/alpha/projects/__init__.py
+-rw-r--r--   0        0        0     1645 2023-05-09 17:22:36.892544 enhancedocs-0.5.6/src/enhancedocs/commands/alpha/projects/create.py
+-rw-r--r--   0        0        0     2802 2023-05-09 17:22:36.892544 enhancedocs-0.5.6/src/enhancedocs/commands/ask.py
+-rw-r--r--   0        0        0     1315 2023-05-09 17:22:36.892544 enhancedocs-0.5.6/src/enhancedocs/commands/build.py
+-rw-r--r--   0        0        0     1842 2023-05-09 17:22:36.892544 enhancedocs-0.5.6/src/enhancedocs/commands/push.py
+-rw-r--r--   0        0        0     1151 2023-05-09 17:22:36.892544 enhancedocs-0.5.6/src/enhancedocs/config.py
+-rw-r--r--   0        0        0      481 2023-05-09 17:22:36.892544 enhancedocs-0.5.6/src/enhancedocs/main.py
+-rw-r--r--   0        0        0     1447 2023-05-09 17:22:36.896544 enhancedocs-0.5.6/src/enhancedocs/utils.py
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 enhancedocs-0.5.6/PKG-INFO
```

### Comparing `enhancedocs-0.5.5/LICENSE` & `enhancedocs-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.5/README.md` & `enhancedocs-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.5/src/enhancedocs/commands/ask.py` & `enhancedocs-0.5.6/src/enhancedocs/commands/ask.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.5/src/enhancedocs/commands/build.py` & `enhancedocs-0.5.6/src/enhancedocs/commands/build.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.5/src/enhancedocs/commands/push.py` & `enhancedocs-0.5.6/src/enhancedocs/commands/push.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.5/src/enhancedocs/config.py` & `enhancedocs-0.5.6/src/enhancedocs/config.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.5/src/enhancedocs/utils.py` & `enhancedocs-0.5.6/src/enhancedocs/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import click
+from .config import ENVIRONMENT_VARIABLES_HELP
 from pathspec import PathSpec
 from pathspec.patterns import GitWildMatchPattern
 
 
 def find_gitignore_files(dir_path):
     gitignore_files = []
     for entry in os.scandir(dir_path):
@@ -27,7 +29,13 @@
     for entry in os.scandir(dir_path):
         entry_path = os.path.join(dir_path, entry.name)
         if entry.is_file() and not ignore_spec.match_file(entry_path):
             files_list.append(entry_path)
         elif entry.is_dir():
             files_list.extend(get_files(entry_path, ignore_spec))
     return files_list
+
+
+class CustomHelpGroup(click.Group):
+    def get_help(self, ctx):
+        default_help = super().get_help(ctx)
+        return f"{default_help}\n{ENVIRONMENT_VARIABLES_HELP}"
```

### Comparing `enhancedocs-0.5.5/PKG-INFO` & `enhancedocs-0.5.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhancedocs
-Version: 0.5.5
+Version: 0.5.6
 Summary: EnhanceDocs Command Line Interface (CLI)
 License: Apache-2.0
 Author: Alvaro Molina
 Author-email: alw3ys@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

