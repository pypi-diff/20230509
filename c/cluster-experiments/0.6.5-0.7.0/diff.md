# Comparing `tmp/cluster_experiments-0.6.5.tar.gz` & `tmp/cluster_experiments-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cluster_experiments-0.6.5.tar", last modified: Mon May  8 15:13:25 2023, max compression
+gzip compressed data, was "dist/cluster_experiments-0.7.0.tar", last modified: Tue May  9 07:58:22 2023, max compression
```

## Comparing `cluster_experiments-0.6.5.tar` & `cluster_experiments-0.7.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.444192 cluster_experiments-0.6.5/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.6.5/LICENSE
--rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.6.5/MANIFEST.in
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-08 15:13:25.443566 cluster_experiments-0.6.5/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     7140 2023-04-16 08:27:58.000000 cluster_experiments-0.6.5/README.md
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.403521 cluster_experiments-0.6.5/cluster_experiments/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1512 2023-04-05 14:50:51.000000 cluster_experiments-0.6.5/cluster_experiments/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.6.5/cluster_experiments/cupac.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    18320 2023-04-28 14:00:38.000000 cluster_experiments-0.6.5/cluster_experiments/experiment_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5609 2023-05-08 15:13:10.000000 cluster_experiments-0.6.5/cluster_experiments/perturbator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    19384 2023-04-14 12:56:48.000000 cluster_experiments-0.6.5/cluster_experiments/power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-02-10 16:31:12.000000 cluster_experiments-0.6.5/cluster_experiments/power_config.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    17741 2023-05-08 15:05:16.000000 cluster_experiments-0.6.5/cluster_experiments/random_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.6.5/cluster_experiments/utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.6.5/cluster_experiments/washover.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.410104 cluster_experiments-0.6.5/cluster_experiments.egg-info/
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-08 15:13:25.000000 cluster_experiments-0.6.5/cluster_experiments.egg-info/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     1447 2023-05-08 15:13:25.000000 cluster_experiments-0.6.5/cluster_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-05-08 15:13:25.000000 cluster_experiments-0.6.5/cluster_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-08 15:13:25.000000 cluster_experiments-0.6.5/cluster_experiments.egg-info/requires.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-05-08 15:13:25.000000 cluster_experiments-0.6.5/cluster_experiments.egg-info/top_level.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-05-08 15:13:25.444445 cluster_experiments-0.6.5/setup.cfg
--rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-08 15:13:10.000000 cluster_experiments-0.6.5/setup.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.418656 cluster_experiments-0.6.5/tests/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.6.5/tests/__init__.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.422461 cluster_experiments-0.6.5/tests/analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.5/tests/analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3771 2023-03-01 11:45:41.000000 cluster_experiments-0.6.5/tests/analysis/test_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.6.5/tests/analysis/test_ols_analysis.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.425910 cluster_experiments-0.6.5/tests/cupac/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.5/tests/cupac/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.6.5/tests/cupac/test_aggregator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.6.5/tests/cupac/test_cupac_handler.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2234 2023-02-08 15:47:52.000000 cluster_experiments-0.6.5/tests/examples.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.428103 cluster_experiments-0.6.5/tests/perturbator/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.5/tests/perturbator/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2879 2023-05-08 15:13:10.000000 cluster_experiments-0.6.5/tests/perturbator/test_perturbator.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.436096 cluster_experiments-0.6.5/tests/power_analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.5/tests/power_analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3164 2023-02-10 16:31:12.000000 cluster_experiments-0.6.5/tests/power_analysis/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.6.5/tests/power_analysis/test_cupac_power.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.6.5/tests/power_analysis/test_multivariate.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.6.5/tests/power_analysis/test_parallel.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.6.5/tests/power_analysis/test_power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.6.5/tests/power_analysis/test_power_raises.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3109 2023-04-07 10:35:06.000000 cluster_experiments-0.6.5/tests/power_analysis/test_switchback_power.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-08 15:13:25.442745 cluster_experiments-0.6.5/tests/splitter/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.5/tests/splitter/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5686 2023-05-08 15:05:16.000000 cluster_experiments-0.6.5/tests/splitter/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.6.5/tests/splitter/test_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.6.5/tests/splitter/test_switchback_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.6.5/tests/splitter/test_time_col.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.6.5/tests/splitter/test_washover.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2042 2023-04-05 14:50:51.000000 cluster_experiments-0.6.5/tests/test_docs.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.6.5/tests/test_non_clustered.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.6.5/tests/test_utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.6.5/tests/utils.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.776365 cluster_experiments-0.7.0/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.7.0/LICENSE
+-rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.7.0/MANIFEST.in
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-09 07:58:22.775724 cluster_experiments-0.7.0/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7150 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/README.md
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.705041 cluster_experiments-0.7.0/cluster_experiments/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1512 2023-04-05 14:50:51.000000 cluster_experiments-0.7.0/cluster_experiments/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.7.0/cluster_experiments/cupac.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    18320 2023-04-28 14:00:38.000000 cluster_experiments-0.7.0/cluster_experiments/experiment_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5609 2023-05-09 07:57:58.000000 cluster_experiments-0.7.0/cluster_experiments/perturbator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    19753 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/cluster_experiments/power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     4342 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/cluster_experiments/power_config.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    17741 2023-05-08 15:05:16.000000 cluster_experiments-0.7.0/cluster_experiments/random_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.7.0/cluster_experiments/utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.7.0/cluster_experiments/washover.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.713376 cluster_experiments-0.7.0/cluster_experiments.egg-info/
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-09 07:58:22.000000 cluster_experiments-0.7.0/cluster_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1481 2023-05-09 07:58:22.000000 cluster_experiments-0.7.0/cluster_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-05-09 07:58:22.000000 cluster_experiments-0.7.0/cluster_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-09 07:58:22.000000 cluster_experiments-0.7.0/cluster_experiments.egg-info/requires.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-05-09 07:58:22.000000 cluster_experiments-0.7.0/cluster_experiments.egg-info/top_level.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-05-09 07:58:22.776542 cluster_experiments-0.7.0/setup.cfg
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/setup.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.726593 cluster_experiments-0.7.0/tests/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.7.0/tests/__init__.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.731282 cluster_experiments-0.7.0/tests/analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.7.0/tests/analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3771 2023-03-01 11:45:41.000000 cluster_experiments-0.7.0/tests/analysis/test_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.7.0/tests/analysis/test_ols_analysis.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.736343 cluster_experiments-0.7.0/tests/cupac/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.7.0/tests/cupac/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.7.0/tests/cupac/test_aggregator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.7.0/tests/cupac/test_cupac_handler.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2406 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/tests/examples.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.739573 cluster_experiments-0.7.0/tests/perturbator/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.7.0/tests/perturbator/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2879 2023-05-08 15:13:10.000000 cluster_experiments-0.7.0/tests/perturbator/test_perturbator.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.764530 cluster_experiments-0.7.0/tests/power_analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.7.0/tests/power_analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3283 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/tests/power_analysis/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.7.0/tests/power_analysis/test_cupac_power.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.7.0/tests/power_analysis/test_multivariate.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.7.0/tests/power_analysis/test_parallel.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.7.0/tests/power_analysis/test_power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.7.0/tests/power_analysis/test_power_raises.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      941 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/tests/power_analysis/test_seed.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3107 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/tests/power_analysis/test_switchback_power.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.774551 cluster_experiments-0.7.0/tests/splitter/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.7.0/tests/splitter/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5686 2023-05-08 15:05:16.000000 cluster_experiments-0.7.0/tests/splitter/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.7.0/tests/splitter/test_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.7.0/tests/splitter/test_switchback_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.7.0/tests/splitter/test_time_col.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.7.0/tests/splitter/test_washover.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2042 2023-04-05 14:50:51.000000 cluster_experiments-0.7.0/tests/test_docs.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.7.0/tests/test_non_clustered.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.7.0/tests/test_utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.7.0/tests/utils.py
```

### Comparing `cluster_experiments-0.6.5/LICENSE` & `cluster_experiments-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/README.md` & `cluster_experiments-0.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 # Use gee to run the analysis
 analysis = GeeExperimentAnalysis(
     cluster_cols=["cluster", "date"],
 )
 
 # Run the power analysis
 pw = PowerAnalysis(
-    perturbator=perturbator, splitter=sw, analysis=analysis, n_simulations=50
+    perturbator=perturbator, splitter=sw, analysis=analysis, n_simulations=50, seed=123
 )
 
 # Keep in mind that the average effect is the absolute effect added, this is not relative!
 power = pw.power_analysis(df, average_effect=0.1)
 print(f"{power = }")
 ```
```

### Comparing `cluster_experiments-0.6.5/cluster_experiments/__init__.py` & `cluster_experiments-0.7.0/cluster_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/cluster_experiments/cupac.py` & `cluster_experiments-0.7.0/cluster_experiments/cupac.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/cluster_experiments/experiment_analysis.py` & `cluster_experiments-0.7.0/cluster_experiments/experiment_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/cluster_experiments/perturbator.py` & `cluster_experiments-0.7.0/cluster_experiments/perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/cluster_experiments/power_analysis.py` & `cluster_experiments-0.7.0/cluster_experiments/power_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
+import random
 from typing import Dict, Generator, Iterable, List, Optional, Tuple
 
+import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator
 from tqdm import tqdm
 
 from cluster_experiments.cupac import CupacHandler
 from cluster_experiments.experiment_analysis import ExperimentAnalysis
 from cluster_experiments.perturbator import Perturbator
@@ -37,14 +39,15 @@
         target_col: Name of the column with the outcome variable.
         treatment_col: Name of the column with the treatment variable.
         treatment: value of treatment_col considered to be treatment (not control)
         control: value of treatment_col considered to be control (not treatment)
         n_simulations: Number of simulations to run.
         alpha: Significance level.
         features_cupac_model: Covariates to be used in cupac model
+        seed: Optional. Seed to use for the splitter.
 
     Usage:
     ```python
     from datetime import date
 
     import numpy as np
     import pandas as pd
@@ -95,14 +98,15 @@
         target_col: str = "target",
         treatment_col: str = "treatment",
         treatment: str = "B",
         control: str = "A",
         n_simulations: int = 100,
         alpha: float = 0.05,
         features_cupac_model: Optional[List[str]] = None,
+        seed: Optional[int] = None,
     ):
         self.perturbator = perturbator
         self.splitter = splitter
         self.analysis = analysis
         self.n_simulations = n_simulations
         self.target_col = target_col
         self.treatment = treatment
@@ -111,14 +115,18 @@
         self.alpha = alpha
 
         self.cupac_handler = CupacHandler(
             cupac_model=cupac_model,
             target_col=target_col,
             features_cupac_model=features_cupac_model,
         )
+        if seed is not None:
+            random.seed(seed)  # seed for splitter
+            np.random.seed(seed)  # seed for the binary perturbator
+            # may need to seed other stochasticity sources if added
 
         self.check_inputs()
 
     def _simulate_perturbed_df(
         self,
         df: pd.DataFrame,
         pre_experiment_df: Optional[pd.DataFrame] = None,
@@ -377,14 +385,15 @@
             analysis=analysis_cls.from_config(config),
             cupac_model=cupac_cls.from_config(config),
             target_col=config.target_col,
             treatment_col=config.treatment_col,
             treatment=config.treatment,
             n_simulations=config.n_simulations,
             alpha=config.alpha,
+            seed=config.seed,
         )
 
     def check_treatment_col(self):
         """Checks consistency of treatment column"""
         assert (
             self.analysis.treatment_col == self.perturbator.treatment_col
         ), f"treatment_col in analysis ({self.analysis.treatment_col}) must be the same as treatment_col in perturbator ({self.perturbator.treatment_col})"
```

### Comparing `cluster_experiments-0.6.5/cluster_experiments/power_config.py` & `cluster_experiments-0.7.0/cluster_experiments/power_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         covariates: list of columns to use as covariates
         average_effect: average effect to use in the perturbator
         treatments: list of treatments to use
         alpha: alpha value to use in the power analysis
         agg_col: column to use for aggregation in the CUPAC model
         smoothing_factor: smoothing value to use in the CUPAC model
         features_cupac_model: list of features to use in the CUPAC model
+        seed: seed to make the power analysis reproducible
 
     Usage:
 
     ```python
     from cluster_experiments.power_config import PowerConfig
     from cluster_experiments.power_analysis import PowerAnalysis
 
@@ -106,14 +107,16 @@
     control: str = "A"
 
     # Cupac
     agg_col: str = ""
     smoothing_factor: float = 20
     features_cupac_model: Optional[List[str]] = None
 
+    seed: Optional[int] = None
+
 
 perturbator_mapping = {
     "binary": BinaryPerturbator,
     "uniform": UniformPerturbator,
 }
 
 splitter_mapping = {
```

### Comparing `cluster_experiments-0.6.5/cluster_experiments/random_splitter.py` & `cluster_experiments-0.7.0/cluster_experiments/random_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/cluster_experiments/washover.py` & `cluster_experiments-0.7.0/cluster_experiments/washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/cluster_experiments.egg-info/SOURCES.txt` & `cluster_experiments-0.7.0/cluster_experiments.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 tests/power_analysis/__init__.py
 tests/power_analysis/conftest.py
 tests/power_analysis/test_cupac_power.py
 tests/power_analysis/test_multivariate.py
 tests/power_analysis/test_parallel.py
 tests/power_analysis/test_power_analysis.py
 tests/power_analysis/test_power_raises.py
+tests/power_analysis/test_seed.py
 tests/power_analysis/test_switchback_power.py
 tests/splitter/__init__.py
 tests/splitter/conftest.py
 tests/splitter/test_splitter.py
 tests/splitter/test_switchback_splitter.py
 tests/splitter/test_time_col.py
 tests/splitter/test_washover.py
```

### Comparing `cluster_experiments-0.6.5/cluster_experiments.egg-info/requires.txt` & `cluster_experiments-0.7.0/cluster_experiments.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/setup.py` & `cluster_experiments-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "matplotlib==3.4.3",
 ]
 
 dev_packages = test_packages + util_packages + docs_packages
 
 setup(
     name="cluster_experiments",
-    version="0.6.5",
+    version="0.7.0",
     packages=find_packages(),
     extras_require={
         "dev": dev_packages,
         "test": test_packages,
         "only-test": only_test_packages,
         "docs": docs_packages,
     },
```

### Comparing `cluster_experiments-0.6.5/tests/analysis/test_analysis.py` & `cluster_experiments-0.7.0/tests/analysis/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/cupac/test_aggregator.py` & `cluster_experiments-0.7.0/tests/cupac/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/cupac/test_cupac_handler.py` & `cluster_experiments-0.7.0/tests/cupac/test_cupac_handler.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/examples.py` & `cluster_experiments-0.7.0/tests/examples.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 import numpy as np
 import pandas as pd
 
+TARGETS = {
+    "binary": lambda x: np.random.choice([0, 1], size=x),
+    "continuous": lambda x: np.random.normal(0, 1, x),
+}
 
-def generate_random_data(clusters, dates, N):
+
+def generate_random_data(clusters, dates, N, target="continuous"):
     # Generate random data with clusters and target
     users = [f"User {i}" for i in range(1000)]
+
+    target_values = TARGETS[target](N)
     df = pd.DataFrame(
         {
             "cluster": np.random.choice(clusters, size=N),
-            "target": np.random.normal(0, 1, size=N),
+            "target": target_values,
             "user": np.random.choice(users, size=N),
             "date": np.random.choice(dates, size=N),
         }
     )
 
     return df
```

### Comparing `cluster_experiments-0.6.5/tests/perturbator/test_perturbator.py` & `cluster_experiments-0.7.0/tests/perturbator/test_perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/power_analysis/conftest.py` & `cluster_experiments-0.7.0/tests/power_analysis/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,19 @@
     df = generate_random_data(clusters, dates, N)
     df["x1"] = np.random.normal(0, 1, N)
     df["x2"] = np.random.normal(0, 1, N)
     return df
 
 
 @pytest.fixture
+def df_binary(clusters, dates):
+    return generate_random_data(clusters, dates, N, target="binary")
+
+
+@pytest.fixture
 def perturbator():
     return UniformPerturbator(average_effect=0.1)
 
 
 @pytest.fixture
 def analysis_gee_vainilla():
     return GeeExperimentAnalysis(
```

### Comparing `cluster_experiments-0.6.5/tests/power_analysis/test_cupac_power.py` & `cluster_experiments-0.7.0/tests/power_analysis/test_cupac_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/power_analysis/test_multivariate.py` & `cluster_experiments-0.7.0/tests/power_analysis/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/power_analysis/test_parallel.py` & `cluster_experiments-0.7.0/tests/power_analysis/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/power_analysis/test_power_analysis.py` & `cluster_experiments-0.7.0/tests/power_analysis/test_power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/power_analysis/test_power_raises.py` & `cluster_experiments-0.7.0/tests/power_analysis/test_power_raises.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/power_analysis/test_switchback_power.py` & `cluster_experiments-0.7.0/tests/power_analysis/test_switchback_power.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         verbose=True,
     )
     assert power >= 0
     assert power <= 1
 
 
 def test_switchback_washover(switchback_power_analysis, df):
-
     power_no_washover = switchback_power_analysis.power_analysis(
         df,
         average_effect=0.1,
         n_simulations=10,
     )
     switchback_power_analysis.splitter.washover = ConstantWashover(
         washover_time_delta=datetime.timedelta(hours=23)
@@ -81,15 +80,14 @@
         n_simulations=10,
     )
     assert power >= 0
     assert power <= 1
 
 
 def test_switchback_strata():
-
     # Define bihourly switchback splitter
     config = {
         "time_col": "time",
         "switch_frequency": "30min",
         "perturbator": "uniform",
         "analysis": "ols_clustered",
         "splitter": "switchback_stratified",
```

### Comparing `cluster_experiments-0.6.5/tests/splitter/conftest.py` & `cluster_experiments-0.7.0/tests/splitter/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/splitter/test_splitter.py` & `cluster_experiments-0.7.0/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/splitter/test_switchback_splitter.py` & `cluster_experiments-0.7.0/tests/splitter/test_switchback_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/splitter/test_time_col.py` & `cluster_experiments-0.7.0/tests/splitter/test_time_col.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/splitter/test_washover.py` & `cluster_experiments-0.7.0/tests/splitter/test_washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/test_docs.py` & `cluster_experiments-0.7.0/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/test_non_clustered.py` & `cluster_experiments-0.7.0/tests/test_non_clustered.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.5/tests/utils.py` & `cluster_experiments-0.7.0/tests/utils.py`

 * *Files identical despite different names*

