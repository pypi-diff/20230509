# Comparing `tmp/syngen-0.0.98.tar.gz` & `tmp/syngen-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.0.98.tar", last modified: Fri May  5 17:23:39 2023, max compression
+gzip compressed data, was "syngen-0.0.99.tar", last modified: Tue May  9 12:36:19 2023, max compression
```

## Comparing `syngen-0.0.98.tar` & `syngen-0.0.99.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-05 17:22:19.000000 syngen-0.0.98/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-05 17:22:19.000000 syngen-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-05 17:22:19.000000 syngen-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-05-05 17:23:39.702504 syngen-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-05-05 17:22:19.000000 syngen-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-05 17:22:19.000000 syngen-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-05 17:23:39.702504 syngen-0.0.98/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.686504 syngen-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.694504 syngen-0.0.98/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7287 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.690504 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14647 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5649 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    30207 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10439 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11543 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-05-05 17:23:39.000000 syngen-0.0.98/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-05 17:23:39.000000 syngen-0.0.98/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 17:23:39.000000 syngen-0.0.98/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-05 17:23:39.000000 syngen-0.0.98/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-05 17:23:39.000000 syngen-0.0.98/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-05 17:23:39.000000 syngen-0.0.98/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-09 12:34:38.000000 syngen-0.0.99/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-09 12:34:38.000000 syngen-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-09 12:34:38.000000 syngen-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-05-09 12:36:18.996407 syngen-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-05-09 12:34:38.000000 syngen-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-09 12:34:38.000000 syngen-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-09 12:36:19.000407 syngen-0.0.99/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.980407 syngen-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.984407 syngen-0.0.99/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.984407 syngen-0.0.99/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.988407 syngen-0.0.99/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.988407 syngen-0.0.99/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.988407 syngen-0.0.99/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7287 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.988407 syngen-0.0.99/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.988407 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.980407 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.988407 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.992407 syngen-0.0.99/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.992407 syngen-0.0.99/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.992407 syngen-0.0.99/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.992407 syngen-0.0.99/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7044 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14647 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5649 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30363 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10439 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.984407 syngen-0.0.99/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-05-09 12:36:18.000000 syngen-0.0.99/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-09 12:36:18.000000 syngen-0.0.99/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 12:36:18.000000 syngen-0.0.99/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-09 12:36:18.000000 syngen-0.0.99/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-09 12:36:18.000000 syngen-0.0.99/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-09 12:36:18.000000 syngen-0.0.99/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.0.98/LICENSE` & `syngen-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/PKG-INFO` & `syngen-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.98
+Version: 0.0.99
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.98 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.0.99 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.0.98/README.md` & `syngen-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/setup.cfg` & `syngen-0.0.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/infer.py` & `syngen-0.0.99/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/config/configurations.py` & `syngen-0.0.99/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/convertor/convertor.py` & `syngen-0.0.99/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.0.99/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/metrics/__init__.py` & `syngen-0.0.99/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.0.99/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.0.99/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.0.99/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/metrics/utils.py` & `syngen-0.0.99/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/reporters/reporters.py` & `syngen-0.0.99/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/strategies/strategies.py` & `syngen-0.0.99/src/syngen/ml/strategies/strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import ABC, abstractmethod
 import os
 import traceback
+import random
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
 
 from loguru import logger
 from syngen.ml.train_chain import RootHandler
 from syngen.ml.reporters import (
     Report,
     AccuracyReporter,
@@ -18,14 +19,15 @@
     LongTextsHandler,
     VaeTrainHandler,
     VaeInferHandler
 )
 from syngen.ml.vae import VanillaVAEWrapper
 from syngen.ml.data_loaders import BinaryLoader
 
+RANDOM_STATE = random.randint(0, 2 ** 32 - 1)
 
 class Strategy(ABC):
     """
     Abstract class for the strategies of training or infer process
     """
     def __init__(self):
         self.handler = None
@@ -139,15 +141,16 @@
             source=kwargs["source"],
             epochs=kwargs["epochs"],
             drop_null=kwargs["drop_null"],
             row_limit=kwargs["row_limit"],
             table_name=kwargs["table_name"],
             metadata_path=kwargs["metadata_path"],
             print_report=kwargs["print_report"],
-            batch_size=kwargs["batch_size"]
+            batch_size=kwargs["batch_size"],
+            random_state=RANDOM_STATE
         )
 
         self.add_reporters().\
             set_metadata(kwargs["metadata"]).\
             add_handler()
 
         try:
```

### Comparing `syngen-0.0.98/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.0.99/src/syngen/ml/train_chain/train_chain.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/utils/utils.py` & `syngen-0.0.99/src/syngen/ml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.0.99/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/vae/models/dataset.py` & `syngen-0.0.99/src/syngen/ml/vae/models/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     is_fitted: bool = field(init=False)
     all_columns: List = field(init=False)
     null_num_column_names: List = field(init=False)
     zero_num_column_names: List = field(init=False)
     nan_labels_dict: Dict = field(init=False)
 
     def __post_init__(self):
+        self._predefine_fields()
+        self._set_metadata()
+
+    def _predefine_fields(self):
         self.features = dict()
         self.columns = dict()
         self.is_fitted = False
         self.all_columns = list()
         self.null_num_column_names = list()
         self.zero_num_column_names = list()
         self.nan_labels_dict = dict()
@@ -138,15 +142,15 @@
             self.unique_keys_mapping_list = []
             self.unique_keys_list = []
             self.uq_columns = []
             self.foreign_keys_mapping = {}
             self.foreign_keys_list = []
             self.fk_columns = []
 
-    def set_metadata(self):
+    def _set_metadata(self):
         self.__set_metadata(self.metadata, self.table_name)
         self.__data_pipeline(self.df, self.schema)
 
     @staticmethod
     def _update_schema(schema: Dict[str, Dict[str, str]], df: pd.DataFrame):
         """
         Synchronize the schema of the table with dataframe
@@ -287,14 +291,15 @@
                 if data_type == "string"
             ]
             data_subset = df[text_columns]
         self.long_text_columns = set()
         if not data_subset.empty:
             data_subset = data_subset.loc[:, data_subset.apply(lambda x: (x.str.len() > 200).any())]
             self.long_text_columns = set(data_subset.columns)
+            self.long_text_columns -= self.categ_columns
             if self.long_text_columns:
                 logger.info(
                     f"Please note that the columns - {self.long_text_columns} contain long texts (> 200 symbols). "
                     f"Such texts' handling consumes significant resources and results in poor quality content, "
                     f"therefore this column(-s) will be generated using a simplified statistical approach")
 
     def _general_data_pipeline(self, df: pd.DataFrame, schema: Dict, check_object_on_float: bool = True):
@@ -369,15 +374,15 @@
 
         logger.debug(
             f"Count of string columns: {len(self.str_columns)}; "
             + f"Count of float columns: {len(self.float_columns)}; "
             + f"Count of int columns: {len(self.int_columns)}; "
             + f"Count of categorical columns: {len(self.categ_columns)}; "
             + f"Count of date columns: {len(self.date_columns)}; "
-            + f"Count of binary columns: {len(self.binary_columns)}"
+            + f"Count of binary columns: {len(self.binary_columns)}; "
             + f"Count of long text columns: {len(self.long_text_columns)}"
         )
 
     def assign_feature(self, feature, columns):
         name = feature.original_name
 
         if name in self.features:
```

### Comparing `syngen-0.0.98/src/syngen/ml/vae/models/features.py` & `syngen-0.0.99/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/vae/models/model.py` & `syngen-0.0.99/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.0.99/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,24 +183,17 @@
             df[column_name] = df[column_name].fillna(np.nan) if nan_label is None else df[column_name].fillna(nan_label)
         return df
 
     @abstractmethod
     def _init_model(self):
         pass
 
-    def _set_dataset_metadata(self):
-        """
-        Set metadata for the dataset and save it on the disk
-        """
-        self.dataset.set_metadata()
-        self._save_dataset()
-
     def prepare_dataset(self):
         self.__post__init__()
-        self._set_dataset_metadata()
+        self._save_dataset()
 
     def fit_on_df(
         self,
         df: pd.DataFrame,
         epochs: int,
         columns_subset: List[str] = None,  # TODO columns_subset does not work
     ):
```

### Comparing `syngen-0.0.98/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.0.99/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/ml/worker/worker.py` & `syngen-0.0.99/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen/train.py` & `syngen-0.0.99/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.98/src/syngen.egg-info/PKG-INFO` & `syngen-0.0.99/src/syngen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.98
+Version: 0.0.99
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.98 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.0.99 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.0.98/src/syngen.egg-info/SOURCES.txt` & `syngen-0.0.99/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

