# Comparing `tmp/psgspecialelements-1.0.2.2.tar.gz` & `tmp/psgspecialelements-1.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psgspecialelements-1.0.2.2.tar", last modified: Tue May  9 08:11:53 2023, max compression
+gzip compressed data, was "psgspecialelements-1.0.2.3.tar", last modified: Tue May  9 08:15:28 2023, max compression
```

## Comparing `psgspecialelements-1.0.2.2.tar` & `psgspecialelements-1.0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 08:11:53.159721 psgspecialelements-1.0.2.2/
--rw-rw-rw-   0        0        0      255 2023-05-09 08:11:53.158720 psgspecialelements-1.0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1525 2023-04-21 00:40:07.000000 psgspecialelements-1.0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 08:11:53.139716 psgspecialelements-1.0.2.2/config/
-drwxrwxrwx   0        0        0        0 2023-05-09 08:11:53.147718 psgspecialelements-1.0.2.2/config/img/
--rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 psgspecialelements-1.0.2.2/config/img/table_arrow9_transparent_64.ico
--rw-rw-rw-   0        0        0    34392 2023-04-06 03:13:05.000000 psgspecialelements-1.0.2.2/hash_password.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:11:53.156720 psgspecialelements-1.0.2.2/psgspecialelements.egg-info/
--rw-rw-rw-   0        0        0      255 2023-05-09 08:11:53.000000 psgspecialelements-1.0.2.2/psgspecialelements.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-05-09 08:11:53.000000 psgspecialelements-1.0.2.2/psgspecialelements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 08:11:53.000000 psgspecialelements-1.0.2.2/psgspecialelements.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-09 08:11:53.000000 psgspecialelements-1.0.2.2/psgspecialelements.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2023-05-09 08:11:53.000000 psgspecialelements-1.0.2.2/psgspecialelements.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-05-09 08:11:53.000000 psgspecialelements-1.0.2.2/psgspecialelements.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   239428 2023-05-09 08:11:32.000000 psgspecialelements-1.0.2.2/psgspecialelements.py
--rw-rw-rw-   0        0        0       42 2023-05-09 08:11:53.159721 psgspecialelements-1.0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2782 2023-05-09 08:11:04.000000 psgspecialelements-1.0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:15:28.466161 psgspecialelements-1.0.2.3/
+-rw-rw-rw-   0        0        0      255 2023-05-09 08:15:28.465161 psgspecialelements-1.0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1525 2023-04-21 00:40:07.000000 psgspecialelements-1.0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 08:15:28.445156 psgspecialelements-1.0.2.3/config/
+drwxrwxrwx   0        0        0        0 2023-05-09 08:15:28.454158 psgspecialelements-1.0.2.3/config/img/
+-rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 psgspecialelements-1.0.2.3/config/img/table_arrow9_transparent_64.ico
+-rw-rw-rw-   0        0        0    34392 2023-04-06 03:13:05.000000 psgspecialelements-1.0.2.3/hash_password.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:15:28.463160 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/
+-rw-rw-rw-   0        0        0      255 2023-05-09 08:15:28.000000 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-05-09 08:15:28.000000 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 08:15:28.000000 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-09 08:15:28.000000 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2023-05-09 08:15:28.000000 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-05-09 08:15:28.000000 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   239428 2023-05-09 08:11:32.000000 psgspecialelements-1.0.2.3/psgspecialelements.py
+-rw-rw-rw-   0        0        0       42 2023-05-09 08:15:28.466161 psgspecialelements-1.0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2782 2023-05-09 08:15:08.000000 psgspecialelements-1.0.2.3/setup.py
```

### Comparing `psgspecialelements-1.0.2.2/README.md` & `psgspecialelements-1.0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `psgspecialelements-1.0.2.2/config/img/table_arrow9_transparent_64.ico` & `psgspecialelements-1.0.2.3/config/img/table_arrow9_transparent_64.ico`

 * *Files identical despite different names*

### Comparing `psgspecialelements-1.0.2.2/hash_password.py` & `psgspecialelements-1.0.2.3/hash_password.py`

 * *Files identical despite different names*

### Comparing `psgspecialelements-1.0.2.2/psgspecialelements.py` & `psgspecialelements-1.0.2.3/psgspecialelements.py`

 * *Files identical despite different names*

### Comparing `psgspecialelements-1.0.2.2/setup.py` & `psgspecialelements-1.0.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0d0a 6672 6f6d 2073 6574 7570 746f 6f6c  ..from setuptool
 00000010: 7320 696d 706f 7274 2073 6574 7570 2c20  s import setup, 
 00000020: 6669 6e64 5f70 6163 6b61 6765 730d 0a0d  find_packages...
 00000030: 0a73 6574 7570 280d 0a20 2020 206e 616d  .setup(..    nam
 00000040: 653d 2770 7367 7370 6563 6961 6c65 6c65  e='psgspecialele
 00000050: 6d65 6e74 7327 2c0d 0a20 2020 2076 6572  ments',..    ver
-00000060: 7369 6f6e 3d27 312e 302e 322e 3227 2c0d  sion='1.0.2.2',.
+00000060: 7369 6f6e 3d27 312e 302e 322e 3327 2c0d  sion='1.0.2.3',.
 00000070: 0a20 2020 2064 6573 6372 6970 7469 6f6e  .    description
 00000080: 3d27 7370 6563 6961 6c20 656c 656d 656e  ='special elemen
 00000090: 7473 2062 6173 6564 206f 6e20 7079 7369  ts based on pysi
 000000a0: 6d70 6c65 6775 6920 656c 656d 656e 7473  mplegui elements
 000000b0: 272c 0d0a 2020 2020 6175 7468 6f72 3d27  ',..    author='
 000000c0: 4672 616e 6b20 476f 6e67 272c 0d0a 2020  Frank Gong',..  
 000000d0: 2020 6175 7468 6f72 5f65 6d61 696c 3d27    author_email='
```

