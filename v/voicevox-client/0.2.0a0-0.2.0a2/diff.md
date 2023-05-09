# Comparing `tmp/voicevox-client-0.2.0a0.tar.gz` & `tmp/voicevox-client-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicevox-client-0.2.0a0.tar", last modified: Sat Mar 18 01:22:41 2023, max compression
+gzip compressed data, was "voicevox-client-0.2.0a2.tar", last modified: Tue May  9 14:20:05 2023, max compression
```

## Comparing `voicevox-client-0.2.0a0.tar` & `voicevox-client-0.2.0a2.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:22:41.751243 voicevox-client-0.2.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-03-18 01:22:41.751243 voicevox-client-0.2.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-18 01:22:41.751243 voicevox-client-0.2.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:22:41.751243 voicevox-client-0.2.0a0/voicevox/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/voicevox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/voicevox/audio_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/voicevox/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/voicevox/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/voicevox/http.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/voicevox/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/voicevox/speakers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:22:41.751243 voicevox-client-0.2.0a0/voicevox/types/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/voicevox/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/voicevox/types/audio_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-18 01:22:28.000000 voicevox-client-0.2.0a0/voicevox/types/speakers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 01:22:41.751243 voicevox-client-0.2.0a0/voicevox_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-03-18 01:22:41.000000 voicevox-client-0.2.0a0/voicevox_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-18 01:22:41.000000 voicevox-client-0.2.0a0/voicevox_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 01:22:41.000000 voicevox-client-0.2.0a0/voicevox_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-18 01:22:41.000000 voicevox-client-0.2.0a0/voicevox_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-18 01:22:41.000000 voicevox-client-0.2.0a0/voicevox_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:20:05.866662 voicevox-client-0.2.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-09 14:19:49.000000 voicevox-client-0.2.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-09 14:20:05.866662 voicevox-client-0.2.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-09 14:19:49.000000 voicevox-client-0.2.0a2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:20:05.866662 voicevox-client-0.2.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:20:05.866662 voicevox-client-0.2.0a2/voicevox/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/audio_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/speaker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/speakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/supported_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:20:05.866662 voicevox-client-0.2.0a2/voicevox/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/types/audio_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/types/speaker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/types/speakers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:20:05.866662 voicevox-client-0.2.0a2/voicevox_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-09 14:20:05.000000 voicevox-client-0.2.0a2/voicevox_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-09 14:20:05.000000 voicevox-client-0.2.0a2/voicevox_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:20:05.000000 voicevox-client-0.2.0a2/voicevox_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 14:20:05.000000 voicevox-client-0.2.0a2/voicevox_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 14:20:05.000000 voicevox-client-0.2.0a2/voicevox_client.egg-info/top_level.txt
```

### Comparing `voicevox-client-0.2.0a0/LICENSE` & `voicevox-client-0.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `voicevox-client-0.2.0a0/PKG-INFO` & `voicevox-client-0.2.0a2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,60 @@
 Metadata-Version: 2.1
 Name: voicevox-client
-Version: 0.2.0a0
+Version: 0.2.0a2
 Summary: Voicevox engine unoffical wrapper
 Home-page: https://github.com/voicevox-client/python
 Author: tuna2134
 License: MIT
 Project-URL: Documentation, https://voicevox-client.tuna2134.jp
-Project-URL: Source, https://github.com/tuna2134/voicevox-client
-Description-Content-Type: text/markdown
+Project-URL: Source, https://github.com/voicevox-client/python
+Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
-# voicevox client for python.
+voicevox client for python.
+===========================
+
+.. image:: https://readthedocs.org/projects/voicevox-client/badge/?version=latest
+    :target: https://voicevox-client.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
 Unoffical API wrapper that you can use voicevox easy!
 
-## Requirements
-`Voicevox engine` only!
+Requirements
+------------
+
+``Voicevox engine`` only!
 
-Well if you want install voicevox engine, please read [this](https://github.com/VOICEVOX/voicevox_engine/blob/master/README.md).
+Well if you want install voicevox engine, please read
+`this <https://github.com/VOICEVOX/voicevox_engine/blob/master/README.md>`__.
 
-## Install
-```sh
-pip install voicevox-client
-```
+Install
+-------
+
+.. code:: sh
+
+   pip install voicevox-client
 
 All that!
 
-## Example
-```python
-from voicevox import Client
-import asyncio
-
-
-async def main():
-    async with Client() as client:
-        audio_query = await client.create_audio_query(
-            "こんにちは！", speaker=1
-        )
-        with open("voice.wav", "wb") as f:
-            f.write(await audio_query.synthesis())
-
-
-if __name__ == "__main__":
-    asyncio.run(main())
-```
+Example
+-------
+
+.. code:: python
+
+   from voicevox import Client
+   import asyncio
+
+
+   async def main():
+       async with Client() as client:
+           audio_query = await client.create_audio_query(
+               "こんにちは！", speaker=1
+           )
+           with open("voice.wav", "wb") as f:
+               f.write(await audio_query.synthesis())
+
+
+   if __name__ == "__main__":
+       asyncio.run(main())
```

### Comparing `voicevox-client-0.2.0a0/README.md` & `voicevox-client-0.2.0a2/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,46 @@
-# voicevox client for python.
+voicevox client for python.
+===========================
+
+.. image:: https://readthedocs.org/projects/voicevox-client/badge/?version=latest
+    :target: https://voicevox-client.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
 Unoffical API wrapper that you can use voicevox easy!
 
-## Requirements
-`Voicevox engine` only!
+Requirements
+------------
+
+``Voicevox engine`` only!
 
-Well if you want install voicevox engine, please read [this](https://github.com/VOICEVOX/voicevox_engine/blob/master/README.md).
+Well if you want install voicevox engine, please read
+`this <https://github.com/VOICEVOX/voicevox_engine/blob/master/README.md>`__.
 
-## Install
-```sh
-pip install voicevox-client
-```
+Install
+-------
+
+.. code:: sh
+
+   pip install voicevox-client
 
 All that!
 
-## Example
-```python
-from voicevox import Client
-import asyncio
-
-
-async def main():
-    async with Client() as client:
-        audio_query = await client.create_audio_query(
-            "こんにちは！", speaker=1
-        )
-        with open("voice.wav", "wb") as f:
-            f.write(await audio_query.synthesis())
-
-
-if __name__ == "__main__":
-    asyncio.run(main())
-```
+Example
+-------
+
+.. code:: python
+
+   from voicevox import Client
+   import asyncio
+
+
+   async def main():
+       async with Client() as client:
+           audio_query = await client.create_audio_query(
+               "こんにちは！", speaker=1
+           )
+           with open("voice.wav", "wb") as f:
+               f.write(await audio_query.synthesis())
+
+
+   if __name__ == "__main__":
+       asyncio.run(main())
```

### Comparing `voicevox-client-0.2.0a0/setup.py` & `voicevox-client-0.2.0a2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 
 
 def get_version():
     with open("voicevox/__init__.py", "r") as f:
         return re.search(r'__version__ = "([^"]+)"', f.read()).group(1)
 
 
-with open("README.md", "r",  encoding='utf-8') as f:
+with open("README.rst", "r",  encoding='utf-8') as f:
     long_description = f.read()
 
 
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 
 setup(
     name="voicevox-client",
     description="Voicevox engine unoffical wrapper",
     url="https://github.com/voicevox-client/python",
     project_urls={
         "Documentation": "https://voicevox-client.tuna2134.jp",
-        "Source": "https://github.com/tuna2134/voicevox-client",
+        "Source": "https://github.com/voicevox-client/python",
     },
     version=get_version(),
     long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description_content_type="text/x-rst",
     author="tuna2134",
     license="MIT",
     packages=["voicevox", "voicevox.types"],
     package_data={
         "voicevox": ["py.typed"]
     },
     install_requires=requirements,
```

### Comparing `voicevox-client-0.2.0a0/voicevox/audio_query.py` & `voicevox-client-0.2.0a2/voicevox/audio_query.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,25 +88,25 @@
 
     Audio query to do synthesis.
 
     Attributes
     ----------
     accent_phrases: dict
         アクセント句のリスト
-    speed_scale: int
+    speed_scale: float
         Speech speed
-    pitch_scale: int
+    pitch_scale: float
         Speech pitch
-    intonation_scale: int
+    intonation_scale: float
         Speech intonation
-    volume_scale: int
+    volume_scale: float
         Speech volume
-    pre_phoneme_length: int
+    pre_phoneme_length: float
         音声の前の無音時間
-    post_phoneme_length: int
+    post_phoneme_length: float
         音声の後の無音時間
     output_sampling_rate: int
         音声データの出力サンプリングレート
     output_stereo: bool
         音声データをステレオ出力するか否か
     kana: str
         [読み取り専用]AquesTalkライクな読み仮名。音声合成クエリとしては無視される
@@ -118,20 +118,20 @@
         self.http = http
         self.__data = payload
 
         self.accent_phrases: List[AccentPhrase] = [
             AccentPhrase(accent_phrase)
             for accent_phrase in payload["accent_phrases"]
         ]
-        self.speed_scale: int = payload["speedScale"]
-        self.pitch_scale: int = payload["pitchScale"]
-        self.intonation_scale: int = payload["intonationScale"]
-        self.volume_scale: int = payload["volumeScale"]
-        self.pre_phoneme_length: int = payload["prePhonemeLength"]
-        self.post_phoneme_length: int = payload["postPhonemeLength"]
+        self.speed_scale: float = payload["speedScale"]
+        self.pitch_scale: float = payload["pitchScale"]
+        self.intonation_scale: float = payload["intonationScale"]
+        self.volume_scale: float = payload["volumeScale"]
+        self.pre_phoneme_length: float = payload["prePhonemeLength"]
+        self.post_phoneme_length: float = payload["postPhonemeLength"]
         self.output_sampling_rate: int = payload["outputSamplingRate"]
         self.output_stereo: bool = payload["outputStereo"]
 
     @property
     def kana(self) -> str:
         return self.__data["kana"]
```

### Comparing `voicevox-client-0.2.0a0/voicevox/client.py` & `voicevox-client-0.2.0a2/voicevox/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from typing_extensions import Self
 
 import logging
 
 from .audio_query import AudioQuery
 from .http import HttpClient
 from .speakers import Speaker
-
+from .speaker_info import SpeakerInfo
+from .supported_devices import SupportedDevices
 
 logger = logging.getLogger(__name__)
 
 
 class Client:
     """Voicevox client class
 
@@ -124,14 +125,41 @@
         Returns
         -------
         List[Speaker]
             Speakers
         """
         speakers = await self.http.get_speakers(core_version)
         return [Speaker(speaker) for speaker in speakers]
+    
+    async def fetch_speaker_info(
+        self, speaker_uuid: str, core_version: Optional[str] = None
+    ) -> SpeakerInfo:
+        """Fetch speaker's info by given uuid.
+
+        This function retrieves additional information about a specific speaker, including its voice samples, icon, and portrait images.
+
+        Parameters
+        ----------
+        speaker_uuid : str
+            speaker's uuid
+        core_version : Optional[str]
+            voicevox core version
+
+        Returns
+        -------
+        SpeakerInfo
+            Contains additional information of the speaker.
+        """
+        return SpeakerInfo(await self.http.get_speaker_info(speaker_uuid, core_version)) 
+
+    async def check_devices(self, core_version: Optional[str] = None) -> SupportedDevices:
+        params = {}
+        if core_version:
+            params["core_version"] = core_version
+        return SupportedDevices(await self.http.supported_devices(params))
 
     async def multi_synthesis(
         self, audio_queries: List[AudioQuery], speaker: int,
         *, core_version: Optional[str] = None
     ) -> bytes:
         """Multi synthe
```

### Comparing `voicevox-client-0.2.0a0/voicevox/http.py` & `voicevox-client-0.2.0a2/voicevox/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # voicevox - http
 
-from typing import List, Optional
+from typing import List, Optional, Dict
 
 import logging
 
 from httpx import AsyncClient
 
+
 from .errors import NotfoundError, HttpException
 from .types import AudioQueryType, SpeakerType
+from .types.speaker_info import SpeakerInfoType 
 
 
 logger = logging.getLogger(__name__)
 
 
 class HttpClient:
 
@@ -23,15 +25,16 @@
         logger.debug("Stop session")
         await self.session.aclose()
 
     async def request(self, method: str, path: str, **kwargs) -> dict:
         logger.debug(f"Request: {method} Path: {path} kwargs: {kwargs}")
         response = await self.session.request(method, path, **kwargs)
         logger.debug("StatusCode: {0.status_code} Response: {0.content}".format(response))
-        if response.status_code == 200 or response.status_code == 204:
+        if response.status_code == 200 or \
+        response.status_code == 204:
             if response.headers.get("content-type") == "application/json":
                 return response.json()
             else:
                 return response.content
         elif response.status_code == 404:
             raise NotfoundError(response.json()["detail"])
         else:
@@ -75,15 +78,25 @@
         self, core_version: Optional[str]
     ) -> List[SpeakerType]:
         params = {}
         if core_version is not None:
             params["core_version"] = core_version
         return await self.request("GET", "/speakers", params=params)
 
+    async def get_speaker_info(
+        self, speaker_uuid: str, core_version: Optional[str]
+    ) -> SpeakerInfoType:
+        params = {
+            "speaker_uuid": speaker_uuid 
+        }
+        if core_version is not None:
+            params["core_version"] = core_version
+        return await self.request("GET", "/speaker_info", params=params)
+
     async def initialize_speaker(self, params: dict) -> None:
         await self.request("POST", "/initialize_speaker", params=params)
 
     async def is_initialized_speaker(self, params: dict) -> bool:
         return await self.request("GET", "/is_initialized_speaker", params=params)
 
-
-
+    async def supported_devices(self, params: dict) -> Dict[str, bool]:
+        return await self.request("GET", "/supported_devices")
```

### Comparing `voicevox-client-0.2.0a0/voicevox/speakers.py` & `voicevox-client-0.2.0a2/voicevox/speakers.py`

 * *Files identical despite different names*

### Comparing `voicevox-client-0.2.0a0/voicevox/types/audio_query.py` & `voicevox-client-0.2.0a2/voicevox/types/audio_query.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 
 class MoraType(TypedDict):
     text: str
     consonant: str
     consonant_length: int
     vowel: str
     vowel_length: int
-    pitch: int
+    pitch: float
 
 
 class AccentPhraseType(TypedDict):
     moras: List[MoraType]
     accent: int
     is_interrogative: bool
     pause_mora: List[MoraType]
 
 
 class AudioQueryType(TypedDict):
     accent_phrases: List[AccentPhraseType]
-    speedScale: int
-    pitchScale: int
-    volumeScale: int
-    prePhonemeLength: int
-    postPhonemeLength: int
+    speedScale: float
+    pitchScale: float
+    intonationScale: float
+    volumeScale: float
+    prePhonemeLength: float
+    postPhonemeLength: float
     outputSamplingRate: int
     outputStereo: bool
     kana: str
```

### Comparing `voicevox-client-0.2.0a0/voicevox_client.egg-info/PKG-INFO` & `voicevox-client-0.2.0a2/voicevox_client.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,60 @@
 Metadata-Version: 2.1
 Name: voicevox-client
-Version: 0.2.0a0
+Version: 0.2.0a2
 Summary: Voicevox engine unoffical wrapper
 Home-page: https://github.com/voicevox-client/python
 Author: tuna2134
 License: MIT
 Project-URL: Documentation, https://voicevox-client.tuna2134.jp
-Project-URL: Source, https://github.com/tuna2134/voicevox-client
-Description-Content-Type: text/markdown
+Project-URL: Source, https://github.com/voicevox-client/python
+Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
-# voicevox client for python.
+voicevox client for python.
+===========================
+
+.. image:: https://readthedocs.org/projects/voicevox-client/badge/?version=latest
+    :target: https://voicevox-client.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
 Unoffical API wrapper that you can use voicevox easy!
 
-## Requirements
-`Voicevox engine` only!
+Requirements
+------------
+
+``Voicevox engine`` only!
 
-Well if you want install voicevox engine, please read [this](https://github.com/VOICEVOX/voicevox_engine/blob/master/README.md).
+Well if you want install voicevox engine, please read
+`this <https://github.com/VOICEVOX/voicevox_engine/blob/master/README.md>`__.
 
-## Install
-```sh
-pip install voicevox-client
-```
+Install
+-------
+
+.. code:: sh
+
+   pip install voicevox-client
 
 All that!
 
-## Example
-```python
-from voicevox import Client
-import asyncio
-
-
-async def main():
-    async with Client() as client:
-        audio_query = await client.create_audio_query(
-            "こんにちは！", speaker=1
-        )
-        with open("voice.wav", "wb") as f:
-            f.write(await audio_query.synthesis())
-
-
-if __name__ == "__main__":
-    asyncio.run(main())
-```
+Example
+-------
+
+.. code:: python
+
+   from voicevox import Client
+   import asyncio
+
+
+   async def main():
+       async with Client() as client:
+           audio_query = await client.create_audio_query(
+               "こんにちは！", speaker=1
+           )
+           with open("voice.wav", "wb") as f:
+               f.write(await audio_query.synthesis())
+
+
+   if __name__ == "__main__":
+       asyncio.run(main())
```

