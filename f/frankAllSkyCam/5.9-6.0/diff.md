# Comparing `tmp/frankAllSkyCam-5.9.tar.gz` & `tmp/frankAllSkyCam-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frankAllSkyCam-5.9.tar", last modified: Sun May  7 07:59:05 2023, max compression
+gzip compressed data, was "frankAllSkyCam-6.0.tar", last modified: Mon May  8 22:14:22 2023, max compression
```

## Comparing `frankAllSkyCam-5.9.tar` & `frankAllSkyCam-6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 07:59:05.198250 frankAllSkyCam-5.9/
--rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-05-07 07:59:05.198250 frankAllSkyCam-5.9/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 07:59:05.198250 frankAllSkyCam-5.9/frankAllSkyCam/
--rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-05-07 07:54:34.672446 frankAllSkyCam-5.9/frankAllSkyCam/__init__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3315 2023-05-06 17:05:56.950266 frankAllSkyCam-5.9/frankAllSkyCam/__main__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)      860 2023-05-06 07:38:43.382734 frankAllSkyCam-5.9/frankAllSkyCam/allskycamdelete.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3109 2023-05-06 17:19:03.927275 frankAllSkyCam-5.9/frankAllSkyCam/config.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3413 2023-05-06 06:51:58.022772 frankAllSkyCam-5.9/frankAllSkyCam/crontab.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     1484 2023-05-06 19:44:03.235757 frankAllSkyCam-5.9/frankAllSkyCam/drawtext.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3492 2023-05-06 10:16:56.461921 frankAllSkyCam-5.9/frankAllSkyCam/fileManager.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)    17973 2023-05-06 07:53:00.118852 frankAllSkyCam-5.9/frankAllSkyCam/imageHeader.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-04-30 21:24:45.893867 frankAllSkyCam-5.9/frankAllSkyCam/index.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     2952 2023-05-06 07:38:13.134641 frankAllSkyCam-5.9/frankAllSkyCam/startrail.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-04-30 21:24:46.401862 frankAllSkyCam-5.9/frankAllSkyCam/suncalc2.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-30 21:24:46.401862 frankAllSkyCam-5.9/frankAllSkyCam/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-05-06 06:49:45.473215 frankAllSkyCam-5.9/frankAllSkyCam/test_suncalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     4312 2023-05-07 07:53:56.040788 frankAllSkyCam-5.9/frankAllSkyCam/timelapse.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1397 2023-05-06 07:37:43.869298 frankAllSkyCam-5.9/frankAllSkyCam/watchDog.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-5.9/setup.cfg
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1824 2023-05-07 07:55:28.139972 frankAllSkyCam-5.9/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-08 22:14:22.873233 frankAllSkyCam-6.0/
+-rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-05-08 22:14:22.877233 frankAllSkyCam-6.0/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-08 22:14:22.873233 frankAllSkyCam-6.0/frankAllSkyCam/
+-rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-05-08 22:11:47.838363 frankAllSkyCam-6.0/frankAllSkyCam/__init__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3315 2023-05-06 17:05:56.950266 frankAllSkyCam-6.0/frankAllSkyCam/__main__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)      860 2023-05-06 07:38:43.382734 frankAllSkyCam-6.0/frankAllSkyCam/allskycamdelete.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3109 2023-05-06 17:19:03.927275 frankAllSkyCam-6.0/frankAllSkyCam/config.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3413 2023-05-06 06:51:58.022772 frankAllSkyCam-6.0/frankAllSkyCam/crontab.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     1484 2023-05-06 19:44:03.235757 frankAllSkyCam-6.0/frankAllSkyCam/drawtext.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3492 2023-05-06 10:16:56.461921 frankAllSkyCam-6.0/frankAllSkyCam/fileManager.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)    17978 2023-05-08 21:06:40.797062 frankAllSkyCam-6.0/frankAllSkyCam/imageHeader.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-04-30 21:24:45.893867 frankAllSkyCam-6.0/frankAllSkyCam/index.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2952 2023-05-06 07:38:13.134641 frankAllSkyCam-6.0/frankAllSkyCam/startrail.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-04-30 21:24:46.401862 frankAllSkyCam-6.0/frankAllSkyCam/suncalc2.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-30 21:24:46.401862 frankAllSkyCam-6.0/frankAllSkyCam/test_sqm.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-05-06 06:49:45.473215 frankAllSkyCam-6.0/frankAllSkyCam/test_suncalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     4312 2023-05-07 07:53:56.040788 frankAllSkyCam-6.0/frankAllSkyCam/timelapse.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1397 2023-05-06 07:37:43.869298 frankAllSkyCam-6.0/frankAllSkyCam/watchDog.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-6.0/setup.cfg
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1824 2023-05-08 22:11:26.855139 frankAllSkyCam-6.0/setup.py
```

### Comparing `frankAllSkyCam-5.9/PKG-INFO` & `frankAllSkyCam-6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: frankAllSkyCam
-Version: 5.9
+Version: 6.0
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/5.9.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/6.0.tar.gz
 Description: UNKNOWN
 Keywords: AllSkyCamera,Astronomy,AllSky
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/__main__.py` & `frankAllSkyCam-6.0/frankAllSkyCam/__main__.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/allskycamdelete.py` & `frankAllSkyCam-6.0/frankAllSkyCam/allskycamdelete.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/config.py` & `frankAllSkyCam-6.0/frankAllSkyCam/config.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/crontab.py` & `frankAllSkyCam-6.0/frankAllSkyCam/crontab.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/drawtext.py` & `frankAllSkyCam-6.0/frankAllSkyCam/drawtext.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/fileManager.py` & `frankAllSkyCam-6.0/frankAllSkyCam/fileManager.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/imageHeader.py` & `frankAllSkyCam-6.0/frankAllSkyCam/imageHeader.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,25 +350,26 @@
    smt_prima = suncalc2.getMoonTimes(datacalcolo+timedelta(days=-1), latitude, longitude)
    smt_dopo  = suncalc2.getMoonTimes(datacalcolo+timedelta(days=1), latitude, longitude)
 
    try:
       mrise= smt["rise"].astimezone(tz)
       moon_rise = str(mrise)[11:16]
    except:
-      mset="--"
-      moon_set="--"
+      mrise="--"
+      moon_rise="--"
 
 
    try:
       mset= smt["set"].astimezone(tz)
       moon_set = str(mset)[11:16]
    except:
       mset="--"
       moon_set="--"
 
+  
    if moon_rise!="--" and moon_set!="--":
       if mrise > mset and datacalcolo > mrise:
          if datacalcolo <=mset:
             # mrise del giorno prima
             mrise= "--"
             moon_rise = "--"
          elif (datacalcolo > mset and datacalcolo < mrise) or (datacalcolo >=mrise):
```

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/startrail.py` & `frankAllSkyCam-6.0/frankAllSkyCam/startrail.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/suncalc2.py` & `frankAllSkyCam-6.0/frankAllSkyCam/suncalc2.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/test_sqm.py` & `frankAllSkyCam-6.0/frankAllSkyCam/test_sqm.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/test_suncalc.py` & `frankAllSkyCam-6.0/frankAllSkyCam/test_suncalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/timelapse.py` & `frankAllSkyCam-6.0/frankAllSkyCam/timelapse.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/frankAllSkyCam/watchDog.py` & `frankAllSkyCam-6.0/frankAllSkyCam/watchDog.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-5.9/setup.py` & `frankAllSkyCam-6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'frankAllSkyCam',         # How you named your package folder (MyLib)
   packages = ['frankAllSkyCam'],   # Chose the same as "name"
-  version = '5.9',      # Start with a small number and increase it with every change you make
+  version = '6.0',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'AllSkyCamera with Raspberry Pi and Pi HQ Camera ',   # Give a short description about your library
   author = 'Francesco Sferlazza',                   # Type in your name
   author_email = 'sferlazza@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/sferlix/frankAllSkyCam',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/5.9.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/6.0.tar.gz',    # I explain this later on
   keywords = ['AllSkyCamera', 'Astronomy', 'AllSky'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'pytz',
           'numpy',
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

