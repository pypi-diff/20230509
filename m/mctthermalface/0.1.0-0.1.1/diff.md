# Comparing `tmp/mctthermalface-0.1.0.tar.gz` & `tmp/mctthermalface-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctthermalface-0.1.0.tar", last modified: Tue May  9 01:20:23 2023, max compression
+gzip compressed data, was "mctthermalface-0.1.1.tar", last modified: Tue May  9 01:33:25 2023, max compression
```

## Comparing `mctthermalface-0.1.0.tar` & `mctthermalface-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:20:23.792504 mctthermalface-0.1.0/
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1940 2023-05-09 01:20:23.792504 mctthermalface-0.1.0/PKG-INFO
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1497 2023-05-08 08:56:05.000000 mctthermalface-0.1.0/README.md
-drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:20:23.792504 mctthermalface-0.1.0/mctthermalface.egg-info/
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1940 2023-05-09 01:20:23.000000 mctthermalface-0.1.0/mctthermalface.egg-info/PKG-INFO
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      207 2023-05-09 01:20:23.000000 mctthermalface-0.1.0/mctthermalface.egg-info/SOURCES.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)        1 2023-05-09 01:20:23.000000 mctthermalface-0.1.0/mctthermalface.egg-info/dependency_links.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-09 01:20:23.000000 mctthermalface-0.1.0/mctthermalface.egg-info/requires.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)        1 2023-05-09 01:20:23.000000 mctthermalface-0.1.0/mctthermalface.egg-info/top_level.txt
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-09 01:20:23.792504 mctthermalface-0.1.0/setup.cfg
--rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      782 2023-05-09 01:20:14.000000 mctthermalface-0.1.0/setup.py
+drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:33:25.353996 mctthermalface-0.1.1/
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1940 2023-05-09 01:33:25.353996 mctthermalface-0.1.1/PKG-INFO
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1497 2023-05-08 08:56:05.000000 mctthermalface-0.1.1/README.md
+drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:33:25.353996 mctthermalface-0.1.1/mctthermalface/
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:32:50.000000 mctthermalface-0.1.1/mctthermalface/__init__.py
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     2010 2023-05-08 08:48:44.000000 mctthermalface-0.1.1/mctthermalface/mctthermalface.py
+drwxrwxr-x   0 bestlabmct  (1000) bestlabmct  (1000)        0 2023-05-09 01:33:25.353996 mctthermalface-0.1.1/mctthermalface.egg-info/
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)     1940 2023-05-09 01:33:25.000000 mctthermalface-0.1.1/mctthermalface.egg-info/PKG-INFO
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      267 2023-05-09 01:33:25.000000 mctthermalface-0.1.1/mctthermalface.egg-info/SOURCES.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)        1 2023-05-09 01:33:25.000000 mctthermalface-0.1.1/mctthermalface.egg-info/dependency_links.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-09 01:33:25.000000 mctthermalface-0.1.1/mctthermalface.egg-info/requires.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       15 2023-05-09 01:33:25.000000 mctthermalface-0.1.1/mctthermalface.egg-info/top_level.txt
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)       38 2023-05-09 01:33:25.353996 mctthermalface-0.1.1/setup.cfg
+-rw-rw-r--   0 bestlabmct  (1000) bestlabmct  (1000)      782 2023-05-09 01:33:14.000000 mctthermalface-0.1.1/setup.py
```

### Comparing `mctthermalface-0.1.0/PKG-INFO` & `mctthermalface-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctthermalface
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mctthermalface Version: 0.1.0 Classifier:
+Metadata-Version: 2.1 Name: mctthermalface Version: 0.1.1 Classifier:
 Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown
     # Face Detection on Thermal Image [Python] [PyTorch] ![Sample](https://
      raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample.png)
```

### Comparing `mctthermalface-0.1.0/README.md` & `mctthermalface-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mctthermalface-0.1.0/mctthermalface.egg-info/PKG-INFO` & `mctthermalface-0.1.1/mctthermalface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctthermalface
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mctthermalface Version: 0.1.0 Classifier:
+Metadata-Version: 2.1 Name: mctthermalface Version: 0.1.1 Classifier:
 Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown
     # Face Detection on Thermal Image [Python] [PyTorch] ![Sample](https://
      raw.githubusercontent.com/mctosima/MCTThermalFace/master/sample.png)
```

### Comparing `mctthermalface-0.1.0/setup.py` & `mctthermalface-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mctthermalface',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'torch',
         'torchvision',
         'opencv-python',
     ],
```

