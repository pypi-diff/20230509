# Comparing `tmp/hikaxpro-2.1.2.tar.gz` & `tmp/hikaxpro-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikaxpro-2.1.2.tar", last modified: Mon Apr 17 11:28:16 2023, max compression
+gzip compressed data, was "hikaxpro-2.1.3.tar", last modified: Tue May  9 21:19:21 2023, max compression
```

## Comparing `hikaxpro-2.1.2.tar` & `hikaxpro-2.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:28:16.111501 hikaxpro-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-17 11:28:16.111501 hikaxpro-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 11:28:16.111501 hikaxpro-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:28:16.107500 hikaxpro-2.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/src/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:28:16.107500 hikaxpro-2.1.2/src/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/src/errors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:28:16.107500 hikaxpro-2.1.2/src/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/src/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/src/helpers/sha256.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/src/helpers/xmlBuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:28:16.107500 hikaxpro-2.1.2/src/hikaxpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-17 11:28:16.000000 hikaxpro-2.1.2/src/hikaxpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-17 11:28:16.000000 hikaxpro-2.1.2/src/hikaxpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:28:16.000000 hikaxpro-2.1.2/src/hikaxpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 11:28:16.000000 hikaxpro-2.1.2/src/hikaxpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 11:28:16.000000 hikaxpro-2.1.2/src/hikaxpro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/src/hikaxpro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:28:16.111501 hikaxpro-2.1.2/src/models/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/src/models/SessionLogin.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/src/models/SessionLoginCap.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:28:16.111501 hikaxpro-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/tests/test_hikaxpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-17 11:28:04.000000 hikaxpro-2.1.2/tests/test_xmlBuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.754901 hikaxpro-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-09 21:19:21.754901 hikaxpro-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 21:19:21.754901 hikaxpro-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.750901 hikaxpro-2.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.750901 hikaxpro-2.1.3/src/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/errors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.750901 hikaxpro-2.1.3/src/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/helpers/sha256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/helpers/xmlBuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.754901 hikaxpro-2.1.3/src/hikaxpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-09 21:19:21.000000 hikaxpro-2.1.3/src/hikaxpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-09 21:19:21.000000 hikaxpro-2.1.3/src/hikaxpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:19:21.000000 hikaxpro-2.1.3/src/hikaxpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-09 21:19:21.000000 hikaxpro-2.1.3/src/hikaxpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 21:19:21.000000 hikaxpro-2.1.3/src/hikaxpro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/hikaxpro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.754901 hikaxpro-2.1.3/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/models/SessionLogin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/models/SessionLoginCap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.754901 hikaxpro-2.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/tests/test_hikaxpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/tests/test_xmlBuilder.py
```

### Comparing `hikaxpro-2.1.2/LICENSE` & `hikaxpro-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.1.2/PKG-INFO` & `hikaxpro-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikaxpro
-Version: 2.1.2
+Version: 2.1.3
 Summary: Hikvision AX Pro alarm kit ISAPI integration for home assistant alarm panel
 Author-email: Günkut Zeybek <gunkut.zeybek@gmail.com>, Petr Leo Compel <petrleocompel@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2022 smartha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `hikaxpro-2.1.2/pyproject.toml` & `hikaxpro-2.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hikaxpro"
-version = "2.1.2"
+version = "2.1.3"
 description = "Hikvision AX Pro alarm kit ISAPI integration for home assistant alarm panel"
 readme = "README.md"
 authors = [
     { name = "Günkut Zeybek", email = "gunkut.zeybek@gmail.com" },
     { name = "Petr Leo Compel", email = "petrleocompel@gmail.com" }
 ]
 license = { file = "LICENSE" }
@@ -26,15 +26,15 @@
 [project.urls]
 repository = "https://github.com/petrleocompel/hikaxpro/"
 
 [project.optional-dependencies]
 dev = ["pytest", "requests_mock"]
 
 [tool.bumpver]
-current_version = "2.1.2"
+current_version = "2.1.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore: release version {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `hikaxpro-2.1.2/src/consts.py` & `hikaxpro-2.1.3/src/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     AlertStream = "/ISAPI/Event/notification/alertStream"
     DetectorConfig = "/ISAPI/SecurityCP/BasicParam/DetectorCfg"
     DetectorConfigCap = "/ISAPI/SecurityCP/BasicParam/DetectorCfg/capabilities"
     Caps = "/ISAPI/SecurityCP/capabilities"
     CheckResultCap = "/ISAPI/SecurityCP/CheckResult/capabilities"
     CheckResult = "/ISAPI/SecurityCP/CheckResult"
     ConfCap = "/ISAPI/SecurityCP/Configuration/capabilities"
+    ZonesConfig = "/ISAPI/SecurityCP/Configuration/zones"
     DeviceTime = "/ISAPI/SecurityCP/Configuration/deviceTime"
     EventRecordCap = "/ISAPI/SecurityCP/Configuration/eventRecord/channels/2/capabilities"
     EventRecord = "/ISAPI/SecurityCP/Configuration/eventRecord/channels/1"
     FaultCheck = "/ISAPI/SecurityCP/Configuration/faultCheckCfg"
     GlassBreakDetector = "/ISAPI/SecurityCP/Configuration/glassBreakDetector/zone/5"
     MagneticContact = "/ISAPI/SecurityCP/Configuration/magneticContact/zone/0"
     PublicSubSystem = "/ISAPI/SecurityCP/Configuration/publicSubSys"
```

### Comparing `hikaxpro-2.1.2/src/helpers/sha256.py` & `hikaxpro-2.1.3/src/helpers/sha256.py`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.1.2/src/helpers/xmlBuilder.py` & `hikaxpro-2.1.3/src/helpers/xmlBuilder.py`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.1.2/src/hikaxpro.egg-info/PKG-INFO` & `hikaxpro-2.1.3/src/hikaxpro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikaxpro
-Version: 2.1.2
+Version: 2.1.3
 Summary: Hikvision AX Pro alarm kit ISAPI integration for home assistant alarm panel
 Author-email: Günkut Zeybek <gunkut.zeybek@gmail.com>, Petr Leo Compel <petrleocompel@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2022 smartha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `hikaxpro-2.1.2/src/hikaxpro.py` & `hikaxpro-2.1.3/src/hikaxpro.py`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.1.2/tests/test_hikaxpro.py` & `hikaxpro-2.1.3/tests/test_hikaxpro.py`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.1.2/tests/test_xmlBuilder.py` & `hikaxpro-2.1.3/tests/test_xmlBuilder.py`

 * *Files identical despite different names*

