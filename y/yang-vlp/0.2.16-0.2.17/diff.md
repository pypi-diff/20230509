# Comparing `tmp/yang-vlp-0.2.16.tar.gz` & `tmp/yang-vlp-0.2.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\yang-vlp0.2\dist\.tmp-_qcwp4vf\yang-vlp-0.2.16.tar", last modified: Sat May  6 06:41:29 2023, max compression
+gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\yang-vlp0.2\dist\.tmp-q1nh1uww\yang-vlp-0.2.17.tar", last modified: Tue May  9 02:37:00 2023, max compression
```

## Comparing `yang-vlp-0.2.16.tar` & `yang-vlp-0.2.17.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.508913 yang-vlp-0.2.16/
--rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 yang-vlp-0.2.16/LICENSE
--rw-rw-rw-   0        0        0      294 2023-04-18 03:27:59.000000 yang-vlp-0.2.16/MANIFEST.in
--rw-rw-rw-   0        0        0     2687 2023-05-06 06:41:29.507950 yang-vlp-0.2.16/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-04-27 01:00:56.000000 yang-vlp-0.2.16/README.md
--rw-rw-rw-   0        0        0      639 2023-05-06 06:39:43.000000 yang-vlp-0.2.16/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 06:41:29.509917 yang-vlp-0.2.16/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-05-06 06:39:38.000000 yang-vlp-0.2.16/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.332920 yang-vlp-0.2.16/vlppy/
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.334911 yang-vlp-0.2.16/vlppy/.vscode/
--rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 yang-vlp-0.2.16/vlppy/.vscode/settings.json
--rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 yang-vlp-0.2.16/vlppy/LICENSE.txt
--rw-rw-rw-   0        0        0      271 2023-04-18 03:27:13.000000 yang-vlp-0.2.16/vlppy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.349956 yang-vlp-0.2.16/vlppy/demo/
--rw-rw-rw-   0        0        0      348 2023-04-20 03:12:41.000000 yang-vlp-0.2.16/vlppy/demo/README.md
--rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 yang-vlp-0.2.16/vlppy/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.356913 yang-vlp-0.2.16/vlppy/demo/__pycache__/
--rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 yang-vlp-0.2.16/vlppy/demo/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 yang-vlp-0.2.16/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
--rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 yang-vlp-0.2.16/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
--rw-rw-rw-   0        0        0     1342 2023-04-27 10:40:52.000000 yang-vlp-0.2.16/vlppy/demo/demo_filter.py
--rw-rw-rw-   0        0        0     2607 2023-04-19 03:46:42.000000 yang-vlp-0.2.16/vlppy/demo/demo_main.py
--rw-rw-rw-   0        0        0     3188 2023-05-05 07:55:54.000000 yang-vlp-0.2.16/vlppy/demo/vlp_model.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.363916 yang-vlp-0.2.16/vlppy/error/
--rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 yang-vlp-0.2.16/vlppy/error/__init__.py
--rw-rw-rw-   0        0        0     1619 2023-04-20 05:53:48.000000 yang-vlp-0.2.16/vlppy/error/error.py
--rw-rw-rw-   0        0        0      108 2023-05-06 06:40:05.000000 yang-vlp-0.2.16/vlppy/info.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.369947 yang-vlp-0.2.16/vlppy/io/
--rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 yang-vlp-0.2.16/vlppy/io/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-04-20 06:14:59.000000 yang-vlp-0.2.16/vlppy/io/io.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.381941 yang-vlp-0.2.16/vlppy/model/
--rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 yang-vlp-0.2.16/vlppy/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.424914 yang-vlp-0.2.16/vlppy/model/__pycache__/
--rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 yang-vlp-0.2.16/vlppy/model/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 yang-vlp-0.2.16/vlppy/model/__pycache__/filter.cpython-39.pyc
--rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 yang-vlp-0.2.16/vlppy/model/__pycache__/led.cpython-39.pyc
--rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 yang-vlp-0.2.16/vlppy/model/__pycache__/pd.cpython-39.pyc
--rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 yang-vlp-0.2.16/vlppy/model/__pycache__/room.cpython-39.pyc
--rw-rw-rw-   0        0        0     6154 2023-05-05 07:26:43.000000 yang-vlp-0.2.16/vlppy/model/led.py
--rw-rw-rw-   0        0        0    17943 2023-05-05 10:56:03.000000 yang-vlp-0.2.16/vlppy/model/pd.py
--rw-rw-rw-   0        0        0    17682 2023-05-06 06:38:15.000000 yang-vlp-0.2.16/vlppy/model/room.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.435915 yang-vlp-0.2.16/vlppy/setting/
--rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 yang-vlp-0.2.16/vlppy/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.441914 yang-vlp-0.2.16/vlppy/setting/__pycache__/
--rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 yang-vlp-0.2.16/vlppy/setting/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 yang-vlp-0.2.16/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
--rw-rw-rw-   0        0        0     2903 2023-04-20 06:15:26.000000 yang-vlp-0.2.16/vlppy/setting/json_setting.py
--rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 yang-vlp-0.2.16/vlppy/setting/settings.json
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.453929 yang-vlp-0.2.16/vlppy/signal/
--rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 yang-vlp-0.2.16/vlppy/signal/__init__.py
--rw-rw-rw-   0        0        0    10010 2023-04-20 06:24:52.000000 yang-vlp-0.2.16/vlppy/signal/filter.py
--rw-rw-rw-   0        0        0     3719 2023-04-27 10:42:14.000000 yang-vlp-0.2.16/vlppy/signal/plot.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.485913 yang-vlp-0.2.16/vlppy/tools/
--rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 yang-vlp-0.2.16/vlppy/tools/__init__.py
--rw-rw-rw-   0        0        0      273 2023-04-18 03:22:02.000000 yang-vlp-0.2.16/vlppy/tools/decorator.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.489941 yang-vlp-0.2.16/vlppy/vis/
--rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 yang-vlp-0.2.16/vlppy/vis/__init__.py
--rw-rw-rw-   0        0        0     3653 2023-04-19 02:52:08.000000 yang-vlp-0.2.16/vlppy/vis/vis.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.505948 yang-vlp-0.2.16/yang_vlp.egg-info/
--rw-rw-rw-   0        0        0     2687 2023-05-06 06:41:29.000000 yang-vlp-0.2.16/yang_vlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1281 2023-05-06 06:41:29.000000 yang-vlp-0.2.16/yang_vlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 06:41:29.000000 yang-vlp-0.2.16/yang_vlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-06 06:41:29.000000 yang-vlp-0.2.16/yang_vlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-06 06:41:29.000000 yang-vlp-0.2.16/yang_vlp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.933731 yang-vlp-0.2.17/
+-rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 yang-vlp-0.2.17/LICENSE
+-rw-rw-rw-   0        0        0      294 2023-04-18 03:27:59.000000 yang-vlp-0.2.17/MANIFEST.in
+-rw-rw-rw-   0        0        0     2686 2023-05-09 02:37:00.930699 yang-vlp-0.2.17/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-06 06:53:58.000000 yang-vlp-0.2.17/README.md
+-rw-rw-rw-   0        0        0      639 2023-05-09 01:52:32.000000 yang-vlp-0.2.17/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 02:37:00.935730 yang-vlp-0.2.17/setup.cfg
+-rw-rw-rw-   0        0        0      932 2023-05-09 01:52:40.000000 yang-vlp-0.2.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.742200 yang-vlp-0.2.17/vlppy/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.744198 yang-vlp-0.2.17/vlppy/.vscode/
+-rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 yang-vlp-0.2.17/vlppy/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 yang-vlp-0.2.17/vlppy/LICENSE.txt
+-rw-rw-rw-   0        0        0      271 2023-04-18 03:27:13.000000 yang-vlp-0.2.17/vlppy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.760028 yang-vlp-0.2.17/vlppy/demo/
+-rw-rw-rw-   0        0        0      348 2023-04-20 03:12:41.000000 yang-vlp-0.2.17/vlppy/demo/README.md
+-rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 yang-vlp-0.2.17/vlppy/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.771040 yang-vlp-0.2.17/vlppy/demo/__pycache__/
+-rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 yang-vlp-0.2.17/vlppy/demo/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 yang-vlp-0.2.17/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 yang-vlp-0.2.17/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1342 2023-04-27 10:40:52.000000 yang-vlp-0.2.17/vlppy/demo/demo_filter.py
+-rw-rw-rw-   0        0        0     2607 2023-04-19 03:46:42.000000 yang-vlp-0.2.17/vlppy/demo/demo_main.py
+-rw-rw-rw-   0        0        0     3096 2023-05-09 01:51:31.000000 yang-vlp-0.2.17/vlppy/demo/vlp_model.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.776039 yang-vlp-0.2.17/vlppy/error/
+-rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 yang-vlp-0.2.17/vlppy/error/__init__.py
+-rw-rw-rw-   0        0        0     1619 2023-04-20 05:53:48.000000 yang-vlp-0.2.17/vlppy/error/error.py
+-rw-rw-rw-   0        0        0      108 2023-05-09 01:52:25.000000 yang-vlp-0.2.17/vlppy/info.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.780038 yang-vlp-0.2.17/vlppy/io/
+-rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 yang-vlp-0.2.17/vlppy/io/__init__.py
+-rw-rw-rw-   0        0        0     5346 2023-04-20 06:14:59.000000 yang-vlp-0.2.17/vlppy/io/io.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.793055 yang-vlp-0.2.17/vlppy/model/
+-rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 yang-vlp-0.2.17/vlppy/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.809053 yang-vlp-0.2.17/vlppy/model/__pycache__/
+-rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 yang-vlp-0.2.17/vlppy/model/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 yang-vlp-0.2.17/vlppy/model/__pycache__/filter.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 yang-vlp-0.2.17/vlppy/model/__pycache__/led.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 yang-vlp-0.2.17/vlppy/model/__pycache__/pd.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 yang-vlp-0.2.17/vlppy/model/__pycache__/room.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6177 2023-05-09 02:19:05.000000 yang-vlp-0.2.17/vlppy/model/led.py
+-rw-rw-rw-   0        0        0    17524 2023-05-09 02:36:28.000000 yang-vlp-0.2.17/vlppy/model/pd.py
+-rw-rw-rw-   0        0        0    17673 2023-05-06 06:55:51.000000 yang-vlp-0.2.17/vlppy/model/room.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.873685 yang-vlp-0.2.17/vlppy/setting/
+-rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 yang-vlp-0.2.17/vlppy/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.878700 yang-vlp-0.2.17/vlppy/setting/__pycache__/
+-rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 yang-vlp-0.2.17/vlppy/setting/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 yang-vlp-0.2.17/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2903 2023-04-20 06:15:26.000000 yang-vlp-0.2.17/vlppy/setting/json_setting.py
+-rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 yang-vlp-0.2.17/vlppy/setting/settings.json
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.896704 yang-vlp-0.2.17/vlppy/signal/
+-rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 yang-vlp-0.2.17/vlppy/signal/__init__.py
+-rw-rw-rw-   0        0        0    10010 2023-04-20 06:24:52.000000 yang-vlp-0.2.17/vlppy/signal/filter.py
+-rw-rw-rw-   0        0        0     3719 2023-04-27 10:42:14.000000 yang-vlp-0.2.17/vlppy/signal/plot.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.906697 yang-vlp-0.2.17/vlppy/tools/
+-rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 yang-vlp-0.2.17/vlppy/tools/__init__.py
+-rw-rw-rw-   0        0        0      273 2023-04-18 03:22:02.000000 yang-vlp-0.2.17/vlppy/tools/decorator.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.911731 yang-vlp-0.2.17/vlppy/vis/
+-rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 yang-vlp-0.2.17/vlppy/vis/__init__.py
+-rw-rw-rw-   0        0        0     3653 2023-04-19 02:52:08.000000 yang-vlp-0.2.17/vlppy/vis/vis.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:37:00.928696 yang-vlp-0.2.17/yang_vlp.egg-info/
+-rw-rw-rw-   0        0        0     2686 2023-05-09 02:37:00.000000 yang-vlp-0.2.17/yang_vlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2023-05-09 02:37:00.000000 yang-vlp-0.2.17/yang_vlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 02:37:00.000000 yang-vlp-0.2.17/yang_vlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-09 02:37:00.000000 yang-vlp-0.2.17/yang_vlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-09 02:37:00.000000 yang-vlp-0.2.17/yang_vlp.egg-info/top_level.txt
```

### Comparing `yang-vlp-0.2.16/LICENSE` & `yang-vlp-0.2.17/LICENSE`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/PKG-INFO` & `yang-vlp-0.2.17/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yang-vlp
-Version: 0.2.16
+Version: 0.2.17
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/yang_vlp
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,17 +31,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 @start date:  2022-08-26
 
-@auther:  yang wu ju
+@auther:  yangwuju
 
-@url: https://gitee.com/yangwuju/yang_vlp
+@url：https://gitee.com/yangwuju/yang_vlp
 
 @file:
 
 - model/room：房间、墙壁参数
 - model/led：led位置、发射的信号(None、DC、AC、AIM)
 - model/pd：pd 各种参数、LOS链路和NLOS链路接收LED信号、噪声
 - signal/filter：滤波器设计（包括fir,iir）
```

### Comparing `yang-vlp-0.2.16/README.md` & `yang-vlp-0.2.17/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 @start date:  2022-08-26
 
-@auther:  yang wu ju
+@auther:  yangwuju
 
-@url: https://gitee.com/yangwuju/yang_vlp
+@url：https://gitee.com/yangwuju/yang_vlp
 
 @file:
 
 - model/room：房间、墙壁参数
 - model/led：led位置、发射的信号(None、DC、AC、AIM)
 - model/pd：pd 各种参数、LOS链路和NLOS链路接收LED信号、噪声
 - signal/filter：滤波器设计（包括fir,iir）
```

### Comparing `yang-vlp-0.2.16/pyproject.toml` & `yang-vlp-0.2.17/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yang-vlp"
-version = "0.2.16"
+version = "0.2.17"
 authors = [
   { name="yangwuju", email="1424134319@qq.com" },
 ]
 description = "Construction of visible light positioning model"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.5"
```

### Comparing `yang-vlp-0.2.16/setup.py` & `yang-vlp-0.2.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 path = os.path.join(CUR_PATH, 'build')
 if os.path.isdir(path):
     print('INFO del dir ', path) 
     shutil.rmtree(path)
 
 setup(
     name = 'yang-vlp', #应用名
-    version = '0.2.16',  #版本号
+    version = '0.2.17',  #版本号
     description = 'Construction of visible light positioning model', 
     packages = find_packages(),  #包括在安装包内的Python包
     include_package_data = True, #启用清单文件MANIFEST.in,包含数据文件
     # exclude_package_data = {'docs':['1.txt']},  #排除文件
     install_requires = [#自动安装依赖
         'numpy>=1.19.0',
         'matplotlib>=3.5.0',
```

### Comparing `yang-vlp-0.2.16/vlppy/LICENSE.txt` & `yang-vlp-0.2.17/vlppy/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/demo/__pycache__/demo_main.cpython-39.pyc` & `yang-vlp-0.2.17/vlppy/demo/__pycache__/demo_main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc` & `yang-vlp-0.2.17/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/demo/demo_filter.py` & `yang-vlp-0.2.17/vlppy/demo/demo_filter.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/demo/demo_main.py` & `yang-vlp-0.2.17/vlppy/demo/demo_main.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/demo/vlp_model.py` & `yang-vlp-0.2.17/vlppy/demo/vlp_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,23 @@
         # PD
         pd = kwargs["PD_Info"] 
         pd1 = pd["PD1"]   
         pd2 = pd["PD2"]   
         pd3 = pd["PD3"]   
         pd4 = pd["PD4"]   
         
-        pd1_pos, (alpha1,beta1) = PD.recv_frame_model(l=pd["l"], alpha=pd1["alpha"], beta=pd1["beta"], center_tp_pos=self.room.tp_pos)  # PD位置和倾斜角
-        pd2_pos, (alpha2,beta2) = PD.recv_frame_model(l=pd["l"], alpha=pd2["alpha"], beta=pd2["beta"], center_tp_pos=self.room.tp_pos) 
-        pd3_pos, (alpha3,beta3) = PD.recv_frame_model(l=pd["l"], alpha=pd3["alpha"], beta=pd3["beta"], center_tp_pos=self.room.tp_pos)  
-        pd4_pos, (alpha4,beta4) = PD.recv_frame_model(l=pd["l"], alpha=pd4["alpha"], beta=pd4["beta"], center_tp_pos=self.room.tp_pos) 
+        pd1_pos, pd1_Nv = PD.recv_frame_model(l=pd["l"], alpha=pd1["alpha"], beta=pd1["beta"], center_tp_pos=self.room.tp_pos)  # PD位置和倾斜角
+        pd2_pos, pd2_Nv = PD.recv_frame_model(l=pd["l"], alpha=pd2["alpha"], beta=pd2["beta"], center_tp_pos=self.room.tp_pos) 
+        pd3_pos, pd3_Nv = PD.recv_frame_model(l=pd["l"], alpha=pd3["alpha"], beta=pd3["beta"], center_tp_pos=self.room.tp_pos)  
+        pd4_pos, pd4_Nv = PD.recv_frame_model(l=pd["l"], alpha=pd4["alpha"], beta=pd4["beta"], center_tp_pos=self.room.tp_pos) 
         
-        self.pd1 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd1_pos, alpha=alpha1, beta=beta1) 
-        self.pd2 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd2_pos, alpha=alpha2, beta=beta2)
-        self.pd3 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd3_pos, alpha=alpha3, beta=beta3) 
-        self.pd4 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd4_pos, alpha=alpha4, beta=beta4) 
+        self.pd1 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd1_pos, Nv=pd1_Nv) 
+        self.pd2 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd2_pos, Nv=pd2_Nv)
+        self.pd3 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd3_pos, Nv=pd3_Nv) 
+        self.pd4 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd4_pos, Nv=pd4_Nv) 
         
         # LED
         led = kwargs["LED_Info"] 
         fs = led['Fs']   # 采样率 
         npt = led['NPT'] # 采样点数 
         self.t = LED.get_time_series(fs=fs,npt=npt) # 以采样时间为间隔的时间序列
```

### Comparing `yang-vlp-0.2.16/vlppy/error/error.py` & `yang-vlp-0.2.17/vlppy/error/error.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/io/io.py` & `yang-vlp-0.2.17/vlppy/io/io.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/model/__pycache__/filter.cpython-39.pyc` & `yang-vlp-0.2.17/vlppy/model/__pycache__/filter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/model/__pycache__/led.cpython-39.pyc` & `yang-vlp-0.2.17/vlppy/model/__pycache__/led.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/model/__pycache__/pd.cpython-39.pyc` & `yang-vlp-0.2.17/vlppy/model/__pycache__/pd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/model/__pycache__/room.cpython-39.pyc` & `yang-vlp-0.2.17/vlppy/model/__pycache__/room.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/model/led.py` & `yang-vlp-0.2.17/vlppy/model/led.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,30 +141,32 @@
         """
         return self._pos + self.origin
     
     @pos.setter
     def pos(self, pos:tuple):
         """设置参考位置
         """
-        if not np.shape(pos)[-1] == 3:
-            raise VLPSequenceLenError(np.shape(pos)[-1],3)
+        pos = np.asarray(pos)
+        if not pos.shape[-1] == 3:
+            raise VLPSequenceLenError(pos.shape[-1],3)
         self._pos = np.asarray(pos)
         
     @property
     def Nv(self):  
-        """获取LED单位法向量  
+        """获取LED法向量  
         """  
-        return self._Nv/np.linalg.norm(self._Nv)
+        return self._Nv
 
     @Nv.setter
     def Nv(self, n): 
         """设置LED法向量 
         """
-        if not len(n) == 3:
-            raise VLPSequenceLenError(n, 3)
+        n = np.asarray(n)
+        if not n.shape[-1] == 3:
+            raise VLPSequenceLenError(n,3)
         self._Nv = n
 
     @property
     def theta(self):  
         """获取半功率点半角 (单位: 度)  
         """  
         return self._theta
```

### Comparing `yang-vlp-0.2.16/vlppy/model/pd.py` & `yang-vlp-0.2.17/vlppy/model/pd.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,79 +10,77 @@
     """
     def __init__(self,
                 n:Number=1.5,
                 fov:Number=60,
                 Ar:Number=1e-4,
                 Ts:Number=1,
                 pos:tuple=(0,0,0),
-                alpha:Number=0, 
-                beta:Number=0,
+                Nv:tuple=(0,0,1),
                 *args,
                 **kwargs) -> None:
         """ 
         n: 透镜的折射率
         fov: 接收视场角 (单位: 度) [0,90]
         Ar: PD检测器的接收面积(单位:平方米)
         Ts: 光学滤波器的增益
         pos: PD参考位置(注意:self._pos为参考位置,self.pos为相对位置) 
-        alpha: PD方位角(单位: 度) [0,360]
-        beta: PD倾斜角(单位: 度) [-90,90]
+        Nv: PD 法向量
         """
         self.n = n
         self.fov = fov
         self.Ar = Ar
         self.Ts = Ts
 
         self.pos = pos
+        self.Nv = Nv
         self.origin = (0,0,0) #原点位置
 
-        self.alpha = alpha
-        self.beta = beta
-
     @staticmethod
     def recv_frame_model(l, alpha, beta, center_tp_pos:tuple):
         """接收机模型:PD支架模型(倾斜PD和中心参考点位置关系)
         Params
             l: 倾斜PD到中心水平PD(参考点)的长度(单位:米)
-            alpha: PD倾斜面的方位角(单位:度)
+            alpha: PD摆放角(单位:度)
             beta: PD倾斜面倾斜角(单位:度)
             center_tp_pos: 水平中心测试点位置
         Return
             pos: 倾斜PD位置
-            (alpha,beta): 倾斜PD的方位角和倾斜角(单位:度)
+            Nv: 倾斜PD的法向量
         """
         x0, y0, z0 = np.split(center_tp_pos, indices_or_sections=3, axis=-1)
         x0, y0, z0 = x0.flatten(), y0.flatten(), z0.flatten()
 
         # 倾斜PD的方位角和倾斜角,角度制转弧度制
         alpha_rad, beta_rad = np.radians([alpha, beta])
 
         xr = x0 + l * np.cos(alpha_rad) * np.cos(beta_rad) 
         yr = y0 + l * np.sin(alpha_rad) * np.cos(beta_rad)
         zr = z0 + l * np.sin(beta_rad)
         pos = np.stack([xr,yr,zr], axis=-1) # 在最后一维度上堆叠
         
-        # PD的方位角和PD倾斜面的方位角反向
-        # PD的倾斜角和PD倾斜面的倾斜角相等
-        pd_alpha = alpha+180  
-        pd_alpha = pd_alpha-360 if pd_alpha > 360 else pd_alpha if pd_alpha >= 0 else pd_alpha+360 # 转到区间 [0,360)
-        
-        return pos, (alpha,beta)
+        # alpha_rad+np.pi: PD的方位角和PD倾斜面的摆放角反向
+        # beta_rad: PD的法向量与z轴的夹角和PD倾斜面的倾斜角相等
+        Nx = np.cos(alpha_rad+np.pi) * np.sin(beta_rad)
+        Ny = np.sin(alpha_rad+np.pi) * np.sin(beta_rad)
+        Nz = np.cos(beta_rad)
+        Nv = np.stack([Nx,Ny,Nz],axis=-1) 
+
+        return pos, Nv
 
     @staticmethod
     def recv_surface_model(r:Union[Number,tuple], alpha, beta, center_tp_pos:tuple):
         """接收机模型:安全帽椭球面(倾斜PD和中心参考点位置关系)
         Params
             r: 曲球面半径(单位:米)
-            alpha:倾斜PD方位角(单位:度)
-            beta:  倾斜PD倾斜角(单位:度)
+            alpha:PD摆放角(单位:度)
+            beta: PD倾斜面倾斜角(单位:度)
             center_tp_pos: 椭球面顶部中心测试点位置
         Return
             pos: 倾斜PD位置
-            (alpha,beta): 倾斜PD的方位角和倾斜角(单位:度)
+            Nv: 倾斜PD的法向量
         """
         r = np.asarray(r)
         assert r.size in (1,3)
         a, b, c = np.full(shape=(3), fill_value=r) if r.size == 1 else r
 
         # 倾斜PD的方位角和倾斜角
         alpha_rad, beta_rad = np.radians([alpha,beta]) # 角度制转弧度制
@@ -95,34 +93,40 @@
 
         # 倾斜PD位置
         xr = x0 + a * np.cos(alpha_rad) * np.sin(beta_rad)
         yr = y0 + b * np.sin(alpha_rad) * np.sin(beta_rad)
         zr = z0 - c * (1 - np.cos(beta_rad))
         pos = np.stack([xr,yr,zr], axis=-1) # 在最后一维度上堆叠
 
-        # PD的方位角和PD倾斜面的方位角相等
-        # PD的倾斜角和PD倾斜面的倾斜角相等
-        return pos, (alpha,beta)
+        # alpha_rad: PD的方位角和PD倾斜面的摆放角相等
+        # beta_rad: PD的法向量与z轴的夹角和PD倾斜面的倾斜角相等
+        Nx = 1/a * np.cos(alpha_rad) * np.sin(beta_rad)
+        Ny = 1/b * np.sin(alpha_rad) * np.sin(beta_rad)
+        Nz = 1/c * np.cos(beta_rad)
+        Nv = np.stack([Nx,Ny,Nz],axis=-1)
+
+        return pos, Nv
 
     @staticmethod
     def recv_hemisphere_model(r, l, alpha, center_tp_pos:tuple):
         """接收机模型:半球面模型(倾斜PD和中心参考点位置关系)
         Params
             r: 曲球面半径(单位:米)
             l: 倾斜PD到顶部中心(参考点)的弧长(单位:米)   
             alpha:倾斜PD方位角(单位:度) 
             center_tp_pos: 测试点位置 
         Return
             pos: 倾斜PD位置
-            (alpha,beta): 倾斜PD的方位角和倾斜角(单位:度)
+            Nv: 倾斜PD的法向量
         """
         # 倾斜PD的方位角和倾斜角
         beta_rad = l/r   # PD倾斜角
         beta = np.degrees(beta_rad) # 弧度制转角度制
-        return PD.recv_surface_model(r, alpha, beta, center_tp_pos)
+        pos, Nv = PD.recv_surface_model(r, alpha, beta, center_tp_pos)
+        return pos, Nv
 
     def recv_led_radiation_intensity(self, led:LED):
         """计算LED辐射强度(LOS链路):
         Parameters
             led: LED实例化
         Return 
             LOS链路LED辐射强度
@@ -147,20 +151,22 @@
         Parameters
             led: LED实例化
         Return 
             LOS链路中PD探测器接收LED信号
         """
         # LED发射端
         Vt_r = self.pos - led.pos                     # LED到PD的方向向量 (l*w*h,3)
-        d = np.linalg.norm(Vt_r,axis=-1)            # 求模:LED到PD的方向向量的模 (l*w*h)
-        cos_led_t_angle_rad_rad = np.sum(Vt_r*led.Nv, axis=-1) / d # LED发射角的余弦值 (l*w*h)
+        d = np.linalg.norm(Vt_r,axis=-1)              # 求模:LED到PD的方向向量的模 (l*w*h)
+        led_Nv = led.Nv/np.linalg.norm(led.Nv)        # LED单位法向量
+        cos_led_t_angle_rad_rad = np.sum(Vt_r*led_Nv, axis=-1) / d  # LED发射角的余弦值 (l*w*h)
 
         # PD接收端
         Vr_t = -Vt_r # PD到LED的方向向量 (l*w*h,3)
-        cos_pd_r_angle_rad = np.sum(Vr_t*self.Nv, axis=-1) / d     # PD接收角的余弦值 (l*w*h) 
+        pd_Nv = self.Nv/np.linalg.norm(self.Nv)                # PD单位法向量
+        cos_pd_r_angle_rad = np.sum(Vr_t*pd_Nv, axis=-1) / d   # PD接收角的余弦值 (l*w*h) 
 
         # PD入射角
         pd_r_angle_rad = np.arccos(cos_pd_r_angle_rad) # PD接收器入射角的大小(弧度制) (l*w*h)
         pd_r_angle = np.degrees(pd_r_angle_rad)        # 弧度制转为角度制 (l*w*h)
 
         # 计算信道增益
         H0 = (((led.m + 1) * self.Ar) / (2 * np.pi * d**2)) * cos_led_t_angle_rad_rad**led.m * cos_pd_r_angle_rad * self.Ts * self.G_Con # 信道增益 (l*w*h)
@@ -197,24 +203,25 @@
             w_alpha_rad, w_beta_rad = np.radians([w_alpha, w_beta]) # (l1*w1)
 
             # 墙壁反射单元法向量
             Nx = np.cos(w_alpha_rad) * np.sin(w_beta_rad)
             Ny = np.sin(w_alpha_rad) * np.sin(w_beta_rad)
             Nz = np.cos(w_beta_rad)
             Nw = np.stack([Nx,Ny,Nz], axis=-1)  # 墙壁反射点法向量 (l1*w1,3)
-            Nw = Nw/np.linalg.norm(Nw)  # 墙壁反射点的单位法向量 (l1*w1,3)
+            Nw = Nw/np.linalg.norm(Nw)          # 墙壁反射点的单位法向量 (l1*w1,3)
 
             # LED -> 墙壁反射单元
             # 发射端
-            Vt_w = w_pos - led.pos  # LED灯到墙壁反射单元的方向向量 (l1*w1,3)
+            Vt_w = w_pos - led.pos             # LED灯到墙壁反射单元的方向向量 (l1*w1,3)
             d1 = np.linalg.norm(Vt_w, axis=-1) # 求模:LED灯到墙壁反射单元的距离 (l1*w1)
-            mark1 = np.all(Vt_w==0, axis=-1) # 异常点处理:判断墙壁反射单元和LED是否重合(方向向量是否为零向量) (l1*w1)
-            d1 = np.where(mark1, 1, d1)      # 异常点处理:为使cos_led_t_angle_rad分母不为0,让墙壁反射单元和LED重合时的距离不为0 (l1*w1)
+            mark1 = np.all(Vt_w==0, axis=-1)   # 异常点处理:判断墙壁反射单元和LED是否重合(方向向量是否为零向量) (l1*w1)
+            d1 = np.where(mark1, 1, d1)        # 异常点处理:为使cos_led_t_angle_rad分母不为0,让墙壁反射单元和LED重合时的距离不为0 (l1*w1)
             
-            cos_led_t_angle_rad = np.sum(Vt_w*led.Nv, axis=-1) / d1  # LED发射角的余弦值 (l1*w1)
+            led_Nv = led.Nv/np.linalg.norm(led.Nv)        # LED单位法向量
+            cos_led_t_angle_rad = np.sum(Vt_w*led_Nv, axis=-1) / d1  # LED发射角的余弦值 (l1*w1)
 
             # 接收端
             Vw_t = -Vt_w  # 墙壁反射单元到LED灯的方向向量 (l1,w1,3)
             cos_wall_r_angle_rad = np.sum(Vw_t*Nw, axis=-1) / d1 # 墙壁反射单元入射角 (l1*w1)
 
             # 墙壁反射单元 -> PD
             # 发射端
@@ -225,15 +232,16 @@
             d2 = np.where(mark2, 1, d2)      # 异常点处理:为使cos_wall_t_angle_rad分母不为0,让墙壁反射单元和参考点重合时的距离不为0
 
             cos_wall_t_angle_rad = np.sum(Vw_r*Nw, axis=-1) / d2 # 墙壁反射单元发射角  (l*w*h,l1*w1)
             cos_wall_t_angle_rad = np.where(cos_wall_t_angle_rad>0, cos_wall_t_angle_rad, 0) # 满足墙壁反射入射条件 (l*w*h,l1*w1)
       
             # 接收端
             Vr_w = -Vw_r  # PD到墙壁反射单元的方向向量   (l*w*h,l1*w1,3)
-            cos_pd_r_angle_rad = np.sum(Vr_w*self.Nv, axis=-1) / d2 # PD接收角的余弦值   (l*w*h,l1*w1)
+            pd_Nv = self.Nv/np.linalg.norm(self.Nv)               # PD单位法向量
+            cos_pd_r_angle_rad = np.sum(Vr_w*pd_Nv, axis=-1) / d2 # PD接收角的余弦值   (l*w*h,l1*w1)
             cos_pd_r_angle_rad = np.where(cos_pd_r_angle_rad>0, cos_pd_r_angle_rad, 0) # 满足墙壁反射发射条件
 
             # PD入射角
             pd_r_angle_rad = np.arccos(cos_pd_r_angle_rad) # PD接收器入射角(弧度制) (l*w*h,l1*w1)
             pd_r_angle = np.degrees(pd_r_angle_rad) # 弧度制转为角度制 (l*w*h,l1*w1)
 
             rho = room.rho[i]   #墙壁反射率
@@ -324,59 +332,31 @@
         """
         return self._pos + self.origin
     
     @pos.setter
     def pos(self, pos:tuple):
         """设置参考位置
         """
-        if not np.shape(pos)[-1] == 3:
-            raise VLPSequenceLenError(np.shape(pos)[-1],3)
+        pos = np.asarray(pos)
+        if not pos.shape[-1] == 3:
+            raise VLPSequenceLenError(pos.shape[-1],3)
         self._pos = np.asarray(pos)
 
     @property
     def Nv(self):  
-        """获取PD单位法向量  
+        """获取PD法向量  
         """  
-        # PD方位角和倾斜角,角度制转弧度制
-        alpha_rad, beta_rad = np.radians([self.alpha, self.beta])
-        
-        Nx = np.cos(alpha_rad) * np.sin(beta_rad)
-        Ny = np.sin(alpha_rad) * np.sin(beta_rad)
-        Nz = np.cos(beta_rad)
-        N = (Nx,Ny,Nz)
-
-        return  N/np.linalg.norm(N) # 单位化
-
-    @property
-    def alpha(self):
-        """获取PD方位角(单位: 度)
-        """
-        return self._alpha
-    
-    @alpha.setter
-    def alpha(self, alpha):
-        """设置PD方位角(单位: 度)
-        """
-        if not 0 <= alpha <= 360:
-            raise VLPValueRangeError(alpha,0,360)
-        self._alpha = alpha 
-
-    @property
-    def beta(self):
-        """获取PD倾斜角(单位: 度)
-        """
-        return self._beta
+        return self._Nv
     
-    @beta.setter
-    def beta(self, beta):
-        """设置PD倾斜角(单位: 度)
-        """
-        if not -90 <= beta <= 90:
-            raise VLPValueRangeError(beta,-90,90)
-        self._beta = beta 
+    @Nv.setter
+    def Nv(self, n):
+        n = np.asarray(n)
+        if not n.shape[-1] == 3:
+            raise VLPSequenceLenError(n,3)
+        self._Nv = n
 
     @property
     def fov(self):
         """获取接收视场角 (单位: 度)
         """    
         return self._fov
```

### Comparing `yang-vlp-0.2.16/vlppy/model/room.py` & `yang-vlp-0.2.17/vlppy/model/room.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,17 +57,16 @@
             reflect_pos: 反射点坐标(列表元素个数等于反射单元的个数)
         """
         if wall not in (0,1,2,3,4,5):
             raise VLPValueError(wall,0,1,2,3,4,5)
         (xo, yo, zo) = self.origin # 原点
         gx, gy, gz = gap # 墙壁网格划分的间隔
 
-        # 不取靠近墙壁的点（符合实际环境）
         if wall in (0,5):    # 地板或天花板
-            x = np.arange(gx, self.length-gx+1e-3, gx) 
+            x = np.arange(gx, self.length-gx+1e-3, gx)  # 不取靠近墙壁的点（符合实际环境）
             y = np.arange(gy, self.width-gy+1e-3, gy) 
             z = 0 if wall == 0 else self.height 
             Xw, Yw, Zw = np.meshgrid(xo+x, yo+y, zo+z, indexing='ij') # 地板和天花板平面建立二维网格矩阵 
         elif wall in (1,3): #前后墙  
             x = np.arange(0, self.length+1e-3, gx) 
             y = 0 if wall == 1 else self.width 
             z = np.arange(self.rp_height[0], self.rp_height[1]+1e-3, gz)
```

### Comparing `yang-vlp-0.2.16/vlppy/setting/__pycache__/json_setting.cpython-39.pyc` & `yang-vlp-0.2.17/vlppy/setting/__pycache__/json_setting.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/setting/json_setting.py` & `yang-vlp-0.2.17/vlppy/setting/json_setting.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/setting/settings.json` & `yang-vlp-0.2.17/vlppy/setting/settings.json`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/signal/filter.py` & `yang-vlp-0.2.17/vlppy/signal/filter.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/signal/plot.py` & `yang-vlp-0.2.17/vlppy/signal/plot.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/vlppy/vis/vis.py` & `yang-vlp-0.2.17/vlppy/vis/vis.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.16/yang_vlp.egg-info/PKG-INFO` & `yang-vlp-0.2.17/yang_vlp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yang-vlp
-Version: 0.2.16
+Version: 0.2.17
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/yang_vlp
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,17 +31,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 @start date:  2022-08-26
 
-@auther:  yang wu ju
+@auther:  yangwuju
 
-@url: https://gitee.com/yangwuju/yang_vlp
+@url：https://gitee.com/yangwuju/yang_vlp
 
 @file:
 
 - model/room：房间、墙壁参数
 - model/led：led位置、发射的信号(None、DC、AC、AIM)
 - model/pd：pd 各种参数、LOS链路和NLOS链路接收LED信号、噪声
 - signal/filter：滤波器设计（包括fir,iir）
```

### Comparing `yang-vlp-0.2.16/yang_vlp.egg-info/SOURCES.txt` & `yang-vlp-0.2.17/yang_vlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

