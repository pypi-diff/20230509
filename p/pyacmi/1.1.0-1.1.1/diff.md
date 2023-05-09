# Comparing `tmp/pyacmi-1.1.0.tar.gz` & `tmp/pyacmi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacmi-1.1.0.tar", last modified: Tue May  9 08:14:56 2023, max compression
+gzip compressed data, was "pyacmi-1.1.1.tar", last modified: Tue May  9 08:41:35 2023, max compression
```

## Comparing `pyacmi-1.1.0.tar` & `pyacmi-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 08:14:56.762560 pyacmi-1.1.0/
--rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 16:16:44.000000 pyacmi-1.1.0/LICENSE
--rw-r--r--   0 wangtong   (501) staff       (20)     1407 2023-05-09 08:14:56.762422 pyacmi-1.1.0/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      729 2023-05-08 16:16:44.000000 pyacmi-1.1.0/README.md
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 08:14:56.761552 pyacmi-1.1.0/pyacmi/
--rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 16:19:56.000000 pyacmi-1.1.0/pyacmi/__init__.py
--rw-r--r--   0 wangtong   (501) staff       (20)    23245 2023-05-09 08:14:22.000000 pyacmi-1.1.0/pyacmi/acmi.py
-drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 08:14:56.762235 pyacmi-1.1.0/pyacmi.egg-info/
--rw-r--r--   0 wangtong   (501) staff       (20)     1407 2023-05-09 08:14:56.000000 pyacmi-1.1.0/pyacmi.egg-info/PKG-INFO
--rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-09 08:14:56.000000 pyacmi-1.1.0/pyacmi.egg-info/SOURCES.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-09 08:14:56.000000 pyacmi-1.1.0/pyacmi.egg-info/dependency_links.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       17 2023-05-09 08:14:56.000000 pyacmi-1.1.0/pyacmi.egg-info/requires.txt
--rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-09 08:14:56.000000 pyacmi-1.1.0/pyacmi.egg-info/top_level.txt
--rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-09 08:14:56.762627 pyacmi-1.1.0/setup.cfg
--rw-r--r--   0 wangtong   (501) staff       (20)     1022 2023-05-09 08:14:33.000000 pyacmi-1.1.0/setup.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 08:41:35.404556 pyacmi-1.1.1/
+-rw-r--r--   0 wangtong   (501) staff       (20)    11357 2023-05-08 16:16:44.000000 pyacmi-1.1.1/LICENSE
+-rw-r--r--   0 wangtong   (501) staff       (20)     1407 2023-05-09 08:41:35.404441 pyacmi-1.1.1/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)      729 2023-05-08 16:16:44.000000 pyacmi-1.1.1/README.md
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 08:41:35.403650 pyacmi-1.1.1/pyacmi/
+-rw-r--r--   0 wangtong   (501) staff       (20)       20 2023-05-08 16:19:56.000000 pyacmi-1.1.1/pyacmi/__init__.py
+-rw-r--r--   0 wangtong   (501) staff       (20)    23217 2023-05-09 08:40:58.000000 pyacmi-1.1.1/pyacmi/acmi.py
+drwxr-xr-x   0 wangtong   (501) staff       (20)        0 2023-05-09 08:41:35.404265 pyacmi-1.1.1/pyacmi.egg-info/
+-rw-r--r--   0 wangtong   (501) staff       (20)     1407 2023-05-09 08:41:35.000000 pyacmi-1.1.1/pyacmi.egg-info/PKG-INFO
+-rw-r--r--   0 wangtong   (501) staff       (20)      209 2023-05-09 08:41:35.000000 pyacmi-1.1.1/pyacmi.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        1 2023-05-09 08:41:35.000000 pyacmi-1.1.1/pyacmi.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       17 2023-05-09 08:41:35.000000 pyacmi-1.1.1/pyacmi.egg-info/requires.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)        7 2023-05-09 08:41:35.000000 pyacmi-1.1.1/pyacmi.egg-info/top_level.txt
+-rw-r--r--   0 wangtong   (501) staff       (20)       38 2023-05-09 08:41:35.404599 pyacmi-1.1.1/setup.cfg
+-rw-r--r--   0 wangtong   (501) staff       (20)     1022 2023-05-09 08:41:31.000000 pyacmi-1.1.1/setup.py
```

### Comparing `pyacmi-1.1.0/LICENSE` & `pyacmi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacmi-1.1.0/PKG-INFO` & `pyacmi-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.1.0
+Version: 1.1.1
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyacmi-1.1.0/README.md` & `pyacmi-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyacmi-1.1.0/pyacmi/acmi.py` & `pyacmi-1.1.1/pyacmi/acmi.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,15 +323,15 @@
     def __next__(self):
         line = self.fh.readline()
         # line = rl.decode(AcmiFileReader._codec)
         if len(line) == 0:
             raise StopIteration
 
         while line.strip().endswith('\\'):
-            line = line.strip()[:-1] + '\n' + self.fh.readline().decode(_ACMI_FILE_ENCODING)
+            line = line.strip()[:-1] + '\n' + self.fh.readline()
 
         return line
 
 
 class Acmi:
 
     def __init__(self, filepath: str):
```

### Comparing `pyacmi-1.1.0/pyacmi.egg-info/PKG-INFO` & `pyacmi-1.1.1/pyacmi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacmi
-Version: 1.1.0
+Version: 1.1.1
 Summary: ACMI flight record file parser
 Home-page: https://github.com/wangtong2015/pyacmi
 Author: Wang Tong
 Author-email: astroboythu@gmail.com
 License: MIT
 Keywords: acmi tacview
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyacmi-1.1.0/setup.py` & `pyacmi-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
         name="pyacmi",
-        version='1.1.0',
+        version='1.1.1',
         description="ACMI flight record file parser",
         long_description=long_description,
         long_description_content_type='text/markdown',
         url='https://github.com/wangtong2015/pyacmi',
         author="Wang Tong",
         author_email="astroboythu@gmail.com",
         license="MIT",
```

