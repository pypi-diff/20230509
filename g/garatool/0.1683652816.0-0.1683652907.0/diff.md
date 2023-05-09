# Comparing `tmp/garatool-0.1683652816.0.tar.gz` & `tmp/garatool-0.1683652907.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683652816.0.tar", last modified: Tue May  9 17:20:16 2023, max compression
+gzip compressed data, was "garatool-0.1683652907.0.tar", last modified: Tue May  9 17:21:47 2023, max compression
```

## Comparing `garatool-0.1683652816.0.tar` & `garatool-0.1683652907.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:20:16.605913 garatool-0.1683652816.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:20:16.605307 garatool-0.1683652816.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683652816.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:20:16.602803 garatool-0.1683652816.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)     5763 2023-05-09 17:19:53.000000 garatool-0.1683652816.0/garatool/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683652816.0/garatool/__main__.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:20:16.604788 garatool-0.1683652816.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:20:16.000000 garatool-0.1683652816.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 17:20:16.000000 garatool-0.1683652816.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 17:20:16.000000 garatool-0.1683652816.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 17:20:16.000000 garatool-0.1683652816.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 17:20:16.000000 garatool-0.1683652816.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 17:20:16.606129 garatool-0.1683652816.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683652816.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:21:47.321288 garatool-0.1683652907.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:21:47.320774 garatool-0.1683652907.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683652907.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:21:47.317903 garatool-0.1683652907.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)     5740 2023-05-09 17:21:45.000000 garatool-0.1683652907.0/garatool/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683652907.0/garatool/__main__.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:21:47.320290 garatool-0.1683652907.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:21:47.000000 garatool-0.1683652907.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 17:21:47.000000 garatool-0.1683652907.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 17:21:47.000000 garatool-0.1683652907.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 17:21:47.000000 garatool-0.1683652907.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 17:21:47.000000 garatool-0.1683652907.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 17:21:47.321389 garatool-0.1683652907.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683652907.0/setup.py
```

### Comparing `garatool-0.1683652816.0/garatool/__init__.py` & `garatool-0.1683652907.0/garatool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,27 +138,27 @@
 
 
 
     partition_params = ' '.join([
         f'{p["offset"]} \"{p["file"]}\"' for p in br.partitions
     ])
 
-    subprocess.getoutput(cmd(' '.join([
+    os.system(cmd(' '.join([
         ESPTOOL,
         '--port', parsed.port,
         '--baud', '460800',
         '--no-stub' if br.nostub else ' '
         '--before=default_reset',
         '--after=hard_reset',
         '--chip', 'auto',
         'write_flash',
         '--flash_mode=dio',
         '--flash_size=keep',
         partition_params
-    ])), shell=True)
+    ])))
 
     for parti in br.partitions:
         try:
             os.remove(parti['file'])
         except OSError:
             pass
```

### Comparing `garatool-0.1683652816.0/setup.py` & `garatool-0.1683652907.0/setup.py`

 * *Files identical despite different names*

