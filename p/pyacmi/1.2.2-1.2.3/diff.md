# Comparing `tmp/pyacmi-1.2.2.tar.gz` & `tmp/pyacmi-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacmi-1.2.2.tar", last modified: Tue May  9 20:10:57 2023, max compression
+gzip compressed data, was "pyacmi-1.2.3.tar", last modified: Tue May  9 20:15:18 2023, max compression
```

## Comparing `pyacmi-1.2.2.tar` & `pyacmi-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:10:57.880019 pyacmi-1.2.2/
--rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 16:16:44.000000 pyacmi-1.2.2/LICENSE
--rw-r--r--   0 wangtong   (501) staff       (20)     2104 2023-05-09 20:10:57.879865 pyacmi-1.2.2/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)     1426 2023-05-09 20:00:51.000000 pyacmi-1.2.2/README.md
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:10:57.878868 pyacmi-1.2.2/pyacmi/
--rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 16:19:56.000000 pyacmi-1.2.2/pyacmi/__init__.py
--rw-r--r--   0 wangtong   (501) staff       (20)    36271 2023-05-09 20:09:06.000000 pyacmi-1.2.2/pyacmi/acmi.py
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:10:57.879672 pyacmi-1.2.2/pyacmi.egg-info/
--rw-r--r--   0 wangtong   (501) staff       (20)     2104 2023-05-09 20:10:57.000000 pyacmi-1.2.2/pyacmi.egg-info/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-09 20:10:57.000000 pyacmi-1.2.2/pyacmi.egg-info/SOURCES.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-09 20:10:57.000000 pyacmi-1.2.2/pyacmi.egg-info/dependency_links.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       22 2023-05-09 20:10:57.000000 pyacmi-1.2.2/pyacmi.egg-info/requires.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-09 20:10:57.000000 pyacmi-1.2.2/pyacmi.egg-info/top_level.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-09 20:10:57.880071 pyacmi-1.2.2/setup.cfg
--rw-r--r--   0 wangtong   (501) staff       (20)     1030 2023-05-09 20:10:41.000000 pyacmi-1.2.2/setup.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:15:18.780234 pyacmi-1.2.3/
+-rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 16:16:44.000000 pyacmi-1.2.3/LICENSE
+-rw-r--r--   0 wangtong   (501) staff       (20)     2104 2023-05-09 20:15:18.780085 pyacmi-1.2.3/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)     1426 2023-05-09 20:14:47.000000 pyacmi-1.2.3/README.md
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:15:18.779183 pyacmi-1.2.3/pyacmi/
+-rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 16:19:56.000000 pyacmi-1.2.3/pyacmi/__init__.py
+-rw-r--r--   0 wangtong   (501) staff       (20)    36480 2023-05-09 20:13:50.000000 pyacmi-1.2.3/pyacmi/acmi.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:15:18.779895 pyacmi-1.2.3/pyacmi.egg-info/
+-rw-r--r--   0 wangtong   (501) staff       (20)     2104 2023-05-09 20:15:18.000000 pyacmi-1.2.3/pyacmi.egg-info/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-09 20:15:18.000000 pyacmi-1.2.3/pyacmi.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-09 20:15:18.000000 pyacmi-1.2.3/pyacmi.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       22 2023-05-09 20:15:18.000000 pyacmi-1.2.3/pyacmi.egg-info/requires.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-09 20:15:18.000000 pyacmi-1.2.3/pyacmi.egg-info/top_level.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-09 20:15:18.780282 pyacmi-1.2.3/setup.cfg
+-rw-r--r--   0 wangtong   (501) staff       (20)     1030 2023-05-09 20:15:17.000000 pyacmi-1.2.3/setup.py
```

### Comparing `pyacmi-1.2.2/LICENSE` & `pyacmi-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacmi-1.2.2/PKG-INFO` & `pyacmi-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.2.2
+Version: 1.2.3
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
@@ -36,15 +36,15 @@
 ```shell
 $ pip3 install pyacmi
 ```
 
 You can install a specific version of pyacmi by:
 
 ```shell
-$ pip3 install pyacmi==1.2.0
+$ pip3 install pyacmi==1.2.3
 ```
 
 You can upgrade pyacmi to the latest version by:
 
 ```shell
 $ pip3 install --upgrade pyacmi
 ```
```

### Comparing `pyacmi-1.2.2/README.md` & `pyacmi-1.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```shell
 $ pip3 install pyacmi
 ```
 
 You can install a specific version of pyacmi by:
 
 ```shell
-$ pip3 install pyacmi==1.2.0
+$ pip3 install pyacmi==1.2.3
 ```
 
 You can upgrade pyacmi to the latest version by:
 
 ```shell
 $ pip3 install --upgrade pyacmi
 ```
```

### Comparing `pyacmi-1.2.2/pyacmi/acmi.py` & `pyacmi-1.2.3/pyacmi/acmi.py`

 * *Files 2% similar despite different names*

```diff
@@ -594,62 +594,62 @@
 
         return line
 
 
 class Acmi:
 
     def __init__(self, filepath: str):
-        self.filepath = filepath
-        self.file_version = None
-        self.file_type = None
+        self.filepath: Optional[str] = filepath
+        self.file_version: Optional[str] = None
+        self.file_type: Optional[str] = None
 
         # global properties
-        self.data_source = None
-        self.data_recorder = None
-        self.reference_time = None
-        self.recording_time = None
-        self.author = None
-        self.title = None
+        self.data_source: Optional[str] = None
+        self.data_recorder: Optional[str] = None
+        self.reference_time: Optional[str] = None
+        self.recording_time: Optional[str] = None
+        self.author: Optional[str] = None
+        self.title: Optional[str] = None
 
         # Category of the flight/mission:
         # - Air - to - Air：空中对空战斗任务
         # - Air - to - Ground：空中对地攻击任务
         # - Reconnaissance：侦察或侦察任务
         # - Close air support：提供地面部队近距离空中支援
         # - Maritime：海上巡逻和攻击任务
         # - Training：用于教学或练习的任务
         # - Other：其他任务类型，根据实际情况而定。
-        self.category = None
+        self.category: Optional[str] = None
 
-        self.briefing = None
-        self.debriefing = None
-        self.comments = None
+        self.briefing: Optional[str] = None
+        self.debriefing: Optional[str] = None
+        self.comments: Optional[str] = None
         self.reference_longitude = 0
         self.reference_latitude = 0
 
         self.objects: dict[str, AcmiObject] = { }
         self.timeframes: list[float] = []
         # 加载
         # 解析到的object_keys
-        self.object_fields = { 'ID', 'Name', 'Type', 'Tags' }
+        self.object_fields: set[str] = { 'ID', 'Name', 'Type', 'Tags' }
 
         self._parse(filepath=filepath)
 
     @staticmethod
     def parse_obj_id(val: str) -> str:
         # return int(val, 16)
         return val
 
     @staticmethod
     def strptime(val: str):
         if len(val) < 22:
             return datetime.datetime.strptime(val, "%Y-%m-%dT%H:%M:%SZ")
         else:
             return datetime.datetime.strptime(val, "%Y-%m-%dT%H:%M:%S.%fZ")
-
+    
     @staticmethod
     def split_fields(line):
         fields = []
         i = 1
         lastfield = 0
         while i < len(line):
             if line[i - 1] != '\\' and line[i] == ',':
```

### Comparing `pyacmi-1.2.2/pyacmi.egg-info/PKG-INFO` & `pyacmi-1.2.3/pyacmi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.2.2
+Version: 1.2.3
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
@@ -36,15 +36,15 @@
 ```shell
 $ pip3 install pyacmi
 ```
 
 You can install a specific version of pyacmi by:
 
 ```shell
-$ pip3 install pyacmi==1.2.0
+$ pip3 install pyacmi==1.2.3
 ```
 
 You can upgrade pyacmi to the latest version by:
 
 ```shell
 $ pip3 install --upgrade pyacmi
 ```
```

### Comparing `pyacmi-1.2.2/setup.py` & `pyacmi-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
         name="pyacmi",
-        version='1.2.2',
+        version='1.2.3',
         description="ACMI flight record file parser",
         long_description=long_description,
         long_description_content_type='text/markdown',
         url='https://github.com/wangtong2015/pyacmi',
         author="Wang Tong",
         author_email="astroboythu@gmail.com",
         license="MIT",
```

