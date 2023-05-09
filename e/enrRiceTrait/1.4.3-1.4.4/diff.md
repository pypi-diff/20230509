# Comparing `tmp/enrRiceTrait-1.4.3.tar.gz` & `tmp/enrRiceTrait-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enrRiceTrait-1.4.3.tar", last modified: Thu May  4 15:19:30 2023, max compression
+gzip compressed data, was "enrRiceTrait-1.4.4.tar", last modified: Tue May  9 03:37:34 2023, max compression
```

## Comparing `enrRiceTrait-1.4.3.tar` & `enrRiceTrait-1.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-05-04 15:19:30.326972 enrRiceTrait-1.4.3/
--rw-rw-r--   0 yao        (501) staff       (20)       53 2021-03-29 13:55:50.000000 enrRiceTrait-1.4.3/MANIFEST.in
--rw-r--r--   0 yao        (501) staff       (20)      599 2023-05-04 15:19:30.326712 enrRiceTrait-1.4.3/PKG-INFO
--rw-rw-r--   0 yao        (501) staff       (20)       92 2020-07-13 13:31:42.000000 enrRiceTrait-1.4.3/README.md
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-05-04 15:19:30.303075 enrRiceTrait-1.4.3/enrRiceTrait/
--rw-r--r--   0 yao        (501) staff       (20)    25252 2023-05-04 15:18:20.000000 enrRiceTrait-1.4.3/enrRiceTrait/Enrichment.py
--rw-rw-r--   0 yao        (501) staff       (20)      478 2021-03-29 14:59:32.000000 enrRiceTrait-1.4.3/enrRiceTrait/PTE_config.py
--rw-rw-r--   0 yao        (501) staff       (20)      222 2023-05-04 15:19:13.000000 enrRiceTrait-1.4.3/enrRiceTrait/__init__.py
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-05-04 15:19:30.320311 enrRiceTrait-1.4.3/enrRiceTrait/data/
--rw-rw-r--   0 yao        (501) staff       (20)  9834834 2021-03-27 15:22:16.000000 enrRiceTrait-1.4.3/enrRiceTrait/data/Total_Association.txt
--rw-r--r--   0 yao        (501) staff       (20)  1074775 2023-04-25 14:00:56.000000 enrRiceTrait-1.4.3/enrRiceTrait/data/to.wto.ro.funRiceGene.obo
--rw-rw-r--   0 yao        (501) staff       (20)  1090456 2021-03-25 12:59:06.000000 enrRiceTrait-1.4.3/enrRiceTrait/data/to.wto.ro.funRiceGene.wheat(do not change to rice).obo
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-05-04 15:19:30.304103 enrRiceTrait-1.4.3/enrRiceTrait.egg-info/
--rw-rw-r--   0 yao        (501) staff       (20)      599 2023-05-04 15:19:30.000000 enrRiceTrait-1.4.3/enrRiceTrait.egg-info/PKG-INFO
--rw-rw-r--   0 yao        (501) staff       (20)      410 2023-05-04 15:19:30.000000 enrRiceTrait-1.4.3/enrRiceTrait.egg-info/SOURCES.txt
--rw-rw-r--   0 yao        (501) staff       (20)        1 2023-05-04 15:19:30.000000 enrRiceTrait-1.4.3/enrRiceTrait.egg-info/dependency_links.txt
--rw-rw-r--   0 yao        (501) staff       (20)       13 2023-05-04 15:19:30.000000 enrRiceTrait-1.4.3/enrRiceTrait.egg-info/top_level.txt
--rw-r--r--   0 yao        (501) staff       (20)       38 2023-05-04 15:19:30.327056 enrRiceTrait-1.4.3/setup.cfg
--rw-rw-r--   0 yao        (501) staff       (20)     1085 2023-05-04 15:19:13.000000 enrRiceTrait-1.4.3/setup.py
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-05-09 03:37:34.837449 enrRiceTrait-1.4.4/
+-rw-rw-r--   0 yao        (501) staff       (20)       53 2021-03-29 13:55:50.000000 enrRiceTrait-1.4.4/MANIFEST.in
+-rw-r--r--   0 yao        (501) staff       (20)      599 2023-05-09 03:37:34.837129 enrRiceTrait-1.4.4/PKG-INFO
+-rw-rw-r--   0 yao        (501) staff       (20)       92 2020-07-13 13:31:42.000000 enrRiceTrait-1.4.4/README.md
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-05-09 03:37:34.799736 enrRiceTrait-1.4.4/enrRiceTrait/
+-rw-r--r--   0 yao        (501) staff       (20)    25473 2023-05-09 01:51:44.000000 enrRiceTrait-1.4.4/enrRiceTrait/Enrichment.py
+-rw-rw-r--   0 yao        (501) staff       (20)      478 2021-03-29 14:59:32.000000 enrRiceTrait-1.4.4/enrRiceTrait/PTE_config.py
+-rw-rw-r--   0 yao        (501) staff       (20)      222 2023-05-09 03:37:16.000000 enrRiceTrait-1.4.4/enrRiceTrait/__init__.py
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-05-09 03:37:34.829106 enrRiceTrait-1.4.4/enrRiceTrait/data/
+-rw-rw-r--   0 yao        (501) staff       (20)  9834834 2021-03-27 15:22:16.000000 enrRiceTrait-1.4.4/enrRiceTrait/data/Total_Association.txt
+-rw-r--r--   0 yao        (501) staff       (20)  1074775 2023-04-25 14:00:56.000000 enrRiceTrait-1.4.4/enrRiceTrait/data/to.wto.ro.funRiceGene.obo
+-rw-rw-r--   0 yao        (501) staff       (20)  1090456 2021-03-25 12:59:06.000000 enrRiceTrait-1.4.4/enrRiceTrait/data/to.wto.ro.funRiceGene.wheat(do not change to rice).obo
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-05-09 03:37:34.800899 enrRiceTrait-1.4.4/enrRiceTrait.egg-info/
+-rw-rw-r--   0 yao        (501) staff       (20)      599 2023-05-09 03:37:34.000000 enrRiceTrait-1.4.4/enrRiceTrait.egg-info/PKG-INFO
+-rw-rw-r--   0 yao        (501) staff       (20)      410 2023-05-09 03:37:34.000000 enrRiceTrait-1.4.4/enrRiceTrait.egg-info/SOURCES.txt
+-rw-rw-r--   0 yao        (501) staff       (20)        1 2023-05-09 03:37:34.000000 enrRiceTrait-1.4.4/enrRiceTrait.egg-info/dependency_links.txt
+-rw-rw-r--   0 yao        (501) staff       (20)       13 2023-05-09 03:37:34.000000 enrRiceTrait-1.4.4/enrRiceTrait.egg-info/top_level.txt
+-rw-r--r--   0 yao        (501) staff       (20)       38 2023-05-09 03:37:34.837528 enrRiceTrait-1.4.4/setup.cfg
+-rw-rw-r--   0 yao        (501) staff       (20)     1085 2023-05-09 03:37:16.000000 enrRiceTrait-1.4.4/setup.py
```

### Comparing `enrRiceTrait-1.4.3/PKG-INFO` & `enrRiceTrait-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enrRiceTrait
-Version: 1.4.3
+Version: 1.4.4
 Summary: A python package for Rice Trait Enrichment.
 Home-page: https://github.com/YaoXinZhi/enrRiceTrait
 Author: xinzhi_yao
 Author-email: xinzhi_bioinfo@163.com
 License: UNKNOWN
 Description: # Plant Trait Enrichment Package  
         This is a python package for plant trait enrichment.
```

### Comparing `enrRiceTrait-1.4.3/enrRiceTrait/Enrichment.py` & `enrRiceTrait-1.4.4/enrRiceTrait/Enrichment.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import numpy as np
 import pandas as pd
 #from plotnine import *
 import matplotlib.pyplot as plt
 from scipy.stats import hypergeom
 from collections import defaultdict
 from .PTE_config import db_config
-
+from matplotlib import ticker
 
 class enrichment_result:
     def __init__(self):
 
         self.query_gene_set = set()
         self.miss_id_set = set()
 
@@ -456,14 +456,16 @@
         # set color map
         # matplotlib update
         # cmap = plt.cm.get_cmap('RdYlBu_r')
         cmap = plt.cm.RdYlBu_r
         # cmap = plt.cm.RdYlBu
 
         # 转换基因数和p值为浮点数
+        # gene_nums = [ float(d[ 1 ]) for d in data ]
+        # change to int
         gene_nums = [ float(d[ 1 ]) for d in data ]
         p_values = [ -np.log10(float(d[ 2 ])) for d in data ]
         # p_values = [ float(d[ 2 ]) for d in data ]
 
         # 根据p值设置颜色
         colors = [ cmap(p) for p in np.interp(p_values, (np.min(p_values), np.max(p_values)), (0, 1)) ]
 
@@ -475,16 +477,18 @@
         ax.grid(True, linestyle='--', linewidth=0.5, color='gray')
 
         # 设置Y轴标签和刻度
         ax.set_yticks(range(len(data)))
         ax.set_yticklabels([ d[ 0 ].capitalize() for d in data ], fontsize=font_size)
 
         # fix the warning
-        ax.set_xticklabels([ i for i in range(len(gene_nums)) ], fontsize=font_size)
-        # ax.set_xticks([ i for i in range(len(gene_nums)) ], fontsize=font_size)
+        # ax.set_xticklabels([ i for i in range(len(gene_nums)) ], fontsize=font_size)
+        # ax.xaxis.set_major_locator(ticker.MaxNLocator(integer=True))
+        ax.xaxis.set_major_locator(ticker.MaxNLocator(integer=True))
+        ax.tick_params(axis='x', labelsize=font_size)
 
         # 设置X轴标签和刻度
         ax.set_xlabel('Gene Count', fontsize=font_size)
         # ax.set_ylabel('GO Enrichment Name')
         # ax.set_title('GO Enrichment Bar Plot')
         sm = plt.cm.ScalarMappable(cmap=cmap, norm=plt.Normalize(vmin=np.min(p_values), vmax=np.max(p_values)))
         sm._A = [ ]
```

### Comparing `enrRiceTrait-1.4.3/enrRiceTrait/data/Total_Association.txt` & `enrRiceTrait-1.4.4/enrRiceTrait/data/Total_Association.txt`

 * *Files identical despite different names*

### Comparing `enrRiceTrait-1.4.3/enrRiceTrait/data/to.wto.ro.funRiceGene.obo` & `enrRiceTrait-1.4.4/enrRiceTrait/data/to.wto.ro.funRiceGene.obo`

 * *Files identical despite different names*

### Comparing `enrRiceTrait-1.4.3/enrRiceTrait/data/to.wto.ro.funRiceGene.wheat(do not change to rice).obo` & `enrRiceTrait-1.4.4/enrRiceTrait/data/to.wto.ro.funRiceGene.wheat(do not change to rice).obo`

 * *Files identical despite different names*

### Comparing `enrRiceTrait-1.4.3/enrRiceTrait.egg-info/PKG-INFO` & `enrRiceTrait-1.4.4/enrRiceTrait.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enrRiceTrait
-Version: 1.4.3
+Version: 1.4.4
 Summary: A python package for Rice Trait Enrichment.
 Home-page: https://github.com/YaoXinZhi/enrRiceTrait
 Author: xinzhi_yao
 Author-email: xinzhi_bioinfo@163.com
 License: UNKNOWN
 Description: # Plant Trait Enrichment Package  
         This is a python package for plant trait enrichment.
```

### Comparing `enrRiceTrait-1.4.3/setup.py` & `enrRiceTrait-1.4.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setup(
   name='enrRiceTrait',
-  version='1.4.3',
+  version='1.4.4',
   author='xinzhi_yao',
   author_email='xinzhi_bioinfo@163.com',
   description="A python package for Rice Trait Enrichment.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/YaoXinZhi/enrRiceTrait",
```

