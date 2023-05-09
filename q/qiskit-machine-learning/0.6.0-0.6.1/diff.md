# Comparing `tmp/qiskit-machine-learning-0.6.0.tar.gz` & `tmp/qiskit-machine-learning-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qiskit-machine-learning-0.6.0.tar", last modified: Mon Mar 27 20:48:34 2023, max compression
+gzip compressed data, was "dist/qiskit-machine-learning-0.6.1.tar", last modified: Tue May  9 08:00:12 2023, max compression
```

## Comparing `qiskit-machine-learning-0.6.0.tar` & `qiskit-machine-learning-0.6.1.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/classifiers/neural_network_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/classifiers/pegasos_qsvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/classifiers/qsvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/classifiers/vqc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/_pytorch_discriminator_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/discriminative_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/generative_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    15573 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/numpy_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/pytorch_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18410 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/qgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    19244 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/quantum_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/objective_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/regressors/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/regressors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/regressors/neural_network_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/regressors/qsvr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/regressors/vqr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/serializable_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/trainable_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/circuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/circuit/library/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/circuit/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/circuit/library/raw_feature_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/connectors/torch_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/datasets/ad_hoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/datasets/dataset_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/algorithms/quantum_kernel_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/base_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/fidelity_quantum_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/fidelity_statevector_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    30498 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/quantum_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/trainable_fidelity_quantum_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/trainable_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/circuit_qnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    14749 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/effective_dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/estimator_qnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10104 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/opflow_qnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/sampler_qnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/sampling_neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/two_layer_qnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/optionals.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/runtime/hookbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/runtime/torch_runtime_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/utils/adjust_num_qubits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/utils/loss_functions/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/utils/loss_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/utils/loss_functions/kernel_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/utils/loss_functions/loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/qiskit_machine_learning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/algorithms/classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_fidelity_quantum_kernel_pegasos_qsvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_fidelity_quantum_kernel_qsvc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17914 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_neural_network_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_neural_network_classifier_sampler_qnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_pegasos_qsvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_qsvc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_vqc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/algorithms/distribution_learners/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/distribution_learners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/algorithms/distribution_learners/qgan/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/distribution_learners/qgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/distribution_learners/qgan/test_qgan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/algorithms/regressors/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/regressors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/regressors/test_fidelity_quantum_kernel_qsvr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/regressors/test_neural_network_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/regressors/test_neural_network_regressor_estimator_qnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/regressors/test_qsvr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/regressors/test_vqr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/algorithms/regressors/test_vqr_estimator_qnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/circuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/circuit/library/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/circuit/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/circuit/library/test_raw_feature_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/connectors/test_cpu_torch_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/connectors/test_cpu_torch_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/connectors/test_gpu_torch_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/connectors/test_gpu_torch_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/connectors/test_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26436 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/connectors/test_torch_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/connectors/test_torch_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/datasets/ad_hoc_ref.json
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/datasets/test_ad_hoc_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/kernels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/kernels/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/kernels/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/kernels/algorithms/test_fidelity_qkernel_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/kernels/algorithms/test_qkernel_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/kernels/test_deprecated_qkernel_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/kernels/test_fidelity_qkernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15574 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/kernels/test_fidelity_statevector_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/kernels/test_new_vs_old_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/kernels/test_new_vs_old_kernel_sv.py
--rw-r--r--   0 runner    (1001) docker     (123)    33682 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/kernels/test_qkernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/kernels/test_trainable_fidelity_qkernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/machine_learning_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/neural_networks/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/neural_networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17124 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/neural_networks/test_circuit_qnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/neural_networks/test_circuit_vs_sampler_qnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/neural_networks/test_effective_dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/neural_networks/test_effective_dimension_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/neural_networks/test_estimator_qnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/neural_networks/test_neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/neural_networks/test_opflow_qnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11629 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/neural_networks/test_sampler_qnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/neural_networks/test_two_layer_qnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/runtime/fake_torchruntime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/runtime/test_torch_runtime_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18879 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/test_readme_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:34.000000 qiskit-machine-learning-0.6.0/test/utils/loss_functions/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/utils/loss_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/utils/loss_functions/test_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-03-27 20:48:21.000000 qiskit-machine-learning-0.6.0/test/utils/test_adjust_num_qubits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12009 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/classifiers/neural_network_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/classifiers/pegasos_qsvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/classifiers/qsvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/classifiers/vqc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/_pytorch_discriminator_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/discriminative_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/generative_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15606 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/numpy_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/pytorch_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18410 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/qgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19244 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/quantum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/objective_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/regressors/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/regressors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/regressors/neural_network_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/regressors/qsvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/regressors/vqr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/serializable_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/trainable_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/circuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/circuit/library/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/circuit/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/circuit/library/raw_feature_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/connectors/torch_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/datasets/ad_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/datasets/dataset_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/algorithms/quantum_kernel_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/base_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/fidelity_quantum_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/fidelity_statevector_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30498 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/quantum_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/trainable_fidelity_quantum_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/trainable_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/circuit_qnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14749 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/effective_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/estimator_qnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10104 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/opflow_qnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/sampler_qnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/sampling_neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/two_layer_qnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/optionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/runtime/hookbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/runtime/torch_runtime_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/utils/adjust_num_qubits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/utils/loss_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/utils/loss_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/utils/loss_functions/kernel_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/utils/loss_functions/loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12009 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/qiskit_machine_learning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/algorithms/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_fidelity_quantum_kernel_pegasos_qsvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_fidelity_quantum_kernel_qsvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17914 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_neural_network_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_neural_network_classifier_sampler_qnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_pegasos_qsvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_qsvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_vqc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/algorithms/distribution_learners/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/distribution_learners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/algorithms/distribution_learners/qgan/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/distribution_learners/qgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/distribution_learners/qgan/test_qgan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/algorithms/regressors/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/regressors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/regressors/test_fidelity_quantum_kernel_qsvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/regressors/test_neural_network_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/regressors/test_neural_network_regressor_estimator_qnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/regressors/test_qsvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/regressors/test_vqr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/algorithms/regressors/test_vqr_estimator_qnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/circuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/circuit/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/circuit/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/circuit/library/test_raw_feature_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/connectors/test_cpu_torch_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/connectors/test_cpu_torch_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/connectors/test_gpu_torch_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/connectors/test_gpu_torch_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/connectors/test_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26470 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/connectors/test_torch_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/connectors/test_torch_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/datasets/ad_hoc_ref.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/datasets/test_ad_hoc_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/kernels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/kernels/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/kernels/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/kernels/algorithms/test_fidelity_qkernel_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/kernels/algorithms/test_qkernel_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/kernels/test_deprecated_qkernel_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16073 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/kernels/test_fidelity_qkernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/kernels/test_fidelity_statevector_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/kernels/test_new_vs_old_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/kernels/test_new_vs_old_kernel_sv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33682 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/kernels/test_qkernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/kernels/test_trainable_fidelity_qkernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/machine_learning_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/neural_networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/neural_networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17124 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/neural_networks/test_circuit_qnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/neural_networks/test_circuit_vs_sampler_qnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/neural_networks/test_effective_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/neural_networks/test_effective_dimension_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/neural_networks/test_estimator_qnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/neural_networks/test_neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/neural_networks/test_opflow_qnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11629 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/neural_networks/test_sampler_qnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/neural_networks/test_two_layer_qnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/runtime/fake_torchruntime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/runtime/test_torch_runtime_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18879 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/test_readme_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:00:12.000000 qiskit-machine-learning-0.6.1/test/utils/loss_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/utils/loss_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/utils/loss_functions/test_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-09 08:00:01.000000 qiskit-machine-learning-0.6.1/test/utils/test_adjust_num_qubits.py
```

### Comparing `qiskit-machine-learning-0.6.0/LICENSE.txt` & `qiskit-machine-learning-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/PKG-INFO` & `qiskit-machine-learning-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-machine-learning
-Version: 0.6.0
+Version: 0.6.1
 Summary: Qiskit Machine Learning: A library of quantum computing machine learning experiments
 Home-page: https://github.com/Qiskit/qiskit-machine-learning
 Author: Qiskit Machine Learning Development Team
 Author-email: hello@qiskit.org
 License: Apache-2.0
 Keywords: qiskit sdk quantum machine learning ml
 Classifier: Environment :: Console
@@ -15,14 +15,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: torch
 Provides-Extra: sparse
 License-File: LICENSE.txt
```

### Comparing `qiskit-machine-learning-0.6.0/README.md` & `qiskit-machine-learning-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/classifiers/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/classifiers/neural_network_classifier.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/classifiers/neural_network_classifier.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/classifiers/pegasos_qsvc.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/classifiers/pegasos_qsvc.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/classifiers/qsvc.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/classifiers/qsvc.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/classifiers/vqc.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/classifiers/vqc.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/_pytorch_discriminator_net.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/_pytorch_discriminator_net.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/discriminative_network.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/discriminative_network.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/generative_network.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/generative_network.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/numpy_discriminator.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/numpy_discriminator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2019, 2022.
+# (C) Copyright IBM 2019, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -12,15 +12,15 @@
 
 """
 Discriminator
 
 The neural network is based on a neural network introduced in:
 https://towardsdatascience.com/lets-code-a-neural-network-in-plain-numpy-ae7e74410795
 """
-
+import builtins
 from typing import Dict, Any
 import os
 import numpy as np
 from qiskit.utils import algorithm_globals
 from qiskit.algorithms.optimizers import ADAM
 
 from ....deprecation import deprecate_function
@@ -99,15 +99,15 @@
             z_curr = np.dot(w_new, x_old)
 
             if activation == "leaky_relu":
                 activation_func = leaky_relu
             elif activation == "sigmoid":
                 activation_func = sigmoid
             else:
-                raise Exception("Non-supported activation function")
+                raise builtins.Exception("Non-supported activation function")
 
             return activation_func(z_curr), z_curr
 
         x_new = x
         pointer = 0
         for idx, layer in enumerate(self.architecture):
             layer_idx = idx + 1
@@ -159,15 +159,15 @@
         ):
             # m = a_prev.shape[1]
             if activation == "leaky_relu":
                 backward_activation_func = leaky_relu_backward
             elif activation == "sigmoid":
                 backward_activation_func = sigmoid_backward
             else:
-                raise Exception("Non-supported activation function")
+                raise builtins.Exception("Non-supported activation function")
 
             dz_curr = backward_activation_func(da_curr, z_curr)
             dw_curr = np.dot(dz_curr, a_prev.T)
             da_prev = np.dot(w_curr.T, dz_curr)
 
             return da_prev, dw_curr
```

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/pytorch_discriminator.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/pytorch_discriminator.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/qgan.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/qgan.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/distribution_learners/qgan/quantum_generator.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/distribution_learners/qgan/quantum_generator.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/objective_functions.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/objective_functions.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/regressors/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/regressors/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/regressors/neural_network_regressor.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/regressors/neural_network_regressor.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/regressors/qsvr.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/regressors/qsvr.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/regressors/vqr.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/regressors/vqr.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/serializable_model.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/serializable_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/algorithms/trainable_model.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/algorithms/trainable_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/circuit/library/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/circuit/library/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/circuit/library/raw_feature_vector.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/circuit/library/raw_feature_vector.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/connectors/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/connectors/torch_connector.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/connectors/torch_connector.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/datasets/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/datasets/ad_hoc.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/datasets/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/datasets/dataset_helper.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/datasets/dataset_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2018, 2022.
+# (C) Copyright IBM 2018, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -117,15 +117,15 @@
         else:
             temp = []
             for grid_element in grid_elements:
                 for element_current in elements_current_dim:
                     temp.append(grid_element + [element_current])
             grid_elements = deepcopy(temp)
             data_grid.append(elements_current_dim)
-    data_grid = np.array(data_grid)
+    data_grid = np.array(data_grid, dtype=object)
 
     data = np.reshape(data, (len(data), len(data[0])))
 
     if return_prob:
         if np.ndim(data) > 1:
             prob_data = np.zeros(int(np.prod(np.power(np.ones(len(data[0])) * 2, num_qubits))))
         else:
```

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/deprecation.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/deprecation.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/exceptions.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/algorithms/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/algorithms/quantum_kernel_trainer.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/algorithms/quantum_kernel_trainer.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/base_kernel.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/base_kernel.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/fidelity_quantum_kernel.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/fidelity_quantum_kernel.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/fidelity_statevector_kernel.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/fidelity_statevector_kernel.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/quantum_kernel.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/quantum_kernel.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/trainable_fidelity_quantum_kernel.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/trainable_fidelity_quantum_kernel.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/kernels/trainable_kernel.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/kernels/trainable_kernel.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/circuit_qnn.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/circuit_qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/effective_dimension.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/effective_dimension.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/estimator_qnn.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/estimator_qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/neural_network.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/neural_network.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/opflow_qnn.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/opflow_qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/sampler_qnn.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/sampler_qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/sampling_neural_network.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/sampling_neural_network.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/neural_networks/two_layer_qnn.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/neural_networks/two_layer_qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/optionals.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/optionals.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/runtime/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/runtime/hookbase.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/runtime/hookbase.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/runtime/torch_runtime_client.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/runtime/torch_runtime_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/utils/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/utils/adjust_num_qubits.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/utils/adjust_num_qubits.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/utils/loss_functions/__init__.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/utils/loss_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/utils/loss_functions/kernel_loss_functions.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/utils/loss_functions/kernel_loss_functions.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/utils/loss_functions/loss_functions.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/utils/loss_functions/loss_functions.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning/version.py` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning.egg-info/PKG-INFO` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-machine-learning
-Version: 0.6.0
+Version: 0.6.1
 Summary: Qiskit Machine Learning: A library of quantum computing machine learning experiments
 Home-page: https://github.com/Qiskit/qiskit-machine-learning
 Author: Qiskit Machine Learning Development Team
 Author-email: hello@qiskit.org
 License: Apache-2.0
 Keywords: qiskit sdk quantum machine learning ml
 Classifier: Environment :: Console
@@ -15,14 +15,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: torch
 Provides-Extra: sparse
 License-File: LICENSE.txt
```

### Comparing `qiskit-machine-learning-0.6.0/qiskit_machine_learning.egg-info/SOURCES.txt` & `qiskit-machine-learning-0.6.1/qiskit_machine_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/setup.py` & `qiskit-machine-learning-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2021, 2022.
+# (C) Copyright IBM 2021, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -57,20 +57,21 @@
         "Operating System :: MacOS",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering"
     ],
     keywords='qiskit sdk quantum machine learning ml',
     packages=setuptools.find_packages(include=['qiskit_machine_learning','qiskit_machine_learning.*']),
     install_requires=REQUIREMENTS,
     include_package_data=True,
     python_requires=">=3.7",
     extras_require={
-        'torch': ["torch; python_version < '3.10'"],
+        'torch': ["torch"],
         'sparse': ["sparse"],
     },
     zip_safe=False
 )
```

### Comparing `qiskit-machine-learning-0.6.0/test/__init__.py` & `qiskit-machine-learning-0.6.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_fidelity_quantum_kernel_pegasos_qsvc.py` & `qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_fidelity_quantum_kernel_pegasos_qsvc.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_fidelity_quantum_kernel_qsvc.py` & `qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_fidelity_quantum_kernel_qsvc.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_neural_network_classifier.py` & `qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_neural_network_classifier.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_neural_network_classifier_sampler_qnn.py` & `qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_neural_network_classifier_sampler_qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_pegasos_qsvc.py` & `qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_pegasos_qsvc.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_qsvc.py` & `qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_qsvc.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/classifiers/test_vqc.py` & `qiskit-machine-learning-0.6.1/test/algorithms/classifiers/test_vqc.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/distribution_learners/qgan/test_qgan.py` & `qiskit-machine-learning-0.6.1/test/algorithms/distribution_learners/qgan/test_qgan.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/regressors/test_fidelity_quantum_kernel_qsvr.py` & `qiskit-machine-learning-0.6.1/test/algorithms/regressors/test_fidelity_quantum_kernel_qsvr.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/regressors/test_neural_network_regressor.py` & `qiskit-machine-learning-0.6.1/test/algorithms/regressors/test_neural_network_regressor.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/regressors/test_neural_network_regressor_estimator_qnn.py` & `qiskit-machine-learning-0.6.1/test/algorithms/regressors/test_neural_network_regressor_estimator_qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/regressors/test_qsvr.py` & `qiskit-machine-learning-0.6.1/test/algorithms/regressors/test_qsvr.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/regressors/test_vqr.py` & `qiskit-machine-learning-0.6.1/test/algorithms/regressors/test_vqr.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/algorithms/regressors/test_vqr_estimator_qnn.py` & `qiskit-machine-learning-0.6.1/test/algorithms/regressors/test_vqr_estimator_qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/circuit/library/test_raw_feature_vector.py` & `qiskit-machine-learning-0.6.1/test/circuit/library/test_raw_feature_vector.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/connectors/test_cpu_torch_connector.py` & `qiskit-machine-learning-0.6.1/test/connectors/test_cpu_torch_connector.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/connectors/test_cpu_torch_networks.py` & `qiskit-machine-learning-0.6.1/test/connectors/test_cpu_torch_networks.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/connectors/test_gpu_torch_connector.py` & `qiskit-machine-learning-0.6.1/test/connectors/test_gpu_torch_connector.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/connectors/test_gpu_torch_networks.py` & `qiskit-machine-learning-0.6.1/test/connectors/test_gpu_torch_networks.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/connectors/test_torch.py` & `qiskit-machine-learning-0.6.1/test/connectors/test_torch.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Test Torch Base."""
 
 import unittest
+import builtins
 import warnings
 from abc import ABC, abstractmethod
 from qiskit.utils import QuantumInstance, algorithm_globals, optionals
 import qiskit_machine_learning.optionals as _optionals
 
 
 class TestTorch(ABC):
@@ -58,48 +59,48 @@
         """Tear down the test."""
         warnings.filterwarnings("always", category=PendingDeprecationWarning)
 
     @abstractmethod
     def subTest(self, msg, **kwargs):
         # pylint: disable=invalid-name
         """Sub test."""
-        raise Exception("Abstract method")
+        raise builtins.Exception("Abstract method")
 
     @abstractmethod
     def assertAlmostEqual(self, first, second, places=None, msg=None, delta=None):
         """Assert almost equal."""
-        raise Exception("Abstract method")
+        raise builtins.Exception("Abstract method")
 
     @abstractmethod
     def assertEqual(self, first, second, msg=None):
         """Assert equal."""
-        raise Exception("Abstract method")
+        raise builtins.Exception("Abstract method")
 
     @abstractmethod
     def assertTrue(self, expr, msg=None):
         """Assert true."""
-        raise Exception("Abstract method")
+        raise builtins.Exception("Abstract method")
 
     @abstractmethod
     def assertFalse(self, expr, msg=None):
         """assert False"""
-        raise Exception("Abstract method")
+        raise builtins.Exception("Abstract method")
 
     @abstractmethod
     def skipTest(self, reason):  # pylint: disable=invalid-name
         """Skip test."""
-        raise Exception("Abstract method")
+        raise builtins.Exception("Abstract method")
 
     @abstractmethod
     def assertLogs(self, logger=None, level=None):
         """Assert logs."""
-        raise Exception("Abstract method")
+        raise builtins.Exception("Abstract method")
 
     @abstractmethod
     def assertListEqual(self, list1, list2, msg=None):
         """Assert list equal."""
-        raise Exception("Abstract method")
+        raise builtins.Exception("Abstract method")
 
     @abstractmethod
     def assertRaises(self, expected_exception):
         """Assert raises an exception."""
-        raise Exception("Abstract method")
+        raise builtins.Exception("Abstract method")
```

### Comparing `qiskit-machine-learning-0.6.0/test/connectors/test_torch_connector.py` & `qiskit-machine-learning-0.6.1/test/connectors/test_torch_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Test Torch Connector."""
+import builtins
 import itertools
 import sys
 from typing import List, cast
 
 from test.connectors.test_torch import TestTorch
 
 import numpy as np
@@ -79,28 +80,28 @@
         # iterate over test data and validate behavior of model
         for x in test_data:
             x = x.to(self._device)
             # test linear model and track whether it failed or store the output shape
             c_worked = True
             try:
                 c_shape = linear(x).shape
-            except Exception:  # pylint: disable=broad-except
+            except builtins.Exception:  # pylint: disable=broad-except
                 c_worked = False
 
             # test quantum model and track whether it failed or store the output shape
             q_worked = True
             try:
                 output = model(x)
 
                 # check output is sparse
                 model_sparse = model.sparse if model.sparse else False
                 self.assertEqual(output.is_sparse, model_sparse)
 
                 q_shape = output.shape
-            except Exception:  # pylint: disable=broad-except
+            except builtins.Exception:  # pylint: disable=broad-except
                 q_worked = False
 
             # compare results and assert that the behavior is equal
             with self.subTest("c_worked == q_worked", tensor=x):
                 self.assertEqual(c_worked, q_worked)
             if c_worked and q_worked:
                 with self.subTest("c_shape == q_shape", tensor=x):
```

### Comparing `qiskit-machine-learning-0.6.0/test/connectors/test_torch_networks.py` & `qiskit-machine-learning-0.6.1/test/connectors/test_torch_networks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2022.
+# (C) Copyright IBM 2022, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -56,17 +56,20 @@
                 x = self.qnn(x)  # apply QNN
                 x = self.fc2(x)
                 return cat((x, 1 - x), -1)
 
         return Net()
 
     def _create_circuit_qnn(self) -> CircuitQNN:
-        output_shape, interpret = 2, lambda x: f"{x:b}".count("1") % 2
+        output_shape = 2
         num_inputs = 2
 
+        def interpret(x):
+            return f"{x:b}".count("1") % 2
+
         feature_map = ZZFeatureMap(num_inputs)
         ansatz = RealAmplitudes(num_inputs, entanglement="linear", reps=1)
 
         qc = QuantumCircuit(num_inputs)
         qc.append(feature_map, range(num_inputs))
         qc.append(ansatz, range(num_inputs))
 
@@ -107,17 +110,20 @@
             input_params=feature_map.parameters,
             weight_params=ansatz.parameters,
             input_gradients=True,  # for hybrid qnn
         )
         return qnn
 
     def _create_sampler_qnn(self) -> SamplerQNN:
-        output_shape, interpret = 2, lambda x: f"{x:b}".count("1") % 2
+        output_shape = 2
         num_inputs = 2
 
+        def interpret(x):
+            return f"{x:b}".count("1") % 2
+
         feature_map = ZZFeatureMap(num_inputs)
         ansatz = RealAmplitudes(num_inputs, entanglement="linear", reps=1)
 
         qc = QuantumCircuit(num_inputs)
         qc.append(feature_map, range(num_inputs))
         qc.append(ansatz, range(num_inputs))
```

### Comparing `qiskit-machine-learning-0.6.0/test/datasets/__init__.py` & `qiskit-machine-learning-0.6.1/test/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/datasets/ad_hoc_ref.json` & `qiskit-machine-learning-0.6.1/test/datasets/ad_hoc_ref.json`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/datasets/test_ad_hoc_data.py` & `qiskit-machine-learning-0.6.1/test/datasets/test_ad_hoc_data.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/kernels/algorithms/test_fidelity_qkernel_trainer.py` & `qiskit-machine-learning-0.6.1/test/kernels/algorithms/test_fidelity_qkernel_trainer.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/kernels/algorithms/test_qkernel_trainer.py` & `qiskit-machine-learning-0.6.1/test/kernels/algorithms/test_qkernel_trainer.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/kernels/test_deprecated_qkernel_methods.py` & `qiskit-machine-learning-0.6.1/test/kernels/test_deprecated_qkernel_methods.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/kernels/test_fidelity_qkernel.py` & `qiskit-machine-learning-0.6.1/test/kernels/test_fidelity_qkernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2021, 2022.
+# (C) Copyright IBM 2021, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -60,21 +60,21 @@
 
         self.sample_test = np.asarray([[2.199114860, 5.15221195], [0.50265482, 0.06283185]])
         self.label_test = np.asarray([0, 1])
 
         self.sampler = Sampler()
         self.fidelity = ComputeUncompute(self.sampler)
 
-        self.properties = dict(
-            samples_1=self.sample_train[0],
-            samples_4=self.sample_train,
-            samples_test=self.sample_test,
-            z_fm=self.feature_map,
-            no_fm=None,
-        )
+        self.properties = {
+            "samples_1": self.sample_train[0],
+            "samples_4": self.sample_train,
+            "samples_test": self.sample_test,
+            "z_fm": self.feature_map,
+            "no_fm": None,
+        }
 
     def test_svc_callable(self):
         """Test callable kernel in sklearn."""
         kernel = FidelityQuantumKernel(feature_map=self.feature_map)
         svc = SVC(kernel=kernel.evaluate)
         svc.fit(self.sample_train, self.label_train)
         score = svc.score(self.sample_test, self.label_test)
```

### Comparing `qiskit-machine-learning-0.6.0/test/kernels/test_fidelity_statevector_kernel.py` & `qiskit-machine-learning-0.6.1/test/kernels/test_fidelity_statevector_kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,21 @@
 
         self.sample_test = np.asarray([[2.199114860, 5.15221195], [0.50265482, 0.06283185]])
         self.label_test = np.asarray([0, 1])
 
         self.sampler = Sampler()
         self.fidelity = ComputeUncompute(self.sampler)
 
-        self.properties = dict(
-            samples_1=self.sample_train[0],
-            samples_4=self.sample_train,
-            samples_test=self.sample_test,
-            z_fm=self.feature_map,
-            no_fm=None,
-        )
+        self.properties = {
+            "samples_1": self.sample_train[0],
+            "samples_4": self.sample_train,
+            "samples_test": self.sample_test,
+            "z_fm": self.feature_map,
+            "no_fm": None,
+        }
 
     def test_svc_callable(self):
         """Test callable kernel in sklearn."""
         kernel = FidelityStatevectorKernel(feature_map=self.feature_map)
         svc = SVC(kernel=kernel.evaluate)
         svc.fit(self.sample_train, self.label_train)
         score = svc.score(self.sample_test, self.label_test)
```

### Comparing `qiskit-machine-learning-0.6.0/test/kernels/test_new_vs_old_kernel.py` & `qiskit-machine-learning-0.6.1/test/kernels/test_new_vs_old_kernel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2021, 2022.
+# (C) Copyright IBM 2021, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -38,21 +38,21 @@
     def setUp(self):
         super().setUp()
         warnings.filterwarnings("ignore", category=DeprecationWarning)
         warnings.filterwarnings("ignore", category=PendingDeprecationWarning)
         algorithm_globals.random_seed = 10598
 
         self.statevector_simulator = QuantumInstance(BasicAer.get_backend("statevector_simulator"))
-        self.properties = dict(
-            z1=ZFeatureMap(1),
-            z2=ZFeatureMap(2),
-            zz2=ZZFeatureMap(2),
-            z4=ZFeatureMap(4),
-            zz4=ZZFeatureMap(4),
-        )
+        self.properties = {
+            "z1": ZFeatureMap(1),
+            "z2": ZFeatureMap(2),
+            "zz2": ZZFeatureMap(2),
+            "z4": ZFeatureMap(4),
+            "zz4": ZZFeatureMap(4),
+        }
 
     def tearDown(self) -> None:
         super().tearDown()
         warnings.filterwarnings("always", category=DeprecationWarning)
         warnings.filterwarnings("always", category=PendingDeprecationWarning)
 
     @idata(
```

### Comparing `qiskit-machine-learning-0.6.0/test/kernels/test_new_vs_old_kernel_sv.py` & `qiskit-machine-learning-0.6.1/test/kernels/test_new_vs_old_kernel_sv.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,21 +37,21 @@
     def setUp(self):
         super().setUp()
         warnings.filterwarnings("ignore", category=DeprecationWarning)
         warnings.filterwarnings("ignore", category=PendingDeprecationWarning)
         algorithm_globals.random_seed = 10598
 
         self.statevector_simulator = QuantumInstance(BasicAer.get_backend("statevector_simulator"))
-        self.properties = dict(
-            z1=ZFeatureMap(1),
-            z2=ZFeatureMap(2),
-            zz2=ZZFeatureMap(2),
-            z4=ZFeatureMap(4),
-            zz4=ZZFeatureMap(4),
-        )
+        self.properties = {
+            "z1": ZFeatureMap(1),
+            "z2": ZFeatureMap(2),
+            "zz2": ZZFeatureMap(2),
+            "z4": ZFeatureMap(4),
+            "zz4": ZZFeatureMap(4),
+        }
 
     def tearDown(self) -> None:
         super().tearDown()
         warnings.filterwarnings("always", category=DeprecationWarning)
         warnings.filterwarnings("always", category=PendingDeprecationWarning)
 
     @idata(
```

### Comparing `qiskit-machine-learning-0.6.0/test/kernels/test_qkernel.py` & `qiskit-machine-learning-0.6.1/test/kernels/test_qkernel.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/kernels/test_trainable_fidelity_qkernel.py` & `qiskit-machine-learning-0.6.1/test/kernels/test_trainable_fidelity_qkernel.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/machine_learning_test_case.py` & `qiskit-machine-learning-0.6.1/test/machine_learning_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/neural_networks/test_circuit_qnn.py` & `qiskit-machine-learning-0.6.1/test/neural_networks/test_circuit_qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/neural_networks/test_circuit_vs_sampler_qnn.py` & `qiskit-machine-learning-0.6.1/test/neural_networks/test_circuit_vs_sampler_qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/neural_networks/test_effective_dimension.py` & `qiskit-machine-learning-0.6.1/test/neural_networks/test_effective_dimension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2022.
+# (C) Copyright IBM 2022, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -217,15 +217,15 @@
         """Test that QiskitMachineLearningError is raised for wrong parameters sizes."""
 
         qnn = self.qnns["circuit1"]
 
         num_inputs, num_params = 10, 10
         inputs_ok = algorithm_globals.random.uniform(0, 1, size=(num_inputs, qnn.num_inputs))
         weights_ok = algorithm_globals.random.uniform(0, 1, size=(1, qnn.num_weights))
-        weights_ok2 = algorithm_globals.random.uniform(0, 1, size=(qnn.num_weights))
+        weights_ok2 = algorithm_globals.random.uniform(0, 1, size=qnn.num_weights)
         weights_wrong = algorithm_globals.random.uniform(0, 1, size=(num_params, qnn.num_weights))
 
         LocalEffectiveDimension(
             qnn=qnn,
             weight_samples=weights_ok,
             input_samples=inputs_ok,
         )
```

### Comparing `qiskit-machine-learning-0.6.0/test/neural_networks/test_effective_dimension_primitives.py` & `qiskit-machine-learning-0.6.1/test/neural_networks/test_effective_dimension_primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2022.
+# (C) Copyright IBM 2022, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -199,15 +199,15 @@
         """Test that QiskitMachineLearningError is raised for wrong parameters sizes."""
 
         qnn = self.qnns["sampler_qnn_1"]
 
         num_inputs, num_params = 10, 10
         inputs_ok = algorithm_globals.random.uniform(0, 1, size=(num_inputs, qnn.num_inputs))
         weights_ok = algorithm_globals.random.uniform(0, 1, size=(1, qnn.num_weights))
-        weights_ok2 = algorithm_globals.random.uniform(0, 1, size=(qnn.num_weights))
+        weights_ok2 = algorithm_globals.random.uniform(0, 1, size=qnn.num_weights)
         weights_wrong = algorithm_globals.random.uniform(0, 1, size=(num_params, qnn.num_weights))
 
         LocalEffectiveDimension(
             qnn=qnn,
             weight_samples=weights_ok,
             input_samples=inputs_ok,
         )
```

### Comparing `qiskit-machine-learning-0.6.0/test/neural_networks/test_estimator_qnn.py` & `qiskit-machine-learning-0.6.1/test/neural_networks/test_estimator_qnn.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2022.
+# (C) Copyright IBM 2022, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -18,158 +18,158 @@
 
 import numpy as np
 from qiskit.circuit import Parameter, QuantumCircuit
 from qiskit.quantum_info import SparsePauliOp
 
 from qiskit_machine_learning.neural_networks.estimator_qnn import EstimatorQNN
 
-CASE_DATA = dict(
-    shape_1_1=dict(
-        test_data=[1, [1], [[1], [2]], [[[1], [2]], [[3], [4]]]],
-        weights=[1],
-        correct_forwards=[
+CASE_DATA = {
+    "shape_1_1": {
+        "test_data": [1, [1], [[1], [2]], [[[1], [2]], [[3], [4]]]],
+        "weights": [1],
+        "correct_forwards": [
             [[0.08565359]],
             [[0.08565359]],
             [[0.08565359], [-0.90744233]],
             [[[0.08565359], [-0.90744233]], [[-1.06623996], [-0.24474149]]],
         ],
-        correct_weight_backwards=[
+        "correct_weight_backwards": [
             [[[0.70807342]]],
             [[[0.70807342]]],
             [[[0.70807342]], [[0.7651474]]],
             [[[[0.70807342]], [[0.7651474]]], [[[0.11874839]], [[-0.63682734]]]],
         ],
-        correct_input_backwards=[
+        "correct_input_backwards": [
             [[[-1.13339757]]],
             [[[-1.13339757]]],
             [[[-1.13339757]], [[-0.68445233]]],
             [[[[-1.13339757]], [[-0.68445233]]], [[[0.39377522]], [[1.10996765]]]],
         ],
-    ),
-    shape_2_1=dict(
-        test_data=[[1, 2], [[1, 2]], [[1, 2], [3, 4]]],
-        weights=[1, 2],
-        correct_forwards=[
+    },
+    "shape_2_1": {
+        "test_data": [[1, 2], [[1, 2]], [[1, 2], [3, 4]]],
+        "weights": [1, 2],
+        "correct_forwards": [
             [[0.41256026]],
             [[0.41256026]],
             [[0.41256026], [0.72848859]],
         ],
-        correct_weight_backwards=[
+        "correct_weight_backwards": [
             [[[0.12262287, -0.17203964]]],
             [[[0.12262287, -0.17203964]]],
             [[[0.12262287, -0.17203964]], [[0.03230095, -0.04531817]]],
         ],
-        correct_input_backwards=[
+        "correct_input_backwards": [
             [[[-0.81570272, -0.39688474]]],
             [[[-0.81570272, -0.39688474]]],
             [[[-0.81570272, -0.39688474]], [[0.25229775, 0.67111573]]],
         ],
-    ),
-    shape_1_2=dict(
-        test_data=[
+    },
+    "shape_1_2": {
+        "test_data": [
             [1],
             [[1], [2]],
             [[[1], [2]], [[3], [4]]],
         ],
-        weights=[1],
-        correct_forwards=[
+        "weights": [1],
+        "correct_forwards": [
             [[0.08565359, 0.17130718]],
             [[0.08565359, 0.17130718], [-0.90744233, -1.81488467]],
             [
                 [[0.08565359, 0.17130718], [-0.90744233, -1.81488467]],
                 [[-1.06623996, -2.13247992], [-0.24474149, -0.48948298]],
             ],
         ],
-        correct_weight_backwards=[
+        "correct_weight_backwards": [
             [[[0.70807342], [1.41614684]]],
             [[[0.70807342], [1.41614684]], [[0.7651474], [1.5302948]]],
             [
                 [[[0.70807342], [1.41614684]], [[0.7651474], [1.5302948]]],
                 [[[0.11874839], [0.23749678]], [[-0.63682734], [-1.27365468]]],
             ],
         ],
-        correct_input_backwards=[
+        "correct_input_backwards": [
             [[[-1.13339757], [-2.26679513]]],
             [[[-1.13339757], [-2.26679513]], [[-0.68445233], [-1.36890466]]],
             [
                 [[[-1.13339757], [-2.26679513]], [[-0.68445233], [-1.36890466]]],
                 [[[0.39377522], [0.78755044]], [[1.10996765], [2.2199353]]],
             ],
         ],
-    ),
-    shape_2_2=dict(
-        test_data=[[1, 2], [[1, 2], [3, 4]]],
-        weights=[1, 2],
-        correct_forwards=[
+    },
+    "shape_2_2": {
+        "test_data": [[1, 2], [[1, 2], [3, 4]]],
+        "weights": [1, 2],
+        "correct_forwards": [
             [[-0.07873524, 0.4912955]],
             [[-0.07873524, 0.4912955], [-0.0207402, 0.74922879]],
         ],
-        correct_weight_backwards=[
+        "correct_weight_backwards": [
             [[[0.12262287, -0.17203964], [0, 0]]],
             [[[0.12262287, -0.17203964], [0, 0]], [[0.03230095, -0.04531817], [0, 0]]],
         ],
-        correct_input_backwards=[
+        "correct_input_backwards": [
             [[[-0.05055532, -0.17203964], [-0.7651474, -0.2248451]]],
             [
                 [[-0.05055532, -0.17203964], [-0.7651474, -0.2248451]],
                 [[0.14549777, 0.02401345], [0.10679997, 0.64710228]],
             ],
         ],
-    ),
-    no_input_parameters=dict(
-        test_data=[None],
-        weights=[1, 1],
-        correct_forwards=[[[0.08565359]]],
-        correct_weight_backwards=[[[[-1.13339757, 0.70807342]]]],
-        correct_input_backwards=[None],
-    ),
-    no_weight_parameters=dict(
-        test_data=[[1, 1]],
-        weights=None,
-        correct_forwards=[[[0.08565359]]],
-        correct_weight_backwards=[None],
-        correct_input_backwards=[[[[-1.13339757, 0.70807342]]]],
-    ),
-    no_parameters=dict(
-        test_data=[None],
-        weights=None,
-        correct_forwards=[[[1]]],
-        correct_weight_backwards=[None],
-        correct_input_backwards=[None],
-    ),
-    default_observables=dict(
-        test_data=[[[1], [2]]],
-        weights=[1],
-        correct_forwards=[[[-0.45464871], [-0.4912955]]],
-        correct_weight_backwards=[[[[0.70807342]], [[0.7651474]]]],
-        correct_input_backwards=[[[[-0.29192658]], [[0.2248451]]]],
-    ),
-    single_observable=dict(
-        test_data=[1, [1], [[1], [2]], [[[1], [2]], [[3], [4]]]],
-        weights=[1],
-        correct_forwards=[
+    },
+    "no_input_parameters": {
+        "test_data": [None],
+        "weights": [1, 1],
+        "correct_forwards": [[[0.08565359]]],
+        "correct_weight_backwards": [[[[-1.13339757, 0.70807342]]]],
+        "correct_input_backwards": [None],
+    },
+    "no_weight_parameters": {
+        "test_data": [[1, 1]],
+        "weights": None,
+        "correct_forwards": [[[0.08565359]]],
+        "correct_weight_backwards": [None],
+        "correct_input_backwards": [[[[-1.13339757, 0.70807342]]]],
+    },
+    "no_parameters": {
+        "test_data": [None],
+        "weights": None,
+        "correct_forwards": [[[1]]],
+        "correct_weight_backwards": [None],
+        "correct_input_backwards": [None],
+    },
+    "default_observables": {
+        "test_data": [[[1], [2]]],
+        "weights": [1],
+        "correct_forwards": [[[-0.45464871], [-0.4912955]]],
+        "correct_weight_backwards": [[[[0.70807342]], [[0.7651474]]]],
+        "correct_input_backwards": [[[[-0.29192658]], [[0.2248451]]]],
+    },
+    "single_observable": {
+        "test_data": [1, [1], [[1], [2]], [[[1], [2]], [[3], [4]]]],
+        "weights": [1],
+        "correct_forwards": [
             [[0.08565359]],
             [[0.08565359]],
             [[0.08565359], [-0.90744233]],
             [[[0.08565359], [-0.90744233]], [[-1.06623996], [-0.24474149]]],
         ],
-        correct_weight_backwards=[
+        "correct_weight_backwards": [
             [[[0.70807342]]],
             [[[0.70807342]]],
             [[[0.70807342]], [[0.7651474]]],
             [[[[0.70807342]], [[0.7651474]]], [[[0.11874839]], [[-0.63682734]]]],
         ],
-        correct_input_backwards=[
+        "correct_input_backwards": [
             [[[-1.13339757]]],
             [[[-1.13339757]]],
             [[[-1.13339757]], [[-0.68445233]]],
             [[[[-1.13339757]], [[-0.68445233]]], [[[0.39377522]], [[1.10996765]]]],
         ],
-    ),
-)
+    },
+}
 
 
 class TestEstimatorQNN(QiskitMachineLearningTestCase):
     """EstimatorQNN Tests. The correct references is obtained from OpflowQNN"""
 
     def _test_network_passes(
         self,
```

### Comparing `qiskit-machine-learning-0.6.0/test/neural_networks/test_neural_network.py` & `qiskit-machine-learning-0.6.1/test/neural_networks/test_neural_network.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/neural_networks/test_opflow_qnn.py` & `qiskit-machine-learning-0.6.1/test/neural_networks/test_opflow_qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/neural_networks/test_sampler_qnn.py` & `qiskit-machine-learning-0.6.1/test/neural_networks/test_sampler_qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/neural_networks/test_two_layer_qnn.py` & `qiskit-machine-learning-0.6.1/test/neural_networks/test_two_layer_qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/runtime/fake_torchruntime.py` & `qiskit-machine-learning-0.6.1/test/runtime/fake_torchruntime.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/runtime/test_torch_runtime_client.py` & `qiskit-machine-learning-0.6.1/test/runtime/test_torch_runtime_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/test_deprecation.py` & `qiskit-machine-learning-0.6.1/test/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/test_readme_sample.py` & `qiskit-machine-learning-0.6.1/test/test_readme_sample.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/utils/loss_functions/test_loss_functions.py` & `qiskit-machine-learning-0.6.1/test/utils/loss_functions/test_loss_functions.py`

 * *Files identical despite different names*

### Comparing `qiskit-machine-learning-0.6.0/test/utils/test_adjust_num_qubits.py` & `qiskit-machine-learning-0.6.1/test/utils/test_adjust_num_qubits.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2022.
+# (C) Copyright IBM 2022, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -24,17 +24,20 @@
 
 @ddt
 class TestAdjustNumQubits(QiskitMachineLearningTestCase):
     """Tests for the derive_num_qubits_feature_map_ansatz function."""
 
     def setUp(self) -> None:
         super().setUp()
-        self.properties = dict(
-            z1=ZFeatureMap(1), z2=ZFeatureMap(2), ra1=RealAmplitudes(1), ra2=RealAmplitudes(2)
-        )
+        self.properties = {
+            "z1": ZFeatureMap(1),
+            "z2": ZFeatureMap(2),
+            "ra1": RealAmplitudes(1),
+            "ra2": RealAmplitudes(2),
+        }
 
     def test_all_none(self):
         """Test when all parameters are ``None``."""
         self.assertRaises(
             QiskitMachineLearningError, derive_num_qubits_feature_map_ansatz, None, None, None
         )
```

