# Comparing `tmp/sigmadsp-3.0.3.tar.gz` & `tmp/sigmadsp-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmadsp-3.0.3.tar", max compression
+gzip compressed data, was "sigmadsp-3.0.4.tar", max compression
```

## Comparing `sigmadsp-3.0.3.tar` & `sigmadsp-3.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    35149 2023-05-01 21:18:22.947966 sigmadsp-3.0.3/LICENSE
--rw-r--r--   0        0        0     3755 2023-05-01 21:18:22.947966 sigmadsp-3.0.3/README.md
--rw-r--r--   0        0        0     1198 2023-05-01 21:18:43.448146 sigmadsp-3.0.3/pyproject.toml
--rw-r--r--   0        0        0       99 2023-05-01 21:18:43.452146 sigmadsp-3.0.3/sigmadsp/__init__.py
--rw-r--r--   0        0        0    14651 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/backend.py
--rw-r--r--   0        0        0       92 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/dsp/__init__.py
--rw-r--r--   0        0        0     3108 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/dsp/adau14xx.py
--rw-r--r--   0        0        0     3006 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/dsp/adau1x01.py
--rw-r--r--   0        0        0     9870 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/dsp/common.py
--rw-r--r--   0        0        0     3297 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/dsp/factory.py
--rw-r--r--   0        0        0     5268 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/frontend.py
--rw-r--r--   0        0        0       53 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/generated/__init__.py
--rw-r--r--   0        0        0      223 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/generated/backend_service/__init__.py
--rw-r--r--   0        0        0     4802 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/generated/backend_service/control_pb2.py
--rw-r--r--   0        0        0     5651 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/generated/backend_service/control_pb2.pyi
--rw-r--r--   0        0        0     4033 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/generated/backend_service/control_pb2_grpc.py
--rw-r--r--   0        0        0       86 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/helper/__init__.py
--rw-r--r--   0        0        0     7388 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/helper/conversion.py
--rw-r--r--   0        0        0     9510 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/helper/parser.py
--rw-r--r--   0        0        0     2262 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/helper/settings.py
--rw-r--r--   0        0        0       78 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/protocols/__init__.py
--rw-r--r--   0        0        0     2981 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/protocols/common.py
--rw-r--r--   0        0        0     1855 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/protocols/i2c.py
--rw-r--r--   0        0        0     4404 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/protocols/spi.py
--rw-r--r--   0        0        0       64 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/sigmastudio/__init__.py
--rw-r--r--   0        0        0     1722 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/sigmastudio/adau14xx.py
--rw-r--r--   0        0        0     1505 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/sigmastudio/adau1x01.py
--rw-r--r--   0        0        0      695 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/sigmastudio/common.py
--rw-r--r--   0        0        0    11449 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/sigmastudio/header.py
--rw-r--r--   0        0        0     8600 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/sigmastudio/server.py
--rw-r--r--   0        0        0     4827 1970-01-01 00:00:00.000000 sigmadsp-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/LICENSE
+-rw-r--r--   0        0        0     9855 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/README.md
+-rw-r--r--   0        0        0     1198 2023-05-09 20:57:11.403565 sigmadsp-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0       99 2023-05-09 20:57:11.403565 sigmadsp-3.0.4/sigmadsp/__init__.py
+-rw-r--r--   0        0        0    14651 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/backend.py
+-rw-r--r--   0        0        0       92 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/dsp/__init__.py
+-rw-r--r--   0        0        0     3108 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/dsp/adau14xx.py
+-rw-r--r--   0        0        0     3006 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/dsp/adau1x01.py
+-rw-r--r--   0        0        0     9870 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/dsp/common.py
+-rw-r--r--   0        0        0     3213 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/dsp/factory.py
+-rw-r--r--   0        0        0     5268 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/frontend.py
+-rw-r--r--   0        0        0       53 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/generated/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/generated/backend_service/__init__.py
+-rw-r--r--   0        0        0     4802 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/generated/backend_service/control_pb2.py
+-rw-r--r--   0        0        0     5651 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/generated/backend_service/control_pb2.pyi
+-rw-r--r--   0        0        0     4033 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/generated/backend_service/control_pb2_grpc.py
+-rw-r--r--   0        0        0       86 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/helper/__init__.py
+-rw-r--r--   0        0        0     7388 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/helper/conversion.py
+-rw-r--r--   0        0        0     9510 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/helper/parser.py
+-rw-r--r--   0        0        0     2262 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/helper/settings.py
+-rw-r--r--   0        0        0       78 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/protocols/__init__.py
+-rw-r--r--   0        0        0     2981 2023-05-09 20:56:56.815228 sigmadsp-3.0.4/sigmadsp/protocols/common.py
+-rw-r--r--   0        0        0     1855 2023-05-09 20:56:56.819228 sigmadsp-3.0.4/sigmadsp/protocols/i2c.py
+-rw-r--r--   0        0        0     4404 2023-05-09 20:56:56.819228 sigmadsp-3.0.4/sigmadsp/protocols/spi.py
+-rw-r--r--   0        0        0       64 2023-05-09 20:56:56.819228 sigmadsp-3.0.4/sigmadsp/sigmastudio/__init__.py
+-rw-r--r--   0        0        0     1722 2023-05-09 20:56:56.819228 sigmadsp-3.0.4/sigmadsp/sigmastudio/adau14xx.py
+-rw-r--r--   0        0        0     1505 2023-05-09 20:56:56.819228 sigmadsp-3.0.4/sigmadsp/sigmastudio/adau1x01.py
+-rw-r--r--   0        0        0      695 2023-05-09 20:56:56.819228 sigmadsp-3.0.4/sigmadsp/sigmastudio/common.py
+-rw-r--r--   0        0        0    11449 2023-05-09 20:56:56.819228 sigmadsp-3.0.4/sigmadsp/sigmastudio/header.py
+-rw-r--r--   0        0        0     8600 2023-05-09 20:56:56.819228 sigmadsp-3.0.4/sigmadsp/sigmastudio/server.py
+-rw-r--r--   0        0        0    10927 1970-01-01 00:00:00.000000 sigmadsp-3.0.4/PKG-INFO
```

### Comparing `sigmadsp-3.0.3/LICENSE` & `sigmadsp-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/pyproject.toml` & `sigmadsp-3.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sigmadsp"
 license = "GPL-3.0-or-later"
-version = "3.0.3"
+version = "3.0.4"
 description = "A package for controlling Analog Devices Sigma DSP chipsets."
 readme = "README.md"
 authors = ["Adrian Figueroa <elagil@takanome.de>"]
 repository = "https://github.com/elagil/sigmadsp"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `sigmadsp-3.0.3/sigmadsp/backend.py` & `sigmadsp-3.0.4/sigmadsp/backend.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/dsp/adau14xx.py` & `sigmadsp-3.0.4/sigmadsp/dsp/adau14xx.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/dsp/adau1x01.py` & `sigmadsp-3.0.4/sigmadsp/dsp/adau1x01.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from sigmadsp.helper.conversion import int16_to_bytes
 from sigmadsp.sigmastudio.adau1x01 import Adau1x01HeaderGenerator
 
 # A logger for this module
 logger = logging.getLogger(__name__)
 
 
-class Adau1x01(Dsp):
+class Adau1x0x(Dsp):
     """A class for controlling functionality of Analog Devices Sigma DSPs, especially ADAU1x01 series parts."""
 
     # Addresses and sizes of important registers
     CONTROL_REGISTER = 0x081C
     CONTROL_REGISTER_LENGTH = 2
 
     # Safeload registers (address, data)
@@ -64,25 +64,25 @@
         # Number of words with length FIXPOINT_REGISTER_LENGTH in data.
         word_count = math.ceil(len(data) / self.FIXPOINT_REGISTER_LENGTH)
 
         assert address >= 0
 
         # load up the address and data in safeload registers
         for sd in range(0, word_count):
-            address_register, data_register = Adau1x01.SAFELOAD_REGISTERS[sd]
+            address_register, data_register = Adau1x0x.SAFELOAD_REGISTERS[sd]
             address_bytes = int16_to_bytes(address)
-            data_buf = bytearray(Adau1x01.SAFELOAD_SD_LENGTH)
+            data_buf = bytearray(Adau1x0x.SAFELOAD_SD_LENGTH)
 
-            data_buf[1:] = data[sd * Adau1x01.FIXPOINT_REGISTER_LENGTH : (sd + 1) * Adau1x01.FIXPOINT_REGISTER_LENGTH]
+            data_buf[1:] = data[sd * Adau1x0x.FIXPOINT_REGISTER_LENGTH : (sd + 1) * Adau1x0x.FIXPOINT_REGISTER_LENGTH]
 
             self.write(address_register, address_bytes)
             self.write(data_register, data_buf)
 
-        control_bytes = self.read(Adau1x01.CONTROL_REGISTER, Adau1x01.CONTROL_REGISTER_LENGTH)
+        control_bytes = self.read(Adau1x0x.CONTROL_REGISTER, Adau1x0x.CONTROL_REGISTER_LENGTH)
         control_reg = bytes_to_int16(control_bytes)
 
         ist_mask = 1 << 5
 
         control_reg |= ist_mask
 
         # start safe load
-        self.write(Adau1x01.CONTROL_REGISTER, int16_to_bytes(control_reg))
+        self.write(Adau1x0x.CONTROL_REGISTER, int16_to_bytes(control_reg))
```

### Comparing `sigmadsp-3.0.3/sigmadsp/dsp/common.py` & `sigmadsp-3.0.4/sigmadsp/dsp/common.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/dsp/factory.py` & `sigmadsp-3.0.4/sigmadsp/dsp/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """Factory module for generating DSP objects."""
 import logging
 from typing import Dict
 from typing import Type
 from typing import Union
 
 from .adau14xx import Adau14xx
-from .adau1x01 import Adau1x01
+from .adau1x01 import Adau1x0x
 from .common import ConfigurationError
 from .common import Dsp
 from .common import InputPin
 from .common import OutputPin
 from sigmadsp.protocols.i2c import I2cProtocol
 from sigmadsp.protocols.spi import SpiProtocol
 
 logger = logging.getLogger(__name__)
 
-VALID_ADAU14XX = ["adau14xx", "adau145x", "adau146x", "adau147x"]
-VALID_ADAU1X01 = ["adau1x01", "adau1401", "adau1701"]
+ADAU_14XX = "adau14xx"
+ADAU_1X0X = "adau1x0x"
 
 
 def dsp_factory(dsp_type_name: str) -> Type[Dsp]:
     """Creates Dsp objects, based on the name of the DSP.
 
     Args:
         dsp_type_name (str): The name of the DSP.
 
     Returns:
         Type[Dsp]: The matching DSP class.
     """
-    if dsp_type_name in VALID_ADAU14XX:
+    if dsp_type_name == ADAU_14XX:
         return Adau14xx
 
-    elif dsp_type_name in VALID_ADAU1X01:
-        return Adau1x01
+    elif dsp_type_name == ADAU_1X0X:
+        return Adau1x0x
 
     else:
         raise TypeError("DSP type {dsp_type} is not known.")
 
 
 def dsp_from_config(config: Dict) -> Dsp:
     """Parse a configuration dictionary and create a new DSP from it.
```

### Comparing `sigmadsp-3.0.3/sigmadsp/frontend.py` & `sigmadsp-3.0.4/sigmadsp/frontend.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/generated/backend_service/control_pb2.py` & `sigmadsp-3.0.4/sigmadsp/generated/backend_service/control_pb2.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/generated/backend_service/control_pb2.pyi` & `sigmadsp-3.0.4/sigmadsp/generated/backend_service/control_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/generated/backend_service/control_pb2_grpc.py` & `sigmadsp-3.0.4/sigmadsp/generated/backend_service/control_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/helper/conversion.py` & `sigmadsp-3.0.4/sigmadsp/helper/conversion.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/helper/parser.py` & `sigmadsp-3.0.4/sigmadsp/helper/parser.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/helper/settings.py` & `sigmadsp-3.0.4/sigmadsp/helper/settings.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/protocols/common.py` & `sigmadsp-3.0.4/sigmadsp/protocols/common.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/protocols/i2c.py` & `sigmadsp-3.0.4/sigmadsp/protocols/i2c.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/protocols/spi.py` & `sigmadsp-3.0.4/sigmadsp/protocols/spi.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/sigmastudio/adau14xx.py` & `sigmadsp-3.0.4/sigmadsp/sigmastudio/adau14xx.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/sigmastudio/adau1x01.py` & `sigmadsp-3.0.4/sigmadsp/sigmastudio/adau1x01.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/sigmastudio/common.py` & `sigmadsp-3.0.4/sigmadsp/sigmastudio/common.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/sigmastudio/header.py` & `sigmadsp-3.0.4/sigmadsp/sigmastudio/header.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.3/sigmadsp/sigmastudio/server.py` & `sigmadsp-3.0.4/sigmadsp/sigmastudio/server.py`

 * *Files identical despite different names*

