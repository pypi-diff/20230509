# Comparing `tmp/np_tools-0.1.6.tar.gz` & `tmp/np_tools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_tools-0.1.6.tar", last modified: Tue May  2 16:22:57 2023, max compression
+gzip compressed data, was "np_tools-0.1.7.tar", last modified: Tue May  9 01:53:26 2023, max compression
```

## Comparing `np_tools-0.1.6.tar` & `np_tools-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      273 2023-04-13 18:32:03.410128 np_tools-0.1.6/README.md
--rw-r--r--   0        0        0     2407 2023-05-02 16:22:57.834073 np_tools-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      300 2023-04-19 20:41:36.127176 np_tools-0.1.6/src/np_tools/__init__.py
--rw-r--r--   0        0        0      268 2023-04-13 18:53:25.697520 np_tools-0.1.6/src/np_tools/config.py
--rw-r--r--   0        0        0     8517 2023-04-19 23:59:55.459560 np_tools-0.1.6/src/np_tools/openephys.py
--rw-r--r--   0        0        0     4196 2023-04-19 20:13:12.296840 np_tools-0.1.6/src/np_tools/remote.py
--rw-r--r--   0        0        0     4056 2023-04-25 20:24:36.073231 np_tools-0.1.6/src/np_tools/tools.py
--rw-r--r--   0        0        0     1702 1970-01-01 00:00:00.000000 np_tools-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      273 2023-04-13 18:32:03.410128 np_tools-0.1.7/README.md
+-rw-r--r--   0        0        0     2432 2023-05-09 01:53:26.904220 np_tools-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-19 20:41:36.127176 np_tools-0.1.7/src/np_tools/__init__.py
+-rw-r--r--   0        0        0      272 2023-05-08 23:52:55.568188 np_tools-0.1.7/src/np_tools/config.py
+-rw-r--r--   0        0        0     8517 2023-04-19 23:59:55.459560 np_tools-0.1.7/src/np_tools/openephys.py
+-rw-r--r--   0        0        0     4196 2023-04-19 20:13:12.296840 np_tools-0.1.7/src/np_tools/remote.py
+-rw-r--r--   0        0        0     5842 2023-05-09 01:51:41.154598 np_tools-0.1.7/src/np_tools/tools.py
+-rw-r--r--   0        0        0     2568 2023-05-09 01:48:24.111994 np_tools-0.1.7/tests/test_file_io.py
+-rw-r--r--   0        0        0     1735 1970-01-01 00:00:00.000000 np_tools-0.1.7/PKG-INFO
```

### Comparing `np_tools-0.1.6/pyproject.toml` & `np_tools-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -71,24 +71,25 @@
 ]
 
 [tool.coverage.report]
 show_missing = true
 
 [project]
 name = "np_tools"
-version = "0.1.6"
+version = "0.1.7"
 description = "General-purpose tools for common tasks encountered in Mindscope Neuropixels workflows."
 authors = [
     { name = "bjhardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "fabric",
     "invoke<2.1",
     "np-config>=0.4.17",
     "np-logging>=0.5.1",
+    "crc32c>=2.3.post0",
 ]
 requires-python = ">=3.7,<4"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `np_tools-0.1.6/src/np_tools/openephys.py` & `np_tools-0.1.7/src/np_tools/openephys.py`

 * *Files identical despite different names*

### Comparing `np_tools-0.1.6/src/np_tools/remote.py` & `np_tools-0.1.7/src/np_tools/remote.py`

 * *Files identical despite different names*

### Comparing `np_tools-0.1.6/PKG-INFO` & `np_tools-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-tools
-Version: 0.1.6
+Version: 0.1.7
 Summary: General-purpose tools for common tasks encountered in Mindscope Neuropixels workflows.
 Author-Email: bjhardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,14 +16,15 @@
 Project-URL: Repository, https://github.com/AllenInstitute/np_tools
 Project-URL: Bug tracker, https://github.com/AllenInstitute/np_tools/issues
 Requires-Python: <4,>=3.7
 Requires-Dist: fabric
 Requires-Dist: invoke<2.1
 Requires-Dist: np-config>=0.4.17
 Requires-Dist: np-logging>=0.5.1
+Requires-Dist: crc32c>=2.3.post0
 Requires-Dist: blue>=0.9.1; extra == "dev"
 Requires-Dist: pytest>=7.2.2; extra == "dev"
 Requires-Dist: mypy>=1.1.1; extra == "dev"
 Requires-Dist: coverage[toml]>=7.2.2; extra == "dev"
 Requires-Dist: pdm>=2.4.9; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
 Requires-Dist: bump>=1.3.2; extra == "dev"
```

