# Comparing `tmp/pymx2-0.1.4.tar.gz` & `tmp/pymx2-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymx2-0.1.4.tar", last modified: Wed May  3 08:13:45 2023, max compression
+gzip compressed data, was "pymx2-0.1.5.tar", last modified: Tue May  9 15:23:08 2023, max compression
```

## Comparing `pymx2-0.1.4.tar` & `pymx2-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-03 08:13:45.532081 pymx2-0.1.4/
--rw-r--r--   0 vpaeder    (501) staff       (20)       39 2023-04-27 13:13:03.000000 pymx2-0.1.4/.gitignore
--rw-r--r--   0 vpaeder    (501) staff       (20)     1071 2023-04-27 13:41:31.000000 pymx2-0.1.4/LICENSE
--rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-03 08:13:45.531479 pymx2-0.1.4/PKG-INFO
--rw-r--r--   0 vpaeder    (501) staff       (20)     2938 2023-04-28 18:35:35.000000 pymx2-0.1.4/README.md
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-03 08:13:45.516489 pymx2-0.1.4/docs/
--rw-r--r--   0 vpaeder    (501) staff       (20)   214194 2023-05-02 15:01:56.000000 pymx2-0.1.4/docs/mx2.enums.html
--rw-r--r--   0 vpaeder    (501) staff       (20)    60476 2023-05-02 15:02:06.000000 pymx2-0.1.4/docs/mx2.exceptions.html
--rw-r--r--   0 vpaeder    (501) staff       (20)    22217 2023-05-02 15:01:50.000000 pymx2-0.1.4/docs/mx2.html
--rw-r--r--   0 vpaeder    (501) staff       (20)    10077 2023-05-02 15:02:00.000000 pymx2-0.1.4/docs/mx2.types.html
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-03 08:13:45.520691 pymx2-0.1.4/examples/
--rw-r--r--   0 vpaeder    (501) staff       (20)      431 2023-04-24 11:33:12.000000 pymx2-0.1.4/examples/01_connect.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      978 2023-04-24 11:35:16.000000 pymx2-0.1.4/examples/02_read_write_coil.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      903 2023-04-26 16:47:32.000000 pymx2-0.1.4/examples/03_read_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      841 2023-04-27 12:28:11.000000 pymx2-0.1.4/examples/04_write_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      954 2023-04-27 11:31:32.000000 pymx2-0.1.4/examples/05_read_write_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     1766 2023-04-27 12:08:57.000000 pymx2-0.1.4/examples/06_data_types.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-03 08:13:45.523704 pymx2-0.1.4/mx2/
--rw-r--r--   0 vpaeder    (501) staff       (20)    31998 2023-05-03 07:51:28.000000 pymx2-0.1.4/mx2/__init__.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    48702 2023-04-28 12:11:12.000000 pymx2-0.1.4/mx2/enums.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     2161 2023-04-21 11:17:50.000000 pymx2-0.1.4/mx2/exceptions.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    11345 2023-05-02 14:57:19.000000 pymx2-0.1.4/mx2/types.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-03 08:13:45.526567 pymx2-0.1.4/pymx2.egg-info/
--rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-03 08:13:45.000000 pymx2-0.1.4/pymx2.egg-info/PKG-INFO
--rw-r--r--   0 vpaeder    (501) staff       (20)      577 2023-05-03 08:13:45.000000 pymx2-0.1.4/pymx2.egg-info/SOURCES.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)        1 2023-05-03 08:13:45.000000 pymx2-0.1.4/pymx2.egg-info/dependency_links.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)        9 2023-05-03 08:13:45.000000 pymx2-0.1.4/pymx2.egg-info/requires.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)       10 2023-05-03 08:13:45.000000 pymx2-0.1.4/pymx2.egg-info/top_level.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)       38 2023-05-03 08:13:45.532341 pymx2-0.1.4/setup.cfg
--rw-r--r--   0 vpaeder    (501) staff       (20)     1056 2023-05-03 07:51:39.000000 pymx2-0.1.4/setup.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-03 08:13:45.530263 pymx2-0.1.4/tests/
--rw-r--r--   0 vpaeder    (501) staff       (20)      144 2023-04-27 07:40:09.000000 pymx2-0.1.4/tests/__init__.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    15021 2023-05-02 15:00:57.000000 pymx2-0.1.4/tests/inverter.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     4511 2023-05-02 14:58:17.000000 pymx2-0.1.4/tests/modbus.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     3616 2023-04-21 10:52:45.000000 pymx2-0.1.4/tests/ser.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    10281 2023-04-27 12:31:47.000000 pymx2-0.1.4/tests/types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-09 15:23:08.455088 pymx2-0.1.5/
+-rw-r--r--   0 vpaeder    (501) staff       (20)       39 2023-04-27 13:13:03.000000 pymx2-0.1.5/.gitignore
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1071 2023-04-27 13:41:31.000000 pymx2-0.1.5/LICENSE
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-09 15:23:08.454703 pymx2-0.1.5/PKG-INFO
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2938 2023-04-28 18:35:35.000000 pymx2-0.1.5/README.md
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-09 15:23:08.444067 pymx2-0.1.5/docs/
+-rw-r--r--   0 vpaeder    (501) staff       (20)   214194 2023-05-02 15:01:56.000000 pymx2-0.1.5/docs/mx2.enums.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    60476 2023-05-02 15:02:06.000000 pymx2-0.1.5/docs/mx2.exceptions.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    22217 2023-05-02 15:01:50.000000 pymx2-0.1.5/docs/mx2.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    10077 2023-05-02 15:02:00.000000 pymx2-0.1.5/docs/mx2.types.html
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-09 15:23:08.447185 pymx2-0.1.5/examples/
+-rw-r--r--   0 vpaeder    (501) staff       (20)      431 2023-04-24 11:33:12.000000 pymx2-0.1.5/examples/01_connect.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      978 2023-04-24 11:35:16.000000 pymx2-0.1.5/examples/02_read_write_coil.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      903 2023-04-26 16:47:32.000000 pymx2-0.1.5/examples/03_read_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      841 2023-04-27 12:28:11.000000 pymx2-0.1.5/examples/04_write_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      954 2023-04-27 11:31:32.000000 pymx2-0.1.5/examples/05_read_write_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1766 2023-04-27 12:08:57.000000 pymx2-0.1.5/examples/06_data_types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-09 15:23:08.449444 pymx2-0.1.5/mx2/
+-rw-r--r--   0 vpaeder    (501) staff       (20)    31998 2023-05-03 07:51:28.000000 pymx2-0.1.5/mx2/__init__.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    48828 2023-05-05 06:34:19.000000 pymx2-0.1.5/mx2/enums.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2161 2023-04-21 11:17:50.000000 pymx2-0.1.5/mx2/exceptions.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    11345 2023-05-02 14:57:19.000000 pymx2-0.1.5/mx2/types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-09 15:23:08.451351 pymx2-0.1.5/pymx2.egg-info/
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-09 15:23:08.000000 pymx2-0.1.5/pymx2.egg-info/PKG-INFO
+-rw-r--r--   0 vpaeder    (501) staff       (20)      577 2023-05-09 15:23:08.000000 pymx2-0.1.5/pymx2.egg-info/SOURCES.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)        1 2023-05-09 15:23:08.000000 pymx2-0.1.5/pymx2.egg-info/dependency_links.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)        9 2023-05-09 15:23:08.000000 pymx2-0.1.5/pymx2.egg-info/requires.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)       10 2023-05-09 15:23:08.000000 pymx2-0.1.5/pymx2.egg-info/top_level.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)       38 2023-05-09 15:23:08.455180 pymx2-0.1.5/setup.cfg
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1056 2023-05-09 15:22:40.000000 pymx2-0.1.5/setup.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-09 15:23:08.454121 pymx2-0.1.5/tests/
+-rw-r--r--   0 vpaeder    (501) staff       (20)      144 2023-04-27 07:40:09.000000 pymx2-0.1.5/tests/__init__.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    15021 2023-05-02 15:00:57.000000 pymx2-0.1.5/tests/inverter.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     4511 2023-05-02 14:58:17.000000 pymx2-0.1.5/tests/modbus.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3616 2023-04-21 10:52:45.000000 pymx2-0.1.5/tests/ser.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    10281 2023-04-27 12:31:47.000000 pymx2-0.1.5/tests/types.py
```

### Comparing `pymx2-0.1.4/LICENSE` & `pymx2-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/PKG-INFO` & `pymx2-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymx2
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python driver to communicate with an Omron MX2 inverter through Modbus
 Home-page: https://github.com/vpaeder/pymx2
 Author: Vincent Paeder
 Author-email: python@paeder.fi
 Project-URL: Bug Tracker, https://github.com/vpaeder/pymx2/issues
 Keywords: omron,mx2,inverter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymx2-0.1.4/README.md` & `pymx2-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/docs/mx2.enums.html` & `pymx2-0.1.5/docs/mx2.enums.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/docs/mx2.exceptions.html` & `pymx2-0.1.5/docs/mx2.exceptions.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/docs/mx2.html` & `pymx2-0.1.5/docs/mx2.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/docs/mx2.types.html` & `pymx2-0.1.5/docs/mx2.types.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/examples/02_read_write_coil.py` & `pymx2-0.1.5/examples/02_read_write_coil.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/examples/03_read_registers.py` & `pymx2-0.1.5/examples/03_read_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/examples/04_write_registers.py` & `pymx2-0.1.5/examples/04_write_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/examples/05_read_write_registers.py` & `pymx2-0.1.5/examples/05_read_write_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/examples/06_data_types.py` & `pymx2-0.1.5/examples/06_data_types.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/mx2/__init__.py` & `pymx2-0.1.5/mx2/__init__.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/mx2/enums.py` & `pymx2-0.1.5/mx2/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1079,23 +1079,25 @@
     H005 = 0x1506
     StabilizationParameter = 0x1507
     H006 = 0x1507
     MotorParameterR1 = 0x1516
     H020 = 0x1516
     MotorParameterR2 = 0x1518
     H021 = 0x1518
+    MotorParameterL = 0x151A
     H022 = 0x151A
     MotorParameterIo = 0x151C
     H023 = 0x151C
     MotorParameterJ = (0x151D, 2)
     H024 = (0x151D, 2)
     AutoTuningParameterR1 = 0x1525
     H030 = 0x1525
     AutoTuningParameterR2 = 0x1527
     H031 = 0x1527
+    AutoTuningParameterL = 0x1529
     H032 = 0x1529
     AutoTuningParameterIo = 0x152B
     H033 = 0x152B
     AutoTuningParameterJ = (0x152C, 2)
     H034 = (0x152C, 2)
     SlipCompensationPGain = 0x153D
     H050 = 0x153D
@@ -1562,23 +1564,25 @@
     H204 = 0x2504
     SpeedResponse = 0x2506
     H205 = 0x2506
     MotorParameterR1 = 0x2516
     H220 = 0x2516
     MotorParameterR2 = 0x2518
     H221 = 0x2518
+    MotorParameterL = 0x251A
     H222 = 0x251A
     MotorParameterIo = 0x251C
     H223 = 0x251C
     MotorParameterJ = (0x251D, 2)
     H224 = (0x251D, 2)
     AutoTuningParameterR1 = 0x2525
     H230 = 0x2525
     AutoTuningParameterR2 = 0x2527
     H231 = 0x2527
+    AutoTuningParameterL = 0x2529
     H232 = 0x2529
     AutoTuningParameterIo = 0x252B
     H233 = 0x252B
     AutoTuningParameterJ = (0x252C, 2)
     H234 = (0x252C, 2)
```

### Comparing `pymx2-0.1.4/mx2/exceptions.py` & `pymx2-0.1.5/mx2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/mx2/types.py` & `pymx2-0.1.5/mx2/types.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/pymx2.egg-info/PKG-INFO` & `pymx2-0.1.5/pymx2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymx2
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python driver to communicate with an Omron MX2 inverter through Modbus
 Home-page: https://github.com/vpaeder/pymx2
 Author: Vincent Paeder
 Author-email: python@paeder.fi
 Project-URL: Bug Tracker, https://github.com/vpaeder/pymx2/issues
 Keywords: omron,mx2,inverter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymx2-0.1.4/pymx2.egg-info/SOURCES.txt` & `pymx2-0.1.5/pymx2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/setup.py` & `pymx2-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymx2",
-    version="0.1.4",
+    version="0.1.5",
     author="Vincent Paeder",
     author_email="python@paeder.fi",
     description="A Python driver to communicate with an Omron MX2 inverter through Modbus",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['omron', 'mx2', 'inverter'],
     url="https://github.com/vpaeder/pymx2",
```

### Comparing `pymx2-0.1.4/tests/inverter.py` & `pymx2-0.1.5/tests/inverter.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/tests/modbus.py` & `pymx2-0.1.5/tests/modbus.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/tests/ser.py` & `pymx2-0.1.5/tests/ser.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.4/tests/types.py` & `pymx2-0.1.5/tests/types.py`

 * *Files identical despite different names*

