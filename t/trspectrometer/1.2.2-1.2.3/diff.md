# Comparing `tmp/trspectrometer-1.2.2.tar.gz` & `tmp/trspectrometer-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trspectrometer-1.2.2.tar", last modified: Mon May  2 06:21:47 2022, max compression
+gzip compressed data, was "trspectrometer-1.2.3.tar", last modified: Tue May  9 07:48:18 2023, max compression
```

## Comparing `trspectrometer-1.2.2.tar` & `trspectrometer-1.2.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/
--rw-r--r--   0 patrick   (1000) patrick   (1000)    35149 2020-12-01 04:12:53.000000 trspectrometer-1.2.2/LICENSE.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)     3460 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/PKG-INFO
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2752 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/README.rst
--rw-r--r--   0 patrick   (1000) patrick   (1000)      100 2020-12-01 04:12:53.000000 trspectrometer-1.2.2/pyproject.toml
--rw-r--r--   0 patrick   (1000) patrick   (1000)       38 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/setup.cfg
--rwxr-xr-x   0 patrick   (1000) patrick   (1000)     6442 2022-05-02 06:20:00.000000 trspectrometer-1.2.2/setup.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/trspectrometer/
--rw-r--r--   0 patrick   (1000) patrick   (1000)      251 2022-05-02 06:20:00.000000 trspectrometer-1.2.2/trspectrometer/__init__.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)      123 2021-10-19 03:01:23.000000 trspectrometer-1.2.2/trspectrometer/__main__.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1144 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/aboutpanel.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     5960 2020-12-17 00:24:58.000000 trspectrometer-1.2.2/trspectrometer/aboutpanel.ui
--rwxr-xr-x   0 patrick   (1000) patrick   (1000)     8674 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/busydialog.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     6190 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/configuration.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)    54517 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/datapanel.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)    14314 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/datapanel.ui
--rw-r--r--   0 patrick   (1000) patrick   (1000)     7559 2020-12-17 00:24:58.000000 trspectrometer-1.2.2/trspectrometer/datapanelscans.ui
--rw-r--r--   0 patrick   (1000) patrick   (1000)    29268 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/datastorage.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     4340 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/hardware.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     3356 2022-05-02 06:20:00.000000 trspectrometer-1.2.2/trspectrometer/logpanel.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     5297 2022-05-02 06:20:00.000000 trspectrometer-1.2.2/trspectrometer/logpanel.ui
--rw-r--r--   0 patrick   (1000) patrick   (1000)     9785 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/mainwindow.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     4563 2021-11-15 08:14:39.000000 trspectrometer-1.2.2/trspectrometer/mainwindow.ui
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/trspectrometer/plugins/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1635 2021-11-15 08:14:39.000000 trspectrometer-1.2.2/trspectrometer/plugins/__init__.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/trspectrometer/plugins/acquisition/
--rw-r--r--   0 patrick   (1000) patrick   (1000)    13894 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/acquisition/__init__.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     8317 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/acquisition/ta_dummy.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)    22700 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/acquisition/ta_stepped.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)    28260 2022-05-02 06:20:00.000000 trspectrometer-1.2.2/trspectrometer/plugins/acquisition/ta_swept.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/trspectrometer/plugins/aligncam/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     7590 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/aligncam/__init__.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)    13331 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/aligncam/alignmentpanel.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     6894 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/aligncam/alignmentpanel.ui
--rw-r--r--   0 patrick   (1000) patrick   (1000)    10493 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/aligncam/cv2camera.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/trspectrometer/plugins/chopper/
--rw-r--r--   0 patrick   (1000) patrick   (1000)    12663 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/chopper/__init__.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2273 2021-11-15 08:14:39.000000 trspectrometer-1.2.2/trspectrometer/plugins/chopper/dummychopper.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     3045 2021-11-15 08:14:39.000000 trspectrometer-1.2.2/trspectrometer/plugins/chopper/thorlabs_mc2000b.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/trspectrometer/plugins/delay/
--rw-r--r--   0 patrick   (1000) patrick   (1000)    17431 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/delay/__init__.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1720 2021-11-15 08:14:39.000000 trspectrometer-1.2.2/trspectrometer/plugins/delay/dummydelay.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)    12720 2021-11-15 08:14:39.000000 trspectrometer-1.2.2/trspectrometer/plugins/delay/thorlabs_apt.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/trspectrometer/plugins/detector/
--rw-r--r--   0 patrick   (1000) patrick   (1000)    18752 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/detector/__init__.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     3936 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/detector/dummydetector.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     7655 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/detector/zylafixed.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/trspectrometer/plugins/interface/
--rw-r--r--   0 patrick   (1000) patrick   (1000)    15872 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/interface/__init__.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2889 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/interface/dummyinterface.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     4666 2022-05-02 06:20:00.000000 trspectrometer-1.2.2/trspectrometer/plugins/interface/trsi.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/trspectrometer/plugins/repratemenu/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     4151 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/repratemenu/__init__.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/trspectrometer/plugins/scope/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1527 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/plugins/scope/__init__.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)    32336 2022-05-02 06:20:00.000000 trspectrometer-1.2.2/trspectrometer/plugins/scope/scopepanel.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     8835 2021-11-15 08:14:39.000000 trspectrometer-1.2.2/trspectrometer/plugins/scope/scopepanel.ui
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/trspectrometer/plugins/zylaalign/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     4101 2022-05-02 06:20:00.000000 trspectrometer-1.2.2/trspectrometer/plugins/zylaalign/__init__.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)    12444 2022-05-02 06:20:00.000000 trspectrometer-1.2.2/trspectrometer/plugins/zylaalign/zylaalignpanel.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2292 2022-05-02 06:20:00.000000 trspectrometer-1.2.2/trspectrometer/plugins/zylaalign/zylaalignpanel.ui
--rw-r--r--   0 patrick   (1000) patrick   (1000)     4945 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/qtwidgets.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     4926 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/signalstorage.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)   302324 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/trspectrometer_rc.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     7965 2021-11-15 08:14:39.000000 trspectrometer-1.2.2/trspectrometer/ufsfile.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     5783 2022-02-07 23:58:29.000000 trspectrometer-1.2.2/trspectrometer/utils.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-05-02 06:21:47.283697 trspectrometer-1.2.2/trspectrometer.egg-info/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     3460 2022-05-02 06:21:47.000000 trspectrometer-1.2.2/trspectrometer.egg-info/PKG-INFO
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2133 2022-05-02 06:21:47.000000 trspectrometer-1.2.2/trspectrometer.egg-info/SOURCES.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)        1 2022-05-02 06:21:47.000000 trspectrometer-1.2.2/trspectrometer.egg-info/dependency_links.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)       56 2022-05-02 06:21:47.000000 trspectrometer-1.2.2/trspectrometer.egg-info/entry_points.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)      160 2022-05-02 06:21:47.000000 trspectrometer-1.2.2/trspectrometer.egg-info/requires.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)       15 2022-05-02 06:21:47.000000 trspectrometer-1.2.2/trspectrometer.egg-info/top_level.txt
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-09 07:48:18.228675 trspectrometer-1.2.3/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    35149 2020-12-01 04:12:53.000000 trspectrometer-1.2.3/LICENSE.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     3406 2023-05-09 07:48:18.228675 trspectrometer-1.2.3/PKG-INFO
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     2735 2023-05-09 01:04:41.000000 trspectrometer-1.2.3/README.rst
+-rw-r--r--   0 patrick   (1000) patrick   (1000)      100 2020-12-01 04:12:53.000000 trspectrometer-1.2.3/pyproject.toml
+-rw-r--r--   0 patrick   (1000) patrick   (1000)       38 2023-05-09 07:48:18.228675 trspectrometer-1.2.3/setup.cfg
+-rwxr-xr-x   0 patrick   (1000) patrick   (1000)     6435 2023-05-09 01:04:41.000000 trspectrometer-1.2.3/setup.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-09 07:48:18.225341 trspectrometer-1.2.3/trspectrometer/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)      251 2023-05-09 01:04:41.000000 trspectrometer-1.2.3/trspectrometer/__init__.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)      123 2021-10-19 03:01:23.000000 trspectrometer-1.2.3/trspectrometer/__main__.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1123 2023-05-09 07:42:57.000000 trspectrometer-1.2.3/trspectrometer/aboutpanel.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     5968 2023-05-09 01:04:41.000000 trspectrometer-1.2.3/trspectrometer/aboutpanel.ui
+-rwxr-xr-x   0 patrick   (1000) patrick   (1000)     8674 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/busydialog.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     6190 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/configuration.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    54476 2023-05-09 07:42:41.000000 trspectrometer-1.2.3/trspectrometer/datapanel.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    14314 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/datapanel.ui
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     7559 2020-12-17 00:24:58.000000 trspectrometer-1.2.3/trspectrometer/datapanelscans.ui
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    29268 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/datastorage.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     4340 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/hardware.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     3336 2023-05-09 07:41:47.000000 trspectrometer-1.2.3/trspectrometer/logpanel.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     5297 2022-05-02 06:20:00.000000 trspectrometer-1.2.3/trspectrometer/logpanel.ui
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     9760 2023-05-09 07:44:22.000000 trspectrometer-1.2.3/trspectrometer/mainwindow.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     4563 2021-11-15 08:14:39.000000 trspectrometer-1.2.3/trspectrometer/mainwindow.ui
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-09 07:48:18.225341 trspectrometer-1.2.3/trspectrometer/plugins/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1635 2021-11-15 08:14:39.000000 trspectrometer-1.2.3/trspectrometer/plugins/__init__.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-09 07:48:18.225341 trspectrometer-1.2.3/trspectrometer/plugins/acquisition/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    13894 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/acquisition/__init__.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     8317 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/acquisition/ta_dummy.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    22700 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/acquisition/ta_stepped.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    28260 2022-05-02 06:20:00.000000 trspectrometer-1.2.3/trspectrometer/plugins/acquisition/ta_swept.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-09 07:48:18.228675 trspectrometer-1.2.3/trspectrometer/plugins/aligncam/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     7590 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/aligncam/__init__.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    13310 2023-05-09 07:44:40.000000 trspectrometer-1.2.3/trspectrometer/plugins/aligncam/alignmentpanel.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     6894 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/aligncam/alignmentpanel.ui
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    10493 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/aligncam/cv2camera.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-09 07:48:18.228675 trspectrometer-1.2.3/trspectrometer/plugins/chopper/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    12663 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/chopper/__init__.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     2273 2021-11-15 08:14:39.000000 trspectrometer-1.2.3/trspectrometer/plugins/chopper/dummychopper.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     3045 2021-11-15 08:14:39.000000 trspectrometer-1.2.3/trspectrometer/plugins/chopper/thorlabs_mc2000b.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-09 07:48:18.228675 trspectrometer-1.2.3/trspectrometer/plugins/delay/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    17431 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/delay/__init__.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1720 2021-11-15 08:14:39.000000 trspectrometer-1.2.3/trspectrometer/plugins/delay/dummydelay.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    12720 2021-11-15 08:14:39.000000 trspectrometer-1.2.3/trspectrometer/plugins/delay/thorlabs_apt.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-09 07:48:18.228675 trspectrometer-1.2.3/trspectrometer/plugins/detector/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    18752 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/detector/__init__.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     3936 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/detector/dummydetector.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     7655 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/detector/zylafixed.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-09 07:48:18.228675 trspectrometer-1.2.3/trspectrometer/plugins/interface/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    15872 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/interface/__init__.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     2889 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/interface/dummyinterface.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     4666 2022-05-02 06:20:00.000000 trspectrometer-1.2.3/trspectrometer/plugins/interface/trsi.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-09 07:48:18.228675 trspectrometer-1.2.3/trspectrometer/plugins/repratemenu/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     4151 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/repratemenu/__init__.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-09 07:48:18.228675 trspectrometer-1.2.3/trspectrometer/plugins/scope/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1527 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/plugins/scope/__init__.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    32315 2023-05-09 07:44:49.000000 trspectrometer-1.2.3/trspectrometer/plugins/scope/scopepanel.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     8835 2021-11-15 08:14:39.000000 trspectrometer-1.2.3/trspectrometer/plugins/scope/scopepanel.ui
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-09 07:48:18.228675 trspectrometer-1.2.3/trspectrometer/plugins/zylaalign/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     4101 2022-05-02 06:20:00.000000 trspectrometer-1.2.3/trspectrometer/plugins/zylaalign/__init__.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    12423 2023-05-09 07:45:52.000000 trspectrometer-1.2.3/trspectrometer/plugins/zylaalign/zylaalignpanel.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     2292 2022-05-02 06:20:00.000000 trspectrometer-1.2.3/trspectrometer/plugins/zylaalign/zylaalignpanel.ui
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     4945 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/qtwidgets.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     4926 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/signalstorage.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)   302324 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/trspectrometer_rc.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     7965 2021-11-15 08:14:39.000000 trspectrometer-1.2.3/trspectrometer/ufsfile.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     5783 2022-02-07 23:58:29.000000 trspectrometer-1.2.3/trspectrometer/utils.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-09 07:48:18.225341 trspectrometer-1.2.3/trspectrometer.egg-info/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     3406 2023-05-09 07:48:18.000000 trspectrometer-1.2.3/trspectrometer.egg-info/PKG-INFO
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     2133 2023-05-09 07:48:18.000000 trspectrometer-1.2.3/trspectrometer.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)        1 2023-05-09 07:48:18.000000 trspectrometer-1.2.3/trspectrometer.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)       55 2023-05-09 07:48:18.000000 trspectrometer-1.2.3/trspectrometer.egg-info/entry_points.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)      153 2023-05-09 07:48:18.000000 trspectrometer-1.2.3/trspectrometer.egg-info/requires.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)       15 2023-05-09 07:48:18.000000 trspectrometer-1.2.3/trspectrometer.egg-info/top_level.txt
```

### Comparing `trspectrometer-1.2.2/LICENSE.txt` & `trspectrometer-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/PKG-INFO` & `trspectrometer-1.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: trspectrometer
-Version: 1.2.2
+Version: 1.2.3
 Summary: Software for running a time-resolved spectrometer.
 Home-page: https://gitlab.com/ptapping/trspectrometer
 Author: Patrick Tapping
 Author-email: mail@patricktapping.com
-License: UNKNOWN
 Project-URL: Documentation, https://trspectrometer.readthedocs.io/
 Project-URL: Source, https://gitlab.com/ptapping/trspectrometer
 Project-URL: Tracker, https://gitlab.com/ptapping/trspectrometer/-/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 License-File: LICENSE.txt
 
 TRSpectrometer
@@ -60,25 +58,23 @@
 On Linux, a launcher icon should be installed in your menus (this feature is not yet implemented on Windows or MacOS).
 On all operating systems, the application can be launched from the command line:
 
 .. code-block:: sh
 
     trspectrometer
 
-Further details can be found in the `Getting Started <https://trspectrometer.readthedocs.io/en/latest/gettingstarted.html>`__ section of the documentation.
+Further details can be found in the `Getting Started <https://ptapping.gitlab.io/trspectrometer/gettingstarted.html>`__ section of the documentation.
 
 
 Support
 -------
 
-Documentation can be read online at `Read the Docs <https://trspectrometer.readthedocs.io/>`__.
+Documentation can be read online at `<https://ptapping.gitlab.io/trspectrometer>`__.
 
 Bug reports, feature requests and suggestions can be submitted to the `issue tracker <https://gitlab.com/ptapping/trspectrometer/-/issues>`__.
 
 
 License
 -------
 
 All original work is free and open source, licensed under the GNU Public License.
 See the `LICENSE.txt <https://gitlab.com/ptapping/trspectrometer/-/blob/main/LICENSE.txt>`__ for details.
-
-
```

### Comparing `trspectrometer-1.2.2/README.rst` & `trspectrometer-1.2.3/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -42,21 +42,21 @@
 On Linux, a launcher icon should be installed in your menus (this feature is not yet implemented on Windows or MacOS).
 On all operating systems, the application can be launched from the command line:
 
 .. code-block:: sh
 
     trspectrometer
 
-Further details can be found in the `Getting Started <https://trspectrometer.readthedocs.io/en/latest/gettingstarted.html>`__ section of the documentation.
+Further details can be found in the `Getting Started <https://ptapping.gitlab.io/trspectrometer/gettingstarted.html>`__ section of the documentation.
 
 
 Support
 -------
 
-Documentation can be read online at `Read the Docs <https://trspectrometer.readthedocs.io/>`__.
+Documentation can be read online at `<https://ptapping.gitlab.io/trspectrometer>`__.
 
 Bug reports, feature requests and suggestions can be submitted to the `issue tracker <https://gitlab.com/ptapping/trspectrometer/-/issues>`__.
 
 
 License
 -------
```

### Comparing `trspectrometer-1.2.2/setup.py` & `trspectrometer-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                     print(f"Removed directory: {dirname}")
                 except Exception as ex:
                     pass
 
 
 setuptools.setup(
     name="trspectrometer",
-    version="1.2.2",
+    version="1.2.3",
     author="Patrick Tapping",
     author_email="mail@patricktapping.com",
     description="Software for running a time-resolved spectrometer.",
     long_description=long_description,
     url="https://gitlab.com/ptapping/trspectrometer",
     project_urls={
         "Documentation": "https://trspectrometer.readthedocs.io/",
@@ -147,15 +147,15 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
     install_requires=[
-        "PySide6==6.2.1",
+        "PySide6",
         "pyqtgraph",
         "numpy",
         "scipy",
         "opencv-python-headless",
         "tomlkit",
         "appdirs",
         "zarr",
```

### Comparing `trspectrometer-1.2.2/trspectrometer/aboutpanel.py` & `trspectrometer-1.2.3/trspectrometer/aboutpanel.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from PySide6 import QtCore, QtGui, QtWidgets
 from PySide6.QtUiTools import loadUiType
 
 import trspectrometer
 
-class AboutPanel(QtWidgets.QDialog, loadUiType(__file__.split(".py")[0] + ".ui")[0]):
+class AboutPanel(*loadUiType(__file__.split(".py")[0] + ".ui")):
 
     """
     Show a dialog box with information about the application.
     """
 
     def __init__(self, parent=None):
         super().__init__(parent)
```

### Comparing `trspectrometer-1.2.2/trspectrometer/aboutpanel.ui` & `trspectrometer-1.2.3/trspectrometer/aboutpanel.ui`

 * *Files 2% similar despite different names*

#### Comparing `trspectrometer-1.2.2/trspectrometer/aboutpanel.ui` & `trspectrometer-1.2.3/trspectrometer/aboutpanel.ui`

```diff
@@ -98,15 +98,15 @@
         <widget class="QLabel" name="infoLabel">
           <property name="text">
             <string>&lt;!DOCTYPE HTML PUBLIC &quot;-//W3C//DTD HTML 4.0//EN&quot; &quot;http://www.w3.org/TR/REC-html40/strict.dtd&quot;&gt;
 &lt;html&gt;&lt;head&gt;&lt;meta name=&quot;qrichtext&quot; content=&quot;1&quot; /&gt;&lt;style type=&quot;text/css&quot;&gt;
 p, li { white-space: pre-wrap; }
 &lt;/style&gt;&lt;/head&gt;&lt;body style=&quot; font-family:'Ubuntu'; font-size:11pt; font-weight:400; font-style:normal;&quot;&gt;
 &lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Documentation at:&lt;/p&gt;
-&lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;&lt;a href=&quot;https://trspectrometer.readthedocs.io/&quot;&gt;&lt;span style=&quot; text-decoration: underline; color:#0000ff;&quot;&gt;https://trspectrometer.readthedocs.io/&lt;/span&gt;&lt;/a&gt;&lt;br /&gt;&lt;/p&gt;
+&lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;&lt;a href=&quot;https://ptapping.gitlab.io/trspectrometer/&quot;&gt;&lt;span style=&quot; text-decoration: underline; color:#0000ff;&quot;&gt;https://ptapping.gitlab.io/trspectrometer/&lt;/span&gt;&lt;/a&gt;&lt;br /&gt;&lt;/p&gt;
 &lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Get the source code or report issues at:&lt;/p&gt;
 &lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;&lt;a href=&quot;https://gitlab.com/ptapping/trspectrometer&quot;&gt;&lt;span style=&quot; text-decoration: underline; color:#0000ff;&quot;&gt;https://gitlab.com/ptapping/trspectrometer&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
           </property>
           <property name="alignment">
             <set>Qt::AlignCenter</set>
           </property>
           <property name="wordWrap">
```

### Comparing `trspectrometer-1.2.2/trspectrometer/busydialog.py` & `trspectrometer-1.2.3/trspectrometer/busydialog.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/configuration.py` & `trspectrometer-1.2.3/trspectrometer/configuration.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/datapanel.py` & `trspectrometer-1.2.3/trspectrometer/datapanel.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 # Gradient start and stop RGBA colours to use for individual scan traces
 start = [0, 64, 255, 128]
 stop  = [192, 0, 0, 128]
 # Highlight RGBA colour to use when highlighting a specific scan trace
 highlight = [192, 192, 192, 255]
 """
 
-class DataPanel(QtWidgets.QWidget, loadUiType(__file__.split(".py")[0] + ".ui")[0]):
+class DataPanel(*loadUiType(__file__.split(".py")[0] + ".ui")):
     """
     UI panel to facilitate the collection and viewing of data.
 
     :param parent: Parent of the QWidget.
     """    
     def __init__(self, parent=None):
         super().__init__(parent)
@@ -1052,15 +1052,15 @@
         step = float(index.model().data(model.index(index.row(), 2), QtCore.Qt.EditRole).split()[0])
         model.setData(model.index(index.row(), 0), f"{int(window/step)}")
 
     def updateEditorGeometry(self, editor, option, index):
         editor.setGeometry(option.rect)
 
 
-class DataPanelScansWidget(QtWidgets.QFrame, loadUiType(os.path.join(os.path.dirname(__file__), "datapanelscans.ui"))[0]):
+class DataPanelScansWidget(*loadUiType(os.path.join(os.path.dirname(__file__), "datapanelscans.ui"))):
     """
     The QWidget which will be inserted into the GraphicsLayout to display a
     list of checkboxes to disable or enable individiual scans. 
     """
 
     def __init__(self, parent=None, plotitems=[], label="Scan #{}"):
         super().__init__(parent)
```

### Comparing `trspectrometer-1.2.2/trspectrometer/datapanel.ui` & `trspectrometer-1.2.3/trspectrometer/datapanel.ui`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/datapanelscans.ui` & `trspectrometer-1.2.3/trspectrometer/datapanelscans.ui`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/datastorage.py` & `trspectrometer-1.2.3/trspectrometer/datastorage.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/hardware.py` & `trspectrometer-1.2.3/trspectrometer/hardware.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/logpanel.py` & `trspectrometer-1.2.3/trspectrometer/logpanel.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from PySide6 import QtGui, QtWidgets
 from PySide6.QtUiTools import loadUiType
 from PySide6.QtWidgets import QFileDialog, QMessageBox
 
 import configuration as config
 
-class LogPanel(QtWidgets.QFrame, loadUiType(__file__.split(".py")[0] + ".ui")[0]):
+class LogPanel(*loadUiType(__file__.split(".py")[0] + ".ui")):
 
     """
     A UI panel which attaches to the root logger to display logged messages.
 
     Note that this panel is unable to display log messages which occur prior to
     its initialisation.
     """
```

### Comparing `trspectrometer-1.2.2/trspectrometer/logpanel.ui` & `trspectrometer-1.2.3/trspectrometer/logpanel.ui`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/mainwindow.py` & `trspectrometer-1.2.3/trspectrometer/mainwindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     Global handler for exceptions.
     Not particularly smart, but stops crashes from minor recoverable errors.
     The exception details are sent to the log.
     """
     logging.error("Caught an unhandled exception:\n  " + "  ".join(traceback.format_exception(extype, value, tb)).rstrip("\n"))
 sys.excepthook = exception_handler
 
-class MainWindow(QtWidgets.QMainWindow, loadUiType(__file__.split(".py")[0] + ".ui")[0]):
+class MainWindow(*loadUiType(__file__.split(".py")[0] + ".ui")):
     """
     Main window for the various components of the spectrometer software.
     """
 
     #: Signal to trigger a status bar message.
     show_message = Signal(str)
```

### Comparing `trspectrometer-1.2.2/trspectrometer/mainwindow.ui` & `trspectrometer-1.2.3/trspectrometer/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/__init__.py` & `trspectrometer-1.2.3/trspectrometer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/acquisition/__init__.py` & `trspectrometer-1.2.3/trspectrometer/plugins/acquisition/__init__.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/acquisition/ta_dummy.py` & `trspectrometer-1.2.3/trspectrometer/plugins/acquisition/ta_dummy.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/acquisition/ta_stepped.py` & `trspectrometer-1.2.3/trspectrometer/plugins/acquisition/ta_stepped.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/acquisition/ta_swept.py` & `trspectrometer-1.2.3/trspectrometer/plugins/acquisition/ta_swept.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/aligncam/__init__.py` & `trspectrometer-1.2.3/trspectrometer/plugins/aligncam/__init__.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/aligncam/alignmentpanel.py` & `trspectrometer-1.2.3/trspectrometer/plugins/aligncam/alignmentpanel.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import cv2
 
 import pyqtgraph as pg
 import configuration as config
 import hardware as hw
 
 
-class AlignmentPanel(QtWidgets.QWidget, loadUiType(__file__.split(".py")[0] + ".ui")[0]):
+class AlignmentPanel(*loadUiType(__file__.split(".py")[0] + ".ui")):
 
     """
     UI panel to facilitate the alignment of a laser beam through a translating
     retroreflector delay stage.
 
     When the beam is properly aligned into the input of the delay stage,
     translating the retroreflector should not cause any change in the beam
```

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/aligncam/alignmentpanel.ui` & `trspectrometer-1.2.3/trspectrometer/plugins/aligncam/alignmentpanel.ui`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/aligncam/cv2camera.py` & `trspectrometer-1.2.3/trspectrometer/plugins/aligncam/cv2camera.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/chopper/__init__.py` & `trspectrometer-1.2.3/trspectrometer/plugins/chopper/__init__.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/chopper/dummychopper.py` & `trspectrometer-1.2.3/trspectrometer/plugins/chopper/dummychopper.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/chopper/thorlabs_mc2000b.py` & `trspectrometer-1.2.3/trspectrometer/plugins/chopper/thorlabs_mc2000b.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/delay/__init__.py` & `trspectrometer-1.2.3/trspectrometer/plugins/delay/__init__.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/delay/dummydelay.py` & `trspectrometer-1.2.3/trspectrometer/plugins/delay/dummydelay.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/delay/thorlabs_apt.py` & `trspectrometer-1.2.3/trspectrometer/plugins/delay/thorlabs_apt.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/detector/__init__.py` & `trspectrometer-1.2.3/trspectrometer/plugins/detector/__init__.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/detector/dummydetector.py` & `trspectrometer-1.2.3/trspectrometer/plugins/detector/dummydetector.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/detector/zylafixed.py` & `trspectrometer-1.2.3/trspectrometer/plugins/detector/zylafixed.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/interface/__init__.py` & `trspectrometer-1.2.3/trspectrometer/plugins/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/interface/dummyinterface.py` & `trspectrometer-1.2.3/trspectrometer/plugins/interface/dummyinterface.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/interface/trsi.py` & `trspectrometer-1.2.3/trspectrometer/plugins/interface/trsi.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/repratemenu/__init__.py` & `trspectrometer-1.2.3/trspectrometer/plugins/repratemenu/__init__.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/scope/__init__.py` & `trspectrometer-1.2.3/trspectrometer/plugins/scope/__init__.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/scope/scopepanel.py` & `trspectrometer-1.2.3/trspectrometer/plugins/scope/scopepanel.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 import configuration as config
 from signalstorage import signals
 import hardware as hw
 import datastorage as ds
 from utils import AcquisitionError, AcquisitionAbortedWarning, no_infs, status_message, si_unit_factor
 
 
-class ScopePanel(QtWidgets.QWidget, loadUiType(__file__.split(".py")[0] + ".ui")[0]):
+class ScopePanel(*loadUiType(__file__.split(".py")[0] + ".ui")):
 
     """
     UI panel to view realtime data from the detector device.
 
     Currently only uses the first delay, chopper, interface, and detector devices. Data can be
     viewed as raw signal from the detector, or as a change in absorbance (ΔA) signal.
```

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/scope/scopepanel.ui` & `trspectrometer-1.2.3/trspectrometer/plugins/scope/scopepanel.ui`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/zylaalign/__init__.py` & `trspectrometer-1.2.3/trspectrometer/plugins/zylaalign/__init__.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/zylaalign/zylaalignpanel.py` & `trspectrometer-1.2.3/trspectrometer/plugins/zylaalign/zylaalignpanel.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 import hardware as hw
 import configuration as config
 from utils import status_message
 from signalstorage import signals
 
 
-class ZylaAlign(QtWidgets.QWidget, loadUiType(__file__.split(".py")[0] + ".ui")[0]):
+class ZylaAlign(*loadUiType(__file__.split(".py")[0] + ".ui")):
     """
     UI panel to view the Zyla image data to assist with alignment.
 
     :param parent: Parent of the QWidget.
     """
 
     _data_received = Signal(np.ndarray)
```

### Comparing `trspectrometer-1.2.2/trspectrometer/plugins/zylaalign/zylaalignpanel.ui` & `trspectrometer-1.2.3/trspectrometer/plugins/zylaalign/zylaalignpanel.ui`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/qtwidgets.py` & `trspectrometer-1.2.3/trspectrometer/qtwidgets.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/signalstorage.py` & `trspectrometer-1.2.3/trspectrometer/signalstorage.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/trspectrometer_rc.py` & `trspectrometer-1.2.3/trspectrometer/trspectrometer_rc.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/ufsfile.py` & `trspectrometer-1.2.3/trspectrometer/ufsfile.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer/utils.py` & `trspectrometer-1.2.3/trspectrometer/utils.py`

 * *Files identical despite different names*

### Comparing `trspectrometer-1.2.2/trspectrometer.egg-info/PKG-INFO` & `trspectrometer-1.2.3/trspectrometer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: trspectrometer
-Version: 1.2.2
+Version: 1.2.3
 Summary: Software for running a time-resolved spectrometer.
 Home-page: https://gitlab.com/ptapping/trspectrometer
 Author: Patrick Tapping
 Author-email: mail@patricktapping.com
-License: UNKNOWN
 Project-URL: Documentation, https://trspectrometer.readthedocs.io/
 Project-URL: Source, https://gitlab.com/ptapping/trspectrometer
 Project-URL: Tracker, https://gitlab.com/ptapping/trspectrometer/-/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 License-File: LICENSE.txt
 
 TRSpectrometer
@@ -60,25 +58,23 @@
 On Linux, a launcher icon should be installed in your menus (this feature is not yet implemented on Windows or MacOS).
 On all operating systems, the application can be launched from the command line:
 
 .. code-block:: sh
 
     trspectrometer
 
-Further details can be found in the `Getting Started <https://trspectrometer.readthedocs.io/en/latest/gettingstarted.html>`__ section of the documentation.
+Further details can be found in the `Getting Started <https://ptapping.gitlab.io/trspectrometer/gettingstarted.html>`__ section of the documentation.
 
 
 Support
 -------
 
-Documentation can be read online at `Read the Docs <https://trspectrometer.readthedocs.io/>`__.
+Documentation can be read online at `<https://ptapping.gitlab.io/trspectrometer>`__.
 
 Bug reports, feature requests and suggestions can be submitted to the `issue tracker <https://gitlab.com/ptapping/trspectrometer/-/issues>`__.
 
 
 License
 -------
 
 All original work is free and open source, licensed under the GNU Public License.
 See the `LICENSE.txt <https://gitlab.com/ptapping/trspectrometer/-/blob/main/LICENSE.txt>`__ for details.
-
-
```

### Comparing `trspectrometer-1.2.2/trspectrometer.egg-info/SOURCES.txt` & `trspectrometer-1.2.3/trspectrometer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

