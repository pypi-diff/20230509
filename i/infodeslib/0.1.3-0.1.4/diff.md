# Comparing `tmp/infodeslib-0.1.3.tar.gz` & `tmp/infodeslib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infodeslib-0.1.3.tar", last modified: Tue May  9 12:21:28 2023, max compression
+gzip compressed data, was "infodeslib-0.1.4.tar", last modified: Tue May  9 12:30:07 2023, max compression
```

## Comparing `infodeslib-0.1.3.tar` & `infodeslib-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 12:21:28.839751 infodeslib-0.1.3/
--rw-rw-rw-   0        0        0      412 2023-05-09 12:21:28.839751 infodeslib-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      112 2023-05-09 12:20:22.000000 infodeslib-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      528 2023-05-09 12:21:28.841746 infodeslib-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 12:21:28.786599 infodeslib-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 12:21:28.790590 infodeslib-0.1.3/src/infodeslib/
--rw-rw-rw-   0        0        0       25 2023-05-09 11:37:17.000000 infodeslib-0.1.3/src/infodeslib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 12:21:28.812298 infodeslib-0.1.3/src/infodeslib/dcs/
--rw-rw-rw-   0        0        0       81 2023-05-09 10:58:23.000000 infodeslib-0.1.3/src/infodeslib/dcs/__init__.py
--rw-rw-rw-   0        0        0    16481 2023-05-09 10:20:50.000000 infodeslib-0.1.3/src/infodeslib/dcs/lca.py
--rw-rw-rw-   0        0        0    16925 2023-05-09 10:20:53.000000 infodeslib-0.1.3/src/infodeslib/dcs/mla.py
--rw-rw-rw-   0        0        0    20862 2023-05-09 10:20:56.000000 infodeslib-0.1.3/src/infodeslib/dcs/ola.py
--rw-rw-rw-   0        0        0    21295 2023-05-09 10:20:59.000000 infodeslib-0.1.3/src/infodeslib/dcs/rank.py
-drwxrwxrwx   0        0        0        0 2023-05-09 12:21:28.815815 infodeslib-0.1.3/src/infodeslib/dcs/util/
--rw-rw-rw-   0        0        0       47 2023-05-09 10:21:07.000000 infodeslib-0.1.3/src/infodeslib/dcs/util/__init__.py
--rw-rw-rw-   0        0        0     9573 2023-05-09 10:21:11.000000 infodeslib-0.1.3/src/infodeslib/dcs/util/diversity.py
--rw-rw-rw-   0        0        0      990 2023-05-09 10:21:14.000000 infodeslib-0.1.3/src/infodeslib/dcs/util/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 12:21:28.830776 infodeslib-0.1.3/src/infodeslib/des/
--rw-rw-rw-   0        0        0      181 2023-05-09 10:57:33.000000 infodeslib-0.1.3/src/infodeslib/des/__init__.py
--rw-rw-rw-   0        0        0    20486 2023-05-09 10:19:27.000000 infodeslib-0.1.3/src/infodeslib/des/base.py
--rw-rw-rw-   0        0        0    23268 2023-05-09 10:19:31.000000 infodeslib-0.1.3/src/infodeslib/des/desknn.py
--rw-rw-rw-   0        0        0     3754 2023-05-09 10:19:35.000000 infodeslib-0.1.3/src/infodeslib/des/desp.py
--rw-rw-rw-   0        0        0    17334 2023-05-09 10:19:38.000000 infodeslib-0.1.3/src/infodeslib/des/knop.py
--rw-rw-rw-   0        0        0     3650 2023-05-09 10:19:42.000000 infodeslib-0.1.3/src/infodeslib/des/knorae.py
--rw-rw-rw-   0        0        0    22640 2023-05-09 10:19:46.000000 infodeslib-0.1.3/src/infodeslib/des/knorae_w.py
--rw-rw-rw-   0        0        0     3641 2023-05-09 10:19:49.000000 infodeslib-0.1.3/src/infodeslib/des/knorau.py
--rw-rw-rw-   0        0        0    22337 2023-05-09 10:19:53.000000 infodeslib-0.1.3/src/infodeslib/des/knorau_w.py
-drwxrwxrwx   0        0        0        0 2023-05-09 12:21:28.838754 infodeslib-0.1.3/src/infodeslib/des/util/
--rw-rw-rw-   0        0        0       47 2023-05-09 10:20:10.000000 infodeslib-0.1.3/src/infodeslib/des/util/__init__.py
--rw-rw-rw-   0        0        0     9573 2023-05-09 10:20:13.000000 infodeslib-0.1.3/src/infodeslib/des/util/diversity.py
--rw-rw-rw-   0        0        0      990 2023-05-09 10:20:17.000000 infodeslib-0.1.3/src/infodeslib/des/util/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 12:21:28.804488 infodeslib-0.1.3/src/infodeslib.egg-info/
--rw-rw-rw-   0        0        0      412 2023-05-09 12:21:28.000000 infodeslib-0.1.3/src/infodeslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      812 2023-05-09 12:21:28.000000 infodeslib-0.1.3/src/infodeslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 12:21:28.000000 infodeslib-0.1.3/src/infodeslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 12:21:28.000000 infodeslib-0.1.3/src/infodeslib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 12:30:07.775312 infodeslib-0.1.4/
+-rw-rw-rw-   0        0        0      412 2023-05-09 12:30:07.776310 infodeslib-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      111 2023-05-09 12:26:26.000000 infodeslib-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      528 2023-05-09 12:30:07.777308 infodeslib-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 12:30:07.682164 infodeslib-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 12:30:07.687150 infodeslib-0.1.4/src/infodeslib/
+-rw-rw-rw-   0        0        0       25 2023-05-09 11:37:17.000000 infodeslib-0.1.4/src/infodeslib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:30:07.752375 infodeslib-0.1.4/src/infodeslib/dcs/
+-rw-rw-rw-   0        0        0       81 2023-05-09 10:58:23.000000 infodeslib-0.1.4/src/infodeslib/dcs/__init__.py
+-rw-rw-rw-   0        0        0    16481 2023-05-09 10:20:50.000000 infodeslib-0.1.4/src/infodeslib/dcs/lca.py
+-rw-rw-rw-   0        0        0    16925 2023-05-09 10:20:53.000000 infodeslib-0.1.4/src/infodeslib/dcs/mla.py
+-rw-rw-rw-   0        0        0    20862 2023-05-09 10:20:56.000000 infodeslib-0.1.4/src/infodeslib/dcs/ola.py
+-rw-rw-rw-   0        0        0    21295 2023-05-09 10:20:59.000000 infodeslib-0.1.4/src/infodeslib/dcs/rank.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:30:07.755367 infodeslib-0.1.4/src/infodeslib/dcs/util/
+-rw-rw-rw-   0        0        0       47 2023-05-09 10:21:07.000000 infodeslib-0.1.4/src/infodeslib/dcs/util/__init__.py
+-rw-rw-rw-   0        0        0     9573 2023-05-09 10:21:11.000000 infodeslib-0.1.4/src/infodeslib/dcs/util/diversity.py
+-rw-rw-rw-   0        0        0      990 2023-05-09 10:21:14.000000 infodeslib-0.1.4/src/infodeslib/dcs/util/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:30:07.771324 infodeslib-0.1.4/src/infodeslib/des/
+-rw-rw-rw-   0        0        0      181 2023-05-09 10:57:33.000000 infodeslib-0.1.4/src/infodeslib/des/__init__.py
+-rw-rw-rw-   0        0        0    20486 2023-05-09 10:19:27.000000 infodeslib-0.1.4/src/infodeslib/des/base.py
+-rw-rw-rw-   0        0        0    23268 2023-05-09 10:19:31.000000 infodeslib-0.1.4/src/infodeslib/des/desknn.py
+-rw-rw-rw-   0        0        0     3754 2023-05-09 10:19:35.000000 infodeslib-0.1.4/src/infodeslib/des/desp.py
+-rw-rw-rw-   0        0        0    17334 2023-05-09 10:19:38.000000 infodeslib-0.1.4/src/infodeslib/des/knop.py
+-rw-rw-rw-   0        0        0     3650 2023-05-09 10:19:42.000000 infodeslib-0.1.4/src/infodeslib/des/knorae.py
+-rw-rw-rw-   0        0        0    22640 2023-05-09 10:19:46.000000 infodeslib-0.1.4/src/infodeslib/des/knorae_w.py
+-rw-rw-rw-   0        0        0     3641 2023-05-09 10:19:49.000000 infodeslib-0.1.4/src/infodeslib/des/knorau.py
+-rw-rw-rw-   0        0        0    22337 2023-05-09 10:19:53.000000 infodeslib-0.1.4/src/infodeslib/des/knorau_w.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:30:07.774316 infodeslib-0.1.4/src/infodeslib/des/util/
+-rw-rw-rw-   0        0        0       47 2023-05-09 10:20:10.000000 infodeslib-0.1.4/src/infodeslib/des/util/__init__.py
+-rw-rw-rw-   0        0        0     9573 2023-05-09 10:20:13.000000 infodeslib-0.1.4/src/infodeslib/des/util/diversity.py
+-rw-rw-rw-   0        0        0      990 2023-05-09 10:20:17.000000 infodeslib-0.1.4/src/infodeslib/des/util/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:30:07.743427 infodeslib-0.1.4/src/infodeslib.egg-info/
+-rw-rw-rw-   0        0        0      412 2023-05-09 12:30:07.000000 infodeslib-0.1.4/src/infodeslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      812 2023-05-09 12:30:07.000000 infodeslib-0.1.4/src/infodeslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 12:30:07.000000 infodeslib-0.1.4/src/infodeslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 12:30:07.000000 infodeslib-0.1.4/src/infodeslib.egg-info/top_level.txt
```

### Comparing `infodeslib-0.1.3/setup.cfg` & `infodeslib-0.1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 6e66 6f64 6573 6c69 620d 0a76   = infodeslib..v
-00000020: 6572 7369 6f6e 203d 2030 2e31 2e33 0d0a  ersion = 0.1.3..
+00000020: 6572 7369 6f6e 203d 2030 2e31 2e34 0d0a  ersion = 0.1.4..
 00000030: 6175 7468 6f72 203d 2061 6476 2d70 616e  author = adv-pan
 00000040: 6461 0d0a 6175 7468 6f72 5f65 6d61 696c  da..author_email
 00000050: 203d 2070 616e 6461 4067 6d61 696c 2e63   = panda@gmail.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 496d 706c 656d 656e 7461 7469 6f6e  = Implementation
 00000080: 206f 6620 4479 6e61 6d69 6320 456e 7365   of Dynamic Ense
 00000090: 6d62 6c65 2053 656c 6563 7469 6f6e 206d  mble Selection m
```

### Comparing `infodeslib-0.1.3/src/infodeslib/dcs/lca.py` & `infodeslib-0.1.4/src/infodeslib/dcs/lca.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/dcs/mla.py` & `infodeslib-0.1.4/src/infodeslib/dcs/mla.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/dcs/ola.py` & `infodeslib-0.1.4/src/infodeslib/dcs/ola.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/dcs/rank.py` & `infodeslib-0.1.4/src/infodeslib/dcs/rank.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/dcs/util/diversity.py` & `infodeslib-0.1.4/src/infodeslib/dcs/util/diversity.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/dcs/util/utils.py` & `infodeslib-0.1.4/src/infodeslib/dcs/util/utils.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/des/base.py` & `infodeslib-0.1.4/src/infodeslib/des/base.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/des/desknn.py` & `infodeslib-0.1.4/src/infodeslib/des/desknn.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/des/desp.py` & `infodeslib-0.1.4/src/infodeslib/des/desp.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/des/knop.py` & `infodeslib-0.1.4/src/infodeslib/des/knop.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/des/knorae.py` & `infodeslib-0.1.4/src/infodeslib/des/knorae.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/des/knorae_w.py` & `infodeslib-0.1.4/src/infodeslib/des/knorae_w.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/des/knorau.py` & `infodeslib-0.1.4/src/infodeslib/des/knorau.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/des/knorau_w.py` & `infodeslib-0.1.4/src/infodeslib/des/knorau_w.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/des/util/diversity.py` & `infodeslib-0.1.4/src/infodeslib/des/util/diversity.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib/des/util/utils.py` & `infodeslib-0.1.4/src/infodeslib/des/util/utils.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.3/src/infodeslib.egg-info/SOURCES.txt` & `infodeslib-0.1.4/src/infodeslib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

