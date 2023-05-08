# Comparing `tmp/synthesisai-0.4.0.tar.gz` & `tmp/synthesisai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthesisai-0.4.0.tar", last modified: Tue Mar 28 04:02:15 2023, max compression
+gzip compressed data, was "synthesisai-0.5.0.tar", last modified: Mon May  8 23:15:23 2023, max compression
```

## Comparing `synthesisai-0.4.0.tar` & `synthesisai-0.5.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-03-28 04:02:15.443807 synthesisai-0.4.0/
--rw-r--r--   0 anish      (501) staff       (20)     3591 2022-11-03 23:30:29.000000 synthesisai-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 anish      (501) staff       (20)     1071 2022-10-31 22:02:41.000000 synthesisai-0.4.0/LICENSE
--rw-r--r--   0 anish      (501) staff       (20)      242 2022-10-31 22:02:41.000000 synthesisai-0.4.0/MANIFEST.in
--rw-r--r--   0 anish      (501) staff       (20)     3250 2023-03-28 04:02:15.443922 synthesisai-0.4.0/PKG-INFO
--rw-r--r--   0 anish      (501) staff       (20)     2544 2023-01-19 17:24:14.000000 synthesisai-0.4.0/README.rst
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-03-28 04:02:15.438640 synthesisai-0.4.0/docs/
--rw-r--r--   0 anish      (501) staff       (20)      612 2022-11-04 03:04:02.000000 synthesisai-0.4.0/docs/Makefile
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-03-28 04:02:15.434603 synthesisai-0.4.0/docs/_build/
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-03-28 04:02:15.434646 synthesisai-0.4.0/docs/_build/html/
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-03-28 04:02:15.439492 synthesisai-0.4.0/docs/_build/html/_static/
--rw-r--r--   0 anish      (501) staff       (20)      286 2022-11-03 23:26:09.000000 synthesisai-0.4.0/docs/_build/html/_static/file.png
--rw-r--r--   0 anish      (501) staff       (20)       90 2022-11-03 23:26:09.000000 synthesisai-0.4.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 anish      (501) staff       (20)       90 2022-11-03 23:26:09.000000 synthesisai-0.4.0/docs/_build/html/_static/plus.png
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-03-28 04:02:15.440264 synthesisai-0.4.0/docs/_static/
--rw-r--r--   0 anish      (501) staff       (20)      286 2023-03-28 04:00:53.000000 synthesisai-0.4.0/docs/_static/file.png
--rw-r--r--   0 anish      (501) staff       (20)       90 2023-03-28 04:00:53.000000 synthesisai-0.4.0/docs/_static/minus.png
--rw-r--r--   0 anish      (501) staff       (20)       90 2023-03-28 04:00:53.000000 synthesisai-0.4.0/docs/_static/plus.png
--rwxr-xr-x   0 anish      (501) staff       (20)     4891 2022-12-22 00:54:59.000000 synthesisai-0.4.0/docs/conf.py
--rw-r--r--   0 anish      (501) staff       (20)       33 2022-10-31 22:02:41.000000 synthesisai-0.4.0/docs/contributing.rst
--rw-r--r--   0 anish      (501) staff       (20)      271 2022-11-04 04:17:08.000000 synthesisai-0.4.0/docs/index.rst
--rw-r--r--   0 anish      (501) staff       (20)     1178 2022-11-03 23:30:29.000000 synthesisai-0.4.0/docs/installation.rst
--rw-r--r--   0 anish      (501) staff       (20)      809 2022-10-31 22:02:41.000000 synthesisai-0.4.0/docs/make.bat
--rw-r--r--   0 anish      (501) staff       (20)       70 2023-03-28 04:00:50.000000 synthesisai-0.4.0/docs/modules.rst
--rw-r--r--   0 anish      (501) staff       (20)       27 2022-10-31 22:02:41.000000 synthesisai-0.4.0/docs/readme.rst
--rw-r--r--   0 anish      (501) staff       (20)     1319 2023-03-28 04:00:50.000000 synthesisai-0.4.0/docs/synthesisai.rst
--rw-r--r--   0 anish      (501) staff       (20)      383 2023-03-28 04:02:15.444316 synthesisai-0.4.0/setup.cfg
--rw-r--r--   0 anish      (501) staff       (20)     1285 2023-03-28 04:01:40.000000 synthesisai-0.4.0/setup.py
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-03-28 04:02:15.442538 synthesisai-0.4.0/synthesisai/
--rw-r--r--   0 anish      (501) staff       (20)      203 2023-03-28 04:01:40.000000 synthesisai-0.4.0/synthesisai/__init__.py
--rw-r--r--   0 anish      (501) staff       (20)      723 2022-12-22 00:54:59.000000 synthesisai-0.4.0/synthesisai/data_types.py
--rw-r--r--   0 anish      (501) staff       (20)    20951 2023-03-14 01:00:13.000000 synthesisai-0.4.0/synthesisai/dataset.py
--rw-r--r--   0 anish      (501) staff       (20)     2368 2022-11-02 12:43:53.000000 synthesisai-0.4.0/synthesisai/item_loader.py
--rw-r--r--   0 anish      (501) staff       (20)     2137 2022-12-22 00:54:59.000000 synthesisai-0.4.0/synthesisai/item_loader_factory.py
--rw-r--r--   0 anish      (501) staff       (20)    27966 2023-03-28 03:54:58.000000 synthesisai-0.4.0/synthesisai/item_loader_v1.py
--rw-r--r--   0 anish      (501) staff       (20)    25551 2023-03-28 03:53:36.000000 synthesisai-0.4.0/synthesisai/item_loader_v2.py
--rw-r--r--   0 anish      (501) staff       (20)    10096 2023-03-28 04:00:28.000000 synthesisai-0.4.0/synthesisai/modality.py
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-03-28 04:02:15.443316 synthesisai-0.4.0/synthesisai.egg-info/
--rw-r--r--   0 anish      (501) staff       (20)     3250 2023-03-28 04:02:15.000000 synthesisai-0.4.0/synthesisai.egg-info/PKG-INFO
--rw-r--r--   0 anish      (501) staff       (20)      861 2023-03-28 04:02:15.000000 synthesisai-0.4.0/synthesisai.egg-info/SOURCES.txt
--rw-r--r--   0 anish      (501) staff       (20)        1 2023-03-28 04:02:15.000000 synthesisai-0.4.0/synthesisai.egg-info/dependency_links.txt
--rw-r--r--   0 anish      (501) staff       (20)        1 2023-03-28 04:02:15.000000 synthesisai-0.4.0/synthesisai.egg-info/not-zip-safe
--rw-r--r--   0 anish      (501) staff       (20)      202 2023-03-28 04:02:15.000000 synthesisai-0.4.0/synthesisai.egg-info/requires.txt
--rw-r--r--   0 anish      (501) staff       (20)       12 2023-03-28 04:02:15.000000 synthesisai-0.4.0/synthesisai.egg-info/top_level.txt
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-03-28 04:02:15.443556 synthesisai-0.4.0/tests/
--rw-r--r--   0 anish      (501) staff       (20)       41 2022-10-31 22:02:41.000000 synthesisai-0.4.0/tests/__init__.py
--rw-r--r--   0 anish      (501) staff       (20)      407 2022-10-31 22:02:41.000000 synthesisai-0.4.0/tests/test_synthesisai.py
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-08 23:15:23.765958 synthesisai-0.5.0/
+-rw-r--r--   0 anish      (501) staff       (20)     3591 2022-11-03 23:30:29.000000 synthesisai-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 anish      (501) staff       (20)     1071 2022-10-31 22:02:41.000000 synthesisai-0.5.0/LICENSE
+-rw-r--r--   0 anish      (501) staff       (20)      242 2022-10-31 22:02:41.000000 synthesisai-0.5.0/MANIFEST.in
+-rw-r--r--   0 anish      (501) staff       (20)     3250 2023-05-08 23:15:23.766023 synthesisai-0.5.0/PKG-INFO
+-rw-r--r--   0 anish      (501) staff       (20)     2544 2023-01-19 17:24:14.000000 synthesisai-0.5.0/README.rst
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-08 23:15:23.761940 synthesisai-0.5.0/docs/
+-rw-r--r--   0 anish      (501) staff       (20)      612 2022-11-04 03:04:02.000000 synthesisai-0.5.0/docs/Makefile
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-08 23:15:23.759214 synthesisai-0.5.0/docs/_build/
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-08 23:15:23.759257 synthesisai-0.5.0/docs/_build/html/
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-08 23:15:23.762618 synthesisai-0.5.0/docs/_build/html/_static/
+-rw-r--r--   0 anish      (501) staff       (20)      286 2022-11-03 23:26:09.000000 synthesisai-0.5.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 anish      (501) staff       (20)       90 2022-11-03 23:26:09.000000 synthesisai-0.5.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 anish      (501) staff       (20)       90 2022-11-03 23:26:09.000000 synthesisai-0.5.0/docs/_build/html/_static/plus.png
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-08 23:15:23.763697 synthesisai-0.5.0/docs/_static/
+-rw-r--r--   0 anish      (501) staff       (20)      286 2023-03-28 04:00:53.000000 synthesisai-0.5.0/docs/_static/file.png
+-rw-r--r--   0 anish      (501) staff       (20)       90 2023-03-28 04:00:53.000000 synthesisai-0.5.0/docs/_static/minus.png
+-rw-r--r--   0 anish      (501) staff       (20)       90 2023-03-28 04:00:53.000000 synthesisai-0.5.0/docs/_static/plus.png
+-rwxr-xr-x   0 anish      (501) staff       (20)     4891 2022-12-22 00:54:59.000000 synthesisai-0.5.0/docs/conf.py
+-rw-r--r--   0 anish      (501) staff       (20)       33 2022-10-31 22:02:41.000000 synthesisai-0.5.0/docs/contributing.rst
+-rw-r--r--   0 anish      (501) staff       (20)      271 2022-11-04 04:17:08.000000 synthesisai-0.5.0/docs/index.rst
+-rw-r--r--   0 anish      (501) staff       (20)     1178 2022-11-03 23:30:29.000000 synthesisai-0.5.0/docs/installation.rst
+-rw-r--r--   0 anish      (501) staff       (20)      809 2022-10-31 22:02:41.000000 synthesisai-0.5.0/docs/make.bat
+-rw-r--r--   0 anish      (501) staff       (20)       70 2023-03-28 04:00:50.000000 synthesisai-0.5.0/docs/modules.rst
+-rw-r--r--   0 anish      (501) staff       (20)       27 2022-10-31 22:02:41.000000 synthesisai-0.5.0/docs/readme.rst
+-rw-r--r--   0 anish      (501) staff       (20)     1319 2023-03-28 04:00:50.000000 synthesisai-0.5.0/docs/synthesisai.rst
+-rw-r--r--   0 anish      (501) staff       (20)      383 2023-05-08 23:15:23.766293 synthesisai-0.5.0/setup.cfg
+-rw-r--r--   0 anish      (501) staff       (20)     1285 2023-05-08 23:14:20.000000 synthesisai-0.5.0/setup.py
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-08 23:15:23.764759 synthesisai-0.5.0/synthesisai/
+-rw-r--r--   0 anish      (501) staff       (20)      203 2023-05-08 23:14:20.000000 synthesisai-0.5.0/synthesisai/__init__.py
+-rw-r--r--   0 anish      (501) staff       (20)      723 2022-12-22 00:54:59.000000 synthesisai-0.5.0/synthesisai/data_types.py
+-rw-r--r--   0 anish      (501) staff       (20)    21006 2023-05-08 23:10:43.000000 synthesisai-0.5.0/synthesisai/dataset.py
+-rw-r--r--   0 anish      (501) staff       (20)     2368 2022-11-02 12:43:53.000000 synthesisai-0.5.0/synthesisai/item_loader.py
+-rw-r--r--   0 anish      (501) staff       (20)     2137 2022-12-22 00:54:59.000000 synthesisai-0.5.0/synthesisai/item_loader_factory.py
+-rw-r--r--   0 anish      (501) staff       (20)    28065 2023-03-28 05:18:14.000000 synthesisai-0.5.0/synthesisai/item_loader_v1.py
+-rw-r--r--   0 anish      (501) staff       (20)    25551 2023-03-28 03:53:36.000000 synthesisai-0.5.0/synthesisai/item_loader_v2.py
+-rw-r--r--   0 anish      (501) staff       (20)    10096 2023-03-28 04:00:28.000000 synthesisai-0.5.0/synthesisai/modality.py
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-08 23:15:23.765434 synthesisai-0.5.0/synthesisai.egg-info/
+-rw-r--r--   0 anish      (501) staff       (20)     3250 2023-05-08 23:15:23.000000 synthesisai-0.5.0/synthesisai.egg-info/PKG-INFO
+-rw-r--r--   0 anish      (501) staff       (20)      861 2023-05-08 23:15:23.000000 synthesisai-0.5.0/synthesisai.egg-info/SOURCES.txt
+-rw-r--r--   0 anish      (501) staff       (20)        1 2023-05-08 23:15:23.000000 synthesisai-0.5.0/synthesisai.egg-info/dependency_links.txt
+-rw-r--r--   0 anish      (501) staff       (20)        1 2023-05-08 23:15:23.000000 synthesisai-0.5.0/synthesisai.egg-info/not-zip-safe
+-rw-r--r--   0 anish      (501) staff       (20)      202 2023-05-08 23:15:23.000000 synthesisai-0.5.0/synthesisai.egg-info/requires.txt
+-rw-r--r--   0 anish      (501) staff       (20)       12 2023-05-08 23:15:23.000000 synthesisai-0.5.0/synthesisai.egg-info/top_level.txt
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-08 23:15:23.765844 synthesisai-0.5.0/tests/
+-rw-r--r--   0 anish      (501) staff       (20)       41 2022-10-31 22:02:41.000000 synthesisai-0.5.0/tests/__init__.py
+-rw-r--r--   0 anish      (501) staff       (20)      407 2022-10-31 22:02:41.000000 synthesisai-0.5.0/tests/test_synthesisai.py
```

### Comparing `synthesisai-0.4.0/CONTRIBUTING.rst` & `synthesisai-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `synthesisai-0.4.0/LICENSE` & `synthesisai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synthesisai-0.4.0/PKG-INFO` & `synthesisai-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthesisai
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python library for loading synthetic data for ML use cases
 Home-page: https://github.com/Synthesis-AI-Dev/synthesisai
 Author: Synthesis AI
 Author-email: anish@synthesis.ai
 License: MIT license
 Keywords: synthesisai
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `synthesisai-0.4.0/README.rst` & `synthesisai-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `synthesisai-0.4.0/docs/Makefile` & `synthesisai-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `synthesisai-0.4.0/docs/conf.py` & `synthesisai-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `synthesisai-0.4.0/docs/installation.rst` & `synthesisai-0.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `synthesisai-0.4.0/docs/make.bat` & `synthesisai-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `synthesisai-0.4.0/docs/synthesisai.rst` & `synthesisai-0.5.0/docs/synthesisai.rst`

 * *Files identical despite different names*

### Comparing `synthesisai-0.4.0/setup.py` & `synthesisai-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,10 +33,10 @@
     include_package_data=True,
     keywords="synthesisai",
     name="synthesisai",
     packages=find_packages(include=["synthesisai", "synthesisai.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/Synthesis-AI-Dev/synthesisai",
-    version='0.4.0',
+    version='0.5.0',
     zip_safe=False,
 )
```

### Comparing `synthesisai-0.4.0/synthesisai/data_types.py` & `synthesisai-0.5.0/synthesisai/data_types.py`

 * *Files identical despite different names*

### Comparing `synthesisai-0.4.0/synthesisai/dataset.py` & `synthesisai-0.5.0/synthesisai/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,105 +109,107 @@
         # eyes
         "caruncle_left": 28,
         "caruncle_right": 29,
         "eyebrow_left": 30,
         "eyebrow_right": 31,
         "eyelashes_left": 32,
         "eyelashes_right": 33,
-        "eye_fluid": 34,
-        "iris_left": 35,
-        "iris_right": 36,
-        "lower_eyelid_left": 37,
-        "lower_eyelid_right": 38,
-        "pupil_left": 39,
-        "pupil_right": 40,
-        "sclera_left": 41,
-        "sclera_right": 42,
-        "upper_eyelid_left": 43,
-        "upper_eyelid_right": 44,
+        "eye_fluid_left": 34,
+        "eye_fluid_right": 35,
+        "iris_left": 36,
+        "iris_right": 37,
+        "lower_eyelid_left": 38,
+        "lower_eyelid_right": 39,
+        "pupil_left": 40,
+        "pupil_right": 41,
+        "sclera_left": 42,
+        "sclera_right": 43,
+        "upper_eyelid_left": 44,
+        "upper_eyelid_right": 45,
         # torso
-        "shoulders": 45,
-        "torso_lower_left": 46,
-        "torso_lower_right": 47,
-        "torso_mid_left": 48,
-        "torso_mid_right": 49,
-        "torso_upper_left": 50,
-        "torso_upper_right": 51,
+        "shoulders": 46,
+        "torso_lower_left": 47,
+        "torso_lower_right": 48,
+        "torso_mid_left": 49,
+        "torso_mid_right": 50,
+        "torso_upper_left": 51,
+        "torso_upper_right": 52,
         # arms
-        "arm_lower_left": 52,
-        "arm_lower_right": 53,
-        "arm_upper_left": 54,
-        "arm_upper_right": 55,
+        "arm_lower_left": 53,
+        "arm_lower_right": 54,
+        "arm_upper_left": 55,
+        "arm_upper_right": 56,
         # hands
-        "finger1_mid_bottom_left": 56,
-        "finger1_mid_bottom_right": 57,
-        "finger1_mid_left": 58,
-        "finger1_mid_right": 59,
-        "finger1_mid_top_left": 60,
-        "finger1_mid_top_right": 61,
-        "finger2_mid_bottom_left": 62,
-        "finger2_mid_bottom_right": 63,
-        "finger2_mid_left": 64,
-        "finger2_mid_right": 65,
-        "finger2_mid_top_left": 66,
-        "finger2_mid_top_right": 67,
-        "finger3_mid_bottom_left": 68,
-        "finger3_mid_bottom_right": 69,
-        "finger3_mid_left": 70,
-        "finger3_mid_right": 71,
-        "finger3_mid_top_left": 72,
-        "finger3_mid_top_right": 73,
-        "finger4_mid_bottom_left": 74,
-        "finger4_mid_bottom_right": 75,
-        "finger4_mid_left": 76,
-        "finger4_mid_right": 77,
-        "finger4_mid_top_left": 78,
-        "finger4_mid_top_right": 79,
-        "finger5_mid_bottom_left": 80,
-        "finger5_mid_bottom_right": 81,
-        "finger5_mid_left": 82,
-        "finger5_mid_right": 83,
-        "finger5_mid_top_left": 84,
-        "finger5_mid_top_right": 85,
-        "hand_left": 86,
-        "hand_right": 87,
-        "nails_left": 88,
-        "nails_right": 89,
+        "finger1_mid_bottom_left": 57,
+        "finger1_mid_bottom_right": 58,
+        "finger1_mid_left": 59,
+        "finger1_mid_right": 60,
+        "finger1_mid_top_left": 61,
+        "finger1_mid_top_right": 62,
+        "finger2_mid_bottom_left": 63,
+        "finger2_mid_bottom_right": 64,
+        "finger2_mid_left": 65,
+        "finger2_mid_right": 66,
+        "finger2_mid_top_left": 67,
+        "finger2_mid_top_right": 68,
+        "finger3_mid_bottom_left": 69,
+        "finger3_mid_bottom_right": 70,
+        "finger3_mid_left": 71,
+        "finger3_mid_right": 72,
+        "finger3_mid_top_left": 73,
+        "finger3_mid_top_right": 74,
+        "finger4_mid_bottom_left": 75,
+        "finger4_mid_bottom_right": 76,
+        "finger4_mid_left": 77,
+        "finger4_mid_right": 78,
+        "finger4_mid_top_left": 79,
+        "finger4_mid_top_right": 80,
+        "finger5_mid_bottom_left": 81,
+        "finger5_mid_bottom_right": 82,
+        "finger5_mid_left": 83,
+        "finger5_mid_right": 84,
+        "finger5_mid_top_left": 85,
+        "finger5_mid_top_right": 86,
+        "hand_left": 87,
+        "hand_right": 88,
+        "nails_left": 89,
+        "nails_right": 90,
         # legs
-        "foot_left": 90,
-        "foot_right": 91,
-        "leg_lower_left": 92,
-        "leg_lower_right": 93,
-        "leg_upper_left": 94,
-        "leg_upper_right": 95,
+        "foot_left": 91,
+        "foot_right": 92,
+        "leg_lower_left": 93,
+        "leg_lower_right": 94,
+        "leg_upper_left": 95,
+        "leg_upper_right": 96,
         # accessories
-        "glasses_frame": 96,
-        "glasses_lens_left": 97,
-        "glasses_lens_right": 98,
-        "headphones": 99,
-        "headwear": 100,
-        "mask": 101,
+        "glasses_frame": 97,
+        "glasses_lens_left": 98,
+        "glasses_lens_right": 99,
+        "headphones": 100,
+        "headwear": 101,
+        "mask": 102,
         # below are old classes that shouldn't exist anymore
         # keeping these around to support older datasets
-        "body": 102,
-        "clothing": 103,
-        "cornea_left": 104,
-        "cornea_right": 105,
-        "eyebrows": 106,
-        "eyelashes": 107,
-        "eyelid": 108,
-        "eyes": 109,
-        "eyelid_left": 110,
-        "eyelid_right": 111,
-        "eye_left": 112,
-        "eye_right": 113,
-        "glasses": 114,
-        "undereye_left": 115,
-        "undereye_right": 116,
-        "undereye": 117,        
+        "body": 103,
+        "clothing": 104,
+        "cornea_left": 105,
+        "cornea_right": 106,
+        "eyebrows": 107,
+        "eyelashes": 108,
+        "eyelid": 109,
+        "eyes": 110,
+        "eyelid_left": 111,
+        "eyelid_right": 112,
+        "eye_fluid": 113,
+        "eye_left": 114,
+        "eye_right": 115,
+        "glasses": 116,
+        "undereye_left": 117,
+        "undereye_right": 118,
+        "undereye": 119,
     }
     """
     Default body segmentation mapping.
     """
 
     CLOTHING_SEGMENTATION_MAPPING = {
         "default": 0,
```

### Comparing `synthesisai-0.4.0/synthesisai/item_loader.py` & `synthesisai-0.5.0/synthesisai/item_loader.py`

 * *Files identical despite different names*

### Comparing `synthesisai-0.4.0/synthesisai/item_loader_factory.py` & `synthesisai-0.5.0/synthesisai/item_loader_factory.py`

 * *Files identical despite different names*

### Comparing `synthesisai-0.4.0/synthesisai/item_loader_v1.py` & `synthesisai-0.5.0/synthesisai/item_loader_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,15 +351,18 @@
             }
 
             # v1 only has one character with ID 1
             gaze = {"human_1": gaze}
             return gaze
         
         if modality == Modality.GAZE_TARGET:
-            target = info["gaze_target"]["target_name"]
+            target = info.get("gaze_target", None)
+            if target is None:
+                return target
+            target = target["target_name"]
 
             # v1 only has one character with ID 1
             target = {"human_1": target}
             return target
 
         if modality == Modality.HEAD_TURN:
             head_turn = info["facial_attributes"]["head_turn"]
```

### Comparing `synthesisai-0.4.0/synthesisai/item_loader_v2.py` & `synthesisai-0.5.0/synthesisai/item_loader_v2.py`

 * *Files identical despite different names*

### Comparing `synthesisai-0.4.0/synthesisai/modality.py` & `synthesisai-0.5.0/synthesisai/modality.py`

 * *Files identical despite different names*

### Comparing `synthesisai-0.4.0/synthesisai.egg-info/PKG-INFO` & `synthesisai-0.5.0/synthesisai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthesisai
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python library for loading synthetic data for ML use cases
 Home-page: https://github.com/Synthesis-AI-Dev/synthesisai
 Author: Synthesis AI
 Author-email: anish@synthesis.ai
 License: MIT license
 Keywords: synthesisai
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `synthesisai-0.4.0/synthesisai.egg-info/SOURCES.txt` & `synthesisai-0.5.0/synthesisai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

