# Comparing `tmp/webcam-0.9.tar.gz` & `tmp/webcam-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-0.9.tar", last modified: Mon May  8 12:05:00 2023, max compression
+gzip compressed data, was "webcam-1.0.tar", last modified: Mon May  8 13:09:06 2023, max compression
```

## Comparing `webcam-0.9.tar` & `webcam-1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 12:05:00.464250 webcam-0.9/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.9/LICENSE
--rw-rw-rw-   0        0        0     1311 2023-05-08 12:05:00.463251 webcam-0.9/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 12:05:00.464250 webcam-0.9/setup.cfg
--rw-rw-rw-   0        0        0     1309 2023-05-08 12:04:13.000000 webcam-0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 12:05:00.438249 webcam-0.9/webcam/
--rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-0.9/webcam/__init__.py
--rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-0.9/webcam/_video_webcam.py
--rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.9/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    13299 2023-05-08 12:04:13.000000 webcam-0.9/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-05-08 12:05:00.453257 webcam-0.9/webcam.egg-info/
--rw-rw-rw-   0        0        0     1311 2023-05-08 12:05:00.000000 webcam-0.9/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-08 12:05:00.000000 webcam-0.9/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 12:05:00.000000 webcam-0.9/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-08 12:05:00.000000 webcam-0.9/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-08 12:05:00.000000 webcam-0.9/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 13:09:06.753152 webcam-1.0/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-1.0/LICENSE
+-rw-rw-rw-   0        0        0     1323 2023-05-08 13:09:06.752111 webcam-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 13:09:06.753152 webcam-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1321 2023-05-08 13:09:03.000000 webcam-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:09:06.725807 webcam-1.0/webcam/
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-1.0/webcam/__init__.py
+-rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-1.0/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-1.0/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    13307 2023-05-08 13:07:07.000000 webcam-1.0/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:09:06.749101 webcam-1.0/webcam.egg-info/
+-rw-rw-rw-   0        0        0     1323 2023-05-08 13:09:06.000000 webcam-1.0/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-08 13:09:06.000000 webcam-1.0/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:09:06.000000 webcam-1.0/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-08 13:09:06.000000 webcam-1.0/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 13:09:06.000000 webcam-1.0/webcam.egg-info/top_level.txt
```

### Comparing `webcam-0.9/LICENSE` & `webcam-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-0.9/PKG-INFO` & `webcam-1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.9
+Version: 1.0
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Capture
```

### Comparing `webcam-0.9/setup.py` & `webcam-1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='0.9',
+    version='1.0',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
@@ -16,15 +16,15 @@
     install_requires=[
         'numpy',
         'opencv-python',
         'imutils'
     ],
 
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'Topic :: Multimedia :: Graphics',
         'Topic :: Multimedia :: Graphics :: Capture',
```

### Comparing `webcam-0.9/webcam/_video_webcam.py` & `webcam-1.0/webcam/_video_webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-0.9/webcam/_webcam_background.py` & `webcam-1.0/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-0.9/webcam/webcam.py` & `webcam-1.0/webcam/webcam.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self._background = run_in_background
         self.on_aspect_ratio_lost = on_aspect_ratio_lost
         # Initialize it for videos if the source is a string and a file exists at the path
         if isinstance(src, str) and os.path.isfile(src):
             self.cap = _VideoWebcam(video_path=src)
         # Otherwise assume it is a webcam (both webcam or RTSP stream)
         else:
-            self.cap = cv2.VideoCapture(src) if not run_in_background else _WebcamBackground(src=src)
+            self.cap = cv2.VideoCapture(src) if not run_in_background else _WebcamBackground(src=src).start()
         self.as_bgr = as_bgr
 
         # Calculate and set output frame size
         self.frame_size_hw = self._calculate_and_set_desired_resolution(h, w)
 
         # Set batch size and frame rate attributes
         self.batch_size = batch_size
```

### Comparing `webcam-0.9/webcam.egg-info/PKG-INFO` & `webcam-1.0/webcam.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.9
+Version: 1.0
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Capture
```

