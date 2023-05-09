# Comparing `tmp/vChatGPT-1.0.tar.gz` & `tmp/vChatGPT-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vChatGPT-1.0.tar", last modified: Sun Mar 26 05:44:49 2023, max compression
+gzip compressed data, was "vChatGPT-1.1.tar", last modified: Tue May  9 02:47:14 2023, max compression
```

## Comparing `vChatGPT-1.0.tar` & `vChatGPT-1.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-03-26 05:44:49.070795 vChatGPT-1.0/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1101 2023-03-26 05:44:49.070795 vChatGPT-1.0/PKG-INFO
--rw-rw-r--   0 ywatanabe  (1000) ywatanabe  (1000)      504 2023-03-26 05:17:16.000000 vChatGPT-1.0/README.md
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       38 2023-03-26 05:44:49.070795 vChatGPT-1.0/setup.cfg
--rwxrwxr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2460 2023-03-26 04:16:50.000000 vChatGPT-1.0/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-03-26 05:44:49.060795 vChatGPT-1.0/src/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-03-26 05:44:49.060795 vChatGPT-1.0/src/vChatGPT/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      317 2023-03-26 05:44:26.000000 vChatGPT-1.0/src/vChatGPT/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      142 2023-03-25 17:24:38.000000 vChatGPT-1.0/src/vChatGPT/__main__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-03-26 05:44:49.060795 vChatGPT-1.0/src/vChatGPT/data/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)   186756 2022-06-11 00:50:23.000000 vChatGPT-1.0/src/vChatGPT/data/buzzer.wav
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-03-26 05:44:49.070795 vChatGPT-1.0/src/vChatGPT/scripts/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      119 2023-03-25 16:57:33.000000 vChatGPT-1.0/src/vChatGPT/scripts/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4371 2023-03-26 05:28:55.000000 vChatGPT-1.0/src/vChatGPT/scripts/audio.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1160 2023-03-26 05:39:40.000000 vChatGPT-1.0/src/vChatGPT/scripts/main.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3481 2023-03-26 05:36:41.000000 vChatGPT-1.0/src/vChatGPT/scripts/ml.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      448 2023-03-24 01:17:53.000000 vChatGPT-1.0/src/vChatGPT/scripts/utils.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-03-26 05:44:49.060795 vChatGPT-1.0/src/vChatGPT.egg-info/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1101 2023-03-26 05:44:48.000000 vChatGPT-1.0/src/vChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      425 2023-03-26 05:44:48.000000 vChatGPT-1.0/src/vChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2023-03-26 05:44:48.000000 vChatGPT-1.0/src/vChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       75 2023-03-26 05:44:48.000000 vChatGPT-1.0/src/vChatGPT.egg-info/requires.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        9 2023-03-26 05:44:48.000000 vChatGPT-1.0/src/vChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-05-09 02:47:14.273123 vChatGPT-1.1/
+-rw-rw-r--   0 ywatanabe  (1000) ywatanabe  (1000)    35149 2021-09-25 06:22:17.000000 vChatGPT-1.1/LICENSE
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      838 2023-05-09 02:47:14.273123 vChatGPT-1.1/PKG-INFO
+-rw-rw-r--   0 ywatanabe  (1000) ywatanabe  (1000)      394 2023-03-26 05:50:27.000000 vChatGPT-1.1/README.md
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       38 2023-05-09 02:47:14.273123 vChatGPT-1.1/setup.cfg
+-rwxrwxr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2460 2023-03-26 04:16:50.000000 vChatGPT-1.1/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-05-09 02:47:14.273123 vChatGPT-1.1/src/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-05-09 02:47:14.273123 vChatGPT-1.1/src/vChatGPT/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      317 2023-05-09 02:47:06.000000 vChatGPT-1.1/src/vChatGPT/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1181 2023-05-06 07:53:04.000000 vChatGPT-1.1/src/vChatGPT/__main__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-05-09 02:47:14.273123 vChatGPT-1.1/src/vChatGPT/data/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)   186756 2022-06-11 00:50:23.000000 vChatGPT-1.1/src/vChatGPT/data/buzzer.wav
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-05-09 02:47:14.273123 vChatGPT-1.1/src/vChatGPT/scripts/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      119 2023-03-25 16:57:33.000000 vChatGPT-1.1/src/vChatGPT/scripts/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4371 2023-03-26 07:05:19.000000 vChatGPT-1.1/src/vChatGPT/scripts/audio.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1181 2023-05-06 07:53:04.000000 vChatGPT-1.1/src/vChatGPT/scripts/main.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3565 2023-05-07 02:31:30.000000 vChatGPT-1.1/src/vChatGPT/scripts/ml.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      448 2023-03-24 01:17:53.000000 vChatGPT-1.1/src/vChatGPT/scripts/utils.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-05-09 02:47:14.273123 vChatGPT-1.1/src/vChatGPT.egg-info/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      838 2023-05-09 02:47:14.000000 vChatGPT-1.1/src/vChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      433 2023-05-09 02:47:14.000000 vChatGPT-1.1/src/vChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2023-05-09 02:47:14.000000 vChatGPT-1.1/src/vChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       75 2023-05-09 02:47:14.000000 vChatGPT-1.1/src/vChatGPT.egg-info/requires.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        9 2023-05-09 02:47:14.000000 vChatGPT-1.1/src/vChatGPT.egg-info/top_level.txt
```

### Comparing `vChatGPT-1.0/PKG-INFO` & `vChatGPT-1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: vChatGPT
-Version: 1.0
+Version: 1.1
 Summary: Verbal ChatGPT
 Home-page: https://github.com/ywatanabe1989/vChatGPT
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: GPL3.0
-Description: #### vChatGPT
-        You can talk to and listen to ChatGPT.
-        
-        #### Demo screenshot
-         Input: Your voice through a microphone  
-        Output: Speech reaction of ChatGPT from speakers as well as text  
-        ![alt text](https://github.com/ywatanabe1989/vChatGPT/blob/main/docs/vChatGPT_demo.png?raw=true)
-        
-        #### Installation
-        ``` bash
-        $ pip install vChatGPT
-        ```
-        
-        #### How to run vChatGPT
-        ``` bash
-        $ export OPENAI_API_KEY="52-DIGIT-YOUR_API_KEY" # Available on https://platform.openai.com/account/api-keys
-        $ python -m vChatGPT
-        ```
-        
 Keywords: verbal ChatGPT,AI language model,learning English
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+#### vChatGPT
+You can talk to and listen to ChatGPT.
+
+#### Screenshot
+![alt text](https://github.com/ywatanabe1989/vChatGPT/blob/main/docs/vChatGPT_demo_new.png?raw=true)
+
+#### Installation
+``` bash
+$ pip install vChatGPT
+```
+
+#### How to run vChatGPT
+``` bash
+$ export OPENAI_API_KEY="52-DIGIT-YOUR_API_KEY" # Available on https://platform.openai.com/account/api-keys
+$ python -m vChatGPT
+```
```

### Comparing `vChatGPT-1.0/setup.py` & `vChatGPT-1.1/setup.py`

 * *Files identical despite different names*

### Comparing `vChatGPT-1.0/src/vChatGPT/data/buzzer.wav` & `vChatGPT-1.1/src/vChatGPT/data/buzzer.wav`

 * *Files identical despite different names*

### Comparing `vChatGPT-1.0/src/vChatGPT/scripts/audio.py` & `vChatGPT-1.1/src/vChatGPT/scripts/audio.py`

 * *Files identical despite different names*

### Comparing `vChatGPT-1.0/src/vChatGPT/scripts/main.py` & `vChatGPT-1.1/src/vChatGPT/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2023-03-26 14:39:40 (ywatanabe)"
+# Time-stamp: "2023-05-06 16:53:04 (ywatanabe)"
 
 import os
 import time
 
 from vChatGPT.scripts import audio, ml, utils
 
 
@@ -22,24 +22,26 @@
 
     # Speech to text
     # if "mywhisper" not in globals():
     #     mywhisper = utils.Whisper()
     # said = mywhisper(spath_in_wav)
     said = ml.s2t_unpaid(spath_in_wav, language="EN")
     print(said)
-
+    print()
+    
     # Text to text (using ChatGPT)
     # gpt_out = ml.t2t_chatGPT(said)
     gpt_out = chatgpt(said)
     print(gpt_out)
     print()
 
     # Text to speech
     spath_out_mp3 = f"/tmp/vChatGPT/output-{ID}.mp3"
     ml.t2s(gpt_out, spath=spath_out_mp3, print_save=False)
+    
 
     # Plays the ChatGPT's output
     audio.play_audio_file(spath_out_mp3)
 
 
 def main():
     chatgpt = ml.ChatGPT()
```

### Comparing `vChatGPT-1.0/src/vChatGPT/scripts/ml.py` & `vChatGPT-1.1/src/vChatGPT/scripts/ml.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2023-03-26 14:36:41 (ywatanabe)"
+# Time-stamp: "2023-05-07 11:31:30 (ywatanabe)"
 import os
 import warnings
 
 import openai
 import speech_recognition as sr
 
 # import whisper
@@ -34,15 +34,15 @@
         print(e)
 
 
 class ChatGPT(object):
     def __init__(
         self,
         system_setting="Please answer in a conversational manner as if you are my friend. "
-        "I would be grateful if your response would be less than 20 words.",
+        "I would be grateful if your response would be less than 20 words. By the way, I am preparing for the IELTS exam. So, please use idioms when possible.",
     ):
         self.counter = 0
         self.OPENAI_API_KEY = os.getenv("OPENAI_API_KEY")
         openai.api_key = self.OPENAI_API_KEY
 
         if self.OPENAI_API_KEY is None:
             print('\n"OPENAI_API_KEY" is not set as an environmental varible.\n')
```

### Comparing `vChatGPT-1.0/src/vChatGPT.egg-info/PKG-INFO` & `vChatGPT-1.1/src/vChatGPT.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: vChatGPT
-Version: 1.0
+Version: 1.1
 Summary: Verbal ChatGPT
 Home-page: https://github.com/ywatanabe1989/vChatGPT
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: GPL3.0
-Description: #### vChatGPT
-        You can talk to and listen to ChatGPT.
-        
-        #### Demo screenshot
-         Input: Your voice through a microphone  
-        Output: Speech reaction of ChatGPT from speakers as well as text  
-        ![alt text](https://github.com/ywatanabe1989/vChatGPT/blob/main/docs/vChatGPT_demo.png?raw=true)
-        
-        #### Installation
-        ``` bash
-        $ pip install vChatGPT
-        ```
-        
-        #### How to run vChatGPT
-        ``` bash
-        $ export OPENAI_API_KEY="52-DIGIT-YOUR_API_KEY" # Available on https://platform.openai.com/account/api-keys
-        $ python -m vChatGPT
-        ```
-        
 Keywords: verbal ChatGPT,AI language model,learning English
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+#### vChatGPT
+You can talk to and listen to ChatGPT.
+
+#### Screenshot
+![alt text](https://github.com/ywatanabe1989/vChatGPT/blob/main/docs/vChatGPT_demo_new.png?raw=true)
+
+#### Installation
+``` bash
+$ pip install vChatGPT
+```
+
+#### How to run vChatGPT
+``` bash
+$ export OPENAI_API_KEY="52-DIGIT-YOUR_API_KEY" # Available on https://platform.openai.com/account/api-keys
+$ python -m vChatGPT
+```
```

