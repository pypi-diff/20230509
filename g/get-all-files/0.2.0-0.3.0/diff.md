# Comparing `tmp/get_all_files-0.2.0.tar.gz` & `tmp/get_all_files-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_all_files-0.2.0.tar", max compression
+gzip compressed data, was "get_all_files-0.3.0.tar", max compression
```

## Comparing `get_all_files-0.2.0.tar` & `get_all_files-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-05-08 01:12:21.808449 get_all_files-0.2.0/LICENSE
--rw-r--r--   0        0        0     2149 2023-05-08 01:12:21.808449 get_all_files-0.2.0/README.md
--rw-r--r--   0        0        0      198 2023-05-08 01:12:21.808449 get_all_files-0.2.0/get_all_files/__init__.py
--rw-r--r--   0        0        0     2958 2023-05-08 01:12:21.808449 get_all_files-0.2.0/get_all_files/_get_all_files.py
--rw-r--r--   0        0        0      644 2023-05-08 01:12:21.808449 get_all_files-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 get_all_files-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-09 04:25:39.683543 get_all_files-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2149 2023-05-09 04:25:39.683543 get_all_files-0.3.0/README.md
+-rw-r--r--   0        0        0      198 2023-05-09 04:25:39.683543 get_all_files-0.3.0/get_all_files/__init__.py
+-rw-r--r--   0        0        0     3210 2023-05-09 04:25:39.683543 get_all_files-0.3.0/get_all_files/_get_all_files.py
+-rw-r--r--   0        0        0      644 2023-05-09 04:25:39.683543 get_all_files-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2688 1970-01-01 00:00:00.000000 get_all_files-0.3.0/PKG-INFO
```

### Comparing `get_all_files-0.2.0/LICENSE` & `get_all_files-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `get_all_files-0.2.0/README.md` & `get_all_files-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `get_all_files-0.2.0/get_all_files/_get_all_files.py` & `get_all_files-0.3.0/get_all_files/_get_all_files.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,36 +25,41 @@
     """
     if isinstance(file_extensions, str):
         file_extensions = [file_extensions]
     if not isinstance(file_extensions, list):
         raise TypeError(f'file_extensions must be type str or list, not {type(file_extensions)}')
     processed_extensions = []
     for extension in file_extensions:
-        if not file_extensions[0] == '.':
+        if not extension[0] == '.':
             # handles the case where the user entered 'jpg' instead of '.jpg'
             extension = '.' + extension
         processed_extensions.append(extension)
     return processed_extensions
 
 
 def _get_all_files(path_to_data: (Path, str),
                    file_extensions: (str, list),
                    file_name: str = '*',
+                   sorted: bool = True,
                    return_absolute_filepath: bool = False) -> list:
     """
     quick script to just collect all the files in the Analysis path. Basically a wrapper around glob with (for me)
     easier to use syntax.
 
     :param path_to_data: folder where the files are
     :type path_to_data: pathlib.Path, string
     :param file_extensions: extension of files to return, e.g. 'dcm'
     :type file_extensions: str, list
     :param file_name: string to match files to; defaults to '*' which gives all files matching the extensions. set to
         e.g. 'a*' to get all files starting with a
+    :type file_name: str, optional
+    :param sorted: applys default list sorting to found files.
+    :type sorted: bool, optional
     :param return_absolute_filepath: if False (default) file names are returned; if True absolute file names returned
+    :type return_absolute_filepath: bool, optional
     :returns Files: list of all found files
     """
     # process input path:
     path_to_data = _process_input_path(path_to_data)
 
     # process extensions:
     file_extensions = _process_extensions(file_extensions)
@@ -71,8 +76,10 @@
             else:
                 head, tail = os.path.split(file)
                 Files.append(tail)
 
         if not Files:
             warnings.warn(f'\nno files matching {search_string} in {path_to_data}\n')
 
+    if sorted:
+        Files.sort()
     return Files
```

### Comparing `get_all_files-0.2.0/pyproject.toml` & `get_all_files-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "get-all-files"
-version = "0.2.0"
+version = "0.3.0"
 description = "a simple package to get all files with given file extension in a directory"
 authors = ["brendan whelan <bwheelz360@gmail.com>"]
 readme = "README.md"
 license = "LICENSE"
 packages = [{include = "get_all_files"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 flake8 = "^6.0.0"
 flake8-pyproject = "^1.2.3"
+pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.flake8]
 ignore = ["E402"]
```

### Comparing `get_all_files-0.2.0/PKG-INFO` & `get_all_files-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: get-all-files
-Version: 0.2.0
+Version: 0.3.0
 Summary: a simple package to get all files with given file extension in a directory
 License: LICENSE
 Author: brendan whelan
 Author-email: bwheelz360@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # READ ME
 
 ![tests](https://github.com/bwheelz36/get_all_files/actions/workflows/run_tests.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/get_all_files.svg)](https://badge.fury.io/py/get_all_files)
 [![codecov](https://codecov.io/gh/bwheelz36/get_all_files/branch/main/graph/badge.svg?token=CCVB5BAR8W)](https://codecov.io/gh/bwheelz36/get_all_files)
```

