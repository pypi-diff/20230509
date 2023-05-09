# Comparing `tmp/khloraascaf-1.7.0.tar.gz` & `tmp/khloraascaf-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf-1.7.0.tar", last modified: Mon May  8 18:23:05 2023, max compression
+gzip compressed data, was "khloraascaf-1.7.1.tar", last modified: Tue May  9 00:52:19 2023, max compression
```

## Comparing `khloraascaf-1.7.0.tar` & `khloraascaf-1.7.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:23:05.330433 khloraascaf-1.7.0/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/LICENCE
--rw-r--r--   0 root         (0) root         (0)    46361 2023-05-08 18:23:05.329433 khloraascaf-1.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4981 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1339 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 18:23:05.330433 khloraascaf-1.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:23:05.312432 khloraascaf-1.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:23:05.320433 khloraascaf-1.7.0/src/khloraascaf/
--rw-rw-rw-   0 root         (0) root         (0)     1579 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1760 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    13402 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     5619 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5600 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:23:05.326433 khloraascaf-1.7.0/src/khloraascaf/ilp/
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11068 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/dirf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)    10725 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/invf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)     4901 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_circuit.py
--rw-rw-rw-   0 root         (0) root         (0)     3418 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_max_dirf.py
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_max_invf.py
--rw-rw-rw-   0 root         (0) root         (0)     3738 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_max_presscore.py
--rw-rw-rw-   0 root         (0) root         (0)    12009 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_repeated_fragments.py
--rw-rw-rw-   0 root         (0) root         (0)     3027 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_to_solver.py
--rw-rw-rw-   0 root         (0) root         (0)    10512 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_var_db.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/lib.py
--rw-rw-rw-   0 root         (0) root         (0)    12867 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/multiplied_doubled_contig_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     8323 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    21836 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/result.py
--rw-rw-rw-   0 root         (0) root         (0)    28116 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/run_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    21539 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/scaffolding_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     7160 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/utils_debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:23:05.322433 khloraascaf-1.7.0/src/khloraascaf.egg-info/
--rw-r--r--   0 root         (0) root         (0)    46361 2023-05-08 18:23:05.000000 khloraascaf-1.7.0/src/khloraascaf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1174 2023-05-08 18:23:05.000000 khloraascaf-1.7.0/src/khloraascaf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 18:23:05.000000 khloraascaf-1.7.0/src/khloraascaf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-08 18:23:05.000000 khloraascaf-1.7.0/src/khloraascaf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-08 18:23:05.000000 khloraascaf-1.7.0/src/khloraascaf.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:23:05.329433 khloraascaf-1.7.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13219 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/tests/test_assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/tests/test_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)    14876 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/tests/test_run_metdata.py
--rw-rw-rw-   0 root         (0) root         (0)    22601 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/tests/test_toy_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     2989 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/tests/test_utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 00:52:19.934183 khloraascaf-1.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    46361 2023-05-09 00:52:19.933183 khloraascaf-1.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4981 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 00:52:19.934183 khloraascaf-1.7.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 00:52:19.917186 khloraascaf-1.7.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 00:52:19.924185 khloraascaf-1.7.1/src/khloraascaf/
+-rw-rw-rw-   0 root         (0) root         (0)     1579 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13402 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5619 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5600 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 00:52:19.930184 khloraascaf-1.7.1/src/khloraascaf/ilp/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11068 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/dirf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)    10725 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/invf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)     4901 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3418 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_max_dirf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_max_invf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_max_presscore.py
+-rw-rw-rw-   0 root         (0) root         (0)    12009 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_repeated_fragments.py
+-rw-rw-rw-   0 root         (0) root         (0)     3027 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_to_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)    10512 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_var_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12867 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/multiplied_doubled_contig_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     8323 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    21863 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/result.py
+-rw-rw-rw-   0 root         (0) root         (0)    28116 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/run_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    21539 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/scaffolding_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     7160 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 00:52:19.926184 khloraascaf-1.7.1/src/khloraascaf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    46361 2023-05-09 00:52:19.000000 khloraascaf-1.7.1/src/khloraascaf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-05-09 00:52:19.000000 khloraascaf-1.7.1/src/khloraascaf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 00:52:19.000000 khloraascaf-1.7.1/src/khloraascaf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-09 00:52:19.000000 khloraascaf-1.7.1/src/khloraascaf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-09 00:52:19.000000 khloraascaf-1.7.1/src/khloraascaf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 00:52:19.933183 khloraascaf-1.7.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13219 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/tests/test_assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/tests/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/tests/test_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)    14876 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/tests/test_run_metdata.py
+-rw-rw-rw-   0 root         (0) root         (0)    22601 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/tests/test_toy_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     2989 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/tests/test_utils_debug.py
```

### Comparing `khloraascaf-1.7.0/LICENCE` & `khloraascaf-1.7.1/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/PKG-INFO` & `khloraascaf-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.7.0
+Version: 1.7.1
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf-1.7.0/README.md` & `khloraascaf-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/pyproject.toml` & `khloraascaf-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf"
-version = "1.7.0"
+version = "1.7.1"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `khloraascaf-1.7.0/src/khloraascaf/__init__.py` & `khloraascaf-1.7.1/src/khloraascaf/__init__.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/__main__.py` & `khloraascaf-1.7.1/src/khloraascaf/__main__.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/assembly_graph.py` & `khloraascaf-1.7.1/src/khloraascaf/assembly_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/cli.py` & `khloraascaf-1.7.1/src/khloraascaf/cli.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/exceptions.py` & `khloraascaf-1.7.1/src/khloraascaf/exceptions.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/ilp/dirf_sets.py` & `khloraascaf-1.7.1/src/khloraascaf/ilp/dirf_sets.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/ilp/invf_sets.py` & `khloraascaf-1.7.1/src/khloraascaf/ilp/invf_sets.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_circuit.py` & `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_circuit.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_max_dirf.py` & `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_max_dirf.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_max_invf.py` & `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_max_invf.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_max_presscore.py` & `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_max_presscore.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_repeated_fragments.py` & `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_repeated_fragments.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_to_solver.py` & `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_to_solver.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_var_db.py` & `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_var_db.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/inputs.py` & `khloraascaf-1.7.1/src/khloraascaf/inputs.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/lib.py` & `khloraascaf-1.7.1/src/khloraascaf/lib.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/multiplied_doubled_contig_graph.py` & `khloraascaf-1.7.1/src/khloraascaf/multiplied_doubled_contig_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/outputs.py` & `khloraascaf-1.7.1/src/khloraascaf/outputs.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/result.py` & `khloraascaf-1.7.1/src/khloraascaf/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -629,15 +629,16 @@
         The first vertex of the starter's region
     """
     v: OccOrCT = starter_vertex
     u: Optional[OccOrCT] = __pred_in_path(
         starter_vertex, mdcg, var, starter_vertex)
     # pylint: disable=compare-to-zero
     while (u is not None
-           and __get_region_code(u, set_invf_paired, set_dirf_paired) == 0
+           and __get_region_code(
+               u, set_invf_paired, set_dirf_paired) == SC_REGION_ID
            ):
         v = u
         u = __pred_in_path(v, mdcg, var, starter_vertex)
     if u is None:
         return starter_vertex
     return v
```

### Comparing `khloraascaf-1.7.0/src/khloraascaf/run_metadata.py` & `khloraascaf-1.7.1/src/khloraascaf/run_metadata.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/scaffolding_methods.py` & `khloraascaf-1.7.1/src/khloraascaf/scaffolding_methods.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf/utils_debug.py` & `khloraascaf-1.7.1/src/khloraascaf/utils_debug.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/src/khloraascaf.egg-info/PKG-INFO` & `khloraascaf-1.7.1/src/khloraascaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.7.0
+Version: 1.7.1
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf-1.7.0/src/khloraascaf.egg-info/SOURCES.txt` & `khloraascaf-1.7.1/src/khloraascaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/tests/test_assembly_graph.py` & `khloraascaf-1.7.1/tests/test_assembly_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/tests/test_exceptions.py` & `khloraascaf-1.7.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/tests/test_run_metdata.py` & `khloraascaf-1.7.1/tests/test_run_metdata.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/tests/test_toy_examples.py` & `khloraascaf-1.7.1/tests/test_toy_examples.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.0/tests/test_utils_debug.py` & `khloraascaf-1.7.1/tests/test_utils_debug.py`

 * *Files identical despite different names*

