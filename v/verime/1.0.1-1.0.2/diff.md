# Comparing `tmp/verime-1.0.1.tar.gz` & `tmp/verime-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verime-1.0.1.tar", last modified: Wed May  3 08:27:39 2023, max compression
+gzip compressed data, was "verime-1.0.2.tar", last modified: Tue May  9 16:13:45 2023, max compression
```

## Comparing `verime-1.0.1.tar` & `verime-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 gcassiers  (1000) gcassiers  (1000)        0 2023-05-03 08:27:39.696207 verime-1.0.1/
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)    35150 2023-04-24 15:38:24.000000 verime-1.0.1/COPYING
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)    15844 2023-05-03 08:27:39.696207 verime-1.0.1/PKG-INFO
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)    15651 2023-04-26 13:48:09.000000 verime-1.0.1/README.md
--rw-------   0 gcassiers  (1000) gcassiers  (1000)      105 2022-08-19 12:06:44.000000 verime-1.0.1/pyproject.toml
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)      562 2023-05-03 08:27:39.696207 verime-1.0.1/setup.cfg
-drwxrwxr-x   0 gcassiers  (1000) gcassiers  (1000)        0 2023-05-03 08:27:39.692207 verime-1.0.1/src/
-drwxrwxr-x   0 gcassiers  (1000) gcassiers  (1000)        0 2023-05-03 08:27:39.692207 verime-1.0.1/src/verime/
--rw-------   0 gcassiers  (1000) gcassiers  (1000)        0 2022-08-19 12:06:44.000000 verime-1.0.1/src/verime/__init__.py
-drwxrwxr-x   0 gcassiers  (1000) gcassiers  (1000)        0 2023-05-03 08:27:39.696207 verime-1.0.1/src/verime/data/
--rw-------   0 gcassiers  (1000) gcassiers  (1000)       17 2022-08-25 13:26:09.000000 verime-1.0.1/src/verime/data/MANIFEST.in
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     6214 2023-05-03 08:25:39.000000 verime-1.0.1/src/verime/data/pymod.cpp
--rw-------   0 gcassiers  (1000) gcassiers  (1000)      105 2022-08-25 12:04:43.000000 verime-1.0.1/src/verime/data/pyproject.toml
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     5553 2023-05-03 08:25:39.000000 verime-1.0.1/src/verime/data/pysimu.py
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)       36 2023-05-03 08:25:39.000000 verime-1.0.1/src/verime/data/setup.cfg
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     1656 2023-05-03 08:25:39.000000 verime-1.0.1/src/verime/data/setup.py
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     2607 2023-04-24 15:38:24.000000 verime-1.0.1/src/verime/data/simulation_runner.cpp
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     1551 2023-04-24 15:38:24.000000 verime-1.0.1/src/verime/data/simulation_runner.h
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     1160 2023-05-02 18:05:23.000000 verime-1.0.1/src/verime/data/template_makefile.mk
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)    28025 2023-05-03 08:25:39.000000 verime-1.0.1/src/verime/verime.py
-drwxrwxr-x   0 gcassiers  (1000) gcassiers  (1000)        0 2023-05-03 08:27:39.696207 verime-1.0.1/src/verime.egg-info/
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)    15844 2023-05-03 08:27:39.000000 verime-1.0.1/src/verime.egg-info/PKG-INFO
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)      565 2023-05-03 08:27:39.000000 verime-1.0.1/src/verime.egg-info/SOURCES.txt
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)        1 2023-05-03 08:27:39.000000 verime-1.0.1/src/verime.egg-info/dependency_links.txt
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)       46 2023-05-03 08:27:39.000000 verime-1.0.1/src/verime.egg-info/entry_points.txt
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)       60 2023-05-03 08:27:39.000000 verime-1.0.1/src/verime.egg-info/requires.txt
--rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)        7 2023-05-03 08:27:39.000000 verime-1.0.1/src/verime.egg-info/top_level.txt
+drwxrwxr-x   0 gcassiers  (1000) gcassiers  (1000)        0 2023-05-09 16:13:45.866945 verime-1.0.2/
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)    35150 2023-04-24 15:38:24.000000 verime-1.0.2/COPYING
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     1760 2023-05-09 16:13:45.866945 verime-1.0.2/PKG-INFO
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)    15651 2023-04-26 13:48:09.000000 verime-1.0.2/README.md
+-rw-------   0 gcassiers  (1000) gcassiers  (1000)      105 2022-08-19 12:06:44.000000 verime-1.0.2/pyproject.toml
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     2119 2023-05-09 16:13:45.866945 verime-1.0.2/setup.cfg
+drwxrwxr-x   0 gcassiers  (1000) gcassiers  (1000)        0 2023-05-09 16:13:45.862945 verime-1.0.2/src/
+drwxrwxr-x   0 gcassiers  (1000) gcassiers  (1000)        0 2023-05-09 16:13:45.862945 verime-1.0.2/src/verime/
+-rw-------   0 gcassiers  (1000) gcassiers  (1000)        0 2022-08-19 12:06:44.000000 verime-1.0.2/src/verime/__init__.py
+drwxrwxr-x   0 gcassiers  (1000) gcassiers  (1000)        0 2023-05-09 16:13:45.866945 verime-1.0.2/src/verime/data/
+-rw-------   0 gcassiers  (1000) gcassiers  (1000)       17 2022-08-25 13:26:09.000000 verime-1.0.2/src/verime/data/MANIFEST.in
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     6214 2023-05-03 08:25:39.000000 verime-1.0.2/src/verime/data/pymod.cpp
+-rw-------   0 gcassiers  (1000) gcassiers  (1000)      105 2022-08-25 12:04:43.000000 verime-1.0.2/src/verime/data/pyproject.toml
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     5553 2023-05-03 08:25:39.000000 verime-1.0.2/src/verime/data/pysimu.py
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)       36 2023-05-03 08:25:39.000000 verime-1.0.2/src/verime/data/setup.cfg
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     1656 2023-05-03 08:25:39.000000 verime-1.0.2/src/verime/data/setup.py
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     2607 2023-04-24 15:38:24.000000 verime-1.0.2/src/verime/data/simulation_runner.cpp
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     1551 2023-04-24 15:38:24.000000 verime-1.0.2/src/verime/data/simulation_runner.h
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     1160 2023-05-02 18:05:23.000000 verime-1.0.2/src/verime/data/template_makefile.mk
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)    28025 2023-05-03 08:25:39.000000 verime-1.0.2/src/verime/verime.py
+drwxrwxr-x   0 gcassiers  (1000) gcassiers  (1000)        0 2023-05-09 16:13:45.866945 verime-1.0.2/src/verime.egg-info/
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)     1760 2023-05-09 16:13:45.000000 verime-1.0.2/src/verime.egg-info/PKG-INFO
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)      565 2023-05-09 16:13:45.000000 verime-1.0.2/src/verime.egg-info/SOURCES.txt
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)        1 2023-05-09 16:13:45.000000 verime-1.0.2/src/verime.egg-info/dependency_links.txt
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)       46 2023-05-09 16:13:45.000000 verime-1.0.2/src/verime.egg-info/entry_points.txt
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)       60 2023-05-09 16:13:45.000000 verime-1.0.2/src/verime.egg-info/requires.txt
+-rw-rw-r--   0 gcassiers  (1000) gcassiers  (1000)        7 2023-05-09 16:13:45.000000 verime-1.0.2/src/verime.egg-info/top_level.txt
```

### Comparing `verime-1.0.1/COPYING` & `verime-1.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `verime-1.0.1/PKG-INFO` & `verime-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: verime
-Version: 1.0.1
-Author: 'Charles Momin, Gaëtan Cassiers'
-License: GPLv3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: COPYING
-
 # Verime 
 
 In the context of the side-channel analysis of hardware implementations, an evaluator usually requires to have access to the internal values of a target circuitry. For this purpose, a circuit oracle simulating these values is implemented, which may turn out to be time consuming to do manually (e.g., each probed internal value should be modeled and any modification of the original circuitry implies to rewrite the circuit oracle) and/or achieve poor performances (e.g., spawning a simulator process for each simulation).
 
 The Verime tool is proposed to tackle these issues. In particular, it automatically generates a prediction library of a circuit (described in Verilog). More precisely, it performs behavioral verilog simulations during an arbitrary amount of clock cycles thanks to a Verilator backend. Verilator is a powerful tool, but requires some expertise and predicting certain internal states using the `\* verilator public *\` pragma can be challenging and time consuming to setup for a non-experienced user. Based on that, the Verime tools acts as a wrapper for verilator and aims to (significantly) reduce the evaluator work: it automatically generates the C++ Verilator backend code and generates a user friendly python package thant can be easily integrated and used. 
 
 The advantages over "raw" Verilator usage are:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `verime-1.0.1/src/verime/data/pymod.cpp` & `verime-1.0.2/src/verime/data/pymod.cpp`

 * *Files identical despite different names*

### Comparing `verime-1.0.1/src/verime/data/pysimu.py` & `verime-1.0.2/src/verime/data/pysimu.py`

 * *Files identical despite different names*

### Comparing `verime-1.0.1/src/verime/data/setup.py` & `verime-1.0.2/src/verime/data/setup.py`

 * *Files identical despite different names*

### Comparing `verime-1.0.1/src/verime/data/simulation_runner.cpp` & `verime-1.0.2/src/verime/data/simulation_runner.cpp`

 * *Files identical despite different names*

### Comparing `verime-1.0.1/src/verime/data/simulation_runner.h` & `verime-1.0.2/src/verime/data/simulation_runner.h`

 * *Files identical despite different names*

### Comparing `verime-1.0.1/src/verime/data/template_makefile.mk` & `verime-1.0.2/src/verime/data/template_makefile.mk`

 * *Files identical despite different names*

### Comparing `verime-1.0.1/src/verime/verime.py` & `verime-1.0.2/src/verime/verime.py`

 * *Files identical despite different names*

### Comparing `verime-1.0.1/src/verime.egg-info/SOURCES.txt` & `verime-1.0.2/src/verime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

