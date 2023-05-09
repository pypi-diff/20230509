# Comparing `tmp/emBRICK-0.20.tar.gz` & `tmp/emBRICK-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emBRICK-0.20.tar", last modified: Tue Apr 11 11:14:51 2023, max compression
+gzip compressed data, was "emBRICK-0.21.tar", last modified: Tue May  9 08:04:23 2023, max compression
```

## Comparing `emBRICK-0.20.tar` & `emBRICK-0.21.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 11:14:51.082891 emBRICK-0.20/
--rw-rw-rw-   0        0        0     1088 2023-02-13 10:03:34.000000 emBRICK-0.20/LICENSE
--rw-rw-rw-   0        0        0     1114 2023-04-11 11:14:51.082963 emBRICK-0.20/PKG-INFO
--rw-rw-rw-   0        0        0     2825 2023-02-13 10:03:34.000000 emBRICK-0.20/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 11:14:51.077364 emBRICK-0.20/emBRICK/
--rw-rw-rw-   0        0        0        1 2021-04-12 11:58:59.000000 emBRICK-0.20/emBRICK/__init__.py
--rw-rw-rw-   0        0        0     1332 2023-04-06 15:14:43.000000 emBRICK-0.20/emBRICK/binary_utils.py
--rw-rw-rw-   0        0        0    39747 2023-04-11 10:27:42.000000 emBRICK-0.20/emBRICK/bricks.py
--r--r--r--   0        0        0    15285 2023-02-07 16:00:09.000000 emBRICK-0.20/emBRICK/ethernet.py
--rw-rw-rw-   0        0        0    15561 2023-04-11 10:06:20.000000 emBRICK-0.20/emBRICK/modbus_rtu.py
--rw-rw-rw-   0        0        0    11572 2023-04-11 10:22:59.000000 emBRICK-0.20/emBRICK/modbus_tcp.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:14:51.081834 emBRICK-0.20/emBRICK.egg-info/
--rw-rw-rw-   0        0        0     1114 2023-04-11 11:14:51.000000 emBRICK-0.20/emBRICK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-04-11 11:14:51.000000 emBRICK-0.20/emBRICK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 11:14:51.000000 emBRICK-0.20/emBRICK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-11 11:14:51.000000 emBRICK-0.20/emBRICK.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 11:14:51.000000 emBRICK-0.20/emBRICK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-11 11:14:51.083819 emBRICK-0.20/setup.cfg
--rw-rw-rw-   0        0        0     2076 2023-04-11 08:41:03.000000 emBRICK-0.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:04:23.002815 emBRICK-0.21/
+-rw-rw-rw-   0        0        0      991 2023-05-09 08:04:23.002815 emBRICK-0.21/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-09 08:04:22.982103 emBRICK-0.21/emBRICK/
+-rw-rw-rw-   0        0        0        1 2021-04-12 11:58:59.000000 emBRICK-0.21/emBRICK/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-04-06 15:14:43.000000 emBRICK-0.21/emBRICK/binary_utils.py
+-rw-rw-rw-   0        0        0    40211 2023-05-08 13:41:45.000000 emBRICK-0.21/emBRICK/bricks.py
+-r--r--r--   0        0        0    15285 2023-02-07 16:00:09.000000 emBRICK-0.21/emBRICK/ethernet.py
+-rw-rw-rw-   0        0        0    15391 2023-05-09 07:01:13.000000 emBRICK-0.21/emBRICK/modbus_rtu.py
+-rw-rw-rw-   0        0        0    11572 2023-04-11 10:22:59.000000 emBRICK-0.21/emBRICK/modbus_tcp.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:04:23.000272 emBRICK-0.21/emBRICK.egg-info/
+-rw-rw-rw-   0        0        0      991 2023-05-09 08:04:22.000000 emBRICK-0.21/emBRICK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-05-09 08:04:22.000000 emBRICK-0.21/emBRICK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 08:04:22.000000 emBRICK-0.21/emBRICK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-09 08:04:22.000000 emBRICK-0.21/emBRICK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-09 08:04:22.000000 emBRICK-0.21/emBRICK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-09 08:04:23.004673 emBRICK-0.21/setup.cfg
+-rw-rw-rw-   0        0        0     1993 2023-05-09 08:01:25.000000 emBRICK-0.21/setup.py
```

### Comparing `emBRICK-0.20/PKG-INFO` & `emBRICK-0.21/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: emBRICK
-Version: 0.20
+Version: 0.21
 Summary: Driver to build a connection RemoteMaster <-> LWCS over Ethernet, Modbus TCP & RTU
 Home-page: https://github.com/IMACS-GmbH/emBRICK/tree/main/Protocol%20Stacks/remoteBUS/Python%20via%20TCP-IP%20or%20RSxxx
 Download-URL: https://github.com/IMACS-GmbH/emBRICK/raw/main/Protocol%20Stacks/remoteBUS/Python%20via%20TCP-IP%20or%20RSxxx/emBRICK-0.15.tar.gz
 Author: IMACS
 Author-email: serkan.sen@imacs-gmbh.de
 License: MIT
 Keywords: IMACS,EMBRICK,PYTHON,TCP/IP,Modbus,RTU,TCP
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `emBRICK-0.20/emBRICK/binary_utils.py` & `emBRICK-0.21/emBRICK/binary_utils.py`

 * *Files identical despite different names*

### Comparing `emBRICK-0.20/emBRICK/bricks.py` & `emBRICK-0.21/emBRICK/bricks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from emBRICK.modbus_rtu import bB_update
 from emBRICK.modbus_rtu import bB
 from emBRICK.modbus_rtu import connect
 import threading
 import math
 import time
 import sys
@@ -10,69 +9,73 @@
 from datetime import datetime
 import scipy.interpolate
 
 lock = threading.Lock()
 
 brick_info = ''
 lock.acquire()
+
+
 def findBricks():
     '''
     Check connected Bricks and configure the corresponding objects
     '''
-    
+
     # TODO: braucht man das global hier? 
     global brick_info
 
     bricks = {2181: CAE_G8Di8Do, 4602: CAE_B3U4I, 4603: CAE_B3U4I, 2470: CAE_G2Mi2Ao, 2471: CAE_G2Mi2Ao,
               2472: CAE_G2Mi2Ao, 2431: CAE_G4Ai4Tmp, 2432: CAE_G4Ai4Tmp, 2433: CAE_G4Ai4Tmp, 2434: CAE_G4Ai4Tmp,
               2435: CAE_G4Ai4Tmp, 2436: CAE_G4Ai4Tmp}
     '''
     bricks = {2181: G8Di8Do, 4602: B3U4I, 4603: B3U4I, 2470: G2Mi2Ao, 2471: G2Mi2Ao, 2472: G2Mi2Ao, 2431: G4Ai4Tmp,
               2432: G4Ai4Tmp, 2433: G4Ai4Tmp, 2434: G4Ai4Tmp, 2435: G4Ai4Tmp, 2436: G4Ai4Tmp}
     '''
     for node in connect.unit_id:
         for i in range(connect.master["local" + str(node)].number_bricks):
             id = connect.slave["master" + str(node)]["Brick" + str(i + 1)].brick_id
-            found = bricks.get(id, "None") # find brick name in dictionary or otherwise return "None"
+            found = bricks.get(id, "None")  # find brick name in dictionary or otherwise return "None"
             if found == "None":
                 error = open("error.txt", "a+")
                 error.write(f'{datetime.now()} ERROR: No Brick with ID {id} found.\n')
                 error.close()
-                brick_info += f'NOT FOUND! Brick {i+1}: {connect.slave["master" + str(node)]["Brick" + str(i+1)].name} '\
-                f'ID: {connect.slave["master" + str(node)]["Brick" + str(i+1)].brick_id // 1000}-{connect.slave["master" + str(node)]["Brick" + str(i+1)].brick_id % 1000} '\
-                f'Hardware Revision: {connect.slave["master" + str(node)]["Brick" + str(i+1)].hard_rev}\n'
+                brick_info += f'NOT FOUND! Brick {i + 1}: {connect.slave["master" + str(node)]["Brick" + str(i + 1)].name} ' \
+                              f'ID: {connect.slave["master" + str(node)]["Brick" + str(i + 1)].brick_id // 1000}-{connect.slave["master" + str(node)]["Brick" + str(i + 1)].brick_id % 1000} ' \
+                              f'Hardware Revision: {connect.slave["master" + str(node)]["Brick" + str(i + 1)].hard_rev}\n'
             else:
-                globals()[f"Brick{i + 1}"] = found(node, bricks[id], i+1, \
-                connect.slave["master" + str(node)]["Brick" + str(i+1)].brick_id,\
-                connect.slave["master" + str(node)]["Brick" + str(i+1)].data_miso,\
-                connect.slave["master" + str(node)]["Brick" + str(i+1)].data_mosi,\
-                connect.slave["master" + str(node)]["Brick" + str(i+1)].offset_miso,\
-                connect.slave["master" + str(node)]["Brick" + str(i+1)].offset_mosi)
-
-                found = "Brick"+str(i+1)
-
-                brick_info += f'{found}: {connect.slave["master" + str(node)]["Brick" + str(i+1)].name} '\
-                f'ID: {connect.slave["master" + str(node)]["Brick" + str(i+1)].brick_id // 1000}-{connect.slave["master" + str(node)]["Brick" + str(i+1)].brick_id % 1000} '\
-                f'Hardware Revision: {connect.slave["master" + str(node)]["Brick" + str(i+1)].hard_rev}\n'
+                globals()[f"Brick{i + 1}"] = found(node, bricks[id], i + 1,
+                                                   connect.slave["master" + str(node)]["Brick" + str(i + 1)].brick_id,
+                                                   connect.slave["master" + str(node)]["Brick" + str(i + 1)].data_miso,
+                                                   connect.slave["master" + str(node)]["Brick" + str(i + 1)].data_mosi,
+                                                   connect.slave["master" + str(node)][
+                                                       "Brick" + str(i + 1)].offset_miso,
+                                                   connect.slave["master" + str(node)][
+                                                       "Brick" + str(i + 1)].offset_mosi)
+
+                found = "Brick" + str(i + 1)
+
+                brick_info += f'{found}: {connect.slave["master" + str(node)]["Brick" + str(i + 1)].name} ' \
+                              f'ID: {connect.slave["master" + str(node)]["Brick" + str(i + 1)].brick_id // 1000}-{connect.slave["master" + str(node)]["Brick" + str(i + 1)].brick_id % 1000} ' \
+                              f'Hardware Revision: {connect.slave["master" + str(node)]["Brick" + str(i + 1)].hard_rev}\n'
     print(brick_info)
     print("To abort the program please press STRG + C\n\n")
 
 
 def start():
     return lock.release()
 
 
-
 class CAE_G8Di8Do:
     '''
     Brick Information can be found in eB_products.pdf under Chapter 1.6.1 G-8Di8Do-01
     Integrated Functions:
     digital_input(di_pos)
     digital_output(do_pos, value)
     '''
+
     def __init__(self, node, name, brick_no, brick_id, data_length_miso, data_length_mosi, offset_miso, offset_mosi):
         self.node = node
         self.name = name
         self.id = 2181
         self.brick_no = brick_no
         self.brick_id = brick_id
         # Data Lenght
@@ -136,14 +139,15 @@
     resultCnt()
     readPower()
     calcEnergy()
     readPhase()
     readCurrent()
     readVoltage()
     '''
+
     def __init__(self, node, name, brick_no, brick_id, data_length_miso, data_length_mosi, offset_miso, offset_mosi):
         self.node = node
         self.name = name
         self.id = [4602, 4603]
         self.brick_id = brick_id
         self.brick_no = brick_no
         # Data Lenght
@@ -173,15 +177,15 @@
         self.energy = [0] * 3
         self.maxsize = sys.maxsize
         self.run = False
         self.raw_power = [0] * 3
 
     def start(self):
         self.run = True
-    
+
     def stop(self):
         self.run = False
 
     def phase_cor(self, phase_cor_angle_l1, phase_cor_angle_l2, phase_cor_angle_l3):
         '''
         Set how much the phase angle for L1 - L3 should be corrected.
         '''
@@ -332,17 +336,19 @@
             self.offset_miso + 6]
         power_l2 = (bB_update.updated[self.node][self.offset_miso + 7] << 8) + bB_update.updated[self.node][
             self.offset_miso + 8]
         power_l3 = (bB_update.updated[self.node][self.offset_miso + 9] << 8) + bB_update.updated[self.node][
             self.offset_miso + 10]
         self.raw_power = [power_l1, power_l2, power_l3]
         if self.brick_id == 4602:
-            self.power = [i * self.pow_val_602 if i > self.filter_max or i < self.filter_min else 0 for i in np.int16(self.raw_power)]
+            self.power = [i * self.pow_val_602 if i > self.filter_max or i < self.filter_min else 0 for i in
+                          np.int16(self.raw_power)]
         else:
-            self.power = [i * self.pow_val_603 if i > self.filter_max or i < self.filter_min else 0 for i in np.int16(self.raw_power)]
+            self.power = [i * self.pow_val_603 if i > self.filter_max or i < self.filter_min else 0 for i in
+                          np.int16(self.raw_power)]
 
         return self.power
 
     def calcEnergy(self):
         '''
         Calculate and Return the Energy[L1, L2, L3] in Ws from Power[L1, L2, L3]
         '''
@@ -464,18 +470,19 @@
     pulse_input_sum1()   # Count the input pulse and give them back as value
     pulse_input_sum1_counter()  # Count from 0 to 3 in 1 second steps
     pulse_input_dif1()
     pulse_input_sum2() # Count the input pulse and give them back as value
     pulse_input_sum2_counter() # Count from 0 to 3 in 1 second steps
     pulse_input_dif2()
     '''
+
     def __init__(self, node, name, brick_no, brick_id, data_length_miso, data_length_mosi, offset_miso, offset_mosi):
         self.node = node
         self.name = name
-        #self.id = [2470, 2471, 2472]
+        # self.id = [2470, 2471, 2472]
         self.brick_id = brick_id
         self.brick_no = brick_no
         # Data Length
         self.data_length_miso = data_length_miso
         self.data_length_mosi = data_length_mosi
         # Offset
         self.offset_miso = offset_miso
@@ -491,15 +498,15 @@
         self.pulse_sum1 = 0
         self.pulse_sum2 = 0
         self.maxsize = sys.maxsize
         self.run = False
 
     def start(self):
         self.run = True
-    
+
     def stop(self):
         self.run = False
 
     def analog_output1(self, value):
         '''
         Set the analog output 1 to the value
         Brick ID 2-470, 2-471 set a value between 0..10 A
@@ -745,32 +752,33 @@
     analog_input3()
     analog_input4()
     temp_input1()
     temp_input2()
     temp_input3()
     temp_input4()
     '''
+
     def __init__(self, node, name, brick_no, brick_id, data_length_miso, data_length_mosi, offset_miso, offset_mosi):
         self.node = node
         self.name = name
         self.id = [2431, 2432, 2433, 2434, 2435, 2436]
         self.brick_id = brick_id
         self.brick_no = brick_no
         # Data Length
         self.data_length_miso = data_length_miso
         self.data_length_mosi = data_length_mosi
         # Offset
         self.offset_miso = offset_miso
         self.offset_mosi = offset_mosi
         self.digit_pt1000 = [0, 64, 128, 192, 256, 320, 384, 448, 512, 576, 640, 704, 768, 832, 896, 1000]
-        self.temp_pt1000 = [-78.276, -56.207, -33.929, -10.714, 13.6, 38.8, 65.217, 92.609, 121.364, 151.429, 183.0, 215.789,
-                250.556, 286.667, 325.0, 378.571]
+        self.temp_pt1000 = [-78.276, -56.207, -33.929, -10.714, 13.6, 38.8, 65.217, 92.609, 121.364, 151.429, 183.0,
+                            215.789,
+                            250.556, 286.667, 325.0, 378.571]
         self.y_interp = ''
 
-
     def analog_input1(self):
         '''
         Return the value in mini Ampere (0 - 20) by Brick ID 2-431, 2-432, 2-433)
                          in Volt (0 - 30) by Brick ID 2-434, 2-435, 2-436)
         '''
         lock.acquire()
         short = (bB_update.updated[self.node][self.offset_miso + 1] << 8) + bB_update.updated[self.node][
@@ -894,9 +902,7 @@
             ti = -10 + (60 / 948) * short
         elif self.brick_id in [2432, 2435]:
             ti = (110 / 901) * short
         elif self.brick_id in [2433, 2436]:
             ti = self.y_interp(short) if short > 0 and short < 1000 else None
         lock.release()
         return ti
-
-
```

### Comparing `emBRICK-0.20/emBRICK/ethernet.py` & `emBRICK-0.21/emBRICK/ethernet.py`

 * *Files identical despite different names*

### Comparing `emBRICK-0.20/emBRICK/modbus_rtu.py` & `emBRICK-0.21/emBRICK/modbus_rtu.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 #!/usr/bin/evn python3
 # Import Threading Module
 import threading
 import time
 import math
 import json
 from datetime import datetime
-import emBRICK.binary_utils as binary_utils 
+
+from pymodbus.exceptions import ConnectionException, ModbusException
+
+import emBRICK.binary_utils as binary_utils
 
 # Import pymodbus for the Modbus RTU Module
 from pymodbus.client.sync import ModbusSerialClient as ModbusClient
 lock = threading.Lock()
 
 filename = "error"
 ERROR = open(filename, "w+")
@@ -111,17 +114,17 @@
         self.updates = {}
         self.stopThread = False
     def getLWCsInfo(self):
         for id in connect.unit_id:
             i = 0
             # Reads in the Init Data in the address range 1000h ... 107 ch
             while(i < 5):
-                responce = connect.node.read_input_registers(4096,104, unit = id)
-                if not responce.isError():
-                    data_16byte = responce.registers
+                response = connect.node.read_input_registers(4096, 104, unit=id)
+                if not response.isError():
+                    data_16byte = response.registers
                     self.local_data[id] = binary_utils.convert16bitTo8bitList(data_16byte)
                     break
                 else:
                     ERROR.write(f'{datetime.now()}\tERROR: Connection to the Coupling-Master with Modbus Address {id} failed!\n')
                     i += 1
                 if i == 5:
                     ERROR.write(f'{datetime.now()}\tERROR: Connection to the Coupling-Master with Modbus Address {id} failed!\n')
@@ -132,20 +135,20 @@
             exit()
 
     def update_first(self, ):
         ''' Update the emBricks in the individual updaterate '''
         for id in connect.unit_id:
             i = 0
             while(i < 5):
-                responce = connect.node.read_input_registers(0, 120, unit=id)
+                response = connect.node.read_input_registers(0, 120, unit=id)
                 time.sleep(0.005)
-                if not responce.isError():
-                    self.updates[id] = responce.registers
+                if not response.isError():
+                    self.updates[id] = response.registers
                 else:
-                    ERROR.write(f'{datetime.now()}\tERROR: Checksum Error or Timeout\n')
+                    ERROR.write(f'{datetime.now()}\tERROR: Checksum Error or Timeout. {response}\n')
                     i += 1
                 if self.updates[id] != 0:
                     self.updated[id] = binary_utils.convert16bitTo8bitList(self.updates[id])
                     break
             if i == 5:
                 ERROR.write(f'{datetime.now()}\tERROR: Connection with LWCs on Modbus Address {id} not possible\n')
                 connect.unit_id.remove(id)
@@ -166,29 +169,25 @@
                 arguments = {
                     'read_address': 0,
                     'read_count': bB.buffer_length[id],
                     'write_address': 0,
                     'write_registers': bB.set[id],
                 }
 
-                try:
-                    response = connect.node.readwrite_registers(unit=id, **arguments)
+                response = connect.node.readwrite_registers(unit=id, **arguments)
+                if not response.isError():
                     self.updates[id] = response.registers
-                except ConnectionException as e:
-                    ERROR.write(f'{datetime.now()}\tERROR: Connection error: {e}\n')
-                except ModbusException as e:
-                    ERROR.write(f'{datetime.now()}\tERROR: Modbus error: {e}\n')
-                except Exception as e:
-                    ERROR.write(f'{datetime.now()}\tERROR: Unknown error: {e}\n')
+                else:
+                    ERROR.write(f'{datetime.now()}\tERROR: Connection error: {response}\n')
 
                 if self.updates[id] != 0:
                     lock.acquire()
                     self.updated[id] = binary_utils.convert16bitTo8bitList(self.updates[id])
-
                     lock.release()
+
                 if self.stopThread:
                     ERROR.close()
                     raise SystemExit()
             time.sleep(connect.updateRate)
 
 
 bB_update = brickBus_communication()
@@ -223,15 +222,15 @@
                 input += connect.slave["master" + str(id)]["Brick" + str(j+1)].data_miso
             input = math.ceil(input / 2)
             self.put[id] = [0] * output
             self.buffer_length[id] = input
 
     def getShort(self, node, module, bytePos):
         ''' Return the value in Size of 2 bytes(16bit) of the desired Byte Position '''
-        if  "Brick" + str(module) in connect.slave["master" + str(node)]:
+        if "Brick" + str(module) in connect.slave["master" + str(node)]:
             lock.acquire()
             byte1 = (bB_update.updated[node][connect.slave["master" + str(node)]["Brick" + str(module)].offset_miso + bytePos + 1]) << 8
             byte2 = bB_update.updated[node][connect.slave["master" + str(node)]["Brick" + str(module)].offset_miso + bytePos + 2]
             lock.release()
             self.gS = byte1 + byte2
         else:
             self.gS = None
```

### Comparing `emBRICK-0.20/emBRICK/modbus_tcp.py` & `emBRICK-0.21/emBRICK/modbus_tcp.py`

 * *Files identical despite different names*

### Comparing `emBRICK-0.20/emBRICK.egg-info/PKG-INFO` & `emBRICK-0.21/emBRICK.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: emBRICK
-Version: 0.20
+Version: 0.21
 Summary: Driver to build a connection RemoteMaster <-> LWCS over Ethernet, Modbus TCP & RTU
 Home-page: https://github.com/IMACS-GmbH/emBRICK/tree/main/Protocol%20Stacks/remoteBUS/Python%20via%20TCP-IP%20or%20RSxxx
 Download-URL: https://github.com/IMACS-GmbH/emBRICK/raw/main/Protocol%20Stacks/remoteBUS/Python%20via%20TCP-IP%20or%20RSxxx/emBRICK-0.15.tar.gz
 Author: IMACS
 Author-email: serkan.sen@imacs-gmbh.de
 License: MIT
 Keywords: IMACS,EMBRICK,PYTHON,TCP/IP,Modbus,RTU,TCP
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `emBRICK-0.20/setup.py` & `emBRICK-0.21/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 from distutils.core import setup
 setup(
   name = 'emBRICK',         # How you named your package folder (MyLib)
   packages = ['emBRICK'],   # Chose the same as "name"
-  version = '0.20',      # Start with a small number and increase it with every change you make
+  version = '0.21',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Driver to build a connection RemoteMaster <-> LWCS over Ethernet, Modbus TCP & RTU',   # Give a short description about your library
   author = 'IMACS',                   # Type in your name
   author_email = 'serkan.sen@imacs-gmbh.de',      # Type in your E-Mail
   url = 'https://github.com/IMACS-GmbH/emBRICK/tree/main/Protocol%20Stacks/remoteBUS/Python%20via%20TCP-IP%20or%20RSxxx',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/IMACS-GmbH/emBRICK/raw/main/Protocol%20Stacks/remoteBUS/Python%20via%20TCP-IP%20or%20RSxxx/emBRICK-0.15.tar.gz',    # I explain this later on
   keywords = ['IMACS', 'EMBRICK', 'PYTHON','TCP/IP','Modbus', 'RTU','TCP'],   # Keywords that define your package best
   install_requires=[            
           'threaded',
           'pyserial',
-          'pymodbus',
+          'pymodbus>=3.2',
           'sockets',
           'DateTime',
           'numpy',
           'scipy'
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
-    'Programming Language :: Python :: 3.4',
-    'Programming Language :: Python :: 3.5',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
   ],
 )
```

