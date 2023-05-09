# Comparing `tmp/beam-ds-2.0.2.tar.gz` & `tmp/beam-ds-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beam-ds-2.0.2.tar", last modified: Sun Apr 16 19:45:05 2023, max compression
+gzip compressed data, was "beam-ds-2.0.3.tar", last modified: Tue May  9 08:17:10 2023, max compression
```

## Comparing `beam-ds-2.0.2.tar` & `beam-ds-2.0.3.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 19:40:34.637224 beam-ds-2.0.2/
--rw-r--r--   0 root         (0) root         (0)     1080 2023-04-01 19:19:43.000000 beam-ds-2.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2184 2023-04-16 19:40:34.638217 beam-ds-2.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1767 2023-04-01 19:19:43.000000 beam-ds-2.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)      114 2023-04-01 19:19:43.000000 beam-ds-2.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      718 2023-04-16 19:40:34.647206 beam-ds-2.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-01 19:19:43.000000 beam-ds-2.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 19:40:34.510285 beam-ds-2.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 19:40:34.614237 beam-ds-2.0.2/src/beam/
--rw-r--r--   0 root         (0) root         (0)      909 2023-04-14 13:16:22.000000 beam-ds-2.0.2/src/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-16 19:37:48.000000 beam-ds-2.0.2/src/beam/_version.py
--rw-r--r--   0 root         (0) root         (0)    52097 2023-04-15 21:36:48.000000 beam-ds-2.0.2/src/beam/algorithm.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/beam_mlflow.py
--rw-r--r--   0 root         (0) root         (0)    17001 2023-04-15 21:36:48.000000 beam-ds-2.0.2/src/beam/config.py
--rw-r--r--   0 root         (0) root         (0)    75918 2023-04-13 20:08:35.000000 beam-ds-2.0.2/src/beam/data.py
--rw-r--r--   0 root         (0) root         (0)    12112 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/data_tensor.py
--rw-r--r--   0 root         (0) root         (0)    25836 2023-04-14 14:04:41.000000 beam-ds-2.0.2/src/beam/dataset.py
--rw-r--r--   0 root         (0) root         (0)    36437 2023-04-15 21:52:36.000000 beam-ds-2.0.2/src/beam/experiment.py
--rw-r--r--   0 root         (0) root         (0)    32143 2023-04-09 04:35:52.000000 beam-ds-2.0.2/src/beam/model.py
--rw-r--r--   0 root         (0) root         (0)    13309 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/optim.py
--rw-r--r--   0 root         (0) root         (0)     9613 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/packed_folds.py
--rw-r--r--   0 root         (0) root         (0)    12102 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/parallel.py
--rw-r--r--   0 root         (0) root         (0)    21001 2023-04-16 19:14:33.000000 beam-ds-2.0.2/src/beam/path.py
--rw-r--r--   0 root         (0) root         (0)    15377 2023-04-02 17:55:04.000000 beam-ds-2.0.2/src/beam/processor.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/server.py
--rw-r--r--   0 root         (0) root         (0)    35911 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/ssl.py
--rw-r--r--   0 root         (0) root         (0)    11533 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/study.py
--rw-r--r--   0 root         (0) root         (0)    51731 2023-04-15 21:13:48.000000 beam-ds-2.0.2/src/beam/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 19:40:34.632751 beam-ds-2.0.2/src/beam_ds.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2184 2023-04-16 19:40:34.000000 beam-ds-2.0.2/src/beam_ds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      608 2023-04-16 19:40:34.000000 beam-ds-2.0.2/src/beam_ds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 19:40:34.000000 beam-ds-2.0.2/src/beam_ds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-16 19:40:34.000000 beam-ds-2.0.2/src/beam_ds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-16 19:40:34.000000 beam-ds-2.0.2/src/beam_ds.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:17:10.547906 beam-ds-2.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1060 2022-12-12 12:28:22.000000 beam-ds-2.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-05-09 08:17:10.547906 beam-ds-2.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-05-09 08:15:35.000000 beam-ds-2.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      107 2022-12-12 12:28:27.000000 beam-ds-2.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      718 2023-05-09 08:17:10.547906 beam-ds-2.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       37 2023-03-15 09:05:53.000000 beam-ds-2.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:17:10.543907 beam-ds-2.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:17:10.543907 beam-ds-2.0.3/src/beam/
+-rw-r--r--   0 root         (0) root         (0)      941 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/_version.py
+-rw-r--r--   0 root         (0) root         (0)    52272 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/beam_mlflow.py
+-rw-r--r--   0 root         (0) root         (0)    17480 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/config.py
+-rw-r--r--   0 root         (0) root         (0)    80093 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/data.py
+-rw-r--r--   0 root         (0) root         (0)    16059 2022-12-04 11:58:49.000000 beam-ds-2.0.3/src/beam/data1.py
+-rw-r--r--   0 root         (0) root         (0)    12112 2023-05-09 08:15:17.000000 beam-ds-2.0.3/src/beam/data_tensor.py
+-rw-r--r--   0 root         (0) root         (0)    25884 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    37770 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/experiment.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-02-09 08:05:12.000000 beam-ds-2.0.3/src/beam/explorer.py
+-rw-r--r--   0 root         (0) root         (0)     9342 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/logger.py
+-rw-r--r--   0 root         (0) root         (0)    32178 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/model.py
+-rw-r--r--   0 root         (0) root         (0)    13327 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/optim.py
+-rw-r--r--   0 root         (0) root         (0)     9608 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/packed_folds.py
+-rw-r--r--   0 root         (0) root         (0)    12334 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/parallel.py
+-rw-r--r--   0 root         (0) root         (0)    21313 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/path.py
+-rw-r--r--   0 root         (0) root         (0)    17439 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/processor.py
+-rw-r--r--   0 root         (0) root         (0)     3008 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/server.py
+-rw-r--r--   0 root         (0) root         (0)    35926 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/ssl.py
+-rw-r--r--   0 root         (0) root         (0)    11794 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/study.py
+-rw-r--r--   0 root         (0) root         (0)    17775 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/tensor.py
+-rw-r--r--   0 root         (0) root         (0)    56371 2023-05-09 08:15:35.000000 beam-ds-2.0.3/src/beam/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:17:10.547906 beam-ds-2.0.3/src/beam_ds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-05-09 08:17:10.000000 beam-ds-2.0.3/src/beam_ds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      685 2023-05-09 08:17:10.000000 beam-ds-2.0.3/src/beam_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 08:17:10.000000 beam-ds-2.0.3/src/beam_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-09 08:17:10.000000 beam-ds-2.0.3/src/beam_ds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-09 08:17:10.000000 beam-ds-2.0.3/src/beam_ds.egg-info/top_level.txt
```

### Comparing `beam-ds-2.0.2/LICENSE` & `beam-ds-2.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 elad
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2021 elad
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `beam-ds-2.0.2/PKG-INFO` & `beam-ds-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: beam-ds
-Version: 2.0.2
+Version: 2.0.3
 Summary: Beam Datascience package
 Home-page: https://github.com/mlutils/beamds
 Author: Beam Maintainer
 Author-email: author@example.com
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mlutils/beamds/issues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -71,14 +73,31 @@
 
 Scalene is a high-performance python profiler that supports GPU profiling. 
 To analyze your code with Scalene use the following arguments:
 ```shell
 scalene --reduced-profile --outfile OUTFILE.html --html --- your_prog.py <your additional arguments>
 ```
 
+## Uploading the package to PyPi
+
+1. Install twine:
+```shell
+python -m pip install --user --upgrade twine
+```
+
+2. Build the package:
+```shell
+python -m build
+```
+
+3. Upload the package:
+```shell
+python -m twine upload --repository pypi dist/* 
+```
+
```

### Comparing `beam-ds-2.0.2/README.md` & `beam-ds-2.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,31 @@
 
 Scalene is a high-performance python profiler that supports GPU profiling. 
 To analyze your code with Scalene use the following arguments:
 ```shell
 scalene --reduced-profile --outfile OUTFILE.html --html --- your_prog.py <your additional arguments>
 ```
 
+## Uploading the package to PyPi
+
+1. Install twine:
+```shell
+python -m pip install --user --upgrade twine
+```
+
+2. Build the package:
+```shell
+python -m build
+```
+
+3. Upload the package:
+```shell
+python -m twine upload --repository pypi dist/* 
+```
+
```

### Comparing `beam-ds-2.0.2/setup.cfg` & `beam-ds-2.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.2/src/beam/__init__.py` & `beam-ds-2.0.3/src/beam/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from .dataset import UniversalBatchSampler, UniversalDataset
 from .packed_folds import PackedFolds
 from .config import get_beam_parser, beam_arguments
 from .config import boolean_feature as beam_boolean_feature
 from .experiment import Experiment, beam_algorithm_generator
 from .study import Study
-from .utils import setup_distributed, cleanup, check_type, slice_to_index, beam_logger, beam_device, as_tensor, \
+from .utils import setup_distributed, cleanup, check_type, slice_to_index, beam_device, as_tensor, \
     batch_augmentation, as_numpy
 from .utils import tqdm_beam as tqdm
 from .algorithm import Algorithm
 from .model import LinearNet, PackedSet, BetterEmbedding, SplineEmbedding, copy_network, reset_network
-from .data_tensor import DataTensor
+from .tensor import DataTensor
 from .optim import BeamOptimizer, BeamScheduler
+from .logger import beam_logger, beam_kpi, Timer
 # from .ssl import BeamSimilarity, Similarities, BeamSSL, BYOL, BeamVICReg, BarlowTwins, VICReg, SimCLR, SimSiam
 # from .server import BeamServer, BeamClient
 
 from ._version import __version__
```

### Comparing `beam-ds-2.0.2/src/beam/algorithm.py` & `beam-ds-2.0.3/src/beam/algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,40 @@
 import math
 from collections import defaultdict
 from torch import nn
 import torch
 import copy
 from .utils import tqdm_beam as tqdm
-from .utils import logger
+from .logger import beam_logger as logger
 import numpy as np
 from .optim import BeamOptimizer, BeamScheduler, MultipleScheduler
 from torch.nn.parallel import DistributedDataParallel as DDP
 from .utils import finite_iterations, to_device, check_type, rate_string_format, concat_data, \
-    stack_batched_results, as_numpy, stack_train_results
+    stack_batched_results, as_numpy, stack_train_results, beam_device, retrieve_name
 from .config import beam_arguments, get_beam_parser
 from .dataset import UniversalBatchSampler, UniversalDataset, TransformedDataset, DataBatch
 from .experiment import Experiment
 from timeit import default_timer as timer
 from ray import tune
 from .path import beam_path, BeamPath
 from .processor import Processor
-
-
-# class BeamResult(object):
-#
-#     def __init__(self, data_batch, results, objective, objective_name, objective_direction,
-#     best_state, best_objective, best_objective_name, best_objective_direction):
-#
-#         self.data_batch = data_batch
-#         self.results = results
-#         self.objective = objective
-#         self.objective_name = objective_name
-#         self.objective_direction = objective_direction
-#         self.best_state = best_state
-#         self.best_objective = best_objective
-#         self.best_objective_name = best_objective_name
-#         self.best_objective_direction = best_objective_direction
+from .logger import beam_kpi
 
 
 class Algorithm(object):
 
-    def __init__(self, hparams, networks=None, optimizers=None, schedulers=None, processors=None, dataset=None):
+    def __init__(self, hparams, networks=None, optimizers=None, schedulers=None, processors=None, dataset=None,
+                 name=None, **kwargs):
 
         self._experiment = None
         self.trial = None
 
         self.hparams = hparams
 
-        self.device = hparams.device
+        self.device = beam_device(hparams.device)
         self.ddp = hparams.ddp
         self.hpo = hparams.hpo
 
         self.rank = hparams.rank
         self.world_size = hparams.world_size
 
         # some experiment hyperparameters
@@ -89,26 +75,33 @@
         self.dataset = None
         self.persistent_dataloaders = {}
         self.dataloaders = {}
         self.eval_subset = None
         self.objective = None
         self.best_objective = None
         self.best_state = False
+        self._name = name
 
         self.add_components(networks=networks, optimizers=optimizers, schedulers=schedulers, processors=processors)
 
         if hparams.reload_path is not None:
             self.load_checkpoint(hparams.reload_path)
 
         if hparams.store_initial_weights:
             self.initial_weights = self.save_checkpoint()
 
         if dataset is not None:
             self.load_dataset(dataset)
 
+    @property
+    def name(self):
+        if self._name is None:
+            self._name = retrieve_name(self)
+        return self._name
+
     def get_hparam(self, hparam, specific=None, default=None):
 
         if type(specific) is list:
             for s in specific:
                 if f"{s}_{hparam}" in self.hparams:
                     return getattr(self.hparams, f"{specific}_{hparam}")
         elif specific is not None and f"{specific}_{hparam}" in self.hparams:
@@ -131,23 +124,25 @@
         return self
 
     @staticmethod
     def get_parser():
         return get_beam_parser()
 
     @classmethod
-    def from_pretrained(cls, path=None, override_hparams=None, hparams=None, **kwargs):
+    def from_pretrained(cls, path=None, override_hparams=None, hparams=None, Dataset=None, alg_args=None, alg_kwargs=None,
+                             dataset_args=None, dataset_kwargs=None, **kwargs):
         if path is not None:
             experiment = Experiment.reload_from_path(path, override_hparams=override_hparams)
         elif hparams is not None:
             experiment = Experiment(hparams)
         else:
             hparams = beam_arguments(cls.get_parser(), **kwargs)
             experiment = Experiment(hparams)
-        return experiment.algorithm_generator(cls)
+        return experiment.algorithm_generator(cls, Dataset=Dataset, alg_args=alg_args, alg_kwargs=alg_kwargs,
+                             dataset_args=dataset_args, dataset_kwargs=dataset_kwargs)
 
     def add_components(self, networks=None, optimizers=None, schedulers=None, processors=None,
                        build_optimizers=True, build_schedulers=True, name='net'):
 
         if networks is None:
             networks = self.networks
         else:
@@ -536,15 +531,15 @@
 
         for k, scheduler in self.schedulers_flat.items():
             if type(scheduler) is BeamScheduler:
 
                 k, ki = self.split_names(k)
 
                 state = self.schedulers_initial_state[k] if k in self.schedulers_initial_state else None
-                if ki is not None and k is not None:
+                if ki is not None and state is not None:
                     state = state[ki]
 
                 scheduler.update_total_steps(epochs=self.n_epochs,
                                              steps_per_epochs=self.epoch_length['train'], initial_state=state)
 
     def get_optimizer_name(self, opt):
         i = id(opt)
@@ -875,15 +870,15 @@
         return False
 
     def __call__(self, subset, predicting=False, enable_tqdm=None, max_iterations=None, head=None, eval_mode=True,
                  return_dataset=None, **kwargs):
 
         with torch.no_grad():
 
-            self.set_mode(training=eval_mode)
+            self.set_mode(training= not eval_mode)
             results = defaultdict(lambda: defaultdict(list))
             transforms = []
             index = []
 
             desc = subset if type(subset) is str else ('predict' if predicting else 'evaluate')
 
             if enable_tqdm is None:
@@ -1167,14 +1162,22 @@
 
     def evaluate(self, *args, **kwargs):
         '''
         For validation and test purposes (when labels are known)
         '''
         return self(*args, predicting=False, **kwargs)
 
-    def predict(self, dataset, *args, lazy=False, **kwargs):
+    def predict(self, dataset, *args, lazy=False, kpi=True, **kwargs):
         '''
         For real data purposes (when labels are unknown)
         '''
         if lazy:
             return TransformedDataset(dataset, self, *args, **kwargs)
-        return self(dataset, *args, predicting=True, **kwargs)
+
+        if not kpi:
+            self(dataset, *args, predicting=True, **kwargs)
+
+        @beam_kpi
+        def predict_wrapper(sample, algorithm=None, **kwargs):
+            return algorithm(sample, predicting=True, **kwargs)
+
+        return predict_wrapper(dataset, algorithm=self, *args, **kwargs)
```

### Comparing `beam-ds-2.0.2/src/beam/config.py` & `beam-ds-2.0.3/src/beam/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import copy
 import os
 import sys
-from .utils import is_notebook, check_type, logger
+from .utils import is_notebook, check_type
+from .logger import beam_logger as logger
 import re
 import math
 
 
 def boolean_feature(parser, feature, default=False, help='', metavar=None):
     featurename = feature.replace("-", "_")
     feature_parser = parser.add_mutually_exclusive_group(required=False)
@@ -185,14 +186,19 @@
                         help='when to store results to pickle files')
     parser.add_argument('--store-networks', type=str, default='logscale',
                         help='when to store network weights to the log directory')
 
     parser.add_argument('--mp-context', type=str, default='spawn', help='The multiprocessing context to use')
     parser.add_argument('--mp-backend', type=str, default=None, help='The multiprocessing backend to use')
 
+    boolean_feature(parser, "comet", False, "Whether to use comet.ml for logging")
+    parser.add_argument('--git-directory', type=str, default=None, help='The git directory to use for comet.ml logging')
+    parser.add_argument('--comet-api-key', type=str, default=None, help='The comet.ml api key to use for logging')
+    parser.add_argument('--comet-workspace', type=str, default=None, help='The comet.ml workspace to use for logging')
+
     return parser
 
 
 def normalize_key(k):
     return k.replace('-', '_')
 
 def normalize_value(v):
```

### Comparing `beam-ds-2.0.2/src/beam/data.py` & `beam-ds-2.0.3/src/beam/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+import copy
 import itertools
 import numpy as np
 import torch
 from .utils import check_type, slice_to_index, as_tensor, to_device, recursive_batch, as_numpy, beam_device, \
     recursive_device, container_len, recursive, recursive_len, recursive_shape, recursive_types, retrieve_name
 import pandas as pd
 import math
 from collections import namedtuple
-from .utils import divide_chunks, collate_chunks, recursive_chunks, iter_container, logger, \
-    recursive_size_summary, container_len, is_arange, is_chunk, \
+from .utils import divide_chunks, collate_chunks, recursive_chunks, iter_container, \
+    recursive_size_summary, container_len, is_arange, is_chunk, is_container, \
     recursive_size, recursive_flatten, recursive_collate_chunks, recursive_keys, recursive_slice_columns, \
     recursive_slice, recursive_flatten_with_keys, get_item_with_tuple_key, PureBeamPath, set_item_with_tuple_key, \
     get_closest_item_with_tuple_key
-import os
+from .logger import beam_logger as logger
 from .path import BeamPath, beam_path
 from functools import partial
 from collections import defaultdict
 import time
+from copy import deepcopy
+
 
 DataBatch = namedtuple("DataBatch", "index label data")
 
 
 class Groups(object):
 
     def __init__(self, groupby_pointer):
@@ -102,15 +105,16 @@
     index_partition_directory_name = '.index_part'
     columns_partition_directory_name = '.columns_part'
 
     def __init__(self, *args, data=None, path=None, name=None, all_paths=None,
                  index=None, label=None, columns=None, lazy=True, device=None, target_device=None, schema=None,
                  override=True, compress=None, split_by='keys', chunksize=int(1e9), chunklen=None, n_chunks=None,
                  key_map=None, partition=None, archive_size=int(1e6), preferred_orientation='columns', read_kwargs=None,
-                 write_kwargs=None, quick_getitem=False, orientation=None, glob_filter=None, info=None, **kwargs):
+                 write_kwargs=None, quick_getitem=False, orientation=None, glob_filter=None, info=None,
+                 write_metadata=True, metadata_path_prefix=None, **kwargs):
 
         '''
 
         @param args:
         @param data:
         @param path: if not str, requires to support the pathlib Path attributes and operations, can be container of paths
         @param lazy:
@@ -151,24 +155,26 @@
         self.override = override
         self.compress = compress
         self.chunksize = chunksize
         self.chunklen = chunklen
         self.n_chunks = n_chunks
         self.partition = partition
         self.archive_size = archive_size
-        self.target_device = target_device
+        self.target_device = beam_device(target_device)
         self._index = index
         self._label = label
         self._schema = schema
         self.columns = columns
         self.preferred_orientation = preferred_orientation
         self.split_by = split_by
         self.quick_getitem = quick_getitem
         self.glob_filter = glob_filter
         self._key_map = key_map
+        self.write_metadata = write_metadata
+        self.metadata_path_prefix = beam_path(metadata_path_prefix)
 
         self.stored = False
         self.cached = True
 
         self._columns_map = None
         self._device = None
         self._len = None
@@ -180,15 +186,17 @@
         self._flatten_items = None
         self._size = None
         self._total_size = None
         self._conf = None
         self._info_groups = None
         self._all_paths = None
         self._root_path = None
+        self._keys = None
         self._metadata_paths = None
+        self._metadata_path_exists = {}
         self.groups = Groups(self.get_info_groups)
 
         self._info = info
         self._orientation = orientation
 
         self.iloc = Iloc(self)
         self.loc = Loc(self)
@@ -208,74 +216,95 @@
             self.data = data
         else:
             self.data = None
             self.cached = False
             # in this case the data is not cached, so it should be stored ether in root_path or in all_paths
 
         if device is not None:
+            device = beam_device(device)
             self.as_tensor(device=device)
+            self._device = device
 
         path = beam_path(path)
-        path_type = check_type(path)
 
         self._name = name
 
         if path is not None:
             self._name = path.name
         else:
             self._name = None
 
-        if path_type.major == 'container':
+        if is_container(path):
             self._all_paths = path
         elif path is not None:
 
-            self._root_path, self._all_paths, self._metadata_paths = BeamData.single_file_case(path, all_paths,
+            self._root_path, self._all_paths, self._metadata_paths = self.single_file_case(path, all_paths,
                                                                                                self._metadata_paths)
             self._root_path = path
 
         if ((self._all_paths is not None) or (self._root_path is not None and self._root_path.not_empty())) and \
                 not self.cached:
             self.stored = True
             if not lazy:
                 self.cache()
 
     @property
     def metadata_paths(self):
 
         if self._metadata_paths is not None:
             return self._metadata_paths
-        self._metadata_paths = {k: self.root_path.joinpath(v) for k, v in BeamData.metadata_files.items()}
 
+        root_path = self.root_path
+        if self.metadata_path_prefix is not None:
+            if self.metadata_path_prefix.is_absolute():
+                root_path = self.metadata_path_prefix
+            else:
+                root_path = self.root_path.joinpath(self.metadata_path_prefix)
+
+        self._metadata_paths = {k: root_path.joinpath(v) for k, v in BeamData.metadata_files.items()}
         return self._metadata_paths
 
     @property
     def root_path(self):
         if self._root_path is not None:
             return self._root_path
 
         if self.all_paths is not None:
             self._root_path = self.recursive_root_finder(self.all_paths)
             return self._root_path
 
         return self._root_path
 
+    @staticmethod
+    def clear_metadata(path):
+        path = beam_path(path)
+        if path.is_file():
+            name = path.stem
+            if name in ['.all_paths', '.info', '.conf']:
+                path.unlink()
+        elif path.is_dir():
+            for new_path in list(path):
+                BeamData.clear_metadata(new_path)
+
     @property
     def all_paths(self):
 
         if self._all_paths is not None:
             return self._all_paths
 
         if self.stored:
             path = self.metadata_paths['all_paths']
-            if path.exists():
+            if self.write_metadata and path.exists():
+                logger.debug(f"Reading all_paths file: {path}")
                 self._all_paths = path.read()
 
             else:
                 self._all_paths = BeamData.recursive_map_path(self.root_path, glob_filter=self.glob_filter)
-                BeamData.write_file(self._all_paths, path)
+                if self.write_metadata:
+                    BeamData.write_file(self._all_paths, path)
 
         return self._all_paths
 
     def get_info_groups(self):
         if self._info_groups is not None:
             return self._info_groups
         self._info_groupby = self.info.groupby('fold')
@@ -287,58 +316,61 @@
             return self._index
 
         if self.stored:
 
             for path in self.metadata_paths['index'].parent.iterdir():
                 if path.stem == BeamData.metadata_files['index']:
                     if path.exists():
+                        logger.debug(f"Reading index file: {path}")
                         self._index = path.read()
                         return self._index
-
-        info = self.info
-        if self.orientation in ['columns', 'simple',  'simplified_index']:
-            self._index = info.index.values
-        else:
-            # TODO: support index for packed and index case
-            self._index = None
-            # info_filtered = BeamData.recursive_filter(self.size, self.info)
-            # if info_filtered is not None:
-            #     self._index = info_filtered.index
-            #     if self._objects_type == 'tensor':
-            #
-            #         func = partial(as_tensor, device=self.device, dtype=None, return_vector=False)
-            #         self._index = recursive(func)(self._index)
+        if self.cached:
+            info = self.info
+            if self.orientation in ['columns', 'simple',  'simplified_index']:
+                self._index = info.index.values
+            else:
+                # TODO: support index for packed and index case
+                @recursive
+                def replace_key_map_with_index(ind):
+                    return self.info[self.info.fold == ind].index.values
+                self._index = replace_key_map_with_index(deepcopy(self.key_map))
 
         return self._index
 
     @property
     def label(self):
 
         if self._label is not None:
             return self._label
 
         if self.stored:
 
             for path in self.metadata_paths['label'].parent.iterdir():
                 if path.stem == BeamData.metadata_files['label']:
                     if path.exists():
+                        logger.debug(f"Reading label file: {path}")
                         self._label = path.read()
                         return self._label
 
         return self._label
 
-    @staticmethod
-    def single_file_case(root_path, all_paths, metadata_paths):
+    def single_file_case(self, root_path, all_paths, metadata_paths):
 
-        if root_path.parent.is_dir():
+        if all_paths is None and not root_path.is_root() and root_path.parent.is_dir():
             for p in root_path.parent.iterdir():
                 if p.stem == root_path.stem and p.is_file():
 
-                    meta_path = p.parent.joinpath(f'.{p.name}')
-                    meta_path.mkdir(exist_ok=True)
+                    meta_root_path = p.parent
+                    if self.metadata_path_prefix is not None:
+                        if self.metadata_path_prefix.is_absolute():
+                            meta_root_path = self.metadata_path_prefix
+                        else:
+                            meta_root_path = meta_root_path.joinpath(self.metadata_path_prefix)
+
+                    meta_path = meta_root_path.joinpath(f'.{p.name}')
                     metadata_paths = {k: meta_path.joinpath(v) for k, v in BeamData.metadata_files.items()}
                     root_path = p
                     all_paths = {'data': ''}
                     break
 
         return root_path, all_paths, metadata_paths
 
@@ -436,46 +468,48 @@
 
         if self._objects_type is not None:
             return self._objects_type
 
         objects_types = recursive_flatten(self.data_types)
         objects_types = [v.minor for v in objects_types if v.minor != 'none']
 
-        u = np.unique(objects_types)
+        u = set(objects_types)
 
         if len(u) == 1:
-            self._objects_type = u[0]
+            self._objects_type = next(iter(u))
         else:
             self._objects_type = 'mixed'
 
         return self._objects_type
 
     @property
     def schema(self):
 
         if self._schema is not None:
             return self._schema
 
         if self.stored:
-            schema_path = self.metadata_paths['schema']
-            if schema_path.is_file():
+            if self.metadata_path_exists('schema'):
+                schema_path = self.metadata_paths['schema']
+                logger.debug(f"Reading schema file {schema_path}")
                 self._schema = schema_path.read()
                 return self._schema
 
         return self._schema
 
     @property
     def conf(self):
 
         if self._conf is not None:
             return self._conf
 
-        if self.stored:
-            conf_path = self.metadata_paths['conf']
-            if conf_path.is_file():
+        if self.stored and self.write_metadata:
+            if self.metadata_path_exists('conf'):
+                conf_path = self.metadata_paths['conf']
+                logger.debug(f"Reading conf file {conf_path}")
                 self._conf = conf_path.read()
                 return self._conf
 
         if self.cached:
             self._conf = {'orientation': self.orientation,
                           'objects_type': self.objects_type,
                           'len': len(self),
@@ -494,23 +528,29 @@
     def key_map(self):
         if self._key_map is not None:
             return self._key_map
         self._key_map = {k: i for i, (k, v) in enumerate(self.flatten_items.items())}
 
         return self._key_map
 
+    def metadata_path_exists(self, key):
+        if key not in self._metadata_path_exists:
+            self._metadata_path_exists[key] = self.metadata_paths[key].is_file()
+        return self._metadata_path_exists[key]
+
     @property
     def info(self):
 
         if self._info is not None:
             return self._info
 
-        if self.stored:
-            info_path = self.metadata_paths['info']
-            if info_path.is_file():
+        if self.stored and self.write_metadata:
+            if self.metadata_path_exists('info'):
+                info_path = self.metadata_paths['info']
+                logger.debug(f"Reading info file {info_path}")
                 self._info = info_path.read()
                 return self._info
 
         if self.cached:
 
             if self.orientation in ['index', 'packed']:
                 filtered_data = list(filter(lambda x: x is not None, self.flatten_data))
@@ -570,27 +610,30 @@
         if self.root_path is not None:
             logger.warning(f'path already set to {self.root_path}, overwriting with {value}')
         value = beam_path(value)
         if value.is_dir() and len(list(value.iterdir())):
             raise ValueError(f'path {value} is not empty')
         self._root_path = value
         self._all_paths = None
+        self._metadata_paths = None
         self.stored = False
 
     @property
     def index_mapper(self):
 
         info = self.info
         if 'map' in info.columns:
             return info['map']
 
         return None
 
     @staticmethod
     def normalize_key(key):
+        if type(key) is tuple:
+            key = '/'.join([BeamData.normalize_key(k) for k in key])
         if type(key) is not str:
             key = f'{key:06}'
         return key
 
     @property
     def flatten_data(self):
         if self._flatten_data is not None:
@@ -654,17 +697,15 @@
 
         if self._conf is not None:
             self._orientation = self._conf['orientation']
             return self._orientation
 
         if self.cached:
 
-            data_type = check_type(self.data)
-
-            if data_type.major != 'container':
+            if not is_container(self.data):
                 self._orientation = 'simple'
                 if hasattr(self.data, 'columns') and self.columns is None:
                     self.columns = self.data.columns
                 if hasattr(self.data, 'index') and self.index is None:
                     self._index = self.data.index
 
             else:
@@ -672,23 +713,23 @@
                 if self.preferred_orientation == 'columns':
                     lens = recursive_flatten(recursive_len([self.data]), flat_array=True)
                     lens = list(filter(lambda x: x is not None, lens))
 
                     lens_index = recursive_flatten(recursive_len([self._index]), flat_array=True)
                     lens_index = list(filter(lambda x: x is not None, lens_index))
 
-                    if len(np.unique(lens)) == 1 and len(lens_index) <= 1:
+                    if len(set(lens)) == 1 and len(lens_index) <= 1:
                         self._orientation = 'columns'
                         return self._orientation
 
                 shapes = recursive_flatten(recursive(lambda x: tuple(x.shape[1:])
                                                      if hasattr(x, 'shape') else None)([self.data]))
 
                 shapes = list(filter(lambda x: x is not None, shapes))
-                if len(np.unique(shapes)) == 1:
+                if len(set(shapes)) == 1:
                     self._orientation = 'index'
                 else:
                     self._orientation = 'packed'
 
         elif self.stored:
             self._orientation = self.conf['orientation']
 
@@ -724,14 +765,15 @@
         path = beam_path(path)
 
         if (not override) and path.exists():
             raise NameError(f"File {path} exists. "
                             f"Please specify write_file(...,overwrite=True) to write on existing file")
 
         path.clean()
+        logger.debug(f"Writing file: {path}")
         path = path.write(data, **kwargs)
 
         return path
 
     @staticmethod
     def get_schema_from_subset(schema, key, schema_type=None):
 
@@ -753,32 +795,32 @@
         for k in key:
             schema = BeamData.get_schema_from_subset(schema, k, schema_type=schema_type)
         return schema
 
     @staticmethod
     def containerize_keys_and_values(keys, values):
 
-        if not is_arange(keys):
+        argsort, isarange = is_arange(keys)
+        if not isarange:
             values = dict(zip(keys, values))
             # values = {k: values[k] for k in sorted(values.keys())}
         else:
-            values = [values[i] for i in np.argsort(keys)]
+            values = [values[i] for i in argsort]
 
         if type(values) is dict and 'data' in values and len(values) == 1:
             values = values['data']
 
         return values
 
     @staticmethod
     def recursive_root_finder(all_paths, head=None):
         if head is None:
             head = []
 
-        all_paths_type = check_type(all_paths)
-        if all_paths_type.major == 'container':
+        if is_container(all_paths):
 
             k, v = next(iter_container(all_paths))
             head.append(k)
             return BeamData.recursive_root_finder(v, head=head)
 
         if all_paths.is_file():
             return all_paths.parent.joinpath(all_paths.stem)
@@ -830,18 +872,23 @@
 
             # if the directory contains chunks it is considered as a single path
             if all([BeamData.index_chunk_file_extension in p.name for p in keys_paths]):
                 return relative_path
             elif all([BeamData.columns_chunk_file_extension in p.name for p in keys_paths]):
                 return relative_path
 
-            if not is_arange(keys):
+            argsort, isarange = is_arange(keys)
+
+            if not isarange:
                 values = dict(zip(keys, values))
             else:
-                values = [values[i] for i in np.argsort(keys)]
+                values = [values[i] for i in argsort]
+
+            if type(values) is dict and 'data' in values and len(values) == 1:
+                values = values['data']
 
             return values
 
         # we store the files without their extension? why?
         # if path.is_file():
         #     return path.parent.joinpath(path.stem)
         if path.is_file():
@@ -889,20 +936,18 @@
             self.cache()
 
         return self.data
 
     @staticmethod
     def read(paths, schema=None, **kwargs):
 
-        paths_type = check_type(paths)
-
         if paths is None:
             return None
 
-        if paths_type.major == 'container':
+        if is_container(paths):
             keys = []
             values = []
 
             schema_type = check_type(schema)
 
             for k, next_path in iter_container(paths):
 
@@ -913,14 +958,15 @@
             return BeamData.containerize_keys_and_values(keys, values)
 
         path = beam_path(paths)
         if schema is not None:
             kwargs = {**schema.read_schema, **kwargs}
 
         if path.is_file():
+            logger.debug(f"Reading file: {path}")
             return path.read(**kwargs)
 
         if path.is_dir():
 
             keys = []
             values = []
 
@@ -953,17 +999,15 @@
                    chunklen=None, n_chunks=None, partition=None, file_type=None, root=False, schema=None, **kwargs):
 
         path = beam_path(path)
 
         if sizes is None:
             sizes = recursive_size(data)
 
-        data_type = check_type(data)
-
-        if data_type.major == 'container':
+        if is_container(data):
 
             size_summary = sum(recursive_flatten(sizes, flat_array=True))
 
             if size_summary < archive_size:
 
                 if root:
                     path = path.joinpath(BeamData.default_data_file_name)
@@ -1097,19 +1141,22 @@
         if self.columns is not None:
             self._columns_map = {str(k): i for i, k in enumerate(self.columns)}
 
         self._columns_map = None
         return self._columns_map
 
     def keys(self):
-        if self.orientation == 'simple':
-            return self.columns
-        if self.cached:
-            return recursive_keys(self.data)
-        return recursive_keys(self.all_paths)
+        if self._keys is None:
+            if self.orientation == 'simple':
+                self._keys = self.columns
+            if self.cached:
+                self._keys = recursive_keys(self.data)
+            else:
+                self._keys = recursive_keys(self.all_paths)
+        return self._keys
 
     @property
     def dtypes(self):
         return recursive_types(self.data)
 
     @property
     def shape(self):
@@ -1194,15 +1241,18 @@
         self._total_size = sum(recursive_flatten(self.size, flat_array=True))
         return self._total_size
 
     def store(self, data=None, path=None, compress=None, chunksize=None,
               chunklen=None, n_chunks=None, partition=None, split_by=None,
               archive_size=None, override=True, **kwargs):
 
-        path = self.get_default('root_path', path)
+        if path is not None:
+            self.path = path
+        else:
+            path = self.path
 
         sizes = None
         if data is None:
             data = self.data
             sizes = self.size
 
         path.clean()
@@ -1210,36 +1260,35 @@
         kwargs = self.get_default_params(compress=compress, chunksize=chunksize, chunklen=chunklen, n_chunks=n_chunks,
                                          partition=partition, split_by=split_by, archive_size=archive_size,
                                          override=override, **kwargs)
 
         BeamData.write_tree(data, path, root=True, sizes=sizes, schema=self.schema, **kwargs)
 
         # store info and conf files
-        info_path = path.joinpath(BeamData.metadata_files['info'])
-        BeamData.write_object(self.info, info_path)
-        conf_path = path.joinpath(BeamData.metadata_files['conf'])
-        BeamData.write_object({**self.conf}, conf_path, archive=True)
-        conf_path = path.joinpath(BeamData.metadata_files['conf'])
-        BeamData.write_object({**self.conf}, conf_path, archive=True)
+        if self.write_metadata:
+            info_path = self.metadata_paths['info']
+            BeamData.write_object(self.info, info_path)
+            conf_path = self.metadata_paths['conf']
+            BeamData.write_object({**self.conf}, conf_path, archive=True)
+            conf_path = self.metadata_paths['conf']
+            BeamData.write_object({**self.conf}, conf_path, archive=True)
 
         # store index and label
         if self.index is not None:
-            index_path = path.joinpath(BeamData.metadata_files['index'])
+            index_path = self.metadata_paths['index']
             BeamData.write_object(self.index, index_path)
         if self.label is not None:
-            label_path = path.joinpath(BeamData.metadata_files['label'])
+            label_path = self.metadata_paths['label']
             BeamData.write_object(self.label, label_path)
 
         self.stored = True
-        self._root_path = path
         self.data = data
 
         self._all_paths = BeamData.recursive_map_path(self.root_path, glob_filter=self.glob_filter)
-        path = self.root_path.joinpath(BeamData.metadata_files['all_paths'])
-        BeamData.write_file(self._all_paths, path)
+        self.update_all_paths_file()
 
     def state_dict(self):
         if not self.cached:
             self.cache()
 
         return {'data': self.data, 'info': self.info, 'conf': self.conf, 'index': self.index, 'label': self.label,
                 'schema': self.schema}
@@ -1249,14 +1298,16 @@
         if root_path is None:
             root_path = self.root_path
 
         @recursive
         def _abs_all_paths(path):
             if path is None:
                 return None
+            if isinstance(path, list):
+                return [root_path.joinpath(p) for p in path]
             return root_path.joinpath(path)
 
         if all_paths is None:
             all_paths = self.all_paths
 
         return _abs_all_paths(all_paths)
 
@@ -1317,14 +1368,17 @@
         for param in reset_params:
             if param not in avoid_reset:
                 setattr(self, param, None)
 
         for param in args:
             setattr(self, param, None)
 
+        if 'metadata_path_exists' not in avoid_reset:
+            self._metadata_path_exists = {}
+
     def inverse_map(self, ind):
 
         ind = slice_to_index(ind, l=len(self), sliced=self.index)
 
         index_type = check_type(ind)
         if index_type.major == 'scalar':
             ind = [ind]
@@ -1418,14 +1472,23 @@
         if self.quick_getitem:
             return BeamData.data_batch(data=data, index=self.index, label=self.label)
 
         return self.clone(data=data, columns=columns, index=self.index, label=self.label, orientation=self.orientation)
 
     @property
     def stacked_values(self):
+
+        if not self.cached:
+            self.cache()
+
+        if self.orientation == 'packed':
+            raise ValueError("Cannot stack packed data")
+        elif self.orientation in ['simple', 'simplified_index']:
+            return self.data
+
         data = self.concatenate()
         return data
 
     @property
     def stacked_index(self):
         index = self.info.index
         return index
@@ -1492,81 +1555,86 @@
                 label = self.concatenate(recursive_flatten(label), orientation=self.orientation)
 
         if self.quick_getitem:
             return BeamData.data_batch(data=data, index=index, label=label)
 
         return self.clone(data=data, index=index, label=label)
 
-    @staticmethod
-    def recursive_filter(x, info):
+    def recursive_filter(self, x, info):
 
         if info is None:
             return None
 
         inf_g = info.groupby('fold')
-        folds = info['fold'].unique()
+        folds = set(info['fold'].unique())
 
         def _recursive_filter(xi, flat_key=0):
-            x_type = check_type(xi)
-            if x_type.major == 'container':
+
+            if is_container(xi):
 
                 keys = []
                 values = []
                 index = []
                 label = []
 
                 for k, v in iter_container(xi):
                     i, v, l, flat_key = _recursive_filter(v, flat_key=flat_key)
-                    if len(v):
+                    if v is not None:
                         values.append(v)
                         index.append(i)
                         keys.append(k)
                         label.append(l)
 
-                if not is_arange(keys):
+                argsort, isarange = is_arange(keys)
+                if not isarange:
                     values = dict(zip(keys, values))
                     index = dict(zip(keys, index))
                     label = dict(zip(keys, label))
                 else:
-                    values = [values[j] for j in np.argsort(keys)]
-                    index = [index[j] for j in np.argsort(keys)]
-                    label = [label[j] for j in np.argsort(keys)]
+                    values = [values[j] for j in argsort]
+                    index = [index[j] for j in argsort]
+                    label = [label[j] for j in argsort]
 
                 return index, values, label, flat_key
 
             else:
 
                 if flat_key not in folds:
-                    return [], [], [], flat_key + 1
+                    return None, None, None, flat_key + 1
 
                 info_in_fold = inf_g.get_group(flat_key)
 
                 in_fold_index = info_in_fold['fold_index']
                 x_type = check_type(xi)
 
                 label = info_in_fold['label'] if 'label' in info_in_fold else None
+                index = info_in_fold.index
 
                 if xi is None:
                     return None, None, None, flat_key + 1
                 elif x_type.minor == 'pandas':
-                    return in_fold_index.index, xi.iloc[in_fold_index.values], label, flat_key + 1
+                    return index, xi.iloc[in_fold_index.values], label, flat_key + 1
                 elif x_type.minor == 'native':
-                    return in_fold_index.index, [xi], label, flat_key + 1
+                    return index, [xi], label, flat_key + 1
                 else:
-                    return in_fold_index.index, xi[in_fold_index.values], label, flat_key + 1
+                    return index, xi[in_fold_index.values], label, flat_key + 1
 
         i, d, l, _ = _recursive_filter(x)
 
+        if all([li is None for li in recursive_flatten(l)]):
+            l = None
+
         return DataBatch(data=d, index=i, label=l)
 
     def slice_index(self, index):
 
         if not self.cached:
             raise LookupError(f"Cannot slice by index as data is not cached")
 
+        orientation = self.orientation
         if self.orientation in ['simple', 'columns', 'simplified_index']:
 
             info = None
             if self.label is not None:
                 if hasattr(self.label, 'loc'):
                     label = self.label.loc[index]
                 else:
@@ -1587,34 +1655,56 @@
                 else:
                     iloc = index
 
                 data = recursive_batch(self.data, iloc)
 
         elif self.orientation in ['index', 'packed']:
 
-            info = self.info.loc[index]
-            db = BeamData.recursive_filter(self.data, info)
+            info = None
+            batch_info = self.info.loc[index]
+            # batch_info['map'] = np.arange(len(batch_info))
+
+            db = self.recursive_filter(self.data, batch_info)
             data = db.data
             index = db.index
             label = db.label
+            if self.orientation == 'index':
+                data = collate_chunks(*recursive_flatten(data), dim=0)
+                index = collate_chunks(*recursive_flatten(index), dim=0)
+                label = collate_chunks(*recursive_flatten(label), dim=0)
+
+                index_map = pd.Series(np.arange(len(index)), index=index)
+                index_map = index_map.loc[batch_info.index].values
+
+                data_type = check_type(data)
+
+                if data_type.minor == 'pandas':
+                    data = data.iloc[index_map]
+                else:
+                    data = data[index_map]
+
+                if label is not None:
+                    label = label.values[index_map]
+
+                index = batch_info.index
+                orientation = 'simplified_index'
 
         else:
             raise ValueError(f"Cannot fetch batch for BeamData with orientation={self.orientation}")
 
         if self.quick_getitem:
             return BeamData.data_batch(data, index=index, label=label, orientation=self.orientation, info=info)
 
-        return self.clone(data=data, columns=self.columns, index=index, label=label,
-                          orientation=self.orientation, info=info)
+        return self.clone(data=data, columns=self.columns, index=index, label=label, orientation=orientation, info=info)
 
     @staticmethod
     def data_batch(data, index=None, label=None, orientation=None, info=None):
 
-        data_type = check_type(data, check_element=False, check_minor=False)
-        if data_type.major == 'container' and len(data) == 1:
+        ic = is_container(data)
+        if ic and len(data) == 1:
             if isinstance(data, dict):
                 key = list(data.keys())[0]
             else:
                 key = 0
 
             data = data[key]
             if index is not None:
@@ -1622,15 +1712,15 @@
                 if isinstance(label, pd.Series):
                     label = label.values
             if label is not None:
                 label = label[key]
                 if isinstance(label, pd.Series):
                     label = label.values
 
-        elif data_type.major == 'container':
+        elif ic:
             data = BeamData._concatenate(data=data, orientation=orientation)
 
             if index is not None:
                 index = BeamData._concatenate(data=index, orientation=orientation)
 
                 if info is not None:
                     flat_index = pd.Series(np.arange(len(info)), index=index)
@@ -1709,15 +1799,15 @@
         @recursive
         def reduce_hierarchy(x):
             if isinstance(x, list):
                 return ['/'.join(xi.split('/')[1:]) for xi in x]
             return '/'.join(x.split('/')[1:])
 
         while True:
-            flat_paths = recursive_flatten(all_paths)
+            flat_paths = recursive_flatten(all_paths, flat_array=True)
             if len(flat_paths) == 1:
                 return root_path.joinpath(flat_paths[0]), None
 
             h = flat_paths[0].split('/')[0]
             if all([h == p.split('/')[0] for p in flat_paths]):
                 root_path = root_path.joinpath(h)
                 all_paths = reduce_hierarchy(all_paths)
@@ -1805,15 +1895,16 @@
         else:
             return default
 
     def clone(self, *args, data=None, path=None, name=None, all_paths=None, key_map=None,
                  index=None, label=None, columns=None, lazy=None, device=None, target_device=None, schema=None,
                  override=None, compress=None, split_by=None, chunksize=None, chunklen=None, n_chunks=None,
                  partition=None, archive_size=None, preferred_orientation=None, read_kwargs=None, write_kwargs=None,
-                 quick_getitem=None, orientation=None, glob_filter=None, info=None, constructor=None, **kwargs):
+                 quick_getitem=None, orientation=None, glob_filter=None, info=None, constructor=None,
+                 write_metadata=None, metadata_path_prefix=None, **kwargs):
 
         name = self.get_default('name', name)
         lazy = self.get_default('lazy', lazy)
         device = self.get_default('device', device)
         target_device = self.get_default('target_device', target_device)
         override = self.get_default('override', override)
         compress = self.get_default('compress', compress)
@@ -1824,38 +1915,47 @@
         partition = self.get_default('partition', partition)
         archive_size = self.get_default('archive_size', archive_size)
         preferred_orientation = self.get_default('preferred_orientation', preferred_orientation)
         read_kwargs = self.get_default('read_kwargs', read_kwargs)
         write_kwargs = self.get_default('write_kwargs', write_kwargs)
         quick_getitem = self.get_default('quick_getitem', quick_getitem)
         glob_filter = self.get_default('glob_filter', glob_filter)
+        write_metadata = self.get_default('write_metadata', write_metadata)
+        metadata_path_prefix = self.get_default('metadata_path_prefix', metadata_path_prefix)
 
         if constructor is None:
             constructor = BeamData
 
         return constructor(*args, data=data, path=path, name=name, all_paths=all_paths, key_map=key_map,
                  index=index, label=label, columns=columns, lazy=lazy, device=device, target_device=target_device,
                  override=override, compress=compress, split_by=split_by, chunksize=chunksize,
                  chunklen=chunklen, n_chunks=n_chunks, partition=partition, archive_size=archive_size, schema=schema,
                  preferred_orientation=preferred_orientation, read_kwargs=read_kwargs, write_kwargs=write_kwargs,
-                 quick_getitem=quick_getitem, orientation=orientation, glob_filter=glob_filter, info=info, **kwargs)
+                 quick_getitem=quick_getitem, orientation=orientation, glob_filter=glob_filter, info=info,
+                 write_metadata=write_metadata, metadata_path_prefix=metadata_path_prefix, **kwargs)
 
     def inverse_columns_map(self, columns):
 
         columns_map = self.columns_map
         if check_type(columns).major == 'scalar':
             columns = columns_map[columns]
         else:
             columns = [columns_map[i] for i in columns]
 
         return columns
 
     def __repr__(self):
         return self.__str__()
 
+    def update_all_paths_file(self):
+
+        path = self.metadata_paths['all_paths']
+        if self.write_metadata:
+            BeamData.write_file(self.all_paths, path)
+
     def __str__(self):
 
         params = {'orientation': self.orientation, 'lazy': self.lazy, 'stored': self.stored,
                   'cached': self.cached, 'device': self.device, 'objects_type': self.objects_type,
                   'quick_getitem': self.quick_getitem, 'has_index': self.index is not None,
                   'has_label': self.label is not None}
         params_line = ' | '.join([f"{k}: {v}" for k, v in params.items()])
@@ -1911,15 +2011,16 @@
                     all_paths = all_paths[k]
                     path = path.joinpath(BeamData.normalize_key(k))
 
                 key = key[-1]
 
             path = path.joinpath(key)
             path = BeamData.write_object(value, path, **kwargs)
-            all_paths[key] = path
+            all_paths[key] = str(path.relative_to(self.root_path))
+            self.update_all_paths_file()
 
         if self.cached:
 
             key = org_key
             if self.orientation in ['simple', 'simplified_index']:
                 self.data.__setitem__(key, value)
             else:
@@ -1995,15 +2096,15 @@
                         info = None
                         if self.info is not None:
                             info = self.info[self.info['fold_index'] == i]
                         yield k, self.clone(d, index=index, label=label, schema=s, info=info)
 
                 else:
 
-                    for i, (k, p) in enumerate(recursive_flatten_with_keys(self.all_paths)):
+                    for i, (k, p) in enumerate(recursive_flatten_with_keys(self.all_paths).items()):
                         s = get_item_with_tuple_key(self.schema, k)
 
                         info = None
                         if self.info is not None:
                             info = self.info[self.info['fold_index'] == i]
 
                         yield k, self.clone(path=self.root_path, all_paths={'data': p}, schema=s, info=info)
```

### Comparing `beam-ds-2.0.2/src/beam/data_tensor.py` & `beam-ds-2.0.3/src/beam/data_tensor.py`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.2/src/beam/dataset.py` & `beam-ds-2.0.3/src/beam/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,23 +153,25 @@
     @property
     def device(self):
 
         if self.data_type is None:
             self.data_type = check_type(self.data).minor
 
         if self.data_type == 'dict':
-            return recursive_device(next(iter(self.data.values())))
+            device = recursive_device(next(iter(self.data.values())))
         elif self.data_type == 'list':
-            return recursive_device(self.data[0])
+            device = recursive_device(self.data[0])
         elif self.data_type == 'simple':
-            return self.data.device
+            device = self.data.device
         elif hasattr(self.data, 'device'):
-            return self.data.device
+            device = self.data.device
         else:
-            return self.__device__()
+            device = self.__device__()
+
+        return beam_device(device)
 
     def __repr__(self):
         return repr(self.data)
 
     @property
     def values(self):
         return self.data
```

### Comparing `beam-ds-2.0.2/src/beam/experiment.py` & `beam-ds-2.0.3/src/beam/experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,37 +10,42 @@
 # from torch.utils.tensorboard import SummaryWriter
 # from tensorboardX import SummaryWriter
 from shutil import copytree
 import torch
 import copy
 import shutil
 from collections import defaultdict
-from .utils import include_patterns, logger, check_type, beam_device, check_element_type, print_beam_hyperparameters
+from .utils import include_patterns, check_type, beam_device, check_element_type, print_beam_hyperparameters
 import pandas as pd
 import torch.multiprocessing as mp
 from .utils import setup_distributed, cleanup, set_seed, find_free_port, check_if_port_is_available, is_notebook, find_port, \
     pretty_format_number, as_numpy
 import torch.distributed as dist
 from functools import partial
 from argparse import Namespace
 from tensorboard.notebook import start as start_tensorboard
 from ._version import __version__
 import inspect
 from .path import beam_path, BeamPath
+from .logger import beam_logger as logger
 
-done = mp.Event()
 
+done = mp.Event()
 
 def gen_hparams_string(experiment_path):
     experiment_path = beam_path(experiment_path)
     tensorboard_hparams = experiment_path.joinpath("hparams.pkl").read()
     return '/'.join([f"{k}_{v}" for k, v in tensorboard_hparams.items()])
 
 
 def path_depth(path):
+
+    if isinstance(path, str):
+        path = BeamPath(path)
+
     return len(str(path.resolve()).split(os.sep))
 
 
 def beam_algorithm_generator(experiment, Alg, Dataset=None, alg_args=None, alg_kwargs=None,
                              dataset_args=None, dataset_kwargs=None):
 
     if alg_args is None:
@@ -279,34 +284,33 @@
             # copy code to dir
 
             if is_notebook():
                 code_root_path = os.getcwd()
             else:
                 code_root_path = sys.argv[0]
 
+            self.source_dir = os.path.dirname(os.path.realpath(code_root_path))
             #TODO: handle the case where root_path is not BeamPath object
             if isinstance(self.code_dir, BeamPath):
-                copytree(os.path.dirname(os.path.realpath(code_root_path)), str(self.code_dir),
+                copytree(self.source_dir, str(self.code_dir),
                          ignore=include_patterns('*.py', '*.md', '*.ipynb'))
             else:
                 logger.warning("Code directory is not BeamPath object. Skipping code copy.")
 
             self.root.joinpath('args.pkl').write(self.vars_args)
 
         self.writer = None
 
         self.rank = 0
         self.world_size = args.parallel
 
         if self.world_size > 1:
             torch.multiprocessing.set_sharing_strategy('file_system')
 
-        log_file = str(self.root.joinpath('experiment.log'))
-        logger.add(log_file, level='INFO', colorize=True,
-                   format='<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <8}</level> | <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>')
+        logger.add_file_handlers(self.root.joinpath('experiment.log'))
 
         print_beam_hyperparameters(args, debug_only=not print_hyperparameters)
 
         # replace zero split_dataset_seed to none (non-deterministic split) - if zero
         if self.hparams.split_dataset_seed == 0:
             self.hparams.split_dataset_seed = None
 
@@ -339,14 +343,43 @@
             if self.hparams.device_list is not None:
                 self.hparams.device_list = [beam_device(di) for di in self.hparams.device_list]
             else:
                 self.hparams.device_list = [beam_device(di+self.hparams.device.index) for di in range(self.hparams.parallel)]
 
         self.root.joinpath('hparams.pkl').write(self.tensorboard_hparams)
 
+        self.comet_exp = None
+        if self.hparams.comet:
+
+            from comet_ml import Experiment
+            # from comet_ml.integration.pytorch import log_model
+
+            api_key = self.hparams.comet_api_key
+            if api_key is None:
+                api_key = os.environ.get('COMET_API_KEY', None)
+            git_directory = self.hparams.git_directory
+            if git_directory is None and isinstance(self.code_dir, BeamPath):
+                git_directory = str(self.code_dir)
+            if git_directory is not None:
+                os.environ['COMET_GIT_DIRECTORY'] = git_directory
+                log_code = True
+            else:
+                log_code = False
+
+            logger.info("Logging this experiment to comet.ml")
+
+            self.comet_exp = Experiment(api_key=api_key, project_name=self.hparams.project_name,
+                                        log_code=log_code, workspace=self.hparams.comet_workspace,
+                                        disabled=not self.hparams.comet)
+
+            self.comet_exp.add_tag(self.hparams.identifier)
+            self.comet_exp.set_name(self.exp_name)
+            self.comet_exp.log_parameters(self.tensorboard_hparams)
+
+
     @staticmethod
     def reload_from_path(path, override_hparams=None, **argv):
 
         path = beam_path(path)
         logger.info(f"Reload experiment from path: {path}")
 
         args = path.joinpath('args.pkl').read()
@@ -420,17 +453,20 @@
             from tensorboardX import SummaryWriter
             if isinstance(self.tensorboard_dir, BeamPath):
                 self.writer = SummaryWriter(log_dir=str(self.tensorboard_dir.joinpath('logs')),
                                             comment=self.hparams.identifier)
             else:
                 logger.warning(f"Tensorboard directory is not a BeamPath object. Tensorboard will not be enabled.")
 
-        if networks is not None and enable and self.writer is not None:
-            for k, net in networks.items():
-                self.writer.add_graph(net, inputs[k])
+        if networks is not None and enable:
+            if self.writer is not None:
+                for k, net in networks.items():
+                    self.writer.add_graph(net, inputs[k])
+            if self.comet_exp is not None:
+                self.comet_exp.set_model_graph(str(networks))
 
     def save_model_results(self, results, algorithm, iteration, visualize_results='yes',
                            store_results='logscale', store_networks='logscale', print_results=True,
                            visualize_weights=False, argv=None):
 
         '''
 
@@ -467,15 +503,15 @@
             logscale = not (epoch - 1) % (10 ** (decade - 1))
 
             for subset, res in results.items():
 
                 if store_results == 'yes' or store_results == 'logscale' and logscale:
 
                     self.results_dir.joinpath(subset).mkdir(parents=True, exist_ok=True)
-                    self.results_dir.joinpath(subset, f'results_{epoch:06d}').write(res, ext='.pt')
+                    self.results_dir.joinpath(subset, f'results_{epoch:06d}.pt').write(res)
 
                 alg = algorithm if visualize_weights else None
 
             if visualize_results == 'yes' or visualize_results == 'logscale' and logscale:
                 self.log_data(results, epoch, print_log=print_results, alg=alg, argv=argv)
 
             checkpoint_file = self.checkpoints_dir.joinpath(f'checkpoint_{epoch:06d}')
@@ -717,14 +753,16 @@
         elif add_all_of_same_identifier:
             base_dir = os.path.join(self.hparams.root_dir, self.hparams.project_name, self.hparams.algorithm, self.hparams.identifier)
             depth = 1
         else:
             base_dir = self.root
             depth = 0
 
+        #TODO: add support for beampath
+        base_dir = str(base_dir)
         experiments = [d[0] for d in list(os.walk(base_dir)) if (path_depth(d[0]) - path_depth(base_dir)) == depth]
 
         if more_experiments is not None:
             if hparams:
                 logger.error("hparams visualization does not support adding additional experiments")
             if type(more_experiments) is str:
                 more_experiments = [more_experiments]
```

### Comparing `beam-ds-2.0.2/src/beam/model.py` & `beam-ds-2.0.3/src/beam/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import copy
 
 import torch
 from torch import nn
 from collections import defaultdict
 import numpy as np
 import math
-from .utils import slice_to_index, logger, hash_tensor
+from .utils import slice_to_index, hash_tensor
+from .logger import beam_logger as logger
 from .optim import BeamOptimizer
 from functools import partial
 import random
 
 
 class PackedSet(object):
```

### Comparing `beam-ds-2.0.2/src/beam/optim.py` & `beam-ds-2.0.3/src/beam/optim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import torch
 from torch import nn
 from collections import defaultdict
 import math
 from functools import partial
-from .utils import logger
+from .logger import beam_logger as logger
+
 
 class MultipleScheduler(object):
 
     def __init__(self, multiple_optimizer, scheduler, *argc, **argv):
 
         self.schedulers = {}
         self.multiple_optimizer = multiple_optimizer
```

### Comparing `beam-ds-2.0.2/src/beam/packed_folds.py` & `beam-ds-2.0.3/src/beam/packed_folds.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import torch
 from .utils import check_type, slice_to_index, as_tensor, beam_device
 import pandas as pd
-from .data_tensor import DataTensor
+from .tensor import DataTensor
 
 
 class PackedFolds(object):
 
     def __init__(self, data, index=None, names=None, fold=None, fold_index=None, device=None,
                  sort_index=False, quick_getitem=True):
```

### Comparing `beam-ds-2.0.2/src/beam/parallel.py` & `beam-ds-2.0.3/src/beam/parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .utils import tqdm_beam
 from tqdm import tqdm
 from .utils import divide_chunks, collate_chunks, retrieve_name
 import inspect
-from .utils import logger, Timer
+from .logger import Timer
+from .logger import beam_logger as logger
 
 
 def parallel(tasks, n_workers=0, func=None, method='joblib', progressbar='beam', reduce=False, reduce_dim=0, **kwargs):
     bp = BeamParallel(func=func, n_workers=n_workers, method=method, progressbar=progressbar,
                       reduce=reduce, reduce_dim=reduce_dim, **kwargs)
     return bp(tasks)
 
@@ -96,14 +97,17 @@
 
     @property
     def name(self):
         if self._name is None:
             self._name = retrieve_name(self)
         return self._name
 
+    def __len__(self):
+        return len(self.queue)
+
     def add(self, *args, **kwargs):
 
         args_list = []
         args_dict = {}
         for a in args:
             if isinstance(args[0], BeamTask):
                 if a.name is None:
@@ -332,14 +336,18 @@
 
         if n_workers is None:
             n_workers = self.n_workers
         n_workers = min(n_workers, len(self.queue))
         if method is None:
             method = self.method
 
+        if len(self.queue) == 0:
+            logger.info(f"Queue {self.name} is empty, returning empty list.")
+            return []
+
         logger.info(f"Start running queue: {self.name}: {len(self.queue)} tasks with {n_workers} workers,"
                     f" method: {method}")
 
         if n_workers <= 1 or len(self.queue) == 1:
             results = [t.run() for t in self.progressbar(self.queue)]
         elif method == 'joblib':
             results = self._run_joblib(n_workers=n_workers)
```

### Comparing `beam-ds-2.0.2/src/beam/path.py` & `beam-ds-2.0.3/src/beam/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,17 @@
     @classmethod
     def home(cls):
         return cls(str(Path.home()))
 
     def stat(self):  # add follow_symlinks=False for python 3.10
         return self.path.stat()
 
+    def getmtime(self):
+        return os.path.getmtime(str(self.path))
+
     def chmod(self, mode):
         return self.path.chmod(mode)
 
     def exists(self):
         return self.path.exists()
 
     def expanduser(self):
@@ -373,27 +376,34 @@
     def object(self):
         if self._object is None:
             self._object = self.client.Object(self.bucket_name, self.key)
         return self._object
 
     def is_file(self):
 
+        if self.bucket_name is None or self.key is None:
+            return False
+
         key = self.key.rstrip('/')
         return S3Path._exists(self.client, self.bucket_name, key)
 
     @staticmethod
-    def _exists(client, bucket, key):
+    def _exists(client, bucket_name, key):
         try:
-            client.Object(bucket, key).load()
+            # client.Object(bucket_name, key).load()
+            client.meta.client.head_object(Bucket=bucket_name, Key=key)
             return True
         except botocore.exceptions.ClientError:
             return False
 
     def is_dir(self):
 
+        if self.bucket_name is None:
+            return True
+
         if self.key is None:
             return self._check_if_bucket_exists()
 
         key = self.normalize_directory_key()
         return S3Path._exists(self.client, self.bucket_name, key) or \
                (self._check_if_bucket_exists() and (not self._is_empty(key)))
```

### Comparing `beam-ds-2.0.2/src/beam/processor.py` & `beam-ds-2.0.3/src/beam/processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from .utils import divide_chunks, collate_chunks, recursive_chunks, iter_container, logger, \
-    recursive_size_summary, container_len, retrieve_name, build_container_from_tupled_keys
+from .utils import divide_chunks, collate_chunks, recursive_chunks, iter_container, \
+    recursive_size_summary, container_len, retrieve_name, build_container_from_tupled_keys, is_empty
 from .parallel import parallel, BeamParallel, BeamTask
 from collections import OrderedDict
 from .data import BeamData
 from .path import beam_path
 import pickle
 import io
+from .utils import tqdm_beam as tqdm
+from .logger import beam_logger as logger
 
 
 class Processor(object):
 
     def __init__(self, *args, name=None, state=None, path=None, **kwargs):
         self._name = name
         self.state = state
@@ -113,16 +115,16 @@
     def reduce(self, *xs, **kwargs):
         return collate_chunks(*xs, dim=self.dim, **kwargs)
 
 
 class Transformer(Processor):
 
     def __init__(self, *args, n_workers=0, n_chunks=None, name=None, store_path=None, partition=None,
-                 chunksize=None, multiprocess_method='joblib', squeeze=True, reduce_dim=0, transform_strategy=None,
-                 split_by='key', **kwargs):
+                 chunksize=None, multiprocess_method='joblib', squeeze=True, reduce=True, reduce_dim=0,
+                 transform_strategy=None, split_by='keys', **kwargs):
         """
 
         @param args:
         @param n_workers:
         @param n_chunks:
         @param name:
         @param store_path:
@@ -144,15 +146,15 @@
             'SS' - the data stored and given to the transformer as a list of paths, the output of each process is stored
             and is returned to the main process as a list of paths. This approach suits for the case when the input data
             is too large to fit into the memory and the transformation generate a large output that cannot be cached,
             e.g. image transformations.
             'C' - the input type is inferred from the BeamData object and the output is cached.
             'S' - the input type is inferred from the BeamData object and the output is stored.
         @param split_by: The split strategy of the data into chunks.
-        'key' - the data is split by the key,
+        'keys' - the data is split by the key,
         'index' - the data is split by the index (i.e. dim=0).
         'columns' - the data is split by the columns (i.e. dim=1).
         @param kwargs:
         """
         super(Transformer, self).__init__(*args, name=name, **kwargs)
 
         if (n_chunks is None) and (chunksize is None):
@@ -162,31 +164,30 @@
         self.chunksize = chunksize
         self.n_chunks = n_chunks
         self.n_workers = n_workers
         self.squeeze = squeeze
         self.kwargs = kwargs
         self.transform_strategy = transform_strategy
         self.split_by = split_by
-        if self.transform_strategy in ['SC', 'SS'] and self.split_by != 'key':
-            logger.warning(f'transformation strategy {self.transform_strategy} supports only split_by=\"key\", '
-                           f'The split_by is set to "key".')
-            self.split_by = 'key'
+        if self.transform_strategy in ['SC', 'SS'] and self.split_by != 'keys':
+            logger.warning(f'transformation strategy {self.transform_strategy} supports only split_by=\"keys\", '
+                           f'The split_by is set to "keys".')
+            self.split_by = 'keys'
 
         if store_path is not None:
             store_path = beam_path(store_path)
         if store_path is not None and name is not None:
             store_path = store_path.joinpath(name)
 
         self.store_path = store_path
         self.partition = partition
         self.multiprocess_method = multiprocess_method
         self.reduce_dim = reduce_dim
-
-        self.queue = BeamParallel(n_workers=n_workers, func=None, method=multiprocess_method,
-                                  progressbar='beam', reduce=False, reduce_dim=reduce_dim, **kwargs)
+        self.to_reduce = reduce
+        self._exceptions = None
 
     def chunks(self, x, chunksize=None, n_chunks=None, squeeze=None, split_by=None, partition=None):
 
         if split_by is None:
             split_by = self.split_by
 
         if partition is None:
@@ -227,29 +228,43 @@
             x = BeamData.from_path(path=store_path)
 
         return key, x
 
     def fit(self, x, **kwargs):
         return x
 
+    @property
+    def exceptions(self):
+        return self._exceptions
+
+    @exceptions.setter
+    def exceptions(self, exceptions):
+        self._exceptions = exceptions
+
     def fit_transform(self, x, **kwargs):
         return self.transform(x, fit=True, **kwargs)
         # self.fit(x, **kwargs)
         # return self.transform(x, **kwargs)
 
-    def reduce(self, x, reduce_dim=None, **kwargs):
+    def reduce(self, x, reduce_dim=None, split_by=None , **kwargs):
+
+        if isinstance(next(iter_container(x))[1], BeamData):
+            x = BeamData.collate(x, split_by=split_by, **kwargs)
+        else:
 
-        if reduce_dim is None:
-            reduce_dim = self.reduce_dim
+            if reduce_dim is None:
+                reduce_dim = self.reduce_dim
 
-        return collate_chunks(*x, dim=reduce_dim, **kwargs)
+            x = collate_chunks(*x, dim=reduce_dim, **kwargs)
+
+        return x
 
     def transform(self, x, chunksize=None, n_chunks=None, n_workers=None, squeeze=None, multiprocess_method=None,
                   fit=False, path=None, split_by=None, partition=None, transform_strategy=None, cache=True, store=False,
-                  **kwargs):
+                  reduce=True, **kwargs):
         """
 
         @param x:
         @param chunksize:
         @param n_chunks:
         @param n_workers:
         @param squeeze:
@@ -266,38 +281,48 @@
         """
         if split_by is None:
             split_by = self.split_by
 
         if partition is None:
             partition = self.partition
 
+        if multiprocess_method is None:
+            multiprocess_method = self.multiprocess_method
+
+        if n_workers is None:
+            n_workers = self.n_workers
+
         if transform_strategy is None:
             transform_strategy = self.transform_strategy
 
-        if transform_strategy in ['SC', 'SS'] and split_by != 'key':
+        if reduce is None:
+            reduce = self.to_reduce
+
+        reduce_dim = self.reduce_dim
+
+        if transform_strategy in ['SC', 'SS'] and split_by != 'keys':
             logger.warning(f'transformation strategy {transform_strategy} supports only split_by=\"key\", '
                            f'The split_by is set to "key".')
-            split_by = 'key'
+            split_by = 'keys'
 
         if path is None:
             path = self.store_path
 
         logger.info(f"Starting transformer process: {self.name}")
 
-        if len(x) == 0:
+        if is_empty(x):
             return x
 
         if (chunksize is None) and (n_chunks is None):
             chunksize = self.chunksize
             n_chunks = self.n_chunks
         if squeeze is None:
             squeeze = self.squeeze
 
-        is_chunk = (n_chunks != 1) or (not squeeze)
-        self.queue.set_name(self.name)
+        is_chunk = (n_chunks != 1) or (not squeeze) or (split_by == 'keys' and isinstance(x, BeamData) and x.stored)
 
         if ((transform_strategy is None) or (transform_strategy == 'C')) and type(x) == BeamData:
             if x.cached:
                 transform_strategy = 'CC'
             elif x.stored:
                 transform_strategy = 'SC'
             else:
@@ -334,55 +359,80 @@
             else:
                 logger.warning(f"Path is not specified for transformer: {self.name}, "
                                f"the chunk will not be stored.")
                 store_chunk = False
         elif store_chunk:
             logger.info(f"Storing transformed chunks of data in: {path}")
 
+        queue = BeamParallel(n_workers=n_workers, func=None, method=multiprocess_method, name=self.name,
+                                  progressbar='beam', reduce=False, reduce_dim=reduce_dim, **kwargs)
+
         if is_chunk:
-            for k, c in self.chunks(x, chunksize=chunksize, n_chunks=n_chunks,
-                                    squeeze=squeeze, split_by=split_by, partition=partition):
+            logger.info(f"Splitting data to chunks for transformer: {self.name}")
+            for k, c in tqdm(self.chunks(x, chunksize=chunksize, n_chunks=n_chunks,
+                                    squeeze=squeeze, split_by=split_by, partition=partition)):
 
                 chunk_path = None
                 if store_chunk:
 
                     if split_by == 'index':
                         part_name = BeamData.index_partition_directory_name
                     elif split_by == 'columns':
                         part_name = BeamData.columns_partition_directory_name
                     else:
                         part_name = ''
 
                     chunk_path = path.joinpath(f"{BeamData.normalize_key(k)}{part_name}")
-                    chunk_path = chunk_path.as_uri()
+                    # chunk_path = chunk_path.as_uri()
 
-                self.queue.add(BeamTask(self.worker, c, key=k, is_chunk=is_chunk, fit=fit, store_path=chunk_path,
+                queue.add(BeamTask(self.worker, c, key=k, is_chunk=is_chunk, fit=fit, store_path=chunk_path,
                                         cache=cache, store=store_chunk, name=f"{self.name}/{k}", **kwargs))
 
         else:
-            self.queue.add(BeamTask(self.worker, x, key=None, is_chunk=is_chunk, fit=fit, cache=cache,
+            queue.add(BeamTask(self.worker, x, key=None, is_chunk=is_chunk, fit=fit, cache=cache,
                                     store=store_chunk,  name=f"{self.name}", **kwargs))
 
-        x_with_keys = self.queue.run(n_workers=n_workers, method=multiprocess_method)
+        logger.info(f"Starting transformer: {self.name} with {n_workers} workers. "
+                    f"Number of queued tasks is {len(queue)}.")
+
+        x_with_keys = queue.run(n_workers=n_workers, method=multiprocess_method)
+
+        exceptions = [{'exception': xi, 'task': queue.queue[i]} for i, xi in enumerate(x_with_keys)
+                      if isinstance(xi, Exception)]
+
+        if len(exceptions) > 0:
+            logger.error(f"Transformer {self.name} had {len(exceptions)} exceptions during operation.")
+            logger.info("Failed tasks can be obtained in self.exceptions")
+            self.exceptions = exceptions
+
+        x_with_keys = [xi for xi in x_with_keys if not isinstance(xi, Exception)]
 
         if is_chunk:
             values = [xi[1] for xi in x_with_keys]
             keys = [xi[0] for xi in x_with_keys]
             keys = [ki if type(ki) is tuple else (ki, ) for ki in keys]
 
-            x = build_container_from_tupled_keys(keys, values)
+            if len(exceptions) == 0:
+                x = build_container_from_tupled_keys(keys, values)
 
-            logger.info(f"Finished transformer process: {self.name}. Collating results...")
+                logger.info(f"Finished transformer process: {self.name}. Collating results...")
 
-            if isinstance(x[0], BeamData):
-                x = BeamData.collate(x, split_by=split_by, **kwargs)
+                if reduce:
+                    x = self.reduce(x, split_by=split_by, **kwargs)
             else:
-                x = self.reduce(x, **kwargs)
+                x = {k: v for k, v in zip(keys, values)}
+                if store:
+                    logger.warning("Due to exceptions, the data will not be stored, "
+                                   "the data is returned as a dictionary of all the successful tasks.")
+                return x
 
         else:
+            if len(exceptions) > 0:
+                logger.warning("Exception occurred, the exception object and the task are returned.")
+                return x_with_keys
             logger.info(f"Finished transformer process: {self.name}.")
             x = x_with_keys[0][1]
 
         if store:
 
             logger.info(f"Storing transformed of data in: {path}")
             if not isinstance(x, BeamData):
```

### Comparing `beam-ds-2.0.2/src/beam/server.py` & `beam-ds-2.0.3/src/beam/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from flask import Flask, jsonify, request, send_file
 from .experiment import Experiment
 import requests
 import io
 import torch
-from .utils import logger, find_port
+from .utils import find_port
 from gevent.pywsgi import WSGIServer
+from .logger import beam_logger as logger
 
 
 class BeamClient(object):
 
     def __init__(self, host):
         self.host = host
```

### Comparing `beam-ds-2.0.2/src/beam/ssl.py` & `beam-ds-2.0.3/src/beam/ssl.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import torch.nn.functional as F
 from torch import nn
 import numpy as np
 import math
 
 from .model import soft_target_update, reset_network, copy_network, BeamEnsemble
 from .model import beam_weights_initializer, freeze_network_params, free_network_params
-from .utils import as_numpy, pretty_format_number, logger, beam_logger
+from .utils import as_numpy, pretty_format_number
+from .logger import beam_logger as logger
 from .algorithm import Algorithm
 from .optim import BeamOptimizer
 from .config import boolean_feature, get_beam_parser
 
 import lightgbm as lgb
 from torch.nn.utils import spectral_norm
 import faiss
@@ -203,15 +204,15 @@
         if networks is None:
             networks = {}
 
         encoder = self.generate_encoder()
         if encoder is not None:
             networks['encoder'] = encoder
 
-        self.logger = beam_logger()
+        self.logger = logger
 
         super().__init__(hparams, networks=networks, optimizers=optimizers, schedulers=schedulers)
 
         if labeled_dataset is None:
             labeled_dataset = self.generate_labeled_set()
         self.labeled_dataset = labeled_dataset
```

### Comparing `beam-ds-2.0.2/src/beam/study.py` & `beam-ds-2.0.3/src/beam/study.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import time
 import os
 import copy
 
-from .utils import logger, find_port, print_beam_hyperparameters, check_type, is_notebook
-from .path import beam_path
+from .utils import find_port, print_beam_hyperparameters, check_type, is_notebook
+from .logger import beam_logger as logger
+from .path import beam_path, BeamPath
 import pandas as pd
 import ray
 from ray.tune import JupyterNotebookReporter
 from ray import tune
 import optuna
 from functools import partial
 from .experiment import Experiment, beam_algorithm_generator
@@ -93,14 +94,18 @@
         if print_hyperparameters:
             print_beam_hyperparameters(hparams)
 
         root_path = beam_path(self.hparams.root_dir)
         self.ray_logs = root_path.joinpath('ray_results', self.hparams.project_name, self.hparams.algorithm,
                                            self.hparams.identifier)
 
+        if not isinstance(self.ray_logs, BeamPath):
+            ValueError("Currently ray.tune does not support not-local-fs path, please provide local root_dir path")
+        self.ray_logs = str(self.ray_logs)
+
         self.experiments_tracker = []
         self.track_results = track_results
         self.track_algorithms = track_algorithms
         self.track_hparams = track_hparams
         self.track_suggestion = track_suggestion
 
     def tracker(self, algorithm=None, results=None, hparams=None, suggestion=None):
```

### Comparing `beam-ds-2.0.2/src/beam/utils.py` & `beam-ds-2.0.3/src/beam/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 import torch.distributed as dist
 from fnmatch import filter
 from tqdm.notebook import tqdm as tqdm_notebook
 from tqdm import tqdm
 import random
 import torch
 import pandas as pd
+import json
 import pyarrow.feather as feather
+import __main__
 
 try:
     import modin.pandas as mpd
     has_modin = True
 except ImportError:
     mpd = None
     has_modin = False
 
 import socket
 from contextlib import closing
 from collections import namedtuple
 from timeit import default_timer as timer
-from loguru import logger
 from torchvision import transforms
 import hashlib
 from functools import partial
 import itertools
 import scipy
 from pathlib import Path
 import re
@@ -43,14 +44,26 @@
                  fragment=None, params=None, **query):
 
         self._url = url
         self._parsed_url = None
         if url is None:
             netloc = BeamURL.to_netloc(hostname=hostname, port=port, username=username, password=password)
             query = BeamURL.dict_to_query(**query)
+            if scheme is None:
+                scheme = 'file'
+            if path is None:
+                path = ''
+            if netloc is None:
+                netloc = ''
+            if query is None:
+                query = ''
+            if fragment is None:
+                fragment = ''
+            if params is None:
+                params = ''
             self._parsed_url = ParseResult(scheme=scheme, netloc=netloc, path=path, params=params, query=query,
                                            fragment=fragment)
 
         assert self._url is not None or self._parsed_url is not None, 'Either url or parsed_url must be provided'
 
     @property
     def parsed_url(self):
@@ -157,20 +170,14 @@
 
     @classmethod
     def from_string(cls, url):
         parsed_url = urlparse(url)
         return cls(url, parsed_url)
 
 
-# logger.remove(handler_id=0)
-logger.remove()
-logger.add(sys.stdout, level='INFO', colorize=True, format=
-           '<green>{time:YYYY-MM-DD HH:mm:ss}</green> | BeamLog | <level>{level}</level> | <level>{message}</level>')
-
-
 def retrieve_name(var):
     for fi in reversed(inspect.stack()):
         names = [var_name for var_name, var_val in fi.frame.f_locals.items() if var_val is var]
         if len(names) > 0:
             return names[0]
 
 
@@ -200,14 +207,24 @@
         self.url = BeamURL(scheme=scheme, hostname=hostname, port=port, username=username, fragment=fragment,
                            params=params, password=password, path=str(self.path), **kwargs)
 
         self.mode = "rb"
         self.file_object = None
         self.client = client
 
+    def __getstate__(self):
+        return self.as_uri()
+
+    def __setstate__(self, state):
+
+        url = BeamURL.from_string(state)
+
+        self.__init__(url.path, hostname=url.hostname, port=url.port, username=url.username,
+                      password=url.password, fragment=url.fragment, params=url.params, client=None, **url.query)
+
     def __iter__(self):
         for p in self.iterdir():
             yield p
 
     def __getitem__(self, item):
         if item in self.url.query:
             return self.url.query[item]
@@ -243,36 +260,52 @@
                 for p in self.parent.iterdir():
                     if p.stem == self.name:
                         rmtree(p)
 
         self.mkdir(parents=True)
         self.rmdir()
 
+    def getmtime(self):
+        return None
+
+    def stat(self):
+        raise NotImplementedError
+
     def rmdir(self):
         raise NotImplementedError
 
     def unlink(self, **kwargs):
         raise NotImplementedError
 
     def __truediv__(self, other):
         return self.joinpath(str(other))
 
+    def __fspath__(self, mode="rb"):
+        raise TypeError("For BeamPath (named bp), use bp.open(mode) instead of open(bp, mode)")
+
     def __call__(self, mode="rb"):
         self.mode = mode
         return self
 
     def open(self, mode="rb"):
         self.mode = mode
         return self
 
+    def close(self):
+        if self.file_object is not None:
+            self.file_object.close()
+            self.file_object = None
+
     def __str__(self):
         return str(self.path)
 
     def __repr__(self):
-        return str(self.url)
+        if self.is_absolute():
+            return str(self.url)
+        return str(self.path)
 
     def __enter__(self):
         raise NotImplementedError
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         raise NotImplementedError
 
@@ -319,17 +352,20 @@
     def drive(self):
         return self.path.drive
 
     @property
     def root(self):
         return self.path.root
 
+    def is_root(self):
+        return str(self.path) == '/'
+
     @property
     def anchor(self):
-        return self.path.anchor
+        return self.gen(self.path.anchor)
 
     @property
     def parents(self):
         return tuple([self.gen(p) for p in self.path.parents])
 
     @property
     def parent(self):
@@ -357,28 +393,35 @@
     def as_uri(self):
         return self.url.url
 
     def is_absolute(self):
         return self.path.is_absolute()
 
     def is_relative_to(self, *other):
-        return self.path.is_relative_to(*other)
+        if len(other) == 1 and isinstance(other[0], PureBeamPath):
+            other = str(other[0])
+        else:
+            other = str(PureBeamPath(*other))
+        return self.path.is_relative_to(other)
 
     def is_reserved(self):
         return self.path.is_reserved()
 
     def joinpath(self, *other):
         return self.gen(self.path.joinpath(*[str(o) for o in other]))
 
     def match(self, pattern):
         return self.path.match(pattern)
 
     def relative_to(self, *other):
-        other = PureBeamPath(*other)
-        return PureBeamPath(self.path.relative_to(str(other)))
+        if len(other) == 1 and isinstance(other[0], PureBeamPath):
+            other = str(other[0])
+        else:
+            other = str(PureBeamPath(*other))
+        return PureBeamPath(self.path.relative_to(other))
 
     def with_name(self, name):
         return self.gen(self.path.with_name(name))
 
     def with_stem(self, stem):
         return self.gen(self.path.with_stem(stem))
 
@@ -405,14 +448,17 @@
 
     def glob(self, *args, **kwargs):
         raise NotImplementedError
 
     def rename(self, target):
         return NotImplementedError
 
+    def replace(self, target):
+        return NotImplementedError
+
     def read(self, ext=None, **kwargs):
 
         if ext is None:
             ext = self.suffix
 
         with self(mode=PureBeamPath.mode('read', ext)) as fo:
 
@@ -451,23 +497,24 @@
                 x = pd.read_excel(fo, **kwargs)
             elif ext == '.avro':
                 x = []
                 with open(fo, 'rb') as fo:
                     import fastavro
                     for record in fastavro.reader(fo):
                         x.append(record)
-            elif ext == '.json':
+            elif ext in ['.json', '.ndjson']:
 
                 #TODO: add json read with fastavro and shcema
                 # x = []
                 # with open(path, 'r') as fo:
                 #     for record in fastavro.json_reader(fo):
                 #         x.append(record)
 
-                x = pd.read_json(fo, **kwargs)
+                nd = ext == '.ndjson'
+                x = pd.read_json(fo, lines=nd,  **kwargs)
 
             elif ext == '.orc':
                 import pyarrow as pa
                 x = pa.orc.read(fo, **kwargs)
 
             else:
                 raise ValueError("Unknown extension type.")
@@ -477,15 +524,15 @@
     @staticmethod
     def mode(op, ext):
         if op == 'write':
             m = 'w'
         else:
             m = 'r'
 
-        if ext not in ['.avro', '.json', '.orc', '.txt', '.text']:
+        if ext not in ['.avro', '.json', '.orc', '.txt', '.text', '.ndjson']:
             m = f"{m}b"
 
         return m
 
     def write(self, x, ext=None, **kwargs):
 
         if ext is None:
@@ -499,28 +546,40 @@
 
                 if len(x.shape) == 1:
                     x = pd.Series(x)
                     if x.name is None:
                         x.name = 'val'
 
                 x = pd.DataFrame(x)
+
+                if isinstance(x.index, pd.MultiIndex):
+                    raise TypeError("MultiIndex not supported with feather extension.")
+
                 x = x.rename({c: str(c) for c in x.columns}, axis=1)
 
                 index_name = x.index.name if x.index.name is not None else 'index'
                 df = x.reset_index()
                 new_name = PureBeamPath.feather_index_mark + index_name
                 x = df.rename(columns={index_name: new_name})
                 x.to_feather(fo, **kwargs)
             elif ext == '.csv':
                 x = pd.DataFrame(x)
                 x.to_csv(fo, **kwargs)
             elif ext in ['.pkl', '.pickle']:
                 pd.to_pickle(x, fo, **kwargs)
             elif ext == '.npy':
                 np.save(fo, x, **kwargs)
+            elif ext == '.json':
+                json.dump(x, fo, **kwargs)
+            elif ext == '.ndjson':
+                for xi in x:
+                    json.dump(xi, fo, **kwargs)
+                    fo.write("\n")
+            elif ext == '.txt':
+                fo.write(str(x))
             elif ext == '.npz':
                 np.savez(fo, x, **kwargs)
             elif ext == '.scipy_npz':
                 scipy.sparse.save_npz(fo, x, **kwargs)
                 self.rename(f'{path}.npz', path)
             elif ext == '.parquet':
                 x = pd.DataFrame(x)
@@ -532,44 +591,14 @@
 
         return self
 
     def resolve(self, strict=False):
         return self
 
 
-class Timer(object):
-
-    def __init__(self, silence=False):
-        self.silence = silence
-        self._elapsed = 0
-        self.t0 = time.time()
-
-    def __enter__(self):
-        if not self.silence:
-            logger.info(f"Starting timer")
-        self.t0 = time.time()
-        return self
-
-    @property
-    def elapsed(self):
-        return self._elapsed + time.time() - self.t0
-
-    def pause(self):
-        self._elapsed = self._elapsed + time.time() - self.t0
-        return self._elapsed
-
-    def run(self):
-        self.t0 = time.time()
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        td = time.time() - self.t0
-        if not self.silence:
-            logger.info(f"Time elapsed: {pretty_format_number(td)} Sec")
-
-
 def stack_train_results(results, batch_size=None):
 
     stacked_results = defaultdict(dict)
 
     for k_type in results.keys():
         for k_name, v in results[k_type].items():
             stacked_results[k_type][k_name] = v
@@ -616,20 +645,18 @@
 
 def rate_string_format(n, t):
     if n / t > 1:
         return f"{n / t: .4} [iter/sec]"
     return f"{t / n: .4} [sec/iter]"
 
 
-def beam_logger():
-    return logger
-
-
 def print_beam_hyperparameters(args, debug_only=False):
 
+    from .logger import beam_logger as logger
+
     if debug_only:
         log_func = logger.debug
     else:
         log_func = logger.info
 
     log_func(f"beam project: {args.project_name}")
     log_func('Experiment Hyperparameters')
@@ -649,14 +676,16 @@
 
     log_func('----------------------------------------------------------'
              '---------------------------------------------------------------------')
 
 
 def find_port(port=None, get_port_from_beam_port_range=True, application='tensorboard'):
 
+    from .logger import beam_logger as logger
+
     if application == 'tensorboard':
         first_beam_range = 66
         first_global_range = 26006
     elif application == 'flask':
         first_beam_range = 50
         first_global_range = 25000
     else:
@@ -772,37 +801,60 @@
 
     keys = []
     values = []
     for k, v in recursive_chunks(x, chunksize=chunksize, n_chunks=n_chunks, partition=partition, dim=dim):
         keys.append(k)
         values.append(v)
 
-    if not is_arange(keys):
+    argsort, isarange = is_arange(keys)
+    if not isarange:
         values = dict(zip(keys, values))
     else:
-        values = [values[i] for i in np.argsort(keys)]
+        values = [values[i] for i in argsort]
 
     return values
 
 
 def is_arange(x):
 
     x_type = check_type(x)
 
     if x_type.element in ['array', 'object', 'empty', 'none', 'unknown']:
         return False
 
-    arr_x = np.array(x)
+    if x_type.element == 'str':
+        pattern = re.compile(r'^(?P<prefix>.*?)(?P<number>\d+)(?P<suffix>.*)$')
+        df = []
+        for xi in x:
+            match = pattern.match(xi)
+            if match:
+                df.append(match.groupdict())
+            else:
+                return None, False
+        df = pd.DataFrame(df)
+        if not df['prefix'].nunique() == 1 or not df['suffix'].nunique() == 1:
+            return None, False
+
+        arr_x = df['number'].astype(int).values
+    else:
+        arr_x = np.array(x)
+
     try:
         arr_x = arr_x.astype(int)
-        arr_x.sort()
+        argsort = np.argsort(arr_x)
+        arr_x = arr_x[argsort]
     except (ValueError, TypeError):
-        return False
+        return None, False
+
+    isa = np.issubdtype(arr_x.dtype, np.number) and (np.abs(np.arange(len(x)) - arr_x).sum() == 0)
 
-    return np.issubdtype(arr_x.dtype, np.number) and (np.abs(np.arange(len(x)) - arr_x).sum() == 0)
+    if not isa:
+        argsort = None
+
+    return argsort, isa
 
 
 def recursive_chunks(x, chunksize=None, n_chunks=None, partition=None, squeeze=False, dim=0):
 
     x_type = check_type(x)
 
     try:
@@ -876,29 +928,54 @@
                 return np.sum([sys.getsizeof(i) for i in x])
             ind = np.random.randint(len(x), size=(1000,))
             return len(x) * np.mean([sys.getsizeof(x[i]) for i in ind])
         else:
             return sys.getsizeof(x)
 
 
+# def recursive(func):
+#
+#     def apply_recursively(x, *args, **kwargs):
+#
+#         x_type = check_type(x)
+#         if x_type.major == 'container':
+#
+#             keys = []
+#             values = []
+#
+#             for k, v in iter_container(x):
+#                 keys.append(k)
+#                 values.append(apply_recursively(v, *args, **kwargs))
+#
+#             if x_type.minor == 'dict':
+#                 values = dict(zip(keys, values))
+#
+#             return values
+#
+#         else:
+#
+#             return func(x, *args, **kwargs)
+#
+#     return apply_recursively
+
+
 def recursive(func):
 
     def apply_recursively(x, *args, **kwargs):
 
-        x_type = check_type(x)
-        if x_type.major == 'container':
+        if is_container(x):
 
             keys = []
             values = []
 
             for k, v in iter_container(x):
                 keys.append(k)
                 values.append(apply_recursively(v, *args, **kwargs))
 
-            if x_type.minor == 'dict':
+            if isinstance(x, dict):
                 values = dict(zip(keys, values))
 
             return values
 
         else:
 
             return func(x, *args, **kwargs)
@@ -918,18 +995,20 @@
             keys.append(k)
             values.append(recursive_keys(v))
 
         if all([v is None for v in values]):
             return keys
 
         if x_type.minor == 'dict':
-            if not is_arange(values):
+
+            argsort, isarange = is_arange(keys)
+            if not isarange:
                 values = dict(zip(keys, values))
             else:
-                values = [values[i] for i in np.argsort(keys)]
+                values = [values[i] for i in argsort]
 
         return values
 
     return None
 
 
 def recursive_size_summary(x, mode='sum'):
@@ -1030,14 +1109,39 @@
 
                 c = []
 
         i = i+1 if i > 0 else i
         yield i, c
 
 
+@recursive
+def empty_elements(x):
+    x_type = check_type(x)
+    if x_type.minor in ['numpy', 'pandas', 'tensor', 'scipy_sparse']:
+        return x.size == 0
+
+    if x_type.minor in ['list', 'tuple', 'set', 'dict']:
+        return len(x) == 0
+
+    if x_type.minor == 'native':
+        return x is None
+
+    if hasattr(x, '__len__'):
+        return x.__len__() == 0
+
+    return False
+
+
+def is_empty(x):
+
+        x = empty_elements(x)
+        x = recursive_flatten(x)
+        return all(x)
+
+
 def recursive_merge(dfs, method='tree', **kwargs):
     if len(dfs) == 1:
         return dfs[0]
     if len(dfs) == 2:
         return pd.merge(dfs[0], dfs[1], **kwargs)
     if method == 'series':
         return recursive_merge([dfs[0], recursive_merge(dfs[1:], method='series', **kwargs)], method='series', **kwargs)
@@ -1091,20 +1195,30 @@
 
     else:
         return collate_chunks(*xs, dim=dim, on=on, how=how, method=method)
 
 
 def collate_chunks(*xs, keys=None, dim=0, on='index', how='outer', method='tree'):
 
-    x = list(xs)
+    if len(xs) == 0:
+        return []
 
-    if not len(x):
-        return x
+    if len(xs) == 1:
+        return xs[0]
+
+    x = list(xs)
 
     x_type = check_type(x[0], check_element=False)
+
+    if x_type.major == 'container' and x_type.minor == 'dict':
+        dictionary = {}
+        for xi in x:
+            dictionary.update(xi)
+        return dictionary
+
     if (x_type.major not in ['array', 'other']) or (dim == 1 and x_type.minor not in ['tensor', 'numpy', 'pandas']):
         return x
 
     if x_type.minor == 'tensor':
         return torch.cat(x, dim=dim)
 
     elif x_type.minor == 'numpy':
@@ -1166,14 +1280,18 @@
     if not unknown and not np.isscalar(x) and (not (torch.is_tensor(x) and (not len(x.shape)))):
         return 'array'
 
     if pd.isna(x):
         return 'none'
 
     if hasattr(x, 'dtype'):
+        # this case happens in custom classes that have a dtype attribute
+        if unknown:
+            return 'other'
+
         t = str(x.dtype).lower()
     else:
         t = str(type(x)).lower()
 
     if 'int' in t:
         return 'int'
     if 'bool' in t:
@@ -1182,17 +1300,14 @@
         if '16' in t:
             return 'float16'
         else:
             return 'float'
     if 'str' in t:
         return 'str'
 
-    if unknown:
-        return 'other'
-
     return 'object'
 
 
 def check_minor_type(x):
 
     if isinstance(x, torch.Tensor):
         return 'tensor'
@@ -1206,32 +1321,80 @@
         return 'scipy_sparse'
     if isinstance(x, dict):
         return 'dict'
     if isinstance(x, list):
         return 'list'
     if isinstance(x, tuple):
         return 'tuple'
+    if isinstance(x, set):
+        return 'set'
     if isinstance(x, Path) or isinstance(x, PureBeamPath):
         return 'path'
     else:
         return 'other'
 
 
 type_tuple = namedtuple('Type', 'major minor element')
 
 
+def elt_of_list(x):
+
+    if len(x) < 100:
+        sampled_indices = range(len(x))
+    else:
+        sampled_indices = np.random.randint(len(x), size=(100,))
+
+    elt0 = None
+    for i in sampled_indices:
+        elt = check_element_type(x[i])
+
+        if elt0 is None:
+            elt0 = elt
+
+        if elt != elt0:
+            return 'object'
+
+    return elt0
+
+
+def is_container(x):
+    if isinstance(x, dict):
+        return True
+    if isinstance(x, list):
+
+        if len(x) < 100:
+            sampled_indices = range(len(x))
+        else:
+            sampled_indices = np.random.randint(len(x), size=(100,))
+
+        elt0 = None
+        for i in sampled_indices:
+            elt = check_element_type(x[i])
+
+            if elt0 is None:
+                elt0 = elt
+
+            if elt != elt0:
+                return True
+
+            if elt in ['array', 'none']:
+                return True
+
+    return False
+
+
 def check_type(x, check_minor=True, check_element=True):
     '''
 
     returns:
 
     <major type>, <minor type>, <elements type>
 
     major type: container, array, scalar, none, other
-    minor type: dict, list, tuple, tensor, numpy, pandas, scipy_sparse, native, none
+    minor type: dict, list, tuple, set, tensor, numpy, pandas, scipy_sparse, native, none
     elements type: array, int, float, str, object, empty, none, unknown
 
     '''
 
     if np.isscalar(x) or (torch.is_tensor(x) and (not len(x.shape))):
         mjt = 'scalar'
         if check_minor:
@@ -1274,15 +1437,15 @@
 
         elt = 'unknown'
 
         if hasattr(x, '__len__'):
             mjt = 'array'
         else:
             mjt = 'other'
-        if isinstance(x, list) or isinstance(x, tuple):
+        if isinstance(x, list) or isinstance(x, tuple) or isinstance(x, set):
             if not len(x):
                 elt = 'empty'
             else:
 
                 if len(x) < 100:
                     elts = [check_element_type(xi) for xi in x]
 
@@ -1291,15 +1454,15 @@
                     elts = [check_element_type(x[i]) for i in ind]
 
                 if len(set(elts)) == 1:
                     elt = elts[0]
                 else:
                     elt = 'object'
 
-            if elt in ['array', 'object']:
+            if elt in ['array', 'object', 'none']:
                 mjt = 'container'
 
         mit = check_minor_type(x) if check_minor else 'na'
 
         if elt:
             if mit in ['numpy', 'tensor', 'pandas', 'scipy_sparse']:
                 if mit == 'pandas':
@@ -1334,29 +1497,33 @@
                    for name in filter(names, pattern))
         ignore = set(name for name in names
                      if name not in keep and not os.path.isdir(os.path.join(path, name)))
         return ignore
 
     return _ignore_patterns
 
-# def is_notebook():
-#     return '_' in os.environ and 'jupyter' in os.environ['_']
 
+def running_platform() -> str:
 
-def is_notebook() -> bool:
     try:
         shell = get_ipython().__class__.__name__
         if shell == 'ZMQInteractiveShell':
-            return True   # Jupyter notebook or qtconsole
+            return 'notebook' # Jupyter notebook or qtconsole
         elif shell == 'TerminalInteractiveShell':
-            return False  # Terminal running IPython
+            return 'ipython'  # Terminal running IPython
         else:
-            return False  # Other type (?)
+            return 'other'  # Other type (?)
     except NameError:
-        return False      # Probably standard Python interpreter
+        if hasattr(__main__, '__file__'):
+            return 'script'
+        else:
+            return 'console'
+
+def is_notebook() -> bool:
+    return running_platform() == 'notebook'
 
 
 def setup_distributed(rank, world_size, port='7463', backend='gloo'):
     os.environ['MASTER_ADDR'] = 'localhost'
     os.environ['MASTER_PORT'] = port
 
     # initialize the process group
@@ -1415,15 +1582,15 @@
         return data
 
 
 def recursive_func(x, func, *args, **kwargs):
 
     if isinstance(x, dict):
         return {k: recursive_func(v, func, *args, **kwargs) for k, v in x.items()}
-    elif isinstance(x, list) or isinstance(x, tuple):
+    elif isinstance(x, list):
         return [recursive_func(s, func, *args, **kwargs) for s in x]
     elif x is None:
         return None
     else:
         return func(x, *args, **kwargs)
 
 
@@ -1484,16 +1651,21 @@
         return d
     else:
         return {tuple(): x}
 
 
 def get_item_with_tuple_key(x, key):
 
+    if x is None:
+        return None
+
     if isinstance(key, tuple):
         for k in key:
+            if x is None:
+                return None
             x = x[k]
         return x
     else:
         return x[key]
 
 
 def get_closest_item_with_tuple_key(x, key):
@@ -1529,32 +1701,37 @@
         x = []
     else:
         x = {}
 
     return x
 
 
-def insert_tupled_key(x, k, v):
-    if x is None:
+def insert_tupled_key(x, k, v, default=None):
+
+    if x is None and default is None:
         x = new_container(k[0])
+    elif x is None:
+        x = default
 
     xi = x
 
     for ki, kip1 in zip(k[:-1], k[1:]):
 
-        if type(ki) is int and len(xi) == ki:
+        if isinstance(xi, list):
+            assert type(ki) is int and len(xi) == ki, 'Invalid key'
             xi.append(new_container(kip1))
 
         elif ki not in xi:
             xi[ki] = new_container(kip1)
 
         xi = xi[ki]
 
     ki = k[-1]
-    if type(ki) is int and len(xi) == ki:
+    if isinstance(xi, list):
+        assert type(ki) is int and len(xi) == ki, 'Invalid key'
         xi.append(v)
     else:
         xi[ki] = v
 
     return x
 
 
@@ -1631,24 +1808,25 @@
     if x is None:
         return None
     elif x_type.minor == 'pandas':
         return x[columns]
     else:
         return x[:, columns]
 
+
 def recursive_device(x):
 
     if isinstance(x, dict):
         for xi in x.values():
             try:
                 return recursive_device(xi)
             except AttributeError:
                 # case of None
                 pass
-    elif isinstance(x, list) or isinstance(x, tuple):
+    elif isinstance(x, list):
         for xi in x:
             try:
                 return recursive_device(xi)
             except AttributeError:
                 # case of None
                 pass
     return x.device
@@ -1660,30 +1838,30 @@
         for xi in x.values():
             try:
                 return container_len(xi)
             except TypeError:
                 # case of None
                 pass
 
-    elif isinstance(x, list) or isinstance(x, tuple):
+    elif isinstance(x, list):
         for xi in x:
             try:
                 return container_len(xi)
             except TypeError:
                 # case of None
                 pass
 
     return len(x)
 
 
 def as_numpy(x):
 
     if isinstance(x, dict):
         return {k: as_numpy(v) for k, v in x.items()}
-    elif isinstance(x, list) or isinstance(x, tuple):
+    elif isinstance(x, list):
         return [as_numpy(s) for s in x]
 
     if isinstance(x, torch.Tensor):
         x = x.detach().cpu().numpy()
     else:
         x = np.array(x)
 
@@ -1694,17 +1872,18 @@
             x = float(x)
 
     return x
 
 
 def as_tensor(x, device=None, dtype=None, return_vector=False):
 
-    if isinstance(x, dict):
+    x_type = check_type(x)
+    if x_type.major == 'container' and x_type.minor == 'dict':
         return {k: as_tensor(v, device=device, return_vector=return_vector) for k, v in x.items()}
-    elif isinstance(x, list) or isinstance(x, tuple):
+    elif x_type.major == 'container' and x_type.minor in ['list', 'tuple']:
         return [as_tensor(s, device=device, return_vector=return_vector) for s in x]
     elif x is None:
         return None
 
     if dtype is None and hasattr(x, 'dtype'):
         if 'int' in str(x.dtype):
             dtype = torch.int64
```

### Comparing `beam-ds-2.0.2/src/beam_ds.egg-info/PKG-INFO` & `beam-ds-2.0.3/src/beam_ds.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: beam-ds
-Version: 2.0.2
+Version: 2.0.3
 Summary: Beam Datascience package
 Home-page: https://github.com/mlutils/beamds
 Author: Beam Maintainer
 Author-email: author@example.com
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mlutils/beamds/issues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -71,14 +73,31 @@
 
 Scalene is a high-performance python profiler that supports GPU profiling. 
 To analyze your code with Scalene use the following arguments:
 ```shell
 scalene --reduced-profile --outfile OUTFILE.html --html --- your_prog.py <your additional arguments>
 ```
 
+## Uploading the package to PyPi
+
+1. Install twine:
+```shell
+python -m pip install --user --upgrade twine
+```
+
+2. Build the package:
+```shell
+python -m build
+```
+
+3. Upload the package:
+```shell
+python -m twine upload --repository pypi dist/* 
+```
+
```

### Comparing `beam-ds-2.0.2/src/beam_ds.egg-info/SOURCES.txt` & `beam-ds-2.0.3/src/beam_ds.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,25 +5,29 @@
 setup.py
 src/beam/__init__.py
 src/beam/_version.py
 src/beam/algorithm.py
 src/beam/beam_mlflow.py
 src/beam/config.py
 src/beam/data.py
+src/beam/data1.py
 src/beam/data_tensor.py
 src/beam/dataset.py
 src/beam/experiment.py
+src/beam/explorer.py
+src/beam/logger.py
 src/beam/model.py
 src/beam/optim.py
 src/beam/packed_folds.py
 src/beam/parallel.py
 src/beam/path.py
 src/beam/processor.py
 src/beam/server.py
 src/beam/ssl.py
 src/beam/study.py
+src/beam/tensor.py
 src/beam/utils.py
 src/beam_ds.egg-info/PKG-INFO
 src/beam_ds.egg-info/SOURCES.txt
 src/beam_ds.egg-info/dependency_links.txt
 src/beam_ds.egg-info/requires.txt
 src/beam_ds.egg-info/top_level.txt
```

