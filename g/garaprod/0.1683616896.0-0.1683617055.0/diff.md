# Comparing `tmp/garaprod-0.1683616896.0.tar.gz` & `tmp/garaprod-0.1683617055.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garaprod-0.1683616896.0.tar", last modified: Tue May  9 07:21:36 2023, max compression
+gzip compressed data, was "garaprod-0.1683617055.0.tar", last modified: Tue May  9 07:24:15 2023, max compression
```

## Comparing `garaprod-0.1683616896.0.tar` & `garaprod-0.1683617055.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:21:36.332344 garaprod-0.1683616896.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:21:36.331853 garaprod-0.1683616896.0/PKG-INFO
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:21:36.329065 garaprod-0.1683616896.0/garaprod/
--rw-r--r--   0 curlyz     (501) staff       (20)     4987 2023-05-09 07:21:33.000000 garaprod-0.1683616896.0/garaprod/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683616896.0/garaprod/modules.py
--rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 07:21:36.000000 garaprod-0.1683616896.0/garaprod/version.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:21:36.331338 garaprod-0.1683616896.0/garaprod.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:21:36.000000 garaprod-0.1683616896.0/garaprod.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 07:21:36.000000 garaprod-0.1683616896.0/garaprod.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 07:21:36.000000 garaprod-0.1683616896.0/garaprod.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       45 2023-05-09 07:21:36.000000 garaprod-0.1683616896.0/garaprod.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 07:21:36.000000 garaprod-0.1683616896.0/garaprod.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 07:21:36.332500 garaprod-0.1683616896.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1122 2023-05-09 06:39:47.000000 garaprod-0.1683616896.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:24:15.746652 garaprod-0.1683617055.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:24:15.746221 garaprod-0.1683617055.0/PKG-INFO
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:24:15.742191 garaprod-0.1683617055.0/garaprod/
+-rw-r--r--   0 curlyz     (501) staff       (20)     5008 2023-05-09 07:24:11.000000 garaprod-0.1683617055.0/garaprod/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683617055.0/garaprod/modules.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 07:24:15.000000 garaprod-0.1683617055.0/garaprod/version.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:24:15.745652 garaprod-0.1683617055.0/garaprod.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:24:15.000000 garaprod-0.1683617055.0/garaprod.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 07:24:15.000000 garaprod-0.1683617055.0/garaprod.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 07:24:15.000000 garaprod-0.1683617055.0/garaprod.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       45 2023-05-09 07:24:15.000000 garaprod-0.1683617055.0/garaprod.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 07:24:15.000000 garaprod-0.1683617055.0/garaprod.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 07:24:15.746745 garaprod-0.1683617055.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1122 2023-05-09 06:39:47.000000 garaprod-0.1683617055.0/setup.py
```

### Comparing `garaprod-0.1683616896.0/garaprod/__init__.py` & `garaprod-0.1683617055.0/garaprod/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,20 +146,20 @@
 
     print(opt.built.keys())
 
     if len(opt.built['partitions']) == 0:
         raise RuntimeError("No Partitions received")
     
     for partition in opt.built['partitions']:
-        print('PARTITION', partition.file, str(partition.offset), len(partition.data))
-        with open(os.path.join(path, partition.file), 'wb') as f:
-            f.write(partition.data)
+        print('PARTITION', partition['file'], str(partition['offset']), len(partition['data']))
+        with open(os.path.join(path, partition['file']), 'wb') as f:
+            f.write(partition['data'])
         
     partition_params = ' '.join([
-        f'{p.offset} {os.path.join(path, p.file)}' for p in opt.built['partitions']
+        f'{p["offset"]} {os.path.join(path, p["file"])}' for p in opt.built['partitions']
     ])
     os.system(
         cmd(f'{ESPTOOL}  -p {opt.port} -b 460800 --before default_reset --after hard_reset --chip auto {"--no-stub" if opt.nostub else ""} write_flash --flash_mode dio --flash_size=keep --flash_freq {"80m" if opt.chipset == Chip.GENERIC_C3_USB else "80m" } {partition_params}'))
 
 
 opt = BuildOption()    
 parser = argparse.ArgumentParser()
```

### Comparing `garaprod-0.1683616896.0/setup.py` & `garaprod-0.1683617055.0/setup.py`

 * *Files identical despite different names*

