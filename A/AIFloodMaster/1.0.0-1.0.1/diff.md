# Comparing `tmp/AIFloodMaster-1.0.0.tar.gz` & `tmp/AIFloodMaster-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIFloodMaster-1.0.0.tar", last modified: Tue May  9 06:53:35 2023, max compression
+gzip compressed data, was "AIFloodMaster-1.0.1.tar", last modified: Tue May  9 07:24:48 2023, max compression
```

## Comparing `AIFloodMaster-1.0.0.tar` & `AIFloodMaster-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:35.537767 AIFloodMaster-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:35.508514 AIFloodMaster-1.0.0/AIFloodMaster.egg-info/
--rw-rw-rw-   0        0        0      250 2023-05-09 06:53:35.000000 AIFloodMaster-1.0.0/AIFloodMaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      648 2023-05-09 06:53:35.000000 AIFloodMaster-1.0.0/AIFloodMaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 06:53:35.000000 AIFloodMaster-1.0.0/AIFloodMaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-09 06:53:35.000000 AIFloodMaster-1.0.0/AIFloodMaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      250 2023-05-09 06:53:35.537767 AIFloodMaster-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1985 2023-05-09 02:32:15.000000 AIFloodMaster-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:35.509443 AIFloodMaster-1.0.0/cores/
--rw-rw-rw-   0        0        0        0 2023-05-09 06:49:01.000000 AIFloodMaster-1.0.0/cores/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:35.519540 AIFloodMaster-1.0.0/cores/controllers/
--rw-rw-rw-   0        0        0        0 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/controllers/__init__.py
--rw-rw-rw-   0        0        0     7443 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/controllers/agent.py
--rw-rw-rw-   0        0        0     1854 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/controllers/controller.py
--rw-rw-rw-   0        0        0     4346 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/controllers/env.py
--rw-rw-rw-   0        0        0     4044 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/controllers/processor.py
--rw-rw-rw-   0        0        0     1095 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/controllers/space.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:35.520907 AIFloodMaster-1.0.0/cores/delegators/
--rw-rw-rw-   0        0        0        0 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/delegators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:35.523568 AIFloodMaster-1.0.0/cores/forecasters/
--rw-rw-rw-   0        0        0    23179 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/forecasters/LstmPredictor.py
--rw-rw-rw-   0        0        0      262 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/forecasters/__init__.py
--rw-rw-rw-   0        0        0     3271 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/forecasters/predictor.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:35.535891 AIFloodMaster-1.0.0/cores/utils/
--rw-rw-rw-   0        0        0    17852 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/utils/CategoryEncoder.py
--rw-rw-rw-   0        0        0      164 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/utils/DataAnalyzer.py
--rw-rw-rw-   0        0        0     8739 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/utils/DataLoader.py
--rw-rw-rw-   0        0        0    10997 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/utils/DataPreprocessor.py
--rw-rw-rw-   0        0        0     5210 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/utils/DataScaler.py
--rw-rw-rw-   0        0        0      387 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.0/cores/utils/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-09 06:53:35.537767 AIFloodMaster-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-05-09 06:51:46.000000 AIFloodMaster-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:24:48.892106 AIFloodMaster-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-09 07:24:48.864019 AIFloodMaster-1.0.1/AIFloodMaster.egg-info/
+-rw-rw-rw-   0        0        0      250 2023-05-09 07:24:48.000000 AIFloodMaster-1.0.1/AIFloodMaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2023-05-09 07:24:48.000000 AIFloodMaster-1.0.1/AIFloodMaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 07:24:48.000000 AIFloodMaster-1.0.1/AIFloodMaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-09 07:24:48.000000 AIFloodMaster-1.0.1/AIFloodMaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      250 2023-05-09 07:24:48.892106 AIFloodMaster-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1985 2023-05-09 02:32:15.000000 AIFloodMaster-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 07:24:48.865012 AIFloodMaster-1.0.1/cores/
+-rw-rw-rw-   0        0        0        0 2023-05-09 06:49:01.000000 AIFloodMaster-1.0.1/cores/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:24:48.876314 AIFloodMaster-1.0.1/cores/controllers/
+-rw-rw-rw-   0        0        0        0 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/controllers/__init__.py
+-rw-rw-rw-   0        0        0     7443 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/controllers/agent.py
+-rw-rw-rw-   0        0        0     1854 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/controllers/controller.py
+-rw-rw-rw-   0        0        0     4346 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/controllers/env.py
+-rw-rw-rw-   0        0        0     4044 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/controllers/processor.py
+-rw-rw-rw-   0        0        0     1095 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/controllers/space.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:24:48.878086 AIFloodMaster-1.0.1/cores/delegators/
+-rw-rw-rw-   0        0        0        0 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/delegators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:24:48.880334 AIFloodMaster-1.0.1/cores/forecasters/
+-rw-rw-rw-   0        0        0    23179 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/forecasters/LstmPredictor.py
+-rw-rw-rw-   0        0        0      262 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/forecasters/__init__.py
+-rw-rw-rw-   0        0        0     3271 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/forecasters/predictor.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:24:48.891449 AIFloodMaster-1.0.1/cores/utils/
+-rw-rw-rw-   0        0        0    17852 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/utils/CategoryEncoder.py
+-rw-rw-rw-   0        0        0      164 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/utils/DataAnalyzer.py
+-rw-rw-rw-   0        0        0     8739 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/utils/DataLoader.py
+-rw-rw-rw-   0        0        0    10997 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/utils/DataPreprocessor.py
+-rw-rw-rw-   0        0        0     5210 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/utils/DataScaler.py
+-rw-rw-rw-   0        0        0      387 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.1/cores/utils/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-09 07:24:48.893132 AIFloodMaster-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      818 2023-05-09 06:51:46.000000 AIFloodMaster-1.0.1/setup.py
```

### Comparing `AIFloodMaster-1.0.0/AIFloodMaster.egg-info/SOURCES.txt` & `AIFloodMaster-1.0.1/AIFloodMaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.0/README.md` & `AIFloodMaster-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.0/cores/controllers/agent.py` & `AIFloodMaster-1.0.1/cores/controllers/agent.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.0/cores/controllers/controller.py` & `AIFloodMaster-1.0.1/cores/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.0/cores/controllers/env.py` & `AIFloodMaster-1.0.1/cores/controllers/env.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.0/cores/controllers/processor.py` & `AIFloodMaster-1.0.1/cores/controllers/processor.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.0/cores/controllers/space.py` & `AIFloodMaster-1.0.1/cores/controllers/space.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.0/cores/forecasters/LstmPredictor.py` & `AIFloodMaster-1.0.1/cores/forecasters/LstmPredictor.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.0/cores/forecasters/predictor.py` & `AIFloodMaster-1.0.1/cores/forecasters/predictor.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.0/cores/utils/CategoryEncoder.py` & `AIFloodMaster-1.0.1/cores/utils/CategoryEncoder.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.0/cores/utils/DataLoader.py` & `AIFloodMaster-1.0.1/cores/utils/DataLoader.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.0/cores/utils/DataPreprocessor.py` & `AIFloodMaster-1.0.1/cores/utils/DataPreprocessor.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.0/cores/utils/DataScaler.py` & `AIFloodMaster-1.0.1/cores/utils/DataScaler.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.0/setup.py` & `AIFloodMaster-1.0.1/setup.py`

 * *Files identical despite different names*

