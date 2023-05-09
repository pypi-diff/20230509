# Comparing `tmp/mctthermalface-0.1.1.tar.gz` & `tmp/mctthermalface-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctthermalface-0.1.1.tar", last modified: Tue May  9 01:33:25 2023, max compression
+gzip compressed data, was "mctthermalface-0.2.0.tar", last modified: Tue May  9 01:56:21 2023, max compression
```

## Comparing `mctthermalface-0.1.1.tar` & `mctthermalface-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:33:25.353996 mctthermalface-0.1.1/
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1940 2023-05-09 01:33:25.353996 mctthermalface-0.1.1/PKG-INFO
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1497 2023-05-08 08:56:05.000000 mctthermalface-0.1.1/README.md
-drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:33:25.353996 mctthermalface-0.1.1/mctthermalface/
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:32:50.000000 mctthermalface-0.1.1/mctthermalface/__init__.py
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     2010 2023-05-08 08:48:44.000000 mctthermalface-0.1.1/mctthermalface/mctthermalface.py
-drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:33:25.353996 mctthermalface-0.1.1/mctthermalface.egg-info/
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1940 2023-05-09 01:33:25.000000 mctthermalface-0.1.1/mctthermalface.egg-info/PKG-INFO
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      267 2023-05-09 01:33:25.000000 mctthermalface-0.1.1/mctthermalface.egg-info/SOURCES.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)        1 2023-05-09 01:33:25.000000 mctthermalface-0.1.1/mctthermalface.egg-info/dependency_links.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-09 01:33:25.000000 mctthermalface-0.1.1/mctthermalface.egg-info/requires.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       15 2023-05-09 01:33:25.000000 mctthermalface-0.1.1/mctthermalface.egg-info/top_level.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-09 01:33:25.353996 mctthermalface-0.1.1/setup.cfg
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      782 2023-05-09 01:33:14.000000 mctthermalface-0.1.1/setup.py
+drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:56:21.618426 mctthermalface-0.2.0/
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1940 2023-05-09 01:56:21.618426 mctthermalface-0.2.0/PKG-INFO
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1497 2023-05-09 01:41:57.000000 mctthermalface-0.2.0/README.md
+drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:56:21.618426 mctthermalface-0.2.0/mctthermalface/
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       36 2023-05-09 01:51:30.000000 mctthermalface-0.2.0/mctthermalface/__init__.py
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     2010 2023-05-09 01:42:35.000000 mctthermalface-0.2.0/mctthermalface/mctthermalface.py
+drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:56:21.618426 mctthermalface-0.2.0/mctthermalface.egg-info/
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1940 2023-05-09 01:56:21.000000 mctthermalface-0.2.0/mctthermalface.egg-info/PKG-INFO
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      267 2023-05-09 01:56:21.000000 mctthermalface-0.2.0/mctthermalface.egg-info/SOURCES.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)        1 2023-05-09 01:56:21.000000 mctthermalface-0.2.0/mctthermalface.egg-info/dependency_links.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-09 01:56:21.000000 mctthermalface-0.2.0/mctthermalface.egg-info/requires.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       15 2023-05-09 01:56:21.000000 mctthermalface-0.2.0/mctthermalface.egg-info/top_level.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-09 01:56:21.618426 mctthermalface-0.2.0/setup.cfg
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      782 2023-05-09 01:55:49.000000 mctthermalface-0.2.0/setup.py
```

### Comparing `mctthermalface-0.1.1/PKG-INFO` & `mctthermalface-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctthermalface
-Version: 0.1.1
+Version: 0.2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,22 +27,22 @@
 - Numpy
 - PyTorch (I recommend to install your PyTorch from [following website](https://pytorch.org/))
 - PIL
 - OpenCV
 
 To Install, run the following command:
 ```bash
-pip install MCTThermalFace
+pip install mctthermalface
 ```
 
 *Only available in PIP, not in Conda*
 
 # Usage
 ```python
-import MCTThermalFace
+import mctthermalface
 from PIL import Image
 
 detector = ThermalFace.Detector('thermal_face_detection.pt')
 img = Image.open("img_path")
 bbox = detector.detect(img)
 ```
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: mctthermalface Version: 0.1.1 Classifier:
+Metadata-Version: 2.1 Name: mctthermalface Version: 0.2.0 Classifier:
 Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown
     # Face Detection on Thermal Image [Python] [PyTorch] ![Sample](https://
      raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample.png)
 # Installation Before installing, make sure the following packages are
 available: - Numpy - PyTorch (I recommend to install your PyTorch from
 [following website](https://pytorch.org/)) - PIL - OpenCV To Install, run the
-following command: ```bash pip install MCTThermalFace ``` *Only available in
-PIP, not in Conda* # Usage ```python import MCTThermalFace from PIL import
+following command: ```bash pip install mctthermalface ``` *Only available in
+PIP, not in Conda* # Usage ```python import mctthermalface from PIL import
 Image detector = ThermalFace.Detector('thermal_face_detection.pt') img =
 Image.open("img_path") bbox = detector.detect(img) ```
 # Model Download Click Here To Download [thermal_face_detection.pt](https://
 github.com/mctosima/MCTThermalFace/blob/master/thermal_face_detection.pt)
 # Sample Usage Check this [notebook](https://github.com/mctosima/
 MCTThermalFace/blob/master/how_to_use.ipynb)
 # Credits Original Works by: Diza Febriyan Hasal on his Bachelor Thesis about
```

### Comparing `mctthermalface-0.1.1/README.md` & `mctthermalface-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 - Numpy
 - PyTorch (I recommend to install your PyTorch from [following website](https://pytorch.org/))
 - PIL
 - OpenCV
 
 To Install, run the following command:
 ```bash
-pip install MCTThermalFace
+pip install mctthermalface
 ```
 
 *Only available in PIP, not in Conda*
 
 # Usage
 ```python
-import MCTThermalFace
+import mctthermalface
 from PIL import Image
 
 detector = ThermalFace.Detector('thermal_face_detection.pt')
 img = Image.open("img_path")
 bbox = detector.detect(img)
 ```
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
     # Face Detection on Thermal Image [Python] [PyTorch] ![Sample](https://
      raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample.png)
 # Installation Before installing, make sure the following packages are
 available: - Numpy - PyTorch (I recommend to install your PyTorch from
 [following website](https://pytorch.org/)) - PIL - OpenCV To Install, run the
-following command: ```bash pip install MCTThermalFace ``` *Only available in
-PIP, not in Conda* # Usage ```python import MCTThermalFace from PIL import
+following command: ```bash pip install mctthermalface ``` *Only available in
+PIP, not in Conda* # Usage ```python import mctthermalface from PIL import
 Image detector = ThermalFace.Detector('thermal_face_detection.pt') img =
 Image.open("img_path") bbox = detector.detect(img) ```
 # Model Download Click Here To Download [thermal_face_detection.pt](https://
 github.com/mctosima/MCTThermalFace/blob/master/thermal_face_detection.pt)
 # Sample Usage Check this [notebook](https://github.com/mctosima/
 MCTThermalFace/blob/master/how_to_use.ipynb)
 # Credits Original Works by: Diza Febriyan Hasal on his Bachelor Thesis about
```

### Comparing `mctthermalface-0.1.1/mctthermalface/mctthermalface.py` & `mctthermalface-0.2.0/mctthermalface/mctthermalface.py`

 * *Files identical despite different names*

### Comparing `mctthermalface-0.1.1/mctthermalface.egg-info/PKG-INFO` & `mctthermalface-0.2.0/mctthermalface.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctthermalface
-Version: 0.1.1
+Version: 0.2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,22 +27,22 @@
 - Numpy
 - PyTorch (I recommend to install your PyTorch from [following website](https://pytorch.org/))
 - PIL
 - OpenCV
 
 To Install, run the following command:
 ```bash
-pip install MCTThermalFace
+pip install mctthermalface
 ```
 
 *Only available in PIP, not in Conda*
 
 # Usage
 ```python
-import MCTThermalFace
+import mctthermalface
 from PIL import Image
 
 detector = ThermalFace.Detector('thermal_face_detection.pt')
 img = Image.open("img_path")
 bbox = detector.detect(img)
 ```
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: mctthermalface Version: 0.1.1 Classifier:
+Metadata-Version: 2.1 Name: mctthermalface Version: 0.2.0 Classifier:
 Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown
     # Face Detection on Thermal Image [Python] [PyTorch] ![Sample](https://
      raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample.png)
 # Installation Before installing, make sure the following packages are
 available: - Numpy - PyTorch (I recommend to install your PyTorch from
 [following website](https://pytorch.org/)) - PIL - OpenCV To Install, run the
-following command: ```bash pip install MCTThermalFace ``` *Only available in
-PIP, not in Conda* # Usage ```python import MCTThermalFace from PIL import
+following command: ```bash pip install mctthermalface ``` *Only available in
+PIP, not in Conda* # Usage ```python import mctthermalface from PIL import
 Image detector = ThermalFace.Detector('thermal_face_detection.pt') img =
 Image.open("img_path") bbox = detector.detect(img) ```
 # Model Download Click Here To Download [thermal_face_detection.pt](https://
 github.com/mctosima/MCTThermalFace/blob/master/thermal_face_detection.pt)
 # Sample Usage Check this [notebook](https://github.com/mctosima/
 MCTThermalFace/blob/master/how_to_use.ipynb)
 # Credits Original Works by: Diza Febriyan Hasal on his Bachelor Thesis about
```

### Comparing `mctthermalface-0.1.1/setup.py` & `mctthermalface-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mctthermalface',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version='0.1.1',
+    version='0.2.0',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'torch',
         'torchvision',
         'opencv-python',
     ],
```

