# Comparing `tmp/hubitatcontrol-2.2.0.tar.gz` & `tmp/hubitatcontrol-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubitatcontrol-2.2.0.tar", max compression
+gzip compressed data, was "hubitatcontrol-2.3.0.tar", max compression
```

## Comparing `hubitatcontrol-2.2.0.tar` & `hubitatcontrol-2.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-2.2.0/LICENSE
--rw-r--r--   0        0        0     6311 2023-05-01 03:13:59.733229 hubitatcontrol-2.2.0/README.md
--rw-r--r--   0        0        0     2381 2023-05-01 03:13:59.733229 hubitatcontrol-2.2.0/hubitatcontrol/__init__.py
--rw-r--r--   0        0        0     3824 2023-05-01 03:13:59.733229 hubitatcontrol-2.2.0/hubitatcontrol/__main__.py
--rw-r--r--   0        0        0      172 2023-05-01 03:13:59.733229 hubitatcontrol-2.2.0/hubitatcontrol/environment.py
--rw-r--r--   0        0        0     1060 2023-04-23 03:06:31.104361 hubitatcontrol-2.2.0/hubitatcontrol/generic.py
--rw-r--r--   0        0        0     2902 2023-04-23 03:06:31.104361 hubitatcontrol-2.2.0/hubitatcontrol/hub.py
--rw-r--r--   0        0        0     2774 2023-04-23 03:06:31.104361 hubitatcontrol-2.2.0/hubitatcontrol/lights.py
--rw-r--r--   0        0        0      336 2023-04-29 01:51:56.296942 hubitatcontrol-2.2.0/hubitatcontrol/sensors.py
--rw-r--r--   0        0        0     2606 2023-05-01 03:17:15.357544 hubitatcontrol-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     7193 1970-01-01 00:00:00.000000 hubitatcontrol-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-2.3.0/LICENSE
+-rw-r--r--   0        0        0     6311 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.0/README.md
+-rw-r--r--   0        0        0     3072 2023-05-09 03:28:26.350568 hubitatcontrol-2.3.0/hubitatcontrol/__init__.py
+-rw-r--r--   0        0        0     3824 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.0/hubitatcontrol/__main__.py
+-rw-r--r--   0        0        0      172 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.0/hubitatcontrol/environment.py
+-rw-r--r--   0        0        0     1060 2023-04-23 03:06:31.104361 hubitatcontrol-2.3.0/hubitatcontrol/generic.py
+-rw-r--r--   0        0        0     2902 2023-04-23 03:06:31.104361 hubitatcontrol-2.3.0/hubitatcontrol/hub.py
+-rw-r--r--   0        0        0     2774 2023-04-23 03:06:31.104361 hubitatcontrol-2.3.0/hubitatcontrol/lights.py
+-rw-r--r--   0        0        0      478 2023-05-09 03:28:26.350568 hubitatcontrol-2.3.0/hubitatcontrol/sensors.py
+-rw-r--r--   0        0        0     2606 2023-05-09 03:36:53.317222 hubitatcontrol-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7193 1970-01-01 00:00:00.000000 hubitatcontrol-2.3.0/PKG-INFO
```

### Comparing `hubitatcontrol-2.2.0/LICENSE` & `hubitatcontrol-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.2.0/README.md` & `hubitatcontrol-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.2.0/hubitatcontrol/__init__.py` & `hubitatcontrol-2.3.0/hubitatcontrol/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,19 @@
         return hubitatcontrol.lights.Bulb(device_from_hub=device_in, hub=hub_in)
     if "SwitchLevel" in device_in["capabilities"]:
         return hubitatcontrol.lights.Dimmer(device_from_hub=device_in, hub=hub_in)
     if "PowerMeter" in device_in["capabilities"] and "Outlet" in device_in["capabilities"]:
         return hubitatcontrol.generic.ZigbeeOutlet(device_from_hub=device_in, hub=hub_in)
     if "Switch" in device_in["capabilities"]:
         return hubitatcontrol.generic.Switch(device_from_hub=device_in, hub=hub_in)
+    if (
+        "TemperatureMeasurement" in device_in["capabilities"]
+        and "RelativeHumidityMeasurement" in device_in["capabilities"]
+    ):
+        return hubitatcontrol.sensors.EnvironmentalSensor(device_from_hub=device_in, hub=hub_in)
     if "TemperatureMeasurement" in device_in["capabilities"]:
         return hubitatcontrol.sensors.TemperatureSensor(device_from_hub=device_in, hub=hub_in)
 
 
 def get_hub(host, token, app_id, cloud_token=None) -> Hub:
     return Hub(host=host, token=token, app_id=app_id, cloud_token=cloud_token)
 
@@ -37,21 +42,31 @@
     return get_device_type(
         device_in=hub_in.get_device(device_lookup), hub_in=hub_in
     )  # Fall through return # pragma: no cover
 
 
 def lookup_device_id(hub_in, device_id):
     """
-    Takes device NAME, not ID for lookup
+    Takes device ID for lookup
     """
     return get_device_type(
         device_in=hub_in.get_device_id(device_id), hub_in=hub_in
     )  # Fall through return # pragma: no cover
 
 
+# TODO Refactor this to be dry
 def get_all_temperature_sensors(hub_in: hubitatcontrol.hub) -> list[hubitatcontrol.sensors.TemperatureSensor]:
     """Returns list of all hub devices with associated helper functions"""
     device_list = []
     for i in hub_in.devices:
         if "TemperatureMeasurement" in i["capabilities"]:
-            device_list.append(lookup_device_id(hub_in, i['id']))
+            device_list.append(get_device_type(i, hub_in))
+    return device_list
+
+
+def get_all_env_sensors(hub_in: hubitatcontrol.hub) -> list[hubitatcontrol.sensors.EnvironmentalSensor]:
+    """Returns list of all hub devices with associated helper functions"""
+    device_list = []
+    for i in hub_in.devices:
+        if ("RelativeHumidityMeasurement" in i["capabilities"]) and ("TemperatureMeasurement" in i["capabilities"]):
+            device_list.append(get_device_type(i, hub_in))
     return device_list
```

### Comparing `hubitatcontrol-2.2.0/hubitatcontrol/__main__.py` & `hubitatcontrol-2.3.0/hubitatcontrol/__main__.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.2.0/hubitatcontrol/generic.py` & `hubitatcontrol-2.3.0/hubitatcontrol/generic.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.2.0/hubitatcontrol/hub.py` & `hubitatcontrol-2.3.0/hubitatcontrol/hub.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.2.0/hubitatcontrol/lights.py` & `hubitatcontrol-2.3.0/hubitatcontrol/lights.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.2.0/pyproject.toml` & `hubitatcontrol-2.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hubitatcontrol"
-version = "v2.2.0"
+version = "v2.3.0"
 description = "Hubitat Maker API Interface"
 authors = ["Jesse Schoepfer <jelloeater@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/Jelloeater/hubitatcontrol"
 keywords = ["hubitat", "makerapi","requests"]
 classifiers = ["Development Status :: 5 - Production/Stable",
```

### Comparing `hubitatcontrol-2.2.0/PKG-INFO` & `hubitatcontrol-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubitatcontrol
-Version: 2.2.0
+Version: 2.3.0
 Summary: Hubitat Maker API Interface
 Home-page: https://github.com/Jelloeater/hubitatcontrol
 License: MIT
 Keywords: hubitat,makerapi,requests
 Author: Jesse Schoepfer
 Author-email: jelloeater@gmail.com
 Requires-Python: >=3.10,<4.0
```

