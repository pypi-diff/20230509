# Comparing `tmp/mctthermalface-0.2.0.tar.gz` & `tmp/mctthermalface-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctthermalface-0.2.0.tar", last modified: Tue May  9 01:56:21 2023, max compression
+gzip compressed data, was "mctthermalface-0.2.2.tar", last modified: Tue May  9 02:28:34 2023, max compression
```

## Comparing `mctthermalface-0.2.0.tar` & `mctthermalface-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:56:21.618426 mctthermalface-0.2.0/
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1940 2023-05-09 01:56:21.618426 mctthermalface-0.2.0/PKG-INFO
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1497 2023-05-09 01:41:57.000000 mctthermalface-0.2.0/README.md
-drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:56:21.618426 mctthermalface-0.2.0/mctthermalface/
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       36 2023-05-09 01:51:30.000000 mctthermalface-0.2.0/mctthermalface/__init__.py
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     2010 2023-05-09 01:42:35.000000 mctthermalface-0.2.0/mctthermalface/mctthermalface.py
-drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:56:21.618426 mctthermalface-0.2.0/mctthermalface.egg-info/
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1940 2023-05-09 01:56:21.000000 mctthermalface-0.2.0/mctthermalface.egg-info/PKG-INFO
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      267 2023-05-09 01:56:21.000000 mctthermalface-0.2.0/mctthermalface.egg-info/SOURCES.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)        1 2023-05-09 01:56:21.000000 mctthermalface-0.2.0/mctthermalface.egg-info/dependency_links.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-09 01:56:21.000000 mctthermalface-0.2.0/mctthermalface.egg-info/requires.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       15 2023-05-09 01:56:21.000000 mctthermalface-0.2.0/mctthermalface.egg-info/top_level.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-09 01:56:21.618426 mctthermalface-0.2.0/setup.cfg
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      782 2023-05-09 01:55:49.000000 mctthermalface-0.2.0/setup.py
+drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 02:28:34.596764 mctthermalface-0.2.2/
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     2411 2023-05-09 02:28:34.596764 mctthermalface-0.2.2/PKG-INFO
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1968 2023-05-09 02:24:47.000000 mctthermalface-0.2.2/README.md
+drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 02:28:34.596764 mctthermalface-0.2.2/mctthermalface/
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       36 2023-05-09 01:51:30.000000 mctthermalface-0.2.2/mctthermalface/__init__.py
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     2128 2023-05-09 02:08:00.000000 mctthermalface-0.2.2/mctthermalface/mctthermalface.py
+drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 02:28:34.596764 mctthermalface-0.2.2/mctthermalface.egg-info/
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     2411 2023-05-09 02:28:34.000000 mctthermalface-0.2.2/mctthermalface.egg-info/PKG-INFO
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      267 2023-05-09 02:28:34.000000 mctthermalface-0.2.2/mctthermalface.egg-info/SOURCES.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)        1 2023-05-09 02:28:34.000000 mctthermalface-0.2.2/mctthermalface.egg-info/dependency_links.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-09 02:28:34.000000 mctthermalface-0.2.2/mctthermalface.egg-info/requires.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       15 2023-05-09 02:28:34.000000 mctthermalface-0.2.2/mctthermalface.egg-info/top_level.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-09 02:28:34.596764 mctthermalface-0.2.2/setup.cfg
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      782 2023-05-09 02:28:17.000000 mctthermalface-0.2.2/setup.py
```

### Comparing `mctthermalface-0.2.0/PKG-INFO` & `mctthermalface-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctthermalface
-Version: 0.2.0
+Version: 0.2.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -12,15 +12,15 @@
 
 <div align="center">
 
 # Face Detection on Thermal Image
 <a href="https://www.python.org/"><img alt="Python" src="https://img.shields.io/badge/-Python 3.7+-blue?style=for-the-badge&logo=python&logoColor=white"></a>
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/-PyTorch 1.8+-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white"></a>
 
-![Sample](https://raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample.png)
+![Sample](https://raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample_new.png)
 
 <br>
 </div>
 
 # Installation
 
 Before installing, make sure the following packages are available:
@@ -33,23 +33,44 @@
 ```bash
 pip install mctthermalface
 ```
 
 *Only available in PIP, not in Conda*
 
 # Usage
+
+### For 3 channels image (8-bit)
 ```python
 import mctthermalface
 from PIL import Image
 
-detector = ThermalFace.Detector('thermal_face_detection.pt')
-img = Image.open("img_path")
+detector = mctthermalface.Detector('thermal_face_detection.pt')
+img = Image.open("img_path.png")
 bbox = detector.detect(img)
 ```
 
+### Fpr 1 channels image (16-bit) stored in csv
+```python
+import mctthermalface
+import cv2
+import numpy as np
+
+detector = mctthermalface.Detector('thermal_face_detection.pt')
+
+img_1channel = np.loadtxt("img_path.csv", delimiter=",")
+img_1channel = cv2.normalize(img_1channel, None, 0, 255, cv2.NORM_MINMAX, cv2.CV_8U)
+bbox = detector.detect(img_1channel)
+```
+
+### Bounding Box Format
+
+```
+bbox = [xmax, xmin, ymax, ymin]
+```
+
 <br>
 
 # Model Download
 Click Here To Download [thermal_face_detection.pt](https://github.com/mctosima/MCTThermalFace/blob/master/thermal_face_detection.pt)
 
 <br>
```

#### html2text {}

```diff
@@ -1,22 +1,28 @@
-Metadata-Version: 2.1 Name: mctthermalface Version: 0.2.0 Classifier:
+Metadata-Version: 2.1 Name: mctthermalface Version: 0.2.2 Classifier:
 Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown
     # Face Detection on Thermal Image [Python] [PyTorch] ![Sample](https://
-     raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample.png)
+   raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample_new.png)
 # Installation Before installing, make sure the following packages are
 available: - Numpy - PyTorch (I recommend to install your PyTorch from
 [following website](https://pytorch.org/)) - PIL - OpenCV To Install, run the
 following command: ```bash pip install mctthermalface ``` *Only available in
-PIP, not in Conda* # Usage ```python import mctthermalface from PIL import
-Image detector = ThermalFace.Detector('thermal_face_detection.pt') img =
-Image.open("img_path") bbox = detector.detect(img) ```
+PIP, not in Conda* # Usage ### For 3 channels image (8-bit) ```python import
+mctthermalface from PIL import Image detector = mctthermalface.Detector
+('thermal_face_detection.pt') img = Image.open("img_path.png") bbox =
+detector.detect(img) ``` ### Fpr 1 channels image (16-bit) stored in csv
+```python import mctthermalface import cv2 import numpy as np detector =
+mctthermalface.Detector('thermal_face_detection.pt') img_1channel = np.loadtxt
+("img_path.csv", delimiter=",") img_1channel = cv2.normalize(img_1channel,
+None, 0, 255, cv2.NORM_MINMAX, cv2.CV_8U) bbox = detector.detect(img_1channel)
+``` ### Bounding Box Format ``` bbox = [xmax, xmin, ymax, ymin] ```
 # Model Download Click Here To Download [thermal_face_detection.pt](https://
 github.com/mctosima/MCTThermalFace/blob/master/thermal_face_detection.pt)
 # Sample Usage Check this [notebook](https://github.com/mctosima/
 MCTThermalFace/blob/master/how_to_use.ipynb)
 # Credits Original Works by: Diza Febriyan Hasal on his Bachelor Thesis about
 Detecting Face in Thermal Image. Reworked by Martin Clinton Manullang to adjust
 the performance, adaptability, and compatibility (2023).
```

### Comparing `mctthermalface-0.2.0/README.md` & `mctthermalface-0.2.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div align="center">
 
 # Face Detection on Thermal Image
 <a href="https://www.python.org/"><img alt="Python" src="https://img.shields.io/badge/-Python 3.7+-blue?style=for-the-badge&logo=python&logoColor=white"></a>
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/-PyTorch 1.8+-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white"></a>
 
-![Sample](https://raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample.png)
+![Sample](https://raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample_new.png)
 
 <br>
 </div>
 
 # Installation
 
 Before installing, make sure the following packages are available:
@@ -21,23 +21,44 @@
 ```bash
 pip install mctthermalface
 ```
 
 *Only available in PIP, not in Conda*
 
 # Usage
+
+### For 3 channels image (8-bit)
 ```python
 import mctthermalface
 from PIL import Image
 
-detector = ThermalFace.Detector('thermal_face_detection.pt')
-img = Image.open("img_path")
+detector = mctthermalface.Detector('thermal_face_detection.pt')
+img = Image.open("img_path.png")
 bbox = detector.detect(img)
 ```
 
+### Fpr 1 channels image (16-bit) stored in csv
+```python
+import mctthermalface
+import cv2
+import numpy as np
+
+detector = mctthermalface.Detector('thermal_face_detection.pt')
+
+img_1channel = np.loadtxt("img_path.csv", delimiter=",")
+img_1channel = cv2.normalize(img_1channel, None, 0, 255, cv2.NORM_MINMAX, cv2.CV_8U)
+bbox = detector.detect(img_1channel)
+```
+
+### Bounding Box Format
+
+```
+bbox = [xmax, xmin, ymax, ymin]
+```
+
 <br>
 
 # Model Download
 Click Here To Download [thermal_face_detection.pt](https://github.com/mctosima/MCTThermalFace/blob/master/thermal_face_detection.pt)
 
 <br>
```

#### html2text {}

```diff
@@ -1,16 +1,22 @@
     # Face Detection on Thermal Image [Python] [PyTorch] ![Sample](https://
-     raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample.png)
+   raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample_new.png)
 # Installation Before installing, make sure the following packages are
 available: - Numpy - PyTorch (I recommend to install your PyTorch from
 [following website](https://pytorch.org/)) - PIL - OpenCV To Install, run the
 following command: ```bash pip install mctthermalface ``` *Only available in
-PIP, not in Conda* # Usage ```python import mctthermalface from PIL import
-Image detector = ThermalFace.Detector('thermal_face_detection.pt') img =
-Image.open("img_path") bbox = detector.detect(img) ```
+PIP, not in Conda* # Usage ### For 3 channels image (8-bit) ```python import
+mctthermalface from PIL import Image detector = mctthermalface.Detector
+('thermal_face_detection.pt') img = Image.open("img_path.png") bbox =
+detector.detect(img) ``` ### Fpr 1 channels image (16-bit) stored in csv
+```python import mctthermalface import cv2 import numpy as np detector =
+mctthermalface.Detector('thermal_face_detection.pt') img_1channel = np.loadtxt
+("img_path.csv", delimiter=",") img_1channel = cv2.normalize(img_1channel,
+None, 0, 255, cv2.NORM_MINMAX, cv2.CV_8U) bbox = detector.detect(img_1channel)
+``` ### Bounding Box Format ``` bbox = [xmax, xmin, ymax, ymin] ```
 # Model Download Click Here To Download [thermal_face_detection.pt](https://
 github.com/mctosima/MCTThermalFace/blob/master/thermal_face_detection.pt)
 # Sample Usage Check this [notebook](https://github.com/mctosima/
 MCTThermalFace/blob/master/how_to_use.ipynb)
 # Credits Original Works by: Diza Febriyan Hasal on his Bachelor Thesis about
 Detecting Face in Thermal Image. Reworked by Martin Clinton Manullang to adjust
 the performance, adaptability, and compatibility (2023).
```

### Comparing `mctthermalface-0.2.0/mctthermalface/mctthermalface.py` & `mctthermalface-0.2.2/mctthermalface/mctthermalface.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,20 +30,24 @@
         self.model = torch.jit.load(model_path)
     
     def preprocess(self, img):
         if isinstance(img, Image.Image):
             img = np.array(img)
 
         self.original_shape = img.shape[:2]
-        img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+        
+        if len(img.shape) == 3 and img.shape[2] == 3:  # Check if the image has 3 channels
+            img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+            
         img = cv2.resize(img, (160, 160))
         img = torch.from_numpy(img).unsqueeze(0).float()
         img = img / 255.0
         return [img]
 
+
     def resize_bbox(self, bbox):
         scale_y, scale_x = np.array(self.original_shape) / np.array([160, 160])
         bbox = np.array(bbox)
         bbox[[0, 2]] = bbox[[0, 2]] * scale_x
         bbox[[1, 3]] = bbox[[1, 3]] * scale_y
         return bbox
```

### Comparing `mctthermalface-0.2.0/mctthermalface.egg-info/PKG-INFO` & `mctthermalface-0.2.2/mctthermalface.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctthermalface
-Version: 0.2.0
+Version: 0.2.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -12,15 +12,15 @@
 
 <div align="center">
 
 # Face Detection on Thermal Image
 <a href="https://www.python.org/"><img alt="Python" src="https://img.shields.io/badge/-Python 3.7+-blue?style=for-the-badge&logo=python&logoColor=white"></a>
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/-PyTorch 1.8+-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white"></a>
 
-![Sample](https://raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample.png)
+![Sample](https://raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample_new.png)
 
 <br>
 </div>
 
 # Installation
 
 Before installing, make sure the following packages are available:
@@ -33,23 +33,44 @@
 ```bash
 pip install mctthermalface
 ```
 
 *Only available in PIP, not in Conda*
 
 # Usage
+
+### For 3 channels image (8-bit)
 ```python
 import mctthermalface
 from PIL import Image
 
-detector = ThermalFace.Detector('thermal_face_detection.pt')
-img = Image.open("img_path")
+detector = mctthermalface.Detector('thermal_face_detection.pt')
+img = Image.open("img_path.png")
 bbox = detector.detect(img)
 ```
 
+### Fpr 1 channels image (16-bit) stored in csv
+```python
+import mctthermalface
+import cv2
+import numpy as np
+
+detector = mctthermalface.Detector('thermal_face_detection.pt')
+
+img_1channel = np.loadtxt("img_path.csv", delimiter=",")
+img_1channel = cv2.normalize(img_1channel, None, 0, 255, cv2.NORM_MINMAX, cv2.CV_8U)
+bbox = detector.detect(img_1channel)
+```
+
+### Bounding Box Format
+
+```
+bbox = [xmax, xmin, ymax, ymin]
+```
+
 <br>
 
 # Model Download
 Click Here To Download [thermal_face_detection.pt](https://github.com/mctosima/MCTThermalFace/blob/master/thermal_face_detection.pt)
 
 <br>
```

#### html2text {}

```diff
@@ -1,22 +1,28 @@
-Metadata-Version: 2.1 Name: mctthermalface Version: 0.2.0 Classifier:
+Metadata-Version: 2.1 Name: mctthermalface Version: 0.2.2 Classifier:
 Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown
     # Face Detection on Thermal Image [Python] [PyTorch] ![Sample](https://
-     raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample.png)
+   raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample_new.png)
 # Installation Before installing, make sure the following packages are
 available: - Numpy - PyTorch (I recommend to install your PyTorch from
 [following website](https://pytorch.org/)) - PIL - OpenCV To Install, run the
 following command: ```bash pip install mctthermalface ``` *Only available in
-PIP, not in Conda* # Usage ```python import mctthermalface from PIL import
-Image detector = ThermalFace.Detector('thermal_face_detection.pt') img =
-Image.open("img_path") bbox = detector.detect(img) ```
+PIP, not in Conda* # Usage ### For 3 channels image (8-bit) ```python import
+mctthermalface from PIL import Image detector = mctthermalface.Detector
+('thermal_face_detection.pt') img = Image.open("img_path.png") bbox =
+detector.detect(img) ``` ### Fpr 1 channels image (16-bit) stored in csv
+```python import mctthermalface import cv2 import numpy as np detector =
+mctthermalface.Detector('thermal_face_detection.pt') img_1channel = np.loadtxt
+("img_path.csv", delimiter=",") img_1channel = cv2.normalize(img_1channel,
+None, 0, 255, cv2.NORM_MINMAX, cv2.CV_8U) bbox = detector.detect(img_1channel)
+``` ### Bounding Box Format ``` bbox = [xmax, xmin, ymax, ymin] ```
 # Model Download Click Here To Download [thermal_face_detection.pt](https://
 github.com/mctosima/MCTThermalFace/blob/master/thermal_face_detection.pt)
 # Sample Usage Check this [notebook](https://github.com/mctosima/
 MCTThermalFace/blob/master/how_to_use.ipynb)
 # Credits Original Works by: Diza Febriyan Hasal on his Bachelor Thesis about
 Detecting Face in Thermal Image. Reworked by Martin Clinton Manullang to adjust
 the performance, adaptability, and compatibility (2023).
```

### Comparing `mctthermalface-0.2.0/setup.py` & `mctthermalface-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mctthermalface',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version='0.2.0',
+    version='0.2.2',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'torch',
         'torchvision',
         'opencv-python',
     ],
```

