# Comparing `tmp/sports2d-0.0.9.tar.gz` & `tmp/sports2d-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports2d-0.0.9.tar", last modified: Sun May  7 09:28:54 2023, max compression
+gzip compressed data, was "sports2d-0.1.0.tar", last modified: Tue May  9 15:10:26 2023, max compression
```

## Comparing `sports2d-0.0.9.tar` & `sports2d-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:28:54.448033 sports2d-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-07 09:28:40.000000 sports2d-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-05-07 09:28:54.448033 sports2d-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-05-07 09:28:40.000000 sports2d-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:28:54.444033 sports2d-0.0.9/Sports2D/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:28:54.444033 sports2d-0.0.9/Sports2D/Demo/
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Demo/Config_demo.toml
--rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Demo/demo.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Sports2D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:28:54.448033 sports2d-0.0.9/Sports2D/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Utilities/Blazepose_runsave.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Utilities/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Utilities/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Utilities/skeletons.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Utilities/test_with_blazepose.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/compute_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    23724 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/detect_pose.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-07 09:28:40.000000 sports2d-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-07 09:28:54.452033 sports2d-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 09:28:40.000000 sports2d-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:28:54.448033 sports2d-0.0.9/sports2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-05-07 09:28:54.000000 sports2d-0.0.9/sports2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-07 09:28:54.000000 sports2d-0.0.9/sports2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:28:54.000000 sports2d-0.0.9/sports2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:28:54.000000 sports2d-0.0.9/sports2d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-07 09:28:54.000000 sports2d-0.0.9/sports2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-07 09:28:54.000000 sports2d-0.0.9/sports2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:26.635247 sports2d-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-09 15:10:16.000000 sports2d-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-09 15:10:26.635247 sports2d-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12773 2023-05-09 15:10:16.000000 sports2d-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:26.631247 sports2d-0.1.0/Sports2D/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:26.631247 sports2d-0.1.0/Sports2D/Demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Demo/Config_demo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Demo/demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Sports2D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:26.635247 sports2d-0.1.0/Sports2D/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Utilities/Blazepose_runsave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Utilities/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Utilities/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Utilities/skeletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Utilities/test_with_blazepose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/compute_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23753 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/detect_pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-09 15:10:16.000000 sports2d-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-09 15:10:26.635247 sports2d-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-09 15:10:16.000000 sports2d-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:26.635247 sports2d-0.1.0/sports2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-09 15:10:26.000000 sports2d-0.1.0/sports2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-09 15:10:26.000000 sports2d-0.1.0/sports2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:10:26.000000 sports2d-0.1.0/sports2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:10:26.000000 sports2d-0.1.0/sports2d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 15:10:26.000000 sports2d-0.1.0/sports2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 15:10:26.000000 sports2d-0.1.0/sports2d.egg-info/top_level.txt
```

### Comparing `sports2d-0.0.9/LICENSE` & `sports2d-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.9/PKG-INFO` & `sports2d-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.0.9
+Version: 0.1.0
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
@@ -24,15 +24,17 @@
 Requires-Python: <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D)\
-[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\
+[![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+[![DOI](https://zenodo.org/badge/634044634.svg)](https://zenodo.org/badge/latestdoi/634044634)\
 <a href="https://colab.research.google.com/github/davidpagnon/Sports2D/blob/main/Sports2D/Sports2D.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 <!-- [![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
 [![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
 [![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
 [![DOI](https://zenodo.org/badge/501642916.svg)](https://zenodo.org/badge/latestdoi/501642916)
@@ -77,15 +79,15 @@
     pip install sports2d
     ```
 
 - OPTION 2: **Safer install with Anaconda**\
     Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):\
     Open an Anaconda prompt and create a virtual environment by typing:
     ```
-    conda create -n Sports2D python<=3.10 
+    conda create -n Sports2D python=3.10 -y
     conda activate Sports2D
     pip install sports2d
     ```
 
 - OPTION 3: **Build from source and test the last changes**\
      Open a terminal in the directory of your choice and clone the Sports2D repository.
      ```
@@ -190,20 +192,20 @@
 
 ### How it works
 
 #### Pose detection:
 
 BlazePose or OpenPose are used to detect joint centers from a video.
 
-If `BlazePose` is used, only one person can be detected.\
-No interpolation nor filtering options are available. Not plotting available.
+- If `BlazePose` is used, only one person can be detected.\
+  No interpolation nor filtering options are available. Not plotting available.
 
-If `OpenPose` is used, multiple persons can be consistently detected across frames. A person is matched to another in the next frame when their average point clouds are at a small euclidian distance.\
-Sequences of missing data are interpolated if they are less than N frames long.\
-Resulting coordinates can be filtered with Butterworth, gaussian, median, or loess filter. They can also be plotted.
+- If `OpenPose` is used, multiple persons can be consistently detected across frames. A person is matched to another in the next frame when their average point clouds are at a small euclidian distance.\
+  Sequences of missing data are interpolated if they are less than N frames long.\
+  Resulting coordinates can be filtered with Butterworth, gaussian, median, or loess filter. They can also be plotted.
 
 
 #### Angle computation:
 
 Joint and segment angles are computed from csv position files.\
 If a person suddently faces the other way, this change of direction is taken into account.\
 Resulting angles can be filtered in the same way as point coordinates, and they can also be plotted.
@@ -229,35 +231,38 @@
 ### How to cite
 If you use this code or data, please cite [Pagnon, 2023].
 
      @misc{Pagnon2023,
        author = {Pagnon, David},
        title = {Sports2D - Angles from video},
        year = {2023},
+       doi= {10.5281/zenodo.7903963},
        publisher = {GitHub},
        journal = {GitHub repository},
        howpublished = {\url{https://github.com/davidpagnon/Sports2D}},
      }
 
 ### How to contribute
 I would happily welcome any proposal for new features, code improvement, and more!\
 If you want to contribute to Sports2D, please follow [this guide](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) on how to fork, modify and push code, and submit a pull request. I would appreciate it if you provided as much useful information as possible about how you modified the code, and a rationale for why you're making this pull request. Please also specify on which operating system and on which python version you have tested the code.
 
 *Here is a to-do list: feel free to complete it:*
-- [x] Compute **segment angles**
-- [x] **Multi-person** detection, consistent over time
-- [x] **Only interpolate small gaps**
-- [x] **Filtering and plotting tools**
-- [x] Handle sudden **changes of direction**
-- [x] **Colab version** for those who cannot install OpenPose
-- [ ] Full test on **MacOS**
-- [ ] **GUI applications** for Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with [Kivy](https://kivy.org)
-- [ ] **Pose refinement**. Click and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/watch?v=bEuBKB7eqmk) for inspiration
+- [x] Compute **segment angles**.
+- [x] **Multi-person** detection, consistent over time.
+- [x] **Only interpolate small gaps**.
+- [x] **Filtering and plotting tools**.
+- [x] Handle sudden **changes of direction**.
+- [x] **Colab version** for those who cannot install OpenPose.
+- [ ] Full test on **MacOS**.
+- [ ] **GUI applications** for Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with [Kivy](https://kivy.org).
 - [ ] **Include OpenPose** in Sports2D executable files. [Dockerize](https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile) it? 
+- [ ] **Track other points and angles** with classic tracking methods (cf. [Kinovea](https://www.kinovea.org/features.html)), or by training a model (cf. [DeepLabCut](https://deeplabcut.github.io/DeepLabCut/README.html)).
+- [ ] **Pose refinement**. Click and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/watch?v=bEuBKB7eqmk) for inspiration.
 - [ ] **Constrain points** to OpenSim skeletal model for better angle estimation (like with [Pose2Sim](https://github.com/perfanalytics/pose2sim), but in 2D.
+- [ ] Add tools for annotating images, undistort them, take perspective into account, etc. (cf. [Kinovea](https://www.kinovea.org/features.html)).
 
 BSD 3-Clause License
 
 Copyright (c) 2022, perfanalytics
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sports2d Version: 0.0.9 Summary: Detect pose and
+Metadata-Version: 2.1 Name: sports2d Version: 0.1.0 Summary: Detect pose and
 compute 2D joint angles from a video. Home-page: https://github.com/
 davidpagnon/Sports2D Author: David Pagnon Author-email: contact@david-
 pagnon.com License: BSD 3-Clause License Project-URL: Bug Tracker, https://
 github.com/davidpagnon/Sports2D/issues Keywords:
 markerless,kinematics,OpenPose,BlazePose,joint
 angles,2D,biomechanics,sports,sports-analytics Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Development Status :: 3 - Alpha
@@ -14,52 +14,56 @@
 Engineering :: Medical Science Apps. Classifier: Topic :: Multimedia ::
 Graphics Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling Requires-
 Python: <3.11 Description-Content-Type: text/markdown License-File: LICENSE [!
 [Continuous integration](https://github.com/davidpagnon/sports2d/actions/
 workflows/continuous-integration.yml/badge.svg?branch=main)](https://
 github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/
-py/Sports2D)\ [![License](https://img.shields.io/badge/License-BSD_3--Clause-
-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\ [Open_In_Colab]  #
-Sports2D **`Sports2D` lets you compute 2D joint and segment angles from a
-video.** [Content/demo_gif.gif] `Warning:` Angle estimation is only as good as
-the pose estimation algorithm, i.e., it is not perfect.\ `Warning:` Results are
-acceptable only if the persons move in the 2D plane, from right to left or from
-left to right.\ If you need research-grade markerless joint kinematics,
-consider using several cameras, and constraining angles to a biomechanically
-accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for
-example. `Know issue`: Results won't be good with some iPhone videos in
-portrait mode. This is solved by priorly converting them with `ffmpeg -
-i video_input.mov video_output.mp4`, or even more simply with any random online
-video converter such as https://video-converter.com. `Announcement:` Apps with
-GUI will soon be released for Windows, Linux, MacOS, as well as Android and
-iOS. Mobile versions will only support simple exploratory analysis. This
-involves single-person angle computation, in a potentially less accurate and
-tunable way. ## Contents 1. [Installation and Demonstration](#installation-and-
-demonstration) 1. [Installation](#installation) 2. [Demonstration: Detect pose
-and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles) 2. [Go
-further](#go-further) 1. [Use on your own videos](#use-on-your-own-videos) 2.
-[Use OpenPose for multi-person, more accurate analysis](#use-openpose-for-
-multi-person-more-accurate-analysis) 3. [Advanced-settings](#advanced-settings)
-4. [How it works](#how-it-works) 3. [How to cite and how to contribute](#how-
-to-cite-and-how-to-contribute) ## Installation and Demonstration ###
-Installation - OPTION 1: **Quick install** \ Open a terminal. Type `python -V`
-to make sure python '>=3.7 <=3.10' is installed, and then: ``` pip install
-sports2d ``` - OPTION 2: **Safer install with Anaconda**\ Install [Miniconda]
-(https://docs.conda.io/en/latest/miniconda.html):\ Open an Anaconda prompt and
-create a virtual environment by typing: ``` conda create -n Sports2D
-python<=3.10 conda activate Sports2D pip install sports2d ``` - OPTION 3:
-**Build from source and test the last changes**\ Open a terminal in the
-directory of your choice and clone the Sports2D repository. ``` git clone
-https://github.com/davidpagnon/sports2d.git cd sports2d pip install . ``` ###
-Demonstration: Detect pose and compute 2D angles Open a terminal, enter `pip
-show sports2d`, check sports2d package location. \ Copy this path and go to the
-Demo folder by typing `cd \Sports2D\Demo`. \ Type `ipython`, and test the
-following code: ``` from Sports2D import Sports2D Sports2D.detect_pose
-('Config_demo.toml') Sports2D.compute_angles('Config_demo.toml') ``` [Content/
+py/Sports2D)\ [![Open Source? Yes!](https://badgen.net/badge/
+Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/
+badges/) [![License](https://img.shields.io/badge/License-BSD_3--Clause-
+blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![DOI](https://
+zenodo.org/badge/634044634.svg)](https://zenodo.org/badge/latestdoi/634044634)\
+[Open_In_Colab]  # Sports2D **`Sports2D` lets you compute 2D joint and segment
+angles from a video.** [Content/demo_gif.gif] `Warning:` Angle estimation is
+only as good as the pose estimation algorithm, i.e., it is not perfect.\
+`Warning:` Results are acceptable only if the persons move in the 2D plane,
+from right to left or from left to right.\ If you need research-grade
+markerless joint kinematics, consider using several cameras, and constraining
+angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/
+perfanalytics/pose2sim) for example. `Know issue`: Results won't be good with
+some iPhone videos in portrait mode. This is solved by priorly converting them
+with `ffmpeg -i video_input.mov video_output.mp4`, or even more simply with any
+random online video converter such as https://video-converter.com.
+`Announcement:` Apps with GUI will soon be released for Windows, Linux, MacOS,
+as well as Android and iOS. Mobile versions will only support simple
+exploratory analysis. This involves single-person angle computation, in a
+potentially less accurate and tunable way. ## Contents 1. [Installation and
+Demonstration](#installation-and-demonstration) 1. [Installation]
+(#installation) 2. [Demonstration: Detect pose and compute 2D angles]
+(#demonstration-detect-pose-and-compute-2d-angles) 2. [Go further](#go-further)
+1. [Use on your own videos](#use-on-your-own-videos) 2. [Use OpenPose for
+multi-person, more accurate analysis](#use-openpose-for-multi-person-more-
+accurate-analysis) 3. [Advanced-settings](#advanced-settings) 4. [How it works]
+(#how-it-works) 3. [How to cite and how to contribute](#how-to-cite-and-how-to-
+contribute) ## Installation and Demonstration ### Installation - OPTION 1:
+**Quick install** \ Open a terminal. Type `python -V` to make sure python
+'>=3.7 <=3.10' is installed, and then: ``` pip install sports2d ``` - OPTION 2:
+**Safer install with Anaconda**\ Install [Miniconda](https://docs.conda.io/en/
+latest/miniconda.html):\ Open an Anaconda prompt and create a virtual
+environment by typing: ``` conda create -n Sports2D python=3.10 -y conda
+activate Sports2D pip install sports2d ``` - OPTION 3: **Build from source and
+test the last changes**\ Open a terminal in the directory of your choice and
+clone the Sports2D repository. ``` git clone https://github.com/davidpagnon/
+sports2d.git cd sports2d pip install . ``` ### Demonstration: Detect pose and
+compute 2D angles Open a terminal, enter `pip show sports2d`, check sports2d
+package location. \ Copy this path and go to the Demo folder by typing `cd
+\Sports2D\Demo`. \ Type `ipython`, and test the following code: ``` from
+Sports2D import Sports2D Sports2D.detect_pose('Config_demo.toml')
+Sports2D.compute_angles('Config_demo.toml') ``` [Content/
 demo_blazepose_terminal.png] You should obtain a video with the overlaid 2D
 joint positions, and angle text values. This output is also provided as an
 image folder.\ You should additionally obtain the same information as time
 series, stored in .csv files. These files can be opened with any spreadsheet
 software, or with the Pandas Python library for example.\ In addition, you will
 get the original OpenPose-like json coordinates files. [Content/
 demo_blazepose_results.png] ## Go further ### Use on your own videos 1. Copy-
@@ -107,17 +111,17 @@
 to crash. 2. `Config_demo.toml` â `compute_angles_advanced`: These settings
 are taken into account both with BlazePose and OpenPose. 1. `save_vid` and
 `save_img`: Cf `pose_advanced`. 2. `filter`: Cf `pose_advanced`. 3.
 `show_plots`: Cf `pose_advanced`. [Content/demo_show_plots.png] *N.B.:* The
 settings and results of all analyses are stored int the `logs.txt` file, which
 can be found in in the sports2d installation folder (`pip show sports2d` to
 find the path). ### How it works #### Pose detection: BlazePose or OpenPose are
-used to detect joint centers from a video. If `BlazePose` is used, only one
+used to detect joint centers from a video. - If `BlazePose` is used, only one
 person can be detected.\ No interpolation nor filtering options are available.
-Not plotting available. If `OpenPose` is used, multiple persons can be
+Not plotting available. - If `OpenPose` is used, multiple persons can be
 consistently detected across frames. A person is matched to another in the next
 frame when their average point clouds are at a small euclidian distance.\
 Sequences of missing data are interpolated if they are less than N frames
 long.\ Resulting coordinates can be filtered with Butterworth, gaussian,
 median, or loess filter. They can also be plotted. #### Angle computation:
 Joint and segment angles are computed from csv position files.\ If a person
 suddently faces the other way, this change of direction is taken into account.\
@@ -129,49 +133,54 @@
 shoulder **Segment angle conventions:**\ Angles are measured anticlockwise
 between the horizontal and the segment. - Foot: Between heel and big toe -
 Shank: Between knee and ankle - Thigh: Between hip and knee - Arm: Between
 shoulder and elbow - Forearm: Between elbow and wrist - Trunk: Between shoulder
 midpoint and hip midpoint ## How to cite and how to contribute ### How to cite
 If you use this code or data, please cite [Pagnon, 2023]. @misc{Pagnon2023,
 author = {Pagnon, David}, title = {Sports2D - Angles from video}, year =
-{2023}, publisher = {GitHub}, journal = {GitHub repository}, howpublished =
-{\url{https://github.com/davidpagnon/Sports2D}}, } ### How to contribute I
-would happily welcome any proposal for new features, code improvement, and
-more!\ If you want to contribute to Sports2D, please follow [this guide](https:
-//docs.github.com/en/get-started/quickstart/contributing-to-projects) on how to
-fork, modify and push code, and submit a pull request. I would appreciate it if
-you provided as much useful information as possible about how you modified the
-code, and a rationale for why you're making this pull request. Please also
-specify on which operating system and on which python version you have tested
-the code. *Here is a to-do list: feel free to complete it:* - [x] Compute
-**segment angles** - [x] **Multi-person** detection, consistent over time - [x]
-**Only interpolate small gaps** - [x] **Filtering and plotting tools** - [x]
-Handle sudden **changes of direction** - [x] **Colab version** for those who
-cannot install OpenPose - [ ] Full test on **MacOS** - [ ] **GUI applications**
-for Windows, Mac, and Linux, as well as for Android and iOS (minimal version on
-mobile device, with only BlazePose). Code with [Kivy](https://kivy.org) - [ ]
-**Pose refinement**. Click and move badly estimated 2D points. See [DeepLabCut]
-(https://www.youtube.com/watch?v=bEuBKB7eqmk) for inspiration - [ ] **Include
-OpenPose** in Sports2D executable files. [Dockerize](https://github.com/
-stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile) it? - [ ] **Constrain
-points** to OpenSim skeletal model for better angle estimation (like with
-[Pose2Sim](https://github.com/perfanalytics/pose2sim), but in 2D. BSD 3-Clause
-License Copyright (c) 2022, perfanalytics All rights reserved. Redistribution
-and use in source and binary forms, with or without modification, are permitted
-provided that the following conditions are met: 1. Redistributions of source
-code must retain the above copyright notice, this list of conditions and the
-following disclaimer. 2. Redistributions in binary form must reproduce the
-above copyright notice, this list of conditions and the following disclaimer in
-the documentation and/or other materials provided with the distribution. 3.
-Neither the name of the copyright holder nor the names of its contributors may
-be used to endorse or promote products derived from this software without
-specific prior written permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT
-HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
-INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
-FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
-COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
-INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
-LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
-PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
-LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
-OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
-ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+{2023}, doi= {10.5281/zenodo.7903963}, publisher = {GitHub}, journal = {GitHub
+repository}, howpublished = {\url{https://github.com/davidpagnon/Sports2D}}, }
+### How to contribute I would happily welcome any proposal for new features,
+code improvement, and more!\ If you want to contribute to Sports2D, please
+follow [this guide](https://docs.github.com/en/get-started/quickstart/
+contributing-to-projects) on how to fork, modify and push code, and submit a
+pull request. I would appreciate it if you provided as much useful information
+as possible about how you modified the code, and a rationale for why you're
+making this pull request. Please also specify on which operating system and on
+which python version you have tested the code. *Here is a to-do list: feel free
+to complete it:* - [x] Compute **segment angles**. - [x] **Multi-person**
+detection, consistent over time. - [x] **Only interpolate small gaps**. - [x]
+**Filtering and plotting tools**. - [x] Handle sudden **changes of direction**.
+- [x] **Colab version** for those who cannot install OpenPose. - [ ] Full test
+on **MacOS**. - [ ] **GUI applications** for Windows, Mac, and Linux, as well
+as for Android and iOS (minimal version on mobile device, with only BlazePose).
+Code with [Kivy](https://kivy.org). - [ ] **Include OpenPose** in Sports2D
+executable files. [Dockerize](https://github.com/stanfordnmbl/mobile-gaitlab/
+blob/master/demo/Dockerfile) it? - [ ] **Track other points and angles** with
+classic tracking methods (cf. [Kinovea](https://www.kinovea.org/
+features.html)), or by training a model (cf. [DeepLabCut](https://
+deeplabcut.github.io/DeepLabCut/README.html)). - [ ] **Pose refinement**. Click
+and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/
+watch?v=bEuBKB7eqmk) for inspiration. - [ ] **Constrain points** to OpenSim
+skeletal model for better angle estimation (like with [Pose2Sim](https://
+github.com/perfanalytics/pose2sim), but in 2D. - [ ] Add tools for annotating
+images, undistort them, take perspective into account, etc. (cf. [Kinovea]
+(https://www.kinovea.org/features.html)). BSD 3-Clause License Copyright (c)
+2022, perfanalytics All rights reserved. Redistribution and use in source and
+binary forms, with or without modification, are permitted provided that the
+following conditions are met: 1. Redistributions of source code must retain the
+above copyright notice, this list of conditions and the following disclaimer.
+2. Redistributions in binary form must reproduce the above copyright notice,
+this list of conditions and the following disclaimer in the documentation and/
+or other materials provided with the distribution. 3. Neither the name of the
+copyright holder nor the names of its contributors may be used to endorse or
+promote products derived from this software without specific prior written
+permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
+GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
+HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
+OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `sports2d-0.0.9/README.md` & `sports2d-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
 [![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D)\
-[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\
+[![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+[![DOI](https://zenodo.org/badge/634044634.svg)](https://zenodo.org/badge/latestdoi/634044634)\
 <a href="https://colab.research.google.com/github/davidpagnon/Sports2D/blob/main/Sports2D/Sports2D.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 <!-- [![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
 [![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
 [![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
 [![DOI](https://zenodo.org/badge/501642916.svg)](https://zenodo.org/badge/latestdoi/501642916)
@@ -50,15 +52,15 @@
     pip install sports2d
     ```
 
 - OPTION 2: **Safer install with Anaconda**\
     Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):\
     Open an Anaconda prompt and create a virtual environment by typing:
     ```
-    conda create -n Sports2D python<=3.10 
+    conda create -n Sports2D python=3.10 -y
     conda activate Sports2D
     pip install sports2d
     ```
 
 - OPTION 3: **Build from source and test the last changes**\
      Open a terminal in the directory of your choice and clone the Sports2D repository.
      ```
@@ -163,20 +165,20 @@
 
 ### How it works
 
 #### Pose detection:
 
 BlazePose or OpenPose are used to detect joint centers from a video.
 
-If `BlazePose` is used, only one person can be detected.\
-No interpolation nor filtering options are available. Not plotting available.
+- If `BlazePose` is used, only one person can be detected.\
+  No interpolation nor filtering options are available. Not plotting available.
 
-If `OpenPose` is used, multiple persons can be consistently detected across frames. A person is matched to another in the next frame when their average point clouds are at a small euclidian distance.\
-Sequences of missing data are interpolated if they are less than N frames long.\
-Resulting coordinates can be filtered with Butterworth, gaussian, median, or loess filter. They can also be plotted.
+- If `OpenPose` is used, multiple persons can be consistently detected across frames. A person is matched to another in the next frame when their average point clouds are at a small euclidian distance.\
+  Sequences of missing data are interpolated if they are less than N frames long.\
+  Resulting coordinates can be filtered with Butterworth, gaussian, median, or loess filter. They can also be plotted.
 
 
 #### Angle computation:
 
 Joint and segment angles are computed from csv position files.\
 If a person suddently faces the other way, this change of direction is taken into account.\
 Resulting angles can be filtered in the same way as point coordinates, and they can also be plotted.
@@ -202,28 +204,31 @@
 ### How to cite
 If you use this code or data, please cite [Pagnon, 2023].
 
      @misc{Pagnon2023,
        author = {Pagnon, David},
        title = {Sports2D - Angles from video},
        year = {2023},
+       doi= {10.5281/zenodo.7903963},
        publisher = {GitHub},
        journal = {GitHub repository},
        howpublished = {\url{https://github.com/davidpagnon/Sports2D}},
      }
 
 ### How to contribute
 I would happily welcome any proposal for new features, code improvement, and more!\
 If you want to contribute to Sports2D, please follow [this guide](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) on how to fork, modify and push code, and submit a pull request. I would appreciate it if you provided as much useful information as possible about how you modified the code, and a rationale for why you're making this pull request. Please also specify on which operating system and on which python version you have tested the code.
 
 *Here is a to-do list: feel free to complete it:*
-- [x] Compute **segment angles**
-- [x] **Multi-person** detection, consistent over time
-- [x] **Only interpolate small gaps**
-- [x] **Filtering and plotting tools**
-- [x] Handle sudden **changes of direction**
-- [x] **Colab version** for those who cannot install OpenPose
-- [ ] Full test on **MacOS**
-- [ ] **GUI applications** for Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with [Kivy](https://kivy.org)
-- [ ] **Pose refinement**. Click and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/watch?v=bEuBKB7eqmk) for inspiration
+- [x] Compute **segment angles**.
+- [x] **Multi-person** detection, consistent over time.
+- [x] **Only interpolate small gaps**.
+- [x] **Filtering and plotting tools**.
+- [x] Handle sudden **changes of direction**.
+- [x] **Colab version** for those who cannot install OpenPose.
+- [ ] Full test on **MacOS**.
+- [ ] **GUI applications** for Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with [Kivy](https://kivy.org).
 - [ ] **Include OpenPose** in Sports2D executable files. [Dockerize](https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile) it? 
+- [ ] **Track other points and angles** with classic tracking methods (cf. [Kinovea](https://www.kinovea.org/features.html)), or by training a model (cf. [DeepLabCut](https://deeplabcut.github.io/DeepLabCut/README.html)).
+- [ ] **Pose refinement**. Click and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/watch?v=bEuBKB7eqmk) for inspiration.
 - [ ] **Constrain points** to OpenSim skeletal model for better angle estimation (like with [Pose2Sim](https://github.com/perfanalytics/pose2sim), but in 2D.
+- [ ] Add tools for annotating images, undistort them, take perspective into account, etc. (cf. [Kinovea](https://www.kinovea.org/features.html)).
```

#### html2text {}

```diff
@@ -1,49 +1,53 @@
  [![Continuous integration](https://github.com/davidpagnon/sports2d/actions/
 workflows/continuous-integration.yml/badge.svg?branch=main)](https://
 github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/
-py/Sports2D)\ [![License](https://img.shields.io/badge/License-BSD_3--Clause-
-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\ [Open_In_Colab]  #
-Sports2D **`Sports2D` lets you compute 2D joint and segment angles from a
-video.** [Content/demo_gif.gif] `Warning:` Angle estimation is only as good as
-the pose estimation algorithm, i.e., it is not perfect.\ `Warning:` Results are
-acceptable only if the persons move in the 2D plane, from right to left or from
-left to right.\ If you need research-grade markerless joint kinematics,
-consider using several cameras, and constraining angles to a biomechanically
-accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for
-example. `Know issue`: Results won't be good with some iPhone videos in
-portrait mode. This is solved by priorly converting them with `ffmpeg -
-i video_input.mov video_output.mp4`, or even more simply with any random online
-video converter such as https://video-converter.com. `Announcement:` Apps with
-GUI will soon be released for Windows, Linux, MacOS, as well as Android and
-iOS. Mobile versions will only support simple exploratory analysis. This
-involves single-person angle computation, in a potentially less accurate and
-tunable way. ## Contents 1. [Installation and Demonstration](#installation-and-
-demonstration) 1. [Installation](#installation) 2. [Demonstration: Detect pose
-and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles) 2. [Go
-further](#go-further) 1. [Use on your own videos](#use-on-your-own-videos) 2.
-[Use OpenPose for multi-person, more accurate analysis](#use-openpose-for-
-multi-person-more-accurate-analysis) 3. [Advanced-settings](#advanced-settings)
-4. [How it works](#how-it-works) 3. [How to cite and how to contribute](#how-
-to-cite-and-how-to-contribute) ## Installation and Demonstration ###
-Installation - OPTION 1: **Quick install** \ Open a terminal. Type `python -V`
-to make sure python '>=3.7 <=3.10' is installed, and then: ``` pip install
-sports2d ``` - OPTION 2: **Safer install with Anaconda**\ Install [Miniconda]
-(https://docs.conda.io/en/latest/miniconda.html):\ Open an Anaconda prompt and
-create a virtual environment by typing: ``` conda create -n Sports2D
-python<=3.10 conda activate Sports2D pip install sports2d ``` - OPTION 3:
-**Build from source and test the last changes**\ Open a terminal in the
-directory of your choice and clone the Sports2D repository. ``` git clone
-https://github.com/davidpagnon/sports2d.git cd sports2d pip install . ``` ###
-Demonstration: Detect pose and compute 2D angles Open a terminal, enter `pip
-show sports2d`, check sports2d package location. \ Copy this path and go to the
-Demo folder by typing `cd \Sports2D\Demo`. \ Type `ipython`, and test the
-following code: ``` from Sports2D import Sports2D Sports2D.detect_pose
-('Config_demo.toml') Sports2D.compute_angles('Config_demo.toml') ``` [Content/
+py/Sports2D)\ [![Open Source? Yes!](https://badgen.net/badge/
+Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/
+badges/) [![License](https://img.shields.io/badge/License-BSD_3--Clause-
+blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![DOI](https://
+zenodo.org/badge/634044634.svg)](https://zenodo.org/badge/latestdoi/634044634)\
+[Open_In_Colab]  # Sports2D **`Sports2D` lets you compute 2D joint and segment
+angles from a video.** [Content/demo_gif.gif] `Warning:` Angle estimation is
+only as good as the pose estimation algorithm, i.e., it is not perfect.\
+`Warning:` Results are acceptable only if the persons move in the 2D plane,
+from right to left or from left to right.\ If you need research-grade
+markerless joint kinematics, consider using several cameras, and constraining
+angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/
+perfanalytics/pose2sim) for example. `Know issue`: Results won't be good with
+some iPhone videos in portrait mode. This is solved by priorly converting them
+with `ffmpeg -i video_input.mov video_output.mp4`, or even more simply with any
+random online video converter such as https://video-converter.com.
+`Announcement:` Apps with GUI will soon be released for Windows, Linux, MacOS,
+as well as Android and iOS. Mobile versions will only support simple
+exploratory analysis. This involves single-person angle computation, in a
+potentially less accurate and tunable way. ## Contents 1. [Installation and
+Demonstration](#installation-and-demonstration) 1. [Installation]
+(#installation) 2. [Demonstration: Detect pose and compute 2D angles]
+(#demonstration-detect-pose-and-compute-2d-angles) 2. [Go further](#go-further)
+1. [Use on your own videos](#use-on-your-own-videos) 2. [Use OpenPose for
+multi-person, more accurate analysis](#use-openpose-for-multi-person-more-
+accurate-analysis) 3. [Advanced-settings](#advanced-settings) 4. [How it works]
+(#how-it-works) 3. [How to cite and how to contribute](#how-to-cite-and-how-to-
+contribute) ## Installation and Demonstration ### Installation - OPTION 1:
+**Quick install** \ Open a terminal. Type `python -V` to make sure python
+'>=3.7 <=3.10' is installed, and then: ``` pip install sports2d ``` - OPTION 2:
+**Safer install with Anaconda**\ Install [Miniconda](https://docs.conda.io/en/
+latest/miniconda.html):\ Open an Anaconda prompt and create a virtual
+environment by typing: ``` conda create -n Sports2D python=3.10 -y conda
+activate Sports2D pip install sports2d ``` - OPTION 3: **Build from source and
+test the last changes**\ Open a terminal in the directory of your choice and
+clone the Sports2D repository. ``` git clone https://github.com/davidpagnon/
+sports2d.git cd sports2d pip install . ``` ### Demonstration: Detect pose and
+compute 2D angles Open a terminal, enter `pip show sports2d`, check sports2d
+package location. \ Copy this path and go to the Demo folder by typing `cd
+\Sports2D\Demo`. \ Type `ipython`, and test the following code: ``` from
+Sports2D import Sports2D Sports2D.detect_pose('Config_demo.toml')
+Sports2D.compute_angles('Config_demo.toml') ``` [Content/
 demo_blazepose_terminal.png] You should obtain a video with the overlaid 2D
 joint positions, and angle text values. This output is also provided as an
 image folder.\ You should additionally obtain the same information as time
 series, stored in .csv files. These files can be opened with any spreadsheet
 software, or with the Pandas Python library for example.\ In addition, you will
 get the original OpenPose-like json coordinates files. [Content/
 demo_blazepose_results.png] ## Go further ### Use on your own videos 1. Copy-
@@ -91,17 +95,17 @@
 to crash. 2. `Config_demo.toml` â `compute_angles_advanced`: These settings
 are taken into account both with BlazePose and OpenPose. 1. `save_vid` and
 `save_img`: Cf `pose_advanced`. 2. `filter`: Cf `pose_advanced`. 3.
 `show_plots`: Cf `pose_advanced`. [Content/demo_show_plots.png] *N.B.:* The
 settings and results of all analyses are stored int the `logs.txt` file, which
 can be found in in the sports2d installation folder (`pip show sports2d` to
 find the path). ### How it works #### Pose detection: BlazePose or OpenPose are
-used to detect joint centers from a video. If `BlazePose` is used, only one
+used to detect joint centers from a video. - If `BlazePose` is used, only one
 person can be detected.\ No interpolation nor filtering options are available.
-Not plotting available. If `OpenPose` is used, multiple persons can be
+Not plotting available. - If `OpenPose` is used, multiple persons can be
 consistently detected across frames. A person is matched to another in the next
 frame when their average point clouds are at a small euclidian distance.\
 Sequences of missing data are interpolated if they are less than N frames
 long.\ Resulting coordinates can be filtered with Butterworth, gaussian,
 median, or loess filter. They can also be plotted. #### Angle computation:
 Joint and segment angles are computed from csv position files.\ If a person
 suddently faces the other way, this change of direction is taken into account.\
@@ -113,29 +117,35 @@
 shoulder **Segment angle conventions:**\ Angles are measured anticlockwise
 between the horizontal and the segment. - Foot: Between heel and big toe -
 Shank: Between knee and ankle - Thigh: Between hip and knee - Arm: Between
 shoulder and elbow - Forearm: Between elbow and wrist - Trunk: Between shoulder
 midpoint and hip midpoint ## How to cite and how to contribute ### How to cite
 If you use this code or data, please cite [Pagnon, 2023]. @misc{Pagnon2023,
 author = {Pagnon, David}, title = {Sports2D - Angles from video}, year =
-{2023}, publisher = {GitHub}, journal = {GitHub repository}, howpublished =
-{\url{https://github.com/davidpagnon/Sports2D}}, } ### How to contribute I
-would happily welcome any proposal for new features, code improvement, and
-more!\ If you want to contribute to Sports2D, please follow [this guide](https:
-//docs.github.com/en/get-started/quickstart/contributing-to-projects) on how to
-fork, modify and push code, and submit a pull request. I would appreciate it if
-you provided as much useful information as possible about how you modified the
-code, and a rationale for why you're making this pull request. Please also
-specify on which operating system and on which python version you have tested
-the code. *Here is a to-do list: feel free to complete it:* - [x] Compute
-**segment angles** - [x] **Multi-person** detection, consistent over time - [x]
-**Only interpolate small gaps** - [x] **Filtering and plotting tools** - [x]
-Handle sudden **changes of direction** - [x] **Colab version** for those who
-cannot install OpenPose - [ ] Full test on **MacOS** - [ ] **GUI applications**
-for Windows, Mac, and Linux, as well as for Android and iOS (minimal version on
-mobile device, with only BlazePose). Code with [Kivy](https://kivy.org) - [ ]
-**Pose refinement**. Click and move badly estimated 2D points. See [DeepLabCut]
-(https://www.youtube.com/watch?v=bEuBKB7eqmk) for inspiration - [ ] **Include
-OpenPose** in Sports2D executable files. [Dockerize](https://github.com/
-stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile) it? - [ ] **Constrain
-points** to OpenSim skeletal model for better angle estimation (like with
-[Pose2Sim](https://github.com/perfanalytics/pose2sim), but in 2D.
+{2023}, doi= {10.5281/zenodo.7903963}, publisher = {GitHub}, journal = {GitHub
+repository}, howpublished = {\url{https://github.com/davidpagnon/Sports2D}}, }
+### How to contribute I would happily welcome any proposal for new features,
+code improvement, and more!\ If you want to contribute to Sports2D, please
+follow [this guide](https://docs.github.com/en/get-started/quickstart/
+contributing-to-projects) on how to fork, modify and push code, and submit a
+pull request. I would appreciate it if you provided as much useful information
+as possible about how you modified the code, and a rationale for why you're
+making this pull request. Please also specify on which operating system and on
+which python version you have tested the code. *Here is a to-do list: feel free
+to complete it:* - [x] Compute **segment angles**. - [x] **Multi-person**
+detection, consistent over time. - [x] **Only interpolate small gaps**. - [x]
+**Filtering and plotting tools**. - [x] Handle sudden **changes of direction**.
+- [x] **Colab version** for those who cannot install OpenPose. - [ ] Full test
+on **MacOS**. - [ ] **GUI applications** for Windows, Mac, and Linux, as well
+as for Android and iOS (minimal version on mobile device, with only BlazePose).
+Code with [Kivy](https://kivy.org). - [ ] **Include OpenPose** in Sports2D
+executable files. [Dockerize](https://github.com/stanfordnmbl/mobile-gaitlab/
+blob/master/demo/Dockerfile) it? - [ ] **Track other points and angles** with
+classic tracking methods (cf. [Kinovea](https://www.kinovea.org/
+features.html)), or by training a model (cf. [DeepLabCut](https://
+deeplabcut.github.io/DeepLabCut/README.html)). - [ ] **Pose refinement**. Click
+and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/
+watch?v=bEuBKB7eqmk) for inspiration. - [ ] **Constrain points** to OpenSim
+skeletal model for better angle estimation (like with [Pose2Sim](https://
+github.com/perfanalytics/pose2sim), but in 2D. - [ ] Add tools for annotating
+images, undistort them, take perspective into account, etc. (cf. [Kinovea]
+(https://www.kinovea.org/features.html)).
```

### Comparing `sports2d-0.0.9/Sports2D/Demo/Config_demo.toml` & `sports2d-0.1.0/Sports2D/Demo/Config_demo.toml`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.9/Sports2D/Demo/demo.mp4` & `sports2d-0.1.0/Sports2D/Demo/demo.mp4`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.9/Sports2D/Sports2D.py` & `sports2d-0.1.0/Sports2D/Sports2D.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.9/Sports2D/Utilities/Blazepose_runsave.py` & `sports2d-0.1.0/Sports2D/Utilities/Blazepose_runsave.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.9/Sports2D/Utilities/common.py` & `sports2d-0.1.0/Sports2D/Utilities/common.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.9/Sports2D/Utilities/filter.py` & `sports2d-0.1.0/Sports2D/Utilities/filter.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.9/Sports2D/Utilities/skeletons.py` & `sports2d-0.1.0/Sports2D/Utilities/skeletons.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.9/Sports2D/compute_angles.py` & `sports2d-0.1.0/Sports2D/compute_angles.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
     filter_options = (do_filter, filter_type, butterworth_filter_order, butterworth_filter_cutoff, frame_rate, gaussian_filter_kernel, loess_filter_kernel, median_filter_kernel)
     
     show_angles_img = config_dict.get('compute_angles_advanced').get('save_img')
     show_angles_vid = config_dict.get('compute_angles_advanced').get('save_vid')
     
     # Find csv position files in video_dir, search pose_model and video_file.stem
     logging.info(f'Retrieving csv position files in {video_dir}...')
-    csv_paths = list(video_dir.glob(f'*{video_file.stem}_{pose_model}_*points*.csv'))
+    csv_paths = sorted(video_dir.glob(f'*{video_file.stem}_{pose_model}_*points*.csv'))
     logging.info(f'{len(csv_paths)} persons found.')
 
     # Compute angles
     df_angles_list = []
     for i, c in enumerate(csv_paths):
         # Prepare angle csv header
         scorer = ['DavidPagnon']*angle_nb
@@ -460,15 +460,15 @@
             cap = [cv2.VideoCapture(str(video_pose)) if Path.exists(video_pose) else cv2.VideoCapture(str(video_base))][0]
             fps = cap.get(cv2.CAP_PROP_FPS)
             W, H = cap.get(cv2.CAP_PROP_FRAME_WIDTH), cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
             fourcc = cv2.VideoWriter_fourcc(*'mp4v')
             writer = cv2.VideoWriter(str(video_pose2), fourcc, fps, (int(W), int(H)))
         
         # Preferentially from pose image files
-        frames_img = list(img_pose.glob('*'))
+        frames_img = sorted(img_pose.glob('*'))
         if len(frames_img)>0:
             for frame_nb in range(df_angles_list[0].shape[0]):
                 df_angles_list_frame = [df_angles_list[n].iloc[frame_nb,:] for n in range(len(df_angles_list))]
                 frame = cv2.imread(str(frames_img[frame_nb]))
                 frame = overlay_angles(frame, df_angles_list_frame)
                 if show_angles_img:
                     cv2.imwrite(str(frames_img[frame_nb]), frame)
```

### Comparing `sports2d-0.0.9/Sports2D/detect_pose.py` & `sports2d-0.1.0/Sports2D/detect_pose.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
     keypoints_ids = [node.id for _, _, node in RenderTree(model) if node.id!=None]
     keypoints_names = [node.name for _, _, node in RenderTree(model) if node.id!=None]
     keypoints_names_rearranged = [y for x,y in sorted(zip(keypoints_ids,keypoints_names))]
     keypoints_nb = len(keypoints_ids)
 
     # Retrieve coordinates
     logging.info('Sorting people across frames.')
-    json_fnames = list(json_path.glob('*.json'))
+    json_fnames = sorted(json_path.glob('*.json'))
     nb_persons_to_detect = max([len(json.load(open(json_fname))['people']) for json_fname in json_fnames])
     Coords = [np.array([]).reshape(0,keypoints_nb*3)] * nb_persons_to_detect
     for json_fname in json_fnames:    # for each frame
         with open(json_fname) as json_f:
             json_file = json.load(json_f)
             keypt = []
             # Retrieve coords for this frame 
@@ -451,17 +451,17 @@
     json_display_with_img -j "<json_folder>" -i "<raw_img_folder>"
     json_display_with_img -j "<json_folder>" -i "<raw_img_folder>" -o "<output_img_folder>" -d True -s True
     import json_display_with_img; json_display_with_img.json_display_with_img_func(json_folder=r'<json_folder>', raw_img_folder=r'<raw_img_folder>')
     '''
             
    # Find csv position files, prepare video and image saving paths
     pose_model = pose_model[0]
-    csv_paths = list(video_path.parent.glob(f'*{video_path.stem}*{pose_model}*points*refined*.csv'))
+    csv_paths = sorted(video_path.parent.glob(f'*{video_path.stem}*{pose_model}*points*refined*.csv'))
     if csv_paths == []:
-        csv_paths = list(video_path.parent.glob(f'*{video_path.stem}*{pose_model}*points*.csv'))
+        csv_paths = sorted(video_path.parent.glob(f'*{video_path.stem}*{pose_model}*points*.csv'))
         
     # Open csv files
     coords = []
     for c in csv_paths:
         with open(c) as c_f:
             coords += [pd.read_csv(c_f, header=[0,1,2,3])]
 
@@ -476,15 +476,15 @@
         fourcc = cv2.VideoWriter_fourcc(*'mp4v')
         writer = cv2.VideoWriter(str(video_pose_path), fourcc, fps, (int(W), int(H)))
     if save_img:
         img_pose_path = video_path.parent / (video_path.stem + '_' + pose_model + '_img')
         img_pose_path.mkdir(parents=True, exist_ok=True)  
         
     f = 0
-    while(cap.isOpened()):
+    while(cap.isOpened() and f < len(coords[0])):
         ret, frame = cap.read()
         if ret == True:
             X = [np.array(coord.iloc[f,1::3]) for coord in coords]
             X = [np.where(x==0., np.nan, x) for x in X]
             Y = [np.array(coord.iloc[f,2::3]) for coord in coords]
             Y = [np.where(y==0., np.nan, y) for y in Y]
```

### Comparing `sports2d-0.0.9/setup.cfg` & `sports2d-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sports2d
-version = 0.0.9
+version = 0.1.0
 author = David Pagnon
 author_email = contact@david-pagnon.com
 description = Detect pose and compute 2D joint angles from a video.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/davidpagnon/Sports2D
 keywords = markerless, kinematics, OpenPose, BlazePose, joint angles, 2D, biomechanics, sports, sports-analytics
```

### Comparing `sports2d-0.0.9/sports2d.egg-info/PKG-INFO` & `sports2d-0.1.0/sports2d.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.0.9
+Version: 0.1.0
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
@@ -24,15 +24,17 @@
 Requires-Python: <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D)\
-[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\
+[![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+[![DOI](https://zenodo.org/badge/634044634.svg)](https://zenodo.org/badge/latestdoi/634044634)\
 <a href="https://colab.research.google.com/github/davidpagnon/Sports2D/blob/main/Sports2D/Sports2D.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 <!-- [![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
 [![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
 [![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
 [![DOI](https://zenodo.org/badge/501642916.svg)](https://zenodo.org/badge/latestdoi/501642916)
@@ -77,15 +79,15 @@
     pip install sports2d
     ```
 
 - OPTION 2: **Safer install with Anaconda**\
     Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):\
     Open an Anaconda prompt and create a virtual environment by typing:
     ```
-    conda create -n Sports2D python<=3.10 
+    conda create -n Sports2D python=3.10 -y
     conda activate Sports2D
     pip install sports2d
     ```
 
 - OPTION 3: **Build from source and test the last changes**\
      Open a terminal in the directory of your choice and clone the Sports2D repository.
      ```
@@ -190,20 +192,20 @@
 
 ### How it works
 
 #### Pose detection:
 
 BlazePose or OpenPose are used to detect joint centers from a video.
 
-If `BlazePose` is used, only one person can be detected.\
-No interpolation nor filtering options are available. Not plotting available.
+- If `BlazePose` is used, only one person can be detected.\
+  No interpolation nor filtering options are available. Not plotting available.
 
-If `OpenPose` is used, multiple persons can be consistently detected across frames. A person is matched to another in the next frame when their average point clouds are at a small euclidian distance.\
-Sequences of missing data are interpolated if they are less than N frames long.\
-Resulting coordinates can be filtered with Butterworth, gaussian, median, or loess filter. They can also be plotted.
+- If `OpenPose` is used, multiple persons can be consistently detected across frames. A person is matched to another in the next frame when their average point clouds are at a small euclidian distance.\
+  Sequences of missing data are interpolated if they are less than N frames long.\
+  Resulting coordinates can be filtered with Butterworth, gaussian, median, or loess filter. They can also be plotted.
 
 
 #### Angle computation:
 
 Joint and segment angles are computed from csv position files.\
 If a person suddently faces the other way, this change of direction is taken into account.\
 Resulting angles can be filtered in the same way as point coordinates, and they can also be plotted.
@@ -229,35 +231,38 @@
 ### How to cite
 If you use this code or data, please cite [Pagnon, 2023].
 
      @misc{Pagnon2023,
        author = {Pagnon, David},
        title = {Sports2D - Angles from video},
        year = {2023},
+       doi= {10.5281/zenodo.7903963},
        publisher = {GitHub},
        journal = {GitHub repository},
        howpublished = {\url{https://github.com/davidpagnon/Sports2D}},
      }
 
 ### How to contribute
 I would happily welcome any proposal for new features, code improvement, and more!\
 If you want to contribute to Sports2D, please follow [this guide](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) on how to fork, modify and push code, and submit a pull request. I would appreciate it if you provided as much useful information as possible about how you modified the code, and a rationale for why you're making this pull request. Please also specify on which operating system and on which python version you have tested the code.
 
 *Here is a to-do list: feel free to complete it:*
-- [x] Compute **segment angles**
-- [x] **Multi-person** detection, consistent over time
-- [x] **Only interpolate small gaps**
-- [x] **Filtering and plotting tools**
-- [x] Handle sudden **changes of direction**
-- [x] **Colab version** for those who cannot install OpenPose
-- [ ] Full test on **MacOS**
-- [ ] **GUI applications** for Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with [Kivy](https://kivy.org)
-- [ ] **Pose refinement**. Click and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/watch?v=bEuBKB7eqmk) for inspiration
+- [x] Compute **segment angles**.
+- [x] **Multi-person** detection, consistent over time.
+- [x] **Only interpolate small gaps**.
+- [x] **Filtering and plotting tools**.
+- [x] Handle sudden **changes of direction**.
+- [x] **Colab version** for those who cannot install OpenPose.
+- [ ] Full test on **MacOS**.
+- [ ] **GUI applications** for Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with [Kivy](https://kivy.org).
 - [ ] **Include OpenPose** in Sports2D executable files. [Dockerize](https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile) it? 
+- [ ] **Track other points and angles** with classic tracking methods (cf. [Kinovea](https://www.kinovea.org/features.html)), or by training a model (cf. [DeepLabCut](https://deeplabcut.github.io/DeepLabCut/README.html)).
+- [ ] **Pose refinement**. Click and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/watch?v=bEuBKB7eqmk) for inspiration.
 - [ ] **Constrain points** to OpenSim skeletal model for better angle estimation (like with [Pose2Sim](https://github.com/perfanalytics/pose2sim), but in 2D.
+- [ ] Add tools for annotating images, undistort them, take perspective into account, etc. (cf. [Kinovea](https://www.kinovea.org/features.html)).
 
 BSD 3-Clause License
 
 Copyright (c) 2022, perfanalytics
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sports2d Version: 0.0.9 Summary: Detect pose and
+Metadata-Version: 2.1 Name: sports2d Version: 0.1.0 Summary: Detect pose and
 compute 2D joint angles from a video. Home-page: https://github.com/
 davidpagnon/Sports2D Author: David Pagnon Author-email: contact@david-
 pagnon.com License: BSD 3-Clause License Project-URL: Bug Tracker, https://
 github.com/davidpagnon/Sports2D/issues Keywords:
 markerless,kinematics,OpenPose,BlazePose,joint
 angles,2D,biomechanics,sports,sports-analytics Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Development Status :: 3 - Alpha
@@ -14,52 +14,56 @@
 Engineering :: Medical Science Apps. Classifier: Topic :: Multimedia ::
 Graphics Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling Requires-
 Python: <3.11 Description-Content-Type: text/markdown License-File: LICENSE [!
 [Continuous integration](https://github.com/davidpagnon/sports2d/actions/
 workflows/continuous-integration.yml/badge.svg?branch=main)](https://
 github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/
-py/Sports2D)\ [![License](https://img.shields.io/badge/License-BSD_3--Clause-
-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\ [Open_In_Colab]  #
-Sports2D **`Sports2D` lets you compute 2D joint and segment angles from a
-video.** [Content/demo_gif.gif] `Warning:` Angle estimation is only as good as
-the pose estimation algorithm, i.e., it is not perfect.\ `Warning:` Results are
-acceptable only if the persons move in the 2D plane, from right to left or from
-left to right.\ If you need research-grade markerless joint kinematics,
-consider using several cameras, and constraining angles to a biomechanically
-accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for
-example. `Know issue`: Results won't be good with some iPhone videos in
-portrait mode. This is solved by priorly converting them with `ffmpeg -
-i video_input.mov video_output.mp4`, or even more simply with any random online
-video converter such as https://video-converter.com. `Announcement:` Apps with
-GUI will soon be released for Windows, Linux, MacOS, as well as Android and
-iOS. Mobile versions will only support simple exploratory analysis. This
-involves single-person angle computation, in a potentially less accurate and
-tunable way. ## Contents 1. [Installation and Demonstration](#installation-and-
-demonstration) 1. [Installation](#installation) 2. [Demonstration: Detect pose
-and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles) 2. [Go
-further](#go-further) 1. [Use on your own videos](#use-on-your-own-videos) 2.
-[Use OpenPose for multi-person, more accurate analysis](#use-openpose-for-
-multi-person-more-accurate-analysis) 3. [Advanced-settings](#advanced-settings)
-4. [How it works](#how-it-works) 3. [How to cite and how to contribute](#how-
-to-cite-and-how-to-contribute) ## Installation and Demonstration ###
-Installation - OPTION 1: **Quick install** \ Open a terminal. Type `python -V`
-to make sure python '>=3.7 <=3.10' is installed, and then: ``` pip install
-sports2d ``` - OPTION 2: **Safer install with Anaconda**\ Install [Miniconda]
-(https://docs.conda.io/en/latest/miniconda.html):\ Open an Anaconda prompt and
-create a virtual environment by typing: ``` conda create -n Sports2D
-python<=3.10 conda activate Sports2D pip install sports2d ``` - OPTION 3:
-**Build from source and test the last changes**\ Open a terminal in the
-directory of your choice and clone the Sports2D repository. ``` git clone
-https://github.com/davidpagnon/sports2d.git cd sports2d pip install . ``` ###
-Demonstration: Detect pose and compute 2D angles Open a terminal, enter `pip
-show sports2d`, check sports2d package location. \ Copy this path and go to the
-Demo folder by typing `cd \Sports2D\Demo`. \ Type `ipython`, and test the
-following code: ``` from Sports2D import Sports2D Sports2D.detect_pose
-('Config_demo.toml') Sports2D.compute_angles('Config_demo.toml') ``` [Content/
+py/Sports2D)\ [![Open Source? Yes!](https://badgen.net/badge/
+Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/
+badges/) [![License](https://img.shields.io/badge/License-BSD_3--Clause-
+blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![DOI](https://
+zenodo.org/badge/634044634.svg)](https://zenodo.org/badge/latestdoi/634044634)\
+[Open_In_Colab]  # Sports2D **`Sports2D` lets you compute 2D joint and segment
+angles from a video.** [Content/demo_gif.gif] `Warning:` Angle estimation is
+only as good as the pose estimation algorithm, i.e., it is not perfect.\
+`Warning:` Results are acceptable only if the persons move in the 2D plane,
+from right to left or from left to right.\ If you need research-grade
+markerless joint kinematics, consider using several cameras, and constraining
+angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/
+perfanalytics/pose2sim) for example. `Know issue`: Results won't be good with
+some iPhone videos in portrait mode. This is solved by priorly converting them
+with `ffmpeg -i video_input.mov video_output.mp4`, or even more simply with any
+random online video converter such as https://video-converter.com.
+`Announcement:` Apps with GUI will soon be released for Windows, Linux, MacOS,
+as well as Android and iOS. Mobile versions will only support simple
+exploratory analysis. This involves single-person angle computation, in a
+potentially less accurate and tunable way. ## Contents 1. [Installation and
+Demonstration](#installation-and-demonstration) 1. [Installation]
+(#installation) 2. [Demonstration: Detect pose and compute 2D angles]
+(#demonstration-detect-pose-and-compute-2d-angles) 2. [Go further](#go-further)
+1. [Use on your own videos](#use-on-your-own-videos) 2. [Use OpenPose for
+multi-person, more accurate analysis](#use-openpose-for-multi-person-more-
+accurate-analysis) 3. [Advanced-settings](#advanced-settings) 4. [How it works]
+(#how-it-works) 3. [How to cite and how to contribute](#how-to-cite-and-how-to-
+contribute) ## Installation and Demonstration ### Installation - OPTION 1:
+**Quick install** \ Open a terminal. Type `python -V` to make sure python
+'>=3.7 <=3.10' is installed, and then: ``` pip install sports2d ``` - OPTION 2:
+**Safer install with Anaconda**\ Install [Miniconda](https://docs.conda.io/en/
+latest/miniconda.html):\ Open an Anaconda prompt and create a virtual
+environment by typing: ``` conda create -n Sports2D python=3.10 -y conda
+activate Sports2D pip install sports2d ``` - OPTION 3: **Build from source and
+test the last changes**\ Open a terminal in the directory of your choice and
+clone the Sports2D repository. ``` git clone https://github.com/davidpagnon/
+sports2d.git cd sports2d pip install . ``` ### Demonstration: Detect pose and
+compute 2D angles Open a terminal, enter `pip show sports2d`, check sports2d
+package location. \ Copy this path and go to the Demo folder by typing `cd
+\Sports2D\Demo`. \ Type `ipython`, and test the following code: ``` from
+Sports2D import Sports2D Sports2D.detect_pose('Config_demo.toml')
+Sports2D.compute_angles('Config_demo.toml') ``` [Content/
 demo_blazepose_terminal.png] You should obtain a video with the overlaid 2D
 joint positions, and angle text values. This output is also provided as an
 image folder.\ You should additionally obtain the same information as time
 series, stored in .csv files. These files can be opened with any spreadsheet
 software, or with the Pandas Python library for example.\ In addition, you will
 get the original OpenPose-like json coordinates files. [Content/
 demo_blazepose_results.png] ## Go further ### Use on your own videos 1. Copy-
@@ -107,17 +111,17 @@
 to crash. 2. `Config_demo.toml` â `compute_angles_advanced`: These settings
 are taken into account both with BlazePose and OpenPose. 1. `save_vid` and
 `save_img`: Cf `pose_advanced`. 2. `filter`: Cf `pose_advanced`. 3.
 `show_plots`: Cf `pose_advanced`. [Content/demo_show_plots.png] *N.B.:* The
 settings and results of all analyses are stored int the `logs.txt` file, which
 can be found in in the sports2d installation folder (`pip show sports2d` to
 find the path). ### How it works #### Pose detection: BlazePose or OpenPose are
-used to detect joint centers from a video. If `BlazePose` is used, only one
+used to detect joint centers from a video. - If `BlazePose` is used, only one
 person can be detected.\ No interpolation nor filtering options are available.
-Not plotting available. If `OpenPose` is used, multiple persons can be
+Not plotting available. - If `OpenPose` is used, multiple persons can be
 consistently detected across frames. A person is matched to another in the next
 frame when their average point clouds are at a small euclidian distance.\
 Sequences of missing data are interpolated if they are less than N frames
 long.\ Resulting coordinates can be filtered with Butterworth, gaussian,
 median, or loess filter. They can also be plotted. #### Angle computation:
 Joint and segment angles are computed from csv position files.\ If a person
 suddently faces the other way, this change of direction is taken into account.\
@@ -129,49 +133,54 @@
 shoulder **Segment angle conventions:**\ Angles are measured anticlockwise
 between the horizontal and the segment. - Foot: Between heel and big toe -
 Shank: Between knee and ankle - Thigh: Between hip and knee - Arm: Between
 shoulder and elbow - Forearm: Between elbow and wrist - Trunk: Between shoulder
 midpoint and hip midpoint ## How to cite and how to contribute ### How to cite
 If you use this code or data, please cite [Pagnon, 2023]. @misc{Pagnon2023,
 author = {Pagnon, David}, title = {Sports2D - Angles from video}, year =
-{2023}, publisher = {GitHub}, journal = {GitHub repository}, howpublished =
-{\url{https://github.com/davidpagnon/Sports2D}}, } ### How to contribute I
-would happily welcome any proposal for new features, code improvement, and
-more!\ If you want to contribute to Sports2D, please follow [this guide](https:
-//docs.github.com/en/get-started/quickstart/contributing-to-projects) on how to
-fork, modify and push code, and submit a pull request. I would appreciate it if
-you provided as much useful information as possible about how you modified the
-code, and a rationale for why you're making this pull request. Please also
-specify on which operating system and on which python version you have tested
-the code. *Here is a to-do list: feel free to complete it:* - [x] Compute
-**segment angles** - [x] **Multi-person** detection, consistent over time - [x]
-**Only interpolate small gaps** - [x] **Filtering and plotting tools** - [x]
-Handle sudden **changes of direction** - [x] **Colab version** for those who
-cannot install OpenPose - [ ] Full test on **MacOS** - [ ] **GUI applications**
-for Windows, Mac, and Linux, as well as for Android and iOS (minimal version on
-mobile device, with only BlazePose). Code with [Kivy](https://kivy.org) - [ ]
-**Pose refinement**. Click and move badly estimated 2D points. See [DeepLabCut]
-(https://www.youtube.com/watch?v=bEuBKB7eqmk) for inspiration - [ ] **Include
-OpenPose** in Sports2D executable files. [Dockerize](https://github.com/
-stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile) it? - [ ] **Constrain
-points** to OpenSim skeletal model for better angle estimation (like with
-[Pose2Sim](https://github.com/perfanalytics/pose2sim), but in 2D. BSD 3-Clause
-License Copyright (c) 2022, perfanalytics All rights reserved. Redistribution
-and use in source and binary forms, with or without modification, are permitted
-provided that the following conditions are met: 1. Redistributions of source
-code must retain the above copyright notice, this list of conditions and the
-following disclaimer. 2. Redistributions in binary form must reproduce the
-above copyright notice, this list of conditions and the following disclaimer in
-the documentation and/or other materials provided with the distribution. 3.
-Neither the name of the copyright holder nor the names of its contributors may
-be used to endorse or promote products derived from this software without
-specific prior written permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT
-HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
-INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
-FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
-COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
-INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
-LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
-PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
-LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
-OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
-ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+{2023}, doi= {10.5281/zenodo.7903963}, publisher = {GitHub}, journal = {GitHub
+repository}, howpublished = {\url{https://github.com/davidpagnon/Sports2D}}, }
+### How to contribute I would happily welcome any proposal for new features,
+code improvement, and more!\ If you want to contribute to Sports2D, please
+follow [this guide](https://docs.github.com/en/get-started/quickstart/
+contributing-to-projects) on how to fork, modify and push code, and submit a
+pull request. I would appreciate it if you provided as much useful information
+as possible about how you modified the code, and a rationale for why you're
+making this pull request. Please also specify on which operating system and on
+which python version you have tested the code. *Here is a to-do list: feel free
+to complete it:* - [x] Compute **segment angles**. - [x] **Multi-person**
+detection, consistent over time. - [x] **Only interpolate small gaps**. - [x]
+**Filtering and plotting tools**. - [x] Handle sudden **changes of direction**.
+- [x] **Colab version** for those who cannot install OpenPose. - [ ] Full test
+on **MacOS**. - [ ] **GUI applications** for Windows, Mac, and Linux, as well
+as for Android and iOS (minimal version on mobile device, with only BlazePose).
+Code with [Kivy](https://kivy.org). - [ ] **Include OpenPose** in Sports2D
+executable files. [Dockerize](https://github.com/stanfordnmbl/mobile-gaitlab/
+blob/master/demo/Dockerfile) it? - [ ] **Track other points and angles** with
+classic tracking methods (cf. [Kinovea](https://www.kinovea.org/
+features.html)), or by training a model (cf. [DeepLabCut](https://
+deeplabcut.github.io/DeepLabCut/README.html)). - [ ] **Pose refinement**. Click
+and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/
+watch?v=bEuBKB7eqmk) for inspiration. - [ ] **Constrain points** to OpenSim
+skeletal model for better angle estimation (like with [Pose2Sim](https://
+github.com/perfanalytics/pose2sim), but in 2D. - [ ] Add tools for annotating
+images, undistort them, take perspective into account, etc. (cf. [Kinovea]
+(https://www.kinovea.org/features.html)). BSD 3-Clause License Copyright (c)
+2022, perfanalytics All rights reserved. Redistribution and use in source and
+binary forms, with or without modification, are permitted provided that the
+following conditions are met: 1. Redistributions of source code must retain the
+above copyright notice, this list of conditions and the following disclaimer.
+2. Redistributions in binary form must reproduce the above copyright notice,
+this list of conditions and the following disclaimer in the documentation and/
+or other materials provided with the distribution. 3. Neither the name of the
+copyright holder nor the names of its contributors may be used to endorse or
+promote products derived from this software without specific prior written
+permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
+GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
+HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
+OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `sports2d-0.0.9/sports2d.egg-info/SOURCES.txt` & `sports2d-0.1.0/sports2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

