# Comparing `tmp/buteo-0.9.1.tar.gz` & `tmp/buteo-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buteo-0.9.1.tar", last modified: Tue May  9 10:00:11 2023, max compression
+gzip compressed data, was "buteo-0.9.2.tar", last modified: Tue May  9 10:18:21 2023, max compression
```

## Comparing `buteo-0.9.1.tar` & `buteo-0.9.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1089 2023-03-07 09:20:18.869934 buteo-0.9.1/LICENSE
--rw-r--r--   0        0        0     4757 2023-05-02 12:41:19.141044 buteo-0.9.1/buteo/__init__.py
--rw-r--r--   0        0        0      220 2023-04-27 09:49:05.656052 buteo-0.9.1/buteo/ai/__init__.py
--rw-r--r--   0        0        0     9274 2023-05-02 11:43:21.384585 buteo-0.9.1/buteo/ai/augmentation.py
--rw-r--r--   0        0        0    28123 2023-05-02 12:32:55.881464 buteo-0.9.1/buteo/ai/augmentation_funcs.py
--rw-r--r--   0        0        0     5632 2023-04-28 10:13:19.277505 buteo-0.9.1/buteo/ai/augmentation_utils.py
--rw-r--r--   0        0        0    12666 2023-04-27 12:08:41.855227 buteo-0.9.1/buteo/ai/encoding.py
--rw-r--r--   0        0        0    13346 2023-04-27 12:10:59.465989 buteo-0.9.1/buteo/ai/scalers.py
--rw-r--r--   0        0        0     7952 2023-05-04 12:07:45.359917 buteo-0.9.1/buteo/ai/selection.py
--rw-r--r--   0        0        0      408 2023-05-03 11:12:45.284473 buteo-0.9.1/buteo/array/__init__.py
--rw-r--r--   0        0        0     5365 2023-05-02 12:17:14.771058 buteo-0.9.1/buteo/array/color.py
--rw-r--r--   0        0        0    16282 2023-05-05 12:25:08.221262 buteo-0.9.1/buteo/array/convolution.py
--rw-r--r--   0        0        0     3808 2023-05-08 13:11:10.703319 buteo-0.9.1/buteo/array/convolution_distance.py
--rw-r--r--   0        0        0    12279 2023-04-30 17:19:03.247105 buteo-0.9.1/buteo/array/convolution_funcs.py
--rw-r--r--   0        0        0    15308 2023-05-03 14:21:39.376562 buteo-0.9.1/buteo/array/convolution_kernels.py
--rw-r--r--   0        0        0     2634 2023-05-03 14:18:12.376178 buteo-0.9.1/buteo/array/edge_detection.py
--rw-r--r--   0        0        0     4090 2023-05-03 14:09:36.372639 buteo-0.9.1/buteo/array/fill.py
--rw-r--r--   0        0        0    10639 2023-05-05 12:27:09.566352 buteo-0.9.1/buteo/array/filters.py
--rw-r--r--   0        0        0     7902 2023-05-05 12:33:39.152123 buteo-0.9.1/buteo/array/morphology.py
--rw-r--r--   0        0        0    31020 2023-05-03 14:24:10.280152 buteo-0.9.1/buteo/array/patches.py
--rw-r--r--   0        0        0     2513 2023-05-03 14:16:07.383138 buteo-0.9.1/buteo/array/timeseries.py
--rw-r--r--   0        0        0     2861 2023-05-01 15:16:23.098217 buteo-0.9.1/buteo/array/utils_array.py
--rw-r--r--   0        0        0      155 2023-04-12 12:14:08.281651 buteo-0.9.1/buteo/eo/__init__.py
--rw-r--r--   0        0        0     5677 2022-08-16 15:39:47.000000 buteo-0.9.1/buteo/eo/graphs/L2A_GIPP.xml
--rw-r--r--   0        0        0     3552 2022-08-16 15:39:47.000000 buteo-0.9.1/buteo/eo/graphs/step_01_backstatter.xml
--rw-r--r--   0        0        0    12077 2022-08-16 15:39:47.000000 buteo-0.9.1/buteo/eo/graphs/step_01_coherence.xml
--rw-r--r--   0        0        0     3572 2022-08-16 15:39:47.000000 buteo-0.9.1/buteo/eo/graphs/step_02_backscatter.xml
--rw-r--r--   0        0        0     4299 2022-08-16 15:39:47.000000 buteo-0.9.1/buteo/eo/graphs/step_02_backscatter_speckle.xml
--rw-r--r--   0        0        0     3712 2022-08-16 15:39:47.000000 buteo-0.9.1/buteo/eo/graphs/step_02_coherence.xml
--rw-r--r--   0        0        0    10510 2023-05-08 18:31:03.565806 buteo-0.9.1/buteo/eo/s1_preprocess.py
--rw-r--r--   0        0        0     2133 2023-05-03 09:56:32.765943 buteo-0.9.1/buteo/eo/s1_utils.py
--rw-r--r--   0        0        0     9188 2023-05-03 09:56:39.496000 buteo-0.9.1/buteo/eo/s2_indices.py
--rw-r--r--   0        0        0    12465 2023-05-08 15:14:09.972611 buteo-0.9.1/buteo/eo/s2_utils.py
--rw-r--r--   0        0        0      497 2023-05-05 06:20:35.014620 buteo-0.9.1/buteo/raster/__init__.py
--rw-r--r--   0        0        0    16663 2023-05-08 13:09:19.688308 buteo-0.9.1/buteo/raster/align.py
--rw-r--r--   0        0        0     7299 2023-05-05 17:25:56.416262 buteo-0.9.1/buteo/raster/borders.py
--rw-r--r--   0        0        0    13523 2023-05-08 15:16:27.420173 buteo-0.9.1/buteo/raster/clip.py
--rw-r--r--   0        0        0     1510 2023-05-08 06:54:59.813075 buteo-0.9.1/buteo/raster/coordinates.py
--rw-r--r--   0        0        0     9674 2023-05-05 10:46:19.677097 buteo-0.9.1/buteo/raster/core_offsets.py
--rw-r--r--   0        0        0    18427 2023-05-08 14:45:50.472324 buteo-0.9.1/buteo/raster/core_raster.py
--rw-r--r--   0        0        0    36962 2023-05-09 09:58:23.625148 buteo-0.9.1/buteo/raster/core_raster_io.py
--rw-r--r--   0        0        0    10157 2023-05-05 12:25:08.222263 buteo-0.9.1/buteo/raster/core_stack.py
--rw-r--r--   0        0        0     7431 2023-05-08 07:41:05.893227 buteo-0.9.1/buteo/raster/datatype.py
--rw-r--r--   0        0        0     8331 2023-05-08 08:18:57.689620 buteo-0.9.1/buteo/raster/dem.py
--rw-r--r--   0        0        0     6231 2023-05-08 07:52:34.295257 buteo-0.9.1/buteo/raster/grid.py
--rw-r--r--   0        0        0     4079 2023-05-08 13:07:43.602719 buteo-0.9.1/buteo/raster/metadata.py
--rw-r--r--   0        0        0     8386 2023-05-08 09:51:45.634002 buteo-0.9.1/buteo/raster/nodata.py
--rw-r--r--   0        0        0     6167 2023-05-08 13:49:35.641110 buteo-0.9.1/buteo/raster/proximity.py
--rw-r--r--   0        0        0     9300 2023-05-08 11:56:10.990154 buteo-0.9.1/buteo/raster/reproject.py
--rw-r--r--   0        0        0    10673 2023-05-08 13:04:45.244156 buteo-0.9.1/buteo/raster/resample.py
--rw-r--r--   0        0        0     8041 2023-05-08 13:37:41.583753 buteo-0.9.1/buteo/raster/shift.py
--rw-r--r--   0        0        0     4318 2023-05-08 13:48:24.329191 buteo-0.9.1/buteo/raster/vectorize.py
--rw-r--r--   0        0        0      298 2023-05-03 14:19:58.866941 buteo-0.9.1/buteo/utils/__init__.py
--rw-r--r--   0        0        0     4536 2023-05-05 12:25:22.517045 buteo-0.9.1/buteo/utils/utils_aux.py
--rw-r--r--   0        0        0     9459 2023-05-05 12:26:38.230306 buteo-0.9.1/buteo/utils/utils_base.py
--rw-r--r--   0        0        0    33937 2023-05-07 07:53:13.792610 buteo-0.9.1/buteo/utils/utils_bbox.py
--rw-r--r--   0        0        0    28852 2023-05-09 07:50:41.612053 buteo-0.9.1/buteo/utils/utils_gdal.py
--rw-r--r--   0        0        0     8668 2023-05-08 10:00:37.380883 buteo-0.9.1/buteo/utils/utils_io.py
--rw-r--r--   0        0        0    28485 2023-05-08 09:46:50.435511 buteo-0.9.1/buteo/utils/utils_path.py
--rw-r--r--   0        0        0    18880 2023-05-08 14:44:59.714163 buteo-0.9.1/buteo/utils/utils_projection.py
--rw-r--r--   0        0        0    16670 2023-05-09 09:57:09.207943 buteo-0.9.1/buteo/utils/utils_translate.py
--rw-r--r--   0        0        0      377 2023-05-08 15:17:25.536089 buteo-0.9.1/buteo/vector/__init__.py
--rw-r--r--   0        0        0     5661 2023-05-09 08:20:47.551957 buteo-0.9.1/buteo/vector/buffer.py
--rw-r--r--   0        0        0     6639 2023-05-09 08:45:14.629449 buteo-0.9.1/buteo/vector/clip.py
--rw-r--r--   0        0        0    13506 2023-05-08 15:13:20.210020 buteo-0.9.1/buteo/vector/convert_parts.py
--rw-r--r--   0        0        0    24435 2023-05-09 08:19:00.716883 buteo-0.9.1/buteo/vector/core_vector.py
--rw-r--r--   0        0        0     6187 2023-05-08 15:13:20.210020 buteo-0.9.1/buteo/vector/dissolve.py
--rw-r--r--   0        0        0      263 2023-05-02 12:27:13.705244 buteo-0.9.1/buteo/vector/grid.py
--rw-r--r--   0        0        0     6529 2023-05-08 15:13:20.210020 buteo-0.9.1/buteo/vector/intersect.py
--rw-r--r--   0        0        0     1926 2023-05-08 15:13:20.210020 buteo-0.9.1/buteo/vector/merge.py
--rw-r--r--   0        0        0     7523 2023-05-08 15:13:20.210020 buteo-0.9.1/buteo/vector/metadata.py
--rw-r--r--   0        0        0     6936 2023-05-08 15:13:20.218015 buteo-0.9.1/buteo/vector/rasterize.py
--rw-r--r--   0        0        0     4870 2023-05-09 09:04:48.200349 buteo-0.9.1/buteo/vector/reproject.py
--rw-r--r--   0        0        0     6973 2023-05-08 15:13:20.210020 buteo-0.9.1/buteo/vector/shapes.py
--rw-r--r--   0        0        0     2637 2023-05-09 08:37:35.507047 buteo-0.9.1/buteo/vector/split.py
--rw-r--r--   0        0        0    18080 2023-05-08 07:22:45.435592 buteo-0.9.1/buteo/vector/zonal_statistics.py
--rw-r--r--   0        0        0      785 2023-05-09 09:58:51.817755 buteo-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4710 2023-04-23 13:45:46.888099 buteo-0.9.1/readme.md
--rw-r--r--   0        0        0     5170 1970-01-01 00:00:00.000000 buteo-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-03-07 09:20:18.869934 buteo-0.9.2/LICENSE
+-rw-r--r--   0        0        0     4757 2023-05-02 12:41:19.141044 buteo-0.9.2/buteo/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-27 09:49:05.656052 buteo-0.9.2/buteo/ai/__init__.py
+-rw-r--r--   0        0        0     9274 2023-05-02 11:43:21.384585 buteo-0.9.2/buteo/ai/augmentation.py
+-rw-r--r--   0        0        0    28123 2023-05-02 12:32:55.881464 buteo-0.9.2/buteo/ai/augmentation_funcs.py
+-rw-r--r--   0        0        0     5632 2023-04-28 10:13:19.277505 buteo-0.9.2/buteo/ai/augmentation_utils.py
+-rw-r--r--   0        0        0    12666 2023-04-27 12:08:41.855227 buteo-0.9.2/buteo/ai/encoding.py
+-rw-r--r--   0        0        0    13346 2023-04-27 12:10:59.465989 buteo-0.9.2/buteo/ai/scalers.py
+-rw-r--r--   0        0        0     7952 2023-05-04 12:07:45.359917 buteo-0.9.2/buteo/ai/selection.py
+-rw-r--r--   0        0        0      408 2023-05-03 11:12:45.284473 buteo-0.9.2/buteo/array/__init__.py
+-rw-r--r--   0        0        0     5365 2023-05-02 12:17:14.771058 buteo-0.9.2/buteo/array/color.py
+-rw-r--r--   0        0        0    16282 2023-05-05 12:25:08.221262 buteo-0.9.2/buteo/array/convolution.py
+-rw-r--r--   0        0        0     3808 2023-05-08 13:11:10.703319 buteo-0.9.2/buteo/array/convolution_distance.py
+-rw-r--r--   0        0        0    12279 2023-04-30 17:19:03.247105 buteo-0.9.2/buteo/array/convolution_funcs.py
+-rw-r--r--   0        0        0    15308 2023-05-03 14:21:39.376562 buteo-0.9.2/buteo/array/convolution_kernels.py
+-rw-r--r--   0        0        0     2634 2023-05-03 14:18:12.376178 buteo-0.9.2/buteo/array/edge_detection.py
+-rw-r--r--   0        0        0     4090 2023-05-03 14:09:36.372639 buteo-0.9.2/buteo/array/fill.py
+-rw-r--r--   0        0        0    10639 2023-05-05 12:27:09.566352 buteo-0.9.2/buteo/array/filters.py
+-rw-r--r--   0        0        0     7902 2023-05-05 12:33:39.152123 buteo-0.9.2/buteo/array/morphology.py
+-rw-r--r--   0        0        0    31020 2023-05-03 14:24:10.280152 buteo-0.9.2/buteo/array/patches.py
+-rw-r--r--   0        0        0     2513 2023-05-03 14:16:07.383138 buteo-0.9.2/buteo/array/timeseries.py
+-rw-r--r--   0        0        0     2861 2023-05-01 15:16:23.098217 buteo-0.9.2/buteo/array/utils_array.py
+-rw-r--r--   0        0        0      155 2023-04-12 12:14:08.281651 buteo-0.9.2/buteo/eo/__init__.py
+-rw-r--r--   0        0        0     5677 2022-08-16 15:39:47.000000 buteo-0.9.2/buteo/eo/graphs/L2A_GIPP.xml
+-rw-r--r--   0        0        0     3552 2022-08-16 15:39:47.000000 buteo-0.9.2/buteo/eo/graphs/step_01_backstatter.xml
+-rw-r--r--   0        0        0    12077 2022-08-16 15:39:47.000000 buteo-0.9.2/buteo/eo/graphs/step_01_coherence.xml
+-rw-r--r--   0        0        0     3572 2022-08-16 15:39:47.000000 buteo-0.9.2/buteo/eo/graphs/step_02_backscatter.xml
+-rw-r--r--   0        0        0     4299 2022-08-16 15:39:47.000000 buteo-0.9.2/buteo/eo/graphs/step_02_backscatter_speckle.xml
+-rw-r--r--   0        0        0     3712 2022-08-16 15:39:47.000000 buteo-0.9.2/buteo/eo/graphs/step_02_coherence.xml
+-rw-r--r--   0        0        0    10510 2023-05-08 18:31:03.565806 buteo-0.9.2/buteo/eo/s1_preprocess.py
+-rw-r--r--   0        0        0     2133 2023-05-03 09:56:32.765943 buteo-0.9.2/buteo/eo/s1_utils.py
+-rw-r--r--   0        0        0     9188 2023-05-03 09:56:39.496000 buteo-0.9.2/buteo/eo/s2_indices.py
+-rw-r--r--   0        0        0    12465 2023-05-08 15:14:09.972611 buteo-0.9.2/buteo/eo/s2_utils.py
+-rw-r--r--   0        0        0      497 2023-05-05 06:20:35.014620 buteo-0.9.2/buteo/raster/__init__.py
+-rw-r--r--   0        0        0    16663 2023-05-08 13:09:19.688308 buteo-0.9.2/buteo/raster/align.py
+-rw-r--r--   0        0        0     7299 2023-05-05 17:25:56.416262 buteo-0.9.2/buteo/raster/borders.py
+-rw-r--r--   0        0        0    13523 2023-05-08 15:16:27.420173 buteo-0.9.2/buteo/raster/clip.py
+-rw-r--r--   0        0        0     1510 2023-05-08 06:54:59.813075 buteo-0.9.2/buteo/raster/coordinates.py
+-rw-r--r--   0        0        0     9674 2023-05-05 10:46:19.677097 buteo-0.9.2/buteo/raster/core_offsets.py
+-rw-r--r--   0        0        0    18427 2023-05-08 14:45:50.472324 buteo-0.9.2/buteo/raster/core_raster.py
+-rw-r--r--   0        0        0    36962 2023-05-09 09:58:23.625148 buteo-0.9.2/buteo/raster/core_raster_io.py
+-rw-r--r--   0        0        0    10157 2023-05-05 12:25:08.222263 buteo-0.9.2/buteo/raster/core_stack.py
+-rw-r--r--   0        0        0     7431 2023-05-08 07:41:05.893227 buteo-0.9.2/buteo/raster/datatype.py
+-rw-r--r--   0        0        0     8331 2023-05-08 08:18:57.689620 buteo-0.9.2/buteo/raster/dem.py
+-rw-r--r--   0        0        0     6231 2023-05-08 07:52:34.295257 buteo-0.9.2/buteo/raster/grid.py
+-rw-r--r--   0        0        0     4079 2023-05-08 13:07:43.602719 buteo-0.9.2/buteo/raster/metadata.py
+-rw-r--r--   0        0        0     8386 2023-05-08 09:51:45.634002 buteo-0.9.2/buteo/raster/nodata.py
+-rw-r--r--   0        0        0     6167 2023-05-08 13:49:35.641110 buteo-0.9.2/buteo/raster/proximity.py
+-rw-r--r--   0        0        0     9300 2023-05-08 11:56:10.990154 buteo-0.9.2/buteo/raster/reproject.py
+-rw-r--r--   0        0        0    10673 2023-05-08 13:04:45.244156 buteo-0.9.2/buteo/raster/resample.py
+-rw-r--r--   0        0        0     8041 2023-05-08 13:37:41.583753 buteo-0.9.2/buteo/raster/shift.py
+-rw-r--r--   0        0        0     4318 2023-05-08 13:48:24.329191 buteo-0.9.2/buteo/raster/vectorize.py
+-rw-r--r--   0        0        0      298 2023-05-03 14:19:58.866941 buteo-0.9.2/buteo/utils/__init__.py
+-rw-r--r--   0        0        0     4536 2023-05-05 12:25:22.517045 buteo-0.9.2/buteo/utils/utils_aux.py
+-rw-r--r--   0        0        0     9459 2023-05-05 12:26:38.230306 buteo-0.9.2/buteo/utils/utils_base.py
+-rw-r--r--   0        0        0    33937 2023-05-07 07:53:13.792610 buteo-0.9.2/buteo/utils/utils_bbox.py
+-rw-r--r--   0        0        0    28852 2023-05-09 07:50:41.612053 buteo-0.9.2/buteo/utils/utils_gdal.py
+-rw-r--r--   0        0        0     8668 2023-05-08 10:00:37.380883 buteo-0.9.2/buteo/utils/utils_io.py
+-rw-r--r--   0        0        0    28485 2023-05-08 09:46:50.435511 buteo-0.9.2/buteo/utils/utils_path.py
+-rw-r--r--   0        0        0    18880 2023-05-08 14:44:59.714163 buteo-0.9.2/buteo/utils/utils_projection.py
+-rw-r--r--   0        0        0    16744 2023-05-09 10:16:56.513576 buteo-0.9.2/buteo/utils/utils_translate.py
+-rw-r--r--   0        0        0      377 2023-05-08 15:17:25.536089 buteo-0.9.2/buteo/vector/__init__.py
+-rw-r--r--   0        0        0     5661 2023-05-09 08:20:47.551957 buteo-0.9.2/buteo/vector/buffer.py
+-rw-r--r--   0        0        0     6639 2023-05-09 08:45:14.629449 buteo-0.9.2/buteo/vector/clip.py
+-rw-r--r--   0        0        0    13506 2023-05-08 15:13:20.210020 buteo-0.9.2/buteo/vector/convert_parts.py
+-rw-r--r--   0        0        0    24435 2023-05-09 08:19:00.716883 buteo-0.9.2/buteo/vector/core_vector.py
+-rw-r--r--   0        0        0     6187 2023-05-08 15:13:20.210020 buteo-0.9.2/buteo/vector/dissolve.py
+-rw-r--r--   0        0        0      263 2023-05-02 12:27:13.705244 buteo-0.9.2/buteo/vector/grid.py
+-rw-r--r--   0        0        0     6529 2023-05-08 15:13:20.210020 buteo-0.9.2/buteo/vector/intersect.py
+-rw-r--r--   0        0        0     1926 2023-05-08 15:13:20.210020 buteo-0.9.2/buteo/vector/merge.py
+-rw-r--r--   0        0        0     7523 2023-05-08 15:13:20.210020 buteo-0.9.2/buteo/vector/metadata.py
+-rw-r--r--   0        0        0     6936 2023-05-08 15:13:20.218015 buteo-0.9.2/buteo/vector/rasterize.py
+-rw-r--r--   0        0        0     4870 2023-05-09 09:04:48.200349 buteo-0.9.2/buteo/vector/reproject.py
+-rw-r--r--   0        0        0     6973 2023-05-08 15:13:20.210020 buteo-0.9.2/buteo/vector/shapes.py
+-rw-r--r--   0        0        0     2637 2023-05-09 08:37:35.507047 buteo-0.9.2/buteo/vector/split.py
+-rw-r--r--   0        0        0    18080 2023-05-08 07:22:45.435592 buteo-0.9.2/buteo/vector/zonal_statistics.py
+-rw-r--r--   0        0        0      785 2023-05-09 10:12:35.307994 buteo-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4710 2023-04-23 13:45:46.888099 buteo-0.9.2/readme.md
+-rw-r--r--   0        0        0     5170 1970-01-01 00:00:00.000000 buteo-0.9.2/PKG-INFO
```

### Comparing `buteo-0.9.1/LICENSE` & `buteo-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/__init__.py` & `buteo-0.9.2/buteo/__init__.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/ai/augmentation.py` & `buteo-0.9.2/buteo/ai/augmentation.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/ai/augmentation_funcs.py` & `buteo-0.9.2/buteo/ai/augmentation_funcs.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/ai/augmentation_utils.py` & `buteo-0.9.2/buteo/ai/augmentation_utils.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/ai/encoding.py` & `buteo-0.9.2/buteo/ai/encoding.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/ai/scalers.py` & `buteo-0.9.2/buteo/ai/scalers.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/ai/selection.py` & `buteo-0.9.2/buteo/ai/selection.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/array/color.py` & `buteo-0.9.2/buteo/array/color.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/array/convolution.py` & `buteo-0.9.2/buteo/array/convolution.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/array/convolution_distance.py` & `buteo-0.9.2/buteo/array/convolution_distance.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/array/convolution_funcs.py` & `buteo-0.9.2/buteo/array/convolution_funcs.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/array/convolution_kernels.py` & `buteo-0.9.2/buteo/array/convolution_kernels.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/array/edge_detection.py` & `buteo-0.9.2/buteo/array/edge_detection.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/array/fill.py` & `buteo-0.9.2/buteo/array/fill.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/array/filters.py` & `buteo-0.9.2/buteo/array/filters.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/array/morphology.py` & `buteo-0.9.2/buteo/array/morphology.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/array/patches.py` & `buteo-0.9.2/buteo/array/patches.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/array/timeseries.py` & `buteo-0.9.2/buteo/array/timeseries.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/array/utils_array.py` & `buteo-0.9.2/buteo/array/utils_array.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/eo/graphs/L2A_GIPP.xml` & `buteo-0.9.2/buteo/eo/graphs/L2A_GIPP.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/eo/graphs/step_01_backstatter.xml` & `buteo-0.9.2/buteo/eo/graphs/step_01_backstatter.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/eo/graphs/step_01_coherence.xml` & `buteo-0.9.2/buteo/eo/graphs/step_01_coherence.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/eo/graphs/step_02_backscatter.xml` & `buteo-0.9.2/buteo/eo/graphs/step_02_backscatter.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/eo/graphs/step_02_backscatter_speckle.xml` & `buteo-0.9.2/buteo/eo/graphs/step_02_backscatter_speckle.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/eo/graphs/step_02_coherence.xml` & `buteo-0.9.2/buteo/eo/graphs/step_02_coherence.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/eo/s1_preprocess.py` & `buteo-0.9.2/buteo/eo/s1_preprocess.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/eo/s1_utils.py` & `buteo-0.9.2/buteo/eo/s1_utils.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/eo/s2_indices.py` & `buteo-0.9.2/buteo/eo/s2_indices.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/eo/s2_utils.py` & `buteo-0.9.2/buteo/eo/s2_utils.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/align.py` & `buteo-0.9.2/buteo/raster/align.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/borders.py` & `buteo-0.9.2/buteo/raster/borders.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/clip.py` & `buteo-0.9.2/buteo/raster/clip.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/coordinates.py` & `buteo-0.9.2/buteo/raster/coordinates.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/core_offsets.py` & `buteo-0.9.2/buteo/raster/core_offsets.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/core_raster.py` & `buteo-0.9.2/buteo/raster/core_raster.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/core_raster_io.py` & `buteo-0.9.2/buteo/raster/core_raster_io.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/core_stack.py` & `buteo-0.9.2/buteo/raster/core_stack.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/datatype.py` & `buteo-0.9.2/buteo/raster/datatype.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/dem.py` & `buteo-0.9.2/buteo/raster/dem.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/grid.py` & `buteo-0.9.2/buteo/raster/grid.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/metadata.py` & `buteo-0.9.2/buteo/raster/metadata.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/nodata.py` & `buteo-0.9.2/buteo/raster/nodata.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/proximity.py` & `buteo-0.9.2/buteo/raster/proximity.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/reproject.py` & `buteo-0.9.2/buteo/raster/reproject.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/resample.py` & `buteo-0.9.2/buteo/raster/resample.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/shift.py` & `buteo-0.9.2/buteo/raster/shift.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/raster/vectorize.py` & `buteo-0.9.2/buteo/raster/vectorize.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/utils/utils_aux.py` & `buteo-0.9.2/buteo/utils/utils_aux.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/utils/utils_base.py` & `buteo-0.9.2/buteo/utils/utils_base.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/utils/utils_bbox.py` & `buteo-0.9.2/buteo/utils/utils_bbox.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/utils/utils_gdal.py` & `buteo-0.9.2/buteo/utils/utils_gdal.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/utils/utils_io.py` & `buteo-0.9.2/buteo/utils/utils_io.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/utils/utils_path.py` & `buteo-0.9.2/buteo/utils/utils_path.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/utils/utils_projection.py` & `buteo-0.9.2/buteo/utils/utils_projection.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/utils/utils_translate.py` & `buteo-0.9.2/buteo/utils/utils_translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -581,16 +581,17 @@
     assert isinstance(target_dtype, (str, np.dtype, type(np.int8))), "target_dtype must be a string or numpy dtype."
 
     target_dtype = _parse_dtype(target_dtype)
 
     if arr.dtype == target_dtype:
         return arr
 
+    min_val, max_val = _get_range_for_numpy_datatype(target_dtype.name)
     outarr = np.zeros(arr.shape, dtype=target_dtype)
 
     if _check_is_int_numpy_dtype(target_dtype) and not _check_is_int_numpy_dtype(arr.dtype):
-        arr = np.rint(arr)
-
-    min_val, max_val = _get_range_for_numpy_datatype(target_dtype.name)
-    outarr = np.clip(outarr, min_val, max_val)
+        outarr[:] = np.rint(arr)
+        np.clip(outarr, min_val, max_val, out=outarr)
+    else:
+        np.clip(arr, min_val, max_val, out=outarr)
 
     return outarr
```

### Comparing `buteo-0.9.1/buteo/vector/buffer.py` & `buteo-0.9.2/buteo/vector/buffer.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/vector/clip.py` & `buteo-0.9.2/buteo/vector/clip.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/vector/convert_parts.py` & `buteo-0.9.2/buteo/vector/convert_parts.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/vector/core_vector.py` & `buteo-0.9.2/buteo/vector/core_vector.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/vector/dissolve.py` & `buteo-0.9.2/buteo/vector/dissolve.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/vector/intersect.py` & `buteo-0.9.2/buteo/vector/intersect.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/vector/merge.py` & `buteo-0.9.2/buteo/vector/merge.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/vector/metadata.py` & `buteo-0.9.2/buteo/vector/metadata.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/vector/rasterize.py` & `buteo-0.9.2/buteo/vector/rasterize.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/vector/reproject.py` & `buteo-0.9.2/buteo/vector/reproject.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/vector/shapes.py` & `buteo-0.9.2/buteo/vector/shapes.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/vector/split.py` & `buteo-0.9.2/buteo/vector/split.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/buteo/vector/zonal_statistics.py` & `buteo-0.9.2/buteo/vector/zonal_statistics.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/pyproject.toml` & `buteo-0.9.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.8.0", "numba>=0.56.4", "psutil>=5.4.8", "PyYAML>=6.0", "tqdm>=4.62.3"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "buteo"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
   { name="Casper Fibaek", email="casperfibaek@gmail.com" },
 ]
 description = "Tools for merging Geospatial Analysis and AI."
 readme = "readme.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `buteo-0.9.1/readme.md` & `buteo-0.9.2/readme.md`

 * *Files identical despite different names*

### Comparing `buteo-0.9.1/PKG-INFO` & `buteo-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buteo
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tools for merging Geospatial Analysis and AI.
 Author-email: Casper Fibaek <casperfibaek@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

