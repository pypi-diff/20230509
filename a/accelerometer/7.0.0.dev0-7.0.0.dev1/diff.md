# Comparing `tmp/accelerometer-7.0.0.dev0.tar.gz` & `tmp/accelerometer-7.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelerometer-7.0.0.dev0.tar", last modified: Mon Apr 24 18:09:04 2023, max compression
+gzip compressed data, was "accelerometer-7.0.0.dev1.tar", last modified: Tue May  9 20:36:47 2023, max compression
```

## Comparing `accelerometer-7.0.0.dev0.tar` & `accelerometer-7.0.0.dev1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:09:04.028379 accelerometer-7.0.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-24 18:09:04.028379 accelerometer-7.0.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:09:04.028379 accelerometer-7.0.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:09:04.012379 accelerometer-7.0.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:09:04.028379 accelerometer-7.0.0.dev0/src/accelerometer/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-24 18:09:04.028379 accelerometer-7.0.0.dev0/src/accelerometer/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/accCollateSummary.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/accPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/accProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/accWriteCmds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:09:04.016379 accelerometer-7.0.0.dev0/src/accelerometer/activityModels/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/activityModels/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/circadian.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    22477 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:09:04.024379 accelerometer-7.0.0.dev0/src/accelerometer/java/
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/AccStats.class
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/AccStats.java
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/AccelerometerParser.class
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/AccelerometerParser.java
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/ActigraphReader.class
--rw-r--r--   0 runner    (1001) docker     (123)    29730 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/ActigraphReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/AxivityReader.class
--rw-r--r--   0 runner    (1001) docker     (123)    16174 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/AxivityReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/BandpassFilter.class
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/BandpassFilter.java
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/CsvReader.class
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/CsvReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/DeviceReader.class
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/DeviceReader.java
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/EpochWriter.class
--rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/EpochWriter.java
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/Features.class
--rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/Features.java
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/Filter.class
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/Filter.java
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/GENEActivReader.class
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/GENEActivReader.java
--rw-r--r--   0 runner    (1001) docker     (123)  1501730 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/JTransforms-3.1-with-dependencies.jar
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/LowpassFilter.class
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/LowpassFilter.java
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/NpyWriter.class
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/NpyWriter.java
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/Resample.class
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/Resample.java
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/logging.properties
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/summarisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:09:04.016379 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-24 18:09:03.000000 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-24 18:09:03.000000 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:09:03.000000 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 18:09:03.000000 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-24 18:09:03.000000 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 18:09:03.000000 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:36:47.929013 accelerometer-7.0.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-09 20:36:47.929013 accelerometer-7.0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 20:36:47.929013 accelerometer-7.0.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:36:47.921013 accelerometer-7.0.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:36:47.929013 accelerometer-7.0.0.dev1/src/accelerometer/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 20:36:47.929013 accelerometer-7.0.0.dev1/src/accelerometer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/accCollateSummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/accPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/accProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/accWriteCmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:36:47.925013 accelerometer-7.0.0.dev1/src/accelerometer/activityModels/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/activityModels/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/circadian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22477 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:36:47.929013 accelerometer-7.0.0.dev1/src/accelerometer/java/
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/AccStats.class
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/AccStats.java
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/AccelerometerParser.class
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/AccelerometerParser.java
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/ActigraphReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    29730 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/ActigraphReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/AxivityReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    16174 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/AxivityReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/BandpassFilter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/BandpassFilter.java
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/CsvReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/CsvReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/DeviceReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/DeviceReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/EpochWriter.class
+-rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/EpochWriter.java
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/Features.class
+-rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/Features.java
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/Filter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/Filter.java
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/GENEActivReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/GENEActivReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)  1501730 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/JTransforms-3.1-with-dependencies.jar
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/LowpassFilter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/LowpassFilter.java
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/NpyWriter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/NpyWriter.java
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-09 20:36:34.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/Resample.class
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/Resample.java
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/logging.properties
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/summarisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:36:47.925013 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-09 20:36:47.000000 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-09 20:36:47.000000 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:36:47.000000 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-09 20:36:47.000000 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-09 20:36:47.000000 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 20:36:47.000000 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/versioneer.py
```

### Comparing `accelerometer-7.0.0.dev0/LICENSE.md` & `accelerometer-7.0.0.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/PKG-INFO` & `accelerometer-7.0.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelerometer
-Version: 7.0.0.dev0
+Version: 7.0.0.dev1
 Summary: A package to extract meaningful health information from large accelerometer datasets e.g. how much time individuals spend in sleep, sedentary behaviour, walking and moderate intensity physical activity
 Home-page: https://github.com/activityMonitoring/biobankAccelerometerAnalysis
 Download-URL: https://github.com/activityMonitoring/biobankAccelerometerAnalysis
 Author: Aiden Doherty, Shing Chan, Rosemary Walmsley, Hang Yuan
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE.md
 Keywords: wearables,accelerometer,health data science,human activity recognition
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.7
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.md
 
 ![Accelerometer data processing overview](docs/source/accelerometerLogo.png)
```

### Comparing `accelerometer-7.0.0.dev0/README.md` & `accelerometer-7.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/pyproject.toml` & `accelerometer-7.0.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/setup.py` & `accelerometer-7.0.0.dev1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         raise RuntimeError(f"Unable to find {string}.")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="accelerometer",
-    python_requires=">=3.7",
+    python_requires=">=3.7, <3.11",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description="A package to extract meaningful health information from large accelerometer datasets e.g. how much time individuals spend in sleep, sedentary behaviour, walking and moderate intensity physical activity",
     keywords="wearables, accelerometer, health data science, human activity recognition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/activityMonitoring/biobankAccelerometerAnalysis",
@@ -47,32 +47,32 @@
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Medical Science Apps.",
     ],
     packages=setuptools.find_packages(where="src", exclude=("test", "tests")),
     package_dir={"": "src"},
     include_package_data=True,
     install_requires=[
-        'numpy',
-        'scipy',
-        'matplotlib',
-        'pandas>=1.2.5',
-        'tqdm>=4.59.0',
-        'statsmodels>=0.12.2',
+        'numpy==1.21.*',
+        'scipy==1.7.*',
+        'matplotlib==3.5.*',
+        'pandas==1.3.*',
+        'tqdm==4.65.*',
+        'statsmodels==0.13.*',
+        'joblib==1.1.*',
         'imbalanced-learn==0.8.1',
         'scikit-learn==1.0.1',
-        'joblib==1.1.0',
-        'tqdm>=4.59.0',
     ],
     extras_require={
         "dev": [
             "flake8",
             "autopep8",
             "ipython",
             "ipdb",
             "twine",
+            "tomli",
         ],
         "docs": [
             "sphinx>=4.2",
             "sphinx_rtd_theme>=1.0",
             "readthedocs-sphinx-search>=0.1",
             "sphinxcontrib-programoutput>=0.17",
             "docutils<0.18",
```

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/accPlot.py` & `accelerometer-7.0.0.dev1/src/accelerometer/accPlot.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/accProcess.py` & `accelerometer-7.0.0.dev1/src/accelerometer/accProcess.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/accWriteCmds.py` & `accelerometer-7.0.0.dev1/src/accelerometer/accWriteCmds.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/circadian.py` & `accelerometer-7.0.0.dev1/src/accelerometer/circadian.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/classification.py` & `accelerometer-7.0.0.dev1/src/accelerometer/classification.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/device.py` & `accelerometer-7.0.0.dev1/src/accelerometer/device.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/AccStats.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/AccStats.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/AccStats.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/AccStats.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/AccelerometerParser.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/AccelerometerParser.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/AccelerometerParser.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/AccelerometerParser.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/ActigraphReader.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/ActigraphReader.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/ActigraphReader.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/ActigraphReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/AxivityReader.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/AxivityReader.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/AxivityReader.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/AxivityReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/BandpassFilter.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/BandpassFilter.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/BandpassFilter.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/BandpassFilter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/CsvReader.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/CsvReader.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/CsvReader.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/CsvReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/DeviceReader.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/DeviceReader.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/DeviceReader.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/DeviceReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/EpochWriter.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/EpochWriter.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/EpochWriter.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/EpochWriter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/Features.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/Features.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/Features.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/Features.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/Filter.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/Filter.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/Filter.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/Filter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/GENEActivReader.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/GENEActivReader.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/GENEActivReader.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/GENEActivReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/JTransforms-3.1-with-dependencies.jar` & `accelerometer-7.0.0.dev1/src/accelerometer/java/JTransforms-3.1-with-dependencies.jar`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/LowpassFilter.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/LowpassFilter.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/LowpassFilter.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/LowpassFilter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/NpyWriter.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/NpyWriter.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/NpyWriter.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/NpyWriter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/Resample.class` & `accelerometer-7.0.0.dev1/src/accelerometer/java/Resample.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/java/Resample.java` & `accelerometer-7.0.0.dev1/src/accelerometer/java/Resample.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/models.py` & `accelerometer-7.0.0.dev1/src/accelerometer/models.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/summarisation.py` & `accelerometer-7.0.0.dev1/src/accelerometer/summarisation.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer/utils.py` & `accelerometer-7.0.0.dev1/src/accelerometer/utils.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer.egg-info/PKG-INFO` & `accelerometer-7.0.0.dev1/src/accelerometer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelerometer
-Version: 7.0.0.dev0
+Version: 7.0.0.dev1
 Summary: A package to extract meaningful health information from large accelerometer datasets e.g. how much time individuals spend in sleep, sedentary behaviour, walking and moderate intensity physical activity
 Home-page: https://github.com/activityMonitoring/biobankAccelerometerAnalysis
 Download-URL: https://github.com/activityMonitoring/biobankAccelerometerAnalysis
 Author: Aiden Doherty, Shing Chan, Rosemary Walmsley, Hang Yuan
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE.md
 Keywords: wearables,accelerometer,health data science,human activity recognition
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.7
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.md
 
 ![Accelerometer data processing overview](docs/source/accelerometerLogo.png)
```

### Comparing `accelerometer-7.0.0.dev0/src/accelerometer.egg-info/SOURCES.txt` & `accelerometer-7.0.0.dev1/src/accelerometer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev0/versioneer.py` & `accelerometer-7.0.0.dev1/versioneer.py`

 * *Files identical despite different names*

