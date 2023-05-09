# Comparing `tmp/wyoming_faster_whisper-0.0.1.tar.gz` & `tmp/wyoming_faster_whisper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyoming_faster_whisper-0.0.1.tar", last modified: Wed Apr 19 16:30:31 2023, max compression
+gzip compressed data, was "wyoming_faster_whisper-0.0.2.tar", last modified: Tue May  9 19:41:26 2023, max compression
```

## Comparing `wyoming_faster_whisper-0.0.1.tar` & `wyoming_faster_whisper-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-19 16:30:31.424368 wyoming_faster_whisper-0.0.1/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-04-19 16:16:21.000000 wyoming_faster_whisper-0.0.1/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-04-19 16:30:31.424368 wyoming_faster_whisper-0.0.1/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       55 2023-04-19 16:19:47.000000 wyoming_faster_whisper-0.0.1/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-04-19 16:30:31.424368 wyoming_faster_whisper-0.0.1/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1225 2023-04-19 15:11:12.000000 wyoming_faster_whisper-0.0.1/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-19 16:30:31.424368 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       41 2023-04-19 15:27:06.000000 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/__init__.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     3762 2023-04-19 16:29:49.000000 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-19 15:13:49.000000 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/const.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     1608 2023-04-19 15:47:33.000000 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/download.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-19 16:30:31.424368 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/faster_whisper/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       37 2023-04-19 15:35:16.000000 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/faster_whisper/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5809 2023-02-11 21:34:47.000000 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/faster_whisper/feature_extractor.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12038 2023-04-19 16:21:20.000000 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/faster_whisper/transcribe.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2199 2023-04-19 16:29:11.000000 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/handler.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-19 16:30:31.424368 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-04-19 16:30:31.000000 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-04-19 16:30:31.000000 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-19 16:30:31.000000 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       54 2023-04-19 16:30:31.000000 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-04-19 16:30:31.000000 wyoming_faster_whisper-0.0.1/wyoming_faster_whisper.egg-info/top_level.txt
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-09 19:41:26.123894 wyoming_faster_whisper-0.0.2/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-05-09 19:41:26.123894 wyoming_faster_whisper-0.0.2/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       55 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-05-09 19:41:26.123894 wyoming_faster_whisper-0.0.2/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1225 2023-05-03 14:29:10.000000 wyoming_faster_whisper-0.0.2/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-09 19:41:26.123894 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       41 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/__init__.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     3837 2023-05-03 17:15:52.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/const.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4593 2023-05-09 19:37:24.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/download.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-09 19:41:26.123894 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/faster_whisper/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       37 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/faster_whisper/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5809 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/faster_whisper/feature_extractor.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12038 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/faster_whisper/transcribe.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-09 19:37:36.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/file_hash.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2199 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/handler.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-09 19:41:26.123894 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-05-09 19:41:26.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      634 2023-05-09 19:41:26.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-09 19:41:26.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       54 2023-05-09 19:41:26.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-05-09 19:41:26.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/top_level.txt
```

### Comparing `wyoming_faster_whisper-0.0.1/PKG-INFO` & `wyoming_faster_whisper-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wyoming_faster_whisper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wyoming Server for Faster Whisper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Keywords: rhasspy wyoming whisper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `wyoming_faster_whisper-0.0.1/setup.py` & `wyoming_faster_whisper-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     with open(requirements_path, "r", encoding="utf-8") as requirements_file:
         requirements = requirements_file.read().splitlines()
 
 # -----------------------------------------------------------------------------
 
 setup(
     name="wyoming_faster_whisper",
-    version="0.0.1",
+    version="0.0.2",
     description="Wyoming Server for Faster Whisper",
     url="http://github.com/rhasspy/rhasspy3",
     author="Michael Hansen",
     author_email="mike@rhasspy.org",
     license="MIT",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

### Comparing `wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/__main__.py` & `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
     if model_dir is None:
         _LOGGER.info("Downloading %s to %s", model, args.download_dir)
         model_dir = download_model(model, args.download_dir)
 
     if args.language and (args.language != "auto"):
         _LOGGER.debug("Language: %s", args.language)
         languages = [args.language]
+
+        # Whisper does not understand "auto"
+        args.language = None
     else:
         languages = WHISPER_LANGUAGES
 
     wyoming_info = Info(
         asr=[
             AsrProgram(
                 name="faster-whisper",
```

### Comparing `wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/const.py` & `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/const.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/faster_whisper/feature_extractor.py` & `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/faster_whisper/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/faster_whisper/transcribe.py` & `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/faster_whisper/transcribe.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.1/wyoming_faster_whisper/handler.py` & `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Event handler for clients of the server."""
-import asyncio
 import argparse
+import asyncio
 import logging
 
 from wyoming.asr import Transcript
-from wyoming.audio import AudioChunk, AudioStop, AudioChunkConverter
+from wyoming.audio import AudioChunk, AudioChunkConverter, AudioStop
 from wyoming.event import Event
 from wyoming.info import Describe, Info
 from wyoming.server import AsyncEventHandler
 
 from .faster_whisper import WhisperModel
 
 _LOGGER = logging.getLogger(__name__)
```

### Comparing `wyoming_faster_whisper-0.0.1/wyoming_faster_whisper.egg-info/PKG-INFO` & `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wyoming-faster-whisper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wyoming Server for Faster Whisper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Keywords: rhasspy wyoming whisper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `wyoming_faster_whisper-0.0.1/wyoming_faster_whisper.egg-info/SOURCES.txt` & `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 requirements.txt
 setup.py
 wyoming_faster_whisper/__init__.py
 wyoming_faster_whisper/__main__.py
 wyoming_faster_whisper/const.py
 wyoming_faster_whisper/download.py
+wyoming_faster_whisper/file_hash.py
 wyoming_faster_whisper/handler.py
 wyoming_faster_whisper.egg-info/PKG-INFO
 wyoming_faster_whisper.egg-info/SOURCES.txt
 wyoming_faster_whisper.egg-info/dependency_links.txt
 wyoming_faster_whisper.egg-info/requires.txt
 wyoming_faster_whisper.egg-info/top_level.txt
 wyoming_faster_whisper/faster_whisper/__init__.py
```

