# Comparing `tmp/csst-ifs-gehong-0.0.1.8.tar.gz` & `tmp/csst-ifs-gehong-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csst-ifs-gehong-0.0.1.8.tar", last modified: Thu May  4 11:51:12 2023, max compression
+gzip compressed data, was "csst-ifs-gehong-1.0.0.tar", last modified: Tue May  9 06:35:43 2023, max compression
```

## Comparing `csst-ifs-gehong-0.0.1.8.tar` & `csst-ifs-gehong-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 11:51:12.083974 csst-ifs-gehong-0.0.1.8/
--rw-r--r--   0 sfeng      (501) staff       (20)     1073 2023-04-25 01:31:05.000000 csst-ifs-gehong-0.0.1.8/LICENSE
--rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-04 11:51:12.084092 csst-ifs-gehong-0.0.1.8/PKG-INFO
--rw-r--r--   0 sfeng      (501) staff       (20)      244 2023-04-26 13:40:59.000000 csst-ifs-gehong-0.0.1.8/README.md
--rw-r--r--   0 sfeng      (501) staff       (20)      103 2023-05-04 11:51:12.084495 csst-ifs-gehong-0.0.1.8/setup.cfg
--rw-r--r--   0 sfeng      (501) staff       (20)      392 2023-05-04 11:50:41.000000 csst-ifs-gehong-0.0.1.8/setup.py
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 11:51:12.080198 csst-ifs-gehong-0.0.1.8/src/
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 11:51:12.081535 csst-ifs-gehong-0.0.1.8/src/csst_ifs_gehong.egg-info/
--rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-04 11:51:12.000000 csst-ifs-gehong-0.0.1.8/src/csst_ifs_gehong.egg-info/PKG-INFO
--rw-r--r--   0 sfeng      (501) staff       (20)      415 2023-05-04 11:51:12.000000 csst-ifs-gehong-0.0.1.8/src/csst_ifs_gehong.egg-info/SOURCES.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        1 2023-05-04 11:51:12.000000 csst-ifs-gehong-0.0.1.8/src/csst_ifs_gehong.egg-info/dependency_links.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        8 2023-05-04 11:51:12.000000 csst-ifs-gehong-0.0.1.8/src/csst_ifs_gehong.egg-info/requires.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        7 2023-05-04 11:51:12.000000 csst-ifs-gehong-0.0.1.8/src/csst_ifs_gehong.egg-info/top_level.txt
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 11:51:12.082734 csst-ifs-gehong-0.0.1.8/src/gehong/
--rw-r--r--   0 sfeng      (501) staff       (20)        0 2023-04-12 01:06:24.000000 csst-ifs-gehong-0.0.1.8/src/gehong/__init__.py
--rw-r--r--   0 sfeng      (501) staff       (20)     1236 2023-05-02 10:42:18.000000 csst-ifs-gehong-0.0.1.8/src/gehong/config.py
--rw-r--r--   0 sfeng      (501) staff       (20)     3593 2023-05-04 09:46:41.000000 csst-ifs-gehong-0.0.1.8/src/gehong/cube3d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    11669 2023-05-04 01:23:49.000000 csst-ifs-gehong-0.0.1.8/src/gehong/map2d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    37404 2023-05-04 11:50:16.000000 csst-ifs-gehong-0.0.1.8/src/gehong/spec1d.py
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-04 11:51:12.083499 csst-ifs-gehong-0.0.1.8/test/
--rw-r--r--   0 sfeng      (501) staff       (20)     2710 2023-05-03 04:52:05.000000 csst-ifs-gehong-0.0.1.8/test/test_cube3d.py
--rw-r--r--   0 sfeng      (501) staff       (20)     8115 2023-05-03 04:46:37.000000 csst-ifs-gehong-0.0.1.8/test/test_map2d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    17388 2023-05-03 01:16:32.000000 csst-ifs-gehong-0.0.1.8/test/test_spec1d.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-09 06:35:43.000272 csst-ifs-gehong-1.0.0/
+-rw-r--r--   0 sfeng      (501) staff       (20)     1073 2023-04-25 01:31:05.000000 csst-ifs-gehong-1.0.0/LICENSE
+-rw-r--r--   0 sfeng      (501) staff       (20)      226 2023-05-09 06:35:43.000517 csst-ifs-gehong-1.0.0/PKG-INFO
+-rw-r--r--   0 sfeng      (501) staff       (20)      244 2023-04-26 13:40:59.000000 csst-ifs-gehong-1.0.0/README.md
+-rw-r--r--   0 sfeng      (501) staff       (20)      103 2023-05-09 06:35:43.000995 csst-ifs-gehong-1.0.0/setup.cfg
+-rw-r--r--   0 sfeng      (501) staff       (20)      390 2023-05-07 01:08:57.000000 csst-ifs-gehong-1.0.0/setup.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-09 06:35:42.994135 csst-ifs-gehong-1.0.0/src/
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-09 06:35:42.996133 csst-ifs-gehong-1.0.0/src/csst_ifs_gehong.egg-info/
+-rw-r--r--   0 sfeng      (501) staff       (20)      226 2023-05-09 06:35:42.000000 csst-ifs-gehong-1.0.0/src/csst_ifs_gehong.egg-info/PKG-INFO
+-rw-r--r--   0 sfeng      (501) staff       (20)      415 2023-05-09 06:35:42.000000 csst-ifs-gehong-1.0.0/src/csst_ifs_gehong.egg-info/SOURCES.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        1 2023-05-09 06:35:42.000000 csst-ifs-gehong-1.0.0/src/csst_ifs_gehong.egg-info/dependency_links.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        8 2023-05-09 06:35:42.000000 csst-ifs-gehong-1.0.0/src/csst_ifs_gehong.egg-info/requires.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        7 2023-05-09 06:35:42.000000 csst-ifs-gehong-1.0.0/src/csst_ifs_gehong.egg-info/top_level.txt
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-09 06:35:42.997465 csst-ifs-gehong-1.0.0/src/gehong/
+-rw-r--r--   0 sfeng      (501) staff       (20)        0 2023-04-12 01:06:24.000000 csst-ifs-gehong-1.0.0/src/gehong/__init__.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     1236 2023-05-02 10:42:18.000000 csst-ifs-gehong-1.0.0/src/gehong/config.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     3597 2023-05-09 06:32:21.000000 csst-ifs-gehong-1.0.0/src/gehong/cube3d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    11669 2023-05-04 01:23:49.000000 csst-ifs-gehong-1.0.0/src/gehong/map2d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    37404 2023-05-04 11:50:16.000000 csst-ifs-gehong-1.0.0/src/gehong/spec1d.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-09 06:35:42.999306 csst-ifs-gehong-1.0.0/test/
+-rw-r--r--   0 sfeng      (501) staff       (20)     2710 2023-05-03 04:52:05.000000 csst-ifs-gehong-1.0.0/test/test_cube3d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     8115 2023-05-03 04:46:37.000000 csst-ifs-gehong-1.0.0/test/test_map2d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    17388 2023-05-03 01:16:32.000000 csst-ifs-gehong-1.0.0/test/test_spec1d.py
```

### Comparing `csst-ifs-gehong-0.0.1.8/LICENSE` & `csst-ifs-gehong-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.8/src/gehong/config.py` & `csst-ifs-gehong-1.0.0/src/gehong/config.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.8/src/gehong/cube3d.py` & `csst-ifs-gehong-1.0.0/src/gehong/cube3d.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,16 +63,16 @@
                     'CRPIX3': np.round(self.nx / 2.), 
                     'CRVAL3': 1, 
                     'BUNIT' : '10**(-17)*erg/s/cm**2/Angstrom'}
         input_wcs = astropy.wcs.WCS(wcs_dict)
         self.wcs_header = input_wcs.to_header()
         
     def insert_spec(self, spec, dx = 0, dy = 0):
-        x0 = np.int(np.round(self.inst.nx / 2.))
-        y0 = np.int(np.round(self.inst.ny / 2.))
+        x0 = np.int(np.round(self.config.nx / 2.))
+        y0 = np.int(np.round(self.config.ny / 2.))
         self.flux[x0 + dx, y0 + dy, :] = self.flux[x0 + dx, y0 + dy, :] + spec.flux
         
     def savefits(self, filename, path = './'): 
         
         hdr = fits.Header()
         
         hdr['FILETYPE'] = 'SCICUBE'
```

### Comparing `csst-ifs-gehong-0.0.1.8/src/gehong/map2d.py` & `csst-ifs-gehong-1.0.0/src/gehong/map2d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.8/src/gehong/spec1d.py` & `csst-ifs-gehong-1.0.0/src/gehong/spec1d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.8/test/test_cube3d.py` & `csst-ifs-gehong-1.0.0/test/test_cube3d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.8/test/test_map2d.py` & `csst-ifs-gehong-1.0.0/test/test_map2d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.8/test/test_spec1d.py` & `csst-ifs-gehong-1.0.0/test/test_spec1d.py`

 * *Files identical despite different names*

