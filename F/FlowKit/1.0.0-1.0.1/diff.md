# Comparing `tmp/FlowKit-1.0.0.tar.gz` & `tmp/FlowKit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowKit-1.0.0.tar", last modified: Wed Feb 22 21:50:30 2023, max compression
+gzip compressed data, was "FlowKit-1.0.1.tar", last modified: Mon May  8 23:00:34 2023, max compression
```

## Comparing `FlowKit-1.0.0.tar` & `FlowKit-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-02-22 21:50:30.534725 FlowKit-1.0.0/
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-02-22 21:50:30.530725 FlowKit-1.0.0/FlowKit.egg-info/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     9555 2023-02-22 21:50:30.000000 FlowKit-1.0.0/FlowKit.egg-info/PKG-INFO
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     1264 2023-02-22 21:50:30.000000 FlowKit-1.0.0/FlowKit.egg-info/SOURCES.txt
--rw-rw-r--   0 swhite    (1000) swhite    (1000)        1 2023-02-22 21:50:30.000000 FlowKit-1.0.0/FlowKit.egg-info/dependency_links.txt
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      169 2023-02-22 21:50:30.000000 FlowKit-1.0.0/FlowKit.egg-info/requires.txt
--rw-rw-r--   0 swhite    (1000) swhite    (1000)        8 2023-02-22 21:50:30.000000 FlowKit-1.0.0/FlowKit.egg-info/top_level.txt
--rw-r--r--   0 swhite    (1000) swhite    (1000)     1511 2019-08-08 15:30:26.000000 FlowKit-1.0.0/LICENSE
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       69 2022-07-18 16:34:26.000000 FlowKit-1.0.0/MANIFEST.in
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     9555 2023-02-22 21:50:30.534725 FlowKit-1.0.0/PKG-INFO
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     9129 2023-02-22 16:57:29.000000 FlowKit-1.0.0/README.md
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-02-22 21:50:30.530725 FlowKit-1.0.0/flowkit/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      978 2023-01-24 14:08:16.000000 FlowKit-1.0.0/flowkit/__init__.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      769 2022-07-18 16:34:27.000000 FlowKit-1.0.0/flowkit/_conf.py
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-02-22 21:50:30.530725 FlowKit-1.0.0/flowkit/_models/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       36 2022-07-18 16:34:27.000000 FlowKit-1.0.0/flowkit/_models/__init__.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     5252 2022-10-12 15:57:40.000000 FlowKit-1.0.0/flowkit/_models/dimension.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     3274 2023-01-24 14:08:16.000000 FlowKit-1.0.0/flowkit/_models/gate_node.py
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-02-22 21:50:30.530725 FlowKit-1.0.0/flowkit/_models/gates/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      251 2022-07-18 16:34:27.000000 FlowKit-1.0.0/flowkit/_models/gates/__init__.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     1174 2023-01-24 14:08:16.000000 FlowKit-1.0.0/flowkit/_models/gates/_base_gate.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    15888 2023-01-24 14:08:16.000000 FlowKit-1.0.0/flowkit/_models/gates/_gates.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    13786 2023-01-24 14:08:16.000000 FlowKit-1.0.0/flowkit/_models/gates/_gml_gates.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     9766 2023-01-24 14:08:16.000000 FlowKit-1.0.0/flowkit/_models/gates/_wsp_gates.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     6399 2022-07-18 16:34:27.000000 FlowKit-1.0.0/flowkit/_models/gating_results.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    37944 2023-02-21 18:59:20.000000 FlowKit-1.0.0/flowkit/_models/gating_strategy.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    51529 2023-02-16 04:12:02.000000 FlowKit-1.0.0/flowkit/_models/sample.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    32867 2023-02-20 22:54:38.000000 FlowKit-1.0.0/flowkit/_models/session.py
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-02-22 21:50:30.534725 FlowKit-1.0.0/flowkit/_models/transforms/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      446 2022-07-18 16:34:27.000000 FlowKit-1.0.0/flowkit/_models/transforms/__init__.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     1515 2023-01-24 14:08:16.000000 FlowKit-1.0.0/flowkit/_models/transforms/_base_transform.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    10923 2023-02-14 17:29:54.000000 FlowKit-1.0.0/flowkit/_models/transforms/_gml_transforms.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     4163 2022-10-12 15:57:40.000000 FlowKit-1.0.0/flowkit/_models/transforms/_matrix.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    11735 2022-07-18 16:34:27.000000 FlowKit-1.0.0/flowkit/_models/transforms/_transforms.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     8240 2022-10-11 20:08:25.000000 FlowKit-1.0.0/flowkit/_models/transforms/_wsp_transforms.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    37605 2023-02-20 20:53:13.000000 FlowKit-1.0.0/flowkit/_models/workspace.py
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-02-22 21:50:30.534725 FlowKit-1.0.0/flowkit/_resources/
--rw-r--r--   0 swhite    (1000) swhite    (1000)     4954 2019-08-08 15:31:13.000000 FlowKit-1.0.0/flowkit/_resources/DataTypes.v2.0.xsd
--rw-r--r--   0 swhite    (1000) swhite    (1000)    11745 2019-08-08 15:31:13.000000 FlowKit-1.0.0/flowkit/_resources/Gating-ML.v2.0.xsd
--rw-r--r--   0 swhite    (1000) swhite    (1000)     9405 2019-08-08 15:31:13.000000 FlowKit-1.0.0/flowkit/_resources/Transformations.v2.0.xsd
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      814 2022-09-01 17:34:53.000000 FlowKit-1.0.0/flowkit/_resources/__init__.py
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-02-22 21:50:30.534725 FlowKit-1.0.0/flowkit/_utils/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       21 2022-07-18 16:34:27.000000 FlowKit-1.0.0/flowkit/_utils/__init__.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     4790 2023-01-24 14:08:16.000000 FlowKit-1.0.0/flowkit/_utils/gating_utils.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    14764 2023-02-16 17:55:39.000000 FlowKit-1.0.0/flowkit/_utils/plot_utils.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     2337 2023-02-03 18:53:15.000000 FlowKit-1.0.0/flowkit/_utils/sample_utils.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    45011 2023-02-20 20:42:42.000000 FlowKit-1.0.0/flowkit/_utils/wsp_utils.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    30404 2023-02-20 22:54:38.000000 FlowKit-1.0.0/flowkit/_utils/xml_utils.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       46 2023-02-22 16:57:29.000000 FlowKit-1.0.0/flowkit/_version.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      946 2023-01-26 16:21:41.000000 FlowKit-1.0.0/flowkit/exceptions.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       38 2023-02-22 21:50:30.534725 FlowKit-1.0.0/setup.cfg
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     1404 2023-02-22 17:23:37.000000 FlowKit-1.0.0/setup.py
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.459097 FlowKit-1.0.1/
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.451097 FlowKit-1.0.1/FlowKit.egg-info/
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     9746 2023-05-08 23:00:34.000000 FlowKit-1.0.1/FlowKit.egg-info/PKG-INFO
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     1264 2023-05-08 23:00:34.000000 FlowKit-1.0.1/FlowKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)        1 2023-05-08 23:00:34.000000 FlowKit-1.0.1/FlowKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)      169 2023-05-08 23:00:34.000000 FlowKit-1.0.1/FlowKit.egg-info/requires.txt
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)        8 2023-05-08 23:00:34.000000 FlowKit-1.0.1/FlowKit.egg-info/top_level.txt
+-rw-r--r--   0 swhite    (1000) swhite    (1000)     1511 2019-08-08 15:30:26.000000 FlowKit-1.0.1/LICENSE
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)       69 2022-07-18 16:34:26.000000 FlowKit-1.0.1/MANIFEST.in
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     9746 2023-05-08 23:00:34.459097 FlowKit-1.0.1/PKG-INFO
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     9320 2023-05-08 14:38:48.000000 FlowKit-1.0.1/README.md
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.451097 FlowKit-1.0.1/flowkit/
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)      978 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/__init__.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)      769 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_conf.py
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.455097 FlowKit-1.0.1/flowkit/_models/
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)       36 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_models/__init__.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     5252 2022-10-12 15:57:40.000000 FlowKit-1.0.1/flowkit/_models/dimension.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     3274 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_models/gate_node.py
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.455097 FlowKit-1.0.1/flowkit/_models/gates/
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)      251 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_models/gates/__init__.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     1174 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_models/gates/_base_gate.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    15888 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_models/gates/_gates.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    13786 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_models/gates/_gml_gates.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     9766 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_models/gates/_wsp_gates.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     6399 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_models/gating_results.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    37951 2023-05-08 22:51:18.000000 FlowKit-1.0.1/flowkit/_models/gating_strategy.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    51529 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_models/sample.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    32867 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_models/session.py
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.455097 FlowKit-1.0.1/flowkit/_models/transforms/
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)      446 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_models/transforms/__init__.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     1515 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_models/transforms/_base_transform.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    10923 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_models/transforms/_gml_transforms.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     4292 2023-05-08 22:51:18.000000 FlowKit-1.0.1/flowkit/_models/transforms/_matrix.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    11735 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_models/transforms/_transforms.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     8240 2022-10-11 20:08:25.000000 FlowKit-1.0.1/flowkit/_models/transforms/_wsp_transforms.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    37605 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_models/workspace.py
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.455097 FlowKit-1.0.1/flowkit/_resources/
+-rw-r--r--   0 swhite    (1000) swhite    (1000)     4954 2019-08-08 15:31:13.000000 FlowKit-1.0.1/flowkit/_resources/DataTypes.v2.0.xsd
+-rw-r--r--   0 swhite    (1000) swhite    (1000)    11745 2019-08-08 15:31:13.000000 FlowKit-1.0.1/flowkit/_resources/Gating-ML.v2.0.xsd
+-rw-r--r--   0 swhite    (1000) swhite    (1000)     9405 2019-08-08 15:31:13.000000 FlowKit-1.0.1/flowkit/_resources/Transformations.v2.0.xsd
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)      814 2022-09-01 17:34:53.000000 FlowKit-1.0.1/flowkit/_resources/__init__.py
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-08 23:00:34.459097 FlowKit-1.0.1/flowkit/_utils/
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)       21 2022-07-18 16:34:27.000000 FlowKit-1.0.1/flowkit/_utils/__init__.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     4790 2023-01-24 14:08:16.000000 FlowKit-1.0.1/flowkit/_utils/gating_utils.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    14764 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_utils/plot_utils.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     2337 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_utils/sample_utils.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    45011 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_utils/wsp_utils.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    30404 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/_utils/xml_utils.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)       46 2023-05-08 22:52:05.000000 FlowKit-1.0.1/flowkit/_version.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)      946 2023-02-22 22:15:26.000000 FlowKit-1.0.1/flowkit/exceptions.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)       38 2023-05-08 23:00:34.459097 FlowKit-1.0.1/setup.cfg
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     1404 2023-02-22 22:15:26.000000 FlowKit-1.0.1/setup.py
```

### Comparing `FlowKit-1.0.0/FlowKit.egg-info/PKG-INFO` & `FlowKit-1.0.1/FlowKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: FlowKit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Flow Cytometry Toolkit
 Home-page: https://github.com/whitews/flowkit
 Author: Scott White
 License: BSD
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# FlowKit
+
 [!["FlowKit"](https://raw.githubusercontent.com/whitews/FlowKit/master/docs/_static/flowkit.png)](https://github.com/whitews/flowkit)
 
 [![PyPI license](https://img.shields.io/pypi/l/flowkit.svg?colorB=dodgerblue)](https://pypi.python.org/pypi/flowkit/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/flowkit.svg)](https://pypi.python.org/pypi/flowkit/)
 [![PyPI version](https://img.shields.io/pypi/v/flowkit.svg?colorB=blue)](https://pypi.python.org/pypi/flowkit/)
 [![DOI](https://zenodo.org/badge/138655889.svg)](https://zenodo.org/badge/latestdoi/138655889)
 
@@ -151,14 +153,15 @@
 
 Below are more advanced and practical examples for using FlowKit. If you have an example you would like to submit for consideration in this list (preferably with data), please [submit an issue](https://github.com/whitews/FlowKit/issues/new/).
 
 * [Compare mean fluorescence intensity (MFI) in gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/flowkit-session-compare-mfi-of-gated-events.ipynb)
 * [Importing a FlowJo 10 WSP file & replicating analysis in FlowKit](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/flowkit-session-replicate-flowjo-wsp.ipynb)
 * [Dimension reduction on gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/dimension_reduction_on_gated_populations.ipynb)
 * [Comparison between Leiden & Louvain clustering](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/clustering_comparison_leiden_vs_louvain.ipynb)
+* [Saving Flow Analysis Data as AnnData objects for ScanPy](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/scanpy_creating_and_using_AnnData_objects.ipynb)
 
 ## Contributing
 
 Want to get involved in the development of FlowKit? 
 
 [Read our CONTRIBUTING guidelines](https://github.com/whitews/FlowKit/blob/master/CONTRIBUTING.md)
```

### Comparing `FlowKit-1.0.0/FlowKit.egg-info/SOURCES.txt` & `FlowKit-1.0.1/FlowKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/LICENSE` & `FlowKit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/PKG-INFO` & `FlowKit-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: FlowKit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Flow Cytometry Toolkit
 Home-page: https://github.com/whitews/flowkit
 Author: Scott White
 License: BSD
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# FlowKit
+
 [!["FlowKit"](https://raw.githubusercontent.com/whitews/FlowKit/master/docs/_static/flowkit.png)](https://github.com/whitews/flowkit)
 
 [![PyPI license](https://img.shields.io/pypi/l/flowkit.svg?colorB=dodgerblue)](https://pypi.python.org/pypi/flowkit/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/flowkit.svg)](https://pypi.python.org/pypi/flowkit/)
 [![PyPI version](https://img.shields.io/pypi/v/flowkit.svg?colorB=blue)](https://pypi.python.org/pypi/flowkit/)
 [![DOI](https://zenodo.org/badge/138655889.svg)](https://zenodo.org/badge/latestdoi/138655889)
 
@@ -151,14 +153,15 @@
 
 Below are more advanced and practical examples for using FlowKit. If you have an example you would like to submit for consideration in this list (preferably with data), please [submit an issue](https://github.com/whitews/FlowKit/issues/new/).
 
 * [Compare mean fluorescence intensity (MFI) in gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/flowkit-session-compare-mfi-of-gated-events.ipynb)
 * [Importing a FlowJo 10 WSP file & replicating analysis in FlowKit](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/flowkit-session-replicate-flowjo-wsp.ipynb)
 * [Dimension reduction on gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/dimension_reduction_on_gated_populations.ipynb)
 * [Comparison between Leiden & Louvain clustering](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/clustering_comparison_leiden_vs_louvain.ipynb)
+* [Saving Flow Analysis Data as AnnData objects for ScanPy](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/scanpy_creating_and_using_AnnData_objects.ipynb)
 
 ## Contributing
 
 Want to get involved in the development of FlowKit? 
 
 [Read our CONTRIBUTING guidelines](https://github.com/whitews/FlowKit/blob/master/CONTRIBUTING.md)
```

### Comparing `FlowKit-1.0.0/README.md` & `FlowKit-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# FlowKit
+
 [!["FlowKit"](https://raw.githubusercontent.com/whitews/FlowKit/master/docs/_static/flowkit.png)](https://github.com/whitews/flowkit)
 
 [![PyPI license](https://img.shields.io/pypi/l/flowkit.svg?colorB=dodgerblue)](https://pypi.python.org/pypi/flowkit/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/flowkit.svg)](https://pypi.python.org/pypi/flowkit/)
 [![PyPI version](https://img.shields.io/pypi/v/flowkit.svg?colorB=blue)](https://pypi.python.org/pypi/flowkit/)
 [![DOI](https://zenodo.org/badge/138655889.svg)](https://zenodo.org/badge/latestdoi/138655889)
 
@@ -137,14 +139,15 @@
 
 Below are more advanced and practical examples for using FlowKit. If you have an example you would like to submit for consideration in this list (preferably with data), please [submit an issue](https://github.com/whitews/FlowKit/issues/new/).
 
 * [Compare mean fluorescence intensity (MFI) in gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/flowkit-session-compare-mfi-of-gated-events.ipynb)
 * [Importing a FlowJo 10 WSP file & replicating analysis in FlowKit](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/flowkit-session-replicate-flowjo-wsp.ipynb)
 * [Dimension reduction on gated populations](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/dimension_reduction_on_gated_populations.ipynb)
 * [Comparison between Leiden & Louvain clustering](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/clustering_comparison_leiden_vs_louvain.ipynb)
+* [Saving Flow Analysis Data as AnnData objects for ScanPy](https://github.com/whitews/FlowKit/blob/master/docs/notebooks/advanced/scanpy_creating_and_using_AnnData_objects.ipynb)
 
 ## Contributing
 
 Want to get involved in the development of FlowKit? 
 
 [Read our CONTRIBUTING guidelines](https://github.com/whitews/FlowKit/blob/master/CONTRIBUTING.md)
```

### Comparing `FlowKit-1.0.0/flowkit/__init__.py` & `FlowKit-1.0.1/flowkit/__init__.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_conf.py` & `FlowKit-1.0.1/flowkit/_conf.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/dimension.py` & `FlowKit-1.0.1/flowkit/_models/dimension.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/gate_node.py` & `FlowKit-1.0.1/flowkit/_models/gate_node.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/gates/_base_gate.py` & `FlowKit-1.0.1/flowkit/_models/gates/_base_gate.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/gates/_gates.py` & `FlowKit-1.0.1/flowkit/_models/gates/_gates.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/gates/_gml_gates.py` & `FlowKit-1.0.1/flowkit/_models/gates/_gml_gates.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/gates/_wsp_gates.py` & `FlowKit-1.0.1/flowkit/_models/gates/_wsp_gates.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/gating_results.py` & `FlowKit-1.0.1/flowkit/_models/gating_results.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/gating_strategy.py` & `FlowKit-1.0.1/flowkit/_models/gating_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,27 +585,27 @@
 
         if events is not None:
             return events
 
         if comp_ref == 'FCS':
             meta = sample.get_metadata()
 
-            if 'spill' not in meta or 'spillover' not in meta:
+            if 'spill' not in meta and 'spillover' not in meta:
                 # GML 2.0 spec states if 'FCS' is specified but no spill is present, treat as uncompensated
                 events = sample.get_events(source='raw')
                 return events.copy()
 
             try:
                 spill = meta['spillover']  # preferred, per FCS standard
             except KeyError:
                 spill = meta['spill']
 
             detectors = [sample.pnn_labels[i] for i in sample.fluoro_indices]
             fluorochromes = [sample.pns_labels[i] for i in sample.fluoro_indices]
-            matrix = Matrix('fcs', spill, detectors, fluorochromes, null_channels=sample.null_channels)
+            matrix = Matrix('tmp_spill', spill, detectors, fluorochromes, null_channels=sample.null_channels)
         else:
             # lookup specified comp-ref in gating strategy
             matrix = self.comp_matrices[comp_ref]
 
         if matrix is not None:
             events = matrix.apply(sample)
             # cache the comp events
```

### Comparing `FlowKit-1.0.0/flowkit/_models/sample.py` & `FlowKit-1.0.1/flowkit/_models/sample.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/session.py` & `FlowKit-1.0.1/flowkit/_models/session.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/transforms/_base_transform.py` & `FlowKit-1.0.1/flowkit/_models/transforms/_base_transform.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/transforms/_gml_transforms.py` & `FlowKit-1.0.1/flowkit/_models/transforms/_gml_transforms.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/transforms/_matrix.py` & `FlowKit-1.0.1/flowkit/_models/transforms/_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,18 @@
             self,
             matrix_id,
             spill_data_or_file,
             detectors,
             fluorochromes=None,
             null_channels=None
     ):
-        if matrix_id == 'uncompensated' or matrix_id == 'fcs':
+        # Technically, the GML 2.0 spec states 'FCS' (note uppercase) is reserved, but we'll cover that case-insensitive
+        if matrix_id == 'uncompensated' or matrix_id.lower() == 'fcs':
             raise ValueError(
-                "Matrix IDs 'uncompensated' and 'fcs' are reserved compensation references " +
+                "Matrix IDs 'uncompensated' and 'FCS' are reserved compensation references " +
                 "used in Dimension instances to specify that channel data should either be " +
                 "uncompensated or compensated using the spill value from a Sample's metadata"
             )
 
         if isinstance(spill_data_or_file, np.ndarray):
             spill = spill_data_or_file
         else:
```

### Comparing `FlowKit-1.0.0/flowkit/_models/transforms/_transforms.py` & `FlowKit-1.0.1/flowkit/_models/transforms/_transforms.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/transforms/_wsp_transforms.py` & `FlowKit-1.0.1/flowkit/_models/transforms/_wsp_transforms.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_models/workspace.py` & `FlowKit-1.0.1/flowkit/_models/workspace.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_resources/DataTypes.v2.0.xsd` & `FlowKit-1.0.1/flowkit/_resources/DataTypes.v2.0.xsd`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_resources/Gating-ML.v2.0.xsd` & `FlowKit-1.0.1/flowkit/_resources/Gating-ML.v2.0.xsd`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_resources/Transformations.v2.0.xsd` & `FlowKit-1.0.1/flowkit/_resources/Transformations.v2.0.xsd`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_resources/__init__.py` & `FlowKit-1.0.1/flowkit/_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_utils/gating_utils.py` & `FlowKit-1.0.1/flowkit/_utils/gating_utils.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_utils/plot_utils.py` & `FlowKit-1.0.1/flowkit/_utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_utils/sample_utils.py` & `FlowKit-1.0.1/flowkit/_utils/sample_utils.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_utils/wsp_utils.py` & `FlowKit-1.0.1/flowkit/_utils/wsp_utils.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/_utils/xml_utils.py` & `FlowKit-1.0.1/flowkit/_utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/flowkit/exceptions.py` & `FlowKit-1.0.1/flowkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.0.0/setup.py` & `FlowKit-1.0.1/setup.py`

 * *Files identical despite different names*

