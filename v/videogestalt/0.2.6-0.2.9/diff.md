# Comparing `tmp/videogestalt-0.2.6.tar.gz` & `tmp/videogestalt-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "videogestalt-0.2.6.tar", last modified: Mon May  8 22:37:17 2023, max compression
+gzip compressed data, was "videogestalt-0.2.9.tar", last modified: Mon May  8 23:37:39 2023, max compression
```

## Comparing `videogestalt-0.2.6.tar` & `videogestalt-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 22:37:17.737264 videogestalt-0.2.6/
--rw-rw-rw-   0        0        0    16725 2023-05-08 22:34:10.000000 videogestalt-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      194 2023-05-08 22:34:10.000000 videogestalt-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6376 2023-05-08 22:37:17.737264 videogestalt-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     4051 2023-05-08 22:34:10.000000 videogestalt-0.2.6/README.md
--rw-rw-rw-   0        0        0     4872 2023-05-08 22:34:10.000000 videogestalt-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 22:37:17.737264 videogestalt-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      455 2023-05-08 22:34:10.000000 videogestalt-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:37:17.721640 videogestalt-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 22:37:17.737264 videogestalt-0.2.6/src/videogestalt/
--rw-rw-rw-   0        0        0     7302 2023-05-08 22:34:10.000000 videogestalt-0.2.6/src/videogestalt/videogestalt.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:37:17.737264 videogestalt-0.2.6/src/videogestalt.egg-info/
--rw-rw-rw-   0        0        0     6376 2023-05-08 22:37:17.000000 videogestalt-0.2.6/src/videogestalt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-05-08 22:37:17.000000 videogestalt-0.2.6/src/videogestalt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 22:37:17.000000 videogestalt-0.2.6/src/videogestalt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-08 22:37:17.000000 videogestalt-0.2.6/src/videogestalt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2023-05-08 22:37:17.000000 videogestalt-0.2.6/src/videogestalt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-08 22:37:17.000000 videogestalt-0.2.6/src/videogestalt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 23:37:39.960989 videogestalt-0.2.9/
+-rw-rw-rw-   0        0        0    16725 2023-05-08 23:36:18.000000 videogestalt-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      194 2023-05-08 23:36:18.000000 videogestalt-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6422 2023-05-08 23:37:39.960989 videogestalt-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4211 2023-05-08 23:36:18.000000 videogestalt-0.2.9/README.md
+-rw-rw-rw-   0        0        0     4731 2023-05-08 23:36:18.000000 videogestalt-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 23:37:39.960989 videogestalt-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      455 2023-05-08 23:36:18.000000 videogestalt-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:37:39.945373 videogestalt-0.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 23:37:39.945373 videogestalt-0.2.9/src/videogestalt/
+-rw-rw-rw-   0        0        0     7302 2023-05-08 23:36:18.000000 videogestalt-0.2.9/src/videogestalt/videogestalt.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:37:39.960989 videogestalt-0.2.9/src/videogestalt.egg-info/
+-rw-rw-rw-   0        0        0     6422 2023-05-08 23:37:39.000000 videogestalt-0.2.9/src/videogestalt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-05-08 23:37:39.000000 videogestalt-0.2.9/src/videogestalt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 23:37:39.000000 videogestalt-0.2.9/src/videogestalt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-08 23:37:39.000000 videogestalt-0.2.9/src/videogestalt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2023-05-08 23:37:39.000000 videogestalt-0.2.9/src/videogestalt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-08 23:37:39.000000 videogestalt-0.2.9/src/videogestalt.egg-info/top_level.txt
```

### Comparing `videogestalt-0.2.6/LICENSE` & `videogestalt-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `videogestalt-0.2.6/PKG-INFO` & `videogestalt-0.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: videogestalt
-Version: 0.2.6
-Summary: Regular Expression Path Matcher - Easily batch manipulate folders and files trees with regular expression!
+Version: 0.2.9
+Summary: One-Glance Overview of Any Video
 Author-email: Eamonn O'Brien-Strain <eobrain@proton.me>
-Maintainer-email: Eamonn O'Brien-Strain <eobrain@proton.me>, Stephen Karl Larroque <lrq3000@gmail.com>
+Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
 License: Mozilla Public License 2.0
 Project-URL: Homepage, https://github.com/eobrain/videogestalt
 Project-URL: Documentation, https://github.com/eobrain/videogestalt/blob/master/README.md
 Project-URL: Source, https://github.com/eobrain/videogestalt
 Project-URL: Tracker, https://github.com/eobrain/videogestalt/issues
 Project-URL: Download, https://github.com/eobrain/videogestalt/releases
 Keywords: video,gestalt,movie,summary,summarization,thumbnails
@@ -38,23 +38,26 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: testmeta
 License-File: LICENSE
 
+[![videogestalt-logo][6]
 # Video Gestalt
 
-[![PyPI-Status][1]][2] [![PyPI-Versions][3]][4] [![PyPI-Downloads][5]][6]
+[![PyPI-Status][1]][2] [![PyPI-Versions][3]][2] [![PyPi-License][4]][2] [![PyPI-Downloads][5]][2]
 
 [![Build-Status][7]][8] [![Coverage-Status][9]][10]
 
+One-Glance Overview of Any Video
+
 [![Example video gestalt: Vespa-Scooter-Commercial][11]][12]
 
-Presents a video in a summary form that shows the entire video at once as an array of moving video thumbnails.
+Video Gestalt displays a video in a summary form that shows the entire video at once as an array of moving video thumbnails.
 
 ## Description
 
 Video Gestalt presents a condensed video array, showing the entire video at once as moving video thumbnails.
 
 The above is an example of the Video Gestalt for a 50-second commercial for Vesta scooters. (Click the Video Gestalt to see the original video.)
 
@@ -133,16 +136,16 @@
 Created by Eamonn O'Brien-Strain.
 
 Licensed under the Mozilla Public License 2.0
 
 [1]: https://img.shields.io/pypi/v/videogestalt.svg
 [2]: https://pypi.org/project/videogestalt
 [3]: https://img.shields.io/pypi/pyversions/videogestalt.svg?logo=python&logoColor=white
-[4]: https://pypi.org/project/videogestalt
+[4]: https://img.shields.io/pypi/l/videogestalt.svg
 [5]: https://img.shields.io/pypi/dm/videogestalt.svg?label=pypi%20downloads&logo=python&logoColor=white
-[6]: https://pypi.org/project/videogestalt
+[6]: https://raw.githubusercontent.com/eobrain/videogestalt/main/resources/videogestalt_logo.png
 [7]: https://github.com/eobrain/videogestalt/actions/workflows/ci-build.yml/badge.svg?event=push
 [8]: https://github.com/eobrain/videogestalt/actions/workflows/ci-build.yml
 [9]: https://codecov.io/github/eobrain/videogestalt/coverage.svg?branch=master
 [10]: https://codecov.io/github/eobrain/videogestalt?branch=master
 [11]: https://raw.githubusercontent.com/eobrain/videogestalt/main/resources/vespa-commercial-gestalt.gif
 [12]: https://ia904607.us.archive.org/11/items/vespa-scooter-commercial/Vespa%20Scooter%20Commercial.mp4
```

### Comparing `videogestalt-0.2.6/README.md` & `videogestalt-0.2.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+[![videogestalt-logo][6]
 # Video Gestalt
 
-[![PyPI-Status][1]][2] [![PyPI-Versions][3]][4] [![PyPI-Downloads][5]][6]
+[![PyPI-Status][1]][2] [![PyPI-Versions][3]][2] [![PyPi-License][4]][2] [![PyPI-Downloads][5]][2]
 
 [![Build-Status][7]][8] [![Coverage-Status][9]][10]
 
+One-Glance Overview of Any Video
+
 [![Example video gestalt: Vespa-Scooter-Commercial][11]][12]
 
-Presents a video in a summary form that shows the entire video at once as an array of moving video thumbnails.
+Video Gestalt displays a video in a summary form that shows the entire video at once as an array of moving video thumbnails.
 
 ## Description
 
 Video Gestalt presents a condensed video array, showing the entire video at once as moving video thumbnails.
 
 The above is an example of the Video Gestalt for a 50-second commercial for Vesta scooters. (Click the Video Gestalt to see the original video.)
 
@@ -89,16 +92,16 @@
 Created by Eamonn O'Brien-Strain.
 
 Licensed under the Mozilla Public License 2.0
 
 [1]: https://img.shields.io/pypi/v/videogestalt.svg
 [2]: https://pypi.org/project/videogestalt
 [3]: https://img.shields.io/pypi/pyversions/videogestalt.svg?logo=python&logoColor=white
-[4]: https://pypi.org/project/videogestalt
+[4]: https://img.shields.io/pypi/l/videogestalt.svg
 [5]: https://img.shields.io/pypi/dm/videogestalt.svg?label=pypi%20downloads&logo=python&logoColor=white
-[6]: https://pypi.org/project/videogestalt
+[6]: https://raw.githubusercontent.com/eobrain/videogestalt/main/resources/videogestalt_logo.png
 [7]: https://github.com/eobrain/videogestalt/actions/workflows/ci-build.yml/badge.svg?event=push
 [8]: https://github.com/eobrain/videogestalt/actions/workflows/ci-build.yml
 [9]: https://codecov.io/github/eobrain/videogestalt/coverage.svg?branch=master
 [10]: https://codecov.io/github/eobrain/videogestalt?branch=master
 [11]: https://raw.githubusercontent.com/eobrain/videogestalt/main/resources/vespa-commercial-gestalt.gif
 [12]: https://ia904607.us.archive.org/11/items/vespa-scooter-commercial/Vespa%20Scooter%20Commercial.mp4
```

### Comparing `videogestalt-0.2.6/pyproject.toml` & `videogestalt-0.2.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 [build-system]
 # never uppercap requirements unless we have evidence it won't work https://iscinumpy.dev/post/bound-version-constraints/ 
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]  # beware if using setuptools: setup.py still gets executed, and even if pyproject.toml fields take precedence, if there is any code error in setup.py, building will fail!
 name = "videogestalt"
-version = "0.2.6"  # see PEP 440 https://peps.python.org/pep-0440/#pre-releases and https://packaging.python.org/en/latest/guides/single-sourcing-package-version/
-description = "Regular Expression Path Matcher - Easily batch manipulate folders and files trees with regular expression!"
+version = "0.2.9"  # see PEP 440 https://peps.python.org/pep-0440/#pre-releases and https://packaging.python.org/en/latest/guides/single-sourcing-package-version/
+description = "One-Glance Overview of Any Video"
 authors = [
     {name = "Eamonn O'Brien-Strain", email = "eobrain@proton.me"},
     ]
 maintainers = [
-    {name = "Eamonn O'Brien-Strain", email = "eobrain@proton.me"},
     {name = "Stephen Karl Larroque", email = "lrq3000@gmail.com"},
     ]
 requires-python = ">=3.7"
 license = {text = "Mozilla Public License 2.0"} # { file = "LICENSE" }
 keywords = ["video", "gestalt", "movie", "summary", "summarization", "thumbnails"]
 classifiers = [
     'Development Status :: 3 - Alpha',
```

### Comparing `videogestalt-0.2.6/src/videogestalt/videogestalt.py` & `videogestalt-0.2.9/src/videogestalt/videogestalt.py`

 * *Files identical despite different names*

### Comparing `videogestalt-0.2.6/src/videogestalt.egg-info/PKG-INFO` & `videogestalt-0.2.9/src/videogestalt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: videogestalt
-Version: 0.2.6
-Summary: Regular Expression Path Matcher - Easily batch manipulate folders and files trees with regular expression!
+Version: 0.2.9
+Summary: One-Glance Overview of Any Video
 Author-email: Eamonn O'Brien-Strain <eobrain@proton.me>
-Maintainer-email: Eamonn O'Brien-Strain <eobrain@proton.me>, Stephen Karl Larroque <lrq3000@gmail.com>
+Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
 License: Mozilla Public License 2.0
 Project-URL: Homepage, https://github.com/eobrain/videogestalt
 Project-URL: Documentation, https://github.com/eobrain/videogestalt/blob/master/README.md
 Project-URL: Source, https://github.com/eobrain/videogestalt
 Project-URL: Tracker, https://github.com/eobrain/videogestalt/issues
 Project-URL: Download, https://github.com/eobrain/videogestalt/releases
 Keywords: video,gestalt,movie,summary,summarization,thumbnails
@@ -38,23 +38,26 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: testmeta
 License-File: LICENSE
 
+[![videogestalt-logo][6]
 # Video Gestalt
 
-[![PyPI-Status][1]][2] [![PyPI-Versions][3]][4] [![PyPI-Downloads][5]][6]
+[![PyPI-Status][1]][2] [![PyPI-Versions][3]][2] [![PyPi-License][4]][2] [![PyPI-Downloads][5]][2]
 
 [![Build-Status][7]][8] [![Coverage-Status][9]][10]
 
+One-Glance Overview of Any Video
+
 [![Example video gestalt: Vespa-Scooter-Commercial][11]][12]
 
-Presents a video in a summary form that shows the entire video at once as an array of moving video thumbnails.
+Video Gestalt displays a video in a summary form that shows the entire video at once as an array of moving video thumbnails.
 
 ## Description
 
 Video Gestalt presents a condensed video array, showing the entire video at once as moving video thumbnails.
 
 The above is an example of the Video Gestalt for a 50-second commercial for Vesta scooters. (Click the Video Gestalt to see the original video.)
 
@@ -133,16 +136,16 @@
 Created by Eamonn O'Brien-Strain.
 
 Licensed under the Mozilla Public License 2.0
 
 [1]: https://img.shields.io/pypi/v/videogestalt.svg
 [2]: https://pypi.org/project/videogestalt
 [3]: https://img.shields.io/pypi/pyversions/videogestalt.svg?logo=python&logoColor=white
-[4]: https://pypi.org/project/videogestalt
+[4]: https://img.shields.io/pypi/l/videogestalt.svg
 [5]: https://img.shields.io/pypi/dm/videogestalt.svg?label=pypi%20downloads&logo=python&logoColor=white
-[6]: https://pypi.org/project/videogestalt
+[6]: https://raw.githubusercontent.com/eobrain/videogestalt/main/resources/videogestalt_logo.png
 [7]: https://github.com/eobrain/videogestalt/actions/workflows/ci-build.yml/badge.svg?event=push
 [8]: https://github.com/eobrain/videogestalt/actions/workflows/ci-build.yml
 [9]: https://codecov.io/github/eobrain/videogestalt/coverage.svg?branch=master
 [10]: https://codecov.io/github/eobrain/videogestalt?branch=master
 [11]: https://raw.githubusercontent.com/eobrain/videogestalt/main/resources/vespa-commercial-gestalt.gif
 [12]: https://ia904607.us.archive.org/11/items/vespa-scooter-commercial/Vespa%20Scooter%20Commercial.mp4
```

