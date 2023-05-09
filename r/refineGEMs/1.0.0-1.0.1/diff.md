# Comparing `tmp/refineGEMs-1.0.0.tar.gz` & `tmp/refineGEMs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/baeuerle/Organisation/Masterarbeit/refinegems/dist/tmpMbltqQ/refineGEMs-1.0.0.tar", last modified: Thu May  4 12:05:30 2023, max compression
+gzip compressed data, was "refineGEMs-1.0.1.tar", last modified: Tue May  9 14:59:15 2023, max compression
```

## Comparing `refineGEMs-1.0.0.tar` & `refineGEMs-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-04 12:05:30.000000 refineGEMs-1.0.0/
--rw-r--r--   0 root         (0) staff       (20)      220 2023-05-04 12:05:30.000000 refineGEMs-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      140 2023-05-04 11:55:59.000000 refineGEMs-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-04 11:30:07.000000 refineGEMs-1.0.0/MANIFEST.in
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-04 12:05:30.000000 refineGEMs-1.0.0/refineGEMs.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      220 2023-05-04 12:05:30.000000 refineGEMs-1.0.0/refineGEMs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-04 12:05:30.000000 refineGEMs-1.0.0/refineGEMs.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)      719 2023-05-04 12:05:30.000000 refineGEMs-1.0.0/refineGEMs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)      292 2023-05-04 12:05:30.000000 refineGEMs-1.0.0/refineGEMs.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       11 2023-05-04 12:05:30.000000 refineGEMs-1.0.0/refineGEMs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-04 12:05:30.000000 refineGEMs-1.0.0/refineGEMs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)     2868 2023-05-04 11:41:21.000000 refineGEMs-1.0.0/README.md
--rw-r--r--   0 root         (0) staff       (20)      950 2023-05-04 12:00:25.000000 refineGEMs-1.0.0/setup.py
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-04 12:05:30.000000 refineGEMs-1.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-04 12:05:30.000000 refineGEMs-1.0.0/refinegems/
--rw-r--r--   0 root         (0) staff       (20)    12891 2023-05-04 09:57:20.000000 refineGEMs-1.0.0/refinegems/gapfill.py
--rw-r--r--   0 root         (0) staff       (20)     6328 2023-03-09 16:45:46.000000 refineGEMs-1.0.0/refinegems/analysis_kegg.py
--rw-r--r--   0 root         (0) staff       (20)     5672 2023-03-09 16:45:46.000000 refineGEMs-1.0.0/refinegems/curate.py
--rw-r--r--   0 root         (0) staff       (20)     9537 2023-03-09 16:45:46.000000 refineGEMs-1.0.0/refinegems/databases.py
--rw-r--r--   0 root         (0) staff       (20)       21 2023-05-04 11:31:53.000000 refineGEMs-1.0.0/refinegems/version.py
--rw-r--r--   0 root         (0) staff       (20)    14987 2023-05-04 09:57:20.000000 refineGEMs-1.0.0/refinegems/analysis_db.py
--rw-r--r--   0 root         (0) staff       (20)     7224 2023-05-04 10:24:25.000000 refineGEMs-1.0.0/refinegems/modelseed.py
--rw-r--r--   0 root         (0) staff       (20)    20824 2023-05-04 10:24:25.000000 refineGEMs-1.0.0/refinegems/io.py
--rw-r--r--   0 root         (0) staff       (20)     3167 2023-03-14 15:27:23.000000 refineGEMs-1.0.0/refinegems/charges.py
--rw-r--r--   0 root         (0) staff       (20)    22498 2023-05-04 10:24:25.000000 refineGEMs-1.0.0/refinegems/analysis_biocyc.py
--rw-r--r--   0 root         (0) staff       (20)      595 2023-05-04 11:40:57.000000 refineGEMs-1.0.0/refinegems/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    15225 2023-05-04 10:24:25.000000 refineGEMs-1.0.0/refinegems/growth.py
--rw-r--r--   0 root         (0) staff       (20)     7042 2023-05-04 10:24:25.000000 refineGEMs-1.0.0/refinegems/pathways.py
--rw-r--r--   0 root         (0) staff       (20)    10352 2023-05-04 10:24:25.000000 refineGEMs-1.0.0/refinegems/comparison.py
--rw-r--r--   0 root         (0) staff       (20)     8936 2023-03-09 16:45:46.000000 refineGEMs-1.0.0/refinegems/cvterms.py
--rw-r--r--   0 root         (0) staff       (20)    10350 2023-05-04 10:24:25.000000 refineGEMs-1.0.0/refinegems/entities.py
--rw-r--r--   0 root         (0) staff       (20)    41756 2023-05-04 10:24:25.000000 refineGEMs-1.0.0/refinegems/polish.py
--rw-r--r--   0 root         (0) staff       (20)    11765 2023-03-09 16:45:46.000000 refineGEMs-1.0.0/refinegems/investigate.py
--rw-r--r--   0 root         (0) staff       (20)    23740 2023-03-09 16:45:46.000000 refineGEMs-1.0.0/refinegems/sboann.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-04 12:05:30.000000 refineGEMs-1.0.0/data/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-04 12:05:30.000000 refineGEMs-1.0.0/data/database/
--rw-r--r--   0 root         (0) staff       (20)   353015 2023-05-04 10:24:25.000000 refineGEMs-1.0.0/data/database/sbo_media_db.sql
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 14:59:15.832120 refineGEMs-1.0.1/
+-rw-r--r--   0 root         (0) staff       (20)     1068 2022-05-04 13:39:38.000000 refineGEMs-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     3117 2023-05-09 14:59:15.831723 refineGEMs-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2735 2023-05-09 14:56:11.000000 refineGEMs-1.0.1/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 14:59:15.819773 refineGEMs-1.0.1/data/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 14:59:15.822757 refineGEMs-1.0.1/data/database/
+-rw-r--r--   0 root         (0) staff       (20)   353015 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/data/database/sbo_media_db.sql
+-rw-r--r--   0 root         (0) staff       (20)      140 2023-05-04 11:55:59.000000 refineGEMs-1.0.1/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 14:59:15.824968 refineGEMs-1.0.1/refineGEMs.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     3117 2023-05-09 14:59:15.000000 refineGEMs-1.0.1/refineGEMs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      693 2023-05-09 14:59:15.000000 refineGEMs-1.0.1/refineGEMs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-09 14:59:15.000000 refineGEMs-1.0.1/refineGEMs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-04 12:05:30.000000 refineGEMs-1.0.1/refineGEMs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)      292 2023-05-09 14:59:15.000000 refineGEMs-1.0.1/refineGEMs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       11 2023-05-09 14:59:15.000000 refineGEMs-1.0.1/refineGEMs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 14:59:15.831015 refineGEMs-1.0.1/refinegems/
+-rw-r--r--   0 root         (0) staff       (20)      595 2023-05-04 11:40:57.000000 refineGEMs-1.0.1/refinegems/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    22498 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/analysis_biocyc.py
+-rw-r--r--   0 root         (0) staff       (20)    14987 2023-05-04 09:57:20.000000 refineGEMs-1.0.1/refinegems/analysis_db.py
+-rw-r--r--   0 root         (0) staff       (20)     6328 2023-03-09 16:45:46.000000 refineGEMs-1.0.1/refinegems/analysis_kegg.py
+-rw-r--r--   0 root         (0) staff       (20)     3167 2023-03-14 15:27:23.000000 refineGEMs-1.0.1/refinegems/charges.py
+-rw-r--r--   0 root         (0) staff       (20)    10352 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/comparison.py
+-rw-r--r--   0 root         (0) staff       (20)     5672 2023-03-09 16:45:46.000000 refineGEMs-1.0.1/refinegems/curate.py
+-rw-r--r--   0 root         (0) staff       (20)     8936 2023-03-09 16:45:46.000000 refineGEMs-1.0.1/refinegems/cvterms.py
+-rw-r--r--   0 root         (0) staff       (20)     9537 2023-03-09 16:45:46.000000 refineGEMs-1.0.1/refinegems/databases.py
+-rw-r--r--   0 root         (0) staff       (20)    10350 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/entities.py
+-rw-r--r--   0 root         (0) staff       (20)    12891 2023-05-04 09:57:20.000000 refineGEMs-1.0.1/refinegems/gapfill.py
+-rw-r--r--   0 root         (0) staff       (20)    15225 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/growth.py
+-rw-r--r--   0 root         (0) staff       (20)    11765 2023-03-09 16:45:46.000000 refineGEMs-1.0.1/refinegems/investigate.py
+-rw-r--r--   0 root         (0) staff       (20)    20824 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/io.py
+-rw-r--r--   0 root         (0) staff       (20)     7224 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/modelseed.py
+-rw-r--r--   0 root         (0) staff       (20)     7042 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/pathways.py
+-rw-r--r--   0 root         (0) staff       (20)    41756 2023-05-04 10:24:25.000000 refineGEMs-1.0.1/refinegems/polish.py
+-rw-r--r--   0 root         (0) staff       (20)    23740 2023-03-09 16:45:46.000000 refineGEMs-1.0.1/refinegems/sboann.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-09 14:59:15.832211 refineGEMs-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1234 2023-05-09 14:59:04.000000 refineGEMs-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `refineGEMs-1.0.0/refineGEMs.egg-info/SOURCES.txt` & `refineGEMs-1.0.1/refineGEMs.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MANIFEST.in
+LICENSE
 README.md
 pyproject.toml
 setup.py
 data/database/sbo_media_db.sql
 refineGEMs.egg-info/PKG-INFO
 refineGEMs.egg-info/SOURCES.txt
 refineGEMs.egg-info/dependency_links.txt
@@ -22,9 +22,8 @@
 refinegems/gapfill.py
 refinegems/growth.py
 refinegems/investigate.py
 refinegems/io.py
 refinegems/modelseed.py
 refinegems/pathways.py
 refinegems/polish.py
-refinegems/sboann.py
-refinegems/version.py
+refinegems/sboann.py
```

### Comparing `refineGEMs-1.0.0/README.md` & `refineGEMs-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,29 @@
-[![DOI](https://zenodo.org/badge/359867657.svg)](https://zenodo.org/badge/latestdoi/359867657) [![Update Docs](https://github.com/draeger-lab/refinegems/actions/workflows/docs.yml/badge.svg)](https://github.com/draeger-lab/refinegems/actions/workflows/docs.yml) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+Metadata-Version: 2.1
+Name: refineGEMs
+Version: 1.0.1
+Summary: refineGEMs is a python package inteded to help with the curation of genome-scale metabolic models (GEMS)
+Home-page: https://github.com/draeger-lab/refinegems
+Author: Famke Baeuerle and Gwendolyn O. Gusak
+Author-email: famke.baeuerle@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7915766.svg)](https://doi.org/10.5281/zenodo.7915766) [![Documentation Status](https://readthedocs.org/projects/refinegems/badge/?version=latest)](https://refinegems.readthedocs.io/en/latest/?badge=latest) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 <p align="center">
-<img src="https://github.com/draeger-lab/refinegems/blob/4db6de15e0d780ac73223a907b0b92b39742cd86/docs/source/images/refineGEMs_logo.png" height="200"/>
+<img src="https://github.com/draeger-lab/refinegems/raw/main/docs/source/images/refineGEMs_logo.png" height="200"/>
 </p>
 
 # refineGEMs
 `refineGEMs` is a python package inteded to help with the curation of genome-scale metabolic models (GEMS).
 
 ## Documentation
-To access the documentation please enter `<path to refineGEMs>/refinegems/docs/build/html/index.html` into your favourite browser. As soon as the repository is made public this will be moved to a standalone website.
+The docs can be found [here](https://refinegems.readthedocs.io/en/latest/).
 
 ## Overview
 
 Currently `refineGEMs` can be used for the investigation of a GEM, it can complete the following tasks:
 - loading GEMS with `cobrapy` and `libSBML`
 - report number of metabolites, reactions and genes
 - report orphaned, deadends and disconnected metabolites
@@ -25,15 +36,22 @@
 - correction of a model created with [CarveMe](https://github.com/cdanielmachado/carveme) v.1.5.1 (for example moving all relevant information from the notes to the annotation field) this includes automated annotation of NCBI genes to the GeneProtein section of the model
 - addition of [KEGG](https://www.genome.jp/kegg/kegg1.html) Pathways as Groups (using the [libSBML](https://synonym.caltech.edu/software/libsbml/5.18.0/docs/formatted/python-api/classlibsbml_1_1_groups_model_plugin.html) Groups Plugin)
 - SBO-Term annotation based on a script by Elisabeth Fritze
 - annotation of metabolites based using a table created by the user `data/manual_annotations.xlsx`
 
 ## Installation
 
-`refineGEMs` is distributed via this github repository, all dependencies are denoted in the `setup.py` file which can be used to install refineGEMs to a local conda environment:
+You can install `refineGEMs` via pip:
+
+```bash
+pip install refinegems
+
+```
+
+or to a local conda environment where `refineGEMs` is distributed via this github repository and all dependencies are denoted in the `setup.py` file:
 
 ```bash
 # clone or pull the latest source code
 git clone https://github.com/draeger-lab/refinegems.git
 cd refinegems
 
 conda create -n <EnvName> python=3.9
```

### Comparing `refineGEMs-1.0.0/setup.py` & `refineGEMs-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # needed for installation of refinegems
 from setuptools import setup
 
+with open('README.md') as readme_file:
+    readme = readme_file.read()
+
 setup(name='refineGEMs',
-      version='1.0.0',
-      description='Scripts to curate a GEM',
-      author='Famke Baeuerle',
+      version='1.0.1',
+      description='refineGEMs is a python package inteded to help with the curation of genome-scale metabolic models (GEMS)',
+      long_description=readme,
+      long_description_content_type='text/markdown',
+      author='Famke Baeuerle and Gwendolyn O. Gusak',
       author_email='famke.baeuerle@gmail.com',
+      url='https://github.com/draeger-lab/refinegems',
       license='MIT',
       packages=['refinegems'],
       install_requires = [
             "cobra==0.22.0",
             "biopython==1.79",
             "bioservices",
             "memote==0.13.0",
             "pandas==1.2.4",
             "numpy==1.20.3",
-            # "pyyaml==5.4.1",
             "gffutils==0.10.1",
             "markupsafe==2.0.1", 
             "depinfo==1.7.0",
             "sortedcontainers==2.4.0",
             "libchebipy==1.0.10",
             "ratelimit==2.2.1",
             "sqlalchemy==1.4.43",
```

### Comparing `refineGEMs-1.0.0/refinegems/gapfill.py` & `refineGEMs-1.0.1/refinegems/gapfill.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/analysis_kegg.py` & `refineGEMs-1.0.1/refinegems/analysis_kegg.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/curate.py` & `refineGEMs-1.0.1/refinegems/curate.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/databases.py` & `refineGEMs-1.0.1/refinegems/databases.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/analysis_db.py` & `refineGEMs-1.0.1/refinegems/analysis_db.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/modelseed.py` & `refineGEMs-1.0.1/refinegems/modelseed.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/io.py` & `refineGEMs-1.0.1/refinegems/io.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/charges.py` & `refineGEMs-1.0.1/refinegems/charges.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/analysis_biocyc.py` & `refineGEMs-1.0.1/refinegems/analysis_biocyc.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/__init__.py` & `refineGEMs-1.0.1/refinegems/__init__.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/growth.py` & `refineGEMs-1.0.1/refinegems/growth.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/pathways.py` & `refineGEMs-1.0.1/refinegems/pathways.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/comparison.py` & `refineGEMs-1.0.1/refinegems/comparison.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/cvterms.py` & `refineGEMs-1.0.1/refinegems/cvterms.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/entities.py` & `refineGEMs-1.0.1/refinegems/entities.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/polish.py` & `refineGEMs-1.0.1/refinegems/polish.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/investigate.py` & `refineGEMs-1.0.1/refinegems/investigate.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/refinegems/sboann.py` & `refineGEMs-1.0.1/refinegems/sboann.py`

 * *Files identical despite different names*

### Comparing `refineGEMs-1.0.0/data/database/sbo_media_db.sql` & `refineGEMs-1.0.1/data/database/sbo_media_db.sql`

 * *Files identical despite different names*

