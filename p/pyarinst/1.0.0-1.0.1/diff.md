# Comparing `tmp/pyarinst-1.0.0.tar.gz` & `tmp/pyarinst-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarinst-1.0.0.tar", last modified: Fri Jun 17 10:25:55 2022, max compression
+gzip compressed data, was "pyarinst-1.0.1.tar", last modified: Tue May  9 15:54:34 2023, max compression
```

## Comparing `pyarinst-1.0.0.tar` & `pyarinst-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 10:25:55.571932 pyarinst-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-06-17 10:25:42.000000 pyarinst-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-06-17 10:25:55.571932 pyarinst-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-17 10:25:42.000000 pyarinst-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 10:25:55.567932 pyarinst-1.0.0/pyarinst/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-17 10:25:42.000000 pyarinst-1.0.0/pyarinst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4157 2022-06-17 10:25:42.000000 pyarinst-1.0.0/pyarinst/pyarinst.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 10:25:55.571932 pyarinst-1.0.0/pyarinst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-06-17 10:25:54.000000 pyarinst-1.0.0/pyarinst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-06-17 10:25:55.000000 pyarinst-1.0.0/pyarinst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 10:25:55.000000 pyarinst-1.0.0/pyarinst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-17 10:25:55.000000 pyarinst-1.0.0/pyarinst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-17 10:25:55.000000 pyarinst-1.0.0/pyarinst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-17 10:25:55.571932 pyarinst-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-06-17 10:25:42.000000 pyarinst-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:54:34.722829 pyarinst-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 15:54:19.000000 pyarinst-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-09 15:54:34.722829 pyarinst-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 15:54:19.000000 pyarinst-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:54:34.722829 pyarinst-1.0.1/pyarinst/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 15:54:19.000000 pyarinst-1.0.1/pyarinst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-09 15:54:19.000000 pyarinst-1.0.1/pyarinst/pyarinst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:54:34.722829 pyarinst-1.0.1/pyarinst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-09 15:54:34.000000 pyarinst-1.0.1/pyarinst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-09 15:54:34.000000 pyarinst-1.0.1/pyarinst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:54:34.000000 pyarinst-1.0.1/pyarinst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 15:54:34.000000 pyarinst-1.0.1/pyarinst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 15:54:34.000000 pyarinst-1.0.1/pyarinst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 15:54:34.722829 pyarinst-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-09 15:54:19.000000 pyarinst-1.0.1/setup.py
```

### Comparing `pyarinst-1.0.0/LICENSE` & `pyarinst-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarinst-1.0.0/pyarinst/pyarinst.py` & `pyarinst-1.0.1/pyarinst/pyarinst.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,29 +63,29 @@
         response = self.send_command(command, frequency)
         if len(response) == 3:
             return response[-1][0] == b"complete" and str(response[0][0], 'ascii') == command and str(response[1][0], 'ascii') == "success"
         else:
             return False
         
     def set_amplitude(self, amplitude : int) -> bool:
-        if -15 <= amplitude <= -25:
+        if -25 <= amplitude <= -15:
             command = ArinstCommand.GENERATOR_SET_AMPLITUDE
             amplitude = ((amplitude + 15) * 100) + 10000
             response = self.send_command(command, amplitude)
             return response[-1][0] == b"complete" and str(response[0][0], 'ascii') == command
         else:
             return False
 
     def __decode_data(self, response, attenuation):
         amplitudes = []
         for i in range(0, len(response), 2):
             first = int.from_bytes(response[i:i + 1], byteorder='little')
             second = int.from_bytes(response[i + 2:i + 3], byteorder='little')
             val = first << 8 | second
-            data = val & 0b000011111111111
+            data = val & 0b0000011111111111
             amplitudes.append((800.0 - data)/10.0 - attenuation)
         return amplitudes
 
     def get_scan_range(self, start = 1500000000, stop = 1700000000, step = 1000000, attenuation = 0, tracking = False):
         if -30 <= attenuation <= 0:
             command = None
             if tracking:
@@ -93,8 +93,8 @@
             else:
                 command = ArinstCommand.SCAN_RANGE
             attenuation = (attenuation * 100) + 10000
             response = self.send_command(command, start, stop, step, 200, 20, 10700000, attenuation)
             if len(response) == 3:
                 if response[-1][0] == b"complete" and str(response[0][0], 'ascii') == command:
                     return self.__decode_data(response[1][0][0:-2], attenuation)
-        return None
+        return None
```

