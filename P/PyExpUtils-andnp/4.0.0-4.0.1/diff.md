# Comparing `tmp/PyExpUtils-andnp-4.0.0.tar.gz` & `tmp/PyExpUtils-andnp-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyExpUtils-andnp-4.0.0.tar", last modified: Mon May  8 20:25:25 2023, max compression
+gzip compressed data, was "PyExpUtils-andnp-4.0.1.tar", last modified: Mon May  8 23:10:20 2023, max compression
```

## Comparing `PyExpUtils-andnp-4.0.0.tar` & `PyExpUtils-andnp-4.0.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1011 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/FileSystemContext.py
--rw-r--r--   0        0        0      119 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/__init__.py
--rw-r--r--   0        0        0     1207 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/models/Config.py
--rw-r--r--   0        0        0     7915 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/models/ExperimentDescription.py
--rw-r--r--   0        0        0       87 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/py.typed
--rw-r--r--   0        0        0     3110 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/results/Collection.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/results/__init__.py
--rw-r--r--   0        0        0      510 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/results/indices.py
--rw-r--r--   0        0        0     7798 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/results/pandas.py
--rw-r--r--   0        0        0     1070 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/results/tools.py
--rw-r--r--   0        0        0     8921 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/results/voting.py
--rw-r--r--   0        0        0     5211 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/runner/Slurm.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/runner/__init__.py
--rw-r--r--   0        0        0      742 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/runner/parallel.py
--rw-r--r--   0        0        0     1450 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/runner/utils.py
--rw-r--r--   0        0        0     2826 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/Collector.py
--rw-r--r--   0        0        0     3030 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/NestedDict.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/__init__.py
--rw-r--r--   0        0        0     3432 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/arrays.py
--rw-r--r--   0        0        0      403 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/asyncio.py
--rw-r--r--   0        0        0      595 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/cache.py
--rw-r--r--   0        0        0      368 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/cmdline.py
--rw-r--r--   0        0        0     1233 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/csv.py
--rw-r--r--   0        0        0     3547 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/dict.py
--rw-r--r--   0        0        0     1266 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/fp.py
--rw-r--r--   0        0        0      921 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/generator.py
--rw-r--r--   0        0        0      476 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/jit.py
--rw-r--r--   0        0        0     1218 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/path.py
--rw-r--r--   0        0        0     3454 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/permute.py
--rw-r--r--   0        0        0     1046 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/random.py
--rw-r--r--   0        0        0      278 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/str.py
--rw-r--r--   0        0        0      439 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/PyExpUtils/utils/types.py
--rw-r--r--   0        0        0     6884 2023-05-08 20:24:49.746093 PyExpUtils-andnp-4.0.0/README.md
--rw-r--r--   0        0        0     1036 2023-05-08 20:25:24.334010 PyExpUtils-andnp-4.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/__init__.py
--rw-r--r--   0        0        0      214 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/_utils/pandas.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/models/__init__.py
--rw-r--r--   0        0        0     5461 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/models/test_ExperimentDescription.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/results/__init__.py
--rw-r--r--   0        0        0      898 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/results/test_indices.py
--rw-r--r--   0        0        0     9113 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/results/test_pandas.py
--rw-r--r--   0        0        0     2010 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/results/test_tools.py
--rw-r--r--   0        0        0     8723 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/results/test_voting.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/runner/__init__.py
--rw-r--r--   0        0        0      385 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/runner/test_parallel.py
--rw-r--r--   0        0        0      987 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/runner/test_slurm.py
--rw-r--r--   0        0        0     2278 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/test_FileSystemContext.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     3210 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_Collector.py
--rw-r--r--   0        0        0     4023 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_arrays.py
--rw-r--r--   0        0        0      881 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_cmdline.py
--rw-r--r--   0        0        0     1911 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_csv.py
--rw-r--r--   0        0        0     5882 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_dict.py
--rw-r--r--   0        0        0      586 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_generator.py
--rw-r--r--   0        0        0     1685 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_path.py
--rw-r--r--   0        0        0     3725 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_permute.py
--rw-r--r--   0        0        0     1591 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_random.py
--rw-r--r--   0        0        0      365 2023-05-08 20:24:49.750093 PyExpUtils-andnp-4.0.0/tests/utils/test_str.py
--rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 PyExpUtils-andnp-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1011 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/FileSystemContext.py
+-rw-r--r--   0        0        0      119 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/__init__.py
+-rw-r--r--   0        0        0     1207 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/models/Config.py
+-rw-r--r--   0        0        0     7915 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/models/ExperimentDescription.py
+-rw-r--r--   0        0        0       87 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/py.typed
+-rw-r--r--   0        0        0     3110 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/results/Collection.py
+-rw-r--r--   0        0        0        0 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/results/__init__.py
+-rw-r--r--   0        0        0      510 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/results/indices.py
+-rw-r--r--   0        0        0     7798 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/results/pandas.py
+-rw-r--r--   0        0        0     1070 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/results/tools.py
+-rw-r--r--   0        0        0     8921 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/results/voting.py
+-rw-r--r--   0        0        0     5211 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/runner/Slurm.py
+-rw-r--r--   0        0        0        0 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/runner/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/runner/parallel.py
+-rw-r--r--   0        0        0     1450 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/runner/utils.py
+-rw-r--r--   0        0        0     2826 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/Collector.py
+-rw-r--r--   0        0        0     3030 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/NestedDict.py
+-rw-r--r--   0        0        0        0 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/__init__.py
+-rw-r--r--   0        0        0     3432 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/arrays.py
+-rw-r--r--   0        0        0      403 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/asyncio.py
+-rw-r--r--   0        0        0      595 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/cache.py
+-rw-r--r--   0        0        0      368 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/cmdline.py
+-rw-r--r--   0        0        0     1233 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/csv.py
+-rw-r--r--   0        0        0     3547 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/dict.py
+-rw-r--r--   0        0        0     1266 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/fp.py
+-rw-r--r--   0        0        0      921 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/generator.py
+-rw-r--r--   0        0        0      476 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/jit.py
+-rw-r--r--   0        0        0     1218 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/path.py
+-rw-r--r--   0        0        0     3454 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/permute.py
+-rw-r--r--   0        0        0      969 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/random.py
+-rw-r--r--   0        0        0      278 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/str.py
+-rw-r--r--   0        0        0      439 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/types.py
+-rw-r--r--   0        0        0     6884 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/README.md
+-rw-r--r--   0        0        0     1018 2023-05-08 23:10:19.091060 PyExpUtils-andnp-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      214 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/_utils/pandas.py
+-rw-r--r--   0        0        0        0 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/models/__init__.py
+-rw-r--r--   0        0        0     5461 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/models/test_ExperimentDescription.py
+-rw-r--r--   0        0        0        0 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/results/__init__.py
+-rw-r--r--   0        0        0      898 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/results/test_indices.py
+-rw-r--r--   0        0        0     9113 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/results/test_pandas.py
+-rw-r--r--   0        0        0     2010 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/results/test_tools.py
+-rw-r--r--   0        0        0     8723 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/results/test_voting.py
+-rw-r--r--   0        0        0        0 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/runner/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/runner/test_parallel.py
+-rw-r--r--   0        0        0      987 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/runner/test_slurm.py
+-rw-r--r--   0        0        0     2278 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/test_FileSystemContext.py
+-rw-r--r--   0        0        0        0 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3210 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_Collector.py
+-rw-r--r--   0        0        0     4023 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_arrays.py
+-rw-r--r--   0        0        0      881 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_cmdline.py
+-rw-r--r--   0        0        0     1911 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_csv.py
+-rw-r--r--   0        0        0     5882 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_dict.py
+-rw-r--r--   0        0        0      586 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_generator.py
+-rw-r--r--   0        0        0     1685 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_path.py
+-rw-r--r--   0        0        0     3725 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_permute.py
+-rw-r--r--   0        0        0     1560 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_random.py
+-rw-r--r--   0        0        0      365 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_str.py
+-rw-r--r--   0        0        0     7138 1970-01-01 00:00:00.000000 PyExpUtils-andnp-4.0.1/PKG-INFO
```

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/FileSystemContext.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/FileSystemContext.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/models/Config.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/models/Config.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/models/ExperimentDescription.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/models/ExperimentDescription.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/results/Collection.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/results/Collection.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/results/pandas.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/results/pandas.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/results/tools.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/results/tools.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/results/voting.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/results/voting.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/runner/Slurm.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/runner/Slurm.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/runner/parallel.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/runner/parallel.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/runner/utils.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/runner/utils.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/Collector.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/Collector.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/NestedDict.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/NestedDict.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/arrays.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/cache.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/cache.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/csv.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/csv.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/dict.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/dict.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/fp.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/fp.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/generator.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/generator.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/path.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/path.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/permute.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/permute.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/PyExpUtils/utils/random.py` & `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/random.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import numpy as np
-from typing import Any, Sequence
+from typing import Sequence, TypeVar
 from PyExpUtils.utils.arrays import argsmax
-from PyExpUtils.utils.types import NpList, T
 from PyExpUtils.utils.jit import try2jit
 
+T = TypeVar('T')
+
 # way faster than np.random.choice
 # arr is an array of probabilities, should sum to 1
-def sample(arr: NpList, rng: Any = np.random):
-    r = rng.random()
-    return _sample(np.asarray(arr), r)
-
 @try2jit
-def _sample(arr: np.ndarray, r: float):
+def sample(arr: np.ndarray, rng: np.random.Generator):
+    r = rng.random()
     s = 0
     for i, p in enumerate(arr):
         s += p
         if s > r or s == 1:
             return i
 
     # worst case if we run into floating point error, just return the last element
     # we should never get here
     return len(arr) - 1
 
 # also much faster than np.random.choice
 # choose an element from a list with uniform random probability
-def choice(arr: Sequence[T], rng: Any = np.random) -> T:
+@try2jit
+def choice(arr: Sequence[T], rng: np.random.Generator) -> T:
     idxs = rng.permutation(len(arr))
     return arr[idxs[0]]
 
 # argmax that breaks ties randomly
-def argmax(vals: NpList, rng: Any = np.random):
-    ties = argsmax(np.asarray(vals))
+@try2jit
+def argmax(vals: np.ndarray, rng: np.random.Generator):
+    ties = argsmax(vals)
     return choice(ties, rng)
```

### Comparing `PyExpUtils-andnp-4.0.0/README.md` & `PyExpUtils-andnp-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/pyproject.toml` & `PyExpUtils-andnp-4.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "4.0.0"
+version = "4.0.1"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
 ]
 
 [tool.pdm]
 source = [
@@ -26,27 +26,26 @@
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "PyExpUtils-andnp"
-version = "4.0.0"
+version = "4.0.1"
 description = "A small set of utilities for RL and ML experiments"
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
-    "numba>=0.52.0",
+    "numba>=0.57.0",
     "numpy>=1.21.5",
-    "h5py>=3.1.0",
     "filelock>=3.0.0",
     "pandas",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
```

### Comparing `PyExpUtils-andnp-4.0.0/tests/models/test_ExperimentDescription.py` & `PyExpUtils-andnp-4.0.1/tests/models/test_ExperimentDescription.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/results/test_indices.py` & `PyExpUtils-andnp-4.0.1/tests/results/test_indices.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/results/test_pandas.py` & `PyExpUtils-andnp-4.0.1/tests/results/test_pandas.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/results/test_tools.py` & `PyExpUtils-andnp-4.0.1/tests/results/test_tools.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/results/test_voting.py` & `PyExpUtils-andnp-4.0.1/tests/results/test_voting.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/runner/test_slurm.py` & `PyExpUtils-andnp-4.0.1/tests/runner/test_slurm.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/test_FileSystemContext.py` & `PyExpUtils-andnp-4.0.1/tests/test_FileSystemContext.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/utils/test_Collector.py` & `PyExpUtils-andnp-4.0.1/tests/utils/test_Collector.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/utils/test_arrays.py` & `PyExpUtils-andnp-4.0.1/tests/utils/test_arrays.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/utils/test_cmdline.py` & `PyExpUtils-andnp-4.0.1/tests/utils/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/utils/test_csv.py` & `PyExpUtils-andnp-4.0.1/tests/utils/test_csv.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/utils/test_dict.py` & `PyExpUtils-andnp-4.0.1/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/utils/test_generator.py` & `PyExpUtils-andnp-4.0.1/tests/utils/test_generator.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/utils/test_path.py` & `PyExpUtils-andnp-4.0.1/tests/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/utils/test_permute.py` & `PyExpUtils-andnp-4.0.1/tests/utils/test_permute.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.0/tests/utils/test_random.py` & `PyExpUtils-andnp-4.0.1/tests/utils/test_random.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,59 @@
+import numba.typed
 import unittest
 import numpy as np
 from PyExpUtils.utils.random import argmax, choice, sample
+
 class TestRandom(unittest.TestCase):
     def test_sample(self):
-        np.random.seed(0)
+        rng = np.random.default_rng(0)
         # base functionality
-        arr = [.50, .20, .10, .10, .10]
+        arr = np.array([.50, .20, .10, .10, .10])
 
-        got = sample(arr)
+        got = sample(arr, rng)
         expected = 1 # an index from 0-4
 
         self.assertEqual(got, expected)
 
-        arr = [.01, .01, .08, .9]
+        arr = np.array([.01, .01, .08, .9])
 
-        got = sample(arr)
+        got = sample(arr, rng)
         expected = 3 # an index from 0-3
 
         self.assertEqual(got, expected)
 
     def test_choice(self):
-        np.random.seed(0)
+        rng = np.random.default_rng(0)
 
-        arr = ['a', 'b', 'c']
+        arr = numba.typed.List(['a', 'b', 'c'])
 
-        got = choice(arr)
+        got = choice(arr, rng)
         expected = 'c' # one of the three elements
 
         self.assertEqual(got, expected)
 
         counts = {'a': 0, 'b': 0, 'c': 0}
         for _ in range(10000):
-            element = choice(arr)
+            element = choice(arr, rng)
             counts[element] += 1
 
         # super fragile
         # TODO: make this a statistical test for uniformity
-        self.assertDictEqual(counts, { 'a': 3313, 'b': 3304, 'c': 3383 })
+        self.assertDictEqual(counts, { 'a': 3309, 'b': 3389, 'c': 3302 })
 
     def test_argmax(self):
-        np.random.seed(0)
+        rng = np.random.default_rng(0)
 
-        arr = [3, 2, 3]
+        arr = np.array([3, 2, 3])
 
-        got = argmax(arr)
-        expected = 2 # either 0 or 2
+        got = argmax(arr, rng)
+        expected = 0 # either 0 or 2
 
         self.assertEqual(got, expected)
 
         counts = [0, 0, 0]
         for _ in range(10000):
-            got = argmax(arr)
+            got = argmax(arr, rng)
             counts[got] += 1
 
         # TODO: make this a statistical test for uniformity
-        self.assertEqual(counts, [5086, 0, 4914])
-
-        # return nan values
-        arr = [np.nan, np.nan, 3]
-
-        got = argmax(arr)
-        expected = 0 # either 0 or 1
-
-        self.assertEqual(got, expected)
+        self.assertEqual(counts, [4971, 0, 5029])
```

### Comparing `PyExpUtils-andnp-4.0.0/PKG-INFO` & `PyExpUtils-andnp-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PyExpUtils-andnp
-Version: 4.0.0
+Version: 4.0.1
 Summary: A small set of utilities for RL and ML experiments
 License: MIT
 Author-email: Andy Patterson <andnpatterson@gmail.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # PyExpUtils
 
 [![Test](https://github.com/andnp/PyExpUtils/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/andnp/PyExpUtils/actions/workflows/test.yml)
 
 Short for python experiment utilities.
```

