# Comparing `tmp/garatool-0.1683655042.0.tar.gz` & `tmp/garatool-0.1683657432.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683655042.0.tar", last modified: Tue May  9 17:57:22 2023, max compression
+gzip compressed data, was "garatool-0.1683657432.0.tar", last modified: Tue May  9 18:37:12 2023, max compression
```

## Comparing `garatool-0.1683655042.0.tar` & `garatool-0.1683657432.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:57:22.352327 garatool-0.1683655042.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:57:22.352052 garatool-0.1683655042.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683655042.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:57:22.349347 garatool-0.1683655042.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)     5759 2023-05-09 17:56:22.000000 garatool-0.1683655042.0/garatool/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683655042.0/garatool/__main__.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:57:22.351619 garatool-0.1683655042.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:57:22.000000 garatool-0.1683655042.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 17:57:22.000000 garatool-0.1683655042.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 17:57:22.000000 garatool-0.1683655042.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 17:57:22.000000 garatool-0.1683655042.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 17:57:22.000000 garatool-0.1683655042.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 17:57:22.352420 garatool-0.1683655042.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683655042.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 18:37:12.385780 garatool-0.1683657432.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 18:37:12.385486 garatool-0.1683657432.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683657432.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 18:37:12.382584 garatool-0.1683657432.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)     6005 2023-05-09 18:22:07.000000 garatool-0.1683657432.0/garatool/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683657432.0/garatool/__main__.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 18:37:12.384972 garatool-0.1683657432.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 18:37:12.000000 garatool-0.1683657432.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 18:37:12.000000 garatool-0.1683657432.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 18:37:12.000000 garatool-0.1683657432.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 18:37:12.000000 garatool-0.1683657432.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 18:37:12.000000 garatool-0.1683657432.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 18:37:12.385873 garatool-0.1683657432.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683657432.0/setup.py
```

### Comparing `garatool-0.1683655042.0/garatool/__init__.py` & `garatool-0.1683657432.0/garatool/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 parser.add_argument('-t', '--tag', type=str, help="Select firmware tag", default='dev')
 parser.add_argument('-i', '--imei', type=str, help='IMEI code', default='NOIMEI')
 parser.add_argument('-n', '--name', help='Device name', default='Creator Device')
 parser.add_argument('-s', '--serial', action='store_true', help='Enable Serial debug')
 parser.add_argument('-u', '--upload', help='(Admin) Publish firmware tag',action='store_true')
 parser.add_argument('-k', '--key', help='(Admin) With secret key', default='')
 parser.add_argument('-r', '--root', help='(Admin) Location of firmware', default='')
-
+parser.add_argument('-d', '--download', help="(Admin) Download tagged firmware", action='store_true')
 
 def get_mac(port: str, nostub: bool) -> str:
     output = subprocess.getoutput(
         cmd(' '.join([
             ESPTOOL,
             '-p', port,
             '--no-stub' if  nostub else ' ',
@@ -158,16 +158,22 @@
 
     for parti in br.partitions:
         try:
             os.remove(parti['file'])
         except OSError:
             pass
 
+def download_tag(tag: str, key: str):
+    req = requests.post(
+        url = 'https://api.garastem.com/api/v1/toolchain/garatool',
 
+    )
+    
 def start():
+    
     br = BuildRequest()
     br.event = 'build_firmware'
     br.name = parsed.name
     br.imei = parsed.imei
     br.tag = parsed.tag
     br.key = parsed.key
     br.upload = parsed.upload
@@ -206,10 +212,10 @@
 
 
     br = request_firmware_build(br)
     # Start burning firmware
     program_device(br)
 
     if parsed.serial:
-        if platform.platform() == 'darwin':
+        if platform.system() == 'Darwin':
             os.system('say start')
             os.system(f'screen {parsed.port} 115200')
```

### Comparing `garatool-0.1683655042.0/setup.py` & `garatool-0.1683657432.0/setup.py`

 * *Files identical despite different names*

