# Comparing `tmp/mesures-2.6.0.tar.gz` & `tmp/mesures-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mesures-2.6.0.tar", last modified: Tue Apr 18 13:47:52 2023, max compression
+gzip compressed data, was "dist/mesures-2.6.1.tar", last modified: Tue May  9 12:50:01 2023, max compression
```

## Comparing `mesures-2.6.0.tar` & `mesures-2.6.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-18 13:47:52.000000 mesures-2.6.0/
--rw-rw-r--   0 david     (1000) david     (1000)     2041 2022-11-15 17:47:41.000000 mesures-2.6.0/README.md
--rw-rw-r--   0 david     (1000) david     (1000)       25 2022-11-15 17:47:41.000000 mesures-2.6.0/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)      290 2023-04-18 13:47:52.000000 mesures-2.6.0/PKG-INFO
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)      290 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       33 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      836 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)      560 2022-11-15 17:47:41.000000 mesures-2.6.0/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures/
--rw-rw-r--   0 david     (1000) david     (1000)     3141 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/almacenacau.py
--rw-rw-r--   0 david     (1000) david     (1000)      434 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)     5204 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/f1.py
--rw-rw-r--   0 david     (1000) david     (1000)     3524 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/f5d.py
--rw-rw-r--   0 david     (1000) david     (1000)     3482 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/p5d.py
--rw-rw-r--   0 david     (1000) david     (1000)     1539 2023-04-18 11:11:41.000000 mesures-2.6.0/mesures/p2.py
--rw-rw-r--   0 david     (1000) david     (1000)     2115 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/cilcau.py
--rw-rw-r--   0 david     (1000) david     (1000)     2314 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/p1d.py
--rw-rw-r--   0 david     (1000) david     (1000)       75 2023-04-18 13:47:02.000000 mesures-2.6.0/mesures/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     5633 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/p1.py
--rw-rw-r--   0 david     (1000) david     (1000)     3702 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/a5d.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures/dates/
--rw-rw-r--   0 david     (1000) david     (1000)      256 2022-11-15 17:47:41.000000 mesures-2.6.0/mesures/dates/date.py
--rw-rw-r--   0 david     (1000) david     (1000)       96 2022-11-15 17:47:41.000000 mesures-2.6.0/mesures/dates/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     5867 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/f5.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-18 13:47:52.000000 mesures-2.6.0/mesures/parsers/
--rw-rw-r--   0 david     (1000) david     (1000)       24 2022-11-15 17:47:41.000000 mesures-2.6.0/mesures/parsers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4185 2022-11-29 14:12:56.000000 mesures-2.6.0/mesures/parsers/dummy_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     3367 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/cupscau.py
--rw-rw-r--   0 david     (1000) david     (1000)     5962 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/mcil345.py
--rw-rw-r--   0 david     (1000) david     (1000)     4739 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/f3.py
--rw-rw-r--   0 david     (1000) david     (1000)     3083 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/cildat.py
--rw-rw-r--   0 david     (1000) david     (1000)     2061 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/p2d.py
--rw-rw-r--   0 david     (1000) david     (1000)     3075 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/agrecl.py
--rw-rw-r--   0 david     (1000) david     (1000)    19081 2022-11-15 17:47:41.000000 mesures-2.6.0/mesures/headers.py
--rw-rw-r--   0 david     (1000) david     (1000)     3715 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/b5d.py
--rw-rw-r--   0 david     (1000) david     (1000)     3329 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/enelectroaut.py
--rw-rw-r--   0 david     (1000) david     (1000)     3373 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/potelectro.py
--rw-rw-r--   0 david     (1000) david     (1000)     3251 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/cumpelectro.py
--rw-rw-r--   0 david     (1000) david     (1000)      624 2023-04-18 11:08:18.000000 mesures-2.6.0/mesures/cups45.py
--rw-rw-r--   0 david     (1000) david     (1000)     3325 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/cupsdat.py
--rw-rw-r--   0 david     (1000) david     (1000)     8317 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/medidas.py
--rw-rw-r--   0 david     (1000) david     (1000)     3471 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/autoconsumo.py
--rw-rw-r--   0 david     (1000) david     (1000)     3357 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/cupselectro.py
--rw-rw-r--   0 david     (1000) david     (1000)     5103 2023-04-18 13:46:39.000000 mesures-2.6.0/mesures/pmest.py
--rw-rw-r--   0 david     (1000) david     (1000)       32 2022-11-15 17:47:41.000000 mesures-2.6.0/requirements.txt
--rw-rw-r--   0 david     (1000) david     (1000)       79 2023-04-18 13:47:52.000000 mesures-2.6.0/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-09 12:50:01.000000 mesures-2.6.1/
+-rw-rw-r--   0 david     (1000) david     (1000)     2041 2022-11-15 17:47:41.000000 mesures-2.6.1/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)       25 2022-11-15 17:47:41.000000 mesures-2.6.1/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)      290 2023-05-09 12:50:01.000000 mesures-2.6.1/PKG-INFO
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-09 12:50:01.000000 mesures-2.6.1/mesures.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)      290 2023-05-09 12:50:01.000000 mesures-2.6.1/mesures.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-05-09 12:50:01.000000 mesures-2.6.1/mesures.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       33 2023-05-09 12:50:01.000000 mesures-2.6.1/mesures.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-05-09 12:50:01.000000 mesures-2.6.1/mesures.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      836 2023-05-09 12:50:01.000000 mesures-2.6.1/mesures.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      560 2022-11-15 17:47:41.000000 mesures-2.6.1/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-09 12:50:01.000000 mesures-2.6.1/mesures/
+-rw-rw-r--   0 david     (1000) david     (1000)     3141 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/almacenacau.py
+-rw-rw-r--   0 david     (1000) david     (1000)      434 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5204 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/f1.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3524 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/f5d.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3482 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/p5d.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1539 2023-04-18 11:11:41.000000 mesures-2.6.1/mesures/p2.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2115 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/cilcau.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2314 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/p1d.py
+-rw-rw-r--   0 david     (1000) david     (1000)       75 2023-05-09 12:49:18.000000 mesures-2.6.1/mesures/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5633 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/p1.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3702 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/a5d.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-09 12:50:01.000000 mesures-2.6.1/mesures/dates/
+-rw-rw-r--   0 david     (1000) david     (1000)      256 2022-11-15 17:47:41.000000 mesures-2.6.1/mesures/dates/date.py
+-rw-rw-r--   0 david     (1000) david     (1000)       96 2022-11-15 17:47:41.000000 mesures-2.6.1/mesures/dates/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5867 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/f5.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-09 12:50:01.000000 mesures-2.6.1/mesures/parsers/
+-rw-rw-r--   0 david     (1000) david     (1000)       24 2022-11-15 17:47:41.000000 mesures-2.6.1/mesures/parsers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4185 2022-11-29 14:12:56.000000 mesures-2.6.1/mesures/parsers/dummy_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3367 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/cupscau.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5962 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/mcil345.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4739 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/f3.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3083 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/cildat.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2061 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/p2d.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3075 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/agrecl.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19081 2022-11-15 17:47:41.000000 mesures-2.6.1/mesures/headers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3715 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/b5d.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3329 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/enelectroaut.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3373 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/potelectro.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3251 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/cumpelectro.py
+-rw-rw-r--   0 david     (1000) david     (1000)      624 2023-04-18 11:08:18.000000 mesures-2.6.1/mesures/cups45.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3325 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/cupsdat.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8317 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/medidas.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3494 2023-05-09 12:48:51.000000 mesures-2.6.1/mesures/autoconsumo.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3357 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/cupselectro.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5103 2023-04-18 13:46:39.000000 mesures-2.6.1/mesures/pmest.py
+-rw-rw-r--   0 david     (1000) david     (1000)       32 2022-11-15 17:47:41.000000 mesures-2.6.1/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       79 2023-05-09 12:50:01.000000 mesures-2.6.1/setup.cfg
```

### Comparing `mesures-2.6.0/README.md` & `mesures-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures.egg-info/SOURCES.txt` & `mesures-2.6.1/mesures.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/setup.py` & `mesures-2.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/almacenacau.py` & `mesures-2.6.1/mesures/almacenacau.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/f1.py` & `mesures-2.6.1/mesures/f1.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/f5d.py` & `mesures-2.6.1/mesures/f5d.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/p5d.py` & `mesures-2.6.1/mesures/p5d.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/p2.py` & `mesures-2.6.1/mesures/p2.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/cilcau.py` & `mesures-2.6.1/mesures/cilcau.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/p1d.py` & `mesures-2.6.1/mesures/p1d.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/p1.py` & `mesures-2.6.1/mesures/p1.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/a5d.py` & `mesures-2.6.1/mesures/a5d.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/f5.py` & `mesures-2.6.1/mesures/f5.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/parsers/dummy_data.py` & `mesures-2.6.1/mesures/parsers/dummy_data.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/cupscau.py` & `mesures-2.6.1/mesures/cupscau.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/mcil345.py` & `mesures-2.6.1/mesures/mcil345.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/f3.py` & `mesures-2.6.1/mesures/f3.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/cildat.py` & `mesures-2.6.1/mesures/cildat.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/p2d.py` & `mesures-2.6.1/mesures/p2d.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/agrecl.py` & `mesures-2.6.1/mesures/agrecl.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/headers.py` & `mesures-2.6.1/mesures/headers.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/b5d.py` & `mesures-2.6.1/mesures/b5d.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/enelectroaut.py` & `mesures-2.6.1/mesures/enelectroaut.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/potelectro.py` & `mesures-2.6.1/mesures/potelectro.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/cumpelectro.py` & `mesures-2.6.1/mesures/cumpelectro.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/cups45.py` & `mesures-2.6.1/mesures/cups45.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/cupsdat.py` & `mesures-2.6.1/mesures/cupsdat.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/medidas.py` & `mesures-2.6.1/mesures/medidas.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/autoconsumo.py` & `mesures-2.6.1/mesures/autoconsumo.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,17 +68,17 @@
             raise Exception("Filepath must be an str or a list")
 
         df['data_baixa'] = df['data_baixa'].apply(
             lambda x: REE_END_DATE if not isinstance(x, pd.Timestamp) else x.strftime('%Y%m%d'))
         df['data_alta'] = df['data_alta'].apply(lambda x: x.strftime('%Y%m%d'))
         df['emmagatzematge'] = np.where(df['emmagatzematge'], 'S', 'N')
         #df['potencia_nominal'] = np.where(df['cil'], '', df['potencia_nominal'])
-        df['subgrup'] = df['subgrup'].apply(lambda x: x.replace('.', '')[:2])
+        df['subgrup'] = df['subgrup'].apply(lambda x: '{}.{}.{}'.format(x[0], x[1], x[2]) if x != '' else '')
         df['tipus_antiabocament'] = (
-            df['tipus_antiabocament'].apply(lambda x: '' if (x == 0 or not x or x == '') else x.zfill(2)))
+            df['tipus_antiabocament'].apply(lambda x: '' if (x == 0 or not x or x == '') else x))
         df = df[columns]
         return df
 
     def writer(self):
         """
         :return: file path of generated AUTOCONSUMO File
         """
```

### Comparing `mesures-2.6.0/mesures/cupselectro.py` & `mesures-2.6.1/mesures/cupselectro.py`

 * *Files identical despite different names*

### Comparing `mesures-2.6.0/mesures/pmest.py` & `mesures-2.6.1/mesures/pmest.py`

 * *Files identical despite different names*

