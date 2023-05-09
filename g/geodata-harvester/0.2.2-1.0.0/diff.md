# Comparing `tmp/geodata-harvester-0.2.2.tar.gz` & `tmp/geodata-harvester-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodata-harvester-0.2.2.tar", last modified: Thu Feb 16 02:56:45 2023, max compression
+gzip compressed data, was "geodata-harvester-1.0.0.tar", last modified: Tue May  9 03:44:35 2023, max compression
```

## Comparing `geodata-harvester-0.2.2.tar` & `geodata-harvester-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-02-16 02:56:45.529652 geodata-harvester-0.2.2/
--rw-r--r--   0 seb        (504) staff       (20)     7652 2023-01-10 23:44:41.000000 geodata-harvester-0.2.2/LICENSE.txt
--rw-r--r--   0 seb        (504) staff       (20)    10578 2023-02-16 02:56:45.529448 geodata-harvester-0.2.2/PKG-INFO
--rw-r--r--   0 seb        (504) staff       (20)    10164 2023-02-15 23:37:25.000000 geodata-harvester-0.2.2/README.md
--rw-r--r--   0 seb        (504) staff       (20)       38 2023-02-16 02:56:45.529692 geodata-harvester-0.2.2/setup.cfg
--rw-r--r--   0 seb        (504) staff       (20)     1981 2023-02-16 02:44:15.000000 geodata-harvester-0.2.2/setup.py
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-02-16 02:56:45.523841 geodata-harvester-0.2.2/src/
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-02-16 02:56:45.526848 geodata-harvester-0.2.2/src/geodata_harvester/
--rw-r--r--   0 seb        (504) staff       (20)     1030 2023-02-16 02:44:26.000000 geodata-harvester-0.2.2/src/geodata_harvester/__init__.py
--rw-r--r--   0 seb        (504) staff       (20)     1040 2022-03-23 04:23:00.000000 geodata-harvester-0.2.2/src/geodata_harvester/arc2meter.py
--rw-r--r--   0 seb        (504) staff       (20)    35525 2023-01-23 03:29:23.000000 geodata-harvester-0.2.2/src/geodata_harvester/getdata_dea.py
--rw-r--r--   0 seb        (504) staff       (20)    10787 2023-01-18 01:59:45.000000 geodata-harvester-0.2.2/src/geodata_harvester/getdata_dem.py
--rw-r--r--   0 seb        (504) staff       (20)     8655 2023-01-18 01:54:54.000000 geodata-harvester-0.2.2/src/geodata_harvester/getdata_landscape.py
--rw-r--r--   0 seb        (504) staff       (20)    11275 2023-01-18 01:55:09.000000 geodata-harvester-0.2.2/src/geodata_harvester/getdata_radiometric.py
--rw-r--r--   0 seb        (504) staff       (20)    19313 2023-01-18 02:20:25.000000 geodata-harvester-0.2.2/src/geodata_harvester/getdata_silo.py
--rw-r--r--   0 seb        (504) staff       (20)    15851 2023-02-06 06:20:02.000000 geodata-harvester-0.2.2/src/geodata_harvester/getdata_slga.py
--rw-r--r--   0 seb        (504) staff       (20)    13374 2023-02-14 04:30:58.000000 geodata-harvester-0.2.2/src/geodata_harvester/harvest.py
--rw-r--r--   0 seb        (504) staff       (20)      738 2023-01-15 23:19:22.000000 geodata-harvester-0.2.2/src/geodata_harvester/settingshandler.py
--rw-r--r--   0 seb        (504) staff       (20)     6228 2023-01-27 00:29:41.000000 geodata-harvester-0.2.2/src/geodata_harvester/spatial.py
--rw-r--r--   0 seb        (504) staff       (20)     8815 2022-11-29 22:57:00.000000 geodata-harvester-0.2.2/src/geodata_harvester/temporal.py
--rw-r--r--   0 seb        (504) staff       (20)    26437 2023-02-14 00:30:47.000000 geodata-harvester-0.2.2/src/geodata_harvester/utils.py
--rw-r--r--   0 seb        (504) staff       (20)    11604 2023-01-18 02:18:57.000000 geodata-harvester-0.2.2/src/geodata_harvester/validate_settings.py
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-02-16 02:56:45.528453 geodata-harvester-0.2.2/src/geodata_harvester/widgets/
--rw-rw-r--   0 seb        (504) staff       (20)       40 2016-10-31 16:56:29.000000 geodata-harvester-0.2.2/src/geodata_harvester/widgets/__init__.py
--rw-r--r--   0 seb        (504) staff       (20)    25214 2023-02-16 02:40:52.000000 geodata-harvester-0.2.2/src/geodata_harvester/widgets/harvesterwidgets.py
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-02-16 02:56:45.529232 geodata-harvester-0.2.2/src/geodata_harvester/widgets/ipyfilechooser/
--rwxr-xr-x   0 seb        (504) staff       (20)       60 2021-09-15 22:24:00.000000 geodata-harvester-0.2.2/src/geodata_harvester/widgets/ipyfilechooser/__init__.py
--rw-rw-r--   0 seb        (504) staff       (20)     1056 2021-09-15 22:24:00.000000 geodata-harvester-0.2.2/src/geodata_harvester/widgets/ipyfilechooser/errors.py
--rw-rw-r--   0 seb        (504) staff       (20)    22928 2022-06-09 00:48:28.000000 geodata-harvester-0.2.2/src/geodata_harvester/widgets/ipyfilechooser/filechooser.py
--rw-rw-r--   0 seb        (504) staff       (20)     3976 2021-09-15 22:24:00.000000 geodata-harvester-0.2.2/src/geodata_harvester/widgets/ipyfilechooser/utils.py
--rw-rw-r--   0 seb        (504) staff       (20)     1996 2016-10-31 16:56:29.000000 geodata-harvester-0.2.2/src/geodata_harvester/widgets/ipywidgets_file_selector.py
--rw-r--r--   0 seb        (504) staff       (20)     3703 2022-07-14 05:17:29.000000 geodata-harvester-0.2.2/src/geodata_harvester/write_logs.py
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-02-16 02:56:45.527708 geodata-harvester-0.2.2/src/geodata_harvester.egg-info/
--rw-r--r--   0 seb        (504) staff       (20)    10578 2023-02-16 02:56:45.000000 geodata-harvester-0.2.2/src/geodata_harvester.egg-info/PKG-INFO
--rw-r--r--   0 seb        (504) staff       (20)     1188 2023-02-16 02:56:45.000000 geodata-harvester-0.2.2/src/geodata_harvester.egg-info/SOURCES.txt
--rw-r--r--   0 seb        (504) staff       (20)        1 2023-02-16 02:56:45.000000 geodata-harvester-0.2.2/src/geodata_harvester.egg-info/dependency_links.txt
--rw-r--r--   0 seb        (504) staff       (20)      217 2023-02-16 02:56:45.000000 geodata-harvester-0.2.2/src/geodata_harvester.egg-info/requires.txt
--rw-r--r--   0 seb        (504) staff       (20)       18 2023-02-16 02:56:45.000000 geodata-harvester-0.2.2/src/geodata_harvester.egg-info/top_level.txt
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-09 03:44:35.031032 geodata-harvester-1.0.0/
+-rw-r--r--   0 seb        (504) staff       (20)     7652 2023-01-10 23:44:41.000000 geodata-harvester-1.0.0/LICENSE.txt
+-rw-r--r--   0 seb        (504) staff       (20)    12715 2023-05-09 03:44:35.030834 geodata-harvester-1.0.0/PKG-INFO
+-rw-r--r--   0 seb        (504) staff       (20)    12301 2023-05-09 03:40:12.000000 geodata-harvester-1.0.0/README.md
+-rw-r--r--   0 seb        (504) staff       (20)       38 2023-05-09 03:44:35.031084 geodata-harvester-1.0.0/setup.cfg
+-rw-r--r--   0 seb        (504) staff       (20)     1981 2023-05-09 03:28:52.000000 geodata-harvester-1.0.0/setup.py
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-09 03:44:35.026524 geodata-harvester-1.0.0/src/
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-09 03:44:35.029114 geodata-harvester-1.0.0/src/geodata_harvester/
+-rw-r--r--   0 seb        (504) staff       (20)     1030 2023-05-09 03:28:44.000000 geodata-harvester-1.0.0/src/geodata_harvester/__init__.py
+-rw-r--r--   0 seb        (504) staff       (20)     1040 2022-03-23 04:23:00.000000 geodata-harvester-1.0.0/src/geodata_harvester/arc2meter.py
+-rw-r--r--   0 seb        (504) staff       (20)    35525 2023-01-23 03:29:23.000000 geodata-harvester-1.0.0/src/geodata_harvester/getdata_dea.py
+-rw-r--r--   0 seb        (504) staff       (20)    10787 2023-01-18 01:59:45.000000 geodata-harvester-1.0.0/src/geodata_harvester/getdata_dem.py
+-rw-r--r--   0 seb        (504) staff       (20)     8655 2023-01-18 01:54:54.000000 geodata-harvester-1.0.0/src/geodata_harvester/getdata_landscape.py
+-rw-r--r--   0 seb        (504) staff       (20)    11275 2023-01-18 01:55:09.000000 geodata-harvester-1.0.0/src/geodata_harvester/getdata_radiometric.py
+-rw-r--r--   0 seb        (504) staff       (20)    18323 2023-05-08 08:11:38.000000 geodata-harvester-1.0.0/src/geodata_harvester/getdata_silo.py
+-rw-r--r--   0 seb        (504) staff       (20)    15851 2023-02-06 06:20:02.000000 geodata-harvester-1.0.0/src/geodata_harvester/getdata_slga.py
+-rw-r--r--   0 seb        (504) staff       (20)    23169 2023-05-09 01:43:38.000000 geodata-harvester-1.0.0/src/geodata_harvester/harvest.py
+-rw-r--r--   0 seb        (504) staff       (20)      738 2023-01-15 23:19:22.000000 geodata-harvester-1.0.0/src/geodata_harvester/settingshandler.py
+-rw-r--r--   0 seb        (504) staff       (20)     6228 2023-01-27 00:29:41.000000 geodata-harvester-1.0.0/src/geodata_harvester/spatial.py
+-rw-r--r--   0 seb        (504) staff       (20)    12970 2023-05-08 08:12:08.000000 geodata-harvester-1.0.0/src/geodata_harvester/temporal.py
+-rw-r--r--   0 seb        (504) staff       (20)    30584 2023-05-09 01:49:21.000000 geodata-harvester-1.0.0/src/geodata_harvester/utils.py
+-rw-r--r--   0 seb        (504) staff       (20)    11604 2023-01-18 02:18:57.000000 geodata-harvester-1.0.0/src/geodata_harvester/validate_settings.py
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-09 03:44:35.030120 geodata-harvester-1.0.0/src/geodata_harvester/widgets/
+-rw-rw-r--   0 seb        (504) staff       (20)       40 2016-10-31 16:56:29.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/__init__.py
+-rw-r--r--   0 seb        (504) staff       (20)    25214 2023-02-16 02:40:52.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/harvesterwidgets.py
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-09 03:44:35.030642 geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/
+-rwxr-xr-x   0 seb        (504) staff       (20)       60 2021-09-15 22:24:00.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/__init__.py
+-rw-rw-r--   0 seb        (504) staff       (20)     1056 2021-09-15 22:24:00.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/errors.py
+-rw-rw-r--   0 seb        (504) staff       (20)    22928 2022-06-09 00:48:28.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/filechooser.py
+-rw-rw-r--   0 seb        (504) staff       (20)     3976 2021-09-15 22:24:00.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/utils.py
+-rw-rw-r--   0 seb        (504) staff       (20)     1996 2016-10-31 16:56:29.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipywidgets_file_selector.py
+-rw-r--r--   0 seb        (504) staff       (20)     3703 2022-07-14 05:17:29.000000 geodata-harvester-1.0.0/src/geodata_harvester/write_logs.py
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-09 03:44:35.029724 geodata-harvester-1.0.0/src/geodata_harvester.egg-info/
+-rw-r--r--   0 seb        (504) staff       (20)    12715 2023-05-09 03:44:34.000000 geodata-harvester-1.0.0/src/geodata_harvester.egg-info/PKG-INFO
+-rw-r--r--   0 seb        (504) staff       (20)     1188 2023-05-09 03:44:34.000000 geodata-harvester-1.0.0/src/geodata_harvester.egg-info/SOURCES.txt
+-rw-r--r--   0 seb        (504) staff       (20)        1 2023-05-09 03:44:34.000000 geodata-harvester-1.0.0/src/geodata_harvester.egg-info/dependency_links.txt
+-rw-r--r--   0 seb        (504) staff       (20)      217 2023-05-09 03:44:34.000000 geodata-harvester-1.0.0/src/geodata_harvester.egg-info/requires.txt
+-rw-r--r--   0 seb        (504) staff       (20)       18 2023-05-09 03:44:34.000000 geodata-harvester-1.0.0/src/geodata_harvester.egg-info/top_level.txt
```

### Comparing `geodata-harvester-0.2.2/LICENSE.txt` & `geodata-harvester-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/PKG-INFO` & `geodata-harvester-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 Metadata-Version: 2.1
 Name: geodata-harvester
-Version: 0.2.2
+Version: 1.0.0
 Summary: An automation tool for harvesting and processing geodata from the web
 Home-page: https://github.com/Sydney-Informatics-Hub/geodata-harvester
 License: LGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Geodata-Harvester
 
-<h3><em>Automate geodata harvesting from the web and jumpstart your analysis with a ready-made set of spatial-temporal processed maps and dataframes.</em></h3> 
+<h3><em>Automate geodata harvesting from the web and jumpstart your analysis with a ready-made set of spatiotemporal processed maps and data tables.</em></h3> 
 
 <center><a><img src="quarto/images/dataharvester_logo.png" alt="Geodata-Harvester logo" width="100%"/></a></center>
 
 
 <!-- Badges  start -->
 
 [![License](https://img.shields.io/badge/License-LGPL3-blue)](#license)
-
-<!-- [![GitHub tag](https://img.shields.io/github/tag/Sydney-Informatics-Hub/AgReFed-DataHarvester?include_prereleases=&sort=semver&color=blue)](https://github.com/Sydney-Informatics-Hub/AgReFed-DataHarvester/releases/)
-[![issues - AgReFed-DataHarvester](https://img.shields.io/github/issues/Sydney-Informatics-Hub/AgReFed-DataHarvester)](https://github.com/Sydney-Informatics-Hub/AgReFed-DataHarvester/issues) -->
+[![PyPI-Server](https://img.shields.io/pypi/v/geodata-harvester.svg)](https://pypi.org/project/geodata-harvester/)
+[![Conda
+Version](https://img.shields.io/conda/vn/conda-forge/geodata-harvester.svg)](https://anaconda.org/conda-forge/geodata-harvester)
+[![Monthly Downloads](https://pepy.tech/badge/geodata-harvester/month)](https://pepy.tech/project/geodata-harvester)
 
 <!-- Badges end -->
 
 The Geodata-Harvester Python package offers reusable and automated workflows for data extraction from a wide range of geospatial and environmental data sources. User provided data is auto-completed with a suitable set of spatial- and temporal-aligned covariates as a ready-made dataset for machine learning and environmental models. In addition, all requested data layer maps are automatically extracted and aligned for a specific region and time period.
 
 For the R-package wrapper of the Geodata-Harvester, please visit the [Github dataharvesteR project](https://github.com/Sydney-Informatics-Hub/dataharvester).
 
 ## Content
 
 - [Introduction](#introduction)
 - [Data Sources](#data-sources)
 - [Functionality](#functionality)
 - [Key Features](#key-features)
 - [Installation](#installation)
+    - [Conda or Mamba](#conda-or-mamba)
+    - [PyPI](#pypi)
+    - [Google Earth Engine extension](#google-earth-engine-extension)
+    - [Local development](#local-development)
+    - [Workshop Cloud Sandbox](#workshop-cloud-sandbox)
 - [How to get started](#how-to-get-started)
 - [How to add new data source modules](#how-to-add-new-data-source-modules)
+- [Code reference API](#code-reference-api)
 - [Contributions](#contributions)
 - [Attribution and Acknowledgments](#attribution-and-acknowledgments)
 - [License](#license)
 
 
 ## Introduction
 
@@ -74,70 +81,91 @@
 
 Geodata-Harvester is designed as a modular and maintainable project in the form of a multi-stage pipeline by providing explicit boundaries among tasks. To encourage interaction and experimentation with the pipeline, multiple frontend notebooks and use case scenarios are provided.
 
 ## Key Features
 
 Below is a list of features available for the geodata-harvester package. Please check the project Github webpage and notebooks for examples, data selection, and other settings.
 
-- enabling reproducible workflows via YAML settings files
-- automatic data retrieval from geodata APIs for given locations and dates
-- automatic download and spatial-temporal processing of geo-spatial maps for user-specified bounding box, resolution, and time-scale.
-- support for multiple temporal aggregation options and spatial-temporal buffer
-- automatic extraction of retrieved data into ready-made dataframes for ML training
-- automatic generation of ready-made aligned maps and data for ML prediction models
-- visualisation of downloaded and aligned maps
-- support for saving and loading settings via interactive widgets
-- with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices
+- enabling reproducible workflows via YAML settings files.
+- automatic data retrieval from geodata APIs for given locations and dates.
+- automatic download and spatiotemporal processing of geo-spatial maps for user-specified bounding box, resolution, and time-scale.
+- support for time-series data extraction for multiple time slices. 
+- automatic extraction of retrieved data into ready-made dataframes for ML training.
+- automatic generation of ready-made aligned maps in GeoTiff format.
+- preview of downloaded and aligned maps.
+- support for saving and loading settings via interactive widgets.
+- with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices.
+- example notebooks and use-cases are provided for the user to get started.
 
 For more features, please see the [API reference documentation](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
 
 ## Installation
 
 Geodata-Harvester can be run on cloud-servers (e.g., in JupyterHub environment) or on your local machine. 
-Example notebooks for importing and using the package can be found in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks). To install the package run one of the following
+Example notebooks for importing and using the package can be found in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks). The package can be installed via PyPI or Conda:
 
-### Conda or Mamba install
+### Conda or Mamba
 
 The package geodata-harvester is available via the conda-forge channel:
 
 ```bash
 conda install geodata-harvester -c conda-forge
 ```
 
 Note that the geodata-harvester is imported with underscore as 
 
 ```Python
 import geodata_harvester
 ```
 
-### Pip install
+### PyPI
 
-Installation via pypi requires a pre-installation of gdal (see, e.g., [pypi.org/project/GDAL/installation guide](https://pypi.org/project/GDAL/)) in your environment. Once gdal is installed, you can install geodata-harvester via
+Installation via PyPI requires a pre-installation of gdal (see, e.g., [pypi.org/project/GDAL/installation guide](https://pypi.org/project/GDAL/)) in your environment. Once gdal is installed, you can install geodata-harvester via
 
 ```bash
 pip install geodata-harvester
 ```
 The geodata-harvester library can then be imported via
 
 ```Python
 import geodata_harvester
 ```
 
-### Requirements
+### Google Earth Engine extension
+
+Optionally you can include Google Earth Engine (GEE) data in Geodata-Harvester (see [Settings_Overview](quarto/docs/Settings_Overview.md)).
+GEE requires a Google account and a GEE authorization. If this is your first time using GEE, please follow [these instructions](https://earthengine.google.com/signup/) and authorise Geodata-Harvester to use the Google Earth Engine API. See a preview of the process [here](https://sydney-informatics-hub.github.io/AgReFed-Workshop/pydocs/setup-gee.html#part-ii-authorising-your-workstation-with-gee).
+
+NOTE: You only have to perform this authorisation ONCE. Or at least you only have to do it once per “connection” or if you use an incognito window.  
+
+
+### Local development
+
+If you like to develop Data Harvester locally, it is recommended to setup a virtual environment for the installation, e.g., via conda miniforge (see for dependencies `environment.yaml`) and to fork the Geodata-harvester repo. To install only the latest development version use:
+
+```bash
+pip install git+https://github.com/Sydney-Informatics-Hub/geodata-harvester
+```
+
+### Workshop Cloud Sandbox
+
+As play-ground for workshop training sessions and testing of the Geodata-Harvester we provide a pre-installed cloud Python Jupyterlab environment, which does not require any local installation. For login instructions and how to access the sandbox, please visit our [Python workshop page](https://sydney-informatics-hub.github.io/AgReFed-Workshop/pydocs/py00-workshop.html).
 
-If you like to develop Data Harvester locally, it is recommended to setup a virtual environment for the installation, e.g., via conda miniforge (see for dependencies `environment.yaml`).
+The Jupyter environment is hosted on the ARDC Nectar Research Cloud in partnership with AgReFed and Australian Research Data Commons (ARDC). Note that this sandbox is currently hosted for test purposes only and generated data is not permanently stored.
+
+The Geodata-Harvester can be easily installed also on other cloud services (e.g., Google Colab, Azure Notebooks).
 
 
 ## How to get started
 
 You may now invoke the geodata-harvester directly from a python terminal with:
 
 ```python
-import geodata_harvester as gh
-gh.harvest.run(PATH_TO_SETTINGS_YAMLFILE)
+import geodata_harvester as gdh
+gdh.harvest.run(PATH_TO_SETTINGS_YAMLFILE)
 ```
 
 **Note the subtle but important difference in use of an underscore `_` to import the package and the use of a dash `-` to install it!**
 
 To get started, some example workflows are provided as Jupyter notebooks:
 
 1. Options and user settings are defined by the user in the settings; see for settings documentation [Settings_Overview](quarto/docs/Settings_Overview.md)
@@ -149,14 +177,18 @@
 ## How to add new data source modules
 
 The Geodata-Harvester is designed to be extendable and new data source modules can be added as Python modules (for examples, see `getdata_*.py` modules). If you would like to add a new data source, please follow the [adding new data source guidelines](quarto/docs/How_to_add_DataSources.md)  
 
 We recommend to fork the geodata-harvester repo and develop new modules in a local environment. If you would like to contribute your data source module to the geodata-harvester package, please visit the [geodata-harvester contribution guidelines](quarto/docs/Contributing.md).
 
 
+## Code reference API
+
+An auto-generated API reference documentation is available [here](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
+
 ## Contributions
 We are happy for any contribution to the geodata-harvester, whether feedbacks and bug reports via github Issues, adding use-case examples via notebook contributions, to improving source-code and adding new or updating existing data source modules. 
 
 For more details about about how to contribute to the development, please visit the [Geodata-Harvester contribution guidelines](quarto/docs/Contributing.md).
 
 
 ## Attribution and Acknowledgments
```

### Comparing `geodata-harvester-0.2.2/README.md` & `geodata-harvester-1.0.0/src/geodata_harvester.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,55 @@
+Metadata-Version: 2.1
+Name: geodata-harvester
+Version: 1.0.0
+Summary: An automation tool for harvesting and processing geodata from the web
+Home-page: https://github.com/Sydney-Informatics-Hub/geodata-harvester
+License: LGPL-3.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Geodata-Harvester
 
-<h3><em>Automate geodata harvesting from the web and jumpstart your analysis with a ready-made set of spatial-temporal processed maps and dataframes.</em></h3> 
+<h3><em>Automate geodata harvesting from the web and jumpstart your analysis with a ready-made set of spatiotemporal processed maps and data tables.</em></h3> 
 
 <center><a><img src="quarto/images/dataharvester_logo.png" alt="Geodata-Harvester logo" width="100%"/></a></center>
 
 
 <!-- Badges  start -->
 
 [![License](https://img.shields.io/badge/License-LGPL3-blue)](#license)
-
-<!-- [![GitHub tag](https://img.shields.io/github/tag/Sydney-Informatics-Hub/AgReFed-DataHarvester?include_prereleases=&sort=semver&color=blue)](https://github.com/Sydney-Informatics-Hub/AgReFed-DataHarvester/releases/)
-[![issues - AgReFed-DataHarvester](https://img.shields.io/github/issues/Sydney-Informatics-Hub/AgReFed-DataHarvester)](https://github.com/Sydney-Informatics-Hub/AgReFed-DataHarvester/issues) -->
+[![PyPI-Server](https://img.shields.io/pypi/v/geodata-harvester.svg)](https://pypi.org/project/geodata-harvester/)
+[![Conda
+Version](https://img.shields.io/conda/vn/conda-forge/geodata-harvester.svg)](https://anaconda.org/conda-forge/geodata-harvester)
+[![Monthly Downloads](https://pepy.tech/badge/geodata-harvester/month)](https://pepy.tech/project/geodata-harvester)
 
 <!-- Badges end -->
 
 The Geodata-Harvester Python package offers reusable and automated workflows for data extraction from a wide range of geospatial and environmental data sources. User provided data is auto-completed with a suitable set of spatial- and temporal-aligned covariates as a ready-made dataset for machine learning and environmental models. In addition, all requested data layer maps are automatically extracted and aligned for a specific region and time period.
 
 For the R-package wrapper of the Geodata-Harvester, please visit the [Github dataharvesteR project](https://github.com/Sydney-Informatics-Hub/dataharvester).
 
 ## Content
 
 - [Introduction](#introduction)
 - [Data Sources](#data-sources)
 - [Functionality](#functionality)
 - [Key Features](#key-features)
 - [Installation](#installation)
+    - [Conda or Mamba](#conda-or-mamba)
+    - [PyPI](#pypi)
+    - [Google Earth Engine extension](#google-earth-engine-extension)
+    - [Local development](#local-development)
+    - [Workshop Cloud Sandbox](#workshop-cloud-sandbox)
 - [How to get started](#how-to-get-started)
 - [How to add new data source modules](#how-to-add-new-data-source-modules)
+- [Code reference API](#code-reference-api)
 - [Contributions](#contributions)
 - [Attribution and Acknowledgments](#attribution-and-acknowledgments)
 - [License](#license)
 
 
 ## Introduction
 
@@ -62,70 +81,91 @@
 
 Geodata-Harvester is designed as a modular and maintainable project in the form of a multi-stage pipeline by providing explicit boundaries among tasks. To encourage interaction and experimentation with the pipeline, multiple frontend notebooks and use case scenarios are provided.
 
 ## Key Features
 
 Below is a list of features available for the geodata-harvester package. Please check the project Github webpage and notebooks for examples, data selection, and other settings.
 
-- enabling reproducible workflows via YAML settings files
-- automatic data retrieval from geodata APIs for given locations and dates
-- automatic download and spatial-temporal processing of geo-spatial maps for user-specified bounding box, resolution, and time-scale.
-- support for multiple temporal aggregation options and spatial-temporal buffer
-- automatic extraction of retrieved data into ready-made dataframes for ML training
-- automatic generation of ready-made aligned maps and data for ML prediction models
-- visualisation of downloaded and aligned maps
-- support for saving and loading settings via interactive widgets
-- with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices
+- enabling reproducible workflows via YAML settings files.
+- automatic data retrieval from geodata APIs for given locations and dates.
+- automatic download and spatiotemporal processing of geo-spatial maps for user-specified bounding box, resolution, and time-scale.
+- support for time-series data extraction for multiple time slices. 
+- automatic extraction of retrieved data into ready-made dataframes for ML training.
+- automatic generation of ready-made aligned maps in GeoTiff format.
+- preview of downloaded and aligned maps.
+- support for saving and loading settings via interactive widgets.
+- with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices.
+- example notebooks and use-cases are provided for the user to get started.
 
 For more features, please see the [API reference documentation](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
 
 ## Installation
 
 Geodata-Harvester can be run on cloud-servers (e.g., in JupyterHub environment) or on your local machine. 
-Example notebooks for importing and using the package can be found in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks). To install the package run one of the following
+Example notebooks for importing and using the package can be found in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks). The package can be installed via PyPI or Conda:
 
-### Conda or Mamba install
+### Conda or Mamba
 
 The package geodata-harvester is available via the conda-forge channel:
 
 ```bash
 conda install geodata-harvester -c conda-forge
 ```
 
 Note that the geodata-harvester is imported with underscore as 
 
 ```Python
 import geodata_harvester
 ```
 
-### Pip install
+### PyPI
 
-Installation via pypi requires a pre-installation of gdal (see, e.g., [pypi.org/project/GDAL/installation guide](https://pypi.org/project/GDAL/)) in your environment. Once gdal is installed, you can install geodata-harvester via
+Installation via PyPI requires a pre-installation of gdal (see, e.g., [pypi.org/project/GDAL/installation guide](https://pypi.org/project/GDAL/)) in your environment. Once gdal is installed, you can install geodata-harvester via
 
 ```bash
 pip install geodata-harvester
 ```
 The geodata-harvester library can then be imported via
 
 ```Python
 import geodata_harvester
 ```
 
-### Requirements
+### Google Earth Engine extension
+
+Optionally you can include Google Earth Engine (GEE) data in Geodata-Harvester (see [Settings_Overview](quarto/docs/Settings_Overview.md)).
+GEE requires a Google account and a GEE authorization. If this is your first time using GEE, please follow [these instructions](https://earthengine.google.com/signup/) and authorise Geodata-Harvester to use the Google Earth Engine API. See a preview of the process [here](https://sydney-informatics-hub.github.io/AgReFed-Workshop/pydocs/setup-gee.html#part-ii-authorising-your-workstation-with-gee).
+
+NOTE: You only have to perform this authorisation ONCE. Or at least you only have to do it once per “connection” or if you use an incognito window.  
 
-If you like to develop Data Harvester locally, it is recommended to setup a virtual environment for the installation, e.g., via conda miniforge (see for dependencies `environment.yaml`).
+
+### Local development
+
+If you like to develop Data Harvester locally, it is recommended to setup a virtual environment for the installation, e.g., via conda miniforge (see for dependencies `environment.yaml`) and to fork the Geodata-harvester repo. To install only the latest development version use:
+
+```bash
+pip install git+https://github.com/Sydney-Informatics-Hub/geodata-harvester
+```
+
+### Workshop Cloud Sandbox
+
+As play-ground for workshop training sessions and testing of the Geodata-Harvester we provide a pre-installed cloud Python Jupyterlab environment, which does not require any local installation. For login instructions and how to access the sandbox, please visit our [Python workshop page](https://sydney-informatics-hub.github.io/AgReFed-Workshop/pydocs/py00-workshop.html).
+
+The Jupyter environment is hosted on the ARDC Nectar Research Cloud in partnership with AgReFed and Australian Research Data Commons (ARDC). Note that this sandbox is currently hosted for test purposes only and generated data is not permanently stored.
+
+The Geodata-Harvester can be easily installed also on other cloud services (e.g., Google Colab, Azure Notebooks).
 
 
 ## How to get started
 
 You may now invoke the geodata-harvester directly from a python terminal with:
 
 ```python
-import geodata_harvester as gh
-gh.harvest.run(PATH_TO_SETTINGS_YAMLFILE)
+import geodata_harvester as gdh
+gdh.harvest.run(PATH_TO_SETTINGS_YAMLFILE)
 ```
 
 **Note the subtle but important difference in use of an underscore `_` to import the package and the use of a dash `-` to install it!**
 
 To get started, some example workflows are provided as Jupyter notebooks:
 
 1. Options and user settings are defined by the user in the settings; see for settings documentation [Settings_Overview](quarto/docs/Settings_Overview.md)
@@ -137,14 +177,18 @@
 ## How to add new data source modules
 
 The Geodata-Harvester is designed to be extendable and new data source modules can be added as Python modules (for examples, see `getdata_*.py` modules). If you would like to add a new data source, please follow the [adding new data source guidelines](quarto/docs/How_to_add_DataSources.md)  
 
 We recommend to fork the geodata-harvester repo and develop new modules in a local environment. If you would like to contribute your data source module to the geodata-harvester package, please visit the [geodata-harvester contribution guidelines](quarto/docs/Contributing.md).
 
 
+## Code reference API
+
+An auto-generated API reference documentation is available [here](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
+
 ## Contributions
 We are happy for any contribution to the geodata-harvester, whether feedbacks and bug reports via github Issues, adding use-case examples via notebook contributions, to improving source-code and adding new or updating existing data source modules. 
 
 For more details about about how to contribute to the development, please visit the [Geodata-Harvester contribution guidelines](quarto/docs/Contributing.md).
 
 
 ## Attribution and Acknowledgments
```

### Comparing `geodata-harvester-0.2.2/setup.py` & `geodata-harvester-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 try:
     from setuptools import setup, find_packages
 except ImportError:
     from distutils.core import setup
 from os import path
 import io
 
-PYPI_VERSION = '0.2.2'
+PYPI_VERSION = '1.0.0'
 
 this_directory = path.abspath(path.dirname(__file__))
 with io.open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 packages = find_packages('src')
 package_dir = {'': 'src'}
```

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/__init__.py` & `geodata-harvester-1.0.0/src/geodata_harvester/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 - SILO Climate Database, see getdata_silo.py
 - National Digital Elevation Model (DEM), see getdata_dem.py
 - Digital Earth Australia (DEA) Geoscience Earth Observations, see getdata_dea.py
 - Radiometric Data, see getdata_radiometric.py
 - Google Earth Engine Data (GEE account needed), see docs for eeharvest
 """
 
-__version__ = "0.2.2"
+__version__ = "1.0.0"
 __title__ = "Geodata-Harvester"
 __description__ = """
 This Python package provides automation tools for harvesting and processing geodata from the web.
 """
 __uri__ = "https://github.com/Sydney-Informatics-Hub/geodata-harvester"
 __doc__ = __description__ + " <" + __uri__ + ">"
```

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/arc2meter.py` & `geodata-harvester-1.0.0/src/geodata_harvester/arc2meter.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/getdata_dea.py` & `geodata-harvester-1.0.0/src/geodata_harvester/getdata_dea.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/getdata_dem.py` & `geodata-harvester-1.0.0/src/geodata_harvester/getdata_dem.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/getdata_landscape.py` & `geodata-harvester-1.0.0/src/geodata_harvester/getdata_landscape.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/getdata_radiometric.py` & `geodata-harvester-1.0.0/src/geodata_harvester/getdata_radiometric.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/getdata_silo.py` & `geodata-harvester-1.0.0/src/geodata_harvester/getdata_silo.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,29 +145,34 @@
     """
 
     # create empty array
     dsnew = xarray.Dataset()
 
     for i in range(len(ds.time)):
 
-        # We will use the date of the image to name the GeoTIFF
+        # We will the date of the image to name the GeoTIFF
         date = ds.isel(time=i).time.dt.strftime("%Y-%m-%d").data
         # print(f'Writing {date}')
 
         da = ds.isel(time=i)
+        attr = ds.attrs
         dsnew[str(date)] = xarray.DataArray(
             da.variables[layername][:],
             dims=["lat", "lon"],
             coords={"lat": da.variables["lat"], "lon": da.variables["lon"]},
+            name = str(date)     
         )
+        dsnew[str(date)].attrs = {'long_name': str(date)}
 
         # Write GeoTIFF with datacube libary for cloud optimized GeoTIFFs (COG)
         # write_cog(geo_im=singletimestamp_da,
         #         fname=os.path.join(outpath,f'{outfname_base}_{date}.tif',
         #         overwrite=True)
+
+    
     # Set crs
     dsnew.rio.write_crs(4326, inplace=True)
 
     # Write GeoTIFF to disk
     dsnew.rio.to_raster(outfname)
 
 
@@ -270,43 +275,14 @@
         else:
             fnames_out_silo.append(outfname)
 
     return fnames_out_silo
     
 
 
-def process_raster_daterange(infnames, date_start, date_end, outfname, layername):
-    """ Combines all the raster data into one xarray dataset, trimming to the date range, 
-    and saves it as a multiband tif file.
-
-    Input:
-        infnames : list of input filenames
-        date_start : str, start date of time series in format 'YYYY-MM-DD'
-        date_end : str, end date of time series in format 'YYYY-MM-DD'
-        outfname : str, path+name of output file
-    """
-    # Read all the raster data into one xarray dataset
-    try:
-        # Requires dask installed
-        ds = xarray.open_mfdataset(infnames, combine="by_coords")
-    except:
-        # If dask is not installed, merge it this way (not as memory efficient)
-        ds = xarray.merge([xarray.open_dataset(f) for f in infnames])
-    # Clip to date range
-    ds = ds.sel(time=slice(date_start, date_end))
-    # Save file
-    # if file extension is tif, save as 
-    if outfname.endswith('.tif'):
-        xarray2tif(ds, outfname, layername)
-    if outfname.endswith('.nc'):
-        ds.to_netcdf(outfname)
-    # Close file
-    ds.close()
-
-
 
 def process_raster_daterange(infnames, date_start, date_end, outfname, layername):
     """ Combines all the raster data into one xarray dataset, trimming to the date range, 
     and saves it as a multiband tif file.
 
     Input:
         infnames : list of input filenames
```

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/getdata_slga.py` & `geodata-harvester-1.0.0/src/geodata_harvester/getdata_slga.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/settingshandler.py` & `geodata-harvester-1.0.0/src/geodata_harvester/settingshandler.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/spatial.py` & `geodata-harvester-1.0.0/src/geodata_harvester/spatial.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/utils.py` & `geodata-harvester-1.0.0/src/geodata_harvester/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     channels.
 aggregate_multiband: Averages (or similar) over multiple files but keeps
     multi-channels independent.
 _get_coords_at_point (internal): Finds closest index of a point-location in an
     array (raster).
 raster_query: Given a longitude,latitude value, return the value at that point
     of a raster/tif.
+extract_values_from_rasters: Given a list of rasters, extract the values at coords.
 init_logtable: Stores metdata for each step of raster download and processing.
 update_logtable: Updates each the logtable with new information.
 """
 
 from glob import glob
 import os
 import json
@@ -31,14 +32,15 @@
 from rasterio.mask import mask
 from rasterio.warp import calculate_default_transform, reproject, Resampling
 from rasterio.plot import show
 
 import numpy as np
 import pandas as pd
 import geopandas as gpd
+import rioxarray as rxr
 
 from pyproj import CRS
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 from matplotlib.ticker import FormatStrFormatter
 
@@ -570,14 +572,16 @@
     col = int((lat - gt[5]) / gt[4])
 
     return (col, row)
 
 
 def raster_query(longs, lats, rasters, titles=None):
     """
+    DEPRECATED: Use extract_values_from_rasters instead.
+
     given a longitude,latitude value, return the value at that point of the
         first channel/band in the raster/tif.
 
     INPUTS
         longs:list of longitudes
         lats:list of latitudes
         rasters:list of raster filenames (as strings)
@@ -599,14 +603,15 @@
     for filepath in rasters:
         filename = Path(filepath).resolve().stem
         # print("Opening:", filename)
         # Open the file:
         raster = rasterio.open(filepath)
         # Get the transformation crs data
         gt = raster.transform
+
         # This will only be the first band, usally multiband has same index.
         arr = raster.read(1)
 
         if titles is not None:
             colname = titles[rasters.index(filepath)]
         else:
             colname = Path(filepath).stem
@@ -642,14 +647,101 @@
         # dd the values at the points to the dataframe
         gdf[filepath] = values
         gdf = gdf.rename(columns={filepath: colname})
 
     return gdf
 
 
+def extract_values_from_rasters(coords, raster_files, method = "nearest"):
+    """
+    Extract values from a list of raster files at given coordinates using rioxarray.
+    Values will be extracted for all bands in each raster file.
+    Return geopandas DataFrame with extracted values and geometry.
+
+    Input:
+        coords: A list of tuples containing longitude and latitude coordinates.
+                Format: [(lng1, lat1), (lng2, lat2), ...]
+
+        raster_files: A list of raster file paths.
+                      Format: ["path/to/raster1.tif", "path/to/raster2.tif", ...]
+
+        method: The method to select values from raster files for 
+                inexact matches between input coords and raster coords:
+                 {"nearest", "pad", "ffill", "backfill", "bfill"}, optional
+            - nearest (Default): use nearest valid index value. 
+            - pad / ffill: propagate last valid index value forward
+            - backfill / bfill: propagate next valid index value backward
+            - None: only exact matches
+
+    Output:
+        A geopandas DataFrame containing the extracted values and geometry, where each row represents
+        a coordinate point and the columns represent the bands for each raster file.
+        Output column names are the raster file name plus the band name.
+    """
+    all_coords_data = []
+    column_names = []
+
+    with spin("Extracting values from raster files...", "blue") as s:
+        for raster_file in raster_files:
+            # Open the raster file with rioxarray
+            ds = rxr.open_rasterio(raster_file)
+            
+            # Extract values for all coordinates
+            coords_data = []
+            for lng, lat in coords:
+                # Select the nearest lat and lon coordinates from the dataset
+                data = ds.sel(x=lng, y=lat, method=method)
+                
+                # Convert the data to a numpy array and flatten it
+                data_array = data.values.flatten().tolist()
+                
+                # Add the extracted values to the list
+                coords_data.append(data_array)
+
+            # Concatenate the extracted values from all raster files
+            all_coords_data.append(coords_data)
+
+            # try to det the band names from the dataset, otherwise use the band number
+            try:
+                band_names = ds.attrs['long_name']
+                if isinstance(band_names, str):
+                    band_names = [band_names]
+                if isinstance(band_names, tuple):
+                    band_names = list(band_names)
+                if len(band_names) != len(ds.band.values.tolist()):
+                    band_names = ds.band.values.tolist()
+            except:
+                band_names = ds.band.values.tolist()
+            # get the raster name
+            raster_name = os.path.basename(raster_file).split(".")[0]
+            # Add the raster name to the band names
+            band_names = [f"{raster_name}_{band_name}" for band_name in band_names]
+
+            # Add the band names to the column names list
+            column_names.extend(band_names)
+
+    # Convert the data to a pandas DataFrame and include the column names
+    all_coords_data = pd.DataFrame(np.hstack(all_coords_data), columns=column_names)
+    
+    # Check for potential duplicate column names in all_coords_data
+    if all_coords_data.columns.duplicated().any():
+        print("Duplicate column names found. Please check the input raster files.")
+        # drop duplicate columns and leave only first occurence
+        all_coords_data = all_coords_data.loc[:,~all_coords_data.columns.duplicated()].copy()
+
+    # save all_coords_data with coords as geopackage with geopandas
+    gdf = gpd.GeoDataFrame(all_coords_data, geometry=gpd.points_from_xy(coords[:,0], coords[:,1]), crs="EPSG:4326")
+
+    # insert the coords into the dataframe
+    gdf.insert(0, 'Longitude', coords[:,0])
+    gdf.insert(1, 'Latitude', coords[:,1])
+
+    return gdf
+
+
 def init_logtable():
     """
     Create a log table to store information from the raster download or processing.
 
     RETURNS:
         df_log: dataframe to update
     """
```

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/validate_settings.py` & `geodata-harvester-1.0.0/src/geodata_harvester/validate_settings.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/widgets/harvesterwidgets.py` & `geodata-harvester-1.0.0/src/geodata_harvester/widgets/harvesterwidgets.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/widgets/ipyfilechooser/errors.py` & `geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/errors.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/widgets/ipyfilechooser/filechooser.py` & `geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/filechooser.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/widgets/ipyfilechooser/utils.py` & `geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/utils.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/widgets/ipywidgets_file_selector.py` & `geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipywidgets_file_selector.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester/write_logs.py` & `geodata-harvester-1.0.0/src/geodata_harvester/write_logs.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester.egg-info/PKG-INFO` & `geodata-harvester-1.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,43 @@
-Metadata-Version: 2.1
-Name: geodata-harvester
-Version: 0.2.2
-Summary: An automation tool for harvesting and processing geodata from the web
-Home-page: https://github.com/Sydney-Informatics-Hub/geodata-harvester
-License: LGPL-3.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Geodata-Harvester
 
-<h3><em>Automate geodata harvesting from the web and jumpstart your analysis with a ready-made set of spatial-temporal processed maps and dataframes.</em></h3> 
+<h3><em>Automate geodata harvesting from the web and jumpstart your analysis with a ready-made set of spatiotemporal processed maps and data tables.</em></h3> 
 
 <center><a><img src="quarto/images/dataharvester_logo.png" alt="Geodata-Harvester logo" width="100%"/></a></center>
 
 
 <!-- Badges  start -->
 
 [![License](https://img.shields.io/badge/License-LGPL3-blue)](#license)
-
-<!-- [![GitHub tag](https://img.shields.io/github/tag/Sydney-Informatics-Hub/AgReFed-DataHarvester?include_prereleases=&sort=semver&color=blue)](https://github.com/Sydney-Informatics-Hub/AgReFed-DataHarvester/releases/)
-[![issues - AgReFed-DataHarvester](https://img.shields.io/github/issues/Sydney-Informatics-Hub/AgReFed-DataHarvester)](https://github.com/Sydney-Informatics-Hub/AgReFed-DataHarvester/issues) -->
+[![PyPI-Server](https://img.shields.io/pypi/v/geodata-harvester.svg)](https://pypi.org/project/geodata-harvester/)
+[![Conda
+Version](https://img.shields.io/conda/vn/conda-forge/geodata-harvester.svg)](https://anaconda.org/conda-forge/geodata-harvester)
+[![Monthly Downloads](https://pepy.tech/badge/geodata-harvester/month)](https://pepy.tech/project/geodata-harvester)
 
 <!-- Badges end -->
 
 The Geodata-Harvester Python package offers reusable and automated workflows for data extraction from a wide range of geospatial and environmental data sources. User provided data is auto-completed with a suitable set of spatial- and temporal-aligned covariates as a ready-made dataset for machine learning and environmental models. In addition, all requested data layer maps are automatically extracted and aligned for a specific region and time period.
 
 For the R-package wrapper of the Geodata-Harvester, please visit the [Github dataharvesteR project](https://github.com/Sydney-Informatics-Hub/dataharvester).
 
 ## Content
 
 - [Introduction](#introduction)
 - [Data Sources](#data-sources)
 - [Functionality](#functionality)
 - [Key Features](#key-features)
 - [Installation](#installation)
+    - [Conda or Mamba](#conda-or-mamba)
+    - [PyPI](#pypi)
+    - [Google Earth Engine extension](#google-earth-engine-extension)
+    - [Local development](#local-development)
+    - [Workshop Cloud Sandbox](#workshop-cloud-sandbox)
 - [How to get started](#how-to-get-started)
 - [How to add new data source modules](#how-to-add-new-data-source-modules)
+- [Code reference API](#code-reference-api)
 - [Contributions](#contributions)
 - [Attribution and Acknowledgments](#attribution-and-acknowledgments)
 - [License](#license)
 
 
 ## Introduction
 
@@ -74,70 +69,91 @@
 
 Geodata-Harvester is designed as a modular and maintainable project in the form of a multi-stage pipeline by providing explicit boundaries among tasks. To encourage interaction and experimentation with the pipeline, multiple frontend notebooks and use case scenarios are provided.
 
 ## Key Features
 
 Below is a list of features available for the geodata-harvester package. Please check the project Github webpage and notebooks for examples, data selection, and other settings.
 
-- enabling reproducible workflows via YAML settings files
-- automatic data retrieval from geodata APIs for given locations and dates
-- automatic download and spatial-temporal processing of geo-spatial maps for user-specified bounding box, resolution, and time-scale.
-- support for multiple temporal aggregation options and spatial-temporal buffer
-- automatic extraction of retrieved data into ready-made dataframes for ML training
-- automatic generation of ready-made aligned maps and data for ML prediction models
-- visualisation of downloaded and aligned maps
-- support for saving and loading settings via interactive widgets
-- with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices
+- enabling reproducible workflows via YAML settings files.
+- automatic data retrieval from geodata APIs for given locations and dates.
+- automatic download and spatiotemporal processing of geo-spatial maps for user-specified bounding box, resolution, and time-scale.
+- support for time-series data extraction for multiple time slices. 
+- automatic extraction of retrieved data into ready-made dataframes for ML training.
+- automatic generation of ready-made aligned maps in GeoTiff format.
+- preview of downloaded and aligned maps.
+- support for saving and loading settings via interactive widgets.
+- with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices.
+- example notebooks and use-cases are provided for the user to get started.
 
 For more features, please see the [API reference documentation](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
 
 ## Installation
 
 Geodata-Harvester can be run on cloud-servers (e.g., in JupyterHub environment) or on your local machine. 
-Example notebooks for importing and using the package can be found in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks). To install the package run one of the following
+Example notebooks for importing and using the package can be found in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks). The package can be installed via PyPI or Conda:
 
-### Conda or Mamba install
+### Conda or Mamba
 
 The package geodata-harvester is available via the conda-forge channel:
 
 ```bash
 conda install geodata-harvester -c conda-forge
 ```
 
 Note that the geodata-harvester is imported with underscore as 
 
 ```Python
 import geodata_harvester
 ```
 
-### Pip install
+### PyPI
 
-Installation via pypi requires a pre-installation of gdal (see, e.g., [pypi.org/project/GDAL/installation guide](https://pypi.org/project/GDAL/)) in your environment. Once gdal is installed, you can install geodata-harvester via
+Installation via PyPI requires a pre-installation of gdal (see, e.g., [pypi.org/project/GDAL/installation guide](https://pypi.org/project/GDAL/)) in your environment. Once gdal is installed, you can install geodata-harvester via
 
 ```bash
 pip install geodata-harvester
 ```
 The geodata-harvester library can then be imported via
 
 ```Python
 import geodata_harvester
 ```
 
-### Requirements
+### Google Earth Engine extension
+
+Optionally you can include Google Earth Engine (GEE) data in Geodata-Harvester (see [Settings_Overview](quarto/docs/Settings_Overview.md)).
+GEE requires a Google account and a GEE authorization. If this is your first time using GEE, please follow [these instructions](https://earthengine.google.com/signup/) and authorise Geodata-Harvester to use the Google Earth Engine API. See a preview of the process [here](https://sydney-informatics-hub.github.io/AgReFed-Workshop/pydocs/setup-gee.html#part-ii-authorising-your-workstation-with-gee).
+
+NOTE: You only have to perform this authorisation ONCE. Or at least you only have to do it once per “connection” or if you use an incognito window.  
 
-If you like to develop Data Harvester locally, it is recommended to setup a virtual environment for the installation, e.g., via conda miniforge (see for dependencies `environment.yaml`).
+
+### Local development
+
+If you like to develop Data Harvester locally, it is recommended to setup a virtual environment for the installation, e.g., via conda miniforge (see for dependencies `environment.yaml`) and to fork the Geodata-harvester repo. To install only the latest development version use:
+
+```bash
+pip install git+https://github.com/Sydney-Informatics-Hub/geodata-harvester
+```
+
+### Workshop Cloud Sandbox
+
+As play-ground for workshop training sessions and testing of the Geodata-Harvester we provide a pre-installed cloud Python Jupyterlab environment, which does not require any local installation. For login instructions and how to access the sandbox, please visit our [Python workshop page](https://sydney-informatics-hub.github.io/AgReFed-Workshop/pydocs/py00-workshop.html).
+
+The Jupyter environment is hosted on the ARDC Nectar Research Cloud in partnership with AgReFed and Australian Research Data Commons (ARDC). Note that this sandbox is currently hosted for test purposes only and generated data is not permanently stored.
+
+The Geodata-Harvester can be easily installed also on other cloud services (e.g., Google Colab, Azure Notebooks).
 
 
 ## How to get started
 
 You may now invoke the geodata-harvester directly from a python terminal with:
 
 ```python
-import geodata_harvester as gh
-gh.harvest.run(PATH_TO_SETTINGS_YAMLFILE)
+import geodata_harvester as gdh
+gdh.harvest.run(PATH_TO_SETTINGS_YAMLFILE)
 ```
 
 **Note the subtle but important difference in use of an underscore `_` to import the package and the use of a dash `-` to install it!**
 
 To get started, some example workflows are provided as Jupyter notebooks:
 
 1. Options and user settings are defined by the user in the settings; see for settings documentation [Settings_Overview](quarto/docs/Settings_Overview.md)
@@ -149,14 +165,18 @@
 ## How to add new data source modules
 
 The Geodata-Harvester is designed to be extendable and new data source modules can be added as Python modules (for examples, see `getdata_*.py` modules). If you would like to add a new data source, please follow the [adding new data source guidelines](quarto/docs/How_to_add_DataSources.md)  
 
 We recommend to fork the geodata-harvester repo and develop new modules in a local environment. If you would like to contribute your data source module to the geodata-harvester package, please visit the [geodata-harvester contribution guidelines](quarto/docs/Contributing.md).
 
 
+## Code reference API
+
+An auto-generated API reference documentation is available [here](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
+
 ## Contributions
 We are happy for any contribution to the geodata-harvester, whether feedbacks and bug reports via github Issues, adding use-case examples via notebook contributions, to improving source-code and adding new or updating existing data source modules. 
 
 For more details about about how to contribute to the development, please visit the [Geodata-Harvester contribution guidelines](quarto/docs/Contributing.md).
 
 
 ## Attribution and Acknowledgments
```

### Comparing `geodata-harvester-0.2.2/src/geodata_harvester.egg-info/SOURCES.txt` & `geodata-harvester-1.0.0/src/geodata_harvester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

