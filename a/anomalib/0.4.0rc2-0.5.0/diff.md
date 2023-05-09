# Comparing `tmp/anomalib-0.4.0rc2.tar.gz` & `tmp/anomalib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anomalib-0.4.0rc2.tar", last modified: Fri Feb 10 15:57:04 2023, max compression
+gzip compressed data, was "anomalib-0.5.0.tar", last modified: Tue May  9 15:43:58 2023, max compression
```

## Comparing `anomalib-0.4.0rc2.tar` & `anomalib-0.5.0.tar`

### file list

```diff
@@ -1,340 +1,279 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.404320 anomalib-0.4.0rc2/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    24377 2023-02-10 15:57:04.404320 anomalib-0.4.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23900 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.384320 anomalib-0.4.0rc2/anomalib/
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.384320 anomalib-0.4.0rc2/anomalib/config/
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13764 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.384320 anomalib-0.4.0rc2/anomalib/data/
--rw-r--r--   0 runner    (1001) docker     (122)     8450 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12198 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/avenue.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.384320 anomalib-0.4.0rc2/anomalib/data/base/
--rw-r--r--   0 runner    (1001) docker     (122)      384 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8120 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/base/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     7344 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/base/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     4548 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/base/video.py
--rw-r--r--   0 runner    (1001) docker     (122)    11996 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/btech.py
--rw-r--r--   0 runner    (1001) docker     (122)    14482 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/folder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/inference.py
--rw-r--r--   0 runner    (1001) docker     (122)    11736 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/mvtec.py
--rw-r--r--   0 runner    (1001) docker     (122)    13937 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/shanghaitech.py
--rw-r--r--   0 runner    (1001) docker     (122)     6941 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/task_type.py
--rw-r--r--   0 runner    (1001) docker     (122)    11258 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/ucsd_ped.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.384320 anomalib-0.4.0rc2/anomalib/data/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1119 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6762 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/utils/augmenter.py
--rw-r--r--   0 runner    (1001) docker     (122)     5077 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/utils/boxes.py
--rw-r--r--   0 runner    (1001) docker     (122)    13144 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/utils/download.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.384320 anomalib-0.4.0rc2/anomalib/data/utils/generators/
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/utils/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6027 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/utils/generators/perlin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/utils/split.py
--rw-r--r--   0 runner    (1001) docker     (122)     5086 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/utils/transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     3651 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/utils/video.py
--rw-r--r--   0 runner    (1001) docker     (122)     9615 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/data/visa.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.384320 anomalib-0.4.0rc2/anomalib/deploy/
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4031 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/deploy/export.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.384320 anomalib-0.4.0rc2/anomalib/deploy/inferencers/
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/deploy/inferencers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/deploy/inferencers/base_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8798 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/deploy/inferencers/openvino_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8524 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/deploy/inferencers/torch_inferencer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.384320 anomalib-0.4.0rc2/anomalib/models/
--rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.384320 anomalib-0.4.0rc2/anomalib/models/cfa/
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/cfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/cfa/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3051 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/cfa/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5766 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/cfa/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/cfa/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    13215 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/cfa/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/cflow/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/cflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/cflow/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/cflow/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     8299 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/cflow/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5230 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/cflow/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/cflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/components/
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/components/base/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/base/anomaly_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/base/dynamic_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/components/classification/
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/classification/kde_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/components/dimensionality_reduction/
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/dimensionality_reduction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/dimensionality_reduction/pca.py
--rw-r--r--   0 runner    (1001) docker     (122)     5337 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/dimensionality_reduction/random_projection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/components/feature_extractors/
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/feature_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4104 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/feature_extractors/timm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7928 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/feature_extractors/torchfx.py
--rw-r--r--   0 runner    (1001) docker     (122)      960 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/feature_extractors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/components/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/filters/blur.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/components/layers/
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/layers/sspcab.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/components/sampling/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/sampling/k_center_greedy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/components/stats/
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2776 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/stats/kde.py
--rw-r--r--   0 runner    (1001) docker     (122)     5603 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/components/stats/multi_variate_gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/csflow/
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/csflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/csflow/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/csflow/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4772 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/csflow/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/csflow/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    21234 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/csflow/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/dfkde/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/dfkde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/dfkde/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4824 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/dfkde/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/dfkde/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/dfm/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/dfm/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3016 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/dfm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4998 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/dfm/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     6872 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/dfm/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.388320 anomalib-0.4.0rc2/anomalib/models/draem/
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/draem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/draem/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/draem/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/draem/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    19097 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/draem/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.392320 anomalib-0.4.0rc2/anomalib/models/fastflow/
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/fastflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1624 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/fastflow/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3467 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/fastflow/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4769 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/fastflow/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/fastflow/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     9897 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/fastflow/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.392320 anomalib-0.4.0rc2/anomalib/models/ganomaly/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/ganomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3070 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/ganomaly/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     9293 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/ganomaly/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/ganomaly/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    12986 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/ganomaly/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.392320 anomalib-0.4.0rc2/anomalib/models/padim/
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/padim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4731 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/padim/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/padim/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4851 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/padim/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5900 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/padim/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.392320 anomalib-0.4.0rc2/anomalib/models/patchcore/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/patchcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/patchcore/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/patchcore/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4699 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/patchcore/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     7789 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/patchcore/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.392320 anomalib-0.4.0rc2/anomalib/models/reverse_distillation/
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/reverse_distillation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2892 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/reverse_distillation/anomaly_map.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.392320 anomalib-0.4.0rc2/anomalib/models/reverse_distillation/components/
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/reverse_distillation/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5832 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/reverse_distillation/components/bottleneck.py
--rw-r--r--   0 runner    (1001) docker     (122)    11795 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/reverse_distillation/components/de_resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/reverse_distillation/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5340 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/reverse_distillation/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/reverse_distillation/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     2853 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/reverse_distillation/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.392320 anomalib-0.4.0rc2/anomalib/models/rkde/
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/rkde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3225 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/rkde/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/rkde/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/rkde/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5611 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/rkde/region_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/rkde/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.392320 anomalib-0.4.0rc2/anomalib/models/stfpm/
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/stfpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/stfpm/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/stfpm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4438 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/stfpm/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2691 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/stfpm/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/models/stfpm/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.392320 anomalib-0.4.0rc2/anomalib/post_processing/
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/post_processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.392320 anomalib-0.4.0rc2/anomalib/post_processing/normalization/
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/post_processing/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/post_processing/normalization/cdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/post_processing/normalization/min_max.py
--rw-r--r--   0 runner    (1001) docker     (122)     5800 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/post_processing/post_process.py
--rw-r--r--   0 runner    (1001) docker     (122)    12614 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/post_processing/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.392320 anomalib-0.4.0rc2/anomalib/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/pre_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/pre_processing/pre_process.py
--rw-r--r--   0 runner    (1001) docker     (122)    14845 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/pre_processing/tiler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.392320 anomalib-0.4.0rc2/anomalib/pre_processing/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/pre_processing/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/pre_processing/transforms/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.392320 anomalib-0.4.0rc2/anomalib/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.396320 anomalib-0.4.0rc2/anomalib/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)     8399 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6536 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/cdf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (122)     1691 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/export.py
--rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/metrics_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     4143 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/min_max_normalization.py
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/model_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.396320 anomalib-0.4.0rc2/anomalib/utils/callbacks/nncf/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/nncf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3607 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/nncf/callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     7377 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/nncf/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/post_processing_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2845 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/tiler_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.396320 anomalib-0.4.0rc2/anomalib/utils/callbacks/visualizer/
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4033 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/visualizer/visualizer_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/visualizer/visualizer_image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/callbacks/visualizer/visualizer_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.396320 anomalib-0.4.0rc2/anomalib/utils/cli/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.396320 anomalib-0.4.0rc2/anomalib/utils/cv/
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/cv/connected_components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.396320 anomalib-0.4.0rc2/anomalib/utils/hpo/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/hpo/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/hpo/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.396320 anomalib-0.4.0rc2/anomalib/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (122)     4881 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4849 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/loggers/comet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     4201 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/loggers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.396320 anomalib-0.4.0rc2/anomalib/utils/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)     6914 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/metrics/anomaly_score_distribution.py
--rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/metrics/anomaly_score_threshold.py
--rw-r--r--   0 runner    (1001) docker     (122)     2780 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/metrics/aupr.py
--rw-r--r--   0 runner    (1001) docker     (122)     8435 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/metrics/aupro.py
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/metrics/auroc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/metrics/collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/metrics/min_max.py
--rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/metrics/optimal_f1.py
--rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/metrics/plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2400 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/metrics/pro.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.396320 anomalib-0.4.0rc2/anomalib/utils/sweep/
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6456 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/sweep/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.396320 anomalib-0.4.0rc2/anomalib/utils/sweep/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/sweep/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/sweep/helpers/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2387 2023-02-10 15:56:55.000000 anomalib-0.4.0rc2/anomalib/utils/sweep/helpers/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.384320 anomalib-0.4.0rc2/anomalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    24377 2023-02-10 15:57:04.000000 anomalib-0.4.0rc2/anomalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10399 2023-02-10 15:57:04.000000 anomalib-0.4.0rc2/anomalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-10 15:57:04.000000 anomalib-0.4.0rc2/anomalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-02-10 15:57:04.000000 anomalib-0.4.0rc2/anomalib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      748 2023-02-10 15:57:04.000000 anomalib-0.4.0rc2/anomalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-02-10 15:57:04.000000 anomalib-0.4.0rc2/anomalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3138 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.396320 anomalib-0.4.0rc2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      300 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/requirements/extras.txt
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/requirements/openvino.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-10 15:57:04.404320 anomalib-0.4.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3461 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.380320 anomalib-0.4.0rc2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10022 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/helpers/aupro_reference.py
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    10745 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/helpers/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/helpers/detection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/helpers/dummy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/helpers/inference.py
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/helpers/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6437 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/helpers/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     7898 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/helpers/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/nightly/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/nightly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/nightly/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/nightly/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6418 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/nightly/models/test_model_nightly.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/nightly/tools/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/nightly/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/nightly/tools/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/nightly/tools/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/nightly/tools/benchmarking/test_benchmarking.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/config/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/config/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11447 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/datasets/test_bounding_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/datasets/test_collate.py
--rw-r--r--   0 runner    (1001) docker     (122)    15776 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/datasets/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/datasets/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/datasets/test_synthetic_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4871 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/datasets/test_tiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/datasets/test_video.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/deploy/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5387 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/deploy/test_inferencer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/models/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/models/components/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      818 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/models/components/test_blur.py
--rw-r--r--   0 runner    (1001) docker     (122)     4473 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/models/test_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1545 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/models/test_model_premerge.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/post_processing/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/post_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/post_processing/test_visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/pre_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4871 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/pre_processing/test_tiler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/pre_processing/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/pre_processing/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3462 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/pre_processing/transforms/test_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/export_callback/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/export_callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/export_callback/dummy_lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/export_callback/test_export.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/metrics_configuration_callback/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/metrics_configuration_callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/metrics_configuration_callback/test_metrics_configuration_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/normalization_callback/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/normalization_callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/normalization_callback/test_normalization_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/visualizer_callback/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/visualizer_callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2286 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/visualizer_callback/dummy_lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1823 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/callbacks/visualizer_callback/test_visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.400320 anomalib-0.4.0rc2/tests/pre_merge/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/loggers/test_get_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.404320 anomalib-0.4.0rc2/tests/pre_merge/utils/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/metrics/test_adaptive_threshold.py
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/metrics/test_aupro.py
--rw-r--r--   0 runner    (1001) docker     (122)     2543 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/metrics/test_pro.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-10 15:57:04.404320 anomalib-0.4.0rc2/tests/pre_merge/utils/sweep/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2371 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/sweep/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-02-10 15:56:56.000000 anomalib-0.4.0rc2/tests/pre_merge/utils/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-09 15:43:45.000000 anomalib-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-05-09 15:43:45.000000 anomalib-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    24126 2023-05-09 15:43:58.925282 anomalib-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23624 2023-05-09 15:43:45.000000 anomalib-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2955 2023-05-09 15:43:45.000000 anomalib-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.905282 anomalib-0.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-05-09 15:43:45.000000 anomalib-0.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-05-09 15:43:45.000000 anomalib-0.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-09 15:43:45.000000 anomalib-0.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-09 15:43:45.000000 anomalib-0.5.0/requirements/loggers.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-09 15:43:45.000000 anomalib-0.5.0/requirements/notebooks.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-09 15:43:45.000000 anomalib-0.5.0/requirements/openvino.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 15:43:58.925282 anomalib-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3609 2023-05-09 15:43:45.000000 anomalib-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.901282 anomalib-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.905282 anomalib-0.5.0/src/anomalib/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.905282 anomalib-0.5.0/src/anomalib/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13768 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.905282 anomalib-0.5.0/src/anomalib/data/
+-rw-r--r--   0 runner    (1001) docker     (122)    11412 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12710 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/avenue.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.905282 anomalib-0.5.0/src/anomalib/data/base/
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8134 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/base/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7327 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/base/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2540 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/base/depth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/base/video.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12043 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/btech.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12955 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/folder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17503 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/folder_3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/inference.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11831 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/mvtec.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12984 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/mvtec_3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14449 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/shanghaitech.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6941 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11770 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/ucsd_ped.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5077 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/boxes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14332 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/download.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/data/utils/generators/
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6027 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/generators/perlin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8113 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/label.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/split.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3651 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/utils/video.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9615 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/data/visa.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/deploy/
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5674 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/deploy/export.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/deploy/inferencers/
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/deploy/inferencers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7184 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/deploy/inferencers/base_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7826 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/deploy/inferencers/openvino_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/deploy/inferencers/torch_inferencer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/models/ai_vad/
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/models/ai_vad/clip/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7865 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/clip/clip.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17868 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/clip/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2922 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    11997 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/density.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9489 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/flow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4699 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/regions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4331 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ai_vad/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/models/cfa/
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cfa/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3059 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cfa/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5766 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cfa/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cfa/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13213 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cfa/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/models/cflow/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cflow/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cflow/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     8299 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cflow/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5230 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cflow/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4179 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/cflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.909282 anomalib-0.5.0/src/anomalib/models/components/
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/base/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/base/anomaly_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/base/dynamic_module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/classification/kde_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/dimensionality_reduction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/dimensionality_reduction/pca.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5337 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/dimensionality_reduction/random_projection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/feature_extractors/
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/feature_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4104 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/feature_extractors/timm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9158 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/feature_extractors/torchfx.py
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/feature_extractors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/filters/blur.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/flow/
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12649 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/flow/all_in_one_block.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/layers/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3143 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/layers/sspcab.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/sampling/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/sampling/k_center_greedy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/components/stats/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2776 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/stats/kde.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5603 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/components/stats/multi_variate_gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/csflow/
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/csflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/csflow/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/csflow/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4772 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/csflow/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/csflow/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21233 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/csflow/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/dfkde/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfkde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfkde/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4824 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfkde/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfkde/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.913282 anomalib-0.5.0/src/anomalib/models/dfm/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfm/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3024 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4998 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfm/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6872 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/dfm/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/draem/
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/draem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/draem/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/draem/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/draem/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19097 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/draem/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/fastflow/
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/fastflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1624 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/fastflow/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/fastflow/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4769 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/fastflow/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/fastflow/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9915 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/fastflow/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/ganomaly/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ganomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3070 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ganomaly/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     9292 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ganomaly/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ganomaly/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12986 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/ganomaly/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/padim/
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/padim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4731 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/padim/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3049 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/padim/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4851 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/padim/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5900 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/padim/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/patchcore/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/patchcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/patchcore/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/patchcore/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4699 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/patchcore/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7789 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/patchcore/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/reverse_distillation/
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/anomaly_map.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5832 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/bottleneck.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11795 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/de_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5411 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/reverse_distillation/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.917282 anomalib-0.5.0/src/anomalib/models/rkde/
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/rkde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3233 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/rkde/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/rkde/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/rkde/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/rkde/region_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/rkde/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/models/stfpm/
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/stfpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/stfpm/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/stfpm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4438 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/stfpm/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2691 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/stfpm/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/models/stfpm/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/post_processing/
+-rw-r--r--   0 runner    (1001) docker     (122)      683 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/post_processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/post_processing/normalization/
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/post_processing/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/post_processing/normalization/cdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/post_processing/normalization/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5797 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/post_processing/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13077 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/post_processing/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/pre_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/pre_processing/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15168 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/pre_processing/tiler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/pre_processing/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/pre_processing/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/pre_processing/transforms/custom.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)     8412 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6536 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/cdf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1760 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/export.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/metrics_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4143 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/min_max_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/model_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/utils/callbacks/nncf/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/nncf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3607 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/nncf/callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7363 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/nncf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/post_processing_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/tiler_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4066 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/visualizer_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/visualizer_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/visualizer_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.921282 anomalib-0.5.0/src/anomalib/utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/src/anomalib/utils/cv/
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/cv/connected_components.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/src/anomalib/utils/hpo/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/hpo/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/hpo/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/src/anomalib/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (122)     4881 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4849 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/loggers/comet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4201 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/loggers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/src/anomalib/utils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     6914 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/anomaly_score_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/anomaly_score_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/aupr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9080 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/aupro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/optimal_f1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2400 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/metrics/pro.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/src/anomalib/utils/sweep/
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6456 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/sweep/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.925282 anomalib-0.5.0/src/anomalib/utils/sweep/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/sweep/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/sweep/helpers/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2325 2023-05-09 15:43:45.000000 anomalib-0.5.0/src/anomalib/utils/sweep/helpers/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:43:58.905282 anomalib-0.5.0/src/anomalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    24126 2023-05-09 15:43:58.000000 anomalib-0.5.0/src/anomalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9182 2023-05-09 15:43:58.000000 anomalib-0.5.0/src/anomalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 15:43:58.000000 anomalib-0.5.0/src/anomalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-09 15:43:58.000000 anomalib-0.5.0/src/anomalib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-05-09 15:43:58.000000 anomalib-0.5.0/src/anomalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-09 15:43:58.000000 anomalib-0.5.0/src/anomalib.egg-info/top_level.txt
```

### Comparing `anomalib-0.4.0rc2/LICENSE` & `anomalib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/PKG-INFO` & `anomalib-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: anomalib
-Version: 0.4.0rc2
+Version: 0.5.0
 Summary: anomalib - Anomaly Detection Library
 Home-page: 
 Author: Intel OpenVINO
 Author-email: help@openvino.intel.com
 License: Copyright (c) Intel - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the "License")See LICENSE file for more details.
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: extra
-Provides-Extra: full
+Provides-Extra: loggers
+Provides-Extra: notebooks
 Provides-Extra: openvino
+Provides-Extra: full
 License-File: LICENSE
 
 <div align="center">
 
 <img src="https://raw.githubusercontent.com/openvinotoolkit/anomalib/main/docs/source/images/logos/anomalib-wide-blue.png" width="600px">
 
 **A library for benchmarking, developing and deploying deep learning anomaly detection algorithms**
@@ -55,23 +56,19 @@
 - All models can be exported to [**OpenVINO**](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) Intermediate Representation (IR) for accelerated inference on intel hardware.
 - A set of [inference tools](#inference) for quick and easy deployment of the standard or custom anomaly detection models.
 
 ---
 
 # Getting Started
 
-To get an overview of all the devices where `anomalib` as been tested thoroughly, look at the [Supported Hardware](https://openvinotoolkit.github.io/anomalib/#supported-hardware) section in the documentation.
+Following is a guide on how to get started with `anomalib`. For more details, look at the [Documentation](https://openvinotoolkit.github.io/anomalib).
 
 ## Jupyter Notebooks
 
-For getting started with a Jupyter Notebook, please refer to the [Notebooks](./notebooks) folder of this repository. Additionally, you can refer to a few created by the community:
-
-<a href="https://colab.research.google.com/drive/1K4a4z2iZGBNhWdmt9Aqdld7kTAxBfAmi?usp=sharing" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> by [@bth5](https://github.com/bth5)
-
-<a target="_blank" href="https://www.kaggle.com/code/ipythonx/mvtec-ad-anomaly-detection-with-anomalib-library"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" /></a> by [@innat](https://github.com/innat)
+For getting started with a Jupyter Notebook, please refer to the [Notebooks](notebooks) folder of this repository. Additionally, you can refer to a few created by the community:
 
 ## PyPI Install
 
 You can get started with `anomalib` by just using pip.
 
 ```bash
 pip install anomalib
@@ -87,55 +84,55 @@
 git clone https://github.com/openvinotoolkit/anomalib.git
 cd anomalib
 pip install -e .
 ```
 
 # Training
 
-By default [`python tools/train.py`](https://github.com/openvinotoolkit/anomalib/blob/main/tools/train.py)
+By default [`python tools/train.py`](tools/train.py)
 runs [PADIM](https://arxiv.org/abs/2011.08785) model on `leather` category from the [MVTec AD](https://www.mvtec.com/company/research/datasets/mvtec-ad) [(CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) dataset.
 
 ```bash
 python tools/train.py    # Train PADIM on MVTec AD leather
 ```
 
 Training a model on a specific dataset and category requires further configuration. Each model has its own configuration
-file, [`config.yaml`](https://github.com/openvinotoolkit/anomalib/blob/main/configs/model/padim.yaml)
+file, [`config.yaml`](src/anomalib/models/padim/config.yaml)
 , which contains data, model and training configurable parameters. To train a specific model on a specific dataset and
 category, the config file is to be provided:
 
 ```bash
 python tools/train.py --config <path/to/model/config.yaml>
 ```
 
-For example, to train [PADIM](anomalib/models/padim) you can use
+For example, to train [PADIM](src/anomalib/models/padim) you can use
 
 ```bash
-python tools/train.py --config anomalib/models/padim/config.yaml
+python tools/train.py --config src/anomalib/models/padim/config.yaml
 ```
 
 Alternatively, a model name could also be provided as an argument, where the scripts automatically finds the corresponding config file.
 
 ```bash
 python tools/train.py --model padim
 ```
 
 where the currently available models are:
 
-- [CFA](anomalib/models/cfa)
-- [CFlow](anomalib/models/cflow)
-- [DFKDE](anomalib/models/dfkde)
-- [DFM](anomalib/models/dfm)
-- [DRAEM](anomalib/models/draem)
-- [FastFlow](anomalib/models/fastflow)
-- [GANomaly](anomalib/models/ganomaly)
-- [PADIM](anomalib/models/padim)
-- [PatchCore](anomalib/models/patchcore)
-- [Reverse Distillation](anomalib/models/reverse_distillation)
-- [STFPM](anomalib/models/stfpm)
+- [CFA](src/anomalib/models/cfa)
+- [CFlow](src/anomalib/models/cflow)
+- [DFKDE](src/anomalib/models/dfkde)
+- [DFM](src/anomalib/models/dfm)
+- [DRAEM](src/anomalib/models/draem)
+- [FastFlow](src/anomalib/models/fastflow)
+- [GANomaly](src/anomalib/models/ganomaly)
+- [PADIM](src/anomalib/models/padim)
+- [PatchCore](src/anomalib/models/patchcore)
+- [Reverse Distillation](src/anomalib/models/reverse_distillation)
+- [STFPM](src/anomalib/models/stfpm)
 
 ## Feature extraction & (pre-trained) backbones
 
 The pre-trained backbones come from [PyTorch Image Models (timm)](https://github.com/rwightman/pytorch-image-models), which are wrapped by `FeatureExtractor`.
 
 For more information, please check our documentation or the [section about feature extraction in "Getting Started with PyTorch Image Models (timm): A Practitioner’s Guide"](https://towardsdatascience.com/getting-started-with-pytorch-image-models-timm-a-practitioners-guide-4e77b4bf9055#b83b:~:text=ready%20to%20train!-,Feature%20Extraction,-timm%20models%20also>).
 
@@ -197,41 +194,39 @@
 python tools/inference/lightning_inference.py -h
 ```
 
 As a quick example:
 
 ```bash
 python tools/inference/lightning_inference.py \
-    --config anomalib/models/padim/config.yaml \
-    --weights results/padim/mvtec/bottle/weights/model.ckpt \
+    --config src/anomalib/models/padim/config.yaml \
+    --weights results/padim/mvtec/bottle/run/weights/model.ckpt \
     --input datasets/MVTec/bottle/test/broken_large/000.png \
     --output results/padim/mvtec/bottle/images
 ```
 
 Example OpenVINO Inference:
 
 ```bash
 python tools/inference/openvino_inference.py \
-    --config anomalib/models/padim/config.yaml \
-    --weights results/padim/mvtec/bottle/openvino/openvino_model.bin \
-    --meta_data results/padim/mvtec/bottle/openvino/meta_data.json \
+    --weights results/padim/mvtec/bottle/run/openvino/model.bin \
+    --metadata results/padim/mvtec/bottle/run/openvino/metadata.json \
     --input datasets/MVTec/bottle/test/broken_large/000.png \
     --output results/padim/mvtec/bottle/images
 ```
 
-> Ensure that you provide path to `meta_data.json` if you want the normalization to be applied correctly.
+> Ensure that you provide path to `metadata.json` if you want the normalization to be applied correctly.
 
-You can also use Gradio Inference to interact with the trained models using a UI. Refer to our [guide](https://openvinotoolkit.github.io/anomalib/guides/inference.html#gradio-inference) for more details.
+You can also use Gradio Inference to interact with the trained models using a UI. Refer to our [guide](https://openvinotoolkit.github.io/anomalib/tutorials/inference.html#gradio-inference) for more details.
 
 A quick example:
 
 ```bash
 python tools/inference/gradio_inference.py \
-        --config ./anomalib/models/padim/config.yaml \
-        --weights ./results/padim/mvtec/bottle/weights/model.ckpt
+        --weights results/padim/mvtec/bottle/run/weights/model.ckpt
 ```
 
 ## Exporting Model to ONNX or OpenVINO IR
 
 It is possible to export your model to ONNX or OpenVINO IR
 
 If you want to export your PyTorch model to an OpenVINO model, ensure that `export_mode` is set to `"openvino"` in the respective model `config.yaml`.
@@ -247,26 +242,26 @@
 
 ```bash
 python tools/hpo/sweep.py \
     --model padim --model_config ./path_to_config.yaml \
     --sweep_config tools/hpo/sweep.yaml
 ```
 
-For more details refer the [HPO Documentation](https://openvinotoolkit.github.io/anomalib/guides/hyperparameter_optimization.html)
+For more details refer the [HPO Documentation](https://openvinotoolkit.github.io/anomalib/tutorials/hyperparameter_optimization.html)
 
 # Benchmarking
 
 To gather benchmarking data such as throughput across categories, use the following command:
 
 ```bash
 python tools/benchmarking/benchmark.py \
     --config <relative/absolute path>/<paramfile>.yaml
 ```
 
-Refer to the [Benchmarking Documentation](https://openvinotoolkit.github.io/anomalib/guides/benchmarking.html) for more details.
+Refer to the [Benchmarking Documentation](https://openvinotoolkit.github.io/anomalib/tutorials/benchmarking.html) for more details.
 
 # Experiment Management
 
 Anomablib is integrated with various libraries for experiment tracking such as Comet, tensorboard, and wandb through [pytorch lighting loggers](https://pytorch-lightning.readthedocs.io/en/stable/extensions/logging.html).
 
 Below is an example of how to enable logging for hyper-parameters, metrics, model graphs, and predictions on images in the test data-set
 
@@ -276,15 +271,15 @@
   mode: full # options: ["full", "simple"]
 
  logging:
   logger: [comet, tensorboard, wandb]
   log_graph: True
 ```
 
-For more information, refer to the [Logging Documentation](https://openvinotoolkit.github.io/anomalib/guides/logging.html)
+For more information, refer to the [Logging Documentation](https://openvinotoolkit.github.io/anomalib/tutorials/logging.html)
 
 Note: Set your API Key for [Comet.ml](https://www.comet.com/signup?utm_source=anomalib&utm_medium=referral) via `comet_ml.init()` in interactive python or simply run `export COMET_API_KEY=<Your API Key>`
 
 # Community Projects
 
 ## 1. Web-based Pipeline for Training and Inference
 
@@ -371,7 +366,17 @@
               Utku Genc},
       year={2022},
       eprint={2202.08341},
       archivePrefix={arXiv},
       primaryClass={cs.CV}
 }
 ```
+
+# Contributing
+
+For those who would like to contribute to the library, see [CONTRIBUTING.md](CONTRIBUTING.md) for details.
+
+Thank you to all of the people who have already made a contribution - we appreciate your support!
+
+<a href="https://github.com/openvinotoolkit/anomalib/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=openvinotoolkit/anomalib" />
+</a>
```

### Comparing `anomalib-0.4.0rc2/README.md` & `anomalib-0.5.0/src/anomalib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,1494 +1,1508 @@
-00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
-00000010: 6572 223e 0a0a 3c69 6d67 2073 7263 3d22  er">..<img src="
-00000020: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00000030: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00000040: 6d2f 6f70 656e 7669 6e6f 746f 6f6c 6b69  m/openvinotoolki
-00000050: 742f 616e 6f6d 616c 6962 2f6d 6169 6e2f  t/anomalib/main/
-00000060: 646f 6373 2f73 6f75 7263 652f 696d 6167  docs/source/imag
-00000070: 6573 2f6c 6f67 6f73 2f61 6e6f 6d61 6c69  es/logos/anomali
-00000080: 622d 7769 6465 2d62 6c75 652e 706e 6722  b-wide-blue.png"
-00000090: 2077 6964 7468 3d22 3630 3070 7822 3e0a   width="600px">.
-000000a0: 0a2a 2a41 206c 6962 7261 7279 2066 6f72  .**A library for
-000000b0: 2062 656e 6368 6d61 726b 696e 672c 2064   benchmarking, d
-000000c0: 6576 656c 6f70 696e 6720 616e 6420 6465  eveloping and de
-000000d0: 706c 6f79 696e 6720 6465 6570 206c 6561  ploying deep lea
-000000e0: 726e 696e 6720 616e 6f6d 616c 7920 6465  rning anomaly de
-000000f0: 7465 6374 696f 6e20 616c 676f 7269 7468  tection algorith
-00000100: 6d73 2a2a 0a0a 2d2d 2d0a 0a5b 4b65 7920  ms**..---..[Key 
-00000110: 4665 6174 7572 6573 5d28 236b 6579 2d66  Features](#key-f
-00000120: 6561 7475 7265 7329 20e2 80a2 0a5b 4765  eatures) ....[Ge
-00000130: 7474 696e 6720 5374 6172 7465 645d 2823  tting Started](#
-00000140: 6765 7474 696e 672d 7374 6172 7465 6429  getting-started)
-00000150: 20e2 80a2 0a5b 446f 6373 5d28 6874 7470   ....[Docs](http
-00000160: 733a 2f2f 6f70 656e 7669 6e6f 746f 6f6c  s://openvinotool
-00000170: 6b69 742e 6769 7468 7562 2e69 6f2f 616e  kit.github.io/an
-00000180: 6f6d 616c 6962 2920 e280 a20a 5b4c 6963  omalib) ....[Lic
-00000190: 656e 7365 5d28 6874 7470 733a 2f2f 6769  ense](https://gi
-000001a0: 7468 7562 2e63 6f6d 2f6f 7065 6e76 696e  thub.com/openvin
-000001b0: 6f74 6f6f 6c6b 6974 2f61 6e6f 6d61 6c69  otoolkit/anomali
-000001c0: 622f 626c 6f62 2f6d 6169 6e2f 4c49 4345  b/blob/main/LICE
-000001d0: 4e53 4529 0a0a 5b21 5b70 7974 686f 6e5d  NSE)..[![python]
-000001e0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000001f0: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
-00000200: 7468 6f6e 2d33 2e37 2532 422d 6772 6565  thon-3.7%2B-gree
-00000210: 6e29 5d28 290a 5b21 5b70 7974 6f72 6368  n)]().[![pytorch
-00000220: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000230: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
-00000240: 7974 6f72 6368 2d31 2e38 2e31 2532 422d  ytorch-1.8.1%2B-
-00000250: 6f72 616e 6765 295d 2829 0a5b 215b 6f70  orange)]().[![op
-00000260: 656e 7669 6e6f 5d28 6874 7470 733a 2f2f  envino](https://
-00000270: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000280: 6164 6765 2f6f 7065 6e76 696e 6f2d 3230  adge/openvino-20
-00000290: 3231 2e34 2e32 2d70 7572 706c 6529 5d28  21.4.2-purple)](
-000002a0: 290a 5b21 5b63 6f6d 6574 5d28 6874 7470  ).[![comet](http
-000002b0: 733a 2f2f 6375 7374 6f6d 2d69 636f 6e2d  s://custom-icon-
-000002c0: 6261 6467 6573 2e68 6572 6f6b 7561 7070  badges.herokuapp
-000002d0: 2e63 6f6d 2f62 6164 6765 2f63 6f6d 6574  .com/badge/comet
-000002e0: 5f5f 6d6c 2d33 2e33 312e 372d 6f72 616e  __ml-3.31.7-oran
-000002f0: 6765 3f6c 6f67 6f3d 6c6f 676f 5f63 6f6d  ge?logo=logo_com
-00000300: 6574 5f6d 6c29 5d28 6874 7470 733a 2f2f  et_ml)](https://
-00000310: 7777 772e 636f 6d65 742e 636f 6d2f 7369  www.comet.com/si
-00000320: 7465 2f70 726f 6475 6374 732f 6d6c 2d65  te/products/ml-e
-00000330: 7870 6572 696d 656e 742d 7472 6163 6b69  xperiment-tracki
-00000340: 6e67 2f3f 7574 6d5f 736f 7572 6365 3d61  ng/?utm_source=a
-00000350: 6e6f 6d61 6c69 6226 7574 6d5f 6d65 6469  nomalib&utm_medi
-00000360: 756d 3d72 6566 6572 7261 6c29 0a5b 215b  um=referral).[![
-00000370: 436f 6461 6379 2042 6164 6765 5d28 6874  Codacy Badge](ht
-00000380: 7470 733a 2f2f 6170 702e 636f 6461 6379  tps://app.codacy
-00000390: 2e63 6f6d 2f70 726f 6a65 6374 2f62 6164  .com/project/bad
-000003a0: 6765 2f47 7261 6465 2f36 3834 3932 3763  ge/Grade/684927c
-000003b0: 3163 3736 6334 6335 6539 3462 6235 3334  1c76c4c5e94bb534
-000003c0: 3830 3831 3266 6262 6229 5d28 6874 7470  80812fbbb)](http
-000003d0: 733a 2f2f 7777 772e 636f 6461 6379 2e63  s://www.codacy.c
-000003e0: 6f6d 2f67 682f 6f70 656e 7669 6e6f 746f  om/gh/openvinoto
-000003f0: 6f6c 6b69 742f 616e 6f6d 616c 6962 2f64  olkit/anomalib/d
-00000400: 6173 6862 6f61 7264 3f75 746d 5f73 6f75  ashboard?utm_sou
-00000410: 7263 653d 6769 7468 7562 2e63 6f6d 2675  rce=github.com&u
-00000420: 746d 5f6d 6564 6975 6d3d 7265 6665 7272  tm_medium=referr
-00000430: 616c 2675 746d 5f63 6f6e 7465 6e74 3d6f  al&utm_content=o
-00000440: 7065 6e76 696e 6f74 6f6f 6c6b 6974 2f61  penvinotoolkit/a
-00000450: 6e6f 6d61 6c69 6226 7574 6d5f 6361 6d70  nomalib&utm_camp
-00000460: 6169 676e 3d42 6164 6765 5f47 7261 6465  aign=Badge_Grade
-00000470: 290a 5b21 5b62 6c61 636b 5d28 6874 7470  ).[![black](http
-00000480: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000490: 696f 2f62 6164 6765 2f63 6f64 6525 3230  io/badge/code%20
-000004a0: 7374 796c 652d 626c 6163 6b2d 3030 3030  style-black-0000
-000004b0: 3030 2e73 7667 295d 2829 0a5b 215b 4e69  00.svg)]().[![Ni
-000004c0: 6768 746c 792d 5265 6772 6573 7369 6f6e  ghtly-Regression
-000004d0: 2054 6573 745d 2868 7474 7073 3a2f 2f67   Test](https://g
-000004e0: 6974 6875 622e 636f 6d2f 6f70 656e 7669  ithub.com/openvi
-000004f0: 6e6f 746f 6f6c 6b69 742f 616e 6f6d 616c  notoolkit/anomal
-00000500: 6962 2f61 6374 696f 6e73 2f77 6f72 6b66  ib/actions/workf
-00000510: 6c6f 7773 2f6e 6967 6874 6c79 2e79 6d6c  lows/nightly.yml
-00000520: 2f62 6164 6765 2e73 7667 295d 2868 7474  /badge.svg)](htt
-00000530: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000540: 6f70 656e 7669 6e6f 746f 6f6c 6b69 742f  openvinotoolkit/
-00000550: 616e 6f6d 616c 6962 2f61 6374 696f 6e73  anomalib/actions
-00000560: 2f77 6f72 6b66 6c6f 7773 2f6e 6967 6874  /workflows/night
-00000570: 6c79 2e79 6d6c 290a 5b21 5b50 7265 2d4d  ly.yml).[![Pre-M
-00000580: 6572 6765 2043 6865 636b 735d 2868 7474  erge Checks](htt
-00000590: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000005a0: 6f70 656e 7669 6e6f 746f 6f6c 6b69 742f  openvinotoolkit/
-000005b0: 616e 6f6d 616c 6962 2f61 6374 696f 6e73  anomalib/actions
-000005c0: 2f77 6f72 6b66 6c6f 7773 2f70 7265 5f6d  /workflows/pre_m
-000005d0: 6572 6765 2e79 6d6c 2f62 6164 6765 2e73  erge.yml/badge.s
-000005e0: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
-000005f0: 6875 622e 636f 6d2f 6f70 656e 7669 6e6f  hub.com/openvino
-00000600: 746f 6f6c 6b69 742f 616e 6f6d 616c 6962  toolkit/anomalib
-00000610: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000620: 7773 2f70 7265 5f6d 6572 6765 2e79 6d6c  ws/pre_merge.yml
-00000630: 290a 5b21 5b63 6f64 6563 6f76 5d28 6874  ).[![codecov](ht
-00000640: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-00000650: 2f67 682f 6f70 656e 7669 6e6f 746f 6f6c  /gh/openvinotool
-00000660: 6b69 742f 616e 6f6d 616c 6962 2f62 7261  kit/anomalib/bra
-00000670: 6e63 682f 6d61 696e 2f67 7261 7068 2f62  nch/main/graph/b
-00000680: 6164 6765 2e73 7667 3f74 6f6b 656e 3d5a  adge.svg?token=Z
-00000690: 3641 3037 4e31 425a 4b29 5d28 6874 7470  6A07N1BZK)](http
-000006a0: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
-000006b0: 682f 6f70 656e 7669 6e6f 746f 6f6c 6b69  h/openvinotoolki
-000006c0: 742f 616e 6f6d 616c 6962 290a 5b21 5b44  t/anomalib).[![D
-000006d0: 6f63 735d 2868 7474 7073 3a2f 2f67 6974  ocs](https://git
-000006e0: 6875 622e 636f 6d2f 6f70 656e 7669 6e6f  hub.com/openvino
-000006f0: 746f 6f6c 6b69 742f 616e 6f6d 616c 6962  toolkit/anomalib
-00000700: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000710: 7773 2f64 6f63 732e 796d 6c2f 6261 6467  ws/docs.yml/badg
-00000720: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-00000730: 6769 7468 7562 2e63 6f6d 2f6f 7065 6e76  github.com/openv
-00000740: 696e 6f74 6f6f 6c6b 6974 2f61 6e6f 6d61  inotoolkit/anoma
-00000750: 6c69 622f 6163 7469 6f6e 732f 776f 726b  lib/actions/work
-00000760: 666c 6f77 732f 646f 6373 2e79 6d6c 290a  flows/docs.yml).
-00000770: 5b21 5b44 6f77 6e6c 6f61 6473 5d28 6874  [![Downloads](ht
-00000780: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
-00000790: 792e 7465 6368 2f70 6572 736f 6e61 6c69  y.tech/personali
-000007a0: 7a65 642d 6261 6467 652f 616e 6f6d 616c  zed-badge/anomal
-000007b0: 6962 3f70 6572 696f 643d 746f 7461 6c26  ib?period=total&
-000007c0: 756e 6974 733d 696e 7465 726e 6174 696f  units=internatio
-000007d0: 6e61 6c5f 7379 7374 656d 266c 6566 745f  nal_system&left_
-000007e0: 636f 6c6f 723d 6772 6579 2672 6967 6874  color=grey&right
-000007f0: 5f63 6f6c 6f72 3d67 7265 656e 266c 6566  _color=green&lef
-00000800: 745f 7465 7874 3d50 7950 4925 3230 446f  t_text=PyPI%20Do
-00000810: 776e 6c6f 6164 7329 5d28 6874 7470 733a  wnloads)](https:
-00000820: 2f2f 7065 7079 2e74 6563 682f 7072 6f6a  //pepy.tech/proj
-00000830: 6563 742f 616e 6f6d 616c 6962 290a 0a3c  ect/anomalib)..<
-00000840: 2f64 6976 3e0a 0a2d 2d2d 0a0a 2320 496e  /div>..---..# In
-00000850: 7472 6f64 7563 7469 6f6e 0a0a 416e 6f6d  troduction..Anom
-00000860: 616c 6962 2069 7320 6120 6465 6570 206c  alib is a deep l
-00000870: 6561 726e 696e 6720 6c69 6272 6172 7920  earning library 
-00000880: 7468 6174 2061 696d 7320 746f 2063 6f6c  that aims to col
-00000890: 6c65 6374 2073 7461 7465 2d6f 662d 7468  lect state-of-th
-000008a0: 652d 6172 7420 616e 6f6d 616c 7920 6465  e-art anomaly de
-000008b0: 7465 6374 696f 6e20 616c 676f 7269 7468  tection algorith
-000008c0: 6d73 2066 6f72 2062 656e 6368 6d61 726b  ms for benchmark
-000008d0: 696e 6720 6f6e 2062 6f74 6820 7075 626c  ing on both publ
-000008e0: 6963 2061 6e64 2070 7269 7661 7465 2064  ic and private d
-000008f0: 6174 6173 6574 732e 2041 6e6f 6d61 6c69  atasets. Anomali
-00000900: 6220 7072 6f76 6964 6573 2073 6576 6572  b provides sever
-00000910: 616c 2072 6561 6479 2d74 6f2d 7573 6520  al ready-to-use 
-00000920: 696d 706c 656d 656e 7461 7469 6f6e 7320  implementations 
-00000930: 6f66 2061 6e6f 6d61 6c79 2064 6574 6563  of anomaly detec
-00000940: 7469 6f6e 2061 6c67 6f72 6974 686d 7320  tion algorithms 
-00000950: 6465 7363 7269 6265 6420 696e 2074 6865  described in the
-00000960: 2072 6563 656e 7420 6c69 7465 7261 7475   recent literatu
-00000970: 7265 2c20 6173 2077 656c 6c20 6173 2061  re, as well as a
-00000980: 2073 6574 206f 6620 746f 6f6c 7320 7468   set of tools th
-00000990: 6174 2066 6163 696c 6974 6174 6520 7468  at facilitate th
-000009a0: 6520 6465 7665 6c6f 706d 656e 7420 616e  e development an
-000009b0: 6420 696d 706c 656d 656e 7461 7469 6f6e  d implementation
-000009c0: 206f 6620 6375 7374 6f6d 206d 6f64 656c   of custom model
-000009d0: 732e 2054 6865 206c 6962 7261 7279 2068  s. The library h
-000009e0: 6173 2061 2073 7472 6f6e 6720 666f 6375  as a strong focu
-000009f0: 7320 6f6e 2069 6d61 6765 2d62 6173 6564  s on image-based
-00000a00: 2061 6e6f 6d61 6c79 2064 6574 6563 7469   anomaly detecti
-00000a10: 6f6e 2c20 7768 6572 6520 7468 6520 676f  on, where the go
-00000a20: 616c 206f 6620 7468 6520 616c 676f 7269  al of the algori
-00000a30: 7468 6d20 6973 2074 6f20 6964 656e 7469  thm is to identi
-00000a40: 6679 2061 6e6f 6d61 6c6f 7573 2069 6d61  fy anomalous ima
-00000a50: 6765 732c 206f 7220 616e 6f6d 616c 6f75  ges, or anomalou
-00000a60: 7320 7069 7865 6c20 7265 6769 6f6e 7320  s pixel regions 
-00000a70: 7769 7468 696e 2069 6d61 6765 7320 696e  within images in
-00000a80: 2061 2064 6174 6173 6574 2e20 416e 6f6d   a dataset. Anom
-00000a90: 616c 6962 2069 7320 636f 6e73 7461 6e74  alib is constant
-00000aa0: 6c79 2075 7064 6174 6564 2077 6974 6820  ly updated with 
-00000ab0: 6e65 7720 616c 676f 7269 7468 6d73 2061  new algorithms a
-00000ac0: 6e64 2074 7261 696e 696e 672f 696e 6665  nd training/infe
-00000ad0: 7265 6e63 6520 6578 7465 6e73 696f 6e73  rence extensions
-00000ae0: 2c20 736f 206b 6565 7020 6368 6563 6b69  , so keep checki
-00000af0: 6e67 210a 0a21 5b53 616d 706c 6520 496d  ng!..![Sample Im
-00000b00: 6167 655d 2868 7474 7073 3a2f 2f72 6177  age](https://raw
-00000b10: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000b20: 6e74 2e63 6f6d 2f6f 7065 6e76 696e 6f74  nt.com/openvinot
-00000b30: 6f6f 6c6b 6974 2f61 6e6f 6d61 6c69 622f  oolkit/anomalib/
-00000b40: 6d61 696e 2f64 6f63 732f 736f 7572 6365  main/docs/source
-00000b50: 2f69 6d61 6765 732f 7265 6164 6d65 2e70  /images/readme.p
-00000b60: 6e67 290a 0a23 2320 4b65 7920 6665 6174  ng)..## Key feat
-00000b70: 7572 6573 0a0a 2d20 5468 6520 6c61 7267  ures..- The larg
-00000b80: 6573 7420 7075 626c 6963 2063 6f6c 6c65  est public colle
-00000b90: 6374 696f 6e20 6f66 2072 6561 6479 2d74  ction of ready-t
-00000ba0: 6f2d 7573 6520 6465 6570 206c 6561 726e  o-use deep learn
-00000bb0: 696e 6720 616e 6f6d 616c 7920 6465 7465  ing anomaly dete
-00000bc0: 6374 696f 6e20 616c 676f 7269 7468 6d73  ction algorithms
-00000bd0: 2061 6e64 2062 656e 6368 6d61 726b 2064   and benchmark d
-00000be0: 6174 6173 6574 732e 0a2d 205b 2a2a 5079  atasets..- [**Py
-00000bf0: 546f 7263 6820 4c69 6768 746e 696e 672a  Torch Lightning*
-00000c00: 2a5d 2868 7474 7073 3a2f 2f77 7777 2e70  *](https://www.p
-00000c10: 7974 6f72 6368 6c69 6768 746e 696e 672e  ytorchlightning.
-00000c20: 6169 2f29 2062 6173 6564 206d 6f64 656c  ai/) based model
-00000c30: 2069 6d70 6c65 6d65 6e74 6174 696f 6e73   implementations
-00000c40: 2074 6f20 7265 6475 6365 2062 6f69 6c65   to reduce boile
-00000c50: 7270 6c61 7465 2063 6f64 6520 616e 6420  rplate code and 
-00000c60: 6c69 6d69 7420 7468 6520 696d 706c 656d  limit the implem
-00000c70: 656e 7461 7469 6f6e 2065 6666 6f72 7473  entation efforts
-00000c80: 2074 6f20 7468 6520 6261 7265 2065 7373   to the bare ess
-00000c90: 656e 7469 616c 732e 0a2d 2041 6c6c 206d  entials..- All m
-00000ca0: 6f64 656c 7320 6361 6e20 6265 2065 7870  odels can be exp
-00000cb0: 6f72 7465 6420 746f 205b 2a2a 4f70 656e  orted to [**Open
-00000cc0: 5649 4e4f 2a2a 5d28 6874 7470 733a 2f2f  VINO**](https://
-00000cd0: 7777 772e 696e 7465 6c2e 636f 6d2f 636f  www.intel.com/co
-00000ce0: 6e74 656e 742f 7777 772f 7573 2f65 6e2f  ntent/www/us/en/
-00000cf0: 6465 7665 6c6f 7065 722f 746f 6f6c 732f  developer/tools/
-00000d00: 6f70 656e 7669 6e6f 2d74 6f6f 6c6b 6974  openvino-toolkit
-00000d10: 2f6f 7665 7276 6965 772e 6874 6d6c 2920  /overview.html) 
-00000d20: 496e 7465 726d 6564 6961 7465 2052 6570  Intermediate Rep
-00000d30: 7265 7365 6e74 6174 696f 6e20 2849 5229  resentation (IR)
-00000d40: 2066 6f72 2061 6363 656c 6572 6174 6564   for accelerated
-00000d50: 2069 6e66 6572 656e 6365 206f 6e20 696e   inference on in
-00000d60: 7465 6c20 6861 7264 7761 7265 2e0a 2d20  tel hardware..- 
-00000d70: 4120 7365 7420 6f66 205b 696e 6665 7265  A set of [infere
-00000d80: 6e63 6520 746f 6f6c 735d 2823 696e 6665  nce tools](#infe
-00000d90: 7265 6e63 6529 2066 6f72 2071 7569 636b  rence) for quick
-00000da0: 2061 6e64 2065 6173 7920 6465 706c 6f79   and easy deploy
-00000db0: 6d65 6e74 206f 6620 7468 6520 7374 616e  ment of the stan
-00000dc0: 6461 7264 206f 7220 6375 7374 6f6d 2061  dard or custom a
-00000dd0: 6e6f 6d61 6c79 2064 6574 6563 7469 6f6e  nomaly detection
-00000de0: 206d 6f64 656c 732e 0a0a 2d2d 2d0a 0a23   models...---..#
-00000df0: 2047 6574 7469 6e67 2053 7461 7274 6564   Getting Started
-00000e00: 0a0a 546f 2067 6574 2061 6e20 6f76 6572  ..To get an over
-00000e10: 7669 6577 206f 6620 616c 6c20 7468 6520  view of all the 
-00000e20: 6465 7669 6365 7320 7768 6572 6520 6061  devices where `a
-00000e30: 6e6f 6d61 6c69 6260 2061 7320 6265 656e  nomalib` as been
-00000e40: 2074 6573 7465 6420 7468 6f72 6f75 6768   tested thorough
-00000e50: 6c79 2c20 6c6f 6f6b 2061 7420 7468 6520  ly, look at the 
-00000e60: 5b53 7570 706f 7274 6564 2048 6172 6477  [Supported Hardw
-00000e70: 6172 655d 2868 7474 7073 3a2f 2f6f 7065  are](https://ope
-00000e80: 6e76 696e 6f74 6f6f 6c6b 6974 2e67 6974  nvinotoolkit.git
-00000e90: 6875 622e 696f 2f61 6e6f 6d61 6c69 622f  hub.io/anomalib/
-00000ea0: 2373 7570 706f 7274 6564 2d68 6172 6477  #supported-hardw
-00000eb0: 6172 6529 2073 6563 7469 6f6e 2069 6e20  are) section in 
-00000ec0: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
-00000ed0: 6e2e 0a0a 2323 204a 7570 7974 6572 204e  n...## Jupyter N
-00000ee0: 6f74 6562 6f6f 6b73 0a0a 466f 7220 6765  otebooks..For ge
-00000ef0: 7474 696e 6720 7374 6172 7465 6420 7769  tting started wi
-00000f00: 7468 2061 204a 7570 7974 6572 204e 6f74  th a Jupyter Not
-00000f10: 6562 6f6f 6b2c 2070 6c65 6173 6520 7265  ebook, please re
-00000f20: 6665 7220 746f 2074 6865 205b 4e6f 7465  fer to the [Note
-00000f30: 626f 6f6b 735d 282e 2f6e 6f74 6562 6f6f  books](./noteboo
-00000f40: 6b73 2920 666f 6c64 6572 206f 6620 7468  ks) folder of th
-00000f50: 6973 2072 6570 6f73 6974 6f72 792e 2041  is repository. A
-00000f60: 6464 6974 696f 6e61 6c6c 792c 2079 6f75  dditionally, you
-00000f70: 2063 616e 2072 6566 6572 2074 6f20 6120   can refer to a 
-00000f80: 6665 7720 6372 6561 7465 6420 6279 2074  few created by t
-00000f90: 6865 2063 6f6d 6d75 6e69 7479 3a0a 0a3c  he community:..<
-00000fa0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000fb0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-00000fc0: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
-00000fd0: 314b 3461 347a 3269 5a47 424e 6857 646d  1K4a4z2iZGBNhWdm
-00000fe0: 7439 4171 646c 6437 6b54 4178 4266 416d  t9Aqdld7kTAxBfAm
-00000ff0: 693f 7573 703d 7368 6172 696e 6722 2074  i?usp=sharing" t
-00001000: 6172 6765 743d 225f 7061 7265 6e74 223e  arget="_parent">
-00001010: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001020: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-00001030: 2e67 6f6f 676c 652e 636f 6d2f 6173 7365  .google.com/asse
-00001040: 7473 2f63 6f6c 6162 2d62 6164 6765 2e73  ts/colab-badge.s
-00001050: 7667 2220 616c 743d 224f 7065 6e20 496e  vg" alt="Open In
-00001060: 2043 6f6c 6162 222f 3e3c 2f61 3e20 6279   Colab"/></a> by
-00001070: 205b 4062 7468 355d 2868 7474 7073 3a2f   [@bth5](https:/
-00001080: 2f67 6974 6875 622e 636f 6d2f 6274 6835  /github.com/bth5
-00001090: 290a 0a3c 6120 7461 7267 6574 3d22 5f62  )..<a target="_b
-000010a0: 6c61 6e6b 2220 6872 6566 3d22 6874 7470  lank" href="http
-000010b0: 733a 2f2f 7777 772e 6b61 6767 6c65 2e63  s://www.kaggle.c
-000010c0: 6f6d 2f63 6f64 652f 6970 7974 686f 6e78  om/code/ipythonx
-000010d0: 2f6d 7674 6563 2d61 642d 616e 6f6d 616c  /mvtec-ad-anomal
-000010e0: 792d 6465 7465 6374 696f 6e2d 7769 7468  y-detection-with
-000010f0: 2d61 6e6f 6d61 6c69 622d 6c69 6272 6172  -anomalib-librar
-00001100: 7922 3e3c 696d 6720 7372 633d 2268 7474  y"><img src="htt
-00001110: 7073 3a2f 2f6b 6167 676c 652e 636f 6d2f  ps://kaggle.com/
-00001120: 7374 6174 6963 2f69 6d61 6765 732f 6f70  static/images/op
-00001130: 656e 2d69 6e2d 6b61 6767 6c65 2e73 7667  en-in-kaggle.svg
-00001140: 2220 2f3e 3c2f 613e 2062 7920 5b40 696e  " /></a> by [@in
-00001150: 6e61 745d 2868 7474 7073 3a2f 2f67 6974  nat](https://git
-00001160: 6875 622e 636f 6d2f 696e 6e61 7429 0a0a  hub.com/innat)..
-00001170: 2323 2050 7950 4920 496e 7374 616c 6c0a  ## PyPI Install.
-00001180: 0a59 6f75 2063 616e 2067 6574 2073 7461  .You can get sta
-00001190: 7274 6564 2077 6974 6820 6061 6e6f 6d61  rted with `anoma
-000011a0: 6c69 6260 2062 7920 6a75 7374 2075 7369  lib` by just usi
-000011b0: 6e67 2070 6970 2e0a 0a60 6060 6261 7368  ng pip...```bash
-000011c0: 0a70 6970 2069 6e73 7461 6c6c 2061 6e6f  .pip install ano
-000011d0: 6d61 6c69 620a 6060 600a 0a23 2320 4c6f  malib.```..## Lo
-000011e0: 6361 6c20 496e 7374 616c 6c0a 0a49 7420  cal Install..It 
-000011f0: 6973 2068 6967 686c 7920 7265 636f 6d6d  is highly recomm
-00001200: 656e 6465 6420 746f 2075 7365 2076 6972  ended to use vir
-00001210: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
-00001220: 2077 6865 6e20 696e 7374 616c 6c69 6e67   when installing
-00001230: 2061 6e6f 6d61 6c69 622e 2046 6f72 2069   anomalib. For i
-00001240: 6e73 7461 6e63 652c 2077 6974 6820 5b61  nstance, with [a
-00001250: 6e61 636f 6e64 615d 2868 7474 7073 3a2f  naconda](https:/
-00001260: 2f77 7777 2e61 6e61 636f 6e64 612e 636f  /www.anaconda.co
-00001270: 6d2f 7072 6f64 7563 7473 2f69 6e64 6976  m/products/indiv
-00001280: 6964 7561 6c29 2c20 6061 6e6f 6d61 6c69  idual), `anomali
-00001290: 6260 2063 6f75 6c64 2062 6520 696e 7374  b` could be inst
-000012a0: 616c 6c65 6420 6173 2c0a 0a60 6060 6261  alled as,..```ba
-000012b0: 7368 0a79 6573 207c 2063 6f6e 6461 2063  sh.yes | conda c
-000012c0: 7265 6174 6520 2d6e 2061 6e6f 6d61 6c69  reate -n anomali
-000012d0: 625f 656e 7620 7079 7468 6f6e 3d33 2e38  b_env python=3.8
-000012e0: 0a63 6f6e 6461 2061 6374 6976 6174 6520  .conda activate 
-000012f0: 616e 6f6d 616c 6962 5f65 6e76 0a67 6974  anomalib_env.git
-00001300: 2063 6c6f 6e65 2068 7474 7073 3a2f 2f67   clone https://g
-00001310: 6974 6875 622e 636f 6d2f 6f70 656e 7669  ithub.com/openvi
-00001320: 6e6f 746f 6f6c 6b69 742f 616e 6f6d 616c  notoolkit/anomal
-00001330: 6962 2e67 6974 0a63 6420 616e 6f6d 616c  ib.git.cd anomal
-00001340: 6962 0a70 6970 2069 6e73 7461 6c6c 202d  ib.pip install -
-00001350: 6520 2e0a 6060 600a 0a23 2054 7261 696e  e ..```..# Train
-00001360: 696e 670a 0a42 7920 6465 6661 756c 7420  ing..By default 
-00001370: 5b60 7079 7468 6f6e 2074 6f6f 6c73 2f74  [`python tools/t
-00001380: 7261 696e 2e70 7960 5d28 6874 7470 733a  rain.py`](https:
-00001390: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 7065  //github.com/ope
-000013a0: 6e76 696e 6f74 6f6f 6c6b 6974 2f61 6e6f  nvinotoolkit/ano
-000013b0: 6d61 6c69 622f 626c 6f62 2f6d 6169 6e2f  malib/blob/main/
-000013c0: 746f 6f6c 732f 7472 6169 6e2e 7079 290a  tools/train.py).
-000013d0: 7275 6e73 205b 5041 4449 4d5d 2868 7474  runs [PADIM](htt
-000013e0: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-000013f0: 6273 2f32 3031 312e 3038 3738 3529 206d  bs/2011.08785) m
-00001400: 6f64 656c 206f 6e20 606c 6561 7468 6572  odel on `leather
-00001410: 6020 6361 7465 676f 7279 2066 726f 6d20  ` category from 
-00001420: 7468 6520 5b4d 5654 6563 2041 445d 2868  the [MVTec AD](h
-00001430: 7474 7073 3a2f 2f77 7777 2e6d 7674 6563  ttps://www.mvtec
-00001440: 2e63 6f6d 2f63 6f6d 7061 6e79 2f72 6573  .com/company/res
-00001450: 6561 7263 682f 6461 7461 7365 7473 2f6d  earch/datasets/m
-00001460: 7674 6563 2d61 6429 205b 2843 4320 4259  vtec-ad) [(CC BY
-00001470: 2d4e 432d 5341 2034 2e30 295d 2868 7474  -NC-SA 4.0)](htt
-00001480: 7073 3a2f 2f63 7265 6174 6976 6563 6f6d  ps://creativecom
-00001490: 6d6f 6e73 2e6f 7267 2f6c 6963 656e 7365  mons.org/license
-000014a0: 732f 6279 2d6e 632d 7361 2f34 2e30 2f29  s/by-nc-sa/4.0/)
-000014b0: 2064 6174 6173 6574 2e0a 0a60 6060 6261   dataset...```ba
-000014c0: 7368 0a70 7974 686f 6e20 746f 6f6c 732f  sh.python tools/
-000014d0: 7472 6169 6e2e 7079 2020 2020 2320 5472  train.py    # Tr
-000014e0: 6169 6e20 5041 4449 4d20 6f6e 204d 5654  ain PADIM on MVT
-000014f0: 6563 2041 4420 6c65 6174 6865 720a 6060  ec AD leather.``
-00001500: 600a 0a54 7261 696e 696e 6720 6120 6d6f  `..Training a mo
-00001510: 6465 6c20 6f6e 2061 2073 7065 6369 6669  del on a specifi
-00001520: 6320 6461 7461 7365 7420 616e 6420 6361  c dataset and ca
-00001530: 7465 676f 7279 2072 6571 7569 7265 7320  tegory requires 
-00001540: 6675 7274 6865 7220 636f 6e66 6967 7572  further configur
-00001550: 6174 696f 6e2e 2045 6163 6820 6d6f 6465  ation. Each mode
-00001560: 6c20 6861 7320 6974 7320 6f77 6e20 636f  l has its own co
-00001570: 6e66 6967 7572 6174 696f 6e0a 6669 6c65  nfiguration.file
-00001580: 2c20 5b60 636f 6e66 6967 2e79 616d 6c60  , [`config.yaml`
-00001590: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000015a0: 2e63 6f6d 2f6f 7065 6e76 696e 6f74 6f6f  .com/openvinotoo
-000015b0: 6c6b 6974 2f61 6e6f 6d61 6c69 622f 626c  lkit/anomalib/bl
-000015c0: 6f62 2f6d 6169 6e2f 636f 6e66 6967 732f  ob/main/configs/
-000015d0: 6d6f 6465 6c2f 7061 6469 6d2e 7961 6d6c  model/padim.yaml
-000015e0: 290a 2c20 7768 6963 6820 636f 6e74 6169  )., which contai
-000015f0: 6e73 2064 6174 612c 206d 6f64 656c 2061  ns data, model a
-00001600: 6e64 2074 7261 696e 696e 6720 636f 6e66  nd training conf
-00001610: 6967 7572 6162 6c65 2070 6172 616d 6574  igurable paramet
-00001620: 6572 732e 2054 6f20 7472 6169 6e20 6120  ers. To train a 
-00001630: 7370 6563 6966 6963 206d 6f64 656c 206f  specific model o
-00001640: 6e20 6120 7370 6563 6966 6963 2064 6174  n a specific dat
-00001650: 6173 6574 2061 6e64 0a63 6174 6567 6f72  aset and.categor
-00001660: 792c 2074 6865 2063 6f6e 6669 6720 6669  y, the config fi
-00001670: 6c65 2069 7320 746f 2062 6520 7072 6f76  le is to be prov
-00001680: 6964 6564 3a0a 0a60 6060 6261 7368 0a70  ided:..```bash.p
-00001690: 7974 686f 6e20 746f 6f6c 732f 7472 6169  ython tools/trai
-000016a0: 6e2e 7079 202d 2d63 6f6e 6669 6720 3c70  n.py --config <p
-000016b0: 6174 682f 746f 2f6d 6f64 656c 2f63 6f6e  ath/to/model/con
-000016c0: 6669 672e 7961 6d6c 3e0a 6060 600a 0a46  fig.yaml>.```..F
-000016d0: 6f72 2065 7861 6d70 6c65 2c20 746f 2074  or example, to t
-000016e0: 7261 696e 205b 5041 4449 4d5d 2861 6e6f  rain [PADIM](ano
-000016f0: 6d61 6c69 622f 6d6f 6465 6c73 2f70 6164  malib/models/pad
-00001700: 696d 2920 796f 7520 6361 6e20 7573 650a  im) you can use.
-00001710: 0a60 6060 6261 7368 0a70 7974 686f 6e20  .```bash.python 
-00001720: 746f 6f6c 732f 7472 6169 6e2e 7079 202d  tools/train.py -
-00001730: 2d63 6f6e 6669 6720 616e 6f6d 616c 6962  -config anomalib
-00001740: 2f6d 6f64 656c 732f 7061 6469 6d2f 636f  /models/padim/co
-00001750: 6e66 6967 2e79 616d 6c0a 6060 600a 0a41  nfig.yaml.```..A
-00001760: 6c74 6572 6e61 7469 7665 6c79 2c20 6120  lternatively, a 
-00001770: 6d6f 6465 6c20 6e61 6d65 2063 6f75 6c64  model name could
-00001780: 2061 6c73 6f20 6265 2070 726f 7669 6465   also be provide
-00001790: 6420 6173 2061 6e20 6172 6775 6d65 6e74  d as an argument
-000017a0: 2c20 7768 6572 6520 7468 6520 7363 7269  , where the scri
-000017b0: 7074 7320 6175 746f 6d61 7469 6361 6c6c  pts automaticall
-000017c0: 7920 6669 6e64 7320 7468 6520 636f 7272  y finds the corr
-000017d0: 6573 706f 6e64 696e 6720 636f 6e66 6967  esponding config
-000017e0: 2066 696c 652e 0a0a 6060 6062 6173 680a   file...```bash.
-000017f0: 7079 7468 6f6e 2074 6f6f 6c73 2f74 7261  python tools/tra
-00001800: 696e 2e70 7920 2d2d 6d6f 6465 6c20 7061  in.py --model pa
-00001810: 6469 6d0a 6060 600a 0a77 6865 7265 2074  dim.```..where t
-00001820: 6865 2063 7572 7265 6e74 6c79 2061 7661  he currently ava
-00001830: 696c 6162 6c65 206d 6f64 656c 7320 6172  ilable models ar
-00001840: 653a 0a0a 2d20 5b43 4641 5d28 616e 6f6d  e:..- [CFA](anom
-00001850: 616c 6962 2f6d 6f64 656c 732f 6366 6129  alib/models/cfa)
-00001860: 0a2d 205b 4346 6c6f 775d 2861 6e6f 6d61  .- [CFlow](anoma
-00001870: 6c69 622f 6d6f 6465 6c73 2f63 666c 6f77  lib/models/cflow
-00001880: 290a 2d20 5b44 464b 4445 5d28 616e 6f6d  ).- [DFKDE](anom
-00001890: 616c 6962 2f6d 6f64 656c 732f 6466 6b64  alib/models/dfkd
-000018a0: 6529 0a2d 205b 4446 4d5d 2861 6e6f 6d61  e).- [DFM](anoma
-000018b0: 6c69 622f 6d6f 6465 6c73 2f64 666d 290a  lib/models/dfm).
-000018c0: 2d20 5b44 5241 454d 5d28 616e 6f6d 616c  - [DRAEM](anomal
-000018d0: 6962 2f6d 6f64 656c 732f 6472 6165 6d29  ib/models/draem)
-000018e0: 0a2d 205b 4661 7374 466c 6f77 5d28 616e  .- [FastFlow](an
-000018f0: 6f6d 616c 6962 2f6d 6f64 656c 732f 6661  omalib/models/fa
-00001900: 7374 666c 6f77 290a 2d20 5b47 414e 6f6d  stflow).- [GANom
-00001910: 616c 795d 2861 6e6f 6d61 6c69 622f 6d6f  aly](anomalib/mo
-00001920: 6465 6c73 2f67 616e 6f6d 616c 7929 0a2d  dels/ganomaly).-
-00001930: 205b 5041 4449 4d5d 2861 6e6f 6d61 6c69   [PADIM](anomali
-00001940: 622f 6d6f 6465 6c73 2f70 6164 696d 290a  b/models/padim).
-00001950: 2d20 5b50 6174 6368 436f 7265 5d28 616e  - [PatchCore](an
-00001960: 6f6d 616c 6962 2f6d 6f64 656c 732f 7061  omalib/models/pa
-00001970: 7463 6863 6f72 6529 0a2d 205b 5265 7665  tchcore).- [Reve
-00001980: 7273 6520 4469 7374 696c 6c61 7469 6f6e  rse Distillation
-00001990: 5d28 616e 6f6d 616c 6962 2f6d 6f64 656c  ](anomalib/model
-000019a0: 732f 7265 7665 7273 655f 6469 7374 696c  s/reverse_distil
-000019b0: 6c61 7469 6f6e 290a 2d20 5b53 5446 504d  lation).- [STFPM
-000019c0: 5d28 616e 6f6d 616c 6962 2f6d 6f64 656c  ](anomalib/model
-000019d0: 732f 7374 6670 6d29 0a0a 2323 2046 6561  s/stfpm)..## Fea
-000019e0: 7475 7265 2065 7874 7261 6374 696f 6e20  ture extraction 
-000019f0: 2620 2870 7265 2d74 7261 696e 6564 2920  & (pre-trained) 
-00001a00: 6261 636b 626f 6e65 730a 0a54 6865 2070  backbones..The p
-00001a10: 7265 2d74 7261 696e 6564 2062 6163 6b62  re-trained backb
-00001a20: 6f6e 6573 2063 6f6d 6520 6672 6f6d 205b  ones come from [
-00001a30: 5079 546f 7263 6820 496d 6167 6520 4d6f  PyTorch Image Mo
-00001a40: 6465 6c73 2028 7469 6d6d 295d 2868 7474  dels (timm)](htt
-00001a50: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001a60: 7277 6967 6874 6d61 6e2f 7079 746f 7263  rwightman/pytorc
-00001a70: 682d 696d 6167 652d 6d6f 6465 6c73 292c  h-image-models),
-00001a80: 2077 6869 6368 2061 7265 2077 7261 7070   which are wrapp
-00001a90: 6564 2062 7920 6046 6561 7475 7265 4578  ed by `FeatureEx
-00001aa0: 7472 6163 746f 7260 2e0a 0a46 6f72 206d  tractor`...For m
-00001ab0: 6f72 6520 696e 666f 726d 6174 696f 6e2c  ore information,
-00001ac0: 2070 6c65 6173 6520 6368 6563 6b20 6f75   please check ou
-00001ad0: 7220 646f 6375 6d65 6e74 6174 696f 6e20  r documentation 
-00001ae0: 6f72 2074 6865 205b 7365 6374 696f 6e20  or the [section 
-00001af0: 6162 6f75 7420 6665 6174 7572 6520 6578  about feature ex
-00001b00: 7472 6163 7469 6f6e 2069 6e20 2247 6574  traction in "Get
-00001b10: 7469 6e67 2053 7461 7274 6564 2077 6974  ting Started wit
-00001b20: 6820 5079 546f 7263 6820 496d 6167 6520  h PyTorch Image 
-00001b30: 4d6f 6465 6c73 2028 7469 6d6d 293a 2041  Models (timm): A
-00001b40: 2050 7261 6374 6974 696f 6e65 72e2 8099   Practitioner...
-00001b50: 7320 4775 6964 6522 5d28 6874 7470 733a  s Guide"](https:
-00001b60: 2f2f 746f 7761 7264 7364 6174 6173 6369  //towardsdatasci
-00001b70: 656e 6365 2e63 6f6d 2f67 6574 7469 6e67  ence.com/getting
-00001b80: 2d73 7461 7274 6564 2d77 6974 682d 7079  -started-with-py
-00001b90: 746f 7263 682d 696d 6167 652d 6d6f 6465  torch-image-mode
-00001ba0: 6c73 2d74 696d 6d2d 612d 7072 6163 7469  ls-timm-a-practi
-00001bb0: 7469 6f6e 6572 732d 6775 6964 652d 3465  tioners-guide-4e
-00001bc0: 3737 6234 6266 3930 3535 2362 3833 623a  77b4bf9055#b83b:
-00001bd0: 7e3a 7465 7874 3d72 6561 6479 2532 3074  ~:text=ready%20t
-00001be0: 6f25 3230 7472 6169 6e21 2d2c 4665 6174  o%20train!-,Feat
-00001bf0: 7572 6525 3230 4578 7472 6163 7469 6f6e  ure%20Extraction
-00001c00: 2c2d 7469 6d6d 2532 306d 6f64 656c 7325  ,-timm%20models%
-00001c10: 3230 616c 736f 3e29 2e0a 0a54 6970 733a  20also>)...Tips:
-00001c20: 0a0a 2d20 5061 7065 7273 2057 6974 6820  ..- Papers With 
-00001c30: 436f 6465 2068 6173 2061 6e20 696e 7465  Code has an inte
-00001c40: 7266 6163 6520 746f 2065 6173 696c 7920  rface to easily 
-00001c50: 6272 6f77 7365 206d 6f64 656c 7320 6176  browse models av
-00001c60: 6169 6c61 626c 6520 696e 2074 696d 6d3a  ailable in timm:
-00001c70: 205b 6874 7470 733a 2f2f 7061 7065 7273   [https://papers
-00001c80: 7769 7468 636f 6465 2e63 6f6d 2f6c 6962  withcode.com/lib
-00001c90: 2f74 696d 6d5d 2868 7474 7073 3a2f 2f70  /timm](https://p
-00001ca0: 6170 6572 7377 6974 6863 6f64 652e 636f  aperswithcode.co
-00001cb0: 6d2f 6c69 622f 7469 6d6d 290a 0a2d 2059  m/lib/timm)..- Y
-00001cc0: 6f75 2063 616e 2061 6c73 6f20 6669 6e64  ou can also find
-00001cd0: 2074 6865 6d20 7769 7468 2074 6865 2066   them with the f
-00001ce0: 756e 6374 696f 6e20 6074 696d 6d2e 6c69  unction `timm.li
-00001cf0: 7374 5f6d 6f64 656c 7328 2272 6573 6e65  st_models("resne
-00001d00: 742a 222c 2070 7265 7472 6169 6e65 643d  t*", pretrained=
-00001d10: 5472 7565 2960 0a0a 5468 6520 6261 636b  True)`..The back
-00001d20: 626f 6e65 2063 616e 2062 6520 7365 7420  bone can be set 
-00001d30: 696e 2074 6865 2063 6f6e 6669 6720 6669  in the config fi
-00001d40: 6c65 2c20 7477 6f20 6578 616d 706c 6573  le, two examples
-00001d50: 2062 656c 6f77 2e0a 0a60 6060 7961 6d6c   below...```yaml
-00001d60: 0a6d 6f64 656c 3a0a 2020 6e61 6d65 3a20  .model:.  name: 
-00001d70: 6366 6c6f 770a 2020 6261 636b 626f 6e65  cflow.  backbone
-00001d80: 3a20 7769 6465 5f72 6573 6e65 7435 305f  : wide_resnet50_
-00001d90: 320a 2020 7072 655f 7472 6169 6e65 643a  2.  pre_trained:
-00001da0: 2074 7275 650a 6060 600a 0a23 2320 4375   true.```..## Cu
-00001db0: 7374 6f6d 2044 6174 6173 6574 0a0a 4974  stom Dataset..It
-00001dc0: 2069 7320 616c 736f 2070 6f73 7369 626c   is also possibl
-00001dd0: 6520 746f 2074 7261 696e 206f 6e20 6120  e to train on a 
-00001de0: 6375 7374 6f6d 2066 6f6c 6465 7220 6461  custom folder da
-00001df0: 7461 7365 742e 2054 6f20 646f 2073 6f2c  taset. To do so,
-00001e00: 2060 6461 7461 6020 7365 6374 696f 6e20   `data` section 
-00001e10: 696e 2060 636f 6e66 6967 2e79 616d 6c60  in `config.yaml`
-00001e20: 2069 7320 746f 2062 6520 6d6f 6469 6669   is to be modifi
-00001e30: 6564 2061 7320 666f 6c6c 6f77 733a 0a0a  ed as follows:..
-00001e40: 6060 6079 616d 6c0a 6461 7461 7365 743a  ```yaml.dataset:
-00001e50: 0a20 206e 616d 653a 203c 6e61 6d65 2d6f  .  name: <name-o
-00001e60: 662d 7468 652d 6461 7461 7365 743e 0a20  f-the-dataset>. 
-00001e70: 2066 6f72 6d61 743a 2066 6f6c 6465 720a   format: folder.
-00001e80: 2020 7061 7468 3a20 3c70 6174 682f 746f    path: <path/to
-00001e90: 2f66 6f6c 6465 722f 6461 7461 7365 743e  /folder/dataset>
-00001ea0: 0a20 206e 6f72 6d61 6c5f 6469 723a 206e  .  normal_dir: n
-00001eb0: 6f72 6d61 6c20 2320 6e61 6d65 206f 6620  ormal # name of 
-00001ec0: 7468 6520 666f 6c64 6572 2063 6f6e 7461  the folder conta
-00001ed0: 696e 696e 6720 6e6f 726d 616c 2069 6d61  ining normal ima
-00001ee0: 6765 732e 0a20 2061 626e 6f72 6d61 6c5f  ges..  abnormal_
-00001ef0: 6469 723a 2061 626e 6f72 6d61 6c20 2320  dir: abnormal # 
-00001f00: 6e61 6d65 206f 6620 7468 6520 666f 6c64  name of the fold
-00001f10: 6572 2063 6f6e 7461 696e 696e 6720 6162  er containing ab
-00001f20: 6e6f 726d 616c 2069 6d61 6765 732e 0a20  normal images.. 
-00001f30: 206e 6f72 6d61 6c5f 7465 7374 5f64 6972   normal_test_dir
-00001f40: 3a20 6e75 6c6c 2023 206e 616d 6520 6f66  : null # name of
-00001f50: 2074 6865 2066 6f6c 6465 7220 636f 6e74   the folder cont
-00001f60: 6169 6e69 6e67 206e 6f72 6d61 6c20 7465  aining normal te
-00001f70: 7374 2069 6d61 6765 732e 0a20 2074 6173  st images..  tas
-00001f80: 6b3a 2073 6567 6d65 6e74 6174 696f 6e20  k: segmentation 
-00001f90: 2320 636c 6173 7369 6669 6361 7469 6f6e  # classification
-00001fa0: 206f 7220 7365 676d 656e 7461 7469 6f6e   or segmentation
-00001fb0: 0a20 206d 6173 6b3a 203c 7061 7468 2f74  .  mask: <path/t
-00001fc0: 6f2f 6d61 736b 2f61 6e6e 6f74 6174 696f  o/mask/annotatio
-00001fd0: 6e73 3e20 236f 7074 696f 6e61 6c0a 2020  ns> #optional.  
-00001fe0: 6578 7465 6e73 696f 6e73 3a20 6e75 6c6c  extensions: null
-00001ff0: 0a20 2073 706c 6974 5f72 6174 696f 3a20  .  split_ratio: 
-00002000: 302e 3220 2320 7261 7469 6f20 6f66 2074  0.2 # ratio of t
-00002010: 6865 206e 6f72 6d61 6c20 696d 6167 6573  he normal images
-00002020: 2074 6861 7420 7769 6c6c 2062 6520 7573   that will be us
-00002030: 6564 2074 6f20 6372 6561 7465 2061 2074  ed to create a t
-00002040: 6573 7420 7370 6c69 740a 2020 696d 6167  est split.  imag
-00002050: 655f 7369 7a65 3a20 3235 360a 2020 7472  e_size: 256.  tr
-00002060: 6169 6e5f 6261 7463 685f 7369 7a65 3a20  ain_batch_size: 
-00002070: 3332 0a20 2074 6573 745f 6261 7463 685f  32.  test_batch_
-00002080: 7369 7a65 3a20 3332 0a20 206e 756d 5f77  size: 32.  num_w
-00002090: 6f72 6b65 7273 3a20 380a 2020 7472 616e  orkers: 8.  tran
-000020a0: 7366 6f72 6d5f 636f 6e66 6967 3a0a 2020  sform_config:.  
-000020b0: 2020 7472 6169 6e3a 206e 756c 6c0a 2020    train: null.  
-000020c0: 2020 7661 6c3a 206e 756c 6c0a 2020 6372    val: null.  cr
-000020d0: 6561 7465 5f76 616c 6964 6174 696f 6e5f  eate_validation_
-000020e0: 7365 743a 2074 7275 650a 2020 7469 6c69  set: true.  tili
-000020f0: 6e67 3a0a 2020 2020 6170 706c 793a 2066  ng:.    apply: f
-00002100: 616c 7365 0a20 2020 2074 696c 655f 7369  alse.    tile_si
-00002110: 7a65 3a20 6e75 6c6c 0a20 2020 2073 7472  ze: null.    str
-00002120: 6964 653a 206e 756c 6c0a 2020 2020 7265  ide: null.    re
-00002130: 6d6f 7665 5f62 6f72 6465 725f 636f 756e  move_border_coun
-00002140: 743a 2030 0a20 2020 2075 7365 5f72 616e  t: 0.    use_ran
-00002150: 646f 6d5f 7469 6c69 6e67 3a20 4661 6c73  dom_tiling: Fals
-00002160: 650a 2020 2020 7261 6e64 6f6d 5f74 696c  e.    random_til
-00002170: 655f 636f 756e 743a 2031 360a 6060 600a  e_count: 16.```.
-00002180: 0a23 2049 6e66 6572 656e 6365 0a0a 416e  .# Inference..An
-00002190: 6f6d 616c 6962 2069 6e63 6c75 6465 7320  omalib includes 
-000021a0: 6d75 6c74 6970 6c65 2074 6f6f 6c73 2c20  multiple tools, 
-000021b0: 696e 636c 7564 696e 6720 4c69 6768 746e  including Lightn
-000021c0: 696e 672c 2047 7261 6469 6f2c 2061 6e64  ing, Gradio, and
-000021d0: 204f 7065 6e56 494e 4f20 696e 6665 7265   OpenVINO infere
-000021e0: 6e63 6572 732c 2066 6f72 2070 6572 666f  ncers, for perfo
-000021f0: 726d 696e 6720 696e 6665 7265 6e63 6520  rming inference 
-00002200: 7769 7468 2061 2074 7261 696e 6564 206d  with a trained m
-00002210: 6f64 656c 2e0a 0a54 6865 2066 6f6c 6c6f  odel...The follo
-00002220: 7769 6e67 2063 6f6d 6d61 6e64 2063 616e  wing command can
-00002230: 2062 6520 7573 6564 2074 6f20 7275 6e20   be used to run 
-00002240: 5079 546f 7263 6820 4c69 6768 746e 696e  PyTorch Lightnin
-00002250: 6720 696e 6665 7265 6e63 6520 6672 6f6d  g inference from
-00002260: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
-00002270: 653a 0a0a 6060 6062 6173 680a 7079 7468  e:..```bash.pyth
-00002280: 6f6e 2074 6f6f 6c73 2f69 6e66 6572 656e  on tools/inferen
-00002290: 6365 2f6c 6967 6874 6e69 6e67 5f69 6e66  ce/lightning_inf
-000022a0: 6572 656e 6365 2e70 7920 2d68 0a60 6060  erence.py -h.```
-000022b0: 0a0a 4173 2061 2071 7569 636b 2065 7861  ..As a quick exa
-000022c0: 6d70 6c65 3a0a 0a60 6060 6261 7368 0a70  mple:..```bash.p
-000022d0: 7974 686f 6e20 746f 6f6c 732f 696e 6665  ython tools/infe
-000022e0: 7265 6e63 652f 6c69 6768 746e 696e 675f  rence/lightning_
-000022f0: 696e 6665 7265 6e63 652e 7079 205c 0a20  inference.py \. 
-00002300: 2020 202d 2d63 6f6e 6669 6720 616e 6f6d     --config anom
-00002310: 616c 6962 2f6d 6f64 656c 732f 7061 6469  alib/models/padi
-00002320: 6d2f 636f 6e66 6967 2e79 616d 6c20 5c0a  m/config.yaml \.
-00002330: 2020 2020 2d2d 7765 6967 6874 7320 7265      --weights re
-00002340: 7375 6c74 732f 7061 6469 6d2f 6d76 7465  sults/padim/mvte
-00002350: 632f 626f 7474 6c65 2f77 6569 6768 7473  c/bottle/weights
-00002360: 2f6d 6f64 656c 2e63 6b70 7420 5c0a 2020  /model.ckpt \.  
-00002370: 2020 2d2d 696e 7075 7420 6461 7461 7365    --input datase
-00002380: 7473 2f4d 5654 6563 2f62 6f74 746c 652f  ts/MVTec/bottle/
-00002390: 7465 7374 2f62 726f 6b65 6e5f 6c61 7267  test/broken_larg
-000023a0: 652f 3030 302e 706e 6720 5c0a 2020 2020  e/000.png \.    
-000023b0: 2d2d 6f75 7470 7574 2072 6573 756c 7473  --output results
-000023c0: 2f70 6164 696d 2f6d 7674 6563 2f62 6f74  /padim/mvtec/bot
-000023d0: 746c 652f 696d 6167 6573 0a60 6060 0a0a  tle/images.```..
-000023e0: 4578 616d 706c 6520 4f70 656e 5649 4e4f  Example OpenVINO
-000023f0: 2049 6e66 6572 656e 6365 3a0a 0a60 6060   Inference:..```
-00002400: 6261 7368 0a70 7974 686f 6e20 746f 6f6c  bash.python tool
-00002410: 732f 696e 6665 7265 6e63 652f 6f70 656e  s/inference/open
-00002420: 7669 6e6f 5f69 6e66 6572 656e 6365 2e70  vino_inference.p
-00002430: 7920 5c0a 2020 2020 2d2d 636f 6e66 6967  y \.    --config
-00002440: 2061 6e6f 6d61 6c69 622f 6d6f 6465 6c73   anomalib/models
-00002450: 2f70 6164 696d 2f63 6f6e 6669 672e 7961  /padim/config.ya
-00002460: 6d6c 205c 0a20 2020 202d 2d77 6569 6768  ml \.    --weigh
-00002470: 7473 2072 6573 756c 7473 2f70 6164 696d  ts results/padim
-00002480: 2f6d 7674 6563 2f62 6f74 746c 652f 6f70  /mvtec/bottle/op
-00002490: 656e 7669 6e6f 2f6f 7065 6e76 696e 6f5f  envino/openvino_
-000024a0: 6d6f 6465 6c2e 6269 6e20 5c0a 2020 2020  model.bin \.    
-000024b0: 2d2d 6d65 7461 5f64 6174 6120 7265 7375  --meta_data resu
-000024c0: 6c74 732f 7061 6469 6d2f 6d76 7465 632f  lts/padim/mvtec/
-000024d0: 626f 7474 6c65 2f6f 7065 6e76 696e 6f2f  bottle/openvino/
-000024e0: 6d65 7461 5f64 6174 612e 6a73 6f6e 205c  meta_data.json \
-000024f0: 0a20 2020 202d 2d69 6e70 7574 2064 6174  .    --input dat
-00002500: 6173 6574 732f 4d56 5465 632f 626f 7474  asets/MVTec/bott
-00002510: 6c65 2f74 6573 742f 6272 6f6b 656e 5f6c  le/test/broken_l
-00002520: 6172 6765 2f30 3030 2e70 6e67 205c 0a20  arge/000.png \. 
-00002530: 2020 202d 2d6f 7574 7075 7420 7265 7375     --output resu
-00002540: 6c74 732f 7061 6469 6d2f 6d76 7465 632f  lts/padim/mvtec/
-00002550: 626f 7474 6c65 2f69 6d61 6765 730a 6060  bottle/images.``
-00002560: 600a 0a3e 2045 6e73 7572 6520 7468 6174  `..> Ensure that
-00002570: 2079 6f75 2070 726f 7669 6465 2070 6174   you provide pat
-00002580: 6820 746f 2060 6d65 7461 5f64 6174 612e  h to `meta_data.
-00002590: 6a73 6f6e 6020 6966 2079 6f75 2077 616e  json` if you wan
-000025a0: 7420 7468 6520 6e6f 726d 616c 697a 6174  t the normalizat
-000025b0: 696f 6e20 746f 2062 6520 6170 706c 6965  ion to be applie
-000025c0: 6420 636f 7272 6563 746c 792e 0a0a 596f  d correctly...Yo
-000025d0: 7520 6361 6e20 616c 736f 2075 7365 2047  u can also use G
-000025e0: 7261 6469 6f20 496e 6665 7265 6e63 6520  radio Inference 
-000025f0: 746f 2069 6e74 6572 6163 7420 7769 7468  to interact with
-00002600: 2074 6865 2074 7261 696e 6564 206d 6f64   the trained mod
-00002610: 656c 7320 7573 696e 6720 6120 5549 2e20  els using a UI. 
-00002620: 5265 6665 7220 746f 206f 7572 205b 6775  Refer to our [gu
-00002630: 6964 655d 2868 7474 7073 3a2f 2f6f 7065  ide](https://ope
-00002640: 6e76 696e 6f74 6f6f 6c6b 6974 2e67 6974  nvinotoolkit.git
-00002650: 6875 622e 696f 2f61 6e6f 6d61 6c69 622f  hub.io/anomalib/
-00002660: 6775 6964 6573 2f69 6e66 6572 656e 6365  guides/inference
-00002670: 2e68 746d 6c23 6772 6164 696f 2d69 6e66  .html#gradio-inf
-00002680: 6572 656e 6365 2920 666f 7220 6d6f 7265  erence) for more
-00002690: 2064 6574 6169 6c73 2e0a 0a41 2071 7569   details...A qui
-000026a0: 636b 2065 7861 6d70 6c65 3a0a 0a60 6060  ck example:..```
-000026b0: 6261 7368 0a70 7974 686f 6e20 746f 6f6c  bash.python tool
-000026c0: 732f 696e 6665 7265 6e63 652f 6772 6164  s/inference/grad
-000026d0: 696f 5f69 6e66 6572 656e 6365 2e70 7920  io_inference.py 
-000026e0: 5c0a 2020 2020 2020 2020 2d2d 636f 6e66  \.        --conf
-000026f0: 6967 202e 2f61 6e6f 6d61 6c69 622f 6d6f  ig ./anomalib/mo
-00002700: 6465 6c73 2f70 6164 696d 2f63 6f6e 6669  dels/padim/confi
-00002710: 672e 7961 6d6c 205c 0a20 2020 2020 2020  g.yaml \.       
-00002720: 202d 2d77 6569 6768 7473 202e 2f72 6573   --weights ./res
-00002730: 756c 7473 2f70 6164 696d 2f6d 7674 6563  ults/padim/mvtec
-00002740: 2f62 6f74 746c 652f 7765 6967 6874 732f  /bottle/weights/
-00002750: 6d6f 6465 6c2e 636b 7074 0a60 6060 0a0a  model.ckpt.```..
-00002760: 2323 2045 7870 6f72 7469 6e67 204d 6f64  ## Exporting Mod
-00002770: 656c 2074 6f20 4f4e 4e58 206f 7220 4f70  el to ONNX or Op
-00002780: 656e 5649 4e4f 2049 520a 0a49 7420 6973  enVINO IR..It is
-00002790: 2070 6f73 7369 626c 6520 746f 2065 7870   possible to exp
-000027a0: 6f72 7420 796f 7572 206d 6f64 656c 2074  ort your model t
-000027b0: 6f20 4f4e 4e58 206f 7220 4f70 656e 5649  o ONNX or OpenVI
-000027c0: 4e4f 2049 520a 0a49 6620 796f 7520 7761  NO IR..If you wa
-000027d0: 6e74 2074 6f20 6578 706f 7274 2079 6f75  nt to export you
-000027e0: 7220 5079 546f 7263 6820 6d6f 6465 6c20  r PyTorch model 
-000027f0: 746f 2061 6e20 4f70 656e 5649 4e4f 206d  to an OpenVINO m
-00002800: 6f64 656c 2c20 656e 7375 7265 2074 6861  odel, ensure tha
-00002810: 7420 6065 7870 6f72 745f 6d6f 6465 6020  t `export_mode` 
-00002820: 6973 2073 6574 2074 6f20 6022 6f70 656e  is set to `"open
-00002830: 7669 6e6f 2260 2069 6e20 7468 6520 7265  vino"` in the re
-00002840: 7370 6563 7469 7665 206d 6f64 656c 2060  spective model `
-00002850: 636f 6e66 6967 2e79 616d 6c60 2e0a 0a60  config.yaml`...`
-00002860: 6060 7961 6d6c 0a6f 7074 696d 697a 6174  ``yaml.optimizat
-00002870: 696f 6e3a 0a20 2065 7870 6f72 745f 6d6f  ion:.  export_mo
-00002880: 6465 3a20 226f 7065 6e76 696e 6f22 2023  de: "openvino" #
-00002890: 206f 7074 696f 6e73 3a20 6f70 656e 7669   options: openvi
-000028a0: 6e6f 2c20 6f6e 6e78 0a60 6060 0a0a 2320  no, onnx.```..# 
-000028b0: 4879 7065 7270 6172 616d 6574 6572 204f  Hyperparameter O
-000028c0: 7074 696d 697a 6174 696f 6e0a 0a54 6f20  ptimization..To 
-000028d0: 7275 6e20 6879 7065 7270 6172 616d 6574  run hyperparamet
-000028e0: 6572 206f 7074 696d 697a 6174 696f 6e2c  er optimization,
-000028f0: 2075 7365 2074 6865 2066 6f6c 6c6f 7769   use the followi
-00002900: 6e67 2063 6f6d 6d61 6e64 3a0a 0a60 6060  ng command:..```
-00002910: 6261 7368 0a70 7974 686f 6e20 746f 6f6c  bash.python tool
-00002920: 732f 6870 6f2f 7377 6565 702e 7079 205c  s/hpo/sweep.py \
-00002930: 0a20 2020 202d 2d6d 6f64 656c 2070 6164  .    --model pad
-00002940: 696d 202d 2d6d 6f64 656c 5f63 6f6e 6669  im --model_confi
-00002950: 6720 2e2f 7061 7468 5f74 6f5f 636f 6e66  g ./path_to_conf
-00002960: 6967 2e79 616d 6c20 5c0a 2020 2020 2d2d  ig.yaml \.    --
-00002970: 7377 6565 705f 636f 6e66 6967 2074 6f6f  sweep_config too
-00002980: 6c73 2f68 706f 2f73 7765 6570 2e79 616d  ls/hpo/sweep.yam
-00002990: 6c0a 6060 600a 0a46 6f72 206d 6f72 6520  l.```..For more 
-000029a0: 6465 7461 696c 7320 7265 6665 7220 7468  details refer th
-000029b0: 6520 5b48 504f 2044 6f63 756d 656e 7461  e [HPO Documenta
-000029c0: 7469 6f6e 5d28 6874 7470 733a 2f2f 6f70  tion](https://op
-000029d0: 656e 7669 6e6f 746f 6f6c 6b69 742e 6769  envinotoolkit.gi
-000029e0: 7468 7562 2e69 6f2f 616e 6f6d 616c 6962  thub.io/anomalib
-000029f0: 2f67 7569 6465 732f 6879 7065 7270 6172  /guides/hyperpar
-00002a00: 616d 6574 6572 5f6f 7074 696d 697a 6174  ameter_optimizat
-00002a10: 696f 6e2e 6874 6d6c 290a 0a23 2042 656e  ion.html)..# Ben
-00002a20: 6368 6d61 726b 696e 670a 0a54 6f20 6761  chmarking..To ga
-00002a30: 7468 6572 2062 656e 6368 6d61 726b 696e  ther benchmarkin
-00002a40: 6720 6461 7461 2073 7563 6820 6173 2074  g data such as t
-00002a50: 6872 6f75 6768 7075 7420 6163 726f 7373  hroughput across
-00002a60: 2063 6174 6567 6f72 6965 732c 2075 7365   categories, use
-00002a70: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00002a80: 6f6d 6d61 6e64 3a0a 0a60 6060 6261 7368  ommand:..```bash
-00002a90: 0a70 7974 686f 6e20 746f 6f6c 732f 6265  .python tools/be
-00002aa0: 6e63 686d 6172 6b69 6e67 2f62 656e 6368  nchmarking/bench
-00002ab0: 6d61 726b 2e70 7920 5c0a 2020 2020 2d2d  mark.py \.    --
-00002ac0: 636f 6e66 6967 203c 7265 6c61 7469 7665  config <relative
-00002ad0: 2f61 6273 6f6c 7574 6520 7061 7468 3e2f  /absolute path>/
-00002ae0: 3c70 6172 616d 6669 6c65 3e2e 7961 6d6c  <paramfile>.yaml
-00002af0: 0a60 6060 0a0a 5265 6665 7220 746f 2074  .```..Refer to t
-00002b00: 6865 205b 4265 6e63 686d 6172 6b69 6e67  he [Benchmarking
-00002b10: 2044 6f63 756d 656e 7461 7469 6f6e 5d28   Documentation](
-00002b20: 6874 7470 733a 2f2f 6f70 656e 7669 6e6f  https://openvino
-00002b30: 746f 6f6c 6b69 742e 6769 7468 7562 2e69  toolkit.github.i
-00002b40: 6f2f 616e 6f6d 616c 6962 2f67 7569 6465  o/anomalib/guide
-00002b50: 732f 6265 6e63 686d 6172 6b69 6e67 2e68  s/benchmarking.h
-00002b60: 746d 6c29 2066 6f72 206d 6f72 6520 6465  tml) for more de
-00002b70: 7461 696c 732e 0a0a 2320 4578 7065 7269  tails...# Experi
-00002b80: 6d65 6e74 204d 616e 6167 656d 656e 740a  ment Management.
-00002b90: 0a41 6e6f 6d61 626c 6962 2069 7320 696e  .Anomablib is in
-00002ba0: 7465 6772 6174 6564 2077 6974 6820 7661  tegrated with va
-00002bb0: 7269 6f75 7320 6c69 6272 6172 6965 7320  rious libraries 
-00002bc0: 666f 7220 6578 7065 7269 6d65 6e74 2074  for experiment t
-00002bd0: 7261 636b 696e 6720 7375 6368 2061 7320  racking such as 
-00002be0: 436f 6d65 742c 2074 656e 736f 7262 6f61  Comet, tensorboa
-00002bf0: 7264 2c20 616e 6420 7761 6e64 6220 7468  rd, and wandb th
-00002c00: 726f 7567 6820 5b70 7974 6f72 6368 206c  rough [pytorch l
-00002c10: 6967 6874 696e 6720 6c6f 6767 6572 735d  ighting loggers]
-00002c20: 2868 7474 7073 3a2f 2f70 7974 6f72 6368  (https://pytorch
-00002c30: 2d6c 6967 6874 6e69 6e67 2e72 6561 6474  -lightning.readt
-00002c40: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
-00002c50: 626c 652f 6578 7465 6e73 696f 6e73 2f6c  ble/extensions/l
-00002c60: 6f67 6769 6e67 2e68 746d 6c29 2e0a 0a42  ogging.html)...B
-00002c70: 656c 6f77 2069 7320 616e 2065 7861 6d70  elow is an examp
-00002c80: 6c65 206f 6620 686f 7720 746f 2065 6e61  le of how to ena
-00002c90: 626c 6520 6c6f 6767 696e 6720 666f 7220  ble logging for 
-00002ca0: 6879 7065 722d 7061 7261 6d65 7465 7273  hyper-parameters
-00002cb0: 2c20 6d65 7472 6963 732c 206d 6f64 656c  , metrics, model
-00002cc0: 2067 7261 7068 732c 2061 6e64 2070 7265   graphs, and pre
-00002cd0: 6469 6374 696f 6e73 206f 6e20 696d 6167  dictions on imag
-00002ce0: 6573 2069 6e20 7468 6520 7465 7374 2064  es in the test d
-00002cf0: 6174 612d 7365 740a 0a60 6060 7961 6d6c  ata-set..```yaml
-00002d00: 0a76 6973 7561 6c69 7a61 7469 6f6e 3a0a  .visualization:.
-00002d10: 2020 6c6f 675f 696d 6167 6573 3a20 5472    log_images: Tr
-00002d20: 7565 2023 206c 6f67 2069 6d61 6765 7320  ue # log images 
-00002d30: 746f 2074 6865 2061 7661 696c 6162 6c65  to the available
-00002d40: 206c 6f67 6765 7273 2028 6966 2061 6e79   loggers (if any
-00002d50: 290a 2020 6d6f 6465 3a20 6675 6c6c 2023  ).  mode: full #
-00002d60: 206f 7074 696f 6e73 3a20 5b22 6675 6c6c   options: ["full
-00002d70: 222c 2022 7369 6d70 6c65 225d 0a0a 206c  ", "simple"].. l
-00002d80: 6f67 6769 6e67 3a0a 2020 6c6f 6767 6572  ogging:.  logger
-00002d90: 3a20 5b63 6f6d 6574 2c20 7465 6e73 6f72  : [comet, tensor
-00002da0: 626f 6172 642c 2077 616e 6462 5d0a 2020  board, wandb].  
-00002db0: 6c6f 675f 6772 6170 683a 2054 7275 650a  log_graph: True.
-00002dc0: 6060 600a 0a46 6f72 206d 6f72 6520 696e  ```..For more in
-00002dd0: 666f 726d 6174 696f 6e2c 2072 6566 6572  formation, refer
-00002de0: 2074 6f20 7468 6520 5b4c 6f67 6769 6e67   to the [Logging
-00002df0: 2044 6f63 756d 656e 7461 7469 6f6e 5d28   Documentation](
-00002e00: 6874 7470 733a 2f2f 6f70 656e 7669 6e6f  https://openvino
-00002e10: 746f 6f6c 6b69 742e 6769 7468 7562 2e69  toolkit.github.i
-00002e20: 6f2f 616e 6f6d 616c 6962 2f67 7569 6465  o/anomalib/guide
-00002e30: 732f 6c6f 6767 696e 672e 6874 6d6c 290a  s/logging.html).
-00002e40: 0a4e 6f74 653a 2053 6574 2079 6f75 7220  .Note: Set your 
-00002e50: 4150 4920 4b65 7920 666f 7220 5b43 6f6d  API Key for [Com
-00002e60: 6574 2e6d 6c5d 2868 7474 7073 3a2f 2f77  et.ml](https://w
-00002e70: 7777 2e63 6f6d 6574 2e63 6f6d 2f73 6967  ww.comet.com/sig
-00002e80: 6e75 703f 7574 6d5f 736f 7572 6365 3d61  nup?utm_source=a
-00002e90: 6e6f 6d61 6c69 6226 7574 6d5f 6d65 6469  nomalib&utm_medi
-00002ea0: 756d 3d72 6566 6572 7261 6c29 2076 6961  um=referral) via
-00002eb0: 2060 636f 6d65 745f 6d6c 2e69 6e69 7428   `comet_ml.init(
-00002ec0: 2960 2069 6e20 696e 7465 7261 6374 6976  )` in interactiv
-00002ed0: 6520 7079 7468 6f6e 206f 7220 7369 6d70  e python or simp
-00002ee0: 6c79 2072 756e 2060 6578 706f 7274 2043  ly run `export C
-00002ef0: 4f4d 4554 5f41 5049 5f4b 4559 3d3c 596f  OMET_API_KEY=<Yo
-00002f00: 7572 2041 5049 204b 6579 3e60 0a0a 2320  ur API Key>`..# 
-00002f10: 436f 6d6d 756e 6974 7920 5072 6f6a 6563  Community Projec
-00002f20: 7473 0a0a 2323 2031 2e20 5765 622d 6261  ts..## 1. Web-ba
-00002f30: 7365 6420 5069 7065 6c69 6e65 2066 6f72  sed Pipeline for
-00002f40: 2054 7261 696e 696e 6720 616e 6420 496e   Training and In
-00002f50: 6665 7265 6e63 650a 0a54 6869 7320 7072  ference..This pr
-00002f60: 6f6a 6563 7420 7368 6f77 6361 7365 7320  oject showcases 
-00002f70: 616e 2065 6e64 2d74 6f2d 656e 6420 7472  an end-to-end tr
-00002f80: 6169 6e69 6e67 2061 6e64 2069 6e66 6572  aining and infer
-00002f90: 656e 6365 2070 6970 656c 696e 6520 6275  ence pipeline bu
-00002fa0: 696c 6420 6f6e 2074 6f70 206f 6620 416e  ild on top of An
-00002fb0: 6f6d 616c 6962 2e20 4974 2070 726f 7669  omalib. It provi
-00002fc0: 6465 7320 6120 7765 622d 6261 7365 6420  des a web-based 
-00002fd0: 5549 2066 6f72 2075 706c 6f61 6469 6e67  UI for uploading
-00002fe0: 204d 5654 6563 2073 7479 6c65 2064 6174   MVTec style dat
-00002ff0: 6173 6574 7320 616e 6420 7472 6169 6e69  asets and traini
-00003000: 6e67 2074 6865 6d20 6f6e 2074 6865 2061  ng them on the a
-00003010: 7661 696c 6162 6c65 2041 6e6f 6d61 6c69  vailable Anomali
-00003020: 6220 6d6f 6465 6c73 2e20 4974 2061 6c73  b models. It als
-00003030: 6f20 6861 7320 7365 6374 696f 6e73 2066  o has sections f
-00003040: 6f72 2063 616c 6c69 6e67 2069 6e66 6572  or calling infer
-00003050: 656e 6365 206f 6e20 696e 6469 7669 6475  ence on individu
-00003060: 616c 2069 6d61 6765 7320 6173 2077 656c  al images as wel
-00003070: 6c20 6173 206c 6973 7469 6e67 2061 6c6c  l as listing all
-00003080: 2074 6865 2069 6d61 6765 7320 7769 7468   the images with
-00003090: 2074 6865 6972 2070 7265 6469 6374 696f   their predictio
-000030a0: 6e73 2069 6e20 7468 6520 6461 7461 6261  ns in the databa
-000030b0: 7365 2e0a 0a59 6f75 2063 616e 2076 6965  se...You can vie
-000030c0: 7720 7468 6520 7072 6f6a 6563 7420 6f6e  w the project on
-000030d0: 205b 4769 7468 7562 5d28 6874 7470 733a   [Github](https:
-000030e0: 2f2f 6769 7468 7562 2e63 6f6d 2f76 6e6b  //github.com/vnk
-000030f0: 3830 3731 2f61 6e6f 6d61 6c79 2d64 6574  8071/anomaly-det
-00003100: 6563 7469 6f6e 2d69 6e2d 696e 6475 7374  ection-in-indust
-00003110: 7279 2d6d 616e 7566 6163 7475 7269 6e67  ry-manufacturing
-00003120: 2f74 7265 652f 6d61 7374 6572 2f61 6e6f  /tree/master/ano
-00003130: 6d61 6c69 625f 636f 6e74 7269 6275 7465  malib_contribute
-00003140: 290a 466f 7220 6d6f 7265 2064 6574 6169  ).For more detai
-00003150: 6c73 2073 6565 2074 6865 205b 4469 7363  ls see the [Disc
-00003160: 7573 7369 6f6e 2066 6f72 756d 5d28 6874  ussion forum](ht
-00003170: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003180: 2f6f 7065 6e76 696e 6f74 6f6f 6c6b 6974  /openvinotoolkit
-00003190: 2f61 6e6f 6d61 6c69 622f 6469 7363 7573  /anomalib/discus
-000031a0: 7369 6f6e 732f 3733 3329 0a0a 2320 4461  sions/733)..# Da
-000031b0: 7461 7365 7473 0a0a 6061 6e6f 6d61 6c69  tasets..`anomali
-000031c0: 6260 2073 7570 706f 7274 7320 4d56 5465  b` supports MVTe
-000031d0: 6320 4144 205b 2843 4320 4259 2d4e 432d  c AD [(CC BY-NC-
-000031e0: 5341 2034 2e30 295d 2868 7474 7073 3a2f  SA 4.0)](https:/
-000031f0: 2f63 7265 6174 6976 6563 6f6d 6d6f 6e73  /creativecommons
-00003200: 2e6f 7267 2f6c 6963 656e 7365 732f 6279  .org/licenses/by
-00003210: 2d6e 632d 7361 2f34 2e30 2f29 2061 6e64  -nc-sa/4.0/) and
-00003220: 2042 6561 6e54 6563 6820 5b28 4343 2d42   BeanTech [(CC-B
-00003230: 592d 5341 295d 2868 7474 7073 3a2f 2f63  Y-SA)](https://c
-00003240: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-00003250: 7267 2f6c 6963 656e 7365 732f 6279 2d73  rg/licenses/by-s
-00003260: 612f 342e 302f 6c65 6761 6c63 6f64 6529  a/4.0/legalcode)
-00003270: 2066 6f72 2062 656e 6368 6d61 726b 696e   for benchmarkin
-00003280: 6720 616e 6420 6066 6f6c 6465 7260 2066  g and `folder` f
-00003290: 6f72 2063 7573 746f 6d20 6461 7461 7365  or custom datase
-000032a0: 7420 7472 6169 6e69 6e67 2f69 6e66 6572  t training/infer
-000032b0: 656e 6365 2e0a 0a23 2320 5b4d 5654 6563  ence...## [MVTec
-000032c0: 2041 4420 4461 7461 7365 745d 2868 7474   AD Dataset](htt
-000032d0: 7073 3a2f 2f77 7777 2e6d 7674 6563 2e63  ps://www.mvtec.c
-000032e0: 6f6d 2f63 6f6d 7061 6e79 2f72 6573 6561  om/company/resea
-000032f0: 7263 682f 6461 7461 7365 7473 2f6d 7674  rch/datasets/mvt
-00003300: 6563 2d61 6429 0a0a 4d56 5465 6320 4144  ec-ad)..MVTec AD
-00003310: 2064 6174 6173 6574 2069 7320 6f6e 6520   dataset is one 
-00003320: 6f66 2074 6865 206d 6169 6e20 6265 6e63  of the main benc
-00003330: 686d 6172 6b73 2066 6f72 2061 6e6f 6d61  hmarks for anoma
-00003340: 6c79 2064 6574 6563 7469 6f6e 2c20 616e  ly detection, an
-00003350: 6420 6973 2072 656c 6561 7365 6420 756e  d is released un
-00003360: 6465 7220 7468 650a 4372 6561 7469 7665  der the.Creative
-00003370: 2043 6f6d 6d6f 6e73 2041 7474 7269 6275   Commons Attribu
-00003380: 7469 6f6e 2d4e 6f6e 436f 6d6d 6572 6369  tion-NonCommerci
-00003390: 616c 2d53 6861 7265 416c 696b 6520 342e  al-ShareAlike 4.
-000033a0: 3020 496e 7465 726e 6174 696f 6e61 6c20  0 International 
-000033b0: 4c69 6365 6e73 6520 5b28 4343 2042 592d  License [(CC BY-
-000033c0: 4e43 2d53 4120 342e 3029 5d28 6874 7470  NC-SA 4.0)](http
-000033d0: 733a 2f2f 6372 6561 7469 7665 636f 6d6d  s://creativecomm
-000033e0: 6f6e 732e 6f72 672f 6c69 6365 6e73 6573  ons.org/licenses
-000033f0: 2f62 792d 6e63 2d73 612f 342e 302f 292e  /by-nc-sa/4.0/).
-00003400: 0a0a 3e20 4e6f 7465 3a20 5468 6573 6520  ..> Note: These 
-00003410: 6d65 7472 6963 7320 6172 6520 636f 6c6c  metrics are coll
-00003420: 6563 7465 6420 7769 7468 2069 6d61 6765  ected with image
-00003430: 2073 697a 6520 6f66 2032 3536 2061 6e64   size of 256 and
-00003440: 2073 6565 6420 6034 3260 2e20 5468 6973   seed `42`. This
-00003450: 2063 6f6d 6d6f 6e20 7365 7474 696e 6720   common setting 
-00003460: 6973 2075 7365 6420 746f 206d 616b 6520  is used to make 
-00003470: 6d6f 6465 6c20 636f 6d70 6172 6973 6f6e  model comparison
-00003480: 7320 6661 6972 2e0a 0a23 2320 496d 6167  s fair...## Imag
-00003490: 652d 4c65 7665 6c20 4155 430a 0a7c 204d  e-Level AUC..| M
-000034a0: 6f64 656c 2020 2020 2020 2020 207c 2020  odel         |  
-000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034c0: 2020 7c20 2020 2041 7667 2020 2020 7c20    |    Avg    | 
-000034d0: 2043 6172 7065 7420 2020 7c20 2020 4772   Carpet   |   Gr
-000034e0: 6964 2020 2020 7c20 204c 6561 7468 6572  id    |  Leather
-000034f0: 2020 7c20 2020 5469 6c65 2020 2020 7c20    |   Tile    | 
-00003500: 2020 576f 6f64 2020 2020 7c20 426f 7474    Wood    | Bott
-00003510: 6c65 2020 7c20 2020 4361 626c 6520 2020  le  |   Cable   
-00003520: 7c20 2043 6170 7375 6c65 2020 7c20 4861  |  Capsule  | Ha
-00003530: 7a65 6c6e 7574 207c 204d 6574 616c 204e  zelnut | Metal N
-00003540: 7574 207c 2020 2050 696c 6c20 2020 207c  ut |   Pill    |
-00003550: 2020 2053 6372 6577 2020 207c 2054 6f6f     Screw   | Too
-00003560: 7468 6272 7573 6820 7c20 5472 616e 7369  thbrush | Transi
-00003570: 7374 6f72 207c 2020 5a69 7070 6572 2020  stor |  Zipper  
-00003580: 207c 0a7c 202d 2d2d 2d2d 2d2d 2d2d 2d2d   |.| -----------
-00003590: 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d  -- | -----------
-000035a0: 2d2d 2d2d 2d2d 2d20 7c20 3a2d 2d2d 2d2d  ------- | :-----
-000035b0: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20  --: | :-------: 
-000035c0: 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d  | :-------: | :-
-000035d0: 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d  ------: | :-----
-000035e0: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20  --: | :-------: 
-000035f0: 7c20 3a2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d  | :-----: | :---
-00003600: 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d  ----: | :-------
-00003610: 3a20 7c20 3a2d 2d2d 2d2d 2d3a 207c 203a  : | :------: | :
-00003620: 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d  -------: | :----
-00003630: 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d 2d3a  ---: | :-------:
-00003640: 207c 203a 2d2d 2d2d 2d2d 2d2d 3a20 7c20   | :--------: | 
-00003650: 3a2d 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d  :--------: | :--
-00003660: 2d2d 2d2d 2d3a 207c 0a7c 202a 2a50 6174  -----: |.| **Pat
-00003670: 6368 436f 7265 2a2a 207c 202a 2a57 6964  chCore** | **Wid
-00003680: 6520 5265 734e 6574 2d35 302a 2a20 7c20  e ResNet-50** | 
-00003690: 2a2a 302e 3938 302a 2a20 7c20 2020 302e  **0.980** |   0.
-000036a0: 3938 3420 2020 7c20 2020 302e 3935 3920  984   |   0.959 
-000036b0: 2020 7c20 2020 312e 3030 3020 2020 7c20    |   1.000   | 
-000036c0: 2a2a 312e 3030 302a 2a20 7c20 2020 302e  **1.000** |   0.
-000036d0: 3938 3920 2020 7c20 2031 2e30 3030 2020  989   |  1.000  
-000036e0: 7c20 2a2a 302e 3939 302a 2a20 7c20 2a2a  | **0.990** | **
-000036f0: 302e 3938 322a 2a20 7c20 2031 2e30 3030  0.982** |  1.000
-00003700: 2020 207c 2020 2030 2e39 3934 2020 207c     |   0.994   |
-00003710: 2020 2030 2e39 3234 2020 207c 2020 2030     0.924   |   0
-00003720: 2e39 3630 2020 207c 2020 2030 2e39 3333  .960   |   0.933
-00003730: 2020 2020 7c20 2a2a 312e 3030 302a 2a20      | **1.000** 
-00003740: 207c 2020 2030 2e39 3832 2020 207c 0a7c   |   0.982   |.|
-00003750: 2050 6174 6368 436f 7265 2020 2020 207c   PatchCore     |
-00003760: 2052 6573 4e65 742d 3138 2020 2020 2020   ResNet-18      
-00003770: 2020 2020 7c20 2020 302e 3937 3320 2020      |   0.973   
-00003780: 7c20 2020 302e 3937 3020 2020 7c20 2020  |   0.970   |   
-00003790: 302e 3934 3720 2020 7c20 2020 312e 3030  0.947   |   1.00
-000037a0: 3020 2020 7c20 2020 302e 3939 3720 2020  0   |   0.997   
-000037b0: 7c20 2020 302e 3939 3720 2020 7c20 2031  |   0.997   |  1
-000037c0: 2e30 3030 2020 7c20 2020 302e 3938 3620  .000  |   0.986 
-000037d0: 2020 7c20 2020 302e 3936 3520 2020 7c20    |   0.965   | 
-000037e0: 2031 2e30 3030 2020 207c 2020 2030 2e39   1.000   |   0.9
-000037f0: 3931 2020 207c 2020 2030 2e39 3136 2020  91   |   0.916  
-00003800: 207c 202a 2a30 2e39 3433 2a2a 207c 2020   | **0.943** |  
-00003810: 2030 2e39 3331 2020 2020 7c20 2020 302e   0.931    |   0.
-00003820: 3939 3620 2020 207c 2020 2030 2e39 3533  996    |   0.953
-00003830: 2020 207c 0a7c 2043 466c 6f77 2020 2020     |.| CFlow    
-00003840: 2020 2020 207c 2057 6964 6520 5265 734e       | Wide ResN
-00003850: 6574 2d35 3020 2020 2020 7c20 2020 302e  et-50     |   0.
-00003860: 3936 3220 2020 7c20 2020 302e 3938 3620  962   |   0.986 
-00003870: 2020 7c20 2020 302e 3936 3220 2020 7c20    |   0.962   | 
-00003880: 2a2a 312e 3030 302a 2a20 7c20 2020 302e  **1.000** |   0.
-00003890: 3939 3920 2020 7c20 2020 302e 3939 3320  999   |   0.993 
-000038a0: 2020 7c20 2a2a 312e 302a 2a20 7c20 2020    | **1.0** |   
-000038b0: 302e 3839 3320 2020 7c20 2020 302e 3934  0.893   |   0.94
-000038c0: 3520 2020 7c20 2a2a 312e 302a 2a20 207c  5   | **1.0**  |
-000038d0: 202a 2a30 2e39 3935 2a2a 207c 2020 2030   **0.995** |   0
-000038e0: 2e39 3234 2020 207c 2020 2030 2e39 3038  .924   |   0.908
-000038f0: 2020 207c 2020 2030 2e38 3937 2020 2020     |   0.897    
-00003900: 7c20 2020 302e 3934 3320 2020 207c 202a  |   0.943    | *
-00003910: 2a30 2e39 3834 2a2a 207c 0a7c 2043 4641  *0.984** |.| CFA
-00003920: 2020 2020 2020 2020 2020 207c 2057 6964             | Wid
-00003930: 6520 5265 734e 6574 2d35 3020 2020 2020  e ResNet-50     
-00003940: 7c20 2020 302e 3935 3620 2020 7c20 2020  |   0.956   |   
-00003950: 302e 3937 3820 2020 7c20 2020 302e 3936  0.978   |   0.96
-00003960: 3120 2020 7c20 2020 302e 3939 3020 2020  1   |   0.990   
-00003970: 7c20 2020 302e 3939 3920 2020 7c20 2020  |   0.999   |   
-00003980: 302e 3939 3420 2020 7c20 2030 2e39 3938  0.994   |  0.998
-00003990: 2020 7c20 2020 302e 3937 3920 2020 7c20    |   0.979   | 
-000039a0: 2020 302e 3837 3220 2020 7c20 2031 2e30    0.872   |  1.0
-000039b0: 3030 2020 207c 202a 2a30 2e39 3935 2a2a  00   | **0.995**
-000039c0: 207c 202a 2a30 2e39 3436 2a2a 207c 2020   | **0.946** |  
-000039d0: 2030 2e37 3033 2020 207c 202a 2a31 2e30   0.703   | **1.0
-000039e0: 3030 2a2a 2020 7c20 2020 302e 3935 3720  00**  |   0.957 
-000039f0: 2020 207c 2020 2030 2e39 3637 2020 207c     |   0.967   |
-00003a00: 0a7c 2043 4641 2020 2020 2020 2020 2020  .| CFA          
-00003a10: 207c 2052 6573 4e65 742d 3138 2020 2020   | ResNet-18    
-00003a20: 2020 2020 2020 7c20 2020 302e 3933 3020        |   0.930 
-00003a30: 2020 7c20 2020 302e 3935 3320 2020 7c20    |   0.953   | 
-00003a40: 2020 302e 3934 3720 2020 7c20 2020 302e    0.947   |   0.
-00003a50: 3939 3920 2020 7c20 2020 312e 3030 3020  999   |   1.000 
-00003a60: 2020 7c20 2a2a 312e 3030 302a 2a20 7c20    | **1.000** | 
-00003a70: 2030 2e39 3931 2020 7c20 2020 302e 3934   0.991  |   0.94
-00003a80: 3720 2020 7c20 2020 302e 3835 3820 2020  7   |   0.858   
-00003a90: 7c20 2030 2e39 3935 2020 207c 2020 2030  |  0.995   |   0
-00003aa0: 2e39 3332 2020 207c 2020 2030 2e38 3837  .932   |   0.887
-00003ab0: 2020 207c 2020 2030 2e36 3235 2020 207c     |   0.625   |
-00003ac0: 2020 2030 2e39 3934 2020 2020 7c20 2020     0.994    |   
-00003ad0: 302e 3839 3520 2020 207c 2020 2030 2e39  0.895    |   0.9
-00003ae0: 3139 2020 207c 0a7c 2050 6144 694d 2020  19   |.| PaDiM  
-00003af0: 2020 2020 2020 207c 2057 6964 6520 5265         | Wide Re
-00003b00: 734e 6574 2d35 3020 2020 2020 7c20 2020  sNet-50     |   
-00003b10: 302e 3935 3020 2020 7c20 2a2a 302e 3939  0.950   | **0.99
-00003b20: 352a 2a20 7c20 2020 302e 3934 3220 2020  5** |   0.942   
-00003b30: 7c20 2a2a 312e 3030 302a 2a20 7c20 2020  | **1.000** |   
-00003b40: 302e 3937 3420 2020 7c20 2020 302e 3939  0.974   |   0.99
-00003b50: 3320 2020 7c20 2030 2e39 3939 2020 7c20  3   |  0.999  | 
-00003b60: 2020 302e 3837 3820 2020 7c20 2020 302e    0.878   |   0.
-00003b70: 3932 3720 2020 7c20 2030 2e39 3634 2020  927   |  0.964  
-00003b80: 207c 2020 2030 2e39 3839 2020 207c 2020   |   0.989   |  
-00003b90: 2030 2e39 3339 2020 207c 2020 2030 2e38   0.939   |   0.8
-00003ba0: 3435 2020 207c 2020 2030 2e39 3432 2020  45   |   0.942  
-00003bb0: 2020 7c20 2020 302e 3937 3620 2020 207c    |   0.976    |
-00003bc0: 2020 2030 2e38 3832 2020 207c 0a7c 2050     0.882   |.| P
-00003bd0: 6144 694d 2020 2020 2020 2020 207c 2052  aDiM         | R
-00003be0: 6573 4e65 742d 3138 2020 2020 2020 2020  esNet-18        
-00003bf0: 2020 7c20 2020 302e 3839 3120 2020 7c20    |   0.891   | 
-00003c00: 2020 302e 3934 3520 2020 7c20 2020 302e    0.945   |   0.
-00003c10: 3835 3720 2020 7c20 2020 302e 3938 3220  857   |   0.982 
-00003c20: 2020 7c20 2020 302e 3935 3020 2020 7c20    |   0.950   | 
-00003c30: 2020 302e 3937 3620 2020 7c20 2030 2e39    0.976   |  0.9
-00003c40: 3934 2020 7c20 2020 302e 3834 3420 2020  94  |   0.844   
-00003c50: 7c20 2020 302e 3930 3120 2020 7c20 2030  |   0.901   |  0
-00003c60: 2e37 3530 2020 207c 2020 2030 2e39 3631  .750   |   0.961
-00003c70: 2020 207c 2020 2030 2e38 3633 2020 207c     |   0.863   |
-00003c80: 2020 2030 2e37 3539 2020 207c 2020 2030     0.759   |   0
-00003c90: 2e38 3839 2020 2020 7c20 2020 302e 3932  .889    |   0.92
-00003ca0: 3020 2020 207c 2020 2030 2e37 3830 2020  0    |   0.780  
-00003cb0: 207c 0a7c 2044 464d 2020 2020 2020 2020   |.| DFM        
-00003cc0: 2020 207c 2057 6964 6520 5265 734e 6574     | Wide ResNet
-00003cd0: 2d35 3020 2020 2020 7c20 2020 302e 3934  -50     |   0.94
-00003ce0: 3320 2020 7c20 2020 302e 3835 3520 2020  3   |   0.855   
-00003cf0: 7c20 2020 302e 3738 3420 2020 7c20 2020  |   0.784   |   
-00003d00: 302e 3939 3720 2020 7c20 2020 302e 3939  0.997   |   0.99
-00003d10: 3520 2020 7c20 2020 302e 3937 3520 2020  5   |   0.975   
-00003d20: 7c20 2030 2e39 3939 2020 7c20 2020 302e  |  0.999  |   0.
-00003d30: 3936 3920 2020 7c20 2020 302e 3932 3420  969   |   0.924 
-00003d40: 2020 7c20 2030 2e39 3738 2020 207c 2020    |  0.978   |  
-00003d50: 2030 2e39 3339 2020 207c 2020 2030 2e39   0.939   |   0.9
-00003d60: 3632 2020 207c 2020 2030 2e38 3733 2020  62   |   0.873  
-00003d70: 207c 2020 2030 2e39 3639 2020 2020 7c20   |   0.969    | 
-00003d80: 2020 302e 3937 3120 2020 207c 2020 2030    0.971    |   0
-00003d90: 2e39 3631 2020 207c 0a7c 2044 464d 2020  .961   |.| DFM  
-00003da0: 2020 2020 2020 2020 207c 2052 6573 4e65           | ResNe
-00003db0: 742d 3138 2020 2020 2020 2020 2020 7c20  t-18          | 
-00003dc0: 2020 302e 3933 3620 2020 7c20 2020 302e    0.936   |   0.
-00003dd0: 3831 3720 2020 7c20 2020 302e 3733 3620  817   |   0.736 
-00003de0: 2020 7c20 2020 302e 3939 3320 2020 7c20    |   0.993   | 
-00003df0: 2020 302e 3936 3620 2020 7c20 2020 302e    0.966   |   0.
-00003e00: 3937 3720 2020 7c20 2031 2e30 3030 2020  977   |  1.000  
-00003e10: 7c20 2020 302e 3935 3620 2020 7c20 2020  |   0.956   |   
-00003e20: 302e 3934 3420 2020 7c20 2030 2e39 3934  0.944   |  0.994
-00003e30: 2020 207c 2020 2030 2e39 3232 2020 207c     |   0.922   |
-00003e40: 2020 2030 2e39 3631 2020 207c 2020 2030     0.961   |   0
-00003e50: 2e38 3920 2020 207c 2020 2030 2e39 3639  .89    |   0.969
-00003e60: 2020 2020 7c20 2020 302e 3933 3920 2020      |   0.939   
-00003e70: 207c 2020 2030 2e39 3639 2020 207c 0a7c   |   0.969   |.|
-00003e80: 2053 5446 504d 2020 2020 2020 2020 207c   STFPM         |
-00003e90: 2057 6964 6520 5265 734e 6574 2d35 3020   Wide ResNet-50 
-00003ea0: 2020 2020 7c20 2020 302e 3837 3620 2020      |   0.876   
-00003eb0: 7c20 2020 302e 3935 3720 2020 7c20 2020  |   0.957   |   
-00003ec0: 302e 3937 3720 2020 7c20 2020 302e 3938  0.977   |   0.98
-00003ed0: 3120 2020 7c20 2020 302e 3937 3620 2020  1   |   0.976   
-00003ee0: 7c20 2020 302e 3933 3920 2020 7c20 2030  |   0.939   |  0
-00003ef0: 2e39 3837 2020 7c20 2020 302e 3837 3820  .987  |   0.878 
-00003f00: 2020 7c20 2020 302e 3733 3220 2020 7c20    |   0.732   | 
-00003f10: 2030 2e39 3935 2020 207c 2020 2030 2e39   0.995   |   0.9
-00003f20: 3733 2020 207c 2020 2030 2e36 3532 2020  73   |   0.652  
-00003f30: 207c 2020 2030 2e38 3235 2020 207c 2020   |   0.825   |  
-00003f40: 2030 2e35 3030 2020 2020 7c20 2020 302e   0.500    |   0.
-00003f50: 3837 3520 2020 207c 2020 2030 2e38 3939  875    |   0.899
-00003f60: 2020 207c 0a7c 2053 5446 504d 2020 2020     |.| STFPM    
-00003f70: 2020 2020 207c 2052 6573 4e65 742d 3138       | ResNet-18
-00003f80: 2020 2020 2020 2020 2020 7c20 2020 302e            |   0.
-00003f90: 3839 3320 2020 7c20 2020 302e 3935 3420  893   |   0.954 
-00003fa0: 2020 7c20 2a2a 302e 3938 322a 2a20 7c20    | **0.982** | 
-00003fb0: 2020 302e 3938 3920 2020 7c20 2020 302e    0.989   |   0.
-00003fc0: 3934 3920 2020 7c20 2020 302e 3936 3120  949   |   0.961 
-00003fd0: 2020 7c20 2030 2e39 3739 2020 7c20 2020    |  0.979  |   
-00003fe0: 302e 3833 3820 2020 7c20 2020 302e 3735  0.838   |   0.75
-00003ff0: 3920 2020 7c20 2030 2e39 3939 2020 207c  9   |  0.999   |
-00004000: 2020 2030 2e39 3536 2020 207c 2020 2030     0.956   |   0
-00004010: 2e37 3035 2020 207c 2020 2030 2e38 3335  .705   |   0.835
-00004020: 2020 207c 202a 2a30 2e39 3937 2a2a 2020     | **0.997**  
-00004030: 7c20 2020 302e 3835 3320 2020 207c 2020  |   0.853    |  
-00004040: 2030 2e36 3435 2020 207c 0a7c 2044 464b   0.645   |.| DFK
-00004050: 4445 2020 2020 2020 2020 207c 2057 6964  DE         | Wid
-00004060: 6520 5265 734e 6574 2d35 3020 2020 2020  e ResNet-50     
-00004070: 7c20 2020 302e 3737 3420 2020 7c20 2020  |   0.774   |   
-00004080: 302e 3730 3820 2020 7c20 2020 302e 3432  0.708   |   0.42
-00004090: 3220 2020 7c20 2020 302e 3930 3520 2020  2   |   0.905   
-000040a0: 7c20 2020 302e 3935 3920 2020 7c20 2020  |   0.959   |   
-000040b0: 302e 3930 3320 2020 7c20 2030 2e39 3336  0.903   |  0.936
-000040c0: 2020 7c20 2020 302e 3734 3620 2020 7c20    |   0.746   | 
-000040d0: 2020 302e 3835 3320 2020 7c20 2030 2e37    0.853   |  0.7
-000040e0: 3336 2020 207c 2020 2030 2e36 3837 2020  36   |   0.687  
-000040f0: 207c 2020 2030 2e37 3439 2020 207c 2020   |   0.749   |  
-00004100: 2030 2e35 3734 2020 207c 2020 2030 2e36   0.574   |   0.6
-00004110: 3937 2020 2020 7c20 2020 302e 3834 3320  97    |   0.843 
-00004120: 2020 207c 2020 2030 2e38 3932 2020 207c     |   0.892   |
-00004130: 0a7c 2044 464b 4445 2020 2020 2020 2020  .| DFKDE        
-00004140: 207c 2052 6573 4e65 742d 3138 2020 2020   | ResNet-18    
-00004150: 2020 2020 2020 7c20 2020 302e 3736 3220        |   0.762 
-00004160: 2020 7c20 2020 302e 3634 3620 2020 7c20    |   0.646   | 
-00004170: 2020 302e 3537 3720 2020 7c20 2020 302e    0.577   |   0.
-00004180: 3636 3920 2020 7c20 2020 302e 3936 3520  669   |   0.965 
-00004190: 2020 7c20 2020 302e 3836 3320 2020 7c20    |   0.863   | 
-000041a0: 2030 2e39 3531 2020 7c20 2020 302e 3735   0.951  |   0.75
-000041b0: 3120 2020 7c20 2020 302e 3639 3820 2020  1   |   0.698   
-000041c0: 7c20 2030 2e38 3036 2020 207c 2020 2030  |  0.806   |   0
-000041d0: 2e37 3239 2020 207c 2020 2030 2e36 3037  .729   |   0.607
-000041e0: 2020 207c 2020 2030 2e36 3934 2020 207c     |   0.694   |
-000041f0: 2020 2030 2e37 3637 2020 2020 7c20 2020     0.767    |   
-00004200: 302e 3833 3920 2020 207c 2020 2030 2e38  0.839    |   0.8
-00004210: 3636 2020 207c 0a7c 2047 414e 6f6d 616c  66   |.| GANomal
-00004220: 7920 2020 2020 207c 2020 2020 2020 2020  y      |        
-00004230: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00004240: 302e 3432 3120 2020 7c20 2020 302e 3230  0.421   |   0.20
-00004250: 3320 2020 7c20 2020 302e 3430 3420 2020  3   |   0.404   
-00004260: 7c20 2020 302e 3431 3320 2020 7c20 2020  |   0.413   |   
-00004270: 302e 3430 3820 2020 7c20 2020 302e 3734  0.408   |   0.74
-00004280: 3420 2020 7c20 2030 2e32 3531 2020 7c20  4   |  0.251  | 
-00004290: 2020 302e 3435 3720 2020 7c20 2020 302e    0.457   |   0.
-000042a0: 3638 3220 2020 7c20 2030 2e35 3337 2020  682   |  0.537  
-000042b0: 207c 2020 2030 2e32 3730 2020 207c 2020   |   0.270   |  
-000042c0: 2030 2e34 3732 2020 207c 2020 2030 2e32   0.472   |   0.2
-000042d0: 3331 2020 207c 2020 2030 2e33 3732 2020  31   |   0.372  
-000042e0: 2020 7c20 2020 302e 3434 3020 2020 207c    |   0.440    |
-000042f0: 2020 2030 2e34 3334 2020 207c 0a0a 2323     0.434   |..##
-00004300: 2050 6978 656c 2d4c 6576 656c 2041 5543   Pixel-Level AUC
-00004310: 0a0a 7c20 4d6f 6465 6c20 2020 2020 7c20  ..| Model     | 
-00004320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004330: 2020 207c 2020 2020 4176 6720 2020 207c     |    Avg    |
-00004340: 2020 4361 7270 6574 2020 207c 2020 2047    Carpet   |   G
-00004350: 7269 6420 2020 207c 2020 4c65 6174 6865  rid    |  Leathe
-00004360: 7220 207c 2020 2054 696c 6520 2020 207c  r  |   Tile    |
-00004370: 2020 2057 6f6f 6420 2020 207c 2020 426f     Wood    |  Bo
-00004380: 7474 6c65 2020 207c 2020 2043 6162 6c65  ttle   |   Cable
-00004390: 2020 207c 2020 4361 7073 756c 6520 207c     |  Capsule  |
-000043a0: 2048 617a 656c 6e75 7420 207c 204d 6574   Hazelnut  | Met
-000043b0: 616c 204e 7574 207c 2020 2050 696c 6c20  al Nut |   Pill 
-000043c0: 2020 207c 2020 2053 6372 6577 2020 207c     |   Screw   |
-000043d0: 2054 6f6f 7468 6272 7573 6820 7c20 5472   Toothbrush | Tr
-000043e0: 616e 7369 7374 6f72 207c 2020 5a69 7070  ansistor |  Zipp
-000043f0: 6572 2020 207c 0a7c 202d 2d2d 2d2d 2d2d  er   |.| -------
-00004400: 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d  -- | -----------
-00004410: 2d2d 2d2d 2d2d 2d20 7c20 3a2d 2d2d 2d2d  ------- | :-----
-00004420: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20  --: | :-------: 
-00004430: 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d  | :-------: | :-
-00004440: 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d  ------: | :-----
-00004450: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20  --: | :-------: 
-00004460: 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d  | :-------: | :-
-00004470: 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d  ------: | :-----
-00004480: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20  --: | :-------: 
-00004490: 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d  | :-------: | :-
-000044a0: 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d  ------: | :-----
-000044b0: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 2d3a  --: | :--------:
-000044c0: 207c 203a 2d2d 2d2d 2d2d 2d2d 3a20 7c20   | :--------: | 
-000044d0: 3a2d 2d2d 2d2d 2d2d 3a20 7c0a 7c20 2a2a  :-------: |.| **
-000044e0: 4346 412a 2a20 2020 7c20 2a2a 5769 6465  CFA**   | **Wide
-000044f0: 2052 6573 4e65 742d 3530 2a2a 207c 202a   ResNet-50** | *
-00004500: 2a30 2e39 3833 2a2a 207c 2020 2030 2e39  *0.983** |   0.9
-00004510: 3830 2020 207c 2020 2030 2e39 3534 2020  80   |   0.954  
-00004520: 207c 2020 2030 2e39 3839 2020 207c 202a   |   0.989   | *
-00004530: 2a30 2e39 3835 2a2a 207c 202a 2a30 2e39  *0.985** | **0.9
-00004540: 3734 2a2a 207c 202a 2a30 2e39 3839 2a2a  74** | **0.989**
-00004550: 207c 202a 2a30 2e39 3838 2a2a 207c 202a   | **0.988** | *
-00004560: 2a30 2e39 3839 2a2a 207c 2020 2030 2e39  *0.989** |   0.9
-00004570: 3835 2020 207c 202a 2a30 2e39 3932 2a2a  85   | **0.992**
-00004580: 207c 202a 2a30 2e39 3838 2a2a 207c 2020   | **0.988** |  
-00004590: 2030 2e39 3739 2020 207c 202a 2a30 2e39   0.979   | **0.9
-000045a0: 3931 2a2a 2020 7c20 2020 302e 3937 3720  91**  |   0.977 
-000045b0: 2020 207c 202a 2a30 2e39 3930 2a2a 207c     | **0.990** |
-000045c0: 0a7c 2043 4641 2020 2020 2020 207c 2052  .| CFA       | R
-000045d0: 6573 4e65 742d 3138 2020 2020 2020 2020  esNet-18        
-000045e0: 2020 7c20 2020 302e 3937 3920 2020 7c20    |   0.979   | 
-000045f0: 2020 302e 3937 3020 2020 7c20 2020 302e    0.970   |   0.
-00004600: 3937 3320 2020 7c20 2020 302e 3939 3220  973   |   0.992 
-00004610: 2020 7c20 2020 302e 3937 3820 2020 7c20    |   0.978   | 
-00004620: 2020 302e 3936 3420 2020 7c20 2020 302e    0.964   |   0.
-00004630: 3938 3620 2020 7c20 2020 302e 3938 3420  986   |   0.984 
-00004640: 2020 7c20 2020 302e 3938 3720 2020 7c20    |   0.987   | 
-00004650: 2020 302e 3938 3720 2020 7c20 2020 302e    0.987   |   0.
-00004660: 3938 3120 2020 7c20 2020 302e 3938 3120  981   |   0.981 
-00004670: 2020 7c20 2020 302e 3937 3320 2020 7c20    |   0.973   | 
-00004680: 2020 302e 3939 3020 2020 207c 2020 2030    0.990    |   0
-00004690: 2e39 3634 2020 2020 7c20 2020 302e 3937  .964    |   0.97
-000046a0: 3820 2020 7c0a 7c20 5061 7463 6843 6f72  8   |.| PatchCor
-000046b0: 6520 7c20 5769 6465 2052 6573 4e65 742d  e | Wide ResNet-
-000046c0: 3530 2020 2020 207c 2020 2030 2e39 3830  50     |   0.980
-000046d0: 2020 207c 2020 2030 2e39 3838 2020 207c     |   0.988   |
-000046e0: 2020 2030 2e39 3638 2020 207c 2020 2030     0.968   |   0
-000046f0: 2e39 3931 2020 207c 2020 2030 2e39 3631  .991   |   0.961
-00004700: 2020 207c 2020 2030 2e39 3334 2020 207c     |   0.934   |
-00004710: 2020 2030 2e39 3834 2020 207c 202a 2a30     0.984   | **0
-00004720: 2e39 3838 2a2a 207c 2020 2030 2e39 3838  .988** |   0.988
-00004730: 2020 207c 2020 2030 2e39 3837 2020 207c     |   0.987   |
-00004740: 2020 2030 2e39 3839 2020 207c 2020 2030     0.989   |   0
-00004750: 2e39 3830 2020 207c 202a 2a30 2e39 3839  .980   | **0.989
-00004760: 2a2a 207c 2020 2030 2e39 3838 2020 2020  ** |   0.988    
-00004770: 7c20 2a2a 302e 3938 312a 2a20 207c 2020  | **0.981**  |  
-00004780: 2030 2e39 3833 2020 207c 0a7c 2050 6174   0.983   |.| Pat
-00004790: 6368 436f 7265 207c 2052 6573 4e65 742d  chCore | ResNet-
-000047a0: 3138 2020 2020 2020 2020 2020 7c20 2020  18          |   
-000047b0: 302e 3937 3620 2020 7c20 2020 302e 3938  0.976   |   0.98
-000047c0: 3620 2020 7c20 2020 302e 3935 3520 2020  6   |   0.955   
-000047d0: 7c20 2020 302e 3939 3020 2020 7c20 2020  |   0.990   |   
-000047e0: 302e 3934 3320 2020 7c20 2020 302e 3933  0.943   |   0.93
-000047f0: 3320 2020 7c20 2020 302e 3938 3120 2020  3   |   0.981   
-00004800: 7c20 2020 302e 3938 3420 2020 7c20 2020  |   0.984   |   
-00004810: 302e 3938 3620 2020 7c20 2020 302e 3938  0.986   |   0.98
-00004820: 3620 2020 7c20 2020 302e 3938 3620 2020  6   |   0.986   
-00004830: 7c20 2020 302e 3937 3420 2020 7c20 2020  |   0.974   |   
-00004840: 302e 3939 3120 2020 7c20 2020 302e 3938  0.991   |   0.98
-00004850: 3820 2020 207c 2020 2030 2e39 3734 2020  8    |   0.974  
-00004860: 2020 7c20 2020 302e 3938 3320 2020 7c0a    |   0.983   |.
-00004870: 7c20 4346 6c6f 7720 2020 2020 7c20 5769  | CFlow     | Wi
-00004880: 6465 2052 6573 4e65 742d 3530 2020 2020  de ResNet-50    
-00004890: 207c 2020 2030 2e39 3731 2020 207c 2020   |   0.971   |  
-000048a0: 2030 2e39 3836 2020 207c 2020 2030 2e39   0.986   |   0.9
-000048b0: 3638 2020 207c 2020 2030 2e39 3933 2020  68   |   0.993  
-000048c0: 207c 2020 2030 2e39 3638 2020 207c 2020   |   0.968   |  
-000048d0: 2030 2e39 3234 2020 207c 2020 2030 2e39   0.924   |   0.9
-000048e0: 3831 2020 207c 2020 2030 2e39 3535 2020  81   |   0.955  
-000048f0: 207c 2020 2030 2e39 3838 2020 207c 202a   |   0.988   | *
-00004900: 2a30 2e39 3930 2a2a 207c 2020 2030 2e39  *0.990** |   0.9
-00004910: 3832 2020 207c 2020 2030 2e39 3833 2020  82   |   0.983  
-00004920: 207c 2020 2030 2e39 3739 2020 207c 2020   |   0.979   |  
-00004930: 2030 2e39 3835 2020 2020 7c20 2020 302e   0.985    |   0.
-00004940: 3839 3720 2020 207c 2020 2030 2e39 3830  897    |   0.980
-00004950: 2020 207c 0a7c 2050 6144 694d 2020 2020     |.| PaDiM    
-00004960: 207c 2057 6964 6520 5265 734e 6574 2d35   | Wide ResNet-5
-00004970: 3020 2020 2020 7c20 2020 302e 3937 3920  0     |   0.979 
-00004980: 2020 7c20 2a2a 302e 3939 312a 2a20 7c20    | **0.991** | 
-00004990: 2020 302e 3937 3020 2020 7c20 2020 302e    0.970   |   0.
-000049a0: 3939 3320 2020 7c20 2020 302e 3935 3520  993   |   0.955 
-000049b0: 2020 7c20 2020 302e 3935 3720 2020 7c20    |   0.957   | 
-000049c0: 2020 302e 3938 3520 2020 7c20 2020 302e    0.985   |   0.
-000049d0: 3937 3020 2020 7c20 2020 302e 3938 3820  970   |   0.988 
-000049e0: 2020 7c20 2020 302e 3938 3520 2020 7c20    |   0.985   | 
-000049f0: 2020 302e 3938 3220 2020 7c20 2020 302e    0.982   |   0.
-00004a00: 3936 3620 2020 7c20 2020 302e 3938 3820  966   |   0.988 
-00004a10: 2020 7c20 2a2a 302e 3939 312a 2a20 207c    | **0.991**  |
-00004a20: 2020 2030 2e39 3736 2020 2020 7c20 2020     0.976    |   
-00004a30: 302e 3938 3620 2020 7c0a 7c20 5061 4469  0.986   |.| PaDi
-00004a40: 4d20 2020 2020 7c20 5265 734e 6574 2d31  M     | ResNet-1
-00004a50: 3820 2020 2020 2020 2020 207c 2020 2030  8          |   0
-00004a60: 2e39 3638 2020 207c 2020 2030 2e39 3834  .968   |   0.984
-00004a70: 2020 207c 2020 2030 2e39 3138 2020 207c     |   0.918   |
-00004a80: 202a 2a30 2e39 3934 2a2a 207c 2020 2030   **0.994** |   0
-00004a90: 2e39 3334 2020 207c 2020 2030 2e39 3437  .934   |   0.947
-00004aa0: 2020 207c 2020 2030 2e39 3833 2020 207c     |   0.983   |
-00004ab0: 2020 2030 2e39 3635 2020 207c 2020 2030     0.965   |   0
-00004ac0: 2e39 3834 2020 207c 2020 2030 2e39 3738  .984   |   0.978
-00004ad0: 2020 207c 2020 2030 2e39 3730 2020 207c     |   0.970   |
-00004ae0: 2020 2030 2e39 3537 2020 207c 2020 2030     0.957   |   0
-00004af0: 2e39 3738 2020 207c 2020 2030 2e39 3838  .978   |   0.988
-00004b00: 2020 2020 7c20 2020 302e 3936 3820 2020      |   0.968   
-00004b10: 207c 2020 2030 2e39 3739 2020 207c 0a7c   |   0.979   |.|
-00004b20: 2053 5446 504d 2020 2020 207c 2057 6964   STFPM     | Wid
-00004b30: 6520 5265 734e 6574 2d35 3020 2020 2020  e ResNet-50     
-00004b40: 7c20 2020 302e 3930 3320 2020 7c20 2020  |   0.903   |   
-00004b50: 302e 3938 3720 2020 7c20 2a2a 302e 3938  0.987   | **0.98
-00004b60: 392a 2a20 7c20 2020 302e 3938 3020 2020  9** |   0.980   
-00004b70: 7c20 2020 302e 3936 3620 2020 7c20 2020  |   0.966   |   
-00004b80: 302e 3935 3620 2020 7c20 2020 302e 3936  0.956   |   0.96
-00004b90: 3620 2020 7c20 2020 302e 3931 3320 2020  6   |   0.913   
-00004ba0: 7c20 2020 302e 3935 3620 2020 7c20 2020  |   0.956   |   
-00004bb0: 302e 3937 3420 2020 7c20 2020 302e 3936  0.974   |   0.96
-00004bc0: 3120 2020 7c20 2020 302e 3934 3620 2020  1   |   0.946   
-00004bd0: 7c20 2020 302e 3938 3820 2020 7c20 2020  |   0.988   |   
-00004be0: 302e 3137 3820 2020 207c 2020 2030 2e38  0.178    |   0.8
-00004bf0: 3037 2020 2020 7c20 2020 302e 3938 3020  07    |   0.980 
-00004c00: 2020 7c0a 7c20 5354 4650 4d20 2020 2020    |.| STFPM     
-00004c10: 7c20 5265 734e 6574 2d31 3820 2020 2020  | ResNet-18     
-00004c20: 2020 2020 207c 2020 2030 2e39 3531 2020       |   0.951  
-00004c30: 207c 2020 2030 2e39 3836 2020 207c 2020   |   0.986   |  
-00004c40: 2030 2e39 3838 2020 207c 2020 2030 2e39   0.988   |   0.9
-00004c50: 3931 2020 207c 2020 2030 2e39 3436 2020  91   |   0.946  
-00004c60: 207c 2020 2030 2e39 3439 2020 207c 2020   |   0.949   |  
-00004c70: 2030 2e39 3731 2020 207c 2020 2030 2e38   0.971   |   0.8
-00004c80: 3938 2020 207c 2020 2030 2e39 3632 2020  98   |   0.962  
-00004c90: 207c 2020 2030 2e39 3831 2020 207c 2020   |   0.981   |  
-00004ca0: 2030 2e39 3432 2020 207c 2020 2030 2e38   0.942   |   0.8
-00004cb0: 3738 2020 207c 2020 2030 2e39 3833 2020  78   |   0.983  
-00004cc0: 207c 2020 2030 2e39 3833 2020 2020 7c20   |   0.983    | 
-00004cd0: 2020 302e 3833 3820 2020 207c 2020 2030    0.838    |   0
-00004ce0: 2e39 3732 2020 207c 0a0a 2323 2049 6d61  .972   |..## Ima
-00004cf0: 6765 2046 3120 5363 6f72 650a 0a7c 204d  ge F1 Score..| M
-00004d00: 6f64 656c 2020 2020 2020 2020 207c 2020  odel         |  
-00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d20: 2020 7c20 2020 2041 7667 2020 2020 7c20    |    Avg    | 
-00004d30: 2043 6172 7065 7420 2020 7c20 2020 4772   Carpet   |   Gr
-00004d40: 6964 2020 2020 7c20 204c 6561 7468 6572  id    |  Leather
-00004d50: 2020 7c20 2020 5469 6c65 2020 2020 7c20    |   Tile    | 
-00004d60: 2020 576f 6f64 2020 2020 7c20 2042 6f74    Wood    |  Bot
-00004d70: 746c 6520 2020 7c20 2020 4361 626c 6520  tle   |   Cable 
-00004d80: 2020 7c20 2043 6170 7375 6c65 2020 7c20    |  Capsule  | 
-00004d90: 4861 7a65 6c6e 7574 2020 7c20 4d65 7461  Hazelnut  | Meta
-00004da0: 6c20 4e75 7420 7c20 2020 5069 6c6c 2020  l Nut |   Pill  
-00004db0: 2020 7c20 2020 5363 7265 7720 2020 7c20    |   Screw   | 
-00004dc0: 546f 6f74 6862 7275 7368 207c 2054 7261  Toothbrush | Tra
-00004dd0: 6e73 6973 746f 7220 7c20 205a 6970 7065  nsistor |  Zippe
-00004de0: 7220 2020 7c0a 7c20 2d2d 2d2d 2d2d 2d2d  r   |.| --------
-00004df0: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
-00004e00: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 203a 2d2d  ---------- | :--
-00004e10: 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d  -----: | :------
-00004e20: 2d3a 207c 203a 2d2d 2d2d 2d2d 2d3a 207c  -: | :-------: |
-00004e30: 203a 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d   :-------: | :--
-00004e40: 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d  -----: | :------
-00004e50: 2d3a 207c 203a 2d2d 2d2d 2d2d 2d3a 207c  -: | :-------: |
-00004e60: 203a 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d   :-------: | :--
-00004e70: 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d  -----: | :------
-00004e80: 2d3a 207c 203a 2d2d 2d2d 2d2d 2d3a 207c  -: | :-------: |
-00004e90: 203a 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d   :-------: | :--
-00004ea0: 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d  -----: | :------
-00004eb0: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 2d3a  --: | :--------:
-00004ec0: 207c 203a 2d2d 2d2d 2d2d 2d3a 207c 0a7c   | :-------: |.|
-00004ed0: 202a 2a50 6174 6368 436f 7265 2a2a 207c   **PatchCore** |
-00004ee0: 202a 2a57 6964 6520 5265 734e 6574 2d35   **Wide ResNet-5
-00004ef0: 302a 2a20 7c20 2a2a 302e 3937 362a 2a20  0** | **0.976** 
-00004f00: 7c20 2020 302e 3937 3120 2020 7c20 2020  |   0.971   |   
-00004f10: 302e 3937 3420 2020 7c20 2a2a 312e 3030  0.974   | **1.00
-00004f20: 302a 2a20 7c20 2a2a 312e 3030 302a 2a20  0** | **1.000** 
-00004f30: 7c20 2020 302e 3936 3720 2020 7c20 2a2a  |   0.967   | **
-00004f40: 312e 3030 302a 2a20 7c20 2020 302e 3936  1.000** |   0.96
-00004f50: 3820 2020 7c20 2a2a 302e 3938 322a 2a20  8   | **0.982** 
-00004f60: 7c20 2a2a 312e 3030 302a 2a20 7c20 2020  | **1.000** |   
-00004f70: 302e 3938 3420 2020 7c20 2020 302e 3934  0.984   |   0.94
-00004f80: 3020 2020 7c20 2020 302e 3934 3320 2020  0   |   0.943   
-00004f90: 7c20 2020 302e 3933 3820 2020 207c 202a  |   0.938    | *
-00004fa0: 2a31 2e30 3030 2a2a 2020 7c20 2a2a 302e  *1.000**  | **0.
-00004fb0: 3937 392a 2a20 7c0a 7c20 5061 7463 6843  979** |.| PatchC
-00004fc0: 6f72 6520 2020 2020 7c20 5265 734e 6574  ore     | ResNet
-00004fd0: 2d31 3820 2020 2020 2020 2020 207c 2020  -18          |  
-00004fe0: 2030 2e39 3730 2020 207c 2020 2030 2e39   0.970   |   0.9
-00004ff0: 3439 2020 207c 2020 2030 2e39 3436 2020  49   |   0.946  
-00005000: 207c 202a 2a31 2e30 3030 2a2a 207c 2020   | **1.000** |  
-00005010: 2030 2e39 3820 2020 207c 2020 2030 2e39   0.98    |   0.9
-00005020: 3932 2020 207c 202a 2a31 2e30 3030 2a2a  92   | **1.000**
-00005030: 207c 202a 2a30 2e39 3738 2a2a 207c 2020   | **0.978** |  
-00005040: 2030 2e39 3639 2020 207c 202a 2a31 2e30   0.969   | **1.0
-00005050: 3030 2a2a 207c 202a 2a30 2e39 3839 2a2a  00** | **0.989**
-00005060: 207c 2020 2030 2e39 3430 2020 207c 2020   |   0.940   |  
-00005070: 2030 2e39 3332 2020 207c 2020 2030 2e39   0.932   |   0.9
-00005080: 3335 2020 2020 7c20 2020 302e 3937 3420  35    |   0.974 
-00005090: 2020 207c 2020 2030 2e39 3637 2020 207c     |   0.967   |
-000050a0: 0a7c 2043 4641 2020 2020 2020 2020 2020  .| CFA          
-000050b0: 207c 2057 6964 6520 5265 734e 6574 2d35   | Wide ResNet-5
-000050c0: 3020 2020 2020 7c20 2020 302e 3936 3220  0     |   0.962 
-000050d0: 2020 7c20 2020 302e 3936 3120 2020 7c20    |   0.961   | 
-000050e0: 2020 302e 3935 3720 2020 7c20 2020 302e    0.957   |   0.
-000050f0: 3939 3520 2020 7c20 2020 302e 3939 3420  995   |   0.994 
-00005100: 2020 7c20 2020 302e 3938 3320 2020 7c20    |   0.983   | 
-00005110: 2020 302e 3938 3420 2020 7c20 2020 302e    0.984   |   0.
-00005120: 3936 3220 2020 7c20 2020 302e 3934 3620  962   |   0.946 
-00005130: 2020 7c20 2a2a 312e 3030 302a 2a20 7c20    | **1.000** | 
-00005140: 2020 302e 3938 3420 2020 7c20 2a2a 302e    0.984   | **0.
-00005150: 3935 322a 2a20 7c20 2020 302e 3835 3520  952** |   0.855 
-00005160: 2020 7c20 2a2a 312e 3030 302a 2a20 207c    | **1.000**  |
-00005170: 2020 2030 2e39 3037 2020 2020 7c20 2020     0.907    |   
-00005180: 302e 3937 3520 2020 7c0a 7c20 4346 4120  0.975   |.| CFA 
-00005190: 2020 2020 2020 2020 2020 7c20 5265 734e            | ResN
-000051a0: 6574 2d31 3820 2020 2020 2020 2020 207c  et-18          |
-000051b0: 2020 2030 2e39 3436 2020 207c 2020 2030     0.946   |   0
-000051c0: 2e39 3536 2020 207c 2020 2030 2e39 3436  .956   |   0.946
-000051d0: 2020 207c 2020 2030 2e39 3733 2020 207c     |   0.973   |
-000051e0: 202a 2a31 2e30 3030 2a2a 207c 202a 2a31   **1.000** | **1
-000051f0: 2e30 3030 2a2a 207c 2020 2030 2e39 3833  .000** |   0.983
-00005200: 2020 207c 2020 2030 2e39 3037 2020 207c     |   0.907   |
-00005210: 2020 2030 2e39 3338 2020 207c 2020 2030     0.938   |   0
-00005220: 2e39 3936 2020 207c 2020 2030 2e39 3538  .996   |   0.958
-00005230: 2020 207c 2020 2030 2e39 3230 2020 207c     |   0.920   |
-00005240: 2020 2030 2e38 3538 2020 207c 2020 2030     0.858   |   0
-00005250: 2e39 3834 2020 2020 7c20 2020 302e 3739  .984    |   0.79
-00005260: 3520 2020 207c 2020 2030 2e39 3439 2020  5    |   0.949  
-00005270: 207c 0a7c 2043 466c 6f77 2020 2020 2020   |.| CFlow      
-00005280: 2020 207c 2057 6964 6520 5265 734e 6574     | Wide ResNet
-00005290: 2d35 3020 2020 2020 7c20 2020 302e 3934  -50     |   0.94
-000052a0: 3420 2020 7c20 2020 302e 3937 3220 2020  4   |   0.972   
-000052b0: 7c20 2020 302e 3933 3220 2020 7c20 2a2a  |   0.932   | **
-000052c0: 312e 3030 302a 2a20 7c20 2020 302e 3938  1.000** |   0.98
-000052d0: 3820 2020 7c20 2020 302e 3936 3720 2020  8   |   0.967   
-000052e0: 7c20 2a2a 312e 3030 302a 2a20 7c20 2020  | **1.000** |   
-000052f0: 302e 3833 3220 2020 7c20 2020 302e 3933  0.832   |   0.93
-00005300: 3920 2020 7c20 2a2a 312e 3030 302a 2a20  9   | **1.000** 
-00005310: 7c20 2020 302e 3937 3920 2020 7c20 2020  |   0.979   |   
-00005320: 302e 3932 3420 2020 7c20 2a2a 302e 3937  0.924   | **0.97
-00005330: 312a 2a20 7c20 2020 302e 3837 3020 2020  1** |   0.870   
-00005340: 207c 2020 2030 2e38 3138 2020 2020 7c20   |   0.818    | 
-00005350: 2020 302e 3936 3720 2020 7c0a 7c20 5061    0.967   |.| Pa
-00005360: 4469 4d20 2020 2020 2020 2020 7c20 5769  DiM         | Wi
-00005370: 6465 2052 6573 4e65 742d 3530 2020 2020  de ResNet-50    
-00005380: 207c 2020 2030 2e39 3531 2020 207c 202a   |   0.951   | *
-00005390: 2a30 2e39 3839 2a2a 207c 2020 2030 2e39  *0.989** |   0.9
-000053a0: 3330 2020 207c 202a 2a31 2e30 3030 2a2a  30   | **1.000**
-000053b0: 207c 2020 2030 2e39 3630 2020 207c 2020   |   0.960   |  
-000053c0: 2030 2e39 3833 2020 207c 2020 2030 2e39   0.983   |   0.9
-000053d0: 3932 2020 207c 2020 2030 2e38 3536 2020  92   |   0.856  
-000053e0: 207c 202a 2a30 2e39 3832 2a2a 207c 2020   | **0.982** |  
-000053f0: 2030 2e39 3337 2020 207c 2020 2030 2e39   0.937   |   0.9
-00005400: 3738 2020 207c 2020 2030 2e39 3436 2020  78   |   0.946  
-00005410: 207c 2020 2030 2e38 3935 2020 207c 2020   |   0.895   |  
-00005420: 2030 2e39 3532 2020 2020 7c20 2020 302e   0.952    |   0.
-00005430: 3931 3420 2020 207c 2020 2030 2e39 3437  914    |   0.947
-00005440: 2020 207c 0a7c 2050 6144 694d 2020 2020     |.| PaDiM    
-00005450: 2020 2020 207c 2052 6573 4e65 742d 3138       | ResNet-18
-00005460: 2020 2020 2020 2020 2020 7c20 2020 302e            |   0.
-00005470: 3931 3620 2020 7c20 2020 302e 3933 3020  916   |   0.930 
-00005480: 2020 7c20 2020 302e 3839 3320 2020 7c20    |   0.893   | 
-00005490: 2020 302e 3938 3420 2020 7c20 2020 302e    0.984   |   0.
-000054a0: 3933 3420 2020 7c20 2020 302e 3935 3220  934   |   0.952 
-000054b0: 2020 7c20 2020 302e 3937 3620 2020 7c20    |   0.976   | 
-000054c0: 2020 302e 3835 3820 2020 7c20 2020 302e    0.858   |   0.
-000054d0: 3936 3020 2020 7c20 2020 302e 3833 3620  960   |   0.836 
-000054e0: 2020 7c20 2020 302e 3937 3420 2020 7c20    |   0.974   | 
-000054f0: 2020 302e 3933 3220 2020 7c20 2020 302e    0.932   |   0.
-00005500: 3837 3920 2020 7c20 2020 302e 3932 3320  879   |   0.923 
-00005510: 2020 207c 2020 2030 2e37 3936 2020 2020     |   0.796    
-00005520: 7c20 2020 302e 3931 3520 2020 7c0a 7c20  |   0.915   |.| 
-00005530: 4446 4d20 2020 2020 2020 2020 2020 7c20  DFM           | 
-00005540: 5769 6465 2052 6573 4e65 742d 3530 2020  Wide ResNet-50  
-00005550: 2020 207c 2020 2030 2e39 3530 2020 207c     |   0.950   |
-00005560: 2020 2030 2e39 3135 2020 207c 2020 2030     0.915   |   0
-00005570: 2e38 3730 2020 207c 2020 2030 2e39 3935  .870   |   0.995
-00005580: 2020 207c 2020 2030 2e39 3838 2020 207c     |   0.988   |
-00005590: 2020 2030 2e39 3630 2020 207c 2020 2030     0.960   |   0
-000055a0: 2e39 3932 2020 207c 2020 2030 2e39 3339  .992   |   0.939
-000055b0: 2020 207c 2020 2030 2e39 3635 2020 207c     |   0.965   |
-000055c0: 2020 2030 2e39 3731 2020 207c 2020 2030     0.971   |   0
-000055d0: 2e39 3432 2020 207c 2020 2030 2e39 3536  .942   |   0.956
-000055e0: 2020 207c 2020 2030 2e39 3036 2020 207c     |   0.906   |
-000055f0: 2020 2030 2e39 3636 2020 2020 7c20 2020     0.966    |   
-00005600: 302e 3931 3420 2020 207c 2020 2030 2e39  0.914    |   0.9
-00005610: 3731 2020 207c 0a7c 2044 464d 2020 2020  71   |.| DFM    
-00005620: 2020 2020 2020 207c 2052 6573 4e65 742d         | ResNet-
-00005630: 3138 2020 2020 2020 2020 2020 7c20 2020  18          |   
-00005640: 302e 3934 3320 2020 7c20 2020 302e 3839  0.943   |   0.89
-00005650: 3520 2020 7c20 2020 302e 3837 3120 2020  5   |   0.871   
-00005660: 7c20 2020 302e 3937 3820 2020 7c20 2020  |   0.978   |   
-00005670: 302e 3935 3820 2020 7c20 2020 302e 3930  0.958   |   0.90
-00005680: 3020 2020 7c20 2020 312e 3030 3020 2020  0   |   1.000   
-00005690: 7c20 2020 302e 3933 3520 2020 7c20 2020  |   0.935   |   
-000056a0: 302e 3936 3520 2020 7c20 2020 302e 3936  0.965   |   0.96
-000056b0: 3620 2020 7c20 2020 302e 3934 3220 2020  6   |   0.942   
-000056c0: 7c20 2020 302e 3935 3620 2020 7c20 2020  |   0.956   |   
-000056d0: 302e 3931 3420 2020 7c20 2020 302e 3936  0.914   |   0.96
-000056e0: 3620 2020 207c 2020 2030 2e38 3638 2020  6    |   0.868  
-000056f0: 2020 7c20 2020 302e 3936 3420 2020 7c0a    |   0.964   |.
-00005700: 7c20 5354 4650 4d20 2020 2020 2020 2020  | STFPM         
-00005710: 7c20 5769 6465 2052 6573 4e65 742d 3530  | Wide ResNet-50
-00005720: 2020 2020 207c 2020 2030 2e39 3236 2020       |   0.926  
-00005730: 207c 2020 2030 2e39 3733 2020 207c 2020   |   0.973   |  
-00005740: 2030 2e39 3733 2020 207c 2020 2030 2e39   0.973   |   0.9
-00005750: 3734 2020 207c 2020 2030 2e39 3635 2020  74   |   0.965  
-00005760: 207c 2020 2030 2e39 3239 2020 207c 2020   |   0.929   |  
-00005770: 2030 2e39 3736 2020 207c 2020 2030 2e38   0.976   |   0.8
-00005780: 3533 2020 207c 2020 2030 2e39 3230 2020  53   |   0.920  
-00005790: 207c 2020 2030 2e39 3732 2020 207c 2020   |   0.972   |  
-000057a0: 2030 2e39 3734 2020 207c 2020 2030 2e39   0.974   |   0.9
-000057b0: 3232 2020 207c 2020 2030 2e38 3834 2020  22   |   0.884  
-000057c0: 207c 2020 2030 2e38 3333 2020 2020 7c20   |   0.833    | 
-000057d0: 2020 302e 3831 3520 2020 207c 2020 2030    0.815    |   0
-000057e0: 2e39 3331 2020 207c 0a7c 2053 5446 504d  .931   |.| STFPM
-000057f0: 2020 2020 2020 2020 207c 2052 6573 4e65           | ResNe
-00005800: 742d 3138 2020 2020 2020 2020 2020 7c20  t-18          | 
-00005810: 2020 302e 3933 3220 2020 7c20 2020 302e    0.932   |   0.
-00005820: 3936 3120 2020 7c20 2a2a 302e 3938 322a  961   | **0.982*
-00005830: 2a20 7c20 2020 302e 3938 3920 2020 7c20  * |   0.989   | 
-00005840: 2020 302e 3933 3020 2020 7c20 2020 302e    0.930   |   0.
-00005850: 3935 3120 2020 7c20 2020 302e 3938 3420  951   |   0.984 
-00005860: 2020 7c20 2020 302e 3831 3920 2020 7c20    |   0.819   | 
-00005870: 2020 302e 3931 3820 2020 7c20 2020 302e    0.918   |   0.
-00005880: 3939 3320 2020 7c20 2020 302e 3937 3320  993   |   0.973 
-00005890: 2020 7c20 2020 302e 3931 3820 2020 7c20    |   0.918   | 
-000058a0: 2020 302e 3838 3720 2020 7c20 2a2a 302e    0.887   | **0.
-000058b0: 3938 342a 2a20 207c 2020 2030 2e37 3930  984**  |   0.790
-000058c0: 2020 2020 7c20 2020 302e 3930 3820 2020      |   0.908   
-000058d0: 7c0a 7c20 4446 4b44 4520 2020 2020 2020  |.| DFKDE       
-000058e0: 2020 7c20 5769 6465 2052 6573 4e65 742d    | Wide ResNet-
-000058f0: 3530 2020 2020 207c 2020 2030 2e38 3735  50     |   0.875
-00005900: 2020 207c 2020 2030 2e39 3037 2020 207c     |   0.907   |
-00005910: 2020 2030 2e38 3434 2020 207c 2020 2030     0.844   |   0
-00005920: 2e39 3035 2020 207c 2020 2030 2e39 3435  .905   |   0.945
-00005930: 2020 207c 2020 2030 2e39 3134 2020 207c     |   0.914   |
-00005940: 2020 2030 2e39 3436 2020 207c 2020 2030     0.946   |   0
-00005950: 2e37 3930 2020 207c 2020 2030 2e39 3134  .790   |   0.914
-00005960: 2020 207c 2020 2030 2e38 3137 2020 207c     |   0.817   |
-00005970: 2020 2030 2e38 3934 2020 207c 2020 2030     0.894   |   0
-00005980: 2e39 3232 2020 207c 2020 2030 2e38 3535  .922   |   0.855
-00005990: 2020 207c 2020 2030 2e38 3435 2020 2020     |   0.845    
-000059a0: 7c20 2020 302e 3732 3220 2020 207c 2020  |   0.722    |  
-000059b0: 2030 2e39 3130 2020 207c 0a7c 2044 464b   0.910   |.| DFK
-000059c0: 4445 2020 2020 2020 2020 207c 2052 6573  DE         | Res
-000059d0: 4e65 742d 3138 2020 2020 2020 2020 2020  Net-18          
-000059e0: 7c20 2020 302e 3837 3220 2020 7c20 2020  |   0.872   |   
-000059f0: 302e 3836 3420 2020 7c20 2020 302e 3834  0.864   |   0.84
-00005a00: 3420 2020 7c20 2020 302e 3835 3420 2020  4   |   0.854   
-00005a10: 7c20 2020 302e 3936 3020 2020 7c20 2020  |   0.960   |   
-00005a20: 302e 3839 3820 2020 7c20 2020 302e 3934  0.898   |   0.94
-00005a30: 3220 2020 7c20 2020 302e 3739 3320 2020  2   |   0.793   
-00005a40: 7c20 2020 302e 3930 3820 2020 7c20 2020  |   0.908   |   
-00005a50: 302e 3832 3720 2020 7c20 2020 302e 3839  0.827   |   0.89
-00005a60: 3420 2020 7c20 2020 302e 3931 3620 2020  4   |   0.916   
-00005a70: 7c20 2020 302e 3835 3920 2020 7c20 2020  |   0.859   |   
-00005a80: 302e 3835 3320 2020 207c 2020 2030 2e37  0.853    |   0.7
-00005a90: 3536 2020 2020 7c20 2020 302e 3931 3620  56    |   0.916 
-00005aa0: 2020 7c0a 7c20 4741 4e6f 6d61 6c79 2020    |.| GANomaly  
-00005ab0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00005ac0: 2020 2020 2020 2020 207c 2020 2030 2e38           |   0.8
-00005ad0: 3334 2020 207c 2020 2030 2e38 3634 2020  34   |   0.864  
-00005ae0: 207c 2020 2030 2e38 3434 2020 207c 2020   |   0.844   |  
-00005af0: 2030 2e38 3532 2020 207c 2020 2030 2e38   0.852   |   0.8
-00005b00: 3336 2020 207c 2020 2030 2e38 3633 2020  36   |   0.863  
-00005b10: 207c 2020 2030 2e38 3633 2020 207c 2020   |   0.863   |  
-00005b20: 2030 2e37 3630 2020 207c 2020 2030 2e39   0.760   |   0.9
-00005b30: 3035 2020 207c 2020 2030 2e37 3737 2020  05   |   0.777  
-00005b40: 207c 2020 2030 2e38 3934 2020 207c 2020   |   0.894   |  
-00005b50: 2030 2e39 3136 2020 207c 2020 2030 2e38   0.916   |   0.8
-00005b60: 3533 2020 207c 2020 2030 2e38 3333 2020  53   |   0.833  
-00005b70: 2020 7c20 2020 302e 3537 3120 2020 207c    |   0.571    |
-00005b80: 2020 2030 2e38 3831 2020 207c 0a0a 2320     0.881   |..# 
-00005b90: 5265 6665 7265 6e63 650a 0a49 6620 796f  Reference..If yo
-00005ba0: 7520 7573 6520 7468 6973 206c 6962 7261  u use this libra
-00005bb0: 7279 2061 6e64 206c 6f76 6520 6974 2c20  ry and love it, 
-00005bc0: 7573 6520 7468 6973 2074 6f20 6369 7465  use this to cite
-00005bd0: 2069 7420 f09f a497 0a0a 6060 6074 6578   it ......```tex
-00005be0: 0a40 6d69 7363 7b61 6e6f 6d61 6c69 622c  .@misc{anomalib,
-00005bf0: 0a20 2020 2020 2074 6974 6c65 3d7b 416e  .      title={An
-00005c00: 6f6d 616c 6962 3a20 4120 4465 6570 204c  omalib: A Deep L
-00005c10: 6561 726e 696e 6720 4c69 6272 6172 7920  earning Library 
-00005c20: 666f 7220 416e 6f6d 616c 7920 4465 7465  for Anomaly Dete
-00005c30: 6374 696f 6e7d 2c0a 2020 2020 2020 6175  ction},.      au
-00005c40: 7468 6f72 3d7b 5361 6d65 7420 416b 6361  thor={Samet Akca
-00005c50: 7920 616e 640a 2020 2020 2020 2020 2020  y and.          
-00005c60: 2020 2020 4469 636b 2041 6d65 6c6e 2061      Dick Ameln a
-00005c70: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-00005c80: 2041 7368 7769 6e20 5661 6964 7961 2061   Ashwin Vaidya a
-00005c90: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-00005ca0: 2042 6172 6174 6820 4c61 6b73 686d 616e   Barath Lakshman
-00005cb0: 616e 2061 6e64 0a20 2020 2020 2020 2020  an and.         
-00005cc0: 2020 2020 204e 696c 6573 6820 4168 756a       Nilesh Ahuj
-00005cd0: 6120 616e 640a 2020 2020 2020 2020 2020  a and.          
-00005ce0: 2020 2020 5574 6b75 2047 656e 637d 2c0a      Utku Genc},.
-00005cf0: 2020 2020 2020 7965 6172 3d7b 3230 3232        year={2022
-00005d00: 7d2c 0a20 2020 2020 2065 7072 696e 743d  },.      eprint=
-00005d10: 7b32 3230 322e 3038 3334 317d 2c0a 2020  {2202.08341},.  
-00005d20: 2020 2020 6172 6368 6976 6550 7265 6669      archivePrefi
-00005d30: 783d 7b61 7258 6976 7d2c 0a20 2020 2020  x={arXiv},.     
-00005d40: 2070 7269 6d61 7279 436c 6173 733d 7b63   primaryClass={c
-00005d50: 732e 4356 7d0a 7d0a 6060 600a            s.CV}.}.```.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 616e 6f6d  : 2.1.Name: anom
+00000020: 616c 6962 0a56 6572 7369 6f6e 3a20 302e  alib.Version: 0.
+00000030: 352e 300a 5375 6d6d 6172 793a 2061 6e6f  5.0.Summary: ano
+00000040: 6d61 6c69 6220 2d20 416e 6f6d 616c 7920  malib - Anomaly 
+00000050: 4465 7465 6374 696f 6e20 4c69 6272 6172  Detection Librar
+00000060: 790a 486f 6d65 2d70 6167 653a 200a 4175  y.Home-page: .Au
+00000070: 7468 6f72 3a20 496e 7465 6c20 4f70 656e  thor: Intel Open
+00000080: 5649 4e4f 0a41 7574 686f 722d 656d 6169  VINO.Author-emai
+00000090: 6c3a 2068 656c 7040 6f70 656e 7669 6e6f  l: help@openvino
+000000a0: 2e69 6e74 656c 2e63 6f6d 0a4c 6963 656e  .intel.com.Licen
+000000b0: 7365 3a20 436f 7079 7269 6768 7420 2863  se: Copyright (c
+000000c0: 2920 496e 7465 6c20 2d20 416c 6c20 5269  ) Intel - All Ri
+000000d0: 6768 7473 2052 6573 6572 7665 642e 204c  ghts Reserved. L
+000000e0: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
+000000f0: 6520 4170 6163 6865 204c 6963 656e 7365  e Apache License
+00000100: 2c20 5665 7273 696f 6e20 322e 3020 2874  , Version 2.0 (t
+00000110: 6865 2022 4c69 6365 6e73 6522 2953 6565  he "License")See
+00000120: 204c 4943 454e 5345 2066 696c 6520 666f   LICENSE file fo
+00000130: 7220 6d6f 7265 2064 6574 6169 6c73 2e0a  r more details..
+00000140: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
+00000150: 203e 3d33 2e37 0a44 6573 6372 6970 7469   >=3.7.Descripti
+00000160: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00000170: 2074 6578 742f 6d61 726b 646f 776e 0a50   text/markdown.P
+00000180: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
+00000190: 6f67 6765 7273 0a50 726f 7669 6465 732d  oggers.Provides-
+000001a0: 4578 7472 613a 206e 6f74 6562 6f6f 6b73  Extra: notebooks
+000001b0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+000001c0: 206f 7065 6e76 696e 6f0a 5072 6f76 6964   openvino.Provid
+000001d0: 6573 2d45 7874 7261 3a20 6675 6c6c 0a4c  es-Extra: full.L
+000001e0: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
+000001f0: 454e 5345 0a0a 3c64 6976 2061 6c69 676e  ENSE..<div align
+00000200: 3d22 6365 6e74 6572 223e 0a0a 3c69 6d67  ="center">..<img
+00000210: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00000220: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00000230: 656e 742e 636f 6d2f 6f70 656e 7669 6e6f  ent.com/openvino
+00000240: 746f 6f6c 6b69 742f 616e 6f6d 616c 6962  toolkit/anomalib
+00000250: 2f6d 6169 6e2f 646f 6373 2f73 6f75 7263  /main/docs/sourc
+00000260: 652f 696d 6167 6573 2f6c 6f67 6f73 2f61  e/images/logos/a
+00000270: 6e6f 6d61 6c69 622d 7769 6465 2d62 6c75  nomalib-wide-blu
+00000280: 652e 706e 6722 2077 6964 7468 3d22 3630  e.png" width="60
+00000290: 3070 7822 3e0a 0a2a 2a41 206c 6962 7261  0px">..**A libra
+000002a0: 7279 2066 6f72 2062 656e 6368 6d61 726b  ry for benchmark
+000002b0: 696e 672c 2064 6576 656c 6f70 696e 6720  ing, developing 
+000002c0: 616e 6420 6465 706c 6f79 696e 6720 6465  and deploying de
+000002d0: 6570 206c 6561 726e 696e 6720 616e 6f6d  ep learning anom
+000002e0: 616c 7920 6465 7465 6374 696f 6e20 616c  aly detection al
+000002f0: 676f 7269 7468 6d73 2a2a 0a0a 2d2d 2d0a  gorithms**..---.
+00000300: 0a5b 4b65 7920 4665 6174 7572 6573 5d28  .[Key Features](
+00000310: 236b 6579 2d66 6561 7475 7265 7329 20e2  #key-features) .
+00000320: 80a2 0a5b 4765 7474 696e 6720 5374 6172  ...[Getting Star
+00000330: 7465 645d 2823 6765 7474 696e 672d 7374  ted](#getting-st
+00000340: 6172 7465 6429 20e2 80a2 0a5b 446f 6373  arted) ....[Docs
+00000350: 5d28 6874 7470 733a 2f2f 6f70 656e 7669  ](https://openvi
+00000360: 6e6f 746f 6f6c 6b69 742e 6769 7468 7562  notoolkit.github
+00000370: 2e69 6f2f 616e 6f6d 616c 6962 2920 e280  .io/anomalib) ..
+00000380: a20a 5b4c 6963 656e 7365 5d28 6874 7470  ..[License](http
+00000390: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
+000003a0: 7065 6e76 696e 6f74 6f6f 6c6b 6974 2f61  penvinotoolkit/a
+000003b0: 6e6f 6d61 6c69 622f 626c 6f62 2f6d 6169  nomalib/blob/mai
+000003c0: 6e2f 4c49 4345 4e53 4529 0a0a 5b21 5b70  n/LICENSE)..[![p
+000003d0: 7974 686f 6e5d 2868 7474 7073 3a2f 2f69  ython](https://i
+000003e0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+000003f0: 6467 652f 7079 7468 6f6e 2d33 2e37 2532  dge/python-3.7%2
+00000400: 422d 6772 6565 6e29 5d28 290a 5b21 5b70  B-green)]().[![p
+00000410: 7974 6f72 6368 5d28 6874 7470 733a 2f2f  ytorch](https://
+00000420: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000430: 6164 6765 2f70 7974 6f72 6368 2d31 2e38  adge/pytorch-1.8
+00000440: 2e31 2532 422d 6f72 616e 6765 295d 2829  .1%2B-orange)]()
+00000450: 0a5b 215b 6f70 656e 7669 6e6f 5d28 6874  .[![openvino](ht
+00000460: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000470: 732e 696f 2f62 6164 6765 2f6f 7065 6e76  s.io/badge/openv
+00000480: 696e 6f2d 3230 3231 2e34 2e32 2d70 7572  ino-2021.4.2-pur
+00000490: 706c 6529 5d28 290a 5b21 5b63 6f6d 6574  ple)]().[![comet
+000004a0: 5d28 6874 7470 733a 2f2f 6375 7374 6f6d  ](https://custom
+000004b0: 2d69 636f 6e2d 6261 6467 6573 2e68 6572  -icon-badges.her
+000004c0: 6f6b 7561 7070 2e63 6f6d 2f62 6164 6765  okuapp.com/badge
+000004d0: 2f63 6f6d 6574 5f5f 6d6c 2d33 2e33 312e  /comet__ml-3.31.
+000004e0: 372d 6f72 616e 6765 3f6c 6f67 6f3d 6c6f  7-orange?logo=lo
+000004f0: 676f 5f63 6f6d 6574 5f6d 6c29 5d28 6874  go_comet_ml)](ht
+00000500: 7470 733a 2f2f 7777 772e 636f 6d65 742e  tps://www.comet.
+00000510: 636f 6d2f 7369 7465 2f70 726f 6475 6374  com/site/product
+00000520: 732f 6d6c 2d65 7870 6572 696d 656e 742d  s/ml-experiment-
+00000530: 7472 6163 6b69 6e67 2f3f 7574 6d5f 736f  tracking/?utm_so
+00000540: 7572 6365 3d61 6e6f 6d61 6c69 6226 7574  urce=anomalib&ut
+00000550: 6d5f 6d65 6469 756d 3d72 6566 6572 7261  m_medium=referra
+00000560: 6c29 0a5b 215b 436f 6461 6379 2042 6164  l).[![Codacy Bad
+00000570: 6765 5d28 6874 7470 733a 2f2f 6170 702e  ge](https://app.
+00000580: 636f 6461 6379 2e63 6f6d 2f70 726f 6a65  codacy.com/proje
+00000590: 6374 2f62 6164 6765 2f47 7261 6465 2f36  ct/badge/Grade/6
+000005a0: 3834 3932 3763 3163 3736 6334 6335 6539  84927c1c76c4c5e9
+000005b0: 3462 6235 3334 3830 3831 3266 6262 6229  4bb53480812fbbb)
+000005c0: 5d28 6874 7470 733a 2f2f 7777 772e 636f  ](https://www.co
+000005d0: 6461 6379 2e63 6f6d 2f67 682f 6f70 656e  dacy.com/gh/open
+000005e0: 7669 6e6f 746f 6f6c 6b69 742f 616e 6f6d  vinotoolkit/anom
+000005f0: 616c 6962 2f64 6173 6862 6f61 7264 3f75  alib/dashboard?u
+00000600: 746d 5f73 6f75 7263 653d 6769 7468 7562  tm_source=github
+00000610: 2e63 6f6d 2675 746d 5f6d 6564 6975 6d3d  .com&utm_medium=
+00000620: 7265 6665 7272 616c 2675 746d 5f63 6f6e  referral&utm_con
+00000630: 7465 6e74 3d6f 7065 6e76 696e 6f74 6f6f  tent=openvinotoo
+00000640: 6c6b 6974 2f61 6e6f 6d61 6c69 6226 7574  lkit/anomalib&ut
+00000650: 6d5f 6361 6d70 6169 676e 3d42 6164 6765  m_campaign=Badge
+00000660: 5f47 7261 6465 290a 5b21 5b62 6c61 636b  _Grade).[![black
+00000670: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000680: 6965 6c64 732e 696f 2f62 6164 6765 2f63  ields.io/badge/c
+00000690: 6f64 6525 3230 7374 796c 652d 626c 6163  ode%20style-blac
+000006a0: 6b2d 3030 3030 3030 2e73 7667 295d 2829  k-000000.svg)]()
+000006b0: 0a5b 215b 4e69 6768 746c 792d 5265 6772  .[![Nightly-Regr
+000006c0: 6573 7369 6f6e 2054 6573 745d 2868 7474  ession Test](htt
+000006d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000006e0: 6f70 656e 7669 6e6f 746f 6f6c 6b69 742f  openvinotoolkit/
+000006f0: 616e 6f6d 616c 6962 2f61 6374 696f 6e73  anomalib/actions
+00000700: 2f77 6f72 6b66 6c6f 7773 2f6e 6967 6874  /workflows/night
+00000710: 6c79 2e79 6d6c 2f62 6164 6765 2e73 7667  ly.yml/badge.svg
+00000720: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000730: 622e 636f 6d2f 6f70 656e 7669 6e6f 746f  b.com/openvinoto
+00000740: 6f6c 6b69 742f 616e 6f6d 616c 6962 2f61  olkit/anomalib/a
+00000750: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000760: 2f6e 6967 6874 6c79 2e79 6d6c 290a 5b21  /nightly.yml).[!
+00000770: 5b50 7265 2d4d 6572 6765 2043 6865 636b  [Pre-Merge Check
+00000780: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00000790: 622e 636f 6d2f 6f70 656e 7669 6e6f 746f  b.com/openvinoto
+000007a0: 6f6c 6b69 742f 616e 6f6d 616c 6962 2f61  olkit/anomalib/a
+000007b0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+000007c0: 2f70 7265 5f6d 6572 6765 2e79 6d6c 2f62  /pre_merge.yml/b
+000007d0: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
+000007e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f70  ://github.com/op
+000007f0: 656e 7669 6e6f 746f 6f6c 6b69 742f 616e  envinotoolkit/an
+00000800: 6f6d 616c 6962 2f61 6374 696f 6e73 2f77  omalib/actions/w
+00000810: 6f72 6b66 6c6f 7773 2f70 7265 5f6d 6572  orkflows/pre_mer
+00000820: 6765 2e79 6d6c 290a 5b21 5b63 6f64 6563  ge.yml).[![codec
+00000830: 6f76 5d28 6874 7470 733a 2f2f 636f 6465  ov](https://code
+00000840: 636f 762e 696f 2f67 682f 6f70 656e 7669  cov.io/gh/openvi
+00000850: 6e6f 746f 6f6c 6b69 742f 616e 6f6d 616c  notoolkit/anomal
+00000860: 6962 2f62 7261 6e63 682f 6d61 696e 2f67  ib/branch/main/g
+00000870: 7261 7068 2f62 6164 6765 2e73 7667 3f74  raph/badge.svg?t
+00000880: 6f6b 656e 3d5a 3641 3037 4e31 425a 4b29  oken=Z6A07N1BZK)
+00000890: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
+000008a0: 762e 696f 2f67 682f 6f70 656e 7669 6e6f  v.io/gh/openvino
+000008b0: 746f 6f6c 6b69 742f 616e 6f6d 616c 6962  toolkit/anomalib
+000008c0: 290a 5b21 5b44 6f63 735d 2868 7474 7073  ).[![Docs](https
+000008d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f70  ://github.com/op
+000008e0: 656e 7669 6e6f 746f 6f6c 6b69 742f 616e  envinotoolkit/an
+000008f0: 6f6d 616c 6962 2f61 6374 696f 6e73 2f77  omalib/actions/w
+00000900: 6f72 6b66 6c6f 7773 2f64 6f63 732e 796d  orkflows/docs.ym
+00000910: 6c2f 6261 6467 652e 7376 6729 5d28 6874  l/badge.svg)](ht
+00000920: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000930: 2f6f 7065 6e76 696e 6f74 6f6f 6c6b 6974  /openvinotoolkit
+00000940: 2f61 6e6f 6d61 6c69 622f 6163 7469 6f6e  /anomalib/action
+00000950: 732f 776f 726b 666c 6f77 732f 646f 6373  s/workflows/docs
+00000960: 2e79 6d6c 290a 5b21 5b44 6f77 6e6c 6f61  .yml).[![Downloa
+00000970: 6473 5d28 6874 7470 733a 2f2f 7374 6174  ds](https://stat
+00000980: 6963 2e70 6570 792e 7465 6368 2f70 6572  ic.pepy.tech/per
+00000990: 736f 6e61 6c69 7a65 642d 6261 6467 652f  sonalized-badge/
+000009a0: 616e 6f6d 616c 6962 3f70 6572 696f 643d  anomalib?period=
+000009b0: 746f 7461 6c26 756e 6974 733d 696e 7465  total&units=inte
+000009c0: 726e 6174 696f 6e61 6c5f 7379 7374 656d  rnational_system
+000009d0: 266c 6566 745f 636f 6c6f 723d 6772 6579  &left_color=grey
+000009e0: 2672 6967 6874 5f63 6f6c 6f72 3d67 7265  &right_color=gre
+000009f0: 656e 266c 6566 745f 7465 7874 3d50 7950  en&left_text=PyP
+00000a00: 4925 3230 446f 776e 6c6f 6164 7329 5d28  I%20Downloads)](
+00000a10: 6874 7470 733a 2f2f 7065 7079 2e74 6563  https://pepy.tec
+00000a20: 682f 7072 6f6a 6563 742f 616e 6f6d 616c  h/project/anomal
+00000a30: 6962 290a 0a3c 2f64 6976 3e0a 0a2d 2d2d  ib)..</div>..---
+00000a40: 0a0a 2320 496e 7472 6f64 7563 7469 6f6e  ..# Introduction
+00000a50: 0a0a 416e 6f6d 616c 6962 2069 7320 6120  ..Anomalib is a 
+00000a60: 6465 6570 206c 6561 726e 696e 6720 6c69  deep learning li
+00000a70: 6272 6172 7920 7468 6174 2061 696d 7320  brary that aims 
+00000a80: 746f 2063 6f6c 6c65 6374 2073 7461 7465  to collect state
+00000a90: 2d6f 662d 7468 652d 6172 7420 616e 6f6d  -of-the-art anom
+00000aa0: 616c 7920 6465 7465 6374 696f 6e20 616c  aly detection al
+00000ab0: 676f 7269 7468 6d73 2066 6f72 2062 656e  gorithms for ben
+00000ac0: 6368 6d61 726b 696e 6720 6f6e 2062 6f74  chmarking on bot
+00000ad0: 6820 7075 626c 6963 2061 6e64 2070 7269  h public and pri
+00000ae0: 7661 7465 2064 6174 6173 6574 732e 2041  vate datasets. A
+00000af0: 6e6f 6d61 6c69 6220 7072 6f76 6964 6573  nomalib provides
+00000b00: 2073 6576 6572 616c 2072 6561 6479 2d74   several ready-t
+00000b10: 6f2d 7573 6520 696d 706c 656d 656e 7461  o-use implementa
+00000b20: 7469 6f6e 7320 6f66 2061 6e6f 6d61 6c79  tions of anomaly
+00000b30: 2064 6574 6563 7469 6f6e 2061 6c67 6f72   detection algor
+00000b40: 6974 686d 7320 6465 7363 7269 6265 6420  ithms described 
+00000b50: 696e 2074 6865 2072 6563 656e 7420 6c69  in the recent li
+00000b60: 7465 7261 7475 7265 2c20 6173 2077 656c  terature, as wel
+00000b70: 6c20 6173 2061 2073 6574 206f 6620 746f  l as a set of to
+00000b80: 6f6c 7320 7468 6174 2066 6163 696c 6974  ols that facilit
+00000b90: 6174 6520 7468 6520 6465 7665 6c6f 706d  ate the developm
+00000ba0: 656e 7420 616e 6420 696d 706c 656d 656e  ent and implemen
+00000bb0: 7461 7469 6f6e 206f 6620 6375 7374 6f6d  tation of custom
+00000bc0: 206d 6f64 656c 732e 2054 6865 206c 6962   models. The lib
+00000bd0: 7261 7279 2068 6173 2061 2073 7472 6f6e  rary has a stron
+00000be0: 6720 666f 6375 7320 6f6e 2069 6d61 6765  g focus on image
+00000bf0: 2d62 6173 6564 2061 6e6f 6d61 6c79 2064  -based anomaly d
+00000c00: 6574 6563 7469 6f6e 2c20 7768 6572 6520  etection, where 
+00000c10: 7468 6520 676f 616c 206f 6620 7468 6520  the goal of the 
+00000c20: 616c 676f 7269 7468 6d20 6973 2074 6f20  algorithm is to 
+00000c30: 6964 656e 7469 6679 2061 6e6f 6d61 6c6f  identify anomalo
+00000c40: 7573 2069 6d61 6765 732c 206f 7220 616e  us images, or an
+00000c50: 6f6d 616c 6f75 7320 7069 7865 6c20 7265  omalous pixel re
+00000c60: 6769 6f6e 7320 7769 7468 696e 2069 6d61  gions within ima
+00000c70: 6765 7320 696e 2061 2064 6174 6173 6574  ges in a dataset
+00000c80: 2e20 416e 6f6d 616c 6962 2069 7320 636f  . Anomalib is co
+00000c90: 6e73 7461 6e74 6c79 2075 7064 6174 6564  nstantly updated
+00000ca0: 2077 6974 6820 6e65 7720 616c 676f 7269   with new algori
+00000cb0: 7468 6d73 2061 6e64 2074 7261 696e 696e  thms and trainin
+00000cc0: 672f 696e 6665 7265 6e63 6520 6578 7465  g/inference exte
+00000cd0: 6e73 696f 6e73 2c20 736f 206b 6565 7020  nsions, so keep 
+00000ce0: 6368 6563 6b69 6e67 210a 0a21 5b53 616d  checking!..![Sam
+00000cf0: 706c 6520 496d 6167 655d 2868 7474 7073  ple Image](https
+00000d00: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000d10: 7263 6f6e 7465 6e74 2e63 6f6d 2f6f 7065  rcontent.com/ope
+00000d20: 6e76 696e 6f74 6f6f 6c6b 6974 2f61 6e6f  nvinotoolkit/ano
+00000d30: 6d61 6c69 622f 6d61 696e 2f64 6f63 732f  malib/main/docs/
+00000d40: 736f 7572 6365 2f69 6d61 6765 732f 7265  source/images/re
+00000d50: 6164 6d65 2e70 6e67 290a 0a23 2320 4b65  adme.png)..## Ke
+00000d60: 7920 6665 6174 7572 6573 0a0a 2d20 5468  y features..- Th
+00000d70: 6520 6c61 7267 6573 7420 7075 626c 6963  e largest public
+00000d80: 2063 6f6c 6c65 6374 696f 6e20 6f66 2072   collection of r
+00000d90: 6561 6479 2d74 6f2d 7573 6520 6465 6570  eady-to-use deep
+00000da0: 206c 6561 726e 696e 6720 616e 6f6d 616c   learning anomal
+00000db0: 7920 6465 7465 6374 696f 6e20 616c 676f  y detection algo
+00000dc0: 7269 7468 6d73 2061 6e64 2062 656e 6368  rithms and bench
+00000dd0: 6d61 726b 2064 6174 6173 6574 732e 0a2d  mark datasets..-
+00000de0: 205b 2a2a 5079 546f 7263 6820 4c69 6768   [**PyTorch Ligh
+00000df0: 746e 696e 672a 2a5d 2868 7474 7073 3a2f  tning**](https:/
+00000e00: 2f77 7777 2e70 7974 6f72 6368 6c69 6768  /www.pytorchligh
+00000e10: 746e 696e 672e 6169 2f29 2062 6173 6564  tning.ai/) based
+00000e20: 206d 6f64 656c 2069 6d70 6c65 6d65 6e74   model implement
+00000e30: 6174 696f 6e73 2074 6f20 7265 6475 6365  ations to reduce
+00000e40: 2062 6f69 6c65 7270 6c61 7465 2063 6f64   boilerplate cod
+00000e50: 6520 616e 6420 6c69 6d69 7420 7468 6520  e and limit the 
+00000e60: 696d 706c 656d 656e 7461 7469 6f6e 2065  implementation e
+00000e70: 6666 6f72 7473 2074 6f20 7468 6520 6261  fforts to the ba
+00000e80: 7265 2065 7373 656e 7469 616c 732e 0a2d  re essentials..-
+00000e90: 2041 6c6c 206d 6f64 656c 7320 6361 6e20   All models can 
+00000ea0: 6265 2065 7870 6f72 7465 6420 746f 205b  be exported to [
+00000eb0: 2a2a 4f70 656e 5649 4e4f 2a2a 5d28 6874  **OpenVINO**](ht
+00000ec0: 7470 733a 2f2f 7777 772e 696e 7465 6c2e  tps://www.intel.
+00000ed0: 636f 6d2f 636f 6e74 656e 742f 7777 772f  com/content/www/
+00000ee0: 7573 2f65 6e2f 6465 7665 6c6f 7065 722f  us/en/developer/
+00000ef0: 746f 6f6c 732f 6f70 656e 7669 6e6f 2d74  tools/openvino-t
+00000f00: 6f6f 6c6b 6974 2f6f 7665 7276 6965 772e  oolkit/overview.
+00000f10: 6874 6d6c 2920 496e 7465 726d 6564 6961  html) Intermedia
+00000f20: 7465 2052 6570 7265 7365 6e74 6174 696f  te Representatio
+00000f30: 6e20 2849 5229 2066 6f72 2061 6363 656c  n (IR) for accel
+00000f40: 6572 6174 6564 2069 6e66 6572 656e 6365  erated inference
+00000f50: 206f 6e20 696e 7465 6c20 6861 7264 7761   on intel hardwa
+00000f60: 7265 2e0a 2d20 4120 7365 7420 6f66 205b  re..- A set of [
+00000f70: 696e 6665 7265 6e63 6520 746f 6f6c 735d  inference tools]
+00000f80: 2823 696e 6665 7265 6e63 6529 2066 6f72  (#inference) for
+00000f90: 2071 7569 636b 2061 6e64 2065 6173 7920   quick and easy 
+00000fa0: 6465 706c 6f79 6d65 6e74 206f 6620 7468  deployment of th
+00000fb0: 6520 7374 616e 6461 7264 206f 7220 6375  e standard or cu
+00000fc0: 7374 6f6d 2061 6e6f 6d61 6c79 2064 6574  stom anomaly det
+00000fd0: 6563 7469 6f6e 206d 6f64 656c 732e 0a0a  ection models...
+00000fe0: 2d2d 2d0a 0a23 2047 6574 7469 6e67 2053  ---..# Getting S
+00000ff0: 7461 7274 6564 0a0a 466f 6c6c 6f77 696e  tarted..Followin
+00001000: 6720 6973 2061 2067 7569 6465 206f 6e20  g is a guide on 
+00001010: 686f 7720 746f 2067 6574 2073 7461 7274  how to get start
+00001020: 6564 2077 6974 6820 6061 6e6f 6d61 6c69  ed with `anomali
+00001030: 6260 2e20 466f 7220 6d6f 7265 2064 6574  b`. For more det
+00001040: 6169 6c73 2c20 6c6f 6f6b 2061 7420 7468  ails, look at th
+00001050: 6520 5b44 6f63 756d 656e 7461 7469 6f6e  e [Documentation
+00001060: 5d28 6874 7470 733a 2f2f 6f70 656e 7669  ](https://openvi
+00001070: 6e6f 746f 6f6c 6b69 742e 6769 7468 7562  notoolkit.github
+00001080: 2e69 6f2f 616e 6f6d 616c 6962 292e 0a0a  .io/anomalib)...
+00001090: 2323 204a 7570 7974 6572 204e 6f74 6562  ## Jupyter Noteb
+000010a0: 6f6f 6b73 0a0a 466f 7220 6765 7474 696e  ooks..For gettin
+000010b0: 6720 7374 6172 7465 6420 7769 7468 2061  g started with a
+000010c0: 204a 7570 7974 6572 204e 6f74 6562 6f6f   Jupyter Noteboo
+000010d0: 6b2c 2070 6c65 6173 6520 7265 6665 7220  k, please refer 
+000010e0: 746f 2074 6865 205b 4e6f 7465 626f 6f6b  to the [Notebook
+000010f0: 735d 286e 6f74 6562 6f6f 6b73 2920 666f  s](notebooks) fo
+00001100: 6c64 6572 206f 6620 7468 6973 2072 6570  lder of this rep
+00001110: 6f73 6974 6f72 792e 2041 6464 6974 696f  ository. Additio
+00001120: 6e61 6c6c 792c 2079 6f75 2063 616e 2072  nally, you can r
+00001130: 6566 6572 2074 6f20 6120 6665 7720 6372  efer to a few cr
+00001140: 6561 7465 6420 6279 2074 6865 2063 6f6d  eated by the com
+00001150: 6d75 6e69 7479 3a0a 0a23 2320 5079 5049  munity:..## PyPI
+00001160: 2049 6e73 7461 6c6c 0a0a 596f 7520 6361   Install..You ca
+00001170: 6e20 6765 7420 7374 6172 7465 6420 7769  n get started wi
+00001180: 7468 2060 616e 6f6d 616c 6962 6020 6279  th `anomalib` by
+00001190: 206a 7573 7420 7573 696e 6720 7069 702e   just using pip.
+000011a0: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
+000011b0: 7374 616c 6c20 616e 6f6d 616c 6962 0a60  stall anomalib.`
+000011c0: 6060 0a0a 2323 204c 6f63 616c 2049 6e73  ``..## Local Ins
+000011d0: 7461 6c6c 0a0a 4974 2069 7320 6869 6768  tall..It is high
+000011e0: 6c79 2072 6563 6f6d 6d65 6e64 6564 2074  ly recommended t
+000011f0: 6f20 7573 6520 7669 7274 7561 6c20 656e  o use virtual en
+00001200: 7669 726f 6e6d 656e 7420 7768 656e 2069  vironment when i
+00001210: 6e73 7461 6c6c 696e 6720 616e 6f6d 616c  nstalling anomal
+00001220: 6962 2e20 466f 7220 696e 7374 616e 6365  ib. For instance
+00001230: 2c20 7769 7468 205b 616e 6163 6f6e 6461  , with [anaconda
+00001240: 5d28 6874 7470 733a 2f2f 7777 772e 616e  ](https://www.an
+00001250: 6163 6f6e 6461 2e63 6f6d 2f70 726f 6475  aconda.com/produ
+00001260: 6374 732f 696e 6469 7669 6475 616c 292c  cts/individual),
+00001270: 2060 616e 6f6d 616c 6962 6020 636f 756c   `anomalib` coul
+00001280: 6420 6265 2069 6e73 7461 6c6c 6564 2061  d be installed a
+00001290: 732c 0a0a 6060 6062 6173 680a 7965 7320  s,..```bash.yes 
+000012a0: 7c20 636f 6e64 6120 6372 6561 7465 202d  | conda create -
+000012b0: 6e20 616e 6f6d 616c 6962 5f65 6e76 2070  n anomalib_env p
+000012c0: 7974 686f 6e3d 332e 380a 636f 6e64 6120  ython=3.8.conda 
+000012d0: 6163 7469 7661 7465 2061 6e6f 6d61 6c69  activate anomali
+000012e0: 625f 656e 760a 6769 7420 636c 6f6e 6520  b_env.git clone 
+000012f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001300: 6f6d 2f6f 7065 6e76 696e 6f74 6f6f 6c6b  om/openvinotoolk
+00001310: 6974 2f61 6e6f 6d61 6c69 622e 6769 740a  it/anomalib.git.
+00001320: 6364 2061 6e6f 6d61 6c69 620a 7069 7020  cd anomalib.pip 
+00001330: 696e 7374 616c 6c20 2d65 202e 0a60 6060  install -e ..```
+00001340: 0a0a 2320 5472 6169 6e69 6e67 0a0a 4279  ..# Training..By
+00001350: 2064 6566 6175 6c74 205b 6070 7974 686f   default [`pytho
+00001360: 6e20 746f 6f6c 732f 7472 6169 6e2e 7079  n tools/train.py
+00001370: 605d 2874 6f6f 6c73 2f74 7261 696e 2e70  `](tools/train.p
+00001380: 7929 0a72 756e 7320 5b50 4144 494d 5d28  y).runs [PADIM](
+00001390: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+000013a0: 672f 6162 732f 3230 3131 2e30 3837 3835  g/abs/2011.08785
+000013b0: 2920 6d6f 6465 6c20 6f6e 2060 6c65 6174  ) model on `leat
+000013c0: 6865 7260 2063 6174 6567 6f72 7920 6672  her` category fr
+000013d0: 6f6d 2074 6865 205b 4d56 5465 6320 4144  om the [MVTec AD
+000013e0: 5d28 6874 7470 733a 2f2f 7777 772e 6d76  ](https://www.mv
+000013f0: 7465 632e 636f 6d2f 636f 6d70 616e 792f  tec.com/company/
+00001400: 7265 7365 6172 6368 2f64 6174 6173 6574  research/dataset
+00001410: 732f 6d76 7465 632d 6164 2920 5b28 4343  s/mvtec-ad) [(CC
+00001420: 2042 592d 4e43 2d53 4120 342e 3029 5d28   BY-NC-SA 4.0)](
+00001430: 6874 7470 733a 2f2f 6372 6561 7469 7665  https://creative
+00001440: 636f 6d6d 6f6e 732e 6f72 672f 6c69 6365  commons.org/lice
+00001450: 6e73 6573 2f62 792d 6e63 2d73 612f 342e  nses/by-nc-sa/4.
+00001460: 302f 2920 6461 7461 7365 742e 0a0a 6060  0/) dataset...``
+00001470: 6062 6173 680a 7079 7468 6f6e 2074 6f6f  `bash.python too
+00001480: 6c73 2f74 7261 696e 2e70 7920 2020 2023  ls/train.py    #
+00001490: 2054 7261 696e 2050 4144 494d 206f 6e20   Train PADIM on 
+000014a0: 4d56 5465 6320 4144 206c 6561 7468 6572  MVTec AD leather
+000014b0: 0a60 6060 0a0a 5472 6169 6e69 6e67 2061  .```..Training a
+000014c0: 206d 6f64 656c 206f 6e20 6120 7370 6563   model on a spec
+000014d0: 6966 6963 2064 6174 6173 6574 2061 6e64  ific dataset and
+000014e0: 2063 6174 6567 6f72 7920 7265 7175 6972   category requir
+000014f0: 6573 2066 7572 7468 6572 2063 6f6e 6669  es further confi
+00001500: 6775 7261 7469 6f6e 2e20 4561 6368 206d  guration. Each m
+00001510: 6f64 656c 2068 6173 2069 7473 206f 776e  odel has its own
+00001520: 2063 6f6e 6669 6775 7261 7469 6f6e 0a66   configuration.f
+00001530: 696c 652c 205b 6063 6f6e 6669 672e 7961  ile, [`config.ya
+00001540: 6d6c 605d 2873 7263 2f61 6e6f 6d61 6c69  ml`](src/anomali
+00001550: 622f 6d6f 6465 6c73 2f70 6164 696d 2f63  b/models/padim/c
+00001560: 6f6e 6669 672e 7961 6d6c 290a 2c20 7768  onfig.yaml)., wh
+00001570: 6963 6820 636f 6e74 6169 6e73 2064 6174  ich contains dat
+00001580: 612c 206d 6f64 656c 2061 6e64 2074 7261  a, model and tra
+00001590: 696e 696e 6720 636f 6e66 6967 7572 6162  ining configurab
+000015a0: 6c65 2070 6172 616d 6574 6572 732e 2054  le parameters. T
+000015b0: 6f20 7472 6169 6e20 6120 7370 6563 6966  o train a specif
+000015c0: 6963 206d 6f64 656c 206f 6e20 6120 7370  ic model on a sp
+000015d0: 6563 6966 6963 2064 6174 6173 6574 2061  ecific dataset a
+000015e0: 6e64 0a63 6174 6567 6f72 792c 2074 6865  nd.category, the
+000015f0: 2063 6f6e 6669 6720 6669 6c65 2069 7320   config file is 
+00001600: 746f 2062 6520 7072 6f76 6964 6564 3a0a  to be provided:.
+00001610: 0a60 6060 6261 7368 0a70 7974 686f 6e20  .```bash.python 
+00001620: 746f 6f6c 732f 7472 6169 6e2e 7079 202d  tools/train.py -
+00001630: 2d63 6f6e 6669 6720 3c70 6174 682f 746f  -config <path/to
+00001640: 2f6d 6f64 656c 2f63 6f6e 6669 672e 7961  /model/config.ya
+00001650: 6d6c 3e0a 6060 600a 0a46 6f72 2065 7861  ml>.```..For exa
+00001660: 6d70 6c65 2c20 746f 2074 7261 696e 205b  mple, to train [
+00001670: 5041 4449 4d5d 2873 7263 2f61 6e6f 6d61  PADIM](src/anoma
+00001680: 6c69 622f 6d6f 6465 6c73 2f70 6164 696d  lib/models/padim
+00001690: 2920 796f 7520 6361 6e20 7573 650a 0a60  ) you can use..`
+000016a0: 6060 6261 7368 0a70 7974 686f 6e20 746f  ``bash.python to
+000016b0: 6f6c 732f 7472 6169 6e2e 7079 202d 2d63  ols/train.py --c
+000016c0: 6f6e 6669 6720 7372 632f 616e 6f6d 616c  onfig src/anomal
+000016d0: 6962 2f6d 6f64 656c 732f 7061 6469 6d2f  ib/models/padim/
+000016e0: 636f 6e66 6967 2e79 616d 6c0a 6060 600a  config.yaml.```.
+000016f0: 0a41 6c74 6572 6e61 7469 7665 6c79 2c20  .Alternatively, 
+00001700: 6120 6d6f 6465 6c20 6e61 6d65 2063 6f75  a model name cou
+00001710: 6c64 2061 6c73 6f20 6265 2070 726f 7669  ld also be provi
+00001720: 6465 6420 6173 2061 6e20 6172 6775 6d65  ded as an argume
+00001730: 6e74 2c20 7768 6572 6520 7468 6520 7363  nt, where the sc
+00001740: 7269 7074 7320 6175 746f 6d61 7469 6361  ripts automatica
+00001750: 6c6c 7920 6669 6e64 7320 7468 6520 636f  lly finds the co
+00001760: 7272 6573 706f 6e64 696e 6720 636f 6e66  rresponding conf
+00001770: 6967 2066 696c 652e 0a0a 6060 6062 6173  ig file...```bas
+00001780: 680a 7079 7468 6f6e 2074 6f6f 6c73 2f74  h.python tools/t
+00001790: 7261 696e 2e70 7920 2d2d 6d6f 6465 6c20  rain.py --model 
+000017a0: 7061 6469 6d0a 6060 600a 0a77 6865 7265  padim.```..where
+000017b0: 2074 6865 2063 7572 7265 6e74 6c79 2061   the currently a
+000017c0: 7661 696c 6162 6c65 206d 6f64 656c 7320  vailable models 
+000017d0: 6172 653a 0a0a 2d20 5b43 4641 5d28 7372  are:..- [CFA](sr
+000017e0: 632f 616e 6f6d 616c 6962 2f6d 6f64 656c  c/anomalib/model
+000017f0: 732f 6366 6129 0a2d 205b 4346 6c6f 775d  s/cfa).- [CFlow]
+00001800: 2873 7263 2f61 6e6f 6d61 6c69 622f 6d6f  (src/anomalib/mo
+00001810: 6465 6c73 2f63 666c 6f77 290a 2d20 5b44  dels/cflow).- [D
+00001820: 464b 4445 5d28 7372 632f 616e 6f6d 616c  FKDE](src/anomal
+00001830: 6962 2f6d 6f64 656c 732f 6466 6b64 6529  ib/models/dfkde)
+00001840: 0a2d 205b 4446 4d5d 2873 7263 2f61 6e6f  .- [DFM](src/ano
+00001850: 6d61 6c69 622f 6d6f 6465 6c73 2f64 666d  malib/models/dfm
+00001860: 290a 2d20 5b44 5241 454d 5d28 7372 632f  ).- [DRAEM](src/
+00001870: 616e 6f6d 616c 6962 2f6d 6f64 656c 732f  anomalib/models/
+00001880: 6472 6165 6d29 0a2d 205b 4661 7374 466c  draem).- [FastFl
+00001890: 6f77 5d28 7372 632f 616e 6f6d 616c 6962  ow](src/anomalib
+000018a0: 2f6d 6f64 656c 732f 6661 7374 666c 6f77  /models/fastflow
+000018b0: 290a 2d20 5b47 414e 6f6d 616c 795d 2873  ).- [GANomaly](s
+000018c0: 7263 2f61 6e6f 6d61 6c69 622f 6d6f 6465  rc/anomalib/mode
+000018d0: 6c73 2f67 616e 6f6d 616c 7929 0a2d 205b  ls/ganomaly).- [
+000018e0: 5041 4449 4d5d 2873 7263 2f61 6e6f 6d61  PADIM](src/anoma
+000018f0: 6c69 622f 6d6f 6465 6c73 2f70 6164 696d  lib/models/padim
+00001900: 290a 2d20 5b50 6174 6368 436f 7265 5d28  ).- [PatchCore](
+00001910: 7372 632f 616e 6f6d 616c 6962 2f6d 6f64  src/anomalib/mod
+00001920: 656c 732f 7061 7463 6863 6f72 6529 0a2d  els/patchcore).-
+00001930: 205b 5265 7665 7273 6520 4469 7374 696c   [Reverse Distil
+00001940: 6c61 7469 6f6e 5d28 7372 632f 616e 6f6d  lation](src/anom
+00001950: 616c 6962 2f6d 6f64 656c 732f 7265 7665  alib/models/reve
+00001960: 7273 655f 6469 7374 696c 6c61 7469 6f6e  rse_distillation
+00001970: 290a 2d20 5b53 5446 504d 5d28 7372 632f  ).- [STFPM](src/
+00001980: 616e 6f6d 616c 6962 2f6d 6f64 656c 732f  anomalib/models/
+00001990: 7374 6670 6d29 0a0a 2323 2046 6561 7475  stfpm)..## Featu
+000019a0: 7265 2065 7874 7261 6374 696f 6e20 2620  re extraction & 
+000019b0: 2870 7265 2d74 7261 696e 6564 2920 6261  (pre-trained) ba
+000019c0: 636b 626f 6e65 730a 0a54 6865 2070 7265  ckbones..The pre
+000019d0: 2d74 7261 696e 6564 2062 6163 6b62 6f6e  -trained backbon
+000019e0: 6573 2063 6f6d 6520 6672 6f6d 205b 5079  es come from [Py
+000019f0: 546f 7263 6820 496d 6167 6520 4d6f 6465  Torch Image Mode
+00001a00: 6c73 2028 7469 6d6d 295d 2868 7474 7073  ls (timm)](https
+00001a10: 3a2f 2f67 6974 6875 622e 636f 6d2f 7277  ://github.com/rw
+00001a20: 6967 6874 6d61 6e2f 7079 746f 7263 682d  ightman/pytorch-
+00001a30: 696d 6167 652d 6d6f 6465 6c73 292c 2077  image-models), w
+00001a40: 6869 6368 2061 7265 2077 7261 7070 6564  hich are wrapped
+00001a50: 2062 7920 6046 6561 7475 7265 4578 7472   by `FeatureExtr
+00001a60: 6163 746f 7260 2e0a 0a46 6f72 206d 6f72  actor`...For mor
+00001a70: 6520 696e 666f 726d 6174 696f 6e2c 2070  e information, p
+00001a80: 6c65 6173 6520 6368 6563 6b20 6f75 7220  lease check our 
+00001a90: 646f 6375 6d65 6e74 6174 696f 6e20 6f72  documentation or
+00001aa0: 2074 6865 205b 7365 6374 696f 6e20 6162   the [section ab
+00001ab0: 6f75 7420 6665 6174 7572 6520 6578 7472  out feature extr
+00001ac0: 6163 7469 6f6e 2069 6e20 2247 6574 7469  action in "Getti
+00001ad0: 6e67 2053 7461 7274 6564 2077 6974 6820  ng Started with 
+00001ae0: 5079 546f 7263 6820 496d 6167 6520 4d6f  PyTorch Image Mo
+00001af0: 6465 6c73 2028 7469 6d6d 293a 2041 2050  dels (timm): A P
+00001b00: 7261 6374 6974 696f 6e65 72e2 8099 7320  ractitioner...s 
+00001b10: 4775 6964 6522 5d28 6874 7470 733a 2f2f  Guide"](https://
+00001b20: 746f 7761 7264 7364 6174 6173 6369 656e  towardsdatascien
+00001b30: 6365 2e63 6f6d 2f67 6574 7469 6e67 2d73  ce.com/getting-s
+00001b40: 7461 7274 6564 2d77 6974 682d 7079 746f  tarted-with-pyto
+00001b50: 7263 682d 696d 6167 652d 6d6f 6465 6c73  rch-image-models
+00001b60: 2d74 696d 6d2d 612d 7072 6163 7469 7469  -timm-a-practiti
+00001b70: 6f6e 6572 732d 6775 6964 652d 3465 3737  oners-guide-4e77
+00001b80: 6234 6266 3930 3535 2362 3833 623a 7e3a  b4bf9055#b83b:~:
+00001b90: 7465 7874 3d72 6561 6479 2532 3074 6f25  text=ready%20to%
+00001ba0: 3230 7472 6169 6e21 2d2c 4665 6174 7572  20train!-,Featur
+00001bb0: 6525 3230 4578 7472 6163 7469 6f6e 2c2d  e%20Extraction,-
+00001bc0: 7469 6d6d 2532 306d 6f64 656c 7325 3230  timm%20models%20
+00001bd0: 616c 736f 3e29 2e0a 0a54 6970 733a 0a0a  also>)...Tips:..
+00001be0: 2d20 5061 7065 7273 2057 6974 6820 436f  - Papers With Co
+00001bf0: 6465 2068 6173 2061 6e20 696e 7465 7266  de has an interf
+00001c00: 6163 6520 746f 2065 6173 696c 7920 6272  ace to easily br
+00001c10: 6f77 7365 206d 6f64 656c 7320 6176 6169  owse models avai
+00001c20: 6c61 626c 6520 696e 2074 696d 6d3a 205b  lable in timm: [
+00001c30: 6874 7470 733a 2f2f 7061 7065 7273 7769  https://paperswi
+00001c40: 7468 636f 6465 2e63 6f6d 2f6c 6962 2f74  thcode.com/lib/t
+00001c50: 696d 6d5d 2868 7474 7073 3a2f 2f70 6170  imm](https://pap
+00001c60: 6572 7377 6974 6863 6f64 652e 636f 6d2f  erswithcode.com/
+00001c70: 6c69 622f 7469 6d6d 290a 0a2d 2059 6f75  lib/timm)..- You
+00001c80: 2063 616e 2061 6c73 6f20 6669 6e64 2074   can also find t
+00001c90: 6865 6d20 7769 7468 2074 6865 2066 756e  hem with the fun
+00001ca0: 6374 696f 6e20 6074 696d 6d2e 6c69 7374  ction `timm.list
+00001cb0: 5f6d 6f64 656c 7328 2272 6573 6e65 742a  _models("resnet*
+00001cc0: 222c 2070 7265 7472 6169 6e65 643d 5472  ", pretrained=Tr
+00001cd0: 7565 2960 0a0a 5468 6520 6261 636b 626f  ue)`..The backbo
+00001ce0: 6e65 2063 616e 2062 6520 7365 7420 696e  ne can be set in
+00001cf0: 2074 6865 2063 6f6e 6669 6720 6669 6c65   the config file
+00001d00: 2c20 7477 6f20 6578 616d 706c 6573 2062  , two examples b
+00001d10: 656c 6f77 2e0a 0a60 6060 7961 6d6c 0a6d  elow...```yaml.m
+00001d20: 6f64 656c 3a0a 2020 6e61 6d65 3a20 6366  odel:.  name: cf
+00001d30: 6c6f 770a 2020 6261 636b 626f 6e65 3a20  low.  backbone: 
+00001d40: 7769 6465 5f72 6573 6e65 7435 305f 320a  wide_resnet50_2.
+00001d50: 2020 7072 655f 7472 6169 6e65 643a 2074    pre_trained: t
+00001d60: 7275 650a 6060 600a 0a23 2320 4375 7374  rue.```..## Cust
+00001d70: 6f6d 2044 6174 6173 6574 0a0a 4974 2069  om Dataset..It i
+00001d80: 7320 616c 736f 2070 6f73 7369 626c 6520  s also possible 
+00001d90: 746f 2074 7261 696e 206f 6e20 6120 6375  to train on a cu
+00001da0: 7374 6f6d 2066 6f6c 6465 7220 6461 7461  stom folder data
+00001db0: 7365 742e 2054 6f20 646f 2073 6f2c 2060  set. To do so, `
+00001dc0: 6461 7461 6020 7365 6374 696f 6e20 696e  data` section in
+00001dd0: 2060 636f 6e66 6967 2e79 616d 6c60 2069   `config.yaml` i
+00001de0: 7320 746f 2062 6520 6d6f 6469 6669 6564  s to be modified
+00001df0: 2061 7320 666f 6c6c 6f77 733a 0a0a 6060   as follows:..``
+00001e00: 6079 616d 6c0a 6461 7461 7365 743a 0a20  `yaml.dataset:. 
+00001e10: 206e 616d 653a 203c 6e61 6d65 2d6f 662d   name: <name-of-
+00001e20: 7468 652d 6461 7461 7365 743e 0a20 2066  the-dataset>.  f
+00001e30: 6f72 6d61 743a 2066 6f6c 6465 720a 2020  ormat: folder.  
+00001e40: 7061 7468 3a20 3c70 6174 682f 746f 2f66  path: <path/to/f
+00001e50: 6f6c 6465 722f 6461 7461 7365 743e 0a20  older/dataset>. 
+00001e60: 206e 6f72 6d61 6c5f 6469 723a 206e 6f72   normal_dir: nor
+00001e70: 6d61 6c20 2320 6e61 6d65 206f 6620 7468  mal # name of th
+00001e80: 6520 666f 6c64 6572 2063 6f6e 7461 696e  e folder contain
+00001e90: 696e 6720 6e6f 726d 616c 2069 6d61 6765  ing normal image
+00001ea0: 732e 0a20 2061 626e 6f72 6d61 6c5f 6469  s..  abnormal_di
+00001eb0: 723a 2061 626e 6f72 6d61 6c20 2320 6e61  r: abnormal # na
+00001ec0: 6d65 206f 6620 7468 6520 666f 6c64 6572  me of the folder
+00001ed0: 2063 6f6e 7461 696e 696e 6720 6162 6e6f   containing abno
+00001ee0: 726d 616c 2069 6d61 6765 732e 0a20 206e  rmal images..  n
+00001ef0: 6f72 6d61 6c5f 7465 7374 5f64 6972 3a20  ormal_test_dir: 
+00001f00: 6e75 6c6c 2023 206e 616d 6520 6f66 2074  null # name of t
+00001f10: 6865 2066 6f6c 6465 7220 636f 6e74 6169  he folder contai
+00001f20: 6e69 6e67 206e 6f72 6d61 6c20 7465 7374  ning normal test
+00001f30: 2069 6d61 6765 732e 0a20 2074 6173 6b3a   images..  task:
+00001f40: 2073 6567 6d65 6e74 6174 696f 6e20 2320   segmentation # 
+00001f50: 636c 6173 7369 6669 6361 7469 6f6e 206f  classification o
+00001f60: 7220 7365 676d 656e 7461 7469 6f6e 0a20  r segmentation. 
+00001f70: 206d 6173 6b3a 203c 7061 7468 2f74 6f2f   mask: <path/to/
+00001f80: 6d61 736b 2f61 6e6e 6f74 6174 696f 6e73  mask/annotations
+00001f90: 3e20 236f 7074 696f 6e61 6c0a 2020 6578  > #optional.  ex
+00001fa0: 7465 6e73 696f 6e73 3a20 6e75 6c6c 0a20  tensions: null. 
+00001fb0: 2073 706c 6974 5f72 6174 696f 3a20 302e   split_ratio: 0.
+00001fc0: 3220 2320 7261 7469 6f20 6f66 2074 6865  2 # ratio of the
+00001fd0: 206e 6f72 6d61 6c20 696d 6167 6573 2074   normal images t
+00001fe0: 6861 7420 7769 6c6c 2062 6520 7573 6564  hat will be used
+00001ff0: 2074 6f20 6372 6561 7465 2061 2074 6573   to create a tes
+00002000: 7420 7370 6c69 740a 2020 696d 6167 655f  t split.  image_
+00002010: 7369 7a65 3a20 3235 360a 2020 7472 6169  size: 256.  trai
+00002020: 6e5f 6261 7463 685f 7369 7a65 3a20 3332  n_batch_size: 32
+00002030: 0a20 2074 6573 745f 6261 7463 685f 7369  .  test_batch_si
+00002040: 7a65 3a20 3332 0a20 206e 756d 5f77 6f72  ze: 32.  num_wor
+00002050: 6b65 7273 3a20 380a 2020 7472 616e 7366  kers: 8.  transf
+00002060: 6f72 6d5f 636f 6e66 6967 3a0a 2020 2020  orm_config:.    
+00002070: 7472 6169 6e3a 206e 756c 6c0a 2020 2020  train: null.    
+00002080: 7661 6c3a 206e 756c 6c0a 2020 6372 6561  val: null.  crea
+00002090: 7465 5f76 616c 6964 6174 696f 6e5f 7365  te_validation_se
+000020a0: 743a 2074 7275 650a 2020 7469 6c69 6e67  t: true.  tiling
+000020b0: 3a0a 2020 2020 6170 706c 793a 2066 616c  :.    apply: fal
+000020c0: 7365 0a20 2020 2074 696c 655f 7369 7a65  se.    tile_size
+000020d0: 3a20 6e75 6c6c 0a20 2020 2073 7472 6964  : null.    strid
+000020e0: 653a 206e 756c 6c0a 2020 2020 7265 6d6f  e: null.    remo
+000020f0: 7665 5f62 6f72 6465 725f 636f 756e 743a  ve_border_count:
+00002100: 2030 0a20 2020 2075 7365 5f72 616e 646f   0.    use_rando
+00002110: 6d5f 7469 6c69 6e67 3a20 4661 6c73 650a  m_tiling: False.
+00002120: 2020 2020 7261 6e64 6f6d 5f74 696c 655f      random_tile_
+00002130: 636f 756e 743a 2031 360a 6060 600a 0a23  count: 16.```..#
+00002140: 2049 6e66 6572 656e 6365 0a0a 416e 6f6d   Inference..Anom
+00002150: 616c 6962 2069 6e63 6c75 6465 7320 6d75  alib includes mu
+00002160: 6c74 6970 6c65 2074 6f6f 6c73 2c20 696e  ltiple tools, in
+00002170: 636c 7564 696e 6720 4c69 6768 746e 696e  cluding Lightnin
+00002180: 672c 2047 7261 6469 6f2c 2061 6e64 204f  g, Gradio, and O
+00002190: 7065 6e56 494e 4f20 696e 6665 7265 6e63  penVINO inferenc
+000021a0: 6572 732c 2066 6f72 2070 6572 666f 726d  ers, for perform
+000021b0: 696e 6720 696e 6665 7265 6e63 6520 7769  ing inference wi
+000021c0: 7468 2061 2074 7261 696e 6564 206d 6f64  th a trained mod
+000021d0: 656c 2e0a 0a54 6865 2066 6f6c 6c6f 7769  el...The followi
+000021e0: 6e67 2063 6f6d 6d61 6e64 2063 616e 2062  ng command can b
+000021f0: 6520 7573 6564 2074 6f20 7275 6e20 5079  e used to run Py
+00002200: 546f 7263 6820 4c69 6768 746e 696e 6720  Torch Lightning 
+00002210: 696e 6665 7265 6e63 6520 6672 6f6d 2074  inference from t
+00002220: 6865 2063 6f6d 6d61 6e64 206c 696e 653a  he command line:
+00002230: 0a0a 6060 6062 6173 680a 7079 7468 6f6e  ..```bash.python
+00002240: 2074 6f6f 6c73 2f69 6e66 6572 656e 6365   tools/inference
+00002250: 2f6c 6967 6874 6e69 6e67 5f69 6e66 6572  /lightning_infer
+00002260: 656e 6365 2e70 7920 2d68 0a60 6060 0a0a  ence.py -h.```..
+00002270: 4173 2061 2071 7569 636b 2065 7861 6d70  As a quick examp
+00002280: 6c65 3a0a 0a60 6060 6261 7368 0a70 7974  le:..```bash.pyt
+00002290: 686f 6e20 746f 6f6c 732f 696e 6665 7265  hon tools/infere
+000022a0: 6e63 652f 6c69 6768 746e 696e 675f 696e  nce/lightning_in
+000022b0: 6665 7265 6e63 652e 7079 205c 0a20 2020  ference.py \.   
+000022c0: 202d 2d63 6f6e 6669 6720 7372 632f 616e   --config src/an
+000022d0: 6f6d 616c 6962 2f6d 6f64 656c 732f 7061  omalib/models/pa
+000022e0: 6469 6d2f 636f 6e66 6967 2e79 616d 6c20  dim/config.yaml 
+000022f0: 5c0a 2020 2020 2d2d 7765 6967 6874 7320  \.    --weights 
+00002300: 7265 7375 6c74 732f 7061 6469 6d2f 6d76  results/padim/mv
+00002310: 7465 632f 626f 7474 6c65 2f72 756e 2f77  tec/bottle/run/w
+00002320: 6569 6768 7473 2f6d 6f64 656c 2e63 6b70  eights/model.ckp
+00002330: 7420 5c0a 2020 2020 2d2d 696e 7075 7420  t \.    --input 
+00002340: 6461 7461 7365 7473 2f4d 5654 6563 2f62  datasets/MVTec/b
+00002350: 6f74 746c 652f 7465 7374 2f62 726f 6b65  ottle/test/broke
+00002360: 6e5f 6c61 7267 652f 3030 302e 706e 6720  n_large/000.png 
+00002370: 5c0a 2020 2020 2d2d 6f75 7470 7574 2072  \.    --output r
+00002380: 6573 756c 7473 2f70 6164 696d 2f6d 7674  esults/padim/mvt
+00002390: 6563 2f62 6f74 746c 652f 696d 6167 6573  ec/bottle/images
+000023a0: 0a60 6060 0a0a 4578 616d 706c 6520 4f70  .```..Example Op
+000023b0: 656e 5649 4e4f 2049 6e66 6572 656e 6365  enVINO Inference
+000023c0: 3a0a 0a60 6060 6261 7368 0a70 7974 686f  :..```bash.pytho
+000023d0: 6e20 746f 6f6c 732f 696e 6665 7265 6e63  n tools/inferenc
+000023e0: 652f 6f70 656e 7669 6e6f 5f69 6e66 6572  e/openvino_infer
+000023f0: 656e 6365 2e70 7920 5c0a 2020 2020 2d2d  ence.py \.    --
+00002400: 7765 6967 6874 7320 7265 7375 6c74 732f  weights results/
+00002410: 7061 6469 6d2f 6d76 7465 632f 626f 7474  padim/mvtec/bott
+00002420: 6c65 2f72 756e 2f6f 7065 6e76 696e 6f2f  le/run/openvino/
+00002430: 6d6f 6465 6c2e 6269 6e20 5c0a 2020 2020  model.bin \.    
+00002440: 2d2d 6d65 7461 6461 7461 2072 6573 756c  --metadata resul
+00002450: 7473 2f70 6164 696d 2f6d 7674 6563 2f62  ts/padim/mvtec/b
+00002460: 6f74 746c 652f 7275 6e2f 6f70 656e 7669  ottle/run/openvi
+00002470: 6e6f 2f6d 6574 6164 6174 612e 6a73 6f6e  no/metadata.json
+00002480: 205c 0a20 2020 202d 2d69 6e70 7574 2064   \.    --input d
+00002490: 6174 6173 6574 732f 4d56 5465 632f 626f  atasets/MVTec/bo
+000024a0: 7474 6c65 2f74 6573 742f 6272 6f6b 656e  ttle/test/broken
+000024b0: 5f6c 6172 6765 2f30 3030 2e70 6e67 205c  _large/000.png \
+000024c0: 0a20 2020 202d 2d6f 7574 7075 7420 7265  .    --output re
+000024d0: 7375 6c74 732f 7061 6469 6d2f 6d76 7465  sults/padim/mvte
+000024e0: 632f 626f 7474 6c65 2f69 6d61 6765 730a  c/bottle/images.
+000024f0: 6060 600a 0a3e 2045 6e73 7572 6520 7468  ```..> Ensure th
+00002500: 6174 2079 6f75 2070 726f 7669 6465 2070  at you provide p
+00002510: 6174 6820 746f 2060 6d65 7461 6461 7461  ath to `metadata
+00002520: 2e6a 736f 6e60 2069 6620 796f 7520 7761  .json` if you wa
+00002530: 6e74 2074 6865 206e 6f72 6d61 6c69 7a61  nt the normaliza
+00002540: 7469 6f6e 2074 6f20 6265 2061 7070 6c69  tion to be appli
+00002550: 6564 2063 6f72 7265 6374 6c79 2e0a 0a59  ed correctly...Y
+00002560: 6f75 2063 616e 2061 6c73 6f20 7573 6520  ou can also use 
+00002570: 4772 6164 696f 2049 6e66 6572 656e 6365  Gradio Inference
+00002580: 2074 6f20 696e 7465 7261 6374 2077 6974   to interact wit
+00002590: 6820 7468 6520 7472 6169 6e65 6420 6d6f  h the trained mo
+000025a0: 6465 6c73 2075 7369 6e67 2061 2055 492e  dels using a UI.
+000025b0: 2052 6566 6572 2074 6f20 6f75 7220 5b67   Refer to our [g
+000025c0: 7569 6465 5d28 6874 7470 733a 2f2f 6f70  uide](https://op
+000025d0: 656e 7669 6e6f 746f 6f6c 6b69 742e 6769  envinotoolkit.gi
+000025e0: 7468 7562 2e69 6f2f 616e 6f6d 616c 6962  thub.io/anomalib
+000025f0: 2f74 7574 6f72 6961 6c73 2f69 6e66 6572  /tutorials/infer
+00002600: 656e 6365 2e68 746d 6c23 6772 6164 696f  ence.html#gradio
+00002610: 2d69 6e66 6572 656e 6365 2920 666f 7220  -inference) for 
+00002620: 6d6f 7265 2064 6574 6169 6c73 2e0a 0a41  more details...A
+00002630: 2071 7569 636b 2065 7861 6d70 6c65 3a0a   quick example:.
+00002640: 0a60 6060 6261 7368 0a70 7974 686f 6e20  .```bash.python 
+00002650: 746f 6f6c 732f 696e 6665 7265 6e63 652f  tools/inference/
+00002660: 6772 6164 696f 5f69 6e66 6572 656e 6365  gradio_inference
+00002670: 2e70 7920 5c0a 2020 2020 2020 2020 2d2d  .py \.        --
+00002680: 7765 6967 6874 7320 7265 7375 6c74 732f  weights results/
+00002690: 7061 6469 6d2f 6d76 7465 632f 626f 7474  padim/mvtec/bott
+000026a0: 6c65 2f72 756e 2f77 6569 6768 7473 2f6d  le/run/weights/m
+000026b0: 6f64 656c 2e63 6b70 740a 6060 600a 0a23  odel.ckpt.```..#
+000026c0: 2320 4578 706f 7274 696e 6720 4d6f 6465  # Exporting Mode
+000026d0: 6c20 746f 204f 4e4e 5820 6f72 204f 7065  l to ONNX or Ope
+000026e0: 6e56 494e 4f20 4952 0a0a 4974 2069 7320  nVINO IR..It is 
+000026f0: 706f 7373 6962 6c65 2074 6f20 6578 706f  possible to expo
+00002700: 7274 2079 6f75 7220 6d6f 6465 6c20 746f  rt your model to
+00002710: 204f 4e4e 5820 6f72 204f 7065 6e56 494e   ONNX or OpenVIN
+00002720: 4f20 4952 0a0a 4966 2079 6f75 2077 616e  O IR..If you wan
+00002730: 7420 746f 2065 7870 6f72 7420 796f 7572  t to export your
+00002740: 2050 7954 6f72 6368 206d 6f64 656c 2074   PyTorch model t
+00002750: 6f20 616e 204f 7065 6e56 494e 4f20 6d6f  o an OpenVINO mo
+00002760: 6465 6c2c 2065 6e73 7572 6520 7468 6174  del, ensure that
+00002770: 2060 6578 706f 7274 5f6d 6f64 6560 2069   `export_mode` i
+00002780: 7320 7365 7420 746f 2060 226f 7065 6e76  s set to `"openv
+00002790: 696e 6f22 6020 696e 2074 6865 2072 6573  ino"` in the res
+000027a0: 7065 6374 6976 6520 6d6f 6465 6c20 6063  pective model `c
+000027b0: 6f6e 6669 672e 7961 6d6c 602e 0a0a 6060  onfig.yaml`...``
+000027c0: 6079 616d 6c0a 6f70 7469 6d69 7a61 7469  `yaml.optimizati
+000027d0: 6f6e 3a0a 2020 6578 706f 7274 5f6d 6f64  on:.  export_mod
+000027e0: 653a 2022 6f70 656e 7669 6e6f 2220 2320  e: "openvino" # 
+000027f0: 6f70 7469 6f6e 733a 206f 7065 6e76 696e  options: openvin
+00002800: 6f2c 206f 6e6e 780a 6060 600a 0a23 2048  o, onnx.```..# H
+00002810: 7970 6572 7061 7261 6d65 7465 7220 4f70  yperparameter Op
+00002820: 7469 6d69 7a61 7469 6f6e 0a0a 546f 2072  timization..To r
+00002830: 756e 2068 7970 6572 7061 7261 6d65 7465  un hyperparamete
+00002840: 7220 6f70 7469 6d69 7a61 7469 6f6e 2c20  r optimization, 
+00002850: 7573 6520 7468 6520 666f 6c6c 6f77 696e  use the followin
+00002860: 6720 636f 6d6d 616e 643a 0a0a 6060 6062  g command:..```b
+00002870: 6173 680a 7079 7468 6f6e 2074 6f6f 6c73  ash.python tools
+00002880: 2f68 706f 2f73 7765 6570 2e70 7920 5c0a  /hpo/sweep.py \.
+00002890: 2020 2020 2d2d 6d6f 6465 6c20 7061 6469      --model padi
+000028a0: 6d20 2d2d 6d6f 6465 6c5f 636f 6e66 6967  m --model_config
+000028b0: 202e 2f70 6174 685f 746f 5f63 6f6e 6669   ./path_to_confi
+000028c0: 672e 7961 6d6c 205c 0a20 2020 202d 2d73  g.yaml \.    --s
+000028d0: 7765 6570 5f63 6f6e 6669 6720 746f 6f6c  weep_config tool
+000028e0: 732f 6870 6f2f 7377 6565 702e 7961 6d6c  s/hpo/sweep.yaml
+000028f0: 0a60 6060 0a0a 466f 7220 6d6f 7265 2064  .```..For more d
+00002900: 6574 6169 6c73 2072 6566 6572 2074 6865  etails refer the
+00002910: 205b 4850 4f20 446f 6375 6d65 6e74 6174   [HPO Documentat
+00002920: 696f 6e5d 2868 7474 7073 3a2f 2f6f 7065  ion](https://ope
+00002930: 6e76 696e 6f74 6f6f 6c6b 6974 2e67 6974  nvinotoolkit.git
+00002940: 6875 622e 696f 2f61 6e6f 6d61 6c69 622f  hub.io/anomalib/
+00002950: 7475 746f 7269 616c 732f 6879 7065 7270  tutorials/hyperp
+00002960: 6172 616d 6574 6572 5f6f 7074 696d 697a  arameter_optimiz
+00002970: 6174 696f 6e2e 6874 6d6c 290a 0a23 2042  ation.html)..# B
+00002980: 656e 6368 6d61 726b 696e 670a 0a54 6f20  enchmarking..To 
+00002990: 6761 7468 6572 2062 656e 6368 6d61 726b  gather benchmark
+000029a0: 696e 6720 6461 7461 2073 7563 6820 6173  ing data such as
+000029b0: 2074 6872 6f75 6768 7075 7420 6163 726f   throughput acro
+000029c0: 7373 2063 6174 6567 6f72 6965 732c 2075  ss categories, u
+000029d0: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
+000029e0: 2063 6f6d 6d61 6e64 3a0a 0a60 6060 6261   command:..```ba
+000029f0: 7368 0a70 7974 686f 6e20 746f 6f6c 732f  sh.python tools/
+00002a00: 6265 6e63 686d 6172 6b69 6e67 2f62 656e  benchmarking/ben
+00002a10: 6368 6d61 726b 2e70 7920 5c0a 2020 2020  chmark.py \.    
+00002a20: 2d2d 636f 6e66 6967 203c 7265 6c61 7469  --config <relati
+00002a30: 7665 2f61 6273 6f6c 7574 6520 7061 7468  ve/absolute path
+00002a40: 3e2f 3c70 6172 616d 6669 6c65 3e2e 7961  >/<paramfile>.ya
+00002a50: 6d6c 0a60 6060 0a0a 5265 6665 7220 746f  ml.```..Refer to
+00002a60: 2074 6865 205b 4265 6e63 686d 6172 6b69   the [Benchmarki
+00002a70: 6e67 2044 6f63 756d 656e 7461 7469 6f6e  ng Documentation
+00002a80: 5d28 6874 7470 733a 2f2f 6f70 656e 7669  ](https://openvi
+00002a90: 6e6f 746f 6f6c 6b69 742e 6769 7468 7562  notoolkit.github
+00002aa0: 2e69 6f2f 616e 6f6d 616c 6962 2f74 7574  .io/anomalib/tut
+00002ab0: 6f72 6961 6c73 2f62 656e 6368 6d61 726b  orials/benchmark
+00002ac0: 696e 672e 6874 6d6c 2920 666f 7220 6d6f  ing.html) for mo
+00002ad0: 7265 2064 6574 6169 6c73 2e0a 0a23 2045  re details...# E
+00002ae0: 7870 6572 696d 656e 7420 4d61 6e61 6765  xperiment Manage
+00002af0: 6d65 6e74 0a0a 416e 6f6d 6162 6c69 6220  ment..Anomablib 
+00002b00: 6973 2069 6e74 6567 7261 7465 6420 7769  is integrated wi
+00002b10: 7468 2076 6172 696f 7573 206c 6962 7261  th various libra
+00002b20: 7269 6573 2066 6f72 2065 7870 6572 696d  ries for experim
+00002b30: 656e 7420 7472 6163 6b69 6e67 2073 7563  ent tracking suc
+00002b40: 6820 6173 2043 6f6d 6574 2c20 7465 6e73  h as Comet, tens
+00002b50: 6f72 626f 6172 642c 2061 6e64 2077 616e  orboard, and wan
+00002b60: 6462 2074 6872 6f75 6768 205b 7079 746f  db through [pyto
+00002b70: 7263 6820 6c69 6768 7469 6e67 206c 6f67  rch lighting log
+00002b80: 6765 7273 5d28 6874 7470 733a 2f2f 7079  gers](https://py
+00002b90: 746f 7263 682d 6c69 6768 746e 696e 672e  torch-lightning.
+00002ba0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00002bb0: 6e2f 7374 6162 6c65 2f65 7874 656e 7369  n/stable/extensi
+00002bc0: 6f6e 732f 6c6f 6767 696e 672e 6874 6d6c  ons/logging.html
+00002bd0: 292e 0a0a 4265 6c6f 7720 6973 2061 6e20  )...Below is an 
+00002be0: 6578 616d 706c 6520 6f66 2068 6f77 2074  example of how t
+00002bf0: 6f20 656e 6162 6c65 206c 6f67 6769 6e67  o enable logging
+00002c00: 2066 6f72 2068 7970 6572 2d70 6172 616d   for hyper-param
+00002c10: 6574 6572 732c 206d 6574 7269 6373 2c20  eters, metrics, 
+00002c20: 6d6f 6465 6c20 6772 6170 6873 2c20 616e  model graphs, an
+00002c30: 6420 7072 6564 6963 7469 6f6e 7320 6f6e  d predictions on
+00002c40: 2069 6d61 6765 7320 696e 2074 6865 2074   images in the t
+00002c50: 6573 7420 6461 7461 2d73 6574 0a0a 6060  est data-set..``
+00002c60: 6079 616d 6c0a 7669 7375 616c 697a 6174  `yaml.visualizat
+00002c70: 696f 6e3a 0a20 206c 6f67 5f69 6d61 6765  ion:.  log_image
+00002c80: 733a 2054 7275 6520 2320 6c6f 6720 696d  s: True # log im
+00002c90: 6167 6573 2074 6f20 7468 6520 6176 6169  ages to the avai
+00002ca0: 6c61 626c 6520 6c6f 6767 6572 7320 2869  lable loggers (i
+00002cb0: 6620 616e 7929 0a20 206d 6f64 653a 2066  f any).  mode: f
+00002cc0: 756c 6c20 2320 6f70 7469 6f6e 733a 205b  ull # options: [
+00002cd0: 2266 756c 6c22 2c20 2273 696d 706c 6522  "full", "simple"
+00002ce0: 5d0a 0a20 6c6f 6767 696e 673a 0a20 206c  ].. logging:.  l
+00002cf0: 6f67 6765 723a 205b 636f 6d65 742c 2074  ogger: [comet, t
+00002d00: 656e 736f 7262 6f61 7264 2c20 7761 6e64  ensorboard, wand
+00002d10: 625d 0a20 206c 6f67 5f67 7261 7068 3a20  b].  log_graph: 
+00002d20: 5472 7565 0a60 6060 0a0a 466f 7220 6d6f  True.```..For mo
+00002d30: 7265 2069 6e66 6f72 6d61 7469 6f6e 2c20  re information, 
+00002d40: 7265 6665 7220 746f 2074 6865 205b 4c6f  refer to the [Lo
+00002d50: 6767 696e 6720 446f 6375 6d65 6e74 6174  gging Documentat
+00002d60: 696f 6e5d 2868 7474 7073 3a2f 2f6f 7065  ion](https://ope
+00002d70: 6e76 696e 6f74 6f6f 6c6b 6974 2e67 6974  nvinotoolkit.git
+00002d80: 6875 622e 696f 2f61 6e6f 6d61 6c69 622f  hub.io/anomalib/
+00002d90: 7475 746f 7269 616c 732f 6c6f 6767 696e  tutorials/loggin
+00002da0: 672e 6874 6d6c 290a 0a4e 6f74 653a 2053  g.html)..Note: S
+00002db0: 6574 2079 6f75 7220 4150 4920 4b65 7920  et your API Key 
+00002dc0: 666f 7220 5b43 6f6d 6574 2e6d 6c5d 2868  for [Comet.ml](h
+00002dd0: 7474 7073 3a2f 2f77 7777 2e63 6f6d 6574  ttps://www.comet
+00002de0: 2e63 6f6d 2f73 6967 6e75 703f 7574 6d5f  .com/signup?utm_
+00002df0: 736f 7572 6365 3d61 6e6f 6d61 6c69 6226  source=anomalib&
+00002e00: 7574 6d5f 6d65 6469 756d 3d72 6566 6572  utm_medium=refer
+00002e10: 7261 6c29 2076 6961 2060 636f 6d65 745f  ral) via `comet_
+00002e20: 6d6c 2e69 6e69 7428 2960 2069 6e20 696e  ml.init()` in in
+00002e30: 7465 7261 6374 6976 6520 7079 7468 6f6e  teractive python
+00002e40: 206f 7220 7369 6d70 6c79 2072 756e 2060   or simply run `
+00002e50: 6578 706f 7274 2043 4f4d 4554 5f41 5049  export COMET_API
+00002e60: 5f4b 4559 3d3c 596f 7572 2041 5049 204b  _KEY=<Your API K
+00002e70: 6579 3e60 0a0a 2320 436f 6d6d 756e 6974  ey>`..# Communit
+00002e80: 7920 5072 6f6a 6563 7473 0a0a 2323 2031  y Projects..## 1
+00002e90: 2e20 5765 622d 6261 7365 6420 5069 7065  . Web-based Pipe
+00002ea0: 6c69 6e65 2066 6f72 2054 7261 696e 696e  line for Trainin
+00002eb0: 6720 616e 6420 496e 6665 7265 6e63 650a  g and Inference.
+00002ec0: 0a54 6869 7320 7072 6f6a 6563 7420 7368  .This project sh
+00002ed0: 6f77 6361 7365 7320 616e 2065 6e64 2d74  owcases an end-t
+00002ee0: 6f2d 656e 6420 7472 6169 6e69 6e67 2061  o-end training a
+00002ef0: 6e64 2069 6e66 6572 656e 6365 2070 6970  nd inference pip
+00002f00: 656c 696e 6520 6275 696c 6420 6f6e 2074  eline build on t
+00002f10: 6f70 206f 6620 416e 6f6d 616c 6962 2e20  op of Anomalib. 
+00002f20: 4974 2070 726f 7669 6465 7320 6120 7765  It provides a we
+00002f30: 622d 6261 7365 6420 5549 2066 6f72 2075  b-based UI for u
+00002f40: 706c 6f61 6469 6e67 204d 5654 6563 2073  ploading MVTec s
+00002f50: 7479 6c65 2064 6174 6173 6574 7320 616e  tyle datasets an
+00002f60: 6420 7472 6169 6e69 6e67 2074 6865 6d20  d training them 
+00002f70: 6f6e 2074 6865 2061 7661 696c 6162 6c65  on the available
+00002f80: 2041 6e6f 6d61 6c69 6220 6d6f 6465 6c73   Anomalib models
+00002f90: 2e20 4974 2061 6c73 6f20 6861 7320 7365  . It also has se
+00002fa0: 6374 696f 6e73 2066 6f72 2063 616c 6c69  ctions for calli
+00002fb0: 6e67 2069 6e66 6572 656e 6365 206f 6e20  ng inference on 
+00002fc0: 696e 6469 7669 6475 616c 2069 6d61 6765  individual image
+00002fd0: 7320 6173 2077 656c 6c20 6173 206c 6973  s as well as lis
+00002fe0: 7469 6e67 2061 6c6c 2074 6865 2069 6d61  ting all the ima
+00002ff0: 6765 7320 7769 7468 2074 6865 6972 2070  ges with their p
+00003000: 7265 6469 6374 696f 6e73 2069 6e20 7468  redictions in th
+00003010: 6520 6461 7461 6261 7365 2e0a 0a59 6f75  e database...You
+00003020: 2063 616e 2076 6965 7720 7468 6520 7072   can view the pr
+00003030: 6f6a 6563 7420 6f6e 205b 4769 7468 7562  oject on [Github
+00003040: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00003050: 2e63 6f6d 2f76 6e6b 3830 3731 2f61 6e6f  .com/vnk8071/ano
+00003060: 6d61 6c79 2d64 6574 6563 7469 6f6e 2d69  maly-detection-i
+00003070: 6e2d 696e 6475 7374 7279 2d6d 616e 7566  n-industry-manuf
+00003080: 6163 7475 7269 6e67 2f74 7265 652f 6d61  acturing/tree/ma
+00003090: 7374 6572 2f61 6e6f 6d61 6c69 625f 636f  ster/anomalib_co
+000030a0: 6e74 7269 6275 7465 290a 466f 7220 6d6f  ntribute).For mo
+000030b0: 7265 2064 6574 6169 6c73 2073 6565 2074  re details see t
+000030c0: 6865 205b 4469 7363 7573 7369 6f6e 2066  he [Discussion f
+000030d0: 6f72 756d 5d28 6874 7470 733a 2f2f 6769  orum](https://gi
+000030e0: 7468 7562 2e63 6f6d 2f6f 7065 6e76 696e  thub.com/openvin
+000030f0: 6f74 6f6f 6c6b 6974 2f61 6e6f 6d61 6c69  otoolkit/anomali
+00003100: 622f 6469 7363 7573 7369 6f6e 732f 3733  b/discussions/73
+00003110: 3329 0a0a 2320 4461 7461 7365 7473 0a0a  3)..# Datasets..
+00003120: 6061 6e6f 6d61 6c69 6260 2073 7570 706f  `anomalib` suppo
+00003130: 7274 7320 4d56 5465 6320 4144 205b 2843  rts MVTec AD [(C
+00003140: 4320 4259 2d4e 432d 5341 2034 2e30 295d  C BY-NC-SA 4.0)]
+00003150: 2868 7474 7073 3a2f 2f63 7265 6174 6976  (https://creativ
+00003160: 6563 6f6d 6d6f 6e73 2e6f 7267 2f6c 6963  ecommons.org/lic
+00003170: 656e 7365 732f 6279 2d6e 632d 7361 2f34  enses/by-nc-sa/4
+00003180: 2e30 2f29 2061 6e64 2042 6561 6e54 6563  .0/) and BeanTec
+00003190: 6820 5b28 4343 2d42 592d 5341 295d 2868  h [(CC-BY-SA)](h
+000031a0: 7474 7073 3a2f 2f63 7265 6174 6976 6563  ttps://creativec
+000031b0: 6f6d 6d6f 6e73 2e6f 7267 2f6c 6963 656e  ommons.org/licen
+000031c0: 7365 732f 6279 2d73 612f 342e 302f 6c65  ses/by-sa/4.0/le
+000031d0: 6761 6c63 6f64 6529 2066 6f72 2062 656e  galcode) for ben
+000031e0: 6368 6d61 726b 696e 6720 616e 6420 6066  chmarking and `f
+000031f0: 6f6c 6465 7260 2066 6f72 2063 7573 746f  older` for custo
+00003200: 6d20 6461 7461 7365 7420 7472 6169 6e69  m dataset traini
+00003210: 6e67 2f69 6e66 6572 656e 6365 2e0a 0a23  ng/inference...#
+00003220: 2320 5b4d 5654 6563 2041 4420 4461 7461  # [MVTec AD Data
+00003230: 7365 745d 2868 7474 7073 3a2f 2f77 7777  set](https://www
+00003240: 2e6d 7674 6563 2e63 6f6d 2f63 6f6d 7061  .mvtec.com/compa
+00003250: 6e79 2f72 6573 6561 7263 682f 6461 7461  ny/research/data
+00003260: 7365 7473 2f6d 7674 6563 2d61 6429 0a0a  sets/mvtec-ad)..
+00003270: 4d56 5465 6320 4144 2064 6174 6173 6574  MVTec AD dataset
+00003280: 2069 7320 6f6e 6520 6f66 2074 6865 206d   is one of the m
+00003290: 6169 6e20 6265 6e63 686d 6172 6b73 2066  ain benchmarks f
+000032a0: 6f72 2061 6e6f 6d61 6c79 2064 6574 6563  or anomaly detec
+000032b0: 7469 6f6e 2c20 616e 6420 6973 2072 656c  tion, and is rel
+000032c0: 6561 7365 6420 756e 6465 7220 7468 650a  eased under the.
+000032d0: 4372 6561 7469 7665 2043 6f6d 6d6f 6e73  Creative Commons
+000032e0: 2041 7474 7269 6275 7469 6f6e 2d4e 6f6e   Attribution-Non
+000032f0: 436f 6d6d 6572 6369 616c 2d53 6861 7265  Commercial-Share
+00003300: 416c 696b 6520 342e 3020 496e 7465 726e  Alike 4.0 Intern
+00003310: 6174 696f 6e61 6c20 4c69 6365 6e73 6520  ational License 
+00003320: 5b28 4343 2042 592d 4e43 2d53 4120 342e  [(CC BY-NC-SA 4.
+00003330: 3029 5d28 6874 7470 733a 2f2f 6372 6561  0)](https://crea
+00003340: 7469 7665 636f 6d6d 6f6e 732e 6f72 672f  tivecommons.org/
+00003350: 6c69 6365 6e73 6573 2f62 792d 6e63 2d73  licenses/by-nc-s
+00003360: 612f 342e 302f 292e 0a0a 3e20 4e6f 7465  a/4.0/)...> Note
+00003370: 3a20 5468 6573 6520 6d65 7472 6963 7320  : These metrics 
+00003380: 6172 6520 636f 6c6c 6563 7465 6420 7769  are collected wi
+00003390: 7468 2069 6d61 6765 2073 697a 6520 6f66  th image size of
+000033a0: 2032 3536 2061 6e64 2073 6565 6420 6034   256 and seed `4
+000033b0: 3260 2e20 5468 6973 2063 6f6d 6d6f 6e20  2`. This common 
+000033c0: 7365 7474 696e 6720 6973 2075 7365 6420  setting is used 
+000033d0: 746f 206d 616b 6520 6d6f 6465 6c20 636f  to make model co
+000033e0: 6d70 6172 6973 6f6e 7320 6661 6972 2e0a  mparisons fair..
+000033f0: 0a23 2320 496d 6167 652d 4c65 7665 6c20  .## Image-Level 
+00003400: 4155 430a 0a7c 204d 6f64 656c 2020 2020  AUC..| Model    
+00003410: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00003420: 2020 2020 2020 2020 2020 7c20 2020 2041            |    A
+00003430: 7667 2020 2020 7c20 2043 6172 7065 7420  vg    |  Carpet 
+00003440: 2020 7c20 2020 4772 6964 2020 2020 7c20    |   Grid    | 
+00003450: 204c 6561 7468 6572 2020 7c20 2020 5469   Leather  |   Ti
+00003460: 6c65 2020 2020 7c20 2020 576f 6f64 2020  le    |   Wood  
+00003470: 2020 7c20 426f 7474 6c65 2020 7c20 2020    | Bottle  |   
+00003480: 4361 626c 6520 2020 7c20 2043 6170 7375  Cable   |  Capsu
+00003490: 6c65 2020 7c20 4861 7a65 6c6e 7574 207c  le  | Hazelnut |
+000034a0: 204d 6574 616c 204e 7574 207c 2020 2050   Metal Nut |   P
+000034b0: 696c 6c20 2020 207c 2020 2053 6372 6577  ill    |   Screw
+000034c0: 2020 207c 2054 6f6f 7468 6272 7573 6820     | Toothbrush 
+000034d0: 7c20 5472 616e 7369 7374 6f72 207c 2020  | Transistor |  
+000034e0: 5a69 7070 6572 2020 207c 0a7c 202d 2d2d  Zipper   |.| ---
+000034f0: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  ---------- | ---
+00003500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  --------------- 
+00003510: 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d  | :-------: | :-
+00003520: 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d  ------: | :-----
+00003530: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20  --: | :-------: 
+00003540: 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d  | :-------: | :-
+00003550: 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d  ------: | :-----
+00003560: 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20  : | :-------: | 
+00003570: 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d  :-------: | :---
+00003580: 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d 2d3a  ---: | :-------:
+00003590: 207c 203a 2d2d 2d2d 2d2d 2d3a 207c 203a   | :-------: | :
+000035a0: 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d  -------: | :----
+000035b0: 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d  ----: | :-------
+000035c0: 2d3a 207c 203a 2d2d 2d2d 2d2d 2d3a 207c  -: | :-------: |
+000035d0: 0a7c 202a 2a50 6174 6368 436f 7265 2a2a  .| **PatchCore**
+000035e0: 207c 202a 2a57 6964 6520 5265 734e 6574   | **Wide ResNet
+000035f0: 2d35 302a 2a20 7c20 2a2a 302e 3938 302a  -50** | **0.980*
+00003600: 2a20 7c20 2020 302e 3938 3420 2020 7c20  * |   0.984   | 
+00003610: 2020 302e 3935 3920 2020 7c20 2020 312e    0.959   |   1.
+00003620: 3030 3020 2020 7c20 2a2a 312e 3030 302a  000   | **1.000*
+00003630: 2a20 7c20 2020 302e 3938 3920 2020 7c20  * |   0.989   | 
+00003640: 2031 2e30 3030 2020 7c20 2a2a 302e 3939   1.000  | **0.99
+00003650: 302a 2a20 7c20 2a2a 302e 3938 322a 2a20  0** | **0.982** 
+00003660: 7c20 2031 2e30 3030 2020 207c 2020 2030  |  1.000   |   0
+00003670: 2e39 3934 2020 207c 2020 2030 2e39 3234  .994   |   0.924
+00003680: 2020 207c 2020 2030 2e39 3630 2020 207c     |   0.960   |
+00003690: 2020 2030 2e39 3333 2020 2020 7c20 2a2a     0.933    | **
+000036a0: 312e 3030 302a 2a20 207c 2020 2030 2e39  1.000**  |   0.9
+000036b0: 3832 2020 207c 0a7c 2050 6174 6368 436f  82   |.| PatchCo
+000036c0: 7265 2020 2020 207c 2052 6573 4e65 742d  re     | ResNet-
+000036d0: 3138 2020 2020 2020 2020 2020 7c20 2020  18          |   
+000036e0: 302e 3937 3320 2020 7c20 2020 302e 3937  0.973   |   0.97
+000036f0: 3020 2020 7c20 2020 302e 3934 3720 2020  0   |   0.947   
+00003700: 7c20 2020 312e 3030 3020 2020 7c20 2020  |   1.000   |   
+00003710: 302e 3939 3720 2020 7c20 2020 302e 3939  0.997   |   0.99
+00003720: 3720 2020 7c20 2031 2e30 3030 2020 7c20  7   |  1.000  | 
+00003730: 2020 302e 3938 3620 2020 7c20 2020 302e    0.986   |   0.
+00003740: 3936 3520 2020 7c20 2031 2e30 3030 2020  965   |  1.000  
+00003750: 207c 2020 2030 2e39 3931 2020 207c 2020   |   0.991   |  
+00003760: 2030 2e39 3136 2020 207c 202a 2a30 2e39   0.916   | **0.9
+00003770: 3433 2a2a 207c 2020 2030 2e39 3331 2020  43** |   0.931  
+00003780: 2020 7c20 2020 302e 3939 3620 2020 207c    |   0.996    |
+00003790: 2020 2030 2e39 3533 2020 207c 0a7c 2043     0.953   |.| C
+000037a0: 466c 6f77 2020 2020 2020 2020 207c 2057  Flow         | W
+000037b0: 6964 6520 5265 734e 6574 2d35 3020 2020  ide ResNet-50   
+000037c0: 2020 7c20 2020 302e 3936 3220 2020 7c20    |   0.962   | 
+000037d0: 2020 302e 3938 3620 2020 7c20 2020 302e    0.986   |   0.
+000037e0: 3936 3220 2020 7c20 2a2a 312e 3030 302a  962   | **1.000*
+000037f0: 2a20 7c20 2020 302e 3939 3920 2020 7c20  * |   0.999   | 
+00003800: 2020 302e 3939 3320 2020 7c20 2a2a 312e    0.993   | **1.
+00003810: 302a 2a20 7c20 2020 302e 3839 3320 2020  0** |   0.893   
+00003820: 7c20 2020 302e 3934 3520 2020 7c20 2a2a  |   0.945   | **
+00003830: 312e 302a 2a20 207c 202a 2a30 2e39 3935  1.0**  | **0.995
+00003840: 2a2a 207c 2020 2030 2e39 3234 2020 207c  ** |   0.924   |
+00003850: 2020 2030 2e39 3038 2020 207c 2020 2030     0.908   |   0
+00003860: 2e38 3937 2020 2020 7c20 2020 302e 3934  .897    |   0.94
+00003870: 3320 2020 207c 202a 2a30 2e39 3834 2a2a  3    | **0.984**
+00003880: 207c 0a7c 2043 4641 2020 2020 2020 2020   |.| CFA        
+00003890: 2020 207c 2057 6964 6520 5265 734e 6574     | Wide ResNet
+000038a0: 2d35 3020 2020 2020 7c20 2020 302e 3935  -50     |   0.95
+000038b0: 3620 2020 7c20 2020 302e 3937 3820 2020  6   |   0.978   
+000038c0: 7c20 2020 302e 3936 3120 2020 7c20 2020  |   0.961   |   
+000038d0: 302e 3939 3020 2020 7c20 2020 302e 3939  0.990   |   0.99
+000038e0: 3920 2020 7c20 2020 302e 3939 3420 2020  9   |   0.994   
+000038f0: 7c20 2030 2e39 3938 2020 7c20 2020 302e  |  0.998  |   0.
+00003900: 3937 3920 2020 7c20 2020 302e 3837 3220  979   |   0.872 
+00003910: 2020 7c20 2031 2e30 3030 2020 207c 202a    |  1.000   | *
+00003920: 2a30 2e39 3935 2a2a 207c 202a 2a30 2e39  *0.995** | **0.9
+00003930: 3436 2a2a 207c 2020 2030 2e37 3033 2020  46** |   0.703  
+00003940: 207c 202a 2a31 2e30 3030 2a2a 2020 7c20   | **1.000**  | 
+00003950: 2020 302e 3935 3720 2020 207c 2020 2030    0.957    |   0
+00003960: 2e39 3637 2020 207c 0a7c 2043 4641 2020  .967   |.| CFA  
+00003970: 2020 2020 2020 2020 207c 2052 6573 4e65           | ResNe
+00003980: 742d 3138 2020 2020 2020 2020 2020 7c20  t-18          | 
+00003990: 2020 302e 3933 3020 2020 7c20 2020 302e    0.930   |   0.
+000039a0: 3935 3320 2020 7c20 2020 302e 3934 3720  953   |   0.947 
+000039b0: 2020 7c20 2020 302e 3939 3920 2020 7c20    |   0.999   | 
+000039c0: 2020 312e 3030 3020 2020 7c20 2a2a 312e    1.000   | **1.
+000039d0: 3030 302a 2a20 7c20 2030 2e39 3931 2020  000** |  0.991  
+000039e0: 7c20 2020 302e 3934 3720 2020 7c20 2020  |   0.947   |   
+000039f0: 302e 3835 3820 2020 7c20 2030 2e39 3935  0.858   |  0.995
+00003a00: 2020 207c 2020 2030 2e39 3332 2020 207c     |   0.932   |
+00003a10: 2020 2030 2e38 3837 2020 207c 2020 2030     0.887   |   0
+00003a20: 2e36 3235 2020 207c 2020 2030 2e39 3934  .625   |   0.994
+00003a30: 2020 2020 7c20 2020 302e 3839 3520 2020      |   0.895   
+00003a40: 207c 2020 2030 2e39 3139 2020 207c 0a7c   |   0.919   |.|
+00003a50: 2050 6144 694d 2020 2020 2020 2020 207c   PaDiM         |
+00003a60: 2057 6964 6520 5265 734e 6574 2d35 3020   Wide ResNet-50 
+00003a70: 2020 2020 7c20 2020 302e 3935 3020 2020      |   0.950   
+00003a80: 7c20 2a2a 302e 3939 352a 2a20 7c20 2020  | **0.995** |   
+00003a90: 302e 3934 3220 2020 7c20 2a2a 312e 3030  0.942   | **1.00
+00003aa0: 302a 2a20 7c20 2020 302e 3937 3420 2020  0** |   0.974   
+00003ab0: 7c20 2020 302e 3939 3320 2020 7c20 2030  |   0.993   |  0
+00003ac0: 2e39 3939 2020 7c20 2020 302e 3837 3820  .999  |   0.878 
+00003ad0: 2020 7c20 2020 302e 3932 3720 2020 7c20    |   0.927   | 
+00003ae0: 2030 2e39 3634 2020 207c 2020 2030 2e39   0.964   |   0.9
+00003af0: 3839 2020 207c 2020 2030 2e39 3339 2020  89   |   0.939  
+00003b00: 207c 2020 2030 2e38 3435 2020 207c 2020   |   0.845   |  
+00003b10: 2030 2e39 3432 2020 2020 7c20 2020 302e   0.942    |   0.
+00003b20: 3937 3620 2020 207c 2020 2030 2e38 3832  976    |   0.882
+00003b30: 2020 207c 0a7c 2050 6144 694d 2020 2020     |.| PaDiM    
+00003b40: 2020 2020 207c 2052 6573 4e65 742d 3138       | ResNet-18
+00003b50: 2020 2020 2020 2020 2020 7c20 2020 302e            |   0.
+00003b60: 3839 3120 2020 7c20 2020 302e 3934 3520  891   |   0.945 
+00003b70: 2020 7c20 2020 302e 3835 3720 2020 7c20    |   0.857   | 
+00003b80: 2020 302e 3938 3220 2020 7c20 2020 302e    0.982   |   0.
+00003b90: 3935 3020 2020 7c20 2020 302e 3937 3620  950   |   0.976 
+00003ba0: 2020 7c20 2030 2e39 3934 2020 7c20 2020    |  0.994  |   
+00003bb0: 302e 3834 3420 2020 7c20 2020 302e 3930  0.844   |   0.90
+00003bc0: 3120 2020 7c20 2030 2e37 3530 2020 207c  1   |  0.750   |
+00003bd0: 2020 2030 2e39 3631 2020 207c 2020 2030     0.961   |   0
+00003be0: 2e38 3633 2020 207c 2020 2030 2e37 3539  .863   |   0.759
+00003bf0: 2020 207c 2020 2030 2e38 3839 2020 2020     |   0.889    
+00003c00: 7c20 2020 302e 3932 3020 2020 207c 2020  |   0.920    |  
+00003c10: 2030 2e37 3830 2020 207c 0a7c 2044 464d   0.780   |.| DFM
+00003c20: 2020 2020 2020 2020 2020 207c 2057 6964             | Wid
+00003c30: 6520 5265 734e 6574 2d35 3020 2020 2020  e ResNet-50     
+00003c40: 7c20 2020 302e 3934 3320 2020 7c20 2020  |   0.943   |   
+00003c50: 302e 3835 3520 2020 7c20 2020 302e 3738  0.855   |   0.78
+00003c60: 3420 2020 7c20 2020 302e 3939 3720 2020  4   |   0.997   
+00003c70: 7c20 2020 302e 3939 3520 2020 7c20 2020  |   0.995   |   
+00003c80: 302e 3937 3520 2020 7c20 2030 2e39 3939  0.975   |  0.999
+00003c90: 2020 7c20 2020 302e 3936 3920 2020 7c20    |   0.969   | 
+00003ca0: 2020 302e 3932 3420 2020 7c20 2030 2e39    0.924   |  0.9
+00003cb0: 3738 2020 207c 2020 2030 2e39 3339 2020  78   |   0.939  
+00003cc0: 207c 2020 2030 2e39 3632 2020 207c 2020   |   0.962   |  
+00003cd0: 2030 2e38 3733 2020 207c 2020 2030 2e39   0.873   |   0.9
+00003ce0: 3639 2020 2020 7c20 2020 302e 3937 3120  69    |   0.971 
+00003cf0: 2020 207c 2020 2030 2e39 3631 2020 207c     |   0.961   |
+00003d00: 0a7c 2044 464d 2020 2020 2020 2020 2020  .| DFM          
+00003d10: 207c 2052 6573 4e65 742d 3138 2020 2020   | ResNet-18    
+00003d20: 2020 2020 2020 7c20 2020 302e 3933 3620        |   0.936 
+00003d30: 2020 7c20 2020 302e 3831 3720 2020 7c20    |   0.817   | 
+00003d40: 2020 302e 3733 3620 2020 7c20 2020 302e    0.736   |   0.
+00003d50: 3939 3320 2020 7c20 2020 302e 3936 3620  993   |   0.966 
+00003d60: 2020 7c20 2020 302e 3937 3720 2020 7c20    |   0.977   | 
+00003d70: 2031 2e30 3030 2020 7c20 2020 302e 3935   1.000  |   0.95
+00003d80: 3620 2020 7c20 2020 302e 3934 3420 2020  6   |   0.944   
+00003d90: 7c20 2030 2e39 3934 2020 207c 2020 2030  |  0.994   |   0
+00003da0: 2e39 3232 2020 207c 2020 2030 2e39 3631  .922   |   0.961
+00003db0: 2020 207c 2020 2030 2e38 3920 2020 207c     |   0.89    |
+00003dc0: 2020 2030 2e39 3639 2020 2020 7c20 2020     0.969    |   
+00003dd0: 302e 3933 3920 2020 207c 2020 2030 2e39  0.939    |   0.9
+00003de0: 3639 2020 207c 0a7c 2053 5446 504d 2020  69   |.| STFPM  
+00003df0: 2020 2020 2020 207c 2057 6964 6520 5265         | Wide Re
+00003e00: 734e 6574 2d35 3020 2020 2020 7c20 2020  sNet-50     |   
+00003e10: 302e 3837 3620 2020 7c20 2020 302e 3935  0.876   |   0.95
+00003e20: 3720 2020 7c20 2020 302e 3937 3720 2020  7   |   0.977   
+00003e30: 7c20 2020 302e 3938 3120 2020 7c20 2020  |   0.981   |   
+00003e40: 302e 3937 3620 2020 7c20 2020 302e 3933  0.976   |   0.93
+00003e50: 3920 2020 7c20 2030 2e39 3837 2020 7c20  9   |  0.987  | 
+00003e60: 2020 302e 3837 3820 2020 7c20 2020 302e    0.878   |   0.
+00003e70: 3733 3220 2020 7c20 2030 2e39 3935 2020  732   |  0.995  
+00003e80: 207c 2020 2030 2e39 3733 2020 207c 2020   |   0.973   |  
+00003e90: 2030 2e36 3532 2020 207c 2020 2030 2e38   0.652   |   0.8
+00003ea0: 3235 2020 207c 2020 2030 2e35 3030 2020  25   |   0.500  
+00003eb0: 2020 7c20 2020 302e 3837 3520 2020 207c    |   0.875    |
+00003ec0: 2020 2030 2e38 3939 2020 207c 0a7c 2053     0.899   |.| S
+00003ed0: 5446 504d 2020 2020 2020 2020 207c 2052  TFPM         | R
+00003ee0: 6573 4e65 742d 3138 2020 2020 2020 2020  esNet-18        
+00003ef0: 2020 7c20 2020 302e 3839 3320 2020 7c20    |   0.893   | 
+00003f00: 2020 302e 3935 3420 2020 7c20 2a2a 302e    0.954   | **0.
+00003f10: 3938 322a 2a20 7c20 2020 302e 3938 3920  982** |   0.989 
+00003f20: 2020 7c20 2020 302e 3934 3920 2020 7c20    |   0.949   | 
+00003f30: 2020 302e 3936 3120 2020 7c20 2030 2e39    0.961   |  0.9
+00003f40: 3739 2020 7c20 2020 302e 3833 3820 2020  79  |   0.838   
+00003f50: 7c20 2020 302e 3735 3920 2020 7c20 2030  |   0.759   |  0
+00003f60: 2e39 3939 2020 207c 2020 2030 2e39 3536  .999   |   0.956
+00003f70: 2020 207c 2020 2030 2e37 3035 2020 207c     |   0.705   |
+00003f80: 2020 2030 2e38 3335 2020 207c 202a 2a30     0.835   | **0
+00003f90: 2e39 3937 2a2a 2020 7c20 2020 302e 3835  .997**  |   0.85
+00003fa0: 3320 2020 207c 2020 2030 2e36 3435 2020  3    |   0.645  
+00003fb0: 207c 0a7c 2044 464b 4445 2020 2020 2020   |.| DFKDE      
+00003fc0: 2020 207c 2057 6964 6520 5265 734e 6574     | Wide ResNet
+00003fd0: 2d35 3020 2020 2020 7c20 2020 302e 3737  -50     |   0.77
+00003fe0: 3420 2020 7c20 2020 302e 3730 3820 2020  4   |   0.708   
+00003ff0: 7c20 2020 302e 3432 3220 2020 7c20 2020  |   0.422   |   
+00004000: 302e 3930 3520 2020 7c20 2020 302e 3935  0.905   |   0.95
+00004010: 3920 2020 7c20 2020 302e 3930 3320 2020  9   |   0.903   
+00004020: 7c20 2030 2e39 3336 2020 7c20 2020 302e  |  0.936  |   0.
+00004030: 3734 3620 2020 7c20 2020 302e 3835 3320  746   |   0.853 
+00004040: 2020 7c20 2030 2e37 3336 2020 207c 2020    |  0.736   |  
+00004050: 2030 2e36 3837 2020 207c 2020 2030 2e37   0.687   |   0.7
+00004060: 3439 2020 207c 2020 2030 2e35 3734 2020  49   |   0.574  
+00004070: 207c 2020 2030 2e36 3937 2020 2020 7c20   |   0.697    | 
+00004080: 2020 302e 3834 3320 2020 207c 2020 2030    0.843    |   0
+00004090: 2e38 3932 2020 207c 0a7c 2044 464b 4445  .892   |.| DFKDE
+000040a0: 2020 2020 2020 2020 207c 2052 6573 4e65           | ResNe
+000040b0: 742d 3138 2020 2020 2020 2020 2020 7c20  t-18          | 
+000040c0: 2020 302e 3736 3220 2020 7c20 2020 302e    0.762   |   0.
+000040d0: 3634 3620 2020 7c20 2020 302e 3537 3720  646   |   0.577 
+000040e0: 2020 7c20 2020 302e 3636 3920 2020 7c20    |   0.669   | 
+000040f0: 2020 302e 3936 3520 2020 7c20 2020 302e    0.965   |   0.
+00004100: 3836 3320 2020 7c20 2030 2e39 3531 2020  863   |  0.951  
+00004110: 7c20 2020 302e 3735 3120 2020 7c20 2020  |   0.751   |   
+00004120: 302e 3639 3820 2020 7c20 2030 2e38 3036  0.698   |  0.806
+00004130: 2020 207c 2020 2030 2e37 3239 2020 207c     |   0.729   |
+00004140: 2020 2030 2e36 3037 2020 207c 2020 2030     0.607   |   0
+00004150: 2e36 3934 2020 207c 2020 2030 2e37 3637  .694   |   0.767
+00004160: 2020 2020 7c20 2020 302e 3833 3920 2020      |   0.839   
+00004170: 207c 2020 2030 2e38 3636 2020 207c 0a7c   |   0.866   |.|
+00004180: 2047 414e 6f6d 616c 7920 2020 2020 207c   GANomaly      |
+00004190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041a0: 2020 2020 7c20 2020 302e 3432 3120 2020      |   0.421   
+000041b0: 7c20 2020 302e 3230 3320 2020 7c20 2020  |   0.203   |   
+000041c0: 302e 3430 3420 2020 7c20 2020 302e 3431  0.404   |   0.41
+000041d0: 3320 2020 7c20 2020 302e 3430 3820 2020  3   |   0.408   
+000041e0: 7c20 2020 302e 3734 3420 2020 7c20 2030  |   0.744   |  0
+000041f0: 2e32 3531 2020 7c20 2020 302e 3435 3720  .251  |   0.457 
+00004200: 2020 7c20 2020 302e 3638 3220 2020 7c20    |   0.682   | 
+00004210: 2030 2e35 3337 2020 207c 2020 2030 2e32   0.537   |   0.2
+00004220: 3730 2020 207c 2020 2030 2e34 3732 2020  70   |   0.472  
+00004230: 207c 2020 2030 2e32 3331 2020 207c 2020   |   0.231   |  
+00004240: 2030 2e33 3732 2020 2020 7c20 2020 302e   0.372    |   0.
+00004250: 3434 3020 2020 207c 2020 2030 2e34 3334  440    |   0.434
+00004260: 2020 207c 0a0a 2323 2050 6978 656c 2d4c     |..## Pixel-L
+00004270: 6576 656c 2041 5543 0a0a 7c20 4d6f 6465  evel AUC..| Mode
+00004280: 6c20 2020 2020 7c20 2020 2020 2020 2020  l     |         
+00004290: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+000042a0: 4176 6720 2020 207c 2020 4361 7270 6574  Avg    |  Carpet
+000042b0: 2020 207c 2020 2047 7269 6420 2020 207c     |   Grid    |
+000042c0: 2020 4c65 6174 6865 7220 207c 2020 2054    Leather  |   T
+000042d0: 696c 6520 2020 207c 2020 2057 6f6f 6420  ile    |   Wood 
+000042e0: 2020 207c 2020 426f 7474 6c65 2020 207c     |  Bottle   |
+000042f0: 2020 2043 6162 6c65 2020 207c 2020 4361     Cable   |  Ca
+00004300: 7073 756c 6520 207c 2048 617a 656c 6e75  psule  | Hazelnu
+00004310: 7420 207c 204d 6574 616c 204e 7574 207c  t  | Metal Nut |
+00004320: 2020 2050 696c 6c20 2020 207c 2020 2053     Pill    |   S
+00004330: 6372 6577 2020 207c 2054 6f6f 7468 6272  crew   | Toothbr
+00004340: 7573 6820 7c20 5472 616e 7369 7374 6f72  ush | Transistor
+00004350: 207c 2020 5a69 7070 6572 2020 207c 0a7c   |  Zipper   |.|
+00004360: 202d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d   --------- | ---
+00004370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  --------------- 
+00004380: 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d  | :-------: | :-
+00004390: 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d  ------: | :-----
+000043a0: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20  --: | :-------: 
+000043b0: 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d  | :-------: | :-
+000043c0: 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d  ------: | :-----
+000043d0: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20  --: | :-------: 
+000043e0: 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d  | :-------: | :-
+000043f0: 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d  ------: | :-----
+00004400: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20  --: | :-------: 
+00004410: 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d  | :-------: | :-
+00004420: 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d  -------: | :----
+00004430: 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d  ----: | :-------
+00004440: 3a20 7c0a 7c20 2a2a 4346 412a 2a20 2020  : |.| **CFA**   
+00004450: 7c20 2a2a 5769 6465 2052 6573 4e65 742d  | **Wide ResNet-
+00004460: 3530 2a2a 207c 202a 2a30 2e39 3833 2a2a  50** | **0.983**
+00004470: 207c 2020 2030 2e39 3830 2020 207c 2020   |   0.980   |  
+00004480: 2030 2e39 3534 2020 207c 2020 2030 2e39   0.954   |   0.9
+00004490: 3839 2020 207c 202a 2a30 2e39 3835 2a2a  89   | **0.985**
+000044a0: 207c 202a 2a30 2e39 3734 2a2a 207c 202a   | **0.974** | *
+000044b0: 2a30 2e39 3839 2a2a 207c 202a 2a30 2e39  *0.989** | **0.9
+000044c0: 3838 2a2a 207c 202a 2a30 2e39 3839 2a2a  88** | **0.989**
+000044d0: 207c 2020 2030 2e39 3835 2020 207c 202a   |   0.985   | *
+000044e0: 2a30 2e39 3932 2a2a 207c 202a 2a30 2e39  *0.992** | **0.9
+000044f0: 3838 2a2a 207c 2020 2030 2e39 3739 2020  88** |   0.979  
+00004500: 207c 202a 2a30 2e39 3931 2a2a 2020 7c20   | **0.991**  | 
+00004510: 2020 302e 3937 3720 2020 207c 202a 2a30    0.977    | **0
+00004520: 2e39 3930 2a2a 207c 0a7c 2043 4641 2020  .990** |.| CFA  
+00004530: 2020 2020 207c 2052 6573 4e65 742d 3138       | ResNet-18
+00004540: 2020 2020 2020 2020 2020 7c20 2020 302e            |   0.
+00004550: 3937 3920 2020 7c20 2020 302e 3937 3020  979   |   0.970 
+00004560: 2020 7c20 2020 302e 3937 3320 2020 7c20    |   0.973   | 
+00004570: 2020 302e 3939 3220 2020 7c20 2020 302e    0.992   |   0.
+00004580: 3937 3820 2020 7c20 2020 302e 3936 3420  978   |   0.964 
+00004590: 2020 7c20 2020 302e 3938 3620 2020 7c20    |   0.986   | 
+000045a0: 2020 302e 3938 3420 2020 7c20 2020 302e    0.984   |   0.
+000045b0: 3938 3720 2020 7c20 2020 302e 3938 3720  987   |   0.987 
+000045c0: 2020 7c20 2020 302e 3938 3120 2020 7c20    |   0.981   | 
+000045d0: 2020 302e 3938 3120 2020 7c20 2020 302e    0.981   |   0.
+000045e0: 3937 3320 2020 7c20 2020 302e 3939 3020  973   |   0.990 
+000045f0: 2020 207c 2020 2030 2e39 3634 2020 2020     |   0.964    
+00004600: 7c20 2020 302e 3937 3820 2020 7c0a 7c20  |   0.978   |.| 
+00004610: 5061 7463 6843 6f72 6520 7c20 5769 6465  PatchCore | Wide
+00004620: 2052 6573 4e65 742d 3530 2020 2020 207c   ResNet-50     |
+00004630: 2020 2030 2e39 3830 2020 207c 2020 2030     0.980   |   0
+00004640: 2e39 3838 2020 207c 2020 2030 2e39 3638  .988   |   0.968
+00004650: 2020 207c 2020 2030 2e39 3931 2020 207c     |   0.991   |
+00004660: 2020 2030 2e39 3631 2020 207c 2020 2030     0.961   |   0
+00004670: 2e39 3334 2020 207c 2020 2030 2e39 3834  .934   |   0.984
+00004680: 2020 207c 202a 2a30 2e39 3838 2a2a 207c     | **0.988** |
+00004690: 2020 2030 2e39 3838 2020 207c 2020 2030     0.988   |   0
+000046a0: 2e39 3837 2020 207c 2020 2030 2e39 3839  .987   |   0.989
+000046b0: 2020 207c 2020 2030 2e39 3830 2020 207c     |   0.980   |
+000046c0: 202a 2a30 2e39 3839 2a2a 207c 2020 2030   **0.989** |   0
+000046d0: 2e39 3838 2020 2020 7c20 2a2a 302e 3938  .988    | **0.98
+000046e0: 312a 2a20 207c 2020 2030 2e39 3833 2020  1**  |   0.983  
+000046f0: 207c 0a7c 2050 6174 6368 436f 7265 207c   |.| PatchCore |
+00004700: 2052 6573 4e65 742d 3138 2020 2020 2020   ResNet-18      
+00004710: 2020 2020 7c20 2020 302e 3937 3620 2020      |   0.976   
+00004720: 7c20 2020 302e 3938 3620 2020 7c20 2020  |   0.986   |   
+00004730: 302e 3935 3520 2020 7c20 2020 302e 3939  0.955   |   0.99
+00004740: 3020 2020 7c20 2020 302e 3934 3320 2020  0   |   0.943   
+00004750: 7c20 2020 302e 3933 3320 2020 7c20 2020  |   0.933   |   
+00004760: 302e 3938 3120 2020 7c20 2020 302e 3938  0.981   |   0.98
+00004770: 3420 2020 7c20 2020 302e 3938 3620 2020  4   |   0.986   
+00004780: 7c20 2020 302e 3938 3620 2020 7c20 2020  |   0.986   |   
+00004790: 302e 3938 3620 2020 7c20 2020 302e 3937  0.986   |   0.97
+000047a0: 3420 2020 7c20 2020 302e 3939 3120 2020  4   |   0.991   
+000047b0: 7c20 2020 302e 3938 3820 2020 207c 2020  |   0.988    |  
+000047c0: 2030 2e39 3734 2020 2020 7c20 2020 302e   0.974    |   0.
+000047d0: 3938 3320 2020 7c0a 7c20 4346 6c6f 7720  983   |.| CFlow 
+000047e0: 2020 2020 7c20 5769 6465 2052 6573 4e65      | Wide ResNe
+000047f0: 742d 3530 2020 2020 207c 2020 2030 2e39  t-50     |   0.9
+00004800: 3731 2020 207c 2020 2030 2e39 3836 2020  71   |   0.986  
+00004810: 207c 2020 2030 2e39 3638 2020 207c 2020   |   0.968   |  
+00004820: 2030 2e39 3933 2020 207c 2020 2030 2e39   0.993   |   0.9
+00004830: 3638 2020 207c 2020 2030 2e39 3234 2020  68   |   0.924  
+00004840: 207c 2020 2030 2e39 3831 2020 207c 2020   |   0.981   |  
+00004850: 2030 2e39 3535 2020 207c 2020 2030 2e39   0.955   |   0.9
+00004860: 3838 2020 207c 202a 2a30 2e39 3930 2a2a  88   | **0.990**
+00004870: 207c 2020 2030 2e39 3832 2020 207c 2020   |   0.982   |  
+00004880: 2030 2e39 3833 2020 207c 2020 2030 2e39   0.983   |   0.9
+00004890: 3739 2020 207c 2020 2030 2e39 3835 2020  79   |   0.985  
+000048a0: 2020 7c20 2020 302e 3839 3720 2020 207c    |   0.897    |
+000048b0: 2020 2030 2e39 3830 2020 207c 0a7c 2050     0.980   |.| P
+000048c0: 6144 694d 2020 2020 207c 2057 6964 6520  aDiM     | Wide 
+000048d0: 5265 734e 6574 2d35 3020 2020 2020 7c20  ResNet-50     | 
+000048e0: 2020 302e 3937 3920 2020 7c20 2a2a 302e    0.979   | **0.
+000048f0: 3939 312a 2a20 7c20 2020 302e 3937 3020  991** |   0.970 
+00004900: 2020 7c20 2020 302e 3939 3320 2020 7c20    |   0.993   | 
+00004910: 2020 302e 3935 3520 2020 7c20 2020 302e    0.955   |   0.
+00004920: 3935 3720 2020 7c20 2020 302e 3938 3520  957   |   0.985 
+00004930: 2020 7c20 2020 302e 3937 3020 2020 7c20    |   0.970   | 
+00004940: 2020 302e 3938 3820 2020 7c20 2020 302e    0.988   |   0.
+00004950: 3938 3520 2020 7c20 2020 302e 3938 3220  985   |   0.982 
+00004960: 2020 7c20 2020 302e 3936 3620 2020 7c20    |   0.966   | 
+00004970: 2020 302e 3938 3820 2020 7c20 2a2a 302e    0.988   | **0.
+00004980: 3939 312a 2a20 207c 2020 2030 2e39 3736  991**  |   0.976
+00004990: 2020 2020 7c20 2020 302e 3938 3620 2020      |   0.986   
+000049a0: 7c0a 7c20 5061 4469 4d20 2020 2020 7c20  |.| PaDiM     | 
+000049b0: 5265 734e 6574 2d31 3820 2020 2020 2020  ResNet-18       
+000049c0: 2020 207c 2020 2030 2e39 3638 2020 207c     |   0.968   |
+000049d0: 2020 2030 2e39 3834 2020 207c 2020 2030     0.984   |   0
+000049e0: 2e39 3138 2020 207c 202a 2a30 2e39 3934  .918   | **0.994
+000049f0: 2a2a 207c 2020 2030 2e39 3334 2020 207c  ** |   0.934   |
+00004a00: 2020 2030 2e39 3437 2020 207c 2020 2030     0.947   |   0
+00004a10: 2e39 3833 2020 207c 2020 2030 2e39 3635  .983   |   0.965
+00004a20: 2020 207c 2020 2030 2e39 3834 2020 207c     |   0.984   |
+00004a30: 2020 2030 2e39 3738 2020 207c 2020 2030     0.978   |   0
+00004a40: 2e39 3730 2020 207c 2020 2030 2e39 3537  .970   |   0.957
+00004a50: 2020 207c 2020 2030 2e39 3738 2020 207c     |   0.978   |
+00004a60: 2020 2030 2e39 3838 2020 2020 7c20 2020     0.988    |   
+00004a70: 302e 3936 3820 2020 207c 2020 2030 2e39  0.968    |   0.9
+00004a80: 3739 2020 207c 0a7c 2053 5446 504d 2020  79   |.| STFPM  
+00004a90: 2020 207c 2057 6964 6520 5265 734e 6574     | Wide ResNet
+00004aa0: 2d35 3020 2020 2020 7c20 2020 302e 3930  -50     |   0.90
+00004ab0: 3320 2020 7c20 2020 302e 3938 3720 2020  3   |   0.987   
+00004ac0: 7c20 2a2a 302e 3938 392a 2a20 7c20 2020  | **0.989** |   
+00004ad0: 302e 3938 3020 2020 7c20 2020 302e 3936  0.980   |   0.96
+00004ae0: 3620 2020 7c20 2020 302e 3935 3620 2020  6   |   0.956   
+00004af0: 7c20 2020 302e 3936 3620 2020 7c20 2020  |   0.966   |   
+00004b00: 302e 3931 3320 2020 7c20 2020 302e 3935  0.913   |   0.95
+00004b10: 3620 2020 7c20 2020 302e 3937 3420 2020  6   |   0.974   
+00004b20: 7c20 2020 302e 3936 3120 2020 7c20 2020  |   0.961   |   
+00004b30: 302e 3934 3620 2020 7c20 2020 302e 3938  0.946   |   0.98
+00004b40: 3820 2020 7c20 2020 302e 3137 3820 2020  8   |   0.178   
+00004b50: 207c 2020 2030 2e38 3037 2020 2020 7c20   |   0.807    | 
+00004b60: 2020 302e 3938 3020 2020 7c0a 7c20 5354    0.980   |.| ST
+00004b70: 4650 4d20 2020 2020 7c20 5265 734e 6574  FPM     | ResNet
+00004b80: 2d31 3820 2020 2020 2020 2020 207c 2020  -18          |  
+00004b90: 2030 2e39 3531 2020 207c 2020 2030 2e39   0.951   |   0.9
+00004ba0: 3836 2020 207c 2020 2030 2e39 3838 2020  86   |   0.988  
+00004bb0: 207c 2020 2030 2e39 3931 2020 207c 2020   |   0.991   |  
+00004bc0: 2030 2e39 3436 2020 207c 2020 2030 2e39   0.946   |   0.9
+00004bd0: 3439 2020 207c 2020 2030 2e39 3731 2020  49   |   0.971  
+00004be0: 207c 2020 2030 2e38 3938 2020 207c 2020   |   0.898   |  
+00004bf0: 2030 2e39 3632 2020 207c 2020 2030 2e39   0.962   |   0.9
+00004c00: 3831 2020 207c 2020 2030 2e39 3432 2020  81   |   0.942  
+00004c10: 207c 2020 2030 2e38 3738 2020 207c 2020   |   0.878   |  
+00004c20: 2030 2e39 3833 2020 207c 2020 2030 2e39   0.983   |   0.9
+00004c30: 3833 2020 2020 7c20 2020 302e 3833 3820  83    |   0.838 
+00004c40: 2020 207c 2020 2030 2e39 3732 2020 207c     |   0.972   |
+00004c50: 0a0a 2323 2049 6d61 6765 2046 3120 5363  ..## Image F1 Sc
+00004c60: 6f72 650a 0a7c 204d 6f64 656c 2020 2020  ore..| Model    
+00004c70: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00004c80: 2020 2020 2020 2020 2020 7c20 2020 2041            |    A
+00004c90: 7667 2020 2020 7c20 2043 6172 7065 7420  vg    |  Carpet 
+00004ca0: 2020 7c20 2020 4772 6964 2020 2020 7c20    |   Grid    | 
+00004cb0: 204c 6561 7468 6572 2020 7c20 2020 5469   Leather  |   Ti
+00004cc0: 6c65 2020 2020 7c20 2020 576f 6f64 2020  le    |   Wood  
+00004cd0: 2020 7c20 2042 6f74 746c 6520 2020 7c20    |  Bottle   | 
+00004ce0: 2020 4361 626c 6520 2020 7c20 2043 6170    Cable   |  Cap
+00004cf0: 7375 6c65 2020 7c20 4861 7a65 6c6e 7574  sule  | Hazelnut
+00004d00: 2020 7c20 4d65 7461 6c20 4e75 7420 7c20    | Metal Nut | 
+00004d10: 2020 5069 6c6c 2020 2020 7c20 2020 5363    Pill    |   Sc
+00004d20: 7265 7720 2020 7c20 546f 6f74 6862 7275  rew   | Toothbru
+00004d30: 7368 207c 2054 7261 6e73 6973 746f 7220  sh | Transistor 
+00004d40: 7c20 205a 6970 7065 7220 2020 7c0a 7c20  |  Zipper   |.| 
+00004d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20  ------------- | 
+00004d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004d70: 2d2d 207c 203a 2d2d 2d2d 2d2d 2d3a 207c  -- | :-------: |
+00004d80: 203a 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d   :-------: | :--
+00004d90: 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d  -----: | :------
+00004da0: 2d3a 207c 203a 2d2d 2d2d 2d2d 2d3a 207c  -: | :-------: |
+00004db0: 203a 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d   :-------: | :--
+00004dc0: 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d  -----: | :------
+00004dd0: 2d3a 207c 203a 2d2d 2d2d 2d2d 2d3a 207c  -: | :-------: |
+00004de0: 203a 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d   :-------: | :--
+00004df0: 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d 2d2d  -----: | :------
+00004e00: 2d3a 207c 203a 2d2d 2d2d 2d2d 2d3a 207c  -: | :-------: |
+00004e10: 203a 2d2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d   :--------: | :-
+00004e20: 2d2d 2d2d 2d2d 2d3a 207c 203a 2d2d 2d2d  -------: | :----
+00004e30: 2d2d 2d3a 207c 0a7c 202a 2a50 6174 6368  ---: |.| **Patch
+00004e40: 436f 7265 2a2a 207c 202a 2a57 6964 6520  Core** | **Wide 
+00004e50: 5265 734e 6574 2d35 302a 2a20 7c20 2a2a  ResNet-50** | **
+00004e60: 302e 3937 362a 2a20 7c20 2020 302e 3937  0.976** |   0.97
+00004e70: 3120 2020 7c20 2020 302e 3937 3420 2020  1   |   0.974   
+00004e80: 7c20 2a2a 312e 3030 302a 2a20 7c20 2a2a  | **1.000** | **
+00004e90: 312e 3030 302a 2a20 7c20 2020 302e 3936  1.000** |   0.96
+00004ea0: 3720 2020 7c20 2a2a 312e 3030 302a 2a20  7   | **1.000** 
+00004eb0: 7c20 2020 302e 3936 3820 2020 7c20 2a2a  |   0.968   | **
+00004ec0: 302e 3938 322a 2a20 7c20 2a2a 312e 3030  0.982** | **1.00
+00004ed0: 302a 2a20 7c20 2020 302e 3938 3420 2020  0** |   0.984   
+00004ee0: 7c20 2020 302e 3934 3020 2020 7c20 2020  |   0.940   |   
+00004ef0: 302e 3934 3320 2020 7c20 2020 302e 3933  0.943   |   0.93
+00004f00: 3820 2020 207c 202a 2a31 2e30 3030 2a2a  8    | **1.000**
+00004f10: 2020 7c20 2a2a 302e 3937 392a 2a20 7c0a    | **0.979** |.
+00004f20: 7c20 5061 7463 6843 6f72 6520 2020 2020  | PatchCore     
+00004f30: 7c20 5265 734e 6574 2d31 3820 2020 2020  | ResNet-18     
+00004f40: 2020 2020 207c 2020 2030 2e39 3730 2020       |   0.970  
+00004f50: 207c 2020 2030 2e39 3439 2020 207c 2020   |   0.949   |  
+00004f60: 2030 2e39 3436 2020 207c 202a 2a31 2e30   0.946   | **1.0
+00004f70: 3030 2a2a 207c 2020 2030 2e39 3820 2020  00** |   0.98   
+00004f80: 207c 2020 2030 2e39 3932 2020 207c 202a   |   0.992   | *
+00004f90: 2a31 2e30 3030 2a2a 207c 202a 2a30 2e39  *1.000** | **0.9
+00004fa0: 3738 2a2a 207c 2020 2030 2e39 3639 2020  78** |   0.969  
+00004fb0: 207c 202a 2a31 2e30 3030 2a2a 207c 202a   | **1.000** | *
+00004fc0: 2a30 2e39 3839 2a2a 207c 2020 2030 2e39  *0.989** |   0.9
+00004fd0: 3430 2020 207c 2020 2030 2e39 3332 2020  40   |   0.932  
+00004fe0: 207c 2020 2030 2e39 3335 2020 2020 7c20   |   0.935    | 
+00004ff0: 2020 302e 3937 3420 2020 207c 2020 2030    0.974    |   0
+00005000: 2e39 3637 2020 207c 0a7c 2043 4641 2020  .967   |.| CFA  
+00005010: 2020 2020 2020 2020 207c 2057 6964 6520           | Wide 
+00005020: 5265 734e 6574 2d35 3020 2020 2020 7c20  ResNet-50     | 
+00005030: 2020 302e 3936 3220 2020 7c20 2020 302e    0.962   |   0.
+00005040: 3936 3120 2020 7c20 2020 302e 3935 3720  961   |   0.957 
+00005050: 2020 7c20 2020 302e 3939 3520 2020 7c20    |   0.995   | 
+00005060: 2020 302e 3939 3420 2020 7c20 2020 302e    0.994   |   0.
+00005070: 3938 3320 2020 7c20 2020 302e 3938 3420  983   |   0.984 
+00005080: 2020 7c20 2020 302e 3936 3220 2020 7c20    |   0.962   | 
+00005090: 2020 302e 3934 3620 2020 7c20 2a2a 312e    0.946   | **1.
+000050a0: 3030 302a 2a20 7c20 2020 302e 3938 3420  000** |   0.984 
+000050b0: 2020 7c20 2a2a 302e 3935 322a 2a20 7c20    | **0.952** | 
+000050c0: 2020 302e 3835 3520 2020 7c20 2a2a 312e    0.855   | **1.
+000050d0: 3030 302a 2a20 207c 2020 2030 2e39 3037  000**  |   0.907
+000050e0: 2020 2020 7c20 2020 302e 3937 3520 2020      |   0.975   
+000050f0: 7c0a 7c20 4346 4120 2020 2020 2020 2020  |.| CFA         
+00005100: 2020 7c20 5265 734e 6574 2d31 3820 2020    | ResNet-18   
+00005110: 2020 2020 2020 207c 2020 2030 2e39 3436         |   0.946
+00005120: 2020 207c 2020 2030 2e39 3536 2020 207c     |   0.956   |
+00005130: 2020 2030 2e39 3436 2020 207c 2020 2030     0.946   |   0
+00005140: 2e39 3733 2020 207c 202a 2a31 2e30 3030  .973   | **1.000
+00005150: 2a2a 207c 202a 2a31 2e30 3030 2a2a 207c  ** | **1.000** |
+00005160: 2020 2030 2e39 3833 2020 207c 2020 2030     0.983   |   0
+00005170: 2e39 3037 2020 207c 2020 2030 2e39 3338  .907   |   0.938
+00005180: 2020 207c 2020 2030 2e39 3936 2020 207c     |   0.996   |
+00005190: 2020 2030 2e39 3538 2020 207c 2020 2030     0.958   |   0
+000051a0: 2e39 3230 2020 207c 2020 2030 2e38 3538  .920   |   0.858
+000051b0: 2020 207c 2020 2030 2e39 3834 2020 2020     |   0.984    
+000051c0: 7c20 2020 302e 3739 3520 2020 207c 2020  |   0.795    |  
+000051d0: 2030 2e39 3439 2020 207c 0a7c 2043 466c   0.949   |.| CFl
+000051e0: 6f77 2020 2020 2020 2020 207c 2057 6964  ow         | Wid
+000051f0: 6520 5265 734e 6574 2d35 3020 2020 2020  e ResNet-50     
+00005200: 7c20 2020 302e 3934 3420 2020 7c20 2020  |   0.944   |   
+00005210: 302e 3937 3220 2020 7c20 2020 302e 3933  0.972   |   0.93
+00005220: 3220 2020 7c20 2a2a 312e 3030 302a 2a20  2   | **1.000** 
+00005230: 7c20 2020 302e 3938 3820 2020 7c20 2020  |   0.988   |   
+00005240: 302e 3936 3720 2020 7c20 2a2a 312e 3030  0.967   | **1.00
+00005250: 302a 2a20 7c20 2020 302e 3833 3220 2020  0** |   0.832   
+00005260: 7c20 2020 302e 3933 3920 2020 7c20 2a2a  |   0.939   | **
+00005270: 312e 3030 302a 2a20 7c20 2020 302e 3937  1.000** |   0.97
+00005280: 3920 2020 7c20 2020 302e 3932 3420 2020  9   |   0.924   
+00005290: 7c20 2a2a 302e 3937 312a 2a20 7c20 2020  | **0.971** |   
+000052a0: 302e 3837 3020 2020 207c 2020 2030 2e38  0.870    |   0.8
+000052b0: 3138 2020 2020 7c20 2020 302e 3936 3720  18    |   0.967 
+000052c0: 2020 7c0a 7c20 5061 4469 4d20 2020 2020    |.| PaDiM     
+000052d0: 2020 2020 7c20 5769 6465 2052 6573 4e65      | Wide ResNe
+000052e0: 742d 3530 2020 2020 207c 2020 2030 2e39  t-50     |   0.9
+000052f0: 3531 2020 207c 202a 2a30 2e39 3839 2a2a  51   | **0.989**
+00005300: 207c 2020 2030 2e39 3330 2020 207c 202a   |   0.930   | *
+00005310: 2a31 2e30 3030 2a2a 207c 2020 2030 2e39  *1.000** |   0.9
+00005320: 3630 2020 207c 2020 2030 2e39 3833 2020  60   |   0.983  
+00005330: 207c 2020 2030 2e39 3932 2020 207c 2020   |   0.992   |  
+00005340: 2030 2e38 3536 2020 207c 202a 2a30 2e39   0.856   | **0.9
+00005350: 3832 2a2a 207c 2020 2030 2e39 3337 2020  82** |   0.937  
+00005360: 207c 2020 2030 2e39 3738 2020 207c 2020   |   0.978   |  
+00005370: 2030 2e39 3436 2020 207c 2020 2030 2e38   0.946   |   0.8
+00005380: 3935 2020 207c 2020 2030 2e39 3532 2020  95   |   0.952  
+00005390: 2020 7c20 2020 302e 3931 3420 2020 207c    |   0.914    |
+000053a0: 2020 2030 2e39 3437 2020 207c 0a7c 2050     0.947   |.| P
+000053b0: 6144 694d 2020 2020 2020 2020 207c 2052  aDiM         | R
+000053c0: 6573 4e65 742d 3138 2020 2020 2020 2020  esNet-18        
+000053d0: 2020 7c20 2020 302e 3931 3620 2020 7c20    |   0.916   | 
+000053e0: 2020 302e 3933 3020 2020 7c20 2020 302e    0.930   |   0.
+000053f0: 3839 3320 2020 7c20 2020 302e 3938 3420  893   |   0.984 
+00005400: 2020 7c20 2020 302e 3933 3420 2020 7c20    |   0.934   | 
+00005410: 2020 302e 3935 3220 2020 7c20 2020 302e    0.952   |   0.
+00005420: 3937 3620 2020 7c20 2020 302e 3835 3820  976   |   0.858 
+00005430: 2020 7c20 2020 302e 3936 3020 2020 7c20    |   0.960   | 
+00005440: 2020 302e 3833 3620 2020 7c20 2020 302e    0.836   |   0.
+00005450: 3937 3420 2020 7c20 2020 302e 3933 3220  974   |   0.932 
+00005460: 2020 7c20 2020 302e 3837 3920 2020 7c20    |   0.879   | 
+00005470: 2020 302e 3932 3320 2020 207c 2020 2030    0.923    |   0
+00005480: 2e37 3936 2020 2020 7c20 2020 302e 3931  .796    |   0.91
+00005490: 3520 2020 7c0a 7c20 4446 4d20 2020 2020  5   |.| DFM     
+000054a0: 2020 2020 2020 7c20 5769 6465 2052 6573        | Wide Res
+000054b0: 4e65 742d 3530 2020 2020 207c 2020 2030  Net-50     |   0
+000054c0: 2e39 3530 2020 207c 2020 2030 2e39 3135  .950   |   0.915
+000054d0: 2020 207c 2020 2030 2e38 3730 2020 207c     |   0.870   |
+000054e0: 2020 2030 2e39 3935 2020 207c 2020 2030     0.995   |   0
+000054f0: 2e39 3838 2020 207c 2020 2030 2e39 3630  .988   |   0.960
+00005500: 2020 207c 2020 2030 2e39 3932 2020 207c     |   0.992   |
+00005510: 2020 2030 2e39 3339 2020 207c 2020 2030     0.939   |   0
+00005520: 2e39 3635 2020 207c 2020 2030 2e39 3731  .965   |   0.971
+00005530: 2020 207c 2020 2030 2e39 3432 2020 207c     |   0.942   |
+00005540: 2020 2030 2e39 3536 2020 207c 2020 2030     0.956   |   0
+00005550: 2e39 3036 2020 207c 2020 2030 2e39 3636  .906   |   0.966
+00005560: 2020 2020 7c20 2020 302e 3931 3420 2020      |   0.914   
+00005570: 207c 2020 2030 2e39 3731 2020 207c 0a7c   |   0.971   |.|
+00005580: 2044 464d 2020 2020 2020 2020 2020 207c   DFM           |
+00005590: 2052 6573 4e65 742d 3138 2020 2020 2020   ResNet-18      
+000055a0: 2020 2020 7c20 2020 302e 3934 3320 2020      |   0.943   
+000055b0: 7c20 2020 302e 3839 3520 2020 7c20 2020  |   0.895   |   
+000055c0: 302e 3837 3120 2020 7c20 2020 302e 3937  0.871   |   0.97
+000055d0: 3820 2020 7c20 2020 302e 3935 3820 2020  8   |   0.958   
+000055e0: 7c20 2020 302e 3930 3020 2020 7c20 2020  |   0.900   |   
+000055f0: 312e 3030 3020 2020 7c20 2020 302e 3933  1.000   |   0.93
+00005600: 3520 2020 7c20 2020 302e 3936 3520 2020  5   |   0.965   
+00005610: 7c20 2020 302e 3936 3620 2020 7c20 2020  |   0.966   |   
+00005620: 302e 3934 3220 2020 7c20 2020 302e 3935  0.942   |   0.95
+00005630: 3620 2020 7c20 2020 302e 3931 3420 2020  6   |   0.914   
+00005640: 7c20 2020 302e 3936 3620 2020 207c 2020  |   0.966    |  
+00005650: 2030 2e38 3638 2020 2020 7c20 2020 302e   0.868    |   0.
+00005660: 3936 3420 2020 7c0a 7c20 5354 4650 4d20  964   |.| STFPM 
+00005670: 2020 2020 2020 2020 7c20 5769 6465 2052          | Wide R
+00005680: 6573 4e65 742d 3530 2020 2020 207c 2020  esNet-50     |  
+00005690: 2030 2e39 3236 2020 207c 2020 2030 2e39   0.926   |   0.9
+000056a0: 3733 2020 207c 2020 2030 2e39 3733 2020  73   |   0.973  
+000056b0: 207c 2020 2030 2e39 3734 2020 207c 2020   |   0.974   |  
+000056c0: 2030 2e39 3635 2020 207c 2020 2030 2e39   0.965   |   0.9
+000056d0: 3239 2020 207c 2020 2030 2e39 3736 2020  29   |   0.976  
+000056e0: 207c 2020 2030 2e38 3533 2020 207c 2020   |   0.853   |  
+000056f0: 2030 2e39 3230 2020 207c 2020 2030 2e39   0.920   |   0.9
+00005700: 3732 2020 207c 2020 2030 2e39 3734 2020  72   |   0.974  
+00005710: 207c 2020 2030 2e39 3232 2020 207c 2020   |   0.922   |  
+00005720: 2030 2e38 3834 2020 207c 2020 2030 2e38   0.884   |   0.8
+00005730: 3333 2020 2020 7c20 2020 302e 3831 3520  33    |   0.815 
+00005740: 2020 207c 2020 2030 2e39 3331 2020 207c     |   0.931   |
+00005750: 0a7c 2053 5446 504d 2020 2020 2020 2020  .| STFPM        
+00005760: 207c 2052 6573 4e65 742d 3138 2020 2020   | ResNet-18    
+00005770: 2020 2020 2020 7c20 2020 302e 3933 3220        |   0.932 
+00005780: 2020 7c20 2020 302e 3936 3120 2020 7c20    |   0.961   | 
+00005790: 2a2a 302e 3938 322a 2a20 7c20 2020 302e  **0.982** |   0.
+000057a0: 3938 3920 2020 7c20 2020 302e 3933 3020  989   |   0.930 
+000057b0: 2020 7c20 2020 302e 3935 3120 2020 7c20    |   0.951   | 
+000057c0: 2020 302e 3938 3420 2020 7c20 2020 302e    0.984   |   0.
+000057d0: 3831 3920 2020 7c20 2020 302e 3931 3820  819   |   0.918 
+000057e0: 2020 7c20 2020 302e 3939 3320 2020 7c20    |   0.993   | 
+000057f0: 2020 302e 3937 3320 2020 7c20 2020 302e    0.973   |   0.
+00005800: 3931 3820 2020 7c20 2020 302e 3838 3720  918   |   0.887 
+00005810: 2020 7c20 2a2a 302e 3938 342a 2a20 207c    | **0.984**  |
+00005820: 2020 2030 2e37 3930 2020 2020 7c20 2020     0.790    |   
+00005830: 302e 3930 3820 2020 7c0a 7c20 4446 4b44  0.908   |.| DFKD
+00005840: 4520 2020 2020 2020 2020 7c20 5769 6465  E         | Wide
+00005850: 2052 6573 4e65 742d 3530 2020 2020 207c   ResNet-50     |
+00005860: 2020 2030 2e38 3735 2020 207c 2020 2030     0.875   |   0
+00005870: 2e39 3037 2020 207c 2020 2030 2e38 3434  .907   |   0.844
+00005880: 2020 207c 2020 2030 2e39 3035 2020 207c     |   0.905   |
+00005890: 2020 2030 2e39 3435 2020 207c 2020 2030     0.945   |   0
+000058a0: 2e39 3134 2020 207c 2020 2030 2e39 3436  .914   |   0.946
+000058b0: 2020 207c 2020 2030 2e37 3930 2020 207c     |   0.790   |
+000058c0: 2020 2030 2e39 3134 2020 207c 2020 2030     0.914   |   0
+000058d0: 2e38 3137 2020 207c 2020 2030 2e38 3934  .817   |   0.894
+000058e0: 2020 207c 2020 2030 2e39 3232 2020 207c     |   0.922   |
+000058f0: 2020 2030 2e38 3535 2020 207c 2020 2030     0.855   |   0
+00005900: 2e38 3435 2020 2020 7c20 2020 302e 3732  .845    |   0.72
+00005910: 3220 2020 207c 2020 2030 2e39 3130 2020  2    |   0.910  
+00005920: 207c 0a7c 2044 464b 4445 2020 2020 2020   |.| DFKDE      
+00005930: 2020 207c 2052 6573 4e65 742d 3138 2020     | ResNet-18  
+00005940: 2020 2020 2020 2020 7c20 2020 302e 3837          |   0.87
+00005950: 3220 2020 7c20 2020 302e 3836 3420 2020  2   |   0.864   
+00005960: 7c20 2020 302e 3834 3420 2020 7c20 2020  |   0.844   |   
+00005970: 302e 3835 3420 2020 7c20 2020 302e 3936  0.854   |   0.96
+00005980: 3020 2020 7c20 2020 302e 3839 3820 2020  0   |   0.898   
+00005990: 7c20 2020 302e 3934 3220 2020 7c20 2020  |   0.942   |   
+000059a0: 302e 3739 3320 2020 7c20 2020 302e 3930  0.793   |   0.90
+000059b0: 3820 2020 7c20 2020 302e 3832 3720 2020  8   |   0.827   
+000059c0: 7c20 2020 302e 3839 3420 2020 7c20 2020  |   0.894   |   
+000059d0: 302e 3931 3620 2020 7c20 2020 302e 3835  0.916   |   0.85
+000059e0: 3920 2020 7c20 2020 302e 3835 3320 2020  9   |   0.853   
+000059f0: 207c 2020 2030 2e37 3536 2020 2020 7c20   |   0.756    | 
+00005a00: 2020 302e 3931 3620 2020 7c0a 7c20 4741    0.916   |.| GA
+00005a10: 4e6f 6d61 6c79 2020 2020 2020 7c20 2020  Nomaly      |   
+00005a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a30: 207c 2020 2030 2e38 3334 2020 207c 2020   |   0.834   |  
+00005a40: 2030 2e38 3634 2020 207c 2020 2030 2e38   0.864   |   0.8
+00005a50: 3434 2020 207c 2020 2030 2e38 3532 2020  44   |   0.852  
+00005a60: 207c 2020 2030 2e38 3336 2020 207c 2020   |   0.836   |  
+00005a70: 2030 2e38 3633 2020 207c 2020 2030 2e38   0.863   |   0.8
+00005a80: 3633 2020 207c 2020 2030 2e37 3630 2020  63   |   0.760  
+00005a90: 207c 2020 2030 2e39 3035 2020 207c 2020   |   0.905   |  
+00005aa0: 2030 2e37 3737 2020 207c 2020 2030 2e38   0.777   |   0.8
+00005ab0: 3934 2020 207c 2020 2030 2e39 3136 2020  94   |   0.916  
+00005ac0: 207c 2020 2030 2e38 3533 2020 207c 2020   |   0.853   |  
+00005ad0: 2030 2e38 3333 2020 2020 7c20 2020 302e   0.833    |   0.
+00005ae0: 3537 3120 2020 207c 2020 2030 2e38 3831  571    |   0.881
+00005af0: 2020 207c 0a0a 2320 5265 6665 7265 6e63     |..# Referenc
+00005b00: 650a 0a49 6620 796f 7520 7573 6520 7468  e..If you use th
+00005b10: 6973 206c 6962 7261 7279 2061 6e64 206c  is library and l
+00005b20: 6f76 6520 6974 2c20 7573 6520 7468 6973  ove it, use this
+00005b30: 2074 6f20 6369 7465 2069 7420 f09f a497   to cite it ....
+00005b40: 0a0a 6060 6074 6578 0a40 6d69 7363 7b61  ..```tex.@misc{a
+00005b50: 6e6f 6d61 6c69 622c 0a20 2020 2020 2074  nomalib,.      t
+00005b60: 6974 6c65 3d7b 416e 6f6d 616c 6962 3a20  itle={Anomalib: 
+00005b70: 4120 4465 6570 204c 6561 726e 696e 6720  A Deep Learning 
+00005b80: 4c69 6272 6172 7920 666f 7220 416e 6f6d  Library for Anom
+00005b90: 616c 7920 4465 7465 6374 696f 6e7d 2c0a  aly Detection},.
+00005ba0: 2020 2020 2020 6175 7468 6f72 3d7b 5361        author={Sa
+00005bb0: 6d65 7420 416b 6361 7920 616e 640a 2020  met Akcay and.  
+00005bc0: 2020 2020 2020 2020 2020 2020 4469 636b              Dick
+00005bd0: 2041 6d65 6c6e 2061 6e64 0a20 2020 2020   Ameln and.     
+00005be0: 2020 2020 2020 2020 2041 7368 7769 6e20           Ashwin 
+00005bf0: 5661 6964 7961 2061 6e64 0a20 2020 2020  Vaidya and.     
+00005c00: 2020 2020 2020 2020 2042 6172 6174 6820           Barath 
+00005c10: 4c61 6b73 686d 616e 616e 2061 6e64 0a20  Lakshmanan and. 
+00005c20: 2020 2020 2020 2020 2020 2020 204e 696c               Nil
+00005c30: 6573 6820 4168 756a 6120 616e 640a 2020  esh Ahuja and.  
+00005c40: 2020 2020 2020 2020 2020 2020 5574 6b75              Utku
+00005c50: 2047 656e 637d 2c0a 2020 2020 2020 7965   Genc},.      ye
+00005c60: 6172 3d7b 3230 3232 7d2c 0a20 2020 2020  ar={2022},.     
+00005c70: 2065 7072 696e 743d 7b32 3230 322e 3038   eprint={2202.08
+00005c80: 3334 317d 2c0a 2020 2020 2020 6172 6368  341},.      arch
+00005c90: 6976 6550 7265 6669 783d 7b61 7258 6976  ivePrefix={arXiv
+00005ca0: 7d2c 0a20 2020 2020 2070 7269 6d61 7279  },.      primary
+00005cb0: 436c 6173 733d 7b63 732e 4356 7d0a 7d0a  Class={cs.CV}.}.
+00005cc0: 6060 600a 0a23 2043 6f6e 7472 6962 7574  ```..# Contribut
+00005cd0: 696e 670a 0a46 6f72 2074 686f 7365 2077  ing..For those w
+00005ce0: 686f 2077 6f75 6c64 206c 696b 6520 746f  ho would like to
+00005cf0: 2063 6f6e 7472 6962 7574 6520 746f 2074   contribute to t
+00005d00: 6865 206c 6962 7261 7279 2c20 7365 6520  he library, see 
+00005d10: 5b43 4f4e 5452 4942 5554 494e 472e 6d64  [CONTRIBUTING.md
+00005d20: 5d28 434f 4e54 5249 4255 5449 4e47 2e6d  ](CONTRIBUTING.m
+00005d30: 6429 2066 6f72 2064 6574 6169 6c73 2e0a  d) for details..
+00005d40: 0a54 6861 6e6b 2079 6f75 2074 6f20 616c  .Thank you to al
+00005d50: 6c20 6f66 2074 6865 2070 656f 706c 6520  l of the people 
+00005d60: 7768 6f20 6861 7665 2061 6c72 6561 6479  who have already
+00005d70: 206d 6164 6520 6120 636f 6e74 7269 6275   made a contribu
+00005d80: 7469 6f6e 202d 2077 6520 6170 7072 6563  tion - we apprec
+00005d90: 6961 7465 2079 6f75 7220 7375 7070 6f72  iate your suppor
+00005da0: 7421 0a0a 3c61 2068 7265 663d 2268 7474  t!..<a href="htt
+00005db0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00005dc0: 6f70 656e 7669 6e6f 746f 6f6c 6b69 742f  openvinotoolkit/
+00005dd0: 616e 6f6d 616c 6962 2f67 7261 7068 732f  anomalib/graphs/
+00005de0: 636f 6e74 7269 6275 746f 7273 223e 0a20  contributors">. 
+00005df0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00005e00: 3a2f 2f63 6f6e 7472 6962 2e72 6f63 6b73  ://contrib.rocks
+00005e10: 2f69 6d61 6765 3f72 6570 6f3d 6f70 656e  /image?repo=open
+00005e20: 7669 6e6f 746f 6f6c 6b69 742f 616e 6f6d  vinotoolkit/anom
+00005e30: 616c 6962 2220 2f3e 0a3c 2f61 3e0a       alib" />.</a>.
```

### Comparing `anomalib-0.4.0rc2/anomalib/config/config.py` & `anomalib-0.5.0/src/anomalib/config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
     if model_name is None is config_path:
         raise ValueError(
             "Both model_name and model config path cannot be None! "
             "Please provide a model name or path to a config file!"
         )
 
     if config_path is None:
-        config_path = Path(f"anomalib/models/{model_name}/{config_filename}.{config_file_extension}")
+        config_path = Path(f"src/anomalib/models/{model_name}/{config_filename}.{config_file_extension}")
 
     config = OmegaConf.load(config_path)
 
     # keep track of the original config file because it will be modified
     config_original: DictConfig = config.copy()
 
     # if the seed value is 0, notify a user that the behavior of the seed value zero has been changed.
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/__init__.py` & `anomalib-0.5.0/src/anomalib/data/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,31 +2,48 @@
 
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import logging
+from enum import Enum
 
 from omegaconf import DictConfig, ListConfig
 
 from .avenue import Avenue
 from .base import AnomalibDataModule, AnomalibDataset
 from .btech import BTech
 from .folder import Folder
+from .folder_3d import Folder3D
 from .inference import InferenceDataset
 from .mvtec import MVTec
+from .mvtec_3d import MVTec3D
 from .shanghaitech import ShanghaiTech
 from .task_type import TaskType
 from .ucsd_ped import UCSDped
 from .visa import Visa
 
 logger = logging.getLogger(__name__)
 
 
+class DataFormat(str, Enum):
+    """Supported Dataset Types"""
+
+    MVTEC = "mvtec"
+    MVTEC_3D = "mvtec_3d"
+    BTECH = "btech"
+    FOLDER = "folder"
+    FOLDER_3D = "folder_3d"
+    UCSDPED = "ucsdped"
+    AVENUE = "avenue"
+    VISA = "visa"
+    SHANGHAITECH = "shanghaitech"
+
+
 def get_datamodule(config: DictConfig | ListConfig) -> AnomalibDataModule:
     """Get Anomaly Datamodule.
 
     Args:
         config (DictConfig | ListConfig): Configuration of the anomaly model.
 
     Returns:
@@ -37,15 +54,15 @@
     datamodule: AnomalibDataModule
 
     # convert center crop to tuple
     center_crop = config.dataset.get("center_crop")
     if center_crop is not None:
         center_crop = (center_crop[0], center_crop[1])
 
-    if config.dataset.format.lower() == "mvtec":
+    if config.dataset.format.lower() == DataFormat.MVTEC:
         datamodule = MVTec(
             root=config.dataset.path,
             category=config.dataset.category,
             image_size=(config.dataset.image_size[0], config.dataset.image_size[1]),
             center_crop=center_crop,
             normalization=config.dataset.normalization,
             train_batch_size=config.dataset.train_batch_size,
@@ -55,15 +72,33 @@
             transform_config_train=config.dataset.transform_config.train,
             transform_config_eval=config.dataset.transform_config.eval,
             test_split_mode=config.dataset.test_split_mode,
             test_split_ratio=config.dataset.test_split_ratio,
             val_split_mode=config.dataset.val_split_mode,
             val_split_ratio=config.dataset.val_split_ratio,
         )
-    elif config.dataset.format.lower() == "btech":
+    elif config.dataset.format.lower() == DataFormat.MVTEC_3D:
+        datamodule = MVTec3D(
+            root=config.dataset.path,
+            category=config.dataset.category,
+            image_size=(config.dataset.image_size[0], config.dataset.image_size[1]),
+            center_crop=center_crop,
+            normalization=config.dataset.normalization,
+            train_batch_size=config.dataset.train_batch_size,
+            eval_batch_size=config.dataset.eval_batch_size,
+            num_workers=config.dataset.num_workers,
+            task=config.dataset.task,
+            transform_config_train=config.dataset.transform_config.train,
+            transform_config_eval=config.dataset.transform_config.eval,
+            test_split_mode=config.dataset.test_split_mode,
+            test_split_ratio=config.dataset.test_split_ratio,
+            val_split_mode=config.dataset.val_split_mode,
+            val_split_ratio=config.dataset.val_split_ratio,
+        )
+    elif config.dataset.format.lower() == DataFormat.BTECH:
         datamodule = BTech(
             root=config.dataset.path,
             category=config.dataset.category,
             image_size=(config.dataset.image_size[0], config.dataset.image_size[1]),
             center_crop=center_crop,
             normalization=config.dataset.normalization,
             train_batch_size=config.dataset.train_batch_size,
@@ -73,15 +108,15 @@
             transform_config_train=config.dataset.transform_config.train,
             transform_config_eval=config.dataset.transform_config.eval,
             test_split_mode=config.dataset.test_split_mode,
             test_split_ratio=config.dataset.test_split_ratio,
             val_split_mode=config.dataset.val_split_mode,
             val_split_ratio=config.dataset.val_split_ratio,
         )
-    elif config.dataset.format.lower() == "folder":
+    elif config.dataset.format.lower() == DataFormat.FOLDER:
         datamodule = Folder(
             root=config.dataset.root,
             normal_dir=config.dataset.normal_dir,
             abnormal_dir=config.dataset.abnormal_dir,
             task=config.dataset.task,
             normal_test_dir=config.dataset.normal_test_dir,
             mask_dir=config.dataset.mask_dir,
@@ -95,51 +130,78 @@
             transform_config_train=config.dataset.transform_config.train,
             transform_config_eval=config.dataset.transform_config.eval,
             test_split_mode=config.dataset.test_split_mode,
             test_split_ratio=config.dataset.test_split_ratio,
             val_split_mode=config.dataset.val_split_mode,
             val_split_ratio=config.dataset.val_split_ratio,
         )
-    elif config.dataset.format.lower() == "ucsdped":
+    elif config.dataset.format.lower() == DataFormat.FOLDER_3D:
+        datamodule = Folder3D(
+            root=config.dataset.root,
+            normal_dir=config.dataset.normal_dir,
+            normal_depth_dir=config.dataset.normal_depth_dir,
+            abnormal_dir=config.dataset.abnormal_dir,
+            abnormal_depth_dir=config.dataset.abnormal_depth_dir,
+            task=config.dataset.task,
+            normal_test_dir=config.dataset.normal_test_dir,
+            normal_test_depth_dir=config.dataset.normal_test_depth_dir,
+            mask_dir=config.dataset.mask_dir,
+            extensions=config.dataset.extensions,
+            image_size=(config.dataset.image_size[0], config.dataset.image_size[1]),
+            center_crop=center_crop,
+            normalization=config.dataset.normalization,
+            train_batch_size=config.dataset.train_batch_size,
+            eval_batch_size=config.dataset.eval_batch_size,
+            num_workers=config.dataset.num_workers,
+            transform_config_train=config.dataset.transform_config.train,
+            transform_config_eval=config.dataset.transform_config.eval,
+            test_split_mode=config.dataset.test_split_mode,
+            test_split_ratio=config.dataset.test_split_ratio,
+            val_split_mode=config.dataset.val_split_mode,
+            val_split_ratio=config.dataset.val_split_ratio,
+        )
+    elif config.dataset.format.lower() == DataFormat.UCSDPED:
         datamodule = UCSDped(
             root=config.dataset.path,
             category=config.dataset.category,
             task=config.dataset.task,
             clip_length_in_frames=config.dataset.clip_length_in_frames,
             frames_between_clips=config.dataset.frames_between_clips,
+            target_frame=config.dataset.target_frame,
             image_size=(config.dataset.image_size[0], config.dataset.image_size[1]),
             center_crop=center_crop,
             normalization=config.dataset.normalization,
             transform_config_train=config.dataset.transform_config.train,
             transform_config_eval=config.dataset.transform_config.eval,
             train_batch_size=config.dataset.train_batch_size,
             eval_batch_size=config.dataset.eval_batch_size,
             num_workers=config.dataset.num_workers,
             val_split_mode=config.dataset.val_split_mode,
             val_split_ratio=config.dataset.val_split_ratio,
         )
-    elif config.dataset.format.lower() == "avenue":
+    elif config.dataset.format.lower() == DataFormat.AVENUE:
         datamodule = Avenue(
             root=config.dataset.path,
             gt_dir=config.dataset.gt_dir,
             task=config.dataset.task,
             clip_length_in_frames=config.dataset.clip_length_in_frames,
             frames_between_clips=config.dataset.frames_between_clips,
+            target_frame=config.dataset.target_frame,
             image_size=(config.dataset.image_size[0], config.dataset.image_size[1]),
             center_crop=center_crop,
             normalization=config.dataset.normalization,
             transform_config_train=config.dataset.transform_config.train,
             transform_config_eval=config.dataset.transform_config.eval,
             train_batch_size=config.dataset.train_batch_size,
             eval_batch_size=config.dataset.eval_batch_size,
             num_workers=config.dataset.num_workers,
             val_split_mode=config.dataset.val_split_mode,
             val_split_ratio=config.dataset.val_split_ratio,
         )
-    elif config.dataset.format.lower() == "visa":
+    elif config.dataset.format.lower() == DataFormat.VISA:
         datamodule = Visa(
             root=config.dataset.path,
             category=config.dataset.category,
             image_size=(config.dataset.image_size[0], config.dataset.image_size[1]),
             center_crop=center_crop,
             normalization=config.dataset.normalization,
             train_batch_size=config.dataset.train_batch_size,
@@ -149,21 +211,22 @@
             transform_config_train=config.dataset.transform_config.train,
             transform_config_eval=config.dataset.transform_config.eval,
             test_split_mode=config.dataset.test_split_mode,
             test_split_ratio=config.dataset.test_split_ratio,
             val_split_mode=config.dataset.val_split_mode,
             val_split_ratio=config.dataset.val_split_ratio,
         )
-    elif config.dataset.format.lower() == "shanghaitech":
+    elif config.dataset.format.lower() == DataFormat.SHANGHAITECH:
         datamodule = ShanghaiTech(
             root=config.dataset.path,
             scene=config.dataset.scene,
             task=config.dataset.task,
             clip_length_in_frames=config.dataset.clip_length_in_frames,
             frames_between_clips=config.dataset.frames_between_clips,
+            target_frame=config.dataset.target_frame,
             image_size=(config.dataset.image_size[0], config.dataset.image_size[1]),
             center_crop=center_crop,
             normalization=config.dataset.normalization,
             transform_config_train=config.dataset.transform_config.train,
             transform_config_eval=config.dataset.transform_config.eval,
             train_batch_size=config.dataset.train_batch_size,
             eval_batch_size=config.dataset.eval_batch_size,
@@ -183,14 +246,16 @@
 
 __all__ = [
     "AnomalibDataset",
     "AnomalibDataModule",
     "get_datamodule",
     "BTech",
     "Folder",
+    "Folder3D",
     "InferenceDataset",
     "MVTec",
+    "MVTec3D",
     "Avenue",
     "UCSDped",
     "TaskType",
     "ShanghaiTech",
 ]
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/avenue.py` & `anomalib-0.5.0/src/anomalib/data/avenue.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import albumentations as A
 import cv2
 import numpy as np
 import scipy.io
 from pandas import DataFrame
 
 from anomalib.data.base import AnomalibVideoDataModule, AnomalibVideoDataset
+from anomalib.data.base.video import VideoTargetFrame
 from anomalib.data.task_type import TaskType
 from anomalib.data.utils import (
     DownloadInfo,
     InputNormalizationMethod,
     Split,
     ValSplitMode,
     download_and_extract,
@@ -136,27 +137,29 @@
         task (TaskType): Task type, 'classification', 'detection' or 'segmentation'
         root (Path | str): Path to the root of the dataset
         gt_dir (Path | str): Path to the ground truth files
         transform (A.Compose): Albumentations Compose object describing the transforms that are applied to the inputs.
         split (Split): Split of the dataset, usually Split.TRAIN or Split.TEST
         clip_length_in_frames (int, optional): Number of video frames in each clip.
         frames_between_clips (int, optional): Number of frames between each consecutive video clip.
+        target_frame (VideoTargetFrame): Specifies the target frame in the video clip, used for ground truth retrieval
     """
 
     def __init__(
         self,
         task: TaskType,
         root: Path | str,
         gt_dir: Path | str,
         transform: A.Compose,
         split: Split,
         clip_length_in_frames: int = 1,
         frames_between_clips: int = 1,
+        target_frame: VideoTargetFrame = VideoTargetFrame.LAST,
     ) -> None:
-        super().__init__(task, transform, clip_length_in_frames, frames_between_clips)
+        super().__init__(task, transform, clip_length_in_frames, frames_between_clips, target_frame)
 
         self.root = root if isinstance(root, Path) else Path(root)
         self.gt_dir = gt_dir if isinstance(gt_dir, Path) else Path(gt_dir)
         self.split = split
         self.indexer_cls: Callable = AvenueClipsIndexer
 
     def _setup(self) -> None:
@@ -168,14 +171,15 @@
     """Avenue DataModule class.
 
     Args:
         root (Path | str): Path to the root of the dataset
         gt_dir (Path | str): Path to the ground truth files
         clip_length_in_frames (int, optional): Number of video frames in each clip.
         frames_between_clips (int, optional): Number of frames between each consecutive video clip.
+        target_frame (VideoTargetFrame): Specifies the target frame in the video clip, used for ground truth retrieval
         task TaskType): Task type, 'classification', 'detection' or 'segmentation'
         image_size (int | tuple[int, int] | None, optional): Size of the input image.
             Defaults to None.
         center_crop (int | tuple[int, int] | None, optional): When provided, the images will be center-cropped
             to the provided dimensions.
         normalize (bool): When True, the images will be normalized to the ImageNet statistics.
         train_batch_size (int, optional): Training batch size. Defaults to 32.
@@ -194,14 +198,15 @@
 
     def __init__(
         self,
         root: Path | str,
         gt_dir: Path | str,
         clip_length_in_frames: int = 1,
         frames_between_clips: int = 1,
+        target_frame: VideoTargetFrame = VideoTargetFrame.LAST,
         task: TaskType = TaskType.SEGMENTATION,
         image_size: int | tuple[int, int] | None = None,
         center_crop: int | tuple[int, int] | None = None,
         normalization: str | InputNormalizationMethod = InputNormalizationMethod.IMAGENET,
         train_batch_size: int = 32,
         eval_batch_size: int = 32,
         num_workers: int = 8,
@@ -237,24 +242,26 @@
         )
 
         self.train_data = AvenueDataset(
             task=task,
             transform=transform_train,
             clip_length_in_frames=clip_length_in_frames,
             frames_between_clips=frames_between_clips,
+            target_frame=target_frame,
             root=root,
             gt_dir=gt_dir,
             split=Split.TRAIN,
         )
 
         self.test_data = AvenueDataset(
             task=task,
             transform=transform_eval,
             clip_length_in_frames=clip_length_in_frames,
             frames_between_clips=frames_between_clips,
+            target_frame=target_frame,
             root=root,
             gt_dir=gt_dir,
             split=Split.TEST,
         )
 
     def prepare_data(self) -> None:
         """Download the dataset and ground truth if not available, and convert mask files to a more usable format."""
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/base/datamodule.py` & `anomalib-0.5.0/src/anomalib/data/base/datamodule.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 from abc import ABC
 from typing import Any
 
 from pandas import DataFrame
 from pytorch_lightning import LightningDataModule
 from pytorch_lightning.utilities.types import EVAL_DATALOADERS, TRAIN_DATALOADERS
-from torch.utils.data import DataLoader, default_collate
+from torch.utils.data.dataloader import DataLoader, default_collate
 
 from anomalib.data.base.dataset import AnomalibDataset
 from anomalib.data.synthetic import SyntheticAnomalyDataset
 from anomalib.data.utils import (
     TestSplitMode,
     ValSplitMode,
     random_split,
@@ -126,15 +126,15 @@
         if self.test_data.has_normal:
             # split the test data into normal and anomalous so these can be processed separately
             normal_test_data, self.test_data = split_by_label(self.test_data)
         elif self.test_split_mode != TestSplitMode.NONE:
             # when the user did not provide any normal images for testing, we sample some from the training set,
             # except when the user explicitly requested no test splitting.
             logger.info(
-                "No normal test images found. Sampling from training set using a split ratio of %d",
+                "No normal test images found. Sampling from training set using a split ratio of %0.2f",
                 self.test_split_ratio,
             )
             if self.test_split_ratio is not None:
                 self.train_data, normal_test_data = random_split(self.train_data, self.test_split_ratio, seed=self.seed)
 
         if self.test_split_mode == TestSplitMode.FROM_DIR:
             self.test_data += normal_test_data
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/base/dataset.py` & `anomalib-0.5.0/src/anomalib/data/base/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         transform (A.Compose): Albumentations Compose object describing the transforms that are applied to the inputs.
     """
 
     def __init__(self, task: TaskType, transform: A.Compose) -> None:
         super().__init__()
         self.task = task
         self.transform = transform
-        self._samples: DataFrame = None
+        self._samples: DataFrame
 
     def __len__(self) -> int:
         """Get length of the dataset."""
         return len(self.samples)
 
     def subsample(self, indices: Sequence[int], inplace: bool = False) -> AnomalibDataset:
         """Subsamples the dataset at the provided indices.
@@ -62,15 +62,15 @@
         dataset = self if inplace else copy.deepcopy(self)
         dataset.samples = self.samples.iloc[indices].reset_index(drop=True)
         return dataset
 
     @property
     def is_setup(self) -> bool:
         """Checks if setup() been called."""
-        return isinstance(self._samples, DataFrame)
+        return hasattr(self, "_samples")
 
     @property
     def samples(self) -> DataFrame:
         """Get the samples dataframe."""
         if not self.is_setup:
             raise RuntimeError("Dataset is not setup yet. Call setup() first.")
         return self._samples
@@ -122,14 +122,15 @@
 
         if self.task == TaskType.CLASSIFICATION:
             transformed = self.transform(image=image)
             item["image"] = transformed["image"]
         elif self.task in (TaskType.DETECTION, TaskType.SEGMENTATION):
             # Only Anomalous (1) images have masks in anomaly datasets
             # Therefore, create empty mask for Normal (0) images.
+
             if label_index == 0:
                 mask = np.zeros(shape=image.shape[:2])
             else:
                 mask = cv2.imread(mask_path, flags=0) / 255.0
 
             transformed = self.transform(image=image, mask=mask)
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/base/video.py` & `anomalib-0.5.0/src/anomalib/data/base/video.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,69 @@
 """Base Video Dataset."""
 
 from __future__ import annotations
 
 from abc import ABC
+from enum import Enum
 from typing import Callable
 
 import albumentations as A
 import torch
 from pandas import DataFrame
 from torch import Tensor
 
 from anomalib.data.base.datamodule import AnomalibDataModule
 from anomalib.data.base.dataset import AnomalibDataset
 from anomalib.data.task_type import TaskType
 from anomalib.data.utils import ValSplitMode, masks_to_boxes
 from anomalib.data.utils.video import ClipsIndexer
 
 
+class VideoTargetFrame(str, Enum):
+    """Target frame for a video-clip.
+
+    Used in multi-frame models to determine which frame's ground truth information will be used.
+    """
+
+    FIRST = "first"
+    LAST = "last"
+    MID = "mid"
+    ALL = "all"
+
+
 class AnomalibVideoDataset(AnomalibDataset, ABC):
     """Base video anomalib dataset class.
 
     Args:
         task (str): Task type, either 'classification' or 'segmentation'
         transform (A.Compose): Albumentations Compose object describing the transforms that are applied to the inputs.
         clip_length_in_frames (int): Number of video frames in each clip.
         frames_between_clips (int): Number of frames between each consecutive video clip.
+        target_frame (VideoTargetFrame): Specifies the target frame in the video clip, used for ground truth retrieval
     """
 
     def __init__(
-        self, task: TaskType, transform: A.Compose, clip_length_in_frames: int, frames_between_clips: int
+        self,
+        task: TaskType,
+        transform: A.Compose,
+        clip_length_in_frames: int,
+        frames_between_clips: int,
+        target_frame=VideoTargetFrame.LAST,
     ) -> None:
         super().__init__(task, transform)
 
         self.clip_length_in_frames = clip_length_in_frames
         self.frames_between_clips = frames_between_clips
         self.transform = transform
 
         self.indexer: ClipsIndexer | None = None
         self.indexer_cls: Callable | None = None
 
+        self.target_frame = target_frame
+
     def __len__(self) -> int:
         """Get length of the dataset."""
         assert isinstance(self.indexer, ClipsIndexer)
         return self.indexer.num_clips()
 
     @property
     def samples(self) -> DataFrame:
@@ -64,14 +85,36 @@
         self.indexer = self.indexer_cls(  # pylint: disable=not-callable
             video_paths=list(self.samples.image_path),
             mask_paths=list(self.samples.mask_path),
             clip_length_in_frames=self.clip_length_in_frames,
             frames_between_clips=self.frames_between_clips,
         )
 
+    def _select_targets(self, item):
+        if self.target_frame == VideoTargetFrame.FIRST:
+            idx = 0
+        elif self.target_frame == VideoTargetFrame.LAST:
+            idx = -1
+        elif self.target_frame == VideoTargetFrame.MID:
+            idx = int(self.clip_length_in_frames / 2)
+        else:
+            raise ValueError(f"Unknown video target frame: {self.target_frame}")
+
+        if item.get("mask") is not None:
+            item["mask"] = item["mask"][idx, ...]
+        if item.get("boxes") is not None:
+            item["boxes"] = item["boxes"][idx]
+        if item.get("label") is not None:
+            item["label"] = item["label"][idx]
+        if item.get("original_image") is not None:
+            item["original_image"] = item["original_image"][idx]
+        if item.get("frames") is not None:
+            item["frames"] = item["frames"][idx]
+        return item
+
     def __getitem__(self, index: int) -> dict[str, str | Tensor]:
         """Return mask, clip and file system information."""
         assert isinstance(self.indexer, ClipsIndexer)
 
         item = self.indexer.get_item(index)
         # include the untransformed image for visualization
         item["original_image"] = item["image"].to(torch.uint8)
@@ -89,14 +132,18 @@
                 item["boxes"], _ = masks_to_boxes(item["mask"])
                 item["boxes"] = item["boxes"][0] if len(item["boxes"]) == 1 else item["boxes"]
         else:
             item["image"] = torch.stack(
                 [self.transform(image=frame.numpy())["image"] for frame in item["image"]]
             ).squeeze(0)
 
+        # include only target frame in gt
+        if self.clip_length_in_frames > 1 and self.target_frame != VideoTargetFrame.ALL:
+            item = self._select_targets(item)
+
         if item["mask"] is None:
             item.pop("mask")
 
         return item
 
 
 class AnomalibVideoDataModule(AnomalibDataModule):
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/btech.py` & `anomalib-0.5.0/src/anomalib/data/btech.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from tqdm import tqdm
 
 from anomalib.data.base import AnomalibDataModule, AnomalibDataset
 from anomalib.data.task_type import TaskType
 from anomalib.data.utils import (
     DownloadInfo,
     InputNormalizationMethod,
+    LabelName,
     Split,
     TestSplitMode,
     ValSplitMode,
     download_and_extract,
     get_transforms,
 )
 
@@ -100,16 +101,16 @@
     # Modify image_path column by converting to absolute path
     samples["image_path"] = samples.path + "/" + samples.split + "/" + samples.label + "/" + samples.image_path
 
     # Good images don't have mask
     samples.loc[(samples.split == "test") & (samples.label == "ok"), "mask_path"] = ""
 
     # Create label index for normal (0) and anomalous (1) images.
-    samples.loc[(samples.label == "ok"), "label_index"] = 0
-    samples.loc[(samples.label != "ok"), "label_index"] = 1
+    samples.loc[(samples.label == "ok"), "label_index"] = LabelName.NORMAL
+    samples.loc[(samples.label != "ok"), "label_index"] = LabelName.ABNORMAL
     samples.label_index = samples.label_index.astype(int)
 
     # Get the data frame for the split.
     if split:
         samples = samples[samples.split == split]
         samples = samples.reset_index(drop=True)
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/folder.py` & `anomalib-0.5.0/src/anomalib/data/folder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,210 +1,155 @@
 """Custom Folder Dataset.
-
 This script creates a custom dataset from a folder.
 """
 
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from pathlib import Path
 
 import albumentations as A
 from pandas import DataFrame
-from torchvision.datasets.folder import IMG_EXTENSIONS
 
 from anomalib.data.base import AnomalibDataModule, AnomalibDataset
 from anomalib.data.task_type import TaskType
 from anomalib.data.utils import (
+    DirType,
     InputNormalizationMethod,
+    LabelName,
     Split,
     TestSplitMode,
     ValSplitMode,
     get_transforms,
 )
-
-
-def _check_and_convert_path(path: str | Path) -> Path:
-    """Check an input path, and convert to Pathlib object.
-
-    Args:
-        path (str | Path): Input path.
-
-    Returns:
-        Path: Output path converted to pathlib object.
-    """
-    if not isinstance(path, Path):
-        path = Path(path)
-    return path
-
-
-def _prepare_files_labels(
-    path: str | Path, path_type: str, extensions: tuple[str, ...] | None = None
-) -> tuple[list, list]:
-    """Return a list of filenames and list corresponding labels.
-
-    Args:
-        path (str | Path): Path to the directory containing images.
-        path_type (str): Type of images in the provided path ("normal", "abnormal", "normal_test")
-        extensions (tuple[str, ...] | None, optional): Type of the image extensions to read from the
-            directory.
-
-    Returns:
-        List, List: Filenames of the images provided in the paths, labels of the images provided in the paths
-    """
-    path = _check_and_convert_path(path)
-    if extensions is None:
-        extensions = IMG_EXTENSIONS
-
-    if isinstance(extensions, str):
-        extensions = (extensions,)
-
-    filenames = [f for f in path.glob(r"**/*") if f.suffix in extensions and not f.is_dir()]
-    if not filenames:
-        raise RuntimeError(f"Found 0 {path_type} images in {path}")
-
-    labels = [path_type] * len(filenames)
-
-    return filenames, labels
-
-
-def _resolve_path(folder: str | Path, root: str | Path | None = None) -> Path:
-    """Combines root and folder and returns the absolute path.
-
-    This allows users to pass either a root directory and relative paths, or absolute paths to each of the
-    image sources. This function makes sure that the samples dataframe always contains absolute paths.
-
-    Args:
-        folder (str | Path | None): Folder location containing image or mask data.
-        root (str | Path | None): Root directory for the dataset.
-    """
-    folder = Path(folder)
-    if folder.is_absolute():
-        # path is absolute; return unmodified
-        path = folder
-    # path is relative.
-    elif root is None:
-        # no root provided; return absolute path
-        path = folder.resolve()
-    else:
-        # root provided; prepend root and return absolute path
-        path = (Path(root) / folder).resolve()
-    return path
+from anomalib.data.utils.path import _prepare_files_labels, _resolve_path
 
 
 def make_folder_dataset(
     normal_dir: str | Path,
     root: str | Path | None = None,
     abnormal_dir: str | Path | None = None,
     normal_test_dir: str | Path | None = None,
     mask_dir: str | Path | None = None,
     split: str | Split | None = None,
     extensions: tuple[str, ...] | None = None,
 ) -> DataFrame:
     """Make Folder Dataset.
-
     Args:
         normal_dir (str | Path): Path to the directory containing normal images.
         root (str | Path | None): Path to the root directory of the dataset.
         abnormal_dir (str | Path | None, optional): Path to the directory containing abnormal images.
         normal_test_dir (str | Path | None, optional): Path to the directory containing
             normal images for the test dataset. Normal test images will be a split of `normal_dir`
             if `None`. Defaults to None.
         mask_dir (str | Path | None, optional): Path to the directory containing
             the mask annotations. Defaults to None.
         split (str | Split | None, optional): Dataset split (ie., Split.FULL, Split.TRAIN or Split.TEST).
             Defaults to None.
         extensions (tuple[str, ...] | None, optional): Type of the image extensions to read from the
             directory.
-
     Returns:
         DataFrame: an output dataframe containing samples for the requested split (ie., train or test)
     """
     normal_dir = _resolve_path(normal_dir, root)
     abnormal_dir = _resolve_path(abnormal_dir, root) if abnormal_dir is not None else None
     normal_test_dir = _resolve_path(normal_test_dir, root) if normal_test_dir is not None else None
     mask_dir = _resolve_path(mask_dir, root) if mask_dir is not None else None
     assert normal_dir.is_dir(), "A folder location must be provided in normal_dir."
 
     filenames = []
     labels = []
-    dirs = {"normal": normal_dir}
+    dirs = {DirType.NORMAL: normal_dir}
 
     if abnormal_dir:
-        dirs = {**dirs, **{"abnormal": abnormal_dir}}
+        dirs = {**dirs, **{DirType.ABNORMAL: abnormal_dir}}
 
     if normal_test_dir:
-        dirs = {**dirs, **{"normal_test": normal_test_dir}}
+        dirs = {**dirs, **{DirType.NORMAL_TEST: normal_test_dir}}
+
+    if mask_dir:
+        dirs = {**dirs, **{DirType.MASK: mask_dir}}
 
     for dir_type, path in dirs.items():
         filename, label = _prepare_files_labels(path, dir_type, extensions)
         filenames += filename
         labels += label
 
-    samples = DataFrame({"image_path": filenames, "label": labels, "mask_path": ""})
+    samples = DataFrame({"image_path": filenames, "label": labels})
+    samples = samples.sort_values(by="image_path", ignore_index=True)
 
     # Create label index for normal (0) and abnormal (1) images.
-    samples.loc[(samples.label == "normal") | (samples.label == "normal_test"), "label_index"] = 0
-    samples.loc[(samples.label == "abnormal"), "label_index"] = 1
-    samples.label_index = samples.label_index.astype(int)
+    samples.loc[
+        (samples.label == DirType.NORMAL) | (samples.label == DirType.NORMAL_TEST), "label_index"
+    ] = LabelName.NORMAL
+    samples.loc[(samples.label == DirType.ABNORMAL), "label_index"] = LabelName.ABNORMAL
+    samples.label_index = samples.label_index.astype("Int64")
 
     # If a path to mask is provided, add it to the sample dataframe.
-    if mask_dir is not None:
-        mask_dir = _check_and_convert_path(mask_dir)
-        for index, row in samples.iterrows():
-            if row.label_index == 1:
-                rel_image_path = row.image_path.relative_to(abnormal_dir)
-                samples.loc[index, "mask_path"] = str(mask_dir / rel_image_path)
-
-        # make sure all the files exist
-        # samples.image_path does NOT need to be checked because we build the df based on that
-        assert samples.mask_path.apply(
-            lambda x: Path(x).exists() if x != "" else True
-        ).all(), f"missing mask files, mask_dir={mask_dir}"
+
+    if mask_dir is not None and abnormal_dir is not None:
+        samples.loc[samples.label == DirType.ABNORMAL, "mask_path"] = samples.loc[
+            samples.label == DirType.MASK
+        ].image_path.values
+        samples["mask_path"].fillna("", inplace=True)
+        samples = samples.astype({"mask_path": "str"})
+
+        # make sure all every rgb image has a corresponding mask image.
+        assert (
+            samples.loc[samples.label_index == LabelName.ABNORMAL]
+            .apply(lambda x: Path(x.image_path).stem in Path(x.mask_path).stem, axis=1)
+            .all()
+        ), "Mismatch between anomalous images and mask images. Make sure the mask files \
+            folder follow the same naming convention as the anomalous images in the dataset \
+            (e.g. image: '000.png', mask: '000.png')."
+    else:
+        samples["mask_path"] = ""
+
+    # remove all the rows with temporal image samples that have already been assigned
+    samples = samples.loc[
+        (samples.label == DirType.NORMAL) | (samples.label == DirType.ABNORMAL) | (samples.label == DirType.NORMAL_TEST)
+    ]
 
     # Ensure the pathlib objects are converted to str.
     # This is because torch dataloader doesn't like pathlib.
     samples = samples.astype({"image_path": "str"})
 
     # Create train/test split.
     # By default, all the normal samples are assigned as train.
     #   and all the abnormal samples are test.
-    samples.loc[(samples.label == "normal"), "split"] = "train"
-    samples.loc[(samples.label == "abnormal") | (samples.label == "normal_test"), "split"] = "test"
+    samples.loc[(samples.label == DirType.NORMAL), "split"] = Split.TRAIN
+    samples.loc[(samples.label == DirType.ABNORMAL) | (samples.label == DirType.NORMAL_TEST), "split"] = Split.TEST
 
     # Get the data frame for the split.
     if split:
         samples = samples[samples.split == split]
         samples = samples.reset_index(drop=True)
 
     return samples
 
 
 class FolderDataset(AnomalibDataset):
     """Folder dataset.
-
     Args:
         task (TaskType): Task type. (``classification``, ``detection`` or ``segmentation``).
         transform (A.Compose): Albumentations Compose object describing the transforms that are applied to the inputs.
         split (str | Split | None): Fixed subset split that follows from folder structure on file system.
             Choose from [Split.FULL, Split.TRAIN, Split.TEST]
         normal_dir (str | Path): Path to the directory containing normal images.
         root (str | Path | None): Root folder of the dataset.
         abnormal_dir (str | Path | None, optional): Path to the directory containing abnormal images.
         normal_test_dir (str | Path | None, optional): Path to the directory containing
             normal images for the test dataset. Defaults to None.
         mask_dir (str | Path | None, optional): Path to the directory containing
             the mask annotations. Defaults to None.
-
         extensions (tuple[str, ...] | None, optional): Type of the image extensions to read from the
             directory.
         val_split_mode (ValSplitMode): Setting that determines how the validation subset is obtained.
-
     Raises:
         ValueError: When task is set to classification and `mask_dir` is provided. When `mask_dir` is
             provided, `task` should be set to `segmentation`.
     """
 
     def __init__(
         self,
@@ -239,15 +184,14 @@
             split=self.split,
             extensions=self.extensions,
         )
 
 
 class Folder(AnomalibDataModule):
     """Folder DataModule.
-
     Args:
         normal_dir (str | Path): Name of the directory containing normal images.
             Defaults to "normal".
         root (str | Path | None): Path to the root folder containing normal and abnormal dirs.
         abnormal_dir (str | Path | None): Name of the directory containing abnormal images.
             Defaults to "abnormal".
         normal_test_dir (str | Path | None, optional): Path to the directory containing
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/inference.py` & `anomalib-0.5.0/src/anomalib/data/inference.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/data/mvtec.py` & `anomalib-0.5.0/src/anomalib/data/mvtec.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from pandas import DataFrame
 
 from anomalib.data.base import AnomalibDataModule, AnomalibDataset
 from anomalib.data.task_type import TaskType
 from anomalib.data.utils import (
     DownloadInfo,
     InputNormalizationMethod,
+    LabelName,
     Split,
     TestSplitMode,
     ValSplitMode,
     download_and_extract,
     get_transforms,
 )
 
@@ -115,29 +116,31 @@
 
     samples = DataFrame(samples_list, columns=["path", "split", "label", "image_path"])
 
     # Modify image_path column by converting to absolute path
     samples["image_path"] = samples.path + "/" + samples.split + "/" + samples.label + "/" + samples.image_path
 
     # Create label index for normal (0) and anomalous (1) images.
-    samples.loc[(samples.label == "good"), "label_index"] = 0
-    samples.loc[(samples.label != "good"), "label_index"] = 1
+    samples.loc[(samples.label == "good"), "label_index"] = LabelName.NORMAL
+    samples.loc[(samples.label != "good"), "label_index"] = LabelName.ABNORMAL
     samples.label_index = samples.label_index.astype(int)
 
     # separate masks from samples
     mask_samples = samples.loc[samples.split == "ground_truth"].sort_values(by="image_path", ignore_index=True)
     samples = samples[samples.split != "ground_truth"].sort_values(by="image_path", ignore_index=True)
 
     # assign mask paths to anomalous test images
     samples["mask_path"] = ""
-    samples.loc[(samples.split == "test") & (samples.label_index == 1), "mask_path"] = mask_samples.image_path.values
+    samples.loc[
+        (samples.split == "test") & (samples.label_index == LabelName.ABNORMAL), "mask_path"
+    ] = mask_samples.image_path.values
 
     # assert that the right mask files are associated with the right test images
     assert (
-        samples.loc[samples.label_index == 1]
+        samples.loc[samples.label_index == LabelName.ABNORMAL]
         .apply(lambda x: Path(x.image_path).stem in Path(x.mask_path).stem, axis=1)
         .all()
     ), "Mismatch between anomalous images and ground truth masks. Make sure the mask files in 'ground_truth' \
               folder follow the same naming convention as the anomalous images in the dataset (e.g. image: '000.png', \
               mask: '000.png' or '000_mask.png')."
 
     if split:
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/shanghaitech.py` & `anomalib-0.5.0/src/anomalib/data/shanghaitech.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import numpy as np
 import pandas as pd
 import torch
 from pandas import DataFrame
 from torch import Tensor
 
 from anomalib.data.base import AnomalibVideoDataModule, AnomalibVideoDataset
+from anomalib.data.base.video import VideoTargetFrame
 from anomalib.data.task_type import TaskType
 from anomalib.data.utils import (
     DownloadInfo,
     InputNormalizationMethod,
     Split,
     ValSplitMode,
     download_and_extract,
@@ -183,27 +184,29 @@
         task (TaskType): Task type, 'classification', 'detection' or 'segmentation'
         root (Path | str): Path to the root of the dataset
         scene (int): Index of the dataset scene (category) in range [1, 13]
         transform (A.Compose): Albumentations Compose object describing the transforms that are applied to the inputs.
         split (Split): Split of the dataset, usually Split.TRAIN or Split.TEST
         clip_length_in_frames (int, optional): Number of video frames in each clip.
         frames_between_clips (int, optional): Number of frames between each consecutive video clip.
+        target_frame (VideoTargetFrame): Specifies the target frame in the video clip, used for ground truth retrieval
     """
 
     def __init__(
         self,
         task: TaskType,
         root: Path | str,
         scene: int,
         transform: A.Compose,
         split: Split,
         clip_length_in_frames: int = 1,
         frames_between_clips: int = 1,
+        target_frame: VideoTargetFrame = VideoTargetFrame.LAST,
     ):
-        super().__init__(task, transform, clip_length_in_frames, frames_between_clips)
+        super().__init__(task, transform, clip_length_in_frames, frames_between_clips, target_frame)
 
         self.root = root
         self.scene = scene
         self.split = split
         self.indexer_cls = ShanghaiTechTrainClipsIndexer if self.split == Split.TRAIN else ShanghaiTechTestClipsIndexer
 
     def _setup(self):
@@ -215,14 +218,15 @@
     """ShanghaiTech DataModule class.
 
     Args:
         root (Path | str): Path to the root of the dataset
         scene (int): Index of the dataset scene (category) in range [1, 13]
         clip_length_in_frames (int, optional): Number of video frames in each clip.
         frames_between_clips (int, optional): Number of frames between each consecutive video clip.
+        target_frame (VideoTargetFrame): Specifies the target frame in the video clip, used for ground truth retrieval
         task TaskType): Task type, 'classification', 'detection' or 'segmentation'
         image_size (int | tuple[int, int] | None, optional): Size of the input image.
             Defaults to None.
         center_crop (int | tuple[int, int] | None, optional): When provided, the images will be center-cropped
             to the provided dimensions.
         normalize (bool): When True, the images will be normalized to the ImageNet statistics.
         train_batch_size (int, optional): Training batch size. Defaults to 32.
@@ -241,14 +245,15 @@
 
     def __init__(
         self,
         root: Path | str,
         scene: int,
         clip_length_in_frames: int = 1,
         frames_between_clips: int = 1,
+        target_frame: VideoTargetFrame = VideoTargetFrame.LAST,
         task: TaskType = TaskType.SEGMENTATION,
         image_size: int | tuple[int, int] | None = None,
         center_crop: int | tuple[int, int] | None = None,
         normalization: InputNormalizationMethod | str = InputNormalizationMethod.IMAGENET,
         train_batch_size: int = 32,
         eval_batch_size: int = 32,
         num_workers: int = 8,
@@ -284,24 +289,26 @@
         )
 
         self.train_data = ShanghaiTechDataset(
             task=task,
             transform=transform_train,
             clip_length_in_frames=clip_length_in_frames,
             frames_between_clips=frames_between_clips,
+            target_frame=target_frame,
             root=root,
             scene=scene,
             split=Split.TRAIN,
         )
 
         self.test_data = ShanghaiTechDataset(
             task=task,
             transform=transform_eval,
             clip_length_in_frames=clip_length_in_frames,
             frames_between_clips=frames_between_clips,
+            target_frame=target_frame,
             root=root,
             scene=scene,
             split=Split.TEST,
         )
 
     def prepare_data(self) -> None:
         """Download the dataset and convert video files."""
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/synthetic.py` & `anomalib-0.5.0/src/anomalib/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/data/ucsd_ped.py` & `anomalib-0.5.0/src/anomalib/data/ucsd_ped.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import cv2
 import numpy as np
 import torch
 from pandas import DataFrame
 from torch import Tensor
 
 from anomalib.data.base import AnomalibVideoDataModule, AnomalibVideoDataset
+from anomalib.data.base.video import VideoTargetFrame
 from anomalib.data.task_type import TaskType
 from anomalib.data.utils import (
     DownloadInfo,
     InputNormalizationMethod,
     Split,
     ValSplitMode,
     download_and_extract,
@@ -151,27 +152,29 @@
         task (TaskType): Task type, 'classification', 'detection' or 'segmentation'
         root (Path | str): Path to the root of the dataset
         category (str): Sub-category of the dataset, e.g. 'bottle'
         transform (A.Compose): Albumentations Compose object describing the transforms that are applied to the inputs.
         split (str | Split | None): Split of the dataset, usually Split.TRAIN or Split.TEST
         clip_length_in_frames (int, optional): Number of video frames in each clip.
         frames_between_clips (int, optional): Number of frames between each consecutive video clip.
+        target_frame (VideoTargetFrame): Specifies the target frame in the video clip, used for ground truth retrieval
     """
 
     def __init__(
         self,
         task: TaskType,
         root: str | Path,
         category: str,
         transform: A.Compose,
         split: Split,
         clip_length_in_frames: int = 1,
         frames_between_clips: int = 1,
+        target_frame: VideoTargetFrame = VideoTargetFrame.LAST,
     ) -> None:
-        super().__init__(task, transform, clip_length_in_frames, frames_between_clips)
+        super().__init__(task, transform, clip_length_in_frames, frames_between_clips, target_frame)
 
         self.root_category = Path(root) / category
         self.split = split
         self.indexer_cls: Callable = UCSDpedClipsIndexer
 
     def _setup(self) -> None:
         """Create and assign samples."""
@@ -182,14 +185,15 @@
     """UCSDped DataModule class.
 
     Args:
         root (Path | str): Path to the root of the dataset
         category (str): Sub-category of the dataset, e.g. 'bottle'
         clip_length_in_frames (int, optional): Number of video frames in each clip.
         frames_between_clips (int, optional): Number of frames between each consecutive video clip.
+        target_frame (VideoTargetFrame): Specifies the target frame in the video clip, used for ground truth retrieval
         task (TaskType): Task type, 'classification', 'detection' or 'segmentation'
         image_size (int | tuple[int, int] | None, optional): Size of the input image.
             Defaults to None.
         center_crop (int | tuple[int, int] | None, optional): When provided, the images will be center-cropped
             to the provided dimensions.
         normalize (bool): When True, the images will be normalized to the ImageNet statistics.
         center_crop (int | tuple[int, int] | None, optional): When provided, the images will be center-cropped
@@ -211,14 +215,15 @@
 
     def __init__(
         self,
         root: Path | str,
         category: str,
         clip_length_in_frames: int = 1,
         frames_between_clips: int = 1,
+        target_frame: VideoTargetFrame = VideoTargetFrame.LAST,
         task: TaskType = TaskType.SEGMENTATION,
         image_size: int | tuple[int, int] | None = None,
         center_crop: int | tuple[int, int] | None = None,
         normalization: str | InputNormalizationMethod = InputNormalizationMethod.IMAGENET,
         train_batch_size: int = 32,
         eval_batch_size: int = 32,
         num_workers: int = 8,
@@ -254,24 +259,26 @@
         )
 
         self.train_data = UCSDpedDataset(
             task=task,
             transform=transform_train,
             clip_length_in_frames=clip_length_in_frames,
             frames_between_clips=frames_between_clips,
+            target_frame=target_frame,
             root=root,
             category=category,
             split=Split.TRAIN,
         )
 
         self.test_data = UCSDpedDataset(
             task=task,
             transform=transform_eval,
             clip_length_in_frames=clip_length_in_frames,
             frames_between_clips=frames_between_clips,
+            target_frame=target_frame,
             root=root,
             category=category,
             split=Split.TEST,
         )
 
     def prepare_data(self) -> None:
         """Download the dataset if not available."""
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/utils/__init__.py` & `anomalib-0.5.0/src/anomalib/data/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 from .boxes import boxes_to_anomaly_maps, boxes_to_masks, masks_to_boxes
 from .download import DownloadInfo, download_and_extract
 from .generators import random_2d_perlin
 from .image import (
     generate_output_image_filename,
     get_image_filenames,
     get_image_height_and_width,
+    read_depth_image,
     read_image,
 )
+from .label import LabelName
+from .path import DirType, _check_and_convert_path, _prepare_files_labels, _resolve_path
 from .split import (
     Split,
     TestSplitMode,
     ValSplitMode,
     concatenate_datasets,
     random_split,
     split_by_label,
@@ -25,22 +28,28 @@
 
 __all__ = [
     "generate_output_image_filename",
     "get_image_filenames",
     "get_image_height_and_width",
     "random_2d_perlin",
     "read_image",
+    "read_depth_image",
     "random_split",
     "split_by_label",
     "concatenate_datasets",
     "Split",
     "ValSplitMode",
     "TestSplitMode",
+    "LabelName",
+    "DirType",
     "Augmenter",
     "masks_to_boxes",
     "boxes_to_masks",
     "boxes_to_anomaly_maps",
     "get_transforms",
     "InputNormalizationMethod",
     "download_and_extract",
     "DownloadInfo",
+    "_check_and_convert_path",
+    "_prepare_files_labels",
+    "_resolve_path",
 ]
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/utils/augmenter.py` & `anomalib-0.5.0/src/anomalib/data/utils/augmenter.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
     def __init__(
         self,
         anomaly_source_path: str | None = None,
         p_anomalous: float = 0.5,
         beta: float | tuple[float, float] = (0.2, 1.0),
     ):
-
         self.p_anomalous = p_anomalous
         self.beta = beta
 
         self.anomaly_source_paths = []
         if anomaly_source_path is not None:
             for img_ext in IMG_EXTENSIONS:
                 self.anomaly_source_paths.extend(glob.glob(anomaly_source_path + "/**/*" + img_ext, recursive=True))
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/utils/boxes.py` & `anomalib-0.5.0/src/anomalib/data/utils/boxes.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/data/utils/download.py` & `anomalib-0.5.0/src/anomalib/data/utils/download.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import hashlib
 import io
 import logging
+import os
 import tarfile
 from dataclasses import dataclass
 from pathlib import Path
+from tarfile import TarError, TarFile
 from typing import Iterable
 from urllib.request import urlretrieve
 from zipfile import ZipFile
 
 from tqdm import tqdm
 
 logger = logging.getLogger(__name__)
@@ -241,13 +243,46 @@
 
     logger.info("Extracting dataset into root folder.")
     if downloaded_file_path.suffix == ".zip":
         with ZipFile(downloaded_file_path, "r") as zip_file:
             zip_file.extractall(root)
     elif downloaded_file_path.suffix in (".tar", ".gz", ".xz"):
         with tarfile.open(downloaded_file_path) as tar_file:
-            tar_file.extractall(root)
+            safe_extract(tar_file, root)
     else:
         raise ValueError(f"Unrecognized file format: {downloaded_file_path}")
 
     logger.info("Cleaning up files.")
     (downloaded_file_path).unlink()
+
+
+def is_within_directory(directory: Path, target: Path):
+    """Checks if a target path is located within a given directory.
+
+    Args:
+        directory (Path): path of the parent directory
+        target (Path): path of the target
+    Returns:
+        (bool): True if the target is within the directory, False otherwise
+    """
+    abs_directory = directory.resolve()
+    abs_target = target.resolve()
+
+    # TODO: replace with pathlib is_relative_to after switching to Python 3.10
+    prefix = os.path.commonprefix([abs_directory, abs_target])
+    return prefix == str(abs_directory)
+
+
+def safe_extract(tar_file: TarFile, path: str | Path = "."):
+    """Extract a tar file safely by first checking for attempted path traversal.
+
+    Args:
+        tar_file (TarFile): Tar file to be extracted
+        path (str | Path): path in which the extracted files will be placed
+    """
+    path = Path(path)
+    for member in tar_file.getmembers():
+        member_path = path / member.name
+        if not is_within_directory(path, member_path):
+            raise TarError("Attempted Path Traversal in Tar File")
+
+    tar_file.extractall(path)
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/utils/generators/perlin.py` & `anomalib-0.5.0/src/anomalib/data/utils/generators/perlin.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/data/utils/image.py` & `anomalib-0.5.0/src/anomalib/data/utils/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import math
 import warnings
 from pathlib import Path
 
 import cv2
 import numpy as np
+import tifffile as tiff
 import torch.nn.functional as F
 from torch import Tensor
 from torchvision.datasets.folder import IMG_EXTENSIONS
 
 
 def get_image_filenames(path: str | Path) -> list[Path]:
     """Get image filenames.
@@ -119,15 +120,15 @@
         output_path = Path(output_path)
 
     # This function expects an ``input_path`` that is a file. This is to check if output_path
     if input_path.is_file() is False:
         raise ValueError("input_path is expected to be a file to generate a proper output filename.")
 
     file_path: Path
-    if output_path.suffix == "":
+    if output_path.is_dir():
         # If the output is a directory, then add parent directory name
         # and filename to the path. This is to ensure we do not overwrite
         # images and organize based on the categories.
         file_path = output_path / input_path.parent.name / input_path.name
     else:
         file_path = output_path
 
@@ -202,14 +203,32 @@
         # prototyping new ideas.
         height, width = get_image_height_and_width(image_size)
         image = cv2.resize(image, dsize=(width, height), interpolation=cv2.INTER_AREA)
 
     return image
 
 
+def read_depth_image(path: str | Path) -> np.ndarray:
+    """Read tiff depth image from disk.
+
+    Args:
+        path (str, Path): path to the image file
+
+    Example:
+        >>> image = read_depth_image("test_image.tiff")
+
+    Returns:
+        image as numpy array
+    """
+    path = path if isinstance(path, str) else str(path)
+    image = tiff.imread(path)
+
+    return image
+
+
 def pad_nextpow2(batch: Tensor) -> Tensor:
     """Compute required padding from input size and return padded images.
 
     Finds the largest dimension and computes a square image of dimensions that are of the power of 2.
     In case the image dimension is odd, it returns the image with an extra padding on one side.
 
     Args:
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/utils/split.py` & `anomalib-0.5.0/src/anomalib/data/utils/split.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/data/utils/transform.py` & `anomalib-0.5.0/src/anomalib/data/utils/transform.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from __future__ import annotations
 
 import logging
 from enum import Enum
 
 import albumentations as A
 from albumentations.pytorch import ToTensorV2
+from omegaconf import DictConfig
 
 from anomalib.data.utils.image import get_image_height_and_width
 
 logger = logging.getLogger(__name__)
 
 
 class InputNormalizationMethod(str, Enum):
@@ -78,16 +79,30 @@
         >>> output = transforms(image=image)
         >>> output["image"].shape
         torch.Size([3, 1024, 1024])
     """
     transforms: A.Compose
 
     if config is not None:
+        if isinstance(config, DictConfig):
+            logger.info("Loading transforms from config File")
+            transforms_list = []
+            for key, value in config.items():
+                if hasattr(A, key):
+                    transform = getattr(A, key)(**value)
+                    logger.info(f"Transform {transform} added!")
+                    transforms_list.append(transform)
+                else:
+                    raise ValueError(f"Transformation {key} is not part of albumentations")
+
+            transforms_list.append(ToTensorV2())
+            transforms = A.Compose(transforms_list, additional_targets={"image": "image", "depth_image": "image"})
+
         # load transforms from config file
-        if isinstance(config, str):
+        elif isinstance(config, str):
             logger.info("Reading transforms from Albumentations config file: %s.", config)
             transforms = A.load(filepath=config, data_format="yaml")
         elif isinstance(config, A.Compose):
             logger.info("Transforms loaded from Albumentations Compose object")
             transforms = config
         else:
             raise ValueError("config could be either ``str`` or ``A.Compose``")
@@ -120,10 +135,10 @@
         else:
             raise ValueError(f"Unknown normalization method: {normalization}")
 
         # add tensor conversion
         if to_tensor:
             transforms_list.append(ToTensorV2())
 
-        transforms = A.Compose(transforms_list)
+        transforms = A.Compose(transforms_list, additional_targets={"image": "image", "depth_image": "image"})
 
     return transforms
```

### Comparing `anomalib-0.4.0rc2/anomalib/data/utils/video.py` & `anomalib-0.5.0/src/anomalib/data/utils/video.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/data/visa.py` & `anomalib-0.5.0/src/anomalib/data/visa.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/deploy/inferencers/base_inferencer.py` & `anomalib-0.5.0/src/anomalib/deploy/inferencers/base_inferencer.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 from skimage.segmentation import find_boundaries
 from torch import Tensor
 
 from anomalib.data.utils import read_image
 from anomalib.post_processing import ImageResult, compute_mask
 from anomalib.post_processing.normalization.cdf import normalize as normalize_cdf
 from anomalib.post_processing.normalization.cdf import standardize
-from anomalib.post_processing.normalization.min_max import (
-    normalize as normalize_min_max,
-)
+from anomalib.post_processing.normalization.min_max import normalize as normalize_min_max
 
 
 class Inferencer(ABC):
     """Abstract class for the inference.
 
     This is used by both Torch and OpenVINO inference.
     """
@@ -43,76 +41,76 @@
 
     @abstractmethod
     def forward(self, image: np.ndarray | Tensor) -> np.ndarray | Tensor:
         """Forward-Pass input to model."""
         raise NotImplementedError
 
     @abstractmethod
-    def post_process(self, predictions: np.ndarray | Tensor, meta_data: dict[str, Any] | None) -> dict[str, Any]:
+    def post_process(self, predictions: np.ndarray | Tensor, metadata: dict[str, Any] | None) -> dict[str, Any]:
         """Post-Process."""
         raise NotImplementedError
 
     def predict(
         self,
         image: str | Path | np.ndarray,
-        meta_data: dict[str, Any] | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> ImageResult:
         """Perform a prediction for a given input image.
 
         The main workflow is (i) pre-processing, (ii) forward-pass, (iii) post-process.
 
         Args:
             image (Union[str, np.ndarray]): Input image whose output is to be predicted.
                 It could be either a path to image or numpy array itself.
 
-            meta_data: Meta-data information such as shape, threshold.
+            metadata: Metadata information such as shape, threshold.
 
         Returns:
             ImageResult: Prediction results to be visualized.
         """
-        if meta_data is None:
-            if hasattr(self, "meta_data"):
-                meta_data = getattr(self, "meta_data")
+        if metadata is None:
+            if hasattr(self, "metadata"):
+                metadata = getattr(self, "metadata")
             else:
-                meta_data = {}
+                metadata = {}
         if isinstance(image, (str, Path)):
             image_arr: np.ndarray = read_image(image)
         else:  # image is already a numpy array. Kept for mypy compatibility.
             image_arr = image
-        meta_data["image_shape"] = image_arr.shape[:2]
+        metadata["image_shape"] = image_arr.shape[:2]
 
         processed_image = self.pre_process(image_arr)
         predictions = self.forward(processed_image)
-        output = self.post_process(predictions, meta_data=meta_data)
+        output = self.post_process(predictions, metadata=metadata)
 
         return ImageResult(
             image=image_arr,
             pred_score=output["pred_score"],
             pred_label=output["pred_label"],
             anomaly_map=output["anomaly_map"],
             pred_mask=output["pred_mask"],
             pred_boxes=output["pred_boxes"],
             box_labels=output["box_labels"],
         )
 
     @staticmethod
-    def _superimpose_segmentation_mask(meta_data: dict, anomaly_map: np.ndarray, image: np.ndarray) -> np.ndarray:
+    def _superimpose_segmentation_mask(metadata: dict, anomaly_map: np.ndarray, image: np.ndarray) -> np.ndarray:
         """Superimpose segmentation mask on top of image.
 
         Args:
-            meta_data (dict): Metadata of the image which contains the image size.
+            metadata (dict): Metadata of the image which contains the image size.
             anomaly_map (np.ndarray): Anomaly map which is used to extract segmentation mask.
             image (np.ndarray): Image on which segmentation mask is to be superimposed.
 
         Returns:
             np.ndarray: Image with segmentation mask superimposed.
         """
         pred_mask = compute_mask(anomaly_map, 0.5)  # assumes predictions are normalized.
-        image_height = meta_data["image_shape"][0]
-        image_width = meta_data["image_shape"][1]
+        image_height = metadata["image_shape"][0]
+        image_width = metadata["image_shape"][1]
         pred_mask = cv2.resize(pred_mask, (image_width, image_height))
         boundaries = find_boundaries(pred_mask)
         outlines = dilation(boundaries, np.ones((7, 7)))
         image[outlines] = [255, 0, 0]
         return image
 
     def __call__(self, image: np.ndarray) -> ImageResult:
@@ -125,63 +123,69 @@
             ImageResult: Prediction results to be visualized.
         """
         return self.predict(image)
 
     @staticmethod
     def _normalize(
         pred_scores: Tensor | np.float32,
-        meta_data: dict | DictConfig,
+        metadata: dict | DictConfig,
         anomaly_maps: Tensor | np.ndarray | None = None,
     ) -> tuple[np.ndarray | Tensor | None, float]:
         """Applies normalization and resizes the image.
 
         Args:
             pred_scores (Tensor | np.float32): Predicted anomaly score
-            meta_data (dict | DictConfig): Meta data. Post-processing step sometimes requires
+            metadata (dict | DictConfig): Meta data. Post-processing step sometimes requires
                 additional meta data such as image shape. This variable comprises such info.
             anomaly_maps (Tensor | np.ndarray | None): Predicted raw anomaly map.
 
         Returns:
             tuple[np.ndarray | Tensor | None, float]: Post processed predictions that are ready to be
                 visualized and predicted scores.
         """
 
         # min max normalization
-        if "min" in meta_data and "max" in meta_data:
+        if "min" in metadata and "max" in metadata:
             if anomaly_maps is not None:
                 anomaly_maps = normalize_min_max(
-                    anomaly_maps, meta_data["pixel_threshold"], meta_data["min"], meta_data["max"]
+                    anomaly_maps,
+                    metadata["pixel_threshold"],
+                    metadata["min"],
+                    metadata["max"],
                 )
             pred_scores = normalize_min_max(
-                pred_scores, meta_data["image_threshold"], meta_data["min"], meta_data["max"]
+                pred_scores,
+                metadata["image_threshold"],
+                metadata["min"],
+                metadata["max"],
             )
 
         # standardize pixel scores
-        if "pixel_mean" in meta_data.keys() and "pixel_std" in meta_data.keys():
+        if "pixel_mean" in metadata.keys() and "pixel_std" in metadata.keys():
             if anomaly_maps is not None:
                 anomaly_maps = standardize(
-                    anomaly_maps, meta_data["pixel_mean"], meta_data["pixel_std"], center_at=meta_data["image_mean"]
+                    anomaly_maps, metadata["pixel_mean"], metadata["pixel_std"], center_at=metadata["image_mean"]
                 )
-                anomaly_maps = normalize_cdf(anomaly_maps, meta_data["pixel_threshold"])
+                anomaly_maps = normalize_cdf(anomaly_maps, metadata["pixel_threshold"])
 
         # standardize image scores
-        if "image_mean" in meta_data.keys() and "image_std" in meta_data.keys():
-            pred_scores = standardize(pred_scores, meta_data["image_mean"], meta_data["image_std"])
-            pred_scores = normalize_cdf(pred_scores, meta_data["image_threshold"])
+        if "image_mean" in metadata.keys() and "image_std" in metadata.keys():
+            pred_scores = standardize(pred_scores, metadata["image_mean"], metadata["image_std"])
+            pred_scores = normalize_cdf(pred_scores, metadata["image_threshold"])
 
         return anomaly_maps, float(pred_scores)
 
-    def _load_meta_data(self, path: str | Path | None = None) -> dict | DictConfig:
+    def _load_metadata(self, path: str | Path | None = None) -> dict | DictConfig:
         """Loads the meta data from the given path.
 
         Args:
             path (str | Path | None, optional): Path to JSON file containing the metadata.
                 If no path is provided, it returns an empty dict. Defaults to None.
 
         Returns:
             dict | DictConfig: Dictionary containing the metadata.
         """
-        meta_data: dict[str, float | np.ndarray | Tensor] | DictConfig = {}
+        metadata: dict[str, float | np.ndarray | Tensor] | DictConfig = {}
         if path is not None:
             config = OmegaConf.load(path)
-            meta_data = cast(DictConfig, config)
-        return meta_data
+            metadata = cast(DictConfig, config)
+        return metadata
```

### Comparing `anomalib-0.4.0rc2/anomalib/deploy/inferencers/openvino_inferencer.py` & `anomalib-0.5.0/src/anomalib/deploy/inferencers/openvino_inferencer.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,58 +5,50 @@
 
 from __future__ import annotations
 
 from importlib.util import find_spec
 from pathlib import Path
 from typing import Any
 
+import albumentations as A
 import cv2
 import numpy as np
-from omegaconf import DictConfig, ListConfig
+from omegaconf import DictConfig
 
-from anomalib.config import get_configurable_parameters
 from anomalib.data import TaskType
-from anomalib.data.utils import InputNormalizationMethod, get_transforms
 
 from .base_inferencer import Inferencer
 
 if find_spec("openvino") is not None:
     from openvino.inference_engine import (  # type: ignore  # pylint: disable=no-name-in-module
         IECore,
     )
 
 
 class OpenVINOInferencer(Inferencer):
     """OpenVINO implementation for the inference.
 
     Args:
-        config (str | Path | DictConfig | ListConfig): Configurable parameters that are used
-            during the training stage.
         path (str | Path): Path to the openvino onnx, xml or bin file.
-        meta_data_path (str | Path, optional): Path to metadata file. Defaults to None.
+        metadata_path (str | Path, optional): Path to metadata file. Defaults to None.
+        device (str | None, optional): Device to run the inference on. Defaults to "CPU".
+        task (TaskType | None, optional): Task type. Defaults to None.
     """
 
     def __init__(
         self,
-        config: str | Path | DictConfig | ListConfig,
         path: str | Path | tuple[bytes, bytes],
-        meta_data_path: str | Path | None = None,
+        metadata_path: str | Path | None = None,
         device: str | None = "CPU",
+        task: str | None = None,
     ) -> None:
-        # Check and load the configuration
-        if isinstance(config, (str, Path)):
-            self.config = get_configurable_parameters(config_path=config)
-        elif isinstance(config, (DictConfig, ListConfig)):
-            self.config = config
-        else:
-            raise ValueError(f"Unknown config type {type(config)}")
-
         self.device = device
         self.input_blob, self.output_blob, self.network = self.load_model(path)
-        self.meta_data = super()._load_meta_data(meta_data_path)
+        self.metadata = super()._load_metadata(metadata_path)
+        self.task = TaskType(task) if task else TaskType(self.metadata["task"])
 
     def load_model(self, path: str | Path | tuple[bytes, bytes]):
         """Load the OpenVINO model.
 
         Args:
             path (str | Path | tuple[bytes, bytes]): Path to the onnx or xml and bin files
                                                         or tuple of .xml and .bin data as bytes.
@@ -94,26 +86,15 @@
 
         Args:
             image (np.ndarray): Input image.
 
         Returns:
             np.ndarray: pre-processed image.
         """
-        transform_config = (
-            self.config.dataset.transform_config.eval if "transform_config" in self.config.dataset.keys() else None
-        )
-
-        image_size = (self.config.dataset.image_size[0], self.config.dataset.image_size[1])
-        center_crop = self.config.dataset.get("center_crop")
-        if center_crop is not None:
-            center_crop = tuple(center_crop)
-        normalization = InputNormalizationMethod(self.config.dataset.normalization)
-        transform = get_transforms(
-            config=transform_config, image_size=image_size, center_crop=center_crop, normalization=normalization
-        )
+        transform = A.from_dict(self.metadata["transform"])
         processed_image = transform(image=image)["image"]
 
         if len(processed_image.shape) == 3:
             processed_image = np.expand_dims(processed_image, axis=0)
 
         if processed_image.shape[-1] == 3:
             processed_image = processed_image.transpose(0, 3, 1, 2)
@@ -127,28 +108,28 @@
             image (np.ndarray): Input tensor.
 
         Returns:
             np.ndarray: Output predictions.
         """
         return self.network.infer(inputs={self.input_blob: image})
 
-    def post_process(self, predictions: np.ndarray, meta_data: dict | DictConfig | None = None) -> dict[str, Any]:
+    def post_process(self, predictions: np.ndarray, metadata: dict | DictConfig | None = None) -> dict[str, Any]:
         """Post process the output predictions.
 
         Args:
             predictions (np.ndarray): Raw output predicted by the model.
-            meta_data (Dict, optional): Meta data. Post-processing step sometimes requires
+            metadata (Dict, optional): Meta data. Post-processing step sometimes requires
                 additional meta data such as image shape. This variable comprises such info.
                 Defaults to None.
 
         Returns:
             dict[str, Any]: Post processed prediction results.
         """
-        if meta_data is None:
-            meta_data = self.meta_data
+        if metadata is None:
+            metadata = self.metadata
 
         predictions = predictions[self.output_blob]
 
         # Initialize the result variables.
         anomaly_map: np.ndarray | None = None
         pred_label: float | None = None
         pred_mask: float | None = None
@@ -162,39 +143,39 @@
             task = TaskType.SEGMENTATION
             anomaly_map = predictions.squeeze()
             pred_score = anomaly_map.reshape(-1).max()
 
         # Common practice in anomaly detection is to assign anomalous
         # label to the prediction if the prediction score is greater
         # than the image threshold.
-        if "image_threshold" in meta_data:
-            pred_label = pred_score >= meta_data["image_threshold"]
+        if "image_threshold" in metadata:
+            pred_label = pred_score >= metadata["image_threshold"]
 
         if task == TaskType.CLASSIFICATION:
-            _, pred_score = self._normalize(pred_scores=pred_score, meta_data=meta_data)
+            _, pred_score = self._normalize(pred_scores=pred_score, metadata=metadata)
         elif task in (TaskType.SEGMENTATION, TaskType.DETECTION):
-            if "pixel_threshold" in meta_data:
-                pred_mask = (anomaly_map >= meta_data["pixel_threshold"]).astype(np.uint8)
+            if "pixel_threshold" in metadata:
+                pred_mask = (anomaly_map >= metadata["pixel_threshold"]).astype(np.uint8)
 
             anomaly_map, pred_score = self._normalize(
-                pred_scores=pred_score, anomaly_maps=anomaly_map, meta_data=meta_data
+                pred_scores=pred_score, anomaly_maps=anomaly_map, metadata=metadata
             )
             assert anomaly_map is not None
 
-            if "image_shape" in meta_data and anomaly_map.shape != meta_data["image_shape"]:
-                image_height = meta_data["image_shape"][0]
-                image_width = meta_data["image_shape"][1]
+            if "image_shape" in metadata and anomaly_map.shape != metadata["image_shape"]:
+                image_height = metadata["image_shape"][0]
+                image_width = metadata["image_shape"][1]
                 anomaly_map = cv2.resize(anomaly_map, (image_width, image_height))
 
                 if pred_mask is not None:
                     pred_mask = cv2.resize(pred_mask, (image_width, image_height))
         else:
             raise ValueError(f"Unknown task type: {task}")
 
-        if self.config.dataset.task == TaskType.DETECTION:
+        if self.task == TaskType.DETECTION:
             pred_boxes = self._get_boxes(pred_mask)
             box_labels = np.ones(pred_boxes.shape[0])
         else:
             pred_boxes = None
             box_labels = None
 
         return {
```

### Comparing `anomalib-0.4.0rc2/anomalib/deploy/inferencers/torch_inferencer.py` & `anomalib-0.5.0/src/anomalib/deploy/inferencers/torch_inferencer.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,68 +4,46 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any
 
+import albumentations as A
 import cv2
 import numpy as np
 import torch
-from omegaconf import DictConfig, ListConfig
-from torch import Tensor
+from omegaconf import DictConfig
+from torch import Tensor, nn
 
-from anomalib.config import get_configurable_parameters
 from anomalib.data import TaskType
-from anomalib.data.utils import InputNormalizationMethod, get_transforms
 from anomalib.data.utils.boxes import masks_to_boxes
-from anomalib.deploy.export import get_model_metadata
-from anomalib.models import get_model
-from anomalib.models.components import AnomalyModule
 
 from .base_inferencer import Inferencer
 
 
 class TorchInferencer(Inferencer):
     """PyTorch implementation for the inference.
 
     Args:
-        config (str | Path | DictConfig | ListConfig): Configurable parameters that are used
-            during the training stage.
-        model_source (str | Path | AnomalyModule): Path to the model ckpt file or the Anomaly model.
-        meta_data_path (str | Path, optional): Path to metadata file. If none, it tries to load the params
-                from the model state_dict. Defaults to None.
-        device (str | None, optional): Device to use for inference. Options are auto, cpu, cuda. Defaults to "auto".
+        path (str | Path): Path to Torch model weights.
+        device (str): Device to use for inference. Options are auto, cpu, cuda. Defaults to "auto".
     """
 
     def __init__(
         self,
-        config: str | Path | DictConfig | ListConfig,
-        model_source: str | Path | AnomalyModule,
-        meta_data_path: str | Path | None = None,
+        path: str | Path,
         device: str = "auto",
     ) -> None:
-
         self.device = self._get_device(device)
 
-        # Check and load the configuration
-        if isinstance(config, (str, Path)):
-            self.config = get_configurable_parameters(config_path=config)
-        elif isinstance(config, (DictConfig, ListConfig)):
-            self.config = config
-        else:
-            raise ValueError(f"Unknown config type {type(config)}")
-
-        # Check and load the model weights.
-        if isinstance(model_source, AnomalyModule):
-            self.model = model_source
-        else:
-            self.model = self.load_model(model_source)
-
-        self.meta_data = self._load_meta_data(meta_data_path)
+        # Load the model weights.
+        self.model = self.load_model(path)
+        self.metadata = self._load_metadata(path)
+        self.transform = A.from_dict(self.metadata["transform"])
 
     @staticmethod
     def _get_device(device: str) -> torch.device:
         """Get the device to use for inference.
 
         Args:
             device (str): Device to use for inference. Options are auto, cpu, cuda.
@@ -78,67 +56,50 @@
 
         if device == "auto":
             device = "cuda" if torch.cuda.is_available() else "cpu"
         elif device == "gpu":
             device = "cuda"
         return torch.device(device)
 
-    def _load_meta_data(self, path: str | Path | None = None) -> dict | DictConfig:
-        """Load metadata from file or from model state dict.
+    def _load_metadata(self, path: str | Path | None = None) -> dict | DictConfig:
+        """Load metadata from file.
 
         Args:
-            path (str | Path | None, optional): Path to metadata file. If none, it tries to load the params
-                from the model state_dict. Defaults to None.
+            path (str | Path): Path to the model pt file.
 
         Returns:
-            dict: Dictionary containing the meta_data.
+            dict: Dictionary containing the metadata.
         """
-        meta_data: dict[str, float | np.ndarray | Tensor] | DictConfig
-        if path is None:
-            meta_data = get_model_metadata(self.model)
-        else:
-            meta_data = super()._load_meta_data(path)
-        return meta_data
+        metadata = torch.load(path, map_location=self.device)["metadata"] if path else {}
+        return metadata
 
-    def load_model(self, path: str | Path) -> AnomalyModule:
+    def load_model(self, path: str | Path) -> nn.Module:
         """Load the PyTorch model.
 
         Args:
             path (str | Path): Path to model ckpt file.
 
         Returns:
             (AnomalyModule): PyTorch Lightning model.
         """
-        model = get_model(self.config)
-        model.load_state_dict(torch.load(path, map_location=self.device)["state_dict"])
+
+        model = torch.load(path, map_location=self.device)["model"]
         model.eval()
         return model.to(self.device)
 
     def pre_process(self, image: np.ndarray) -> Tensor:
         """Pre process the input image by applying transformations.
 
         Args:
             image (np.ndarray): Input image
 
         Returns:
             Tensor: pre-processed image.
         """
-        transform_config = (
-            self.config.dataset.transform_config.eval if "transform_config" in self.config.dataset.keys() else None
-        )
-
-        image_size = (self.config.dataset.image_size[0], self.config.dataset.image_size[1])
-        center_crop = self.config.dataset.get("center_crop")
-        if center_crop is not None:
-            center_crop = tuple(center_crop)
-        normalization = InputNormalizationMethod(self.config.dataset.normalization)
-        transform = get_transforms(
-            config=transform_config, image_size=image_size, center_crop=center_crop, normalization=normalization
-        )
-        processed_image = transform(image=image)["image"]
+        processed_image = self.transform(image=image)["image"]
 
         if len(processed_image) == 3:
             processed_image = processed_image.unsqueeze(0)
 
         return processed_image.to(self.device)
 
     def forward(self, image: Tensor) -> Tensor:
@@ -148,28 +109,28 @@
             image (Tensor): Input tensor.
 
         Returns:
             Tensor: Output predictions.
         """
         return self.model(image)
 
-    def post_process(self, predictions: Tensor, meta_data: dict | DictConfig | None = None) -> dict[str, Any]:
+    def post_process(self, predictions: Tensor, metadata: dict | DictConfig | None = None) -> dict[str, Any]:
         """Post process the output predictions.
 
         Args:
             predictions (Tensor): Raw output predicted by the model.
-            meta_data (dict, optional): Meta data. Post-processing step sometimes requires
+            metadata (dict, optional): Meta data. Post-processing step sometimes requires
                 additional meta data such as image shape. This variable comprises such info.
                 Defaults to None.
 
         Returns:
             dict[str, str | float | np.ndarray]: Post processed prediction results.
         """
-        if meta_data is None:
-            meta_data = self.meta_data
+        if metadata is None:
+            metadata = self.metadata
 
         if isinstance(predictions, Tensor):
             anomaly_map = predictions.detach().cpu().numpy()
             pred_score = anomaly_map.reshape(-1).max()
         else:
             # NOTE: Patchcore `forward`` returns heatmap and score.
             #   We need to add the following check to ensure the variables
@@ -183,37 +144,37 @@
                 anomaly_map, pred_score = predictions
                 pred_score = pred_score.detach()
 
         # Common practice in anomaly detection is to assign anomalous
         # label to the prediction if the prediction score is greater
         # than the image threshold.
         pred_label: str | None = None
-        if "image_threshold" in meta_data:
-            pred_idx = pred_score >= meta_data["image_threshold"]
+        if "image_threshold" in metadata:
+            pred_idx = pred_score >= metadata["image_threshold"]
             pred_label = "Anomalous" if pred_idx else "Normal"
 
         pred_mask: np.ndarray | None = None
-        if "pixel_threshold" in meta_data:
-            pred_mask = (anomaly_map >= meta_data["pixel_threshold"]).squeeze().astype(np.uint8)
+        if "pixel_threshold" in metadata:
+            pred_mask = (anomaly_map >= metadata["pixel_threshold"]).squeeze().astype(np.uint8)
 
         anomaly_map = anomaly_map.squeeze()
-        anomaly_map, pred_score = self._normalize(anomaly_maps=anomaly_map, pred_scores=pred_score, meta_data=meta_data)
+        anomaly_map, pred_score = self._normalize(anomaly_maps=anomaly_map, pred_scores=pred_score, metadata=metadata)
 
         if isinstance(anomaly_map, Tensor):
             anomaly_map = anomaly_map.detach().cpu().numpy()
 
-        if "image_shape" in meta_data and anomaly_map.shape != meta_data["image_shape"]:
-            image_height = meta_data["image_shape"][0]
-            image_width = meta_data["image_shape"][1]
+        if "image_shape" in metadata and anomaly_map.shape != metadata["image_shape"]:
+            image_height = metadata["image_shape"][0]
+            image_width = metadata["image_shape"][1]
             anomaly_map = cv2.resize(anomaly_map, (image_width, image_height))
 
             if pred_mask is not None:
                 pred_mask = cv2.resize(pred_mask, (image_width, image_height))
 
-        if self.config.dataset.task == TaskType.DETECTION:
+        if self.metadata["task"] == TaskType.DETECTION:
             pred_boxes = masks_to_boxes(torch.from_numpy(pred_mask))[0][0].numpy()
             box_labels = np.ones(pred_boxes.shape[0])
         else:
             pred_boxes = None
             box_labels = None
 
         return {
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/__init__.py` & `anomalib-0.5.0/src/anomalib/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import logging
 import os
 from importlib import import_module
 
 from omegaconf import DictConfig, ListConfig
 from torch import load
 
+from anomalib.models.ai_vad import AiVad
 from anomalib.models.cfa import Cfa
 from anomalib.models.cflow import Cflow
 from anomalib.models.components import AnomalyModule
 from anomalib.models.csflow import Csflow
 from anomalib.models.dfkde import Dfkde
 from anomalib.models.dfm import Dfm
 from anomalib.models.draem import Draem
@@ -37,14 +38,15 @@
     "Fastflow",
     "Ganomaly",
     "Padim",
     "Patchcore",
     "ReverseDistillation",
     "Rkde",
     "Stfpm",
+    "AiVad",
 ]
 
 logger = logging.getLogger(__name__)
 
 
 def _snake_to_pascal_case(model_name: str) -> str:
     """Convert model name from snake case to Pascal case.
@@ -88,14 +90,15 @@
         "fastflow",
         "ganomaly",
         "padim",
         "patchcore",
         "reverse_distillation",
         "rkde",
         "stfpm",
+        "ai_vad",
     ]
     model: AnomalyModule
 
     if config.model.name in model_list:
         module = import_module(f"anomalib.models.{config.model.name}")
         model = getattr(module, f"{_snake_to_pascal_case(config.model.name)}Lightning")(config)
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/cfa/anomaly_map.py` & `anomalib-0.5.0/src/anomalib/models/cfa/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/cfa/config.yaml` & `anomalib-0.5.0/src/anomalib/models/cfa/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
   path: ./results
 
 logging:
   logger: [] # options: [comet, tensorboard, wandb, csv] or combinations.
   log_graph: false # Logs the model graph to respective logger.
 
 optimization:
-  export_mode: null #options: onnx, openvino
+  export_mode: null # options: torch, onnx, openvino
 
 # PL Trainer Args. Don't add extra parameter here.
 trainer:
   enable_checkpointing: true
   default_root_dir: null
   gradient_clip_val: 0
   gradient_clip_algorithm: norm
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/cfa/lightning_model.py` & `anomalib-0.5.0/src/anomalib/models/cfa/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/cfa/loss.py` & `anomalib-0.5.0/src/anomalib/models/cfa/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/cfa/torch_model.py` & `anomalib-0.5.0/src/anomalib/models/cfa/torch_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,23 +110,23 @@
         self.num_hard_negative_features = num_hard_negative_features
 
         self.register_buffer("memory_bank", torch.tensor(0.0))
         self.memory_bank: Tensor
 
         return_nodes = get_return_nodes(backbone)
         self.feature_extractor = get_feature_extractor(backbone, return_nodes)
-        feature_map_meta_data = dryrun_find_featuremap_dims(
+        feature_map_metadata = dryrun_find_featuremap_dims(
             feature_extractor=self.feature_extractor,
             input_size=input_size,
             layers=return_nodes,
         )
         # Scale is to get the largest feature map dimensions of different layers
         # of the feature extractor. In a typical feature extractor, the first
         # layer has the highest resolution.
-        resolution = list(feature_map_meta_data.values())[0]["resolution"]
+        resolution = list(feature_map_metadata.values())[0]["resolution"]
         if isinstance(resolution, int):
             self.scale = (resolution,) * 2
         elif isinstance(resolution, tuple):
             self.scale = resolution
         else:
             raise ValueError(
                 f"Unknown type {type(resolution)} for `resolution`. Expected types are either int or tuple[int, int]."
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/cflow/anomaly_map.py` & `anomalib-0.5.0/src/anomalib/models/cflow/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/cflow/config.yaml` & `anomalib-0.5.0/src/anomalib/models/cflow/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
   path: ./results
 
 logging:
   logger: [] # options: [comet, tensorboard, wandb, csv] or combinations.
   log_graph: false # Logs the model graph to respective logger.
 
 optimization:
-  export_mode: null #options: onnx, openvino
+  export_mode: null # options: torch, onnx, openvino
 
 # PL Trainer Args. Don't add extra parameter here.
 trainer:
   enable_checkpointing: true
   default_root_dir: null
   gradient_clip_val: 0
   gradient_clip_algorithm: norm
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/cflow/lightning_model.py` & `anomalib-0.5.0/src/anomalib/models/cflow/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/cflow/torch_model.py` & `anomalib-0.5.0/src/anomalib/models/cflow/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/cflow/utils.py` & `anomalib-0.5.0/src/anomalib/models/cflow/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 import logging
 import math
 
 import numpy as np
 import torch
 from FrEIA.framework import SequenceINN
-from FrEIA.modules import AllInOneBlock
 from torch import Tensor, nn
 
+from anomalib.models.components.flow import AllInOneBlock
+
 logger = logging.getLogger(__name__)
 
 
 def get_logp(dim_feature_vector: int, p_u: Tensor, logdet_j: Tensor) -> Tensor:
     """Returns the log likelihood estimation.
 
     Args:
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/__init__.py` & `anomalib-0.5.0/src/anomalib/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/base/anomaly_module.py` & `anomalib-0.5.0/src/anomalib/models/components/base/anomaly_module.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/base/dynamic_module.py` & `anomalib-0.5.0/src/anomalib/models/components/base/dynamic_module.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/classification/kde_classifier.py` & `anomalib-0.5.0/src/anomalib/models/components/classification/kde_classifier.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/dimensionality_reduction/pca.py` & `anomalib-0.5.0/src/anomalib/models/components/dimensionality_reduction/pca.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/dimensionality_reduction/random_projection.py` & `anomalib-0.5.0/src/anomalib/models/components/dimensionality_reduction/random_projection.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/feature_extractors/timm.py` & `anomalib-0.5.0/src/anomalib/models/components/feature_extractors/timm.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/feature_extractors/torchfx.py` & `anomalib-0.5.0/src/anomalib/models/components/feature_extractors/torchfx.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 from torchvision.models.feature_extraction import create_feature_extractor
 
 
 @dataclass
 class BackboneParams:
     """Used for serializing the backbone."""
 
-    class_path: str | nn.Module
+    class_path: str | type[nn.Module]
     init_args: dict = field(default_factory=dict)
 
 
 class TorchFXFeatureExtractor(nn.Module):
     """Extract features from a CNN.
 
     Args:
         backbone (str | BackboneParams | dict | nn.Module): The backbone to which the feature extraction hooks are
             attached. If the name is provided, the model is loaded from torchvision. Otherwise, the model class can be
-            provided and it will try to load the weights from the provided weights file.
+            provided and it will try to load the weights from the provided weights file. Last, an instance of nn.Module
+            can also be passed directly.
         return_nodes (Iterable[str]): List of layer names of the backbone to which the hooks are attached.
             You can find the names of these nodes by using ``get_graph_node_names`` function.
         weights (str | WeightsEnum | None): Weights enum to use for the model. Torchvision models require
             ``WeightsEnum``. These enums are defined in ``torchvision.models.<model>``. You can pass the weights
             path for custom models.
         requires_grad (bool): Models like ``stfpm`` use the feature extractor for training. In such cases we should
             set ``requires_grad`` to ``True``. Default is ``False``.
@@ -55,79 +56,103 @@
             >>> [layer for layer in features.keys()]
                 ["features.6.8"]
             >>> [feature.shape for feature in features.values()]
                 [torch.Size([32, 304, 8, 8])]
 
         With custom models:
 
+            >>> import torch
             >>> from anomalib.models.components.feature_extractors import TorchFXFeatureExtractor
             >>> feature_extractor = TorchFXFeatureExtractor(
                     "path.to.CustomModel", ["linear_relu_stack.3"], weights="path/to/weights.pth"
                 )
             >>> input = torch.randn(1, 1, 28, 28)
             >>> features = feature_extractor(input)
             >>> [layer for layer in features.keys()]
                 ["linear_relu_stack.3"]
+
+        with model instances:
+
+            >>> import torch
+            >>> from anomalib.models.components.feature_extractors import TorchFXFeatureExtractor
+            >>> from timm import create_model
+            >>> model = create_model("resnet18", pretrained=True)
+            >>> feature_extractor = TorchFXFeatureExtractor(model, ["layer1"])
+            >>> input = torch.rand((32, 3, 256, 256))
+            >>> features = feature_extractor(input)
+            >>> [layer for layer in features.keys()]
+                ["layer1"]
+            >>> [feature.shape for feature in features.values()]
+                [torch.Size([32, 64, 64, 64])]
     """
 
     def __init__(
         self,
         backbone: str | BackboneParams | dict | nn.Module,
         return_nodes: list[str],
         weights: str | WeightsEnum | None = None,
         requires_grad: bool = False,
     ):
         super().__init__()
         if isinstance(backbone, dict):
             backbone = BackboneParams(**backbone)
-        elif not isinstance(backbone, BackboneParams):  # if str or nn.Module
+        elif isinstance(backbone, str):
             backbone = BackboneParams(class_path=backbone)
+        elif not isinstance(backbone, (nn.Module, BackboneParams)):
+            raise ValueError(
+                f"backbone needs to be of type str | BackboneParams | dict | nn.Module, but was type {type(backbone)}"
+            )
 
         self.feature_extractor = self.initialize_feature_extractor(backbone, return_nodes, weights, requires_grad)
 
     def initialize_feature_extractor(
         self,
-        backbone: BackboneParams,
+        backbone: BackboneParams | nn.Module,
         return_nodes: list[str],
         weights: str | WeightsEnum | None = None,
         requires_grad: bool = False,
-    ) -> GraphModule | nn.Module:
+    ) -> GraphModule:
         """Extract features from a CNN.
 
         Args:
-            backbone (BackboneParams): The backbone to which the feature extraction hooks are attached.
-                If the name is provided, the model is loaded from torchvision. Otherwise, the model class can be
-                provided and it will try to load the weights from the provided weights file.
+            backbone (BackboneParams | nn.Module): The backbone to which the feature extraction hooks are attached.
+                If the name is provided for BackboneParams, the model is loaded from torchvision. Otherwise, the model
+                class can be provided and it will try to load the weights from the provided weights file. Last, an
+                instance of the model can be provided as well, which will be used as-is.
             return_nodes (Iterable[str]): List of layer names of the backbone to which the hooks are attached.
                 You can find the names of these nodes by using ``get_graph_node_names`` function.
             weights (str | WeightsEnum | None): Weights enum to use for the model. Torchvision models require
                 ``WeightsEnum``. These enums are defined in ``torchvision.models.<model>``. You can pass the weights
                 path for custom models.
             requires_grad (bool): Models like ``stfpm`` use the feature extractor for training. In such cases we should
                 set ``requires_grad`` to ``True``. Default is ``False``.
 
         Returns:
             Feature Extractor based on TorchFX.
         """
-        if isinstance(backbone.class_path, str):
-            backbone_class = self._get_backbone_class(backbone.class_path)
-            backbone_model = backbone_class(weights=weights, **backbone.init_args)
+        if isinstance(backbone, nn.Module):
+            backbone_model = backbone
         else:
-            backbone_class = backbone.class_path
-            backbone_model = backbone_class(**backbone.init_args)
-        if isinstance(weights, WeightsEnum):  # torchvision models
-            feature_extractor = create_feature_extractor(model=backbone_model, return_nodes=return_nodes)
-        else:
-            if weights is not None:
-                assert isinstance(weights, str), "Weights should point to a path"
-                model_weights = torch.load(weights)
-                if "state_dict" in model_weights:
-                    model_weights = model_weights["state_dict"]
-                backbone_model.load_state_dict(model_weights)
-            feature_extractor = create_feature_extractor(backbone_model, return_nodes)
+            if isinstance(backbone.class_path, str):
+                backbone_class = self._get_backbone_class(backbone.class_path)
+                backbone_model = backbone_class(weights=weights, **backbone.init_args)
+            else:
+                backbone_class = backbone.class_path
+                backbone_model = backbone_class(**backbone.init_args)
+            if isinstance(weights, WeightsEnum):  # torchvision models
+                feature_extractor = create_feature_extractor(model=backbone_model, return_nodes=return_nodes)
+            else:
+                if weights is not None:
+                    assert isinstance(weights, str), "Weights should point to a path"
+                    model_weights = torch.load(weights)
+                    if "state_dict" in model_weights:
+                        model_weights = model_weights["state_dict"]
+                    backbone_model.load_state_dict(model_weights)
+
+        feature_extractor = create_feature_extractor(backbone_model, return_nodes)
 
         if not requires_grad:
             feature_extractor.eval()
             for param in feature_extractor.parameters():
                 param.requires_grad_(False)
 
         return feature_extractor
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/feature_extractors/utils.py` & `anomalib-0.5.0/src/anomalib/models/components/feature_extractors/utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/filters/blur.py` & `anomalib-0.5.0/src/anomalib/models/components/filters/blur.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/layers/sspcab.py` & `anomalib-0.5.0/src/anomalib/models/components/layers/sspcab.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         reduction_ratio (int): Reduction ratio of the attention module.
     """
 
     def __init__(self, in_channels: int, kernel_size: int = 1, dilation: int = 1, reduction_ratio: int = 8):
         super().__init__()
 
         self.pad = kernel_size + dilation
-        self.crop = 2 * (kernel_size + dilation)
+        self.crop = kernel_size + 2 * dilation + 1
 
         self.masked_conv1 = nn.Conv2d(in_channels=in_channels, out_channels=in_channels, kernel_size=kernel_size)
         self.masked_conv2 = nn.Conv2d(in_channels=in_channels, out_channels=in_channels, kernel_size=kernel_size)
         self.masked_conv3 = nn.Conv2d(in_channels=in_channels, out_channels=in_channels, kernel_size=kernel_size)
         self.masked_conv4 = nn.Conv2d(in_channels=in_channels, out_channels=in_channels, kernel_size=kernel_size)
 
         self.attention_module = AttentionModule(in_channels=in_channels, reduction_ratio=reduction_ratio)
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/sampling/k_center_greedy.py` & `anomalib-0.5.0/src/anomalib/models/components/sampling/k_center_greedy.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/stats/kde.py` & `anomalib-0.5.0/src/anomalib/models/components/stats/kde.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/components/stats/multi_variate_gaussian.py` & `anomalib-0.5.0/src/anomalib/models/components/stats/multi_variate_gaussian.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/csflow/anomaly_map.py` & `anomalib-0.5.0/src/anomalib/models/csflow/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/csflow/config.yaml` & `anomalib-0.5.0/src/anomalib/models/csflow/config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
   path: ./results
 
 logging:
   logger: [] # options: [comet, tensorboard, wandb, csv] or combinations.
   log_graph: false # Logs the model graph to respective logger.
 
 optimization:
-  export_mode: null #options: onnx, openvino
+  export_mode: null # options: torch, onnx, openvino
 # PL Trainer Args. Don't add extra parameter here.
 trainer:
   enable_checkpointing: true
   default_root_dir: null
   gradient_clip_val: 1 # Grad clip value set based on the official implementation
   gradient_clip_algorithm: norm
   num_nodes: 1
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/csflow/lightning_model.py` & `anomalib-0.5.0/src/anomalib/models/csflow/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/csflow/loss.py` & `anomalib-0.5.0/src/anomalib/models/csflow/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/csflow/torch_model.py` & `anomalib-0.5.0/src/anomalib/models/csflow/torch_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,15 +515,14 @@
         self,
         input_size: tuple[int, int],
         cross_conv_hidden_channels: int,
         n_coupling_blocks: int = 4,
         clamp: int = 3,
         num_channels: int = 3,
     ) -> None:
-
         super().__init__()
         self.input_dims = (num_channels, *input_size)
         self.clamp = clamp
         self.cross_conv_hidden_channels = cross_conv_hidden_channels
         self.feature_extractor = MultiScaleFeatureExtractor(n_scales=3, input_size=input_size)
         self.graph = CrossScaleFlow(
             input_dims=self.input_dims,
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/dfkde/config.yaml` & `anomalib-0.5.0/src/anomalib/models/dfkde/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
   path: ./results
 
 logging:
   logger: [] # options: [comet, tensorboard, wandb, csv] or combinations.
   log_graph: false # Logs the model graph to respective logger.
 
 optimization:
-  export_mode: null #options: onnx, openvino
+  export_mode: null # options: torch, onnx, openvino
 # PL Trainer Args. Don't add extra parameter here.
 trainer:
   enable_checkpointing: true
   default_root_dir: null
   gradient_clip_val: 0
   gradient_clip_algorithm: norm
   num_nodes: 1
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/dfkde/lightning_model.py` & `anomalib-0.5.0/src/anomalib/models/dfkde/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/dfkde/torch_model.py` & `anomalib-0.5.0/src/anomalib/models/dfkde/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/dfm/config.yaml` & `anomalib-0.5.0/src/anomalib/models/dfm/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
   path: ./results
 
 logging:
   logger: [] # options: [comet, tensorboard, wandb, csv] or combinations.
   log_graph: false # Logs the model graph to respective logger.
 
 optimization:
-  export_mode: null #options: onnx, openvino
+  export_mode: null # options: torch, onnx, openvino
 # PL Trainer Args. Don't add extra parameter here.
 trainer:
   enable_checkpointing: true
   default_root_dir: null
   gradient_clip_val: 0
   gradient_clip_algorithm: norm
   num_nodes: 1
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/dfm/lightning_model.py` & `anomalib-0.5.0/src/anomalib/models/dfm/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/dfm/torch_model.py` & `anomalib-0.5.0/src/anomalib/models/dfm/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/draem/config.yaml` & `anomalib-0.5.0/src/anomalib/models/draem/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
   path: ./results
 
 logging:
   logger: [] # options: [comet, tensorboard, wandb, csv] or combinations.
   log_graph: false # Logs the model graph to respective logger.
 
 optimization:
-  export_mode: null #options: onnx, openvino
+  export_mode: null # options: torch, onnx, openvino
 # PL Trainer Args. Don't add extra parameter here.
 trainer:
   enable_checkpointing: true
   default_root_dir: null
   gradient_clip_val: 0
   gradient_clip_algorithm: norm
   num_nodes: 1
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/draem/lightning_model.py` & `anomalib-0.5.0/src/anomalib/models/draem/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/draem/loss.py` & `anomalib-0.5.0/src/anomalib/models/draem/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/draem/torch_model.py` & `anomalib-0.5.0/src/anomalib/models/draem/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/fastflow/anomaly_map.py` & `anomalib-0.5.0/src/anomalib/models/fastflow/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/fastflow/config.yaml` & `anomalib-0.5.0/src/anomalib/models/fastflow/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
   path: ./results
 
 logging:
   logger: [] # options: [comet, tensorboard, wandb, csv] or combinations.
   log_graph: false # Logs the model graph to respective logger.
 
 optimization:
-  export_mode: null #options: onnx, openvino
+  export_mode: null # options: torch, onnx, openvino
 
 # PL Trainer Args. Don't add extra parameter here.
 trainer:
   enable_checkpointing: true
   default_root_dir: null
   gradient_clip_val: 0
   gradient_clip_algorithm: norm
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/fastflow/lightning_model.py` & `anomalib-0.5.0/src/anomalib/models/fastflow/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/fastflow/loss.py` & `anomalib-0.5.0/src/anomalib/models/fastflow/loss.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,10 +19,10 @@
             hidden_variables (list[Tensor]): Hidden variables from the fastflow model. f: X -> Z
             jacobians (list[Tensor]): Log of the jacobian determinants from the fastflow model.
 
         Returns:
             Tensor: Fastflow loss computed based on the hidden variables and the log of the Jacobians.
         """
         loss = torch.tensor(0.0, device=hidden_variables[0].device)  # pylint: disable=not-callable
-        for (hidden_variable, jacobian) in zip(hidden_variables, jacobians):
+        for hidden_variable, jacobian in zip(hidden_variables, jacobians):
             loss += torch.mean(0.5 * torch.sum(hidden_variable**2, dim=(1, 2, 3)) - jacobian)
         return loss
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/fastflow/torch_model.py` & `anomalib-0.5.0/src/anomalib/models/fastflow/torch_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 from __future__ import annotations
 
 from typing import Callable
 
 import timm
 import torch
 from FrEIA.framework import SequenceINN
-from FrEIA.modules import AllInOneBlock
 from timm.models.cait import Cait
 from timm.models.vision_transformer import VisionTransformer
 from torch import Tensor, nn
 
+from anomalib.models.components.flow import AllInOneBlock
 from anomalib.models.fastflow.anomaly_map import AnomalyMapGenerator
 
 
 def subnet_conv_func(kernel_size: int, hidden_ratio: float) -> Callable:
     """Subnet Convolutional Function.
 
     Callable class or function ``f``, called as ``f(channels_in, channels_out)`` and
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/ganomaly/config.yaml` & `anomalib-0.5.0/src/anomalib/models/ganomaly/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/ganomaly/lightning_model.py` & `anomalib-0.5.0/src/anomalib/models/ganomaly/lightning_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,14 @@
     """PL Lightning Module for the GANomaly Algorithm.
 
     Args:
         hparams (DictConfig | ListConfig): Model params
     """
 
     def __init__(self, hparams: DictConfig | ListConfig) -> None:
-
         super().__init__(
             batch_size=hparams.dataset.train_batch_size,
             input_size=hparams.model.input_size,
             n_features=hparams.model.n_features,
             latent_vec_size=hparams.model.latent_vec_size,
             extra_layers=hparams.model.extra_layers,
             add_final_conv_layer=hparams.model.add_final_conv,
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/ganomaly/loss.py` & `anomalib-0.5.0/src/anomalib/models/ganomaly/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/ganomaly/torch_model.py` & `anomalib-0.5.0/src/anomalib/models/ganomaly/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/padim/anomaly_map.py` & `anomalib-0.5.0/src/anomalib/models/padim/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/padim/config.yaml` & `anomalib-0.5.0/src/anomalib/models/padim/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
   path: ./results
 
 logging:
   logger: [] # options: [comet, tensorboard, wandb, csv] or combinations.
   log_graph: false # Logs the model graph to respective logger.
 
 optimization:
-  export_mode: null #options: onnx, openvino
+  export_mode: null # options: torch, onnx, openvino
 
 # PL Trainer Args. Don't add extra parameter here.
 trainer:
   enable_checkpointing: true
   default_root_dir: null
   gradient_clip_val: 0
   gradient_clip_algorithm: norm
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/padim/lightning_model.py` & `anomalib-0.5.0/src/anomalib/models/padim/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/padim/torch_model.py` & `anomalib-0.5.0/src/anomalib/models/padim/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/patchcore/anomaly_map.py` & `anomalib-0.5.0/src/anomalib/models/patchcore/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/patchcore/config.yaml` & `anomalib-0.5.0/src/anomalib/models/patchcore/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/patchcore/lightning_model.py` & `anomalib-0.5.0/src/anomalib/models/patchcore/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/patchcore/torch_model.py` & `anomalib-0.5.0/src/anomalib/models/patchcore/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/reverse_distillation/anomaly_map.py` & `anomalib-0.5.0/src/anomalib/models/reverse_distillation/anomaly_map.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,70 +7,85 @@
 #
 # Modified
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
+from enum import Enum
+
 import torch
 import torch.nn.functional as F
 from kornia.filters import gaussian_blur2d
 from omegaconf import ListConfig
 from torch import Tensor, nn
 
 
+class AnomalyMapGenerationMode(str, Enum):
+    """Type of mode when generating anomaly imape."""
+
+    ADD = "add"
+    MULTIPLY = "multiply"
+
+
 class AnomalyMapGenerator(nn.Module):
     """Generate Anomaly Heatmap.
 
     Args:
         image_size (ListConfig, tuple): Size of original image used for upscaling the anomaly map.
         sigma (int): Standard deviation of the gaussian kernel used to smooth anomaly map.
-        mode (str, optional): Operation used to generate anomaly map. Options are `add` and `multiply`.
-                Defaults to "multiply".
+        mode (AnomalyMapGenerationMode, optional): Operation used to generate anomaly map.
+        Options are `AnomalyMapGenerationMode.ADD` and `AnomalyMapGenerationMode.MULTIPLY`.
+        Defaults to "AnomalyMapGenerationMode.MULTIPLY".
 
     Raises:
         ValueError: In case modes other than multiply and add are passed.
     """
 
-    def __init__(self, image_size: ListConfig | tuple, sigma: int = 4, mode: str = "multiply") -> None:
+    def __init__(
+        self,
+        image_size: ListConfig | tuple,
+        sigma: int = 4,
+        mode: AnomalyMapGenerationMode = AnomalyMapGenerationMode.MULTIPLY,
+    ) -> None:
         super().__init__()
         self.image_size = image_size if isinstance(image_size, tuple) else tuple(image_size)
         self.sigma = sigma
         self.kernel_size = 2 * int(4.0 * sigma + 0.5) + 1
 
-        if mode not in ("add", "multiply"):
+        if mode not in (AnomalyMapGenerationMode.ADD, AnomalyMapGenerationMode.MULTIPLY):
             raise ValueError(f"Found mode {mode}. Only multiply and add are supported.")
         self.mode = mode
 
     def forward(self, student_features: list[Tensor], teacher_features: list[Tensor]) -> Tensor:
         """Computes anomaly map given encoder and decoder features.
 
         Args:
             student_features (list[Tensor]): List of encoder features
             teacher_features (list[Tensor]): List of decoder features
 
         Returns:
             Tensor: Anomaly maps of length batch.
         """
-        if self.mode == "multiply":
+        if self.mode == AnomalyMapGenerationMode.MULTIPLY:
             anomaly_map = torch.ones(
                 [student_features[0].shape[0], 1, *self.image_size], device=student_features[0].device
             )  # b c h w
-        elif self.mode == "add":
+        elif self.mode == AnomalyMapGenerationMode.ADD:
             anomaly_map = torch.zeros(
                 [student_features[0].shape[0], 1, *self.image_size], device=student_features[0].device
             )
 
         for student_feature, teacher_feature in zip(student_features, teacher_features):
             distance_map = 1 - F.cosine_similarity(student_feature, teacher_feature)
             distance_map = torch.unsqueeze(distance_map, dim=1)
             distance_map = F.interpolate(distance_map, size=self.image_size, mode="bilinear", align_corners=True)
-            if self.mode == "multiply":
+            if self.mode == AnomalyMapGenerationMode.MULTIPLY:
                 anomaly_map *= distance_map
-            elif self.mode == "add":
+            elif self.mode == AnomalyMapGenerationMode.ADD:
                 anomaly_map += distance_map
 
         anomaly_map = gaussian_blur2d(
             anomaly_map, kernel_size=(self.kernel_size, self.kernel_size), sigma=(self.sigma, self.sigma)
         )
 
         return anomaly_map
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/reverse_distillation/components/__init__.py` & `anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/reverse_distillation/components/bottleneck.py` & `anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/bottleneck.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/reverse_distillation/components/de_resnet.py` & `anomalib-0.5.0/src/anomalib/models/reverse_distillation/components/de_resnet.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/reverse_distillation/config.yaml` & `anomalib-0.5.0/src/anomalib/models/reverse_distillation/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
   path: ./results
 
 logging:
   logger: [] # options: [comet, tensorboard, wandb, csv] or combinations.
   log_graph: false # Logs the model graph to respective logger.
 
 optimization:
-  export_mode: null #options: onnx, openvino
+  export_mode: null # options: torch, onnx, openvino
 
 # PL Trainer Args. Don't add extra parameter here.
 trainer:
   enable_checkpointing: true
   default_root_dir: null
   gradient_clip_val: 0
   gradient_clip_algorithm: norm
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/reverse_distillation/lightning_model.py` & `anomalib-0.5.0/src/anomalib/models/reverse_distillation/lightning_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from omegaconf import DictConfig, ListConfig
 from pytorch_lightning.callbacks import EarlyStopping
 from pytorch_lightning.utilities.types import STEP_OUTPUT
 from torch import Tensor, optim
 
 from anomalib.models.components import AnomalyModule
 
+from .anomaly_map import AnomalyMapGenerationMode
 from .loss import ReverseDistillationLoss
 from .torch_model import ReverseDistillationModel
 
 
 class ReverseDistillation(AnomalyModule):
     """PL Lightning Module for Reverse Distillation Algorithm.
 
@@ -30,15 +31,15 @@
     """
 
     def __init__(
         self,
         input_size: tuple[int, int],
         backbone: str,
         layers: list[str],
-        anomaly_map_mode: str,
+        anomaly_map_mode: AnomalyMapGenerationMode,
         lr: float,
         beta1: float,
         beta2: float,
         pre_trained: bool = True,
     ) -> None:
         super().__init__()
         self.model = ReverseDistillationModel(
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/reverse_distillation/loss.py` & `anomalib-0.5.0/src/anomalib/models/reverse_distillation/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/reverse_distillation/torch_model.py` & `anomalib-0.5.0/src/anomalib/models/reverse_distillation/torch_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from anomalib.models.reverse_distillation.anomaly_map import AnomalyMapGenerator
 from anomalib.models.reverse_distillation.components import (
     get_bottleneck_layer,
     get_decoder,
 )
 from anomalib.pre_processing import Tiler
 
+from .anomaly_map import AnomalyMapGenerationMode
+
 
 class ReverseDistillationModel(nn.Module):
     """Reverse Distillation Model.
 
     Args:
         backbone (str): Name of the backbone used for encoder and decoder
         input_size (tuple[int, int]): Size of input image
@@ -28,15 +30,15 @@
     """
 
     def __init__(
         self,
         backbone: str,
         input_size: tuple[int, int],
         layers: list[str],
-        anomaly_map_mode: str,
+        anomaly_map_mode: AnomalyMapGenerationMode,
         pre_trained: bool = True,
     ) -> None:
         super().__init__()
         self.tiler: Tiler | None = None
 
         encoder_backbone = backbone
         self.encoder = FeatureExtractor(backbone=encoder_backbone, pre_trained=pre_trained, layers=layers)
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/rkde/config.yaml` & `anomalib-0.5.0/src/anomalib/models/rkde/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
   path: ./results
 
 logging:
   logger: [] # options: [comet, tensorboard, wandb, csv] or combinations.
   log_graph: false # Logs the model graph to respective logger.
 
 optimization:
-  export_mode: null #options: onnx, openvino
+  export_mode: null # options: torch, onnx, openvino
 # PL Trainer Args. Don't add extra parameter here.
 trainer:
   enable_checkpointing: true
   default_root_dir: null
   gradient_clip_val: 0
   gradient_clip_algorithm: norm
   num_nodes: 1
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/rkde/feature_extractor.py` & `anomalib-0.5.0/src/anomalib/models/rkde/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/rkde/lightning_model.py` & `anomalib-0.5.0/src/anomalib/models/rkde/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/rkde/region_extractor.py` & `anomalib-0.5.0/src/anomalib/models/rkde/region_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,14 @@
 
         Returns:
             list[Tensor]: Post-processed box predictions of shape (N, 4).
         """
 
         processed_boxes: list[Tensor] = []
         for boxes, scores in zip(pred_boxes, pred_scores):
-
             # remove small boxes
             keep = box_ops.remove_small_boxes(boxes, min_size=self.min_size)
             boxes, scores = boxes[keep], scores[keep]
 
             # non-maximum suppression, all boxes together
             keep = box_ops.nms(boxes, scores, self.iou_threshold)
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/rkde/torch_model.py` & `anomalib-0.5.0/src/anomalib/models/rkde/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/stfpm/anomaly_map.py` & `anomalib-0.5.0/src/anomalib/models/stfpm/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/stfpm/config.yaml` & `anomalib-0.5.0/src/anomalib/models/stfpm/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
   path: ./results
 
 logging:
   logger: [] # options: [comet, tensorboard, wandb, csv] or combinations.
   log_graph: false # Logs the model graph to respective logger.
 
 optimization:
-  export_mode: null #options: onnx, openvino
+  export_mode: null # options: torch, onnx, openvino
 # PL Trainer Args. Don't add extra parameter here.
 trainer:
   enable_checkpointing: true
   default_root_dir: null
   gradient_clip_val: 0
   gradient_clip_algorithm: norm
   num_nodes: 1
```

### Comparing `anomalib-0.4.0rc2/anomalib/models/stfpm/lightning_model.py` & `anomalib-0.5.0/src/anomalib/models/stfpm/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/stfpm/loss.py` & `anomalib-0.5.0/src/anomalib/models/stfpm/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/models/stfpm/torch_model.py` & `anomalib-0.5.0/src/anomalib/models/stfpm/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/post_processing/__init__.py` & `anomalib-0.5.0/src/anomalib/post_processing/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,20 +8,21 @@
     ThresholdMethod,
     add_anomalous_label,
     add_normal_label,
     anomaly_map_to_color_map,
     compute_mask,
     superimpose_anomaly_map,
 )
-from .visualizer import ImageResult, Visualizer
+from .visualizer import ImageResult, VisualizationMode, Visualizer
 
 __all__ = [
     "add_anomalous_label",
     "add_normal_label",
     "anomaly_map_to_color_map",
     "superimpose_anomaly_map",
     "compute_mask",
     "ImageResult",
     "NormalizationMethod",
     "Visualizer",
+    "VisualizationMode",
     "ThresholdMethod",
 ]
```

### Comparing `anomalib-0.4.0rc2/anomalib/post_processing/normalization/cdf.py` & `anomalib-0.5.0/src/anomalib/post_processing/normalization/cdf.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/post_processing/normalization/min_max.py` & `anomalib-0.5.0/src/anomalib/post_processing/normalization/min_max.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/post_processing/post_process.py` & `anomalib-0.5.0/src/anomalib/post_processing/post_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,10 +162,10 @@
         boxes (np.nparray): 2D array of shape (N, 4) where each row contains the xyxy coordinates of a bounding box.
         color (tuple[int, int, int]): Color of the drawn boxes in RGB format.
 
     Returns:
         np.ndarray: Image showing the bounding boxes drawn on top of the source image.
     """
     for box in boxes:
-        x_1, y_1, x_2, y_2 = box.astype(np.int)
+        x_1, y_1, x_2, y_2 = box.astype(int)
         image = cv2.rectangle(image, (x_1, y_1), (x_2, y_2), color=color, thickness=2)
     return image
```

### Comparing `anomalib-0.4.0rc2/anomalib/post_processing/visualizer.py` & `anomalib-0.5.0/src/anomalib/post_processing/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
+from enum import Enum
 from pathlib import Path
 from typing import Iterator
 
 import cv2
 import matplotlib.figure
 import matplotlib.pyplot as plt
 import numpy as np
@@ -57,24 +58,31 @@
             self.gt_mask *= 255
         if self.pred_boxes is not None:
             assert self.box_labels is not None, "Box labels must be provided when box locations are provided."
             self.normal_boxes = self.pred_boxes[~self.box_labels.astype(bool)]
             self.anomalous_boxes = self.pred_boxes[self.box_labels.astype(bool)]
 
 
+class VisualizationMode(str, Enum):
+    """Type of visualization mode."""
+
+    FULL = "full"
+    SIMPLE = "simple"
+
+
 class Visualizer:
     """Class that handles the logic of composing the visualizations.
 
     Args:
-        mode (str): visualization mode, either "full" or "simple"
+        mode (VisualizationMode): visualization mode, either "full" or "simple"
         task (TaskType): task type "segmentation", "detection" or "classification"
     """
 
-    def __init__(self, mode: str, task: TaskType) -> None:
-        if mode not in ("full", "simple"):
+    def __init__(self, mode: VisualizationMode, task: TaskType) -> None:
+        if mode not in (VisualizationMode.FULL, VisualizationMode.SIMPLE):
             raise ValueError(f"Unknown visualization mode: {mode}. Please choose one of ['full', 'simple']")
         self.mode = mode
         if task not in (TaskType.CLASSIFICATION, TaskType.DETECTION, TaskType.SEGMENTATION):
             raise ValueError(
                 f"Unknown task type: {mode}. Please choose one of ['classification', 'detection', 'segmentation']"
             )
         self.task = task
@@ -84,19 +92,21 @@
 
         Args:
             batch (dict): Dictionary containing the ground truth and predictions of a batch of images.
 
         Returns:
             Generator that yields a display-ready visualization for each image.
         """
-        batch_size, _num_channels, height, width = batch["image"].size()
+        batch_size = batch["image"].shape[0]
         for i in range(batch_size):
             if "image_path" in batch:
+                height, width = batch["image"].shape[-2:]
                 image = read_image(path=batch["image_path"][i], image_size=(height, width))
             elif "video_path" in batch:
+                height, width = batch["original_image"].shape[1:3]
                 image = batch["original_image"][i].squeeze().numpy()
                 image = cv2.resize(image, dsize=(width, height), interpolation=cv2.INTER_AREA)
             else:
                 raise KeyError("Batch must have either 'image_path' or 'video_path' defined.")
 
             image_result = ImageResult(
                 image=image,
@@ -116,17 +126,17 @@
 
         Args:
             image_result (ImageResult): GT and Prediction data for a single image.
 
         Returns:
             The full or simple visualization for the image, depending on the specified mode.
         """
-        if self.mode == "full":
+        if self.mode == VisualizationMode.FULL:
             return self._visualize_full(image_result)
-        if self.mode == "simple":
+        if self.mode == VisualizationMode.SIMPLE:
             return self._visualize_simple(image_result)
         raise ValueError(f"Unknown visualization mode: {self.mode}")
 
     def _visualize_full(self, image_result: ImageResult) -> np.ndarray:
         """Generate the full set of visualization for an image.
 
         The full visualization mode shows a grid with subplots that contain the original image, the GT mask (if
@@ -157,14 +167,16 @@
             if image_result.gt_mask is not None:
                 visualization.add_image(image=image_result.gt_mask, color_map="gray", title="Ground Truth")
             visualization.add_image(image_result.heat_map, "Predicted Heat Map")
             visualization.add_image(image=image_result.pred_mask, color_map="gray", title="Predicted Mask")
             visualization.add_image(image=image_result.segmentations, title="Segmentation Result")
         elif self.task == TaskType.CLASSIFICATION:
             visualization.add_image(image_result.image, title="Image")
+            if hasattr(image_result, "heat_map"):
+                visualization.add_image(image_result.heat_map, "Predicted Heat Map")
             if image_result.pred_label:
                 image_classified = add_anomalous_label(image_result.image, image_result.pred_score)
             else:
                 image_classified = add_normal_label(image_result.image, 1 - image_result.pred_score)
             visualization.add_image(image=image_classified, title="Prediction")
 
         return visualization.generate()
```

### Comparing `anomalib-0.4.0rc2/anomalib/pre_processing/pre_process.py` & `anomalib-0.5.0/src/anomalib/pre_processing/pre_process.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/pre_processing/tiler.py` & `anomalib-0.5.0/src/anomalib/pre_processing/tiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 """Image Tiler."""
 
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
+from enum import Enum
 from itertools import product
 from math import ceil
 from typing import Sequence
 
 import torch
 import torchvision.transforms as T
 from torch import Tensor
 from torch.nn import functional as F
 
 
+class ImageUpscaleMode(str, Enum):
+    """Type of mode when upscaling image."""
+
+    PADDING = "padding"
+    INTERPOLATION = "interpolation"
+
+
 class StrideSizeError(Exception):
     """StrideSizeError to raise exception when stride size is greater than the tile size."""
 
 
 def compute_new_image_size(image_size: tuple, tile_size: tuple, stride: tuple) -> tuple:
     """This function checks if image size is divisible by tile size and stride.
 
@@ -49,15 +57,15 @@
 
     resized_h = __compute_new_edge_size(image_size[0], tile_size[0], stride[0])
     resized_w = __compute_new_edge_size(image_size[1], tile_size[1], stride[1])
 
     return resized_h, resized_w
 
 
-def upscale_image(image: Tensor, size: tuple, mode: str = "padding") -> Tensor:
+def upscale_image(image: Tensor, size: tuple, mode: ImageUpscaleMode = ImageUpscaleMode.PADDING) -> Tensor:
     """Upscale image to the desired size via either padding or interpolation.
 
     Args:
         image (Tensor): Image
         size (tuple): tuple to which image is upscaled.
         mode (str, optional): Upscaling mode. Defaults to "padding".
 
@@ -75,28 +83,28 @@
     Returns:
         Tensor: Upscaled image.
     """
 
     image_h, image_w = image.shape[2:]
     resize_h, resize_w = size
 
-    if mode == "padding":
+    if mode == ImageUpscaleMode.PADDING:
         pad_h = resize_h - image_h
         pad_w = resize_w - image_w
 
         image = F.pad(image, [0, pad_w, 0, pad_h])
-    elif mode == "interpolation":
+    elif mode == ImageUpscaleMode.INTERPOLATION:
         image = F.interpolate(input=image, size=(resize_h, resize_w))
     else:
         raise ValueError(f"Unknown mode {mode}. Only padding and interpolation is available.")
 
     return image
 
 
-def downscale_image(image: Tensor, size: tuple, mode: str = "padding") -> Tensor:
+def downscale_image(image: Tensor, size: tuple, mode: ImageUpscaleMode = ImageUpscaleMode.PADDING) -> Tensor:
     """Opposite of upscaling. This image downscales image to a desired size.
 
     Args:
         image (Tensor): Input image
         size (tuple): Size to which image is down scaled.
         mode (str, optional): Downscaling mode. Defaults to "padding".
 
@@ -107,15 +115,15 @@
         >>> torch.allclose(x, y)
         True
 
     Returns:
         Tensor: Downscaled image
     """
     input_h, input_w = size
-    if mode == "padding":
+    if mode == ImageUpscaleMode.PADDING:
         image = image[:, :, :input_h, :input_w]
     else:
         image = F.interpolate(input=image, size=(input_h, input_w))
 
     return image
 
 
@@ -147,18 +155,17 @@
     """
 
     def __init__(
         self,
         tile_size: int | Sequence,
         stride: int | Sequence | None = None,
         remove_border_count: int = 0,
-        mode: str = "padding",
+        mode: ImageUpscaleMode = ImageUpscaleMode.PADDING,
         tile_count: int = 4,
     ) -> None:
-
         self.tile_size_h, self.tile_size_w = self.__validate_size_type(tile_size)
         self.tile_count = tile_count
 
         if stride is not None:
             self.stride_h, self.stride_w = self.__validate_size_type(stride)
 
         self.remove_border_count = remove_border_count
@@ -167,15 +174,15 @@
 
         if self.stride_h > self.tile_size_h or self.stride_w > self.tile_size_w:
             raise StrideSizeError(
                 "Larger stride size than kernel size produces unreliable tiling results. "
                 "Please ensure stride size is less than or equal than tiling size."
             )
 
-        if self.mode not in ("padding", "interpolation"):
+        if self.mode not in (ImageUpscaleMode.PADDING, ImageUpscaleMode.INTERPOLATION):
             raise ValueError(f"Unknown tiling mode {self.mode}. Available modes are padding and interpolation")
 
         self.batch_size: int
         self.num_channels: int
 
         self.input_h: int
         self.input_w: int
```

### Comparing `anomalib-0.4.0rc2/anomalib/pre_processing/transforms/custom.py` & `anomalib-0.5.0/src/anomalib/pre_processing/transforms/custom.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/__init__.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     callbacks: list[Callback] = []
 
     monitor_metric = None if "early_stopping" not in config.model.keys() else config.model.early_stopping.metric
     monitor_mode = "max" if "early_stopping" not in config.model.keys() else config.model.early_stopping.mode
 
     checkpoint = ModelCheckpoint(
-        dirpath=os.path.join(config.project.path, "weights"),
+        dirpath=os.path.join(config.project.path, "weights", "lightning"),
         filename="model",
         monitor=monitor_metric,
         mode=monitor_mode,
         auto_insert_metric_name=False,
     )
 
     callbacks.extend([checkpoint, TimerCallback()])
```

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/cdf_normalization.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/cdf_normalization.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/export.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/export.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,17 +36,18 @@
 
     def on_train_end(self, trainer: pl.Trainer, pl_module: AnomalyModule) -> None:
         """Call when the train ends.
 
         Converts the model to ``onnx`` format and then calls OpenVINO's model optimizer to get the
         ``.xml`` and ``.bin`` IR files.
         """
-        del trainer  # `trainer` variable is not used.
-
         logger.info("Exporting the model")
         Path(self.dirpath).mkdir(parents=True, exist_ok=True)
+
         export(
-            model=pl_module,
+            task=trainer.datamodule.test_data.task,
             input_size=self.input_size,
+            transform=trainer.datamodule.test_data.transform.to_dict(),
+            model=pl_module,
             export_root=self.dirpath,
             export_mode=self.export_mode,
         )
```

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/graph.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/graph.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/metrics_configuration.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/metrics_configuration.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/min_max_normalization.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/min_max_normalization.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/model_loader.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/model_loader.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/nncf/callback.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/nncf/callback.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/nncf/utils.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/nncf/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         Returns:
             None
         """
         return None
 
 
 def wrap_nncf_model(
-    model: nn.Module, config: dict, dataloader: DataLoader = None, init_state_dict: dict = None
+    model: nn.Module, config: dict, dataloader: DataLoader, init_state_dict: dict
 ) -> tuple[CompressionAlgorithmController, NNCFNetwork]:
     """Wrap model by NNCF.
 
     :param model: Anomalib model.
     :param config: NNCF config.
     :param dataloader: Dataloader for initialization of NNCF model.
     :param init_state_dict: Opti
```

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/post_processing_configuration.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/post_processing_configuration.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/tiler_configuration.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/tiler_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 
 from typing import Sequence
 
 import pytorch_lightning as pl
 from pytorch_lightning.callbacks import Callback
 
 from anomalib.models.components import AnomalyModule
-from anomalib.pre_processing.tiler import Tiler
+from anomalib.pre_processing.tiler import ImageUpscaleMode, Tiler
 
 __all__ = ["TilerConfigurationCallback"]
 
 
 class TilerConfigurationCallback(Callback):
     """Tiler Configuration Callback."""
 
     def __init__(
         self,
         enable: bool = False,
         tile_size: int | Sequence = 256,
         stride: int | Sequence | None = None,
         remove_border_count: int = 0,
-        mode: str = "padding",
+        mode: ImageUpscaleMode = ImageUpscaleMode.PADDING,
         tile_count: int = 4,
     ) -> None:
         """Sets tiling configuration from the command line.
 
         Args:
             enable (bool): Boolean to enable tiling operation.
                 Defaults to False.
```

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/timer.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/timer.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/visualizer/visualizer_base.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/visualizer_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 
 import numpy as np
 import pytorch_lightning as pl
 from pytorch_lightning import Callback
 
 from anomalib.data import TaskType
 from anomalib.models.components import AnomalyModule
-from anomalib.post_processing import Visualizer
+from anomalib.post_processing import VisualizationMode, Visualizer
 from anomalib.utils.loggers import AnomalibWandbLogger
 from anomalib.utils.loggers.base import ImageLoggerBase
 
 
 class BaseVisualizerCallback(Callback):
     """Callback that visualizes the results of a model.
 
     To save the images to the filesystem, add the 'local' keyword to the `project.log_images_to` parameter in the
     config.yaml file.
     """
 
     def __init__(
         self,
         task: TaskType,
-        mode: str,
+        mode: VisualizationMode,
         image_save_path: str,
         inputs_are_normalized: bool = True,
         show_images: bool = False,
         log_images: bool = True,
         save_images: bool = True,
     ) -> None:
         """Visualizer callback."""
```

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/visualizer/visualizer_image.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/visualizer_image.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/callbacks/visualizer/visualizer_metric.py` & `anomalib-0.5.0/src/anomalib/utils/callbacks/visualizer/visualizer_metric.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/cli/cli.py` & `anomalib-0.5.0/src/anomalib/utils/cli/cli.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/cv/connected_components.py` & `anomalib-0.5.0/src/anomalib/utils/cv/connected_components.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/hpo/config.py` & `anomalib-0.5.0/src/anomalib/utils/hpo/config.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/hpo/runners.py` & `anomalib-0.5.0/src/anomalib/utils/hpo/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Sweep Backends."""
 
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
+import gc
+
 import pytorch_lightning as pl
+import torch
+import wandb
 from comet_ml import Optimizer
 from omegaconf import DictConfig, ListConfig, OmegaConf
 from pytorch_lightning.loggers import CometLogger, WandbLogger
 
-import wandb
 from anomalib.config import update_input_size_config
 from anomalib.data import get_datamodule
 from anomalib.models import get_model
 from anomalib.utils.sweep import (
     flatten_sweep_params,
     get_sweep_callbacks,
     set_in_nested_config,
@@ -73,14 +76,18 @@
 
         # Disable saving checkpoints as all checkpoints from the sweep will get uploaded
         config.trainer.enable_checkpointing = False
 
         trainer = pl.Trainer(**config.trainer, logger=wandb_logger, callbacks=callbacks)
         trainer.fit(model, datamodule=datamodule)
 
+        del model
+        gc.collect()
+        torch.cuda.empty_cache()
+
 
 class CometSweep:
     """comet sweep.
 
     Args:
         config (DictConfig): Original model configuration.
         sweep_config (DictConfig): Sweep configuration.
```

### Comparing `anomalib-0.4.0rc2/anomalib/utils/loggers/__init__.py` & `anomalib-0.5.0/src/anomalib/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/loggers/base.py` & `anomalib-0.5.0/src/anomalib/utils/loggers/base.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/loggers/comet.py` & `anomalib-0.5.0/src/anomalib/utils/loggers/comet.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/loggers/tensorboard.py` & `anomalib-0.5.0/src/anomalib/utils/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/loggers/wandb.py` & `anomalib-0.5.0/src/anomalib/utils/loggers/wandb.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/metrics/__init__.py` & `anomalib-0.5.0/src/anomalib/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/metrics/anomaly_score_distribution.py` & `anomalib-0.5.0/src/anomalib/utils/metrics/anomaly_score_distribution.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/metrics/anomaly_score_threshold.py` & `anomalib-0.5.0/src/anomalib/utils/metrics/anomaly_score_threshold.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/metrics/aupr.py` & `anomalib-0.5.0/src/anomalib/utils/metrics/aupr.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 
 from __future__ import annotations
 
-import torch
 from matplotlib.figure import Figure
 from torch import Tensor
 from torchmetrics import PrecisionRecallCurve
 from torchmetrics.functional import auc
 from torchmetrics.utilities.data import dim_zero_cat
 
 from .plotting_utils import plot_figure
@@ -25,18 +24,15 @@
         Returns:
             Value of the AUPR metric
         """
         prec: Tensor
         rec: Tensor
 
         prec, rec = self._compute()
-        # TODO: use stable sort after upgrading to pytorch 1.9.x (https://github.com/openvinotoolkit/anomalib/issues/92)
-        if not (torch.all(prec.diff() <= 0) or torch.all(prec.diff() >= 0)):
-            return auc(rec, prec, reorder=True)  # only reorder if rec is not increasing or decreasing
-        return auc(rec, prec)
+        return auc(rec, prec, reorder=True)
 
     def update(self, preds: Tensor, target: Tensor) -> None:  # type: ignore
         """Update state with new values.
 
         Need to flatten new values as PrecicionRecallCurve expects them in this format for binary classification.
 
         Args:
```

### Comparing `anomalib-0.4.0rc2/anomalib/utils/metrics/aupro.py` & `anomalib-0.5.0/src/anomalib/utils/metrics/aupro.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     target: list[Tensor]
 
     def __init__(
         self,
         compute_on_step: bool = True,
         dist_sync_on_step: bool = False,
         process_group: Any | None = None,
-        dist_sync_fn: Callable = None,
+        dist_sync_fn: Callable | None = None,
         fpr_limit: float = 0.3,
     ) -> None:
         super().__init__(
             compute_on_step=compute_on_step,
             dist_sync_on_step=dist_sync_on_step,
             process_group=process_group,
             dist_sync_fn=dist_sync_fn,
@@ -56,46 +56,50 @@
         Args:
             preds (Tensor): predictions of the model
             target (Tensor): ground truth targets
         """
         self.target.append(target)
         self.preds.append(preds)
 
-    def _compute(self) -> tuple[Tensor, Tensor]:
-        """Compute the pro/fpr value-pairs until the fpr specified by self.fpr_limit.
-
-        It leverages the fact that the overlap corresponds to the tpr, and thus computes the overall
-        PRO curve by aggregating per-region tpr/fpr values produced by ROC-construction.
+    def perform_cca(self) -> Tensor:
+        """Perform the Connected Component Analysis on the self.target tensor.
 
         Raises:
             ValueError: ValueError is raised if self.target doesn't conform with requirements imposed by kornia for
                         connected component analysis.
 
         Returns:
-            tuple[Tensor, Tensor]: tuple containing final fpr and tpr values.
+            Tensor: Components labeled from 0 to N.
         """
         target = dim_zero_cat(self.target)
-        preds = dim_zero_cat(self.preds)
 
         # check and prepare target for labeling via kornia
         if target.min() < 0 or target.max() > 1:
             raise ValueError(
                 f"kornia.contrib.connected_components expects input to lie in the interval [0, 1], but found "
                 f"interval was [{target.min()}, {target.max()}]."
             )
         target = target.unsqueeze(1)  # kornia expects N1HW format
         target = target.type(torch.float)  # kornia expects FloatTensor
         if target.is_cuda:
             cca = connected_components_gpu(target)
         else:
             cca = connected_components_cpu(target)
 
-        preds = preds.flatten()
-        cca = cca.flatten()
-        target = target.flatten()
+        return cca
+
+    def compute_pro(self, cca: Tensor, target: Tensor, preds: Tensor) -> tuple[Tensor, Tensor]:
+        """Compute the pro/fpr value-pairs until the fpr specified by self.fpr_limit.
+
+        It leverages the fact that the overlap corresponds to the tpr, and thus computes the overall
+        PRO curve by aggregating per-region tpr/fpr values produced by ROC-construction.
+
+        Returns:
+            tuple[Tensor, Tensor]: tuple containing final fpr and tpr values.
+        """
 
         # compute the global fpr-size
         fpr: Tensor = roc(preds, target)[0]  # only need fpr
         output_size = torch.where(fpr <= self.fpr_limit)[0].size(0)
 
         # compute the PRO curve by aggregating per-region tpr/fpr curves/values.
         tpr = torch.zeros(output_size, device=preds.device, dtype=torch.float)
@@ -150,23 +154,38 @@
             fpr += _fpr
 
         # Actually perform the averaging
         tpr /= labels.size(0)
         fpr /= labels.size(0)
         return fpr, tpr
 
+    def _compute(self) -> tuple[Tensor, Tensor]:
+        """Compute the PRO curve.
+
+        Perform the Connected Component Analysis first then compute the PRO curve.
+
+        Returns:
+            tuple[Tensor, Tensor]: tuple containing final fpr and tpr values.
+        """
+
+        cca = self.perform_cca().flatten()
+        target = dim_zero_cat(self.target).flatten()
+        preds = dim_zero_cat(self.preds).flatten()
+
+        return self.compute_pro(cca=cca, target=target, preds=preds)
+
     def compute(self) -> Tensor:
         """Fist compute PRO curve, then compute and scale area under the curve.
 
         Returns:
             Tensor: Value of the AUPRO metric
         """
         fpr, tpr = self._compute()
 
-        aupro = auc(fpr, tpr)
+        aupro = auc(fpr, tpr, reorder=True)
         aupro = aupro / fpr[-1]  # normalize the area
 
         return aupro
 
     def generate_figure(self) -> tuple[Figure, str]:
         """Generate a figure containing the PRO curve and the AUPRO.
```

### Comparing `anomalib-0.4.0rc2/anomalib/utils/metrics/auroc.py` & `anomalib-0.5.0/src/anomalib/utils/metrics/auroc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Implementation of AUROC metric based on TorchMetrics."""
 
 # Copyright (C) 2022 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
-import torch
 from matplotlib.figure import Figure
 from torch import Tensor
 from torchmetrics import ROC
 from torchmetrics.functional import auc
 
 from .plotting_utils import plot_figure
 
@@ -23,18 +22,15 @@
         Returns:
             Tensor: Value of the AUROC metric
         """
         tpr: Tensor
         fpr: Tensor
 
         fpr, tpr = self._compute()
-        # TODO: use stable sort after upgrading to pytorch 1.9.x (https://github.com/openvinotoolkit/anomalib/issues/92)
-        if not (torch.all(fpr.diff() <= 0) or torch.all(fpr.diff() >= 0)):
-            return auc(fpr, tpr, reorder=True)  # only reorder if fpr is not increasing or decreasing
-        return auc(fpr, tpr)
+        return auc(fpr, tpr, reorder=True)
 
     def update(self, preds: Tensor, target: Tensor) -> None:  # type: ignore
         """Update state with new values.
 
         Need to flatten new values as ROC expects them in this format for binary classification.
 
         Args:
```

### Comparing `anomalib-0.4.0rc2/anomalib/utils/metrics/collection.py` & `anomalib-0.5.0/src/anomalib/utils/metrics/collection.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/metrics/min_max.py` & `anomalib-0.5.0/src/anomalib/utils/metrics/min_max.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/metrics/optimal_f1.py` & `anomalib-0.5.0/src/anomalib/utils/metrics/optimal_f1.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/metrics/plotting_utils.py` & `anomalib-0.5.0/src/anomalib/utils/metrics/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/metrics/pro.py` & `anomalib-0.5.0/src/anomalib/utils/metrics/pro.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/sweep/config.py` & `anomalib-0.5.0/src/anomalib/utils/sweep/config.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/sweep/helpers/callbacks.py` & `anomalib-0.5.0/src/anomalib/utils/sweep/helpers/callbacks.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.4.0rc2/anomalib/utils/sweep/helpers/inference.py` & `anomalib-0.5.0/src/anomalib/utils/sweep/helpers/inference.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,65 +5,67 @@
 
 from __future__ import annotations
 
 import time
 from pathlib import Path
 
 import torch
-from omegaconf import DictConfig, ListConfig
-from torch.utils.data import DataLoader
+from torch.utils.data import Dataset
 
 from anomalib.deploy import OpenVINOInferencer, TorchInferencer
-from anomalib.models.components import AnomalyModule
 
 
-def get_torch_throughput(config: DictConfig | ListConfig, model: AnomalyModule, test_dataset: DataLoader) -> float:
+def get_torch_throughput(model_path: str | Path, test_dataset: Dataset, device: str) -> float:
     """Tests the model on dummy data. Images are passed sequentially to make the comparision with OpenVINO model fair.
 
     Args:
-        config (DictConfig | ListConfig): Model config.
-        model (Path): Model on which inference is called.
-        test_dataset (DataLoader): The test dataset used as a reference for the mock dataset.
+        model_path (str, Path): Path to folder containing the Torch models.
+        test_dataset (Dataset): The test dataset used as a reference for the mock dataset.
+        device (str): Device to use for inference. Options are auto, cpu, gpu, cuda.
 
     Returns:
         float: Inference throughput
     """
+    model_path = Path(model_path)
     torch.set_grad_enabled(False)
-    model.eval()
 
-    device = config.trainer.accelerator
     if device == "gpu":
         device = "cuda"
 
-    inferencer = TorchInferencer(config, model.to(device), device=device)
+    inferencer = TorchInferencer(
+        path=model_path / "weights" / "torch" / "model.pt",
+        device=device,
+    )
     start_time = time.time()
     for image_path in test_dataset.samples.image_path:
         inferencer.predict(image_path)
 
     # get throughput
     inference_time = time.time() - start_time
     throughput = len(test_dataset) / inference_time
 
     torch.set_grad_enabled(True)
     return throughput
 
 
-def get_openvino_throughput(config: DictConfig | ListConfig, model_path: Path, test_dataset: DataLoader) -> float:
+def get_openvino_throughput(model_path: str | Path, test_dataset: Dataset) -> float:
     """Runs the generated OpenVINO model on a dummy dataset to get throughput.
 
     Args:
-        config (DictConfig | ListConfig): Model config.
-        model_path (Path): Path to folder containing the OpenVINO models. It then searches `model.xml` in the folder.
-        test_dataset (DataLoader): The test dataset used as a reference for the mock dataset.
+        model_path (str, Path): Path to folder containing the OpenVINO models. It then searches `model.xml` in folder.
+        test_dataset (Dataset): The test dataset used as a reference for the mock dataset.
 
     Returns:
         float: Inference throughput
     """
+    model_path = Path(model_path)
+
     inferencer = OpenVINOInferencer(
-        config, model_path / "openvino" / "model.xml", model_path / "openvino" / "meta_data.json"
+        path=model_path / "weights" / "openvino" / "model.xml",
+        metadata_path=model_path / "weights" / "openvino" / "metadata.json",
     )
     start_time = time.time()
     for image_path in test_dataset.samples.image_path:
         inferencer.predict(image_path)
 
     # get throughput
     inference_time = time.time() - start_time
```

### Comparing `anomalib-0.4.0rc2/anomalib.egg-info/PKG-INFO` & `anomalib-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: anomalib
-Version: 0.4.0rc2
-Summary: anomalib - Anomaly Detection Library
-Home-page: 
-Author: Intel OpenVINO
-Author-email: help@openvino.intel.com
-License: Copyright (c) Intel - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the "License")See LICENSE file for more details.
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: extra
-Provides-Extra: full
-Provides-Extra: openvino
-License-File: LICENSE
-
 <div align="center">
 
 <img src="https://raw.githubusercontent.com/openvinotoolkit/anomalib/main/docs/source/images/logos/anomalib-wide-blue.png" width="600px">
 
 **A library for benchmarking, developing and deploying deep learning anomaly detection algorithms**
 
 ---
@@ -55,23 +40,19 @@
 - All models can be exported to [**OpenVINO**](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) Intermediate Representation (IR) for accelerated inference on intel hardware.
 - A set of [inference tools](#inference) for quick and easy deployment of the standard or custom anomaly detection models.
 
 ---
 
 # Getting Started
 
-To get an overview of all the devices where `anomalib` as been tested thoroughly, look at the [Supported Hardware](https://openvinotoolkit.github.io/anomalib/#supported-hardware) section in the documentation.
+Following is a guide on how to get started with `anomalib`. For more details, look at the [Documentation](https://openvinotoolkit.github.io/anomalib).
 
 ## Jupyter Notebooks
 
-For getting started with a Jupyter Notebook, please refer to the [Notebooks](./notebooks) folder of this repository. Additionally, you can refer to a few created by the community:
-
-<a href="https://colab.research.google.com/drive/1K4a4z2iZGBNhWdmt9Aqdld7kTAxBfAmi?usp=sharing" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> by [@bth5](https://github.com/bth5)
-
-<a target="_blank" href="https://www.kaggle.com/code/ipythonx/mvtec-ad-anomaly-detection-with-anomalib-library"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" /></a> by [@innat](https://github.com/innat)
+For getting started with a Jupyter Notebook, please refer to the [Notebooks](notebooks) folder of this repository. Additionally, you can refer to a few created by the community:
 
 ## PyPI Install
 
 You can get started with `anomalib` by just using pip.
 
 ```bash
 pip install anomalib
@@ -87,55 +68,55 @@
 git clone https://github.com/openvinotoolkit/anomalib.git
 cd anomalib
 pip install -e .
 ```
 
 # Training
 
-By default [`python tools/train.py`](https://github.com/openvinotoolkit/anomalib/blob/main/tools/train.py)
+By default [`python tools/train.py`](tools/train.py)
 runs [PADIM](https://arxiv.org/abs/2011.08785) model on `leather` category from the [MVTec AD](https://www.mvtec.com/company/research/datasets/mvtec-ad) [(CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) dataset.
 
 ```bash
 python tools/train.py    # Train PADIM on MVTec AD leather
 ```
 
 Training a model on a specific dataset and category requires further configuration. Each model has its own configuration
-file, [`config.yaml`](https://github.com/openvinotoolkit/anomalib/blob/main/configs/model/padim.yaml)
+file, [`config.yaml`](src/anomalib/models/padim/config.yaml)
 , which contains data, model and training configurable parameters. To train a specific model on a specific dataset and
 category, the config file is to be provided:
 
 ```bash
 python tools/train.py --config <path/to/model/config.yaml>
 ```
 
-For example, to train [PADIM](anomalib/models/padim) you can use
+For example, to train [PADIM](src/anomalib/models/padim) you can use
 
 ```bash
-python tools/train.py --config anomalib/models/padim/config.yaml
+python tools/train.py --config src/anomalib/models/padim/config.yaml
 ```
 
 Alternatively, a model name could also be provided as an argument, where the scripts automatically finds the corresponding config file.
 
 ```bash
 python tools/train.py --model padim
 ```
 
 where the currently available models are:
 
-- [CFA](anomalib/models/cfa)
-- [CFlow](anomalib/models/cflow)
-- [DFKDE](anomalib/models/dfkde)
-- [DFM](anomalib/models/dfm)
-- [DRAEM](anomalib/models/draem)
-- [FastFlow](anomalib/models/fastflow)
-- [GANomaly](anomalib/models/ganomaly)
-- [PADIM](anomalib/models/padim)
-- [PatchCore](anomalib/models/patchcore)
-- [Reverse Distillation](anomalib/models/reverse_distillation)
-- [STFPM](anomalib/models/stfpm)
+- [CFA](src/anomalib/models/cfa)
+- [CFlow](src/anomalib/models/cflow)
+- [DFKDE](src/anomalib/models/dfkde)
+- [DFM](src/anomalib/models/dfm)
+- [DRAEM](src/anomalib/models/draem)
+- [FastFlow](src/anomalib/models/fastflow)
+- [GANomaly](src/anomalib/models/ganomaly)
+- [PADIM](src/anomalib/models/padim)
+- [PatchCore](src/anomalib/models/patchcore)
+- [Reverse Distillation](src/anomalib/models/reverse_distillation)
+- [STFPM](src/anomalib/models/stfpm)
 
 ## Feature extraction & (pre-trained) backbones
 
 The pre-trained backbones come from [PyTorch Image Models (timm)](https://github.com/rwightman/pytorch-image-models), which are wrapped by `FeatureExtractor`.
 
 For more information, please check our documentation or the [section about feature extraction in "Getting Started with PyTorch Image Models (timm): A Practitioner’s Guide"](https://towardsdatascience.com/getting-started-with-pytorch-image-models-timm-a-practitioners-guide-4e77b4bf9055#b83b:~:text=ready%20to%20train!-,Feature%20Extraction,-timm%20models%20also>).
 
@@ -197,41 +178,39 @@
 python tools/inference/lightning_inference.py -h
 ```
 
 As a quick example:
 
 ```bash
 python tools/inference/lightning_inference.py \
-    --config anomalib/models/padim/config.yaml \
-    --weights results/padim/mvtec/bottle/weights/model.ckpt \
+    --config src/anomalib/models/padim/config.yaml \
+    --weights results/padim/mvtec/bottle/run/weights/model.ckpt \
     --input datasets/MVTec/bottle/test/broken_large/000.png \
     --output results/padim/mvtec/bottle/images
 ```
 
 Example OpenVINO Inference:
 
 ```bash
 python tools/inference/openvino_inference.py \
-    --config anomalib/models/padim/config.yaml \
-    --weights results/padim/mvtec/bottle/openvino/openvino_model.bin \
-    --meta_data results/padim/mvtec/bottle/openvino/meta_data.json \
+    --weights results/padim/mvtec/bottle/run/openvino/model.bin \
+    --metadata results/padim/mvtec/bottle/run/openvino/metadata.json \
     --input datasets/MVTec/bottle/test/broken_large/000.png \
     --output results/padim/mvtec/bottle/images
 ```
 
-> Ensure that you provide path to `meta_data.json` if you want the normalization to be applied correctly.
+> Ensure that you provide path to `metadata.json` if you want the normalization to be applied correctly.
 
-You can also use Gradio Inference to interact with the trained models using a UI. Refer to our [guide](https://openvinotoolkit.github.io/anomalib/guides/inference.html#gradio-inference) for more details.
+You can also use Gradio Inference to interact with the trained models using a UI. Refer to our [guide](https://openvinotoolkit.github.io/anomalib/tutorials/inference.html#gradio-inference) for more details.
 
 A quick example:
 
 ```bash
 python tools/inference/gradio_inference.py \
-        --config ./anomalib/models/padim/config.yaml \
-        --weights ./results/padim/mvtec/bottle/weights/model.ckpt
+        --weights results/padim/mvtec/bottle/run/weights/model.ckpt
 ```
 
 ## Exporting Model to ONNX or OpenVINO IR
 
 It is possible to export your model to ONNX or OpenVINO IR
 
 If you want to export your PyTorch model to an OpenVINO model, ensure that `export_mode` is set to `"openvino"` in the respective model `config.yaml`.
@@ -247,26 +226,26 @@
 
 ```bash
 python tools/hpo/sweep.py \
     --model padim --model_config ./path_to_config.yaml \
     --sweep_config tools/hpo/sweep.yaml
 ```
 
-For more details refer the [HPO Documentation](https://openvinotoolkit.github.io/anomalib/guides/hyperparameter_optimization.html)
+For more details refer the [HPO Documentation](https://openvinotoolkit.github.io/anomalib/tutorials/hyperparameter_optimization.html)
 
 # Benchmarking
 
 To gather benchmarking data such as throughput across categories, use the following command:
 
 ```bash
 python tools/benchmarking/benchmark.py \
     --config <relative/absolute path>/<paramfile>.yaml
 ```
 
-Refer to the [Benchmarking Documentation](https://openvinotoolkit.github.io/anomalib/guides/benchmarking.html) for more details.
+Refer to the [Benchmarking Documentation](https://openvinotoolkit.github.io/anomalib/tutorials/benchmarking.html) for more details.
 
 # Experiment Management
 
 Anomablib is integrated with various libraries for experiment tracking such as Comet, tensorboard, and wandb through [pytorch lighting loggers](https://pytorch-lightning.readthedocs.io/en/stable/extensions/logging.html).
 
 Below is an example of how to enable logging for hyper-parameters, metrics, model graphs, and predictions on images in the test data-set
 
@@ -276,15 +255,15 @@
   mode: full # options: ["full", "simple"]
 
  logging:
   logger: [comet, tensorboard, wandb]
   log_graph: True
 ```
 
-For more information, refer to the [Logging Documentation](https://openvinotoolkit.github.io/anomalib/guides/logging.html)
+For more information, refer to the [Logging Documentation](https://openvinotoolkit.github.io/anomalib/tutorials/logging.html)
 
 Note: Set your API Key for [Comet.ml](https://www.comet.com/signup?utm_source=anomalib&utm_medium=referral) via `comet_ml.init()` in interactive python or simply run `export COMET_API_KEY=<Your API Key>`
 
 # Community Projects
 
 ## 1. Web-based Pipeline for Training and Inference
 
@@ -371,7 +350,17 @@
               Utku Genc},
       year={2022},
       eprint={2202.08341},
       archivePrefix={arXiv},
       primaryClass={cs.CV}
 }
 ```
+
+# Contributing
+
+For those who would like to contribute to the library, see [CONTRIBUTING.md](CONTRIBUTING.md) for details.
+
+Thank you to all of the people who have already made a contribution - we appreciate your support!
+
+<a href="https://github.com/openvinotoolkit/anomalib/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=openvinotoolkit/anomalib" />
+</a>
```

### Comparing `anomalib-0.4.0rc2/anomalib.egg-info/SOURCES.txt` & `anomalib-0.5.0/src/anomalib.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,264 +1,223 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
-anomalib/__init__.py
-anomalib.egg-info/PKG-INFO
-anomalib.egg-info/SOURCES.txt
-anomalib.egg-info/dependency_links.txt
-anomalib.egg-info/entry_points.txt
-anomalib.egg-info/requires.txt
-anomalib.egg-info/top_level.txt
-anomalib/config/__init__.py
-anomalib/config/config.py
-anomalib/data/__init__.py
-anomalib/data/avenue.py
-anomalib/data/btech.py
-anomalib/data/folder.py
-anomalib/data/inference.py
-anomalib/data/mvtec.py
-anomalib/data/shanghaitech.py
-anomalib/data/synthetic.py
-anomalib/data/task_type.py
-anomalib/data/ucsd_ped.py
-anomalib/data/visa.py
-anomalib/data/base/__init__.py
-anomalib/data/base/datamodule.py
-anomalib/data/base/dataset.py
-anomalib/data/base/video.py
-anomalib/data/utils/__init__.py
-anomalib/data/utils/augmenter.py
-anomalib/data/utils/boxes.py
-anomalib/data/utils/download.py
-anomalib/data/utils/image.py
-anomalib/data/utils/split.py
-anomalib/data/utils/transform.py
-anomalib/data/utils/video.py
-anomalib/data/utils/generators/__init__.py
-anomalib/data/utils/generators/perlin.py
-anomalib/deploy/__init__.py
-anomalib/deploy/export.py
-anomalib/deploy/inferencers/__init__.py
-anomalib/deploy/inferencers/base_inferencer.py
-anomalib/deploy/inferencers/openvino_inferencer.py
-anomalib/deploy/inferencers/torch_inferencer.py
-anomalib/models/__init__.py
-anomalib/models/cfa/__init__.py
-anomalib/models/cfa/anomaly_map.py
-anomalib/models/cfa/config.yaml
-anomalib/models/cfa/lightning_model.py
-anomalib/models/cfa/loss.py
-anomalib/models/cfa/torch_model.py
-anomalib/models/cflow/__init__.py
-anomalib/models/cflow/anomaly_map.py
-anomalib/models/cflow/config.yaml
-anomalib/models/cflow/lightning_model.py
-anomalib/models/cflow/torch_model.py
-anomalib/models/cflow/utils.py
-anomalib/models/components/__init__.py
-anomalib/models/components/base/__init__.py
-anomalib/models/components/base/anomaly_module.py
-anomalib/models/components/base/dynamic_module.py
-anomalib/models/components/classification/__init__.py
-anomalib/models/components/classification/kde_classifier.py
-anomalib/models/components/dimensionality_reduction/__init__.py
-anomalib/models/components/dimensionality_reduction/pca.py
-anomalib/models/components/dimensionality_reduction/random_projection.py
-anomalib/models/components/feature_extractors/__init__.py
-anomalib/models/components/feature_extractors/timm.py
-anomalib/models/components/feature_extractors/torchfx.py
-anomalib/models/components/feature_extractors/utils.py
-anomalib/models/components/filters/__init__.py
-anomalib/models/components/filters/blur.py
-anomalib/models/components/layers/__init__.py
-anomalib/models/components/layers/sspcab.py
-anomalib/models/components/sampling/__init__.py
-anomalib/models/components/sampling/k_center_greedy.py
-anomalib/models/components/stats/__init__.py
-anomalib/models/components/stats/kde.py
-anomalib/models/components/stats/multi_variate_gaussian.py
-anomalib/models/csflow/__init__.py
-anomalib/models/csflow/anomaly_map.py
-anomalib/models/csflow/config.yaml
-anomalib/models/csflow/lightning_model.py
-anomalib/models/csflow/loss.py
-anomalib/models/csflow/torch_model.py
-anomalib/models/dfkde/__init__.py
-anomalib/models/dfkde/config.yaml
-anomalib/models/dfkde/lightning_model.py
-anomalib/models/dfkde/torch_model.py
-anomalib/models/dfm/__init__.py
-anomalib/models/dfm/config.yaml
-anomalib/models/dfm/lightning_model.py
-anomalib/models/dfm/torch_model.py
-anomalib/models/draem/__init__.py
-anomalib/models/draem/config.yaml
-anomalib/models/draem/lightning_model.py
-anomalib/models/draem/loss.py
-anomalib/models/draem/torch_model.py
-anomalib/models/fastflow/__init__.py
-anomalib/models/fastflow/anomaly_map.py
-anomalib/models/fastflow/config.yaml
-anomalib/models/fastflow/lightning_model.py
-anomalib/models/fastflow/loss.py
-anomalib/models/fastflow/torch_model.py
-anomalib/models/ganomaly/__init__.py
-anomalib/models/ganomaly/config.yaml
-anomalib/models/ganomaly/lightning_model.py
-anomalib/models/ganomaly/loss.py
-anomalib/models/ganomaly/torch_model.py
-anomalib/models/padim/__init__.py
-anomalib/models/padim/anomaly_map.py
-anomalib/models/padim/config.yaml
-anomalib/models/padim/lightning_model.py
-anomalib/models/padim/torch_model.py
-anomalib/models/patchcore/__init__.py
-anomalib/models/patchcore/anomaly_map.py
-anomalib/models/patchcore/config.yaml
-anomalib/models/patchcore/lightning_model.py
-anomalib/models/patchcore/torch_model.py
-anomalib/models/reverse_distillation/__init__.py
-anomalib/models/reverse_distillation/anomaly_map.py
-anomalib/models/reverse_distillation/config.yaml
-anomalib/models/reverse_distillation/lightning_model.py
-anomalib/models/reverse_distillation/loss.py
-anomalib/models/reverse_distillation/torch_model.py
-anomalib/models/reverse_distillation/components/__init__.py
-anomalib/models/reverse_distillation/components/bottleneck.py
-anomalib/models/reverse_distillation/components/de_resnet.py
-anomalib/models/rkde/__init__.py
-anomalib/models/rkde/config.yaml
-anomalib/models/rkde/feature_extractor.py
-anomalib/models/rkde/lightning_model.py
-anomalib/models/rkde/region_extractor.py
-anomalib/models/rkde/torch_model.py
-anomalib/models/stfpm/__init__.py
-anomalib/models/stfpm/anomaly_map.py
-anomalib/models/stfpm/config.yaml
-anomalib/models/stfpm/lightning_model.py
-anomalib/models/stfpm/loss.py
-anomalib/models/stfpm/torch_model.py
-anomalib/post_processing/__init__.py
-anomalib/post_processing/post_process.py
-anomalib/post_processing/visualizer.py
-anomalib/post_processing/normalization/__init__.py
-anomalib/post_processing/normalization/cdf.py
-anomalib/post_processing/normalization/min_max.py
-anomalib/pre_processing/__init__.py
-anomalib/pre_processing/pre_process.py
-anomalib/pre_processing/tiler.py
-anomalib/pre_processing/transforms/__init__.py
-anomalib/pre_processing/transforms/custom.py
-anomalib/utils/__init__.py
-anomalib/utils/callbacks/__init__.py
-anomalib/utils/callbacks/cdf_normalization.py
-anomalib/utils/callbacks/export.py
-anomalib/utils/callbacks/graph.py
-anomalib/utils/callbacks/metrics_configuration.py
-anomalib/utils/callbacks/min_max_normalization.py
-anomalib/utils/callbacks/model_loader.py
-anomalib/utils/callbacks/post_processing_configuration.py
-anomalib/utils/callbacks/tiler_configuration.py
-anomalib/utils/callbacks/timer.py
-anomalib/utils/callbacks/nncf/__init__.py
-anomalib/utils/callbacks/nncf/callback.py
-anomalib/utils/callbacks/nncf/utils.py
-anomalib/utils/callbacks/visualizer/__init__.py
-anomalib/utils/callbacks/visualizer/visualizer_base.py
-anomalib/utils/callbacks/visualizer/visualizer_image.py
-anomalib/utils/callbacks/visualizer/visualizer_metric.py
-anomalib/utils/cli/__init__.py
-anomalib/utils/cli/cli.py
-anomalib/utils/cv/__init__.py
-anomalib/utils/cv/connected_components.py
-anomalib/utils/hpo/__init__.py
-anomalib/utils/hpo/config.py
-anomalib/utils/hpo/runners.py
-anomalib/utils/loggers/__init__.py
-anomalib/utils/loggers/base.py
-anomalib/utils/loggers/comet.py
-anomalib/utils/loggers/tensorboard.py
-anomalib/utils/loggers/wandb.py
-anomalib/utils/metrics/__init__.py
-anomalib/utils/metrics/anomaly_score_distribution.py
-anomalib/utils/metrics/anomaly_score_threshold.py
-anomalib/utils/metrics/aupr.py
-anomalib/utils/metrics/aupro.py
-anomalib/utils/metrics/auroc.py
-anomalib/utils/metrics/collection.py
-anomalib/utils/metrics/min_max.py
-anomalib/utils/metrics/optimal_f1.py
-anomalib/utils/metrics/plotting_utils.py
-anomalib/utils/metrics/pro.py
-anomalib/utils/sweep/__init__.py
-anomalib/utils/sweep/config.py
-anomalib/utils/sweep/helpers/__init__.py
-anomalib/utils/sweep/helpers/callbacks.py
-anomalib/utils/sweep/helpers/inference.py
 requirements/base.txt
 requirements/dev.txt
 requirements/docs.txt
-requirements/extras.txt
+requirements/loggers.txt
+requirements/notebooks.txt
 requirements/openvino.txt
-tests/helpers/__init__.py
-tests/helpers/aupro_reference.py
-tests/helpers/config.py
-tests/helpers/dataset.py
-tests/helpers/detection.py
-tests/helpers/dummy.py
-tests/helpers/inference.py
-tests/helpers/metrics.py
-tests/helpers/model.py
-tests/helpers/shapes.py
-tests/nightly/__init__.py
-tests/nightly/models/__init__.py
-tests/nightly/models/test_model_nightly.py
-tests/nightly/tools/__init__.py
-tests/nightly/tools/benchmarking/__init__.py
-tests/nightly/tools/benchmarking/test_benchmarking.py
-tests/pre_merge/__init__.py
-tests/pre_merge/config/__init__.py
-tests/pre_merge/config/test_config.py
-tests/pre_merge/datasets/__init__.py
-tests/pre_merge/datasets/test_bounding_box_utils.py
-tests/pre_merge/datasets/test_collate.py
-tests/pre_merge/datasets/test_datamodule.py
-tests/pre_merge/datasets/test_dataset.py
-tests/pre_merge/datasets/test_synthetic_data.py
-tests/pre_merge/datasets/test_tiler.py
-tests/pre_merge/datasets/test_video.py
-tests/pre_merge/deploy/__init__.py
-tests/pre_merge/deploy/test_inferencer.py
-tests/pre_merge/models/__init__.py
-tests/pre_merge/models/test_feature_extractor.py
-tests/pre_merge/models/test_model_premerge.py
-tests/pre_merge/models/components/__init__.py
-tests/pre_merge/models/components/test_blur.py
-tests/pre_merge/post_processing/__init__.py
-tests/pre_merge/post_processing/test_visualizer.py
-tests/pre_merge/pre_processing/__init__.py
-tests/pre_merge/pre_processing/test_tiler.py
-tests/pre_merge/pre_processing/transforms/__init__.py
-tests/pre_merge/pre_processing/transforms/test_transforms.py
-tests/pre_merge/utils/__init__.py
-tests/pre_merge/utils/test_config.py
-tests/pre_merge/utils/callbacks/__init__.py
-tests/pre_merge/utils/callbacks/export_callback/__init__.py
-tests/pre_merge/utils/callbacks/export_callback/dummy_lightning_model.py
-tests/pre_merge/utils/callbacks/export_callback/test_export.py
-tests/pre_merge/utils/callbacks/metrics_configuration_callback/__init__.py
-tests/pre_merge/utils/callbacks/metrics_configuration_callback/test_metrics_configuration_callback.py
-tests/pre_merge/utils/callbacks/normalization_callback/__init__.py
-tests/pre_merge/utils/callbacks/normalization_callback/test_normalization_callback.py
-tests/pre_merge/utils/callbacks/visualizer_callback/__init__.py
-tests/pre_merge/utils/callbacks/visualizer_callback/dummy_lightning_model.py
-tests/pre_merge/utils/callbacks/visualizer_callback/test_visualizer.py
-tests/pre_merge/utils/loggers/__init__.py
-tests/pre_merge/utils/loggers/test_get_logger.py
-tests/pre_merge/utils/metrics/__init__.py
-tests/pre_merge/utils/metrics/test_adaptive_threshold.py
-tests/pre_merge/utils/metrics/test_aupro.py
-tests/pre_merge/utils/metrics/test_pro.py
-tests/pre_merge/utils/sweep/__init__.py
-tests/pre_merge/utils/sweep/test_config.py
+src/anomalib/__init__.py
+src/anomalib/py.typed
+src/anomalib.egg-info/PKG-INFO
+src/anomalib.egg-info/SOURCES.txt
+src/anomalib.egg-info/dependency_links.txt
+src/anomalib.egg-info/entry_points.txt
+src/anomalib.egg-info/requires.txt
+src/anomalib.egg-info/top_level.txt
+src/anomalib/config/__init__.py
+src/anomalib/config/config.py
+src/anomalib/data/__init__.py
+src/anomalib/data/avenue.py
+src/anomalib/data/btech.py
+src/anomalib/data/folder.py
+src/anomalib/data/folder_3d.py
+src/anomalib/data/inference.py
+src/anomalib/data/mvtec.py
+src/anomalib/data/mvtec_3d.py
+src/anomalib/data/shanghaitech.py
+src/anomalib/data/synthetic.py
+src/anomalib/data/task_type.py
+src/anomalib/data/ucsd_ped.py
+src/anomalib/data/visa.py
+src/anomalib/data/base/__init__.py
+src/anomalib/data/base/datamodule.py
+src/anomalib/data/base/dataset.py
+src/anomalib/data/base/depth.py
+src/anomalib/data/base/video.py
+src/anomalib/data/utils/__init__.py
+src/anomalib/data/utils/augmenter.py
+src/anomalib/data/utils/boxes.py
+src/anomalib/data/utils/download.py
+src/anomalib/data/utils/image.py
+src/anomalib/data/utils/label.py
+src/anomalib/data/utils/path.py
+src/anomalib/data/utils/split.py
+src/anomalib/data/utils/transform.py
+src/anomalib/data/utils/video.py
+src/anomalib/data/utils/generators/__init__.py
+src/anomalib/data/utils/generators/perlin.py
+src/anomalib/deploy/__init__.py
+src/anomalib/deploy/export.py
+src/anomalib/deploy/inferencers/__init__.py
+src/anomalib/deploy/inferencers/base_inferencer.py
+src/anomalib/deploy/inferencers/openvino_inferencer.py
+src/anomalib/deploy/inferencers/torch_inferencer.py
+src/anomalib/models/__init__.py
+src/anomalib/models/ai_vad/__init__.py
+src/anomalib/models/ai_vad/config.yaml
+src/anomalib/models/ai_vad/density.py
+src/anomalib/models/ai_vad/features.py
+src/anomalib/models/ai_vad/flow.py
+src/anomalib/models/ai_vad/lightning_model.py
+src/anomalib/models/ai_vad/regions.py
+src/anomalib/models/ai_vad/torch_model.py
+src/anomalib/models/ai_vad/clip/__init__.py
+src/anomalib/models/ai_vad/clip/clip.py
+src/anomalib/models/ai_vad/clip/model.py
+src/anomalib/models/cfa/__init__.py
+src/anomalib/models/cfa/anomaly_map.py
+src/anomalib/models/cfa/config.yaml
+src/anomalib/models/cfa/lightning_model.py
+src/anomalib/models/cfa/loss.py
+src/anomalib/models/cfa/torch_model.py
+src/anomalib/models/cflow/__init__.py
+src/anomalib/models/cflow/anomaly_map.py
+src/anomalib/models/cflow/config.yaml
+src/anomalib/models/cflow/lightning_model.py
+src/anomalib/models/cflow/torch_model.py
+src/anomalib/models/cflow/utils.py
+src/anomalib/models/components/__init__.py
+src/anomalib/models/components/base/__init__.py
+src/anomalib/models/components/base/anomaly_module.py
+src/anomalib/models/components/base/dynamic_module.py
+src/anomalib/models/components/classification/__init__.py
+src/anomalib/models/components/classification/kde_classifier.py
+src/anomalib/models/components/dimensionality_reduction/__init__.py
+src/anomalib/models/components/dimensionality_reduction/pca.py
+src/anomalib/models/components/dimensionality_reduction/random_projection.py
+src/anomalib/models/components/feature_extractors/__init__.py
+src/anomalib/models/components/feature_extractors/timm.py
+src/anomalib/models/components/feature_extractors/torchfx.py
+src/anomalib/models/components/feature_extractors/utils.py
+src/anomalib/models/components/filters/__init__.py
+src/anomalib/models/components/filters/blur.py
+src/anomalib/models/components/flow/__init__.py
+src/anomalib/models/components/flow/all_in_one_block.py
+src/anomalib/models/components/layers/__init__.py
+src/anomalib/models/components/layers/sspcab.py
+src/anomalib/models/components/sampling/__init__.py
+src/anomalib/models/components/sampling/k_center_greedy.py
+src/anomalib/models/components/stats/__init__.py
+src/anomalib/models/components/stats/kde.py
+src/anomalib/models/components/stats/multi_variate_gaussian.py
+src/anomalib/models/csflow/__init__.py
+src/anomalib/models/csflow/anomaly_map.py
+src/anomalib/models/csflow/config.yaml
+src/anomalib/models/csflow/lightning_model.py
+src/anomalib/models/csflow/loss.py
+src/anomalib/models/csflow/torch_model.py
+src/anomalib/models/dfkde/__init__.py
+src/anomalib/models/dfkde/config.yaml
+src/anomalib/models/dfkde/lightning_model.py
+src/anomalib/models/dfkde/torch_model.py
+src/anomalib/models/dfm/__init__.py
+src/anomalib/models/dfm/config.yaml
+src/anomalib/models/dfm/lightning_model.py
+src/anomalib/models/dfm/torch_model.py
+src/anomalib/models/draem/__init__.py
+src/anomalib/models/draem/config.yaml
+src/anomalib/models/draem/lightning_model.py
+src/anomalib/models/draem/loss.py
+src/anomalib/models/draem/torch_model.py
+src/anomalib/models/fastflow/__init__.py
+src/anomalib/models/fastflow/anomaly_map.py
+src/anomalib/models/fastflow/config.yaml
+src/anomalib/models/fastflow/lightning_model.py
+src/anomalib/models/fastflow/loss.py
+src/anomalib/models/fastflow/torch_model.py
+src/anomalib/models/ganomaly/__init__.py
+src/anomalib/models/ganomaly/config.yaml
+src/anomalib/models/ganomaly/lightning_model.py
+src/anomalib/models/ganomaly/loss.py
+src/anomalib/models/ganomaly/torch_model.py
+src/anomalib/models/padim/__init__.py
+src/anomalib/models/padim/anomaly_map.py
+src/anomalib/models/padim/config.yaml
+src/anomalib/models/padim/lightning_model.py
+src/anomalib/models/padim/torch_model.py
+src/anomalib/models/patchcore/__init__.py
+src/anomalib/models/patchcore/anomaly_map.py
+src/anomalib/models/patchcore/config.yaml
+src/anomalib/models/patchcore/lightning_model.py
+src/anomalib/models/patchcore/torch_model.py
+src/anomalib/models/reverse_distillation/__init__.py
+src/anomalib/models/reverse_distillation/anomaly_map.py
+src/anomalib/models/reverse_distillation/config.yaml
+src/anomalib/models/reverse_distillation/lightning_model.py
+src/anomalib/models/reverse_distillation/loss.py
+src/anomalib/models/reverse_distillation/torch_model.py
+src/anomalib/models/reverse_distillation/components/__init__.py
+src/anomalib/models/reverse_distillation/components/bottleneck.py
+src/anomalib/models/reverse_distillation/components/de_resnet.py
+src/anomalib/models/rkde/__init__.py
+src/anomalib/models/rkde/config.yaml
+src/anomalib/models/rkde/feature_extractor.py
+src/anomalib/models/rkde/lightning_model.py
+src/anomalib/models/rkde/region_extractor.py
+src/anomalib/models/rkde/torch_model.py
+src/anomalib/models/stfpm/__init__.py
+src/anomalib/models/stfpm/anomaly_map.py
+src/anomalib/models/stfpm/config.yaml
+src/anomalib/models/stfpm/lightning_model.py
+src/anomalib/models/stfpm/loss.py
+src/anomalib/models/stfpm/torch_model.py
+src/anomalib/post_processing/__init__.py
+src/anomalib/post_processing/post_process.py
+src/anomalib/post_processing/visualizer.py
+src/anomalib/post_processing/normalization/__init__.py
+src/anomalib/post_processing/normalization/cdf.py
+src/anomalib/post_processing/normalization/min_max.py
+src/anomalib/pre_processing/__init__.py
+src/anomalib/pre_processing/pre_process.py
+src/anomalib/pre_processing/tiler.py
+src/anomalib/pre_processing/transforms/__init__.py
+src/anomalib/pre_processing/transforms/custom.py
+src/anomalib/utils/__init__.py
+src/anomalib/utils/callbacks/__init__.py
+src/anomalib/utils/callbacks/cdf_normalization.py
+src/anomalib/utils/callbacks/export.py
+src/anomalib/utils/callbacks/graph.py
+src/anomalib/utils/callbacks/metrics_configuration.py
+src/anomalib/utils/callbacks/min_max_normalization.py
+src/anomalib/utils/callbacks/model_loader.py
+src/anomalib/utils/callbacks/post_processing_configuration.py
+src/anomalib/utils/callbacks/tiler_configuration.py
+src/anomalib/utils/callbacks/timer.py
+src/anomalib/utils/callbacks/nncf/__init__.py
+src/anomalib/utils/callbacks/nncf/callback.py
+src/anomalib/utils/callbacks/nncf/utils.py
+src/anomalib/utils/callbacks/visualizer/__init__.py
+src/anomalib/utils/callbacks/visualizer/visualizer_base.py
+src/anomalib/utils/callbacks/visualizer/visualizer_image.py
+src/anomalib/utils/callbacks/visualizer/visualizer_metric.py
+src/anomalib/utils/cli/__init__.py
+src/anomalib/utils/cli/cli.py
+src/anomalib/utils/cv/__init__.py
+src/anomalib/utils/cv/connected_components.py
+src/anomalib/utils/hpo/__init__.py
+src/anomalib/utils/hpo/config.py
+src/anomalib/utils/hpo/runners.py
+src/anomalib/utils/loggers/__init__.py
+src/anomalib/utils/loggers/base.py
+src/anomalib/utils/loggers/comet.py
+src/anomalib/utils/loggers/tensorboard.py
+src/anomalib/utils/loggers/wandb.py
+src/anomalib/utils/metrics/__init__.py
+src/anomalib/utils/metrics/anomaly_score_distribution.py
+src/anomalib/utils/metrics/anomaly_score_threshold.py
+src/anomalib/utils/metrics/aupr.py
+src/anomalib/utils/metrics/aupro.py
+src/anomalib/utils/metrics/auroc.py
+src/anomalib/utils/metrics/collection.py
+src/anomalib/utils/metrics/min_max.py
+src/anomalib/utils/metrics/optimal_f1.py
+src/anomalib/utils/metrics/plotting_utils.py
+src/anomalib/utils/metrics/pro.py
+src/anomalib/utils/sweep/__init__.py
+src/anomalib/utils/sweep/config.py
+src/anomalib/utils/sweep/helpers/__init__.py
+src/anomalib/utils/sweep/helpers/callbacks.py
+src/anomalib/utils/sweep/helpers/inference.py
```

### Comparing `anomalib-0.4.0rc2/setup.py` & `anomalib-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
 from types import ModuleType
 
 from setuptools import find_packages, setup
 
 
-def load_module(name: str = "anomalib/__init__.py") -> ModuleType:
+def load_module(name: str = "src/anomalib/__init__.py") -> ModuleType:
     """Load Python Module.
 
     Args:
         name (str, optional): Name of the module to load.
             Defaults to "anomalib/__init__.py".
 
     Returns:
@@ -41,15 +41,15 @@
         >>> # Assume that __version__ = "0.2.6"
         >>> get_version()
         "0.2.6"
 
     Returns:
         str: `anomalib` version.
     """
-    anomalib = load_module(name="anomalib/__init__.py")
+    anomalib = load_module(name="src/anomalib/__init__.py")
     version = anomalib.__version__
     return version
 
 
 def get_required_packages(requirement_files: list[str]) -> list[str]:
     """Get packages from requirements.txt file.
 
@@ -79,17 +79,18 @@
     return required_packages
 
 
 VERSION = get_version()
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text(encoding="utf8")
 INSTALL_REQUIRES = get_required_packages(requirement_files=["base"])
 EXTRAS_REQUIRE = {
-    "extra": get_required_packages(requirement_files=["extras"]),
-    "full": get_required_packages(requirement_files=["docs", "openvino", "extras"]),
+    "loggers": get_required_packages(requirement_files=["loggers"]),
+    "notebooks": get_required_packages(requirement_files=["notebooks"]),
     "openvino": get_required_packages(requirement_files=["openvino"]),
+    "full": get_required_packages(requirement_files=["loggers", "notebooks", "openvino"]),
 }
 
 
 setup(
     name="anomalib",
     version=get_version(),
     author="Intel OpenVINO",
@@ -98,13 +99,14 @@
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="",
     license="Copyright (c) Intel - All Rights Reserved. "
     'Licensed under the Apache License, Version 2.0 (the "License")'
     "See LICENSE file for more details.",
     python_requires=">=3.7",
-    packages=find_packages(exclude=("tests",)),
+    package_dir={"": "src"},
+    packages=find_packages(where="src", include=["anomalib", "anomalib.*"]),
     install_requires=INSTALL_REQUIRES,
     extras_require=EXTRAS_REQUIRE,
     package_data={"": ["config.yaml"]},
     entry_points={"console_scripts": ["anomalib=anomalib.utils.cli.cli:main"]},
 )
```

