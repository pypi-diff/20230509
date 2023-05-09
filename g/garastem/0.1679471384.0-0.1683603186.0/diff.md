# Comparing `tmp/garastem-0.1679471384.0.tar.gz` & `tmp/garastem-0.1683603186.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garastem-0.1679471384.0.tar", last modified: Wed Mar 22 07:49:44 2023, max compression
+gzip compressed data, was "garastem-0.1683603186.0.tar", last modified: Tue May  9 03:33:06 2023, max compression
```

## Comparing `garastem-0.1679471384.0.tar` & `garastem-0.1683603186.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-03-22 07:49:44.929737 garastem-0.1679471384.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      287 2023-03-22 07:49:44.929458 garastem-0.1679471384.0/PKG-INFO
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-03-22 07:49:44.926853 garastem-0.1679471384.0/garastem/
--rw-r--r--   0 curlyz     (501) staff       (20)     8864 2023-03-12 17:35:08.000000 garastem-0.1679471384.0/garastem/__init__ copy.py
--rw-r--r--   0 curlyz     (501) staff       (20)     8401 2023-03-22 03:02:44.000000 garastem-0.1679471384.0/garastem/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-03-22 07:49:44.000000 garastem-0.1679471384.0/garastem/version.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-03-22 07:49:44.929111 garastem-0.1679471384.0/garastem.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      287 2023-03-22 07:49:44.000000 garastem-0.1679471384.0/garastem.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      234 2023-03-22 07:49:44.000000 garastem-0.1679471384.0/garastem.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-03-22 07:49:44.000000 garastem-0.1679471384.0/garastem.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       42 2023-03-22 07:49:44.000000 garastem-0.1679471384.0/garastem.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-03-22 07:49:44.000000 garastem-0.1679471384.0/garastem.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-03-22 07:49:44.929814 garastem-0.1679471384.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1116 2023-03-03 09:28:24.000000 garastem-0.1679471384.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:33:06.668853 garastem-0.1683603186.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      287 2023-05-09 03:33:06.667649 garastem-0.1683603186.0/PKG-INFO
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:33:06.664341 garastem-0.1683603186.0/garastem/
+-rw-r--r--   0 curlyz     (501) staff       (20)     8864 2023-03-12 17:35:08.000000 garastem-0.1683603186.0/garastem/__init__ copy.py
+-rw-r--r--   0 curlyz     (501) staff       (20)     9583 2023-03-28 09:34:47.000000 garastem-0.1683603186.0/garastem/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-03-28 08:56:23.000000 garastem-0.1683603186.0/garastem/modules.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 03:33:06.000000 garastem-0.1683603186.0/garastem/version.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:33:06.666781 garastem-0.1683603186.0/garastem.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      287 2023-05-09 03:33:06.000000 garastem-0.1683603186.0/garastem.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      254 2023-05-09 03:33:06.000000 garastem-0.1683603186.0/garastem.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 03:33:06.000000 garastem-0.1683603186.0/garastem.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       42 2023-05-09 03:33:06.000000 garastem-0.1683603186.0/garastem.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 03:33:06.000000 garastem-0.1683603186.0/garastem.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 03:33:06.669079 garastem-0.1683603186.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1116 2023-03-03 09:28:24.000000 garastem-0.1683603186.0/setup.py
```

### Comparing `garastem-0.1679471384.0/garastem/__init__ copy.py` & `garastem-0.1683603186.0/garastem/__init__ copy.py`

 * *Files identical despite different names*

### Comparing `garastem-0.1679471384.0/garastem/__init__.py` & `garastem-0.1683603186.0/garastem/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,22 +27,36 @@
         print("Warning: Please update to latest version of this library")
 except Exception as err:
     # print(err)
     pass
 
 print('Running versions', version.version)
 
+class Port:
+    def __inint__(self, parent, index, name):
+        self.parent = parent
+        self.index = index
+        self.name = name
+        self.module = None
+    
 class GRobot:
     DISCONNECTED = 0
     CONNECTED = 1
     READY = 2
     discovered_devices = {}
     
     
     def __init__(self, name):
+        self.PORT1 = Port(self, 0, 'PORT1')
+        self.PORT2 = Port(self, 1, 'PORT2')
+        self.PORT3 = Port(self, 2, 'PORT3')
+        self.PORT4 = Port(self, 3, 'PORT4')
+        self.PORT5 = Port(self, 4, 'PORT5')
+        self.PORT6 = Port(self, 5, 'PORT6')
+        
         self.name = name
         self.buzzer = GRobot.Buzzer(self)
         self.motor = GRobot.Motor(self)
         self.led = GRobot.Pixel(self)
         
         self.state = GRobot.DISCONNECTED
         # ble
@@ -235,8 +249,43 @@
                     str(pixel),
                     str(color[0]),
                     str(color[1]),
                     str(color[2]),
                 ])
             await self.parent.send(f'*{pkg}#', expect=pkg)
                 
+
+
+class Button:
+    def __init__(self, port):
+        self.port = port
+        self.callbacks = {}
+    def when(self,event, do):
+        self.callbacks[event] = do
+
+class LightSensor:
+    def __init__(self, port):
+        self.port = port
+    async def read(self) -> float:
+        pass
+    
+class WeatherSensor:
+    def __init__(self, port):
+        self.port = port
+    async def read_temperature(self) -> float:
+        pass
+    async def read_humidity(self) -> float:
+        pass
+    
+class DistanceSensor:
+    def __init__(self,port):
+        self.port = port
+    async def measure(self) -> float:
+        pass
+
+class Relay:
+    def __init__(self, port):
+        self.port = port
+    
+    async def turn(self, state): 
+        pass
```

### Comparing `garastem-0.1679471384.0/setup.py` & `garastem-0.1683603186.0/setup.py`

 * *Files identical despite different names*

