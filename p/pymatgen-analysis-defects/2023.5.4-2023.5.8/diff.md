# Comparing `tmp/pymatgen-analysis-defects-2023.5.4.tar.gz` & `tmp/pymatgen-analysis-defects-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatgen-analysis-defects-2023.5.4.tar", last modified: Thu May  4 22:57:36 2023, max compression
+gzip compressed data, was "pymatgen-analysis-defects-2023.5.8.tar", last modified: Mon May  8 23:46:05 2023, max compression
```

## Comparing `pymatgen-analysis-defects-2023.5.4.tar` & `pymatgen-analysis-defects-2023.5.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.123659 pymatgen-analysis-defects-2023.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-04 22:57:36.127658 pymatgen-analysis-defects-2023.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.119658 pymatgen-analysis-defects-2023.5.4/pymatgen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.119658 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.123659 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26443 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.123659 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/corrections/
--rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/corrections/freysoldt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/corrections/kumagai.py
--rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17001 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/recombination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/supercells.py
--rw-r--r--   0 runner    (1001) docker     (123)    42384 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)    38571 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.123659 pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-04 22:57:36.000000 pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-04 22:57:36.000000 pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:57:36.000000 pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 22:57:36.000000 pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 22:57:36.000000 pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 22:57:36.127658 pymatgen-analysis-defects-2023.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:57:36.123659 pymatgen-analysis-defects-2023.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/tests/test_ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-04 22:57:21.000000 pymatgen-analysis-defects-2023.5.4/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-04 22:57:22.000000 pymatgen-analysis-defects-2023.5.4/tests/test_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-04 22:57:22.000000 pymatgen-analysis-defects-2023.5.4/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-04 22:57:22.000000 pymatgen-analysis-defects-2023.5.4/tests/test_recombination.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-04 22:57:22.000000 pymatgen-analysis-defects-2023.5.4/tests/test_supercells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-05-04 22:57:22.000000 pymatgen-analysis-defects-2023.5.4/tests/test_thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-04 22:57:22.000000 pymatgen-analysis-defects-2023.5.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.506053 pymatgen-analysis-defects-2023.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-08 23:46:05.506053 pymatgen-analysis-defects-2023.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.498053 pymatgen-analysis-defects-2023.5.8/pymatgen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.498053 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.502053 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26443 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.506053 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/corrections/
+-rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/corrections/freysoldt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/corrections/kumagai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17001 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/supercells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42384 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38571 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.506053 pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-08 23:46:05.000000 pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-08 23:46:05.000000 pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 23:46:05.000000 pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-08 23:46:05.000000 pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 23:46:05.000000 pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 23:46:05.506053 pymatgen-analysis-defects-2023.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.506053 pymatgen-analysis-defects-2023.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/tests/test_ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-08 23:45:49.000000 pymatgen-analysis-defects-2023.5.8/tests/test_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-08 23:45:49.000000 pymatgen-analysis-defects-2023.5.8/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-08 23:45:49.000000 pymatgen-analysis-defects-2023.5.8/tests/test_recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-08 23:45:49.000000 pymatgen-analysis-defects-2023.5.8/tests/test_supercells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-05-08 23:45:49.000000 pymatgen-analysis-defects-2023.5.8/tests/test_thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-08 23:45:49.000000 pymatgen-analysis-defects-2023.5.8/tests/test_utils.py
```

### Comparing `pymatgen-analysis-defects-2023.5.4/LICENSE` & `pymatgen-analysis-defects-2023.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/PKG-INFO` & `pymatgen-analysis-defects-2023.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2023.5.4
+Version: 2023.5.8
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
```

### Comparing `pymatgen-analysis-defects-2023.5.4/README.rst` & `pymatgen-analysis-defects-2023.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/ccd.py` & `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/ccd.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/constants.py` & `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/constants.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/core.py` & `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/core.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/corrections/freysoldt.py` & `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/corrections/freysoldt.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/corrections/kumagai.py` & `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/corrections/kumagai.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/finder.py` & `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/finder.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/generators.py` & `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/generators.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/recombination.py` & `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/recombination.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/supercells.py` & `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/supercells.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/thermo.py` & `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/thermo.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/pymatgen/analysis/defects/utils.py` & `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/utils.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/PKG-INFO` & `pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2023.5.4
+Version: 2023.5.8
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
```

### Comparing `pymatgen-analysis-defects-2023.5.4/pymatgen_analysis_defects.egg-info/SOURCES.txt` & `pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/pyproject.toml` & `pymatgen-analysis-defects-2023.5.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   "Programming Language :: Python :: 3.10",
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Science/Research",
   "Operating System :: OS Independent",
   "Topic :: Other/Nonlisted Topic",
   "Topic :: Scientific/Engineering",
 ]
-dependencies = ["pymatgen==2023.1.9", "scikit-image>=0.19.3", "mp-pyrho>=0.3.0", "numpy<=1.23.5"]
+dependencies = ["pymatgen>=2023.5.8", "scikit-image>=0.19.3", "mp-pyrho>=0.3.0", "numpy<=1.23.5"]
 description = "Pymatgen extension for defects analysis"
 dynamic = ["version"]
 keywords = ["high-throughput", "automated", "dft", "defects"]
 license = { text = "modified BSD" }
 name = "pymatgen-analysis-defects"
 readme = "README.rst"
 requires-python = '>=3.8'
@@ -29,21 +29,20 @@
 dev = ["pre-commit>=2.12.1"]
 docs = [
   "jupyter-book>=0.13.1",
 ]
 pydefect = ["pydefect>=0.6.2"]
 
 strict = [
-  "pymatgen==2023.1.9",
+  "pymatgen>=2023.5.8",
   "dscribe==1.2.2",
   "scikit-image==0.19.3",
   "pytest==7.2.2",
   "pytest-cov==4.0.0",
   "pre-commit==3.1.0",
-  "pydefect==0.7.0",
   "mp-pyrho==0.3.0",
   "numpy==1.23.5"
 ]
 
 tests = ["pytest==7.2.2", "pytest-cov==4.0.0"]
 
 [tool.setuptools.dynamic]
```

### Comparing `pymatgen-analysis-defects-2023.5.4/tests/test_ccd.py` & `pymatgen-analysis-defects-2023.5.8/tests/test_ccd.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/tests/test_core.py` & `pymatgen-analysis-defects-2023.5.8/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/tests/test_corrections.py` & `pymatgen-analysis-defects-2023.5.8/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/tests/test_finder.py` & `pymatgen-analysis-defects-2023.5.8/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/tests/test_generators.py` & `pymatgen-analysis-defects-2023.5.8/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/tests/test_recombination.py` & `pymatgen-analysis-defects-2023.5.8/tests/test_recombination.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/tests/test_supercells.py` & `pymatgen-analysis-defects-2023.5.8/tests/test_supercells.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/tests/test_thermo.py` & `pymatgen-analysis-defects-2023.5.8/tests/test_thermo.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.4/tests/test_utils.py` & `pymatgen-analysis-defects-2023.5.8/tests/test_utils.py`

 * *Files identical despite different names*

