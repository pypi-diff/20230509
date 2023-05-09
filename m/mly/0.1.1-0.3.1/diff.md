# Comparing `tmp/mly-0.1.1.tar.gz` & `tmp/mly-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mly-0.1.1.tar", last modified: Mon Apr 20 09:48:20 2020, max compression
+gzip compressed data, was "mly-0.3.1.tar", last modified: Tue May  9 15:01:27 2023, max compression
```

## Comparing `mly-0.1.1.tar` & `mly-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,41 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2020-04-20 09:48:20.000000 mly-0.1.1/
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2020-04-20 09:48:19.000000 mly-0.1.1/mly/
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2020-04-20 09:48:20.000000 mly-0.1.1/mly/oldVersionsPackages/
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2020-02-12 15:56:17.000000 mly-0.1.1/mly/oldVersionsPackages/__init__.py
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   160887 2019-11-19 13:44:19.000000 mly-0.1.1/mly/oldVersionsPackages/generators.py
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    70064 2019-06-30 14:03:02.000000 mly-0.1.1/mly/oldVersionsPackages/validators.py
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  1433718 2020-02-19 22:42:09.000000 mly-0.1.1/mly/SRD.py
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1416 2019-05-29 15:41:54.000000 mly-0.1.1/mly/__init__.py
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28543 2020-04-15 15:34:38.000000 mly-0.1.1/mly/core.py
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    84868 2020-04-15 15:31:17.000000 mly-0.1.1/mly/datatools.py
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1689 2019-05-29 09:45:09.000000 mly-0.1.1/mly/examples.py
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7770 2019-12-13 14:03:50.000000 mly-0.1.1/mly/mlTools.py
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6996 2019-04-03 14:53:57.000000 mly-0.1.1/mly/models.py
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8873 2020-02-19 22:42:43.000000 mly-0.1.1/mly/simulateddetectornoise.py
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4178 2020-04-09 12:21:16.000000 mly-0.1.1/mly/tools.py
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    67150 2020-02-28 21:32:51.000000 mly-0.1.1/mly/validators.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10203 2020-02-18 17:09:21.000000 mly-0.1.1/mly/waveforms.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2020-04-20 09:48:19.000000 mly-0.1.1/mly.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      531 2020-04-20 09:47:50.000000 mly-0.1.1/mly.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      443 2020-04-20 09:47:53.000000 mly-0.1.1/mly.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2020-04-20 09:47:50.000000 mly-0.1.1/mly.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       67 2020-04-20 09:47:50.000000 mly-0.1.1/mly.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2020-04-20 09:47:50.000000 mly-0.1.1/mly.egg-info/top_level.txt
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2019-04-01 15:58:41.000000 mly-0.1.1/README.md
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2020-04-20 09:46:43.000000 mly-0.1.1/setup.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      531 2020-04-20 09:48:20.000000 mly-0.1.1/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2020-04-20 09:48:20.000000 mly-0.1.1/setup.cfg
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-09 15:01:27.039848 mly-0.3.1/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2021-01-11 16:48:33.000000 mly-0.3.1/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      497 2023-05-09 15:01:27.039848 mly-0.3.1/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2021-01-11 16:48:33.000000 mly-0.3.1/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-09 15:01:27.019848 mly-0.3.1/mly/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  1433718 2021-05-11 10:43:11.000000 mly-0.3.1/mly/SRD.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:15:39.000000 mly-0.3.1/mly/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10226 2023-05-09 14:55:57.000000 mly-0.3.1/mly/createFileSystem.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-09 15:01:27.030848 mly-0.3.1/mly/datatools/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      140 2023-05-09 14:56:02.000000 mly-0.3.1/mly/datatools/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22280 2023-05-09 14:56:02.000000 mly-0.3.1/mly/datatools/core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29349 2023-05-09 14:56:02.000000 mly-0.3.1/mly/datatools/datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    90481 2023-05-09 14:56:02.000000 mly-0.3.1/mly/datatools/generator.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-09 15:01:27.034848 mly-0.3.1/mly/datatools/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:56:02.000000 mly-0.3.1/mly/datatools/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3438 2023-05-09 14:56:02.000000 mly-0.3.1/mly/datatools/tests/test_core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      441 2023-05-09 14:56:02.000000 mly-0.3.1/mly/datatools/tests/test_datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4570 2023-05-09 14:56:02.000000 mly-0.3.1/mly/datatools/tests/test_generator.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18459 2023-05-09 14:56:02.000000 mly-0.3.1/mly/exceptions.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7770 2022-08-17 15:08:03.000000 mly-0.3.1/mly/mlTools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6996 2021-01-11 16:48:33.000000 mly-0.3.1/mly/models.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    12353 2023-05-04 12:56:19.000000 mly-0.3.1/mly/null_energy_map.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7262 2023-05-04 12:56:19.000000 mly-0.3.1/mly/offlinefar.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7797 2023-05-04 12:56:19.000000 mly-0.3.1/mly/plugins.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10134 2023-05-04 12:56:19.000000 mly-0.3.1/mly/projectwave.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8913 2022-03-15 16:16:40.000000 mly-0.3.1/mly/simulateddetectornoise.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-09 15:01:27.038848 mly-0.3.1/mly/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      728 2021-10-07 09:34:45.000000 mly-0.3.1/mly/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1601 2021-10-08 08:22:16.000000 mly-0.3.1/mly/tests/test_init.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5258 2022-03-02 09:58:19.000000 mly-0.3.1/mly/tests/test_tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13014 2023-05-04 12:56:19.000000 mly-0.3.1/mly/tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   126781 2023-05-04 12:56:19.000000 mly-0.3.1/mly/validators.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    34282 2023-05-09 14:56:02.000000 mly-0.3.1/mly/waveforms.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-09 15:01:27.025848 mly-0.3.1/mly.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      497 2023-05-09 15:01:25.000000 mly-0.3.1/mly.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      733 2023-05-09 15:01:25.000000 mly-0.3.1/mly.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-05-09 15:01:25.000000 mly-0.3.1/mly.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       77 2023-05-09 15:01:25.000000 mly-0.3.1/mly.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-05-09 15:01:25.000000 mly-0.3.1/mly.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       79 2023-05-09 15:01:27.040848 mly-0.3.1/setup.cfg
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      913 2023-05-09 15:01:08.000000 mly-0.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mly-0.1.1/mly/SRD.py` & `mly-0.3.1/mly/SRD.py`

 * *Files identical despite different names*

### Comparing `mly-0.1.1/mly/core.py` & `mly-0.3.1/mly/datatools/datatools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,672 +1,748 @@
-from gwpy.timeseries import TimeSeries
-from gwpy.segments import Segment, SegmentList
-import numpy as np
-import pandas as pd
-from sys import getsizeof
-import copy
-import pickle 
+from .core import DataPodBase, DataSetBase
+from ..tools import dirlist, internalLags, correlate
+from ..plugins import *
+
+import pickle
 import os
+import sys
+import time
+import random
+import copy
+
+import numpy as npl
+import matplotlib.pyplot as plt
+
+from gwpy.timeseries import TimeSeries
+from gwpy.segments import Segment,SegmentList,DataQualityFlag
+from gwpy.time import to_gps, from_gps
+
+
 
 ################################################################################
 
-class DataPodBase:
-    # --- INFO --------------------------------------------------------------- #
-    #                                                                          # 
-    # DataPod is an object that holds all the information required from a data #
-    # instance. The reason for this object is to be the building block for a   #
-    # versatile dataset object that can be easyly used as input to many types  #
-    # of machine learning networks.                                            # 
-    #                                                                          # 
-    # ------------------------------------------------------------------------ #
-    
-    #                                                                          #             
-    ###--- STR & REPR methods -----------------------------------------------###        
-    #                                                                          #
-    
-    def __str__(self):
-        statement=''
-        
-        lim = 10
-        labels_len=0
-        final_len=81
-        
-        for _ in self._labels.keys():
-            labels_len += len((str(self._labels[_])+' ')) 
-            
-        while final_len>80:
-            labels_len=0
-            for _ in self._labels.keys():
-                labels_len += len((str(self._labels[_])+' '))
-            final_len =(33+len(str(self.shape))+labels_len+4*lim)
-            lim-=1    
-            
-        for i in range(len(self._detectors)):
-
-            labels_str=''
-            if i==len(self._detectors)-1 :
-                labels_str+='  LABELS: '
-                for _ in self._labels.keys():
-                    labels_str += (str(self._labels[_])+' ') 
-
-            info=''
-            if i==0: 
-                info+=str(self.shape)
-            else:
-                info+=len(str(self.shape))*' '
-            info +=('[ '+str(self._strain[i][0])[0:lim]+' '
-                    +str(self._strain[i][1])[0:lim]+' ... '
-                    +str(self._strain[i][-2])[0:lim]+' '
-                    +str(self._strain[i][-1])[0:lim]+' ] ')
-            if self._detectors[i]!='U': info+=(self._detectors[i]) 
-            if self._gps[i]!=0.0 : info+=('_'+str("%10d" % self._gps[i]))
-
-            statement+=info+labels_str+' \n'
-
-        return(statement)
-    
-    def __repr__(self):
-        statement=''
-        lim=6    
-        for i in range(len(self._detectors)):
-
-            labels_str=''
-            if i==len(self._detectors)-1 :
-                labels_str+='  LABELS: '
-                for _ in self._labels.keys():
-                    labels_str += (str(self._labels[_])+' ') 
-
-            info=''
-            if i==0: 
-                info+=str(self.shape)
-            else:
-                info+=len(str(self.shape))*' '
-            info +=('[ '+str(self._strain[i][0])[0:lim]+' '
-                    +str(self._strain[i][1])[0:lim]+' ... '
-                    +str(self._strain[i][-2])[0:lim]+' '
-                    +str(self._strain[i][-1])[0:lim]+' ] ')
-            if self._detectors[i]!='U': info+=(self._detectors[i]) 
-            if self._gps[i]!=0.0 : info+=('_'+str("%010d" % self._gps[i]))
+class DataPod(DataPodBase):
 
-            statement+=info+labels_str+' \n'
+    '''DataPod is an object to consentrate all the information of a data.
+    instance. The reason for their creation is to encapsulate all the usefull
+    attributes a machine learning algorithm will need. Getting them together 
+    into DataSet objects creates a powerfull tool to simplify machine learning
+    training and testing procedures for any kind of network.
+    
+    Attributes
+    ----------
+    
+    strain :  numpy.ndarray / gwpy.timeseries.TimeSeries / list
+        The main data of the pod. It can be a timeseries or a picture or 
+        anything with fixed dimentions. The input is checked for nan
+        and inf values and raises error if the data have size or value problems.
+            
+    fs : int
+        This is the sample frequency of the data. It is used to determine 
+        the duration of the of the strain input. If the strain is not a
+        time series it is not used anywhere.
+            
+    labels : dict (optional)
+        It determines the main labels of the DataPod. These labels will be
+        used by algorithms for classification. If empty, a label called 
+        "UNDEFINED" is given. Suggested keys for labels are the following:
+        
+              { 'type' : ('noise' , 'cbc' , 'signal' , 'burst' , 'glitch', ...),
+                'snr'  : ( any int or float number bigger than zero),
+                'delta': ( Declination for sky localisation, float [-pi/2,pi/2])
+                'ra'   : ( Right ascention for sky licalisation float [0,2pi) )}
+                
+                For all labels, keys and values are not case sensitive.
+            
+    detectors : list (optional)
+        If the strain belongs to a specific detector it is suggested to 
+        state which detector is it. If it not specified the number of 
+        detectors is assumed to be the smallest strain dimention and a
+        list of 'U' is set with length equal to the detector number that 
+        was assumed. The first dimention of every strain must be the 
+        number of detectors involved. If it's not a check takes place to
+        see if the dimention is somewhere else. If it is we the strain is
+        transposed.
+              
+    gps : int / float (optional)
+        The gps time of each of the detector strains. If not defined a
+        list of zeros with length equal to detectors is defined. It has to
+        be a possitive number.
+    
+    duration : int / float (optional for timeseries)
+        The duration in seconds of the strain. If the strain is more than
+        2D in shape the duration has to be difined independently.
+              
+    metadata : dict (optional)
+        A dictionary with additional infromation about the pod.
+        
+    plugins : Plugin / str (optional)
+        Except strain data it might be wanted to have other related data. 
+        You can define PlugIn objects and pass them into the Dataset. Some
+        of those PlugIns like 'correlation', are already defined and you can 
+        call them as by passing their names as strings.
+    '''
+        
+    def __getitem__(self,index):
+        if isinstance(index,int): index=slice(index,None,None)
+        if isinstance(index,slice):
+            return self._strain[index]
+        elif isinstance(index,list) and all((isinstance(det,str) and (det in self._detectors) 
+             and det!='U') for det in index):
+            newStrain=[]
+            newGPS=[]
+            newMeta=copy.deepcopy(self.metadata)
+            ignoredDetectors=[]
+            for d in self.detectors:
+                if not (d in index) : ignoredDetectors.append(d)
+            for det in index:
+                ind = self._detectors.index(det)
+                newStrain.append(self._strain[ind])
+                newGPS.append(self.gps[ind])
+            for d in ignoredDetectors:
+                for key in newMeta:
+                    if isinstance(newMeta[key],dict) and len(self.metadata[key])==len(self.detectors):
+                        del newMeta[key][d]
+            return(DataPod(newStrain,fs=self.fs,labels=copy.deepcopy(self.labels)
+                           ,gps = newGPS,detectors=index
+                           ,duration=self.duration
+                           ,metadata=newMeta))
+        else:
+            raise TypeError("index can be int or a list with detector names that exists")
+    
+      
+    # --- saving method ------------------------------------------------------ #
+    
+    def save(self, name=None
+             , saving_format = None
+             , allowed_formats = ['pkl','txt']):
+        """Method to save the DataPod object
+
+        Parameters
+        -------------
+        name : str 
+            Name of the file to be saved.
+
+        type_ : '.pkl' or .'txt'
+            The format to save it.
+
+        """
+        if name is None:
+            raise TypeError("You need to provide a name for the saved file.")
+
+        elif isinstance(name,str):
+
+            if any("."+f in name for f in allowed_formats):
+                name = '.'.join(name.split(".")[:-1])
+
+        if saving_format is None:
+            saving_format = 'pkl'
+
+        if saving_format == 'pkl' and (saving_format in allowed_formats):
+            with open(finalName+'.pkl', 'wb') as output:
+                pickle.dump(self, output, 4)
+
+        elif saving_format == 'txt' and (saving_format in allowed_formats):
+            np.savetxt(finalName+'.txt', self.strain)
+
+        else:
+            raise TypeError(saving_format+" is not supported.")
+            
+    # --- loading method ------------------------------------------------------#    
+    
+    def load(filename):
+        """Method to load a DataPod object
+        
+        Parameters
+        -------------
+        filename : str (path)
+            Path to the file.
+        
+        """
+        if ".pkl" in filename:
+            with open(filename,'rb') as obj:
+                a = pickle.load(obj)
+            return(a)
+        elif ".txt" in filename:
+            nArray = np.loadtxt(filename)
+            return(nArray)
+        else:
+            raise TypeError("Only .pkl files are supported for loading")
+
+    
+    
+    def addPlugIn(self,*args):
+        """Method to add PlugIn objects to the dataPod. PlugIn objects are extra
+        data derived either from the already existing data in the pod or tottaly
+        new ones. You can add a simple value to generation function and also a
+        plot function if you need to plot the new data.
+
+        Parameters
+        ----------
+
+        *args: PlugIn objects
+            The PlugIn objects that you have already defined and you want to add
+            on the pod.
+
+        """
+        for plugin in args:
+            if not isinstance(plugin,PlugIn):
+                raise TypeError("Inputs must be PlugIn objects")
+                
+        for plugin in args:
+            plugAttributes=[]
+            for at in plugin.attributes:
+                if at in dir(self):
+                    plugAttributes.append(self.__getattribute__(at))
+                else:
+                    raise AttributeError(at+" is not part of DataPod instance")
+            if callable(plugin.genFunction):
+                self.__setattr__(plugin.name,plugin.genFunction(*plugAttributes,**plugin.kwargs))
+            else:
+                self.__setattr__(plugin.name,plugin.genFunction)
 
-        return(statement)
-   
-        
-    #                                                                          #
-    ###--- INIT method ------------------------------------------------------###
-    #                                                                          #
-    
-    def __init__(self
-                 , strain             # The core data (any consistent shape)
-                 , fs = None          # Sample frequency
-                 , gps = None         # GPS time of the data
-                 , labels = None      # Labels of any type
-                 , detectors = None   # Detectors coresponding to data
-                 , duration = None    # Duration of the data
-                 , metadata = None):  # Any other useful information 
-        
-        
-        # -------------------------------------------------------------------- #
-        # -- strain check ---------------------------------------------------- #
-        
-        # # Checking the type of input for strain:
-        # ---> This is the type would want.
-        if (isinstance(strain,np.ndarray)): 
-            pass
-        # ---> If it is a list we just make it a numpy.ndarray.
-        elif (isinstance(strain,list)): 
-            strain = np.array(strain)      
-        # ---> If it is a TimeSeries we take the value only.   
-        elif (isinstance(strain,TimeSeries)): 
-            strain = strain.value      
-        else:
-            raise TypeError("strain type can be only one of the following:/n"+
-                           "list \nnumpy.ndarray\ngwpy.timeseries.TimeSeries")
-            
-        # # Strain has to have clear fixed dimentions.
-        # ---> If all elements have the same len with the first we are fine.
-        if (isinstance(strain[0],np.ndarray) 
-            and not all(len(x)==len(strain[0]) for x in strain)):
-            raise IndexError("Some detector strain have different size that "+
-                             "the others")
-            
-        # # Strain has to be free from infs and nans
-        # ---> If there is an inf or nan in the strain an erros is raised.
-        if not np.isfinite(strain).all():
-            raise ValueError("There is nan or inf value in the strain")
-        if all(np.isreal(x) for x in strain.flatten()):
-            # # For one dimentional data, we need to specify the shape differently.   
-            if len(strain.shape) == 1:
-                strain= strain.reshape(1,-1)
-            self._strain = strain
-        else:
-            raise TypeError("strain values can only be int or float")
- 
+            self.pluginDict[plugin.name]=plugin
             
-        # -------------------------------------------------------------------- #
-        # --- fs check --------------------------------------------------------#
+            
+    def plot(self,type_='strain'):
         
-        # # fs has to be a valid number.
-        # ---> If fs is not a positive int and error is raised.
-        if fs==None: fs = 1
-        if isinstance(fs, int) and fs > 0:
-            self._fs = fs 
-        else:
-            raise ValueError("Sample frequency must have no decimal part")
-            
-            
-        # -------------------------------------------------------------------- #
-        # --- labels check ----------------------------------------------------#
-        
-        # # Labels are optional and it has to be a dictionary.
-        # ---> If empty a label 'UNDEFINED' is given.
-        if labels == None:
-            self._labels={'type':'UNDEFINED'}
-        # ---> If a dictionary is given we have to make sure is not empty.
-        elif isinstance(labels,dict):
-            if len(labels) == 0:
-                # ---> If it is empty we give the 'UNDEFINED' label.
-                print("Labels should have at least one element key \'type\'."
-                      +"\'UNDEFINED\' value has been set as \'type\'. ")
-                self._labels={'type':'UNDEFINED'} 
-            else:
-                self._labels=labels
-        # ---> If a non dictionary object is given, an error is called.
-        else:
-            raise TypeError("labels must be a dictionary")
-            
-            
-        # -------------------------------------------------------------------- #
-        # --- detectors check ------------------------------------------------ #
-        
-        # # Detectors is an optional parameter.
-        # ---> If not given it will be assumed from the smallest dimention.
-        # ---> This can create problems for dimentions > 1D.
-        if detectors == None: 
-            d=np.min(self._strain.shape)
-            detectors = d*['U']
-        # # If detectors is used, it has to be a list.
-        # ---> If it is not an error is raised.
-        if not isinstance(detectors,(list,str)): raise TypeError(
-            "detectors have to be a list of strings"+
-            " with at least one the followings as elements: \n"+
-            "'H' for LIGO Hanford \n'L' for LIGO Livingston\n"+
-            "'V' for Virgo \n'K' for KAGRA \n'I' for LIGO India (INDIGO) \n"+
-            "\n'U' if you don't want to specify detector")
+        """A visualisation function for the DataPod. It will plot the data 
+        currently present on the DataPod object, following LIGO colour 
+        conventions.
+        
+        Parameters
+        ----------
+        
+        type_ : str (optional)
+            The type of data to plot. Some pods might have plottable PlugIn data.
+            In this case you can provide the name of that PlugIn to be ploted. 
+            Currently only strain, psd and correlation are supported. The
+            default value is strain.
+        
+        """
+        
+        colors = {'H': '#ee0000','L':'#4ba6ff','V':'#9b59b6','K':'#ffb200','I':'#b0dd8b','U':'black'}
+        names=[]
+        if type_ == 'strain':
             
-        # # Moreover it has to be a list containing specific detector initials.
-        # ---> If elements of detectors aren't in detector it gives an error. 
-        detectorOptions = ['H','L','V','K','I','U']
-        if isinstance(detectors,list):
-            for det in detectors:
-                if det not in detectorOptions: 
-                    raise ValueError(
-                        "detectors have to be a list of strings"+
-                        " with at least one the followings as elements: \n"+
-                        "'H' for LIGO Hanford \n'L' for LIGO Livingston\n"+
-                        "'V' for Virgo \n'K' for KAGRA \n'I' for LIGO India"+
-                        " (INDIGO) \n"+
-                        "\n'U' if you don't want to specify detector")
-        
-        # # The number of detectors must be shown at the first dimention.
-        if (self._strain.shape[0] == len(detectors)):
-            self._detectors = detectors
-        # ---> If it is not in the first dimention maybe needs transpose.
-        elif (self._strain.shape[0] != len(detectors)):
-            # ---> If the number of detectors is present at some dimention.
-            if ((len(detectors) in self._strain.shape) 
-                and self._strain.shape.count(len(detectors))==1):
-                # --- Then we traspose the strain.
-                newShape = list(self._strain.shape)
-                newShape.pop(newShape.index(len(detectors)))
-                newShape.insert(0,len(detectors))
-                ind = [list(self._strain.shape).index(i) for i in newShape]
-                self._strain = np.transpose(self._strain, ind)
-                print("Needed shape change of the strain occured")
-                self._detectors = detectors
-            # ---> If not, an error occures.
-            else:
-                raise IndexError("detectors must be as many as the strain")
-                         
-                          
-        # -------------------------------------------------------------------- #
-        #--- gps check ------------------------------------------------------- #
-  
-        # # GPS is optional or a list of positive numbers.
-        # ---> If not defined, a list of zeros is defined equal to detectors.
-        if gps == None:
-            self._gps = len(self._detectors)*[0.0]  
-        # ---> If it is a list, it has to include positive numbers.
-        elif (isinstance(gps,list) and len(gps)==len(self._detectors)):
-            if all((isinstance(_,(float,int)) and _ >=0) for _ in gps):
-                self._gps = gps
-        # ---> If not an error is raised.
-        else:
-            raise TypeError("gps has to be a list of positive numbers"
-                            +" with number of elements equal to detectors")
-                          
-                          
-        # -------------------------------------------------------------------- #
-        # --- duration check --------------------------------------------------#
-        
-        # # Duration is optional.
-        # ---> If not defined, we try to define with fs.
-        if duration == None:
-            # ---> Safe assumption can happen only on timeseries (2D).
-            if len(self._strain.shape) == 2:
-                self._duration = self._strain.shape[1]/int(self._fs)
-            # ---> If not definition is mandatory.
-            else:
-                raise TypeError("Duration of the input cannot be assumed ")
-        # ---> If it is defined, it has to be a number.
-        elif isinstance(duration,(int, float)):
-            self._duration = duration
-        # ---> If not an error is raised.
-        else:
-            raise TypeError("duration must be a float or int")
-                       
-                          
-        # -------------------------------------------------------------------- #
-        # --- metadata check --------------------------------------------------#
-        
-        # # Metadata is optinal and is a dictionary with exta information.
-        # ---> If defined it has to be a non empty dictionary.
-        if metadata == None:
-            self._metadata = None
-        elif isinstance(metadata,dict):
-            self._metadata = metadata
-        # ---> If not an error is raised.
-        else:
-            raise TypeError("metadata has to be a dictionary")
+            plt.figure(figsize=(15,7))#,facecolor='lightslategray')
+            if 'U' in self.detectors:
+                names = list('Strain '+str(i) for i in range(len(self.detectors)))
+            else:
+                names = list(det for det in self.detectors)
 
-    #                                                                          #
-    ### --- setters and getters ---------------------------------------------###   
-    #                                                                          #
+            plt.xlabel('Time')
+            plt.ylabel('Strain')
+            t=np.arange(0,self.duration,1/self.fs)
 
+            minim=0
+            for i in range(len(self.detectors)):
+                plt.plot(t,self.strain[i]+minim,color= colors[self.detectors[i]],label = names[i] )
+                minim =max(self.strain[i]+minim+abs(min(self.strain[i])))
+            plt.legend()
+            
+        elif type_ in dir(self):
+            
+            plugin=self.pluginDict[type_]
+            plugAttributes=[]
+            for at in plugin.plotAttributes:
+                plugAttributes.append(self.__getattribute__(at))
+            self.pluginDict[type_].plotFunction(*plugAttributes,data=self.__getattribute__(type_))
+        
+        else:
+            raise ValueError("The type specified is not present in the DataPod or it does not have a plot function.")
 
 
-    @property
-    def strain(self):
-        return self._strain                 
-    @strain.setter
-    def strain(self,whatever):
-        raise AttributeError("It is not encouraged to change the strain by "+
-                            "hand. If you really want to change them, use"+
-                            " ._strain instead. Strain did not change")
-
-    @property
-    def fs(self):
-        return self._fs
-    
-    @fs.setter
-    def fs(self,newfs):
-        # # fs has to be a valid number.
-        # ---> If fs is not a positive int and error is raised.
-        if isinstance(newfs, int) and newfs > 0:
-            self._fs = newfs 
-        else:
-            raise ValueError("Sample frequency must have no decimal part")
-
-    @property
-    def labels(self):
-        return self._labels
-    @labels.setter        
-    def labels(self, newLabels):
-        # # Labels are optional and it has to be a dictionary.
-        # ---> If a dictionary is given we have to make sure is not empty.
-        if isinstance(newLabels,dict):
-            if len(newLabels) == 0:
-                # ---> If it is empty we give the 'UNDEFINED' label.
-                print("Labels should have at least one element key \'type\'."
-                      +"\'UNDEFINED\' value has been set as \'type\'. ")
-                self._labels={'type':'UNDEFINED'} 
-            else:
-                self._labels=newLabels
-        # ---> If a non dictionary object is given, an error is called.
-        else:
-            raise TypeError("labels must be a dictionary")
-
-    @property
-    def detectors(self):
-        return self._detectors
-    @detectors.setter
-    def detectors(self,newDetectors):
-        # # If detectors is used, it has to be a list.
-        # ---> If it is not an error is raised.
-        if not isinstance(newDetectors,list): raise TypeError(
-            "detectors have to be a list of strings"+
-            " with at least one the followings as elements: \n"+
-            "'H' for LIGO Hanford \n'L' for LIGO Livingston\n"+
-            "'V' for Virgo \n'K' for KAGRA \n'I' for LIGO India (INDIGO) \n"+
-            "\n'U' if you don't want to specify detector")
             
-        # # Moreover it has to be a list containing specific detector initials.
-        # ---> If elements of detectors aren't in detector it gives an error. 
-        detectorOptions = ['H','L','V','K','I','U']
-        if isinstance(newDetectors,list):
-            for det in newDetectors:
-                if det not in detectorOptions: 
-                    raise ValueError(
-                        "detectors have to be a list of strings"+
-                        " with at least one the followings as elements: \n"+
-                        "'H' for LIGO Hanford \n'L' for LIGO Livingston\n"+
-                        "'V' for Virgo \n'K' for KAGRA \n'I' for LIGO India"+
-                        " (INDIGO) \n"+
-                        "\n'U' if you don't want to specify detector")
-        
-        # # The number of detectors must be shown at the first dimention.
-        if (self._strain.shape[0] == len(newDetectors)):
-            self._detectors = newDetectors
-        # ---> If it is not in the first dimention maybe needs transpose.
-        elif (self._strain.shape[0] != len(newDetectors)):
-            # ---> If the number of detectors is present at some dimention.
-            if ((len(newDetectors) in self._strain.shape) 
-                and self._strain.shape.count(len(newDetectors))==1):
-                # --- Then we traspose the strain.
-                newShape = list(self._strain.shape)
-                newShape.pop(newShape.index(len(newDetectors)))
-                newShape.insert(0,len(newDetectors))
-                ind = [list(self._strain.shape).index(i) for i in newShape]
-                self._strain = np.transpose(self._strain, ind)
-                print("Needed shape change of the strain occured")
-                self._detectors = newDetectors
-            # ---> If not, an error occures.
-            else:
-                raise IndexError("detectors must be as many as the strain")
-
-    @property
-    def gps(self):
-        return self._gps  
-    @gps.setter
-    def gps(self,newgps):
-        # # GPS is optional or a list of positive numbers. 
-        # ---> If it is a list, it has to include positive numbers.
-        if (isinstance(newgps,list) and len(newgps)==len(self._detectors)):
-            if all((isinstance(_,(float,int)) and _ >=0) for _ in newgps):
-                self._gps = newgps
-        # ---> If not an error is raised.
-        else:
-            raise TypeError("gps has to be a list of positive numbers"
-                            +" with number of elements equal to detectors")
-    @property
-    def duration(self):
-        return self._duration
-    @duration.setter
-    def duration(self,newDuration):
-        # ---> If it is defined, it has to be a number.
-        if isinstance(newDuration,(int, float)):
-            self._duration = newDuration
-        # ---> If not an error is raised.
-        else:
-            raise TypeError("duration must be a float or int")
-
-    @property
-    def metadata(self):
-        return self._metadata
-    @metadata.setter
-    def metadata(self,newMetadata):
-        # # Metadata is optinal and is a dictionary with exta information.
-        # ---> If defined it has to be a non empty dictionary.
-        if isinstance(newMetadata,dict):
-            if len(newMetadata.keys())!=0:
-                self._metadata = newMetadata
-            else: raise ValueError("metadata cannot be an empty dictionary")
-        # ---> If not an error is raised.
-        else:
-            raise TypeError("metadata has to be a dictionary")
-    
-    # --- extra usefull attributes ------------------------------------------- #
-    
-    @property
-    def shape(self):
-        return self._strain.shape
-                  
-    @property
-    def memory(self):
-        return self._strain.nbytes
-    
-    # --- __MAGIC_METHODS__ -------------------------------------------------- #
-
-    def __add__(self, num):
-        newPod = copy.copy(self)
-        if isinstance(num,(float,int)):
-            if not np.isfinite(num).all():
-                raise ValueError("inf or nan value is present")
-            else:
-                newPod._strain = newPod._strain + num
-                return(newPod)
-        elif isinstance(num,np.ndarray):
-            if not np.isfinite(num).all():
-                raise ValueError("inf or nan value is present")
-            if (num.shape == self._strain.shape):
-                newPod._strain = newPod._strain + num
-                return(newPod)
-            else:
-                raise IndexError("You cannot operate shape "+str(num.shape)
-                                +" with shape "+str(self._strain.shape))
-        else:
-            raise TypeError("Mathematical operations are not allowed with "
-                           +str(type(num))+"types. Only int, float or" 
-                           +" numpy.ndarray")
-            
-    def __iadd__(self, num):
-        return(self.__add__(num))
-    def __radd__(self, num):
-        return(self.__add__(num))        
-    def __sub__(self, num):
-        return(self.__add__(-num))      
-    def __isub__(self, num):
-        return(self.__add__(-num))
-    def __rsub__(self, num):
-        return(self.__add__(-num))
-        
-    def __mul__(self, num):
-        newPod = copy.copy(self)
-        if isinstance(num,(float,int)):
-            if not np.isfinite(num).all():
-                raise ValueError("inf or nan value is present")
-            else:
-                newPod._strain = newPod._strain * num
-                return(newPod)
-        elif isinstance(num,np.ndarray):
-            if not np.isfinite(num).all():
-                raise ValueError("inf or nan value is present")
-            if (num.shape == self._strain.shape):
-                newPod._strain = newPod._strain * num
-                return(newPod)
-            else:
-                raise IndexError("You cannot operate shape "+str(num.shape)
-                                +" with shape "+str(self._strain.shape))
-        else:
-            raise TypeError("Mathematical operations are not allowed with "
-                           +str(type(num))+"types. Only int, float or" 
-                           +" numpy.ndarray")
-    def __imul__(self, num):
-        return(self.__mul__(num))
-    def __rmul__(self, num):
-        return(self.__mul__(num))
-    
-
-    def __truediv__(self, num):
-        newPod = copy.copy(self)
-        if isinstance(num,(float,int)):
-            if not np.isfinite(num).all():
-                raise ValueError("inf or nan value is present")
-            elif num == 0:
-                raise ValueError("Division with zero encountered")                
-            else:
-                newPod._strain = newPod._strain / num
-                return(newPod)
-        elif isinstance(num,np.ndarray):
-            if not np.isfinite(num).all():
-                raise ValueError("inf or nan value is present")
-            elif (num==0).any():
-                raise ValueError("Division with zero encountered") 
-            if (num.shape == self._strain.shape):
-                newPod._strain = newPod._strain / num
-                return(newPod)
-            else:
-                raise IndexError("You cannot operate shape "+str(num.shape)
-                                +" with shape "+str(self._strain.shape))
-        else:
-            raise TypeError("Mathematical operations are not allowed with "
-                           +str(type(num))+"types. Only int, float or" 
-                           +" numpy.ndarray")
-            
-    def __itruediv__(self, num):
-        return(self.__truediv__(num))
-
-
-    
-    def __len__(self):
-        return(len(self._strain))
-        
-    # def __getitem__() --> It is moved to the main function DataPod
-
-    
-    def __delitem__(self,key):
-        if isinstance(key,int):
-            del self._strain[key]
-            del self._detectors[key]
-            del self._gps[key]
-        elif (isinstance(key,str) and (key in self._detectors) 
-             and key!='U'):
-            ind = self._detectors.index(key)
-            del self._strain[ind]
-            del self._detectors[ind]
-            del self._gps[ind]
-        else:
-            raise TypeErrro("index can be int or a detector name that exists")
-    def __copy__(self):
-        return self
-    #def __iter__(self)
-    #def __contains__(self,item)
-
+            
+            
 
-        
-        
-        
-class DataSetBase:
-    #                                                                          #             
-    ###--- STR & REPR methods -----------------------------------------------###        
-    #                                                                          #
+              
+class DataSet(DataSetBase):
     
-    def __str__(self):
-        statement=(str(len(self))+" instances with shape "
-                   +str(self.dataPods[0].shape)+"\n\n")
-        if len(self) > 5:
-            statement = statement + str(self._dataPods[0])+ "\n"
-            statement = statement + str(self._dataPods[1])+ "\n"
-            statement = statement + (9*" "+6*("."+9*" ")+".\n")
-            statement = statement + (9*" "+6*("."+9*" ")+".\n")
-            statement = statement + (9*" "+6*("."+9*" ")+".\n\n")
-            statement = statement + str(self._dataPods[-2])+ "\n"
-            statement = statement + str(self._dataPods[-1])+ "\n"            
-        else:
-            for pod in self._dataPods:
-                statement = statement + str(pod)      
-        return (statement)
+    """DataSet is an object that helps manipulate groups of DataPods as a whole.
+    The main attribute is a list of the DataPods. All methods are providing ways
+    to manipulate the data and export them to desired shapes. 
     
-    def __repr__(self):
-        statement=(str(len(self))+" instances with shape "
-                   +str(self.dataPods[0].shape)+"\n\n")
-        if len(self) > 5:
-            statement = statement + str(self._dataPods[0])+ "\n"
-            statement = statement + str(self._dataPods[1])+ "\n"
-            statement = statement + (9*" "+6*("."+9*" ")+".\n")
-            statement = statement + (9*" "+6*("."+9*" ")+".\n")
-            statement = statement + (9*" "+6*("."+9*" ")+".\n\n")
-            statement = statement + str(self._dataPods[-2])+ "\n"
-            statement = statement + str(self._dataPods[-1])+ "\n"            
-        else:
+    Attributes
+    ----------
+    
+    dataPods: list of DataPod objects (optional)
+        List of the DataPod objects to be part of this DataSet instance. All 
+        DataPods are checked for inconsistences such as different shapes, 
+        different number of detectors and different sample frequencies.
+    
+    name: str (optional)
+        The name of the DataSet
+    
+    """
+    
+    
+    def __getitem__(self,index):
+        if isinstance(index,int):
+            return self._dataPods[index]
+        elif isinstance(index,slice):
+            return DataSet(self._dataPods[index])
+        elif (isinstance(index,list) 
+              and all(isinstance(det,str) for det in index)):
+            newPods=[]
             for pod in self._dataPods:
-                statement = statement + str(pod)      
-        return (statement)
+                newPods.append(pod[index])
+            return(DataSet(newPods))
+                
     
-    #                                                                          #             
-    ###--- INIT method ------------------------------------------------------###        
-    #                                                                          #
+    # --- saving method -------------------------------------------------------#
     
-    def __init__(self, dataPods=None, name = None):
-        # data check
-        if isinstance(dataPods,list):
-            if all(isinstance(x , DataPodBase) for x in dataPods):
-                self._dataPods = dataPods
+    def save(self, name = None,type_ = 'pkl'):
+        
+        """Method to save the DataSet.
+        
+        Parameters
+        -------------
+        name : str  (optional)
+            Name of the file to be saved. If not specified the name becomes the 
+            name attribute.
+        
+        type_ : '.pkl'
+            The format to save the DataSet. Currently available only as pkl.
+        
+        """       
+        if name == None : name= self.name
+        if name == None:
+            finalName = 'dataSetNameToken'+str("%04d" %
+                (np.random.randint(0,10000)))+'.'+type_
+        else:
+            finalName = name
+        if type_ == 'pkl':
+            if finalName[-4:]!='.pkl':
+                finalName+='.pkl'
+            with open(finalName, 'wb') as output:
+                pickle.dump(self, output, pickle.HIGHEST_PROTOCOL)
+        else:
+            raise TypeError("."+type_+" files are not supported for saving")
+            
+    # --- loading method ------------------------------------------------------#    
+    
+    # needs chop
+    def load(filename, source = 'file'):
+        
+        """Method to load a DataSet object
+        
+        Parameters
+        -------------
+        filename : str (path)
+            Path to the file.
+        
+        """
+        
+        if source == 'file':
+            if ".pkl" in filename:
+                with open(filename,'rb') as obj:
+                    set_ = pickle.load(obj)
+                if isinstance(set_,DataSet):
+                    return(set_)
+                else:
+                    raise TypeError("Object in file is not a DataSet object")
             else:
-                raise ValueError("List has elements that are not DataPods")
+                raise TypeError("Only .pkl files are supported for loading")
+                
+        elif source == 'directory':
+            
+            det=dirlist(filename)
+            if filename[-1] == '/' : filename.pop[-1]
+            detectors=[]
+            for i in range(len(det)):
+                if det[i] in ['H','L','V','K','I',]:
+                    detectors.append(det[i])
+            if len(detectors)==0: 
+                raise ValueError("Directory does't have detector data")
                 
-        elif (dataPods == None):
-                self._dataPods = []
+            filelist=[]
+            for det in detectors:
+                filelist.append(dirlist(filename +'/'+ det))
+
+            filelist = np.asarray(filelist)
+            index=np.arange(len(filelist[0]))
+            np.random.shuffle(index)
+            for i in range(len(filelist)):
+                filelist[i] = filelist[i,index]
+
+            pods=[]      
+            for i in range(len(filelist[0])):
+
+                data=[]  
+                for det in detectors:
+                    data.append( np.loadtxt(filename+'/'+det+'/'+filelist[detectors.index(det)][i]).tolist())
+                pod = DataPod( data 
+                               , fs =2048 , labels={'type': 'injection'}
+                               , detectors = ['H','L','V']
+                               , gps =None
+                               , metadata = {'source file':filename})
+                pods.append(pod)
+
+            set_=DataSet(pods)
+            return set_
         else:
-            raise TypeError("DataSet object has to be a list of DataPods")
+            raise ValueError("source can be a 'file' or a 'directory'")
             
-        # name check
-        if name == None:
-            self._name = 'NoName'
-        elif isinstance(name, str):
-            self._name = name
-        else:
-            raise TypeError("name must be a str")
-        
-        # pods similarity check --
-        if len(self._dataPods) !=0:
-            pod0=self._dataPods[0]
-            for pod in self._dataPods:
+    # --- add method ---------------------------------------------------------#    
+    
+    def add(self, newData):
+        """This method works similarly to how append works in lists. You can
+        add a new DataPod or a new DataSet.
+            
+        
+        
+        """
+        if isinstance(newData,DataPod):
+            if self.dataPods==[]:
+                pod0 = newData
+            else:
+                pod0=self.dataPods[0]
+            if newData.shape != pod0.shape:
+                print("Pods with different shapes")
+            elif newData.fs != pod0.fs:
+                print("Pods woth different sample frequencies")
+            else:
+                self.dataPods.append(newData)
+        elif isinstance(newData, DataSet):
+            pod0=self.dataPods[0]
+            for pod in newData:
                 if pod.shape != pod0.shape:
                     print("Pods with different shapes")
                 if pod.fs != pod0.fs:
-                    print("Pods with different sample frequencies")
+                    print("Pods woth different sample frequencies")
                 if not all(d in pod0.detectors for d in pod.detectors):
                     print("Pods with different detectors")
+                else:
+                    pass
+            self.dataPods += newData.dataPods
+
+        else:
+            raise TypeError("Appended object is not a DataPod or Dataset")
+            
+    def addPlugIn(self,*args):
+        """Method to add PlugIn objects to the dataPod. PlugIn objects are extra
+        data derived either from the already existing data in the pod or tottaly
+        new ones. You can add a simple value to generation function and also a 
+        plot function if you need to plot the new data.
+
+        Parameters
+        ----------
+
+        *args: PlugIn objects
+            The PlugIn objects that you have already defined and you want to add
+            on the pod.
+
+        """
+        for plugin in args:
+            if not isinstance(plugin,PlugIn):
+                raise TypeError("Inputs must be PlugIn objects")
+                
+        for plugin in args:
+            plugAttributes=[]
+            for at in plugin.attributes:
+                if at in dir(self.dataPods[0]):
+                    for pod in self.dataPods:
+                        pod.addPlugIn(plugin)
+                else:
+                    raise AttributeError(at+" is not part of DataPod instance")
+
+            self.pluginDict[plugin.name]=plugin
+            
+           
+    # --- fusion method --        
+    def fusion(elements, sizes = None, save = None):
+        
+        if not isinstance(elements,list): raise TypeError(
+            "The fusion input must be a list containing either DataSet "+
+            "object or file names, you can also have both")
+        
+        for element in elements:
+            if isinstance(element, str):
+                if not (os.path.isfile(element)):
+                    raise FileNotFoundError("File "+element+" not found")
+                elif not (".pkl" in element):
+                    raise TypeError("File must be of the .pkl type")
+            elif isinstance(element, DataSet):
+                pass
+            else:
+                raise TypeError("The fusion input must be a list "
+                    +"containing either DataSet object or file names,"
+                    +" you can also have both")
+        
+        if isinstance(save, str):
+            pass
+        elif save == None:
+            pass
+        else:
+            raise TypeError("save value can be a str or None")
+                
+        if sizes == None:
+            pass
+        else:
+            if isinstance(sizes,list):
+                if all(isinstance(x,int) for x in sizes):
+                    if len(sizes) == len(elements):
+                        pass
+                    else:
+                        raise TypeError("sizes must be equal in number "
+                                        +"to the DataSets to fuse")
+                else:
+                    raise TypeError("sizes must be a list of integers or None")
+            else:
+                raise TypeError("sizes must be a list of integers or None")
+        
+        datasets=[]
+        for i in range(len(elements)):
+            if isinstance(elements[i], str):
+                set_=DataSet.load(elements[i])
+            elif isinstance(elements[i], DataSet):
+                set_=elements[i]
+            else:
+                raise TypeError("element is not what expected")
+            if sizes == None:
+                datasets += set_._dataPods
+            else:
+                datasets += set_._dataPods[:sizes[i]]
+            del set_
+
+        random.shuffle(datasets)
+        finalSet = DataSet(datasets)
+        
+        if isinstance(save,str):
+            finalSet.save(name= save)        
+        
+        return(finalSet)
 
-
+    # --- filterGPS method --------------------------------------------------- #
     #                                                                          #
-    ### --- setters and getters ---------------------------------------------###
+    # This method clears the DataSet from DataPods that include specific GPS   #
+    # times. This can be done selectively for specific ditectors. The times    #
+    # and intervals stated in filterTimes parameter are rejected for the       #
+    # detectors stated in detectors parameter. The window parameter adds extra #
+    # opotional discrimination at the intervals to be rejected.                #
     #                                                                          #
-
-    @property
-    def dataPods(self):
-        return self._dataPods                 
-
-    @property
-    def name(self):
-        return self._name 
+    # ------------------------------------------------------------------------ #
+    def filterGPS(self, filterTimes, detectors = None, window=0):
+        
+        if isinstance(filterTimes, (int,float)):
+            fitlertTimes = [filterTimes]
+        elif (isinstance(filterTimes, list) and all(
+            isinstance(x,(int,float,list)) for x in filterTimes)):
+            for x in filterTimes:
+                if isinstance(x,list):
+                    if not (len(x)==2 and all(
+                        isinstance(t,(int,float)) for t in x) and x[1]>x[0]):
+                         raise TypeError(
+                             "filterTimes must be a list including gps times"
+                            +" or intervals of gps times in the form of lists"
+                             +" [start,end)")
+        else:
+             raise TypeError(
+                 "filterTimes must be a list including gps times"
+                +" or intervals of gps times in the form of lists [start,end)")
+        
+        if detectors != None:
+            if isinstance(detectors,str): detectors = [detectors]
+            if not (isinstance(detectors,list) 
+                    and all(d in ['H','L','V','K','I','U'] for d in detectors)):
+                raise TypeError(
+                "detectors have to be a list of strings"+
+                " with at least one the followings as elements: \n"+
+                "'H' for LIGO Hanford \n'L' for LIGO Livingston\n"+
+                "'V' for Virgo \n'K' for KAGRA \n'I' for LIGO India"+
+                " (INDIGO) \n\n'U' if you don't want to specify detector")
+
+        
+        rejectionInterval=SegmentList()
+        for tm in filterTimes:
+            if not isinstance(tm,list):
+                rejectionInterval.append(Segment(tm-0.5,tm+0.5))
+            else:
+                rejectionInterval.append(Segment(tm[0],tm[1]))
+        rejectionInterval.coalesce()
+        filteredPods=[]
+        for i in range(len(self.dataPods)):
+            exlusion = False
+            
+            if detectors==None:
+                for j in range(len(self.dataPods[i].detectors)):
+                    if rejectionInterval.intersects_segment(Segment(
+                        self.dataPods[i].gps[j]-window,
+                        self.dataPods[i].gps[j]+
+                        self.dataPods[i].duration+window)):
+                        exlusion = True
+    
+            else:
+                for d in detectors:
+                    ind = self.dataPods[i].detectors.index(d)
+                    if rejectionInterval.intersects_segment(Segment(
+                        self.dataPods[i].gps[ind]-window,
+                        self.dataPods[i].gps[ind]+
+                        self.dataPods[i].duration+window)):
+                        exlusion = True
+            
+            if exlusion == False:
+                filteredPods.append(self.dataPods[i])
+                
+        self._dataPods=filteredPods
+        print("Given GPS times, no longer in DataSet")
     
-
-    @dataPods.setter
-    def dataPods(self,whatever):
-        raise AttributeError("It is not encouraged to change the DataSet by "+
-                            "hand. If you really want to change them, use"+
-                            " ._dataPods instead. DataSet did not change")
-    @name.setter
-    def name(self,newname):
-        if isinstance(newname, str):
-            self._name = newname
-        else:
-            raise TypeError("name must be a str")    
+    def filterDetector(self,detectors):
+        
+        if isinstance(detectors,str): detectors = [detectors]
+        if not (isinstance(detectors,list) 
+                and all(d in ['H','L','V','K','I','U'] for d in detectors)):
+            raise TypeError(
+            "detectors have to be a list of strings"+
+            " with at least one the followings as elements: \n"+
+            "'H' for LIGO Hanford \n'L' for LIGO Livingston\n"+
+            "'V' for Virgo \n'K' for KAGRA \n'I' for LIGO India (INDIGO) \n"+
+            "\n'U' if you don't want to specify detector")
             
-
-    def duration(self):
-        return self.dataPods[0].duration
+        for i in range(len(self.dataPods)):
+            for d in detectors:
+                ind = self.dataPods[i].detectors.index(d)                
+                self._dataPods[i]._strain = np.delete(self._dataPods[i]._strain
+                                                      , ind , 0)
+                self._dataPods[i]._detectors = np.delete(
+                    self._dataPods[i]._detectors, ind, 0)
+                self._dataPods[i]._gps = np.delete(self._dataPods[i]._gps
+                                                   , ind, 0)
+        message = "Detector"
+        if len(detectors)==1:
+            message+=" "
+        else:
+            message+="s "
+        for d in detectors:
+            message+=(d+", ")
+        message += "no longer in this DataSet"
+        print(message)
+        
+    def filterLabel(self,labels):
+        
+        if not (isinstance(labels, dict) and len(labels)>0):
+            raise ValueError("labels have to be a dict with at least"
+                             +" one key-value pare")
+        
+        finalPods=[]
+        for i in range(len(self._dataPods)):
+            
+            same = 0
+            for j in range(len(self._dataPods[i].labels)):
+                for k in range(len(labels)):
+                    if ((list(labels.keys(
+                    ))[k]==list(self._dataPods[i].labels.keys())[j])
+                        and (labels[list(labels.keys(
+                        ))[k]]==self._dataPods[i].labels[list(
+                            self._dataPods[i].labels.keys())[j]])):
+                        same+=1
+            if same == len(labels):
+                finalPods.append(self._dataPods[i])
+                
+        self._dataPods = finalPods
         
-    # def __getitem__() --> It is moved to the main function DataSets
-    
-    def __len__(self):
-        return(len(self._dataPods))
 
-    def selfcheck(self):
-        pod0=self.dataPods[0]
-        check = True
+    def exportData(self,plugin=None, shape = None):
+
+        goods =[]
+        if plugin==None:
+            for pod in self.dataPods:
+                goods.append(pod.strain.tolist())
+            goods=np.array(goods)                
+
+        elif isinstance(plugin,str):
+            for pod in self.dataPods:
+                goods.append(pod.__getattribute__(plugin))
+            goods=np.array(goods)
+        else:
+            raise ValueError('PlugIn '+str(plugin)+' not present in DataPod')
+            
+        if shape == None:
+            shape = goods.shape
+            shape = tuple([None]+list(shape[1:]))
+        # print("goods.shape",goods.shape)
+        if isinstance(shape,tuple):
+            if all(((dim in goods.shape) or dim==None) for dim in shape):
+                shapeList = list(shape)
+                goodsShapeList = [None]+list(goods.shape)[1:]
+                newIndex = list(shapeList.index(goodsShapeList[i]) for i in range(len(shape)))
+                goods = np.transpose(goods, newIndex)
+            else:
+                raise ValueError("Shape values are not the same as the DataSet shape")
+
+        else:
+            raise TypeError("Not valid shape.")
+        print("DataSet with shape "+str(goods.shape)+" is exported")
+        return(goods)
+    
+    def exportLabels(self,*args,reshape=False):
+        # Checking the types of labels and how many
+        # pods have the specific label.
+        labelOccur={}
         for pod in self.dataPods:
-            if pod.shape != pod0.shape:
-                print("Pods with different shapes")
-                check = False
-            if pod.fs != pod0.fs:
-                print("Pods with different sample frequencies")
-                check = False
-            if not all(d in pod0.detectors for d in pod.detectors):
-                print("Pods with different detectors")
-        if check == True:
-            print("All good")
-        return(check)
-                      
+            for key in list(pod.labels.keys()):
+                if key not in list(labelOccur.keys()): labelOccur[key]=0
+                labelOccur[key]+=1
+        # 'type' is a default label
+        if len(args)==0: args=('type',)    
+        for arg in args:
+            # labels must be strings
+            if not isinstance(arg,str):
+                raise TypeError("Label keys must be strings")
+            # if a label type doesn't exist an error is raised
+            if not arg in list(labelOccur.keys()):
+                raise KeyError("There is no label key "+str(arg))
+            # The label type must occur as many times as the size of the dataset
+            if labelOccur[arg]!=len(self):
+                raise ValueError(str(len(self)-labelOccur[arg])
+                                 +" pods don't have the label "+str(arg)+" defined")
+                
+        goods=[]
+        for i in range(len(self)):
+            if len(args)>1:
+                label=[]
+                for arg in args:
+                    label.append(self[i].labels[arg])
+            else:
+                label=self[i].labels[arg]
+            goods.append(label)
+        goods=np.asarray(goods)
+        # reshaping in case only one label is required
+        if (len(args)==1 and reshape==True): goods=goods.reshape((len(goods),1))
+        print("Labels "+str(list(args))+" with shape "+str(goods.shape)+" are exported")
+        return goods
+   
+    def exportGPS(self):
+        goods =[]
+        for pod in self.dataPods:
+            goods.append(pod.gps)
+        return goods
+        
+ 
+    def stackDetector(self,**kwargs):
+        kwargs['size']=len(self)
+        if 'duration' not in kwargs: kwargs['duration']=self[0].duration
+        if 'fs' not in kwargs: kwargs['fs']=self[0].fs   
+        if 'detectors' not in kwargs: 
+            raise ValueError("You need to at least specify a detector")
+
+        if 'plugins' not in kwargs: kwargs['plugins']=[]
+        if 'psd' in self[0].pluginDict and 'psd' not in kwargs['plugins']: kwargs['plugins'].append('psd')
+        # if 'snr'+self[0].detectors[0] in self[0].pluginDict and 'snr' not in kwargs['plugins']: 
+        #     kwargs['plugins'].append('snr')
+        
+
+        newSet=generator(**kwargs)
+
+        for i in range(len(self)):
+            self[i].strain=np.vstack((self[i].strain,newSet[i].strain))
+            self[i].detectors+=newSet[i].detectors
+            self[i].gps+=newSet[i].gps
+            if 'psd' in kwargs['plugins']: self[i].psd+=newSet[i].psd
+            # if 'snr' in kwargs['plugins']:
+            #     for d in newSet[i].detectors:
+            #         self[i].addPlugIn(newSet[i].pluginDict['snr'+d])        
+            if 'correlation' in self[i].pluginDict:
+                self[i].addPlugIn(self[i].pluginDict['correlation'])   
+
```

### Comparing `mly-0.1.1/mly/datatools.py` & `mly-0.3.1/mly/datatools/generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,1102 +1,1282 @@
-from .core import DataPodBase
-from .core import DataSetBase
-from .tools import dirlist, index_combinations, correlate
-from .simulateddetectornoise import *  
-from gwpy.timeseries import TimeSeries
-import matplotlib.pyplot as plt
-from matplotlib.mlab import psd
-from scipy.stats import pearsonr
-from scipy.special import comb
+from ..simulateddetectornoise import *  
+from ..tools import dirlist, internalLags, correlate
+from ..plugins import *
+
+from .datatools import DataSet, DataPod
 
-import numpy as np
-import pickle
 import os
-import sys
 import time
+import gwdatafind
+import pickle
 import random
 import copy
+import string
+
+import numpy as np
+import matplotlib.pyplot as plt
+
+from pathlib import Path
 from math import ceil
+from pycondor import Job, Dagman
 
-################################################################################
-#  TODO:You have to make nan checks to the injection files and noise files 
-#  before running the generator function.
-# 
-#  auto_gen does not work on optimal noise
-################################################################################
+from matplotlib.mlab import psd
+from gwpy.time import to_gps, from_gps
+from gwpy.timeseries import TimeSeries
+from gwpy.segments import Segment,SegmentList,DataQualityFlag
+from dqsegdb2.query import query_segments
+from scipy.stats import pearsonr
+from scipy.special import comb
+from urllib.error import HTTPError
 
-class DataPod(DataPodBase):
 
-    '''
-        DataPod is an object to consentrate all the information of a data.
-    instance. The reason for their creation is to encapsulate all the usefull
-    attributes a machine learning algorithm will need. Getting them together 
-    into DataSet objects creates a powerfull tool to simplify machine learning
-    training and testing procedures for any kind of network.
-    
-    
-    strain:   (numpy.ndarray / gwpy.timeseries.TimeSeries / list)
-              The main data of the pod. It can be a timeseries or a picture or 
-              anything with fixed dimentions. Finally it checks the input for 
-              nans and infs and returns errors if the data have size or value
-              problems.
-            
-    fs:       (int)
-              This is the sample frequency of the data. It is used to determine 
-              the duration of the of the strain input. If the strain is not a
-              time series it is not used anywhere.
-            
-    labels:   (dict)[optional] 
-              It determines the main labels of the DataPod. These labels will be
-              used by algorithms for classification. If empty, a label called 
-              "UNDEFINED" is given. Suggested keys for labels are the following:
-              
-              { 'type' : ('noise' , 'cbc' , 'signal' , 'burst' , 'glitch', ...),
-                'snr'  : ( any int or float number bigger than zero),
-                'delta': ( Declination for sky localisation, float [-pi/2,pi/2])
-                'ra'   : ( Right ascention for sky licalisation float [0,2pi) )}
-                
-              For all labels, keys and values are not case sensitive.
-            
-    detectors:(list)[optional]
-              If the strain belongs to a specific detector it is suggested to 
-              state which detector is it. If it not specified the number of 
-              detectors is assumed to be the smallest strain dimention and a
-              list of 'U' is set with length equal to the detector number that 
-              was assumed. The first dimention of every strain must be the 
-              number of detectors involved. If it's not a check takes place to
-              see if the dimention is somewhere else. If it is we the strain is
-              transposed.
-              
-    gps      :(int / float)[optional]
-              The gps time of each of the detector strains. If not defined a
-              list of zeros with length equal to detectors is defined. It has to
-              be a possitive number.
-    
-    duration :(int / float)[optinal for timeseries]
-              The duration in seconds of the strain. If the strain is more than
-              2D in shape the duration has to be difined independently.
-              
-    metadata :(dict)[optional]
-              A dictionary with additional infromation about the pod.
-    '''
-    
-    
-        
-    def __getitem__(self,index):
-        if isinstance(index,int): index=slice(index,None,None)
-        if isinstance(index,slice):
-            return self._strain[index]
-        elif isinstance(index,list) and all((isinstance(det,str) and (det in self._detectors) 
-             and det!='U') for det in index):
-            newStrain=[]
-            newGPS=[]
-            newMeta=copy.deepcopy(self.metadata)
-            ignoredDetectors=[]
-            for d in self.detectors:
-                if not (d in index) : ignoredDetectors.append(d)
-            for det in index:
-                ind = self._detectors.index(det)
-                newStrain.append(self._strain[ind])
-                newGPS.append(self.gps[ind])
-            for d in ignoredDetectors:
-                for key in newMeta:
-                    if isinstance(newMeta[key],dict) and len(self.metadata[key])==len(self.detectors):
-                        del newMeta[key][d]
-            return(DataPod(newStrain,fs=self.fs,labels=copy.deepcopy(self.labels)
-                           ,gps = newGPS,detectors=index
-                           ,duration=self.duration
-                           ,metadata=newMeta))
-        else:
-            raise TypeError("index can be int or a list with detector names that exists")
-    
-      
-    # --- saving method ------------------------------------------------------ #
-    
-    def save(self, name='',type_ = 'pkl'):
-        if name == '':
-            finalName = 'dataPodNameToken'+str("%04d" %
-                (np.random.randint(0,10000)))+'.'+type_
-        elif ('.pkl' == name[-4:]) or ('.txt' == name[-4:]):
-            finalName = name[:-4]
-        else:
-            finalName = name
-            
-        if type_ == 'pkl':
-            with open(finalName+'.pkl', 'wb') as output:
-                pickle.dump(self, output, pickle.HIGHEST_PROTOCOL)
-        elif type_ == 'txt':
-            np.savetxt(finalName+'.txt', self.strain)
-        else:
-            raise TypeError("."+type_+" files are not supported for saving")
-            
-    # --- loading method ------------------------------------------------------#    
-    
-    def load(filename):
-        if ".pkl" in filename:
-            with open(filename,'rb') as obj:
-                a = pickle.load(obj)
-            return(a)
-        elif ".txt" in filename:
-            nArray = np.loadtxt(filename)
-            return(nArray)
-        else:
-            raise TypeError("Only .pkl files are supported for loading")
-            
-    def plot(self,type_='strain'):
-        
-        colors = {'H': '#ee0000','L':'#4ba6ff','V':'#9b59b6','K':'#ffb200','I':'#b0dd8b','U':'black'}
-        names=[]
-        plt.figure(figsize=(15,7))#,facecolor='lightslategray')
-        if type_ == 'strain':
-            if 'U' in self.detectors:
-                names = list('Strain '+str(i) for i in range(len(self.detectors)))
-            else:
-                names = list(det for det in self.detectors)
 
-            plt.xlabel('Time')
-            plt.ylabel('Strain')
-            t=np.arange(0,self.duration,1/self.fs)
-
-            minim=0
-            for i in range(len(self.detectors)):
-                plt.plot(t,self.strain[i]+minim,color= colors[self.detectors[i]],label = names[i] )
-                minim =max(self.strain[i]+minim+abs(min(self.strain[i])))
-            plt.legend()
-            
-        elif type_ =='psd' and ('psd' in list(self.metadata.keys())):
-            if 'U' in self.detectors:
-                names = list('PSD '+str(i) for i in range(len(self.detectors)))
-            else:
-                names = list(det for det in self.detectors)
 
-            plt.xlabel('Frequency')
-            plt.ylabel('Power Spectral Density')
-            colors = {'H': '#ee0000','L':'#4ba6ff','V':'#9b59b6','K':'#ffb200','I':'#b0dd8b','U': 'black'}
-            f=np.arange(0,int(self.fs/2)+1)
-
-            #minim=0
-            for det in self.detectors:
-                plt.loglog(f,self.metadata['psd'][self.detectors.index(det)],color= colors[det]
-                           ,label = names[self.detectors.index(det)] )
-                #minim =max(self.strain[i]+minim+abs(min(self.strain[i])))
-            plt.legend()
-        elif type_ =='psd' and not ('psd' in list(self.metadata.keys())):
-            raise KeyError("psd key is not pressent in the pod")
-            
-            
-        elif type_ =='correlation' and ('correlation' in list(self.metadata.keys())):
 
-            plt.xlabel('Time Shift')
-            plt.ylabel('Pearson Correlation')
-            tlength=len(self.metadata['correlation'][0])/self.fs
-            tarray=np.arange(-tlength/2,tlength/2,1/self.fs)
-            count_=0
-            for i in np.arange(len(self.detectors)):
-                for j in np.arange(i+1,len(self.detectors)):
-                    plt.plot(tarray,self.metadata['correlation'][count_]
-                             ,label=str(self.detectors[i])+str(self.detectors[j]))
-                    plt.legend()
-                    count_+=1
+def injection_initialization(injection_source, detectors):
 
-            
-            
-class DataSet(DataSetBase):
-    
-    
-    def __getitem__(self,index):
-        if isinstance(index,int):
-            return self._dataPods[index]
-        elif isinstance(index,slice):
-            return DataSet(self._dataPods[index])
-        elif (isinstance(index,list) 
-              and all(isinstance(det,str) for det in index)):
-            newPods=[]
-            for pod in self._dataPods:
-                newPods.append(pod[index])
-            return(DataSet(newPods))
-                
-    
-    # --- saving method -------------------------------------------------------#
-    
-    def save(self, name = None,type_ = 'pkl'):
-        if name == None : name= self.name
-        if name == None:
-            finalName = 'dataSetNameToken'+str("%04d" %
-                (np.random.randint(0,10000)))+'.'+type_
-        else:
-            finalName = (name+'.'+type_)
-        if type_ == 'pkl':
-            with open(finalName, 'wb') as output:
-                pickle.dump(self, output, pickle.HIGHEST_PROTOCOL)
-        else:
-            raise TypeError("."+type_+" files are not supported for saving")
-            
-    # --- loading method ------------------------------------------------------#    
-    
-    def load(filename, source = 'file'):
-        if source == 'file':
-            if ".pkl" in filename:
-                with open(filename,'rb') as obj:
-                    set_ = pickle.load(obj)
-                if isinstance(set_,DataSet):
-                    return(set_)
-                else:
-                    raise TypeError("Object in file is not a DataSet object")
-            else:
-                raise TypeError("Only .pkl files are supported for loading")
-                
-        elif source == 'directory':
-            
-            det=dirlist(filename)
-            if filename[-1] == '/' : filename.pop[-1]
-            detectors=[]
-            for i in range(len(det)):
-                if det[i] in ['H','L','V','K','I',]:
-                    detectors.append(det[i])
-            if len(detectors)==0: 
-                raise ValueError("Directory does't have detector data")
-                
-            filelist=[]
-            for det in detectors:
-                filelist.append(dirlist(filename +'/'+ det))
+    '''Processing of the injection format in the generator
 
-            filelist = np.asarray(filelist)
-            index=np.arange(len(filelist[0]))
-            np.random.shuffle(index)
-            for i in range(len(filelist)):
-                filelist[i] = filelist[i,index]
+    '''
 
-            pods=[]      
-            for i in range(len(filelist[0])):
+    if injection_source == None:
+        inj_type = None
 
-                data=[]  
-                for det in detectors:
-                    data.append( np.loadtxt(filename+'/'+det+'/'+filelist[detectors.index(det)][i]).tolist())
-                pod = DataPod( data 
-                               , fs =2048 , labels={'type': 'injection'}
-                               , detectors = ['H','L','V']
-                               , gps =None
-                               , metadata = {'source file':filename})
-                pods.append(pod)
+    # Path input
+    elif isinstance(injection_source, str): 
 
-            set_=DataSet(pods)
-            return set_
-        else:
-            raise ValueError("source can be a 'file' or a 'directory'")
-            
-    # --- add method ---------------------------------------------------------#    
-    
-    def add(self, newData):
-        if isinstance(newData,DataPod):
-            if self._dataPods==[]:
-                pod0 = newData
-            else:
-                pod0=self._dataPods[0]
-            if newData.shape != pod0.shape:
-                print("Pods with different shapes")
-            elif newData.fs != pod0.fs:
-                print("Pods woth different sample frequencies")
+        # directory with pods path
+        if os.path.isdir(injection_source):
+
+            if injection_source[-1] != "/": injection_source+="/" 
+
+            if all(os.path.isdir(injection_source+det) for det in detectors):
+
+                inj_type = 'oldtxt'
             else:
-                self._dataPods.append(newData)
-        elif isinstance(newData, DataSet):
-            pod0=self._dataPods[0]
-            for pod in newData:
-                if pod.shape != pod0.shape:
-                    print("Pods with different shapes")
-                if pod.fs != pod0.fs:
-                    print("Pods woth different sample frequencies")
-                if all(d in pod0.detectors for d in pod.detectors):
-                    print("Pods with different detectors")
+                inj_type = 'directory'
+
+        # dataPod or dataSet path
+        elif (os.path.isfile(injection_source) and injection_source[-4:]=='.pkl'):
+            with open(injection_source,'rb') as obj:
+                injection_source = pickle.load(obj)
+
+            if isinstance(injection_source,DataPod):
+                injection_source = 'DataPod'
+            
+            elif isinstance(ç,DataSet):
+                if len(injection_source) > 0:
+                    inj_type = 'DataSet'
                 else:
-                    self._dataPods.append(newData.dataPods)
-        else:
-            raise TypeError("Appended object is not a DataPod or Dataset")
-            
-            
-            
-    # --- fusion method --        
-    def fusion(elements, sizes = None, save = None):
-        
-        if not isinstance(elements,list): raise TypeError(
-            "The fusion input must be a list containing either DataSet "+
-            "object or file names, you can also have both")
-        
-        for element in elements:
-            if isinstance(element, str):
-                if not (os.path.isfile(element)):
-                    raise FileNotFoundError("File "+element+" not found")
-                elif not (".pkl" in element):
-                    raise TypeError("File must be of the .pkl type")
-            elif isinstance(element, DataSet):
-                pass
-            else:
-                raise TypeError("The fusion input must be a list "
-                    +"containing either DataSet object or file names,"
-                    +" you can also have both")
-        
-        if isinstance(save, str):
-            pass
-        elif save == None:
-            pass
-        else:
-            raise TypeError("save value can be a str or None")
-                
-        if sizes == None:
-            pass
+                    raise ValueError("injection_source DataSet is empty")
+
         else:
-            if isinstance(sizes,list):
-                if all(isinstance(x,int) for x in sizes):
-                    if len(sizes) == len(elements):
-                        pass
-                    else:
-                        raise TypeError("sizes must be equal in number "
-                                        +"to the DataSets to fuse")
-                else:
-                    raise TypeError("sizes must be a list of integers or None")
-            else:
-                raise TypeError("sizes must be a list of integers or None")
-        
-        datasets=[]
-        for i in range(len(elements)):
-            if isinstance(elements[i], str):
-                set_=DataSet.load(elements[i])
-            elif isinstance(elements[i], DataSet):
-                set_=elements[i]
-            else:
-                raise TypeError("element is not what expected")
-                
-            if sizes == None:
-                datasets += set_._dataPods
-            else:
-                datasets += set_._dataPods[:sizes[i]]
-        random.shuffle(datasets)
-        finalSet = DataSet(datasets)
+            raise FileNotFoundError('Not valid directory for :'+injection_source)
         
-        if isinstance(save,str):
-            finalSet.save(name= save)        
-        
-        return(finalSet)
+    # DataSet                     
+    elif isinstance(injection_source,DataSet):
 
-    # --- filterGPS method --------------------------------------------------- #
-    #                                                                          #
-    # This method clears the DataSet from DataPods that include specific GPS   #
-    # times. This can be done selectively for specific ditectors. The times    #
-    # and intervals stated in filterTimes parameter are rejected for the       #
-    # detectors stated in detectors parameter. The window parameter adds extra #
-    # opotional discrimination at the intervals to be rejected.                #
-    #                                                                          #
-    # ------------------------------------------------------------------------ #
-    def filterGPS(self, filterTimes, detectors = None, window=0):
-        
-        if isinstance(filterTimes, (int,float)):
-            fitlertTimes = [filterTimes]
-        elif (isinstance(filterTimes, list) and all(
-            isinstance(x,(int,float,list)) for x in filterTimes)):
-            for x in filterTimes:
-                if isinstance(x,list):
-                    if not (len(x)==2 and all(
-                        isinstance(t,(int,float)) for t in x) and x[1]>x[0]):
-                         raise TypeError(
-                             "filterTimes must be a list including gps times"
-                            +" or intervals of gps times in the form of lists"
-                             +" [start,end)")
+        if len(injection_source) > 0:
+            inj_type = 'DataSet'
         else:
-             raise TypeError(
-                 "filterTimes must be a list including gps times"
-                +" or intervals of gps times in the form of lists [start,end)")
-        
-        if detectors != None:
-            if isinstance(detectors,str): detectors = [detectors]
-            if not (isinstance(detectors,list) 
-                    and all(d in ['H','L','V','K','I','U'] for d in detectors)):
-                raise TypeError(
-                "detectors have to be a list of strings"+
-                " with at least one the followings as elements: \n"+
-                "'H' for LIGO Hanford \n'L' for LIGO Livingston\n"+
-                "'V' for Virgo \n'K' for KAGRA \n'I' for LIGO India"+
-                " (INDIGO) \n\n'U' if you don't want to specify detector")
+            raise ValueError("injection_source DataSet is empty")
 
-        
-        rejectionInterval=SegmentList()
-        for tm in filterTimes:
-            if not isinstance(tm,list):
-                rejectionInterval.append(Segment(tm-0.5,tm+0.5))
-            else:
-                rejectionInterval.append(Segment(tm[0],tm[1]))
-        rejectionInterval.coalesce()
-        filteredPods=[]
-        for i in range(len(self.dataPods)):
-            exlusion = False
-            
-            if detectors==None:
-                for j in range(len(self.dataPods[i].detectors)):
-                    if rejectionInterval.intersects_segment(Segment(
-                        self.dataPods[i].gps[j]-window,
-                        self.dataPods[i].gps[j]+
-                        self.dataPods[i].duration+window)):
-                        exlusion = True
-    
-            else:
-                for d in detectors:
-                    ind = self.dataPods[i].detectors.index(d)
-                    if rejectionInterval.intersects_segment(Segment(
-                        self.dataPods[i].gps[ind]-window,
-                        self.dataPods[i].gps[ind]+
-                        self.dataPods[i].duration+window)):
-                        exlusion = True
-            
-            if exlusion == False:
-                filteredPods.append(self.dataPods[i])
-                
-        self._dataPods=filteredPods
-        print("Given GPS times, no longer in DataSet")
-    
-    def filterDetector(self,detectors):
-        
-        if isinstance(detectors,str): detectors = [detectors]
-        if not (isinstance(detectors,list) 
-                and all(d in ['H','L','V','K','I','U'] for d in detectors)):
-            raise TypeError(
-            "detectors have to be a list of strings"+
+    # DataPod
+    elif isinstance(injection_source,DataPod):
+        inj_type = 'DataPod'
+
+    else:
+        raise TypeError('Not valid input for injection_source: ',injection_source 
+                    ,"\nIt has to be either a folder or a DataPod or DataSet object.")
+
+    return injection_source, inj_type
+
+
+
+
+
+def generator(duration
+               ,fs
+               ,size
+               ,detectors
+               ,injection_source = None
+               ,labels = None
+               ,backgroundType = None
+               ,injectionSNR = None
+               ,noiseSourceFile = None
+               ,windowSize = None #(32)            
+               ,timeSlides = None #(1)
+               ,startingPoint= None #(32)
+               ,name = None
+               ,savePath = None
+               ,single = False  # Making single detector injections as glitch
+               ,injectionCrop = 0  # Allows to crop part of the injection when you move the injection arroud, 0 is no 1 is maximum means 100% cropping allowed. The cropping will be a random displacement from zero to parto of duration
+               ,frames=None 
+               ,channels=None
+               ,disposition=None
+               ,maxDuration=None
+               ,differentSignals=False   # In case we want to put different injection to every detector.
+               ,plugins=None
+               ,**kwargs):
+
+    """This is one of the core methods/function of this module.
+    It generates data instances of detector strain data that could be 
+    from real detectors or simulated noise. It has many options for
+    each different type of instance -that it can generate.
+
+    Parameters
+    ----------
+
+    duration : float/int
+        The duration of instances to be generated in seconds.
+
+    fs : float/ing
+        The sample frequency of the instances to be generated.
+
+    size : int
+        The number of instances to be generated.
+
+    detectors : str/ list of str
+        The detectors to be used for the background. Even for optimal 
+        gaussian noise the background is different for each detector. 
+        For example if you wan to include Hanford, Livingston and Virgo
+        you state it as 'HLV' or ['H','L','V'].
+
+    injection_source: str (path, optional)
+        The path to the directory with the injections. If not specified
+        the generator will just generate noise instances, setting
+        injectionSNR to 0.
+
+    labels: dict (optional)
+        The optional label for all the instances to be generated. 
+        If not specified labels is {'type':'UNDEFINED'}.
+
+    backgroundType: {'optimal','real'}
+        The type of background to be used. If 'optimal' is chosen,
+        a simulated noise background will be used (simulateddetectornoise.py)
+        depending the detector. If 'real' is chosen, a source of real detector
+        noise will need to be specified from noiseSourceFile.
+
+    injectionSNR: float/int
+        The Signal to Noise Ration of the injection used for the instances.
+        All injections are calibrated to be in that SNR value.
+
+    noiseSourceFile: {gps intervals, path, txt file, numpy.ndarray}
+        The source of real noise. There are many options to provide source 
+        of real noise. 
+
+        * A list intervals (one for each detectors) with gps times. The script 
+        will get the available coinsident data within the 'detectors' and use them.
+
+        * A path with txt or DataPod files that have noise data.
+
+        * A numpy.ndarray with the data directly.
+
+        This parameter evolves depending on the needs of users.
+
+    windowSize: int/float
+        The amount of seconds to use around the instance duration, for the 
+        calculation of PSD. The bigger the windowSize the better whittening.
+        Although the calculation takes more time. It defaults to 16 times
+        the duration parameter.
+
+    timeSlides: int (optional)
+        The number of timeshifts to use on the provided noise source.
+        If noise source has N instances of utilisable noise by using
+        timeSlides we will have N*(1-timeSlides) instances. Default
+        is 1 which means not using timeSlides.
+
+    startingPoint: float/int (optional)
+        The starting point in seconds from which we will use the noise
+        source. In case we have a big noise sample by specifing startingPoint
+        we do not start from the beggining but from that second. Default is 0.
+
+    name : str (optional)
+        The name of the dataset, if it is saved. 
+
+    savePath : str (path, optional)
+        The of the file to be saved. If not stated file will not be saved and
+        it will just be returned.
+
+    single : bool
+        If true and injectionSNR or injectionHRSS is defined, it will add
+        a signal to only one of the available detectors, randomly selected.
+        All SNR or hrss will be used on the single injection. Default is False.
+
+    differentSignals : bool
+        If true each detector gets a different randomly selected signal. 
+        Default is False.
+
+    injectionCrop : float [0,1]
+        Allows to crop part of the injection (up to the value provided when 
+        randomly positions the injection arroud on the background. 0 means
+        no croppin allowd and 1 means maximum 100% cropping allowed. The cropping 
+        will be a random displacement from zero to parto of durationn.
+
+    frames: dict or {C00, C01,C02}
+        In case we use real detector noise and the script looks for the available 
+        noise segments we need to specify the frames to look for. We have to provide 
+        a dictionary of the frames for the given detectors. C00, C01 and C02 provides a
+        shortcut for the widly used frames. 
+        {'H': 'H1_HOFT_C0X' ,'L': 'L1_HOFT_C0X' ,'V': 'V1Online'}.
+        C02 is chossen as default given that is pressent in all observing runs.
+
+    channels: dict or {C00, C01,C02} 
+        As with frames, in case we use real detector noise and the script looks for 
+        the available noise segments we need to specify the channels to look for. 
+        We have to provide a dictionary of the channels for the given detectors. 
+        C00, C01 and C02 provides a shortcut for the widly used frames. 
+        {'H': 'H1:DCS-CALIB_STRAIN_C0X','L': 'L1:DCS-CALIB_STRAIN_C0X' ,'V': 'V1:Hrec_hoft_16384Hz'}.
+        C02 is chossen as default given that is pressent in all observing runs.
+
+    disposition: float (optional)
+        Disposition is the time interval in seconds within we want the central times of the 
+        signals to appear. It is used with differentSignals = True. The bigger
+        the interval the bigger the spread. Although the spread is always constrained by
+        the duration of the longest signa selected so that the signals don't get cropped.
+
+    maxDuration : float (optional)
+        If you want to use injections and want to restrict the maximum duration used.
+        This will check the randomly selected injection's duration. If it is bigger
+        that the one specified here, it will select another random injection. This will
+        continue until it finds one with duration smaller than maxDuration parameter.
+        Note that the smaller this parameter is the more time it will take to complete
+        the generation.
+
+    plugins : list of strings
+        You can specify here plugins that are included in plugins.known_plug_ins variable.
+        Those plugins will automaticly be added into the dataset returned.
+
+
+    Returns
+    -------
+
+    A DataSet object. If savePath is defined, it saves the DataSet to that path
+    and it returns None.
+
+
+
+    """
+    # Integration limits for the calculation of analytical SNR
+    # These values are very important for the calculation
+    print(injection_initialization)
+    fl, fm=20, int(fs/2)#
+
+    profile = {'H' :'aligo','L':'aligo','V':'avirgo','K':'KAGRA_Early','I':'aligo'}
+
+    # Labels used in saving file
+    #lab={10:'X', 100:'C', 1000:'M', 10000:'XM',100000:'CM'}  
+
+    lab={}
+    if size not in lab:
+        lab[size]=str(size)
+
+    # ---------------------------------------------------------------------------------------- #   
+    # --- duration --------------------------------------------------------------------------- #
+
+    if not (isinstance(duration,(float,int)) and duration>0 ):
+        raise ValueError('The duration value has to be a possitive float'
+            +' or integer representing seconds.')
+
+    # ---------------------------------------------------------------------------------------- #   
+    # --- fs - sample frequency -------------------------------------------------------------- #
+
+    if not (isinstance(fs,int) and fs>0):
+        raise ValueError('Sample frequency has to be a positive integer.')
+
+    # ---------------------------------------------------------------------------------------- #   
+    # --- detectors -------------------------------------------------------------------------- #
+
+    if isinstance(detectors,(str,list)):
+        for d in detectors:
+            if d not in ['H','L','V','K','I']: 
+                raise ValueError("detectors have to be a list of strings or a string"+
+            " with at least one the followings as elements: \n"+
+            "'H' for LIGO Hanford \n'L' for LIGO Livingston\n"+
+            "'V' for Virgo \n'K' for KAGRA \n'I' for LIGO India (INDIGO) \n"+
+            "\n'U' if you don't want to specify detector")
+        if isinstance(detectors,str): detectors=list(detectors)
+    else:
+        raise ValueError("detectors have to be a list of strings or a string"+
             " with at least one the followings as elements: \n"+
             "'H' for LIGO Hanford \n'L' for LIGO Livingston\n"+
             "'V' for Virgo \n'K' for KAGRA \n'I' for LIGO India (INDIGO) \n"+
             "\n'U' if you don't want to specify detector")
-            
-        for i in range(len(self.dataPods)):
-            for d in detectors:
-                ind = self.dataPods[i].detectors.index(d)                
-                self._dataPods[i]._strain = np.delete(self._dataPods[i]._strain
-                                                      , ind , 0)
-                self._dataPods[i]._detectors = np.delete(
-                    self._dataPods[i]._detectors, ind, 0)
-                self._dataPods[i]._gps = np.delete(self._dataPods[i]._gps
-                                                   , ind, 0)
-        message = "Detector"
-        if len(detectors)==1:
-            message+=" "
-        else:
-            message+="s "
-        for d in detectors:
-            message+=(d+", ")
-        message += "no longer in this DataSet"
-        print(message)
-        
-    def filterLabel(self,labels):
-        
-        if not (isinstance(labels, dict) and len(labels)>0):
-            raise ValueError("labels have to be a dict with at least"
-                             +" one key-value pare")
-        
-        finalPods=[]
-        for i in range(len(self._dataPods)):
-            
-            same = 0
-            for j in range(len(self._dataPods[i].labels)):
-                for k in range(len(labels)):
-                    if ((list(labels.keys(
-                    ))[k]==list(self._dataPods[i].labels.keys())[j])
-                        and (labels[list(labels.keys(
-                        ))[k]]==self._dataPods[i].labels[list(
-                            self._dataPods[i].labels.keys())[j]])):
-                        same+=1
-            if same == len(labels):
-                finalPods.append(self._dataPods[i])
-                
-        self._dataPods = finalPods
-        
 
-    def unloadData(self,extras=None, shape = None):
 
-        goods =[]
-        if extras==None:
-            for pod in self.dataPods:
-                goods.append(pod.strain.tolist())
-            goods=np.asarray(goods)                
-
-        elif isinstance(extras,str):
-            for pod in self.dataPods:
-                goods.append(pod.metadata[extras].tolist())
-            goods=np.asarray(goods)
-        else:
-            raise ValueError('Metadata have no option for '+str(extras))
-            
-        if shape == None:
-            shape = goods.shape
-        if isinstance(shape,tuple):
-            if shape[0]==None: 
-                shapeList=list(shape)
-                shapeList[0]=len(self)
-                shape=tuple(shapeList)
-            if all(dim in goods.shape for dim in shape):
-                shapeList = list(shape)
-                goodsShapeList = list(goods.shape)
-                newIndex = list(shapeList.index(goods.shape[i]) for i in range(len(shape)))
-                goods = np.transpose(goods, newIndex)
-            else:
-                raise ValueError("Shape values are not the same as the DataSet shape")
-        else:
-            raise TypeError("Not valid shape.")
-        print("DataSet with shape "+str(goods.shape)+" is unloaded")
-        return goods
-    
-    def unloadLabels(self,*args,reshape=False):
-        # Checking the types of labels and how many
-        # pods have the specific label.
-        labelOccur={}
-        for pod in self.dataPods:
-            for key in list(pod.labels.keys()):
-                if key not in list(labelOccur.keys()): labelOccur[key]=0
-                labelOccur[key]+=1
-        # 'type' is a default label
-        if len(args)==0: args=('type',)    
-        for arg in args:
-            # labels must be strings
-            if not isinstance(arg,str):
-                raise TypeError("Label keys must be strings")
-            # if a label type doesn't exist an error is raised
-            if not arg in list(labelOccur.keys()):
-                raise KeyError("There is no label key "+str(arg))
-            # The label type must occur as many times as the size of the dataset
-            if labelOccur[arg]!=len(self):
-                raise ValueError(str(len(self)-labelOccur[arg])
-                                 +" pods don't have the label "+str(arg)+" defined")
-                
-        goods=[]
-        for i in range(len(self)):
-            if len(args)>1:
-                label=[]
-                for arg in args:
-                    label.append(self[i].labels[arg])
-            else:
-                label=self[i].labels[arg]
-            goods.append(label)
-        goods=np.asarray(goods)
-        # reshaping in case only one label is required
-        if (len(args)==1 and reshape==True): goods=goods.reshape((len(goods),1))
-        print("Labels "+str(list(args))+" with shape "+str(goods.shape)+" are unloaded")
-        return goods
-   
-        
-        
-    def generator(duration
-                   ,fs
-                   ,size
-                   ,detectors
-                   ,injectionFolder = None
-                   ,labels = None
-                   ,backgroundType = None
-                   ,injectionSNR = None
-                   ,noiseSourceFile = None  
-                   ,windowSize = None #(32)            
-                   ,timeSlides = None #(1)
-                   ,startingPoint= None #(32)
-                   ,name = None
-                   ,savePath = None
-                   ,single = False  # Making single detector injections as glitch
-                   ,injectionCrop = 0  # Allows to crop part of the injection when you move the injection arroud, 0 is no 1 is maximum means 100% cropping allowed. The cropping will be a random displacement from zero to parto of duration
-                
-                   ,disposition=None
-                   ,maxDuration=None
-                   ,differentSignals=False   # In case we want to put different injection to every detector.
-                   ,extras=None):
-
-        # Integration limits for the calculation of analytical SNR
-        # These values are very important for the calculation
-
-        fl, fm=20, int(fs/2)#
-
-        profile = {'H' :'aligo','L':'aligo','V':'avirgo','K':'KAGRA_Early','I':'aligo'}
-
-        # Labels used in saving file
-        #lab={10:'X', 100:'C', 1000:'M', 10000:'XM',100000:'CM'}  
-
-        lab={}
-        if size not in lab:
-            lab[size]=str(size)
-
-        # ---------------------------------------------------------------------------------------- #   
-        # --- duration --------------------------------------------------------------------------- #
-
-        if not (isinstance(duration,(float,int)) and duration>0 ):
-            raise ValueError('The duration value has to be a possitive float'
-                +' or integer representing seconds.')
-
-        # ---------------------------------------------------------------------------------------- #   
-        # --- fs - sample frequency -------------------------------------------------------------- #
-
-        if not (isinstance(fs,int) and fs>0):
-            raise ValueError('Sample frequency has to be a positive integer.')
-
-        # ---------------------------------------------------------------------------------------- #   
-        # --- detectors -------------------------------------------------------------------------- #
-
-        if isinstance(detectors,(str,list)):
-            for d in detectors:
-                if d not in ['H','L','V','K','I']: 
-                    raise ValueError("detectors have to be a list of strings or a string"+
-                " with at least one the followings as elements: \n"+
-                "'H' for LIGO Hanford \n'L' for LIGO Livingston\n"+
-                "'V' for Virgo \n'K' for KAGRA \n'I' for LIGO India (INDIGO) \n"+
-                "\n'U' if you don't want to specify detector")
-            if isinstance(detectors,str): detectors=list(detectors)
-        else:
-            raise ValueError("detectors have to be a list of strings or a string"+
-                " with at least one the followings as elements: \n"+
-                "'H' for LIGO Hanford \n'L' for LIGO Livingston\n"+
-                "'V' for Virgo \n'K' for KAGRA \n'I' for LIGO India (INDIGO) \n"+
-                "\n'U' if you don't want to specify detector")
-        
+    # ---------------------------------------------------------------------------------------- #   
+    # --- size ------------------------------------------------------------------------------- #        
 
-        # ---------------------------------------------------------------------------------------- #   
-        # --- size ------------------------------------------------------------------------------- #        
+    if not (isinstance(size, int) and size > 0):
+        raise ValueError("size must be a possitive integer.")
 
-        if not (isinstance(size, int) and size > 0):
-            raise ValuError("size must be a possitive integer.")
+    # ---------------------------------------------------------------------------------------- #   
+    # --- injection_source -------------------------------------------------------------------- #
 
-        # ---------------------------------------------------------------------------------------- #   
-        # --- injectionFolder -------------------------------------------------------------------- #
+    injection_source, inj_type = injection_initialization(injection_source, detectors)
 
-        if injectionFolder == None:
-            pass
-        elif isinstance(injectionFolder, str):            
-            if (('/' in injectionFolder) and os.path.isdir(injectionFolder)):
-                injectionFolder_set = injectionFolder.split('/')[-1]
-            elif (('/' not in injectionFolder) and any('injections' in p for p in sys.path)):
-                    for p in sys.path:
-                        if ('injections' in p):
-                            injectionFolder_path = (p.split('injections')[0]+'injections'
-                                +'/'+injectionFolder)
-                            if os.path.isdir(injectionFolder_path):
-                                injectionFolder = injectionFolder_path
-                                injectionFolder_set = injectionFolder.split('/')[-1]
-                            else:
-                                raise FileNotFoundError('No such file or directory:'
-                                                        +injectionFolder_path)
+    # ---------------------------------------------------------------------------------------- #   
+    # --- labels ----------------------------------------------------------------------------- #
 
-            else:
-                raise FileNotFoundError('No such file or directory:'+injectionFolder) 
-        else:
-            raise TypeError("cbcFolder has to be a string indicating a folder "
-                            +"in MLyWorkbench or a full path to a folder")
+    if labels == None:
+        labels = {'type' : 'UNDEFINED'}
+    elif not isinstance(labels,dict):
+        raise TypeError(" Labels must be a dictionary.Suggested keys for labels"
+                        +"are the following: \n{ 'type' : ('noise' , 'cbc' , 'signal'"
+                        +" , 'burst' , 'glitch', ...),\n'snr'  : ( any int or float number "
+                        +"bigger than zero),\n'delta': ( Declination for sky localisation,"
+                        +" float [-pi/2,pi/2])\n'ra'   : ( Right ascention for sky "
+                        +"localisation float [0,2pi) )})")
 
-        # ---------------------------------------------------------------------------------------- #   
-        # --- labels ----------------------------------------------------------------------------- #
+    # ---------------------------------------------------------------------------------------- #   
+    # --- backgroundType --------------------------------------------------------------------- #
 
-        if labels == None:
-            labels = {'type' : 'UNDEFINED'}
-        elif not isinstance(labels,dict):
-            raise TypeError(" Labels must be a dictionary.Suggested keys for labels"
-                            +"are the following: \n{ 'type' : ('noise' , 'cbc' , 'signal'"
-                            +" , 'burst' , 'glitch', ...),\n'snr'  : ( any int or float number "
-                            +"bigger than zero),\n'delta': ( Declination for sky localisation,"
-                            +" float [-pi/2,pi/2])\n'ra'   : ( Right ascention for sky "
-                            +"localisation float [0,2pi) )})")
-
-        # ---------------------------------------------------------------------------------------- #   
-        # --- backgroundType --------------------------------------------------------------------- #
-
-        if backgroundType == None:
-            backgroundType = 'optimal'
-        elif not (isinstance(backgroundType,str) 
-              and (backgroundType in ['optimal','sudo_real','real'])):
-            raise ValueError("backgroundType is a string that can take values : "
-                            +"'optimal' | 'sudo_real' | 'real'.")
-
-        # ---------------------------------------------------------------------------------------- #   
-        # --- injectionSNR ----------------------------------------------------------------------- #
-        if injectionFolder == None :
-            injectionSNR = 0
-        elif (injectionFolder != None and injectionSNR == None ):
-            raise ValueError("If you want to use an injection for generation of"+
-                             "data, you have to specify the SNR you want.")
-        elif injectionFolder != None and (not (isinstance(injectionSNR,(int,float)) 
-                                          and injectionSNR >= 0)):
-            raise ValueError("injectionSNR has to be a positive number")
-
-
-        # ---------------------------------------------------------------------------------------- #   
-        # --- noiseSourceFile -------------------------------------------------------------------- #
-
-        if (backgroundType == 'sudo_real' or backgroundType =='real'):
-
-            if noiseSourceFile == None:
-                raise TypeError('If you use sudo_real or real noise you need'
-                    +' a real noise file as a source.')
-
-            if (noiseSourceFile!=None and isinstance(noiseSourceFile,list) 
-                    and len(noiseSourceFile)==2 
-                    and all(isinstance(el,str) for el in noiseSourceFile)):
-
-                if '.txt' in noiseSourceFile[1]:
-                    noiseSourceFile[1] = noiseSourceFile[1][:-4]
-
-                path_main=''
-                path_check = False
-
-                if (('/' in noiseSourceFile[0]) and all(os.path.isfile( noiseSourceFile[0]
-                                +'/'+det+'/'+noiseSourceFile[1]+'.txt') for det in detectors)):
-                    path_main = ''
-                    path_check = True
-
-
-                elif (('/' not in noiseSourceFile[0]) and any('ligo_data' in p for p in sys.path)):
-                    for p in sys.path:
-                        if ('ligo_data' in p):
-                            path_main = (p.split('ligo_data')[0]+'ligo_data/'+str(int(fs))+'/')
-                            if all(os.path.isfile(path_main+noiseSourceFile[0]+'/'+det+'/'
-                                    +noiseSourceFile[1]+'.txt') for det in detectors):    
-                                path_check = True
-                                break
-                            else:
-                                raise FileNotFoundError("No such file or directory: "+path_main
-                                                        +"/<detector>/"+noiseSourceFile[1]+".txt")
-                if path_check == False:
-                    raise FileNotFoundError(
-                        "No such file or directory: "+noiseSourceFile[0]
-                        +"/<detector>/"+noiseSourceFile[1]+".txt")
-            else:
-                raise TypeError("Noise source file has to be a list of two strings:\n"
-                                +"--> The first is the path to the date folder that include\n "
-                                +"    the data of all the detectors or just the datefile given\n"
-                                +"    that the path is in sys.path.\n\n"
-                                +"--> The second is the file name of the segment to be used.")
-        # ---------------------------------------------------------------------------------------- #   
-        # --- windowSize --(for PSD)-------------------------------------------------------------- #        
-
-        if windowSize == None: windowSize = duration*8
-        if not isinstance(windowSize,int):
-            raise ValueError('windowSize needs to be an integral')
-        if windowSize < duration :
-            raise ValueError('windowSize needs to be bigger than the duration')
-
-        # ---------------------------------------------------------------------------------------- #   
-        # --- timeSlides ------------------------------------------------------------------------- #
-
-        if timeSlides == None: timeSlides = 1
-        if not (isinstance(timeSlides, int) and timeSlides >=1) :
-            raise ValueError('timeSlides has to be an integer equal or bigger than 1')
-
-        # ---------------------------------------------------------------------------------------- #   
-        # --- startingPoint ---------------------------------------------------------------------- #
-
-        if startingPoint == None : startingPoint = windowSize 
-        if not (isinstance(startingPoint, int) and startingPoint >=0) :
-            raise ValueError('lags has to be an integer')        
-
-        # ---------------------------------------------------------------------------------------- #   
-        # --- name ------------------------------------------------------------------------------- #
-
-        if name == None : name = ''
-        if not isinstance(name,str): 
-            raise ValueError('name optional value has to be a string')
+    if backgroundType == None:
+        backgroundType = 'optimal'
+    elif not (isinstance(backgroundType,str) 
+          and (backgroundType in ['optimal','sudo_real','real'])):
+        raise ValueError("backgroundType is a string that can take values : "
+                        +"'optimal' | 'sudo_real' | 'real'.")
 
-        # ---------------------------------------------------------------------------------------- #   
-        # --- savePath --------------------------------------------------------------------------- #
+    # ---------------------------------------------------------------------------------------- #   
+    # --- injectionSNR ----------------------------------------------------------------------- #
+    if injection_source == None :
+        injectionSNR = 0
+#         elif (injection_source != None and injectionSNR == None ):
+#             raise ValueError("If you want to use an injection for generation of"+
+#                              "data, you have to specify the SNR you want.")
+#         elif injection_source != None and (not (isinstance(injectionSNR,(int,float)) 
+#                                           and injectionSNR >= 0)):
+#             raise ValueError("injectionSNR has to be a positive number")
+
+
+    # ---------------------------------------------------------------------------------------- #   
+    # --- noiseSourceFile -------------------------------------------------------------------- #
+
+    if (backgroundType == 'sudo_real' or backgroundType =='real'):
+        # if noiseSourceFile == None:
+        #     raise TypeError('If you use sudo_real or real noise you need'
+        #         +' a real noise file as a source.')
+
+        # Loading noise using gwdatafind and gwpy
+        if (isinstance(noiseSourceFile,list) 
+                and len(noiseSourceFile)==len(detectors) 
+                and all(len(el)==2 for el in noiseSourceFile)):
+
+            noiseFormat='gwdatafind'
+
+        # Loading noise using file paths of txt files (different for each detector)
+        elif (isinstance(noiseSourceFile,list) 
+              and len(noiseSourceFile)==len(detectors) 
+              and all(isisntance(path_,str) for path_ in noiseSourceFile)
+              and all(path_[-4:]=='.txt' for path_ in noiseSourceFile)):
+
+            noiseFormat='txtD'
+
+        # Loading noise using file paths of txt files (one with all detectors)
+        elif (isinstance(noiseSourceFile,str) 
+              and noiseSourceFile[-4:]=='.txt'):
+
+            noiseFormat='txt1'
+
+        # Loading noise using file paths of txt files (one with all detectors)
+        elif (isinstance(noiseSourceFile,np.ndarray) and len(detectors) in noiseSourceFile.shape):
+
+            noiseFormat='array'
+
+        # Loding noise using DataPods or DataSets (one with all detectors)
+        elif ((isinstance(noiseSourceFile,str) 
+              and noiseSourceFile[-4:]=='.pkl') 
+              or (('Pod' in str(type(noiseSourceFile))) or ('Set' in str(type(noiseSourceFile))))):
+
+            noiseFormat='PodorSet'
 
-        if savePath == None : 
-            pass
-        elif (savePath,str): 
-            if not os.path.isdir(savePath) : 
-                raise FileNotFoundError('No such file or directory:' +savePath)
-        else:
-            raise TypeError("Destination Path has to be a string valid path")
-            
-        # ---------------------------------------------------------------------------------------- #   
-        # --- extras ----------------------------------------------------------------------------- #
-        
-        theExtras=['snr','psd','correlation']
-        if extras == None:
-            extras = []
-        elif isinstance(extras,str):
-            extras = [extras]
-        elif isinstance(extras,list) and all(ex in theExtras for ex in extras):
-            pass
         else:
-            raise ValueError('extras must be a list of valid strings included in '+str(theExtras))
+            raise TypeError("The noise type format given is not one valid")
 
-        # max Duration
-        
-        if maxDuration == None:
-            if duration == None:
+
+
+    # ---------------------------------------------------------------------------------------- #   
+    # --- windowSize --(for PSD)-------------------------------------------------------------- #        
+
+    if windowSize == None: windowSize = duration*16
+    if not isinstance(windowSize,int):
+        raise ValueError('windowSize needs to be a number')
+    if windowSize < duration :
+        raise ValueError('windowSize needs to be bigger than the duration')
+
+    # ---------------------------------------------------------------------------------------- #   
+    # --- timeSlides ------------------------------------------------------------------------- #
+
+    # if timeSlides == None: timeSlides = 0
+    # if not (isinstance(timeSlides, int) and timeSlides >=0) :
+    #     raise ValueError('timeSlides has to be an integer equal or bigger than 0')
+
+    # ---------------------------------------------------------------------------------------- #   
+    # --- startingPoint ---------------------------------------------------------------------- #
+
+    if startingPoint == None : startingPoint = 0 
+    if not (isinstance(startingPoint, (float,int)) and (startingPoint%duration)%(1/fs) ==0) :
+        raise ValueError('Starting point decimal part must always be a multiple of time step')        
+
+    # ---------------------------------------------------------------------------------------- #   
+    # --- name ------------------------------------------------------------------------------- #
+
+    if name == None : name = ''
+    if not isinstance(name,str): 
+        raise ValueError('name optional value has to be a string')
+
+    # ---------------------------------------------------------------------------------------- #   
+    # --- savePath --------------------------------------------------------------------------- #
+
+    if savePath == None : 
+        pass
+    elif (savePath,str): 
+        if not os.path.isdir(savePath) : 
+            raise FileNotFoundError('No such file or directory:' +savePath)
+    else:
+        raise TypeError("Destination Path has to be a string valid path")
+
+    # ---------------------------------------------------------------------------------------- #   
+    # --- plugins ---------------------------------------------------------------------------- #
+
+    if plugins == None:
+        plugins = []
+    elif not isinstance(plugins,list):
+        plugins = [plugins]
+    if isinstance(plugins,list):
+        for pl in plugins:
+            if pl in known_plug_ins:
+                pass
+            elif isinstance(pl,str) and ('knownPlugIns' in pl):
                 pass
             else:
-                maxDuration=duration
-                
-        # Making a list of the injection names,
-        # so that we can sample randomly from them
+                raise TypeError("plugins must be a list of PlugIn object or from "+str(known_plug_ins))
+
+    # --- fames ---
+
+    if frames==None or (isinstance(frames,str) and frames.upper()=='C02'):
+        frames = {'H': 'H1_HOFT_C02'
+                 ,'L': 'L1_HOFT_C02'
+                 ,'V': 'V1Online'}
+    elif (isinstance(frames,str) and frames.upper()=='C01'):
+        frames = {'H': 'H1_HOFT_C01'
+                 ,'L': 'L1_HOFT_C01'
+                 ,'V': 'V1Online'}
+    elif (isinstance(frames,str) and frames.upper()=='C00'):
+        frames = {'H': 'H1_HOFT_C00'
+                 ,'L': 'L1_HOFT_C00'
+                 ,'V': 'V1Online'}
+    elif not (isinstance(frames,dict)): 
+
+          raise ValueError("Frame type "+str(frames)+" is not valid")
+
+    if channels==None or (isinstance(channels,str) and channels.upper()=='C02'):
+        channels = {'H': 'H1:DCS-CALIB_STRAIN_C02'
+                   ,'L': 'L1:DCS-CALIB_STRAIN_C02'
+                   ,'V': 'V1:Hrec_hoft_16384Hz'}
+    elif (isinstance(channels,str) and channels.upper()=='C01'):
+        channels = {'H': 'H1:DCS-CALIB_STRAIN_C01'
+                   ,'L': 'L1:DCS-CALIB_STRAIN_C01'
+                   ,'V': 'V1:Hrec_hoft_16384Hz'}
+    elif (isinstance(channels,str) and channels.upper()=='C00'):
+        channels = {'H': 'H1:GDS-CALIB_STRAIN'
+                   ,'L': 'L1:GDS-CALIB_STRAIN'
+                   ,'V': 'V1:Hrec_hoft_16384Hz'}
+    elif not (isinstance(channels,dict)): 
+
+          raise ValueError("Channel type "+str(channels)+" is not valid")
+
+    #print(frames,channels)
+
+
+    # --- disposition
+
+
+    # If you want no shiftings disposition will be zero
+    if disposition == None: disposition=0
+    # If you want shiftings disposition has to adjust the maximum length of an injection
+    if isinstance(disposition,(int,float)) and 0<=disposition<duration:
+        disposition_=disposition
+        maxDuration_ = duration-disposition_
+    # If you want random shiftings you can define a tuple or list of those random2*[[eventgps-windowSize/2,eventgps+windowSize/2]] shiftings.
+    # This will adjust also
+    elif (isinstance(disposition,(list,tuple))):
+        if not(len(disposition)==2 
+            and isinstance(disposition[0],(int,float))
+            and isinstance(disposition[1],(int,float)) 
+            and 0<=disposition[0]<duration 
+            and disposition[0]<disposition[1]<duration):
+
+            raise ValueError('If you want random range of dispositons '
+                            +'it needs to be a tuple or list of two numbers that represent a range')
+        else: disposition_=disposition[1]
+    else:
+        raise TypeError('Disposition can be a number or a range'
+                        +' of two nubers (start,end) that always is less than duration')
+
+    # --- max Duration
+
+    if maxDuration == None: 
+        maxDuration=duration
+    if not (isinstance(maxDuration,(int,float)) and 0<maxDuration<=duration):
+        raise ValueError('maxDuration must be between 0 and duration')
+    else:
+        maxDuration_=min(duration-disposition_,maxDuration)
+
+    # Making a list of the injection names,
+    # so that we can sample randomly from them
+
+    injectionFileDict={}
+    noise_segDict={}
+    for det in detectors:
+
+        if injection_source == None:
+            injectionFileDict[det] = None
+        elif inj_type == 'oldtxt':
+            injectionFileDict[det] = dirlist(injection_source+'/' + det)
+
+        elif inj_type == 'directory':
+            injectionFileDict[det] = dirlist(injection_source)
+
+        elif inj_type == 'DataPod':
+            injectionFileDict[det] = [injection_source]
+
+        elif inj_type == 'DataSet':
+            injectionFileDict[det] = [injection_source.dataPods]
 
-        injectionFileDict={}
-        noise_segDict={}
+        else:
+            raise TypeError("Unknown type of injections")
+
+
+
+    # --- PSDm PSDc
+    if 'PSDm' in kwargs: 
+        PSDm=kwargs['PSDm']
+    else:
+        PSDm=None
+
+    if 'PSDc' in kwargs: 
+        PSDc=kwargs['PSDc']
+    else:
+        PSDc=None
+
+    if PSDm==None: 
+        PSDm={}
         for det in detectors:
+            PSDm[det]=1
+    if PSDc==None: 
+        PSDc={}
+        for det in detectors:
+            PSDc[det]=0
+    # ------------------------------
+    # --- injectionHRSS ------------
+
+    if 'injectionHRSS' in kwargs:
+        injectionHRSS = kwargs['injectionHRSS']
+    else: 
+        injectionHRSS=None
+
+    if injection_source == None :
+        injectionHRSS = None
+    # ------------------------------
+    if 'ignoreDetector' in kwargs: 
+        ignoreDetector=kwargs['ignoreDetector']
+    else:
+        ignoreDetector=None
 
-            if injectionFolder == None:
-                injectionFileDict[det] = None
-            else:
-                injectionFileDict[det] = dirlist(injectionFolder+'/' + det)
 
-        if backgroundType == 'optimal':
-            magic={1024: 2**(-21./16.), 2048: 2**(-23./16.), 4096: 2**(-25./16.), 8192: 2**(-27./16.)}
-            param = magic[fs]
+    if backgroundType in ['sudo_real','real']:
+        gps0 = {}
+        if noiseFormat=='txtD':
 
-        elif backgroundType in ['sudo_real','real']:
-            param = 1
             for det in detectors:
-                noise_segDict[det] = np.loadtxt(path_main+noiseSourceFile[0]
-                                                       +'/'+det+'/'+noiseSourceFile[1]+'.txt')    
-            ind=index_combinations(detectors = detectors
+                noise_segDict[det] = np.loadtxt(noiseSourceFile[detectors.index(det)])
+
+                gps0[det]=float(noiseSourceFile[detectors.index(det)].split('_')[1])
+
+            ind=internalLags(detectors = detectors
                                ,lags = timeSlides
-                               ,length = duration
+                               ,duration = duration
                                ,fs = fs
-                               ,size = size
+                               ,size = int(len(noise_segDict[detectors[0]])/fs
+                                           -startingPoint-(windowSize-duration))
                                ,start_from_sec=startingPoint)
 
-            gps0 = int(noiseSourceFile[1].split('_')[1])
+        elif noiseFormat=='txt1':
 
+            file_=np.loadtxt(noiseSourceFile)
 
-        thetime = time.time()
-        DATA=DataSet(name = name)
-        
-        for I in range(size):
+            if len(detectors) not in file_.shape: 
+                raise ValueError(".txt file provided for noise doesn't have equal "
+                                 +"to detector number entries of noise")
 
-            detKeys = list(injectionFileDict.keys())
+            for det in detectors:
+                noise_segDict[det] = file_[detectors.index(det)]
 
-            if injectionFolder != None:
-                inj_ind = np.random.randint(0,len(injectionFileDict[detKeys[0]]))
+                gps0[det]=float(noiseSourceFile.split('_')[1])
 
-            SNR0_dict={}
-            back_dict={}
-            inj_fft_0_dict={}
-            asd_dict={}
-            PSD_dict={}
-            gps_list = []
-            
-            if single == True: luckyDet = np.random.choice(detKeys)
-            for det in detKeys:
-                
-                # In case we want to put different injection to every detectors.
-                if differentSignals==True:
-                    inj_ind = np.random.randint(0,len(injectionFileDict[detKeys[0]]))
-
-                if backgroundType == 'optimal':
-
-                    # Creation of the artificial noise.
-                    PSD,X,T=simulateddetectornoise(profile[det],windowSize,fs,10,fs/2)
-                    PSD_dict[det]=PSD
-                    back_dict[det] = X
-                    # Making the noise a TimeSeries
-                    back=TimeSeries(X,sample_rate=fs) 
-                    # Calculating the ASD so tha we can use it for whitening later
-                    asd=back.asd(1,0.5)
-                    asd_dict[det] = asd
-                    gps_list.append(0.0)
-
-
-                elif backgroundType == 'sudo_real':
-
-                    noise_seg=noise_segDict[det]
-                    # Calling the real noise segments
-                    noise=noise_seg[ind[det][I]:ind[det][I]+windowSize*fs]  
-                    # Generating the PSD of it
-                    p, f = psd(noise, Fs=fs, NFFT=fs) 
-                    p, f=p[1::],f[1::]
-                    # Feeding the PSD to generate the sudo-real noise.            
-                    PSD,X,T=simulateddetectornoise([f,p],windowSize,fs,10,fs/2)
-                    PSD_dict[det]=PSD
-                    # Making the noise a TimeSeries
-                    back=TimeSeries(X,sample_rate=fs)
-                    # Calculating the ASD so tha we can use it for whitening later
-                    asd=back.asd(1,0.5)                 
-                    asd_dict[det] = asd
-                    gps_list.append(gps0+ind[det][I]/fs)
-                    back_dict[det] = back.value
-                elif backgroundType == 'real':
-
-                    noise_seg=noise_segDict[det]
-                    # Calling the real noise segments
-                    noise=noise_seg[ind[det][I]:ind[det][I]+windowSize*fs] 
-                    # Calculatint the psd of FFT=1s
-                    p, f = psd(noise, Fs=fs,NFFT=fs)
-                    # Interpolate so that has t*fs values
-                    psd_int=interp1d(f,p)                                     
-                    PSD=psd_int(np.arange(0,fs/2,1/windowSize))
-                    PSD_dict[det]=PSD
-                    # Making the noise a TimeSeries
-                    back=TimeSeries(noise,sample_rate=fs)
-                    back_dict[det] = back
-                    # Calculating the ASD so tha we can use it for whitening later
-                    asd=back.asd(1,0.5)
-                    asd_dict[det] = asd
-                    gps_list.append(gps0+ind[det][I]/fs)
-
-                #If this dataset includes injections:            
-                if injectionFolder != None:
-                    # Calling the templates generated with PyCBC
-                    # OLD inj=load_inj(injectionFolder,injectionFileDict[det][inj_ind], det) 
-                    inj = np.loadtxt(injectionFolder+'/'+det+'/'+injectionFileDict[det][inj_ind])
-                    # Saving the length of the injection
-                    inj_len = len(inj)/fs
-                    # I put a random offset for all injection so that
-                    # the signal is not always in the same place
-                    if inj_len > duration: 
-                        inj = inj[int(inj_len-duration)*fs:]
-                        print('Injection was cropped to fit duration. First'
-                              +str(inj_len-duration)+' seconds have been removed.')
-                        inj_len = len(inj)/fs
-                    if inj_len <= duration: inj = np.hstack((np.zeros(int(fs*(duration-inj_len)/2))
-                                                        , inj
-                                                        , np.zeros(int(fs*(duration-inj_len)/2))))
-                    # DISPOSITIONS
-                    
-                    # Default case when coherent
-                    if disposition == None:
-                        if det == detKeys[0]:
-                            disp = np.random.random_integers(low = min(-int(fs*(duration-0.1-inj_len)/2),0) 
-                                                         ,high = max(int(fs*((duration-0.1-inj_len)/2 
-                                                                         + injectionCrop*(duration-0.1))),1))
-                            
-                    # Case when signals will be randomly positioned for each detector seperatly. 
-                    # Does not affect if signals will be different or not.
-                    elif disposition == 'random':
-                        disp = np.random.random_integers(low = min(-int(fs*(duration-0.1-inj_len)/2),0) 
-                                                         ,high = max(int(fs*((duration-0.1-inj_len)/2 
-                                                                         + injectionCrop*(duration-0.1))),1))
-                    # Case when signals will be positioned within a duration stated by the disposition.
-                    # The center of this duration will be moved randomly given the maxDuration
-                    # of the injections.
-                    elif isinstance(disposition,(int,float)):
-                        if det == detKeys[0]:
-                            center_position = np.random.random_integers(
-                                low = min(-int(fs*(duration-0.1-maxDuration-disposition)/2),0)
-                               ,high = max(int(fs*(duration-0.1-maxDuration-disposition)/2)+1,1))
-                                # the +1 is because there is an error if the high becomes 0
-                                
-                            positions=np.arange(-disposition/2,disposition/2+0.0001
-                                                ,disposition/(len(detKeys)-1))
-                            np.random.shuffle(positions)
-                        disp = center_position+int(positions[detKeys.index(det)]*fs)
-                    
-                    
-                    if disp >= 0: 
-                        inj = np.hstack((np.zeros(int(fs*(windowSize-duration)/2)),inj[disp:]
-                                             ,np.zeros(int(fs*(windowSize-duration)/2)+disp)))   
-                    if disp < 0: 
-                        inj = np.hstack((np.zeros(int(fs*(windowSize-duration)/2)-disp),inj[:disp]
-                                             ,np.zeros(int(fs*(windowSize-duration)/2)))) 
+            ind=internalLags(detectors = detectors
+                               ,lags = timeSlides
+                               ,duration = duration
+                               ,fs = fs
+                               ,size = int(len(noise_segDict[detectors[0]])/fs
+                                           -startingPoint-(windowSize-duration))
+                               ,start_from_sec=startingPoint)
 
+        elif noiseFormat=='array':
 
-                    
-                    # Calculating the one sided fft of the template,                
-                    inj_fft_0=np.fft.fft(inj)
-                    inj_fft_0_dict[det] = inj_fft_0
-                    # we get rid of the DC value and everything above fs/2.
-                    inj_fft_0N=np.abs(inj_fft_0[1:int(windowSize*fs/2)+1]) 
-                    
-                    SNR0_dict[det]=np.sqrt(param*2*(1/windowSize)*np.sum(np.abs(inj_fft_0N
-                                *inj_fft_0N.conjugate())[windowSize*fl-1:windowSize*fm-1]
-                                /PSD_dict[det][windowSize*fl-1:windowSize*fm-1]))
-                                        
-                    if single == True:
-                        if det != luckyDet:
-                            SNR0_dict[det] = 0.01 # Making single detector injections as glitch
-                            inj_fft_0_dict[det] = np.zeros(windowSize*fs)
+            file_=noiseSourceFile
 
+            if len(detectors) not in file_.shape: 
+                raise ValueError(".txt file provided for noise doesn't have equal "
+                                 +"to detector number entries of noise")
 
-                else:
-                    SNR0_dict[det] = 0.01 # avoiding future division with zero
-                    inj_fft_0_dict[det] = np.zeros(windowSize*fs)
+            for det in detectors:
+                noise_segDict[det] = file_[detectors.index(det)]
+
+                gps0[det]=0
 
+            ind=internalLags(detectors = detectors
+                               ,lags = timeSlides
+                               ,duration = duration
+                               ,fs = fs
+                               ,size = int(len(noise_segDict[detectors[0]])/fs
+                                           -startingPoint-(windowSize-duration))
+                               ,start_from_sec=startingPoint)
 
-            # Calculation of combined SNR    
-            SNR0=np.sqrt(np.sum(np.asarray(list(SNR0_dict.values()))**2))
+        elif noiseFormat=='PodorSet':
 
-            # Tuning injection amplitude to the SNR wanted
-            podstrain = []
-            podPSD = []
-            podCorrelations=[]
-            SNR_new=[]
-            
-            for det in detectors:
-                fft_cal=(injectionSNR/SNR0)*inj_fft_0_dict[det]         
-                inj_cal=np.real(np.fft.ifft(fft_cal*fs))
-                                    
-                strain=TimeSeries(back_dict[det]+inj_cal,sample_rate=fs,t0=0)
-                #Whitening final data
-                podstrain.append(((strain.whiten(1,0.5,asd=asd_dict[det])[int(((windowSize
-                        -duration)/2)*fs):int(((windowSize+duration)/2)*fs)]).value).tolist())
-                
-                if 'snr' in extras:
-                    # Calculating the new SNR which will be slightly different that the desired one.    
-                    inj_fft_N=np.abs(fft_cal[1:int(windowSize*fs/2)+1]) 
+            if isinstance(noiseSourceFile,str):
+                with open(noiseSourceFile,'rb') as obj:
+                    file_ = pickle.load(obj)
+            else:
+                file_=noiseSourceFile
 
+            if 'Pod' in str(type(file_)):
+                noiseFormat = 'DataPod'
+                for det in detectors:
+                    noise_segDict[det] = file_.strain[detectors.index(det)]
 
-                    SNR_new.append(np.sqrt(param*2*(1/windowSize)*np.sum(np.abs(inj_fft_N
-                                *inj_fft_N.conjugate())[windowSize*fl-1:windowSize*fm-1]
-                                /PSD_dict[det][windowSize*fl-1:windowSize*fm-1])))
+                    gps0[det]=float(file_.gps[detectors.index(det)])
 
 
-                if 'psd' in extras:
-                    podPSD.append(asd_dict[det]**2)
-            
-            if 'correlation' in extras:
+                ind=internalLags(detectors = detectors
+                                   ,lags = timeSlides
+                                   ,duration = duration
+                                   ,fs = fs
+                                   ,size = int(len(noise_segDict[detectors[0]])/fs
+                                               -startingPoint-(windowSize-duration))
+                                   ,start_from_sec=startingPoint)
 
-                for i in np.arange(len(detectors)):
-                    for j in np.arange(i+1,len(detectors)):
-                        window= int((6371/300000)*fs)+1
-                        podCorrelations.append(correlate(podstrain[i],podstrain[j],window))
-                        
-            
-            podMetadata={}
-            
-            if 'snr' in extras:
-                podMetadata['snr']=np.array(SNR_new)
-            if 'psd' in extras:
-                podMetadata['psd'] = np.array(podPSD)
-            if 'correlation' in extras:
-                if len(np.array(podCorrelations).shape)==1: podCorrelations=[podCorrelations]
-                podMetadata['correlation'] = np.array(podCorrelations)
-            
+                if size > int(len(noise_segDict[detectors[0]])/fs
+                                               -startingPoint-(windowSize-duration)):
+                    print("Requested size is bigger that the noise sourse data"
+                                     +" can provide. Background will be used multiple times")
 
-                
+                    indexRepetition = ceil(size/int(len(noise_segDict[detectors[0]])/fs
+                                               -startingPoint-(windowSize-duration)))
 
+                    for det in detectors:
+                        ind[det] = indexRepetition*ind[det]
 
-            DATA.add(DataPod(strain = podstrain
-                               ,fs = fs
-                               ,gps = gps_list
-                               ,labels =  labels
-                               ,detectors = detKeys
+            elif 'Set' in str(type(file_)):
+                noiseFormat = 'DataSet'
+                for podi in range(len(file_)):
+
+                    if podi==0:
+                        for det in detectors:
+                            noise_segDict[det] = [file_[podi].strain[detectors.index(det)]]
+
+                            gps0[det]=float(file_[podi].gps[detectors.index(det)])
+                            if len(file_[podi].strain[detectors.index(det)])!=windowSize*fs:
+                                raise ValueError("Noise source data are not in the shape expected.")
+
+                    else:
+                        for det in detectors:
+                            noise_segDict[det].append(file_[podi].strain[detectors.index(det)])
+
+
+
+                ind=internalLags(detectors = detectors
+                                   ,lags = timeSlides
+                                   ,duration = duration
+                                   ,fs = 1
+                                   ,size = len(file_)
+                                   ,start_from_sec=startingPoint)
+                for det in detectors:
+                    print("det",gps0[det]+np.array(ind[det])+(windowSize-duration)/2)
+
+                if size > len(file_):
+                    print("Requested size is bigger that the noise sourse data"
+                                     +" can provide. Background will be used multiple times")
+
+                    indexRepetition = ceil(size/len(file_))
+
+                    for det in detectors:
+                        ind[det] = indexRepetition*ind[det]
+                        noise_segDict[det] = indexRepetition*noise_segDict[det]
+
+
+
+
+        elif noiseFormat=='gwdatafind':
+            for d in range(len(detectors)):
+
+                for trial in range(1):
+                    try:
+                        t0=time.time()
+                        conn=gwdatafind.connect()
+                        urls=conn.find_urls(detectors[d]
+                                           , frames[detectors[d]]
+                                           , noiseSourceFile[d][0]
+                                           , noiseSourceFile[d][1])
+
+                        noise_segDict[detectors[d]]=TimeSeries.read(urls
+                                                                    , channels[detectors[d]]
+                                                                    , start =noiseSourceFile[d][0]
+                                                                    , end =noiseSourceFile[d][1]
+                                                                   ).resample(fs).astype('float64').value#[fs:-fs].value
+                        # Added [fs:fs] because there was and edge effect
+
+                        print("\n time to get "+detectors[d]+" data : "+str(time.time()-t0))
+
+                        if (len(np.where(noise_segDict[detectors[d]]==0.0)[0])
+                            ==len(noise_segDict[detectors[d]])):
+                            raise ValueError("Detector "+detectors[d]+" is full of zeros")
+                        elif len(np.where(noise_segDict[detectors[d]]==0.0)[0])!=0:
+                            print("WARNING : "+str(
+                                len(np.where(noise_segDict[detectors[d]]==0.0)[0]))
+                                  +" zeros were replased with the average of the array")
+                        print("Success on getting the "+str(detectors[d])+" data.")
+                        break
+
+                    except Exception as e:
+                        print(e.__class__,e)
+                        print("/n")
+                        print("Failed getting the "+str(detectors[d])+" data.\n")
+
+                        #waiting=140+120*np.random.rand()
+                        #os.system("sleep "+str(waiting))
+                        #print("waiting "+str(waiting)+"s")
+                        continue
+
+                gps0[detectors[d]] = float(noiseSourceFile[d][0])
+
+            ind=internalLags(detectors = detectors
+                               ,lags = timeSlides
                                ,duration = duration
-                               ,metadata = podMetadata))   
-        random.shuffle(DATA.dataPods)
-        if savePath!=None:
-            DATA.save(savePath+'/'+name,'pkl')
-        else:
-            return(DATA)
+                               ,fs = fs
+                               ,size = int(len(noise_segDict[detectors[0]])/fs-(windowSize-duration))
+                               ,start_from_sec=startingPoint)
 
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
+#             print(len(ind['H']),len(ind['L']))
+#             print(len(noise_segDict['H'])/fs,len(noise_segDict['L'])/fs)
 
 
-import string
+
+    thetime = time.time()
+    DATA=DataSet(name = name)
+    for I in range(size):
+
+
+        t0=time.time()
+
+        detKeys = list(injectionFileDict.keys())
+
+        if single == True: luckyDet = np.random.choice(detKeys)
+        if isinstance(disposition,(list,tuple)):
+            disposition_=disposition[0]+np.random.rand()*(disposition[1]-disposition[0])
+            maxDuration_=min(duration-disposition_,maxDuration)
+
+        index_selection={}
+        if injection_source != None:
+            if differentSignals==True:
+                if maxDuration_ != duration:
+                    for det in detectors: 
+                        index_sample=np.random.randint(0,
+                                                  len(injectionFileDict[detKeys[0]]))
+
+                        if inj_type =='oldtxt':
+                            sampling_strain=np.loadtxt(injection_source+'/'
+                                                       +det+'/'+injectionFileDict[det][index_sample])
+
+                        elif inj_type == 'directory':
+                            s_pod=DataPod.load(injection_source+
+                                                         '/'+injectionFileDict[det][index_sample])
+                            sampling_strain=s_pod.strain[s_pod.detectors.index(det)]
+
+                        # case where we pass one pod only
+                        elif inj_type == 'DataPod':
+                            raise TypeError("You cannot have single pod for inejctions and "
+                                            +" also differentSignals = True")
+
+                        elif inj_type == 'DataSet':
+                            s_pod = injectionFileDict[det][index_sample] 
+                            sampling_strain=s_pod.strain[s_pod.detectors.index(det)]
+
+                        index_selection[det]=index_sample
+
+                        while (len(sampling_strain)/fs > maxDuration_ 
+                               or list(index_selection.values()).count(index_sample) > 1 ):
+
+                            index_sample=np.random.randint(0,
+                                                      len(injectionFileDict[detKeys[0]]))
+
+                            if inj_type=='oldtxt':
+                                sampling_strain=np.loadtxt(injection_source+'/'
+                                                       +det+'/'+injectionFileDict[det][index_sample])
+
+                            elif inj_type == 'directory':
+                                s_pod=DataPod.load(injection_source+
+                                                         '/'+injectionFileDict[det][index_sample])
+                                sampling_strain=s_pod.strain[s_pod.detectors.index(det)]
+
+                            elif inj_type == 'DataSet':
+                                s_pod = injectionFileDict[det][index_sample] 
+                                sampling_strain=s_pod.strain[s_pod.detectors.index(det)]
+
+                            index_selection[det]=index_sample
+
+                else:
+                    for det in detectors: 
+                        index_sample=np.random.randint(0,
+                                                  len(injectionFileDict[detKeys[0]]))
+
+                        index_selection[det]=index_sample
+
+                        while (list(index_selection.values()).count(index_sample) > 1):
+
+                            index_sample=np.random.randint(0,
+                                                      len(injectionFileDict[detKeys[0]]))
+
+                            index_selection[det]=index_sample
+            else:
+                if maxDuration_ != duration:
+                    index_sample=np.random.randint(0,len(injectionFileDict[detKeys[0]]))
+
+                    if inj_type =='oldtxt':
+                        sampling_strain=np.loadtxt(injection_source+'/'
+                                                   +det+'/'+injectionFileDict[det][index_sample])
+
+                    elif inj_type == 'directory':
+                        s_pod=DataPod.load(injection_source+
+                                                     '/'+injectionFileDict[det][index_sample])
+                        sampling_strain=s_pod.strain[s_pod.detectors.index(det)]
+
+                    elif inj_type == 'DataPod':
+                        s_pod=injection_source
+                        sampling_strain=s_pod.strain[s_pod.detectors.index(det)]         
+
+                    elif inj_type == 'DataSet':
+                        s_pod = injectionFileDict[det][index_sample] 
+                        sampling_strain=s_pod.strain[s_pod.detectors.index(det)]
+
+                    while (len(sampling_strain)/fs > maxDuration_
+                           or index_sample in list(index_selection.values())):
+
+                        index_sample=np.random.randint(0,len(injectionFileDict[detKeys[0]]))
+
+                        if inj_type =='oldtxt':
+                            sampling_strain=np.loadtxt(injection_source+'/'
+                                                       +det+'/'+injectionFileDict[det][index_sample])
+
+                        elif inj_type == 'directory':
+                            s_pod=DataPod.load(injection_source+
+                                                         '/'+injectionFileDict[det][index_sample])
+                            sampling_strain=s_pod.strain[s_pod.detectors.index(det)]
+
+                        elif inj_type == 'DataPod':
+                            s_pod=injection_source
+                            sampling_strain=s_pod.strain[s_pod.detectors.index(det)]         
+
+                        elif inj_type == 'DataSet':
+                            s_pod = injectionFileDict[det][index_sample] 
+                            sampling_strain=s_pod.strain[s_pod.detectors.index(det)]
+
+                    for det in detectors: index_selection[det]=index_sample
+                else:
+                    index_sample=np.random.randint(0,len(injectionFileDict[detKeys[0]]))
+                    for det in detectors: index_selection[det]=index_sample
+
+#                 inj_ind = np.random.randint(0,len(injectionFileDict[detKeys[0]]))
+
+        SNR0_dict={}
+        back_dict={}
+        inj_fft_0_dict={}
+        asd_dict={}
+        PSD_dict={}
+        gps_list = []
+
+
+
+        for det in detKeys:
+
+            # In case we want to put different injection to every detectors.
+#                 if differentSignals==True:
+#                     inj_ind = np.random.randint(0,len(injectionFileDict[detKeys[0]]))
+
+            if backgroundType == 'optimal':
+
+                # Creation of the artificial noise.
+                PSD,X,T=simulateddetectornoise(profile[det]
+                                              ,windowSize
+                                              ,fs,10,fs/2
+                                              ,PSDm=PSDm[det]
+                                              ,PSDc=PSDc[det])
+                # Calculatint the psd of FFT=1s
+                p, f = psd(X, Fs=fs,NFFT=fs)
+                # Interpolate so that has t*fs values
+                psd_int=interp1d(f,p)                                     
+                PSD=psd_int(np.arange(0,fs/2,1/windowSize))
+                PSD_dict[det]=PSD
+                back_dict[det] = X
+                # Making the noise a TimeSeries
+                back=TimeSeries(X,sample_rate=fs) 
+                # Calculating the ASD so tha we can use it for whitening later
+                asd=back.asd(1,0.5)
+                asd_dict[det] = asd
+                gps_list.append(0.0)
+
+
+            elif backgroundType == 'sudo_real':
+
+                noise_seg=noise_segDict[det]
+                # Calling the real noise segments
+                noise=noise_seg[int(ind[det][I]):int(ind[det][I])+windowSize*fs]  
+                # Generating the PSD of it
+                p, f = psd(noise, Fs=fs, NFFT=fs) 
+                p, f=p[1::],f[1::]
+                # Feeding the PSD to generate the sudo-real noise.            
+                PSD,X,T=simulateddetectornoise([f,p]
+                                               ,windowSize,fs,10
+                                               ,fs/2,PSDm=PSDm[det]
+                                               ,PSDc=PSDc[det])
+                p, f = psd(X, Fs=fs,NFFT=fs)
+                # Interpolate so that has t*fs values
+                psd_int=interp1d(f,p)                                     
+                PSD=psd_int(np.arange(0,fs/2,1/windowSize))
+                PSD_dict[det]=PSD
+                back_dict[det] = X
+                # Making the noise a TimeSeries
+                back=TimeSeries(X,sample_rate=fs)
+                # Calculating the ASD so tha we can use it for whitening later
+                asd=back.asd(1,0.5)                 
+                asd_dict[det] = asd
+                gps_list.append(gps0[det]+ind[det][I]/fs+(windowSize-duration)/2)
+                back_dict[det] = back.value
+
+            elif backgroundType == 'real':
+                noise_seg=noise_segDict[det]
+                # Calling the real noise segments
+
+                if noiseFormat == 'DataSet':
+                    noise=noise_seg[I]
+
+                else:
+                    noise=noise_seg[int(ind[det][I]):int(ind[det][I])+windowSize*fs]
+                # Calculatint the psd of FFT=1s
+                p, f = psd(noise, Fs=fs,NFFT=fs)
+                # Interpolate so that has t*fs values
+                psd_int=interp1d(f,p)                                     
+                PSD=psd_int(np.arange(0,fs/2,1/windowSize))
+                PSD_dict[det]=PSD
+                # Making the noise a TimeSeries
+                back=TimeSeries(noise,sample_rate=fs)
+                back_dict[det] = back
+                # Calculating the ASD so tha we can use it for whitening later
+                #print(det,back,len(back),type(back))
+                asd=back.asd(1,0.5)
+                asd_dict[det] = asd
+                if noiseFormat == 'DataSet':
+                    gps_list.append(gps0[det]+ind[det][I]+(windowSize-duration)/2)
+                else:
+                    gps_list.append(gps0[det]+ind[det][I]/fs+(windowSize-duration)/2)
+
+            #If this dataset includes injections:            
+            if injection_source != None:      
+
+                # Calling the templates generated with PyCBC
+                # OLD inj=load_inj(injection_source,injectionFileDict[det][inj_ind], det) 
+                if inj_type =='oldtxt':
+                    inj = np.loadtxt(injection_source+'/'
+                                     +det+'/'+injectionFileDict[det][index_selection[det]])
+
+                elif inj_type == 'directory':
+                    inj_pod=DataPod.load(injection_source+'/'+injectionFileDict[det][index_selection[det]])
+                    inj=np.array(inj_pod.strain[inj_pod.detectors.index(det)])
+
+
+                elif inj_type == 'DataPod':
+                    inj_pod=injection_source
+                    inj=np.array(inj_pod.strain[inj_pod.detectors.index(det)])
+
+                elif inj_type == 'DataSet':
+                    inj_pod = injectionFileDict[det][index_selection[det]]
+                    inj=np.array(inj_pod.strain[inj_pod.detectors.index(det)])
+
+                if inj_type in ['DataSet','DataPod','directory']:
+
+                    if injectionHRSS!=None:
+                        if 'hrss' in inj_pod.pluginDict.keys():
+                            hrss0=inj_pod.hrss
+                        else:
+                            raise AttributeError("There is no hrss in the injection pod")
+                    else:
+                        if 'hrss' in inj_pod.pluginDict.keys():
+                            hrss0=inj_pod.hrss
+
+
+                # Saving the length of the injection
+                inj_len = len(inj)/fs
+                inj_len_original=min(inj_len,duration)
+                # I put a random offset for all injection so that
+                # the signal is not always in the same place
+                if inj_len > duration: 
+                    print('Injection was cropped symmetricaly by '
+                          +str(inj_len_original-fs*duration)+' to fit duration.')
+
+                    inj = inj[int((inj_len-duration)*fs/2):]
+                    inj_len_=len(inj)/fs                    
+                    inj = inj[:int(duration*fs)]
+                    inj_len = len(inj)/fs
+
+                if inj_len <= duration:
+                    inj = np.hstack((np.zeros(int(fs*(duration-inj_len)/2)), inj))
+                    inj_len_=len(inj)/fs                    
+                    inj = np.hstack((inj, np.zeros(int(fs*(duration-inj_len_)))))
+
+                # DISPOSITIONS
+
+                # Default case when coherent
+                if disposition == 0:
+                    if det == detKeys[0]:
+                        disp = np.random.random_integers(low = min(-int(fs*(duration-inj_len_original)/2),0) 
+                                                       ,high = max(int(fs*((duration-inj_len_original)/2 
+                                                                     + injectionCrop*(duration))),1))
+
+#                     # Case when signals will be randomly positioned for each detector seperatly. 
+#                     # Does not affect if signals will be different or not.
+#                     elif isinstance(disposition,(list,tuple):
+#                         disp = np.random.random_integers(low = min(-int(fs*(duration-inj_len)/2),0) 
+#                                                          ,high = max(int(fs*((duration-inj_len)/2 
+#                                                                          + injectionCrop*(duration-0.1))),1))
+                # Case when signals will be positioned within a duration stated by the disposition.
+                # The center of this duration will be moved randomly given the maxDuration
+                # of the injections.
+                elif isinstance(disposition_,(int,float)) and disposition_>0:
+                    if det == detKeys[0]:
+                        wind = 0.2*disposition_/max((len(detKeys)-1),1)
+                        center_position = np.random.random_integers(
+                            low = min(-int(fs*(duration-maxDuration_-disposition_)/2),0)
+                           ,high = max(int(fs*(duration-maxDuration_-disposition_)/2)+1,1))
+                            # the +1 is because there is an error if the high becomes 0
+
+                        if len(detKeys)>1:
+                            positions=np.arange(-disposition_/2,disposition_/2+0.0001 
+                                                ,disposition_/max((len(detKeys)-1),1))
+                            positions=list([positions[0]+np.random.rand()*wind/2]
+                                 +list(p+np.random.rand()*wind-wind/2 for p in positions[1:-1])
+                                 +[positions[-1]-np.random.rand()*wind/2])
+
+                        else:
+                            positions=[0.0+np.random.rand()*wind/2]
+
+                        np.random.shuffle(positions)
+                    disp = center_position+int(positions[detKeys.index(det)]*fs)
+
+
+                if disp >= 0: 
+                    inj = np.hstack((np.zeros(int(fs*(windowSize-duration)/2)),inj[disp:]
+                                         ,np.zeros(int(fs*(windowSize-duration)/2)+disp)))   
+                if disp < 0: 
+                    inj = np.hstack((np.zeros(int(fs*(windowSize-duration)/2)-disp),inj[:disp]
+                                         ,np.zeros(int(fs*(windowSize-duration)/2)))) 
+
+
+                # Calculating the one sided fft of the template,
+                # Norm default is 'backwards' which means that it normalises with 1/N during IFFT and not duriong FFT
+                inj_fft_0=(1/fs)*np.fft.fft(inj)
+                inj_fft_0_dict[det] = inj_fft_0
+
+                # Getting rid of negative frequencies and DC
+                inj_fft_0N= inj_fft_0[1:int(windowSize*fs/2)+1]
+
+
+                SNR0_dict[det]=np.sqrt((1/windowSize #(fs/N=fs/fs*windowSize 
+                                       )*4*np.sum( # 2 from PSD, S=1/2 S1(one sided) and 2 from integral symetry
+                    np.abs(inj_fft_0N*inj_fft_0N.conjugate())[windowSize*fl-1:windowSize*fm-1]
+                                               /PSD_dict[det][windowSize*fl-1:windowSize*fm-1]))
+
+                if single == True:
+                    if det != luckyDet:
+                        SNR0_dict[det] = 0.01 # Making single detector injections as glitch
+                        inj_fft_0_dict[det] = np.zeros(windowSize*fs)
+
+
+            else:
+                SNR0_dict[det] = 0.01 # avoiding future division with zero
+                inj_fft_0_dict[det] = np.zeros(windowSize*fs)
+
+
+#             print(
+#                 list(
+#                     len(np.where(
+#                         noise_segDict[det][int(ind[det][I]):int(ind[det][I])+windowSize*fs]
+#                     )[0]
+#                        )
+#                     for det in detKeys
+#                 )
+#             )
+        if (backgroundType=='real' 
+            and any(len(np.where(noise_segDict[det][
+                int(ind[det][I]):int(ind[det][I])+windowSize*fs]==0)[0])==windowSize*fs for det in detKeys)):
+            print(I,"skipped")
+            continue
+
+        # Calculation of combined SNR    
+        SNR0=np.sqrt(np.sum(np.asarray(list(SNR0_dict.values()))**2))
+
+        # Tuning injection amplitude to the SNR wanted
+        podstrain = []
+        podPSD = []
+        podCorrelations=[]
+        SNR_new=[]
+        SNR_new_sq_sum=0
+        psdPlugDict={}
+        plugInToApply=[]
+
+        for det in detectors:
+            if injectionHRSS!=None:
+                fft_cal=(injectionHRSS/hrss0)*inj_fft_0_dict[det]         
+            else:
+                fft_cal=(injectionSNR/SNR0)*inj_fft_0_dict[det] 
+            # Norm default is 'backwards' which means that it normalises with 1/N during IFFT and not duriong FFT
+            if ignoreDetector ==None:
+                inj_cal=np.real(np.fft.ifft(fs*fft_cal)) 
+            elif ignoreDetector==det:
+                inj_cal=0.0001*np.real(np.fft.ifft(fs*fft_cal)) 
+            else:
+                inj_cal=np.real(np.fft.ifft(fs*fft_cal)) 
+            # Joining calibrated injection and background noise
+            strain=TimeSeries(back_dict[det]+inj_cal,sample_rate=fs,t0=0).astype('float64')
+            #print(det,len(strain),np.prod(np.isfinite(strain)),len(strain)-np.sum(np.isfinite(strain)))
+            #print(det,len(strain),'zeros',len(np.where(strain.value==0.0)[0]))
+            #print(strain.value.tolist())
+            # Bandpassing
+            # strain=strain.bandpass(20,int(fs/2)-1)
+            # Whitenning the data with the asd of the noise
+            whiten_strain=strain.whiten(4,2,fduration=4,method = 'welch', highpass=20)#,asd=asd_dict[det])
+
+            #print(det,len(strain),np.prod(np.isfinite(strain)),len(strain)-np.sum(np.isfinite(strain)))
+            #print(det,len(strain),'zeros',len(np.where(strain.value==0.0)[0]))
+
+            # Crop data to the duration length
+            whiten_strain=whiten_strain[int(((windowSize-duration)/2)*fs):int(((windowSize+duration)/2)*fs)]
+            podstrain.append(whiten_strain.value.tolist())
+
+            if 'snr' in plugins:
+                whiten_strain_median=strain.whiten(4,2,fduration=4,method = 'median'
+                        , highpass=20)[int(((windowSize-duration)/2)*fs):int(((windowSize+duration)/2)*fs)]
+                # This is strictly for duration 1 and fs 1024
+                new_snr = np.sum(whiten_strain_median.value**2 -0.978**2)
+
+                SNR_new.append(np.sqrt(max(new_snr,0)))
+                SNR_new_sq_sum += new_snr
+
+
+            # if 'snr' in plugins:
+            #     # Adding snr value as plugin.
+            #     # Calculating the new SNR which will be slightly different that the desired one.    
+            #     inj_fft_N=fft_cal[1:int(windowSize*fs/2)+1]
+            #     SNR_new.append(np.sqrt((1/windowSize #(fs/fs*windowsize
+            #                            )*4*np.sum( # 2 from integral + 2 from S=1/2 S1(one sided)
+            #         np.abs(inj_fft_N*inj_fft_N.conjugate())[windowSize*fl-1:windowSize*fm-1]
+            #                                  /PSD_dict[det][windowSize*fl-1:windowSize*fm-1])))
+
+            #     plugInToApply.append(PlugIn('snr'+det,SNR_new[-1]))
+
+            if 'psd' in plugins:
+                podPSD.append(asd_dict[det]**2)
+
+        if 'snr' in plugins: 
+
+            network_snr = np.sqrt(max(SNR_new_sq_sum,0))
+            SNR_new.append(network_snr)
+            plugInToApply.append(PlugIn('snr',SNR_new))
+
+
+
+
+        if 'psd' in plugins:
+            plugInToApply.append(PlugIn('psd'
+                                        ,genFunction=podPSD
+                                        ,plotFunction=plotpsd
+                                        ,plotAttributes=['detectors','fs']))
+
+        for pl in plugins:
+            if 'correlation' in pl:
+                plugInToApply.append(knownPlugIns(pl))
+
+
+
+        pod = DataPod(strain = podstrain
+                           ,fs = fs
+                           ,labels =  labels
+                           ,detectors = detKeys
+                           ,gps = gps_list
+                           ,duration = duration)
+
+        if injection_source!=None and inj_type in ['DataSet','DataPod','directory']:
+
+            for plkey in list(inj_pod.pluginDict.keys()):
+                if not (plkey in list(pod.pluginDict.keys())):
+                    pod.addPlugIn(inj_pod.pluginDict[plkey])
+
+        if 'hrss' in plugins: 
+            if 'hrss' in inj_pod.pluginDict.keys():
+                if injectionHRSS!=None:
+                    plugInToApply.append(PlugIn('hrss'
+                                            ,genFunction=inj_pod.hrss*(injectionHRSS/hrss0)))
+                else:
+                    plugInToApply.append(PlugIn('hrss'
+                                            ,genFunction=inj_pod.hrss*(injectionSNR/SNR0)))
+
+            else:
+                print("Warning: Unable to calculate hrss, There was no hrss in the injection pod.")
+
+        for pl in plugInToApply:
+            pod.addPlugIn(pl)
+
+        DATA.add(pod)
+
+        #t1=time.time()
+        #sys.stdout.write("\r Instantiation %i / %i --- %s" % (I+1, size, str(t1-t0)))
+        #sys.stdout.flush()
+        #t0=time.time()
+
+    if not ('shuffle' in kwargs):
+        kwargs['shuffle'] = True
+
+    if not isinstance(kwargs['shuffle'],bool):
+        raise TypeError("shuffle option must be a bool value")
+
+    if kwargs['shuffle']==True:
+         random.shuffle(DATA.dataPods)
+    # else if false do not shuffle.
+
+    print('\n')
+    if savePath!=None:
+        DATA.save(savePath+'/'+name,'pkl')
+    else:
+        return(DATA)
+
+
+
+    
 
 def auto_gen(duration 
              ,fs
              ,detectors
              ,size
              ,injectionFolder = None
              ,labels = None
@@ -1111,15 +1291,17 @@
              ,single = False  # Making single detector injections as glitch
              ,injectionCrop = 0   # Allowing part precentage of the injection to be croped
                                   # so that the signal can move from the center. Used only 
                                   # when injection duration = duaration
              ,disposition=None
              ,maxDuration=None
              ,differentSignals=False
-             ,extras=None): 
+             ,plugins=None
+             ,finalDirectory=None
+             ,**kwargs): 
 
 
 
 
     # ---------------------------------------------------------------------------------------- #
     # --- duration --------------------------------------------------------------------------- #
 
@@ -1153,15 +1335,15 @@
     if isinstance(detectors,str):
         detectors = list(detectors)
 
     # ---------------------------------------------------------------------------------------- #    
     # --- size ------------------------------------------------------------------------------- #        
 
     if not (isinstance(size, int) and size > 0):
-        raise ValuError("size must be a possitive integer.")
+        raise ValueError("size must be a possitive integer.")
 
 
     # ---------------------------------------------------------------------------------------- #
     # --- injectionFolder -------------------------------------------------------------------- #
 
     if injectionFolder == None:
         pass
@@ -1170,15 +1352,15 @@
             injectionFolder_set = injectionFolder.split('/')[-1]
         elif (('/' not in injectionFolder) and any('injections' in p for p in sys.path)):
             for p in sys.path:
                 if ('injections' in p):
                     injectionFolder_path = (p.split('injections')[0]+'injections'
                         +'/'+injectionFolder)
                     if os.path.isdir(injectionFolder_path):
-                        injectionFolder = injectionFolder_path
+                        injectionFolder = "'"+injectionFolder_path+"'"
                         injectionFolder_set = injectionFolder.split('/')[-1]
                     else:
                         raise FileNotFoundError('No such file or directory:'
                                                 +injectionFolder_path)
 
         else:
             raise FileNotFoundError('No such file or directory:'+injectionFolder) 
@@ -1253,15 +1435,15 @@
     else:
         raise TypeError("Path must be a string")
             
     
     # ---------------------------------------------------------------------------------------- #    
     # --- windowSize --(for PSD)-------------------------------------------------------------- #        
 
-    if windowSize == None: windowSize = duration*8
+    if windowSize == None: windowSize = duration*16
     if not isinstance(windowSize,int):
         raise ValueError('windowSize needs to be an integral')
     if windowSize < duration :
         raise ValueError('windowSize needs to be bigger than the duration')
 
     # ---------------------------------------------------------------------------------------- #    
     # --- timeSlides ------------------------------------------------------------------------- #
@@ -1293,15 +1475,28 @@
         if not os.path.isdir(savePath) : 
             raise FileNotFoundError('No such file or directory:' +savePath)
     else:
         raise TypeError("Destination Path has to be a string valid path")
     if savePath[-1] == '/' : savePath=savePath[:-1]
     
     # ---------------------------------------------------------------------------------------- #    
-               
+    
+    # Accounting group options
+    if 'accounting_group_user' in kwargs:
+        accounting_group_user=kwargs['accounting_group_user']
+    else:
+        accounting_group_user=os.environ['LOGNAME']
+        
+    if 'accounting_group' in kwargs:
+        accounting_group=kwargs['accounting_group']
+    else:
+        accounting_group='ligo.dev.o3.burst.grb.xoffline'
+        print("Accounting group set to 'ligo.dev.o3.burst.grb.xoffline")
+    
+   
     # The number of sets to be generated.
     num_of_sets = len(injectionSNR)
 
     # If noise is optimal it is much more simple
     if backgroundType == 'optimal':
 
         d={'size' : num_of_sets*[size]
@@ -1393,20 +1588,20 @@
 
             # local size indicates the size of the file left for generation 
             # of datasets, when it is depleted the algorithm moves to the next               
             # segment. Here we infere the local size given the timeSlides used in 
             # the method.
 
             if timeSlides==1:    # zero lag case
-                local_size=ceil((duration_[i]-3*windowSize-tail_crop)/duration)
+                local_size=int((duration_[i]-3*windowSize-tail_crop)/duration) #changed ceil to int
             if timeSlides%2 == 0:
-                local_size=ceil((duration_[i]-3*windowSize-tail_crop)
+                local_size=int((duration_[i]-3*windowSize-tail_crop)
                                 /duration/timeSlides)*timeSlides*(timeSlides-2)
             if timeSlides%2 != 0 and timeSlides !=1 :
-                local_size=ceil((duration_[i]-3*windowSize-tail_crop)
+                local_size=int((duration_[i]-3*windowSize-tail_crop)
                                 /duration/timeSlides)*timeSlides*(timeSlides-1)
 
             # starting point always begins with the window of the psd to avoid
             # deformed data of the begining    
             local_starting_point=windowSize
 
             # There are three cases when a segment is used.
@@ -1529,34 +1724,45 @@
 
         print('These are the details of the datasets to be generated: \n')
         for i in range(len(d['segment'])):
             print(d['segment'][i], d['size'][i], d['start_point'][i] ,d['name'][i])
         
         
     answers = ['no','n', 'No','NO','N','yes','y','YES','Yes','Y','exit']
-    answer = None
+    if finalDirectory==None:
+        answer=None
+    else:
+        answer='y'
+        
     while answer not in answers:
         print('Should we proceed to the generation of the following'
               +' data y/n ? \n \n')
         answer=input()
         if answer not in answers: print("Not valid answer ...")
     
     if answer in ['no','n', 'No','NO','N','exit']:
         print('Exiting procedure ...')
         return
     elif answer in ['yes','y','YES','Yes','Y']:
-        print('Type the name of the dataset directory:')
-        dir_name = '0 0'
+        if finalDirectory==None:
+            print('Type the name of the temporary directory:')
+            dir_name = '0 0'
+        else:
+            dir_name = finalDirectory
+        
         while not dir_name.isidentifier():
             dir_name=input()
             if not dir_name.isidentifier(): print("Not valid Folder name ...")
         
     path = savePath+'/'
     print("The current path of the directory is: \n"+path+dir_name+"\n" )  
-    answer = None
+    if finalDirectory==None:
+        answer=None
+    else:
+        answer='y'
     while answer not in answers:
         print('Do you accept the path y/n ?')
         answer=input()
         if answer not in answers: print("Not valid answer ...")
 
     if answer in ['no','n', 'No','NO','N','exit']:
         print('Exiting procedure ...')
@@ -1575,168 +1781,171 @@
             elif answer in ['no','n', 'No','NO','N']:
                 print('Generation is cancelled\n')
                 print('Exiting procedure ...')
                 return
             
     print('Initiating procedure ...')
     os.system('mkdir '+path+dir_name)
+    
+    error = path+dir_name+'/condor/error'
+    output = path+dir_name+'/condor/output'
+    log = path+dir_name+'/condor/log'
+    submit = path+dir_name+'/condor/submit'
+
+    dagman = Dagman(name='falsAlarmDagman',
+            submit=submit)
+    job_list=[]
+    
     print('Creation of directory complete: '+path+dir_name)
-    os.system('cd '+path+dir_name)
-                
+    #os.system('cd '+path+dir_name)
+    
+    kwstr=""
+    for k in kwargs:
+        kwstr+=(","+k+"="+str(kwargs[k]))           
 
     for i in range(len(d['size'])):
 
         with open(path+dir_name+'/'+'gen_'+d['name'][i]+'_'
             +str(d['size'][i])+'.py','w') as f:
             f.write('#! /usr/bin/env python3\n')
             f.write('import sys \n')
-            #This path is used only for me to test it
-            pwd=os.getcwd()
-            if 'vasileios.skliris' in pwd:
-                f.write('sys.path.append(\'/home/vasileios.skliris/mly/\')\n')
+            f.write('sys.path.append(\'/home/'+accounting_group_user+'/mly/\')\n')
 
             f.write('from mly.datatools import DataPod, DataSet\n\n')
 
             if isinstance(d['set'][i],(float,int)):
                 token_snr = str(d['set'][i])
             else:
                 token_snr = '0'
             f.write("import time\n\n")
             f.write("t0=time.time()\n")
             
+            if injectionFolder!=None and injectionFolder[0]!="'":
+                injectionFolder = "'"+injectionFolder+"'"
+
             if backgroundType == 'optimal':
-                comand=( "SET = DataSet.generator(\n"
+                comand=( "SET = generator(\n"
                          +24*" "+"duration = "+str(duration)+"\n"
                          +24*" "+",fs = "+str(fs)+"\n"
                          +24*" "+",size = "+str(d['size'][i])+"\n"
                          +24*" "+",detectors = "+str(detectors)+"\n"
-                         +24*" "+",injectionFolder = '"+str(injectionFolder)+"'\n"
+                         +24*" "+",injectionFolder ="+str(injectionFolder)+"\n"
                          +24*" "+",labels = "+str(labels)+"\n"
                          +24*" "+",backgroundType = '"+str(backgroundType)+"'\n"
                          +24*" "+",injectionSNR = "+token_snr+"\n"
                          +24*" "+",name = '"+str(d['name'][i])+"_"+str(d['size'][i])+"'\n"
                          +24*" "+",savePath ='"+path+dir_name+"'\n"
                          +24*" "+",single = "+str(single)+"\n"
                          +24*" "+",injectionCrop = "+str(injectionCrop)+"\n"
                          +24*" "+",differentSignals = "+str(differentSignals)+"\n"
-                         +24*" "+",extras = "+str(extras)+")\n")
+                         +24*" "+",plugins = "+str(plugins)+kwstr+")\n")
 
             else:
                 f.write("sys.path.append('"+date_list_path[:-1]+"')\n")
-                comand=( "SET = DataSet.generator(\n"
+                comand=( "SET = generator(\n"
                          +24*" "+"duration = "+str(duration)+"\n"
                          +24*" "+",fs = "+str(fs)+"\n"
                          +24*" "+",size = "+str(d['size'][i])+"\n"
                          +24*" "+",detectors = "+str(detectors)+"\n"
-                         +24*" "+",injectionFolder = '"+str(injectionFolder)+"'\n"
+                         +24*" "+",injectionFolder = "+str(injectionFolder)+"\n"
                          +24*" "+",labels = "+str(labels)+"\n"
                          +24*" "+",backgroundType = '"+str(backgroundType)+"'\n"
                          +24*" "+",injectionSNR = "+token_snr+"\n"
                          +24*" "+",noiseSourceFile = "+str(d['segment'][i])+"\n"
                          +24*" "+",windowSize ="+str(windowSize)+"\n"
                          +24*" "+",timeSlides ="+str(timeSlides)+"\n"
                          +24*" "+",startingPoint = "+str(d['start_point'][i])+"\n"
                          +24*" "+",name = '"+str(d['name'][i])+"_"+str(d['size'][i])+"'\n"
                          +24*" "+",savePath ='"+path+dir_name+"'\n"
                          +24*" "+",single = "+str(single)+"\n"
                          +24*" "+",injectionCrop = "+str(injectionCrop)+"\n"
                          +24*" "+",differentSignals = "+str(differentSignals)+"\n"
-                         +24*" "+",extras = "+str(extras)+")\n")
+                         +24*" "+",plugins = "+str(plugins)+kwstr+")\n")
 
             
             f.write(comand+'\n\n')
             f.write("print(time.time()-t0)\n")
-            f.write("sys.stdout.flush()")
-    with open(path+dir_name+'/'+'auto_gen.sh','w') as f2:
 
-        f2.write('#!/usr/bin/bash \n\n')
-        f2.write("commands=()\n\n")
-        
-        for i in range(len(d['size'])):
+        os.system('chmod 777 '+path+dir_name+'/'+'gen_'+d['name'][i]+'_'
+            +str(d['size'][i])+'.py' )
+        job = Job(name='partOfGeneration_'+str(i)
+                  ,executable=path+dir_name+'/'+'gen_'+d['name'][i]+'_'+str(d['size'][i])+'.py' 
+               ,submit=submit
+               ,error=error
+               ,output=output
+               ,log=log
+               ,getenv=True
+               ,dag=dagman
+               ,retry=10
+               ,extra_lines=["accounting_group_user="+accounting_group_user
+                             ,"accounting_group="+accounting_group
+                             ,"request_disk            = 64M"] )
 
-            f2.write("commands+=('"+'nohup python '+path+dir_name+'/gen_'+d['name'][i]
-                +'_'+str(d['size'][i])+'.py > '+path+dir_name+'/out_gen_'
-                +d['name'][i]+'_'+str(d['size'][i])+'.out &'+"')\n")
-            
-        f2.write("# Number of processes\n")
-        f2.write("N="+str(len(d['size']))+"\n\n")
-        f2.write("ProcessLimit=$(($(grep -c ^processor /proc/cpuinfo)/2))\n")
-        f2.write("jobArray=()\n")
-        f2.write("countOurActiveJobs(){\n")
-        f2.write("    activeid=$(pgrep -u $USER)\n")
-        f2.write("    jobsN=0\n")
-        f2.write("    for i in ${jobArray[*]}; do  \n")
-        f2.write("        for j in ${activeid[*]}; do  \n")     
-        f2.write("            if [ $i = $j ]; then\n")
-        f2.write("                jobsN=$(($jobsN+1))\n")
-        f2.write("            fi\n")
-        f2.write("        done\n")
-        f2.write("    done\n")
-        f2.write("}\n\n")
-        f2.write("eval ProcessList=({1..$N})\n")
-        f2.write("for (( k = 0; k < ${#commands[@]} ; k++ ))\n")
-        f2.write("do\n")
-        f2.write("    countOurActiveJobs\n")
-        f2.write("    echo \"Number of jobs running: $jobsN\"\n")
-        f2.write("    while [ $jobsN -ge $ProcessLimit ]\n")
-        f2.write("    do\n")
-        f2.write("        echo \"Waiting for space\"\n")
-        f2.write("        sleep 10\n")
-        f2.write("        countOurActiveJobs\n")
-        f2.write("    done\n")
-        f2.write("    eval ${commands[$k]}\n")
-        f2.write("    jobArray+=$(echo \"$! \")\n")
-        f2.write("done\n\n")
-        
-        f2.write("countOurActiveJobs\n")
-        f2.write("while [ $jobsN != 0 ]\n")
-        f2.write("do\n")
-        f2.write("    echo \"Genrating... \"\n")
-        f2.write("    sleep 60\n")
-        f2.write("    countOurActiveJobs\n")
-        f2.write("done\n")
-        f2.write("nohup python "+path+dir_name+"/final_gen.py > "+path+dir_name+"/final_gen.out")
+        job_list.append(job)
 
     with open(path+dir_name+'/info.txt','w') as f3:
         f3.write('INFO ABOUT DATASETS GENERATION \n\n')
         f3.write('fs: '+str(fs)+'\n')
         f3.write('duration: '+str(duration)+'\n')
         f3.write('window: '+str(windowSize)+'\n')
+        if injectionFolder!=None:
+            f3.write('injectionFolder: '+str(injectionFolder)+'\n')
+        
         if backgroundType != 'optimal':
             f3.write('timeSlides: '+str(timeSlides)+'\n'+'\n')
-
             for i in range(len(d['size'])):
                 f3.write(d['segment'][i][0]+' '+d['segment'][i][1]
                          +' '+str(d['size'][i])+' '
                          +str(d['start_point'][i])+'_'+d['name'][i]+'\n')
-            
     with open(path+dir_name+'/final_gen.py','w') as f4:
         f4.write("#! /usr/bin/env python3\n")
-        pwd=os.getcwd()
-        if 'vasileios.skliris' in pwd:
-            f4.write("import sys \n")
-            f4.write("sys.path.append('/home/vasileios.skliris/mly/')\n")
+        f4.write("import sys \n")
+        f4.write("sys.path.append('/home/"+accounting_group_user+"/mly/')\n")
         f4.write("from mly.datatools import *\n")
         f4.write("finalise_gen('"+path+dir_name+"')\n")
+        
+    os.system('chmod 777 '+path+dir_name+'/final_gen.py')
+    final_job = Job(name='finishing'
+               ,executable=path+dir_name+'/final_gen.py'
+               ,submit=submit
+               ,error=error
+               ,output=output
+               ,log=log
+               ,getenv=True
+               ,dag=dagman
+               ,extra_lines=["accounting_group_user="+accounting_group_user
+                             ,"accounting_group="+accounting_group
+                             ,"request_disk            = 64M"])
+    
+    final_job.add_parents(job_list)
+    
+    if finalDirectory==None:
+        print('All set. Initiate dataset generation y/n?')
+        answer4=input()
+    else:
+        answer4='y'
 
-    print('All set. Initiate dataset generation y/n?')
-    answer4=input()
 
     if answer4 in ['yes','y','YES','Yes','Y']:
-        os.system('nohup sh '+path+dir_name+'/auto_gen.sh > '+path+dir_name+'/auto_gen.out &')
+        print('Creating Job queue')
+        
+        dagman.build_submit()
+
         return
+    
     else:
         print('Data generation canceled')
         os.system('cd')
         os.system('rm -r '+path+dir_name)
         return
 
 
     
-def finalise_gen(path):
+    
+def finalise_gen(path,generation=True,**kwargs):
     
     if path[-1]!='/': path=path+'/' # making sure path is right
     files=dirlist(path)             # making a list of files in that path 
     merging_flag=False              # The flag that makes the fusion to happen
 
     print('Running diagnostics for file: '+path+'  ... \n') 
     pyScripts=[]
@@ -1764,72 +1973,76 @@
             for dataset in dataSets:
                 if pyScripts_id in dataset:
                     counter=1
             if counter==0:
                 print(pyScripts[i],' failed to proceed')
                 failed_pyScripts.append(pyScripts[i])
                 
-                
-    if merging_flag==False:
+    # Accounting group options
+    if 'accounting_group_user' in kwargs:
+        accounting_group_user=kwargs['accounting_group_user']
+    else:
+        accounting_group_user=os.environ['LOGNAME']
+        
+    if 'accounting_group' in kwargs:
+        accounting_group=kwargs['accounting_group']
+    else:
+        accounting_group='ligo.dev.o3.burst.grb.xoffline'
+        print("Accounting group set to 'ligo.dev.o3.burst.grb.xoffline")
+    
+    
+    if merging_flag==False and generation==True:
+        
+        with open(path+'/'+'flag_file.sh','w+') as f2:
+             f2.write('#!/usr/bin/bash +x\n\n')
+        print(path)
+        error = path+'condor/error'
+        output = path+'condor/output'
+        log = path+'condor/log'
+        submit = path+'condor/submit'
+
+        repeat_dagman = Dagman(name='repeat_genDagman',
+                submit=submit)
+        repeat_job_list=[]
         
         if os.path.isfile(path+'/'+'auto_gen_redo.sh'):
             print("\nThe following scripts failed to run trough:\n")
-            for failed_pyScript in failed_pyScripts:
-                print(failed_pyScript+"\n")
-        else:
-            with open(path+'/'+'auto_gen_redo.sh','w') as f2:
-
-                f2.write('#!/usr/bin/bash +x\n\n')
-                f2.write("commands=()\n\n")
+            for script in failed_pyScripts:
+                    
+                repeat_job = Job(name='partOfGeneration_'+str(i)
+                           ,executable=path+script
+                           ,submit=submit
+                           ,error=error
+                           ,output=output
+                           ,log=log
+                           ,getenv=True
+                           ,dag=repeat_dagman
+                           ,retry=10
+                           ,extra_lines=["accounting_group_user="+accounting_group_user
+                             ,"accounting_group="+accounting_group
+                             ,"request_disk            = 64M"])
 
-                for script in failed_pyScripts:
+                repeat_job_list.append(repeat_job)
 
-                    f2.write("commands+=('"+'nohup python '+path+script
-                             +' > '+path+'out_'+script[:-3]+'.out &'+"')\n")
-
-                f2.write("# Number of processes\n")
-                f2.write("N="+str(len(failed_pyScripts))+"\n\n")
-                f2.write("ProcessLimit=$(($(grep -c ^processor /proc/cpuinfo)/2))\n")
-                f2.write("jobArray=()\n")
-                f2.write("countOurActiveJobs(){\n")
-                f2.write("    activeid=$(pgrep -u $USER)\n")
-                f2.write("    jobsN=0\n")
-                f2.write("    for i in ${jobArray[*]}; do  \n")
-                f2.write("        for j in ${activeid[*]}; do  \n")     
-                f2.write("            if [ $i = $j ]; then\n")
-                f2.write("                jobsN=$(($jobsN+1))\n")
-                f2.write("            fi\n")
-                f2.write("        done\n")
-                f2.write("    done\n")
-                f2.write("}\n\n")
-                f2.write("eval ProcessList=({1..$N})\n")
-                f2.write("for (( k = 0; k < ${#commands[@]} ; k++ ))\n")
-                f2.write("do\n")
-                f2.write("    countOurActiveJobs\n")
-                f2.write("    echo \"Number of jobs running: $jobsN\"\n")
-                f2.write("    while [ $jobsN -ge $ProcessLimit ]\n")
-                f2.write("    do\n")
-                f2.write("        echo \"Waiting for space\"\n")
-                f2.write("        sleep 10\n")
-                f2.write("        countOurActiveJobs\n")
-                f2.write("    done\n")
-                f2.write("    eval ${commands[$k]}\n")
-                f2.write("    jobArray+=$(echo \"$! \")\n")
-                f2.write("done\n\n")
-
-                f2.write("countOurActiveJobs\n")
-                f2.write("while [ $jobsN != 0 ]\n")
-                f2.write("do\n")
-                f2.write("    echo \"Genrating... \"\n")
-                f2.write("    sleep 60\n")
-                f2.write("    countOurActiveJobs\n")
-                f2.write("done\n")
-                f2.write("nohup python "+path+"/final_gen.py > "+path+"/final_gen.out")
+               
+        repeat_final_job = Job(name='repeat_finishing'
+                           ,executable=path+'finalise_gen.py'
+                           ,submit=submit
+                           ,error=error
+                           ,output=output
+                           ,log=log
+                           ,getenv=True
+                           ,dag=repeat_dagman
+                           ,extra_lines=["accounting_group_user="+accounting_group_user
+                             ,"accounting_group="+accounting_group
+                             ,"request_disk            = 64M"])
 
-            os.system('nohup sh '+path+'/auto_gen_redo.sh > '+path+'/auto_gen.out &')
+        repeat_final_job.add_parents(repeat_job_list)
+        
+        repeat_dagman.build_submit()
             
 
     if merging_flag==True:
         
         setNames=[]
         setIDs=[]
         setSizes=[]
@@ -1857,8 +2070,7 @@
             _=DataSet.fusion(fusionNames, sizes = sizes, save = path+finalName+str(sum(sizes)))
 
         # Deleting unnescesary file in the folder
         for file in dirlist(path):
             if (('.out' in file) or ('.py' in file)
                 or ('part_of' in file) or ('.sh' in file)):
                 os.system('rm '+path+file)
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mly-0.1.1/mly/mlTools.py` & `mly-0.3.1/mly/mlTools.py`

 * *Files identical despite different names*

### Comparing `mly-0.1.1/mly/models.py` & `mly-0.3.1/mly/models.py`

 * *Files identical despite different names*

### Comparing `mly-0.1.1/mly/simulateddetectornoise.py` & `mly-0.3.1/mly/simulateddetectornoise.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 # There are 3 modes for this function.
 # a) Simulated noise from the detector curves without any complexity          DET=SDR string
 # b) Simulated noise as a purtubation of a real noise PSD (sudo-real noise)   DET=[freq, PSD]
 # c) Simulated noise following a psd that could be anything                   DET=[PSD] size: T*fs/2
 
 
-def simulateddetectornoise(DET,T,fs,fmin,fmax):#,seed):
+def simulateddetectornoise(DET,T,fs,fmin,fmax,PSDm=1,PSDc=0):#,seed):
     
     #DET: Can be a string vector, a PSD vector of size T*fs/2 or
     #     it can be a size two array with frequencies and values of a PSD (sudodetectornoize)
 
     #% ---- Checks.
     ###narginchk(5,6);
     if (T>0 and fs>0 and fmin>0 and fmax>0)!=True :
@@ -175,15 +175,15 @@
         elif f[i]>fmax or f[i]>fstop[1]:
             k_p.append(i)
         else:
             f_w.append(f[i])
 
     f_w=np.array(f_w)
 
-    PSD=PSD_int(f_w)/2
+    PSD=((PSDm*np.sqrt(PSD_int(f_w))+PSDc)**2)/2
 
     PSD_frondtail=[]
     if len(k_m)>0:
         for i in range(0,len(k_m)):
             PSD_frondtail.append(PSD[0]*(f[k_m[i]]/f[k_m[-1]])**2)
         PSD=np.hstack((np.array(PSD_frondtail),PSD))
```

### Comparing `mly-0.1.1/setup.py` & `mly-0.3.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mly",
-    version="0.1.1",
+    version="0.3.1",
     author="Vasileios Skliris",
     author_email='vas.skliris@gmail.com',
     description='This tool helps you create training and testing data for ML to use for gravitational wave detection.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://pypi.python.org/pypi/mly/',
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "gwpy >= 0.13.1",
-        "Keras >= 2.2.4",
-        "tensorflow >= 1.12.0",
-        "numpy >= 1.16.1",
-        "sklearn"
+        "tensorflow >= 2.6",
+        "numpy",
+        "scikit-learn",
+        "pandas",
+        "pytest",
+        "pycondor",
+        "pycbc"
     ]
 )
```

