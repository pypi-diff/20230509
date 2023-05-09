# Comparing `tmp/med-imagetools-1.1.3.tar.gz` & `tmp/med-imagetools-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "med-imagetools-1.1.3.tar", last modified: Tue Mar 21 19:42:02 2023, max compression
+gzip compressed data, was "med-imagetools-1.1.5.tar", last modified: Tue May  9 19:17:04 2023, max compression
```

## Comparing `med-imagetools-1.1.3.tar` & `med-imagetools-1.1.5.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:42:02.233621 med-imagetools-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-03-21 19:42:02.233621 med-imagetools-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:42:02.225620 med-imagetools-1.1.3/imgtools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41500 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/autopipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:42:02.225620 med-imagetools-1.1.3/imgtools/io/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/io/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/io/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/io/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/io/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:42:02.229621 med-imagetools-1.1.3/imgtools/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27849 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/modules/datagraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/modules/dose.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/modules/pet.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/modules/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/modules/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/modules/sparsemask.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/modules/structureset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:42:02.229621 med-imagetools-1.1.3/imgtools/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22695 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/ops/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    60277 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/ops/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:42:02.229621 med-imagetools-1.1.3/imgtools/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/transforms/intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/transforms/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:42:02.229621 med-imagetools-1.1.3/imgtools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/utils/args.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/utils/arrayutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/utils/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/utils/dicomutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/utils/imageutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/imgtools/utils/nnunet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:42:02.233621 med-imagetools-1.1.3/med_imagetools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-03-21 19:42:02.000000 med-imagetools-1.1.3/med_imagetools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-21 19:42:02.000000 med-imagetools-1.1.3/med_imagetools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:42:02.000000 med-imagetools-1.1.3/med_imagetools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-21 19:42:02.000000 med-imagetools-1.1.3/med_imagetools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-21 19:42:02.000000 med-imagetools-1.1.3/med_imagetools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-21 19:42:02.000000 med-imagetools-1.1.3/med_imagetools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 19:42:02.233621 med-imagetools-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-21 19:39:31.000000 med-imagetools-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.709253 med-imagetools-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-09 19:17:04.705253 med-imagetools-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.693253 med-imagetools-1.1.5/imgtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41500 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/autopipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.693253 med-imagetools-1.1.5/imgtools/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/io/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/io/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13169 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/io/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/io/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.697253 med-imagetools-1.1.5/imgtools/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28509 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/datagraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/pet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/sparsemask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/modules/structureset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.697253 med-imagetools-1.1.5/imgtools/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22695 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/ops/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63999 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/ops/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.701253 med-imagetools-1.1.5/imgtools/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/transforms/intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/transforms/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.705253 med-imagetools-1.1.5/imgtools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/arrayutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/autopipeutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/dicomutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/imageutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/imgtools/utils/nnunet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:17:04.705253 med-imagetools-1.1.5/med_imagetools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-09 19:17:04.000000 med-imagetools-1.1.5/med_imagetools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-09 19:17:04.000000 med-imagetools-1.1.5/med_imagetools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:17:04.000000 med-imagetools-1.1.5/med_imagetools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-09 19:17:04.000000 med-imagetools-1.1.5/med_imagetools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-09 19:17:04.000000 med-imagetools-1.1.5/med_imagetools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 19:17:04.000000 med-imagetools-1.1.5/med_imagetools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:17:04.709253 med-imagetools-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-09 19:13:49.000000 med-imagetools-1.1.5/setup.py
```

### Comparing `med-imagetools-1.1.3/LICENSE` & `med-imagetools-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/PKG-INFO` & `med-imagetools-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: med-imagetools
-Version: 1.1.3
+Version: 1.1.5
 Summary: Transparent and reproducible image processing pipelines in Python.
 Home-page: https://github.com/bhklab/med-imagetools
 Author: Sejin Kim, Michal Kazmierski, Kevin Qu, Vishwesh Ramanathan, Benjamin Haibe-Kains
 Author-email: benjamin.haibe.kains@utoronto.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `med-imagetools-1.1.3/README.md` & `med-imagetools-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/autopipeline.py` & `med-imagetools-1.1.5/imgtools/autopipeline.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/image.py` & `med-imagetools-1.1.5/imgtools/image.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/io/common.py` & `med-imagetools-1.1.5/imgtools/io/common.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/io/dataset.py` & `med-imagetools-1.1.5/imgtools/io/dataset.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/io/loaders.py` & `med-imagetools-1.1.5/imgtools/io/loaders.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import os, pathlib
+import os, pathlib, json
 import glob
 import re
 from typing import Optional, List
 from collections import namedtuple
-import copy
+# import copy
 
 import pandas as pd
 import SimpleITK as sitk
 from pydicom import dcmread
 
-from joblib import Parallel, delayed
-from tqdm.auto import tqdm
+# from joblib import Parallel, delayed
+# from tqdm.auto import tqdm
 
 from ..modules import StructureSet, Dose, PET, Scan, Segmentation
 from ..utils.crawl import *
 from ..utils.dicomutils import *
 
 def read_image(path):
     return sitk.ReadImage(path)
@@ -65,16 +65,16 @@
     reader.MetaDataDictionaryArrayUpdateOn()
     reader.LoadPrivateTagsOn()
 
     return reader.Execute()
 
     
 
-def read_dicom_scan(path, series_id=None, recursive: bool=False) -> Scan:
-    image = read_dicom_series(path, series_id=series_id, recursive=recursive)
+def read_dicom_scan(path, series_id=None, recursive: bool=False, file_names=None) -> Scan:
+    image = read_dicom_series(path, series_id=series_id, recursive=recursive, file_names=file_names)
     return Scan(image, {})
 
 def read_dicom_rtstruct(path):
     return StructureSet.from_dicom_rtstruct(path)
 
 def read_dicom_rtdose(path):
     return Dose.from_dicom_rtdose(path)
@@ -82,26 +82,29 @@
 def read_dicom_pet(path, series=None):
     return PET.from_dicom_pet(path, series, "SUV")
 
 def read_dicom_seg(path, meta, series=None):
     seg_img = read_dicom_series(path, series)
     return Segmentation.from_dicom_seg(seg_img, meta)
 
-def read_dicom_auto(path, series=None):
+def read_dicom_auto(path, series=None, file_names=None):
     if path is None:
         return None
-    dcms = glob.glob(pathlib.Path(path, "*.dcm").as_posix())
+    if path.endswith(".dcm"):
+        dcms = [path]
+    else:
+        dcms = glob.glob(pathlib.Path(path, "*.dcm").as_posix())
     for dcm in dcms:
         meta = dcmread(dcm)
         if meta.SeriesInstanceUID != series and series is not None:
             continue
         
         modality = meta.Modality
         if modality in ['CT', 'MR']:
-            obj = read_dicom_scan(path, series)
+            obj = read_dicom_scan(path, series, file_names=file_names)
         elif modality == 'PT':
             obj = read_dicom_pet(path, series)
         elif modality == 'RTSTRUCT':
             obj = read_dicom_rtstruct(dcm)
         elif modality == 'RTDOSE':
             obj = read_dicom_rtdose(dcm)
         elif modality == 'SEG':
@@ -135,14 +138,85 @@
 
     def get(self, subject_id, default=None):
         try:
             return self[subject_id]
         except KeyError:
             return default
 
+class ImageTreeLoader(BaseLoader):
+    def __init__(self,
+                 json_path,
+                 csv_path_or_dataframe,
+                 col_names=[],
+                 study_names=[],
+                 series_names=[],
+                 subseries_names=[],
+                 id_column=None,
+                 expand_paths=False,
+                 readers=None):
+
+        if readers is None:
+            readers = [read_image] # no mutable defaults https://florimond.dev/en/posts/2018/08/python-mutable-defaults-are-the-source-of-all-evil/
+
+        self.expand_paths = expand_paths
+        self.readers = readers
+        self.colnames = col_names
+        self.studynames = study_names
+        self.seriesnames = series_names
+        self.subseriesnames = subseries_names
+
+        if isinstance(csv_path_or_dataframe, str):
+            if id_column is not None and id_column not in self.colnames:
+                self.colnames.append(id_column)
+            self.paths = pd.read_csv(csv_path_or_dataframe,
+                                     index_col=id_column)
+        elif isinstance(csv_path_or_dataframe, pd.DataFrame):
+            self.paths = csv_path_or_dataframe
+            if id_column:
+                self.paths = self.paths.set_index(id_column)
+            if len(self.colnames) == 0:
+                self.colnames = self.paths.columns
+        else:
+            raise ValueError(f"Expected a path to csv file or pd.DataFrame, not {type(csv_path_or_dataframe)}.")
+        
+        if isinstance(json_path, str):
+            with open(json_path, 'r') as f:
+                self.tree = json.load(json_path)
+        else:
+            raise ValueError(f"Expected a path to a json file, not {type(json_path)}.")
+
+        if not isinstance(readers, list):
+            readers = [readers] * len(self.colnames)
+
+        self.output_tuple = namedtuple("Output", self.colnames)
+
+    def __getitem__(self, subject_id):
+        row = self.paths.loc[subject_id]
+        paths = {col: row[col] for col in self.colnames}
+        study = {col: row[col] for col in self.studynames}
+        series = {col: row[col] for col in self.seriesnames}
+        subseries = {col: row[col] for col in self.subseriesnames}
+        paths = {k: v if pd.notna(v) else None for k, v in paths.items()}
+        
+        if self.expand_paths:
+            # paths = {col: glob.glob(path)[0] for col, path in paths.items()}
+            paths = {col: glob.glob(path)[0] if pd.notna(path) else None for col, path in paths.items()}
+        
+        for i, (col, path) in enumerate(paths.items()):
+            files = self.tree[subject_id][study["study_"+("_").join(col.split("_")[1:])]][series["series_"+("_").join(col.split("_")[1:])]][subseries["subseries_"+("_").join(col.split("_")[1:])]]
+            self.readers[i](path, series["series_"+("_").join(col.split("_")[1:])])
+        outputs = {col: self.readers[i](path, series["series_"+("_").join(col.split("_")[1:])], file_names=files) for i, (col, path) in enumerate(paths.items())}
+        return self.output_tuple(**outputs)
+
+    def keys(self):
+        return list(self.paths.index)
+
+    def items(self):
+        return ((k, self[k]) for k in self.keys())
+    
 class ImageCSVLoader(BaseLoader):
     def __init__(self,
                  csv_path_or_dataframe,
                  colnames=[],
                  seriesnames=[],
                  id_column=None,
                  expand_paths=False,
```

### Comparing `med-imagetools-1.1.3/imgtools/io/writers.py` & `med-imagetools-1.1.5/imgtools/io/writers.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/modules/datagraph.py` & `med-imagetools-1.1.5/imgtools/modules/datagraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,16 @@
         plan = df_study.loc[df_study["modality"] == "RTPLAN"]
         dose = df_study.loc[df_study["modality"] == "RTDOSE"]
         struct = df_study.loc[df_study["modality"] == "RTSTRUCT"]
         ct = df_study.loc[df_study["modality"] == "CT"]
         mr = df_study.loc[df_study["modality"] == "MR"]
         pet = df_study.loc[df_study["modality"] == "PT"]
         seg = df_study.loc[df_study["modality"] == "SEG"]
-        edge_types = np.arange(7)
+        edge_types = np.arange(8)
+
         for edge in edge_types:
             if edge==0:    # FORMS RTDOSE->RTSTRUCT, can be formed on both series and instance uid
                 df_comb1    = pd.merge(struct, dose, left_on="instance_uid", right_on="reference_rs")
                 df_comb2    = pd.merge(struct, dose, left_on="series", right_on="reference_rs")
                 df_combined = pd.concat([df_comb1, df_comb2])
                 #Cases where both series and instance_uid are the same for struct
                 df_combined = df_combined.drop_duplicates(subset=["instance_uid_x"])
@@ -262,23 +263,25 @@
         9) RTDOSE,RTSTRUCT,CT
         10) RTDOSE,CT,PT
         11) RTSTRUCT,CT,PT
         12) RTDOSE,RTSTRUCT,CT,PT
         '''
         #Basic processing of just one modality
         supp_mods   = ["RTDOSE", "RTSTRUCT", "CT", "PT", 'MR']
-        edge_def    = {"RTSTRUCT,RTDOSE" : 0, "CT,RTDOSE" : 1, "CT,RTSTRUCT" : 2, "PET,RTSTRUCT" : 3, "CT,PT" : 4, 'MR,RTSTRUCT': 2, "RTPLAN,RTSTRUCT": 6, "RTPLAN,RTDOSE": 5, "CT,SEG": 7}
+        edge_def    = {"RTSTRUCT,RTDOSE" : 0, "CT,RTDOSE" : 1, "CT,RTSTRUCT" : 2, "PET,RTSTRUCT" : 3, "CT,PT" : 4, 'MR,RTSTRUCT': 2, "RTPLAN,RTSTRUCT": 6, "RTPLAN,RTDOSE": 5, "CT,SEG": 7, "MR,SEG": 7, "MR,RTSTRUCT": 2}
         self.mods   = query_string.split(",")
         self.mods_n = len(self.mods)
 
         #Deals with single node queries
         if query_string in supp_mods:
-            final_df = self.df.loc[self.df.modality == query_string, ["study", "patient_ID", "series", "folder"]]
+            final_df = self.df.loc[self.df.modality == query_string, ["study", "patient_ID", "series", "folder", "subseries"]]
             final_df.rename(columns = {"series": f"series_{query_string}", 
-                                       "folder": f"folder_{query_string}"}, inplace=True)
+                                       "study": f"study_{query_string}", 
+                                       "folder": f"folder_{query_string}",
+                                       "subseries": f"subseries_{query_string}", }, inplace=True)
         
         elif self.mods_n == 2:
             #Reverse the query string
             query_string_rev = (",").join(self.mods[::-1])
             if query_string in edge_def.keys():
                 edge_type = edge_def[query_string]
                 valid = query_string
@@ -301,23 +304,29 @@
                     regex_term = '((?=.*1)|(((?=.*0)|(?=.*5)(?=.*6))(?=.*2)))'
                     final_df = self.graph_query(regex_term, edge_list, "RTSTRUCT")
                 elif edge_type==2:
                     #Search for subgraphs with edges 2 or (1 and 0)
                     regex_term = '((?=.*2)|(((?=.*0)|(?=.*5)(?=.*6))(?=.*1)))'
                     final_df = self.graph_query(regex_term, edge_list, "RTDOSE") 
             else:
-                final_df = self.df_edges.loc[self.df_edges.edge_type == edge_type, ["study_x","patient_ID_x","series_x","folder_x","series_y","folder_y"]]
+                final_df = self.df_edges.loc[self.df_edges.edge_type == edge_type, ["study_x","patient_ID_x", "study_x", "study_y", "series_x","folder_x","series_y","folder_y", "subseries_x", "subseries_y"]]
                 node_dest = valid.split(",")[0]
                 node_origin = valid.split(",")[1]
                 final_df.rename(columns={"study_x": "study", 
                                          "patient_ID_x": "patient_ID",
                                          "series_x": f"series_{node_dest}", 
                                          "series_y": f"series_{node_origin}", 
+                                         
+                                         "study_x": f"study_{node_dest}", 
+                                         "study_y": f"study_{node_origin}", 
                                          "folder_x": f"folder_{node_dest}", 
-                                         "folder_y": f"folder_{node_origin}"}, inplace=True)
+                                         "folder_y": f"folder_{node_origin}",
+                                         
+                                         "subseries_x": f"subseries_{node_dest}", 
+                                         "subseries_y": f"subseries_{node_origin}", }, inplace=True)
 
         elif self.mods_n > 2:
             #Processing of combinations of modality
             bads = ["RTPLAN"]
             # CT/MR,RTSTRUCT,RTDOSE
             if (("CT" in query_string) or ('MR' in query_string)) & ("RTSTRUCT" in query_string) & ("RTDOSE" in query_string) & ("PT" not in query_string):
                 #Fetch the required data. Checks whether each study has edge 2 and (1 or 0)
```

### Comparing `med-imagetools-1.1.3/imgtools/modules/dose.py` & `med-imagetools-1.1.5/imgtools/modules/dose.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/modules/pet.py` & `med-imagetools-1.1.5/imgtools/modules/pet.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/modules/segmentation.py` & `med-imagetools-1.1.5/imgtools/modules/segmentation.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/modules/structureset.py` & `med-imagetools-1.1.5/imgtools/modules/structureset.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,32 +102,30 @@
     def get_mask(self, reference_image, mask, label, idx, continuous):
         size = reference_image.GetSize()[::-1]
         physical_points = self.roi_points.get(label, np.array([]))
         mask_points = physical_points_to_idxs(reference_image, physical_points, continuous=continuous)
         for contour in mask_points:
             try:
                 z, slice_points = np.unique(contour[:, 0]), contour[:, 1:]
-                if len(z) == 1:
-                    #f assert len(z) == 1, f"This contour ({name}) spreads across more than 1 slice."
-                    z = z[0]
+                if len(z) == 1: # assert len(z) == 1, f"This contour ({name}) spreads across more than 1 slice."
                     slice_mask = polygon2mask(size[1:], slice_points)
-                    mask[z, :, :, idx] += slice_mask
+                    mask[z[0], :, :, idx] += slice_mask
             except: # rounding errors for points on the boundary
                 if z == mask.shape[0]:
                     z -= 1
-                elif z == -1:
+                elif z == -1: #?
                     z += 1
                 elif z > mask.shape[0] or z < -1:
                     raise IndexError(f"{z} index is out of bounds for image sized {mask.shape}.")
                 
                 # if the contour spans only 1 z-slice 
                 if len(z) == 1:
-                    z = int(np.floor(z[0]))
+                    z_idx = int(np.floor(z[0]))
                     slice_mask = polygon2mask(size[1:], slice_points)
-                    mask[z, :, :, label] += slice_mask
+                    mask[z_idx, :, :, idx] += slice_mask
                 else:
                     raise ValueError("This contour is corrupted and spans across 2 or more slices.")
 
     def to_segmentation(self, reference_image: sitk.Image,
                         roi_names: Dict[str, str] = None,
                         continuous: bool = True,
                         existing_roi_indices: Dict[str, int] = None,
```

### Comparing `med-imagetools-1.1.3/imgtools/ops/functional.py` & `med-imagetools-1.1.5/imgtools/ops/functional.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/ops/ops.py` & `med-imagetools-1.1.5/imgtools/ops/ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, TypeVar, Sequence, Union, Tuple, Optional, Any
 
 import numpy as np
 import SimpleITK as sitk
 
 from .functional import *
 from ..io import *
-from ..utils import image_to_array, array_to_image, crawl
+from ..utils import image_to_array, array_to_image, crawl, physical_points_to_idxs
 from ..modules import map_over_labels
 from ..modules import DataGraph
 
 
 LoaderFunction = TypeVar('LoaderFunction')
 ImageFilter = TypeVar('ImageFilter')
 Function = TypeVar('Function')
@@ -51,14 +51,85 @@
                 f"writer must be a subclass of io.BaseWriter, got {type(writer)}"
             )
         self._writer = writer
 
     def __call__(self, key, *args, **kwargs):
         self._writer.put(key, *args, **kwargs)
 
+class BetaAutoInput(BaseInput):
+    """ImageAutoInput class is a wrapper class around ImgCSVloader which looks for the specified directory and crawls through it as the first step. Using the crawled output data, a graph on modalties present in the dataset is formed
+    which stores the relation between all the modalities.
+    Based on the user provided modalities, this class loads the information of the user provided modalities
+
+    Parameters
+    ----------
+    dir_path: str
+        Path to dataset top-level directory. The crawler/indexer will start at this directory.
+
+    modalities: str
+        List of modalities to process. Only samples with ALL modalities will be processed. Make sure there are no space between list elements as it is parsed as a string.
+
+    visualize: bool
+        Whether to return visualization of the data graph
+
+    update: bool
+        Whether to update crawled index
+    """
+    def __init__(self,
+                 dir_path: str,
+                 modalities: str,
+                 n_jobs: int = -1,
+                 visualize: bool = False,
+                 update: bool = False):
+        self.dir_path = dir_path
+        self.modalities = modalities
+        self.parent, self.dataset_name = os.path.split(self.dir_path)
+
+        ####### CRAWLER ############
+        # Checks if dataset has already been indexed
+        # To be changed later
+        df_crawl_path   = pathlib.Path(self.parent, ".imgtools", f"imgtools_{self.dataset_name}.csv").as_posix()
+        tree_crawl_path = pathlib.Path(self.parent, ".imgtools", f"imgtools_{self.dataset_name}.json").as_posix()
+
+        if not os.path.exists(df_crawl_path) or update:
+            print("Indexing the dataset...")
+            db = crawl(self.dir_path, n_jobs=n_jobs)
+            print(f"Number of patients in the dataset: {len(db)}")
+        else:
+            print("The dataset has already been indexed.")
+
+        import json
+        with open(tree_crawl_path, 'r') as f:
+            tree_db = json.load(f)
+
+        ####### GRAPH ##########
+        # Form the graph
+        edge_path = pathlib.Path(self.parent,".imgtools",f"imgtools_{self.dataset_name}_edges.csv").as_posix()
+        graph = DataGraph(path_crawl=df_crawl_path, edge_path=edge_path, visualize=visualize)
+        print(f"Forming the graph based on the given modalities: {self.modalities}")
+        self.df_combined = graph.parser(self.modalities)
+        self.output_streams = [("_").join(cols.split("_")[1:]) for cols in self.df_combined.columns if cols.split("_")[0] == "folder"]
+        self.column_names = [cols for cols in self.df_combined.columns if cols.split("_")[0] == "folder"]
+        self.study_names  = [cols for cols in self.df_combined.columns if cols.split("_")[0] == "study"]
+        self.series_names = [cols for cols in self.df_combined.columns if cols.split("_")[0] == "series"]
+        self.subseries_names = [cols for cols in self.df_combined.columns if cols.split("_")[0] == "subseries"]
+        print(f"There are {len(self.df_combined)} cases containing all {modalities} modalities.")
+
+        self.readers = [read_dicom_auto for _ in range(len(self.output_streams))]
+
+        loader = ImageCSVLoader(self.df_combined,
+                                col_names=self.column_names,
+                                study_names=self.study_names,
+                                series_names=self.series_names,
+                                subseries_names=self.subseries_names,
+                                id_column=None,
+                                expand_paths=False,
+                                readers=self.readers)
+        
+        super().__init__(loader)
 
 class ImageAutoInput(BaseInput):
     """ImageAutoInput class is a wrapper class around ImgCSVloader which looks for the specified directory and crawls through it as the first step. Using the crawled output data, a graph on modalties present in the dataset is formed
     which stores the relation between all the modalities.
     Based on the user provided modalities, this class loads the information of the user provided modalities
 
     Parameters
@@ -1614,14 +1685,16 @@
             Image used as reference geometry.
 
         Returns
         -------
         Segmentation
             The segmentation object.
         """
+        from itertools import groupby
+
         # variable name isn't ideal, but follows StructureSet.to_segmentation convention
         self.roi_names    = seg.raw_roi_names 
         labels = {}
         
         # `roi_names` in .to_segmentation() method = self.roi_patterns
         if self.roi_patterns is None or self.roi_patterns == {}:
             self.roi_patterns = self.roi_names
```

### Comparing `med-imagetools-1.1.3/imgtools/pipeline.py` & `med-imagetools-1.1.5/imgtools/pipeline.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/transforms/spatial.py` & `med-imagetools-1.1.5/imgtools/transforms/spatial.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/utils/args.py` & `med-imagetools-1.1.5/imgtools/utils/args.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/utils/arrayutils.py` & `med-imagetools-1.1.5/imgtools/utils/arrayutils.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/utils/crawl.py` & `med-imagetools-1.1.5/imgtools/utils/crawl.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,34 @@
 import pandas as pd
 from pydicom import dcmread
 from tqdm import tqdm
 
 from joblib import Parallel, delayed
 
 def crawl_one(folder):
+    folder_path = pathlib.Path(folder)
     database = {}
     for path, _, _ in os.walk(folder):
         # find dicoms
-        dicoms = glob.glob(pathlib.Path(path, "*.dcm").as_posix())
-
+        dicoms = glob.glob(pathlib.Path(path, "**", "*.dcm").as_posix(), recursive=True)
+        # print('\n', folder, dicoms)
         # instance (slice) information
         for dcm in dicoms:
             try:
-                fname    = pathlib.Path(dcm).name
-                meta     = dcmread(dcm, force=True)
-                patient  = str(meta.PatientID)
-                study    = str(meta.StudyInstanceUID)
-                series   = str(meta.SeriesInstanceUID)
-                instance = str(meta.SOPInstanceUID)
+                dcm_path  = pathlib.Path(dcm)
+                # parent    = dcm_path.parent#.as_posix()
+                fname     = dcm_path.name
+                rel_path  = dcm_path.relative_to(folder_path.parent.parent)                                        # rel_path of dicom from folder
+                rel_posix = rel_path.parent.as_posix()     # folder name + until parent folder of dicom
+
+                meta      = dcmread(dcm, force=True)
+                patient   = str(meta.PatientID)
+                study     = str(meta.StudyInstanceUID)
+                series    = str(meta.SeriesInstanceUID)
+                instance  = str(meta.SOPInstanceUID)
 
                 reference_ct, reference_rs, reference_pl,  = "", "", ""
                 tr, te, tesla, scan_seq, elem = "", "", "", "", ""
                 try:
                     orientation = str(meta.ImageOrientationPatient) # (0020, 0037)
                 except:
                     orientation = ""
@@ -106,37 +112,40 @@
                     
 
                 if patient not in database:
                     database[patient] = {}
                 if study not in database[patient]:
                     database[patient][study] = {'description': study_description}
                 if series not in database[patient][study]:
-                    parent, _ = os.path.split(folder)
-                    rel_path = pathlib.Path(os.path.split(parent)[1], os.path.relpath(path, parent)).as_posix()
+                    rel_crawl_path  = rel_posix
+                    if meta.Modality == 'RTSTRUCT':
+                        rel_crawl_path = os.path.join(rel_crawl_path, fname)
+                    
                     database[patient][study][series] = {'description': series_description}
                 if subseries not in database[patient][study][series]:
                     database[patient][study][series][subseries] = {'instances': {},
                                                                    'instance_uid': instance,
                                                                    'modality': meta.Modality,
                                                                    'reference_ct': reference_ct,
                                                                    'reference_rs': reference_rs,
                                                                    'reference_pl': reference_pl,
                                                                    'reference_frame': reference_frame,
-                                                                   'folder': rel_path,
+                                                                   'folder': rel_crawl_path,
                                                                    'orientation': orientation,
                                                                    'orientation_type': orientation_type,
                                                                    'repetition_time':tr,
                                                                    'echo_time':te,
                                                                    'scan_sequence': scan_seq,
                                                                    'mag_field_strength': tesla,
-                                                                   'imaged_nucleus': elem
+                                                                   'imaged_nucleus': elem,
+                                                                   'fname': rel_path.as_posix() #temporary until we switch to json-based loading
                                                                    }
-
-                database[patient][study][series][subseries]['instances'][instance] = fname
-            except:
+                database[patient][study][series][subseries]['instances'][instance] = rel_path.as_posix()
+            except Exception as e:
+                print(folder, e)
                 pass
     
     return database
 
 def to_df(database_dict):
     df = pd.DataFrame()
     for pat in database_dict:
@@ -146,24 +155,25 @@
                     for subseries in database_dict[pat][study][series]:
                         if subseries != 'description': # skip description key in dict
                             columns = ['patient_ID', 'study', 'study_description', 
                                        'series', 'series_description', 'subseries', 'modality', 
                                        'instances', 'instance_uid', 
                                        'reference_ct', 'reference_rs', 'reference_pl', 'reference_frame', 'folder',
                                        'orientation', 'orientation_type', 'MR_repetition_time', 'MR_echo_time', 
-                                       'MR_scan_sequence', 'MR_magnetic_field_strength', 'MR_imaged_nucleus']
+                                       'MR_scan_sequence', 'MR_magnetic_field_strength', 'MR_imaged_nucleus', 'file_path']
                             values = [pat, study, database_dict[pat][study]['description'], 
                                       series, database_dict[pat][study][series]['description'], 
                                       subseries, database_dict[pat][study][series][subseries]['modality'], 
                                       len(database_dict[pat][study][series][subseries]['instances']), database_dict[pat][study][series][subseries]['instance_uid'], 
                                       database_dict[pat][study][series][subseries]['reference_ct'], database_dict[pat][study][series][subseries]['reference_rs'], 
                                       database_dict[pat][study][series][subseries]['reference_pl'], database_dict[pat][study][series][subseries]['reference_frame'], database_dict[pat][study][series][subseries]['folder'],
                                       database_dict[pat][study][series][subseries]['orientation'], database_dict[pat][study][series][subseries]['orientation_type'],
                                       database_dict[pat][study][series][subseries]['repetition_time'], database_dict[pat][study][series][subseries]['echo_time'],
                                       database_dict[pat][study][series][subseries]['scan_sequence'], database_dict[pat][study][series][subseries]['mag_field_strength'], database_dict[pat][study][series][subseries]['imaged_nucleus'],
+                                      database_dict[pat][study][series][subseries]['fname']
                                       ]
 
                             df_add = pd.DataFrame([values], columns=columns)
                             df = pd.concat([df, df_add], ignore_index=True)
     return df
 
 def crawl(top,
```

### Comparing `med-imagetools-1.1.3/imgtools/utils/dicomutils.py` & `med-imagetools-1.1.5/imgtools/utils/dicomutils.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/utils/imageutils.py` & `med-imagetools-1.1.5/imgtools/utils/imageutils.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/imgtools/utils/nnunet.py` & `med-imagetools-1.1.5/imgtools/utils/nnunet.py`

 * *Files identical despite different names*

### Comparing `med-imagetools-1.1.3/med_imagetools.egg-info/PKG-INFO` & `med-imagetools-1.1.5/med_imagetools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: med-imagetools
-Version: 1.1.3
+Version: 1.1.5
 Summary: Transparent and reproducible image processing pipelines in Python.
 Home-page: https://github.com/bhklab/med-imagetools
 Author: Sejin Kim, Michal Kazmierski, Kevin Qu, Vishwesh Ramanathan, Benjamin Haibe-Kains
 Author-email: benjamin.haibe.kains@utoronto.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `med-imagetools-1.1.3/med_imagetools.egg-info/SOURCES.txt` & `med-imagetools-1.1.5/med_imagetools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 imgtools/ops/ops.py
 imgtools/transforms/__init__.py
 imgtools/transforms/intensity.py
 imgtools/transforms/spatial.py
 imgtools/utils/__init__.py
 imgtools/utils/args.py
 imgtools/utils/arrayutils.py
+imgtools/utils/autopipeutils.py
 imgtools/utils/crawl.py
 imgtools/utils/dicomutils.py
 imgtools/utils/imageutils.py
 imgtools/utils/nnunet.py
 med_imagetools.egg-info/PKG-INFO
 med_imagetools.egg-info/SOURCES.txt
 med_imagetools.egg-info/dependency_links.txt
```

### Comparing `med-imagetools-1.1.3/setup.py` & `med-imagetools-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     reqs = fh.read()
     
 setup(
     name="med-imagetools",
-    version="1.1.3",
+    version="1.1.5",
     author="Sejin Kim, Michal Kazmierski, Kevin Qu, Vishwesh Ramanathan, Benjamin Haibe-Kains",
     author_email="benjamin.haibe.kains@utoronto.ca",
     description="Transparent and reproducible image processing pipelines in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bhklab/med-imagetools",
     install_requires=reqs,
```

