# Comparing `tmp/qucumber-1.3.2.tar.gz` & `tmp/qucumber-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qucumber-1.3.2.tar", last modified: Tue Jan 12 01:22:12 2021, max compression
+gzip compressed data, was "/home/ejaaz/Documents/QuCumber/dist/.tmp-a7stkci4/qucumber-1.3.3.tar", last modified: Tue May  9 04:05:56 2023, max compression
```

## Comparing `qucumber-1.3.2.tar` & `qucumber-1.3.3.tar`

### file list

```diff
@@ -1,54 +1,64 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-12 01:22:12.000000 qucumber-1.3.2/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-12 01:22:12.000000 qucumber-1.3.2/qucumber/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-12 01:22:12.000000 qucumber-1.3.2/qucumber/rbm/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16923 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/rbm/purification_rbm.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     8555 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/rbm/binary_rbm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/rbm/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-12 01:22:12.000000 qucumber-1.3.2/qucumber/nn_states/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2791 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/nn_states/wavefunction.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     8742 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/nn_states/complex_wavefunction.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     8178 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/nn_states/positive_wavefunction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24756 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/nn_states/neural_state.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13299 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/nn_states/density_matrix.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      239 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/nn_states/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-12 01:22:12.000000 qucumber-1.3.2/qucumber/callbacks/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/callbacks/logger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5615 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/callbacks/early_stopping.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8013 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/callbacks/observable_evaluator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2121 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/callbacks/timer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3385 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/callbacks/model_saver.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3106 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/callbacks/variance_based_early_stopping.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3652 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/callbacks/lambda_callback.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2482 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/callbacks/callback.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4125 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/callbacks/liveplotting.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5510 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/callbacks/metric_evaluator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      459 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/callbacks/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2405 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/callbacks/callback_list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/__version__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-12 01:22:12.000000 qucumber-1.3.2/qucumber/observables/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3422 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/observables/entanglement.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6102 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/observables/pauli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6143 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/observables/system.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2390 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/observables/interactions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11516 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/observables/observable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1797 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/observables/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      219 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/observables/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-12 01:22:12.000000 qucumber-1.3.2/qucumber/utils/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    10932 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/utils/cplx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9986 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/utils/unitaries.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4609 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/utils/data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1862 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/utils/gradients_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8796 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/utils/training_statistics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2318 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1184 2021-01-12 01:21:28.000000 qucumber-1.3.2/qucumber/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7421 2021-01-12 01:22:12.000000 qucumber-1.3.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     5381 2021-01-12 01:21:28.000000 qucumber-1.3.2/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-01-12 01:22:12.000000 qucumber-1.3.2/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-12 01:22:12.000000 qucumber-1.3.2/qucumber.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7421 2021-01-12 01:22:11.000000 qucumber-1.3.2/qucumber.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-01-12 01:22:11.000000 qucumber-1.3.2/qucumber.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-01-12 01:22:11.000000 qucumber-1.3.2/qucumber.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-01-12 01:22:11.000000 qucumber-1.3.2/qucumber.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2021-01-12 01:22:11.000000 qucumber-1.3.2/qucumber.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1365 2021-01-12 01:22:11.000000 qucumber-1.3.2/qucumber.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3526 2021-01-12 01:21:28.000000 qucumber-1.3.2/setup.py
+drwxr-xr-x   0 ejaaz     (1000) ejaaz     (1000)        0 2023-05-09 04:05:56.000000 qucumber-1.3.3/
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)    16893 2023-05-08 23:55:08.000000 qucumber-1.3.3/LICENSE
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)      570 2023-05-08 23:55:08.000000 qucumber-1.3.3/LICENSE_HEADER
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     6657 2023-05-09 04:05:56.000000 qucumber-1.3.3/PKG-INFO
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     5381 2023-05-08 23:55:08.000000 qucumber-1.3.3/README.md
+drwxr-xr-x   0 ejaaz     (1000) ejaaz     (1000)        0 2023-05-09 04:05:56.000000 qucumber-1.3.3/qucumber/
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     1184 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/__init__.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)       22 2023-05-09 04:03:26.000000 qucumber-1.3.3/qucumber/__version__.py
+drwxr-xr-x   0 ejaaz     (1000) ejaaz     (1000)        0 2023-05-09 04:05:56.000000 qucumber-1.3.3/qucumber/callbacks/
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)      459 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/callbacks/__init__.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     2482 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/callbacks/callback.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     2405 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/callbacks/callback_list.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     5615 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/callbacks/early_stopping.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     3652 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/callbacks/lambda_callback.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     4125 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/callbacks/liveplotting.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     1964 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/callbacks/logger.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     5510 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/callbacks/metric_evaluator.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     3385 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/callbacks/model_saver.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     8013 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/callbacks/observable_evaluator.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     2121 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/callbacks/timer.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     3106 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/callbacks/variance_based_early_stopping.py
+drwxr-xr-x   0 ejaaz     (1000) ejaaz     (1000)        0 2023-05-09 04:05:56.000000 qucumber-1.3.3/qucumber/nn_states/
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)      239 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/nn_states/__init__.py
+-rwxr-xr-x   0 ejaaz     (1000) ejaaz     (1000)     8742 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/nn_states/complex_wavefunction.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)    13299 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/nn_states/density_matrix.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)    24756 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/nn_states/neural_state.py
+-rwxr-xr-x   0 ejaaz     (1000) ejaaz     (1000)     8178 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/nn_states/positive_wavefunction.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     2791 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/nn_states/wavefunction.py
+drwxr-xr-x   0 ejaaz     (1000) ejaaz     (1000)        0 2023-05-09 04:05:56.000000 qucumber-1.3.3/qucumber/observables/
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)      219 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/observables/__init__.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     3422 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/observables/entanglement.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     2390 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/observables/interactions.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)    11516 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/observables/observable.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     6102 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/observables/pauli.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     6143 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/observables/system.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     1797 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/observables/utils.py
+drwxr-xr-x   0 ejaaz     (1000) ejaaz     (1000)        0 2023-05-09 04:05:56.000000 qucumber-1.3.3/qucumber/rbm/
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)       80 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/rbm/__init__.py
+-rwxr-xr-x   0 ejaaz     (1000) ejaaz     (1000)     8555 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/rbm/binary_rbm.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)    16923 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/rbm/purification_rbm.py
+drwxr-xr-x   0 ejaaz     (1000) ejaaz     (1000)        0 2023-05-09 04:05:56.000000 qucumber-1.3.3/qucumber/utils/
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     2318 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/utils/__init__.py
+-rwxr-xr-x   0 ejaaz     (1000) ejaaz     (1000)    10932 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/utils/cplx.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     4609 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/utils/data.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     1862 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/utils/gradients_utils.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     8818 2023-05-09 02:05:38.000000 qucumber-1.3.3/qucumber/utils/training_statistics.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     9986 2023-05-08 23:55:08.000000 qucumber-1.3.3/qucumber/utils/unitaries.py
+drwxr-xr-x   0 ejaaz     (1000) ejaaz     (1000)        0 2023-05-09 04:05:56.000000 qucumber-1.3.3/qucumber.egg-info/
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     6657 2023-05-09 04:05:56.000000 qucumber-1.3.3/qucumber.egg-info/PKG-INFO
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     1587 2023-05-09 04:05:56.000000 qucumber-1.3.3/qucumber.egg-info/SOURCES.txt
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)        1 2023-05-09 04:05:56.000000 qucumber-1.3.3/qucumber.egg-info/dependency_links.txt
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)        1 2023-05-09 00:02:34.000000 qucumber-1.3.3/qucumber.egg-info/not-zip-safe
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     1365 2023-05-09 04:05:56.000000 qucumber-1.3.3/qucumber.egg-info/requires.txt
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)        9 2023-05-09 04:05:56.000000 qucumber-1.3.3/qucumber.egg-info/top_level.txt
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)       38 2023-05-09 04:05:56.000000 qucumber-1.3.3/setup.cfg
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     3675 2023-05-09 00:05:53.000000 qucumber-1.3.3/setup.py
+drwxr-xr-x   0 ejaaz     (1000) ejaaz     (1000)        0 2023-05-09 04:05:56.000000 qucumber-1.3.3/tests/
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     2193 2023-05-08 23:55:08.000000 qucumber-1.3.3/tests/test_callbacks.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)    12689 2023-05-08 23:55:08.000000 qucumber-1.3.3/tests/test_cplx.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     8624 2023-05-08 23:55:08.000000 qucumber-1.3.3/tests/test_grads.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)    12858 2023-05-08 23:55:08.000000 qucumber-1.3.3/tests/test_models_misc.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     7520 2023-05-08 23:55:08.000000 qucumber-1.3.3/tests/test_observables.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     9194 2023-05-08 23:55:08.000000 qucumber-1.3.3/tests/test_training.py
+-rw-r--r--   0 ejaaz     (1000) ejaaz     (1000)     1162 2023-05-08 23:55:08.000000 qucumber-1.3.3/tests/test_unitaries.py
```

### Comparing `qucumber-1.3.2/qucumber/rbm/purification_rbm.py` & `qucumber-1.3.3/qucumber/rbm/purification_rbm.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/rbm/binary_rbm.py` & `qucumber-1.3.3/qucumber/rbm/binary_rbm.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/nn_states/wavefunction.py` & `qucumber-1.3.3/qucumber/nn_states/wavefunction.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/nn_states/complex_wavefunction.py` & `qucumber-1.3.3/qucumber/nn_states/complex_wavefunction.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/nn_states/positive_wavefunction.py` & `qucumber-1.3.3/qucumber/nn_states/positive_wavefunction.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/nn_states/neural_state.py` & `qucumber-1.3.3/qucumber/nn_states/neural_state.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/nn_states/density_matrix.py` & `qucumber-1.3.3/qucumber/nn_states/density_matrix.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/callbacks/logger.py` & `qucumber-1.3.3/qucumber/callbacks/logger.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/callbacks/early_stopping.py` & `qucumber-1.3.3/qucumber/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/callbacks/observable_evaluator.py` & `qucumber-1.3.3/qucumber/callbacks/observable_evaluator.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/callbacks/timer.py` & `qucumber-1.3.3/qucumber/callbacks/timer.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/callbacks/model_saver.py` & `qucumber-1.3.3/qucumber/callbacks/model_saver.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/callbacks/variance_based_early_stopping.py` & `qucumber-1.3.3/qucumber/callbacks/variance_based_early_stopping.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/callbacks/lambda_callback.py` & `qucumber-1.3.3/qucumber/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/callbacks/callback.py` & `qucumber-1.3.3/qucumber/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/callbacks/liveplotting.py` & `qucumber-1.3.3/qucumber/callbacks/liveplotting.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/callbacks/metric_evaluator.py` & `qucumber-1.3.3/qucumber/callbacks/metric_evaluator.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/callbacks/callback_list.py` & `qucumber-1.3.3/qucumber/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/observables/entanglement.py` & `qucumber-1.3.3/qucumber/observables/entanglement.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/observables/pauli.py` & `qucumber-1.3.3/qucumber/observables/pauli.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/observables/system.py` & `qucumber-1.3.3/qucumber/observables/system.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/observables/interactions.py` & `qucumber-1.3.3/qucumber/observables/interactions.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/observables/observable.py` & `qucumber-1.3.3/qucumber/observables/observable.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/observables/utils.py` & `qucumber-1.3.3/qucumber/observables/utils.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/utils/cplx.py` & `qucumber-1.3.3/qucumber/utils/cplx.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/utils/unitaries.py` & `qucumber-1.3.3/qucumber/utils/unitaries.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/utils/data.py` & `qucumber-1.3.3/qucumber/utils/data.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/utils/gradients_utils.py` & `qucumber-1.3.3/qucumber/utils/gradients_utils.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/utils/training_statistics.py` & `qucumber-1.3.3/qucumber/utils/training_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,21 +60,21 @@
     else:
         assert target.dim() == 3, "target must be a complex matrix!"
 
         rho = nn_state.rho(space, space) / Z
         rho_rbm_ = cplx.numpy(rho)
         target_ = cplx.numpy(target)
 
-        sqrt_rho_rbm = sqrtm(rho_rbm_)
-        prod = np.matmul(sqrt_rho_rbm, np.matmul(target_, sqrt_rho_rbm))
+        # sqrt_rho_rbm = sqrtm(rho_rbm_)
+        prod = np.matmul(target_, rho_rbm_)
 
         # Instead of sqrt'ing then taking the trace, we compute the eigenvals,
         #  sqrt those, and then sum them up. This is a bit more efficient.
         eigvals = np.linalg.eigvals(prod).real  # imaginary parts should be zero
-        eigvals = np.abs(eigvals)
+        eigvals = np.abs(eigvals) # 0 eigenvals sometimes end up slightly negative
         trace = np.sum(np.sqrt(eigvals))
 
         return trace ** 2
 
 
 def NLL(nn_state, samples, space=None, sample_bases=None, **kwargs):
     r"""A function for calculating the negative log-likelihood (NLL).
```

### Comparing `qucumber-1.3.2/qucumber/utils/__init__.py` & `qucumber-1.3.3/qucumber/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber/__init__.py` & `qucumber-1.3.3/qucumber/__init__.py`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/PKG-INFO` & `qucumber-1.3.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,139 +1,23 @@
 Metadata-Version: 2.1
 Name: qucumber
-Version: 1.3.2
+Version: 1.3.3
 Summary: Neural Network Quantum State Tomography.
 Home-page: http://github.com/PIQuIL/QuCumber
 Author: PIQuIL
 Author-email: piquildbeets@gmail.com
 License: Apache License 2.0
-Description: # ![QuCumber](https://raw.githubusercontent.com/PIQuIL/QuCumber/master/docs/_static/img/QuCumber_full.png)
-        [![PyPI Version](https://img.shields.io/pypi/v/qucumber)](https://pypi.org/project/qucumber)
-        [![Python Versions](https://img.shields.io/pypi/pyversions/qucumber)](https://pypi.org/project/qucumber)
-        [![Documentation Status](https://readthedocs.org/projects/qucumber/badge/?version=stable)](https://qucumber.readthedocs.io/en/stable/?badge=stable)
-        [![Build Status (Travis)](https://travis-ci.com/PIQuIL/QuCumber.svg?branch=master)](https://travis-ci.com/PIQuIL/QuCumber)
-        [![Build Status (AppVeyor)](https://ci.appveyor.com/api/projects/status/lqdrc8qp94w4b9kf/branch/master?svg=true)](https://ci.appveyor.com/project/emerali/qucumber/branch/master)
-        [![codecov](https://codecov.io/gh/PIQuIL/QuCumber/branch/master/graph/badge.svg)](https://codecov.io/gh/PIQuIL/QuCumber)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-        [![arXiv](https://img.shields.io/badge/arXiv-1812.09329-B31B1B.svg)](https://arxiv.org/abs/1812.09329)
-        [![scipost](https://img.shields.io/badge/SciPost-7.1.009-blue.svg)](https://scipost.org/SciPostPhys.7.1.009)
-        
-        ## A Quantum Calculator Used for Many-body Eigenstate Reconstruction
-        
-        QuCumber is a program that reconstructs an unknown quantum wavefunction
-        from a set of measurements. The measurements should consist of binary counts;
-        for example, the occupation of an atomic orbital, or angular momentum eigenvalue of
-        a qubit. These measurements form a training set, which is used to train a
-        stochastic neural network called a Restricted Boltzmann Machine. Once trained, the
-        neural network is a reconstructed representation of the unknown wavefunction
-        underlying the measurement data. It can be used for generative modelling, i.e.
-        producing new instances of measurements, and to calculate estimators not
-        contained in the original data set.
-        
-        QuCumber is developed by the Perimeter Institute Quantum Intelligence Lab (PIQuIL).
-        
-        ## Features
-        
-        QuCumber implements unsupervised generative modelling with a two-layer RBM.
-        Each layer is a number of binary stochastic variables (with values 0 or 1). The
-        size of the visible layer corresponds to the input data, i.e. the number of
-        qubits. The size of the hidden layer is a hyperparameter, varied to systematically control
-        representation error.
-        
-        Currently, quantum state reconstruction/tomography can be performed on both pure and mixed states.
-        Pure state reconstruction can be further broken down into positive or complex wavefunction reconstruction.
-        In the case of a positive wavefunction, data is only required in one basis. For complex wavefunctions as
-        well as mixed states, measurement data in additional bases will be required to train the state.
-        
-        ## Documentation
-        
-        Documentation can be found [here](https://qucumber.readthedocs.io/en/stable/).
-        
-        See "QuCumber: wavefunction reconstruction with neural networks" https://scipost.org/SciPostPhys.7.1.009
-        
-        ## Getting Started
-        
-        These instructions will get you a copy of the project up and running on your
-        local machine for development and testing purposes.
-        
-        ### Installing
-        
-        If you're on Windows, you will have to install PyTorch manually; instructions
-        can be found on their website: [pytorch.org](https://pytorch.org).
-        
-        You can install the latest stable version of QuCumber, along with its dependencies,
-        using [`pip`](https://pip.pypa.io/en/stable/quickstart/):
-        
-        ```bash
-        pip install qucumber
-        ```
-        
-        If, for some reason, `pip` fails to install PyTorch, you can find installation
-        instructions on their website. Once that's done you should be able to install
-        QuCumber through `pip` as above.
-        
-        QuCumber supports Python 3.6 and newer stable versions.
-        
-        ### Installing the bleeding-edge version
-        
-        If you'd like to install the most upto date, but potentially unstable version,
-        you can clone the repository's master branch and then build from source like so:
-        
-        ```bash
-        git clone git@github.com:PIQuIL/QuCumber.git
-        cd ./QuCumber
-        python setup.py install
-        ```
-        
-        ## Contributing
-        
-        Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute
-        to the project, and the process for submitting pull requests to us.
-        
-        ## License
-        
-        QuCumber is licensed under the Apache License Version 2.0, this includes almost
-        all files in this repo. However, some miscellaneous files may be licensed
-        differently. See [LICENSE](LICENSE) for more details.
-        
-        ## Citation
-        
-        ```latex
-        @Article{10.21468/SciPostPhys.7.1.009,
-            title={{QuCumber: wavefunction reconstruction with neural networks}},
-            author={Matthew J. S. Beach and Isaac De Vlugt and Anna Golubeva and Patrick Huembeli and Bohdan Kulchytskyy and Xiuzhe Luo and Roger G. Melko and Ejaaz Merali and Giacomo Torlai},
-            journal={SciPost Phys.},
-            volume={7},
-            issue={1},
-            pages={9},
-            year={2019},
-            publisher={SciPost},
-            doi={10.21468/SciPostPhys.7.1.009},
-            url={https://scipost.org/10.21468/SciPostPhys.7.1.009},
-        }
-        ```
-        
-        ## Acknowledgments
-        
-        - We thank M. Albergo, G. Carleo, J. Carrasquilla, D. Sehayek, and
-          L. Hayward Sierens for many helpful discussions.
-        
-        - We thank the [Perimeter Institute](https://www.perimeterinstitute.ca) for the
-          continuing support of PIQuIL.
-        
-        - Thanks to Nick Mercer for creating our awesome logo. You can check out more of
-          Nick's work by visiting [his portfolio](https://www.behance.net/nickdmercec607)
-          on Behance!
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6.1,<4
@@ -142,7 +26,127 @@
 Provides-Extra: test
 Provides-Extra: coverage
 Provides-Extra: style
 Provides-Extra: travis
 Provides-Extra: appveyor
 Provides-Extra: rtd
 Provides-Extra: docs
+License-File: LICENSE
+License-File: LICENSE_HEADER
+
+# ![QuCumber](https://raw.githubusercontent.com/PIQuIL/QuCumber/master/docs/_static/img/QuCumber_full.png)
+[![PyPI Version](https://img.shields.io/pypi/v/qucumber)](https://pypi.org/project/qucumber)
+[![Python Versions](https://img.shields.io/pypi/pyversions/qucumber)](https://pypi.org/project/qucumber)
+[![Documentation Status](https://readthedocs.org/projects/qucumber/badge/?version=stable)](https://qucumber.readthedocs.io/en/stable/?badge=stable)
+[![Build Status (Travis)](https://travis-ci.com/PIQuIL/QuCumber.svg?branch=master)](https://travis-ci.com/PIQuIL/QuCumber)
+[![Build Status (AppVeyor)](https://ci.appveyor.com/api/projects/status/lqdrc8qp94w4b9kf/branch/master?svg=true)](https://ci.appveyor.com/project/emerali/qucumber/branch/master)
+[![codecov](https://codecov.io/gh/PIQuIL/QuCumber/branch/master/graph/badge.svg)](https://codecov.io/gh/PIQuIL/QuCumber)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![arXiv](https://img.shields.io/badge/arXiv-1812.09329-B31B1B.svg)](https://arxiv.org/abs/1812.09329)
+[![scipost](https://img.shields.io/badge/SciPost-7.1.009-blue.svg)](https://scipost.org/SciPostPhys.7.1.009)
+
+## A Quantum Calculator Used for Many-body Eigenstate Reconstruction
+
+QuCumber is a program that reconstructs an unknown quantum wavefunction
+from a set of measurements. The measurements should consist of binary counts;
+for example, the occupation of an atomic orbital, or angular momentum eigenvalue of
+a qubit. These measurements form a training set, which is used to train a
+stochastic neural network called a Restricted Boltzmann Machine. Once trained, the
+neural network is a reconstructed representation of the unknown wavefunction
+underlying the measurement data. It can be used for generative modelling, i.e.
+producing new instances of measurements, and to calculate estimators not
+contained in the original data set.
+
+QuCumber is developed by the Perimeter Institute Quantum Intelligence Lab (PIQuIL).
+
+## Features
+
+QuCumber implements unsupervised generative modelling with a two-layer RBM.
+Each layer is a number of binary stochastic variables (with values 0 or 1). The
+size of the visible layer corresponds to the input data, i.e. the number of
+qubits. The size of the hidden layer is a hyperparameter, varied to systematically control
+representation error.
+
+Currently, quantum state reconstruction/tomography can be performed on both pure and mixed states.
+Pure state reconstruction can be further broken down into positive or complex wavefunction reconstruction.
+In the case of a positive wavefunction, data is only required in one basis. For complex wavefunctions as
+well as mixed states, measurement data in additional bases will be required to train the state.
+
+## Documentation
+
+Documentation can be found [here](https://qucumber.readthedocs.io/en/stable/).
+
+See "QuCumber: wavefunction reconstruction with neural networks" https://scipost.org/SciPostPhys.7.1.009
+
+## Getting Started
+
+These instructions will get you a copy of the project up and running on your
+local machine for development and testing purposes.
+
+### Installing
+
+If you're on Windows, you will have to install PyTorch manually; instructions
+can be found on their website: [pytorch.org](https://pytorch.org).
+
+You can install the latest stable version of QuCumber, along with its dependencies,
+using [`pip`](https://pip.pypa.io/en/stable/quickstart/):
+
+```bash
+pip install qucumber
+```
+
+If, for some reason, `pip` fails to install PyTorch, you can find installation
+instructions on their website. Once that's done you should be able to install
+QuCumber through `pip` as above.
+
+QuCumber supports Python 3.6 and newer stable versions.
+
+### Installing the bleeding-edge version
+
+If you'd like to install the most upto date, but potentially unstable version,
+you can clone the repository's master branch and then build from source like so:
+
+```bash
+git clone git@github.com:PIQuIL/QuCumber.git
+cd ./QuCumber
+python setup.py install
+```
+
+## Contributing
+
+Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute
+to the project, and the process for submitting pull requests to us.
+
+## License
+
+QuCumber is licensed under the Apache License Version 2.0, this includes almost
+all files in this repo. However, some miscellaneous files may be licensed
+differently. See [LICENSE](LICENSE) for more details.
+
+## Citation
+
+```latex
+@Article{10.21468/SciPostPhys.7.1.009,
+    title={{QuCumber: wavefunction reconstruction with neural networks}},
+    author={Matthew J. S. Beach and Isaac De Vlugt and Anna Golubeva and Patrick Huembeli and Bohdan Kulchytskyy and Xiuzhe Luo and Roger G. Melko and Ejaaz Merali and Giacomo Torlai},
+    journal={SciPost Phys.},
+    volume={7},
+    issue={1},
+    pages={9},
+    year={2019},
+    publisher={SciPost},
+    doi={10.21468/SciPostPhys.7.1.009},
+    url={https://scipost.org/10.21468/SciPostPhys.7.1.009},
+}
+```
+
+## Acknowledgments
+
+- We thank M. Albergo, G. Carleo, J. Carrasquilla, D. Sehayek, and
+  L. Hayward Sierens for many helpful discussions.
+
+- We thank the [Perimeter Institute](https://www.perimeterinstitute.ca) for the
+  continuing support of PIQuIL.
+
+- Thanks to Nick Mercer for creating our awesome logo. You can check out more of
+  Nick's work by visiting [his portfolio](https://www.behance.net/nickdmercec607)
+  on Behance!
```

### Comparing `qucumber-1.3.2/README.md` & `qucumber-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `qucumber-1.3.2/qucumber.egg-info/PKG-INFO` & `qucumber-1.3.3/qucumber.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,139 +1,23 @@
 Metadata-Version: 2.1
 Name: qucumber
-Version: 1.3.2
+Version: 1.3.3
 Summary: Neural Network Quantum State Tomography.
 Home-page: http://github.com/PIQuIL/QuCumber
 Author: PIQuIL
 Author-email: piquildbeets@gmail.com
 License: Apache License 2.0
-Description: # ![QuCumber](https://raw.githubusercontent.com/PIQuIL/QuCumber/master/docs/_static/img/QuCumber_full.png)
-        [![PyPI Version](https://img.shields.io/pypi/v/qucumber)](https://pypi.org/project/qucumber)
-        [![Python Versions](https://img.shields.io/pypi/pyversions/qucumber)](https://pypi.org/project/qucumber)
-        [![Documentation Status](https://readthedocs.org/projects/qucumber/badge/?version=stable)](https://qucumber.readthedocs.io/en/stable/?badge=stable)
-        [![Build Status (Travis)](https://travis-ci.com/PIQuIL/QuCumber.svg?branch=master)](https://travis-ci.com/PIQuIL/QuCumber)
-        [![Build Status (AppVeyor)](https://ci.appveyor.com/api/projects/status/lqdrc8qp94w4b9kf/branch/master?svg=true)](https://ci.appveyor.com/project/emerali/qucumber/branch/master)
-        [![codecov](https://codecov.io/gh/PIQuIL/QuCumber/branch/master/graph/badge.svg)](https://codecov.io/gh/PIQuIL/QuCumber)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-        [![arXiv](https://img.shields.io/badge/arXiv-1812.09329-B31B1B.svg)](https://arxiv.org/abs/1812.09329)
-        [![scipost](https://img.shields.io/badge/SciPost-7.1.009-blue.svg)](https://scipost.org/SciPostPhys.7.1.009)
-        
-        ## A Quantum Calculator Used for Many-body Eigenstate Reconstruction
-        
-        QuCumber is a program that reconstructs an unknown quantum wavefunction
-        from a set of measurements. The measurements should consist of binary counts;
-        for example, the occupation of an atomic orbital, or angular momentum eigenvalue of
-        a qubit. These measurements form a training set, which is used to train a
-        stochastic neural network called a Restricted Boltzmann Machine. Once trained, the
-        neural network is a reconstructed representation of the unknown wavefunction
-        underlying the measurement data. It can be used for generative modelling, i.e.
-        producing new instances of measurements, and to calculate estimators not
-        contained in the original data set.
-        
-        QuCumber is developed by the Perimeter Institute Quantum Intelligence Lab (PIQuIL).
-        
-        ## Features
-        
-        QuCumber implements unsupervised generative modelling with a two-layer RBM.
-        Each layer is a number of binary stochastic variables (with values 0 or 1). The
-        size of the visible layer corresponds to the input data, i.e. the number of
-        qubits. The size of the hidden layer is a hyperparameter, varied to systematically control
-        representation error.
-        
-        Currently, quantum state reconstruction/tomography can be performed on both pure and mixed states.
-        Pure state reconstruction can be further broken down into positive or complex wavefunction reconstruction.
-        In the case of a positive wavefunction, data is only required in one basis. For complex wavefunctions as
-        well as mixed states, measurement data in additional bases will be required to train the state.
-        
-        ## Documentation
-        
-        Documentation can be found [here](https://qucumber.readthedocs.io/en/stable/).
-        
-        See "QuCumber: wavefunction reconstruction with neural networks" https://scipost.org/SciPostPhys.7.1.009
-        
-        ## Getting Started
-        
-        These instructions will get you a copy of the project up and running on your
-        local machine for development and testing purposes.
-        
-        ### Installing
-        
-        If you're on Windows, you will have to install PyTorch manually; instructions
-        can be found on their website: [pytorch.org](https://pytorch.org).
-        
-        You can install the latest stable version of QuCumber, along with its dependencies,
-        using [`pip`](https://pip.pypa.io/en/stable/quickstart/):
-        
-        ```bash
-        pip install qucumber
-        ```
-        
-        If, for some reason, `pip` fails to install PyTorch, you can find installation
-        instructions on their website. Once that's done you should be able to install
-        QuCumber through `pip` as above.
-        
-        QuCumber supports Python 3.6 and newer stable versions.
-        
-        ### Installing the bleeding-edge version
-        
-        If you'd like to install the most upto date, but potentially unstable version,
-        you can clone the repository's master branch and then build from source like so:
-        
-        ```bash
-        git clone git@github.com:PIQuIL/QuCumber.git
-        cd ./QuCumber
-        python setup.py install
-        ```
-        
-        ## Contributing
-        
-        Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute
-        to the project, and the process for submitting pull requests to us.
-        
-        ## License
-        
-        QuCumber is licensed under the Apache License Version 2.0, this includes almost
-        all files in this repo. However, some miscellaneous files may be licensed
-        differently. See [LICENSE](LICENSE) for more details.
-        
-        ## Citation
-        
-        ```latex
-        @Article{10.21468/SciPostPhys.7.1.009,
-            title={{QuCumber: wavefunction reconstruction with neural networks}},
-            author={Matthew J. S. Beach and Isaac De Vlugt and Anna Golubeva and Patrick Huembeli and Bohdan Kulchytskyy and Xiuzhe Luo and Roger G. Melko and Ejaaz Merali and Giacomo Torlai},
-            journal={SciPost Phys.},
-            volume={7},
-            issue={1},
-            pages={9},
-            year={2019},
-            publisher={SciPost},
-            doi={10.21468/SciPostPhys.7.1.009},
-            url={https://scipost.org/10.21468/SciPostPhys.7.1.009},
-        }
-        ```
-        
-        ## Acknowledgments
-        
-        - We thank M. Albergo, G. Carleo, J. Carrasquilla, D. Sehayek, and
-          L. Hayward Sierens for many helpful discussions.
-        
-        - We thank the [Perimeter Institute](https://www.perimeterinstitute.ca) for the
-          continuing support of PIQuIL.
-        
-        - Thanks to Nick Mercer for creating our awesome logo. You can check out more of
-          Nick's work by visiting [his portfolio](https://www.behance.net/nickdmercec607)
-          on Behance!
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6.1,<4
@@ -142,7 +26,127 @@
 Provides-Extra: test
 Provides-Extra: coverage
 Provides-Extra: style
 Provides-Extra: travis
 Provides-Extra: appveyor
 Provides-Extra: rtd
 Provides-Extra: docs
+License-File: LICENSE
+License-File: LICENSE_HEADER
+
+# ![QuCumber](https://raw.githubusercontent.com/PIQuIL/QuCumber/master/docs/_static/img/QuCumber_full.png)
+[![PyPI Version](https://img.shields.io/pypi/v/qucumber)](https://pypi.org/project/qucumber)
+[![Python Versions](https://img.shields.io/pypi/pyversions/qucumber)](https://pypi.org/project/qucumber)
+[![Documentation Status](https://readthedocs.org/projects/qucumber/badge/?version=stable)](https://qucumber.readthedocs.io/en/stable/?badge=stable)
+[![Build Status (Travis)](https://travis-ci.com/PIQuIL/QuCumber.svg?branch=master)](https://travis-ci.com/PIQuIL/QuCumber)
+[![Build Status (AppVeyor)](https://ci.appveyor.com/api/projects/status/lqdrc8qp94w4b9kf/branch/master?svg=true)](https://ci.appveyor.com/project/emerali/qucumber/branch/master)
+[![codecov](https://codecov.io/gh/PIQuIL/QuCumber/branch/master/graph/badge.svg)](https://codecov.io/gh/PIQuIL/QuCumber)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![arXiv](https://img.shields.io/badge/arXiv-1812.09329-B31B1B.svg)](https://arxiv.org/abs/1812.09329)
+[![scipost](https://img.shields.io/badge/SciPost-7.1.009-blue.svg)](https://scipost.org/SciPostPhys.7.1.009)
+
+## A Quantum Calculator Used for Many-body Eigenstate Reconstruction
+
+QuCumber is a program that reconstructs an unknown quantum wavefunction
+from a set of measurements. The measurements should consist of binary counts;
+for example, the occupation of an atomic orbital, or angular momentum eigenvalue of
+a qubit. These measurements form a training set, which is used to train a
+stochastic neural network called a Restricted Boltzmann Machine. Once trained, the
+neural network is a reconstructed representation of the unknown wavefunction
+underlying the measurement data. It can be used for generative modelling, i.e.
+producing new instances of measurements, and to calculate estimators not
+contained in the original data set.
+
+QuCumber is developed by the Perimeter Institute Quantum Intelligence Lab (PIQuIL).
+
+## Features
+
+QuCumber implements unsupervised generative modelling with a two-layer RBM.
+Each layer is a number of binary stochastic variables (with values 0 or 1). The
+size of the visible layer corresponds to the input data, i.e. the number of
+qubits. The size of the hidden layer is a hyperparameter, varied to systematically control
+representation error.
+
+Currently, quantum state reconstruction/tomography can be performed on both pure and mixed states.
+Pure state reconstruction can be further broken down into positive or complex wavefunction reconstruction.
+In the case of a positive wavefunction, data is only required in one basis. For complex wavefunctions as
+well as mixed states, measurement data in additional bases will be required to train the state.
+
+## Documentation
+
+Documentation can be found [here](https://qucumber.readthedocs.io/en/stable/).
+
+See "QuCumber: wavefunction reconstruction with neural networks" https://scipost.org/SciPostPhys.7.1.009
+
+## Getting Started
+
+These instructions will get you a copy of the project up and running on your
+local machine for development and testing purposes.
+
+### Installing
+
+If you're on Windows, you will have to install PyTorch manually; instructions
+can be found on their website: [pytorch.org](https://pytorch.org).
+
+You can install the latest stable version of QuCumber, along with its dependencies,
+using [`pip`](https://pip.pypa.io/en/stable/quickstart/):
+
+```bash
+pip install qucumber
+```
+
+If, for some reason, `pip` fails to install PyTorch, you can find installation
+instructions on their website. Once that's done you should be able to install
+QuCumber through `pip` as above.
+
+QuCumber supports Python 3.6 and newer stable versions.
+
+### Installing the bleeding-edge version
+
+If you'd like to install the most upto date, but potentially unstable version,
+you can clone the repository's master branch and then build from source like so:
+
+```bash
+git clone git@github.com:PIQuIL/QuCumber.git
+cd ./QuCumber
+python setup.py install
+```
+
+## Contributing
+
+Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute
+to the project, and the process for submitting pull requests to us.
+
+## License
+
+QuCumber is licensed under the Apache License Version 2.0, this includes almost
+all files in this repo. However, some miscellaneous files may be licensed
+differently. See [LICENSE](LICENSE) for more details.
+
+## Citation
+
+```latex
+@Article{10.21468/SciPostPhys.7.1.009,
+    title={{QuCumber: wavefunction reconstruction with neural networks}},
+    author={Matthew J. S. Beach and Isaac De Vlugt and Anna Golubeva and Patrick Huembeli and Bohdan Kulchytskyy and Xiuzhe Luo and Roger G. Melko and Ejaaz Merali and Giacomo Torlai},
+    journal={SciPost Phys.},
+    volume={7},
+    issue={1},
+    pages={9},
+    year={2019},
+    publisher={SciPost},
+    doi={10.21468/SciPostPhys.7.1.009},
+    url={https://scipost.org/10.21468/SciPostPhys.7.1.009},
+}
+```
+
+## Acknowledgments
+
+- We thank M. Albergo, G. Carleo, J. Carrasquilla, D. Sehayek, and
+  L. Hayward Sierens for many helpful discussions.
+
+- We thank the [Perimeter Institute](https://www.perimeterinstitute.ca) for the
+  continuing support of PIQuIL.
+
+- Thanks to Nick Mercer for creating our awesome logo. You can check out more of
+  Nick's work by visiting [his portfolio](https://www.behance.net/nickdmercec607)
+  on Behance!
```

### Comparing `qucumber-1.3.2/qucumber.egg-info/requires.txt` & `qucumber-1.3.3/qucumber.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 tqdm>=4.23
 numpy>=1.13
 scipy>=1.3.3
 matplotlib>=2.2
 
 [:sys_platform != "win32"]
-torch<1.8,>=1.2
+torch<2.1,>=1.2
 
 [appveyor]
 setuptools>=40.0.0
 wheel>=0.31.1
 pytest>=3.7.1
 tox>=3.2.1
```

### Comparing `qucumber-1.3.2/setup.py` & `qucumber-1.3.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description = fh.read()
 
 version_file = {}
 with open(os.path.join("qucumber", "__version__.py"), "r") as f:
     exec(f.read(), version_file)
 
 install_requires = [
-    "torch>=1.2,<1.8; sys_platform != 'win32'",
+    "torch>=1.2,<2.1; sys_platform != 'win32'",
     "tqdm>=4.23",
     "numpy>=1.13",
     "scipy>=1.3.3",
     "matplotlib>=2.2",
 ]
 
 # using a requirements.txt file for RTD dependencies
@@ -86,14 +86,17 @@
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Physics",
     ],
```

