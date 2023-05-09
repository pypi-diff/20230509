# Comparing `tmp/garaprod-0.1683618340.0.tar.gz` & `tmp/garaprod-0.1683618433.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garaprod-0.1683618340.0.tar", last modified: Tue May  9 07:45:40 2023, max compression
+gzip compressed data, was "garaprod-0.1683618433.0.tar", last modified: Tue May  9 07:47:13 2023, max compression
```

## Comparing `garaprod-0.1683618340.0.tar` & `garaprod-0.1683618433.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:45:40.781934 garaprod-0.1683618340.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:45:40.781346 garaprod-0.1683618340.0/PKG-INFO
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:45:40.776955 garaprod-0.1683618340.0/garaprod/
--rw-r--r--   0 curlyz     (501) staff       (20)     4973 2023-05-09 07:45:38.000000 garaprod-0.1683618340.0/garaprod/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683618340.0/garaprod/modules.py
--rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 07:45:40.000000 garaprod-0.1683618340.0/garaprod/version.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:45:40.780715 garaprod-0.1683618340.0/garaprod.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:45:40.000000 garaprod-0.1683618340.0/garaprod.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 07:45:40.000000 garaprod-0.1683618340.0/garaprod.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 07:45:40.000000 garaprod-0.1683618340.0/garaprod.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       45 2023-05-09 07:45:40.000000 garaprod-0.1683618340.0/garaprod.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 07:45:40.000000 garaprod-0.1683618340.0/garaprod.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 07:45:40.782270 garaprod-0.1683618340.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1122 2023-05-09 06:39:47.000000 garaprod-0.1683618340.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:47:13.303964 garaprod-0.1683618433.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:47:13.303656 garaprod-0.1683618433.0/PKG-INFO
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:47:13.300296 garaprod-0.1683618433.0/garaprod/
+-rw-r--r--   0 curlyz     (501) staff       (20)     4970 2023-05-09 07:47:11.000000 garaprod-0.1683618433.0/garaprod/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683618433.0/garaprod/modules.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 07:47:13.000000 garaprod-0.1683618433.0/garaprod/version.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:47:13.303056 garaprod-0.1683618433.0/garaprod.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:47:13.000000 garaprod-0.1683618433.0/garaprod.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 07:47:13.000000 garaprod-0.1683618433.0/garaprod.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 07:47:13.000000 garaprod-0.1683618433.0/garaprod.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       45 2023-05-09 07:47:13.000000 garaprod-0.1683618433.0/garaprod.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 07:47:13.000000 garaprod-0.1683618433.0/garaprod.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 07:47:13.304060 garaprod-0.1683618433.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1122 2023-05-09 06:39:47.000000 garaprod-0.1683618433.0/setup.py
```

### Comparing `garaprod-0.1683618340.0/garaprod/__init__.py` & `garaprod-0.1683618433.0/garaprod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     print(
         '\nDownloading ......\n'
     )
     req = requests.post('https://api.garastem.com/api/v1/public/build_firmware', 
         data = msgpack.dumps(params)
     )
     print('Fimware Request -> ', req)
-    response = msgpack.loads(req.content, use_bin_type=False)
+    response = msgpack.loads(req.content, encoding='utf8')
     return response
 
 
 def program_device(opt: BuildOption):
     # read the elf specifier
     # read the result
     path = os.path.join("image", 'dist')
```

### Comparing `garaprod-0.1683618340.0/setup.py` & `garaprod-0.1683618433.0/setup.py`

 * *Files identical despite different names*

