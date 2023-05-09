# Comparing `tmp/floret-0.10.2.tar.gz` & `tmp/floret-0.10.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floret-0.10.2.tar", last modified: Tue Feb 15 13:02:19 2022, max compression
+gzip compressed data, was "floret-0.10.3.tar", last modified: Tue May  9 06:21:25 2023, max compression
```

## Comparing `floret-0.10.2.tar` & `floret-0.10.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-15 13:02:19.903191 floret-0.10.2/
--rw-r--r--   0 vsts      (1001) docker     (121)     1111 2022-02-15 13:02:14.000000 floret-0.10.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)       85 2022-02-15 13:02:14.000000 floret-0.10.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     2983 2022-02-15 13:02:19.903191 floret-0.10.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)    19776 2022-02-15 13:02:14.000000 floret-0.10.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)      111 2022-02-15 13:02:14.000000 floret-0.10.2/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-15 13:02:19.899191 floret-0.10.2/python/
--rw-r--r--   0 vsts      (1001) docker     (121)     2063 2022-02-15 13:02:14.000000 floret-0.10.2/python/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-15 13:02:19.899191 floret-0.10.2/python/floret_module/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-15 13:02:19.899191 floret-0.10.2/python/floret_module/floret/
--rw-r--r--   0 vsts      (1001) docker     (121)      639 2022-02-15 13:02:14.000000 floret-0.10.2/python/floret_module/floret/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    20068 2022-02-15 13:02:14.000000 floret-0.10.2/python/floret_module/floret/floret.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-15 13:02:19.899191 floret-0.10.2/python/floret_module/floret/pybind/
--rw-r--r--   0 vsts      (1001) docker     (121)    20431 2022-02-15 13:02:14.000000 floret-0.10.2/python/floret_module/floret/pybind/floret_pybind.cc
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-15 13:02:19.899191 floret-0.10.2/python/floret_module/floret/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)      102 2022-02-15 13:02:14.000000 floret-0.10.2/python/floret_module/floret/tests/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)      475 2022-02-15 13:02:14.000000 floret-0.10.2/python/floret_module/floret/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10914 2022-02-15 13:02:14.000000 floret-0.10.2/python/floret_module/floret/tests/data.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     7060 2022-02-15 13:02:14.000000 floret-0.10.2/python/floret_module/floret/tests/test_configurations.py
--rw-r--r--   0 vsts      (1001) docker     (121)    21765 2022-02-15 13:02:14.000000 floret-0.10.2/python/floret_module/floret/tests/test_script.py
--rw-r--r--   0 vsts      (1001) docker     (121)       96 2022-02-15 13:02:14.000000 floret-0.10.2/python/floret_module/floret/tests/test_tokenize.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2111 2022-02-15 13:02:14.000000 floret-0.10.2/python/floret_module/floret/tests/test_train.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-15 13:02:19.899191 floret-0.10.2/python/floret_module/floret/util/
--rw-r--r--   0 vsts      (1001) docker     (121)      472 2022-02-15 13:02:14.000000 floret-0.10.2/python/floret_module/floret/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7490 2022-02-15 13:02:14.000000 floret-0.10.2/python/floret_module/floret/util/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-15 13:02:19.899191 floret-0.10.2/python/floret_module/floret.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     2983 2022-02-15 13:02:19.000000 floret-0.10.2/python/floret_module/floret.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1392 2022-02-15 13:02:19.000000 floret-0.10.2/python/floret_module/floret.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-02-15 13:02:19.000000 floret-0.10.2/python/floret_module/floret.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-02-15 13:02:19.000000 floret-0.10.2/python/floret_module/floret.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)        6 2022-02-15 13:02:19.000000 floret-0.10.2/python/floret_module/floret.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       21 2022-02-15 13:02:19.000000 floret-0.10.2/python/floret_module/floret.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       79 2022-02-15 13:02:19.903191 floret-0.10.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)     5975 2022-02-15 13:02:14.000000 floret-0.10.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-15 13:02:19.903191 floret-0.10.2/src/
--rw-r--r--   0 vsts      (1001) docker     (121)     8609 2022-02-15 13:02:14.000000 floret-0.10.2/src/MurmurHash3.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      804 2022-02-15 13:02:14.000000 floret-0.10.2/src/MurmurHash3.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17847 2022-02-15 13:02:14.000000 floret-0.10.2/src/args.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     2309 2022-02-15 13:02:14.000000 floret-0.10.2/src/args.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13879 2022-02-15 13:02:14.000000 floret-0.10.2/src/autotune.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     2266 2022-02-15 13:02:14.000000 floret-0.10.2/src/autotune.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4230 2022-02-15 13:02:14.000000 floret-0.10.2/src/densematrix.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     2155 2022-02-15 13:02:14.000000 floret-0.10.2/src/densematrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15049 2022-02-15 13:02:14.000000 floret-0.10.2/src/dictionary.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     3219 2022-02-15 13:02:14.000000 floret-0.10.2/src/dictionary.h
--rw-r--r--   0 vsts      (1001) docker     (121)    25809 2022-02-15 13:02:14.000000 floret-0.10.2/src/fasttext.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     4819 2022-02-15 13:02:14.000000 floret-0.10.2/src/fasttext.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9124 2022-02-15 13:02:14.000000 floret-0.10.2/src/loss.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     3879 2022-02-15 13:02:14.000000 floret-0.10.2/src/loss.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12928 2022-02-15 13:02:14.000000 floret-0.10.2/src/main.cc
--rw-r--r--   0 vsts      (1001) docker     (121)      494 2022-02-15 13:02:14.000000 floret-0.10.2/src/matrix.cc
--rw-r--r--   0 vsts      (1001) docker     (121)      972 2022-02-15 13:02:14.000000 floret-0.10.2/src/matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6129 2022-02-15 13:02:14.000000 floret-0.10.2/src/meter.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     2510 2022-02-15 13:02:14.000000 floret-0.10.2/src/meter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2271 2022-02-15 13:02:14.000000 floret-0.10.2/src/model.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1720 2022-02-15 13:02:14.000000 floret-0.10.2/src/model.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6234 2022-02-15 13:02:14.000000 floret-0.10.2/src/productquantizer.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1607 2022-02-15 13:02:14.000000 floret-0.10.2/src/productquantizer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3370 2022-02-15 13:02:14.000000 floret-0.10.2/src/quantmatrix.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1474 2022-02-15 13:02:14.000000 floret-0.10.2/src/quantmatrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)      266 2022-02-15 13:02:14.000000 floret-0.10.2/src/real.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1275 2022-02-15 13:02:14.000000 floret-0.10.2/src/utils.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1722 2022-02-15 13:02:14.000000 floret-0.10.2/src/utils.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1961 2022-02-15 13:02:14.000000 floret-0.10.2/src/vector.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     1273 2022-02-15 13:02:14.000000 floret-0.10.2/src/vector.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.487887 floret-0.10.3/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1111 2023-05-09 06:21:09.000000 floret-0.10.3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-05-09 06:21:09.000000 floret-0.10.3/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     2968 2023-05-09 06:21:25.487887 floret-0.10.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    20392 2023-05-09 06:21:09.000000 floret-0.10.3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-05-09 06:21:09.000000 floret-0.10.3/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.483886 floret-0.10.3/python/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2068 2023-05-09 06:21:09.000000 floret-0.10.3/python/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.479886 floret-0.10.3/python/floret_module/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.483886 floret-0.10.3/python/floret_module/floret/
+-rw-r--r--   0 vsts      (1001) docker     (122)      639 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20068 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/floret.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.483886 floret-0.10.3/python/floret_module/floret/pybind/
+-rw-r--r--   0 vsts      (1001) docker     (122)    20431 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/pybind/floret_pybind.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.483886 floret-0.10.3/python/floret_module/floret/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      475 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10914 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/data.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     7060 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/test_configurations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21765 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/test_script.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       96 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/test_tokenize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2111 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/test_train.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.483886 floret-0.10.3/python/floret_module/floret/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      472 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7490 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/util/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.483886 floret-0.10.3/python/floret_module/floret.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2968 2023-05-09 06:21:25.000000 floret-0.10.3/python/floret_module/floret.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1392 2023-05-09 06:21:25.000000 floret-0.10.3/python/floret_module/floret.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-09 06:21:25.000000 floret-0.10.3/python/floret_module/floret.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-09 06:21:25.000000 floret-0.10.3/python/floret_module/floret.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)        6 2023-05-09 06:21:25.000000 floret-0.10.3/python/floret_module/floret.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-05-09 06:21:25.000000 floret-0.10.3/python/floret_module/floret.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       79 2023-05-09 06:21:25.487887 floret-0.10.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     5975 2023-05-09 06:21:09.000000 floret-0.10.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.487887 floret-0.10.3/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     8609 2023-05-09 06:21:09.000000 floret-0.10.3/src/MurmurHash3.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      804 2023-05-09 06:21:09.000000 floret-0.10.3/src/MurmurHash3.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    17847 2023-05-09 06:21:09.000000 floret-0.10.3/src/args.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2309 2023-05-09 06:21:09.000000 floret-0.10.3/src/args.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    13879 2023-05-09 06:21:09.000000 floret-0.10.3/src/autotune.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2266 2023-05-09 06:21:09.000000 floret-0.10.3/src/autotune.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4230 2023-05-09 06:21:09.000000 floret-0.10.3/src/densematrix.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2155 2023-05-09 06:21:09.000000 floret-0.10.3/src/densematrix.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    15049 2023-05-09 06:21:09.000000 floret-0.10.3/src/dictionary.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3219 2023-05-09 06:21:09.000000 floret-0.10.3/src/dictionary.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    25809 2023-05-09 06:21:09.000000 floret-0.10.3/src/fasttext.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4819 2023-05-09 06:21:09.000000 floret-0.10.3/src/fasttext.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     9124 2023-05-09 06:21:09.000000 floret-0.10.3/src/loss.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3879 2023-05-09 06:21:09.000000 floret-0.10.3/src/loss.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12928 2023-05-09 06:21:09.000000 floret-0.10.3/src/main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)      494 2023-05-09 06:21:09.000000 floret-0.10.3/src/matrix.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-05-09 06:21:09.000000 floret-0.10.3/src/matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6129 2023-05-09 06:21:09.000000 floret-0.10.3/src/meter.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2510 2023-05-09 06:21:09.000000 floret-0.10.3/src/meter.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2271 2023-05-09 06:21:09.000000 floret-0.10.3/src/model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1720 2023-05-09 06:21:09.000000 floret-0.10.3/src/model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6234 2023-05-09 06:21:09.000000 floret-0.10.3/src/productquantizer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1607 2023-05-09 06:21:09.000000 floret-0.10.3/src/productquantizer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3370 2023-05-09 06:21:09.000000 floret-0.10.3/src/quantmatrix.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1474 2023-05-09 06:21:09.000000 floret-0.10.3/src/quantmatrix.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      266 2023-05-09 06:21:09.000000 floret-0.10.3/src/real.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1275 2023-05-09 06:21:09.000000 floret-0.10.3/src/utils.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1722 2023-05-09 06:21:09.000000 floret-0.10.3/src/utils.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1961 2023-05-09 06:21:09.000000 floret-0.10.3/src/vector.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1273 2023-05-09 06:21:09.000000 floret-0.10.3/src/vector.h
```

### Comparing `floret-0.10.2/LICENSE` & `floret-0.10.3/LICENSE`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/PKG-INFO` & `floret-0.10.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: floret
-Version: 0.10.2
+Version: 0.10.3
 Summary: floret Python bindings
 Home-page: https://github.com/explosion/floret
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -86,20 +85,18 @@
 fastText vectors.
 
 ## Use floret vectors in spaCy
 
 Import floret vectors into spaCy v3.2+:
 
 ```bash
-spacy init vectors --mode floret vectors.floret spacy_vectors_model
+spacy init vectors LANG vectors.floret spacy_vectors_model --mode floret
 ```
 
 ## Notes
 
 `floret` contains all features of the original [`fasttext`
-module](https://pypi.org/project/fasttest). See the [`fasttext`
+module](https://pypi.org/project/fasttext). See the [`fasttext`
 docs](https://fasttext.cc/docs/en/python-module.html) for more information.
 
 The `fasttext` and `floret` binary formats saved with
 `model.save_model("model.bin")` are not compatible.
-
-
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: floret Version: 0.10.2 Summary: floret Python
+Metadata-Version: 2.1 Name: floret Version: 0.10.3 Summary: floret Python
 bindings Home-page: https://github.com/explosion/floret Author: Explosion
-Author-email: contact@explosion.ai License: MIT Platform: UNKNOWN Classifier:
-Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development Classifier: Topic :: Scientific/
-Engineering Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: POSIX Classifier: Operating System :: Unix Classifier:
-Operating System :: MacOS Description-Content-Type: text/markdown License-File:
-LICENSE [https://explosion.ai/assets/img/logo.svg] # floret: fastText + Bloom
-embeddings for compact, full-coverage vectors with spaCy floret is an extended
-version of [fastText](https://fasttext.cc) that can produce word
-representations for any word from a compact vector table. It combines: -
-fastText's subwords to provide embeddings for any word - Bloom embeddings
-("hashing trick") for a compact vector table ## Installation ```bash pip
-install floret ``` ## Usage Train floret vectors using the options: - `mode`:
-`"floret"`, storing both words and subwords in the same compact hash table -
-`hashCount`: store each entry in 1-4 rows in the hash table (recommended: `2`)
-- `bucket`: in combination with `hashCount>1`, the size of the hash table can
-be greatly reduced (recommended: `25000`--`100000`, reduced from the fastText
-default of `2000000`) - `minn`: min length of char ngram (default: `3`) -
-`maxn`: max length of char ngram (default: `6`) ```python import floret # train
-vectors model = floret.train_unsupervised( "data.txt", model="cbow",
-mode="floret", hashCount=2, bucket=50000, minn=3, maxn=6, ) # query vector
+Author-email: contact@explosion.ai License: MIT Classifier: Development Status
+:: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
+Development Classifier: Topic :: Scientific/Engineering Classifier: Operating
+System :: Microsoft :: Windows Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix Classifier: Operating System :: MacOS
+Description-Content-Type: text/markdown License-File: LICENSE [https://
+explosion.ai/assets/img/logo.svg] # floret: fastText + Bloom embeddings for
+compact, full-coverage vectors with spaCy floret is an extended version of
+[fastText](https://fasttext.cc) that can produce word representations for any
+word from a compact vector table. It combines: - fastText's subwords to provide
+embeddings for any word - Bloom embeddings ("hashing trick") for a compact
+vector table ## Installation ```bash pip install floret ``` ## Usage Train
+floret vectors using the options: - `mode`: `"floret"`, storing both words and
+subwords in the same compact hash table - `hashCount`: store each entry in 1-
+4 rows in the hash table (recommended: `2`) - `bucket`: in combination with
+`hashCount>1`, the size of the hash table can be greatly reduced (recommended:
+`25000`--`100000`, reduced from the fastText default of `2000000`) - `minn`:
+min length of char ngram (default: `3`) - `maxn`: max length of char ngram
+(default: `6`) ```python import floret # train vectors model =
+floret.train_unsupervised( "data.txt", model="cbow", mode="floret",
+hashCount=2, bucket=50000, minn=3, maxn=6, ) # query vector
 model.get_word_vector("broccoli") # save full model model.save_model
 ("vectors.bin") # export standard word-only vector table model.save_vectors
 ("vectors.vec") # export floret vector table model.save_floret_vectors
 ("vectors.floret") ``` **Note:** with the default setting `mode="fasttext"`,
 `floret` trains original fastText vectors. ## Use floret vectors in spaCy
-Import floret vectors into spaCy v3.2+: ```bash spacy init vectors --mode
-floret vectors.floret spacy_vectors_model ``` ## Notes `floret` contains all
-features of the original [`fasttext` module](https://pypi.org/project/
-fasttest). See the [`fasttext` docs](https://fasttext.cc/docs/en/python-
+Import floret vectors into spaCy v3.2+: ```bash spacy init vectors LANG
+vectors.floret spacy_vectors_model --mode floret ``` ## Notes `floret` contains
+all features of the original [`fasttext` module](https://pypi.org/project/
+fasttext). See the [`fasttext` docs](https://fasttext.cc/docs/en/python-
 module.html) for more information. The `fasttext` and `floret` binary formats
 saved with `model.save_model("model.bin")` are not compatible.
```

### Comparing `floret-0.10.2/README.md` & `floret-0.10.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,24 @@
 floret is an extended version of [fastText](https://fasttext.cc) that can
 produce word representations for any word from a compact vector table. It
 combines:
 
 - fastText's subwords to provide embeddings for any word
 - Bloom embeddings ("hashing trick") for a compact vector table
 
+To learn more about floret, check out our [blog post on floret vectors](https://explosion.ai/blog/floret-vectors).
+
+For a hands-on introduction, experiment with English vectors in this example
+notebook: [`intro_to_floret`][intro_to_floret] [![Open in
+Colab][colab]][intro_to_floret_colab]
+
+[colab]: https://gistcdn.githack.com/ines/dcf354aa71a7665ae19871d7fd14a4e0/raw/461fc1f61a7bc5860f943cd4b6bcfabb8c8906e7/colab-badge.svg
+[intro_to_floret]: examples/01_intro_to_floret.ipynb
+[intro_to_floret_colab]: https://colab.research.google.com/github/explosion/floret/blob/main/examples/01_intro_to_floret.ipynb
+
 ## Install floret
 
 ### Build floret from source
 
 ```bash
 git clone https://github.com/explosion/floret
 cd floret
@@ -73,29 +83,29 @@
 header line followed by one line per vector. The word tokens are replaced with
 the index of the row and the header is extended to contain all the relevant
 training settings needed to load this table in spaCy.
 
 To import this vector table in [spaCy](https://spacy.io) v3.2+:
 
 ```bash
-spacy init vectors --mode floret vectors.floret spacy_vectors_dir
+spacy init vectors LANG vectors.floret spacy_vectors_dir --mode floret
 ```
 
 ## How floret works
 
 In its original implementation, fastText stores words and subwords in two
 separate tables. The word table contains one entry per word in the vocabulary
 (typically ~1M entries) and the subwords are stored a separate fixed-size table
 by hashing each subword into one row in the table (default 2M entries). A
 relatively large table is used to reduce the number of collisions between
 subwords. However, for 1M words + 2M subwords with 300-dimensional vectors of
 32-bit floats, you'd need around 3GB to store the resulting data, which is
 prohibitive for many use cases.
 
-In addition, many libraries that import vectors only support the word table 
+In addition, many libraries that import vectors only support the word table
 (`.vec`), which limits the coverage to words above a certain frequency in the
 training data. For languages with rich morphology, even a large vector table
 may not provide good coverage for words seen during training and you are still
 likely to encounter words that were not seen at all during training.
 
 In order to store word and subword vectors in a more compact format, we turn to
 an algorithm that's been used by [spaCy](https://spacy.io) all along: Bloom
@@ -157,15 +167,15 @@
 9 8.0678 -4.4142 3.6236 4.5889 -2.7611 2.4455 0.67096 -4.2822 2.0875 4.6274
 ```
 
 This table can be imported into a spaCy pipeline using `spacy init vectors` in
 spaCy v3.2+ with the option `--mode floret`:
 
 ```bash
-spacy init vectors --mode floret vectors.floret spacy_vectors_dir
+spacy init vectors LANG vectors.floret spacy_vectors_dir --mode floret
 ```
 
 ## Notes
 
 The fastText and floret binary formats (`.bin`) are not compatible, so it's
 important to load a `.bin` file with the same program used to train it.
```

#### html2text {}

```diff
@@ -1,117 +1,126 @@
 [https://explosion.ai/assets/img/logo.svg] # floret: fastText + Bloom
 embeddings for compact, full-coverage vectors with spaCy floret is an extended
 version of [fastText](https://fasttext.cc) that can produce word
 representations for any word from a compact vector table. It combines: -
 fastText's subwords to provide embeddings for any word - Bloom embeddings
-("hashing trick") for a compact vector table ## Install floret ### Build floret
-from source ```bash git clone https://github.com/explosion/floret cd floret
-make ``` This produces the main binary `floret`. ### Install for python Install
-the python wrapper with `pip`: ```bash pip install floret ``` Or install from
-source in developer mode: ```bash git clone https://github.com/explosion/floret
-cd floret pip install -r requirements.txt pip install --no-build-isolation --
-editable . ``` See the [python docs](python/README.md). ## Usage `floret` adds
-two additional command line options to `fasttext`: ``` -mode fasttext (default)
-or floret (word and char ngrams hashed in buckets) [fasttext] -hashCount floret
-mode only: number of hashes (1-4) per word/subword [1] ``` With `-mode floret`,
-the word entries are stored in the same table as the subword embeddings
-(buckets), reducing the size of the saved vector data. With `-hashCount 2`,
-each entry is stored as the sum of 2 rows in the internal subwords hash table.
-`floret` supports 1-4 hashes per entry in the embeddings table. By storing an
-entry in the embedding table as the sum of more than one row, it is possible to
-greatly reduce the number of rows in the table with a relatively small effect
-on the performance, both in terms of accuracy and speed. Here's how to train
-CBOW embeddings with subwords as 4-grams and 5-grams, 2 hashes per entry, and a
-compact table of 50K entries rather than the default of 2M entries. ```bash
-floret cbow -dim 300 -minn 4 -maxn 5 -mode floret -hashCount 2 -bucket 50000 \
--input input.txt -output vectors ``` With the `-mode floret` option, floret
-will save an additional vector table with the file ending `.floret`. The format
-is very similar to `.vec` with a header line followed by one line per vector.
-The word tokens are replaced with the index of the row and the header is
-extended to contain all the relevant training settings needed to load this
-table in spaCy. To import this vector table in [spaCy](https://spacy.io) v3.2+:
-```bash spacy init vectors --mode floret vectors.floret spacy_vectors_dir ```
-## How floret works In its original implementation, fastText stores words and
-subwords in two separate tables. The word table contains one entry per word in
-the vocabulary (typically ~1M entries) and the subwords are stored a separate
-fixed-size table by hashing each subword into one row in the table (default 2M
-entries). A relatively large table is used to reduce the number of collisions
-between subwords. However, for 1M words + 2M subwords with 300-dimensional
-vectors of 32-bit floats, you'd need around 3GB to store the resulting data,
-which is prohibitive for many use cases. In addition, many libraries that
-import vectors only support the word table (`.vec`), which limits the coverage
-to words above a certain frequency in the training data. For languages with
-rich morphology, even a large vector table may not provide good coverage for
-words seen during training and you are still likely to encounter words that
-were not seen at all during training. In order to store word and subword
-vectors in a more compact format, we turn to an algorithm that's been used by
-[spaCy](https://spacy.io) all along: Bloom embeddings. Bloom embeddings (also
-called the "hashing trick", or known as [`HashEmbed`](https://thinc.ai/docs/
-api-layers#hashembed) within spaCy's ML library [thinc](https://thinc.ai)) can
-be used to store distinct representations in a compact table by hashing each
-entry into multiple rows in the table. By representing each entry as the sum of
-multiple rows, where it's unlikely that two entries will collide on multiple
-hashes, most entries will end up with a distinct representation. With the
-settings `-minn 4 -maxn 5 -mode floret -hashCount 2`, the embedding for the
-word `apple` is stored internally as the sum of 2 hashed rows for each of the
-word, 4-grams and 5-grams. The word is padded with the BOW and EOW characters
-`<` and `>`, creating the following word and subword entries: ```    ``` For
-compatibility with spaCy, [MurmurHash](https://github.com/aappleby/smhasher) is
-used to hash the word and char ngram strings. The final embedding for `apple`
-is then the sum of two rows (`-hashCount 2`) per word and char ngram above.
-With `-mode floret`, `floret` will save an additional vector table with the
-ending `.floret` alongside the usual `.bin` and `.vec` files. The format is
-very similar to `.vec` with a header line followed by one line per entry in the
-vector table with the row index rather than a word token at the beginning of
-each line. The header is extended to contain all the training settings required
-to use this table in another application or library like spaCy. The header
-contains the space-separated settings: ```none bucket dim minn maxn hashCount
-hashSeed BOW EOW ``` A demo `.floret` table with `-bucket 10 -dim 10 -minn 2 -
-maxn3 -hashCount 2`: ```none 10 10 2 3 2 2166136261 < > 0 -2.2611 3.9302 2.6676
--11.233 0.093715 -10.52 -9.6463 -0.11853 2.101 -0.10145 1 -3.12 -1.7981 10.7 -
-6.171 4.4527 10.967 9.073 6.2056 -6.1199 -2.0402 2 9.5689 5.6721 -8.4832 -
-1.2249 2.1871 -3.0264 -2.391 -5.3308 -3.2847 -4.0382 3 3.6268 4.2759 -1.7007
-1.5002 5.5266 1.8716 -12.063 0.26314 2.7645 2.4929 4 -11.683 -7.7068 2.1102
-2.214 7.2202 0.69799 3.2173 -5.382 -2.0838 5.0314 5 -4.3024 8.0241 2.0714 -
-1.0174 -0.28369 1.7622 7.8797 -1.7795 6.7541 5.6703 6 8.3574 -5.225 8.6529
-8.5605 -8.9465 3.767 -5.4636 -1.4635 -0.98947 -0.58025 7 -10.01 3.3894 -4.4487
-1.1669 -11.904 6.5158 4.3681 0.79913 -6.9131 -8.687 8 -5.4576 7.1019 -8.8259
-1.7189 4.955 -8.9157 -3.8905 -0.60086 -2.1233 5.892 9 8.0678 -4.4142 3.6236
-4.5889 -2.7611 2.4455 0.67096 -4.2822 2.0875 4.6274 ``` This table can be
-imported into a spaCy pipeline using `spacy init vectors` in spaCy v3.2+ with
-the option `--mode floret`: ```bash spacy init vectors --mode floret
-vectors.floret spacy_vectors_dir ``` ## Notes The fastText and floret binary
-formats (`.bin`) are not compatible, so it's important to load a `.bin` file
-with the same program used to train it. See the [fastText documentation](https:
-//fasttext.cc) for details about all other commands and options. `floret`
-supports all existing `fasttext` commands and does not modify any `fasttext`
-defaults. The original fastText README is provided below for reference. --- #
-fastText README [fastText](https://fasttext.cc/) is a library for efficient
-learning of word representations and sentence classification. ## Table of
-contents - [Resources](#resources) - [Models](#models) - [Supplementary data]
-(#supplementary-data) - [FAQ](#faq) - [Cheatsheet](#cheatsheet) -
-[Requirements](#requirements) - [Building fastText](#building-fasttext) -
-[Getting the source code](#getting-the-source-code) - [Building fastText using
-make (preferred)](#building-fasttext-using-make-preferred) - [Building fastText
-using cmake](#building-fasttext-using-cmake) - [Building fastText for Python]
-(#building-fasttext-for-python) - [Example use cases](#example-use-cases) -
-[Word representation learning](#word-representation-learning) - [Obtaining word
-vectors for out-of-vocabulary words](#obtaining-word-vectors-for-out-of-
-vocabulary-words) - [Text classification](#text-classification) - [Full
-documentation](#full-documentation) - [References](#references) - [Enriching
-Word Vectors with Subword Information](#enriching-word-vectors-with-subword-
-information) - [Bag of Tricks for Efficient Text Classification](#bag-of-
-tricks-for-efficient-text-classification) - [FastText.zip: Compressing text
-classification models](#fasttextzip-compressing-text-classification-models) ##
-Resources ### Models - Recent state-of-the-art [English word vectors](https://
-fasttext.cc/docs/en/english-vectors.html). - Word vectors for [157 languages
-trained on Wikipedia and Crawl](https://fasttext.cc/docs/en/crawl-
-vectors.html). - Models for [language identification](https://fasttext.cc/docs/
-en/language-identification.html#content) and [various supervised tasks](https:/
-/fasttext.cc/docs/en/supervised-models.html#content). ### Supplementary data -
+("hashing trick") for a compact vector table To learn more about floret, check
+out our [blog post on floret vectors](https://explosion.ai/blog/floret-
+vectors). For a hands-on introduction, experiment with English vectors in this
+example notebook: [`intro_to_floret`][intro_to_floret] [![Open in Colab]
+[colab]][intro_to_floret_colab] [colab]: https://gistcdn.githack.com/ines/
+dcf354aa71a7665ae19871d7fd14a4e0/raw/461fc1f61a7bc5860f943cd4b6bcfabb8c8906e7/
+colab-badge.svg [intro_to_floret]: examples/01_intro_to_floret.ipynb
+[intro_to_floret_colab]: https://colab.research.google.com/github/explosion/
+floret/blob/main/examples/01_intro_to_floret.ipynb ## Install floret ### Build
+floret from source ```bash git clone https://github.com/explosion/floret cd
+floret make ``` This produces the main binary `floret`. ### Install for python
+Install the python wrapper with `pip`: ```bash pip install floret ``` Or
+install from source in developer mode: ```bash git clone https://github.com/
+explosion/floret cd floret pip install -r requirements.txt pip install --no-
+build-isolation --editable . ``` See the [python docs](python/README.md). ##
+Usage `floret` adds two additional command line options to `fasttext`: ``` -
+mode fasttext (default) or floret (word and char ngrams hashed in buckets)
+[fasttext] -hashCount floret mode only: number of hashes (1-4) per word/subword
+[1] ``` With `-mode floret`, the word entries are stored in the same table as
+the subword embeddings (buckets), reducing the size of the saved vector data.
+With `-hashCount 2`, each entry is stored as the sum of 2 rows in the internal
+subwords hash table. `floret` supports 1-4 hashes per entry in the embeddings
+table. By storing an entry in the embedding table as the sum of more than one
+row, it is possible to greatly reduce the number of rows in the table with a
+relatively small effect on the performance, both in terms of accuracy and
+speed. Here's how to train CBOW embeddings with subwords as 4-grams and 5-
+grams, 2 hashes per entry, and a compact table of 50K entries rather than the
+default of 2M entries. ```bash floret cbow -dim 300 -minn 4 -maxn 5 -mode
+floret -hashCount 2 -bucket 50000 \ -input input.txt -output vectors ``` With
+the `-mode floret` option, floret will save an additional vector table with the
+file ending `.floret`. The format is very similar to `.vec` with a header line
+followed by one line per vector. The word tokens are replaced with the index of
+the row and the header is extended to contain all the relevant training
+settings needed to load this table in spaCy. To import this vector table in
+[spaCy](https://spacy.io) v3.2+: ```bash spacy init vectors LANG vectors.floret
+spacy_vectors_dir --mode floret ``` ## How floret works In its original
+implementation, fastText stores words and subwords in two separate tables. The
+word table contains one entry per word in the vocabulary (typically ~1M
+entries) and the subwords are stored a separate fixed-size table by hashing
+each subword into one row in the table (default 2M entries). A relatively large
+table is used to reduce the number of collisions between subwords. However, for
+1M words + 2M subwords with 300-dimensional vectors of 32-bit floats, you'd
+need around 3GB to store the resulting data, which is prohibitive for many use
+cases. In addition, many libraries that import vectors only support the word
+table (`.vec`), which limits the coverage to words above a certain frequency in
+the training data. For languages with rich morphology, even a large vector
+table may not provide good coverage for words seen during training and you are
+still likely to encounter words that were not seen at all during training. In
+order to store word and subword vectors in a more compact format, we turn to an
+algorithm that's been used by [spaCy](https://spacy.io) all along: Bloom
+embeddings. Bloom embeddings (also called the "hashing trick", or known as
+[`HashEmbed`](https://thinc.ai/docs/api-layers#hashembed) within spaCy's ML
+library [thinc](https://thinc.ai)) can be used to store distinct
+representations in a compact table by hashing each entry into multiple rows in
+the table. By representing each entry as the sum of multiple rows, where it's
+unlikely that two entries will collide on multiple hashes, most entries will
+end up with a distinct representation. With the settings `-minn 4 -maxn 5 -mode
+floret -hashCount 2`, the embedding for the word `apple` is stored internally
+as the sum of 2 hashed rows for each of the word, 4-grams and 5-grams. The word
+is padded with the BOW and EOW characters `<` and `>`, creating the following
+word and subword entries: ```    ``` For compatibility with spaCy, [MurmurHash]
+(https://github.com/aappleby/smhasher) is used to hash the word and char ngram
+strings. The final embedding for `apple` is then the sum of two rows (`-
+hashCount 2`) per word and char ngram above. With `-mode floret`, `floret` will
+save an additional vector table with the ending `.floret` alongside the usual
+`.bin` and `.vec` files. The format is very similar to `.vec` with a header
+line followed by one line per entry in the vector table with the row index
+rather than a word token at the beginning of each line. The header is extended
+to contain all the training settings required to use this table in another
+application or library like spaCy. The header contains the space-separated
+settings: ```none bucket dim minn maxn hashCount hashSeed BOW EOW ``` A demo
+`.floret` table with `-bucket 10 -dim 10 -minn 2 -maxn3 -hashCount 2`: ```none
+10 10 2 3 2 2166136261 < > 0 -2.2611 3.9302 2.6676 -11.233 0.093715 -10.52 -
+9.6463 -0.11853 2.101 -0.10145 1 -3.12 -1.7981 10.7 -6.171 4.4527 10.967 9.073
+6.2056 -6.1199 -2.0402 2 9.5689 5.6721 -8.4832 -1.2249 2.1871 -3.0264 -2.391 -
+5.3308 -3.2847 -4.0382 3 3.6268 4.2759 -1.7007 1.5002 5.5266 1.8716 -12.063
+0.26314 2.7645 2.4929 4 -11.683 -7.7068 2.1102 2.214 7.2202 0.69799 3.2173 -
+5.382 -2.0838 5.0314 5 -4.3024 8.0241 2.0714 -1.0174 -0.28369 1.7622 7.8797 -
+1.7795 6.7541 5.6703 6 8.3574 -5.225 8.6529 8.5605 -8.9465 3.767 -5.4636 -
+1.4635 -0.98947 -0.58025 7 -10.01 3.3894 -4.4487 1.1669 -11.904 6.5158 4.3681
+0.79913 -6.9131 -8.687 8 -5.4576 7.1019 -8.8259 1.7189 4.955 -8.9157 -3.8905 -
+0.60086 -2.1233 5.892 9 8.0678 -4.4142 3.6236 4.5889 -2.7611 2.4455 0.67096 -
+4.2822 2.0875 4.6274 ``` This table can be imported into a spaCy pipeline using
+`spacy init vectors` in spaCy v3.2+ with the option `--mode floret`: ```bash
+spacy init vectors LANG vectors.floret spacy_vectors_dir --mode floret ``` ##
+Notes The fastText and floret binary formats (`.bin`) are not compatible, so
+it's important to load a `.bin` file with the same program used to train it.
+See the [fastText documentation](https://fasttext.cc) for details about all
+other commands and options. `floret` supports all existing `fasttext` commands
+and does not modify any `fasttext` defaults. The original fastText README is
+provided below for reference. --- # fastText README [fastText](https://
+fasttext.cc/) is a library for efficient learning of word representations and
+sentence classification. ## Table of contents - [Resources](#resources) -
+[Models](#models) - [Supplementary data](#supplementary-data) - [FAQ](#faq) -
+[Cheatsheet](#cheatsheet) - [Requirements](#requirements) - [Building fastText]
+(#building-fasttext) - [Getting the source code](#getting-the-source-code) -
+[Building fastText using make (preferred)](#building-fasttext-using-make-
+preferred) - [Building fastText using cmake](#building-fasttext-using-cmake) -
+[Building fastText for Python](#building-fasttext-for-python) - [Example use
+cases](#example-use-cases) - [Word representation learning](#word-
+representation-learning) - [Obtaining word vectors for out-of-vocabulary words]
+(#obtaining-word-vectors-for-out-of-vocabulary-words) - [Text classification]
+(#text-classification) - [Full documentation](#full-documentation) -
+[References](#references) - [Enriching Word Vectors with Subword Information]
+(#enriching-word-vectors-with-subword-information) - [Bag of Tricks for
+Efficient Text Classification](#bag-of-tricks-for-efficient-text-
+classification) - [FastText.zip: Compressing text classification models]
+(#fasttextzip-compressing-text-classification-models) ## Resources ### Models -
+Recent state-of-the-art [English word vectors](https://fasttext.cc/docs/en/
+english-vectors.html). - Word vectors for [157 languages trained on Wikipedia
+and Crawl](https://fasttext.cc/docs/en/crawl-vectors.html). - Models for
+[language identification](https://fasttext.cc/docs/en/language-
+identification.html#content) and [various supervised tasks](https://
+fasttext.cc/docs/en/supervised-models.html#content). ### Supplementary data -
 The preprocessed [YFCC100M data](https://fasttext.cc/docs/en/
 dataset.html#content) used in [2]. ### FAQ You can find [answers to frequently
 asked questions](https://fasttext.cc/docs/en/faqs.html#content) on our
 [website](https://fasttext.cc/). ### Cheatsheet We also provide a [cheatsheet]
 (https://fasttext.cc/docs/en/cheatsheet.html#content) full of useful one-
 liners. ## Requirements We are continuously building and testing our library,
 CLI and Python bindings under various docker images using [circleci](https://
```

### Comparing `floret-0.10.2/python/README.md` & `floret-0.10.3/python/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -60,18 +60,18 @@
 fastText vectors.
 
 ## Use floret vectors in spaCy
 
 Import floret vectors into spaCy v3.2+:
 
 ```bash
-spacy init vectors --mode floret vectors.floret spacy_vectors_model
+spacy init vectors LANG vectors.floret spacy_vectors_model --mode floret
 ```
 
 ## Notes
 
 `floret` contains all features of the original [`fasttext`
-module](https://pypi.org/project/fasttest). See the [`fasttext`
+module](https://pypi.org/project/fasttext). See the [`fasttext`
 docs](https://fasttext.cc/docs/en/python-module.html) for more information.
 
 The `fasttext` and `floret` binary formats saved with
 `model.save_model("model.bin")` are not compatible.
```

#### html2text {}

```diff
@@ -14,13 +14,13 @@
 vectors model = floret.train_unsupervised( "data.txt", model="cbow",
 mode="floret", hashCount=2, bucket=50000, minn=3, maxn=6, ) # query vector
 model.get_word_vector("broccoli") # save full model model.save_model
 ("vectors.bin") # export standard word-only vector table model.save_vectors
 ("vectors.vec") # export floret vector table model.save_floret_vectors
 ("vectors.floret") ``` **Note:** with the default setting `mode="fasttext"`,
 `floret` trains original fastText vectors. ## Use floret vectors in spaCy
-Import floret vectors into spaCy v3.2+: ```bash spacy init vectors --mode
-floret vectors.floret spacy_vectors_model ``` ## Notes `floret` contains all
-features of the original [`fasttext` module](https://pypi.org/project/
-fasttest). See the [`fasttext` docs](https://fasttext.cc/docs/en/python-
+Import floret vectors into spaCy v3.2+: ```bash spacy init vectors LANG
+vectors.floret spacy_vectors_model --mode floret ``` ## Notes `floret` contains
+all features of the original [`fasttext` module](https://pypi.org/project/
+fasttext). See the [`fasttext` docs](https://fasttext.cc/docs/en/python-
 module.html) for more information. The `fasttext` and `floret` binary formats
 saved with `model.save_model("model.bin")` are not compatible.
```

### Comparing `floret-0.10.2/python/floret_module/floret/__init__.py` & `floret-0.10.3/python/floret_module/floret/__init__.py`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/python/floret_module/floret/floret.py` & `floret-0.10.3/python/floret_module/floret/floret.py`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/python/floret_module/floret/pybind/floret_pybind.cc` & `floret-0.10.3/python/floret_module/floret/pybind/floret_pybind.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/python/floret_module/floret/tests/data.txt` & `floret-0.10.3/python/floret_module/floret/tests/data.txt`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/python/floret_module/floret/tests/test_configurations.py` & `floret-0.10.3/python/floret_module/floret/tests/test_configurations.py`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/python/floret_module/floret/tests/test_script.py` & `floret-0.10.3/python/floret_module/floret/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/python/floret_module/floret/tests/test_train.py` & `floret-0.10.3/python/floret_module/floret/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/python/floret_module/floret/util/util.py` & `floret-0.10.3/python/floret_module/floret/util/util.py`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/python/floret_module/floret.egg-info/PKG-INFO` & `floret-0.10.3/python/floret_module/floret.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: floret
-Version: 0.10.2
+Version: 0.10.3
 Summary: floret Python bindings
 Home-page: https://github.com/explosion/floret
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -86,20 +85,18 @@
 fastText vectors.
 
 ## Use floret vectors in spaCy
 
 Import floret vectors into spaCy v3.2+:
 
 ```bash
-spacy init vectors --mode floret vectors.floret spacy_vectors_model
+spacy init vectors LANG vectors.floret spacy_vectors_model --mode floret
 ```
 
 ## Notes
 
 `floret` contains all features of the original [`fasttext`
-module](https://pypi.org/project/fasttest). See the [`fasttext`
+module](https://pypi.org/project/fasttext). See the [`fasttext`
 docs](https://fasttext.cc/docs/en/python-module.html) for more information.
 
 The `fasttext` and `floret` binary formats saved with
 `model.save_model("model.bin")` are not compatible.
-
-
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: floret Version: 0.10.2 Summary: floret Python
+Metadata-Version: 2.1 Name: floret Version: 0.10.3 Summary: floret Python
 bindings Home-page: https://github.com/explosion/floret Author: Explosion
-Author-email: contact@explosion.ai License: MIT Platform: UNKNOWN Classifier:
-Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development Classifier: Topic :: Scientific/
-Engineering Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: POSIX Classifier: Operating System :: Unix Classifier:
-Operating System :: MacOS Description-Content-Type: text/markdown License-File:
-LICENSE [https://explosion.ai/assets/img/logo.svg] # floret: fastText + Bloom
-embeddings for compact, full-coverage vectors with spaCy floret is an extended
-version of [fastText](https://fasttext.cc) that can produce word
-representations for any word from a compact vector table. It combines: -
-fastText's subwords to provide embeddings for any word - Bloom embeddings
-("hashing trick") for a compact vector table ## Installation ```bash pip
-install floret ``` ## Usage Train floret vectors using the options: - `mode`:
-`"floret"`, storing both words and subwords in the same compact hash table -
-`hashCount`: store each entry in 1-4 rows in the hash table (recommended: `2`)
-- `bucket`: in combination with `hashCount>1`, the size of the hash table can
-be greatly reduced (recommended: `25000`--`100000`, reduced from the fastText
-default of `2000000`) - `minn`: min length of char ngram (default: `3`) -
-`maxn`: max length of char ngram (default: `6`) ```python import floret # train
-vectors model = floret.train_unsupervised( "data.txt", model="cbow",
-mode="floret", hashCount=2, bucket=50000, minn=3, maxn=6, ) # query vector
+Author-email: contact@explosion.ai License: MIT Classifier: Development Status
+:: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
+Development Classifier: Topic :: Scientific/Engineering Classifier: Operating
+System :: Microsoft :: Windows Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix Classifier: Operating System :: MacOS
+Description-Content-Type: text/markdown License-File: LICENSE [https://
+explosion.ai/assets/img/logo.svg] # floret: fastText + Bloom embeddings for
+compact, full-coverage vectors with spaCy floret is an extended version of
+[fastText](https://fasttext.cc) that can produce word representations for any
+word from a compact vector table. It combines: - fastText's subwords to provide
+embeddings for any word - Bloom embeddings ("hashing trick") for a compact
+vector table ## Installation ```bash pip install floret ``` ## Usage Train
+floret vectors using the options: - `mode`: `"floret"`, storing both words and
+subwords in the same compact hash table - `hashCount`: store each entry in 1-
+4 rows in the hash table (recommended: `2`) - `bucket`: in combination with
+`hashCount>1`, the size of the hash table can be greatly reduced (recommended:
+`25000`--`100000`, reduced from the fastText default of `2000000`) - `minn`:
+min length of char ngram (default: `3`) - `maxn`: max length of char ngram
+(default: `6`) ```python import floret # train vectors model =
+floret.train_unsupervised( "data.txt", model="cbow", mode="floret",
+hashCount=2, bucket=50000, minn=3, maxn=6, ) # query vector
 model.get_word_vector("broccoli") # save full model model.save_model
 ("vectors.bin") # export standard word-only vector table model.save_vectors
 ("vectors.vec") # export floret vector table model.save_floret_vectors
 ("vectors.floret") ``` **Note:** with the default setting `mode="fasttext"`,
 `floret` trains original fastText vectors. ## Use floret vectors in spaCy
-Import floret vectors into spaCy v3.2+: ```bash spacy init vectors --mode
-floret vectors.floret spacy_vectors_model ``` ## Notes `floret` contains all
-features of the original [`fasttext` module](https://pypi.org/project/
-fasttest). See the [`fasttext` docs](https://fasttext.cc/docs/en/python-
+Import floret vectors into spaCy v3.2+: ```bash spacy init vectors LANG
+vectors.floret spacy_vectors_model --mode floret ``` ## Notes `floret` contains
+all features of the original [`fasttext` module](https://pypi.org/project/
+fasttext). See the [`fasttext` docs](https://fasttext.cc/docs/en/python-
 module.html) for more information. The `fasttext` and `floret` binary formats
 saved with `model.save_model("model.bin")` are not compatible.
```

### Comparing `floret-0.10.2/python/floret_module/floret.egg-info/SOURCES.txt` & `floret-0.10.3/python/floret_module/floret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/setup.py` & `floret-0.10.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import setuptools
 import os
 import subprocess
 import platform
 import io
 import pybind11
 
-__version__ = '0.10.2'
+__version__ = '0.10.3'
 FASTTEXT_SRC = "src"
 
 # Based on https://github.com/pybind/python_example
 
 class get_pybind_include(object):
     """Helper class to determine the pybind11 include path"""
```

### Comparing `floret-0.10.2/src/MurmurHash3.cpp` & `floret-0.10.3/src/MurmurHash3.cpp`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/MurmurHash3.h` & `floret-0.10.3/src/MurmurHash3.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/args.cc` & `floret-0.10.3/src/args.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/args.h` & `floret-0.10.3/src/args.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/autotune.cc` & `floret-0.10.3/src/autotune.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/autotune.h` & `floret-0.10.3/src/autotune.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/densematrix.cc` & `floret-0.10.3/src/densematrix.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/densematrix.h` & `floret-0.10.3/src/densematrix.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/dictionary.cc` & `floret-0.10.3/src/dictionary.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/dictionary.h` & `floret-0.10.3/src/dictionary.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/fasttext.cc` & `floret-0.10.3/src/fasttext.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/fasttext.h` & `floret-0.10.3/src/fasttext.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/loss.cc` & `floret-0.10.3/src/loss.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/loss.h` & `floret-0.10.3/src/loss.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/main.cc` & `floret-0.10.3/src/main.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/matrix.h` & `floret-0.10.3/src/matrix.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/meter.cc` & `floret-0.10.3/src/meter.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/meter.h` & `floret-0.10.3/src/meter.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/model.cc` & `floret-0.10.3/src/model.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/model.h` & `floret-0.10.3/src/model.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/productquantizer.cc` & `floret-0.10.3/src/productquantizer.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/productquantizer.h` & `floret-0.10.3/src/productquantizer.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/quantmatrix.cc` & `floret-0.10.3/src/quantmatrix.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/quantmatrix.h` & `floret-0.10.3/src/quantmatrix.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/utils.cc` & `floret-0.10.3/src/utils.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/utils.h` & `floret-0.10.3/src/utils.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/vector.cc` & `floret-0.10.3/src/vector.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.2/src/vector.h` & `floret-0.10.3/src/vector.h`

 * *Files identical despite different names*

