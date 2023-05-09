# Comparing `tmp/napari-sam-0.4.7.tar.gz` & `tmp/napari-sam-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.4.7.tar", last modified: Mon May  8 12:07:19 2023, max compression
+gzip compressed data, was "napari-sam-0.4.8.tar", last modified: Tue May  9 13:02:31 2023, max compression
```

## Comparing `napari-sam-0.4.7.tar` & `napari-sam-0.4.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:07:19.217528 napari-sam-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-08 12:06:59.000000 napari-sam-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 12:06:59.000000 napari-sam-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-08 12:07:19.217528 napari-sam-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-08 12:06:59.000000 napari-sam-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 12:06:59.000000 napari-sam-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-08 12:07:19.217528 napari-sam-0.4.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:07:19.209528 napari-sam-0.4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:07:19.213528 napari-sam-0.4.7/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-08 12:06:59.000000 napari-sam-0.4.7/src/napari_sam/QCollapsibleBox.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 12:06:59.000000 napari-sam-0.4.7/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66801 2023-05-08 12:06:59.000000 napari-sam-0.4.7/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 12:06:59.000000 napari-sam-0.4.7/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-08 12:06:59.000000 napari-sam-0.4.7/src/napari_sam/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-08 12:06:59.000000 napari-sam-0.4.7/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:07:19.217528 napari-sam-0.4.7/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-08 12:07:19.000000 napari-sam-0.4.7/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 12:07:19.000000 napari-sam-0.4.7/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:07:19.000000 napari-sam-0.4.7/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 12:07:19.000000 napari-sam-0.4.7/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-08 12:07:19.000000 napari-sam-0.4.7/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 12:07:19.000000 napari-sam-0.4.7/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:02:31.727481 napari-sam-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 13:02:06.000000 napari-sam-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-09 13:02:06.000000 napari-sam-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-09 13:02:31.727481 napari-sam-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-09 13:02:06.000000 napari-sam-0.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-09 13:02:06.000000 napari-sam-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-09 13:02:31.727481 napari-sam-0.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:02:31.723480 napari-sam-0.4.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:02:31.727481 napari-sam-0.4.8/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-09 13:02:06.000000 napari-sam-0.4.8/src/napari_sam/QCollapsibleBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 13:02:06.000000 napari-sam-0.4.8/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66908 2023-05-09 13:02:06.000000 napari-sam-0.4.8/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-09 13:02:06.000000 napari-sam-0.4.8/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-09 13:02:06.000000 napari-sam-0.4.8/src/napari_sam/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-09 13:02:06.000000 napari-sam-0.4.8/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:02:31.727481 napari-sam-0.4.8/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-09 13:02:31.000000 napari-sam-0.4.8/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-09 13:02:31.000000 napari-sam-0.4.8/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:02:31.000000 napari-sam-0.4.8/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 13:02:31.000000 napari-sam-0.4.8/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-09 13:02:31.000000 napari-sam-0.4.8/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 13:02:31.000000 napari-sam-0.4.8/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.4.7/LICENSE` & `napari-sam-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.7/PKG-INFO` & `napari-sam-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.7
+Version: 0.4.8
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

### Comparing `napari-sam-0.4.7/README.md` & `napari-sam-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.7/setup.cfg` & `napari-sam-0.4.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.7/src/napari_sam/QCollapsibleBox.py` & `napari-sam-0.4.8/src/napari_sam/QCollapsibleBox.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.7/src/napari_sam/_widget.py` & `napari-sam-0.4.8/src/napari_sam/_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,30 +578,31 @@
         self.btn_activate.setEnabled(False)
         if not self.is_active:
             self.image_name = self.cb_image_layers.currentText()
             self.image_layer = self.viewer.layers[self.cb_image_layers.currentText()]
             self.label_layer = self.viewer.layers[self.cb_label_layers.currentText()]
             self.label_layer_changes = None
             # Fixes shape adjustment by napari
-            self.image_layer_affine_scale = self.image_layer.affine.scale
-            self.image_layer_scale = self.image_layer.scale
-            self.image_layer_scale_factor = self.image_layer.scale_factor
-            self.label_layer_affine_scale = self.label_layer.affine.scale
-            self.label_layer_scale = self.label_layer.scale
-            self.label_layer_scale_factor = self.label_layer.scale_factor
-            self.image_layer.affine.scale = np.array([1, 1, 1])
-            self.image_layer.scale = np.array([1, 1, 1])
-            self.image_layer.scale_factor = 1
-            self.label_layer.affine.scale = np.array([1, 1, 1])
-            self.label_layer.scale = np.array([1, 1, 1])
-            self.label_layer.scale_factor = 1
-            pos = self.viewer.dims.point
-            self.viewer.dims.set_point(0, 0)
-            self.viewer.dims.set_point(0, pos[0])
-            self.viewer.reset_view()
+            if self.image_layer.ndim == 3:
+                self.image_layer_affine_scale = self.image_layer.affine.scale
+                self.image_layer_scale = self.image_layer.scale
+                self.image_layer_scale_factor = self.image_layer.scale_factor
+                self.label_layer_affine_scale = self.label_layer.affine.scale
+                self.label_layer_scale = self.label_layer.scale
+                self.label_layer_scale_factor = self.label_layer.scale_factor
+                self.image_layer.affine.scale = np.array([1, 1, 1])
+                self.image_layer.scale = np.array([1, 1, 1])
+                self.image_layer.scale_factor = 1
+                self.label_layer.affine.scale = np.array([1, 1, 1])
+                self.label_layer.scale = np.array([1, 1, 1])
+                self.label_layer.scale_factor = 1
+                pos = self.viewer.dims.point
+                self.viewer.dims.set_point(0, 0)
+                self.viewer.dims.set_point(0, pos[0])
+                self.viewer.reset_view()
 
             if self.image_layer.ndim != 2 and self.image_layer.ndim != 3:
                 raise RuntimeError("Only 2D and 3D images are supported.")
 
             if self.image_layer.ndim == 2:
                 self.sam_logits = None
             else:
```

### Comparing `napari-sam-0.4.7/src/napari_sam/slicer.py` & `napari-sam-0.4.8/src/napari_sam/slicer.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.7/src/napari_sam/utils.py` & `napari-sam-0.4.8/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.7/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.4.8/src/napari_sam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.7
+Version: 0.4.8
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

