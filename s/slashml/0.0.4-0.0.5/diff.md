# Comparing `tmp/slashml-0.0.4.tar.gz` & `tmp/slashml-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/faizank/workspace/experiments/live_projects/slashml/sdk_tests/slashml/dist/.tmp-xe0cfgkz/slashml-0.0.4.tar", last modified: Mon May  8 22:24:05 2023, max compression
+gzip compressed data, was "/Users/faizank/workspace/experiments/live_projects/slashml/sdk_tests/slashml/dist/.tmp-o1v63c_a/slashml-0.0.5.tar", last modified: Mon May  8 22:45:10 2023, max compression
```

## Comparing `slashml-0.0.4.tar` & `slashml-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-08 22:24:05.805208 slashml-0.0.4/
--rw-r--r--   0 faizank    (501) staff       (20)     1064 2023-04-24 05:35:14.000000 slashml-0.0.4/LICENSE.txt
--rw-r--r--   0 faizank    (501) staff       (20)      279 2023-05-08 22:24:05.804988 slashml-0.0.4/PKG-INFO
--rw-r--r--   0 faizank    (501) staff       (20)     5520 2023-05-08 21:56:06.000000 slashml-0.0.4/README.md
--rw-r--r--   0 faizank    (501) staff       (20)       38 2023-05-08 22:24:05.805268 slashml-0.0.4/setup.cfg
--rw-r--r--   0 faizank    (501) staff       (20)      751 2023-05-08 22:23:56.000000 slashml-0.0.4/setup.py
-drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-08 22:24:05.803756 slashml-0.0.4/slashml/
--rw-r--r--   0 faizank    (501) staff       (20)      190 2023-05-08 20:59:11.000000 slashml-0.0.4/slashml/__init__.py
--rw-r--r--   0 faizank    (501) staff       (20)     1354 2023-05-08 22:21:28.000000 slashml-0.0.4/slashml/speech_to_text.py
--rw-r--r--   0 faizank    (501) staff       (20)      979 2023-05-08 22:21:12.000000 slashml-0.0.4/slashml/text_summarization.py
--rw-r--r--   0 faizank    (501) staff       (20)      956 2023-05-08 22:23:19.000000 slashml-0.0.4/slashml/text_to_speech.py
--rw-r--r--   0 faizank    (501) staff       (20)     1257 2023-05-08 22:20:49.000000 slashml-0.0.4/slashml/utils.py
-drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-08 22:24:05.804739 slashml-0.0.4/slashml.egg-info/
--rw-r--r--   0 faizank    (501) staff       (20)      279 2023-05-08 22:24:05.000000 slashml-0.0.4/slashml.egg-info/PKG-INFO
--rw-r--r--   0 faizank    (501) staff       (20)      313 2023-05-08 22:24:05.000000 slashml-0.0.4/slashml.egg-info/SOURCES.txt
--rw-r--r--   0 faizank    (501) staff       (20)        1 2023-05-08 22:24:05.000000 slashml-0.0.4/slashml.egg-info/dependency_links.txt
--rw-r--r--   0 faizank    (501) staff       (20)       31 2023-05-08 22:24:05.000000 slashml-0.0.4/slashml.egg-info/requires.txt
--rw-r--r--   0 faizank    (501) staff       (20)        8 2023-05-08 22:24:05.000000 slashml-0.0.4/slashml.egg-info/top_level.txt
+drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-08 22:45:10.277303 slashml-0.0.5/
+-rw-r--r--   0 faizank    (501) staff       (20)     1064 2023-04-24 05:35:14.000000 slashml-0.0.5/LICENSE.txt
+-rw-r--r--   0 faizank    (501) staff       (20)     6379 2023-05-08 22:45:10.277092 slashml-0.0.5/PKG-INFO
+-rw-r--r--   0 faizank    (501) staff       (20)     6059 2023-05-08 22:40:33.000000 slashml-0.0.5/README.md
+-rw-r--r--   0 faizank    (501) staff       (20)       38 2023-05-08 22:45:10.277362 slashml-0.0.5/setup.cfg
+-rw-r--r--   0 faizank    (501) staff       (20)     1022 2023-05-08 22:44:55.000000 slashml-0.0.5/setup.py
+drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-08 22:45:10.275987 slashml-0.0.5/slashml/
+-rw-r--r--   0 faizank    (501) staff       (20)      190 2023-05-08 20:59:11.000000 slashml-0.0.5/slashml/__init__.py
+-rw-r--r--   0 faizank    (501) staff       (20)     1354 2023-05-08 22:40:33.000000 slashml-0.0.5/slashml/speech_to_text.py
+-rw-r--r--   0 faizank    (501) staff       (20)      979 2023-05-08 22:40:33.000000 slashml-0.0.5/slashml/text_summarization.py
+-rw-r--r--   0 faizank    (501) staff       (20)      956 2023-05-08 22:40:33.000000 slashml-0.0.5/slashml/text_to_speech.py
+-rw-r--r--   0 faizank    (501) staff       (20)     1257 2023-05-08 22:40:33.000000 slashml-0.0.5/slashml/utils.py
+drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-08 22:45:10.276869 slashml-0.0.5/slashml.egg-info/
+-rw-r--r--   0 faizank    (501) staff       (20)     6379 2023-05-08 22:45:10.000000 slashml-0.0.5/slashml.egg-info/PKG-INFO
+-rw-r--r--   0 faizank    (501) staff       (20)      313 2023-05-08 22:45:10.000000 slashml-0.0.5/slashml.egg-info/SOURCES.txt
+-rw-r--r--   0 faizank    (501) staff       (20)        1 2023-05-08 22:45:10.000000 slashml-0.0.5/slashml.egg-info/dependency_links.txt
+-rw-r--r--   0 faizank    (501) staff       (20)       31 2023-05-08 22:45:10.000000 slashml-0.0.5/slashml.egg-info/requires.txt
+-rw-r--r--   0 faizank    (501) staff       (20)        8 2023-05-08 22:45:10.000000 slashml-0.0.5/slashml.egg-info/top_level.txt
```

### Comparing `slashml-0.0.4/LICENSE.txt` & `slashml-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slashml-0.0.4/README.md` & `slashml-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,52 +7,54 @@
 
 ```
 pip install slashml
 ```
 
 # Quickstart
 
-#### Transcribe an audio file
+#### Convert text to audio
 <!-- write a code snippet in the minimum number of lines  -->
 
 ```python
-from slashml import SpeechToText
+from slashml import TextToSpeech
+import time
 
 # Initialize model
-model = SpeechToText()
+model = TextToSpeech()
 
-service_provider = SpeechToText.ServiceProvider.ASSEMBLY
-# Submit transcription request
-job = model.transcribe(upload_url="https://slashml.s3.ca-central-1.amazonaws.com/c7d38026-3ab4-4a04-ad9e-b6679ab79a87", service_provider=service_provider)
+service_provider = TextToSpeech.ServiceProvider.GOOGLE
+
+# Submit speechification request
+job = model.speechify(text="To be or not to be, that is the question!", service_provider=service_provider)
 
 assert job.status != "ERROR", f"{job}"
 print(f"Job ID: {job.id}")
 
 # check job status
 response = model.status(job.id, service_provider=service_provider)
 
 while response.status == "IN_PROGRESS":
     time.sleep(30)
     response = model.status(job.id, service_provider=service_provider)
     print(f"Response = {response}. Retrying in 30 seconds")
 
-return response
+print(response)
 ```
 
-#### Summarize a text input
+#### Transcribe an audio file
 <!-- write a code snippet in the minimum number of lines  -->
 
 ```python
 from slashml import SpeechToText
 import time
 
 # Initialize model
 model = SpeechToText()
 
-service_provider = SpeechToText.ServiceProvider.ASSEMBLY
+service_provider = SpeechToText.ServiceProvider.WHISPER
 # Submit transcription request
 job = model.transcribe(upload_url="https://slashml.s3.ca-central-1.amazonaws.com/c7d38026-3ab4-4a04-ad9e-b6679ab79a87", service_provider=service_provider)
 
 assert job.status != "ERROR", f"{job}"
 print(f"Job ID: {job.id}")
 
 # check job status
@@ -62,43 +64,46 @@
     time.sleep(5)
     response = model.status(job.id, service_provider=service_provider)
     print(f"Response = {response}. Retrying in 5 seconds")
 
 print(response)
 ```
 
-
-#### Convert text to audio
+#### Summarize a text input
 <!-- write a code snippet in the minimum number of lines  -->
 
 ```python
-from slashml import TextToSpeech
+from slashml import TextSummarization
+import time
 
 # Initialize model
-model = TextToSpeech()
+model = TextSummarization()
 
-service_provider = TextToSpeech.ServiceProvider.GOOGLE
+service_provider = TextSummarization.ServiceProvider.OPENAI
 
-# Submit speechification request
-job = model.speechify(text="To be or not to be, that is the question!", service_provider=service_provider)
+# Submit summariztion request
+job = model.summarize(text="There are of course kinds of thinking that can be done without writing. If you don't need to go too deeply into a problem, you can solve it without writing. If you're thinking about how two pieces of machinery should fit together, writing about it probably won't help much. And when a problem can be described formally, you can sometimes solve it in your head. But if you need to solve a complicated, ill-defined problem, it will almost always help to write about it. Which in turn means that someone who's not good at writing will almost always be at a disadvantage in solving such problems.", service_provider=service_provider)
 
 assert job.status != "ERROR", f"{job}"
 print(f"Job ID: {job.id}")
 
 # check job status
 response = model.status(job.id, service_provider=service_provider)
 
 while response.status == "IN_PROGRESS":
-    time.sleep(30)
+    time.sleep(5)
     response = model.status(job.id, service_provider=service_provider)
-    print(f"Response = {response}. Retrying in 30 seconds")
+    print(f"Response = {response}. Retrying in 5 seconds")
 
-return response
+print(response)
 ```
 
+
+
+
 ### View the list of service providers available
 
 ```python
 from slashml import TextToSpeech
 
 print(TextToSpeech.ServiceProvider.choices())
```

### Comparing `slashml-0.0.4/setup.py` & `slashml-0.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,23 +4,28 @@
 SLASHML_DIR = os.environ['SLASHML_DIR']
 
 def read_req_file(req_type):
     with open(f"{SLASHML_DIR}requires-{req_type}.txt") as fp:  # pylint: disable=W1514
         requires = (line.strip() for line in fp)
         return [req for req in requires if req and not req.startswith("#")]
 
+# Read the contents of the README file
+with open("README.md", "r") as fh:
+    long_description = fh.read()
 
 setup(
     name="slashml",
-    version="0.0.4",
+    version="0.0.5",
     url="https://slashml.com/",
     author="eff-kay",
     author_email="faiizan14@gmail.com",
     description=(
         "A Python client for interacting with SlashML services" "Developed by SlashML."
     ),
+    long_description=long_description,  # Use the contents of the README file
+    long_description_content_type="text/markdown",  # Set the type of the README file
     packages=find_packages("."),
     package_dir={"": "."},
     install_requires=read_req_file("install"),
     license="MIT",
     python_requires=">=3.6",
 )
```

### Comparing `slashml-0.0.4/slashml/speech_to_text.py` & `slashml-0.0.5/slashml/speech_to_text.py`

 * *Files identical despite different names*

### Comparing `slashml-0.0.4/slashml/text_summarization.py` & `slashml-0.0.5/slashml/text_summarization.py`

 * *Files identical despite different names*

### Comparing `slashml-0.0.4/slashml/text_to_speech.py` & `slashml-0.0.5/slashml/text_to_speech.py`

 * *Files identical despite different names*

### Comparing `slashml-0.0.4/slashml/utils.py` & `slashml-0.0.5/slashml/utils.py`

 * *Files identical despite different names*

