# Comparing `tmp/enhanceezqq-1.0.0.1.tar.gz` & `tmp/enhanceezqq-1.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhanceezqq-1.0.0.1.tar", last modified: Tue May  9 08:29:08 2023, max compression
+gzip compressed data, was "enhanceezqq-1.0.0.2.tar", last modified: Tue May  9 12:51:46 2023, max compression
```

## Comparing `enhanceezqq-1.0.0.1.tar` & `enhanceezqq-1.0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 08:29:08.808408 enhanceezqq-1.0.0.1/
--rw-rw-rw-   0        0        0      307 2023-05-09 08:29:08.808408 enhanceezqq-1.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2696 2023-04-16 04:39:07.000000 enhanceezqq-1.0.0.1/akpack.py
--rw-rw-rw-   0        0        0     5179 2023-04-15 07:50:36.000000 enhanceezqq-1.0.0.1/basefund.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:29:08.789404 enhanceezqq-1.0.0.1/config/
-drwxrwxrwx   0        0        0        0 2023-05-09 08:29:08.799406 enhanceezqq-1.0.0.1/config/enhanceezqq/
--rw-rw-rw-   0        0        0      394 2023-04-15 01:21:04.000000 enhanceezqq-1.0.0.1/config/enhanceezqq/enhanceezqq_config.json
-drwxrwxrwx   0        0        0        0 2023-05-09 08:29:08.806408 enhanceezqq-1.0.0.1/enhanceezqq.egg-info/
--rw-rw-rw-   0        0        0      307 2023-05-09 08:29:08.000000 enhanceezqq-1.0.0.1/enhanceezqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-09 08:29:08.000000 enhanceezqq-1.0.0.1/enhanceezqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 08:29:08.000000 enhanceezqq-1.0.0.1/enhanceezqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-09 08:29:08.000000 enhanceezqq-1.0.0.1/enhanceezqq.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      299 2023-05-09 08:29:08.000000 enhanceezqq-1.0.0.1/enhanceezqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2023-05-09 08:29:08.000000 enhanceezqq-1.0.0.1/enhanceezqq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17690 2023-04-18 03:13:40.000000 enhanceezqq-1.0.0.1/enhanceezqq.py
--rw-rw-rw-   0        0        0       42 2023-05-09 08:29:08.809409 enhanceezqq-1.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     6270 2023-05-09 08:28:49.000000 enhanceezqq-1.0.0.1/setup.py
--rw-rw-rw-   0        0        0     5674 2023-04-15 05:59:20.000000 enhanceezqq-1.0.0.1/ths.py
--rw-rw-rw-   0        0        0     5690 2023-04-15 05:59:20.000000 enhanceezqq-1.0.0.1/ttjj.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:51:46.786028 enhanceezqq-1.0.0.2/
+-rw-rw-rw-   0        0        0      307 2023-05-09 12:51:46.786028 enhanceezqq-1.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2696 2023-04-16 04:39:07.000000 enhanceezqq-1.0.0.2/akpack.py
+-rw-rw-rw-   0        0        0     5179 2023-04-15 07:50:36.000000 enhanceezqq-1.0.0.2/basefund.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:51:46.762023 enhanceezqq-1.0.0.2/config/
+drwxrwxrwx   0        0        0        0 2023-05-09 12:51:46.774025 enhanceezqq-1.0.0.2/config/enhanceezqq/
+-rw-rw-rw-   0        0        0      394 2023-04-15 01:21:04.000000 enhanceezqq-1.0.0.2/config/enhanceezqq/enhanceezqq_config.json
+drwxrwxrwx   0        0        0        0 2023-05-09 12:51:46.784027 enhanceezqq-1.0.0.2/enhanceezqq.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-05-09 12:51:46.000000 enhanceezqq-1.0.0.2/enhanceezqq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-09 12:51:46.000000 enhanceezqq-1.0.0.2/enhanceezqq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 12:51:46.000000 enhanceezqq-1.0.0.2/enhanceezqq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-09 12:51:46.000000 enhanceezqq-1.0.0.2/enhanceezqq.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      299 2023-05-09 12:51:46.000000 enhanceezqq-1.0.0.2/enhanceezqq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2023-05-09 12:51:46.000000 enhanceezqq-1.0.0.2/enhanceezqq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17684 2023-05-09 12:51:24.000000 enhanceezqq-1.0.0.2/enhanceezqq.py
+-rw-rw-rw-   0        0        0       42 2023-05-09 12:51:46.786028 enhanceezqq-1.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     6270 2023-05-09 12:51:24.000000 enhanceezqq-1.0.0.2/setup.py
+-rw-rw-rw-   0        0        0     5674 2023-04-15 05:59:20.000000 enhanceezqq-1.0.0.2/ths.py
+-rw-rw-rw-   0        0        0     5690 2023-04-15 05:59:20.000000 enhanceezqq-1.0.0.2/ttjj.py
```

### Comparing `enhanceezqq-1.0.0.1/akpack.py` & `enhanceezqq-1.0.0.2/akpack.py`

 * *Files identical despite different names*

### Comparing `enhanceezqq-1.0.0.1/basefund.py` & `enhanceezqq-1.0.0.2/basefund.py`

 * *Files identical despite different names*

### Comparing `enhanceezqq-1.0.0.1/enhanceezqq.py` & `enhanceezqq-1.0.0.2/enhanceezqq.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
     # 是否更新股票本地代码信息
     parser.add_argument('-u', '-updateflag', type=str, choices=("y", "n", "Y", "N"), default=updatecodesflag,
                         help='是否根据网络数据更新股票代码信息的本地缓冲, 默认值：{}'.format(updatecodesflag))
 
     # 是否更新基金或者股票的历史数据本地缓存
     parser.add_argument('-his', '-history', type=str, choices=("y", "n", "Y", "N"), default=historyflag,
-                        help='是否根据网络数据更新股票代码信息的本地缓冲, 默认值：{}'.format(historyflag))
+                        help='是否更新基金或者股票的历史数据本地缓存, 默认值：{}'.format(historyflag))
 
     # 获取股票全部股票代码
     parser.add_argument('-g', '-getcodes', type=str, choices=getcodechoice, default=getcodesflag,
                         help='获取网络股票代码/本地缓冲信息, 默认值：{}'.format(getcodesflag))
 
     # 数据源为jsl时的子参数
     parser.add_argument('-j', '-jsltype', type=str,  default=jsltypedefault, choices=jsltypelist,
```

### Comparing `enhanceezqq-1.0.0.1/setup.py` & `enhanceezqq-1.0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 00000940: 7269 6769 6e63 6f6e 6669 6764 6972 2c20  riginconfigdir, 
 00000950: 5b6f 7267 696e 636f 6e66 6967 6669 6c65  [orginconfigfile
 00000960: 5d29 2c0d 0a20 2020 2020 2020 205d 0d0a  ]),..        ]..
 00000970: 2020 2020 7265 7475 726e 2064 6174 615f      return data_
 00000980: 6669 6c65 730d 0a0d 0a0d 0a73 6574 7570  files......setup
 00000990: 280d 0a20 2020 206e 616d 653d 2765 6e68  (..    name='enh
 000009a0: 616e 6365 657a 7171 272c 0d0a 2020 2020  anceezqq',..    
-000009b0: 7665 7273 696f 6e3d 2731 2e30 2e30 2e31  version='1.0.0.1
+000009b0: 7665 7273 696f 6e3d 2731 2e30 2e30 2e32  version='1.0.0.2
 000009c0: 272c 0d0a 2020 2020 6465 7363 7269 7074  ',..    descript
 000009d0: 696f 6e3d 27e7 94a8 e4ba 8ee5 afb9 657a  ion='.........ez
 000009e0: 7171 e6a8 a1e5 9d97 e5a2 9ee5 bcba e58a  qq..............
 000009f0: 9fe8 83bd efbc 8ce8 83bd e5a4 9fe8 8eb7  ................
 00000a00: e58f 96e5 8e86 e58f b2e6 95b0 e68d aee4  ................
 00000a10: bf9d e5ad 98e5 88b0 e695 b0e6 8dae e5ba  ................
 00000a20: 93ef bc8c e5b9 b6e4 bb8e e695 b0e6 8dae  ................
```

### Comparing `enhanceezqq-1.0.0.1/ths.py` & `enhanceezqq-1.0.0.2/ths.py`

 * *Files identical despite different names*

### Comparing `enhanceezqq-1.0.0.1/ttjj.py` & `enhanceezqq-1.0.0.2/ttjj.py`

 * *Files identical despite different names*

