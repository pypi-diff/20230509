# Comparing `tmp/khloraascaf_utils-0.7.0.tar.gz` & `tmp/khloraascaf_utils-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf_utils-0.7.0.tar", last modified: Mon May  8 20:11:32 2023, max compression
+gzip compressed data, was "khloraascaf_utils-0.8.0.tar", last modified: Tue May  9 12:21:19 2023, max compression
```

## Comparing `khloraascaf_utils-0.7.0.tar` & `khloraascaf_utils-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:11:32.461345 khloraascaf_utils-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-08 20:11:07.000000 khloraascaf_utils-0.7.0/LICENCE
--rw-r--r--   0 root         (0) root         (0)    43838 2023-05-08 20:11:32.460344 khloraascaf_utils-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2535 2023-05-08 20:11:07.000000 khloraascaf_utils-0.7.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-08 20:11:07.000000 khloraascaf_utils-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 20:11:32.461345 khloraascaf_utils-0.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:11:32.453344 khloraascaf_utils-0.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:11:32.457344 khloraascaf_utils-0.7.0/src/khloraascaf_utils/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-08 20:11:07.000000 khloraascaf_utils-0.7.0/src/khloraascaf_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8224 2023-05-08 20:11:07.000000 khloraascaf_utils-0.7.0/src/khloraascaf_utils/artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7285 2023-05-08 20:11:07.000000 khloraascaf_utils-0.7.0/src/khloraascaf_utils/asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-05-08 20:11:07.000000 khloraascaf_utils-0.7.0/src/khloraascaf_utils/contigs_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    13756 2023-05-08 20:11:07.000000 khloraascaf_utils-0.7.0/src/khloraascaf_utils/to_networkx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:11:32.459344 khloraascaf_utils-0.7.0/src/khloraascaf_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    43838 2023-05-08 20:11:32.000000 khloraascaf_utils-0.7.0/src/khloraascaf_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      552 2023-05-08 20:11:32.000000 khloraascaf_utils-0.7.0/src/khloraascaf_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 20:11:32.000000 khloraascaf_utils-0.7.0/src/khloraascaf_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-08 20:11:32.000000 khloraascaf_utils-0.7.0/src/khloraascaf_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-08 20:11:32.000000 khloraascaf_utils-0.7.0/src/khloraascaf_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 20:11:32.460344 khloraascaf_utils-0.7.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4111 2023-05-08 20:11:07.000000 khloraascaf_utils-0.7.0/tests/test_artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3590 2023-05-08 20:11:07.000000 khloraascaf_utils-0.7.0/tests/test_asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     1770 2023-05-08 20:11:07.000000 khloraascaf_utils-0.7.0/tests/test_contigs_attributes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:21:19.153237 khloraascaf_utils-0.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-05-09 12:21:19.152237 khloraascaf_utils-0.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 12:21:19.153237 khloraascaf_utils-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:21:19.145237 khloraascaf_utils-0.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:21:19.149237 khloraascaf_utils-0.8.0/src/khloraascaf_utils/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8224 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils/artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7285 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils/asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils/contigs_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    13769 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils/to_networkx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:21:19.151237 khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-05-09 12:21:19.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-09 12:21:19.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 12:21:19.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-09 12:21:19.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-09 12:21:19.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:21:19.152237 khloraascaf_utils-0.8.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4111 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/tests/test_artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/tests/test_asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/tests/test_contigs_attributes.py
```

### Comparing `khloraascaf_utils-0.7.0/LICENCE` & `khloraascaf_utils-0.8.0/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.7.0/PKG-INFO` & `khloraascaf_utils-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf_utils
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf_utils-0.7.0/README.md` & `khloraascaf_utils-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.7.0/pyproject.toml` & `khloraascaf_utils-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf_utils"
-version = "0.7.0"
+version = "0.8.0"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "Python utilities for khloraascaf python package."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -17,15 +17,15 @@
     "Operating System :: Unix",
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 license = { file = "LICENCE" }
 requires-python = ">=3.9"
 dependencies = [
-    "khloraascaf >=1.7.0, <1.8",
+    "khloraascaf >=1.8.0, <1.9",
     "networkx >=3.0, <3.1",
     "biopython >=1.81, <1.82",
 ]
 
 [project.urls]
 
 Homepage = "https://gitlab.com/khloraa_scaffolding/khloraascaf_utils"
```

### Comparing `khloraascaf_utils-0.7.0/src/khloraascaf_utils/artificial_data.py` & `khloraascaf_utils-0.8.0/src/khloraascaf_utils/artificial_data.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.7.0/src/khloraascaf_utils/asm_graph_to_fasta.py` & `khloraascaf_utils-0.8.0/src/khloraascaf_utils/asm_graph_to_fasta.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.7.0/src/khloraascaf_utils/contigs_attributes.py` & `khloraascaf_utils-0.8.0/src/khloraascaf_utils/contigs_attributes.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.7.0/src/khloraascaf_utils/to_networkx.py` & `khloraascaf_utils-0.8.0/src/khloraascaf_utils/to_networkx.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         Order of oriented regions
     attribute_suffix : str
         Suffix for the attribute name
     """
     #
     # Record vertices and oriented regions path
     #
-    vertices_regions: list[list[OccOrCT]] = list(
+    vertices_regions: tuple[tuple[OccOrCT, ...], ...] = tuple(
         read_vertices_of_regions(vertices_of_regions_path),
     )
     first_region_discovered: list[bool] = [False] * len(vertices_regions)
     #
     # Add the solutions path and repeated fragments
     #
     vertex_path: list[OccOrCT] = []
```

### Comparing `khloraascaf_utils-0.7.0/src/khloraascaf_utils.egg-info/PKG-INFO` & `khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf-utils
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf_utils-0.7.0/src/khloraascaf_utils.egg-info/SOURCES.txt` & `khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.7.0/tests/test_artificial_data.py` & `khloraascaf_utils-0.8.0/tests/test_artificial_data.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.7.0/tests/test_asm_graph_to_fasta.py` & `khloraascaf_utils-0.8.0/tests/test_asm_graph_to_fasta.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.7.0/tests/test_contigs_attributes.py` & `khloraascaf_utils-0.8.0/tests/test_contigs_attributes.py`

 * *Files identical despite different names*

