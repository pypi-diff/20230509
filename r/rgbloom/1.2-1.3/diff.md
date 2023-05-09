# Comparing `tmp/rgbloom-1.2.tar.gz` & `tmp/rgbloom-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgbloom-1.2.tar", last modified: Thu Mar 23 15:55:53 2023, max compression
+gzip compressed data, was "/Users/cardiel/s/rgbloom/dist/.tmp-8du81lci/rgbloom-1.3.tar", last modified: Tue May  9 11:47:14 2023, max compression
```

## Comparing `rgbloom-1.2.tar` & `rgbloom-1.3.tar`

### file list

```diff
@@ -1,37 +1,29 @@
-drwxr-xr-x   0 spr       (1000) spr       (1000)        0 2023-03-23 15:55:53.623129 rgbloom-1.2/
-drwxr-xr-x   0 spr       (1000) spr       (1000)        0 2023-03-23 15:55:53.619129 rgbloom-1.2/.github/
-drwxr-xr-x   0 spr       (1000) spr       (1000)        0 2023-03-23 15:55:53.620128 rgbloom-1.2/.github/workflows/
--rw-r--r--   0 spr       (1000) spr       (1000)      594 2023-03-23 15:44:31.000000 rgbloom-1.2/.github/workflows/test.yml
--rw-r--r--   0 spr       (1000) spr       (1000)      255 2023-03-23 15:44:31.000000 rgbloom-1.2/.gitignore
--rw-r--r--   0 spr       (1000) spr       (1000)    35149 2022-11-15 08:28:58.000000 rgbloom-1.2/LICENSE
--rw-r--r--   0 spr       (1000) spr       (1000)    11692 2023-03-23 15:55:53.623129 rgbloom-1.2/PKG-INFO
--rw-r--r--   0 spr       (1000) spr       (1000)    10902 2023-03-23 15:44:31.000000 rgbloom-1.2/README.md
--rw-r--r--   0 spr       (1000) spr       (1000)      100 2022-11-15 08:28:58.000000 rgbloom-1.2/pyproject.toml
-drwxr-xr-x   0 spr       (1000) spr       (1000)        0 2023-03-23 15:55:53.621128 rgbloom-1.2/rgbloom/
--rw-r--r--   0 spr       (1000) spr       (1000)       51 2022-11-15 08:28:58.000000 rgbloom-1.2/rgbloom/__init__.py
--rw-r--r--   0 spr       (1000) spr       (1000)     5613 2023-03-23 15:44:31.000000 rgbloom-1.2/rgbloom/__main__.py
-drwxr-xr-x   0 spr       (1000) spr       (1000)        0 2023-03-23 15:55:53.622129 rgbloom-1.2/rgbloom/core/
--rw-r--r--   0 spr       (1000) spr       (1000)        0 2022-11-15 08:28:58.000000 rgbloom-1.2/rgbloom/core/__init__.py
--rw-r--r--   0 spr       (1000) spr       (1000)     2487 2022-11-15 08:28:58.000000 rgbloom-1.2/rgbloom/core/step1.py
--rw-r--r--   0 spr       (1000) spr       (1000)     1844 2022-11-15 08:28:58.000000 rgbloom-1.2/rgbloom/core/step2.py
--rw-r--r--   0 spr       (1000) spr       (1000)     3128 2023-03-23 15:44:31.000000 rgbloom-1.2/rgbloom/core/step3.py
--rw-r--r--   0 spr       (1000) spr       (1000)     2560 2022-11-15 08:28:58.000000 rgbloom-1.2/rgbloom/core/step4.py
--rw-r--r--   0 spr       (1000) spr       (1000)     3007 2023-03-23 15:44:31.000000 rgbloom-1.2/rgbloom/core/step5.py
-drwxr-xr-x   0 spr       (1000) spr       (1000)        0 2023-03-23 15:55:53.623129 rgbloom-1.2/rgbloom/gui/
--rw-r--r--   0 spr       (1000) spr       (1000)        0 2022-11-15 08:28:58.000000 rgbloom-1.2/rgbloom/gui/__init__.py
--rw-r--r--   0 spr       (1000) spr       (1000)     7832 2023-03-23 15:44:31.000000 rgbloom-1.2/rgbloom/gui/step6.py
--rw-r--r--   0 spr       (1000) spr       (1000)      497 2022-11-15 08:28:58.000000 rgbloom-1.2/rgbloom/gui/style.py
-drwxr-xr-x   0 spr       (1000) spr       (1000)        0 2023-03-23 15:55:53.623129 rgbloom-1.2/rgbloom/tests/
--rw-r--r--   0 spr       (1000) spr       (1000)        0 2022-11-15 08:28:58.000000 rgbloom-1.2/rgbloom/tests/__init__.py
--rw-r--r--   0 spr       (1000) spr       (1000)     1389 2023-03-23 15:44:31.000000 rgbloom-1.2/rgbloom/tests/test_pleiades.py
--rw-r--r--   0 spr       (1000) spr       (1000)       16 2023-03-23 15:44:31.000000 rgbloom-1.2/rgbloom/version.py
-drwxr-xr-x   0 spr       (1000) spr       (1000)        0 2023-03-23 15:55:53.622129 rgbloom-1.2/rgbloom.egg-info/
--rw-r--r--   0 spr       (1000) spr       (1000)    11692 2023-03-23 15:55:52.000000 rgbloom-1.2/rgbloom.egg-info/PKG-INFO
--rw-r--r--   0 spr       (1000) spr       (1000)      602 2023-03-23 15:55:53.000000 rgbloom-1.2/rgbloom.egg-info/SOURCES.txt
--rw-r--r--   0 spr       (1000) spr       (1000)        1 2023-03-23 15:55:53.000000 rgbloom-1.2/rgbloom.egg-info/dependency_links.txt
--rw-r--r--   0 spr       (1000) spr       (1000)       50 2023-03-23 15:55:53.000000 rgbloom-1.2/rgbloom.egg-info/entry_points.txt
--rw-r--r--   0 spr       (1000) spr       (1000)       80 2023-03-23 15:55:53.000000 rgbloom-1.2/rgbloom.egg-info/requires.txt
--rw-r--r--   0 spr       (1000) spr       (1000)        8 2023-03-23 15:55:53.000000 rgbloom-1.2/rgbloom.egg-info/top_level.txt
--rw-r--r--   0 spr       (1000) spr       (1000)     1040 2023-03-23 15:55:53.624129 rgbloom-1.2/setup.cfg
--rw-r--r--   0 spr       (1000) spr       (1000)       68 2022-11-15 08:28:58.000000 rgbloom-1.2/setup.py
--rw-r--r--   0 spr       (1000) spr       (1000)      363 2023-03-23 15:55:03.000000 rgbloom-1.2/tox.ini
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-09 11:47:14.601941 rgbloom-1.3/
+-rw-r--r--   0 cardiel    (501) staff       (20)    35149 2022-11-06 08:36:25.000000 rgbloom-1.3/LICENSE
+-rw-r--r--   0 cardiel    (501) staff       (20)    11724 2023-05-09 11:47:14.602127 rgbloom-1.3/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)    10934 2023-03-27 18:00:47.000000 rgbloom-1.3/README.md
+-rw-r--r--   0 cardiel    (501) staff       (20)      100 2022-11-06 08:38:35.000000 rgbloom-1.3/pyproject.toml
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-09 11:47:14.595991 rgbloom-1.3/rgbloom/
+-rw-r--r--   0 cardiel    (501) staff       (20)       51 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     5613 2023-03-21 18:25:00.000000 rgbloom-1.3/rgbloom/__main__.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-09 11:47:14.600376 rgbloom-1.3/rgbloom/core/
+-rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/core/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2487 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/core/step1.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1844 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/core/step2.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3128 2023-03-21 17:40:50.000000 rgbloom-1.3/rgbloom/core/step3.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2560 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/core/step4.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3007 2023-03-21 17:42:15.000000 rgbloom-1.3/rgbloom/core/step5.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-09 11:47:14.601605 rgbloom-1.3/rgbloom/gui/
+-rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/gui/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     7832 2023-03-21 18:17:15.000000 rgbloom-1.3/rgbloom/gui/step6.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      497 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/gui/style.py
+-rw-r--r--   0 cardiel    (501) staff       (20)       16 2023-05-09 11:45:51.000000 rgbloom-1.3/rgbloom/version.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-09 11:47:14.598030 rgbloom-1.3/rgbloom.egg-info/
+-rw-r--r--   0 cardiel    (501) staff       (20)    11724 2023-05-09 11:47:14.000000 rgbloom-1.3/rgbloom.egg-info/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)      499 2023-05-09 11:47:14.000000 rgbloom-1.3/rgbloom.egg-info/SOURCES.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        1 2023-05-09 11:47:14.000000 rgbloom-1.3/rgbloom.egg-info/dependency_links.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       50 2023-05-09 11:47:14.000000 rgbloom-1.3/rgbloom.egg-info/entry_points.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       80 2023-05-09 11:47:14.000000 rgbloom-1.3/rgbloom.egg-info/requires.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        8 2023-05-09 11:47:14.000000 rgbloom-1.3/rgbloom.egg-info/top_level.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)     1040 2023-05-09 11:47:14.602878 rgbloom-1.3/setup.cfg
+-rw-r--r--   0 cardiel    (501) staff       (20)       68 2022-11-06 08:39:44.000000 rgbloom-1.3/setup.py
```

### Comparing `rgbloom-1.2/LICENSE` & `rgbloom-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rgbloom-1.2/PKG-INFO` & `rgbloom-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgbloom
-Version: 1.2
+Version: 1.3
 Summary: RGB from Gaia EDR3
 Home-page: https://github.com/guaix-ucm/rgbloom
 Author: Nicolás Cardiel
 Author-email: cardiel@ucm.es
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -188,15 +188,15 @@
       - `RGB_R`: red RGB magnitude estimate
 
   The list of objects in these two files is sorted by right ascension.
 
 - Step 6: generation of a finding chart plot (in PDF format): `rgbloom.pdf`. 
   The execution of the previous example generates a cone search around 
   the [Pleiades](https://en.wikipedia.org/wiki/Pleiades) star cluster:
-  ![Pleiades plot](http://nartex.hst.ucm.es/~ncl/rgbphot/gaiaDR3/pleiades_v4.png)
+  ![Pleiades plot](http://nartex.hst.ucm.es/~ncl/rgbphot/gaiaDR3/pleiades_v5.png)
   The objects in this plot are color coded based on the *Gaia* G_BP - G_RP 
   colour. Stars brighter than a pre-defined threshold are displayed 
   with big star symbols. To facilitate the identification of each object, the
   consecutive identification numbers in the two files `rgbloom_200m.csv` and
   `rgbloom_no200m.csv` are also displayed, in red
   and black, respectively. The identification numbers corresponding to the less
   reliable sources in `rgbloom_20m.csv` (`qlflag=1`) appear inside a rectangle
@@ -259,8 +259,8 @@
 
 <a id="1">Cardiel et al. (2021a)</a>, 
 MNRAS, https://ui.adsabs.harvard.edu/abs/2021MNRAS.504.3730C/abstract
 
 <a id="2">Cardiel et al. (2021b)</a>, 
 MNRAS, https://ui.adsabs.harvard.edu/abs/2021MNRAS.507..318C/abstract
 
-<a id="3">Carrasco et al. (2023)</a>, Remote Sensing, in press
+<a id="3">Carrasco et al. (2023)</a>, Remote Sensing, https://www.mdpi.com/2072-4292/15/7/1767
```

### Comparing `rgbloom-1.2/README.md` & `rgbloom-1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
       - `RGB_R`: red RGB magnitude estimate
 
   The list of objects in these two files is sorted by right ascension.
 
 - Step 6: generation of a finding chart plot (in PDF format): `rgbloom.pdf`. 
   The execution of the previous example generates a cone search around 
   the [Pleiades](https://en.wikipedia.org/wiki/Pleiades) star cluster:
-  ![Pleiades plot](http://nartex.hst.ucm.es/~ncl/rgbphot/gaiaDR3/pleiades_v4.png)
+  ![Pleiades plot](http://nartex.hst.ucm.es/~ncl/rgbphot/gaiaDR3/pleiades_v5.png)
   The objects in this plot are color coded based on the *Gaia* G_BP - G_RP 
   colour. Stars brighter than a pre-defined threshold are displayed 
   with big star symbols. To facilitate the identification of each object, the
   consecutive identification numbers in the two files `rgbloom_200m.csv` and
   `rgbloom_no200m.csv` are also displayed, in red
   and black, respectively. The identification numbers corresponding to the less
   reliable sources in `rgbloom_20m.csv` (`qlflag=1`) appear inside a rectangle
@@ -237,8 +237,8 @@
 
 <a id="1">Cardiel et al. (2021a)</a>, 
 MNRAS, https://ui.adsabs.harvard.edu/abs/2021MNRAS.504.3730C/abstract
 
 <a id="2">Cardiel et al. (2021b)</a>, 
 MNRAS, https://ui.adsabs.harvard.edu/abs/2021MNRAS.507..318C/abstract
 
-<a id="3">Carrasco et al. (2023)</a>, Remote Sensing, in press
+<a id="3">Carrasco et al. (2023)</a>, Remote Sensing, https://www.mdpi.com/2072-4292/15/7/1767
```

### Comparing `rgbloom-1.2/rgbloom/__main__.py` & `rgbloom-1.3/rgbloom/__main__.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.2/rgbloom/core/step1.py` & `rgbloom-1.3/rgbloom/core/step1.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.2/rgbloom/core/step2.py` & `rgbloom-1.3/rgbloom/core/step2.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.2/rgbloom/core/step3.py` & `rgbloom-1.3/rgbloom/core/step3.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.2/rgbloom/core/step4.py` & `rgbloom-1.3/rgbloom/core/step4.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.2/rgbloom/core/step5.py` & `rgbloom-1.3/rgbloom/core/step5.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.2/rgbloom/gui/step6.py` & `rgbloom-1.3/rgbloom/gui/step6.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.2/rgbloom.egg-info/PKG-INFO` & `rgbloom-1.3/rgbloom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgbloom
-Version: 1.2
+Version: 1.3
 Summary: RGB from Gaia EDR3
 Home-page: https://github.com/guaix-ucm/rgbloom
 Author: Nicolás Cardiel
 Author-email: cardiel@ucm.es
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -188,15 +188,15 @@
       - `RGB_R`: red RGB magnitude estimate
 
   The list of objects in these two files is sorted by right ascension.
 
 - Step 6: generation of a finding chart plot (in PDF format): `rgbloom.pdf`. 
   The execution of the previous example generates a cone search around 
   the [Pleiades](https://en.wikipedia.org/wiki/Pleiades) star cluster:
-  ![Pleiades plot](http://nartex.hst.ucm.es/~ncl/rgbphot/gaiaDR3/pleiades_v4.png)
+  ![Pleiades plot](http://nartex.hst.ucm.es/~ncl/rgbphot/gaiaDR3/pleiades_v5.png)
   The objects in this plot are color coded based on the *Gaia* G_BP - G_RP 
   colour. Stars brighter than a pre-defined threshold are displayed 
   with big star symbols. To facilitate the identification of each object, the
   consecutive identification numbers in the two files `rgbloom_200m.csv` and
   `rgbloom_no200m.csv` are also displayed, in red
   and black, respectively. The identification numbers corresponding to the less
   reliable sources in `rgbloom_20m.csv` (`qlflag=1`) appear inside a rectangle
@@ -259,8 +259,8 @@
 
 <a id="1">Cardiel et al. (2021a)</a>, 
 MNRAS, https://ui.adsabs.harvard.edu/abs/2021MNRAS.504.3730C/abstract
 
 <a id="2">Cardiel et al. (2021b)</a>, 
 MNRAS, https://ui.adsabs.harvard.edu/abs/2021MNRAS.507..318C/abstract
 
-<a id="3">Carrasco et al. (2023)</a>, Remote Sensing, in press
+<a id="3">Carrasco et al. (2023)</a>, Remote Sensing, https://www.mdpi.com/2072-4292/15/7/1767
```

### Comparing `rgbloom-1.2/setup.cfg` & `rgbloom-1.3/setup.cfg`

 * *Files identical despite different names*

