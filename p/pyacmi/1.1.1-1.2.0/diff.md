# Comparing `tmp/pyacmi-1.1.1.tar.gz` & `tmp/pyacmi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacmi-1.1.1.tar", last modified: Tue May  9 08:41:35 2023, max compression
+gzip compressed data, was "pyacmi-1.2.0.tar", last modified: Tue May  9 19:49:12 2023, max compression
```

## Comparing `pyacmi-1.1.1.tar` & `pyacmi-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 08:41:35.404556 pyacmi-1.1.1/
--rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 16:16:44.000000 pyacmi-1.1.1/LICENSE
--rw-r--r--   0 wangtong   (501) staff       (20)     1407 2023-05-09 08:41:35.404441 pyacmi-1.1.1/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      729 2023-05-08 16:16:44.000000 pyacmi-1.1.1/README.md
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 08:41:35.403650 pyacmi-1.1.1/pyacmi/
--rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 16:19:56.000000 pyacmi-1.1.1/pyacmi/__init__.py
--rw-r--r--   0 wangtong   (501) staff       (20)    23217 2023-05-09 08:40:58.000000 pyacmi-1.1.1/pyacmi/acmi.py
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 08:41:35.404265 pyacmi-1.1.1/pyacmi.egg-info/
--rw-r--r--   0 wangtong   (501) staff       (20)     1407 2023-05-09 08:41:35.000000 pyacmi-1.1.1/pyacmi.egg-info/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-09 08:41:35.000000 pyacmi-1.1.1/pyacmi.egg-info/SOURCES.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-09 08:41:35.000000 pyacmi-1.1.1/pyacmi.egg-info/dependency_links.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       17 2023-05-09 08:41:35.000000 pyacmi-1.1.1/pyacmi.egg-info/requires.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-09 08:41:35.000000 pyacmi-1.1.1/pyacmi.egg-info/top_level.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-09 08:41:35.404599 pyacmi-1.1.1/setup.cfg
--rw-r--r--   0 wangtong   (501) staff       (20)     1022 2023-05-09 08:41:31.000000 pyacmi-1.1.1/setup.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 19:49:12.191181 pyacmi-1.2.0/
+-rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 16:16:44.000000 pyacmi-1.2.0/LICENSE
+-rw-r--r--   0 wangtong   (501) staff       (20)     2083 2023-05-09 19:49:12.191053 pyacmi-1.2.0/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)     1405 2023-05-09 19:47:49.000000 pyacmi-1.2.0/README.md
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 19:49:12.189774 pyacmi-1.2.0/pyacmi/
+-rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 16:19:56.000000 pyacmi-1.2.0/pyacmi/__init__.py
+-rw-r--r--   0 wangtong   (501) staff       (20)    35803 2023-05-09 19:47:21.000000 pyacmi-1.2.0/pyacmi/acmi.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 19:49:12.190857 pyacmi-1.2.0/pyacmi.egg-info/
+-rw-r--r--   0 wangtong   (501) staff       (20)     2083 2023-05-09 19:49:12.000000 pyacmi-1.2.0/pyacmi.egg-info/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-09 19:49:12.000000 pyacmi-1.2.0/pyacmi.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-09 19:49:12.000000 pyacmi-1.2.0/pyacmi.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       22 2023-05-09 19:49:12.000000 pyacmi-1.2.0/pyacmi.egg-info/requires.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-09 19:49:12.000000 pyacmi-1.2.0/pyacmi.egg-info/top_level.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-09 19:49:12.191332 pyacmi-1.2.0/setup.cfg
+-rw-r--r--   0 wangtong   (501) staff       (20)     1030 2023-05-09 19:48:33.000000 pyacmi-1.2.0/setup.py
```

### Comparing `pyacmi-1.1.1/LICENSE` & `pyacmi-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacmi-1.1.1/PKG-INFO` & `pyacmi-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.1.1
+Version: 1.2.0
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
@@ -23,29 +23,53 @@
 [![License](https://img.shields.io/pypi/l/pyacmi.svg)](https://github.com/wangtong2015/pyacmi)
 [![Package Status](https://img.shields.io/pypi/status/pyacmi.svg)](https://pypi.org/project/pyacmi/)
 
 `**.acmi` is a file used by tacview for creating flight recording from simulators or real world.
 
 The source code is currently hosted on GitHub at: https://github.com/wangtong2015/pyacmi
 
-## Install
+ACMI file Introduction:  [Tacview - ACMI flight recordings.md](Tacview - ACMI flight recordings.md)
+
+## Installation
+
+You can install pyacmi via pip or pip3 for Python 3+:
+
+```shell
+$ pip3 install pyacmi
+```
+
+You can install a specific version of pyacmi by:
 
 ```shell
+$ pip3 install pyacmi==1.1.0
+```
 
-pip install pyacmi
+You can upgrade pyacmi to the latest version by:
 
+```shell
+$ pip3 install --upgrade pyacmi
 ```
 
 ## Example
 
 ```python
 
-from pyacmi import *
+from pyacmi import Acmi
 
 acmi = Acmi('test.acmi')
 print(acmi)
 
+print(acmi.reference_latitude, acmi.reference_longitude, acmi.reference_time)
+
+# 打印所有的object
+for obj_id in acmi.objects:
+    obj = acmi.objects[obj_id]
+    print(obj)
+    print(obj.id, obj.name, obj.country, obj.tags, obj.type)
+
+# 导出成csv
+acmi.export_csv('test.csv', remove_empty=True, export_obj_ids=None)
 ```
 
 ## Credits
 
 - [https://github.com/rp-/acmi](https://github.com/rp-/acmi)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyacmi-1.1.1/pyacmi/acmi.py` & `pyacmi-1.2.0/pyacmi/acmi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,189 @@
+"""
+documentation: https://www.tacview.net/documentation/acmi/
+"""
+import os.path
 import zipfile
 import datetime
 import sortedcontainers
 import bisect
 import json
 import io
 from constantly import ValueConstant
+import csv
+from typing import Union, Optional
+from tqdm import tqdm
+
+ACMI_FILE_ENCODING = 'utf-8-sig'
+
+ACMI_NUMERIC_PROPERTIES = {
+    'Importance',
+    'Slot',
+    'Disabled', 'Visible',
+    'Health',
+    'Length', 'Width', 'Height',
+    'Radius',
+    'IAS', 'CAS', 'TAS', 'Mach', 'AOA', 'AOS', 'AGL', 'HDG', 'HDM',
+    'Throttle', 'Throttle2',
+    'EngineRPM', 'EngineRPM2',
+    'Afterburner', 'AirBrakes',
+    'Flaps',
+    'LandingGear', 'LandingGearHandle',
+    "Tailhook",
+    "Parachute", "DragChute",
+    'FuelWeight', 'FuelWeight2', 'FuelWeight3', 'FuelWeight4', 'FuelWeight5', 'FuelWeight6', 'FuelWeight7',
+    'FuelWeight8', 'FuelWeight9',
+    'FuelVolume', 'FuelVolume2', 'FuelVolume3', 'FuelVolume4', 'FuelVolume5', 'FuelVolume6', 'FuelVolume7',
+    'FuelVolume8', 'FuelVolume9',
+    'FuelFlowWeight', 'FuelFlowWeight2', 'FuelFlowWeight3', 'FuelFlowWeight4', 'FuelFlowWeight5', 'FuelFlowWeight6',
+    'FuelFlowWeight7', 'FuelFlowWeight8',
+    'FuelFlowVolume', 'FuelFlowVolume2', 'FuelFlowVolume3', 'FuelFlowVolume4', 'FuelFlowVolume5', 'FuelFlowVolume6',
+    'FuelFlowVolume7', 'FuelFlowVolume8',
+    'RadarMode',
+    'RadarAzimuth',
+    'RadarElevation',
+    'RadarRoll',
+    'RadarRange',
+    'RadarHorizontalBeamwidth',
+    'RadarVerticalBeamwidth',
+    'RadarRangeGateAzimuth',
+    'RadarRangeGateElevation',
+    'RadarRangeGateRoll', 'RadarRangeGateMin', 'RadarRangeGateMax',
+    'RadarRangeGateHorizontalBeamwidth', 'RadarRangeGateVerticalBeamwidth',
+    'LockedTargetMode',
+    "LockedTargetAzimuth",
+    'LockedTargetElevation',
+    'LockedTargetRange',
+
+    'EngagementMode', 'EngagementMode2',
+    'EngagementRange', 'EngagementRange2',
+    'VerticalEngagementRange', 'VerticalEngagementRange2',
+    'RollControlInput', 'PitchControlInput', 'YawControlInput',
+    "RollControlPosition", "PitchControlPosition", "YawControlPosition",
+    'RollTrimTab', 'PitchTrimTab', 'YawTrimTab',
+    'AileronLeft', 'AileronRight', 'Elevator', 'Rudder',
+    'PilotHeadRoll', 'PilotHeadPitch', "PilotHeadYaw",
+    'VerticalGForce', 'LongitudinalGForce', 'LateralGForce',
+    'TriggerPressed',
+    'ENL',
+    'HeartRate',
+    'SpO2'
+}
+
+ACMI_TEXT_PROPERTIES = {
+    'Name',
+    # Object types are built using tags. This makes object management much more powerful and transparent than with the previous exclusive types. (see below for the list of supported types). Type and Name are the only properties which *CANNOT* be predefined in Tacview
+    'Type',
+    'AdditionalType',
+    'Parent',
+    'Next',
+    'ShortName',
+    'LongName',
+    'FullName',
+    'CallSign',
+    'Registration',
+    'Squawk',
+    'ICAO24',
+    'Pilot',
+    'Group',
+    'Country',
+    'Coalition',
+    'Color',
+    'Shape',
+    'Debug',
+    'Label',
+    'FocusedTarget',
+    'LockedTarget', 'LockedTarget2', 'LockedTarget3', 'LockedTarget4', 'LockedTarget5', 'LockedTarget6',
+    'LockedTarget7', 'LockedTarget8', 'LockedTarget9',
+}
 
-_ACMI_FILE_ENCODING = 'utf-8-sig'
-_FLOAT_OBJECT_KEYS = {
-    "Importance", "Length", "Width", "Height",
-    "IAS", "CAS", "TAS", "Mach", "AOA", "HDG",
-    "HDM", "Throttle", "RadarAzimuth", "RadarElevation",
-    "RadarRange", "LockedTargetAzimuth",
-    "LockedTargetElevation", "LockedTargetRange", "Flaps", "LandingGear",
-    "AirBrakes",
-    "PilotHeadRoll", "PilotHeadPitch", "PilotHeadYaw",
-    "RollControlPosition", "PitchControlPosition", "YawControlPosition" }
-_INT_OBJECT_KEYS = { "Slot", "Afterburner", "Tailhook",
-                     "Parachute", "DragChute", "RadarMode",
-                     "LockedTargetMode" }
-_STR_OBJECT_KEYS = { "Pilot", "Group", "Country", "Coalition",
-                     "Color", "Registration", "Squawk", "Debug", "Label" }
+# acmi导出csv的header
+ACMI_EXPORT_CSV_HEADERS = [
+    'ReferenceTime',
+    'Category',
+    'ID',
+    'Name'
+    'Tags',
+    'Type',
+    'Time',
+
+    'AdditionalType',
+    'Parent',
+    'Next',
+    'ShortName',
+    'LongName',
+    'FullName',
+    'CallSign',
+    'Registration',
+    'Squawk',
+    'ICAO24',
+    'Pilot',
+    'Group',
+    'Country',
+    'Coalition',
+    'Color',
+    'Shape',
+    'Debug',
+    'Label',
+    'FocusedTarget',
+    'LockedTarget', 'LockedTarget2', 'LockedTarget3', 'LockedTarget4', 'LockedTarget5', 'LockedTarget6',
+    'LockedTarget7', 'LockedTarget8', 'LockedTarget9',
+
+    'Importance',
+    'Slot',
+    'Disabled', 'Visible',
+    'Health',
+    'Length', 'Width', 'Height',
+    'Radius',
+    'IAS', 'CAS', 'TAS', 'Mach', 'AOA', 'AOS', 'AGL', 'HDG', 'HDM',
+    'Throttle', 'Throttle2',
+    'EngineRPM', 'EngineRPM2',
+    'Afterburner', 'AirBrakes',
+    'Flaps',
+    'LandingGear', 'LandingGearHandle',
+    "Tailhook",
+    "Parachute", "DragChute",
+    'FuelWeight', 'FuelWeight2', 'FuelWeight3', 'FuelWeight4', 'FuelWeight5', 'FuelWeight6', 'FuelWeight7',
+    'FuelWeight8', 'FuelWeight9',
+    'FuelVolume', 'FuelVolume2', 'FuelVolume3', 'FuelVolume4', 'FuelVolume5', 'FuelVolume6', 'FuelVolume7',
+    'FuelVolume8', 'FuelVolume9',
+    'FuelFlowWeight', 'FuelFlowWeight2', 'FuelFlowWeight3', 'FuelFlowWeight4', 'FuelFlowWeight5', 'FuelFlowWeight6',
+    'FuelFlowWeight7', 'FuelFlowWeight8',
+    'FuelFlowVolume', 'FuelFlowVolume2', 'FuelFlowVolume3', 'FuelFlowVolume4', 'FuelFlowVolume5', 'FuelFlowVolume6',
+    'FuelFlowVolume7', 'FuelFlowVolume8',
+    'RadarMode',
+    'RadarAzimuth',
+    'RadarElevation',
+    'RadarRoll',
+    'RadarRange',
+    'RadarHorizontalBeamwidth',
+    'RadarVerticalBeamwidth',
+    'RadarRangeGateAzimuth',
+    'RadarRangeGateElevation',
+    'RadarRangeGateRoll', 'RadarRangeGateMin', 'RadarRangeGateMax',
+    'RadarRangeGateHorizontalBeamwidth', 'RadarRangeGateVerticalBeamwidth',
+    'LockedTargetMode',
+    "LockedTargetAzimuth",
+    'LockedTargetElevation',
+    'LockedTargetRange',
+
+    'EngagementMode', 'EngagementMode2',
+    'EngagementRange', 'EngagementRange2',
+    'VerticalEngagementRange', 'VerticalEngagementRange2',
+    'RollControlInput', 'PitchControlInput', 'YawControlInput',
+    "RollControlPosition", "PitchControlPosition", "YawControlPosition",
+    'RollTrimTab', 'PitchTrimTab', 'YawTrimTab',
+    'AileronLeft', 'AileronRight', 'Elevator', 'Rudder',
+    'PilotHeadRoll', 'PilotHeadPitch', "PilotHeadYaw",
+    'VerticalGForce', 'LongitudinalGForce', 'LateralGForce',
+    'TriggerPressed',
+    'ENL',
+    'HeartRate',
+    'SpO2'
+]
 
 
 class AcmiType(ValueConstant):
     Plane = 'Plane'
     Helicopter = 'Helicopter'
     AntiAircraft = 'AntiAircraft'
     Armor = 'Armor'
@@ -101,15 +260,15 @@
     AcmiType.MinorObject    : ['Misc+Minor'],
     AcmiType.Explosion      : ['Misc+Explosion'],
     AcmiType.F16C           : ['Medium+Air+FixedWing'],
     AcmiType.Bicycle        : ['Light+Ground+Vehicle'],
     AcmiType.AIM120C        : ['Medium+Weapon+Missile'],
 }
 
-# 将_ACMI_TYPE_TAGS预处理（内部按照顺序排序，方便后续匹配）
+# 将_ACMI_TYPE_TAGS预处理（内部按照ascii顺序排序，方便后续快速匹配）
 for k in ACMI_TYPE_TAGS:
     tags = ACMI_TYPE_TAGS[k]
     ACMI_TYPE_TAGS[k] = ['+'.join(sorted(tag.split('+'))) for tag in tags]
 
 
 class AcmiObject:
 
@@ -153,167 +312,272 @@
         return AcmiType.Shrapnel in self.type
 
     # 牛眼: 空战中心点的位置，用来方便飞行员报告目标位置和距离
     @property
     def is_bullseye(self):
         return AcmiType.Bullseye in self.type
 
-    def set_value(self, field, timeframe, val):
+    def set_value(self, field: str, timeframe: float, val: Union[int, float, str]):
+        def do_set_value(do_field, do_val):
+            if do_field not in self.data:
+                self.data[do_field] = sortedcontainers.SortedDict()
+            self.data[do_field][timeframe] = do_val
+
         if field == 'Type':
             match_tags = '+'.join(sorted(val.split('+')))
             match_types = []
             self.tags = val
+            do_set_value('Tags', self.type)
             if not self.type:
                 for _type in ACMI_TYPE_TAGS:
                     if match_tags in ACMI_TYPE_TAGS[_type]:
                         match_types.append(_type)
                 self.type = '+'.join(match_types)
+                do_set_value('Type', self.type)
             return
         elif field == 'Name':
             self.name = val
-            return
         elif field == 'Country':
             self.country = val
-            return
-
-        if field not in self.data:
-            self.data[field] = sortedcontainers.SortedDict()
-        self.data[field][timeframe] = val
+        do_set_value(field, val)
 
     # 该类的get_value函数用于获取指定场景下（field）的数据值。
     # 如果指定了timeframe参数，
     #   如果timeframe存在，则返回对应时间点的值或
     #   否则，返回timeframe上一条时间点的值（不存在则返回第一条数据）
     # 否则，返回场景最近一条数据的值。
-    def get_value(self, field: str, timeframe=None):
+    def get_value(self, field: str, time: Optional[float] = None):
         if field not in self.data:
             return None
         data = self.data[field]
         timeframe_keys = data.keys()
         if len(timeframe_keys) == 0:
             return None
 
-        if timeframe is not None:
-            if timeframe in timeframe_keys:
-                return data[timeframe]
-            pos = bisect.bisect_left(timeframe_keys, timeframe)
+        if time is not None:
+            if time in timeframe_keys:
+                return data[time]
+            pos = bisect.bisect_left(timeframe_keys, time)
             if pos == 0:
                 return data[timeframe_keys[0]]
             else:
                 return data[timeframe_keys[pos - 1]]
         return data[timeframe_keys[-1]]
 
+    def u(self, time: Optional[float] = None):
+        return self.get_value("U", time)
+
+    def v(self, time: Optional[float] = None):
+        return self.get_value('V', time)
+
     # Latitude：对象的纬度。用于标识对象所在的位置。例如，F-16飞机的纬度为“32.1234”。
-    def latitude(self, time=None):
+    def latitude(self, time: Optional[float] = None):
         return self.get_value("Latitude", time)
 
     # Longitude：对象的经度。用于标识对象所在的位置。例如，F-16飞机的经度为“-117.2345”。
-    def longitude(self, time=None):
+    def longitude(self, time: Optional[float] = None):
         return self.get_value("Longitude", time)
 
     # Altitude：对象的高度。用于标识对象所在的高度。例如，F-16飞机的高度为“10000”。
-    def altitude(self, time=None):
+    def altitude(self, time: Optional[float] = None):
         return self.get_value("Altitude", time)
 
     # Heading：对象的航向。用于标识对象的方向。例如，F-16飞机的航向为“280”。
-    def heading(self, time=None):
+    def heading(self, time: Optional[float] = None):
         return self.get_value("Heading", time)
 
     # Pitch：对象的俯仰角。用于标识对象的俯仰角度。例如，F-16飞机的俯仰角为“10”。
-    def pitch(self, time=None):
+    def pitch(self, time: Optional[float] = None):
         return self.get_value("Pitch", time)
 
+    # Yaw：对象的偏航角。用于标识对象的偏航角度。例如，F-16飞机的偏航角为“30”。
+    def yaw(self, time: Optional[float] = None):
+        return self.get_value("Yaw", time)
+
     # Roll：对象的横滚角。用于标识对象的横滚角度。例如，F-16飞机的横滚角为“20”。
-    def roll(self, time=None):
+    def roll(self, time: Optional[float] = None):
         return self.get_value("Roll", time)
 
-    # IAS：对象的空速。用于标识对象的速度。例如，F-16飞机的空速为“300”。
-    def ias(self, time=None):
-        return self.get_value("IAS", time)
-
-    # Flaps：对象的襟翼状态。用于标识对象襟翼的状态。例如，F-16飞机的襟翼状态为“放下”。
-    def flaps(self, time=None):
-        return self.get_value("Flaps", time)
-
-    # LandingGear：对象的起落架状态。用于标识对象起落架的状态。例如，F-16飞机的起落架状态为“收起”。
-    def landing_gear(self, time=None):
-        return self.get_value("LandingGear", time)
-
-    # AirBrakes：对象的空气刹车状态。用于标识对象空气刹车的状态。例如，F-16飞机的空气刹车状态为“关闭”。
-    def air_brakes(self, time=None):
-        return self.get_value("AirBrakes", time)
-
     # PitchControlPosition：对象的俯仰控制杆位置。用于标识对象的俯仰控制杆位置。例如，F-16飞机的俯仰控制杆位置为“中间”。
-    def pitch_control_position(self, time=None):
+    def pitch_control_position(self, time: Optional[float] = None):
         return self.get_value("PitchControlPosition", time)
 
     # RollControlPosition：对象的横滚控制杆位置。用于标识对象的横滚控制杆位置。例如，F-16飞机的横滚控制杆位置为“左”。
-    def roll_control_position(self, time=None):
+    def roll_control_position(self, time: Optional[float] = None):
         return self.get_value("RollControlPosition", time)
 
     # YawControlPosition：对象的偏航控制杆位置。用于标识对象的偏航控制杆位置。例如，F-16飞机的偏航控制杆位置为“右”。
-    def yaw_control_position(self, time=None):
+    def yaw_control_position(self, time: Optional[float] = None):
         return self.get_value("YawControlPosition", time)
 
-    # Yaw：对象的偏航角。用于标识对象的偏航角度。例如，F-16飞机的偏航角为“30”。
-    def yaw(self, time=None):
-        return self.get_value("Yaw", time)
-
     # Pilot：对象的驾驶员。用于标识对象的驾驶员。例如，F-16飞机的驾驶员为“Tom”。
-    def pilot(self, time=None):
+    def pilot(self, time: Optional[float] = None):
         return self.get_value("Pilot", time)
 
     # PilotHeadPitch：驾驶员的头部俯仰角。用于标识驾驶员的头部俯仰角度。例如，驾驶员的头部俯仰角为“-10”。
-    def pilot_head_pitch(self, time=None):
+    def pilot_head_pitch(self, time: Optional[float] = None):
         return self.get_value("PilotHeadPitch", time)
 
     # PilotHeadRoll：驾驶员的头部横滚角。用于标识驾驶员的头部横滚角度。例如，驾驶员的头部横滚角为“0”。
-    def pilot_head_roll(self, time=None):
+    def pilot_head_roll(self, time: Optional[float] = None):
         return self.get_value("PilotHeadRoll", time)
 
     # PilotHeadYaw：驾驶员的头部偏航角。用于标识驾驶员的头部偏航角度。例如，驾驶员的头部偏航角为“20”。
-    def pilot_head_yaw(self, time=None):
+    def pilot_head_yaw(self, time: Optional[float] = None):
         return self.get_value("PilotHeadYaw", time)
 
-    def json(self):
-        return {
-            'ID'                  : self.id,
-            'Name'                : self.name,
-            'Tags'                : self.tags,
-            'Type'                : self.type,
-            'Country'             : self.country,
-            'Latitude'            : self.latitude(),
-            'Longitude'           : self.longitude(),
-            'Altitude'            : self.altitude(),
-            'Heading'             : self.heading(),
-            'Pitch'               : self.pitch(),
-            'Roll'                : self.roll(),
-            'IAS'                 : self.ias(),
-            'Flaps'               : self.flaps(),
-            'LandingGear'         : self.landing_gear(),
-            'AirBrakes'           : self.air_brakes(),
-            'PitchControlPosition': self.pitch_control_position(),
-            'RollControlPosition' : self.roll_control_position(),
-            'YawControlPosition'  : self.yaw_control_position(),
-            'Yaw'                 : self.yaw(),
-            'Pilot'               : self.pilot(),
-            'PilotHeadPitch'      : self.pilot_head_pitch(),
-            'PilotHeadRoll'       : self.pilot_head_roll(),
-            'PilotHeadYaw'        : self.pilot_head_yaw()
+    # 父十六进制对象ID。用于将导弹（子对象）与其发射飞机（父对象）关联起来非常有用
+    def parent(self, time: Optional[float] = None):
+        return self.get_value('Parent', time)
+
+    # 呼号
+    def call_sign(self, time: Optional[float] = None):
+        return self.get_value('CallSign', time)
+
+    # 飞机注册号（机尾号码）
+    def registration(self, time: Optional[float] = None):
+        return self.get_value('Registration', time)
+
+    # 联盟
+    def coalition(self, time: Optional[float] = None):
+        return self.get_value('Coalition', time)
+
+    def color(self, time: Optional[float] = None):
+        return self.get_value('Color', time)
+
+    # 当前由对象聚焦的目标（通常用于指定激光束目标对象，也可以用于显示飞行员当前聚焦的内容）
+    def focused_target(self, time: Optional[float] = None):
+        return self.get_value('FocusedTarget', time)
+
+    # 首要目标的十六进制ID（0到9）（可以使用任何设备（如雷达，红外线，夜视仪等）进行锁定）
+    def locked_target(self, index: int = 0, time=None):
+        key = 'LockedTarget'
+        if index > 0:
+            key += index
+
+        return self.get_value(key, time)
+
+    # 重要性因素越高，对象就越重要（例如，本地模拟飞机的重要性因素可能为1.0）
+    def importance(self, time: Optional[float] = None):
+        return self.get_value('Importance', time)
+
+    # 飞机在其编队中的位置（0代表最低，是领航员）
+    def slot(self, time: Optional[float] = None):
+        return self.get_value('Slot', time)
+
+    # 指定对象在尚未被摧毁的情况下被禁用（通常是在战斗之外）。这在战斗训练和射击记录中特别有用。
+    def disabled(self, time: Optional[float] = None):
+        return self.get_value('Disabled', time)
+
+    # 这个属性用于从三维视图中隐藏特定对象。可以用于制造战争迷雾效果，或防止虚拟对象被显示。当设置为1时，对象是完全可见的。当设置为0时，对象是看不见的，可能被从对象列表中省略。
+    def visible(self, time: Optional[float] = None):
+        return self.get_value('Visible', time)
+
+    # 使用这个属性记录对象的当前健康状态。当对象全新时，比率等于1.0，当对象处于战斗/死亡/摧毁状态时，比率为0.0。该属性目前对事件没有影响，仍需手动删除对象
+    def health(self, time: Optional[float] = None):
+        return self.get_value('Health', time)
+
+    # 对象长度。在显示建筑物时尤其有用
+    def length(self, time: Optional[float] = None):
+        return self.get_value('Length', time)
+
+    def width(self, time: Optional[float] = None):
+        return self.get_value('Width', time)
+
+    def radius(self, time: Optional[float] = None):
+        return self.get_value('Radius', time)
+
+    # IAS：对象的空速。用于标识对象的速度。例如，F-16飞机的空速为“300”。
+    def ias(self, time: Optional[float] = None):
+        return self.get_value('IAS', time)
+
+    def cas(self, time: Optional[float] = None):
+        return self.get_value('CAS', time)
+
+    def tas(self, time: Optional[float] = None):
+        return self.get_value('TAS', time)
+
+    def mach(self, time: Optional[float] = None):
+        return self.get_value('Mach', time)
+
+    # AOA (Angle of Attack) 是指飞机相对于气流的进出角度。它是一项非常重要的飞行指标，在飞行中用于监测飞机的飞行状态。过高或过低的 AOA 都可能会导致飞机进入危险状态，因此飞行员需要时刻关注并控制 AOA。在模拟飞行游戏 DCS World 中，也需要考虑和控制 AOA 以获得更稳定、安全的飞行体验。
+    def aoa(self, time: Optional[float] = None):
+        return self.get_value('AOA', time)
+
+    # 侧滑角，也叫侧滑角度
+    def aos(self, time: Optional[float] = None):
+        return self.get_value('AOS', time)
+
+    def agl(self, time: Optional[float] = None):
+        return self.get_value('AGL', time)
+
+    def hdg(self, time: Optional[float] = None):
+        return self.get_value('HDG', time)
+
+    def hdm(self, time: Optional[float] = None):
+        return self.get_value('HDM', time)
+
+    def throttle(self, time: Optional[float] = None):
+        return self.get_value('Throttle', time)
+
+    def throttle2(self, time: Optional[float] = None):
+        return self.get_value('Throttle2', time)
+
+    def engine_rpm(self, time: Optional[float] = None):
+        return self.get_value('EngineRPM', time)
+
+    def engine_rpm2(self, time: Optional[float] = None):
+        return self.get_value('EngineRPM2', time)
+
+    def after_burner(self, time: Optional[float] = None):
+        return self.get_value('AfterBurner', time)
+
+    # AirBrakes：对象的空气刹车状态。用于标识对象空气刹车的状态。例如，F-16飞机的空气刹车状态为“关闭”。
+    def air_brakes(self, time: Optional[float] = None):
+        return self.get_value('AirBrakes', time)
+
+    # Flaps：对象的襟翼状态。用于标识对象襟翼的状态。例如，F-16飞机的襟翼状态为“放下”。
+    def flaps(self, time: Optional[float] = None):
+        return self.get_value('Flaps', time)
+
+    # LandingGear：对象的起落架状态。用于标识对象起落架的状态。例如，F-16飞机的起落架状态为“收起”。
+    def landing_gear(self, time: Optional[float] = None):
+        return self.get_value('LandingGear', time)
+
+    # 起落架手柄位置
+    def landing_gear_handle(self, time: Optional[float] = None):
+        return self.get_value('LandingGearHandle', time)
+
+    # 阻拦钩状态
+    def tail_hook(self, time: Optional[float] = None):
+        return self.get_value('TailHook', time)
+
+    # 降落伞状态（与拖曳伞不要混淆）
+    def para_chute(self, time: Optional[float] = None):
+        return self.get_value('ParaChute', time)
+
+    def drag_chute(self, time: Optional[float] = None):
+        return self.get_value('DragChute', time)
+
+    def json(self, time: Optional[float] = None):
+        json_data = {
+            'ID'     : self.id,
+            'Name'   : self.name,
+            'Tags'   : self.tags,
+            'Type'   : self.type,
+            'Country': self.country,
         }
 
+        for field in self.data:
+            json_data[field] = self.get_value(field, time=time)
+        return json_data
+
     def __str__(self):
         return json.dumps(self.json(), ensure_ascii=False, indent=2)
 
-    # class Frame:
-
-
-#     def __init__(self, time):
-#         self.time = time
-#         self.objects = { }
 
 class AcmiFileReader:
     """Stream reading class that correctly line escaped acmi files."""
 
     def __init__(self, fh):
         self.fh = fh
 
@@ -350,16 +614,18 @@
         self.briefing = None
         self.debriefing = None
         self.comments = None
         self.reference_longitude = 0
         self.reference_latitude = 0
 
         self.objects: dict[str, AcmiObject] = { }
-        self.timeframes = []
+        self.timeframes: list[float] = []
         # 加载
+        # 解析到的object_keys
+        self.object_fields = { 'ID', 'Name', 'Type', 'Tags' }
 
         self._parse(filepath=filepath)
 
     @staticmethod
     def parse_obj_id(val: str) -> str:
         # return int(val, 16)
         return val
@@ -423,67 +689,80 @@
 
         obj = self.objects[obj_id]
         for field in fields[1:]:
             (prop, val) = field.split('=', 1)
 
             if prop == "T":
                 pos_list = val.split('|')
-                if pos_list:
-                    if pos_list[0]:
-                        obj.set_value("Longitude", timeframe, self.reference_longitude + float(pos_list[0]))
-                    if pos_list[1]:
-                        obj.set_value("Latitude", timeframe, self.reference_latitude + float(pos_list[1]))
-                    if pos_list[2]:
-                        obj.set_value("Altitude", timeframe, float(pos_list[2]))
-
-                    if len(pos_list) == 5:
-                        if pos_list[3]:
-                            obj.set_value("x", timeframe, float(pos_list[3]))
-                        if pos_list[4]:
-                            obj.set_value("y", timeframe, float(pos_list[4]))
-                    if len(pos_list) == 6:
-                        if pos_list[3]:
-                            obj.set_value("Roll", timeframe, float(pos_list[3]))
-                        if pos_list[4]:
-                            obj.set_value("Pitch", timeframe, float(pos_list[4]))
-                        if pos_list[5]:
-                            obj.set_value("Yaw", timeframe, float(pos_list[5]))
-                    if len(pos_list) == 9:
-                        if pos_list[3]:
-                            obj.set_value("Roll", timeframe, float(pos_list[3]))
-                        if pos_list[4]:
-                            obj.set_value("Pitch", timeframe, float(pos_list[4]))
-                        if pos_list[5]:
-                            obj.set_value("Yaw", timeframe, float(pos_list[5]))
-                        if pos_list[6]:
-                            obj.set_value("x", timeframe, float(pos_list[6]))
-                        if pos_list[7]:
-                            obj.set_value("y", timeframe, float(pos_list[7]))
-                        if pos_list[8]:
-                            obj.set_value("Heading", timeframe, float(pos_list[8]))
+                if not pos_list:
+                    continue
+                if pos_list[0]:
+                    obj.set_value("Longitude", timeframe, self.reference_longitude + float(pos_list[0]))
+                    self.object_fields.add('Longitude')
+                if pos_list[1]:
+                    obj.set_value("Latitude", timeframe, self.reference_latitude + float(pos_list[1]))
+                    self.object_fields.add('Latitude')
+                if pos_list[2]:
+                    obj.set_value("Altitude", timeframe, float(pos_list[2]))
+                    self.object_fields.add('Altitude')
+
+                if len(pos_list) == 5:
+                    if pos_list[3]:
+                        obj.set_value("U", timeframe, float(pos_list[3]))
+                        self.object_fields.add('U')
+                    if pos_list[4]:
+                        obj.set_value("V", timeframe, float(pos_list[4]))
+                        self.object_fields.add('V')
+                if len(pos_list) == 6:
+                    if pos_list[3]:
+                        obj.set_value("Roll", timeframe, float(pos_list[3]))
+                        self.object_fields.add('Roll')
+                    if pos_list[4]:
+                        obj.set_value("Pitch", timeframe, float(pos_list[4]))
+                        self.object_fields.add('Pitch')
+                    if pos_list[5]:
+                        obj.set_value("Yaw", timeframe, float(pos_list[5]))
+                        self.object_fields.add('Yaw')
+                if len(pos_list) == 9:
+                    if pos_list[3]:
+                        obj.set_value("Roll", timeframe, float(pos_list[3]))
+                        self.object_fields.add('Roll')
+                    if pos_list[4]:
+                        obj.set_value("Pitch", timeframe, float(pos_list[4]))
+                        self.object_fields.add('Pitch')
+                    if pos_list[5]:
+                        obj.set_value("Yaw", timeframe, float(pos_list[5]))
+                        self.object_fields.add('Yaw')
+                    if pos_list[6]:
+                        obj.set_value("U", timeframe, float(pos_list[6]))
+                        self.object_fields.add('U')
+                    if pos_list[7]:
+                        obj.set_value("V", timeframe, float(pos_list[7]))
+                        self.object_fields.add('V')
+                    if pos_list[8]:
+                        obj.set_value("Heading", timeframe, float(pos_list[8]))
+                        self.object_fields.add('Heading')
 
+                continue
             elif prop == "Name":
                 obj.set_value(prop, timeframe, val)
-            elif prop == "Parent" or prop == "FocusTarget" or prop == "LockedTarget":
+            elif prop == "Parent" or prop == "FocusTarget" or prop.startswith('LockedTarget'):
                 obj.set_value(prop, timeframe, self.parse_obj_id(val))
             elif prop == "Type":
                 obj.set_value(prop, timeframe, val)
-            elif prop in _STR_OBJECT_KEYS:
+            elif prop in ACMI_TEXT_PROPERTIES:
                 obj.set_value(prop, timeframe, val)
-            # numeric except coordinates start here
-            # floats
-            elif prop in _FLOAT_OBJECT_KEYS:
+            elif prop in ACMI_NUMERIC_PROPERTIES:
                 obj.set_value(prop, timeframe, float(val))
-            # int
-            elif prop in _INT_OBJECT_KEYS:
-                obj.set_value(prop, timeframe, int(val))
             else:
                 obj.set_value(prop, timeframe, val)
                 print("Unknown property:", prop)
 
+            self.object_fields.add(prop)
+
     def _parse(self, filepath: str):
 
         def do_parse(f):
             ar = AcmiFileReader(f)
             rawline = next(ar)
             if rawline.startswith('FileType='):
                 self.file_type = rawline[len('FileType='):].strip()
@@ -530,29 +809,29 @@
         if zipfile.is_zipfile(filepath):
             with zipfile.ZipFile(file=filepath) as my_zip:
                 # 打印zip文件中的文件列表
 
                 # 读取zip文件中的一个文件
                 for name in my_zip.namelist():
                     with my_zip.open(name) as f:
-                        do_parse(io.TextIOWrapper(f, encoding=_ACMI_FILE_ENCODING))
+                        do_parse(io.TextIOWrapper(f, encoding=ACMI_FILE_ENCODING))
         else:
-            with open(filepath, 'r', encoding=_ACMI_FILE_ENCODING) as f:
+            with open(filepath, 'r', encoding=ACMI_FILE_ENCODING) as f:
                 do_parse(f)
 
     def object_ids(self):
         return self.objects.keys()
 
     def alive_objects(self):
         return [self.objects[obj_key] for obj_key in self.objects if self.objects[obj_key].removed_at is None]
 
     def removed_objects(self):
         return [self.objects[objkey] for objkey in self.objects if self.objects[objkey].removed_at is not None]
 
-    def json(self):
+    def global_json(self):
         return {
             "FileType"          : self.file_type,
             "FileVersion"       : self.file_version,
             "DataSource"        : self.data_source,
             "DataRecorder"      : self.data_recorder,
             "ReferenceTime"     : self.reference_time.isoformat(),
             "RecordingTime"     : self.recording_time.isoformat(),
@@ -565,13 +844,67 @@
             "ReferenceLongitude": self.reference_longitude,
             "ReferenceLatitude" : self.reference_latitude,
             "Objects"           : len(self.objects),
             "TimeFrames"        : len(self.timeframes),
         }
 
     def __str__(self):
-        return json.dumps(obj=self.json(), indent=2, ensure_ascii=False)
+        return json.dumps(obj=self.global_json(), indent=2, ensure_ascii=False)
 
-    def export(self, export_filepath: str):
-        with open(export_filepath, 'w', encoding='utf-8') as f:
-            data = { "Global": self.json(), "Objects": [self.objects[k].json() for k in self.objects] }
-            json.dump(data, f, ensure_ascii=False, indent=2)
+    # def export_global_to_json(self, export_filepath: str):
+    #     with open(export_filepath, 'w', encoding='utf-8') as f:
+    #         json.dump(self.global_json(), f, ensure_ascii=False)
+
+    # 导出CSV
+    # remove_empty: 是否移除空列，默认移除
+    # export_obj_ids: 选择导出的object ID
+    def export_csv(self, filepath: str, remove_empty=True, export_obj_ids: Optional[list[str]] = None):
+        # 如果目录不存在，则创建目录
+        dirname = os.path.dirname(filepath)
+        if dirname and not os.path.exists(dirname):
+            os.makedirs(dirname)
+        
+        headers = []
+        if remove_empty:
+            for field in ACMI_EXPORT_CSV_HEADERS:
+                if field == 'ReferenceTime':
+                    if not self.reference_time:
+                        continue
+                elif field == 'Category':
+                    if not self.category:
+                        continue
+                elif field == 'Time' or field == 'ID' or field == 'Name':
+                    headers.append(field)
+                    continue
+                else:
+                    if field not in self.object_fields:
+                        continue
+                headers.append(field)
+        else:
+            headers = ACMI_EXPORT_CSV_HEADERS
+        with open(filepath, 'w', newline='') as f:
+            writer = csv.writer(f)
+            # 写入表头
+            writer.writerow(headers)
+            lines = []
+            for t in tqdm(self.timeframes, desc=f'Exporting {self.title} to {filepath}'):
+                for obj_id in self.objects:
+                    if export_obj_ids is not None and obj_id not in export_obj_ids:
+                        continue
+
+                    obj = self.objects[obj_id]
+                    line = []
+
+                    for field in headers:
+                        if field == 'ReferenceTime':
+                            line.append(self.reference_time)
+                        elif field == 'Category':
+                            line.append(self.category)
+                        elif field == 'Time':
+                            line.append(t)
+                        else:
+                            line.append(obj.get_value(field=field, time=t))
+                    lines.append(line)
+                    if len(lines) > 1000:
+                        writer.writerows(lines)
+                        lines = []
+            writer.writerows(lines)
```

### Comparing `pyacmi-1.1.1/pyacmi.egg-info/PKG-INFO` & `pyacmi-1.2.0/pyacmi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.1.1
+Version: 1.2.0
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
@@ -23,29 +23,53 @@
 [![License](https://img.shields.io/pypi/l/pyacmi.svg)](https://github.com/wangtong2015/pyacmi)
 [![Package Status](https://img.shields.io/pypi/status/pyacmi.svg)](https://pypi.org/project/pyacmi/)
 
 `**.acmi` is a file used by tacview for creating flight recording from simulators or real world.
 
 The source code is currently hosted on GitHub at: https://github.com/wangtong2015/pyacmi
 
-## Install
+ACMI file Introduction:  [Tacview - ACMI flight recordings.md](Tacview - ACMI flight recordings.md)
+
+## Installation
+
+You can install pyacmi via pip or pip3 for Python 3+:
+
+```shell
+$ pip3 install pyacmi
+```
+
+You can install a specific version of pyacmi by:
 
 ```shell
+$ pip3 install pyacmi==1.1.0
+```
 
-pip install pyacmi
+You can upgrade pyacmi to the latest version by:
 
+```shell
+$ pip3 install --upgrade pyacmi
 ```
 
 ## Example
 
 ```python
 
-from pyacmi import *
+from pyacmi import Acmi
 
 acmi = Acmi('test.acmi')
 print(acmi)
 
+print(acmi.reference_latitude, acmi.reference_longitude, acmi.reference_time)
+
+# 打印所有的object
+for obj_id in acmi.objects:
+    obj = acmi.objects[obj_id]
+    print(obj)
+    print(obj.id, obj.name, obj.country, obj.tags, obj.type)
+
+# 导出成csv
+acmi.export_csv('test.csv', remove_empty=True, export_obj_ids=None)
 ```
 
 ## Credits
 
 - [https://github.com/rp-/acmi](https://github.com/rp-/acmi)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyacmi-1.1.1/setup.py` & `pyacmi-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
         name="pyacmi",
-        version='1.1.1',
+        version='1.2.0',
         description="ACMI flight record file parser",
         long_description=long_description,
         long_description_content_type='text/markdown',
         url='https://github.com/wangtong2015/pyacmi',
         author="Wang Tong",
         author_email="astroboythu@gmail.com",
         license="MIT",
@@ -19,10 +19,10 @@
             'Intended Audience :: Developers',
             'Intended Audience :: End Users/Desktop',
             'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
             'Programming Language :: Python :: 3.4',
             'Programming Language :: Python :: 3 :: Only'
         ],
         keywords='acmi tacview',
-        install_requires=['sortedcontainers'],
+        install_requires=['sortedcontainers', 'tqdm'],
         packages=['pyacmi'],
 )
```

