# Comparing `tmp/OpenAccess-0.1.2.tar.gz` & `tmp/OpenAccess-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenAccess-0.1.2.tar", last modified: Tue May  9 03:44:32 2023, max compression
+gzip compressed data, was "OpenAccess-0.2.tar", last modified: Tue May  9 14:46:35 2023, max compression
```

## Comparing `OpenAccess-0.1.2.tar` & `OpenAccess-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 03:44:32.148360 OpenAccess-0.1.2/
-drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 03:44:32.148360 OpenAccess-0.1.2/OpenAccess/
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)      105 2023-05-09 03:44:22.000000 OpenAccess-0.1.2/OpenAccess/__init__.py
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)    12381 2023-05-08 22:37:09.000000 OpenAccess-0.1.2/OpenAccess/openaccess.py
-drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 03:44:32.148360 OpenAccess-0.1.2/OpenAccess.egg-info/
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1581 2023-05-09 03:44:32.000000 OpenAccess-0.1.2/OpenAccess.egg-info/PKG-INFO
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)      235 2023-05-09 03:44:32.000000 OpenAccess-0.1.2/OpenAccess.egg-info/SOURCES.txt
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)        1 2023-05-09 03:44:32.000000 OpenAccess-0.1.2/OpenAccess.egg-info/dependency_links.txt
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)        9 2023-05-09 03:44:32.000000 OpenAccess-0.1.2/OpenAccess.egg-info/requires.txt
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)       11 2023-05-09 03:44:32.000000 OpenAccess-0.1.2/OpenAccess.egg-info/top_level.txt
--rw-rw-r--   0 jaiber    (1000) jaiber    (1000)     1581 2023-05-09 03:44:32.148360 OpenAccess-0.1.2/PKG-INFO
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1249 2023-04-24 21:19:05.000000 OpenAccess-0.1.2/README.md
--rw-rw-r--   0 jaiber    (1000) jaiber    (1000)       38 2023-05-09 03:44:32.148360 OpenAccess-0.1.2/setup.cfg
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1392 2023-04-03 16:58:33.000000 OpenAccess-0.1.2/setup.py
+drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 14:46:35.746033 OpenAccess-0.2/
+drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 14:46:35.746033 OpenAccess-0.2/OpenAccess/
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)      103 2023-05-09 14:46:13.000000 OpenAccess-0.2/OpenAccess/__init__.py
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)    12379 2023-05-09 14:46:08.000000 OpenAccess-0.2/OpenAccess/openaccess.py
+drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 14:46:35.746033 OpenAccess-0.2/OpenAccess.egg-info/
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1579 2023-05-09 14:46:35.000000 OpenAccess-0.2/OpenAccess.egg-info/PKG-INFO
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)      235 2023-05-09 14:46:35.000000 OpenAccess-0.2/OpenAccess.egg-info/SOURCES.txt
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)        1 2023-05-09 14:46:35.000000 OpenAccess-0.2/OpenAccess.egg-info/dependency_links.txt
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)        9 2023-05-09 14:46:35.000000 OpenAccess-0.2/OpenAccess.egg-info/requires.txt
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)       11 2023-05-09 14:46:35.000000 OpenAccess-0.2/OpenAccess.egg-info/top_level.txt
+-rw-rw-r--   0 jaiber    (1000) jaiber    (1000)     1579 2023-05-09 14:46:35.746033 OpenAccess-0.2/PKG-INFO
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1249 2023-04-24 21:19:05.000000 OpenAccess-0.2/README.md
+-rw-rw-r--   0 jaiber    (1000) jaiber    (1000)       38 2023-05-09 14:46:35.746033 OpenAccess-0.2/setup.cfg
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1392 2023-04-03 16:58:33.000000 OpenAccess-0.2/setup.py
```

### Comparing `OpenAccess-0.1.2/OpenAccess/openaccess.py` & `OpenAccess-0.2/OpenAccess/openaccess.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,15 @@
 
         # Dictionary of method parameters (none)
         parameter_value = {
             "Device": incommingEvent.device,
             "SubDevice": incommingEvent.subdevice,
             "Description": incommingEvent.description,
             "Source": incommingEvent.source,
-            "IsAccessGrant":incommingEvent.isAccessGranted,
+            "IsAccessGrant":incommingEvent.isAccessGrant,
             "IsAccessDeny":incommingEvent.isAccessDeny,
             "BadgeID":incommingEvent.badgeId
 
         }
 
         # Data object to be serialized by PostAsJsonAsync
         em = {
```

### Comparing `OpenAccess-0.1.2/OpenAccess.egg-info/PKG-INFO` & `OpenAccess-0.2/OpenAccess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAccess
-Version: 0.1.2
+Version: 0.2
 Summary: Librería no oficial para leer comunicarse con un servidor de LENEL OpenAccess 
 Home-page: https://github.com/alejomejia1
 Author: Alejandro Mejia Ayala, Jaiber Camacho
 Author-email: alejandromejia@qaingenieros.com
 License: GNU
 Description-Content-Type: text/markdown
```

### Comparing `OpenAccess-0.1.2/PKG-INFO` & `OpenAccess-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAccess
-Version: 0.1.2
+Version: 0.2
 Summary: Librería no oficial para leer comunicarse con un servidor de LENEL OpenAccess 
 Home-page: https://github.com/alejomejia1
 Author: Alejandro Mejia Ayala, Jaiber Camacho
 Author-email: alejandromejia@qaingenieros.com
 License: GNU
 Description-Content-Type: text/markdown
```

### Comparing `OpenAccess-0.1.2/README.md` & `OpenAccess-0.2/README.md`

 * *Files identical despite different names*

### Comparing `OpenAccess-0.1.2/setup.py` & `OpenAccess-0.2/setup.py`

 * *Files identical despite different names*

