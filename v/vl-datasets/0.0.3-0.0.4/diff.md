# Comparing `tmp/vl_datasets-0.0.3-py3.9-none-any.whl.zip` & `tmp/vl_datasets-0.0.4-py3.9-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10782 bytes, number of entries: 8
--rw-r--r--  2.0 unx      102 b- defN 23-May-08 11:34 vl_datasets/__init__.py
--rw-r--r--  2.0 unx     2351 b- defN 23-May-08 11:34 vl_datasets/filtered_dataset.py
--rw-r--r--  2.0 unx     3127 b- defN 23-May-08 11:34 vl_datasets/food101.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-08 11:34 vl_datasets-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    10118 b- defN 23-May-08 11:34 vl_datasets-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-May-08 11:34 vl_datasets-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-08 11:34 vl_datasets-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      655 b- defN 23-May-08 11:34 vl_datasets-0.0.3.dist-info/RECORD
-8 files, 27830 bytes uncompressed, 9642 bytes compressed:  65.4%
+Zip file size: 11778 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       99 b- defN 23-May-09 06:35 vl_datasets/__init__.py
+-rw-r--r--  2.0 unx     3127 b- defN 23-May-09 06:35 vl_datasets/food101.py
+-rw-r--r--  2.0 unx     2352 b- defN 23-May-09 06:35 vl_datasets/image_folder.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-09 06:35 vl_datasets-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15297 b- defN 23-May-09 06:35 vl_datasets-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-09 06:35 vl_datasets-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-09 06:35 vl_datasets-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      650 b- defN 23-May-09 06:35 vl_datasets-0.0.4.dist-info/RECORD
+8 files, 33002 bytes uncompressed, 10646 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: vl_datasets/__init__.py
 Comment: 
 
-Filename: vl_datasets/filtered_dataset.py
+Filename: vl_datasets/food101.py
 Comment: 
 
-Filename: vl_datasets/food101.py
+Filename: vl_datasets/image_folder.py
 Comment: 
 
-Filename: vl_datasets-0.0.3.dist-info/LICENSE
+Filename: vl_datasets-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: vl_datasets-0.0.3.dist-info/METADATA
+Filename: vl_datasets-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: vl_datasets-0.0.3.dist-info/WHEEL
+Filename: vl_datasets-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: vl_datasets-0.0.3.dist-info/top_level.txt
+Filename: vl_datasets-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: vl_datasets-0.0.3.dist-info/RECORD
+Filename: vl_datasets-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vl_datasets/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.0.3'
-from .filtered_dataset import FilteredDataset
+__version__ = '0.0.4'
+from .image_folder import CleanImageFolder
 from .food101 import CleanFood101
```

## Comparing `vl_datasets/filtered_dataset.py` & `vl_datasets/image_folder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from torchvision.datasets import ImageFolder
 import pandas as pd
 from pathlib import Path
 
-class FilteredDataset(ImageFolder):
+class CleanImageFolder(ImageFolder):
     """
     A modified version of torchvision.datasets.ImageFolder that filters out samples whose filenames
     are listed in a given CSV file.
 
     See: https://pytorch.org/vision/main/generated/torchvision.datasets.ImageFolder.html
 
     Args:
```

## Comparing `vl_datasets-0.0.3.dist-info/LICENSE` & `vl_datasets-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

