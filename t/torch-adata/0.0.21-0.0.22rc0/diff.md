# Comparing `tmp/torch-adata-0.0.21.tar.gz` & `tmp/torch-adata-0.0.22rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-adata-0.0.21.tar", last modified: Fri May  5 01:57:15 2023, max compression
+gzip compressed data, was "torch-adata-0.0.22rc0.tar", last modified: Mon May  8 22:20:17 2023, max compression
```

## Comparing `torch-adata-0.0.21.tar` & `torch-adata-0.0.22rc0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:15.962382 torch-adata-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-05-05 01:57:05.000000 torch-adata-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-05 01:57:15.962382 torch-adata-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-05 01:57:05.000000 torch-adata-0.0.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 01:57:15.962382 torch-adata-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-05 01:57:05.000000 torch-adata-0.0.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:15.958382 torch-adata-0.0.21/torch_adata/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:15.958382 torch-adata-0.0.21/torch_adata/_core/
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_AnnDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:15.958382 torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_data_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_fetch_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_group_and_pad_adata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_identity_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_one_hot_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_register_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_return_data_on_axis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:15.962382 torch-adata-0.0.21/torch_adata/_core/_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_lightning/_auto_parse_base_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_lightning/_configure_adata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_lightning/_function_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_lightning/_lightning_anndata_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_core/_lightning/_train_val_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:15.962382 torch-adata-0.0.21/torch_adata/_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_tools/_anndataset_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_tools/_base_lightning_data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_tools/_dummy_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_tools/_fetch_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_tools/_idx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-05 01:57:05.000000 torch-adata-0.0.21/torch_adata/_tools/_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:15.958382 torch-adata-0.0.21/torch_adata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-05 01:57:15.000000 torch-adata-0.0.21/torch_adata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-05 01:57:15.000000 torch-adata-0.0.21/torch_adata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:57:15.000000 torch-adata-0.0.21/torch_adata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-05 01:57:15.000000 torch-adata-0.0.21/torch_adata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 01:57:15.000000 torch-adata-0.0.21/torch_adata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:17.857854 torch-adata-0.0.22rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-08 22:20:17.857854 torch-adata-0.0.22rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 22:20:17.857854 torch-adata-0.0.22rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:17.849854 torch-adata-0.0.22rc0/torch_adata/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:17.853854 torch-adata-0.0.22rc0/torch_adata/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_AnnDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:17.853854 torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_data_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_fetch_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_group_and_pad_adata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_identity_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_register_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_return_data_on_axis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:17.857854 torch-adata-0.0.22rc0/torch_adata/_core/_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_lightning/_auto_parse_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_lightning/_configure_adata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_lightning/_function_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_lightning/_lightning_anndata_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_core/_lightning/_train_val_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:17.857854 torch-adata-0.0.22rc0/torch_adata/_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_tools/_anndataset_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_tools/_base_lightning_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_tools/_dummy_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_tools/_fetch_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_tools/_idx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-08 22:20:02.000000 torch-adata-0.0.22rc0/torch_adata/_tools/_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:17.853854 torch-adata-0.0.22rc0/torch_adata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-08 22:20:17.000000 torch-adata-0.0.22rc0/torch_adata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-08 22:20:17.000000 torch-adata-0.0.22rc0/torch_adata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:20:17.000000 torch-adata-0.0.22rc0/torch_adata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 22:20:17.000000 torch-adata-0.0.22rc0/torch_adata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 22:20:17.000000 torch-adata-0.0.22rc0/torch_adata.egg-info/top_level.txt
```

### Comparing `torch-adata-0.0.21/LICENSE` & `torch-adata-0.0.22rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/PKG-INFO` & `torch-adata-0.0.22rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-adata
-Version: 0.0.21
+Version: 0.0.22rc0
 Summary: torch-adata
 Author: Michael E. Vinyard
 Author-email: mvinyard@g.harvard.edu
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torch-adata-0.0.21/README.md` & `torch-adata-0.0.22rc0/README.md`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/setup.py` & `torch-adata-0.0.22rc0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 
 __module_name__ = "setup.py"
 __doc__ = """PYPI package distribution setup."""
 __author__ = ", ".join(["Michael E. Vinyard"])
 __email__ = ", ".join(["vinyard@g.harvard.edu"])
 
 
-# -- specify package version: --------------------------------------------------
-__version__ = "0.0.21"
-
-
 # -- import packages: ----------------------------------------------------------
 import setuptools
 import re
 import os
 import sys
 
 
 # -- run setup: ----------------------------------------------------------------
 setuptools.setup(
     name="torch-adata",
-    version="0.0.21",
+    version="0.0.22rc0",
     python_requires=">3.9.0",
     author="Michael E. Vinyard",
     author_email="mvinyard@g.harvard.edu",
     url=None,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="torch-adata",
```

### Comparing `torch-adata-0.0.21/torch_adata/__init__.py` & `torch-adata-0.0.22rc0/torch_adata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 __module_name__ = "__init__.py"
 __doc__ = """Main __init__ module."""
 __author__ = ", ".join(["Michael E. Vinyard"])
 __email__ = ", ".join(["vinyard@g.harvard.edu"])
 
 
 # -- specify package version: --------------------------------------------------
-__version__ = "0.0.21"
+__version__ = "0.0.22rc0"
 
 
 # -- import modules: -----------------------------------------------------------
 from ._core._AnnDataset import AnnDataset
 from ._core._lightning._lightning_anndata_module import LightningAnnDataModule
 from . import _tools as tl
```

### Comparing `torch-adata-0.0.21/torch_adata/_core/_AnnDataset.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_AnnDataset.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/__init__.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_data_typing.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_data_typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 __email__ = ", ".join(["vinyard@g.harvard.edu"])
 
 
 # -- import packages: --------------------------------------------------------------------
 import numpy
 import pandas
 import torch
+import scipy
 
 
 # -- data type handlers: -----------------------------------------------------------------
 def is_numpy_array(x_arr) -> bool:
     """
     Inspects and indicates if input is numpy.ndarray
 
@@ -42,14 +43,31 @@
     --------
     indicator
         type: bool
     """
     return x_arr.__class__ is pandas.Categorical
 
 
+def is_scipy_sparse(x_arr):
+    """
+    Inspects and indicates if input is a subclass of: scipy.sparse.spmatrix, the base class for all scipy sparse matrices.
+
+    Parameters:
+    -----------
+    x_arr
+        type: unknown
+
+    Returns:
+    --------
+    indicator
+        type: bool
+    """
+    return isinstance(x_arr, scipy.sparse.spmatrix)
+
+
 def to_np_array(x_arr) -> numpy.ndarray:
     """
     Inspects input. If input is not, numpy.ndarray, it is transformed to numpy.ndarray.
 
     Parameters:
     -----------
     x_arr
@@ -58,14 +76,16 @@
     Returns:
     --------
     x_arr_transformed
         type: numpy.ndarray
     """
     if is_numpy_array(x_arr):
         return x_arr
+    if is_scipy_sparse(x_arr):
+        return x_arr.toarray()
     if is_pandas_categorical(x_arr):
         return x_arr.to_numpy()
     return x_arr.toarray()
 
 
 def tensorize(x_arr) -> torch.Tensor:
     """
@@ -85,8 +105,8 @@
 
 
 def as_list(item):
     if item:
         if not isinstance(item, list):
             return [item]
         return item
-    return []
+    return []
```

### Comparing `torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_fetch_data.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_fetch_data.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_group_and_pad_adata.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_group_and_pad_adata.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_identity_msg.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_identity_msg.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_one_hot_encode.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_one_hot_encode.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_register_init.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_register_init.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_core/_core_ancilliary/_return_data_on_axis.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_core_ancilliary/_return_data_on_axis.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_core/_lightning/_auto_parse_base_class.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_lightning/_auto_parse_base_class.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_core/_lightning/_configure_adata.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_lightning/_configure_adata.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_core/_lightning/_function_kwargs.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_lightning/_function_kwargs.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_core/_lightning/_lightning_anndata_module.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_lightning/_lightning_anndata_module.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_core/_lightning/_train_val_split.py` & `torch-adata-0.0.22rc0/torch_adata/_core/_lightning/_train_val_split.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_tools/__init__.py` & `torch-adata-0.0.22rc0/torch_adata/_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_tools/_anndataset_split.py` & `torch-adata-0.0.22rc0/torch_adata/_tools/_anndataset_split.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_tools/_base_lightning_data_module.py` & `torch-adata-0.0.22rc0/torch_adata/_tools/_base_lightning_data_module.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_tools/_dummy_batch.py` & `torch-adata-0.0.22rc0/torch_adata/_tools/_dummy_batch.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_tools/_fetch_data.py` & `torch-adata-0.0.22rc0/torch_adata/_tools/_fetch_data.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_tools/_idx.py` & `torch-adata-0.0.22rc0/torch_adata/_tools/_idx.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata/_tools/_split.py` & `torch-adata-0.0.22rc0/torch_adata/_tools/_split.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.21/torch_adata.egg-info/PKG-INFO` & `torch-adata-0.0.22rc0/torch_adata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-adata
-Version: 0.0.21
+Version: 0.0.22rc0
 Summary: torch-adata
 Author: Michael E. Vinyard
 Author-email: mvinyard@g.harvard.edu
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torch-adata-0.0.21/torch_adata.egg-info/SOURCES.txt` & `torch-adata-0.0.22rc0/torch_adata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

