# Comparing `tmp/oexp-0.4.0.tar.gz` & `tmp/oexp-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.4.0.tar", last modified: Tue May  9 00:44:49 2023, max compression
+gzip compressed data, was "oexp-0.5.0.tar", last modified: Tue May  9 00:58:51 2023, max compression
```

## Comparing `oexp-0.4.0.tar` & `oexp-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 00:44:49.523398 oexp-0.4.0/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 00:44:49.523232 oexp-0.4.0/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.4.0/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 00:44:49.522352 oexp-0.4.0/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.4.0/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    71075 2023-05-09 00:41:31.000000 oexp-0.4.0/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-05-09 00:41:15.000000 oexp-0.4.0/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     4894 2023-05-09 00:44:28.000000 oexp-0.4.0/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 00:44:49.523060 oexp-0.4.0/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 00:44:49.000000 oexp-0.4.0/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      224 2023-05-09 00:44:49.000000 oexp-0.4.0/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-05-09 00:44:49.000000 oexp-0.4.0/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-05-09 00:44:49.000000 oexp-0.4.0/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-05-09 00:44:49.000000 oexp-0.4.0/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-05-09 00:44:44.000000 oexp-0.4.0/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-05-09 00:44:49.523443 oexp-0.4.0/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 00:58:51.270355 oexp-0.5.0/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 00:58:51.270198 oexp-0.5.0/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.5.0/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 00:58:51.269379 oexp-0.5.0/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.5.0/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    71075 2023-05-09 00:41:31.000000 oexp-0.5.0/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-05-09 00:41:15.000000 oexp-0.5.0/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     5239 2023-05-09 00:57:49.000000 oexp-0.5.0/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 00:58:51.270023 oexp-0.5.0/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 00:58:51.000000 oexp-0.5.0/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      224 2023-05-09 00:58:51.000000 oexp-0.5.0/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-05-09 00:58:51.000000 oexp-0.5.0/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-05-09 00:58:51.000000 oexp-0.5.0/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-05-09 00:58:51.000000 oexp-0.5.0/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-05-09 00:58:46.000000 oexp-0.5.0/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-05-09 00:58:51.270398 oexp-0.5.0/setup.cfg
```

### Comparing `oexp-0.4.0/oexp/access.py` & `oexp-0.5.0/oexp/access.py`

 * *Files identical despite different names*

### Comparing `oexp-0.4.0/oexp/jbridge.py` & `oexp-0.5.0/oexp/jbridge.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 import oexp.gen as gen
 import oexp.access as access
 import atexit
 import time
 
 
 def _cpu():
-    return subprocess.check_output(['/usr/sbin/sysctl', 'machdep.cpu.brand_string']).decode().strip()
+    if platform.system() == 'Linux':
+        return subprocess.check_output(['uname', '-m']).decode().strip()
+    else:
+        return subprocess.check_output(['/usr/sbin/sysctl', 'machdep.cpu.brand_string']).decode().strip()
 
 
 def _user_data_dir():
     d = {
         'Darwin': lambda: os.path.join(os.path.expanduser('~'), 'Library', 'Application Support', 'oexp'),
         'Linux': lambda: os.path.join(os.path.expanduser('~'), '.oexp')
     }
@@ -41,27 +44,35 @@
 # https://docs.python.org/3/library/importlib.resources.html#module-importlib.resources
 def _init_java():
     global _java_sock, _jar_process, _java_exit_sock, _java_conn, _java_exit_conn
     if _java_sock is not None:
         return
 
     data_dir = _user_data_dir()
-    if _cpu() != "machdep.cpu.brand_string: Apple M1 Max":
-        raise Exception(f"need to figure out java for {_cpu()}")
+
+    cpu = _cpu()
+    if cpu == "machdep.cpu.brand_string: Apple M1 Max":
+        platform_label = "macos-aarch64"
+    elif cpu == "x86_64":
+        platform_label = "linux-x64"
+    else:
+        raise Exception(f"need to figure out java for {cpu}")
 
     j_version = f"jdk-{gen.JAVA_VERSION}"
     j_folder = os.path.join(data_dir, j_version + ".jdk")
     tar_gz_folder = os.path.join(data_dir, "jdk.tar.gz")
     if not os.path.exists(tar_gz_folder):
         print("downloading java...")
         os.makedirs(data_dir, exist_ok=True)
         if os.path.exists(tar_gz_folder):
             os.remove(tar_gz_folder)
+        #     https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html
+
         urllib.request.urlretrieve(
-            f"https://download.oracle.com/java/17/archive/jdk-{gen.JAVA_VERSION}_macos-aarch64_bin.tar.gz",
+            f"https://download.oracle.com/java/17/archive/jdk-{gen.JAVA_VERSION}_{platform_label}_bin.tar.gz",
             tar_gz_folder
         )
         subprocess.run(
             [
                 "/usr/bin/tar", "-xf",
                 tar_gz_folder
             ],
```

