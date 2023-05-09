# Comparing `tmp/mmcb-avt-0.0.67.tar.gz` & `tmp/mmcb-avt-0.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.67.tar", last modified: Tue Mar 21 22:27:10 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.75.tar", last modified: Tue May  9 14:12:18 2023, max compression
```

## Comparing `mmcb-avt-0.0.67.tar` & `mmcb-avt-0.0.75.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-03-21 22:27:10.968818 mmcb-avt-0.0.67/
--rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.67/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     8108 2023-03-21 22:27:10.968098 mmcb-avt-0.0.67/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     6885 2023-03-06 09:10:49.000000 mmcb-avt-0.0.67/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2022-05-30 11:29:45.000000 mmcb-avt-0.0.67/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2023-03-21 22:27:10.968994 mmcb-avt-0.0.67/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     2556 2023-03-21 22:26:57.000000 mmcb-avt-0.0.67/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-03-21 22:27:10.934900 mmcb-avt-0.0.67/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-03-21 22:27:10.962632 mmcb-avt-0.0.67/src/mmcb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.67/src/mmcb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)    93094 2023-03-08 11:04:09.000000 mmcb-avt-0.0.67/src/mmcb/common.py
--rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.67/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.67/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.67/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt        (501) staff       (20)    30913 2023-02-01 16:04:01.000000 mmcb-avt-0.0.67/src/mmcb/detect.py
--rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.67/src/mmcb/iv.py
--rw-r--r--   0 avt        (501) staff       (20)    21489 2023-03-06 09:13:03.000000 mmcb-avt-0.0.67/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.67/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.67/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.67/src/mmcb/peltier.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.67/src/mmcb/psuset.py
--rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.67/src/mmcb/psustat.py
--rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.67/src/mmcb/sense.py
--rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.67/src/mmcb/sensors.py
--rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.67/src/mmcb/sensors_mod.py
--rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.67/src/mmcb/sequence.py
--rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.67/src/mmcb/ult80.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-03-21 22:27:10.967085 mmcb-avt-0.0.67/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     8108 2023-03-21 22:27:10.000000 mmcb-avt-0.0.67/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      630 2023-03-21 22:27:10.000000 mmcb-avt-0.0.67/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2023-03-21 22:27:10.000000 mmcb-avt-0.0.67/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      310 2023-03-21 22:27:10.000000 mmcb-avt-0.0.67/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      226 2023-03-21 22:27:10.000000 mmcb-avt-0.0.67/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        5 2023-03-21 22:27:10.000000 mmcb-avt-0.0.67/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-09 14:12:18.099981 mmcb-avt-0.0.75/
+-rw-r--r--   0 avt       (1000) avt       (1000)    13827 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/LICENSE
+-rw-r--r--   0 avt       (1000) avt       (1000)     8108 2023-05-09 14:12:18.099981 mmcb-avt-0.0.75/PKG-INFO
+-rw-r--r--   0 avt       (1000) avt       (1000)     6885 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/README.md
+-rw-r--r--   0 avt       (1000) avt       (1000)      104 2023-01-25 09:49:54.000000 mmcb-avt-0.0.75/pyproject.toml
+-rw-r--r--   0 avt       (1000) avt       (1000)       38 2023-05-09 14:12:18.099981 mmcb-avt-0.0.75/setup.cfg
+-rw-r--r--   0 avt       (1000) avt       (1000)     2556 2023-05-09 14:11:36.000000 mmcb-avt-0.0.75/setup.py
+drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-09 14:12:18.079981 mmcb-avt-0.0.75/src/
+drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-09 14:12:18.095981 mmcb-avt-0.0.75/src/mmcb/
+-rw-r--r--   0 avt       (1000) avt       (1000)        0 2023-01-25 09:49:54.000000 mmcb-avt-0.0.75/src/mmcb/__init__.py
+-rw-r--r--   0 avt       (1000) avt       (1000)    93094 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/common.py
+-rw-r--r--   0 avt       (1000) avt       (1000)    32486 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    14416 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)     9078 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    33674 2023-05-09 14:00:27.000000 mmcb-avt-0.0.75/src/mmcb/detect.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)   112129 2023-01-25 09:49:54.000000 mmcb-avt-0.0.75/src/mmcb/iv.py
+-rw-r--r--   0 avt       (1000) avt       (1000)    23401 2023-05-09 14:09:42.000000 mmcb-avt-0.0.75/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    12231 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)     7040 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)     7889 2023-01-25 09:49:54.000000 mmcb-avt-0.0.75/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    33621 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    21883 2023-01-25 09:49:54.000000 mmcb-avt-0.0.75/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    13517 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/sense.py
+-rw-r--r--   0 avt       (1000) avt       (1000)    40226 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/sensors.py
+-rw-r--r--   0 avt       (1000) avt       (1000)    17705 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    17659 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/ult80.py
+drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-09 14:12:18.099981 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt       (1000) avt       (1000)     8108 2023-05-09 14:12:17.000000 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt       (1000) avt       (1000)      606 2023-05-09 14:12:18.000000 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt       (1000) avt       (1000)        1 2023-05-09 14:12:17.000000 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt       (1000) avt       (1000)      310 2023-05-09 14:12:18.000000 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt       (1000) avt       (1000)      226 2023-05-09 14:12:18.000000 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt       (1000) avt       (1000)        5 2023-05-09 14:12:18.000000 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/top_level.txt
```

### Comparing `mmcb-avt-0.0.67/LICENSE` & `mmcb-avt-0.0.75/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/PKG-INFO` & `mmcb-avt-0.0.75/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.67
+Version: 0.0.75
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.67/README.md` & `mmcb-avt-0.0.75/README.md`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/setup.py` & `mmcb-avt-0.0.75/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.67",
+    version="0.0.75",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mmcb-avt-0.0.67/src/mmcb/common.py` & `mmcb-avt-0.0.75/src/mmcb/common.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.75/src/mmcb/configure_environment.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.75/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb/dat2root.py` & `mmcb-avt-0.0.75/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb/detect.py` & `mmcb-avt-0.0.75/src/mmcb/detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -746,14 +746,94 @@
                     pass
 
         ser.close()
 
     return retval
 
 
+def find_dmm_6500(port, config):
+    """
+    check if a Keithley DMM6500 is present on the given serial port
+
+    *IDN? returns:
+    KEITHLEY INSTRUMENTS,MODEL DMM6500,04592428,1.7.12b
+
+    --------------------------------------------------------------------------
+    args
+        port : string
+            port name
+        config : dict
+            serial port configuration
+    --------------------------------------------------------------------------
+    returns
+        retval : tuple
+            (category : string,
+             settings : dict,
+             (port : string,
+              manufacturer : string,
+              model : string,
+              serial_number : string,
+              detected : bool,
+              channels : list,
+              release_delay : float))
+    --------------------------------------------------------------------------
+    """
+    retval = (None, None, (port, None, None, None, None, None, None))
+    ser = serial.Serial()
+    ser.apply_settings(config)
+    ser.port = port
+
+    # initialise and open serial port
+    try:
+        ser.open()
+    except (OSError, serial.SerialException):
+        sys.exit(f'could not open port {port}, exiting.')
+    else:
+        ser.reset_input_buffer()
+        ser.reset_output_buffer()
+        ser.write(lexicon.instrument('dmm6500', 'identify'))
+
+        # attempt to read back response
+        try:
+            response = ser.readline().lower()
+        except serial.SerialException:
+            print(f'cannot access serial port {port}')
+        else:
+            if b'keithley' in response:
+                try:
+                    release_delay = 0.01
+                    parts = response.decode('utf-8').split(',')
+                    manufacturer = parts[0]
+                    # ['KEITHLEY INSTRUMENTS', 'MODEL DMM6500', '04592428', '1.7.12b']
+                    model = parts[1].split()[-1]
+                    serial_number = parts[2]
+                    detected = True
+                    channels = ['']
+                    settings = ser.get_settings()
+                    retval = (
+                        'hvpsu',
+                        settings,
+                        (
+                            port,
+                            manufacturer,
+                            model,
+                            serial_number,
+                            detected,
+                            channels,
+                            release_delay,
+                        ),
+                    )
+                except IndexError:
+                    pass
+
+        ser.close()
+
+    return retval
+
+
 def detect_device_on_port(port, tests, configs):
     """
     try all tests on the given port in a bid to identify which category of
     device is present
 
     --------------------------------------------------------------------------
     args
@@ -844,14 +924,15 @@
 
     tests = collections.OrderedDict(
         {
             'lvpsu': find_lvpsu,
             'lvpsu_hmp4040': find_lvpsu_hmp4040,
             'hvpsu': find_hvpsu,
             'hvpsu_2614b': find_hvpsu_2614b,
+            'dmm_6500': find_dmm_6500,
             'controller': find_controller,
             'controller_smc': find_controller_smc,
         }
     )
 
     # define serial port connection settings for each device
     # see https://pyserial.readthedocs.io/en/latest/pyserial_api.html
@@ -871,14 +952,19 @@
             'rtscts': False,
         },
         'hvpsu_2614b': {
             'baudrate': 57600,
             'xonxoff': False,
             'rtscts': False,
         },
+        'dmm_6500': {
+            'baudrate': 57600,
+            'xonxoff': False,
+            'rtscts': True,
+        },
         'controller': {
             'baudrate': 19200,
             'xonxoff': False,
             'rtscts': False,
         },
         'controller_smc': {
             'baudrate': 57600,
```

### Comparing `mmcb-avt-0.0.67/src/mmcb/iv.py` & `mmcb-avt-0.0.75/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb/lexicon.py` & `mmcb-avt-0.0.75/src/mmcb/lexicon.py`

 * *Files 3% similar despite different names*

```diff
@@ -467,18 +467,73 @@
         'set current limit': f'INST OUT{channel}{terminate}CURR {argument1}',
         # argument1: float, amps
         'set current step': f'INST OUT{channel}{terminate}CURR:STEP {argument1}',
         'read current step': f'INST OUT{channel}{terminate}CURR:STEP?',
         'current step down': f'INST OUT{channel}{terminate}CURR DOWN',
         'current step up': f'INST OUT{channel}{terminate}CURR UP'}
 
-    instructions = {'2410': keithley_2410, '2614b': keithley_2614b,
-                    'shq': iseg_shq,
-                    'e3647a': agilent_e3647a, 'e3634a': agilent_e3634a,
-                    'hmp4040': hameg_hmp4040}
+    instructions = {
+        '2410': keithley_2410, '2614b': keithley_2614b,
+        'shq': iseg_shq,
+        'e3647a': agilent_e3647a, 'e3634a': agilent_e3634a,
+        'hmp4040': hameg_hmp4040
+    }
+
+    # sanity checks
+    first = instructions.get(model)
+    assert first is not None, 'unrecognised model name'
+    second = first.get(command)
+    assert second is not None, 'unrecognised command'
+    cmd_string = instructions[model][command]
+    assert 'None' not in cmd_string, 'missing argument to function'
+
+    return bytes(cmd_string + terminate, 'utf-8')
+
+
+##############################################################################
+# general instrumentation
+##############################################################################
+
+@functools.lru_cache(maxsize=64)
+def instrument(model, command, argument1=None, argument2=None):
+    """
+    generate the requested RS232 command sequence appropriate for the
+    power supply specified
+
+    Manufacturers' implementations of Standard Commands for Programmable
+    Instruments (SCPI) all seem to have their own quirks, which is why there
+    is no generic SCPI command sequence, and each power supply is has its own
+    dictionary.
+
+    --------------------------------------------------------------------------
+    args
+        model : string
+            instrument model
+        command : string
+            name of the command to be fetched
+        argument1 : numeric/string
+            a parameter to substitute into the command string
+        argument2 : numeric/string
+            a parameter to substitute into the command string
+    --------------------------------------------------------------------------
+    returns : string
+        a valid command that can be sent to the psu over RS232
+    --------------------------------------------------------------------------
+    """
+    terminate = '\r\n'
+
+    ##########################################################################
+    # Language: Standard Commands for Programmable Instruments (SCPI)
+    dmm6500 = {
+        'identify': '*IDN?',
+    }
+
+    instructions = {
+        'dmm6500': dmm6500,
+    }
 
     # sanity checks
     first = instructions.get(model)
     assert first is not None, 'unrecognised model name'
     second = first.get(command)
     assert second is not None, 'unrecognised command'
     cmd_string = instructions[model][command]
```

### Comparing `mmcb-avt-0.0.67/src/mmcb/liveplot.py` & `mmcb-avt-0.0.75/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb/log2dat.py` & `mmcb-avt-0.0.75/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb/peltier.py` & `mmcb-avt-0.0.75/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb/psuset.py` & `mmcb-avt-0.0.75/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb/psustat.py` & `mmcb-avt-0.0.75/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb/sense.py` & `mmcb-avt-0.0.75/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb/sensors.py` & `mmcb-avt-0.0.75/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb/sequence.py` & `mmcb-avt-0.0.75/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb/ult80.py` & `mmcb-avt-0.0.75/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.67/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.75/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.67
+Version: 0.0.75
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.67/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.75/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 src/mmcb/liveplot.py
 src/mmcb/log2dat.py
 src/mmcb/peltier.py
 src/mmcb/psuset.py
 src/mmcb/psustat.py
 src/mmcb/sense.py
 src/mmcb/sensors.py
-src/mmcb/sensors_mod.py
 src/mmcb/sequence.py
 src/mmcb/ult80.py
 src/mmcb_avt.egg-info/PKG-INFO
 src/mmcb_avt.egg-info/SOURCES.txt
 src/mmcb_avt.egg-info/dependency_links.txt
 src/mmcb_avt.egg-info/entry_points.txt
 src/mmcb_avt.egg-info/requires.txt
```

