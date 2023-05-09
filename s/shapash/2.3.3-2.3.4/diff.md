# Comparing `tmp/shapash-2.3.3.tar.gz` & `tmp/shapash-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapash-2.3.3.tar", last modified: Thu May  4 12:36:53 2023, max compression
+gzip compressed data, was "shapash-2.3.4.tar", last modified: Tue May  9 15:43:45 2023, max compression
```

## Comparing `shapash-2.3.3.tar` & `shapash-2.3.4.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.448022 shapash-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-04 12:33:20.000000 shapash-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-04 12:33:20.000000 shapash-2.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-05-04 12:36:53.448022 shapash-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20716 2023-05-04 12:33:20.000000 shapash-2.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-04 12:36:53.448022 shapash-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-04 12:33:20.000000 shapash-2.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.432022 shapash-2.3.3/shapash/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.432022 shapash-2.3.3/shapash/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/backend/acv_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/backend/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/backend/lime_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/backend/shap_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.432022 shapash-2.3.3/shapash/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/data/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.432022 shapash-2.3.3/shapash/decomposition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/decomposition/contributions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.436022 shapash-2.3.3/shapash/explainer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/explainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31311 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/explainer/consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/explainer/multi_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    58279 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/explainer/smart_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)   147181 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/explainer/smart_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/explainer/smart_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/explainer/smart_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.436022 shapash-2.3.3/shapash/manipulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/manipulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/manipulation/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/manipulation/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/manipulation/select_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/manipulation/summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.440022 shapash-2.3.3/shapash/report/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/base_report.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.440022 shapash-2.3.3/shapash/report/html/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/html/double_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/html/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/html/explainability.html
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/html/table_two_columns.html
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/html/univariate.html
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/project_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.428022 shapash-2.3.3/shapash/report/template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.440022 shapash-2.3.3/shapash/report/template/custom/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/template/custom/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/template/custom/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/report/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.440022 shapash-2.3.3/shapash/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/style/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/style/colors.json
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/style/style_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.444022 shapash-2.3.3/shapash/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/utils/category_encoder_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    19318 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/utils/columntransformer_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/utils/explanation_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/utils/load_smartpredictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/utils/model_synoptic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/utils/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)    13696 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/utils/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/utils/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.444022 shapash-2.3.3/shapash/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.444022 shapash-2.3.3/shapash/webapp/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   215609 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    88144 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/assets/jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/assets/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/assets/material-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/assets/reload.png
--rw-r--r--   0 runner    (1001) docker     (123)    29911 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/assets/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)   215609 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/assets/shapash-fond-fonce.png
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/assets/style.css
--rw-r--r--   0 runner    (1001) docker     (123)   138568 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/smart_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.448022 shapash-2.3.3/shapash/webapp/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/utils/MyGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/utils/explanations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/webapp_launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-04 12:33:20.000000 shapash-2.3.3/shapash/webapp/webapp_launch_DVF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:36:53.432022 shapash-2.3.3/shapash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-05-04 12:36:53.000000 shapash-2.3.3/shapash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-04 12:36:53.000000 shapash-2.3.3/shapash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:36:53.000000 shapash-2.3.3/shapash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:36:53.000000 shapash-2.3.3/shapash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-04 12:36:53.000000 shapash-2.3.3/shapash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 12:36:53.000000 shapash-2.3.3/shapash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.627162 shapash-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-09 15:40:53.000000 shapash-2.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-09 15:40:53.000000 shapash-2.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-05-09 15:43:45.627162 shapash-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20716 2023-05-09 15:40:53.000000 shapash-2.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-09 15:43:45.627162 shapash-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-09 15:40:53.000000 shapash-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.619162 shapash-2.3.4/shapash/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.619162 shapash-2.3.4/shapash/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/backend/acv_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/backend/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/backend/lime_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/backend/shap_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.619162 shapash-2.3.4/shapash/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/data/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.619162 shapash-2.3.4/shapash/decomposition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/decomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/decomposition/contributions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.623162 shapash-2.3.4/shapash/explainer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31311 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/multi_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58279 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/smart_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147181 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/smart_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/smart_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/smart_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.623162 shapash-2.3.4/shapash/manipulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/manipulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/manipulation/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/manipulation/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/manipulation/select_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/manipulation/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.623162 shapash-2.3.4/shapash/report/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/base_report.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.623162 shapash-2.3.4/shapash/report/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/html/double_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/html/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/html/explainability.html
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/html/table_two_columns.html
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/html/univariate.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/project_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.619162 shapash-2.3.4/shapash/report/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.623162 shapash-2.3.4/shapash/report/template/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/template/custom/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/template/custom/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.623162 shapash-2.3.4/shapash/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/style/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/style/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/style/style_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.627162 shapash-2.3.4/shapash/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/category_encoder_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/columntransformer_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/explanation_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/load_smartpredictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/model_synoptic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13696 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.627162 shapash-2.3.4/shapash/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.627162 shapash-2.3.4/shapash/webapp/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   215609 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    88144 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/material-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/reload.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29911 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)   215609 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/shapash-fond-fonce.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)   138568 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/smart_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.627162 shapash-2.3.4/shapash/webapp/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/utils/MyGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/utils/explanations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/webapp_launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/webapp_launch_DVF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.619162 shapash-2.3.4/shapash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-05-09 15:43:45.000000 shapash-2.3.4/shapash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-09 15:43:45.000000 shapash-2.3.4/shapash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:43:45.000000 shapash-2.3.4/shapash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:43:45.000000 shapash-2.3.4/shapash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-09 15:43:45.000000 shapash-2.3.4/shapash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 15:43:45.000000 shapash-2.3.4/shapash.egg-info/top_level.txt
```

### Comparing `shapash-2.3.3/LICENSE` & `shapash-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/PKG-INFO` & `shapash-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapash
-Version: 2.3.3
+Version: 2.3.4
 Summary: Shapash is a Python library which aims to make machine learning interpretable and understandable by everyone.
 Home-page: https://github.com/MAIF/shapash
 Author: Yann Golhen, Sebastien Bidault, Yann Lagre, Maxime Gendre
 Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0
 Keywords: shapash
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shapash Version: 2.3.3 Summary: Shapash is a Python
+Metadata-Version: 2.1 Name: shapash Version: 2.3.4 Summary: Shapash is a Python
 library which aims to make machine learning interpretable and understandable by
 everyone. Home-page: https://github.com/MAIF/shapash Author: Yann Golhen,
 Sebastien Bidault, Yann Lagre, Maxime Gendre Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0 Keywords: shapash Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
```

### Comparing `shapash-2.3.3/README.md` & `shapash-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/setup.py` & `shapash-2.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open(os.path.join(here, 'shapash', "__version__.py")) as f:
     exec(f.read(), version_d)
 
 
 requirements = [
     'plotly>=5.0.0',
     'matplotlib>=3.2.0',
-    'numpy>1.18.0',
+    'numpy>1.18.0,<1.24.0',
     'pandas>1.0.2,<2.0.0',
     'shap>=0.38.1',
     'Flask<2.3.0',
     'dash>=2.3.1',
     'dash-bootstrap-components>=1.1.0',
     'dash-core-components>=2.0.0',
     'dash-daq>=0.5.0',
```

### Comparing `shapash-2.3.3/shapash/backend/__init__.py` & `shapash-2.3.4/shapash/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/backend/acv_backend.py` & `shapash-2.3.4/shapash/backend/acv_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/backend/base_backend.py` & `shapash-2.3.4/shapash/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/backend/lime_backend.py` & `shapash-2.3.4/shapash/backend/lime_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/backend/shap_backend.py` & `shapash-2.3.4/shapash/backend/shap_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/data/data_loader.py` & `shapash-2.3.4/shapash/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/decomposition/contributions.py` & `shapash-2.3.4/shapash/decomposition/contributions.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/explainer/consistency.py` & `shapash-2.3.4/shapash/explainer/consistency.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/explainer/multi_decorator.py` & `shapash-2.3.4/shapash/explainer/multi_decorator.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/explainer/smart_explainer.py` & `shapash-2.3.4/shapash/explainer/smart_explainer.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/explainer/smart_plotter.py` & `shapash-2.3.4/shapash/explainer/smart_plotter.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/explainer/smart_predictor.py` & `shapash-2.3.4/shapash/explainer/smart_predictor.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/explainer/smart_state.py` & `shapash-2.3.4/shapash/explainer/smart_state.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/manipulation/filters.py` & `shapash-2.3.4/shapash/manipulation/filters.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/manipulation/mask.py` & `shapash-2.3.4/shapash/manipulation/mask.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/manipulation/select_lines.py` & `shapash-2.3.4/shapash/manipulation/select_lines.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/manipulation/summarize.py` & `shapash-2.3.4/shapash/manipulation/summarize.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/report/__init__.py` & `shapash-2.3.4/shapash/report/__init__.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/report/base_report.ipynb` & `shapash-2.3.4/shapash/report/base_report.ipynb`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/report/common.py` & `shapash-2.3.4/shapash/report/common.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/report/data_analysis.py` & `shapash-2.3.4/shapash/report/data_analysis.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/report/generation.py` & `shapash-2.3.4/shapash/report/generation.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/report/html/dropdown.html` & `shapash-2.3.4/shapash/report/html/dropdown.html`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/report/html/explainability.html` & `shapash-2.3.4/shapash/report/html/explainability.html`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/report/html/univariate.html` & `shapash-2.3.4/shapash/report/html/univariate.html`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/report/plots.py` & `shapash-2.3.4/shapash/report/plots.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/report/project_report.py` & `shapash-2.3.4/shapash/report/project_report.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/report/template/custom/index.html.j2` & `shapash-2.3.4/shapash/report/template/custom/index.html.j2`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/report/visualisation.py` & `shapash-2.3.4/shapash/report/visualisation.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/style/colors.json` & `shapash-2.3.4/shapash/style/colors.json`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/style/style_utils.py` & `shapash-2.3.4/shapash/style/style_utils.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/utils/category_encoder_backend.py` & `shapash-2.3.4/shapash/utils/category_encoder_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/utils/check.py` & `shapash-2.3.4/shapash/utils/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,21 +131,21 @@
         if not isinstance(y, (pd.DataFrame, pd.Series)):
             raise ValueError(f"{y_name} must be a one column pd.Dataframe or pd.Series.")
         if not y.index.equals(x.index):
             raise ValueError(f"x and {y_name} should have the same index.")
         if isinstance(y, pd.DataFrame):
             if y.shape[1] > 1:
                 raise ValueError(f"{y_name} must be a one column pd.Dataframe or pd.Series.")
-            if not (y.dtypes[0] in [np.float, np.int, np.int32, np.float32, np.int64, np.float64]):
+            if not (y.dtypes[0] in [float, int, np.int32, np.float32, np.int64, np.float64]):
                 raise ValueError(f"{y_name} must contain int or float only")
         if isinstance(y, pd.Series):
-            if not (y.dtype in [np.float, np.int, np.int32, np.float32, np.int64, np.float64]):
+            if not (y.dtype in [float, int, np.int32, np.float32, np.int64, np.float64]):
                 raise ValueError(f"{y_name} must contain int or float only")
             y = y.to_frame()
-            if isinstance(y.columns[0], (np.int, np.float)):
+            if isinstance(y.columns[0], (int, float)):
                 y.columns = [y_name]
     return y
 
 def check_contribution_object(case, classes, contributions):
     """
     Check len of list if _case is "classification"
     Check contributions object type if _case is "regression"
```

### Comparing `shapash-2.3.3/shapash/utils/columntransformer_backend.py` & `shapash-2.3.4/shapash/utils/columntransformer_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/utils/explanation_metrics.py` & `shapash-2.3.4/shapash/utils/explanation_metrics.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/utils/io.py` & `shapash-2.3.4/shapash/utils/io.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/utils/load_smartpredictor.py` & `shapash-2.3.4/shapash/utils/load_smartpredictor.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/utils/model.py` & `shapash-2.3.4/shapash/utils/model.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/utils/model_synoptic.py` & `shapash-2.3.4/shapash/utils/model_synoptic.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/utils/threading.py` & `shapash-2.3.4/shapash/utils/threading.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/utils/transform.py` & `shapash-2.3.4/shapash/utils/transform.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/utils/utils.py` & `shapash-2.3.4/shapash/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/webapp/assets/favicon.ico` & `shapash-2.3.4/shapash/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/webapp/assets/jquery.js` & `shapash-2.3.4/shapash/webapp/assets/jquery.js`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/webapp/assets/material-icons.css` & `shapash-2.3.4/shapash/webapp/assets/material-icons.css`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/webapp/assets/reload.png` & `shapash-2.3.4/shapash/webapp/assets/reload.png`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/webapp/assets/settings.png` & `shapash-2.3.4/shapash/webapp/assets/settings.png`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/webapp/assets/shapash-fond-fonce.png` & `shapash-2.3.4/shapash/webapp/assets/shapash-fond-fonce.png`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/webapp/assets/style.css` & `shapash-2.3.4/shapash/webapp/assets/style.css`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/webapp/smart_app.py` & `shapash-2.3.4/shapash/webapp/smart_app.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/webapp/utils/MyGraph.py` & `shapash-2.3.4/shapash/webapp/utils/MyGraph.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/webapp/utils/explanations.py` & `shapash-2.3.4/shapash/webapp/utils/explanations.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/webapp/utils/utils.py` & `shapash-2.3.4/shapash/webapp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/webapp/webapp_launch.py` & `shapash-2.3.4/shapash/webapp/webapp_launch.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash/webapp/webapp_launch_DVF.py` & `shapash-2.3.4/shapash/webapp/webapp_launch_DVF.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash.egg-info/PKG-INFO` & `shapash-2.3.4/shapash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapash
-Version: 2.3.3
+Version: 2.3.4
 Summary: Shapash is a Python library which aims to make machine learning interpretable and understandable by everyone.
 Home-page: https://github.com/MAIF/shapash
 Author: Yann Golhen, Sebastien Bidault, Yann Lagre, Maxime Gendre
 Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0
 Keywords: shapash
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shapash Version: 2.3.3 Summary: Shapash is a Python
+Metadata-Version: 2.1 Name: shapash Version: 2.3.4 Summary: Shapash is a Python
 library which aims to make machine learning interpretable and understandable by
 everyone. Home-page: https://github.com/MAIF/shapash Author: Yann Golhen,
 Sebastien Bidault, Yann Lagre, Maxime Gendre Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0 Keywords: shapash Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
```

### Comparing `shapash-2.3.3/shapash.egg-info/SOURCES.txt` & `shapash-2.3.4/shapash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shapash-2.3.3/shapash.egg-info/requires.txt` & `shapash-2.3.4/shapash.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 plotly>=5.0.0
 matplotlib>=3.2.0
-numpy>1.18.0
+numpy<1.24.0,>1.18.0
 pandas<2.0.0,>1.0.2
 shap>=0.38.1
 Flask<2.3.0
 dash>=2.3.1
 dash-bootstrap-components>=1.1.0
 dash-core-components>=2.0.0
 dash-daq>=0.5.0
```

