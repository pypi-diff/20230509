# Comparing `tmp/teemi-0.1.3.tar.gz` & `tmp/teemi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teemi-0.1.3.tar", last modified: Thu Apr 13 13:38:43 2023, max compression
+gzip compressed data, was "teemi-0.1.4.tar", last modified: Tue May  9 07:33:09 2023, max compression
```

## Comparing `teemi-0.1.3.tar` & `teemi-0.1.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:38:43.855134 teemi-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-13 13:37:33.000000 teemi-0.1.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 13:37:33.000000 teemi-0.1.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-13 13:37:33.000000 teemi-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 13:37:33.000000 teemi-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-04-13 13:38:43.855134 teemi-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-13 13:37:33.000000 teemi-0.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-13 13:38:43.855134 teemi-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-13 13:37:33.000000 teemi-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:38:43.855134 teemi-0.1.3/teemi/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 13:38:43.855134 teemi-0.1.3/teemi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:38:43.855134 teemi-0.1.3/teemi/build/
--rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/build/PCR.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30079 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/build/containers_wells_picklists.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/build/robot_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/build/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:38:43.855134 teemi-0.1.3/teemi/design/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/design/cloning.py
--rw-r--r--   0 runner    (1001) docker     (123)    24971 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/design/combinatorial_design.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/design/fetch_sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/design/retrieve_gene_homologs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/design/teselagen_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:38:43.855134 teemi-0.1.3/teemi/learn/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/learn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/learn/auto_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    21864 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/learn/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:38:43.855134 teemi-0.1.3/teemi/lims/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/lims/benchling_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/lims/csv_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:38:43.855134 teemi-0.1.3/teemi/test/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/test/genotyping.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-13 13:37:33.000000 teemi-0.1.3/teemi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:38:43.855134 teemi-0.1.3/teemi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-04-13 13:38:43.000000 teemi-0.1.3/teemi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-13 13:38:43.000000 teemi-0.1.3/teemi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:38:43.000000 teemi-0.1.3/teemi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-13 13:38:43.000000 teemi-0.1.3/teemi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:38:43.000000 teemi-0.1.3/teemi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-13 13:38:43.000000 teemi-0.1.3/teemi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 13:38:43.000000 teemi-0.1.3/teemi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-13 13:37:33.000000 teemi-0.1.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.938116 teemi-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-09 07:31:59.000000 teemi-0.1.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-09 07:31:59.000000 teemi-0.1.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-09 07:31:59.000000 teemi-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 07:31:59.000000 teemi-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-05-09 07:33:09.938116 teemi-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10602 2023-05-09 07:31:59.000000 teemi-0.1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-09 07:33:09.938116 teemi-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-09 07:31:59.000000 teemi-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.938116 teemi-0.1.4/teemi/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 07:33:09.938116 teemi-0.1.4/teemi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.934116 teemi-0.1.4/teemi/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/build/PCR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30079 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/build/containers_wells_picklists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/build/robot_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/build/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.938116 teemi-0.1.4/teemi/design/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/design/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24971 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/design/combinatorial_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/design/fetch_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/design/retrieve_gene_homologs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/design/teselagen_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.938116 teemi-0.1.4/teemi/learn/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/learn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/learn/auto_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/learn/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.938116 teemi-0.1.4/teemi/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/lims/benchling_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/lims/csv_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.938116 teemi-0.1.4/teemi/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/test/genotyping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.934116 teemi-0.1.4/teemi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-09 07:31:59.000000 teemi-0.1.4/versioneer.py
```

### Comparing `teemi-0.1.3/LICENSE` & `teemi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/PKG-INFO` & `teemi-0.1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,320 +1,346 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: teemi
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for constructing microbial strains
 Home-page: https://github.com/hiyama341/teemi
 Author: Lucas Levassor
 Author-email: lucaslevassor@gmail.com
 License: MIT license
-Description: .. image:: https://raw.githubusercontent.com/hiyama341/teemi/main/pictures/teemi_logo.svg
-          :width: 400
-          :alt: teemi logo 
-        
-        teemi: a python package designed to make HT strain construction reproducible and FAIR
-        -------------------------------------------------------------------------------------
-        
-        .. summary-start
-        
-        .. image:: https://badge.fury.io/py/teemi.svg
-                :target: https://badge.fury.io/py/teemi
-        
-        .. image:: https://github.com/hiyama341/teemi/actions/workflows/main.yml/badge.svg
-                :target: https://github.com/hiyama341/teemi/actions
-        
-        .. image:: https://readthedocs.org/projects/teemi/badge/?version=latest
-                :target: https://teemi.readthedocs.io/en/latest/?version=latest
-                :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/github/license/hiyama341/teemi
-                :target: https://github.com/hiyama341/teemi/blob/main/LICENSE
-        
-        .. image:: https://img.shields.io/pypi/pyversions/teemi.svg
-                :target: https://pypi.org/project/teemi/
-                :alt: Supported Python Versions
-        
-        .. image:: https://codecov.io/gh/hiyama341/teemi/branch/main/graph/badge.svg?token=P4457QACUY 
-                :target: https://codecov.io/gh/hiyama341/teemi
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-black
-                :target: https://black.readthedocs.io/en/stable/
-        
-        .. image:: https://img.shields.io/github/last-commit/hiyama341/teemi
-        
-        
-        
-        What is teemi?
-        ~~~~~~~~~~~~~~
-        
-        **teemi**, named after the Greek goddess of fairness, is a python package designed
-        to make microbial strain construction reproducible and FAIR (Findable, Accessible, 
-        Interoperable, and Reusable). With teemi, you can simulate all steps of 
-        a strain construction cycle, from generating genetic parts to designing 
-        a combinatorial library and keeping track of samples through a commercial
-        Benchling API and a low-level CSV file database. 
-        This tool can be used in literate programming to 
-        increase efficiency and speed in metabolic engineering tasks. 
-        To try teemi, visit our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__.
-        
-        
-        teemi not only simplifies the strain construction process but also offers the 
-        flexibility to adapt to different experimental workflows through its open-source
-        Python platform. This allows for efficient automation of repetitive tasks and
-        a faster pace in metabolic engineering.
-        
-        Our demonstration of teemi in a complex machine learning-guided
-        metabolic engineering task showcases its efficiency 
-        and speed by debottlenecking a crucial step in the strictosidine pathway. 
-        This highlights the versatility and usefulness of this tool in various  
-        biological applications. 
-        
-        Curious about how you can build strains easier and faster with teemi? 
-        Head over to our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__
-        and give it a try.
-        
-        Please cite our paper (in preparation - link tba) if you've used teemi in a scientific publication.
-        
-        .. summary-end
-        
-        
-        Features
-        --------
-        
-        * Combinatorial library generation
-        * HT cloning and transformation workflows
-        * Flowbot One instructions
-        * CSV-based LIMS system as well as integration to Benchling
-        * Genotyping of microbial strains
-        * Advanced Machine Learning of biological datasets with the AutoML `H2O <https://docs.h2o.ai/h2o/latest-stable/h2o-docs/automl.html>`__
-        * Workflows for selecting enzyme homologs
-        * Promoter selection workflows from RNA-seq datasets
-        * Data analysis of large LC-MS datasets along with workflows for analysis
-        
-        
-        Getting started
-        ~~~~~~~~~~~~~~~
-        To get started with making microbial strains in an HT manner please follow the steps below: 
-        
-        1. Install teemi. You will find the necessary information below for installation.
-        
-        2. Check out our `notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__ for inspiration to make HT strain construction with teemi.
-        
-        3. You can start making your own workflows by importing teemi into either Google colab or Jupyter lab/notebooks.
-        
-        
-        Colab notebooks
-        ---------------
-        As a proof of concept we show how teemi and literate programming can be used to streamline bioengineering workflows.
-        These workflows should serve as a guide or a help to build your own workflows and thereby harnessing the power of literate programming with teemi. 
-        
-        Specifically, in this study we present how teemi and literate programming to build simulation-guided, iterative,
-        and evolution-guided laboratory workflows for optimizing strictosidine production in yeast.
-        
-        Below you can find all the notebooks developed in this work. 
-        Just click the Google colab badge to start the workflows. 
-        
-        Strictosidine case : First DBTL cycle
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        **DESIGN:**
-        
-        ..  |Notebook 00| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 00
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/00_1_DESIGN_Homologs.ipynb 
-        
-        ..  |Notebook 01| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 01
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/01_1_DESIGN_Promoters.ipynb
-        
-        ..  |Notebook 02| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 02
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/02_1_DESIGN_Combinatorial_library.ipynb
-            
-        
-        00. Automatically fetch homologs from NCBI from a query in a standardizable and repeatable way |Notebook 00| 
-        
-        
-        01. Promoters can be selected from RNAseq data and fetched from online database with various quality measurements implemented |Notebook 01|
-        
-        
-        
-        02. Combinatorial libraries can be generated with the DesignAssembly class along with robot executable intructions |Notebook 02| 
-        
-        
-        
-        
-        **BUILD:**
-        
-        ..  |Notebook 03| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 03
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/03_1_BUILD_USER_gRNA_plasmid.ipynb
-        
-        
-        ..  |Notebook 04| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 04
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/04_1_BUILD_Background_strain.ipynb
-        
-        
-        ..  |Notebook 05| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 05
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/05_1_BUILD_CombinatorialLibrary_AllStrains.ipynb
-        
-        
-        03. Assembly of a CRISPR plasmid with USER cloning |Notebook 03|
-        
-        04. Construction of the background strain by K/O of G8H and CPR |Notebook 04|
-        
-        05. First combinatorial library was generated for 1280 possible combinations |Notebook 05| 
-        
-        
-        
-        **TEST:**
-        
-        
-        ..  |Notebook 06| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 06
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/06_1_TEST_LibraryCharacterisation.ipynb
-        
-        
-        06. Data processing of LC-MS data and genotyping of the generated strains |Notebook 06|  
-        
-        
-        **LEARN:**
-        
-        ..  |Notebook 07| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 07
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/07_1_LEARN_DataAnalysis.ipynb
-        
-        
-        07. Use AutoML to predict the best combinations for a targeted second round of library construction |Notebook 07|
-        
-        
-        
-        Strictosidine case : Second DBTL cycle
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        
-        
-        **DESIGN:**
-        
-        ..  |Notebook 08| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 08
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_BUILD_Library2.ipynb
-        
-        08. Results from the ML can be translated into making a targeted library of strains |Notebook 08| 
-        
-        
-        
-        **BUILD:**
-        
-        
-        ..  |Notebook 09| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 09
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_2_BUILD_CombinatorialLibrary.ipynb
-        
-        
-        09. Shows the construction of a targeted library of strains |Notebook 09| 
-        
-        
-        
-        
-        **TEST:**
-        
-        ..  |Notebook 10| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 10
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/10_2_TEST_Library_Characterization.ipynb
-        
-        
-        
-        10. Data processing of LC-MS data like in notebook 6 |Notebook 10|
-        
-        
-        
-        
-        **LEARN:**
-        
-        ..  |Notebook 11| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 11
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/11_2_LEARN_DataAnalysisML.ipynb
-        
-        
-        11. Second ML cycle of ML showing how the model increased performance and saturation of best performing strains |Notebook 11| 
-        
-        
-        
-        Installation
-        ~~~~~~~~~~~~
-        
-        .. installation-start
-        
-        Use pip to install teemi from `PyPI <https://pypi.org/project/teemi/>`__.
-        
-        ::
-        
-            $ pip install teemi
-        
-        
-        If you want to develop or if you cloned the repository from our `GitHub <https://github.com/hiyama341/teemi/>`__
-        you can install teemi in the following way.
-        
-        ::
-        
-            $ pip install -e <path-to-teemi-repo>  
-        
-        
-        You might need to run these commands with administrative
-        privileges if you're not using a virtual environment (using ``sudo`` for example).
-        Please check the `documentation <https://teemi.readthedocs.io/en/latest/installation.html#>`__
-        for further details.
-        
-        .. installation-end
-        
-        Documentation and Examples
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Documentation is available on through numerous Google Colab notebooks with
-        examples on how to use teemi and how we use these notebooks for strain
-        construnction. The Colab notebooks can be found here 
-        `teemi.notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__. 
-        
-        * Documentation: https://teemi.readthedocs.io.
-        
-        
-        Contributions
-        ~~~~~~~~~~~~~
-        
-        Contributions are very welcome! Check our `guidelines <https://teemi.readthedocs.io/en/latest/contributing.html>`__ for instructions how to contribute.
-        
-        
-        License
-        ~~~~~~~
-        * Free software: MIT license
-        
-        Credits
-        -------
-        - This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        - teemis logo was made by Jonas Krogh Fischer. Check out his `website <http://jkfischerproductions.com/kea/portfolio/index.html>`__. 
-        
-        History
-        -------
-        
-        0.1.0 (2023-01-02)
-        ------------------
-        
-        * First release on PyPI.
 Keywords: teemi
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+.. image:: https://raw.githubusercontent.com/hiyama341/teemi/main/pictures/teemi_logo.svg
+  :width: 400
+  :alt: teemi logo 
+
+teemi: a python package designed to make HT strain construction reproducible and FAIR
+-------------------------------------------------------------------------------------
+
+.. summary-start
+
+.. image:: https://badge.fury.io/py/teemi.svg
+        :target: https://badge.fury.io/py/teemi
+
+.. image:: https://github.com/hiyama341/teemi/actions/workflows/main.yml/badge.svg
+        :target: https://github.com/hiyama341/teemi/actions
+
+.. image:: https://readthedocs.org/projects/teemi/badge/?version=latest
+        :target: https://teemi.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+.. image:: https://img.shields.io/github/license/hiyama341/teemi
+        :target: https://github.com/hiyama341/teemi/blob/main/LICENSE
+
+.. image:: https://img.shields.io/pypi/pyversions/teemi.svg
+        :target: https://pypi.org/project/teemi/
+        :alt: Supported Python Versions
+
+.. image:: https://codecov.io/gh/hiyama341/teemi/branch/main/graph/badge.svg?token=P4457QACUY 
+        :target: https://codecov.io/gh/hiyama341/teemi
+
+.. image:: https://img.shields.io/badge/code%20style-black-black
+        :target: https://black.readthedocs.io/en/stable/
+
+.. image:: https://img.shields.io/github/last-commit/hiyama341/teemi
+
+
+
+What is teemi?
+~~~~~~~~~~~~~~
+
+**teemi**, named after the Greek goddess of fairness, is a python package designed
+to make microbial strain construction reproducible and FAIR (Findable, Accessible, 
+Interoperable, and Reusable). With teemi, you can simulate all steps of 
+a strain construction cycle, from generating genetic parts to designing 
+a combinatorial library and keeping track of samples through a commercial
+Benchling API and a low-level CSV file database. 
+This tool can be used in literate programming to 
+increase efficiency and speed in metabolic engineering tasks. 
+To try teemi, visit our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__.
+
+
+teemi not only simplifies the strain construction process but also offers the 
+flexibility to adapt to different experimental workflows through its open-source
+Python platform. This allows for efficient automation of repetitive tasks and
+a faster pace in metabolic engineering.
+
+Our demonstration of teemi in a complex machine learning-guided
+metabolic engineering task showcases its efficiency 
+and speed by debottlenecking a crucial step in the strictosidine pathway. 
+This highlights the versatility and usefulness of this tool in various  
+biological applications. 
+
+Curious about how you can build strains easier and faster with teemi? 
+Head over to our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__
+and give it a try.
+
+Please cite our paper (in preparation - link tba) if you've used teemi in a scientific publication.
+
+.. summary-end
+
+
+Features
+--------
+
+* Combinatorial library generation
+* HT cloning and transformation workflows
+* Flowbot One instructions
+* CSV-based LIMS system as well as integration to Benchling
+* Genotyping of microbial strains
+* Advanced Machine Learning of biological datasets with the AutoML `H2O <https://docs.h2o.ai/h2o/latest-stable/h2o-docs/automl.html>`__
+* Workflows for selecting enzyme homologs
+* Promoter selection workflows from RNA-seq datasets
+* Data analysis of large LC-MS datasets along with workflows for analysis
+
+
+Getting started
+~~~~~~~~~~~~~~~
+To get started with making microbial strains in an HT manner please follow the steps below: 
+
+1. Install teemi. You will find the necessary information below for installation.
+
+2. Check out our `notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__ for inspiration to make HT strain construction with teemi.
+
+3. You can start making your own workflows by importing teemi into either Google colab or Jupyter lab/notebooks.
+
+
+Colab notebooks
+---------------
+As a proof of concept we show how teemi and literate programming can be used to streamline bioengineering workflows.
+These workflows should serve as a guide or a help to build your own workflows and thereby harnessing the power of literate programming with teemi. 
+
+Specifically, in this study we present how teemi and literate programming to build simulation-guided, iterative,
+and evolution-guided laboratory workflows for optimizing strictosidine production in yeast.
+
+Below you can find all the notebooks developed in this work. 
+Just click the Google colab badge to start the workflows. 
+
+Strictosidine case : First DBTL cycle
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+**DESIGN:**
+
+..  |Notebook 00| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 00
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/00_1_DESIGN_Homologs.ipynb 
+
+..  |Notebook 01| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 01
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/01_1_DESIGN_Promoters.ipynb
+
+..  |Notebook 02| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 02
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/02_1_DESIGN_Combinatorial_library.ipynb
+    
+
+00. Automatically fetch homologs from NCBI from a query in a standardizable and repeatable way 
+
+|Notebook 00| 
+
+
+01. Promoters can be selected from RNAseq data and fetched from online database with various quality measurements implemented 
+
+|Notebook 01|
+
+
+
+02. Combinatorial libraries can be generated with the DesignAssembly class along with robot executable intructions 
+
+|Notebook 02| 
+
+
+
+
+**BUILD:**
+
+..  |Notebook 03| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 03
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/03_1_BUILD_USER_gRNA_plasmid.ipynb
+
+
+..  |Notebook 04| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 04
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/04_1_BUILD_Background_strain.ipynb
+
+
+..  |Notebook 05| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 05
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/05_1_BUILD_CombinatorialLibrary_AllStrains.ipynb
+
+
+03. Assembly of a CRISPR plasmid with USER cloning 
+
+|Notebook 03|
+
+04. Construction of the background strain by K/O of G8H and CPR 
+
+|Notebook 04|
+
+05. First combinatorial library was generated for 1280 possible combinations 
+
+|Notebook 05| 
+
+
+
+**TEST:**
+
+
+..  |Notebook 06| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 06
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/06_1_TEST_LibraryCharacterisation.ipynb
+
+
+06. Data processing of LC-MS data and genotyping of the generated strains 
+
+|Notebook 06|  
+
+
+**LEARN:**
+
+..  |Notebook 07| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 07
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/07_1_LEARN_DataAnalysis.ipynb
+
+
+07. Use AutoML to predict the best combinations for a targeted second round of library construction 
+
+|Notebook 07|
+
+
+
+Strictosidine case : Second DBTL cycle
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+
+
+**DESIGN:**
+
+..  |Notebook 08| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 08
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_BUILD_Library2.ipynb
+
+08. Results from the ML can be translated into making a targeted library of strains 
+
+|Notebook 08| 
+
+
+
+**BUILD:**
+
+
+..  |Notebook 09| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 09
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_2_BUILD_CombinatorialLibrary.ipynb
+
+
+09. Shows the construction of a targeted library of strains 
+
+|Notebook 09| 
+
+
+
+
+**TEST:**
+
+..  |Notebook 10| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 10
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/10_2_TEST_Library_Characterization.ipynb
+
+
+
+10. Data processing of LC-MS data like in notebook 6 
+
+|Notebook 10|
+
+
+
+
+**LEARN:**
+
+..  |Notebook 11| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 11
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/11_2_LEARN_DataAnalysisML.ipynb
+
+
+11. Second ML cycle of ML showing how the model increased performance and saturation of best performing strains 
+
+|Notebook 11| 
+
+
+
+Installation
+~~~~~~~~~~~~
+
+.. installation-start
+
+Use pip to install teemi from `PyPI <https://pypi.org/project/teemi/>`__.
+
+::
+
+    $ pip install teemi
+
+
+If you want to develop or if you cloned the repository from our `GitHub <https://github.com/hiyama341/teemi/>`__
+you can install teemi in the following way.
+
+::
+
+    $ pip install -e <path-to-teemi-repo>  
+
+
+You might need to run these commands with administrative
+privileges if you're not using a virtual environment (using ``sudo`` for example).
+Please check the `documentation <https://teemi.readthedocs.io/en/latest/installation.html#>`__
+for further details.
+
+.. installation-end
+
+Documentation and Examples
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Documentation is available on through numerous Google Colab notebooks with
+examples on how to use teemi and how we use these notebooks for strain
+construnction. The Colab notebooks can be found here 
+`teemi.notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__. 
+
+* Documentation: https://teemi.readthedocs.io.
+
+
+Contributions
+~~~~~~~~~~~~~
+
+Contributions are very welcome! Check our `guidelines <https://teemi.readthedocs.io/en/latest/contributing.html>`__ for instructions how to contribute.
+
+
+License
+~~~~~~~
+* Free software: MIT license
+
+Credits
+-------
+- This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+- teemis logo was made by Jonas Krogh Fischer. Check out his `website <http://jkfischerproductions.com/kea/portfolio/index.html>`__. 
+
+History
+-------
+
+0.1.0 (2023-01-02)
+------------------
+
+* First release on PyPI.
```

### Comparing `teemi-0.1.3/README.rst` & `teemi-0.1.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -118,22 +118,28 @@
     :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/01_1_DESIGN_Promoters.ipynb
 
 ..  |Notebook 02| image:: https://colab.research.google.com/assets/colab-badge.svg
     :alt: Notebook 02
     :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/02_1_DESIGN_Combinatorial_library.ipynb
     
 
-00. Automatically fetch homologs from NCBI from a query in a standardizable and repeatable way |Notebook 00| 
+00. Automatically fetch homologs from NCBI from a query in a standardizable and repeatable way 
 
+|Notebook 00| 
 
-01. Promoters can be selected from RNAseq data and fetched from online database with various quality measurements implemented |Notebook 01|
 
+01. Promoters can be selected from RNAseq data and fetched from online database with various quality measurements implemented 
 
+|Notebook 01|
 
-02. Combinatorial libraries can be generated with the DesignAssembly class along with robot executable intructions |Notebook 02| 
+
+
+02. Combinatorial libraries can be generated with the DesignAssembly class along with robot executable intructions 
+
+|Notebook 02| 
 
 
 
 
 **BUILD:**
 
 ..  |Notebook 03| image:: https://colab.research.google.com/assets/colab-badge.svg
@@ -147,93 +153,111 @@
 
 
 ..  |Notebook 05| image:: https://colab.research.google.com/assets/colab-badge.svg
     :alt: Notebook 05
     :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/05_1_BUILD_CombinatorialLibrary_AllStrains.ipynb
 
 
-03. Assembly of a CRISPR plasmid with USER cloning |Notebook 03|
+03. Assembly of a CRISPR plasmid with USER cloning 
+
+|Notebook 03|
+
+04. Construction of the background strain by K/O of G8H and CPR 
+
+|Notebook 04|
 
-04. Construction of the background strain by K/O of G8H and CPR |Notebook 04|
+05. First combinatorial library was generated for 1280 possible combinations 
 
-05. First combinatorial library was generated for 1280 possible combinations |Notebook 05| 
+|Notebook 05| 
 
 
 
 **TEST:**
 
 
 ..  |Notebook 06| image:: https://colab.research.google.com/assets/colab-badge.svg
     :alt: Notebook 06
     :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/06_1_TEST_LibraryCharacterisation.ipynb
 
 
-06. Data processing of LC-MS data and genotyping of the generated strains |Notebook 06|  
+06. Data processing of LC-MS data and genotyping of the generated strains 
+
+|Notebook 06|  
 
 
 **LEARN:**
 
 ..  |Notebook 07| image:: https://colab.research.google.com/assets/colab-badge.svg
     :alt: Notebook 07
     :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/07_1_LEARN_DataAnalysis.ipynb
 
 
-07. Use AutoML to predict the best combinations for a targeted second round of library construction |Notebook 07|
+07. Use AutoML to predict the best combinations for a targeted second round of library construction 
+
+|Notebook 07|
 
 
 
 Strictosidine case : Second DBTL cycle
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 
 **DESIGN:**
 
 ..  |Notebook 08| image:: https://colab.research.google.com/assets/colab-badge.svg
     :alt: Notebook 08
     :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_BUILD_Library2.ipynb
 
-08. Results from the ML can be translated into making a targeted library of strains |Notebook 08| 
+08. Results from the ML can be translated into making a targeted library of strains 
+
+|Notebook 08| 
 
 
 
 **BUILD:**
 
 
 ..  |Notebook 09| image:: https://colab.research.google.com/assets/colab-badge.svg
     :alt: Notebook 09
     :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_2_BUILD_CombinatorialLibrary.ipynb
 
 
-09. Shows the construction of a targeted library of strains |Notebook 09| 
+09. Shows the construction of a targeted library of strains 
+
+|Notebook 09| 
 
 
 
 
 **TEST:**
 
 ..  |Notebook 10| image:: https://colab.research.google.com/assets/colab-badge.svg
     :alt: Notebook 10
     :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/10_2_TEST_Library_Characterization.ipynb
 
 
 
-10. Data processing of LC-MS data like in notebook 6 |Notebook 10|
+10. Data processing of LC-MS data like in notebook 6 
+
+|Notebook 10|
 
 
 
 
 **LEARN:**
 
 ..  |Notebook 11| image:: https://colab.research.google.com/assets/colab-badge.svg
     :alt: Notebook 11
     :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/11_2_LEARN_DataAnalysisML.ipynb
 
 
-11. Second ML cycle of ML showing how the model increased performance and saturation of best performing strains |Notebook 11| 
+11. Second ML cycle of ML showing how the model increased performance and saturation of best performing strains 
+
+|Notebook 11| 
 
 
 
 Installation
 ~~~~~~~~~~~~
 
 .. installation-start
```

### Comparing `teemi-0.1.3/setup.py` & `teemi-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/build/PCR.py` & `teemi-0.1.4/teemi/build/PCR.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/build/containers_wells_picklists.py` & `teemi-0.1.4/teemi/build/containers_wells_picklists.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/build/robot_assembly.py` & `teemi-0.1.4/teemi/build/robot_assembly.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/build/transformation.py` & `teemi-0.1.4/teemi/build/transformation.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/design/cloning.py` & `teemi-0.1.4/teemi/design/cloning.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/design/combinatorial_design.py` & `teemi-0.1.4/teemi/design/combinatorial_design.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/design/fetch_sequences.py` & `teemi-0.1.4/teemi/design/fetch_sequences.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/design/retrieve_gene_homologs.py` & `teemi-0.1.4/teemi/design/retrieve_gene_homologs.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/design/teselagen_helpers.py` & `teemi-0.1.4/teemi/design/teselagen_helpers.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/learn/auto_ml.py` & `teemi-0.1.4/teemi/learn/auto_ml.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/learn/plotting.py` & `teemi-0.1.4/teemi/learn/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     colorDict: dict,
     save_pdf=True,
     path="",
     xlabel="",
     ylabel="",
     size_height: int = 10,
     size_length: int = 20,
-    bar_width = 1.0
+    bar_width = 1.0, 
+    ylim = [0,25]
 ) -> None:
     """Plotting stacked barplots from a pandas dataframe cross tab df
 
     Parameters
     ----------
     pd_dataframe_cross_tab_prop : pd.DataFrames
         pd.crosstab
@@ -108,14 +109,15 @@
     cv_sd: list,
     save_pdf=True,
     path="",
     size_height: int = 10,
     size_length: int = 10,
     title = '', 
     linewidth:int = 1.5,
+    y_axis_range:list = [0,25]
 ) -> None:
     """Plotting a learning curve from partitioned dataframes.
 
     Parameters
     ----------
     x_partitioned_data : list
         x coordinates
@@ -185,14 +187,17 @@
     # Set color
     ax.set_facecolor("white")
 
     # SIze matters
     fig = mpl.pyplot.gcf()
     fig.set_size_inches(size_length,size_height)
 
+    # change y-axis range 
+    plt.ylim(y_axis_range)
+
     if save_pdf and path != "":
         ## save pdf
         plt.savefig(path + ".pdf", format="pdf", dpi=300, bbox_inches="tight")
 
     # show
     plt.show()
```

### Comparing `teemi-0.1.3/teemi/lims/benchling_api.py` & `teemi-0.1.4/teemi/lims/benchling_api.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/lims/csv_database.py` & `teemi-0.1.4/teemi/lims/csv_database.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/test/genotyping.py` & `teemi-0.1.4/teemi/test/genotyping.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi/utils.py` & `teemi-0.1.4/teemi/utils.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/teemi.egg-info/PKG-INFO` & `teemi-0.1.4/teemi.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,320 +1,346 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: teemi
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for constructing microbial strains
 Home-page: https://github.com/hiyama341/teemi
 Author: Lucas Levassor
 Author-email: lucaslevassor@gmail.com
 License: MIT license
-Description: .. image:: https://raw.githubusercontent.com/hiyama341/teemi/main/pictures/teemi_logo.svg
-          :width: 400
-          :alt: teemi logo 
-        
-        teemi: a python package designed to make HT strain construction reproducible and FAIR
-        -------------------------------------------------------------------------------------
-        
-        .. summary-start
-        
-        .. image:: https://badge.fury.io/py/teemi.svg
-                :target: https://badge.fury.io/py/teemi
-        
-        .. image:: https://github.com/hiyama341/teemi/actions/workflows/main.yml/badge.svg
-                :target: https://github.com/hiyama341/teemi/actions
-        
-        .. image:: https://readthedocs.org/projects/teemi/badge/?version=latest
-                :target: https://teemi.readthedocs.io/en/latest/?version=latest
-                :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/github/license/hiyama341/teemi
-                :target: https://github.com/hiyama341/teemi/blob/main/LICENSE
-        
-        .. image:: https://img.shields.io/pypi/pyversions/teemi.svg
-                :target: https://pypi.org/project/teemi/
-                :alt: Supported Python Versions
-        
-        .. image:: https://codecov.io/gh/hiyama341/teemi/branch/main/graph/badge.svg?token=P4457QACUY 
-                :target: https://codecov.io/gh/hiyama341/teemi
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-black
-                :target: https://black.readthedocs.io/en/stable/
-        
-        .. image:: https://img.shields.io/github/last-commit/hiyama341/teemi
-        
-        
-        
-        What is teemi?
-        ~~~~~~~~~~~~~~
-        
-        **teemi**, named after the Greek goddess of fairness, is a python package designed
-        to make microbial strain construction reproducible and FAIR (Findable, Accessible, 
-        Interoperable, and Reusable). With teemi, you can simulate all steps of 
-        a strain construction cycle, from generating genetic parts to designing 
-        a combinatorial library and keeping track of samples through a commercial
-        Benchling API and a low-level CSV file database. 
-        This tool can be used in literate programming to 
-        increase efficiency and speed in metabolic engineering tasks. 
-        To try teemi, visit our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__.
-        
-        
-        teemi not only simplifies the strain construction process but also offers the 
-        flexibility to adapt to different experimental workflows through its open-source
-        Python platform. This allows for efficient automation of repetitive tasks and
-        a faster pace in metabolic engineering.
-        
-        Our demonstration of teemi in a complex machine learning-guided
-        metabolic engineering task showcases its efficiency 
-        and speed by debottlenecking a crucial step in the strictosidine pathway. 
-        This highlights the versatility and usefulness of this tool in various  
-        biological applications. 
-        
-        Curious about how you can build strains easier and faster with teemi? 
-        Head over to our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__
-        and give it a try.
-        
-        Please cite our paper (in preparation - link tba) if you've used teemi in a scientific publication.
-        
-        .. summary-end
-        
-        
-        Features
-        --------
-        
-        * Combinatorial library generation
-        * HT cloning and transformation workflows
-        * Flowbot One instructions
-        * CSV-based LIMS system as well as integration to Benchling
-        * Genotyping of microbial strains
-        * Advanced Machine Learning of biological datasets with the AutoML `H2O <https://docs.h2o.ai/h2o/latest-stable/h2o-docs/automl.html>`__
-        * Workflows for selecting enzyme homologs
-        * Promoter selection workflows from RNA-seq datasets
-        * Data analysis of large LC-MS datasets along with workflows for analysis
-        
-        
-        Getting started
-        ~~~~~~~~~~~~~~~
-        To get started with making microbial strains in an HT manner please follow the steps below: 
-        
-        1. Install teemi. You will find the necessary information below for installation.
-        
-        2. Check out our `notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__ for inspiration to make HT strain construction with teemi.
-        
-        3. You can start making your own workflows by importing teemi into either Google colab or Jupyter lab/notebooks.
-        
-        
-        Colab notebooks
-        ---------------
-        As a proof of concept we show how teemi and literate programming can be used to streamline bioengineering workflows.
-        These workflows should serve as a guide or a help to build your own workflows and thereby harnessing the power of literate programming with teemi. 
-        
-        Specifically, in this study we present how teemi and literate programming to build simulation-guided, iterative,
-        and evolution-guided laboratory workflows for optimizing strictosidine production in yeast.
-        
-        Below you can find all the notebooks developed in this work. 
-        Just click the Google colab badge to start the workflows. 
-        
-        Strictosidine case : First DBTL cycle
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        **DESIGN:**
-        
-        ..  |Notebook 00| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 00
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/00_1_DESIGN_Homologs.ipynb 
-        
-        ..  |Notebook 01| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 01
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/01_1_DESIGN_Promoters.ipynb
-        
-        ..  |Notebook 02| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 02
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/02_1_DESIGN_Combinatorial_library.ipynb
-            
-        
-        00. Automatically fetch homologs from NCBI from a query in a standardizable and repeatable way |Notebook 00| 
-        
-        
-        01. Promoters can be selected from RNAseq data and fetched from online database with various quality measurements implemented |Notebook 01|
-        
-        
-        
-        02. Combinatorial libraries can be generated with the DesignAssembly class along with robot executable intructions |Notebook 02| 
-        
-        
-        
-        
-        **BUILD:**
-        
-        ..  |Notebook 03| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 03
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/03_1_BUILD_USER_gRNA_plasmid.ipynb
-        
-        
-        ..  |Notebook 04| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 04
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/04_1_BUILD_Background_strain.ipynb
-        
-        
-        ..  |Notebook 05| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 05
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/05_1_BUILD_CombinatorialLibrary_AllStrains.ipynb
-        
-        
-        03. Assembly of a CRISPR plasmid with USER cloning |Notebook 03|
-        
-        04. Construction of the background strain by K/O of G8H and CPR |Notebook 04|
-        
-        05. First combinatorial library was generated for 1280 possible combinations |Notebook 05| 
-        
-        
-        
-        **TEST:**
-        
-        
-        ..  |Notebook 06| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 06
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/06_1_TEST_LibraryCharacterisation.ipynb
-        
-        
-        06. Data processing of LC-MS data and genotyping of the generated strains |Notebook 06|  
-        
-        
-        **LEARN:**
-        
-        ..  |Notebook 07| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 07
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/07_1_LEARN_DataAnalysis.ipynb
-        
-        
-        07. Use AutoML to predict the best combinations for a targeted second round of library construction |Notebook 07|
-        
-        
-        
-        Strictosidine case : Second DBTL cycle
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        
-        
-        **DESIGN:**
-        
-        ..  |Notebook 08| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 08
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_BUILD_Library2.ipynb
-        
-        08. Results from the ML can be translated into making a targeted library of strains |Notebook 08| 
-        
-        
-        
-        **BUILD:**
-        
-        
-        ..  |Notebook 09| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 09
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_2_BUILD_CombinatorialLibrary.ipynb
-        
-        
-        09. Shows the construction of a targeted library of strains |Notebook 09| 
-        
-        
-        
-        
-        **TEST:**
-        
-        ..  |Notebook 10| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 10
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/10_2_TEST_Library_Characterization.ipynb
-        
-        
-        
-        10. Data processing of LC-MS data like in notebook 6 |Notebook 10|
-        
-        
-        
-        
-        **LEARN:**
-        
-        ..  |Notebook 11| image:: https://colab.research.google.com/assets/colab-badge.svg
-            :alt: Notebook 11
-            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/11_2_LEARN_DataAnalysisML.ipynb
-        
-        
-        11. Second ML cycle of ML showing how the model increased performance and saturation of best performing strains |Notebook 11| 
-        
-        
-        
-        Installation
-        ~~~~~~~~~~~~
-        
-        .. installation-start
-        
-        Use pip to install teemi from `PyPI <https://pypi.org/project/teemi/>`__.
-        
-        ::
-        
-            $ pip install teemi
-        
-        
-        If you want to develop or if you cloned the repository from our `GitHub <https://github.com/hiyama341/teemi/>`__
-        you can install teemi in the following way.
-        
-        ::
-        
-            $ pip install -e <path-to-teemi-repo>  
-        
-        
-        You might need to run these commands with administrative
-        privileges if you're not using a virtual environment (using ``sudo`` for example).
-        Please check the `documentation <https://teemi.readthedocs.io/en/latest/installation.html#>`__
-        for further details.
-        
-        .. installation-end
-        
-        Documentation and Examples
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Documentation is available on through numerous Google Colab notebooks with
-        examples on how to use teemi and how we use these notebooks for strain
-        construnction. The Colab notebooks can be found here 
-        `teemi.notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__. 
-        
-        * Documentation: https://teemi.readthedocs.io.
-        
-        
-        Contributions
-        ~~~~~~~~~~~~~
-        
-        Contributions are very welcome! Check our `guidelines <https://teemi.readthedocs.io/en/latest/contributing.html>`__ for instructions how to contribute.
-        
-        
-        License
-        ~~~~~~~
-        * Free software: MIT license
-        
-        Credits
-        -------
-        - This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        - teemis logo was made by Jonas Krogh Fischer. Check out his `website <http://jkfischerproductions.com/kea/portfolio/index.html>`__. 
-        
-        History
-        -------
-        
-        0.1.0 (2023-01-02)
-        ------------------
-        
-        * First release on PyPI.
 Keywords: teemi
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+.. image:: https://raw.githubusercontent.com/hiyama341/teemi/main/pictures/teemi_logo.svg
+  :width: 400
+  :alt: teemi logo 
+
+teemi: a python package designed to make HT strain construction reproducible and FAIR
+-------------------------------------------------------------------------------------
+
+.. summary-start
+
+.. image:: https://badge.fury.io/py/teemi.svg
+        :target: https://badge.fury.io/py/teemi
+
+.. image:: https://github.com/hiyama341/teemi/actions/workflows/main.yml/badge.svg
+        :target: https://github.com/hiyama341/teemi/actions
+
+.. image:: https://readthedocs.org/projects/teemi/badge/?version=latest
+        :target: https://teemi.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+.. image:: https://img.shields.io/github/license/hiyama341/teemi
+        :target: https://github.com/hiyama341/teemi/blob/main/LICENSE
+
+.. image:: https://img.shields.io/pypi/pyversions/teemi.svg
+        :target: https://pypi.org/project/teemi/
+        :alt: Supported Python Versions
+
+.. image:: https://codecov.io/gh/hiyama341/teemi/branch/main/graph/badge.svg?token=P4457QACUY 
+        :target: https://codecov.io/gh/hiyama341/teemi
+
+.. image:: https://img.shields.io/badge/code%20style-black-black
+        :target: https://black.readthedocs.io/en/stable/
+
+.. image:: https://img.shields.io/github/last-commit/hiyama341/teemi
+
+
+
+What is teemi?
+~~~~~~~~~~~~~~
+
+**teemi**, named after the Greek goddess of fairness, is a python package designed
+to make microbial strain construction reproducible and FAIR (Findable, Accessible, 
+Interoperable, and Reusable). With teemi, you can simulate all steps of 
+a strain construction cycle, from generating genetic parts to designing 
+a combinatorial library and keeping track of samples through a commercial
+Benchling API and a low-level CSV file database. 
+This tool can be used in literate programming to 
+increase efficiency and speed in metabolic engineering tasks. 
+To try teemi, visit our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__.
+
+
+teemi not only simplifies the strain construction process but also offers the 
+flexibility to adapt to different experimental workflows through its open-source
+Python platform. This allows for efficient automation of repetitive tasks and
+a faster pace in metabolic engineering.
+
+Our demonstration of teemi in a complex machine learning-guided
+metabolic engineering task showcases its efficiency 
+and speed by debottlenecking a crucial step in the strictosidine pathway. 
+This highlights the versatility and usefulness of this tool in various  
+biological applications. 
+
+Curious about how you can build strains easier and faster with teemi? 
+Head over to our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__
+and give it a try.
+
+Please cite our paper (in preparation - link tba) if you've used teemi in a scientific publication.
+
+.. summary-end
+
+
+Features
+--------
+
+* Combinatorial library generation
+* HT cloning and transformation workflows
+* Flowbot One instructions
+* CSV-based LIMS system as well as integration to Benchling
+* Genotyping of microbial strains
+* Advanced Machine Learning of biological datasets with the AutoML `H2O <https://docs.h2o.ai/h2o/latest-stable/h2o-docs/automl.html>`__
+* Workflows for selecting enzyme homologs
+* Promoter selection workflows from RNA-seq datasets
+* Data analysis of large LC-MS datasets along with workflows for analysis
+
+
+Getting started
+~~~~~~~~~~~~~~~
+To get started with making microbial strains in an HT manner please follow the steps below: 
+
+1. Install teemi. You will find the necessary information below for installation.
+
+2. Check out our `notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__ for inspiration to make HT strain construction with teemi.
+
+3. You can start making your own workflows by importing teemi into either Google colab or Jupyter lab/notebooks.
+
+
+Colab notebooks
+---------------
+As a proof of concept we show how teemi and literate programming can be used to streamline bioengineering workflows.
+These workflows should serve as a guide or a help to build your own workflows and thereby harnessing the power of literate programming with teemi. 
+
+Specifically, in this study we present how teemi and literate programming to build simulation-guided, iterative,
+and evolution-guided laboratory workflows for optimizing strictosidine production in yeast.
+
+Below you can find all the notebooks developed in this work. 
+Just click the Google colab badge to start the workflows. 
+
+Strictosidine case : First DBTL cycle
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+**DESIGN:**
+
+..  |Notebook 00| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 00
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/00_1_DESIGN_Homologs.ipynb 
+
+..  |Notebook 01| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 01
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/01_1_DESIGN_Promoters.ipynb
+
+..  |Notebook 02| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 02
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/02_1_DESIGN_Combinatorial_library.ipynb
+    
+
+00. Automatically fetch homologs from NCBI from a query in a standardizable and repeatable way 
+
+|Notebook 00| 
+
+
+01. Promoters can be selected from RNAseq data and fetched from online database with various quality measurements implemented 
+
+|Notebook 01|
+
+
+
+02. Combinatorial libraries can be generated with the DesignAssembly class along with robot executable intructions 
+
+|Notebook 02| 
+
+
+
+
+**BUILD:**
+
+..  |Notebook 03| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 03
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/03_1_BUILD_USER_gRNA_plasmid.ipynb
+
+
+..  |Notebook 04| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 04
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/04_1_BUILD_Background_strain.ipynb
+
+
+..  |Notebook 05| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 05
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/05_1_BUILD_CombinatorialLibrary_AllStrains.ipynb
+
+
+03. Assembly of a CRISPR plasmid with USER cloning 
+
+|Notebook 03|
+
+04. Construction of the background strain by K/O of G8H and CPR 
+
+|Notebook 04|
+
+05. First combinatorial library was generated for 1280 possible combinations 
+
+|Notebook 05| 
+
+
+
+**TEST:**
+
+
+..  |Notebook 06| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 06
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/06_1_TEST_LibraryCharacterisation.ipynb
+
+
+06. Data processing of LC-MS data and genotyping of the generated strains 
+
+|Notebook 06|  
+
+
+**LEARN:**
+
+..  |Notebook 07| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 07
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/07_1_LEARN_DataAnalysis.ipynb
+
+
+07. Use AutoML to predict the best combinations for a targeted second round of library construction 
+
+|Notebook 07|
+
+
+
+Strictosidine case : Second DBTL cycle
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+
+
+**DESIGN:**
+
+..  |Notebook 08| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 08
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_BUILD_Library2.ipynb
+
+08. Results from the ML can be translated into making a targeted library of strains 
+
+|Notebook 08| 
+
+
+
+**BUILD:**
+
+
+..  |Notebook 09| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 09
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_2_BUILD_CombinatorialLibrary.ipynb
+
+
+09. Shows the construction of a targeted library of strains 
+
+|Notebook 09| 
+
+
+
+
+**TEST:**
+
+..  |Notebook 10| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 10
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/10_2_TEST_Library_Characterization.ipynb
+
+
+
+10. Data processing of LC-MS data like in notebook 6 
+
+|Notebook 10|
+
+
+
+
+**LEARN:**
+
+..  |Notebook 11| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :alt: Notebook 11
+    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/11_2_LEARN_DataAnalysisML.ipynb
+
+
+11. Second ML cycle of ML showing how the model increased performance and saturation of best performing strains 
+
+|Notebook 11| 
+
+
+
+Installation
+~~~~~~~~~~~~
+
+.. installation-start
+
+Use pip to install teemi from `PyPI <https://pypi.org/project/teemi/>`__.
+
+::
+
+    $ pip install teemi
+
+
+If you want to develop or if you cloned the repository from our `GitHub <https://github.com/hiyama341/teemi/>`__
+you can install teemi in the following way.
+
+::
+
+    $ pip install -e <path-to-teemi-repo>  
+
+
+You might need to run these commands with administrative
+privileges if you're not using a virtual environment (using ``sudo`` for example).
+Please check the `documentation <https://teemi.readthedocs.io/en/latest/installation.html#>`__
+for further details.
+
+.. installation-end
+
+Documentation and Examples
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Documentation is available on through numerous Google Colab notebooks with
+examples on how to use teemi and how we use these notebooks for strain
+construnction. The Colab notebooks can be found here 
+`teemi.notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__. 
+
+* Documentation: https://teemi.readthedocs.io.
+
+
+Contributions
+~~~~~~~~~~~~~
+
+Contributions are very welcome! Check our `guidelines <https://teemi.readthedocs.io/en/latest/contributing.html>`__ for instructions how to contribute.
+
+
+License
+~~~~~~~
+* Free software: MIT license
+
+Credits
+-------
+- This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+- teemis logo was made by Jonas Krogh Fischer. Check out his `website <http://jkfischerproductions.com/kea/portfolio/index.html>`__. 
+
+History
+-------
+
+0.1.0 (2023-01-02)
+------------------
+
+* First release on PyPI.
```

### Comparing `teemi-0.1.3/teemi.egg-info/SOURCES.txt` & `teemi-0.1.4/teemi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `teemi-0.1.3/versioneer.py` & `teemi-0.1.4/versioneer.py`

 * *Files identical despite different names*

