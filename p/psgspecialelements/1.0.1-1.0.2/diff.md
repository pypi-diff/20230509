# Comparing `tmp/psgspecialelements-1.0.1.tar.gz` & `tmp/psgspecialelements-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psgspecialelements-1.0.1.tar", last modified: Mon May  8 23:57:44 2023, max compression
+gzip compressed data, was "psgspecialelements-1.0.2.tar", last modified: Tue May  9 00:22:01 2023, max compression
```

## Comparing `psgspecialelements-1.0.1.tar` & `psgspecialelements-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 23:57:44.534062 psgspecialelements-1.0.1/
--rw-rw-rw-   0        0        0      253 2023-05-08 23:57:44.533061 psgspecialelements-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1525 2023-04-21 00:40:07.000000 psgspecialelements-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 23:57:44.514057 psgspecialelements-1.0.1/config/
-drwxrwxrwx   0        0        0        0 2023-05-08 23:57:44.524060 psgspecialelements-1.0.1/config/img/
--rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 psgspecialelements-1.0.1/config/img/table_arrow9_transparent_64.ico
--rw-rw-rw-   0        0        0    34392 2023-04-06 03:13:05.000000 psgspecialelements-1.0.1/hash_password.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:57:44.532061 psgspecialelements-1.0.1/psgspecialelements.egg-info/
--rw-rw-rw-   0        0        0      253 2023-05-08 23:57:44.000000 psgspecialelements-1.0.1/psgspecialelements.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-05-08 23:57:44.000000 psgspecialelements-1.0.1/psgspecialelements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 23:57:44.000000 psgspecialelements-1.0.1/psgspecialelements.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-08 23:57:44.000000 psgspecialelements-1.0.1/psgspecialelements.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-05-08 23:57:44.000000 psgspecialelements-1.0.1/psgspecialelements.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   239432 2023-04-08 01:44:09.000000 psgspecialelements-1.0.1/psgspecialelements.py
--rw-rw-rw-   0        0        0       42 2023-05-08 23:57:44.534062 psgspecialelements-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2658 2023-05-08 23:56:39.000000 psgspecialelements-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 00:22:01.375002 psgspecialelements-1.0.2/
+-rw-rw-rw-   0        0        0      253 2023-05-09 00:22:01.374002 psgspecialelements-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1525 2023-04-21 00:40:07.000000 psgspecialelements-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 00:22:01.355998 psgspecialelements-1.0.2/config/
+drwxrwxrwx   0        0        0        0 2023-05-09 00:22:01.365000 psgspecialelements-1.0.2/config/img/
+-rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 psgspecialelements-1.0.2/config/img/table_arrow9_transparent_64.ico
+-rw-rw-rw-   0        0        0    34392 2023-04-06 03:13:05.000000 psgspecialelements-1.0.2/hash_password.py
+drwxrwxrwx   0        0        0        0 2023-05-09 00:22:01.373002 psgspecialelements-1.0.2/psgspecialelements.egg-info/
+-rw-rw-rw-   0        0        0      253 2023-05-09 00:22:01.000000 psgspecialelements-1.0.2/psgspecialelements.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-05-09 00:22:01.000000 psgspecialelements-1.0.2/psgspecialelements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 00:22:01.000000 psgspecialelements-1.0.2/psgspecialelements.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-09 00:22:01.000000 psgspecialelements-1.0.2/psgspecialelements.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-05-09 00:22:01.000000 psgspecialelements-1.0.2/psgspecialelements.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   239432 2023-04-08 01:44:09.000000 psgspecialelements-1.0.2/psgspecialelements.py
+-rw-rw-rw-   0        0        0       42 2023-05-09 00:22:01.375002 psgspecialelements-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2658 2023-05-09 00:21:36.000000 psgspecialelements-1.0.2/setup.py
```

### Comparing `psgspecialelements-1.0.1/README.md` & `psgspecialelements-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `psgspecialelements-1.0.1/config/img/table_arrow9_transparent_64.ico` & `psgspecialelements-1.0.2/config/img/table_arrow9_transparent_64.ico`

 * *Files identical despite different names*

### Comparing `psgspecialelements-1.0.1/hash_password.py` & `psgspecialelements-1.0.2/hash_password.py`

 * *Files identical despite different names*

### Comparing `psgspecialelements-1.0.1/psgspecialelements.py` & `psgspecialelements-1.0.2/psgspecialelements.py`

 * *Files identical despite different names*

### Comparing `psgspecialelements-1.0.1/setup.py` & `psgspecialelements-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='psgspecialelements',
-    version='1.0.1',
+    version='1.0.2',
     description='special elements based on pysimplegui elements',
     author='Frank Gong',
     author_email='583983716@qq.com',
     packages=find_packages(),        # 表示你要封装的包，find_packages用于系统自动从当前目录开始找包
     license="MIT",
     py_modules=['psgspecialelements', 'hash_password'],
     install_requires=['PySimpleGUI', 'pandas~=1.5.2', 'numpy~=1.24.1', 'openpyxl', 'dataclasses', 'pycryptodomex'],
```

