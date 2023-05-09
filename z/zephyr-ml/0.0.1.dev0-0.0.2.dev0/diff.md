# Comparing `tmp/zephyr-ml-0.0.1.dev0.tar.gz` & `tmp/zephyr-ml-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephyr-ml-0.0.1.dev0.tar", last modified: Tue Feb 21 15:38:44 2023, max compression
+gzip compressed data, was "zephyr-ml-0.0.2.dev0.tar", last modified: Tue May  9 15:14:53 2023, max compression
```

## Comparing `zephyr-ml-0.0.1.dev0.tar` & `zephyr-ml-0.0.2.dev0.tar`

### file list

```diff
@@ -1,56 +1,65 @@
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-21 15:38:44.911180 zephyr-ml-0.0.1.dev0/
--rw-r--r--   0 sarah      (501) staff       (20)     8318 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/CONTRIBUTING.rst
--rw-r--r--   0 sarah      (501) staff       (20)     1088 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/LICENSE
--rw-r--r--   0 sarah      (501) staff       (20)      265 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/MANIFEST.in
--rw-r--r--   0 sarah      (501) staff       (20)     8274 2023-02-21 15:38:44.911351 zephyr-ml-0.0.1.dev0/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     7550 2023-01-24 19:21:30.000000 zephyr-ml-0.0.1.dev0/README.md
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-21 15:38:44.893530 zephyr-ml-0.0.1.dev0/docs/
--rw-r--r--   0 sarah      (501) staff       (20)      607 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/docs/Makefile
--rw-r--r--   0 sarah      (501) staff       (20)       28 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/docs/authors.rst
--rw-r--r--   0 sarah      (501) staff       (20)     5879 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/docs/conf.py
--rw-r--r--   0 sarah      (501) staff       (20)       33 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/docs/contributing.rst
--rw-r--r--   0 sarah      (501) staff       (20)       29 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/docs/history.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-21 15:38:44.894188 zephyr-ml-0.0.1.dev0/docs/images/
--rw-r--r--   0 sarah      (501) staff       (20)    33432 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/docs/images/dai-logo-white-200.png
--rw-r--r--   0 sarah      (501) staff       (20)      300 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/docs/index.rst
--rw-r--r--   0 sarah      (501) staff       (20)      768 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/docs/make.bat
--rw-r--r--   0 sarah      (501) staff       (20)       28 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/docs/readme.rst
--rw-r--r--   0 sarah      (501) staff       (20)     1014 2023-02-21 15:38:44.912109 zephyr-ml-0.0.1.dev0/setup.cfg
--rw-r--r--   0 sarah      (501) staff       (20)     2696 2023-02-21 15:33:04.000000 zephyr-ml-0.0.1.dev0/setup.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-21 15:38:44.897348 zephyr-ml-0.0.1.dev0/tests/
--rw-r--r--   0 sarah      (501) staff       (20)        0 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/tests/__init__.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-21 15:38:44.898927 zephyr-ml-0.0.1.dev0/tests/labeling/
--rw-r--r--   0 sarah      (501) staff       (20)        0 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/tests/labeling/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)      416 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/tests/labeling/test_data_labeler.py
--rw-r--r--   0 sarah      (501) staff       (20)     4174 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/tests/labeling/test_helpers.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-21 15:38:44.899669 zephyr-ml-0.0.1.dev0/tests/primitives/
--rw-r--r--   0 sarah      (501) staff       (20)      927 2023-02-21 15:33:04.000000 zephyr-ml-0.0.1.dev0/tests/primitives/test_postprocessing.py
--rw-r--r--   0 sarah      (501) staff       (20)     5363 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/tests/test___init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     4233 2023-02-21 15:33:04.000000 zephyr-ml-0.0.1.dev0/tests/test_core.py
--rw-r--r--   0 sarah      (501) staff       (20)     8708 2023-02-08 18:08:47.000000 zephyr-ml-0.0.1.dev0/tests/test_entityset.py
--rw-r--r--   0 sarah      (501) staff       (20)     1926 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/tests/test_metadata.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-21 15:38:44.902194 zephyr-ml-0.0.1.dev0/zephyr_ml/
--rw-r--r--   0 sarah      (501) staff       (20)      482 2023-02-21 15:33:04.000000 zephyr-ml-0.0.1.dev0/zephyr_ml/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     7815 2023-02-21 15:33:04.000000 zephyr-ml-0.0.1.dev0/zephyr_ml/core.py
--rw-r--r--   0 sarah      (501) staff       (20)     5246 2023-02-08 18:08:47.000000 zephyr-ml-0.0.1.dev0/zephyr_ml/entityset.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-21 15:38:44.907439 zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/
--rw-r--r--   0 sarah      (501) staff       (20)      994 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     2739 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/data_labeler.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-21 15:38:44.909801 zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/labeling_functions/
--rw-r--r--   0 sarah      (501) staff       (20)      291 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/labeling_functions/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     1786 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/labeling_functions/brake_pad_presence.py
--rw-r--r--   0 sarah      (501) staff       (20)     2128 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/labeling_functions/converter_replacement_presence.py
--rw-r--r--   0 sarah      (501) staff       (20)     1639 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/labeling_functions/total_power_loss.py
--rw-r--r--   0 sarah      (501) staff       (20)     7299 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/utils.py
--rw-r--r--   0 sarah      (501) staff       (20)     5766 2022-11-15 18:58:24.000000 zephyr-ml-0.0.1.dev0/zephyr_ml/metadata.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-21 15:38:44.910623 zephyr-ml-0.0.1.dev0/zephyr_ml/primitives/
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-01-21 00:16:34.000000 zephyr-ml-0.0.1.dev0/zephyr_ml/primitives/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     2103 2023-02-21 15:33:04.000000 zephyr-ml-0.0.1.dev0/zephyr_ml/primitives/postprocessing.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-21 15:38:44.905659 zephyr-ml-0.0.1.dev0/zephyr_ml.egg-info/
--rw-r--r--   0 sarah      (501) staff       (20)     8274 2023-02-21 15:38:44.000000 zephyr-ml-0.0.1.dev0/zephyr_ml.egg-info/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     1192 2023-02-21 15:38:44.000000 zephyr-ml-0.0.1.dev0/zephyr_ml.egg-info/SOURCES.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-02-21 15:38:44.000000 zephyr-ml-0.0.1.dev0/zephyr_ml.egg-info/dependency_links.txt
--rw-r--r--   0 sarah      (501) staff       (20)       95 2023-02-21 15:38:44.000000 zephyr-ml-0.0.1.dev0/zephyr_ml.egg-info/entry_points.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-02-21 15:38:44.000000 zephyr-ml-0.0.1.dev0/zephyr_ml.egg-info/not-zip-safe
--rw-r--r--   0 sarah      (501) staff       (20)      629 2023-02-21 15:38:44.000000 zephyr-ml-0.0.1.dev0/zephyr_ml.egg-info/requires.txt
--rw-r--r--   0 sarah      (501) staff       (20)       10 2023-02-21 15:38:44.000000 zephyr-ml-0.0.1.dev0/zephyr_ml.egg-info/top_level.txt
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:14:53.421074 zephyr-ml-0.0.2.dev0/
+-rw-r--r--   0 sarah      (501) staff       (20)     8318 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      460 2023-05-01 17:28:27.000000 zephyr-ml-0.0.2.dev0/HISTORY.md
+-rw-r--r--   0 sarah      (501) staff       (20)     1088 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/LICENSE
+-rw-r--r--   0 sarah      (501) staff       (20)      301 2023-05-01 17:28:27.000000 zephyr-ml-0.0.2.dev0/MANIFEST.in
+-rw-r--r--   0 sarah      (501) staff       (20)    10889 2023-05-09 15:14:53.421240 zephyr-ml-0.0.2.dev0/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     9705 2023-05-01 17:28:27.000000 zephyr-ml-0.0.2.dev0/README.md
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:14:53.399653 zephyr-ml-0.0.2.dev0/docs/
+-rw-r--r--   0 sarah      (501) staff       (20)      607 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/docs/Makefile
+-rw-r--r--   0 sarah      (501) staff       (20)     5879 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/docs/conf.py
+-rw-r--r--   0 sarah      (501) staff       (20)       33 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/docs/contributing.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       29 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/docs/history.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:14:53.400381 zephyr-ml-0.0.2.dev0/docs/images/
+-rw-r--r--   0 sarah      (501) staff       (20)    33432 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/docs/images/dai-logo-white-200.png
+-rw-r--r--   0 sarah      (501) staff       (20)      289 2023-05-01 17:28:27.000000 zephyr-ml-0.0.2.dev0/docs/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      768 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/docs/make.bat
+-rw-r--r--   0 sarah      (501) staff       (20)       28 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/docs/readme.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     1014 2023-05-09 15:14:53.422188 zephyr-ml-0.0.2.dev0/setup.cfg
+-rw-r--r--   0 sarah      (501) staff       (20)     2722 2023-05-09 15:09:33.000000 zephyr-ml-0.0.2.dev0/setup.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:14:53.404337 zephyr-ml-0.0.2.dev0/tests/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/tests/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:14:53.406625 zephyr-ml-0.0.2.dev0/tests/labeling/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/tests/labeling/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)      416 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/tests/labeling/test_data_labeler.py
+-rw-r--r--   0 sarah      (501) staff       (20)     4174 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/tests/labeling/test_helpers.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:14:53.407231 zephyr-ml-0.0.2.dev0/tests/primitives/
+-rw-r--r--   0 sarah      (501) staff       (20)      991 2023-05-09 15:09:33.000000 zephyr-ml-0.0.2.dev0/tests/primitives/test_postprocessing.py
+-rw-r--r--   0 sarah      (501) staff       (20)     5363 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/tests/test___init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     5252 2023-05-09 15:09:33.000000 zephyr-ml-0.0.2.dev0/tests/test_core.py
+-rw-r--r--   0 sarah      (501) staff       (20)     8708 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/tests/test_entityset.py
+-rw-r--r--   0 sarah      (501) staff       (20)    10024 2023-05-09 15:09:33.000000 zephyr-ml-0.0.2.dev0/tests/test_feature_engineering.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1926 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/tests/test_metadata.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:14:53.409789 zephyr-ml-0.0.2.dev0/zephyr_ml/
+-rw-r--r--   0 sarah      (501) staff       (20)      482 2023-05-01 17:28:27.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     9156 2023-05-09 15:09:33.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/core.py
+-rw-r--r--   0 sarah      (501) staff       (20)     5246 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/entityset.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2592 2023-05-09 15:09:33.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/feature_engineering.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:14:53.414141 zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/
+-rw-r--r--   0 sarah      (501) staff       (20)      994 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2739 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/data_labeler.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:14:53.417144 zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/labeling_functions/
+-rw-r--r--   0 sarah      (501) staff       (20)      291 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/labeling_functions/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1786 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/labeling_functions/brake_pad_presence.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2128 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/labeling_functions/converter_replacement_presence.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1639 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/labeling_functions/total_power_loss.py
+-rw-r--r--   0 sarah      (501) staff       (20)     7299 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/utils.py
+-rw-r--r--   0 sarah      (501) staff       (20)     5766 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/metadata.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:14:53.418318 zephyr-ml-0.0.2.dev0/zephyr_ml/pipelines/
+-rw-r--r--   0 sarah      (501) staff       (20)     1013 2023-05-09 15:09:33.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/pipelines/xgb_classifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)      281 2023-05-01 17:28:27.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/pipelines/xgb_regressor.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:14:53.419148 zephyr-ml-0.0.2.dev0/zephyr_ml/primitives/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/primitives/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:14:53.420759 zephyr-ml-0.0.2.dev0/zephyr_ml/primitives/jsons/
+-rw-r--r--   0 sarah      (501) staff       (20)     2715 2023-05-09 15:09:33.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/primitives/jsons/xgboost.XGBClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2220 2023-05-01 17:28:27.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/primitives/jsons/xgboost.XGBRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1335 2023-05-09 15:09:33.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/primitives/jsons/zephyr_ml.primitives.postprocessing.FindThreshold.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2314 2023-05-09 15:09:33.000000 zephyr-ml-0.0.2.dev0/zephyr_ml/primitives/postprocessing.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:14:53.412726 zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/
+-rw-r--r--   0 sarah      (501) staff       (20)    10889 2023-05-09 15:14:53.000000 zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     1521 2023-05-09 15:14:53.000000 zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-05-09 15:14:53.000000 zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 sarah      (501) staff       (20)       95 2023-05-09 15:14:53.000000 zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/entry_points.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-05-09 15:14:53.000000 zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/not-zip-safe
+-rw-r--r--   0 sarah      (501) staff       (20)      648 2023-05-09 15:14:53.000000 zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/requires.txt
+-rw-r--r--   0 sarah      (501) staff       (20)       10 2023-05-09 15:14:53.000000 zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/top_level.txt
```

### Comparing `zephyr-ml-0.0.1.dev0/CONTRIBUTING.rst` & `zephyr-ml-0.0.2.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/LICENSE` & `zephyr-ml-0.0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/PKG-INFO` & `zephyr-ml-0.0.2.dev0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: zephyr-ml
-Version: 0.0.1.dev0
-Summary: Prediction engineering methods for Draco.
-Home-page: https://github.com/sintel-dev/zephyr
-Author: MIT Data To AI Lab
-Author-email: dai-lab@mit.edu
-Keywords: zephyr Draco Prediction Engineering
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7,<3.9
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-License-File: LICENSE
-
 <p align="left">
 <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt="DAI-Lab" />
 <i>A project from Data to AI Lab at MIT.</i>
 </p>
 
 <!-- Uncomment these lines after releasing the package to PyPI for version and downloads badges -->
 <!--[![PyPI Shield](https://img.shields.io/pypi/v/zephyr_ml.svg)](https://pypi.python.org/pypi/zephyr_ml)-->
@@ -43,14 +22,15 @@
  | :scroll: **[License]**              | The repository is published under the MIT License.                   |
  | :keyboard: **[Development Status]** | This software is in its Pre-Alpha stage.                             |
  | ![][Slack Logo] **[Community]**    | Join our Slack Workspace for announcements and discussions.          |
 
  [Website]: https://sintel.dev/
  [Documentation]: https://dtail.gitbook.io/zephyr/
  [Repository]: https://github.com/sintel-dev/Zephyr
+ [Tutorials]: https://github.com/sintel-dev/Zephyr/blob/master/notebooks
  [License]: https://github.com/sintel-dev/Zephyr/blob/master/LICENSE
  [Development Status]: https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha
  [Community]: https://join.slack.com/t/sintel-space/shared_invite/zt-q147oimb-4HcphcxPfDAM0O9_4PaUtw
  [Slack Logo]: https://github.com/sintel-dev/Orion/blob/master/docs/images/slack.png
 
  - Homepage: https://github.com/signals-dev/zephyr
 
@@ -166,24 +146,25 @@
 This will return us a dictionary with the name and a short description of each available
 function.
 
 ```
 {'brake_pad_presence': 'Calculates the total power loss over the data slice.',
  'converter_replacement_presence': 'Calculates the converter replacement presence.',
  'total_power_loss': 'Calculates the total power loss over the data slice.'}
- ```
+```
 
 In this case, we will choose the `total_power_loss` function, which calculates the total
 amount of power lost over a slice of time.
 
 ## 3. Generate Target Times
 
 Once we have loaded the data and the Labeling Function, we are ready to start using
 the `zephyr_ml.generate_labels` function to generate a Target Times table.
 
+
 ```python3
 from zephyr_ml import DataLabeler
 
 data_labeler = DataLabeler(labeling.labeling_functions.total_power_loss)
 target_times, metadata = data_labeler.generate_label_times(scada_es)
 ```
 
@@ -191,14 +172,71 @@
 working on a Machine Learning problem: the turbine ID (COD_ELEMENT), the cutoff time (time) and the label.
 
 ```
    COD_ELEMENT       time    label
 0            0 2022-01-01  45801.0
 ```
 
+## 4. Feature Engineering
+Using EntitySets and LabelTimes allows us to easily use Featuretools for automatic feature generation.
+
+```python3
+import featuretools as ft
+
+feature_matrix, features = ft.dfs(
+    entityset=scada_es,
+    target_dataframe_name='turbines',
+    cutoff_time_in_index=True,
+    cutoff_time=target_times,
+    max_features=20
+)
+```
+
+Then we get a list of features and the computed `feature_matrix`.
+
+```
+                       TURBINE_PI_ID TURBINE_LOCAL_ID TURBINE_SAP_COD DES_CORE_ELEMENT      SITE DES_CORE_PLANT  ... MODE(alarms.COD_STATUS) MODE(alarms.DES_NAME)  MODE(alarms.DES_TITLE)  NUM_UNIQUE(alarms.COD_ALARM)  NUM_UNIQUE(alarms.COD_ALARM_INT)    label
+COD_ELEMENT time                                                                                                 ...                                                                                                                                               
+0           2022-01-01          TA00               A0          LOC000              T00  LOCATION            LOC  ...                  Alarm1                Alarm1  Description of alarm 1                             1                                 1  45801.0
+
+[1 rows x 21 columns]
+```
+
+
+## 5. Modeling
+
+Once we have the feature matrix, we can train a model using the Zephyr interface where you can train, infer, and evaluate a pipeline. 
+First, we need to prepare our dataset for training by creating ``X`` and ``y`` variables and one-hot encoding features.
+
+```python3
+y = list(feature_matrix.pop('label'))
+X = pd.get_dummies(feature_matrix).values
+```
+
+In this example, we will use an 'xgb' regression pipeline to predict total power loss.
+
+```python3
+from zephyr_ml import Zephyr
+
+pipeline_name = 'xgb_regressor'
+
+zephyr = Zephyr(pipeline_name)
+```
+
+To train the pipeline, we simply use the `fit` function.
+```python3
+zephyr.fit(X, y)
+```
+
+After it finished training,  we can make prediciton using `predict`
+
+```python3
+y_pred =  zephyr.predict(X)
+```
+
+We can also use ``zephyr.evaluate`` to obtain the performance of the pipeline.
+
 # What's Next?
 
 If you want to continue learning about **Zephyr** and all its
 features please have a look at the tutorials found inside the [notebooks folder](
 https://github.com/signals-dev/zephyr/tree/main/notebooks).
-
-
```

### Comparing `zephyr-ml-0.0.1.dev0/README.md` & `zephyr-ml-0.0.2.dev0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: zephyr-ml
+Version: 0.0.2.dev0
+Summary: Prediction engineering methods for Draco.
+Home-page: https://github.com/sintel-dev/zephyr
+Author: MIT Data To AI Lab
+Author-email: dai-lab@mit.edu
+Keywords: zephyr Draco Prediction Engineering
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.7,<3.9
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+License-File: LICENSE
+
 <p align="left">
 <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt="DAI-Lab" />
 <i>A project from Data to AI Lab at MIT.</i>
 </p>
 
 <!-- Uncomment these lines after releasing the package to PyPI for version and downloads badges -->
 <!--[![PyPI Shield](https://img.shields.io/pypi/v/zephyr_ml.svg)](https://pypi.python.org/pypi/zephyr_ml)-->
@@ -22,14 +43,15 @@
  | :scroll: **[License]**              | The repository is published under the MIT License.                   |
  | :keyboard: **[Development Status]** | This software is in its Pre-Alpha stage.                             |
  | ![][Slack Logo] **[Community]**    | Join our Slack Workspace for announcements and discussions.          |
 
  [Website]: https://sintel.dev/
  [Documentation]: https://dtail.gitbook.io/zephyr/
  [Repository]: https://github.com/sintel-dev/Zephyr
+ [Tutorials]: https://github.com/sintel-dev/Zephyr/blob/master/notebooks
  [License]: https://github.com/sintel-dev/Zephyr/blob/master/LICENSE
  [Development Status]: https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha
  [Community]: https://join.slack.com/t/sintel-space/shared_invite/zt-q147oimb-4HcphcxPfDAM0O9_4PaUtw
  [Slack Logo]: https://github.com/sintel-dev/Orion/blob/master/docs/images/slack.png
 
  - Homepage: https://github.com/signals-dev/zephyr
 
@@ -145,24 +167,25 @@
 This will return us a dictionary with the name and a short description of each available
 function.
 
 ```
 {'brake_pad_presence': 'Calculates the total power loss over the data slice.',
  'converter_replacement_presence': 'Calculates the converter replacement presence.',
  'total_power_loss': 'Calculates the total power loss over the data slice.'}
- ```
+```
 
 In this case, we will choose the `total_power_loss` function, which calculates the total
 amount of power lost over a slice of time.
 
 ## 3. Generate Target Times
 
 Once we have loaded the data and the Labeling Function, we are ready to start using
 the `zephyr_ml.generate_labels` function to generate a Target Times table.
 
+
 ```python3
 from zephyr_ml import DataLabeler
 
 data_labeler = DataLabeler(labeling.labeling_functions.total_power_loss)
 target_times, metadata = data_labeler.generate_label_times(scada_es)
 ```
 
@@ -170,12 +193,90 @@
 working on a Machine Learning problem: the turbine ID (COD_ELEMENT), the cutoff time (time) and the label.
 
 ```
    COD_ELEMENT       time    label
 0            0 2022-01-01  45801.0
 ```
 
+## 4. Feature Engineering
+Using EntitySets and LabelTimes allows us to easily use Featuretools for automatic feature generation.
+
+```python3
+import featuretools as ft
+
+feature_matrix, features = ft.dfs(
+    entityset=scada_es,
+    target_dataframe_name='turbines',
+    cutoff_time_in_index=True,
+    cutoff_time=target_times,
+    max_features=20
+)
+```
+
+Then we get a list of features and the computed `feature_matrix`.
+
+```
+                       TURBINE_PI_ID TURBINE_LOCAL_ID TURBINE_SAP_COD DES_CORE_ELEMENT      SITE DES_CORE_PLANT  ... MODE(alarms.COD_STATUS) MODE(alarms.DES_NAME)  MODE(alarms.DES_TITLE)  NUM_UNIQUE(alarms.COD_ALARM)  NUM_UNIQUE(alarms.COD_ALARM_INT)    label
+COD_ELEMENT time                                                                                                 ...                                                                                                                                               
+0           2022-01-01          TA00               A0          LOC000              T00  LOCATION            LOC  ...                  Alarm1                Alarm1  Description of alarm 1                             1                                 1  45801.0
+
+[1 rows x 21 columns]
+```
+
+
+## 5. Modeling
+
+Once we have the feature matrix, we can train a model using the Zephyr interface where you can train, infer, and evaluate a pipeline. 
+First, we need to prepare our dataset for training by creating ``X`` and ``y`` variables and one-hot encoding features.
+
+```python3
+y = list(feature_matrix.pop('label'))
+X = pd.get_dummies(feature_matrix).values
+```
+
+In this example, we will use an 'xgb' regression pipeline to predict total power loss.
+
+```python3
+from zephyr_ml import Zephyr
+
+pipeline_name = 'xgb_regressor'
+
+zephyr = Zephyr(pipeline_name)
+```
+
+To train the pipeline, we simply use the `fit` function.
+```python3
+zephyr.fit(X, y)
+```
+
+After it finished training,  we can make prediciton using `predict`
+
+```python3
+y_pred =  zephyr.predict(X)
+```
+
+We can also use ``zephyr.evaluate`` to obtain the performance of the pipeline.
+
 # What's Next?
 
 If you want to continue learning about **Zephyr** and all its
 features please have a look at the tutorials found inside the [notebooks folder](
 https://github.com/signals-dev/zephyr/tree/main/notebooks).
+
+
+# History
+
+## 0.0.1 - 2023-03-02
+
+New modeling module using Zephyr class
+
+* Expand GH action tests - [Issue #4](https://github.com/signals-dev/Zephyr/issues/4) by @sarahmish 
+* Add XGB Pipeline - [Issue #1](https://github.com/signals-dev/Zephyr/issues/1) by @sarahmish
+
+
+## 0.0.0 - 2022-11-17
+
+First full release
+
+* Prediction Engineering Framework by @frances-h 
+* EntitySet creation by @frances-h 
+* DataLabeler and initial labeling functions by @frances-h
```

### Comparing `zephyr-ml-0.0.1.dev0/docs/Makefile` & `zephyr-ml-0.0.2.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/docs/conf.py` & `zephyr-ml-0.0.2.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/docs/images/dai-logo-white-200.png` & `zephyr-ml-0.0.2.dev0/docs/images/dai-logo-white-200.png`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/docs/make.bat` & `zephyr-ml-0.0.2.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/setup.cfg` & `zephyr-ml-0.0.2.dev0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.1.dev0
+current_version = 0.0.2.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `zephyr-ml-0.0.1.dev0/setup.py` & `zephyr-ml-0.0.2.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 install_requires = [
     'numpy>=1.16.0,<1.23.0',
     'pandas>=1,<2',
     'composeml>=0.1.6,<0.10',
     'featuretools>=1.0.0,<2.0.0',
     'mlblocks>=0.5.0,<0.6',
+    'sigpro>=0.1.1.dev0',
     'xgboost>=0.72.1,<1',
     'jupyter==1.0.0',
 ]
 
 setup_requires = [
     'pytest-runner>=2.11.1',
 ]
@@ -105,10 +106,10 @@
     name='zephyr-ml',
     packages=find_packages(include=['zephyr_ml', 'zephyr_ml.*']),
     python_requires='>=3.7,<3.9',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sintel-dev/zephyr',
-    version='0.0.1.dev0',
+    version='0.0.2.dev0',
     zip_safe=False,
 )
```

### Comparing `zephyr-ml-0.0.1.dev0/tests/labeling/test_helpers.py` & `zephyr-ml-0.0.2.dev0/tests/labeling/test_helpers.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/tests/primitives/test_postprocessing.py` & `zephyr-ml-0.0.2.dev0/tests/primitives/test_postprocessing.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,14 +19,15 @@
                          [0.8, 0.2]])
 
     def _run(self, y, y_hat, value):
         threshold = FindThreshold()
         threshold.fit(y, y_hat)
 
         assert threshold._threshold == value
-        np.testing.assert_allclose(threshold.apply_threshold(y_hat), y)
+        binary_y_hat, detected_threshold, scores = threshold.apply_threshold(y_hat)
+        np.testing.assert_allclose(binary_y_hat, y)
 
     def test_1d(self):
         self._run(self.y, self.y_hat_1d, 0.6)
 
     def test_2d(self):
         self._run(self.y, self.y_hat_2d, 0.6)
```

### Comparing `zephyr-ml-0.0.1.dev0/tests/test___init__.py` & `zephyr-ml-0.0.2.dev0/tests/test___init__.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/tests/test_core.py` & `zephyr-ml-0.0.2.dev0/tests/test_core.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,48 +28,80 @@
             'feature 1': list(range(100)),
             'feature 2': np.random.random(100),
             'feature 3': np.random.random(100),
         })
         cls.random_y = [1 if x > 0.5 else 0 for x in np.random.random(100)]
 
     def setup(self):
-        self.zephyr = Zephyr('xgb')
+        self.zephyr = Zephyr('xgb_classifier')
 
     def test_hyperparameters(self):
         hyperparameters = {
             "xgboost.XGBClassifier#1": {
                 "max_depth": 2
             },
             "zephyr_ml.primitives.postprocessing.FindThreshold#1": {
                 "metric": "precision"
             }
         }
 
-        zephyr = Zephyr('xgb', hyperparameters)
+        zephyr = Zephyr('xgb_classifier', hyperparameters)
 
         assert zephyr._hyperparameters == hyperparameters
 
     def test_json(self):
         file = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-        json_zephyr = Zephyr(os.path.join(file, 'zephyr_ml', 'pipelines', 'xgb.json'))
+        json_zephyr = Zephyr(os.path.join(file, 'zephyr_ml', 'pipelines', 'xgb_classifier.json'))
 
         json_zephyr_hyperparameters = json_zephyr._mlpipeline.get_hyperparameters()
         zephyr_hyperparameters = self.zephyr._mlpipeline.get_hyperparameters()
         assert json_zephyr_hyperparameters == zephyr_hyperparameters
 
     def test_fit(self):
         self.zephyr.fit(self.train, self.train_y)
 
+    def test_fit_visual(self):
+        output = self.zephyr.fit(self.train, self.train_y, visual=True)
+
+        assert isinstance(output, dict)
+        assert list(output.keys()) == ['threshold', 'scores']
+
+    def test_fit_no_visual(self):
+        zephyr = Zephyr(['xgboost.XGBClassifier'])
+
+        output = zephyr.fit(self.train, self.train_y, visual=True)
+        assert output is None
+
     def test_predict(self):
         self.zephyr.fit(self.train, self.train_y)
 
         predicted = self.zephyr.predict(self.test)
 
         assert self.test_y == predicted
 
+    def test_predict_visual(self):
+        self.zephyr.fit(self.train, self.train_y)
+
+        predicted, output = self.zephyr.predict(self.test, visual=True)
+
+        # predictions
+        assert self.test_y == predicted
+
+        # visualization
+        assert isinstance(output, dict)
+        assert list(output.keys()) == ['threshold', 'scores']
+
+    def test_predict_no_visual(self):
+        zephyr = Zephyr(['xgboost.XGBClassifier'])
+
+        zephyr.fit(self.train, self.train_y)
+
+        predicted = zephyr.predict(self.test, visual=True)
+        assert len(self.test_y) == len(predicted)
+
     def test_fit_predict(self):
         predicted = self.zephyr.fit_predict(self.random, self.random_y)
 
         assert isinstance(predicted, list)
 
     def test_save_load(self, tmpdir):
         path = os.path.join(tmpdir, 'some_path.pkl')
```

### Comparing `zephyr-ml-0.0.1.dev0/tests/test_entityset.py` & `zephyr-ml-0.0.2.dev0/tests/test_entityset.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/tests/test_metadata.py` & `zephyr-ml-0.0.2.dev0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/zephyr_ml/core.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 * An ``str`` with a path to a JSON file.
                 * An ``str`` with the name of a registered pipeline.
                 * An ``MLPipeline`` instance.
                 * A ``dict`` with an ``MLPipeline`` specification.
         hyperparameters (dict):
             Additional hyperparameters to set to the Pipeline.
     """
-    DEFAULT_PIPELINE = 'xgb'
+    DEFAULT_PIPELINE = 'xgb_classifier'
 
     def _get_mlpipeline(self):
         pipeline = self._pipeline
         if isinstance(pipeline, str) and os.path.isfile(pipeline):
             with open(pipeline) as json_file:
                 pipeline = json.load(json_file)
 
@@ -76,44 +76,81 @@
         return (
             isinstance(other, self.__class__) and
             self._pipeline == other._pipeline and
             self._hyperparameters == other._hyperparameters and
             self._fitted == other._fitted
         )
 
-    def fit(self, X: pd.DataFrame, y: Union[pd.Series, np.ndarray], **kwargs):
+    def _get_outputs_spec(self, default=True):
+        outputs_spec = ["default"] if default else []
+
+        try:
+            visual_names = self._mlpipeline.get_output_names('visual')
+            outputs_spec.append('visual')
+        except ValueError:
+            visual_names = []
+
+        return outputs_spec, visual_names
+
+    def fit(self, X: pd.DataFrame, y: Union[pd.Series, np.ndarray],
+            visual: bool = False, **kwargs):
         """Fit the pipeline to the given data.
 
         Args:
             X (DataFrame):
                 Input data, passed as a ``pandas.DataFrame`` containing
                 the feature matrix.
             y (Series or ndarray):
                 Target data, passed as a ``pandas.Series`` or ``numpy.ndarray``
                 containing the target values.
+            visual (bool):
+                If ``True``, capture the ``visual`` named output from the
+                ``MLPipeline`` and return it as an output.
         """
         if not self._fitted:
             self._mlpipeline = self._get_mlpipeline()
 
-        self._mlpipeline.fit(X, y, **kwargs)
+        if visual:
+            outputs_spec, visual_names = self._get_outputs_spec(False)
+        else:
+            outputs_spec = None
+
+        outputs = self._mlpipeline.fit(X, y, output_=outputs_spec, **kwargs)
         self._fitted = True
 
-    def predict(self, X: pd.DataFrame) -> pd.Series:
+        if visual and outputs is not None:
+            return dict(zip(visual_names, outputs))
+
+    def predict(self, X: pd.DataFrame, visual: bool = False, **kwargs) -> pd.Series:
         """Predict the pipeline to the given data.
 
         Args:
             X (DataFrame):
                 Input data, passed as a ``pandas.DataFrame`` containing
                 the feature matrix.
+        visual (bool):
+                If ``True``, capture the ``visual`` named output from the
+                ``MLPipeline`` and return it as an output.
 
         Returns:
             Series or ndarray:
                 Predictions to the input data.
         """
-        return self._mlpipeline.predict(X)
+        if visual:
+            outputs_spec, visual_names = self._get_outputs_spec()
+        else:
+            outputs_spec = 'default'
+
+        outputs = self._mlpipeline.predict(X, output_=outputs_spec, **kwargs)
+
+        if visual and visual_names:
+            prediction = outputs[0]
+            return prediction, dict(zip(visual_names, outputs[-len(visual_names):]))
+
+        return outputs
 
     def fit_predict(self, X: pd.DataFrame, y: Union[pd.Series, np.ndarray],
                     **kwargs) -> pd.Series:
         """Fit the pipeline to the data and then predict targets.
 
         This method is functionally equivalent to calling ``fit(X, y)``
         and later on ``predict(X)`` but with the difference that
```

### Comparing `zephyr-ml-0.0.1.dev0/zephyr_ml/entityset.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/entityset.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/__init__.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/__init__.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/data_labeler.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/data_labeler.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/labeling_functions/brake_pad_presence.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/labeling_functions/brake_pad_presence.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/labeling_functions/converter_replacement_presence.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/labeling_functions/converter_replacement_presence.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/labeling_functions/total_power_loss.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/labeling_functions/total_power_loss.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/zephyr_ml/labeling/utils.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/utils.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/zephyr_ml/metadata.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/metadata.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.1.dev0/zephyr_ml/primitives/postprocessing.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/primitives/postprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,33 +46,37 @@
                 ``pandas.Series`` or ``numpy.ndarray`` predicted target valeus.
         """
         if y_pred.ndim > 1:
             y_pred = y_pred[:, 1]
 
         RANGE = np.arange(0, 1, 0.01)
 
-        values = list()
+        scores = list()
         scorer = METRICS[self._metric]
         for thresh in RANGE:
             y = [1 if x else 0 for x in y_pred > thresh]
-            values.append(scorer(y_true, y))
+            scores.append(scorer(y_true, y))
 
-        threshold = RANGE[np.argmax(values)]
+        threshold = RANGE[np.argmax(scores)]
         LOGGER.info(f'best threshold found at {threshold}')
 
         self._threshold = threshold
+        self._scores = scores
 
     def apply_threshold(self, y_pred):
         """Apply threshold on predicted values.
 
         Args:
             y_pred (Series):
                 ``pandas.Series`` predicted target valeus.
 
         Return:
-            list:
-                predicted target valeus in binary codes.
+            tuple:
+                * list of predicted target valeus in binary codes.
+                * detected float value for threshold.
+                * list of scores obtained at each threshold.
         """
         if y_pred.ndim > 1:
             y_pred = y_pred[:, 1]
 
-        return [1 if x else 0 for x in y_pred > self._threshold]
+        binary = [1 if x else 0 for x in y_pred > self._threshold]
+        return binary, self._threshold, self._scores
```

### Comparing `zephyr-ml-0.0.1.dev0/zephyr_ml.egg-info/PKG-INFO` & `zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyr-ml
-Version: 0.0.1.dev0
+Version: 0.0.2.dev0
 Summary: Prediction engineering methods for Draco.
 Home-page: https://github.com/sintel-dev/zephyr
 Author: MIT Data To AI Lab
 Author-email: dai-lab@mit.edu
 Keywords: zephyr Draco Prediction Engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -43,14 +43,15 @@
  | :scroll: **[License]**              | The repository is published under the MIT License.                   |
  | :keyboard: **[Development Status]** | This software is in its Pre-Alpha stage.                             |
  | ![][Slack Logo] **[Community]**    | Join our Slack Workspace for announcements and discussions.          |
 
  [Website]: https://sintel.dev/
  [Documentation]: https://dtail.gitbook.io/zephyr/
  [Repository]: https://github.com/sintel-dev/Zephyr
+ [Tutorials]: https://github.com/sintel-dev/Zephyr/blob/master/notebooks
  [License]: https://github.com/sintel-dev/Zephyr/blob/master/LICENSE
  [Development Status]: https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha
  [Community]: https://join.slack.com/t/sintel-space/shared_invite/zt-q147oimb-4HcphcxPfDAM0O9_4PaUtw
  [Slack Logo]: https://github.com/sintel-dev/Orion/blob/master/docs/images/slack.png
 
  - Homepage: https://github.com/signals-dev/zephyr
 
@@ -166,24 +167,25 @@
 This will return us a dictionary with the name and a short description of each available
 function.
 
 ```
 {'brake_pad_presence': 'Calculates the total power loss over the data slice.',
  'converter_replacement_presence': 'Calculates the converter replacement presence.',
  'total_power_loss': 'Calculates the total power loss over the data slice.'}
- ```
+```
 
 In this case, we will choose the `total_power_loss` function, which calculates the total
 amount of power lost over a slice of time.
 
 ## 3. Generate Target Times
 
 Once we have loaded the data and the Labeling Function, we are ready to start using
 the `zephyr_ml.generate_labels` function to generate a Target Times table.
 
+
 ```python3
 from zephyr_ml import DataLabeler
 
 data_labeler = DataLabeler(labeling.labeling_functions.total_power_loss)
 target_times, metadata = data_labeler.generate_label_times(scada_es)
 ```
 
@@ -191,14 +193,90 @@
 working on a Machine Learning problem: the turbine ID (COD_ELEMENT), the cutoff time (time) and the label.
 
 ```
    COD_ELEMENT       time    label
 0            0 2022-01-01  45801.0
 ```
 
+## 4. Feature Engineering
+Using EntitySets and LabelTimes allows us to easily use Featuretools for automatic feature generation.
+
+```python3
+import featuretools as ft
+
+feature_matrix, features = ft.dfs(
+    entityset=scada_es,
+    target_dataframe_name='turbines',
+    cutoff_time_in_index=True,
+    cutoff_time=target_times,
+    max_features=20
+)
+```
+
+Then we get a list of features and the computed `feature_matrix`.
+
+```
+                       TURBINE_PI_ID TURBINE_LOCAL_ID TURBINE_SAP_COD DES_CORE_ELEMENT      SITE DES_CORE_PLANT  ... MODE(alarms.COD_STATUS) MODE(alarms.DES_NAME)  MODE(alarms.DES_TITLE)  NUM_UNIQUE(alarms.COD_ALARM)  NUM_UNIQUE(alarms.COD_ALARM_INT)    label
+COD_ELEMENT time                                                                                                 ...                                                                                                                                               
+0           2022-01-01          TA00               A0          LOC000              T00  LOCATION            LOC  ...                  Alarm1                Alarm1  Description of alarm 1                             1                                 1  45801.0
+
+[1 rows x 21 columns]
+```
+
+
+## 5. Modeling
+
+Once we have the feature matrix, we can train a model using the Zephyr interface where you can train, infer, and evaluate a pipeline. 
+First, we need to prepare our dataset for training by creating ``X`` and ``y`` variables and one-hot encoding features.
+
+```python3
+y = list(feature_matrix.pop('label'))
+X = pd.get_dummies(feature_matrix).values
+```
+
+In this example, we will use an 'xgb' regression pipeline to predict total power loss.
+
+```python3
+from zephyr_ml import Zephyr
+
+pipeline_name = 'xgb_regressor'
+
+zephyr = Zephyr(pipeline_name)
+```
+
+To train the pipeline, we simply use the `fit` function.
+```python3
+zephyr.fit(X, y)
+```
+
+After it finished training,  we can make prediciton using `predict`
+
+```python3
+y_pred =  zephyr.predict(X)
+```
+
+We can also use ``zephyr.evaluate`` to obtain the performance of the pipeline.
+
 # What's Next?
 
 If you want to continue learning about **Zephyr** and all its
 features please have a look at the tutorials found inside the [notebooks folder](
 https://github.com/signals-dev/zephyr/tree/main/notebooks).
 
 
+# History
+
+## 0.0.1 - 2023-03-02
+
+New modeling module using Zephyr class
+
+* Expand GH action tests - [Issue #4](https://github.com/signals-dev/Zephyr/issues/4) by @sarahmish 
+* Add XGB Pipeline - [Issue #1](https://github.com/signals-dev/Zephyr/issues/1) by @sarahmish
+
+
+## 0.0.0 - 2022-11-17
+
+First full release
+
+* Prediction Engineering Framework by @frances-h 
+* EntitySet creation by @frances-h 
+* DataLabeler and initial labeling functions by @frances-h
```

### Comparing `zephyr-ml-0.0.1.dev0/zephyr_ml.egg-info/SOURCES.txt` & `zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 CONTRIBUTING.rst
+HISTORY.md
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 docs/Makefile
-docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/make.bat
 docs/readme.rst
 docs/images/dai-logo-white-200.png
 tests/__init__.py
 tests/test___init__.py
 tests/test_core.py
 tests/test_entityset.py
+tests/test_feature_engineering.py
 tests/test_metadata.py
 tests/labeling/__init__.py
 tests/labeling/test_data_labeler.py
 tests/labeling/test_helpers.py
 tests/primitives/test_postprocessing.py
 zephyr_ml/__init__.py
 zephyr_ml/core.py
 zephyr_ml/entityset.py
+zephyr_ml/feature_engineering.py
 zephyr_ml/metadata.py
 zephyr_ml.egg-info/PKG-INFO
 zephyr_ml.egg-info/SOURCES.txt
 zephyr_ml.egg-info/dependency_links.txt
 zephyr_ml.egg-info/entry_points.txt
 zephyr_ml.egg-info/not-zip-safe
 zephyr_ml.egg-info/requires.txt
@@ -36,9 +38,14 @@
 zephyr_ml/labeling/__init__.py
 zephyr_ml/labeling/data_labeler.py
 zephyr_ml/labeling/utils.py
 zephyr_ml/labeling/labeling_functions/__init__.py
 zephyr_ml/labeling/labeling_functions/brake_pad_presence.py
 zephyr_ml/labeling/labeling_functions/converter_replacement_presence.py
 zephyr_ml/labeling/labeling_functions/total_power_loss.py
+zephyr_ml/pipelines/xgb_classifier.json
+zephyr_ml/pipelines/xgb_regressor.json
 zephyr_ml/primitives/__init__.py
-zephyr_ml/primitives/postprocessing.py
+zephyr_ml/primitives/postprocessing.py
+zephyr_ml/primitives/jsons/xgboost.XGBClassifier.json
+zephyr_ml/primitives/jsons/xgboost.XGBRegressor.json
+zephyr_ml/primitives/jsons/zephyr_ml.primitives.postprocessing.FindThreshold.json
```

### Comparing `zephyr-ml-0.0.1.dev0/zephyr_ml.egg-info/requires.txt` & `zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 numpy<1.23.0,>=1.16.0
 pandas<2,>=1
 composeml<0.10,>=0.1.6
 featuretools<2.0.0,>=1.0.0
 mlblocks<0.6,>=0.5.0
+sigpro>=0.1.1.dev0
 xgboost<1,>=0.72.1
 jupyter==1.0.0
 
 [dev]
 bumpversion<0.6,>=0.5.3
 pip>=9.0.1
 watchdog<0.11,>=0.8.3
```

