# Comparing `tmp/np_tools-0.1.7.tar.gz` & `tmp/np_tools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_tools-0.1.7.tar", last modified: Tue May  9 01:53:26 2023, max compression
+gzip compressed data, was "np_tools-0.1.8.tar", last modified: Tue May  9 04:41:57 2023, max compression
```

## Comparing `np_tools-0.1.7.tar` & `np_tools-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      273 2023-04-13 18:32:03.410128 np_tools-0.1.7/README.md
--rw-r--r--   0        0        0     2432 2023-05-09 01:53:26.904220 np_tools-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      300 2023-04-19 20:41:36.127176 np_tools-0.1.7/src/np_tools/__init__.py
--rw-r--r--   0        0        0      272 2023-05-08 23:52:55.568188 np_tools-0.1.7/src/np_tools/config.py
--rw-r--r--   0        0        0     8517 2023-04-19 23:59:55.459560 np_tools-0.1.7/src/np_tools/openephys.py
--rw-r--r--   0        0        0     4196 2023-04-19 20:13:12.296840 np_tools-0.1.7/src/np_tools/remote.py
--rw-r--r--   0        0        0     5842 2023-05-09 01:51:41.154598 np_tools-0.1.7/src/np_tools/tools.py
--rw-r--r--   0        0        0     2568 2023-05-09 01:48:24.111994 np_tools-0.1.7/tests/test_file_io.py
--rw-r--r--   0        0        0     1735 1970-01-01 00:00:00.000000 np_tools-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      273 2023-04-13 18:32:03.410128 np_tools-0.1.8/README.md
+-rw-r--r--   0        0        0     2432 2023-05-09 04:41:57.505773 np_tools-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-19 20:41:36.127176 np_tools-0.1.8/src/np_tools/__init__.py
+-rw-r--r--   0        0        0      272 2023-05-08 23:52:55.568188 np_tools-0.1.8/src/np_tools/config.py
+-rw-r--r--   0        0        0     8517 2023-04-19 23:59:55.459560 np_tools-0.1.8/src/np_tools/openephys.py
+-rw-r--r--   0        0        0     4196 2023-04-19 20:13:12.296840 np_tools-0.1.8/src/np_tools/remote.py
+-rw-r--r--   0        0        0     5842 2023-05-09 01:51:41.154598 np_tools-0.1.8/src/np_tools/tools.py
+-rw-r--r--   0        0        0     2293 2023-05-09 04:40:44.380440 np_tools-0.1.8/tests/test_file_io.py
+-rw-r--r--   0        0        0     1735 1970-01-01 00:00:00.000000 np_tools-0.1.8/PKG-INFO
```

### Comparing `np_tools-0.1.7/pyproject.toml` & `np_tools-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 ]
 
 [tool.coverage.report]
 show_missing = true
 
 [project]
 name = "np_tools"
-version = "0.1.7"
+version = "0.1.8"
 description = "General-purpose tools for common tasks encountered in Mindscope Neuropixels workflows."
 authors = [
     { name = "bjhardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "fabric",
     "invoke<2.1",
```

### Comparing `np_tools-0.1.7/src/np_tools/openephys.py` & `np_tools-0.1.8/src/np_tools/openephys.py`

 * *Files identical despite different names*

### Comparing `np_tools-0.1.7/src/np_tools/remote.py` & `np_tools-0.1.8/src/np_tools/remote.py`

 * *Files identical despite different names*

### Comparing `np_tools-0.1.7/src/np_tools/tools.py` & `np_tools-0.1.8/src/np_tools/tools.py`

 * *Files identical despite different names*

### Comparing `np_tools-0.1.7/PKG-INFO` & `np_tools-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: General-purpose tools for common tasks encountered in Mindscope Neuropixels workflows.
 Author-Email: bjhardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

