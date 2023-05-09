# Comparing `tmp/oursin-0.4.5.tar.gz` & `tmp/oursin-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oursin-0.4.5.tar", last modified: Mon Apr 17 21:55:32 2023, max compression
+gzip compressed data, was "oursin-0.4.7.tar", last modified: Tue May  9 18:47:31 2023, max compression
```

## Comparing `oursin-0.4.5.tar` & `oursin-0.4.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 21:55:32.650126 oursin-0.4.5/
--rw-rw-rw-   0        0        0    35823 2023-01-24 19:55:46.000000 oursin-0.4.5/LICENSE
--rw-rw-rw-   0        0        0    42009 2023-04-17 21:55:32.650126 oursin-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-02-15 20:37:09.000000 oursin-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 21:55:32.547171 oursin-0.4.5/oursin/
--rw-rw-rw-   0        0        0      545 2023-02-15 20:37:09.000000 oursin-0.4.5/oursin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:55:32.640119 oursin-0.4.5/oursin/atlas/
--rw-rw-rw-   0        0        0       17 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/atlas/__init__.py
--rw-rw-rw-   0        0        0     3786 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/atlas/ccf.py
--rw-rw-rw-   0        0        0     3589 2023-04-17 21:53:19.000000 oursin-0.4.5/oursin/camera.py
--rw-rw-rw-   0        0        0     1244 2023-04-17 21:53:19.000000 oursin-0.4.5/oursin/client.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:55:32.648132 oursin-0.4.5/oursin/colors/
--rw-rw-rw-   0        0        0       46 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/colors/__init__.py
--rw-rw-rw-   0        0        0     4531 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/colors/colors.py
--rw-rw-rw-   0        0        0    36410 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/colors/xkcd_rgb.py
--rw-rw-rw-   0        0        0     1214 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/lines.py
--rw-rw-rw-   0        0        0     2487 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/neurons.py
--rw-rw-rw-   0        0        0     1904 2023-04-17 21:53:19.000000 oursin-0.4.5/oursin/primitives.py
--rw-rw-rw-   0        0        0     2438 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/probes.py
--rw-rw-rw-   0        0        0     1514 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/renderer.py
--rw-rw-rw-   0        0        0     1927 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/text.py
--rw-rw-rw-   0        0        0     3524 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/volumes.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:55:32.622105 oursin-0.4.5/oursin.egg-info/
--rw-rw-rw-   0        0        0    42009 2023-04-17 21:55:32.000000 oursin-0.4.5/oursin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-17 21:55:32.000000 oursin-0.4.5/oursin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 21:55:32.000000 oursin-0.4.5/oursin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-17 21:55:32.000000 oursin-0.4.5/oursin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 21:55:32.000000 oursin-0.4.5/oursin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      772 2023-04-17 21:53:19.000000 oursin-0.4.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 21:55:32.658106 oursin-0.4.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 18:47:31.942548 oursin-0.4.7/
+-rw-rw-rw-   0        0        0    35823 2023-01-24 19:55:46.000000 oursin-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0    42009 2023-05-09 18:47:31.943546 oursin-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-02-15 20:37:09.000000 oursin-0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 18:47:31.884624 oursin-0.4.7/oursin/
+-rw-rw-rw-   0        0        0      545 2023-05-09 18:47:07.000000 oursin-0.4.7/oursin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:47:31.933534 oursin-0.4.7/oursin/atlas/
+-rw-rw-rw-   0        0        0       17 2023-02-15 20:37:10.000000 oursin-0.4.7/oursin/atlas/__init__.py
+-rw-rw-rw-   0        0        0     3786 2023-02-15 20:37:10.000000 oursin-0.4.7/oursin/atlas/ccf.py
+-rw-rw-rw-   0        0        0     3589 2023-04-17 22:07:09.000000 oursin-0.4.7/oursin/camera.py
+-rw-rw-rw-   0        0        0     1244 2023-04-17 23:49:59.000000 oursin-0.4.7/oursin/client.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:47:31.940562 oursin-0.4.7/oursin/colors/
+-rw-rw-rw-   0        0        0       46 2023-02-15 20:37:10.000000 oursin-0.4.7/oursin/colors/__init__.py
+-rw-rw-rw-   0        0        0     4531 2023-02-15 20:37:10.000000 oursin-0.4.7/oursin/colors/colors.py
+-rw-rw-rw-   0        0        0    36410 2023-02-15 20:37:10.000000 oursin-0.4.7/oursin/colors/xkcd_rgb.py
+-rw-rw-rw-   0        0        0     1214 2023-02-15 20:37:10.000000 oursin-0.4.7/oursin/lines.py
+-rw-rw-rw-   0        0        0     2487 2023-02-15 20:37:10.000000 oursin-0.4.7/oursin/neurons.py
+-rw-rw-rw-   0        0        0     1904 2023-04-17 22:07:09.000000 oursin-0.4.7/oursin/primitives.py
+-rw-rw-rw-   0        0        0     2438 2023-02-15 20:37:10.000000 oursin-0.4.7/oursin/probes.py
+-rw-rw-rw-   0        0        0     1514 2023-02-15 20:37:10.000000 oursin-0.4.7/oursin/renderer.py
+-rw-rw-rw-   0        0        0     1927 2023-02-15 20:37:10.000000 oursin-0.4.7/oursin/text.py
+-rw-rw-rw-   0        0        0     3524 2023-02-15 20:37:10.000000 oursin-0.4.7/oursin/volumes.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:47:31.928547 oursin-0.4.7/oursin.egg-info/
+-rw-rw-rw-   0        0        0    42009 2023-05-09 18:47:31.000000 oursin-0.4.7/oursin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-05-09 18:47:31.000000 oursin-0.4.7/oursin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 18:47:31.000000 oursin-0.4.7/oursin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-09 18:47:31.000000 oursin-0.4.7/oursin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-09 18:47:31.000000 oursin-0.4.7/oursin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      803 2023-05-09 18:46:54.000000 oursin-0.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 18:47:31.945540 oursin-0.4.7/setup.cfg
```

### Comparing `oursin-0.4.5/LICENSE` & `oursin-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oursin-0.4.5/PKG-INFO` & `oursin-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oursin
-Version: 0.4.5
+Version: 0.4.7
 Summary: Urchin - Universal Renderer Creating Helpful Images for Neuroscience Python API
 Author-email: Daniel Birman <danbirman@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,15 +674,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://virtualbrainlab.org/03_unity_neuro/01_urn_intro.html
+Project-URL: Homepage, https://virtualbrainlab.org/urchin/installation_and_use.html
 Project-URL: Bug Tracker, https://github.com/VirtualBrainLab/Urchin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oursin-0.4.5/oursin/__init__.py` & `oursin-0.4.7/oursin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 urchin.
 
 Python library for connecting to and sending data to a Universal Renderer for Neuroscience renderer.
 """
 __author__ = 'Daniel Birman'
-__version__ = "0.4.4"
+__version__ = "0.4.7"
 
 # load the client
 from . import client
 from .renderer import *
 
 # load the scene controls
 from . import camera
```

### Comparing `oursin-0.4.5/oursin/atlas/ccf.py` & `oursin-0.4.7/oursin/atlas/ccf.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.5/oursin/camera.py` & `oursin-0.4.7/oursin/camera.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.5/oursin/client.py` & `oursin-0.4.7/oursin/client.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.5/oursin/colors/colors.py` & `oursin-0.4.7/oursin/colors/colors.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.5/oursin/colors/xkcd_rgb.py` & `oursin-0.4.7/oursin/colors/xkcd_rgb.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.5/oursin/lines.py` & `oursin-0.4.7/oursin/lines.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.5/oursin/neurons.py` & `oursin-0.4.7/oursin/neurons.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.5/oursin/primitives.py` & `oursin-0.4.7/oursin/primitives.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.5/oursin/probes.py` & `oursin-0.4.7/oursin/probes.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.5/oursin/renderer.py` & `oursin-0.4.7/oursin/renderer.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.5/oursin/text.py` & `oursin-0.4.7/oursin/text.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.5/oursin/volumes.py` & `oursin-0.4.7/oursin/volumes.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.5/oursin.egg-info/PKG-INFO` & `oursin-0.4.7/oursin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oursin
-Version: 0.4.5
+Version: 0.4.7
 Summary: Urchin - Universal Renderer Creating Helpful Images for Neuroscience Python API
 Author-email: Daniel Birman <danbirman@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,15 +674,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://virtualbrainlab.org/03_unity_neuro/01_urn_intro.html
+Project-URL: Homepage, https://virtualbrainlab.org/urchin/installation_and_use.html
 Project-URL: Bug Tracker, https://github.com/VirtualBrainLab/Urchin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oursin-0.4.5/pyproject.toml` & `oursin-0.4.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "oursin"
-version = "0.4.5"
+version = "0.4.7"
 authors = [
   { name="Daniel Birman", email="danbirman@gmail.com" },
 ]
 description = "Urchin - Universal Renderer Creating Helpful Images for Neuroscience Python API"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "python-socketio[client]",
-  "numpy",
-  "PIL"
+  "python-socketio[client] ~= 5.8.0",
+  "numpy ~= 1.24.3",
+  "Pillow ~= 9.5.0"
 ]
 
 [project.urls]
-"Homepage" = "https://virtualbrainlab.org/03_unity_neuro/01_urn_intro.html"
+"Homepage" = "https://virtualbrainlab.org/urchin/installation_and_use.html"
 "Bug Tracker" = "https://github.com/VirtualBrainLab/Urchin/issues"
```

