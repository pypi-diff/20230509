# Comparing `tmp/infodeslib-0.1.1.tar.gz` & `tmp/infodeslib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infodeslib-0.1.1.tar", last modified: Tue May  9 11:10:16 2023, max compression
+gzip compressed data, was "infodeslib-0.1.2.tar", last modified: Tue May  9 11:52:59 2023, max compression
```

## Comparing `infodeslib-0.1.1.tar` & `infodeslib-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 11:10:16.086191 infodeslib-0.1.1/
--rw-rw-rw-   0        0        0      488 2023-05-09 11:10:16.084195 infodeslib-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-09 11:10:16.047547 infodeslib-0.1.1/dcs/
--rw-rw-rw-   0        0        0       81 2023-05-09 10:58:23.000000 infodeslib-0.1.1/dcs/__init__.py
--rw-rw-rw-   0        0        0    16481 2023-05-09 10:20:50.000000 infodeslib-0.1.1/dcs/lca.py
--rw-rw-rw-   0        0        0    16925 2023-05-09 10:20:53.000000 infodeslib-0.1.1/dcs/mla.py
--rw-rw-rw-   0        0        0    20862 2023-05-09 10:20:56.000000 infodeslib-0.1.1/dcs/ola.py
--rw-rw-rw-   0        0        0    21295 2023-05-09 10:20:59.000000 infodeslib-0.1.1/dcs/rank.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:10:16.053533 infodeslib-0.1.1/dcs/util/
--rw-rw-rw-   0        0        0       47 2023-05-09 10:21:07.000000 infodeslib-0.1.1/dcs/util/__init__.py
--rw-rw-rw-   0        0        0     9573 2023-05-09 10:21:11.000000 infodeslib-0.1.1/dcs/util/diversity.py
--rw-rw-rw-   0        0        0      990 2023-05-09 10:21:14.000000 infodeslib-0.1.1/dcs/util/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:10:16.064503 infodeslib-0.1.1/des/
--rw-rw-rw-   0        0        0      181 2023-05-09 10:57:33.000000 infodeslib-0.1.1/des/__init__.py
--rw-rw-rw-   0        0        0    20486 2023-05-09 10:19:27.000000 infodeslib-0.1.1/des/base.py
--rw-rw-rw-   0        0        0    23268 2023-05-09 10:19:31.000000 infodeslib-0.1.1/des/desknn.py
--rw-rw-rw-   0        0        0     3754 2023-05-09 10:19:35.000000 infodeslib-0.1.1/des/desp.py
--rw-rw-rw-   0        0        0    17334 2023-05-09 10:19:38.000000 infodeslib-0.1.1/des/knop.py
--rw-rw-rw-   0        0        0     3650 2023-05-09 10:19:42.000000 infodeslib-0.1.1/des/knorae.py
--rw-rw-rw-   0        0        0    22640 2023-05-09 10:19:46.000000 infodeslib-0.1.1/des/knorae_w.py
--rw-rw-rw-   0        0        0     3641 2023-05-09 10:19:49.000000 infodeslib-0.1.1/des/knorau.py
--rw-rw-rw-   0        0        0    22337 2023-05-09 10:19:53.000000 infodeslib-0.1.1/des/knorau_w.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:10:16.072256 infodeslib-0.1.1/des/util/
--rw-rw-rw-   0        0        0       47 2023-05-09 10:20:10.000000 infodeslib-0.1.1/des/util/__init__.py
--rw-rw-rw-   0        0        0     9573 2023-05-09 10:20:13.000000 infodeslib-0.1.1/des/util/diversity.py
--rw-rw-rw-   0        0        0      990 2023-05-09 10:20:17.000000 infodeslib-0.1.1/des/util/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:10:16.083228 infodeslib-0.1.1/infodeslib.egg-info/
--rw-rw-rw-   0        0        0      488 2023-05-09 11:10:15.000000 infodeslib-0.1.1/infodeslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-05-09 11:10:15.000000 infodeslib-0.1.1/infodeslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 11:10:15.000000 infodeslib-0.1.1/infodeslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-09 11:10:15.000000 infodeslib-0.1.1/infodeslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 11:10:16.086191 infodeslib-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      704 2023-05-09 11:10:09.000000 infodeslib-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 11:52:59.600274 infodeslib-0.1.2/
+-rw-rw-rw-   0        0        0      412 2023-05-09 11:52:59.600274 infodeslib-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      111 2023-05-09 11:48:14.000000 infodeslib-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      528 2023-05-09 11:52:59.601274 infodeslib-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 11:52:59.545833 infodeslib-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 11:52:59.554809 infodeslib-0.1.2/src/dcs/
+-rw-rw-rw-   0        0        0       81 2023-05-09 10:58:23.000000 infodeslib-0.1.2/src/dcs/__init__.py
+-rw-rw-rw-   0        0        0    16481 2023-05-09 10:20:50.000000 infodeslib-0.1.2/src/dcs/lca.py
+-rw-rw-rw-   0        0        0    16925 2023-05-09 10:20:53.000000 infodeslib-0.1.2/src/dcs/mla.py
+-rw-rw-rw-   0        0        0    20862 2023-05-09 10:20:56.000000 infodeslib-0.1.2/src/dcs/ola.py
+-rw-rw-rw-   0        0        0    21295 2023-05-09 10:20:59.000000 infodeslib-0.1.2/src/dcs/rank.py
+drwxrwxrwx   0        0        0        0 2023-05-09 11:52:59.560794 infodeslib-0.1.2/src/dcs/util/
+-rw-rw-rw-   0        0        0       47 2023-05-09 10:21:07.000000 infodeslib-0.1.2/src/dcs/util/__init__.py
+-rw-rw-rw-   0        0        0     9573 2023-05-09 10:21:11.000000 infodeslib-0.1.2/src/dcs/util/diversity.py
+-rw-rw-rw-   0        0        0      990 2023-05-09 10:21:14.000000 infodeslib-0.1.2/src/dcs/util/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 11:52:59.577795 infodeslib-0.1.2/src/des/
+-rw-rw-rw-   0        0        0      181 2023-05-09 10:57:33.000000 infodeslib-0.1.2/src/des/__init__.py
+-rw-rw-rw-   0        0        0    20486 2023-05-09 10:19:27.000000 infodeslib-0.1.2/src/des/base.py
+-rw-rw-rw-   0        0        0    23268 2023-05-09 10:19:31.000000 infodeslib-0.1.2/src/des/desknn.py
+-rw-rw-rw-   0        0        0     3754 2023-05-09 10:19:35.000000 infodeslib-0.1.2/src/des/desp.py
+-rw-rw-rw-   0        0        0    17334 2023-05-09 10:19:38.000000 infodeslib-0.1.2/src/des/knop.py
+-rw-rw-rw-   0        0        0     3650 2023-05-09 10:19:42.000000 infodeslib-0.1.2/src/des/knorae.py
+-rw-rw-rw-   0        0        0    22640 2023-05-09 10:19:46.000000 infodeslib-0.1.2/src/des/knorae_w.py
+-rw-rw-rw-   0        0        0     3641 2023-05-09 10:19:49.000000 infodeslib-0.1.2/src/des/knorau.py
+-rw-rw-rw-   0        0        0    22337 2023-05-09 10:19:53.000000 infodeslib-0.1.2/src/des/knorau_w.py
+drwxrwxrwx   0        0        0        0 2023-05-09 11:52:59.582013 infodeslib-0.1.2/src/des/util/
+-rw-rw-rw-   0        0        0       47 2023-05-09 10:20:10.000000 infodeslib-0.1.2/src/des/util/__init__.py
+-rw-rw-rw-   0        0        0     9573 2023-05-09 10:20:13.000000 infodeslib-0.1.2/src/des/util/diversity.py
+-rw-rw-rw-   0        0        0      990 2023-05-09 10:20:17.000000 infodeslib-0.1.2/src/des/util/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 11:52:59.598818 infodeslib-0.1.2/src/infodeslib.egg-info/
+-rw-rw-rw-   0        0        0      412 2023-05-09 11:52:59.000000 infodeslib-0.1.2/src/infodeslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2023-05-09 11:52:59.000000 infodeslib-0.1.2/src/infodeslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 11:52:59.000000 infodeslib-0.1.2/src/infodeslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-09 11:52:59.000000 infodeslib-0.1.2/src/infodeslib.egg-info/top_level.txt
```

### Comparing `infodeslib-0.1.1/dcs/lca.py` & `infodeslib-0.1.2/src/dcs/lca.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/dcs/mla.py` & `infodeslib-0.1.2/src/dcs/mla.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/dcs/ola.py` & `infodeslib-0.1.2/src/dcs/ola.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/dcs/rank.py` & `infodeslib-0.1.2/src/dcs/rank.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/dcs/util/diversity.py` & `infodeslib-0.1.2/src/dcs/util/diversity.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/dcs/util/utils.py` & `infodeslib-0.1.2/src/dcs/util/utils.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/des/base.py` & `infodeslib-0.1.2/src/des/base.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/des/desknn.py` & `infodeslib-0.1.2/src/des/desknn.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/des/desp.py` & `infodeslib-0.1.2/src/des/desp.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/des/knop.py` & `infodeslib-0.1.2/src/des/knop.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/des/knorae.py` & `infodeslib-0.1.2/src/des/knorae.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/des/knorae_w.py` & `infodeslib-0.1.2/src/des/knorae_w.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/des/knorau.py` & `infodeslib-0.1.2/src/des/knorau.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/des/knorau_w.py` & `infodeslib-0.1.2/src/des/knorau_w.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/des/util/diversity.py` & `infodeslib-0.1.2/src/des/util/diversity.py`

 * *Files identical despite different names*

### Comparing `infodeslib-0.1.1/des/util/utils.py` & `infodeslib-0.1.2/src/des/util/utils.py`

 * *Files identical despite different names*

