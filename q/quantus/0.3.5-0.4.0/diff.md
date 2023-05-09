# Comparing `tmp/quantus-0.3.5.tar.gz` & `tmp/quantus-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantus-0.3.5.tar", last modified: Wed Apr  5 09:48:06 2023, max compression
+gzip compressed data, was "quantus-0.4.0.tar", last modified: Tue May  9 20:55:45 2023, max compression
```

## Comparing `quantus-0.3.5.tar` & `quantus-0.4.0.tar`

### file list

```diff
@@ -1,118 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.884597 quantus-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-05 09:47:55.000000 quantus-0.3.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-05 09:47:55.000000 quantus-0.3.5/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-05 09:47:55.000000 quantus-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29660 2023-04-05 09:48:06.884597 quantus-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28962 2023-04-05 09:47:55.000000 quantus-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.872597 quantus-0.3.5/quantus/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.872597 quantus-0.3.5/quantus/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/functions/discretise_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    32812 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/functions/explanation_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/functions/loss_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/functions/mosaic_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/functions/norm_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/functions/normalise_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    16936 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/functions/perturb_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/functions/similarity_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.876597 quantus-0.3.5/quantus/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/helpers/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/helpers/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.876597 quantus-0.3.5/quantus/helpers/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/helpers/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/helpers/model/model_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/helpers/model/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/helpers/model/pytorch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16081 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/helpers/model/tf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/helpers/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    32190 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/helpers/warn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.876597 quantus-0.3.5/quantus/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.876597 quantus-0.3.5/quantus/metrics/axiomatic/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/axiomatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/axiomatic/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/axiomatic/input_invariance.py
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/axiomatic/non_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    33101 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/base_batched.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.876597 quantus-0.3.5/quantus/metrics/complexity/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/complexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/complexity/complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/complexity/effective_complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/complexity/sparseness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.880597 quantus-0.3.5/quantus/metrics/faithfulness/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/faithfulness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15554 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/faithfulness/faithfulness_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/faithfulness/faithfulness_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16959 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/faithfulness/infidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/faithfulness/irof.py
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/faithfulness/monotonicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/faithfulness/monotonicity_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/faithfulness/pixel_flipping.py
--rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/faithfulness/region_perturbation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15473 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/faithfulness/road.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/faithfulness/selectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/faithfulness/sensitivity_n.py
--rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/faithfulness/sufficiency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.880597 quantus-0.3.5/quantus/metrics/localisation/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/localisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/localisation/attribution_localisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/localisation/auc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/localisation/focus.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/localisation/pointing_game.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/localisation/relevance_mass_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/localisation/relevance_rank_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/localisation/top_k_intersection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.880597 quantus-0.3.5/quantus/metrics/randomisation/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/randomisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17093 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/randomisation/model_parameter_randomisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/randomisation/random_logit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.880597 quantus-0.3.5/quantus/metrics/robustness/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/robustness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17232 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/robustness/avg_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/robustness/consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    18914 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/robustness/continuity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/robustness/local_lipschitz_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/robustness/max_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14250 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/robustness/relative_input_stability.py
--rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/robustness/relative_output_stability.py
--rw-r--r--   0 runner    (1001) docker     (123)    15810 2023-04-05 09:47:55.000000 quantus-0.3.5/quantus/metrics/robustness/relative_representation_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.872597 quantus-0.3.5/quantus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29660 2023-04-05 09:48:06.000000 quantus-0.3.5/quantus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-05 09:48:06.000000 quantus-0.3.5/quantus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:48:06.000000 quantus-0.3.5/quantus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:48:06.000000 quantus-0.3.5/quantus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-05 09:48:06.000000 quantus-0.3.5/quantus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-05 09:48:06.000000 quantus-0.3.5/quantus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 09:48:06.884597 quantus-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-05 09:47:55.000000 quantus-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.880597 quantus-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.884597 quantus-0.3.5/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34140 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/helpers/test_explanation_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/helpers/test_loss_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/helpers/test_mosaic_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/helpers/test_norm_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/helpers/test_normalise_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/helpers/test_perturb_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/helpers/test_pytorch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/helpers/test_similarity_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/helpers/test_tf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31385 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/helpers/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:06.884597 quantus-0.3.5/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/metrics/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    21122 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/metrics/test_axiomatic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    16673 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/metrics/test_complexity_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    58794 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/metrics/test_faithfulness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    53754 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/metrics/test_localisation_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    15765 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/metrics/test_randomisation_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/metrics/test_relative_stability.py
--rw-r--r--   0 runner    (1001) docker     (123)    30197 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/metrics/test_robustness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-05 09:47:55.000000 quantus-0.3.5/tests/test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.864278 quantus-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 20:55:32.000000 quantus-0.4.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-09 20:55:32.000000 quantus-0.4.0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-09 20:55:32.000000 quantus-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-09 20:55:32.000000 quantus-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-05-09 20:55:45.864278 quantus-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29516 2023-05-09 20:55:32.000000 quantus-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.852278 quantus-0.4.0/quantus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.852278 quantus-0.4.0/quantus/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/discretise_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32857 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/explanation_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/loss_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/mosaic_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/norm_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/normalise_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16936 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/perturb_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/similarity_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.852278 quantus-0.4.0/quantus/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.852278 quantus-0.4.0/quantus/helpers/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/model/model_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/model/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/model/pytorch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16081 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/model/tf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32190 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/warn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.856279 quantus-0.4.0/quantus/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.856279 quantus-0.4.0/quantus/metrics/axiomatic/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/axiomatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/axiomatic/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/axiomatic/input_invariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/axiomatic/non_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33179 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/base_batched.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.856279 quantus-0.4.0/quantus/metrics/complexity/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/complexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/complexity/complexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/complexity/effective_complexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/complexity/sparseness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.856279 quantus-0.4.0/quantus/metrics/faithfulness/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15554 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/faithfulness_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/faithfulness_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16959 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/infidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/irof.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/monotonicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/monotonicity_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/pixel_flipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/region_perturbation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15473 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/road.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/selectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/sensitivity_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/sufficiency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.860278 quantus-0.4.0/quantus/metrics/localisation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/attribution_localisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/focus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/pointing_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/relevance_mass_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/relevance_rank_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/top_k_intersection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.860278 quantus-0.4.0/quantus/metrics/randomisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/randomisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17093 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/randomisation/model_parameter_randomisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/randomisation/random_logit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.860278 quantus-0.4.0/quantus/metrics/robustness/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17232 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/avg_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18914 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/continuity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/local_lipschitz_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/max_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14250 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/relative_input_stability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/relative_output_stability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15810 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/relative_representation_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.852278 quantus-0.4.0/quantus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-05-09 20:55:45.000000 quantus-0.4.0/quantus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-09 20:55:45.000000 quantus-0.4.0/quantus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:55:45.000000 quantus-0.4.0/quantus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:55:45.000000 quantus-0.4.0/quantus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-09 20:55:45.000000 quantus-0.4.0/quantus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 20:55:45.000000 quantus-0.4.0/quantus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-09 20:55:32.000000 quantus-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-09 20:55:32.000000 quantus-0.4.0/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 20:55:45.864278 quantus-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-09 20:55:32.000000 quantus-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.860278 quantus-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.860278 quantus-0.4.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34140 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_explanation_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_loss_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_mosaic_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_norm_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_normalise_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12891 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_perturb_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_pytorch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_similarity_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_tf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31385 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.864278 quantus-0.4.0/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21113 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_axiomatic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16673 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_complexity_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58855 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_faithfulness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53755 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_localisation_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16183 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_randomisation_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_relative_stability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30229 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_robustness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/test_evaluation.py
```

### Comparing `quantus-0.3.5/COPYING` & `quantus-0.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/COPYING.LESSER` & `quantus-0.4.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/PKG-INFO` & `quantus-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: quantus
-Version: 0.3.5
-Summary: A metrics toolkit to evaluate neural network explanations.
+Version: 0.4.0
+Summary: A toolkit to evaluate neural network explanations.
 Home-page: http://github.com/understandable-machine-intelligence-lab/Quantus
 Author: Anna Hedstrom
 Author-email: hedstroem.anna@gmail.com
 License: GNU LESSER GENERAL PUBLIC LICENSE VERSION 3
 Keywords: explainable ai,xai,machine learning,deep learning
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: torch
 Provides-Extra: tensorflow
 Provides-Extra: captum
 Provides-Extra: tf-explain
 Provides-Extra: zennit
-Provides-Extra: tutorials
 Provides-Extra: tests
 Provides-Extra: full
 License-File: LICENSE
 License-File: COPYING
 License-File: COPYING.LESSER
 
 <p align="center">
@@ -29,32 +28,33 @@
 <p align="center">
   PyTorch and TensorFlow
 
 [![Getting started!](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/understandable-machine-intelligence-lab/Quantus/blob/main/tutorials/Tutorial_ImageNet_Example_All_Metrics.ipynb)
 [![Launch Tutorials](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/understandable-machine-intelligence-lab/Quantus/HEAD?labpath=tutorials)
 [![Python package](https://github.com/understandable-machine-intelligence-lab/Quantus/actions/workflows/python-package.yml/badge.svg)](https://github.com/understandable-machine-intelligence-lab/Quantus/actions/workflows/python-package.yml)
 [![Code coverage](https://github.com/understandable-machine-intelligence-lab/Quantus/actions/workflows/codecov.yml/badge.svg)](https://github.com/understandable-machine-intelligence-lab/Quantus/actions/workflows/codecov.yml)
-![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)
+![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)
 [![PyPI version](https://badge.fury.io/py/quantus.svg)](https://badge.fury.io/py/quantus)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation Status](https://readthedocs.org/projects/quantus/badge/?version=latest)](https://quantus.readthedocs.io/en/latest/?badge=latest)
 [![codecov.io](https://codecov.io/github/understandable-machine-intelligence-lab/Quantus/coverage.svg?branch=master)](https://codecov.io/github/understandable-machine-intelligence-lab/Quantus?branch=master)
 [![Downloads](https://static.pepy.tech/badge/quantus)](https://pepy.tech/project/quantus)
 
 _Quantus is currently under active development so carefully note the Quantus release version to ensure reproducibility of your work._
 
 [📑 Shortcut to paper!](https://jmlr.org/papers/volume24/22-0142/22-0142.pdf)
         
 ## News and Highlights! :rocket:
 
-- Accepted to Journal of Machine Learning Research (MLOSS) ([paper](https://jmlr.org/papers/v24/22-0142.html))!
+- Released a new version 0.4.0 that now supports Python 3.10 and 3.11, read more [here](https://github.com/understandable-machine-intelligence-lab/Quantus/releases)!
+- Accepted to Journal of Machine Learning Research (MLOSS), read the [paper](https://jmlr.org/papers/v24/22-0142.html)
 - Offers more than **30+ metrics in 6 categories** for XAI evaluation
 - Supports different data types (image, time-series, tabular, NLP next up!) and models (PyTorch, TensorFlow)
 - Extended built-in support for explanation methods ([captum](https://captum.ai/) and [tf-explain](https://tf-explain.readthedocs.io/en/latest/))
-- New optimisations to help speed up computation, see API reference [here](https://quantus.readthedocs.io/en/latest/docs_api/quantus.metrics.base_batched.html)!
+- New optimisations to help speed up computation, see API reference [here](https://quantus.readthedocs.io/en/latest/docs_api/quantus.metrics.base_batched.html)
 
 See [here](https://github.com/understandable-machine-intelligence-lab/Quantus/releases) for the latest release(s).
 
 ## Citation
 
 If you find this toolkit or its companion paper
 [**Quantus: An Explainable AI Toolkit for Responsible Evaluation of Neural Network Explanations and Beyond**](https://jmlr.org/papers/v24/22-0142.html)
@@ -216,17 +216,18 @@
 For a more in-depth guide on how to install Quantus, please read more [here](https://quantus.readthedocs.io/en/latest/getting_started/installation.html). This includes instructions for how to install a desired deep learning framework such as PyTorch or TensorFlow together with Quantus.
 
 ### Package requirements
 
 The package requirements are as follows:
 ```
 python>=3.7.0
-pytorch>=1.10.1
-TensorFlow==2.6.2
+torch>=1.11.0
+tensorflow>=2.5.0
 ```
+Please note that the exact [PyTorch](https://pytorch.org/) and/ or [TensorFlow](https://www.TensorFlow.org) versions to be installed depends on your Python version (3.7-3.11) and platform (`darwin`, `linux`, …). See `requirements_test.txt` to retrieve the exact versions of [PyTorch](https://pytorch.org/) and/ or [TensorFlow](https://www.TensorFlow.org).
 
 ## Getting started
 
 The following will give a short introduction to how to get started with Quantus. Note that this example is based on the [PyTorch](https://pytorch.org/) framework, but we also support 
 [TensorFlow](https://www.tensorflow.org), which would differ only in the loading of the model, data and explanations. To get started with Quantus, you need:
 * A model (`model`), inputs (`x_batch`) and labels (`y_batch`)
 * Some explanations you want to evaluate (`a_batch`)
```

### Comparing `quantus-0.3.5/README.md` & `quantus-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,32 +6,33 @@
 <p align="center">
   PyTorch and TensorFlow
 
 [![Getting started!](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/understandable-machine-intelligence-lab/Quantus/blob/main/tutorials/Tutorial_ImageNet_Example_All_Metrics.ipynb)
 [![Launch Tutorials](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/understandable-machine-intelligence-lab/Quantus/HEAD?labpath=tutorials)
 [![Python package](https://github.com/understandable-machine-intelligence-lab/Quantus/actions/workflows/python-package.yml/badge.svg)](https://github.com/understandable-machine-intelligence-lab/Quantus/actions/workflows/python-package.yml)
 [![Code coverage](https://github.com/understandable-machine-intelligence-lab/Quantus/actions/workflows/codecov.yml/badge.svg)](https://github.com/understandable-machine-intelligence-lab/Quantus/actions/workflows/codecov.yml)
-![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)
+![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)
 [![PyPI version](https://badge.fury.io/py/quantus.svg)](https://badge.fury.io/py/quantus)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation Status](https://readthedocs.org/projects/quantus/badge/?version=latest)](https://quantus.readthedocs.io/en/latest/?badge=latest)
 [![codecov.io](https://codecov.io/github/understandable-machine-intelligence-lab/Quantus/coverage.svg?branch=master)](https://codecov.io/github/understandable-machine-intelligence-lab/Quantus?branch=master)
 [![Downloads](https://static.pepy.tech/badge/quantus)](https://pepy.tech/project/quantus)
 
 _Quantus is currently under active development so carefully note the Quantus release version to ensure reproducibility of your work._
 
 [📑 Shortcut to paper!](https://jmlr.org/papers/volume24/22-0142/22-0142.pdf)
         
 ## News and Highlights! :rocket:
 
-- Accepted to Journal of Machine Learning Research (MLOSS) ([paper](https://jmlr.org/papers/v24/22-0142.html))!
+- Released a new version 0.4.0 that now supports Python 3.10 and 3.11, read more [here](https://github.com/understandable-machine-intelligence-lab/Quantus/releases)!
+- Accepted to Journal of Machine Learning Research (MLOSS), read the [paper](https://jmlr.org/papers/v24/22-0142.html)
 - Offers more than **30+ metrics in 6 categories** for XAI evaluation
 - Supports different data types (image, time-series, tabular, NLP next up!) and models (PyTorch, TensorFlow)
 - Extended built-in support for explanation methods ([captum](https://captum.ai/) and [tf-explain](https://tf-explain.readthedocs.io/en/latest/))
-- New optimisations to help speed up computation, see API reference [here](https://quantus.readthedocs.io/en/latest/docs_api/quantus.metrics.base_batched.html)!
+- New optimisations to help speed up computation, see API reference [here](https://quantus.readthedocs.io/en/latest/docs_api/quantus.metrics.base_batched.html)
 
 See [here](https://github.com/understandable-machine-intelligence-lab/Quantus/releases) for the latest release(s).
 
 ## Citation
 
 If you find this toolkit or its companion paper
 [**Quantus: An Explainable AI Toolkit for Responsible Evaluation of Neural Network Explanations and Beyond**](https://jmlr.org/papers/v24/22-0142.html)
@@ -193,17 +194,18 @@
 For a more in-depth guide on how to install Quantus, please read more [here](https://quantus.readthedocs.io/en/latest/getting_started/installation.html). This includes instructions for how to install a desired deep learning framework such as PyTorch or TensorFlow together with Quantus.
 
 ### Package requirements
 
 The package requirements are as follows:
 ```
 python>=3.7.0
-pytorch>=1.10.1
-TensorFlow==2.6.2
+torch>=1.11.0
+tensorflow>=2.5.0
 ```
+Please note that the exact [PyTorch](https://pytorch.org/) and/ or [TensorFlow](https://www.TensorFlow.org) versions to be installed depends on your Python version (3.7-3.11) and platform (`darwin`, `linux`, …). See `requirements_test.txt` to retrieve the exact versions of [PyTorch](https://pytorch.org/) and/ or [TensorFlow](https://www.TensorFlow.org).
 
 ## Getting started
 
 The following will give a short introduction to how to get started with Quantus. Note that this example is based on the [PyTorch](https://pytorch.org/) framework, but we also support 
 [TensorFlow](https://www.tensorflow.org), which would differ only in the loading of the model, data and explanations. To get started with Quantus, you need:
 * A model (`model`), inputs (`x_batch`) and labels (`y_batch`)
 * Some explanations you want to evaluate (`a_batch`)
```

### Comparing `quantus-0.3.5/quantus/__init__.py` & `quantus-0.4.0/quantus/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/evaluation.py` & `quantus-0.4.0/quantus/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,17 +132,15 @@
             )
             a_batch = utils.expand_attribution_channel(a_batch, x_batch)
 
             # Asserts.
             asserts.assert_attributions(a_batch=a_batch, x_batch=x_batch)
 
         elif isinstance(value, np.ndarray):
-            explain_funcs[
-                method
-            ] = explain
+            explain_funcs[method] = explain
             a_batch = value
 
         else:
 
             raise TypeError(
                 "xai_methods type is not in: Dict[str, Callable], Dict[str, Dict], Dict[str, np.ndarray]."
             )
```

### Comparing `quantus-0.3.5/quantus/functions/discretise_func.py` & `quantus-0.4.0/quantus/functions/discretise_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/functions/explanation_func.py` & `quantus-0.4.0/quantus/functions/explanation_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
             channel_first: boolean, optional
                 Indicates if the image dimensions are channel first, or channel last.
                 Inferred from the input shape if None.
             reduce_axes: tuple
                 Indicates the indices of dimensions of the output explanation array to be summed. For example, an input
                 array of shape (8, 28, 28, 3) with keepdims=True and reduce_axes = (-1,) will return an array of shape
                 (8, 28, 28, -1). Passing "()" will keep
-                the original dimensions. 
+                the original dimensions.
             keepdims: boolean
                 Indicated if the reduced axes shall be preserved (True) or removed (False).
     Returns
     -------
     explanation: np.ndarray
          Returns np.ndarray of same shape as inputs.
 
@@ -509,15 +509,18 @@
         "reduce_axes", [1]
     ), "Reduction over batch_axis is not available, please do not include axis 0 in 'reduce_axes' kwargs."
     assert len(kwargs.get("reduce_axes", [1])) <= inputs.ndim - 1, (
         "Cannot reduce attributions over more axes than each sample has dimensions, but got "
         "{} and  {}.".format(len(kwargs.get("reduce_axes", [1])), inputs.ndim - 1)
     )
 
-    reduce_axes = {"axis": tuple(kwargs.get("reduce_axes", [1])), "keepdims": kwargs.get("keepdims", True)}
+    reduce_axes = {
+        "axis": tuple(kwargs.get("reduce_axes", [1])),
+        "keepdims": kwargs.get("keepdims", True),
+    }
 
     # Prevent attribution summation for 2D-data. Recreate np.sum behavior when passing reduce_axes=(), i.e. no change.
     if (len(tuple(kwargs.get("reduce_axes", [1]))) == 0) | (inputs.ndim < 3):
 
         def f_reduce_axes(a):
             return a
 
@@ -751,15 +754,18 @@
         "reduce_axes", [1]
     ), "Reduction over batch_axis is not available, please do not include axis 0 in 'reduce_axes' kwarg."
     assert len(kwargs.get("reduce_axes", [1])) <= inputs.ndim - 1, (
         "Cannot reduce attributions over more axes than each sample has dimensions, but got "
         "{} and  {}.".format(len(kwargs.get("reduce_axes", [1])), inputs.ndim - 1)
     )
 
-    reduce_axes = {"axis": tuple(kwargs.get("reduce_axes", [1])), "keepdims": kwargs.get("keepdims", True)}
+    reduce_axes = {
+        "axis": tuple(kwargs.get("reduce_axes", [1])),
+        "keepdims": kwargs.get("keepdims", True),
+    }
 
     # Get zennit composite, canonizer, attributor and handle canonizer kwargs.
     canonizer = kwargs.get("canonizer", None)
     if not canonizer == None and not issubclass(canonizer, zcanon.Canonizer):
         raise ValueError(
             "The specified canonizer is not valid. "
             "Please provide None or an instance of zennit.canonizers.Canonizer"
```

### Comparing `quantus-0.3.5/quantus/functions/loss_func.py` & `quantus-0.4.0/quantus/functions/loss_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/functions/mosaic_func.py` & `quantus-0.4.0/quantus/functions/mosaic_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/functions/norm_func.py` & `quantus-0.4.0/quantus/functions/norm_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/functions/normalise_func.py` & `quantus-0.4.0/quantus/functions/normalise_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/functions/perturb_func.py` & `quantus-0.4.0/quantus/functions/perturb_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/functions/similarity_func.py` & `quantus-0.4.0/quantus/functions/similarity_func.py`

 * *Files 4% similar despite different names*

```diff
@@ -237,16 +237,20 @@
         Keyword arguments.
 
     Returns
     -------
     float
         The similarity score.
     """
+    max_point, min_point = np.max(np.concatenate([a, b])), np.min(
+        np.concatenate([a, b])
+    )
+    data_range = float(np.abs(max_point - min_point))
     return skimage.metrics.structural_similarity(
-        im1=a, im2=b, win_size=kwargs.get("win_size", None)
+        im1=a, im2=b, win_size=kwargs.get("win_size", None), data_range=data_range
     )
 
 
 def difference(a: np.array, b: np.array, **kwargs) -> float:
     """
     Calculate the difference between two images (or explanations).
```

### Comparing `quantus-0.3.5/quantus/helpers/__init__.py` & `quantus-0.4.0/quantus/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/helpers/asserts.py` & `quantus-0.4.0/quantus/helpers/asserts.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/helpers/constants.py` & `quantus-0.4.0/quantus/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/helpers/model/model_interface.py` & `quantus-0.4.0/quantus/helpers/model/model_interface.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/helpers/model/models.py` & `quantus-0.4.0/quantus/helpers/model/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,17 +228,19 @@
     def CifarCNNModel() -> tf.keras.Model:
         """
         Source: https://www.tensorflow.org/tutorials/images/cnn
         """
 
         return tf.keras.Sequential(
             [
-                tf.keras.layers.Conv2D(32, (3, 3), activation='relu', input_shape=(32, 32, 3)),
+                tf.keras.layers.Conv2D(
+                    32, (3, 3), activation="relu", input_shape=(32, 32, 3)
+                ),
                 tf.keras.layers.MaxPooling2D((2, 2)),
-                tf.keras.layers.Conv2D(64, (3, 3), activation='relu'),
+                tf.keras.layers.Conv2D(64, (3, 3), activation="relu"),
                 tf.keras.layers.MaxPooling2D((2, 2)),
-                tf.keras.layers.Conv2D(64, (3, 3), activation='relu'),
+                tf.keras.layers.Conv2D(64, (3, 3), activation="relu"),
                 tf.keras.layers.Flatten(),
-                tf.keras.layers.Dense(64, activation='relu'),
+                tf.keras.layers.Dense(64, activation="relu"),
                 tf.keras.layers.Dense(10),
             ]
         )
```

### Comparing `quantus-0.3.5/quantus/helpers/model/pytorch_model.py` & `quantus-0.4.0/quantus/helpers/model/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/helpers/model/tf_model.py` & `quantus-0.4.0/quantus/helpers/model/tf_model.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/helpers/plotting.py` & `quantus-0.4.0/quantus/helpers/plotting.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/helpers/utils.py` & `quantus-0.4.0/quantus/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/helpers/warn.py` & `quantus-0.4.0/quantus/helpers/warn.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,28 +242,28 @@
 
     if text != "\n":
         print(text)
 
 
 def warn_perturbation_caused_no_change(x: np.ndarray, x_perturbed: np.ndarray) -> None:
     """
-    Warn that perturbation applied to input caused change so that input and perturbed input is not the same.
+    Warn that perturbation applied to input caused no change so that input and perturbed input is the same.
 
     Parameters
     ----------
     x: np.ndarray
          The original input that is considered unperturbed.
     x_perturbed: np.ndarray
          The perturbed input.
 
     Returns
     -------
     None
     """
-    if (x.flatten() != x_perturbed.flatten()).any():
+    if np.allclose(x, x_perturbed, equal_nan=True):
         warnings.warn(
             "The settings for perturbing input e.g., 'perturb_func' "
             "didn't cause change in input. "
             "Reconsider the parameter settings."
         )
```

### Comparing `quantus-0.3.5/quantus/metrics/__init__.py` & `quantus-0.4.0/quantus/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/axiomatic/__init__.py` & `quantus-0.4.0/quantus/metrics/axiomatic/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/axiomatic/completeness.py` & `quantus-0.4.0/quantus/metrics/axiomatic/completeness.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/axiomatic/input_invariance.py` & `quantus-0.4.0/quantus/metrics/axiomatic/input_invariance.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/axiomatic/non_sensitivity.py` & `quantus-0.4.0/quantus/metrics/axiomatic/non_sensitivity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/base.py` & `quantus-0.4.0/quantus/metrics/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -675,28 +675,28 @@
         any
             Can be implemented, optionally by the child class.
         """
         pass
 
     def plot(
         self,
-        plot_func: Callable,
+        plot_func: Optional[Callable] = None,
         show: bool = True,
         path_to_save: Union[str, None] = None,
         *args,
         **kwargs,
     ) -> None:
         """
         Basic plotting functionality for Metric class.
         The user provides a plot_func (Callable) that contains the actual plotting logic (but returns None).
 
         Parameters
         ----------
         plot_func: callable
-            A Callable with the actual plotting logic.
+            A Callable with the actual plotting logic. Default set to None, which implies default_plot_func is set.
         show: boolean
             A boolean to state if the plot shall be shown.
         path_to_save (str):
             A string that specifies the path to save file.
         args: optional
             An optional with additional arguments.
         kwargs: optional
```

### Comparing `quantus-0.3.5/quantus/metrics/base_batched.py` & `quantus-0.4.0/quantus/metrics/base_batched.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/complexity/__init__.py` & `quantus-0.4.0/quantus/metrics/complexity/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/complexity/complexity.py` & `quantus-0.4.0/quantus/metrics/complexity/complexity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/complexity/effective_complexity.py` & `quantus-0.4.0/quantus/metrics/complexity/effective_complexity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/complexity/sparseness.py` & `quantus-0.4.0/quantus/metrics/complexity/sparseness.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/faithfulness/__init__.py` & `quantus-0.4.0/quantus/metrics/faithfulness/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/faithfulness/faithfulness_correlation.py` & `quantus-0.4.0/quantus/metrics/faithfulness/faithfulness_correlation.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/faithfulness/faithfulness_estimate.py` & `quantus-0.4.0/quantus/metrics/faithfulness/faithfulness_estimate.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/faithfulness/infidelity.py` & `quantus-0.4.0/quantus/metrics/faithfulness/infidelity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/faithfulness/irof.py` & `quantus-0.4.0/quantus/metrics/faithfulness/irof.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/faithfulness/monotonicity.py` & `quantus-0.4.0/quantus/metrics/faithfulness/monotonicity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/faithfulness/monotonicity_correlation.py` & `quantus-0.4.0/quantus/metrics/faithfulness/monotonicity_correlation.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/faithfulness/pixel_flipping.py` & `quantus-0.4.0/quantus/metrics/faithfulness/pixel_flipping.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/faithfulness/region_perturbation.py` & `quantus-0.4.0/quantus/metrics/faithfulness/region_perturbation.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/faithfulness/road.py` & `quantus-0.4.0/quantus/metrics/faithfulness/road.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/faithfulness/selectivity.py` & `quantus-0.4.0/quantus/metrics/faithfulness/selectivity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/faithfulness/sensitivity_n.py` & `quantus-0.4.0/quantus/metrics/faithfulness/sensitivity_n.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/faithfulness/sufficiency.py` & `quantus-0.4.0/quantus/metrics/faithfulness/sufficiency.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/localisation/__init__.py` & `quantus-0.4.0/quantus/metrics/localisation/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/localisation/attribution_localisation.py` & `quantus-0.4.0/quantus/metrics/localisation/attribution_localisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from quantus.metrics.base import Metric
 
 
 class AttributionLocalisation(Metric):
     """
     Implementation of the Attribution Localization by Kohlbrenner et al., 2020.
 
-    The Attribution Localization implements the ratio of positive attributions within the target to the overall
+    Attribution Localization implements the ratio of positive attributions within the target to the overall
     attribution. High scores are desired, as it means, that the positively attributed pixels belong to the
     targeted object class.
 
     References:
         1) Max Kohlbrenner et al.:
            "Towards Best Practice in Explaining Neural Network Decisions with LRP."
            IJCNN (2020): 1-7.
```

### Comparing `quantus-0.3.5/quantus/metrics/localisation/auc.py` & `quantus-0.4.0/quantus/metrics/localisation/auc.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/localisation/focus.py` & `quantus-0.4.0/quantus/metrics/localisation/focus.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/localisation/pointing_game.py` & `quantus-0.4.0/quantus/metrics/localisation/pointing_game.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/localisation/relevance_mass_accuracy.py` & `quantus-0.4.0/quantus/metrics/localisation/relevance_mass_accuracy.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from quantus.metrics.base import Metric
 
 
 class RelevanceMassAccuracy(Metric):
     """
     Implementation of the Relevance Rank Accuracy by Arras et al., 2021.
 
-    The Relevance Mass Accuracy computes the ratio of positive attributions inside the bounding box to
+    The Relevance Mass Accuracy computes the ratio of attributions inside the bounding box to
     the sum of overall positive attributions. High scores are desired, as the pixels with the highest positively
     attributed scores should be within the bounding box of the targeted object.
 
     References:
         1) Leila Arras et al.: "CLEVR-XAI: A benchmark dataset for the ground
         truth evaluation of neural network explanations." Inf. Fusion 81 (2022): 14-40.
     """
```

### Comparing `quantus-0.3.5/quantus/metrics/localisation/relevance_rank_accuracy.py` & `quantus-0.4.0/quantus/metrics/localisation/relevance_rank_accuracy.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/localisation/top_k_intersection.py` & `quantus-0.4.0/quantus/metrics/localisation/top_k_intersection.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/randomisation/__init__.py` & `quantus-0.4.0/quantus/metrics/randomisation/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/randomisation/model_parameter_randomisation.py` & `quantus-0.4.0/quantus/metrics/randomisation/model_parameter_randomisation.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/randomisation/random_logit.py` & `quantus-0.4.0/quantus/metrics/randomisation/random_logit.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/robustness/__init__.py` & `quantus-0.4.0/quantus/metrics/robustness/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/robustness/avg_sensitivity.py` & `quantus-0.4.0/quantus/metrics/robustness/avg_sensitivity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/robustness/consistency.py` & `quantus-0.4.0/quantus/metrics/robustness/consistency.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/robustness/continuity.py` & `quantus-0.4.0/quantus/metrics/robustness/continuity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/robustness/local_lipschitz_estimate.py` & `quantus-0.4.0/quantus/metrics/robustness/local_lipschitz_estimate.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/robustness/max_sensitivity.py` & `quantus-0.4.0/quantus/metrics/robustness/max_sensitivity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/robustness/relative_input_stability.py` & `quantus-0.4.0/quantus/metrics/robustness/relative_input_stability.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/robustness/relative_output_stability.py` & `quantus-0.4.0/quantus/metrics/robustness/relative_output_stability.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus/metrics/robustness/relative_representation_stability.py` & `quantus-0.4.0/quantus/metrics/robustness/relative_representation_stability.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/quantus.egg-info/PKG-INFO` & `quantus-0.4.0/quantus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: quantus
-Version: 0.3.5
-Summary: A metrics toolkit to evaluate neural network explanations.
+Version: 0.4.0
+Summary: A toolkit to evaluate neural network explanations.
 Home-page: http://github.com/understandable-machine-intelligence-lab/Quantus
 Author: Anna Hedstrom
 Author-email: hedstroem.anna@gmail.com
 License: GNU LESSER GENERAL PUBLIC LICENSE VERSION 3
 Keywords: explainable ai,xai,machine learning,deep learning
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: torch
 Provides-Extra: tensorflow
 Provides-Extra: captum
 Provides-Extra: tf-explain
 Provides-Extra: zennit
-Provides-Extra: tutorials
 Provides-Extra: tests
 Provides-Extra: full
 License-File: LICENSE
 License-File: COPYING
 License-File: COPYING.LESSER
 
 <p align="center">
@@ -29,32 +28,33 @@
 <p align="center">
   PyTorch and TensorFlow
 
 [![Getting started!](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/understandable-machine-intelligence-lab/Quantus/blob/main/tutorials/Tutorial_ImageNet_Example_All_Metrics.ipynb)
 [![Launch Tutorials](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/understandable-machine-intelligence-lab/Quantus/HEAD?labpath=tutorials)
 [![Python package](https://github.com/understandable-machine-intelligence-lab/Quantus/actions/workflows/python-package.yml/badge.svg)](https://github.com/understandable-machine-intelligence-lab/Quantus/actions/workflows/python-package.yml)
 [![Code coverage](https://github.com/understandable-machine-intelligence-lab/Quantus/actions/workflows/codecov.yml/badge.svg)](https://github.com/understandable-machine-intelligence-lab/Quantus/actions/workflows/codecov.yml)
-![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)
+![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)
 [![PyPI version](https://badge.fury.io/py/quantus.svg)](https://badge.fury.io/py/quantus)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation Status](https://readthedocs.org/projects/quantus/badge/?version=latest)](https://quantus.readthedocs.io/en/latest/?badge=latest)
 [![codecov.io](https://codecov.io/github/understandable-machine-intelligence-lab/Quantus/coverage.svg?branch=master)](https://codecov.io/github/understandable-machine-intelligence-lab/Quantus?branch=master)
 [![Downloads](https://static.pepy.tech/badge/quantus)](https://pepy.tech/project/quantus)
 
 _Quantus is currently under active development so carefully note the Quantus release version to ensure reproducibility of your work._
 
 [📑 Shortcut to paper!](https://jmlr.org/papers/volume24/22-0142/22-0142.pdf)
         
 ## News and Highlights! :rocket:
 
-- Accepted to Journal of Machine Learning Research (MLOSS) ([paper](https://jmlr.org/papers/v24/22-0142.html))!
+- Released a new version 0.4.0 that now supports Python 3.10 and 3.11, read more [here](https://github.com/understandable-machine-intelligence-lab/Quantus/releases)!
+- Accepted to Journal of Machine Learning Research (MLOSS), read the [paper](https://jmlr.org/papers/v24/22-0142.html)
 - Offers more than **30+ metrics in 6 categories** for XAI evaluation
 - Supports different data types (image, time-series, tabular, NLP next up!) and models (PyTorch, TensorFlow)
 - Extended built-in support for explanation methods ([captum](https://captum.ai/) and [tf-explain](https://tf-explain.readthedocs.io/en/latest/))
-- New optimisations to help speed up computation, see API reference [here](https://quantus.readthedocs.io/en/latest/docs_api/quantus.metrics.base_batched.html)!
+- New optimisations to help speed up computation, see API reference [here](https://quantus.readthedocs.io/en/latest/docs_api/quantus.metrics.base_batched.html)
 
 See [here](https://github.com/understandable-machine-intelligence-lab/Quantus/releases) for the latest release(s).
 
 ## Citation
 
 If you find this toolkit or its companion paper
 [**Quantus: An Explainable AI Toolkit for Responsible Evaluation of Neural Network Explanations and Beyond**](https://jmlr.org/papers/v24/22-0142.html)
@@ -216,17 +216,18 @@
 For a more in-depth guide on how to install Quantus, please read more [here](https://quantus.readthedocs.io/en/latest/getting_started/installation.html). This includes instructions for how to install a desired deep learning framework such as PyTorch or TensorFlow together with Quantus.
 
 ### Package requirements
 
 The package requirements are as follows:
 ```
 python>=3.7.0
-pytorch>=1.10.1
-TensorFlow==2.6.2
+torch>=1.11.0
+tensorflow>=2.5.0
 ```
+Please note that the exact [PyTorch](https://pytorch.org/) and/ or [TensorFlow](https://www.TensorFlow.org) versions to be installed depends on your Python version (3.7-3.11) and platform (`darwin`, `linux`, …). See `requirements_test.txt` to retrieve the exact versions of [PyTorch](https://pytorch.org/) and/ or [TensorFlow](https://www.TensorFlow.org).
 
 ## Getting started
 
 The following will give a short introduction to how to get started with Quantus. Note that this example is based on the [PyTorch](https://pytorch.org/) framework, but we also support 
 [TensorFlow](https://www.tensorflow.org), which would differ only in the loading of the model, data and explanations. To get started with Quantus, you need:
 * A model (`model`), inputs (`x_batch`) and labels (`y_batch`)
 * Some explanations you want to evaluate (`a_batch`)
```

### Comparing `quantus-0.3.5/quantus.egg-info/SOURCES.txt` & `quantus-0.4.0/quantus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 COPYING
 COPYING.LESSER
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
+requirements_test.txt
 setup.py
 quantus/__init__.py
 quantus/evaluation.py
 quantus.egg-info/PKG-INFO
 quantus.egg-info/SOURCES.txt
 quantus.egg-info/dependency_links.txt
 quantus.egg-info/not-zip-safe
```

### Comparing `quantus-0.3.5/tests/conftest.py` & `quantus-0.4.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,11 +198,11 @@
 def titanic_dataset():
     df = pd.read_csv("tutorials/assets/titanic3.csv")
     df = df[["age", "embarked", "fare", "parch", "pclass", "sex", "sibsp", "survived"]]
     df["age"] = df["age"].fillna(df["age"].mean())
     df["fare"] = df["fare"].fillna(df["fare"].mean())
 
     df_enc = pd.get_dummies(df, columns=["embarked", "pclass", "sex"]).sample(frac=1)
-    X = df_enc.drop(["survived"], axis=1).values.astype(np.float)
-    Y = df_enc["survived"].values.astype(np.int)
+    X = df_enc.drop(["survived"], axis=1).values.astype(float)
+    Y = df_enc["survived"].values.astype(int)
     _, test_features, _, test_labels = train_test_split(X, Y, test_size=0.3)
     return {"x_batch": test_features, "y_batch": test_labels}
```

### Comparing `quantus-0.3.5/tests/helpers/test_explanation_func.py` & `quantus-0.4.0/tests/helpers/test_explanation_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/tests/helpers/test_loss_func.py` & `quantus-0.4.0/tests/helpers/test_loss_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/tests/helpers/test_mosaic_func.py` & `quantus-0.4.0/tests/helpers/test_mosaic_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/tests/helpers/test_norm_func.py` & `quantus-0.4.0/tests/helpers/test_norm_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/tests/helpers/test_normalise_func.py` & `quantus-0.4.0/tests/helpers/test_normalise_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/tests/helpers/test_perturb_func.py` & `quantus-0.4.0/tests/helpers/test_perturb_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 
 @pytest.fixture
 def input_uniform_mnist():
     return np.random.uniform(0, 0.1, size=(1, 28, 28))
 
 
-@pytest.mark.fixed
+@pytest.mark.perturb_func
 @pytest.mark.parametrize(
     "data,params,expected",
     [
         (
             lazy_fixture("input_zeros_2d_3ch"),
             {
                 "indices": [0, 2],
@@ -157,15 +157,15 @@
 
     if isinstance(expected, (int, float)):
         assert np.all(
             [i == expected for i in out[indices].flatten()]
         ), f"Test failed.{out}"
 
 
-@pytest.mark.fixed
+@pytest.mark.perturb_func
 @pytest.mark.parametrize(
     "data,params,expected",
     [
         (
             lazy_fixture("input_zeros_2d_3ch"),
             {
                 "indices": [0, 2],
```

### Comparing `quantus-0.3.5/tests/helpers/test_pytorch_model.py` & `quantus-0.4.0/tests/helpers/test_pytorch_model.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/tests/helpers/test_similarity_func.py` & `quantus-0.4.0/tests/helpers/test_similarity_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/tests/helpers/test_tf_model.py` & `quantus-0.4.0/tests/helpers/test_tf_model.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/tests/helpers/test_utils.py` & `quantus-0.4.0/tests/helpers/test_utils.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/tests/metrics/conftest.py` & `quantus-0.4.0/tests/metrics/conftest.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/tests/metrics/test_axiomatic_metrics.py` & `quantus-0.4.0/tests/metrics/test_axiomatic_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,33 +427,33 @@
 
 
 @pytest.mark.axiomatic
 @pytest.mark.parametrize(
     "model,data,params,expected",
     [
         (
-                lazy_fixture("load_mnist_model_tf"),
-                lazy_fixture("load_mnist_images_tf"),
-                {
-                    "a_batch_generate": True,
-                    "init": {
-                        "abs": False,
-                        "normalise": False,
-                        "input_shift": 0.2,
-                        "disable_warnings": True,
-                        "display_progressbar": False,
-                    },
-                    "call": {
-                        "explain_func": explain,
-                        "explain_func_kwargs": {
-                            "method": "VanillaGradients",
-                        },
+            lazy_fixture("load_mnist_model_tf"),
+            lazy_fixture("load_mnist_images_tf"),
+            {
+                "a_batch_generate": True,
+                "init": {
+                    "abs": False,
+                    "normalise": False,
+                    "input_shift": 0.2,
+                    "disable_warnings": True,
+                    "display_progressbar": False,
+                },
+                "call": {
+                    "explain_func": explain,
+                    "explain_func_kwargs": {
+                        "method": "VanillaGradients",
                     },
                 },
-                {"dtypes": [True, False]},
+            },
+            {"dtypes": [True, False]},
         ),
         (
             lazy_fixture("load_1d_3ch_conv_model"),
             lazy_fixture("almost_uniform_1d"),
             {
                 "a_batch_generate": False,
                 "init": {
@@ -504,15 +504,16 @@
                     "input_shift": -1,
                     "disable_warnings": True,
                     "display_progressbar": False,
                 },
                 "call": {
                     "explain_func": explain,
                     "explain_func_kwargs": {
-                        "method": "InputXGradient",},
+                        "method": "InputXGradient",
+                    },
                 },
             },
             {"dtypes": [True, False]},
         ),
         (
             lazy_fixture("load_mnist_model"),
             lazy_fixture("load_mnist_images"),
@@ -586,15 +587,17 @@
                     "normalise": False,
                     "input_shift": -1,
                     "disable_warnings": True,
                     "display_progressbar": False,
                 },
                 "call": {
                     "explain_func": explain,
-                    "explain_func_kwargs": {"method": "InputXGradient",},
+                    "explain_func_kwargs": {
+                        "method": "InputXGradient",
+                    },
                 },
             },
             {"dtypes": [True, False]},
         ),
         (
             lazy_fixture("load_1d_3ch_conv_model"),
             lazy_fixture("almost_uniform_1d"),
```

### Comparing `quantus-0.3.5/tests/metrics/test_complexity_metrics.py` & `quantus-0.4.0/tests/metrics/test_complexity_metrics.py`

 * *Files identical despite different names*

### Comparing `quantus-0.3.5/tests/metrics/test_faithfulness_metrics.py` & `quantus-0.4.0/tests/metrics/test_faithfulness_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,17 @@
                     "similarity_func": correlation_spearman,
                     "normalise": True,
                     "disable_warnings": True,
                     "display_progressbar": False,
                 },
                 "call": {
                     "explain_func": explain,
-                    "explain_func_kwargs": {"method": "GradientsInput",},
+                    "explain_func_kwargs": {
+                        "method": "GradientsInput",
+                    },
                 },
             },
             {"min": -1.0, "max": 1.0},
         ),
         (
             lazy_fixture("load_mnist_model"),
             lazy_fixture("load_mnist_images"),
@@ -1301,15 +1303,17 @@
                     "patch_size": 4,
                     "normalise": True,
                     "disable_warnings": True,
                     "display_progressbar": False,
                 },
                 "call": {
                     "explain_func": explain,
-                    "explain_func_kwargs": {"method": "VanillaGradients",},
+                    "explain_func_kwargs": {
+                        "method": "VanillaGradients",
+                    },
                 },
             },
             {"type": np.float64},
         ),
         (
             lazy_fixture("load_mnist_model"),
             lazy_fixture("load_mnist_images"),
@@ -1807,15 +1811,14 @@
     scores = ROAD(**init_params)(
         model=model,
         x_batch=x_batch,
         y_batch=y_batch,
         a_batch=a_batch,
         **call_params,
     )
-    print("scores!!!", scores)
 
     assert all(s <= expected["max"] for s in scores.values()) & (
         all(s >= expected["min"] for s in scores.values())
     ), "Test failed."
 
 
 @pytest.mark.faithfulness
```

### Comparing `quantus-0.3.5/tests/metrics/test_localisation_metrics.py` & `quantus-0.4.0/tests/metrics/test_localisation_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1348,15 +1348,15 @@
                 "init": {
                     "weighted": False,
                     "disable_warnings": True,
                     "display_progressbar": False,
                 },
             },
             {"min": 0.8, "max": 0.95},  # TODO: verify correctness
-            marks=pytest.mark.xfail
+            marks=pytest.mark.xfail,
         ),
         (
             lazy_fixture("load_mnist_model"),
             lazy_fixture("all_in_gt_2d_3ch"),
             {
                 "init": {
                     "weighted": False,
```

### Comparing `quantus-0.3.5/tests/metrics/test_randomisation_metrics.py` & `quantus-0.4.0/tests/metrics/test_randomisation_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,15 +109,17 @@
                     "similarity_func": correlation_spearman,
                     "normalise": True,
                     "disable_warnings": True,
                     "display_progressbar": False,
                 },
                 "call": {
                     "explain_func": explain,
-                    "explain_func_kwargs": {"method": "VanillaGradients",},
+                    "explain_func_kwargs": {
+                        "method": "VanillaGradients",
+                    },
                 },
             },
             {"min": -1.0, "max": 1.0},
         ),
         (
             lazy_fixture("load_1d_3ch_conv_model_tf"),
             lazy_fixture("almost_uniform_1d_no_abatch_channel_last"),
@@ -128,15 +130,17 @@
                     "similarity_func": correlation_pearson,
                     "normalise": True,
                     "disable_warnings": True,
                     "display_progressbar": False,
                 },
                 "call": {
                     "explain_func": explain,
-                    "explain_func_kwargs": {"method": "VanillaGradients",},
+                    "explain_func_kwargs": {
+                        "method": "VanillaGradients",
+                    },
                 },
             },
             {"exception": ValueError},
         ),
         (
             lazy_fixture("load_mnist_model_tf"),
             lazy_fixture("load_mnist_images_tf"),
@@ -147,15 +151,17 @@
                     "similarity_func": correlation_pearson,
                     "normalise": True,
                     "disable_warnings": True,
                     "display_progressbar": False,
                 },
                 "call": {
                     "explain_func": explain,
-                    "explain_func_kwargs": {"method": "Gradient",},
+                    "explain_func_kwargs": {
+                        "method": "Gradient",
+                    },
                 },
             },
             {"min": -1.0, "max": 1.0},
         ),
         (
             lazy_fixture("load_1d_3ch_conv_model"),
             lazy_fixture("almost_uniform_1d_no_abatch"),
@@ -303,14 +309,15 @@
                 "init": {
                     "num_classes": 10,
                     "normalise": True,
                     "disable_warnings": False,
                     "display_progressbar": False,
                 },
                 "call": {
+                    "softmax": True,
                     "explain_func": explain,
                     "explain_func_kwargs": {
                         "method": "Saliency",
                     },
                 },
             },
             {"min": -1.0, "max": 1.0},
@@ -322,73 +329,77 @@
                 "init": {
                     "num_classes": 10,
                     "normalise": True,
                     "disable_warnings": False,
                     "display_progressbar": False,
                 },
                 "call": {
+                    "softmax": True,
                     "explain_func": explain,
                     "explain_func_kwargs": {
                         "method": "Saliency",
                     },
                 },
             },
-            {"min": 0.0, "max": 1.0},
+            {"min": -1.0, "max": 1.0},
         ),
         (
             lazy_fixture("load_1d_3ch_conv_model"),
             lazy_fixture("almost_uniform_1d_no_abatch"),
             {
                 "a_batch_generate": False,
                 "init": {
                     "num_classes": 10,
                     "normalise": False,
                     "disable_warnings": True,
                     "display_progressbar": False,
                 },
                 "call": {
+                    "softmax": True,
                     "explain_func": explain,
                     "explain_func_kwargs": {
                         "method": "Saliency",
                     },
                 },
             },
-            {"min": 0.0, "max": 1.0},
+            {"min": -1.0, "max": 1.0},
         ),
         (
             lazy_fixture("load_mnist_model"),
             lazy_fixture("load_mnist_images"),
             {
                 "a_batch_generate": False,
                 "init": {
                     "num_classes": 10,
                     "normalise": False,
                     "disable_warnings": True,
                     "display_progressbar": False,
                 },
                 "call": {
+                    "softmax": True,
                     "explain_func": explain,
                     "explain_func_kwargs": {
                         "method": "Saliency",
                     },
                 },
             },
-            {"min": 0.0, "max": 1.0},
+            {"min": -1.0, "max": 1.0},
         ),
         (
             lazy_fixture("load_1d_3ch_conv_model"),
             lazy_fixture("almost_uniform_1d_no_abatch"),
             {
                 "init": {
                     "num_classes": 10,
                     "normalise": True,
                     "disable_warnings": True,
                     "display_progressbar": True,
                 },
                 "call": {
+                    "softmax": True,
                     "explain_func": explain,
                     "explain_func_kwargs": {
                         "method": "Saliency",
                     },
                 },
             },
             {"min": -1.0, "max": 1.0},
@@ -400,33 +411,35 @@
                 "init": {
                     "num_classes": 10,
                     "normalise": True,
                     "disable_warnings": True,
                     "display_progressbar": True,
                 },
                 "call": {
+                    "softmax": True,
                     "explain_func": explain,
                     "explain_func_kwargs": {
                         "method": "Saliency",
                     },
                 },
             },
-            {"min": 0.0, "max": 1.0},
+            {"min": -1.0, "max": 1.0},
         ),
         (
             lazy_fixture("titanic_model_torch"),
             lazy_fixture("titanic_dataset"),
             {
                 "init": {
                     "num_classes": 2,
                     "normalise": True,
                     "abs": True,
                     "disable_warnings": True,
                 },
                 "call": {
+                    "softmax": True,
                     "explain_func": explain,
                     "explain_func_kwargs": {
                         "method": "IntegratedGradients",
                         "reduce_axes": (),
                     },
                 },
             },
@@ -438,15 +451,15 @@
             {
                 "init": {
                     "num_classes": 2,
                     "normalise": True,
                     "abs": True,
                     "disable_warnings": True,
                 },
-                "call": {"explain_func": explain_func_stub},
+                "call": {"softmax": True, "explain_func": explain_func_stub},
             },
             {"min": -1.0, "max": 1.01},
         ),
     ],
 )
 def test_random_logit(
     model: ModelInterface,
```

### Comparing `quantus-0.3.5/tests/metrics/test_relative_stability.py` & `quantus-0.4.0/tests/metrics/test_relative_stability.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,17 @@
 
 @pytest.mark.robustness
 @pytest.mark.parametrize(
     "metric",
     [RIS_CONSTRUCTOR, ROS_CONSTRUCTOR, RRS_CONSTRUCTOR],
     ids=["RIS", "ROS", "RRS"],
 )
-def test_return_nan(metric, load_mnist_model_tf, load_mnist_images_tf, mock_prediction_changed):
+def test_return_nan(
+    metric, load_mnist_model_tf, load_mnist_images_tf, mock_prediction_changed
+):
     x_batch = load_mnist_images_tf["x_batch"]
     y_batch = predict(load_mnist_model_tf, x_batch)
 
     rs = metric()
     result = rs(
         model=load_mnist_model_tf,
         x_batch=x_batch,
```

### Comparing `quantus-0.3.5/tests/metrics/test_robustness_metrics.py` & `quantus-0.4.0/tests/metrics/test_robustness_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                     "explain_func_kwargs": {
                         "method": "VanillaGradients",
                     },
                 },
             },
             {"min": 0.0, "max": 1.0},
         ),
-(
+        (
             lazy_fixture("load_mnist_model_tf"),
             lazy_fixture("load_mnist_images_tf"),
             {
                 "init": {
                     "lower_bound": 0.2,
                     "nr_samples": 10,
                     "disable_warnings": True,
@@ -334,15 +334,15 @@
                     "explain_func_kwargs": {
                         "method": "Saliency",
                     },
                 },
             },
             {"min": 0.0, "max": 1.0},
         ),
-(
+        (
             lazy_fixture("load_mnist_model"),
             lazy_fixture("load_mnist_images"),
             {
                 "a_batch_generate": False,
                 "init": {
                     "perturb_std": 0.1,
                     "nr_samples": 10,
@@ -673,15 +673,15 @@
                     "explain_func_kwargs": {
                         "method": "Saliency",
                     },
                 },
             },
             {"min": 0.0, "max": 1.0},
         ),
-(
+        (
             lazy_fixture("load_mnist_model"),
             lazy_fixture("load_mnist_images"),
             {
                 "a_batch_generate": False,
                 "init": {
                     "lower_bound": 0.2,
                     "nr_samples": 10,
@@ -818,15 +818,15 @@
                         "method": "Saliency",
                     },
                 },
                 "a_batch_generate": False,
             },
             {"min": 0.0, "max": 1.0},
         ),
-(
+        (
             lazy_fixture("load_mnist_model"),
             lazy_fixture("load_mnist_images"),
             {
                 "init": {
                     "discretise_func": rank,
                     "disable_warnings": True,
                     "display_progressbar": False,
```

### Comparing `quantus-0.3.5/tests/test_evaluation.py` & `quantus-0.4.0/tests/test_evaluation.py`

 * *Files identical despite different names*

