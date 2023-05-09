# Comparing `tmp/napari-feature-classifier-0.0.3.tar.gz` & `tmp/napari-feature-classifier-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-feature-classifier-0.0.3.tar", last modified: Fri Mar  3 13:58:43 2023, max compression
+gzip compressed data, was "napari-feature-classifier-0.1.0.tar", last modified: Tue May  9 18:05:29 2023, max compression
```

## Comparing `napari-feature-classifier-0.0.3.tar` & `napari-feature-classifier-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:58:43.962758 napari-feature-classifier-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-03-03 13:58:43.962758 napari-feature-classifier-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-03 13:58:43.962758 napari-feature-classifier-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:58:43.958758 napari-feature-classifier-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:58:43.962758 napari-feature-classifier-0.0.3/src/napari_feature_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:58:43.962758 napari-feature-classifier-0.0.3/src/napari_feature_classifier/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier/_tests/test_annotator_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier/_tests/test_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier/annotator_init_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier/annotator_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    23861 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier/classifier_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-03 13:58:26.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:58:43.962758 napari-feature-classifier-0.0.3/src/napari_feature_classifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-03-03 13:58:43.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-03 13:58:43.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 13:58:43.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-03 13:58:43.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-03 13:58:43.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-03 13:58:43.000000 napari-feature-classifier-0.0.3/src/napari_feature_classifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:05:29.253214 napari-feature-classifier-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-09 18:05:29.253214 napari-feature-classifier-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-09 18:05:29.253214 napari-feature-classifier-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:05:29.249215 napari-feature-classifier-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:05:29.249215 napari-feature-classifier-0.1.0/src/napari_feature_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:05:29.253214 napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/test_annotator_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/test_classifier_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/annotator_init_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/annotator_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24130 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/classifier_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/dev_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/feature_loader_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:05:29.253214 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-09 18:05:29.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-09 18:05:29.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:05:29.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 18:05:29.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 18:05:29.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 18:05:29.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/top_level.txt
```

### Comparing `napari-feature-classifier-0.0.3/LICENSE` & `napari-feature-classifier-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-feature-classifier-0.0.3/PKG-INFO` & `napari-feature-classifier-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-feature-classifier
-Version: 0.0.3
+Version: 0.1.0
 Summary: An interactive classifier plugin to use with label images and feature measurements
 Home-page: https://github.com/fractal-napari-plugins-collection/napari-feature-classifier
 Author: Joel Luethi and Max Hess
 Author-email: joel.luethi@uzh.ch
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/issues
 Project-URL: Documentation, https://github.com/fractal-napari-plugins-collection/napari-feature-classifier#napari-feature-classifier
@@ -18,105 +18,133 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # napari-feature-classifier
 
 [![License](https://img.shields.io/pypi/l/napari-feature-classifier.svg?color=green)](https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-feature-classifier.svg?color=green)](https://pypi.org/project/napari-feature-classifier)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-feature-classifier.svg?color=green)](https://python.org)
 [![tests](https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/workflows/tests/badge.svg)](https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/actions)
 [![codecov](https://codecov.io/gh/fractal-napari-plugins-collection/napari-feature-classifier/branch/main/graph/badge.svg)](https://codecov.io/gh/fractal-napari-plugins-collection/napari-feature-classifier)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-feature-classifier)](https://napari-hub.org/plugins/napari-feature-classifier)
 
 An interactive classifier plugin that allows the user to assign objects in a label image to multiple classes and train a classifier to learn those classes based on a feature dataframe.
 
-
 ## Usage
-<p align="center"><img src="https://user-images.githubusercontent.com/18033446/153727595-60380204-f299-485f-b762-d2030b75e7d3.gif" /></p>
-To use the napari-feature-classifier, you need to have a label image and a csv file containing measurements that correspond to the object in the label image. The csv file needs to contain a column with integer values corresponding to the label values in the label image.
+<p align="center"><img src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/1ebf0890-1a7b-4e4b-a21c-88ca8f1dd800" /></p>
+
+To use the napari-feature-classifier, you need to have a label image and corresponding measurements: as a csv file, loaded to layer.features or in an [OME-Zarr Anndata table loaded with another plugin](https://github.com/jluethi/napari-ome-zarr-roi-loader). Your feature measurements need to contain a `label` column that matches the label objects in the label image.
 These interactive classification workflows are well suited to visually define cell types, find mitotic cells in images, do quality control by automatically detecting missegmented cells and other tasks where a user can easily assign objects to groups.
 
+#### Prepare the label layer:
+- Load your label layer into napari and add the features measurements to layer.features of the corresponding label layer. You can have multiple label layers with their features open at the same time
+    - To load features from a CSV file: `Plugins -> napari-feature-classifier -> CSV Feature Loader`, then load the features for the correct label image.
+    - To load features from an OME-Zarr file: Get both the label layer into memory as a normal label layer (not a pyramidal label layer, currently untested) and the corresponding features. If your OME-Zarr file is created by [Fractal](https://fractal-analytics-platform.github.io/), you can use [this ROI loader plugin](https://github.com/jluethi/napari-ome-zarr-roi-loader).
+    - To load features from anywhere else, load them manually to your label_layer.features
+- Your feature table should have 2 columns used for indexing (but stored as normal columns in layer.features):
+    - The `label` column to match the object in the label image
+    - The `roi_id` column to identify the image you're currently classifying (used when a classifier is trained on multiple label images)
+
+
 #### Initialize a classifier:
 - Start the classifier in napari by going to `Plugins -> napari-feature-classifier -> Initialize a Classifier`  
-- Provide a csv file that contains feature measurements and a column with the integer labels corresponding to the label layer you are using.
-- Choose a name (or relative path from the current working directory) for the classifier. The classifier is initially saved in the current working directory (you can change this later on).
-- Select the features you want to use for the classifier (you need to do the feature selection before initializing. The feature selection can't be changed after initialization anymore). Hold the command key to select multiple features.
-<img width="1831" alt="Initialize Classifier" src="https://user-images.githubusercontent.com/18033446/153727784-d7b7d44b-a7b1-479f-a4af-34e0e280c8d6.png">
+- Select the features you want to use for the classifier (you need to do the feature selection before initializing. The feature selection can't be changed after initialization anymore). Hold the command key to select multiple features. Feature options are always shown for the features available in the last selected label layer, based on layer.features available features.
+- (Optional) Give your classes recognizable names (e.g. Mitotic & Interphase, Cell Type a, b and c etc.)
+<img width="1606" alt="Screenshot 2023-05-09 at 11 46 35" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/452c0d6a-98a3-4e2d-9233-33bfd5bcad19">
+
+
 
 
 #### Classify objects:
+<img width="1802" alt="Classifier_annotation" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/556739b8-972b-4570-9da4-637738fc6a75">
+
 - Make sure you have the label layer selected on which you want to classify
-- Select the current class with the radio buttons or by pressing 0, 1, 2, 3 or 4
+- Select the current class with the radio buttons or by pressing 0, 1, 2, etc.
 - Click on label objects in the viewer to assign them to the currently selected class
-- While you need to have the label layer active to select, sometimes you want to focus on the intensity images. You can press `v` (or manually change the opacity of the label layer) to focus on the intensity images.
-- Once you have trained enough examples, click "Run Classifier" (or press `t`) to run the classifier and have it make a prediction for all objects. Aim for at least a dozen annotations per class, as the classifier divides your annotations 80/20 in training and test sets. To get good performance readouts, aim for >30 annotations per class.
+- Once you have trained enough examples, click "Run Classifier" to run the classifier and have it make a prediction for all objects. Aim for at least a dozen annotations per class, as the classifier divides your annotations 80/20 in training and test sets. 
 - Once you get predictions, correct mistakes the classifier made and retrain it to improve its performance.
-- You can save the classifier under a different name (to move it to a new folder or to have a slightly different version of the classifier - but careful, it autosaves whenever you run it). Define the new output location and then click `Save Classifier` (you need to click the Save Classifier button. Just defining the new output path does not save it yet)
-<img width="1831" alt="trainClassifier" src="https://user-images.githubusercontent.com/18033446/153727960-daae2955-4368-4081-88da-1a1cdbda6e69.png">
+- You can save the classifier under a different name or in a different location. Define the new output location and then click `Save Classifier` (you need to click the Save Classifier button. Just defining the new output path does not save it yet. But every run of the classifier triggers an autosave)
+<img width="1802" alt="Classifier_prediction" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/69cff600-4585-4a66-9274-d2e7caeb335f">
+
 
 
 #### Apply the classifier to additional images:
 - You can apply a classifier trained on one image to additional label images. Use `Plugins -> napari-feature-classifier -> Load Classifier`  
-- Select the classifier (.clf file with the name you gave above) and a csv file containing the same features as the past images.
+- Select the classifier (.clf file with the name you gave above) while already having the label images ready (see `Prepare the label layer` above).
 - Click Load Classifier, proceed as above.
-<img width="1831" alt="LoadClassifier" src="https://user-images.githubusercontent.com/18033446/153728100-dd60918d-c9a4-4de8-8f0e-8fd8c6a51700.png">
+<img width="1606" alt="Screenshot 2023-05-09 at 12 01 00" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/e1143f9f-9729-4f8e-979c-2ab195e0aaca">
+
 
 
 #### Export classifier results
-- To export the training data and the results of the classifier, define an Export Name (full path to an output file or just a filename ending in .csv) where the results of the classifier shall be saved
-- Click `Export Classifier Result` (Just selecting a filename is not enough, you need to click the export button)
-- The results of the classifier are save in a csv file. The first two columns are index columns: path describes the Feature Path used (and allows you to understand which image / feature dataframe a result is from) and label is an integer of the label object within that image. The predict column contains predictions of the classifier for all objects (except those that contained NaNs in their feature data) and the train column contains the annotations you made (0 for unclassified objects, 1, 2, 3 or 4 for the classes)
-![DataStructure](https://user-images.githubusercontent.com/18033446/153728461-d685987d-e1a9-46ff-834b-073008252ccb.png)
+- To export the training data and the results of the classifier, define an Export Name (full path to an output file or just a filename ending in .csv) where the results of the classifier shall be saved. It defaults to the layer name for the selected layer in the last directory you chose (or the current working directory if none was chosen so far)
+- Click `Export Classifier Result` (Just selecting a filename is not enough, you need to click the export button). This will export the predictions for the currently selected layer.
+- The results of the classifier are save in a csv file. The label is an integer of the label object within that image. The prediction column contains predictions of the classifier for all objects (except those that contained NaNs in their feature data) and the annotation column contains the annotations you made (NaN for unclassified objects, -1 for objects you deselected, 1 - 9 for the classes)
+<img width="1802" alt="Classifier_prediction" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/e8f6f7b7-d88b-44f8-b43e-8a2fa81e18d4">
 
 
+#### Batch mode result export
+(To be updated: Create a new notebook to run batch processing, this is for the older version of the classifier)
 There is a simple workflow for the classifier in the examples folder:
 - Install jupyter-lab (`pip install jupyterlab`)
 - Open the notebook in jupyter lab (Type `jupyter-lab` in the terminal when you are in the examples folder)
 - Follow the instructions to generate an example dataframe and an example label image
 - Use the classifier in napari with this simplified data
 
-## Refactored Classifier
-We're currently in the process of refactoring the classifier code to make it more modular. As a first step, we have created a separate Annotator widget that is already available in version 0.0.2 of the classifier. The current classifier doesn't make use of these annotations yet, so only use the new annotator widget if you need annotation only. We are refactoring the classifier to also work with this and will release the refactored classifier later.
 
-#### Initializing the new Annotator
+#### Initializing the Annotator
+You can use the annotation functionality also independently from the classifier
 Start the annotator widget by going to `Plugins -> napari-feature-classifier -> Annotator`
 Select names for your classes. You can name up to 9 classes. Only classes that you give a name will be created upon initialization.
 Then click `Initialize`.
 
 <img width="1411" alt="Screenshot 2023-02-16 at 14 49 38" src="https://user-images.githubusercontent.com/18033446/219384524-9873bd66-270b-4cdd-b913-60d390f6c77a.png">
 
-A new annotator widget opens. Use the Radio-Buttons to select what class you're annotating (or keybindings for 1-9 for classes, 0 for deselect).
+A annotator widget opens. Use the Radio-Buttons to select what class you're annotating (or keybindings for 1-9 for classes, 0 for deselect).
 The annotator will always work on the currently selected label layer. While the annotator is open, you can't edit the labels. Restart napari to allow editing of labels again.
 
 <img width="1411" alt="Screenshot 2023-02-16 at 14 50 00" src="https://user-images.githubusercontent.com/18033446/219384925-b20e4c1a-2eca-4070-8269-902493c5d5ef.png">
 
 The annotations are saved in the `layer.features` table of the corresponding label layer as an `annotations` column.
 <img width="1411" alt="Screenshot 2023-02-16 at 15 01 01" src="https://user-images.githubusercontent.com/18033446/219385788-f61bd0a5-fbb6-42d7-81e5-f77ee4d1b4ff.png">
 
 
 ## Installation
 
 This plugin is written for the new napari npe2 plugin engine. Thus, it requires napari >= 0.4.13.
 Activate your environment where you have napari installed (or install napari using `pip install "napari[all]"`), then install the classifier plugin:
 
     pip install napari-feature-classifier
+
+The layer.features dataframes have some issues in napari 0.4.17 (see [here](https://github.com/napari/napari/issues/5617)). They seem to be working again in the nighlty builds. To set up a nightly builds napari env, do the following:
+
+```
+conda create -n classifier-dev-napari-main -c "napari/label/nightly" -c conda-forge napari python=3.10 -y
+```
     
 ## Similar napari plugins
 If you're looking for other classification approaches, [apoc](https://github.com/haesleinhuepf/apoc) by [Robert Haase](https://github.com/haesleinhuepf) has a pixel classifier in napari and an object classification workflow:  
 [napari-accelerated-pixel-and-object-classification (APOC)](https://github.com/haesleinhuepf/napari-accelerated-pixel-and-object-classification)  
 Alternatively, Clément Cazorla has built [napari-svetlana, a deep learning based classifier](https://www.napari-hub.org/plugins/napari-svetlana)
 
+## Release process
+1. Update the version number in src/napari-feature-classifier/__init__.py
+2. Update the version in setup.cfg
+3. Add a Github release with a new version tag (matching the version set above)
+4. Once tests pass, this should automatically be deployed to pypi
+5. Wait for conda automation to make a PR for an updated conda release (see https://github.com/conda-forge/napari-feature-classifier-feedstock). This can take 1-2 days. Make sure that PR gets merged.
+
 
 ## Contributing
 
 Contributions are very welcome.
 
 ## License
```

### Comparing `napari-feature-classifier-0.0.3/README.md` & `napari-feature-classifier-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,90 +5,118 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-feature-classifier.svg?color=green)](https://python.org)
 [![tests](https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/workflows/tests/badge.svg)](https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/actions)
 [![codecov](https://codecov.io/gh/fractal-napari-plugins-collection/napari-feature-classifier/branch/main/graph/badge.svg)](https://codecov.io/gh/fractal-napari-plugins-collection/napari-feature-classifier)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-feature-classifier)](https://napari-hub.org/plugins/napari-feature-classifier)
 
 An interactive classifier plugin that allows the user to assign objects in a label image to multiple classes and train a classifier to learn those classes based on a feature dataframe.
 
-
 ## Usage
-<p align="center"><img src="https://user-images.githubusercontent.com/18033446/153727595-60380204-f299-485f-b762-d2030b75e7d3.gif" /></p>
-To use the napari-feature-classifier, you need to have a label image and a csv file containing measurements that correspond to the object in the label image. The csv file needs to contain a column with integer values corresponding to the label values in the label image.
+<p align="center"><img src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/1ebf0890-1a7b-4e4b-a21c-88ca8f1dd800" /></p>
+
+To use the napari-feature-classifier, you need to have a label image and corresponding measurements: as a csv file, loaded to layer.features or in an [OME-Zarr Anndata table loaded with another plugin](https://github.com/jluethi/napari-ome-zarr-roi-loader). Your feature measurements need to contain a `label` column that matches the label objects in the label image.
 These interactive classification workflows are well suited to visually define cell types, find mitotic cells in images, do quality control by automatically detecting missegmented cells and other tasks where a user can easily assign objects to groups.
 
+#### Prepare the label layer:
+- Load your label layer into napari and add the features measurements to layer.features of the corresponding label layer. You can have multiple label layers with their features open at the same time
+    - To load features from a CSV file: `Plugins -> napari-feature-classifier -> CSV Feature Loader`, then load the features for the correct label image.
+    - To load features from an OME-Zarr file: Get both the label layer into memory as a normal label layer (not a pyramidal label layer, currently untested) and the corresponding features. If your OME-Zarr file is created by [Fractal](https://fractal-analytics-platform.github.io/), you can use [this ROI loader plugin](https://github.com/jluethi/napari-ome-zarr-roi-loader).
+    - To load features from anywhere else, load them manually to your label_layer.features
+- Your feature table should have 2 columns used for indexing (but stored as normal columns in layer.features):
+    - The `label` column to match the object in the label image
+    - The `roi_id` column to identify the image you're currently classifying (used when a classifier is trained on multiple label images)
+
+
 #### Initialize a classifier:
 - Start the classifier in napari by going to `Plugins -> napari-feature-classifier -> Initialize a Classifier`  
-- Provide a csv file that contains feature measurements and a column with the integer labels corresponding to the label layer you are using.
-- Choose a name (or relative path from the current working directory) for the classifier. The classifier is initially saved in the current working directory (you can change this later on).
-- Select the features you want to use for the classifier (you need to do the feature selection before initializing. The feature selection can't be changed after initialization anymore). Hold the command key to select multiple features.
-<img width="1831" alt="Initialize Classifier" src="https://user-images.githubusercontent.com/18033446/153727784-d7b7d44b-a7b1-479f-a4af-34e0e280c8d6.png">
+- Select the features you want to use for the classifier (you need to do the feature selection before initializing. The feature selection can't be changed after initialization anymore). Hold the command key to select multiple features. Feature options are always shown for the features available in the last selected label layer, based on layer.features available features.
+- (Optional) Give your classes recognizable names (e.g. Mitotic & Interphase, Cell Type a, b and c etc.)
+<img width="1606" alt="Screenshot 2023-05-09 at 11 46 35" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/452c0d6a-98a3-4e2d-9233-33bfd5bcad19">
+
+
 
 
 #### Classify objects:
+<img width="1802" alt="Classifier_annotation" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/556739b8-972b-4570-9da4-637738fc6a75">
+
 - Make sure you have the label layer selected on which you want to classify
-- Select the current class with the radio buttons or by pressing 0, 1, 2, 3 or 4
+- Select the current class with the radio buttons or by pressing 0, 1, 2, etc.
 - Click on label objects in the viewer to assign them to the currently selected class
-- While you need to have the label layer active to select, sometimes you want to focus on the intensity images. You can press `v` (or manually change the opacity of the label layer) to focus on the intensity images.
-- Once you have trained enough examples, click "Run Classifier" (or press `t`) to run the classifier and have it make a prediction for all objects. Aim for at least a dozen annotations per class, as the classifier divides your annotations 80/20 in training and test sets. To get good performance readouts, aim for >30 annotations per class.
+- Once you have trained enough examples, click "Run Classifier" to run the classifier and have it make a prediction for all objects. Aim for at least a dozen annotations per class, as the classifier divides your annotations 80/20 in training and test sets. 
 - Once you get predictions, correct mistakes the classifier made and retrain it to improve its performance.
-- You can save the classifier under a different name (to move it to a new folder or to have a slightly different version of the classifier - but careful, it autosaves whenever you run it). Define the new output location and then click `Save Classifier` (you need to click the Save Classifier button. Just defining the new output path does not save it yet)
-<img width="1831" alt="trainClassifier" src="https://user-images.githubusercontent.com/18033446/153727960-daae2955-4368-4081-88da-1a1cdbda6e69.png">
+- You can save the classifier under a different name or in a different location. Define the new output location and then click `Save Classifier` (you need to click the Save Classifier button. Just defining the new output path does not save it yet. But every run of the classifier triggers an autosave)
+<img width="1802" alt="Classifier_prediction" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/69cff600-4585-4a66-9274-d2e7caeb335f">
+
 
 
 #### Apply the classifier to additional images:
 - You can apply a classifier trained on one image to additional label images. Use `Plugins -> napari-feature-classifier -> Load Classifier`  
-- Select the classifier (.clf file with the name you gave above) and a csv file containing the same features as the past images.
+- Select the classifier (.clf file with the name you gave above) while already having the label images ready (see `Prepare the label layer` above).
 - Click Load Classifier, proceed as above.
-<img width="1831" alt="LoadClassifier" src="https://user-images.githubusercontent.com/18033446/153728100-dd60918d-c9a4-4de8-8f0e-8fd8c6a51700.png">
+<img width="1606" alt="Screenshot 2023-05-09 at 12 01 00" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/e1143f9f-9729-4f8e-979c-2ab195e0aaca">
+
 
 
 #### Export classifier results
-- To export the training data and the results of the classifier, define an Export Name (full path to an output file or just a filename ending in .csv) where the results of the classifier shall be saved
-- Click `Export Classifier Result` (Just selecting a filename is not enough, you need to click the export button)
-- The results of the classifier are save in a csv file. The first two columns are index columns: path describes the Feature Path used (and allows you to understand which image / feature dataframe a result is from) and label is an integer of the label object within that image. The predict column contains predictions of the classifier for all objects (except those that contained NaNs in their feature data) and the train column contains the annotations you made (0 for unclassified objects, 1, 2, 3 or 4 for the classes)
-![DataStructure](https://user-images.githubusercontent.com/18033446/153728461-d685987d-e1a9-46ff-834b-073008252ccb.png)
+- To export the training data and the results of the classifier, define an Export Name (full path to an output file or just a filename ending in .csv) where the results of the classifier shall be saved. It defaults to the layer name for the selected layer in the last directory you chose (or the current working directory if none was chosen so far)
+- Click `Export Classifier Result` (Just selecting a filename is not enough, you need to click the export button). This will export the predictions for the currently selected layer.
+- The results of the classifier are save in a csv file. The label is an integer of the label object within that image. The prediction column contains predictions of the classifier for all objects (except those that contained NaNs in their feature data) and the annotation column contains the annotations you made (NaN for unclassified objects, -1 for objects you deselected, 1 - 9 for the classes)
+<img width="1802" alt="Classifier_prediction" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/e8f6f7b7-d88b-44f8-b43e-8a2fa81e18d4">
 
 
+#### Batch mode result export
+(To be updated: Create a new notebook to run batch processing, this is for the older version of the classifier)
 There is a simple workflow for the classifier in the examples folder:
 - Install jupyter-lab (`pip install jupyterlab`)
 - Open the notebook in jupyter lab (Type `jupyter-lab` in the terminal when you are in the examples folder)
 - Follow the instructions to generate an example dataframe and an example label image
 - Use the classifier in napari with this simplified data
 
-## Refactored Classifier
-We're currently in the process of refactoring the classifier code to make it more modular. As a first step, we have created a separate Annotator widget that is already available in version 0.0.2 of the classifier. The current classifier doesn't make use of these annotations yet, so only use the new annotator widget if you need annotation only. We are refactoring the classifier to also work with this and will release the refactored classifier later.
 
-#### Initializing the new Annotator
+#### Initializing the Annotator
+You can use the annotation functionality also independently from the classifier
 Start the annotator widget by going to `Plugins -> napari-feature-classifier -> Annotator`
 Select names for your classes. You can name up to 9 classes. Only classes that you give a name will be created upon initialization.
 Then click `Initialize`.
 
 <img width="1411" alt="Screenshot 2023-02-16 at 14 49 38" src="https://user-images.githubusercontent.com/18033446/219384524-9873bd66-270b-4cdd-b913-60d390f6c77a.png">
 
-A new annotator widget opens. Use the Radio-Buttons to select what class you're annotating (or keybindings for 1-9 for classes, 0 for deselect).
+A annotator widget opens. Use the Radio-Buttons to select what class you're annotating (or keybindings for 1-9 for classes, 0 for deselect).
 The annotator will always work on the currently selected label layer. While the annotator is open, you can't edit the labels. Restart napari to allow editing of labels again.
 
 <img width="1411" alt="Screenshot 2023-02-16 at 14 50 00" src="https://user-images.githubusercontent.com/18033446/219384925-b20e4c1a-2eca-4070-8269-902493c5d5ef.png">
 
 The annotations are saved in the `layer.features` table of the corresponding label layer as an `annotations` column.
 <img width="1411" alt="Screenshot 2023-02-16 at 15 01 01" src="https://user-images.githubusercontent.com/18033446/219385788-f61bd0a5-fbb6-42d7-81e5-f77ee4d1b4ff.png">
 
 
 ## Installation
 
 This plugin is written for the new napari npe2 plugin engine. Thus, it requires napari >= 0.4.13.
 Activate your environment where you have napari installed (or install napari using `pip install "napari[all]"`), then install the classifier plugin:
 
     pip install napari-feature-classifier
+
+The layer.features dataframes have some issues in napari 0.4.17 (see [here](https://github.com/napari/napari/issues/5617)). They seem to be working again in the nighlty builds. To set up a nightly builds napari env, do the following:
+
+```
+conda create -n classifier-dev-napari-main -c "napari/label/nightly" -c conda-forge napari python=3.10 -y
+```
     
 ## Similar napari plugins
 If you're looking for other classification approaches, [apoc](https://github.com/haesleinhuepf/apoc) by [Robert Haase](https://github.com/haesleinhuepf) has a pixel classifier in napari and an object classification workflow:  
 [napari-accelerated-pixel-and-object-classification (APOC)](https://github.com/haesleinhuepf/napari-accelerated-pixel-and-object-classification)  
 Alternatively, Clément Cazorla has built [napari-svetlana, a deep learning based classifier](https://www.napari-hub.org/plugins/napari-svetlana)
 
+## Release process
+1. Update the version number in src/napari-feature-classifier/__init__.py
+2. Update the version in setup.cfg
+3. Add a Github release with a new version tag (matching the version set above)
+4. Once tests pass, this should automatically be deployed to pypi
+5. Wait for conda automation to make a PR for an updated conda release (see https://github.com/conda-forge/napari-feature-classifier-feedstock). This can take 1-2 days. Make sure that PR gets merged.
+
 
 ## Contributing
 
 Contributions are very welcome.
 
 ## License
```

### Comparing `napari-feature-classifier-0.0.3/setup.cfg` & `napari-feature-classifier-0.1.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-feature-classifier
-version = 0.0.3
+version = 0.1.0
 author = Joel Luethi and Max Hess
 author_email = joel.luethi@uzh.ch
 url = https://github.com/fractal-napari-plugins-collection/napari-feature-classifier
 project_urls = 
 	Bug Tracker = https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/issues
 	Documentation = https://github.com/fractal-napari-plugins-collection/napari-feature-classifier#napari-feature-classifier
 	Source Code = https://github.com/fractal-napari-plugins-collection/napari-feature-classifier
@@ -26,24 +26,27 @@
 	Programming Language :: Python :: 3.10
 	Operating System :: OS Independent
 	License :: OSI Approved :: BSD License
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >=3.7
+python_requires = >=3.9
 package_dir = 
 	=src
 install_requires = 
 	numpy
 	napari
 	matplotlib
 	magicgui
 	pandas
 	scikit-learn
+	pandera
+	xxhash
+	hypothesis
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 napari-feature-classifier = 
 	napari.yaml
```

### Comparing `napari-feature-classifier-0.0.3/src/napari_feature_classifier/_tests/test_annotator_widgets.py` & `napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/test_classifier_widget.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,72 @@
-""" Tests for 3 core dock widgets to see if their initialization generates errors"""
-from pathlib import Path
+""" Tests for classifier widget initialization"""
 import numpy as np
 import pandas as pd
-from napari_feature_classifier.annotator_init_widget import InitializeLabelAnnotator
-from napari_feature_classifier.annotator_widget import (
-    LabelAnnotator, 
-    get_class_selection
-)
 
-# Define a simple test label image for all widgets
-shape = (1, 50, 50)
-lbl_img_np = np.zeros(shape).astype('uint16')
-lbl_img_np[0, 5:10, 5:10] = 1
-lbl_img_np[0, 15:20, 5:10] = 2
-lbl_img_np[0, 25:30, 5:10] = 3
-lbl_img_np[0, 5:10, 15:20] = 4
-lbl_img_np[0, 15:20, 15:20] = 5
-lbl_img_np[0, 25:30, 15:20] = 6
-lbl_img_np[0, 35:40, 15:20] = 7
-lbl_img_np[0, 35:40, 25:30] = 8
-lbl_img_np[0, 5:10, 35:40] = 9
-lbl_img_np[0, 25:30, 25:30] = 10
-lbl_img_np[0, 25:30, 35:40] = 11
-lbl_img_np[0, 5:10, 25:30] = 12
-lbl_img_np[0, 15:20, 25:30] = 13
-lbl_img_np[0, 15:20, 35:40] = 14
-lbl_img_np[0, 35:40, 5:10] = 15
-lbl_img_np[0, 35:40, 35:40] = 16
+import imageio
+from pathlib import Path
+from napari_feature_classifier.feature_loader_widget import make_features
+from napari_feature_classifier.classifier_widget import (
+    ClassifierWidget,
+)
 
+lbl_img_np = imageio.v2.imread(Path("src/napari_feature_classifier/sample_data/test_labels.tif"))
 
 # make_napari_viewer is a pytest fixture that returns a napari viewer object
 # capsys is a pytest fixture that captures stdout and stderr output streams
-def test_annotator_widgets(make_napari_viewer, capsys):
+def test_classifier_widgets_initialization_no_features_selected(make_napari_viewer):
     """
-    Tests if the AnnotatorInit & Annotator widget can be initialized
+    Tests if the main widget launches
     """
     # make viewer and add an image layer using our fixture
     viewer = make_napari_viewer()
-    label_layer = viewer.add_labels(lbl_img_np)
+    _ = viewer.add_labels(lbl_img_np)
 
     # Start init widget
-    _ = InitializeLabelAnnotator(viewer)
+    classifier_widget = ClassifierWidget(viewer)
 
-    # Start the annotator widget
-    annotator_widget = LabelAnnotator(viewer)
+    classifier_widget.initialize_run_widget()
 
-    # call our widget method
-    #my_widget._on_click()
-    annotator_widget._init_annotation(label_layer)
+    # TODO: Catch that it doesn't actually initialize, but instead shows a 
+    # message to the user that now features were selected
+    assert classifier_widget._run_container is None
 
 
-def test_custom_class_selection(make_napari_viewer, capsys):
+# make_napari_viewer is a pytest fixture that returns a napari viewer object
+# TODO: Verify the actual results of the classification
+def test_running_classification_through_widget(make_napari_viewer):
     """
-    Tests the custom class selection
+    Tests if the main widget launches
     """
     # make viewer and add an image layer using our fixture
     viewer = make_napari_viewer()
-    viewer.add_labels(lbl_img_np)
+    label_layer = viewer.add_labels(lbl_img_np)
+    labels = np.unique(lbl_img_np)[1:]
+    label_layer.features = make_features(labels, roi_id="ROI1", n_features=6)
 
-    class_names = ['Class Test', 'Class XYZ', '12345']
-    # Start the annotator widget with a list of named classes
-    LabelAnnotator(
-        viewer,
-        ClassSelection = get_class_selection(class_names = class_names)
-    )
+    # Start init widget
+    classifier_widget = ClassifierWidget(viewer)
 
-def test_numbered_class_selection(make_napari_viewer, capsys):
-    """
-    Tests the custom class selection
-    """
-    # make viewer and add an image layer using our fixture
-    viewer = make_napari_viewer()
-    viewer.add_labels(lbl_img_np)
-    # Start the annotator widget with a given number of classes
-    LabelAnnotator(
-        viewer,
-        ClassSelection = get_class_selection(n_classes = 8)
-    )
+    # Select relevant features
+    classifier_widget._init_container._feature_combobox.value = [
+        "feature_1",
+        "feature_2",
+        "feature_3",
+    ]
+
+    classifier_widget.initialize_run_widget()
+
+    # Check that the run widget is initialized
+    assert classifier_widget._run_container is not None
+
+    # Add some annotations manually
+    label_layer.features.loc[0, "annotations"] = 1.0
+    label_layer.features.loc[1, "annotations"] = 1.0
+    label_layer.features.loc[3, "annotations"] = 3.0
+
+    # Run the classifier
+    classifier_widget._run_container.run()
+
+    # TODO: Assert something
+    assert classifier_widget._run_container._prediction_layer.visible
+    assert "prediction" in label_layer.features.columns
+    assert pd.notna(label_layer.features["prediction"]).all().all()
```

### Comparing `napari-feature-classifier-0.0.3/src/napari_feature_classifier/classifier_widgets.py` & `napari-feature-classifier-0.1.0/src/napari_feature_classifier/classifier_widget.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,608 +1,629 @@
-"""Classfier widget code"""
-import warnings
-import os
-from pathlib import Path
+"""Classifier container widget for napari"""
 import pickle
-from napari import Viewer  # pylint: disable-msg=E0611
-from magicgui import magic_factory, widgets
-from matplotlib.colors import ListedColormap
-from qtpy.QtWidgets import QMessageBox  # pylint: disable-msg=E0611
-from .utils import get_df, napari_info
-from .classifier import Classifier
+
+from pathlib import Path
+from typing import Optional
+
+import napari
+import napari.layers
+import napari.viewer
+import numpy as np
+import pandas as pd
+from magicgui.widgets import (
+    Container,
+    Label,
+    FileEdit,
+    PushButton,
+    Select,
+)
+from qtpy.QtWidgets import QMessageBox  # pylint: disable=E0611
+
+from napari_feature_classifier.annotator_init_widget import LabelAnnotatorTextSelector
+from napari_feature_classifier.annotator_widget import (
+    LabelAnnotator,
+    get_class_selection,
+)
+from napari_feature_classifier.classifier import Classifier
+from napari_feature_classifier.utils import (
+    get_colormap,
+    reset_display_colormaps,
+    get_valid_label_layers,
+    get_selected_or_valid_label_layer,
+    napari_info,
+    overwrite_check_passed,
+    add_annotation_names,
+)
 
 
-def _init_classifier(widget):
+class ClassifierInitContainer(Container):
     """
-    Classifier Initialization Widget initialization
+    The ClassifierInitContainer presents all the options needed for
+    initializing a `ClassifierRunContainer`. It's intended as a container
+    that's used in other magicgui containers.
+
+    It offers feature selection for the last label layer that was selected
+    (or a valid label layer if none had been selected). Changing the selected
+    label layer changes the feature selection that is offered.
+    No action is bound to the _initialize_button => needs to be done in the
+    parent container to bind the correct run action (e.g. start a
+    `ClassifierRunContainer` with the correct parameters)
 
-    Parameters
+    Paramters
+    ---------
+    viewer: napari.Viewer
+        The current napari.Viewer instance
+
+    Attributes
     ----------
-    widget: napari widget
+    viewer: napari.Viewer
+        The current napari.Viewer instance
+    _last_selected_label_layer: napari.layers.Labels
+        The last selected label layer
+    last_selected_layer_label: magicgui.widgets.Label
+        The Label widget for displaying the last selected label layer
+    _feature_combobox: magicgui.widgets.Select
+        The Select widget for selecting the features to use for classification
+    _annotation_name_selector: LabelAnnotatorTextSelector
+        The LabelAnnotatorTextSelector widget for selecting the annotation names
+    _initialize_button: magicgui.widgets.PushButton
+        The PushButton widget for initializing the classifier
     """
 
-    def get_feature_choices(*args):
+    def __init__(self, viewer: napari.viewer.Viewer):
+        self._viewer = viewer
+        try:
+            self._last_selected_label_layer = get_selected_or_valid_label_layer(
+                viewer=self._viewer
+            )
+        except NotImplementedError:
+            self._last_selected_label_layer = None
+        # TODO: Make this label left-aligned, not centered
+        self.last_selected_layer_label = Label(
+            label="Selecting features from:", value=self._last_selected_label_layer
+        )
+        self._feature_combobox = Select(
+            choices=self.get_feature_options(self._last_selected_label_layer),
+            allow_multiple=True,
+            label="Feature Selection:",
+        )
+        self._annotation_name_selector = LabelAnnotatorTextSelector()
+        # pylint: disable=W0212
+        self._initialize_button = PushButton(text="Initialize")
+        super().__init__(
+            widgets=[
+                self.last_selected_layer_label,
+                self._feature_combobox,
+                self._annotation_name_selector,
+                self._initialize_button,
+            ]
+        )
+        self._viewer.layers.selection.events.changed.connect(
+            self.update_layer_selection
+        )
+
+    def get_selected_features(self):
         """
-        Function loading the column names of the widget dataframe
+        Returns the currently selected features (0-n features)
         """
-        try:
-            dataframe = get_df(widget.feature_path.value)
-            return list(dataframe.columns)
-        except IOError:
-            return [""]
-
-    # set feature and label_column "default choices"
-    # to be a function that gets the column names of the
-    # currently loaded dataframe
-    # pylint: disable-msg=W0212
-    widget.feature_selection._default_choices = get_feature_choices
-    widget.label_column._default_choices = get_feature_choices
-
-    @widget.feature_path.changed.connect
-    def update_df_columns():
-        """
-        Handles updating of dropdown options and setting defaults
-        """
-        # ...reset_choices() calls the "get_feature_choices" function above
-        # to keep them updated with the current dataframe
-        widget.feature_selection.reset_choices()
-        widget.label_column.reset_choices()
-        features = widget.label_column.choices
-        if "label" in features:
-            widget.label_column.value = "label"
-        elif "Label" in features:
-            widget.label_column.value = "Label"
-        elif "index" in features:
-            widget.label_column.value = "index"
-
-        # If a user provides a custom property called "feature_selection" for
-        # the label layer and the content of this property is a valid choice,
-        # set the feature selection to that property
-        if "feature_selection" in widget.label_layer.value.properties:
-            if (
-                widget.label_layer.value.properties["feature_selection"]
-                in widget.feature_selection.choices
-            ):
-                widget.feature_selection.value = widget.label_layer.value.properties[
-                    "feature_selection"
-                ]
+        return self._feature_combobox.value
 
-    @widget.label_layer.changed.connect
-    def update_paths():
+    def get_class_names(self):
         """
-        Handles changing label_layer inputs
+        Returns the available class names of the classifier
+        """
+        return self._annotation_name_selector.get_class_names()
 
-        If a user provides a custom property called "feature_path" for
-        the label layer, set the feature_path to that property
+    def get_feature_options(self, layer):
         """
-        if "feature_path" in widget.label_layer.value.properties:
-            widget.feature_path.value = widget.label_layer.value.properties[
-                "feature_path"
-            ]
+        Get the feature options of the currently selected layer
+        Only works if a label layer is selected (we don't load features from other layers)
+        """
+        if isinstance(layer, napari.layers.Labels):
+            return list(layer.features.columns)
+        return []
 
+    def update_layer_selection(self):
+        """
+        Update the layer selection and the feature options if the newly
+        selected layer is a label layer
+        """
+        if isinstance(self._viewer.layers.selection.active, napari.layers.Labels):
+            self._last_selected_label_layer = self._viewer.layers.selection.active
+            self.last_selected_layer_label.value = self._last_selected_label_layer
+            self._feature_combobox.choices = self.get_feature_options(
+                self._last_selected_label_layer
+            )
+            # pylint: disable=W0212
+            self._feature_combobox._default_choices = self.get_feature_options(
+                self._last_selected_label_layer
+            )
 
-# pylint: disable-msg=R0913
-# pylint: disable-msg=W0102
-@magic_factory(
-    call_button="Initialize Classifier",
-    label_layer={"label": "Label Layer:"},
-    feature_path={"label": "Feature Path:", "filter": "*.csv"},
-    classifier_name={"label": "Classifier Name:"},
-    feature_selection={
-        "choices": [""],
-        "allow_multiple": True,
-        "label": "Feature Selection:",
-    },
-    label_column={"choices": [""], "label": "Label Column:"},
-    widget_init=_init_classifier,
-)
-def initialize_classifier(
-    viewer: Viewer,
-    label_layer: "napari.layers.Labels",
-    feature_path: Path,
-    classifier_name="test",
-    feature_selection=[""],
-    label_column="",
-):
+
+# pylint: disable=R0902
+class ClassifierRunContainer(Container):
     """
-    Launches classifier initialization dockwidget
+    The `ClassifierRunContainer` manages all the options needed to do
+    annotations, train a classifier and show classifier results.
 
-    Parameters
+    The `ClassifierRunContainer` can be initialized with either an existing
+    classifier or with class_names + feature_names
+
+    Paramters
+    ---------
+    viewer: napari.Viewer
+        The current napari.Viewer instance
+    classifier: Optional[Classifier]
+        The container can be initialized with an existing classifier. If none
+        is provided, a classifier is generated upon init.
+    class_names: Optional[list[str]]
+        The class names of the classifier. Needs to be provided if no
+        classifier is provided.
+    feature_names: Optional[list[str]]
+        The feature names of the classifier. Needs to be provided if no
+        classifier is provided.
+    classifier_save_path: Optional[str]
+        The path to save the classifier to. If none is provided, the
+        classifier creates a default path in the current working directory.
+    auto_save: Optional[bool]
+        Whether the classifier can automatically save at the
+        classifier_save_path upon run and save. If false, run does not
+        trigger a save and save checks for overwrite conflicts.
+
+    Attributes
     ----------
     viewer: napari.Viewer
         The current napari.Viewer instance
-    label_layer: napari.layers.Labels
-        The napari label layer on which objects shall be classified
-    feature_path: pathlib.Path
-        Path to the .csv file that contains the measurements used for
-        quantification and a column of label integers
-    classifier_name: str
-        Name as which the classifier will be saved. If the default test is
-        chosen, the classifier will be saved as test.clf in the current working
-        directory
-    feature_selection: list
-        List of features that can be selected to classify the objects
-    label_column: str
-        Column name of the column in the feature_path csv file containing the
-        label values
+    _last_selected_label_layer: napari.layers.Labels
+        The last selected label layer
+    _classifier: Classifier
+        The classifier object
+    class_names: list[str]
+        The class names of the classifier classes. Matching the first name to
+        1, second to 2 etc.
+    feature_names: list[str]
+        The feature names of the classifier. These features are loaded from
+        layer.features to train the classifier
+    _label_column: str
+        The column name of the label column in the layer.features dataframe,
+        hard-coded to "label"
+    _roi_id_column: str
+        The column name of the roi_id column in the layer.features dataframe,
+        hard-coded to "roi_id"
+    _annotator: LabelAnnotator
+        The LabelAnnotator container that manages annotations
+    _prediction_layer: napari.layers.Labels
+        The prediction layer that is generated by the classifier and which
+        displays predictions made for the currently selected label layer.
+    _run_button: magicgui.widgets.PushButton
+        The PushButton widget for running the classifier
+    _save_destination: magicgui.widgets.FileEdit
+        The FileEdit widget for selecting the save destination of the classifier
+    _save_button: magicgui.widgets.PushButton
+        The PushButton widget for saving the classifier
     """
-    # TODO: Check whether features are associated with the Labels layer in the
-    # new napari convention (as a dataframe). Use them if they are,
-    # otherwise load csv
-    if not str(feature_path).endswith(".csv"):
-        warnings.warn(
-            "The feature_path does not lead to a .csv file. This "
-            "classifier requires the data to be save in a .csv "
-            "file that is readable with pd.read_csv()"
-        )
-
-    site_df = get_df(feature_path)
-    site_df["path"] = feature_path
-    index_columns = ("path", label_column)
-    site_df = site_df.set_index(list(index_columns))
-
-    if os.path.exists(classifier_name + ".clf"):
-        msg_box = QMessageBox()
-        msg_box.setText(
-            f"A classifier with the name {classifier_name}.clf already exists "
-            "in your working directory. This will overwrite it."
-        )
-        msg_box.setWindowTitle("Overwrite Classifier?")
-        msg_box.setStandardButtons(QMessageBox.Ok | QMessageBox.Cancel)
-        answer = msg_box.exec()
-        if answer == QMessageBox.Cancel:
-            return
 
-    clf = Classifier(
-        name=classifier_name,
-        features=site_df,
-        training_features=feature_selection,
-        index_columns=index_columns,
-    )
-
-    if len(feature_selection) < 1:
-        warnings.warn(
-            "No features were selected for the classifier. Please select '\
-            'features before initializing the classifier"
-        )
-    else:
-        ClassifierWidget(clf, label_layer, feature_path, viewer)
-
-
-def _init_load_classifier(widget):
-    # TODO: Add an option to check the current working directory for .clf files?
-    #       As an option if no classifier_path is provided as a property
-    # Inputs always update with properties when label layer is changed.
-    @widget.label_layer.changed.connect
-    def update_paths():
-        if "classifier_path" in widget.label_layer.value.properties:
-            widget.classifier_path.value = widget.label_layer.value.properties[
-                "classifier_path"
+    # pylint: disable=R0913
+    def __init__(
+        self,
+        viewer: napari.viewer.Viewer,
+        classifier: Optional[Classifier] = None,
+        class_names: Optional[list[str]] = None,
+        feature_names: Optional[list[str]] = None,
+        classifier_save_path: Optional[str] = None,
+        auto_save: Optional[bool] = False,
+    ):
+        self._viewer = viewer
+        self.auto_save = auto_save
+        self._last_selected_label_layer = get_selected_or_valid_label_layer(
+            viewer=self._viewer
+        )
+        # Initialize the classifier
+        if classifier:
+            self._classifier = classifier
+            self.class_names = self._classifier.get_class_names()
+            self.feature_names = self._classifier.get_feature_names()
+        else:
+            if not class_names or not feature_names:
+                raise ValueError(
+                    "A classifier object or "
+                    "class_names & feature_names "
+                    "must be provided"
+                )
+            self._classifier = Classifier(
+                feature_names=feature_names, class_names=class_names
+            )
+            self.class_names = class_names
+            self.feature_names = feature_names
+
+        self._label_column = "label"
+        self._roi_id_colum = "roi_id"
+
+        self._annotator = LabelAnnotator(
+            self._viewer, get_class_selection(class_names=self.class_names)
+        )
+
+        self._prediction_layer = self._viewer.add_labels(
+            self._last_selected_label_layer.data,
+            scale=self._last_selected_label_layer.scale,
+            name="Predictions",
+        )
+
+        # Set the label selection to a valid label layer => Running into proxy bug
+        self._viewer.layers.selection.active = self._last_selected_label_layer
+
+        self._run_button = PushButton(text="Run Classifier")
+        self._save_destination = FileEdit(
+            label="Classifier Save Path",
+            value=f"{self._last_selected_label_layer}_classifier.clf",
+            mode="w",
+        )
+        if classifier_save_path:
+            self._save_destination.value = classifier_save_path
+        self._save_button = PushButton(text="Save Classifier")
+
+        # Export options
+        self._export_destination = FileEdit(
+            label="Prediction Export Path",
+            value=f"{self._last_selected_label_layer}_prediction.csv",
+            mode="w",
+        )
+        self._export_button = PushButton(text="Export Classifier Result")
+        super().__init__(
+            widgets=[
+                self._annotator,
+                self._save_destination,
+                self._run_button,
+                self._save_button,
+                self._export_destination,
+                self._export_button,
             ]
-        if "feature_path" in widget.label_layer.value.properties:
-            widget.feature_path.value = widget.label_layer.value.properties[
-                "feature_path"
+        )
+        self._run_button.clicked.connect(self.run)
+        self._save_button.clicked.connect(self.save)
+        self._export_button.clicked.connect(self.export_results)
+        self._viewer.layers.selection.events.changed.connect(self.selection_changed)
+        self._init_prediction_layer(self._last_selected_label_layer)
+        # Whenever the label layer is clicked, hide the prediction layer
+        # (e.g. new annotations are made)
+        self._last_selected_label_layer.mouse_drag_callbacks.append(
+            self.hide_prediction_layer
+        )
+
+    def run(self):
+        """
+        Run method that adds features to the classifier, trains it, triggers
+        predictions & saves the classifier
+        """
+
+        self.add_features_to_classifier()
+        try:
+            self._classifier.train()
+        except ValueError:
+            napari_info("Not enough annotations made. Please make more annotations.")
+        else:
+            self.make_predictions()
+            self._prediction_layer.visible = True
+            self.save()
+
+    def add_features_to_classifier(self):
+        """
+        Generate a dict of features: Key are roi_ids, values are dataframes
+        from layer.features.
+        """
+        dict_of_features = {}
+        for layer in self._viewer.layers:
+            if (
+                isinstance(layer, napari.layers.Labels)
+                and len(layer.features) > 0
+                and "annotations" in layer.features.columns
+            ):
+                # TODO: Add extra checks that it contains valid features?
+                if "roi_id" in layer.features.columns:
+                    roi_ids = layer.features["roi_id"].unique()
+                    if len(roi_ids) > 1:
+                        raise NotImplementedError(
+                            f"{layer=} contained no-unique roi_ids: {roi_ids}"
+                        )
+
+                    roi_id = roi_ids[0]
+                    dict_of_features[roi_id] = layer.features
+                else:
+                    # TODO: Consider label-layer hashing here instead of
+                    # using the layer name as roi_id
+                    dict_of_features[layer.name] = layer.features
+        self._classifier.add_dict_of_features(dict_of_features)
+
+    def make_predictions(self):
+        """
+        Make predictions for all relevant label layers and add them to the
+        layer.features `prediction` column of each layer
+        """
+        # Get all the label layers that have fitting features
+        relevant_label_layers = self.get_relevant_label_layers()
+
+        # Get the features dataframes with the relevant features
+        prediction_dfs = {}
+        for label_layer in relevant_label_layers:
+            roi_id = self.get_layer_roi_id(label_layer)
+            if roi_id in prediction_dfs.keys():
+                raise ValueError(
+                    f"Duplicate roi_id {roi_id} found in {label_layer.name}. "
+                    "It's already present as the roi_id of another label layer. "
+                )
+            prediction_dfs[roi_id] = self.get_relevant_features(
+                label_layer.features, set_index=False
+            )
+
+        # Get the classifier predictions
+        prediction_results_dict = self._classifier.predict_on_dict(prediction_dfs)
+
+        # Append the predictions to each open label layer ("prediction" column)
+        for label_layer in relevant_label_layers:
+            roi_id = self.get_layer_roi_id(label_layer)
+            if "prediction" in label_layer.features.columns:
+                label_layer.features.drop(columns=["prediction"], inplace=True)
+            # Merge the predictions back into the layer.features dataframe
+            label_layer.features = label_layer.features.merge(
+                prediction_results_dict[roi_id],
+                left_on=[self._roi_id_colum, self._label_column],
+                right_index=True,
+                how="outer",
+            )
+
+        self._init_prediction_layer(self._last_selected_label_layer)
+
+    def selection_changed(self):
+        """
+        Check if the selection change results in a valid label layer being
+        selected. If so, initialize the prediction layer for it.
+        """
+        if self._viewer.layers.selection.active:
+            if self._viewer.layers.selection.active in get_valid_label_layers(
+                viewer=self._viewer
+            ):
+                self._last_selected_label_layer = self._viewer.layers.selection.active
+                self._init_prediction_layer(self._viewer.layers.selection.active)
+                self._last_selected_label_layer.mouse_drag_callbacks.append(
+                    self.hide_prediction_layer
+                )
+                self._update_export_destination(self._last_selected_label_layer)
+
+    def _init_prediction_layer(self, label_layer: napari.layers.Labels):
+        """
+        Initialize the prediction layer and reset its data (to fit the input
+        label_layer) and its colormap
+        """
+        # Check if the predict column already exists in the layer.features
+        if "prediction" not in label_layer.features:
+            unique_labels = np.unique(label_layer.data)[1:]
+            predict_df = pd.DataFrame(
+                {self._label_column: unique_labels, "prediction": np.NaN}
+            )
+            if self._label_column in label_layer.features.columns:
+                label_layer.features = label_layer.features.merge(
+                    predict_df, on=self._label_column, how="outer"
+                )
+            else:
+                label_layer.features = pd.concat(
+                    [label_layer.features, predict_df], axis=1
+                )
+
+        # Update the label data in the prediction layer
+        self._prediction_layer.data = label_layer.data
+        self._prediction_layer.scale = label_layer.scale
+
+        # Update the colormap of the prediction layer
+        reset_display_colormaps(
+            label_layer,
+            feature_col="prediction",
+            display_layer=self._prediction_layer,
+            label_column=self._label_column,
+            cmap=get_colormap(),
+        )
+
+    def hide_prediction_layer(self, labels_layer, event):
+        """
+        Hide the prediction layer
+        """
+        self._prediction_layer.visible = False
+
+    def get_relevant_label_layers(self):
+        relevant_label_layers = []
+        required_columns = [self._label_column, self._roi_id_colum]
+        excluded_label_layers = ["Annotations", "Predictions"]
+        for label_layer in self._viewer.layers:
+            if (
+                isinstance(label_layer, napari.layers.Labels)
+                and label_layer.name not in excluded_label_layers
+            ):
+                if label_layer.features is not None:
+                    if all(x in label_layer.features.columns for x in required_columns):
+                        relevant_label_layers.append(label_layer)
+        return relevant_label_layers
+
+    def get_layer_roi_id(self, label_layer):
+        roi_ids = label_layer.features[self._roi_id_colum].unique()
+        if len(roi_ids) > 1:
+            raise NotImplementedError(
+                f"{label_layer=} contained no-unique roi_ids: {roi_ids}"
+            )
+        return roi_ids[0]
+
+    # pylint: disable=C0103
+    def get_relevant_features(
+        self, df, filter_annotations: bool = False, set_index=False
+    ):
+        """
+        Get the relevant features from the pandas table
+        Can optionally create a double-indexing with label & roi_id
+        filter_annotations: Only return rows that contain annotations?
+        """
+        if not filter_annotations:
+            df_relevant = df[
+                [*self.feature_names, self._label_column, self._roi_id_colum]
             ]
+        else:
+            df_relevant = df.loc[
+                df["annotations"].notna(),
+                [
+                    *self.feature_names,
+                    self._label_column,
+                    self._roi_id_colum,
+                    "annotations",
+                ],
+            ]
+        if set_index:
+            df_relevant.set_index(
+                [self._roi_id_colum, self._label_column], inplace=True
+            )
+        return df_relevant
 
+    def save(self):
+        """
+        Save the classifier and handle overwriting of existing classifier file
+        """
+        if not self.auto_save:
+            # Handle existing classifier file => ask for overwrite
+            if not overwrite_check_passed(
+                file_path=self._save_destination.value, output_type="classifier"
+            ):
+                return
+        # If the user confirms overwriting the classifier once, keep
+        # overwriting it going forward. We want classifier auto-save, just not
+        # overwriting of other existing classifiers with the same name.
+        self.auto_save = True
+        output_path = Path(self._save_destination.value)
+        self._classifier.save(output_path)
 
-@magic_factory(
-    call_button="Load Classifier",
-    label_layer={"label": "Label Layer:"},
-    classifier_path={"label": "Classifier Name:", "filter": "*.clf"},
-    feature_path={"label": "Feature Path:", "filter": "*.csv"},
-    widget_init=_init_load_classifier,
-)
-def load_classifier(
-    viewer: Viewer,
-    label_layer: "napari.layers.Labels",
-    classifier_path: Path,
-    feature_path: Path,
-):
+    def _update_export_destination(self, label_layer: napari.layers.Labels):
+        """
+        Update the default export destination to the name of the label layer.
+        If a base_path was already set, keep it on that base path.
+
+        """
+        base_path = Path(self._export_destination.value).parent
+        self._export_destination.value = base_path / f"annotation_{label_layer.name}.csv"
+
+    def export_results(self):
+        """
+        Export classifier results for the current layer if available
+        """
+        if not overwrite_check_passed(
+            file_path=self._export_destination.value, output_type="predictions"
+        ):
+            return
+
+        predictions = self._last_selected_label_layer.features.loc[
+            :, [self._label_column, "prediction", "annotations"]
+        ]
+        # pylint: disable=C0103
+        df = add_annotation_names(
+            df=pd.DataFrame(predictions), ClassSelection=self._annotator.ClassSelection
+        )
+
+        df.to_csv(self._export_destination.value)
+        napari_info(f"Annotations were saved at {self._export_destination.value}")
+
+
+class LoadClassifierContainer(Container):
     """
-    Launches classifier loading dockwidget
+    The `LoadClassifierContainer` is a second entry-way to the classifier and
+    can launch an appropriate `ClassifierRunContainer`.
 
-    Loads an existing classifier from a .clf file with the set options for
-    feature_selection
+    Paramters
+    ---------
+    viewer: napari.Viewer
+        The current napari.Viewer instance
 
-    Parameters
+    Attributes
     ----------
     viewer: napari.Viewer
         The current napari.Viewer instance
-    label_layer: napari.layers.Labels
-        The napari label layer on which objects shall be classified
-    classifier_path: pathlib.Path
-        Path to an existing classifier .clf file
-    feature_path: pathlib.Path
-        Path to the .csv file that contains the measurements used for
-        quantification and a column of label integers
+    _clf_destination: magicgui.widgets.FileEdit
+        The file edit widget that allows the user to select a classifier file
+    _load_button: magicgui.widgets.PushButton
+        The button that launches the `ClassifierRunContainer`
+    _run_container: ClassifierRunContainer
+         The `ClassifierRunContainer` that is launched by the `_load_button`
     """
-    # TODO: Add option to add new features to the classifier that were not
-    # added at initialization => unsure where to do this. Should it also be
-    # possible when initializing a classifier?
-    # TODO: Add ability to see currently selected features (-> part of being
-    # able to change the features)
-    if not str(feature_path).endswith(".csv"):
-        warnings.warn(
-            "The feature_path does not lead to a .csv file. This "
-            "classifier requires the data to be save in a .csv "
-            "file that is readable with pd.read_csv()"
-        )
-
-    if not str(classifier_path).endswith(".clf"):
-        warnings.warn(
-            "The classifier_path does not lead to a .clf file. This "
-            "plugin only works with classifiers created by its own "
-            "classifier class that are saved as .clf files"
-        )
-
-    with open(classifier_path, "rb") as f:  # pylint: disable-msg=C0103
-        clf = pickle.loads(f.read())
-
-    training_features = clf.training_features
-    site_df = get_df(feature_path)
-    site_df["path"] = feature_path
-    index_columns = clf.index_columns
-    # Catches if new data frame doesn't contain the index columns
-    assert all([index_column in site_df.columns for index_column in index_columns]), (
-        "These two columns are not available in the current "
-        f"dataframe: {index_columns}"
-    )
-    site_df = site_df.set_index(list(index_columns))  # pylint: disable-msg=E1101
-
-    clf.add_data(
-        site_df, training_features=training_features, index_columns=index_columns
-    )
 
-    ClassifierWidget(clf, label_layer, feature_path, viewer)
+    def __init__(self, viewer: napari.viewer.Viewer):
+        self._viewer = viewer
+        self._clf_destination = FileEdit(mode="r", filter="*.clf")
+        self._load_button = PushButton(label="Load Classifier")
+        self._run_container = None
+        super().__init__(widgets=[self._clf_destination, self._load_button])
+        self._load_button.clicked.connect(self.load)
+
+    def load(self):
+        """
+        Load a classifier from a file and start the run container with the
+        correct options(already set classifier_save_path and turn on auto_save)
+        """
+        clf_path = Path(self._clf_destination.value)
+        with open(clf_path, "rb") as f:  # pylint: disable=C0103
+            clf = pickle.load(f)
+
+        self._run_container = ClassifierRunContainer(
+            self._viewer,
+            clf,
+            classifier_save_path=clf_path,
+            auto_save=True,
+        )
+        self.clear()
+        self.append(self._run_container)
+
+        # TODO: Add functionality that loads existing annotations from the
+        # classifier and adds them back to the currently open label images
 
 
-class ClassifierWidget:  # pylint: disable-msg=R0902, R0914
+class ClassifierWidget(Container):
     """
-    The ClassifierWidget creates the napari layers necessary for the classifier
-    and handles the interaction with the classifier clf object
+    The `ClassifierWidget` is the parent widget and the one that is added as
+    a dockwidget. It manages the `ClassifierInitContainer` and the
+    `ClassifierRunContainer`.
 
     Paramters
     ---------
-    clf: clf object
-        Classifier object containing the actual classifier data
-    label_layer: napari.layers.Labels
-        The napari label layer on which objects shall be classified
-    feature_path: pathlib.Path
-        Path to the .csv file that contains the measurements used for
-        quantification and a column of label integers
     viewer: napari.Viewer
         The current napari.Viewer instance
 
     Attributes
     ----------
-    clf: clf object
-        Classifier object containing the actual classifier data
-    label_layer: napari.layers.Labels
-        The napari label layer on which objects shall be classified
-    feature_path: pathlib.Path
-        Path to the .csv file that contains the measurements used for
-        quantification and a column of label integers
     viewer: napari.Viewer
         The current napari.Viewer instance
-    nb_classes: int
-        Number of classes that can be trained with the classifier
-    cmap: matplotlib.colors.ListedColormap
-        colormaps for the classes
-    prediction_layer: napari.layers.Labels
-        Automatically generated label layer on which predictions for each
-        object are shown.
-    selection_layer: napari.layers.Labels
-        Automatically generated label layer on which the annotations made by
-        the user are shown.
-    colordict: dict
-        Dictionary of colors for each index to map colors to label objects
+    _run_container: None or ClassifierRunContainer
+        The `ClassifierRunContainer` that's started.
+    _init_container: None or ClassifierInitContainer
+        The `ClassifierInitContainer` that's started.
     """
 
-    def __init__(self, clf, label_layer, feature_path, viewer):
-        self.clf = clf
-        self.clf.save()
-        self.label_layer = label_layer
-        self.feature_path = feature_path
-        self.viewer = viewer
-
-        # Parameters for the colormaps
-        # TODO: Generalize number of classes & colormap
-        self.nb_classes = 4
-        self.cmap = ListedColormap(
-            [
-                (0.0, 0.0, 0.0, 0.0),
-                (1.0, 0.0, 0.0, 1.0),
-                (0.0, 1.0, 0.0, 1.0),
-                (0.0, 0.0, 1.0, 1.0),
-                (1.0, 0.0, 1.0, 1.0),
-            ]
-        )
+    def __init__(self, viewer: napari.viewer.Viewer):
+        self._viewer = viewer
 
-        # Create a selection & prediction layer
-        if "prediction" in viewer.layers:
-            viewer.layers.remove("prediction")
-        if "selection" in viewer.layers:
-            viewer.layers.remove("selection")
-        self.prediction_layer = viewer.add_labels(
-            label_layer.data, name="prediction", opacity=1.0, scale=label_layer.scale
-        )
-        self.selection_layer = viewer.add_labels(
-            label_layer.data, name="selection", opacity=1.0, scale=label_layer.scale
-        )
-        self.colordict = self.create_label_colormap(
-            self.selection_layer, clf.train_data, "train"
-        )
-        self.create_label_colormap(self.prediction_layer, clf.predict_data, "predict")
-        self.viewer.layers.selection.clear()
-        self.viewer.layers.selection.add(label_layer)
-
-        widget = self.create_selector_widget(self.label_layer)
-
-        # Should I remove the Classifier widget if a new classifier is
-        # initialized?
-        # If so, find a new way to do remove widget of another existing
-        # classifier. Currently triggers a deprecation
-        # warning for napari 0.5
-        # try:
-        #     if self.clf.name in viewer.window._dock_widgets:
-        #         viewer.window.remove_dock_widget(viewer.window._dock_widgets[self.clf.name])
-        # except:
-        #     # If the API for getting dock_widgets changes, just ignore this.
-        #     # This is optional functionality
-        #     pass
-
-        # add widget to napari
-        viewer.window.add_dock_widget(widget, area="right", name=clf.name)
-
-    def create_selector_widget(self, label_layer):  # pylint: disable-msg=R0915
-        """
-        Creates the selector widget to choose a current class, save and export
-        the classifier
-
-        Parameters
-        ----------
-        label_layer: napari.layers.Labels
-            The napari label layer on which objects shall be classified
-        """
-        # TODO: Generalize this. Instead of 0, 1, 2, 3, 4: Arbitrary class
-        # numbers. Ability to add classes & name them?
-        choices = ["Deselect", "Class 1", "Class 2", "Class 3", "Class 4"]
-        selector = widgets.RadioButtons(
-            choices=choices, label="Selection Class:", value="Class 1"
-        )
-        save_path = widgets.FileEdit(
-            value=Path(os.getcwd()) / (self.clf.name + ".clf"),
-            label="Save Classifier As:",
-            mode="w",
-        )
-        save_button = widgets.PushButton(value=True, text="Save Classifier")
-        run_button = widgets.PushButton(value=True, text="Run Classifier")
-        export_path = widgets.FileEdit(
-            value=Path(os.getcwd()) / "Classifier_output.csv",
-            label="Export Name:",
-            mode="w",
-            filter="*.csv",
-        )
-        export_button = widgets.PushButton(value=True, text="Export Classifier Result")
-        container = widgets.Container(
-            widgets=[
-                selector,
-                run_button,
-                save_path,
-                save_button,
-                export_path,
-                export_button,
-            ]
-        )
+        self._init_container = None
+        self._run_container = None
+        self._init_container = None
 
-        @label_layer.mouse_drag_callbacks.append
-        def toggle_label(obj, event):  # pylint: disable-msg=W0613
-            """
-            Handles user annotations by setting the corresponding classifier
-            variables and changing the
-            """
-            # TODO: Add a warning when user clicks while the wrong layer is
-            # selected?
-            self.selection_layer.visible = True
-            # Need to scale position that event.position returns by the
-            # label_layer scale.
-            # If scale is (1, 1, 1), nothing changes
-            # If scale is anything else, this makes the click still match the
-            # correct label
-            scaled_position = tuple(
-                pos / scale for pos, scale in zip(event.position, label_layer.scale)
-            )
-            label = label_layer.get_value(scaled_position)
-            if selector.value is None:
-                napari_info(
-                    "No class is selected. Select a class in the classifier widget."
-                )
-            # Check if background or foreground was clicked. If background was
-            # clicked, do nothing (background can't be assigned a class)
-            elif label == 0 or label is None:
-                pass
-            else:
-                # Check if the label exists in the current dataframe.
-                # Otherwise, do nothing
-                if (self.feature_path, label) in self.clf.train_data.index:
-                    # Assign name of class
-                    # self.clf.train_data.loc[(feature_path, label)] = selector.value
-                    # Assign a numeric value to make it easier
-                    # (colormap currently only supports this mode)
-                    self.clf.train_data.loc[(self.feature_path, label)] = choices.index(
-                        selector.value
-                    )
-                    self.update_label_colormap(
-                        self.selection_layer, label, choices.index(selector.value)
-                    )
-                    self.clf.is_trained = False
-                else:
-                    napari_info(
-                        "The data that was provided to the classifier "
-                        f"does not contain an object with index {label}. "
-                        "Thus, this object cannot be included in the "
-                        "classifier"
-                    )
-
-        @selector.changed.connect
-        def change_choice():
-            self.selection_layer.visible = True
-            self.viewer.layers.selection.clear()
-            # This doesn't work during testing
-            try:
-                self.viewer.layers.selection.add(self.label_layer)
-            except ValueError:
-                pass
-
-        @label_layer.bind_key("s", overwrite=True)
-        @save_button.changed.connect
-        def save_classifier():
-            # Handle name changes
-            classifier_name = Path(save_path.value).name
-            directory = Path(save_path.value).parent
-            napari_info("Saving classifier")
-            self.clf.save(new_name=classifier_name, directory=directory)
-
-        @export_button.changed.connect
-        def export_classifier():
-            # TODO: Check if file path ends in csv.
-            # If not, give a warning dialogue with the option to cancel or add a .csv
-            if not str(export_path.value).endswith(".csv"):
-                warnings.warn(
-                    "The export path does not lead to a .csv file. This "
-                    "export function will export in .csv format anyway"
-                )
+        super().__init__(widgets=[])
 
-            # Check if file already exists
-            if os.path.exists(Path(export_path.value)):
-                msg_box = QMessageBox()
-                msg_box.setText(
-                    f"A csv export with the name {Path(export_path.value).name}"
-                    " already exists. This will overwrite it."
-                )
-                msg_box.setWindowTitle("Overwrite Export?")
-                msg_box.setStandardButtons(QMessageBox.Ok | QMessageBox.Cancel)
-                answer = msg_box.exec()
-                if answer == QMessageBox.Cancel:
-                    return
-            napari_info("Exporting classifier results")
-            self.clf.export_results(export_path.value)
-
-        @label_layer.bind_key("t", overwrite=True)
-        @run_button.changed.connect
-        def run_classifier(key: str):  # pylint: disable-msg=W0613
-            # Check if the classifer contains any training data
-            if len(self.clf.train_data["train"].unique()) > 1:
-                # TODO: Add Run mode? Fuzzy (i.e. trained on everything),
-                # Cross-validated, train/test split
-                self.clf.train()
-                self.create_label_colormap(
-                    self.prediction_layer, self.clf.predict_data, "predict"
-                )
-                self.clf.save()
-                self.selection_layer.visible = False
-                self.prediction_layer.visible = True
-            else:
-                warnings.warn(
-                    "You need to include some annotations to run " "the classifier"
-                )
+        self.initialize_init_widget()
 
-        @label_layer.bind_key("o", overwrite=True)
-        def toggle_selection_sel_layer(layer):  # pylint: disable-msg=W0613
-            current = self.selection_layer.visible
-            self.selection_layer.visible = not current
-
-        @label_layer.bind_key("p", overwrite=True)
-        def toggle_selection_pred_layer(layer):  # pylint: disable-msg=W0613
-            current = self.prediction_layer.visible
-            self.prediction_layer.visible = not current
-
-        @label_layer.bind_key("v", overwrite=True)
-        def toggle_selection(layer):
-            # Toggling off the label layer would be inconvenient
-            # (can't click on it anymore)
-            # => just toggle the opacity to 0
-            opacity = label_layer.opacity
-            if opacity > 0:
-                label_layer.opacity = 0.0
-            else:
-                label_layer.opacity = 0.8
+    def initialize_init_widget(self):
+        self._init_container = ClassifierInitContainer(self._viewer)
+        self.append(self._init_container)
+        self._init_container._initialize_button.clicked.connect(
+            self.initialize_run_widget
+        )
 
-        @label_layer.bind_key("0", overwrite=True)
-        def set_class_0(event):  # pylint: disable-msg=W0613
-            selector.value = choices[0]
-            change_choice()
-
-        @label_layer.bind_key("1", overwrite=True)
-        def set_class_1(event):  # pylint: disable-msg=W0613
-            selector.value = choices[1]
-            change_choice()
-
-        @label_layer.bind_key("2", overwrite=True)
-        def set_class_2(event):  # pylint: disable-msg=W0613
-            selector.value = choices[2]
-            change_choice()
-
-        @label_layer.bind_key("3", overwrite=True)
-        def set_class_3(event):  # pylint: disable-msg=W0613
-            selector.value = choices[3]
-            change_choice()
-
-        @label_layer.bind_key("4", overwrite=True)
-        def set_class_4(event):  # pylint: disable-msg=W0613
-            selector.value = choices[4]
-            change_choice()
-
-        return container
-
-    def update_label_colormap(self, curr_label_layer, label, new_class):
-        """
-        Updates the label colormap and sends the updated colormap to the label
-        layer
-
-        Parameters
-        ----------
-        curr_label_layer: napari.layers.Labels
-            A napari label layer for which an annotation colormap needs to be
-            applied
-        label: int
-            The label value that is being updated
-        new_class: int
-            The new class annotation that is being set
-        """
-
-        # This is still kinda laggy on large dataset.
-        # Is there a way to not send a whole new colormap, but just change
-        # the colormap in one place?
-        # See here for discussion on this topic:
-        # https://forum.image.sc/t/napari-layer-colormaps-update-individual-objects-only/52547
-        # And here for the napari issue:
-        # https://github.com/napari/napari/issues/2380
-        self.colordict[label] = self.cmap(new_class / self.nb_classes)
-        curr_label_layer.color = self.colordict
-        # Directly change just the color of the one object, not replacing the
-        # whole colormap
-        # curr_label_layer.color[label] = self.cmap(new_class/self.nb_classes)
-        # Doesn't do anything. Color doesn't update.
-
-    def create_label_colormap(self, curr_label_layer, data_frame, feature):
-        """
-        Create a new colormap for a whole layer based on a dataframe with
-        annotations
-
-        Parameters
-        ----------
-        curr_label_layer: napari.layers.Labels
-            A napari label layer for which an annotation colormap needs to be
-            applied
-        data_frame: pd.DataFrame
-            Dataframe containing labels and label annotations
-        feature: str
-            Name of the dataframe column containing the annotations
-            (e.g. train or predict)
-        """
-        site_df = data_frame[data_frame.index.isin([self.feature_path], level=0)]
-        site_df.index = site_df.index.droplevel()
-        colors = self.cmap(site_df[feature] / self.nb_classes)
-        colordict = dict(zip(site_df.index, colors))
-        curr_label_layer.color = colordict
-        return colordict
+    def initialize_run_widget(self):
+        class_names = self._init_container.get_class_names()
+        feature_names = self._init_container.get_selected_features()
+        if not feature_names:
+            napari_info("No features selected")
+            return
+        self._run_container = ClassifierRunContainer(
+            self._viewer, class_names=class_names, feature_names=feature_names
+        )
+        self.clear()
+        self.append(self._run_container)
```

### Comparing `napari-feature-classifier-0.0.3/src/napari_feature_classifier/napari.yaml` & `napari-feature-classifier-0.1.0/src/napari_feature_classifier/napari.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 name: napari-feature-classifier
 display_name: napari feature classifier
 contributions:
   commands:
-    - id: napari-feature-classifier.initialize_classifier
-      python_name: napari_feature_classifier.classifier_widgets:initialize_classifier
+    - id: napari-feature-classifier.annotator_init_widget
+      python_name: napari_feature_classifier.annotator_init_widget:InitializeLabelAnnotatorWidget
+      title: Annotator
+    - id: napari-feature-classifier.initialize_classifier_new
+      python_name: napari_feature_classifier.classifier_widget:ClassifierWidget
       title: Initialize a Classifier
     - id: napari-feature-classifier.load_classifier
-      python_name: napari_feature_classifier.classifier_widgets:load_classifier
+      python_name: napari_feature_classifier.classifier_widget:LoadClassifierContainer
       title: Load a Classifier
-    - id: napari-feature-classifier.annotator_init_widget
-      python_name: napari_feature_classifier.annotator_init_widget:InitializeLabelAnnotator
-      title: Annotator
+    - id: napari-feature-classifier.load_csv_features
+      python_name: napari_feature_classifier.feature_loader_widget:load_features_factory
+      title: CSV Feature loader
   widgets:
-    - command: napari-feature-classifier.initialize_classifier
+    - command: napari-feature-classifier.annotator_init_widget
+      display_name: Annotator
+    - command: napari-feature-classifier.initialize_classifier_new
       display_name: Initialize a Classifier
     - command: napari-feature-classifier.load_classifier
       display_name: Load Classifier
-    - command: napari-feature-classifier.annotator_init_widget
-      display_name: Annotator
+    - command: napari-feature-classifier.load_csv_features
+      display_name: CSV Feature loader
```

### Comparing `napari-feature-classifier-0.0.3/src/napari_feature_classifier.egg-info/PKG-INFO` & `napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-feature-classifier
-Version: 0.0.3
+Version: 0.1.0
 Summary: An interactive classifier plugin to use with label images and feature measurements
 Home-page: https://github.com/fractal-napari-plugins-collection/napari-feature-classifier
 Author: Joel Luethi and Max Hess
 Author-email: joel.luethi@uzh.ch
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/issues
 Project-URL: Documentation, https://github.com/fractal-napari-plugins-collection/napari-feature-classifier#napari-feature-classifier
@@ -18,105 +18,133 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # napari-feature-classifier
 
 [![License](https://img.shields.io/pypi/l/napari-feature-classifier.svg?color=green)](https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-feature-classifier.svg?color=green)](https://pypi.org/project/napari-feature-classifier)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-feature-classifier.svg?color=green)](https://python.org)
 [![tests](https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/workflows/tests/badge.svg)](https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/actions)
 [![codecov](https://codecov.io/gh/fractal-napari-plugins-collection/napari-feature-classifier/branch/main/graph/badge.svg)](https://codecov.io/gh/fractal-napari-plugins-collection/napari-feature-classifier)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-feature-classifier)](https://napari-hub.org/plugins/napari-feature-classifier)
 
 An interactive classifier plugin that allows the user to assign objects in a label image to multiple classes and train a classifier to learn those classes based on a feature dataframe.
 
-
 ## Usage
-<p align="center"><img src="https://user-images.githubusercontent.com/18033446/153727595-60380204-f299-485f-b762-d2030b75e7d3.gif" /></p>
-To use the napari-feature-classifier, you need to have a label image and a csv file containing measurements that correspond to the object in the label image. The csv file needs to contain a column with integer values corresponding to the label values in the label image.
+<p align="center"><img src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/1ebf0890-1a7b-4e4b-a21c-88ca8f1dd800" /></p>
+
+To use the napari-feature-classifier, you need to have a label image and corresponding measurements: as a csv file, loaded to layer.features or in an [OME-Zarr Anndata table loaded with another plugin](https://github.com/jluethi/napari-ome-zarr-roi-loader). Your feature measurements need to contain a `label` column that matches the label objects in the label image.
 These interactive classification workflows are well suited to visually define cell types, find mitotic cells in images, do quality control by automatically detecting missegmented cells and other tasks where a user can easily assign objects to groups.
 
+#### Prepare the label layer:
+- Load your label layer into napari and add the features measurements to layer.features of the corresponding label layer. You can have multiple label layers with their features open at the same time
+    - To load features from a CSV file: `Plugins -> napari-feature-classifier -> CSV Feature Loader`, then load the features for the correct label image.
+    - To load features from an OME-Zarr file: Get both the label layer into memory as a normal label layer (not a pyramidal label layer, currently untested) and the corresponding features. If your OME-Zarr file is created by [Fractal](https://fractal-analytics-platform.github.io/), you can use [this ROI loader plugin](https://github.com/jluethi/napari-ome-zarr-roi-loader).
+    - To load features from anywhere else, load them manually to your label_layer.features
+- Your feature table should have 2 columns used for indexing (but stored as normal columns in layer.features):
+    - The `label` column to match the object in the label image
+    - The `roi_id` column to identify the image you're currently classifying (used when a classifier is trained on multiple label images)
+
+
 #### Initialize a classifier:
 - Start the classifier in napari by going to `Plugins -> napari-feature-classifier -> Initialize a Classifier`  
-- Provide a csv file that contains feature measurements and a column with the integer labels corresponding to the label layer you are using.
-- Choose a name (or relative path from the current working directory) for the classifier. The classifier is initially saved in the current working directory (you can change this later on).
-- Select the features you want to use for the classifier (you need to do the feature selection before initializing. The feature selection can't be changed after initialization anymore). Hold the command key to select multiple features.
-<img width="1831" alt="Initialize Classifier" src="https://user-images.githubusercontent.com/18033446/153727784-d7b7d44b-a7b1-479f-a4af-34e0e280c8d6.png">
+- Select the features you want to use for the classifier (you need to do the feature selection before initializing. The feature selection can't be changed after initialization anymore). Hold the command key to select multiple features. Feature options are always shown for the features available in the last selected label layer, based on layer.features available features.
+- (Optional) Give your classes recognizable names (e.g. Mitotic & Interphase, Cell Type a, b and c etc.)
+<img width="1606" alt="Screenshot 2023-05-09 at 11 46 35" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/452c0d6a-98a3-4e2d-9233-33bfd5bcad19">
+
+
 
 
 #### Classify objects:
+<img width="1802" alt="Classifier_annotation" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/556739b8-972b-4570-9da4-637738fc6a75">
+
 - Make sure you have the label layer selected on which you want to classify
-- Select the current class with the radio buttons or by pressing 0, 1, 2, 3 or 4
+- Select the current class with the radio buttons or by pressing 0, 1, 2, etc.
 - Click on label objects in the viewer to assign them to the currently selected class
-- While you need to have the label layer active to select, sometimes you want to focus on the intensity images. You can press `v` (or manually change the opacity of the label layer) to focus on the intensity images.
-- Once you have trained enough examples, click "Run Classifier" (or press `t`) to run the classifier and have it make a prediction for all objects. Aim for at least a dozen annotations per class, as the classifier divides your annotations 80/20 in training and test sets. To get good performance readouts, aim for >30 annotations per class.
+- Once you have trained enough examples, click "Run Classifier" to run the classifier and have it make a prediction for all objects. Aim for at least a dozen annotations per class, as the classifier divides your annotations 80/20 in training and test sets. 
 - Once you get predictions, correct mistakes the classifier made and retrain it to improve its performance.
-- You can save the classifier under a different name (to move it to a new folder or to have a slightly different version of the classifier - but careful, it autosaves whenever you run it). Define the new output location and then click `Save Classifier` (you need to click the Save Classifier button. Just defining the new output path does not save it yet)
-<img width="1831" alt="trainClassifier" src="https://user-images.githubusercontent.com/18033446/153727960-daae2955-4368-4081-88da-1a1cdbda6e69.png">
+- You can save the classifier under a different name or in a different location. Define the new output location and then click `Save Classifier` (you need to click the Save Classifier button. Just defining the new output path does not save it yet. But every run of the classifier triggers an autosave)
+<img width="1802" alt="Classifier_prediction" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/69cff600-4585-4a66-9274-d2e7caeb335f">
+
 
 
 #### Apply the classifier to additional images:
 - You can apply a classifier trained on one image to additional label images. Use `Plugins -> napari-feature-classifier -> Load Classifier`  
-- Select the classifier (.clf file with the name you gave above) and a csv file containing the same features as the past images.
+- Select the classifier (.clf file with the name you gave above) while already having the label images ready (see `Prepare the label layer` above).
 - Click Load Classifier, proceed as above.
-<img width="1831" alt="LoadClassifier" src="https://user-images.githubusercontent.com/18033446/153728100-dd60918d-c9a4-4de8-8f0e-8fd8c6a51700.png">
+<img width="1606" alt="Screenshot 2023-05-09 at 12 01 00" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/e1143f9f-9729-4f8e-979c-2ab195e0aaca">
+
 
 
 #### Export classifier results
-- To export the training data and the results of the classifier, define an Export Name (full path to an output file or just a filename ending in .csv) where the results of the classifier shall be saved
-- Click `Export Classifier Result` (Just selecting a filename is not enough, you need to click the export button)
-- The results of the classifier are save in a csv file. The first two columns are index columns: path describes the Feature Path used (and allows you to understand which image / feature dataframe a result is from) and label is an integer of the label object within that image. The predict column contains predictions of the classifier for all objects (except those that contained NaNs in their feature data) and the train column contains the annotations you made (0 for unclassified objects, 1, 2, 3 or 4 for the classes)
-![DataStructure](https://user-images.githubusercontent.com/18033446/153728461-d685987d-e1a9-46ff-834b-073008252ccb.png)
+- To export the training data and the results of the classifier, define an Export Name (full path to an output file or just a filename ending in .csv) where the results of the classifier shall be saved. It defaults to the layer name for the selected layer in the last directory you chose (or the current working directory if none was chosen so far)
+- Click `Export Classifier Result` (Just selecting a filename is not enough, you need to click the export button). This will export the predictions for the currently selected layer.
+- The results of the classifier are save in a csv file. The label is an integer of the label object within that image. The prediction column contains predictions of the classifier for all objects (except those that contained NaNs in their feature data) and the annotation column contains the annotations you made (NaN for unclassified objects, -1 for objects you deselected, 1 - 9 for the classes)
+<img width="1802" alt="Classifier_prediction" src="https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/assets/18033446/e8f6f7b7-d88b-44f8-b43e-8a2fa81e18d4">
 
 
+#### Batch mode result export
+(To be updated: Create a new notebook to run batch processing, this is for the older version of the classifier)
 There is a simple workflow for the classifier in the examples folder:
 - Install jupyter-lab (`pip install jupyterlab`)
 - Open the notebook in jupyter lab (Type `jupyter-lab` in the terminal when you are in the examples folder)
 - Follow the instructions to generate an example dataframe and an example label image
 - Use the classifier in napari with this simplified data
 
-## Refactored Classifier
-We're currently in the process of refactoring the classifier code to make it more modular. As a first step, we have created a separate Annotator widget that is already available in version 0.0.2 of the classifier. The current classifier doesn't make use of these annotations yet, so only use the new annotator widget if you need annotation only. We are refactoring the classifier to also work with this and will release the refactored classifier later.
 
-#### Initializing the new Annotator
+#### Initializing the Annotator
+You can use the annotation functionality also independently from the classifier
 Start the annotator widget by going to `Plugins -> napari-feature-classifier -> Annotator`
 Select names for your classes. You can name up to 9 classes. Only classes that you give a name will be created upon initialization.
 Then click `Initialize`.
 
 <img width="1411" alt="Screenshot 2023-02-16 at 14 49 38" src="https://user-images.githubusercontent.com/18033446/219384524-9873bd66-270b-4cdd-b913-60d390f6c77a.png">
 
-A new annotator widget opens. Use the Radio-Buttons to select what class you're annotating (or keybindings for 1-9 for classes, 0 for deselect).
+A annotator widget opens. Use the Radio-Buttons to select what class you're annotating (or keybindings for 1-9 for classes, 0 for deselect).
 The annotator will always work on the currently selected label layer. While the annotator is open, you can't edit the labels. Restart napari to allow editing of labels again.
 
 <img width="1411" alt="Screenshot 2023-02-16 at 14 50 00" src="https://user-images.githubusercontent.com/18033446/219384925-b20e4c1a-2eca-4070-8269-902493c5d5ef.png">
 
 The annotations are saved in the `layer.features` table of the corresponding label layer as an `annotations` column.
 <img width="1411" alt="Screenshot 2023-02-16 at 15 01 01" src="https://user-images.githubusercontent.com/18033446/219385788-f61bd0a5-fbb6-42d7-81e5-f77ee4d1b4ff.png">
 
 
 ## Installation
 
 This plugin is written for the new napari npe2 plugin engine. Thus, it requires napari >= 0.4.13.
 Activate your environment where you have napari installed (or install napari using `pip install "napari[all]"`), then install the classifier plugin:
 
     pip install napari-feature-classifier
+
+The layer.features dataframes have some issues in napari 0.4.17 (see [here](https://github.com/napari/napari/issues/5617)). They seem to be working again in the nighlty builds. To set up a nightly builds napari env, do the following:
+
+```
+conda create -n classifier-dev-napari-main -c "napari/label/nightly" -c conda-forge napari python=3.10 -y
+```
     
 ## Similar napari plugins
 If you're looking for other classification approaches, [apoc](https://github.com/haesleinhuepf/apoc) by [Robert Haase](https://github.com/haesleinhuepf) has a pixel classifier in napari and an object classification workflow:  
 [napari-accelerated-pixel-and-object-classification (APOC)](https://github.com/haesleinhuepf/napari-accelerated-pixel-and-object-classification)  
 Alternatively, Clément Cazorla has built [napari-svetlana, a deep learning based classifier](https://www.napari-hub.org/plugins/napari-svetlana)
 
+## Release process
+1. Update the version number in src/napari-feature-classifier/__init__.py
+2. Update the version in setup.cfg
+3. Add a Github release with a new version tag (matching the version set above)
+4. Once tests pass, this should automatically be deployed to pypi
+5. Wait for conda automation to make a PR for an updated conda release (see https://github.com/conda-forge/napari-feature-classifier-feedstock). This can take 1-2 days. Make sure that PR gets merged.
+
 
 ## Contributing
 
 Contributions are very welcome.
 
 ## License
```

### Comparing `napari-feature-classifier-0.0.3/src/napari_feature_classifier.egg-info/SOURCES.txt` & `napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 README.md
 pyproject.toml
 setup.cfg
 src/napari_feature_classifier/__init__.py
 src/napari_feature_classifier/annotator_init_widget.py
 src/napari_feature_classifier/annotator_widget.py
 src/napari_feature_classifier/classifier.py
-src/napari_feature_classifier/classifier_widgets.py
+src/napari_feature_classifier/classifier_widget.py
+src/napari_feature_classifier/dev_main.py
+src/napari_feature_classifier/feature_loader_widget.py
 src/napari_feature_classifier/napari.yaml
 src/napari_feature_classifier/utils.py
 src/napari_feature_classifier.egg-info/PKG-INFO
 src/napari_feature_classifier.egg-info/SOURCES.txt
 src/napari_feature_classifier.egg-info/dependency_links.txt
 src/napari_feature_classifier.egg-info/entry_points.txt
 src/napari_feature_classifier.egg-info/requires.txt
 src/napari_feature_classifier.egg-info/top_level.txt
 src/napari_feature_classifier/_tests/__init__.py
 src/napari_feature_classifier/_tests/test_annotator_widgets.py
-src/napari_feature_classifier/_tests/test_dock_widget.py
+src/napari_feature_classifier/_tests/test_classifier.py
+src/napari_feature_classifier/_tests/test_classifier_widget.py
```

