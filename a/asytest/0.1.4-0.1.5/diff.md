# Comparing `tmp/asytest-0.1.4.tar.gz` & `tmp/asytest-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asytest-0.1.4.tar", last modified: Thu May  4 13:26:35 2023, max compression
+gzip compressed data, was "asytest-0.1.5.tar", last modified: Tue May  9 06:53:14 2023, max compression
```

## Comparing `asytest-0.1.4.tar` & `asytest-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.181889 asytest-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.173889 asytest-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.177889 asytest-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-04 13:26:20.000000 asytest-0.1.4/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-04 13:26:20.000000 asytest-0.1.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-04 13:26:20.000000 asytest-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 13:26:20.000000 asytest-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-04 13:26:35.181889 asytest-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-04 13:26:20.000000 asytest-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-04 13:26:20.000000 asytest-0.1.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.177889 asytest-0.1.4/example_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-04 13:26:20.000000 asytest-0.1.4/example_tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-04 13:26:20.000000 asytest-0.1.4/example_tests/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-04 13:26:20.000000 asytest-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-04 13:26:20.000000 asytest-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:26:35.181889 asytest-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.173889 asytest-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.177889 asytest-0.1.4/src/asytest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:20.000000 asytest-0.1.4/src/asytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-04 13:26:20.000000 asytest-0.1.4/src/asytest/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 13:26:35.000000 asytest-0.1.4/src/asytest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-05-04 13:26:20.000000 asytest-0.1.4/src/asytest/asytest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.181889 asytest-0.1.4/src/asytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-04 13:26:35.000000 asytest-0.1.4/src/asytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-04 13:26:35.000000 asytest-0.1.4/src/asytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:26:35.000000 asytest-0.1.4/src/asytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-04 13:26:35.000000 asytest-0.1.4/src/asytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 13:26:35.000000 asytest-0.1.4/src/asytest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.181889 asytest-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-04 13:26:20.000000 asytest-0.1.4/tests/test_asytest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:14.161157 asytest-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:14.157157 asytest-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:14.157157 asytest-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-09 06:52:51.000000 asytest-0.1.5/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-09 06:52:51.000000 asytest-0.1.5/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-09 06:52:51.000000 asytest-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-09 06:52:51.000000 asytest-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-09 06:53:14.161157 asytest-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-09 06:52:51.000000 asytest-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-09 06:52:51.000000 asytest-0.1.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:14.157157 asytest-0.1.5/example_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-09 06:52:51.000000 asytest-0.1.5/example_tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-09 06:52:51.000000 asytest-0.1.5/example_tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 06:52:51.000000 asytest-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 06:52:51.000000 asytest-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 06:53:14.161157 asytest-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:14.157157 asytest-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:14.157157 asytest-0.1.5/src/asytest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:52:51.000000 asytest-0.1.5/src/asytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-09 06:52:51.000000 asytest-0.1.5/src/asytest/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 06:53:14.000000 asytest-0.1.5/src/asytest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-05-09 06:52:51.000000 asytest-0.1.5/src/asytest/asytest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:14.161157 asytest-0.1.5/src/asytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-09 06:53:14.000000 asytest-0.1.5/src/asytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-09 06:53:14.000000 asytest-0.1.5/src/asytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:53:14.000000 asytest-0.1.5/src/asytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 06:53:14.000000 asytest-0.1.5/src/asytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 06:53:14.000000 asytest-0.1.5/src/asytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:14.161157 asytest-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-09 06:52:51.000000 asytest-0.1.5/tests/test_asytest.py
```

### Comparing `asytest-0.1.4/.github/workflows/build.yaml` & `asytest-0.1.5/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `asytest-0.1.4/.github/workflows/release.yaml` & `asytest-0.1.5/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `asytest-0.1.4/LICENSE` & `asytest-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asytest-0.1.4/PKG-INFO` & `asytest-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asytest
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tiny async test framework for python 
 Author: Pavel Rabetski
 Project-URL: Homepage, https://github.com/pavradev/asytest
 Project-URL: Bug Tracker, https://github.com/pavradev/asytest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asytest-0.1.4/dev-requirements.txt` & `asytest-0.1.5/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `asytest-0.1.4/example_tests/test_concurrent.py` & `asytest-0.1.5/example_tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `asytest-0.1.4/pyproject.toml` & `asytest-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asytest-0.1.4/src/asytest/asytest.py` & `asytest-0.1.5/src/asytest/asytest.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     print(format_line(" TEST RESULTS "))
     for result in test_results:
         exec_time_formatted = "{:.1f}".format(result.exec_time)
         name = result.name
         module = result.module
         status = result.status.value
         color = "\033[92m" if status == "SUCCESS" else "\033[91m"
-        print(f"{module}::{name} {color}{status:<10}\033[0m [{exec_time_formatted}s]")
+        print(f"[{exec_time_formatted}s]\t{module}::{name} {color}{status:<10}\033[0m")
     print()
 
 def print_summary(result: TestSuiteResult) -> None:
     """
     Prints a summary of the test suite result to stdout.
 
     Args:
@@ -245,8 +245,8 @@
     parser.add_argument(
         "-n",
         "--max-concurrent",
         type=int,
         default=10,
         help="Maximum number of tests to run concurrently",
     )
-    return parser.parse_args()
+    return parser.parse_args()
```

### Comparing `asytest-0.1.4/src/asytest.egg-info/PKG-INFO` & `asytest-0.1.5/src/asytest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asytest
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tiny async test framework for python 
 Author: Pavel Rabetski
 Project-URL: Homepage, https://github.com/pavradev/asytest
 Project-URL: Bug Tracker, https://github.com/pavradev/asytest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asytest-0.1.4/tests/test_asytest.py` & `asytest-0.1.5/tests/test_asytest.py`

 * *Files identical despite different names*

