# Comparing `tmp/SpatialGlue-1.0.4.tar.gz` & `tmp/SpatialGlue-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpatialGlue-1.0.4.tar", last modified: Tue May  9 02:21:35 2023, max compression
+gzip compressed data, was "dist/SpatialGlue-1.0.5.tar", last modified: Tue May  9 02:41:58 2023, max compression
```

## Comparing `SpatialGlue-1.0.4.tar` & `SpatialGlue-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 02:21:35.061217 SpatialGlue-1.0.4/
--rw-rw-r--   0 yahui     (9019) yahui     (1023)    34523 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/LICENSE.md
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     1006 2023-05-09 02:21:35.061217 SpatialGlue-1.0.4/PKG-INFO
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     1671 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/README.md
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/README.rst
-drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 02:21:35.061217 SpatialGlue-1.0.4/SpatialGlue/
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     6845 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/SpatialGlue/SpatialGlue.py
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     7620 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/SpatialGlue/model.py
--rw-rw-r--   0 yahui     (9019) yahui     (1023)    12330 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/SpatialGlue/preprocess.py
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/SpatialGlue/readme.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     5974 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/SpatialGlue/utils.py
-drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 02:21:35.061217 SpatialGlue-1.0.4/SpatialGlue.egg-info/
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     1006 2023-05-09 02:21:34.000000 SpatialGlue-1.0.4/SpatialGlue.egg-info/PKG-INFO
--rw-rw-r--   0 yahui     (9019) yahui     (1023)      409 2023-05-09 02:21:35.000000 SpatialGlue-1.0.4/SpatialGlue.egg-info/SOURCES.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 02:21:34.000000 SpatialGlue-1.0.4/SpatialGlue.egg-info/dependency_links.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 02:21:34.000000 SpatialGlue-1.0.4/SpatialGlue.egg-info/not-zip-safe
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        9 2023-05-09 02:21:34.000000 SpatialGlue-1.0.4/SpatialGlue.egg-info/requires.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)       12 2023-05-09 02:21:34.000000 SpatialGlue-1.0.4/SpatialGlue.egg-info/top_level.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)   653466 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/SpatialGlue.png
--rw-rw-r--   0 yahui     (9019) yahui     (1023)      330 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/__init__.py
-drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 02:21:35.061217 SpatialGlue-1.0.4/data/
--rw-rw-r--   0 yahui     (9019) yahui     (1023)      628 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/data/readme.md
--rw-rw-r--   0 yahui     (9019) yahui     (1023)       38 2023-05-09 02:21:35.061217 SpatialGlue-1.0.4/setup.cfg
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     1685 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/setup.py
+drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 02:41:58.532153 SpatialGlue-1.0.5/
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)    34523 2023-05-09 02:41:27.000000 SpatialGlue-1.0.5/LICENSE.md
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     1006 2023-05-09 02:41:58.532153 SpatialGlue-1.0.5/PKG-INFO
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     1671 2023-05-09 02:41:27.000000 SpatialGlue-1.0.5/README.md
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 02:41:27.000000 SpatialGlue-1.0.5/README.rst
+drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 02:41:58.532153 SpatialGlue-1.0.5/SpatialGlue/
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     6845 2023-05-09 02:41:27.000000 SpatialGlue-1.0.5/SpatialGlue/SpatialGlue.py
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     7620 2023-05-09 02:41:27.000000 SpatialGlue-1.0.5/SpatialGlue/model.py
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)    12330 2023-05-09 02:41:27.000000 SpatialGlue-1.0.5/SpatialGlue/preprocess.py
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 02:41:27.000000 SpatialGlue-1.0.5/SpatialGlue/readme.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     6034 2023-05-09 02:41:27.000000 SpatialGlue-1.0.5/SpatialGlue/utils.py
+drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 02:41:58.532153 SpatialGlue-1.0.5/SpatialGlue.egg-info/
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     1006 2023-05-09 02:41:58.000000 SpatialGlue-1.0.5/SpatialGlue.egg-info/PKG-INFO
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)      409 2023-05-09 02:41:58.000000 SpatialGlue-1.0.5/SpatialGlue.egg-info/SOURCES.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 02:41:58.000000 SpatialGlue-1.0.5/SpatialGlue.egg-info/dependency_links.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 02:41:58.000000 SpatialGlue-1.0.5/SpatialGlue.egg-info/not-zip-safe
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        9 2023-05-09 02:41:58.000000 SpatialGlue-1.0.5/SpatialGlue.egg-info/requires.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)       12 2023-05-09 02:41:58.000000 SpatialGlue-1.0.5/SpatialGlue.egg-info/top_level.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)   653466 2023-05-09 02:41:27.000000 SpatialGlue-1.0.5/SpatialGlue.png
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)      330 2023-05-09 02:41:27.000000 SpatialGlue-1.0.5/__init__.py
+drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 02:41:58.532153 SpatialGlue-1.0.5/data/
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)      628 2023-05-09 02:41:27.000000 SpatialGlue-1.0.5/data/readme.md
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)       38 2023-05-09 02:41:58.532153 SpatialGlue-1.0.5/setup.cfg
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     1685 2023-05-09 02:41:27.000000 SpatialGlue-1.0.5/setup.py
```

### Comparing `SpatialGlue-1.0.4/LICENSE.md` & `SpatialGlue-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.4/PKG-INFO` & `SpatialGlue-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpatialGlue
-Version: 1.0.4
+Version: 1.0.5
 Summary: Integrated analysis of spatial multi-omics with SpatialGlue
 Home-page: https://github.com/JinmiaoChenLab/SpatialGlue
 Author: Yahui Long
 Author-email: longyh@immunol.a-star.edu.sg
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `SpatialGlue-1.0.4/README.md` & `SpatialGlue-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.4/SpatialGlue/SpatialGlue.py` & `SpatialGlue-1.0.5/SpatialGlue/SpatialGlue.py`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.4/SpatialGlue/model.py` & `SpatialGlue-1.0.5/SpatialGlue/model.py`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.4/SpatialGlue/preprocess.py` & `SpatialGlue-1.0.5/SpatialGlue/preprocess.py`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.4/SpatialGlue/utils.py` & `SpatialGlue-1.0.5/SpatialGlue/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import pickle
 import numpy as np
+import pandas as pd
 import scanpy as sc
 import seaborn as sns
+from sklearn.decomposition import PCA
 import matplotlib.pyplot as plt
 
 #os.environ['R_HOME'] = '/scbio4/tools/R/R-4.0.3_openblas/R-4.0.3'    
 
 def mclust_R(adata, num_cluster, modelNames='EEE', used_obsm='emb_pca', random_seed=2020):
     """\
     Clustering using the mclust algorithm.
```

### Comparing `SpatialGlue-1.0.4/SpatialGlue.egg-info/PKG-INFO` & `SpatialGlue-1.0.5/SpatialGlue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpatialGlue
-Version: 1.0.4
+Version: 1.0.5
 Summary: Integrated analysis of spatial multi-omics with SpatialGlue
 Home-page: https://github.com/JinmiaoChenLab/SpatialGlue
 Author: Yahui Long
 Author-email: longyh@immunol.a-star.edu.sg
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `SpatialGlue-1.0.4/SpatialGlue.png` & `SpatialGlue-1.0.5/SpatialGlue.png`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.4/data/readme.md` & `SpatialGlue-1.0.5/data/readme.md`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.4/setup.py` & `SpatialGlue-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import Command, find_packages, setup
 
 __lib_name__ = "SpatialGlue"
-__lib_version__ = "1.0.4"
+__lib_version__ = "1.0.5"
 __description__ = "Integrated analysis of spatial multi-omics with SpatialGlue"
 __url__ = "https://github.com/JinmiaoChenLab/SpatialGlue"
 __author__ = "Yahui Long"
 __author_email__ = "longyh@immunol.a-star.edu.sg"
 __license__ = "MIT"
 __keywords__ = ["Spatial multi-omics", "Cross-omics integration", "Deep learning", "Graph neural networks", "Dual attention"]
 __requires__ = ["requests",]
```

