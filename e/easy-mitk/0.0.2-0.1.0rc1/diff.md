# Comparing `tmp/easy_mitk-0.0.2.tar.gz` & `tmp/easy_mitk-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/app/sdk/easy-mitk/dist/.tmp-l1rfdq5k/easy_mitk-0.0.2.tar", last modified: Sat May  6 16:01:00 2023, max compression
+gzip compressed data, was "/app/sdk/easy-mitk/dist/.tmp-sh7h_5z8/easy_mitk-0.1.0rc1.tar", last modified: Tue May  9 13:55:29 2023, max compression
```

## Comparing `easy_mitk-0.0.2.tar` & `easy_mitk-0.1.0rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1066 2023-05-03 11:31:57.000000 easy_mitk-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      450 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       94 2023-05-06 15:55:55.000000 easy_mitk-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk/
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-03 11:32:27.000000 easy_mitk-0.0.2/easy_mitk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22752 2023-05-06 15:51:39.000000 easy_mitk-0.0.2/easy_mitk/dicom.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-05-06 15:18:42.000000 easy_mitk-0.0.2/easy_mitk/measure.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-06 15:52:33.000000 easy_mitk-0.0.2/easy_mitk/nifti.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 11:32:27.000000 easy_mitk-0.0.2/easy_mitk/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1308 2023-05-06 15:54:22.000000 easy_mitk-0.0.2/easy_mitk/utils/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      450 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-03 11:32:27.000000 easy_mitk-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      739 2023-05-06 15:59:15.000000 easy_mitk-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/tests/
--rw-r--r--   0 root         (0) root         (0)     2893 2023-05-03 11:33:31.000000 easy_mitk-0.0.2/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)      536 2023-05-03 15:28:18.000000 easy_mitk-0.0.2/tests/test_measure.py
--rw-r--r--   0 root         (0) root         (0)      193 2023-05-03 11:32:28.000000 easy_mitk-0.0.2/tests/test_torch_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:55:29.000000 easy_mitk-0.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-05-03 11:31:57.000000 easy_mitk-0.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      599 2023-05-09 13:55:29.000000 easy_mitk-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-09 13:52:17.000000 easy_mitk-0.1.0rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:55:29.000000 easy_mitk-0.1.0rc1/easy_mitk/
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-03 11:32:27.000000 easy_mitk-0.1.0rc1/easy_mitk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24732 2023-05-07 13:19:50.000000 easy_mitk-0.1.0rc1/easy_mitk/dicom.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-05-06 15:18:42.000000 easy_mitk-0.1.0rc1/easy_mitk/measure.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-06 15:52:33.000000 easy_mitk-0.1.0rc1/easy_mitk/nifti.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:55:29.000000 easy_mitk-0.1.0rc1/easy_mitk/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 11:32:27.000000 easy_mitk-0.1.0rc1/easy_mitk/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-05-06 15:54:22.000000 easy_mitk-0.1.0rc1/easy_mitk/utils/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:55:29.000000 easy_mitk-0.1.0rc1/easy_mitk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      599 2023-05-09 13:55:29.000000 easy_mitk-0.1.0rc1/easy_mitk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-09 13:55:29.000000 easy_mitk-0.1.0rc1/easy_mitk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 13:55:29.000000 easy_mitk-0.1.0rc1/easy_mitk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-09 13:55:29.000000 easy_mitk-0.1.0rc1/easy_mitk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-09 13:55:29.000000 easy_mitk-0.1.0rc1/easy_mitk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-03 11:32:27.000000 easy_mitk-0.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 13:55:29.000000 easy_mitk-0.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-07 10:34:16.000000 easy_mitk-0.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:55:29.000000 easy_mitk-0.1.0rc1/tests/
+-rw-r--r--   0 root         (0) root         (0)     3420 2023-05-07 12:06:20.000000 easy_mitk-0.1.0rc1/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-05-03 15:28:18.000000 easy_mitk-0.1.0rc1/tests/test_measure.py
+-rw-r--r--   0 root         (0) root         (0)      193 2023-05-03 11:32:28.000000 easy_mitk-0.1.0rc1/tests/test_torch_model.py
```

### Comparing `easy_mitk-0.0.2/LICENSE` & `easy_mitk-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_mitk-0.0.2/easy_mitk/dicom.py` & `easy_mitk-0.1.0rc1/easy_mitk/dicom.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 """
 import os
 from datetime import datetime
 from glob import glob
-from typing import List, Tuple
+from typing import Dict, List, Tuple
 
 import dicom2nifti
 import nibabel as nib
 import numpy as np
 import pydicom
 from nibabel import nifti1
-from pydicom import Dataset, Sequence, dataset, uid
+from pydicom import Dataset, Sequence, dataset, uid, errors
 from rle import encode_pixel_data
 
 
 def get_slice_location(dcm: Dataset) -> float:
     """
     Get stack position from the SliceLocation.
     :param dcm: DICOM Dataset
@@ -155,15 +155,15 @@
 
     Returns:
         np.ndarray: _description_
     """
     arr = []
     for d in dcms:
         # arr.append(np.rot90(d.pixel_array, 1, [0, 1]))
-        arr.append(d.pixel_array)
+        arr.append(d.pixel_array * d.RescaleSlope + d.RescaleIntercept)
     return np.stack(arr, axis=-1)
 
 
 def load_as_arr1(dcm_dir: os.PathLike) -> np.ndarray:
     """
     Same with load_as_arr but parameters.
     除了参数，其它与load_as_arr一样。
@@ -576,8 +576,66 @@
     assert origin_dcm[0].SeriesInstanceUID == referenced_series_uid
     affine, _ = get_affine(origin_dcm, load_pixel_arr=False)
 
     nii = nifti1.Nifti1Image(arr, affine)
     if save_path:
         os.makedirs(os.path.dirname(save_path), exist_ok=True)
         nib.save(nii, save_path)
-    return nii
+    return nii
+
+
+ANONYMOUS_TAGS = {
+    "InstitutionName": "", 
+    "InstitutionAddress": "",
+    "ReferringPhysicianName": "",
+    "PatientName": "", 
+    "OtherPatientNames": "", 
+    "RequestingService": "",
+    "StationName": ""
+    }
+
+def anonymous(dcms: List[Dataset], anonymous_tags: Dict=ANONYMOUS_TAGS):
+    """
+    tag: 
+    """    
+    for d in dcms:
+        for k, v in anonymous_tags.items():
+            try:
+                e = getattr(d, k)
+                if isinstance(e, pydicom.DataElement):
+                    e: pydicom.DataElement
+                    e.value = v
+                else:
+                    setattr(d, k, v)
+            except AttributeError:
+                continue
+            except Exception as e:
+                print(f'failed to set {k} to {v}')
+                raise e
+
+
+def save_to_disk(dcms: List[Dataset], target_dir: os.PathLike):
+    os.makedirs(target_dir, exist_ok=True)
+    for i in range(len(dcms)):
+        full_path = os.path.join(target_dir, f'{i}.dcm')
+        pydicom.dcmwrite(full_path, dcms[i])
+
+def anonymous_dir(source_dir: os.PathLike, target_dir: os.PathLike, anonymous_tags: Dict=ANONYMOUS_TAGS):
+    assert not str(source_dir).startswith('/'), 'source_dir needs to be a relative path'
+    assert os.path.exists(source_dir)
+    p = f'{source_dir}/.?*/?*'
+    # print(p)
+    for root, _, filenames in os.walk(source_dir):
+        for i in filenames:
+           full_path = os.path.join(root, i)
+           print(f'Dealing with: {full_path}')
+           try:
+               dcm = pydicom.dcmread(full_path)
+           except errors.InvalidDicomError:
+               # TODO 添加日志文件
+               continue
+           anonymous([dcm], anonymous_tags)
+           target_path = os.path.join(target_dir, full_path)
+           os.makedirs(os.path.dirname(target_path), exist_ok=True)
+           pydicom.dcmwrite(target_path, dcm)
+    # for i in files:
+    #     print(i)
```

### Comparing `easy_mitk-0.0.2/easy_mitk/measure.py` & `easy_mitk-0.1.0rc1/easy_mitk/measure.py`

 * *Files identical despite different names*

### Comparing `easy_mitk-0.0.2/easy_mitk/nifti.py` & `easy_mitk-0.1.0rc1/easy_mitk/nifti.py`

 * *Files identical despite different names*

### Comparing `easy_mitk-0.0.2/easy_mitk/utils/helper.py` & `easy_mitk-0.1.0rc1/easy_mitk/utils/helper.py`

 * *Files identical despite different names*

### Comparing `easy_mitk-0.0.2/setup.py` & `easy_mitk-0.1.0rc1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="easy_mitk",
-    version="0.0.2",
+    version="0.1.0-rc.1",
     author="Daryl.Xu",
     author_email="ziqiang_xu@qq.com",
     description="An easy-to-use Medical Imaging ToolKit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/daryl6/easy-mitk",
     packages=setuptools.find_packages(),
```

### Comparing `easy_mitk-0.0.2/tests/test_dicom.py` & `easy_mitk-0.1.0rc1/tests/test_dicom.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,13 +76,27 @@
 
     origin_img = dicom.load_series(Path.DICOM_CASE1)
     seg = pydicom.dcmread(Path.DICOM_CASE1_SEG)
     nii = dicom.seg2nii(seg, origin_img, save_path=os.path.join(target_dir, 'label.nii.gz'))
     print(nii.affine)
 
 
+def test_anonymous():
+    target_dir = get_test_tmp_dir(Path.DICOM_CASE1, 'anonymous')
+    dcms = dicom.load_series(Path.DICOM_CASE1)
+    dicom.anonymous(dcms)
+    dicom.save_to_disk(dcms, target_dir)
+
+def test_anonymous_dir():
+    # dicom.anonymous_dir('test-data/dicom', 'test-data/dicom-anonymous')
+    # dicom.anonymous_dir('tmp/quanjing_ct', '/app/sdk/easy-mitk/tmp/quanjing_ct-anonymous')
+    dicom.anonymous_dir('tmp/quanjing-mask', 'tmp/quanjing-mask-anonymous')
+
+
 if __name__ == '__main__':
     dir = os.path.dirname(__file__)
     os.chdir(os.path.join(dir, '..'))
-
-    test_seg2nii()
+    
+    test_anonymous_dir()
+    # test_anonymous()
+    # test_seg2nii()
     # test_dcm2nii2()
```

### Comparing `easy_mitk-0.0.2/tests/test_measure.py` & `easy_mitk-0.1.0rc1/tests/test_measure.py`

 * *Files identical despite different names*

