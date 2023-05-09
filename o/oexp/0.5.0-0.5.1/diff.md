# Comparing `tmp/oexp-0.5.0.tar.gz` & `tmp/oexp-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.5.0.tar", last modified: Tue May  9 00:58:51 2023, max compression
+gzip compressed data, was "oexp-0.5.1.tar", last modified: Tue May  9 01:07:57 2023, max compression
```

## Comparing `oexp-0.5.0.tar` & `oexp-0.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 00:58:51.270355 oexp-0.5.0/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 00:58:51.270198 oexp-0.5.0/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.5.0/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 00:58:51.269379 oexp-0.5.0/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.5.0/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    71075 2023-05-09 00:41:31.000000 oexp-0.5.0/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-05-09 00:41:15.000000 oexp-0.5.0/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     5239 2023-05-09 00:57:49.000000 oexp-0.5.0/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 00:58:51.270023 oexp-0.5.0/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 00:58:51.000000 oexp-0.5.0/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      224 2023-05-09 00:58:51.000000 oexp-0.5.0/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-05-09 00:58:51.000000 oexp-0.5.0/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-05-09 00:58:51.000000 oexp-0.5.0/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-05-09 00:58:51.000000 oexp-0.5.0/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-05-09 00:58:46.000000 oexp-0.5.0/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-05-09 00:58:51.270398 oexp-0.5.0/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 01:07:57.741349 oexp-0.5.1/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 01:07:57.741185 oexp-0.5.1/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.5.1/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 01:07:57.740300 oexp-0.5.1/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.5.1/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    71075 2023-05-09 00:41:31.000000 oexp-0.5.1/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-05-09 00:41:15.000000 oexp-0.5.1/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     5401 2023-05-09 01:06:53.000000 oexp-0.5.1/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 01:07:57.741011 oexp-0.5.1/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 01:07:57.000000 oexp-0.5.1/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      224 2023-05-09 01:07:57.000000 oexp-0.5.1/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-05-09 01:07:57.000000 oexp-0.5.1/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-05-09 01:07:57.000000 oexp-0.5.1/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-05-09 01:07:57.000000 oexp-0.5.1/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-05-09 01:07:53.000000 oexp-0.5.1/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-05-09 01:07:57.741397 oexp-0.5.1/setup.cfg
```

### Comparing `oexp-0.5.0/oexp/access.py` & `oexp-0.5.1/oexp/access.py`

 * *Files identical despite different names*

### Comparing `oexp-0.5.0/oexp/jbridge.py` & `oexp-0.5.1/oexp/jbridge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-import subprocess
-
+import atexit
+import os
 import platform
-
-import urllib.request
 import socket
-import os
+import subprocess
+import urllib.request
 from typing import Optional
-import oexp.gen as gen
+
 import oexp.access as access
-import atexit
-import time
+import oexp.gen as gen
+
+system = platform.system()
 
 
 def _cpu():
-    if platform.system() == 'Linux':
+    if system == 'Linux':
         return subprocess.check_output(['uname', '-m']).decode().strip()
     else:
         return subprocess.check_output(['/usr/sbin/sysctl', 'machdep.cpu.brand_string']).decode().strip()
 
 
 def _user_data_dir():
     d = {
         'Darwin': lambda: os.path.join(os.path.expanduser('~'), 'Library', 'Application Support', 'oexp'),
         'Linux': lambda: os.path.join(os.path.expanduser('~'), '.oexp')
     }
-    system = platform.system()
     if system not in d:
-        raise Exception(f"TODO: implement user_data_dir for {platform.system()}")
+        raise Exception(f"TODO: implement user_data_dir for {system}")
     else:
         return d[system]()
 
 
 _initialized_java = False
 _jar_process = None
 _java_sock: Optional[socket.socket] = None
@@ -54,15 +53,18 @@
         platform_label = "macos-aarch64"
     elif cpu == "x86_64":
         platform_label = "linux-x64"
     else:
         raise Exception(f"need to figure out java for {cpu}")
 
     j_version = f"jdk-{gen.JAVA_VERSION}"
-    j_folder = os.path.join(data_dir, j_version + ".jdk")
+    if system == 'Linux':
+        j_folder = os.path.join(data_dir, j_version)
+    else:
+        j_folder = os.path.join(data_dir, j_version + ".jdk")
     tar_gz_folder = os.path.join(data_dir, "jdk.tar.gz")
     if not os.path.exists(tar_gz_folder):
         print("downloading java...")
         os.makedirs(data_dir, exist_ok=True)
         if os.path.exists(tar_gz_folder):
             os.remove(tar_gz_folder)
         #     https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html
@@ -111,17 +113,22 @@
         except:
             print(f"port {next_port_to_try} is being used, trying for _java_sock {next_port_to_try + 1} ")
             next_port_to_try += 1
     if not did_bind:
         raise Exception("could not bind socket 1")
     _java_sock.listen()
 
+    if system == 'Linux':
+        java = os.path.join(j_folder, "bin/java")
+    else:
+        java = os.path.join(j_folder, "Contents/Home/bin/java")
+
     _jar_process = subprocess.Popen(
         [
-            os.path.join(j_folder, "Contents/Home/bin/java"),
+            java,
             "-jar",
             jar_path,
             str(next_port_to_try)
         ],
     )
 
     _java_conn, addr = _java_sock.accept()
```

