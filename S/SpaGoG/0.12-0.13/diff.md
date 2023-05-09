# Comparing `tmp/SpaGoG-0.12.tar.gz` & `tmp/SpaGoG-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpaGoG-0.12.tar", last modified: Tue May  9 00:44:16 2023, max compression
+gzip compressed data, was "SpaGoG-0.13.tar", last modified: Tue May  9 12:40:28 2023, max compression
```

## Comparing `SpaGoG-0.12.tar` & `SpaGoG-0.13.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 00:44:16.101998 SpaGoG-0.12/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      370 2023-05-09 00:44:16.101998 SpaGoG-0.12/PKG-INFO
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-08 23:47:17.000000 SpaGoG-0.12/README.md
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 00:44:16.101998 SpaGoG-0.12/SpaGoG.egg-info/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      370 2023-05-09 00:44:16.000000 SpaGoG-0.12/SpaGoG.egg-info/PKG-INFO
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      844 2023-05-09 00:44:16.000000 SpaGoG-0.12/SpaGoG.egg-info/SOURCES.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-05-09 00:44:16.000000 SpaGoG-0.12/SpaGoG.egg-info/dependency_links.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)       29 2023-05-09 00:44:16.000000 SpaGoG-0.12/SpaGoG.egg-info/requires.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        7 2023-05-09 00:44:16.000000 SpaGoG-0.12/SpaGoG.egg-info/top_level.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)       79 2023-05-09 00:44:16.101998 SpaGoG-0.12/setup.cfg
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      565 2023-05-09 00:44:07.000000 SpaGoG-0.12/setup.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 00:44:16.101998 SpaGoG-0.12/spagog/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-04-24 11:36:25.000000 SpaGoG-0.12/spagog/__init__.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 00:44:16.101998 SpaGoG-0.12/spagog/datasets/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-04-24 11:36:25.000000 SpaGoG-0.12/spagog/datasets/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     7327 2023-05-08 19:46:45.000000 SpaGoG-0.12/spagog/datasets/graphDataPair.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1986 2023-04-24 22:46:08.000000 SpaGoG-0.12/spagog/datasets/graphDataset.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     7667 2023-05-08 21:57:56.000000 SpaGoG-0.12/spagog/datasets/graphsDataPair.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    13224 2023-05-08 21:57:56.000000 SpaGoG-0.12/spagog/datasets/graphsDataset.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     7421 2023-04-24 22:49:26.000000 SpaGoG-0.12/spagog/datasets/tabDataPair.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    11827 2023-05-08 21:57:56.000000 SpaGoG-0.12/spagog/datasets/tabDataset.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    11773 2023-05-08 21:59:22.000000 SpaGoG-0.12/spagog/experiments.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     5200 2023-05-08 23:26:11.000000 SpaGoG-0.12/spagog/main.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 00:44:16.101998 SpaGoG-0.12/spagog/models/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-04-24 11:36:25.000000 SpaGoG-0.12/spagog/models/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      423 2023-04-24 11:36:25.000000 SpaGoG-0.12/spagog/models/abstractModel.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    14162 2023-05-08 21:57:56.000000 SpaGoG-0.12/spagog/models/abstractNN.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     6706 2023-05-08 20:04:49.000000 SpaGoG-0.12/spagog/models/graphClassification.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    17298 2023-05-08 21:49:16.000000 SpaGoG-0.12/spagog/models/graphNodeClassification.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     3979 2023-04-24 22:55:37.000000 SpaGoG-0.12/spagog/models/nodeClassification.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 00:44:16.101998 SpaGoG-0.12/spagog/utils/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-04-24 11:36:41.000000 SpaGoG-0.12/spagog/utils/__init__.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 00:44:16.101998 SpaGoG-0.12/spagog/utils/data/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-04-24 11:36:41.000000 SpaGoG-0.12/spagog/utils/data/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     6352 2023-04-24 22:54:37.000000 SpaGoG-0.12/spagog/utils/data/tab2graph.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     2887 2023-04-24 22:46:08.000000 SpaGoG-0.12/spagog/utils/gfp.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     6336 2023-04-24 22:54:51.000000 SpaGoG-0.12/spagog/utils/knn.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 00:44:16.101998 SpaGoG-0.12/spagog/utils/metrics/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-04-24 11:36:41.000000 SpaGoG-0.12/spagog/utils/metrics/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1799 2023-04-24 22:52:07.000000 SpaGoG-0.12/spagog/utils/metrics/metrics.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      370 2023-05-09 12:40:28.508539 SpaGoG-0.13/PKG-INFO
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-08 23:47:17.000000 SpaGoG-0.13/README.md
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/SpaGoG.egg-info/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      370 2023-05-09 12:40:28.000000 SpaGoG-0.13/SpaGoG.egg-info/PKG-INFO
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      915 2023-05-09 12:40:28.000000 SpaGoG-0.13/SpaGoG.egg-info/SOURCES.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-05-09 12:40:28.000000 SpaGoG-0.13/SpaGoG.egg-info/dependency_links.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)       29 2023-05-09 12:40:28.000000 SpaGoG-0.13/SpaGoG.egg-info/requires.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        7 2023-05-09 12:40:28.000000 SpaGoG-0.13/SpaGoG.egg-info/top_level.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)       79 2023-05-09 12:40:28.508539 SpaGoG-0.13/setup.cfg
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      565 2023-05-09 12:40:20.000000 SpaGoG-0.13/setup.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/__init__.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/datasets/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     7361 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/graphDataPair.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1986 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/graphDataset.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     7661 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/graphsDataPair.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    13210 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/graphsDataset.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     7421 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/tabDataPair.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    11832 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/datasets/tabDataset.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/default_params/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/default_params/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      706 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/default_params/load_params.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    11778 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/experiments.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     5062 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/main.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/models/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/models/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      423 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/models/abstractModel.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    14164 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/models/abstractNN.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     6708 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/models/graphClassification.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    17286 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/models/graphNodeClassification.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     3979 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/models/nodeClassification.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/utils/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/__init__.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/utils/data/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/data/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     6347 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/data/tab2graph.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     2887 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/gfp.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     6338 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/knn.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-05-09 12:40:28.508539 SpaGoG-0.13/spagog/utils/metrics/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/metrics/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1799 2023-05-09 11:55:00.000000 SpaGoG-0.13/spagog/utils/metrics/metrics.py
```

### Comparing `SpaGoG-0.12/SpaGoG.egg-info/SOURCES.txt` & `SpaGoG-0.13/SpaGoG.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 spagog/datasets/__init__.py
 spagog/datasets/graphDataPair.py
 spagog/datasets/graphDataset.py
 spagog/datasets/graphsDataPair.py
 spagog/datasets/graphsDataset.py
 spagog/datasets/tabDataPair.py
 spagog/datasets/tabDataset.py
+spagog/default_params/__init__.py
+spagog/default_params/load_params.py
 spagog/models/__init__.py
 spagog/models/abstractModel.py
 spagog/models/abstractNN.py
 spagog/models/graphClassification.py
 spagog/models/graphNodeClassification.py
 spagog/models/nodeClassification.py
 spagog/utils/__init__.py
```

### Comparing `SpaGoG-0.12/setup.py` & `SpaGoG-0.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='SpaGoG',
     packages=find_packages(),
-    version='0.12',
+    version='0.13',
     license='MIT',
     description='Sparse data classification using Graph of Graphs models',
     author='Shachar Hananya',
     author_email='shacharhananya@gmail.com',
     url='https://github.com/HananyaS/SpaGoG',
-    download_url='https://github.com/HananyaS/SpaGoG/archive/refs/tags/v_0.12.tar.gz',
+    download_url='https://github.com/HananyaS/SpaGoG/archive/refs/tags/v_0.13.tar.gz',
     keywords=["GoG"],
     install_requires=[
         'pandas',
         'torch',
         'torch_geometric',
     ],
 )
```

### Comparing `SpaGoG-0.12/spagog/datasets/graphDataPair.py` & `SpaGoG-0.13/spagog/datasets/graphDataPair.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import torch
 import numpy as np
-from datasets.tabDataPair import TabDataPair
+
+from .tabDataPair import TabDataPair
 from typing import Type, Union
 from torch.utils.data import DataLoader, Dataset
 
 from copy import deepcopy
 
-from utils.data.tab2graph import fill_data_gfp
+import sys
+
+sys.path.insert(1, "../")
+
+from ..utils.data.tab2graph import fill_data_gfp
 
 
 class GraphDataPair(TabDataPair):
     _input_types = Union[np.ndarray, torch.Tensor]
 
     def __init__(
         self,
```

### Comparing `SpaGoG-0.12/spagog/datasets/graphDataset.py` & `SpaGoG-0.13/spagog/datasets/graphDataset.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.12/spagog/datasets/graphsDataPair.py` & `SpaGoG-0.13/spagog/datasets/graphsDataPair.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
-from datasets.graphDataPair import GraphDataPair
+from .graphDataPair import GraphDataPair
 
 import numpy as np
 from typing import List, Union, Tuple
 
-from utils.data.tab2graph import tab2graphs
+from ..utils.data.tab2graph import tab2graphs
 from torch.utils.data import Dataset, DataLoader
 
 
 class GraphsDataPair:
     _input_types = Union[torch.Tensor, np.ndarray]
 
     def __init__(
```

### Comparing `SpaGoG-0.12/spagog/datasets/graphsDataset.py` & `SpaGoG-0.13/spagog/datasets/graphsDataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import copy
 
 import torch
 import numpy as np
 from typing import List, Union
 
-from datasets.graphsDataPair import GraphsDataPair
-from datasets.tabDataset import TabDataset
+from .graphsDataPair import GraphsDataPair
+from .tabDataset import TabDataset
 
-from utils.data.tab2graph import tab2graphs
+from ..utils.data.tab2graph import tab2graphs
 
 from operator import itemgetter
 
 
 class GraphsDataset:
     _input_types = Union[torch.Tensor, np.ndarray]
```

### Comparing `SpaGoG-0.12/spagog/datasets/tabDataPair.py` & `SpaGoG-0.13/spagog/datasets/tabDataPair.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.12/spagog/datasets/tabDataset.py` & `SpaGoG-0.13/spagog/datasets/tabDataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import sys
+
 import numpy as np
 import pandas as pd
 
 import torch
 from torch.utils.data import DataLoader
 
 from typing import Union
-from datasets.tabDataPair import TabDataPair
+
+from .tabDataPair import TabDataPair
 
 from sklearn.feature_selection import mutual_info_classif
 from scipy.sparse import csr_matrix
 
 from sklearn.model_selection import train_test_split
```

### Comparing `SpaGoG-0.12/spagog/experiments.py` & `SpaGoG-0.13/spagog/experiments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 import torch
 
-from datasets.tabDataset import TabDataset
-from datasets.graphsDataset import GraphsDataset
+from .datasets.tabDataset import TabDataset
+from .datasets.graphsDataset import GraphsDataset
 
-from models.graphClassification import ValuesAndGraphStructure as GC
-from models.graphNodeClassification import GraphNodeClassification as GNC
-from models.nodeClassification import NodeClassification
+from .models.graphClassification import ValuesAndGraphStructure as GC
+from .models.graphNodeClassification import GraphNodeClassification as GNC
+from .models.nodeClassification import NodeClassification
 
 PROJECT_DIR = "."
 
 
 def run_gc(
         tab_dataset: TabDataset,
         params: dict,
```

### Comparing `SpaGoG-0.12/spagog/main.py` & `SpaGoG-0.13/spagog/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import json
 import warnings
 
 import torch
 import pandas as pd
 import numpy as np
 
-from experiments import run_gc, run_gnc, run_gc_nc, get_default_params_file, get_tab_data
+from .experiments import run_gc, run_gnc, run_gc_nc, get_default_params_file, get_tab_data
+from .default_params.load_params import load_params
 
 warnings.filterwarnings("ignore")
 
 PROJECT_DIR = "."
 os.chdir(PROJECT_DIR)
 
 
@@ -37,23 +38,18 @@
     assert verbosity in [0, 1, 2], "Please provide a valid verbosity level {0, 1, 2}"
 
     if verbosity > 0:
         _st = time.time()
 
     is_graph = edges is not None
 
-    params = get_default_params_file(model)
-
-    with open(params, "r") as f:
-        params = json.load(f)
+    params = load_params(model)
 
     if model == "gnc" and params.get("gc_pretrain", False):
-        gc_default_params_file = get_default_params_file("gc")
-        with open(gc_default_params_file, "r") as f:
-            gc_params = json.load(f)
+        gc_params = load_params("gc")
 
         params["gc_params"] = gc_params
 
     for k, v in spec_params.items():
         if k in params.keys():
             params[k] = v
```

### Comparing `SpaGoG-0.12/spagog/models/abstractNN.py` & `SpaGoG-0.13/spagog/models/abstractNN.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from torch.utils.data import DataLoader
 
 from typing import Callable, List
 from sklearn.metrics import roc_auc_score
 
 from .abstractModel import AbstractModel
 
-from utils.metrics.metrics import find_best_metrics_bin, find_best_metrics_multi
+from ..utils.metrics.metrics import find_best_metrics_bin, find_best_metrics_multi
 
 
 class AbstractNN(nn.Module, AbstractModel):
     def __init__(
         self,
         device: torch.device = torch.device("cpu")
         if not torch.cuda.is_available()
```

### Comparing `SpaGoG-0.12/spagog/models/graphClassification.py` & `SpaGoG-0.13/spagog/models/graphClassification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import torch.nn as nn
 from torch.nn.functional import one_hot
 from .abstractNN import AbstractNN
 from typing import Union, Type, List
 from torch.utils.data import DataLoader
-from datasets.graphsDataset import GraphsDataset
+from ..datasets.graphsDataset import GraphsDataset
 
 
 class ValuesAndGraphStructure(AbstractNN):
     def __init__(
             self,
             nodes_number: int = None,
             feature_size: int = None,
```

### Comparing `SpaGoG-0.12/spagog/models/graphNodeClassification.py` & `SpaGoG-0.13/spagog/models/graphNodeClassification.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 import numpy as np
 import matplotlib.pyplot as plt
 
 import torch
 from torch import nn
 from torch import optim
 
-from datasets.graphsDataset import GraphsDataset
+from ..datasets.graphsDataset import GraphsDataset
 
-from utils.metrics.metrics import find_best_metrics_bin
+from ..utils.metrics.metrics import find_best_metrics_bin
 
 MODEL = "gnc"
 PROJECT_DIR = "."
 sys.path.append(PROJECT_DIR)
 
-from models.abstractModel import AbstractModel
-from models.nodeClassification import NodeClassification
-from models.graphClassification import ValuesAndGraphStructure
+from .abstractModel import AbstractModel
+from .nodeClassification import NodeClassification
+from .graphClassification import ValuesAndGraphStructure
 
 from typing import Dict
 
 from sklearn.metrics import roc_auc_score
 from torch.nn.functional import one_hot
 
-from utils.metrics.metrics import find_best_metrics_multi
+from ..utils.metrics.metrics import find_best_metrics_multi
 
 
 class GraphNodeClassification(nn.Module, AbstractModel):
     def predict(self, graphs_loader, inter_samples_edges, mask, clf_from, probs, to_numpy=True, *args, **kwargs):
         final_output, gc_output = self(
             graphs_loader,
             inter_samples_edges,
```

### Comparing `SpaGoG-0.12/spagog/models/nodeClassification.py` & `SpaGoG-0.13/spagog/models/nodeClassification.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.12/spagog/utils/data/tab2graph.py` & `SpaGoG-0.13/spagog/utils/data/tab2graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 import numpy as np
 import pandas as pd
 
-from datasets.tabDataPair import TabDataPair
+from ...datasets.tabDataPair import TabDataPair
 
-from utils.gfp import GFP
-from utils.knn import KNN
+from ..gfp import GFP
+from ..knn import KNN
 
 from copy import deepcopy
 from typing import Union, Type
 
 from itertools import combinations
```

### Comparing `SpaGoG-0.12/spagog/utils/gfp.py` & `SpaGoG-0.13/spagog/utils/gfp.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.12/spagog/utils/knn.py` & `SpaGoG-0.13/spagog/utils/knn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 
 import numpy as np
 import torch
-from datasets.tabDataPair import TabDataPair
+from ..datasets.tabDataPair import TabDataPair
 
 from copy import deepcopy
 
 from typing import Type
 
 
 class KNN:
```

### Comparing `SpaGoG-0.12/spagog/utils/metrics/metrics.py` & `SpaGoG-0.13/spagog/utils/metrics/metrics.py`

 * *Files identical despite different names*

