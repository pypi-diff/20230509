# Comparing `tmp/elastix_napari-0.1.8.tar.gz` & `tmp/elastix_napari-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elastix_napari-0.1.8.tar", last modified: Thu Mar 30 16:54:49 2023, max compression
+gzip compressed data, was "elastix_napari-0.2.0.tar", last modified: Tue May  9 10:53:25 2023, max compression
```

## Comparing `elastix_napari-0.1.8.tar` & `elastix_napari-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:54:49.317461 elastix_napari-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:54:49.305461 elastix_napari-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:54:49.313461 elastix_napari-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/.github/workflows/plugin_preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:54:49.313461 elastix_napari-0.1.8/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/.napari/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-03-30 16:54:49.317461 elastix_napari-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:54:49.313461 elastix_napari-0.1.8/elastix_napari/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/elastix_registration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:54:49.313461 elastix_napari-0.1.8/elastix_napari/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:54:49.317461 elastix_napari-0.1.8/elastix_napari/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   131383 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/tests/data/CT_2D_head_fixed.mha
--rw-r--r--   0 runner    (1001) docker     (123)    65847 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/tests/data/CT_2D_head_fixed_mask.mha
--rw-r--r--   0 runner    (1001) docker     (123)   131383 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/tests/data/CT_2D_head_moving.mha
--rw-r--r--   0 runner    (1001) docker     (123)    65847 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/tests/data/CT_2D_head_moving_mask.mha
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/tests/data/TransformParameters.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/tests/data/fixed_point_set_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/tests/data/moving_point_set_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/tests/data/parameters_Rigid.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/elastix_napari/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:54:49.313461 elastix_napari-0.1.8/elastix_napari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-03-30 16:54:49.000000 elastix_napari-0.1.8/elastix_napari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-30 16:54:49.000000 elastix_napari-0.1.8/elastix_napari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 16:54:49.000000 elastix_napari-0.1.8/elastix_napari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 16:54:49.000000 elastix_napari-0.1.8/elastix_napari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-30 16:54:49.000000 elastix_napari-0.1.8/elastix_napari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-30 16:54:49.000000 elastix_napari-0.1.8/elastix_napari.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 16:54:49.317461 elastix_napari-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-30 16:54:37.000000 elastix_napari-0.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.183645 elastix_napari-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/.github/workflows/plugin_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/.napari/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/elastix_napari/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/elastix_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/elastix_napari/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/elastix_napari/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   131383 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_fixed.mha
+-rw-r--r--   0 runner    (1001) docker     (123)    65847 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_fixed_mask.mha
+-rw-r--r--   0 runner    (1001) docker     (123)   131383 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_moving.mha
+-rw-r--r--   0 runner    (1001) docker     (123)    65847 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_moving_mask.mha
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/TransformParameters.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/fixed_point_set_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/moving_point_set_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/parameters_Rigid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/test_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/test_transformix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/transformix_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/elastix_napari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-09 10:53:25.000000 elastix_napari-0.2.0/elastix_napari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-09 10:53:25.000000 elastix_napari-0.2.0/elastix_napari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:53:25.000000 elastix_napari-0.2.0/elastix_napari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-09 10:53:25.000000 elastix_napari-0.2.0/elastix_napari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-09 10:53:25.000000 elastix_napari-0.2.0/elastix_napari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 10:53:25.000000 elastix_napari-0.2.0/elastix_napari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/tox.ini
```

### Comparing `elastix_napari-0.1.8/.github/workflows/plugin_preview.yml` & `elastix_napari-0.2.0/.github/workflows/plugin_preview.yml`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.1.8/.github/workflows/test_and_deploy.yml` & `elastix_napari-0.2.0/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.1.8/.gitignore` & `elastix_napari-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.1.8/.napari/DESCRIPTION.md` & `elastix_napari-0.2.0/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.1.8/LICENSE` & `elastix_napari-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.1.8/PKG-INFO` & `elastix_napari-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastix_napari
-Version: 0.1.8
+Version: 0.2.0
 Summary: A toolbox for rigid and nonrigid registration of images.
 Home-page: https://github.com/SuperElastix/elastix_napari
 Author: Viktor van der Valk
 Author-email: v.o.van_der_valk@lumc.nl
 License: Apache Software License 2.0
 Project-URL: Project Site, https://elastix.lumc.nl/
 Project-URL: Bug Tracker, https://github.com/SuperElastix/elastix_napari/issues
```

### Comparing `elastix_napari-0.1.8/README.md` & `elastix_napari-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.1.8/elastix_napari/elastix_registration.py` & `elastix_napari-0.2.0/elastix_napari/elastix_registration.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import TYPE_CHECKING
 import elastix_napari.utils as utils
-from napari_plugin_engine import napari_hook_implementation
 from magicgui import magic_factory
 import itk
 from pathlib import Path
 from itk_napari_conversion import image_from_image_layer
 from itk_napari_conversion import image_layer_from_image
 
 # For IDE type support and autocompletion
@@ -18,15 +17,15 @@
     Updates widget layout according to user input.
     """
     widget.native.setStyleSheet("QWidget{font-size: 12pt;}")
 
     for x in ['fixed_mask', 'moving_mask', 'param1', 'param2', 'param3',
               'fixed_ps', 'moving_ps', 'metric', 'init_trans',
               'resolutions', 'max_iterations', 'nr_spatial_samples',
-              'max_step_length']:
+              'max_step_length', 'output_dir']:
         setattr(getattr(widget, x), 'visible', False)
 
     @widget.masks.changed.connect
     def toggle_mask_widgets(value):
         for x in ['fixed_mask', 'moving_mask']:
             setattr(getattr(widget, x), 'visible', value)
 
@@ -43,14 +42,19 @@
             for x in ['param1', 'param2', 'param3']:
                 setattr(getattr(widget, x), 'visible', False)
             for x in ['metric', 'init_trans', 'resolutions', 'max_iterations',
                       'nr_spatial_samples', 'max_step_length', 'moving_ps',
                       'fixed_ps']:
                 setattr(getattr(widget, x), 'visible', widget.advanced.value)
 
+    @widget.save_output.changed.connect
+    def toggle_save_output_widget(value):
+        setattr(getattr(widget, 'output_dir'), 'visible', value)
+
+
     @widget.advanced.changed.connect
     def toggle_advanced_widget(value):
         if widget.preset.value == "custom":
             for x in ['init_trans', 'fixed_ps', 'moving_ps']:
                 setattr(getattr(widget, x), 'visible', value)
         else:
             for x in ['metric', 'init_trans', 'resolutions',
@@ -81,50 +85,54 @@
                metric={"choices": ["AdvancedMattesMutualInformation",
                                    "AdvancedNormalizedCorrelation",
                                    "AdvancedMeanSquares"],
                        "tooltip": 'Select a metric to use'},
                init_trans={"label": "initial transform", "filter": "*.txt",
                            "tooltip": 'Load a initial transform from a .txt '
                            'file'},
+               output_dir={"label": "output directory", "mode": "d",
+                           "tooltip": "Specify output directory to store the results"},
                nr_spatial_samples={"max": 8192, "step": 256,
                                    "tooltip": 'Select the number of spatial '
                                    'samples to use'})
-def elastix_registration(fixed: 'napari.layers.Image',
-                         moving: 'napari.layers.Image', preset: str,
+def elastix_registration(fixed_image: 'napari.layers.Image',
+                         moving_image: 'napari.layers.Image', preset: str,
                          fixed_mask: 'napari.layers.Image',
                          moving_mask: 'napari.layers.Image',
                          fixed_ps: Path, moving_ps: Path,
                          param1: Path, param2: Path,
                          param3: Path, init_trans: Path,
+                         output_dir: Path,
                          metric: str = "AdvancedMattesMutualInformation",
                          resolutions: int = 4, max_iterations: int = 500,
                          nr_spatial_samples: int = 512,
-                         max_step_length: float = 1.0,  masks: bool = False,
+                         max_step_length: float = 1.0,   
+                         masks: bool = False, save_output: bool = False, 
                          advanced: bool = False
                          ) -> 'napari.layers.Image':
     """
     Takes user input and calls elastix' registration function in itkelastix.
     """
-    if fixed is None or moving is None:
+    if fixed_image is None or moving_image is None:
         return utils.error("No images selected for registration.")
     if fixed_ps.exists() != moving_ps.exists():
         return utils.error("Select both fixed and moving point set.")
 
     if not utils.check_filename(init_trans):
         init_trans = ''
     if not utils.check_filename(fixed_ps):
         fixed_ps = ''
     if not utils.check_filename(moving_ps):
         moving_ps = ''
 
     # Convert image layer to itk_image
-    fixed = image_from_image_layer(fixed)
-    moving = image_from_image_layer(moving)
-    fixed = fixed.astype(itk.F)
-    moving = moving.astype(itk.F)
+    fixed_image = image_from_image_layer(fixed_image)
+    moving_image = image_from_image_layer(moving_image)
+    fixed_image = fixed_image.astype(itk.F)
+    moving_image = moving_image.astype(itk.F)
 
     parameter_object = itk.ParameterObject.New()
     if preset == "custom":
         for par in [param1, param2, param3]:
             if par.suffix == ".txt":
                 try:
                     parameter_object.AddParameterFile(str(par))
@@ -147,70 +155,45 @@
             parameter_map['MaximumStepLength'] = [str(max_step_length)]
             parameter_map['NumberOfSpatialSamples'] = [str(nr_spatial_samples)]
             parameter_map['MaximumNumberOfIterations'] = [str(max_iterations)]
         else:
             parameter_map = parameter_object.GetDefaultParameterMap(preset, 4)
         parameter_object.AddParameterMap(parameter_map)
 
-    if not masks:
-        result_image, result_transform_parameters = \
-            itk.elastix_registration_method(
-                fixed, moving, parameter_object,
-                fixed_point_set_file_name=str(fixed_ps),
-                moving_point_set_file_name=str(moving_ps),
-                initial_transform_parameter_file_name=str(init_trans),
-                log_to_console=True)
+    kwargs = {"fixed_image": fixed_image,
+              "moving_image": moving_image,
+              "parameter_object": parameter_object,
+              "fixed_point_set_file_name": str(fixed_ps),
+              "moving_point_set_file_name": str(moving_ps),
+              "initial_transform_parameter_file_name": str(init_trans),
+              "log_to_console": True}
 
-    elif masks:
+    if masks:
         if fixed_mask is None and moving_mask is None:
             return utils.error("No masks selected for registration")
         else:
-            if moving_mask is None:
-                # Convert mask layer to itk_image
+            if fixed_mask:
                 fixed_mask = image_from_image_layer(fixed_mask)
                 fixed_mask = fixed_mask.astype(itk.UC)
+                kwargs["fixed_mask"] = fixed_mask
 
-                # Call elastix
-                result_image, rtp = itk.elastix_registration_method(
-                    fixed, moving, parameter_object, fixed_mask=fixed_mask,
-                    fixed_point_set_file_name=str(fixed_ps),
-                    moving_point_set_file_name=str(moving_ps),
-                    initial_transform_parameter_file_name=str(init_trans),
-                    log_to_console=False)
-
-            elif fixed_mask is None:
-                # Convert mask layer to itk_image
-                moving_mask = image_from_image_layer(moving_mask)
-                moving_mask = moving_mask.astype(itk.UC)
-
-                # Call elastix
-                result_image, rtp = itk.elastix_registration_method(
-                    fixed, moving, parameter_object, moving_mask=moving_mask,
-                    fixed_point_set_file_name=str(fixed_ps),
-                    moving_point_set_file_name=str(moving_ps),
-                    initial_transform_parameter_file_name=str(init_trans),
-                    log_to_console=False)
-            else:
-                # Convert mask layer to itk_image
-                fixed_mask = image_from_image_layer(fixed_mask)
-                fixed_mask = fixed_mask.astype(itk.UC)
+            if moving_mask:
                 moving_mask = image_from_image_layer(moving_mask)
                 moving_mask = moving_mask.astype(itk.UC)
+                kwargs["moving_mask"] = moving_mask
+    
+    if save_output:
+        if not output_dir.is_dir() or output_dir == Path():
+            return utils.error("Output directory is not chosen/valid")
+
+        kwargs["output_directory"] = str(output_dir)            
 
-                # Call elastix
-                result_image, rtp = itk.elastix_registration_method(
-                    fixed, moving, parameter_object, fixed_mask=fixed_mask,
-                    moving_mask=moving_mask,
-                    fixed_point_set_file_name=str(fixed_ps),
-                    moving_point_set_file_name=str(moving_ps),
-                    initial_transform_parameter_file_name=str(init_trans),
-                    log_to_console=False)
 
+    # Run elastix registration
+    result_image, result_transform_parameters = itk.elastix_registration_method(**kwargs)
+    
+    # Convert result (itk.Image) to napari layer
     layer = image_layer_from_image(result_image)
     layer.name = preset + " Registration"
     return layer
 
 
-@napari_hook_implementation
-def napari_experimental_provide_dock_widget():
-    return elastix_registration
-
```

### Comparing `elastix_napari-0.1.8/elastix_napari/tests/data/CT_2D_head_fixed.mha` & `elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_fixed.mha`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.1.8/elastix_napari/tests/data/CT_2D_head_fixed_mask.mha` & `elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_fixed_mask.mha`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.1.8/elastix_napari/tests/data/CT_2D_head_moving.mha` & `elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_moving.mha`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.1.8/elastix_napari/tests/data/CT_2D_head_moving_mask.mha` & `elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_moving_mask.mha`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.1.8/elastix_napari/tests/data/TransformParameters.0.txt` & `elastix_napari-0.2.0/elastix_napari/tests/data/TransformParameters.0.txt`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.1.8/elastix_napari/tests/data/parameters_Rigid.txt` & `elastix_napari-0.2.0/elastix_napari/tests/data/parameters_Rigid.txt`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.1.8/elastix_napari/tests/test_registration.py` & `elastix_napari-0.2.0/elastix_napari/tests/test_registration.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,16 @@
 import elastix_napari
 import itk
 from elastix_napari import elastix_registration
 import numpy as np
 from qtpy.QtWidgets import QMessageBox
 from itk_napari_conversion import image_layer_from_image
 from itk_napari_conversion import image_from_image_layer
-
-
-# Test widget function
-def test_dock_widget():
-    assert elastix_napari.napari_experimental_provide_dock_widget() is not None
-
+import tempfile
+from pathlib import Path
 
 # Helper functions
 def image_generator(x1, x2, y1, y2, mask=False, artefact=False,
                     pointset=False, ps_name='fixed', data_dir='none'):
     if mask:
         image = np.zeros([100, 100], np.uint8)
     elif pointset:
@@ -60,15 +56,15 @@
     fixed_image = image_generator(25, 75, 25, 75, artefact=True)
     moving_image = image_generator(1, 51, 10, 60, artefact=True)
 
     # Create mask for artefact
     fixed_mask = image_generator(0, 100, 0, 90, mask=True)
     moving_mask = image_generator(0, 100, 0, 90, mask=True)
 
-    result_image = get_er(fixed=fixed_image, moving=moving_image,
+    result_image = get_er(fixed_image=fixed_image, moving_image=moving_image,
                           fixed_mask=fixed_mask, moving_mask=moving_mask,
                           preset='rigid', masks=True)
 
     # Filter artifacts out of the images.
     masked_fixed_image = np.asarray(
         image_from_image_layer(fixed_image))[0:90, 0:90]
     masked_result_image = np.asarray(
@@ -138,7 +134,27 @@
 
 def test_empty_masks():
     fixed_image = image_generator(25, 75, 25, 75)
     moving_image = image_generator(1, 51, 10, 60)
     im = get_er(fixed_image, moving_image, fixed_mask=None, moving_mask=None,
                 preset='rigid', masks=True)
     assert isinstance(im, QMessageBox)
+
+def test_empty_output_dir():
+    fixed_image = image_generator(25, 75, 25, 75)
+    moving_image = image_generator(1, 51, 10, 60)
+    im = get_er(fixed_image, moving_image, preset='rigid', save_output=True)
+    assert isinstance(im, QMessageBox)
+
+def test_writing_result():
+
+    fixed_image = image_generator(25, 75, 25, 75)
+    moving_image = image_generator(1, 51, 10, 60)
+
+    with tempfile.TemporaryDirectory() as tmpdirname:
+        tmpdir = Path(tmpdirname)
+        im = get_er(fixed_image, moving_image, preset='rigid', save_output=True,
+                    output_dir=tmpdir)
+        assert (tmpdir / "TransformParameters.0.txt").exists()
+    
+
+
```

### Comparing `elastix_napari-0.1.8/elastix_napari/utils.py` & `elastix_napari-0.2.0/elastix_napari/utils.py`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.1.8/elastix_napari.egg-info/PKG-INFO` & `elastix_napari-0.2.0/elastix_napari.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastix-napari
-Version: 0.1.8
+Version: 0.2.0
 Summary: A toolbox for rigid and nonrigid registration of images.
 Home-page: https://github.com/SuperElastix/elastix_napari
 Author: Viktor van der Valk
 Author-email: v.o.van_der_valk@lumc.nl
 License: Apache Software License 2.0
 Project-URL: Project Site, https://elastix.lumc.nl/
 Project-URL: Bug Tracker, https://github.com/SuperElastix/elastix_napari/issues
```

### Comparing `elastix_napari-0.1.8/setup.py` & `elastix_napari-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -63,9 +63,10 @@
     ],
     project_urls={
         'Project Site': 'https://elastix.lumc.nl/',
         'Bug Tracker': 'https://github.com/SuperElastix/elastix_napari/issues',
         'Source Code': 'https://github.com/SuperElastix/elastix_napari',
         'User Support': 'https://groups.google.com/g/elastix-imageregistration',
     },
-    entry_points={'napari.plugin': 'itk-elastix_napari = elastix_napari'},
+    entry_points={'napari.manifest': ['elastix-napari = elastix_napari:napari.yaml']},
+    package_data={'elastix_napari': ['napari.yaml']}
 )
```

### Comparing `elastix_napari-0.1.8/tox.ini` & `elastix_napari-0.2.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -25,12 +25,13 @@
     DISPLAY
     XAUTHORITY
     NUMPY_EXPERIMENTAL_ARRAY_FUNCTION
     PYVISTA_OFF_SCREEN
 deps =
     pytest  # https://docs.pytest.org/en/latest/contents.html
     pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
+    pytest-qt
     linux: pytest-xvfb
     # you can remove these if you don't use them
     qtpy
     pyqt5
 commands = pytest -v --color=yes --cov=elastix_napari --cov-report term-missing
```

