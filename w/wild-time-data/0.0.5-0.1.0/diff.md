# Comparing `tmp/wild_time_data-0.0.5.tar.gz` & `tmp/wild_time_data-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wild_time_data-0.0.5.tar", last modified: Sun Apr 16 07:31:51 2023, max compression
+gzip compressed data, was "wild_time_data-0.1.0.tar", last modified: Tue May  9 16:39:22 2023, max compression
```

## Comparing `wild_time_data-0.0.5.tar` & `wild_time_data-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:31:51.996630 wild_time_data-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:31:51.992629 wild_time_data-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:31:51.992629 wild_time_data-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-16 07:31:51.992629 wild_time_data-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 07:31:51.996630 wild_time_data-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:31:51.992629 wild_time_data-0.0.5/wild_time_data/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/wild_time_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/wild_time_data/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/wild_time_data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/wild_time_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:31:51.992629 wild_time_data-0.0.5/wild_time_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-16 07:31:51.000000 wild_time_data-0.0.5/wild_time_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-16 07:31:51.000000 wild_time_data-0.0.5/wild_time_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 07:31:51.000000 wild_time_data-0.0.5/wild_time_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-16 07:31:51.000000 wild_time_data-0.0.5/wild_time_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 07:31:51.000000 wild_time_data-0.0.5/wild_time_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)   255896 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/yearbook.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:39:22.054627 wild_time_data-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:39:22.046626 wild_time_data-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:39:22.050626 wild_time_data-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-09 16:39:22.054627 wild_time_data-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:39:22.050626 wild_time_data-0.1.0/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/converter/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/converter/fmow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/converter/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:39:22.054627 wild_time_data-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:39:22.050626 wild_time_data-0.1.0/wild_time_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/wild_time_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/wild_time_data/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/wild_time_data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/wild_time_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:39:22.054627 wild_time_data-0.1.0/wild_time_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-09 16:39:22.000000 wild_time_data-0.1.0/wild_time_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-09 16:39:22.000000 wild_time_data-0.1.0/wild_time_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:39:22.000000 wild_time_data-0.1.0/wild_time_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-09 16:39:22.000000 wild_time_data-0.1.0/wild_time_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 16:39:22.000000 wild_time_data-0.1.0/wild_time_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   255896 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/yearbook.png
```

### Comparing `wild_time_data-0.0.5/.github/workflows/pypi_publish.yml` & `wild_time_data-0.1.0/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.0.5/.gitignore` & `wild_time_data-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.0.5/LICENSE` & `wild_time_data-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.0.5/PKG-INFO` & `wild_time_data-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild_time_data
-Version: 0.0.5
+Version: 0.1.0
 Summary: WILDS distribution shift data
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,17 @@
 Wild-Time-Data: Easy access to the Wild-Time data
 *************************************************
 
 This repository provides a simpler interface to access the
 `Wild-Time datasets <https://github.com/huaxiuyao/Wild-Time>`_ in PyTorch.
 In contrast to the original repository, this repository contains only code relevant for data loading
 and has fewer dependencies.
+Furthermore, we no longer use pickle to store the data but store it as HDF5 which has two advantages.
+First, this is more space-efficient, e.g., for the yearbook dataset the data file size changed from 1.7GB to only 37MB.
+Second, it addresses a security concern people may have when using unknown pickled Python objects.
 
 .. image:: yearbook.png
    :align: center
 
 
 Installation
 ============
@@ -59,30 +62,48 @@
     .. code-block:: python
 
       from wild_time_data import available_time_steps
 
       available_time_steps("arxiv")
 
 * ``split``: Selects the partition. Can either be ``train`` or ``test``.
+* ``transform``: Defines custom transformations on the predictors of a data point. Can be used to normalize, augment or tokenize data. By default, no transformation is applied for text datasets, image are converted to Tensors via ``transforms.ToTensor()``, and the data for ``Drug`` is one-hot encoded. Additionally, ``FMoW`` images are normalized. The default transformation can be accessed via
+
+    .. code-block:: python
+
+      from wild_time_data import default_transform
+
+      default_transform("huffpost")
+
+* ``target_transform``: Same as ``transform`` but for labels. By default, no transformation is applied.
+* ``in_memory``: If set to ``True``, all data is loaded in memory. By default, data is loaded from disk which might be slower but requires less memory. For all datasets but ``FMoW`` ``in_memory=True`` should work on most hardware.
 * ``data_dir``: Location where to store the data. By default it will be downloaded to ``~/wild-time-data/``.
 
 Other Useful Functions
 ======================
 
 Several other functions can be imported from ``wild_time_data``.
 
 .. code-block:: python
 
   from wild_time_data import available_time_steps, input_dim, list_datasets, num_outputs
 
 * ``available_time_steps``: Given the dataset name, a sorted list of available time steps is returned. Example: ``available_time_steps("huffpost")`` returns ``[2012, 2013, 2014, 2015, 2016, 2017, 2018]``.
+* ``default_transform``: Given the dataset name, the transformation which is applied to the predictors unless a custom transformation is passed. Example: ``default_transform("yearbook")`` returns ``transfroms.ToTensor()``. If the return value is ``None``, no transformation is applied. In order to override a default transformation, pass ``transform=lambda x: x`` to ``load_dataset``.
 * ``input_dim``: Given the dataset name, the input dimensionality is returned. For image datasets the shape of the image is returned. For text datasets the maximum number of words separated by spaces is returned. Example: ``input_dim("yearbook")`` returns ``(1, 32, 32)``.
 * ``list_datasets``: Returns the list of all available datasets. Example: ``list_datasets()`` returns ``["arxiv", "drug", "fmow", "huffpost", "yearbook"]``.
 * ``num_outputs``: Given the dataset name, either the number of classes is returned or it returns 1. In cases where 1 is returned, this indicates that this is a regression dataset. Example: ``num_outputs("arxiv")`` returns ``172``.
 
+
+FMoW Dataset
+============
+
+If you want to use the FMoW dataset, please follow `the instructions to prepare it <https://github.com/wistuba/Wild-Time-Data/tree/main/converter>`__.
+
+
 Licenses
 ========
 All additional code for Wild-Time-Data is available under the Apache 2.0 license.
 The license for each Wild-Time dataset is listed below:
 
 * arXiv: CC0: Public Domain
 * Drug-BA: MIT License
```

### Comparing `wild_time_data-0.0.5/pyproject.toml` & `wild_time_data-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,17 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
 ]
 requires-python = ">=3.8, <=3.10"
 dynamic = ["version", "readme", "dependencies"]
 
+[tool.setuptools]
+packages = ["wild_time_data"]
+
 [tool.setuptools.dynamic]
 version = {attr = "wild_time_data.__version__"}
 readme = {file = ["README.rst"]}
 dependencies = {file = ["requirements.txt"]}
 
 [tool.black]
 line-length = 100
```

### Comparing `wild_time_data-0.0.5/wild_time_data/core.py` & `wild_time_data-0.1.0/wild_time_data/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,54 +5,82 @@
 dataset_classes = {
     "arxiv": ArXiv,
     "drug": Drug,
     "fmow": FMoW,
     "huffpost": HuffPost,
     "yearbook": Yearbook,
 }
-splits = {"train": 0, "test": 1}
+
+
+def _check_dataset_exists(dataset_name):
+    if dataset_name not in dataset_classes:
+        raise ValueError(
+            f"Unknown dataset {dataset_name}. Available datasets are {dataset_classes.keys()}"
+        )
 
 
 def available_time_steps(dataset_name):
     """Lists all available time steps."""
+    _check_dataset_exists(dataset_name)
     return dataset_classes[dataset_name].time_steps
 
 
 def input_dim(dataset_name):
     """Returns the input dimensionality of the data.
 
     Image datasets: image shape
     Text datasets: highest number of words in a sentence
     Protein datasets: list of two tuples
     """
+    _check_dataset_exists(dataset_name)
     return dataset_classes[dataset_name].input_dim
 
 
 def num_outputs(dataset_name):
     """Returns the number of classes for a classification task (num_outputs > 1) and 1 for a regression task."""
-    return dataset_classes[dataset_name].num_classes
+    _check_dataset_exists(dataset_name)
+    return dataset_classes[dataset_name].num_outputs
+
+
+def default_transform(dataset_name):
+    """Returns the default transformation applied to the predictors."""
+    _check_dataset_exists(dataset_name)
+    return dataset_classes[dataset_name].default_transform
 
 
 def list_datasets():
     """Lists all available dataset names."""
     return list(dataset_classes.keys())
 
 
-def load_dataset(dataset_name, time_step, split, data_dir=os.path.expanduser("~/wild-time-data")):
+def load_dataset(
+    dataset_name,
+    time_step,
+    split,
+    transform=None,
+    target_transform=None,
+    in_memory=False,
+    data_dir=os.path.expanduser("~/wild-time-data"),
+):
     """Loads the different Wild-Time datasets.
 
     Args:
         dataset_name: The name of the respective dataset.
         time_step: Indicate the time slice. Available time slices can be accessed via ``available_time_steps()``.
         split: Whether to load train or test split.
+        transform: Change default transformations on the predictors of a data point. Can be used to normalize, augment or tokenize data.
+        target_transform: Add a transformation to the labels.
+        in_memory: If ``True``, the entire data will be loaded into memory.
         data_dir: Location where the data is stored.
     """
-    if dataset_name not in dataset_classes:
-        raise ValueError(
-            f"Unknown dataset {dataset_name}. Available datasets are {dataset_classes.keys()}"
-        )
-    if split not in splits:
+    _check_dataset_exists(dataset_name)
+    if split not in ["train", "test"]:
         raise ValueError("Only available splits are train and test.")
 
     return dataset_classes[dataset_name](
-        time_step=time_step, split=splits[split], data_dir=data_dir
+        time_step=time_step,
+        split=split,
+        transform=transform,
+        target_transform=target_transform,
+        in_memory=in_memory,
+        data_dir=data_dir,
     )
```

### Comparing `wild_time_data-0.0.5/wild_time_data/utils.py` & `wild_time_data-0.1.0/wild_time_data/utils.py`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.0.5/wild_time_data.egg-info/PKG-INFO` & `wild_time_data-0.1.0/wild_time_data.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-time-data
-Version: 0.0.5
+Version: 0.1.0
 Summary: WILDS distribution shift data
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,17 @@
 Wild-Time-Data: Easy access to the Wild-Time data
 *************************************************
 
 This repository provides a simpler interface to access the
 `Wild-Time datasets <https://github.com/huaxiuyao/Wild-Time>`_ in PyTorch.
 In contrast to the original repository, this repository contains only code relevant for data loading
 and has fewer dependencies.
+Furthermore, we no longer use pickle to store the data but store it as HDF5 which has two advantages.
+First, this is more space-efficient, e.g., for the yearbook dataset the data file size changed from 1.7GB to only 37MB.
+Second, it addresses a security concern people may have when using unknown pickled Python objects.
 
 .. image:: yearbook.png
    :align: center
 
 
 Installation
 ============
@@ -59,30 +62,48 @@
     .. code-block:: python
 
       from wild_time_data import available_time_steps
 
       available_time_steps("arxiv")
 
 * ``split``: Selects the partition. Can either be ``train`` or ``test``.
+* ``transform``: Defines custom transformations on the predictors of a data point. Can be used to normalize, augment or tokenize data. By default, no transformation is applied for text datasets, image are converted to Tensors via ``transforms.ToTensor()``, and the data for ``Drug`` is one-hot encoded. Additionally, ``FMoW`` images are normalized. The default transformation can be accessed via
+
+    .. code-block:: python
+
+      from wild_time_data import default_transform
+
+      default_transform("huffpost")
+
+* ``target_transform``: Same as ``transform`` but for labels. By default, no transformation is applied.
+* ``in_memory``: If set to ``True``, all data is loaded in memory. By default, data is loaded from disk which might be slower but requires less memory. For all datasets but ``FMoW`` ``in_memory=True`` should work on most hardware.
 * ``data_dir``: Location where to store the data. By default it will be downloaded to ``~/wild-time-data/``.
 
 Other Useful Functions
 ======================
 
 Several other functions can be imported from ``wild_time_data``.
 
 .. code-block:: python
 
   from wild_time_data import available_time_steps, input_dim, list_datasets, num_outputs
 
 * ``available_time_steps``: Given the dataset name, a sorted list of available time steps is returned. Example: ``available_time_steps("huffpost")`` returns ``[2012, 2013, 2014, 2015, 2016, 2017, 2018]``.
+* ``default_transform``: Given the dataset name, the transformation which is applied to the predictors unless a custom transformation is passed. Example: ``default_transform("yearbook")`` returns ``transfroms.ToTensor()``. If the return value is ``None``, no transformation is applied. In order to override a default transformation, pass ``transform=lambda x: x`` to ``load_dataset``.
 * ``input_dim``: Given the dataset name, the input dimensionality is returned. For image datasets the shape of the image is returned. For text datasets the maximum number of words separated by spaces is returned. Example: ``input_dim("yearbook")`` returns ``(1, 32, 32)``.
 * ``list_datasets``: Returns the list of all available datasets. Example: ``list_datasets()`` returns ``["arxiv", "drug", "fmow", "huffpost", "yearbook"]``.
 * ``num_outputs``: Given the dataset name, either the number of classes is returned or it returns 1. In cases where 1 is returned, this indicates that this is a regression dataset. Example: ``num_outputs("arxiv")`` returns ``172``.
 
+
+FMoW Dataset
+============
+
+If you want to use the FMoW dataset, please follow `the instructions to prepare it <https://github.com/wistuba/Wild-Time-Data/tree/main/converter>`__.
+
+
 Licenses
 ========
 All additional code for Wild-Time-Data is available under the Apache 2.0 license.
 The license for each Wild-Time dataset is listed below:
 
 * arXiv: CC0: Public Domain
 * Drug-BA: MIT License
```

### Comparing `wild_time_data-0.0.5/yearbook.png` & `wild_time_data-0.1.0/yearbook.png`

 * *Files identical despite different names*

