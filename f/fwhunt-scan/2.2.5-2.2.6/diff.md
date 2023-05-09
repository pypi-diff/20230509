# Comparing `tmp/fwhunt_scan-2.2.5.tar.gz` & `tmp/fwhunt_scan-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fwhunt_scan-2.2.5.tar", last modified: Sat May  6 19:49:33 2023, max compression
+gzip compressed data, was "fwhunt_scan-2.2.6.tar", last modified: Tue May  9 10:56:23 2023, max compression
```

## Comparing `fwhunt_scan-2.2.5.tar` & `fwhunt_scan-2.2.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-06 19:49:33.727982 fwhunt_scan-2.2.5/
--rw-r--r--   0 yv         (501) staff       (20)    35149 2022-04-11 15:38:46.000000 fwhunt_scan-2.2.5/LICENSE
--rw-r--r--   0 yv         (501) staff       (20)     4302 2023-05-06 19:49:33.728029 fwhunt_scan-2.2.5/PKG-INFO
--rw-r--r--   0 yv         (501) staff       (20)     3728 2023-03-17 22:44:15.000000 fwhunt_scan-2.2.5/README.md
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-06 19:49:33.726987 fwhunt_scan-2.2.5/fwhunt_scan/
--rw-r--r--   0 yv         (501) staff       (20)      615 2023-05-06 19:46:06.000000 fwhunt_scan-2.2.5/fwhunt_scan/__init__.py
--rw-r--r--   0 yv         (501) staff       (20)      362 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/__init__.pyi
--rw-r--r--   0 yv         (501) staff       (20)       64 2022-04-11 15:38:46.000000 fwhunt_scan-2.2.5/fwhunt_scan/py.typed
--rw-r--r--   0 yv         (501) staff       (20)      817 2023-02-20 11:45:24.000000 fwhunt_scan-2.2.5/fwhunt_scan/test_internal.py
--rw-r--r--   0 yv         (501) staff       (20)    27550 2022-10-11 01:00:17.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_analyzer.py
--rw-r--r--   0 yv         (501) staff       (20)     2686 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_analyzer.pyi
--rw-r--r--   0 yv         (501) staff       (20)     5237 2023-02-20 13:44:10.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_extractor.py
--rw-r--r--   0 yv         (501) staff       (20)   304114 2022-05-30 08:29:58.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_protocols.py
--rw-r--r--   0 yv         (501) staff       (20)      218 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_protocols.pyi
--rw-r--r--   0 yv         (501) staff       (20)    36316 2023-03-06 19:27:41.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_scanner.py
--rw-r--r--   0 yv         (501) staff       (20)     2634 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_scanner.pyi
--rw-r--r--   0 yv         (501) staff       (20)     9985 2022-09-20 15:07:51.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_smm.py
--rw-r--r--   0 yv         (501) staff       (20)     1337 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_smm.pyi
--rw-r--r--   0 yv         (501) staff       (20)     5596 2022-05-30 08:30:06.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_tables.py
--rw-r--r--   0 yv         (501) staff       (20)      280 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_tables.pyi
--rw-r--r--   0 yv         (501) staff       (20)     3035 2022-07-27 15:10:58.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_te.py
--rw-r--r--   0 yv         (501) staff       (20)      727 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_te.pyi
--rw-r--r--   0 yv         (501) staff       (20)     3875 2022-04-13 18:03:37.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_types.py
--rw-r--r--   0 yv         (501) staff       (20)     1596 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_types.pyi
--rw-r--r--   0 yv         (501) staff       (20)     2112 2022-07-15 12:35:57.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_utils.py
--rw-r--r--   0 yv         (501) staff       (20)      418 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_utils.pyi
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-06 19:49:33.727662 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/
--rw-r--r--   0 yv         (501) staff       (20)     4302 2023-05-06 19:49:33.000000 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/PKG-INFO
--rw-r--r--   0 yv         (501) staff       (20)      888 2023-05-06 19:49:33.000000 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/SOURCES.txt
--rw-r--r--   0 yv         (501) staff       (20)        1 2023-05-06 19:49:33.000000 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/dependency_links.txt
--rw-r--r--   0 yv         (501) staff       (20)        1 2022-05-30 08:58:37.000000 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/not-zip-safe
--rw-r--r--   0 yv         (501) staff       (20)      127 2023-05-06 19:49:33.000000 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/requires.txt
--rw-r--r--   0 yv         (501) staff       (20)       12 2023-05-06 19:49:33.000000 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/top_level.txt
--rw-r--r--   0 yv         (501) staff       (20)     7250 2023-05-06 19:42:48.000000 fwhunt_scan-2.2.5/fwhunt_scan_analyzer.py
--rw-r--r--   0 yv         (501) staff       (20)     3860 2023-03-17 22:40:12.000000 fwhunt_scan-2.2.5/fwhunt_scan_docker.py
--rw-r--r--   0 yv         (501) staff       (20)      116 2023-05-06 19:49:33.728199 fwhunt_scan-2.2.5/setup.cfg
--rw-r--r--   0 yv         (501) staff       (20)     1408 2023-02-20 17:31:56.000000 fwhunt_scan-2.2.5/setup.py
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-06 19:49:33.727872 fwhunt_scan-2.2.5/test/
--rw-r--r--   0 yv         (501) staff       (20)     1208 2022-05-30 08:09:52.000000 fwhunt_scan-2.2.5/test/test.py
--rw-r--r--   0 yv         (501) staff       (20)      230 2022-08-03 15:21:16.000000 fwhunt_scan-2.2.5/test/test_variants.py
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-09 10:56:23.087656 fwhunt_scan-2.2.6/
+-rw-r--r--   0 yv         (501) staff       (20)    35149 2022-04-11 15:38:46.000000 fwhunt_scan-2.2.6/LICENSE
+-rw-r--r--   0 yv         (501) staff       (20)     4302 2023-05-09 10:56:23.087706 fwhunt_scan-2.2.6/PKG-INFO
+-rw-r--r--   0 yv         (501) staff       (20)     3728 2023-03-17 22:44:15.000000 fwhunt_scan-2.2.6/README.md
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-09 10:56:23.086642 fwhunt_scan-2.2.6/fwhunt_scan/
+-rw-r--r--   0 yv         (501) staff       (20)      615 2023-05-09 10:54:32.000000 fwhunt_scan-2.2.6/fwhunt_scan/__init__.py
+-rw-r--r--   0 yv         (501) staff       (20)      362 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/__init__.pyi
+-rw-r--r--   0 yv         (501) staff       (20)       64 2022-04-11 15:38:46.000000 fwhunt_scan-2.2.6/fwhunt_scan/py.typed
+-rw-r--r--   0 yv         (501) staff       (20)      817 2023-02-20 11:45:24.000000 fwhunt_scan-2.2.6/fwhunt_scan/test_internal.py
+-rw-r--r--   0 yv         (501) staff       (20)    27487 2023-05-09 10:54:10.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_analyzer.py
+-rw-r--r--   0 yv         (501) staff       (20)     2686 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_analyzer.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     5237 2023-02-20 13:44:10.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_extractor.py
+-rw-r--r--   0 yv         (501) staff       (20)   304114 2022-05-30 08:29:58.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_protocols.py
+-rw-r--r--   0 yv         (501) staff       (20)      218 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_protocols.pyi
+-rw-r--r--   0 yv         (501) staff       (20)    36316 2023-03-06 19:27:41.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_scanner.py
+-rw-r--r--   0 yv         (501) staff       (20)     2634 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_scanner.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     9985 2022-09-20 15:07:51.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_smm.py
+-rw-r--r--   0 yv         (501) staff       (20)     1337 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_smm.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     5596 2022-05-30 08:30:06.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_tables.py
+-rw-r--r--   0 yv         (501) staff       (20)      280 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_tables.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     3035 2022-07-27 15:10:58.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_te.py
+-rw-r--r--   0 yv         (501) staff       (20)      727 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_te.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     3875 2022-04-13 18:03:37.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_types.py
+-rw-r--r--   0 yv         (501) staff       (20)     1596 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_types.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     2112 2022-07-15 12:35:57.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_utils.py
+-rw-r--r--   0 yv         (501) staff       (20)      418 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_utils.pyi
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-09 10:56:23.087317 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/
+-rw-r--r--   0 yv         (501) staff       (20)     4302 2023-05-09 10:56:23.000000 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/PKG-INFO
+-rw-r--r--   0 yv         (501) staff       (20)      888 2023-05-09 10:56:23.000000 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/SOURCES.txt
+-rw-r--r--   0 yv         (501) staff       (20)        1 2023-05-09 10:56:23.000000 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/dependency_links.txt
+-rw-r--r--   0 yv         (501) staff       (20)        1 2022-05-30 08:58:37.000000 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/not-zip-safe
+-rw-r--r--   0 yv         (501) staff       (20)      127 2023-05-09 10:56:23.000000 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/requires.txt
+-rw-r--r--   0 yv         (501) staff       (20)       12 2023-05-09 10:56:23.000000 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/top_level.txt
+-rw-r--r--   0 yv         (501) staff       (20)     7250 2023-05-08 17:59:45.000000 fwhunt_scan-2.2.6/fwhunt_scan_analyzer.py
+-rw-r--r--   0 yv         (501) staff       (20)     3860 2023-03-17 22:40:12.000000 fwhunt_scan-2.2.6/fwhunt_scan_docker.py
+-rw-r--r--   0 yv         (501) staff       (20)      116 2023-05-09 10:56:23.087889 fwhunt_scan-2.2.6/setup.cfg
+-rw-r--r--   0 yv         (501) staff       (20)     1408 2023-02-20 17:31:56.000000 fwhunt_scan-2.2.6/setup.py
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-09 10:56:23.087538 fwhunt_scan-2.2.6/test/
+-rw-r--r--   0 yv         (501) staff       (20)     1208 2022-05-30 08:09:52.000000 fwhunt_scan-2.2.6/test/test.py
+-rw-r--r--   0 yv         (501) staff       (20)      230 2022-08-03 15:21:16.000000 fwhunt_scan-2.2.6/test/test_variants.py
```

### Comparing `fwhunt_scan-2.2.5/LICENSE` & `fwhunt_scan-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/PKG-INFO` & `fwhunt_scan-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwhunt_scan
-Version: 2.2.5
+Version: 2.2.6
 Summary: Tools for analyzing UEFI firmware and checking UEFI modules with FwHunt rules
 Home-page: https://github.com/binarly-io/fwhunt-scan
 Author: FwHunt team
 Author-email: fwhunt@binarly.io
 License: GPL-3.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fwhunt_scan-2.2.5/README.md` & `fwhunt_scan-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/__init__.py` & `fwhunt_scan-2.2.6/fwhunt_scan/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 Tools for analyzing UEFI firmware and checking UEFI modules with FwHunt rules
 """
 
 __author__ = "FwHunt team"
 __email__ = "fwhunt@binarly.io"
-__version__ = "2.2.5"
+__version__ = "2.2.6"
 
 from .uefi_analyzer import UefiAnalyzer, UefiAnalyzerError
 from .uefi_scanner import UefiRule, UefiScanner, UefiScannerError
 from .uefi_te import TerseExecutableParser
 from .uefi_extractor import UefiBinary, UefiExtractor
 
 __all__ = [
```

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/test_internal.py` & `fwhunt_scan-2.2.6/fwhunt_scan/test_internal.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_analyzer.py` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,25 +80,24 @@
                     self._rz.cmd("aaaa")
             try:
                 self._te = TerseExecutableParser(image_path=image_path)
             except TerseExecutableError:
                 self._te = None
 
         if blob and sys.platform in ["linux"]:
-            if blob[:2] not in [b"MZ", b"VZ"]:
-                raise UefiAnalyzerError("Invalid data format")
             blob_size = len(blob)
             self._shm = shared_memory.SharedMemory(create=True, size=blob_size)
             self._shm.buf[:] = blob[:]
             self._rz = rzpipe.open(
                 filename=f"shm://{self._shm.name}/{blob_size:#d}",
                 flags=["-2"],
                 rizin_home=rizinhome,
             )
-            self._rz.cmd("aaaa")
+            if blob[:2] in [b"MZ", b"VZ"]:
+                self._rz.cmd("aaaa")
             try:
                 self._te = TerseExecutableParser(blob=blob)
             except TerseExecutableError:
                 self._te = None
 
         if self._rz is None:
             raise UefiAnalyzerError(
```

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_analyzer.pyi` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_analyzer.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_extractor.py` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_extractor.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_protocols.py` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_protocols.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_scanner.py` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_scanner.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_scanner.pyi` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_scanner.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_smm.py` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_smm.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_smm.pyi` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_smm.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_tables.py` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_tables.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_te.py` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_te.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_te.pyi` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_te.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_types.py` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_types.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_types.pyi` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_types.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan/uefi_utils.py` & `fwhunt_scan-2.2.6/fwhunt_scan/uefi_utils.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan.egg-info/PKG-INFO` & `fwhunt_scan-2.2.6/fwhunt_scan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwhunt-scan
-Version: 2.2.5
+Version: 2.2.6
 Summary: Tools for analyzing UEFI firmware and checking UEFI modules with FwHunt rules
 Home-page: https://github.com/binarly-io/fwhunt-scan
 Author: FwHunt team
 Author-email: fwhunt@binarly.io
 License: GPL-3.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan.egg-info/SOURCES.txt` & `fwhunt_scan-2.2.6/fwhunt_scan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan_analyzer.py` & `fwhunt_scan-2.2.6/fwhunt_scan_analyzer.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/fwhunt_scan_docker.py` & `fwhunt_scan-2.2.6/fwhunt_scan_docker.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/setup.py` & `fwhunt_scan-2.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.5/test/test.py` & `fwhunt_scan-2.2.6/test/test.py`

 * *Files identical despite different names*

