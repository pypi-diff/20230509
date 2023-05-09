# Comparing `tmp/ecoscope-1.1.2.tar.gz` & `tmp/ecoscope-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoscope-1.1.2.tar", last modified: Wed Feb  8 07:18:39 2023, max compression
+gzip compressed data, was "ecoscope-1.2.0.tar", last modified: Tue May  9 13:40:43 2023, max compression
```

## Comparing `ecoscope-1.1.2.tar` & `ecoscope-1.2.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-02-08 07:18:39.263688 ecoscope-1.1.2/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2023-02-08 06:59:30.000000 ecoscope-1.1.2/LICENSE
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-02-08 07:18:39.263688 ecoscope-1.1.2/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2935 2023-02-08 06:59:30.000000 ecoscope-1.1.2/README.rst
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-02-08 07:18:39.255688 ecoscope-1.1.2/ecoscope/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3753 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/__init__.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-02-08 07:18:39.255688 ecoscope-1.1.2/ecoscope/analysis/
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-02-08 07:18:39.259688 ecoscope-1.1.2/ecoscope/analysis/UD/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/analysis/UD/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/analysis/UD/etd_range.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/analysis/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/analysis/astronomy.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/analysis/ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3881 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/analysis/geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/analysis/immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/analysis/percentile.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/analysis/proximity.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3505 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/analysis/seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2735 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/analysis/speed.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-02-08 07:18:39.259688 ecoscope-1.1.2/ecoscope/base/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/base/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/base/_dataclasses.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25180 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/base/base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6650 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/base/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-02-08 07:18:39.259688 ecoscope-1.1.2/ecoscope/contrib/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       60 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/contrib/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/contrib/basemaps.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    34508 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/contrib/dasclient.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   112572 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/contrib/foliumap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2197 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/contrib/legend.txt
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-02-08 07:18:39.259688 ecoscope-1.1.2/ecoscope/io/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/io/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    29580 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/io/earthranger.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    12171 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/io/eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6620 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/io/raster.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2225 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/io/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-02-08 07:18:39.259688 ecoscope-1.1.2/ecoscope/mapping/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      141 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/mapping/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    17821 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/mapping/map.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-02-08 07:18:39.259688 ecoscope-1.1.2/ecoscope/plotting/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      376 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/plotting/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    14348 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/plotting/plot.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2023-02-08 06:59:30.000000 ecoscope-1.1.2/ecoscope/version.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-02-08 07:18:39.255688 ecoscope-1.1.2/ecoscope.egg-info/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-02-08 07:18:39.000000 ecoscope-1.1.2/ecoscope.egg-info/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1352 2023-02-08 07:18:39.000000 ecoscope-1.1.2/ecoscope.egg-info/SOURCES.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-02-08 07:18:39.000000 ecoscope-1.1.2/ecoscope.egg-info/dependency_links.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-02-08 07:18:39.000000 ecoscope-1.1.2/ecoscope.egg-info/not-zip-safe
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      265 2023-02-08 07:18:39.000000 ecoscope-1.1.2/ecoscope.egg-info/requires.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2023-02-08 07:18:39.000000 ecoscope-1.1.2/ecoscope.egg-info/top_level.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2023-02-08 06:59:30.000000 ecoscope-1.1.2/pyproject.toml
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2023-02-08 07:18:39.263688 ecoscope-1.1.2/setup.cfg
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1914 2023-02-08 06:59:30.000000 ecoscope-1.1.2/setup.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-02-08 07:18:39.263688 ecoscope-1.1.2/tests/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6080 2023-02-08 06:59:30.000000 ecoscope-1.1.2/tests/test_base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7590 2023-02-08 06:59:30.000000 ecoscope-1.1.2/tests/test_earthranger_io.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2023-02-08 06:59:30.000000 ecoscope-1.1.2/tests/test_ecodataframe.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5098 2023-02-08 06:59:30.000000 ecoscope-1.1.2/tests/test_ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      285 2023-02-08 06:59:30.000000 ecoscope-1.1.2/tests/test_ecomap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2907 2023-02-08 06:59:30.000000 ecoscope-1.1.2/tests/test_eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2023-02-08 06:59:30.000000 ecoscope-1.1.2/tests/test_geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2023-02-08 06:59:30.000000 ecoscope-1.1.2/tests/test_immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      862 2023-02-08 06:59:30.000000 ecoscope-1.1.2/tests/test_seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2023-02-08 06:59:30.000000 ecoscope-1.1.2/tests/test_speed.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1877 2023-02-08 06:59:30.000000 ecoscope-1.1.2/tests/test_ud.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      329 2023-02-08 06:59:30.000000 ecoscope-1.1.2/tests/test_utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.949401 ecoscope-1.2.0/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2023-05-09 13:36:07.000000 ecoscope-1.2.0/LICENSE
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-05-09 13:40:43.949401 ecoscope-1.2.0/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2935 2023-05-09 13:36:07.000000 ecoscope-1.2.0/README.rst
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.941401 ecoscope-1.2.0/ecoscope/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3744 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/__init__.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.945401 ecoscope-1.2.0/ecoscope/analysis/
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.945401 ecoscope-1.2.0/ecoscope/analysis/UD/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/UD/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/UD/etd_range.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/astronomy.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3881 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/percentile.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/proximity.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3505 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2735 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/speed.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.945401 ecoscope-1.2.0/ecoscope/base/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/base/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/base/_dataclasses.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25180 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/base/base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6650 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/base/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.945401 ecoscope-1.2.0/ecoscope/contrib/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       60 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/contrib/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/contrib/basemaps.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   112572 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/contrib/foliumap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2197 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/contrib/legend.txt
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.945401 ecoscope-1.2.0/ecoscope/io/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/io/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    32507 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/io/earthranger.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    12171 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/io/eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6620 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/io/raster.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2225 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/io/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.949401 ecoscope-1.2.0/ecoscope/mapping/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      141 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/mapping/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    17821 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/mapping/map.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.949401 ecoscope-1.2.0/ecoscope/plotting/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      376 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/plotting/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    14348 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/plotting/plot.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/version.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.945401 ecoscope-1.2.0/ecoscope.egg-info/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-05-09 13:40:43.000000 ecoscope-1.2.0/ecoscope.egg-info/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1322 2023-05-09 13:40:43.000000 ecoscope-1.2.0/ecoscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-09 13:40:43.000000 ecoscope-1.2.0/ecoscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-09 13:40:43.000000 ecoscope-1.2.0/ecoscope.egg-info/not-zip-safe
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      284 2023-05-09 13:40:43.000000 ecoscope-1.2.0/ecoscope.egg-info/requires.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2023-05-09 13:40:43.000000 ecoscope-1.2.0/ecoscope.egg-info/top_level.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2023-05-09 13:36:07.000000 ecoscope-1.2.0/pyproject.toml
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2023-05-09 13:40:43.949401 ecoscope-1.2.0/setup.cfg
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1940 2023-05-09 13:36:07.000000 ecoscope-1.2.0/setup.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.949401 ecoscope-1.2.0/tests/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6080 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6908 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_earthranger_io.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_ecodataframe.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5098 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      285 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_ecomap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2907 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      862 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_speed.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1877 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_ud.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      329 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_utils.py
```

### Comparing `ecoscope-1.1.2/LICENSE` & `ecoscope-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/PKG-INFO` & `ecoscope-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.1.2
+Version: 1.2.0
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.1.2/README.rst` & `ecoscope-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/__init__.py` & `ecoscope-1.2.0/ecoscope/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,20 +74,22 @@
 
     pio.templates.default = "seaborn"
 
     import sys
 
     if "google.colab" in sys.modules and selenium:
         from IPython import get_ipython
-        
+
         shell_text = """\
 cat > /etc/apt/sources.list.d/debian.list <<'EOF'
 deb [arch=amd64 signed-by=/usr/share/keyrings/debian-buster.gpg] http://deb.debian.org/debian buster main
-deb [arch=amd64 signed-by=/usr/share/keyrings/debian-buster-updates.gpg] http://deb.debian.org/debian buster-updates main
-deb [arch=amd64 signed-by=/usr/share/keyrings/debian-security-buster.gpg] http://deb.debian.org/debian-security buster/updates main
+deb [arch=amd64 signed-by=/usr/share/keyrings/debian-buster-updates.gpg]\
+        http://deb.debian.org/debian buster-updates main
+deb [arch=amd64 signed-by=/usr/share/keyrings/debian-security-buster.gpg]\
+        http://deb.debian.org/debian-security buster/updates main
 EOF
 
 apt-key adv --keyserver keyserver.ubuntu.com --recv-keys DCC9EFBF77E11517
 apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 648ACFD622F3D138
 apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 112695A0E562B32A
 
 apt-key export 77E11517 | gpg --dearmour -o /usr/share/keyrings/debian-buster.gpg
@@ -111,18 +113,19 @@
 EOF
 
 apt-get update
 apt-get install chromium chromium-driver
 
 pip install selenium
 """
-        
+
         if silent:
             from IPython.utils import io
-            with io.capture_output() as captured:
+
+            with io.capture_output():
                 get_ipython().run_cell_magic("shell", "", shell_text)
         else:
             get_ipython().run_cell_magic("shell", "", shell_text)
 
     __initialized = True
     if not silent:
         print(ASCII)
```

### Comparing `ecoscope-1.1.2/ecoscope/analysis/UD/etd_range.py` & `ecoscope-1.2.0/ecoscope/analysis/UD/etd_range.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/analysis/astronomy.py` & `ecoscope-1.2.0/ecoscope/analysis/astronomy.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/analysis/ecograph.py` & `ecoscope-1.2.0/ecoscope/analysis/ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/analysis/geofence.py` & `ecoscope-1.2.0/ecoscope/analysis/geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/analysis/immobility.py` & `ecoscope-1.2.0/ecoscope/analysis/immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/analysis/percentile.py` & `ecoscope-1.2.0/ecoscope/analysis/percentile.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/analysis/proximity.py` & `ecoscope-1.2.0/ecoscope/analysis/proximity.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/analysis/seasons.py` & `ecoscope-1.2.0/ecoscope/analysis/seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/analysis/speed.py` & `ecoscope-1.2.0/ecoscope/analysis/speed.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/base/__init__.py` & `ecoscope-1.2.0/ecoscope/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/base/_dataclasses.py` & `ecoscope-1.2.0/ecoscope/base/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/base/base.py` & `ecoscope-1.2.0/ecoscope/base/base.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/base/utils.py` & `ecoscope-1.2.0/ecoscope/base/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/contrib/basemaps.py` & `ecoscope-1.2.0/ecoscope/contrib/basemaps.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/contrib/foliumap.py` & `ecoscope-1.2.0/ecoscope/contrib/foliumap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/contrib/legend.txt` & `ecoscope-1.2.0/ecoscope/contrib/legend.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/io/earthranger.py` & `ecoscope-1.2.0/ecoscope/io/earthranger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,339 +1,198 @@
-import concurrent.futures
 import datetime
-import itertools
-import math
-import re
+import json
 import typing
 
-import backoff
 import geopandas as gpd
 import pandas as pd
 import requests
+from erclient.client import ERClient, ERClientException
 from tqdm.auto import tqdm
 
 import ecoscope
-from ecoscope.contrib.dasclient import DasClient, DasClientException
 from ecoscope.io.utils import pack_columns, to_hex
 
 
-class BackoffDasClient(DasClient):
-    """
-    Extends DasClient to add backoff to requests.
-
-    """
-
-    @backoff.on_exception(
-        backoff.expo,
-        requests.exceptions.RequestException,
-        max_tries=10,
-    )
-    @backoff.on_exception(
-        backoff.expo,
-        DasClientException,
-        max_tries=10,
-        giveup=lambda e: len(e.args) == 0
-        or not isinstance(e.args[0], str)
-        or re.match("Failed to call DAS web service. 50[24] .*", e.args[0]) is None,
-    )
-    def _get(self, *args, **kwargs):
-        return super()._get(*args, **kwargs)
+def fatal_status_code(e):
+    return 400 <= e.response.status_code < 500
 
 
-class ConcurrentDasClient(BackoffDasClient):
-    """
-    Extends DasClient to make multiple requests while maintaining interface.
-
-    """
+class EarthRangerIO(ERClient):
+    def __init__(self, sub_page_size=4000, tcp_limit=5, **kwargs):
+        if "server" in kwargs:
+            server = kwargs.pop("server")
+            kwargs["service_root"] = f"{server}/api/v1.0"
+            kwargs["token_url"] = f"{server}/oauth2/token"
 
-    def __init__(self, *, sub_page_size=4000, tcp_limit=5, **kwargs):
         self.sub_page_size = sub_page_size
         self.tcp_limit = tcp_limit
+        kwargs["client_id"] = kwargs.get("client_id", "das_web_client")
         super().__init__(**kwargs)
 
-    def _concurrent_get(self, path, stream=False, **kwargs):
-        page_size = kwargs.get("params", {}).get("page_size")
-
-        if page_size is None or page_size % self.sub_page_size or stream:
-            return super()._get(path, stream=stream, **kwargs)
-
-        p = kwargs["params"].copy()
-        p["page"] = int(p.get("page", 1))
-        current_page = p["page"]
-
-        p["page_size"] = 1
-        response = super()._get(path=path, params=p)
-        p["page_size"] = self.sub_page_size
-
-        if "count" not in response:
-            return response
-
-        if not response.get("count"):
-            return response
-
-        start = 1 + (p["page"] - 1) * page_size // self.sub_page_size
-        end = 1 + min(
-            p["page"] * page_size // self.sub_page_size,
-            math.ceil(response["count"] / self.sub_page_size),
-        )
-
-        if response["previous"] is not None:
-            response["previous"] = response["previous"].replace("page_size=1", f"page_size={page_size}")
-        if response["count"] > page_size * current_page:
-            response["next"] = response["next"].replace("page_size=1", f"page_size={page_size}")
-        else:
-            response["next"] = None
-
-        with concurrent.futures.ThreadPoolExecutor(max_workers=self.tcp_limit) as executor:
-            futures = []
-            for page in range(start, end):
-                p["page"] = page
-                futures.append(executor.submit(super()._get, path=path, params=p.copy()))
+    @staticmethod
+    def _clean_kwargs(addl_kwargs={}, **kwargs):
+        for k in addl_kwargs.keys():
+            print(f"Warning: {k} is a non-standard parameter. Results may be unexpected.")
+        return {k: v for k, v in {**addl_kwargs, **kwargs}.items() if v is not None}
 
-            response["results"] = itertools.chain(
-                *(future.result()["results"] for future in concurrent.futures.as_completed(futures))
-            )
-        return response
+    @staticmethod
+    def _normalize_column(df, col):
+        print(col)
+        for k, v in pd.json_normalize(df.pop(col), sep="__").add_prefix(f"{col}__").iteritems():
+            df[k] = v.values
 
-    def _get(self, *args, **kwargs):
-        params = kwargs.get("params", {})
-        if "sub_page_size" in params or "tcp_limit" in params:
-            print(
-                f"Warning: `sub_page_size` and `tcp_limit` should only be provided to the constructor of {type(self)}"
+    @staticmethod
+    def _dataframe_to_dict(events):
+        if isinstance(events, gpd.GeoDataFrame):
+            events["location"] = pd.DataFrame({"longitude": events.geometry.x, "latitude": events.geometry.y}).to_dict(
+                "records"
             )
-        params["page"] = params.get("page", 1)
-        params["page_size"] = params.get("page_size", 1000000000)
-        params = {k: v if not isinstance(v, bool) else str(v).lower() for k, v in params.items()}
-        kwargs["params"] = params
-        return self._concurrent_get(*args, **kwargs)
-
-
-class EarthRangerIO(ConcurrentDasClient):
-    """
-    Extends ConcurrentDasClient with Ecoscope-specific configuration.
-
-    """
-
-    def __init__(self, **kwargs):
-        if "server" in kwargs:
-            server = kwargs.pop("server")
-            kwargs["service_root"] = server + "/api/v1.0"
-            kwargs["token_url"] = server + "/oauth2/token"
-
-        kwargs["client_id"] = kwargs.get("client_id", "das_web_client")
+            del events["geometry"]
 
-        super().__init__(**kwargs)
+        if isinstance(events, pd.DataFrame):
+            events = events.to_dict("records")
+        return events
 
     @staticmethod
     def _to_gdf(df):
         longitude, latitude = (0, 1) if isinstance(df["location"].iat[0], list) else ("longitude", "latitude")
         return gpd.GeoDataFrame(
             df,
             geometry=gpd.points_from_xy(df["location"].str[longitude], df["location"].str[latitude]),
             crs=4326,
         )
 
-    @staticmethod
-    def _normalize_column(df, col):
-        print(col)
-        for k, v in pd.json_normalize(df.pop(col), sep="__").add_prefix(f"{col}__").iteritems():
-            df[k] = v.values
-
-    @staticmethod
-    def _clean_kwargs(addl_kwargs={}, **kwargs):
-        for k in addl_kwargs.keys():
-            print(f"Warning: {k} is a non-standard parameter. Results may be unexpected.")
-        return {k: v for k, v in {**addl_kwargs, **kwargs}.items() if v is not None}
+    """
+    GET Functions
+    """
 
-    def get_subjectsources(self, subjects=None, sources=None, **addl_kwargs):
+    def get_sources(
+        self,
+        manufacturer_id=None,
+        provider_key=None,
+        provider=None,
+        id=None,
+        **addl_kwargs,
+    ):
         """
         Parameters
         ----------
-        subjects
-            A comma-delimited list of Subject IDs.
-        sources
-            A comma-delimited list of Source IDs.
-
+        manufacturer_id
+        provider_key
+        provider
+        id
         Returns
         -------
-        subjectsources : pd.DataFrame
-            DataFrame of queried subjectssources
-
+        sources : pd.DataFrame
+            DataFrame of queried sources
         """
 
-        kwargs = self._clean_kwargs(
+        params = self._clean_kwargs(
             addl_kwargs,
-            subjects=subjects,
-            sources=sources,
+            manufacturer_id=manufacturer_id,
+            provider_key=provider_key,
+            provider=provider,
+            id=id,
         )
-
-        return pd.DataFrame(self._get("subjectsources/", params=kwargs)["results"])
+        df = pd.DataFrame(
+            self.get_objects_multithreaded(
+                object="sources/", threads=self.tcp_limit, page_size=self.sub_page_size, **params
+            )
+        )
+        assert not df.empty
+        return df
 
     def get_subjects(
         self,
         include_inactive=None,
-        tracks_since=None,
-        tracks_until=None,
         bbox=None,
         subject_group=None,
         name=None,
         updated_since=None,
-        render_last_location=None,
         tracks=None,
         id=None,
         updated_until=None,
         group_name=None,
         **addl_kwargs,
     ):
         """
         Parameters
         ----------
-        include_inactive
-            Include inactive subjects in list.
-        tracks_since
-            Include tracks since this timestamp
-        tracks_until
-            Include tracks up through this timestamp
-        bbox
-            Include subjects having track data within this bounding box defined by a 4-tuple of coordinates marking
+        include_inactive: Include inactive subjects in list.
+        bbox: Include subjects having track data within this bounding box defined by a 4-tuple of coordinates marking
             west, south, east, north.
-        subject_group
-            Indicate a subject group for which Subjects should be listed.
-        name : UUID
-            Find subjects with the given name.
-        updated_since
-            Return Subject that have been updated since the given timestamp.
-        render_last_location
-            Indicate whether to render each subject's last location.
-        tracks
-            Indicate whether to render each subject's recent tracks.
-        id
-            A comma-delimited list of Subject IDs.
+        subject_group: Indicate a subject group for which Subjects should be listed.
+        name : Find subjects with the given name
+        updated_since: Return Subject that have been updated since the given timestamp.
+        tracks: Indicate whether to render each subject's recent tracks.
+        id: A comma-delimited list of Subject IDs.
         updated_until
         group_name
-
         Returns
         -------
         subjects : pd.DataFrame
-            DataFrame of queried subjects
-
         """
 
-        kwargs = self._clean_kwargs(
+        params = self._clean_kwargs(
             addl_kwargs,
             include_inactive=include_inactive,
-            tracks_since=tracks_since,
-            tracks_until=tracks_until,
             bbox=bbox,
             subject_group=subject_group,
             name=name,
             updated_since=updated_since,
-            render_last_location=render_last_location,
             tracks=tracks,
             id=id,
             updated_until=updated_until,
             group_name=group_name,
         )
 
-        assert kwargs.get("subject_group") is None or kwargs.get("group_name") is None
+        assert params.get("subject_group") is None or params.get("group_name") is None
 
-        if kwargs.get("group_name") is not None:
+        if params.get("group_name") is not None:
             try:
-                kwargs["subject_group"] = self._get(
+                params["subject_group"] = self._get(
                     "subjectgroups/",
                     params={
-                        "group_name": kwargs.pop("group_name"),
+                        "group_name": params.pop("group_name"),
                         "include_inactive": True,
                         "include_hidden": True,
                         "flat": True,
                     },
                 )[0]["id"]
             except IndexError:
                 raise KeyError("`group_name` not found")
 
-        df = pd.DataFrame(self._get("subjects/", params=kwargs)["results"])
+        df = pd.DataFrame(
+            self.get_objects_multithreaded(
+                object="subjects/", threads=self.tcp_limit, page_size=self.sub_page_size, **params
+            )
+        )
         assert not df.empty
 
         df["hex"] = df["additional"].str["rgb"].map(to_hex) if "additional" in df else "#ff0000"
 
         return df
 
-    def get_patrols(self, filter=None, status=None, **addl_kwargs):
-        """
-        Parameters
-        ----------
-        filter:
-            example: {"date_range":{"lower":"2020-09-16T00:00:00.000Z"}}
-            date_range
-            patrols_overlap_daterange
-            text
-            patrol_type
-            tracked_by
-        status
-            Comma-separated list of 'scheduled'/'active'/'overdue'/'done'/'cancelled'
-
-        Returns
-        -------
-        patrols : pd.DataFrame
-            DataFrame of queried patrols
-
-        """
-
-        kwargs = self._clean_kwargs(
-            addl_kwargs,
-            filter=filter,
-            status=status,
-        )
-
-        return pd.DataFrame(self._get("activity/patrols/", params=kwargs)["results"])
-
-    def get_users(self) -> pd.DataFrame:
-        """
-        Get all users
-
-        Returns
-        -------
-        users: pd.DataFrame
-
-        """
-        return pd.DataFrame(super().get_users())
-
-    def get_sources(
-        self,
-        manufacturer_id=None,
-        provider_key=None,
-        provider=None,
-        id=None,
-        **addl_kwargs,
-    ):
+    def get_subjectsources(self, subjects=None, sources=None, **addl_kwargs):
         """
         Parameters
         ----------
-        manufacturer_id
-        provider_key
-        provider
-        id
-
+        subjects: A comma-delimited list of Subject IDs.
+        sources: A comma-delimited list of Source IDs.
         Returns
         -------
-        sources : pd.DataFrame
-            DataFrame of queried sources
-
+        subjectsources : pd.DataFrame
         """
-
-        kwargs = self._clean_kwargs(
-            addl_kwargs,
-            manufacturer_id=manufacturer_id,
-            provider_key=provider_key,
-            provider=provider,
-            id=id,
+        params = self._clean_kwargs(addl_kwargs, sources=sources, subjects=subjects)
+        return pd.DataFrame(
+            self.get_objects_multithreaded(
+                object="subjectsources/", threads=self.tcp_limit, page_size=self.sub_page_size, **params
+            )
         )
 
-        return pd.DataFrame(self._get("sources/", params=kwargs)["results"])
-
     def _get_observations(
         self,
         source_ids=None,
         subject_ids=None,
         subjectsource_ids=None,
         tz="UTC",
         since=None,
@@ -342,119 +201,103 @@
         include_details=None,
         created_after=None,
         **addl_kwargs,
     ):
         """
         Return observations matching queries. If `subject_id`, `source_id`, or `subjectsource_id` is specified, the
         index is set to the provided value.
-
         Parameters
         ----------
-        subject_ids
-            filter to a single subject
-        source_ids
-            filter to a single source
-        subjectsource_ids
-            filter to a subjectsource_id, rather than source_id + time range
-        since
-            get observations after this ISO8061 date, include timezone
-        until
-            get observations up to this ISO8061 date, include timezone
+        subject_ids: filter to a single subject
+        source_ids: filter to a single source
+        subjectsource_ids: filter to a subjectsource_id, rather than source_id + time range
+        since: get observations after this ISO8061 date, include timezone
+        until:get observations up to this ISO8061 date, include timezone
         filter
             filter using exclusion_flags for an observation.
             filter=None returns everything
             filter=0  filters out everything but rows with exclusion flag 0 (i.e, passes back clean data)
             filter=1  filters out everything but rows with exclusion flag 1 (i.e, passes back manually filtered data)
             filter=2, filters out everything but rows with exclusion flag 2 (i.e., passes back automatically filtered
             data)
             filter=3, filters out everything but rows with exclusion flag 2 or 1 (i.e., passes back both manual and
             automatically filtered data)
-        include_details
-            one of [true,false], default is false. This brings back the observation additional field
-        created_after
-            get observations created (saved in EarthRanger) after this ISO8061 date, include timezone
-
+        include_details: one of [true,false], default is false. This brings back the observation additional field
+        created_after: get observations created (saved in EarthRanger) after this ISO8061 date, include timezone
         Returns
         -------
         observations : gpd.GeoDataFrame
-            GeoDataFrame of queried observations
-
         """
-
         assert (source_ids, subject_ids, subjectsource_ids).count(None) == 2
 
-        kwargs = self._clean_kwargs(
+        params = self._clean_kwargs(
             addl_kwargs,
             since=since,
             until=until,
             filter=filter,
             include_details=include_details,
             created_after=created_after,
         )
 
-        if source_ids is not None:
-            id_name = "source_id"
-            ids = source_ids
-        elif subject_ids is not None:
-            id_name = "subject_id"
-            ids = subject_ids
+        if source_ids:
+            id_name, ids = "source_id", source_ids
+        elif subject_ids:
+            id_name, ids = "subject_id", subject_ids
         else:
-            id_name = "subjectsource_id"
-            ids = subjectsource_ids
-
-        if isinstance(ids, str):
-            ids = [ids]
+            id_name, ids = "subjectsource_id", subjectsource_ids
 
         observations = []
-        pbar = tqdm(ids)
-        for id in pbar:
-            pbar.set_description(f"Downloading Observations for {id_name}={id}")
-            kwargs[id_name] = id
-            df = pd.DataFrame(self._get("observations/", params=kwargs)["results"])
-            df[id_name] = id
-            observations.append(df)
+        pbar = tqdm([ids] if isinstance(ids, str) else ids)
+
+        for _id in pbar:
+            params[id_name] = _id
+            pbar.set_description(f"Downloading Observations for {id_name}={_id}")
+            dataframe = pd.DataFrame(
+                self.get_objects_multithreaded(
+                    object="observations/", threads=self.tcp_limit, page_size=self.sub_page_size, **params
+                )
+            )
+            dataframe[id_name] = _id
+            observations.append(dataframe)
 
         observations = pd.concat(observations)
         if observations.empty:
             return gpd.GeoDataFrame()
 
         observations["created_at"] = pd.to_datetime(
             observations["created_at"],
             errors="coerce",
             utc=True,
         ).dt.tz_convert(tz)
+
         observations["recorded_at"] = pd.to_datetime(
             observations["recorded_at"],
             errors="coerce",
             utc=True,
         ).dt.tz_convert(tz)
 
         observations.sort_values("recorded_at", inplace=True)
-
         return EarthRangerIO._to_gdf(observations)
 
     def get_source_observations(self, source_ids, include_source_details=False, relocations=True, **kwargs):
         """
         Get observations for each listed source and create a `Relocations` object.
-
         Parameters
         ----------
         source_ids : str or list[str]
             List of source UUIDs
         include_source_details : bool, optional
             Whether to merge source info into dataframe
         kwargs
             Additional arguments to pass in the request to EarthRanger. See the docstring of `_get_observations` for
             info.
-
         Returns
         -------
         relocations : ecoscope.base.Relocations
             Observations in `Relocations` format
-
         """
 
         if isinstance(source_ids, str):
             source_ids = [source_ids]
 
         observations = self._get_observations(source_ids=source_ids, **kwargs)
         if observations.empty:
@@ -484,71 +327,67 @@
         include_subject_details=False,
         include_subjectsource_details=False,
         relocations=True,
         **kwargs,
     ):
         """
         Get observations for each listed subject and create a `Relocations` object.
-
         Parameters
         ----------
         subject_ids : str or list[str]
             List of subject UUIDs
         include_source_details : bool, optional
             Whether to merge source info into dataframe
         include_subject_details : bool, optional
             Whether to merge subject info into dataframe
         include_subjectsource_details : bool, optional
             Whether to merge subjectsource info into dataframe
         kwargs
             Additional arguments to pass in the request to EarthRanger. See the docstring of `__get_observations` for
             info.
-
         Returns
         -------
         relocations : ecoscope.base.Relocations
             Observations in `Relocations` format
-
         """
 
         if isinstance(subject_ids, str):
             subject_ids = [subject_ids]
 
         observations = self._get_observations(subject_ids=subject_ids, **kwargs)
 
         if observations.empty:
             return gpd.GeoDataFrame()
 
         if include_source_details:
             observations = observations.merge(
-                pd.DataFrame(self.get_sources(id=",".join(observations["source"].unique()))).add_prefix("source__"),
+                self.get_sources(id=",".join(observations["source"].unique())).add_prefix("source__"),
                 left_on="source",
                 right_on="source__id",
             )
-
         if include_subject_details:
             observations = observations.merge(
                 self.get_subjects(id=",".join(subject_ids), include_inactive=True).add_prefix("subject__"),
                 left_on="subject_id",
                 right_on="subject__id",
             )
 
         if include_subjectsource_details:
             observations = observations.merge(
                 self.get_subjectsources(subjects=",".join(observations["subject_id"].unique())).add_prefix(
                     "subjectsource__"
                 ),
-                left_on=["subject_id", "source"],
+                left_on=["id", "source"],
                 right_on=["subjectsource__subject", "subjectsource__source"],
             )
 
         if relocations:
             return ecoscope.base.Relocations.from_gdf(
                 observations,
-                groupby_col="subject_id",
+                groupby_col="id",
                 uuid_col="id",
                 time_col="recorded_at",
             )
         else:
             return observations
 
     def get_subjectsource_observations(
@@ -556,30 +395,27 @@
         subjectsource_ids,
         include_source_details=False,
         relocations=True,
         **kwargs,
     ):
         """
         Get observations for each listed subjectsource and create a `Relocations` object.
-
         Parameters
         ----------
         subjectsource_ids : str or list[str]
             List of subjectsource UUIDs
         include_source_details : bool, optional
             Whether to merge source info into dataframe
         kwargs
             Additional arguments to pass in the request to EarthRanger. See the docstring of `__get_observations` for
             info.
-
         Returns
         -------
         relocations : ecoscope.base.Relocations
             Observations in `Relocations` format
-
         """
 
         if isinstance(subjectsource_ids, str):
             subjectsource_ids = [subjectsource_ids]
 
         observations = self._get_observations(subjectsource_ids=subjectsource_ids, **kwargs)
 
@@ -599,164 +435,219 @@
                 groupby_col="subjectsource_id",
                 uuid_col="id",
                 time_col="recorded_at",
             )
         else:
             return observations
 
+    def get_subjectgroup_observations(self, subject_group=None, group_name=None, include_inactive=True, **kwargs):
+        """
+        Parameters
+        ----------
+        subject_group : str
+            UUID of subject group to filter by
+        group_name : str
+            Common name of subject group to filter by
+        include_inactive : bool, optional
+            Whether to get observations for Subjects marked inactive by EarthRanger
+        kwargs
+            Additional arguments to pass in the request to `get_subject_observations`. See the docstring of
+            `get_subject_observations` for info.
+        Returns
+        -------
+        relocations : ecoscope.base.Relocations
+            Observations in `Relocations` format
+        """
+
+        assert (subject_group is None) != (group_name is None)
+
+        if subject_group:
+            subject_ids = self.get_subjects(subject_group=subject_group, include_inactive=include_inactive).id.tolist()
+        else:
+            subject_ids = self.get_subjects(group_name=group_name, include_inactive=include_inactive).id.tolist()
+
+        return self.get_subject_observations(subject_ids, **kwargs)
+
     def get_events(
         self,
         is_collection=None,
         updated_size=None,
         event_ids=None,
         bbox=None,
-        include_updates=None,
-        include_details=None,
         sort_by=None,
         patrol_segment=None,
         state=None,
         event_type=None,
-        include_notes=None,
-        include_related_events=None,
-        include_files=None,
+        include_updates=False,
+        include_details=False,
+        include_notes=False,
+        include_related_events=False,
+        include_files=False,
         max_results=None,
         oldest_update_date=None,
         exclude_contained=None,
         updated_since=None,
         event_category=None,
-        filter=None,
+        since=None,
+        until=None,
         **addl_kwargs,
     ):
         """
         Parameters
         ----------
         is_collection
             true/false whether to filter on is_collection
         updated_since
             date-string to limit on updated_at
         event_ids : array[string]
             Event IDs, comma-separated
         bbox
             bounding box including four coordinate values, comma-separated. Ex. bbox=-122.4,48.4,-122.95,49.0
             (west, south, east, north).
-        include_updates
-            Boolean value
-        include_details
-            Boolean value
         sort_by
             Sort by (use 'event_time', 'updated_at', 'created_at', 'serial_number') with optional minus ('-') prefix to
             reverse order.
         patrol_segment
             ID of patrol segment to filter on
         state
             Comma-separated list of 'scheduled'/'active'/'overdue'/'done'/'cancelled'
         event_type
             Comma-separated list of event type uuids
+        include_updates
+            Boolean value
+        include_details
+            Boolean value
         include_notes
             Boolean value
         include_related_events
             Boolean value
         include_files
             Boolean value
         max_results
         oldest_update_date
         exclude_contained
         event_category
-        filter : json dict
-            Can contain any of 'event_filter_id', 'text', 'date_range', 'duration', 'state', 'priority',
-            'event_category', 'event_type', 'reported_by', 'create_date', 'update_date'
-
+        since
+        until
         Returns
         -------
         events : gpd.GeoDataFrame
             GeoDataFrame of queried events
-
         """
 
-        kwargs = self._clean_kwargs(
+        params = self._clean_kwargs(
             addl_kwargs,
             is_collection=is_collection,
             updated_size=updated_size,
             event_ids=event_ids,
             bbox=bbox,
-            include_updates=include_updates,
-            include_details=include_details,
             sort_by=sort_by,
             patrol_segment=patrol_segment,
             state=state,
             event_type=event_type,
+            include_updates=include_updates,
+            include_details=include_details,
             include_notes=include_notes,
             include_related_events=include_related_events,
             include_files=include_files,
             max_results=max_results,
             oldest_update_date=oldest_update_date,
             exclude_contained=exclude_contained,
             updated_since=updated_since,
             event_category=event_category,
-            filter=filter,
         )
 
-        df = pd.DataFrame(self._get("activity/events/", params=kwargs)["results"])
+        filter = {"date_range": {}}
+        if since is not None:
+            filter["date_range"]["lower"] = since
+            params["filter"] = json.dumps(filter)
+        if until is not None:
+            filter["date_range"]["upper"] = until
+            params["filter"] = json.dumps(filter)
+
+        df = pd.DataFrame(
+            self.get_objects_multithreaded(
+                object="activity/events/", threads=self.tcp_limit, page_size=self.sub_page_size, **params
+            )
+        )
+
         assert not df.empty
         df["time"] = pd.to_datetime(df["time"])
 
         df = gpd.GeoDataFrame(df)
         df.loc[~df["geojson"].isna(), "geometry"] = gpd.GeoDataFrame.from_features(
             df.loc[~df["geojson"].isna(), "geojson"]
         )["geometry"]
         df.set_crs(4326, inplace=True)
 
         df.sort_values("time", inplace=True)
         return df
 
-    def get_subjectgroup_observations(self, subject_group=None, group_name=None, include_inactive=True, **kwargs):
+    def get_patrols(self, since=None, until=None, patrol_type=None, status=None, **addl_kwargs):
         """
         Parameters
         ----------
-        subject_group : str
-            UUID of subject group to filter by
-        group_name : str
-            Common name of subject group to filter by
-        include_inactive : bool, optional
-            Whether to get observations for Subjects marked inactive by EarthRanger
-        kwargs
-            Additional arguments to pass in the request to `get_subject_observations`. See the docstring of
-            `get_subject_observations` for info.
-
+        since:
+            lower date range
+        until:
+            upper date range
+        patrol_type:
+            Comma-separated list of type of patrol UUID
+        status
+            Comma-separated list of 'scheduled'/'active'/'overdue'/'done'/'cancelled'
         Returns
         -------
-        relocations : ecoscope.base.Relocations
-            Observations in `Relocations` format
-
+        patrols : pd.DataFrame
+            DataFrame of queried patrols
         """
 
-        assert (subject_group is None) != (group_name is None)
+        params = self._clean_kwargs(
+            addl_kwargs,
+            status=status,
+            patrol_type=[patrol_type] if isinstance(patrol_type, str) else patrol_type,
+            return_data=True,
+        )
 
-        if subject_group:
-            subject_ids = self.get_subjects(subject_group=subject_group, include_inactive=include_inactive).id.tolist()
-        else:
-            subject_ids = self.get_subjects(group_name=group_name, include_inactive=include_inactive).id.tolist()
+        filter = {"date_range": {}, "patrol_type": []}
 
-        return self.get_subject_observations(subject_ids, **kwargs)
+        if since is not None:
+            filter["date_range"]["lower"] = since
+        if until is not None:
+            filter["date_range"]["upper"] = until
+        if patrol_type is not None:
+            filter["patrol_type"] = params["patrol_type"]
+        params["filter"] = json.dumps(filter)
+
+        df = pd.DataFrame(
+            self.get_objects_multithreaded(
+                object="activity/patrols", threads=self.tcp_limit, page_size=self.sub_page_size, **params
+            )
+        )
+        if "serial_number" in df.columns:
+            df = df.sort_values(by="serial_number").reset_index(drop=True)
+        return df
+
+    def get_patrol_segments(self):
+        object = "activity/patrols/segments/"
+        return pd.DataFrame(
+            self.get_objects_multithreaded(object=object, threads=self.tcp_limit, page_size=self.sub_page_size)
+        )
 
     def get_observations_for_patrols(self, patrols_df, **kwargs):
         """
         Download observations for provided `patrols_df`.
-
         Parameters
         ----------
         patrols_df : pd.DataFrame
             Data returned from a call to `get_patrols`.
         kwargs
             Additional parameters to pass to `get_subject_observations`.
-
         Returns
         -------
         relocations : ecoscope.base.Relocations
-
         """
 
         observations = []
         for _, patrol in patrols_df.iterrows():
             for patrol_segment in patrol["patrol_segments"]:
                 subject_id = (patrol_segment.get("leader") or {}).get("id")
                 start_time = (patrol_segment.get("time_range") or {}).get("start_time")
@@ -775,150 +666,352 @@
                     )
                 except Exception as e:
                     # print(f'Getting observations for {subject_id=} {start_time=} {end_time=} failed for: {e}')
                     print(
                         f"Getting observations for subject_id={subject_id} start_time={start_time} end_time={end_time}"
                         f"failed for: {e}"
                     )
+        return ecoscope.base.Relocations(pd.concat(observations))
+
+    def get_patrol_segment_events(
+        self,
+        patrol_segment_id=None,
+        include_details=False,
+        include_files=False,
+        include_related_events=False,
+        include_notes=False,
+        **addl_kwargs,
+    ):
+        params = self._clean_kwargs(
+            addl_kwargs,
+            patrol_segment_id=patrol_segment_id,
+            include_details=include_details,
+            include_files=include_files,
+            include_related_events=include_related_events,
+            include_notes=include_notes,
+        )
 
-        for i, patrol in patrols_df.iterrows():
-            pd.DataFrame(observations[i])["groupby_col"] = patrol["id"]
+        object = f"activity/patrols/segments/{patrol_segment_id}/events/"
+        return pd.DataFrame(
+            self.get_objects_multithreaded(
+                object=object, threads=self.tcp_limit, page_size=self.sub_page_size, **params
+            )
+        )
 
-        return ecoscope.base.Relocations(pd.concat(observations))
+    """
+    POST Functions
+    """
 
-    def post_observations(
+    def post_source(
         self,
-        observations: gpd.GeoDataFrame,
-        source_id_col: str = "source",
-        recorded_at_col: str = "recorded_at",
+        source_type: str,
+        manufacturer_id: str,
+        model_name: str,
+        provider: str = "default",
+        additional: typing.Dict = {},
+        **kwargs,
     ) -> pd.DataFrame:
         """
         Parameters
         ----------
-        observations : gpd.GeoDataFrame
-            observation data to be uploaded
-        source_id_col : str
-            The source column in the observation dataframe
-        recorded_at_col : str
-            The observation recorded time column in the dataframe
-
+        source_type
+        manufacturer_id
+        model_name
+        provider
+        additional
         Returns
         -------
-        None
+        pd.DataFrame
+        """
+
+        payload = {
+            "source_type": source_type,
+            "manufacturer_id": manufacturer_id,
+            "model_name": model_name,
+            "additional": additional,
+            "provider": provider,
+        }
 
+        if kwargs:
+            payload.update(kwargs)
+
+        response = self._post("sources", payload=payload)
+        return pd.DataFrame([response])
+
+    def post_subject(
+        self,
+        subject_name: str,
+        subject_type: str,
+        subject_subtype: str,
+        is_active: bool = True,
+        **kwargs,
+    ) -> pd.DataFrame:
         """
+        Parameters
+        ----------
+        subject_name
+        subject_subtype
+        is_active
 
-        def upload(obs):
-            try:
-                obs = obs.rename(columns={source_id_col: "source", recorded_at_col: "recorded_at"})
-                obs["location"] = pd.DataFrame({"longitude": obs.geometry.x, "latitude": obs.geometry.y}).to_dict(
-                    "records"
-                )
-                del obs["geometry"]
-                obs = pack_columns(obs, columns=["source", "recorded_at", "location"])
-                post_data = obs.to_dict("records")
-                results = super(EarthRangerIO, self).post_observation(post_data)
-            except DasClientException as exc:
-                self.logger.error(exc)
-            except requests.exceptions.RequestException as exc:
-                self.logger.error(exc)
-            else:
-                return pd.DataFrame(results)
+        Returns
+        -------
+        pd.DataFrame
+        """
+
+        payload = {
+            "name": subject_name,
+            "subject_subtype": subject_subtype,
+            "is_active": is_active,
+        }
 
-        return observations.groupby(source_id_col).progress_apply(upload)
+        if kwargs:
+            payload.update(kwargs)
+
+        response = self._post("subjects", payload=payload)
+        return pd.DataFrame([response])
 
     def post_subjectsource(
         self,
         subject_id: str,
         source_id: str,
-        lower_bound_assignend_range: datetime.datetime,
+        lower_bound_assigned_range: datetime.datetime,
         upper_bound_assigned_range: datetime.datetime,
         additional: typing.Dict = None,
     ) -> pd.DataFrame:
         """
         Parameters
         ----------
         subject_id
         source_id
-        lower_bound_assignend_range
+        lower_bound_assigned_range
         upper_bound_assigned_range
         additional
-
         Returns
         -------
         pd.DataFrame
-
         """
 
         if additional is None:
             additional = {}
         payload = {
             "source": source_id,
             "assigned_range": {
-                "lower": lower_bound_assignend_range,
+                "lower": lower_bound_assigned_range,
                 "upper": upper_bound_assigned_range,
             },
             "additional": additional,
         }
 
         urlpath = f"subject/{subject_id}/sources"
         response = self._post(urlpath, payload=payload)
         return pd.DataFrame([response])
 
-    @staticmethod
-    def _dataframe_to_dict(events):
-        if isinstance(events, gpd.GeoDataFrame):
-            events["location"] = pd.DataFrame({"longitude": events.geometry.x, "latitude": events.geometry.y}).to_dict(
-                "records"
-            )
-            del events["geometry"]
+    def post_observations(
+        self,
+        observations: gpd.GeoDataFrame,
+        source_id_col: str = "source",
+        recorded_at_col: str = "recorded_at",
+    ) -> pd.DataFrame:
+        """
+        Parameters
+        ----------
+        observations : gpd.GeoDataFrame
+            observation data to be uploaded
+        source_id_col : str
+            The source column in the observation dataframe
+        recorded_at_col : str
+            The observation recorded time column in the dataframe
+        Returns
+        -------
+        None
+        """
 
-        if isinstance(events, pd.DataFrame):
-            events = events.to_dict("records")
-        return events
+        def upload(obs):
+            try:
+                obs = obs.rename(columns={source_id_col: "source", recorded_at_col: "recorded_at"})
+                obs["location"] = pd.DataFrame({"longitude": obs.geometry.x, "latitude": obs.geometry.y}).to_dict(
+                    "records"
+                )
+                del obs["geometry"]
+                obs = pack_columns(obs, columns=["source", "recorded_at", "location"])
+                post_data = obs.to_dict("records")
+                results = super(EarthRangerIO, self).post_observation(post_data)
+            except ERClientException as exc:
+                self.logger.error(exc)
+            except requests.exceptions.RequestException as exc:
+                self.logger.error(exc)
+            else:
+                return pd.DataFrame(results)
+
+        return observations.groupby(source_id_col, group_keys=False).progress_apply(upload)
 
     def post_event(
         self,
         events: typing.Union[gpd.GeoDataFrame, pd.DataFrame, typing.Dict, typing.List[typing.Dict]],
     ) -> pd.DataFrame:
         """
         Parameters
         ----------
         events
-
         Returns
         -------
         pd.DataFrame:
             New events created in EarthRanger.
-
         """
 
         events = self._dataframe_to_dict(events)
         results = super().post_event(event=events)
         results = results if isinstance(results, list) else [results]
         return pd.DataFrame(results)
 
+    def post_patrol(self, priority: int, **kwargs) -> pd.DataFrame:
+        """
+        Parameters
+        ----------
+        priority
+
+        Returns
+        -------
+        pd.DataFrame
+        """
+        payload = {"priority": priority}
+
+        if kwargs:
+            payload.update(kwargs)
+
+        response = self._post("activity/patrols", payload=payload)
+        return pd.DataFrame([response])
+
+    def post_patrol_segment(
+        self,
+        patrol_id: str,
+        patrol_segment_id: str,
+        patrol_type: str = None,
+        tracked_subject_id: str = None,
+        scheduled_start: str = None,
+        scheduled_end: str = None,
+        start_time: str = None,
+        end_time: str = None,
+        start_location: typing.Tuple[float, float] = None,
+        end_location: typing.Tuple[float, float] = None,
+        **kwargs,
+    ) -> pd.DataFrame:
+        """
+        Parameters
+        ----------
+        patrol_id
+        patrol_segment_id
+        patrol_type
+        tracked_subject_id
+        scheduled_start
+        scheduled_end
+        start_time
+        end_time
+        start_location
+        end_location
+
+        Returns
+        -------
+        pd.DataFrame
+        """
+
+        payload = {
+            "patrol": patrol_id,
+            "patrol_segment": patrol_segment_id,
+            "scheduled_start": scheduled_start,
+            "scheduled_end": scheduled_end,
+            "time_range": {"start_time": start_time, "end_time": end_time},
+        }
+
+        if tracked_subject_id is not None:
+            payload.update({"leader": {"content_type": "observations.subject", "id": tracked_subject_id}})
+        else:
+            payload.update({"leader": None})
+
+        if start_location is not None:
+            payload.update({"start_location": {"latitude": start_location[0], "longitude": start_location[1]}})
+        else:
+            payload.update({"start_location": None})
+
+        if end_location is not None:
+            payload.update({"end_location": {"latitude": end_location[0], "longitude": end_location[1]}})
+        else:
+            payload.update({"end_location": None})
+
+        if patrol_type is not None:
+            payload.update({"patrol_type": patrol_type})
+
+        if kwargs:
+            payload.update(kwargs)
+
+        response = self._post("activity/patrols/segments/", payload=payload)
+        return pd.DataFrame([response])
+
+    def post_patrol_segment_event(
+        self,
+        patrol_segment_id: str,
+        event_type: str,
+        **addl_kwargs,
+    ) -> pd.DataFrame:
+        """
+        Parameters
+        ----------
+        patrol_segment_id
+        event_type
+
+        Returns
+        -------
+        pd.DataFrame
+        """
+
+        payload = {
+            "patrol_segment": patrol_segment_id,
+            "event_type": event_type,
+        }
+
+        if addl_kwargs:
+            payload.update(addl_kwargs)
+
+        response = self._post(f"activity/patrols/segments/{patrol_segment_id}/events/", payload=payload)
+        return pd.DataFrame([response])
+
+    """
+    PATCH Functions
+    """
+
     def patch_event(
         self,
         event_id: str,
         events: typing.Union[gpd.GeoDataFrame, pd.DataFrame, typing.Dict, typing.List[typing.Dict]],
     ) -> pd.DataFrame:
         """
         Parameters
         ----------
         event_id
             UUID for the event that will be updated.
         events
-
         Returns
         -------
         pd.DataFrame:
             Updated events in EarthRanger.
-
         """
 
         events = self._dataframe_to_dict(events)
         if isinstance(events, list):
             results = [self._patch(f"activity/event/{event_id}", payload=event) for event in events]
         else:
             results = [self._patch(f"activity/event/{event_id}", payload=events)]
         return pd.DataFrame(results)
+
+    """
+    DELETE Functions
+    """
+
+    def delete_observation(self, observation_id: str):
+        """
+        Parameters
+        ----------
+        observation_id
+        -------
+        """
+
+        self._delete("observation/" + observation_id + "/")
```

### Comparing `ecoscope-1.1.2/ecoscope/io/eetools.py` & `ecoscope-1.2.0/ecoscope/io/eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/io/raster.py` & `ecoscope-1.2.0/ecoscope/io/raster.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/io/utils.py` & `ecoscope-1.2.0/ecoscope/io/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/mapping/map.py` & `ecoscope-1.2.0/ecoscope/mapping/map.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope/plotting/plot.py` & `ecoscope-1.2.0/ecoscope/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/ecoscope.egg-info/PKG-INFO` & `ecoscope-1.2.0/ecoscope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.1.2
+Version: 1.2.0
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.1.2/ecoscope.egg-info/SOURCES.txt` & `ecoscope-1.2.0/ecoscope.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 ecoscope/analysis/UD/etd_range.py
 ecoscope/base/__init__.py
 ecoscope/base/_dataclasses.py
 ecoscope/base/base.py
 ecoscope/base/utils.py
 ecoscope/contrib/__init__.py
 ecoscope/contrib/basemaps.py
-ecoscope/contrib/dasclient.py
 ecoscope/contrib/foliumap.py
 ecoscope/contrib/legend.txt
 ecoscope/io/__init__.py
 ecoscope/io/earthranger.py
 ecoscope/io/eetools.py
 ecoscope/io/raster.py
 ecoscope/io/utils.py
```

### Comparing `ecoscope-1.1.2/pyproject.toml` & `ecoscope-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/setup.py` & `ecoscope-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "scikit-image",
     "scikit-learn",
     "scipy",
     "selenium",
     "shapely",
     "tqdm",
     "xyzservices",
+    "earthranger-client",
 ]
 
 setup(
     name="ecoscope",
     version=version_data["version"],
     description="Standard Analytical Reporting Framework for Conservation",
     long_description=descr,
```

### Comparing `ecoscope-1.1.2/tests/test_base.py` & `ecoscope-1.2.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/tests/test_earthranger_io.py` & `ecoscope-1.2.0/tests/test_earthranger_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,24 +26,14 @@
     )
     assert isinstance(relocations, ecoscope.base.Relocations)
     assert "groupby_col" in relocations
     assert "fixtime" in relocations
     assert "extra__source" in relocations
 
 
-def test_get_subject_no_observations(er_io):
-    with pytest.raises(ecoscope.contrib.dasclient.DasClientNotFound):
-        er_io.get_subject_observations(
-            subject_ids=str(uuid.uuid4()),
-            include_subject_details=True,
-            include_source_details=True,
-            include_subjectsource_details=True,
-        )
-
-
 def test_get_source_observations(er_io):
     relocations = er_io.get_source_observations(
         source_ids=er_io.SOURCE_IDS,
         include_source_details=True,
     )
     assert isinstance(relocations, ecoscope.base.Relocations)
     assert "fixtime" in relocations
@@ -72,32 +62,22 @@
     relocations = er_io.get_subjectsource_observations(
         subjectsource_ids=str(uuid.uuid4()),
         include_source_details=True,
     )
     assert relocations.empty
 
 
-def test_get_subjectsource_observations_with_pagesize_one(er_io):
-    relocations = er_io.get_subjectsource_observations(
-        subjectsource_ids=er_io.SUBJECTSOURCE_IDS[0],
-        include_source_details=True,
-        page_size=1,
-    )
-    assert isinstance(relocations, ecoscope.base.Relocations)
-    assert len(relocations) == 1
-
-
 def test_get_subjectgroup_observations(er_io):
     relocations = er_io.get_subjectgroup_observations(group_name=er_io.GROUP_NAME)
     assert "groupby_col" in relocations
 
 
 def test_get_events(er_io):
-    events = er_io.get_events(page_size=100)
-    assert len(events) <= 100
+    events = er_io.get_events()
+    assert not events.empty
 
 
 @pytest.mark.filterwarnings("ignore:All-NaN slice encountered:RuntimeWarning")
 @pytest.mark.filterwarnings("ignore:Mean of empty slice:RuntimeWarning")
 def test_collar_voltage(er_io):
     start_time = pytz.utc.localize(datetime.datetime.now() - datetime.timedelta(days=31))
     observations = er_io.get_subjectgroup_observations(
@@ -151,27 +131,27 @@
 def test_post_events(er_io):
     events = [
         {
             "id": str(uuid.uuid4()),
             "title": "Accident",
             "event_type": "accident_rep",
             "time": pd.Timestamp.utcnow(),
-            "location": {"longitude": "38.033294677734375", "latitude": "-2.9553841592697982"},
+            "location": {"latitude": -2.9553841592697982, "longitude": 38.033294677734375},
             "priority": 200,
             "state": "new",
             "event_details": {"type_accident": "head-on collision", "number_people_involved": 3, "animals_involved": 1},
             "is_collection": False,
             "icon_id": "accident_rep",
         },
         {
             "id": str(uuid.uuid4()),
             "title": "Accident",
             "event_type": "accident_rep",
             "time": pd.Timestamp.utcnow(),
-            "location": {"longitude": "38.4906005859375", "latitude": "-3.0321834919139206"},
+            "location": {"latitude": -3.0321834919139206, "longitude": 38.4906005859375},
             "priority": 300,
             "state": "active",
             "event_details": {
                 "type_accident": "side-impact collision",
                 "number_people_involved": 2,
                 "animals_involved": 1,
             },
@@ -190,37 +170,37 @@
 def test_patch_event(er_io):
     event = [
         {
             "id": str(uuid.uuid4()),
             "title": "Arrest",
             "event_type": "arrest_rep",
             "time": pd.Timestamp.utcnow(),
-            "location": {"longitude": 38.11809539794921, "latitude": -3.4017015747197306},
+            "location": {"latitude": -3.4017015747197306, "longitude": 38.11809539794921},
             "priority": 200,
             "state": "new",
             "event_details": {
                 "arrestrep_dateofbirth": "1985-01-1T13:00:00.000Z",
                 "arrestrep_nationality": "other",
                 "arrestrep_timeofarrest": datetime.datetime.utcnow().isoformat(),
                 "arrestrep_reaonforarrest": "firearm",
-                "arrestrep_arrestingranger": "Ranger Siera",
+                "arrestrep_arrestingranger": "catherine's cellphone",
             },
             "is_collection": False,
             "icon_id": "arrest_rep",
         }
     ]
     er_io.post_event(event)
     event_id = event[0]["id"]
 
     updated_event = pd.DataFrame(
         [
             {
                 "priority": 300,
                 "state": "active",
-                "location": {"longitude": "38.4576416015625", "latitude": "-4.135503657998179"},
+                "location": {"latitude": -4.135503657998179, "longitude": 38.4576416015625},
             }
         ]
     )
 
     result = er_io.patch_event(event_id=event_id, events=updated_event)
     result = result[["priority", "state", "location"]]
     pd.testing.assert_frame_equal(result, updated_event)
@@ -234,9 +214,9 @@
         include_subject_details=False,
         include_subjectsource_details=False,
     )
     assert not observations.empty
 
 
 def test_users(er_io):
-    users = er_io.get_users()
+    users = pd.DataFrame(er_io.get_users())
     assert not users.empty
```

### Comparing `ecoscope-1.1.2/tests/test_ecodataframe.py` & `ecoscope-1.2.0/tests/test_ecodataframe.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/tests/test_ecograph.py` & `ecoscope-1.2.0/tests/test_ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/tests/test_eetools.py` & `ecoscope-1.2.0/tests/test_eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/tests/test_geofence.py` & `ecoscope-1.2.0/tests/test_geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/tests/test_immobility.py` & `ecoscope-1.2.0/tests/test_immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/tests/test_seasons.py` & `ecoscope-1.2.0/tests/test_seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.1.2/tests/test_ud.py` & `ecoscope-1.2.0/tests/test_ud.py`

 * *Files identical despite different names*

