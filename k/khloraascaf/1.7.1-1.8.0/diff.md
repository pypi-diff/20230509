# Comparing `tmp/khloraascaf-1.7.1.tar.gz` & `tmp/khloraascaf-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf-1.7.1.tar", last modified: Tue May  9 00:52:19 2023, max compression
+gzip compressed data, was "khloraascaf-1.8.0.tar", last modified: Tue May  9 12:11:22 2023, max compression
```

## Comparing `khloraascaf-1.7.1.tar` & `khloraascaf-1.8.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 00:52:19.934183 khloraascaf-1.7.1/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/LICENCE
--rw-r--r--   0 root         (0) root         (0)    46361 2023-05-09 00:52:19.933183 khloraascaf-1.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4981 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1339 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 00:52:19.934183 khloraascaf-1.7.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 00:52:19.917186 khloraascaf-1.7.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 00:52:19.924185 khloraascaf-1.7.1/src/khloraascaf/
--rw-rw-rw-   0 root         (0) root         (0)     1579 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1760 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    13402 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     5619 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5600 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 00:52:19.930184 khloraascaf-1.7.1/src/khloraascaf/ilp/
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11068 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/dirf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)    10725 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/invf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)     4901 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_circuit.py
--rw-rw-rw-   0 root         (0) root         (0)     3418 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_max_dirf.py
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_max_invf.py
--rw-rw-rw-   0 root         (0) root         (0)     3738 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_max_presscore.py
--rw-rw-rw-   0 root         (0) root         (0)    12009 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_repeated_fragments.py
--rw-rw-rw-   0 root         (0) root         (0)     3027 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_to_solver.py
--rw-rw-rw-   0 root         (0) root         (0)    10512 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_var_db.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/lib.py
--rw-rw-rw-   0 root         (0) root         (0)    12867 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/multiplied_doubled_contig_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     8323 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    21863 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/result.py
--rw-rw-rw-   0 root         (0) root         (0)    28116 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/run_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    21539 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/scaffolding_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     7160 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/src/khloraascaf/utils_debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 00:52:19.926184 khloraascaf-1.7.1/src/khloraascaf.egg-info/
--rw-r--r--   0 root         (0) root         (0)    46361 2023-05-09 00:52:19.000000 khloraascaf-1.7.1/src/khloraascaf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1174 2023-05-09 00:52:19.000000 khloraascaf-1.7.1/src/khloraascaf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 00:52:19.000000 khloraascaf-1.7.1/src/khloraascaf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-09 00:52:19.000000 khloraascaf-1.7.1/src/khloraascaf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-09 00:52:19.000000 khloraascaf-1.7.1/src/khloraascaf.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 00:52:19.933183 khloraascaf-1.7.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13219 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/tests/test_assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/tests/test_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)    14876 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/tests/test_run_metdata.py
--rw-rw-rw-   0 root         (0) root         (0)    22601 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/tests/test_toy_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     2989 2023-05-09 00:51:56.000000 khloraascaf-1.7.1/tests/test_utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:11:22.363547 khloraascaf-1.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    46344 2023-05-09 12:11:22.362547 khloraascaf-1.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 12:11:22.363547 khloraascaf-1.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:11:22.346546 khloraascaf-1.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:11:22.354547 khloraascaf-1.8.0/src/khloraascaf/
+-rw-rw-rw-   0 root         (0) root         (0)     1579 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13402 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5619 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5600 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:11:22.360547 khloraascaf-1.8.0/src/khloraascaf/ilp/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11068 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/dirf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)    10725 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/invf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)     4901 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3418 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_max_dirf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_max_invf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_max_presscore.py
+-rw-rw-rw-   0 root         (0) root         (0)    12009 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_repeated_fragments.py
+-rw-rw-rw-   0 root         (0) root         (0)     3027 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_to_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)    10512 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_var_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12867 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/multiplied_doubled_contig_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     8323 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    21582 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/result.py
+-rw-rw-rw-   0 root         (0) root         (0)    28593 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/run_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    21539 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/scaffolding_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     7160 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:11:22.356547 khloraascaf-1.8.0/src/khloraascaf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    46344 2023-05-09 12:11:22.000000 khloraascaf-1.8.0/src/khloraascaf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-05-09 12:11:22.000000 khloraascaf-1.8.0/src/khloraascaf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 12:11:22.000000 khloraascaf-1.8.0/src/khloraascaf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-09 12:11:22.000000 khloraascaf-1.8.0/src/khloraascaf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-09 12:11:22.000000 khloraascaf-1.8.0/src/khloraascaf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:11:22.362547 khloraascaf-1.8.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13219 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/tests/test_assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/tests/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/tests/test_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)    15226 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/tests/test_run_metdata.py
+-rw-rw-rw-   0 root         (0) root         (0)    22601 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/tests/test_toy_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     2989 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/tests/test_utils_debug.py
```

### Comparing `khloraascaf-1.7.1/LICENCE` & `khloraascaf-1.8.0/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/PKG-INFO` & `khloraascaf-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.7.1
+Version: 1.8.0
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -764,17 +764,17 @@
 # Use metadata class to easily dive into the results
 # (you can also see by hand the solutions.yaml file that has been produced)
 #
 all_solutions_metadata = MetadataAllSolutions.from_run_directory(outdir_gen)
 #
 # * How many solutions the scaffolding has produced?
 #
-print(len(all_solutions_metadata.solutions()))
+print(len(all_solutions_metadata))
 #   = 1, let pick its metadata
-sol_metadata = all_solutions_metadata.solutions()[0]
+sol_metadata = tuple(all_solutions_metadata)[0]
 #
 # See which files the scaffolding has produced:
 #
 files = set(outdir_gen.glob('*'))
 assert len(files) == 4
 #
 # * The list of oriented contigs for each region
```

### Comparing `khloraascaf-1.7.1/README.md` & `khloraascaf-1.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,17 +68,17 @@
 # Use metadata class to easily dive into the results
 # (you can also see by hand the solutions.yaml file that has been produced)
 #
 all_solutions_metadata = MetadataAllSolutions.from_run_directory(outdir_gen)
 #
 # * How many solutions the scaffolding has produced?
 #
-print(len(all_solutions_metadata.solutions()))
+print(len(all_solutions_metadata))
 #   = 1, let pick its metadata
-sol_metadata = all_solutions_metadata.solutions()[0]
+sol_metadata = tuple(all_solutions_metadata)[0]
 #
 # See which files the scaffolding has produced:
 #
 files = set(outdir_gen.glob('*'))
 assert len(files) == 4
 #
 # * The list of oriented contigs for each region
```

### Comparing `khloraascaf-1.7.1/pyproject.toml` & `khloraascaf-1.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf"
-version = "1.7.1"
+version = "1.8.0"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `khloraascaf-1.7.1/src/khloraascaf/__init__.py` & `khloraascaf-1.8.0/src/khloraascaf/__init__.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/__main__.py` & `khloraascaf-1.8.0/src/khloraascaf/__main__.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/assembly_graph.py` & `khloraascaf-1.8.0/src/khloraascaf/assembly_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/cli.py` & `khloraascaf-1.8.0/src/khloraascaf/cli.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/exceptions.py` & `khloraascaf-1.8.0/src/khloraascaf/exceptions.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/ilp/dirf_sets.py` & `khloraascaf-1.8.0/src/khloraascaf/ilp/dirf_sets.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/ilp/invf_sets.py` & `khloraascaf-1.8.0/src/khloraascaf/ilp/invf_sets.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_circuit.py` & `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_circuit.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_max_dirf.py` & `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_max_dirf.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_max_invf.py` & `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_max_invf.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_max_presscore.py` & `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_max_presscore.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_repeated_fragments.py` & `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_repeated_fragments.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_to_solver.py` & `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_to_solver.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/ilp/pulp_var_db.py` & `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_var_db.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/inputs.py` & `khloraascaf-1.8.0/src/khloraascaf/inputs.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/lib.py` & `khloraascaf-1.8.0/src/khloraascaf/lib.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/multiplied_doubled_contig_graph.py` & `khloraascaf-1.8.0/src/khloraascaf/multiplied_doubled_contig_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/outputs.py` & `khloraascaf-1.8.0/src/khloraascaf/outputs.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/result.py` & `khloraascaf-1.8.0/src/khloraascaf/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,22 +369,28 @@
     set_invf_paired = __create_set_invf_paired(var, fix_result)
     set_dirf_paired = __create_set_dirf_paired(var, fix_result)
 
     # ------------------------------------------------------------------------ #
     # Init regions
     # ------------------------------------------------------------------------ #
     result_builder = _ScaffoldingResultBuilder()
-    prev_region_code = SC_REGION_ID
-    region_index = result_builder.add_region(SC_REGION_ID)
 
     initial_vertex = __find_initial(
         mdcg, starter_vertex, var, set_invf_paired, set_dirf_paired)
 
     u: OccOrCT = initial_vertex  # previous v
-    v: Optional[OccOrCT] = initial_vertex
+
+    prev_region_code = SC_REGION_ID
+    region_index = result_builder.add_region(prev_region_code)
+    result_builder.add_occorc_to_region(u, region_index)
+
+    v: OccOrCT = __succ_in_path(u, mdcg, var)
+
+    region_code = SC_REGION_ID
+
     #
     # Region IR: LIFO, DR: FIFO
     #
     # XXX no order between pairs of repeats
     #   * for the moment, the pairs of contiguous repeat are not considered
     #       ordered (e.g. pairs of contiguous IR should be lifo, DR fifo)
     rep_queue: RepQueueT = {}
@@ -392,15 +398,15 @@
     # Canonical to the region's index: repeat was discovered
     #
     v_canonical_rep: dict[OccOrCT, IndexT] = {}
 
     # ------------------------------------------------------------------------ #
     # Walk into the solution path
     # ------------------------------------------------------------------------ #
-    while v is not None:
+    while v != initial_vertex:
         region_code = __get_region_code(v, set_invf_paired, set_dirf_paired)
         #
         # Single-copy
         #
         if region_code == SC_REGION_ID:
             #
             # New single-copy
@@ -441,104 +447,91 @@
                         u, v, var, prev_region_code, region_code):
                     region_index = v_canonical_rep[canonical_repf]
                     result_builder.add_region(region_code, region_index)
                 assert v == rep_queue[region_index].get()
 
         prev_region_code = region_code
         u = v
-        v = __succ_in_path(v, mdcg, var, initial_vertex)
+        v = __succ_in_path(v, mdcg, var)
 
     # ------------------------------------------------------------------------ #
     # To view
     # ------------------------------------------------------------------------ #
     return result_builder.view(prob, ilp_combi)
 
 
 # ---------------------------------------------------------------------------- #
 #                               Walk In The Path                               #
 # ---------------------------------------------------------------------------- #
-def __pred_in_path(v: OccOrCT, mdcg: MDCGraph,
-                   var: PuLPVarModelT, initial_vertex: OccOrCT) -> (
-        Optional[OccOrCT]):
+def __pred_in_path(v: OccOrCT, mdcg: MDCGraph, var: PuLPVarModelT) -> OccOrCT:
     """Return the predecessor of vertex v in solution path.
 
     Stop if the predecessor is the initial vertex.
 
     Parameters
     ----------
     v : OccOrCT
         Vertex
     mdcg : MDCGraph
         Multiplied doubled contig graph
     var : PuLPVarModelT
         PuLP variables
-    initial_vertex : OccOrCT
-        Starter vertex
 
     Returns
     -------
     OccOrCT, optional
         The previous vertex in solution path, None if it is the
         initial vertex
 
     Raises
     ------
     NotACircuit
         If the path is not a circuit
     """
     for u in mdcg.multiplied_preds(v):
         if var.x[u, v].varValue > BIN_THRESHOLD:
-            if u == initial_vertex:
-                return None
             return u
     raise NotACircuit()
 
 
-def __succ_in_path(v: OccOrCT, mdcg: MDCGraph,
-                   var: PuLPVarModelT, initial_vertex: OccOrCT) -> (
-        Optional[OccOrCT]):
+def __succ_in_path(v: OccOrCT, mdcg: MDCGraph, var: PuLPVarModelT) -> OccOrCT:
     """Return the successor of vertex v in solution path.
 
     Stop if the successor is the initial vertex.
 
     Parameters
     ----------
     v : OccOrCT
         Vertex
     mdcg : MDCGraph
         Multiplied doubled contig graph
     var : PuLPVarModelT
         PuLP variables
-    initial_vertex : OccOrCT
-        Starter vertex
 
     Returns
     -------
-    OccOrCT, optional
-        The next vertex in solution path, None if it is the
-        initial vertex
+    OccOrCT
+        The next vertex in solution path
 
     Raises
     ------
     NotACircuit
         If the path is not a circuit
     """
     for w in mdcg.multiplied_succs(v):
         if var.x[v, w].varValue > BIN_THRESHOLD:
-            if w == initial_vertex:
-                return None
             return w
     raise NotACircuit()
 
 
 # ---------------------------------------------------------------------------- #
 #                                Initialisation                                #
 # ---------------------------------------------------------------------------- #
 def __create_set_invf_paired(var: PuLPVarModelT,
-                             fix_result: Optional[ScaffoldingResult]) -> (
+                             fix_result: ScaffoldingResult | None) -> (
         set[OccOrCT]):
     """Create set of canonical of paired inverted fragments.
 
     Parameters
     ----------
     var : PuLPVarModelT
         PuLP variables
@@ -625,24 +618,25 @@
 
     Returns
     -------
     OccOrCT
         The first vertex of the starter's region
     """
     v: OccOrCT = starter_vertex
-    u: Optional[OccOrCT] = __pred_in_path(
-        starter_vertex, mdcg, var, starter_vertex)
-    # pylint: disable=compare-to-zero
-    while (u is not None
-           and __get_region_code(
-               u, set_invf_paired, set_dirf_paired) == SC_REGION_ID
-           ):
+    u: OccOrCT = __pred_in_path(starter_vertex, mdcg, var)
+    region_code = __get_region_code(u, set_invf_paired, set_dirf_paired)
+
+    while u != starter_vertex and region_code == SC_REGION_ID:
         v = u
-        u = __pred_in_path(v, mdcg, var, starter_vertex)
-    if u is None:
+        u = __pred_in_path(v, mdcg, var)
+        region_code = __get_region_code(u, set_invf_paired, set_dirf_paired)
+    #
+    # Special case: circular SC
+    #
+    if region_code == SC_REGION_ID:
         return starter_vertex
     return v
 
 
 # ---------------------------------------------------------------------------- #
 #                               Region Management                              #
 # ---------------------------------------------------------------------------- #
```

### Comparing `khloraascaf-1.7.1/src/khloraascaf/run_metadata.py` & `khloraascaf-1.8.0/src/khloraascaf/run_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding=utf-8 -*-
 
 """Module for the RunMetadata class."""
 
 
 from __future__ import annotations
 
-from collections.abc import Iterable
+from collections.abc import Iterable, Iterator
 from pathlib import Path
 from typing import Any, Optional
 
 import yaml  # type: ignore
 from pulp import LpStatus, LpStatusOptimal
 from revsymg.index_lib import IndexT
 
@@ -502,24 +502,14 @@
         Returns
         -------
         Path
             Solutions directory path
         """
         return self.__sol_dir
 
-    def solutions(self) -> list[MetadataSolution]:
-        """List of solutions metadata.
-
-        Returns
-        -------
-        list of MetadataSolution
-            List of solutions metadata
-        """
-        return self.__solutions
-
     # ~*~ I/O ~*~
 
     def write_yaml(self, append_yaml: bool = False):
         """Write the solutions metadata to a YAML file.
 
         Parameters
         ----------
@@ -556,14 +546,36 @@
         Returns
         -------
         Path
             YAML file path
         """
         return self.__sol_dir / self.YAML_FILE
 
+    # ~*~ Special ~*~
+
+    def __iter__(self) -> Iterator[MetadataSolution]:
+        """Iterate over the solution metadata.
+
+        Yields
+        ------
+        MetadataSolution
+            Solution metadata
+        """
+        yield from self.__solutions
+
+    def __len__(self) -> int:
+        """Return the number of solution metadata.
+
+        Returns
+        -------
+        int
+            Number of solution metadata
+        """
+        return len(self.__solutions)
+
 
 # DOCU MetadataDebug
 class MetadataDebug():
     """Debug metadata class."""
 
     YAML_FILE: str = 'debug.yaml'
     """Debug metadata file name."""
@@ -885,24 +897,14 @@
         Returns
         -------
         Path
             Runs directory path
         """
         return self.__run_dir
 
-    def debugs(self) -> list[MetadataDebug]:
-        """List of debugs metadata.
-
-        Returns
-        -------
-        list of MetadataDebug
-            List of debugs metadata
-        """
-        return self.__debugs
-
     # ~*~ I/O ~*~
 
     def write_yaml(self, append_yaml: bool = False):
         """Write the debugs metadata to a YAML file.
 
         Parameters
         ----------
@@ -955,14 +957,36 @@
         Returns
         -------
         Path
             YAML file path
         """
         return self.__run_dir / self.YAML_FILE
 
+    # ~*~ Special ~*~
+
+    def __iter__(self) -> Iterator[MetadataDebug]:
+        """Iterate over the debug metadata.
+
+        Yields
+        ------
+        MetadataDebug
+            Solution metadata
+        """
+        yield from self.__debugs
+
+    def __len__(self) -> int:
+        """Return the number of debug metadata.
+
+        Returns
+        -------
+        int
+            Number of debug metadata
+        """
+        return len(self.__debugs)
+
 
 # ============================================================================ #
 #                                   FUNCTIONS                                  #
 # ============================================================================ #
 # ---------------------------------------------------------------------------- #
 #                               String Formatter                               #
 # ---------------------------------------------------------------------------- #
```

### Comparing `khloraascaf-1.7.1/src/khloraascaf/scaffolding_methods.py` & `khloraascaf-1.8.0/src/khloraascaf/scaffolding_methods.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf/utils_debug.py` & `khloraascaf-1.8.0/src/khloraascaf/utils_debug.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/src/khloraascaf.egg-info/PKG-INFO` & `khloraascaf-1.8.0/src/khloraascaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.7.1
+Version: 1.8.0
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -764,17 +764,17 @@
 # Use metadata class to easily dive into the results
 # (you can also see by hand the solutions.yaml file that has been produced)
 #
 all_solutions_metadata = MetadataAllSolutions.from_run_directory(outdir_gen)
 #
 # * How many solutions the scaffolding has produced?
 #
-print(len(all_solutions_metadata.solutions()))
+print(len(all_solutions_metadata))
 #   = 1, let pick its metadata
-sol_metadata = all_solutions_metadata.solutions()[0]
+sol_metadata = tuple(all_solutions_metadata)[0]
 #
 # See which files the scaffolding has produced:
 #
 files = set(outdir_gen.glob('*'))
 assert len(files) == 4
 #
 # * The list of oriented contigs for each region
```

### Comparing `khloraascaf-1.7.1/src/khloraascaf.egg-info/SOURCES.txt` & `khloraascaf-1.8.0/src/khloraascaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/tests/test_assembly_graph.py` & `khloraascaf-1.8.0/tests/test_assembly_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,19 +165,19 @@
     # TOTEST use fixture for assembly graph
     asm_graph = AssemblyGraph(
         _DR_SC_SOL_REGMAP,
         _DR_SC_SOL_REGCTG,
     )
     s_orc_paths: set[tuple[OrCT, ...]] = {
         (
-            ('C0', FORWARD_INT),
-            ('C1', REVERSE_INT),
+            ('C0', REVERSE_INT),
+            ('C1', FORWARD_INT),
             ('C2', REVERSE_INT),
             ('C3', FORWARD_INT),
-            ('C4', FORWARD_INT),
+            ('C4', REVERSE_INT),
             ('C2', REVERSE_INT),
             ('C3', FORWARD_INT),
         ),
     }
     asm_graph_paths = tuple(asm_graph.all_oriented_contig_paths())
     assert len(asm_graph_paths) == len(s_orc_paths)
     assert set(asm_graph_paths) == s_orc_paths
```

### Comparing `khloraascaf-1.7.1/tests/test_exceptions.py` & `khloraascaf-1.8.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.7.1/tests/test_run_metdata.py` & `khloraascaf-1.8.0/tests/test_run_metdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,19 +83,25 @@
 
 
 def test_iocfg_config_directory(io_cfg_ir_sc: IOConfig):
     assert io_cfg_ir_sc.io_config_directory() == _IR_SC_DIR
 
 
 def test_iocfg_contig_attrs(io_cfg_ir_sc: IOConfig):
-    assert io_cfg_ir_sc.contig_attrs() == _IR_SC_CONTIG_ATTRS
+    assert (
+        io_cfg_ir_sc.contig_attrs()
+        == _IR_SC_CONTIG_ATTRS.relative_to(_IR_SC_DIR)
+    )
 
 
 def test_iocfg_contig_links(io_cfg_ir_sc: IOConfig):
-    assert io_cfg_ir_sc.contig_links() == _IR_SC_CONTIG_LINKS
+    assert (
+        io_cfg_ir_sc.contig_links()
+        == _IR_SC_CONTIG_LINKS.relative_to(_IR_SC_DIR)
+    )
 
 
 def test_iocfg_contig_starter(io_cfg_ir_sc: IOConfig):
     assert io_cfg_ir_sc.contig_starter() == _IR_SC_CONTIG_STARTER
 
 
 def test_iocfg_mult_upb(io_cfg_ir_sc: IOConfig):
@@ -107,15 +113,18 @@
 
 
 def test_iocfg_solver(io_cfg_ir_sc: IOConfig):
     assert io_cfg_ir_sc.solver() == SOLVER_CBC
 
 
 def test_iocfg_outdir(io_cfg_ir_sc: IOConfig):
-    assert io_cfg_ir_sc.outdir() == _IR_SC_DIR / 'tmp'
+    assert (
+        io_cfg_ir_sc.outdir()
+        == (_IR_SC_DIR / 'tmp').relative_to(_IR_SC_DIR)
+    )
 
 
 def test_iocfg_instance_name(io_cfg_ir_sc: IOConfig):
     assert io_cfg_ir_sc.instance_name() == INSTANCE_NAME_DEF
 
 
 def test_iocfg_debug(io_cfg_ir_sc: IOConfig):
@@ -223,24 +232,28 @@
 
 def test_allsol_meta_from_run_dir(allsol_meta_ir_sc: MetadataAllSolutions):
     assert allsol_meta_ir_sc
 
 
 def test_sol_meta_from_run_dir_empty():
     nosol_meta = MetadataAllSolutions.from_run_directory(Path('. /'))
-    assert not nosol_meta.solutions()
+    assert not nosol_meta
 
 
 def test_allsol_meta_solutions_directory(
         allsol_meta_ir_sc: MetadataAllSolutions):
     assert allsol_meta_ir_sc.solutions_directory() == _IR_SC_DIR
 
 
-def test_allsol_meta_solutions(allsol_meta_ir_sc: MetadataAllSolutions):
-    assert len(allsol_meta_ir_sc.solutions()) == 1
+def test_allsol_meta_iter(allsol_meta_ir_sc: MetadataAllSolutions):
+    assert sum(1 for _ in allsol_meta_ir_sc) == 1
+
+
+def test_allsol_meta_len(allsol_meta_ir_sc: MetadataAllSolutions):
+    assert len(allsol_meta_ir_sc) == 1
 
 
 def test_allsol_meta_write_yaml(allsol_meta_ir_sc: MetadataAllSolutions):
     true_allsol_meta_path = _IR_SC_DIR / 'true_solutions.yaml'
     _IR_SC_SOLUTIONS_YAML.rename(true_allsol_meta_path)
     allsol_meta_ir_sc.write_yaml()
     assert _IR_SC_SOLUTIONS_YAML.exists()
@@ -342,16 +355,20 @@
     assert alldebugs_meta_ir_sc
 
 
 def test_alldebugs_meta_run_dir(alldebugs_meta_ir_sc: MetadataAllDebugs):
     assert alldebugs_meta_ir_sc.runs_directory() == _IR_SC_DIR
 
 
-def test_alldebugs_meta_debugs(alldebugs_meta_ir_sc: MetadataAllDebugs):
-    assert len(alldebugs_meta_ir_sc.debugs()) == 4
+def test_alldebugs_meta_iter(alldebugs_meta_ir_sc: MetadataAllDebugs):
+    assert sum(1 for _ in alldebugs_meta_ir_sc) == 4
+
+
+def test_alldebugs_meta_len(alldebugs_meta_ir_sc: MetadataAllDebugs):
+    assert len(alldebugs_meta_ir_sc) == 4
 
 
 def test_alldebugs_meta_write_yaml(alldebugs_meta_ir_sc: MetadataAllDebugs):
     true_alldebugs_meta_path = _IR_SC_DIR / 'true_debugs.yaml'
     _IR_SC_DEBUGS_YAML.rename(true_alldebugs_meta_path)
     alldebugs_meta_ir_sc.write_yaml()
     assert _IR_SC_DEBUGS_YAML.exists()
```

### Comparing `khloraascaf-1.7.1/tests/test_toy_examples.py` & `khloraascaf-1.8.0/tests/test_toy_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 # ---------------------------------------------------------------------------- #
 #                                    DR - SC                                   #
 # ---------------------------------------------------------------------------- #
 _DR_SC_DIR = _TOY_DATADIR / 'dr_sc'
 _DR_SC_CONTIG_ATTRS = _DR_SC_DIR / 'contig_attrs.tsv'
 _DR_SC_CONTIG_LINKS = _DR_SC_DIR / 'contig_links.tsv'
-_DR_SC_CONTIG_STARTER = 'C0'
+_DR_SC_CONTIG_STARTER = 'C1'
 _DR_SC_SOL_REGMAP = _DR_SC_DIR / 'map_of_regions_sol.tsv'
 _DR_SC_SOL_REGCTG = _DR_SC_DIR / 'contigs_of_regions_sol.tsv'
 
 # ---------------------------------------------------------------------------- #
 #                                      SC                                      #
 # ---------------------------------------------------------------------------- #
 _SC_DIR = _TOY_DATADIR / 'sc'
```

### Comparing `khloraascaf-1.7.1/tests/test_utils_debug.py` & `khloraascaf-1.8.0/tests/test_utils_debug.py`

 * *Files identical despite different names*

