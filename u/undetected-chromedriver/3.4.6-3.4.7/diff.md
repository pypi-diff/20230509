# Comparing `tmp/undetected-chromedriver-3.4.6.tar.gz` & `tmp/undetected-chromedriver-3.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undetected-chromedriver-3.4.6.tar", last modified: Fri Feb 10 18:27:49 2023, max compression
+gzip compressed data, was "undetected-chromedriver-3.4.7.tar", last modified: Tue May  9 20:27:03 2023, max compression
```

## Comparing `undetected-chromedriver-3.4.6.tar` & `undetected-chromedriver-3.4.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 18:27:49.603393 undetected-chromedriver-3.4.6/
--rw-rw-rw-   0        0        0    35823 2023-02-04 15:47:40.000000 undetected-chromedriver-3.4.6/LICENSE
--rw-rw-rw-   0        0        0    76699 2023-02-10 18:27:49.602893 undetected-chromedriver-3.4.6/PKG-INFO
--rw-rw-rw-   0        0        0    75683 2023-02-10 18:17:15.000000 undetected-chromedriver-3.4.6/README.md
--rw-rw-rw-   0        0        0       42 2023-02-10 18:27:49.603393 undetected-chromedriver-3.4.6/setup.cfg
--rw-rw-rw-   0        0        0     2670 2023-02-05 14:13:45.000000 undetected-chromedriver-3.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-10 18:27:49.596893 undetected-chromedriver-3.4.6/undetected_chromedriver/
--rw-rw-rw-   0        0        0    33704 2023-02-10 18:27:29.000000 undetected-chromedriver-3.4.6/undetected_chromedriver/__init__.py
--rw-rw-rw-   0        0        0     3498 2023-02-04 20:52:44.000000 undetected-chromedriver-3.4.6/undetected_chromedriver/cdp.py
--rw-rw-rw-   0        0        0     5937 2023-02-04 20:52:44.000000 undetected-chromedriver-3.4.6/undetected_chromedriver/devtool.py
--rw-rw-rw-   0        0        0     1837 2023-02-05 14:13:45.000000 undetected-chromedriver-3.4.6/undetected_chromedriver/dprocess.py
--rw-rw-rw-   0        0        0     2751 2023-02-05 14:13:45.000000 undetected-chromedriver-3.4.6/undetected_chromedriver/options.py
--rw-rw-rw-   0        0        0     9697 2023-02-10 18:18:17.000000 undetected-chromedriver-3.4.6/undetected_chromedriver/patcher.py
--rw-rw-rw-   0        0        0     3065 2023-02-05 14:13:45.000000 undetected-chromedriver-3.4.6/undetected_chromedriver/reactor.py
--rw-rw-rw-   0        0        0     2900 2023-02-05 14:13:45.000000 undetected-chromedriver-3.4.6/undetected_chromedriver/webelement.py
-drwxrwxrwx   0        0        0        0 2023-02-10 18:27:49.601393 undetected-chromedriver-3.4.6/undetected_chromedriver.egg-info/
--rw-rw-rw-   0        0        0    76699 2023-02-10 18:27:49.000000 undetected-chromedriver-3.4.6/undetected_chromedriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      541 2023-02-10 18:27:49.000000 undetected-chromedriver-3.4.6/undetected_chromedriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 18:27:49.000000 undetected-chromedriver-3.4.6/undetected_chromedriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-02-10 18:27:49.000000 undetected-chromedriver-3.4.6/undetected_chromedriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-02-10 18:27:49.000000 undetected-chromedriver-3.4.6/undetected_chromedriver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 20:27:03.496985 undetected-chromedriver-3.4.7/
+-rw-rw-rw-   0        0        0    35823 2023-02-04 20:28:40.000000 undetected-chromedriver-3.4.7/LICENSE
+-rw-rw-rw-   0        0        0    76699 2023-05-09 20:27:03.495982 undetected-chromedriver-3.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0    75683 2023-05-09 16:23:12.000000 undetected-chromedriver-3.4.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 20:27:03.496985 undetected-chromedriver-3.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     2670 2023-05-09 16:23:12.000000 undetected-chromedriver-3.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:27:03.462915 undetected-chromedriver-3.4.7/undetected_chromedriver/
+-rw-rw-rw-   0        0        0    34297 2023-05-09 20:19:13.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/__init__.py
+-rw-rw-rw-   0        0        0     3498 2023-02-04 20:28:40.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/cdp.py
+-rw-rw-rw-   0        0        0     5937 2023-02-04 20:28:40.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/devtool.py
+-rw-rw-rw-   0        0        0     1837 2023-05-09 16:23:12.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/dprocess.py
+-rw-rw-rw-   0        0        0     2751 2023-05-09 16:23:12.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/options.py
+-rw-rw-rw-   0        0        0    11782 2023-05-09 20:10:37.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/patcher.py
+-rw-rw-rw-   0        0        0     3065 2023-05-09 16:23:12.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/reactor.py
+-rw-rw-rw-   0        0        0     2900 2023-05-09 16:23:12.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/webelement.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:27:03.483421 undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/
+-rw-rw-rw-   0        0        0    76699 2023-05-09 20:27:02.000000 undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      541 2023-05-09 20:27:03.000000 undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 20:27:02.000000 undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-09 20:27:03.000000 undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-09 20:27:03.000000 undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/top_level.txt
```

### Comparing `undetected-chromedriver-3.4.6/LICENSE` & `undetected-chromedriver-3.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.4.6/PKG-INFO` & `undetected-chromedriver-3.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: undetected-chromedriver
-Version: 3.4.6
+Version: 3.4.7
 Summary: ('Selenium.webdriver.Chrome replacement with compatiblity for Brave, and other Chromium based browsers.', 'Not triggered by CloudFlare/Imperva/hCaptcha and such.', 'NOTE: results may vary due to many factors. No guarantees are given, except for ongoing efforts in understanding detection algorithms.')
 Home-page: https://github.com/ultrafunkamsterdam/undetected-chromedriver
 Author: UltrafunkAmsterdam
 Author-email: info@blackhat-security.nl
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `undetected-chromedriver-3.4.6/README.md` & `undetected-chromedriver-3.4.7/README.md`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.4.6/setup.py` & `undetected-chromedriver-3.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.4.6/undetected_chromedriver/__init__.py` & `undetected-chromedriver-3.4.7/undetected_chromedriver/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 by UltrafunkAmsterdam (https://github.com/ultrafunkamsterdam)
 
 """
 from __future__ import annotations
 
 
-__version__ = "3.4.6"
+__version__ = "3.4.7"
 
 import json
 import logging
 import os
 import re
 import shutil
 import subprocess
@@ -119,14 +119,15 @@
         headless=False,
         version_main=None,
         patcher_force_close=False,
         suppress_welcome=True,
         use_subprocess=True,
         debug=False,
         no_sandbox=True,
+        user_multi_procs: bool = False,
         **kw,
     ):
         """
         Creates a new instance of the chrome driver.
 
         Starts the service and then creates new instance of chrome driver.
 
@@ -230,24 +231,35 @@
               in that case you can set this to `True`. The browser will start via subprocess, and will keep running most of times.
               ! setting it to True comes with NO support when being detected. !
 
         no_sandbox: bool, optional, default=True
              uses the --no-sandbox option, and additionally does suppress the "unsecure option" status bar
              this option has a default of True since many people seem to run this as root (....) , and chrome does not start
              when running as root without using --no-sandbox flag.
+
+        user_multi_procs:
+            set to true when you are using multithreads/multiprocessing
+            ensures not all processes are trying to modify a binary which is in use by another.
+            for this to work. YOU MUST HAVE AT LEAST 1 UNDETECTED_CHROMEDRIVER BINARY IN YOUR ROAMING DATA FOLDER.
+            this requirement can be easily satisfied, by just running this program "normal" and close/kill it.
+
+
         """
 
         finalize(self, self._ensure_close, self)
         self.debug = debug
         self.patcher = Patcher(
             executable_path=driver_executable_path,
             force=patcher_force_close,
             version_main=version_main,
+            user_multi_procs=user_multi_procs,
         )
+        # self.patcher.auto(user_multiprocess = user_multi_num_procs)
         self.patcher.auto()
+
         # self.patcher = patcher
         if not options:
             options = ChromeOptions()
 
         try:
             if hasattr(options, "_session") and options._session is not None:
                 #  prevent reuse of options,
```

### Comparing `undetected-chromedriver-3.4.6/undetected_chromedriver/cdp.py` & `undetected-chromedriver-3.4.7/undetected_chromedriver/cdp.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.4.6/undetected_chromedriver/devtool.py` & `undetected-chromedriver-3.4.7/undetected_chromedriver/devtool.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.4.6/undetected_chromedriver/dprocess.py` & `undetected-chromedriver-3.4.7/undetected_chromedriver/dprocess.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.4.6/undetected_chromedriver/options.py` & `undetected-chromedriver-3.4.7/undetected_chromedriver/options.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.4.6/undetected_chromedriver/patcher.py` & `undetected-chromedriver-3.4.7/undetected_chromedriver/patcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 #!/usr/bin/env python3
 # this module is part of undetected_chromedriver
 
 from distutils.version import LooseVersion
 import io
 import logging
 import os
+import pathlib
 import random
 import re
+import shutil
 import string
 import sys
 import time
 from urllib.request import urlopen
 from urllib.request import urlretrieve
 import zipfile
-
+from multiprocessing import Lock
 
 logger = logging.getLogger(__name__)
 
 IS_POSIX = sys.platform.startswith(("darwin", "cygwin", "linux", "linux2"))
 
 
 class Patcher(object):
+    lock = Lock()
     url_repo = "https://chromedriver.storage.googleapis.com"
     zip_name = "chromedriver_%s.zip"
     exe_name = "chromedriver%s"
 
     platform = sys.platform
     if platform.endswith("win32"):
         zip_name %= "win32"
@@ -44,27 +47,34 @@
         d = "~/.local/share/undetected_chromedriver"
     elif platform.endswith("darwin"):
         d = "~/Library/Application Support/undetected_chromedriver"
     else:
         d = "~/.undetected_chromedriver"
     data_path = os.path.abspath(os.path.expanduser(d))
 
-    def __init__(self, executable_path=None, force=False, version_main: int = 0):
+    def __init__(
+        self,
+        executable_path=None,
+        force=False,
+        version_main: int = 0,
+        user_multi_procs=False,
+    ):
         """
         Args:
             executable_path: None = automatic
                              a full file path to the chromedriver executable
             force: False
                     terminate processes which are holding lock
             version_main: 0 = auto
                 specify main chrome version (rounded, ex: 82)
         """
         self.force = force
         self._custom_exe_path = False
         prefix = "undetected"
+        self.user_multi_procs = user_multi_procs
 
         if not os.path.exists(self.data_path):
             os.makedirs(self.data_path, exist_ok=True)
 
         if not executable_path:
             self.executable_path = os.path.join(
                 self.data_path, "_".join([prefix, self.exe_name])
@@ -74,25 +84,49 @@
             if executable_path:
                 if not executable_path[-4:] == ".exe":
                     executable_path += ".exe"
 
         self.zip_path = os.path.join(self.data_path, prefix)
 
         if not executable_path:
-            self.executable_path = os.path.abspath(
-                os.path.join(".", self.executable_path)
-            )
+            if not self.user_multi_procs:
+                self.executable_path = os.path.abspath(
+                    os.path.join(".", self.executable_path)
+                )
 
         if executable_path:
             self._custom_exe_path = True
             self.executable_path = executable_path
+
         self.version_main = version_main
         self.version_full = None
 
-    def auto(self, executable_path=None, force=False, version_main=None):
+    def auto(self, executable_path=None, force=False, version_main=None, _=None):
+        """
+
+        Args:
+            executable_path:
+            force:
+            version_main:
+
+        Returns:
+
+        """
+        # if self.user_multi_procs and \
+        #         self.user_multi_procs != -1:
+        #     # -1 being a skip value used later in this block
+        #
+        p = pathlib.Path(self.data_path)
+        with Lock():
+            files = list(p.rglob("*chromedriver*?"))
+            for file in files:
+                if self.is_binary_patched(file):
+                    self.executable_path = str(file)
+                    return True
+
         if executable_path:
             self.executable_path = executable_path
             self._custom_exe_path = True
 
         if self._custom_exe_path:
             ispatched = self.is_binary_patched(self.executable_path)
             if not ispatched:
@@ -123,14 +157,57 @@
 
         release = self.fetch_release_number()
         self.version_main = release.version[0]
         self.version_full = release
         self.unzip_package(self.fetch_package())
         return self.patch()
 
+    def driver_binary_in_use(self, path: str = None) -> bool:
+        """
+        naive test to check if a found chromedriver binary is
+        currently in use
+
+        Args:
+            path: a string or PathLike object to the binary to check.
+                  if not specified, we check use this object's executable_path
+        """
+        if not path:
+            path = self.executable_path
+        p = pathlib.Path(path)
+
+        if not p.exists():
+            raise OSError("file does not exist: %s" % p)
+        try:
+            with open(p, mode="a+b") as fs:
+                exc = []
+                try:
+
+                    fs.seek(0, 0)
+                except PermissionError as e:
+                    exc.append(e)  # since some systems apprently allow seeking
+                    # we conduct another test
+                try:
+                    fs.readline()
+                except PermissionError as e:
+                    exc.append(e)
+
+                if exc:
+
+                    return True
+                return False
+            # ok safe to assume this is in use
+        except Exception as e:
+            # logger.exception("whoops ", e)
+            pass
+
+    def cleanup_unused_files(self):
+        p = pathlib.Path(self.data_path)
+        items = list(p.glob("*undetected*"))
+        print(items)
+
     def patch(self):
         self.patch_exe()
         return self.is_binary_patched()
 
     def fetch_release_number(self):
         """
         Gets the latest major version available, or the latest major version of self.target_version if set explicitly.
@@ -251,25 +328,21 @@
         if self._custom_exe_path:
             # if the driver binary is specified by user
             # we assume it is important enough to not delete it
             return
         else:
             timeout = 3  # stop trying after this many seconds
             t = time.monotonic()
-            while True:
-                now = time.monotonic()
-                if now - t > timeout:
-                    # we don't want to wait until the end of time
-                    logger.debug(
-                        "could not unlink %s in time (%d seconds)"
-                        % (self.executable_path, timeout)
-                    )
-                    break
+            now = lambda: time.monotonic()
+            while now() - t > timeout:
+                # we don't want to wait until the end of time
                 try:
+                    if self.user_multi_procs:
+                        break
                     os.unlink(self.executable_path)
                     logger.debug("successfully unlinked %s" % self.executable_path)
                     break
                 except (OSError, RuntimeError, PermissionError):
-                    time.sleep(0.1)
+                    time.sleep(0.01)
                     continue
                 except FileNotFoundError:
                     break
```

### Comparing `undetected-chromedriver-3.4.6/undetected_chromedriver/reactor.py` & `undetected-chromedriver-3.4.7/undetected_chromedriver/reactor.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.4.6/undetected_chromedriver/webelement.py` & `undetected-chromedriver-3.4.7/undetected_chromedriver/webelement.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.4.6/undetected_chromedriver.egg-info/PKG-INFO` & `undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: undetected-chromedriver
-Version: 3.4.6
+Version: 3.4.7
 Summary: ('Selenium.webdriver.Chrome replacement with compatiblity for Brave, and other Chromium based browsers.', 'Not triggered by CloudFlare/Imperva/hCaptcha and such.', 'NOTE: results may vary due to many factors. No guarantees are given, except for ongoing efforts in understanding detection algorithms.')
 Home-page: https://github.com/ultrafunkamsterdam/undetected-chromedriver
 Author: UltrafunkAmsterdam
 Author-email: info@blackhat-security.nl
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `undetected-chromedriver-3.4.6/undetected_chromedriver.egg-info/SOURCES.txt` & `undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

