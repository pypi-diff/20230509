# Comparing `tmp/biobookshelf-0.2.4.tar.gz` & `tmp/biobookshelf-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobookshelf-0.2.4.tar", last modified: Fri May  5 13:20:37 2023, max compression
+gzip compressed data, was "biobookshelf-0.2.5.tar", last modified: Tue May  9 04:56:14 2023, max compression
```

## Comparing `biobookshelf-0.2.4.tar` & `biobookshelf-0.2.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.971949 biobookshelf-0.2.4/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    34600 2022-04-04 14:27:30.000000 biobookshelf-0.2.4/LICENSE
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        0 2022-04-04 14:27:30.000000 biobookshelf-0.2.4/MANIFEST.in
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-05-05 13:20:36.971949 biobookshelf-0.2.4/PKG-INFO
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      221 2022-04-04 14:27:30.000000 biobookshelf-0.2.4/README.md
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.447940 biobookshelf-0.2.4/biobookshelf/
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.463940 biobookshelf-0.2.4/biobookshelf/BA/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       30 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/BA/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     7975 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/BA/bitarray_utils.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.479941 biobookshelf-0.2.4/biobookshelf/CLI/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/CLI/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3013 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/CLI/unclassified_programs.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.515941 biobookshelf-0.2.4/biobookshelf/INT/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/INT/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      389 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/INT/integer.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.543942 biobookshelf-0.2.4/biobookshelf/IT/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       35 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/IT/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       32 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/IT/interval_tree_utils.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.551942 biobookshelf-0.2.4/biobookshelf/L/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/L/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       39 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/L/l_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.559942 biobookshelf-0.2.4/biobookshelf/MAP/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/MAP/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      594 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/MAP/mapping.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.591943 biobookshelf-0.2.4/biobookshelf/MP/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/MP/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      260 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/MP/multiprocessing_utils.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.595943 biobookshelf-0.2.4/biobookshelf/ONT/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       34 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/ONT/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    66087 2023-05-05 08:17:52.000000 biobookshelf-0.2.4/biobookshelf/ONT/nanopore_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.615943 biobookshelf-0.2.4/biobookshelf/PD/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/PD/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       85 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/PD/pd_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.647944 biobookshelf-0.2.4/biobookshelf/PDB/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       19 2022-04-04 14:27:31.000000 biobookshelf-0.2.4/biobookshelf/PDB/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    29100 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/PDB/pdb.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.667944 biobookshelf-0.2.4/biobookshelf/PKG/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/PKG/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3095 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/PKG/package_util.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.683944 biobookshelf-0.2.4/biobookshelf/RNA/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/RNA/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    19437 2023-05-01 11:20:30.000000 biobookshelf-0.2.4/biobookshelf/RNA/rnaseq.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.727945 biobookshelf-0.2.4/biobookshelf/SAM/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2022-04-04 14:27:31.000000 biobookshelf-0.2.4/biobookshelf/SAM/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    69402 2023-05-01 11:20:32.000000 biobookshelf-0.2.4/biobookshelf/SAM/sam_util.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.775946 biobookshelf-0.2.4/biobookshelf/SC/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/SC/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   122849 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/SC/single_cell.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.799946 biobookshelf-0.2.4/biobookshelf/SEQ/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/SEQ/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14831 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/SEQ/sequence.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.835947 biobookshelf-0.2.4/biobookshelf/STR/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/STR/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14367 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/STR/string.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.867948 biobookshelf-0.2.4/biobookshelf/UniProt/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2022-04-04 14:27:31.000000 biobookshelf-0.2.4/biobookshelf/UniProt/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      837 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/UniProt/uniprot.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.903948 biobookshelf-0.2.4/biobookshelf/WEB/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       31 2022-04-04 14:27:31.000000 biobookshelf-0.2.4/biobookshelf/WEB/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     8727 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/WEB/web_application.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.947949 biobookshelf-0.2.4/biobookshelf/ZA/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       26 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/ZA/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       12 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/ZA/zarr_utils.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      370 2023-05-05 13:19:35.000000 biobookshelf-0.2.4/biobookshelf/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      162 2023-05-01 11:20:29.000000 biobookshelf-0.2.4/biobookshelf/__main__.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.967949 biobookshelf-0.2.4/biobookshelf/main/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2022-04-18 07:53:18.000000 biobookshelf-0.2.4/biobookshelf/main/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   712244 2023-05-02 03:16:15.000000 biobookshelf-0.2.4/biobookshelf/main/unclassified_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-05 13:20:36.447940 biobookshelf-0.2.4/biobookshelf.egg-info/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-05-05 13:20:35.000000 biobookshelf-0.2.4/biobookshelf.egg-info/PKG-INFO
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     1538 2023-05-05 13:20:35.000000 biobookshelf-0.2.4/biobookshelf.egg-info/SOURCES.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        1 2023-05-05 13:20:35.000000 biobookshelf-0.2.4/biobookshelf.egg-info/dependency_links.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      394 2023-05-05 13:20:35.000000 biobookshelf-0.2.4/biobookshelf.egg-info/entry_points.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      480 2023-05-05 13:20:35.000000 biobookshelf-0.2.4/biobookshelf.egg-info/requires.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       13 2023-05-05 13:20:35.000000 biobookshelf-0.2.4/biobookshelf.egg-info/top_level.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2023-05-05 13:20:36.971949 biobookshelf-0.2.4/setup.cfg
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     2122 2023-05-05 13:19:26.000000 biobookshelf-0.2.4/setup.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.668303 biobookshelf-0.2.5/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    34600 2022-04-04 14:27:30.000000 biobookshelf-0.2.5/LICENSE
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        0 2022-04-04 14:27:30.000000 biobookshelf-0.2.5/MANIFEST.in
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-05-09 04:56:14.668303 biobookshelf-0.2.5/PKG-INFO
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      221 2022-04-04 14:27:30.000000 biobookshelf-0.2.5/README.md
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.032290 biobookshelf-0.2.5/biobookshelf/
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.064290 biobookshelf-0.2.5/biobookshelf/BA/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       30 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/BA/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     7975 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/BA/bitarray_utils.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.084291 biobookshelf-0.2.5/biobookshelf/CLI/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/CLI/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3013 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/CLI/unclassified_programs.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.116291 biobookshelf-0.2.5/biobookshelf/INT/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/INT/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      389 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/INT/integer.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.128291 biobookshelf-0.2.5/biobookshelf/IT/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       35 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/IT/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       32 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/IT/interval_tree_utils.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.140292 biobookshelf-0.2.5/biobookshelf/L/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/L/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       39 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/L/l_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.168292 biobookshelf-0.2.5/biobookshelf/MAP/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/MAP/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      594 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/MAP/mapping.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.228294 biobookshelf-0.2.5/biobookshelf/MP/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/MP/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      260 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/MP/multiprocessing_utils.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.228294 biobookshelf-0.2.5/biobookshelf/ONT/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       34 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/ONT/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    69306 2023-05-08 16:30:42.000000 biobookshelf-0.2.5/biobookshelf/ONT/nanopore_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.236294 biobookshelf-0.2.5/biobookshelf/PD/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/PD/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       85 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/PD/pd_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.268294 biobookshelf-0.2.5/biobookshelf/PDB/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       19 2022-04-04 14:27:31.000000 biobookshelf-0.2.5/biobookshelf/PDB/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    29100 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/PDB/pdb.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.316295 biobookshelf-0.2.5/biobookshelf/PKG/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/PKG/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3095 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/PKG/package_util.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.336296 biobookshelf-0.2.5/biobookshelf/RNA/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/RNA/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    19437 2023-05-01 11:20:30.000000 biobookshelf-0.2.5/biobookshelf/RNA/rnaseq.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.376297 biobookshelf-0.2.5/biobookshelf/SAM/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2022-04-04 14:27:31.000000 biobookshelf-0.2.5/biobookshelf/SAM/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    69402 2023-05-01 11:20:32.000000 biobookshelf-0.2.5/biobookshelf/SAM/sam_util.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.412297 biobookshelf-0.2.5/biobookshelf/SC/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/SC/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   122849 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/SC/single_cell.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.440298 biobookshelf-0.2.5/biobookshelf/SEQ/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/SEQ/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14831 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/SEQ/sequence.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.500299 biobookshelf-0.2.5/biobookshelf/STR/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/STR/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14367 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/STR/string.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.548300 biobookshelf-0.2.5/biobookshelf/UniProt/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2022-04-04 14:27:31.000000 biobookshelf-0.2.5/biobookshelf/UniProt/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      837 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/UniProt/uniprot.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.576301 biobookshelf-0.2.5/biobookshelf/WEB/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       31 2022-04-04 14:27:31.000000 biobookshelf-0.2.5/biobookshelf/WEB/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     8727 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/WEB/web_application.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.604301 biobookshelf-0.2.5/biobookshelf/ZA/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       26 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/ZA/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       12 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/ZA/zarr_utils.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      370 2023-05-09 04:54:53.000000 biobookshelf-0.2.5/biobookshelf/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      162 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/__main__.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.636302 biobookshelf-0.2.5/biobookshelf/main/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2022-04-18 07:53:18.000000 biobookshelf-0.2.5/biobookshelf/main/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   712244 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/main/unclassified_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.048290 biobookshelf-0.2.5/biobookshelf.egg-info/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-05-09 04:56:13.000000 biobookshelf-0.2.5/biobookshelf.egg-info/PKG-INFO
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     1538 2023-05-09 04:56:13.000000 biobookshelf-0.2.5/biobookshelf.egg-info/SOURCES.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        1 2023-05-09 04:56:13.000000 biobookshelf-0.2.5/biobookshelf.egg-info/dependency_links.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      394 2023-05-09 04:56:13.000000 biobookshelf-0.2.5/biobookshelf.egg-info/entry_points.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      480 2023-05-09 04:56:13.000000 biobookshelf-0.2.5/biobookshelf.egg-info/requires.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       13 2023-05-09 04:56:13.000000 biobookshelf-0.2.5/biobookshelf.egg-info/top_level.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2023-05-09 04:56:14.668303 biobookshelf-0.2.5/setup.cfg
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     2122 2023-05-09 04:55:14.000000 biobookshelf-0.2.5/setup.py
```

### Comparing `biobookshelf-0.2.4/LICENSE` & `biobookshelf-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/PKG-INFO` & `biobookshelf-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobookshelf
-Version: 0.2.4
+Version: 0.2.5
 Summary: a collection of python scripts and functions for exploratory analysis of bioinformatic data in Python
 Home-page: https://github.com/ahs2202/biobookshelf
 Author: Hyunsu An
 Author-email: ahs2202@gm.gist.ac.kr
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `biobookshelf-0.2.4/biobookshelf/BA/bitarray_utils.py` & `biobookshelf-0.2.5/biobookshelf/BA/bitarray_utils.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/biobookshelf/CLI/unclassified_programs.py` & `biobookshelf-0.2.5/biobookshelf/CLI/unclassified_programs.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/biobookshelf/MAP/mapping.py` & `biobookshelf-0.2.5/biobookshelf/MAP/mapping.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/biobookshelf/ONT/nanopore_functions.py` & `biobookshelf-0.2.5/biobookshelf/ONT/nanopore_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,25 @@
         n_threads=int_num_cpus,
         drop_unaligned=False,
         return_bash_shellscript=False,
         path_file_junc_bed=path_file_splice_junc,
     )  # perform alignment
 
 
-def create_gene_count_from_fast5(
+
+def create_gene_count_from_raw_ont_data(
     l_path_folder_nanopore_sequencing_data: Union[
         str, list, None
     ] = None,  # list of folders containing nanopore sequencing data
     l_name_config: Union[str, List] = None,  # a name of config or a list of name_config
     l_barcoding_kit: Union[
         str, List, None
     ] = None,  # a name of barcoding kit or a list of barcoding kits. if barcoding kits were not used, use None
     path_folder_output: Union[str, None] = None,  # a path to the output folder
-    dict_name_bc_to_name_sample: Union[dict, None] = None,  # barcode to name_sample
+    dict_name_bc_to_name_sample: Union[str, dict, None] = None,  # barcode to name_sample
     dict_name_sample_to_organism: Union[
         dict, None
     ] = None,  # define organism for each sample
     dict_anno: Union[
         dict, None
     ] = None,  # a dictionary containing annotation information for each organism
     int_num_cpus: Union[
@@ -51,20 +52,20 @@
     flag_include_failed: bool = True,  # include the failed reads into the fastq output
     int_max_num_reads_for_drawing_size_distribution: int = 100000,  # the maximum number of reads to use to draw a size distribution
     int_max_size_for_displaying_size_distribution: int = 2000,  # max molecule length to display in the histogram
     int_num_bins_for_displaying_size_distribution: int = 200,  # number of bins for drawing histogram
     flag_require_barcodes_both_ends: bool = True,  # require barcodes for both ends. if unclassified are too large, consider turning of this option to recover barcodes from the unclassified reads.
     flag_rerun_guppy=False,  # rename the the output folder (if it exists) and rerun guppy if the flag is True
 ):
-    """# 2023-05-05 17:16:59 
+    """# 2023-05-09 00:42:08 
     l_path_folder_nanopore_sequencing_data : list, # list of folders containing nanopore sequencing data
     l_name_config : Union[ str, List ], # a name of config or a list of name_config
     l_barcoding_kit : Union[ str, List, None ], # a name of barcoding kit or a list of barcoding kits. if barcoding kits were not used, use None
     path_folder_output : str, # a path to the output folder
-    dict_name_bc_to_name_sample : Union[ dict, None ], # barcode to name_sample. if not given, exit after combining fastq files.
+    dict_name_bc_to_name_sample : Union[ dict, str, None ], # barcode to name_sample. if not given, exit after combining fastq files. If barcoding is not used, a single string representing name of the sample can be given.
     dict_name_sample_to_organism : Union[ dict, None ], # define organism for each sample. if not given, does not align reads to genome and transcriptomes
     dict_anno : Union[ dict, None ], # a dictionary containing annotation information for each organism. if not given, does not align reads to genome and transcriptomes
     flag_include_failed : bool = True # include the failed reads into the fastq output
     int_max_num_reads_for_drawing_size_distribution : int = 100000 # the maximum number of reads to use to draw a size distribution
     int_max_size_for_displaying_size_distribution : int = 2000 # max molecule length to display in the histogram
     int_num_bins_for_displaying_size_distribution : int = 200 # number of bins for drawing histogram
     flag_require_barcodes_both_ends : bool = True, # require barcodes for both ends. if unclassified are too large, consider turning of this option to recover barcodes from the unclassified reads.
@@ -114,48 +115,58 @@
             e + ".cfg" if e[-4:] != ".cfg" else e for e in l_name_config
         )
         # match length
 
         for path_folder_nanopore_data, name_config, id_barcoding_kit in zip(
             l_path_folder_nanopore_sequencing_data, l_name_config, l_barcoding_kit
         ):
+            # retrieve a flag indicating the barcoding kit was used.
+            flag_barcoding = id_barcoding_kit is not None
+            # automatically detect output file type
+            raw_data_type = 'fast5' if len( glob.glob(f"{path_folder_nanopore_data}fast5*/") ) > 0 else 'pod5'
             # create folders
-            path_folder_fast5 = f"{path_folder_nanopore_data}fast5_all/"
+            path_folder_raw = f"{path_folder_nanopore_data}{raw_data_type}_all/"
             path_folder_guppy_output = f"{path_folder_nanopore_data}guppy_out/"
-            for path_folder in [path_folder_fast5, path_folder_guppy_output]:
+            for path_folder in [path_folder_raw, path_folder_guppy_output]:
                 os.makedirs(path_folder, exist_ok=True)
+            # if skipped raw data does not exist, indicating all raw data has been analyzed by MinKNOW, search for fastq output files and move the fastq output files to the guppy_out folder
+            if not os.path.exists(f"{path_folder_nanopore_data}{raw_data_type}_skip/") and len( glob.glob(f"{path_folder_nanopore_data}fastq*/") ) > 0 : # if skipped raw data does not exist and fastq output files exist, move these files into the guppy_out folder
+                bk.OS_Run( ["mv", f"{path_folder_nanopore_data}fastq_fail/", f"{path_folder_nanopore_data}guppy_out/fail/" ] ) 
+                bk.OS_Run( ["mv", f"{path_folder_nanopore_data}fastq_pass/", f"{path_folder_nanopore_data}guppy_out/pass/" ] ) 
+                with open( f"{path_folder_guppy_output}sequencing_summary.txt", 'w' ) as newfile : # create a file that functions as a flag.
+                    newfile.write( 'minknow output' )
 
-            # collect fast5 files
+            # collect raw output files
             for path_file in (
-                glob.glob(f"{path_folder_nanopore_data}fast5_skip/*.fast5")
-                + glob.glob(f"{path_folder_nanopore_data}fast5_fail/*/*.fast5")
-                + glob.glob(f"{path_folder_nanopore_data}fast5_pass/*/*.fast5")
+                glob.glob(f"{path_folder_nanopore_data}{raw_data_type}_skip/*.{raw_data_type}")
+                + glob.glob(f"{path_folder_nanopore_data}{raw_data_type}_fail/{'*/' if flag_barcoding else ''}*.{raw_data_type}")
+                + glob.glob(f"{path_folder_nanopore_data}{raw_data_type}_pass/{'*/' if flag_barcoding else ''}*.{raw_data_type}")
             ):
                 os.rename(
-                    path_file, f"{path_folder_fast5}{path_file.rsplit( '/', 1 )[ 1 ]}"
+                    path_file, f"{path_folder_raw}{bk.UUID( )}.{path_file.rsplit( '/', 1 )[ 1 ]}" # add uuid to avoid collision
                 )
 
             # run guppy
             l_args = [
                 "guppy_basecaller",
                 "-c",
                 name_config,
                 "--input_path",
-                path_folder_fast5,
+                path_folder_raw,
                 "--save_path",
                 path_folder_guppy_output,
                 "--device",
                 "auto",
                 "--compress_fastq",
             ]
             if (
                 flag_require_barcodes_both_ends
             ):  # if 'flag_require_barcodes_both_ends' is True
                 l_args += ["--require_barcodes_both_ends"]
-            if l_barcoding_kit is not None:  # if valid 'l_barcoding_kit' has been given
+            if id_barcoding_kit is not None:  # if valid 'id_barcoding_kit' has been given
                 l_args += ["--barcode_kits", id_barcoding_kit]
             print(" ".join(l_args))  # print the guppy_basecaller command
 
             flag_output_exists = os.path.exists(
                 f"{path_folder_guppy_output}sequencing_summary.txt"
             )  # retrieve a flag indicating that the guppy output folder already exists
             if (
@@ -179,47 +190,63 @@
             return
 
         # collect fastq files
         df_fq = pd.concat(
             list(
                 bk.GLOB_Retrive_Strings_in_Wildcards(
                     f"{path_folder_nanopore_data}guppy_out/*/"
-                    + ("*/" if id_barcoding_kit is not None else "")
+                    + ("*/" if flag_barcoding else "")
                     + "*.fastq.gz"
                 )
                 for path_folder_nanopore_data in l_path_folder_nanopore_sequencing_data
             )
         )
 
         # filter fastq files
         if not flag_include_failed:
             df_fq = PD_Select(df_fq, wildcard_0="pass")  # use only passed reads.
 
         # combine fastq files
-        for name_bc in df_fq.wildcard_1.unique():
-            df_fq_for_name_bc = bk.PD_Select(df_fq, wildcard_1=name_bc)
+        if flag_barcoding : # combine files for each barcode
+            for name_bc in df_fq.wildcard_1.unique():
+                df_fq_for_name_bc = bk.PD_Select(df_fq, wildcard_1=name_bc)
+                path_file_output= f"{path_folder_output}{name_bc}.fastq.gz"
+                path_file_temp = f"{path_folder_output}{name_bc}.fastq.gz.partial"
+                bk.OS_Run(
+                    ["cat"] + list(df_fq_for_name_bc.path.values),
+                    path_file_stdout=path_file_temp,
+                    stdout_binary=True,
+                ) # combine fastq files into a single temorary file
+                os.rename( path_file_temp, path_file_output ) # rename the temporary file to the output file
+        else :
+            path_file_output= f"{path_folder_output}combined.fastq.gz"
+            path_file_temp = f"{path_folder_output}combined.fastq.gz.partial"
             bk.OS_Run(
-                ["cat"] + list(df_fq_for_name_bc.path.values),
-                path_file_stdout=f"{path_folder_output}{name_bc}.fastq.gz",
+                ["cat"] + list(df_fq.path.values),
+                path_file_stdout=path_file_temp,
                 stdout_binary=True,
-            )
+            ) # combine fastq files into a single temorary file
+            os.rename( path_file_temp, path_file_output ) # rename the temporary file to the output file
 
     # if 'dict_name_bc_to_name_sample' has given, rename fastq files and remove files that are not needed.
     if dict_name_bc_to_name_sample is not None:
-        for path_file_fq in glob.glob(
-            f"{path_folder_pipeline}*.fastq.gz"
-        ):  # for each fastq file
-            name_file = path_file_fq.rsplit("/", 1)[1].rsplit(".fastq.gz", 1)[0]
-            if (
-                name_file in dict_name_bc_to_name_sample
-            ):  # if 'name_sample' is available for the barcode, rename the file
-                name_sample = dict_name_bc_to_name_sample[name_file]
-                os.rename(path_file_fq, f"{path_folder_pipeline}{name_sample}.fastq.gz")
-            else:  # if 'name_sample' is not available for the barcode, remove the file
-                os.remove(path_file_fq)
+        if flag_barcoding and isinstance( dict_name_bc_to_name_sample, dict ) :
+            for path_file_fq in glob.glob(
+                f"{path_folder_pipeline}*.fastq.gz"
+            ):  # for each fastq file
+                name_file = path_file_fq.rsplit("/", 1)[1].rsplit(".fastq.gz", 1)[0]
+                if (
+                    name_file in dict_name_bc_to_name_sample
+                ):  # if 'name_sample' is available for the barcode, rename the file
+                    name_sample = dict_name_bc_to_name_sample[name_file]
+                    os.rename(path_file_fq, f"{path_folder_pipeline}{name_sample}.fastq.gz")
+                else:  # if 'name_sample' is not available for the barcode, remove the file
+                    os.remove(path_file_fq)
+        elif not flag_barcoding and isinstance( dict_name_bc_to_name_sample, str ) : # if barcoding was not used.
+            os.rename(f"{path_folder_pipeline}combined.fastq.gz", f"{path_folder_pipeline}{dict_name_bc_to_name_sample}.fastq.gz")
 
     # draw molecule length distribution of each sample
     df_fastq = bk.GLOB_Retrive_Strings_in_Wildcards(
         f"{path_folder_pipeline}*.fastq.gz"
     )  # retrieve the paths of input fastq files
     int_num_samples = len(
         df_fastq
@@ -423,46 +450,77 @@
         df_count.to_excel(
             f"{path_folder_processed_data}{name_sample}.alignment_summary.gene_level.xlsx"
         )  # output excel file
         df_count.to_csv(
             f"{path_folder_processed_data}{name_sample}.alignment_summary.gene_level.tsv.gz",
             sep="\t",
         )  # output tsv file
-        
+
         # calculate accumulated sequencing throughput to determine library diversity
-        s_sequencing_throughput = df_count.gene_count * df_count.average_length_of_read # retrieve total number of base pairs for each entry
-        s_sequencing_throughput_proportion = ( s_sequencing_throughput / s_sequencing_throughput.sum( ) ).sort_values( ascending = False )
-        df_accumulated_throughput = pd.concat( [ 
-            pd.DataFrame( { 
-                'accumulated proportions of sequencing throughput' : [ 0 ], 
-                'number of covered genes' : [ 0 ], 
-                'proportion of sequencing throughput' : [ 0 ], 
-                'gene name' : [ '-' ]
-            } ),
-            pd.DataFrame( { 
-                'accumulated proportions of sequencing throughput' : np.cumsum( s_sequencing_throughput_proportion.values ), 
-                'number of covered genes' : np.arange( len( s_sequencing_throughput_proportion ) ) + 1, 
-                'proportion of sequencing throughput' : s_sequencing_throughput_proportion.values, 
-                'gene name' : s_sequencing_throughput_proportion.index.values
-            } ),
-        ] )
+        s_sequencing_throughput = (
+            df_count.gene_count * df_count.average_length_of_read
+        )  # retrieve total number of base pairs for each entry
+        s_sequencing_throughput_proportion = (
+            s_sequencing_throughput / s_sequencing_throughput.sum()
+        ).sort_values(ascending=False)
+        df_accumulated_throughput = pd.concat(
+            [
+                pd.DataFrame(
+                    {
+                        "accumulated proportions of sequencing throughput": [0],
+                        "number of covered genes": [0],
+                        "proportion of sequencing throughput": [0],
+                        "gene name": ["-"],
+                    }
+                ),
+                pd.DataFrame(
+                    {
+                        "accumulated proportions of sequencing throughput": np.cumsum(
+                            s_sequencing_throughput_proportion.values
+                        ),
+                        "number of covered genes": np.arange(
+                            len(s_sequencing_throughput_proportion)
+                        )
+                        + 1,
+                        "proportion of sequencing throughput": s_sequencing_throughput_proportion.values,
+                        "gene name": s_sequencing_throughput_proportion.index.values,
+                    }
+                ),
+            ]
+        )
         # write result as files
         df_accumulated_throughput.to_excel(
             f"{path_folder_processed_data}{name_sample}.(supplementary).accumulated_sequencing_throughput.gene_level.xlsx"
         )  # output excel file
         df_accumulated_throughput.to_csv(
             f"{path_folder_processed_data}{name_sample}.(supplementary).accumulated_sequencing_throughput.gene_level.tsv.gz",
             sep="\t",
         )  # output tsv file
-        
+
         # draw graph
-        float_area_under_the_curve = np.cumsum( s_sequencing_throughput_proportion.values ).mean( ) # calculate area under the curve, which indicates higher library diversity
-        fig = px.line( df_accumulated_throughput, y = 'accumulated proportions of sequencing throughput', x = 'number of covered genes', log_y = False, line_shape='vh', hover_data = [ 'gene name', 'proportion of sequencing throughput' ], title = f"Area Under the Curve (AUC) = {np.round( float_area_under_the_curve, 5 )}<br>(lower AUC indicates higher library diversity)" )
-        os.makedirs( f'{path_folder_graph}accumulated_sequencing_throughput/', exist_ok = True ) # create the output folder
-        fig.write_html( f'{path_folder_graph}accumulated_sequencing_throughput/{name_sample}.accumulated_sequencing_throughput.gene_level.html' ) # write the graph
+        float_area_under_the_curve = np.cumsum(
+            s_sequencing_throughput_proportion.values
+        ).mean()  # calculate area under the curve, which indicates higher library diversity
+        fig = px.line(
+            df_accumulated_throughput,
+            y="accumulated proportions of sequencing throughput",
+            x="number of covered genes",
+            log_y=False,
+            line_shape="vh",
+            hover_data=["gene name", "proportion of sequencing throughput"],
+            title=f"Area Under the Curve (AUC) = {np.round( float_area_under_the_curve, 5 )}<br>(lower AUC indicates higher library diversity)",
+        )
+        os.makedirs(
+            f"{path_folder_graph}accumulated_sequencing_throughput/", exist_ok=True
+        )  # create the output folder
+        fig.write_html(
+            f"{path_folder_graph}accumulated_sequencing_throughput/{name_sample}.accumulated_sequencing_throughput.gene_level.html"
+        )  # write the graph
+create_gene_count_from_fast5 = create_gene_count_from_raw_ont_data
+
 
 def Guppy_Run_and_Combine_Output(
     path_folder_nanopore_sequencing_data=None,
     flag_barcoding_was_used=False,
     path_folder_output_fastq=None,
     id_flowcell=None,
     id_lib_prep=None,
```

### Comparing `biobookshelf-0.2.4/biobookshelf/PDB/pdb.py` & `biobookshelf-0.2.5/biobookshelf/PDB/pdb.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/biobookshelf/PKG/package_util.py` & `biobookshelf-0.2.5/biobookshelf/PKG/package_util.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/biobookshelf/RNA/rnaseq.py` & `biobookshelf-0.2.5/biobookshelf/RNA/rnaseq.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/biobookshelf/SAM/sam_util.py` & `biobookshelf-0.2.5/biobookshelf/SAM/sam_util.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/biobookshelf/SC/single_cell.py` & `biobookshelf-0.2.5/biobookshelf/SC/single_cell.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/biobookshelf/SEQ/sequence.py` & `biobookshelf-0.2.5/biobookshelf/SEQ/sequence.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/biobookshelf/STR/string.py` & `biobookshelf-0.2.5/biobookshelf/STR/string.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/biobookshelf/UniProt/uniprot.py` & `biobookshelf-0.2.5/biobookshelf/UniProt/uniprot.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/biobookshelf/WEB/web_application.py` & `biobookshelf-0.2.5/biobookshelf/WEB/web_application.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/biobookshelf/main/unclassified_functions.py` & `biobookshelf-0.2.5/biobookshelf/main/unclassified_functions.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/biobookshelf.egg-info/PKG-INFO` & `biobookshelf-0.2.5/biobookshelf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobookshelf
-Version: 0.2.4
+Version: 0.2.5
 Summary: a collection of python scripts and functions for exploratory analysis of bioinformatic data in Python
 Home-page: https://github.com/ahs2202/biobookshelf
 Author: Hyunsu An
 Author-email: ahs2202@gm.gist.ac.kr
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `biobookshelf-0.2.4/biobookshelf.egg-info/SOURCES.txt` & `biobookshelf-0.2.5/biobookshelf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.4/setup.py` & `biobookshelf-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="biobookshelf",
-    version="0.2.4",
+    version="0.2.5",
     author="Hyunsu An",
     author_email="ahs2202@gm.gist.ac.kr",
     description="a collection of python scripts and functions for exploratory analysis of bioinformatic data in Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/ahs2202/biobookshelf",
     license="GPLv3",
```

