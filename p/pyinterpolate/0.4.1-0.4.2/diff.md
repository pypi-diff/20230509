# Comparing `tmp/pyinterpolate-0.4.1.tar.gz` & `tmp/pyinterpolate-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinterpolate-0.4.1.tar", last modified: Sun Apr 16 09:56:38 2023, max compression
+gzip compressed data, was "pyinterpolate-0.4.2.tar", last modified: Tue May  9 11:32:54 2023, max compression
```

## Comparing `pyinterpolate-0.4.1.tar` & `pyinterpolate-0.4.2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.065284 pyinterpolate-0.4.1/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       42 2021-10-17 13:15:38.000000 pyinterpolate-0.4.1/MANIFEST.in
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     9660 2023-04-16 09:56:38.069284 pyinterpolate-0.4.1/PKG-INFO
--rwxrwxr-x   0 szymon    (1000) szymon    (1000)     8654 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/README.md
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.049284 pyinterpolate-0.4.1/pyinterpolate/
--rwxrwxr-x   0 szymon    (1000) szymon    (1000)     1442 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/__init__.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.053284 pyinterpolate-0.4.1/pyinterpolate/distance/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      187 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/distance/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     7804 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/distance/clusters.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    11000 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/distance/distance.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     6216 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/distance/gridding.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.053284 pyinterpolate-0.4.1/pyinterpolate/idw/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       60 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/idw/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     3507 2022-10-08 09:51:45.000000 pyinterpolate-0.4.1/pyinterpolate/idw/idw.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.053284 pyinterpolate-0.4.1/pyinterpolate/io/
--rwxrwxr-x   0 szymon    (1000) szymon    (1000)       70 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/io/__init__.py
--rwxrwxr-x   0 szymon    (1000) szymon    (1000)     5946 2022-10-08 09:51:45.000000 pyinterpolate-0.4.1/pyinterpolate/io/read_data.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.053284 pyinterpolate-0.4.1/pyinterpolate/kriging/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      595 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/__init__.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.053284 pyinterpolate-0.4.1/pyinterpolate/kriging/models/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/__init__.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.057284 pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      187 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     7711 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/area_to_area_poisson_kriging.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     9806 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/area_to_point_poisson_kriging.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     7405 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/centroid_based_poisson_kriging.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    10644 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/weight.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.057284 pyinterpolate-0.4.1/pyinterpolate/kriging/models/indicator/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/indicator/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    13128 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/indicator/indicator_point_kriging.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.057284 pyinterpolate-0.4.1/pyinterpolate/kriging/models/point/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/point/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     6965 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/point/ordinary_kriging.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     3766 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/point/simple_kriging.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.057284 pyinterpolate-0.4.1/pyinterpolate/kriging/models/structures/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/structures/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      687 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/structures/point_kriging.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     7666 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/point_kriging.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.057284 pyinterpolate-0.4.1/pyinterpolate/kriging/utils/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/utils/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1078 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/utils/kwarnings.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     4870 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/utils/process.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.057284 pyinterpolate-0.4.1/pyinterpolate/pipelines/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      246 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/pipelines/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    13437 2022-10-08 09:51:45.000000 pyinterpolate-0.4.1/pyinterpolate/pipelines/block_filtering.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     5227 2022-11-05 20:50:31.000000 pyinterpolate-0.4.1/pyinterpolate/pipelines/deconvolution.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    12890 2022-10-08 09:51:45.000000 pyinterpolate-0.4.1/pyinterpolate/pipelines/multi_kriging.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/processing/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       79 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/processing/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     2543 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/processing/checks.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/processing/preprocessing/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/processing/preprocessing/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    17173 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/processing/preprocessing/blocks.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    36344 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/processing/select_values.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/processing/transform/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/processing/transform/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     5490 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/processing/transform/statistics.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    11202 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/processing/transform/transform.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/processing/utils/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/processing/utils/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1802 2022-11-05 20:50:31.000000 pyinterpolate-0.4.1/pyinterpolate/processing/utils/exceptions.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/validation/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/validation/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     4079 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/validation/cross_validation.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/variogram/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      682 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/__init__.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1857 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    23322 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/cloud.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    10484 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/covariance.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    24364 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/experimental_variogram.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    23469 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/semivariance.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/variogram/indicator/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/indicator/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    16428 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/indicator/indicator_variogram.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    24569 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/aggregated.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.065284 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1489 2022-10-09 07:47:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/avg_block_to_block_semivariances.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     4047 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/avg_inblock_semivariances.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     5343 2022-10-09 07:47:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/block_to_block_semivariance.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     8847 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/inblock_semivariance.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    33633 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/deconvolution.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.065284 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     5340 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/__init__.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.065284 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/models/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       31 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/models/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     8319 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/models/variogram_models.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    37830 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/semivariogram.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1140 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/spatial_dependency_index.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.065284 pyinterpolate-0.4.1/pyinterpolate/variogram/utils/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/utils/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     6990 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/utils/exceptions.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     9500 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/utils/metrics.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     2046 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/utils/plots.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.065284 pyinterpolate-0.4.1/pyinterpolate/viz/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       55 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/viz/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     5348 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/viz/raster.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.053284 pyinterpolate-0.4.1/pyinterpolate.egg-info/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     9660 2023-04-16 09:56:38.000000 pyinterpolate-0.4.1/pyinterpolate.egg-info/PKG-INFO
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     3556 2023-04-16 09:56:38.000000 pyinterpolate-0.4.1/pyinterpolate.egg-info/SOURCES.txt
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        1 2023-04-16 09:56:38.000000 pyinterpolate-0.4.1/pyinterpolate.egg-info/dependency_links.txt
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        1 2023-04-16 09:56:37.000000 pyinterpolate-0.4.1/pyinterpolate.egg-info/not-zip-safe
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      884 2023-04-16 09:56:38.000000 pyinterpolate-0.4.1/pyinterpolate.egg-info/requires.txt
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       14 2023-04-16 09:56:38.000000 pyinterpolate-0.4.1/pyinterpolate.egg-info/top_level.txt
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       80 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyproject.toml
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     2186 2023-04-16 09:56:38.069284 pyinterpolate-0.4.1/setup.cfg
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.152296 pyinterpolate-0.4.2/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       42 2021-10-17 13:15:38.000000 pyinterpolate-0.4.2/MANIFEST.in
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     9660 2023-05-09 11:32:54.152296 pyinterpolate-0.4.2/PKG-INFO
+-rwxrwxr-x   0 szymon    (1000) szymon    (1000)     8654 2023-05-09 11:30:07.000000 pyinterpolate-0.4.2/README.md
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.144296 pyinterpolate-0.4.2/pyinterpolate/
+-rwxrwxr-x   0 szymon    (1000) szymon    (1000)     1442 2023-05-09 11:30:07.000000 pyinterpolate-0.4.2/pyinterpolate/__init__.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.144296 pyinterpolate-0.4.2/pyinterpolate/distance/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      187 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/distance/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     7804 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/distance/clusters.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    11000 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/distance/distance.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     6216 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/distance/gridding.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.144296 pyinterpolate-0.4.2/pyinterpolate/idw/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       60 2022-09-07 20:00:15.000000 pyinterpolate-0.4.2/pyinterpolate/idw/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     3507 2022-10-08 09:51:45.000000 pyinterpolate-0.4.2/pyinterpolate/idw/idw.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.144296 pyinterpolate-0.4.2/pyinterpolate/io/
+-rwxrwxr-x   0 szymon    (1000) szymon    (1000)       70 2022-09-07 20:00:15.000000 pyinterpolate-0.4.2/pyinterpolate/io/__init__.py
+-rwxrwxr-x   0 szymon    (1000) szymon    (1000)     6650 2023-05-09 11:30:07.000000 pyinterpolate-0.4.2/pyinterpolate/io/read_data.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.144296 pyinterpolate-0.4.2/pyinterpolate/kriging/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      595 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/__init__.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.144296 pyinterpolate-0.4.2/pyinterpolate/kriging/models/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/models/__init__.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.144296 pyinterpolate-0.4.2/pyinterpolate/kriging/models/block/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      187 2022-09-07 20:00:15.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/models/block/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     7711 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/models/block/area_to_area_poisson_kriging.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     9806 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/models/block/area_to_point_poisson_kriging.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     7405 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/models/block/centroid_based_poisson_kriging.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    10644 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/models/block/weight.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.144296 pyinterpolate-0.4.2/pyinterpolate/kriging/models/indicator/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/models/indicator/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    13128 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/models/indicator/indicator_point_kriging.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.144296 pyinterpolate-0.4.2/pyinterpolate/kriging/models/point/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/models/point/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     6965 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/models/point/ordinary_kriging.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     3766 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/models/point/simple_kriging.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.144296 pyinterpolate-0.4.2/pyinterpolate/kriging/models/structures/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/models/structures/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      687 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/models/structures/point_kriging.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     7666 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/point_kriging.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.148296 pyinterpolate-0.4.2/pyinterpolate/kriging/utils/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/utils/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1078 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/utils/kwarnings.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     4870 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/kriging/utils/process.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.148296 pyinterpolate-0.4.2/pyinterpolate/pipelines/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      246 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/pipelines/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    13437 2022-10-08 09:51:45.000000 pyinterpolate-0.4.2/pyinterpolate/pipelines/block_filtering.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     5227 2022-11-05 20:50:31.000000 pyinterpolate-0.4.2/pyinterpolate/pipelines/deconvolution.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    12890 2022-10-08 09:51:45.000000 pyinterpolate-0.4.2/pyinterpolate/pipelines/multi_kriging.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.148296 pyinterpolate-0.4.2/pyinterpolate/processing/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       79 2022-09-07 20:00:15.000000 pyinterpolate-0.4.2/pyinterpolate/processing/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     2543 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/processing/checks.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.148296 pyinterpolate-0.4.2/pyinterpolate/processing/preprocessing/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.2/pyinterpolate/processing/preprocessing/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    18251 2023-05-09 11:30:07.000000 pyinterpolate-0.4.2/pyinterpolate/processing/preprocessing/blocks.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    36344 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/processing/select_values.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.148296 pyinterpolate-0.4.2/pyinterpolate/processing/transform/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.2/pyinterpolate/processing/transform/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     5490 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/processing/transform/statistics.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    11202 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/processing/transform/transform.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.148296 pyinterpolate-0.4.2/pyinterpolate/processing/utils/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.2/pyinterpolate/processing/utils/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1802 2022-11-05 20:50:31.000000 pyinterpolate-0.4.2/pyinterpolate/processing/utils/exceptions.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.148296 pyinterpolate-0.4.2/pyinterpolate/validation/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/validation/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     4079 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/validation/cross_validation.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.148296 pyinterpolate-0.4.2/pyinterpolate/variogram/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      682 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/__init__.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.148296 pyinterpolate-0.4.2/pyinterpolate/variogram/empirical/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1857 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/empirical/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    23322 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/empirical/cloud.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    10484 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/empirical/covariance.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    24364 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/empirical/experimental_variogram.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    23469 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/empirical/semivariance.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.148296 pyinterpolate-0.4.2/pyinterpolate/variogram/indicator/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/indicator/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    16428 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/indicator/indicator_variogram.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.152296 pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:16.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    24569 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/aggregated.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.152296 pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/block/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:16.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/block/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1489 2022-10-09 07:47:16.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/block/avg_block_to_block_semivariances.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     4047 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/block/avg_inblock_semivariances.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     5343 2022-10-09 07:47:16.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/block/block_to_block_semivariance.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     8847 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/block/inblock_semivariance.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    33633 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/deconvolution.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.152296 pyinterpolate-0.4.2/pyinterpolate/variogram/theoretical/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     5340 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/theoretical/__init__.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.152296 pyinterpolate-0.4.2/pyinterpolate/variogram/theoretical/models/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       31 2022-09-07 20:00:16.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/theoretical/models/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     8319 2022-09-07 20:00:16.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/theoretical/models/variogram_models.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    37830 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/theoretical/semivariogram.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1140 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/theoretical/spatial_dependency_index.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.152296 pyinterpolate-0.4.2/pyinterpolate/variogram/utils/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:16.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/utils/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     6990 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/utils/exceptions.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     9500 2022-09-07 20:00:16.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/utils/metrics.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     2046 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/variogram/utils/plots.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.152296 pyinterpolate-0.4.2/pyinterpolate/viz/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       55 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/viz/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     5348 2023-04-16 09:55:49.000000 pyinterpolate-0.4.2/pyinterpolate/viz/raster.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-05-09 11:32:54.144296 pyinterpolate-0.4.2/pyinterpolate.egg-info/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     9660 2023-05-09 11:32:54.000000 pyinterpolate-0.4.2/pyinterpolate.egg-info/PKG-INFO
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     3556 2023-05-09 11:32:54.000000 pyinterpolate-0.4.2/pyinterpolate.egg-info/SOURCES.txt
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        1 2023-05-09 11:32:54.000000 pyinterpolate-0.4.2/pyinterpolate.egg-info/dependency_links.txt
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        1 2023-04-16 09:56:37.000000 pyinterpolate-0.4.2/pyinterpolate.egg-info/not-zip-safe
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      892 2023-05-09 11:32:54.000000 pyinterpolate-0.4.2/pyinterpolate.egg-info/requires.txt
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       14 2023-05-09 11:32:54.000000 pyinterpolate-0.4.2/pyinterpolate.egg-info/top_level.txt
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       80 2022-09-07 20:00:16.000000 pyinterpolate-0.4.2/pyproject.toml
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     2195 2023-05-09 11:32:54.152296 pyinterpolate-0.4.2/setup.cfg
```

### Comparing `pyinterpolate-0.4.1/PKG-INFO` & `pyinterpolate-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinterpolate
-Version: 0.4.1
+Version: 0.4.2
 Summary: Spatial Interpolation in Python
 Home-page: https://github.com/DataverseLabs/pyinterpolate
 Download-URL: https://github.com/DataverseLabs/pyinterpolate/archive/
 Author: Szymon Moliński
 Author-email: simon@dataverselabs.com
 License: BSD 3-clause
 Project-URL: Documentation, https://readthedocs.org/projects/pyinterpolate/
@@ -23,15 +23,15 @@
 
 ![status](https://joss.theoj.org/papers/3f87f562264c4e5174d9e6ed6d8812aa/status.svg) ![License](https://img.shields.io/github/license/szymon-datalions/pyinterpolate) ![Documentation Status](https://readthedocs.org/projects/pyinterpolate/badge/?version=latest) [![CodeFactor](https://www.codefactor.io/repository/github/dataverselabs/pyinterpolate/badge)](https://www.codefactor.io/repository/github/dataverselabs/pyinterpolate)
 
 ![Pyinterpolate](https://github.com/DataverseLabs/pyinterpolate/blob/main/logov04.jpg?raw=true  "Pyinterpolate logo")
 
 # Pyinterpolate
 
-**version 0.4.1** - *Kharkiv*
+**version 0.4.2** - *Kharkiv*
 
 ---
 
 Pyinterpolate is the Python library for **spatial statistics**. The package provides access to spatial statistics tools used in various studies. This package helps you **interpolate spatial data** with the *Kriging* technique.
 
 If you’re:
```

### Comparing `pyinterpolate-0.4.1/README.md` & `pyinterpolate-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![status](https://joss.theoj.org/papers/3f87f562264c4e5174d9e6ed6d8812aa/status.svg) ![License](https://img.shields.io/github/license/szymon-datalions/pyinterpolate) ![Documentation Status](https://readthedocs.org/projects/pyinterpolate/badge/?version=latest) [![CodeFactor](https://www.codefactor.io/repository/github/dataverselabs/pyinterpolate/badge)](https://www.codefactor.io/repository/github/dataverselabs/pyinterpolate)
 
 ![Pyinterpolate](https://github.com/DataverseLabs/pyinterpolate/blob/main/logov04.jpg?raw=true  "Pyinterpolate logo")
 
 # Pyinterpolate
 
-**version 0.4.1** - *Kharkiv*
+**version 0.4.2** - *Kharkiv*
 
 ---
 
 Pyinterpolate is the Python library for **spatial statistics**. The package provides access to spatial statistics tools used in various studies. This package helps you **interpolate spatial data** with the *Kriging* technique.
 
 If you’re:
```

### Comparing `pyinterpolate-0.4.1/pyinterpolate/__init__.py` & `pyinterpolate-0.4.2/pyinterpolate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 # Indicator
 from pyinterpolate.variogram import IndicatorVariogramData, ExperimentalIndicatorVariogram, IndicatorVariograms
 
 # Viz
 from pyinterpolate.viz import interpolate_raster
 
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
```

### Comparing `pyinterpolate-0.4.1/pyinterpolate/distance/clusters.py` & `pyinterpolate-0.4.2/pyinterpolate/distance/clusters.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/distance/distance.py` & `pyinterpolate-0.4.2/pyinterpolate/distance/distance.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/distance/gridding.py` & `pyinterpolate-0.4.2/pyinterpolate/distance/gridding.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/idw/idw.py` & `pyinterpolate-0.4.2/pyinterpolate/idw/idw.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/io/read_data.py` & `pyinterpolate-0.4.2/pyinterpolate/io/read_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """
 Read and load data.
 
 Authors
 -------
 1. Szymon Moliński | @SimonMolinsky
+2. Taher Chegini | @cheginit
 """
+from pathlib import Path
+from typing import Any
+
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 
 
 def read_txt(path: str, delim=',', skip_header=True) -> np.ndarray:
     """Function reads data from a text file.
@@ -98,34 +102,45 @@
     )
 
     data_arr = df[[lon_col_name, lat_col_name, val_col_name]].to_numpy()
 
     return data_arr
 
 
+def _open_geopandas(fpath: Path, **kwargs: Any)-> gpd.GeoDataFrame:
+    """Open the file with geopandas file."""
+    if fpath.suffix == ".feather":
+        return gpd.read_feather(fpath, **kwargs)
+    if fpath.suffix == ".parquet":
+        return gpd.read_parquet(fpath, **kwargs)
+    return gpd.read_file(fpath, **kwargs)
+
+
 def read_block(
         path: str,
         val_col_name: str,
         geometry_col_name='geometry',
         id_col_name=None,
         centroid_col_name=None,
         epsg=None,
-        crs=None
+        crs=None,
+        **kwargs,
 ) -> gpd.GeoDataFrame:
-    """Function reads block data from files supported by fiona / geopandas.
+    """Function reads block data from files supported by geopandas.
 
     Value column name must be provided. If geometry column has different name than `'geometry'` then
     it must be provided too. ID column name is optional, if not given then ``GeoDataFrame`` `index` is
     treated as an id column. Optional parameters are `epsg` and `crs`. If any is set then data is reprojected
     into a specific `crs/epsg`.` Function returns ``GeoDataFrame`` with columns: ``[id, value, geometry, centroid]``.
 
     Parameters
     ----------
     path : str
-        Path to the file.
+        Path to the file with appropriate extension such as ``.shp``,
+        ``.gpkg``, ``.feather``, or ``.parquet``.
 
     val_col_name : str
         Name of the value column (header title).
 
     geometry_col_name : str, default='geometry'
         Name of the column with polygons.
 
@@ -139,14 +154,18 @@
 
     epsg : str or None, default=None
         If provided then ``GeoDataFrame`` projection is set to it. You should choose if you provide `EPSG` or `CRS`.
 
     crs : str or None, default=None
         If provided then ``GeoDataFrame`` projection is set to it. You should choose if you provide `CRS` or `EPSG`.
 
+    **kwargs : Any
+        Additional kwargs parameters passed to the ``geopandas.read_file()``,
+        ``geopandas.read_feather()`` or ``geopandas.read_parquet()`` functions.
+
     Returns
     -------
     gpd : GeoDataFrame
         Returned output has columns: ``['id', 'geometry', 'value', 'centroid']``.
 
     Raises
     ------
@@ -177,15 +196,15 @@
     if check_geometry_params:
         pass
     else:
         raise TypeError(f'Only one value CRS or EPSG should be provided but both are given: crs {crs}; epsg: {epsg}')
 
     # FUNCTION'S BODY
 
-    gdf = gpd.read_file(path)
+    gdf = _open_geopandas(Path(path), **kwargs)
 
     # Check if columns exist
     gdf_cols = gdf.columns
     for c in columns:
         if c not in gdf_cols:
             raise TypeError(f'Given column {c} is not present in a dataset. Available columns: {gdf_cols}')
```

### Comparing `pyinterpolate-0.4.1/pyinterpolate/kriging/__init__.py` & `pyinterpolate-0.4.2/pyinterpolate/kriging/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/area_to_area_poisson_kriging.py` & `pyinterpolate-0.4.2/pyinterpolate/kriging/models/block/area_to_area_poisson_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/area_to_point_poisson_kriging.py` & `pyinterpolate-0.4.2/pyinterpolate/kriging/models/block/area_to_point_poisson_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/centroid_based_poisson_kriging.py` & `pyinterpolate-0.4.2/pyinterpolate/kriging/models/block/centroid_based_poisson_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/weight.py` & `pyinterpolate-0.4.2/pyinterpolate/kriging/models/block/weight.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/kriging/models/indicator/indicator_point_kriging.py` & `pyinterpolate-0.4.2/pyinterpolate/kriging/models/indicator/indicator_point_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/kriging/models/point/ordinary_kriging.py` & `pyinterpolate-0.4.2/pyinterpolate/kriging/models/point/ordinary_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/kriging/models/point/simple_kriging.py` & `pyinterpolate-0.4.2/pyinterpolate/kriging/models/point/simple_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/kriging/models/structures/point_kriging.py` & `pyinterpolate-0.4.2/pyinterpolate/kriging/models/structures/point_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/kriging/point_kriging.py` & `pyinterpolate-0.4.2/pyinterpolate/kriging/point_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/kriging/utils/kwarnings.py` & `pyinterpolate-0.4.2/pyinterpolate/kriging/utils/kwarnings.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/kriging/utils/process.py` & `pyinterpolate-0.4.2/pyinterpolate/kriging/utils/process.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/pipelines/block_filtering.py` & `pyinterpolate-0.4.2/pyinterpolate/pipelines/block_filtering.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/pipelines/deconvolution.py` & `pyinterpolate-0.4.2/pyinterpolate/pipelines/deconvolution.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/pipelines/multi_kriging.py` & `pyinterpolate-0.4.2/pyinterpolate/pipelines/multi_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/processing/checks.py` & `pyinterpolate-0.4.2/pyinterpolate/processing/checks.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/processing/preprocessing/blocks.py` & `pyinterpolate-0.4.2/pyinterpolate/processing/preprocessing/blocks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 """
 Core data structures for block interpolation.
 
 Authors
 -------
 1. Szymon Moliński | @SimonMolinsky
+2. Taher Chegini | @cheginit
 """
+from pathlib import Path
 import logging
-from typing import Union
+from typing import Any, Union
 
 import geopandas as gpd
 import pandas as pd
 
 from pyinterpolate.processing.utils.exceptions import IndexColNotUniqueError
 
 
+def _open_geopandas(fpath: Path, **kwargs: Any)-> gpd.GeoDataFrame:
+    """Open a file with the appropriate geopandas function."""
+    if fpath.suffix == ".feather":
+        return gpd.read_feather(fpath, **kwargs)
+    if fpath.suffix == ".parquet":
+        return gpd.read_parquet(fpath, **kwargs)
+    return gpd.read_file(fpath, **kwargs)
+
+
 class Blocks:
     """Class stores and prepares aggregated data.
 
     Attributes
     ----------
     data : gpd.GeoDataFrame
         Dataset with block values.
@@ -105,47 +116,51 @@
         self.geometry_column_name = geom_col
 
     def from_file(self,
                   fpath: str,
                   value_col,
                   geometry_col='geometry',
                   index_col=None,
-                  layer_name=None):
+                  layer_name=None,
+                  **kwargs):
         """
         Loads areal dataset from a file supported by GeoPandas.
 
         Parameters
         ----------
         fpath : str
-            Path to the spatial file.
+            Path to the spatial file with appropriate extension such as ``.shp``,
+        ``.gpkg``, ``.feather``, or ``.parquet``.
 
         value_col : Any
             The name of a column with values.
 
         geometry_col : default='geometry'
             The name of a column with blocks.
 
         index_col : default = None
             Index column name. It could be any unique value from a dataset. If not given then index is taken
             from the index array of ``GeoDataFrame``, and it is named ``'index'``.
 
         layer_name : Any, default = None
             The name of a layer with data if provided input is a *gpkg* file.
 
+        **kwargs : Any
+            Additional kwargs parameters passed to the ``geopandas.read_file()``,
+            ``geopandas.read_feather()`` or ``geopandas.read_parquet()`` functions.
+
         Raises
         ------
         IndexColNotUniqueError
             Raised when given index column has not unique values.
 
         """
-
-        if fpath.lower().endswith('.gpkg'):
-            dataset = gpd.read_file(fpath, layer=layer_name)
-        else:
-            dataset = gpd.read_file(fpath)
+        if layer_name is not None:
+            kwargs['layer'] = layer_name
+        dataset = _open_geopandas(Path(fpath), **kwargs)
 
         if index_col is not None:
             dataset = dataset[[index_col, geometry_col, value_col]]
             # Check indices
             self._check_index(dataset, index_col)
         else:
             if dataset.index.name:
@@ -298,25 +313,30 @@
                    blocks_file: str,
                    point_support_geometry_col,
                    point_support_val_col,
                    blocks_geometry_col,
                    blocks_index_col,
                    use_point_support_crs: bool = True,
                    point_support_layer_name=None,
-                   blocks_layer_name=None):
+                   blocks_layer_name=None,
+                   **kwargs):
         """
         Methods prepares the point support data from files.
 
         Parameters
         ----------
         point_support_data_file : str
-            Path to the file with point support data. Reads all files processed by the GeoPandas.
+            Path to the file with point support data. Reads all files
+            processed by the GeoPandas with appropriate extension such as ``.shp``,
+            ``.gpkg``, ``.feather``, or ``.parquet``.
 
         blocks_file : str
-            Path to the file with polygon data. Reads all files processed by GeoPandas.
+            Path to the file with polygon data. Reads all files processed
+            by GeoPandas with appropriate extension such as ``.shp``,
+        ``.gpkg``, ``.feather``, or ``.parquet``.
 
         point_support_geometry_col : Any
             The name of the point support geometry column.
 
         point_support_val_col : Any
             The name of the point support column with values.
 
@@ -330,25 +350,29 @@
             If set to ``False`` then the point support crs is transformed to the same crs as polygon dataset.
 
         point_support_layer_name : Any, default = None
             If provided file is *.gpkg* then this parameter must be provided.
 
         blocks_layer_name  : Any, default = None
             If provided file is *.gpkg* then this parameter must be provided.
+
+        **kwargs : Any
+            Additional kwargs parameters passed to the ``geopandas.read_file()``,
+            ``geopandas.read_feather()`` or ``geopandas.read_parquet()`` functions.
         """
         # Load data
-        if point_support_data_file.lower().endswith('.gpkg'):
-            point_support = gpd.read_file(point_support_data_file, layer=point_support_layer_name)
-        else:
-            point_support = gpd.read_file(point_support_data_file)
+        if point_support_layer_name is not None:
+            kwargs['layer'] = point_support_layer_name
+        point_support = _open_geopandas(Path(point_support_data_file), **kwargs)
 
-        if blocks_file.lower().endswith('.gpkg'):
-            blocks = gpd.read_file(blocks_file, layer=blocks_layer_name)
+        if blocks_layer_name is not None:
+            kwargs['layer'] = blocks_layer_name
         else:
-            blocks = gpd.read_file(blocks_file)
+            kwargs['layer'] = None
+        blocks = _open_geopandas(Path(blocks_file), **kwargs)
 
         self.from_geodataframes(point_support,
                                 blocks,
                                 point_support_val_col=point_support_val_col,
                                 blocks_geometry_col=blocks_geometry_col,
                                 blocks_index_col=blocks_index_col,
                                 point_support_geometry_col=point_support_geometry_col,
```

### Comparing `pyinterpolate-0.4.1/pyinterpolate/processing/select_values.py` & `pyinterpolate-0.4.2/pyinterpolate/processing/select_values.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/processing/transform/statistics.py` & `pyinterpolate-0.4.2/pyinterpolate/processing/transform/statistics.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/processing/transform/transform.py` & `pyinterpolate-0.4.2/pyinterpolate/processing/transform/transform.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/processing/utils/exceptions.py` & `pyinterpolate-0.4.2/pyinterpolate/processing/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/validation/cross_validation.py` & `pyinterpolate-0.4.2/pyinterpolate/validation/cross_validation.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/__init__.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/__init__.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/empirical/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/cloud.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/empirical/cloud.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/covariance.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/empirical/covariance.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/experimental_variogram.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/empirical/experimental_variogram.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/semivariance.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/empirical/semivariance.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/indicator/indicator_variogram.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/indicator/indicator_variogram.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/aggregated.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/aggregated.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/avg_block_to_block_semivariances.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/block/avg_block_to_block_semivariances.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/avg_inblock_semivariances.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/block/avg_inblock_semivariances.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/block_to_block_semivariance.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/block/block_to_block_semivariance.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/inblock_semivariance.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/block/inblock_semivariance.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/deconvolution.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/regularization/deconvolution.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/__init__.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/theoretical/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/models/variogram_models.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/theoretical/models/variogram_models.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/semivariogram.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/theoretical/semivariogram.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/spatial_dependency_index.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/theoretical/spatial_dependency_index.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/utils/exceptions.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/utils/metrics.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/variogram/utils/plots.py` & `pyinterpolate-0.4.2/pyinterpolate/variogram/utils/plots.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate/viz/raster.py` & `pyinterpolate-0.4.2/pyinterpolate/viz/raster.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate.egg-info/PKG-INFO` & `pyinterpolate-0.4.2/pyinterpolate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinterpolate
-Version: 0.4.1
+Version: 0.4.2
 Summary: Spatial Interpolation in Python
 Home-page: https://github.com/DataverseLabs/pyinterpolate
 Download-URL: https://github.com/DataverseLabs/pyinterpolate/archive/
 Author: Szymon Moliński
 Author-email: simon@dataverselabs.com
 License: BSD 3-clause
 Project-URL: Documentation, https://readthedocs.org/projects/pyinterpolate/
@@ -23,15 +23,15 @@
 
 ![status](https://joss.theoj.org/papers/3f87f562264c4e5174d9e6ed6d8812aa/status.svg) ![License](https://img.shields.io/github/license/szymon-datalions/pyinterpolate) ![Documentation Status](https://readthedocs.org/projects/pyinterpolate/badge/?version=latest) [![CodeFactor](https://www.codefactor.io/repository/github/dataverselabs/pyinterpolate/badge)](https://www.codefactor.io/repository/github/dataverselabs/pyinterpolate)
 
 ![Pyinterpolate](https://github.com/DataverseLabs/pyinterpolate/blob/main/logov04.jpg?raw=true  "Pyinterpolate logo")
 
 # Pyinterpolate
 
-**version 0.4.1** - *Kharkiv*
+**version 0.4.2** - *Kharkiv*
 
 ---
 
 Pyinterpolate is the Python library for **spatial statistics**. The package provides access to spatial statistics tools used in various studies. This package helps you **interpolate spatial data** with the *Kriging* technique.
 
 If you’re:
```

### Comparing `pyinterpolate-0.4.1/pyinterpolate.egg-info/SOURCES.txt` & `pyinterpolate-0.4.2/pyinterpolate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4.1/pyinterpolate.egg-info/requires.txt` & `pyinterpolate-0.4.2/pyinterpolate.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 descartes
 hdbscan
 matplotlib>=3.6
 prettytable>=3.3.0
 pyogrio
 rtree>=1.0.0
 shapely>=2.0.1
+pyarrow
 
 [:python_version <= "3.9"]
 numpy==1.21.2
 tqdm==4.64.0
 
 [:python_version == "3.7"]
 dask==2021.10.0
```

### Comparing `pyinterpolate-0.4.1/setup.cfg` & `pyinterpolate-0.4.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = pyinterpolate
 description = Spatial Interpolation in Python
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
-version = 0.4.1
+version = 0.4.2
 url = https://github.com/DataverseLabs/pyinterpolate
 download_url = https://github.com/DataverseLabs/pyinterpolate/archive/
 author = Szymon Moliński
 author_email = simon@dataverselabs.com
 license = BSD 3-clause
 classifiers = 
 	Development Status :: 4 - Beta
@@ -50,14 +50,15 @@
 	pyogrio
 	rtree>=1.0.0
 	shapely>=2.0.1
 	scipy>=1.9.0; python_version>='3.8'
 	scipy==1.7.3; python_version=='3.7'
 	tqdm>=4.64; python_version>'3.9'
 	tqdm==4.64.0; python_version<='3.9'
+	pyarrow
 
 [options.packages.find]
 exclude = 
 	tests*
 	tutorials*
 	new_concepts*
 	sample_data*
```

