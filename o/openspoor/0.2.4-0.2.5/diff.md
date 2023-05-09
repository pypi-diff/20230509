# Comparing `tmp/openspoor-0.2.4.tar.gz` & `tmp/openspoor-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openspoor-0.2.4.tar", last modified: Mon Jan 30 12:06:56 2023, max compression
+gzip compressed data, was "openspoor-0.2.5.tar", last modified: Tue May  9 12:58:09 2023, max compression
```

## Comparing `openspoor-0.2.4.tar` & `openspoor-0.2.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:06:56.460156 openspoor-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-30 12:06:34.000000 openspoor-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-01-30 12:06:56.456155 openspoor-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-01-30 12:06:34.000000 openspoor-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:06:56.448155 openspoor-0.2.4/openspoor/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:06:56.452155 openspoor-0.2.4/openspoor/mapservices/
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/mapservices/MapservicesQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/mapservices/PUICMapservices.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/mapservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/mapservices/find_mapservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:06:56.452155 openspoor-0.2.4/openspoor/spoortakmodel/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/spoortakmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/spoortakmodel/spoortak_model_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/spoortakmodel/spoortak_model_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/spoortakmodel/spoortak_models_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/spoortakmodel/spoortak_subsection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:06:56.452155 openspoor-0.2.4/openspoor/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/transformers/TransformerCoordinatesToSpoor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/transformers/TransformerGeocodeToCoordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/transformers/TransformerSpoortakToCoordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/transformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:06:56.452155 openspoor-0.2.4/openspoor/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/utils/safe_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:06:56.452155 openspoor-0.2.4/openspoor/visualisations/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/visualisations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17297 2023-01-30 12:06:38.000000 openspoor-0.2.4/openspoor/visualisations/trackmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:06:56.452155 openspoor-0.2.4/openspoor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-01-30 12:06:56.000000 openspoor-0.2.4/openspoor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-01-30 12:06:56.000000 openspoor-0.2.4/openspoor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 12:06:56.000000 openspoor-0.2.4/openspoor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 12:06:56.000000 openspoor-0.2.4/openspoor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-30 12:06:56.000000 openspoor-0.2.4/openspoor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-30 12:06:56.000000 openspoor-0.2.4/openspoor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-30 12:06:38.000000 openspoor-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 12:06:56.460156 openspoor-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-01-30 12:06:38.000000 openspoor-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:06:56.456155 openspoor-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 12:06:38.000000 openspoor-0.2.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:06:56.456155 openspoor-0.2.4/tests/spoortakmodel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 12:06:38.000000 openspoor-0.2.4/tests/spoortakmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-01-30 12:06:38.000000 openspoor-0.2.4/tests/spoortakmodel/test_spoortak_model_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-01-30 12:06:38.000000 openspoor-0.2.4/tests/spoortakmodel/test_spoortak_model_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-01-30 12:06:38.000000 openspoor-0.2.4/tests/spoortakmodel/test_spoortak_models_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23391 2023-01-30 12:06:38.000000 openspoor-0.2.4/tests/test_Acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-01-30 12:06:38.000000 openspoor-0.2.4/tests/test_MapservicesData.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-01-30 12:06:38.000000 openspoor-0.2.4/tests/test_PUICMapservices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-01-30 12:06:38.000000 openspoor-0.2.4/tests/test_TransformerCoordinatesToSpoor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-01-30 12:06:38.000000 openspoor-0.2.4/tests/test_TransformerGeocodeToCoordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-01-30 12:06:38.000000 openspoor-0.2.4/tests/test_TransformerSpoortakToCoordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-01-30 12:06:38.000000 openspoor-0.2.4/tests/test_find_mapservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:58:09.994083 openspoor-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-09 12:57:51.000000 openspoor-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-05-09 12:58:09.994083 openspoor-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-05-09 12:57:51.000000 openspoor-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:58:09.986082 openspoor-0.2.5/openspoor/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:58:09.990082 openspoor-0.2.5/openspoor/mapservices/
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/mapservices/MapservicesQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/mapservices/PUICMapservices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/mapservices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/mapservices/find_mapservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:58:09.990082 openspoor-0.2.5/openspoor/spoortakmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/spoortakmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/spoortakmodel/spoortak_model_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/spoortakmodel/spoortak_model_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/spoortakmodel/spoortak_models_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/spoortakmodel/spoortak_subsection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:58:09.990082 openspoor-0.2.5/openspoor/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/transformers/TransformerCoordinatesToSpoor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/transformers/TransformerGeocodeToCoordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/transformers/TransformerSpoortakToCoordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:58:09.990082 openspoor-0.2.5/openspoor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/utils/safe_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:58:09.990082 openspoor-0.2.5/openspoor/visualisations/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/visualisations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17297 2023-05-09 12:57:55.000000 openspoor-0.2.5/openspoor/visualisations/trackmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:58:09.990082 openspoor-0.2.5/openspoor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-05-09 12:58:09.000000 openspoor-0.2.5/openspoor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-09 12:58:09.000000 openspoor-0.2.5/openspoor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 12:58:09.000000 openspoor-0.2.5/openspoor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 12:58:09.000000 openspoor-0.2.5/openspoor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-09 12:58:09.000000 openspoor-0.2.5/openspoor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 12:58:09.000000 openspoor-0.2.5/openspoor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-09 12:57:55.000000 openspoor-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 12:58:09.994083 openspoor-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-09 12:57:55.000000 openspoor-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:58:09.990082 openspoor-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:57:55.000000 openspoor-0.2.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:58:09.994083 openspoor-0.2.5/tests/spoortakmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:57:55.000000 openspoor-0.2.5/tests/spoortakmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-09 12:57:55.000000 openspoor-0.2.5/tests/spoortakmodel/test_spoortak_model_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-09 12:57:55.000000 openspoor-0.2.5/tests/spoortakmodel/test_spoortak_model_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-09 12:57:55.000000 openspoor-0.2.5/tests/spoortakmodel/test_spoortak_models_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-05-09 12:57:55.000000 openspoor-0.2.5/tests/test_Acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-09 12:57:55.000000 openspoor-0.2.5/tests/test_MapservicesData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-09 12:57:55.000000 openspoor-0.2.5/tests/test_PUICMapservices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-09 12:57:55.000000 openspoor-0.2.5/tests/test_TransformerCoordinatesToSpoor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-09 12:57:55.000000 openspoor-0.2.5/tests/test_TransformerGeocodeToCoordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-09 12:57:55.000000 openspoor-0.2.5/tests/test_TransformerSpoortakToCoordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-09 12:57:55.000000 openspoor-0.2.5/tests/test_find_mapservice.py
```

### Comparing `openspoor-0.2.4/LICENSE` & `openspoor-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/PKG-INFO` & `openspoor-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openspoor
-Version: 0.2.4
+Version: 0.2.5
 Summary: Open source project to allow translations between different spoor referential systems
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Openspoor
 
@@ -44,15 +44,15 @@
 
 #### Linux
 
 - `pip install openspoor`
 
 #### Mac
 
-- `conda create -n [env_name] python=3.8`
+- `conda create -n [env_name] python=3.11`
 - `conda install -c conda-forge proj=7.0.0`
 - `conda install -c conda-forge pyproj=2.6.0`
 - `pip install openspoor`
 
 The steps above involving conda(-forge) are necessary for Mac M1 chips (used since Nov 2020). In case your Mac does not
 have a M1 chip, then `pip install openspoor` should suffice.
 
@@ -60,19 +60,19 @@
 
 #### Windows
 
 Installation using anaconda
 - Clone the "openspoor" repository
   - `git clone https://github.com/ProRail-DataLab/openspoor.git`
 - create an environment:
-  - `conda create -n openspoorenv python==3.8`
+  - `conda create -n openspoorenv python==3.11`
 - activate the environment:
   - `conda activate openspoorenv`
 - install dependencies:
-  - `conda install -c conda-forge --file requirements.txt`
+  - `pip install -r requirements.txt`
 - In the root directory of the repository, execute the command:
   - `pip install -e .[dev]`
 - In the root directory of the repository, execute the command:
   - `pytest --nbmake --nbmake-kernel=python3`
 - If all the test succeed, the openspoor package is ready to use and you are on the right "track"!
 
 #### Linux
```

### Comparing `openspoor-0.2.4/README.md` & `openspoor-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 #### Linux
 
 - `pip install openspoor`
 
 #### Mac
 
-- `conda create -n [env_name] python=3.8`
+- `conda create -n [env_name] python=3.11`
 - `conda install -c conda-forge proj=7.0.0`
 - `conda install -c conda-forge pyproj=2.6.0`
 - `pip install openspoor`
 
 The steps above involving conda(-forge) are necessary for Mac M1 chips (used since Nov 2020). In case your Mac does not
 have a M1 chip, then `pip install openspoor` should suffice.
 
@@ -52,19 +52,19 @@
 
 #### Windows
 
 Installation using anaconda
 - Clone the "openspoor" repository
   - `git clone https://github.com/ProRail-DataLab/openspoor.git`
 - create an environment:
-  - `conda create -n openspoorenv python==3.8`
+  - `conda create -n openspoorenv python==3.11`
 - activate the environment:
   - `conda activate openspoorenv`
 - install dependencies:
-  - `conda install -c conda-forge --file requirements.txt`
+  - `pip install -r requirements.txt`
 - In the root directory of the repository, execute the command:
   - `pip install -e .[dev]`
 - In the root directory of the repository, execute the command:
   - `pytest --nbmake --nbmake-kernel=python3`
 - If all the test succeed, the openspoor package is ready to use and you are on the right "track"!
 
 #### Linux
```

### Comparing `openspoor-0.2.4/openspoor/config.yaml` & `openspoor-0.2.5/openspoor/config.yaml`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/openspoor/mapservices/MapservicesQuery.py` & `openspoor-0.2.5/openspoor/mapservices/MapservicesQuery.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/openspoor/mapservices/PUICMapservices.py` & `openspoor-0.2.5/openspoor/mapservices/PUICMapservices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 from loguru import logger
-from .MapservicesQuery import MapServicesQuery
+from functools import cache
 from .find_mapservice import FeatureServerOverview
 from ..utils.common import read_config
 
 config = read_config()
 
 
 class PUICMapservices:
@@ -26,14 +26,15 @@
         if spoor_cache_location:
             self.spoor_query.write_gpkg(spoor_cache_location)
         if wisselkruisingbeen_cache_location:
             self.wisselkruisingbeen_query.write_gpkg(wisselkruisingbeen_cache_location)
 
         self.spoordata_columns = config['spoordata_columns']
 
+    @cache
     def load_data(self, *args, **kwargs):
         """
         Return combined spoortak, wissel and kruising data from
         self.spoor_url and self.wisselkruisingbeen_url
         """
         spoor_gdf = self.spoor_query.load_data()
         spoor_gdf = self._prep_spoor_gdf(spoor_gdf)
```

### Comparing `openspoor-0.2.4/openspoor/mapservices/find_mapservice.py` & `openspoor-0.2.5/openspoor/mapservices/find_mapservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pandas as pd
 import re
 from loguru import logger
 from pathlib import Path
 import geopandas as gpd
+from functools import cache
 
 from ..utils.safe_requests import SafeRequest
 from openspoor.mapservices.MapservicesQuery import MapServicesQuery
 from openspoor.utils.singleton import Singleton
 
 
 class FeatureSearchResults(pd.DataFrame):
@@ -64,14 +65,15 @@
         :return: A pandas dataframe, listing the urls and descriptions of the found layers
         """
         featureserver_text = SafeRequest().get_string('GET', featureserver_url)
         featureservers = re.findall(r'href="/(.+)">(.+)</a> \(\d+\)', featureserver_text)
         featureservers = [[f'{self.prefix}{fs}', description] for fs, description in featureservers]
         return pd.DataFrame(featureservers, columns=['layer_url', 'description'])
 
+    @cache
     def get_all_featureserver_layers(self) -> pd.DataFrame:
         """
         Find all available layers within the mapservices featureservers.
 
         :return: A pandas dataframe, listing the urls and descriptions of the found layers in all featureservers
         """
         all_services = SafeRequest().get_string('GET', self.base_url)
```

### Comparing `openspoor-0.2.4/openspoor/spoortakmodel/spoortak_model_inspector.py` & `openspoor-0.2.5/openspoor/spoortakmodel/spoortak_model_inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,15 @@
 
         model_data = pd.DataFrame(columns=list(self.data.models[baseline_model].columns) + ['spoortakmodel'])
 
         for spoortakmodel_version, model in self.data.models.items():
             if spoortak_identifier in model.index:
                 df = model.loc[spoortak_identifier]
                 df['spoortakmodel'] = spoortakmodel_version
-                # model_data = pd.concat([model_data, df], axis=1)
-                model_data = model_data.append(df)
+                model_data = pd.concat([model_data, pd.DataFrame(df).T], axis=0)
         pprint(model_data)
 
         print(f'--- {spoortak_identifier} spoortakmodel changes ---')
 
         change_data = pd.DataFrame(columns=list(self.data.model_changes[baseline_model].columns) + ['spoortakmodel'])
 
         for spoortakmodel_version, model_changes in self.data.model_changes.items():
```

### Comparing `openspoor-0.2.4/openspoor/spoortakmodel/spoortak_model_mapper.py` & `openspoor-0.2.5/openspoor/spoortakmodel/spoortak_model_mapper.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/openspoor/spoortakmodel/spoortak_models_data.py` & `openspoor-0.2.5/openspoor/spoortakmodel/spoortak_models_data.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/openspoor/spoortakmodel/spoortak_subsection.py` & `openspoor-0.2.5/openspoor/spoortakmodel/spoortak_subsection.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/openspoor/transformers/TransformerCoordinatesToSpoor.py` & `openspoor-0.2.5/openspoor/transformers/TransformerCoordinatesToSpoor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import geopandas as gpd
 from loguru import logger
-from functools import lru_cache
+from functools import cache
 
 from openspoor.utils.common import read_config
 from openspoor.mapservices import FeatureServerOverview
 
 config = read_config()
 
 
@@ -24,18 +24,16 @@
         logger.info(
             "Initiating TransformerCoordinatesToSpoor object in order to "
             "transform between various ProRail spoor coordinate systems"
         )
 
         self.buffer_distance = buffer_distance
         self.stgk = self._get_spoortak_met_geokm()
-        # Buffer style prevents overflow into next segment; buffer has straight edges at the end
-        self.buffered_stgk = self.stgk.assign(geometry=lambda x: x.geometry.buffer(self.buffer_distance, cap_style=2))
 
-    @lru_cache
+    @cache
     def _get_spoortak_met_geokm(self):
         return FeatureServerOverview().search_for('Spoortakdeel met geocode kilometrering') \
             .load_data(return_m=True)
 
     @staticmethod
     def _determine_geocode_km(gdf_lines, gdf_points):
         """
@@ -59,14 +57,17 @@
 
         :param gdf_points: A geodataframe with points data for which the geocode and spoortak coordinates are wanted.
         All crs are allowed
         :return: A geodataframe, based on the input dataframe. Every point will occur in the final output at least once,
          even if no match could be made.
         """
         # Coordinates used are RD in the below.
+        # Buffer style prevents overflow into next segment; buffer has straight edges at the end
+        self.buffered_stgk = self.stgk.assign(geometry=lambda x: x.geometry.buffer(self.buffer_distance, cap_style=2))
+        
         starting_crs = gdf_points.crs
         gdf_points = gdf_points.to_crs('EPSG:28992')
         close_geocodes = self.buffered_stgk.sjoin(gdf_points)
 
         points_geocodes = (
             self.stgk.loc[close_geocodes.index]
             .set_index(close_geocodes['index_right'])  # Sample only the list of matching hits
```

### Comparing `openspoor-0.2.4/openspoor/transformers/TransformerGeocodeToCoordinates.py` & `openspoor-0.2.5/openspoor/transformers/TransformerGeocodeToCoordinates.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/openspoor/transformers/TransformerSpoortakToCoordinates.py` & `openspoor-0.2.5/openspoor/transformers/TransformerSpoortakToCoordinates.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/openspoor/utils/common.py` & `openspoor-0.2.5/openspoor/utils/common.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/openspoor/utils/safe_requests.py` & `openspoor-0.2.5/openspoor/utils/safe_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from openspoor.utils.singleton import Singleton
 
 
 class SafeRequest(Singleton):
 
     last_request = 0  # Use a class attribute, as we use the Singleton pattern
 
-    def __init__(self, max_retry: int = 5, time_between: float = 1.0):
+    def __init__(self, max_retry: int = 5, time_between: float = 0.3):
         """
         Create a package from where we can make requests. The requests are done using certificates and a sleep is
         built in to guarantee that there is some time between every API call.
 
         :param max_retry: The maximum amount of times a request is attempted
         :param time_between: The minimum time between two consecutive queries
         """
```

### Comparing `openspoor-0.2.4/openspoor/visualisations/trackmap.py` & `openspoor-0.2.5/openspoor/visualisations/trackmap.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/openspoor.egg-info/PKG-INFO` & `openspoor-0.2.5/openspoor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openspoor
-Version: 0.2.4
+Version: 0.2.5
 Summary: Open source project to allow translations between different spoor referential systems
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Openspoor
 
@@ -44,15 +44,15 @@
 
 #### Linux
 
 - `pip install openspoor`
 
 #### Mac
 
-- `conda create -n [env_name] python=3.8`
+- `conda create -n [env_name] python=3.11`
 - `conda install -c conda-forge proj=7.0.0`
 - `conda install -c conda-forge pyproj=2.6.0`
 - `pip install openspoor`
 
 The steps above involving conda(-forge) are necessary for Mac M1 chips (used since Nov 2020). In case your Mac does not
 have a M1 chip, then `pip install openspoor` should suffice.
 
@@ -60,19 +60,19 @@
 
 #### Windows
 
 Installation using anaconda
 - Clone the "openspoor" repository
   - `git clone https://github.com/ProRail-DataLab/openspoor.git`
 - create an environment:
-  - `conda create -n openspoorenv python==3.8`
+  - `conda create -n openspoorenv python==3.11`
 - activate the environment:
   - `conda activate openspoorenv`
 - install dependencies:
-  - `conda install -c conda-forge --file requirements.txt`
+  - `pip install -r requirements.txt`
 - In the root directory of the repository, execute the command:
   - `pip install -e .[dev]`
 - In the root directory of the repository, execute the command:
   - `pytest --nbmake --nbmake-kernel=python3`
 - If all the test succeed, the openspoor package is ready to use and you are on the right "track"!
 
 #### Linux
```

### Comparing `openspoor-0.2.4/openspoor.egg-info/SOURCES.txt` & `openspoor-0.2.5/openspoor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/setup.py` & `openspoor-0.2.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 requirements = [
     "importlib_metadata",
-    "geopandas<=0.11.1",
+    "geopandas",
     "pyyaml",
     "loguru",
     "requests",
     "rtree",
-    "pyproj<3",
+    "pyproj",
     "pandas",
     "shapely",
     "folium"
 ]
 
 dev_packages = [
     "pytest",
     "pytest-cov",
     "pytest-xdist",
     "parameterized",
     "nbmake",
 ]
 
 setup(name='openspoor',
-      version='0.2.4',
+      version='0.2.5',
       description='Open source project to allow translations between different spoor referential systems',
       long_description=(Path(__file__).parent / "README.md").read_text(),
       long_description_content_type='text/markdown',
       install_requires=requirements,
       extras_require={"dev": dev_packages},
       packages=find_packages(include="openspoor*"),
       package_data={'openspoor': ['config.yaml']},
```

### Comparing `openspoor-0.2.4/tests/spoortakmodel/test_spoortak_model_inspector.py` & `openspoor-0.2.5/tests/spoortakmodel/test_spoortak_model_inspector.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         expected_bericht_rows = 3
 
         # For development and debugging we still want to see the prints
         mock_pprint.side_effect = pprint
 
         sut = SpoortakModelInspector(SpoortakModelsData(MODELS_DATA_DIR))
         sut.inspect('603_89R_2.6')
-        mock_pprint.assert_called()
         self.assertEqual(expected_spoortak_model_rows, len(mock_pprint.call_args_list[0][0][0]), )
         self.assertEqual(expected_bericht_rows, len(mock_pprint.call_args_list[1][0][0]))
 
     @patch('openspoor.spoortakmodel.spoortak_model_inspector.pprint')
     def test_spoortak_in_dassignname(self, mock_pprint):
         expected_spoortak_model_rows = 4
         expected_bericht_rows = 9
@@ -46,15 +45,14 @@
         expected_bericht_rows = 1
 
         # For development and debugging we still want to see the prints
         mock_pprint.side_effect = pprint
 
         sut = SpoortakModelInspector(SpoortakModelsData(MODELS_DATA_DIR))
         sut.inspect('927_3325R_904.6')
-        mock_pprint.assert_called()
         self.assertEqual(expected_spoortak_model_rows, len(mock_pprint.call_args_list[0][0][0]), )
         self.assertEqual(expected_bericht_rows, len(mock_pprint.call_args_list[1][0][0]))
 
     @patch('openspoor.spoortakmodel.spoortak_model_inspector.pprint')
     def test_spoortak_478_1201V_0_6(self, mock_pprint):
         """ Bug test: Gives issues on linux, but works on windows """
         expected_spoortak_model_rows = 4
@@ -62,15 +60,15 @@
 
         # For development and debugging we still want to see the prints
         mock_pprint.side_effect = pprint
 
         sut = SpoortakModelInspector(SpoortakModelsData(MODELS_DATA_DIR))
         sut.inspect('478_1201V_0.6')
         mock_pprint.assert_called()
-        self.assertEqual(expected_spoortak_model_rows, len(mock_pprint.call_args_list[0][0][0]), )
+        self.assertEqual(expected_spoortak_model_rows, len(mock_pprint.call_args_list[0][0][0]))
         self.assertEqual(expected_bericht_rows, len(mock_pprint.call_args_list[1][0][0]))
 
     @skip('Development only test, comment this skip to enable it')
     def test_develop(self):
         """ quickly inspect the data of a spoortak"""
         sut = SpoortakModelInspector(SpoortakModelsData(MODELS_DATA_DIR))
         sut.inspect('518_107BL_63.5')
```

### Comparing `openspoor-0.2.4/tests/spoortakmodel/test_spoortak_model_mapper.py` & `openspoor-0.2.5/tests/spoortakmodel/test_spoortak_model_mapper.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/tests/spoortakmodel/test_spoortak_models_data.py` & `openspoor-0.2.5/tests/spoortakmodel/test_spoortak_models_data.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/tests/test_Acceptance.py` & `openspoor-0.2.5/tests/test_Acceptance.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,19 +88,17 @@
                           (90606.367, 439129.4860, 102.8109),
                           (90621.9310, 439205.797, 102.9),
                           (90621.9452, 439205.8664, 102.9)]),
               LineString([(90451.424, 438372.246, 101.9577),
                           (90604.6240, 439120.9771, 102.8010)])],
     crs="EPSG:28992")
 
-
 @pytest.fixture
-@mock.patch("openspoor.transformers.TransformerCoordinatesToSpoor._get_spoortak_met_geokm")
-def coordinates_transformer(mocked_load):
-    mocked_load.return_value = mock_spoordata_gdf
+def coordinates_transformer(monkeypatch):
+    monkeypatch.setattr(TransformerCoordinatesToSpoor, '_get_spoortak_met_geokm', lambda d: mock_spoordata_gdf)
     return TransformerCoordinatesToSpoor()
 
 
 class Test:
     spoortak_mock_output = mock_spoordata_gdf
 
     puic_mock_output = gpd.GeoDataFrame(
@@ -149,62 +147,52 @@
                         (146837.78700000048, 430114.2259999998), (146887.78599999845, 430114.4210000001),
                         (146917.56799999997, 430114.38899999857), (146954.33300000057, 430114.1770000011),
                         (146985.48299999908, 430113.8579999991), (147030.68100000173, 430113.1460000016),
                         (147257.83199999854, 430108.6009999998), ]), ],
         crs="epsg:28992",
     )
 
-    @mock.patch("openspoor.mapservices.MapServicesQuery._load_all_features_to_gdf")
-    def test_caching_singlequery(self, mocked_load, tmp_path):
-        mocked_load.return_value = self.spoortak_mock_output
+    def test_singlequery(self, monkeypatch, tmp_path):     
+        monkeypatch.setattr("openspoor.mapservices.MapServicesQuery._load_all_features_to_gdf", lambda d: self.spoortak_mock_output)
         cache_path = tmp_path / "spoortak.p"
 
         assert ~os.path.exists(cache_path)
         spoortak_mapservices = MapServicesQuery(url=config['spoor_url'], cache_location=cache_path)
-
-        spoortak_mapservices.load_data()
-        assert os.path.exists(cache_path)
-
-        # Load a second time to actually use cached file
         output = spoortak_mapservices.load_data()
+        assert os.path.exists(cache_path)
 
         expected_output = self.spoortak_mock_output
 
         pd.testing.assert_frame_equal(
             pd.DataFrame(output.drop(columns="geometry")),
             pd.DataFrame(expected_output.drop(columns="geometry")),
         )
         assert all(output.geometry.geom_almost_equals(expected_output.geometry, 6))
 
-    @mock.patch("openspoor.mapservices.MapServicesQuery._load_all_features_to_gdf")
-    def test_caching_puicmapservices(self, mocked_load, tmp_path):
-        mocked_load.return_value = self.puic_mock_output
+    def test_puicmapservices(self, monkeypatch, tmp_path):
+        monkeypatch.setattr("openspoor.mapservices.MapServicesQuery._load_all_features_to_gdf", lambda d: self.puic_mock_output)
         cache_path = tmp_path / "puic.p"
 
         assert ~os.path.exists(cache_path)
         puic_mapservices = PUICMapservices(spoor_cache_location=cache_path,
                                            wisselkruisingbeen_cache_location=cache_path)
-        puic_mapservices.spoor_query.load_data()
-        assert os.path.exists(cache_path)
-
-        # Load a second time to actually use cached file
         output = puic_mapservices.spoor_query.load_data()
 
         expected_output = self.puic_mock_output
 
         pd.testing.assert_frame_equal(
             pd.DataFrame(output.drop(columns="geometry")),
             pd.DataFrame(expected_output.drop(columns="geometry")),
         )
         assert all(output.geometry.geom_almost_equals(expected_output.geometry, 6))
 
     def test_acceptance_TransformerCoordinatesToSpoor(self, coordinates_transformer):
         xy_test_df = pd.DataFrame(
             {
-                "x": [
+                "x": [                    
                     112734.526,
                     112734.526,
                     112732.526,
                     112679.485,
                     95659.5,
                     0,
                     95648.723,
@@ -354,15 +342,15 @@
                 ]
             ]
         )
 
         expected_output_df["x"] = gps_test_gdf["x"]
         expected_output_df["y"] = gps_test_gdf["y"]
         pd.testing.assert_frame_equal(
-            output_df, expected_output_df, check_less_precise=3
+            output_df, expected_output_df, atol=0.05
         )
 
     def test_acceptance_TransformerCoordinatesToSpoor_intersecting_tracks(self, coordinates_transformer):
         x_coord, y_coord = 96070, 450383
         points_df = pd.DataFrame({"x": [x_coord], "y": [y_coord]})
         points_gdf = gpd.GeoDataFrame(
             points_df,
@@ -397,15 +385,15 @@
                                            "GEOSUBCODE": ["107__", "166__"],
                                            "PRORAIL_GEBIED": ["Zuid-Holland Noord", "Zuid-Holland Zuid"],
                                            "geocode_kilometrering": [10.239600, 115.515389],
                                        }
                                        )
 
         pd.testing.assert_frame_equal(output_df.sort_values(['NAAM_LANG']),
-                                      expected_output.sort_values(['NAAM_LANG']), check_less_precise=3)
+                                      expected_output.sort_values(['NAAM_LANG']), atol=1e-3)
 
     def test_acceptance_TransformerGeocodeToCoordinates(self):
         geocode_transformer = TransformerGeocodeToCoordinates(
             geocode_column="Geocode",
             geocode_km_column="geocode_km",
             coordinate_system="Rijksdriehoek",
         )
@@ -441,15 +429,15 @@
                     534190.950,
                     534204.614,
                 ],
             },
             index=pd.Series([66, 11, 55, 44, 33, 22], name="Indexname"),
         )
 
-        pd.testing.assert_frame_equal(output, output_expected, check_less_precise=2)
+        pd.testing.assert_frame_equal(output, output_expected, atol=1e-2)
 
     def test_acceptance_TransformerSpoortakToCoordinates(self):
         spoortak_transformer = TransformerSpoortakToCoordinates(
             "SPOOR_ID", "lokale_kilometrering", coordinate_system="Rijksdriehoek"
         )
         spoortak_transformer = spoortak_transformer.fit(self.spoortak_mock_output)
         input_df = pd.DataFrame(
```

### Comparing `openspoor-0.2.4/tests/test_MapservicesData.py` & `openspoor-0.2.5/tests/test_MapservicesData.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/tests/test_PUICMapservices.py` & `openspoor-0.2.5/tests/test_PUICMapservices.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/tests/test_TransformerCoordinatesToSpoor.py` & `openspoor-0.2.5/tests/test_TransformerCoordinatesToSpoor.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,30 +46,29 @@
     return gpd.GeoDataFrame({'pointname': ['P', 'Q']},
                             crs='EPSG:28992',
                             index=[0, 1],
                             geometry=[Point(-0.5, 0),  # Should be in next segment
                                       Point(0, 30.5)])  # Should be in another segment
 
 
-@mock.patch("openspoor.transformers.TransformerCoordinatesToSpoor._get_spoortak_met_geokm")
-def test_transform(mocked_load, points_gdf, lines_gdf):
-    mocked_load.return_value = lines_gdf
-
-    out = TransformerCoordinatesToSpoor().transform(points_gdf)
+def test_transform(monkeypatch, points_gdf, lines_gdf):
+    
+    monkeypatch.setattr(TransformerCoordinatesToSpoor, '_get_spoortak_met_geokm', lambda q: lines_gdf)
+    transformer = TransformerCoordinatesToSpoor()
+    out = transformer.transform(points_gdf)
+    # print(mock_transformer.stgk)
 
     expected_out = pd.concat([points_gdf, points_gdf.iloc[2:, :]])
     for col in ['linename', 'GEOCODE', 'SUBCODE', 'NAAM_LANG', 'KM_GEOCODE_VAN', 'KM_GEOCODE_TOT']:
         expected_out[col] = list(lines_gdf[col].values) * 2
     expected_out['geocode_kilometrering'] = [26.0, 8.0, 35.0, 5.0]
     pd.testing.assert_frame_equal(out, expected_out)
-
-
-@mock.patch("openspoor.transformers.TransformerCoordinatesToSpoor._get_spoortak_met_geokm")
-def test_transform_far_points(mocked_load, far_points_gdf, lines_gdf):
-    mocked_load.return_value = lines_gdf
+    
+def test_transform_far_points(monkeypatch, far_points_gdf, lines_gdf):    
+    monkeypatch.setattr(TransformerCoordinatesToSpoor, '_get_spoortak_met_geokm', lambda q: lines_gdf)
 
     out = TransformerCoordinatesToSpoor().transform(far_points_gdf)
 
     expected_out = far_points_gdf
     for col in ['linename', 'GEOCODE', 'SUBCODE', 'NAAM_LANG']:
         expected_out[col] = [None] * 2
     for col in ['KM_GEOCODE_VAN', 'KM_GEOCODE_TOT', 'geocode_kilometrering']:
```

### Comparing `openspoor-0.2.4/tests/test_TransformerGeocodeToCoordinates.py` & `openspoor-0.2.5/tests/test_TransformerGeocodeToCoordinates.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/tests/test_TransformerSpoortakToCoordinates.py` & `openspoor-0.2.5/tests/test_TransformerSpoortakToCoordinates.py`

 * *Files identical despite different names*

### Comparing `openspoor-0.2.4/tests/test_find_mapservice.py` & `openspoor-0.2.5/tests/test_find_mapservice.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
-from unittest import mock
 import pandas as pd
 import geopandas as gpd
 from glob import glob
+from geopandas.testing import assert_geodataframe_equal
 
 from shapely.geometry import Point
 from pathlib import Path
 
 from openspoor.mapservices import FeatureServerOverview, FeatureSearchResults
 
 
@@ -61,22 +61,18 @@
     spoortak_mock_output = gpd.GeoDataFrame({'example_col': [1, 2, 3],
                                              },
                                             geometry=[Point(112734.52699999884, 480849.4979999997),
                                                       Point(112679.4849999994, 480767.1550000012),
                                                       Point(112622.47399999946, 480681.72399999946)],
                                             crs="epsg:28992")
 
-    @mock.patch("openspoor.mapservices.MapServicesQuery._load_all_features_to_gdf")
-    def test_FeatureSearchResults(self, mocked_load, search_results, tmpdir):
+    def test_FeatureSearchResults(self, monkeypatch, search_results, tmpdir):
+        monkeypatch.setattr("openspoor.mapservices.MapServicesQuery._load_all_features_to_gdf", lambda d: self.spoortak_mock_output)
         out_gdf = FeatureSearchResults(search_results).load_data(0)
-        gpd.testing.assert_geodataframe_equal(out_gdf, mocked_load), 'Incorrecting loading of data'
-
-    @mock.patch("openspoor.mapservices.MapServicesQuery._load_all_features_to_gdf")
-    def test_FeatureSearchResults(self, mocked_load, search_results, tmpdir):
-        mocked_load.return_value = self.spoortak_mock_output
+        assert_geodataframe_equal(out_gdf, self.spoortak_mock_output), 'Incorrecting loading of data'
 
         output_dir = Path(tmpdir) / 'outputs'
         FeatureSearchResults(search_results).write_gpkg(output_dir, 0)
 
         files = glob(str(output_dir) + "/**")
         assert len(files) == 1, 'A file was written'
         assert gpd.read_file(files[0]).shape == (3, 2), 'Incorrect shape'
```

