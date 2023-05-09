# Comparing `tmp/shareddata-2.0.7.tar.gz` & `tmp/shareddata-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.0.7.tar", last modified: Tue May  9 10:41:27 2023, max compression
+gzip compressed data, was "shareddata-2.0.8.tar", last modified: Tue May  9 14:12:37 2023, max compression
```

## Comparing `shareddata-2.0.7.tar` & `shareddata-2.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 10:41:27.219871 shareddata-2.0.7/
--rw-rw-rw-   0        0        0    35823 2023-01-12 20:44:38.000000 shareddata-2.0.7/LICENSE
--rw-rw-rw-   0        0        0     1100 2023-05-09 10:41:27.219871 shareddata-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      530 2023-05-07 14:43:50.000000 shareddata-2.0.7/README.md
--rw-rw-rw-   0        0        0      108 2023-01-12 20:44:38.000000 shareddata-2.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      906 2023-05-09 10:41:27.220871 shareddata-2.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 10:41:27.191724 shareddata-2.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 10:41:27.210724 shareddata-2.0.7/src/SharedData/
--rw-rw-rw-   0        0        0     1562 2023-04-11 20:53:38.000000 shareddata-2.0.7/src/SharedData/Defaults.py
--rw-rw-rw-   0        0        0     4735 2023-01-16 18:59:43.000000 shareddata-2.0.7/src/SharedData/Logger.py
--rw-rw-rw-   0        0        0     1275 2023-02-17 15:06:53.000000 shareddata-2.0.7/src/SharedData/LoggerConsumerProcess.py
--rw-rw-rw-   0        0        0    11544 2023-05-07 12:00:04.000000 shareddata-2.0.7/src/SharedData/Metadata.py
--rw-rw-rw-   0        0        0     3862 2023-01-12 20:44:38.000000 shareddata-2.0.7/src/SharedData/MultiProc.py
--rw-rw-rw-   0        0        0     5182 2023-01-12 20:44:38.000000 shareddata-2.0.7/src/SharedData/SeriesLib.py
--rw-rw-rw-   0        0        0     3085 2023-03-02 10:46:06.000000 shareddata-2.0.7/src/SharedData/SharedData.py
--rw-rw-rw-   0        0        0    14573 2023-02-27 22:09:20.000000 shareddata-2.0.7/src/SharedData/SharedDataAWSKinesis.py
--rw-rw-rw-   0        0        0     4586 2023-05-07 14:46:16.000000 shareddata-2.0.7/src/SharedData/SharedDataAWSS3.py
--rw-rw-rw-   0        0        0     6275 2023-05-04 17:59:07.000000 shareddata-2.0.7/src/SharedData/SharedDataFeeder.py
--rw-rw-rw-   0        0        0    11176 2023-05-07 14:43:48.000000 shareddata-2.0.7/src/SharedData/SharedDataFrame.py
--rw-rw-rw-   0        0        0     5818 2023-03-17 12:56:52.000000 shareddata-2.0.7/src/SharedData/SharedDataPeriod.py
--rw-rw-rw-   0        0        0     3672 2023-01-12 20:44:38.000000 shareddata-2.0.7/src/SharedData/SharedDataRealTime.py
--rw-rw-rw-   0        0        0     2545 2023-01-12 20:44:38.000000 shareddata-2.0.7/src/SharedData/SharedDataRealTimeProcess.py
--rw-rw-rw-   0        0        0    26032 2023-05-09 10:40:45.000000 shareddata-2.0.7/src/SharedData/SharedDataTable.py
--rw-rw-rw-   0        0        0    31232 2023-05-04 13:59:43.000000 shareddata-2.0.7/src/SharedData/SharedDataTableKeys.py
--rw-rw-rw-   0        0        0    17673 2023-05-07 14:43:48.000000 shareddata-2.0.7/src/SharedData/SharedDataTimeSeries.py
--rw-rw-rw-   0        0        0     6768 2023-05-07 13:26:07.000000 shareddata-2.0.7/src/SharedData/SharedNumpy.py
--rw-rw-rw-   0        0        0        0 2023-01-12 20:44:38.000000 shareddata-2.0.7/src/SharedData/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 10:41:27.218872 shareddata-2.0.7/src/shareddata.egg-info/
--rw-rw-rw-   0        0        0     1100 2023-05-09 10:41:27.000000 shareddata-2.0.7/src/shareddata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2023-05-09 10:41:27.000000 shareddata-2.0.7/src/shareddata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 10:41:27.000000 shareddata-2.0.7/src/shareddata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-05-09 10:41:27.000000 shareddata-2.0.7/src/shareddata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 10:41:27.000000 shareddata-2.0.7/src/shareddata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 14:12:37.527450 shareddata-2.0.8/
+-rw-rw-rw-   0        0        0    35823 2023-01-12 20:44:38.000000 shareddata-2.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1100 2023-05-09 14:12:37.528450 shareddata-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      530 2023-05-07 14:43:50.000000 shareddata-2.0.8/README.md
+-rw-rw-rw-   0        0        0      108 2023-01-12 20:44:38.000000 shareddata-2.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      906 2023-05-09 14:12:37.531451 shareddata-2.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 14:12:37.508445 shareddata-2.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 14:12:37.520450 shareddata-2.0.8/src/SharedData/
+-rw-rw-rw-   0        0        0     1562 2023-04-11 20:53:38.000000 shareddata-2.0.8/src/SharedData/Defaults.py
+-rw-rw-rw-   0        0        0     4735 2023-01-16 18:59:43.000000 shareddata-2.0.8/src/SharedData/Logger.py
+-rw-rw-rw-   0        0        0     1275 2023-02-17 15:06:53.000000 shareddata-2.0.8/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-rw-   0        0        0    11544 2023-05-07 12:00:04.000000 shareddata-2.0.8/src/SharedData/Metadata.py
+-rw-rw-rw-   0        0        0     3862 2023-01-12 20:44:38.000000 shareddata-2.0.8/src/SharedData/MultiProc.py
+-rw-rw-rw-   0        0        0     5182 2023-01-12 20:44:38.000000 shareddata-2.0.8/src/SharedData/SeriesLib.py
+-rw-rw-rw-   0        0        0     3085 2023-03-02 10:46:06.000000 shareddata-2.0.8/src/SharedData/SharedData.py
+-rw-rw-rw-   0        0        0    14573 2023-02-27 22:09:20.000000 shareddata-2.0.8/src/SharedData/SharedDataAWSKinesis.py
+-rw-rw-rw-   0        0        0     4586 2023-05-07 14:46:16.000000 shareddata-2.0.8/src/SharedData/SharedDataAWSS3.py
+-rw-rw-rw-   0        0        0     6275 2023-05-04 17:59:07.000000 shareddata-2.0.8/src/SharedData/SharedDataFeeder.py
+-rw-rw-rw-   0        0        0    11176 2023-05-07 14:43:48.000000 shareddata-2.0.8/src/SharedData/SharedDataFrame.py
+-rw-rw-rw-   0        0        0     5818 2023-03-17 12:56:52.000000 shareddata-2.0.8/src/SharedData/SharedDataPeriod.py
+-rw-rw-rw-   0        0        0     3672 2023-01-12 20:44:38.000000 shareddata-2.0.8/src/SharedData/SharedDataRealTime.py
+-rw-rw-rw-   0        0        0     2545 2023-01-12 20:44:38.000000 shareddata-2.0.8/src/SharedData/SharedDataRealTimeProcess.py
+-rw-rw-rw-   0        0        0    26032 2023-05-09 10:40:45.000000 shareddata-2.0.8/src/SharedData/SharedDataTable.py
+-rw-rw-rw-   0        0        0    31232 2023-05-04 13:59:43.000000 shareddata-2.0.8/src/SharedData/SharedDataTableKeys.py
+-rw-rw-rw-   0        0        0    17673 2023-05-07 14:43:48.000000 shareddata-2.0.8/src/SharedData/SharedDataTimeSeries.py
+-rw-rw-rw-   0        0        0     7221 2023-05-09 14:12:01.000000 shareddata-2.0.8/src/SharedData/SharedNumpy.py
+-rw-rw-rw-   0        0        0        0 2023-01-12 20:44:38.000000 shareddata-2.0.8/src/SharedData/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:12:37.527450 shareddata-2.0.8/src/shareddata.egg-info/
+-rw-rw-rw-   0        0        0     1100 2023-05-09 14:12:37.000000 shareddata-2.0.8/src/shareddata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2023-05-09 14:12:37.000000 shareddata-2.0.8/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 14:12:37.000000 shareddata-2.0.8/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-05-09 14:12:37.000000 shareddata-2.0.8/src/shareddata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 14:12:37.000000 shareddata-2.0.8/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.0.7/LICENSE` & `shareddata-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/PKG-INFO` & `shareddata-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.0.7
+Version: 2.0.8
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.0.7/README.md` & `shareddata-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/setup.cfg` & `shareddata-2.0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6861 7265 6464 6174 610d 0a76   = shareddata..v
-00000020: 6572 7369 6f6e 203d 2032 2e30 2e37 0d0a  ersion = 2.0.7..
+00000020: 6572 7369 6f6e 203d 2032 2e30 2e38 0d0a  ersion = 2.0.8..
 00000030: 6175 7468 6f72 203d 204a 6f73 6520 4361  author = Jose Ca
 00000040: 726c 6974 6f20 6465 204f 6c69 7665 6972  rlito de Oliveir
 00000050: 6120 4669 6c68 6f0d 0a61 7574 686f 725f  a Filho..author_
 00000060: 656d 6169 6c20 3d20 6a63 6172 6c69 746f  email = jcarlito
 00000070: 6f6c 6976 6569 7261 4067 6d61 696c 2e63  oliveira@gmail.c
 00000080: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000090: 3d20 5368 6172 6564 204d 656d 6f72 7920  = Shared Memory
```

### Comparing `shareddata-2.0.7/src/SharedData/Defaults.py` & `shareddata-2.0.8/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/Logger.py` & `shareddata-2.0.8/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.0.8/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/Metadata.py` & `shareddata-2.0.8/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/MultiProc.py` & `shareddata-2.0.8/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/SeriesLib.py` & `shareddata-2.0.8/src/SharedData/SeriesLib.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/SharedData.py` & `shareddata-2.0.8/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/SharedDataAWSKinesis.py` & `shareddata-2.0.8/src/SharedData/SharedDataAWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/SharedDataAWSS3.py` & `shareddata-2.0.8/src/SharedData/SharedDataAWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/SharedDataFeeder.py` & `shareddata-2.0.8/src/SharedData/SharedDataFeeder.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/SharedDataFrame.py` & `shareddata-2.0.8/src/SharedData/SharedDataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/SharedDataPeriod.py` & `shareddata-2.0.8/src/SharedData/SharedDataPeriod.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/SharedDataRealTime.py` & `shareddata-2.0.8/src/SharedData/SharedDataRealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/SharedDataRealTimeProcess.py` & `shareddata-2.0.8/src/SharedData/SharedDataRealTimeProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/SharedDataTable.py` & `shareddata-2.0.8/src/SharedData/SharedDataTable.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/SharedDataTableKeys.py` & `shareddata-2.0.8/src/SharedData/SharedDataTableKeys.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/SharedDataTimeSeries.py` & `shareddata-2.0.8/src/SharedData/SharedDataTimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.7/src/SharedData/SharedNumpy.py` & `shareddata-2.0.8/src/SharedData/SharedNumpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,22 @@
     
     def insert(self,new_records):
         self.master.acquire()
 
         nrec = new_records.size           
         _count = self.count
         if (_count + nrec <= self.size):
+            # convert new_records
+            if (self.dtype != new_records.dtype):
+                new_records = self.convert(new_records)
+            # fill mtime
+            nidx = np.isnat(new_records['mtime'])
+            if nidx.any():
+                new_records['mtime'][nidx] = time.time_ns()
+
             arr = super().__getitem__(slice(0, self.size))
             arr[_count:_count+nrec] = new_records
             self.count = _count + nrec            
             self.mtime = datetime.now().timestamp()
         else:
             Logger.log.error('Dataset max size reached!')
 
@@ -35,20 +43,24 @@
 
         # assume new_records is sorted 
         # overwrite based on the first date
         if isinstance(new_records,pd.DataFrame):
             new_records = self.master.df2records(new_records)
         elif (self.dtype != new_records.dtype):
             new_records = self.convert(new_records)
+        # fill mtime
+        nidx = np.isnat(new_records['mtime'])
+        if nidx.any():
+            new_records['mtime'][nidx] = time.time_ns()
 
         nrec = new_records.size
         _count = self.count
         # overwrite from first date
         fdate = new_records[0]['date']
-        fdateid = np.where(self['date']>=fdate)[0]        
+        fdateid = np.where(self['date']>=fdate)[0]
         if np.any(fdateid):
             _count = fdateid[0]
         # set data
         if (_count + nrec <= self.size):                        
             arr = super().__getitem__(slice(0, self.size))
             arr[_count:_count+nrec] = new_records
             self.count = _count + nrec
```

### Comparing `shareddata-2.0.7/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.0.8/src/shareddata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.0.7
+Version: 2.0.8
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.0.7/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.0.8/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

