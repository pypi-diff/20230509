# Comparing `tmp/neuraloperator-0.1.1.tar.gz` & `tmp/neuraloperator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuraloperator-0.1.1.tar", last modified: Wed Feb 22 01:29:48 2023, max compression
+gzip compressed data, was "neuraloperator-0.2.0.tar", last modified: Tue May  9 02:31:44 2023, max compression
```

## Comparing `neuraloperator-0.1.1.tar` & `neuraloperator-0.2.0.tar`

### file list

```diff
@@ -1,53 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 01:29:48.387712 neuraloperator-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-02-22 01:29:48.387712 neuraloperator-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 01:29:48.383712 neuraloperator-0.1.1/neuralop/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 01:29:48.383712 neuraloperator-0.1.1/neuralop/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/datasets/burgers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/datasets/darcy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/datasets/hdf5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/datasets/navier_stokes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/datasets/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/datasets/tensor_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/datasets/zarr_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 01:29:48.383712 neuraloperator-0.1.1/neuralop/models/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18630 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/models/fno_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/models/fourier_continuation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/models/model_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/models/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/models/skip_connections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 01:29:48.383712 neuraloperator-0.1.1/neuralop/models/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/models/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/models/tests/test_fno_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/models/tests/test_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/models/tests/test_tfno.py
--rw-r--r--   0 runner    (1001) docker     (123)    25348 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/models/tfno.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 01:29:48.383712 neuraloperator-0.1.1/neuralop/mpu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/mpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/mpu/comm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/mpu/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/mpu/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 01:29:48.383712 neuraloperator-0.1.1/neuralop/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/tests/test_model_from_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 01:29:48.383712 neuraloperator-0.1.1/neuralop/training/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/training/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/training/patching.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/training/torch_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/training/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/neuralop/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 01:29:48.387712 neuraloperator-0.1.1/neuraloperator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-02-22 01:29:48.000000 neuraloperator-0.1.1/neuraloperator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-02-22 01:29:48.000000 neuraloperator-0.1.1/neuraloperator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 01:29:48.000000 neuraloperator-0.1.1/neuraloperator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-22 01:29:48.000000 neuraloperator-0.1.1/neuraloperator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 01:29:48.000000 neuraloperator-0.1.1/neuraloperator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 01:29:48.387712 neuraloperator-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-02-22 01:29:03.000000 neuraloperator-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:31:44.669474 neuraloperator-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-09 02:31:44.665474 neuraloperator-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:31:44.657474 neuraloperator-0.2.0/neuralop/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:31:44.657474 neuraloperator-0.2.0/neuralop/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/datasets/burgers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/datasets/darcy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:31:44.661474 neuraloperator-0.2.0/neuralop/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    64999 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/datasets/data/darcy_test_16.pt
+-rw-r--r--   0 runner    (1001) docker     (123)   256999 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/datasets/data/darcy_test_32.pt
+-rw-r--r--   0 runner    (1001) docker     (123)  1280999 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/datasets/data/darcy_train_16.pt
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/datasets/hdf5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/datasets/navier_stokes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/datasets/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/datasets/pt_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/datasets/tensor_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/datasets/zarr_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:31:44.665474 neuraloperator-0.2.0/neuralop/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/fno_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/fourier_continuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/model_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/skip_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/spectral_convolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:31:44.665474 neuraloperator-0.2.0/neuralop/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/tests/test_fno_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/tests/test_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/tests/test_spectral_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/tests/test_tfno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/tests/test_uno.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25148 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/tfno.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/models/uno.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:31:44.665474 neuraloperator-0.2.0/neuralop/mpu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/mpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/mpu/comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/mpu/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/mpu/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:31:44.665474 neuraloperator-0.2.0/neuralop/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/tests/test_model_from_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:31:44.665474 neuraloperator-0.2.0/neuralop/training/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/training/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/training/patching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/training/torch_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/training/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/neuralop/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:31:44.665474 neuraloperator-0.2.0/neuraloperator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-09 02:31:44.000000 neuraloperator-0.2.0/neuraloperator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-09 02:31:44.000000 neuraloperator-0.2.0/neuraloperator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 02:31:44.000000 neuraloperator-0.2.0/neuraloperator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 02:31:44.000000 neuraloperator-0.2.0/neuraloperator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 02:31:44.000000 neuraloperator-0.2.0/neuraloperator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 02:31:44.669474 neuraloperator-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-09 02:30:12.000000 neuraloperator-0.2.0/setup.py
```

### Comparing `neuraloperator-0.1.1/LICENSE` & `neuraloperator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/PKG-INFO` & `neuraloperator-0.2.0/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: neuraloperator
-Version: 0.1.1
-Summary: Learning (Tensorized) Neural Operators in PyTorch.
-Home-page: UNKNOWN
-License: Modified BSD
-Platform: UNKNOWN
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 .. image:: https://img.shields.io/pypi/v/neuraloperator
    :target: https://pypi.org/project/neuraloperator/
    :alt: PyPI
 
 .. image:: https://github.com/NeuralOperator/neuraloperator/actions/workflows/test.yml/badge.svg
    :target: https://github.com/NeuralOperator/neuraloperator/actions/workflows/test.yml
 
@@ -58,17 +45,17 @@
 ----------
 
 After you've installed the library, you can start training operators seemlessly:
 
 
 .. code-block:: python
 
-   from neuralop.models import TFNO
+   from neuralop.models import FNO
 
-   operator = TFNO(n_modes=(16, 16), hidden_channels=64,
+   operator = FNO(n_modes=(16, 16), hidden_channels=64,
                    in_channels=3, out_channels=1)
 
 Tensorization is also provided out of the box: you can improve the previous models
 by simply using a Tucker Tensorized FNO with just a few parameters:
 
 .. code-block:: python
 
@@ -91,10 +78,39 @@
 Using with weights and biases
 -----------------------------
 
 Create a file in `neuraloperator/config` called `wandb_api_key.txt` and paste your Weights and Biases API key there.
 You can configure the project you want to use and your username in the main yaml configuration files.
 
 
+Citing
+------
+
+If you use NeuralOperator in an academic paper, please cite [1]_, [2]_::
+
+   @misc{li2020fourier,
+      title={Fourier Neural Operator for Parametric Partial Differential Equations}, 
+      author={Zongyi Li and Nikola Kovachki and Kamyar Azizzadenesheli and Burigede Liu and Kaushik Bhattacharya and Andrew Stuart and Anima Anandkumar},
+      year={2020},
+      eprint={2010.08895},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
+   }
+
+   @article{kovachki2021neural,
+      author    = {Nikola B. Kovachki and
+                     Zongyi Li and
+                     Burigede Liu and
+                     Kamyar Azizzadenesheli and
+                     Kaushik Bhattacharya and
+                     Andrew M. Stuart and
+                     Anima Anandkumar},
+      title     = {Neural Operator: Learning Maps Between Function Spaces},
+      journal   = {CoRR},
+      volume    = {abs/2108.08481},
+      year      = {2021},
+   }
 
 
+.. [1] Li, Z., Kovachki, N., Azizzadenesheli, K., Liu, B., Bhattacharya, K., Stuart, A., and Anandkumar A., “Fourier Neural Operator for Parametric Partial Differential Equations”, ICLR, 2021. doi:10.48550/arXiv.2010.08895.
 
+.. [2] Kovachki, N., Li, Z., Liu, B., Azizzadenesheli, K., Bhattacharya, K., Stuart, A., and Anandkumar A., “Neural Operator: Learning Maps Between Function Spaces”, JMLR, 2021. doi:10.48550/arXiv.2108.08481.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `neuraloperator-0.1.1/neuralop/datasets/burgers.py` & `neuraloperator-0.2.0/neuralop/datasets/burgers.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/datasets/darcy.py` & `neuraloperator-0.2.0/neuralop/datasets/darcy.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/datasets/hdf5_dataset.py` & `neuraloperator-0.2.0/neuralop/datasets/hdf5_dataset.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/datasets/navier_stokes.py` & `neuraloperator-0.2.0/neuralop/datasets/navier_stokes.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         
         transform_y = Normalizer(y_mean, y_std)
 
     training_db.transform_x = transforms.Compose(transform_x)
     training_db.transform_y = transform_y
     
     train_loader = torch.utils.data.DataLoader(training_db,
-                                               batch_size=batch_size, 
+                                               batch_size=batch_size, drop_last=True,
                                                shuffle=True,
                                                num_workers=num_workers,
                                                pin_memory=pin_memory,
                                                persistent_workers=persistent_workers)
 
     test_loaders = dict()
     for (res, n_test, test_batch_size) in zip(test_resolutions, n_tests, test_batch_sizes):
@@ -200,15 +200,15 @@
         output_encoder = UnitGaussianNormalizer(y_train, reduce_dim=reduce_dims)
         y_train = output_encoder.encode(y_train)
     else:
         output_encoder = None
 
     train_db = TensorDataset(x_train, y_train, transform_x=PositionalEmbedding(grid_boundaries, 0) if positional_encoding else None)
     train_loader = torch.utils.data.DataLoader(train_db,
-                                               batch_size=batch_size, shuffle=True,
+                                               batch_size=batch_size, shuffle=True, drop_last=True,
                                                num_workers=num_workers, pin_memory=pin_memory, persistent_workers=persistent_workers)
 
     test_db = TensorDataset(x_test, y_test,transform_x=PositionalEmbedding(grid_boundaries, 0) if positional_encoding else None)
     test_loader = torch.utils.data.DataLoader(test_db,
                                               batch_size=test_batch_size, shuffle=False,
                                               num_workers=num_workers, pin_memory=pin_memory, persistent_workers=persistent_workers)
```

### Comparing `neuraloperator-0.1.1/neuralop/datasets/positional_encoding.py` & `neuraloperator-0.2.0/neuralop/datasets/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/datasets/transforms.py` & `neuraloperator-0.2.0/neuralop/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/datasets/zarr_dataset.py` & `neuraloperator-0.2.0/neuralop/datasets/zarr_dataset.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/models/fno_block.py` & `neuraloperator-0.2.0/neuralop/models/spectral_convolution.py`

 * *Files 16% similar despite different names*

```diff
@@ -120,21 +120,21 @@
             return _contract_dense_separable
         else:
             return _contract_dense
     elif implementation == 'factorized':
         if torch.is_tensor(weight):
             return _contract_dense
         elif isinstance(weight, FactorizedTensor):
-            if weight.name.lower() == 'complexdense':
+            if weight.name.lower().endswith('dense'):
                 return _contract_dense
-            elif weight.name.lower() == 'complextucker':
+            elif weight.name.lower().endswith('tucker'):
                 return _contract_tucker
-            elif weight.name.lower() == 'complextt':
+            elif weight.name.lower().endswith('tt'):
                 return _contract_tt
-            elif weight.name.lower() == 'complexcp':
+            elif weight.name.lower().endswith('cp'):
                 return _contract_cp
             else:
                 raise ValueError(f'Got unexpected factorized weight type {weight.name}')
         else:
             raise ValueError(f'Got unexpected weight type of class {weight.__class__.__name__}')
     else:
         raise ValueError(f'Got {implementation=}, expected "reconstructed" or "factorized"')
@@ -145,21 +145,28 @@
 
     Parameters
     ----------
     in_channels : int, optional
         Number of input channels
     out_channels : int, optional
         Number of output channels
-    kept_modes : int tuple
+    n_modes : int tuple
         total number of modes to keep in Fourier Layer, along each dim
     separable : bool, default is True
-    scale : float or 'auto', default is 'auto'
-        scale to use for the init
+    init_std : float or 'auto', default is 'auto'
+        std to use for the init
     n_layers : int, optional
         Number of Fourier Layers, by default 4
+    incremental_n_modes : None or int tuple, default is None
+        * If not None, this allows to incrementally increase the number of modes in Fourier domain 
+          during training. Has to verify n <= N for (n, m) in zip(incremental_n_modes, n_modes).
+        
+        * If None, all the n_modes are used.
+
+        This can be updated dynamically during training.
     joint_factorization : bool, optional
         Whether all the Fourier Layers should be parametrized by a single tensor (vs one per layer), by default False
     rank : float or rank, optional
         Rank of the tensor factorization of the Fourier weights, by default 1.0
     factorization : str, {'tucker', 'cp', 'tt'}, optional
         Tensor factorization of the parameters weight to use, by default 'tucker'
     fixed_rank_modes : bool, optional
@@ -169,125 +176,170 @@
     implementation : {'factorized', 'reconstructed'}, optional, default is 'factorized'
         If factorization is not None, forward mode to use::
         * `reconstructed` : the full weight tensor is reconstructed from the factorization and used for the forward pass
         * `factorized` : the input is directly contracted with the factors of the decomposition
     decomposition_kwargs : dict, optional, default is {}
         Optionaly additional parameters to pass to the tensor decomposition
     """
-    def __init__(self, in_channels, out_channels, n_modes, n_layers=1, scale='auto', separable=False,
-                 fft_norm='backward', bias=True, implementation='reconstructed', joint_factorization=False,
-                 rank=0.5, factorization='cp', fixed_rank_modes=False, decomposition_kwargs=dict()):
+    def __init__(self, in_channels, out_channels, n_modes, incremental_n_modes=None, bias=True,
+                 n_layers=1, separable=False, output_scaling_factor=None,
+                 rank=0.5, factorization='cp', implementation='reconstructed', 
+                 fixed_rank_modes=False, joint_factorization=False, decomposition_kwargs=dict(),
+                 init_std='auto', fft_norm='backward'):
         super().__init__()
 
         self.in_channels = in_channels
         self.out_channels = out_channels
-        self.order = len(n_modes)
+        self.joint_factorization = joint_factorization
 
         # We index quadrands only
         # n_modes is the total number of modes kept along each dimension
-        # half_modes is half of that except in the last mode, correponding to the number of modes to keep in *each* quadrant for each dim
+        # half_n_modes is half of that except in the last mode, correponding to the number of modes to keep in *each* quadrant for each dim
         if isinstance(n_modes, int):
             n_modes = [n_modes]
         self.n_modes = n_modes
-        half_modes = [m//2 for m in n_modes]
-        self.half_modes = half_modes
+        self.order = len(n_modes)
+
+        half_total_n_modes = [m//2 for m in n_modes]
+        self.half_total_n_modes = half_total_n_modes
+
+        # WE use half_total_n_modes to build the full weights
+        # During training we can adjust incremental_n_modes which will also
+        # update half_n_modes 
+        # So that we can train on a smaller part of the Fourier modes and total weights
+        self.incremental_n_modes = incremental_n_modes
 
         self.rank = rank
         self.factorization = factorization
         self.n_layers = n_layers
         self.implementation = implementation
 
-        if scale == 'auto':
-            scale = (1 / (in_channels * out_channels))
+        if output_scaling_factor is not None:
+            if isinstance(output_scaling_factor, (float, int)):
+                output_scaling_factor = [float(output_scaling_factor)]*len(self.n_modes)
+        self.output_scaling_factor = output_scaling_factor
+
+        if init_std == 'auto':
+            init_std = (1 / (in_channels * out_channels))
+        else:
+            init_std = 0.02
 
         if isinstance(fixed_rank_modes, bool):
             if fixed_rank_modes:
                 # If bool, keep the number of layers fixed
                 fixed_rank_modes=[0]
             else:
                 fixed_rank_modes=None
-
-        self.mlp = None
-
         self.fft_norm = fft_norm
 
-        # Make sure we are using a Complex Factorized Tensor
+        # Make sure we are using a Complex Factorized Tensor to parametrize the conv
         if factorization is None:
             factorization = 'Dense' # No factorization
         if not factorization.lower().startswith('complex'):
             factorization = f'Complex{factorization}'
-    
+
         if separable:
             if in_channels != out_channels:
                 raise ValueError('To use separable Fourier Conv, in_channels must be equal to out_channels, ',
                                  f'but got {in_channels=} and {out_channels=}')
-            weight_shape = (in_channels, *self.half_modes)
+            weight_shape = (in_channels, *half_total_n_modes)
         else:
-            weight_shape = (in_channels, out_channels, *self.half_modes)
+            weight_shape = (in_channels, out_channels, *half_total_n_modes)
         self.separable = separable
 
+        self.n_weights_per_layer = 2**(self.order-1)
         if joint_factorization:
-            self.weight = FactorizedTensor.new(((2**(self.order-1))*n_layers, *weight_shape),
+            self.weight = FactorizedTensor.new((self.n_weights_per_layer*n_layers, *weight_shape),
                                                 rank=self.rank, factorization=factorization, 
                                                 fixed_rank_modes=fixed_rank_modes,
                                                 **decomposition_kwargs)
-            self.weight.normal_(0, scale)
+            self.weight.normal_(0, init_std)
         else:
             self.weight = nn.ModuleList([
                  FactorizedTensor.new(
                     weight_shape,
                     rank=self.rank, factorization=factorization, 
                     fixed_rank_modes=fixed_rank_modes,
                     **decomposition_kwargs
-                    ) for _ in range((2**(self.order-1))*n_layers)]
+                    ) for _ in range(self.n_weights_per_layer*n_layers)]
                 )
             for w in self.weight:
-                w.normal_(0, scale)
-
+                w.normal_(0, init_std)
         self._contract = get_contract_fun(self.weight[0], implementation=implementation, separable=separable)
 
         if bias:
-            self.bias = nn.Parameter(scale * torch.randn(*((n_layers, self.out_channels) + (1, )*self.order)))
+            self.bias = nn.Parameter(init_std * torch.randn(*((n_layers, self.out_channels) + (1, )*self.order)))
         else:
             self.bias = None
 
+    def _get_weight(self, index):
+        if self.incremental_n_modes is not None:
+            return self.weight[index][self.weight_slices]
+        else:
+            return self.weight[index]
+
+    @property
+    def incremental_n_modes(self):
+        return self._incremental_n_modes
+
+    @incremental_n_modes.setter
+    def incremental_n_modes(self, incremental_n_modes):
+        if incremental_n_modes is None:
+            self._incremental_n_modes = None
+            self.half_n_modes = [m//2 for m in self.n_modes]
+
+        else:
+            if isinstance(incremental_n_modes, int):
+                self._incremental_n_modes = [incremental_n_modes]*len(self.n_modes)
+            else:
+                if len(incremental_n_modes) == len(self.n_modes):
+                    self._incremental_n_modes = incremental_n_modes
+                else:
+                    raise ValueError(f'Provided {incremental_n_modes} for actual n_modes={self.n_modes}.')
+            self.weight_slices = [slice(None)]*2 + [slice(None, n//2) for n in self._incremental_n_modes]
+            self.half_n_modes = [m//2 for m in self._incremental_n_modes]
+
     def forward(self, x, indices=0):
         """Generic forward pass for the Factorized Spectral Conv
-        
-        Parameters 
+
+        Parameters
         ----------
         x : torch.Tensor
             input activation of size (batch_size, channels, d1, ..., dN)
         indices : int, default is 0
             if joint_factorization, index of the layers for n_layers > 1
-        
+
         Returns
         -------
         tensorized_spectral_conv(x)
         """
         batchsize, channels, *mode_sizes = x.shape
+
         fft_size = list(mode_sizes)
         fft_size[-1] = fft_size[-1]//2 + 1 # Redundant last coefficient
         
-        #Compute Fourier coeffcients 
+        #Compute Fourier coeffcients
         fft_dims = list(range(-self.order, 0))
         x = torch.fft.rfftn(x.float(), norm=self.fft_norm, dim=fft_dims)
 
         out_fft = torch.zeros([batchsize, self.out_channels, *fft_size], device=x.device, dtype=torch.cfloat)
         
         # We contract all corners of the Fourier coefs
         # Except for the last mode: there, we take all coefs as redundant modes were already removed
-        mode_indexing = [((None, m), (-m, None)) for m in self.half_modes[:-1]] + [((None, self.half_modes[-1]), )]
+        mode_indexing = [((None, m), (-m, None)) for m in self.half_n_modes[:-1]] + [((None, self.half_n_modes[-1]), )]
 
         for i, boundaries in enumerate(itertools.product(*mode_indexing)):
             # Keep all modes for first 2 modes (batch-size and channels)
             idx_tuple = [slice(None), slice(None)] + [slice(*b) for b in boundaries]
-            
+
             # For 2D: [:, :, :height, :width] and [:, :, -height:, width]
-            out_fft[idx_tuple] = self._contract(x[idx_tuple], self.weight[indices + i], separable=self.separable)
+            out_fft[idx_tuple] = self._contract(x[idx_tuple], self._get_weight(self.n_weights_per_layer*indices + i), separable=self.separable)
+
+        if self.output_scaling_factor is not None:
+            mode_sizes = tuple([int(round(s*r)) for (s, r) in zip(mode_sizes, self.output_scaling_factor)])
 
         x = torch.fft.irfftn(out_fft, s=(mode_sizes), norm=self.fft_norm)
 
         if self.bias is not None:
             x = x + self.bias[indices, ...]
 
         return x
@@ -296,22 +348,22 @@
         """Returns a sub-convolutional layer from the joint parametrize main-convolution
 
         The parametrization of sub-convolutional layers is shared with the main one.
         """
         if self.n_layers == 1:
             raise ValueError('A single convolution is parametrized, directly use the main class.')
         
-        return SubConv2d(self, indices)
+        return SubConv(self, indices)
     
     def __getitem__(self, indices):
         return self.get_conv(indices)
 
 
 
-class SubConv2d(nn.Module):
+class SubConv(nn.Module):
     """Class representing one of the convolutions from the mother joint factorized convolution
 
     Notes
     -----
     This relies on the fact that nn.Parameters are not duplicated:
     if the same nn.Parameter is assigned to multiple modules, they all point to the same data, 
     which is shared.
@@ -322,114 +374,82 @@
         self.indices = indices
     
     def forward(self, x):
         return self.main_conv.forward(x, self.indices)
 
 
 class FactorizedSpectralConv1d(FactorizedSpectralConv):
-    def __init__(
-        self, in_channels, out_channels, modes_height,
-        n_layers=1, scale='auto', separable=False,
-        fft_norm='backward', bias=True, implementation='reconstucted',
-        joint_factorization=False, rank=0.5, factorization='cp',
-        fixed_rank_modes=False, decomposition_kwargs=dict()):
-        super().__init__(in_channels, out_channels, (modes_height, ),
-            n_layers=n_layers, scale=scale, separable=separable,
-            fft_norm=fft_norm, bias=bias, implementation=implementation,
-            joint_factorization=joint_factorization, rank=rank, 
-            factorization=factorization, fixed_rank_modes=fixed_rank_modes,
-            decomposition_kwargs=decomposition_kwargs
-            )
-        self.half_modes_height = self.half_modes[0]
-
     def forward(self, x, indices=0):
         batchsize, channels, width = x.shape
 
         x = torch.fft.rfft(x, norm=self.fft_norm)
 
         out_fft = torch.zeros([batchsize, self.out_channels,  width//2 + 1], device=x.device, dtype=torch.cfloat)
-        out_fft[:, :, :self.half_modes_height] = self._contract(x[:, :, :self.half_modes_height], self.weight[indices], separable=self.separable)
+        out_fft[:, :, :self.half_n_modes[0]] = self._contract(x[:, :, :self.half_n_modes[0]], self._get_weight(indices), separable=self.separable)
+        
+        if self.output_scaling_factor is not None:
+            width = int(round(width*self.output_scaling_factor[0]))
 
         x = torch.fft.irfft(out_fft, n=width, norm=self.fft_norm)
 
         if self.bias is not None:
             x = x + self.bias[indices, ...]
 
         return x
 
 
 class FactorizedSpectralConv2d(FactorizedSpectralConv):
-    def __init__(self, in_channels, out_channels, modes_height, modes_width, n_layers=1, scale='auto', separable=False,
-                 fft_norm='backward', bias=True, implementation='reconstucted', joint_factorization=False,
-                 rank=0.5, factorization='cp', fixed_rank_modes=False, decomposition_kwargs=dict()):
-        super().__init__(
-            in_channels, out_channels, (modes_height, modes_width),
-            n_layers=n_layers, scale=scale, separable=separable,
-            fft_norm=fft_norm, bias=bias, implementation=implementation,
-            joint_factorization=joint_factorization, rank=rank, 
-            factorization=factorization, fixed_rank_modes=fixed_rank_modes,
-            decomposition_kwargs=decomposition_kwargs
-            )
-        self.half_modes_height, self.half_modes_width = self.half_modes
-
     def forward(self, x, indices=0):
         batchsize, channels, height, width = x.shape
 
         x = torch.fft.rfft2(x.float(), norm=self.fft_norm)
 
         # The output will be of size (batch_size, self.out_channels, x.size(-2), x.size(-1)//2 + 1)
         out_fft = torch.zeros([batchsize, self.out_channels, height, width//2 + 1], dtype=x.dtype, device=x.device)
 
         # upper block (truncate high freq)
-        out_fft[:, :, :self.half_modes_height, :self.half_modes_width] = self._contract(x[:, :, :self.half_modes_height, :self.half_modes_width], 
-                                                                              self.weight[2*indices], separable=self.separable)
+        out_fft[:, :, :self.half_n_modes[0], :self.half_n_modes[1]] = self._contract(x[:, :, :self.half_n_modes[0], :self.half_n_modes[1]], 
+                                                                              self._get_weight(2*indices), separable=self.separable)
         # Lower block
-        out_fft[:, :, -self.half_modes_height:, :self.half_modes_width] = self._contract(x[:, :, -self.half_modes_height:, :self.half_modes_width],
-                                                                               self.weight[2*indices + 1], separable=self.separable)
+        out_fft[:, :, -self.half_n_modes[0]:, :self.half_n_modes[1]] = self._contract(x[:, :, -self.half_n_modes[0]:, :self.half_n_modes[1]],
+                                                                              self._get_weight(2*indices + 1), separable=self.separable)
+        
+        if self.output_scaling_factor is not None:
+            width = int(round(width*self.output_scaling_factor[0]))
+            height = int(round(height*self.output_scaling_factor[1]))
 
         x = torch.fft.irfft2(out_fft, s=(height, width), dim=(-2, -1), norm=self.fft_norm)
 
         if self.bias is not None:
             x = x + self.bias[indices, ...]
 
         return x
 
 
 class FactorizedSpectralConv3d(FactorizedSpectralConv):
-    def __init__(
-        self, in_channels, out_channels, 
-        modes_height, modes_width, modes_depth, 
-        n_layers=1, scale='auto', separable=False,
-        fft_norm='backward', bias=True, implementation='reconstucted',
-         joint_factorization=False, rank=0.5, factorization='cp',
-          fixed_rank_modes=False, decomposition_kwargs=dict()):
-        super().__init__(in_channels, out_channels, (modes_height, modes_width, modes_depth),            
-            n_layers=n_layers, scale=scale, separable=separable,
-            fft_norm=fft_norm, bias=bias, implementation=implementation,
-            joint_factorization=joint_factorization, rank=rank, 
-            factorization=factorization, fixed_rank_modes=fixed_rank_modes,
-            decomposition_kwargs=decomposition_kwargs
-            )
-        self.half_modes_height, self.half_modes_width, self.half_modes_depth = self.half_modes
-
     def forward(self, x, indices=0):
         batchsize, channels, height, width, depth = x.shape
 
         x = torch.fft.rfftn(x.float(), norm=self.fft_norm, dim=[-3, -2, -1])
 
         out_fft = torch.zeros([batchsize, self.out_channels, height, width, depth//2 + 1], device=x.device, dtype=torch.cfloat)
 
-        out_fft[:, :, :self.half_modes_height, :self.half_modes_width, :self.half_modes_depth] = self._contract(
-            x[:, :, :self.half_modes_height, :self.half_modes_width, :self.half_modes_depth], self.weight[indices + 0], separable=self.separable)
-        out_fft[:, :, :self.half_modes_height, -self.half_modes_width:, :self.half_modes_depth] = self._contract(
-            x[:, :, :self.half_modes_height, -self.half_modes_width:, :self.half_modes_depth], self.weight[indices + 1], separable=self.separable)
-        out_fft[:, :, -self.half_modes_height:, :self.half_modes_width, :self.half_modes_depth] = self._contract(
-            x[:, :, -self.half_modes_height:, :self.half_modes_width, :self.half_modes_depth], self.weight[indices + 2], separable=self.separable)
-        out_fft[:, :, -self.half_modes_height:, -self.half_modes_width:, :self.half_modes_depth] = self._contract(
-            x[:, :, -self.half_modes_height:, -self.half_modes_width:, :self.half_modes_depth], self.weight[indices + 3], separable=self.separable)
+        out_fft[:, :, :self.half_n_modes[0], :self.half_n_modes[1], :self.half_n_modes[2]] = self._contract(
+            x[:, :, :self.half_n_modes[0], :self.half_n_modes[1], :self.half_n_modes[2]], self._get_weight(4*indices + 0), separable=self.separable)
+        out_fft[:, :, :self.half_n_modes[0], -self.half_n_modes[1]:, :self.half_n_modes[2]] = self._contract(
+            x[:, :, :self.half_n_modes[0], -self.half_n_modes[1]:, :self.half_n_modes[2]], self._get_weight(4*indices + 1), separable=self.separable)
+        out_fft[:, :, -self.half_n_modes[0]:, :self.half_n_modes[1], :self.half_n_modes[2]] = self._contract(
+            x[:, :, -self.half_n_modes[0]:, :self.half_n_modes[1], :self.half_n_modes[2]], self._get_weight(4*indices + 2), separable=self.separable)
+        out_fft[:, :, -self.half_n_modes[0]:, -self.half_n_modes[1]:, :self.half_n_modes[2]] = self._contract(
+            x[:, :, -self.half_n_modes[0]:, -self.half_n_modes[1]:, :self.half_n_modes[2]], self._get_weight(4*indices + 3), separable=self.separable)
+        
+        if self.output_scaling_factor is not None:
+            width = int(round(width*self.output_scaling_factor[0]))
+            height = int(round(height*self.output_scaling_factor[1]))
+            depth = int(round(depth*self.output_scaling_factor[2]))
 
         x = torch.fft.irfftn(out_fft, s=(height, width, depth), norm=self.fft_norm)
 
         if self.bias is not None:
             x = x + self.bias[indices, ...]
 
         return x
```

### Comparing `neuraloperator-0.1.1/neuralop/models/fourier_continuation.py` & `neuraloperator-0.2.0/neuralop/models/fourier_continuation.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/models/mlp.py` & `neuraloperator-0.2.0/neuralop/models/mlp.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/models/model_dispatcher.py` & `neuraloperator-0.2.0/neuralop/models/model_dispatcher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,30 @@
-from .tfno import TFNO2d
+from .tfno import TFNO, TFNO1d, TFNO2d, TFNO3d
+from .tfno import FNO, FNO1d, FNO2d, FNO3d
+from .uno import UNO
 import inspect
-import warnings
+
+
+MODEL_ZOO = {
+    'tfno'   : TFNO,
+    'tfno1d' : TFNO1d,
+    'tfno2d' : TFNO2d,
+    'tfno3d' : TFNO3d,
+    'fno'    : FNO,
+    'fno1d'  : FNO1d,
+    'fno2d'  : FNO2d,
+    'fno3d'  : FNO3d,
+    'uno'    : UNO,
+}
+
+
+def available_models():
+    """List the available neural operators
+    """
+    return list(MODEL_ZOO.keys())
 
 
 def get_model(config):
     """Returns an instantiated model for the given config
 
     Also prints warnings for safety, in case::
     * some given arguments aren't actually used by the model
@@ -18,33 +38,32 @@
         and the corresponding config[arch] (a subdict with the kwargs of the model)
 
     Returns
     -------
     model : nn.Module
         the instanciated module
     """
-    models = {'tfno2d': TFNO2d}
     arch = config['arch'].lower()
     config_arch = config.get(arch)
 
     # Set the number of input channels depending on channels in data + mg patching
     data_channels = config_arch.pop('data_channels')
     try:
         patching_levels = config['patching']['levels']
     except KeyError:
         patching_levels = 0
     if patching_levels:
-        data_channels *= 2**patching_levels
+        data_channels *= (patching_levels + 1)
     config_arch['in_channels'] = data_channels
 
     # Dispatch model creation
     try:
-        return dispatch_model(models[arch], config_arch)
+        return dispatch_model(MODEL_ZOO[arch], config_arch)
     except KeyError:
-        raise ValueError(f'Got config.{arch=}, expected one of {models.keys}.')
+        raise ValueError(f'Got config.{arch=}, expected one of {MODEL_ZOO.keys}.')
 
 
 def dispatch_model(ModelClass, config):
     """This function just creates an instance of the model ModelClass(**config)
     but performs additional checks to warn users about missing/wrong arguments.
     
     Parameters
```

### Comparing `neuraloperator-0.1.1/neuralop/models/padding.py` & `neuraloperator-0.2.0/neuralop/models/padding.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,18 +12,19 @@
         whether to pad on both sides, by default 'one-sided'
 
     Notes
     -----
     This class works for any input resolution, as long as it is in the form
     `(batch-size, channels, d1, ...., dN)`
     """
-    def __init__(self, domain_padding, padding_mode='one-sided'):
+    def __init__(self, domain_padding, padding_mode='one-sided', output_scale_factor = None):
         super().__init__()
         self.domain_padding = domain_padding
         self.padding_mode = padding_mode.lower()
+        self.output_scale_factor = output_scale_factor
         
         # dict(f'{resolution}'=padding) such that padded = F.pad(x, indices)
         self._padding = dict()
         
         # dict(f'{resolution}'=indices_to_unpad) such that unpadded = x[indices]
         self._unpad_indices = dict()
 
@@ -36,41 +37,59 @@
         
         The amount of padding will be automatically scaled with the resolution
         """
         resolution = x.shape[2:]
 
         if isinstance(self.domain_padding, (float, int)):
             self.domain_padding = [float(self.domain_padding)]*len(resolution)
+        if self.output_scale_factor is None:
+            self.output_scale_factor = [1]*len(resolution)
+        elif isinstance(self.output_scale_factor, (float, int)):
+            self.output_scale_factor = [float(self.output_scale_factor)]*len(resolution)
 
         try:
             padding = self._padding[f'{resolution}']
             return F.pad(x, padding, mode='constant')
 
         except KeyError:
             padding = [int(round(p*r)) for (p, r) in zip(self.domain_padding, resolution)]
             
             print(f'Padding inputs of {resolution=} with {padding=}, {self.padding_mode}')
 
+            output_pad = padding
+
+            for scale_factor in self.output_scale_factor:
+                if isinstance(scale_factor, (float, int)):
+                    scale_factor = [scale_factor]*len(resolution)
+                output_pad = [int(round(i*j)) for (i,j) in zip(scale_factor,output_pad)]
+
             if self.padding_mode == 'symmetric':
                 # Pad both sides
-                unpad_indices = (Ellipsis, ) + tuple([slice(p, -p, None) for p in padding])
+                unpad_indices = (Ellipsis, ) + tuple([slice(p, -p, None) for p in output_pad ])
                 padding = [i for p in padding for i in (p, p)]
 
             elif self.padding_mode == 'one-sided':
                 # One-side padding
-                unpad_indices = (Ellipsis, ) + tuple([slice(None, -p, None) for p in padding])
+                unpad_indices = (Ellipsis, ) + tuple([slice(None, -p, None) for p in output_pad])
                 padding = [i for p in padding for i in (0, p)]
             else:
                 raise ValueError(f'Got {self.padding_mode=}')
             
             self._padding[f'{resolution}'] = padding
 
             padded = F.pad(x, padding, mode='constant')
-            self._unpad_indices[f'{padded.shape[2:]}'] = unpad_indices
+
+            out_put_shape = padded.shape[2:]
+            for scale_factor in self.output_scale_factor:
+                if isinstance(scale_factor, (float, int)):
+                    scale_factor = [scale_factor]*len(resolution)
+                out_put_shape = [int(round(i*j)) for (i,j) in zip(scale_factor,out_put_shape)]
+            
+            self._unpad_indices[f'{[i for i in out_put_shape]}'] = unpad_indices
+
             return padded
 
     def unpad(self, x):
         """Remove the padding from padding inputs
         """
-        unpad_indices = self._unpad_indices[f'{x.shape[2:]}']
-
+        unpad_indices = self._unpad_indices[f'{list(x.shape[2:])}']
         return x[unpad_indices]
```

### Comparing `neuraloperator-0.1.1/neuralop/models/skip_connections.py` & `neuraloperator-0.2.0/neuralop/models/skip_connections.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,42 +32,44 @@
     elif type.lower() == 'identity':
         return nn.Identity()
     else:
         raise ValueError(f"Got skip-connection {type=}, expected one of {'soft-gating', 'linear', 'id'}.")
 
 
 class SoftGating(nn.Module):
-    def __init__(self, in_features, out_features=None, n_dim=2, bias=False):
-        """Applies soft-gating by weighting the channels of the given input
+    """Applies soft-gating by weighting the channels of the given input
 
-        Given an input x of size `(batch-size, channels, height, width)`,
-        this returns `x * w `
-        where w is of shape `(1, channels, 1, 1)`
-
-        Parameters
-        ----------
-        in_features : int
-        out_features : None
-            this is provided for API compatibility with nn.Linear only
-        n_dim : int, default is 2
-            Dimensionality of the input (excluding batch-size and channels).
-            ``n_dim=2`` corresponds to having Module2D. 
-        bias : bool, default is False
-        """
+    Given an input x of size `(batch-size, channels, height, width)`,
+    this returns `x * w `
+    where w is of shape `(1, channels, 1, 1)`
+
+    Parameters
+    ----------
+    in_features : int
+    out_features : None
+        this is provided for API compatibility with nn.Linear only
+    n_dim : int, default is 2
+        Dimensionality of the input (excluding batch-size and channels).
+        ``n_dim=2`` corresponds to having Module2D. 
+    bias : bool, default is False
+    """
+    def __init__(self, in_features, out_features=None, n_dim=2, bias=False):
         super().__init__()
         if out_features is not None and in_features != out_features:
             raise ValueError(f"Got {in_features=} and {out_features=}"
                              "but these two must be the same for soft-gating")
         self.in_features = in_features
         self.out_features = out_features
         self.weight = nn.Parameter(torch.ones(1, self.in_features, *(1,)*n_dim))
         if bias:
             self.bias = nn.Parameter(torch.ones(1, self.in_features, *(1,)*n_dim))
         else:
             self.bias = None
 
     def forward(self, x):
+        """Applies soft-gating to a batch of activations
+        """
         if self.bias is not None:
             return self.weight*x + self.bias
         else:
             return self.weight*x
```

### Comparing `neuraloperator-0.1.1/neuralop/models/tests/test_tfno.py` & `neuraloperator-0.2.0/neuralop/models/tests/test_tfno.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,27 +32,34 @@
 
         use_mlp = True
         mlp = Bunch(dict(expansion=0.5, dropout=0))
 
     rank = 0.2
     size = (s, )*n_dim
     m_modes = (modes,)*n_dim
-    model = TFNO(hidden_channels=width, n_modes=m_modes, 
-                            factorization=factorization,
-                            implementation=implementation,
-                            rank=rank,
-                            fixed_rank_modes=False,
-                            joint_factorization=False,
-                            n_layers=n_layers,
-                            use_mlp=use_mlp, mlp=mlp,
-                            fc_channels=fc_channels).to(device)
+    model = TFNO(hidden_channels=width, n_modes=m_modes,
+                 factorization=factorization,
+                 implementation=implementation,
+                 rank=rank,
+                 fixed_rank_modes=False,
+                 joint_factorization=False,
+                 n_layers=n_layers,
+                 use_mlp=use_mlp, mlp=mlp,
+                 fc_channels=fc_channels).to(device)
     in_data = torch.randn(batch_size, 3, *size).to(device)
 
     # Test forward pass
     out = model(in_data)
 
     # Check output size
     assert list(out.shape) == [batch_size, 1, *size]
 
     # Check backward pass
     loss = out.sum()
     loss.backward()
+
+    n_unused_params = 0
+    for param in model.parameters():
+        if param.grad is None:
+            n_unused_params += 1
+    assert n_unused_params == 0, f'{n_unused_params} parameters were unused!'
+
```

### Comparing `neuraloperator-0.1.1/neuralop/models/tfno.py` & `neuraloperator-0.2.0/neuralop/models/tfno.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import torch.nn as nn
 import torch.nn.functional as F
-from .mlp import MLP
-
-from .fno_block import FactorizedSpectralConv3d, FactorizedSpectralConv2d, FactorizedSpectralConv1d
-from .fno_block import FactorizedSpectralConv
-from .skip_connections import skip_connection
+from functools import partialmethod
+import torch
+from .spectral_convolution import FactorizedSpectralConv
 from .padding import DomainPadding
+from .fno_block import FNOBlocks, resample
 
 
 class Lifting(nn.Module):
     def __init__(self, in_channels, out_channels, n_dim=2):
         super().__init__()
         self.in_channels = in_channels
         self.out_channels = out_channels
@@ -34,16 +33,17 @@
     def forward(self, x):
         x = self.fc1(x)
         x = self.non_linearity(x)
         x = self.fc2(x)
         return x
 
 
-class TFNO(nn.Module):
-    """Generic N-D Tensorized Fourier Neural Operator
+
+class FNO(nn.Module):
+    """N-Dimensional Fourier Neural Operator
 
     Parameters
     ----------
     n_modes : int tuple
         number of modes to keep in Fourier Layer, along each dimension
         The dimensionality of the TFNO is inferred from ``len(n_modes)``
     hidden_channels : int
@@ -54,14 +54,21 @@
         Number of output channels, by default 1
     lifting_channels : int, optional
         number of hidden channels of the lifting block of the FNO, by default 256
     projection_channels : int, optional
         number of hidden channels of the projection block of the FNO, by default 256
     n_layers : int, optional
         Number of Fourier Layers, by default 4
+    incremental_n_modes : None or int tuple, default is None
+        * If not None, this allows to incrementally increase the number of modes in Fourier domain 
+          during training. Has to verify n <= N for (n, m) in zip(incremental_n_modes, n_modes).
+        
+        * If None, all the n_modes are used.
+
+        This can be updated dynamically during training.
     use_mlp : bool, optional
         Whether to use an MLP layer after each FNO block, by default False
     mlp : dict, optional
         Parameters of the MLP, by default None
         {'expansion': float, 'dropout': float}
     non_linearity : nn.Module, optional
         Non-Linearity module to use, by default F.gelu
@@ -69,15 +76,15 @@
         Normalization layer to use, by default None
     preactivation : bool, default is False
         if True, use resnet-style preactivation
     skip : {'linear', 'identity', 'soft-gating'}, optional
         Type of skip connection to use, by default 'soft-gating'
     separable : bool, default is False
         if True, use a depthwise separable spectral convolution
-    factorization : str or None, {'tucker', 'cp', 'tt'}, default is None
+    factorization : str or None, {'tucker', 'cp', 'tt'}
         Tensor factorization of the parameters weight to use, by default None.
         * If None, a dense tensor parametrizes the Spectral convolutions
         * Otherwise, the specified tensor factorization is used.
     joint_factorization : bool, optional
         Whether all the Fourier Layers should be parametrized by a single tensor (vs one per layer), by default False
     rank : float or rank, optional
         Rank of the tensor factorization of the Fourier weights, by default 1.0
@@ -98,28 +105,31 @@
     """
     def __init__(self, n_modes, hidden_channels,
                  in_channels=3, 
                  out_channels=1,
                  lifting_channels=256,
                  projection_channels=256,
                  n_layers=4,
+                 incremental_n_modes=None,
                  use_mlp=False, mlp=None,
                  non_linearity=F.gelu,
                  norm=None, preactivation=False,
-                 skip='soft-gating',
+                 fno_skip='linear',
+                 mlp_skip='soft-gating',
                  separable=False,
-                 factorization='tucker', 
+                 factorization=None,
                  rank=1.0,
                  joint_factorization=False, 
                  fixed_rank_modes=False,
                  implementation='factorized',
                  decomposition_kwargs=dict(),
                  domain_padding=None,
                  domain_padding_mode='one-sided',
                  fft_norm='forward',
+                 SpectralConv=FactorizedSpectralConv,
                  **kwargs):
         super().__init__()
         self.n_dim = len(n_modes)
         self.n_modes = n_modes
         self.hidden_channels = hidden_channels
         self.lifting_channels = lifting_channels
         self.projection_channels = projection_channels
@@ -128,116 +138,85 @@
         self.n_layers = n_layers
         self.joint_factorization = joint_factorization
         self.non_linearity = non_linearity
         self.rank = rank
         self.factorization = factorization
         self.fixed_rank_modes = fixed_rank_modes
         self.decomposition_kwargs = decomposition_kwargs
-        self.skip = skip,
+        self.fno_skip = fno_skip,
+        self.mlp_skip = mlp_skip,
         self.fft_norm = fft_norm
         self.implementation = implementation
         self.separable = separable
         self.preactivation = preactivation
 
+        # See the class' property for underlying mechanism
+        # When updated, change should be reflected in fno blocks
+        self._incremental_n_modes = incremental_n_modes
+
         if domain_padding is not None and domain_padding > 0:
             self.domain_padding = DomainPadding(domain_padding=domain_padding, padding_mode=domain_padding_mode)
         else:
             self.domain_padding = None
         self.domain_padding_mode = domain_padding_mode
 
-        self.convs = FactorizedSpectralConv(
-            self.hidden_channels, self.hidden_channels, self.n_modes, 
+        self.fno_blocks = FNOBlocks(
+            in_channels=hidden_channels,
+            out_channels=hidden_channels, 
+            n_modes=self.n_modes,
+            use_mlp=use_mlp, mlp=mlp,
+            non_linearity=non_linearity,
+            norm=norm, preactivation=preactivation,
+            fno_skip=fno_skip,
+            mlp_skip=mlp_skip,
+            incremental_n_modes=incremental_n_modes,
             rank=rank,
             fft_norm=fft_norm,
             fixed_rank_modes=fixed_rank_modes, 
             implementation=implementation,
             separable=separable,
             factorization=factorization,
             decomposition_kwargs=decomposition_kwargs,
             joint_factorization=joint_factorization,
-            n_layers=n_layers,
-        )
-
-        self.fno_skips = nn.ModuleList([skip_connection(self.hidden_channels, self.hidden_channels, type=skip, n_dim=self.n_dim) for _ in range(n_layers)])
-
-        if use_mlp:
-            self.mlp = nn.ModuleList(
-                [MLP(in_channels=self.hidden_channels, hidden_channels=int(round(self.hidden_channels*mlp['expansion'])),
-                     dropout=mlp['dropout'], n_dim=self.n_dim) for _ in range(n_layers)]
-            )
-            self.mlp_skips = nn.ModuleList([skip_connection(self.hidden_channels, self.hidden_channels, type=skip, n_dim=self.n_dim) for _ in range(n_layers)])
-        else:
-            self.mlp = None
-
-        if norm is None:
-            self.norm = None
-        elif norm == 'instance_norm':
-            self.norm = nn.ModuleList([getattr(nn, f'InstanceNorm{self.n_dim}d')(num_features=self.hidden_channels) for _ in range(n_layers)])
-        elif norm == 'group_norm':
-            self.norm = nn.ModuleList([nn.GroupNorm(num_groups=1, num_channels=self.hidden_channels) for _ in range(n_layers)])
-        elif norm == 'layer_norm':
-            self.norm = nn.ModuleList([nn.LayerNorm() for _ in range(n_layers)])
-        else:
-            raise ValueError(f'Got {norm=} but expected None or one of [instance_norm, group_norm, layer_norm]')
+            SpectralConv=SpectralConv,
+            n_layers=n_layers)
 
         self.lifting = Lifting(in_channels=in_channels, out_channels=self.hidden_channels, n_dim=self.n_dim)
         self.projection = Projection(in_channels=self.hidden_channels, out_channels=out_channels, hidden_channels=projection_channels,
                                      non_linearity=non_linearity, n_dim=self.n_dim)
 
-
     def forward(self, x):
         """TFNO's forward pass
         """
         x = self.lifting(x)
 
         if self.domain_padding is not None:
             x = self.domain_padding.pad(x)
 
-        for i in range(self.n_layers):
-
-            if self.preactivation:
-                x = self.non_linearity(x)
-
-                if self.norm is not None:
-                    x = self.norm[i](x)
-
-            x_fno = self.convs[i](x)
-
-            if not self.preactivation and self.norm is not None:
-                x_fno = self.norm[i](x_fno)
-
-            x_skip = self.fno_skips[i](x)
-            x = x_fno + x_skip
-
-            if not self.preactivation and i < (self.n_layers - 1):
-                x = self.non_linearity(x)
-
-            if self.mlp is not None:
-                x_skip = self.mlp_skips[i](x)
-
-                if self.preactivation:
-                    if i < (self.n_layers - 1):
-                        x = self.non_linearity(x)
-
-                x = self.mlp[i](x) + x_skip
-
-                if not self.preactivation:
-                    if i < (self.n_layers - 1):
-                        x = self.non_linearity(x)
-
+        for layer_idx in range(self.n_layers):
+            x = self.fno_blocks(x, layer_idx)
 
         if self.domain_padding is not None:
             x = self.domain_padding.unpad(x)
 
         x = self.projection(x)
+
         return x
 
+    @property
+    def incremental_n_modes(self):
+        return self._incremental_n_modes
+
+    @incremental_n_modes.setter
+    def incremental_n_modes(self, incremental_n_modes):
+        self.fno_blocks.incremental_n_modes = incremental_n_modes
 
-class TFNO1d(TFNO):
-    """Generic 1D Fourier Neural Operator
+
+class FNO1d(FNO):
+    """1D Fourier Neural Operator
 
     Parameters
     ----------
     modes_height : int
         number of Fourier modes to keep along the height
     hidden_channels : int
         width of the FNO (i.e. number of channels)
@@ -247,14 +226,21 @@
         Number of output channels, by default 1
     lifting_channels : int, optional
         number of hidden channels of the lifting block of the FNO, by default 256
     projection_channels : int, optional
         number of hidden channels of the projection block of the FNO, by default 256
     n_layers : int, optional
         Number of Fourier Layers, by default 4
+    incremental_n_modes : None or int tuple, default is None
+        * If not None, this allows to incrementally increase the number of modes in Fourier domain 
+          during training. Has to verify n <= N for (n, m) in zip(incremental_n_modes, n_modes).
+        
+        * If None, all the n_modes are used.
+
+        This can be updated dynamically during training.
     use_mlp : bool, optional
         Whether to use an MLP layer after each FNO block, by default False
     mlp : dict, optional
         Parameters of the MLP, by default None
         {'expansion': float, 'dropout': float}
     non_linearity : nn.Module, optional
         Non-Linearity module to use, by default F.gelu
@@ -262,15 +248,15 @@
         Normalization layer to use, by default None
     preactivation : bool, default is False
         if True, use resnet-style preactivation
     skip : {'linear', 'identity', 'soft-gating'}, optional
         Type of skip connection to use, by default 'soft-gating'
     separable : bool, default is False
         if True, use a depthwise separable spectral convolution
-    factorization : str or None, {'tucker', 'cp', 'tt'}, default is None
+    factorization : str or None, {'tucker', 'cp', 'tt'}
         Tensor factorization of the parameters weight to use, by default None.
         * If None, a dense tensor parametrizes the Spectral convolutions
         * Otherwise, the specified tensor factorization is used.
     joint_factorization : bool, optional
         Whether all the Fourier Layers should be parametrized by a single tensor (vs one per layer), by default False
     rank : float or rank, optional
         Rank of the tensor factorization of the Fourier weights, by default 1.0
@@ -293,22 +279,23 @@
         self,
         n_modes_height,
         hidden_channels,
         in_channels=3, 
         out_channels=1,
         lifting_channels=256,
         projection_channels=256,
+        incremental_n_modes=None,
         n_layers=4,
         non_linearity=F.gelu,
         use_mlp=False, mlp=None,
         norm=None,
         skip='soft-gating',
         separable=False,
         preactivation=False,
-        factorization='tucker', 
+        factorization=None, 
         rank=1.0,
         joint_factorization=False, 
         fixed_rank_modes=False,
         implementation='factorized',
         decomposition_kwargs=dict(),
         domain_padding=None,
         domain_padding_mode='one-sided',
@@ -320,14 +307,15 @@
             in_channels=in_channels, 
             out_channels=out_channels,
             lifting_channels=lifting_channels,
             projection_channels=projection_channels,
             n_layers=n_layers,
             non_linearity=non_linearity,
             use_mlp=use_mlp, mlp=mlp,
+            incremental_n_modes=incremental_n_modes,
             norm=norm,
             skip=skip,
             separable=separable,
             preactivation=preactivation,
             factorization=factorization, 
             rank=rank,
             joint_factorization=joint_factorization, 
@@ -336,30 +324,17 @@
             decomposition_kwargs=decomposition_kwargs,
             domain_padding=domain_padding,
             domain_padding_mode=domain_padding_mode,
             fft_norm=fft_norm
             )
         self.n_modes_height = n_modes_height
 
-        self.convs = FactorizedSpectralConv1d(
-            self.hidden_channels, self.hidden_channels, self.n_modes_height, 
-            rank=rank,
-            fft_norm=fft_norm,
-            fixed_rank_modes=fixed_rank_modes, 
-            implementation=implementation,
-            separable=separable,
-            factorization=factorization,
-            decomposition_kwargs=decomposition_kwargs,
-            joint_factorization=joint_factorization,
-            n_layers=n_layers,
-        )
-
 
-class TFNO2d(TFNO):
-    """Generic 2D Fourier Neural Operator
+class FNO2d(FNO):
+    """2D Fourier Neural Operator
 
     Parameters
     ----------
     n_modes_width : int
         number of modes to keep in Fourier Layer, along the width
     n_modes_height : int
         number of Fourier modes to keep along the height
@@ -371,14 +346,21 @@
         Number of output channels, by default 1
     lifting_channels : int, optional
         number of hidden channels of the lifting block of the FNO, by default 256
     projection_channels : int, optional
         number of hidden channels of the projection block of the FNO, by default 256
     n_layers : int, optional
         Number of Fourier Layers, by default 4
+    incremental_n_modes : None or int tuple, default is None
+        * If not None, this allows to incrementally increase the number of modes in Fourier domain 
+          during training. Has to verify n <= N for (n, m) in zip(incremental_n_modes, n_modes).
+        
+        * If None, all the n_modes are used.
+
+        This can be updated dynamically during training.
     use_mlp : bool, optional
         Whether to use an MLP layer after each FNO block, by default False
     mlp : dict, optional
         Parameters of the MLP, by default None
         {'expansion': float, 'dropout': float}
     non_linearity : nn.Module, optional
         Non-Linearity module to use, by default F.gelu
@@ -386,15 +368,15 @@
         Normalization layer to use, by default None
     preactivation : bool, default is False
         if True, use resnet-style preactivation
     skip : {'linear', 'identity', 'soft-gating'}, optional
         Type of skip connection to use, by default 'soft-gating'
     separable : bool, default is False
         if True, use a depthwise separable spectral convolution
-    factorization : str or None, {'tucker', 'cp', 'tt'}, default is None
+    factorization : str or None, {'tucker', 'cp', 'tt'}
         Tensor factorization of the parameters weight to use, by default None.
         * If None, a dense tensor parametrizes the Spectral convolutions
         * Otherwise, the specified tensor factorization is used.
     joint_factorization : bool, optional
         Whether all the Fourier Layers should be parametrized by a single tensor (vs one per layer), by default False
     rank : float or rank, optional
         Rank of the tensor factorization of the Fourier weights, by default 1.0
@@ -419,21 +401,22 @@
         n_modes_width,
         hidden_channels,
         in_channels=3, 
         out_channels=1,
         lifting_channels=256,
         projection_channels=256,
         n_layers=4,
+        incremental_n_modes=None,
         non_linearity=F.gelu,
         use_mlp=False, mlp=None,
         norm=None,
         skip='soft-gating',
         separable=False,
         preactivation=False,
-        factorization='tucker', 
+        factorization=None, 
         rank=1.0,
         joint_factorization=False, 
         fixed_rank_modes=False,
         implementation='factorized',
         decomposition_kwargs=dict(),
         domain_padding=None,
         domain_padding_mode='one-sided',
@@ -445,14 +428,15 @@
             in_channels=in_channels, 
             out_channels=out_channels,
             lifting_channels=lifting_channels,
             projection_channels=projection_channels,
             n_layers=n_layers,
             non_linearity=non_linearity,
             use_mlp=use_mlp, mlp=mlp,
+            incremental_n_modes=incremental_n_modes,
             norm=norm,
             skip=skip,
             separable=separable,
             preactivation=preactivation,
             factorization=factorization, 
             rank=rank,
             joint_factorization=joint_factorization, 
@@ -462,31 +446,18 @@
             domain_padding=domain_padding,
             domain_padding_mode=domain_padding_mode,
             fft_norm=fft_norm
             )
         self.n_modes_height = n_modes_height
         self.n_modes_width = n_modes_width
 
-        self.convs = FactorizedSpectralConv2d(
-            self.hidden_channels, self.hidden_channels,
-            self.n_modes_height, self.n_modes_width, 
-            rank=rank,
-            fft_norm=fft_norm,
-            fixed_rank_modes=fixed_rank_modes, 
-            implementation=implementation,
-            separable=separable,
-            factorization=factorization,
-            decomposition_kwargs=decomposition_kwargs,
-            joint_factorization=joint_factorization,
-            n_layers=n_layers,
-        )
 
 
-class TFNO3d(TFNO):
-    """Generic 3D Fourier Neural Operator
+class FNO3d(FNO):
+    """3D Fourier Neural Operator
 
     Parameters
     ----------
     modes_width : int
         number of modes to keep in Fourier Layer, along the width
     modes_height : int
         number of Fourier modes to keep along the height    
@@ -500,14 +471,21 @@
         Number of output channels, by default 1
     lifting_channels : int, optional
         number of hidden channels of the lifting block of the FNO, by default 256
     projection_channels : int, optional
         number of hidden channels of the projection block of the FNO, by default 256
     n_layers : int, optional
         Number of Fourier Layers, by default 4
+    incremental_n_modes : None or int tuple, default is None
+        * If not None, this allows to incrementally increase the number of modes in Fourier domain 
+          during training. Has to verify n <= N for (n, m) in zip(incremental_n_modes, n_modes).
+        
+        * If None, all the n_modes are used.
+
+        This can be updated dynamically during training.
     use_mlp : bool, optional
         Whether to use an MLP layer after each FNO block, by default False
     mlp : dict, optional
         Parameters of the MLP, by default None
         {'expansion': float, 'dropout': float}
     non_linearity : nn.Module, optional
         Non-Linearity module to use, by default F.gelu
@@ -515,15 +493,15 @@
         Normalization layer to use, by default None
     preactivation : bool, default is False
         if True, use resnet-style preactivation
     skip : {'linear', 'identity', 'soft-gating'}, optional
         Type of skip connection to use, by default 'soft-gating'
     separable : bool, default is False
         if True, use a depthwise separable spectral convolution
-    factorization : str or None, {'tucker', 'cp', 'tt'}, default is None
+    factorization : str or None, {'tucker', 'cp', 'tt'}
         Tensor factorization of the parameters weight to use, by default None.
         * If None, a dense tensor parametrizes the Spectral convolutions
         * Otherwise, the specified tensor factorization is used.
     joint_factorization : bool, optional
         Whether all the Fourier Layers should be parametrized by a single tensor (vs one per layer), by default False
     rank : float or rank, optional
         Rank of the tensor factorization of the Fourier weights, by default 1.0
@@ -548,21 +526,22 @@
         n_modes_depth,
         hidden_channels,
         in_channels=3, 
         out_channels=1,
         lifting_channels=256,
         projection_channels=256,
         n_layers=4,
+        incremental_n_modes=None,
         non_linearity=F.gelu,
         use_mlp=False, mlp=None,
         norm=None,
         skip='soft-gating',
         separable=False,
         preactivation=False,
-        factorization='tucker', 
+        factorization=None, 
         rank=1.0,
         joint_factorization=False, 
         fixed_rank_modes=False,
         implementation='factorized',
         decomposition_kwargs=dict(),
         domain_padding=None,
         domain_padding_mode='one-sided',
@@ -573,14 +552,15 @@
             hidden_channels=hidden_channels,
             in_channels=in_channels, 
             out_channels=out_channels,
             lifting_channels=lifting_channels,
             projection_channels=projection_channels,
             n_layers=n_layers,
             non_linearity=non_linearity,
+            incremental_n_modes=incremental_n_modes,
             use_mlp=use_mlp, mlp=mlp,
             norm=norm,
             skip=skip,
             separable=separable,
             preactivation=preactivation,
             factorization=factorization, 
             rank=rank,
@@ -592,21 +572,37 @@
             domain_padding_mode=domain_padding_mode,
             fft_norm=fft_norm
             )
         self.n_modes_height = n_modes_height
         self.n_modes_width = n_modes_width
         self.n_modes_height = n_modes_height
 
-        self.convs = FactorizedSpectralConv3d(
-            self.hidden_channels, self.hidden_channels, 
-            self.n_modes_height, self.n_modes_width, self.n_modes_height,
-            rank=rank,
-            fft_norm=fft_norm,
-            fixed_rank_modes=fixed_rank_modes, 
-            implementation=implementation,
-            separable=separable,
-            factorization=factorization,
-            decomposition_kwargs=decomposition_kwargs,
-            joint_factorization=joint_factorization,
-            n_layers=n_layers,
-        )
 
+def partialclass(new_name, cls, *args, **kwargs):
+    """Create a new class with different default values
+
+    Notes
+    -----
+    An obvious alternative would be to use functools.partial
+    >>> new_class = partial(cls, **kwargs)
+
+    The issue is twofold:
+    1. the class doesn't have a name, so one would have to set it explicitly:
+    >>> new_class.__name__ = new_name
+
+    2. the new class will be a functools object and one cannot inherit from it.
+
+    Instead, here, we define dynamically a new class, inheriting from the existing one.
+    """
+    __init__ = partialmethod(cls.__init__, *args, **kwargs)
+    new_class = type(new_name, (cls,),  {
+        '__init__': __init__,
+        '__doc__': cls.__doc__,
+        'forward': cls.forward, 
+    })
+    return new_class
+
+
+TFNO   = partialclass('TFNO', FNO, factorization='Tucker')
+TFNO1d = partialclass('TFNO1d', FNO1d, factorization='Tucker')
+TFNO2d = partialclass('TFNO2d', FNO2d, factorization='Tucker')
+TFNO3d = partialclass('TFNO3d', FNO3d, factorization='Tucker')
```

### Comparing `neuraloperator-0.1.1/neuralop/mpu/comm.py` & `neuraloperator-0.2.0/neuralop/mpu/comm.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/mpu/helpers.py` & `neuraloperator-0.2.0/neuralop/mpu/helpers.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/mpu/mappings.py` & `neuraloperator-0.2.0/neuralop/mpu/mappings.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/tests/test_model_from_config.py` & `neuraloperator-0.2.0/neuralop/tests/test_model_from_config.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/training/losses.py` & `neuraloperator-0.2.0/neuralop/training/losses.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/training/patching.py` & `neuraloperator-0.2.0/neuralop/training/patching.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/training/torch_setup.py` & `neuraloperator-0.2.0/neuralop/training/torch_setup.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuralop/training/trainer.py` & `neuraloperator-0.2.0/neuralop/training/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,34 +95,45 @@
         
         for epoch in range(self.n_epochs):
             avg_loss = 0
             avg_lasso_loss = 0
             model.train()
             t1 = default_timer()
             train_err = 0.0
-            for sample in train_loader:
+
+            for idx, sample in enumerate(train_loader):
                 x, y = sample['x'], sample['y']
                 
+                if epoch == 0 and idx == 0 and self.verbose and is_logger:
+                    print(f'Training on raw inputs of size {x.shape=}, {y.shape=}')
+
                 x, y = self.patcher.patch(x, y)
+
+                if epoch == 0 and idx == 0 and self.verbose and is_logger:
+                    print(f'.. patched inputs of size {x.shape=}, {y.shape=}')
+
                 x = x.to(self.device)
                 y = y.to(self.device)
 
                 optimizer.zero_grad(set_to_none=True)
                 if regularizer:
                     regularizer.reset()
 
                 out = model(x)
-                
-                out, y = self.patcher.unpatch(out, y)
+                if epoch == 0 and idx == 0 and self.verbose and is_logger:
+                    print(f'Raw outputs of size {out.shape=}')
 
+                out, y = self.patcher.unpatch(out, y)
                 #Output encoding only works if output is stiched
                 if output_encoder is not None and self.mg_patching_stitching:
                     out = output_encoder.decode(out)
                     y = output_encoder.decode(y)
-                    
+                if epoch == 0 and idx == 0 and self.verbose and is_logger:
+                    print(f'.. Processed (unpatched) outputs of size {out.shape=}')
+
                 loss = training_loss(out.float(), y)
 
                 if regularizer:
                     loss += regularizer.loss
 
                 loss.backward()
```

### Comparing `neuraloperator-0.1.1/neuralop/utils.py` & `neuraloperator-0.2.0/neuralop/utils.py`

 * *Files identical despite different names*

### Comparing `neuraloperator-0.1.1/neuraloperator.egg-info/SOURCES.txt` & `neuraloperator-0.2.0/neuraloperator.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,39 @@
 neuralop/utils.py
 neuralop/datasets/__init__.py
 neuralop/datasets/burgers.py
 neuralop/datasets/darcy.py
 neuralop/datasets/hdf5_dataset.py
 neuralop/datasets/navier_stokes.py
 neuralop/datasets/positional_encoding.py
+neuralop/datasets/pt_dataset.py
 neuralop/datasets/tensor_dataset.py
 neuralop/datasets/transforms.py
 neuralop/datasets/zarr_dataset.py
+neuralop/datasets/data/darcy_test_16.pt
+neuralop/datasets/data/darcy_test_32.pt
+neuralop/datasets/data/darcy_train_16.pt
 neuralop/models/__init__.py
 neuralop/models/fno_block.py
 neuralop/models/fourier_continuation.py
 neuralop/models/mlp.py
 neuralop/models/model_dispatcher.py
 neuralop/models/padding.py
+neuralop/models/resample.py
 neuralop/models/skip_connections.py
+neuralop/models/spectral_convolution.py
 neuralop/models/tfno.py
+neuralop/models/uno.py
 neuralop/models/tests/__init__.py
 neuralop/models/tests/test_fno_block.py
 neuralop/models/tests/test_padding.py
+neuralop/models/tests/test_resample.py
+neuralop/models/tests/test_spectral_convolution.py
 neuralop/models/tests/test_tfno.py
+neuralop/models/tests/test_uno.py
 neuralop/mpu/__init__.py
 neuralop/mpu/comm.py
 neuralop/mpu/helpers.py
 neuralop/mpu/mappings.py
 neuralop/tests/__init__.py
 neuralop/tests/test_model_from_config.py
 neuralop/training/__init__.py
```

### Comparing `neuraloperator-0.1.1/setup.py` & `neuraloperator-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,16 @@
         {'name': "Nikola Kovachki", 'email': "nkovachki@caltech.edu"},
         {'name': "Zongyi Li", 'email': "zongyili@caltech.edu"}
         ],
     'version': VERSION,
     'install_requires': ['numpy', 'configmypy', 'pytest'],
     'license': 'Modified BSD',
     'scripts': [],
+    'include_package_data': True,
+    'package_data': {'': ['datasets/data/*.pt']},
     'classifiers': [
         'Topic :: Scientific/Engineering',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3'
     ],
 }
```

