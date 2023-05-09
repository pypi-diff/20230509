# Comparing `tmp/rpmdyn-2023.5.7.3.tar.gz` & `tmp/rpmdyn-2023.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpmdyn-2023.5.7.3.tar", last modified: Sun May  7 03:03:42 2023, max compression
+gzip compressed data, was "rpmdyn-2023.5.9.tar", last modified: Tue May  9 00:06:24 2023, max compression
```

## Comparing `rpmdyn-2023.5.7.3.tar` & `rpmdyn-2023.5.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.617071 rpmdyn-2023.5.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    43845 2023-05-07 03:03:42.617071 rpmdyn-2023.5.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.613070 rpmdyn-2023.5.7.3/custom_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/custom_build/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 03:03:42.621070 rpmdyn-2023.5.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.613070 rpmdyn-2023.5.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.617071 rpmdyn-2023.5.7.3/src/rpmdyn/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-07 03:03:42.000000 rpmdyn-2023.5.7.3/src/rpmdyn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24226 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/_ffi.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/_keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/_pth_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/_rpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/rpmdyn.pth
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.617071 rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43845 2023-05-07 03:03:42.000000 rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-07 03:03:42.000000 rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:03:42.000000 rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 03:03:42.000000 rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 03:03:42.000000 rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.617071 rpmdyn-2023.5.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.617071 rpmdyn-2023.5.7.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/data/test-srpm01-1.0-1.src.rpm
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/data/walrus-5.21-1.noarch.rpm
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/test_labelcompare.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/test_transactionset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:06:24.253623 rpmdyn-2023.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    43843 2023-05-09 00:06:24.253623 rpmdyn-2023.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:06:24.249623 rpmdyn-2023.5.9/custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/custom_build/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:06:24.253623 rpmdyn-2023.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:06:24.249623 rpmdyn-2023.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:06:24.249623 rpmdyn-2023.5.9/src/rpmdyn/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-09 00:06:23.000000 rpmdyn-2023.5.9/src/rpmdyn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24226 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/src/rpmdyn/_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/src/rpmdyn/_ffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/src/rpmdyn/_keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/src/rpmdyn/_pth_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/src/rpmdyn/_rpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/src/rpmdyn/_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/src/rpmdyn/rpmdyn.pth
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:06:24.249623 rpmdyn-2023.5.9/src/rpmdyn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43843 2023-05-09 00:06:24.000000 rpmdyn-2023.5.9/src/rpmdyn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-09 00:06:24.000000 rpmdyn-2023.5.9/src/rpmdyn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:06:24.000000 rpmdyn-2023.5.9/src/rpmdyn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 00:06:24.000000 rpmdyn-2023.5.9/src/rpmdyn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 00:06:24.000000 rpmdyn-2023.5.9/src/rpmdyn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:06:24.253623 rpmdyn-2023.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:06:24.253623 rpmdyn-2023.5.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/tests/data/test-srpm01-1.0-1.src.rpm
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/tests/data/walrus-5.21-1.noarch.rpm
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/tests/test_labelcompare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-09 00:06:02.000000 rpmdyn-2023.5.9/tests/test_transactionset.py
```

### Comparing `rpmdyn-2023.5.7.3/LICENSE` & `rpmdyn-2023.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7.3/PKG-INFO` & `rpmdyn-2023.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpmdyn
-Version: 2023.5.7.3
+Version: 2023.5.9
 Summary: Alternative dynamic RPM bindings for Python
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rpmdyn-2023.5.7.3/README.md` & `rpmdyn-2023.5.9/README.md`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7.3/custom_build/backend.py` & `rpmdyn-2023.5.9/custom_build/backend.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7.3/pyproject.toml` & `rpmdyn-2023.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7.3/src/rpmdyn/_const.py` & `rpmdyn-2023.5.9/src/rpmdyn/_const.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7.3/src/rpmdyn/_ffi.py` & `rpmdyn-2023.5.9/src/rpmdyn/_ffi.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7.3/src/rpmdyn/_pth_hook.py` & `rpmdyn-2023.5.9/src/rpmdyn/_pth_hook.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7.3/src/rpmdyn/_rpm.py` & `rpmdyn-2023.5.9/src/rpmdyn/_rpm.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7.3/src/rpmdyn/_transaction.py` & `rpmdyn-2023.5.9/src/rpmdyn/_transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,16 @@
     def __init__(self):
         self.__ts = gc(_ffi.rpmtsCreate(), _ffi.rpmtsFree)
 
         # native bindings set a default vsflags
         flags = _ffi.rpmExpandNumeric(cstr("%{?__vsflags}"))
         self.setVSFlags(flags)
 
-    # TODO: ts.setKeyring
+    def setKeyring(self, keyring):
+        return _ffi.rpmtsSetKeyring(self.__ts, keyring._keyring__kr if keyring else _ffi.NULL)
 
     def setVSFlags(self, flags):
         return _ffi.rpmtsSetVSFlags(self.__ts, flags)
 
     def getVSFlags(self):
         return _ffi.rpmtsVSFlags(self.__ts)
```

### Comparing `rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/PKG-INFO` & `rpmdyn-2023.5.9/src/rpmdyn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpmdyn
-Version: 2023.5.7.3
+Version: 2023.5.9
 Summary: Alternative dynamic RPM bindings for Python
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/SOURCES.txt` & `rpmdyn-2023.5.9/src/rpmdyn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7.3/tests/conftest.py` & `rpmdyn-2023.5.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7.3/tests/data/test-srpm01-1.0-1.src.rpm` & `rpmdyn-2023.5.9/tests/data/test-srpm01-1.0-1.src.rpm`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7.3/tests/data/walrus-5.21-1.noarch.rpm` & `rpmdyn-2023.5.9/tests/data/walrus-5.21-1.noarch.rpm`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7.3/tests/test_headers.py` & `rpmdyn-2023.5.9/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7.3/tests/test_labelcompare.py` & `rpmdyn-2023.5.9/tests/test_labelcompare.py`

 * *Files identical despite different names*

