# Comparing `tmp/brainlit-0.3.3.tar.gz` & `tmp/brainlit-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainlit-0.3.3.tar", last modified: Wed Mar  2 15:20:25 2022, max compression
+gzip compressed data, was "brainlit-0.3.4.tar", last modified: Tue May  9 16:47:48 2023, max compression
```

## Comparing `brainlit-0.3.3.tar` & `brainlit-0.3.4.tar`

### file list

```diff
@@ -1,75 +1,63 @@
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.145072 brainlit-0.3.3/
--rw-r--r--   0 thomasathey   (501) staff       (20)    11358 2020-10-26 19:40:08.000000 brainlit-0.3.3/LICENSE
--rw-r--r--   0 thomasathey   (501) staff       (20)     3411 2022-03-02 15:20:25.144653 brainlit-0.3.3/PKG-INFO
--rw-r--r--   0 thomasathey   (501) staff       (20)     2597 2022-01-31 22:42:20.000000 brainlit-0.3.3/README.md
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.115567 brainlit-0.3.3/brainlit/
--rw-r--r--   0 thomasathey   (501) staff       (20)      413 2022-03-02 15:19:55.000000 brainlit-0.3.3/brainlit/__init__.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.117818 brainlit-0.3.3/brainlit/algorithms/
--rw-r--r--   0 thomasathey   (501) staff       (20)      394 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/algorithms/__init__.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.118886 brainlit-0.3.3/brainlit/algorithms/connect_fragments/
--rw-r--r--   0 thomasathey   (501) staff       (20)      231 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/algorithms/connect_fragments/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     2173 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/algorithms/connect_fragments/trace_evaluation.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    16212 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/algorithms/connect_fragments/viterbrain.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.119692 brainlit-0.3.3/brainlit/algorithms/detect_somas/
--rw-r--r--   0 thomasathey   (501) staff       (20)       54 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/algorithms/detect_somas/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     5191 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/algorithms/detect_somas/detect.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.122591 brainlit-0.3.3/brainlit/algorithms/generate_fragments/
--rwxr-xr-x   0 thomasathey   (501) staff       (20)      261 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/algorithms/generate_fragments/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    12490 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/algorithms/generate_fragments/adaptive_thresh.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     4931 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/algorithms/generate_fragments/pcurve.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    25030 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/algorithms/generate_fragments/state_generation.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     6017 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/algorithms/generate_fragments/tube_seg.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.124532 brainlit-0.3.3/brainlit/algorithms/trace_analysis/
--rwxr-xr-x   0 thomasathey   (501) staff       (20)      121 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/algorithms/trace_analysis/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    12887 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/algorithms/trace_analysis/fit_spline.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    11686 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/algorithms/trace_analysis/spline_fxns.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.126287 brainlit-0.3.3/brainlit/feature_extraction/
--rw-r--r--   0 thomasathey   (501) staff       (20)       55 2020-10-26 19:40:08.000000 brainlit-0.3.3/brainlit/feature_extraction/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    12243 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/feature_extraction/base.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     3332 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/feature_extraction/neighborhood.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.128213 brainlit-0.3.3/brainlit/preprocessing/
--rw-r--r--   0 thomasathey   (501) staff       (20)       99 2020-10-26 19:40:08.000000 brainlit-0.3.3/brainlit/preprocessing/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    21884 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/preprocessing/image_process.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     8177 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/preprocessing/preprocess.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.132004 brainlit-0.3.3/brainlit/registration/
--rw-r--r--   0 thomasathey   (501) staff       (20)      586 2020-10-26 19:40:08.000000 brainlit-0.3.3/brainlit/registration/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     1168 2020-10-26 19:40:08.000000 brainlit-0.3.3/brainlit/registration/__version__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     5181 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/registration/file_io.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     7847 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/registration/imageData.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.135795 brainlit-0.3.3/brainlit/registration/lddmm/
--rw-r--r--   0 thomasathey   (501) staff       (20)      121 2020-10-26 19:40:08.000000 brainlit-0.3.3/brainlit/registration/lddmm/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    89713 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/registration/lddmm/_lddmm.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    16639 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/registration/lddmm/_lddmm_utilities.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    28518 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/registration/lddmm/_test_lddmm.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    25183 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/registration/lddmm/_test_lddmm_utilities.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.139427 brainlit-0.3.3/brainlit/registration/preprocessing/
--rw-r--r--   0 thomasathey   (501) staff       (20)     6466 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/registration/preprocessing/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     8058 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/registration/preprocessing/bias_and_artifact_correction.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     6694 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/registration/preprocessing/initialization.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     2364 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/registration/preprocessing/normalization.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     5615 2020-10-26 19:40:08.000000 brainlit-0.3.3/brainlit/registration/preprocessing/resampling.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.140752 brainlit-0.3.3/brainlit/registration/presets/
--rw-r--r--   0 thomasathey   (501) staff       (20)      238 2020-10-26 19:40:08.000000 brainlit-0.3.3/brainlit/registration/presets/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     1343 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/registration/presets/batch_preprocessing.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     2375 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/registration/presets/registration_parameters.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    21820 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/registration/transform.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     8994 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/registration/utilities.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    13243 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/registration/visualization.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.143303 brainlit-0.3.3/brainlit/utils/
--rwxr-xr-x   0 thomasathey   (501) staff       (20)    39813 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/utils/Neuron_trace.py
--rw-r--r--   0 thomasathey   (501) staff       (20)      164 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/utils/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     3021 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/utils/benchmarking_params.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    15719 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/utils/session.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    20114 2022-03-02 14:37:16.000000 brainlit-0.3.3/brainlit/utils/upload.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     2499 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/utils/util.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.144122 brainlit-0.3.3/brainlit/viz/
--rw-r--r--   0 thomasathey   (501) staff       (20)       37 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/viz/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     7405 2022-01-31 22:42:20.000000 brainlit-0.3.3/brainlit/viz/swc2voxel.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2022-03-02 15:20:25.117377 brainlit-0.3.3/brainlit.egg-info/
--rw-r--r--   0 thomasathey   (501) staff       (20)     3411 2022-03-02 15:20:24.000000 brainlit-0.3.3/brainlit.egg-info/PKG-INFO
--rw-r--r--   0 thomasathey   (501) staff       (20)     2248 2022-03-02 15:20:24.000000 brainlit-0.3.3/brainlit.egg-info/SOURCES.txt
--rw-r--r--   0 thomasathey   (501) staff       (20)        1 2022-03-02 15:20:24.000000 brainlit-0.3.3/brainlit.egg-info/dependency_links.txt
--rw-r--r--   0 thomasathey   (501) staff       (20)      253 2022-03-02 15:20:24.000000 brainlit-0.3.3/brainlit.egg-info/requires.txt
--rw-r--r--   0 thomasathey   (501) staff       (20)        9 2022-03-02 15:20:24.000000 brainlit-0.3.3/brainlit.egg-info/top_level.txt
--rw-r--r--   0 thomasathey   (501) staff       (20)       38 2022-03-02 15:20:25.145205 brainlit-0.3.3/setup.cfg
--rw-r--r--   0 thomasathey   (501) staff       (20)     2094 2022-01-31 22:42:21.000000 brainlit-0.3.3/setup.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.905185 brainlit-0.3.4/
+-rw-r--r--   0 thomasathey   (501) staff       (20)    11358 2020-10-26 19:40:08.000000 brainlit-0.3.4/LICENSE
+-rw-r--r--   0 thomasathey   (501) staff       (20)     3056 2023-05-09 16:47:48.904580 brainlit-0.3.4/PKG-INFO
+-rw-r--r--   0 thomasathey   (501) staff       (20)     2262 2023-05-09 16:45:44.000000 brainlit-0.3.4/README.md
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.878351 brainlit-0.3.4/brainlit/
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.883953 brainlit-0.3.4/brainlit/BrainLine/
+-rw-r--r--   0 thomasathey   (501) staff       (20)      346 2023-04-26 12:32:15.000000 brainlit-0.3.4/brainlit/BrainLine/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    44207 2023-05-09 16:45:47.000000 brainlit-0.3.4/brainlit/BrainLine/analyze_results.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    28417 2023-05-09 16:45:44.000000 brainlit-0.3.4/brainlit/BrainLine/apply_ilastik.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)      394 2023-04-12 15:04:36.000000 brainlit-0.3.4/brainlit/BrainLine/imports.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     3778 2023-04-12 15:04:36.000000 brainlit-0.3.4/brainlit/BrainLine/parse_ara.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    10975 2023-05-02 20:53:23.000000 brainlit-0.3.4/brainlit/BrainLine/util.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)      385 2023-05-09 16:46:16.000000 brainlit-0.3.4/brainlit/__init__.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.884356 brainlit-0.3.4/brainlit/algorithms/
+-rw-r--r--   0 thomasathey   (501) staff       (20)      394 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/algorithms/__init__.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.885889 brainlit-0.3.4/brainlit/algorithms/connect_fragments/
+-rw-r--r--   0 thomasathey   (501) staff       (20)      231 2022-03-16 13:30:15.000000 brainlit-0.3.4/brainlit/algorithms/connect_fragments/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     2239 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/algorithms/connect_fragments/trace_evaluation.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    18206 2023-05-09 16:45:44.000000 brainlit-0.3.4/brainlit/algorithms/connect_fragments/viterbrain.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.887230 brainlit-0.3.4/brainlit/algorithms/detect_somas/
+-rw-r--r--   0 thomasathey   (501) staff       (20)       54 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/algorithms/detect_somas/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     5191 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/algorithms/detect_somas/detect.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.888954 brainlit-0.3.4/brainlit/algorithms/generate_fragments/
+-rwxr-xr-x   0 thomasathey   (501) staff       (20)      132 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/algorithms/generate_fragments/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    31716 2023-05-09 16:45:44.000000 brainlit-0.3.4/brainlit/algorithms/generate_fragments/state_generation.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     6158 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/algorithms/generate_fragments/tube_seg.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.890488 brainlit-0.3.4/brainlit/algorithms/trace_analysis/
+-rwxr-xr-x   0 thomasathey   (501) staff       (20)      121 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/algorithms/trace_analysis/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    17453 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/algorithms/trace_analysis/fit_spline.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    11686 2022-03-16 13:30:15.000000 brainlit-0.3.4/brainlit/algorithms/trace_analysis/spline_fxns.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.892177 brainlit-0.3.4/brainlit/feature_extraction/
+-rw-r--r--   0 thomasathey   (501) staff       (20)       55 2020-10-26 19:40:08.000000 brainlit-0.3.4/brainlit/feature_extraction/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    12440 2023-04-03 18:41:18.000000 brainlit-0.3.4/brainlit/feature_extraction/base.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     3332 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/feature_extraction/neighborhood.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.893273 brainlit-0.3.4/brainlit/map_neurons/
+-rw-r--r--   0 thomasathey   (501) staff       (20)       92 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/map_neurons/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    19224 2023-05-05 16:56:46.000000 brainlit-0.3.4/brainlit/map_neurons/map_neurons.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.894038 brainlit-0.3.4/brainlit/napari_viterbrain/
+-rw-r--r--   0 thomasathey   (501) staff       (20)     2049 2023-04-03 21:17:17.000000 brainlit-0.3.4/brainlit/napari_viterbrain/viterbrain_plugin.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.896267 brainlit-0.3.4/brainlit/preprocessing/
+-rw-r--r--   0 thomasathey   (501) staff       (20)       99 2020-10-26 19:40:08.000000 brainlit-0.3.4/brainlit/preprocessing/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    22539 2023-04-07 13:39:56.000000 brainlit-0.3.4/brainlit/preprocessing/image_process.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     8614 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/preprocessing/preprocess.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.902051 brainlit-0.3.4/brainlit/utils/
+-rwxr-xr-x   0 thomasathey   (501) staff       (20)    42070 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/utils/Neuron_trace.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)      232 2023-03-01 16:17:04.000000 brainlit-0.3.4/brainlit/utils/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     3021 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/utils/benchmarking_params.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    15886 2023-05-09 16:45:44.000000 brainlit-0.3.4/brainlit/utils/session.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    20173 2023-04-03 21:17:17.000000 brainlit-0.3.4/brainlit/utils/upload.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     2514 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/utils/util.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     7017 2023-05-09 16:45:44.000000 brainlit-0.3.4/brainlit/utils/write.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.903686 brainlit-0.3.4/brainlit/viz/
+-rw-r--r--   0 thomasathey   (501) staff       (20)       37 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/viz/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     7752 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/viz/swc2voxel.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.881456 brainlit-0.3.4/brainlit.egg-info/
+-rw-r--r--   0 thomasathey   (501) staff       (20)     3056 2023-05-09 16:47:48.000000 brainlit-0.3.4/brainlit.egg-info/PKG-INFO
+-rw-r--r--   0 thomasathey   (501) staff       (20)     1616 2023-05-09 16:47:48.000000 brainlit-0.3.4/brainlit.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasathey   (501) staff       (20)        1 2023-05-09 16:47:48.000000 brainlit-0.3.4/brainlit.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasathey   (501) staff       (20)       68 2023-05-09 16:47:48.000000 brainlit-0.3.4/brainlit.egg-info/entry_points.txt
+-rw-r--r--   0 thomasathey   (501) staff       (20)      325 2023-05-09 16:47:48.000000 brainlit-0.3.4/brainlit.egg-info/requires.txt
+-rw-r--r--   0 thomasathey   (501) staff       (20)        9 2023-05-09 16:47:48.000000 brainlit-0.3.4/brainlit.egg-info/top_level.txt
+-rw-r--r--   0 thomasathey   (501) staff       (20)       38 2023-05-09 16:47:48.905373 brainlit-0.3.4/setup.cfg
+-rw-r--r--   0 thomasathey   (501) staff       (20)     2699 2023-05-02 20:53:23.000000 brainlit-0.3.4/setup.py
```

### Comparing `brainlit-0.3.3/LICENSE` & `brainlit-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.3/PKG-INFO` & `brainlit-0.3.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 Metadata-Version: 2.1
 Name: brainlit
-Version: 0.3.3
+Version: 0.3.4
 Summary: Code to process and analyze brainlit data
 Home-page: https://github.com/neurodata/brainlit
 Author: ('Thomas Athey, Bijan Varjivand, Ryan Lu, Matt Figdore, Alex Fiallos, Stanley Wang, Victor Wang',)
 Author-email: tathey1@jhu.edu
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Brainlit
 [![DOI](https://zenodo.org/badge/237507496.svg)](https://zenodo.org/badge/latestdoi/237507496)
 [![Python](https://img.shields.io/badge/python-3.7-blue.svg)]()
+![Tests](https://img.shields.io/github/actions/workflow/status/neurodata/brainlit/python.yml)
 [![CircleCI](https://circleci.com/gh/neurodata/brainlit/tree/develop.svg?style=svg)](https://circleci.com/gh/neurodata/brainlit/tree/develop)
+[![Netlify Status](https://api.netlify.com/api/v1/badges/daad6ab0-1d47-4685-b6ab-ecc487a01ba7/deploy-status)](https://brainlit.netlify.app/)
 [![PyPI version](https://badge.fury.io/py/brainlit.svg)](https://badge.fury.io/py/brainlit)
 [![Downloads](https://img.shields.io/pypi/dw/brainlit)](https://img.shields.io/pypi/dw/brainlit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/neurodata/brainlit/branch/develop/graph/badge.svg)](https://codecov.io/gh/neurodata/brainlit)
-![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/bvarjavand/brainlit)
-![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/bvarjavand/brainlit)
+![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/neurodata/brainlit)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)  
 
 ## Summary
-This repository is a container of methods that Neurodata uses to expose their open-source code while it is in the process of being merged with larger scientific libraries such as scipy, scikit-image, or scikit-learn. Additionally, methods for computational neuroscience on brains too specific for a general scientific library can be found here, such as image registration software tuned specifically for large brain volumes. Documentation can be found by clicking on the Netlify badge below:
-
-[![Netlify Status](https://api.netlify.com/api/v1/badges/daad6ab0-1d47-4685-b6ab-ecc487a01ba7/deploy-status)](https://brainlit.netlify.app/)
-
-Brainlit is a product of the [neurodata lab](https://neurodata.io/). It is actively maintained by Thomas Athey (@tathey1) and Bijan Varjavand (@bvarjavand), and is regularly used and contributed to by students in the [Neuro Data Design](https://neurodatadesign.io/) course. We strive to follow the same [code of conduct](https://opensource.microsoft.com/codeofconduct/) that applies to the Microsoft open source community.
-
-## Contributing
-We welcome all contributors, and encourage them to follow our contribution guidelines gound in [CONTRIBUTING.md](https://github.com/neurodata/brainlit/blob/master/CONTRIBUTING.md). Issues with the "good first issue" tag are meant for contributors that are either new to open source coding, or new to the package. Additionally, users are encouraged to use issues not only to discuss code-related problems, but for more general discussions about the package.
+This repository is used for various tasks in processing, and analyzing light microscopy images of brains for the purpose of studing neuron morphology. Documentation can be found [here](http://brainlit.neurodata.io/).
 
+Brainlit is a product of the [neurodata lab](https://neurodata.io/) and the [Neuro Data Design](https://neurodatadesign.io/) course. It is actively maintained by Thomas Athey (@tathey1). We strive to follow the same [code of conduct](https://opensource.microsoft.com/codeofconduct/) that applies to the Microsoft open source community.
 
+## Contributing and Questions
+We welcome all contributors, and encourage them to follow our contribution guidelines gound in [CONTRIBUTING.md](https://github.com/neurodata/brainlit/blob/master/CONTRIBUTING.md). Issues with the "good first issue" tag are meant for contributors that are either new to open source coding, or new to the package. Additionally, users are encouraged to use issues not only to discuss code-related problems, but for more general discussions or questions about the package.
```

### Comparing `brainlit-0.3.3/README.md` & `brainlit-0.3.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Brainlit
 [![DOI](https://zenodo.org/badge/237507496.svg)](https://zenodo.org/badge/latestdoi/237507496)
 [![Python](https://img.shields.io/badge/python-3.7-blue.svg)]()
+![Tests](https://img.shields.io/github/actions/workflow/status/neurodata/brainlit/python.yml)
 [![CircleCI](https://circleci.com/gh/neurodata/brainlit/tree/develop.svg?style=svg)](https://circleci.com/gh/neurodata/brainlit/tree/develop)
+[![Netlify Status](https://api.netlify.com/api/v1/badges/daad6ab0-1d47-4685-b6ab-ecc487a01ba7/deploy-status)](https://brainlit.netlify.app/)
 [![PyPI version](https://badge.fury.io/py/brainlit.svg)](https://badge.fury.io/py/brainlit)
 [![Downloads](https://img.shields.io/pypi/dw/brainlit)](https://img.shields.io/pypi/dw/brainlit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/neurodata/brainlit/branch/develop/graph/badge.svg)](https://codecov.io/gh/neurodata/brainlit)
-![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/bvarjavand/brainlit)
-![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/bvarjavand/brainlit)
+![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/neurodata/brainlit)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)  
 
 ## Summary
-This repository is a container of methods that Neurodata uses to expose their open-source code while it is in the process of being merged with larger scientific libraries such as scipy, scikit-image, or scikit-learn. Additionally, methods for computational neuroscience on brains too specific for a general scientific library can be found here, such as image registration software tuned specifically for large brain volumes. Documentation can be found by clicking on the Netlify badge below:
-
-[![Netlify Status](https://api.netlify.com/api/v1/badges/daad6ab0-1d47-4685-b6ab-ecc487a01ba7/deploy-status)](https://brainlit.netlify.app/)
+This repository is used for various tasks in processing, and analyzing light microscopy images of brains for the purpose of studing neuron morphology. Documentation can be found [here](http://brainlit.neurodata.io/).
 
-Brainlit is a product of the [neurodata lab](https://neurodata.io/). It is actively maintained by Thomas Athey (@tathey1) and Bijan Varjavand (@bvarjavand), and is regularly used and contributed to by students in the [Neuro Data Design](https://neurodatadesign.io/) course. We strive to follow the same [code of conduct](https://opensource.microsoft.com/codeofconduct/) that applies to the Microsoft open source community.
+Brainlit is a product of the [neurodata lab](https://neurodata.io/) and the [Neuro Data Design](https://neurodatadesign.io/) course. It is actively maintained by Thomas Athey (@tathey1). We strive to follow the same [code of conduct](https://opensource.microsoft.com/codeofconduct/) that applies to the Microsoft open source community.
 
-## Contributing
-We welcome all contributors, and encourage them to follow our contribution guidelines gound in [CONTRIBUTING.md](https://github.com/neurodata/brainlit/blob/master/CONTRIBUTING.md). Issues with the "good first issue" tag are meant for contributors that are either new to open source coding, or new to the package. Additionally, users are encouraged to use issues not only to discuss code-related problems, but for more general discussions about the package.
+## Contributing and Questions
+We welcome all contributors, and encourage them to follow our contribution guidelines gound in [CONTRIBUTING.md](https://github.com/neurodata/brainlit/blob/master/CONTRIBUTING.md). Issues with the "good first issue" tag are meant for contributors that are either new to open source coding, or new to the package. Additionally, users are encouraged to use issues not only to discuss code-related problems, but for more general discussions or questions about the package.
```

### Comparing `brainlit-0.3.3/brainlit/algorithms/connect_fragments/trace_evaluation.py` & `brainlit-0.3.4/brainlit/algorithms/connect_fragments/trace_evaluation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from sklearn.metrics import pairwise_distances_argmin_min
 
 
-def resample(path, spacing=1):
+def resample(path: np.array, spacing: int = 1) -> np.array:
     """Resample a path (linearly) according to maximum distance between points
 
     Args:
         path (np.array): points of path, shaped as number points x number of features.
         spacing (int, optional): maximum distance between points. Defaults to 1.
 
     Returns:
@@ -27,15 +27,15 @@
                 mid[i, :] = pt1 + (t / dist) * (pt2 - pt1)
             new_path.append(mid)
     new_path.append(pt2)
     new_path = np.concatenate(new_path)
     return new_path
 
 
-def sd(pts1, pts2, substantial=False):
+def sd(pts1: np.array, pts2: np.array, substantial: bool = False) -> float:
     """Compute spatial distance between two paths according to Peng et. al. 2010.
 
     Args:
         pts1 (np.array): points of first path, shaped as number points x number of features.
         pts2 (np.array): points of second path, shaped as number points x number of features.
         substantial (bool, optional): whether to compute substantial spatial distance which ignores all points that have a closest point within 2 voxels. Defaults to False.
         verbose (bool, optional): [description]. Defaults to False.
```

### Comparing `brainlit-0.3.3/brainlit/algorithms/connect_fragments/viterbrain.py` & `brainlit-0.3.4/brainlit/algorithms/connect_fragments/viterbrain.py`

 * *Files 5% similar despite different names*

```diff
@@ -254,15 +254,15 @@
             frag_soma_func (function): function that computes transition cost between fragments
         """
         parallel = self.parallel
         G = self.nxGraph
 
         state_sets = np.array_split(np.arange(self.num_states), parallel)
 
-        results_tuple = Parallel(n_jobs=parallel)(
+        results_tuple = Parallel(n_jobs=parallel, backend="threading")(
             delayed(self._compute_out_costs_dist)(
                 states, frag_frag_func, frag_soma_func
             )
             for states in state_sets
         )
 
         results = [item for result in results_tuple for item in result]
@@ -341,15 +341,15 @@
                     G.nodes[state1]["type"] == "fragment"
                     and G.nodes[state2]["type"] == "fragment"
                 ):
                     line_int_cost = self._line_int(
                         G.nodes[state1]["point2"], G.nodes[state2]["point1"]
                     )
                     int_cost = line_int_cost + G.nodes[state2]["image_cost"]
-                    results.append((state1, state2, line_int_cost))
+                    results.append((state1, state2, int_cost))
                 elif (
                     G.nodes[state1]["type"] == "fragment"
                     and G.nodes[state2]["type"] == "soma"
                 ):
                     line_int_cost = self._line_int(
                         G.nodes[state1]["point2"], G.nodes[state1]["soma_pt"]
                     )
@@ -362,15 +362,15 @@
     def compute_all_costs_int(self) -> None:
         """Splits up transition computation tasks then assembles them into networkx graph"""
         parallel = self.parallel
         G = self.nxGraph
 
         state_sets = np.array_split(np.arange(self.num_states), parallel)
 
-        results_tuple = Parallel(n_jobs=parallel)(
+        results_tuple = Parallel(n_jobs=parallel, backend="threading")(
             delayed(self._compute_out_int_costs)(states) for states in state_sets
         )
 
         results = [item for result in results_tuple for item in result]
         for result in results:
             state1, state2, int_cost = result
             if int_cost != np.inf:
@@ -395,21 +395,19 @@
         """
         fragments = zarr.open(self.fragment_path, mode="r")
 
         # Compute labels of coordinates
         labels = []
         radius = 20
         for coord in [coord1, coord2]:
-            local_labels = fragments[
-                np.amax([coord[0] - radius, 0]) : coord[0] + radius,
-                np.amax([coord[1] - radius, 0]) : coord[1] + radius,
-                np.amax([coord[2] - radius, 0]) : coord[2] + radius,
-            ]
+            local_labels, new_coord = get_valid_bbox(fragments, coord, radius=20)
             label = image_process.label_points(
-                local_labels, [[radius, radius, radius]], res=self.resolution
+                local_labels,
+                [new_coord],
+                res=self.resolution,
             )[1][0]
             labels.append(label)
 
         # find shortest path for all state combinations
         states1 = self.comp_to_states[labels[0]]
         states2 = self.comp_to_states[labels[1]]
         min_cost = -1
@@ -424,22 +422,81 @@
                     continue
                 if cost < min_cost or min_cost == -1:
                     min_cost = cost
                     states = nx.shortest_path(
                         self.nxGraph, state1, state2, weight="total_cost"
                     )
 
+        if min_cost == -1:
+            raise nx.NetworkXNoPath(f"No path found between {coord1} and {coord2}")
+
         # create coordinate list
         coords = [coord1]
-        coords.append(self.nxGraph.nodes[states[0]]["point2"])
+        coords.append(list(self.nxGraph.nodes[states[0]]["point2"]))
         for i, state in enumerate(states[1:]):
             if self.nxGraph.nodes[state]["type"] == "fragment":
-                coords.append(self.nxGraph.nodes[state]["point1"])
-                coords.append(self.nxGraph.nodes[state]["point2"])
+                coords.append(list(self.nxGraph.nodes[state]["point1"]))
+                coords.append(list(self.nxGraph.nodes[state]["point2"]))
             elif self.nxGraph.nodes[state]["type"] == "soma":
-                coords.append(self.nxGraph.nodes[states[i]]["soma_pt"])
+                coords.append(list(self.nxGraph.nodes[states[i]]["soma_pt"]))
                 if i != len(states) - 2:
                     raise ValueError("Soma state is not last state")
 
         coords.append(coord2)
 
         return coords
+
+
+def explain_viterbrain(vb, c1, c2, frag_seq):
+    # assume c1,c2 fall on a fragment
+    path_coords = vb.shortest_path(c1, c2)
+    comp_to_states = vb.comp_to_states
+    z_frags = zarr.open(vb.fragment_path)
+
+    states1 = comp_to_states[z_frags[c1[0], c1[1], c1[2]]]
+    states2 = comp_to_states[z_frags[c2[0], c2[1], c2[2]]]
+
+    min_cost = -1
+    for state1 in states1:
+        for state2 in states2:
+            try:
+                cost = nx.shortest_path_length(
+                    vb.nxGraph, state1, state2, weight="total_cost"
+                )
+            except nx.NetworkXNoPath:
+                continue
+            if cost < min_cost or min_cost == -1:
+                min_cost = cost
+                states = nx.shortest_path(
+                    vb.nxGraph, state1, state2, weight="total_cost"
+                )
+
+    print(f"{len(states)} states")
+    print(f"{len(path_coords)} coordinates")
+    print(f"0: {path_coords[0]} f{z_frags[c1[0],c1[1],c1[2]]} ")
+
+    coord_idx = 1
+    for i, state in enumerate(states):
+        if i > 0:
+            e = vb.nxGraph.edges(states[i - 1], state)
+            print(f"Transition: {states[i-1]}->{state}: {e}")
+        c = path_coords[coord_idx]
+        print(f"{coord_idx}: {c} f{z_frags[c[0],c[1],c[2]]} s{state}")
+        coord_idx += 1
+        c = path_coords[coord_idx]
+        print(f"{coord_idx}: {c} f{z_frags[c[0],c[1],c[2]]} s{state}")
+
+    coord_idx += 1
+    c = path_coords[coord_idx]
+    print(f"{coord_idx}: {c} f{z_frags[c[0],c[1],c[2]]} s{state}")
+
+
+def get_valid_bbox(array, coord, radius):
+    x1 = np.amax([coord[0] - radius, 0])
+    y1 = np.amax([coord[1] - radius, 0])
+    z1 = np.amax([coord[2] - radius, 0])
+    x2 = np.amin([coord[0] + radius, array.shape[0]])
+    y2 = np.amin([coord[1] + radius, array.shape[1]])
+    z2 = np.amin([coord[2] + radius, array.shape[2]])
+
+    subvol = np.array(np.squeeze(array[x1:x2, y1:y2, z1:z2]))
+    return subvol, [coord[0] - x1, coord[1] - y1, coord[2] - z1]
```

### Comparing `brainlit-0.3.3/brainlit/algorithms/detect_somas/detect.py` & `brainlit-0.3.4/brainlit/algorithms/detect_somas/detect.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.3/brainlit/algorithms/generate_fragments/adaptive_thresh.py` & `brainlit-0.3.4/brainlit/feature_extraction/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,445 +1,332 @@
-# Reference: http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/Python_html/300_Segmentation_Overview.html
-
-import SimpleITK as sitk
-from sklearn.mixture import GaussianMixture
+from abc import abstractmethod
+from xmlrpc.client import boolean
+from sklearn.base import BaseEstimator
+from brainlit.utils.session import NeuroglancerSession
+from brainlit.utils.util import *
+import warnings
 import numpy as np
-
-
-def get_seed(voxel):
-    """
-    Get a seed point for the center of a brain volume.
-
-    Parameters
-    ----------
-    voxel : tuple:
-        The seed coordinates in x y z.
-
-    Returns
-    -------
-    tuple
-        A tuple containing the (x, y, z)-coordinates of the seed.
-
-    """
-    numpy_seed = (int(voxel[0]), int(voxel[1]), int(voxel[2]))
-    sitk_seed = (int(voxel[2]), int(voxel[1]), int(voxel[0]))
-    return numpy_seed, sitk_seed
-
-
-def get_img_T1(img):
-    """
-    Converts a volume cutout to a SimpleITK image, as wel
-    as a SimpleITK image with scaled intensity values to 0-255.
-
-    Parameters
-    ----------
-    img : cloudvolume.volumecutout.VolumeCutout
-        The volume to convert to a SimpleITK image.
-
-    Returns
-    -------
-    img_T1 : SimpleITK.SimpleITK.Image
-        A SimpleITK image.
-
-    img_T1_255 : SimpleITK.SimpleITK.Image
-        A SimpleITK image with
-        intensity values between 0 and 255 inclusive.
-
-    """
-
-    img_T1 = sitk.GetImageFromArray(np.squeeze(img), isVector=False)
-    img_T1_255 = sitk.Cast(sitk.RescaleIntensity(img_T1), sitk.sitkUInt8)
-    return img_T1, img_T1_255
-
-
-def thres_from_gmm(img, random_seed=2):
-    """
-    Computes a numerical threshold for segmentation based
-    on a 2-Component Gaussian mixture model.
-
-    The threshold is the minimum value included in the Gaussian
-    mixture model-component containning the highest intensity value.
-
-    Parameters
-    ----------
-    img : cloudvolume.volumecutout.VolumeCutout
-        The image or volume to threshold.
-
-    random_seed : int
-        The random seed for the Gaussian mixture model.
-
-    Returns
-    -------
-    int
-        The threshold value.
-
-    """
-
-    _, img_T1_255 = get_img_T1(img)
-    img_array = sitk.GetArrayFromImage(img_T1_255)
-    flat_array = img_array.flatten().reshape(-1, 1)
-    gmm = GaussianMixture(n_components=2, random_state=random_seed)
-    y = gmm.fit_predict(flat_array)
-    mask = y.astype(bool)
-    a = flat_array[mask]
-    b = flat_array[~mask]
-    if a.max() > b.max():
-        thres = a.min()
-    else:
-        thres = b.min()
-
-    return int(thres)
-
-
-def fast_marching_seg(img, seed, stopping_value=150, sigma=0.5):
-    """
-    Computes a fast-marching segmentation.
-
-    Parameters
-    ----------
-    img : cloudvolume.volumecutout.VolumeCutout
-        The volume to segment.
-
-    seed : tuple
-        The seed containing a coordinate within a known segment.
-
-    stopping_value : float
-        The algorithm stops when the value of the smallest trial
-        point is greater than this stopping value.
-
-    sigma : float
-        Sigma used in computing the feature image.
-
-    Returns
-    -------
-    labels : numpy.ndarray
-        An array consisting of the pixelwise segmentation.
-
-    """
-
-    img_T1, img_T1_255 = get_img_T1(img)
-    feature_img = sitk.GradientMagnitudeRecursiveGaussian(img_T1_255, sigma=sigma)
-    speed_img = sitk.BoundedReciprocal(feature_img)
-    fm_filter = sitk.FastMarchingBaseImageFilter()
-    fm_filter.SetTrialPoints([seed])
-    fm_filter.SetStoppingValue(stopping_value)
-    fm_img = fm_filter.Execute(speed_img)
-    fm_img = sitk.Cast(sitk.RescaleIntensity(fm_img), sitk.sitkUInt8)
-    labels = sitk.GetArrayFromImage(fm_img)
-    labels = (~labels.astype(bool)).astype(int)
-    return labels
-
-
-def level_set_seg(
-    img,
-    seed,
-    lower_threshold=None,
-    upper_threshold=None,
-    factor=2,
-    max_rms_error=0.02,
-    num_iter=1000,
-    curvature_scaling=0.5,
-    propagation_scaling=1,
-):
-    """
-    Computes a level-set segmentation.
-
-    When root mean squared change in the level set function for an iteration is below
-    the threshold, or the maximum number of iteration have elapsed,
-    the algorithm is said to have converged.
-
-    Parameters
-    ----------
-    img : cloudvolume.volumecutout.VolumeCutout
-        The volume to segment.
-
-    seed : tuple
-        The seed containing a coordinate within a known segment.
-
-    lower_threshold : float
-        The lower threshold for segmentation. Set based on image statistics if None.
-
-    upper_threshold : float
-        The upper threshold for segmentation. Set based on image statistics if None.
-
-    factor : float
-        The scaling factor on the standard deviation used in computing thresholds
-        from image statistics.
-
-    max_rms_error : float
-        Root mean squared convergence criterion threshold.
-
-    num_iter : int
-        Maximum number of iterations.
-
-    curvature_scaling : float
-        Curvature scaling for the segmentation.
-
-    propagation_scaling : float
-        Propagation scaling for the segmentation.
-
-    Returns
-    -------
-    labels : numpy.ndarray
-        An array consisting of the pixelwise segmentation.
-
-    """
-
-    img_T1, img_T1_255 = get_img_T1(img)
-
-    seg = sitk.Image(img_T1_255.GetSize(), sitk.sitkUInt8)
-    seg.CopyInformation(img_T1_255)
-    seg[seed] = 1
-    seg = sitk.BinaryDilate(seg, [1] * seg.GetDimension())
-
-    stats = sitk.LabelStatisticsImageFilter()
-    stats.Execute(img_T1_255, seg)
-
-    if lower_threshold == None:
-        lower_threshold = stats.GetMean(1) - factor * stats.GetSigma(1)
-    if upper_threshold == None:
-        upper_threshold = stats.GetMean(1) + factor * stats.GetSigma(1)
-
-    init_ls = sitk.SignedMaurerDistanceMap(
-        seg, insideIsPositive=True, useImageSpacing=True
-    )
-
-    lsFilter = sitk.ThresholdSegmentationLevelSetImageFilter()
-    lsFilter.SetLowerThreshold(lower_threshold)
-    lsFilter.SetUpperThreshold(upper_threshold)
-    lsFilter.SetMaximumRMSError(max_rms_error)
-    lsFilter.SetNumberOfIterations(num_iter)
-    lsFilter.SetCurvatureScaling(curvature_scaling)
-    lsFilter.SetPropagationScaling(propagation_scaling)
-    lsFilter.ReverseExpansionDirectionOn()
-    ls = lsFilter.Execute(init_ls, sitk.Cast(img_T1_255, sitk.sitkFloat32))
-
-    labels = sitk.GetArrayFromImage(ls > 0)
-    return labels
-
-
-def connected_threshold(img, seed, lower_threshold=None, upper_threshold=255):
-    """
-    Compute a threshold-based segmentation via connected region growing.
-
-    Labelled pixels are connected to a seed and lie within a range of values.
-
-    Parameters
-    ----------
-    img : cloudvolume.volumecutout.VolumeCutout
-        The volume to segment.
-
-    seed : tuple
-        The seed containing a coordinate within a known segment.
-
-    lower_threshold : float
-        The lower threshold for the region growth.
-        Set by a 2-component Gaussian mixture model if None.
-
-    upper_threshold : float
-        The upper threshold for the region growth.
-
-    Returns
-    -------
-    labels : numpy.ndarray
-        An array consisting of the pixelwise segmentation.
-
-    """
-
-    img_T1, img_T1_255 = get_img_T1(img)
-    seg = sitk.Image(img_T1.GetSize(), sitk.sitkUInt8)
-    seg.CopyInformation(img_T1)
-    # seg[seed] = 1
-    for s in seed:
-        seg[s] = 1
-    seg = sitk.BinaryDilate(seg, [1] * seg.GetDimension())
-
-    if lower_threshold == None:
-        lower_threshold = thres_from_gmm(img)
-
-    seg_con = sitk.ConnectedThreshold(
-        img_T1_255, seedList=seed, lower=lower_threshold, upper=upper_threshold
-    )
-
-    vectorRadius = (1, 1, 1)
-    kernel = sitk.sitkBall
-    seg_clean = sitk.BinaryMorphologicalClosing(seg_con, vectorRadius, kernel)
-
-    labels = sitk.GetArrayFromImage(seg_clean)
-    return labels
-
-
-def confidence_connected_threshold(
-    img, seed, num_iter=1, multiplier=1, initial_neighborhood_radius=1, replace_value=1
-):
-    """
-    Compute a threshold-based segmentation via confidence-connected region growing.
-
-    The segmentation is based on pixels with intensities that are consistent
-    with pixel statistics of a seed point.
-    Pixels connected to the seed point with values within a confidence interval
-    are grouped.
-    The confidence interval is the mean plus of minus the "multiplier" times
-    the standard deviation.
-    After an initial segmentation is completed, the mean and standard deviation
-    are calculated again at each iteration using pixels in the previous segmentation.
-
-    Parameters
-    ----------
-    img : cloudvolume.volumecutout.VolumeCutout
-        The volume to segment.
-
-    seed : tuple
-        The seed containing a coordinate within a known segment.
-
-    num_iter : int
-        The number of iterations to run the algorithm.
-
-    multiplier : float
-        Multiplier for the confidence interval.
-
-    initial_neighborhood_radius : int
-        The initial neighborhood radius for computing statistics on the seed pixel.
-
-    replace_value : int
-        The value to replace thresholded pixels.
-
-    Returns
-    -------
-    labels : numpy.ndarray
-        An array consisting of the pixelwise segmentation.
-
-    """
-
-    img_T1, img_T1_255 = get_img_T1(img)
-    seg = sitk.Image(img_T1.GetSize(), sitk.sitkUInt8)
-    seg.CopyInformation(img_T1)
-    # seg[seed] = 1
-    for s in seed:
-        seg[s] = 1
-    seg = sitk.BinaryDilate(seg, [1] * seg.GetDimension())
-
-    seg_con = sitk.ConfidenceConnected(
-        img_T1_255,
-        seedList=seed,
-        numberOfIterations=num_iter,
-        multiplier=multiplier,
-        initialNeighborhoodRadius=initial_neighborhood_radius,
-        replaceValue=replace_value,
-    )
-
-    vectorRadius = (1, 1, 1)
-    kernel = sitk.sitkBall
-    seg_clean = sitk.BinaryMorphologicalClosing(seg_con, vectorRadius, kernel)
-
-    labels = sitk.GetArrayFromImage(seg_clean)
-    return labels
-
-
-def neighborhood_connected_threshold(
-    img, seed, lower_threshold=None, upper_threshold=255
-):
-    """
-    Compute a threshold-based segmentation via neighborhood-connected region growing.
-
-    Labelled pixels are connected to a seed and lie within a neighborhood.
-
-    Parameters
-    ----------
-    img : cloudvolume.volumecutout.VolumeCutout
-        The volume to segment.
-
-    seed : tuple
-        The seed containing a coordinate within a known segment.
-
-    lower_threshold : float
-        The lower threshold for the region growth.
-        Set by a 2-component Gaussian mixture model if None.
-
-    upper_threshold : float
-        The upper threshold for the region growth.
-
-    Returns
-    -------
-    labels : numpy.ndarray
-        An array consisting of the pixelwise segmentation.
-
-    """
-
-    img_T1, img_T1_255 = get_img_T1(img)
-    seg = sitk.Image(img_T1.GetSize(), sitk.sitkUInt8)
-    seg.CopyInformation(img_T1)
-    for s in seed:
-        seg[s] = 1
-    seg = sitk.BinaryDilate(seg, [1] * seg.GetDimension())
-
-    if lower_threshold == None:
-        lower_threshold = thres_from_gmm(img)
-
-    seg_con = sitk.NeighborhoodConnected(
-        img_T1_255, seedList=seed, lower=lower_threshold, upper=upper_threshold
-    )
-
-    vectorRadius = (1, 1, 1)
-    kernel = sitk.sitkBall
-    seg_clean = sitk.BinaryMorphologicalClosing(seg_con, vectorRadius, kernel)
-
-    labels = sitk.GetArrayFromImage(seg_clean)
-    return labels
-
-
-def otsu(img, seed):
-    """
-    Compute a threshold-based segmentation via Otsu's method.
-
-    Parameters
-    ----------
-    img : cloudvolume.volumecutout.VolumeCutout
-        The volume to segment.
-
-    Returns
-    -------
-    labels : numpy.ndarray
-        An array consisting of the pixelwise segmentation.
-
-    """
-
-    img_T1, img_T1_255 = get_img_T1(img)
-
-    otsu_filter = sitk.OtsuThresholdImageFilter()
-    otsu_filter.SetInsideValue(0)
-    otsu_filter.SetOutsideValue(1)
-    seg = otsu_filter.Execute(img_T1_255)
-    labels = sitk.GetArrayFromImage(seg)
-    if labels[seed] != 1:
-        labels = abs(labels - 1)
-    return labels
-
-
-def gmm_seg(img, seed, random_seed=3):
-    """
-    Compute a threshold-based segmentation via a 2-component Gaussian mixture model.
-
-    Parameters
-    ----------
-    img : cloudvolume.volumecutout.VolumeCutout
-        The volume to segment.
-
-    random_seed : int
-        The random seed for the Gaussian mixture model.
-
-    Returns
-    -------
-    labels : numpy.ndarray
-        An array consisting of the pixelwise segmentation.
-
-    """
-
-    img_T1, img_T1_255 = get_img_T1(img)
-    img_array = sitk.GetArrayFromImage(img_T1_255)
-    flat_array = img_array.flatten().reshape(-1, 1)
-    gmm = GaussianMixture(n_components=2, random_state=random_seed)
-    y = gmm.fit_predict(flat_array)
-    labels = y.reshape(img.shape).squeeze()
-    if labels[seed] != 1:
-        labels = abs(labels - 1)
-    return labels
+import pandas as pd
+import time
+from cloudvolume import CloudVolume
+import feather
+from joblib import Parallel, delayed
+from typing import Optional, List, Union, Tuple
+
+
+class BaseFeatures(BaseEstimator):
+    """Base class for generating features from precomputed volumes.
+
+    Arguments:
+        url: Precompued path either to a file URI or url URI of image data.
+        size: A size hyperparameter. For Neighborhoods, this is the radius.
+        offset: Added to the coordinates of a positive sample to generate a negative sample.
+        segment_url: Precompued path either to a file URI or url URI of segmentation data.
+
+    Attributes:
+        url: CloudVolumePrecomputedPath to image data.
+        size: A size hyperparameter. In Neighborhoods, this is the radius.
+        offset: Added to the coordinates of a positive sample to generate a negative sample.
+        download_time: Tracks time taken to download the data.
+        conversion_time: Tracks time taken to convert data to features.
+        write_time: Tracks time taken to write features to files.
+        segment_url: CloudVolumePrecomputedPath to segmentation data.
+    """
+
+    def __init__(
+        self,
+        url: str,
+        size: int,
+        offset: Tuple[int, int, int] = [15, 15, 15],
+        segment_url: Optional[str] = None,
+    ):
+        check_precomputed(url)
+        check_type(size, (int, np.integer))
+        if size < 0:
+            raise ValueError(f"Size {size} should be nonnegative.")
+        check_size(offset)
+        if segment_url is not None:
+            check_precomputed(segment_url)
+        self.url = url
+        self.size = size
+        self.offset = offset
+        self.download_time = 0
+        self.conversion_time = 0
+        self.write_time = 0
+        self.segment_url = segment_url
+
+    @abstractmethod
+    def _convert_to_features(self, img: np.ndarray) -> np.ndarray:
+        """Computes features from image data.
+
+        Arguments:
+            img: Image data.
+
+        Returns:
+            features: Feature data.
+        """
+
+    def fit(
+        self,
+        seg_ids: List[int],
+        num_verts: Optional[int] = None,
+        file_path: Optional[str] = None,
+        batch_size: int = 10000,
+        start_seg: Optional[int] = None,
+        start_vert: int = 0,
+        include_neighborhood: bool = False,
+        n_jobs: int = 1,
+    ) -> np.ndarray:
+        """Pulls image and background.
+
+        Arguments:
+            seg_ids: A list of segment indices.
+            num_verts: If not None, only runs on a set number of vertices. Defaults to None.
+            file_path: If not None, then the extracted data will be written directly
+                into a feather binary file. The file_path specifies the prefix
+                of the file. Defaults to None.
+            batch_size: Size of each batch of data to be loaded/written. Only
+                used when file_path is not none. Default 10000.
+            start_seg: Specifies which segment in the seg_ids list to start at. Default 0.
+            start_vert: Specifies which vertex of the first seg_id to start at. Default 0.
+            include_neighborhood: If extracting linear features, specifies if the general
+                neighborhood should be extracted as well. Defaults to False.
+            n_jobs: Number of cores to use. -1 to use all available cores. Defaults to 1.
+
+        Returns:
+            df: A dataframe of data containing [segment, vertex, label, f_1, f_2, ..., f_d] columns.
+        """
+        check_iterable_type(seg_ids, (int, np.integer))
+        if num_verts is not None:
+            check_type(num_verts, (int, np.integer))
+        if file_path is not None:
+            check_type(file_path, str)
+        check_type(batch_size, (int, np.integer))
+        if batch_size < 1:
+            raise ValueError(f"Batch size {batch_size} should not be negative.")
+        if start_seg is not None:
+            check_type(start_seg, (int, np.integer))
+            if start_seg < 0:
+                raise ValueError(
+                    f"Starting segment {start_seg} should not be negative."
+                )
+        check_type(start_vert, (int, np.integer))
+        if start_vert < 0:
+            raise ValueError(f"Starting vertex {start_vert} should not be negative.")
+        check_type(include_neighborhood, bool)
+        check_type(n_jobs, (int, np.integer))
+        if n_jobs < 1:
+            raise ValueError(f"Number of jobs {n_jobs} should be positive.")
+
+        voxel_dict = {}
+        counter = 0
+        batch_id = 0
+        ngl = NeuroglancerSession(self.url, url_segments=self.segment_url)
+        # ngl.cv.progress = False
+        ngl.cv_segments.progress = False
+        # if self.segment_url is None:
+        #     ngl_skel = NeuroglancerSession(self.url)
+        # else:
+        #     ngl_skel = NeuroglancerSession(self.url, self.segment_url)
+
+        if start_seg is not None:
+            seg_ids = seg_ids[seg_ids.index(start_seg) :]
+
+        if file_path is None:
+            return self._serial_processing(
+                seg_ids, ngl, num_verts, start_vert, include_neighborhood
+            )
+        else:
+            if n_jobs == 1:
+                self._serial_processing(
+                    seg_ids,
+                    ngl,
+                    num_verts,
+                    start_vert,
+                    include_neighborhood,
+                    True,
+                    batch_size,
+                    file_path,
+                )
+            else:
+                start_vertices = [0] * len(seg_ids)
+                start_vertices[0] = start_vert
+                par = Parallel(n_jobs=n_jobs)
+                par(
+                    delayed(self._parallel_processing)(
+                        seg_id,
+                        ngl,
+                        ngl_skel,
+                        num_verts,
+                        start_vertices[i],
+                        include_neighborhood,
+                        batch_size,
+                        file_path,
+                    )
+                    for i, seg_id in enumerate(seg_ids)
+                )
+
+    def _serial_processing(
+        self,
+        seg_ids: List[int],
+        ngl: NeuroglancerSession,
+        num_verts: int,
+        start_vert: int,
+        include_neighborhood: bool,
+        write: bool = False,
+        batch_size: int = None,
+        file_path: str = None,
+    ) -> None:
+        """Core code which actually extracts features."""
+        voxel_dict = {}
+        counter = 0
+        batch_id = 0
+
+        for seg_id in seg_ids:
+            if self.segment_url is None:
+                segment = ngl.cv.skeleton.get(seg_id)
+            else:
+                cv_skel = CloudVolume(self.segment_url, use_https=True)
+                segment = cv_skel.skeleton.get(seg_id)
+            if num_verts is not None and num_verts <= len(segment.vertices):
+                if num_verts <= len(segment.vertices):
+                    verts = segment.vertices[start_vert:num_verts]
+                else:
+                    warnings.warn(
+                        UserWarning(
+                            f"Number of vertices {num_verts} greater than total vertices {len(segment.vertices)}. Defaulting to max len."
+                        )
+                    )
+                    verts = segment.vertices[start_vert:]
+            else:
+                verts = segment.vertices[start_vert:]
+            start_vert = 0
+            for v_id, vertex in enumerate(verts):
+                start = time.time()
+
+                img, bounds, voxel = ngl.pull_voxel(seg_id, v_id, self.size)
+                img_off = ngl.pull_bounds_img(bounds + self.offset)
+
+                end = time.time()
+                self.download_time += end - start
+
+                start = time.time()
+
+                features = self._convert_to_features(img)
+                features_off = self._convert_to_features(img_off)
+
+                end = time.time()
+                self.conversion_time += end - start
+
+                voxel_dict[counter] = {
+                    **{"Segment": int(seg_id), "Vertex": int(v_id), "Label": 1},
+                    **features,
+                }
+                counter += 1
+                voxel_dict[counter] = {
+                    **{"Segment": int(seg_id), "Vertex": int(v_id), "Label": 0},
+                    **features_off,
+                }
+                counter += 1
+                if write:
+                    if counter % batch_size == 0 or (counter + 1) % batch_size == 0:
+                        df = pd.DataFrame.from_dict(voxel_dict, "index")
+                        path = (
+                            file_path
+                            + str(batch_id * batch_size)
+                            + "_"
+                            + str((batch_id + 1) * batch_size)
+                            + "_"
+                            + str(seg_id)
+                            + "_"
+                            + str(v_id)
+                            + ".feather"
+                        )
+
+                        start = time.time()
+
+                        feather.write_dataframe(df, path)
+
+                        end = time.time()
+                        self.write_time += end - start
+
+                        voxel_dict = {}
+                        batch_id += 1
+
+        if file_path is None:
+            if write:
+                if not (counter % batch_size == 0 or (counter + 1) % batch_size == 0):
+                    df = pd.DataFrame.from_dict(voxel_dict, "index")
+                    path = (
+                        file_path
+                        + str(batch_id * batch_size)
+                        + "_"
+                        + str(counter)
+                        + "_"
+                        + str(seg_id)
+                        + "_"
+                        + str(v_id)
+                        + ".feather"
+                    )
+                    feather.write_dataframe(df, path)
+            else:
+                df = pd.DataFrame.from_dict(voxel_dict, "index")
+            return df
+
+    def _parallel_processing(
+        self,
+        seg_id: List[int],
+        ngl: NeuroglancerSession,
+        num_verts: int,
+        start_vert: int,
+        include_neighborhood: bool,
+        batch_size: int = None,
+        file_path: str = None,
+    ) -> Tuple[int, int, int]:
+        voxel_dict = {}
+        counter = 0
+        batch_id = 0
+        if self.segment_url is None:
+            segment = ngl.cv.skeleton.get(seg_id)
+        else:
+            cv_skel = CloudVolume(self.segment_url)
+            segment = cv_skel.skeleton.get(seg_id)
+        if num_verts is not None:
+            verts = segment.vertices[start_vert:num_verts]
+        else:
+            verts = segment.vertices[start_vert:]
+        for v_id, vertex in enumerate(verts):
+            img, bounds, voxel = ngl.pull_voxel(seg_id, v_id, self.size)
+            img_off = ngl.pull_bounds_img(bounds + self.offset)
+            features = self._convert_to_features(img, include_neighborhood)
+            features_off = self._convert_to_features(img_off, include_neighborhood)
+            voxel_dict[counter] = {
+                **{"Segment": int(seg_id), "Vertex": int(v_id), "Label": 1},
+                **features,
+            }
+            counter += 1
+            voxel_dict[counter] = {
+                **{"Segment": int(seg_id), "Vertex": int(v_id), "Label": 0},
+                **features_off,
+            }
+            counter += 1
+            if counter % batch_size == 0 or (counter + 1) % batch_size == 0:
+                df = pd.DataFrame.from_dict(voxel_dict, "index")
+                path = (
+                    file_path
+                    + str(batch_id * batch_size)
+                    + "_"
+                    + str((batch_id + 1) * batch_size)
+                    + "_"
+                    + str(seg_id)
+                    + "_"
+                    + str(v_id)
+                    + ".feather"
+                )
+
+                start = time.time()
+
+                feather.write_dataframe(df, path)
+
+                end = time.time()
+                self.write_time += end - start
+        return self.download_time, self.conversion_time, self.write_time
```

### Comparing `brainlit-0.3.3/brainlit/algorithms/generate_fragments/state_generation.py` & `brainlit-0.3.4/brainlit/preprocessing/image_process.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,706 +1,627 @@
-import zarr
+from re import VERBOSE
 import numpy as np
-import h5py
-from joblib import Parallel, delayed
-import os
-from skimage import measure
-from brainlit.preprocessing import image_process
+from skimage.measure import label, regionprops
+import scipy.ndimage as ndi
+from sklearn.metrics import pairwise_distances_argmin_min
+import matplotlib.pyplot as plt
+from itertools import product
+from typing import List, Optional, Union, Tuple
+from brainlit.utils.util import (
+    check_type,
+    check_iterable_type,
+    check_iterable_or_non_iterable_type,
+    numerical,
+)
+import collections
+import numbers
 from tqdm import tqdm
-from skimage import morphology
-from sklearn.neighbors import radius_neighbors_graph, KernelDensity
-from scipy.stats import gaussian_kde
-from brainlit.viz.swc2voxel import Bresenham3D
-from brainlit.algorithms.connect_fragments import ViterBrain
-import math
-import warnings
-import subprocess
-import random
-import pickle
-import networkx as nx
-from typing import List, Tuple
-
-from brainlit.algorithms.generate_fragments import pcurve
-
-
-class state_generation:
-    def __init__(
-        self,
-        image_path: str,
-        ilastik_program_path: str,
-        ilastik_project_path: str,
-        chunk_size: List[float] = [375, 375, 125],
-        soma_coords: List[list] = [],
-        resolution: List[float] = [0.3, 0.3, 1],
-        parallel: int = 1,
-        prob_path: str = None,
-        fragment_path: str = None,
-        tiered_path: str = None,
-        states_path: str = None,
-    ) -> None:
-
-        self.image_path = image_path
-        image = zarr.open(image_path, mode="r")
-        self.image_shape = image.shape
-        self.ilastik_program_path = ilastik_program_path
-        self.ilastik_project_path = ilastik_project_path
-        self.chunk_size = chunk_size
-        self.soma_coords = soma_coords
-        self.resolution = resolution
-        self.parallel = parallel
-
-        for other_im, name in zip(
-            [prob_path, fragment_path, tiered_path], ["prob", "frag", "tiered"]
-        ):
-            if other_im is not None:
-                other_image = zarr.open(other_im, mode="r")
-                if other_image.shape != self.image_shape:
-                    raise ValueError(f"{name} image has different shape than image")
-
-        self.prob_path = prob_path
-        self.fragment_path = fragment_path
-        self.tiered_path = tiered_path
-        self.states_path = states_path
-
-    def _predict_thread(
-        self, corner1: List[int], corner2: List[int], data_bin: str
-    ) -> None:
-        """Execute ilastik on an image chunk
-
-        Args:
-            corner1 (list of ints): first corner of image chunk
-            corner2 (list of ints): second corner of image chunk
-            data_bin (str): path to directory to store intermediate files
-        """
-        image = zarr.open(self.image_path, mode="r")
-        image_chunk = np.squeeze(
-            image[
-                corner1[0] : corner2[0],
-                corner1[1] : corner2[1],
-                corner1[2] : corner2[2],
-            ]
-        )
-        fname = data_bin + "image_" + str(corner1[2]) + ".h5"
-        with h5py.File(fname, "w") as f:
-            f.create_dataset("image_chunk", data=image_chunk)
-        subprocess.run(
-            [
-                self.ilastik_program_path,
-                "--headless",
-                f"--project={self.ilastik_project_path}",
-                fname,
-            ],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-        )
-
-    def predict(self, data_bin: str) -> None:
-        """Run ilastik on zarr image
-
-        Args:
-            data_bin (str): path to directory to store intermediate files
-        """
-        image = zarr.open(self.image_path, mode="r")
-        probabilities = zarr.zeros(
-            np.squeeze(image.shape), chunks=image.chunks, dtype="float"
-        )
-        chunk_size = self.chunk_size
-        items = self.image_path.split(".")
-        prob_fname = items[0] + "_probs.zarr"
-
-        print(
-            f"Constructing probability  image {prob_fname} of shape {probabilities.shape}"
-        )
-
-        for x in tqdm(
-            np.arange(0, image.shape[0], chunk_size[0]),
-            desc="Computing Ilastik Predictions",
-        ):
-            x2 = np.amin([x + chunk_size[0], image.shape[0]])
-            for y in tqdm(np.arange(0, image.shape[1], chunk_size[1]), leave=False):
-                y2 = np.amin([y + chunk_size[1], image.shape[1]])
-                Parallel(n_jobs=self.parallel)(
-                    delayed(self._predict_thread)(
-                        [x, y, z],
-                        [x2, y2, np.amin([z + chunk_size[2], image.shape[2]])],
-                        data_bin,
-                    )
-                    for z in np.arange(0, image.shape[2], chunk_size[2])
-                )
-
-                for f in os.listdir(data_bin):
-                    fname = os.path.join(data_bin, f)
-                    if "Probabilities" in f:
-                        items = f.split("_")
-                        z = int(items[1])
-                        z2 = np.amin([z + chunk_size[2], image.shape[2]])
-                        f = h5py.File(fname, "r")
-                        pred = f.get("exported_data")
-                        pred = pred[:, :, :, 1]
-
-                        probabilities[x:x2, y:y2, z:z2] = pred
-                    os.remove(fname)
-
-        zarr.save(prob_fname, probabilities)
-        self.prob_path = prob_fname
-
-    def _get_frag_specifications(self) -> list:
-        image = zarr.open(self.image_path, mode="r")
-        chunk_size = self.chunk_size
-        soma_coords = self.soma_coords
-
-        specifications = []
-
-        for x in np.arange(0, image.shape[0], chunk_size[0]):
-            x2 = np.amin([x + chunk_size[0], image.shape[0]])
-            for y in np.arange(0, image.shape[1], chunk_size[1]):
-                y2 = np.amin([y + chunk_size[1], image.shape[1]])
-                for z in np.arange(0, image.shape[2], chunk_size[2]):
-                    z2 = np.amin([z + chunk_size[2], image.shape[2]])
-                    soma_coords_new = []
-                    for soma_coord in soma_coords:
-                        if (
-                            np.less_equal([x, y, z], soma_coord).all()
-                            and np.less_equal(
-                                soma_coord,
-                                [x2, y2, z2],
-                            ).all()
-                        ):
-                            soma_coords_new.append(np.subtract(soma_coord, [x, y, z]))
-
-                    specifications.append(
-                        {
-                            "corner1": [x, y, z],
-                            "corner2": [x2, y2, z2],
-                            "soma_coords": soma_coords_new,
-                        }
-                    )
-
-        return specifications
-
-    def _split_frags_thread(
-        self, corner1: List[int], corner2: List[int], soma_coords: List[list] = []
-    ) -> Tuple[List[int], List[int], np.ndarray]:
-        """Compute fragments of image chunk
-
-        Args:
-            corner1 (list of ints): first corner of image chunk
-            corner2 (list of ints): second corner of image chunk
-            soma_coords (list, optional): list of soma centerpoint coordinates. Defaults to [].
-
-        Returns:
-            tuple: tuple containing corner coordinates and fragment image
-        """
-        print(f"Processing @corner: {corner1}")
-        threshold = 0.9
+from joblib import Parallel, delayed
+import multiprocessing as mp
 
-        prob = zarr.open(self.prob_path, mode="r")
 
-        im_processed = prob[
-            corner1[0] : corner2[0], corner1[1] : corner2[1], corner1[2] : corner2[2]
+def gabor_filter(
+    input: np.ndarray,
+    sigma: Union[float, List[float]],
+    phi: Union[float, List[float]],
+    frequency: float,
+    offset: float = 0.0,
+    output: Optional[Union[np.ndarray, np.dtype, None]] = None,
+    mode: str = "reflect",
+    cval: float = 0.0,
+    truncate: float = 4.0,
+) -> Tuple[np.ndarray, np.ndarray]:
+    """Multidimensional Gabor filter. A gabor filter
+    is an elementwise product between a Gaussian
+    and a complex exponential.
+
+    Parameters
+    ----------
+    input : array_like
+        The input array.
+    sigma : scalar or sequence of scalars
+        Standard deviation for Gaussian kernel. The standard
+        deviations of the Gaussian filter are given for each axis as a
+        sequence, or as a single number, in which case it is equal for
+        all axes.
+    phi : scalar or sequence of scalars
+        Angles specifying orientation of the periodic complex
+        exponential. If the input is n-dimensional, then phi
+        is a sequence of length n-1. Convention follows
+        https://en.wikipedia.org/wiki/N-sphere#Spherical_coordinates.
+    frequency : scalar
+        Frequency of the complex exponential. Units are revolutions/voxels.
+    offset : scalar
+        Phase shift of the complex exponential. Units are radians.
+    output : array or dtype, optional
+        The array in which to place the output, or the dtype of the returned array.
+        By default an array of the same dtype as input will be created. Only the real component will be saved
+        if output is an array.
+    mode : {‘reflect’, ‘constant’, ‘nearest’, ‘mirror’, ‘wrap’}, optional
+        The mode parameter determines how the input array is extended beyond its boundaries.
+        Default is ‘reflect’.
+    cval : scalar, optional
+        Value to fill past edges of input if mode is ‘constant’. Default is 0.0.
+    truncate : float
+        Truncate the filter at this many standard deviations.
+        Default is 4.0.
+
+    Returns
+    -------
+    real, imaginary : arrays
+        Returns real and imaginary responses, arrays of same
+        shape as `input`.
+
+    Notes
+    -----
+    The multidimensional filter is implemented by creating
+    a gabor filter array, then using the convolve method.
+    Also, sigma specifies the standard deviations of the
+    Gaussian along the coordinate axes, and the Gaussian
+    is not rotated. This is unlike
+    skimage.filters.gabor, whose Gaussian is
+    rotated with the complex exponential.
+    The reasoning behind this design choice is that
+    sigma can be more easily designed to deal with
+    anisotropic voxels.
+
+    Examples
+    --------
+    >>> from brainlit.preprocessing import gabor_filter
+    >>> a = np.arange(50, step=2).reshape((5,5))
+    >>> a
+    array([[ 0,  2,  4,  6,  8],
+           [10, 12, 14, 16, 18],
+           [20, 22, 24, 26, 28],
+           [30, 32, 34, 36, 38],
+           [40, 42, 44, 46, 48]])
+    >>> gabor_filter(a, sigma=1, phi=[0.0], frequency=0.1)
+    (array([[ 3,  5,  6,  8,  9],
+            [ 9, 10, 12, 13, 14],
+            [16, 18, 19, 21, 22],
+            [24, 25, 27, 28, 30],
+            [29, 30, 32, 34, 35]]),
+     array([[ 0,  0, -1,  0,  0],
+            [ 0,  0, -1,  0,  0],
+            [ 0,  0, -1,  0,  0],
+            [ 0,  0, -1,  0,  0],
+            [ 0,  0, -1,  0,  0]]))
+
+    >>> from scipy import misc
+    >>> import matplotlib.pyplot as plt
+    >>> fig = plt.figure()
+    >>> plt.gray()  # show the filtered result in grayscale
+    >>> ax1 = fig.add_subplot(121)  # left side
+    >>> ax2 = fig.add_subplot(122)  # right side
+    >>> ascent = misc.ascent()
+    >>> result = gabor_filter(ascent, sigma=5, phi=[0.0], frequency=0.1)
+    >>> ax1.imshow(ascent)
+    >>> ax2.imshow(result[0])
+    >>> plt.show()
+    """
+    check_type(input, (list, np.ndarray))
+    check_iterable_or_non_iterable_type(sigma, numerical)
+    check_iterable_or_non_iterable_type(phi, numerical)
+    check_type(frequency, numerical)
+    check_type(offset, numerical)
+    check_type(cval, numerical)
+    check_type(truncate, numerical)
+
+    input = np.asarray(input)
+
+    # Checks that dimensions of inputs are correct
+    sigmas = ndi._ni_support._normalize_sequence(sigma, input.ndim)
+    phi = ndi._ni_support._normalize_sequence(phi, input.ndim - 1)
+
+    limits = [np.ceil(truncate * sigma).astype(int) for sigma in sigmas]
+    ranges = [range(-limit, limit + 1) for limit in limits]
+    coords = np.meshgrid(*ranges, indexing="ij")
+    filter_size = coords[0].shape
+    coords = np.stack(coords, axis=-1)
+
+    new_shape = np.ones(input.ndim)
+    new_shape = np.append(new_shape, -1).astype(int)
+    sigmas = np.reshape(sigmas, new_shape)
+
+    g = np.zeros(filter_size, dtype=complex)
+    g[:] = np.exp(-0.5 * np.sum(np.divide(coords, sigmas) ** 2, axis=-1))
+
+    g /= (2 * np.pi) ** (input.ndim / 2) * np.prod(sigmas)
+    orientation = np.ones(input.ndim)
+    for i, p in enumerate(phi):
+        orientation[i + 1] = orientation[i] * np.sin(p)
+        orientation[i] = orientation[i] * np.cos(p)
+    orientation = np.flip(orientation)
+    rotx = coords @ orientation
+    g *= np.exp(1j * (2 * np.pi * frequency * rotx + offset))
+
+    if isinstance(output, (type, np.dtype)):
+        otype = output
+    elif isinstance(output, str):
+        otype = np.sctypeDict[output]
+    else:
+        otype = None
+
+    output = ndi.convolve(
+        input, weights=np.real(g), output=output, mode=mode, cval=cval
+    )
+    imag = ndi.convolve(input, weights=np.imag(g), output=otype, mode=mode, cval=cval)
+
+    result = (output, imag)
+    return result
+
+
+def getLargestCC(segmentation: np.ndarray) -> np.ndarray:
+    """Returns the largest connected component of a image.
+
+    Arguments:
+    segmentation : Segmentation data of image or volume.
+
+    Returns:
+    largeCC : Segmentation with only largest connected component.
+    """
+
+    check_type(segmentation, (list, np.ndarray))
+    labels = label(segmentation)
+    if labels.max() == 0:
+        raise ValueError("No connected components!")  # assume at least 1 CC
+    largestCC = labels == np.argmax(np.bincount(labels.flat)[1:]) + 1
+    return largestCC
+
+
+def removeSmallCCs(
+    segmentation: np.ndarray, size: Union[int, float], verbose=False
+) -> np.ndarray:
+    """Removes small connected components from an image.
+
+    Parameters:
+    segmentation : Segmentation data of image or volume.
+    size : Maximum connected component size to remove.
+
+    Returns:
+    largeCCs : Segmentation with small connected components removed.
+    """
+    check_type(segmentation, (list, np.ndarray))
+    check_type(size, numerical)
+
+    labels = label(segmentation, return_num=False)
+    counts = np.bincount(labels.flat)[1:]
+
+    for v, count in enumerate(
+        tqdm(counts, desc="looking for components to remove", disable=not verbose)
+    ):
+        if count < size:
+            labels[labels == v + 1] = 0
+
+    largeCCs = labels != 0
+    return largeCCs
+
+
+def label_points(labels: np.array, points: list, res: list) -> Tuple[list, list]:
+    """Adjust points so they fall on a foreground component of labels.
+
+    Args:
+        labels (array): labeled components, such as output from measure.label
+        points (list): points to be adjusted
+        res (list): voxel size
+
+    Returns:
+        [list]: adjusted points
+        [list]: labels of adjusted points
+    """
+    point_labels = []
+    nonzero_locs = np.argwhere(labels)
+    for i, point in enumerate(points):
+        too_big = [p >= l for p, l in zip(point, labels.shape)]
+        if any(too_big) or labels[point[0], point[1], point[2]] == 0:
+            dif = np.multiply(np.subtract(nonzero_locs, point), res)
+            dists = np.linalg.norm(dif, axis=1)
+            arg_min = np.argmin(dists)
+            points[i] = nonzero_locs[arg_min, :]
+        point = points[i]
+        point_labels.append(labels[tuple(point)])
+    return points, point_labels
+
+
+def _get_chunked_args(
+    soma_coords: list,
+    labels: np.array,
+    im_processed: np.array,
+    chunk_size: Optional[list] = [200, 200, 200],
+) -> dict:
+    """Splits large image data into smaller chunks so fragments can be generated in parallel.
+
+    Args:
+        soma_coords (list): list of voxel coordinates of somas
+        labels (np.array): image segmentation
+        im_processed (np.array): voxel-wise probability predictions for foreground
+        chunk_size (list, optional): size of image chunks. Defaults to [200, 200, 200].
+
+    Yields:
+        dict: dictionary of arguments that depend on chunking
+    """
+    shp = labels.shape
+
+    for x1 in np.arange(0, shp[0], chunk_size[0]):
+        x2 = np.amin([x1 + chunk_size[0], shp[0]])
+        for y1 in np.arange(0, shp[1], chunk_size[1]):
+            y2 = np.amin([y1 + chunk_size[1], shp[1]])
+            for z1 in np.arange(0, shp[2], chunk_size[2]):
+                z2 = np.amin([z1 + chunk_size[2], shp[2]])
+                soma_coords_new = []
+                for soma_coord in soma_coords:
+                    if (
+                        np.less_equal([x1, y1, z1], soma_coord).all()
+                        and np.less_equal(
+                            soma_coord,
+                            [x2, y2, z2],
+                        ).all()
+                    ):
+                        soma_coords_new.append(np.subtract(soma_coord, [x1, y1, z1]))
+                yield {
+                    "soma_coords": soma_coords_new,
+                    "labels": labels[x1:x2, y1:y2, z1:z2],
+                    "im_processed": im_processed[x1:x2, y1:y2, z1:z2],
+                }
+
+
+def _merge_chunked_labels(
+    labels: list,
+    new_shape: Tuple[int, int, int],
+    chunk_size: Optional[list] = [200, 200, 200],
+) -> np.array:
+    """Merges the fragments of the chunked image. Assumes that chunking was done according to method in _get_chunked_args
+
+    Args:
+        labels (list): list of fragments generated by image chunks.
+        new_shape (3-tuple of ints): size of stitched image
+        chunk_size (list, optional): [description]. Defaults to [200, 200, 200].
+
+    Returns:
+        np.array: complete label image
+    """
+    new_labels = np.zeros(new_shape, dtype="int")
+    idx = 0
+    max = 0
+    for x1 in np.arange(0, new_shape[0], chunk_size[0]):
+        x2 = np.amin([x1 + chunk_size[0], new_shape[0]])
+        for y1 in np.arange(0, new_shape[1], chunk_size[1]):
+            y2 = np.amin([y1 + chunk_size[1], new_shape[1]])
+            for z1 in np.arange(0, new_shape[2], chunk_size[2]):
+                z2 = np.amin([z1 + chunk_size[2], new_shape[2]])
+
+                lab = labels[idx]
+                lab[lab > 0] += max
+                new_labels[x1:x2, y1:y2, z1:z2] = lab
+
+                max = np.amax(lab)
+                idx += 1
+    return new_labels
+
+
+def compute_frags(
+    soma_coords: list,
+    labels: np.array,
+    im_processed: np.array,
+    threshold: float,
+    res: list,
+    chunk_size: list = None,
+    ncpu: int = 2,
+) -> np.array:
+    """Preprocesses a neuron image segmentation by splitting up non-soma components into 5 micron segments.
+
+    Args:
+        soma_coords (list): list of voxel coordinates of somas
+        labels (np.array): image segmentation
+        im_processed (np.array): voxel-wise probability predictions for foreground
+        threshold (float): threshold used to segment probability predictions into mask
+        res (list): voxel size in image
+        chunk_size (list): size of image chunks
+        ncpu (int): number of cpus to use in parallel mode
+
+    Returns:
+        np.array: new image segmentation - different numbers indicate different fragments, 0 is background
+    """
+    og_shape = labels.shape
+    if chunk_size is None:
+        new_labels = split_frags(soma_coords, labels, im_processed, threshold, res)
+    else:
+        args = _get_chunked_args(
+            soma_coords, labels, im_processed, chunk_size=chunk_size
+        )
+        inputs = [
+            (arg["soma_coords"], arg["labels"], arg["im_processed"], threshold, res)
+            for arg in args
         ]
-        labels = measure.label(im_processed > threshold)
-
-        radius_states = 7
-
-        (
-            image_iterative,
-            states,
-            comp_to_states,
-            new_soma_masks,
-        ) = image_process.remove_somas(
-            soma_coords, labels, im_processed, res=self.resolution, verbose=False
-        )
-        mask = labels > 0
-        mask2 = image_process.removeSmallCCs(mask, 25)
-        image_iterative[mask & (~mask2)] = 0
-
-        states, comp_to_states = image_process.split_frags_place_points(
-            image_iterative=image_iterative,
-            labels=labels,
-            radius_states=radius_states,
-            res=self.resolution,
-            threshold=threshold,
-            states=states,
-            comp_to_states=comp_to_states,
-            verbose=False,
-        )
-
-        new_labels = image_process.split_frags_split_comps(
-            labels, new_soma_masks, states, comp_to_states, verbose=False
-        )
-
-        new_labels = image_process.split_frags_split_fractured_components(
-            new_labels, verbose=False
-        )
-
-        props = measure.regionprops(new_labels)
-        for _, prop in enumerate(
-            tqdm(props, desc="remove small fragments", disable=True)
-        ):
-            if prop.area < 15:
-                new_labels[new_labels == prop.label] = 0
-
-        new_labels = image_process.rename_states_consecutively(new_labels)
-
-        return (corner1, corner2, new_labels)
-
-    def compute_frags(self) -> None:
-        """Compute all fragments for image"""
-        image = zarr.open(self.image_path, mode="r")
-        fragments = zarr.zeros(
-            np.squeeze(image.shape), chunks=image.chunks, dtype="uint16"
-        )
-        items = self.image_path.split(".")
-        frag_fname = items[0] + "_labels.zarr"
+        with mp.Pool(ncpu) as pool:
+            new_labelss = pool.starmap(split_frags, inputs)
 
-        print(f"Constructing fragment image {frag_fname} of shape {fragments.shape}")
+        new_labels = _merge_chunked_labels(new_labelss, og_shape, chunk_size=chunk_size)
+    return new_labels
 
-        specifications = self._get_frag_specifications()
 
-        results = Parallel(n_jobs=self.parallel)(
-            delayed(self._split_frags_thread)(
-                specification["corner1"],
-                specification["corner2"],
-                specification["soma_coords"],
-            )
-            for specification in specifications
-        )
+def split_frags(
+    soma_coords: list,
+    labels: np.array,
+    im_processed: np.array,
+    threshold: float,
+    res: list,
+    verbose=False,
+) -> np.array:
+    """Preprocesses a single image chunk by splitting up non-soma components into 5 micron segments
+
+    Args:
+        soma_coords (list): list of voxel coordinates of somas
+        labels (np.array): image segmentation
+        im_processed (np.array): voxel-wise probability predictions for foreground
+        threshold (float): threshold used to segment probability predictions into mask
+        res (list): voxel size in image
+
+    Returns:
+        np.array: new image segmentation - different numbers indicate different fragments, 0 is background
+    """
+    radius_states = 7
+    image_iterative, states, comp_to_states, new_soma_masks = remove_somas(
+        soma_coords, labels, im_processed, res
+    )
+
+    mask = labels > 0
+    mask2 = removeSmallCCs(mask, 25)
+    image_iterative[mask & (~mask2)] = 0
+
+    states, comp_to_states = split_frags_place_points(
+        image_iterative,
+        labels,
+        radius_states,
+        res,
+        threshold,
+        states,
+        comp_to_states,
+    )
+
+    new_labels = split_frags_split_comps(labels, new_soma_masks, states, comp_to_states)
+
+    new_labels = split_frags_split_fractured_components(new_labels)
+
+    props = regionprops(new_labels)
+    for label, prop in enumerate(
+        tqdm(props, desc="remove small fragments", disable=not verbose)
+    ):
+        if prop.area < 15:
+            new_labels[new_labels == prop.label] = 0
+
+    new_labels = rename_states_consecutively(new_labels)
+
+    return new_labels
+
+
+def remove_somas(
+    soma_coords: list,
+    labels: np.array,
+    im_processed: np.array,
+    res: list,
+    verbose=False,
+) -> Tuple[np.array, list, dict, list]:
+    """Helper function of split_frags. Removes area around somas.
+
+    Args:
+        soma_coords (list): list of voxel coordinates of somas
+        labels (np.array): image segmentation
+        im_processed (np.array): voxel-wise probability predictions for foreground
+        res (list): voxel size in image
+
+    Returns:
+        np.array: probability predictions, with the soma regions masked
+        list: coordinates of the points
+        dictionary: map from component in labels, to set of points that were placed there
+        list: masks of the different somas
+    """
+    states = []
+    comp_to_states = {}
+    # probability image, with all soma regions set to 0
+    image_iterative = np.copy(im_processed)
+    # list of soma region masks
+    new_soma_masks = []
+
+    for soma_pt in tqdm(soma_coords, desc="removing somas", disable=not verbose):
+        _, end_lbls = label_points(labels, [soma_pt], res)
+        soma_lbl = end_lbls[0]
+        soma_mask = labels == soma_lbl
+
+        states.append(np.array(soma_pt))
+        comp = labels[soma_pt[0], soma_pt[1], soma_pt[2]]
+        comp_to_states[comp] = [len(states) - 1]
+
+        # soma component is all the voxels of that component within 12 microns of the soma point
+        dist = np.ones_like(image_iterative)
+        dist[soma_pt[0], soma_pt[1], soma_pt[2]] = 0
+        dt = ndi.distance_transform_edt(dist, sampling=[0.3, 0.3, 1])
+        sphere = dt < 15
+        new_soma_mask = np.logical_and(soma_mask, sphere)
+
+        image_iterative[new_soma_mask] = 0
+        new_soma_masks.append(new_soma_mask)
+
+    return image_iterative, states, comp_to_states, new_soma_masks
+
+
+def split_frags_place_points(
+    image_iterative: np.array,
+    labels: np.array,
+    radius_states: float,
+    res: list,
+    threshold: float,
+    states: list,
+    comp_to_states: dict,
+    verbose=False,
+) -> Tuple[list, dict]:
+    """Helper function of split_frags. Places points on high probability voxels while keeping the points a certain distance apart from each other.
+
+    Args:
+        image_iterative (np.array): probability predictions, with the soma regions masked
+        labels (np.array): image segmentation
+        radius_states (float): distance constraint between points
+        res (list): voxel size in image
+        threshold (float): threshold used to segment probability predictions into mask
+        states (list): coordinates of the points
+        comp_to_states (dictionary): map from component in labels, to set of points that were placed there
+
+    Returns:
+        list: coordinates of the points
+        dictionary: map from component in labels, to set of points that were placed there
+    """
+    top_ind = np.unravel_index(
+        np.argmax(image_iterative, axis=None), image_iterative.shape
+    )
+    top = image_iterative[top_ind[0], top_ind[1], top_ind[2]]
+
+    radius_vox = np.divide(radius_states, res).astype(int)
+
+    prev_tot = np.sum(image_iterative > threshold)
+
+    with tqdm(total=prev_tot, desc="Adding points...", disable=not verbose) as pbar:
+        while top > threshold:
+            states.append(top_ind)
+
+            comp = labels[top_ind[0], top_ind[1], top_ind[2]]
+            if comp in comp_to_states.keys():
+                lst = comp_to_states[comp]
+                lst.append(len(states) - 1)
+                comp_to_states[comp] = lst
+            else:
+                comp_to_states[comp] = [len(states) - 1]
 
-        max_label = 0
-        for result in results:
-            corner1, corner2, labels = result
-            labels[labels > 0] += max_label
-            max_label = np.amax([max_label, np.amax(labels)])
-            fragments[
-                corner1[0] : corner2[0],
-                corner1[1] : corner2[1],
-                corner1[2] : corner2[2],
-            ] = labels
-        print(f"*****************Number of components: {max_label}*******************")
-        zarr.save(frag_fname, fragments)
-
-        self.fragment_path = frag_fname
-
-    def compute_soma_lbls(self) -> None:
-        """Compute fragment ids of soma coordinates."""
-        fragments = zarr.open(self.fragment_path, mode="r")
-
-        soma_lbls = []
-        radius = 20
-        for soma_coord in self.soma_coords:
-            local_labels = fragments[
-                np.amax([soma_coord[0] - radius, 0]) : soma_coord[0] + radius,
-                np.amax([soma_coord[1] - radius, 0]) : soma_coord[1] + radius,
-                np.amax([soma_coord[2] - radius, 0]) : soma_coord[2] + radius,
+            l_bd = [
+                np.amax([0, top_ind[0] - radius_vox[0]]),
+                np.amax([0, top_ind[1] - radius_vox[1]]),
+                np.amax([0, top_ind[2] - radius_vox[2]]),
             ]
-            soma_label = image_process.label_points(
-                local_labels, [[radius, radius, radius]], res=self.resolution
-            )[1][0]
-            soma_lbls.append(soma_label)
-
-        self.soma_lbls = soma_lbls
-
-    def _compute_image_tiered_thread(
-        self, corner1: List[int], corner2: List[int]
-    ) -> Tuple[List[int], List[int], np.ndarray]:
-        """Compute tiered image (image likelihood costs)
-
-        Args:
-            corner1 (list of ints): first corner of image chunk
-            corner2 (list of ints): second corner of image chunk
-
-        Returns:
-            tuple: tuple containing corner coordinates and tiered image
-        """
-        print(f"Processing @corner: {corner1}-{corner2}")
-        kde = self.kde
-        image = zarr.open(self.image_path, mode="r")
-
-        image = image[
-            corner1[0] : corner2[0], corner1[1] : corner2[1], corner1[2] : corner2[2]
-        ]
-
-        vals = np.unique(image)
-        scores_neg = -1 * kde.logpdf(vals)
-
-        data = np.reshape(np.copy(image), (image.size,))
-        sort_idx = np.argsort(vals)
-        idx = np.searchsorted(vals, data, sorter=sort_idx)
-        out = scores_neg[sort_idx][idx]
-        image_tiered = np.reshape(out, image.shape)
-
-        return (corner1, corner2, image_tiered)
-
-    def compute_image_tiered(self) -> None:
-        """Compute entire tiered image then reassemble and save as zarr"""
-        image = zarr.open(self.image_path, mode="r")
-        fragments = zarr.open(self.fragment_path, mode="r")
-        tiered = zarr.zeros(
-            np.squeeze(image.shape), chunks=image.chunks, dtype="uint16"
-        )
-        items = self.image_path.split(".")
-        tiered_fname = items[0] + "_tiered.zarr"
-        print(f"Constructing tiered image {tiered_fname} of shape {tiered.shape}")
-
-        image_chunk = image[:300, :300, :300]
-        fragments_chunk = fragments[:300, :300, :300]
-        data_fg = image_chunk[fragments_chunk > 0]
-        if len(data_fg.flatten()) > 10000:
-            data_sample = random.sample(list(data_fg), k=10000)
-        else:
-            data_sample = data_fg
-
-        kde = gaussian_kde(data_sample)
-
-        self.kde = kde
-
-        specifications = self._get_frag_specifications()
-
-        results = Parallel(n_jobs=self.parallel)(
-            delayed(self._compute_image_tiered_thread)(
-                specification["corner1"],
-                specification["corner2"],
-            )
-            for specification in specifications
-        )
-
-        for result in results:
-            corner1, corner2, image_tiered = result
-            tiered[
-                corner1[0] : corner2[0],
-                corner1[1] : corner2[1],
-                corner1[2] : corner2[2],
-            ] = image_tiered
-
-        zarr.save(tiered_fname, tiered)
-        self.tiered_path = tiered_fname
-
-    def _compute_bounds(
-        self, label: np.ndarray, pad: float
-    ) -> Tuple[int, int, int, int, int, int]:
-        """compute coordinates of bounding box around a masked object, with given padding
-
-        Args:
-            label (np.array): mask of the object
-            pad (float): padding around object in um
-
-        Returns:
-            ints: integer coordinates of bounding box
-        """
-        image_shape = self.image_shape
-        res = self.resolution
-
-        r = np.any(label, axis=(1, 2))
-        c = np.any(label, axis=(0, 2))
-        z = np.any(label, axis=(0, 1))
-        rmin, rmax = np.where(r)[0][[0, -1]]
-        rmin = np.amax((0, math.floor(rmin - pad / res[0])))
-        rmax = np.amin((image_shape[0], math.ceil(rmax + (pad + 1) / res[0])))
-        cmin, cmax = np.where(c)[0][[0, -1]]
-        cmin = np.amax((0, math.floor(cmin - (pad) / res[1])))
-        cmax = np.amin((image_shape[1], math.ceil(cmax + (pad + 1) / res[1])))
-        zmin, zmax = np.where(z)[0][[0, -1]]
-        zmin = np.amax((0, math.floor(zmin - (pad) / res[2])))
-        zmax = np.amin((image_shape[2], math.ceil(zmax + (pad + 1) / res[2])))
-        return int(rmin), int(rmax), int(cmin), int(cmax), int(zmin), int(zmax)
-
-    def _endpoints_from_coords_neighbors(self, coords: np.ndarray) -> List[list]:
-        """Compute endpoints of fragment.
-
-        Args:
-            coords (np.array): coordinates of voxels in the fragment
-
-        Returns:
-            list: endpoints of the fragment
-        """
-        res = self.resolution
-
-        dims = np.multiply(np.amax(coords, axis=0) - np.amin(coords, axis=0), res)
-        max_length = np.sqrt(np.sum([dim**2 for dim in dims]))
-
-        r = 15
-        if max_length < r:
-            radius = max_length / 2
-            close_enough = radius
-        else:
-            radius = r
-            close_enough = 9
-
-        A = radius_neighbors_graph(
-            coords, radius=radius, metric="wminkowski", metric_params={"w": res}
-        )
-        degrees = np.squeeze(np.array(np.sum(A, axis=1).T, dtype=int))
-        indices = np.argsort(degrees)
-        sorted = [degrees[i] for i in indices]
-
-        # point with fewest neighbors
-        ends = [coords[indices[0], :]]
-        # second endpoint is point with fewest neighbors that is not within "close_enough" of the first endpoint
-        # close_enough gets smaller until a second point is found
-        while len(ends) < 2:
-            for coord_idx, degree in zip(indices, sorted):
-                coord = coords[coord_idx, :]
-                dists = np.array(
-                    [np.linalg.norm(np.multiply(coord - end, res)) for end in ends]
-                )
-                if not any(dists < close_enough):
-                    ends.append(coord)
-                    break
-            close_enough = close_enough / 2
-
-        return ends
-
-    def _pc_endpoints_from_coords_neighbors(self, coords: np.ndarray) -> List[list]:
-        """Compute endpoints of fragment with Principal Curves.
-
-        Args:
-            coords (np.array): coordinates of voxels in the fragment
-
-        Returns:
-            list: endpoints of the fragment
-
-        References
-        ----------
-        .. [1] Hastie, Trevor, and Werner Stuetzle. “Principal Curves.”
-        Journal of the American Statistical Association, vol. 84, no. 406,
-        [American Statistical Association, Taylor & Francis, Ltd.], 1989,
-        pp. 502–16, https://doi.org/10.2307/2289936.
-        .. [2] Principal Curves Code written by zsteve,
-        https://github.com/zsteve, https://github.com/zsteve/pcurvepy
-        """
-
-        ends = []
-
-        # Make sure x, y, z ascending & don't repeat
-        sorter = np.lexsort((coords[:, 2], coords[:, 1], coords[:, 0]))
-        coords = coords[sorter]
-        coords = np.unique(coords, axis=0)
-
-        p_curve = pcurve.PrincipalCurve(k=1, s_factor=5)
-        p_curve.fit(coords, max_iter=50)
-        pc = p_curve.p
-
-        pc = np.floor(pc + 0.5)
-        pc_frag_list = [i for i in pc if i in coords]
-
-        ends.append(pc_frag_list[0])
-        ends.append(pc_frag_list[-1])
-
-        return ends
-
-    def _compute_states_thread(
-        self, corner1: List[int], corner2: List[int]
-    ) -> List[tuple]:
-        """Compute states of fragments within image chunk
-
-        Args:
-            corner1 (list of ints): first corner of image chunk
-            corner2 (list of ints): second corner of image chunk
-
-        Raises:
-            ValueError: only one endpoint found for fragment
-
-        Returns:
-            [list]: list of tuples containing fragment and state information
-        """
-        fragments_zarr = zarr.open(self.fragment_path, mode="r")
-        tiered_zarr = zarr.open(self.tiered_path, mode="r")
-        labels = fragments_zarr[
-            corner1[0] : corner2[0], corner1[1] : corner2[1], corner1[2] : corner2[2]
-        ]
-        image_tiered = tiered_zarr[
-            corner1[0] : corner2[0], corner1[1] : corner2[1], corner1[2] : corner2[2]
-        ]
-        unq = np.unique(labels)
-        components = unq[unq != 0]
-
-        results = []
-        for component in tqdm(
-            components,
-            desc=f"Computing state representations @corner {corner1}-{corner2}",
-        ):
-            mask = labels == component
-
-            if component in self.soma_lbls:
-                results.append(
-                    (
-                        component,
-                        np.add(np.argwhere(mask), corner1),
-                        None,
-                        None,
-                        None,
-                        None,
-                    )
-                )
-                continue
-
-            rmin, rmax, cmin, cmax, zmin, zmax = self._compute_bounds(mask, pad=1)
-            # now in bounding box coordinates
-            mask = mask[rmin:rmax, cmin:cmax, zmin:zmax]
-
-            skel = morphology.skeletonize_3d(mask)
-
-            coords_mask = np.argwhere(mask)
-            coords_skel = np.argwhere(skel)
-            if len(coords_skel) < 4:
-                coords = coords_mask
-            else:
-                coords = coords_skel
+            u_bd = [
+                np.amin([image_iterative.shape[0], top_ind[0] + radius_vox[0]]),
+                np.amin([image_iterative.shape[1], top_ind[1] + radius_vox[1]]),
+                np.amin([image_iterative.shape[2], top_ind[2] + radius_vox[2]]),
+            ]
+            image_iterative[l_bd[0] : u_bd[0], l_bd[1] : u_bd[1], l_bd[2] : u_bd[2]] = 0
 
-            endpoints_initial = self._endpoints_from_coords_neighbors(coords)
-            endpoints = endpoints_initial.copy()
-            for i, endpoint in enumerate(endpoints_initial):
-                if mask[endpoint[0], endpoint[1], endpoint[2]] != 1:
-                    difs = np.multiply(
-                        np.subtract(coords_mask, endpoint), self.resolution
-                    )
-                    dists = np.linalg.norm(difs, axis=1)
-                    argmin = np.argmin(dists)
-                    endpoints[i] = coords_mask[argmin, :]
-            a = endpoints[0]
-            try:
-                b = endpoints[1]
-            except:
-                print(f"only 1 endpoint for component {component}")
-                raise ValueError
-
-            # now in chunk coordinates
-            a = np.add(a, [rmin, cmin, zmin])
-            b = np.add(b, [rmin, cmin, zmin])
-            dif = b - a
-            dif = dif / np.linalg.norm(dif)
-
-            a = [int(x) for x in a]
-            b = [int(x) for x in b]
-
-            xlist, ylist, zlist = Bresenham3D(a[0], a[1], a[2], b[0], b[1], b[2])
-            sum = np.sum(image_tiered[xlist, ylist, zlist])
-            if sum < 0:
-                warnings.warn(f"Negative int cost for comp {component}: {sum}")
-
-            # now in full image coordinates
-            a = np.add(a, corner1)
-            b = np.add(b, corner1)
-
-            results.append((component, a, b, -dif, dif, sum))
-        return results
-
-    def compute_states(self) -> None:
-        """Compute entire collection of states
-
-        Raises:
-            ValueError: erroneously computed endpoints of soma state
-        """
-        print(f"Computing states")
-        items = self.image_path.split(".")
-        states_fname = items[0] + "_nx.pickle"
-
-        specifications = self._get_frag_specifications()
-
-        results_tuple = Parallel(n_jobs=self.parallel)(
-            delayed(self._compute_states_thread)(
-                specification["corner1"],
-                specification["corner2"],
+            top_ind = np.unravel_index(
+                np.argmax(image_iterative, axis=None), image_iterative.shape
             )
-            for specification in specifications
-        )
-        results = [item for result in results_tuple for item in result]
+            top = image_iterative[top_ind[0], top_ind[1], top_ind[2]]
 
-        state_num = 0
-        G = nx.DiGraph()
-        soma_comp2state = {}
-        for result in results:
-            component, a, b, oa, ob, sum = result
-            if component in self.soma_lbls:
-                if b is not None:
-                    raise ValueError(
-                        f"Component {component} is a soma component but the state is not a soma: {result}"
-                    )
-                if component in soma_comp2state.keys():
-                    coords1 = G.nodes[soma_comp2state[component]]["soma_coords"]
-                    coords2 = a
-                    coords = np.concatenate((coords1, coords2))
-                    G.nodes[soma_comp2state[component]]["soma_coords"] = coords
-                else:
-                    G.add_node(
-                        state_num, type="soma", fragment=component, soma_coords=a
-                    )
-                    soma_comp2state[component] = state_num
-            else:
-                G.add_node(
-                    state_num,
-                    type="fragment",
-                    fragment=component,
-                    point1=a,
-                    point2=b,
-                    orientation1=-oa,
-                    orientation2=ob,
-                    image_cost=sum,
-                    twin=state_num + 1,
-                )
-
-                state_num += 1
-                G.add_node(
-                    state_num,
-                    type="fragment",
-                    fragment=component,
-                    point1=b,
-                    point2=a,
-                    orientation1=-ob,
-                    orientation2=oa,
-                    image_cost=sum,
-                    twin=state_num - 1,
-                )
-
-            state_num += 1
-        print(
-            f"*****************Number of states: {G.number_of_nodes()}*******************"
-        )
+            tot = np.sum(image_iterative > threshold)
+            pbar.update(prev_tot - tot)
+            prev_tot = tot
+
+    return states, comp_to_states
+
+
+def split_frags_split_comps(
+    labels: np.array, new_soma_masks, states: list, comp_to_states: dict, verbose=False
+) -> np.array:
+    """Helper function of split_frags. Splits the components according to the points that were placed by split_frags_place_points.
+
+    Args:
+        labels (np.array): image segmentation
+        new_soma_masks ([type]): [description]
+        states (list): coordinates of the points
+        comp_to_states (dictionary): map from component in labels, to set of points that were placed there
+
+    Returns:
+        np.array: new image segmentation - different numbers indicate different fragments, 0 is background
+    """
+    labels_split = np.copy(labels)
+
+    next_lbl = np.amax(labels) + 1
+    for comp in tqdm(
+        comp_to_states.keys(), desc="Splitting Fragments", disable=not verbose
+    ):
+        comp_states = comp_to_states[comp]
+        if len(comp_states) > 1:
+            state_coords = []
+            for state in comp_states:
+                state_coords.append(states[state])
+            state_coords = np.stack(state_coords)
+            comp_coords = np.argwhere(labels == comp)
+            amin, _ = pairwise_distances_argmin_min(comp_coords, state_coords)
+
+            for s, state in enumerate(np.unique(amin)):
+                if s > 0:
+                    coords = comp_coords[amin == state]
+                    labels_split[coords[:, 0], coords[:, 1], coords[:, 2]] = next_lbl
+                    next_lbl += 1
+    mx = np.amax(labels_split)
+
+    for i, new_soma_mask in enumerate(new_soma_masks):
+        labels_split[new_soma_mask] = mx + 1 + i
+    new_labels = labels_split
+    return new_labels
+
+
+def split_frags_split_fractured_components(
+    new_labels: np.array, verbose=False
+) -> np.array:
+    """Helper function of split_frags. Some fragments from split_frags_split_comps may not be connected so this function separates those.
+
+    Args:
+        new_labels (np.array): new image segmentation - different numbers indicate different fragments, 0 is background
+
+    Returns:
+        np.array: new image segmentation - different numbers indicate different fragments, 0 is background
+    """
+    props = regionprops(new_labels)
+    new_lbl = np.amax(new_labels) + 1
+    for prop in tqdm(props, desc="Split fractured components", disable=not verbose):
+        bbox = prop["bbox"]
+        lbl = prop["label"]
+        cutout = new_labels[bbox[0] : bbox[3], bbox[1] : bbox[4], bbox[2] : bbox[5]]
+        mask = cutout == lbl
+        lbl_labels = label(mask)
+        for lbl_label in np.unique(lbl_labels):
+            if lbl_label not in [0, 1]:
+                cutout[lbl_labels == lbl_label] = new_lbl
+                new_lbl += 1
+
+    return new_labels
+
+
+def rename_states_consecutively(new_labels: np.array) -> np.array:
+    """Helper function of split_frags. Relabel components in image segmentation so the unique values are consecutive.
+
+    Args:
+        new_labels (np.array): new image segmentation - different numbers indicate different fragments, 0 is background
+
+    Returns:
+        np.array: new image segmentation - different numbers indicate different fragments, 0 is background
+    """
+    vals = np.unique(new_labels)
+    vals = np.delete(vals, 0)
+    vals = np.append(vals, [0])
+    new_vals = np.arange(1, len(vals))
+    new_vals = np.append(new_vals, [0])
+
+    data = np.reshape(np.copy(new_labels), (new_labels.size,))
+    sort_idx = np.argsort(vals)
+    idx = np.searchsorted(vals, data, sorter=sort_idx)
+    out = new_vals[sort_idx][idx]
+    new_labels = np.reshape(out, new_labels.shape)
 
-        with open(states_fname, "wb") as handle:
-            pickle.dump(G, handle)
-
-        self.states_path = states_fname
-
-    def compute_edge_weights(self) -> None:
-        """Create viterbrain object and compute edge weights"""
-        items = self.image_path.split(".")
-        viterbrain_fname = items[0] + "_viterbrain.pickle"
-
-        with open(self.states_path, "rb") as handle:
-            G = pickle.load(handle)
-
-        viterbrain = ViterBrain(
-            G,
-            self.tiered_path,
-            fragment_path=self.fragment_path,
-            resolution=self.resolution,
-            coef_curv=1000,
-            coef_dist=10,
-            coef_int=1,
-            parallel=self.parallel,
-        )
-
-        viterbrain.compute_all_costs_dist(
-            frag_frag_func=viterbrain.frag_frag_dist,
-            frag_soma_func=viterbrain.frag_soma_dist,
-        )
-
-        viterbrain.compute_all_costs_int()
-
-        print(f"# Edges: {viterbrain.nxGraph.number_of_edges()}")
-
-        with open(viterbrain_fname, "wb") as handle:
-            pickle.dump(viterbrain, handle)
-
-        self.viterbrain = viterbrain
-
-    def compute_bfs(self) -> None:
-        """Compute bfs from highest degree node"""
-        nodes_sorted = sorted(
-            self.viterbrain.nxGraph.degree, key=lambda x: x[1], reverse=True
-        )
-
-        print(
-            f"bfs tree: {nx.bfs_tree(self.viterbrain.nxGraph, source=nodes_sorted[0][0])}"
-        )
+    return new_labels
```

### Comparing `brainlit-0.3.3/brainlit/algorithms/generate_fragments/tube_seg.py` & `brainlit-0.3.4/brainlit/algorithms/generate_fragments/tube_seg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import numpy as np
 from skimage import draw
 import itertools
-from scipy.ndimage.morphology import distance_transform_edt
-from typing import Optional, List, Tuple, Union
-from scipy.ndimage.morphology import distance_transform_edt
-from skimage import draw
+from typing import Iterable, Optional, List, Tuple, Union
+from scipy.ndimage import distance_transform_edt
 from brainlit.utils.util import check_type, check_size, check_iterable_type
 from tqdm import tqdm
+import cloudvolume
 
 
-def pairwise(iterable):
+def pairwise(iterable: Iterable):
     # Adapted from https://stackoverflow.com/a/5434936
     a, b = itertools.tee(iterable)
     next(b, None)
     return zip(a, b)
 
 
-def draw_sphere(shape, center, radius):
+def draw_sphere(shape: tuple, center: tuple, radius: float) -> np.ndarray:
     """
     Generate a sphere of a radius at a point.
 
     Adapted from https://stackoverflow.com/a/56060957
 
     Parameters
     -------
@@ -45,15 +44,20 @@
         + (coords[1] - center[1]) ** 2
         + (coords[2] - center[2]) ** 2
     )
     sphere = 1 * (distance <= radius)
     return sphere
 
 
-def draw_tube_from_spheres(img, vertex0, vertex1, radius):
+def draw_tube_from_spheres(
+    img: cloudvolume.volumecutout.VolumeCutout,
+    vertex0: tuple,
+    vertex1: tuple,
+    radius: float,
+) -> np.ndarray:
     """
     Generate a segmentation mask of a tube (series of spheres) connecting known vertices.
 
     Parameters
     -------
     img : cloudvolume.volumecutout.VolumeCutout
         The volume to segment.
@@ -80,15 +84,20 @@
         s = draw_sphere(img.shape, pt, radius)
         seg += s
 
     labels = np.where(seg >= 1, 1, 0)
     return labels
 
 
-def draw_tube_from_edt(img, vertex0, vertex1, radius):
+def draw_tube_from_edt(
+    img: cloudvolume.volumecutout.VolumeCutout,
+    vertex0: tuple,
+    vertex1: tuple,
+    radius: float,
+) -> np.ndarray:
     """
     Generate a segmentation mask of a tube connecting known vertices.
 
     Parameters
     -------
     img : cloudvolume.volumecutout.VolumeCutout
         The volume to segment.
@@ -112,15 +121,20 @@
     line_array = np.ones(img.shape, dtype=int)
     line_array[line] = 0
     seg = distance_transform_edt(line_array)
     labels = np.where(seg <= radius, 1, 0)
     return labels
 
 
-def tubes_seg(img, vertices, radius, spheres=False):
+def tubes_seg(
+    img: cloudvolume.volumecutout.VolumeCutout,
+    vertices: list,
+    radius: float,
+    spheres: bool = False,
+) -> np.ndarray:
     """
     Generate a segmentation mask of cylinders connecting known vertices.
 
     Parameters
     -------
     img : cloudvolume.volumecutout.VolumeCutout
         The volume to segment.
@@ -145,20 +159,19 @@
             output += draw_tube_from_spheres(img, a, b, radius)
         else:
             output += draw_tube_from_edt(img, a, b, radius)
     labels = np.where(output >= 1, 1, 0)
     return labels
 
 
-# TOMMY REVIEW
 def tubes_from_paths(
     size: Tuple[int, int, int],
     paths: List[List[int]],
     radius: Optional[Union[float, int]] = None,
-):
+) -> np.ndarray:
     """Constructs tubes from list of paths.
     Returns densely labeled paths within the shape of the image.
 
     Arguments:
         size: The size of image to consider.
         paths: The list of paths. Each path is a list of points along the path (non-dense).
         radius: The radius of the line to draw. Default is None = 1 pixel wide line.
@@ -187,18 +200,15 @@
             line = draw.line_nd(path[i], path[i + 1])
             line = _within_img(line, size)
             if len(line) > 0:
                 coords[0] = np.concatenate((coords[0], line[0]))
                 coords[1] = np.concatenate((coords[1], line[1]))
                 coords[2] = np.concatenate((coords[2], line[2]))
 
-    try:
-        coords = (coords[0].astype(int), coords[1].astype(int), coords[2].astype(int))
-    except AttributeError:  # if a list was passed
-        coords = (coords[0], coords[1], coords[2])
+    coords = (coords[0].astype(int), coords[1].astype(int), coords[2].astype(int))
 
     if radius is not None:
         line_array = np.ones(size, dtype=int)
         line_array[coords] = 0
         seg = distance_transform_edt(line_array)
         labels = np.where(seg <= radius, 1, 0)
     else:
```

### Comparing `brainlit-0.3.3/brainlit/algorithms/trace_analysis/fit_spline.py` & `brainlit-0.3.4/brainlit/algorithms/trace_analysis/fit_spline.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,94 @@
+from typing import Tuple
 import numpy as np
-from scipy.interpolate import splprep
+from scipy.interpolate import splprep, splev, BSpline, CubicHermiteSpline, PPoly
+from scipy.interpolate._cubic import prepare_input
+import pandas as pd
 import math
 import warnings
 import networkx as nx
 import itertools
 from brainlit.utils.util import (
     check_type,
     check_size,
     check_precomputed,
     check_iterable_type,
     check_iterable_nonnegative,
 )
+from typing import Union, List
+
+
+def compute_parameterization(positions: np.array) -> np.array:
+    """Computes list of parameter values to be used for a list of positions using piecewise linear arclength.
+
+    Parameters
+    ----------
+    positions : np.array
+        nxd array containing coordinates of the n points in d dimentional space.
+    Returns
+    -------
+    TotalDist : np.array
+        n array containing parameter values, first element is 0.
+    """
+    NodeDist = np.linalg.norm(np.diff(positions, axis=0), axis=1)
+    TotalDist = np.concatenate(([0], np.cumsum(NodeDist)))
+    return TotalDist
+
+
+class CubicHermiteChain(PPoly):
+    """A third order spline class (continuous piecewise cubic representation), that is fit to a set of positions and one-sided derivatives. This is not a standard spline class (e.g. b-splines), because the derivatives are not necessarily continuous at the knots.
+
+    A subclass of PPoly, a piecewise polynomial class from scipy.
+    """
+
+    def __init__(
+        self,
+        x: np.array,
+        y: np.array,
+        left_dydx: np.array,
+        right_dydx: np.array,
+        extrapolate=None,
+    ):
+        """Initialize object via:
+
+        Parameters
+        ----------
+        x : np.array
+            Independent variable, shape n.
+        y : np.array
+            Dependent variable, shape n x d.
+        left_dydx : np.array
+            Derivatives on left sides of cubic segments (i.e. right hand derivatives of knots), shape n-1 x d.
+        right_dy_dx : np.array
+            Derivatives on right sides of cubic segments (i.e. left hand derivatives of knots), shape n-1 x d.
+        extrapolate : np.array
+            If bool, determines whether to extrapolate to out-of-bounds points based on first and last intervals, or to return NaNs. If ‘periodic’, periodic extrapolation is used. Default is True.
+        """
+        if extrapolate is None:
+            extrapolate = True
+
+        x, dx, y, axis, _ = prepare_input(x, y, axis=0)
+
+        if not np.array_equal(left_dydx.shape, right_dydx.shape):
+            raise ValueError(
+                f"Left derivatives shape {left_dydx.shape} must be equal to right derivatives shape {right_dydx.shape}"
+            )
+
+        dxr = dx.reshape([dx.shape[0]] + [1] * (y.ndim - 1))
+        slope = np.diff(y, axis=0) / dxr
+        t = (left_dydx + right_dydx - 2 * slope) / dxr
+
+        c = np.empty((4, len(x) - 1) + y.shape[1:], dtype=t.dtype)
+        c[0] = t / dxr
+        c[1] = (slope - left_dydx) / dxr - t
+        c[2] = left_dydx
+        c[3] = y[:-1]
+
+        super().__init__(c, x, extrapolate=extrapolate)
+        self.axis = axis
 
 
 """
 Geometric Graph class
 """
 
 
@@ -22,23 +96,25 @@
     r"""The shape of the neurons are expressed and fitted with splines in this undirected graph class.
 
     The geometry of the neurons are projected on undirected graphs, based on which the trees of neurons consisted for splines is constructed.
     It is required that each node has a loc attribute identifying that points location in space, and the location should be defined in 3-dimensional cartesian coordinates.
     It extends `nx.Graph` and rejects duplicate node input.
     """
 
-    def __init__(self, df=None):
+    def __init__(self, df: pd.DataFrame = None, root=1) -> None:
         super(GeometricGraph, self).__init__()
         self.segments = None
         self.cycle = None
-        self.root = 1
+        self.root = root
+        self.spline_type = None
+        self.spline_tree = None
         if df is not None:
             self.__init_from_df(df)
 
-    def __init_from_df(self, df_neuron):
+    def __init_from_df(self, df_neuron: pd.DataFrame) -> "GeometricGraph":
         """Converts dataframe of swc in voxel coordinates into a GeometricGraph
 
         Parameters
         ----------
         df_neuron : :class:`pandas.DataFrame`
             Indicies, coordinates, and parents of each node in the swc.
         Returns
@@ -70,17 +146,22 @@
 
             # add edges
             child = id
             parent = int(row["parent"])
             if parent > min(df_neuron["parent"]):
                 self.add_edge(parent, child)
 
-    def fit_spline_tree_invariant(self):
+    def fit_spline_tree_invariant(
+        self, spline_type: Union[BSpline, CubicHermiteSpline] = BSpline, k=3
+    ):
         r"""Construct a spline tree based on the path lengths.
 
+        Arguments:
+            spline_type: BSpline or CubicHermiteSpline, spline type that will be fit to the data. BSplines are typically used to fit position data only, and CubicHermiteSplines can only be used if derivative, and independent variable information is also known.
+
         Raises:
             ValueError: check if every node is unigue in location
             ValueError: check if every node is assigned to at least one edge
             ValueError: check if the graph contains undirected cycle(s)
             ValueErorr: check if the graph has disconnected segment(s)
 
         Returns:
@@ -114,14 +195,15 @@
         # check there are no undirected cycles in the graph
         if not nx.algorithms.tree.recognition.is_forest(self):
             raise ValueError("the graph contains undirected cycles")
         # check there are no disconnected segments
         if not nx.algorithms.tree.recognition.is_tree(self):
             raise ValueError("the graph contains disconnected segments")
 
+        # Identify paths
         spline_tree = nx.DiGraph()
         curr_spline_num = 0
         stack = []
         root = self.root
         tree = nx.algorithms.traversal.depth_first_search.dfs_tree(self, source=root)
         main_branch, collateral_branches = self.__find_main_branch(tree)
         spline_tree.add_node(curr_spline_num, path=main_branch, starting_length=0)
@@ -144,28 +226,41 @@
                 curr_spline_num, path=main_branch, starting_length=tree[2]
             )
             spline_tree.add_edge(parent_num, curr_spline_num)
 
             for tree in collateral_branches:
                 stack.append((tree, curr_spline_num))
 
+        # Fit splines
+        self.spline_type = spline_type
+
         for node in spline_tree.nodes:
             main_branch = spline_tree.nodes[node]["path"]
 
-            spline_tree.nodes[node]["spline"] = self.__fit_spline_path(main_branch)
+            if spline_type == BSpline:  # each node must have "loc" attribute
+                spline_tree.nodes[node]["spline"] = self.__fit_bspline_path(
+                    main_branch, k=k
+                )
+            elif (
+                spline_type == CubicHermiteSpline
+            ):  # each node must have "u," "loc," and "deriv" attributes
+                spline_tree.nodes[node]["spline"] = self.__fit_chspline_path(
+                    main_branch
+                )
 
+        self.spline_tree = spline_tree
         return spline_tree
 
-    def __fit_spline_path(self, path):
+    def __fit_bspline_path(self, path, k):
         r"""Fit a B-Spline to a path.
 
         Compute the knots, coefficients, and the degree of the
         B-Spline fitting the path
 
-        Argumets:
+        Arguments:
             path: list, a list of nodes.
 
         Raises:
             ValueError: Nodes should be defined under loc attribute
             TypeError: loc should be of numpy.ndarray class
             ValueError: loc should be 3-dimensional
 
@@ -175,24 +270,47 @@
         """
 
         x = np.zeros((len(path), 3))
 
         for row, node in enumerate(path):
             x[row, :] = self.nodes[node]["loc"]
         path_length = x.shape[0]
-        NodeDist = np.linalg.norm(np.diff(x, axis=0), axis=1)
-        TotalDist = np.concatenate(([0], np.cumsum(NodeDist)))
-        if path_length != 5:
-            k = np.amin([path_length - 1, 5])
-        else:
-            k = 3
+        TotalDist = compute_parameterization(x)
+        # old
+        # if path_length != 5:
+        #     k = np.amin([path_length - 1, 5])
+        # else:
+        #     k = 3
+        k = np.amin([k, path_length - 1])  # change
         tck, u = splprep([x[:, 0], x[:, 1], x[:, 2]], s=0, u=TotalDist, k=k)
 
         return tck, u
 
+    def __fit_chspline_path(self, path: List):
+        """Fit cubic hermite spline to path of nodes that has independent variable (u), position (loc) and derivative (deriv) attributes.
+
+        Args:
+            path (List): sequence of nodes to which the spline will be fit.
+
+        Returns:
+            CubicHermiteSpline: spline that fits the nodes in path.
+        """
+        x = np.zeros((len(path)))
+        y = np.zeros((len(path), 3))
+        dy = np.zeros((len(path), 3))
+
+        for row, node in enumerate(path):
+            x[row] = self.nodes[node]["u"]
+            y[row, :] = self.nodes[node]["loc"]
+            dy[row, :] = self.nodes[node]["deriv"]
+
+        chspline = CubicHermiteSpline(x, y, dy)
+
+        return chspline
+
     def __find_main_branch(self, tree: nx.DiGraph, starting_length: float = 0):
         r"""Find the main branch in a directed graph.
 
         It is used in `fit_spline_tree_invariant` to identify the main branch
         in a neuron and group the collateral branches for later analysis.
         The main branch is defined as the longest possible path connecting the
         neuron's nodes, in terms of spatial distance. An example is provided in
@@ -281,15 +399,15 @@
                                 ),
                                 node,
                                 starting_length,
                             )
                         )
         return list(main_branch), collateral_branches
 
-    def __path_length(self, path):
+    def __path_length(self, path: list) -> float:
         r"""Compute the length of a path.
 
         Given a path ::math::`p = (r_1, \dots, r_N)`, where
         ::math::`r_k = [x_k, y_k, z_k], k = 1, \dots, N`, the length
         `l` of a path is computed as the sum of the lengths of the
         edges of the path. We can write:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `brainlit-0.3.3/brainlit/algorithms/trace_analysis/spline_fxns.py` & `brainlit-0.3.4/brainlit/algorithms/trace_analysis/spline_fxns.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.3/brainlit/feature_extraction/neighborhood.py` & `brainlit-0.3.4/brainlit/feature_extraction/neighborhood.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.3/brainlit/preprocessing/preprocess.py` & `brainlit-0.3.4/brainlit/preprocessing/preprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from typing import Tuple
 import numpy as np
 import scipy.linalg as linalg
 
 
-def center(data):
+def center(data: np.ndarray) -> np.ndarray:
     """Centers data by subtracting the mean
 
     Parameters
     ----------
     data : array-like
         data to be centered
 
@@ -16,15 +17,15 @@
         centered-data
 
     """
     data_centered = data - np.mean(data)
     return data_centered
 
 
-def contrast_normalize(data, centered=False):
+def contrast_normalize(data: np.ndarray, centered: bool = False) -> np.ndarray:
     """Normalizes image data to have variance of 1
 
     Parameters
     ----------
     data : array-like
         data to be normalized
 
@@ -39,15 +40,22 @@
     """
     if not centered:
         data = center(data)
     data = np.divide(data, np.sqrt(np.var(data)))
     return data
 
 
-def whiten(img, window_size, step_size, centered=False, epsilon=1e-5, type="PCA"):
+def whiten(
+    img: np.ndarray,
+    window_size: np.ndarray,
+    step_size: np.ndarray,
+    centered: bool = False,
+    epsilon: float = 1e-5,
+    type: str = "PCA",
+) -> Tuple[np.ndarray, np.ndarray]:
     """Performs PCA or ZCA whitening on an array. This preprocessing step is described
     in _[1].
 
     Parameters
     ----------
     img : array-like
         image to be vectorized
@@ -110,15 +118,17 @@
 
     data_whitened = imagize_vector(whitened, data_padded.shape, window_size, step_size)
     data_whitened = undo_pad(data_whitened, pad_size)
 
     return data_whitened, S
 
 
-def window_pad(img, window_size, step_size):
+def window_pad(
+    img: np.ndarray, window_size: np.ndarray, step_size: np.ndarray
+) -> Tuple[np.ndarray, np.ndarray]:
     """Pad image at edges so the window can convolve evenly.
     Padding will be a copy of the edges.
 
     Parameters
     ----------
     img : array-like
         image to be padded
@@ -161,15 +171,15 @@
     pad_width = [pad_size[dim, :].astype(int).tolist() for dim in range(d)]
 
     img_padded = np.pad(img, pad_width, mode="edge")
     # Why does the padding add so much to the edge?
     return img_padded, pad_size
 
 
-def undo_pad(img, pad_size):
+def undo_pad(img: np.ndarray, pad_size: np.ndarray) -> np.ndarray:
     """Remove padding from edges of images
 
     Parameters
     ----------
     img : array-like
         padded image
 
@@ -193,15 +203,17 @@
     coords = list(zip(start, end))
     slices = tuple(slice(coord[0], coord[1]) for coord in coords)
     img = img[slices]
 
     return img
 
 
-def vectorize_img(img, window_size, step_size):
+def vectorize_img(
+    img: np.ndarray, window_size: np.ndarray, step_size: np.ndarray
+) -> np.ndarray:
     """Reshapes an image by vectorizing different neighborhoods of the image.
 
     Parameters
     ----------
     img : array-like
         image to be vectorized
 
@@ -240,15 +252,17 @@
         coords = list(zip(start, end))
         slices = tuple(slice(coord[0], coord[1]) for coord in coords)
         vectorized[:, step_num] = img[slices].flatten()
 
     return vectorized
 
 
-def imagize_vector(img, orig_shape, window_size, step_size):
+def imagize_vector(
+    img: np.ndarray, orig_shape: tuple, window_size: np.ndarray, step_size: np.ndarray
+) -> np.ndarray:
     """Reshapes a vectorized image back to its original shape.
 
     Parameters
     ----------
     img : array-like
         vectorized image
```

### Comparing `brainlit-0.3.3/brainlit/utils/Neuron_trace.py` & `brainlit-0.3.4/brainlit/utils/Neuron_trace.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from curses import intrflush
+from typing import List, Optional, Tuple, Union
 import numpy as np
 import re
 import pandas as pd
 import networkx as nx
 from cloudvolume import CloudVolume, Skeleton
 from io import StringIO
 import os
@@ -58,21 +60,21 @@
     >>> swc_trace = NeuronTrace(swc_path)
     >>> s3_trace = NeuronTrace(s3_path,seg_id,mip)
 
     """
 
     def __init__(
         self,
-        path,
-        seg_id=None,
-        mip=None,
-        rounding=True,
-        read_offset=False,
-        fill_missing=True,
-        use_https=False,
+        path: str,
+        seg_id: int = None,
+        mip: int = None,
+        rounding: bool = True,
+        read_offset: bool = False,
+        fill_missing: bool = True,
+        use_https: bool = False,
     ):
         self.path = path
         self.input_type = None
         self.df = None
         self.args = []
         self.seg_id = seg_id
         self.mip = mip
@@ -124,30 +126,30 @@
 
         elif self.input_type == "skel":
             df = self._read_s3(path, seg_id, mip, rounding)
             (self.path, seg_id, mip)
             self.df = df
 
     # public methods
-    def get_df_arguments(self):
+    def get_df_arguments(self) -> list:
         """Gets arguments for df - offset, color, cc, branch
 
         Returns
         -------
             self.args : list
                 list of arguments for df, if found - offset, color, cc, branch
 
         Example
         -------
         >>> swc_trace.get_df_arguments()
         >>> [[73954.8686, 17489.532566, 34340.365689], [1.0, 1.0, 1.0], nan, nan]
         """
         return self.args
 
-    def get_df(self):
+    def get_df(self) -> pd.DataFrame:
         """Gets the dataframe providing indices, coordinates, and parents of each node
 
         Returns
         -------
             self.df : :class:`pandas.DataFrame`
                 dataframe providing indices, coordinates, and parents of each node
 
@@ -166,15 +168,17 @@
             150    151    0    46.897125    14.686010    -7.159252    1.0    150
             151    152    0    47.494643    15.294842    -7.159252    1.0    151
             152    153    6    48.092162    15.294842    -7.159252    1.0    152
             53 rows × 7 columns
         """
         return self.df
 
-    def get_skel(self, benchmarking=False, origin=None):
+    def get_skel(
+        self, benchmarking: bool = False, origin: np.ndarray = None
+    ) -> Skeleton:
         """Gets a skeleton version of dataframe, if swc input is provided
 
         Arguments
         ----------
             origin : None, numpy array with shape (3,1) (default = None)
                 origin of coordinate frame in microns, (default: None assumes (0,0,0) origin)
             benchmarking : bool
@@ -203,15 +207,17 @@
                 mip=self.mip,
                 fill_missing=self.fill_missing,
                 use_https=self.use_https,
             )
             skel = cv.skeleton.get(self.seg_id)
             return skel
 
-    def get_df_voxel(self, spacing, origin=np.array([0, 0, 0])):
+    def get_df_voxel(
+        self, spacing: np.array, origin: np.array = np.array([0, 0, 0])
+    ) -> pd.DataFrame:
         """Converts coordinates in pd.DataFrame from spatial units to voxel units
 
         Arguments
         ----------
         spacing : :class:`numpy.array`
             Conversion factor (spatial units/voxel). Assumed to be np.array([x,y,z])
         origin : :class:`numpy.array`
@@ -246,15 +252,17 @@
         check_size(spacing)
         check_type(origin, np.ndarray)
         check_size(origin)
 
         df_voxel = self._df_in_voxel(self.df, spacing, origin)
         return df_voxel
 
-    def get_graph(self, spacing=None, origin=None):
+    def get_graph(
+        self, spacing: np.array = None, origin: np.array = None
+    ) -> nx.classes.digraph.DiGraph:
         """Converts dataframe in either spatial or voxel coordinates into a directed graph.
         Will convert to voxel coordinates if spacing is specified.
 
         Arguments
         ----------
         spacing : None, :class:`numpy.array` (default = None)
             Conversion factor (spatial units/voxel). Assumed to be np.array([x,y,z]).
@@ -291,15 +299,17 @@
             G = self._df_to_graph(df_voxel)
 
         # no voxel conversion option
         else:
             G = self._df_to_graph(self.df)
         return G
 
-    def get_paths(self, spacing=None, origin=None):
+    def get_paths(
+        self, spacing: np.array = None, origin: np.array = None
+    ) -> List[np.array]:
         """Converts dataframe in either spatial or voxel coordinates into a list of paths.
         Will convert to voxel coordinates if spacing is specified.
 
         Arguments
         ----------
         spacing : None, :class:`numpy.array` (default = None)
             Conversion factor (spatial units/voxel). Assumed to be np.array([x,y,z]).
@@ -348,16 +358,19 @@
             G = self._df_to_graph(self.df)
 
         paths = self._graph_to_paths(G)
 
         return paths
 
     def generate_df_subset(
-        self, vox_in_img_list, subneuron_start=None, subneuron_end=None
-    ):
+        self,
+        vox_in_img_list: list,
+        subneuron_start: int = None,
+        subneuron_end: int = None,
+    ) -> pd.DataFrame:
         """Read a new subset dataframe in coordinates in img spacing.
         Specify specific range of vertices from dataframe if desired
 
         Arguments
         ----------
         vox_in_img_list : list
             List of voxels
@@ -413,15 +426,22 @@
             subneuron_df = self.df[subneuron_start:subneuron_end]
             df = subneuron_df
 
         df_new = self._generate_df_subset(df, vox_in_img_list)
 
         return df_new
 
-    def get_bfs_subgraph(self, node_id, depth, df=None, spacing=None, origin=None):
+    def get_bfs_subgraph(
+        self,
+        node_id: int,
+        depth: int,
+        df: pd.DataFrame = None,
+        spacing: np.array = None,
+        origin: np.array = None,
+    ) -> Tuple[nx.classes.digraph.DiGraph, nx.classes.digraph.DiGraph, List[np.array]]:
         """
          Creates a spanning subgraph from a seed node and parent graph using BFS.
 
         Arguments
          ----------
          node_id : int
              The id of the node to use as a seed.
@@ -489,15 +509,20 @@
 
         G_sub, tree = self._get_bfs_subgraph(G, node_id, depth, df)
 
         paths = self._graph_to_paths(G_sub)
 
         return G_sub, tree, paths
 
-    def get_sub_neuron(self, bounding_box, spacing=None, origin=None):
+    def get_sub_neuron(
+        self,
+        bounding_box: Union[tuple, list, None],
+        spacing: np.array = None,
+        origin: np.array = None,
+    ) -> nx.classes.digraph.DiGraph:
         """Returns sub-neuron with node coordinates bounded by start and end
 
         Arguments
         ----------
         bounding_box : tuple or list or None
             Defines a bounding box around a sub-region around the neuron. Length 2
             tuple/list. First element is the coordinate of one corner (inclusive)
@@ -550,15 +575,20 @@
         else:
             G = self._df_to_graph(self.df)
 
         G_sub = self._get_sub_neuron(G, bounding_box)
 
         return G_sub
 
-    def get_sub_neuron_paths(self, bounding_box, spacing=None, origin=None):
+    def get_sub_neuron_paths(
+        self,
+        bounding_box: Union[tuple, list, None],
+        spacing: np.array = None,
+        origin: np.array = None,
+    ) -> List[np.array]:
         """Returns sub-neuron with node coordinates bounded by start and end
 
         Arguments
         ----------
         bounding_box : tuple or list or None
             Defines a bounding box around a sub-region around the neuron. Length 2
             tuple/list. First element is the coordinate of one corner (inclusive)
@@ -609,21 +639,20 @@
             G = self._df_to_graph(df_voxel)
 
         # no voxel conversion option
         else:
             G = self._df_to_graph(self.df)
 
         G_sub = self._get_sub_neuron(G, bounding_box)
-
-        paths = self._graph_to_paths(G_sub)
+        paths = self._graph_to_paths(G_sub, round=True)
 
         return paths
 
     @staticmethod
-    def ssd(pts1, pts2):
+    def ssd(pts1: np.array, pts2: np.array) -> float:
         """Compute significant spatial distance metric between two traces as defined in APP1.
         Args:
             pts1 (np.array): array containing coordinates of points of trace 1. shape: npoints x ndims
             pts2 (np.array): array containing coordinates of points of trace 1. shape: npoints x ndims
         Returns:
             [float]: significant spatial distance as defined by APP1
 
@@ -651,15 +680,17 @@
         else:
             dists = np.concatenate([dists1, dists2])
             ssd = np.mean(dists)
 
         return ssd
 
     # private methods
-    def _read_swc(self, path):
+    def _read_swc(
+        self, path: str
+    ) -> Tuple[pd.DataFrame, List[float], List[int], int, int]:
         """
         Read a single swc file
 
         Arguments:
             path {string} -- path to file
             raw {bool} -- whether you are passing the file directly
 
@@ -714,23 +745,25 @@
             path,
             names=["sample", "structure", "x", "y", "z", "r", "parent"],
             skiprows=header_length,
             delimiter="\s+",
         )
         return df, offset, color, cc, branch
 
-    def _read_swc_offset(self, path):
+    def _read_swc_offset(self, path: str) -> Tuple[pd.DataFrame, List[int], int, int]:
         df, offset, color, cc, branch = self._read_swc(path)
         df["x"] = df["x"] + offset[0]
         df["y"] = df["y"] + offset[1]
         df["z"] = df["z"] + offset[2]
 
         return df, color, cc, branch
 
-    def _read_s3(self, s3_path, seg_id, mip, rounding=True):
+    def _read_s3(
+        self, s3_path: str, seg_id: int, mip: int, rounding: Optional[bool] = True
+    ):
         """Read a s3 bucket path to a skeleton object
         into a pandas dataframe.
 
         Parameters
         ----------
         s3_path : str
             String representing the path to the s3 bucket
@@ -804,15 +837,20 @@
             vox_in_img_list[:][0],
             vox_in_img_list[:][1],
             vox_in_img_list[:][2],
         )
 
         return df_new
 
-    def _space_to_voxel(self, spatial_coord, spacing, origin=np.array([0, 0, 0])):
+    def _space_to_voxel(
+        self,
+        spatial_coord: np.array,
+        spacing: np.array,
+        origin: np.array = np.array([0, 0, 0]),
+    ) -> np.array:
         """Converts coordinate from spatial units to voxel units.
 
         Parameters
         ----------
         spatial_coord : :class:`numpy.array`
             3D coordinate in spatial units. Assumed to be np.array[(x,y,z)]
         spacing : :class:`numpy.array`
@@ -821,20 +859,27 @@
             Origin of the spatial coordinate. Default is (0,0,0). Assumed to be
             np.array([x,y,z])
         Returns
         -------
         voxel_coord : :class:`numpy.array`
             Coordinate in voxel units. Assumed to be np.array([x,y,z])
         """
+        if np.any(spacing == 0):
+            raise ValueError(f"Zero detected in spacing: {spacing}")
 
         voxel_coord = np.round(np.divide(spatial_coord - origin, spacing))
         voxel_coord = voxel_coord.astype(np.int64)
         return voxel_coord
 
-    def _df_in_voxel(self, df, spacing, origin=np.array([0, 0, 0])):
+    def _df_in_voxel(
+        self,
+        df: pd.DataFrame,
+        spacing: np.array,
+        origin: np.array = np.array([0, 0, 0]),
+    ) -> pd.DataFrame:
         """Converts coordinates in pd.DataFrame representing swc from spatial units
         to voxel units
 
         Parameters
         ----------
         df : :class:`pandas.DataFrame`
             Indicies, coordinates, and parents of each node in the swc. Coordinates
@@ -862,50 +907,66 @@
 
         df_voxel["x"] = x
         df_voxel["y"] = y
         df_voxel["z"] = z
 
         return df_voxel
 
-    def _df_to_graph(self, df_voxel):
-        """Converts dataframe of swc in voxel coordinates into a directed graph
+    def _df_to_graph(self, df, round=False):
+        """Converts dataframe form of neuron trace into a directed graph
 
         Parameters
         ----------
         df_voxel : :class:`pandas.DataFrame`
-            Indicies, coordinates, and parents of each node in the swc. Coordinates
-            are in voxel units.
+            Indices, coordinates, and parents of each node in the swc.
+        round : boolean
+            Whether coordinates/distances should be rounded to integers.
+
         Returns
         -------
         G : :class:`networkx.classes.digraph.DiGraph`
             Neuron from swc represented as directed graph. Coordinates x,y,z are
             node attributes accessed by keys 'x','y','z' respectively.
         """
         G = nx.DiGraph()
 
         # add nodes
-        for index, row in df_voxel.iterrows():
+        for index, row in df.iterrows():
             id = int(row["sample"])
 
+            coord = [row["x"], row["y"], row["z"]]
+            if round:
+                coord = [int(c) for c in coord]
+
             G.add_node(id)
-            G.nodes[id]["x"] = int(row["x"])
-            G.nodes[id]["y"] = int(row["y"])
-            G.nodes[id]["z"] = int(row["z"])
+            G.nodes[id]["x"] = coord[0]
+            G.nodes[id]["y"] = coord[1]
+            G.nodes[id]["z"] = coord[2]
 
         # add edges
-        for index, row in df_voxel.iterrows():
+        for index, row in df.iterrows():
             child = int(row["sample"])
+            child_coord = [row["x"], row["y"], row["z"]]
             parent = int(row["parent"])
 
-            if parent > min(df_voxel["parent"]):
-                G.add_edge(parent, child)
+            if parent > min(df["parent"]):
+                parent_row = df[df["sample"] == parent]
+                parent_coord = [parent_row["x"], parent_row["y"], parent_row["z"]]
+
+                dist = np.linalg.norm(np.subtract(child_coord, parent_coord))
+                if round:
+                    dist = int(dist)
+
+                G.add_edge(parent, child, distance=dist)
 
         return G
 
-    def _get_sub_neuron(self, G, bounding_box):
+    def _get_sub_neuron(
+        self, G: nx.classes.digraph.DiGraph, bounding_box: Union[tuple, list, None]
+    ) -> nx.classes.digraph.DiGraph:
         """Returns sub-neuron with node coordinates bounded by start and end
 
         Parameters
         ----------
         G : :class:`networkx.classes.digraph.DiGraph`
             Neuron from swc represented as directed graph. Coordinates x,y,z are
             node attributes accessed by keys 'x','y','z' respectively.
@@ -944,15 +1005,15 @@
         for id in list(G_sub.nodes):
             G_sub.nodes[id]["x"] = G_sub.nodes[id]["x"] - start[0]
             G_sub.nodes[id]["y"] = G_sub.nodes[id]["y"] - start[1]
             G_sub.nodes[id]["z"] = G_sub.nodes[id]["z"] - start[2]
 
         return G_sub
 
-    def _graph_to_paths(self, G):
+    def _graph_to_paths(self, G, round=False):
         """Converts neuron represented as a directed graph with no cycles into a
         list of paths.
 
         Parameters
         ----------
         G : :class:`networkx.classes.digraph.DiGraph`
             Neuron from swc represented as directed graph. Coordinates x,y,z are
@@ -964,38 +1025,51 @@
             units. Each array is one path.
         """
         G_cp = G.copy()  # make copy of input G
         branches = []
         while len(G_cp.edges) != 0:  # iterate over branches
             # get longest branch
             longest = nx.algorithms.dag.dag_longest_path(
-                G_cp
+                G_cp, weight="distance"
             )  # list of nodes on the path
             branches.append(longest)
 
             # remove longest branch
             for idx, e in enumerate(longest):
                 if idx < len(longest) - 1:
                     G_cp.remove_edge(longest[idx], longest[idx + 1])
 
         # convert branches into list of paths
         paths = []
         for branch in branches:
             # get vertices in branch as n by 3 numpy.array; n = length of branches
-            path = np.zeros((len(branch), 3), dtype=np.int64)
+            if round:
+                dtype = "int"
+            else:
+                dtype = "float"
+
+            path = np.zeros((len(branch), 3), dtype=dtype)
             for idx, node in enumerate(branch):
-                path[idx, 0] = np.int64(G_cp.nodes[node]["x"])
-                path[idx, 1] = np.int64(G_cp.nodes[node]["y"])
-                path[idx, 2] = np.int64(G_cp.nodes[node]["z"])
+                coord = [G_cp.nodes[node][c] for c in ["x", "y", "z"]]
+                if round:
+                    coord = [np.int64(c) for c in coord]
+
+                path[idx, :] = coord
 
             paths.append(path)
 
-        return np.array(paths, dtype="object")
+        return paths
 
-    def _get_bfs_subgraph(self, G, node_id, depth, df=None):
+    def _get_bfs_subgraph(
+        self,
+        G: nx.classes.digraph.DiGraph,
+        node_id: int,
+        depth: int,
+        df: pd.DataFrame = None,
+    ) -> Tuple[nx.classes.digraph.DiGraph, nx.classes.digraph.DiGraph]:
         """
         Creates a spanning subgraph from a seed node and parent graph using BFS.
 
         Parameters
         ----------
         G : :class:`networkx.classes.digraph.DiGraph`
             Neuron from swc represented as directed graph.
@@ -1022,15 +1096,17 @@
         if df is not None:
             node_id = int(df.iloc[node_id]["sample"])
         G_undir = G.to_undirected()
         tree = nx.bfs_tree(G_undir, node_id, depth_limit=depth)  # forward BFS
         G_sub = nx.subgraph(G, list(tree.nodes))
         return G_sub, tree
 
-    def _swc2skeleton(self, swc_file, benchmarking=False, origin=None):
+    def _swc2skeleton(
+        self, swc_file: str, benchmarking: bool = False, origin: np.array = None
+    ) -> Skeleton:
         """Converts swc file into Skeleton object
         Arguments:
             swc_file {str} -- path to SWC file
         Keyword Arguments:
             origin {numpy array with shape (3,1)} -- origin of coordinate frame in microns, (default: None assumes (0,0,0) origin)
         Returns:
             skel {cloudvolume.Skeleton} -- Skeleton object of given SWC file
```

### Comparing `brainlit-0.3.3/brainlit/utils/benchmarking_params.py` & `brainlit-0.3.4/brainlit/utils/benchmarking_params.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.3/brainlit/utils/session.py` & `brainlit-0.3.4/brainlit/utils/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # Reference: https://github.com/neurodata/mouselight_code/blob/region_growing/src/ngl_pipeline.py
 
 import numpy as np
-import matplotlib.pyplot as plt
-import SimpleITK as sitk
-from cloudvolume import CloudVolume, view
+from cloudvolume import CloudVolume
 from cloudvolume.lib import Bbox
 from cloudvolume.exceptions import InfoUnavailableError
 from brainlit.utils import Neuron_trace
 from brainlit.algorithms.generate_fragments import tube_seg
-import napari
 import warnings
 import networkx as nx
 from typing import Optional, List, Union, Tuple
 from brainlit.utils.util import (
     check_type,
-    check_size,
     check_precomputed,
     check_iterable_type,
     check_iterable_nonnegative,
 )
-from collections import Iterable
+from collections.abc import Iterable
 
 Bounds = Union[Bbox, Tuple[int, int, int, int, int, int]]
 
 
 class NeuroglancerSession:
     """Utility class which pulls and pushes data.
 
@@ -106,15 +102,14 @@
         check_type(seg_id, (int, np.integer))
         check_type(v_id, (int, np.integer))
         if self.cv_segments is None:
             raise ValueError("Cannot get voxel without segmentation data")
         seg = self.cv_segments.skeleton.get(seg_id).vertices
         if v_id < 0 or v_id >= len(seg):
             raise ValueError(f"{v_id} should be between 0 and {len(seg)}.")
-
         vertex = seg[v_id]
         voxel = np.round(
             np.divide(vertex, self.cv_segments.scales[self.mip]["resolution"])
         ).astype(int)
         return voxel
 
     def set_url_segments(self, seg_url: str):
@@ -145,15 +140,14 @@
             seg_id  The segement to pull.
             bbox: The bounding box object, default None. If None, uses entire volume.
             rounding: Optional, default True. Whether you want S3 file to be rounded or not.
 
         Returns:
             G: A networkx subgraph from the specified segment and bounding box.
         """
-
         check_type(seg_id, (int, np.integer))
         check_type(rounding, bool)
         if self.cv_segments is None:
             raise ValueError("Cannot get segments without segmentation data.")
         s3_trace = Neuron_trace.NeuronTrace(
             self.url_segments, seg_id, self.mip, rounding, use_https=self.use_https
         )
@@ -189,15 +183,15 @@
         Returns:
             labels: A volume within the bounding box, with 1 on tubes and 0 elsewhere.
         """
         if self.cv_segments is None:
             raise ValueError("Cannot get segments without segmentation data.")
         check_type(seg_id, int)
         if radius is not None:
-            check_type(radius, (int, np.integer, float, np.float))
+            check_type(radius, (int, np.integer, float, np.double))
             if radius <= 0:
                 raise ValueError("Radius must be positive.")
 
         # s3_trace = NeuronTrace(self.url_segments,seg_id,self.mip,rounding)
         # paths = s3_trace.get_paths(bbox)
         G_paths = self.get_segments(seg_id, bbox)
         paths = G_paths[1]
@@ -310,25 +304,25 @@
         check_type(seg_id, (int, np.integer))
         check_type(v_id, (int, np.integer))
         check_type(radius, (int, np.integer))
         if radius < 0:
             raise ValueError(f"Radius of {radius} should be nonnegative.")
 
         voxel = self._get_voxel(seg_id, v_id)
-        bounds = Bbox(voxel, voxel).expand_to_chunk_size(self.chunk_size)
+        bounds = Bbox(voxel, voxel + 1).expand_to_chunk_size(self.chunk_size)
         seed = bounds.to_list()
         shape = [
             self.chunk_size[0] * radius,
             self.chunk_size[1] * radius,
             self.chunk_size[2] * radius,
         ]
         bounds = Bbox(np.subtract(seed[:3], shape), np.add(seed[3:], shape))
         img = self.pull_bounds_img(bounds)
         vox_in_img = voxel - np.array(bounds.to_list()[:3])
-        return np.squeeze(np.array(img)), bounds, vox_in_img
+        return img, bounds, vox_in_img
 
     def pull_bounds_img(self, bounds: Bounds) -> np.ndarray:
         """Pull a volume around a specified bounding box. Works on image channels.
 
         Arguments:
             bounds: Bounding box, or tuple containing (x0, y0, z0, x1, y1, z1) bounds.
 
@@ -337,15 +331,21 @@
         """
 
         if isinstance(bounds, Bbox):
             bounds = bounds.to_list()
         check_iterable_type(bounds, (int, np.integer))
         check_iterable_nonnegative(bounds)
         img = self.cv.download(Bbox(bounds[:3], bounds[3:]), mip=self.mip)
-        return np.squeeze(np.array(img))
+        img = np.squeeze(np.array(img))
+        if len(img.shape) < 3:  # in case a dimension with size 1 got squeezed away
+            sz = np.subtract(bounds[3:], bounds[:3])
+            for i, s in enumerate(sz):
+                if s == 1:
+                    img = np.expand_dims(img, axis=i)
+        return img
 
     def pull_bounds_seg(self, bounds: Bounds) -> np.ndarray:
         """Pull a volume around a specified bounding box.
         Works on annotation channels.
 
         Arguments:
             bounds: Bounding box, or tuple containing (x0, y0, z0, x1, y1, z1) bounds.
```

### Comparing `brainlit-0.3.3/brainlit/utils/upload.py` & `brainlit-0.3.4/brainlit/utils/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from brainlit.utils.benchmarking_params import (
     brain_offsets,
     vol_offsets,
     scales,
     type_to_date,
 )
 
+
 import time
 from tqdm.auto import tqdm
 from brainlit.utils.util import (
     tqdm_joblib,
     check_type,
     check_iterable_type,
     check_size,
@@ -105,15 +106,14 @@
         num = int(f[1])
         scale = scales[date]
         brain_offset = brain_offsets[date]
         vol_offset = vol_offsets[date][num]
         origin = np.add(brain_offset, vol_offset)
 
     else:
-
         img_size = np.squeeze(tf.imread(str(p / "default.0.tif"))).T.shape
         transform = open(str(p / "transform.txt"), "r")
         vox_size = [
             float(s[4:].rstrip("\n")) * (0.5 ** (num_resolutions - 1))
             for s in transform.readlines()
             if "s" in s
         ]
@@ -456,16 +456,19 @@
 
         skeletons.append(skel)
         segids.append(skeletons[-1].id)
     return skeletons, segids
 
 
 def upload_segments(
-    input_path, precomputed_path, num_mips, benchmarking: Optional[bool] = False
-):
+    input_path: str,
+    precomputed_path: str,
+    num_mips: int,
+    benchmarking: Optional[bool] = False,
+) -> None:
     """Uploads segmentation data from local to precomputed path.
 
     Arguments:
         input_path: The filepath to the root directory of the octree data with consensus-swcs folder.
         precomputed_path: CloudVolume precomputed path or url.
         num_mips: The number of resolutions to upload (for info file).
         benchmarking: Optional, scales swc benchmarking data.
@@ -509,15 +512,15 @@
     segments, segids = create_skel_segids(str(swc_dir), origin, benchmarking)
     for skel in segments:
         if benchmarking == True:
             skel.vertices /= scale  # Dividing vertices by scale factor
         vols[0].skeleton.upload(skel)
 
 
-def upload_annotations(input_path, precomputed_path, num_mips):
+def upload_annotations(input_path: str, precomputed_path: str, num_mips: int) -> None:
     """Uploads empty annotation volume."""
     (_, _, vox_size, img_size, origin) = get_volume_info(
         input_path,
         num_mips,
     )
     create_cloud_volume(
         precomputed_path,
```

### Comparing `brainlit-0.3.3/brainlit/utils/util.py` & `brainlit-0.3.4/brainlit/utils/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     else:
         check_iterable_type(input, (int, np.integer))
 
 
 def check_precomputed(input):
     check_type(input, str)
     prefix = input.split(":")[0]
-    if prefix not in ["file", "s3", "gc"]:
+    if prefix not in ["file", "s3", "gc", "precomputed"]:
         raise NotImplementedError("only file, s3, and gc prefixes supported")
 
 
 def check_binary_path(input):
     check_iterable_type(input, str)  # ensure list of str
     for bcode in input:
         if not all(c in "01" for c in bcode):
```

### Comparing `brainlit-0.3.3/brainlit/viz/swc2voxel.py` & `brainlit-0.3.4/brainlit/viz/swc2voxel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from typing import Tuple
 import numpy as np
+import pandas as pd
 from scipy import ndimage as ndi
 from skimage import draw
 from brainlit.utils.util import check_type
 
 
-def snap_points(img, points, radius=[3, 3, 3]):
+def snap_points(
+    img: np.ndarray, points: pd.DataFrame, radius: list = [3, 3, 3]
+) -> pd.DataFrame:
     """Moves neuron marker points to the highest intensity within a certain radius
 
     Arguments:
         img {3d array} -- image
         points {pandas dataframe} -- dataframe with swc points as output by combine_swc_img.points2voxel
 
     Keyword Arguments:
@@ -27,15 +31,15 @@
         voxel_new = lower + voxel_new
         points_new.at[idx, "xvox"] = voxel_new[0]
         points_new.at[idx, "yvox"] = voxel_new[1]
         points_new.at[idx, "zvox"] = voxel_new[2]
     return points_new
 
 
-def point_threshold(img, points):
+def point_threshold(img: np.ndarray, points: pd.DataFrame) -> Tuple[np.ndarray, int]:
     """Threshold image according to the minimum intensity of a set of points
 
     Arguments:
         img {3d array} -- image
         points {pandas dataframe} -- dataframe with swc points as output by combine_swc_img.points2voxel
 
     Returns:
@@ -47,15 +51,15 @@
     im_sd = np.std(img)
     thresh = thresh  # - 2*im_sd
     thresholded = np.where(img > thresh, 1, 0)
 
     return thresholded, thresh
 
 
-def remove_small_components(img, size=20):
+def remove_small_components(img: np.ndarray, size: int = 20) -> np.ndarray:
     """Remove components from binary mask that are small
 
     Arguments:
         img {3d array} -- image
 
     Keyword Arguments:
         size {int} -- minimum component size (default: {20})
@@ -66,15 +70,15 @@
     label_im, nb_labels = ndi.label(img)
     sizes = ndi.sum(img, label_im, range(nb_labels + 1))
     mask = sizes > size
     binary_img = mask[label_im]
     return binary_img
 
 
-def skeletonize(img, points):
+def skeletonize(img: np.ndarray, points: pd.DataFrame) -> np.ndarray:
     """Draw lines between points that are connected to produce binary mask
 
     Arguments:
         img {3d array} -- image
         points {pandas dataframe} -- dataframe with swc points as output by combine_swc_img.points2voxel
 
     Returns:
@@ -95,15 +99,17 @@
                 child.zvox,
             )
 
             mask[xs, ys, zs] = 1
     return mask
 
 
-def skeleton_threshold_intersect(img, points):
+def skeleton_threshold_intersect(
+    img: np.ndarray, points: pd.DataFrame
+) -> Tuple[np.ndarray, int]:
     """Compute intersection between two masks: thresholded image and skeletonization of points
 
     Arguments:
         img {3d array} -- image
         points {pandas dataframe} -- dataframe with swc points as output by combine_swc_img.points2voxel
 
     Returns:
@@ -136,15 +142,17 @@
         intersect_iter[idxs] = 1
         _, num_c = ndi.measurements.label(intersect_iter)
         counter += 1 
     """
     return intersect, intersect_iter
 
 
-def Bresenham3D(x1, y1, z1, x2, y2, z2):
+def Bresenham3D(
+    x1: int, y1: int, z1: int, x2: int, y2: int, z2: int
+) -> Tuple[list, list, list]:
     """Takes two coordinates and gives the set of coordinates that connects them with a straight line
 
     Adapted from https://www.geeksforgeeks.org/bresenhams-algorithm-for-3-d-line-drawing/
 
     Arguments:
         x1 {int} -- first x coodinate
         y1 {int} -- first y coodinate
```

### Comparing `brainlit-0.3.3/brainlit.egg-info/PKG-INFO` & `brainlit-0.3.4/brainlit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 Metadata-Version: 2.1
 Name: brainlit
-Version: 0.3.3
+Version: 0.3.4
 Summary: Code to process and analyze brainlit data
 Home-page: https://github.com/neurodata/brainlit
 Author: ('Thomas Athey, Bijan Varjivand, Ryan Lu, Matt Figdore, Alex Fiallos, Stanley Wang, Victor Wang',)
 Author-email: tathey1@jhu.edu
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Brainlit
 [![DOI](https://zenodo.org/badge/237507496.svg)](https://zenodo.org/badge/latestdoi/237507496)
 [![Python](https://img.shields.io/badge/python-3.7-blue.svg)]()
+![Tests](https://img.shields.io/github/actions/workflow/status/neurodata/brainlit/python.yml)
 [![CircleCI](https://circleci.com/gh/neurodata/brainlit/tree/develop.svg?style=svg)](https://circleci.com/gh/neurodata/brainlit/tree/develop)
+[![Netlify Status](https://api.netlify.com/api/v1/badges/daad6ab0-1d47-4685-b6ab-ecc487a01ba7/deploy-status)](https://brainlit.netlify.app/)
 [![PyPI version](https://badge.fury.io/py/brainlit.svg)](https://badge.fury.io/py/brainlit)
 [![Downloads](https://img.shields.io/pypi/dw/brainlit)](https://img.shields.io/pypi/dw/brainlit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/neurodata/brainlit/branch/develop/graph/badge.svg)](https://codecov.io/gh/neurodata/brainlit)
-![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/bvarjavand/brainlit)
-![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/bvarjavand/brainlit)
+![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/neurodata/brainlit)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)  
 
 ## Summary
-This repository is a container of methods that Neurodata uses to expose their open-source code while it is in the process of being merged with larger scientific libraries such as scipy, scikit-image, or scikit-learn. Additionally, methods for computational neuroscience on brains too specific for a general scientific library can be found here, such as image registration software tuned specifically for large brain volumes. Documentation can be found by clicking on the Netlify badge below:
-
-[![Netlify Status](https://api.netlify.com/api/v1/badges/daad6ab0-1d47-4685-b6ab-ecc487a01ba7/deploy-status)](https://brainlit.netlify.app/)
-
-Brainlit is a product of the [neurodata lab](https://neurodata.io/). It is actively maintained by Thomas Athey (@tathey1) and Bijan Varjavand (@bvarjavand), and is regularly used and contributed to by students in the [Neuro Data Design](https://neurodatadesign.io/) course. We strive to follow the same [code of conduct](https://opensource.microsoft.com/codeofconduct/) that applies to the Microsoft open source community.
-
-## Contributing
-We welcome all contributors, and encourage them to follow our contribution guidelines gound in [CONTRIBUTING.md](https://github.com/neurodata/brainlit/blob/master/CONTRIBUTING.md). Issues with the "good first issue" tag are meant for contributors that are either new to open source coding, or new to the package. Additionally, users are encouraged to use issues not only to discuss code-related problems, but for more general discussions about the package.
+This repository is used for various tasks in processing, and analyzing light microscopy images of brains for the purpose of studing neuron morphology. Documentation can be found [here](http://brainlit.neurodata.io/).
 
+Brainlit is a product of the [neurodata lab](https://neurodata.io/) and the [Neuro Data Design](https://neurodatadesign.io/) course. It is actively maintained by Thomas Athey (@tathey1). We strive to follow the same [code of conduct](https://opensource.microsoft.com/codeofconduct/) that applies to the Microsoft open source community.
 
+## Contributing and Questions
+We welcome all contributors, and encourage them to follow our contribution guidelines gound in [CONTRIBUTING.md](https://github.com/neurodata/brainlit/blob/master/CONTRIBUTING.md). Issues with the "good first issue" tag are meant for contributors that are either new to open source coding, or new to the package. Additionally, users are encouraged to use issues not only to discuss code-related problems, but for more general discussions or questions about the package.
```

### Comparing `brainlit-0.3.3/setup.py` & `brainlit-0.3.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,30 +10,34 @@
 AUTHOR = (
     "Thomas Athey, Bijan Varjivand, Ryan Lu, Matt Figdore, Alex Fiallos, Stanley Wang, Victor Wang",
 )
 AUTHOR_EMAIL = "tathey1@jhu.edu"
 URL = "https://github.com/neurodata/brainlit"
 MINIMUM_PYTHON_VERSION = 3, 7  # Minimum of Python 3.7
 REQUIRED_PACKAGES = [
-"numpy>=1.8.1",
-"scikit-image>=0.16.2",
-"simpleitk>=1.2.4",
-"networkx>=2.1",
-"scikit-learn>=0.19.1",
-"scipy>=1.1.0",
-"seaborn>=0.9.0",
-"tifffile>=2020.7.17",
-"napari[pyqt5]>=0.2.11",
-"cloud-volume>=4.2.0",
-"feather-format==0.4.1",
-"nibabel>=2.4.1",
-"nilearn>=0.5.2",
-"zarr>=2.10.2",
-"h5py>=3.3.0"
-
+    "CloudReg",
+    "aicspylibczi>=3.0.5",
+    "brainrender",
+    "numpy>=1.8.1",
+    "scikit-image>=0.16.2",
+    "networkx>=2.1",
+    "scikit-learn==1.1.2",  # issues with pairwise_distances_argmin_min (e.g. used in NeuronTrace) on other versions
+    "scipy>=1.1.0",
+    "seaborn>=0.9.0",
+    "tifffile>=2020.7.17",
+    "napari[pyqt5]>=0.2.11",
+    "PyQt5<=5.15.7",  # bc there was an error with 5.15.8, can remove once that's resolved
+    "cloud-volume>=4.2.0",
+    "feather-format==0.4.1",
+    "ome-zarr>=0.6.0",
+    "zarr>=2.10.2",
+    "h5py>=3.3.0",
+    # "pcurvepy @ git+https://git@github.com/CaseyWeiner/pcurvepy@master#egg=pcurvepy",
+    "similaritymeasures>=0.4.4",
+    "statannotations>=0.4.4",
 ]
 
 # Find savanna version.
 PROJECT_PATH = os.path.dirname(os.path.abspath(__file__))
 for line in open(os.path.join(PROJECT_PATH, "brainlit", "__init__.py")):
     if line.startswith("__version__ = "):
         VERSION = line.strip().split()[2][1:-1]
@@ -66,8 +70,14 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     packages=find_packages(),
     include_package_data=True,
+    entry_points={
+        "napari.manifest": [
+            "brainlit = brainlit.napari_viterbrain:napari.yaml",
+        ],
+    },
+    package_data={"brainlit.napari_viterbrain": ["napari.yaml"]},
 )
```

