# Comparing `tmp/pyacmi-1.0.2.tar.gz` & `tmp/pyacmi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacmi-1.0.2.tar", last modified: Mon May  8 16:14:16 2023, max compression
+gzip compressed data, was "pyacmi-1.1.0.tar", last modified: Tue May  9 08:14:56 2023, max compression
```

## Comparing `pyacmi-1.0.2.tar` & `pyacmi-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 16:14:16.938254 pyacmi-1.0.2/
--rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 10:54:45.000000 pyacmi-1.0.2/LICENSE
--rw-r--r--   0 wangtong   (501) staff       (20)     1407 2023-05-08 16:14:16.938110 pyacmi-1.0.2/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      729 2023-05-08 16:11:33.000000 pyacmi-1.0.2/README.md
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 16:14:16.934492 pyacmi-1.0.2/pyacmi/
--rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 09:42:33.000000 pyacmi-1.0.2/pyacmi/__init__.py
--rw-r--r--   0 wangtong   (501) staff       (20)    17604 2023-05-08 10:59:36.000000 pyacmi-1.0.2/pyacmi/acmi.py
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-08 16:14:16.937109 pyacmi-1.0.2/pyacmi.egg-info/
--rw-r--r--   0 wangtong   (501) staff       (20)     1407 2023-05-08 16:14:16.000000 pyacmi-1.0.2/pyacmi.egg-info/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-08 16:14:16.000000 pyacmi-1.0.2/pyacmi.egg-info/SOURCES.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-08 16:14:16.000000 pyacmi-1.0.2/pyacmi.egg-info/dependency_links.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       17 2023-05-08 16:14:16.000000 pyacmi-1.0.2/pyacmi.egg-info/requires.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-08 16:14:16.000000 pyacmi-1.0.2/pyacmi.egg-info/top_level.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-08 16:14:16.938743 pyacmi-1.0.2/setup.cfg
--rw-r--r--   0 wangtong   (501) staff       (20)     1022 2023-05-08 16:12:09.000000 pyacmi-1.0.2/setup.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 08:14:56.762560 pyacmi-1.1.0/
+-rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 16:16:44.000000 pyacmi-1.1.0/LICENSE
+-rw-r--r--   0 wangtong   (501) staff       (20)     1407 2023-05-09 08:14:56.762422 pyacmi-1.1.0/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)      729 2023-05-08 16:16:44.000000 pyacmi-1.1.0/README.md
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 08:14:56.761552 pyacmi-1.1.0/pyacmi/
+-rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 16:19:56.000000 pyacmi-1.1.0/pyacmi/__init__.py
+-rw-r--r--   0 wangtong   (501) staff       (20)    23245 2023-05-09 08:14:22.000000 pyacmi-1.1.0/pyacmi/acmi.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 08:14:56.762235 pyacmi-1.1.0/pyacmi.egg-info/
+-rw-r--r--   0 wangtong   (501) staff       (20)     1407 2023-05-09 08:14:56.000000 pyacmi-1.1.0/pyacmi.egg-info/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-09 08:14:56.000000 pyacmi-1.1.0/pyacmi.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-09 08:14:56.000000 pyacmi-1.1.0/pyacmi.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       17 2023-05-09 08:14:56.000000 pyacmi-1.1.0/pyacmi.egg-info/requires.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-09 08:14:56.000000 pyacmi-1.1.0/pyacmi.egg-info/top_level.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-09 08:14:56.762627 pyacmi-1.1.0/setup.cfg
+-rw-r--r--   0 wangtong   (501) staff       (20)     1022 2023-05-09 08:14:33.000000 pyacmi-1.1.0/setup.py
```

### Comparing `pyacmi-1.0.2/LICENSE` & `pyacmi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacmi-1.0.2/PKG-INFO` & `pyacmi-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.0.2
+Version: 1.1.0
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyacmi-1.0.2/README.md` & `pyacmi-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyacmi-1.0.2/pyacmi/acmi.py` & `pyacmi-1.1.0/pyacmi/acmi.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,184 @@
 import zipfile
 import datetime
 import sortedcontainers
 import bisect
+import json
+import io
+from constantly import ValueConstant
 
-ACMI_FILE_ENCODING = 'utf-8-sig'
-FLOAT_OBJECT_KEYS = {
+_ACMI_FILE_ENCODING = 'utf-8-sig'
+_FLOAT_OBJECT_KEYS = {
     "Importance", "Length", "Width", "Height",
     "IAS", "CAS", "TAS", "Mach", "AOA", "HDG",
     "HDM", "Throttle", "RadarAzimuth", "RadarElevation",
     "RadarRange", "LockedTargetAzimuth",
     "LockedTargetElevation", "LockedTargetRange", "Flaps", "LandingGear",
     "AirBrakes",
     "PilotHeadRoll", "PilotHeadPitch", "PilotHeadYaw",
     "RollControlPosition", "PitchControlPosition", "YawControlPosition" }
-INT_OBJECT_KEYS = { "Slot", "Afterburner", "Tailhook",
-                    "Parachute", "DragChute", "RadarMode",
-                    "LockedTargetMode" }
-STR_OBJECT_KEYS = { "Pilot", "Group", "Country", "Coalition",
-                    "Color", "Registration", "Squawk", "Debug", "Label" }
+_INT_OBJECT_KEYS = { "Slot", "Afterburner", "Tailhook",
+                     "Parachute", "DragChute", "RadarMode",
+                     "LockedTargetMode" }
+_STR_OBJECT_KEYS = { "Pilot", "Group", "Country", "Coalition",
+                     "Color", "Registration", "Squawk", "Debug", "Label" }
+
+
+class AcmiType(ValueConstant):
+    Plane = 'Plane'
+    Helicopter = 'Helicopter'
+    AntiAircraft = 'AntiAircraft'
+    Armor = 'Armor'
+    Tank = 'Tank'
+    GroundVehicle = 'GroundVehicle'
+    Watercraft = 'Watercraft'
+    Warship = 'Warship'
+    AircraftCarrier = 'AircraftCarrier'
+    Submarine = 'Submarine'
+    Sonobuoy = 'Sonobuoy'
+    Human = 'Human'
+    Infantry = 'Infantry'
+    Parachutist = 'Parachutist'
+    Missile = 'Missile'
+    Rocket = 'Rocket'
+    Bomb = 'Bomb'
+    Projectile = 'Projectile'
+    Beam = 'Beam'
+    Shell = 'Shell'
+    Bullet = 'Bullet'
+    BallisticShell = 'BallisticShell'
+    Grenade = 'Grenade'
+    Decoy = 'Decoy'
+    Flare = 'Flare'
+    Chaff = 'Chaff'
+    SmokeGrenade = 'SmokeGrenade'
+    Building = 'Building'
+    Aerodrome = 'Aerodrome'
+    Bullseye = 'Bullseye'
+    Waypoint = 'Waypoint'
+    Container = 'Container'
+    Shrapnel = 'Shrapnel'
+    MinorObject = 'MinorObject'
+    Explosion = 'Explosion'
+    F16C = 'F16C'
+    Bicycle = 'Bicycle'
+    AIM120C = 'AIM-120C'
+
+
+ACMI_TYPE_TAGS = {
+    AcmiType.Plane          : ['Air+FixedWing'],
+    AcmiType.Helicopter     : ['Air+Rotorcraft'],
+    AcmiType.AntiAircraft   : ['Ground+AntiAircraft'],
+    AcmiType.Armor          : ['Ground+Heavy+Armor+Vehicle'],
+    AcmiType.Tank           : ['Ground+Heavy+Armor+Vehicle+Tank'],
+    AcmiType.GroundVehicle  : ['Ground+Vehicle'],
+    AcmiType.Watercraft     : ['Sea+Watercraft'],
+    AcmiType.Warship        : ['Sea+Watercraft+Warship'],
+    AcmiType.AircraftCarrier: ['Sea+Watercraft+AircraftCarrier', 'Heavy+Sea+Watercraft+AircraftCarrier'],
+    AcmiType.Submarine      : ['Sea+Watercraft+Submarine'],
+    AcmiType.Sonobuoy       : ['Sea+Sensor'],
+    AcmiType.Human          : ['Ground+Light+Human'],
+    AcmiType.Infantry       : ['Ground+Light+Human+Infantry'],
+    AcmiType.Parachutist    : ['Ground+Light+Human+Air+Parachutist'],
+    AcmiType.Missile        : ['Weapon+Missile'],
+    AcmiType.Rocket         : ['Weapon+Rocket'],
+    AcmiType.Bomb           : ['Weapon+Bomb'],
+    AcmiType.Projectile     : ['Weapon+Projectile'],
+    AcmiType.Beam           : ['Weapon+Beam'],
+    AcmiType.Shell          : ['Projectile+Shell'],
+    AcmiType.Bullet         : ['Projectile+Bullet'],
+    AcmiType.BallisticShell : ['Projectile+Shell+Heavy'],
+    AcmiType.Grenade        : ['Projectile+Grenade'],
+    AcmiType.Decoy          : ['Misc+Decoy'],
+    AcmiType.Flare          : ['Misc+Decoy+Flare'],
+    AcmiType.Chaff          : ['Misc+Decoy+Chaff'],
+    AcmiType.SmokeGrenade   : ['Misc+Decoy+SmokeGrenade'],
+    AcmiType.Building       : ['Ground+Static+Building'],
+    AcmiType.Aerodrome      : ['Ground+Static+Aerodrome'],
+    AcmiType.Bullseye       : ['Navaid+Static+Bullseye'],
+    AcmiType.Waypoint       : ['Navaid+Static+Waypoint'],
+    AcmiType.Container      : ['Misc+Container'],
+    AcmiType.Shrapnel       : ['Misc+Shrapnel'],
+    AcmiType.MinorObject    : ['Misc+Minor'],
+    AcmiType.Explosion      : ['Misc+Explosion'],
+    AcmiType.F16C           : ['Medium+Air+FixedWing'],
+    AcmiType.Bicycle        : ['Light+Ground+Vehicle'],
+    AcmiType.AIM120C        : ['Medium+Weapon+Missile'],
+}
+
+# 将_ACMI_TYPE_TAGS预处理（内部按照顺序排序，方便后续匹配）
+for k in ACMI_TYPE_TAGS:
+    tags = ACMI_TYPE_TAGS[k]
+    ACMI_TYPE_TAGS[k] = ['+'.join(sorted(tag.split('+'))) for tag in tags]
 
 
 class AcmiObject:
 
     def __init__(self, obj_id: str):
         self.id = obj_id
         self.removed_at = None
 
         self.data = { }
 
+        self.tags = ''
+        self.type = ''  # 多个类型用+连接
+
+        # 对象的名称。用于标识该对象。例如，F-16飞机的名称为“Viper”。
+        self.name = None
+        # Country：对象所属的国家。用于标识对象所属的国家。例如，F-16飞机所属的国家为“美国”。
+        self.country = None
+
+    # 飞机
+    @property
+    def is_plane(self):
+        return AcmiType.Plane in self.type
+
+    # 导弹，是一种可以自行控制运动轨迹、并击中目标的武器。
+    @property
+    def is_missile(self):
+        return AcmiType.Missile in self.type
+
+    # 箭状烟雾弹，是一种烟雾弹的类型，可以用于干扰敌方导弹、火箭炮或飞机系统。
+    @property
+    def is_flare(self):
+        return AcmiType.Flare in self.type
+
+    # 箔条干扰弹，是一种用于干扰雷达信号的武器，通常由一些金属箔条组成。
+    @property
+    def is_chaff(self):
+        return AcmiType.Chaff in self.type
+
+    # 弹片，是爆炸物体爆炸时产生的金属碎片和碎片。
+    @property
+    def is_shrapnel(self):
+        return AcmiType.Shrapnel in self.type
+
+    # 牛眼: 空战中心点的位置，用来方便飞行员报告目标位置和距离
+    @property
+    def is_bullseye(self):
+        return AcmiType.Bullseye in self.type
+
     def set_value(self, field, timeframe, val):
+        if field == 'Type':
+            match_tags = '+'.join(sorted(val.split('+')))
+            match_types = []
+            self.tags = val
+            if not self.type:
+                for _type in ACMI_TYPE_TAGS:
+                    if match_tags in ACMI_TYPE_TAGS[_type]:
+                        match_types.append(_type)
+                self.type = '+'.join(match_types)
+            return
+        elif field == 'Name':
+            self.name = val
+            return
+        elif field == 'Country':
+            self.country = val
+            return
+
         if field not in self.data:
             self.data[field] = sortedcontainers.SortedDict()
         self.data[field][timeframe] = val
 
     # 该类的get_value函数用于获取指定场景下（field）的数据值。
     # 如果指定了timeframe参数，
     #   如果timeframe存在，则返回对应时间点的值或
@@ -52,26 +198,14 @@
             pos = bisect.bisect_left(timeframe_keys, timeframe)
             if pos == 0:
                 return data[timeframe_keys[0]]
             else:
                 return data[timeframe_keys[pos - 1]]
         return data[timeframe_keys[-1]]
 
-    # Name：对象的名称。用于标识该对象。例如，F-16飞机的名称为“Viper”。
-    def name(self, time=None):
-        return self.get_value("Name", time)
-
-    # Type：对象的类型。用于区分不同类型的对象。例如，F-16飞机的类型为“战斗机”。
-    def type(self, time=None):
-        return self.get_value("Type", time)
-
-    # Country：对象所属的国家。用于标识对象所属的国家。例如，F-16飞机所属的国家为“美国”。
-    def country(self, time=None):
-        return self.get_value("Country", time)
-
     # Latitude：对象的纬度。用于标识对象所在的位置。例如，F-16飞机的纬度为“32.1234”。
     def latitude(self, time=None):
         return self.get_value("Latitude", time)
 
     # Longitude：对象的经度。用于标识对象所在的位置。例如，F-16飞机的经度为“-117.2345”。
     def longitude(self, time=None):
         return self.get_value("Longitude", time)
@@ -136,20 +270,21 @@
     def pilot_head_roll(self, time=None):
         return self.get_value("PilotHeadRoll", time)
 
     # PilotHeadYaw：驾驶员的头部偏航角。用于标识驾驶员的头部偏航角度。例如，驾驶员的头部偏航角为“20”。
     def pilot_head_yaw(self, time=None):
         return self.get_value("PilotHeadYaw", time)
 
-    def __str__(self):
+    def json(self):
         return {
             'ID'                  : self.id,
-            'Name'                : self.name(),
-            'Type'                : self.type(),
-            'Country'             : self.country(),
+            'Name'                : self.name,
+            'Tags'                : self.tags,
+            'Type'                : self.type,
+            'Country'             : self.country,
             'Latitude'            : self.latitude(),
             'Longitude'           : self.longitude(),
             'Altitude'            : self.altitude(),
             'Heading'             : self.heading(),
             'Pitch'               : self.pitch(),
             'Roll'                : self.roll(),
             'IAS'                 : self.ias(),
@@ -162,16 +297,20 @@
             'Yaw'                 : self.yaw(),
             'Pilot'               : self.pilot(),
             'PilotHeadPitch'      : self.pilot_head_pitch(),
             'PilotHeadRoll'       : self.pilot_head_roll(),
             'PilotHeadYaw'        : self.pilot_head_yaw()
         }
 
+    def __str__(self):
+        return json.dumps(self.json(), ensure_ascii=False, indent=2)
+
+    # class Frame:
+
 
-# class Frame:
 #     def __init__(self, time):
 #         self.time = time
 #         self.objects = { }
 
 class AcmiFileReader:
     """Stream reading class that correctly line escaped acmi files."""
 
@@ -184,15 +323,15 @@
     def __next__(self):
         line = self.fh.readline()
         # line = rl.decode(AcmiFileReader._codec)
         if len(line) == 0:
             raise StopIteration
 
         while line.strip().endswith('\\'):
-            line = line.strip()[:-1] + '\n' + self.fh.readline().decode(ACMI_FILE_ENCODING)
+            line = line.strip()[:-1] + '\n' + self.fh.readline().decode(_ACMI_FILE_ENCODING)
 
         return line
 
 
 class Acmi:
 
     def __init__(self, filepath: str):
@@ -210,15 +349,15 @@
         self.category = None
         self.briefing = None
         self.debriefing = None
         self.comments = None
         self.reference_longitude = 0
         self.reference_latitude = 0
 
-        self.objects = { }
+        self.objects: dict[str, AcmiObject] = { }
         self.timeframes = []
         # 加载
 
         self._parse(filepath=filepath)
 
     @staticmethod
     def parse_obj_id(val: str) -> str:
@@ -323,32 +462,31 @@
                             obj.set_value("Heading", timeframe, float(pos_list[8]))
 
             elif prop == "Name":
                 obj.set_value(prop, timeframe, val)
             elif prop == "Parent" or prop == "FocusTarget" or prop == "LockedTarget":
                 obj.set_value(prop, timeframe, self.parse_obj_id(val))
             elif prop == "Type":
-                obj.set_value(prop, timeframe, val.split("+"))
-            elif prop in STR_OBJECT_KEYS:
+                obj.set_value(prop, timeframe, val)
+            elif prop in _STR_OBJECT_KEYS:
                 obj.set_value(prop, timeframe, val)
             # numeric except coordinates start here
             # floats
-            elif prop in FLOAT_OBJECT_KEYS:
+            elif prop in _FLOAT_OBJECT_KEYS:
                 obj.set_value(prop, timeframe, float(val))
             # int
-            elif prop in INT_OBJECT_KEYS:
+            elif prop in _INT_OBJECT_KEYS:
                 obj.set_value(prop, timeframe, int(val))
             else:
+                obj.set_value(prop, timeframe, val)
                 print("Unknown property:", prop)
 
     def _parse(self, filepath: str):
-        if zipfile.is_zipfile(filepath):
-            raise RuntimeError("这是一个zip文件，请先将其解压（如果后缀是acmi，将acmi改成zip即可）: " + filepath)
 
-        with open(filepath, 'r', encoding=ACMI_FILE_ENCODING) as f:
+        def do_parse(f):
             ar = AcmiFileReader(f)
             rawline = next(ar)
             if rawline.startswith('FileType='):
                 self.file_type = rawline[len('FileType='):].strip()
             else:
                 raise RuntimeError("ACMI file doesn't start with FileType.")
 
@@ -382,37 +520,58 @@
 
                     # print(obj_id, fields)
                     if obj_id == '0' or obj_id == 0:
                         self._parse_global_property(fields)
                     else:
                         self._parse_object_property(obj_id, cur_reftime, fields)
 
+        # if zipfile.is_zipfile(filepath):
+        #     raise RuntimeError("这是一个zip文件，请先将其解压（如果后缀是acmi，将acmi改成zip即可）: " + filepath)
+        # 打开zip文件
+        if zipfile.is_zipfile(filepath):
+            with zipfile.ZipFile(file=filepath) as my_zip:
+                # 打印zip文件中的文件列表
+
+                # 读取zip文件中的一个文件
+                for name in my_zip.namelist():
+                    with my_zip.open(name) as f:
+                        do_parse(io.TextIOWrapper(f, encoding=_ACMI_FILE_ENCODING))
+        else:
+            with open(filepath, 'r', encoding=_ACMI_FILE_ENCODING) as f:
+                do_parse(f)
+
     def object_ids(self):
         return self.objects.keys()
 
     def alive_objects(self):
         return [self.objects[obj_key] for obj_key in self.objects if self.objects[obj_key].removed_at is None]
 
     def removed_objects(self):
         return [self.objects[objkey] for objkey in self.objects if self.objects[objkey].removed_at is not None]
 
+    def json(self):
+        return {
+            "FileType"          : self.file_type,
+            "FileVersion"       : self.file_version,
+            "DataSource"        : self.data_source,
+            "DataRecorder"      : self.data_recorder,
+            "ReferenceTime"     : self.reference_time.isoformat(),
+            "RecordingTime"     : self.recording_time.isoformat(),
+            "Author"            : self.author,
+            "Title"             : self.title,
+            "Category"          : self.category,
+            "Briefing"          : self.briefing,
+            "Debriefing"        : self.debriefing,
+            "Comments"          : self.comments,
+            "ReferenceLongitude": self.reference_longitude,
+            "ReferenceLatitude" : self.reference_latitude,
+            "Objects"           : len(self.objects),
+            "TimeFrames"        : len(self.timeframes),
+        }
+
     def __str__(self):
-        return str(
-                {
-                    "FileType"          : self.file_type,
-                    "FileVersion"       : self.file_version,
-                    "DataSource"        : self.data_source,
-                    "DataRecorder"      : self.data_recorder,
-                    "ReferenceTime"     : self.reference_time.isoformat(),
-                    "RecordingTime"     : self.recording_time.isoformat(),
-                    "Author"            : self.author,
-                    "Title"             : self.title,
-                    "Category"          : self.category,
-                    "Briefing"          : self.briefing,
-                    "Debriefing"        : self.debriefing,
-                    "Comments"          : self.comments,
-                    "ReferenceLongitude": self.reference_longitude,
-                    "ReferenceLatitude" : self.reference_latitude,
-                    "Objects"           : len(self.objects),
-                    "TimeFrames"        : len(self.timeframes),
-                }
-        )
+        return json.dumps(obj=self.json(), indent=2, ensure_ascii=False)
+
+    def export(self, export_filepath: str):
+        with open(export_filepath, 'w', encoding='utf-8') as f:
+            data = { "Global": self.json(), "Objects": [self.objects[k].json() for k in self.objects] }
+            json.dump(data, f, ensure_ascii=False, indent=2)
```

### Comparing `pyacmi-1.0.2/pyacmi.egg-info/PKG-INFO` & `pyacmi-1.1.0/pyacmi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.0.2
+Version: 1.1.0
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyacmi-1.0.2/setup.py` & `pyacmi-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
         name="pyacmi",
-        version='1.0.2',
+        version='1.1.0',
         description="ACMI flight record file parser",
         long_description=long_description,
         long_description_content_type='text/markdown',
         url='https://github.com/wangtong2015/pyacmi',
         author="Wang Tong",
         author_email="astroboythu@gmail.com",
         license="MIT",
```

