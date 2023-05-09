# Comparing `tmp/zephyr-ml-0.0.2.tar.gz` & `tmp/zephyr-ml-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephyr-ml-0.0.2.tar", last modified: Tue May  9 15:45:19 2023, max compression
+gzip compressed data, was "zephyr-ml-0.0.2.dev0.tar", last modified: Tue May  9 15:14:53 2023, max compression
```

## Comparing `zephyr-ml-0.0.2.tar` & `zephyr-ml-0.0.2.dev0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:45:19.722142 zephyr-ml-0.0.2/
--rw-r--r--   0 sarah      (501) staff       (20)     8318 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/CONTRIBUTING.rst
--rw-r--r--   0 sarah      (501) staff       (20)      741 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/HISTORY.md
--rw-r--r--   0 sarah      (501) staff       (20)     1088 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/LICENSE
--rw-r--r--   0 sarah      (501) staff       (20)      301 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/MANIFEST.in
--rw-r--r--   0 sarah      (501) staff       (20)    11165 2023-05-09 15:45:19.722411 zephyr-ml-0.0.2/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     9705 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/README.md
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:45:19.698200 zephyr-ml-0.0.2/docs/
--rw-r--r--   0 sarah      (501) staff       (20)      607 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/docs/Makefile
--rw-r--r--   0 sarah      (501) staff       (20)     5879 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/docs/conf.py
--rw-r--r--   0 sarah      (501) staff       (20)       33 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/docs/contributing.rst
--rw-r--r--   0 sarah      (501) staff       (20)       29 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/docs/history.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:45:19.699160 zephyr-ml-0.0.2/docs/images/
--rw-r--r--   0 sarah      (501) staff       (20)    33432 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/docs/images/dai-logo-white-200.png
--rw-r--r--   0 sarah      (501) staff       (20)      289 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/docs/index.rst
--rw-r--r--   0 sarah      (501) staff       (20)      768 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/docs/make.bat
--rw-r--r--   0 sarah      (501) staff       (20)       28 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/docs/readme.rst
--rw-r--r--   0 sarah      (501) staff       (20)     1009 2023-05-09 15:45:19.723695 zephyr-ml-0.0.2/setup.cfg
--rw-r--r--   0 sarah      (501) staff       (20)     2717 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/setup.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:45:19.703884 zephyr-ml-0.0.2/tests/
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/tests/__init__.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:45:19.705691 zephyr-ml-0.0.2/tests/labeling/
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/tests/labeling/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)      416 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/tests/labeling/test_data_labeler.py
--rw-r--r--   0 sarah      (501) staff       (20)     4174 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/tests/labeling/test_helpers.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:45:19.706221 zephyr-ml-0.0.2/tests/primitives/
--rw-r--r--   0 sarah      (501) staff       (20)      991 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/tests/primitives/test_postprocessing.py
--rw-r--r--   0 sarah      (501) staff       (20)     5363 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/tests/test___init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     5252 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/tests/test_core.py
--rw-r--r--   0 sarah      (501) staff       (20)     8708 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/tests/test_entityset.py
--rw-r--r--   0 sarah      (501) staff       (20)    10024 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/tests/test_feature_engineering.py
--rw-r--r--   0 sarah      (501) staff       (20)     1926 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/tests/test_metadata.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:45:19.710005 zephyr-ml-0.0.2/zephyr_ml/
--rw-r--r--   0 sarah      (501) staff       (20)      477 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/zephyr_ml/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     9156 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/zephyr_ml/core.py
--rw-r--r--   0 sarah      (501) staff       (20)     5246 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/zephyr_ml/entityset.py
--rw-r--r--   0 sarah      (501) staff       (20)     2592 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/zephyr_ml/feature_engineering.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:45:19.714836 zephyr-ml-0.0.2/zephyr_ml/labeling/
--rw-r--r--   0 sarah      (501) staff       (20)      994 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/zephyr_ml/labeling/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     2739 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/zephyr_ml/labeling/data_labeler.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:45:19.716910 zephyr-ml-0.0.2/zephyr_ml/labeling/labeling_functions/
--rw-r--r--   0 sarah      (501) staff       (20)      291 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/zephyr_ml/labeling/labeling_functions/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     1786 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/zephyr_ml/labeling/labeling_functions/brake_pad_presence.py
--rw-r--r--   0 sarah      (501) staff       (20)     2128 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/zephyr_ml/labeling/labeling_functions/converter_replacement_presence.py
--rw-r--r--   0 sarah      (501) staff       (20)     1639 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/zephyr_ml/labeling/labeling_functions/total_power_loss.py
--rw-r--r--   0 sarah      (501) staff       (20)     7299 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/zephyr_ml/labeling/utils.py
--rw-r--r--   0 sarah      (501) staff       (20)     5766 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/zephyr_ml/metadata.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:45:19.718130 zephyr-ml-0.0.2/zephyr_ml/pipelines/
--rw-r--r--   0 sarah      (501) staff       (20)     1013 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/zephyr_ml/pipelines/xgb_classifier.json
--rw-r--r--   0 sarah      (501) staff       (20)      281 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/zephyr_ml/pipelines/xgb_regressor.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:45:19.719297 zephyr-ml-0.0.2/zephyr_ml/primitives/
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-03-29 21:30:32.000000 zephyr-ml-0.0.2/zephyr_ml/primitives/__init__.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:45:19.721568 zephyr-ml-0.0.2/zephyr_ml/primitives/jsons/
--rw-r--r--   0 sarah      (501) staff       (20)     2715 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/zephyr_ml/primitives/jsons/xgboost.XGBClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     2220 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/zephyr_ml/primitives/jsons/xgboost.XGBRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     1335 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/zephyr_ml/primitives/jsons/zephyr_ml.primitives.postprocessing.FindThreshold.json
--rw-r--r--   0 sarah      (501) staff       (20)     2314 2023-05-09 15:43:45.000000 zephyr-ml-0.0.2/zephyr_ml/primitives/postprocessing.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-09 15:45:19.713013 zephyr-ml-0.0.2/zephyr_ml.egg-info/
--rw-r--r--   0 sarah      (501) staff       (20)    11165 2023-05-09 15:45:19.000000 zephyr-ml-0.0.2/zephyr_ml.egg-info/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     1521 2023-05-09 15:45:19.000000 zephyr-ml-0.0.2/zephyr_ml.egg-info/SOURCES.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-05-09 15:45:19.000000 zephyr-ml-0.0.2/zephyr_ml.egg-info/dependency_links.txt
--rw-r--r--   0 sarah      (501) staff       (20)       95 2023-05-09 15:45:19.000000 zephyr-ml-0.0.2/zephyr_ml.egg-info/entry_points.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-05-09 15:45:19.000000 zephyr-ml-0.0.2/zephyr_ml.egg-info/not-zip-safe
--rw-r--r--   0 sarah      (501) staff       (20)      648 2023-05-09 15:45:19.000000 zephyr-ml-0.0.2/zephyr_ml.egg-info/requires.txt
--rw-r--r--   0 sarah      (501) staff       (20)       10 2023-05-09 15:45:19.000000 zephyr-ml-0.0.2/zephyr_ml.egg-info/top_level.txt
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

### Comparing `zephyr-ml-0.0.2/CONTRIBUTING.rst` & `zephyr-ml-0.0.2.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/LICENSE` & `zephyr-ml-0.0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/PKG-INFO` & `zephyr-ml-0.0.2.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyr-ml
-Version: 0.0.2
+Version: 0.0.2.dev0
 Summary: Prediction engineering methods for Draco.
 Home-page: https://github.com/sintel-dev/zephyr
 Author: MIT Data To AI Lab
 Author-email: dai-lab@mit.edu
 Keywords: zephyr Draco Prediction Engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -261,22 +261,14 @@
 If you want to continue learning about **Zephyr** and all its
 features please have a look at the tutorials found inside the [notebooks folder](
 https://github.com/signals-dev/zephyr/tree/main/notebooks).
 
 
 # History
 
-## 0.0.2 - 2023-05-09
-
-SigPro integration for processing signals
-
-* Integrating SigPro - [Issue #7](https://github.com/signals-dev/Zephyr/issues/7) by @frances-h @sarahmish 
-* Add options to xgb pipeline - [Issue #5](https://github.com/signals-dev/Zephyr/issues/5) by @sarahmish
-
-
 ## 0.0.1 - 2023-03-02
 
 New modeling module using Zephyr class
 
 * Expand GH action tests - [Issue #4](https://github.com/signals-dev/Zephyr/issues/4) by @sarahmish 
 * Add XGB Pipeline - [Issue #1](https://github.com/signals-dev/Zephyr/issues/1) by @sarahmish
```

### Comparing `zephyr-ml-0.0.2/README.md` & `zephyr-ml-0.0.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/docs/Makefile` & `zephyr-ml-0.0.2.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/docs/conf.py` & `zephyr-ml-0.0.2.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/docs/images/dai-logo-white-200.png` & `zephyr-ml-0.0.2.dev0/docs/images/dai-logo-white-200.png`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/docs/make.bat` & `zephyr-ml-0.0.2.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/setup.cfg` & `zephyr-ml-0.0.2.dev0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.2
+current_version = 0.0.2.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `zephyr-ml-0.0.2/setup.py` & `zephyr-ml-0.0.2.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,10 +106,10 @@
     name='zephyr-ml',
     packages=find_packages(include=['zephyr_ml', 'zephyr_ml.*']),
     python_requires='>=3.7,<3.9',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sintel-dev/zephyr',
-    version='0.0.2',
+    version='0.0.2.dev0',
     zip_safe=False,
 )
```

### Comparing `zephyr-ml-0.0.2/tests/labeling/test_helpers.py` & `zephyr-ml-0.0.2.dev0/tests/labeling/test_helpers.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/tests/primitives/test_postprocessing.py` & `zephyr-ml-0.0.2.dev0/tests/primitives/test_postprocessing.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/tests/test___init__.py` & `zephyr-ml-0.0.2.dev0/tests/test___init__.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/tests/test_core.py` & `zephyr-ml-0.0.2.dev0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/tests/test_entityset.py` & `zephyr-ml-0.0.2.dev0/tests/test_entityset.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/tests/test_feature_engineering.py` & `zephyr-ml-0.0.2.dev0/tests/test_feature_engineering.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/tests/test_metadata.py` & `zephyr-ml-0.0.2.dev0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/core.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/core.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/entityset.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/entityset.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/feature_engineering.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/labeling/__init__.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/__init__.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/labeling/data_labeler.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/data_labeler.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/labeling/labeling_functions/brake_pad_presence.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/labeling_functions/brake_pad_presence.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/labeling/labeling_functions/converter_replacement_presence.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/labeling_functions/converter_replacement_presence.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/labeling/labeling_functions/total_power_loss.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/labeling_functions/total_power_loss.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/labeling/utils.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/labeling/utils.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/metadata.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/metadata.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/pipelines/xgb_classifier.json` & `zephyr-ml-0.0.2.dev0/zephyr_ml/pipelines/xgb_classifier.json`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/primitives/jsons/xgboost.XGBClassifier.json` & `zephyr-ml-0.0.2.dev0/zephyr_ml/primitives/jsons/xgboost.XGBClassifier.json`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/primitives/jsons/xgboost.XGBRegressor.json` & `zephyr-ml-0.0.2.dev0/zephyr_ml/primitives/jsons/xgboost.XGBRegressor.json`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/primitives/jsons/zephyr_ml.primitives.postprocessing.FindThreshold.json` & `zephyr-ml-0.0.2.dev0/zephyr_ml/primitives/jsons/zephyr_ml.primitives.postprocessing.FindThreshold.json`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml/primitives/postprocessing.py` & `zephyr-ml-0.0.2.dev0/zephyr_ml/primitives/postprocessing.py`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml.egg-info/PKG-INFO` & `zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyr-ml
-Version: 0.0.2
+Version: 0.0.2.dev0
 Summary: Prediction engineering methods for Draco.
 Home-page: https://github.com/sintel-dev/zephyr
 Author: MIT Data To AI Lab
 Author-email: dai-lab@mit.edu
 Keywords: zephyr Draco Prediction Engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -261,22 +261,14 @@
 If you want to continue learning about **Zephyr** and all its
 features please have a look at the tutorials found inside the [notebooks folder](
 https://github.com/signals-dev/zephyr/tree/main/notebooks).
 
 
 # History
 
-## 0.0.2 - 2023-05-09
-
-SigPro integration for processing signals
-
-* Integrating SigPro - [Issue #7](https://github.com/signals-dev/Zephyr/issues/7) by @frances-h @sarahmish 
-* Add options to xgb pipeline - [Issue #5](https://github.com/signals-dev/Zephyr/issues/5) by @sarahmish
-
-
 ## 0.0.1 - 2023-03-02
 
 New modeling module using Zephyr class
 
 * Expand GH action tests - [Issue #4](https://github.com/signals-dev/Zephyr/issues/4) by @sarahmish 
 * Add XGB Pipeline - [Issue #1](https://github.com/signals-dev/Zephyr/issues/1) by @sarahmish
```

### Comparing `zephyr-ml-0.0.2/zephyr_ml.egg-info/SOURCES.txt` & `zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zephyr-ml-0.0.2/zephyr_ml.egg-info/requires.txt` & `zephyr-ml-0.0.2.dev0/zephyr_ml.egg-info/requires.txt`

 * *Files identical despite different names*

