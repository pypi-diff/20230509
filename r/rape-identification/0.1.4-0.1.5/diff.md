# Comparing `tmp/rape_identification-0.1.4.tar.gz` & `tmp/rape_identification-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rape_identification-0.1.4.tar", last modified: Tue May  9 11:11:49 2023, max compression
+gzip compressed data, was "rape_identification-0.1.5.tar", last modified: Tue May  9 11:13:54 2023, max compression
```

## Comparing `rape_identification-0.1.4.tar` & `rape_identification-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:11:49.819383 rape_identification-0.1.4/
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 11:11:49.819383 rape_identification-0.1.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:11:49.815383 rape_identification-0.1.4/rape_identification/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.4/rape_identification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:11:49.819383 rape_identification-0.1.4/rape_identification/config/
--rw-rw-r--   0 root         (0) root         (0)      454 2023-05-09 09:48:54.000000 rape_identification-0.1.4/rape_identification/config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2428 2023-05-09 09:48:54.000000 rape_identification-0.1.4/rape_identification/config/default.py
--rw-rw-r--   0 root         (0) root         (0)     1895 2023-05-09 09:48:54.000000 rape_identification-0.1.4/rape_identification/config/default_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:11:49.819383 rape_identification-0.1.4/rape_identification/dataset/
--rw-rw-r--   0 root         (0) root         (0)     1989 2023-05-09 09:48:54.000000 rape_identification-0.1.4/rape_identification/dataset/SlidingWindowDataset.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:44.000000 rape_identification-0.1.4/rape_identification/dataset/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      706 2023-05-09 09:48:54.000000 rape_identification-0.1.4/rape_identification/inference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:11:49.819383 rape_identification-0.1.4/rape_identification/model/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:11:49.819383 rape_identification-0.1.4/rape_identification/model/SwinUNet/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:40.000000 rape_identification-0.1.4/rape_identification/model/SwinUNet/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    31715 2023-05-09 09:48:54.000000 rape_identification-0.1.4/rape_identification/model/SwinUNet/swin_transformer_unet_skip_expand_decoder_sys.py
--rw-rw-r--   0 root         (0) root         (0)     4177 2023-05-09 09:48:54.000000 rape_identification-0.1.4/rape_identification/model/SwinUNet/vision_transformer.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:35.000000 rape_identification-0.1.4/rape_identification/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:11:49.819383 rape_identification-0.1.4/rape_identification/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 10:54:56.000000 rape_identification-0.1.4/rape_identification/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2764 2023-05-09 09:48:54.000000 rape_identification-0.1.4/rape_identification/utils/convert2uint8.py
--rw-rw-r--   0 root         (0) root         (0)      858 2023-05-09 11:10:50.000000 rape_identification-0.1.4/rape_identification/utils/segment.py
--rw-rw-r--   0 root         (0) root         (0)     4086 2023-05-09 11:11:11.000000 rape_identification-0.1.4/rape_identification/utils/test.py
--rw-rw-r--   0 root         (0) root         (0)    13778 2023-05-09 11:04:06.000000 rape_identification-0.1.4/rape_identification/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:11:49.819383 rape_identification-0.1.4/rape_identification.egg-info/
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 11:11:49.000000 rape_identification-0.1.4/rape_identification.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      922 2023-05-09 11:11:49.000000 rape_identification-0.1.4/rape_identification.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 11:11:49.000000 rape_identification-0.1.4/rape_identification.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-09 11:11:49.000000 rape_identification-0.1.4/rape_identification.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-09 11:11:49.000000 rape_identification-0.1.4/rape_identification.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 11:11:49.819383 rape_identification-0.1.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      937 2023-05-09 11:11:35.000000 rape_identification-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:13:54.282506 rape_identification-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 11:13:54.282506 rape_identification-0.1.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:13:54.282506 rape_identification-0.1.5/rape_identification/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 09:48:54.000000 rape_identification-0.1.5/rape_identification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:13:54.282506 rape_identification-0.1.5/rape_identification/config/
+-rw-rw-r--   0 root         (0) root         (0)      454 2023-05-09 09:48:54.000000 rape_identification-0.1.5/rape_identification/config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2428 2023-05-09 09:48:54.000000 rape_identification-0.1.5/rape_identification/config/default.py
+-rw-rw-r--   0 root         (0) root         (0)     1895 2023-05-09 09:48:54.000000 rape_identification-0.1.5/rape_identification/config/default_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:13:54.282506 rape_identification-0.1.5/rape_identification/dataset/
+-rw-rw-r--   0 root         (0) root         (0)     1989 2023-05-09 09:48:54.000000 rape_identification-0.1.5/rape_identification/dataset/SlidingWindowDataset.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:44.000000 rape_identification-0.1.5/rape_identification/dataset/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      706 2023-05-09 09:48:54.000000 rape_identification-0.1.5/rape_identification/inference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:13:54.282506 rape_identification-0.1.5/rape_identification/model/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:13:54.282506 rape_identification-0.1.5/rape_identification/model/SwinUNet/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:40.000000 rape_identification-0.1.5/rape_identification/model/SwinUNet/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    31715 2023-05-09 09:48:54.000000 rape_identification-0.1.5/rape_identification/model/SwinUNet/swin_transformer_unet_skip_expand_decoder_sys.py
+-rw-rw-r--   0 root         (0) root         (0)     4177 2023-05-09 09:48:54.000000 rape_identification-0.1.5/rape_identification/model/SwinUNet/vision_transformer.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 11:05:35.000000 rape_identification-0.1.5/rape_identification/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:13:54.282506 rape_identification-0.1.5/rape_identification/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-09 10:54:56.000000 rape_identification-0.1.5/rape_identification/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2764 2023-05-09 09:48:54.000000 rape_identification-0.1.5/rape_identification/utils/convert2uint8.py
+-rw-rw-r--   0 root         (0) root         (0)      858 2023-05-09 11:10:50.000000 rape_identification-0.1.5/rape_identification/utils/segment.py
+-rw-rw-r--   0 root         (0) root         (0)     4086 2023-05-09 11:11:11.000000 rape_identification-0.1.5/rape_identification/utils/test.py
+-rw-rw-r--   0 root         (0) root         (0)    13780 2023-05-09 11:13:36.000000 rape_identification-0.1.5/rape_identification/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:13:54.282506 rape_identification-0.1.5/rape_identification.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-09 11:13:54.000000 rape_identification-0.1.5/rape_identification.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      922 2023-05-09 11:13:54.000000 rape_identification-0.1.5/rape_identification.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 11:13:54.000000 rape_identification-0.1.5/rape_identification.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-09 11:13:54.000000 rape_identification-0.1.5/rape_identification.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-09 11:13:54.000000 rape_identification-0.1.5/rape_identification.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 11:13:54.282506 rape_identification-0.1.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      937 2023-05-09 11:13:45.000000 rape_identification-0.1.5/setup.py
```

### Comparing `rape_identification-0.1.4/PKG-INFO` & `rape_identification-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rape_identification
-Version: 0.1.4
+Version: 0.1.5
 Summary: Segmentation any rape
 Author: PingYang
 Author-email: PingYang97@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rape_identification-0.1.4/rape_identification/config/default.py` & `rape_identification-0.1.5/rape_identification/config/default.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.4/rape_identification/config/default_test.py` & `rape_identification-0.1.5/rape_identification/config/default_test.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.4/rape_identification/dataset/SlidingWindowDataset.py` & `rape_identification-0.1.5/rape_identification/dataset/SlidingWindowDataset.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.4/rape_identification/inference.py` & `rape_identification-0.1.5/rape_identification/inference.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.4/rape_identification/model/SwinUNet/swin_transformer_unet_skip_expand_decoder_sys.py` & `rape_identification-0.1.5/rape_identification/model/SwinUNet/swin_transformer_unet_skip_expand_decoder_sys.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.4/rape_identification/model/SwinUNet/vision_transformer.py` & `rape_identification-0.1.5/rape_identification/model/SwinUNet/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.4/rape_identification/utils/convert2uint8.py` & `rape_identification-0.1.5/rape_identification/utils/convert2uint8.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.4/rape_identification/utils/segment.py` & `rape_identification-0.1.5/rape_identification/utils/segment.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.4/rape_identification/utils/test.py` & `rape_identification-0.1.5/rape_identification/utils/test.py`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.4/rape_identification/utils/utils.py` & `rape_identification-0.1.5/rape_identification/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         elif self.cfg.NAME == 'FCN':
             from model.FCN_8s.FCN_ResNet import FCN_ResNet
             return FCN_ResNet(self.cfg.NUM_CLASSES)
 
         elif self.cfg.NAME == 'SwinUNet':
             from ..model.SwinUNet.vision_transformer import SwinUnet as ViT_seg
             from ..config.default import get_cfg
-            model_config = get_cfg('config/GID.yaml')
+            model_config = get_cfg('..config/GID.yaml')
             return ViT_seg(model_config)
 
 
 class SegmentationMetric(object):
     def __init__(self, numClass):
         self.numClass = numClass
         self.confusionMatrix = np.zeros((self.numClass,) * 2)
```

### Comparing `rape_identification-0.1.4/rape_identification.egg-info/PKG-INFO` & `rape_identification-0.1.5/rape_identification.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rape-identification
-Version: 0.1.4
+Version: 0.1.5
 Summary: Segmentation any rape
 Author: PingYang
 Author-email: PingYang97@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rape_identification-0.1.4/rape_identification.egg-info/SOURCES.txt` & `rape_identification-0.1.5/rape_identification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rape_identification-0.1.4/setup.py` & `rape_identification-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rape_identification',  # 与项目文件夹结构中的包名相同
-    version='0.1.4',
+    version='0.1.5',
     description='Segmentation any rape',
     author='PingYang',
     author_email='PingYang97@163.com',
     # url='https://github.com/yourusername/your_project',
     packages=find_packages(),
     install_requires=[
         # Add your project's dependencies here, e.g., 'numpy', 'pandas', etc.
```

