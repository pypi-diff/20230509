# Comparing `tmp/audiostack-0.0.5.tar.gz` & `tmp/audiostack-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostack-0.0.5.tar", last modified: Mon Apr 17 07:57:04 2023, max compression
+gzip compressed data, was "audiostack-0.0.6.tar", last modified: Tue May  9 08:44:14 2023, max compression
```

## Comparing `audiostack-0.0.5.tar` & `audiostack-0.0.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.080026 audiostack-0.0.5/
--rw-r--r--   0 hackerman   (501) staff       (20)    33108 2023-04-17 07:57:04.079543 audiostack-0.0.5/PKG-INFO
--rw-r--r--   0 hackerman   (501) staff       (20)    26796 2022-12-13 14:01:40.000000 audiostack-0.0.5/README.md
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.069086 audiostack-0.0.5/audiostack/
--rw-r--r--   0 hackerman   (501) staff       (20)      555 2023-04-17 07:56:01.000000 audiostack-0.0.5/audiostack/__init__.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.071102 audiostack-0.0.5/audiostack/content/
--rw-r--r--   0 hackerman   (501) staff       (20)      459 2023-03-16 15:15:23.000000 audiostack-0.0.5/audiostack/content/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     2270 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/content/media.py
--rw-r--r--   0 hackerman   (501) staff       (20)      947 2023-03-16 15:15:23.000000 audiostack-0.0.5/audiostack/content/root_functions.py
--rw-r--r--   0 hackerman   (501) staff       (20)     3528 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/content/script.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.072118 audiostack-0.0.5/audiostack/delivery/
--rw-r--r--   0 hackerman   (501) staff       (20)       48 2022-12-06 15:30:00.000000 audiostack-0.0.5/audiostack/delivery/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     1902 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/delivery/encoder.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.072863 audiostack-0.0.5/audiostack/docs/
--rw-r--r--   0 hackerman   (501) staff       (20)       47 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/docs/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)      631 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/docs/docs.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.074939 audiostack-0.0.5/audiostack/helpers/
--rw-r--r--   0 hackerman   (501) staff       (20)        0 2022-12-06 15:30:00.000000 audiostack-0.0.5/audiostack/helpers/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)      716 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/helpers/api_item.py
--rw-r--r--   0 hackerman   (501) staff       (20)      811 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/helpers/api_list.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4301 2023-04-17 07:54:26.000000 audiostack-0.0.5/audiostack/helpers/request_interface.py
--rw-r--r--   0 hackerman   (501) staff       (20)      163 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/helpers/request_types.py
--rw-r--r--   0 hackerman   (501) staff       (20)      338 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/helpers/response.py
--rw-r--r--   0 hackerman   (501) staff       (20)      227 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/helpers/util.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.075194 audiostack-0.0.5/audiostack/orchestrator/
--rw-r--r--   0 hackerman   (501) staff       (20)       58 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/orchestrator/__init__.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.076032 audiostack-0.0.5/audiostack/production/
--rw-r--r--   0 hackerman   (501) staff       (20)       88 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/production/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4138 2023-03-16 15:15:23.000000 audiostack-0.0.5/audiostack/production/mix.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4349 2023-04-17 07:55:11.000000 audiostack-0.0.5/audiostack/production/sound.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.077852 audiostack-0.0.5/audiostack/speech/
--rw-r--r--   0 hackerman   (501) staff       (20)      126 2022-12-08 09:57:07.000000 audiostack-0.0.5/audiostack/speech/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     2979 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/speech/diction.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4502 2023-03-16 15:15:23.000000 audiostack-0.0.5/audiostack/speech/tts.py
--rw-r--r--   0 hackerman   (501) staff       (20)     1215 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/speech/voice.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.069855 audiostack-0.0.5/audiostack.egg-info/
--rw-r--r--   0 hackerman   (501) staff       (20)    33108 2023-04-17 07:57:04.000000 audiostack-0.0.5/audiostack.egg-info/PKG-INFO
--rw-r--r--   0 hackerman   (501) staff       (20)      959 2023-04-17 07:57:04.000000 audiostack-0.0.5/audiostack.egg-info/SOURCES.txt
--rw-r--r--   0 hackerman   (501) staff       (20)        1 2023-04-17 07:57:04.000000 audiostack-0.0.5/audiostack.egg-info/dependency_links.txt
--rw-r--r--   0 hackerman   (501) staff       (20)       45 2023-04-17 07:57:04.000000 audiostack-0.0.5/audiostack.egg-info/requires.txt
--rw-r--r--   0 hackerman   (501) staff       (20)       17 2023-04-17 07:57:04.000000 audiostack-0.0.5/audiostack.egg-info/top_level.txt
--rw-r--r--   0 hackerman   (501) staff       (20)       38 2023-04-17 07:57:04.080136 audiostack-0.0.5/setup.cfg
--rw-r--r--   0 hackerman   (501) staff       (20)     1039 2023-02-20 16:12:26.000000 audiostack-0.0.5/setup.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.078871 audiostack-0.0.5/tests/
--rw-r--r--   0 hackerman   (501) staff       (20)      173 2023-02-20 16:03:10.000000 audiostack-0.0.5/tests/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)      659 2023-02-20 16:41:55.000000 audiostack-0.0.5/tests/test_audience.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.902231 audiostack-0.0.6/
+-rw-r--r--   0 hackerman   (501) staff       (20)    33108 2023-05-09 08:44:14.902039 audiostack-0.0.6/PKG-INFO
+-rw-r--r--   0 hackerman   (501) staff       (20)    26796 2022-12-13 14:01:40.000000 audiostack-0.0.6/README.md
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.891264 audiostack-0.0.6/audiostack/
+-rw-r--r--   0 hackerman   (501) staff       (20)      555 2023-05-09 08:43:52.000000 audiostack-0.0.6/audiostack/__init__.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.893330 audiostack-0.0.6/audiostack/content/
+-rw-r--r--   0 hackerman   (501) staff       (20)      459 2023-03-16 15:15:23.000000 audiostack-0.0.6/audiostack/content/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     2270 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/content/media.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      947 2023-03-16 15:15:23.000000 audiostack-0.0.6/audiostack/content/root_functions.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     3528 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/content/script.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.894326 audiostack-0.0.6/audiostack/delivery/
+-rw-r--r--   0 hackerman   (501) staff       (20)       48 2022-12-06 15:30:00.000000 audiostack-0.0.6/audiostack/delivery/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     2313 2023-05-04 12:16:31.000000 audiostack-0.0.6/audiostack/delivery/encoder.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.894909 audiostack-0.0.6/audiostack/docs/
+-rw-r--r--   0 hackerman   (501) staff       (20)       47 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/docs/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      631 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/docs/docs.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.896962 audiostack-0.0.6/audiostack/helpers/
+-rw-r--r--   0 hackerman   (501) staff       (20)        0 2022-12-06 15:30:00.000000 audiostack-0.0.6/audiostack/helpers/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      716 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/helpers/api_item.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      811 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/helpers/api_list.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     4301 2023-04-17 07:54:26.000000 audiostack-0.0.6/audiostack/helpers/request_interface.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      163 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/helpers/request_types.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      338 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/helpers/response.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      227 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/helpers/util.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.897112 audiostack-0.0.6/audiostack/orchestrator/
+-rw-r--r--   0 hackerman   (501) staff       (20)       58 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/orchestrator/__init__.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.898721 audiostack-0.0.6/audiostack/production/
+-rw-r--r--   0 hackerman   (501) staff       (20)       88 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/production/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     3821 2023-05-04 12:16:01.000000 audiostack-0.0.6/audiostack/production/mix.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     4349 2023-04-17 07:55:11.000000 audiostack-0.0.6/audiostack/production/sound.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.900001 audiostack-0.0.6/audiostack/speech/
+-rw-r--r--   0 hackerman   (501) staff       (20)      126 2022-12-08 09:57:07.000000 audiostack-0.0.6/audiostack/speech/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     2979 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/speech/diction.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     4502 2023-03-16 15:15:23.000000 audiostack-0.0.6/audiostack/speech/tts.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     1215 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/speech/voice.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.892015 audiostack-0.0.6/audiostack.egg-info/
+-rw-r--r--   0 hackerman   (501) staff       (20)    33108 2023-05-09 08:44:14.000000 audiostack-0.0.6/audiostack.egg-info/PKG-INFO
+-rw-r--r--   0 hackerman   (501) staff       (20)      959 2023-05-09 08:44:14.000000 audiostack-0.0.6/audiostack.egg-info/SOURCES.txt
+-rw-r--r--   0 hackerman   (501) staff       (20)        1 2023-05-09 08:44:14.000000 audiostack-0.0.6/audiostack.egg-info/dependency_links.txt
+-rw-r--r--   0 hackerman   (501) staff       (20)       45 2023-05-09 08:44:14.000000 audiostack-0.0.6/audiostack.egg-info/requires.txt
+-rw-r--r--   0 hackerman   (501) staff       (20)       17 2023-05-09 08:44:14.000000 audiostack-0.0.6/audiostack.egg-info/top_level.txt
+-rw-r--r--   0 hackerman   (501) staff       (20)       38 2023-05-09 08:44:14.902292 audiostack-0.0.6/setup.cfg
+-rw-r--r--   0 hackerman   (501) staff       (20)     1039 2023-02-20 16:12:26.000000 audiostack-0.0.6/setup.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.901377 audiostack-0.0.6/tests/
+-rw-r--r--   0 hackerman   (501) staff       (20)      173 2023-02-20 16:03:10.000000 audiostack-0.0.6/tests/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      659 2023-02-20 16:41:55.000000 audiostack-0.0.6/tests/test_audience.py
```

### Comparing `audiostack-0.0.5/PKG-INFO` & `audiostack-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: sam@aflorithmic.ai
 License: UNKNOWN
 Description: <p align="center">
         <a href="https://www.api.audio/" rel="noopener">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: audiostack Version: 0.0.5 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 0.0.6 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: sam@aflorithmic.ai License: UNKNOWN
 Description:
                                [api.audio_logo]
                       **** apiaudio - audiostack SDK ****
 ---
    audiostack is the official api.audio Python 3 SDK. This SDK provides easy
```

### Comparing `audiostack-0.0.5/README.md` & `audiostack-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/audiostack/content/media.py` & `audiostack-0.0.6/audiostack/content/media.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/audiostack/content/root_functions.py` & `audiostack-0.0.6/audiostack/content/root_functions.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/audiostack/content/script.py` & `audiostack-0.0.6/audiostack/content/script.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/audiostack/delivery/encoder.py` & `audiostack-0.0.6/audiostack/delivery/encoder.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,15 +18,22 @@
 
     @staticmethod
     def encode_mix(
         productionId: str = "",
         productionItem: object = None,
         preset: str = "",
         public: bool = False,
+        bitRateType: str = "",
+        bitRate: int = None,          
+        sampleRate: int = None,
+        format: str = "",
+        bitDepth: int = None,
+        channels: int = None,
     ) -> Item:
+        
         if productionId and productionItem:
             raise Exception(
                 "productionId or productionItem should be supplied not both"
             )
         if not (productionId or productionItem):
             raise Exception("productionId or productionItem should be supplied")
 
@@ -36,18 +43,23 @@
             except Exception:
                 raise Exception(
                     "supplied productionItem is missing an attribute, productionItem should be type object and a response from Production.Mix"
                 )
         elif productionId:
             if not isinstance(productionId, str):
                 raise Exception("supplied productionId should be a uuid string.")
-
+        
         body = {
             "productionId": productionId,
             "preset": preset,
             "public": public,
+            "bitRateType": bitRateType,
+            "bitRate": bitRate,
+            "sampleRate": sampleRate,
+            "format": format,
+            "bitDepth": bitDepth,
+            "channels": channels
         }
-
         r = Encoder.interface.send_request(
             rtype=RequestTypes.POST, route="encoder", json=body
         )
         return Encoder.Item(r)
```

### Comparing `audiostack-0.0.5/audiostack/docs/docs.py` & `audiostack-0.0.6/audiostack/docs/docs.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/audiostack/helpers/api_item.py` & `audiostack-0.0.6/audiostack/helpers/api_item.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/audiostack/helpers/api_list.py` & `audiostack-0.0.6/audiostack/helpers/api_list.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/audiostack/helpers/request_interface.py` & `audiostack-0.0.6/audiostack/helpers/request_interface.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/audiostack/production/mix.py` & `audiostack-0.0.6/audiostack/production/mix.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,47 +39,42 @@
                 raise Exception()
 
     @staticmethod
     def create(
         speechId="",
         speechItem=None,
         soundTemplate: str = "",
-        forceLength: float = 0.0,  # a value of 0 means no force length
         mediaFiles: dict = {},
+        fxFiles: dict = {},
         sectionProperties: dict = {},
+        timelineProperties: dict = {},
         masteringPreset: str = "",
-        acousticSpace: str = "",
-        callbackUrl: str = "",
         public: bool = False,
     ) -> Item:
         if speechId and speechItem:
             raise Exception("speechId or scriptItem should be supplied not both")
         if not (speechId or speechItem):
             raise Exception("speechId or scriptItem should be supplied")
         if speechItem:
             speechId = speechItem.speechId
 
         if not isinstance(soundTemplate, str):
             raise Exception("soundTemplate argument should be a string")
-        if not isinstance(forceLength, float):
-            raise Exception("forceLength should be a float")
         if not isinstance(masteringPreset, str):
             raise Exception("masteringPreset should be a string")
-        if not isinstance(acousticSpace, str):
-            raise Exception("acousticSpace should be a string")
+        
 
         body = {
             "speechId": speechId,
             "soundTemplate": soundTemplate,
-            "forceLength": forceLength,
             "mediaFiles": mediaFiles,
+            "fxFiles": fxFiles,
             "sectionProperties": sectionProperties,
+            "timelineProperties": timelineProperties,
             "masteringPreset": masteringPreset,
-            "acousticSpace": acousticSpace,
-            "callbackUrl": callbackUrl,
             "public": public,
         }
 
         r = Mix.interface.send_request(rtype=RequestTypes.POST, route="mix", json=body)
         if r["statusCode"] == 202:
             print("Response in progress please wait...")
             return Mix.get(Mix.Item(r).productionId)
```

### Comparing `audiostack-0.0.5/audiostack/production/sound.py` & `audiostack-0.0.6/audiostack/production/sound.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/audiostack/speech/diction.py` & `audiostack-0.0.6/audiostack/speech/diction.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/audiostack/speech/tts.py` & `audiostack-0.0.6/audiostack/speech/tts.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/audiostack/speech/voice.py` & `audiostack-0.0.6/audiostack/speech/voice.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/audiostack.egg-info/PKG-INFO` & `audiostack-0.0.6/audiostack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: sam@aflorithmic.ai
 License: UNKNOWN
 Description: <p align="center">
         <a href="https://www.api.audio/" rel="noopener">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: audiostack Version: 0.0.5 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 0.0.6 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: sam@aflorithmic.ai License: UNKNOWN
 Description:
                                [api.audio_logo]
                       **** apiaudio - audiostack SDK ****
 ---
    audiostack is the official api.audio Python 3 SDK. This SDK provides easy
```

### Comparing `audiostack-0.0.5/audiostack.egg-info/SOURCES.txt` & `audiostack-0.0.6/audiostack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/setup.py` & `audiostack-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.5/tests/test_audience.py` & `audiostack-0.0.6/tests/test_audience.py`

 * *Files identical despite different names*

