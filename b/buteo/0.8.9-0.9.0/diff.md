# Comparing `tmp/buteo-0.8.9.tar.gz` & `tmp/buteo-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buteo-0.8.9.tar", last modified: Wed Mar 29 07:28:58 2023, max compression
+gzip compressed data, was "buteo-0.9.0.tar", last modified: Tue May  9 09:18:29 2023, max compression
```

## Comparing `buteo-0.8.9.tar` & `buteo-0.9.0.tar`

### file list

```diff
@@ -1,42 +1,79 @@
--rw-r--r--   0        0        0     1089 2023-03-07 09:20:18.869934 buteo-0.8.9/LICENSE
--rw-r--r--   0        0        0     5317 2023-03-01 11:05:54.186351 buteo-0.8.9/buteo/__init__.py
--rw-r--r--   0        0        0      468 2023-03-01 11:05:54.186351 buteo-0.8.9/buteo/raster/__init__.py
--rw-r--r--   0        0        0    19904 2023-03-28 08:02:37.301571 buteo-0.8.9/buteo/raster/align.py
--rw-r--r--   0        0        0     6007 2023-03-28 08:02:37.303564 buteo-0.8.9/buteo/raster/borders.py
--rw-r--r--   0        0        0    11138 2023-03-28 08:02:37.304561 buteo-0.8.9/buteo/raster/clip.py
--rw-r--r--   0        0        0    18866 2023-03-28 08:02:37.306554 buteo-0.8.9/buteo/raster/convolution.py
--rw-r--r--   0        0        0    46535 2023-03-29 07:16:39.554091 buteo-0.8.9/buteo/raster/core_raster.py
--rw-r--r--   0        0        0    10456 2023-03-19 10:08:16.444601 buteo-0.8.9/buteo/raster/edge_detection.py
--rw-r--r--   0        0        0     5849 2023-03-01 11:05:54.186351 buteo-0.8.9/buteo/raster/grid.py
--rw-r--r--   0        0        0     3925 2023-03-01 11:05:54.186351 buteo-0.8.9/buteo/raster/morphology.py
--rw-r--r--   0        0        0    14410 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/raster/nodata.py
--rw-r--r--   0        0        0     6657 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/raster/patches.py
--rw-r--r--   0        0        0     6345 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/raster/proximity.py
--rw-r--r--   0        0        0     6526 2023-03-20 12:24:41.883749 buteo-0.8.9/buteo/raster/reproject.py
--rw-r--r--   0        0        0     7297 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/raster/resample.py
--rw-r--r--   0        0        0     4969 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/raster/shift.py
--rw-r--r--   0        0        0    12567 2023-03-29 07:16:39.555089 buteo-0.8.9/buteo/raster/textures.py
--rw-r--r--   0        0        0     1695 2023-03-08 16:28:04.339458 buteo-0.8.9/buteo/raster/timeseries.py
--rw-r--r--   0        0        0     3270 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/raster/vectorize.py
--rw-r--r--   0        0        0    11486 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/raster/warp.py
--rw-r--r--   0        0        0      208 2023-03-07 09:11:46.578377 buteo-0.8.9/buteo/utils/__init__.py
--rw-r--r--   0        0        0    14870 2023-03-29 07:24:39.870805 buteo-0.8.9/buteo/utils/aux_utils.py
--rw-r--r--   0        0        0    33225 2023-03-24 10:39:57.083854 buteo-0.8.9/buteo/utils/bbox_utils.py
--rw-r--r--   0        0        0    25947 2023-03-20 13:19:38.324677 buteo-0.8.9/buteo/utils/core_utils.py
--rw-r--r--   0        0        0    12683 2023-03-17 12:52:44.388017 buteo-0.8.9/buteo/utils/gdal_enums.py
--rw-r--r--   0        0        0    46819 2023-03-29 07:16:39.556084 buteo-0.8.9/buteo/utils/gdal_utils.py
--rw-r--r--   0        0        0      307 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/vector/__init__.py
--rw-r--r--   0        0        0     4258 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/vector/buffer.py
--rw-r--r--   0        0        0     6193 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/vector/clip.py
--rw-r--r--   0        0        0    12800 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/vector/convert_parts.py
--rw-r--r--   0        0        0    26159 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/vector/core_vector.py
--rw-r--r--   0        0        0     5146 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/vector/dissolve.py
--rw-r--r--   0        0        0      252 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/vector/grid.py
--rw-r--r--   0        0        0     6010 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/vector/intersect.py
--rw-r--r--   0        0        0     1777 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/vector/merge.py
--rw-r--r--   0        0        0     6185 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/vector/rasterize.py
--rw-r--r--   0        0        0     4388 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/vector/reproject.py
--rw-r--r--   0        0        0    18077 2023-03-01 11:05:54.201974 buteo-0.8.9/buteo/vector/zonal_statistics.py
--rw-r--r--   0        0        0      759 2023-03-29 07:25:59.882123 buteo-0.8.9/pyproject.toml
--rw-r--r--   0        0        0     5342 2023-03-01 11:05:54.286108 buteo-0.8.9/readme.md
--rw-r--r--   0        0        0     5768 1970-01-01 00:00:00.000000 buteo-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-03-07 09:20:18.869934 buteo-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4757 2023-05-02 12:41:19.141044 buteo-0.9.0/buteo/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-27 09:49:05.656052 buteo-0.9.0/buteo/ai/__init__.py
+-rw-r--r--   0        0        0     9274 2023-05-02 11:43:21.384585 buteo-0.9.0/buteo/ai/augmentation.py
+-rw-r--r--   0        0        0    28123 2023-05-02 12:32:55.881464 buteo-0.9.0/buteo/ai/augmentation_funcs.py
+-rw-r--r--   0        0        0     5632 2023-04-28 10:13:19.277505 buteo-0.9.0/buteo/ai/augmentation_utils.py
+-rw-r--r--   0        0        0    12666 2023-04-27 12:08:41.855227 buteo-0.9.0/buteo/ai/encoding.py
+-rw-r--r--   0        0        0    13346 2023-04-27 12:10:59.465989 buteo-0.9.0/buteo/ai/scalers.py
+-rw-r--r--   0        0        0     7952 2023-05-04 12:07:45.359917 buteo-0.9.0/buteo/ai/selection.py
+-rw-r--r--   0        0        0      408 2023-05-03 11:12:45.284473 buteo-0.9.0/buteo/array/__init__.py
+-rw-r--r--   0        0        0     5365 2023-05-02 12:17:14.771058 buteo-0.9.0/buteo/array/color.py
+-rw-r--r--   0        0        0    16282 2023-05-05 12:25:08.221262 buteo-0.9.0/buteo/array/convolution.py
+-rw-r--r--   0        0        0     3808 2023-05-08 13:11:10.703319 buteo-0.9.0/buteo/array/convolution_distance.py
+-rw-r--r--   0        0        0    12279 2023-04-30 17:19:03.247105 buteo-0.9.0/buteo/array/convolution_funcs.py
+-rw-r--r--   0        0        0    15308 2023-05-03 14:21:39.376562 buteo-0.9.0/buteo/array/convolution_kernels.py
+-rw-r--r--   0        0        0     2634 2023-05-03 14:18:12.376178 buteo-0.9.0/buteo/array/edge_detection.py
+-rw-r--r--   0        0        0     4090 2023-05-03 14:09:36.372639 buteo-0.9.0/buteo/array/fill.py
+-rw-r--r--   0        0        0    10639 2023-05-05 12:27:09.566352 buteo-0.9.0/buteo/array/filters.py
+-rw-r--r--   0        0        0     7902 2023-05-05 12:33:39.152123 buteo-0.9.0/buteo/array/morphology.py
+-rw-r--r--   0        0        0    31020 2023-05-03 14:24:10.280152 buteo-0.9.0/buteo/array/patches.py
+-rw-r--r--   0        0        0     2513 2023-05-03 14:16:07.383138 buteo-0.9.0/buteo/array/timeseries.py
+-rw-r--r--   0        0        0     2861 2023-05-01 15:16:23.098217 buteo-0.9.0/buteo/array/utils_array.py
+-rw-r--r--   0        0        0      155 2023-04-12 12:14:08.281651 buteo-0.9.0/buteo/eo/__init__.py
+-rw-r--r--   0        0        0     5677 2022-08-16 15:39:47.000000 buteo-0.9.0/buteo/eo/graphs/L2A_GIPP.xml
+-rw-r--r--   0        0        0     3552 2022-08-16 15:39:47.000000 buteo-0.9.0/buteo/eo/graphs/step_01_backstatter.xml
+-rw-r--r--   0        0        0    12077 2022-08-16 15:39:47.000000 buteo-0.9.0/buteo/eo/graphs/step_01_coherence.xml
+-rw-r--r--   0        0        0     3572 2022-08-16 15:39:47.000000 buteo-0.9.0/buteo/eo/graphs/step_02_backscatter.xml
+-rw-r--r--   0        0        0     4299 2022-08-16 15:39:47.000000 buteo-0.9.0/buteo/eo/graphs/step_02_backscatter_speckle.xml
+-rw-r--r--   0        0        0     3712 2022-08-16 15:39:47.000000 buteo-0.9.0/buteo/eo/graphs/step_02_coherence.xml
+-rw-r--r--   0        0        0    10510 2023-05-08 18:31:03.565806 buteo-0.9.0/buteo/eo/s1_preprocess.py
+-rw-r--r--   0        0        0     2133 2023-05-03 09:56:32.765943 buteo-0.9.0/buteo/eo/s1_utils.py
+-rw-r--r--   0        0        0     9188 2023-05-03 09:56:39.496000 buteo-0.9.0/buteo/eo/s2_indices.py
+-rw-r--r--   0        0        0    12465 2023-05-08 15:14:09.972611 buteo-0.9.0/buteo/eo/s2_utils.py
+-rw-r--r--   0        0        0      497 2023-05-05 06:20:35.014620 buteo-0.9.0/buteo/raster/__init__.py
+-rw-r--r--   0        0        0    16663 2023-05-08 13:09:19.688308 buteo-0.9.0/buteo/raster/align.py
+-rw-r--r--   0        0        0     7299 2023-05-05 17:25:56.416262 buteo-0.9.0/buteo/raster/borders.py
+-rw-r--r--   0        0        0    13523 2023-05-08 15:16:27.420173 buteo-0.9.0/buteo/raster/clip.py
+-rw-r--r--   0        0        0     1510 2023-05-08 06:54:59.813075 buteo-0.9.0/buteo/raster/coordinates.py
+-rw-r--r--   0        0        0     9674 2023-05-05 10:46:19.677097 buteo-0.9.0/buteo/raster/core_offsets.py
+-rw-r--r--   0        0        0    18427 2023-05-08 14:45:50.472324 buteo-0.9.0/buteo/raster/core_raster.py
+-rw-r--r--   0        0        0    36968 2023-05-08 13:10:58.430080 buteo-0.9.0/buteo/raster/core_raster_io.py
+-rw-r--r--   0        0        0    10157 2023-05-05 12:25:08.222263 buteo-0.9.0/buteo/raster/core_stack.py
+-rw-r--r--   0        0        0     7431 2023-05-08 07:41:05.893227 buteo-0.9.0/buteo/raster/datatype.py
+-rw-r--r--   0        0        0     8331 2023-05-08 08:18:57.689620 buteo-0.9.0/buteo/raster/dem.py
+-rw-r--r--   0        0        0     6231 2023-05-08 07:52:34.295257 buteo-0.9.0/buteo/raster/grid.py
+-rw-r--r--   0        0        0     4079 2023-05-08 13:07:43.602719 buteo-0.9.0/buteo/raster/metadata.py
+-rw-r--r--   0        0        0     8386 2023-05-08 09:51:45.634002 buteo-0.9.0/buteo/raster/nodata.py
+-rw-r--r--   0        0        0     6167 2023-05-08 13:49:35.641110 buteo-0.9.0/buteo/raster/proximity.py
+-rw-r--r--   0        0        0     9300 2023-05-08 11:56:10.990154 buteo-0.9.0/buteo/raster/reproject.py
+-rw-r--r--   0        0        0    10673 2023-05-08 13:04:45.244156 buteo-0.9.0/buteo/raster/resample.py
+-rw-r--r--   0        0        0     8041 2023-05-08 13:37:41.583753 buteo-0.9.0/buteo/raster/shift.py
+-rw-r--r--   0        0        0     4318 2023-05-08 13:48:24.329191 buteo-0.9.0/buteo/raster/vectorize.py
+-rw-r--r--   0        0        0      298 2023-05-03 14:19:58.866941 buteo-0.9.0/buteo/utils/__init__.py
+-rw-r--r--   0        0        0     4536 2023-05-05 12:25:22.517045 buteo-0.9.0/buteo/utils/utils_aux.py
+-rw-r--r--   0        0        0     9459 2023-05-05 12:26:38.230306 buteo-0.9.0/buteo/utils/utils_base.py
+-rw-r--r--   0        0        0    33937 2023-05-07 07:53:13.792610 buteo-0.9.0/buteo/utils/utils_bbox.py
+-rw-r--r--   0        0        0    28852 2023-05-09 07:50:41.612053 buteo-0.9.0/buteo/utils/utils_gdal.py
+-rw-r--r--   0        0        0     8668 2023-05-08 10:00:37.380883 buteo-0.9.0/buteo/utils/utils_io.py
+-rw-r--r--   0        0        0    28485 2023-05-08 09:46:50.435511 buteo-0.9.0/buteo/utils/utils_path.py
+-rw-r--r--   0        0        0    18880 2023-05-08 14:44:59.714163 buteo-0.9.0/buteo/utils/utils_projection.py
+-rw-r--r--   0        0        0    16826 2023-05-08 07:21:50.723919 buteo-0.9.0/buteo/utils/utils_translate.py
+-rw-r--r--   0        0        0      377 2023-05-08 15:17:25.536089 buteo-0.9.0/buteo/vector/__init__.py
+-rw-r--r--   0        0        0     5661 2023-05-09 08:20:47.551957 buteo-0.9.0/buteo/vector/buffer.py
+-rw-r--r--   0        0        0     6639 2023-05-09 08:45:14.629449 buteo-0.9.0/buteo/vector/clip.py
+-rw-r--r--   0        0        0    13506 2023-05-08 15:13:20.210020 buteo-0.9.0/buteo/vector/convert_parts.py
+-rw-r--r--   0        0        0    24435 2023-05-09 08:19:00.716883 buteo-0.9.0/buteo/vector/core_vector.py
+-rw-r--r--   0        0        0     6187 2023-05-08 15:13:20.210020 buteo-0.9.0/buteo/vector/dissolve.py
+-rw-r--r--   0        0        0      263 2023-05-02 12:27:13.705244 buteo-0.9.0/buteo/vector/grid.py
+-rw-r--r--   0        0        0     6529 2023-05-08 15:13:20.210020 buteo-0.9.0/buteo/vector/intersect.py
+-rw-r--r--   0        0        0     1926 2023-05-08 15:13:20.210020 buteo-0.9.0/buteo/vector/merge.py
+-rw-r--r--   0        0        0     7523 2023-05-08 15:13:20.210020 buteo-0.9.0/buteo/vector/metadata.py
+-rw-r--r--   0        0        0     6936 2023-05-08 15:13:20.218015 buteo-0.9.0/buteo/vector/rasterize.py
+-rw-r--r--   0        0        0     4870 2023-05-09 09:04:48.200349 buteo-0.9.0/buteo/vector/reproject.py
+-rw-r--r--   0        0        0     6973 2023-05-08 15:13:20.210020 buteo-0.9.0/buteo/vector/shapes.py
+-rw-r--r--   0        0        0     2637 2023-05-09 08:37:35.507047 buteo-0.9.0/buteo/vector/split.py
+-rw-r--r--   0        0        0    18080 2023-05-08 07:22:45.435592 buteo-0.9.0/buteo/vector/zonal_statistics.py
+-rw-r--r--   0        0        0      785 2023-05-09 09:09:45.358671 buteo-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4710 2023-04-23 13:45:46.888099 buteo-0.9.0/readme.md
+-rw-r--r--   0        0        0     5170 1970-01-01 00:00:00.000000 buteo-0.9.0/PKG-INFO
```

### Comparing `buteo-0.8.9/LICENSE` & `buteo-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `buteo-0.8.9/buteo/raster/clip.py` & `buteo-0.9.0/buteo/raster/core_stack.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,308 +1,280 @@
 """
-### Clip rasters ###
-
-Clips a raster using a vector geometry or the extents of a raster.
+### Functions for changing the datatype of a raster. ###
 """
 
 # Standard library
 import sys; sys.path.append("../../")
-import os
+from typing import Union, List, Optional
 
 # External
-from osgeo import gdal, ogr
-import numpy as np
+from osgeo import gdal
 
 # Internal
-from buteo.raster import core_raster
-from buteo.vector import core_vector
-from buteo.utils import gdal_utils, core_utils, bbox_utils, gdal_enums
-from buteo.vector.reproject import _reproject_vector
+from buteo.utils import (
+    utils_io,
+    utils_base,
+    utils_path,
+    utils_translate,
+)
+from buteo.raster import core_raster, core_raster_io
+
 
 
-def _clip_raster(
-    raster,
-    clip_geom,
-    out_path,
+def raster_stack_list(
+    rasters: List[Union[str, gdal.Dataset]],
+    out_path: Optional[str] = None,
     *,
-    resample_alg="nearest",
-    crop_to_geom=True,
-    adjust_bbox=True,
-    all_touch=True,
-    to_extent=False,
-    overwrite=True,
-    creation_options=None,
-    dst_nodata="infer",
-    src_nodata="infer",
-    layer_to_clip=0,
-    prefix="",
-    suffix="",
-    verbose=1,
-    add_uuid=False,
-    ram="auto",
-):
-    """ INTERNAL. """
-    path_list = gdal_utils.create_output_path_list(
-        core_utils.ensure_list(raster),
-        out_path=out_path,
-        prefix=prefix,
-        suffix=suffix,
-        add_uuid=add_uuid,
-    )
+    overwrite: bool = True,
+    dtype: Optional[str] = None,
+    creation_options: Optional[List[str]] = None,
+) -> Union[str, List[str]]:
+    """
+    Stacks a list of aligned rasters into a single raster file.
 
-    if out_path is not None and isinstance(out_path, str):
-        if "vsimem" not in out_path:
-            if not os.path.isdir(os.path.split(os.path.normpath(out_path))[0]):
-                raise ValueError(f"out_path folder does not exist: {out_path}")
-
-    clip_ds = None
-
-    memory_files = []
-
-    # Input is a vector.
-    if gdal_utils.is_vector(clip_geom):
-        clip_ds = core_vector._open_vector(clip_geom)
-
-        # TODO: Fix potential memory leak
-        if clip_ds.GetLayerCount() > 1:
-            clip_ds = core_vector.vector_filter_layer(clip_ds, layer_name_or_idx=layer_to_clip, add_uuid=True)
-            memory_files.append(clip_ds)
-
-        clip_metadata = core_vector._vector_to_metadata(clip_ds)
-
-        if to_extent:
-            clip_ds = bbox_utils.convert_bbox_to_vector(clip_metadata["bbox"], clip_metadata["projection_osr"])
-            memory_files.append(clip_ds)
-
-        if isinstance(clip_ds, ogr.DataSource):
-            clip_ds = clip_ds.GetName()
-
-    # Input is a raster (use extent)
-    elif gdal_utils.is_raster(clip_geom):
-        clip_metadata = core_raster._raster_to_metadata(clip_geom)
-        clip_ds = bbox_utils.convert_bbox_to_vector(clip_metadata["bbox"], clip_metadata["projection_osr"])
-        memory_files.append(clip_ds)
-    else:
-        if core_utils.file_exists(clip_geom):
-            raise ValueError(f"Unable to parse clip geometry: {clip_geom}")
-        else:
-            raise ValueError(f"Unable to locate clip geometry {clip_geom}")
-
-    if clip_ds is None:
-        raise ValueError(f"Unable to parse input clip geom: {clip_geom}")
-
-    # options
-    warp_options = []
-    if all_touch:
-        warp_options.append("CUTLINE_ALL_TOUCHED=TRUE")
+    Parameters
+    ----------
+    rasters : list
+        List of rasters to stack. These rasters must be aligned.
+
+    out_path : str or None, optional
+        The destination to save the output raster. If not provided, a temporary file will be created. Default: None.
+
+    overwrite : bool, optional
+        If the file exists, should it be overwritten? Default: True.
+
+    dtype : str, optional
+        The data type of the output raster. If not provided, the data type of the input rasters will be used. Default: None.
+
+    creation_options : list, optional
+        A list of GDAL creation options for the output raster. Default is
+        ["TILED=YES", "NUM_THREADS=ALL_CPUS", "BIGTIFF=YES", "COMPRESS=LZW"].
+
+    Returns
+    -------
+    str or list
+        The file path(s) to the newly created raster(s).
+    """
+    utils_base._type_check(rasters, [[str, gdal.Dataset]], "rasters")
+    utils_base._type_check(out_path, [str, None], "out_path")
+    utils_base._type_check(overwrite, [bool], "overwrite")
+    utils_base._type_check(dtype, [str, None], "dtype")
+    utils_base._type_check(creation_options, [[str], None], "creation_options")
+
+    # Get input raster file paths
+    input_data = utils_io._get_input_paths(rasters, "raster")
+
+    # Generate a temporary output file path if out_path is not provided
+    if out_path is None:
+        out_path = utils_path._get_temp_filepath(
+            "temp_stack",
+            ext="tif",
+            add_uuid=True,
+            add_timestamp=True,
+        )
     else:
-        warp_options.append("CUTLINE_ALL_TOUCHED=FALSE")
+        assert utils_path._check_is_valid_output_filepath(out_path), "Invalid output path."
 
-    origin_layer = core_raster.open_raster(raster)
+    # Check if input rasters are aligned
+    assert core_raster.check_rasters_are_aligned(input_data), "Rasters are not aligned."
 
-    raster_metadata = core_raster._raster_to_metadata(raster)
-    origin_projection = raster_metadata["projection_osr"]
+    # Read input rasters as NumPy arrays and stack them
+    array = core_raster_io.raster_to_array(input_data, cast=dtype)
 
-    # Fast check: Does the extent of the two inputs overlap?
-    has_inf = True in [np.isinf(val) for val in raster_metadata["bbox_latlng"]]
-    if not has_inf and not bbox_utils.bboxes_intersect(raster_metadata["bbox_latlng"], clip_metadata["bbox_latlng"]):
-        raise ValueError(f"Geometries of {raster} and {clip_geom} did not intersect.")
-
-    if not origin_projection.IsSame(clip_metadata["projection_osr"]):
-        clip_ds = _reproject_vector(clip_ds, origin_projection)
-        clip_metadata = core_vector._vector_to_metadata(clip_ds)
-        memory_files.append(clip_ds)
-
-    output_bounds = raster_metadata["bbox"]
-
-    if crop_to_geom:
-
-        if adjust_bbox:
-            output_bounds = bbox_utils.align_bboxes_to_pixel_size(
-                raster_metadata["bbox"],
-                clip_metadata["bbox"],
-                raster_metadata["pixel_width"],
-                raster_metadata["pixel_height"],
-            )
-        else:
-            output_bounds = clip_metadata["bbox"]
-
-    # formats
-    out_name = path_list[0]
-    out_format = gdal_utils.path_to_driver_raster(out_name)
-    out_creation_options = gdal_utils.default_creation_options(creation_options)
-
-    # nodata
-    if src_nodata == "infer":
-        src_nodata = raster_metadata["nodata_value"]
-    elif isinstance(src_nodata, (int, float)) or src_nodata is None:
-        src_nodata = float(src_nodata)
-    else:
-        raise ValueError(f"src_nodata must be an int, float or None: {src_nodata}")
+    # Write the stacked array as a raster file
+    out_path = core_raster_io.array_to_raster(
+        array,
+        reference=input_data[0],
+        out_path=out_path,
+        overwrite=overwrite,
+        creation_options=creation_options,
+    )
 
-    out_nodata = None
-    if dst_nodata == "infer":
-        if src_nodata == "infer":
-            out_nodata = raster_metadata["nodata_value"]
-        else:
-            out_nodata = gdal_enums.get_default_nodata_value(raster_metadata["datatype_gdal_raw"])
-    elif isinstance(dst_nodata, (int, float)) or dst_nodata is None:
-        out_nodata = dst_nodata
-    else:
-        raise ValueError(f"Unable to parse nodata_value: {dst_nodata}")
+    return out_path
 
-    # Removes file if it exists and overwrite is True.
-    core_utils.remove_if_required(out_path, overwrite)
 
-    if verbose == 0:
-        gdal.PushErrorHandler("CPLQuietErrorHandler")
+def raster_stack_vrt_list(
+    rasters: List[Union[str, gdal.Dataset]],
+    out_path: Optional[str]=None,
+    separate: bool = True,
+    *,
+    resample_alg: str = "nearest",
+    nodata_src: Optional[float] = None,
+    nodata_VRT: Optional[float] = None,
+    nodata_hide: Optional[bool] = None,
+    options: Optional[list] = None,
+    overwrite: bool = True,
+    reference: Optional[str] = None,
+    creation_options: Optional[List[str]] = None,
+) -> str:
+    """
+    Create a virtual raster (.vrt) by stacking a list of input rasters.
 
-    clipped = gdal.Warp(
-        out_name,
-        origin_layer,
-        format=out_format,
-        resampleAlg=gdal_enums.translate_resample_method(resample_alg),
-        targetAlignedPixels=False,
-        outputBounds=bbox_utils.convert_ogr_bbox_to_gdal_bbox(output_bounds),
-        xRes=raster_metadata["pixel_width"],
-        yRes=raster_metadata["pixel_height"],
-        cutlineDSName=clip_ds,
-        cropToCutline=False,
-        creationOptions=out_creation_options,
-        warpMemoryLimit=gdal_utils.get_gdalwarp_ram_limit(ram),
-        warpOptions=warp_options,
-        srcNodata=src_nodata,
-        dstNodata=out_nodata,
-        multithread=True,
-    )
+    The function accepts a list of rasters and creates a virtual raster stack
+    by combining them. The rasters can be stacked by keeping their bands separate,
+    or by merging the bands in the order of the input rasters.
+
+    Parameters
+    ----------
+    rasters : List[Union[str, gdal.Dataset]]
+        A list of input rasters as either file paths or GDAL datasets to be stacked.
+
+    out_path : Optional[str], default=None
+        The destination file path to save the output VRT raster. If not provided, a
+        temporary file path will be generated.
+
+    separate : bool, default=True
+        If True, the raster bands will be kept separate and stacked in the order of
+        the input rasters. If False, the raster bands will be merged, but all input
+        rasters must have the same number of bands.
+
+    resample_alg : str, default='nearest'
+        The resampling algorithm to use when building the VRT. Accepts any algorithm
+        supported by GDAL's BuildVRT function (e.g., 'nearest', 'bilinear', 'cubic').
+
+    nodata_src : Optional[float], default=None
+        The NoData value to use for the source rasters. If not provided, the NoData
+        value from the input rasters will be used.
+
+    nodata_VRT : Optional[float], default=None
+        The NoData value to use for the output VRT raster. If not provided, the NoData
+        value from the input rasters will be used.
+
+    nodata_hide : Optional[bool], default=None
+        If True, the NoData value will be hidden in the VRT. If not provided, the value
+        will be determined by the input rasters.
+
+    options : Optional[list], default=None
+        A list of VRT options for GDAL. If not provided, default options will be used.
+
+    overwrite : bool, default=True
+        If True and the output file exists, it will be overwritten. If False and the
+        output file exists, an error will be raised.
+
+    reference : Optional[str], default=None
+        A reference raster file path or GDAL dataset to use for aligning the stacked
+        rasters. If not provided, the alignment of the input rasters will be used.
+
+    creation_options : Optional[List[str]], default=None
+        A list of GDAL creation options for the output VRT raster. If not provided,
+        the default options will be used.
+
+    Returns
+    -------
+    str
+        The file path to the newly created VRT raster.
+    """
+    # Type checking for input parameters
+    utils_base._type_check(rasters, [[str, gdal.Dataset]], "rasters")
+    utils_base._type_check(out_path, [str, None], "out_path")
+    utils_base._type_check(separate, [bool], "separate")
+    utils_base._type_check(resample_alg, [str], "resample_alg")
+    utils_base._type_check(options, [list, None], "options")
+    utils_base._type_check(overwrite, [bool], "overwrite")
+    utils_base._type_check(creation_options, [[str], None], "creation_options")
+
+    # Check if all rasters have the same number of bands when separate is False
+    if not separate:
+        master_bands = 0
+
+        for idx, raster_input in enumerate(rasters):
+            if idx == 0:
+                master_bands = core_raster._get_basic_metadata_raster(raster_input)["bands"]
+            else:
+                if master_bands != core_raster._get_basic_metadata_raster(raster_input)["bands"]:
+                    raise ValueError("All rasters must have the same number of bands when separate is False.")
+
+    # Generate a temporary output file path if out_path is not provided
+    if out_path is None:
+        out_path = utils_path._get_temp_filepath(
+            "temp_stack",
+            ext="vrt",
+            add_uuid=True,
+            add_timestamp=True,
+        )
 
-    gdal_utils.delete_if_in_memory_list(memory_files)
+    # Translate the input resample algorithm to a GDAL-compatible format
+    resample_algorithm = utils_translate._translate_resample_method(resample_alg)
 
-    if verbose == 0:
-        gdal.PopErrorHandler()
+    # Build VRT options based on whether a reference raster is provided or not
+    if reference is not None:
+        meta = core_raster._get_basic_metadata_raster(reference)
+        options = gdal.BuildVRTOptions(
+            resampleAlg=resample_algorithm,
+            separate=separate,
+            outputBounds=meta["bbox_gdal"],
+            xRes=meta["pixel_width"],
+            yRes=meta["pixel_height"],
+            targetAlignedPixels=True,
+            srcNodata=nodata_src,
+            VRTNodata=nodata_VRT,
+            hideNodata=nodata_hide,
+        )
+    else:
+        options = gdal.BuildVRTOptions(
+            resampleAlg=resample_algorithm,
+            separate=separate,
+            srcNodata=nodata_src,
+            VRTNodata=nodata_VRT,
+            hideNodata=nodata_hide,
+        )
 
-    if clipped is None:
-        raise ValueError("Error while clipping raster.")
+    # Create separate VRTs for each band if separate is True
+    if separate:
+        tmp_vrt_list = []
+
+        for idx, raster in enumerate(rasters):
+            bands_in_raster = core_raster._get_basic_metadata_raster(raster)["bands"]
+
+            for band in range(bands_in_raster):
+                tmp_vrt_path = utils_path._get_temp_filepath(
+                    "temp_vrt",
+                    ext="vrt",
+                    add_uuid=True,
+                    add_timestamp=True,
+                )
+
+                tmp_vrt_code = gdal.BuildVRT(
+                    tmp_vrt_path,
+                    raster,
+                    options=gdal.BuildVRTOptions(
+                        resampleAlg=resample_algorithm,
+                        separate=True,
+                        srcNodata=nodata_src,
+                        VRTNodata=nodata_VRT,
+                        hideNodata=nodata_hide,
+                        bandList=[band + 1],
+                    )
+                )
+
+                tmp_vrt_list.append(tmp_vrt_path)
+
+                if tmp_vrt_code is None:
+                    raise ValueError(f"Error while creating VRT from rasters: {rasters}")
+
+                tmp_vrt_code = None
+
+        vrt = gdal.BuildVRT(out_path, tmp_vrt_list, options=options)
+
+        # Clean up temporary VRTs
+        for tmp_vrt_path in tmp_vrt_list:
+            gdal.Unlink(tmp_vrt_path)
 
-    return out_name
+    # Create a VRT by merging bands if separate is False
+    else:
+        vrt = gdal.BuildVRT(out_path, rasters, options=options)
 
+    # Flush cache to ensure data is written to the output file
+    vrt.FlushCache()
 
-def clip_raster(
-    raster,
-    clip_geom,
-    out_path=None,
-    *,
-    resample_alg="nearest",
-    crop_to_geom=True,
-    adjust_bbox=False,
-    all_touch=False,
-    to_extent=False,
-    prefix="",
-    suffix="",
-    overwrite=True,
-    creation_options=None,
-    dst_nodata="infer",
-    src_nodata="infer",
-    layer_to_clip=0,
-    verbose=0,
-    add_uuid=False,
-    ram="auto",
-):
-    """
-    Clips a raster(s) using a vector geometry or the extents of a raster.
+    # Check for errors in VRT creation
+    if vrt is None:
+        raise ValueError(f"Error while creating VRT from rasters: {rasters}")
 
-    Args:
-        raster (list/str/gdal.Dataset): The raster(s) to clip.
-        clip_geom (str/ogr.DataSource/gdal.Dataset): The geometry to use to
-            clip the raster.
-
-    Keyword Args:
-        out_path (str/list/None, default=None): The path(s) to save the
-            clipped raster to. If None, a memory raster is created.
-        resample_alg (str, default="nearest"): The resampling algorithm to use.
-            Options include: nearest, bilinear, cubic, cubicspline, lanczos, average,
-                mode, max, min, median, q1, q3, sum, rms.
-        crop_to_geom (bool, default=True): If True, the output raster will be
-            cropped to the extent of the clip geometry.
-        adjust_bbox (bool, default=False): If True, the output raster will have its
-            bbox adjusted to match the clip geometry.
-        all_touch (bool, default=False): If true, all pixels touching the
-            clipping geometry will be included.
-        to_extent (bool, default=False): If True, the output raster will be
-            cropped to the extent of the clip geometry.
-        prefix (str, default=""): The prefix to use for the output raster.
-        suffix (str, default=""): The suffix to use for the output raster.
-        overwrite (bool, default=True): If True, the output raster will be
-            overwritten if it already exists.
-        creation_options (list/None, default=None): A list of creation options
-            to pass to gdal.
-        dst_nodata (int/float/None, default="infer"): The nodata value to use for
-            the output raster.
-        src_nodata (int/float/None, default="infer"): The nodata value to use for
-            the input raster.
-        layer_to_clip (int/str, default=0): The layer ID or name in the
-            vector to use for clipping.
-        verbose (int, default=0): The verbosity level.
-        add_uuid (bool, default=False): If True, a UUID will be added to the
-            output raster.
-        ram (str, default="auto"): The amount of RAM to use for the operation.
-
-    Returns:
-        str/list: A string or list of strings representing the path(s) to
-            the clipped raster(s).
-    """
-    core_utils.type_check(raster, [str, gdal.Dataset, [str, gdal.Dataset]], "raster")
-    core_utils.type_check(clip_geom, [str, ogr.DataSource, gdal.Dataset], "clip_geom")
-    core_utils.type_check(out_path, [[str], str, None], "out_path")
-    core_utils.type_check(resample_alg, [str], "resample_alg")
-    core_utils.type_check(crop_to_geom, [bool], "crop_to_geom")
-    core_utils.type_check(adjust_bbox, [bool], "adjust_bbox")
-    core_utils.type_check(all_touch, [bool], "all_touch")
-    core_utils.type_check(to_extent, [bool], "to_extent")
-    core_utils.type_check(dst_nodata, [str, int, float, None], "dst_nodata")
-    core_utils.type_check(src_nodata, [str, int, float, None], "src_nodata")
-    core_utils.type_check(layer_to_clip, [int], "layer_to_clip")
-    core_utils.type_check(overwrite, [bool], "overwrite")
-    core_utils.type_check(creation_options, [[str], None], "creation_options")
-    core_utils.type_check(prefix, [str], "prefix")
-    core_utils.type_check(suffix, [str], "postfix")
-    core_utils.type_check(verbose, [int], "verbose")
-    core_utils.type_check(add_uuid, [bool], "uuid")
-
-    raster_list = core_utils.ensure_list(raster)
-    path_list = gdal_utils.create_output_path_list(
-        raster_list,
-        out_path=out_path,
-        prefix=prefix,
-        suffix=suffix,
-        add_uuid=add_uuid,
-        overwrite=overwrite,
-    )
+    # Release the VRT object to avoid potential memory leaks
+    vrt = None
 
-    output = []
-    for index, in_raster in enumerate(raster_list):
-        output.append(
-            _clip_raster(
-                in_raster,
-                clip_geom,
-                out_path=path_list[index],
-                resample_alg=resample_alg,
-                crop_to_geom=crop_to_geom,
-                adjust_bbox=adjust_bbox,
-                all_touch=all_touch,
-                to_extent=to_extent,
-                dst_nodata=dst_nodata,
-                src_nodata=src_nodata,
-                layer_to_clip=layer_to_clip,
-                overwrite=overwrite,
-                creation_options=creation_options,
-                prefix=prefix,
-                suffix=suffix,
-                verbose=verbose,
-                ram=ram,
-            )
-        )
+    return out_path
 
-    if isinstance(raster, list):
-        return output
 
-    return output[0]
+# TODO: Mosaic raster(s)
+# TODO: Use gdaltools?
```

### Comparing `buteo-0.8.9/buteo/raster/convolution.py` & `buteo-0.9.0/buteo/array/convolution.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,555 +1,532 @@
 """
 ### Perform convolutions on arrays.  ###
 """
 
+# Standard Library
+import sys; sys.path.append("../../")
+from typing import Union
+
 # External
 import numpy as np
-from numpy.lib.stride_tricks import as_strided
 from numba import jit, prange
 
+# Internal
+from buteo.utils.utils_base import _type_check
+from buteo.array.convolution_funcs import _hood_to_value
 
-def weight_distance(
-    arr,
-    method=None,
-    decay=0.2,
-    sigma=1.0,
-    center=0.0,
-    spherical=False,
-    radius=3.0,
-):
-    """
-    Weights the kernel by distance using various methods.
-
-    Args:
-        arr (numpy.ndarray): The input array.
-        method (str, default=None): The weighting method to use.
-            "none": No weighting (default).
-            "linear": Linear decay.
-            "sqrt": Square root decay.
-            "power": Power decay.
-            "log": Logarithmic decay.
-            "gaussian": Gaussian decay.
-        decay (float, default=0.2): The decay rate for the `linear`, `sqrt`, and `power` methods.
-        sigma (float, default=1.0): The standard deviation for the Gaussian method.
-        center (float, default=0.0): The center of the array.
-        spherical (bool, default=False): If True, adjust weights based on the radius.
-        radius (float, default=3.0): The radius for spherical adjustments.
-
-    Returns:
-        float: The computed weight.
-    """
-
-    if center == 0.0:
-        normed = np.linalg.norm(arr)
-    else:
-        normed = np.linalg.norm(arr - np.array([0, 0, center]))
-
-    if normed == 0.0:
-        weight = 1.0
-
-    if method is None or method == "none" or method == "":
-        weight = 1.0
-    elif method == "linear":
-        weight = np.power((1 - decay), normed)
-    elif method == "sqrt":
-        weight = np.power(np.sqrt((1 - decay)), normed)
-    elif method == "power":
-        weight = np.power(np.power((1 - decay), 2), normed)
-    elif method == "log":
-        weight = np.log(normed + 2)
-    elif method == "gaussian":
-        weight = np.exp(-(np.power(normed, 2)) / (2 * np.power(sigma, 2)))
-    else:
-        raise ValueError("Unable to parse parameters distance_calc.")
-
-    if spherical:
-        sqrt_2 = np.sqrt(2)
-        half_sqrt_2 = np.divide(sqrt_2, 2)
-
-        if normed > (radius - half_sqrt_2) and normed < (radius + half_sqrt_2):
-            adjustment = sqrt_2 / normed
-        elif normed > (radius - half_sqrt_2):
-            adjustment = 0.0
-        elif normed < (radius + half_sqrt_2):
-            adjustment = 1.0
-        else:
-            adjustment = 1.0
-
-        return weight * adjustment
 
-    return weight
 
-
-def rotate_kernel(bottom_right):
+def pad_array(
+    arr: np.ndarray,
+    pad_size: int = 1,
+    method: str = "same",
+    constant_value: Union[float, int] = 0.0,
+) -> np.ndarray:
     """
-    Creates a whole kernel from a quadrant.
-
-    Args:
-        bottom_right (numpy.ndarray): The bottom-right quadrant of the kernel.
+    Create a padded view of an array using SAME padding.
 
-    Returns:
-        numpy.ndarray: The complete kernel generated from the given quadrant.
+    Parameters
+    ----------
+    arr : numpy.ndarray
+        The input array to be padded.
+
+    pad_size : int, optional
+        The number of padding elements to add to each side of the array.
+        Default: 1.
+
+    method : str, optional
+        The padding method to use. Default: "same". Other options are
+        "edge" and "constant".
+
+    constant_value : int, optional
+        The constant value to use when padding with "constant". Default: 0.
+
+    Returns
+    -------
+    numpy.ndarray
+        A padded view of the input array.
+
+    Notes
+    -----
+    This function creates a padded view of an array using SAME padding, which
+    adds padding elements to each side of the array so that the output shape
+    is the same as the input shape. The amount of padding is determined by the
+    `pad_size` parameter. The padding method can be one of three options: "same"
+    (the default), "edge", or "constant". If "constant" padding is used, the
+    `constant_value` parameter specifies the value to use.
     """
+    _type_check(arr, [np.ndarray], "arr")
+    _type_check(pad_size, [int], "pad_size")
+    _type_check(method, [str], "method")
+
+    assert pad_size >= 0, "pad_size must be a non-negative integer"
+    method = method.lower()
+    assert method in ["same", "edge", "constant"], "method must be one of ['same', 'edge', 'constant']"
+
+    if method in ["same", "edge"]:
+        padded_view = np.pad(
+            arr,
+            pad_width=((pad_size, pad_size), (pad_size, pad_size), (0, 0)),
+            mode='edge',
+        )
+    elif method in "constant":
+        padded_view = np.pad(
+            arr,
+            pad_width=((pad_size, pad_size), (pad_size, pad_size), (0, 0)),
+            mode='constant',
+            constant_values=constant_value,
+        )
 
-    size = ((bottom_right.shape[0] - 1) * 2) + 1
-    depth = bottom_right.shape[2]
-    kernel = np.zeros((size, size, depth), dtype="float32")
-
-    top_right = np.flipud(bottom_right)
-    lower_left = np.fliplr(bottom_right)
-    top_left = np.flipud(lower_left)
-
-    kernel = np.block([[top_left, top_right], [lower_left, bottom_right]])
-
-    return kernel
+    return padded_view
 
 
-def get_kernel(
-    size,
-    depth=1,
-    hole=False,
-    inverted=False,
-    normalise=True,
-    multi_dimensional=False,
-    multi_dimensional_center=0,
-    spherical=False,
-    distance_weight=None,
-    distance_decay=0.2,
-    distance_sigma=1,
-):
+@jit(nopython=True, parallel=True, nogil=False, fastmath=True, cache=True)
+def _convolve_array_2D(
+    arr: np.ndarray,
+    offsets: np.ndarray,
+    weights: np.ndarray,
+    method: int = 1,
+    nodata: bool = False,
+    nodata_value: float = -9999.9,
+    func_value: Union[int, float] = 0.5,
+) -> np.ndarray:
     """
-    Generates a square kernel for convolutions.
-
-    Args:
-        size (int): Size of the kernel (must be odd).
-        depth (int, default=1): Depth of the kernel.
-        hole (bool, default=False): Create a hole in the center of the kernel.
-        inverted (bool, default=False): Invert the kernel values.
-        normalise (bool, default=True): Normalize the kernel values.
-        multi_dimensional (bool, default=False): Consider the kernel multi-dimensional.
-        multi_dimensional_center (int, default=0): Center of the
-            multi-dimensional kernel.
-        spherical (bool, default=False): Consider the kernel spherical.
-        distance_weight (str or None, default=None): Distance weighting method.
-        distance_decay (float, default=0.2): Distance decay factor.
-        distance_sigma (float, default=1): Distance sigma for Gaussian distance weighting.
-
-    Returns:
-        tuple: A tuple containing the kernel, weights, and offsets.
+    Internal function for convolving a 2D array.
+    Input should be float32.
     """
+    result = np.zeros((arr.shape[0], arr.shape[1]), dtype="float32")
+    hood_size = len(offsets)
+    weights_total = np.sum(weights)
 
-    assert size >= 3, "Kernel must have atleast size 3."
-    assert size % 2 != 0, "Kernel must be an uneven size."
-    assert isinstance(size, int), "Kernel must be an integer."
-    assert depth >= 1, "Depth must be a positive integer"
-    assert isinstance(depth, int), "Depth must be an integer."
-
-    if distance_weight is False:
-        distance_weight = None
-
-    quadrant = np.zeros((1 + size // 2, 1 + size // 2, depth), dtype="float32")
-
-    for idx_x in range(0, quadrant.shape[0]):
-        for idx_y in range(0, quadrant.shape[1]):
-            for idx_z in range(0, quadrant.shape[2]):
-
-                z_value = idx_z if multi_dimensional else 0
-
-                weighted = weight_distance(
-                    np.array([idx_x, idx_y, z_value], dtype="float32"),
-                    method=distance_weight,
-                    decay=distance_decay,
-                    sigma=distance_sigma,
-                    center=multi_dimensional_center,
-                    spherical=spherical,
-                    radius=size // 2,
-                )
-
-                quadrant[idx_x, idx_y, idx_z] = weighted
-    if hole:
-        for idx_z in range(0, quadrant.shape[2]):
-            quadrant[0, 0, idx_z] = 0
-
-    kernel = rotate_kernel(quadrant)
-
-    if distance_weight == "log":
-        kernel = kernel.max() - kernel
-
-    if inverted:
-        kernel = 1 - kernel
-
-    if normalise:
-        if multi_dimensional:
-            summed = kernel.sum()
-            if summed != 0.0:
-                kernel = kernel / summed
-        else:
-            summed = kernel.sum(axis=(0, 1))
-
-            for dim in range(0, depth):
-                kernel[:, :, dim] = kernel[:, :, dim] / summed[dim]
-
-    weights = []
-    offsets = []
+    nodata_value = np.float32(nodata_value)
 
-    for idx_x in range(0, kernel.shape[0]):
-        for idx_y in range(0, kernel.shape[1]):
-            for idx_z in range(0, kernel.shape[2]):
-                current_weight = kernel[idx_x][idx_y][idx_z]
+    for idx_y in prange(arr.shape[0]):
+        for idx_x in range(arr.shape[1]):
+            hood_values = np.zeros(hood_size, dtype="float32")
+            hood_weights = np.zeros(hood_size, dtype="float32")
+            hood_normalise = False
+            hood_center = 0
+            hood_count = 0
+
+            if nodata and arr[idx_y, idx_x] == nodata_value:
+                result[idx_y, idx_x] = nodata_value
+                continue
+
+            for idx_h in range(0, hood_size):
+                hood_y = idx_y + offsets[idx_h][0]
+                hood_x = idx_x + offsets[idx_h][1]
 
-                if current_weight <= 0.0:
+                if hood_y < 0 or hood_y >= arr.shape[0]:
+                    hood_normalise = True
                     continue
 
-                offsets.append(
-                    [
-                        idx_x - (kernel.shape[0] // 2),
-                        idx_y - (kernel.shape[1] // 2),
-                        idx_z
-                    ]
-                )
-
-                weights.append(current_weight)
-
-    return kernel, np.array(weights, dtype="float32"), np.array(offsets, dtype=int)
-
-
-@jit(nopython=True, parallel=True, nogil=True, fastmath=True, inline="always")
-def hood_max(values, weights):
-    """ Get the weighted maximum. """
-    idx = np.argmax(np.multiply(values, weights))
-    return values[idx]
-
-
-@jit(nopython=True, parallel=True, nogil=True, fastmath=True, inline="always")
-def hood_min(values, weights):
-    """ Get the weighted minimum. """
-    max_val = values.max()
-    adjusted_values = np.where(weights == 0.0, max_val, values)
-    idx = np.argmin(np.divide(adjusted_values, weights + 1e-7))
-    return values[idx]
-
-
-@jit(nopython=True, parallel=True, nogil=True, fastmath=True, inline="always")
-def hood_sum(values, weights):
-    """ Get the weighted sum. """
-    return np.sum(np.multiply(values, weights))
-
-
-@jit(nopython=True, parallel=True, nogil=True, fastmath=True, inline="always")
-def hood_mode(values, weights):
-    """ Get the weighted sum. """
-    values_ints = np.rint(values)
-    unique = np.unique(values_ints)
-
-    most_occured_value = 0
-    most_occured_weight = -9999.9
-
-    for unique_value in unique:
-        cum_weight = 0
-        for idx in range(values.shape[0]):
-            if values_ints[idx] == unique_value:
-                cum_weight += weights[idx]
-
-        if cum_weight > most_occured_weight:
-            most_occured_weight = cum_weight
-            most_occured_value = unique_value
+                if hood_x < 0 or hood_x >= arr.shape[1]:
+                    hood_normalise = True
+                    continue
 
-    return most_occured_value
+                if nodata and arr[hood_y, hood_x] == nodata_value:
+                    hood_normalise = True
+                    continue
 
+                hood_values[hood_count] = arr[hood_y, hood_x]
+                hood_weights[hood_count] = weights[idx_h]
+                hood_count += 1
+
+                if offsets[idx_h][0] == 0 and offsets[idx_h][1] == 0:
+                    hood_center = hood_count - 1
+
+            if hood_count == 0:
+                result[idx_y, idx_x] = nodata_value
+                continue
+
+            hood_values = hood_values[:hood_count]
+            hood_weights = hood_weights[:hood_count]
+
+            if hood_normalise:
+                hood_weights /= np.sum(hood_weights)
+                hood_weights *= weights_total
+
+            result[idx_y, idx_x] = _hood_to_value(
+                method,
+                hood_values,
+                hood_weights,
+                nodata_value,
+                hood_center,
+                func_value,
+            )
 
-@jit(nopython=True, parallel=True, nogil=True, fastmath=True, inline="always")
-def hood_contrast(values, weights):
-    """ Get the local contrast. """
-    max_val = values.max()
-    adjusted_values = np.where(weights == 0.0, max_val, values)
-    local_min = np.min(np.divide(adjusted_values, weights + 1e-7))
-    local_max = np.max(np.multiply(values, weights))
+    return result
 
-    return np.abs(local_max - local_min)
 
-@jit(nopython=True, parallel=True, nogil=True, fastmath=True, inline="always")
-def hood_quantile(values, weights, quant):
-    """ Get the weighted median. """
-    sort_mask = np.argsort(values)
-    sorted_data = values[sort_mask]
-    sorted_weights = weights[sort_mask]
-    cumsum = np.cumsum(sorted_weights)
-    intersect = (cumsum - 0.5 * sorted_weights) / cumsum[-1]
-    return np.interp(quant, intersect, sorted_data)
+@jit(nopython=True, nogil=True, cache=True, fastmath=True, parallel=True)
+def convolve_array_simple(
+    arr: np.ndarray,
+    offsets: np.ndarray,
+    weights: np.ndarray,
+) -> np.ndarray:
+    """
+    Convolve a kernel with an array using a simple method.
+    Array must be 2D (height, width).
+    The function ignores nodata values and pads the array with 'same'.
+    It only supports 'summation' method.
+
+    Parameters
+    ----------
+    arr : numpy.ndarray
+        The array to convolve.
+
+    offsets : numpy.ndarray
+        The offsets of the kernel.
+
+    weights : numpy.ndarray
+        The weights of the kernel.
+
+    Returns
+    -------
+    numpy.ndarray
+        The convolved array.
+    """
+    result = np.zeros(arr.shape, dtype=np.float32)
 
+    for col in prange(arr.shape[0]):
+        for row in range(arr.shape[1]):
 
-@jit(nopython=True, parallel=True, nogil=True, fastmath=True, inline="always")
-def hood_median_absolute_deviation(values, weights):
-    """ Get the median absolute deviation """
-    median = hood_quantile(values, weights, 0.5)
-    absdeviation = np.abs(np.subtract(values, median))
-    return hood_quantile(absdeviation, weights, 0.5)
+            result_value = 0.0
+            for i in range(offsets.shape[0]):
+                new_col = col + offsets[i, 0]
+                new_row = row + offsets[i, 1]
 
+                if new_col < 0:
+                    new_col = 0
+                elif new_col >= arr.shape[0]:
+                    new_col = arr.shape[0] - 1
 
-@jit(nopython=True, parallel=True, nogil=True, fastmath=True, inline="always")
-def hood_z_score(values, center_value, weights):
-    """ Get the local z score ."""
-    std = hood_standard_deviation(values, weights)
-    mean = hood_sum(values, weights)
+                if new_row < 0:
+                    new_row = 0
+                elif new_row >= arr.shape[1]:
+                    new_row = arr.shape[1] - 1
 
-    return (center_value - mean) / std
+                result_value += arr[new_col, new_row] * weights[i]
 
+            result[col, row] = result_value
 
-@jit(nopython=True, parallel=True, nogil=True, fastmath=True, inline="always")
-def hood_z_score_mad(values, center_value, weights):
-    """ Get the local z score calculated around the MAD. """
-    mad_std = hood_median_absolute_deviation(values, weights) * 1.4826
-    median = hood_quantile(values, weights, 0.5)
+    return result
 
-    return (center_value - median) / mad_std
 
+@jit(nopython=True, parallel=True, nogil=False, fastmath=True, cache=True)
+def _convolve_array_channels_HWC(
+    arr: np.ndarray,
+    method: int = 1,
+    nodata: bool = False,
+    nodata_value: float = -9999.9,
+    func_value: Union[int, float] = 0.5,
+) -> np.ndarray:
+    """
+    Internal function for convoling a 3D array along its channels.
+    Input should be float32. Channel-last version.
+    """
+    result = np.zeros((arr.shape[0], arr.shape[1], 1), dtype="float32")
 
-@jit(nopython=True, parallel=True, nogil=True, fastmath=True, inline="always")
-def hood_standard_deviation(values, weights):
-    "Get the weighted standard deviation. "
-    summed = hood_sum(values, weights)
-    variance = np.sum(np.multiply(np.power(np.subtract(values, summed), 2), weights))
-    return np.sqrt(variance)
+    hood_size = arr.shape[2]
+    center_idx = int(hood_size / 2)
 
+    for idx_y in prange(arr.shape[0]):
+        for idx_x in range(arr.shape[1]):
+            hood_values = np.zeros(hood_size, dtype="float32")
+            hood_weights = np.ones(hood_size, dtype="float32")
+            hood_count = 0
 
-@jit(nopython=True, parallel=True, nogil=True, fastmath=True, inline="always")
-def k_to_size(size):
-    """ Preprocess Sigma Lee limits. """
-    return int(np.rint(-0.0000837834 * size ** 2 + 0.045469 * size + 0.805733))
+            for idx_c in range(hood_size):
+                if nodata and arr[idx_y, idx_x, idx_c] == nodata_value:
+                    continue
 
+                hood_values[hood_count] = arr[idx_y, idx_x, idx_c]
+                hood_count += 1
 
-@jit(nopython=True, parallel=True, nogil=True, fastmath=True, inline="always")
-def hood_sigma_lee(values, weights):
-    """ Sigma lee SAR filter. """
-    std = hood_standard_deviation(values, weights)
-    selected_values = np.zeros_like(values)
-    selected_weights = np.zeros_like(weights)
+            if hood_count == 0:
+                result[idx_y, idx_x, 0] = nodata_value
+                continue
+
+            hood_values = hood_values[:hood_count]
+            hood_weights = hood_weights[:hood_count] / hood_weights[:hood_count].sum()
+
+            result[idx_y, idx_x, 0] = _hood_to_value(
+                method,
+                hood_values,
+                hood_weights,
+                nodata_value,
+                center_idx,
+                func_value,
+            )
 
-    sigma_mult = 1
-    passed = 0
-    attempts = 0
-    ks = k_to_size(values.size)
+    return result
 
-    while passed < ks and attempts < 5:
-        for idx, val in np.ndenumerate(values):
-            if val >= std * sigma_mult or val <= -std * sigma_mult:
-                selected_values[idx] = val
-                selected_weights[idx] = weights[idx]
-                passed += 1
 
-        sigma_mult += 1
-        attempts += 1
+@jit(nopython=True, parallel=True, nogil=False, fastmath=True, cache=True)
+def _convolve_array_channels_CHW(
+    arr: np.ndarray,
+    method: int = 1,
+    nodata: bool = False,
+    nodata_value: float = -9999.9,
+    func_value: Union[int, float] = 0.5,
+) -> np.ndarray:
+    """
+    Internal function for convoling a 3D array along its channels.
+    Input should be float32. Channel-first version.
+    """
+    result = np.zeros((1, arr.shape[0], arr.shape[1]), dtype="float32")
 
-    if passed < ks:
-        return hood_sum(values, weights)
+    hood_size = arr.shape[0]
+    center_idx = int(hood_size / 2)
 
-    sum_of_weights = np.sum(selected_weights)
+    for idx_y in prange(arr.shape[1]):
+        for idx_x in range(arr.shape[2]):
+            hood_count = 0
+            hood_values = np.zeros(hood_size, dtype="float32")
+            hood_weights = np.ones(hood_size, dtype="float32")
 
-    if sum_of_weights == 0:
-        return 0
+            for idx_c in range(hood_size):
+                if nodata and arr[idx_c, idx_y, idx_x] == nodata_value:
+                    continue
+                hood_values[hood_count] = arr[idx_c, idx_y, idx_x]
+                hood_count += 1
 
-    selected_weights = np.divide(selected_weights, sum_of_weights)
+            if hood_count == 0:
+                result[0, idx_y, idx_x] = nodata_value
+                continue
+
+            hood_values = hood_values[:hood_count]
+            hood_weights = hood_weights[:hood_count] / hood_weights[:hood_count].sum()
+
+            result[0, idx_y, idx_x] = _hood_to_value(
+                method,
+                hood_values,
+                hood_weights,
+                nodata_value,
+                center_idx,
+                func_value,
+            )
 
-    return hood_sum(selected_values, selected_weights)
+    return result
 
 
-@jit(nopython=True, nogil=True)
-def pad_array_view(arr, pad_size=1):
+def convolve_array_channels(
+    arr: np.ndarray,
+    method: int = 1,
+    nodata: bool = False,
+    nodata_value: float = -9999.9,
+    func_value: Union[int, float] = 0.5,
+    channel_last: bool = True,
+) -> np.ndarray:
     """
-    Create a padded view of an array using SAME padding.
-
-    Args:
-        arr (numpy.ndarray): The input array to be padded.
-2
-    Keyword Args:
-        pad_size (int, default=1): The number of padding elements to add
-            to each side of the array. Default is 1.
-
-    Returns:
-        numpy.ndarray: A padded view of the input array.
-    """
-    # Get original array shape and strides
-    shape = arr.shape
-    strides = arr.strides
-
-    # Compute new shape and strides for the padded view
-    new_shape = (shape[0] + 2 * pad_size, shape[1] + 2 * pad_size, shape[2])
-    new_strides = (strides[0], strides[1], strides[2])
-
-    # Create the padded view using as_strided
-    padded_view = as_strided(arr, shape=new_shape, strides=new_strides)
-
-    # Pad the edges using the SAME padding
-    padded_view[:pad_size, :, :] = padded_view[pad_size:pad_size + 1, :, :]
-    padded_view[-pad_size:, :, :] = padded_view[-pad_size - 1:-pad_size, :, :]
-    padded_view[:, :pad_size, :] = padded_view[:, pad_size:pad_size + 1, :]
-    padded_view[:, -pad_size:, :] = padded_view[:, -pad_size - 1:-pad_size, :]
-
-    return padded_view
+    Convolves a 3D array along its channels.
+    Useful for 'collapsing' a 3D array into a 2D array.
 
+    Parameters
+    ----------
+    arr : np.ndarray
+        A 3D array.
+
+    method : int, optional
+        The method to use for convolving the array.
+
+        The following methods are valid:
+        1. sum
+        2. max
+        3. min
+        4. mean
+        5. median
+        6. variance
+        7. standard deviation
+        8. contrast
+        9. mode
+        10. median absolute deviation (mad)
+        11. z-score
+        12. z-score (mad)
+        13. sigma lee
+        14. quantile
+        15. occurances
+        16. feather
+        17. roughness
+        18. roughness tri
+        19. roughness tpi
+
+        Default: 1.
+    
+    nodata : bool, optional
+        Whether to use nodata values in the convolution. Default: False.
+    
+    nodata_value : float, optional
+        The nodata value to use in the convolution. Default: -9999.9.
+    
+    func_value : int or float, optional
+        The value to use in the convolution. Default: 0.5.
+    
+    channel_last : bool, optional
+        Whether the channels are the last axis in the array. Default: True.
+
+    Returns
+    -------
+    np.ndarray
+        The convolved array.
+    """
+    _type_check(arr, [np.ndarray], "arr")
+    _type_check(method, [int], "method")
+    _type_check(nodata, [bool], "nodata")
+    _type_check(nodata_value, [float], "nodata_value")
+    _type_check(func_value, [int, float], "value")
+
+    assert arr.ndim == 3, "arr must be a 3D array"
+    assert method in range(1, 18), "method must be between 1 and 17"
+
+    if arr.shape[2] == 1:
+        return arr
+
+    arr = arr.astype(np.float32, copy=False)
+
+    if channel_last:
+        return _convolve_array_channels_HWC(
+            arr,
+            method=method,
+            nodata=nodata,
+            nodata_value=nodata_value,
+            func_value=func_value,
+        )
+    else:
+        return _convolve_array_channels_CHW(
+            arr,
+            method=method,
+            nodata=nodata,
+            nodata_value=nodata_value,
+            func_value=func_value,
+        )
 
-@jit(nopython=True, nogil=True)
-def pad_array(arr, pad_size=1):
-    """ Pad an array using SAME """
-    # Core
-    arr_padded = np.zeros((arr.shape[0] + int(pad_size * 2), arr.shape[1] + int(pad_size * 2), arr.shape[2]), dtype=arr.dtype)
-    arr_padded[pad_size:-pad_size, pad_size:-pad_size, :] = arr
-
-    # Corners
-    arr_padded[0:pad_size, 0:pad_size, :] = arr[ 0,  0, :]
-    arr_padded[-pad_size:, -pad_size:, :] = arr[-1, -1, :]
-    arr_padded[0:pad_size, -pad_size:, :] = arr[ 0, -1, :]
-    arr_padded[-pad_size:, 0:pad_size, :] = arr[-1,  0, :]
-
-    # Sides
-    for idx in range(0, pad_size):
-        arr_padded[idx, pad_size:-pad_size, :] = arr[ 0,  :, :]
-        arr_padded[-(idx + 1):, pad_size:-pad_size, :] = arr[-1,  :, :]
-        arr_padded[pad_size:-pad_size, -(idx + 1), :] = arr[ :, -1, :]
-        arr_padded[pad_size:-pad_size, idx, :] = arr[ :,  0, :]
-
-    return arr_padded
-
-METHOD_ENUMS = {
-    "sum": 1,
-    "mode": 2,
-    "max": 3,
-    "min": 4,
-    "contrast": 5,
-    "median": 6,
-    "std": 7,
-    "mad": 8,
-    "z_score": 9,
-    "z_score_mad": 10,
-    "sigma_lee": 11,
-}
 
-@jit(nopython=True, parallel=True, nogil=False, fastmath=True, cache=True)
 def convolve_array(
-    arr,
-    offsets,
-    weights,
-    method=1,
-    nodata=False,
-    nodata_value=-9999.9,
-):
-    """
-    Convolve an image with a function.
-
-    Args:
-        arr (numpy.ndarray): The input array to convolve.
-        offsets (list of tuples): The list of offsets for the neighborhood
-            used in the convolution.
-        weights (list): The list of weights used in the convolution.
-
-    Keyword Args:
-        method (int, default=1): The method to use for the convolution.
-            1: hood_sum
-            2: hood_mode
-            3: hood_max
-            4: hood_min
-            5: hood_contrast
-            6: hood_quantile
-            7: hood_standard_deviation
-            8: hood_median_absolute_deviation
-            9: hood_z_score
-            10: hood_z_score_mad
-            11: hood_sigma_lee
-        nodata (bool, default=False): If True, nodata values are considered
-            in the convolution.
-        nodata_value (float, default=-9999.9): The value representing nodata.
-
-    Returns:
-        numpy.ndarray: The convolved array.
-    """
-    x_adj = arr.shape[0] - 1
-    y_adj = arr.shape[1] - 1
-    z_adj = (arr.shape[2] - 1) // 2
-
-    hood_size = len(offsets)
-
-    result = np.zeros((arr.shape[0], arr.shape[1], 1), dtype="float32")
-
-    for idx_x in prange(arr.shape[0]):
-        for idx_y in range(arr.shape[1]):
-
-            hood_values = np.zeros(hood_size, dtype="float32")
+    arr: np.ndarray,
+    offsets: np.ndarray,
+    weights: np.ndarray,
+    method: int = 1,
+    nodata: bool = False,
+    nodata_value: float = -9999.9,
+    func_value: Union[int, float] = 0.5,
+    channel_last: bool = True,
+) -> np.ndarray:
+    """
+    Convolve an array using a set of offsets and weights.
+    Array can be 2D or 3D.
 
-            hood_weights = np.zeros(hood_size, dtype="float32")
-            weight_sum = np.array([0.0], dtype="float32")
-            center_value = np.float32(arr[idx_x, idx_y, 0])
-            normalise = False
-
-            for idx_n in range(hood_size):
-                offset_x = idx_x + offsets[idx_n][0]
-                offset_y = idx_y + offsets[idx_n][1]
-                offset_z = offsets[idx_n][2]
-
-                outside = False
-
-                if offset_z < -z_adj:
-                    offset_z = -z_adj
-                    outside = True
-                elif offset_z > z_adj:
-                    offset_z = z_adj
-                    outside = True
-
-                if offset_x < 0:
-                    offset_x = 0
-                    outside = True
-                elif offset_x > x_adj:
-                    offset_x = x_adj
-                    outside = True
-
-                if offset_y < 0:
-                    offset_y = 0
-                    outside = True
-                elif offset_y > y_adj:
-                    offset_y = y_adj
-                    outside = True
-
-                value = np.float32(arr[offset_x, offset_y, offset_z])
-
-                if outside is True:
-                    normalise = True
-                    hood_weights[idx_n] = 0
-                elif nodata and value == nodata_value:
-                    normalise = True
-                    hood_weights[idx_n] = 0
-                else:
-                    hood_values[idx_n] = value
-
-                    weight = weights[idx_n]
-
-                    hood_weights[idx_n] = weight
-                    weight_sum[0] += weight
-
-            if normalise and weight_sum[0] > 0.0:
-                hood_weights = np.true_divide(hood_weights, weight_sum[0])
-
-            if method == 1:
-                result[idx_x, idx_y, 0] = hood_sum(hood_values, hood_weights)
-            elif method == 2:
-                result[idx_x, idx_y, 0] = hood_mode(hood_values, hood_weights)
-            elif method == 3:
-                result[idx_x, idx_y, 0] = hood_max(hood_values, hood_weights)
-            elif method == 4:
-                result[idx_x, idx_y, 0] = hood_min(hood_values, hood_weights)
-            elif method == 5:
-                result[idx_x, idx_y, 0] = hood_contrast(hood_values, hood_weights)
-            elif method == 6:
-                result[idx_x, idx_y, 0] = hood_quantile(hood_values, hood_weights, 0.5)
-            elif method == 7:
-                result[idx_x, idx_y, 0] = hood_standard_deviation(hood_values, hood_weights)
-            elif method == 8:
-                result[idx_x, idx_y, 0] = hood_median_absolute_deviation(hood_values, hood_weights)
-            elif method == 9:
-                result[idx_x, idx_y, 0] = hood_z_score(hood_values, center_value, hood_weights)
-            elif method == 10:
-                result[idx_x, idx_y, 0] = hood_z_score_mad(hood_values, center_value, hood_weights)
-            elif method == 11:
-                result[idx_x, idx_y, 0] = hood_sigma_lee(hood_values, hood_weights)
-            else:
-                result[idx_x, idx_y, 0] = nodata_value
+    Parameters
+    ----------
+    arr : numpy.ndarray
+        The input array to be convolved.
+
+    offsets : list of tuples
+        The list of pixel offsets to use in the convolution. Each tuple should be in the
+        format (row_offset, col_offset, depth_offset), where row_offset and col_offset
+        are the row and column offsets from the center pixel, and depth_offset is the
+        depth offset if the input array has more than two dimensions.
+
+    weights : list of floats
+        The list of weights to use in the convolution. The length of the weights list should
+        be the same as the length of the offsets list.
+
+    method : int, optional
+        The convolution method to use. Default: 1.
+        The following methods are valid:
+        1. sum
+        2. max
+        3. min
+        4. mean
+        5. median
+        6. variance
+        7. standard deviation
+        8. contrast
+        9. mode
+        10. median absolute deviation (mad)
+        11. z-score
+        12. z-score (mad)
+        13. sigma lee
+        14. quantile
+        15. occurances
+        16. feather
+        17. roughness
+        18. roughness tri
+        19. roughness tpi
+
+    nodata : bool, optional
+        If True, treat the nodata value as a valid value. Default: False.
+
+    nodata_value : float, optional
+        The nodata value to use when computing the result. Default: -9999.9.
+
+    func_value : int or float, optional
+        The value to use for pixels where the kernel extends outside the input array.
+        If None, use the edge value. Default: 0.5.
+    
+    channel_last : bool, optional
+        Whether the channels are the last axis in the array. Default: True.
+
+    Returns
+    -------
+    numpy.ndarray
+        The convolved array.
+
+    Notes
+    -----
+    This function convolves an array using a set of offsets and weights. The function supports
+    different convolution methods, including nearest, linear, and cubic. The function can also
+    handle nodata values and cases where the kernel extends outside the input array.
+    """
+    _type_check(arr, [np.ndarray], "arr")
+    _type_check(offsets, [np.ndarray], "offsets")
+    _type_check(weights, [np.ndarray], "weights")
+    _type_check(method, [int], "method")
+    _type_check(nodata, [bool], "nodata")
+    _type_check(nodata_value, [float], "nodata_value")
+    _type_check(func_value, [int, float, type(None)], "value")
+    _type_check(channel_last, [bool], "channel_last")
+
+    assert len(offsets) == len(weights), "offsets and weights must be the same length"
+    assert arr.ndim in [2, 3], "arr must be 2 or 3 dimensional"
+    assert method in range(1, 18), "method must be between 1 and 17"
+
+    arr = arr.astype(np.float32, copy=False)
+
+    if arr.ndim == 2:
+        return _convolve_array_2D(
+            arr,
+            offsets,
+            weights,
+            method=method,
+            nodata=nodata,
+            nodata_value=nodata_value,
+            func_value=func_value,
+        )
+
+    result = np.zeros((arr.shape), dtype="float32")
+
+    if channel_last:
+        for idx_d in range(arr.shape[2]):
+            result[:, :, idx_d] = _convolve_array_2D(
+                arr[:, :, idx_d],
+                offsets,
+                weights,
+                method=method,
+                nodata=nodata,
+                nodata_value=nodata_value,
+                func_value=func_value,
+            )
+    else:
+        for idx_d in range(arr.shape[0]):
+            result[idx_d, :, :] = _convolve_array_2D(
+                arr[idx_d, :, :],
+                offsets,
+                weights,
+                method=method,
+                nodata=nodata,
+                nodata_value=nodata_value,
+                func_value=func_value,
+            )
 
     return result
```

### Comparing `buteo-0.8.9/buteo/raster/resample.py` & `buteo-0.9.0/buteo/raster/proximity.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,201 +1,197 @@
 """
-### Resample rasters. ###
+### Calculate distances on a raster. ###
 
-Module to resample rasters to a target resolution.
-Can uses references from vector or other raster datasets.
+Module to calculate the distance from a pixel value to other pixels.
 """
 
 # Standard library
 import sys; sys.path.append("../../")
+from typing import Union, List, Optional
 
 # External
-from osgeo import gdal
 import numpy as np
+from osgeo import gdal
 
 # Internal
-from buteo.utils import core_utils, gdal_utils, gdal_enums
-from buteo.raster import core_raster
+from buteo.utils import (
+    utils_base,
+    utils_io,
+    utils_path,
+)
+from buteo.raster import core_raster, core_raster_io
+from buteo.array.convolution_distance import convolve_distance
+
+
+def _raster_get_proximity(
+    raster: Union[str, gdal.Dataset],
+    target_value: Union[int, float] = 1,
+    unit: str = "geo",
+    out_path: Optional[str] = None,
+    max_dist: Union[int, float] = 1000,
+    add_border: bool = False,
+    border_value: Union[int, float] = 0,
+    inverted: bool = False,
+    overwrite: bool = True,
+) -> str:
+    """
+    Internal. Calculate the proximity of a raster to values.
+    """
+    assert isinstance(raster, (str, gdal.Dataset)), f"Invalid raster. {raster}"
+    assert isinstance(target_value, (int, float)), f"Invalid target_value. {target_value}"
+    assert isinstance(unit, str), f"Invalid unit. {unit}"
+
+    if out_path is None:
+        out_path = utils_path._get_temp_filepath("proximity_raster.tif")
+
+    array = core_raster_io.raster_to_array(raster, filled=True)
+
+    if unit.lower() == "geo":
+        metadata = core_raster._get_basic_metadata_raster(raster)
+        pixel_height = metadata["pixel_height"]
+        pixel_width = metadata["pixel_width"]
+    else:
+        pixel_height = 1
+        pixel_width = 1
 
+    if add_border:
+        padded = np.full((array.shape[0] + 2, array.shape[1] + 2, array.shape[2]), border_value, dtype=array.dtype)
+        padded[1:-1, 1:-1] = array
+        array = padded
+
+    array = convolve_distance(
+        array,
+        target=target_value,
+        maximum_distance=max_dist,
+        pixel_width=pixel_width,
+        pixel_height=pixel_height,
+    )
 
+    if inverted:
+        array = array.max() - array
 
-def _resample_raster(
-    raster,
-    target_size,
-    out_path=None,
-    *,
-    target_in_pixels=False,
-    resample_alg="nearest",
-    overwrite=True,
-    creation_options=None,
-    dtype=None,
-    dst_nodata="infer",
-    prefix="",
-    suffix="_resampled",
-    add_uuid=False,
-):
-    """ Internal. """
-    assert isinstance(raster, (gdal.Dataset, str)), f"The input raster must be in the form of a str or a gdal.Dataset: {raster}"
+    if add_border:
+        array = array[1:-1, 1:-1]
 
-    out_path = gdal_utils.create_output_path(
-        raster,
+    out_path = core_raster_io.array_to_raster(
+        array,
+        reference=raster,
         out_path=out_path,
         overwrite=overwrite,
-        prefix=prefix,
-        suffix=suffix,
-        add_uuid=add_uuid,
     )
 
-    ref = core_raster._open_raster(raster)
-    metadata = core_raster._raster_to_metadata(ref)
+    return out_path
 
-    x_res, y_res, x_pixels, y_pixels = gdal_utils.parse_raster_size(
-        target_size, target_in_pixels=target_in_pixels
-    )
 
-    out_format = gdal_utils.path_to_driver_raster(out_path)
+def raster_get_proximity(
+    raster: Union[str, gdal.Dataset, List[Union[str, gdal.Dataset]]],
+    target_value: Union[int, float] = 1,
+    unit: str = "geo",
+    out_path: Optional[Union[str, List[str]]] = None,
+    max_dist: Union[int, float] = 1000,
+    add_border: bool = False,
+    border_value: Union[int, float] = 0,
+    inverted: bool = False,
+    overwrite: bool = True,
+    prefix: str = "",
+    suffix: str = "",
+    add_uuid: bool = False,
+    add_timestamp: bool = False,
+) -> Union[str, List[str]]:
+    """
+    Calculate the proximity of input_raster to values.
+
+    Parameters
+    ----------
+    raster : Union[str, gdal.Dataset, List]
+        The raster(s) to use as input.
 
-    src_nodata = metadata["nodata_value"]
-    out_nodata = None
-    if dst_nodata == "infer":
-        dst_nodata = src_nodata
-    else:
-        assert isinstance(dst_nodata, (int, float, type(None))), "dst_nodata must be an int, float, 'infer', or 'None'"
-        out_nodata = dst_nodata
+    target_value : Union[int, float], optional
+        The value to use as target, default: 1.
 
-    if dtype is None:
-        dtype = metadata["datatype"]
+    unit : str, optional
+        The unit to use for the distance, GEO or PIXEL, default: "GEO".
 
-    core_utils.remove_if_required(out_path, overwrite)
+    out_path : Union[str, None, List], optional
+        The output path, default: None.
 
-    resampled = gdal.Warp(
-        out_path,
-        ref,
-        width=x_pixels,
-        height=y_pixels,
-        xRes=x_res,
-        yRes=y_res,
-        format=out_format,
-        outputType=gdal_enums.translate_str_to_gdal_dtype(dtype),
-        resampleAlg=gdal_enums.translate_resample_method(resample_alg),
-        creationOptions=gdal_utils.default_creation_options(creation_options),
-        srcNodata=metadata["nodata_value"],
-        dstNodata=out_nodata,
-        multithread=True,
-    )
+    max_dist : Union[int, float], optional
+        The maximum distance to use, default: 1000.
 
-    if resampled is None:
-        raise Exception(f"Error while resampling raster: {out_path}")
+    add_border : bool, optional
+        If True, a border will be added to the raster, default: False.
 
-    return out_path
+    border_value : Union[int, float], optional
+        The value to use for the border, default: 0.
 
+    inverted : bool, optional
+        If True, the target will be inversed, default: False.
 
-def resample_raster(
-    raster,
-    target_size,
-    out_path=None,
-    *,
-    target_in_pixels=False,
-    resample_alg="nearest",
-    creation_options=None,
-    dtype=None,
-    dst_nodata="infer",
-    prefix="",
-    suffix="",
-    add_uuid=False,
-    overwrite=True,
-):
-    """
-    Reprojects raster(s) given a target projection. </br>
-    **Beware** if your input is in latitude and longitude, you'll need to specify the target_size in degrees as well.
+    overwrite : bool, optional
+        If the output path exists already, should it be overwritten?, default: True.
 
-    ## Args:
-    `raster` (_str_/_list_/_gdal.Dataset): The raster(s) to reproject. </br>
-    `target_size` (_str_/_int_/_ogr.DataSource_/_gdal.Dataset_): The target resolution of the
-    raster. In the same unit as the projection of the raster.
-    It's better to reproject to a projected coordinate system for resampling.
-    If a raster is the target_size the function will read the pixel size from
-    that raster. </br>
-
-    ## Kwargs:
-    `target_in_pixels` (_bool_): If True, the target_size will be interpreted as the number of pixels. (Default: **False**) </br>
-    `out_path` (_str_/_None_): The output path. If not provided, the output path is inferred from the input. (Default: **None**) </br>
-    `resample_alg` (_str_): The resampling algorithm. (Default: **nearest**) </br>
-    `copy_if_same` (_bool_): If the input and output projections are the same, copy the input raster to the output path. (Default: **True**) </br>
-    `overwrite` (_bool_): If the output path already exists, overwrite it. (Default: **True**) </br>
-    `creation_options` (_list_/_None_): A list of creation options for the output raster. (Default: **None**) </br>
-    `dst_nodata` (_str_/_int_/_float_): The nodata value for the output raster. (Default: **infer**) </br>
-    `prefix` (_str_): The prefix to add to the output path. (Default: **""**) </br>
-    `suffix` (_str_): The suffix to add to the output path. (Default: **"_reprojected"**) </br>
-    `add_uuid` (_bool_): If True, add a UUID to the output path. (Default: **False**) </br>
+    prefix : str, optional
+        Prefix to add to the output, default: "".
 
-    ## Returns:
-    (_str_/_list_): The output path(s) of the resampled raster(s).
-    """
-    core_utils.type_check(raster, [str, gdal.Dataset, [str, gdal.Dataset]], "raster")
-    core_utils.type_check(target_size, [tuple, [int, float], int, float, str, gdal.Dataset], "target_size")
-    core_utils.type_check(target_in_pixels, [bool], "target_in_pixels")
-    core_utils.type_check(out_path, [str, [str], None], "out_path")
-    core_utils.type_check(resample_alg, [str], "resample_alg")
-    core_utils.type_check(overwrite, [bool], "overwrite")
-    core_utils.type_check(creation_options, [[str], None], "creation_options")
-    core_utils.type_check(dst_nodata, [str, int, float, None], "dst_nodata")
-    core_utils.type_check(dtype, [str, None], "dtype")
-    core_utils.type_check(prefix, [str], "prefix")
-    core_utils.type_check(suffix, [str], "postfix")
+    suffix : str, optional
+        Suffix to add to the output, default: "_proximity".
 
-    if core_utils.is_str_a_glob(raster):
-        raster = core_utils.parse_glob_path(raster)
+    add_uuid : bool, optional
+        Should a uuid be added to the output path?, default: False.
 
-    raster_list = core_utils.ensure_list(raster)
-    assert gdal_utils.is_raster_list(raster_list), f"Invalid raster in raster list: {raster_list}"
+    add_timestamp : bool, optional
+        Should a timestamp be added to the output path?, default: False.
 
-    path_list = gdal_utils.create_output_path_list(
-        raster_list,
-        out_path=out_path,
-        overwrite=overwrite,
+    Returns
+    -------
+    str
+        A path to a raster with the calculated proximity.
+    """
+    utils_base._type_check(raster, [str, gdal.Dataset, [str, gdal.Dataset]], "raster")
+    utils_base._type_check(target_value, [int, float], "target_value")
+    utils_base._type_check(unit, [str], "unit")
+    utils_base._type_check(out_path, [str, [str], None], "out_path")
+    utils_base._type_check(max_dist, [int, float], "max_dist")
+    utils_base._type_check(add_border, [bool], "add_border")
+    utils_base._type_check(border_value, [int, float], "border_value")
+    utils_base._type_check(inverted, [bool], "inverted")
+    utils_base._type_check(overwrite, [bool], "overwrite")
+    utils_base._type_check(prefix, [str], "prefix")
+    utils_base._type_check(suffix, [str], "suffix")
+    utils_base._type_check(add_uuid, [bool], "add_uuid")
+    utils_base._type_check(add_timestamp, [bool], "add_timestamp")
+
+    assert unit.lower() in ["geo", "pixel"], f"Invalid unit. {unit}"
+
+    input_is_list = isinstance(raster, list)
+    input_rasters = utils_io._get_input_paths(raster, "raster")
+    output_rasters = utils_io._get_output_paths(
+        input_rasters,
+        out_path,
+        in_place=False,
         prefix=prefix,
         suffix=suffix,
         add_uuid=add_uuid,
+        add_timestamp=add_timestamp,
+        change_ext="tif"
     )
 
-    resampled_rasters = []
-    for index, in_raster in enumerate(raster_list):
-        resampled_rasters.append(
-            _resample_raster(
-                in_raster,
-                target_size,
-                target_in_pixels=target_in_pixels,
-                out_path=path_list[index],
-                resample_alg=resample_alg,
-                overwrite=overwrite,
-                creation_options=creation_options,
-                dtype=dtype,
-                dst_nodata=dst_nodata,
-                prefix=prefix,
-                suffix=suffix,
-            )
-        )
-
-    if isinstance(raster, list):
-        return resampled_rasters
-
-    return resampled_rasters[0]
-
-
-def resample_array(arr, target_shape_pixels, resample_alg="nearest"):
-    """ Resample a numpy array using the GDAL algorithms. """
-    core_utils.type_check(arr, [np.ndarray, np.ma.MaskedArray], "arr")
-    core_utils.type_check(target_shape_pixels, [tuple, [int, float]], "target_shape_pixels")
-    core_utils.type_check(resample_alg, [str], "resample_alg")
-
-    if len(target_shape_pixels) > 2:
-        target_shape_pixels = target_shape_pixels[:2]
-
-    arr_as_raster = core_raster.create_raster_from_array(arr)
-    resampled = _resample_raster(arr_as_raster, target_shape_pixels, target_in_pixels=True, resample_alg=resample_alg)
-    out_arr = core_raster.raster_to_array(resampled)
+    utils_path._delete_if_required_list(output_rasters, overwrite)
+
+    output = []
+    for idx, in_raster in enumerate(input_rasters):
+        output.append(_raster_get_proximity(
+            in_raster,
+            target_value=target_value,
+            unit=unit.lower(),
+            out_path=output_rasters[idx],
+            max_dist=max_dist,
+            add_border=add_border,
+            border_value=border_value,
+            inverted=inverted,
+            overwrite=overwrite,
+        ))
 
-    gdal_utils.delete_if_in_memory(arr_as_raster)
-    gdal_utils.delete_if_in_memory(resampled)
+    if input_is_list:
+        return output
 
-    return out_arr
+    return output[0]
```

### Comparing `buteo-0.8.9/buteo/raster/shift.py` & `buteo-0.9.0/buteo/raster/vectorize.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,145 +1,146 @@
 """
-### Shift rasters. ###
+### Vectorize rasters. ###
 
-Module to shift the location of rasters in geographic coordinates.
+Module to turn rasters into vector representations.
 """
 
 # Standard library
 import sys; sys.path.append("../../")
+from typing import Union, Optional, List
 
 # External
-from osgeo import gdal
+from osgeo import gdal, ogr
 
 # Internal
-from buteo.utils import core_utils, gdal_utils
+from buteo.utils import (
+    utils_base,
+    utils_gdal,
+    utils_path,
+    utils_io
+)
 from buteo.raster import core_raster
 
 
 
-def _shift_raster(
-    raster,
-    shift_list,
-    out_path=None,
-    *,
-    overwrite=True,
-    creation_options=None,
+def _raster_vectorize(
+    raster: Union[str, gdal.Dataset],
+    out_path: Optional[str] = None,
+    band: int = 1,
 ):
     """ Internal. """
-    assert isinstance(shift_list, (list, tuple)), f"shift_list must be a list or a tuple. {shift_list}"
-    assert len(shift_list) == 2, f"shift_list must be a list or tuple with len 2 (x_shift, y_shift): {shift_list}"
+    meta = core_raster._get_basic_metadata_raster(raster)
+    opened = core_raster._raster_open(raster)
+    src_band = opened.GetRasterBand(band)
 
-    for shift in shift_list:
-        assert isinstance(shift, (int, float)), f"shift must be an int or a float: {shift}"
-
-    ref = core_raster._open_raster(raster)
-    metadata = core_raster._raster_to_metadata(ref)
-
-    x_shift, y_shift = shift_list
+    projection = meta["projection_osr"]
 
     if out_path is None:
-        raster_name = metadata["basename"]
-        out_path = gdal_utils.create_memory_path(raster_name, add_uuid=True)
+        out_path = utils_path._get_temp_filepath("vectorized_raster.gpkg")
     else:
-        if not core_utils.is_valid_output_path(out_path, overwrite=overwrite):
+        if not utils_path._check_is_valid_output_filepath(out_path, overwrite=True):
             raise ValueError(f"out_path is not a valid output path: {out_path}")
 
-    core_utils.remove_if_required(out_path, overwrite)
-
-    driver = gdal.GetDriverByName(gdal_utils.path_to_driver_raster(out_path))
-
-    shifted = driver.Create(
-        out_path,  # Location of the saved raster, ignored if driver is memory.
-        metadata["width"],  # Dataframe width in pixels (e.g. 1920px).
-        metadata["height"],  # Dataframe height in pixels (e.g. 1280px).
-        metadata["band_count"],  # The number of bands required.
-        metadata["datatype_gdal_raw"],  # Datatype of the destination.
-        gdal_utils.default_creation_options(creation_options),
-    )
-
-    new_transform = list(metadata["transform"])
-    new_transform[0] += x_shift
-    new_transform[3] += y_shift
-
-    shifted.SetGeoTransform(new_transform)
-    shifted.SetProjection(metadata["projection_wkt"])
+    utils_path._delete_if_required(out_path, overwrite=True)
 
-    src_nodata = metadata["nodata_value"]
+    driver_name = utils_gdal._get_vector_driver_name_from_path(out_path)
+    driver = ogr.GetDriverByName(driver_name)
 
-    for band in range(metadata["band_count"]):
-        origin_raster_band = ref.GetRasterBand(band + 1)
-        target_raster_band = shifted.GetRasterBand(band + 1)
+    datasource = driver.CreateDataSource(out_path)
+    layer = datasource.CreateLayer(out_path, srs=projection)
 
-        target_raster_band.WriteArray(origin_raster_band.ReadAsArray())
-        target_raster_band.SetNoDataValue(src_nodata)
-
-    if out_path is not None:
-        shifted = None
-        return out_path
-    else:
-        return shifted
-
-
-def shift_raster(
-    raster,
-    shift_list,
-    out_path=None,
-    *,
-    overwrite=True,
-    prefix="",
-    suffix="",
-    add_uuid=False,
-    creation_options=None,
-):
+    try:
+        gdal.Polygonize(src_band, None, layer, 0)
+    except:
+        raise RuntimeError(f"Error while vectorizing raster. {raster}") from None
+    finally:
+        datasource.FlushCache()
+        src_band = None
+        datasource = None
+
+    return out_path
+
+
+def raster_vectorize(
+    raster: Union[str, gdal.Dataset, List],
+    out_path: Optional[str] = None,
+    band: int = 1,
+    prefix: str = "",
+    suffix: str = "",
+    add_uuid: bool = False,
+    add_timestamp: bool = False,
+    overwrite: bool = True,
+) -> Union[str, List[str]]:
     """
-    Shifts a raster in a given direction.
-
-    ## Args:
-    `raster` (_str_/_list_/_gdal.Dataset_): The raster(s) to be shifted. </br>
-    `shift_list` (_list_/_tuple_): The shift in x and y direction. </br>
-
-    ## Kwargs:
-    `out_path` (_str_/_list_/_None_): The path to the output raster. If None, the raster is
-    created in memory. (Default: **None**)</br>
-    `overwrite` (_bool_): If True, the output raster will be overwritten if it already exists. (Default: **True**) </br>
-    `prefix` (_str_): The prefix to be added to the output raster name. (Default: **""**) </br>
-    `suffix` (_str_): The suffix to be added to the output raster name. (Default: **""**) </br>
-    `add_uuid` (_bool_): If True, a unique identifier will be added to the output raster name. (Default: **False**) </br>
-    `creation_options` (_list_/_None_): The creation options to be used when creating the output. (Default: **None**) </br>
+    Vectorizes a raster by turning it into polygons per unique value. Works
+    best on integer rasters.
 
-    ## Returns:
-    (_str_/_list_): The path(s) to the shifted raster(s).
+    Parameters
+    ----------
+    raster : Union[str, gdal.Dataset, List]
+        The raster(s) to vectorize.
+
+    out_path : Optional[str], optional
+        The path(s) to save the vectorized raster(s) to. Default: None
+    
+    band : int, optional
+        The band to vectorize. Default: 1
+
+    prefix : str, optional
+        The prefix to be added to the output raster name. Default: ""
+
+    suffix : str, optional
+        The suffix to be added to the output raster name. Default: ""
+
+    add_uuid : bool, optional
+        If True, a unique identifier will be added to the output raster name. Default: False
+
+    add_timestamp : bool, optional
+        If True, a timestamp will be added to the output raster name. Default: False
+
+    overwrite : bool, optional
+        If True, the output raster will be overwritten if it already exists. Default: True
+
+    Returns
+    -------
+    Union[str, List]
+        The path(s) to the vectorized raster(s).
     """
-    core_utils.type_check(raster, [str, gdal.Dataset, [str, gdal.Dataset]], "raster")
-    core_utils.type_check(shift_list, [[tuple, list]], "shift_list")
-    core_utils.type_check(out_path, [str, [str], None], "out_path")
-    core_utils.type_check(overwrite, [bool], "overwrite")
-    core_utils.type_check(creation_options, [[str], None], "creation_options")
-
-    raster_list = core_utils.ensure_list(raster)
-    assert gdal_utils.is_raster_list(raster_list), f"Invalid raster in raster list: {raster_list}"
-
-    path_list = gdal_utils.create_output_path_list(
-        raster_list,
-        out_path=out_path,
+    utils_base._type_check(raster, [str, gdal.Dataset, [str, gdal.Dataset]], "raster")
+    utils_base._type_check(out_path, [str, [str], None], "out_path")
+    utils_base._type_check(band, [int], "band")
+    utils_base._type_check(prefix, [str], "prefix")
+    utils_base._type_check(suffix, [str], "suffix")
+    utils_base._type_check(add_uuid, [bool], "add_uuid")
+    utils_base._type_check(add_timestamp, [bool], "add_timestamp")
+    utils_base._type_check(overwrite, [bool], "overwrite")
+
+    input_is_list = isinstance(raster, list)
+
+    input_list = utils_io._get_input_paths(raster, "raster")
+    output_list = utils_io._get_output_paths(
+        input_list,
+        out_path,
         overwrite=overwrite,
         prefix=prefix,
         suffix=suffix,
         add_uuid=add_uuid,
+        add_timestamp=add_timestamp,
+        change_ext="gpkg",
     )
 
-    shifted_rasters = []
-    for index, in_raster in enumerate(raster_list):
-        shifted_rasters.append(
-            _shift_raster(
+    utils_path._delete_if_required_list(output_list, overwrite)
+
+    vectorized_rasters = []
+    for idx, in_raster in enumerate(input_list):
+        vectorized_rasters.append(
+            _raster_vectorize(
                 in_raster,
-                shift_list,
-                out_path=path_list[index],
-                overwrite=overwrite,
-                creation_options=creation_options,
+                out_path=output_list[idx],
+                band=band,
             )
         )
 
-    if isinstance(raster, list):
-        return shifted_rasters
+    if input_is_list:
+        return vectorized_rasters
 
-    return shifted_rasters[0]
+    return vectorized_rasters[0]
```

### Comparing `buteo-0.8.9/buteo/raster/timeseries.py` & `buteo-0.9.0/buteo/array/timeseries.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 """ Time series analysis functions. """
 import numpy as np
 
 
-def robust_least_squares_slope(arr, std_threshold=1.0, splits=10, report_progress=True):
+def timeseries_least_square_slope(arr):
+    """ Compute the least squares slope for a set of data points along the last channel. """
+    assert arr.ndim == 3, "Input array must be 3D"
+
+    y = arr
+    x_range = np.arange(y.shape[-1], dtype=np.float32)
+    x = np.tile(x_range, (y.shape[0], y.shape[1], 1))
+
+    # Calculate the means
+    x_mean = np.mean(x, axis=2, keepdims=True)
+    y_mean = np.mean(y, axis=2, keepdims=True)
+
+    # Compute the least squares slope using vectorized operations
+    numerator = np.sum((x - x_mean) * (y - y_mean), axis=2, keepdims=True)
+    denominator = np.sum((x - x_mean) ** 2, axis=2, keepdims=True)
+    slope = numerator / denominator
+
+    return slope
+
+
+def timeseries_robust_least_squares_slope(arr, std_threshold=1.0, splits=10, report_progress=True):
     """ Compute the robust least squares slope for a set of data points along the last channel. """
     assert arr.ndim == 3, "Input array must be 3D"
     assert arr.shape[0] > splits, "Input array must have at least splits rows"
     y_list = np.array_split(arr, splits, axis=0)
     slope_list = []
 
     for idx, y in enumerate(y_list):
@@ -30,11 +50,14 @@
         # Mask out values outside of a STD threshold
         mask = np.logical_and(
             slopes >= (median_slope - (mad_std_slope * std_threshold)),
             slopes <= (median_slope + (mad_std_slope * std_threshold)),
         )
 
         # Calculate slope using the masked median of the slopes
-        slope = np.ma.median(np.ma.masked_array(slopes, mask=~mask), axis=2, keepdims=True).filled(0)
+        masked_slopes = np.ma.masked_array(slopes, mask=~mask)
+
+        # Still takes into account the masked values
+        slope = np.ma.median(masked_slopes, axis=2, keepdims=True).filled(0)
         slope_list.append(slope)
 
     return np.vstack(slope_list)
```

### Comparing `buteo-0.8.9/buteo/raster/warp.py` & `buteo-0.9.0/buteo/raster/clip.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,292 +1,374 @@
 """
-### GDAL Warp functions  ###
+### Clip rasters ###
 
-Module to wrap the functionality of GDAL's gdalwarp.
+Clips a raster using a vector geometry or the extents of a raster.
 """
 
 # Standard library
 import sys; sys.path.append("../../")
-from uuid import uuid4
+from typing import Union, List, Optional
+from warnings import warn
 
 # External
-from osgeo import gdal, ogr, osr
+from osgeo import gdal, ogr
+import numpy as np
 
 # Internal
-from buteo.utils import core_utils, gdal_utils, bbox_utils, gdal_enums
+from buteo.utils import (
+    utils_io,
+    utils_gdal,
+    utils_base,
+    utils_bbox,
+    utils_path,
+    utils_translate,
+)
 from buteo.raster import core_raster
 from buteo.vector import core_vector
+from buteo.vector.reproject import _vector_reproject
 
 
-
-def _warp_raster(
-    raster,
-    out_path=None,
+def _raster_clip(
+    raster: Union[str, List[str], gdal.Dataset, List[gdal.Dataset]],
+    clip_geom: Union[str, ogr.DataSource, ogr.Layer, List[ogr.Layer], List[ogr.DataSource]],
+    out_path: Optional[Union[str, List[str]]] = None,
     *,
-    projection=None,
-    clip_geom=None,
-    target_size=None,
-    target_in_pixels=False,
-    resample_alg="nearest",
-    crop_to_geom=True,
-    all_touch=False,
-    adjust_bbox=False,
-    src_nodata="infer",
-    dst_nodata="infer",
-    layer_to_clip=0,
-    prefix="",
-    suffix="_resampled",
-    overwrite=True,
-    creation_options=None,
+    resample_alg: str = "nearest",
+    crop_to_geom: bool = True,
+    adjust_bbox: bool = True,
+    all_touch: bool = True,
+    to_extent: bool = False,
+    overwrite: bool = True,
+    creation_options: Optional[List] = None,
+    dst_nodata: str = "infer",
+    src_nodata: str = "infer",
+    layer_to_clip: int = 0,
+    prefix: str = "",
+    suffix: str = "",
+    verbose: int = 1,
+    ram: float = 0.8,
+    ram_max: Optional[int] = None,
+    ram_min: Optional[int] = 100,
 ):
-    """ Internal. """
-    if out_path is None:
-        out_path = gdal_utils.create_memory_path(
-            out_path,
-            prefix=prefix,
-            suffix=suffix,
-            add_uuid=True,
-        )
+    """
+    INTERNAL.
+    Clips a raster(s) using a vector geometry or the extents of a raster.
+    """
+    path_list = utils_io._get_output_paths(
+        raster,
+        out_path,
+        prefix=prefix,
+        suffix=suffix,
+        add_uuid=out_path is None,
+    )
+    assert utils_path._check_is_valid_output_path_list(path_list, overwrite), (
+        f"Unable to parse out_path: {out_path}"
+    )
+
+    clip_ds = None
+
+    memory_files = []
+
+    if isinstance(clip_geom, ogr.Geometry):
+        clip_geom = utils_bbox._get_vector_from_geom(clip_geom)
+        clip_geom = utils_gdal._get_path_from_dataset(clip_geom)
+
+    # Input is a vector.
+    if utils_gdal._check_is_vector(clip_geom):
+        clip_ds = core_vector._vector_open(clip_geom)
+
+        # TODO: Fix potential memory leak
+        if clip_ds.GetLayerCount() > 1:
+            clip_ds = core_vector.vector_filter_layer(clip_ds, layer_name_or_idx=layer_to_clip, add_uuid=True)
+            memory_files.append(clip_ds)
+
+        clip_metadata = core_vector._get_basic_metadata_vector(clip_ds)
+
+        if to_extent:
+            clip_ds = utils_bbox._get_vector_from_bbox(clip_metadata["bbox"], clip_metadata["projection_osr"])
+            memory_files.append(clip_ds)
+
+        if isinstance(clip_ds, ogr.DataSource):
+            clip_ds = clip_ds.GetName()
+
+    # Input is a raster (use extent)
+    elif utils_gdal._check_is_raster(clip_geom):
+        clip_metadata = core_raster._get_basic_metadata_raster(clip_geom)
+        clip_ds = utils_bbox._get_vector_from_bbox(clip_metadata["bbox"], clip_metadata["projection_osr"])
+        memory_files.append(clip_ds)
+    else:
+        if utils_path._check_file_exists(clip_geom):
+            raise ValueError(f"Unable to parse clip geometry: {clip_geom}")
+        else:
+            raise ValueError(f"Unable to locate clip geometry {clip_geom}")
 
-    origin = core_raster._open_raster(raster)
-    raster_metadata = core_raster._raster_to_metadata(origin)
+    if clip_ds is None:
+        raise ValueError(f"Unable to parse input clip geom: {clip_geom}")
 
     # options
     warp_options = []
     if all_touch:
         warp_options.append("CUTLINE_ALL_TOUCHED=TRUE")
     else:
         warp_options.append("CUTLINE_ALL_TOUCHED=FALSE")
 
+    origin_layer = core_raster.raster_open(raster)
+
+    raster_metadata = core_raster._get_basic_metadata_raster(raster)
     origin_projection = raster_metadata["projection_osr"]
-    origin_extent = raster_metadata["get_bbox_as_vector_latlng"]() # pylint: disable=not-callable
 
-    target_projection = origin_projection
-    if projection is not None:
-        target_projection = gdal_utils.parse_projection(projection)
-
-    if clip_geom is not None:
-        if gdal_utils.is_raster(clip_geom):
-            opened_raster = core_raster._open_raster(clip_geom)
-            clip_metadata_raster = core_raster._raster_to_metadata(opened_raster)
-            clip_ds = clip_metadata_raster["get_bbox_as_vector"]() # pylint: disable=not-callable
-            clip_metadata = core_vector._vector_to_metadata(clip_ds)
-        elif gdal_utils.is_vector(clip_geom):
-            clip_ds = core_vector.open_vector(clip_geom)
-            clip_metadata = core_vector._vector_to_metadata(clip_ds)
-        else:
-            if core_utils.file_exists(clip_geom):
-                raise ValueError(f"Unable to parse clip geometry: {clip_geom}")
-            else:
-                raise ValueError(f"Unable to find clip geometry {clip_geom}")
-
-        if layer_to_clip > (clip_metadata["layer_count"] - 1):
-            raise ValueError("Requested an unable layer_to_clip.")
-
-        clip_projection = clip_metadata["projection_osr"]
-        clip_extent = clip_metadata["get_bbox_as_vector_latlng"]() # pylint: disable=not-callable
-
-        # Fast check: Does the extent of the two inputs overlap?
-        if not origin_extent.Intersects(clip_extent):
-            raise Exception("Clipping geometry did not intersect raster.")
-
-        # Check if projections match, otherwise reproject target geom.
-        if not target_projection.IsSame(clip_projection):
-            clip_metadata["bbox"] = bbox_utils.reproject_bbox(
+    # Fast check: Does the extent of the two inputs overlap?
+    has_inf = True in [np.isinf(val) for val in raster_metadata["bbox_latlng"]]
+    if not has_inf and not utils_bbox._check_bboxes_intersect(raster_metadata["bbox_latlng"], clip_metadata["bbox_latlng"]):
+        raise ValueError(f"Geometries of {raster} and {clip_geom} did not intersect.")
+
+    if not origin_projection.IsSame(clip_metadata["projection_osr"]):
+        clip_ds = _vector_reproject(clip_ds, origin_projection)
+        clip_metadata = core_vector._get_basic_metadata_vector(clip_ds)
+        memory_files.append(clip_ds)
+
+    output_bounds = raster_metadata["bbox"]
+
+    if crop_to_geom:
+
+        if adjust_bbox:
+            output_bounds = utils_bbox._get_aligned_bbox_to_pixel_size(
+                raster_metadata["bbox"],
                 clip_metadata["bbox"],
-                clip_projection,
-                target_projection,
-            )
-
-        # The extent needs to be reprojected to the target.
-        # this ensures that adjust_bbox works.
-        output_bounds = bbox_utils.reproject_bbox(
-            raster_metadata["extent"],
-            origin_projection,
-            target_projection,
-        )
-
-        if crop_to_geom:
-
-            if adjust_bbox:
-                output_bounds = bbox_utils.align_bboxes_to_pixel_size(
-                    raster_metadata["bbox"],
-                    clip_metadata["bbox"],
-                    raster_metadata["pixel_width"],
-                    raster_metadata["pixel_height"],
-                )
-
-            else:
-                output_bounds = clip_metadata["bbox"]
-
-        if clip_metadata["layer_count"] > 1:
-            clip_ds = core_vector._vector_to_memory(
-                clip_ds,
-                memory_path=f"clip_geom_{uuid4().int}.gpkg",
-                layer_to_extract=layer_to_clip,
+                raster_metadata["pixel_width"],
+                raster_metadata["pixel_height"],
             )
-        elif not isinstance(clip_ds, str):
-            clip_ds = core_vector._vector_to_memory(
-                clip_ds,
-                memory_path=f"clip_geom_{uuid4().int}.gpkg",
-            )
-
-        if clip_ds is None:
-            raise ValueError(f"Unable to parse input clip geom: {clip_geom}")
-
-    x_res, y_res, x_pixels, y_pixels = gdal_utils.parse_raster_size(
-        target_size, target_in_pixels=target_in_pixels
-    )
+        else:
+            output_bounds = clip_metadata["bbox"]
 
-    out_format = gdal_utils.path_to_driver_raster(out_path)
+    # formats
+    out_name = path_list[0]
+    out_format = utils_gdal._get_raster_driver_name_from_path(out_name)
+    out_creation_options = utils_gdal._get_default_creation_options(creation_options)
 
     # nodata
-    out_nodata = None
-    if src_nodata is not None:
-        out_nodata = raster_metadata["nodata_value"]
+    if src_nodata == "infer":
+        src_nodata = raster_metadata["nodata_value"]
+    elif isinstance(src_nodata, (int, float)) or src_nodata is None:
+        src_nodata = float(src_nodata)
     else:
-        if dst_nodata == "infer":
+        raise ValueError(f"src_nodata must be an int, float or None: {src_nodata}")
+
+    out_nodata = None
+    if dst_nodata == "infer":
+        if src_nodata == "infer":
             out_nodata = raster_metadata["nodata_value"]
         else:
-            out_nodata = dst_nodata
+            out_nodata = utils_translate._get_default_nodata_value(raster_metadata["dtype_gdal"])
+    elif isinstance(dst_nodata, (int, float)) or dst_nodata is None:
+        out_nodata = dst_nodata
+    else:
+        raise ValueError(f"Unable to parse nodata_value: {dst_nodata}")
+
+    if not utils_translate._check_is_value_within_dtype_range(out_nodata, raster_metadata["dtype"]):
+        warn("Nodata value is outside of the range of the input raster's dtype. Setting to None.")
+        out_nodata = None
 
     # Removes file if it exists and overwrite is True.
-    core_utils.remove_if_required(out_path, overwrite)
+    utils_path._delete_if_required(out_path, overwrite)
 
-    warped = gdal.Warp(
-        out_path,
-        origin,
-        xRes=x_res,
-        yRes=y_res,
-        width=x_pixels,
-        height=y_pixels,
-        cutlineDSName=clip_ds,
-        outputBounds=bbox_utils.convert_geom_to_bbox(output_bounds),
+    if verbose == 0:
+        gdal.PushErrorHandler("CPLQuietErrorHandler")
+
+    options = gdal.WarpOptions(
         format=out_format,
-        srcSRS=origin_projection,
-        dstSRS=target_projection,
-        resampleAlg=gdal_enums.translate_resample_method(resample_alg),
-        creationOptions=gdal_utils.default_creation_options(creation_options),
+        resampleAlg=utils_translate._translate_resample_method(resample_alg),
+        targetAlignedPixels=False,
+        outputBounds=utils_bbox._get_gdal_bbox_from_ogr_bbox(output_bounds),
+        xRes=raster_metadata["pixel_width"],
+        yRes=raster_metadata["pixel_height"],
+        cutlineDSName=clip_ds,
+        cropToCutline=False,
+        creationOptions=out_creation_options,
+        warpMemoryLimit=utils_gdal._get_dynamic_memory_limit(ram, min_mb=ram_min, max_mb=ram_max),
         warpOptions=warp_options,
         srcNodata=src_nodata,
         dstNodata=out_nodata,
-        targetAlignedPixels=False,
-        cropToCutline=False,
         multithread=True,
     )
 
-    if warped is None:
-        raise Exception(f"Error while warping raster: {raster}")
+    clipped = gdal.Warp(
+        out_name,
+        origin_layer,
+        options=options,
+    )
+
+    utils_gdal.delete_dataset_if_in_memory_list(memory_files)
+
+    if verbose == 0:
+        gdal.PopErrorHandler()
 
-    return out_path
+    if clipped is None:
+        raise ValueError("Error while clipping raster.")
 
+    return out_name
 
-def warp_raster(
-    raster,
-    out_path=None,
+
+def raster_clip(
+    raster: Union[str, gdal.Dataset, List[Union[str, gdal.Dataset]]],
+    clip_geom: Union[str, ogr.DataSource, gdal.Dataset, ogr.Geometry],
+    out_path: Optional[str] = None,
     *,
-    projection=None,
-    clip_geom=None,
-    target_size=None,
-    target_in_pixels=False,
-    resample_alg="nearest",
-    crop_to_geom=True,
-    all_touch=False,
-    adjust_bbox=False,
-    src_nodata="infer",
-    dst_nodata="infer",
-    layer_to_clip=0,
-    prefix="",
-    suffix="_resampled",
-    add_uuid=False,
-    overwrite=True,
-    creation_options=None,
+    resample_alg: str = "nearest",
+    crop_to_geom: bool = True,
+    adjust_bbox: bool = False,
+    all_touch: bool = False,
+    to_extent: bool = False,
+    layer_to_clip: int = 0,
+    dst_nodata: Union[float, int, str] = "infer",
+    src_nodata: Union[float, int, str] = "infer",
+    creation_options: Optional[List[str]] = None,
+    add_uuid: bool = False,
+    add_timestamp: bool = False,
+    prefix: str = "",
+    suffix: str = "",
+    overwrite: bool = True,
+    verbose: int = 0,
+    ram: float = 0.8,
+    ram_max: Optional[int] = None,
+    ram_min: Optional[int] = 100,
 ):
     """
-    Warps a raster into a target raster. </br>
+    Clips a raster(s) using a vector geometry or the extents of a raster.
+
+    Parameters
+    ----------
+    raster : str or gdal.Dataset or list of str/gdal.Dataset
+        The raster(s) to clip.
+
+    clip_geom : str or ogr.DataSource, gdal.Dataset or ogr.Geometry
+        The geometry to use to clip the raster.
+
+    out_path : str or list or None, optional
+        The path(s) to save the clipped raster to. If None, a memory raster is created. Default: None.
+
+    resample_alg : str, optional
+        The resampling algorithm to use. Options include: nearest, bilinear, cubic, cubicspline, lanczos, 
+        average, mode, max, min, median, q1, q3, sum, rms. Default: "nearest".
+
+    crop_to_geom : bool, optional
+        If True, the output raster will be cropped to the extent of the clip geometry. Default: True.
+
+    adjust_bbox : bool, optional
+        If True, the output raster will have its bbox adjusted to match the clip geometry. Default: False.
+
+    all_touch : bool, optional
+        If true, all pixels touching the clipping geometry will be included. Default: False.
+
+    to_extent : bool, optional
+        If True, the output raster will be cropped to the extent of the clip geometry. Default: False.
 
-    Please be aware that all_touch does not work if target_size is set.
-    If all_touch is required while resampling. Do it in two steps:
-    resample -> warp or resample -> clip.
-
-    ## Args:
-    `raster` (_str_/_list_/_gdal.Dataset_): The raster(s) to warp.
-
-    ## Kwargs:
-    `out_path` (_str_/_list_/_None_): The path to the output raster(s). If not set, a memory raster is created. (Default: **None**) </br>
-    `projection` (_str_/_osr.SpatialReference_/_gdal.Dataset_/_ogr.DataSource_): The projection of the output raster. If not set, the projection of the input raster is used. (Default: **None**) </br>
-    `clip_geom` (_str_/_gdal.Dataset_/_ogr.DataSource_): The geometry to clip the raster to. (Default: **None**) </br>
-    `target_size` (_tuple_/_None_): The target size of the output raster. If not set, the size of the input raster is used. (Default: **None**) </br>
-    `target_in_pixels` (_bool_): If True, the target size is in pixels. If False, the target size is in map units. (Default: **False**) </br>
-    `resample_alg` (_str_): The resampling algorithm. (Default: **nearest**) </br>
-    `crop_to_geom` (_bool_): If True, the output raster is cropped to the extent of the clip geometry. (Default: **True**) </br>
-    `all_touch` (_bool_): If True, all pixels touching the clipping geometry is included. (Default: **False**) </br>
-    `adjust_bbox` (_bool_): If True, the bounding box of the output raster is adjusted to align with the clipping geometry. (Default: **False**) </br>
-    `src_nodata` (_str_/_int_/_float_/_None_): The nodata value of the input raster. If not set, the nodata value of the input raster is used. (Default: **infer**) </br>
-    `dst_nodata` (_str_/_int_/_float_/_None_): The nodata value of the output raster. If not set, the nodata value of the input raster is used. (Default: **infer**) </br>
-    `layer_to_clip` (_int_): The layer to clip the raster to. (Default: **0**) </br>
-    `prefix` (_str_): The prefix of the output raster. (Default: **""**) </br>
-    `suffix` (_str_): The suffix of the output raster. (Default: **"_resampled"**) </br>
-    `add_uuid` (_bool_): If True, a unique identifier is added to the output raster. (Default: **False**) </br>
-    `overwrite` (_bool_): If True, the output raster is overwritten if it already exists. (Default: **True**) </br>
-    `creation_options` (_list_): The creation options of the output raster. (Default: **None**) </br>
+    prefix : str, optional
+        The prefix to use for the output raster. Default: "".
 
-    ## Returns:
-    (_str_/_list_): The path to the warped output raster(s).
+    suffix : str, optional
+        The suffix to use for the output raster. Default: "".
+
+    overwrite : bool, optional
+        If True, the output raster will be overwritten if it already exists. Default: True.
+
+    creation_options : list or None, optional
+        A list of creation options to pass to gdal. Default: None.
+
+    dst_nodata : int or float or None, optional
+        The nodata value to use for the output raster. Default: "infer".
+
+    src_nodata : int or float or None, optional
+        The nodata value to use for the input raster. Default: "infer".
+
+    layer_to_clip : int or str, optional
+        The layer ID or name in the vector to use for clipping. Default: 0.
+
+    verbose : int, optional
+        The verbosity level. Default: 0.
+
+    add_uuid : bool, optional
+        If True, a UUID will be added to the output raster. Default: False.
+
+    add_timestamp : bool, optional
+        If True, a timestamp will be added to the output raster. Default: False.
+
+    ram : float, optional
+        The proportion of total ram to allow usage of. Default: 0.8.
+    
+    ram_max: int, optional
+        The maximum amount of ram to use in MB. Default: None.
+    
+    ram_min: int, optional
+        The minimum amount of ram to use in MB. Default: 100.
+
+    Returns
+    -------
+    str or list
+        A string or list of strings representing the path(s) to the clipped raster(s).
     """
-    core_utils.type_check(raster, [str, gdal.Dataset, [str, gdal.Dataset]], "raster")
-    core_utils.type_check(out_path, [str, [str], None], "out_path")
-    core_utils.type_check(projection, [int, str, gdal.Dataset, ogr.DataSource, osr.SpatialReference, None], "projection")
-    core_utils.type_check(clip_geom, [str, ogr.DataSource], "clip_geom")
-    core_utils.type_check(target_size, [tuple, list, int, float, str, gdal.Dataset, None], "target_size")
-    core_utils.type_check(target_in_pixels, [bool], "target_in_pixels")
-    core_utils.type_check(resample_alg, [str], "resample_alg")
-    core_utils.type_check(crop_to_geom, [bool], "crop_to_geom")
-    core_utils.type_check(all_touch, [bool], "all_touch")
-    core_utils.type_check(adjust_bbox, [bool], "adjust_bbox")
-    core_utils.type_check(src_nodata, [str, int, float], "src_nodata")
-    core_utils.type_check(dst_nodata, [str, int, float], "dst_nodata")
-    core_utils.type_check(layer_to_clip, [int], "layer_to_clip")
-    core_utils.type_check(prefix, [str], "prefix")
-    core_utils.type_check(suffix, [str], "postfix")
-    core_utils.type_check(add_uuid, [bool], "add_uuid")
-    core_utils.type_check(overwrite, [bool], "overwrite")
-    core_utils.type_check(creation_options, [[str], None], "creation_options")
-
-    raster_list = core_utils.ensure_list(raster)
-    path_list = gdal_utils.create_output_path_list(
-        raster_list,
-        out_path=out_path,
+    utils_base._type_check(raster, [str, gdal.Dataset, [str, gdal.Dataset]], "raster")
+    utils_base._type_check(clip_geom, [str, ogr.DataSource, gdal.Dataset, ogr.Geometry], "clip_geom")
+    utils_base._type_check(out_path, [[str], str, None], "out_path")
+    utils_base._type_check(resample_alg, [str], "resample_alg")
+    utils_base._type_check(crop_to_geom, [bool], "crop_to_geom")
+    utils_base._type_check(adjust_bbox, [bool], "adjust_bbox")
+    utils_base._type_check(all_touch, [bool], "all_touch")
+    utils_base._type_check(to_extent, [bool], "to_extent")
+    utils_base._type_check(dst_nodata, [str, int, float, None], "dst_nodata")
+    utils_base._type_check(src_nodata, [str, int, float, None], "src_nodata")
+    utils_base._type_check(layer_to_clip, [int], "layer_to_clip")
+    utils_base._type_check(overwrite, [bool], "overwrite")
+    utils_base._type_check(creation_options, [[str], None], "creation_options")
+    utils_base._type_check(prefix, [str], "prefix")
+    utils_base._type_check(suffix, [str], "postfix")
+    utils_base._type_check(verbose, [int], "verbose")
+    utils_base._type_check(add_uuid, [bool], "uuid")
+    utils_base._type_check(add_timestamp, [bool], "timestamp")
+    utils_base._type_check(ram, [float], "ram")
+    utils_base._type_check(ram_max, [int, None], "ram_max")
+    utils_base._type_check(ram_min, [int, None], "ram_min")
+
+    input_is_list = isinstance(raster, list)
+    input_rasters = utils_io._get_input_paths(raster, "raster")
+    out_path_list = utils_io._get_output_paths(
+        raster,
+        out_path,
         prefix=prefix,
         suffix=suffix,
         add_uuid=add_uuid,
+        add_timestamp=add_uuid,
+        change_ext="tif",
         overwrite=overwrite,
     )
+    utils_path._delete_if_required_list(out_path_list, overwrite)
 
     output = []
-    for index, in_raster in enumerate(raster_list):
+    for index, in_raster in enumerate(input_rasters):
         output.append(
-            _warp_raster(
+            _raster_clip(
                 in_raster,
-                out_path=path_list[index],
-                projection=projection,
-                clip_geom=clip_geom,
-                target_size=target_size,
-                target_in_pixels=target_in_pixels,
+                clip_geom,
+                out_path=out_path_list[index],
                 resample_alg=resample_alg,
                 crop_to_geom=crop_to_geom,
-                all_touch=all_touch,
                 adjust_bbox=adjust_bbox,
-                overwrite=overwrite,
-                creation_options=creation_options,
-                src_nodata=src_nodata,
+                all_touch=all_touch,
+                to_extent=to_extent,
                 dst_nodata=dst_nodata,
+                src_nodata=src_nodata,
                 layer_to_clip=layer_to_clip,
+                overwrite=overwrite,
+                creation_options=creation_options,
                 prefix=prefix,
                 suffix=suffix,
+                verbose=verbose,
+                ram=ram,
+                ram_max=ram_max,
+                ram_min=ram_min,
             )
         )
 
-    if isinstance(raster, list):
+    if input_is_list:
         return output
 
     return output[0]
```

### Comparing `buteo-0.8.9/buteo/utils/bbox_utils.py` & `buteo-0.9.0/buteo/utils/utils_bbox.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,140 +11,152 @@
 
 The GDAL geotransform is a list of six parameters:</br>
 `x_min, pixel_width, row_skew, y_max, column_skew, pixel_height (negative for north-up)`
 """
 
 # Standard library
 import sys; sys.path.append("../../")
+from typing import List, Union, Dict, Any, Optional
 from uuid import uuid4
 
 # External
 import numpy as np
 from osgeo import ogr, osr, gdal
 
 # Internal
-from buteo.utils import core_utils, gdal_utils
+from buteo.utils import utils_base, utils_projection, utils_path, utils_gdal
 
 
-def is_valid_bbox(bbox_ogr):
+
+def _check_is_valid_bbox(bbox_ogr: List[Union[int, float]]) -> bool:
     """
     Checks if a bbox is valid.
 
-    A valid ogr formatted bbox has the form: </br>
-    `[x_min, x_max, y_min, y_max]`
-
-    ## Args:
-    `bbox_ogr` (_list_): An OGR formatted bbox. </br>
+    A valid ogr formatted bbox has the form:
+        `[x_min, x_max, y_min, y_max]`
 
-    ## Returns:
-    (_bool_): **True** if the bbox is valid, **False** otherwise.
+    Parameters
+    ----------
+    bbox_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+
+    Returns
+    -------
+    bool
+        True if the bbox is valid, False otherwise.
     """
     if not isinstance(bbox_ogr, list):
         return False
 
     if len(bbox_ogr) != 4:
         return False
 
     for val in bbox_ogr:
-        if not core_utils.is_number(val):
+        if not utils_base._check_variable_is_number_type(val):
             return False
 
     x_min, x_max, y_min, y_max = bbox_ogr
 
+    if x_min >= x_max or y_min >= y_max:
+        return False
+
     if True in [np.isinf(val) for val in bbox_ogr]:
         return True
 
-    if x_min > x_max or y_min > y_max:
-        return False
-
     return True
 
 
-def is_valid_bbox_latlng(bbox_ogr_latlng):
+def _check_is_valid_bbox_latlng(bbox_ogr_latlng: List[Union[int, float]]) -> bool:
     """
     Checks if a bbox is valid and latlng.
 
-    A valid ogr formatted bbox has the form: </br>
-    `[x_min, x_max, y_min, y_max]`
-
-    ## Args:
-    `bbox_ogr_latlng` (_list_): An OGR formatted bbox. </br>
+    A valid ogr formatted bbox has the form:
+        `[x_min, x_max, y_min, y_max]`
 
-    ## Returns:
-    (_bool_): **True** if the bbox is valid, **False** otherwise.
+    Parameters
+    ----------
+    bbox_ogr_latlng : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+        
+    Returns
+    -------
+    bool
+        True if the bbox is valid, False otherwise.
     """
-    if not is_valid_bbox(bbox_ogr_latlng):
+    if not _check_is_valid_bbox(bbox_ogr_latlng):
         return False
 
     x_min, x_max, y_min, y_max = bbox_ogr_latlng
     if x_min < -180 or x_max > 180 or y_min < -90 or y_max > 90:
         return False
 
     return True
 
 
-def is_valid_geotransform(geotransform):
+def _check_is_valid_geotransform(geotransform: List[Union[int, float]]) -> bool:
     """
     Checks if a geotransform is valid.
 
-    A valid geotransform has the form: </br>
+    A valid geotransform has the form:
     `[x_min, pixel_width, row_skew, y_max, column_skew, pixel_height]`
 
-    ## Args:
-    `geotransform` (_list_/_tuple_): A GDAL formatted geotransform.
-
-    ## Returns:
-    (_bool_): **True** if the geotransform is valid, **False** otherwise.
+    Parameters
+    ----------
+    geotransform : list
+        A GDAL formatted geotransform.
+        `[x_min, pixel_width, row_skew, y_max, column_skew, pixel_height]`
+        pixel_height is negative for north up.
+
+    Returns
+    -------
+    bool
+        True if the geotransform is valid, False otherwise.
     """
     if not isinstance(geotransform, (list, tuple)):
         return False
 
     if len(geotransform) != 6:
         return False
 
     for val in geotransform:
-        if not core_utils.is_number(val):
+        if not utils_base._check_variable_is_number_type(val):
             return False
 
     return True
 
 
-def ensure_negative(number):
-    """
-    Ensures that a valid is negative. If the number is positive, it is made negative.
-
-    ## Args:
-    `number` (_int_/_float_): A float or int number. </br>
-
-    ## Returns:
-    (_int_/_float_): The same number made **negative** if necesary.
-    """
-    assert core_utils.is_number(number), f"number must be a number. Received: {number}"
-
-    if number <= 0:
-        return -number
-
-    return number
-
-
-def get_pixel_offsets(geotransform, bbox_ogr):
+def _get_pixel_offsets(
+    geotransform: List[Union[int, float]],
+    bbox_ogr: List[Union[int, float]],
+):
     """
     Get the pixels offsets for a bbox and a geotransform.
 
-    ## Args:
-    `geotransform` (_list_/_tuple_): A GDAL GeoTransform. </br>
-    `bbox_ogr` (_list_): An OGR formatted bbox. </br>
-
-    ## Returns:
-    (_list_): A list of pixel offsets. `[x_start, y_start, x_size, y_size]`
+    Parameters
+    ----------
+    geotransform : list
+        A GDAL formatted geotransform.
+        `[x_min, pixel_width, row_skew, y_max, column_skew, pixel_height]`
+        pixel_height is negative for north up.
+
+    bbox_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+
+    Returns
+    -------
+    list
+        A list of pixel offsets. `[x_start, y_start, x_size, y_size]`
     """
-    assert is_valid_geotransform(
+    assert _check_is_valid_geotransform(
         geotransform
     ), f"geotransform must be a list of length six. Received: {geotransform}."
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox_ogr
     ), f"bbox_ogr must be a valid OGR formatted bbox. Received: {bbox_ogr}."
 
     x_min, x_max, y_min, y_max = bbox_ogr
 
     origin_x = geotransform[0]
     origin_y = geotransform[3]
@@ -155,70 +167,97 @@
     y_start = int(np.rint((y_max - origin_y) / pixel_height))
     x_size = int(np.rint((x_max - x_min) / pixel_width))
     y_size = int(np.rint((y_min - y_max) / pixel_height))
 
     return [x_start, y_start, x_size, y_size]
 
 
-def get_bbox_from_geotransform(geotransform, raster_x_size, raster_y_size):
+def _get_bbox_from_geotransform(
+    geotransform: List[Union[int, float]],
+    raster_x_size: int,
+    raster_y_size: int,
+) -> List[Union[int, float]]:
     """
     Get an OGR bounding box from a geotransform and raster sizes.
 
-    ## Args:
-    `geotransform` (_list_/_tuple_): A GDAL GeoTransform. </br>
-    `raster_x_size` (_int_): The number of pixels in the x direction. </br>
-    `raster_y_size` (_int_): The number of pixels in the y direction. </br>
-
-    ## Returns:
-    (_list_): An OGR formatted bbox. `[x_min, x_max, y_min, y_max]`
+    Parameters
+    ----------
+    geotransform : list
+        A GDAL formatted geotransform.
+        `[x_min, pixel_width, row_skew, y_max, column_skew, pixel_height]`
+
+    raster_x_size : int
+        The number of pixels in the x direction.
+
+    raster_y_size : int
+        The number of pixels in the y direction.
+
+    Returns
+    -------
+    list
+        An OGR formatted bbox. `[x_min, x_max, y_min, y_max]`
     """
-    assert is_valid_geotransform(
+    assert _check_is_valid_geotransform(
         geotransform
     ), f"geotransform was not a valid geotransform. Received: {geotransform}"
 
     x_min, pixel_width, _row_skew, y_max, _column_skew, pixel_height = geotransform
 
     x_max = x_min + (raster_x_size * pixel_width)
     y_min = y_max + (raster_y_size * pixel_height)
 
     return [x_min, x_max, y_min, y_max]
 
 
-def get_bbox_from_raster(raster_dataframe):
+def _get_bbox_from_raster(
+    raster_dataframe: gdal.Dataset,
+) -> List[Union[int, float]]:
     """
     Gets an OGR bounding box from a GDAL raster dataframe.
+    The bounding box is in the same projection as the raster.
 
-    ## Args:
-    `raster_dataframe` (_gdal.DataFrame_): A GDAL raster dataframe. </br>
-
-    ## Returns:
-    (_list_): An OGR formatted bbox. `[x_min, x_max, y_min, y_max]`
+    Parameters
+    ----------
+    raster_dataframe : gdal.Dataset
+        A GDAL raster dataframe.
+
+    Returns
+    -------
+    list
+        An OGR formatted bbox. `[x_min, x_max, y_min, y_max]`
     """
     assert isinstance(
         raster_dataframe, gdal.Dataset
     ), f"raster_dataframe was not a gdal.Datasource. Received: {raster_dataframe}"
 
-    bbox = get_bbox_from_geotransform(
+    bbox = _get_bbox_from_geotransform(
         raster_dataframe.GetGeoTransform(),
         raster_dataframe.RasterXSize,
         raster_dataframe.RasterYSize,
     )
 
     return bbox
 
 
-def get_bbox_from_vector(vector_dataframe):
+def _get_bbox_from_vector(
+    vector_dataframe: ogr.DataSource,
+) -> List[Union[int, float]]:
     """
     Gets an OGR bounding box from an OGR dataframe.
+    The bounding box is in the same projection as the vector.
 
-    ## Args:
-    `vector_dataframe` (_ogr.DataSource_): An OGR vector dataframe. </br>
-
-    ## Returns:
-    (_list_): An OGR formatted bbox. `[x_min, x_max, y_min, y_max]`
+    Parameters
+    ----------
+    vector_dataframe : ogr.DataSource
+        An OGR vector dataframe.
+
+    Returns
+    -------
+    list
+        An OGR formatted bbox. `[x_min, x_max, y_min, y_max]`
     """
     assert isinstance(
         vector_dataframe, ogr.DataSource
     ), f"vector_dataframe was not a valid ogr.DataSource. Received: {vector_dataframe}"
 
     layer_count = vector_dataframe.GetLayerCount()
 
@@ -249,256 +288,331 @@
                 y_min = layer_y_min
             if layer_y_max > y_max:
                 y_max = layer_y_max
 
     return [x_min, x_max, y_min, y_max]
 
 
-def get_bbox_from_vector_layer(vector_layer):
+def _get_bbox_from_vector_layer(
+    vector_layer: ogr.Layer,
+) -> List[Union[int, float]]:
     """
     Gets an OGR bounding box from an OGR dataframe layer.
 
-    ## Args:
-    `vector_layer` (_ogr.Layer_): An OGR vector dataframe layer. </br>
-
-    ## Returns:
-    (_list_): An OGR formatted bbox. `[x_min, x_max, y_min, y_max]`
+    Parameters
+    ----------
+    vector_layer : ogr.Layer
+        An OGR vector dataframe layer.
+
+    Returns
+    -------
+    list
+        An OGR formatted bbox. `[x_min, x_max, y_min, y_max]`
     """
     assert isinstance(
         vector_layer, ogr.Layer
     ), f"vector_layer was not a valid ogr.Layer. Received: {vector_layer}"
 
     x_min, x_max, y_min, y_max = vector_layer.GetExtent()
 
     return [x_min, x_max, y_min, y_max]
 
 
-def get_bbox_from_dataset(dataset):
+def get_bbox_from_dataset(
+    dataset: Union[str, gdal.Dataset, ogr.DataSource],
+) -> List[Union[int, float]]:
     """
     Get the bbox from a dataset.
+    The bounding box is in the same projection as the dataset.
+    If you want the Bounding Box in WGS84, use `get_bbox_from_dataset_wgs84`.
 
-    ## Args:
-    `dataset` (_str_/_gdal.Dataset_/_ogr.DataSource): A dataset or dataset path. </br>
-
-    ## Returns:
-    (_list_): The bounding box in ogr format: [x_min, x_max, y_min, y_max].
+    Parameters
+    ----------
+    dataset : str, gdal.Dataset, ogr.DataSource
+        A dataset or dataset path.
+
+    Returns
+    -------
+    list
+        The bounding box in ogr format: `[x_min, x_max, y_min, y_max]`.
     """
     assert isinstance(dataset, (str, gdal.Dataset, ogr.DataSource)), "DataSet must be a string, ogr.DataSource, or gdal.Dataset."
 
     opened = dataset if isinstance(dataset, (gdal.Dataset, ogr.DataSource)) else None
 
     if opened is None:
         gdal.PushErrorHandler("CPLQuietErrorHandler")
         opened = gdal.Open(dataset, gdal.GA_ReadOnly)
 
         if opened is None:
             opened = ogr.Open(dataset, gdal.GA_ReadOnly)
 
         gdal.PopErrorHandler()
         if opened is None:
-            raise Exception(f"Could not open dataset. {dataset}")
+            raise RuntimeError(f"Could not open dataset. {dataset}")
 
     if isinstance(opened, gdal.Dataset):
-        return get_bbox_from_raster(opened)
+        return _get_bbox_from_raster(opened)
 
     if isinstance(opened, ogr.DataSource):
-        return get_bbox_from_vector(opened)
+        return _get_bbox_from_vector(opened)
 
-    raise Exception(f"Could not get bbox from dataset. {dataset}")
+    raise RuntimeError(f"Could not get bbox from dataset. {dataset}")
 
 
-def get_sub_geotransform(geotransform, bbox_ogr):
+def _get_sub_geotransform(
+    geotransform: List[Union[int, float]],
+    bbox_ogr: List[Union[int, float]],
+) -> Dict:
     """
     Create a GeoTransform and the raster sizes for an OGR formatted bbox.
 
-    ## Args:
-    `geotransform` (_list_): A GDAL geotransform. </br>
-    `bbox_ogr` (_list_): An OGR formatted bbox. </br>
-
-    ## Returns:
-    (_dict_): { "Transform": _list_, "RasterXSize": _int_, "RasterYSize": _int_ }
+    Parameters
+    ----------
+    geotransform : list
+        A GDAL geotransform.
+        `[top_left_x, pixel_width, rotation_x, top_left_y, rotation_y, pixel_height]`
+    
+    bbox_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+
+    Returns
+    -------
+    dict
+        { "Transform": _list_, "RasterXSize": _int_, "RasterYSize": _int_ }
     """
-    assert is_valid_geotransform(
+    assert _check_is_valid_geotransform(
         geotransform
     ), f"geotransform must be a valid geotransform. Received: {geotransform}."
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox_ogr
     ), f"bbox_ogr was not a valid bbox. Received: {bbox_ogr}"
 
     x_min, x_max, y_min, y_max = bbox_ogr
     pixel_width = geotransform[1]
     pixel_height = geotransform[5]
 
     raster_x_size = round((x_max - x_min) / pixel_width)
     raster_y_size = round((y_max - y_min) / pixel_height)
 
     return {
-        "Transform": [x_min, pixel_width, 0, y_max, 0, ensure_negative(pixel_height)],
+        "Transform": [x_min, pixel_width, 0, y_max, 0, utils_base._ensure_negative(pixel_height)],
         "RasterXSize": abs(raster_x_size),
         "RasterYSize": abs(raster_y_size),
     }
 
 
-def convert_bbox_to_geom(bbox_ogr):
+def _get_geom_from_bbox(
+    bbox_ogr: List[Union[int, float]],
+) -> ogr.Geometry:
     """
-    Convert an OGR bounding box to ogr.Geometry.</br>
+    Convert an OGR bounding box to ogr.Geometry.
     `[x_min, x_max, y_min, y_max] -> ogr.Geometry`
 
-    ## Args:
-    `bbox_ogr` (_list_): An OGR formatted bbox. </br>
-
-    ## Returns:
-    (_ogr.Geometry_): An OGR geometry.
+    Parameters
+    ----------
+    bbox_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+
+    Returns
+    -------
+    ogr.Geometry
+        An OGR geometry.
     """
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox_ogr
     ), f"bbox_ogr was not a valid bbox. Received: {bbox_ogr}"
 
     x_min, x_max, y_min, y_max = bbox_ogr
 
     ring = ogr.Geometry(ogr.wkbLinearRing)
+
     ring.AddPoint(x_min, y_min)
     ring.AddPoint(x_max, y_min)
     ring.AddPoint(x_max, y_max)
     ring.AddPoint(x_min, y_max)
     ring.AddPoint(x_min, y_min)
 
     geom = ogr.Geometry(ogr.wkbPolygon)
     geom.AddGeometry(ring)
 
     return geom
 
 
-def convert_geom_to_bbox(geom):
+def _get_bbox_from_geom(geom: ogr.Geometry) -> List[Union[int, float]]:
     """
-    Convert an ogr.Geometry to an OGR bounding box.</br>
+    Convert an ogr.Geometry to an OGR bounding box.
     `ogr.Geometry -> [x_min, x_max, y_min, y_max]`
 
-    ## Args:
-    `geom` (_ogr.Geometry_): An OGR geometry. </br>
-
-    ## Returns:
-    (_list_): An OGR formatted bbox. `[x_min, x_max, y_min, y_max]`
+    Parameters
+    ----------
+    geom : ogr.Geometry
+        An OGR geometry.
+
+    Returns
+    -------
+    list
+        An OGR formatted bbox. `[x_min, x_max, y_min, y_max]`
     """
     assert isinstance(
         geom, ogr.Geometry
     ), f"geom was not a valid ogr.Geometry. Received: {geom}"
 
     bbox_ogr = list(geom.GetEnvelope()) # [x_min, x_max, y_min, y_max]
 
     return bbox_ogr
 
 
-def convert_bbox_to_geotransform(bbox_ogr, raster_x_size, raster_y_size):
+def _get_geotransform_from_bbox(
+    bbox_ogr: List[Union[int, float]],
+    raster_x_size: int,
+    raster_y_size: int,
+) -> List[Union[int, float]]:
     """
-    Convert an OGR formatted bounding box to a GDAL GeoTransform.</br>
+    Convert an OGR formatted bounding box to a GDAL GeoTransform.
     `[x_min, x_max, y_min, y_max] -> [x_min, pixel_width, x_skew, y_max, y_skew, pixel_height]`
 
-    ## Args:
-    `bbox_ogr` (_list_): An OGR formatted bbox. </br>
-    `raster_x_size` (_int_): The number of pixels in the x direction. </br>
-    `raster_y_size` (_int_): The number of pixels in the y direction. </br>
-
-    ## Returns:
-    (_list_): A GDAL GeoTransform. `[x_min, pixel_width, x_skew, y_max, y_skew, pixel_height]`
+    Parameters
+    ----------
+    bbox_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+    
+    raster_x_size : int
+        The number of pixels in the x direction.
+
+    raster_y_size : int
+        The number of pixels in the y direction.
+
+    Returns
+    -------
+    list
+        A GDAL GeoTransform. `[x_min, pixel_width, x_skew, y_max, y_skew, pixel_height]`
     """
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox_ogr
     ), f"bbox_ogr was not a valid bbox. Received: {bbox_ogr}"
 
     x_min, x_max, y_min, y_max = bbox_ogr
 
     origin_x = x_min
     origin_y = y_max
     pixel_width = (x_max - x_min) / raster_x_size
     pixel_height = (y_max - y_min) / raster_y_size
 
-    return [origin_x, pixel_width, 0, origin_y, 0, ensure_negative(pixel_height)]
+    return [origin_x, pixel_width, 0, origin_y, 0, utils_base._ensure_negative(pixel_height)]
 
 
-def convert_ogr_bbox_to_gdal_bbox(bbox_ogr):
+def _get_gdal_bbox_from_ogr_bbox(
+    bbox_ogr: List[Union[int, float]],
+) -> List[Union[int, float]]:
     """
-    Converts an OGR formatted bbox to a GDAL formatted one.</br>
+    Converts an OGR formatted bbox to a GDAL formatted one.
     `[x_min, x_max, y_min, y_max] -> [x_min, y_min, x_max, y_max]`
 
-    ## Args:
-    `bbox_ogr` (_list_): An OGR formatted bbox. </br>
-
-    ## Returns:
-    (_list_): A GDAL formatted bbox. `[x_min, y_min, x_max, y_max]`
+    Parameters
+    ----------
+    bbox_ogr : list
+        An OGR formatted bbox.
+
+    Returns
+    -------
+    list
+        A GDAL formatted bbox. `[x_min, y_min, x_max, y_max]`
     """
     if isinstance(bbox_ogr, tuple):
         bbox_ogr = [val for val in bbox_ogr]
 
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox_ogr
     ), f"bbox_ogr was not a valid bbox. Received: {bbox_ogr}"
 
     x_min, x_max, y_min, y_max = bbox_ogr
 
     return [x_min, y_min, x_max, y_max]
 
 
-def convert_gdal_bbox_to_ogr_bbox(bbox_gdal):
+def _get_ogr_bbox_from_gdal_bbox(
+    bbox_gdal: List[Union[int, float]],
+) -> List[Union[int, float]]:
     """
-    Converts a GDAL formatted bbox to an OGR formatted one.</br>
+    Converts a GDAL formatted bbox to an OGR formatted one.
     `[x_min, y_min, x_max, y_max] -> [x_min, x_max, y_min, y_max]`
 
-    ## Args:
-    `bbox_gdal` (_list_): A GDAL formatted bbox. </br>
-
-    ## Returns:
-    (_list_): An OGR formatted bbox. `[x_min, x_max, y_min, y_max]`
+    Parameters
+    ----------
+    bbox_gdal : list
+        A GDAL formatted bbox.
+
+    Returns
+    -------
+    list
+        An OGR formatted bbox. `[x_min, x_max, y_min, y_max]`
     """
     if isinstance(bbox_ogr, tuple):
         bbox_ogr = [val for val in bbox_ogr]
 
     assert (
         isinstance(bbox_gdal, list) and len(bbox_gdal) == 4
     ), f"bbox_gdal must be a list of length four. Received: {bbox_gdal}."
 
     x_min, y_min, x_max, y_max = bbox_gdal
 
     return [x_min, x_max, y_min, y_max]
 
 
-def convert_bbox_to_wkt(bbox_ogr):
+def _get_wkt_from_bbox(
+    bbox_ogr: List[Union[int, float]],
+) -> str:
     """
-    Converts an OGR formatted bbox to a WKT string.</br>
+    Converts an OGR formatted bbox to a WKT string.
     `[x_min, x_max, y_min, y_max] -> WKT`
 
-    ## Args:
-    `bbox_ogr` (_list_): An OGR formatted bbox. </br>
-
-    ## Returns:
-    (_str_): A WKT Polygon string. `POLYGON ((...))`
+    Parameters
+    ----------
+    bbox_ogr : list
+        An OGR formatted bbox.
+
+    Returns
+    -------
+    str
+        A WKT string. `POLYGON ((...))`
     """
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox_ogr
     ), f"bbox_ogr was not a valid bbox. Received: {bbox_ogr}"
 
     x_min, x_max, y_min, y_max = bbox_ogr
 
     wkt = f"POLYGON (({x_min} {y_min}, {x_max} {y_min}, {x_max} {y_max}, {x_min} {y_max}, {x_min} {y_min}))"
 
     return wkt
 
 
-def convert_bbox_to_geojson(bbox_ogr):
+def _get_geojson_from_bbox(
+    bbox_ogr: List[Union[int, float]],
+) -> Dict[str, Union[str, List]]:
     """
-    Converts an OGR formatted bbox to a GeoJson dictionary.</br>
+    Converts an OGR formatted bbox to a GeoJson dictionary.
     `[x_min, x_max, y_min, y_max] -> GeoJson`
 
-    ## Args:
-    `bbox_ogr` (_list_): an OGR formatted bbox. </br>
-
-    ## Returns:
-    (_dict_): A GeoJson Dictionary. `{ "type": "Polygon", "coordinates": [ ... ] }`
+    Parameters
+    ----------
+    bbox_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+    
+    Returns
+    -------
+    dict
+        A GeoJson dictionary. `{ "type": "Polygon", "coordinates": [ ... ] }`
     """
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox_ogr
     ), f"bbox_ogr was not a valid bbox. Received: {bbox_ogr}"
 
     x_min, x_max, y_min, y_max = bbox_ogr
 
     geojson = {
         "type": "Polygon",
@@ -512,38 +626,48 @@
             ]
         ],
     }
 
     return geojson
 
 
-def convert_bbox_to_vector(bbox_ogr, projection_osr):
+def _get_vector_from_bbox(
+    bbox_ogr: List[Union[int, float]],
+    projection_osr: osr.SpatialReference,
+) -> ogr.DataSource:
     """
-    Converts an OGR formatted bbox to an in-memory vector.</br>
-    _Vectors are stored in /vsimem/ as .gpkg files._</br>
+    Converts an OGR formatted bbox to an in-memory vector.
+    _Vectors are stored in /vsimem/ as .gpkg files.
     **OBS**: Layers should be manually cleared when no longer used.
 
-    ## Args:
-    `bbox_ogr` (_list_): an OGR formatted bbox. </br>
-    `projection_osr` (_osr.SpatialReference_): The projection of the vector. </br>
-
-    ## Returns:
-    (_ogr.DataSource_): The bounding box as a vector.
+    Parameters
+    ----------
+    bbox_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+    
+    projection_osr : osr.SpatialReference
+        The projection of the vector.
+
+    Returns
+    -------
+    ogr.DataSource
+        The bounding box as a vector.
     """
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox_ogr
     ), f"bbox_ogr was not a valid bbox. Received: {bbox_ogr}"
     assert isinstance(
         projection_osr, osr.SpatialReference
     ), f"projection_osr not a valid spatial reference. Recieved: {projection_osr}"
 
-    geom = convert_bbox_to_geom(bbox_ogr)
+    geom = _get_geom_from_bbox(bbox_ogr)
 
     driver = ogr.GetDriverByName("GPKG")
-    extent_name = f"/vsimem/{core_utils.get_unix_seconds_as_str()}_{uuid4().int}_extent.gpkg"
+    extent_name = f"/vsimem/{str(uuid4().int)}_extent.gpkg"
 
     extent_ds = driver.CreateDataSource(extent_name)
 
     layer = extent_ds.CreateLayer("extent_ogr", projection_osr, ogr.wkbPolygon)
 
     feature = ogr.Feature(layer.GetLayerDefn())
     feature.SetGeometry(geom)
@@ -551,29 +675,40 @@
 
     feature = None
     layer.SyncToDisk()
 
     return extent_name
 
 
-def bboxes_intersect(bbox1_ogr, bbox2_ogr):
+def _check_bboxes_intersect(
+    bbox1_ogr: List[Union[int, float]],
+    bbox2_ogr: List[Union[int, float]],
+) -> bool:
     """
     Checks if two OGR formatted bboxes intersect.
 
-    ## Args:
-    `bbox1_ogr` (_list_): An OGR formatted bbox. </br>
-    `bbox2_ogr` (_list_): An OGR formatted bbox. </br>
-
-    ## Returns:
-    (_bool_): **True** if the bboxes intersect, **False** otherwise.
+    Parameters
+    ----------
+    bbox1_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+
+    bbox2_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+
+    Returns
+    -------
+    bool
+        **True** if the bboxes intersect, **False** otherwise.
     """
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox1_ogr
     ), f"bbox1_ogr was not a valid bbox. Received: {bbox1_ogr}"
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox2_ogr
     ), f"bbox1_ogr was not a valid bbox. Received: {bbox2_ogr}"
 
     bbox1_x_min, bbox1_x_max, bbox1_y_min, bbox1_y_max = bbox1_ogr
     bbox2_x_min, bbox2_x_max, bbox2_y_min, bbox2_y_max = bbox2_ogr
 
     if bbox2_x_min > bbox1_x_max:
@@ -587,200 +722,160 @@
 
     if bbox2_y_max < bbox1_y_min:
         return False
 
     return True
 
 
-def bboxes_within(bbox1_ogr, bbox2_ogr):
+def _check_bboxes_within(
+    bbox1_ogr: List[Union[int, float]],
+    bbox2_ogr: List[Union[int, float]],
+) -> bool:
     """
     Checks if one OGR formatted bbox is within another.
 
-    ## Args:
-    `bbox1_ogr` (_list_): An OGR formatted bbox. </br>
-    `bbox2_ogr` (_list_): An OGR formatted bbox. </br>
-
-    ## Returns:
-    (_bool_): **True** if the bbox is within the other, **False** otherwise.
+    Parameters
+    ----------
+    bbox1_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+
+    bbox2_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+
+    Returns
+    -------
+    bool
+        **True** if the bbox is within the other, **False** otherwise.
     """
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox1_ogr
     ), f"bbox1_ogr was not a valid bbox. Received: {bbox1_ogr}"
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox2_ogr
     ), f"bbox1_ogr was not a valid bbox. Received: {bbox2_ogr}"
 
     bbox1_x_min, bbox1_x_max, bbox1_y_min, bbox1_y_max = bbox1_ogr
     bbox2_x_min, bbox2_x_max, bbox2_y_min, bbox2_y_max = bbox2_ogr
 
     return (
         (bbox1_x_min >= bbox2_x_min)
         and (bbox1_x_max <= bbox2_x_max)
         and (bbox1_y_min >= bbox2_y_min)
         and (bbox1_y_max <= bbox2_y_max)
     )
 
 
-def get_intersection_bboxes(bbox1_ogr, bbox2_ogr):
+def _get_intersection_bboxes(
+    bbox1_ogr: List[Union[int, float]],
+    bbox2_ogr: List[Union[int, float]],
+) -> List[Union[int, float]]:
     """
     Get the intersection of two OGR formatted bboxes.
 
-    ## Args:
-    `bbox1_ogr` (_list_): An OGR formatted bbox. </br>
-    `bbox2_ogr` (_list_): An OGR formatted bbox. </br>
-
-    ## Returns:
-    (_list_): An OGR formatted bbox of the intersection. `[x_min, x_max, y_min, y_max]`
+    Parameters
+    ----------
+    bbox1_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+    
+    bbox2_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+    
+    Returns
+    -------
+    list
+        An OGR formatted bbox of the intersection.
     """
-    assert bboxes_intersect(
+    assert _check_bboxes_intersect(
         bbox1_ogr, bbox2_ogr
     ), "The two bounding boxes do not intersect."
 
     bbox1_x_min, bbox1_x_max, bbox1_y_min, bbox1_y_max = bbox1_ogr
     bbox2_x_min, bbox2_x_max, bbox2_y_min, bbox2_y_max = bbox2_ogr
 
     return [
         max(bbox1_x_min, bbox2_x_min),
         min(bbox1_x_max, bbox2_x_max),
         max(bbox1_y_min, bbox2_y_min),
         min(bbox1_y_max, bbox2_y_max),
     ]
 
 
-def get_union_bboxes(bbox1_ogr, bbox2_ogr):
+def _get_union_bboxes(
+    bbox1_ogr: List[Union[int, float]],
+    bbox2_ogr: List[Union[int, float]],
+) -> List[Union[int, float]]:
     """
     Get the union of two OGR formatted bboxes.
 
-    ## Args:
-    `bbox1_ogr` (_list_): An OGR formatted bbox. </br>
-    `bbox2_ogr` (_list_): An OGR formatted bbox. </br>
-
-    ## Returns:
-    (_list_): An OGR formatted bbox of the union. `[x_min, x_max, y_min, y_max]`
+    Parameters
+    ----------
+    bbox1_ogr : list
+        An OGR formatted bbox.
+
+    bbox2_ogr : list
+        An OGR formatted bbox.
+
+    Returns
+    -------
+    list
+        An OGR formatted bbox of the union.
     """
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox1_ogr
     ), f"bbox1_ogr was not a valid bbox. Received: {bbox1_ogr}"
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox2_ogr
     ), f"bbox1_ogr was not a valid bbox. Received: {bbox2_ogr}"
 
     bbox1_x_min, bbox1_x_max, bbox1_y_min, bbox1_y_max = bbox1_ogr
     bbox2_x_min, bbox2_x_max, bbox2_y_min, bbox2_y_max = bbox2_ogr
 
     return [
         min(bbox1_x_min, bbox2_x_min),
         max(bbox1_x_max, bbox2_x_max),
         min(bbox1_y_min, bbox2_y_min),
         max(bbox1_y_max, bbox2_y_max),
     ]
 
 
-def get_projection_from_raster(raster):
-    """
-    Get the projection from a raster.
-
-    ## Args:
-    `raster` (_str_/_gdal.Dataset_): A raster or raster path. </br>
-
-    ## Returns:
-    (_osr.SpatialReference_): The projection in OSR format.
-    """
-    opened = None
-    if isinstance(raster, gdal.Dataset):
-        opened = raster
-    else:
-        gdal.PushErrorHandler("CPLQuietErrorHandler")
-        opened = gdal.Open(raster, gdal.GA_ReadOnly)
-        gdal.PopErrorHandler()
-
-    if opened is None:
-        raise Exception(f"Could not open raster. {raster}")
-
-    projection = osr.SpatialReference()
-    projection.ImportFromWkt(opened.GetProjection())
-    opened = None
-
-    return projection
-
-
-def get_projection_from_vector(vector):
-    """
-    Get the projection from a vector.
-
-    ## Args:
-    `vector` (_str_/_gdal.Dataset_): A vector or vector path. </br>
-
-    ## Returns:
-    (_osr.SpatialReference_): The projection in OSR format.
-    """
-    opened = None
-    if isinstance(vector, ogr.DataSource):
-        opened = vector
-    else:
-        gdal.PushErrorHandler("CPLQuietErrorHandler")
-        opened = ogr.Open(vector, gdal.GA_ReadOnly)
-        gdal.PopErrorHandler()
-
-    if opened is None:
-        raise Exception(f"Could not open vector. {vector}")
-
-    layer = opened.GetLayer()
-    projection = layer.GetSpatialRef()
-    opened = None
-
-    return projection
-
-
-def get_projection_from_dataset(dataset):
-    """
-    Get the projection from a dataset.
-
-    ## Args:
-    `dataset` (_str_/_gdal.Dataset_/_ogr.DataSource): A dataset or dataset path. </br>
-
-    ## Returns:
-    (_osr.SpatialReference_): The projection in OSR format.
-    """
-    assert isinstance(dataset, (str, gdal.Dataset, ogr.DataSource)), "DataSet must be a string, ogr.DataSource, or gdal.Dataset."
-
-    opened = dataset if isinstance(dataset, (gdal.Dataset, ogr.DataSource)) else None
-
-    if opened is None:
-        gdal.PushErrorHandler("CPLQuietErrorHandler")
-        opened = gdal.Open(dataset, gdal.GA_ReadOnly)
-
-        if opened is None:
-            opened = ogr.Open(dataset, gdal.GA_ReadOnly)
-
-        gdal.PopErrorHandler()
-        if opened is None:
-            raise Exception(f"Could not open dataset. {dataset}")
-
-    if isinstance(opened, gdal.Dataset):
-        return get_projection_from_raster(opened)
-
-    if isinstance(opened, ogr.DataSource):
-        return get_projection_from_vector(opened)
-
-    raise Exception(f"Could not get projection from dataset. {dataset}")
-
-
-def align_bboxes_to_pixel_size(bbox1_ogr, bbox2_ogr, pixel_width, pixel_height):
-    """
-    Aligns two OGR formatted bboxes to a pixel size.
-
-    ## Args:
-    `bbox1_ogr` (_list_): An OGR formatted bbox. </br>
-    `bbox2_ogr` (_list_): An OGR formatted bbox. </br>
-    `pixel_width` (_float_/_int_): The width of the pixel. </br>
-    `pixel_height` (_float_/_int_): The height of the pixel. </br>
-
-    ## Returns:
-    (_list_): An OGR formatted bbox of the alignment. `[x_min, x_max, y_min, y_max]`
+def _get_aligned_bbox_to_pixel_size(
+    bbox1_ogr: List[Union[int, float]],
+    bbox2_ogr: List[Union[int, float]],
+    pixel_width: Union[int, float],
+    pixel_height: Union[int, float],
+) -> List[Union[int, float]]:
+    """
+    Aligns two OGR formatted bboxes to a pixel size. Output is an augmented version
+    of bbox2.
+
+    Parameters
+    ----------
+    bbox1_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+    
+    bbox2_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+
+    pixel_width : int or float
+        The width of the pixel.
+    
+    pixel_height : int or float
+        The height of the pixel.
+
+    Returns
+    -------
+    list
+        An OGR formatted bbox of the alignment.
+        `[x_min, x_max, y_min, y_max]`
     """
     assert (
         isinstance(bbox1_ogr, list) and len(bbox1_ogr) == 4
     ), f"bbox1_ogr must be a list of length four. Received: {bbox1_ogr}."
     assert (
         isinstance(bbox2_ogr, list) and len(bbox2_ogr) == 4
     ), f"bbox2_ogr must be a list of length four. Received: {bbox2_ogr}."
@@ -793,262 +888,304 @@
 
     y_min = bbox2_y_min - ((bbox2_y_min - bbox1_y_min) % abs(pixel_height))
     y_max = bbox2_y_max + ((bbox1_y_max - bbox2_y_max) % abs(pixel_height))
 
     return x_min, x_max, y_min, y_max
 
 
-def reproject_bbox(
-    bbox_ogr,
-    source_projection,
-    target_projection,
-):
-    """
-    Reprojects an OGR formatted bbox.
-
-    ## Args:
-    `bbox_ogr` (_list_): An OGR formatted bbox. </br>
-    `source_projection_osr` (_osr.SpatialReference_): The source projection. </br>
-    `target_projection_osr` (_osr.SpatialReference_): The target projection. </br>
-
-    ## Returns:
-    (_list_): An OGR formatted reprojected bbox. `[x_min, x_max, y_min, y_max]`
+def _get_bounds_from_bbox(
+    bbox_ogr: List[Union[int, float]],
+    projection_osr: osr.SpatialReference,
+    wkt: bool = True,
+) -> ogr.Geometry:
+    """ 
+    This is an internal utility function for metadata generation. It takes a standard
+    OGR bounding box and the geometry of the source dataset in latlng and returns a
+    geometry in the source dataset's projection. This is important as, as when 
+    reprojecting to latlng, you might get a skewed bounding box. This function returns
+    the skewed bounds in latlng, which is what you want for overlap checks across
+    projections.
+
+    The return is in WGS84.
+
+    Parameters
+    ----------
+    bbox_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+
+    projection_osr : osr.SpatialReference
+        The projection of the bbox
+
+    wkt : bool, optional
+        Whether to return the geometry as a WKT string or an OGR geometry object.
+
+    Returns
+    -------
+    ogr.Geometry
+        The geometry in the source dataset's projection.
     """
-    assert is_valid_bbox(bbox_ogr), f"Invalid bbox. Received: {bbox_ogr}."
-
-    src_proj = gdal_utils.parse_projection(source_projection)
-    dst_proj = gdal_utils.parse_projection(target_projection)
-
-    if gdal_utils.projections_match(src_proj, dst_proj):
-        return bbox_ogr
-
-    transformer = osr.CoordinateTransformation(src_proj, dst_proj)
+    default_projection = utils_projection._get_default_projection_osr()
+    transformer = osr.CoordinateTransformation(projection_osr, default_projection)
 
     x_min, x_max, y_min, y_max = bbox_ogr
 
-    try:
-        transformed_x_min, transformed_y_min, _z = transformer.TransformPoint(x_min, y_min)
-        transformed_x_max, transformed_y_max, _z = transformer.TransformPoint(x_max, y_max)
-    except: # pylint: disable=bare-except
-        transformed_x_min, transformed_y_min, _z = transformer.TransformPoint(float(x_min), float(y_min))
-        transformed_x_max, transformed_y_max, _z = transformer.TransformPoint(float(x_max), float(y_max))
-
-    return [
-        transformed_x_min,
-        transformed_x_max,
-        transformed_y_min,
-        transformed_y_max,
-    ]
-
-
-def get_utm_zone_from_latlng(latlng, return_epsg=False):
-    """ Get the UTM ZONE from a latlng list.
-
-    ## Args:
-    `bbox_ogr` (_list_): An OGR formatted bbox. </br>
-
-    ## Returns:
-    (_osr.SpatialReference_): The UTM zone projection.
-    """
-    assert isinstance(latlng, (list, np.ndarray)), "latlng must be in the form of a list."
-
-    zone = round(((latlng[1] + 180) / 6) + 1)
-    n_or_s = "S" if latlng[0] < 0 else "N"
-
-    false_northing = "10000000" if n_or_s == "S" else "0"
-    central_meridian = str(round(((zone * 6) - 180) - 3))
-    epsg = f"32{'7' if n_or_s == 'S' else '6'}{str(zone)}"
-
-    if return_epsg:
-        return epsg
-
-    wkt = f"""
-        PROJCS["WGS 84 / UTM zone {str(zone)}{n_or_s}",
-        GEOGCS["WGS 84",
-            DATUM["WGS_1984",
-                SPHEROID["WGS 84",6378137,298.257223563,
-                    AUTHORITY["EPSG","7030"]],
-                AUTHORITY["EPSG","6326"]],
-            PRIMEM["Greenwich",0,
-                AUTHORITY["EPSG","8901"]],
-            UNIT["degree",0.0174532925199433,
-                AUTHORITY["EPSG","9122"]],
-            AUTHORITY["EPSG","4326"]],
-        PROJECTION["Transverse_Mercator"],
-        PARAMETER["latitude_of_origin",0],
-        PARAMETER["central_meridian",{central_meridian}],
-        PARAMETER["scale_factor",0.9996],
-        PARAMETER["false_easting",500000],
-        PARAMETER["false_northing",{false_northing}],
-        UNIT["metre",1,
-            AUTHORITY["EPSG","9001"]],
-        AXIS["Easting",EAST],
-        AXIS["Northing",NORTH],
-        AUTHORITY["EPSG","{epsg}"]]
-    """
-    projection = osr.SpatialReference()
-    projection.ImportFromWkt(wkt)
-
-    return projection
+    p1 = [x_min, y_min]
+    p2 = [x_max, y_min]
+    p3 = [x_max, y_max]
+    p4 = [x_min, y_max]
 
+    gdal.PushErrorHandler("CPLQuietErrorHandler")
+    try:
+        p1t = transformer.TransformPoint(p1[0], p1[1])
+        p2t = transformer.TransformPoint(p2[0], p2[1])
+        p3t = transformer.TransformPoint(p3[0], p3[1])
+        p4t = transformer.TransformPoint(p4[0], p4[1])
+    except RuntimeError:
+        p1t = transformer.TransformPoint(float(p1[0]), float(p1[1]))
+        p2t = transformer.TransformPoint(float(p2[0]), float(p2[1]))
+        p3t = transformer.TransformPoint(float(p3[0]), float(p3[1]))
+        p4t = transformer.TransformPoint(float(p4[0]), float(p4[1]))
+    gdal.PopErrorHandler()
 
-def get_utm_zone_from_bbox(bbox_ogr_latlng):
+    ring = ogr.Geometry(ogr.wkbLinearRing)
+    ring.AddPoint(p1t[0], p1t[1])
+    ring.AddPoint(p2t[0], p2t[1])
+    ring.AddPoint(p3t[0], p3t[1])
+    ring.AddPoint(p4t[0], p4t[1])
+    ring.AddPoint(p1t[0], p1t[1])
+    polygon = ogr.Geometry(ogr.wkbPolygon)
+    polygon.AddGeometry(ring)
+
+    if wkt:
+        return polygon.ExportToWkt()
+
+    return polygon
+
+
+def _get_utm_zone_from_bbox(
+    bbox_ogr_latlng: List[Union[int, float]],
+) -> osr.SpatialReference:
     """
     Get the UTM zone from an OGR formatted bbox.
 
-    ## Args:
-    `bbox_ogr` (_list_): An OGR formatted bbox. </br>
-
-    ## Returns:
-    (_osr.SpatialReference_): The UTM zone projection.
+    Parameters
+    ----------
+    bbox_ogr_latlng : list
+        An OGR formatted bbox.
+
+    Returns
+    -------
+    osr.SpatialReference
+        The UTM zone projection.
     """
-    assert is_valid_bbox(
+    assert _check_is_valid_bbox(
         bbox_ogr_latlng
     ), f"bbox_ogr was not a valid bbox. Received: {bbox_ogr_latlng}"
-    assert is_valid_bbox_latlng(bbox_ogr_latlng), "Bbox is not in latlng format."
+    assert _check_is_valid_bbox_latlng(bbox_ogr_latlng), "Bbox is not in latlng format."
 
     bbox_x_min, bbox_x_max, bbox_y_min, bbox_y_max = bbox_ogr_latlng
 
     mid_lng = (bbox_x_min + bbox_x_max) / 2
     mid_lat = (bbox_y_min + bbox_y_max) / 2
 
-    return get_utm_zone_from_latlng([mid_lat, mid_lng])
+    return utils_projection._get_utm_zone_from_latlng([mid_lat, mid_lng])
 
 
-def get_utm_zone_from_dataset(dataset):
+def _get_utm_zone_from_dataset(
+    dataset: Union[str, gdal.Dataset, ogr.DataSource],
+) -> str:
     """
     Get the UTM zone from a GDAL dataset.
 
-    ## Args:
-    `dataset` (_obj_): A GDAL dataset. </br>
-
-    ## Returns:
-    (_str_): The UTM zone.
+    Parameters
+    ----------
+    dataset : str or gdal.Dataset or ogr.DataSource
+        A GDAL dataset.
+
+    Returns
+    -------
+    str
+        The UTM zone.
     """
     assert isinstance(dataset, (str, gdal.Dataset, ogr.DataSource)), "dataset was not a valid dataset."
 
     bbox = get_bbox_from_dataset(dataset)
-    source_projection = get_projection_from_dataset(dataset)
+    source_projection = utils_projection._get_projection_from_dataset(dataset)
     target_projection = osr.SpatialReference()
-    # target_projection.ImportFromEPSG(4326)
-    target_projection.ImportFromWkt('GEOGCS["WGS 84",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563]],PRIMEM["Greenwich",0],UNIT["degree",0.0174532925199433,AUTHORITY["EPSG","9122"]],AUTHORITY["EPSG","4326"]]')
+    target_projection_wkt = utils_projection._get_default_projection()
+    target_projection.ImportFromWkt(target_projection_wkt)
 
-    bbox = reproject_bbox(bbox, source_projection, target_projection)
-    utm_zone = get_utm_zone_from_bbox(bbox)
+    bbox = utils_projection.reproject_bbox(bbox, source_projection, target_projection)
+    utm_zone = _get_utm_zone_from_bbox(bbox)
 
     return utm_zone
 
 
-def get_utm_zone_from_dataset_list(datasets):
+def _get_utm_zone_from_dataset_list(
+    datasets: List[Union[str, gdal.Dataset, ogr.DataSource]],
+) -> str:
     """
     Get the UTM zone from a list of GDAL datasets.
 
-    ## Args:
-    `datasets` (_list_): A list of GDAL datasets. </br>
-
-    ## Returns:
-    (_str_): The UTM zone.
+    Parameters
+    ----------
+    datasets : list
+        A list of GDAL datasets.
+
+    Returns
+    -------
+    str
+        The UTM zone.
     """
     assert isinstance(datasets, (list, np.ndarray)), "datasets was not a valid list."
 
     latlng_bboxes = []
-    latlng_proj = osr.SpatialReference()
-    # latlng_proj.ImportFromEPSG(4326)
-    latlng_proj.ImportFromWkt('GEOGCS["WGS 84",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563]],PRIMEM["Greenwich",0],UNIT["degree",0.0174532925199433,AUTHORITY["EPSG","9122"]],AUTHORITY["EPSG","4326"]]')
+    latlng_proj = utils_projection._get_default_projection_osr()
 
     for dataset in datasets:
         bbox = get_bbox_from_dataset(dataset)
-        projection = get_projection_from_dataset(dataset)
-        latlng_bboxes.append(reproject_bbox(bbox, projection, latlng_proj))
+        projection = utils_projection._get_projection_from_dataset(dataset)
+        latlng_bboxes.append(utils_projection.reproject_bbox(bbox, projection, latlng_proj))
 
     union_bbox = latlng_bboxes[0]
     for bbox in latlng_bboxes[1:]:
-        union_bbox = get_union_bboxes(union_bbox, bbox)
+        union_bbox = _get_union_bboxes(union_bbox, bbox)
 
-    utm_zone = get_utm_zone_from_bbox(union_bbox)
+    utm_zone = _get_utm_zone_from_bbox(union_bbox)
 
     return utm_zone
 
 
-def reproject_latlng_point_to_utm(latlng):
-    """ Converts a latlng point into an UTM point.
-
-        Takes point in [lat, lng], returns [utm_x, utm_y].
-    """
-    source_projection = osr.SpatialReference()
-    # source_projection.ImportFromEPSG(4326)
-    source_projection.ImportFromWkt('GEOGCS["WGS 84",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563]],PRIMEM["Greenwich",0],UNIT["degree",0.0174532925199433,AUTHORITY["EPSG","9122"]],AUTHORITY["EPSG","4326"]]')
-    target_projection = get_utm_zone_from_latlng(latlng)
-
-    transformer = osr.CoordinateTransformation(
-        source_projection, target_projection
-    )
-
-    try:
-        utm_x, utm_y, _utm_z = transformer.TransformPoint(latlng[0], latlng[1])
-    except: # pylint: disable=bare-except
-        utm_x, utm_y, _utm_z = transformer.TransformPoint(float(latlng[0]), float(latlng[1]))
-
-    return [utm_x, utm_y]
-
-
-def additional_bboxes(bbox_ogr, projection_osr):
+def _additional_bboxes(
+    bbox_ogr: List[Union[int, float]],
+    projection_osr: osr.SpatialReference,
+) -> Dict[str, Any]:
     """
     This is an internal utility function for metadata generation. It takes a standard
     OGR bounding box and returns a list of variations of bounding boxes.
 
-    ## Args:
-    `bbox_ogr` (_list_): An OGR formatted bbox. </br>
-    `projection_osr` (_osr.SpatialReference_): The projection. </br>
-
-    ## Returns:
-    (_dict_): A dictionary of the added bboxes. Contains the following keys: </br>
-    `bbox_latlng`: The bbox in latlng coordinates. </br>
-    `bbox_wkt`: The bbox in WKT format. </br>
-    `bbox_wkt_latlng`: The bbox in WKT format in latlng coordinates. </br>
-    `bbox_geom`: The bbox in ogr.Geometry format. </br>
-    `bbox_geom_latlng`: The bbox in ogr.Geometry format in latlng coordinates. </br>
-    `bbox_gdal`: The bbox in GDAL format. </br>
-    `bbox_gdal_latlng`: The bbox in GDAL format in latlng coordinates. </br>
-    `bbox_dict`: The bbox in a dictionary format. { "x_min": x_min, ... } </br>
-    `bbox_dict_latlng`: The bbox in a dictionary format in latlng coordinates. </br>
+    Parameters
+    ----------
+    bbox_ogr : list
+        An OGR formatted bbox.
+        `[x_min, x_max, y_min, y_max]`
+
+    projection_osr : osr.SpatialReference
+        The projection.
+
+    Returns
+    -------
+    dict
+        A dictionary of the added bboxes. Contains the following keys:
+        `bbox_latlng`: The bbox in latlng coordinates.
+        `bbox_wkt`: The bbox in WKT format.
+        `bbox_wkt_latlng`: The bbox in WKT format in latlng coordinates.
+        `bbox_geom`: The bbox in ogr.Geometry format.
+        `bbox_geom_latlng`: The bbox in ogr.Geometry format in latlng coordinates.
+        `bbox_gdal`: The bbox in GDAL format.
+        `bbox_gdal_latlng`: The bbox in GDAL format in latlng coordinates.
+        `bbox_dict`: The bbox in a dictionary format.
+        `bbox_dict_latlng`: The bbox in a dictionary format in latlng coordinates.
     """
-    assert is_valid_bbox(bbox_ogr), f"Invalid bbox. Received: {bbox_ogr}."
+    assert _check_is_valid_bbox(bbox_ogr), f"Invalid bbox. Received: {bbox_ogr}."
     assert isinstance(
         projection_osr, osr.SpatialReference
     ), f"source_projection not a valid spatial reference. Recieved: {projection_osr}"
 
     x_min, x_max, y_min, y_max = bbox_ogr
 
     original_projection = osr.SpatialReference()
     original_projection.ImportFromWkt(projection_osr.ExportToWkt())
 
-    latlng_projection = osr.SpatialReference()
-    # latlng_projection.ImportFromEPSG(4326)
-    latlng_projection.ImportFromWkt('GEOGCS["WGS 84",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563]],PRIMEM["Greenwich",0],UNIT["degree",0.0174532925199433,AUTHORITY["EPSG","9122"]],AUTHORITY["EPSG","4326"]]')
+    latlng_projection = utils_projection._get_default_projection_osr()
+    bbox_ogr_latlng = utils_projection.reproject_bbox(bbox_ogr, original_projection, latlng_projection)
+
+    world = False
+    if np.isinf(bbox_ogr_latlng).any():
+        world = True
+    if np.isinf(bbox_ogr_latlng[0]):
+        bbox_ogr_latlng[0] = -179.999999
+    if np.isinf(bbox_ogr_latlng[1]):
+        bbox_ogr_latlng[1] = 180.0
+    if np.isinf(bbox_ogr_latlng[2]):
+        bbox_ogr_latlng[2] = -89.999999
+    if np.isinf(bbox_ogr_latlng[3]):
+        bbox_ogr_latlng[3] = 90.0
 
-    bbox_ogr_latlng = reproject_bbox(bbox_ogr, original_projection, latlng_projection)
     latlng_x_min, latlng_x_max, latlng_y_min, latlng_y_max = bbox_ogr_latlng
 
-    bbox_geom = convert_bbox_to_geom(bbox_ogr)
-    bbox_geom_latlng = convert_bbox_to_geom(bbox_ogr_latlng)
+    bbox_geom = _get_geom_from_bbox(bbox_ogr)
+    bbox_geom_latlng = _get_geom_from_bbox(bbox_ogr_latlng)
+    geom = bbox_geom
+
+    if world:
+        geom_latlng = bbox_geom_latlng
+    else:
+        geom_latlng = _get_bounds_from_bbox(bbox_ogr, original_projection, latlng_projection)
 
-    bbox_wkt = convert_bbox_to_wkt(bbox_ogr)
-    bbox_wkt_latlng = convert_bbox_to_wkt(bbox_ogr_latlng)
+    geom_latlng_geom = ogr.CreateGeometryFromWkt(geom_latlng)
+
+    bbox_wkt = _get_wkt_from_bbox(bbox_ogr)
+    bbox_wkt_latlng = _get_wkt_from_bbox(bbox_ogr_latlng)
 
     return {
         "bbox_latlng": bbox_ogr_latlng,
         "bbox_wkt": bbox_wkt,
         "bbox_wkt_latlng": bbox_wkt_latlng,
         "bbox_geom": bbox_geom,
         "bbox_geom_latlng": bbox_geom_latlng,
-        "bbox_gdal": convert_ogr_bbox_to_gdal_bbox(bbox_ogr),
-        "bbox_gdal_latlng": convert_ogr_bbox_to_gdal_bbox(bbox_ogr_latlng),
+        "bbox_gdal": _get_gdal_bbox_from_ogr_bbox(bbox_ogr),
+        "bbox_gdal_latlng": _get_gdal_bbox_from_ogr_bbox(bbox_ogr_latlng),
         "bbox_dict": {"x_min": x_min, "x_max": x_max, "y_min": y_min, "y_max": y_max},
         "bbox_dict_latlng": {
             "x_min": latlng_x_min,
             "x_max": latlng_x_max,
             "y_min": latlng_y_min,
             "y_max": latlng_y_max,
         },
-        "bbox_geojson": convert_bbox_to_geojson(bbox_ogr_latlng),
+        "bbox_geojson": _get_geojson_from_bbox(bbox_ogr_latlng),
+        "area_latlng": geom_latlng_geom.GetArea(),
+        "area": geom.GetArea(),
+        "geom": geom,
+        "geom_latlng": geom_latlng,
     }
+
+
+def _get_vector_from_geom(
+    geom: ogr.Geometry,
+    projection_osr: Optional[osr.SpatialReference] = None,
+) -> ogr.DataSource:
+    """
+    Converts a geometry to a vector.
+
+    Parameters
+    ----------
+    geom : ogr.Geometry
+        The geometry to convert.
+
+    Returns
+    -------
+    ogr.DataSource
+    """
+    assert isinstance(geom, ogr.Geometry), "geom must be an ogr.Geometry."
+
+    path = utils_path._get_augmented_path(
+        "converted_geom.gpkg",
+        add_uuid=True,
+        folder="/vsimem/",
+    )
+
+    driver_name = utils_gdal._get_vector_driver_name_from_path(path)
+    driver = ogr.GetDriverByName(driver_name)
+    vector = driver.CreateDataSource(path)
+
+    proj = projection_osr if projection_osr is not None else utils_projection._get_default_projection_osr()
+    layer = vector.CreateLayer("converted_geom", proj, geom.GetGeometryType())
+
+    feature = ogr.Feature(layer.GetLayerDefn())
+    feature.SetGeometry(geom)
+
+    layer.CreateFeature(feature)
+    feature.Destroy()
+
+    return vector
```

### Comparing `buteo-0.8.9/buteo/utils/core_utils.py` & `buteo-0.9.0/buteo/utils/utils_gdal.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,991 +1,1049 @@
 """
-### Generic utility functions ###
+### Utility functions to work with GDAL ###
 
-Functions that make interacting with the toolbox easier.
+These functions are used to interact with basic GDAL objects.
 """
 
 # Standard Library
+import sys; sys.path.append("../../")
+from typing import Optional, Union, List, Any
+from warnings import warn
 import os
-import sys
-import time
-import shutil
-from glob import glob
-from uuid import uuid4
-from datetime import datetime
-from pathlib import PurePosixPath
 
 # External
+from osgeo import gdal, ogr
 import psutil
-from osgeo import gdal
+import numpy as np
 
-from buteo.utils.gdal_enums import get_valid_raster_driver_extensions, get_valid_vector_driver_extensions
+# Internal
+from buteo.utils import utils_path, utils_translate
 
 
 
-def get_unix_seconds_as_str():
+def _get_default_creation_options(
+    options: Optional[list] = None,
+) -> list:
     """
-    Get a string of the current UNIX time in seconds.
+    Takes a list of GDAL creation options and adds the following defaults to it if their not specified: </br>
 
-    ## Returns:
-    (_str_): A string of the current UNIX time in seconds.
-    """
-    return str(int(time.time()))
+    Default options are:
+    ```python
+    >>> default_options = [
+    ...     "TILED=YES",
+    ...     "NUM_THREADS=ALL_CPUS",
+    ...     "BIGTIFF=IF_SAFER",
+    ...     "COMPRESS=LZW",
+    ...     "BLOCKXSIZE=256",
+    ...     "BLOCKYSIZE=256",
+    ... ]
+    ```
 
+    Parameters
+    ----------
+    options : Optional[list], optional
+        A list of GDAL creation options, default: None
 
-def is_float(value):
+    Returns
+    -------
+    list
+        A list of GDAL creation options with the defaults added.
     """
-    Check if a value is a float. If it is a string, try to convert it to a float.
-
-    ## Args:
-    `value` (_any_): The value to check.
+    assert isinstance(options, (list, type(None))), "Options must be a list or None."
 
-    ## Returns:
-    (_bool_): **True** if the value is a float, **False** otherwise.
-    """
-    if isinstance(value, float):
-        return True
-    elif isinstance(value, str):
-        try:
-            float(value)
-            return True
-        except ValueError:
-            return False
-    else:
-        return False
+    if options is None:
+        options = []
 
+    internal_options = list(options)
 
-def is_number(potential_number):
-    """
-    Check if variable is a number.
+    opt_str = " ".join(internal_options)
+    if "TILED" not in opt_str:
+        internal_options.append("TILED=YES")
 
-    ## Args:
-    `potential_number` (_any_): The variable to check. </br>
+    if "NUM_THREADS" not in opt_str:
+        internal_options.append("NUM_THREADS=ALL_CPUS")
 
-    ## Returns:
-    (_bool_): **True** if the variable is a number, **False** otherwise.
-    """
-    if isinstance(potential_number, float):
-        return True
+    if "BIGTIFF" not in opt_str:
+        internal_options.append("BIGTIFF=IF_SAFER")
 
-    if isinstance(potential_number, int):
-        return True
+    if "COMPRESS" not in opt_str:
+        internal_options.append("COMPRESS=LZW")
 
-    return False
+    if "BLOCKXSIZE" not in opt_str:
+        internal_options.append("BLOCKXSIZE=256")
 
+    if "BLOCKYSIZE" not in opt_str:
+        internal_options.append("BLOCKYSIZE=256")
 
-def is_int(value):
-    """
-    Check if a value is an integer. If it is a string, try to convert it to an integer.
+    return internal_options
 
-    ## Args:
-    `value` (_any_): The value to check. </br>
 
-    ## Returns:
-    (_bool_): **True** if the value is an integer, **False** otherwise.
+def get_gdal_memory() -> list:
     """
-    if isinstance(value, int):
-        return True
-    elif isinstance(value, str):
-        try:
-            int(value)
-            return True
-        except ValueError:
-            return False
+    Get at list of all active memory layers in GDAL.
+    
+    Returns
+    -------
+    list
+        A list of all active memory layers in GDAL.
+    """
+    if hasattr(gdal, "listdir"):
+        datasets = [ds.name for ds in gdal.listdir("/vsimem")]
+    elif hasattr(gdal, "ReadDir"):
+        datasets = ["/vsimem/" + ds for ds in gdal.ReadDir("/vsimem")]
     else:
-        return False
+        warn("Unable to get list of memory datasets.", RuntimeWarning)
+        return []
 
+    return datasets
 
-def is_list_all_the_same(lst):
-    """
-    Check if a list contains all the same elements.
 
-    ## Args:
-    `lst` (_list_): The list to check. </br>
+def clear_gdal_memory() -> None:
+    """
+    Clears all gdal memory.
 
-    ## Returns:
-    (_bool_): **True** if the list contains all the same elements, **False** otherwise.
+    Notes
+    -----
+    This function is not guaranteed to work.
+    It is a best effort attempt to clear all gdal memory.
     """
-    assert isinstance(lst, list), "lst must be a list."
+    memory = get_gdal_memory()
 
-    first = lst[0]
-    for idx, item in enumerate(lst):
-        if idx == 0:
-            continue
+    for dataset in memory:
+        gdal.Unlink(dataset)
 
-        if item != first:
-            return False
+    if len(get_gdal_memory()) != 0:
+        for dataset in get_gdal_memory():
+            opened = None
 
-    return True
+            if _check_is_raster(dataset):
+                opened = gdal.Open(dataset)
+            elif _check_is_raster(dataset):
+                opened = ogr.Open(dataset)
+            else:
+                print(f"Unable to open dataset: {dataset}")
+                continue
+            driver = opened.GetDriver()
+            driver.Delete(dataset)
 
+            opened = None
+            driver = None
 
-def file_exists(path):
+    if len(get_gdal_memory()) != 0:
+        warn("Failed to clear all GDAL memory.", RuntimeWarning)
+
+
+def _check_is_valid_ext(ext: str) -> bool:
     """
-    Check if a file exists. Also checks vsimem.
+    Check if a file extension has a valid GDAL or OGR driver.
 
-    ## Args:
-    `path` (_str_): The path to the file. </br>
+    Parameters
+    ----------
+    ext : str
+        The file extension to check.
 
-    ## Returns:
-    (_bool_): **True** if the file exists, **False** otherwise.
+    Returns
+    -------
+    bool
+        True if the file extension is a valid GDAL or OGR driver, False otherwise.
     """
-    assert isinstance(path, str), "path must be a string."
+    assert isinstance(ext, str), "ext must be a string."
+    if len(ext) == 0:
+        return False
 
-    if os.path.exists(path):
+    if ext in utils_translate._get_valid_driver_extensions():
         return True
 
-    try:
-        if hasattr(gdal, "listdir"):
-            if path in gdal.listdir("/vsimem"):
-                return True
-        elif hasattr(gdal, "ReadDir"):
-            paths = ["/vsimem/" + ds for ds in gdal.ReadDir("/vsimem")]
-            if path in paths:
-                return True
-        else:
-            print("Warning, unable to access vsimem.")
-    except:  # pylint: disable=bare-except
-        pass
-
     return False
 
 
-def folder_exists(path):
+def _check_is_valid_raster_ext(ext: str) -> bool:
     """
-    Check if a folder exists.
-
-    ## Args:
-    `path` (_str_): The path to the folder. </br>
+    Check if a file extension has a valid GDAL driver.
 
-    ## Returns:
-    (_bool_): **True** if the folder exists, **False** otherwise.
+    Parameters
+    ----------
+    ext : str
+        The file extension to check.
+
+    Returns
+    -------
+    bool
+        True if the file extension is a valid GDAL Raster driver, False otherwise.
     """
-    if isinstance(path, str):
-        abs_dir = os.path.isdir(path)
-        if abs_dir:
-            return True
+    assert isinstance(ext, str), "ext must be a string."
+    if len(ext) == 0:
+        return False
 
-        abs_dir = os.path.isdir(os.path.abspath(path))
-        if abs_dir:
-            return True
+    if ext in utils_translate._get_valid_raster_driver_extensions():
+        return True
 
     return False
 
 
-def delete_files_in_folder(folder):
+def _check_is_valid_vector_ext(ext: str) -> bool:
     """
-    Delete all files in a folder. Does not remove subfolders.
+    Check if a file extension has a valid OGR driver.
 
-    ## Args:
-    `folder` (_str_): The path to the folder. </br>
-
-    ## Returns:
-    (_bool_): **True** if the files were deleted, throws exception otherwise..
+    Parameters
+    ----------
+    ext : str
+        The file extension to check.
+
+    Returns
+    -------
+    bool
+        True if the file extension is a valid OGR Vector driver, False otherwise.
     """
-    assert isinstance(folder, str), "folder must be a string."
-    assert folder_exists(folder), "folder must exist."
+    assert isinstance(ext, str), "ext must be a string."
+    if len(ext) == 0:
+        return False
 
-    for file in glob(folder + "*.*"):
-        try:
-            os.remove(file)
-        except Exception:
-            print(f"Warning. Could not remove: {file}")
+    if ext in utils_translate._get_valid_vector_driver_extensions():
+        return True
 
-    return True
+    return False
 
 
-def delete_folder(folder):
+def _check_is_file_valid_ext(file_path: str) -> bool:
     """
-    Delete a folder.
+    Check if a file path has a valid GDAL or OGR driver.
 
-    ## Args:
-    `folder` (_str_): The path to the folder. </br>
+    Parameters
+    ----------
+    file_path : str
+        The file path to check.
 
-    ## Returns:
-    (_bool_): **True** if the folder was deleted, **False** otherwise.
+    Returns
+    -------
+    bool
+        True if the file path is a valid GDAL or OGR driver, False otherwise.
     """
-    assert isinstance(folder, str), "folder must be a string."
-    assert folder_exists(folder), "folder must exist."
+    assert isinstance(file_path, str), "file_path must be a string."
+    assert len(file_path) > 0, "file_path cannot be an empty string."
 
-    shutil.rmtree(folder)
+    ext = utils_path._get_ext_from_path(file_path)
 
-    return True
+    if ext in utils_translate._get_valid_driver_extensions():
+        return True
+
+    return False
 
 
-def delete_file(file):
+def _check_is_file_valid_raster_ext(file_path: str) -> bool:
     """
-    Delete a File
+    Check if a file path has a valid GDAL driver.
 
-    ## Args:
-    `file` (_str_): The path to the file.
+    Parameters
+    ----------
+    file_path : str
+        The file path to check.
 
-    ## Returns:
-    (_bool_): **True** if the file was deleted, **False** otherwise.
+    Returns
+    -------
+    bool
+        True if the file path is a valid GDAL Raster driver, False otherwise.
     """
-    assert isinstance(file, str), "file must be a string."
-    assert file_exists(file), "file must exist."
+    assert isinstance(file_path, str), "file_path must be a string."
+    assert len(file_path) > 0, "file_path cannot be an empty string."
 
-    os.remove(file)
+    ext = utils_path._get_ext_from_path(file_path)
 
-    if file_exists(file):
-        return False
+    if ext in utils_translate._get_valid_raster_driver_extensions():
+        return True
 
-    return True
+    return False
 
 
-def to_number(value):
+def _check_is_file_valid_vector_ext(file_path: str) -> bool:
     """
-    Convert a value to a number.
+    Check if a file path has a valid OGR driver.
 
-    ## Args:
-    `value` (_any_): The value to convert.
+    Parameters
+    ----------
+    file_path : str
+        The file path to check.
 
-    ## Returns:
-    (_float_): The value converted to a number.
+    Returns
+    -------
+    bool
+        True if the file path is a valid OGR Vector driver, False otherwise.
     """
-    assert isinstance(value, (str, int, float)), "value must be a string, integer or float."
-    if is_number(value):
-        return value
+    assert isinstance(file_path, str), "file_path must be a string."
+    assert len(file_path) > 0, "file_path cannot be an empty string."
 
-    if is_float(value):
-        return float(value)
-
-    raise Exception(f"Could not convert {value} to a number.")
+    ext = utils_path._get_ext_from_path(file_path)
 
+    if ext in utils_translate._get_valid_vector_driver_extensions():
+        return True
 
-def make_dir_if_not_exists(path):
-    """
-    Make a directory if it doesn't exist.
+    return False
 
-    ## Args:
-    `path` (_str_): The path to the directory. </br>
 
-    ## Returns:
-    (_str_): The path to the created directory.
+def _get_default_driver_raster() -> gdal.Driver:
     """
-    assert isinstance(path, str), "path must be a string."
-
-    if not folder_exists(path):
-        os.makedirs(path)
-
-    return path
-
+    Get the default GDAL raster driver.
 
-def path_to_ext(path, with_dot=False):
+    Returns
+    -------
+    gdal.Driver
+        The default GDAL raster driver.
     """
-    Get the extension of a file.
+    return gdal.GetDriverByName("GTiff")
 
-    ## Args:
-    `path` (_str_): The path to the file. </br>
 
-    ## Kwargs:
-    `with_dot` (_bool_): If True, return the extension with a dot. (**Default**: `False`) </br>
-
-    ## Returns:
-    (_str_): The extension of the file. (_without the dot_)
+def _get_default_driver_vector() -> ogr.Driver:
     """
-    assert isinstance(path, str), "path must be a string."
-    assert isinstance(with_dot, bool), "with_dot must be a boolean."
-
-    basename = os.path.basename(path)
-    basesplit = os.path.splitext(basename)
-    ext = basesplit[1]
+    Get the default OGR vector driver.
 
-    if ext == "" or len(ext) == 1:
-        raise Exception (f"File: {path} has no extension.")
+    Returns
+    -------
+    ogr.Driver
+        The default OGR vector driver.
+    """
+    return ogr.GetDriverByName("GPKG")
 
-    if with_dot:
-        return ext
 
-    return ext[1:]
+def _get_driver_name_from_path(file_path: str) -> str:
+    """
+    Convert a file path to a GDAL or OGR driver ShortName (e.g. "GTiff" for "new_york.tif")
 
+    Parameters
+    ----------
+    file_path : str
+        The file path to convert.
 
-def path_to_folder(path):
+    Returns
+    -------
+    str
+        The GDAL or OGR driver ShortName.
     """
-    Get the folder of a file.
+    assert isinstance(file_path, str), "file_path must be a string."
+    assert len(file_path) > 0, "file_path cannot be an empty string."
 
-    ## Args:
-    `path` (_str_): The path to the file. </br>
+    ext = utils_path._get_ext_from_path(file_path)
 
-    ## Returns:
-    (_str_): The folder of the file.
-    """
-    assert isinstance(path, str), "path must be a string."
+    if _check_is_file_valid_ext(file_path):
+        return utils_translate._get_driver_shortname_from_ext(ext)
 
-    return os.path.dirname(os.path.abspath(path))
+    raise ValueError(f"Unable to parse GDAL or OGR driver from path: {file_path}")
 
 
-def change_path_ext(path, target_ext):
+def _get_vector_driver_name_from_path(file_path: str) -> str:
     """
-    Change the extension of a file.
+    Convert a file path to an OGR driver ShortName (e.g. "FlatGeoBuf" for "new_york.fgb")
 
-    ## Args:
-    `path` (_str_): The path to the file. </br>
-    `target_ext` (_str_): The new extension. </br>
+    Parameters
+    ----------
+    file_path : str
+        The file path to convert.
 
-    ## Returns:
-    (_str_): The path to the file with the new extension.
+    Returns
+    -------
+    str
+        The OGR driver ShortName.
     """
-    assert isinstance(path, str), "path must be a string."
-    assert isinstance(target_ext, str), "target_ext must be a string."
+    assert isinstance(file_path, str), "file_path must be a string."
+    assert len(file_path) > 0, "file_path cannot be an empty string."
 
-    basename = os.path.basename(path)
-    basesplit = os.path.splitext(basename)
-    ext = basesplit[1]
+    ext = utils_path._get_ext_from_path(file_path)
 
-    if ext == "" or len(ext) == 1:
-        raise Exception(f"File: {path} has no extension.")
+    if _check_is_file_valid_vector_ext(file_path):
+        return utils_translate._get_vector_shortname_from_ext(ext)
 
-    return os.path.join(os.path.dirname(path), f"{basesplit[0]}.{target_ext}")
+    raise ValueError(f"Unable to parse GDAL or OGR driver from path: {file_path}")
 
 
-
-def is_valid_mem_path(path):
+def _get_raster_driver_name_from_path(file_path: str) -> str:
     """
-    Check if a path is a valid memory path that has an extension.
+    Convert a file path to a GDAL driver ShortName (e.g. "GTiff" for "new_york.tif")
 
-    ## Args:
-    `path` (_str_): The path to test. </br>
+    Parameters
+    ----------
+    file_path : str
+        The file path to convert.
 
-    ## Returns:
-    (_bool_): **True** if path is a valid memory path, **False** otherwise.
+    Returns
+    -------
+    str
+        The GDAL driver ShortName.
     """
-    if not isinstance(path, str):
-        return False
-
-    if len(path) < len("/vsimem/x"):
-        return False
-
-    ext = os.path.splitext(path)[1]
+    assert isinstance(file_path, str), "file_path must be a string."
+    assert len(file_path) > 0, "file_path cannot be an empty string."
 
-    if ext == "" or ext == ".":
-        return False
+    ext = utils_path._get_ext_from_path(file_path)
 
-    if path.startswith("/vsimem"):
-        return True
+    if _check_is_file_valid_raster_ext(file_path):
+        return utils_translate._get_raster_shortname_from_ext(ext)
 
-    return False
+    raise ValueError(f"Unable to parse GDAL or OGR driver from path: {file_path}")
 
 
-def is_valid_non_memory_path(path):
+def _check_is_dataset_in_memory(
+    raster_or_vector: Union[str, gdal.Dataset, ogr.DataSource],
+) -> bool:
     """
-    Check if a path is valid, not in memory, and has an extension.
-
-    ## Args:
-    `path` (_str_): The path to the file. </br>
+    Check if vector is in memory
 
-    ## Returns:
-    (_bool_): **True** if the path has an extension, **False** otherwise.
+    Parameters
+    ----------
+    raster_or_vector : Union[str, gdal.Dataset, ogr.DataSource]
+        The raster or vector to check.
+    
+    Returns
+    -------
+    bool
+        True if the raster or vector is in memory, False otherwise.
     """
-    if not isinstance(path, str):
-        return False
-
-    ext = os.path.splitext(path)[1]
+    assert isinstance(raster_or_vector, (str, gdal.Dataset, ogr.DataSource)), "raster_or_vector must be a string, gdal.Dataset, or ogr.DataSource."
 
-    if ext == "" or ext == ".":
-        return False
+    if isinstance(raster_or_vector, str):
+        if utils_path._check_file_exists_vsimem(raster_or_vector):
+            return True
 
-    if not folder_exists(path_to_folder(path)):
         return False
 
-    if is_valid_mem_path(path):
-        return False
+    elif isinstance(raster_or_vector, (gdal.Dataset, ogr.DataSource)):
+        driver = raster_or_vector.GetDriver()
+        driver_short_name = None
+        try:
+            driver_short_name = driver.GetName()
+        except AttributeError:
+            driver_short_name = driver.ShortName
 
-    if os.path.isdir(path):
-        return False
+        if driver_short_name in ["MEM", "Memory", "VirtualMem", "VirtualOGR", "Virtual"]:
+            return True
 
-    return True
+        path = raster_or_vector.GetDescription()
+        if utils_path._check_file_exists_vsimem(path):
+            return True
 
+        return False
 
-def is_valid_file_path(path):
-    """
-    Check if a path is valid and has an extension. Path can be in memory.
+    else:
+        raise TypeError("vector_or_raster must be a string, ogr.DataSource, or gdal.Dataset")
 
-    ## Args:
-    `path` (_str_): The path to the file. </br>
 
-    ## Returns:
-    (_bool_): **True** if the path has an extension, **False** otherwise.
+def delete_dataset_if_in_memory(
+    raster_or_vector: Union[str, gdal.Dataset, ogr.DataSource],
+) -> bool:
     """
-    if is_valid_mem_path(path) or is_valid_non_memory_path(path):
-        return True
-
-    return False
+    Delete raster or vector if it is in memory
 
+    Parameters
+    ----------
+    raster_or_vector : Union[str, gdal.Dataset, ogr.DataSource]
+        The raster or vector to delete.
 
-def is_valid_output_path(path, *, overwrite=True):
+    Returns
+    -------
+    bool
+        True if the raster or vector was deleted, False otherwise.
     """
-    Check if an output path is valid.
+    if not isinstance(raster_or_vector, (str, gdal.Dataset, ogr.DataSource)):
+        return False
 
-    ## Args:
-    `path` (_str_): The path to the file. </br>
+    if not isinstance(raster_or_vector, str):
+        path = _get_path_from_dataset(raster_or_vector)
+    else:
+        path = raster_or_vector
 
-    ## Kwargs:
-    `overwrite` (_bool_): **True** if the file should be overwritten, **False** otherwise. </br>
+    if _check_is_dataset_in_memory(raster_or_vector):
+        if isinstance(raster_or_vector, str):
+            gdal.Unlink(raster_or_vector)
+        else:
+            raster_or_vector.Destroy()
+            raster_or_vector = None
 
-    ## Returns:
-    (_bool_): **True** if the output path is valid, **False** otherwise.
-    """
-    if not is_valid_file_path(path):
-        return False
+            gdal.Unlink(path)
 
-    if file_exists(path):
-        if overwrite:
+        datasets = get_gdal_memory()
+        if path not in datasets:
             return True
 
-        return False
-
-    return True
+    return False
 
 
-def is_valid_output_path_list(output_list, *, overwrite=True):
+def delete_dataset_if_in_memory_list(
+    list_of_raster_or_vectors: List[Union[str, gdal.Dataset, ogr.DataSource]],
+) -> bool:
     """
-    Check if a list of output paths are valid.
-
-    ## Args:
-    `output_list` (_list_): The list of paths to the files. </br>
+    Deletes a list of raster or vector if they are in memory
 
-    ## Kwargs:
-    `overwrite` (_bool_): **True** if the file should be overwritten, **False** otherwise. </br>
+    Parameters
+    ----------
+    list_of_raster_or_vectors : List[Union[str, gdal.Dataset, ogr.DataSource]]
+        A list of rasters or vectors to delete.
 
-    ## Returns:
-    (_bool_): **True** if the list of output paths are valid, **False** otherwise.
+    Returns
+    -------
+    bool
+        True if any of the rasters or vectors were deleted, False otherwise.
     """
-    if not isinstance(output_list, list):
-        return False
+    assert isinstance(list_of_raster_or_vectors, list), "list_of_raster_or_vectors must be a list."
 
-    if len(output_list) == 0:
-        return False
+    if len(list_of_raster_or_vectors) == 0:
+        return True
 
-    for path in output_list:
-        if not is_valid_output_path(path, overwrite=overwrite):
-            return False
+    deleted = []
+    for raster_or_vector in list_of_raster_or_vectors:
+        deleted.append(delete_dataset_if_in_memory(raster_or_vector))
 
-    return True
+    if all(deleted):
+        return True
+
+    return False
 
 
-def remove_if_required(path, overwrite):
+def _delete_raster_or_vector(
+    raster_or_vector: Union[str, gdal.Dataset, ogr.DataSource],
+) -> bool:
     """
-    Remove a file if overwrite is True.
+    Delete raster or vector. Can be used on both in memory and on disk.
 
-    ## Args:
-    `path` (_str_): The path to the file. </br>
-    `remove` (_bool_): If True, remove the file. </br>
+    Parameters
+    ----------
+    raster_or_vector : Union[str, gdal.Dataset, ogr.DataSource]
+        The raster or vector to delete.
 
-    ## Returns:
-    (_bool_): **True** if the file was removed, **False** otherwise.
+    Returns
+    -------
+    bool
+        True if the raster or vector was deleted, False otherwise.
     """
-    assert is_valid_output_path(path), f"path must be a valid output path. {path}"
+    assert isinstance(raster_or_vector, (str, gdal.Dataset, ogr.DataSource)), "raster_or_vector must be a string, gdal.Dataset, or ogr.DataSource."
 
-    if overwrite and path.startswith(f"{os.sep}vsimem"):
-        gdal.Unlink(path)
+    if delete_dataset_if_in_memory(raster_or_vector):
         return True
 
-    if overwrite and os.path.exists(path):
-        try:
-            os.remove(path)
-            return True
-        except:
-            raise RuntimeError(f"Error while deleting file: {path}") from None
+    driver_shortname = _get_driver_name_from_path(raster_or_vector)
+    driver = gdal.GetDriverByName(driver_shortname)
+    driver.Delete(raster_or_vector)
+
+    if not utils_path._check_file_exists(raster_or_vector):
+        return True
 
     return False
 
 
-def remove_if_required_list(output_list, overwrite):
+def _check_is_raster_empty(
+    raster: gdal.Dataset,
+) -> bool:
     """
-    Remove a list of files if overwrite is True.
+    Check if a raster has bands or zero width and zero height.
 
-    ## Args:
-    `output_list` (_list_): The list of paths to the files. </br>
-    `remove` (_bool_): If True, remove the files. </br>
+    Parameters
+    ----------
+    raster : gdal.Dataset
+        The raster to check.
 
-    ## Returns:
-    (_bool_): **True** if the files were removed, **False** otherwise.
+    Returns
+    -------
+    bool
+        True if the raster has bands and width and height greater than zero, False otherwise.
     """
-    assert is_valid_output_path_list(output_list), f"output_list must be a valid output path list. {output_list}"
-
-    for path in output_list:
-        remove_if_required(path, overwrite)
-
-    return True
+    assert isinstance(raster, gdal.Dataset), "raster must be a gdal.Dataset."
 
+    if raster.RasterCount == 0:
+        return True
 
-def get_augmented_path(path, *, prefix="", suffix="", add_uuid=True, folder=None):
-    """
-    Gets a basename from a string in the format: </br>
-    `dir/prefix_basename_time_uuid_suffix.ext`
+    if raster.RasterXSize == 0 or raster.RasterYSize == 0:
+        return True
 
-    ## Args:
-    `path` (_str_): The path to the original file. </br>
+    return False
 
-    ## Kwargs:
-    `prefix` (_str_): The prefix to add to the memory path. (**Default**: `""`) </br>
-    `suffix` (_str_): The suffix to add to the memory path. (**Default**: `""`) </br>
-    `add_uuid` (_bool_): If True, add a uuid to the memory path. (**Default**: `True`) </br>
 
-    ## Returns:
-    (_str_): A string of the current UNIX time in seconds.
+def _check_is_vector_empty(
+    vector: ogr.DataSource,
+) -> bool:
     """
-    assert isinstance(path, str), "path must be a string."
-    assert isinstance(folder, (type(None), str)), "folder must be None or a string"
-    assert len(os.path.splitext(os.path.basename(path))[1]) > 1, f"Path must have an extension. {path}"
-
-    if os.path.basename(os.path.abspath(path)) == path:
-        path = PurePosixPath("/vsimem", path).as_posix()
-
-    if folder is not None:
-
-        if folder.startswith("/vsimem"):
-            path = PurePosixPath("/vsimem", os.path.basename(path)).as_posix()
-        else:
-            assert folder_exists(folder), f"folder must exist. {folder}"
-            path = os.path.join(folder, os.path.basename(path))
-
-        if not path.startswith(f"{os.sep}vsimem") and not folder_exists(path_to_folder(folder)):
-            raise ValueError(f"Folder: {folder} does not exist.")
-
-    assert is_valid_file_path(path), f"path must be a valid file path. {path}"
+    Check if a vector has features with geometries
 
-    base = os.path.basename(path)
-    split = list(os.path.splitext(base))
-
-    uuid = ""
-    if add_uuid:
-        uuid = f"_{get_unix_seconds_as_str()}_{str(uuid4())}"
-
-    if is_valid_mem_path(path):
-        if split[1][1:] in get_valid_raster_driver_extensions():
-            split[1] = ".tif"
-        elif split[1][1:] in get_valid_vector_driver_extensions():
-            split[1] = ".gpkg"
-        else:
-            raise ValueError("Unable to parse file extension as valid datasource.")
+    Parameters
+    ----------
+    vector : ogr.DataSource
+        The vector to check.
 
-    basename = f"{prefix}{split[0]}{uuid}{suffix}{split[1]}"
+    Returns
+    -------
+    bool
+        True if the vector has features with geometries, False otherwise.
+    """
+    assert isinstance(vector, ogr.DataSource), "vector must be an ogr.DataSource."
 
-    if is_valid_mem_path(path):
-        out_path = PurePosixPath("/vsimem", basename).as_posix()
-    else:
-        out_path = os.path.join(os.path.dirname(os.path.abspath(path)), basename)
+    layer_count = vector.GetLayerCount()
 
-    return out_path
+    if layer_count == 0:
+        return True
 
+    for layer in range(0, layer_count):
+        layer = vector.GetLayerByIndex(layer)
+        layer.ResetReading()
+
+        if layer.GetFeatureCount() > 0:
+            feature_count = layer.GetFeatureCount()
+
+            for feature in range(feature_count):
+                feature = layer.GetNextFeature()
+
+                # TODO: Expand this to check geometry.
+                if feature is not None:
+                    return False
 
-def get_size(start_path=".", rough=True):
-    """
-    Get the size of a folder.
+    return True
 
-    ## Kwargs:
-    `start_path` (_str_): The path to the folder. (**Default**: `"."`) </br>
-    `rough` (_bool_): If True, return a rough estimate. (**Default**: `True`) </br>
 
-    ## Returns:
-    (_int_): The size of the folder.
+def _check_is_raster(
+    potential_raster: Any,
+    empty_is_invalid: bool = True,
+) -> bool:
+    """
+    Checks if a variable is a valid raster.
+
+    Parameters
+    ----------
+    potential_raster : Union[str, gdal.Dataset]
+        The variable to check.
+
+    empty_is_invalid : bool, optional
+        If True, an empty raster is considered invalid. The default is True.
+
+    Returns
+    -------
+    bool
+        True if the variable is a valid raster, False otherwise.
     """
-    assert isinstance(start_path, str), "start_path must be a string."
-    assert folder_exists(start_path), "start_path must exist."
-    assert isinstance(rough, bool), "rough must be a boolean."
-
-    total_size = 0
-    for dirpath, _dirnames, filenames in os.walk(start_path):
-        for file in filenames:
-            file_path = os.path.join(dirpath, file)
-
-            if not os.path.islink(file_path): # skip if symbolic link
-                total_size += os.path.getsize(file_path)
+    if isinstance(potential_raster, str):
+        if not utils_path._check_file_exists(potential_raster):
+            return False
 
-    if rough is True:
-        return total_size >> 20
+        try:
+            gdal.PushErrorHandler('CPLQuietErrorHandler')
+            opened = gdal.Open(potential_raster, 0)
+            gdal.PopErrorHandler()
+        except RuntimeError:
+            return False
 
-    return total_size
+        if opened is None:
+            return False
 
+        if empty_is_invalid and _check_is_raster_empty(opened):
+            return False
 
-def divide_into_steps(total, step):
-    """
-    Divide a number into steps.
+        opened = None
 
-    ## Args:
-    `total` (_int_): The total number. </br>
-    `step` (_int_): The step size. </br>
+        return True
 
-    ## Returns:
-    (_list_): The list of steps.
-    """
-    assert isinstance(total, int), "total must be an integer."
-    assert isinstance(step, int), "step must be an integer."
+    if isinstance(potential_raster, gdal.Dataset):
 
-    steps = []
-    remainder = total % step
-    divided = int(total / step)
-    for _ in range(step):
-        if remainder > 0:
-            steps.append(divided + 1)
-            remainder -= 1
-        else:
-            steps.append(divided)
+        if empty_is_invalid and _check_is_raster_empty(potential_raster):
+            return False
 
-    return steps
+        return True
 
+    return False
 
-def divide_arr_into_steps(arr, steps_length):
-    """
-    Divide an array into steps.
 
-    ## Args:
-    `arr` (_list_): The array. </br>
-    `steps_length` (_int_): The length of each step. </br>
+def _check_is_raster_list(
+    potential_raster_list,
+    empty_is_invalid=True,
+) -> bool:
+    """
+    Checks if a list of variables are full of valid rasters.
+
+    Parameters
+    ----------
+    potential_raster_list : List[Union[str, gdal.Dataset]]
+        The list of variables to check.
 
-    ## Returns:
-    (_list_): An array divided into steps.
+    empty_is_invalid : bool, optional
+        If True, an empty raster is considered invalid. Default: True.
     """
-    assert isinstance(arr, list), "arr must be a list."
-    assert isinstance(steps_length, int), "steps_length must be an integer."
-
-    steps = divide_into_steps(len(arr), steps_length)
-
-    ret_arr = []
-    last = 0
-    count = 0
-    for step in steps:
-        count += 1
-        if count > len(arr):
-            continue
-        ret_arr.append(arr[last : step + last])
-        last += step
+    if not isinstance(potential_raster_list, list):
+        return False
 
-    return ret_arr
+    if len(potential_raster_list) == 0:
+        return False
 
+    for element in potential_raster_list:
+        if not _check_is_raster(element, empty_is_invalid=empty_is_invalid):
+            return False
 
-def step_ranges(arr_with_steps):
-    """
-    Get the ranges of each step.
+    return True
 
-    ## Args:
-    `arr_with_steps` (_list_): The array with steps. </br>
 
-    ## Returns:
-    (_dict_): A dictionary of type: `{ "id": _int_, "start": _int_, "stop": _int_}`.
+def _check_is_vector(
+    potential_vector: List[Any],
+    empty_is_invalid: bool = True,
+) -> bool:
+    """
+    Checks if a variable is a valid vector.
+
+    Parameters
+    ----------
+    potential_vector : Union[str, ogr.DataSource]
+        The variable to check.
+
+    empty_is_invalid : bool, optional
+        If True, an empty vector is considered invalid. The default is True.
+
+    Returns
+    -------
+    bool
+        True if the variable is a valid vector, False otherwise.
     """
-    assert isinstance(arr_with_steps, list), "arr_with_steps must be a list."
+    if isinstance(potential_vector, ogr.DataSource):
 
-    start_stop = []
-    last = 0
-    for idx, step_size in enumerate(arr_with_steps):
-        fid = idx + 1
+        if empty_is_invalid and _check_is_vector_empty(potential_vector):
+            print(f"Vector: {potential_vector} was empty.")
 
-        start_stop.append(
-            {
-                "id": fid,
-                "start": last,
-                "stop": last + step_size,
-            }
-        )
+            return False
 
-        last += step_size
+        return True
 
-    return start_stop
+    if isinstance(potential_vector, str):
+        gdal.PushErrorHandler("CPLQuietErrorHandler")
 
+        opened = ogr.Open(potential_vector, 0)
+        if opened is None:
+            extension = os.path.splitext(potential_vector)[1][1:]
 
-def recursive_check_type_list_none_or_tuple(potential_type):
-    """
-    Recursively check if a type, list or tuple.
+            if extension == "memory" or "mem":
+                driver = ogr.GetDriverByName("Memory")
+                opened = driver.Open(potential_vector)
 
-    ## Args:
-    `potential_type` (_any_): The variable to test. </br>
-
-    ## Returns:
-    (_bool_): **True** if a type, list or tuple, **False** otherwise.
-    """
-    if isinstance(potential_type, type(None)):
-        return True
+        gdal.PopErrorHandler()
 
-    if isinstance(potential_type, type):
-        return True
+        if isinstance(opened, ogr.DataSource):
 
-    if isinstance(potential_type, (list, tuple)):
-        for item in potential_type:
-            if not recursive_check_type_list_none_or_tuple(item):
+            if empty_is_invalid and _check_is_vector_empty(opened):
                 return False
 
-        return True
+            return True
 
     return False
 
 
-def type_check(
-    variable,
-    types,
-    name="",
-    *,
-    throw_error=True,
-):
+def _check_is_vector_list(
+    potential_vector_list: List[Any],
+    empty_is_invalid=True,
+) -> bool:
+    """
+    Checks if a variable is a valid list of vectors.
+
+    Parameters
+    ----------
+    potential_vector_list : List[any]
+        The variable to check.
+
+    empty_is_invalid : bool, optional
+        If True, an empty vector is considered invalid. Default: True.
+
+    Returns
+    -------
+    bool
+        True if the variable is a valid list of vectors, False otherwise.
     """
-    Utility function to type check the inputs of a function. Check two levels down.
-
-    ## Args:
-    `variable` (_any_): The variable to check. </br>
-    `types` (_tuple_): The types to check against. `(float, int, ...)` </br>
-
-    ## Kargs:
-    `name` (_str_): The name printed in the error string if an error is thrown. (**Default**: `""`)</br>
-    `throw_error` (_bool_): If True, raise an error if the type is not correct. (**Default**: `True`)</br>
-
-    ## Returns:
-    (_bool_): A boolean indicating if the type is valid. If throw_error an error is raised if the input is not a valid type.
-    """
-    assert isinstance(name, str), "name must be a string."
-    assert recursive_check_type_list_none_or_tuple(types), f"types must be a type, list, None, or tuple. not: {types}"
-
-    if not isinstance(types, (list, tuple)):
-        types = [types]
-
-    valid_types = []
-    for valid_type in types:
-        if valid_type is None:
-            valid_types.append(type(None))
-        elif isinstance(valid_type, type):
-            valid_types.append(valid_type)
-        elif isinstance(valid_type, (list, tuple)):
-            valid_types.append(valid_type)
-        else:
-            raise ValueError(f"Invalid type: {valid_type}")
-
-    if not isinstance(variable, (list, tuple)):
-        sublist_valid_types = []
-        for valid_type in valid_types:
-            if not isinstance(valid_type, (list, tuple)):
-                sublist_valid_types.append(valid_type)
-
-        for valid_type in sublist_valid_types:
-            if isinstance(variable, valid_type):
-                return True
-
-    if type(variable) in valid_types:
-        return True
+    if not isinstance(potential_vector_list, list):
+        return False
 
-    type_list = [type(val) for val in valid_types]
+    if len(potential_vector_list) == 0:
+        return False
 
-    if isinstance(variable, list) and type([]) in type_list:
-        for sublist in valid_types:
-            if not isinstance(sublist, list):
-                continue
+    for element in potential_vector_list:
+        if not _check_is_vector(element, empty_is_invalid=empty_is_invalid):
+            return False
 
-            if len(sublist) == 0:
-                return True
+    return True
 
-            found = 0
-            for item in variable:
-                if type(item) in sublist:
-                    found += 1
-
-            if found == len(variable):
-                return True
-
-    if isinstance(variable, tuple) and type(()) in type_list:
-        for sublist in valid_types:
-            if not isinstance(sublist, tuple):
-                continue
 
-            if len(sublist) == 0:
-                return True
+def _check_is_raster_or_vector(
+    potential_raster_or_vector: Any,
+    empty_is_invalid: bool = True,
+) -> bool:
+    """
+    Checks if a variable is a valid raster or vector.
+
+    Parameters
+    ----------
+    potential_raster_or_vector : Union[str, gdal.Dataset, ogr.DataSource]
+        The variable to check.
+
+    empty_is_invalid : bool, optional
+        If True, an empty raster or vector is considered invalid. The default is True.
+
+    Returns
+    -------
+    bool
+        True if the variable is a valid raster or vector, False otherwise.
+    """
+    if _check_is_raster(potential_raster_or_vector, empty_is_invalid=empty_is_invalid):
+        return True
 
-            found = 0
-            for item in variable:
-                if type(item) in sublist:
-                    found += 1
-
-            if found == len(variable):
-                return True
-    if throw_error:
-        raise ValueError(
-            f"The type of variable {name} is not valid. Expected: {types}, got: {type(variable)}"
-        )
+    if _check_is_vector(potential_raster_or_vector, empty_is_invalid=empty_is_invalid):
+        return True
 
     return False
 
 
-def is_list_all_val(arr, val):
+def _check_is_raster_or_vector_list(
+    potential_raster_or_vector_list: List[Any],
+    empty_is_invalid: bool = True,
+) -> bool:
+    """
+    Checks if a variable is a valid list of rasters or vectors.
+
+    Parameters
+    ----------
+    potential_raster_or_vector_list : List[Union[str, gdal.Dataset, ogr.DataSource]]
+        The variable to check.
+
+    empty_is_invalid : bool, optional
+        If True, an empty raster or vector is considered invalid. Default: True.
+
+    Returns
+    -------
+    bool
+        True if the variable is a valid list of rasters or vectors, False otherwise.
     """
-    Check if a list is all a value. This also considers type.
-
-    ## Args:
-    `arr` (_list_): The list to check. </br>
-    `val` (_any_): The value to check against. </br>
+    if not isinstance(potential_raster_or_vector_list, list):
+        return False
 
-    ## Returns:
-    (_bool_): **True** if all elements are x, **False** otherwise.
-    """
-    assert isinstance(arr, list), "arr must be a list."
+    if len(potential_raster_or_vector_list) == 0:
+        return False
 
-    for item in arr:
-        if not isinstance(val, type(item)) or item != val:
+    for element in potential_raster_or_vector_list:
+        if not _check_is_raster_or_vector(element, empty_is_invalid=empty_is_invalid):
             return False
 
     return True
 
 
-def progress(count, total, name="Processing"):
-    """
-    Print a progress bar.
+def _get_path_from_dataset(
+    dataset: Union[str, gdal.Dataset, ogr.DataSource],
+    dataset_type: Optional[bool] = None,
+) -> str:
+    """
+    Gets the path from a datasets. Can be vector or raster, string or opened.
+
+    Parameters
+    ----------
+    dataset : Union[str, gdal.Dataset, ogr.DataSource]
+        The dataset to get the path from.
+
+    dataset_type : Optional[bool], optional
+        The type of the dataset. Can be "raster", "vector" or None. If None, the type is guessed. Default: None.
+    """
+    if (dataset_type == "raster" or dataset_type is None) and _check_is_raster(dataset, empty_is_invalid=False):
+        if isinstance(dataset, str):
+            raster = gdal.Open(dataset, 0)
+        elif isinstance(dataset, gdal.Dataset):
+            raster = dataset
+        else:
+            raise RuntimeError(f"Could not read input raster: {raster}")
 
-    ## Args:
-    `count` (_int_): The current count. </br>
-    `total` (_int_): The total count. </br>
+        path = raster.GetDescription()
+        raster = None
 
-    ## Kwargs:
-    `name` (_str_): The name to show in the progress bar. (**Default**: `"Processing"`) </br>
+        return utils_path._get_unix_path(path)
 
-    ## Returns:
-    (_None_): Returns None.
-    """
-    assert isinstance(count, int), "count must be an integer."
-    assert isinstance(total, int), "total must be an integer."
-    assert isinstance(name, str), "name must be a string."
+    if (dataset_type == "vector" or dataset_type is None) and _check_is_vector(dataset, empty_is_invalid=False):
+        if isinstance(dataset, str):
+            vector = ogr.Open(dataset, 0)
+        elif isinstance(dataset, ogr.DataSource):
+            vector = dataset
+        else:
+            raise RuntimeError(f"Could not read input vector: {vector}")
 
-    sys.stdout.flush()
+        path = vector.GetDescription()
+        vector = None
 
-    try:
-        bar_len = os.get_terminal_size().columns - 24
-    except Exception:
-        bar_len = shutil.get_terminal_size().columns - 24
+        return utils_path._get_unix_path(path)
 
-    filled_len = int(round(bar_len * count / float(total)))
-    display_name = name[:10] + "..: "
+    raise ValueError("The dataset is not a raster or vector.")
 
-    progress_bar = "█" * filled_len + "." * (bar_len - filled_len)
 
-    percents = round(100.0 * count / float(total), 1)
+def _get_path_from_dataset_list(
+    datasets: List[Union[str, gdal.Dataset, ogr.DataSource]],
+    allow_mixed: bool = False,
+    dataset_type: Optional[bool] = None,
+):
+    """
+    Gets the paths from a list of datasets.
 
-    if percents >= 100.0:
-        percents = 100.0
+    Parameters
+    ----------
+    datasets : List[Union[str, gdal.Dataset, ogr.DataSource]]
+        The datasets to get the paths from.
+
+    allow_mixed : bool, optional
+        If True, vectors and rasters can be mixed. Default: False.
+
+    dataset_type : Optional[bool], optional
+        The type of the datasets. Can be "raster", "vector" or None. If None, the type is guessed. Default: None.
+
+    Returns
+    -------
+    List[str]
+        The paths of the datasets.
+    """
+    assert isinstance(datasets, list), "The datasets must be a list."
+    assert isinstance(dataset_type, (str, type(None))), "The dataset_type must be 'raster', 'vector', or None."
+
+    rasters = False
+    vectors = False
+
+    outputs = []
+    for dataset in datasets:
+        if (dataset_type == "raster" or dataset_type is None) and _check_is_raster(dataset, empty_is_invalid=False):
+            dataset_type = "raster"
+            rasters = True
+        elif (dataset_type == "vector" or dataset_type is None) and _check_is_vector(dataset, empty_is_invalid=False):
+            dataset_type = "vector"
+            vectors = True
+        else:
+            raise ValueError(f"The dataset is not a raster or vector. {dataset}")
 
-    if count == total:
-        sys.stdout.write(f"{display_name}[{progress_bar}] {percents} %\r")
-        sys.stdout.flush()
-        print("")
-        return None
-    else:
-        sys.stdout.write(f"{display_name}[{progress_bar}] {percents} %\r")
-        sys.stdout.flush()
+        if rasters and vectors and not allow_mixed:
+            raise ValueError("vectors and rasters are mixed.")
+
+        outputs.append(_get_path_from_dataset(dataset, dataset_type=dataset_type))
 
-    return None
+    return outputs
 
 
-def timing(before, print_msg=True):
+def _get_raster_size(
+    raster: Union[gdal.Dataset, str],
+):
     """
-    Get the time elapsed since the given time.
+    Gets the size of a raster (xres, yres).
 
-    ## Args:
-    `before` (_datetime_): The time to compare. </br>
+    Parameters
+    ----------
+    target : Union[gdal.Dataset, str]
+        The target to get the size from.
 
-    ## Kwargs:
-    `print_msg` (_bool_): If True, print the time elapsed. (**Default**: `True`) </br>
+    target_in_pixels : bool, optional
+        If True, the target is in pixels. Default: False.
 
-    ```python
-    >>> before = datetime.now()
-    >>> long_running_calculation()
-    >>> timing(before)
-    >>> Processing took: 1h 1m 1s
-    ```
+    Returns
+    -------
+    Tuple[float, float]
     """
-    assert isinstance(before, datetime), "before must be a datetime object."
-
-    after = datetime.now()
-    dif = (after - before).total_seconds()
+    assert _check_is_raster(raster), "The target must be a raster."
 
-    hours = int(dif / 3600)
-    minutes = int((dif % 3600) / 60)
-    seconds = f"{dif % 60:.2f}"
+    try:
+        reference = raster if isinstance(raster, gdal.Dataset) else gdal.Open(raster, 0)
+    except RuntimeError:
+        raise RuntimeError(f"Could not read input raster: {raster}") from None
 
-    message = f"Processing took: {hours}h {minutes}m {seconds}s"
+    transform = reference.GetGeoTransform()
+    reference = None
 
-    if print_msg:
-        print(message)
+    x_res = transform[1]
+    y_res = abs(transform[5])
 
-    return message
+    return x_res, y_res
 
 
-def get_dynamic_memory_limit_bytes(*, percentage=80.0, min_bytes=1000000, available=True):
+def _get_dynamic_memory_limit(
+    proportion: float = 0.8,
+    *,
+    min_mb: int = 100,
+    max_mb: Optional[int] = None,
+    available: bool = False,
+) -> int:
     """
     Returns a dynamic memory limit taking into account total memory and CPU cores.
+    The return is in mbytes. For GDAL.
 
-    ## Args:
-    `percentage` (_int_): The percentage of the total memory to use. (Default: **80**)
-
-    ## Returns:
-    (_int_): The dynamic memory limit in bytes.
-    """
-    assert isinstance(percentage, (int, str, float)), "percentage must be an integer."
-
-    if percentage == "auto" or percentage is None:
-        percentage = 80.0
+    The value is interpreted as being in megabytes if the value is less than 10000. For values >=10000, this is interpreted as bytes.
 
-    assert percentage > 0.0 and percentage <= 100.0, "percentage must be > 0 and <= 100."
-
-    dyn_limit = min_bytes
+    Parameters
+    ----------
+    percentage : float, optional.
+        The percentage of the total memory to use. Default: 0.8.
+    
+    min_mb : int, optional.
+        The minimum number of megabytes to be returned. Default: 100.
+    
+    available : bool, optional.
+        If True, consider available memory instead of total memory. Default: False.
+
+    Returns
+    -------
+    int
+        The dynamic memory limit in bytes.
+    """
+    assert isinstance(proportion, (int, float)), "percentage must be an integer."
+    assert isinstance(min_mb, int), "min_mb must be an integer."
+    assert isinstance(available, bool), "available must be a boolean."
+    assert min_mb > 0, "min_mb must be > 0."
+    assert proportion > 0.0 and proportion <= 1.0, "percentage must be > 0 and <= 1."
 
     if available:
-        dyn_limit = round(psutil.virtual_memory().available * (percentage / 100.0), 0)
+        dyn_limit = np.rint(
+            (psutil.virtual_memory().available * proportion)  / (1024 ** 2),
+        )
     else:
-        dyn_limit = round(psutil.virtual_memory().total * (percentage / 100.0), 0)
-
-    if dyn_limit < min_bytes:
-        dyn_limit = min_bytes
+        dyn_limit = np.rint(
+            (psutil.virtual_memory().total * proportion)  / (1024 ** 2),
+        )
 
-    return int(dyn_limit)
+    if dyn_limit < min_mb:
+        dyn_limit = min_mb
 
+    if max_mb is not None:
+        if dyn_limit > max_mb:
+            dyn_limit = max_mb
+
+    # GDALWarpMemoryLimit() expects the value in bytes if it is >= 10000
+    if dyn_limit > 10000:
+        dyn_limit = dyn_limit * (1024 ** 2)
 
-def is_str_a_glob(test_str):
-    """
-    Check if a string is a glob.
+    return int(dyn_limit)
 
-    ## Args:
-    `test_str` (_str_): The string to check.
 
-    ## Returns:
-    (_bool_): **True** if the string is a glob, **False** otherwise.
+def _convert_to_band_list(
+    band_number: Union[int, List[int]],
+    band_count: int,
+) -> List[int]:
     """
-    if not isinstance(test_str, str):
-        return False
+    Converts a band number or list of band numbers to a list of band numbers.
 
-    if len(test_str) < 6:
-        return False
+    Parameters
+    ----------
+    band_number : Union[int, List[int]]
+        The band number or list of band numbers to convert.
 
-    if test_str[-5:] == ":glob":
-        return True
-
-    return False
+    band_count : int
+        The number of bands in the raster.
 
-
-def parse_glob_path(test_str):
-    """
-    Parses a string containing a glob path.
-
-    ## Args:
-    `test_str` (_str_): The string to parse the pattern from.
-
-    ## Returns:
-    (_list_): A list of the matching paths.
+    Returns
+    -------
+    List[int]
+        The list of band numbers.
     """
-    assert is_str_a_glob(test_str), "test_str must be a glob path."
-    pre_glob = test_str[:-5]
+    if not isinstance(band_number, (int, list)):
+        raise TypeError(f"Invalid type for band: {type(band_number)}")
+    if not isinstance(band_count, int):
+        raise TypeError(f"Invalid type for band_count: {type(band_count)}")
 
-    return glob(pre_glob)
+    if band_number == -1:
+        band_number = list(range(1, band_count + 1))
 
+    input_list = band_number if isinstance(band_number, list) else [band_number]
+    output_list = []
 
-def ensure_list(variable_or_list):
-    """
-    Ensure that a variable is a list.
+    if band_count <= 0:
+        raise ValueError("Band count cannot be 0.")
 
-    ## Args:
-    `variable_or_list` (_any_): The variable to check. </br>
+    if len(input_list) == 0:
+        raise ValueError("Band number cannot be 0.")
 
-    ## Returns:
-    (_list_): The variable as a list.
-    """
-    if isinstance(variable_or_list, str) and is_str_a_glob(variable_or_list):
-        return parse_glob_path(variable_or_list)
+    if any([val <= 0 or val > band_count for val in input_list]):
+        raise ValueError("Band number cannot be 0 or above the band count.")
 
-    if isinstance(variable_or_list, list):
-        return variable_or_list
+    for val in input_list:
+        output_list.append(int(val))
 
-    return [variable_or_list]
+    return output_list
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `buteo-0.8.9/buteo/vector/clip.py` & `buteo-0.9.0/buteo/vector/clip.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,184 +2,202 @@
 ### Clip vectors to other geometries ###
 
 Clip vector files with other geometries. Can come from rasters or vectors.
 """
 
 # Standard library
 import sys; sys.path.append("../../")
+from typing import Union, Optional, List
 
 # External
 from osgeo import ogr, gdal, osr
 
 # Internal
-from buteo.utils import core_utils, gdal_utils
-from buteo.raster import core_raster
+from buteo.utils import (
+    utils_io,
+    utils_base,
+    utils_gdal,
+    utils_path,
+    utils_bbox,
+    utils_projection,
+)
 from buteo.vector import core_vector
-from buteo.vector.reproject import _reproject_vector
+from buteo.vector.reproject import _vector_reproject
 
 
 
-def _clip_vector(
-    vector,
-    clip_geom,
-    out_path=None,
-    *,
-    to_extent=False,
-    target_projection=None,
-    preserve_fid=True,
-    promote_to_multi=True,
-):
+def _vector_clip(
+    vector: Union[str, ogr.DataSource],
+    clip_geom: Union[str, ogr.DataSource],
+    out_path: Optional[str] = None,
+    to_extent: bool = False,
+    target_projection: Optional[Union[str, int, ogr.DataSource, gdal.Dataset, osr.SpatialReference]] = None,
+    preserve_fid: bool = True,
+    promote_to_multi: bool = True,
+    overwrite: bool = True,
+) -> str:
     """ Internal. """
-
-    input_path = gdal_utils.get_path_from_dataset(vector)
+    assert isinstance(vector, (str, ogr.DataSource)), "Invalid vector input."
+    assert isinstance(clip_geom, (str, ogr.DataSource)), "Invalid clip_geom input."
 
     if out_path is None:
-        out_path = gdal_utils.create_memory_path(
-            input_path,
-            prefix="",
-            suffix="_clip",
-            add_uuid=True,
-        )
+        out_path = utils_path._get_temp_filepath(vector, suffix="_clipped", ext="gpkg")
+    else:
+        assert utils_path._check_is_valid_output_filepath(out_path, overwrite), "Invalid vector output path."
 
-    assert core_utils.is_valid_output_path(out_path), "Invalid output path"
+    input_path = utils_gdal._get_path_from_dataset(vector)
 
     options = []
 
     clear_memory = False
     geometry_to_clip = None
-    if gdal_utils.is_vector(clip_geom):
+    if utils_gdal._check_is_vector(clip_geom):
         if to_extent:
-            extent = core_vector._vector_to_metadata(clip_geom)["get_bbox_vector"]() # pylint: disable=not-callable
+            clip_geom_meta = core_vector._get_basic_metadata_vector(clip_geom)
+            bbox = clip_geom_meta["bbox"]
+            proj = clip_geom_meta["projection_osr"]
+            extent = utils_bbox._get_vector_from_bbox(bbox, proj)
             geometry_to_clip = extent
             clear_memory = True
         else:
-            geometry_to_clip = core_vector._open_vector(clip_geom)
-    elif gdal_utils.is_raster(clip_geom):
-        extent = core_raster._raster_to_metadata(clip_geom)["get_bbox_vector"]() # pylint: disable=not-callable
-        geometry_to_clip = extent
-        clear_memory = True
+            geometry_to_clip = core_vector._vector_open(clip_geom)
     else:
         raise ValueError(f"Invalid input in clip_geom, unable to parse: {clip_geom}")
 
-    clip_vector_path = gdal_utils.get_path_from_dataset(geometry_to_clip)
-    clip_vector_reprojected = _reproject_vector(clip_vector_path, vector)
+    clip_vector_path = utils_gdal._get_path_from_dataset(geometry_to_clip)
+    clip_vector_reprojected = _vector_reproject(clip_vector_path, vector)
 
     if clear_memory:
-        gdal_utils.delete_if_in_memory(clip_vector_path)
+        utils_gdal.delete_dataset_if_in_memory(clip_vector_path)
 
-    x_min, x_max, y_min, y_max = core_vector._vector_to_metadata(clip_vector_reprojected)["extent"]
+    x_min, x_max, y_min, y_max = core_vector._get_basic_metadata_vector(clip_vector_reprojected)["bbox"]
 
     options.append(f"-spat {x_min} {y_min} {x_max} {y_max}")
-
     options.append(f'-clipsrc "{clip_vector_reprojected}"')
 
     if promote_to_multi:
         options.append("-nlt PROMOTE_TO_MULTI")
 
     if preserve_fid:
         options.append("-preserve_fid")
     else:
         options.append("-unsetFid")
 
     if target_projection is not None:
-        wkt = gdal_utils.parse_projection(target_projection, return_wkt=True).replace(" ", "\\")
+        wkt = utils_projection.parse_projection(target_projection, return_wkt=True).replace(" ", "\\")
 
         options.append(f'-t_srs "{wkt}"')
 
     # dst  # src
     success = gdal.VectorTranslate(
         out_path,
         input_path,
-        format=gdal_utils.path_to_driver_vector(out_path),
+        format=utils_gdal._get_vector_driver_name_from_path(out_path),
         options=" ".join(options),
     )
 
-    gdal_utils.delete_if_in_memory(clip_vector_reprojected)
+    utils_gdal.delete_dataset_if_in_memory(clip_vector_reprojected)
 
     if success != 0:
         return out_path
     else:
-        raise Exception("Error while clipping geometry.")
+        raise RuntimeError("Error while clipping geometry.")
 
 
-def clip_vector(
-    vector,
-    clip_geom,
-    out_path=None,
-    *,
-    to_extent=False,
-    target_projection=None,
-    preserve_fid=True,
-    prefix="",
-    suffix="",
-    add_uuid=False,
-    allow_lists=True,
-    overwrite=True,
-    promote_to_multi=True,
-):
+def vector_clip(
+    vector: Union[str, ogr.DataSource, List[Union[str, ogr.DataSource]]],
+    clip_geom: Union[str, ogr.DataSource],
+    out_path: Optional[str] = None,
+    to_extent: bool = False,
+    target_projection: Optional[Union[str, int, gdal.Dataset, ogr.DataSource, osr.SpatialReference]] = None,
+    preserve_fid: bool = True,
+    prefix: str = "",
+    suffix: str = "",
+    add_uuid: bool = False,
+    overwrite: bool = True,
+    promote_to_multi: bool = True,
+) -> Union[str, List[str]]:
     """
     Clips a vector to a geometry.
 
-    ## Args:
-    `vector` (_str_/_ogr.DataSource_/_list_): Vector(s) to clip. </br>
-    `clip_geom` (_str_/_ogr.Geometry_): Vector to clip with. </br>
-
-    ## Kwargs:
-    `out_path` (_str_/_None_): Output path. If None, memory vectors are created. (Default: **None**) </br>
-    `to_extent` (_bool_): Clip to extent. (Default: **False**) </br>
-    `target_projection` (_str_/_ogr.DataSource_/_gdal.Dataset_/_osr.SpatialReference_/_int_/_None_): Target projection. (Default: **None**) </br>
-    `preserve_fid` (_bool_): Preserve fid. (Default: **True**) </br>
-    `prefix` (_str_): Prefix to add to the output path. (Default: **""**) </br>
-    `suffix` (_str_): Suffix to add to the output path. (Default: **""**) </br>
-    `add_uuid` (_bool_): Add UUID to the output path. (Default: **False**) </br>
-    `allow_lists` (_bool_): Allow lists of vectors as input. (Default: **True**) </br>
-    `overwrite` (_bool_): Overwrite output if it already exists. (Default: **True**) </br>
-    `promote_to_multi` (_bool_): Should POLYGON by promoted to MULTIPOLYGON.. (Default: **True**) </br>
-
-    ## Returns:
-    (_str_/_list_): Output path(s) of clipped vector(s).
+    Parameters
+    ----------
+    vector : Union[str, ogr.DataSource, List[Union[str, ogr.DataSource]]]
+        Vector(s) to clip.
+
+    clip_geom : Union[str, ogr.DataSource]
+        Vector to clip with.
+
+    out_path : Optional[str], optional
+        Output path. If None, memory vectors are created. Default: None
+    
+    to_extent : bool, optional
+        Clip to extent. Default: False
+
+    target_projection : Optional[Union[str, int, gdal.Dataset, ogr.DataSource, osr.SpatialReference]], optional
+        Target projection. Default: None
+    
+    preserve_fid : bool, optional
+        Preserve fid. Default: True
+
+    prefix : str, optional
+        Prefix to add to the output path. Default: ""
+
+    suffix : str, optional
+        Suffix to add to the output path. Default: ""
+
+    add_uuid : bool, optional
+        Add a uuid to the output path. Default: False
+
+    overwrite : bool, optional
+        Overwrite output. Default: True
+
+    promote_to_multi : bool, optional
+        Promote to multi. Default: True
+
+    Returns
+    -------
+    Union[str, List[str]]
+        Path to the clipped vector(s)
     """
-    core_utils.type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
-    core_utils.type_check(clip_geom, [ogr.DataSource, gdal.Dataset, str, list, tuple], "clip_geom")
-    core_utils.type_check(out_path, [str, None], "out_path")
-    core_utils.type_check(to_extent, [bool], "to_extent")
-    core_utils.type_check(target_projection, [str, ogr.DataSource, gdal.Dataset, osr.SpatialReference, int, None], "target_projection")
-    core_utils.type_check(preserve_fid, [bool], "preserve_fid")
-    core_utils.type_check(prefix, [str], "prefix")
-    core_utils.type_check(suffix, [str], "suffix")
-    core_utils.type_check(add_uuid, [bool], "add_uuid")
-    core_utils.type_check(allow_lists, [bool], "allow_lists")
-
-    if not allow_lists and isinstance(vector, (list, tuple)):
-        raise ValueError("Lists are not allowed for vector.")
-
-    vector_list = core_utils.ensure_list(vector)
-
-    assert gdal_utils.is_vector_list(vector_list), f"Invalid vector in list: {vector_list}"
-
-    path_list = gdal_utils.create_output_path_list(
-        vector_list,
-        out_path=out_path,
+    utils_base._type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
+    utils_base._type_check(clip_geom, [ogr.DataSource, gdal.Dataset, str, list, tuple], "clip_geom")
+    utils_base._type_check(out_path, [str, None], "out_path")
+    utils_base._type_check(to_extent, [bool], "to_extent")
+    utils_base._type_check(target_projection, [str, ogr.DataSource, gdal.Dataset, osr.SpatialReference, int, None], "target_projection")
+    utils_base._type_check(preserve_fid, [bool], "preserve_fid")
+    utils_base._type_check(prefix, [str], "prefix")
+    utils_base._type_check(suffix, [str], "suffix")
+    utils_base._type_check(add_uuid, [bool], "add_uuid")
+
+    input_is_list = isinstance(vector, list)
+    input_data = utils_io._get_input_paths(vector, "vector")
+    output_data = utils_io._get_output_paths(
+        input_data,
+        out_path,
         prefix=prefix,
         suffix=suffix,
         add_uuid=add_uuid,
         overwrite=overwrite,
     )
 
+    utils_path._delete_if_required_list(output_data, overwrite)
+
     output = []
-    for index, in_vector in enumerate(vector_list):
+    for idx, in_vector in enumerate(input_data):
         output.append(
-            _clip_vector(
+            _vector_clip(
                 in_vector,
                 clip_geom,
-                out_path=path_list[index],
+                out_path=output_data[idx],
                 to_extent=to_extent,
                 target_projection=target_projection,
                 preserve_fid=preserve_fid,
                 promote_to_multi=promote_to_multi,
+                overwrite=overwrite,
             )
         )
 
-    if isinstance(vector, list):
+    if input_is_list:
         return output
 
     return output[0]
```

### Comparing `buteo-0.8.9/buteo/vector/convert_parts.py` & `buteo-0.9.0/buteo/vector/convert_parts.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,47 +2,52 @@
 ### Convert geometry composition. ###
 
 Convert geometries from multiparts and singleparts and vice versa.
 """
 
 # Standard library
 import sys; sys.path.append("../../")
+from typing import Union, Optional, List
 
 # External
 from osgeo import ogr
 
 # Internal
-from buteo.utils import core_utils, gdal_utils
+from buteo.utils import (
+    utils_base,
+    utils_gdal,
+    utils_path,
+    utils_io,
+)
 from buteo.vector import core_vector
 
 
 
 def _singlepart_to_multipart(
-    vector,
-    out_path=None,
-    *,
-    overwrite=True,
-    add_index=True,
-    process_layer=-1,
-):
+    vector: Union[str, ogr.DataSource],
+    out_path: Optional[str] = None,
+    overwrite: bool = True,
+    add_index: bool = True,
+    process_layer: int = -1,
+) -> str:
     """ Internal. """
     assert isinstance(vector, (ogr.DataSource, str)), "Invalid input vector"
-    assert gdal_utils.is_vector(vector), "Invalid input vector"
+    assert utils_gdal._check_is_vector(vector), "Invalid input vector"
 
     if out_path is None:
-        out_path = gdal_utils.create_memory_path(gdal_utils.get_path_from_dataset(vector), add_uuid=True)
+        out_path = utils_path._get_temp_filepath(vector)
 
-    assert core_utils.is_valid_output_path(out_path, overwrite=overwrite), "Invalid output path"
+    assert utils_path._check_is_valid_output_filepath(out_path, overwrite=overwrite), "Invalid output path"
 
-    ref = core_vector._open_vector(vector)
+    ref = core_vector._vector_open(vector)
 
-    out_format = gdal_utils.get_path_from_dataset(out_path, dataset_type="vector")
+    out_format = utils_gdal._get_path_from_dataset(out_path, dataset_type="vector")
     driver = ogr.GetDriverByName(out_format)
 
-    core_utils.remove_if_required(out_path, overwrite)
+    utils_path._delete_if_required(out_path, overwrite)
 
     metadata = core_vector._vector_to_metadata(ref)
     destination = driver.CreateDataSource(out_path)
 
     for index, layer_meta in enumerate(metadata["layers"]):
         if process_layer != -1 and index != process_layer:
             continue
@@ -60,42 +65,41 @@
 
     destination.FlushCache()
 
     return out_path
 
 
 def _multipart_to_singlepart(
-    vector,
-    out_path=None,
-    *,
-    copy_attributes=False,
-    overwrite=True,
-    add_index=True,
-    process_layer=-1,
-    verbose=False,
-):
+    vector: Union[str, ogr.DataSource],
+    out_path: Optional[str] = None,
+    copy_attributes: bool = False,
+    overwrite: bool = True,
+    add_index: bool = True,
+    process_layer: int = -1,
+    verbose: bool = False,
+) -> str:
     """ Internal. """
     assert isinstance(vector, (ogr.DataSource, str)), "Invalid input vector"
-    assert gdal_utils.is_vector(vector), "Invalid input vector"
+    assert utils_gdal._check_is_vector(vector), "Invalid input vector"
 
     if out_path is None:
-        out_path = gdal_utils.create_memory_path(gdal_utils.get_path_from_dataset(vector), add_uuid=True)
+        out_path = utils_path._get_temp_filepath(vector)
 
-    assert core_utils.is_valid_output_path(out_path, overwrite=overwrite), "Invalid output path"
+    assert utils_path._check_is_valid_output_filepath(out_path, overwrite=overwrite), "Invalid output path"
 
-    ref = core_vector._open_vector(vector)
+    ref = core_vector._vector_open(vector)
 
-    out_format = gdal_utils.get_path_from_dataset(out_path, dataset_type="vector")
+    out_format = utils_gdal._get_path_from_dataset(out_path, dataset_type="vector")
     driver = ogr.GetDriverByName(out_format)
 
-    core_utils.remove_if_required(out_path, overwrite)
+    utils_path._delete_if_required(out_path, overwrite)
 
     metadata = core_vector._vector_to_metadata(ref)
 
-    core_utils.remove_if_required(out_path, overwrite)
+    utils_path._delete_if_required(out_path, overwrite)
 
     destination = driver.CreateDataSource(out_path)
 
     for index, layer_meta in enumerate(metadata["layers"]):
         if process_layer != -1 and index != process_layer:
             continue
 
@@ -192,72 +196,90 @@
                     for field_id in range(field_count):
                         values = feature.GetField(field_id)
                         out_feat.SetField(field_id, values)
 
                 destination_layer.CreateFeature(out_feat)
 
             if verbose:
-                core_utils.progress(_, feature_count - 1, "Splitting.")
+                utils_base.progress(_, feature_count - 1, "Splitting.")
 
     if add_index:
         core_vector.vector_add_index(destination)
 
     return out_path
 
 
-def singlepart_to_multipart(
-    vector,
-    out_path=None,
-    add_index=True,
-    process_layer=-1,
-    prefix="",
-    suffix="",
-    add_uuid=False,
-    overwrite=True,
-    allow_lists=True,
-):
+def vector_singlepart_to_multipart(
+    vector: Union[str, ogr.DataSource, List[Union[str, ogr.DataSource]]],
+    out_path: Optional[str] = None,
+    add_index: bool = True,
+    process_layer: int = -1,
+    prefix: str = "",
+    suffix: str = "",
+    add_uuid: bool = False,
+    overwrite: bool = True,
+    allow_lists: bool = True,
+) -> Union[str, List[str]]:
     """
     Converts a singlepart vector to multipart.
 
-    ## Args:
-    `vector` (_str_/_ogr.DataSource_/_list_): The vector(s) to convert. </br>
-
-    ## Kvargs:
-    `out_path` (_str_/_None_): The path(s) to the output vector. If None a memory output is produced. (Default: **None**) </br>
-    `add_index` (_bool_): Add an geospatial index to the output vector. (Default: **True**) </br>
-    `process_layer` (_int_): The layer index to process. (Default: **-1**) </br>
-    `prefix` (_str_): The prefix to add to the layer name. (Default: **""**) </br>
-    `suffix` (_str_): The suffix to add to the layer name. (Default: **""**) </br>
-    `add_uuid` (_bool_): Add a UUID field to the output vector. (Default: **False**) </br>
-    `overwrite` (_bool_): Overwrite the output vector if it already exists. (Default: **True**) </br>
-    `allow_lists` (_bool_): Allow the input to be a list of vectors. (Default: **True**) </br>
-
-    ## Returns:
-    (_str_/_list_): The path(s) to the output vector.
+    Parameters
+    ----------
+    vector : Union[str, ogr.DataSource, List[Union[str, ogr.DataSource]]]
+        The vector(s) to convert.
+
+    out_path : Optional[str], optional
+        The path(s) to the output vector. If None a memory output is produced. Default: None
+
+    add_index : bool, optional
+        Add an geospatial index to the output vector. Default: True
+
+    process_layer : int, optional
+        The layer index to process. Default: -1
+
+    prefix : str, optional
+        The prefix to add to the layer name. Default: ""
+
+    suffix : str, optional
+        The suffix to add to the layer name. Default: ""
+    
+    add_uuid : bool, optional
+        Add a UUID field to the output vector. Default: False
+
+    overwrite : bool, optional
+        Overwrite the output vector if it already exists. Default: True
+
+    allow_lists : bool, optional
+        Allow lists of vectors as input. Default: True
+
+    Returns
+    -------
+    Union[str, List[str]]
+        The path(s) to the output vector(s).
     """
-    core_utils.type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
-    core_utils.type_check(out_path, [str, [str], None], "out_path")
-    core_utils.type_check(overwrite, [bool], "overwrite")
-    core_utils.type_check(add_index, [bool], "add_index")
-    core_utils.type_check(process_layer, [int], "process_layer")
-    core_utils.type_check(prefix, [str], "prefix")
-    core_utils.type_check(suffix, [str], "suffix")
-    core_utils.type_check(add_uuid, [bool], "add_uuid")
-    core_utils.type_check(allow_lists, [bool], "allow_lists")
+    utils_base._type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
+    utils_base._type_check(out_path, [str, [str], None], "out_path")
+    utils_base._type_check(overwrite, [bool], "overwrite")
+    utils_base._type_check(add_index, [bool], "add_index")
+    utils_base._type_check(process_layer, [int], "process_layer")
+    utils_base._type_check(prefix, [str], "prefix")
+    utils_base._type_check(suffix, [str], "suffix")
+    utils_base._type_check(add_uuid, [bool], "add_uuid")
+    utils_base._type_check(allow_lists, [bool], "allow_lists")
 
     if not allow_lists and isinstance(vector, list):
         raise ValueError("Vector cannot be a list when allow_lists is False.")
 
-    vector_list = core_utils.ensure_list(vector)
+    vector_list = utils_base._get_variable_as_list(vector)
 
-    assert gdal_utils.is_vector_list(vector_list), f"Vector is not a list of vectors. {vector_list}"
+    assert utils_gdal._check_is_vector_list(vector_list), f"Vector is not a list of vectors. {vector_list}"
 
-    path_list = gdal_utils.create_output_path_list(
+    path_list = utils_io._get_output_paths(
         vector_list,
-        out_path=out_path,
+        out_path,
         prefix=prefix,
         suffix=suffix,
         add_uuid=add_uuid,
         overwrite=overwrite,
     )
 
     output = []
@@ -274,67 +296,86 @@
 
     if isinstance(vector, list):
         return output[0]
 
     return output
 
 
-def multipart_to_singlepart(
-    vector,
-    out_path=None,
-    *,
-    overwrite=True,
-    add_index=True,
-    process_layer=-1,
-    verbose=False,
-    prefix="",
-    suffix="",
-    add_uuid=False,
-    allow_lists=True,
-):
+def vector_multipart_to_singlepart(
+    vector: Union[str, ogr.DataSource, List[Union[str, ogr.DataSource]]],
+    out_path: Optional[str] = None,
+    overwrite: bool = True,
+    add_index: bool = True,
+    process_layer: int = -1,
+    verbose: bool = False,
+    prefix: str ="",
+    suffix: str = "",
+    add_uuid: bool = False,
+    allow_lists: bool = True,
+) -> Union[str, List[str]]:
     """
     Converts a multipart vector to singlepart.
 
-    ## Args:
-    `vector` (_str_/_ogr.DataSource_/_list_): The vector(s) to convert. </br>
+    Parameters
+    ----------
+    vector : Union[str, ogr.DataSource, List[Union[str, ogr.DataSource]]]
+        The vector(s) to convert.
+
+    out_path : Optional[str], optional
+        The path(s) to the output vector. If None a memory output is produced. Default: None
+
+    overwrite : bool, optional
+        Overwrite the output vector if it already exists. Default: True
+
+    add_index : bool, optional
+        Add an geospatial index to the output vector. Default: True
+
+    process_layer : int, optional
+        The layer index to process. Default: -1
+
+    verbose : bool, optional
+        Print progress. Default: False
+
+    prefix : str, optional
+        The prefix to add to the layer name. Default: ""
+
+    suffix : str, optional
+        The suffix to add to the layer name. Default: ""
+
+    add_uuid : bool, optional
+        Add a UUID field to the output vector. Default: False
 
-    ## Kvargs:
-    `out_path` (_str_/_None_): The path(s) to the output vector. If None a memory output is produced. (Default: **None**) </br>
-    `overwrite` (_bool_): Overwrite the output vector if it already exists. (Default: **True**) </br>
-    `add_index` (_bool_): Add an geospatial index to the output vector. (Default: **True**) </br>
-    `process_layer` (_int_): The layer index to process. (Default: **-1**) </br>
-    `verbose` (_bool_): Print progress. (Default: **False**) </br>
-    `prefix` (_str_): The prefix to add to the layer name. (Default: **""**) </br>
-    `suffix` (_str_): The suffix to add to the layer name. (Default: **""**) </br>
-    `add_uuid` (_bool_): Add a UUID field to the output vector. (Default: **False**) </br>
-    `allow_lists` (_bool_): Allow the input to be a list of vectors. (Default: **True**) </br>
+    allow_lists : bool, optional
+        Allow lists of vectors as input. Default: True
 
-    ## Returns:
-    (_str_/_list_): The path(s) to the output vector.
+    Returns
+    -------
+    Union[str, List[str]]
+        The path(s) to the output vector(s).
     """
-    core_utils.type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
-    core_utils.type_check(out_path, [str, [str], None], "out_path")
-    core_utils.type_check(overwrite, [bool], "overwrite")
-    core_utils.type_check(add_index, [bool], "add_index")
-    core_utils.type_check(process_layer, [int], "process_layer")
-    core_utils.type_check(prefix, [str], "prefix")
-    core_utils.type_check(suffix, [str], "suffix")
-    core_utils.type_check(add_uuid, [bool], "add_uuid")
-    core_utils.type_check(allow_lists, [bool], "allow_lists")
+    utils_base._type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
+    utils_base._type_check(out_path, [str, [str], None], "out_path")
+    utils_base._type_check(overwrite, [bool], "overwrite")
+    utils_base._type_check(add_index, [bool], "add_index")
+    utils_base._type_check(process_layer, [int], "process_layer")
+    utils_base._type_check(prefix, [str], "prefix")
+    utils_base._type_check(suffix, [str], "suffix")
+    utils_base._type_check(add_uuid, [bool], "add_uuid")
+    utils_base._type_check(allow_lists, [bool], "allow_lists")
 
     if not allow_lists and isinstance(vector, list):
         raise ValueError("Vector cannot be a list when allow_lists is False.")
 
-    vector_list = core_utils.ensure_list(vector)
+    vector_list = utils_base._get_variable_as_list(vector)
 
-    assert gdal_utils.is_vector_list(vector_list), f"Vector is not a list of vectors. {vector_list}"
+    assert utils_gdal._check_is_vector_list(vector_list), f"Vector is not a list of vectors. {vector_list}"
 
-    path_list = gdal_utils.create_output_path_list(
+    path_list = utils_io._get_output_paths(
         vector_list,
-        out_path=out_path,
+        out_path,
         prefix=prefix,
         suffix=suffix,
         add_uuid=add_uuid,
         overwrite=overwrite,
     )
 
     output = []
```

### Comparing `buteo-0.8.9/buteo/vector/core_vector.py` & `buteo-0.9.0/buteo/vector/core_vector.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,132 +11,157 @@
 # TODO: Union, Erase, ..
 # TODO: Sampling functions
 # TODO: Vector intersects, etc..
 
 # Standard library
 import sys; sys.path.append("../../")
 import os
+from typing import Union, Optional, List, Dict, Any, Callable
 
 # External
-import numpy as np
 from osgeo import ogr, gdal, osr
 
 # Internal
-from buteo.utils import bbox_utils, core_utils, gdal_utils
+from buteo.utils import (
+    utils_io,
+    utils_base,
+    utils_gdal,
+    utils_bbox,
+    utils_path,
+    utils_projection,
+)
 
 
-def _open_vector(vector, *, writeable=True, allow_raster=True):
+def _vector_open(
+    vector: Union[str, ogr.DataSource, gdal.Dataset],
+    writeable: bool = True,
+    allow_raster: bool = True,
+) -> ogr.DataSource:
     """ Internal. """
     assert isinstance(vector, (str, ogr.DataSource)), "vector must be a path or a DataSource"
 
     opened = None
-    if gdal_utils.is_vector(vector):
+    if utils_gdal._check_is_vector(vector):
         if isinstance(vector, str):
             gdal.PushErrorHandler("CPLQuietErrorHandler")
             opened = ogr.Open(vector, gdal.GF_Write) if writeable else ogr.Open(vector, gdal.GF_Read)
             gdal.PopErrorHandler()
         elif isinstance(vector, ogr.DataSource):
             opened = vector
         else:
-            raise Exception(f"Could not read input vector: {vector}")
+            raise RuntimeError(f"Could not read input vector: {vector}")
 
-    elif allow_raster and gdal_utils.is_raster(vector):
+    elif allow_raster and utils_gdal._check_is_raster(vector):
         if isinstance(vector, str):
             gdal.PushErrorHandler("CPLQuietErrorHandler")
-            opened = gdal.Open(vector, gdal.GF_Write) if writeable else ogr.Open(vector, gdal.GF_Read)
+            opened = gdal.Open(vector, gdal.GF_Write) if writeable else gdal.Open(vector, gdal.GF_Read)
             gdal.PopErrorHandler()
         elif isinstance(vector, gdal.Dataset):
             opened = vector
         else:
-            raise Exception(f"Could not read input vector: {vector}")
+            raise RuntimeError(f"Could not read input vector: {vector}")
 
-        bbox = bbox_utils.get_bbox_from_geotransform(
+        bbox = utils_bbox._get_bbox_from_geotransform(
             opened.GetGeoTransform(),
             opened.RasterXSize,
             opened.RasterYSize,
         )
 
         projection_wkt = opened.GetProjection()
         projection_osr = osr.SpatialReference()
         projection_osr.ImportFromWkt(projection_wkt)
 
-        vector_bbox = bbox_utils.convert_bbox_to_vector(bbox, projection_osr)
+        vector_bbox = utils_bbox._get_vector_from_bbox(bbox, projection_osr)
         opened = ogr.Open(vector_bbox, gdal.GF_Write) if writeable else ogr.Open(vector_bbox, gdal.GF_Read)
 
     else:
-        raise Exception(f"Could not read input vector: {vector}")
+        raise RuntimeError(f"Could not read input vector: {vector}")
 
     if opened is None:
-        raise Exception(f"Could not read input vector: {vector}")
+        raise RuntimeError(f"Could not read input vector: {vector}")
 
     return opened
 
 
-def open_vector(
-    vector,
-    *,
-    writeable=True,
-    allow_raster=True,
-    allow_lists=True,
-):
+def vector_open(
+    vector: Union[str, ogr.DataSource, gdal.Dataset, List[Union[str, ogr.DataSource, gdal.Dataset]]],
+    writeable: bool = True,
+    allow_raster: bool = True,
+) -> Union[ogr.DataSource, List[ogr.DataSource]]:
     """
     Opens a vector to an ogr.Datasource class.
 
-    ## Args:
-    `vector` (_str_/_ogr.DataSource_/_gdal.Dataset_): The vector to open. If a
-    raster is supplied the bounding box is opened as a vector. </br>
-
-    ## Kwargs:
-    `writeable` (_bool_): If True, the vector is opened in write mode. (Default: **True**) </br>
-    `allow_raster` (_bool_): If True, a raster will be opened as a vector bounding box. (Default: **True**) </br>
-    `allow_lists` (_bool_): If True, the input can be a list of vectors. (Default: **True**) </br>
-
-    ## Returns:
-    (_ogr.DataSource_/_list_): The opened vector(s).
-    """
-    core_utils.type_check(vector, [str, ogr.DataSource, gdal.Dataset, [str, ogr.DataSource, gdal.Dataset]], "vector")
-    core_utils.type_check(writeable, [bool], "writeable")
-
-    if isinstance(vector, list) and not allow_lists:
-        raise ValueError("Cannot open a list of vectors when allow_list is False.")
+    Parameters
+    ----------
+    vector : str, ogr.DataSource, gdal.Dataset, list[str, ogr.DataSource, gdal.Dataset]
+        The vector to open. If a raster is supplied the bounding box is opened as a vector.
+
+    writeable : bool, optional
+        If True, the vector is opened in write mode. Default: True
+
+    allow_raster : bool, optional
+        If True, a raster will be opened as a vector bounding box. Default: True
+    
+    allow_lists : bool, optional
+        If True, the input can be a list of vectors. Default: True
+
+    Returns
+    -------
+    ogr.DataSource, list[ogr.DataSource]
+        The opened vector(s).
+    """
+    utils_base._type_check(vector, [str, ogr.DataSource, gdal.Dataset, [str, ogr.DataSource, gdal.Dataset]], "vector")
+    utils_base._type_check(writeable, [bool], "writeable")
+    utils_base._type_check(allow_raster, [bool], "allow_raster")
 
-    vectors = core_utils.ensure_list(vector)
+    vectors = utils_base._get_variable_as_list(vector)
 
     output = []
     for element in vectors:
-        output.append(_open_vector(element, writeable=writeable, allow_raster=allow_raster))
+        output.append(_vector_open(element, writeable=writeable, allow_raster=allow_raster))
 
     if isinstance(vector, list):
         return output
 
     return output[0]
 
 
-def _vector_to_metadata(vector):
-    """ Internal. """
-    assert isinstance(vector, (str, ogr.DataSource)), "vector must be a path or a DataSource"
-
-    datasource = _open_vector(vector)
-
-    vector_driver = datasource.GetDriver()
-
-    path = datasource.GetDescription()
-    basename = os.path.basename(path)
-    split_path = os.path.split(basename)
-    name = split_path[0]
-    ext = split_path[1]
 
-    driver = vector_driver.GetName()
+def _get_basic_metadata_vector(
+    vector: Union[str, ogr.DataSource],
+) -> Dict[str, Any]:
+    """
+    Get basic metadata from a vector.
+
+    Parameters
+    ----------
+    raster : str or ogr.DataSource
+        The raster to get the metadata from.
+
+    Returns
+    -------
+    Dict[str]
+        A dictionary with the metadata.
+    """
+    utils_base._type_check(vector, [str, ogr.DataSource], "vector")
+
+    datasource = _vector_open(vector)
+
+    # Paths
+    path = os.path.abspath(datasource.GetDescription())
+    in_memory = False
+    if "\\vsimem\\" in path:
+        path = "/" + path.replace(os.path.abspath(os.sep), "")
+        in_memory = True
 
-    in_memory = gdal_utils.is_in_memory(datasource)
+    path = utils_path._get_unix_path(path)
 
-    layer_count = datasource.GetLayerCount()
     layers = []
-
     vector_bbox = None
+    layer_count = datasource.GetLayerCount()
     for layer_index in range(layer_count):
         layer = datasource.GetLayerByIndex(layer_index)
 
         x_min, x_max, y_min, y_max = layer.GetExtent()
         layer_bbox = [x_min, x_max, y_min, y_max]
         vector_bbox = layer_bbox
 
@@ -194,158 +219,96 @@
             "projection_osr": projection_osr,
             "geom_type": geom_type,
             "geom_type_ogr": geom_type_ogr,
             "field_count": field_count,
             "field_names": field_names,
             "field_types": field_types,
             "field_types_ogr": field_types_ogr,
-            "is_raster": False,
-            "is_vector": True,
             "bbox": layer_bbox,
-            "extent": layer_bbox,
         }
 
-        layer_bboxes = bbox_utils.additional_bboxes(layer_bbox, projection_osr)
-
-        for key, value in layer_bboxes.items():
-            layer_dict[key] = value
-
-
-        ## MOVE TO A SINGLE FUNCTION
-        def get_bbox_as_vector_layer():
-            return bbox_utils.convert_bbox_to_vector(layer_bbox, projection_osr) # pylint: disable=cell-var-from-loop
-
-
-        def get_bbox_as_vector_latlng_layer():
-            projection_osr_latlng = osr.SpatialReference()
-            projection_osr_latlng.ImportFromWkt('GEOGCS["WGS 84",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563]],PRIMEM["Greenwich",0],UNIT["degree",0.0174532925199433,AUTHORITY["EPSG","9122"]],AUTHORITY["EPSG","4326"]]')
-            # projection_osr_latlng.ImportFromEPSG(4326)
-
-            return bbox_utils.convert_bbox_to_vector(layer_dict["bbox_latlng"], projection_osr_latlng)  # pylint: disable=cell-var-from-loop
-
+        layers.append(layer_dict)
 
-        layer_dict["get_bbox_vector"] = get_bbox_as_vector_layer
-        layer_dict["get_bbox_vector_latlng"] = get_bbox_as_vector_latlng_layer
+    x_min, x_max, y_min, y_max = vector_bbox
+    area = (x_max - x_min) * (y_max - y_min)
 
-        layers.append(layer_dict)
+    bbox_latlng = utils_projection.reproject_bbox(vector_bbox, projection_osr, utils_projection._get_default_projection_osr())
+    bounds_latlng = utils_bbox._get_bounds_from_bbox(vector_bbox, projection_osr, wkt=False)
+    bounds_area = bounds_latlng.GetArea()
+    x_min, x_max, y_min, y_max = vector_bbox
+    area = (x_max - x_min) * (y_max - y_min)
+    bounds_wkt = bounds_latlng.ExportToWkt()
+
+    centroid = [(x_max - x_min) / 2, (y_max - y_min) / 2]
+    centroid_latlng = utils_projection._reproject_point(
+        centroid,
+        projection_osr,
+        utils_projection._get_default_projection_osr(),
+    )
 
     metadata = {
         "path": path,
-        "basename": basename,
-        "name": name,
-        "ext": ext,
+        "basename": os.path.basename(path),
+        "name": os.path.splitext(os.path.basename(path))[0],
+        "folder": os.path.dirname(path),
+        "ext": os.path.splitext(path)[1],
         "in_memory": in_memory,
-        "projection_wkt": projection_wkt,
+        "driver": datasource.GetDriver().GetName(),
         "projection_osr": projection_osr,
-        "driver": driver,
+        "projection_wkt": projection_wkt,
+        "bbox": vector_bbox,
+        "bbox_gdal": utils_bbox._get_gdal_bbox_from_ogr_bbox(vector_bbox),
+        "bbox_latlng": bbox_latlng,
+        "bounds_latlng": bounds_wkt,
+        "centroid": centroid,
+        "centroid_latlng": centroid_latlng,
         "x_min": vector_bbox[0],
         "x_max": vector_bbox[1],
         "y_min": vector_bbox[2],
         "y_max": vector_bbox[3],
-        "is_vector": True,
-        "is_raster": False,
+        "area_bounds": bounds_area,
+        "area": area,
         "layer_count": layer_count,
         "layers": layers,
-        "extent": vector_bbox,
-        "bbox": vector_bbox,
     }
 
-    vector_bboxes = bbox_utils.additional_bboxes(vector_bbox, projection_osr)
-
-    for key, value in vector_bboxes.items():
-        metadata[key] = value
-
-
-    def get_bbox_as_vector():
-        return bbox_utils.convert_bbox_to_vector(vector_bbox, projection_osr) # pylint: disable=cell-var-from-loop
-
-
-    def get_bbox_as_vector_latlng():
-        projection_osr_latlng = osr.SpatialReference()
-        projection_osr_latlng.ImportFromWkt('GEOGCS["WGS 84",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563]],PRIMEM["Greenwich",0],UNIT["degree",0.0174532925199433,AUTHORITY["EPSG","9122"]],AUTHORITY["EPSG","4326"]]')
-        # projection_osr_latlng.ImportFromEPSG(4326)
-
-        return bbox_utils.convert_bbox_to_vector(metadata["bbox_latlng"], projection_osr_latlng)  # pylint: disable=cell-var-from-loop
-
-
-    metadata["get_bbox_vector"] = get_bbox_as_vector
-    metadata["get_bbox_vector_latlng"] = get_bbox_as_vector_latlng
-
+    layer = None
+    datasource = None
     return metadata
 
 
-def vector_to_metadata(vector, *, allow_lists=True):
-    """
-    Creates a dictionary with metadata about the vector layer.
-
-    ## Args:
-    `vector` (_ogr.DataSource_/_str_/_list_): A vector layer(s) or path(s) to a vector file.
-
-    ## Kwargs:
-    `allow_lists` (_bool_): If **True**, vector can be a list of vector layers or paths. If `False`, `vector` must be a single vector layer or path. (default: **True**)
-
-    ## Returns:
-    (_dict_/_list_) A dictionary with metadata about the vector layer(s) or a list of dictionaries with metadata about the vector layer(s).
-    """
-    core_utils.type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
-    core_utils.type_check(allow_lists, [bool], "allow_lists")
-
-    if isinstance(vector, list) and not allow_lists:
-        raise ValueError("The vector parameter cannot be a list when allow_lists is False.")
-
-    vector_list = core_utils.ensure_list(vector)
-
-    if not gdal_utils.is_vector_list(vector_list):
-        raise ValueError("The vector parameter must be a list of vector layers.")
-
-    output = []
-
-    for in_vector in vector_list:
-        output.append(_vector_to_metadata(in_vector))
-
-    if isinstance(vector, list):
-        return output
-
-    return output[0]
-
-
-def _filter_vector(
-    vector,
-    filter_function,
-    out_path=None,
-    *,
-    process_layer=-1,
-    prefix="",
-    suffix="",
-    overwrite=True,
-):
+def _vector_filter(
+    vector: Union[ogr.DataSource, str],
+    filter_function: Callable,
+    out_path: Optional[str] = None,
+    process_layer: int = -1,
+    prefix: str = "",
+    suffix: str = "",
+    overwrite: bool = True,
+) -> str:
     """ Internal. """
     assert isinstance(vector, (str, ogr.DataSource)), "vector must be a string or an ogr.DataSource object."
     assert isinstance(filter_function, (type(lambda: True))), "filter_function must be a function."
 
-    metadata = _vector_to_metadata(vector)
+    metadata = _get_basic_metadata_vector(vector)
 
     if out_path is None:
-        out_path = gdal_utils.create_memory_path(
-            gdal_utils.get_path_from_dataset(vector),
-            prefix=prefix,
-            suffix=suffix,
-            add_uuid=True,
-        )
+        out_path = utils_path._get_temp_filepath(vector, prefix=prefix, suffix=suffix)
 
-    assert core_utils.is_valid_output_path(out_path, overwrite=overwrite), f"out_path is not a valid output path. {out_path}"
+    assert utils_path._check_is_valid_output_filepath(out_path, overwrite=overwrite), f"out_path is not a valid output path. {out_path}"
 
     projection = metadata["projection_osr"]
 
-    driver = gdal_utils.path_to_driver_vector(out_path)
+    driver_name = utils_gdal._get_vector_driver_name_from_path(out_path)
+    driver = ogr.GetDriverByName(driver_name)
 
     datasource_destination = driver.CreateDataSource(out_path)
-    datasource_original = open_vector(vector)
+    datasource_original = _vector_open(vector)
 
-    for i, _layer in enumerate(metadata["layers"]):
+    for i in range(metadata["layer_count"]):
         if process_layer != -1 and i != process_layer:
             continue
 
         features = metadata["layers"][i]["feature_count"]
         field_names = metadata["layers"][i]["field_names"]
 
         geom_type = metadata["layers"][i]["geom_type_ogr"]
@@ -370,362 +333,412 @@
         layer_destination.SyncToDisk()
         layer_destination.ResetReading()
         layer_destination = None
 
     return out_path
 
 
-def filter_vector(
-    vector,
-    filter_function,
-    *,
-    out_path=None,
-    process_layer=-1,
-    allow_lists=True,
-    prefix="",
-    suffix="",
-    add_uuid=False,
-    overwrite=True,
-):
+def vector_filter(
+    vector: Union[ogr.DataSource, str, List[Union[ogr.DataSource, str]]],
+    filter_function: Callable,
+    out_path: Optional[Union[str, List[str]]] = None,
+    process_layer: int = -1,
+    prefix: str = "",
+    suffix: str = "",
+    add_uuid: bool = False,
+    overwrite: bool = True,
+) -> Union[str, List[str]]:
     """
     Filters a vector using its attribute table and a function.
 
-    ## Args:
-    `vector` (_ogr.DataSource_/_str_/_list_): A vector layer(s) or path(s) to a vector file.
-    `filter_function` (_function_): A function that takes a dictionary of attributes and returns a boolean.
-
-    ## Kwargs:
-    `out_path` (_str_): Path to the output vector file. If `None`, a memory vector will be created. (Default: **None**) </br>
-    `process_layer` (_int_): The index of the layer to process. If `-1`, all layers will be processed. (Default: **-1**) </br>
-    `allow_lists` (_bool_): If **True**, vector can be a list of vector layers or paths. If `False`, `vector` must be a single vector layer or path. (default: **True**) </br>
-    `prefix` (_str_): A prefix to add to the output vector file. (Default: **""**) </br>
-    `suffix` (_str_): A suffix to add to the output vector file. (Default: **""**) </br>
-    `add_uuid` (_bool_): If **True**, a UUID will be added to the output vector file. (Default: **False**) </br>
-    `overwrite` (_bool_): If **True**, the output vector file will be overwritten if it already exists. (Default: **True**) </br>
-
-    ## Returns:
-    (_str_/_list_): Path(s) to the output vector file(s).
-    """
-    core_utils.type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
-    core_utils.type_check(filter_function, [type(lambda: True)], "filter_function")
-    core_utils.type_check(process_layer, [int], "process_layer")
-    core_utils.type_check(allow_lists, [bool], "allow_lists")
-
-    if isinstance(vector, list) and not allow_lists:
-        raise ValueError("The vector parameter cannot be a list when allow_lists is False.")
-
-    vector_list = core_utils.ensure_list(vector)
-
-    if not gdal_utils.is_vector_list(vector_list):
-        raise ValueError("The vector parameter must be a list of vector layers.")
-
-    path_list = gdal_utils.create_output_path_list(
-        vector_list,
-        out_path=out_path,
+    Parameters
+    ----------
+    vector : Union[ogr.DataSource, str, List[Union[ogr.DataSource, str]]]
+        A vector layer(s) or path(s) to a vector file.
+
+    filter_function : Callable
+        A function that takes a dictionary of attributes and returns a boolean.
+    
+    out_path : Optional[str], optional
+        Path to the output vector file. If None, a memory vector will be created. default: None
+
+    process_layer : int, optional
+        The index of the layer to process. If -1, all layers will be processed. default: -1
+
+    prefix : str, optional
+        A prefix to add to the output vector file. default: ""
+
+    suffix : str, optional
+        A suffix to add to the output vector file. default: ""
+
+    add_uuid : bool, optional
+        If True, a uuid will be added to the output path. default: False
+
+    overwrite : bool, optional
+        If True, the output file will be overwritten if it already exists. default: True
+
+    Returns
+    -------
+    Union[str, List[str]]
+        The path(s) to the output vector file(s).
+    """
+    utils_base._type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
+    utils_base._type_check(filter_function, [type(lambda: True)], "filter_function")
+    utils_base._type_check(process_layer, [int], "process_layer")
+    utils_base._type_check(prefix, [str], "prefix")
+    utils_base._type_check(suffix, [str], "suffix")
+    utils_base._type_check(add_uuid, [bool], "add_uuid")
+    utils_base._type_check(overwrite, [bool], "overwrite")
+
+    input_is_list = isinstance(vector, list)
+    input_list = utils_io._get_input_paths(vector, "vector")
+    output_list = utils_io._get_output_paths(
+        input_list,
+        out_path,
         prefix=prefix,
         suffix=suffix,
         add_uuid=add_uuid,
         overwrite=overwrite,
+        change_ext="gpkg",
     )
 
-    output = []
+    utils_path._delete_if_required_list(output_list, overwrite)
 
-    for index, in_vector in vector_list:
-        output.append(_filter_vector(
+    output = []
+    for idx, in_vector in enumerate(input_list):
+        output.append(_vector_filter(
             in_vector,
             filter_function,
-            out_path=path_list[index],
+            out_path=output_list[idx],
             process_layer=process_layer,
             prefix=prefix,
             suffix=suffix,
             overwrite=overwrite,
         ))
 
-    if isinstance(vector, list):
+    if input_is_list:
         return output
 
     return output[0]
 
 
-def vector_add_index(vector, allow_lists=True):
+def vector_add_index(
+    vector: Union[ogr.DataSource, str, List[Union[ogr.DataSource, str]]],
+) -> Union[str, List[str]]:
     """
     Adds a spatial index to the vector in place, if it doesn't have one.
 
-    ## Args:
-    (_ogr.DataSource_/_str_/_list_): A vector layer(s) or path(s) to add indices to.
-
-    ## Kwargs:
-    `allow_lists` (_bool_): If **True**, vector can be a list of vector layers or paths. If `False`, `vector` must be a single vector layer or path. (default: **True**)
-
-    ## Returns:
-    (_str_/_list_): Path(s) to the input rasters.
+    Parameters
+    ----------
+    vector : Union[ogr.DataSource, str, List[Union[ogr.DataSource, str]]]
+        A vector layer(s) or path(s) to a vector file.
+
+    Returns
+    -------
+    Union[str, List[str]]
+        The path(s) to the input vector file(s).
     """
-    core_utils.type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
-
-    if isinstance(vector, list) and not allow_lists:
-        raise ValueError("The vector parameter cannot be a list when allow_lists is False.")
-
-    vector_list = core_utils.ensure_list(vector)
-
-    if not gdal_utils.is_vector_list(vector_list):
-        raise ValueError("The vector parameter must be a list of vector layers.")
+    utils_base._type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
 
-    output = gdal_utils.get_path_from_dataset_list(vector_list)
+    input_is_list = isinstance(vector, list)
+    input_list = utils_io._get_input_paths(vector, "vector")
 
     try:
-        for in_vector in vector_list:
-            metadata = _vector_to_metadata(in_vector)
-            ref = _open_vector(in_vector)
+        for in_vector in input_list:
+            metadata = _get_basic_metadata_vector(in_vector)
+            ref = _vector_open(in_vector)
 
             for layer in metadata["layers"]:
                 name = layer["layer_name"]
                 geom = layer["column_geom"]
 
                 sql = f"SELECT CreateSpatialIndex('{name}', '{geom}') WHERE NOT EXISTS (SELECT HasSpatialIndex('{name}', '{geom}'));"
                 ref.ExecuteSQL(sql, dialect="SQLITE")
     except:
-        raise Exception(f"Error while creating indices for {vector}") from None
+        raise RuntimeError(f"Error while creating indices for {vector}") from None
 
-    if isinstance(vector, list):
-        return output
+    if input_is_list:
+        return input_list
 
-    return output[0]
+    return input_list[0]
 
 
-def _vector_add_shapes_in_place(vector, *, shapes=None, prefix="", verbose=False):
-    """ Internal. """
-    assert isinstance(vector, (ogr.DataSource, str)), "vector must be a vector layer or path to one."
-    assert isinstance(shapes, (list, tuple)) or shapes is None, "shapes must be a list of shapes."
-    assert isinstance(prefix, str), "prefix must be a string."
+def _vector_get_attribute_table(
+    vector: Union[str, ogr.DataSource],
+    process_layer: int = 0,
+    include_fids: bool = False,
+    include_geometry: bool = False,
+    include_attributes: bool = True,
+) -> Dict[str, Any]:
+    """
+    Get the attribute table(s) of a vector.
 
-    all_shapes = ["area", "perimeter", "ipq", "hull", "compactness", "centroid"]
+    Parameters
+    ----------
+    vector : Union[str, ogr.DataSource, List[str, ogr.DataSource]]
+        Vector layer(s) or path(s) to vector layer(s).
+
+    process_layer : int, optional
+        The layer to process. Default: 0 (first layer).
+
+    include_fids : bool, optional
+        If True, will include the FID column. Default: False.
+
+    include_geometry : bool, optional
+        If True, will include the geometry column. Default: False.
+
+    include_attributes : bool, optional
+        If True, will include the attribute columns. Default: True.
+
+    allow_lists : bool, optional
+        If True, will accept a list of vectors. If False, will raise an error if a list is passed. Default: True.
+    
+    Returns
+    -------
+    attribute_table : Dict[str, Any]
+        The attribute table(s) of the vector(s).
+    """
+    assert isinstance(vector, (str, ogr.DataSource)), "vector must be a string or an ogr.DataSource object."
+    assert isinstance(process_layer, int), "process_layer must be an integer."
+    assert isinstance(include_fids, bool), "include_fids must be a boolean."
+    assert isinstance(include_geometry, bool), "include_geometry must be a boolean."
+    assert isinstance(include_attributes, bool), "include_attributes must be a boolean."
 
-    if shapes is None:
-        shapes = all_shapes
-    else:
-        for shape in shapes:
-            if shape not in all_shapes:
-                raise ValueError(f"{shape} is not a valid shape.")
-
-    datasource = _open_vector(vector)
-    out_path = gdal_utils.get_path_from_dataset(datasource, dataset_type="vector")
-    metadata = _vector_to_metadata(datasource)
-
-    for index in range(metadata["layer_count"]):
-        vector_current_fields = metadata["layers"][index]["field_names"]
-        vector_layer = datasource.GetLayer(index)
-
-        vector_layer.StartTransaction()
-
-        # Add missing fields
-        for attribute in shapes:
-            if attribute == "centroid":
-                if "centroid_x" not in vector_current_fields:
-                    field_defn = ogr.FieldDefn(f"{prefix}centroid_x", ogr.OFTReal)
-                    vector_layer.CreateField(field_defn)
-
-                if "centroid_y" not in vector_current_fields:
-                    field_defn = ogr.FieldDefn(f"{prefix}centroid_y", ogr.OFTReal)
-                    vector_layer.CreateField(field_defn)
-
-            elif attribute not in vector_current_fields:
-                field_defn = ogr.FieldDefn(f"{prefix}{attribute}", ogr.OFTReal)
-                vector_layer.CreateField(field_defn)
-
-        vector_feature_count = vector_layer.GetFeatureCount()
-
-        if verbose:
-            core_utils.progress(0, vector_feature_count, name="shape")
-
-        for i in range(vector_feature_count):
-            vector_feature = vector_layer.GetNextFeature()
-
-            try:
-                vector_geom = vector_feature.GetGeometryRef()
-            except Exception:
-                # vector_geom.Buffer(0)
-                Warning("Invalid geometry at : ", i)
-
-            if vector_geom is None:
-                raise Exception("Invalid geometry. Could not fix.")
-
-            centroid = vector_geom.Centroid()
-            vector_area = vector_geom.GetArea()
-            vector_perimeter = vector_geom.Boundary().Length()
-
-            if "ipq" or "compact" in shapes:
-                vector_ipq = 0
-                if vector_perimeter != 0:
-                    vector_ipq = (4 * np.pi * vector_area) / vector_perimeter ** 2
-
-            if "centroid" in shapes:
-                vector_feature.SetField(f"{prefix}centroid_x", centroid.GetX())
-                vector_feature.SetField(f"{prefix}centroid_y", centroid.GetY())
-
-            if "hull" in shapes or "compact" in shapes:
-                vector_hull = vector_geom.ConvexHull()
-                hull_area = vector_hull.GetArea()
-                hull_peri = vector_hull.Boundary().Length()
-                hull_ratio = float(vector_area) / float(hull_area)
-                compactness = np.sqrt(float(hull_ratio) * float(vector_ipq))
-
-            if "area" in shapes:
-                vector_feature.SetField(f"{prefix}area", vector_area)
-            if "perimeter" in shapes:
-                vector_feature.SetField(f"{prefix}perimeter", vector_perimeter)
-            if "ipq" in shapes:
-                vector_feature.SetField(f"{prefix}ipq", vector_ipq)
-            if "hull" in shapes:
-                vector_feature.SetField(f"{prefix}hull_area", hull_area)
-                vector_feature.SetField(f"{prefix}hull_peri", hull_peri)
-                vector_feature.SetField(f"{prefix}hull_ratio", hull_ratio)
-            if "compact" in shapes:
-                vector_feature.SetField(f"{prefix}compact", compactness)
+    ref = _vector_open(vector)
+    metadata = _get_basic_metadata_vector(ref)
 
-            vector_layer.SetFeature(vector_feature)
+    attribute_table_header = metadata["layers"][process_layer]["field_names"]
+    attribute_table = []
 
-            if verbose:
-                core_utils.progress(i, vector_feature_count, name="shape")
+    layer = ref.GetLayer(process_layer)
+    layer.ResetReading()
+    while True:
+        feature = layer.GetNextFeature()
 
-        vector_layer.CommitTransaction()
+        if feature is None:
+            break
 
-    return out_path
+        attributes = [feature.GetFID()]
 
+        for field_name in attribute_table_header:
+            attributes.append(feature.GetField(field_name))
 
-def vector_add_shapes_in_place(vector, *, shapes=None, prefix="", allow_lists=True, verbose=False):
-    """
-    Adds shape calculations to a vector such as area and perimeter.
-    Can also add compactness measurements.
+        if include_geometry:
+            geom_defn = feature.GetGeometryRef()
+            attributes.append(geom_defn.ExportToIsoWkt())
+
+        attribute_table.append(attributes)
+
+    attribute_table_header.insert(0, "fid")
+
+    if include_geometry:
+        attribute_table_header.append("geom")
 
-    ## Args:
-    `vector` (_str_/_ogr.DataSource_/_list_): Vector layer(s) or path(s) to vector layer(s).
+    ref = None
+    layer = None
 
-    ## Kwargs:
-    `shapes` (_list_/_None_): The shapes to calculate. The following a possible: </br>
-        * Area          (In same unit as projection)
-        * Perimeter     (In same unit as projection)
-        * IPQ           (0-1) given as (4*Pi*Area)/(Perimeter ** 2)
-        * Hull Area     (The area of the convex hull. Same unit as projection)
-        * Compactness   (0-1) given as sqrt((area / hull_area) * ipq)
-        * Centroid      (Coordinate of X and Y)
-    The default is all shapes. </br>
-    `prefix` (_str_): Prefix to add to the field names.
-    `allow_lists` (_bool_): If True, will accept a list of vectors. If False, will raise an error if a list is passed.
-    `verbose` (_bool_): If True, will print progress.
-
-    ## Returns:
-    (_str_/_list_): Path(s) to the original rasters that have been augmented in place.
-
-    Returns:
-        Either the path to the updated vector or a list of the input vectors.
-    """
-    core_utils.type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
-    core_utils.type_check(shapes, [[str], None], "shapes")
+    return attribute_table
+
+
+def vector_get_attribute_table(
+    vector: Union[str, ogr.DataSource, List[Union[str, ogr.DataSource]]],
+    process_layer: int = 0,
+    include_fids: bool = False,
+    include_geometry: bool = False,
+    include_attributes: bool = True,
+) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
+    """
+    Get the attribute table(s) of a vector.
 
-    if not allow_lists and isinstance(vector, list):
-        raise ValueError("Lists of vectors are not supported when allow_list is False.")
+    Parameters
+    ----------
+    vector : Union[str, ogr.DataSource, List[str, ogr.DataSource]]
+        Vector layer(s) or path(s) to vector layer(s).
+
+    process_layer : int, optional
+        The layer to process. Default: 0 (first layer).
+
+    include_fids : bool, optional
+        If True, will include the FID column. Default: False.
+
+    include_geometry : bool, optional
+        If True, will include the geometry column. Default: False.
+
+    include_attributes : bool, optional
+        If True, will include the attribute columns. Default: True.
+
+    allow_lists : bool, optional
+        If True, will accept a list of vectors. If False, will raise an error if a list is passed. Default: True.
+    
+    Returns
+    -------
+    attribute_table : Dict[str, Any]
+        The attribute table(s) of the vector(s).
+    """
+    utils_base._type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
+    utils_base._type_check(process_layer, [int], "process_layer")
+    utils_base._type_check(include_fids, [bool], "include_fids")
+    utils_base._type_check(include_geometry, [bool], "include_geometry")
+    utils_base._type_check(include_attributes, [bool], "include_attributes")
 
-    vector_list = core_utils.ensure_list(vector)
-    output = gdal_utils.get_path_from_dataset_list(vector_list)
+    input_is_list = isinstance(vector, list)
+    input_list = utils_io._get_input_paths(vector, "vector")
 
-    for in_vector in vector_list:
-        output.append(_vector_add_shapes_in_place(
+    output = []
+    for in_vector in input_list:
+        output.append(_vector_get_attribute_table(
             in_vector,
-            shapes=shapes,
-            prefix=prefix,
-            verbose=verbose,
+            process_layer=process_layer,
+            include_fids=include_fids,
+            include_geometry=include_geometry,
+            include_attributes=include_attributes,
         ))
 
-    if isinstance(vector, list):
+    if input_is_list:
         return output
 
     return output[0]
 
 
-def vector_get_attribute_table(
-    vector,
-    process_layer=-1,
-    include_fids=False,
-    include_geometry=False,
-    include_attributes=True,
-    allow_lists=True,
+def vector_filter_layer(
+    vector: Union[str, ogr.DataSource, List[Union[str, ogr.DataSource]]],
+    layer_name_or_idx: Union[str, int],
+    out_path: Optional[Union[str, List[str]]] = None,
+    prefix: str = "",
+    suffix: str = "_layer",
+    add_uuid: bool = False,
+    overwrite: bool = True,
 ):
     """
-    Get the attribute table(s) of a vector.
-    """
-    core_utils.type_check(vector, [str, ogr.DataSource, [str, ogr.DataSource]], "vector")
-    core_utils.type_check(process_layer, [int], "process_layer")
-    core_utils.type_check(include_fids, [bool], "include_fids")
-    core_utils.type_check(include_geometry, [bool], "include_geometry")
-    core_utils.type_check(include_attributes, [bool], "include_attributes")
-    core_utils.type_check(allow_lists, [bool], "allow_lists")
+    Filters a multi-layer vector source to a single layer.
+    
+    Parameters
+    ----------
+    vector : Union[str, ogr.DataSource, List[str, ogr.DataSource]]
+        Vector layer(s) or path(s) to vector layer(s).
+    
+    layer_name_or_idx : Union[str, int]
+        The name or index of the layer to filter.
+
+    out_path : Optional[str], optional
+        The path to the output vector. If None, will create a new file in the same directory as the input vector. Default: None.
+
+    prefix : str, optional
+        Prefix to add to the output vector. Default: "".
+
+    suffix : str, optional
+        Suffix to add to the output vector. Default: "_layer".
+    
+    add_uuid : bool, optional
+        If True, will add a UUID to the output vector. Default: False.
+
+    overwrite : bool, optional
+        If True, will overwrite the output vector if it already exists. Default: True.
+
+    Returns
+    -------
+    out_path : str
+        Path to the output vector.
+    """
+    input_is_list = isinstance(vector, list)
+
+    input_list = utils_io._get_input_paths(vector, "vector")
+    output_list = utils_io._get_output_paths(
+        input_list,
+        out_path,
+        prefix=prefix,
+        suffix=suffix,
+        add_uuid=add_uuid,
+        overwrite=overwrite,
+        change_ext="gpkg",
+    )
 
-    ref = open_vector(vector)
-    metadata = _vector_to_metadata(ref)
+    utils_path._delete_if_required_list(output_list, overwrite)
 
-    attribute_table_header = None
-    feature_count = None
+    output = []
+    for idx, in_vector in enumerate(input_list):
+        ref = _vector_open(in_vector)
+        out_path = output_list[idx]
+
+        if isinstance(layer_name_or_idx, int):
+            layer = ref.GetLayerByIndex(layer_name_or_idx)
+        elif isinstance(layer_name_or_idx, str):
+            layer = ref.GetLayer(layer_name_or_idx)
+        else:
+            raise RuntimeError("Wrong datatype for layer selection")
 
-    attribute_table_header = metadata["layers"][process_layer]["field_names"]
-    feature_count = metadata["layers"][process_layer]["feature_count"]
+        driver_name = utils_gdal._get_vector_driver_name_from_path(out_path)
+        driver = ogr.GetDriverByName(driver_name)
 
-    attribute_table = []
+        destination = driver.CreateDataSource(out_path)
+        destination.CopyLayer(layer, layer.GetName(), ["OVERWRITE=YES"])
+        destination.FlushCache()
 
-    layer = ref.GetLayer(process_layer)
+        destination = None
+        ref = None
 
-    for _ in range(feature_count):
-        feature = layer.GetNextFeature()
-        attributes = [feature.GetFID()]
+        output.append(out_path)
 
-        for field_name in attribute_table_header:
-            attributes.append(feature.GetField(field_name))
+    if input_is_list:
+        return output
 
-        if include_geometry:
-            geom_defn = feature.GetGeometryRef()
-            attributes.append(geom_defn.ExportToIsoWkt())
+    return output[0]
 
-        attribute_table.append(attributes)
 
-    attribute_table_header.insert(0, "fid")
+def vector_copy(
+    vector: Union[str, ogr.DataSource, List[Union[str, ogr.DataSource]]],
+    out_path: Optional[Union[str, List[str]]] = None,
+) -> Union[str, List[str]]:
+    """
+    Creates a copy of a vector.
+
+    Parameters
+    ----------
+    vector : Union[str, ogr.DataSource, List[str, ogr.DataSource]]
+        Vector layer(s) or path(s) to vector layer(s).
+
+    out_path : Optional[str], optional
+        The path to the output vector. If None, will create a new file in the same directory as the input vector. Default: None.
+
+    Returns
+    -------
+    out_path : str
+        Path to the output vector.
+    """
+    assert isinstance(vector, (str, ogr.DataSource)), "vector must be a string or an ogr.DataSource object."
+    assert isinstance(out_path, (str, list, type(None))), "out_path must be a string, list, or None."
 
-    if include_geometry:
-        attribute_table_header.append("geom")
+    input_is_list = isinstance(vector, list)
 
-    return attribute_table
+    input_list = utils_io._get_input_paths(vector, "vector")
+    output_list = utils_io._get_output_paths(
+        input_list,
+        out_path,
+    )
 
+    utils_path._delete_if_required_list(output_list, overwrite=True)
 
-def vector_filter_layer(
-    vector,
-    layer_name_or_idx,
-    out_path=None,
-    prefix="",
-    suffix="_layer",
-    add_uuid=False,
-    overwrite=True,
-):
-    """ Filters a multi-layer vector source to a single layer. """
-    ref = open_vector(vector)
-    meta = vector_to_metadata(ref, allow_lists=False)
-
-    out_path = gdal_utils.create_output_path(
-        meta["path"],
-        out_path=out_path,
-        overwrite=overwrite,
-        prefix=prefix,
-        suffix=suffix,
-        add_uuid=add_uuid,
-    )
+    output = []
+    for idx, in_vector in enumerate(input_list):
+        ref = _vector_open(in_vector)
 
-    if isinstance(layer_name_or_idx, int):
-        layer = ref.GetLayerByIndex(layer_name_or_idx)
-    elif isinstance(layer_name_or_idx, str):
-        layer = ref.GetLayer(layer_name_or_idx)
-    else:
-        raise Exception("Wrong datatype for layer selection")
+        driver_name = utils_gdal._get_vector_driver_name_from_path(output_list[idx])
+        driver = ogr.GetDriverByName(driver_name)
 
-    driver = gdal_utils.path_to_driver_vector(out_path)
+        destination = driver.CreateDataSource(output_list[idx])
+        layers = ref.GetLayerCount()
 
-    destination = driver.CreateDataSource(out_path)
-    destination.CopyLayer(layer, layer.GetName(), ["OVERWRITE=YES"])
-    destination.FlushCache()
+        for layer_index in range(layers):
+            layer = ref.GetLayer(layer_index)
+            layer.ResetReading()
+            destination.CopyLayer(layer, layer.GetName(), ["OVERWRITE=YES"])
 
-    return out_path
+        destination.FlushCache()
+        destination = None
+        ref = None
+
+        output.append(output_list[idx])
+
+    if input_is_list:
+        return output
+
+    return output[0]
```

### Comparing `buteo-0.8.9/buteo/vector/merge.py` & `buteo-0.9.0/buteo/vector/merge.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,65 +2,66 @@
 ### Merge vectors. ###
 
 Merges vectors into a single vector file.
 """
 
 # Standard library
 import sys; sys.path.append("../../")
+from typing import Union, List, Optional
 
 # External
 from osgeo import ogr
 
 # Internal
-from buteo.utils import core_utils, gdal_utils
+from buteo.utils import utils_base, utils_gdal, utils_path
 from buteo.vector import core_vector
 
 
 
-def merge_vectors(
-    vectors,
-    out_path=None,
-    *,
-    preserve_fid=True,
-):
+def vector_merge(
+    vectors: Union[str, ogr.DataSource, List[Union[str, ogr.DataSource]]],
+    out_path: Optional[str] = None,
+    preserve_fid: bool = True,
+) -> str:
     """
     Merge vectors to a single geopackage.
 
-    ## Args:
-    `vectors` (_list_): List of vectors to merge.
-
-    ## Kwargs:
-    `out_path` (_str_): Path to output vector. (Default: **None**) </br>
-    `preserve_fid` (_bool_): Preserve FIDs? (Default: **True**)
-
-    ## Returns:
-    (_str_): Path to output vector.
+    Parameters
+    ----------
+    vectors : Union[str, ogr.DataSource, List[Union[str, ogr.DataSource]]]
+        The input vectors.
+
+    out_path : Optional[str], optional
+        The output path, default: None.
+
+    preserve_fid : bool, optional
+        If True, the FIDs will be preserved, default: True.
+
+    Returns
+    -------
+    str
+        The output path.
     """
-    core_utils.type_check(vectors, [[str, ogr.DataSource]], "vector")
-    core_utils.type_check(out_path, [str, [str], None], "out_path")
-    core_utils.type_check(preserve_fid, [bool], "preserve_fid")
+    utils_base._type_check(vectors, [[str, ogr.DataSource]], "vector")
+    utils_base._type_check(out_path, [str, [str], None], "out_path")
+    utils_base._type_check(preserve_fid, [bool], "preserve_fid")
 
-    vector_list = core_utils.ensure_list(vectors)
+    vector_list = utils_base._get_variable_as_list(vectors)
 
-    assert gdal_utils.is_vector_list(vector_list), "Invalid input vector list"
+    assert utils_gdal._check_is_vector_list(vector_list), "Invalid input vector list"
 
     if out_path is None:
-        out_path = gdal_utils.create_memory_path(
-            gdal_utils.get_path_from_dataset(vector_list[0]),
-            prefix="",
-            suffix="_merged",
-            add_uuid=True,
-        )
+        out_path = utils_path._get_temp_filepath(vector_list[0], suffix="_merged")
 
-    driver = ogr.GetDriverByName(gdal_utils.path_to_driver_vector(out_path))
+    driver = ogr.GetDriverByName(utils_gdal._get_vector_driver_name_from_path(out_path))
 
     merged_ds = driver.CreateDataSource(out_path)
 
     for vector in vector_list:
-        ref = core_vector._open_vector(vector)
+        ref = core_vector._vector_open(vector)
         metadata = core_vector._vector_to_metadata(ref)
 
         for layer in metadata["layers"]:
             name = layer["layer_name"]
             merged_ds.CopyLayer(ref.GetLayer(name), name, ["OVERWRITE=YES"])
 
     merged_ds.FlushCache()
```

### Comparing `buteo-0.8.9/buteo/vector/rasterize.py` & `buteo-0.9.0/buteo/vector/rasterize.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,117 +5,147 @@
 
 TODO:
     * Add support for projections
 """
 
 # Standard library
 import sys; sys.path.append("../../")
-
-from buteo.raster.reproject import reproject_raster
-from buteo.vector.reproject import reproject_vector
-
+from typing import Union, Optional, List
 
 # External
-from osgeo import gdal, ogr
+from osgeo import gdal, ogr, osr
+import numpy as np
 
 # Internal
-from buteo.utils import gdal_utils, gdal_enums
+from buteo.utils import (
+    utils_gdal,
+    utils_path,
+    utils_projection,
+    utils_translate,
+)
+from buteo.raster.reproject import raster_reproject
+from buteo.vector.reproject import vector_reproject
 from buteo.vector import core_vector
 from buteo.raster import core_raster
 
 
 
-def rasterize_vector(
-    vector,
-    pixel_size,
-    out_path=None,
-    *,
-    extent=None,
-    projection=None,
-    all_touch=False,
-    dtype="uint8",
-    optim="raster",
-    band=1,
-    fill_value=0,
-    nodata_value=None,
-    check_memory=True,
+def vector_rasterize(
+    vector: Union[str, ogr.DataSource],
+    pixel_size: Union[float, int],
+    out_path: Optional[str] = None,
+    extent: Optional[List[Union[float, int]]] = None,
+    projection: Optional[Union[str, int, osr.SpatialReference, gdal.Dataset, ogr.DataSource]] = None,
+    all_touch: bool = False,
+    dtype: Union[str, np.dtype] = "uint8",
+    optim: str = "raster",
+    band: int = 1,
+    fill_value: Union[int, float] = 0,
+    nodata_value: Optional[Union[int, float]] = None,
+    check_memory: bool = True,
     burn_value=1,
     attribute=None,
-):
+) -> str:
     """
     Rasterize a vector to a raster.
 
-    ## Args:
-    `vector` (_str_/_ogr.DataSource): The vector to rasterize. </br>
-    `pixel_size` (_float_/_int_): The pixel size of the raster. </br>
-
-    ## Kwargs:
-    `out_path` (_str_/_None_): Path to output raster. (Default: **None**) </br>
-    `extent` (_list_/_None_): Extent of raster. (Default: **None**) </br>
-    `all_touch` (_bool_): All touch? (Default: **False**) </br>
-    `dtype` (_str_): Data type of raster. (Default: **"uint8"**) </br>
-    `optim` (_str_): Optimization for raster or vector? (Default: **"raster"**) </br>
-    `band` (_int_): Band to rasterize. (Default: **1**) </br>
-    `fill_value` (_int_/_float_): Fill value. (Default: **0**) </br>
-    `nodata_value` (_int_/_float_/_None_): Nodata value. (Default: **None**) </br>
-    `check_memory` (_bool_): Check memory? (Default: **True**) </br>
-    `burn_value` (_int_/_float_): Value to burn. (Default: **1**) </br>
-    `attribute` (_str_/_None_): Attribute to burn. (Default: **None**)
-
-    ## Returns:
-    (_str_): Path to output raster.
+    Parameters
+    ----------
+    vector : Union[str, ogr.DataSource]
+        The vector to rasterize.
+    
+    pixel_size : Union[float, int]
+        The pixel size of the raster.
+    
+    out_path : Optional[str], optional
+        Path to output raster. Default: None
+
+    extent : Optional[List[Union[float, int]]], optional
+        Extent of raster. Default: None
+
+    projection : Optional[Union[str, int, osr.SpatialReference, gdal.Dataset, ogr.DataSource]], optional
+        Projection of raster. Default: None
+
+    all_touch : bool, optional
+        All pixel touch? Default: False
+
+    dtype : Union[str, np.dtype], optional
+        Data type of raster. Default: "uint8"
+
+    optim : str, optional
+        Optimization for raster or vector? Default: "raster"
+
+    band : int, optional
+        Band to rasterize. Default: 1
+    
+    fill_value : Union[int, float], optional
+        Fill value. Default: 0
+
+    nodata_value : Optional[Union[int, float]], optional
+        Nodata value. Default: None
+
+    check_memory : bool, optional
+        Check memory? Default: True
+
+    burn_value : int, optional
+        Burn value (The value to burn into the raster). Default: 1
+
+    attribute : Optional[str], optional
+        Attribute to rasterize. Default: None
+        This will burn the value of the attribute into the raster.
+
+    Returns
+    -------
+    str
+        Path to output raster.
     """
     vector_fn = vector
 
     if out_path is None:
-        out_path = gdal_utils.create_memory_path(
-            gdal_utils.get_path_from_dataset(vector),
-            add_uuid=True,
-            suffix="_rasterized",
-        )
+        out_path = utils_path._get_temp_filepath(vector, suffix="_rasterized")
 
     if projection is not None:
-        projection = gdal_utils.parse_projection(projection)
+        projection = utils_projection.parse_projection(projection)
 
-        vector_fn = reproject_vector(vector, projection)
+        vector_fn = vector_reproject(vector, projection)
 
         if isinstance(extent, (gdal.Dataset, ogr.DataSource)):
-            if gdal_utils.is_raster(extent):
-                extent = reproject_raster(extent, projection, add_uuid=True, suffix="_reprojected")
+            if utils_gdal._check_is_raster(extent):
+                extent = raster_reproject(extent, projection, add_uuid=True, suffix="_reprojected")
             else:
-                extent = reproject_vector(extent, projection, add_uuid=True, suffix="_reprojected")
+                extent = vector_reproject(extent, projection, add_uuid=True, suffix="_reprojected")
 
         if isinstance(pixel_size, (gdal.Dataset, ogr.DataSource)):
-            if gdal_utils.is_raster(pixel_size):
-                pixel_size = reproject_raster(pixel_size, projection, add_uuid=True, suffix="_reprojected")
+            if utils_gdal._check_is_raster(pixel_size):
+                pixel_size = raster_reproject(pixel_size, projection, add_uuid=True, suffix="_reprojected")
             else:
-                pixel_size = reproject_vector(pixel_size, projection, add_uuid=True, suffix="_reprojected")
+                pixel_size = vector_reproject(pixel_size, projection, add_uuid=True, suffix="_reprojected")
 
     if projection is None and isinstance(pixel_size, (gdal.Dataset, ogr.DataSource)):
         if extent is not None:
-            extent = reproject_raster(extent, pixel_size, add_uuid=True, suffix="_reprojected")
+            extent = raster_reproject(extent, pixel_size, add_uuid=True, suffix="_reprojected")
 
-        vector_fn = reproject_vector(vector, pixel_size, add_uuid=True, suffix="_reprojected")
+        vector_fn = vector_reproject(vector, pixel_size, add_uuid=True, suffix="_reprojected")
 
     # Open the data source and read in the extent
-    source_ds = core_vector._open_vector(vector_fn)
+    source_ds = core_vector._vector_open(vector_fn)
     source_meta = core_vector._vector_to_metadata(vector_fn)
     source_layer = source_ds.GetLayer()
     x_min, x_max, y_min, y_max = source_layer.GetExtent()
 
     if isinstance(pixel_size, (gdal.Dataset, str)):
-        pixel_size_x = core_raster._open_raster(pixel_size).GetGeoTransform()[1]
-        pixel_size_y = abs(core_raster._open_raster(pixel_size).GetGeoTransform()[5])
+        pixel_size_x = core_raster._raster_open(pixel_size).GetGeoTransform()[1]
+        pixel_size_y = abs(core_raster._raster_open(pixel_size).GetGeoTransform()[5])
     elif isinstance(pixel_size, (int, float)):
         pixel_size_x = pixel_size
         pixel_size_y = pixel_size
     elif isinstance(pixel_size, (list, tuple)):
         pixel_size_x, pixel_size_y = pixel_size
     else:
-        raise Exception("pixel_size must be either a gdal.Dataset or a tuple of (x, y)")
+        raise ValueError("pixel_size must be either a gdal.Dataset or a tuple of (x, y)")
 
     # Create the destination data source
     x_res = int((x_max - x_min) / pixel_size_x)
     y_res = int((y_max - y_min) / pixel_size_y)
 
     if extent is not None:
         extent_vector = core_vector._vector_to_metadata(extent)
@@ -130,21 +160,21 @@
 
     try:
         target_ds = gdal.GetDriverByName("GTiff").Create(
             out_path,
             x_res,
             y_res,
             1,
-            gdal_enums.translate_str_to_gdal_dtype(dtype),
+            utils_translate._translate_dtype_gdal_to_numpy(dtype),
         )
     finally:
         gdal.SetConfigOption("CHECK_DISK_FREE_SPACE", "TRUE")
 
     if target_ds is None:
-        raise Exception("Unable to rasterize.")
+        raise RuntimeError("Unable to rasterize.")
 
     target_ds.SetGeoTransform((x_min, pixel_size_x, 0, y_max, 0, -1 * abs(pixel_size_y)))
     target_ds.SetProjection(source_meta["projection_wkt"])
 
     band = target_ds.GetRasterBand(1)
 
     if nodata_value is not None:
@@ -172,11 +202,11 @@
             source_layer,
             burn_values=[burn_value],
             options=options,
         )
     else:
         options.append(f"ATTRIBUTE={attribute}")
         gdal.RasterizeLayer(
-            target_ds, [1], source_layer, options=gdal_utils.default_creation_options(options)
+            target_ds, [1], source_layer, options=utils_gdal._get_default_creation_options(options)
         )
 
     return out_path
```

### Comparing `buteo-0.8.9/buteo/vector/zonal_statistics.py` & `buteo-0.9.0/buteo/vector/zonal_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # from buteo.vector.reproject import reproject_vector
 # from buteo.vector.core_vector import (
 #     open_vector,
 #     _vector_to_memory,
 #     _vector_to_metadata,
 # )
 # from buteo.vector.zonal_statistics_stats import calculate_array_stats
-# from buteo.utils.core_utils import progress
+# from buteo.utils.utils_base import progress
 
 
 
 # import numpy as np
 # from enum import Enum
 
 # from numba import jit
@@ -317,15 +317,15 @@
 #         vector_metadata = _vector_to_metadata(vector)
 #         vector_layer = vector.GetLayer()
 
 #     vector_projection = vector_metadata["projection_osr"]
 #     raster_projection = raster_metadata["projection_osr"]
 
 #     # Read raster data in overlap
-#     raster_transform = np.array(raster_metadata["transform"], dtype=np.float32)
+#     raster_transform = np.array(raster_metadata["geotransform"], dtype=np.float32)
 #     raster_size = np.array(raster_metadata["size"], dtype=np.int32)
 
 #     raster_extent = get_extent(raster_transform, raster_size)
 
 #     vector_extent = np.array(vector_layer.GetExtent(), dtype=np.float32)
 #     overlap_extent = get_intersection(raster_extent, vector_extent)
```

### Comparing `buteo-0.8.9/pyproject.toml` & `buteo-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
-requires = ["flit_core>=3.7.1", "numba>=0.56.2", "psutil>=5.4.8", "PyYAML>=6.0"]
+requires = ["flit_core>=3.8.0", "numba>=0.56.4", "psutil>=5.4.8", "PyYAML>=6.0", "tqdm>=4.62.3"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "buteo"
-version = "0.8.9"
+version = "0.9.0"
 authors = [
   { name="Casper Fibaek", email="casperfibaek@gmail.com" },
 ]
-description = "Geospatial tools for raster preprocessing and EO work."
+description = "Tools for merging Geospatial Analysis and AI."
 readme = "readme.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "numba>=0.56",
   "psutil>=5.4.8",
+  "tqdm>=4.62.3",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/casperfibaek/buteo"
 "Bug Tracker" = "https://github.com/casperfibaek/buteo/issues"
```

### Comparing `buteo-0.8.9/PKG-INFO` & `buteo-0.9.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,155 +1,141 @@
 Metadata-Version: 2.1
 Name: buteo
-Version: 0.8.9
-Summary: Geospatial tools for raster preprocessing and EO work.
+Version: 0.9.0
+Summary: Tools for merging Geospatial Analysis and AI.
 Author-email: Casper Fibaek <casperfibaek@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: numba>=0.56
 Requires-Dist: psutil>=5.4.8
+Requires-Dist: tqdm>=4.62.3
 Project-URL: Bug Tracker, https://github.com/casperfibaek/buteo/issues
 Project-URL: Homepage, https://github.com/casperfibaek/buteo
 
-# Buteo - Facilitating EO-Driven Decision Support Systems
+# Buteo - Geospatial Analysis Meets AI
 
-The Buteo-Toolbox is a series of modules that ease the creation of Earth Observation Driven Spatial Decision Support Systems. The modules are located in the lib folder, geometry used for testing and clipping is located in geometry. In the examples folder there are jupyter notebooks that showcase analysis' done using the toolbox.
+Buteo is a toolbox designed to simplify the process of working with geospatial data in machine learning. It includes tools for reading, writing, and processing geospatial data, as well as tools for creating labels from vector data and generating patches from geospatial data. Buteo makes it easy to ingest data, create training data, and perform inference on geospatial data.
 
-Documentation available at: https://casperfibaek.github.io/buteo/
+Please note that Buteo is under active development, and its API may not be entirely stable. Feel free to report any bugs or suggest improvements.
+
+When using, please pin the version of Buteo you are using to avoid breaking changes.
+
+For documentation, visit: https://casperfibaek.github.io/buteo/
 
 **Dependencies** </br>
-`numpy` (https://numpy.org/) </br>
+`numba` (https://numba.pydata.org/) </br>
 `gdal` (https://gdal.org/) </br>
 
 **Installation** </br>
-`pip install buteo` </br>
-`conda install buteo --channel casperfibaek` </br>
+Using pip:
+```
+pip install gdal
+pip install buteo
+```
+Using conda:
+```
+conda install gdal
+pip install buteo
+```
 
 **Quickstart**
+
+### Reproject (and other functions) to references. (Vector and raster)
 ```python
 import buteo as beo
 
+OUTDIR = "path/to/output/dir"
+
 vector_file_correct_projection = "path/to/vector/file.gpkg"
 raster_files_wrong_projection = "path/to/raster/files/*.tif:glob"
 
-outdir = "path/to/output/dir"
-
 paths_to_reprojected_rasters = beo.reproject_raster(
     raster_files_with_wrong_projection,
     vector_file_with_correct_projection,
     out_path=outdir
 )
 
 paths_to_reprojected_rasters
 >>> [path/to/output/dir/file1.tif, path/to/output/dir/file2.tif, ...]
 ```
 
-</br>
-
-| Example Colabs                        |                                                                                                                                                                                                               |
-|---------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Create labels from OpenStreetMap data | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/casperfibaek/buteo/blob/master/examples/create_labels_from_osm_data.ipynb)            |
-| Scheduled cleaning of geospatial data | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/casperfibaek/buteo/blob/master/examples/rocket_example.ipynb)                         |
-| Clip and remove noise from rasters    | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/casperfibaek/buteo/blob/master/examples/clip_and_remove_noise_raster.ipynb)           |
-| Sharpen nightlights data              | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/casperfibaek/buteo/blob/master/examples/process_nightlights.ipynb)                    |
-| Filters and morphological operations  | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/casperfibaek/buteo/blob/master/examples/filters_and_morphology.ipynb)                 |
-
-
-</br>
+### Align, stack, and make patches from rasters
+```python
+import buteo as beo
 
-# Modules:
+SRCDIR = "path/to/src/dir/"
 
-## raster
+paths_to_aligned_rasters_in_memory = beo.align_rasters(
+    SRCDIR + "*.tif:glob",
+)
 
-- read and verify a raster or a list of rasters
-- clip rasters to other rasters or vectors
-- align a list of rasters for analysis
-- shift, resample and reproject raster data
-- easily manage nodata values
-- parallel zonal statistics (link - host)
+stacked_numpy_arrays = beo.raster_to_array(
+    paths_to_aligned_rasters_in_memory,
+)
 
-## vector
+patches = beo.array_to_patches(
+    stacked_numpy_arrays,
+    256,
+    offsets_y=1, # 1 overlap at 1/2 patch size (128)
+    offsets_x=1, # 1 overlap at 1/2 patch size (128)
+)
 
-- read and verify integrity
-- parallel zonal statistics (link)
-- clip, buffer
+# patches_nr, height, width, channels
+patches
+>>> np.ndarray([10000, 256, 256, 9])
+```
 
-## filter
+### Predict a raster using a model
+```python
+import buteo as beo
 
-- custom convolution based filters.
-- global filters and multispectral indices (link - host)
-- textures for analysis
-- noise reduction of SAR imagery (link - host)
-- kernel designer & reduction bootcamp
+RASTER_PATH = "path/to/raster/raster.tif"
+RASTER_OUT_PATH = "path/to/raster/raster_pred.tif"
 
-## terrain
+array = beo.raster_to_array(RASTER_PATH)
 
-- download srtm, aster and the danish national DEM
-- basic propocessing of the DEM's.
+callback = model.predict # from pytorch, keras, etc..
 
-## earth_observation
+# Predict the raster using overlaps, and borders.
+# Merge using different methods. (median, mad, mean, mode, ...)
+predicted = predict_array(
+    array,
+    callback,
+    tile_size=256,
+)
 
-- download sentinel 1, 2, 3, 5, landsat and modis data
-- process sentinel 1 and 2 (sentinel 1 requires esa-snap dep.)
-- generate mosaics of sentinel 1 and 2
-- pansharpen bands
-- noise reduction of SAR imagery (link)
-- multispectral indices (link)
+# Write the predicted raster to disk
+beo.array_to_raster(
+    predicted,
+    reference=RASTER_PATH,
+    out_path=RASTER_OUT_PATH,
+)
+# Path to the predicted raster
+>>> "path/to/raster/raster_pred.tif"
+```
 
-## machine_learning
+</br>
 
-- patch extraction of tiles and geometries, allows overlaps, for CNN's
-- machine learning utilities library: rotate images, add noise etc..
-- model for building extraction for sentinel 1 and 2
-- model for pansharpening sentinel 2
+| Example Colabs                        |                                                                                                                                                                                                               |
+|---------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Create labels from OpenStreetMap data | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/casperfibaek/buteo/blob/master/examples/create_labels_from_osm_data.ipynb)            |
+| Scheduled cleaning of geospatial data | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/casperfibaek/buteo/blob/master/examples/rocket_example.ipynb)                         |
+| Clip and remove noise from rasters    | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/casperfibaek/buteo/blob/master/examples/clip_and_remove_noise_raster.ipynb)           |
+| Sharpen nightlights data              | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/casperfibaek/buteo/blob/master/examples/process_nightlights.ipynb)                    |
+| Filters and morphological operations  | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/casperfibaek/buteo/blob/master/examples/filters_and_morphology.ipynb)                 |
 
-## extra
 
-- custom orfeo-toolbox python bindings
-- ESA snap GPT python bindings and graphs
+</br>
 
-The system is under active development and is not ready for public release. It is being developed by ESA, NIRAS, and Aalborg University.
+The toolbox is being developed by ESA-Philab, NIRAS, and Aalborg University.
 
 # Dependencies
-
 gdal
 numba
 
 optional:
 orfeo-toolbox
 esa-snap
 
-# Todo
-
-- finish filters library - kernel tests
-- update zonal statistics & parallelise vector math
-- remove dependencies: sen1mosaic
-- create models for pansharpening, buildings and noise-reduction
-- generate examples
-- synthetic sentinel 2?
-- Move deep learning / machine learning stuff in to seperate package (BUTEO & BUTEO_DL)
-- Add checks modules: raster_overlaps, all_rasters_intersect, etc...
-
-# Functions todo
-
-raster_footprints
-raster_mosaic
-raster_proximity
-raster_hydrology
-raster_vectorize
-
-vector_grid
-vector_select
-vector_buffer_etc..
-
-machine_learning_extract_sample_points
-
-python -m run_tests; python -m build_documentation;
-python -m build; python -m twine upload dist/*;
-
-python -m run_tests && python -m build_documentation
-python -m build && python -m twine upload dist/*
-
-python -m build_anaconda -forge -clean;
```

