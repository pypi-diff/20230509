# Comparing `tmp/aioWiserHeatAPI-1.3.3.tar.gz` & `tmp/aioWiserHeatAPI-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioWiserHeatAPI-1.3.3.tar", last modified: Mon Apr 24 14:57:47 2023, max compression
+gzip compressed data, was "aioWiserHeatAPI-1.3.4.tar", last modified: Tue May  9 12:34:48 2023, max compression
```

## Comparing `aioWiserHeatAPI-1.3.3.tar` & `aioWiserHeatAPI-1.3.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:47.361543 aioWiserHeatAPI-1.3.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-24 14:57:47.361543 aioWiserHeatAPI-1.3.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4460 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:47.361543 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/heating.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/heating_actuator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:47.361543 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/automations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/extra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/opentherm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/special_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/temp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/zigbee.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/hot_water.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/moments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/rest_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    24805 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/roomstat.py
--rw-r--r--   0 runner    (1001) docker     (123)    40806 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/shutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/smartplug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/smartvalve.py
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/ufh.py
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/wiserhub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:47.361543 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-24 14:57:47.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-24 14:57:47.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:57:47.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 14:57:47.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 14:57:47.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 14:57:47.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 14:57:47.361543 aioWiserHeatAPI-1.3.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:48.009354 aioWiserHeatAPI-1.3.4/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-09 12:34:48.009354 aioWiserHeatAPI-1.3.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4541 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:48.005354 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/heating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/heating_actuator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:48.009354 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/automations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/extra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/opentherm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/special_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/zigbee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/hot_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/rest_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24805 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/roomstat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40806 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/shutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/smartplug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/smartvalve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/ufh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/wiserhub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:48.005354 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-09 12:34:47.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-09 12:34:48.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 12:34:47.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-09 12:34:47.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-09 12:34:47.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 12:34:47.000000 aioWiserHeatAPI-1.3.4/aioWiserHeatAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 12:34:48.009354 aioWiserHeatAPI-1.3.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-05-09 12:34:29.000000 aioWiserHeatAPI-1.3.4/setup.py
```

### Comparing `aioWiserHeatAPI-1.3.3/LICENSE` & `aioWiserHeatAPI-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/PKG-INFO` & `aioWiserHeatAPI-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aioWiserHeatAPI
-Version: 1.3.3
+Version: 1.3.4
 Summary: An AsyncIO API for controlling the Drayton Wiser Heating system
 Home-page: https://github.com/msp1974/aioWiserHeatAPI
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Drayton Wiser Hub API Async v1.3.3
+# Drayton Wiser Hub API Async v1.3.4
 
 This repository contains a simple API which queries the Drayton Wiser Heating sysystem used in the UK.
 
 The API functionality provides the following functionality to control the wiser heating system for 1,2 and 3 channel heat hubs
 The API also supports Smart Plugs and initial basic functionality for Shutter and Lights
 
 ## Requirements
@@ -64,14 +64,18 @@
 
 ## 6. Documentation
 
 Documentation available in [info.md](https://github.com/msp1974/wiserHeatAPIv2/blob/master/docs/info.md) in the docs directory and within comments in the code
 
 ## Changelog
 
+### v1.3.4
+
+* Current temperature now returns none for room if TRV signal lost.
+
 ### v1.3.3
 
 * Fixed issue in passive mode so that it works with 3 channel hub and different rooms on different channels
 
 ### v1.3.2
 
 * Fixed issue ot maintaining some parameters after hub update
```

### Comparing `aioWiserHeatAPI-1.3.3/README.md` & `aioWiserHeatAPI-1.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Drayton Wiser Hub API Async v1.3.3
+# Drayton Wiser Hub API Async v1.3.4
 
 This repository contains a simple API which queries the Drayton Wiser Heating sysystem used in the UK.
 
 The API functionality provides the following functionality to control the wiser heating system for 1,2 and 3 channel heat hubs
 The API also supports Smart Plugs and initial basic functionality for Shutter and Lights
 
 ## Requirements
@@ -48,14 +48,18 @@
 
 ## 6. Documentation
 
 Documentation available in [info.md](https://github.com/msp1974/wiserHeatAPIv2/blob/master/docs/info.md) in the docs directory and within comments in the code
 
 ## Changelog
 
+### v1.3.4
+
+* Current temperature now returns none for room if TRV signal lost.
+
 ### v1.3.3
 
 * Fixed issue in passive mode so that it works with 3 channel hub and different rooms on different channels
 
 ### v1.3.2
 
 * Fixed issue ot maintaining some parameters after hub update
```

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/cli.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/cli.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/const.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 WISERROOMSTAT = "RoomStat/{}"
 WISERSMARTPLUG = "SmartPlug/{}"
 WISERHEATINGACTUATOR = "HeatingActuator/{}"
 WISERUFHCONTROLLER = "UnderFloorHeating/{}"
 WISERSHUTTER = "Shutter/{}"
 WISERLIGHT = "Light/{}"
 
+
 # Enums
 class WiserUnitsEnum(enum.Enum):
     imperial = "imperial"
     metric = "metric"
 
 
 class WiserTempLimitsEnum(enum.Enum):
```

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/devices.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/devices.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/discovery.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/discovery.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/heating.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/heating.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/heating_actuator.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/heating_actuator.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/automations.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/automations.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/battery.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/battery.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/capabilities.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/capabilities.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/cloud.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/cloud.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/device.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/device.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/extra_config.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/extra_config.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/firmware.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/firmware.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/network.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/network.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/opentherm.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/opentherm.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/signal.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/signal.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/special_times.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/special_times.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/temp.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/temp.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,17 @@
     ) -> float:
         """
         Converts from wiser hub format to degrees C
         param temp: The wiser temperature to convert
         return: Float
         """
         if temp is not None:
-            if temp >= TEMP_ERROR:  # Fix high value from hub when lost sight of iTRV
-                temp = TEMP_MINIMUM
+            if abs(temp) >= TEMP_ERROR:
+                # Fix high value from hub when lost sight of iTRV
+                return None
             else:
                 temp = _WiserTemperatureFunctions._validate_temperature(
                     round(temp / 10, 1), type
                 )
 
             # Convert to imperial if imperial units set
             if units == WiserUnitsEnum.imperial:
```

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/zigbee.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/helpers/zigbee.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/hot_water.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/hot_water.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/light.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/light.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/moments.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/moments.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/rest_controller.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/rest_controller.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/room.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/room.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/roomstat.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/roomstat.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/schedule.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/schedule.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/shutter.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/shutter.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/smartplug.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/smartplug.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/smartvalve.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/smartvalve.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/system.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/system.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/ufh.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/ufh.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/wiserhub.py` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI/wiserhub.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/PKG-INFO` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aioWiserHeatAPI
-Version: 1.3.3
+Version: 1.3.4
 Summary: An AsyncIO API for controlling the Drayton Wiser Heating system
 Home-page: https://github.com/msp1974/aioWiserHeatAPI
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Drayton Wiser Hub API Async v1.3.3
+# Drayton Wiser Hub API Async v1.3.4
 
 This repository contains a simple API which queries the Drayton Wiser Heating sysystem used in the UK.
 
 The API functionality provides the following functionality to control the wiser heating system for 1,2 and 3 channel heat hubs
 The API also supports Smart Plugs and initial basic functionality for Shutter and Lights
 
 ## Requirements
@@ -64,14 +64,18 @@
 
 ## 6. Documentation
 
 Documentation available in [info.md](https://github.com/msp1974/wiserHeatAPIv2/blob/master/docs/info.md) in the docs directory and within comments in the code
 
 ## Changelog
 
+### v1.3.4
+
+* Current temperature now returns none for room if TRV signal lost.
+
 ### v1.3.3
 
 * Fixed issue in passive mode so that it works with 3 channel hub and different rooms on different channels
 
 ### v1.3.2
 
 * Fixed issue ot maintaining some parameters after hub update
```

### Comparing `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/SOURCES.txt` & `aioWiserHeatAPI-1.3.4/aioWiserHeatAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.3/setup.py` & `aioWiserHeatAPI-1.3.4/setup.py`

 * *Files identical despite different names*

