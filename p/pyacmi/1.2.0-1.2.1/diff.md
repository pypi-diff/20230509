# Comparing `tmp/pyacmi-1.2.0.tar.gz` & `tmp/pyacmi-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacmi-1.2.0.tar", last modified: Tue May  9 19:49:12 2023, max compression
+gzip compressed data, was "pyacmi-1.2.1.tar", last modified: Tue May  9 20:02:23 2023, max compression
```

## Comparing `pyacmi-1.2.0.tar` & `pyacmi-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 19:49:12.191181 pyacmi-1.2.0/
--rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 16:16:44.000000 pyacmi-1.2.0/LICENSE
--rw-r--r--   0 wangtong   (501) staff       (20)     2083 2023-05-09 19:49:12.191053 pyacmi-1.2.0/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)     1405 2023-05-09 19:47:49.000000 pyacmi-1.2.0/README.md
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 19:49:12.189774 pyacmi-1.2.0/pyacmi/
--rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 16:19:56.000000 pyacmi-1.2.0/pyacmi/__init__.py
--rw-r--r--   0 wangtong   (501) staff       (20)    35803 2023-05-09 19:47:21.000000 pyacmi-1.2.0/pyacmi/acmi.py
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 19:49:12.190857 pyacmi-1.2.0/pyacmi.egg-info/
--rw-r--r--   0 wangtong   (501) staff       (20)     2083 2023-05-09 19:49:12.000000 pyacmi-1.2.0/pyacmi.egg-info/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-09 19:49:12.000000 pyacmi-1.2.0/pyacmi.egg-info/SOURCES.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-09 19:49:12.000000 pyacmi-1.2.0/pyacmi.egg-info/dependency_links.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       22 2023-05-09 19:49:12.000000 pyacmi-1.2.0/pyacmi.egg-info/requires.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-09 19:49:12.000000 pyacmi-1.2.0/pyacmi.egg-info/top_level.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-09 19:49:12.191332 pyacmi-1.2.0/setup.cfg
--rw-r--r--   0 wangtong   (501) staff       (20)     1030 2023-05-09 19:48:33.000000 pyacmi-1.2.0/setup.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:02:23.435384 pyacmi-1.2.1/
+-rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 16:16:44.000000 pyacmi-1.2.1/LICENSE
+-rw-r--r--   0 wangtong   (501) staff       (20)     2104 2023-05-09 20:02:23.435260 pyacmi-1.2.1/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)     1426 2023-05-09 20:00:51.000000 pyacmi-1.2.1/README.md
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:02:23.434367 pyacmi-1.2.1/pyacmi/
+-rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 16:19:56.000000 pyacmi-1.2.1/pyacmi/__init__.py
+-rw-r--r--   0 wangtong   (501) staff       (20)    35828 2023-05-09 20:01:42.000000 pyacmi-1.2.1/pyacmi/acmi.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 20:02:23.435079 pyacmi-1.2.1/pyacmi.egg-info/
+-rw-r--r--   0 wangtong   (501) staff       (20)     2104 2023-05-09 20:02:23.000000 pyacmi-1.2.1/pyacmi.egg-info/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-09 20:02:23.000000 pyacmi-1.2.1/pyacmi.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-09 20:02:23.000000 pyacmi-1.2.1/pyacmi.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       22 2023-05-09 20:02:23.000000 pyacmi-1.2.1/pyacmi.egg-info/requires.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-09 20:02:23.000000 pyacmi-1.2.1/pyacmi.egg-info/top_level.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-09 20:02:23.435428 pyacmi-1.2.1/setup.cfg
+-rw-r--r--   0 wangtong   (501) staff       (20)     1030 2023-05-09 20:02:16.000000 pyacmi-1.2.1/setup.py
```

### Comparing `pyacmi-1.2.0/LICENSE` & `pyacmi-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacmi-1.2.0/PKG-INFO` & `pyacmi-1.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.2.0
+Version: 1.2.1
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
@@ -23,28 +23,28 @@
 [![License](https://img.shields.io/pypi/l/pyacmi.svg)](https://github.com/wangtong2015/pyacmi)
 [![Package Status](https://img.shields.io/pypi/status/pyacmi.svg)](https://pypi.org/project/pyacmi/)
 
 `**.acmi` is a file used by tacview for creating flight recording from simulators or real world.
 
 The source code is currently hosted on GitHub at: https://github.com/wangtong2015/pyacmi
 
-ACMI file Introduction:  [Tacview - ACMI flight recordings.md](Tacview - ACMI flight recordings.md)
+ACMI file documentation: [Technical Reference - ACMI flight recordings 2.2](https://www.tacview.net/documentation/acmi/)
 
 ## Installation
 
 You can install pyacmi via pip or pip3 for Python 3+:
 
 ```shell
 $ pip3 install pyacmi
 ```
 
 You can install a specific version of pyacmi by:
 
 ```shell
-$ pip3 install pyacmi==1.1.0
+$ pip3 install pyacmi==1.2.0
 ```
 
 You can upgrade pyacmi to the latest version by:
 
 ```shell
 $ pip3 install --upgrade pyacmi
 ```
```

### Comparing `pyacmi-1.2.0/README.md` & `pyacmi-1.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 [![License](https://img.shields.io/pypi/l/pyacmi.svg)](https://github.com/wangtong2015/pyacmi)
 [![Package Status](https://img.shields.io/pypi/status/pyacmi.svg)](https://pypi.org/project/pyacmi/)
 
 `**.acmi` is a file used by tacview for creating flight recording from simulators or real world.
 
 The source code is currently hosted on GitHub at: https://github.com/wangtong2015/pyacmi
 
-ACMI file Introduction:  [Tacview - ACMI flight recordings.md](Tacview - ACMI flight recordings.md)
+ACMI file documentation: [Technical Reference - ACMI flight recordings 2.2](https://www.tacview.net/documentation/acmi/)
 
 ## Installation
 
 You can install pyacmi via pip or pip3 for Python 3+:
 
 ```shell
 $ pip3 install pyacmi
 ```
 
 You can install a specific version of pyacmi by:
 
 ```shell
-$ pip3 install pyacmi==1.1.0
+$ pip3 install pyacmi==1.2.0
 ```
 
 You can upgrade pyacmi to the latest version by:
 
 ```shell
 $ pip3 install --upgrade pyacmi
 ```
```

### Comparing `pyacmi-1.2.0/pyacmi/acmi.py` & `pyacmi-1.2.1/pyacmi/acmi.py`

 * *Files 0% similar despite different names*

```diff
@@ -852,15 +852,15 @@
 
     # def export_global_to_json(self, export_filepath: str):
     #     with open(export_filepath, 'w', encoding='utf-8') as f:
     #         json.dump(self.global_json(), f, ensure_ascii=False)
 
     # 导出CSV
     # remove_empty: 是否移除空列，默认移除
-    # export_obj_ids: 选择导出的object ID
+    # export_obj_ids: 选择导出的object ID None表示导出全部ID
     def export_csv(self, filepath: str, remove_empty=True, export_obj_ids: Optional[list[str]] = None):
         # 如果目录不存在，则创建目录
         dirname = os.path.dirname(filepath)
         if dirname and not os.path.exists(dirname):
             os.makedirs(dirname)
         
         headers = []
```

### Comparing `pyacmi-1.2.0/pyacmi.egg-info/PKG-INFO` & `pyacmi-1.2.1/pyacmi.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.2.0
+Version: 1.2.1
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
@@ -23,28 +23,28 @@
 [![License](https://img.shields.io/pypi/l/pyacmi.svg)](https://github.com/wangtong2015/pyacmi)
 [![Package Status](https://img.shields.io/pypi/status/pyacmi.svg)](https://pypi.org/project/pyacmi/)
 
 `**.acmi` is a file used by tacview for creating flight recording from simulators or real world.
 
 The source code is currently hosted on GitHub at: https://github.com/wangtong2015/pyacmi
 
-ACMI file Introduction:  [Tacview - ACMI flight recordings.md](Tacview - ACMI flight recordings.md)
+ACMI file documentation: [Technical Reference - ACMI flight recordings 2.2](https://www.tacview.net/documentation/acmi/)
 
 ## Installation
 
 You can install pyacmi via pip or pip3 for Python 3+:
 
 ```shell
 $ pip3 install pyacmi
 ```
 
 You can install a specific version of pyacmi by:
 
 ```shell
-$ pip3 install pyacmi==1.1.0
+$ pip3 install pyacmi==1.2.0
 ```
 
 You can upgrade pyacmi to the latest version by:
 
 ```shell
 $ pip3 install --upgrade pyacmi
 ```
```

### Comparing `pyacmi-1.2.0/setup.py` & `pyacmi-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
         name="pyacmi",
-        version='1.2.0',
+        version='1.2.1',
         description="ACMI flight record file parser",
         long_description=long_description,
         long_description_content_type='text/markdown',
         url='https://github.com/wangtong2015/pyacmi',
         author="Wang Tong",
         author_email="astroboythu@gmail.com",
         license="MIT",
```

