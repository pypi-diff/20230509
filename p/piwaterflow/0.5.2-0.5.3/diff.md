# Comparing `tmp/piwaterflow-0.5.2.tar.gz` & `tmp/piwaterflow-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwaterflow-0.5.2.tar", last modified: Sun May  7 08:13:46 2023, max compression
+gzip compressed data, was "piwaterflow-0.5.3.tar", last modified: Tue May  9 06:53:27 2023, max compression
```

## Comparing `piwaterflow-0.5.2.tar` & `piwaterflow-0.5.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:46.541840 piwaterflow-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-07 08:13:46.541840 piwaterflow-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:46.537840 piwaterflow-0.5.2/piwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/piwaterflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/piwaterflow/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/piwaterflow/config_waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:46.537840 piwaterflow-0.5.2/piwaterflow/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/piwaterflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/piwaterflow/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)    21519 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/piwaterflow/waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:46.537840 piwaterflow-0.5.2/piwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-07 08:13:46.000000 piwaterflow-0.5.2/piwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-07 08:13:46.000000 piwaterflow-0.5.2/piwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 08:13:46.000000 piwaterflow-0.5.2/piwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-07 08:13:46.000000 piwaterflow-0.5.2/piwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 08:13:46.000000 piwaterflow-0.5.2/piwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 08:13:46.541840 piwaterflow-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:46.541840 piwaterflow-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/tests/test_000_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/tests/test_001_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/tests/test_002_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-07 08:13:32.000000 piwaterflow-0.5.2/tests/test_003_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:27.301129 piwaterflow-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-09 06:53:27.301129 piwaterflow-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:27.297129 piwaterflow-0.5.3/piwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/piwaterflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/piwaterflow/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/piwaterflow/config_waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:27.301129 piwaterflow-0.5.3/piwaterflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/piwaterflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/piwaterflow/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21459 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/piwaterflow/waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:27.301129 piwaterflow-0.5.3/piwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-09 06:53:27.000000 piwaterflow-0.5.3/piwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-09 06:53:27.000000 piwaterflow-0.5.3/piwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:53:27.000000 piwaterflow-0.5.3/piwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-09 06:53:27.000000 piwaterflow-0.5.3/piwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 06:53:27.000000 piwaterflow-0.5.3/piwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 06:53:27.301129 piwaterflow-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:27.301129 piwaterflow-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/tests/test_000_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/tests/test_001_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/tests/test_002_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/tests/test_003_lock.py
```

### Comparing `piwaterflow-0.5.2/PKG-INFO` & `piwaterflow-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.2
+Version: 0.5.3
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.2/README.md` & `piwaterflow-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.2/piwaterflow/config-template.yml` & `piwaterflow-0.5.3/piwaterflow/config-template.yml`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.2/piwaterflow/config_waterflow.py` & `piwaterflow-0.5.3/piwaterflow/config_waterflow.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.2/piwaterflow/tests/test_000.py` & `piwaterflow-0.5.3/piwaterflow/tests/test_000.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.2/piwaterflow/waterflow.py` & `piwaterflow-0.5.3/piwaterflow/waterflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 from datetime import datetime, timedelta
 from pathlib import Path
 import json
 
 try:
     from RPi import GPIO
 except (ModuleNotFoundError, ImportError, RuntimeError):
-    from fake_rpi.RPi import GPIO
-    from fake_rpi import toggle_print
-    toggle_print(False)
+    from fake_rpigpio.RPi import GPIO
 
 from influxdb_wrapper import influxdb_factory
 from log_mgr import Logger
 from .config_waterflow import WaterflowConfig
 
 class Waterflow():
     """ Waterflow class that manages a loop system to activate/deactivate watering valves.
```

### Comparing `piwaterflow-0.5.2/piwaterflow.egg-info/PKG-INFO` & `piwaterflow-0.5.3/piwaterflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.2
+Version: 0.5.3
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.2/setup.py` & `piwaterflow-0.5.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+""" Setup.py """
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwaterflow",
-    version="0.5.2",
+    version="0.5.3",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwaterflow",
     packages=setuptools.find_packages(),
@@ -22,12 +23,12 @@
         "Operating System :: OS Independent",
         "Topic :: Home Automation",
     ],
     install_requires=[
         'log_mgr>=0.0.2',
         'config_yml>=0.2.3',
         'RPi.GPIO>=0.7.0',
-        'fake-rpi>=0.7.1',
+        'fake-rpigpio>=0.1.1',
         'influxdb_wrapper>=0.0.3'
     ],
     python_requires='>=3.6',
 )
```

### Comparing `piwaterflow-0.5.2/tests/test_000_loop.py` & `piwaterflow-0.5.3/tests/test_000_loop.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.2/tests/test_001_forward.py` & `piwaterflow-0.5.3/tests/test_001_forward.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.2/tests/test_002_reverse.py` & `piwaterflow-0.5.3/tests/test_002_reverse.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.2/tests/test_003_lock.py` & `piwaterflow-0.5.3/tests/test_003_lock.py`

 * *Files identical despite different names*

