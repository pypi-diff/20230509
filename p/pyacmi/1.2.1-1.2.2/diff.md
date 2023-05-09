# Comparing `tmp/pyacmi-1.2.1.tar.gz` & `tmp/pyacmi-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacmi-1.2.1.tar", last modified: Tue May  9 20:02:23 2023, max compression
+gzip compressed data, was "pyacmi-1.2.2.tar", last modified: Tue May  9 20:10:57 2023, max compression
```

## Comparing `pyacmi-1.2.1.tar` & `pyacmi-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:02:23.435384 pyacmi-1.2.1/
--rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 16:16:44.000000 pyacmi-1.2.1/LICENSE
--rw-r--r--   0 wangtong   (501) staff       (20)     2104 2023-05-09 20:02:23.435260 pyacmi-1.2.1/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)     1426 2023-05-09 20:00:51.000000 pyacmi-1.2.1/README.md
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:02:23.434367 pyacmi-1.2.1/pyacmi/
--rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 16:19:56.000000 pyacmi-1.2.1/pyacmi/__init__.py
--rw-r--r--   0 wangtong   (501) staff       (20)    35828 2023-05-09 20:01:42.000000 pyacmi-1.2.1/pyacmi/acmi.py
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:02:23.435079 pyacmi-1.2.1/pyacmi.egg-info/
--rw-r--r--   0 wangtong   (501) staff       (20)     2104 2023-05-09 20:02:23.000000 pyacmi-1.2.1/pyacmi.egg-info/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-09 20:02:23.000000 pyacmi-1.2.1/pyacmi.egg-info/SOURCES.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-09 20:02:23.000000 pyacmi-1.2.1/pyacmi.egg-info/dependency_links.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       22 2023-05-09 20:02:23.000000 pyacmi-1.2.1/pyacmi.egg-info/requires.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-09 20:02:23.000000 pyacmi-1.2.1/pyacmi.egg-info/top_level.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-09 20:02:23.435428 pyacmi-1.2.1/setup.cfg
--rw-r--r--   0 wangtong   (501) staff       (20)     1030 2023-05-09 20:02:16.000000 pyacmi-1.2.1/setup.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:10:57.880019 pyacmi-1.2.2/
+-rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 16:16:44.000000 pyacmi-1.2.2/LICENSE
+-rw-r--r--   0 wangtong   (501) staff       (20)     2104 2023-05-09 20:10:57.879865 pyacmi-1.2.2/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)     1426 2023-05-09 20:00:51.000000 pyacmi-1.2.2/README.md
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:10:57.878868 pyacmi-1.2.2/pyacmi/
+-rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 16:19:56.000000 pyacmi-1.2.2/pyacmi/__init__.py
+-rw-r--r--   0 wangtong   (501) staff       (20)    36271 2023-05-09 20:09:06.000000 pyacmi-1.2.2/pyacmi/acmi.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:10:57.879672 pyacmi-1.2.2/pyacmi.egg-info/
+-rw-r--r--   0 wangtong   (501) staff       (20)     2104 2023-05-09 20:10:57.000000 pyacmi-1.2.2/pyacmi.egg-info/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-09 20:10:57.000000 pyacmi-1.2.2/pyacmi.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-09 20:10:57.000000 pyacmi-1.2.2/pyacmi.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       22 2023-05-09 20:10:57.000000 pyacmi-1.2.2/pyacmi.egg-info/requires.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-09 20:10:57.000000 pyacmi-1.2.2/pyacmi.egg-info/top_level.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-09 20:10:57.880071 pyacmi-1.2.2/setup.cfg
+-rw-r--r--   0 wangtong   (501) staff       (20)     1030 2023-05-09 20:10:41.000000 pyacmi-1.2.2/setup.py
```

### Comparing `pyacmi-1.2.1/LICENSE` & `pyacmi-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacmi-1.2.1/PKG-INFO` & `pyacmi-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.2.1
+Version: 1.2.2
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyacmi-1.2.1/README.md` & `pyacmi-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyacmi-1.2.1/pyacmi/acmi.py` & `pyacmi-1.2.2/pyacmi/acmi.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,14 @@
     'ReferenceTime',
     'Category',
     'ID',
     'Name'
     'Tags',
     'Type',
     'Time',
-
     'AdditionalType',
     'Parent',
     'Next',
     'ShortName',
     'LongName',
     'FullName',
     'CallSign',
@@ -606,15 +605,25 @@
         # global properties
         self.data_source = None
         self.data_recorder = None
         self.reference_time = None
         self.recording_time = None
         self.author = None
         self.title = None
+
+        # Category of the flight/mission:
+        # - Air - to - Air：空中对空战斗任务
+        # - Air - to - Ground：空中对地攻击任务
+        # - Reconnaissance：侦察或侦察任务
+        # - Close air support：提供地面部队近距离空中支援
+        # - Maritime：海上巡逻和攻击任务
+        # - Training：用于教学或练习的任务
+        # - Other：其他任务类型，根据实际情况而定。
         self.category = None
+
         self.briefing = None
         self.debriefing = None
         self.comments = None
         self.reference_longitude = 0
         self.reference_latitude = 0
 
         self.objects: dict[str, AcmiObject] = { }
@@ -858,15 +867,15 @@
     # remove_empty: 是否移除空列，默认移除
     # export_obj_ids: 选择导出的object ID None表示导出全部ID
     def export_csv(self, filepath: str, remove_empty=True, export_obj_ids: Optional[list[str]] = None):
         # 如果目录不存在，则创建目录
         dirname = os.path.dirname(filepath)
         if dirname and not os.path.exists(dirname):
             os.makedirs(dirname)
-        
+
         headers = []
         if remove_empty:
             for field in ACMI_EXPORT_CSV_HEADERS:
                 if field == 'ReferenceTime':
                     if not self.reference_time:
                         continue
                 elif field == 'Category':
```

### Comparing `pyacmi-1.2.1/pyacmi.egg-info/PKG-INFO` & `pyacmi-1.2.2/pyacmi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.2.1
+Version: 1.2.2
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyacmi-1.2.1/setup.py` & `pyacmi-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
         name="pyacmi",
-        version='1.2.1',
+        version='1.2.2',
         description="ACMI flight record file parser",
         long_description=long_description,
         long_description_content_type='text/markdown',
         url='https://github.com/wangtong2015/pyacmi',
         author="Wang Tong",
         author_email="astroboythu@gmail.com",
         license="MIT",
```

