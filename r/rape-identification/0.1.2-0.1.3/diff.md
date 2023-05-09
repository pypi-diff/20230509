# Comparing `tmp/rape_identification-0.1.2.tar.gz` & `tmp/rape_identification-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rape_identification-0.1.2.tar", last modified: Tue May  9 10:55:55 2023, max compression
+gzip compressed data, was "rape_identification-0.1.3.tar", last modified: Tue May  9 11:07:10 2023, max compression
```

## Comparing `rape_identification-0.1.2.tar` & `rape_identification-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:55:55.790207 rape_identification-0.1.2/
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 10:55:55.790207 rape_identification-0.1.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:55:55.790207 rape_identification-0.1.2/rape_identification/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:55:55.790207 rape_identification-0.1.2/rape_identification/config/
--rw-rw-r--   0 root         (0) root         (0)      454 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2428 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/config/default.py
--rw-rw-r--   0 root         (0) root         (0)     1895 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/config/default_test.py
--rw-rw-r--   0 root         (0) root         (0)      706 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/inference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:55:55.790207 rape_identification-0.1.2/rape_identification/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 10:54:56.000000 rape_identification-0.1.2/rape_identification/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2764 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/utils/convert2uint8.py
--rw-rw-r--   0 root         (0) root         (0)      866 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/utils/segment.py
--rw-rw-r--   0 root         (0) root         (0)     4089 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/utils/test.py
--rw-rw-r--   0 root         (0) root         (0)    13774 2023-05-09 09:48:54.000000 rape_identification-0.1.2/rape_identification/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:55:55.790207 rape_identification-0.1.2/rape_identification.egg-info/
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 10:55:55.000000 rape_identification-0.1.2/rape_identification.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-09 10:55:55.000000 rape_identification-0.1.2/rape_identification.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 10:55:55.000000 rape_identification-0.1.2/rape_identification.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-09 10:55:55.000000 rape_identification-0.1.2/rape_identification.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-09 10:55:55.000000 rape_identification-0.1.2/rape_identification.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 10:55:55.790207 rape_identification-0.1.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      937 2023-05-09 10:55:40.000000 rape_identification-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:07:10.277359 rape_identification-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 11:07:10.277359 rape_identification-0.1.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:07:10.277359 rape_identification-0.1.3/rape_identification/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.3/rape_identification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:07:10.277359 rape_identification-0.1.3/rape_identification/config/
+-rw-rw-r--   0 root         (0) root         (0)      454 2023-05-09 09:48:54.000000 rape_identification-0.1.3/rape_identification/config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2428 2023-05-09 09:48:54.000000 rape_identification-0.1.3/rape_identification/config/default.py
+-rw-rw-r--   0 root         (0) root         (0)     1895 2023-05-09 09:48:54.000000 rape_identification-0.1.3/rape_identification/config/default_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:07:10.277359 rape_identification-0.1.3/rape_identification/dataset/
+-rw-rw-r--   0 root         (0) root         (0)     1989 2023-05-09 09:48:54.000000 rape_identification-0.1.3/rape_identification/dataset/SlidingWindowDataset.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:44.000000 rape_identification-0.1.3/rape_identification/dataset/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      706 2023-05-09 09:48:54.000000 rape_identification-0.1.3/rape_identification/inference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:07:10.277359 rape_identification-0.1.3/rape_identification/model/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:07:10.277359 rape_identification-0.1.3/rape_identification/model/SwinUNet/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:40.000000 rape_identification-0.1.3/rape_identification/model/SwinUNet/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    31715 2023-05-09 09:48:54.000000 rape_identification-0.1.3/rape_identification/model/SwinUNet/swin_transformer_unet_skip_expand_decoder_sys.py
+-rw-rw-r--   0 root         (0) root         (0)     4177 2023-05-09 09:48:54.000000 rape_identification-0.1.3/rape_identification/model/SwinUNet/vision_transformer.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:35.000000 rape_identification-0.1.3/rape_identification/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:07:10.277359 rape_identification-0.1.3/rape_identification/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 10:54:56.000000 rape_identification-0.1.3/rape_identification/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2764 2023-05-09 09:48:54.000000 rape_identification-0.1.3/rape_identification/utils/convert2uint8.py
+-rw-rw-r--   0 root         (0) root         (0)      870 2023-05-09 11:04:50.000000 rape_identification-0.1.3/rape_identification/utils/segment.py
+-rw-rw-r--   0 root         (0) root         (0)     4092 2023-05-09 11:04:31.000000 rape_identification-0.1.3/rape_identification/utils/test.py
+-rw-rw-r--   0 root         (0) root         (0)    13778 2023-05-09 11:04:06.000000 rape_identification-0.1.3/rape_identification/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:07:10.277359 rape_identification-0.1.3/rape_identification.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 11:07:10.000000 rape_identification-0.1.3/rape_identification.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      922 2023-05-09 11:07:10.000000 rape_identification-0.1.3/rape_identification.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 11:07:10.000000 rape_identification-0.1.3/rape_identification.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-09 11:07:10.000000 rape_identification-0.1.3/rape_identification.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-09 11:07:10.000000 rape_identification-0.1.3/rape_identification.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 11:07:10.277359 rape_identification-0.1.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      937 2023-05-09 11:06:49.000000 rape_identification-0.1.3/setup.py
```

### Comparing `rape_identification-0.1.2/PKG-INFO` & `rape_identification-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rape_identification
-Version: 0.1.2
+Version: 0.1.3
 Summary: Segmentation any rape
 Author: PingYang
 Author-email: PingYang97@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rape_identification-0.1.2/rape_identification/config/default.py` & `rape_identification-0.1.3/rape_identification/config/default.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.2/rape_identification/config/default_test.py` & `rape_identification-0.1.3/rape_identification/config/default_test.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.2/rape_identification/inference.py` & `rape_identification-0.1.3/rape_identification/inference.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.2/rape_identification/utils/convert2uint8.py` & `rape_identification-0.1.3/rape_identification/utils/convert2uint8.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.2/rape_identification/utils/segment.py` & `rape_identification-0.1.3/rape_identification/utils/segment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import torch
 import os
 import warnings
 import torch.nn as nn
 import torch.backends.cudnn as cudnn
 from osgeo import gdal
 
-from utils.utils import Creat_model
-from utils.test import process_all_images_in_folder
-from config.default_test import _C as cfg
+from .utils.utils import Creat_model
+from .utils.test import process_all_images_in_folder
+from ..config.default_test import _C as cfg
 
 
 def segment_any_rape(args):
     os.environ['CPL_DEBUG'] = 'OFF'
     os.environ['CPL_LOG'] = '/dev/null'
     warnings.filterwarnings('ignore', category=UserWarning, module='torch')
```

### Comparing `rape_identification-0.1.2/rape_identification/utils/test.py` & `rape_identification-0.1.3/rape_identification/utils/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import torch
 import numpy as np
 import torch.nn.functional as F
 from tqdm import tqdm
 from torch.cuda.amp import autocast
 from torch.utils.data import DataLoader
 
-from utils.convert2uint8 import convert2uint8, save2tif
-from dataset.SlidingWindowDataset import SlidingWindowDataset
+from .utils.convert2uint8 import convert2uint8, save2tif
+from ..dataset.SlidingWindowDataset import SlidingWindowDataset
 
 
 def test_large_image(model, img_path, output_path, num_classes, num_workers, window_size=224, stride=64, batch_size=100, threshold=0.5):
     # Load the large image and create the dataset and dataloader
     array, ds, transform = convert2uint8(img_path)
     dataset = SlidingWindowDataset(img_array=array, window_size=window_size, stride=stride)
     dataloader = DataLoader(dataset,
```

### Comparing `rape_identification-0.1.2/rape_identification/utils/utils.py` & `rape_identification-0.1.3/rape_identification/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
             return UNet(self.cfg.IN_CHANNEL, self.cfg.NUM_CLASSES)
 
         elif self.cfg.NAME == 'FCN':
             from model.FCN_8s.FCN_ResNet import FCN_ResNet
             return FCN_ResNet(self.cfg.NUM_CLASSES)
 
         elif self.cfg.NAME == 'SwinUNet':
-            from model.SwinUNet.vision_transformer import SwinUnet as ViT_seg
-            from config.default import get_cfg
+            from ..model.SwinUNet.vision_transformer import SwinUnet as ViT_seg
+            from ..config.default import get_cfg
             model_config = get_cfg('config/GID.yaml')
             return ViT_seg(model_config)
 
 
 class SegmentationMetric(object):
     def __init__(self, numClass):
         self.numClass = numClass
```

### Comparing `rape_identification-0.1.2/rape_identification.egg-info/PKG-INFO` & `rape_identification-0.1.3/rape_identification.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rape-identification
-Version: 0.1.2
+Version: 0.1.3
 Summary: Segmentation any rape
 Author: PingYang
 Author-email: PingYang97@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rape_identification-0.1.2/setup.py` & `rape_identification-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rape_identification',  # 与项目文件夹结构中的包名相同
-    version='0.1.2',
+    version='0.1.3',
     description='Segmentation any rape',
     author='PingYang',
     author_email='PingYang97@163.com',
     # url='https://github.com/yourusername/your_project',
     packages=find_packages(),
     install_requires=[
         # Add your project's dependencies here, e.g., 'numpy', 'pandas', etc.
```

