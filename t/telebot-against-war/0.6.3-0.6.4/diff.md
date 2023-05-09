# Comparing `tmp/telebot_against_war-0.6.3.tar.gz` & `tmp/telebot_against_war-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebot_against_war-0.6.3.tar", max compression
+gzip compressed data, was "telebot_against_war-0.6.4.tar", max compression
```

## Comparing `telebot_against_war-0.6.3.tar` & `telebot_against_war-0.6.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    18047 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/LICENSE
--rw-r--r--   0        0        0     2064 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/README.md
--rw-r--r--   0        0        0     1103 2023-04-20 20:27:20.101179 telebot_against_war-0.6.3/pyproject.toml
--rw-r--r--   0        0        0   155717 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/__init__.py
--rw-r--r--   0        0        0    81276 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/api.py
--rw-r--r--   0        0        0     5034 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/callback_data.py
--rw-r--r--   0        0        0     2913 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/check_text.py
--rw-r--r--   0        0        0     4733 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/filters.py
--rw-r--r--   0        0        0     8645 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/formatting.py
--rw-r--r--   0        0        0     3225 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/graceful_shutdown.py
--rw-r--r--   0        0        0     2049 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/helpers.py
--rw-r--r--   0        0        0     2046 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/metrics.py
--rw-r--r--   0        0        0        0 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/py.typed
--rw-r--r--   0        0        0     1797 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/runner.py
--rw-r--r--   0        0        0      396 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/storages/__init__.py
--rw-r--r--   0        0        0     1710 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/storages/base_storage.py
--rw-r--r--   0        0        0     2296 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/storages/memory_storage.py
--rw-r--r--   0        0        0     3695 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/storages/pickle_storage.py
--rw-r--r--   0        0        0     5626 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/storages/redis_storage.py
--rw-r--r--   0        0        0    35563 2023-04-20 20:26:38.988561 telebot_against_war-0.6.3/telebot/test_util.py
--rw-r--r--   0        0        0   156941 2023-04-20 20:26:38.988561 telebot_against_war-0.6.3/telebot/types/__init__.py
--rw-r--r--   0        0        0     2724 2023-04-20 20:26:38.988561 telebot_against_war-0.6.3/telebot/types/constants.py
--rw-r--r--   0        0        0     1852 2023-04-20 20:26:38.988561 telebot_against_war-0.6.3/telebot/types/service.py
--rw-r--r--   0        0        0    10649 2023-04-20 20:26:38.988561 telebot_against_war-0.6.3/telebot/util.py
--rw-r--r--   0        0        0     8202 2023-04-20 20:26:38.988561 telebot_against_war-0.6.3/telebot/webhook.py
--rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 telebot_against_war-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    18047 2023-05-09 09:36:01.456969 telebot_against_war-0.6.4/LICENSE
+-rw-r--r--   0        0        0     2064 2023-05-09 09:36:01.456969 telebot_against_war-0.6.4/README.md
+-rw-r--r--   0        0        0     1103 2023-05-09 09:36:48.368161 telebot_against_war-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0   155717 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/__init__.py
+-rw-r--r--   0        0        0    82322 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/api.py
+-rw-r--r--   0        0        0     5034 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/callback_data.py
+-rw-r--r--   0        0        0     2913 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/check_text.py
+-rw-r--r--   0        0        0     4733 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/filters.py
+-rw-r--r--   0        0        0     8645 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/formatting.py
+-rw-r--r--   0        0        0     3225 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/graceful_shutdown.py
+-rw-r--r--   0        0        0     2049 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/helpers.py
+-rw-r--r--   0        0        0     2046 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/metrics.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/py.typed
+-rw-r--r--   0        0        0     1797 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/runner.py
+-rw-r--r--   0        0        0      396 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/storages/__init__.py
+-rw-r--r--   0        0        0     1710 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/storages/base_storage.py
+-rw-r--r--   0        0        0     2296 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/storages/memory_storage.py
+-rw-r--r--   0        0        0     3695 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/storages/pickle_storage.py
+-rw-r--r--   0        0        0     5626 2023-05-09 09:36:01.460969 telebot_against_war-0.6.4/telebot/storages/redis_storage.py
+-rw-r--r--   0        0        0    35563 2023-05-09 09:36:01.464969 telebot_against_war-0.6.4/telebot/test_util.py
+-rw-r--r--   0        0        0   156941 2023-05-09 09:36:01.464969 telebot_against_war-0.6.4/telebot/types/__init__.py
+-rw-r--r--   0        0        0     2724 2023-05-09 09:36:01.464969 telebot_against_war-0.6.4/telebot/types/constants.py
+-rw-r--r--   0        0        0     1852 2023-05-09 09:36:01.464969 telebot_against_war-0.6.4/telebot/types/service.py
+-rw-r--r--   0        0        0    10649 2023-05-09 09:36:01.464969 telebot_against_war-0.6.4/telebot/util.py
+-rw-r--r--   0        0        0     8202 2023-05-09 09:36:01.464969 telebot_against_war-0.6.4/telebot/webhook.py
+-rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 telebot_against_war-0.6.4/PKG-INFO
```

### Comparing `telebot_against_war-0.6.3/LICENSE` & `telebot_against_war-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/README.md` & `telebot_against_war-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/pyproject.toml` & `telebot_against_war-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telebot-against-war"
-version = "0.6.3"  # replaced by dynamic versioning plugin
+version = "0.6.4"  # replaced by dynamic versioning plugin
 description = "Async-first fork of pyTelegramBotApi"
 authors = ["Igor Vaiman <gosha.vaiman@gmail.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 repository = "https://github.com/bots-against-war/telebot"
 packages = [
     { include = "telebot" },
```

### Comparing `telebot_against_war-0.6.3/telebot/__init__.py` & `telebot_against_war-0.6.4/telebot/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/api.py` & `telebot_against_war-0.6.4/telebot/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,5080 +1,5146 @@
 00000000: 696d 706f 7274 206c 6f67 6769 6e67 0a69  import logging.i
 00000010: 6d70 6f72 7420 6f73 0a69 6d70 6f72 7420  mport os.import 
-00000020: 7265 0a69 6d70 6f72 7420 7575 6964 0a66  re.import uuid.f
-00000030: 726f 6d20 6461 7465 7469 6d65 2069 6d70  rom datetime imp
-00000040: 6f72 7420 6461 7465 7469 6d65 0a66 726f  ort datetime.fro
-00000050: 6d20 696f 2069 6d70 6f72 7420 4279 7465  m io import Byte
-00000060: 7349 4f0a 6672 6f6d 2074 7970 696e 6720  sIO.from typing 
-00000070: 696d 706f 7274 2041 6e79 2c20 4469 6374  import Any, Dict
-00000080: 2c20 4f70 7469 6f6e 616c 2c20 556e 696f  , Optional, Unio
-00000090: 6e2c 2063 6173 740a 0a69 6d70 6f72 7420  n, cast..import 
-000000a0: 6169 6f68 7474 700a 696d 706f 7274 2075  aiohttp.import u
-000000b0: 6a73 6f6e 2061 7320 6a73 6f6e 2020 2320  json as json  # 
-000000c0: 7479 7065 3a20 6967 6e6f 7265 0a0a 6672  type: ignore..fr
-000000d0: 6f6d 2074 656c 6562 6f74 2069 6d70 6f72  om telebot impor
-000000e0: 7420 7479 7065 732c 2075 7469 6c0a 0a6c  t types, util..l
-000000f0: 6f67 6765 7220 3d20 6c6f 6767 696e 672e  ogger = logging.
-00000100: 6765 744c 6f67 6765 7228 5f5f 6e61 6d65  getLogger(__name
-00000110: 5f5f 290a 0a0a 4649 4c45 5f55 524c 3a20  __)...FILE_URL: 
-00000120: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00000130: 4e6f 6e65 0a43 5553 544f 4d5f 5345 5249  None.CUSTOM_SERI
-00000140: 414c 495a 4552 203d 204e 6f6e 650a 0a44  ALIZER = None..D
-00000150: 4546 4155 4c54 5f52 4551 5545 5354 5f54  EFAULT_REQUEST_T
-00000160: 494d 454f 5554 203d 204e 6f6e 650a 4d41  IMEOUT = None.MA
-00000170: 585f 5245 5452 4945 5320 3d20 350a 5245  X_RETRIES = 5.RE
-00000180: 5155 4553 545f 4c49 4d49 5420 3d20 3530  QUEST_LIMIT = 50
-00000190: 0a0a 0a63 6c61 7373 2053 6573 7369 6f6e  ...class Session
-000001a0: 4d61 6e61 6765 723a 0a20 2020 2064 6566  Manager:.    def
-000001b0: 205f 5f69 6e69 745f 5f28 7365 6c66 2920   __init__(self) 
-000001c0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-000001d0: 2073 656c 662e 7365 7373 696f 6e3a 204f   self.session: O
-000001e0: 7074 696f 6e61 6c5b 6169 6f68 7474 702e  ptional[aiohttp.
-000001f0: 436c 6965 6e74 5365 7373 696f 6e5d 203d  ClientSession] =
-00000200: 204e 6f6e 650a 0a20 2020 2064 6566 2073   None..    def s
-00000210: 6574 5f73 6573 7369 6f6e 2873 656c 662c  et_session(self,
-00000220: 2073 6573 7369 6f6e 3a20 6169 6f68 7474   session: aiohtt
-00000230: 702e 436c 6965 6e74 5365 7373 696f 6e29  p.ClientSession)
-00000240: 3a0a 2020 2020 2020 2020 7365 6c66 2e73  :.        self.s
-00000250: 6573 7369 6f6e 203d 2073 6573 7369 6f6e  ession = session
-00000260: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00000270: 636c 6f73 655f 7365 7373 696f 6e28 7365  close_session(se
-00000280: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-00000290: 7365 6c66 2e73 6573 7369 6f6e 2069 7320  self.session is 
-000002a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000002b0: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
-000002c0: 2e73 6573 7369 6f6e 2e63 6c6f 7365 2829  .session.close()
-000002d0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-000002e0: 696e 6974 5f73 6573 7369 6f6e 2873 656c  init_session(sel
-000002f0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00000300: 2e73 6573 7369 6f6e 203d 2061 696f 6874  .session = aioht
-00000310: 7470 2e43 6c69 656e 7453 6573 7369 6f6e  tp.ClientSession
-00000320: 2863 6f6e 6e65 6374 6f72 3d61 696f 6874  (connector=aioht
-00000330: 7470 2e54 4350 436f 6e6e 6563 746f 7228  tp.TCPConnector(
-00000340: 6c69 6d69 743d 5245 5155 4553 545f 4c49  limit=REQUEST_LI
-00000350: 4d49 5429 290a 0a20 2020 2061 7379 6e63  MIT))..    async
-00000360: 2064 6566 2067 6574 5f73 6573 7369 6f6e   def get_session
-00000370: 2873 656c 6629 202d 3e20 6169 6f68 7474  (self) -> aiohtt
-00000380: 702e 436c 6965 6e74 5365 7373 696f 6e3a  p.ClientSession:
-00000390: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000003a0: 2e73 6573 7369 6f6e 2069 7320 4e6f 6e65  .session is None
-000003b0: 206f 7220 7365 6c66 2e73 6573 7369 6f6e   or self.session
-000003c0: 2e63 6c6f 7365 6420 6f72 206e 6f74 2073  .closed or not s
-000003d0: 656c 662e 7365 7373 696f 6e2e 5f6c 6f6f  elf.session._loo
-000003e0: 702e 6973 5f72 756e 6e69 6e67 2829 3a0a  p.is_running():.
-000003f0: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00000400: 7420 7365 6c66 2e69 6e69 745f 7365 7373  t self.init_sess
-00000410: 696f 6e28 290a 2020 2020 2020 2020 7265  ion().        re
-00000420: 7475 726e 2063 6173 7428 6169 6f68 7474  turn cast(aiohtt
-00000430: 702e 436c 6965 6e74 5365 7373 696f 6e2c  p.ClientSession,
-00000440: 2073 656c 662e 7365 7373 696f 6e29 0a0a   self.session)..
-00000450: 0a73 6573 7369 6f6e 5f6d 616e 6167 6572  .session_manager
-00000460: 203d 2053 6573 7369 6f6e 4d61 6e61 6765   = SessionManage
-00000470: 7228 290a 0a0a 4669 6c65 4f62 6a65 6374  r()...FileObject
-00000480: 203d 2055 6e69 6f6e 5b42 7974 6573 494f   = Union[BytesIO
-00000490: 2c20 6279 7465 732c 2062 7974 6561 7272  , bytes, bytearr
-000004a0: 6179 2c20 6d65 6d6f 7279 7669 6577 5d0a  ay, memoryview].
-000004b0: 5061 7261 6d73 203d 2064 6963 745b 7374  Params = dict[st
-000004c0: 722c 2041 6e79 5d0a 4669 6c65 7320 3d20  r, Any].Files = 
-000004d0: 6469 6374 5b73 7472 2c20 556e 696f 6e5b  dict[str, Union[
-000004e0: 7475 706c 655b 7374 722c 2046 696c 654f  tuple[str, FileO
-000004f0: 626a 6563 745d 2c20 4669 6c65 4f62 6a65  bject], FileObje
-00000500: 6374 5d5d 0a0a 0a61 7379 6e63 2064 6566  ct]]...async def
-00000510: 205f 7265 7175 6573 7428 0a20 2020 2074   _request(.    t
-00000520: 6f6b 656e 3a20 7374 722c 0a20 2020 2072  oken: str,.    r
-00000530: 6f75 7465 3a20 7374 722c 0a20 2020 206d  oute: str,.    m
-00000540: 6574 686f 643a 2073 7472 203d 2022 6765  ethod: str = "ge
-00000550: 7422 2c0a 2020 2020 7061 7261 6d73 3a20  t",.    params: 
-00000560: 4f70 7469 6f6e 616c 5b50 6172 616d 735d  Optional[Params]
-00000570: 203d 204e 6f6e 652c 0a20 2020 2066 696c   = None,.    fil
-00000580: 6573 3a20 4f70 7469 6f6e 616c 5b46 696c  es: Optional[Fil
-00000590: 6573 5d20 3d20 4e6f 6e65 2c0a 2020 2020  es] = None,.    
-000005a0: 7265 7175 6573 745f 7469 6d65 6f75 743a  request_timeout:
-000005b0: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
-000005c0: 203d 204e 6f6e 652c 0a29 3a0a 2020 2020   = None,.):.    
-000005d0: 7365 7373 696f 6e20 3d20 6177 6169 7420  session = await 
-000005e0: 7365 7373 696f 6e5f 6d61 6e61 6765 722e  session_manager.
-000005f0: 6765 745f 7365 7373 696f 6e28 290a 2020  get_session().  
-00000600: 2020 7265 7175 6573 745f 6465 7363 7269    request_descri
-00000610: 7074 696f 6e20 3d20 6622 7b6d 6574 686f  ption = f"{metho
-00000620: 6420 3d20 7d20 7b72 6f75 7465 203d 207d  d = } {route = }
-00000630: 207b 7061 7261 6d73 203d 207d 207b 6669   {params = } {fi
-00000640: 6c65 7320 3d20 7d20 7b72 6571 7565 7374  les = } {request
-00000650: 5f74 696d 656f 7574 203d 207d 220a 2020  _timeout = }".  
-00000660: 2020 7265 7175 6573 745f 6465 7363 7269    request_descri
-00000670: 7074 696f 6e20 3d20 7265 7175 6573 745f  ption = request_
-00000680: 6465 7363 7269 7074 696f 6e2e 7265 706c  description.repl
-00000690: 6163 6528 746f 6b65 6e2c 2022 3c62 6f74  ace(token, "<bot
-000006a0: 2d74 6f6b 656e 3e22 290a 2020 2020 6c6f  -token>").    lo
-000006b0: 6767 6572 2e64 6562 7567 2822 4d61 6b69  gger.debug("Maki
-000006c0: 6e67 2072 6571 7565 7374 3a20 2573 222c  ng request: %s",
-000006d0: 2072 6571 7565 7374 5f64 6573 6372 6970   request_descrip
-000006e0: 7469 6f6e 290a 2020 2020 6c61 7374 5f65  tion).    last_e
-000006f0: 7863 6570 7469 6f6e 3a20 4f70 7469 6f6e  xception: Option
-00000700: 616c 5b45 7863 6570 7469 6f6e 5d20 3d20  al[Exception] = 
-00000710: 4e6f 6e65 0a20 2020 2066 6f72 2061 7474  None.    for att
-00000720: 656d 7074 2069 6e20 7261 6e67 6528 4d41  empt in range(MA
-00000730: 585f 5245 5452 4945 5329 3a0a 2020 2020  X_RETRIES):.    
-00000740: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00000750: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-00000760: 7365 7373 696f 6e2e 7265 7175 6573 7428  session.request(
-00000770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000780: 206d 6574 686f 643d 6d65 7468 6f64 2c0a   method=method,.
-00000790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007a0: 7572 6c3d 2268 7474 7073 3a2f 2f61 7069  url="https://api
-000007b0: 2e74 656c 6567 7261 6d2e 6f72 672f 626f  .telegram.org/bo
-000007c0: 747b 307d 2f7b 317d 222e 666f 726d 6174  t{0}/{1}".format
-000007d0: 2874 6f6b 656e 2c20 726f 7574 6529 2c0a  (token, route),.
-000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007f0: 6461 7461 3d74 6f5f 666f 726d 5f64 6174  data=to_form_dat
-00000800: 6128 7061 7261 6d73 2c20 6669 6c65 7329  a(params, files)
-00000810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000820: 2020 7469 6d65 6f75 743d 6169 6f68 7474    timeout=aiohtt
-00000830: 702e 436c 6965 6e74 5469 6d65 6f75 7428  p.ClientTimeout(
-00000840: 746f 7461 6c3d 7265 7175 6573 745f 7469  total=request_ti
-00000850: 6d65 6f75 7420 6f72 2044 4546 4155 4c54  meout or DEFAULT
-00000860: 5f52 4551 5545 5354 5f54 494d 454f 5554  _REQUEST_TIMEOUT
-00000870: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
-00000880: 2061 7320 7265 7370 3a0a 2020 2020 2020   as resp:.      
-00000890: 2020 2020 2020 2020 2020 6a73 6f6e 5f72            json_r
-000008a0: 6573 756c 7420 3d20 6177 6169 7420 5f63  esult = await _c
-000008b0: 6865 636b 5f72 6573 706f 6e73 6528 7265  heck_response(re
-000008c0: 7370 290a 2020 2020 2020 2020 2020 2020  sp).            
-000008d0: 2020 2020 6966 206a 736f 6e5f 7265 7375      if json_resu
-000008e0: 6c74 3a0a 2020 2020 2020 2020 2020 2020  lt:.            
-000008f0: 2020 2020 2020 2020 7265 7475 726e 206a          return j
-00000900: 736f 6e5f 7265 7375 6c74 5b22 7265 7375  son_result["resu
-00000910: 6c74 225d 0a20 2020 2020 2020 2065 7863  lt"].        exc
-00000920: 6570 7420 4170 6945 7863 6570 7469 6f6e  ept ApiException
-00000930: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00000940: 6973 650a 2020 2020 2020 2020 6578 6365  ise.        exce
-00000950: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00000960: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
-00000970: 6173 745f 6578 6365 7074 696f 6e20 3d20  ast_exception = 
-00000980: 650a 2020 2020 2020 2020 2020 2020 6c6f  e.            lo
-00000990: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
-000009a0: 2020 2020 2020 2020 2020 2022 5265 7472             "Retr
-000009b0: 7969 6e67 2028 2573 202f 2025 7329 2075  ying (%s / %s) u
-000009c0: 6e65 7870 6563 7465 6420 6572 726f 7220  nexpected error 
-000009d0: 6d61 6b69 6e67 2072 6571 7565 7374 2028  making request (
-000009e0: 2573 2922 2c0a 2020 2020 2020 2020 2020  %s)",.          
-000009f0: 2020 2020 2020 6174 7465 6d70 7420 2b20        attempt + 
-00000a00: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00000a10: 2020 204d 4158 5f52 4554 5249 4553 2c0a     MAX_RETRIES,.
-00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a30: 7265 7175 6573 745f 6465 7363 7269 7074  request_descript
-00000a40: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00000a50: 2020 2020 2065 7863 5f69 6e66 6f3d 5472       exc_info=Tr
-00000a60: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00000a70: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00000a80: 2020 2020 6966 206c 6173 745f 6578 6365      if last_exce
-00000a90: 7074 696f 6e20 6973 206e 6f74 204e 6f6e  ption is not Non
-00000aa0: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
-00000ab0: 6f67 6765 722e 6572 726f 7228 2252 6571  ogger.error("Req
-00000ac0: 7565 7374 2028 2573 2920 6469 646e 2774  uest (%s) didn't
-00000ad0: 2073 7563 6365 6564 6564 2c20 7265 7261   succeeded, rera
-00000ae0: 6973 696e 6720 6c61 7374 2065 7863 6570  ising last excep
-00000af0: 7469 6f6e 222c 2072 6571 7565 7374 5f64  tion", request_d
-00000b00: 6573 6372 6970 7469 6f6e 290a 2020 2020  escription).    
-00000b10: 2020 2020 2020 2020 7261 6973 6520 6c61          raise la
-00000b20: 7374 5f65 7863 6570 7469 6f6e 0a0a 0a64  st_exception...d
-00000b30: 6566 2065 7874 7261 6374 5f66 696c 656e  ef extract_filen
-00000b40: 616d 6528 6f62 6a3a 2041 6e79 2920 2d3e  ame(obj: Any) ->
-00000b50: 204f 7074 696f 6e61 6c5b 7374 725d 3a0a   Optional[str]:.
-00000b60: 2020 2020 6e61 6d65 203d 2067 6574 6174      name = getat
-00000b70: 7472 286f 626a 2c20 226e 616d 6522 2c20  tr(obj, "name", 
-00000b80: 4e6f 6e65 290a 2020 2020 6966 206e 616d  None).    if nam
-00000b90: 6520 616e 6420 6973 696e 7374 616e 6365  e and isinstance
-00000ba0: 286e 616d 652c 2073 7472 2920 616e 6420  (name, str) and 
-00000bb0: 6e61 6d65 5b30 5d20 213d 2022 3c22 2061  name[0] != "<" a
-00000bc0: 6e64 206e 616d 655b 2d31 5d20 213d 2022  nd name[-1] != "
-00000bd0: 3e22 3a0a 2020 2020 2020 2020 7265 7475  >":.        retu
-00000be0: 726e 206f 732e 7061 7468 2e62 6173 656e  rn os.path.basen
-00000bf0: 616d 6528 6e61 6d65 290a 2020 2020 656c  ame(name).    el
-00000c00: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
-00000c10: 726e 204e 6f6e 650a 0a0a 6465 6620 746f  rn None...def to
-00000c20: 5f66 6f72 6d5f 6461 7461 2870 6172 616d  _form_data(param
-00000c30: 733a 204f 7074 696f 6e61 6c5b 5061 7261  s: Optional[Para
-00000c40: 6d73 5d20 3d20 4e6f 6e65 2c20 6669 6c65  ms] = None, file
-00000c50: 733a 204f 7074 696f 6e61 6c5b 4669 6c65  s: Optional[File
-00000c60: 735d 203d 204e 6f6e 6529 202d 3e20 6169  s] = None) -> ai
-00000c70: 6f68 7474 702e 466f 726d 4461 7461 3a0a  ohttp.FormData:.
-00000c80: 2020 2020 6461 7461 203d 2061 696f 6874      data = aioht
-00000c90: 7470 2e66 6f72 6d64 6174 612e 466f 726d  tp.formdata.Form
-00000ca0: 4461 7461 2871 756f 7465 5f66 6965 6c64  Data(quote_field
-00000cb0: 733d 4661 6c73 6529 0a0a 2020 2020 6966  s=False)..    if
-00000cc0: 2070 6172 616d 733a 0a20 2020 2020 2020   params:.       
-00000cd0: 2066 6f72 206b 6579 2c20 7661 6c75 6520   for key, value 
-00000ce0: 696e 2070 6172 616d 732e 6974 656d 7328  in params.items(
-00000cf0: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
-00000d00: 6174 612e 6164 645f 6669 656c 6428 6b65  ata.add_field(ke
-00000d10: 792c 2073 7472 2876 616c 7565 2929 0a0a  y, str(value))..
-00000d20: 2020 2020 6966 2066 696c 6573 3a0a 2020      if files:.  
-00000d30: 2020 2020 2020 666f 7220 6b65 792c 2066        for key, f
-00000d40: 2069 6e20 6669 6c65 732e 6974 656d 7328   in files.items(
-00000d50: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00000d60: 6620 6973 696e 7374 616e 6365 2866 2c20  f isinstance(f, 
-00000d70: 7475 706c 6529 3a0a 2020 2020 2020 2020  tuple):.        
-00000d80: 2020 2020 2020 2020 6966 206c 656e 2866          if len(f
-00000d90: 2920 3d3d 2032 3a0a 2020 2020 2020 2020  ) == 2:.        
-00000da0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00000db0: 6e61 6d65 2c20 6669 6c65 5f6f 626a 6563  name, file_objec
-00000dc0: 7420 3d20 660a 2020 2020 2020 2020 2020  t = f.          
-00000dd0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00000de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000df0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00000e00: 2822 5475 706c 6520 6d75 7374 2068 6176  ("Tuple must hav
-00000e10: 6520 6578 6163 746c 7920 3220 656c 656d  e exactly 2 elem
-00000e20: 656e 7473 3a20 6669 6c65 6e61 6d65 2c20  ents: filename, 
-00000e30: 6669 6c65 5f6f 626a 6563 7422 290a 2020  file_object").  
-00000e40: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e60: 6669 6c65 6e61 6d65 2c20 6669 6c65 5f6f  filename, file_o
-00000e70: 626a 6563 7420 3d20 6578 7472 6163 745f  bject = extract_
-00000e80: 6669 6c65 6e61 6d65 2866 2920 6f72 206b  filename(f) or k
-00000e90: 6579 2c20 660a 0a20 2020 2020 2020 2020  ey, f..         
-00000ea0: 2020 2064 6174 612e 6164 645f 6669 656c     data.add_fiel
-00000eb0: 6428 6b65 792c 2066 696c 655f 6f62 6a65  d(key, file_obje
-00000ec0: 6374 2c20 6669 6c65 6e61 6d65 3d66 696c  ct, filename=fil
-00000ed0: 656e 616d 6529 0a0a 2020 2020 7265 7475  ename)..    retu
-00000ee0: 726e 2064 6174 610a 0a0a 6173 796e 6320  rn data...async 
-00000ef0: 6465 6620 5f63 6f6e 7665 7274 5f6d 6172  def _convert_mar
-00000f00: 6b75 7028 6d61 726b 7570 293a 0a20 2020  kup(markup):.   
-00000f10: 2069 6620 6973 696e 7374 616e 6365 286d   if isinstance(m
-00000f20: 6172 6b75 702c 2074 7970 6573 2e4a 736f  arkup, types.Jso
-00000f30: 6e53 6572 6961 6c69 7a61 626c 6529 3a0a  nSerializable):.
-00000f40: 2020 2020 2020 2020 7265 7475 726e 206d          return m
-00000f50: 6172 6b75 702e 746f 5f6a 736f 6e28 290a  arkup.to_json().
-00000f60: 2020 2020 7265 7475 726e 206d 6172 6b75      return marku
-00000f70: 700a 0a0a 6173 796e 6320 6465 6620 6765  p...async def ge
-00000f80: 745f 6d65 2874 6f6b 656e 293a 0a20 2020  t_me(token):.   
-00000f90: 2072 6574 7572 6e20 6177 6169 7420 5f72   return await _r
-00000fa0: 6571 7565 7374 2874 6f6b 656e 2c20 2267  equest(token, "g
-00000fb0: 6574 4d65 2229 0a0a 0a61 7379 6e63 2064  etMe")...async d
-00000fc0: 6566 206c 6f67 5f6f 7574 2874 6f6b 656e  ef log_out(token
-00000fd0: 293a 0a20 2020 2072 6574 7572 6e20 6177  ):.    return aw
-00000fe0: 6169 7420 5f72 6571 7565 7374 2874 6f6b  ait _request(tok
-00000ff0: 656e 2c20 226c 6f67 4f75 7422 290a 0a0a  en, "logOut")...
-00001000: 6173 796e 6320 6465 6620 636c 6f73 6528  async def close(
-00001010: 746f 6b65 6e29 3a0a 2020 2020 7265 7475  token):.    retu
-00001020: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
-00001030: 7428 746f 6b65 6e2c 2022 636c 6f73 6522  t(token, "close"
-00001040: 290a 0a0a 6173 796e 6320 6465 6620 6765  )...async def ge
-00001050: 745f 6669 6c65 2874 6f6b 656e 2c20 6669  t_file(token, fi
-00001060: 6c65 5f69 6429 3a0a 2020 2020 7265 7475  le_id):.    retu
-00001070: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
-00001080: 7428 746f 6b65 6e2c 2022 6765 7446 696c  t(token, "getFil
-00001090: 6522 2c20 7061 7261 6d73 3d7b 2266 696c  e", params={"fil
-000010a0: 655f 6964 223a 2066 696c 655f 6964 7d29  e_id": file_id})
-000010b0: 0a0a 0a61 7379 6e63 2064 6566 2067 6574  ...async def get
-000010c0: 5f66 696c 655f 7572 6c28 746f 6b65 6e3a  _file_url(token:
-000010d0: 2073 7472 2c20 6669 6c65 5f69 643a 2073   str, file_id: s
-000010e0: 7472 293a 0a20 2020 2069 6620 4649 4c45  tr):.    if FILE
-000010f0: 5f55 524c 2069 7320 4e6f 6e65 3a0a 2020  _URL is None:.  
-00001100: 2020 2020 2020 7265 7475 726e 2022 6874        return "ht
-00001110: 7470 733a 2f2f 6170 692e 7465 6c65 6772  tps://api.telegr
-00001120: 616d 2e6f 7267 2f66 696c 652f 626f 747b  am.org/file/bot{
-00001130: 307d 2f7b 317d 222e 666f 726d 6174 2874  0}/{1}".format(t
-00001140: 6f6b 656e 2c20 6177 6169 7420 6765 745f  oken, await get_
-00001150: 6669 6c65 2874 6f6b 656e 2c20 6669 6c65  file(token, file
-00001160: 5f69 6429 5b22 6669 6c65 5f70 6174 6822  _id)["file_path"
-00001170: 5d29 0a20 2020 2065 6c73 653a 0a20 2020  ]).    else:.   
-00001180: 2020 2020 2072 6574 7572 6e20 4649 4c45       return FILE
-00001190: 5f55 524c 2e66 6f72 6d61 7428 746f 6b65  _URL.format(toke
-000011a0: 6e2c 2061 7761 6974 2067 6574 5f66 696c  n, await get_fil
-000011b0: 6528 746f 6b65 6e2c 2066 696c 655f 6964  e(token, file_id
-000011c0: 295b 2266 696c 655f 7061 7468 225d 290a  )["file_path"]).
-000011d0: 0a0a 6173 796e 6320 6465 6620 646f 776e  ..async def down
-000011e0: 6c6f 6164 5f66 696c 6528 746f 6b65 6e3a  load_file(token:
-000011f0: 2073 7472 2c20 6669 6c65 5f70 6174 683a   str, file_path:
-00001200: 2073 7472 293a 0a20 2020 2069 6620 4649   str):.    if FI
-00001210: 4c45 5f55 524c 2069 7320 4e6f 6e65 3a0a  LE_URL is None:.
-00001220: 2020 2020 2020 2020 7572 6c20 3d20 2268          url = "h
-00001230: 7474 7073 3a2f 2f61 7069 2e74 656c 6567  ttps://api.teleg
-00001240: 7261 6d2e 6f72 672f 6669 6c65 2f62 6f74  ram.org/file/bot
-00001250: 7b30 7d2f 7b31 7d22 2e66 6f72 6d61 7428  {0}/{1}".format(
-00001260: 746f 6b65 6e2c 2066 696c 655f 7061 7468  token, file_path
-00001270: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00001280: 2020 2020 7572 6c20 3d20 4649 4c45 5f55      url = FILE_U
-00001290: 524c 2e66 6f72 6d61 7428 746f 6b65 6e2c  RL.format(token,
-000012a0: 2066 696c 655f 7061 7468 290a 2020 2020   file_path).    
-000012b0: 7365 7373 696f 6e20 3d20 6177 6169 7420  session = await 
-000012c0: 7365 7373 696f 6e5f 6d61 6e61 6765 722e  session_manager.
-000012d0: 6765 745f 7365 7373 696f 6e28 290a 2020  get_session().  
-000012e0: 2020 6173 796e 6320 7769 7468 2073 6573    async with ses
-000012f0: 7369 6f6e 2e67 6574 2875 726c 2920 6173  sion.get(url) as
-00001300: 2072 6573 706f 6e73 653a 0a20 2020 2020   response:.     
-00001310: 2020 2072 6573 756c 7420 3d20 6177 6169     result = awai
-00001320: 7420 7265 7370 6f6e 7365 2e72 6561 6428  t response.read(
-00001330: 290a 2020 2020 2020 2020 6966 2072 6573  ).        if res
-00001340: 706f 6e73 652e 7374 6174 7573 2021 3d20  ponse.status != 
-00001350: 3230 303a 0a20 2020 2020 2020 2020 2020  200:.           
-00001360: 2072 6169 7365 2041 7069 4854 5450 4578   raise ApiHTTPEx
-00001370: 6365 7074 696f 6e28 2245 7272 6f72 2064  ception("Error d
-00001380: 6f77 6e6c 6f61 6469 6e67 2066 696c 6522  ownloading file"
-00001390: 2c20 7265 7370 6f6e 7365 290a 0a20 2020  , response)..   
-000013a0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000013b0: 0a61 7379 6e63 2064 6566 2073 6574 5f77  .async def set_w
-000013c0: 6562 686f 6f6b 280a 2020 2020 746f 6b65  ebhook(.    toke
-000013d0: 6e3a 2073 7472 2c0a 2020 2020 7572 6c3a  n: str,.    url:
-000013e0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-000013f0: 2063 6572 7469 6669 6361 7465 3a20 4f70   certificate: Op
-00001400: 7469 6f6e 616c 5b46 696c 654f 626a 6563  tional[FileObjec
-00001410: 745d 203d 204e 6f6e 652c 0a20 2020 206d  t] = None,.    m
-00001420: 6178 5f63 6f6e 6e65 6374 696f 6e73 3a20  ax_connections: 
-00001430: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00001440: 4e6f 6e65 2c0a 2020 2020 616c 6c6f 7765  None,.    allowe
-00001450: 645f 7570 6461 7465 733a 204f 7074 696f  d_updates: Optio
-00001460: 6e61 6c5b 6c69 7374 5b73 7472 5d5d 203d  nal[list[str]] =
-00001470: 204e 6f6e 652c 0a20 2020 2069 705f 6164   None,.    ip_ad
-00001480: 6472 6573 733a 204f 7074 696f 6e61 6c5b  dress: Optional[
-00001490: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-000014a0: 2064 726f 705f 7065 6e64 696e 675f 7570   drop_pending_up
-000014b0: 6461 7465 733a 204f 7074 696f 6e61 6c5b  dates: Optional[
-000014c0: 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020  bool] = None,.  
-000014d0: 2020 7469 6d65 6f75 743a 204f 7074 696f    timeout: Optio
-000014e0: 6e61 6c5b 666c 6f61 745d 203d 204e 6f6e  nal[float] = Non
-000014f0: 652c 0a20 2020 2073 6563 7265 745f 746f  e,.    secret_to
-00001500: 6b65 6e3a 204f 7074 696f 6e61 6c5b 7374  ken: Optional[st
-00001510: 725d 203d 204e 6f6e 652c 0a29 3a0a 2020  r] = None,.):.  
-00001520: 2020 6669 6c65 733a 204f 7074 696f 6e61    files: Optiona
-00001530: 6c5b 4669 6c65 735d 203d 207b 2263 6572  l[Files] = {"cer
-00001540: 7469 6669 6361 7465 223a 2063 6572 7469  tificate": certi
-00001550: 6669 6361 7465 7d20 6966 2063 6572 7469  ficate} if certi
-00001560: 6669 6361 7465 2065 6c73 6520 4e6f 6e65  ficate else None
-00001570: 0a20 2020 2070 6172 616d 733a 2050 6172  .    params: Par
-00001580: 616d 7320 3d20 7b22 7572 6c22 3a20 7572  ams = {"url": ur
-00001590: 6c7d 0a20 2020 2069 6620 6d61 785f 636f  l}.    if max_co
-000015a0: 6e6e 6563 7469 6f6e 733a 0a20 2020 2020  nnections:.     
-000015b0: 2020 2070 6172 616d 735b 226d 6178 5f63     params["max_c
-000015c0: 6f6e 6e65 6374 696f 6e73 225d 203d 206d  onnections"] = m
-000015d0: 6178 5f63 6f6e 6e65 6374 696f 6e73 0a20  ax_connections. 
-000015e0: 2020 2069 6620 616c 6c6f 7765 645f 7570     if allowed_up
-000015f0: 6461 7465 7320 6973 206e 6f74 204e 6f6e  dates is not Non
-00001600: 653a 2020 2320 456d 7074 7920 6c69 7374  e:  # Empty list
-00001610: 7320 7368 6f75 6c64 2070 6173 730a 2020  s should pass.  
-00001620: 2020 2020 2020 7061 7261 6d73 5b22 616c        params["al
-00001630: 6c6f 7765 645f 7570 6461 7465 7322 5d20  lowed_updates"] 
-00001640: 3d20 6a73 6f6e 2e64 756d 7073 2861 6c6c  = json.dumps(all
-00001650: 6f77 6564 5f75 7064 6174 6573 290a 2020  owed_updates).  
-00001660: 2020 6966 2069 705f 6164 6472 6573 7320    if ip_address 
-00001670: 6973 206e 6f74 204e 6f6e 653a 2020 2320  is not None:  # 
-00001680: 456d 7074 7920 7374 7269 6e67 2073 686f  Empty string sho
-00001690: 756c 6420 7061 7373 0a20 2020 2020 2020  uld pass.       
-000016a0: 2070 6172 616d 735b 2269 705f 6164 6472   params["ip_addr
-000016b0: 6573 7322 5d20 3d20 6970 5f61 6464 7265  ess"] = ip_addre
-000016c0: 7373 0a20 2020 2069 6620 6472 6f70 5f70  ss.    if drop_p
-000016d0: 656e 6469 6e67 5f75 7064 6174 6573 2069  ending_updates i
-000016e0: 7320 6e6f 7420 4e6f 6e65 3a20 2023 2041  s not None:  # A
-000016f0: 6e79 2062 6f6f 6c20 7661 6c75 6520 7368  ny bool value sh
-00001700: 6f75 6c64 2070 6173 730a 2020 2020 2020  ould pass.      
-00001710: 2020 7061 7261 6d73 5b22 6472 6f70 5f70    params["drop_p
-00001720: 656e 6469 6e67 5f75 7064 6174 6573 225d  ending_updates"]
-00001730: 203d 2064 726f 705f 7065 6e64 696e 675f   = drop_pending_
-00001740: 7570 6461 7465 730a 2020 2020 6966 2073  updates.    if s
-00001750: 6563 7265 745f 746f 6b65 6e3a 0a20 2020  ecret_token:.   
-00001760: 2020 2020 2070 6172 616d 735b 2273 6563       params["sec
-00001770: 7265 745f 746f 6b65 6e22 5d20 3d20 7365  ret_token"] = se
-00001780: 6372 6574 5f74 6f6b 656e 0a20 2020 2072  cret_token.    r
-00001790: 6574 7572 6e20 6177 6169 7420 5f72 6571  eturn await _req
-000017a0: 7565 7374 2874 6f6b 656e 2c20 726f 7574  uest(token, rout
-000017b0: 653d 2273 6574 5765 6268 6f6f 6b22 2c20  e="setWebhook", 
-000017c0: 7061 7261 6d73 3d70 6172 616d 732c 2066  params=params, f
-000017d0: 696c 6573 3d66 696c 6573 2c20 7265 7175  iles=files, requ
-000017e0: 6573 745f 7469 6d65 6f75 743d 7469 6d65  est_timeout=time
-000017f0: 6f75 7429 0a0a 0a61 7379 6e63 2064 6566  out)...async def
-00001800: 2064 656c 6574 655f 7765 6268 6f6f 6b28   delete_webhook(
-00001810: 746f 6b65 6e2c 2064 726f 705f 7065 6e64  token, drop_pend
-00001820: 696e 675f 7570 6461 7465 733d 4e6f 6e65  ing_updates=None
-00001830: 2c20 7469 6d65 6f75 743d 4e6f 6e65 293a  , timeout=None):
-00001840: 0a20 2020 206d 6574 686f 645f 7572 6c20  .    method_url 
-00001850: 3d20 7222 6465 6c65 7465 5765 6268 6f6f  = r"deleteWebhoo
-00001860: 6b22 0a20 2020 2070 6179 6c6f 6164 203d  k".    payload =
-00001870: 207b 7d0a 2020 2020 6966 2064 726f 705f   {}.    if drop_
-00001880: 7065 6e64 696e 675f 7570 6461 7465 7320  pending_updates 
-00001890: 6973 206e 6f74 204e 6f6e 653a 2020 2320  is not None:  # 
-000018a0: 416e 7920 626f 6f6c 2076 616c 7565 2073  Any bool value s
-000018b0: 686f 756c 6420 7061 7373 0a20 2020 2020  hould pass.     
-000018c0: 2020 2070 6179 6c6f 6164 5b22 6472 6f70     payload["drop
-000018d0: 5f70 656e 6469 6e67 5f75 7064 6174 6573  _pending_updates
-000018e0: 225d 203d 2064 726f 705f 7065 6e64 696e  "] = drop_pendin
-000018f0: 675f 7570 6461 7465 730a 2020 2020 6966  g_updates.    if
-00001900: 2074 696d 656f 7574 3a0a 2020 2020 2020   timeout:.      
-00001910: 2020 7061 796c 6f61 645b 2274 696d 656f    payload["timeo
-00001920: 7574 225d 203d 2074 696d 656f 7574 0a20  ut"] = timeout. 
-00001930: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00001940: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
-00001950: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
-00001960: 6d73 3d70 6179 6c6f 6164 290a 0a0a 6173  ms=payload)...as
-00001970: 796e 6320 6465 6620 6765 745f 7765 6268  ync def get_webh
-00001980: 6f6f 6b5f 696e 666f 2874 6f6b 656e 2c20  ook_info(token, 
-00001990: 7469 6d65 6f75 743d 4e6f 6e65 293a 0a20  timeout=None):. 
-000019a0: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
-000019b0: 7222 6765 7457 6562 686f 6f6b 496e 666f  r"getWebhookInfo
-000019c0: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
-000019d0: 7b7d 0a20 2020 2069 6620 7469 6d65 6f75  {}.    if timeou
-000019e0: 743a 0a20 2020 2020 2020 2070 6179 6c6f  t:.        paylo
-000019f0: 6164 5b22 7469 6d65 6f75 7422 5d20 3d20  ad["timeout"] = 
-00001a00: 7469 6d65 6f75 740a 2020 2020 7265 7475  timeout.    retu
-00001a10: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
-00001a20: 7428 746f 6b65 6e2c 206d 6574 686f 645f  t(token, method_
-00001a30: 7572 6c2c 2070 6172 616d 733d 7061 796c  url, params=payl
-00001a40: 6f61 6429 0a0a 0a61 7379 6e63 2064 6566  oad)...async def
-00001a50: 2067 6574 5f75 7064 6174 6573 280a 2020   get_updates(.  
-00001a60: 2020 746f 6b65 6e3a 2073 7472 2c0a 2020    token: str,.  
-00001a70: 2020 6f66 6673 6574 3a20 4f70 7469 6f6e    offset: Option
-00001a80: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
-00001a90: 2020 2020 6c69 6d69 743a 204f 7074 696f      limit: Optio
-00001aa0: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-00001ab0: 0a20 2020 2074 696d 656f 7574 3a20 4f70  .    timeout: Op
-00001ac0: 7469 6f6e 616c 5b66 6c6f 6174 5d20 3d20  tional[float] = 
-00001ad0: 4e6f 6e65 2c0a 2020 2020 616c 6c6f 7765  None,.    allowe
-00001ae0: 645f 7570 6461 7465 733a 204f 7074 696f  d_updates: Optio
-00001af0: 6e61 6c5b 6c69 7374 5b73 7472 5d5d 203d  nal[list[str]] =
-00001b00: 204e 6f6e 652c 0a20 2020 2072 6571 7565   None,.    reque
-00001b10: 7374 5f74 696d 656f 7574 3a20 4f70 7469  st_timeout: Opti
-00001b20: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 4e6f  onal[float] = No
-00001b30: 6e65 2c0a 293a 0a20 2020 2070 6172 616d  ne,.):.    param
-00001b40: 733a 2064 6963 7420 3d20 7b7d 0a20 2020  s: dict = {}.   
-00001b50: 2069 6620 6f66 6673 6574 3a0a 2020 2020   if offset:.    
-00001b60: 2020 2020 7061 7261 6d73 5b22 6f66 6673      params["offs
-00001b70: 6574 225d 203d 206f 6666 7365 740a 2020  et"] = offset.  
-00001b80: 2020 6966 206c 696d 6974 3a0a 2020 2020    if limit:.    
-00001b90: 2020 2020 7061 7261 6d73 5b22 6c69 6d69      params["limi
-00001ba0: 7422 5d20 3d20 6c69 6d69 740a 2020 2020  t"] = limit.    
-00001bb0: 6966 2074 696d 656f 7574 3a0a 2020 2020  if timeout:.    
-00001bc0: 2020 2020 7061 7261 6d73 5b22 7469 6d65      params["time
-00001bd0: 6f75 7422 5d20 3d20 7469 6d65 6f75 740a  out"] = timeout.
-00001be0: 2020 2020 6966 2061 6c6c 6f77 6564 5f75      if allowed_u
-00001bf0: 7064 6174 6573 3a0a 2020 2020 2020 2020  pdates:.        
-00001c00: 7061 7261 6d73 5b22 616c 6c6f 7765 645f  params["allowed_
-00001c10: 7570 6461 7465 7322 5d20 3d20 6a73 6f6e  updates"] = json
-00001c20: 2e64 756d 7073 2861 6c6c 6f77 6564 5f75  .dumps(allowed_u
-00001c30: 7064 6174 6573 290a 2020 2020 7265 7475  pdates).    retu
-00001c40: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
-00001c50: 7428 746f 6b65 6e2c 2072 6f75 7465 3d22  t(token, route="
-00001c60: 6765 7455 7064 6174 6573 222c 2070 6172  getUpdates", par
-00001c70: 616d 733d 7061 7261 6d73 2c20 7265 7175  ams=params, requ
-00001c80: 6573 745f 7469 6d65 6f75 743d 7265 7175  est_timeout=requ
-00001c90: 6573 745f 7469 6d65 6f75 7429 0a0a 0a61  est_timeout)...a
-00001ca0: 7379 6e63 2064 6566 205f 6368 6563 6b5f  sync def _check_
-00001cb0: 7265 7370 6f6e 7365 2872 6573 706f 6e73  response(respons
-00001cc0: 653a 2061 696f 6874 7470 2e43 6c69 656e  e: aiohttp.Clien
-00001cd0: 7452 6573 706f 6e73 6529 3a0a 2020 2020  tResponse):.    
-00001ce0: 2222 220a 2020 2020 4368 6563 6b73 2077  """.    Checks w
-00001cf0: 6865 7468 6572 2060 7265 7375 6c74 6020  hether `result` 
-00001d00: 6973 2061 2076 616c 6964 2041 5049 2072  is a valid API r
-00001d10: 6573 706f 6e73 652e 0a20 2020 2041 2072  esponse..    A r
-00001d20: 6573 756c 7420 6973 2063 6f6e 7369 6465  esult is conside
-00001d30: 7265 6420 696e 7661 6c69 6420 6966 3a0a  red invalid if:.
-00001d40: 2020 2020 2020 2020 2d20 5468 6520 7365          - The se
-00001d50: 7276 6572 2072 6574 7572 6e65 6420 616e  rver returned an
-00001d60: 2048 5454 5020 7265 7370 6f6e 7365 2063   HTTP response c
-00001d70: 6f64 6520 6f74 6865 7220 7468 616e 2032  ode other than 2
-00001d80: 3030 0a20 2020 2020 2020 202d 2054 6865  00.        - The
-00001d90: 2063 6f6e 7465 6e74 206f 6620 7468 6520   content of the 
-00001da0: 7265 7375 6c74 2069 7320 696e 7661 6c69  result is invali
-00001db0: 6420 4a53 4f4e 2e0a 2020 2020 2020 2020  d JSON..        
-00001dc0: 2d20 5468 6520 6d65 7468 6f64 2063 616c  - The method cal
-00001dd0: 6c20 7761 7320 756e 7375 6363 6573 7366  l was unsuccessf
-00001de0: 756c 2028 5468 6520 4a53 4f4e 2027 6f6b  ul (The JSON 'ok
-00001df0: 2720 6669 656c 6420 6571 7561 6c73 2046  ' field equals F
-00001e00: 616c 7365 290a 0a20 2020 203a 7261 6973  alse)..    :rais
-00001e10: 6573 2041 7069 4578 6365 7074 696f 6e3a  es ApiException:
-00001e20: 2069 6620 6f6e 6520 6f66 2074 6865 2061   if one of the a
-00001e30: 626f 7665 206c 6973 7465 6420 6361 7365  bove listed case
-00001e40: 7320 6973 2061 7070 6c69 6361 626c 650a  s is applicable.
-00001e50: 2020 2020 3a70 6172 616d 206d 6574 686f      :param metho
-00001e60: 645f 6e61 6d65 3a20 5468 6520 6e61 6d65  d_name: The name
-00001e70: 206f 6620 7468 6520 6d65 7468 6f64 2063   of the method c
-00001e80: 616c 6c65 640a 2020 2020 3a70 6172 616d  alled.    :param
-00001e90: 2072 6573 756c 743a 2054 6865 2072 6574   result: The ret
-00001ea0: 7572 6e65 6420 7265 7375 6c74 206f 6620  urned result of 
-00001eb0: 7468 6520 6d65 7468 6f64 2072 6571 7565  the method reque
-00001ec0: 7374 0a20 2020 203a 7265 7475 726e 3a20  st.    :return: 
-00001ed0: 5468 6520 7265 7375 6c74 2070 6172 7365  The result parse
-00001ee0: 6420 746f 2061 204a 534f 4e20 6469 6374  d to a JSON dict
-00001ef0: 696f 6e61 7279 2e0a 2020 2020 2222 220a  ionary..    """.
-00001f00: 2020 2020 6177 6169 7420 7265 7370 6f6e      await respon
-00001f10: 7365 2e74 6578 7428 2920 2023 206c 6f61  se.text()  # loa
-00001f20: 6469 6e67 2072 6573 706f 6e73 6520 626f  ding response bo
-00001f30: 6479 0a20 2020 2074 7279 3a0a 2020 2020  dy.    try:.    
-00001f40: 2020 2020 7265 7375 6c74 5f6a 736f 6e20      result_json 
-00001f50: 3d20 6177 6169 7420 7265 7370 6f6e 7365  = await response
-00001f60: 2e6a 736f 6e28 656e 636f 6469 6e67 3d22  .json(encoding="
-00001f70: 7574 662d 3822 290a 2020 2020 6578 6365  utf-8").    exce
-00001f80: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00001f90: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
-00001fa0: 2041 7069 496e 7661 6c69 644a 534f 4e45   ApiInvalidJSONE
-00001fb0: 7863 6570 7469 6f6e 2872 6573 706f 6e73  xception(respons
-00001fc0: 652c 2065 290a 2020 2020 6966 206e 6f74  e, e).    if not
-00001fd0: 2069 7369 6e73 7461 6e63 6528 7265 7375   isinstance(resu
-00001fe0: 6c74 5f6a 736f 6e2c 2064 6963 7429 206f  lt_json, dict) o
-00001ff0: 7220 226f 6b22 206e 6f74 2069 6e20 7265  r "ok" not in re
-00002000: 7375 6c74 5f6a 736f 6e3a 0a20 2020 2020  sult_json:.     
-00002010: 2020 2072 6169 7365 2041 7069 4854 5450     raise ApiHTTP
-00002020: 4578 6365 7074 696f 6e28 6622 4a53 4f4e  Exception(f"JSON
-00002030: 2072 6573 706f 6e73 6520 6973 206d 616c   response is mal
-00002040: 666f 726d 6564 3a20 7b72 6573 756c 745f  formed: {result_
-00002050: 6a73 6f6e 7d22 2c20 7265 7370 6f6e 7365  json}", response
-00002060: 290a 2020 2020 6966 2072 6573 756c 745f  ).    if result_
-00002070: 6a73 6f6e 5b22 6f6b 225d 2069 7320 5472  json["ok"] is Tr
-00002080: 7565 3a0a 2020 2020 2020 2020 7265 7475  ue:.        retu
-00002090: 726e 2072 6573 756c 745f 6a73 6f6e 0a20  rn result_json. 
-000020a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000020b0: 2069 6620 2264 6573 6372 6970 7469 6f6e   if "description
-000020c0: 2220 6e6f 7420 696e 2072 6573 756c 745f  " not in result_
-000020d0: 6a73 6f6e 3a0a 2020 2020 2020 2020 2020  json:.          
-000020e0: 2020 7261 6973 6520 4170 6948 5454 5045    raise ApiHTTPE
-000020f0: 7863 6570 7469 6f6e 2866 224a 534f 4e20  xception(f"JSON 
-00002100: 7265 7370 6f6e 7365 206d 6973 7365 7320  response misses 
-00002110: 2764 6573 6372 6970 7469 6f6e 2720 6669  'description' fi
-00002120: 656c 643a 207b 7265 7375 6c74 5f6a 736f  eld: {result_jso
-00002130: 6e7d 222c 2072 6573 706f 6e73 6529 0a20  n}", response). 
-00002140: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00002150: 2020 2020 2020 2020 2072 6169 7365 2041           raise A
-00002160: 7069 4854 5450 4578 6365 7074 696f 6e28  piHTTPException(
-00002170: 7265 7375 6c74 5f6a 736f 6e5b 2264 6573  result_json["des
-00002180: 6372 6970 7469 6f6e 225d 2c20 7265 7370  cription"], resp
-00002190: 6f6e 7365 290a 0a0a 6465 6620 5f61 6464  onse)...def _add
-000021a0: 5f6d 6573 7361 6765 5f74 6872 6561 645f  _message_thread_
-000021b0: 6964 2870 6172 616d 733a 2044 6963 745b  id(params: Dict[
-000021c0: 7374 722c 2041 6e79 5d2c 206d 6573 7361  str, Any], messa
-000021d0: 6765 5f74 6872 6561 645f 6964 3a20 4f70  ge_thread_id: Op
-000021e0: 7469 6f6e 616c 5b69 6e74 5d29 202d 3e20  tional[int]) -> 
-000021f0: 4e6f 6e65 3a0a 2020 2020 6966 206d 6573  None:.    if mes
-00002200: 7361 6765 5f74 6872 6561 645f 6964 2069  sage_thread_id i
-00002210: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00002220: 2020 2020 7061 7261 6d73 5b22 6d65 7373      params["mess
-00002230: 6167 655f 7468 7265 6164 5f69 6422 5d20  age_thread_id"] 
-00002240: 3d20 6d65 7373 6167 655f 7468 7265 6164  = message_thread
-00002250: 5f69 640a 0a0a 6173 796e 6320 6465 6620  _id...async def 
-00002260: 7365 6e64 5f6d 6573 7361 6765 280a 2020  send_message(.  
-00002270: 2020 746f 6b65 6e2c 0a20 2020 2063 6861    token,.    cha
-00002280: 745f 6964 2c0a 2020 2020 7465 7874 2c0a  t_id,.    text,.
-00002290: 2020 2020 6469 7361 626c 655f 7765 625f      disable_web_
-000022a0: 7061 6765 5f70 7265 7669 6577 3d4e 6f6e  page_preview=Non
-000022b0: 652c 0a20 2020 2072 6570 6c79 5f74 6f5f  e,.    reply_to_
-000022c0: 6d65 7373 6167 655f 6964 3d4e 6f6e 652c  message_id=None,
-000022d0: 0a20 2020 2072 6570 6c79 5f6d 6172 6b75  .    reply_marku
-000022e0: 703d 4e6f 6e65 2c0a 2020 2020 7061 7273  p=None,.    pars
-000022f0: 655f 6d6f 6465 3d4e 6f6e 652c 0a20 2020  e_mode=None,.   
-00002300: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
-00002310: 6174 696f 6e3d 4e6f 6e65 2c0a 2020 2020  ation=None,.    
-00002320: 7469 6d65 6f75 743d 4e6f 6e65 2c0a 2020  timeout=None,.  
-00002330: 2020 656e 7469 7469 6573 3d4e 6f6e 652c    entities=None,
-00002340: 0a20 2020 2061 6c6c 6f77 5f73 656e 6469  .    allow_sendi
-00002350: 6e67 5f77 6974 686f 7574 5f72 6570 6c79  ng_without_reply
-00002360: 3d4e 6f6e 652c 0a20 2020 2070 726f 7465  =None,.    prote
-00002370: 6374 5f63 6f6e 7465 6e74 3d4e 6f6e 652c  ct_content=None,
-00002380: 0a20 2020 206d 6573 7361 6765 5f74 6872  .    message_thr
-00002390: 6561 645f 6964 3a20 4f70 7469 6f6e 616c  ead_id: Optional
-000023a0: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 293a  [int] = None,.):
-000023b0: 0a20 2020 2022 2222 0a20 2020 2055 7365  .    """.    Use
-000023c0: 2074 6869 7320 6d65 7468 6f64 2074 6f20   this method to 
-000023d0: 7365 6e64 2074 6578 7420 6d65 7373 6167  send text messag
-000023e0: 6573 2e20 4f6e 2073 7563 6365 7373 2c20  es. On success, 
-000023f0: 7468 6520 7365 6e74 204d 6573 7361 6765  the sent Message
-00002400: 2069 7320 7265 7475 726e 6564 2e0a 2020   is returned..  
-00002410: 2020 3a70 6172 616d 2074 6f6b 656e 3a0a    :param token:.
-00002420: 2020 2020 3a70 6172 616d 2063 6861 745f      :param chat_
-00002430: 6964 3a0a 2020 2020 3a70 6172 616d 2074  id:.    :param t
-00002440: 6578 743a 0a20 2020 203a 7061 7261 6d20  ext:.    :param 
-00002450: 6469 7361 626c 655f 7765 625f 7061 6765  disable_web_page
-00002460: 5f70 7265 7669 6577 3a0a 2020 2020 3a70  _preview:.    :p
-00002470: 6172 616d 2072 6570 6c79 5f74 6f5f 6d65  aram reply_to_me
-00002480: 7373 6167 655f 6964 3a0a 2020 2020 3a70  ssage_id:.    :p
-00002490: 6172 616d 2072 6570 6c79 5f6d 6172 6b75  aram reply_marku
-000024a0: 703a 0a20 2020 203a 7061 7261 6d20 7061  p:.    :param pa
-000024b0: 7273 655f 6d6f 6465 3a0a 2020 2020 3a70  rse_mode:.    :p
-000024c0: 6172 616d 2064 6973 6162 6c65 5f6e 6f74  aram disable_not
-000024d0: 6966 6963 6174 696f 6e3a 0a20 2020 203a  ification:.    :
-000024e0: 7061 7261 6d20 7469 6d65 6f75 743a 0a20  param timeout:. 
-000024f0: 2020 203a 7061 7261 6d20 656e 7469 7469     :param entiti
-00002500: 6573 3a0a 2020 2020 3a70 6172 616d 2061  es:.    :param a
-00002510: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
-00002520: 686f 7574 5f72 6570 6c79 3a0a 2020 2020  hout_reply:.    
-00002530: 3a70 6172 616d 2070 726f 7465 6374 5f63  :param protect_c
-00002540: 6f6e 7465 6e74 3a0a 2020 2020 3a72 6574  ontent:.    :ret
-00002550: 7572 6e3a 0a20 2020 2022 2222 0a20 2020  urn:.    """.   
-00002560: 206d 6574 686f 645f 6e61 6d65 203d 2022   method_name = "
-00002570: 7365 6e64 4d65 7373 6167 6522 0a20 2020  sendMessage".   
-00002580: 2070 6172 616d 7320 3d20 7b22 6368 6174   params = {"chat
-00002590: 5f69 6422 3a20 7374 7228 6368 6174 5f69  _id": str(chat_i
-000025a0: 6429 2c20 2274 6578 7422 3a20 7465 7874  d), "text": text
-000025b0: 7d0a 2020 2020 6966 2064 6973 6162 6c65  }.    if disable
-000025c0: 5f77 6562 5f70 6167 655f 7072 6576 6965  _web_page_previe
-000025d0: 7720 6973 206e 6f74 204e 6f6e 653a 0a20  w is not None:. 
-000025e0: 2020 2020 2020 2070 6172 616d 735b 2264         params["d
-000025f0: 6973 6162 6c65 5f77 6562 5f70 6167 655f  isable_web_page_
-00002600: 7072 6576 6965 7722 5d20 3d20 6469 7361  preview"] = disa
-00002610: 626c 655f 7765 625f 7061 6765 5f70 7265  ble_web_page_pre
-00002620: 7669 6577 0a20 2020 2069 6620 7265 706c  view.    if repl
-00002630: 795f 746f 5f6d 6573 7361 6765 5f69 643a  y_to_message_id:
-00002640: 0a20 2020 2020 2020 2070 6172 616d 735b  .        params[
-00002650: 2272 6570 6c79 5f74 6f5f 6d65 7373 6167  "reply_to_messag
-00002660: 655f 6964 225d 203d 2072 6570 6c79 5f74  e_id"] = reply_t
-00002670: 6f5f 6d65 7373 6167 655f 6964 0a20 2020  o_message_id.   
-00002680: 2069 6620 7265 706c 795f 6d61 726b 7570   if reply_markup
-00002690: 3a0a 2020 2020 2020 2020 7061 7261 6d73  :.        params
-000026a0: 5b22 7265 706c 795f 6d61 726b 7570 225d  ["reply_markup"]
-000026b0: 203d 2061 7761 6974 205f 636f 6e76 6572   = await _conver
-000026c0: 745f 6d61 726b 7570 2872 6570 6c79 5f6d  t_markup(reply_m
-000026d0: 6172 6b75 7029 0a20 2020 2069 6620 7061  arkup).    if pa
-000026e0: 7273 655f 6d6f 6465 3a0a 2020 2020 2020  rse_mode:.      
-000026f0: 2020 7061 7261 6d73 5b22 7061 7273 655f    params["parse_
-00002700: 6d6f 6465 225d 203d 2070 6172 7365 5f6d  mode"] = parse_m
-00002710: 6f64 650a 2020 2020 6966 2064 6973 6162  ode.    if disab
-00002720: 6c65 5f6e 6f74 6966 6963 6174 696f 6e20  le_notification 
-00002730: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00002740: 2020 2020 2070 6172 616d 735b 2264 6973       params["dis
-00002750: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-00002760: 6e22 5d20 3d20 6469 7361 626c 655f 6e6f  n"] = disable_no
-00002770: 7469 6669 6361 7469 6f6e 0a20 2020 2069  tification.    i
-00002780: 6620 7469 6d65 6f75 743a 0a20 2020 2020  f timeout:.     
-00002790: 2020 2070 6172 616d 735b 2274 696d 656f     params["timeo
-000027a0: 7574 225d 203d 2074 696d 656f 7574 0a20  ut"] = timeout. 
-000027b0: 2020 2069 6620 656e 7469 7469 6573 3a0a     if entities:.
-000027c0: 2020 2020 2020 2020 7061 7261 6d73 5b22          params["
-000027d0: 656e 7469 7469 6573 225d 203d 206a 736f  entities"] = jso
-000027e0: 6e2e 6475 6d70 7328 7479 7065 732e 4d65  n.dumps(types.Me
-000027f0: 7373 6167 6545 6e74 6974 792e 746f 5f6c  ssageEntity.to_l
-00002800: 6973 745f 6f66 5f64 6963 7473 2865 6e74  ist_of_dicts(ent
-00002810: 6974 6965 7329 290a 2020 2020 6966 2061  ities)).    if a
-00002820: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
-00002830: 686f 7574 5f72 6570 6c79 2069 7320 6e6f  hout_reply is no
-00002840: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00002850: 7061 7261 6d73 5b22 616c 6c6f 775f 7365  params["allow_se
-00002860: 6e64 696e 675f 7769 7468 6f75 745f 7265  nding_without_re
-00002870: 706c 7922 5d20 3d20 616c 6c6f 775f 7365  ply"] = allow_se
-00002880: 6e64 696e 675f 7769 7468 6f75 745f 7265  nding_without_re
-00002890: 706c 790a 2020 2020 6966 2070 726f 7465  ply.    if prote
-000028a0: 6374 5f63 6f6e 7465 6e74 2069 7320 6e6f  ct_content is no
-000028b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000028c0: 7061 7261 6d73 5b22 7072 6f74 6563 745f  params["protect_
-000028d0: 636f 6e74 656e 7422 5d20 3d20 7072 6f74  content"] = prot
-000028e0: 6563 745f 636f 6e74 656e 740a 2020 2020  ect_content.    
-000028f0: 5f61 6464 5f6d 6573 7361 6765 5f74 6872  _add_message_thr
-00002900: 6561 645f 6964 2870 6172 616d 732c 206d  ead_id(params, m
-00002910: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
-00002920: 290a 2020 2020 7265 7475 726e 2061 7761  ).    return awa
-00002930: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
-00002940: 6e2c 206d 6574 686f 645f 6e61 6d65 2c20  n, method_name, 
-00002950: 7061 7261 6d73 3d70 6172 616d 7329 0a0a  params=params)..
-00002960: 0a23 206d 6574 686f 6473 0a0a 0a61 7379  .# methods...asy
-00002970: 6e63 2064 6566 2067 6574 5f75 7365 725f  nc def get_user_
-00002980: 7072 6f66 696c 655f 7068 6f74 6f73 2874  profile_photos(t
-00002990: 6f6b 656e 2c20 7573 6572 5f69 642c 206f  oken, user_id, o
-000029a0: 6666 7365 743d 4e6f 6e65 2c20 6c69 6d69  ffset=None, limi
-000029b0: 743d 4e6f 6e65 293a 0a20 2020 206d 6574  t=None):.    met
-000029c0: 686f 645f 7572 6c20 3d20 7222 6765 7455  hod_url = r"getU
-000029d0: 7365 7250 726f 6669 6c65 5068 6f74 6f73  serProfilePhotos
-000029e0: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
-000029f0: 7b22 7573 6572 5f69 6422 3a20 7573 6572  {"user_id": user
-00002a00: 5f69 647d 0a20 2020 2069 6620 6f66 6673  _id}.    if offs
-00002a10: 6574 3a0a 2020 2020 2020 2020 7061 796c  et:.        payl
-00002a20: 6f61 645b 226f 6666 7365 7422 5d20 3d20  oad["offset"] = 
-00002a30: 6f66 6673 6574 0a20 2020 2069 6620 6c69  offset.    if li
-00002a40: 6d69 743a 0a20 2020 2020 2020 2070 6179  mit:.        pay
-00002a50: 6c6f 6164 5b22 6c69 6d69 7422 5d20 3d20  load["limit"] = 
-00002a60: 6c69 6d69 740a 2020 2020 7265 7475 726e  limit.    return
-00002a70: 2061 7761 6974 205f 7265 7175 6573 7428   await _request(
-00002a80: 746f 6b65 6e2c 206d 6574 686f 645f 7572  token, method_ur
-00002a90: 6c2c 2070 6172 616d 733d 7061 796c 6f61  l, params=payloa
-00002aa0: 6429 0a0a 0a61 7379 6e63 2064 6566 2067  d)...async def g
-00002ab0: 6574 5f63 6861 7428 746f 6b65 6e2c 2063  et_chat(token, c
-00002ac0: 6861 745f 6964 293a 0a20 2020 206d 6574  hat_id):.    met
-00002ad0: 686f 645f 7572 6c20 3d20 7222 6765 7443  hod_url = r"getC
-00002ae0: 6861 7422 0a20 2020 2070 6179 6c6f 6164  hat".    payload
-00002af0: 203d 207b 2263 6861 745f 6964 223a 2063   = {"chat_id": c
-00002b00: 6861 745f 6964 7d0a 2020 2020 7265 7475  hat_id}.    retu
-00002b10: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
-00002b20: 7428 746f 6b65 6e2c 206d 6574 686f 645f  t(token, method_
-00002b30: 7572 6c2c 2070 6172 616d 733d 7061 796c  url, params=payl
-00002b40: 6f61 6429 0a0a 0a61 7379 6e63 2064 6566  oad)...async def
-00002b50: 206c 6561 7665 5f63 6861 7428 746f 6b65   leave_chat(toke
-00002b60: 6e2c 2063 6861 745f 6964 293a 0a20 2020  n, chat_id):.   
-00002b70: 206d 6574 686f 645f 7572 6c20 3d20 7222   method_url = r"
-00002b80: 6c65 6176 6543 6861 7422 0a20 2020 2070  leaveChat".    p
-00002b90: 6179 6c6f 6164 203d 207b 2263 6861 745f  ayload = {"chat_
-00002ba0: 6964 223a 2063 6861 745f 6964 7d0a 2020  id": chat_id}.  
-00002bb0: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
-00002bc0: 7265 7175 6573 7428 746f 6b65 6e2c 206d  request(token, m
-00002bd0: 6574 686f 645f 7572 6c2c 2070 6172 616d  ethod_url, param
-00002be0: 733d 7061 796c 6f61 6429 0a0a 0a61 7379  s=payload)...asy
-00002bf0: 6e63 2064 6566 2067 6574 5f63 6861 745f  nc def get_chat_
-00002c00: 6164 6d69 6e69 7374 7261 746f 7273 2874  administrators(t
-00002c10: 6f6b 656e 2c20 6368 6174 5f69 6429 3a0a  oken, chat_id):.
-00002c20: 2020 2020 6d65 7468 6f64 5f75 726c 203d      method_url =
-00002c30: 2072 2267 6574 4368 6174 4164 6d69 6e69   r"getChatAdmini
-00002c40: 7374 7261 746f 7273 220a 2020 2020 7061  strators".    pa
-00002c50: 796c 6f61 6420 3d20 7b22 6368 6174 5f69  yload = {"chat_i
-00002c60: 6422 3a20 6368 6174 5f69 647d 0a20 2020  d": chat_id}.   
-00002c70: 2072 6574 7572 6e20 6177 6169 7420 5f72   return await _r
-00002c80: 6571 7565 7374 2874 6f6b 656e 2c20 6d65  equest(token, me
-00002c90: 7468 6f64 5f75 726c 2c20 7061 7261 6d73  thod_url, params
-00002ca0: 3d70 6179 6c6f 6164 290a 0a0a 6173 796e  =payload)...asyn
-00002cb0: 6320 6465 6620 6765 745f 6368 6174 5f6d  c def get_chat_m
-00002cc0: 656d 6265 725f 636f 756e 7428 746f 6b65  ember_count(toke
-00002cd0: 6e2c 2063 6861 745f 6964 293a 0a20 2020  n, chat_id):.   
-00002ce0: 206d 6574 686f 645f 7572 6c20 3d20 7222   method_url = r"
-00002cf0: 6765 7443 6861 744d 656d 6265 7243 6f75  getChatMemberCou
-00002d00: 6e74 220a 2020 2020 7061 796c 6f61 6420  nt".    payload 
-00002d10: 3d20 7b22 6368 6174 5f69 6422 3a20 6368  = {"chat_id": ch
-00002d20: 6174 5f69 647d 0a20 2020 2072 6574 7572  at_id}.    retur
-00002d30: 6e20 6177 6169 7420 5f72 6571 7565 7374  n await _request
-00002d40: 2874 6f6b 656e 2c20 6d65 7468 6f64 5f75  (token, method_u
-00002d50: 726c 2c20 7061 7261 6d73 3d70 6179 6c6f  rl, params=paylo
-00002d60: 6164 290a 0a0a 6173 796e 6320 6465 6620  ad)...async def 
-00002d70: 7365 745f 7374 6963 6b65 725f 7365 745f  set_sticker_set_
-00002d80: 7468 756d 6228 746f 6b65 6e2c 206e 616d  thumb(token, nam
-00002d90: 652c 2075 7365 725f 6964 2c20 7468 756d  e, user_id, thum
-00002da0: 6229 3a0a 2020 2020 6d65 7468 6f64 5f75  b):.    method_u
-00002db0: 726c 203d 2072 2273 6574 5374 6963 6b65  rl = r"setSticke
-00002dc0: 7253 6574 5468 756d 6222 0a20 2020 2070  rSetThumb".    p
-00002dd0: 6179 6c6f 6164 203d 207b 226e 616d 6522  ayload = {"name"
-00002de0: 3a20 6e61 6d65 2c20 2275 7365 725f 6964  : name, "user_id
-00002df0: 223a 2075 7365 725f 6964 7d0a 2020 2020  ": user_id}.    
-00002e00: 6669 6c65 7320 3d20 7b7d 0a20 2020 2069  files = {}.    i
-00002e10: 6620 7468 756d 623a 0a20 2020 2020 2020  f thumb:.       
-00002e20: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-00002e30: 6365 2874 6875 6d62 2c20 7374 7229 3a0a  ce(thumb, str):.
-00002e40: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00002e50: 735b 2274 6875 6d62 225d 203d 2074 6875  s["thumb"] = thu
-00002e60: 6d62 0a20 2020 2020 2020 2065 6c73 653a  mb.        else:
-00002e70: 0a20 2020 2020 2020 2020 2020 2070 6179  .            pay
-00002e80: 6c6f 6164 5b22 7468 756d 6222 5d20 3d20  load["thumb"] = 
-00002e90: 7468 756d 620a 2020 2020 7265 7475 726e  thumb.    return
-00002ea0: 2061 7761 6974 205f 7265 7175 6573 7428   await _request(
-00002eb0: 746f 6b65 6e2c 206d 6574 686f 645f 7572  token, method_ur
-00002ec0: 6c2c 2070 6172 616d 733d 7061 796c 6f61  l, params=payloa
-00002ed0: 642c 2066 696c 6573 3d66 696c 6573 206f  d, files=files o
-00002ee0: 7220 4e6f 6e65 290a 0a0a 6173 796e 6320  r None)...async 
-00002ef0: 6465 6620 7365 745f 6368 6174 5f73 7469  def set_chat_sti
-00002f00: 636b 6572 5f73 6574 2874 6f6b 656e 2c20  cker_set(token, 
-00002f10: 6368 6174 5f69 642c 2073 7469 636b 6572  chat_id, sticker
-00002f20: 5f73 6574 5f6e 616d 6529 3a0a 2020 2020  _set_name):.    
-00002f30: 6d65 7468 6f64 5f75 726c 203d 2072 2273  method_url = r"s
-00002f40: 6574 4368 6174 5374 6963 6b65 7253 6574  etChatStickerSet
-00002f50: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
-00002f60: 7b22 6368 6174 5f69 6422 3a20 6368 6174  {"chat_id": chat
-00002f70: 5f69 642c 2022 7374 6963 6b65 725f 7365  _id, "sticker_se
-00002f80: 745f 6e61 6d65 223a 2073 7469 636b 6572  t_name": sticker
-00002f90: 5f73 6574 5f6e 616d 657d 0a20 2020 2072  _set_name}.    r
-00002fa0: 6574 7572 6e20 6177 6169 7420 5f72 6571  eturn await _req
-00002fb0: 7565 7374 2874 6f6b 656e 2c20 6d65 7468  uest(token, meth
-00002fc0: 6f64 5f75 726c 2c20 7061 7261 6d73 3d70  od_url, params=p
-00002fd0: 6179 6c6f 6164 290a 0a0a 6173 796e 6320  ayload)...async 
-00002fe0: 6465 6620 6465 6c65 7465 5f63 6861 745f  def delete_chat_
-00002ff0: 7374 6963 6b65 725f 7365 7428 746f 6b65  sticker_set(toke
-00003000: 6e2c 2063 6861 745f 6964 293a 0a20 2020  n, chat_id):.   
-00003010: 206d 6574 686f 645f 7572 6c20 3d20 7222   method_url = r"
-00003020: 6465 6c65 7465 4368 6174 5374 6963 6b65  deleteChatSticke
-00003030: 7253 6574 220a 2020 2020 7061 796c 6f61  rSet".    payloa
-00003040: 6420 3d20 7b22 6368 6174 5f69 6422 3a20  d = {"chat_id": 
-00003050: 6368 6174 5f69 647d 0a20 2020 2072 6574  chat_id}.    ret
-00003060: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
-00003070: 7374 2874 6f6b 656e 2c20 6d65 7468 6f64  st(token, method
-00003080: 5f75 726c 2c20 7061 7261 6d73 3d70 6179  _url, params=pay
-00003090: 6c6f 6164 290a 0a0a 6173 796e 6320 6465  load)...async de
-000030a0: 6620 616e 7377 6572 5f77 6562 5f61 7070  f answer_web_app
-000030b0: 5f71 7565 7279 2874 6f6b 656e 2c20 7765  _query(token, we
-000030c0: 625f 6170 705f 7175 6572 795f 6964 2c20  b_app_query_id, 
-000030d0: 7265 7375 6c74 3a20 7479 7065 732e 496e  result: types.In
-000030e0: 6c69 6e65 5175 6572 7952 6573 756c 7442  lineQueryResultB
-000030f0: 6173 6529 3a0a 2020 2020 6d65 7468 6f64  ase):.    method
-00003100: 5f75 726c 203d 2022 616e 7377 6572 5765  _url = "answerWe
-00003110: 6241 7070 5175 6572 7922 0a20 2020 2070  bAppQuery".    p
-00003120: 6179 6c6f 6164 203d 207b 2277 6562 5f61  ayload = {"web_a
-00003130: 7070 5f71 7565 7279 5f69 6422 3a20 7765  pp_query_id": we
-00003140: 625f 6170 705f 7175 6572 795f 6964 2c20  b_app_query_id, 
-00003150: 2272 6573 756c 7422 3a20 7265 7375 6c74  "result": result
-00003160: 2e74 6f5f 6a73 6f6e 2829 7d0a 2020 2020  .to_json()}.    
-00003170: 7265 7475 726e 2061 7761 6974 205f 7265  return await _re
-00003180: 7175 6573 7428 746f 6b65 6e2c 206d 6574  quest(token, met
-00003190: 686f 645f 7572 6c2c 2070 6172 616d 733d  hod_url, params=
-000031a0: 7061 796c 6f61 642c 206d 6574 686f 643d  payload, method=
-000031b0: 2270 6f73 7422 290a 0a0a 6173 796e 6320  "post")...async 
-000031c0: 6465 6620 6765 745f 6368 6174 5f6d 656d  def get_chat_mem
-000031d0: 6265 7228 746f 6b65 6e2c 2063 6861 745f  ber(token, chat_
-000031e0: 6964 2c20 7573 6572 5f69 6429 3a0a 2020  id, user_id):.  
-000031f0: 2020 6d65 7468 6f64 5f75 726c 203d 2072    method_url = r
-00003200: 2267 6574 4368 6174 4d65 6d62 6572 220a  "getChatMember".
-00003210: 2020 2020 7061 796c 6f61 6420 3d20 7b22      payload = {"
-00003220: 6368 6174 5f69 6422 3a20 6368 6174 5f69  chat_id": chat_i
-00003230: 642c 2022 7573 6572 5f69 6422 3a20 7573  d, "user_id": us
-00003240: 6572 5f69 647d 0a20 2020 2072 6574 7572  er_id}.    retur
-00003250: 6e20 6177 6169 7420 5f72 6571 7565 7374  n await _request
-00003260: 2874 6f6b 656e 2c20 6d65 7468 6f64 5f75  (token, method_u
-00003270: 726c 2c20 7061 7261 6d73 3d70 6179 6c6f  rl, params=paylo
-00003280: 6164 290a 0a0a 6173 796e 6320 6465 6620  ad)...async def 
-00003290: 666f 7277 6172 645f 6d65 7373 6167 6528  forward_message(
-000032a0: 0a20 2020 2074 6f6b 656e 2c0a 2020 2020  .    token,.    
-000032b0: 6368 6174 5f69 642c 0a20 2020 2066 726f  chat_id,.    fro
-000032c0: 6d5f 6368 6174 5f69 642c 0a20 2020 206d  m_chat_id,.    m
-000032d0: 6573 7361 6765 5f69 642c 0a20 2020 2064  essage_id,.    d
-000032e0: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
-000032f0: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 7469  ion=None,.    ti
-00003300: 6d65 6f75 743d 4e6f 6e65 2c0a 2020 2020  meout=None,.    
-00003310: 7072 6f74 6563 745f 636f 6e74 656e 743d  protect_content=
-00003320: 4e6f 6e65 2c0a 2020 2020 6d65 7373 6167  None,.    messag
-00003330: 655f 7468 7265 6164 5f69 643a 204f 7074  e_thread_id: Opt
-00003340: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00003350: 652c 0a29 3a0a 2020 2020 6d65 7468 6f64  e,.):.    method
-00003360: 5f75 726c 203d 2072 2266 6f72 7761 7264  _url = r"forward
-00003370: 4d65 7373 6167 6522 0a20 2020 2070 6179  Message".    pay
-00003380: 6c6f 6164 203d 207b 0a20 2020 2020 2020  load = {.       
-00003390: 2022 6368 6174 5f69 6422 3a20 6368 6174   "chat_id": chat
-000033a0: 5f69 642c 0a20 2020 2020 2020 2022 6672  _id,.        "fr
-000033b0: 6f6d 5f63 6861 745f 6964 223a 2066 726f  om_chat_id": fro
-000033c0: 6d5f 6368 6174 5f69 642c 0a20 2020 2020  m_chat_id,.     
-000033d0: 2020 2022 6d65 7373 6167 655f 6964 223a     "message_id":
-000033e0: 206d 6573 7361 6765 5f69 642c 0a20 2020   message_id,.   
-000033f0: 207d 0a20 2020 2069 6620 6469 7361 626c   }.    if disabl
-00003400: 655f 6e6f 7469 6669 6361 7469 6f6e 2069  e_notification i
-00003410: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00003420: 2020 2020 7061 796c 6f61 645b 2264 6973      payload["dis
-00003430: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-00003440: 6e22 5d20 3d20 6469 7361 626c 655f 6e6f  n"] = disable_no
-00003450: 7469 6669 6361 7469 6f6e 0a20 2020 2069  tification.    i
-00003460: 6620 7469 6d65 6f75 743a 0a20 2020 2020  f timeout:.     
-00003470: 2020 2070 6179 6c6f 6164 5b22 7469 6d65     payload["time
-00003480: 6f75 7422 5d20 3d20 7469 6d65 6f75 740a  out"] = timeout.
-00003490: 2020 2020 6966 2070 726f 7465 6374 5f63      if protect_c
-000034a0: 6f6e 7465 6e74 2069 7320 6e6f 7420 4e6f  ontent is not No
-000034b0: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
-000034c0: 6f61 645b 2270 726f 7465 6374 5f63 6f6e  oad["protect_con
-000034d0: 7465 6e74 225d 203d 2070 726f 7465 6374  tent"] = protect
-000034e0: 5f63 6f6e 7465 6e74 0a20 2020 205f 6164  _content.    _ad
-000034f0: 645f 6d65 7373 6167 655f 7468 7265 6164  d_message_thread
-00003500: 5f69 6428 7061 796c 6f61 642c 206d 6573  _id(payload, mes
-00003510: 7361 6765 5f74 6872 6561 645f 6964 290a  sage_thread_id).
-00003520: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-00003530: 205f 7265 7175 6573 7428 746f 6b65 6e2c   _request(token,
-00003540: 206d 6574 686f 645f 7572 6c2c 2070 6172   method_url, par
-00003550: 616d 733d 7061 796c 6f61 6429 0a0a 0a61  ams=payload)...a
-00003560: 7379 6e63 2064 6566 2063 6f70 795f 6d65  sync def copy_me
-00003570: 7373 6167 6528 0a20 2020 2074 6f6b 656e  ssage(.    token
-00003580: 2c0a 2020 2020 6368 6174 5f69 642c 0a20  ,.    chat_id,. 
-00003590: 2020 2066 726f 6d5f 6368 6174 5f69 642c     from_chat_id,
-000035a0: 0a20 2020 206d 6573 7361 6765 5f69 642c  .    message_id,
-000035b0: 0a20 2020 2063 6170 7469 6f6e 3d4e 6f6e  .    caption=Non
-000035c0: 652c 0a20 2020 2070 6172 7365 5f6d 6f64  e,.    parse_mod
-000035d0: 653d 4e6f 6e65 2c0a 2020 2020 6361 7074  e=None,.    capt
-000035e0: 696f 6e5f 656e 7469 7469 6573 3d4e 6f6e  ion_entities=Non
-000035f0: 652c 0a20 2020 2064 6973 6162 6c65 5f6e  e,.    disable_n
-00003600: 6f74 6966 6963 6174 696f 6e3d 4e6f 6e65  otification=None
-00003610: 2c0a 2020 2020 7265 706c 795f 746f 5f6d  ,.    reply_to_m
-00003620: 6573 7361 6765 5f69 643d 4e6f 6e65 2c0a  essage_id=None,.
-00003630: 2020 2020 616c 6c6f 775f 7365 6e64 696e      allow_sendin
-00003640: 675f 7769 7468 6f75 745f 7265 706c 793d  g_without_reply=
-00003650: 4e6f 6e65 2c0a 2020 2020 7265 706c 795f  None,.    reply_
-00003660: 6d61 726b 7570 3d4e 6f6e 652c 0a20 2020  markup=None,.   
-00003670: 2074 696d 656f 7574 3d4e 6f6e 652c 0a20   timeout=None,. 
-00003680: 2020 2070 726f 7465 6374 5f63 6f6e 7465     protect_conte
-00003690: 6e74 3d4e 6f6e 652c 0a20 2020 206d 6573  nt=None,.    mes
-000036a0: 7361 6765 5f74 6872 6561 645f 6964 3a20  sage_thread_id: 
-000036b0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-000036c0: 4e6f 6e65 2c0a 293a 0a20 2020 206d 6574  None,.):.    met
-000036d0: 686f 645f 7572 6c20 3d20 7222 636f 7079  hod_url = r"copy
-000036e0: 4d65 7373 6167 6522 0a20 2020 2070 6179  Message".    pay
-000036f0: 6c6f 6164 203d 207b 0a20 2020 2020 2020  load = {.       
-00003700: 2022 6368 6174 5f69 6422 3a20 6368 6174   "chat_id": chat
-00003710: 5f69 642c 0a20 2020 2020 2020 2022 6672  _id,.        "fr
-00003720: 6f6d 5f63 6861 745f 6964 223a 2066 726f  om_chat_id": fro
-00003730: 6d5f 6368 6174 5f69 642c 0a20 2020 2020  m_chat_id,.     
-00003740: 2020 2022 6d65 7373 6167 655f 6964 223a     "message_id":
-00003750: 206d 6573 7361 6765 5f69 642c 0a20 2020   message_id,.   
-00003760: 207d 0a20 2020 2069 6620 6361 7074 696f   }.    if captio
-00003770: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00003780: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-00003790: 6361 7074 696f 6e22 5d20 3d20 6361 7074  caption"] = capt
-000037a0: 696f 6e0a 2020 2020 6966 2070 6172 7365  ion.    if parse
-000037b0: 5f6d 6f64 653a 0a20 2020 2020 2020 2070  _mode:.        p
-000037c0: 6179 6c6f 6164 5b22 7061 7273 655f 6d6f  ayload["parse_mo
-000037d0: 6465 225d 203d 2070 6172 7365 5f6d 6f64  de"] = parse_mod
-000037e0: 650a 2020 2020 6966 2063 6170 7469 6f6e  e.    if caption
-000037f0: 5f65 6e74 6974 6965 7320 6973 206e 6f74  _entities is not
-00003800: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
-00003810: 6179 6c6f 6164 5b22 6361 7074 696f 6e5f  ayload["caption_
-00003820: 656e 7469 7469 6573 225d 203d 2061 7761  entities"] = awa
-00003830: 6974 205f 636f 6e76 6572 745f 656e 7469  it _convert_enti
-00003840: 7465 7328 6361 7074 696f 6e5f 656e 7469  tes(caption_enti
-00003850: 7469 6573 290a 2020 2020 6966 2064 6973  ties).    if dis
-00003860: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-00003870: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00003880: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-00003890: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-000038a0: 7469 6f6e 225d 203d 2064 6973 6162 6c65  tion"] = disable
-000038b0: 5f6e 6f74 6966 6963 6174 696f 6e0a 2020  _notification.  
-000038c0: 2020 6966 2072 6570 6c79 5f74 6f5f 6d65    if reply_to_me
-000038d0: 7373 6167 655f 6964 3a0a 2020 2020 2020  ssage_id:.      
-000038e0: 2020 7061 796c 6f61 645b 2272 6570 6c79    payload["reply
-000038f0: 5f74 6f5f 6d65 7373 6167 655f 6964 225d  _to_message_id"]
-00003900: 203d 2072 6570 6c79 5f74 6f5f 6d65 7373   = reply_to_mess
-00003910: 6167 655f 6964 0a20 2020 2069 6620 7265  age_id.    if re
-00003920: 706c 795f 6d61 726b 7570 2069 7320 6e6f  ply_markup is no
-00003930: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00003940: 7061 796c 6f61 645b 2272 6570 6c79 5f6d  payload["reply_m
-00003950: 6172 6b75 7022 5d20 3d20 6177 6169 7420  arkup"] = await 
-00003960: 5f63 6f6e 7665 7274 5f6d 6172 6b75 7028  _convert_markup(
-00003970: 7265 706c 795f 6d61 726b 7570 290a 2020  reply_markup).  
-00003980: 2020 6966 2061 6c6c 6f77 5f73 656e 6469    if allow_sendi
-00003990: 6e67 5f77 6974 686f 7574 5f72 6570 6c79  ng_without_reply
-000039a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000039b0: 2020 2020 2020 7061 796c 6f61 645b 2261        payload["a
-000039c0: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
-000039d0: 686f 7574 5f72 6570 6c79 225d 203d 2061  hout_reply"] = a
-000039e0: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
-000039f0: 686f 7574 5f72 6570 6c79 0a20 2020 2069  hout_reply.    i
-00003a00: 6620 7469 6d65 6f75 743a 0a20 2020 2020  f timeout:.     
-00003a10: 2020 2070 6179 6c6f 6164 5b22 7469 6d65     payload["time
-00003a20: 6f75 7422 5d20 3d20 7469 6d65 6f75 740a  out"] = timeout.
-00003a30: 2020 2020 6966 2070 726f 7465 6374 5f63      if protect_c
-00003a40: 6f6e 7465 6e74 2069 7320 6e6f 7420 4e6f  ontent is not No
-00003a50: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
-00003a60: 6f61 645b 2270 726f 7465 6374 5f63 6f6e  oad["protect_con
-00003a70: 7465 6e74 225d 203d 2070 726f 7465 6374  tent"] = protect
-00003a80: 5f63 6f6e 7465 6e74 0a20 2020 205f 6164  _content.    _ad
-00003a90: 645f 6d65 7373 6167 655f 7468 7265 6164  d_message_thread
-00003aa0: 5f69 6428 7061 796c 6f61 642c 206d 6573  _id(payload, mes
-00003ab0: 7361 6765 5f74 6872 6561 645f 6964 290a  sage_thread_id).
-00003ac0: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-00003ad0: 205f 7265 7175 6573 7428 746f 6b65 6e2c   _request(token,
-00003ae0: 206d 6574 686f 645f 7572 6c2c 2070 6172   method_url, par
-00003af0: 616d 733d 7061 796c 6f61 6429 0a0a 0a61  ams=payload)...a
-00003b00: 7379 6e63 2064 6566 2073 656e 645f 6469  sync def send_di
-00003b10: 6365 280a 2020 2020 746f 6b65 6e2c 0a20  ce(.    token,. 
-00003b20: 2020 2063 6861 745f 6964 2c0a 2020 2020     chat_id,.    
-00003b30: 656d 6f6a 693d 4e6f 6e65 2c0a 2020 2020  emoji=None,.    
-00003b40: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-00003b50: 7469 6f6e 3d4e 6f6e 652c 0a20 2020 2072  tion=None,.    r
-00003b60: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
-00003b70: 6964 3d4e 6f6e 652c 0a20 2020 2072 6570  id=None,.    rep
-00003b80: 6c79 5f6d 6172 6b75 703d 4e6f 6e65 2c0a  ly_markup=None,.
-00003b90: 2020 2020 7469 6d65 6f75 743d 4e6f 6e65      timeout=None
-00003ba0: 2c0a 2020 2020 616c 6c6f 775f 7365 6e64  ,.    allow_send
-00003bb0: 696e 675f 7769 7468 6f75 745f 7265 706c  ing_without_repl
-00003bc0: 793d 4e6f 6e65 2c0a 2020 2020 7072 6f74  y=None,.    prot
-00003bd0: 6563 745f 636f 6e74 656e 743d 4e6f 6e65  ect_content=None
-00003be0: 2c0a 2020 2020 6d65 7373 6167 655f 7468  ,.    message_th
-00003bf0: 7265 6164 5f69 643a 204f 7074 696f 6e61  read_id: Optiona
-00003c00: 6c5b 696e 745d 203d 204e 6f6e 652c 0a29  l[int] = None,.)
-00003c10: 3a0a 2020 2020 6d65 7468 6f64 5f75 726c  :.    method_url
-00003c20: 203d 2072 2273 656e 6444 6963 6522 0a20   = r"sendDice". 
-00003c30: 2020 2070 6179 6c6f 6164 203d 207b 2263     payload = {"c
-00003c40: 6861 745f 6964 223a 2063 6861 745f 6964  hat_id": chat_id
-00003c50: 7d0a 2020 2020 6966 2065 6d6f 6a69 3a0a  }.    if emoji:.
-00003c60: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-00003c70: 2265 6d6f 6a69 225d 203d 2065 6d6f 6a69  "emoji"] = emoji
-00003c80: 0a20 2020 2069 6620 6469 7361 626c 655f  .    if disable_
-00003c90: 6e6f 7469 6669 6361 7469 6f6e 2069 7320  notification is 
-00003ca0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00003cb0: 2020 7061 796c 6f61 645b 2264 6973 6162    payload["disab
-00003cc0: 6c65 5f6e 6f74 6966 6963 6174 696f 6e22  le_notification"
-00003cd0: 5d20 3d20 6469 7361 626c 655f 6e6f 7469  ] = disable_noti
-00003ce0: 6669 6361 7469 6f6e 0a20 2020 2069 6620  fication.    if 
-00003cf0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-00003d00: 5f69 643a 0a20 2020 2020 2020 2070 6179  _id:.        pay
-00003d10: 6c6f 6164 5b22 7265 706c 795f 746f 5f6d  load["reply_to_m
-00003d20: 6573 7361 6765 5f69 6422 5d20 3d20 7265  essage_id"] = re
-00003d30: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00003d40: 640a 2020 2020 6966 2072 6570 6c79 5f6d  d.    if reply_m
-00003d50: 6172 6b75 703a 0a20 2020 2020 2020 2070  arkup:.        p
-00003d60: 6179 6c6f 6164 5b22 7265 706c 795f 6d61  ayload["reply_ma
-00003d70: 726b 7570 225d 203d 2061 7761 6974 205f  rkup"] = await _
-00003d80: 636f 6e76 6572 745f 6d61 726b 7570 2872  convert_markup(r
-00003d90: 6570 6c79 5f6d 6172 6b75 7029 0a20 2020  eply_markup).   
-00003da0: 2069 6620 7469 6d65 6f75 743a 0a20 2020   if timeout:.   
-00003db0: 2020 2020 2070 6179 6c6f 6164 5b22 7469       payload["ti
-00003dc0: 6d65 6f75 7422 5d20 3d20 7469 6d65 6f75  meout"] = timeou
-00003dd0: 740a 2020 2020 6966 2061 6c6c 6f77 5f73  t.    if allow_s
-00003de0: 656e 6469 6e67 5f77 6974 686f 7574 5f72  ending_without_r
-00003df0: 6570 6c79 2069 7320 6e6f 7420 4e6f 6e65  eply is not None
-00003e00: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-00003e10: 645b 2261 6c6c 6f77 5f73 656e 6469 6e67  d["allow_sending
-00003e20: 5f77 6974 686f 7574 5f72 6570 6c79 225d  _without_reply"]
-00003e30: 203d 2061 6c6c 6f77 5f73 656e 6469 6e67   = allow_sending
-00003e40: 5f77 6974 686f 7574 5f72 6570 6c79 0a20  _without_reply. 
-00003e50: 2020 2069 6620 7072 6f74 6563 745f 636f     if protect_co
-00003e60: 6e74 656e 7420 6973 206e 6f74 204e 6f6e  ntent is not Non
-00003e70: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-00003e80: 6164 5b22 7072 6f74 6563 745f 636f 6e74  ad["protect_cont
-00003e90: 656e 7422 5d20 3d20 7072 6f74 6563 745f  ent"] = protect_
-00003ea0: 636f 6e74 656e 740a 2020 2020 5f61 6464  content.    _add
-00003eb0: 5f6d 6573 7361 6765 5f74 6872 6561 645f  _message_thread_
-00003ec0: 6964 2870 6179 6c6f 6164 2c20 6d65 7373  id(payload, mess
-00003ed0: 6167 655f 7468 7265 6164 5f69 6429 0a20  age_thread_id). 
-00003ee0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00003ef0: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
-00003f00: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
-00003f10: 6d73 3d70 6179 6c6f 6164 290a 0a0a 6173  ms=payload)...as
-00003f20: 796e 6320 6465 6620 7365 6e64 5f70 686f  ync def send_pho
-00003f30: 746f 280a 2020 2020 746f 6b65 6e2c 0a20  to(.    token,. 
-00003f40: 2020 2063 6861 745f 6964 2c0a 2020 2020     chat_id,.    
-00003f50: 7068 6f74 6f2c 0a20 2020 2063 6170 7469  photo,.    capti
-00003f60: 6f6e 3d4e 6f6e 652c 0a20 2020 2072 6570  on=None,.    rep
-00003f70: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
-00003f80: 3d4e 6f6e 652c 0a20 2020 2072 6570 6c79  =None,.    reply
-00003f90: 5f6d 6172 6b75 703d 4e6f 6e65 2c0a 2020  _markup=None,.  
-00003fa0: 2020 7061 7273 655f 6d6f 6465 3d4e 6f6e    parse_mode=Non
-00003fb0: 652c 0a20 2020 2064 6973 6162 6c65 5f6e  e,.    disable_n
-00003fc0: 6f74 6966 6963 6174 696f 6e3d 4e6f 6e65  otification=None
-00003fd0: 2c0a 2020 2020 7469 6d65 6f75 743d 4e6f  ,.    timeout=No
-00003fe0: 6e65 2c0a 2020 2020 6361 7074 696f 6e5f  ne,.    caption_
-00003ff0: 656e 7469 7469 6573 3d4e 6f6e 652c 0a20  entities=None,. 
-00004000: 2020 2061 6c6c 6f77 5f73 656e 6469 6e67     allow_sending
-00004010: 5f77 6974 686f 7574 5f72 6570 6c79 3d4e  _without_reply=N
-00004020: 6f6e 652c 0a20 2020 2070 726f 7465 6374  one,.    protect
-00004030: 5f63 6f6e 7465 6e74 3d4e 6f6e 652c 0a20  _content=None,. 
-00004040: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
-00004050: 645f 6964 3a20 4f70 7469 6f6e 616c 5b69  d_id: Optional[i
-00004060: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
-00004070: 6861 735f 7370 6f69 6c65 723a 204f 7074  has_spoiler: Opt
-00004080: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-00004090: 6e65 2c0a 293a 0a20 2020 206d 6574 686f  ne,.):.    metho
-000040a0: 645f 7572 6c20 3d20 7222 7365 6e64 5068  d_url = r"sendPh
-000040b0: 6f74 6f22 0a20 2020 2070 6179 6c6f 6164  oto".    payload
-000040c0: 203d 207b 2263 6861 745f 6964 223a 2063   = {"chat_id": c
-000040d0: 6861 745f 6964 7d0a 2020 2020 6669 6c65  hat_id}.    file
-000040e0: 7320 3d20 4e6f 6e65 0a20 2020 2069 6620  s = None.    if 
-000040f0: 7574 696c 2e69 735f 7374 7269 6e67 2870  util.is_string(p
-00004100: 686f 746f 293a 0a20 2020 2020 2020 2070  hoto):.        p
-00004110: 6179 6c6f 6164 5b22 7068 6f74 6f22 5d20  ayload["photo"] 
-00004120: 3d20 7068 6f74 6f0a 2020 2020 656c 7365  = photo.    else
-00004130: 3a0a 2020 2020 2020 2020 6669 6c65 7320  :.        files 
-00004140: 3d20 7b22 7068 6f74 6f22 3a20 7068 6f74  = {"photo": phot
-00004150: 6f7d 0a20 2020 2069 6620 6361 7074 696f  o}.    if captio
-00004160: 6e3a 0a20 2020 2020 2020 2070 6179 6c6f  n:.        paylo
-00004170: 6164 5b22 6361 7074 696f 6e22 5d20 3d20  ad["caption"] = 
-00004180: 6361 7074 696f 6e0a 2020 2020 6966 2072  caption.    if r
-00004190: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
-000041a0: 6964 3a0a 2020 2020 2020 2020 7061 796c  id:.        payl
-000041b0: 6f61 645b 2272 6570 6c79 5f74 6f5f 6d65  oad["reply_to_me
-000041c0: 7373 6167 655f 6964 225d 203d 2072 6570  ssage_id"] = rep
-000041d0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
-000041e0: 0a20 2020 2069 6620 7265 706c 795f 6d61  .    if reply_ma
-000041f0: 726b 7570 3a0a 2020 2020 2020 2020 7061  rkup:.        pa
-00004200: 796c 6f61 645b 2272 6570 6c79 5f6d 6172  yload["reply_mar
-00004210: 6b75 7022 5d20 3d20 6177 6169 7420 5f63  kup"] = await _c
-00004220: 6f6e 7665 7274 5f6d 6172 6b75 7028 7265  onvert_markup(re
-00004230: 706c 795f 6d61 726b 7570 290a 2020 2020  ply_markup).    
-00004240: 6966 2070 6172 7365 5f6d 6f64 653a 0a20  if parse_mode:. 
-00004250: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-00004260: 7061 7273 655f 6d6f 6465 225d 203d 2070  parse_mode"] = p
-00004270: 6172 7365 5f6d 6f64 650a 2020 2020 6966  arse_mode.    if
-00004280: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
-00004290: 6174 696f 6e20 6973 206e 6f74 204e 6f6e  ation is not Non
-000042a0: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-000042b0: 6164 5b22 6469 7361 626c 655f 6e6f 7469  ad["disable_noti
-000042c0: 6669 6361 7469 6f6e 225d 203d 2064 6973  fication"] = dis
-000042d0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-000042e0: 6e0a 2020 2020 6966 2074 696d 656f 7574  n.    if timeout
-000042f0: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-00004300: 645b 2274 696d 656f 7574 225d 203d 2074  d["timeout"] = t
-00004310: 696d 656f 7574 0a20 2020 2069 6620 6361  imeout.    if ca
-00004320: 7074 696f 6e5f 656e 7469 7469 6573 3a0a  ption_entities:.
-00004330: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-00004340: 2263 6170 7469 6f6e 5f65 6e74 6974 6965  "caption_entitie
-00004350: 7322 5d20 3d20 6a73 6f6e 2e64 756d 7073  s"] = json.dumps
-00004360: 2874 7970 6573 2e4d 6573 7361 6765 456e  (types.MessageEn
-00004370: 7469 7479 2e74 6f5f 6c69 7374 5f6f 665f  tity.to_list_of_
-00004380: 6469 6374 7328 6361 7074 696f 6e5f 656e  dicts(caption_en
-00004390: 7469 7469 6573 2929 0a20 2020 2069 6620  tities)).    if 
-000043a0: 616c 6c6f 775f 7365 6e64 696e 675f 7769  allow_sending_wi
-000043b0: 7468 6f75 745f 7265 706c 7920 6973 206e  thout_reply is n
-000043c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000043d0: 2070 6179 6c6f 6164 5b22 616c 6c6f 775f   payload["allow_
-000043e0: 7365 6e64 696e 675f 7769 7468 6f75 745f  sending_without_
-000043f0: 7265 706c 7922 5d20 3d20 616c 6c6f 775f  reply"] = allow_
-00004400: 7365 6e64 696e 675f 7769 7468 6f75 745f  sending_without_
-00004410: 7265 706c 790a 2020 2020 6966 2070 726f  reply.    if pro
-00004420: 7465 6374 5f63 6f6e 7465 6e74 2069 7320  tect_content is 
-00004430: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00004440: 2020 7061 796c 6f61 645b 2270 726f 7465    payload["prote
-00004450: 6374 5f63 6f6e 7465 6e74 225d 203d 2070  ct_content"] = p
-00004460: 726f 7465 6374 5f63 6f6e 7465 6e74 0a20  rotect_content. 
-00004470: 2020 205f 6164 645f 6d65 7373 6167 655f     _add_message_
-00004480: 7468 7265 6164 5f69 6428 7061 796c 6f61  thread_id(payloa
-00004490: 642c 206d 6573 7361 6765 5f74 6872 6561  d, message_threa
-000044a0: 645f 6964 290a 2020 2020 6966 2068 6173  d_id).    if has
-000044b0: 5f73 706f 696c 6572 2069 7320 6e6f 7420  _spoiler is not 
-000044c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
-000044d0: 796c 6f61 645b 2268 6173 5f73 706f 696c  yload["has_spoil
-000044e0: 6572 225d 203d 2068 6173 5f73 706f 696c  er"] = has_spoil
-000044f0: 6572 0a20 2020 2072 6574 7572 6e20 6177  er.    return aw
-00004500: 6169 7420 5f72 6571 7565 7374 2874 6f6b  ait _request(tok
-00004510: 656e 2c20 6d65 7468 6f64 5f75 726c 2c20  en, method_url, 
-00004520: 7061 7261 6d73 3d70 6179 6c6f 6164 2c20  params=payload, 
-00004530: 6669 6c65 733d 6669 6c65 732c 206d 6574  files=files, met
-00004540: 686f 643d 2270 6f73 7422 290a 0a0a 6173  hod="post")...as
-00004550: 796e 6320 6465 6620 7365 6e64 5f6d 6564  ync def send_med
-00004560: 6961 5f67 726f 7570 280a 2020 2020 746f  ia_group(.    to
-00004570: 6b65 6e2c 0a20 2020 2063 6861 745f 6964  ken,.    chat_id
-00004580: 2c0a 2020 2020 6d65 6469 612c 0a20 2020  ,.    media,.   
-00004590: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
-000045a0: 6174 696f 6e3d 4e6f 6e65 2c0a 2020 2020  ation=None,.    
-000045b0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-000045c0: 5f69 643d 4e6f 6e65 2c0a 2020 2020 7469  _id=None,.    ti
-000045d0: 6d65 6f75 743d 4e6f 6e65 2c0a 2020 2020  meout=None,.    
-000045e0: 616c 6c6f 775f 7365 6e64 696e 675f 7769  allow_sending_wi
-000045f0: 7468 6f75 745f 7265 706c 793d 4e6f 6e65  thout_reply=None
-00004600: 2c0a 2020 2020 7072 6f74 6563 745f 636f  ,.    protect_co
-00004610: 6e74 656e 743d 4e6f 6e65 2c0a 2020 2020  ntent=None,.    
-00004620: 6d65 7373 6167 655f 7468 7265 6164 5f69  message_thread_i
-00004630: 643a 204f 7074 696f 6e61 6c5b 696e 745d  d: Optional[int]
-00004640: 203d 204e 6f6e 652c 0a29 3a0a 2020 2020   = None,.):.    
-00004650: 6d65 7468 6f64 5f75 726c 203d 2072 2273  method_url = r"s
-00004660: 656e 644d 6564 6961 4772 6f75 7022 0a20  endMediaGroup". 
-00004670: 2020 206d 6564 6961 5f6a 736f 6e2c 2066     media_json, f
-00004680: 696c 6573 203d 2061 7761 6974 2063 6f6e  iles = await con
-00004690: 7665 7274 5f69 6e70 7574 5f6d 6564 6961  vert_input_media
-000046a0: 5f61 7272 6179 286d 6564 6961 290a 2020  _array(media).  
-000046b0: 2020 7061 796c 6f61 6420 3d20 7b22 6368    payload = {"ch
-000046c0: 6174 5f69 6422 3a20 6368 6174 5f69 642c  at_id": chat_id,
-000046d0: 2022 6d65 6469 6122 3a20 6d65 6469 615f   "media": media_
-000046e0: 6a73 6f6e 7d0a 2020 2020 6966 2064 6973  json}.    if dis
-000046f0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-00004700: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00004710: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-00004720: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-00004730: 7469 6f6e 225d 203d 2064 6973 6162 6c65  tion"] = disable
-00004740: 5f6e 6f74 6966 6963 6174 696f 6e0a 2020  _notification.  
-00004750: 2020 6966 2072 6570 6c79 5f74 6f5f 6d65    if reply_to_me
-00004760: 7373 6167 655f 6964 3a0a 2020 2020 2020  ssage_id:.      
-00004770: 2020 7061 796c 6f61 645b 2272 6570 6c79    payload["reply
-00004780: 5f74 6f5f 6d65 7373 6167 655f 6964 225d  _to_message_id"]
-00004790: 203d 2072 6570 6c79 5f74 6f5f 6d65 7373   = reply_to_mess
-000047a0: 6167 655f 6964 0a20 2020 2069 6620 7469  age_id.    if ti
-000047b0: 6d65 6f75 743a 0a20 2020 2020 2020 2070  meout:.        p
-000047c0: 6179 6c6f 6164 5b22 7469 6d65 6f75 7422  ayload["timeout"
-000047d0: 5d20 3d20 7469 6d65 6f75 740a 2020 2020  ] = timeout.    
-000047e0: 6966 2061 6c6c 6f77 5f73 656e 6469 6e67  if allow_sending
-000047f0: 5f77 6974 686f 7574 5f72 6570 6c79 2069  _without_reply i
-00004800: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00004810: 2020 2020 7061 796c 6f61 645b 2261 6c6c      payload["all
-00004820: 6f77 5f73 656e 6469 6e67 5f77 6974 686f  ow_sending_witho
-00004830: 7574 5f72 6570 6c79 225d 203d 2061 6c6c  ut_reply"] = all
-00004840: 6f77 5f73 656e 6469 6e67 5f77 6974 686f  ow_sending_witho
-00004850: 7574 5f72 6570 6c79 0a20 2020 2069 6620  ut_reply.    if 
-00004860: 7072 6f74 6563 745f 636f 6e74 656e 7420  protect_content 
-00004870: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00004880: 2020 2020 2070 6179 6c6f 6164 5b22 7072       payload["pr
-00004890: 6f74 6563 745f 636f 6e74 656e 7422 5d20  otect_content"] 
-000048a0: 3d20 7072 6f74 6563 745f 636f 6e74 656e  = protect_conten
-000048b0: 740a 2020 2020 5f61 6464 5f6d 6573 7361  t.    _add_messa
-000048c0: 6765 5f74 6872 6561 645f 6964 2870 6179  ge_thread_id(pay
-000048d0: 6c6f 6164 2c20 6d65 7373 6167 655f 7468  load, message_th
-000048e0: 7265 6164 5f69 6429 0a20 2020 2072 6574  read_id).    ret
-000048f0: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
-00004900: 7374 280a 2020 2020 2020 2020 746f 6b65  st(.        toke
-00004910: 6e2c 0a20 2020 2020 2020 206d 6574 686f  n,.        metho
-00004920: 645f 7572 6c2c 0a20 2020 2020 2020 2070  d_url,.        p
-00004930: 6172 616d 733d 7061 796c 6f61 642c 0a20  arams=payload,. 
-00004940: 2020 2020 2020 206d 6574 686f 643d 2270         method="p
-00004950: 6f73 7422 2069 6620 6669 6c65 7320 656c  ost" if files el
-00004960: 7365 2022 6765 7422 2c0a 2020 2020 2020  se "get",.      
-00004970: 2020 6669 6c65 733d 6669 6c65 7320 6966    files=files if
-00004980: 2066 696c 6573 2065 6c73 6520 4e6f 6e65   files else None
-00004990: 2c0a 2020 2020 290a 0a0a 6173 796e 6320  ,.    )...async 
-000049a0: 6465 6620 7365 6e64 5f6c 6f63 6174 696f  def send_locatio
-000049b0: 6e28 0a20 2020 2074 6f6b 656e 2c0a 2020  n(.    token,.  
-000049c0: 2020 6368 6174 5f69 642c 0a20 2020 206c    chat_id,.    l
-000049d0: 6174 6974 7564 652c 0a20 2020 206c 6f6e  atitude,.    lon
-000049e0: 6769 7475 6465 2c0a 2020 2020 6c69 7665  gitude,.    live
-000049f0: 5f70 6572 696f 643d 4e6f 6e65 2c0a 2020  _period=None,.  
-00004a00: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
-00004a10: 6765 5f69 643d 4e6f 6e65 2c0a 2020 2020  ge_id=None,.    
-00004a20: 7265 706c 795f 6d61 726b 7570 3d4e 6f6e  reply_markup=Non
-00004a30: 652c 0a20 2020 2064 6973 6162 6c65 5f6e  e,.    disable_n
-00004a40: 6f74 6966 6963 6174 696f 6e3d 4e6f 6e65  otification=None
-00004a50: 2c0a 2020 2020 7469 6d65 6f75 743d 4e6f  ,.    timeout=No
-00004a60: 6e65 2c0a 2020 2020 686f 7269 7a6f 6e74  ne,.    horizont
-00004a70: 616c 5f61 6363 7572 6163 793d 4e6f 6e65  al_accuracy=None
-00004a80: 2c0a 2020 2020 6865 6164 696e 673d 4e6f  ,.    heading=No
-00004a90: 6e65 2c0a 2020 2020 7072 6f78 696d 6974  ne,.    proximit
-00004aa0: 795f 616c 6572 745f 7261 6469 7573 3d4e  y_alert_radius=N
-00004ab0: 6f6e 652c 0a20 2020 2061 6c6c 6f77 5f73  one,.    allow_s
-00004ac0: 656e 6469 6e67 5f77 6974 686f 7574 5f72  ending_without_r
-00004ad0: 6570 6c79 3d4e 6f6e 652c 0a20 2020 2070  eply=None,.    p
-00004ae0: 726f 7465 6374 5f63 6f6e 7465 6e74 3d4e  rotect_content=N
-00004af0: 6f6e 652c 0a20 2020 206d 6573 7361 6765  one,.    message
-00004b00: 5f74 6872 6561 645f 6964 3a20 4f70 7469  _thread_id: Opti
-00004b10: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00004b20: 2c0a 293a 0a20 2020 206d 6574 686f 645f  ,.):.    method_
-00004b30: 7572 6c20 3d20 7222 7365 6e64 4c6f 6361  url = r"sendLoca
-00004b40: 7469 6f6e 220a 2020 2020 7061 796c 6f61  tion".    payloa
-00004b50: 6420 3d20 7b22 6368 6174 5f69 6422 3a20  d = {"chat_id": 
-00004b60: 6368 6174 5f69 642c 2022 6c61 7469 7475  chat_id, "latitu
-00004b70: 6465 223a 206c 6174 6974 7564 652c 2022  de": latitude, "
-00004b80: 6c6f 6e67 6974 7564 6522 3a20 6c6f 6e67  longitude": long
-00004b90: 6974 7564 657d 0a20 2020 2069 6620 6c69  itude}.    if li
-00004ba0: 7665 5f70 6572 696f 643a 0a20 2020 2020  ve_period:.     
-00004bb0: 2020 2070 6179 6c6f 6164 5b22 6c69 7665     payload["live
-00004bc0: 5f70 6572 696f 6422 5d20 3d20 6c69 7665  _period"] = live
-00004bd0: 5f70 6572 696f 640a 2020 2020 6966 2068  _period.    if h
-00004be0: 6f72 697a 6f6e 7461 6c5f 6163 6375 7261  orizontal_accura
-00004bf0: 6379 3a0a 2020 2020 2020 2020 7061 796c  cy:.        payl
-00004c00: 6f61 645b 2268 6f72 697a 6f6e 7461 6c5f  oad["horizontal_
-00004c10: 6163 6375 7261 6379 225d 203d 2068 6f72  accuracy"] = hor
-00004c20: 697a 6f6e 7461 6c5f 6163 6375 7261 6379  izontal_accuracy
-00004c30: 0a20 2020 2069 6620 6865 6164 696e 673a  .    if heading:
-00004c40: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00004c50: 5b22 6865 6164 696e 6722 5d20 3d20 6865  ["heading"] = he
-00004c60: 6164 696e 670a 2020 2020 6966 2070 726f  ading.    if pro
-00004c70: 7869 6d69 7479 5f61 6c65 7274 5f72 6164  ximity_alert_rad
-00004c80: 6975 733a 0a20 2020 2020 2020 2070 6179  ius:.        pay
-00004c90: 6c6f 6164 5b22 7072 6f78 696d 6974 795f  load["proximity_
-00004ca0: 616c 6572 745f 7261 6469 7573 225d 203d  alert_radius"] =
-00004cb0: 2070 726f 7869 6d69 7479 5f61 6c65 7274   proximity_alert
-00004cc0: 5f72 6164 6975 730a 2020 2020 6966 2072  _radius.    if r
-00004cd0: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
-00004ce0: 6964 3a0a 2020 2020 2020 2020 7061 796c  id:.        payl
-00004cf0: 6f61 645b 2272 6570 6c79 5f74 6f5f 6d65  oad["reply_to_me
-00004d00: 7373 6167 655f 6964 225d 203d 2072 6570  ssage_id"] = rep
-00004d10: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
-00004d20: 0a20 2020 2069 6620 616c 6c6f 775f 7365  .    if allow_se
-00004d30: 6e64 696e 675f 7769 7468 6f75 745f 7265  nding_without_re
-00004d40: 706c 7920 6973 206e 6f74 204e 6f6e 653a  ply is not None:
-00004d50: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00004d60: 5b22 616c 6c6f 775f 7365 6e64 696e 675f  ["allow_sending_
-00004d70: 7769 7468 6f75 745f 7265 706c 7922 5d20  without_reply"] 
-00004d80: 3d20 616c 6c6f 775f 7365 6e64 696e 675f  = allow_sending_
-00004d90: 7769 7468 6f75 745f 7265 706c 790a 2020  without_reply.  
-00004da0: 2020 6966 2072 6570 6c79 5f6d 6172 6b75    if reply_marku
-00004db0: 703a 0a20 2020 2020 2020 2070 6179 6c6f  p:.        paylo
-00004dc0: 6164 5b22 7265 706c 795f 6d61 726b 7570  ad["reply_markup
-00004dd0: 225d 203d 2061 7761 6974 205f 636f 6e76  "] = await _conv
-00004de0: 6572 745f 6d61 726b 7570 2872 6570 6c79  ert_markup(reply
-00004df0: 5f6d 6172 6b75 7029 0a20 2020 2069 6620  _markup).    if 
-00004e00: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-00004e10: 7469 6f6e 2069 7320 6e6f 7420 4e6f 6e65  tion is not None
-00004e20: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-00004e30: 645b 2264 6973 6162 6c65 5f6e 6f74 6966  d["disable_notif
-00004e40: 6963 6174 696f 6e22 5d20 3d20 6469 7361  ication"] = disa
-00004e50: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-00004e60: 0a20 2020 2069 6620 7469 6d65 6f75 743a  .    if timeout:
-00004e70: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00004e80: 5b22 7469 6d65 6f75 7422 5d20 3d20 7469  ["timeout"] = ti
-00004e90: 6d65 6f75 740a 2020 2020 6966 2070 726f  meout.    if pro
-00004ea0: 7465 6374 5f63 6f6e 7465 6e74 2069 7320  tect_content is 
-00004eb0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00004ec0: 2020 7061 796c 6f61 645b 2270 726f 7465    payload["prote
-00004ed0: 6374 5f63 6f6e 7465 6e74 225d 203d 2070  ct_content"] = p
-00004ee0: 726f 7465 6374 5f63 6f6e 7465 6e74 0a20  rotect_content. 
-00004ef0: 2020 205f 6164 645f 6d65 7373 6167 655f     _add_message_
-00004f00: 7468 7265 6164 5f69 6428 7061 796c 6f61  thread_id(payloa
-00004f10: 642c 206d 6573 7361 6765 5f74 6872 6561  d, message_threa
-00004f20: 645f 6964 290a 2020 2020 7265 7475 726e  d_id).    return
-00004f30: 2061 7761 6974 205f 7265 7175 6573 7428   await _request(
-00004f40: 746f 6b65 6e2c 206d 6574 686f 645f 7572  token, method_ur
-00004f50: 6c2c 2070 6172 616d 733d 7061 796c 6f61  l, params=payloa
-00004f60: 6429 0a0a 0a61 7379 6e63 2064 6566 2065  d)...async def e
-00004f70: 6469 745f 6d65 7373 6167 655f 6c69 7665  dit_message_live
-00004f80: 5f6c 6f63 6174 696f 6e28 0a20 2020 2074  _location(.    t
-00004f90: 6f6b 656e 2c0a 2020 2020 6c61 7469 7475  oken,.    latitu
-00004fa0: 6465 2c0a 2020 2020 6c6f 6e67 6974 7564  de,.    longitud
-00004fb0: 652c 0a20 2020 2063 6861 745f 6964 3d4e  e,.    chat_id=N
-00004fc0: 6f6e 652c 0a20 2020 206d 6573 7361 6765  one,.    message
-00004fd0: 5f69 643d 4e6f 6e65 2c0a 2020 2020 696e  _id=None,.    in
-00004fe0: 6c69 6e65 5f6d 6573 7361 6765 5f69 643d  line_message_id=
-00004ff0: 4e6f 6e65 2c0a 2020 2020 7265 706c 795f  None,.    reply_
-00005000: 6d61 726b 7570 3d4e 6f6e 652c 0a20 2020  markup=None,.   
-00005010: 2074 696d 656f 7574 3d4e 6f6e 652c 0a20   timeout=None,. 
-00005020: 2020 2068 6f72 697a 6f6e 7461 6c5f 6163     horizontal_ac
-00005030: 6375 7261 6379 3d4e 6f6e 652c 0a20 2020  curacy=None,.   
-00005040: 2068 6561 6469 6e67 3d4e 6f6e 652c 0a20   heading=None,. 
-00005050: 2020 2070 726f 7869 6d69 7479 5f61 6c65     proximity_ale
-00005060: 7274 5f72 6164 6975 733d 4e6f 6e65 2c0a  rt_radius=None,.
-00005070: 293a 0a20 2020 206d 6574 686f 645f 7572  ):.    method_ur
-00005080: 6c20 3d20 7222 6564 6974 4d65 7373 6167  l = r"editMessag
-00005090: 654c 6976 654c 6f63 6174 696f 6e22 0a20  eLiveLocation". 
-000050a0: 2020 2070 6179 6c6f 6164 203d 207b 226c     payload = {"l
-000050b0: 6174 6974 7564 6522 3a20 6c61 7469 7475  atitude": latitu
-000050c0: 6465 2c20 226c 6f6e 6769 7475 6465 223a  de, "longitude":
-000050d0: 206c 6f6e 6769 7475 6465 7d0a 2020 2020   longitude}.    
-000050e0: 6966 2063 6861 745f 6964 3a0a 2020 2020  if chat_id:.    
-000050f0: 2020 2020 7061 796c 6f61 645b 2263 6861      payload["cha
-00005100: 745f 6964 225d 203d 2063 6861 745f 6964  t_id"] = chat_id
-00005110: 0a20 2020 2069 6620 6d65 7373 6167 655f  .    if message_
-00005120: 6964 3a0a 2020 2020 2020 2020 7061 796c  id:.        payl
-00005130: 6f61 645b 226d 6573 7361 6765 5f69 6422  oad["message_id"
-00005140: 5d20 3d20 6d65 7373 6167 655f 6964 0a20  ] = message_id. 
-00005150: 2020 2069 6620 686f 7269 7a6f 6e74 616c     if horizontal
-00005160: 5f61 6363 7572 6163 793a 0a20 2020 2020  _accuracy:.     
-00005170: 2020 2070 6179 6c6f 6164 5b22 686f 7269     payload["hori
-00005180: 7a6f 6e74 616c 5f61 6363 7572 6163 7922  zontal_accuracy"
-00005190: 5d20 3d20 686f 7269 7a6f 6e74 616c 5f61  ] = horizontal_a
-000051a0: 6363 7572 6163 790a 2020 2020 6966 2068  ccuracy.    if h
-000051b0: 6561 6469 6e67 3a0a 2020 2020 2020 2020  eading:.        
-000051c0: 7061 796c 6f61 645b 2268 6561 6469 6e67  payload["heading
-000051d0: 225d 203d 2068 6561 6469 6e67 0a20 2020  "] = heading.   
-000051e0: 2069 6620 7072 6f78 696d 6974 795f 616c   if proximity_al
-000051f0: 6572 745f 7261 6469 7573 3a0a 2020 2020  ert_radius:.    
-00005200: 2020 2020 7061 796c 6f61 645b 2270 726f      payload["pro
-00005210: 7869 6d69 7479 5f61 6c65 7274 5f72 6164  ximity_alert_rad
-00005220: 6975 7322 5d20 3d20 7072 6f78 696d 6974  ius"] = proximit
-00005230: 795f 616c 6572 745f 7261 6469 7573 0a20  y_alert_radius. 
-00005240: 2020 2069 6620 696e 6c69 6e65 5f6d 6573     if inline_mes
-00005250: 7361 6765 5f69 643a 0a20 2020 2020 2020  sage_id:.       
-00005260: 2070 6179 6c6f 6164 5b22 696e 6c69 6e65   payload["inline
-00005270: 5f6d 6573 7361 6765 5f69 6422 5d20 3d20  _message_id"] = 
-00005280: 696e 6c69 6e65 5f6d 6573 7361 6765 5f69  inline_message_i
-00005290: 640a 2020 2020 6966 2072 6570 6c79 5f6d  d.    if reply_m
-000052a0: 6172 6b75 703a 0a20 2020 2020 2020 2070  arkup:.        p
-000052b0: 6179 6c6f 6164 5b22 7265 706c 795f 6d61  ayload["reply_ma
-000052c0: 726b 7570 225d 203d 2061 7761 6974 205f  rkup"] = await _
-000052d0: 636f 6e76 6572 745f 6d61 726b 7570 2872  convert_markup(r
-000052e0: 6570 6c79 5f6d 6172 6b75 7029 0a20 2020  eply_markup).   
-000052f0: 2069 6620 7469 6d65 6f75 743a 0a20 2020   if timeout:.   
-00005300: 2020 2020 2070 6179 6c6f 6164 5b22 7469       payload["ti
-00005310: 6d65 6f75 7422 5d20 3d20 7469 6d65 6f75  meout"] = timeou
-00005320: 740a 2020 2020 7265 7475 726e 2061 7761  t.    return awa
-00005330: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
-00005340: 6e2c 206d 6574 686f 645f 7572 6c2c 2070  n, method_url, p
-00005350: 6172 616d 733d 7061 796c 6f61 6429 0a0a  arams=payload)..
-00005360: 0a61 7379 6e63 2064 6566 2073 746f 705f  .async def stop_
-00005370: 6d65 7373 6167 655f 6c69 7665 5f6c 6f63  message_live_loc
-00005380: 6174 696f 6e28 0a20 2020 2074 6f6b 656e  ation(.    token
-00005390: 2c0a 2020 2020 6368 6174 5f69 643d 4e6f  ,.    chat_id=No
-000053a0: 6e65 2c0a 2020 2020 6d65 7373 6167 655f  ne,.    message_
-000053b0: 6964 3d4e 6f6e 652c 0a20 2020 2069 6e6c  id=None,.    inl
-000053c0: 696e 655f 6d65 7373 6167 655f 6964 3d4e  ine_message_id=N
-000053d0: 6f6e 652c 0a20 2020 2072 6570 6c79 5f6d  one,.    reply_m
-000053e0: 6172 6b75 703d 4e6f 6e65 2c0a 2020 2020  arkup=None,.    
-000053f0: 7469 6d65 6f75 743d 4e6f 6e65 2c0a 293a  timeout=None,.):
-00005400: 0a20 2020 206d 6574 686f 645f 7572 6c20  .    method_url 
-00005410: 3d20 7222 7374 6f70 4d65 7373 6167 654c  = r"stopMessageL
-00005420: 6976 654c 6f63 6174 696f 6e22 0a20 2020  iveLocation".   
-00005430: 2070 6179 6c6f 6164 203d 207b 7d0a 2020   payload = {}.  
-00005440: 2020 6966 2063 6861 745f 6964 3a0a 2020    if chat_id:.  
-00005450: 2020 2020 2020 7061 796c 6f61 645b 2263        payload["c
-00005460: 6861 745f 6964 225d 203d 2063 6861 745f  hat_id"] = chat_
-00005470: 6964 0a20 2020 2069 6620 6d65 7373 6167  id.    if messag
-00005480: 655f 6964 3a0a 2020 2020 2020 2020 7061  e_id:.        pa
-00005490: 796c 6f61 645b 226d 6573 7361 6765 5f69  yload["message_i
-000054a0: 6422 5d20 3d20 6d65 7373 6167 655f 6964  d"] = message_id
-000054b0: 0a20 2020 2069 6620 696e 6c69 6e65 5f6d  .    if inline_m
-000054c0: 6573 7361 6765 5f69 643a 0a20 2020 2020  essage_id:.     
-000054d0: 2020 2070 6179 6c6f 6164 5b22 696e 6c69     payload["inli
-000054e0: 6e65 5f6d 6573 7361 6765 5f69 6422 5d20  ne_message_id"] 
-000054f0: 3d20 696e 6c69 6e65 5f6d 6573 7361 6765  = inline_message
-00005500: 5f69 640a 2020 2020 6966 2072 6570 6c79  _id.    if reply
-00005510: 5f6d 6172 6b75 703a 0a20 2020 2020 2020  _markup:.       
-00005520: 2070 6179 6c6f 6164 5b22 7265 706c 795f   payload["reply_
-00005530: 6d61 726b 7570 225d 203d 2061 7761 6974  markup"] = await
-00005540: 205f 636f 6e76 6572 745f 6d61 726b 7570   _convert_markup
-00005550: 2872 6570 6c79 5f6d 6172 6b75 7029 0a20  (reply_markup). 
-00005560: 2020 2069 6620 7469 6d65 6f75 743a 0a20     if timeout:. 
-00005570: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-00005580: 7469 6d65 6f75 7422 5d20 3d20 7469 6d65  timeout"] = time
-00005590: 6f75 740a 2020 2020 7265 7475 726e 2061  out.    return a
-000055a0: 7761 6974 205f 7265 7175 6573 7428 746f  wait _request(to
-000055b0: 6b65 6e2c 206d 6574 686f 645f 7572 6c2c  ken, method_url,
-000055c0: 2070 6172 616d 733d 7061 796c 6f61 6429   params=payload)
-000055d0: 0a0a 0a61 7379 6e63 2064 6566 2073 656e  ...async def sen
-000055e0: 645f 7665 6e75 6528 0a20 2020 2074 6f6b  d_venue(.    tok
-000055f0: 656e 2c0a 2020 2020 6368 6174 5f69 642c  en,.    chat_id,
-00005600: 0a20 2020 206c 6174 6974 7564 652c 0a20  .    latitude,. 
-00005610: 2020 206c 6f6e 6769 7475 6465 2c0a 2020     longitude,.  
-00005620: 2020 7469 746c 652c 0a20 2020 2061 6464    title,.    add
-00005630: 7265 7373 2c0a 2020 2020 666f 7572 7371  ress,.    foursq
-00005640: 7561 7265 5f69 643d 4e6f 6e65 2c0a 2020  uare_id=None,.  
-00005650: 2020 666f 7572 7371 7561 7265 5f74 7970    foursquare_typ
-00005660: 653d 4e6f 6e65 2c0a 2020 2020 6469 7361  e=None,.    disa
-00005670: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-00005680: 3d4e 6f6e 652c 0a20 2020 2072 6570 6c79  =None,.    reply
-00005690: 5f74 6f5f 6d65 7373 6167 655f 6964 3d4e  _to_message_id=N
-000056a0: 6f6e 652c 0a20 2020 2072 6570 6c79 5f6d  one,.    reply_m
-000056b0: 6172 6b75 703d 4e6f 6e65 2c0a 2020 2020  arkup=None,.    
-000056c0: 7469 6d65 6f75 743d 4e6f 6e65 2c0a 2020  timeout=None,.  
-000056d0: 2020 616c 6c6f 775f 7365 6e64 696e 675f    allow_sending_
-000056e0: 7769 7468 6f75 745f 7265 706c 793d 4e6f  without_reply=No
-000056f0: 6e65 2c0a 2020 2020 676f 6f67 6c65 5f70  ne,.    google_p
-00005700: 6c61 6365 5f69 643d 4e6f 6e65 2c0a 2020  lace_id=None,.  
-00005710: 2020 676f 6f67 6c65 5f70 6c61 6365 5f74    google_place_t
-00005720: 7970 653d 4e6f 6e65 2c0a 2020 2020 7072  ype=None,.    pr
-00005730: 6f74 6563 745f 636f 6e74 656e 743d 4e6f  otect_content=No
-00005740: 6e65 2c0a 2020 2020 6d65 7373 6167 655f  ne,.    message_
-00005750: 7468 7265 6164 5f69 643a 204f 7074 696f  thread_id: Optio
-00005760: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-00005770: 0a29 3a0a 2020 2020 6d65 7468 6f64 5f75  .):.    method_u
-00005780: 726c 203d 2072 2273 656e 6456 656e 7565  rl = r"sendVenue
-00005790: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
-000057a0: 7b0a 2020 2020 2020 2020 2263 6861 745f  {.        "chat_
-000057b0: 6964 223a 2063 6861 745f 6964 2c0a 2020  id": chat_id,.  
-000057c0: 2020 2020 2020 226c 6174 6974 7564 6522        "latitude"
-000057d0: 3a20 6c61 7469 7475 6465 2c0a 2020 2020  : latitude,.    
-000057e0: 2020 2020 226c 6f6e 6769 7475 6465 223a      "longitude":
-000057f0: 206c 6f6e 6769 7475 6465 2c0a 2020 2020   longitude,.    
-00005800: 2020 2020 2274 6974 6c65 223a 2074 6974      "title": tit
-00005810: 6c65 2c0a 2020 2020 2020 2020 2261 6464  le,.        "add
-00005820: 7265 7373 223a 2061 6464 7265 7373 2c0a  ress": address,.
-00005830: 2020 2020 7d0a 2020 2020 6966 2066 6f75      }.    if fou
-00005840: 7273 7175 6172 655f 6964 3a0a 2020 2020  rsquare_id:.    
-00005850: 2020 2020 7061 796c 6f61 645b 2266 6f75      payload["fou
-00005860: 7273 7175 6172 655f 6964 225d 203d 2066  rsquare_id"] = f
-00005870: 6f75 7273 7175 6172 655f 6964 0a20 2020  oursquare_id.   
-00005880: 2069 6620 666f 7572 7371 7561 7265 5f74   if foursquare_t
-00005890: 7970 653a 0a20 2020 2020 2020 2070 6179  ype:.        pay
-000058a0: 6c6f 6164 5b22 666f 7572 7371 7561 7265  load["foursquare
-000058b0: 5f74 7970 6522 5d20 3d20 666f 7572 7371  _type"] = foursq
-000058c0: 7561 7265 5f74 7970 650a 2020 2020 6966  uare_type.    if
-000058d0: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
-000058e0: 6174 696f 6e20 6973 206e 6f74 204e 6f6e  ation is not Non
-000058f0: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-00005900: 6164 5b22 6469 7361 626c 655f 6e6f 7469  ad["disable_noti
-00005910: 6669 6361 7469 6f6e 225d 203d 2064 6973  fication"] = dis
-00005920: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-00005930: 6e0a 2020 2020 6966 2072 6570 6c79 5f74  n.    if reply_t
-00005940: 6f5f 6d65 7373 6167 655f 6964 3a0a 2020  o_message_id:.  
-00005950: 2020 2020 2020 7061 796c 6f61 645b 2272        payload["r
-00005960: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
-00005970: 6964 225d 203d 2072 6570 6c79 5f74 6f5f  id"] = reply_to_
-00005980: 6d65 7373 6167 655f 6964 0a20 2020 2069  message_id.    i
-00005990: 6620 7265 706c 795f 6d61 726b 7570 3a0a  f reply_markup:.
-000059a0: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-000059b0: 2272 6570 6c79 5f6d 6172 6b75 7022 5d20  "reply_markup"] 
-000059c0: 3d20 6177 6169 7420 5f63 6f6e 7665 7274  = await _convert
-000059d0: 5f6d 6172 6b75 7028 7265 706c 795f 6d61  _markup(reply_ma
-000059e0: 726b 7570 290a 2020 2020 6966 2074 696d  rkup).    if tim
-000059f0: 656f 7574 3a0a 2020 2020 2020 2020 7061  eout:.        pa
-00005a00: 796c 6f61 645b 2274 696d 656f 7574 225d  yload["timeout"]
-00005a10: 203d 2074 696d 656f 7574 0a20 2020 2069   = timeout.    i
-00005a20: 6620 616c 6c6f 775f 7365 6e64 696e 675f  f allow_sending_
-00005a30: 7769 7468 6f75 745f 7265 706c 7920 6973  without_reply is
-00005a40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00005a50: 2020 2070 6179 6c6f 6164 5b22 616c 6c6f     payload["allo
-00005a60: 775f 7365 6e64 696e 675f 7769 7468 6f75  w_sending_withou
-00005a70: 745f 7265 706c 7922 5d20 3d20 616c 6c6f  t_reply"] = allo
-00005a80: 775f 7365 6e64 696e 675f 7769 7468 6f75  w_sending_withou
-00005a90: 745f 7265 706c 790a 2020 2020 6966 2067  t_reply.    if g
-00005aa0: 6f6f 676c 655f 706c 6163 655f 6964 3a0a  oogle_place_id:.
-00005ab0: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-00005ac0: 2267 6f6f 676c 655f 706c 6163 655f 6964  "google_place_id
-00005ad0: 225d 203d 2067 6f6f 676c 655f 706c 6163  "] = google_plac
-00005ae0: 655f 6964 0a20 2020 2069 6620 676f 6f67  e_id.    if goog
-00005af0: 6c65 5f70 6c61 6365 5f74 7970 653a 0a20  le_place_type:. 
-00005b00: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-00005b10: 676f 6f67 6c65 5f70 6c61 6365 5f74 7970  google_place_typ
-00005b20: 6522 5d20 3d20 676f 6f67 6c65 5f70 6c61  e"] = google_pla
-00005b30: 6365 5f74 7970 650a 2020 2020 6966 2070  ce_type.    if p
-00005b40: 726f 7465 6374 5f63 6f6e 7465 6e74 2069  rotect_content i
-00005b50: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00005b60: 2020 2020 7061 796c 6f61 645b 2270 726f      payload["pro
-00005b70: 7465 6374 5f63 6f6e 7465 6e74 225d 203d  tect_content"] =
-00005b80: 2070 726f 7465 6374 5f63 6f6e 7465 6e74   protect_content
-00005b90: 0a20 2020 205f 6164 645f 6d65 7373 6167  .    _add_messag
-00005ba0: 655f 7468 7265 6164 5f69 6428 7061 796c  e_thread_id(payl
-00005bb0: 6f61 642c 206d 6573 7361 6765 5f74 6872  oad, message_thr
-00005bc0: 6561 645f 6964 290a 2020 2020 7265 7475  ead_id).    retu
-00005bd0: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
-00005be0: 7428 746f 6b65 6e2c 206d 6574 686f 645f  t(token, method_
-00005bf0: 7572 6c2c 2070 6172 616d 733d 7061 796c  url, params=payl
-00005c00: 6f61 6429 0a0a 0a61 7379 6e63 2064 6566  oad)...async def
-00005c10: 2073 656e 645f 636f 6e74 6163 7428 0a20   send_contact(. 
-00005c20: 2020 2074 6f6b 656e 2c0a 2020 2020 6368     token,.    ch
-00005c30: 6174 5f69 642c 0a20 2020 2070 686f 6e65  at_id,.    phone
-00005c40: 5f6e 756d 6265 722c 0a20 2020 2066 6972  _number,.    fir
-00005c50: 7374 5f6e 616d 652c 0a20 2020 206c 6173  st_name,.    las
-00005c60: 745f 6e61 6d65 3d4e 6f6e 652c 0a20 2020  t_name=None,.   
-00005c70: 2076 6361 7264 3d4e 6f6e 652c 0a20 2020   vcard=None,.   
-00005c80: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
-00005c90: 6174 696f 6e3d 4e6f 6e65 2c0a 2020 2020  ation=None,.    
-00005ca0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-00005cb0: 5f69 643d 4e6f 6e65 2c0a 2020 2020 7265  _id=None,.    re
-00005cc0: 706c 795f 6d61 726b 7570 3d4e 6f6e 652c  ply_markup=None,
-00005cd0: 0a20 2020 2074 696d 656f 7574 3d4e 6f6e  .    timeout=Non
-00005ce0: 652c 0a20 2020 2061 6c6c 6f77 5f73 656e  e,.    allow_sen
-00005cf0: 6469 6e67 5f77 6974 686f 7574 5f72 6570  ding_without_rep
-00005d00: 6c79 3d4e 6f6e 652c 0a20 2020 2070 726f  ly=None,.    pro
-00005d10: 7465 6374 5f63 6f6e 7465 6e74 3d4e 6f6e  tect_content=Non
-00005d20: 652c 0a20 2020 206d 6573 7361 6765 5f74  e,.    message_t
-00005d30: 6872 6561 645f 6964 3a20 4f70 7469 6f6e  hread_id: Option
-00005d40: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
-00005d50: 293a 0a20 2020 206d 6574 686f 645f 7572  ):.    method_ur
-00005d60: 6c20 3d20 7222 7365 6e64 436f 6e74 6163  l = r"sendContac
-00005d70: 7422 0a20 2020 2070 6179 6c6f 6164 203d  t".    payload =
-00005d80: 207b 0a20 2020 2020 2020 2022 6368 6174   {.        "chat
-00005d90: 5f69 6422 3a20 6368 6174 5f69 642c 0a20  _id": chat_id,. 
-00005da0: 2020 2020 2020 2022 7068 6f6e 655f 6e75         "phone_nu
-00005db0: 6d62 6572 223a 2070 686f 6e65 5f6e 756d  mber": phone_num
-00005dc0: 6265 722c 0a20 2020 2020 2020 2022 6669  ber,.        "fi
-00005dd0: 7273 745f 6e61 6d65 223a 2066 6972 7374  rst_name": first
-00005de0: 5f6e 616d 652c 0a20 2020 207d 0a20 2020  _name,.    }.   
-00005df0: 2069 6620 6c61 7374 5f6e 616d 653a 0a20   if last_name:. 
-00005e00: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-00005e10: 6c61 7374 5f6e 616d 6522 5d20 3d20 6c61  last_name"] = la
-00005e20: 7374 5f6e 616d 650a 2020 2020 6966 2076  st_name.    if v
-00005e30: 6361 7264 3a0a 2020 2020 2020 2020 7061  card:.        pa
-00005e40: 796c 6f61 645b 2276 6361 7264 225d 203d  yload["vcard"] =
-00005e50: 2076 6361 7264 0a20 2020 2069 6620 6469   vcard.    if di
-00005e60: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
-00005e70: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
-00005e80: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-00005e90: 2264 6973 6162 6c65 5f6e 6f74 6966 6963  "disable_notific
-00005ea0: 6174 696f 6e22 5d20 3d20 6469 7361 626c  ation"] = disabl
-00005eb0: 655f 6e6f 7469 6669 6361 7469 6f6e 0a20  e_notification. 
-00005ec0: 2020 2069 6620 7265 706c 795f 746f 5f6d     if reply_to_m
-00005ed0: 6573 7361 6765 5f69 643a 0a20 2020 2020  essage_id:.     
-00005ee0: 2020 2070 6179 6c6f 6164 5b22 7265 706c     payload["repl
-00005ef0: 795f 746f 5f6d 6573 7361 6765 5f69 6422  y_to_message_id"
-00005f00: 5d20 3d20 7265 706c 795f 746f 5f6d 6573  ] = reply_to_mes
-00005f10: 7361 6765 5f69 640a 2020 2020 6966 2072  sage_id.    if r
-00005f20: 6570 6c79 5f6d 6172 6b75 703a 0a20 2020  eply_markup:.   
-00005f30: 2020 2020 2070 6179 6c6f 6164 5b22 7265       payload["re
-00005f40: 706c 795f 6d61 726b 7570 225d 203d 2061  ply_markup"] = a
-00005f50: 7761 6974 205f 636f 6e76 6572 745f 6d61  wait _convert_ma
-00005f60: 726b 7570 2872 6570 6c79 5f6d 6172 6b75  rkup(reply_marku
-00005f70: 7029 0a20 2020 2069 6620 7469 6d65 6f75  p).    if timeou
-00005f80: 743a 0a20 2020 2020 2020 2070 6179 6c6f  t:.        paylo
-00005f90: 6164 5b22 7469 6d65 6f75 7422 5d20 3d20  ad["timeout"] = 
-00005fa0: 7469 6d65 6f75 740a 2020 2020 6966 2061  timeout.    if a
-00005fb0: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
-00005fc0: 686f 7574 5f72 6570 6c79 2069 7320 6e6f  hout_reply is no
-00005fd0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00005fe0: 7061 796c 6f61 645b 2261 6c6c 6f77 5f73  payload["allow_s
-00005ff0: 656e 6469 6e67 5f77 6974 686f 7574 5f72  ending_without_r
-00006000: 6570 6c79 225d 203d 2061 6c6c 6f77 5f73  eply"] = allow_s
-00006010: 656e 6469 6e67 5f77 6974 686f 7574 5f72  ending_without_r
-00006020: 6570 6c79 0a20 2020 2069 6620 7072 6f74  eply.    if prot
-00006030: 6563 745f 636f 6e74 656e 7420 6973 206e  ect_content is n
-00006040: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00006050: 2070 6179 6c6f 6164 5b22 7072 6f74 6563   payload["protec
-00006060: 745f 636f 6e74 656e 7422 5d20 3d20 7072  t_content"] = pr
-00006070: 6f74 6563 745f 636f 6e74 656e 740a 2020  otect_content.  
-00006080: 2020 5f61 6464 5f6d 6573 7361 6765 5f74    _add_message_t
-00006090: 6872 6561 645f 6964 2870 6179 6c6f 6164  hread_id(payload
-000060a0: 2c20 6d65 7373 6167 655f 7468 7265 6164  , message_thread
-000060b0: 5f69 6429 0a20 2020 2072 6574 7572 6e20  _id).    return 
-000060c0: 6177 6169 7420 5f72 6571 7565 7374 2874  await _request(t
-000060d0: 6f6b 656e 2c20 6d65 7468 6f64 5f75 726c  oken, method_url
-000060e0: 2c20 7061 7261 6d73 3d70 6179 6c6f 6164  , params=payload
-000060f0: 290a 0a0a 6173 796e 6320 6465 6620 7365  )...async def se
-00006100: 6e64 5f63 6861 745f 6163 7469 6f6e 2874  nd_chat_action(t
-00006110: 6f6b 656e 2c20 6368 6174 5f69 642c 2061  oken, chat_id, a
-00006120: 6374 696f 6e2c 2074 696d 656f 7574 3d4e  ction, timeout=N
-00006130: 6f6e 652c 206d 6573 7361 6765 5f74 6872  one, message_thr
-00006140: 6561 645f 6964 3a20 4f70 7469 6f6e 616c  ead_id: Optional
-00006150: 5b69 6e74 5d20 3d20 4e6f 6e65 293a 0a20  [int] = None):. 
-00006160: 2020 2072 6f75 7465 203d 2072 2273 656e     route = r"sen
-00006170: 6443 6861 7441 6374 696f 6e22 0a20 2020  dChatAction".   
-00006180: 2070 6179 6c6f 6164 203d 207b 2263 6861   payload = {"cha
-00006190: 745f 6964 223a 2063 6861 745f 6964 2c20  t_id": chat_id, 
-000061a0: 2261 6374 696f 6e22 3a20 6163 7469 6f6e  "action": action
-000061b0: 7d0a 2020 2020 6966 2074 696d 656f 7574  }.    if timeout
-000061c0: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-000061d0: 645b 2274 696d 656f 7574 225d 203d 2074  d["timeout"] = t
-000061e0: 696d 656f 7574 0a20 2020 205f 6164 645f  imeout.    _add_
-000061f0: 6d65 7373 6167 655f 7468 7265 6164 5f69  message_thread_i
-00006200: 6428 7061 796c 6f61 642c 206d 6573 7361  d(payload, messa
-00006210: 6765 5f74 6872 6561 645f 6964 290a 2020  ge_thread_id).  
-00006220: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
-00006230: 7265 7175 6573 7428 746f 6b65 6e2c 2072  request(token, r
-00006240: 6f75 7465 2c20 7061 7261 6d73 3d70 6179  oute, params=pay
-00006250: 6c6f 6164 290a 0a0a 6173 796e 6320 6465  load)...async de
-00006260: 6620 7365 6e64 5f76 6964 656f 280a 2020  f send_video(.  
-00006270: 2020 746f 6b65 6e2c 0a20 2020 2063 6861    token,.    cha
-00006280: 745f 6964 2c0a 2020 2020 6461 7461 2c0a  t_id,.    data,.
-00006290: 2020 2020 6475 7261 7469 6f6e 3d4e 6f6e      duration=Non
-000062a0: 652c 0a20 2020 2063 6170 7469 6f6e 3d4e  e,.    caption=N
-000062b0: 6f6e 652c 0a20 2020 2072 6570 6c79 5f74  one,.    reply_t
-000062c0: 6f5f 6d65 7373 6167 655f 6964 3d4e 6f6e  o_message_id=Non
-000062d0: 652c 0a20 2020 2072 6570 6c79 5f6d 6172  e,.    reply_mar
-000062e0: 6b75 703d 4e6f 6e65 2c0a 2020 2020 7061  kup=None,.    pa
-000062f0: 7273 655f 6d6f 6465 3d4e 6f6e 652c 0a20  rse_mode=None,. 
-00006300: 2020 2073 7570 706f 7274 735f 7374 7265     supports_stre
-00006310: 616d 696e 673d 4e6f 6e65 2c0a 2020 2020  aming=None,.    
-00006320: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-00006330: 7469 6f6e 3d4e 6f6e 652c 0a20 2020 2074  tion=None,.    t
-00006340: 696d 656f 7574 3d4e 6f6e 652c 0a20 2020  imeout=None,.   
-00006350: 2074 6875 6d62 3d4e 6f6e 652c 0a20 2020   thumb=None,.   
-00006360: 2077 6964 7468 3d4e 6f6e 652c 0a20 2020   width=None,.   
-00006370: 2068 6569 6768 743d 4e6f 6e65 2c0a 2020   height=None,.  
-00006380: 2020 6361 7074 696f 6e5f 656e 7469 7469    caption_entiti
-00006390: 6573 3d4e 6f6e 652c 0a20 2020 2061 6c6c  es=None,.    all
-000063a0: 6f77 5f73 656e 6469 6e67 5f77 6974 686f  ow_sending_witho
-000063b0: 7574 5f72 6570 6c79 3d4e 6f6e 652c 0a20  ut_reply=None,. 
-000063c0: 2020 2070 726f 7465 6374 5f63 6f6e 7465     protect_conte
-000063d0: 6e74 3d4e 6f6e 652c 0a20 2020 206d 6573  nt=None,.    mes
-000063e0: 7361 6765 5f74 6872 6561 645f 6964 3a20  sage_thread_id: 
-000063f0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00006400: 4e6f 6e65 2c0a 2020 2020 6861 735f 7370  None,.    has_sp
-00006410: 6f69 6c65 723a 204f 7074 696f 6e61 6c5b  oiler: Optional[
-00006420: 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a 293a  bool] = None,.):
-00006430: 0a20 2020 206d 6574 686f 645f 7572 6c20  .    method_url 
-00006440: 3d20 7222 7365 6e64 5669 6465 6f22 0a20  = r"sendVideo". 
-00006450: 2020 2070 6179 6c6f 6164 203d 207b 2263     payload = {"c
-00006460: 6861 745f 6964 223a 2063 6861 745f 6964  hat_id": chat_id
-00006470: 7d0a 2020 2020 6669 6c65 7320 3d20 4e6f  }.    files = No
-00006480: 6e65 0a20 2020 2069 6620 6e6f 7420 7574  ne.    if not ut
-00006490: 696c 2e69 735f 7374 7269 6e67 2864 6174  il.is_string(dat
-000064a0: 6129 3a0a 2020 2020 2020 2020 6669 6c65  a):.        file
-000064b0: 7320 3d20 7b22 7669 6465 6f22 3a20 6461  s = {"video": da
-000064c0: 7461 7d0a 2020 2020 656c 7365 3a0a 2020  ta}.    else:.  
-000064d0: 2020 2020 2020 7061 796c 6f61 645b 2276        payload["v
-000064e0: 6964 656f 225d 203d 2064 6174 610a 2020  ideo"] = data.  
-000064f0: 2020 6966 2064 7572 6174 696f 6e3a 0a20    if duration:. 
-00006500: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-00006510: 6475 7261 7469 6f6e 225d 203d 2064 7572  duration"] = dur
-00006520: 6174 696f 6e0a 2020 2020 6966 2063 6170  ation.    if cap
-00006530: 7469 6f6e 3a0a 2020 2020 2020 2020 7061  tion:.        pa
-00006540: 796c 6f61 645b 2263 6170 7469 6f6e 225d  yload["caption"]
-00006550: 203d 2063 6170 7469 6f6e 0a20 2020 2069   = caption.    i
-00006560: 6620 7265 706c 795f 746f 5f6d 6573 7361  f reply_to_messa
-00006570: 6765 5f69 643a 0a20 2020 2020 2020 2070  ge_id:.        p
-00006580: 6179 6c6f 6164 5b22 7265 706c 795f 746f  ayload["reply_to
-00006590: 5f6d 6573 7361 6765 5f69 6422 5d20 3d20  _message_id"] = 
-000065a0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-000065b0: 5f69 640a 2020 2020 6966 2072 6570 6c79  _id.    if reply
-000065c0: 5f6d 6172 6b75 703a 0a20 2020 2020 2020  _markup:.       
-000065d0: 2070 6179 6c6f 6164 5b22 7265 706c 795f   payload["reply_
-000065e0: 6d61 726b 7570 225d 203d 2061 7761 6974  markup"] = await
-000065f0: 205f 636f 6e76 6572 745f 6d61 726b 7570   _convert_markup
-00006600: 2872 6570 6c79 5f6d 6172 6b75 7029 0a20  (reply_markup). 
-00006610: 2020 2069 6620 7061 7273 655f 6d6f 6465     if parse_mode
-00006620: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-00006630: 645b 2270 6172 7365 5f6d 6f64 6522 5d20  d["parse_mode"] 
-00006640: 3d20 7061 7273 655f 6d6f 6465 0a20 2020  = parse_mode.   
-00006650: 2069 6620 7375 7070 6f72 7473 5f73 7472   if supports_str
-00006660: 6561 6d69 6e67 2069 7320 6e6f 7420 4e6f  eaming is not No
-00006670: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
-00006680: 6f61 645b 2273 7570 706f 7274 735f 7374  oad["supports_st
-00006690: 7265 616d 696e 6722 5d20 3d20 7375 7070  reaming"] = supp
-000066a0: 6f72 7473 5f73 7472 6561 6d69 6e67 0a20  orts_streaming. 
-000066b0: 2020 2069 6620 6469 7361 626c 655f 6e6f     if disable_no
-000066c0: 7469 6669 6361 7469 6f6e 2069 7320 6e6f  tification is no
-000066d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000066e0: 7061 796c 6f61 645b 2264 6973 6162 6c65  payload["disable
-000066f0: 5f6e 6f74 6966 6963 6174 696f 6e22 5d20  _notification"] 
-00006700: 3d20 6469 7361 626c 655f 6e6f 7469 6669  = disable_notifi
-00006710: 6361 7469 6f6e 0a20 2020 2069 6620 7469  cation.    if ti
-00006720: 6d65 6f75 743a 0a20 2020 2020 2020 2070  meout:.        p
-00006730: 6179 6c6f 6164 5b22 7469 6d65 6f75 7422  ayload["timeout"
-00006740: 5d20 3d20 7469 6d65 6f75 740a 2020 2020  ] = timeout.    
-00006750: 6966 2074 6875 6d62 3a0a 2020 2020 2020  if thumb:.      
-00006760: 2020 6966 206e 6f74 2075 7469 6c2e 6973    if not util.is
-00006770: 5f73 7472 696e 6728 7468 756d 6229 3a0a  _string(thumb):.
-00006780: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-00006790: 696c 6573 3a0a 2020 2020 2020 2020 2020  iles:.          
-000067a0: 2020 2020 2020 6669 6c65 735b 2274 6875        files["thu
-000067b0: 6d62 225d 203d 2074 6875 6d62 0a20 2020  mb"] = thumb.   
-000067c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000067d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000067e0: 696c 6573 203d 207b 2274 6875 6d62 223a  iles = {"thumb":
-000067f0: 2074 6875 6d62 7d0a 2020 2020 2020 2020   thumb}.        
-00006800: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00006810: 2020 7061 796c 6f61 645b 2274 6875 6d62    payload["thumb
-00006820: 225d 203d 2074 6875 6d62 0a20 2020 2069  "] = thumb.    i
-00006830: 6620 7769 6474 683a 0a20 2020 2020 2020  f width:.       
-00006840: 2070 6179 6c6f 6164 5b22 7769 6474 6822   payload["width"
-00006850: 5d20 3d20 7769 6474 680a 2020 2020 6966  ] = width.    if
-00006860: 2068 6569 6768 743a 0a20 2020 2020 2020   height:.       
-00006870: 2070 6179 6c6f 6164 5b22 6865 6967 6874   payload["height
-00006880: 225d 203d 2068 6569 6768 740a 2020 2020  "] = height.    
-00006890: 6966 2063 6170 7469 6f6e 5f65 6e74 6974  if caption_entit
-000068a0: 6965 733a 0a20 2020 2020 2020 2070 6179  ies:.        pay
-000068b0: 6c6f 6164 5b22 6361 7074 696f 6e5f 656e  load["caption_en
-000068c0: 7469 7469 6573 225d 203d 206a 736f 6e2e  tities"] = json.
-000068d0: 6475 6d70 7328 7479 7065 732e 4d65 7373  dumps(types.Mess
-000068e0: 6167 6545 6e74 6974 792e 746f 5f6c 6973  ageEntity.to_lis
-000068f0: 745f 6f66 5f64 6963 7473 2863 6170 7469  t_of_dicts(capti
-00006900: 6f6e 5f65 6e74 6974 6965 7329 290a 2020  on_entities)).  
-00006910: 2020 6966 2061 6c6c 6f77 5f73 656e 6469    if allow_sendi
-00006920: 6e67 5f77 6974 686f 7574 5f72 6570 6c79  ng_without_reply
-00006930: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00006940: 2020 2020 2020 7061 796c 6f61 645b 2261        payload["a
-00006950: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
-00006960: 686f 7574 5f72 6570 6c79 225d 203d 2061  hout_reply"] = a
-00006970: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
-00006980: 686f 7574 5f72 6570 6c79 0a20 2020 2069  hout_reply.    i
-00006990: 6620 7072 6f74 6563 745f 636f 6e74 656e  f protect_conten
-000069a0: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
-000069b0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-000069c0: 7072 6f74 6563 745f 636f 6e74 656e 7422  protect_content"
-000069d0: 5d20 3d20 7072 6f74 6563 745f 636f 6e74  ] = protect_cont
-000069e0: 656e 740a 2020 2020 5f61 6464 5f6d 6573  ent.    _add_mes
-000069f0: 7361 6765 5f74 6872 6561 645f 6964 2870  sage_thread_id(p
-00006a00: 6179 6c6f 6164 2c20 6d65 7373 6167 655f  ayload, message_
-00006a10: 7468 7265 6164 5f69 6429 0a20 2020 2069  thread_id).    i
-00006a20: 6620 6861 735f 7370 6f69 6c65 7220 6973  f has_spoiler is
-00006a30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00006a40: 2020 2070 6179 6c6f 6164 5b22 6861 735f     payload["has_
-00006a50: 7370 6f69 6c65 7222 5d20 3d20 6861 735f  spoiler"] = has_
-00006a60: 7370 6f69 6c65 720a 2020 2020 7265 7475  spoiler.    retu
-00006a70: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
-00006a80: 7428 746f 6b65 6e2c 206d 6574 686f 645f  t(token, method_
-00006a90: 7572 6c2c 2070 6172 616d 733d 7061 796c  url, params=payl
-00006aa0: 6f61 642c 2066 696c 6573 3d66 696c 6573  oad, files=files
-00006ab0: 2c20 6d65 7468 6f64 3d22 706f 7374 2229  , method="post")
-00006ac0: 0a0a 0a61 7379 6e63 2064 6566 2073 656e  ...async def sen
-00006ad0: 645f 616e 696d 6174 696f 6e28 0a20 2020  d_animation(.   
-00006ae0: 2074 6f6b 656e 2c0a 2020 2020 6368 6174   token,.    chat
-00006af0: 5f69 642c 0a20 2020 2064 6174 612c 0a20  _id,.    data,. 
-00006b00: 2020 2064 7572 6174 696f 6e3d 4e6f 6e65     duration=None
-00006b10: 2c0a 2020 2020 6361 7074 696f 6e3d 4e6f  ,.    caption=No
-00006b20: 6e65 2c0a 2020 2020 7265 706c 795f 746f  ne,.    reply_to
-00006b30: 5f6d 6573 7361 6765 5f69 643d 4e6f 6e65  _message_id=None
-00006b40: 2c0a 2020 2020 7265 706c 795f 6d61 726b  ,.    reply_mark
-00006b50: 7570 3d4e 6f6e 652c 0a20 2020 2070 6172  up=None,.    par
-00006b60: 7365 5f6d 6f64 653d 4e6f 6e65 2c0a 2020  se_mode=None,.  
-00006b70: 2020 6469 7361 626c 655f 6e6f 7469 6669    disable_notifi
-00006b80: 6361 7469 6f6e 3d4e 6f6e 652c 0a20 2020  cation=None,.   
-00006b90: 2074 696d 656f 7574 3d4e 6f6e 652c 0a20   timeout=None,. 
-00006ba0: 2020 2074 6875 6d62 3d4e 6f6e 652c 0a20     thumb=None,. 
-00006bb0: 2020 2063 6170 7469 6f6e 5f65 6e74 6974     caption_entit
-00006bc0: 6965 733d 4e6f 6e65 2c0a 2020 2020 616c  ies=None,.    al
-00006bd0: 6c6f 775f 7365 6e64 696e 675f 7769 7468  low_sending_with
-00006be0: 6f75 745f 7265 706c 793d 4e6f 6e65 2c0a  out_reply=None,.
-00006bf0: 2020 2020 7769 6474 683d 4e6f 6e65 2c0a      width=None,.
-00006c00: 2020 2020 6865 6967 6874 3d4e 6f6e 652c      height=None,
-00006c10: 0a20 2020 2070 726f 7465 6374 5f63 6f6e  .    protect_con
-00006c20: 7465 6e74 3d4e 6f6e 652c 0a20 2020 206d  tent=None,.    m
-00006c30: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
-00006c40: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-00006c50: 3d20 4e6f 6e65 2c0a 2020 2020 6861 735f  = None,.    has_
-00006c60: 7370 6f69 6c65 723a 204f 7074 696f 6e61  spoiler: Optiona
-00006c70: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a  l[bool] = None,.
-00006c80: 293a 0a20 2020 206d 6574 686f 645f 7572  ):.    method_ur
-00006c90: 6c20 3d20 7222 7365 6e64 416e 696d 6174  l = r"sendAnimat
-00006ca0: 696f 6e22 0a20 2020 2070 6179 6c6f 6164  ion".    payload
-00006cb0: 203d 207b 2263 6861 745f 6964 223a 2063   = {"chat_id": c
-00006cc0: 6861 745f 6964 7d0a 2020 2020 6669 6c65  hat_id}.    file
-00006cd0: 7320 3d20 4e6f 6e65 0a20 2020 2069 6620  s = None.    if 
-00006ce0: 6e6f 7420 7574 696c 2e69 735f 7374 7269  not util.is_stri
-00006cf0: 6e67 2864 6174 6129 3a0a 2020 2020 2020  ng(data):.      
-00006d00: 2020 6669 6c65 7320 3d20 7b22 616e 696d    files = {"anim
-00006d10: 6174 696f 6e22 3a20 6461 7461 7d0a 2020  ation": data}.  
-00006d20: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00006d30: 7061 796c 6f61 645b 2261 6e69 6d61 7469  payload["animati
-00006d40: 6f6e 225d 203d 2064 6174 610a 2020 2020  on"] = data.    
-00006d50: 6966 2064 7572 6174 696f 6e3a 0a20 2020  if duration:.   
-00006d60: 2020 2020 2070 6179 6c6f 6164 5b22 6475       payload["du
-00006d70: 7261 7469 6f6e 225d 203d 2064 7572 6174  ration"] = durat
-00006d80: 696f 6e0a 2020 2020 6966 2063 6170 7469  ion.    if capti
-00006d90: 6f6e 3a0a 2020 2020 2020 2020 7061 796c  on:.        payl
-00006da0: 6f61 645b 2263 6170 7469 6f6e 225d 203d  oad["caption"] =
-00006db0: 2063 6170 7469 6f6e 0a20 2020 2069 6620   caption.    if 
-00006dc0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-00006dd0: 5f69 643a 0a20 2020 2020 2020 2070 6179  _id:.        pay
-00006de0: 6c6f 6164 5b22 7265 706c 795f 746f 5f6d  load["reply_to_m
-00006df0: 6573 7361 6765 5f69 6422 5d20 3d20 7265  essage_id"] = re
-00006e00: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00006e10: 640a 2020 2020 6966 2072 6570 6c79 5f6d  d.    if reply_m
-00006e20: 6172 6b75 703a 0a20 2020 2020 2020 2070  arkup:.        p
-00006e30: 6179 6c6f 6164 5b22 7265 706c 795f 6d61  ayload["reply_ma
-00006e40: 726b 7570 225d 203d 2061 7761 6974 205f  rkup"] = await _
-00006e50: 636f 6e76 6572 745f 6d61 726b 7570 2872  convert_markup(r
-00006e60: 6570 6c79 5f6d 6172 6b75 7029 0a20 2020  eply_markup).   
-00006e70: 2069 6620 7061 7273 655f 6d6f 6465 3a0a   if parse_mode:.
-00006e80: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-00006e90: 2270 6172 7365 5f6d 6f64 6522 5d20 3d20  "parse_mode"] = 
-00006ea0: 7061 7273 655f 6d6f 6465 0a20 2020 2069  parse_mode.    i
-00006eb0: 6620 6469 7361 626c 655f 6e6f 7469 6669  f disable_notifi
-00006ec0: 6361 7469 6f6e 2069 7320 6e6f 7420 4e6f  cation is not No
-00006ed0: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
-00006ee0: 6f61 645b 2264 6973 6162 6c65 5f6e 6f74  oad["disable_not
-00006ef0: 6966 6963 6174 696f 6e22 5d20 3d20 6469  ification"] = di
-00006f00: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
-00006f10: 6f6e 0a20 2020 2069 6620 7469 6d65 6f75  on.    if timeou
-00006f20: 743a 0a20 2020 2020 2020 2070 6179 6c6f  t:.        paylo
-00006f30: 6164 5b22 7469 6d65 6f75 7422 5d20 3d20  ad["timeout"] = 
-00006f40: 7469 6d65 6f75 740a 2020 2020 6966 2074  timeout.    if t
-00006f50: 6875 6d62 3a0a 2020 2020 2020 2020 6966  humb:.        if
-00006f60: 206e 6f74 2075 7469 6c2e 6973 5f73 7472   not util.is_str
-00006f70: 696e 6728 7468 756d 6229 3a0a 2020 2020  ing(thumb):.    
-00006f80: 2020 2020 2020 2020 6966 2066 696c 6573          if files
-00006f90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006fa0: 2020 6669 6c65 735b 2274 6875 6d62 225d    files["thumb"]
-00006fb0: 203d 2074 6875 6d62 0a20 2020 2020 2020   = thumb.       
-00006fc0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00006fd0: 2020 2020 2020 2020 2020 2066 696c 6573             files
-00006fe0: 203d 207b 2274 6875 6d62 223a 2074 6875   = {"thumb": thu
-00006ff0: 6d62 7d0a 2020 2020 2020 2020 656c 7365  mb}.        else
-00007000: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-00007010: 796c 6f61 645b 2274 6875 6d62 225d 203d  yload["thumb"] =
-00007020: 2074 6875 6d62 0a20 2020 2069 6620 6361   thumb.    if ca
-00007030: 7074 696f 6e5f 656e 7469 7469 6573 3a0a  ption_entities:.
-00007040: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-00007050: 2263 6170 7469 6f6e 5f65 6e74 6974 6965  "caption_entitie
-00007060: 7322 5d20 3d20 6a73 6f6e 2e64 756d 7073  s"] = json.dumps
-00007070: 2874 7970 6573 2e4d 6573 7361 6765 456e  (types.MessageEn
-00007080: 7469 7479 2e74 6f5f 6c69 7374 5f6f 665f  tity.to_list_of_
-00007090: 6469 6374 7328 6361 7074 696f 6e5f 656e  dicts(caption_en
-000070a0: 7469 7469 6573 2929 0a20 2020 2069 6620  tities)).    if 
-000070b0: 616c 6c6f 775f 7365 6e64 696e 675f 7769  allow_sending_wi
-000070c0: 7468 6f75 745f 7265 706c 7920 6973 206e  thout_reply is n
-000070d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000070e0: 2070 6179 6c6f 6164 5b22 616c 6c6f 775f   payload["allow_
-000070f0: 7365 6e64 696e 675f 7769 7468 6f75 745f  sending_without_
-00007100: 7265 706c 7922 5d20 3d20 616c 6c6f 775f  reply"] = allow_
-00007110: 7365 6e64 696e 675f 7769 7468 6f75 745f  sending_without_
-00007120: 7265 706c 790a 2020 2020 6966 2077 6964  reply.    if wid
-00007130: 7468 3a0a 2020 2020 2020 2020 7061 796c  th:.        payl
-00007140: 6f61 645b 2277 6964 7468 225d 203d 2077  oad["width"] = w
-00007150: 6964 7468 0a20 2020 2069 6620 6865 6967  idth.    if heig
-00007160: 6874 3a0a 2020 2020 2020 2020 7061 796c  ht:.        payl
-00007170: 6f61 645b 2268 6569 6768 7422 5d20 3d20  oad["height"] = 
-00007180: 6865 6967 6874 0a20 2020 2069 6620 7072  height.    if pr
-00007190: 6f74 6563 745f 636f 6e74 656e 7420 6973  otect_content is
-000071a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000071b0: 2020 2070 6179 6c6f 6164 5b22 7072 6f74     payload["prot
-000071c0: 6563 745f 636f 6e74 656e 7422 5d20 3d20  ect_content"] = 
-000071d0: 7072 6f74 6563 745f 636f 6e74 656e 740a  protect_content.
-000071e0: 2020 2020 5f61 6464 5f6d 6573 7361 6765      _add_message
-000071f0: 5f74 6872 6561 645f 6964 2870 6179 6c6f  _thread_id(paylo
-00007200: 6164 2c20 6d65 7373 6167 655f 7468 7265  ad, message_thre
-00007210: 6164 5f69 6429 0a0a 2020 2020 6966 2068  ad_id)..    if h
-00007220: 6173 5f73 706f 696c 6572 2069 7320 6e6f  as_spoiler is no
-00007230: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00007240: 7061 796c 6f61 645b 2268 6173 5f73 706f  payload["has_spo
-00007250: 696c 6572 225d 203d 2068 6173 5f73 706f  iler"] = has_spo
-00007260: 696c 6572 0a20 2020 2072 6574 7572 6e20  iler.    return 
-00007270: 6177 6169 7420 5f72 6571 7565 7374 2874  await _request(t
-00007280: 6f6b 656e 2c20 6d65 7468 6f64 5f75 726c  oken, method_url
-00007290: 2c20 7061 7261 6d73 3d70 6179 6c6f 6164  , params=payload
-000072a0: 2c20 6669 6c65 733d 6669 6c65 732c 206d  , files=files, m
-000072b0: 6574 686f 643d 2270 6f73 7422 290a 0a0a  ethod="post")...
-000072c0: 6173 796e 6320 6465 6620 7365 6e64 5f76  async def send_v
-000072d0: 6f69 6365 280a 2020 2020 746f 6b65 6e2c  oice(.    token,
-000072e0: 0a20 2020 2063 6861 745f 6964 2c0a 2020  .    chat_id,.  
-000072f0: 2020 766f 6963 652c 0a20 2020 2063 6170    voice,.    cap
-00007300: 7469 6f6e 3d4e 6f6e 652c 0a20 2020 2064  tion=None,.    d
-00007310: 7572 6174 696f 6e3d 4e6f 6e65 2c0a 2020  uration=None,.  
-00007320: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
-00007330: 6765 5f69 643d 4e6f 6e65 2c0a 2020 2020  ge_id=None,.    
-00007340: 7265 706c 795f 6d61 726b 7570 3d4e 6f6e  reply_markup=Non
-00007350: 652c 0a20 2020 2070 6172 7365 5f6d 6f64  e,.    parse_mod
-00007360: 653d 4e6f 6e65 2c0a 2020 2020 6469 7361  e=None,.    disa
-00007370: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-00007380: 3d4e 6f6e 652c 0a20 2020 2074 696d 656f  =None,.    timeo
-00007390: 7574 3d4e 6f6e 652c 0a20 2020 2063 6170  ut=None,.    cap
-000073a0: 7469 6f6e 5f65 6e74 6974 6965 733d 4e6f  tion_entities=No
-000073b0: 6e65 2c0a 2020 2020 616c 6c6f 775f 7365  ne,.    allow_se
-000073c0: 6e64 696e 675f 7769 7468 6f75 745f 7265  nding_without_re
-000073d0: 706c 793d 4e6f 6e65 2c0a 2020 2020 7072  ply=None,.    pr
-000073e0: 6f74 6563 745f 636f 6e74 656e 743d 4e6f  otect_content=No
-000073f0: 6e65 2c0a 2020 2020 6d65 7373 6167 655f  ne,.    message_
-00007400: 7468 7265 6164 5f69 643a 204f 7074 696f  thread_id: Optio
-00007410: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-00007420: 0a29 3a0a 2020 2020 6d65 7468 6f64 5f75  .):.    method_u
-00007430: 726c 203d 2072 2273 656e 6456 6f69 6365  rl = r"sendVoice
-00007440: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
-00007450: 7b22 6368 6174 5f69 6422 3a20 6368 6174  {"chat_id": chat
-00007460: 5f69 647d 0a20 2020 2066 696c 6573 203d  _id}.    files =
-00007470: 204e 6f6e 650a 2020 2020 6966 206e 6f74   None.    if not
-00007480: 2075 7469 6c2e 6973 5f73 7472 696e 6728   util.is_string(
-00007490: 766f 6963 6529 3a0a 2020 2020 2020 2020  voice):.        
-000074a0: 6669 6c65 7320 3d20 7b22 766f 6963 6522  files = {"voice"
-000074b0: 3a20 766f 6963 657d 0a20 2020 2065 6c73  : voice}.    els
-000074c0: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-000074d0: 6164 5b22 766f 6963 6522 5d20 3d20 766f  ad["voice"] = vo
-000074e0: 6963 650a 2020 2020 6966 2063 6170 7469  ice.    if capti
-000074f0: 6f6e 3a0a 2020 2020 2020 2020 7061 796c  on:.        payl
-00007500: 6f61 645b 2263 6170 7469 6f6e 225d 203d  oad["caption"] =
-00007510: 2063 6170 7469 6f6e 0a20 2020 2069 6620   caption.    if 
-00007520: 6475 7261 7469 6f6e 3a0a 2020 2020 2020  duration:.      
-00007530: 2020 7061 796c 6f61 645b 2264 7572 6174    payload["durat
-00007540: 696f 6e22 5d20 3d20 6475 7261 7469 6f6e  ion"] = duration
-00007550: 0a20 2020 2069 6620 7265 706c 795f 746f  .    if reply_to
-00007560: 5f6d 6573 7361 6765 5f69 643a 0a20 2020  _message_id:.   
-00007570: 2020 2020 2070 6179 6c6f 6164 5b22 7265       payload["re
-00007580: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00007590: 6422 5d20 3d20 7265 706c 795f 746f 5f6d  d"] = reply_to_m
-000075a0: 6573 7361 6765 5f69 640a 2020 2020 6966  essage_id.    if
-000075b0: 2072 6570 6c79 5f6d 6172 6b75 703a 0a20   reply_markup:. 
-000075c0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-000075d0: 7265 706c 795f 6d61 726b 7570 225d 203d  reply_markup"] =
-000075e0: 2061 7761 6974 205f 636f 6e76 6572 745f   await _convert_
-000075f0: 6d61 726b 7570 2872 6570 6c79 5f6d 6172  markup(reply_mar
-00007600: 6b75 7029 0a20 2020 2069 6620 7061 7273  kup).    if pars
-00007610: 655f 6d6f 6465 3a0a 2020 2020 2020 2020  e_mode:.        
-00007620: 7061 796c 6f61 645b 2270 6172 7365 5f6d  payload["parse_m
-00007630: 6f64 6522 5d20 3d20 7061 7273 655f 6d6f  ode"] = parse_mo
-00007640: 6465 0a20 2020 2069 6620 6469 7361 626c  de.    if disabl
-00007650: 655f 6e6f 7469 6669 6361 7469 6f6e 2069  e_notification i
-00007660: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00007670: 2020 2020 7061 796c 6f61 645b 2264 6973      payload["dis
-00007680: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-00007690: 6e22 5d20 3d20 6469 7361 626c 655f 6e6f  n"] = disable_no
-000076a0: 7469 6669 6361 7469 6f6e 0a20 2020 2069  tification.    i
-000076b0: 6620 7469 6d65 6f75 743a 0a20 2020 2020  f timeout:.     
-000076c0: 2020 2070 6179 6c6f 6164 5b22 7469 6d65     payload["time
-000076d0: 6f75 7422 5d20 3d20 7469 6d65 6f75 740a  out"] = timeout.
-000076e0: 2020 2020 6966 2063 6170 7469 6f6e 5f65      if caption_e
-000076f0: 6e74 6974 6965 733a 0a20 2020 2020 2020  ntities:.       
-00007700: 2070 6179 6c6f 6164 5b22 6361 7074 696f   payload["captio
-00007710: 6e5f 656e 7469 7469 6573 225d 203d 206a  n_entities"] = j
-00007720: 736f 6e2e 6475 6d70 7328 7479 7065 732e  son.dumps(types.
-00007730: 4d65 7373 6167 6545 6e74 6974 792e 746f  MessageEntity.to
-00007740: 5f6c 6973 745f 6f66 5f64 6963 7473 2863  _list_of_dicts(c
-00007750: 6170 7469 6f6e 5f65 6e74 6974 6965 7329  aption_entities)
-00007760: 290a 2020 2020 6966 2061 6c6c 6f77 5f73  ).    if allow_s
-00007770: 656e 6469 6e67 5f77 6974 686f 7574 5f72  ending_without_r
-00007780: 6570 6c79 2069 7320 6e6f 7420 4e6f 6e65  eply is not None
-00007790: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-000077a0: 645b 2261 6c6c 6f77 5f73 656e 6469 6e67  d["allow_sending
-000077b0: 5f77 6974 686f 7574 5f72 6570 6c79 225d  _without_reply"]
-000077c0: 203d 2061 6c6c 6f77 5f73 656e 6469 6e67   = allow_sending
-000077d0: 5f77 6974 686f 7574 5f72 6570 6c79 0a20  _without_reply. 
-000077e0: 2020 2069 6620 7072 6f74 6563 745f 636f     if protect_co
-000077f0: 6e74 656e 7420 6973 206e 6f74 204e 6f6e  ntent is not Non
-00007800: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-00007810: 6164 5b22 7072 6f74 6563 745f 636f 6e74  ad["protect_cont
-00007820: 656e 7422 5d20 3d20 7072 6f74 6563 745f  ent"] = protect_
-00007830: 636f 6e74 656e 740a 2020 2020 5f61 6464  content.    _add
-00007840: 5f6d 6573 7361 6765 5f74 6872 6561 645f  _message_thread_
-00007850: 6964 2870 6179 6c6f 6164 2c20 6d65 7373  id(payload, mess
-00007860: 6167 655f 7468 7265 6164 5f69 6429 0a20  age_thread_id). 
-00007870: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00007880: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
-00007890: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
-000078a0: 6d73 3d70 6179 6c6f 6164 2c20 6669 6c65  ms=payload, file
-000078b0: 733d 6669 6c65 732c 206d 6574 686f 643d  s=files, method=
-000078c0: 2270 6f73 7422 290a 0a0a 6173 796e 6320  "post")...async 
-000078d0: 6465 6620 7365 6e64 5f76 6964 656f 5f6e  def send_video_n
-000078e0: 6f74 6528 0a20 2020 2074 6f6b 656e 2c0a  ote(.    token,.
-000078f0: 2020 2020 6368 6174 5f69 642c 0a20 2020      chat_id,.   
-00007900: 2064 6174 612c 0a20 2020 2064 7572 6174   data,.    durat
-00007910: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 6c65  ion=None,.    le
-00007920: 6e67 7468 3d4e 6f6e 652c 0a20 2020 2072  ngth=None,.    r
-00007930: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
-00007940: 6964 3d4e 6f6e 652c 0a20 2020 2072 6570  id=None,.    rep
-00007950: 6c79 5f6d 6172 6b75 703d 4e6f 6e65 2c0a  ly_markup=None,.
-00007960: 2020 2020 6469 7361 626c 655f 6e6f 7469      disable_noti
-00007970: 6669 6361 7469 6f6e 3d4e 6f6e 652c 0a20  fication=None,. 
-00007980: 2020 2074 696d 656f 7574 3d4e 6f6e 652c     timeout=None,
-00007990: 0a20 2020 2074 6875 6d62 3d4e 6f6e 652c  .    thumb=None,
-000079a0: 0a20 2020 2061 6c6c 6f77 5f73 656e 6469  .    allow_sendi
-000079b0: 6e67 5f77 6974 686f 7574 5f72 6570 6c79  ng_without_reply
-000079c0: 3d4e 6f6e 652c 0a20 2020 2070 726f 7465  =None,.    prote
-000079d0: 6374 5f63 6f6e 7465 6e74 3d4e 6f6e 652c  ct_content=None,
-000079e0: 0a20 2020 206d 6573 7361 6765 5f74 6872  .    message_thr
-000079f0: 6561 645f 6964 3a20 4f70 7469 6f6e 616c  ead_id: Optional
-00007a00: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 293a  [int] = None,.):
-00007a10: 0a20 2020 206d 6574 686f 645f 7572 6c20  .    method_url 
-00007a20: 3d20 7222 7365 6e64 5669 6465 6f4e 6f74  = r"sendVideoNot
-00007a30: 6522 0a20 2020 2070 6179 6c6f 6164 203d  e".    payload =
-00007a40: 207b 2263 6861 745f 6964 223a 2063 6861   {"chat_id": cha
-00007a50: 745f 6964 7d0a 2020 2020 6669 6c65 7320  t_id}.    files 
-00007a60: 3d20 4e6f 6e65 0a20 2020 2069 6620 6e6f  = None.    if no
-00007a70: 7420 7574 696c 2e69 735f 7374 7269 6e67  t util.is_string
-00007a80: 2864 6174 6129 3a0a 2020 2020 2020 2020  (data):.        
-00007a90: 6669 6c65 7320 3d20 7b22 7669 6465 6f5f  files = {"video_
-00007aa0: 6e6f 7465 223a 2064 6174 617d 0a20 2020  note": data}.   
-00007ab0: 2065 6c73 653a 0a20 2020 2020 2020 2070   else:.        p
-00007ac0: 6179 6c6f 6164 5b22 7669 6465 6f5f 6e6f  ayload["video_no
-00007ad0: 7465 225d 203d 2064 6174 610a 2020 2020  te"] = data.    
-00007ae0: 6966 2064 7572 6174 696f 6e3a 0a20 2020  if duration:.   
-00007af0: 2020 2020 2070 6179 6c6f 6164 5b22 6475       payload["du
-00007b00: 7261 7469 6f6e 225d 203d 2064 7572 6174  ration"] = durat
-00007b10: 696f 6e0a 2020 2020 6966 206c 656e 6774  ion.    if lengt
-00007b20: 6820 616e 6420 2873 7472 286c 656e 6774  h and (str(lengt
-00007b30: 6829 2e69 7364 6967 6974 2829 2061 6e64  h).isdigit() and
-00007b40: 2069 6e74 286c 656e 6774 6829 203c 3d20   int(length) <= 
-00007b50: 3633 3929 3a0a 2020 2020 2020 2020 7061  639):.        pa
-00007b60: 796c 6f61 645b 226c 656e 6774 6822 5d20  yload["length"] 
-00007b70: 3d20 6c65 6e67 7468 0a20 2020 2065 6c73  = length.    els
-00007b80: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-00007b90: 6164 5b22 6c65 6e67 7468 225d 203d 2036  ad["length"] = 6
-00007ba0: 3339 2020 2320 7365 656d 7320 6c69 6b65  39  # seems like
-00007bb0: 2069 7420 6973 204d 4158 206c 656e 6774   it is MAX lengt
-00007bc0: 6820 7369 7a65 0a20 2020 2069 6620 7265  h size.    if re
-00007bd0: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00007be0: 643a 0a20 2020 2020 2020 2070 6179 6c6f  d:.        paylo
-00007bf0: 6164 5b22 7265 706c 795f 746f 5f6d 6573  ad["reply_to_mes
-00007c00: 7361 6765 5f69 6422 5d20 3d20 7265 706c  sage_id"] = repl
-00007c10: 795f 746f 5f6d 6573 7361 6765 5f69 640a  y_to_message_id.
-00007c20: 2020 2020 6966 2072 6570 6c79 5f6d 6172      if reply_mar
-00007c30: 6b75 703a 0a20 2020 2020 2020 2070 6179  kup:.        pay
-00007c40: 6c6f 6164 5b22 7265 706c 795f 6d61 726b  load["reply_mark
-00007c50: 7570 225d 203d 2061 7761 6974 205f 636f  up"] = await _co
-00007c60: 6e76 6572 745f 6d61 726b 7570 2872 6570  nvert_markup(rep
-00007c70: 6c79 5f6d 6172 6b75 7029 0a20 2020 2069  ly_markup).    i
-00007c80: 6620 6469 7361 626c 655f 6e6f 7469 6669  f disable_notifi
-00007c90: 6361 7469 6f6e 2069 7320 6e6f 7420 4e6f  cation is not No
-00007ca0: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
-00007cb0: 6f61 645b 2264 6973 6162 6c65 5f6e 6f74  oad["disable_not
-00007cc0: 6966 6963 6174 696f 6e22 5d20 3d20 6469  ification"] = di
-00007cd0: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
-00007ce0: 6f6e 0a20 2020 2069 6620 7469 6d65 6f75  on.    if timeou
-00007cf0: 743a 0a20 2020 2020 2020 2070 6179 6c6f  t:.        paylo
-00007d00: 6164 5b22 7469 6d65 6f75 7422 5d20 3d20  ad["timeout"] = 
-00007d10: 7469 6d65 6f75 740a 2020 2020 6966 2074  timeout.    if t
-00007d20: 6875 6d62 3a0a 2020 2020 2020 2020 6966  humb:.        if
-00007d30: 206e 6f74 2075 7469 6c2e 6973 5f73 7472   not util.is_str
-00007d40: 696e 6728 7468 756d 6229 3a0a 2020 2020  ing(thumb):.    
-00007d50: 2020 2020 2020 2020 6966 2066 696c 6573          if files
-00007d60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007d70: 2020 6669 6c65 735b 2274 6875 6d62 225d    files["thumb"]
-00007d80: 203d 2074 6875 6d62 0a20 2020 2020 2020   = thumb.       
-00007d90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00007da0: 2020 2020 2020 2020 2020 2066 696c 6573             files
-00007db0: 203d 207b 2274 6875 6d62 223a 2074 6875   = {"thumb": thu
-00007dc0: 6d62 7d0a 2020 2020 2020 2020 656c 7365  mb}.        else
-00007dd0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-00007de0: 796c 6f61 645b 2274 6875 6d62 225d 203d  yload["thumb"] =
-00007df0: 2074 6875 6d62 0a20 2020 2069 6620 616c   thumb.    if al
-00007e00: 6c6f 775f 7365 6e64 696e 675f 7769 7468  low_sending_with
-00007e10: 6f75 745f 7265 706c 7920 6973 206e 6f74  out_reply is not
-00007e20: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
-00007e30: 6179 6c6f 6164 5b22 616c 6c6f 775f 7365  ayload["allow_se
-00007e40: 6e64 696e 675f 7769 7468 6f75 745f 7265  nding_without_re
-00007e50: 706c 7922 5d20 3d20 616c 6c6f 775f 7365  ply"] = allow_se
-00007e60: 6e64 696e 675f 7769 7468 6f75 745f 7265  nding_without_re
-00007e70: 706c 790a 2020 2020 6966 2070 726f 7465  ply.    if prote
-00007e80: 6374 5f63 6f6e 7465 6e74 2069 7320 6e6f  ct_content is no
-00007e90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00007ea0: 7061 796c 6f61 645b 2270 726f 7465 6374  payload["protect
-00007eb0: 5f63 6f6e 7465 6e74 225d 203d 2070 726f  _content"] = pro
-00007ec0: 7465 6374 5f63 6f6e 7465 6e74 0a20 2020  tect_content.   
-00007ed0: 205f 6164 645f 6d65 7373 6167 655f 7468   _add_message_th
-00007ee0: 7265 6164 5f69 6428 7061 796c 6f61 642c  read_id(payload,
-00007ef0: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
-00007f00: 6964 290a 2020 2020 7265 7475 726e 2061  id).    return a
-00007f10: 7761 6974 205f 7265 7175 6573 7428 746f  wait _request(to
-00007f20: 6b65 6e2c 206d 6574 686f 645f 7572 6c2c  ken, method_url,
-00007f30: 2070 6172 616d 733d 7061 796c 6f61 642c   params=payload,
-00007f40: 2066 696c 6573 3d66 696c 6573 2c20 6d65   files=files, me
-00007f50: 7468 6f64 3d22 706f 7374 2229 0a0a 0a61  thod="post")...a
-00007f60: 7379 6e63 2064 6566 2073 656e 645f 6175  sync def send_au
-00007f70: 6469 6f28 0a20 2020 2074 6f6b 656e 2c0a  dio(.    token,.
-00007f80: 2020 2020 6368 6174 5f69 642c 0a20 2020      chat_id,.   
-00007f90: 2061 7564 696f 2c0a 2020 2020 6361 7074   audio,.    capt
-00007fa0: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 6475  ion=None,.    du
-00007fb0: 7261 7469 6f6e 3d4e 6f6e 652c 0a20 2020  ration=None,.   
-00007fc0: 2070 6572 666f 726d 6572 3d4e 6f6e 652c   performer=None,
-00007fd0: 0a20 2020 2074 6974 6c65 3d4e 6f6e 652c  .    title=None,
-00007fe0: 0a20 2020 2072 6570 6c79 5f74 6f5f 6d65  .    reply_to_me
-00007ff0: 7373 6167 655f 6964 3d4e 6f6e 652c 0a20  ssage_id=None,. 
-00008000: 2020 2072 6570 6c79 5f6d 6172 6b75 703d     reply_markup=
-00008010: 4e6f 6e65 2c0a 2020 2020 7061 7273 655f  None,.    parse_
-00008020: 6d6f 6465 3d4e 6f6e 652c 0a20 2020 2064  mode=None,.    d
-00008030: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
-00008040: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 7469  ion=None,.    ti
-00008050: 6d65 6f75 743d 4e6f 6e65 2c0a 2020 2020  meout=None,.    
-00008060: 7468 756d 623d 4e6f 6e65 2c0a 2020 2020  thumb=None,.    
-00008070: 6361 7074 696f 6e5f 656e 7469 7469 6573  caption_entities
-00008080: 3d4e 6f6e 652c 0a20 2020 2061 6c6c 6f77  =None,.    allow
-00008090: 5f73 656e 6469 6e67 5f77 6974 686f 7574  _sending_without
-000080a0: 5f72 6570 6c79 3d4e 6f6e 652c 0a20 2020  _reply=None,.   
-000080b0: 2070 726f 7465 6374 5f63 6f6e 7465 6e74   protect_content
-000080c0: 3d4e 6f6e 652c 0a20 2020 206d 6573 7361  =None,.    messa
-000080d0: 6765 5f74 6872 6561 645f 6964 3a20 4f70  ge_thread_id: Op
-000080e0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-000080f0: 6e65 2c0a 293a 0a20 2020 206d 6574 686f  ne,.):.    metho
-00008100: 645f 7572 6c20 3d20 7222 7365 6e64 4175  d_url = r"sendAu
-00008110: 6469 6f22 0a20 2020 2070 6179 6c6f 6164  dio".    payload
-00008120: 203d 207b 2263 6861 745f 6964 223a 2063   = {"chat_id": c
-00008130: 6861 745f 6964 7d0a 2020 2020 6669 6c65  hat_id}.    file
-00008140: 7320 3d20 4e6f 6e65 0a20 2020 2069 6620  s = None.    if 
-00008150: 6e6f 7420 7574 696c 2e69 735f 7374 7269  not util.is_stri
-00008160: 6e67 2861 7564 696f 293a 0a20 2020 2020  ng(audio):.     
-00008170: 2020 2066 696c 6573 203d 207b 2261 7564     files = {"aud
-00008180: 696f 223a 2061 7564 696f 7d0a 2020 2020  io": audio}.    
-00008190: 656c 7365 3a0a 2020 2020 2020 2020 7061  else:.        pa
-000081a0: 796c 6f61 645b 2261 7564 696f 225d 203d  yload["audio"] =
-000081b0: 2061 7564 696f 0a20 2020 2069 6620 6361   audio.    if ca
-000081c0: 7074 696f 6e3a 0a20 2020 2020 2020 2070  ption:.        p
-000081d0: 6179 6c6f 6164 5b22 6361 7074 696f 6e22  ayload["caption"
-000081e0: 5d20 3d20 6361 7074 696f 6e0a 2020 2020  ] = caption.    
-000081f0: 6966 2064 7572 6174 696f 6e3a 0a20 2020  if duration:.   
-00008200: 2020 2020 2070 6179 6c6f 6164 5b22 6475       payload["du
-00008210: 7261 7469 6f6e 225d 203d 2064 7572 6174  ration"] = durat
-00008220: 696f 6e0a 2020 2020 6966 2070 6572 666f  ion.    if perfo
-00008230: 726d 6572 3a0a 2020 2020 2020 2020 7061  rmer:.        pa
-00008240: 796c 6f61 645b 2270 6572 666f 726d 6572  yload["performer
-00008250: 225d 203d 2070 6572 666f 726d 6572 0a20  "] = performer. 
-00008260: 2020 2069 6620 7469 746c 653a 0a20 2020     if title:.   
-00008270: 2020 2020 2070 6179 6c6f 6164 5b22 7469       payload["ti
-00008280: 746c 6522 5d20 3d20 7469 746c 650a 2020  tle"] = title.  
-00008290: 2020 6966 2072 6570 6c79 5f74 6f5f 6d65    if reply_to_me
-000082a0: 7373 6167 655f 6964 3a0a 2020 2020 2020  ssage_id:.      
-000082b0: 2020 7061 796c 6f61 645b 2272 6570 6c79    payload["reply
-000082c0: 5f74 6f5f 6d65 7373 6167 655f 6964 225d  _to_message_id"]
-000082d0: 203d 2072 6570 6c79 5f74 6f5f 6d65 7373   = reply_to_mess
-000082e0: 6167 655f 6964 0a20 2020 2069 6620 7265  age_id.    if re
-000082f0: 706c 795f 6d61 726b 7570 3a0a 2020 2020  ply_markup:.    
-00008300: 2020 2020 7061 796c 6f61 645b 2272 6570      payload["rep
-00008310: 6c79 5f6d 6172 6b75 7022 5d20 3d20 6177  ly_markup"] = aw
-00008320: 6169 7420 5f63 6f6e 7665 7274 5f6d 6172  ait _convert_mar
-00008330: 6b75 7028 7265 706c 795f 6d61 726b 7570  kup(reply_markup
-00008340: 290a 2020 2020 6966 2070 6172 7365 5f6d  ).    if parse_m
-00008350: 6f64 653a 0a20 2020 2020 2020 2070 6179  ode:.        pay
-00008360: 6c6f 6164 5b22 7061 7273 655f 6d6f 6465  load["parse_mode
-00008370: 225d 203d 2070 6172 7365 5f6d 6f64 650a  "] = parse_mode.
-00008380: 2020 2020 6966 2064 6973 6162 6c65 5f6e      if disable_n
-00008390: 6f74 6966 6963 6174 696f 6e20 6973 206e  otification is n
-000083a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000083b0: 2070 6179 6c6f 6164 5b22 6469 7361 626c   payload["disabl
-000083c0: 655f 6e6f 7469 6669 6361 7469 6f6e 225d  e_notification"]
-000083d0: 203d 2064 6973 6162 6c65 5f6e 6f74 6966   = disable_notif
-000083e0: 6963 6174 696f 6e0a 2020 2020 6966 2074  ication.    if t
-000083f0: 696d 656f 7574 3a0a 2020 2020 2020 2020  imeout:.        
-00008400: 7061 796c 6f61 645b 2274 696d 656f 7574  payload["timeout
-00008410: 225d 203d 2074 696d 656f 7574 0a20 2020  "] = timeout.   
-00008420: 2069 6620 7468 756d 623a 0a20 2020 2020   if thumb:.     
-00008430: 2020 2069 6620 6e6f 7420 7574 696c 2e69     if not util.i
-00008440: 735f 7374 7269 6e67 2874 6875 6d62 293a  s_string(thumb):
-00008450: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00008460: 6669 6c65 733a 0a20 2020 2020 2020 2020  files:.         
-00008470: 2020 2020 2020 2066 696c 6573 5b22 7468         files["th
-00008480: 756d 6222 5d20 3d20 7468 756d 620a 2020  umb"] = thumb.  
-00008490: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000084a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084b0: 6669 6c65 7320 3d20 7b22 7468 756d 6222  files = {"thumb"
-000084c0: 3a20 7468 756d 627d 0a20 2020 2020 2020  : thumb}.       
-000084d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000084e0: 2020 2070 6179 6c6f 6164 5b22 7468 756d     payload["thum
-000084f0: 6222 5d20 3d20 7468 756d 620a 2020 2020  b"] = thumb.    
-00008500: 6966 2063 6170 7469 6f6e 5f65 6e74 6974  if caption_entit
-00008510: 6965 733a 0a20 2020 2020 2020 2070 6179  ies:.        pay
-00008520: 6c6f 6164 5b22 6361 7074 696f 6e5f 656e  load["caption_en
-00008530: 7469 7469 6573 225d 203d 206a 736f 6e2e  tities"] = json.
-00008540: 6475 6d70 7328 7479 7065 732e 4d65 7373  dumps(types.Mess
-00008550: 6167 6545 6e74 6974 792e 746f 5f6c 6973  ageEntity.to_lis
-00008560: 745f 6f66 5f64 6963 7473 2863 6170 7469  t_of_dicts(capti
-00008570: 6f6e 5f65 6e74 6974 6965 7329 290a 2020  on_entities)).  
-00008580: 2020 6966 2061 6c6c 6f77 5f73 656e 6469    if allow_sendi
-00008590: 6e67 5f77 6974 686f 7574 5f72 6570 6c79  ng_without_reply
-000085a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000085b0: 2020 2020 2020 7061 796c 6f61 645b 2261        payload["a
-000085c0: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
-000085d0: 686f 7574 5f72 6570 6c79 225d 203d 2061  hout_reply"] = a
-000085e0: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
-000085f0: 686f 7574 5f72 6570 6c79 0a20 2020 2069  hout_reply.    i
-00008600: 6620 7072 6f74 6563 745f 636f 6e74 656e  f protect_conten
-00008610: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
-00008620: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-00008630: 7072 6f74 6563 745f 636f 6e74 656e 7422  protect_content"
-00008640: 5d20 3d20 7072 6f74 6563 745f 636f 6e74  ] = protect_cont
-00008650: 656e 740a 2020 2020 5f61 6464 5f6d 6573  ent.    _add_mes
-00008660: 7361 6765 5f74 6872 6561 645f 6964 2870  sage_thread_id(p
-00008670: 6179 6c6f 6164 2c20 6d65 7373 6167 655f  ayload, message_
-00008680: 7468 7265 6164 5f69 6429 0a20 2020 2072  thread_id).    r
-00008690: 6574 7572 6e20 6177 6169 7420 5f72 6571  eturn await _req
-000086a0: 7565 7374 2874 6f6b 656e 2c20 6d65 7468  uest(token, meth
-000086b0: 6f64 5f75 726c 2c20 7061 7261 6d73 3d70  od_url, params=p
-000086c0: 6179 6c6f 6164 2c20 6669 6c65 733d 6669  ayload, files=fi
-000086d0: 6c65 732c 206d 6574 686f 643d 2270 6f73  les, method="pos
-000086e0: 7422 290a 0a0a 6173 796e 6320 6465 6620  t")...async def 
-000086f0: 7365 6e64 5f64 6174 6128 0a20 2020 2074  send_data(.    t
-00008700: 6f6b 656e 2c0a 2020 2020 6368 6174 5f69  oken,.    chat_i
-00008710: 642c 0a20 2020 2064 6174 612c 0a20 2020  d,.    data,.   
-00008720: 2064 6174 615f 7479 7065 2c0a 2020 2020   data_type,.    
-00008730: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-00008740: 5f69 643d 4e6f 6e65 2c0a 2020 2020 7265  _id=None,.    re
-00008750: 706c 795f 6d61 726b 7570 3d4e 6f6e 652c  ply_markup=None,
-00008760: 0a20 2020 2070 6172 7365 5f6d 6f64 653d  .    parse_mode=
-00008770: 4e6f 6e65 2c0a 2020 2020 6469 7361 626c  None,.    disabl
-00008780: 655f 6e6f 7469 6669 6361 7469 6f6e 3d4e  e_notification=N
-00008790: 6f6e 652c 0a20 2020 2074 696d 656f 7574  one,.    timeout
-000087a0: 3d4e 6f6e 652c 0a20 2020 2063 6170 7469  =None,.    capti
-000087b0: 6f6e 3d4e 6f6e 652c 0a20 2020 2074 6875  on=None,.    thu
-000087c0: 6d62 3d4e 6f6e 652c 0a20 2020 2063 6170  mb=None,.    cap
-000087d0: 7469 6f6e 5f65 6e74 6974 6965 733d 4e6f  tion_entities=No
-000087e0: 6e65 2c0a 2020 2020 616c 6c6f 775f 7365  ne,.    allow_se
-000087f0: 6e64 696e 675f 7769 7468 6f75 745f 7265  nding_without_re
-00008800: 706c 793d 4e6f 6e65 2c0a 2020 2020 6469  ply=None,.    di
-00008810: 7361 626c 655f 636f 6e74 656e 745f 7479  sable_content_ty
-00008820: 7065 5f64 6574 6563 7469 6f6e 3d4e 6f6e  pe_detection=Non
-00008830: 652c 0a20 2020 2076 6973 6962 6c65 5f66  e,.    visible_f
-00008840: 696c 655f 6e61 6d65 3d4e 6f6e 652c 0a20  ile_name=None,. 
-00008850: 2020 2070 726f 7465 6374 5f63 6f6e 7465     protect_conte
-00008860: 6e74 3d4e 6f6e 652c 0a20 2020 206d 6573  nt=None,.    mes
-00008870: 7361 6765 5f74 6872 6561 645f 6964 3a20  sage_thread_id: 
-00008880: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00008890: 4e6f 6e65 2c0a 293a 0a20 2020 206d 6574  None,.):.    met
-000088a0: 686f 645f 7572 6c20 3d20 6177 6169 7420  hod_url = await 
-000088b0: 6765 745f 6d65 7468 6f64 5f62 795f 7479  get_method_by_ty
-000088c0: 7065 2864 6174 615f 7479 7065 290a 2020  pe(data_type).  
-000088d0: 2020 7061 796c 6f61 6420 3d20 7b22 6368    payload = {"ch
-000088e0: 6174 5f69 6422 3a20 6368 6174 5f69 647d  at_id": chat_id}
-000088f0: 0a20 2020 2066 696c 6573 203d 204e 6f6e  .    files = Non
-00008900: 650a 2020 2020 6966 206e 6f74 2075 7469  e.    if not uti
-00008910: 6c2e 6973 5f73 7472 696e 6728 6461 7461  l.is_string(data
-00008920: 293a 0a20 2020 2020 2020 2066 696c 655f  ):.        file_
-00008930: 6461 7461 203d 2064 6174 610a 2020 2020  data = data.    
-00008940: 2020 2020 6966 2076 6973 6962 6c65 5f66      if visible_f
-00008950: 696c 655f 6e61 6d65 3a0a 2020 2020 2020  ile_name:.      
-00008960: 2020 2020 2020 6669 6c65 5f64 6174 6120        file_data 
-00008970: 3d20 2876 6973 6962 6c65 5f66 696c 655f  = (visible_file_
-00008980: 6e61 6d65 2c20 6461 7461 290a 2020 2020  name, data).    
-00008990: 2020 2020 6669 6c65 7320 3d20 7b64 6174      files = {dat
-000089a0: 615f 7479 7065 3a20 6669 6c65 5f64 6174  a_type: file_dat
-000089b0: 617d 0a20 2020 2065 6c73 653a 0a20 2020  a}.    else:.   
-000089c0: 2020 2020 2070 6179 6c6f 6164 5b64 6174       payload[dat
-000089d0: 615f 7479 7065 5d20 3d20 6461 7461 0a20  a_type] = data. 
-000089e0: 2020 2069 6620 7265 706c 795f 746f 5f6d     if reply_to_m
-000089f0: 6573 7361 6765 5f69 643a 0a20 2020 2020  essage_id:.     
-00008a00: 2020 2070 6179 6c6f 6164 5b22 7265 706c     payload["repl
-00008a10: 795f 746f 5f6d 6573 7361 6765 5f69 6422  y_to_message_id"
-00008a20: 5d20 3d20 7265 706c 795f 746f 5f6d 6573  ] = reply_to_mes
-00008a30: 7361 6765 5f69 640a 2020 2020 6966 2072  sage_id.    if r
-00008a40: 6570 6c79 5f6d 6172 6b75 703a 0a20 2020  eply_markup:.   
-00008a50: 2020 2020 2070 6179 6c6f 6164 5b22 7265       payload["re
-00008a60: 706c 795f 6d61 726b 7570 225d 203d 2061  ply_markup"] = a
-00008a70: 7761 6974 205f 636f 6e76 6572 745f 6d61  wait _convert_ma
-00008a80: 726b 7570 2872 6570 6c79 5f6d 6172 6b75  rkup(reply_marku
-00008a90: 7029 0a20 2020 2069 6620 7061 7273 655f  p).    if parse_
-00008aa0: 6d6f 6465 2061 6e64 2064 6174 615f 7479  mode and data_ty
-00008ab0: 7065 203d 3d20 2264 6f63 756d 656e 7422  pe == "document"
-00008ac0: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-00008ad0: 645b 2270 6172 7365 5f6d 6f64 6522 5d20  d["parse_mode"] 
-00008ae0: 3d20 7061 7273 655f 6d6f 6465 0a20 2020  = parse_mode.   
-00008af0: 2069 6620 6469 7361 626c 655f 6e6f 7469   if disable_noti
-00008b00: 6669 6361 7469 6f6e 2069 7320 6e6f 7420  fication is not 
-00008b10: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
-00008b20: 796c 6f61 645b 2264 6973 6162 6c65 5f6e  yload["disable_n
-00008b30: 6f74 6966 6963 6174 696f 6e22 5d20 3d20  otification"] = 
-00008b40: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-00008b50: 7469 6f6e 0a20 2020 2069 6620 7469 6d65  tion.    if time
-00008b60: 6f75 743a 0a20 2020 2020 2020 2070 6179  out:.        pay
-00008b70: 6c6f 6164 5b22 7469 6d65 6f75 7422 5d20  load["timeout"] 
-00008b80: 3d20 7469 6d65 6f75 740a 2020 2020 6966  = timeout.    if
-00008b90: 2063 6170 7469 6f6e 3a0a 2020 2020 2020   caption:.      
-00008ba0: 2020 7061 796c 6f61 645b 2263 6170 7469    payload["capti
-00008bb0: 6f6e 225d 203d 2063 6170 7469 6f6e 0a20  on"] = caption. 
-00008bc0: 2020 2069 6620 7468 756d 623a 0a20 2020     if thumb:.   
-00008bd0: 2020 2020 2069 6620 6e6f 7420 7574 696c       if not util
-00008be0: 2e69 735f 7374 7269 6e67 2874 6875 6d62  .is_string(thumb
-00008bf0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00008c00: 6620 6669 6c65 733a 0a20 2020 2020 2020  f files:.       
-00008c10: 2020 2020 2020 2020 2066 696c 6573 5b22           files["
-00008c20: 7468 756d 6222 5d20 3d20 7468 756d 620a  thumb"] = thumb.
-00008c30: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00008c40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008c50: 2020 6669 6c65 7320 3d20 7b22 7468 756d    files = {"thum
-00008c60: 6222 3a20 7468 756d 627d 0a20 2020 2020  b": thumb}.     
-00008c70: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00008c80: 2020 2020 2070 6179 6c6f 6164 5b22 7468       payload["th
-00008c90: 756d 6222 5d20 3d20 7468 756d 620a 2020  umb"] = thumb.  
-00008ca0: 2020 6966 2063 6170 7469 6f6e 5f65 6e74    if caption_ent
-00008cb0: 6974 6965 733a 0a20 2020 2020 2020 2070  ities:.        p
-00008cc0: 6179 6c6f 6164 5b22 6361 7074 696f 6e5f  ayload["caption_
-00008cd0: 656e 7469 7469 6573 225d 203d 206a 736f  entities"] = jso
-00008ce0: 6e2e 6475 6d70 7328 7479 7065 732e 4d65  n.dumps(types.Me
-00008cf0: 7373 6167 6545 6e74 6974 792e 746f 5f6c  ssageEntity.to_l
-00008d00: 6973 745f 6f66 5f64 6963 7473 2863 6170  ist_of_dicts(cap
-00008d10: 7469 6f6e 5f65 6e74 6974 6965 7329 290a  tion_entities)).
-00008d20: 2020 2020 6966 2061 6c6c 6f77 5f73 656e      if allow_sen
-00008d30: 6469 6e67 5f77 6974 686f 7574 5f72 6570  ding_without_rep
-00008d40: 6c79 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ly is not None:.
-00008d50: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-00008d60: 2261 6c6c 6f77 5f73 656e 6469 6e67 5f77  "allow_sending_w
-00008d70: 6974 686f 7574 5f72 6570 6c79 225d 203d  ithout_reply"] =
-00008d80: 2061 6c6c 6f77 5f73 656e 6469 6e67 5f77   allow_sending_w
-00008d90: 6974 686f 7574 5f72 6570 6c79 0a20 2020  ithout_reply.   
-00008da0: 2069 6620 7072 6f74 6563 745f 636f 6e74   if protect_cont
-00008db0: 656e 7420 6973 206e 6f74 204e 6f6e 653a  ent is not None:
-00008dc0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00008dd0: 5b22 7072 6f74 6563 745f 636f 6e74 656e  ["protect_conten
-00008de0: 7422 5d20 3d20 7072 6f74 6563 745f 636f  t"] = protect_co
-00008df0: 6e74 656e 740a 2020 2020 6966 206d 6574  ntent.    if met
-00008e00: 686f 645f 7572 6c20 3d3d 2022 7365 6e64  hod_url == "send
-00008e10: 446f 6375 6d65 6e74 2220 616e 6420 6469  Document" and di
-00008e20: 7361 626c 655f 636f 6e74 656e 745f 7479  sable_content_ty
-00008e30: 7065 5f64 6574 6563 7469 6f6e 2069 7320  pe_detection is 
-00008e40: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00008e50: 2020 7061 796c 6f61 645b 2264 6973 6162    payload["disab
-00008e60: 6c65 5f63 6f6e 7465 6e74 5f74 7970 655f  le_content_type_
-00008e70: 6465 7465 6374 696f 6e22 5d20 3d20 6469  detection"] = di
-00008e80: 7361 626c 655f 636f 6e74 656e 745f 7479  sable_content_ty
-00008e90: 7065 5f64 6574 6563 7469 6f6e 0a20 2020  pe_detection.   
-00008ea0: 205f 6164 645f 6d65 7373 6167 655f 7468   _add_message_th
-00008eb0: 7265 6164 5f69 6428 7061 796c 6f61 642c  read_id(payload,
-00008ec0: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
-00008ed0: 6964 290a 2020 2020 7265 7475 726e 2061  id).    return a
-00008ee0: 7761 6974 205f 7265 7175 6573 7428 746f  wait _request(to
-00008ef0: 6b65 6e2c 206d 6574 686f 645f 7572 6c2c  ken, method_url,
-00008f00: 2070 6172 616d 733d 7061 796c 6f61 642c   params=payload,
-00008f10: 2066 696c 6573 3d66 696c 6573 2c20 6d65   files=files, me
-00008f20: 7468 6f64 3d22 706f 7374 2229 0a0a 0a61  thod="post")...a
-00008f30: 7379 6e63 2064 6566 2067 6574 5f6d 6574  sync def get_met
-00008f40: 686f 645f 6279 5f74 7970 6528 6461 7461  hod_by_type(data
-00008f50: 5f74 7970 6529 3a0a 2020 2020 6966 2064  _type):.    if d
-00008f60: 6174 615f 7479 7065 203d 3d20 2264 6f63  ata_type == "doc
-00008f70: 756d 656e 7422 3a0a 2020 2020 2020 2020  ument":.        
-00008f80: 7265 7475 726e 2072 2273 656e 6444 6f63  return r"sendDoc
-00008f90: 756d 656e 7422 0a20 2020 2069 6620 6461  ument".    if da
-00008fa0: 7461 5f74 7970 6520 3d3d 2022 7374 6963  ta_type == "stic
-00008fb0: 6b65 7222 3a0a 2020 2020 2020 2020 7265  ker":.        re
-00008fc0: 7475 726e 2072 2273 656e 6453 7469 636b  turn r"sendStick
-00008fd0: 6572 220a 0a0a 6173 796e 6320 6465 6620  er"...async def 
-00008fe0: 6261 6e5f 6368 6174 5f6d 656d 6265 7228  ban_chat_member(
-00008ff0: 746f 6b65 6e2c 2063 6861 745f 6964 2c20  token, chat_id, 
-00009000: 7573 6572 5f69 642c 2075 6e74 696c 5f64  user_id, until_d
-00009010: 6174 653d 4e6f 6e65 2c20 7265 766f 6b65  ate=None, revoke
-00009020: 5f6d 6573 7361 6765 733d 4e6f 6e65 293a  _messages=None):
-00009030: 0a20 2020 206d 6574 686f 645f 7572 6c20  .    method_url 
-00009040: 3d20 2262 616e 4368 6174 4d65 6d62 6572  = "banChatMember
-00009050: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
-00009060: 7b22 6368 6174 5f69 6422 3a20 6368 6174  {"chat_id": chat
-00009070: 5f69 642c 2022 7573 6572 5f69 6422 3a20  _id, "user_id": 
-00009080: 7573 6572 5f69 647d 0a20 2020 2069 6620  user_id}.    if 
-00009090: 6973 696e 7374 616e 6365 2875 6e74 696c  isinstance(until
-000090a0: 5f64 6174 652c 2064 6174 6574 696d 6529  _date, datetime)
-000090b0: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-000090c0: 645b 2275 6e74 696c 5f64 6174 6522 5d20  d["until_date"] 
-000090d0: 3d20 756e 7469 6c5f 6461 7465 2e74 696d  = until_date.tim
-000090e0: 6573 7461 6d70 2829 0a20 2020 2065 6c73  estamp().    els
-000090f0: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-00009100: 6164 5b22 756e 7469 6c5f 6461 7465 225d  ad["until_date"]
-00009110: 203d 2075 6e74 696c 5f64 6174 650a 2020   = until_date.  
-00009120: 2020 6966 2072 6576 6f6b 655f 6d65 7373    if revoke_mess
-00009130: 6167 6573 2069 7320 6e6f 7420 4e6f 6e65  ages is not None
-00009140: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-00009150: 645b 2272 6576 6f6b 655f 6d65 7373 6167  d["revoke_messag
-00009160: 6573 225d 203d 2072 6576 6f6b 655f 6d65  es"] = revoke_me
-00009170: 7373 6167 6573 0a20 2020 2072 6574 7572  ssages.    retur
-00009180: 6e20 6177 6169 7420 5f72 6571 7565 7374  n await _request
-00009190: 2874 6f6b 656e 2c20 6d65 7468 6f64 5f75  (token, method_u
-000091a0: 726c 2c20 7061 7261 6d73 3d70 6179 6c6f  rl, params=paylo
-000091b0: 6164 2c20 6d65 7468 6f64 3d22 706f 7374  ad, method="post
-000091c0: 2229 0a0a 0a61 7379 6e63 2064 6566 2075  ")...async def u
-000091d0: 6e62 616e 5f63 6861 745f 6d65 6d62 6572  nban_chat_member
-000091e0: 2874 6f6b 656e 2c20 6368 6174 5f69 642c  (token, chat_id,
-000091f0: 2075 7365 725f 6964 2c20 6f6e 6c79 5f69   user_id, only_i
-00009200: 665f 6261 6e6e 6564 293a 0a20 2020 206d  f_banned):.    m
-00009210: 6574 686f 645f 7572 6c20 3d20 2275 6e62  ethod_url = "unb
-00009220: 616e 4368 6174 4d65 6d62 6572 220a 2020  anChatMember".  
-00009230: 2020 7061 796c 6f61 6420 3d20 7b22 6368    payload = {"ch
-00009240: 6174 5f69 6422 3a20 6368 6174 5f69 642c  at_id": chat_id,
-00009250: 2022 7573 6572 5f69 6422 3a20 7573 6572   "user_id": user
-00009260: 5f69 647d 0a20 2020 2069 6620 6f6e 6c79  _id}.    if only
-00009270: 5f69 665f 6261 6e6e 6564 2069 7320 6e6f  _if_banned is no
-00009280: 7420 4e6f 6e65 3a20 2023 204e 6f6e 6520  t None:  # None 
-00009290: 2f20 5472 7565 202f 2046 616c 7365 0a20  / True / False. 
-000092a0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-000092b0: 6f6e 6c79 5f69 665f 6261 6e6e 6564 225d  only_if_banned"]
-000092c0: 203d 206f 6e6c 795f 6966 5f62 616e 6e65   = only_if_banne
-000092d0: 640a 2020 2020 7265 7475 726e 2061 7761  d.    return awa
-000092e0: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
-000092f0: 6e2c 206d 6574 686f 645f 7572 6c2c 2070  n, method_url, p
-00009300: 6172 616d 733d 7061 796c 6f61 642c 206d  arams=payload, m
-00009310: 6574 686f 643d 2270 6f73 7422 290a 0a0a  ethod="post")...
-00009320: 6173 796e 6320 6465 6620 7265 7374 7269  async def restri
-00009330: 6374 5f63 6861 745f 6d65 6d62 6572 280a  ct_chat_member(.
-00009340: 2020 2020 746f 6b65 6e2c 0a20 2020 2063      token,.    c
-00009350: 6861 745f 6964 2c0a 2020 2020 7573 6572  hat_id,.    user
-00009360: 5f69 642c 0a20 2020 2070 6572 6d69 7373  _id,.    permiss
-00009370: 696f 6e73 2c0a 2020 2020 756e 7469 6c5f  ions,.    until_
-00009380: 6461 7465 3d4e 6f6e 652c 0a20 2020 2075  date=None,.    u
-00009390: 7365 5f69 6e64 6570 656e 6465 6e74 5f63  se_independent_c
-000093a0: 6861 745f 7065 726d 6973 7369 6f6e 733d  hat_permissions=
-000093b0: 4e6f 6e65 2c0a 293a 0a20 2020 206d 6574  None,.):.    met
-000093c0: 686f 645f 7572 6c20 3d20 2272 6573 7472  hod_url = "restr
-000093d0: 6963 7443 6861 744d 656d 6265 7222 0a20  ictChatMember". 
-000093e0: 2020 2070 6179 6c6f 6164 203d 207b 2263     payload = {"c
-000093f0: 6861 745f 6964 223a 2063 6861 745f 6964  hat_id": chat_id
-00009400: 2c20 2275 7365 725f 6964 223a 2075 7365  , "user_id": use
-00009410: 725f 6964 2c20 2270 6572 6d69 7373 696f  r_id, "permissio
-00009420: 6e73 223a 2070 6572 6d69 7373 696f 6e73  ns": permissions
-00009430: 2e74 6f5f 6a73 6f6e 2829 7d0a 2020 2020  .to_json()}.    
-00009440: 6966 2075 7365 5f69 6e64 6570 656e 6465  if use_independe
-00009450: 6e74 5f63 6861 745f 7065 726d 6973 7369  nt_chat_permissi
-00009460: 6f6e 7320 6973 206e 6f74 204e 6f6e 653a  ons is not None:
-00009470: 0a20 2020 2020 2020 2070 6572 6d69 7373  .        permiss
-00009480: 696f 6e73 5b22 7573 655f 696e 6465 7065  ions["use_indepe
-00009490: 6e64 656e 745f 6368 6174 5f70 6572 6d69  ndent_chat_permi
-000094a0: 7373 696f 6e73 225d 203d 2075 7365 5f69  ssions"] = use_i
-000094b0: 6e64 6570 656e 6465 6e74 5f63 6861 745f  ndependent_chat_
-000094c0: 7065 726d 6973 7369 6f6e 730a 2020 2020  permissions.    
-000094d0: 6966 2075 6e74 696c 5f64 6174 6520 6973  if until_date is
-000094e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000094f0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00009500: 2875 6e74 696c 5f64 6174 652c 2064 6174  (until_date, dat
-00009510: 6574 696d 6529 3a0a 2020 2020 2020 2020  etime):.        
-00009520: 2020 2020 7061 796c 6f61 645b 2275 6e74      payload["unt
-00009530: 696c 5f64 6174 6522 5d20 3d20 756e 7469  il_date"] = unti
-00009540: 6c5f 6461 7465 2e74 696d 6573 7461 6d70  l_date.timestamp
-00009550: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
-00009560: 0a20 2020 2020 2020 2020 2020 2070 6179  .            pay
-00009570: 6c6f 6164 5b22 756e 7469 6c5f 6461 7465  load["until_date
-00009580: 225d 203d 2075 6e74 696c 5f64 6174 650a  "] = until_date.
-00009590: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-000095a0: 205f 7265 7175 6573 7428 746f 6b65 6e2c   _request(token,
-000095b0: 206d 6574 686f 645f 7572 6c2c 2070 6172   method_url, par
-000095c0: 616d 733d 7061 796c 6f61 642c 206d 6574  ams=payload, met
-000095d0: 686f 643d 2270 6f73 7422 290a 0a0a 6173  hod="post")...as
-000095e0: 796e 6320 6465 6620 7072 6f6d 6f74 655f  ync def promote_
-000095f0: 6368 6174 5f6d 656d 6265 7228 0a20 2020  chat_member(.   
-00009600: 2074 6f6b 656e 2c0a 2020 2020 6368 6174   token,.    chat
-00009610: 5f69 642c 0a20 2020 2075 7365 725f 6964  _id,.    user_id
-00009620: 2c0a 2020 2020 6361 6e5f 6368 616e 6765  ,.    can_change
-00009630: 5f69 6e66 6f3d 4e6f 6e65 2c0a 2020 2020  _info=None,.    
-00009640: 6361 6e5f 706f 7374 5f6d 6573 7361 6765  can_post_message
-00009650: 733d 4e6f 6e65 2c0a 2020 2020 6361 6e5f  s=None,.    can_
-00009660: 6564 6974 5f6d 6573 7361 6765 733d 4e6f  edit_messages=No
-00009670: 6e65 2c0a 2020 2020 6361 6e5f 6465 6c65  ne,.    can_dele
-00009680: 7465 5f6d 6573 7361 6765 733d 4e6f 6e65  te_messages=None
-00009690: 2c0a 2020 2020 6361 6e5f 696e 7669 7465  ,.    can_invite
-000096a0: 5f75 7365 7273 3d4e 6f6e 652c 0a20 2020  _users=None,.   
-000096b0: 2063 616e 5f72 6573 7472 6963 745f 6d65   can_restrict_me
-000096c0: 6d62 6572 733d 4e6f 6e65 2c0a 2020 2020  mbers=None,.    
-000096d0: 6361 6e5f 7069 6e5f 6d65 7373 6167 6573  can_pin_messages
-000096e0: 3d4e 6f6e 652c 0a20 2020 2063 616e 5f70  =None,.    can_p
-000096f0: 726f 6d6f 7465 5f6d 656d 6265 7273 3d4e  romote_members=N
-00009700: 6f6e 652c 0a20 2020 2069 735f 616e 6f6e  one,.    is_anon
-00009710: 796d 6f75 733d 4e6f 6e65 2c0a 2020 2020  ymous=None,.    
-00009720: 6361 6e5f 6d61 6e61 6765 5f63 6861 743d  can_manage_chat=
-00009730: 4e6f 6e65 2c0a 2020 2020 6361 6e5f 6d61  None,.    can_ma
-00009740: 6e61 6765 5f76 6964 656f 5f63 6861 7473  nage_video_chats
-00009750: 3d4e 6f6e 652c 0a20 2020 2063 616e 5f6d  =None,.    can_m
-00009760: 616e 6167 655f 746f 7069 6373 3d4e 6f6e  anage_topics=Non
-00009770: 652c 0a29 3a0a 2020 2020 6d65 7468 6f64  e,.):.    method
-00009780: 5f75 726c 203d 2022 7072 6f6d 6f74 6543  _url = "promoteC
-00009790: 6861 744d 656d 6265 7222 0a20 2020 2070  hatMember".    p
-000097a0: 6179 6c6f 6164 203d 207b 2263 6861 745f  ayload = {"chat_
-000097b0: 6964 223a 2063 6861 745f 6964 2c20 2275  id": chat_id, "u
-000097c0: 7365 725f 6964 223a 2075 7365 725f 6964  ser_id": user_id
-000097d0: 7d0a 2020 2020 6966 2063 616e 5f63 6861  }.    if can_cha
-000097e0: 6e67 655f 696e 666f 2069 7320 6e6f 7420  nge_info is not 
-000097f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
-00009800: 796c 6f61 645b 2263 616e 5f63 6861 6e67  yload["can_chang
-00009810: 655f 696e 666f 225d 203d 2063 616e 5f63  e_info"] = can_c
-00009820: 6861 6e67 655f 696e 666f 0a20 2020 2069  hange_info.    i
-00009830: 6620 6361 6e5f 706f 7374 5f6d 6573 7361  f can_post_messa
-00009840: 6765 7320 6973 206e 6f74 204e 6f6e 653a  ges is not None:
-00009850: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00009860: 5b22 6361 6e5f 706f 7374 5f6d 6573 7361  ["can_post_messa
-00009870: 6765 7322 5d20 3d20 6361 6e5f 706f 7374  ges"] = can_post
-00009880: 5f6d 6573 7361 6765 730a 2020 2020 6966  _messages.    if
-00009890: 2063 616e 5f65 6469 745f 6d65 7373 6167   can_edit_messag
-000098a0: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
-000098b0: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-000098c0: 2263 616e 5f65 6469 745f 6d65 7373 6167  "can_edit_messag
-000098d0: 6573 225d 203d 2063 616e 5f65 6469 745f  es"] = can_edit_
-000098e0: 6d65 7373 6167 6573 0a20 2020 2069 6620  messages.    if 
-000098f0: 6361 6e5f 6465 6c65 7465 5f6d 6573 7361  can_delete_messa
-00009900: 6765 7320 6973 206e 6f74 204e 6f6e 653a  ges is not None:
-00009910: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00009920: 5b22 6361 6e5f 6465 6c65 7465 5f6d 6573  ["can_delete_mes
-00009930: 7361 6765 7322 5d20 3d20 6361 6e5f 6465  sages"] = can_de
-00009940: 6c65 7465 5f6d 6573 7361 6765 730a 2020  lete_messages.  
-00009950: 2020 6966 2063 616e 5f69 6e76 6974 655f    if can_invite_
-00009960: 7573 6572 7320 6973 206e 6f74 204e 6f6e  users is not Non
-00009970: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-00009980: 6164 5b22 6361 6e5f 696e 7669 7465 5f75  ad["can_invite_u
-00009990: 7365 7273 225d 203d 2063 616e 5f69 6e76  sers"] = can_inv
-000099a0: 6974 655f 7573 6572 730a 2020 2020 6966  ite_users.    if
-000099b0: 2063 616e 5f72 6573 7472 6963 745f 6d65   can_restrict_me
-000099c0: 6d62 6572 7320 6973 206e 6f74 204e 6f6e  mbers is not Non
-000099d0: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-000099e0: 6164 5b22 6361 6e5f 7265 7374 7269 6374  ad["can_restrict
-000099f0: 5f6d 656d 6265 7273 225d 203d 2063 616e  _members"] = can
-00009a00: 5f72 6573 7472 6963 745f 6d65 6d62 6572  _restrict_member
-00009a10: 730a 2020 2020 6966 2063 616e 5f70 696e  s.    if can_pin
-00009a20: 5f6d 6573 7361 6765 7320 6973 206e 6f74  _messages is not
-00009a30: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
-00009a40: 6179 6c6f 6164 5b22 6361 6e5f 7069 6e5f  ayload["can_pin_
-00009a50: 6d65 7373 6167 6573 225d 203d 2063 616e  messages"] = can
-00009a60: 5f70 696e 5f6d 6573 7361 6765 730a 2020  _pin_messages.  
-00009a70: 2020 6966 2063 616e 5f70 726f 6d6f 7465    if can_promote
-00009a80: 5f6d 656d 6265 7273 2069 7320 6e6f 7420  _members is not 
-00009a90: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
-00009aa0: 796c 6f61 645b 2263 616e 5f70 726f 6d6f  yload["can_promo
-00009ab0: 7465 5f6d 656d 6265 7273 225d 203d 2063  te_members"] = c
-00009ac0: 616e 5f70 726f 6d6f 7465 5f6d 656d 6265  an_promote_membe
-00009ad0: 7273 0a20 2020 2069 6620 6973 5f61 6e6f  rs.    if is_ano
-00009ae0: 6e79 6d6f 7573 2069 7320 6e6f 7420 4e6f  nymous is not No
-00009af0: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
-00009b00: 6f61 645b 2269 735f 616e 6f6e 796d 6f75  oad["is_anonymou
-00009b10: 7322 5d20 3d20 6973 5f61 6e6f 6e79 6d6f  s"] = is_anonymo
-00009b20: 7573 0a20 2020 2069 6620 6361 6e5f 6d61  us.    if can_ma
-00009b30: 6e61 6765 5f63 6861 7420 6973 206e 6f74  nage_chat is not
-00009b40: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
-00009b50: 6179 6c6f 6164 5b22 6361 6e5f 6d61 6e61  ayload["can_mana
-00009b60: 6765 5f63 6861 7422 5d20 3d20 6361 6e5f  ge_chat"] = can_
-00009b70: 6d61 6e61 6765 5f63 6861 740a 2020 2020  manage_chat.    
-00009b80: 6966 2063 616e 5f6d 616e 6167 655f 7669  if can_manage_vi
-00009b90: 6465 6f5f 6368 6174 7320 6973 206e 6f74  deo_chats is not
-00009ba0: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
-00009bb0: 6179 6c6f 6164 5b22 6361 6e5f 6d61 6e61  ayload["can_mana
-00009bc0: 6765 5f76 6964 656f 5f63 6861 7473 225d  ge_video_chats"]
-00009bd0: 203d 2063 616e 5f6d 616e 6167 655f 7669   = can_manage_vi
-00009be0: 6465 6f5f 6368 6174 730a 2020 2020 6966  deo_chats.    if
-00009bf0: 2063 616e 5f6d 616e 6167 655f 746f 7069   can_manage_topi
-00009c00: 6373 2069 7320 6e6f 7420 4e6f 6e65 3a0a  cs is not None:.
-00009c10: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-00009c20: 2263 616e 5f6d 616e 6167 655f 746f 7069  "can_manage_topi
-00009c30: 6373 225d 203d 2063 616e 5f6d 616e 6167  cs"] = can_manag
-00009c40: 655f 746f 7069 6373 0a20 2020 2072 6574  e_topics.    ret
-00009c50: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
-00009c60: 7374 2874 6f6b 656e 2c20 6d65 7468 6f64  st(token, method
-00009c70: 5f75 726c 2c20 7061 7261 6d73 3d70 6179  _url, params=pay
-00009c80: 6c6f 6164 2c20 6d65 7468 6f64 3d22 706f  load, method="po
-00009c90: 7374 2229 0a0a 0a61 7379 6e63 2064 6566  st")...async def
-00009ca0: 2073 6574 5f63 6861 745f 6164 6d69 6e69   set_chat_admini
-00009cb0: 7374 7261 746f 725f 6375 7374 6f6d 5f74  strator_custom_t
-00009cc0: 6974 6c65 2874 6f6b 656e 2c20 6368 6174  itle(token, chat
-00009cd0: 5f69 642c 2075 7365 725f 6964 2c20 6375  _id, user_id, cu
-00009ce0: 7374 6f6d 5f74 6974 6c65 293a 0a20 2020  stom_title):.   
-00009cf0: 206d 6574 686f 645f 7572 6c20 3d20 2273   method_url = "s
-00009d00: 6574 4368 6174 4164 6d69 6e69 7374 7261  etChatAdministra
-00009d10: 746f 7243 7573 746f 6d54 6974 6c65 220a  torCustomTitle".
-00009d20: 2020 2020 7061 796c 6f61 6420 3d20 7b22      payload = {"
-00009d30: 6368 6174 5f69 6422 3a20 6368 6174 5f69  chat_id": chat_i
-00009d40: 642c 2022 7573 6572 5f69 6422 3a20 7573  d, "user_id": us
-00009d50: 6572 5f69 642c 2022 6375 7374 6f6d 5f74  er_id, "custom_t
-00009d60: 6974 6c65 223a 2063 7573 746f 6d5f 7469  itle": custom_ti
-00009d70: 746c 657d 0a20 2020 2072 6574 7572 6e20  tle}.    return 
-00009d80: 6177 6169 7420 5f72 6571 7565 7374 2874  await _request(t
-00009d90: 6f6b 656e 2c20 6d65 7468 6f64 5f75 726c  oken, method_url
-00009da0: 2c20 7061 7261 6d73 3d70 6179 6c6f 6164  , params=payload
-00009db0: 2c20 6d65 7468 6f64 3d22 706f 7374 2229  , method="post")
-00009dc0: 0a0a 0a61 7379 6e63 2064 6566 2062 616e  ...async def ban
-00009dd0: 5f63 6861 745f 7365 6e64 6572 5f63 6861  _chat_sender_cha
-00009de0: 7428 746f 6b65 6e2c 2063 6861 745f 6964  t(token, chat_id
-00009df0: 2c20 7365 6e64 6572 5f63 6861 745f 6964  , sender_chat_id
-00009e00: 293a 0a20 2020 206d 6574 686f 645f 7572  ):.    method_ur
-00009e10: 6c20 3d20 2262 616e 4368 6174 5365 6e64  l = "banChatSend
-00009e20: 6572 4368 6174 220a 2020 2020 7061 796c  erChat".    payl
-00009e30: 6f61 6420 3d20 7b22 6368 6174 5f69 6422  oad = {"chat_id"
-00009e40: 3a20 6368 6174 5f69 642c 2022 7365 6e64  : chat_id, "send
-00009e50: 6572 5f63 6861 745f 6964 223a 2073 656e  er_chat_id": sen
-00009e60: 6465 725f 6368 6174 5f69 647d 0a20 2020  der_chat_id}.   
-00009e70: 2072 6574 7572 6e20 6177 6169 7420 5f72   return await _r
-00009e80: 6571 7565 7374 2874 6f6b 656e 2c20 6d65  equest(token, me
-00009e90: 7468 6f64 5f75 726c 2c20 7061 7261 6d73  thod_url, params
-00009ea0: 3d70 6179 6c6f 6164 2c20 6d65 7468 6f64  =payload, method
-00009eb0: 3d22 706f 7374 2229 0a0a 0a61 7379 6e63  ="post")...async
-00009ec0: 2064 6566 2075 6e62 616e 5f63 6861 745f   def unban_chat_
-00009ed0: 7365 6e64 6572 5f63 6861 7428 746f 6b65  sender_chat(toke
-00009ee0: 6e2c 2063 6861 745f 6964 2c20 7365 6e64  n, chat_id, send
-00009ef0: 6572 5f63 6861 745f 6964 293a 0a20 2020  er_chat_id):.   
-00009f00: 206d 6574 686f 645f 7572 6c20 3d20 2275   method_url = "u
-00009f10: 6e62 616e 4368 6174 5365 6e64 6572 4368  nbanChatSenderCh
-00009f20: 6174 220a 2020 2020 7061 796c 6f61 6420  at".    payload 
-00009f30: 3d20 7b22 6368 6174 5f69 6422 3a20 6368  = {"chat_id": ch
-00009f40: 6174 5f69 642c 2022 7365 6e64 6572 5f63  at_id, "sender_c
-00009f50: 6861 745f 6964 223a 2073 656e 6465 725f  hat_id": sender_
-00009f60: 6368 6174 5f69 647d 0a20 2020 2072 6574  chat_id}.    ret
-00009f70: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
-00009f80: 7374 2874 6f6b 656e 2c20 6d65 7468 6f64  st(token, method
-00009f90: 5f75 726c 2c20 7061 7261 6d73 3d70 6179  _url, params=pay
-00009fa0: 6c6f 6164 2c20 6d65 7468 6f64 3d22 706f  load, method="po
-00009fb0: 7374 2229 0a0a 0a61 7379 6e63 2064 6566  st")...async def
-00009fc0: 2073 6574 5f63 6861 745f 7065 726d 6973   set_chat_permis
-00009fd0: 7369 6f6e 7328 746f 6b65 6e2c 2063 6861  sions(token, cha
-00009fe0: 745f 6964 2c20 7065 726d 6973 7369 6f6e  t_id, permission
-00009ff0: 732c 2075 7365 5f69 6e64 6570 656e 6465  s, use_independe
-0000a000: 6e74 5f63 6861 745f 7065 726d 6973 7369  nt_chat_permissi
-0000a010: 6f6e 733a 204f 7074 696f 6e61 6c5b 626f  ons: Optional[bo
-0000a020: 6f6c 5d20 3d20 4e6f 6e65 293a 0a20 2020  ol] = None):.   
-0000a030: 2072 6f75 7465 203d 2022 7365 7443 6861   route = "setCha
-0000a040: 7450 6572 6d69 7373 696f 6e73 220a 2020  tPermissions".  
-0000a050: 2020 7061 796c 6f61 6420 3d20 7b22 6368    payload = {"ch
-0000a060: 6174 5f69 6422 3a20 6368 6174 5f69 642c  at_id": chat_id,
-0000a070: 2022 7065 726d 6973 7369 6f6e 7322 3a20   "permissions": 
-0000a080: 7065 726d 6973 7369 6f6e 732e 746f 5f6a  permissions.to_j
-0000a090: 736f 6e28 297d 0a20 2020 2069 6620 7573  son()}.    if us
-0000a0a0: 655f 696e 6465 7065 6e64 656e 745f 6368  e_independent_ch
-0000a0b0: 6174 5f70 6572 6d69 7373 696f 6e73 2069  at_permissions i
-0000a0c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000a0d0: 2020 2020 7061 796c 6f61 645b 2275 7365      payload["use
-0000a0e0: 5f69 6e64 6570 656e 6465 6e74 5f63 6861  _independent_cha
-0000a0f0: 745f 7065 726d 6973 7369 6f6e 7322 5d20  t_permissions"] 
-0000a100: 3d20 7573 655f 696e 6465 7065 6e64 656e  = use_independen
-0000a110: 745f 6368 6174 5f70 6572 6d69 7373 696f  t_chat_permissio
-0000a120: 6e73 0a20 2020 2072 6574 7572 6e20 6177  ns.    return aw
-0000a130: 6169 7420 5f72 6571 7565 7374 2874 6f6b  ait _request(tok
-0000a140: 656e 2c20 726f 7574 652c 2070 6172 616d  en, route, param
-0000a150: 733d 7061 796c 6f61 642c 206d 6574 686f  s=payload, metho
-0000a160: 643d 2270 6f73 7422 290a 0a0a 6173 796e  d="post")...asyn
-0000a170: 6320 6465 6620 6372 6561 7465 5f63 6861  c def create_cha
-0000a180: 745f 696e 7669 7465 5f6c 696e 6b28 746f  t_invite_link(to
-0000a190: 6b65 6e2c 2063 6861 745f 6964 2c20 6e61  ken, chat_id, na
-0000a1a0: 6d65 2c20 6578 7069 7265 5f64 6174 652c  me, expire_date,
-0000a1b0: 206d 656d 6265 725f 6c69 6d69 742c 2063   member_limit, c
-0000a1c0: 7265 6174 6573 5f6a 6f69 6e5f 7265 7175  reates_join_requ
-0000a1d0: 6573 7429 3a0a 2020 2020 6d65 7468 6f64  est):.    method
-0000a1e0: 5f75 726c 203d 2022 6372 6561 7465 4368  _url = "createCh
-0000a1f0: 6174 496e 7669 7465 4c69 6e6b 220a 2020  atInviteLink".  
-0000a200: 2020 7061 796c 6f61 6420 3d20 7b22 6368    payload = {"ch
-0000a210: 6174 5f69 6422 3a20 6368 6174 5f69 647d  at_id": chat_id}
-0000a220: 0a0a 2020 2020 6966 2065 7870 6972 655f  ..    if expire_
-0000a230: 6461 7465 2069 7320 6e6f 7420 4e6f 6e65  date is not None
-0000a240: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
-0000a250: 6e73 7461 6e63 6528 6578 7069 7265 5f64  nstance(expire_d
-0000a260: 6174 652c 2064 6174 6574 696d 6529 3a0a  ate, datetime):.
-0000a270: 2020 2020 2020 2020 2020 2020 7061 796c              payl
-0000a280: 6f61 645b 2265 7870 6972 655f 6461 7465  oad["expire_date
-0000a290: 225d 203d 2065 7870 6972 655f 6461 7465  "] = expire_date
-0000a2a0: 2e74 696d 6573 7461 6d70 2829 0a20 2020  .timestamp().   
-0000a2b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a2c0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-0000a2d0: 6578 7069 7265 5f64 6174 6522 5d20 3d20  expire_date"] = 
-0000a2e0: 6578 7069 7265 5f64 6174 650a 2020 2020  expire_date.    
-0000a2f0: 6966 206d 656d 6265 725f 6c69 6d69 743a  if member_limit:
-0000a300: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000a310: 5b22 6d65 6d62 6572 5f6c 696d 6974 225d  ["member_limit"]
-0000a320: 203d 206d 656d 6265 725f 6c69 6d69 740a   = member_limit.
-0000a330: 2020 2020 6966 2063 7265 6174 6573 5f6a      if creates_j
-0000a340: 6f69 6e5f 7265 7175 6573 7420 6973 206e  oin_request is n
-0000a350: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000a360: 2070 6179 6c6f 6164 5b22 6372 6561 7465   payload["create
-0000a370: 735f 6a6f 696e 5f72 6571 7565 7374 225d  s_join_request"]
-0000a380: 203d 2063 7265 6174 6573 5f6a 6f69 6e5f   = creates_join_
-0000a390: 7265 7175 6573 740a 2020 2020 6966 206e  request.    if n
-0000a3a0: 616d 653a 0a20 2020 2020 2020 2070 6179  ame:.        pay
-0000a3b0: 6c6f 6164 5b22 6e61 6d65 225d 203d 206e  load["name"] = n
-0000a3c0: 616d 650a 0a20 2020 2072 6574 7572 6e20  ame..    return 
-0000a3d0: 6177 6169 7420 5f72 6571 7565 7374 2874  await _request(t
-0000a3e0: 6f6b 656e 2c20 6d65 7468 6f64 5f75 726c  oken, method_url
-0000a3f0: 2c20 7061 7261 6d73 3d70 6179 6c6f 6164  , params=payload
-0000a400: 2c20 6d65 7468 6f64 3d22 706f 7374 2229  , method="post")
-0000a410: 0a0a 0a61 7379 6e63 2064 6566 2065 6469  ...async def edi
-0000a420: 745f 6368 6174 5f69 6e76 6974 655f 6c69  t_chat_invite_li
-0000a430: 6e6b 2874 6f6b 656e 2c20 6368 6174 5f69  nk(token, chat_i
-0000a440: 642c 2069 6e76 6974 655f 6c69 6e6b 2c20  d, invite_link, 
-0000a450: 6e61 6d65 2c20 6578 7069 7265 5f64 6174  name, expire_dat
-0000a460: 652c 206d 656d 6265 725f 6c69 6d69 742c  e, member_limit,
-0000a470: 2063 7265 6174 6573 5f6a 6f69 6e5f 7265   creates_join_re
-0000a480: 7175 6573 7429 3a0a 2020 2020 6d65 7468  quest):.    meth
-0000a490: 6f64 5f75 726c 203d 2022 6564 6974 4368  od_url = "editCh
-0000a4a0: 6174 496e 7669 7465 4c69 6e6b 220a 2020  atInviteLink".  
-0000a4b0: 2020 7061 796c 6f61 6420 3d20 7b22 6368    payload = {"ch
-0000a4c0: 6174 5f69 6422 3a20 6368 6174 5f69 642c  at_id": chat_id,
-0000a4d0: 2022 696e 7669 7465 5f6c 696e 6b22 3a20   "invite_link": 
-0000a4e0: 696e 7669 7465 5f6c 696e 6b7d 0a0a 2020  invite_link}..  
-0000a4f0: 2020 6966 2065 7870 6972 655f 6461 7465    if expire_date
-0000a500: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000a510: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-0000a520: 6e63 6528 6578 7069 7265 5f64 6174 652c  nce(expire_date,
-0000a530: 2064 6174 6574 696d 6529 3a0a 2020 2020   datetime):.    
+00000020: 7265 0a66 726f 6d20 6461 7461 636c 6173  re.from dataclas
+00000030: 7365 7320 696d 706f 7274 2064 6174 6163  ses import datac
+00000040: 6c61 7373 0a66 726f 6d20 6461 7465 7469  lass.from dateti
+00000050: 6d65 2069 6d70 6f72 7420 6461 7465 7469  me import dateti
+00000060: 6d65 0a66 726f 6d20 696f 2069 6d70 6f72  me.from io impor
+00000070: 7420 4279 7465 7349 4f0a 6672 6f6d 2074  t BytesIO.from t
+00000080: 7970 696e 6720 696d 706f 7274 2041 6e79  yping import Any
+00000090: 2c20 4469 6374 2c20 4f70 7469 6f6e 616c  , Dict, Optional
+000000a0: 2c20 556e 696f 6e2c 2063 6173 740a 0a69  , Union, cast..i
+000000b0: 6d70 6f72 7420 6169 6f68 7474 700a 696d  mport aiohttp.im
+000000c0: 706f 7274 2075 6a73 6f6e 2061 7320 6a73  port ujson as js
+000000d0: 6f6e 2020 2320 7479 7065 3a20 6967 6e6f  on  # type: igno
+000000e0: 7265 0a0a 6672 6f6d 2074 656c 6562 6f74  re..from telebot
+000000f0: 2069 6d70 6f72 7420 7479 7065 732c 2075   import types, u
+00000100: 7469 6c0a 0a6c 6f67 6765 7220 3d20 6c6f  til..logger = lo
+00000110: 6767 696e 672e 6765 744c 6f67 6765 7228  gging.getLogger(
+00000120: 5f5f 6e61 6d65 5f5f 290a 0a0a 4649 4c45  __name__)...FILE
+00000130: 5f55 524c 3a20 4f70 7469 6f6e 616c 5b73  _URL: Optional[s
+00000140: 7472 5d20 3d20 4e6f 6e65 0a43 5553 544f  tr] = None.CUSTO
+00000150: 4d5f 5345 5249 414c 495a 4552 203d 204e  M_SERIALIZER = N
+00000160: 6f6e 650a 0a44 4546 4155 4c54 5f52 4551  one..DEFAULT_REQ
+00000170: 5545 5354 5f54 494d 454f 5554 203d 204e  UEST_TIMEOUT = N
+00000180: 6f6e 650a 4d41 585f 5245 5452 4945 5320  one.MAX_RETRIES 
+00000190: 3d20 350a 5245 5155 4553 545f 4c49 4d49  = 5.REQUEST_LIMI
+000001a0: 5420 3d20 3530 0a0a 0a63 6c61 7373 2053  T = 50...class S
+000001b0: 6573 7369 6f6e 4d61 6e61 6765 723a 0a20  essionManager:. 
+000001c0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000001d0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+000001e0: 2020 2020 2020 2073 656c 662e 7365 7373         self.sess
+000001f0: 696f 6e3a 204f 7074 696f 6e61 6c5b 6169  ion: Optional[ai
+00000200: 6f68 7474 702e 436c 6965 6e74 5365 7373  ohttp.ClientSess
+00000210: 696f 6e5d 203d 204e 6f6e 650a 0a20 2020  ion] = None..   
+00000220: 2064 6566 2073 6574 5f73 6573 7369 6f6e   def set_session
+00000230: 2873 656c 662c 2073 6573 7369 6f6e 3a20  (self, session: 
+00000240: 6169 6f68 7474 702e 436c 6965 6e74 5365  aiohttp.ClientSe
+00000250: 7373 696f 6e29 3a0a 2020 2020 2020 2020  ssion):.        
+00000260: 7365 6c66 2e73 6573 7369 6f6e 203d 2073  self.session = s
+00000270: 6573 7369 6f6e 0a0a 2020 2020 6173 796e  ession..    asyn
+00000280: 6320 6465 6620 636c 6f73 655f 7365 7373  c def close_sess
+00000290: 696f 6e28 7365 6c66 293a 0a20 2020 2020  ion(self):.     
+000002a0: 2020 2069 6620 7365 6c66 2e73 6573 7369     if self.sessi
+000002b0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
+000002c0: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+000002d0: 7420 7365 6c66 2e73 6573 7369 6f6e 2e63  t self.session.c
+000002e0: 6c6f 7365 2829 0a0a 2020 2020 6173 796e  lose()..    asyn
+000002f0: 6320 6465 6620 696e 6974 5f73 6573 7369  c def init_sessi
+00000300: 6f6e 2873 656c 6629 3a0a 2020 2020 2020  on(self):.      
+00000310: 2020 7365 6c66 2e73 6573 7369 6f6e 203d    self.session =
+00000320: 2061 696f 6874 7470 2e43 6c69 656e 7453   aiohttp.ClientS
+00000330: 6573 7369 6f6e 2863 6f6e 6e65 6374 6f72  ession(connector
+00000340: 3d61 696f 6874 7470 2e54 4350 436f 6e6e  =aiohttp.TCPConn
+00000350: 6563 746f 7228 6c69 6d69 743d 5245 5155  ector(limit=REQU
+00000360: 4553 545f 4c49 4d49 5429 290a 0a20 2020  EST_LIMIT))..   
+00000370: 2061 7379 6e63 2064 6566 2067 6574 5f73   async def get_s
+00000380: 6573 7369 6f6e 2873 656c 6629 202d 3e20  ession(self) -> 
+00000390: 6169 6f68 7474 702e 436c 6965 6e74 5365  aiohttp.ClientSe
+000003a0: 7373 696f 6e3a 0a20 2020 2020 2020 2069  ssion:.        i
+000003b0: 6620 7365 6c66 2e73 6573 7369 6f6e 2069  f self.session i
+000003c0: 7320 4e6f 6e65 206f 7220 7365 6c66 2e73  s None or self.s
+000003d0: 6573 7369 6f6e 2e63 6c6f 7365 6420 6f72  ession.closed or
+000003e0: 206e 6f74 2073 656c 662e 7365 7373 696f   not self.sessio
+000003f0: 6e2e 5f6c 6f6f 702e 6973 5f72 756e 6e69  n._loop.is_runni
+00000400: 6e67 2829 3a0a 2020 2020 2020 2020 2020  ng():.          
+00000410: 2020 6177 6169 7420 7365 6c66 2e69 6e69    await self.ini
+00000420: 745f 7365 7373 696f 6e28 290a 2020 2020  t_session().    
+00000430: 2020 2020 7265 7475 726e 2063 6173 7428      return cast(
+00000440: 6169 6f68 7474 702e 436c 6965 6e74 5365  aiohttp.ClientSe
+00000450: 7373 696f 6e2c 2073 656c 662e 7365 7373  ssion, self.sess
+00000460: 696f 6e29 0a0a 0a73 6573 7369 6f6e 5f6d  ion)...session_m
+00000470: 616e 6167 6572 203d 2053 6573 7369 6f6e  anager = Session
+00000480: 4d61 6e61 6765 7228 290a 0a0a 4669 6c65  Manager()...File
+00000490: 4f62 6a65 6374 203d 2055 6e69 6f6e 5b42  Object = Union[B
+000004a0: 7974 6573 494f 2c20 6279 7465 732c 2062  ytesIO, bytes, b
+000004b0: 7974 6561 7272 6179 2c20 6d65 6d6f 7279  ytearray, memory
+000004c0: 7669 6577 5d0a 5061 7261 6d73 203d 2064  view].Params = d
+000004d0: 6963 745b 7374 722c 2041 6e79 5d0a 4669  ict[str, Any].Fi
+000004e0: 6c65 7320 3d20 6469 6374 5b73 7472 2c20  les = dict[str, 
+000004f0: 556e 696f 6e5b 7475 706c 655b 7374 722c  Union[tuple[str,
+00000500: 2046 696c 654f 626a 6563 745d 2c20 4669   FileObject], Fi
+00000510: 6c65 4f62 6a65 6374 5d5d 0a0a 0a61 7379  leObject]]...asy
+00000520: 6e63 2064 6566 205f 7265 7175 6573 7428  nc def _request(
+00000530: 0a20 2020 2074 6f6b 656e 3a20 7374 722c  .    token: str,
+00000540: 0a20 2020 2072 6f75 7465 3a20 7374 722c  .    route: str,
+00000550: 0a20 2020 206d 6574 686f 643a 2073 7472  .    method: str
+00000560: 203d 2022 6765 7422 2c0a 2020 2020 7061   = "get",.    pa
+00000570: 7261 6d73 3a20 4f70 7469 6f6e 616c 5b50  rams: Optional[P
+00000580: 6172 616d 735d 203d 204e 6f6e 652c 0a20  arams] = None,. 
+00000590: 2020 2066 696c 6573 3a20 4f70 7469 6f6e     files: Option
+000005a0: 616c 5b46 696c 6573 5d20 3d20 4e6f 6e65  al[Files] = None
+000005b0: 2c0a 2020 2020 7265 7175 6573 745f 7469  ,.    request_ti
+000005c0: 6d65 6f75 743a 204f 7074 696f 6e61 6c5b  meout: Optional[
+000005d0: 666c 6f61 745d 203d 204e 6f6e 652c 0a29  float] = None,.)
+000005e0: 3a0a 2020 2020 7365 7373 696f 6e20 3d20  :.    session = 
+000005f0: 6177 6169 7420 7365 7373 696f 6e5f 6d61  await session_ma
+00000600: 6e61 6765 722e 6765 745f 7365 7373 696f  nager.get_sessio
+00000610: 6e28 290a 2020 2020 7265 7175 6573 745f  n().    request_
+00000620: 6465 7363 7269 7074 696f 6e20 3d20 6622  description = f"
+00000630: 7b6d 6574 686f 6420 3d20 7d20 7b72 6f75  {method = } {rou
+00000640: 7465 203d 207d 207b 7061 7261 6d73 203d  te = } {params =
+00000650: 207d 207b 6669 6c65 7320 3d20 7d20 7b72   } {files = } {r
+00000660: 6571 7565 7374 5f74 696d 656f 7574 203d  equest_timeout =
+00000670: 207d 220a 2020 2020 7265 7175 6573 745f   }".    request_
+00000680: 6465 7363 7269 7074 696f 6e20 3d20 7265  description = re
+00000690: 7175 6573 745f 6465 7363 7269 7074 696f  quest_descriptio
+000006a0: 6e2e 7265 706c 6163 6528 746f 6b65 6e2c  n.replace(token,
+000006b0: 2022 3c62 6f74 2d74 6f6b 656e 3e22 290a   "<bot-token>").
+000006c0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+000006d0: 2822 4d61 6b69 6e67 2072 6571 7565 7374  ("Making request
+000006e0: 3a20 2573 222c 2072 6571 7565 7374 5f64  : %s", request_d
+000006f0: 6573 6372 6970 7469 6f6e 290a 2020 2020  escription).    
+00000700: 6c61 7374 5f65 7863 6570 7469 6f6e 3a20  last_exception: 
+00000710: 4f70 7469 6f6e 616c 5b45 7863 6570 7469  Optional[Excepti
+00000720: 6f6e 5d20 3d20 4e6f 6e65 0a20 2020 2066  on] = None.    f
+00000730: 6f72 2061 7474 656d 7074 2069 6e20 7261  or attempt in ra
+00000740: 6e67 6528 4d41 585f 5245 5452 4945 5329  nge(MAX_RETRIES)
+00000750: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
+00000760: 2020 2020 2020 2020 2020 2061 7379 6e63             async
+00000770: 2077 6974 6820 7365 7373 696f 6e2e 7265   with session.re
+00000780: 7175 6573 7428 0a20 2020 2020 2020 2020  quest(.         
+00000790: 2020 2020 2020 206d 6574 686f 643d 6d65         method=me
+000007a0: 7468 6f64 2c0a 2020 2020 2020 2020 2020  thod,.          
+000007b0: 2020 2020 2020 7572 6c3d 2268 7474 7073        url="https
+000007c0: 3a2f 2f61 7069 2e74 656c 6567 7261 6d2e  ://api.telegram.
+000007d0: 6f72 672f 626f 747b 307d 2f7b 317d 222e  org/bot{0}/{1}".
+000007e0: 666f 726d 6174 2874 6f6b 656e 2c20 726f  format(token, ro
+000007f0: 7574 6529 2c0a 2020 2020 2020 2020 2020  ute),.          
+00000800: 2020 2020 2020 6461 7461 3d74 6f5f 666f        data=to_fo
+00000810: 726d 5f64 6174 6128 7061 7261 6d73 2c20  rm_data(params, 
+00000820: 6669 6c65 7329 2c0a 2020 2020 2020 2020  files),.        
+00000830: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+00000840: 6169 6f68 7474 702e 436c 6965 6e74 5469  aiohttp.ClientTi
+00000850: 6d65 6f75 7428 746f 7461 6c3d 7265 7175  meout(total=requ
+00000860: 6573 745f 7469 6d65 6f75 7420 6f72 2044  est_timeout or D
+00000870: 4546 4155 4c54 5f52 4551 5545 5354 5f54  EFAULT_REQUEST_T
+00000880: 494d 454f 5554 292c 0a20 2020 2020 2020  IMEOUT),.       
+00000890: 2020 2020 2029 2061 7320 7265 7370 3a0a       ) as resp:.
+000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008b0: 6a73 6f6e 5f72 6573 756c 7420 3d20 6177  json_result = aw
+000008c0: 6169 7420 5f63 6865 636b 5f72 6573 706f  ait _check_respo
+000008d0: 6e73 6528 7265 7370 290a 2020 2020 2020  nse(resp).      
+000008e0: 2020 2020 2020 2020 2020 6966 206a 736f            if jso
+000008f0: 6e5f 7265 7375 6c74 3a0a 2020 2020 2020  n_result:.      
+00000900: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00000910: 7475 726e 206a 736f 6e5f 7265 7375 6c74  turn json_result
+00000920: 5b22 7265 7375 6c74 225d 0a20 2020 2020  ["result"].     
+00000930: 2020 2065 7863 6570 7420 4170 6945 7863     except ApiExc
+00000940: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
+00000950: 2020 2020 7261 6973 650a 2020 2020 2020      raise.      
+00000960: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00000970: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+00000980: 2020 2020 206c 6173 745f 6578 6365 7074       last_except
+00000990: 696f 6e20 3d20 650a 2020 2020 2020 2020  ion = e.        
+000009a0: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+000009b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000009c0: 2022 5265 7472 7969 6e67 2028 2573 202f   "Retrying (%s /
+000009d0: 2025 7329 2075 6e65 7870 6563 7465 6420   %s) unexpected 
+000009e0: 6572 726f 7220 6d61 6b69 6e67 2072 6571  error making req
+000009f0: 7565 7374 2028 2573 2922 2c0a 2020 2020  uest (%s)",.    
+00000a00: 2020 2020 2020 2020 2020 2020 6174 7465              atte
+00000a10: 6d70 7420 2b20 312c 0a20 2020 2020 2020  mpt + 1,.       
+00000a20: 2020 2020 2020 2020 204d 4158 5f52 4554           MAX_RET
+00000a30: 5249 4553 2c0a 2020 2020 2020 2020 2020  RIES,.          
+00000a40: 2020 2020 2020 7265 7175 6573 745f 6465        request_de
+00000a50: 7363 7269 7074 696f 6e2c 0a20 2020 2020  scription,.     
+00000a60: 2020 2020 2020 2020 2020 2065 7863 5f69             exc_i
+00000a70: 6e66 6f3d 5472 7565 2c0a 2020 2020 2020  nfo=True,.      
+00000a80: 2020 2020 2020 290a 2020 2020 656c 7365        ).    else
+00000a90: 3a0a 2020 2020 2020 2020 6966 206c 6173  :.        if las
+00000aa0: 745f 6578 6365 7074 696f 6e20 6973 206e  t_exception is n
+00000ab0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00000ac0: 2020 2020 206c 6f67 6765 722e 6572 726f       logger.erro
+00000ad0: 7228 2252 6571 7565 7374 2028 2573 2920  r("Request (%s) 
+00000ae0: 6469 646e 2774 2073 7563 6365 6564 6564  didn't succeeded
+00000af0: 2c20 7265 7261 6973 696e 6720 6c61 7374  , reraising last
+00000b00: 2065 7863 6570 7469 6f6e 222c 2072 6571   exception", req
+00000b10: 7565 7374 5f64 6573 6372 6970 7469 6f6e  uest_description
+00000b20: 290a 2020 2020 2020 2020 2020 2020 7261  ).            ra
+00000b30: 6973 6520 6c61 7374 5f65 7863 6570 7469  ise last_excepti
+00000b40: 6f6e 0a0a 0a64 6566 2065 7874 7261 6374  on...def extract
+00000b50: 5f66 696c 656e 616d 6528 6f62 6a3a 2041  _filename(obj: A
+00000b60: 6e79 2920 2d3e 204f 7074 696f 6e61 6c5b  ny) -> Optional[
+00000b70: 7374 725d 3a0a 2020 2020 6e61 6d65 203d  str]:.    name =
+00000b80: 2067 6574 6174 7472 286f 626a 2c20 226e   getattr(obj, "n
+00000b90: 616d 6522 2c20 4e6f 6e65 290a 2020 2020  ame", None).    
+00000ba0: 6966 206e 616d 6520 616e 6420 6973 696e  if name and isin
+00000bb0: 7374 616e 6365 286e 616d 652c 2073 7472  stance(name, str
+00000bc0: 2920 616e 6420 6e61 6d65 5b30 5d20 213d  ) and name[0] !=
+00000bd0: 2022 3c22 2061 6e64 206e 616d 655b 2d31   "<" and name[-1
+00000be0: 5d20 213d 2022 3e22 3a0a 2020 2020 2020  ] != ">":.      
+00000bf0: 2020 7265 7475 726e 206f 732e 7061 7468    return os.path
+00000c00: 2e62 6173 656e 616d 6528 6e61 6d65 290a  .basename(name).
+00000c10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00000c20: 2020 7265 7475 726e 204e 6f6e 650a 0a0a    return None...
+00000c30: 6465 6620 746f 5f66 6f72 6d5f 6461 7461  def to_form_data
+00000c40: 2870 6172 616d 733a 204f 7074 696f 6e61  (params: Optiona
+00000c50: 6c5b 5061 7261 6d73 5d20 3d20 4e6f 6e65  l[Params] = None
+00000c60: 2c20 6669 6c65 733a 204f 7074 696f 6e61  , files: Optiona
+00000c70: 6c5b 4669 6c65 735d 203d 204e 6f6e 6529  l[Files] = None)
+00000c80: 202d 3e20 6169 6f68 7474 702e 466f 726d   -> aiohttp.Form
+00000c90: 4461 7461 3a0a 2020 2020 6461 7461 203d  Data:.    data =
+00000ca0: 2061 696f 6874 7470 2e66 6f72 6d64 6174   aiohttp.formdat
+00000cb0: 612e 466f 726d 4461 7461 2871 756f 7465  a.FormData(quote
+00000cc0: 5f66 6965 6c64 733d 4661 6c73 6529 0a0a  _fields=False)..
+00000cd0: 2020 2020 6966 2070 6172 616d 733a 0a20      if params:. 
+00000ce0: 2020 2020 2020 2066 6f72 206b 6579 2c20         for key, 
+00000cf0: 7661 6c75 6520 696e 2070 6172 616d 732e  value in params.
+00000d00: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00000d10: 2020 2020 2064 6174 612e 6164 645f 6669       data.add_fi
+00000d20: 656c 6428 6b65 792c 2073 7472 2876 616c  eld(key, str(val
+00000d30: 7565 2929 0a0a 2020 2020 6966 2066 696c  ue))..    if fil
+00000d40: 6573 3a0a 2020 2020 2020 2020 666f 7220  es:.        for 
+00000d50: 6b65 792c 2066 2069 6e20 6669 6c65 732e  key, f in files.
+00000d60: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00000d70: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00000d80: 6365 2866 2c20 7475 706c 6529 3a0a 2020  ce(f, tuple):.  
+00000d90: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00000da0: 206c 656e 2866 2920 3d3d 2032 3a0a 2020   len(f) == 2:.  
+00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000dc0: 2020 6669 6c65 6e61 6d65 2c20 6669 6c65    filename, file
+00000dd0: 5f6f 626a 6563 7420 3d20 660a 2020 2020  _object = f.    
+00000de0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00000df0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000e00: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00000e10: 6545 7272 6f72 2822 5475 706c 6520 6d75  eError("Tuple mu
+00000e20: 7374 2068 6176 6520 6578 6163 746c 7920  st have exactly 
+00000e30: 3220 656c 656d 656e 7473 3a20 6669 6c65  2 elements: file
+00000e40: 6e61 6d65 2c20 6669 6c65 5f6f 626a 6563  name, file_objec
+00000e50: 7422 290a 2020 2020 2020 2020 2020 2020  t").            
+00000e60: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00000e70: 2020 2020 2020 6669 6c65 6e61 6d65 2c20        filename, 
+00000e80: 6669 6c65 5f6f 626a 6563 7420 3d20 6578  file_object = ex
+00000e90: 7472 6163 745f 6669 6c65 6e61 6d65 2866  tract_filename(f
+00000ea0: 2920 6f72 206b 6579 2c20 660a 0a20 2020  ) or key, f..   
+00000eb0: 2020 2020 2020 2020 2064 6174 612e 6164           data.ad
+00000ec0: 645f 6669 656c 6428 6b65 792c 2066 696c  d_field(key, fil
+00000ed0: 655f 6f62 6a65 6374 2c20 6669 6c65 6e61  e_object, filena
+00000ee0: 6d65 3d66 696c 656e 616d 6529 0a0a 2020  me=filename)..  
+00000ef0: 2020 7265 7475 726e 2064 6174 610a 0a0a    return data...
+00000f00: 6173 796e 6320 6465 6620 5f63 6f6e 7665  async def _conve
+00000f10: 7274 5f6d 6172 6b75 7028 6d61 726b 7570  rt_markup(markup
+00000f20: 293a 0a20 2020 2069 6620 6973 696e 7374  ):.    if isinst
+00000f30: 616e 6365 286d 6172 6b75 702c 2074 7970  ance(markup, typ
+00000f40: 6573 2e4a 736f 6e53 6572 6961 6c69 7a61  es.JsonSerializa
+00000f50: 626c 6529 3a0a 2020 2020 2020 2020 7265  ble):.        re
+00000f60: 7475 726e 206d 6172 6b75 702e 746f 5f6a  turn markup.to_j
+00000f70: 736f 6e28 290a 2020 2020 7265 7475 726e  son().    return
+00000f80: 206d 6172 6b75 700a 0a0a 6173 796e 6320   markup...async 
+00000f90: 6465 6620 6765 745f 6d65 2874 6f6b 656e  def get_me(token
+00000fa0: 293a 0a20 2020 2072 6574 7572 6e20 6177  ):.    return aw
+00000fb0: 6169 7420 5f72 6571 7565 7374 2874 6f6b  ait _request(tok
+00000fc0: 656e 2c20 2267 6574 4d65 2229 0a0a 0a61  en, "getMe")...a
+00000fd0: 7379 6e63 2064 6566 206c 6f67 5f6f 7574  sync def log_out
+00000fe0: 2874 6f6b 656e 293a 0a20 2020 2072 6574  (token):.    ret
+00000ff0: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
+00001000: 7374 2874 6f6b 656e 2c20 226c 6f67 4f75  st(token, "logOu
+00001010: 7422 290a 0a0a 6173 796e 6320 6465 6620  t")...async def 
+00001020: 636c 6f73 6528 746f 6b65 6e29 3a0a 2020  close(token):.  
+00001030: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
+00001040: 7265 7175 6573 7428 746f 6b65 6e2c 2022  request(token, "
+00001050: 636c 6f73 6522 290a 0a0a 6173 796e 6320  close")...async 
+00001060: 6465 6620 6765 745f 6669 6c65 2874 6f6b  def get_file(tok
+00001070: 656e 2c20 6669 6c65 5f69 6429 3a0a 2020  en, file_id):.  
+00001080: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
+00001090: 7265 7175 6573 7428 746f 6b65 6e2c 2022  request(token, "
+000010a0: 6765 7446 696c 6522 2c20 7061 7261 6d73  getFile", params
+000010b0: 3d7b 2266 696c 655f 6964 223a 2066 696c  ={"file_id": fil
+000010c0: 655f 6964 7d29 0a0a 0a61 7379 6e63 2064  e_id})...async d
+000010d0: 6566 2067 6574 5f66 696c 655f 7572 6c28  ef get_file_url(
+000010e0: 746f 6b65 6e3a 2073 7472 2c20 6669 6c65  token: str, file
+000010f0: 5f69 643a 2073 7472 293a 0a20 2020 2069  _id: str):.    i
+00001100: 6620 4649 4c45 5f55 524c 2069 7320 4e6f  f FILE_URL is No
+00001110: 6e65 3a0a 2020 2020 2020 2020 7265 7475  ne:.        retu
+00001120: 726e 2022 6874 7470 733a 2f2f 6170 692e  rn "https://api.
+00001130: 7465 6c65 6772 616d 2e6f 7267 2f66 696c  telegram.org/fil
+00001140: 652f 626f 747b 307d 2f7b 317d 222e 666f  e/bot{0}/{1}".fo
+00001150: 726d 6174 2874 6f6b 656e 2c20 6177 6169  rmat(token, awai
+00001160: 7420 6765 745f 6669 6c65 2874 6f6b 656e  t get_file(token
+00001170: 2c20 6669 6c65 5f69 6429 5b22 6669 6c65  , file_id)["file
+00001180: 5f70 6174 6822 5d29 0a20 2020 2065 6c73  _path"]).    els
+00001190: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
+000011a0: 6e20 4649 4c45 5f55 524c 2e66 6f72 6d61  n FILE_URL.forma
+000011b0: 7428 746f 6b65 6e2c 2061 7761 6974 2067  t(token, await g
+000011c0: 6574 5f66 696c 6528 746f 6b65 6e2c 2066  et_file(token, f
+000011d0: 696c 655f 6964 295b 2266 696c 655f 7061  ile_id)["file_pa
+000011e0: 7468 225d 290a 0a0a 6173 796e 6320 6465  th"])...async de
+000011f0: 6620 646f 776e 6c6f 6164 5f66 696c 6528  f download_file(
+00001200: 746f 6b65 6e3a 2073 7472 2c20 6669 6c65  token: str, file
+00001210: 5f70 6174 683a 2073 7472 293a 0a20 2020  _path: str):.   
+00001220: 2069 6620 4649 4c45 5f55 524c 2069 7320   if FILE_URL is 
+00001230: 4e6f 6e65 3a0a 2020 2020 2020 2020 7572  None:.        ur
+00001240: 6c20 3d20 2268 7474 7073 3a2f 2f61 7069  l = "https://api
+00001250: 2e74 656c 6567 7261 6d2e 6f72 672f 6669  .telegram.org/fi
+00001260: 6c65 2f62 6f74 7b30 7d2f 7b31 7d22 2e66  le/bot{0}/{1}".f
+00001270: 6f72 6d61 7428 746f 6b65 6e2c 2066 696c  ormat(token, fil
+00001280: 655f 7061 7468 290a 2020 2020 656c 7365  e_path).    else
+00001290: 3a0a 2020 2020 2020 2020 7572 6c20 3d20  :.        url = 
+000012a0: 4649 4c45 5f55 524c 2e66 6f72 6d61 7428  FILE_URL.format(
+000012b0: 746f 6b65 6e2c 2066 696c 655f 7061 7468  token, file_path
+000012c0: 290a 2020 2020 7365 7373 696f 6e20 3d20  ).    session = 
+000012d0: 6177 6169 7420 7365 7373 696f 6e5f 6d61  await session_ma
+000012e0: 6e61 6765 722e 6765 745f 7365 7373 696f  nager.get_sessio
+000012f0: 6e28 290a 2020 2020 6173 796e 6320 7769  n().    async wi
+00001300: 7468 2073 6573 7369 6f6e 2e67 6574 2875  th session.get(u
+00001310: 726c 2920 6173 2072 6573 706f 6e73 653a  rl) as response:
+00001320: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00001330: 3d20 6177 6169 7420 7265 7370 6f6e 7365  = await response
+00001340: 2e72 6561 6428 290a 2020 2020 2020 2020  .read().        
+00001350: 6966 2072 6573 706f 6e73 652e 7374 6174  if response.stat
+00001360: 7573 2021 3d20 3230 303a 0a20 2020 2020  us != 200:.     
+00001370: 2020 2020 2020 2072 6169 7365 2041 7069         raise Api
+00001380: 4854 5450 4578 6365 7074 696f 6e28 2245  HTTPException("E
+00001390: 7272 6f72 2064 6f77 6e6c 6f61 6469 6e67  rror downloading
+000013a0: 2066 696c 6522 2c20 7265 7370 6f6e 7365   file", response
+000013b0: 290a 0a20 2020 2072 6574 7572 6e20 7265  )..    return re
+000013c0: 7375 6c74 0a0a 0a61 7379 6e63 2064 6566  sult...async def
+000013d0: 2073 6574 5f77 6562 686f 6f6b 280a 2020   set_webhook(.  
+000013e0: 2020 746f 6b65 6e3a 2073 7472 2c0a 2020    token: str,.  
+000013f0: 2020 7572 6c3a 2073 7472 203d 204e 6f6e    url: str = Non
+00001400: 652c 0a20 2020 2063 6572 7469 6669 6361  e,.    certifica
+00001410: 7465 3a20 4f70 7469 6f6e 616c 5b46 696c  te: Optional[Fil
+00001420: 654f 626a 6563 745d 203d 204e 6f6e 652c  eObject] = None,
+00001430: 0a20 2020 206d 6178 5f63 6f6e 6e65 6374  .    max_connect
+00001440: 696f 6e73 3a20 4f70 7469 6f6e 616c 5b69  ions: Optional[i
+00001450: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
+00001460: 616c 6c6f 7765 645f 7570 6461 7465 733a  allowed_updates:
+00001470: 204f 7074 696f 6e61 6c5b 6c69 7374 5b73   Optional[list[s
+00001480: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
+00001490: 2069 705f 6164 6472 6573 733a 204f 7074   ip_address: Opt
+000014a0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000014b0: 652c 0a20 2020 2064 726f 705f 7065 6e64  e,.    drop_pend
+000014c0: 696e 675f 7570 6461 7465 733a 204f 7074  ing_updates: Opt
+000014d0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+000014e0: 6e65 2c0a 2020 2020 7469 6d65 6f75 743a  ne,.    timeout:
+000014f0: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
+00001500: 203d 204e 6f6e 652c 0a20 2020 2073 6563   = None,.    sec
+00001510: 7265 745f 746f 6b65 6e3a 204f 7074 696f  ret_token: Optio
+00001520: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+00001530: 0a29 3a0a 2020 2020 6669 6c65 733a 204f  .):.    files: O
+00001540: 7074 696f 6e61 6c5b 4669 6c65 735d 203d  ptional[Files] =
+00001550: 207b 2263 6572 7469 6669 6361 7465 223a   {"certificate":
+00001560: 2063 6572 7469 6669 6361 7465 7d20 6966   certificate} if
+00001570: 2063 6572 7469 6669 6361 7465 2065 6c73   certificate els
+00001580: 6520 4e6f 6e65 0a20 2020 2070 6172 616d  e None.    param
+00001590: 733a 2050 6172 616d 7320 3d20 7b22 7572  s: Params = {"ur
+000015a0: 6c22 3a20 7572 6c7d 0a20 2020 2069 6620  l": url}.    if 
+000015b0: 6d61 785f 636f 6e6e 6563 7469 6f6e 733a  max_connections:
+000015c0: 0a20 2020 2020 2020 2070 6172 616d 735b  .        params[
+000015d0: 226d 6178 5f63 6f6e 6e65 6374 696f 6e73  "max_connections
+000015e0: 225d 203d 206d 6178 5f63 6f6e 6e65 6374  "] = max_connect
+000015f0: 696f 6e73 0a20 2020 2069 6620 616c 6c6f  ions.    if allo
+00001600: 7765 645f 7570 6461 7465 7320 6973 206e  wed_updates is n
+00001610: 6f74 204e 6f6e 653a 2020 2320 456d 7074  ot None:  # Empt
+00001620: 7920 6c69 7374 7320 7368 6f75 6c64 2070  y lists should p
+00001630: 6173 730a 2020 2020 2020 2020 7061 7261  ass.        para
+00001640: 6d73 5b22 616c 6c6f 7765 645f 7570 6461  ms["allowed_upda
+00001650: 7465 7322 5d20 3d20 6a73 6f6e 2e64 756d  tes"] = json.dum
+00001660: 7073 2861 6c6c 6f77 6564 5f75 7064 6174  ps(allowed_updat
+00001670: 6573 290a 2020 2020 6966 2069 705f 6164  es).    if ip_ad
+00001680: 6472 6573 7320 6973 206e 6f74 204e 6f6e  dress is not Non
+00001690: 653a 2020 2320 456d 7074 7920 7374 7269  e:  # Empty stri
+000016a0: 6e67 2073 686f 756c 6420 7061 7373 0a20  ng should pass. 
+000016b0: 2020 2020 2020 2070 6172 616d 735b 2269         params["i
+000016c0: 705f 6164 6472 6573 7322 5d20 3d20 6970  p_address"] = ip
+000016d0: 5f61 6464 7265 7373 0a20 2020 2069 6620  _address.    if 
+000016e0: 6472 6f70 5f70 656e 6469 6e67 5f75 7064  drop_pending_upd
+000016f0: 6174 6573 2069 7320 6e6f 7420 4e6f 6e65  ates is not None
+00001700: 3a20 2023 2041 6e79 2062 6f6f 6c20 7661  :  # Any bool va
+00001710: 6c75 6520 7368 6f75 6c64 2070 6173 730a  lue should pass.
+00001720: 2020 2020 2020 2020 7061 7261 6d73 5b22          params["
+00001730: 6472 6f70 5f70 656e 6469 6e67 5f75 7064  drop_pending_upd
+00001740: 6174 6573 225d 203d 2064 726f 705f 7065  ates"] = drop_pe
+00001750: 6e64 696e 675f 7570 6461 7465 730a 2020  nding_updates.  
+00001760: 2020 6966 2073 6563 7265 745f 746f 6b65    if secret_toke
+00001770: 6e3a 0a20 2020 2020 2020 2070 6172 616d  n:.        param
+00001780: 735b 2273 6563 7265 745f 746f 6b65 6e22  s["secret_token"
+00001790: 5d20 3d20 7365 6372 6574 5f74 6f6b 656e  ] = secret_token
+000017a0: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
+000017b0: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
+000017c0: 2c20 726f 7574 653d 2273 6574 5765 6268  , route="setWebh
+000017d0: 6f6f 6b22 2c20 7061 7261 6d73 3d70 6172  ook", params=par
+000017e0: 616d 732c 2066 696c 6573 3d66 696c 6573  ams, files=files
+000017f0: 2c20 7265 7175 6573 745f 7469 6d65 6f75  , request_timeou
+00001800: 743d 7469 6d65 6f75 7429 0a0a 0a61 7379  t=timeout)...asy
+00001810: 6e63 2064 6566 2064 656c 6574 655f 7765  nc def delete_we
+00001820: 6268 6f6f 6b28 746f 6b65 6e2c 2064 726f  bhook(token, dro
+00001830: 705f 7065 6e64 696e 675f 7570 6461 7465  p_pending_update
+00001840: 733d 4e6f 6e65 2c20 7469 6d65 6f75 743d  s=None, timeout=
+00001850: 4e6f 6e65 293a 0a20 2020 206d 6574 686f  None):.    metho
+00001860: 645f 7572 6c20 3d20 7222 6465 6c65 7465  d_url = r"delete
+00001870: 5765 6268 6f6f 6b22 0a20 2020 2070 6179  Webhook".    pay
+00001880: 6c6f 6164 203d 207b 7d0a 2020 2020 6966  load = {}.    if
+00001890: 2064 726f 705f 7065 6e64 696e 675f 7570   drop_pending_up
+000018a0: 6461 7465 7320 6973 206e 6f74 204e 6f6e  dates is not Non
+000018b0: 653a 2020 2320 416e 7920 626f 6f6c 2076  e:  # Any bool v
+000018c0: 616c 7565 2073 686f 756c 6420 7061 7373  alue should pass
+000018d0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+000018e0: 5b22 6472 6f70 5f70 656e 6469 6e67 5f75  ["drop_pending_u
+000018f0: 7064 6174 6573 225d 203d 2064 726f 705f  pdates"] = drop_
+00001900: 7065 6e64 696e 675f 7570 6461 7465 730a  pending_updates.
+00001910: 2020 2020 6966 2074 696d 656f 7574 3a0a      if timeout:.
+00001920: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
+00001930: 2274 696d 656f 7574 225d 203d 2074 696d  "timeout"] = tim
+00001940: 656f 7574 0a20 2020 2072 6574 7572 6e20  eout.    return 
+00001950: 6177 6169 7420 5f72 6571 7565 7374 2874  await _request(t
+00001960: 6f6b 656e 2c20 6d65 7468 6f64 5f75 726c  oken, method_url
+00001970: 2c20 7061 7261 6d73 3d70 6179 6c6f 6164  , params=payload
+00001980: 290a 0a0a 6173 796e 6320 6465 6620 6765  )...async def ge
+00001990: 745f 7765 6268 6f6f 6b5f 696e 666f 2874  t_webhook_info(t
+000019a0: 6f6b 656e 2c20 7469 6d65 6f75 743d 4e6f  oken, timeout=No
+000019b0: 6e65 293a 0a20 2020 206d 6574 686f 645f  ne):.    method_
+000019c0: 7572 6c20 3d20 7222 6765 7457 6562 686f  url = r"getWebho
+000019d0: 6f6b 496e 666f 220a 2020 2020 7061 796c  okInfo".    payl
+000019e0: 6f61 6420 3d20 7b7d 0a20 2020 2069 6620  oad = {}.    if 
+000019f0: 7469 6d65 6f75 743a 0a20 2020 2020 2020  timeout:.       
+00001a00: 2070 6179 6c6f 6164 5b22 7469 6d65 6f75   payload["timeou
+00001a10: 7422 5d20 3d20 7469 6d65 6f75 740a 2020  t"] = timeout.  
+00001a20: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
+00001a30: 7265 7175 6573 7428 746f 6b65 6e2c 206d  request(token, m
+00001a40: 6574 686f 645f 7572 6c2c 2070 6172 616d  ethod_url, param
+00001a50: 733d 7061 796c 6f61 6429 0a0a 0a61 7379  s=payload)...asy
+00001a60: 6e63 2064 6566 2067 6574 5f75 7064 6174  nc def get_updat
+00001a70: 6573 280a 2020 2020 746f 6b65 6e3a 2073  es(.    token: s
+00001a80: 7472 2c0a 2020 2020 6f66 6673 6574 3a20  tr,.    offset: 
+00001a90: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00001aa0: 4e6f 6e65 2c0a 2020 2020 6c69 6d69 743a  None,.    limit:
+00001ab0: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+00001ac0: 204e 6f6e 652c 0a20 2020 2074 696d 656f   None,.    timeo
+00001ad0: 7574 3a20 4f70 7469 6f6e 616c 5b66 6c6f  ut: Optional[flo
+00001ae0: 6174 5d20 3d20 4e6f 6e65 2c0a 2020 2020  at] = None,.    
+00001af0: 616c 6c6f 7765 645f 7570 6461 7465 733a  allowed_updates:
+00001b00: 204f 7074 696f 6e61 6c5b 6c69 7374 5b73   Optional[list[s
+00001b10: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
+00001b20: 2072 6571 7565 7374 5f74 696d 656f 7574   request_timeout
+00001b30: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
+00001b40: 5d20 3d20 4e6f 6e65 2c0a 293a 0a20 2020  ] = None,.):.   
+00001b50: 2070 6172 616d 733a 2064 6963 7420 3d20   params: dict = 
+00001b60: 7b7d 0a20 2020 2069 6620 6f66 6673 6574  {}.    if offset
+00001b70: 3a0a 2020 2020 2020 2020 7061 7261 6d73  :.        params
+00001b80: 5b22 6f66 6673 6574 225d 203d 206f 6666  ["offset"] = off
+00001b90: 7365 740a 2020 2020 6966 206c 696d 6974  set.    if limit
+00001ba0: 3a0a 2020 2020 2020 2020 7061 7261 6d73  :.        params
+00001bb0: 5b22 6c69 6d69 7422 5d20 3d20 6c69 6d69  ["limit"] = limi
+00001bc0: 740a 2020 2020 6966 2074 696d 656f 7574  t.    if timeout
+00001bd0: 3a0a 2020 2020 2020 2020 7061 7261 6d73  :.        params
+00001be0: 5b22 7469 6d65 6f75 7422 5d20 3d20 7469  ["timeout"] = ti
+00001bf0: 6d65 6f75 740a 2020 2020 6966 2061 6c6c  meout.    if all
+00001c00: 6f77 6564 5f75 7064 6174 6573 3a0a 2020  owed_updates:.  
+00001c10: 2020 2020 2020 7061 7261 6d73 5b22 616c        params["al
+00001c20: 6c6f 7765 645f 7570 6461 7465 7322 5d20  lowed_updates"] 
+00001c30: 3d20 6a73 6f6e 2e64 756d 7073 2861 6c6c  = json.dumps(all
+00001c40: 6f77 6564 5f75 7064 6174 6573 290a 2020  owed_updates).  
+00001c50: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
+00001c60: 7265 7175 6573 7428 746f 6b65 6e2c 2072  request(token, r
+00001c70: 6f75 7465 3d22 6765 7455 7064 6174 6573  oute="getUpdates
+00001c80: 222c 2070 6172 616d 733d 7061 7261 6d73  ", params=params
+00001c90: 2c20 7265 7175 6573 745f 7469 6d65 6f75  , request_timeou
+00001ca0: 743d 7265 7175 6573 745f 7469 6d65 6f75  t=request_timeou
+00001cb0: 7429 0a0a 0a61 7379 6e63 2064 6566 205f  t)...async def _
+00001cc0: 6368 6563 6b5f 7265 7370 6f6e 7365 2872  check_response(r
+00001cd0: 6573 706f 6e73 653a 2061 696f 6874 7470  esponse: aiohttp
+00001ce0: 2e43 6c69 656e 7452 6573 706f 6e73 6529  .ClientResponse)
+00001cf0: 3a0a 2020 2020 2222 220a 2020 2020 4368  :.    """.    Ch
+00001d00: 6563 6b73 2077 6865 7468 6572 2060 7265  ecks whether `re
+00001d10: 7375 6c74 6020 6973 2061 2076 616c 6964  sult` is a valid
+00001d20: 2041 5049 2072 6573 706f 6e73 652e 0a20   API response.. 
+00001d30: 2020 2041 2072 6573 756c 7420 6973 2063     A result is c
+00001d40: 6f6e 7369 6465 7265 6420 696e 7661 6c69  onsidered invali
+00001d50: 6420 6966 3a0a 2020 2020 2020 2020 2d20  d if:.        - 
+00001d60: 5468 6520 7365 7276 6572 2072 6574 7572  The server retur
+00001d70: 6e65 6420 616e 2048 5454 5020 7265 7370  ned an HTTP resp
+00001d80: 6f6e 7365 2063 6f64 6520 6f74 6865 7220  onse code other 
+00001d90: 7468 616e 2032 3030 0a20 2020 2020 2020  than 200.       
+00001da0: 202d 2054 6865 2063 6f6e 7465 6e74 206f   - The content o
+00001db0: 6620 7468 6520 7265 7375 6c74 2069 7320  f the result is 
+00001dc0: 696e 7661 6c69 6420 4a53 4f4e 2e0a 2020  invalid JSON..  
+00001dd0: 2020 2020 2020 2d20 5468 6520 6d65 7468        - The meth
+00001de0: 6f64 2063 616c 6c20 7761 7320 756e 7375  od call was unsu
+00001df0: 6363 6573 7366 756c 2028 5468 6520 4a53  ccessful (The JS
+00001e00: 4f4e 2027 6f6b 2720 6669 656c 6420 6571  ON 'ok' field eq
+00001e10: 7561 6c73 2046 616c 7365 290a 0a20 2020  uals False)..   
+00001e20: 203a 7261 6973 6573 2041 7069 4578 6365   :raises ApiExce
+00001e30: 7074 696f 6e3a 2069 6620 6f6e 6520 6f66  ption: if one of
+00001e40: 2074 6865 2061 626f 7665 206c 6973 7465   the above liste
+00001e50: 6420 6361 7365 7320 6973 2061 7070 6c69  d cases is appli
+00001e60: 6361 626c 650a 2020 2020 3a70 6172 616d  cable.    :param
+00001e70: 206d 6574 686f 645f 6e61 6d65 3a20 5468   method_name: Th
+00001e80: 6520 6e61 6d65 206f 6620 7468 6520 6d65  e name of the me
+00001e90: 7468 6f64 2063 616c 6c65 640a 2020 2020  thod called.    
+00001ea0: 3a70 6172 616d 2072 6573 756c 743a 2054  :param result: T
+00001eb0: 6865 2072 6574 7572 6e65 6420 7265 7375  he returned resu
+00001ec0: 6c74 206f 6620 7468 6520 6d65 7468 6f64  lt of the method
+00001ed0: 2072 6571 7565 7374 0a20 2020 203a 7265   request.    :re
+00001ee0: 7475 726e 3a20 5468 6520 7265 7375 6c74  turn: The result
+00001ef0: 2070 6172 7365 6420 746f 2061 204a 534f   parsed to a JSO
+00001f00: 4e20 6469 6374 696f 6e61 7279 2e0a 2020  N dictionary..  
+00001f10: 2020 2222 220a 2020 2020 6177 6169 7420    """.    await 
+00001f20: 7265 7370 6f6e 7365 2e74 6578 7428 2920  response.text() 
+00001f30: 2023 206c 6f61 6469 6e67 2072 6573 706f   # loading respo
+00001f40: 6e73 6520 626f 6479 0a20 2020 2074 7279  nse body.    try
+00001f50: 3a0a 2020 2020 2020 2020 7265 7375 6c74  :.        result
+00001f60: 5f6a 736f 6e20 3d20 6177 6169 7420 7265  _json = await re
+00001f70: 7370 6f6e 7365 2e6a 736f 6e28 656e 636f  sponse.json(enco
+00001f80: 6469 6e67 3d22 7574 662d 3822 290a 2020  ding="utf-8").  
+00001f90: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00001fa0: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+00001fb0: 2072 6169 7365 2041 7069 496e 7661 6c69   raise ApiInvali
+00001fc0: 644a 534f 4e45 7863 6570 7469 6f6e 2872  dJSONException(r
+00001fd0: 6573 706f 6e73 652c 2065 290a 2020 2020  esponse, e).    
+00001fe0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00001ff0: 6528 7265 7375 6c74 5f6a 736f 6e2c 2064  e(result_json, d
+00002000: 6963 7429 206f 7220 7265 7375 6c74 5f6a  ict) or result_j
+00002010: 736f 6e2e 6765 7428 226f 6b22 2920 6973  son.get("ok") is
+00002020: 206e 6f74 2054 7275 653a 0a20 2020 2020   not True:.     
+00002030: 2020 2072 6169 7365 2041 7069 4854 5450     raise ApiHTTP
+00002040: 4578 6365 7074 696f 6e28 7265 7375 6c74  Exception(result
+00002050: 5f6a 736f 6e2c 2072 6573 706f 6e73 6529  _json, response)
+00002060: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
+00002070: 6c74 5f6a 736f 6e0a 0a0a 6465 6620 5f61  lt_json...def _a
+00002080: 6464 5f6d 6573 7361 6765 5f74 6872 6561  dd_message_threa
+00002090: 645f 6964 2870 6172 616d 733a 2044 6963  d_id(params: Dic
+000020a0: 745b 7374 722c 2041 6e79 5d2c 206d 6573  t[str, Any], mes
+000020b0: 7361 6765 5f74 6872 6561 645f 6964 3a20  sage_thread_id: 
+000020c0: 4f70 7469 6f6e 616c 5b69 6e74 5d29 202d  Optional[int]) -
+000020d0: 3e20 4e6f 6e65 3a0a 2020 2020 6966 206d  > None:.    if m
+000020e0: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+000020f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00002100: 2020 2020 2020 7061 7261 6d73 5b22 6d65        params["me
+00002110: 7373 6167 655f 7468 7265 6164 5f69 6422  ssage_thread_id"
+00002120: 5d20 3d20 6d65 7373 6167 655f 7468 7265  ] = message_thre
+00002130: 6164 5f69 640a 0a0a 6173 796e 6320 6465  ad_id...async de
+00002140: 6620 7365 6e64 5f6d 6573 7361 6765 280a  f send_message(.
+00002150: 2020 2020 746f 6b65 6e2c 0a20 2020 2063      token,.    c
+00002160: 6861 745f 6964 2c0a 2020 2020 7465 7874  hat_id,.    text
+00002170: 2c0a 2020 2020 6469 7361 626c 655f 7765  ,.    disable_we
+00002180: 625f 7061 6765 5f70 7265 7669 6577 3d4e  b_page_preview=N
+00002190: 6f6e 652c 0a20 2020 2072 6570 6c79 5f74  one,.    reply_t
+000021a0: 6f5f 6d65 7373 6167 655f 6964 3d4e 6f6e  o_message_id=Non
+000021b0: 652c 0a20 2020 2072 6570 6c79 5f6d 6172  e,.    reply_mar
+000021c0: 6b75 703d 4e6f 6e65 2c0a 2020 2020 7061  kup=None,.    pa
+000021d0: 7273 655f 6d6f 6465 3d4e 6f6e 652c 0a20  rse_mode=None,. 
+000021e0: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
+000021f0: 6963 6174 696f 6e3d 4e6f 6e65 2c0a 2020  ication=None,.  
+00002200: 2020 7469 6d65 6f75 743d 4e6f 6e65 2c0a    timeout=None,.
+00002210: 2020 2020 656e 7469 7469 6573 3d4e 6f6e      entities=Non
+00002220: 652c 0a20 2020 2061 6c6c 6f77 5f73 656e  e,.    allow_sen
+00002230: 6469 6e67 5f77 6974 686f 7574 5f72 6570  ding_without_rep
+00002240: 6c79 3d4e 6f6e 652c 0a20 2020 2070 726f  ly=None,.    pro
+00002250: 7465 6374 5f63 6f6e 7465 6e74 3d4e 6f6e  tect_content=Non
+00002260: 652c 0a20 2020 206d 6573 7361 6765 5f74  e,.    message_t
+00002270: 6872 6561 645f 6964 3a20 4f70 7469 6f6e  hread_id: Option
+00002280: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
+00002290: 293a 0a20 2020 2022 2222 0a20 2020 2055  ):.    """.    U
+000022a0: 7365 2074 6869 7320 6d65 7468 6f64 2074  se this method t
+000022b0: 6f20 7365 6e64 2074 6578 7420 6d65 7373  o send text mess
+000022c0: 6167 6573 2e20 4f6e 2073 7563 6365 7373  ages. On success
+000022d0: 2c20 7468 6520 7365 6e74 204d 6573 7361  , the sent Messa
+000022e0: 6765 2069 7320 7265 7475 726e 6564 2e0a  ge is returned..
+000022f0: 2020 2020 3a70 6172 616d 2074 6f6b 656e      :param token
+00002300: 3a0a 2020 2020 3a70 6172 616d 2063 6861  :.    :param cha
+00002310: 745f 6964 3a0a 2020 2020 3a70 6172 616d  t_id:.    :param
+00002320: 2074 6578 743a 0a20 2020 203a 7061 7261   text:.    :para
+00002330: 6d20 6469 7361 626c 655f 7765 625f 7061  m disable_web_pa
+00002340: 6765 5f70 7265 7669 6577 3a0a 2020 2020  ge_preview:.    
+00002350: 3a70 6172 616d 2072 6570 6c79 5f74 6f5f  :param reply_to_
+00002360: 6d65 7373 6167 655f 6964 3a0a 2020 2020  message_id:.    
+00002370: 3a70 6172 616d 2072 6570 6c79 5f6d 6172  :param reply_mar
+00002380: 6b75 703a 0a20 2020 203a 7061 7261 6d20  kup:.    :param 
+00002390: 7061 7273 655f 6d6f 6465 3a0a 2020 2020  parse_mode:.    
+000023a0: 3a70 6172 616d 2064 6973 6162 6c65 5f6e  :param disable_n
+000023b0: 6f74 6966 6963 6174 696f 6e3a 0a20 2020  otification:.   
+000023c0: 203a 7061 7261 6d20 7469 6d65 6f75 743a   :param timeout:
+000023d0: 0a20 2020 203a 7061 7261 6d20 656e 7469  .    :param enti
+000023e0: 7469 6573 3a0a 2020 2020 3a70 6172 616d  ties:.    :param
+000023f0: 2061 6c6c 6f77 5f73 656e 6469 6e67 5f77   allow_sending_w
+00002400: 6974 686f 7574 5f72 6570 6c79 3a0a 2020  ithout_reply:.  
+00002410: 2020 3a70 6172 616d 2070 726f 7465 6374    :param protect
+00002420: 5f63 6f6e 7465 6e74 3a0a 2020 2020 3a72  _content:.    :r
+00002430: 6574 7572 6e3a 0a20 2020 2022 2222 0a20  eturn:.    """. 
+00002440: 2020 206d 6574 686f 645f 6e61 6d65 203d     method_name =
+00002450: 2022 7365 6e64 4d65 7373 6167 6522 0a20   "sendMessage". 
+00002460: 2020 2070 6172 616d 7320 3d20 7b22 6368     params = {"ch
+00002470: 6174 5f69 6422 3a20 7374 7228 6368 6174  at_id": str(chat
+00002480: 5f69 6429 2c20 2274 6578 7422 3a20 7465  _id), "text": te
+00002490: 7874 7d0a 2020 2020 6966 2064 6973 6162  xt}.    if disab
+000024a0: 6c65 5f77 6562 5f70 6167 655f 7072 6576  le_web_page_prev
+000024b0: 6965 7720 6973 206e 6f74 204e 6f6e 653a  iew is not None:
+000024c0: 0a20 2020 2020 2020 2070 6172 616d 735b  .        params[
+000024d0: 2264 6973 6162 6c65 5f77 6562 5f70 6167  "disable_web_pag
+000024e0: 655f 7072 6576 6965 7722 5d20 3d20 6469  e_preview"] = di
+000024f0: 7361 626c 655f 7765 625f 7061 6765 5f70  sable_web_page_p
+00002500: 7265 7669 6577 0a20 2020 2069 6620 7265  review.    if re
+00002510: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
+00002520: 643a 0a20 2020 2020 2020 2070 6172 616d  d:.        param
+00002530: 735b 2272 6570 6c79 5f74 6f5f 6d65 7373  s["reply_to_mess
+00002540: 6167 655f 6964 225d 203d 2072 6570 6c79  age_id"] = reply
+00002550: 5f74 6f5f 6d65 7373 6167 655f 6964 0a20  _to_message_id. 
+00002560: 2020 2069 6620 7265 706c 795f 6d61 726b     if reply_mark
+00002570: 7570 3a0a 2020 2020 2020 2020 7061 7261  up:.        para
+00002580: 6d73 5b22 7265 706c 795f 6d61 726b 7570  ms["reply_markup
+00002590: 225d 203d 2061 7761 6974 205f 636f 6e76  "] = await _conv
+000025a0: 6572 745f 6d61 726b 7570 2872 6570 6c79  ert_markup(reply
+000025b0: 5f6d 6172 6b75 7029 0a20 2020 2069 6620  _markup).    if 
+000025c0: 7061 7273 655f 6d6f 6465 3a0a 2020 2020  parse_mode:.    
+000025d0: 2020 2020 7061 7261 6d73 5b22 7061 7273      params["pars
+000025e0: 655f 6d6f 6465 225d 203d 2070 6172 7365  e_mode"] = parse
+000025f0: 5f6d 6f64 650a 2020 2020 6966 2064 6973  _mode.    if dis
+00002600: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00002610: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+00002620: 2020 2020 2020 2070 6172 616d 735b 2264         params["d
+00002630: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+00002640: 696f 6e22 5d20 3d20 6469 7361 626c 655f  ion"] = disable_
+00002650: 6e6f 7469 6669 6361 7469 6f6e 0a20 2020  notification.   
+00002660: 2069 6620 7469 6d65 6f75 743a 0a20 2020   if timeout:.   
+00002670: 2020 2020 2070 6172 616d 735b 2274 696d       params["tim
+00002680: 656f 7574 225d 203d 2074 696d 656f 7574  eout"] = timeout
+00002690: 0a20 2020 2069 6620 656e 7469 7469 6573  .    if entities
+000026a0: 3a0a 2020 2020 2020 2020 7061 7261 6d73  :.        params
+000026b0: 5b22 656e 7469 7469 6573 225d 203d 206a  ["entities"] = j
+000026c0: 736f 6e2e 6475 6d70 7328 7479 7065 732e  son.dumps(types.
+000026d0: 4d65 7373 6167 6545 6e74 6974 792e 746f  MessageEntity.to
+000026e0: 5f6c 6973 745f 6f66 5f64 6963 7473 2865  _list_of_dicts(e
+000026f0: 6e74 6974 6965 7329 290a 2020 2020 6966  ntities)).    if
+00002700: 2061 6c6c 6f77 5f73 656e 6469 6e67 5f77   allow_sending_w
+00002710: 6974 686f 7574 5f72 6570 6c79 2069 7320  ithout_reply is 
+00002720: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00002730: 2020 7061 7261 6d73 5b22 616c 6c6f 775f    params["allow_
+00002740: 7365 6e64 696e 675f 7769 7468 6f75 745f  sending_without_
+00002750: 7265 706c 7922 5d20 3d20 616c 6c6f 775f  reply"] = allow_
+00002760: 7365 6e64 696e 675f 7769 7468 6f75 745f  sending_without_
+00002770: 7265 706c 790a 2020 2020 6966 2070 726f  reply.    if pro
+00002780: 7465 6374 5f63 6f6e 7465 6e74 2069 7320  tect_content is 
+00002790: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000027a0: 2020 7061 7261 6d73 5b22 7072 6f74 6563    params["protec
+000027b0: 745f 636f 6e74 656e 7422 5d20 3d20 7072  t_content"] = pr
+000027c0: 6f74 6563 745f 636f 6e74 656e 740a 2020  otect_content.  
+000027d0: 2020 5f61 6464 5f6d 6573 7361 6765 5f74    _add_message_t
+000027e0: 6872 6561 645f 6964 2870 6172 616d 732c  hread_id(params,
+000027f0: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
+00002800: 6964 290a 2020 2020 7265 7475 726e 2061  id).    return a
+00002810: 7761 6974 205f 7265 7175 6573 7428 746f  wait _request(to
+00002820: 6b65 6e2c 206d 6574 686f 645f 6e61 6d65  ken, method_name
+00002830: 2c20 7061 7261 6d73 3d70 6172 616d 7329  , params=params)
+00002840: 0a0a 0a23 206d 6574 686f 6473 0a0a 0a61  ...# methods...a
+00002850: 7379 6e63 2064 6566 2067 6574 5f75 7365  sync def get_use
+00002860: 725f 7072 6f66 696c 655f 7068 6f74 6f73  r_profile_photos
+00002870: 2874 6f6b 656e 2c20 7573 6572 5f69 642c  (token, user_id,
+00002880: 206f 6666 7365 743d 4e6f 6e65 2c20 6c69   offset=None, li
+00002890: 6d69 743d 4e6f 6e65 293a 0a20 2020 206d  mit=None):.    m
+000028a0: 6574 686f 645f 7572 6c20 3d20 7222 6765  ethod_url = r"ge
+000028b0: 7455 7365 7250 726f 6669 6c65 5068 6f74  tUserProfilePhot
+000028c0: 6f73 220a 2020 2020 7061 796c 6f61 6420  os".    payload 
+000028d0: 3d20 7b22 7573 6572 5f69 6422 3a20 7573  = {"user_id": us
+000028e0: 6572 5f69 647d 0a20 2020 2069 6620 6f66  er_id}.    if of
+000028f0: 6673 6574 3a0a 2020 2020 2020 2020 7061  fset:.        pa
+00002900: 796c 6f61 645b 226f 6666 7365 7422 5d20  yload["offset"] 
+00002910: 3d20 6f66 6673 6574 0a20 2020 2069 6620  = offset.    if 
+00002920: 6c69 6d69 743a 0a20 2020 2020 2020 2070  limit:.        p
+00002930: 6179 6c6f 6164 5b22 6c69 6d69 7422 5d20  ayload["limit"] 
+00002940: 3d20 6c69 6d69 740a 2020 2020 7265 7475  = limit.    retu
+00002950: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
+00002960: 7428 746f 6b65 6e2c 206d 6574 686f 645f  t(token, method_
+00002970: 7572 6c2c 2070 6172 616d 733d 7061 796c  url, params=payl
+00002980: 6f61 6429 0a0a 0a61 7379 6e63 2064 6566  oad)...async def
+00002990: 2067 6574 5f63 6861 7428 746f 6b65 6e2c   get_chat(token,
+000029a0: 2063 6861 745f 6964 293a 0a20 2020 206d   chat_id):.    m
+000029b0: 6574 686f 645f 7572 6c20 3d20 7222 6765  ethod_url = r"ge
+000029c0: 7443 6861 7422 0a20 2020 2070 6179 6c6f  tChat".    paylo
+000029d0: 6164 203d 207b 2263 6861 745f 6964 223a  ad = {"chat_id":
+000029e0: 2063 6861 745f 6964 7d0a 2020 2020 7265   chat_id}.    re
+000029f0: 7475 726e 2061 7761 6974 205f 7265 7175  turn await _requ
+00002a00: 6573 7428 746f 6b65 6e2c 206d 6574 686f  est(token, metho
+00002a10: 645f 7572 6c2c 2070 6172 616d 733d 7061  d_url, params=pa
+00002a20: 796c 6f61 6429 0a0a 0a61 7379 6e63 2064  yload)...async d
+00002a30: 6566 206c 6561 7665 5f63 6861 7428 746f  ef leave_chat(to
+00002a40: 6b65 6e2c 2063 6861 745f 6964 293a 0a20  ken, chat_id):. 
+00002a50: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
+00002a60: 7222 6c65 6176 6543 6861 7422 0a20 2020  r"leaveChat".   
+00002a70: 2070 6179 6c6f 6164 203d 207b 2263 6861   payload = {"cha
+00002a80: 745f 6964 223a 2063 6861 745f 6964 7d0a  t_id": chat_id}.
+00002a90: 2020 2020 7265 7475 726e 2061 7761 6974      return await
+00002aa0: 205f 7265 7175 6573 7428 746f 6b65 6e2c   _request(token,
+00002ab0: 206d 6574 686f 645f 7572 6c2c 2070 6172   method_url, par
+00002ac0: 616d 733d 7061 796c 6f61 6429 0a0a 0a61  ams=payload)...a
+00002ad0: 7379 6e63 2064 6566 2067 6574 5f63 6861  sync def get_cha
+00002ae0: 745f 6164 6d69 6e69 7374 7261 746f 7273  t_administrators
+00002af0: 2874 6f6b 656e 2c20 6368 6174 5f69 6429  (token, chat_id)
+00002b00: 3a0a 2020 2020 6d65 7468 6f64 5f75 726c  :.    method_url
+00002b10: 203d 2072 2267 6574 4368 6174 4164 6d69   = r"getChatAdmi
+00002b20: 6e69 7374 7261 746f 7273 220a 2020 2020  nistrators".    
+00002b30: 7061 796c 6f61 6420 3d20 7b22 6368 6174  payload = {"chat
+00002b40: 5f69 6422 3a20 6368 6174 5f69 647d 0a20  _id": chat_id}. 
+00002b50: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+00002b60: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
+00002b70: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
+00002b80: 6d73 3d70 6179 6c6f 6164 290a 0a0a 6173  ms=payload)...as
+00002b90: 796e 6320 6465 6620 6765 745f 6368 6174  ync def get_chat
+00002ba0: 5f6d 656d 6265 725f 636f 756e 7428 746f  _member_count(to
+00002bb0: 6b65 6e2c 2063 6861 745f 6964 293a 0a20  ken, chat_id):. 
+00002bc0: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
+00002bd0: 7222 6765 7443 6861 744d 656d 6265 7243  r"getChatMemberC
+00002be0: 6f75 6e74 220a 2020 2020 7061 796c 6f61  ount".    payloa
+00002bf0: 6420 3d20 7b22 6368 6174 5f69 6422 3a20  d = {"chat_id": 
+00002c00: 6368 6174 5f69 647d 0a20 2020 2072 6574  chat_id}.    ret
+00002c10: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
+00002c20: 7374 2874 6f6b 656e 2c20 6d65 7468 6f64  st(token, method
+00002c30: 5f75 726c 2c20 7061 7261 6d73 3d70 6179  _url, params=pay
+00002c40: 6c6f 6164 290a 0a0a 6173 796e 6320 6465  load)...async de
+00002c50: 6620 7365 745f 7374 6963 6b65 725f 7365  f set_sticker_se
+00002c60: 745f 7468 756d 6228 746f 6b65 6e2c 206e  t_thumb(token, n
+00002c70: 616d 652c 2075 7365 725f 6964 2c20 7468  ame, user_id, th
+00002c80: 756d 6229 3a0a 2020 2020 6d65 7468 6f64  umb):.    method
+00002c90: 5f75 726c 203d 2072 2273 6574 5374 6963  _url = r"setStic
+00002ca0: 6b65 7253 6574 5468 756d 6222 0a20 2020  kerSetThumb".   
+00002cb0: 2070 6179 6c6f 6164 203d 207b 226e 616d   payload = {"nam
+00002cc0: 6522 3a20 6e61 6d65 2c20 2275 7365 725f  e": name, "user_
+00002cd0: 6964 223a 2075 7365 725f 6964 7d0a 2020  id": user_id}.  
+00002ce0: 2020 6669 6c65 7320 3d20 7b7d 0a20 2020    files = {}.   
+00002cf0: 2069 6620 7468 756d 623a 0a20 2020 2020   if thumb:.     
+00002d00: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+00002d10: 616e 6365 2874 6875 6d62 2c20 7374 7229  ance(thumb, str)
+00002d20: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
+00002d30: 6c65 735b 2274 6875 6d62 225d 203d 2074  les["thumb"] = t
+00002d40: 6875 6d62 0a20 2020 2020 2020 2065 6c73  humb.        els
+00002d50: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+00002d60: 6179 6c6f 6164 5b22 7468 756d 6222 5d20  ayload["thumb"] 
+00002d70: 3d20 7468 756d 620a 2020 2020 7265 7475  = thumb.    retu
+00002d80: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
+00002d90: 7428 746f 6b65 6e2c 206d 6574 686f 645f  t(token, method_
+00002da0: 7572 6c2c 2070 6172 616d 733d 7061 796c  url, params=payl
+00002db0: 6f61 642c 2066 696c 6573 3d66 696c 6573  oad, files=files
+00002dc0: 206f 7220 4e6f 6e65 290a 0a0a 6173 796e   or None)...asyn
+00002dd0: 6320 6465 6620 7365 745f 6368 6174 5f73  c def set_chat_s
+00002de0: 7469 636b 6572 5f73 6574 2874 6f6b 656e  ticker_set(token
+00002df0: 2c20 6368 6174 5f69 642c 2073 7469 636b  , chat_id, stick
+00002e00: 6572 5f73 6574 5f6e 616d 6529 3a0a 2020  er_set_name):.  
+00002e10: 2020 6d65 7468 6f64 5f75 726c 203d 2072    method_url = r
+00002e20: 2273 6574 4368 6174 5374 6963 6b65 7253  "setChatStickerS
+00002e30: 6574 220a 2020 2020 7061 796c 6f61 6420  et".    payload 
+00002e40: 3d20 7b22 6368 6174 5f69 6422 3a20 6368  = {"chat_id": ch
+00002e50: 6174 5f69 642c 2022 7374 6963 6b65 725f  at_id, "sticker_
+00002e60: 7365 745f 6e61 6d65 223a 2073 7469 636b  set_name": stick
+00002e70: 6572 5f73 6574 5f6e 616d 657d 0a20 2020  er_set_name}.   
+00002e80: 2072 6574 7572 6e20 6177 6169 7420 5f72   return await _r
+00002e90: 6571 7565 7374 2874 6f6b 656e 2c20 6d65  equest(token, me
+00002ea0: 7468 6f64 5f75 726c 2c20 7061 7261 6d73  thod_url, params
+00002eb0: 3d70 6179 6c6f 6164 290a 0a0a 6173 796e  =payload)...asyn
+00002ec0: 6320 6465 6620 6465 6c65 7465 5f63 6861  c def delete_cha
+00002ed0: 745f 7374 6963 6b65 725f 7365 7428 746f  t_sticker_set(to
+00002ee0: 6b65 6e2c 2063 6861 745f 6964 293a 0a20  ken, chat_id):. 
+00002ef0: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
+00002f00: 7222 6465 6c65 7465 4368 6174 5374 6963  r"deleteChatStic
+00002f10: 6b65 7253 6574 220a 2020 2020 7061 796c  kerSet".    payl
+00002f20: 6f61 6420 3d20 7b22 6368 6174 5f69 6422  oad = {"chat_id"
+00002f30: 3a20 6368 6174 5f69 647d 0a20 2020 2072  : chat_id}.    r
+00002f40: 6574 7572 6e20 6177 6169 7420 5f72 6571  eturn await _req
+00002f50: 7565 7374 2874 6f6b 656e 2c20 6d65 7468  uest(token, meth
+00002f60: 6f64 5f75 726c 2c20 7061 7261 6d73 3d70  od_url, params=p
+00002f70: 6179 6c6f 6164 290a 0a0a 6173 796e 6320  ayload)...async 
+00002f80: 6465 6620 616e 7377 6572 5f77 6562 5f61  def answer_web_a
+00002f90: 7070 5f71 7565 7279 2874 6f6b 656e 2c20  pp_query(token, 
+00002fa0: 7765 625f 6170 705f 7175 6572 795f 6964  web_app_query_id
+00002fb0: 2c20 7265 7375 6c74 3a20 7479 7065 732e  , result: types.
+00002fc0: 496e 6c69 6e65 5175 6572 7952 6573 756c  InlineQueryResul
+00002fd0: 7442 6173 6529 3a0a 2020 2020 6d65 7468  tBase):.    meth
+00002fe0: 6f64 5f75 726c 203d 2022 616e 7377 6572  od_url = "answer
+00002ff0: 5765 6241 7070 5175 6572 7922 0a20 2020  WebAppQuery".   
+00003000: 2070 6179 6c6f 6164 203d 207b 2277 6562   payload = {"web
+00003010: 5f61 7070 5f71 7565 7279 5f69 6422 3a20  _app_query_id": 
+00003020: 7765 625f 6170 705f 7175 6572 795f 6964  web_app_query_id
+00003030: 2c20 2272 6573 756c 7422 3a20 7265 7375  , "result": resu
+00003040: 6c74 2e74 6f5f 6a73 6f6e 2829 7d0a 2020  lt.to_json()}.  
+00003050: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
+00003060: 7265 7175 6573 7428 746f 6b65 6e2c 206d  request(token, m
+00003070: 6574 686f 645f 7572 6c2c 2070 6172 616d  ethod_url, param
+00003080: 733d 7061 796c 6f61 642c 206d 6574 686f  s=payload, metho
+00003090: 643d 2270 6f73 7422 290a 0a0a 6173 796e  d="post")...asyn
+000030a0: 6320 6465 6620 6765 745f 6368 6174 5f6d  c def get_chat_m
+000030b0: 656d 6265 7228 746f 6b65 6e2c 2063 6861  ember(token, cha
+000030c0: 745f 6964 2c20 7573 6572 5f69 6429 3a0a  t_id, user_id):.
+000030d0: 2020 2020 6d65 7468 6f64 5f75 726c 203d      method_url =
+000030e0: 2072 2267 6574 4368 6174 4d65 6d62 6572   r"getChatMember
+000030f0: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
+00003100: 7b22 6368 6174 5f69 6422 3a20 6368 6174  {"chat_id": chat
+00003110: 5f69 642c 2022 7573 6572 5f69 6422 3a20  _id, "user_id": 
+00003120: 7573 6572 5f69 647d 0a20 2020 2072 6574  user_id}.    ret
+00003130: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
+00003140: 7374 2874 6f6b 656e 2c20 6d65 7468 6f64  st(token, method
+00003150: 5f75 726c 2c20 7061 7261 6d73 3d70 6179  _url, params=pay
+00003160: 6c6f 6164 290a 0a0a 6173 796e 6320 6465  load)...async de
+00003170: 6620 666f 7277 6172 645f 6d65 7373 6167  f forward_messag
+00003180: 6528 0a20 2020 2074 6f6b 656e 2c0a 2020  e(.    token,.  
+00003190: 2020 6368 6174 5f69 642c 0a20 2020 2066    chat_id,.    f
+000031a0: 726f 6d5f 6368 6174 5f69 642c 0a20 2020  rom_chat_id,.   
+000031b0: 206d 6573 7361 6765 5f69 642c 0a20 2020   message_id,.   
+000031c0: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
+000031d0: 6174 696f 6e3d 4e6f 6e65 2c0a 2020 2020  ation=None,.    
+000031e0: 7469 6d65 6f75 743d 4e6f 6e65 2c0a 2020  timeout=None,.  
+000031f0: 2020 7072 6f74 6563 745f 636f 6e74 656e    protect_conten
+00003200: 743d 4e6f 6e65 2c0a 2020 2020 6d65 7373  t=None,.    mess
+00003210: 6167 655f 7468 7265 6164 5f69 643a 204f  age_thread_id: O
+00003220: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00003230: 6f6e 652c 0a29 3a0a 2020 2020 6d65 7468  one,.):.    meth
+00003240: 6f64 5f75 726c 203d 2072 2266 6f72 7761  od_url = r"forwa
+00003250: 7264 4d65 7373 6167 6522 0a20 2020 2070  rdMessage".    p
+00003260: 6179 6c6f 6164 203d 207b 0a20 2020 2020  ayload = {.     
+00003270: 2020 2022 6368 6174 5f69 6422 3a20 6368     "chat_id": ch
+00003280: 6174 5f69 642c 0a20 2020 2020 2020 2022  at_id,.        "
+00003290: 6672 6f6d 5f63 6861 745f 6964 223a 2066  from_chat_id": f
+000032a0: 726f 6d5f 6368 6174 5f69 642c 0a20 2020  rom_chat_id,.   
+000032b0: 2020 2020 2022 6d65 7373 6167 655f 6964       "message_id
+000032c0: 223a 206d 6573 7361 6765 5f69 642c 0a20  ": message_id,. 
+000032d0: 2020 207d 0a20 2020 2069 6620 6469 7361     }.    if disa
+000032e0: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+000032f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00003300: 2020 2020 2020 7061 796c 6f61 645b 2264        payload["d
+00003310: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+00003320: 696f 6e22 5d20 3d20 6469 7361 626c 655f  ion"] = disable_
+00003330: 6e6f 7469 6669 6361 7469 6f6e 0a20 2020  notification.   
+00003340: 2069 6620 7469 6d65 6f75 743a 0a20 2020   if timeout:.   
+00003350: 2020 2020 2070 6179 6c6f 6164 5b22 7469       payload["ti
+00003360: 6d65 6f75 7422 5d20 3d20 7469 6d65 6f75  meout"] = timeou
+00003370: 740a 2020 2020 6966 2070 726f 7465 6374  t.    if protect
+00003380: 5f63 6f6e 7465 6e74 2069 7320 6e6f 7420  _content is not 
+00003390: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
+000033a0: 796c 6f61 645b 2270 726f 7465 6374 5f63  yload["protect_c
+000033b0: 6f6e 7465 6e74 225d 203d 2070 726f 7465  ontent"] = prote
+000033c0: 6374 5f63 6f6e 7465 6e74 0a20 2020 205f  ct_content.    _
+000033d0: 6164 645f 6d65 7373 6167 655f 7468 7265  add_message_thre
+000033e0: 6164 5f69 6428 7061 796c 6f61 642c 206d  ad_id(payload, m
+000033f0: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+00003400: 290a 2020 2020 7265 7475 726e 2061 7761  ).    return awa
+00003410: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
+00003420: 6e2c 206d 6574 686f 645f 7572 6c2c 2070  n, method_url, p
+00003430: 6172 616d 733d 7061 796c 6f61 6429 0a0a  arams=payload)..
+00003440: 0a61 7379 6e63 2064 6566 2063 6f70 795f  .async def copy_
+00003450: 6d65 7373 6167 6528 0a20 2020 2074 6f6b  message(.    tok
+00003460: 656e 2c0a 2020 2020 6368 6174 5f69 642c  en,.    chat_id,
+00003470: 0a20 2020 2066 726f 6d5f 6368 6174 5f69  .    from_chat_i
+00003480: 642c 0a20 2020 206d 6573 7361 6765 5f69  d,.    message_i
+00003490: 642c 0a20 2020 2063 6170 7469 6f6e 3d4e  d,.    caption=N
+000034a0: 6f6e 652c 0a20 2020 2070 6172 7365 5f6d  one,.    parse_m
+000034b0: 6f64 653d 4e6f 6e65 2c0a 2020 2020 6361  ode=None,.    ca
+000034c0: 7074 696f 6e5f 656e 7469 7469 6573 3d4e  ption_entities=N
+000034d0: 6f6e 652c 0a20 2020 2064 6973 6162 6c65  one,.    disable
+000034e0: 5f6e 6f74 6966 6963 6174 696f 6e3d 4e6f  _notification=No
+000034f0: 6e65 2c0a 2020 2020 7265 706c 795f 746f  ne,.    reply_to
+00003500: 5f6d 6573 7361 6765 5f69 643d 4e6f 6e65  _message_id=None
+00003510: 2c0a 2020 2020 616c 6c6f 775f 7365 6e64  ,.    allow_send
+00003520: 696e 675f 7769 7468 6f75 745f 7265 706c  ing_without_repl
+00003530: 793d 4e6f 6e65 2c0a 2020 2020 7265 706c  y=None,.    repl
+00003540: 795f 6d61 726b 7570 3d4e 6f6e 652c 0a20  y_markup=None,. 
+00003550: 2020 2074 696d 656f 7574 3d4e 6f6e 652c     timeout=None,
+00003560: 0a20 2020 2070 726f 7465 6374 5f63 6f6e  .    protect_con
+00003570: 7465 6e74 3d4e 6f6e 652c 0a20 2020 206d  tent=None,.    m
+00003580: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+00003590: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+000035a0: 3d20 4e6f 6e65 2c0a 293a 0a20 2020 206d  = None,.):.    m
+000035b0: 6574 686f 645f 7572 6c20 3d20 7222 636f  ethod_url = r"co
+000035c0: 7079 4d65 7373 6167 6522 0a20 2020 2070  pyMessage".    p
+000035d0: 6179 6c6f 6164 203d 207b 0a20 2020 2020  ayload = {.     
+000035e0: 2020 2022 6368 6174 5f69 6422 3a20 6368     "chat_id": ch
+000035f0: 6174 5f69 642c 0a20 2020 2020 2020 2022  at_id,.        "
+00003600: 6672 6f6d 5f63 6861 745f 6964 223a 2066  from_chat_id": f
+00003610: 726f 6d5f 6368 6174 5f69 642c 0a20 2020  rom_chat_id,.   
+00003620: 2020 2020 2022 6d65 7373 6167 655f 6964       "message_id
+00003630: 223a 206d 6573 7361 6765 5f69 642c 0a20  ": message_id,. 
+00003640: 2020 207d 0a20 2020 2069 6620 6361 7074     }.    if capt
+00003650: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
+00003660: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+00003670: 5b22 6361 7074 696f 6e22 5d20 3d20 6361  ["caption"] = ca
+00003680: 7074 696f 6e0a 2020 2020 6966 2070 6172  ption.    if par
+00003690: 7365 5f6d 6f64 653a 0a20 2020 2020 2020  se_mode:.       
+000036a0: 2070 6179 6c6f 6164 5b22 7061 7273 655f   payload["parse_
+000036b0: 6d6f 6465 225d 203d 2070 6172 7365 5f6d  mode"] = parse_m
+000036c0: 6f64 650a 2020 2020 6966 2063 6170 7469  ode.    if capti
+000036d0: 6f6e 5f65 6e74 6974 6965 7320 6973 206e  on_entities is n
+000036e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000036f0: 2070 6179 6c6f 6164 5b22 6361 7074 696f   payload["captio
+00003700: 6e5f 656e 7469 7469 6573 225d 203d 2061  n_entities"] = a
+00003710: 7761 6974 205f 636f 6e76 6572 745f 656e  wait _convert_en
+00003720: 7469 7465 7328 6361 7074 696f 6e5f 656e  tites(caption_en
+00003730: 7469 7469 6573 290a 2020 2020 6966 2064  tities).    if d
+00003740: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+00003750: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
+00003760: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+00003770: 5b22 6469 7361 626c 655f 6e6f 7469 6669  ["disable_notifi
+00003780: 6361 7469 6f6e 225d 203d 2064 6973 6162  cation"] = disab
+00003790: 6c65 5f6e 6f74 6966 6963 6174 696f 6e0a  le_notification.
+000037a0: 2020 2020 6966 2072 6570 6c79 5f74 6f5f      if reply_to_
+000037b0: 6d65 7373 6167 655f 6964 3a0a 2020 2020  message_id:.    
+000037c0: 2020 2020 7061 796c 6f61 645b 2272 6570      payload["rep
+000037d0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+000037e0: 225d 203d 2072 6570 6c79 5f74 6f5f 6d65  "] = reply_to_me
+000037f0: 7373 6167 655f 6964 0a20 2020 2069 6620  ssage_id.    if 
+00003800: 7265 706c 795f 6d61 726b 7570 2069 7320  reply_markup is 
+00003810: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00003820: 2020 7061 796c 6f61 645b 2272 6570 6c79    payload["reply
+00003830: 5f6d 6172 6b75 7022 5d20 3d20 6177 6169  _markup"] = awai
+00003840: 7420 5f63 6f6e 7665 7274 5f6d 6172 6b75  t _convert_marku
+00003850: 7028 7265 706c 795f 6d61 726b 7570 290a  p(reply_markup).
+00003860: 2020 2020 6966 2061 6c6c 6f77 5f73 656e      if allow_sen
+00003870: 6469 6e67 5f77 6974 686f 7574 5f72 6570  ding_without_rep
+00003880: 6c79 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ly is not None:.
+00003890: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
+000038a0: 2261 6c6c 6f77 5f73 656e 6469 6e67 5f77  "allow_sending_w
+000038b0: 6974 686f 7574 5f72 6570 6c79 225d 203d  ithout_reply"] =
+000038c0: 2061 6c6c 6f77 5f73 656e 6469 6e67 5f77   allow_sending_w
+000038d0: 6974 686f 7574 5f72 6570 6c79 0a20 2020  ithout_reply.   
+000038e0: 2069 6620 7469 6d65 6f75 743a 0a20 2020   if timeout:.   
+000038f0: 2020 2020 2070 6179 6c6f 6164 5b22 7469       payload["ti
+00003900: 6d65 6f75 7422 5d20 3d20 7469 6d65 6f75  meout"] = timeou
+00003910: 740a 2020 2020 6966 2070 726f 7465 6374  t.    if protect
+00003920: 5f63 6f6e 7465 6e74 2069 7320 6e6f 7420  _content is not 
+00003930: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
+00003940: 796c 6f61 645b 2270 726f 7465 6374 5f63  yload["protect_c
+00003950: 6f6e 7465 6e74 225d 203d 2070 726f 7465  ontent"] = prote
+00003960: 6374 5f63 6f6e 7465 6e74 0a20 2020 205f  ct_content.    _
+00003970: 6164 645f 6d65 7373 6167 655f 7468 7265  add_message_thre
+00003980: 6164 5f69 6428 7061 796c 6f61 642c 206d  ad_id(payload, m
+00003990: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+000039a0: 290a 2020 2020 7265 7475 726e 2061 7761  ).    return awa
+000039b0: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
+000039c0: 6e2c 206d 6574 686f 645f 7572 6c2c 2070  n, method_url, p
+000039d0: 6172 616d 733d 7061 796c 6f61 6429 0a0a  arams=payload)..
+000039e0: 0a61 7379 6e63 2064 6566 2073 656e 645f  .async def send_
+000039f0: 6469 6365 280a 2020 2020 746f 6b65 6e2c  dice(.    token,
+00003a00: 0a20 2020 2063 6861 745f 6964 2c0a 2020  .    chat_id,.  
+00003a10: 2020 656d 6f6a 693d 4e6f 6e65 2c0a 2020    emoji=None,.  
+00003a20: 2020 6469 7361 626c 655f 6e6f 7469 6669    disable_notifi
+00003a30: 6361 7469 6f6e 3d4e 6f6e 652c 0a20 2020  cation=None,.   
+00003a40: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
+00003a50: 655f 6964 3d4e 6f6e 652c 0a20 2020 2072  e_id=None,.    r
+00003a60: 6570 6c79 5f6d 6172 6b75 703d 4e6f 6e65  eply_markup=None
+00003a70: 2c0a 2020 2020 7469 6d65 6f75 743d 4e6f  ,.    timeout=No
+00003a80: 6e65 2c0a 2020 2020 616c 6c6f 775f 7365  ne,.    allow_se
+00003a90: 6e64 696e 675f 7769 7468 6f75 745f 7265  nding_without_re
+00003aa0: 706c 793d 4e6f 6e65 2c0a 2020 2020 7072  ply=None,.    pr
+00003ab0: 6f74 6563 745f 636f 6e74 656e 743d 4e6f  otect_content=No
+00003ac0: 6e65 2c0a 2020 2020 6d65 7373 6167 655f  ne,.    message_
+00003ad0: 7468 7265 6164 5f69 643a 204f 7074 696f  thread_id: Optio
+00003ae0: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
+00003af0: 0a29 3a0a 2020 2020 6d65 7468 6f64 5f75  .):.    method_u
+00003b00: 726c 203d 2072 2273 656e 6444 6963 6522  rl = r"sendDice"
+00003b10: 0a20 2020 2070 6179 6c6f 6164 203d 207b  .    payload = {
+00003b20: 2263 6861 745f 6964 223a 2063 6861 745f  "chat_id": chat_
+00003b30: 6964 7d0a 2020 2020 6966 2065 6d6f 6a69  id}.    if emoji
+00003b40: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+00003b50: 645b 2265 6d6f 6a69 225d 203d 2065 6d6f  d["emoji"] = emo
+00003b60: 6a69 0a20 2020 2069 6620 6469 7361 626c  ji.    if disabl
+00003b70: 655f 6e6f 7469 6669 6361 7469 6f6e 2069  e_notification i
+00003b80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00003b90: 2020 2020 7061 796c 6f61 645b 2264 6973      payload["dis
+00003ba0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00003bb0: 6e22 5d20 3d20 6469 7361 626c 655f 6e6f  n"] = disable_no
+00003bc0: 7469 6669 6361 7469 6f6e 0a20 2020 2069  tification.    i
+00003bd0: 6620 7265 706c 795f 746f 5f6d 6573 7361  f reply_to_messa
+00003be0: 6765 5f69 643a 0a20 2020 2020 2020 2070  ge_id:.        p
+00003bf0: 6179 6c6f 6164 5b22 7265 706c 795f 746f  ayload["reply_to
+00003c00: 5f6d 6573 7361 6765 5f69 6422 5d20 3d20  _message_id"] = 
+00003c10: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+00003c20: 5f69 640a 2020 2020 6966 2072 6570 6c79  _id.    if reply
+00003c30: 5f6d 6172 6b75 703a 0a20 2020 2020 2020  _markup:.       
+00003c40: 2070 6179 6c6f 6164 5b22 7265 706c 795f   payload["reply_
+00003c50: 6d61 726b 7570 225d 203d 2061 7761 6974  markup"] = await
+00003c60: 205f 636f 6e76 6572 745f 6d61 726b 7570   _convert_markup
+00003c70: 2872 6570 6c79 5f6d 6172 6b75 7029 0a20  (reply_markup). 
+00003c80: 2020 2069 6620 7469 6d65 6f75 743a 0a20     if timeout:. 
+00003c90: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+00003ca0: 7469 6d65 6f75 7422 5d20 3d20 7469 6d65  timeout"] = time
+00003cb0: 6f75 740a 2020 2020 6966 2061 6c6c 6f77  out.    if allow
+00003cc0: 5f73 656e 6469 6e67 5f77 6974 686f 7574  _sending_without
+00003cd0: 5f72 6570 6c79 2069 7320 6e6f 7420 4e6f  _reply is not No
+00003ce0: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
+00003cf0: 6f61 645b 2261 6c6c 6f77 5f73 656e 6469  oad["allow_sendi
+00003d00: 6e67 5f77 6974 686f 7574 5f72 6570 6c79  ng_without_reply
+00003d10: 225d 203d 2061 6c6c 6f77 5f73 656e 6469  "] = allow_sendi
+00003d20: 6e67 5f77 6974 686f 7574 5f72 6570 6c79  ng_without_reply
+00003d30: 0a20 2020 2069 6620 7072 6f74 6563 745f  .    if protect_
+00003d40: 636f 6e74 656e 7420 6973 206e 6f74 204e  content is not N
+00003d50: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
+00003d60: 6c6f 6164 5b22 7072 6f74 6563 745f 636f  load["protect_co
+00003d70: 6e74 656e 7422 5d20 3d20 7072 6f74 6563  ntent"] = protec
+00003d80: 745f 636f 6e74 656e 740a 2020 2020 5f61  t_content.    _a
+00003d90: 6464 5f6d 6573 7361 6765 5f74 6872 6561  dd_message_threa
+00003da0: 645f 6964 2870 6179 6c6f 6164 2c20 6d65  d_id(payload, me
+00003db0: 7373 6167 655f 7468 7265 6164 5f69 6429  ssage_thread_id)
+00003dc0: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
+00003dd0: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
+00003de0: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
+00003df0: 7261 6d73 3d70 6179 6c6f 6164 290a 0a0a  rams=payload)...
+00003e00: 6173 796e 6320 6465 6620 7365 6e64 5f70  async def send_p
+00003e10: 686f 746f 280a 2020 2020 746f 6b65 6e2c  hoto(.    token,
+00003e20: 0a20 2020 2063 6861 745f 6964 2c0a 2020  .    chat_id,.  
+00003e30: 2020 7068 6f74 6f2c 0a20 2020 2063 6170    photo,.    cap
+00003e40: 7469 6f6e 3d4e 6f6e 652c 0a20 2020 2072  tion=None,.    r
+00003e50: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
+00003e60: 6964 3d4e 6f6e 652c 0a20 2020 2072 6570  id=None,.    rep
+00003e70: 6c79 5f6d 6172 6b75 703d 4e6f 6e65 2c0a  ly_markup=None,.
+00003e80: 2020 2020 7061 7273 655f 6d6f 6465 3d4e      parse_mode=N
+00003e90: 6f6e 652c 0a20 2020 2064 6973 6162 6c65  one,.    disable
+00003ea0: 5f6e 6f74 6966 6963 6174 696f 6e3d 4e6f  _notification=No
+00003eb0: 6e65 2c0a 2020 2020 7469 6d65 6f75 743d  ne,.    timeout=
+00003ec0: 4e6f 6e65 2c0a 2020 2020 6361 7074 696f  None,.    captio
+00003ed0: 6e5f 656e 7469 7469 6573 3d4e 6f6e 652c  n_entities=None,
+00003ee0: 0a20 2020 2061 6c6c 6f77 5f73 656e 6469  .    allow_sendi
+00003ef0: 6e67 5f77 6974 686f 7574 5f72 6570 6c79  ng_without_reply
+00003f00: 3d4e 6f6e 652c 0a20 2020 2070 726f 7465  =None,.    prote
+00003f10: 6374 5f63 6f6e 7465 6e74 3d4e 6f6e 652c  ct_content=None,
+00003f20: 0a20 2020 206d 6573 7361 6765 5f74 6872  .    message_thr
+00003f30: 6561 645f 6964 3a20 4f70 7469 6f6e 616c  ead_id: Optional
+00003f40: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
+00003f50: 2020 6861 735f 7370 6f69 6c65 723a 204f    has_spoiler: O
+00003f60: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00003f70: 4e6f 6e65 2c0a 293a 0a20 2020 206d 6574  None,.):.    met
+00003f80: 686f 645f 7572 6c20 3d20 7222 7365 6e64  hod_url = r"send
+00003f90: 5068 6f74 6f22 0a20 2020 2070 6179 6c6f  Photo".    paylo
+00003fa0: 6164 203d 207b 2263 6861 745f 6964 223a  ad = {"chat_id":
+00003fb0: 2063 6861 745f 6964 7d0a 2020 2020 6669   chat_id}.    fi
+00003fc0: 6c65 7320 3d20 4e6f 6e65 0a20 2020 2069  les = None.    i
+00003fd0: 6620 7574 696c 2e69 735f 7374 7269 6e67  f util.is_string
+00003fe0: 2870 686f 746f 293a 0a20 2020 2020 2020  (photo):.       
+00003ff0: 2070 6179 6c6f 6164 5b22 7068 6f74 6f22   payload["photo"
+00004000: 5d20 3d20 7068 6f74 6f0a 2020 2020 656c  ] = photo.    el
+00004010: 7365 3a0a 2020 2020 2020 2020 6669 6c65  se:.        file
+00004020: 7320 3d20 7b22 7068 6f74 6f22 3a20 7068  s = {"photo": ph
+00004030: 6f74 6f7d 0a20 2020 2069 6620 6361 7074  oto}.    if capt
+00004040: 696f 6e3a 0a20 2020 2020 2020 2070 6179  ion:.        pay
+00004050: 6c6f 6164 5b22 6361 7074 696f 6e22 5d20  load["caption"] 
+00004060: 3d20 6361 7074 696f 6e0a 2020 2020 6966  = caption.    if
+00004070: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
+00004080: 655f 6964 3a0a 2020 2020 2020 2020 7061  e_id:.        pa
+00004090: 796c 6f61 645b 2272 6570 6c79 5f74 6f5f  yload["reply_to_
+000040a0: 6d65 7373 6167 655f 6964 225d 203d 2072  message_id"] = r
+000040b0: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
+000040c0: 6964 0a20 2020 2069 6620 7265 706c 795f  id.    if reply_
+000040d0: 6d61 726b 7570 3a0a 2020 2020 2020 2020  markup:.        
+000040e0: 7061 796c 6f61 645b 2272 6570 6c79 5f6d  payload["reply_m
+000040f0: 6172 6b75 7022 5d20 3d20 6177 6169 7420  arkup"] = await 
+00004100: 5f63 6f6e 7665 7274 5f6d 6172 6b75 7028  _convert_markup(
+00004110: 7265 706c 795f 6d61 726b 7570 290a 2020  reply_markup).  
+00004120: 2020 6966 2070 6172 7365 5f6d 6f64 653a    if parse_mode:
+00004130: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+00004140: 5b22 7061 7273 655f 6d6f 6465 225d 203d  ["parse_mode"] =
+00004150: 2070 6172 7365 5f6d 6f64 650a 2020 2020   parse_mode.    
+00004160: 6966 2064 6973 6162 6c65 5f6e 6f74 6966  if disable_notif
+00004170: 6963 6174 696f 6e20 6973 206e 6f74 204e  ication is not N
+00004180: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
+00004190: 6c6f 6164 5b22 6469 7361 626c 655f 6e6f  load["disable_no
+000041a0: 7469 6669 6361 7469 6f6e 225d 203d 2064  tification"] = d
+000041b0: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+000041c0: 696f 6e0a 2020 2020 6966 2074 696d 656f  ion.    if timeo
+000041d0: 7574 3a0a 2020 2020 2020 2020 7061 796c  ut:.        payl
+000041e0: 6f61 645b 2274 696d 656f 7574 225d 203d  oad["timeout"] =
+000041f0: 2074 696d 656f 7574 0a20 2020 2069 6620   timeout.    if 
+00004200: 6361 7074 696f 6e5f 656e 7469 7469 6573  caption_entities
+00004210: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+00004220: 645b 2263 6170 7469 6f6e 5f65 6e74 6974  d["caption_entit
+00004230: 6965 7322 5d20 3d20 6a73 6f6e 2e64 756d  ies"] = json.dum
+00004240: 7073 2874 7970 6573 2e4d 6573 7361 6765  ps(types.Message
+00004250: 456e 7469 7479 2e74 6f5f 6c69 7374 5f6f  Entity.to_list_o
+00004260: 665f 6469 6374 7328 6361 7074 696f 6e5f  f_dicts(caption_
+00004270: 656e 7469 7469 6573 2929 0a20 2020 2069  entities)).    i
+00004280: 6620 616c 6c6f 775f 7365 6e64 696e 675f  f allow_sending_
+00004290: 7769 7468 6f75 745f 7265 706c 7920 6973  without_reply is
+000042a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000042b0: 2020 2070 6179 6c6f 6164 5b22 616c 6c6f     payload["allo
+000042c0: 775f 7365 6e64 696e 675f 7769 7468 6f75  w_sending_withou
+000042d0: 745f 7265 706c 7922 5d20 3d20 616c 6c6f  t_reply"] = allo
+000042e0: 775f 7365 6e64 696e 675f 7769 7468 6f75  w_sending_withou
+000042f0: 745f 7265 706c 790a 2020 2020 6966 2070  t_reply.    if p
+00004300: 726f 7465 6374 5f63 6f6e 7465 6e74 2069  rotect_content i
+00004310: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00004320: 2020 2020 7061 796c 6f61 645b 2270 726f      payload["pro
+00004330: 7465 6374 5f63 6f6e 7465 6e74 225d 203d  tect_content"] =
+00004340: 2070 726f 7465 6374 5f63 6f6e 7465 6e74   protect_content
+00004350: 0a20 2020 205f 6164 645f 6d65 7373 6167  .    _add_messag
+00004360: 655f 7468 7265 6164 5f69 6428 7061 796c  e_thread_id(payl
+00004370: 6f61 642c 206d 6573 7361 6765 5f74 6872  oad, message_thr
+00004380: 6561 645f 6964 290a 2020 2020 6966 2068  ead_id).    if h
+00004390: 6173 5f73 706f 696c 6572 2069 7320 6e6f  as_spoiler is no
+000043a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000043b0: 7061 796c 6f61 645b 2268 6173 5f73 706f  payload["has_spo
+000043c0: 696c 6572 225d 203d 2068 6173 5f73 706f  iler"] = has_spo
+000043d0: 696c 6572 0a20 2020 2072 6574 7572 6e20  iler.    return 
+000043e0: 6177 6169 7420 5f72 6571 7565 7374 2874  await _request(t
+000043f0: 6f6b 656e 2c20 6d65 7468 6f64 5f75 726c  oken, method_url
+00004400: 2c20 7061 7261 6d73 3d70 6179 6c6f 6164  , params=payload
+00004410: 2c20 6669 6c65 733d 6669 6c65 732c 206d  , files=files, m
+00004420: 6574 686f 643d 2270 6f73 7422 290a 0a0a  ethod="post")...
+00004430: 6173 796e 6320 6465 6620 7365 6e64 5f6d  async def send_m
+00004440: 6564 6961 5f67 726f 7570 280a 2020 2020  edia_group(.    
+00004450: 746f 6b65 6e2c 0a20 2020 2063 6861 745f  token,.    chat_
+00004460: 6964 2c0a 2020 2020 6d65 6469 612c 0a20  id,.    media,. 
+00004470: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
+00004480: 6963 6174 696f 6e3d 4e6f 6e65 2c0a 2020  ication=None,.  
+00004490: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
+000044a0: 6765 5f69 643d 4e6f 6e65 2c0a 2020 2020  ge_id=None,.    
+000044b0: 7469 6d65 6f75 743d 4e6f 6e65 2c0a 2020  timeout=None,.  
+000044c0: 2020 616c 6c6f 775f 7365 6e64 696e 675f    allow_sending_
+000044d0: 7769 7468 6f75 745f 7265 706c 793d 4e6f  without_reply=No
+000044e0: 6e65 2c0a 2020 2020 7072 6f74 6563 745f  ne,.    protect_
+000044f0: 636f 6e74 656e 743d 4e6f 6e65 2c0a 2020  content=None,.  
+00004500: 2020 6d65 7373 6167 655f 7468 7265 6164    message_thread
+00004510: 5f69 643a 204f 7074 696f 6e61 6c5b 696e  _id: Optional[in
+00004520: 745d 203d 204e 6f6e 652c 0a29 3a0a 2020  t] = None,.):.  
+00004530: 2020 6d65 7468 6f64 5f75 726c 203d 2072    method_url = r
+00004540: 2273 656e 644d 6564 6961 4772 6f75 7022  "sendMediaGroup"
+00004550: 0a20 2020 206d 6564 6961 5f6a 736f 6e2c  .    media_json,
+00004560: 2066 696c 6573 203d 2061 7761 6974 2063   files = await c
+00004570: 6f6e 7665 7274 5f69 6e70 7574 5f6d 6564  onvert_input_med
+00004580: 6961 5f61 7272 6179 286d 6564 6961 290a  ia_array(media).
+00004590: 2020 2020 7061 796c 6f61 6420 3d20 7b22      payload = {"
+000045a0: 6368 6174 5f69 6422 3a20 6368 6174 5f69  chat_id": chat_i
+000045b0: 642c 2022 6d65 6469 6122 3a20 6d65 6469  d, "media": medi
+000045c0: 615f 6a73 6f6e 7d0a 2020 2020 6966 2064  a_json}.    if d
+000045d0: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+000045e0: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
+000045f0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+00004600: 5b22 6469 7361 626c 655f 6e6f 7469 6669  ["disable_notifi
+00004610: 6361 7469 6f6e 225d 203d 2064 6973 6162  cation"] = disab
+00004620: 6c65 5f6e 6f74 6966 6963 6174 696f 6e0a  le_notification.
+00004630: 2020 2020 6966 2072 6570 6c79 5f74 6f5f      if reply_to_
+00004640: 6d65 7373 6167 655f 6964 3a0a 2020 2020  message_id:.    
+00004650: 2020 2020 7061 796c 6f61 645b 2272 6570      payload["rep
+00004660: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+00004670: 225d 203d 2072 6570 6c79 5f74 6f5f 6d65  "] = reply_to_me
+00004680: 7373 6167 655f 6964 0a20 2020 2069 6620  ssage_id.    if 
+00004690: 7469 6d65 6f75 743a 0a20 2020 2020 2020  timeout:.       
+000046a0: 2070 6179 6c6f 6164 5b22 7469 6d65 6f75   payload["timeou
+000046b0: 7422 5d20 3d20 7469 6d65 6f75 740a 2020  t"] = timeout.  
+000046c0: 2020 6966 2061 6c6c 6f77 5f73 656e 6469    if allow_sendi
+000046d0: 6e67 5f77 6974 686f 7574 5f72 6570 6c79  ng_without_reply
+000046e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000046f0: 2020 2020 2020 7061 796c 6f61 645b 2261        payload["a
+00004700: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
+00004710: 686f 7574 5f72 6570 6c79 225d 203d 2061  hout_reply"] = a
+00004720: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
+00004730: 686f 7574 5f72 6570 6c79 0a20 2020 2069  hout_reply.    i
+00004740: 6620 7072 6f74 6563 745f 636f 6e74 656e  f protect_conten
+00004750: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
+00004760: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+00004770: 7072 6f74 6563 745f 636f 6e74 656e 7422  protect_content"
+00004780: 5d20 3d20 7072 6f74 6563 745f 636f 6e74  ] = protect_cont
+00004790: 656e 740a 2020 2020 5f61 6464 5f6d 6573  ent.    _add_mes
+000047a0: 7361 6765 5f74 6872 6561 645f 6964 2870  sage_thread_id(p
+000047b0: 6179 6c6f 6164 2c20 6d65 7373 6167 655f  ayload, message_
+000047c0: 7468 7265 6164 5f69 6429 0a20 2020 2072  thread_id).    r
+000047d0: 6574 7572 6e20 6177 6169 7420 5f72 6571  eturn await _req
+000047e0: 7565 7374 280a 2020 2020 2020 2020 746f  uest(.        to
+000047f0: 6b65 6e2c 0a20 2020 2020 2020 206d 6574  ken,.        met
+00004800: 686f 645f 7572 6c2c 0a20 2020 2020 2020  hod_url,.       
+00004810: 2070 6172 616d 733d 7061 796c 6f61 642c   params=payload,
+00004820: 0a20 2020 2020 2020 206d 6574 686f 643d  .        method=
+00004830: 2270 6f73 7422 2069 6620 6669 6c65 7320  "post" if files 
+00004840: 656c 7365 2022 6765 7422 2c0a 2020 2020  else "get",.    
+00004850: 2020 2020 6669 6c65 733d 6669 6c65 7320      files=files 
+00004860: 6966 2066 696c 6573 2065 6c73 6520 4e6f  if files else No
+00004870: 6e65 2c0a 2020 2020 290a 0a0a 6173 796e  ne,.    )...asyn
+00004880: 6320 6465 6620 7365 6e64 5f6c 6f63 6174  c def send_locat
+00004890: 696f 6e28 0a20 2020 2074 6f6b 656e 2c0a  ion(.    token,.
+000048a0: 2020 2020 6368 6174 5f69 642c 0a20 2020      chat_id,.   
+000048b0: 206c 6174 6974 7564 652c 0a20 2020 206c   latitude,.    l
+000048c0: 6f6e 6769 7475 6465 2c0a 2020 2020 6c69  ongitude,.    li
+000048d0: 7665 5f70 6572 696f 643d 4e6f 6e65 2c0a  ve_period=None,.
+000048e0: 2020 2020 7265 706c 795f 746f 5f6d 6573      reply_to_mes
+000048f0: 7361 6765 5f69 643d 4e6f 6e65 2c0a 2020  sage_id=None,.  
+00004900: 2020 7265 706c 795f 6d61 726b 7570 3d4e    reply_markup=N
+00004910: 6f6e 652c 0a20 2020 2064 6973 6162 6c65  one,.    disable
+00004920: 5f6e 6f74 6966 6963 6174 696f 6e3d 4e6f  _notification=No
+00004930: 6e65 2c0a 2020 2020 7469 6d65 6f75 743d  ne,.    timeout=
+00004940: 4e6f 6e65 2c0a 2020 2020 686f 7269 7a6f  None,.    horizo
+00004950: 6e74 616c 5f61 6363 7572 6163 793d 4e6f  ntal_accuracy=No
+00004960: 6e65 2c0a 2020 2020 6865 6164 696e 673d  ne,.    heading=
+00004970: 4e6f 6e65 2c0a 2020 2020 7072 6f78 696d  None,.    proxim
+00004980: 6974 795f 616c 6572 745f 7261 6469 7573  ity_alert_radius
+00004990: 3d4e 6f6e 652c 0a20 2020 2061 6c6c 6f77  =None,.    allow
+000049a0: 5f73 656e 6469 6e67 5f77 6974 686f 7574  _sending_without
+000049b0: 5f72 6570 6c79 3d4e 6f6e 652c 0a20 2020  _reply=None,.   
+000049c0: 2070 726f 7465 6374 5f63 6f6e 7465 6e74   protect_content
+000049d0: 3d4e 6f6e 652c 0a20 2020 206d 6573 7361  =None,.    messa
+000049e0: 6765 5f74 6872 6561 645f 6964 3a20 4f70  ge_thread_id: Op
+000049f0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00004a00: 6e65 2c0a 293a 0a20 2020 206d 6574 686f  ne,.):.    metho
+00004a10: 645f 7572 6c20 3d20 7222 7365 6e64 4c6f  d_url = r"sendLo
+00004a20: 6361 7469 6f6e 220a 2020 2020 7061 796c  cation".    payl
+00004a30: 6f61 6420 3d20 7b22 6368 6174 5f69 6422  oad = {"chat_id"
+00004a40: 3a20 6368 6174 5f69 642c 2022 6c61 7469  : chat_id, "lati
+00004a50: 7475 6465 223a 206c 6174 6974 7564 652c  tude": latitude,
+00004a60: 2022 6c6f 6e67 6974 7564 6522 3a20 6c6f   "longitude": lo
+00004a70: 6e67 6974 7564 657d 0a20 2020 2069 6620  ngitude}.    if 
+00004a80: 6c69 7665 5f70 6572 696f 643a 0a20 2020  live_period:.   
+00004a90: 2020 2020 2070 6179 6c6f 6164 5b22 6c69       payload["li
+00004aa0: 7665 5f70 6572 696f 6422 5d20 3d20 6c69  ve_period"] = li
+00004ab0: 7665 5f70 6572 696f 640a 2020 2020 6966  ve_period.    if
+00004ac0: 2068 6f72 697a 6f6e 7461 6c5f 6163 6375   horizontal_accu
+00004ad0: 7261 6379 3a0a 2020 2020 2020 2020 7061  racy:.        pa
+00004ae0: 796c 6f61 645b 2268 6f72 697a 6f6e 7461  yload["horizonta
+00004af0: 6c5f 6163 6375 7261 6379 225d 203d 2068  l_accuracy"] = h
+00004b00: 6f72 697a 6f6e 7461 6c5f 6163 6375 7261  orizontal_accura
+00004b10: 6379 0a20 2020 2069 6620 6865 6164 696e  cy.    if headin
+00004b20: 673a 0a20 2020 2020 2020 2070 6179 6c6f  g:.        paylo
+00004b30: 6164 5b22 6865 6164 696e 6722 5d20 3d20  ad["heading"] = 
+00004b40: 6865 6164 696e 670a 2020 2020 6966 2070  heading.    if p
+00004b50: 726f 7869 6d69 7479 5f61 6c65 7274 5f72  roximity_alert_r
+00004b60: 6164 6975 733a 0a20 2020 2020 2020 2070  adius:.        p
+00004b70: 6179 6c6f 6164 5b22 7072 6f78 696d 6974  ayload["proximit
+00004b80: 795f 616c 6572 745f 7261 6469 7573 225d  y_alert_radius"]
+00004b90: 203d 2070 726f 7869 6d69 7479 5f61 6c65   = proximity_ale
+00004ba0: 7274 5f72 6164 6975 730a 2020 2020 6966  rt_radius.    if
+00004bb0: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
+00004bc0: 655f 6964 3a0a 2020 2020 2020 2020 7061  e_id:.        pa
+00004bd0: 796c 6f61 645b 2272 6570 6c79 5f74 6f5f  yload["reply_to_
+00004be0: 6d65 7373 6167 655f 6964 225d 203d 2072  message_id"] = r
+00004bf0: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
+00004c00: 6964 0a20 2020 2069 6620 616c 6c6f 775f  id.    if allow_
+00004c10: 7365 6e64 696e 675f 7769 7468 6f75 745f  sending_without_
+00004c20: 7265 706c 7920 6973 206e 6f74 204e 6f6e  reply is not Non
+00004c30: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
+00004c40: 6164 5b22 616c 6c6f 775f 7365 6e64 696e  ad["allow_sendin
+00004c50: 675f 7769 7468 6f75 745f 7265 706c 7922  g_without_reply"
+00004c60: 5d20 3d20 616c 6c6f 775f 7365 6e64 696e  ] = allow_sendin
+00004c70: 675f 7769 7468 6f75 745f 7265 706c 790a  g_without_reply.
+00004c80: 2020 2020 6966 2072 6570 6c79 5f6d 6172      if reply_mar
+00004c90: 6b75 703a 0a20 2020 2020 2020 2070 6179  kup:.        pay
+00004ca0: 6c6f 6164 5b22 7265 706c 795f 6d61 726b  load["reply_mark
+00004cb0: 7570 225d 203d 2061 7761 6974 205f 636f  up"] = await _co
+00004cc0: 6e76 6572 745f 6d61 726b 7570 2872 6570  nvert_markup(rep
+00004cd0: 6c79 5f6d 6172 6b75 7029 0a20 2020 2069  ly_markup).    i
+00004ce0: 6620 6469 7361 626c 655f 6e6f 7469 6669  f disable_notifi
+00004cf0: 6361 7469 6f6e 2069 7320 6e6f 7420 4e6f  cation is not No
+00004d00: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
+00004d10: 6f61 645b 2264 6973 6162 6c65 5f6e 6f74  oad["disable_not
+00004d20: 6966 6963 6174 696f 6e22 5d20 3d20 6469  ification"] = di
+00004d30: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+00004d40: 6f6e 0a20 2020 2069 6620 7469 6d65 6f75  on.    if timeou
+00004d50: 743a 0a20 2020 2020 2020 2070 6179 6c6f  t:.        paylo
+00004d60: 6164 5b22 7469 6d65 6f75 7422 5d20 3d20  ad["timeout"] = 
+00004d70: 7469 6d65 6f75 740a 2020 2020 6966 2070  timeout.    if p
+00004d80: 726f 7465 6374 5f63 6f6e 7465 6e74 2069  rotect_content i
+00004d90: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00004da0: 2020 2020 7061 796c 6f61 645b 2270 726f      payload["pro
+00004db0: 7465 6374 5f63 6f6e 7465 6e74 225d 203d  tect_content"] =
+00004dc0: 2070 726f 7465 6374 5f63 6f6e 7465 6e74   protect_content
+00004dd0: 0a20 2020 205f 6164 645f 6d65 7373 6167  .    _add_messag
+00004de0: 655f 7468 7265 6164 5f69 6428 7061 796c  e_thread_id(payl
+00004df0: 6f61 642c 206d 6573 7361 6765 5f74 6872  oad, message_thr
+00004e00: 6561 645f 6964 290a 2020 2020 7265 7475  ead_id).    retu
+00004e10: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
+00004e20: 7428 746f 6b65 6e2c 206d 6574 686f 645f  t(token, method_
+00004e30: 7572 6c2c 2070 6172 616d 733d 7061 796c  url, params=payl
+00004e40: 6f61 6429 0a0a 0a61 7379 6e63 2064 6566  oad)...async def
+00004e50: 2065 6469 745f 6d65 7373 6167 655f 6c69   edit_message_li
+00004e60: 7665 5f6c 6f63 6174 696f 6e28 0a20 2020  ve_location(.   
+00004e70: 2074 6f6b 656e 2c0a 2020 2020 6c61 7469   token,.    lati
+00004e80: 7475 6465 2c0a 2020 2020 6c6f 6e67 6974  tude,.    longit
+00004e90: 7564 652c 0a20 2020 2063 6861 745f 6964  ude,.    chat_id
+00004ea0: 3d4e 6f6e 652c 0a20 2020 206d 6573 7361  =None,.    messa
+00004eb0: 6765 5f69 643d 4e6f 6e65 2c0a 2020 2020  ge_id=None,.    
+00004ec0: 696e 6c69 6e65 5f6d 6573 7361 6765 5f69  inline_message_i
+00004ed0: 643d 4e6f 6e65 2c0a 2020 2020 7265 706c  d=None,.    repl
+00004ee0: 795f 6d61 726b 7570 3d4e 6f6e 652c 0a20  y_markup=None,. 
+00004ef0: 2020 2074 696d 656f 7574 3d4e 6f6e 652c     timeout=None,
+00004f00: 0a20 2020 2068 6f72 697a 6f6e 7461 6c5f  .    horizontal_
+00004f10: 6163 6375 7261 6379 3d4e 6f6e 652c 0a20  accuracy=None,. 
+00004f20: 2020 2068 6561 6469 6e67 3d4e 6f6e 652c     heading=None,
+00004f30: 0a20 2020 2070 726f 7869 6d69 7479 5f61  .    proximity_a
+00004f40: 6c65 7274 5f72 6164 6975 733d 4e6f 6e65  lert_radius=None
+00004f50: 2c0a 293a 0a20 2020 206d 6574 686f 645f  ,.):.    method_
+00004f60: 7572 6c20 3d20 7222 6564 6974 4d65 7373  url = r"editMess
+00004f70: 6167 654c 6976 654c 6f63 6174 696f 6e22  ageLiveLocation"
+00004f80: 0a20 2020 2070 6179 6c6f 6164 203d 207b  .    payload = {
+00004f90: 226c 6174 6974 7564 6522 3a20 6c61 7469  "latitude": lati
+00004fa0: 7475 6465 2c20 226c 6f6e 6769 7475 6465  tude, "longitude
+00004fb0: 223a 206c 6f6e 6769 7475 6465 7d0a 2020  ": longitude}.  
+00004fc0: 2020 6966 2063 6861 745f 6964 3a0a 2020    if chat_id:.  
+00004fd0: 2020 2020 2020 7061 796c 6f61 645b 2263        payload["c
+00004fe0: 6861 745f 6964 225d 203d 2063 6861 745f  hat_id"] = chat_
+00004ff0: 6964 0a20 2020 2069 6620 6d65 7373 6167  id.    if messag
+00005000: 655f 6964 3a0a 2020 2020 2020 2020 7061  e_id:.        pa
+00005010: 796c 6f61 645b 226d 6573 7361 6765 5f69  yload["message_i
+00005020: 6422 5d20 3d20 6d65 7373 6167 655f 6964  d"] = message_id
+00005030: 0a20 2020 2069 6620 686f 7269 7a6f 6e74  .    if horizont
+00005040: 616c 5f61 6363 7572 6163 793a 0a20 2020  al_accuracy:.   
+00005050: 2020 2020 2070 6179 6c6f 6164 5b22 686f       payload["ho
+00005060: 7269 7a6f 6e74 616c 5f61 6363 7572 6163  rizontal_accurac
+00005070: 7922 5d20 3d20 686f 7269 7a6f 6e74 616c  y"] = horizontal
+00005080: 5f61 6363 7572 6163 790a 2020 2020 6966  _accuracy.    if
+00005090: 2068 6561 6469 6e67 3a0a 2020 2020 2020   heading:.      
+000050a0: 2020 7061 796c 6f61 645b 2268 6561 6469    payload["headi
+000050b0: 6e67 225d 203d 2068 6561 6469 6e67 0a20  ng"] = heading. 
+000050c0: 2020 2069 6620 7072 6f78 696d 6974 795f     if proximity_
+000050d0: 616c 6572 745f 7261 6469 7573 3a0a 2020  alert_radius:.  
+000050e0: 2020 2020 2020 7061 796c 6f61 645b 2270        payload["p
+000050f0: 726f 7869 6d69 7479 5f61 6c65 7274 5f72  roximity_alert_r
+00005100: 6164 6975 7322 5d20 3d20 7072 6f78 696d  adius"] = proxim
+00005110: 6974 795f 616c 6572 745f 7261 6469 7573  ity_alert_radius
+00005120: 0a20 2020 2069 6620 696e 6c69 6e65 5f6d  .    if inline_m
+00005130: 6573 7361 6765 5f69 643a 0a20 2020 2020  essage_id:.     
+00005140: 2020 2070 6179 6c6f 6164 5b22 696e 6c69     payload["inli
+00005150: 6e65 5f6d 6573 7361 6765 5f69 6422 5d20  ne_message_id"] 
+00005160: 3d20 696e 6c69 6e65 5f6d 6573 7361 6765  = inline_message
+00005170: 5f69 640a 2020 2020 6966 2072 6570 6c79  _id.    if reply
+00005180: 5f6d 6172 6b75 703a 0a20 2020 2020 2020  _markup:.       
+00005190: 2070 6179 6c6f 6164 5b22 7265 706c 795f   payload["reply_
+000051a0: 6d61 726b 7570 225d 203d 2061 7761 6974  markup"] = await
+000051b0: 205f 636f 6e76 6572 745f 6d61 726b 7570   _convert_markup
+000051c0: 2872 6570 6c79 5f6d 6172 6b75 7029 0a20  (reply_markup). 
+000051d0: 2020 2069 6620 7469 6d65 6f75 743a 0a20     if timeout:. 
+000051e0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+000051f0: 7469 6d65 6f75 7422 5d20 3d20 7469 6d65  timeout"] = time
+00005200: 6f75 740a 2020 2020 7265 7475 726e 2061  out.    return a
+00005210: 7761 6974 205f 7265 7175 6573 7428 746f  wait _request(to
+00005220: 6b65 6e2c 206d 6574 686f 645f 7572 6c2c  ken, method_url,
+00005230: 2070 6172 616d 733d 7061 796c 6f61 6429   params=payload)
+00005240: 0a0a 0a61 7379 6e63 2064 6566 2073 746f  ...async def sto
+00005250: 705f 6d65 7373 6167 655f 6c69 7665 5f6c  p_message_live_l
+00005260: 6f63 6174 696f 6e28 0a20 2020 2074 6f6b  ocation(.    tok
+00005270: 656e 2c0a 2020 2020 6368 6174 5f69 643d  en,.    chat_id=
+00005280: 4e6f 6e65 2c0a 2020 2020 6d65 7373 6167  None,.    messag
+00005290: 655f 6964 3d4e 6f6e 652c 0a20 2020 2069  e_id=None,.    i
+000052a0: 6e6c 696e 655f 6d65 7373 6167 655f 6964  nline_message_id
+000052b0: 3d4e 6f6e 652c 0a20 2020 2072 6570 6c79  =None,.    reply
+000052c0: 5f6d 6172 6b75 703d 4e6f 6e65 2c0a 2020  _markup=None,.  
+000052d0: 2020 7469 6d65 6f75 743d 4e6f 6e65 2c0a    timeout=None,.
+000052e0: 293a 0a20 2020 206d 6574 686f 645f 7572  ):.    method_ur
+000052f0: 6c20 3d20 7222 7374 6f70 4d65 7373 6167  l = r"stopMessag
+00005300: 654c 6976 654c 6f63 6174 696f 6e22 0a20  eLiveLocation". 
+00005310: 2020 2070 6179 6c6f 6164 203d 207b 7d0a     payload = {}.
+00005320: 2020 2020 6966 2063 6861 745f 6964 3a0a      if chat_id:.
+00005330: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
+00005340: 2263 6861 745f 6964 225d 203d 2063 6861  "chat_id"] = cha
+00005350: 745f 6964 0a20 2020 2069 6620 6d65 7373  t_id.    if mess
+00005360: 6167 655f 6964 3a0a 2020 2020 2020 2020  age_id:.        
+00005370: 7061 796c 6f61 645b 226d 6573 7361 6765  payload["message
+00005380: 5f69 6422 5d20 3d20 6d65 7373 6167 655f  _id"] = message_
+00005390: 6964 0a20 2020 2069 6620 696e 6c69 6e65  id.    if inline
+000053a0: 5f6d 6573 7361 6765 5f69 643a 0a20 2020  _message_id:.   
+000053b0: 2020 2020 2070 6179 6c6f 6164 5b22 696e       payload["in
+000053c0: 6c69 6e65 5f6d 6573 7361 6765 5f69 6422  line_message_id"
+000053d0: 5d20 3d20 696e 6c69 6e65 5f6d 6573 7361  ] = inline_messa
+000053e0: 6765 5f69 640a 2020 2020 6966 2072 6570  ge_id.    if rep
+000053f0: 6c79 5f6d 6172 6b75 703a 0a20 2020 2020  ly_markup:.     
+00005400: 2020 2070 6179 6c6f 6164 5b22 7265 706c     payload["repl
+00005410: 795f 6d61 726b 7570 225d 203d 2061 7761  y_markup"] = awa
+00005420: 6974 205f 636f 6e76 6572 745f 6d61 726b  it _convert_mark
+00005430: 7570 2872 6570 6c79 5f6d 6172 6b75 7029  up(reply_markup)
+00005440: 0a20 2020 2069 6620 7469 6d65 6f75 743a  .    if timeout:
+00005450: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+00005460: 5b22 7469 6d65 6f75 7422 5d20 3d20 7469  ["timeout"] = ti
+00005470: 6d65 6f75 740a 2020 2020 7265 7475 726e  meout.    return
+00005480: 2061 7761 6974 205f 7265 7175 6573 7428   await _request(
+00005490: 746f 6b65 6e2c 206d 6574 686f 645f 7572  token, method_ur
+000054a0: 6c2c 2070 6172 616d 733d 7061 796c 6f61  l, params=payloa
+000054b0: 6429 0a0a 0a61 7379 6e63 2064 6566 2073  d)...async def s
+000054c0: 656e 645f 7665 6e75 6528 0a20 2020 2074  end_venue(.    t
+000054d0: 6f6b 656e 2c0a 2020 2020 6368 6174 5f69  oken,.    chat_i
+000054e0: 642c 0a20 2020 206c 6174 6974 7564 652c  d,.    latitude,
+000054f0: 0a20 2020 206c 6f6e 6769 7475 6465 2c0a  .    longitude,.
+00005500: 2020 2020 7469 746c 652c 0a20 2020 2061      title,.    a
+00005510: 6464 7265 7373 2c0a 2020 2020 666f 7572  ddress,.    four
+00005520: 7371 7561 7265 5f69 643d 4e6f 6e65 2c0a  square_id=None,.
+00005530: 2020 2020 666f 7572 7371 7561 7265 5f74      foursquare_t
+00005540: 7970 653d 4e6f 6e65 2c0a 2020 2020 6469  ype=None,.    di
+00005550: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+00005560: 6f6e 3d4e 6f6e 652c 0a20 2020 2072 6570  on=None,.    rep
+00005570: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+00005580: 3d4e 6f6e 652c 0a20 2020 2072 6570 6c79  =None,.    reply
+00005590: 5f6d 6172 6b75 703d 4e6f 6e65 2c0a 2020  _markup=None,.  
+000055a0: 2020 7469 6d65 6f75 743d 4e6f 6e65 2c0a    timeout=None,.
+000055b0: 2020 2020 616c 6c6f 775f 7365 6e64 696e      allow_sendin
+000055c0: 675f 7769 7468 6f75 745f 7265 706c 793d  g_without_reply=
+000055d0: 4e6f 6e65 2c0a 2020 2020 676f 6f67 6c65  None,.    google
+000055e0: 5f70 6c61 6365 5f69 643d 4e6f 6e65 2c0a  _place_id=None,.
+000055f0: 2020 2020 676f 6f67 6c65 5f70 6c61 6365      google_place
+00005600: 5f74 7970 653d 4e6f 6e65 2c0a 2020 2020  _type=None,.    
+00005610: 7072 6f74 6563 745f 636f 6e74 656e 743d  protect_content=
+00005620: 4e6f 6e65 2c0a 2020 2020 6d65 7373 6167  None,.    messag
+00005630: 655f 7468 7265 6164 5f69 643a 204f 7074  e_thread_id: Opt
+00005640: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00005650: 652c 0a29 3a0a 2020 2020 6d65 7468 6f64  e,.):.    method
+00005660: 5f75 726c 203d 2072 2273 656e 6456 656e  _url = r"sendVen
+00005670: 7565 220a 2020 2020 7061 796c 6f61 6420  ue".    payload 
+00005680: 3d20 7b0a 2020 2020 2020 2020 2263 6861  = {.        "cha
+00005690: 745f 6964 223a 2063 6861 745f 6964 2c0a  t_id": chat_id,.
+000056a0: 2020 2020 2020 2020 226c 6174 6974 7564          "latitud
+000056b0: 6522 3a20 6c61 7469 7475 6465 2c0a 2020  e": latitude,.  
+000056c0: 2020 2020 2020 226c 6f6e 6769 7475 6465        "longitude
+000056d0: 223a 206c 6f6e 6769 7475 6465 2c0a 2020  ": longitude,.  
+000056e0: 2020 2020 2020 2274 6974 6c65 223a 2074        "title": t
+000056f0: 6974 6c65 2c0a 2020 2020 2020 2020 2261  itle,.        "a
+00005700: 6464 7265 7373 223a 2061 6464 7265 7373  ddress": address
+00005710: 2c0a 2020 2020 7d0a 2020 2020 6966 2066  ,.    }.    if f
+00005720: 6f75 7273 7175 6172 655f 6964 3a0a 2020  oursquare_id:.  
+00005730: 2020 2020 2020 7061 796c 6f61 645b 2266        payload["f
+00005740: 6f75 7273 7175 6172 655f 6964 225d 203d  oursquare_id"] =
+00005750: 2066 6f75 7273 7175 6172 655f 6964 0a20   foursquare_id. 
+00005760: 2020 2069 6620 666f 7572 7371 7561 7265     if foursquare
+00005770: 5f74 7970 653a 0a20 2020 2020 2020 2070  _type:.        p
+00005780: 6179 6c6f 6164 5b22 666f 7572 7371 7561  ayload["foursqua
+00005790: 7265 5f74 7970 6522 5d20 3d20 666f 7572  re_type"] = four
+000057a0: 7371 7561 7265 5f74 7970 650a 2020 2020  square_type.    
+000057b0: 6966 2064 6973 6162 6c65 5f6e 6f74 6966  if disable_notif
+000057c0: 6963 6174 696f 6e20 6973 206e 6f74 204e  ication is not N
+000057d0: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
+000057e0: 6c6f 6164 5b22 6469 7361 626c 655f 6e6f  load["disable_no
+000057f0: 7469 6669 6361 7469 6f6e 225d 203d 2064  tification"] = d
+00005800: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+00005810: 696f 6e0a 2020 2020 6966 2072 6570 6c79  ion.    if reply
+00005820: 5f74 6f5f 6d65 7373 6167 655f 6964 3a0a  _to_message_id:.
+00005830: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
+00005840: 2272 6570 6c79 5f74 6f5f 6d65 7373 6167  "reply_to_messag
+00005850: 655f 6964 225d 203d 2072 6570 6c79 5f74  e_id"] = reply_t
+00005860: 6f5f 6d65 7373 6167 655f 6964 0a20 2020  o_message_id.   
+00005870: 2069 6620 7265 706c 795f 6d61 726b 7570   if reply_markup
+00005880: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+00005890: 645b 2272 6570 6c79 5f6d 6172 6b75 7022  d["reply_markup"
+000058a0: 5d20 3d20 6177 6169 7420 5f63 6f6e 7665  ] = await _conve
+000058b0: 7274 5f6d 6172 6b75 7028 7265 706c 795f  rt_markup(reply_
+000058c0: 6d61 726b 7570 290a 2020 2020 6966 2074  markup).    if t
+000058d0: 696d 656f 7574 3a0a 2020 2020 2020 2020  imeout:.        
+000058e0: 7061 796c 6f61 645b 2274 696d 656f 7574  payload["timeout
+000058f0: 225d 203d 2074 696d 656f 7574 0a20 2020  "] = timeout.   
+00005900: 2069 6620 616c 6c6f 775f 7365 6e64 696e   if allow_sendin
+00005910: 675f 7769 7468 6f75 745f 7265 706c 7920  g_without_reply 
+00005920: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00005930: 2020 2020 2070 6179 6c6f 6164 5b22 616c       payload["al
+00005940: 6c6f 775f 7365 6e64 696e 675f 7769 7468  low_sending_with
+00005950: 6f75 745f 7265 706c 7922 5d20 3d20 616c  out_reply"] = al
+00005960: 6c6f 775f 7365 6e64 696e 675f 7769 7468  low_sending_with
+00005970: 6f75 745f 7265 706c 790a 2020 2020 6966  out_reply.    if
+00005980: 2067 6f6f 676c 655f 706c 6163 655f 6964   google_place_id
+00005990: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+000059a0: 645b 2267 6f6f 676c 655f 706c 6163 655f  d["google_place_
+000059b0: 6964 225d 203d 2067 6f6f 676c 655f 706c  id"] = google_pl
+000059c0: 6163 655f 6964 0a20 2020 2069 6620 676f  ace_id.    if go
+000059d0: 6f67 6c65 5f70 6c61 6365 5f74 7970 653a  ogle_place_type:
+000059e0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+000059f0: 5b22 676f 6f67 6c65 5f70 6c61 6365 5f74  ["google_place_t
+00005a00: 7970 6522 5d20 3d20 676f 6f67 6c65 5f70  ype"] = google_p
+00005a10: 6c61 6365 5f74 7970 650a 2020 2020 6966  lace_type.    if
+00005a20: 2070 726f 7465 6374 5f63 6f6e 7465 6e74   protect_content
+00005a30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00005a40: 2020 2020 2020 7061 796c 6f61 645b 2270        payload["p
+00005a50: 726f 7465 6374 5f63 6f6e 7465 6e74 225d  rotect_content"]
+00005a60: 203d 2070 726f 7465 6374 5f63 6f6e 7465   = protect_conte
+00005a70: 6e74 0a20 2020 205f 6164 645f 6d65 7373  nt.    _add_mess
+00005a80: 6167 655f 7468 7265 6164 5f69 6428 7061  age_thread_id(pa
+00005a90: 796c 6f61 642c 206d 6573 7361 6765 5f74  yload, message_t
+00005aa0: 6872 6561 645f 6964 290a 2020 2020 7265  hread_id).    re
+00005ab0: 7475 726e 2061 7761 6974 205f 7265 7175  turn await _requ
+00005ac0: 6573 7428 746f 6b65 6e2c 206d 6574 686f  est(token, metho
+00005ad0: 645f 7572 6c2c 2070 6172 616d 733d 7061  d_url, params=pa
+00005ae0: 796c 6f61 6429 0a0a 0a61 7379 6e63 2064  yload)...async d
+00005af0: 6566 2073 656e 645f 636f 6e74 6163 7428  ef send_contact(
+00005b00: 0a20 2020 2074 6f6b 656e 2c0a 2020 2020  .    token,.    
+00005b10: 6368 6174 5f69 642c 0a20 2020 2070 686f  chat_id,.    pho
+00005b20: 6e65 5f6e 756d 6265 722c 0a20 2020 2066  ne_number,.    f
+00005b30: 6972 7374 5f6e 616d 652c 0a20 2020 206c  irst_name,.    l
+00005b40: 6173 745f 6e61 6d65 3d4e 6f6e 652c 0a20  ast_name=None,. 
+00005b50: 2020 2076 6361 7264 3d4e 6f6e 652c 0a20     vcard=None,. 
+00005b60: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
+00005b70: 6963 6174 696f 6e3d 4e6f 6e65 2c0a 2020  ication=None,.  
+00005b80: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
+00005b90: 6765 5f69 643d 4e6f 6e65 2c0a 2020 2020  ge_id=None,.    
+00005ba0: 7265 706c 795f 6d61 726b 7570 3d4e 6f6e  reply_markup=Non
+00005bb0: 652c 0a20 2020 2074 696d 656f 7574 3d4e  e,.    timeout=N
+00005bc0: 6f6e 652c 0a20 2020 2061 6c6c 6f77 5f73  one,.    allow_s
+00005bd0: 656e 6469 6e67 5f77 6974 686f 7574 5f72  ending_without_r
+00005be0: 6570 6c79 3d4e 6f6e 652c 0a20 2020 2070  eply=None,.    p
+00005bf0: 726f 7465 6374 5f63 6f6e 7465 6e74 3d4e  rotect_content=N
+00005c00: 6f6e 652c 0a20 2020 206d 6573 7361 6765  one,.    message
+00005c10: 5f74 6872 6561 645f 6964 3a20 4f70 7469  _thread_id: Opti
+00005c20: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00005c30: 2c0a 293a 0a20 2020 206d 6574 686f 645f  ,.):.    method_
+00005c40: 7572 6c20 3d20 7222 7365 6e64 436f 6e74  url = r"sendCont
+00005c50: 6163 7422 0a20 2020 2070 6179 6c6f 6164  act".    payload
+00005c60: 203d 207b 0a20 2020 2020 2020 2022 6368   = {.        "ch
+00005c70: 6174 5f69 6422 3a20 6368 6174 5f69 642c  at_id": chat_id,
+00005c80: 0a20 2020 2020 2020 2022 7068 6f6e 655f  .        "phone_
+00005c90: 6e75 6d62 6572 223a 2070 686f 6e65 5f6e  number": phone_n
+00005ca0: 756d 6265 722c 0a20 2020 2020 2020 2022  umber,.        "
+00005cb0: 6669 7273 745f 6e61 6d65 223a 2066 6972  first_name": fir
+00005cc0: 7374 5f6e 616d 652c 0a20 2020 207d 0a20  st_name,.    }. 
+00005cd0: 2020 2069 6620 6c61 7374 5f6e 616d 653a     if last_name:
+00005ce0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+00005cf0: 5b22 6c61 7374 5f6e 616d 6522 5d20 3d20  ["last_name"] = 
+00005d00: 6c61 7374 5f6e 616d 650a 2020 2020 6966  last_name.    if
+00005d10: 2076 6361 7264 3a0a 2020 2020 2020 2020   vcard:.        
+00005d20: 7061 796c 6f61 645b 2276 6361 7264 225d  payload["vcard"]
+00005d30: 203d 2076 6361 7264 0a20 2020 2069 6620   = vcard.    if 
+00005d40: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+00005d50: 7469 6f6e 2069 7320 6e6f 7420 4e6f 6e65  tion is not None
+00005d60: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+00005d70: 645b 2264 6973 6162 6c65 5f6e 6f74 6966  d["disable_notif
+00005d80: 6963 6174 696f 6e22 5d20 3d20 6469 7361  ication"] = disa
+00005d90: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+00005da0: 0a20 2020 2069 6620 7265 706c 795f 746f  .    if reply_to
+00005db0: 5f6d 6573 7361 6765 5f69 643a 0a20 2020  _message_id:.   
+00005dc0: 2020 2020 2070 6179 6c6f 6164 5b22 7265       payload["re
+00005dd0: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
+00005de0: 6422 5d20 3d20 7265 706c 795f 746f 5f6d  d"] = reply_to_m
+00005df0: 6573 7361 6765 5f69 640a 2020 2020 6966  essage_id.    if
+00005e00: 2072 6570 6c79 5f6d 6172 6b75 703a 0a20   reply_markup:. 
+00005e10: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+00005e20: 7265 706c 795f 6d61 726b 7570 225d 203d  reply_markup"] =
+00005e30: 2061 7761 6974 205f 636f 6e76 6572 745f   await _convert_
+00005e40: 6d61 726b 7570 2872 6570 6c79 5f6d 6172  markup(reply_mar
+00005e50: 6b75 7029 0a20 2020 2069 6620 7469 6d65  kup).    if time
+00005e60: 6f75 743a 0a20 2020 2020 2020 2070 6179  out:.        pay
+00005e70: 6c6f 6164 5b22 7469 6d65 6f75 7422 5d20  load["timeout"] 
+00005e80: 3d20 7469 6d65 6f75 740a 2020 2020 6966  = timeout.    if
+00005e90: 2061 6c6c 6f77 5f73 656e 6469 6e67 5f77   allow_sending_w
+00005ea0: 6974 686f 7574 5f72 6570 6c79 2069 7320  ithout_reply is 
+00005eb0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00005ec0: 2020 7061 796c 6f61 645b 2261 6c6c 6f77    payload["allow
+00005ed0: 5f73 656e 6469 6e67 5f77 6974 686f 7574  _sending_without
+00005ee0: 5f72 6570 6c79 225d 203d 2061 6c6c 6f77  _reply"] = allow
+00005ef0: 5f73 656e 6469 6e67 5f77 6974 686f 7574  _sending_without
+00005f00: 5f72 6570 6c79 0a20 2020 2069 6620 7072  _reply.    if pr
+00005f10: 6f74 6563 745f 636f 6e74 656e 7420 6973  otect_content is
+00005f20: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00005f30: 2020 2070 6179 6c6f 6164 5b22 7072 6f74     payload["prot
+00005f40: 6563 745f 636f 6e74 656e 7422 5d20 3d20  ect_content"] = 
+00005f50: 7072 6f74 6563 745f 636f 6e74 656e 740a  protect_content.
+00005f60: 2020 2020 5f61 6464 5f6d 6573 7361 6765      _add_message
+00005f70: 5f74 6872 6561 645f 6964 2870 6179 6c6f  _thread_id(paylo
+00005f80: 6164 2c20 6d65 7373 6167 655f 7468 7265  ad, message_thre
+00005f90: 6164 5f69 6429 0a20 2020 2072 6574 7572  ad_id).    retur
+00005fa0: 6e20 6177 6169 7420 5f72 6571 7565 7374  n await _request
+00005fb0: 2874 6f6b 656e 2c20 6d65 7468 6f64 5f75  (token, method_u
+00005fc0: 726c 2c20 7061 7261 6d73 3d70 6179 6c6f  rl, params=paylo
+00005fd0: 6164 290a 0a0a 6173 796e 6320 6465 6620  ad)...async def 
+00005fe0: 7365 6e64 5f63 6861 745f 6163 7469 6f6e  send_chat_action
+00005ff0: 2874 6f6b 656e 2c20 6368 6174 5f69 642c  (token, chat_id,
+00006000: 2061 6374 696f 6e2c 2074 696d 656f 7574   action, timeout
+00006010: 3d4e 6f6e 652c 206d 6573 7361 6765 5f74  =None, message_t
+00006020: 6872 6561 645f 6964 3a20 4f70 7469 6f6e  hread_id: Option
+00006030: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 293a  al[int] = None):
+00006040: 0a20 2020 2072 6f75 7465 203d 2072 2273  .    route = r"s
+00006050: 656e 6443 6861 7441 6374 696f 6e22 0a20  endChatAction". 
+00006060: 2020 2070 6179 6c6f 6164 203d 207b 2263     payload = {"c
+00006070: 6861 745f 6964 223a 2063 6861 745f 6964  hat_id": chat_id
+00006080: 2c20 2261 6374 696f 6e22 3a20 6163 7469  , "action": acti
+00006090: 6f6e 7d0a 2020 2020 6966 2074 696d 656f  on}.    if timeo
+000060a0: 7574 3a0a 2020 2020 2020 2020 7061 796c  ut:.        payl
+000060b0: 6f61 645b 2274 696d 656f 7574 225d 203d  oad["timeout"] =
+000060c0: 2074 696d 656f 7574 0a20 2020 205f 6164   timeout.    _ad
+000060d0: 645f 6d65 7373 6167 655f 7468 7265 6164  d_message_thread
+000060e0: 5f69 6428 7061 796c 6f61 642c 206d 6573  _id(payload, mes
+000060f0: 7361 6765 5f74 6872 6561 645f 6964 290a  sage_thread_id).
+00006100: 2020 2020 7265 7475 726e 2061 7761 6974      return await
+00006110: 205f 7265 7175 6573 7428 746f 6b65 6e2c   _request(token,
+00006120: 2072 6f75 7465 2c20 7061 7261 6d73 3d70   route, params=p
+00006130: 6179 6c6f 6164 290a 0a0a 6173 796e 6320  ayload)...async 
+00006140: 6465 6620 7365 6e64 5f76 6964 656f 280a  def send_video(.
+00006150: 2020 2020 746f 6b65 6e2c 0a20 2020 2063      token,.    c
+00006160: 6861 745f 6964 2c0a 2020 2020 6461 7461  hat_id,.    data
+00006170: 2c0a 2020 2020 6475 7261 7469 6f6e 3d4e  ,.    duration=N
+00006180: 6f6e 652c 0a20 2020 2063 6170 7469 6f6e  one,.    caption
+00006190: 3d4e 6f6e 652c 0a20 2020 2072 6570 6c79  =None,.    reply
+000061a0: 5f74 6f5f 6d65 7373 6167 655f 6964 3d4e  _to_message_id=N
+000061b0: 6f6e 652c 0a20 2020 2072 6570 6c79 5f6d  one,.    reply_m
+000061c0: 6172 6b75 703d 4e6f 6e65 2c0a 2020 2020  arkup=None,.    
+000061d0: 7061 7273 655f 6d6f 6465 3d4e 6f6e 652c  parse_mode=None,
+000061e0: 0a20 2020 2073 7570 706f 7274 735f 7374  .    supports_st
+000061f0: 7265 616d 696e 673d 4e6f 6e65 2c0a 2020  reaming=None,.  
+00006200: 2020 6469 7361 626c 655f 6e6f 7469 6669    disable_notifi
+00006210: 6361 7469 6f6e 3d4e 6f6e 652c 0a20 2020  cation=None,.   
+00006220: 2074 696d 656f 7574 3d4e 6f6e 652c 0a20   timeout=None,. 
+00006230: 2020 2074 6875 6d62 3d4e 6f6e 652c 0a20     thumb=None,. 
+00006240: 2020 2077 6964 7468 3d4e 6f6e 652c 0a20     width=None,. 
+00006250: 2020 2068 6569 6768 743d 4e6f 6e65 2c0a     height=None,.
+00006260: 2020 2020 6361 7074 696f 6e5f 656e 7469      caption_enti
+00006270: 7469 6573 3d4e 6f6e 652c 0a20 2020 2061  ties=None,.    a
+00006280: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
+00006290: 686f 7574 5f72 6570 6c79 3d4e 6f6e 652c  hout_reply=None,
+000062a0: 0a20 2020 2070 726f 7465 6374 5f63 6f6e  .    protect_con
+000062b0: 7465 6e74 3d4e 6f6e 652c 0a20 2020 206d  tent=None,.    m
+000062c0: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+000062d0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+000062e0: 3d20 4e6f 6e65 2c0a 2020 2020 6861 735f  = None,.    has_
+000062f0: 7370 6f69 6c65 723a 204f 7074 696f 6e61  spoiler: Optiona
+00006300: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a  l[bool] = None,.
+00006310: 293a 0a20 2020 206d 6574 686f 645f 7572  ):.    method_ur
+00006320: 6c20 3d20 7222 7365 6e64 5669 6465 6f22  l = r"sendVideo"
+00006330: 0a20 2020 2070 6179 6c6f 6164 203d 207b  .    payload = {
+00006340: 2263 6861 745f 6964 223a 2063 6861 745f  "chat_id": chat_
+00006350: 6964 7d0a 2020 2020 6669 6c65 7320 3d20  id}.    files = 
+00006360: 4e6f 6e65 0a20 2020 2069 6620 6e6f 7420  None.    if not 
+00006370: 7574 696c 2e69 735f 7374 7269 6e67 2864  util.is_string(d
+00006380: 6174 6129 3a0a 2020 2020 2020 2020 6669  ata):.        fi
+00006390: 6c65 7320 3d20 7b22 7669 6465 6f22 3a20  les = {"video": 
+000063a0: 6461 7461 7d0a 2020 2020 656c 7365 3a0a  data}.    else:.
+000063b0: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
+000063c0: 2276 6964 656f 225d 203d 2064 6174 610a  "video"] = data.
+000063d0: 2020 2020 6966 2064 7572 6174 696f 6e3a      if duration:
+000063e0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+000063f0: 5b22 6475 7261 7469 6f6e 225d 203d 2064  ["duration"] = d
+00006400: 7572 6174 696f 6e0a 2020 2020 6966 2063  uration.    if c
+00006410: 6170 7469 6f6e 3a0a 2020 2020 2020 2020  aption:.        
+00006420: 7061 796c 6f61 645b 2263 6170 7469 6f6e  payload["caption
+00006430: 225d 203d 2063 6170 7469 6f6e 0a20 2020  "] = caption.   
+00006440: 2069 6620 7265 706c 795f 746f 5f6d 6573   if reply_to_mes
+00006450: 7361 6765 5f69 643a 0a20 2020 2020 2020  sage_id:.       
+00006460: 2070 6179 6c6f 6164 5b22 7265 706c 795f   payload["reply_
+00006470: 746f 5f6d 6573 7361 6765 5f69 6422 5d20  to_message_id"] 
+00006480: 3d20 7265 706c 795f 746f 5f6d 6573 7361  = reply_to_messa
+00006490: 6765 5f69 640a 2020 2020 6966 2072 6570  ge_id.    if rep
+000064a0: 6c79 5f6d 6172 6b75 703a 0a20 2020 2020  ly_markup:.     
+000064b0: 2020 2070 6179 6c6f 6164 5b22 7265 706c     payload["repl
+000064c0: 795f 6d61 726b 7570 225d 203d 2061 7761  y_markup"] = awa
+000064d0: 6974 205f 636f 6e76 6572 745f 6d61 726b  it _convert_mark
+000064e0: 7570 2872 6570 6c79 5f6d 6172 6b75 7029  up(reply_markup)
+000064f0: 0a20 2020 2069 6620 7061 7273 655f 6d6f  .    if parse_mo
+00006500: 6465 3a0a 2020 2020 2020 2020 7061 796c  de:.        payl
+00006510: 6f61 645b 2270 6172 7365 5f6d 6f64 6522  oad["parse_mode"
+00006520: 5d20 3d20 7061 7273 655f 6d6f 6465 0a20  ] = parse_mode. 
+00006530: 2020 2069 6620 7375 7070 6f72 7473 5f73     if supports_s
+00006540: 7472 6561 6d69 6e67 2069 7320 6e6f 7420  treaming is not 
+00006550: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
+00006560: 796c 6f61 645b 2273 7570 706f 7274 735f  yload["supports_
+00006570: 7374 7265 616d 696e 6722 5d20 3d20 7375  streaming"] = su
+00006580: 7070 6f72 7473 5f73 7472 6561 6d69 6e67  pports_streaming
+00006590: 0a20 2020 2069 6620 6469 7361 626c 655f  .    if disable_
+000065a0: 6e6f 7469 6669 6361 7469 6f6e 2069 7320  notification is 
+000065b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000065c0: 2020 7061 796c 6f61 645b 2264 6973 6162    payload["disab
+000065d0: 6c65 5f6e 6f74 6966 6963 6174 696f 6e22  le_notification"
+000065e0: 5d20 3d20 6469 7361 626c 655f 6e6f 7469  ] = disable_noti
+000065f0: 6669 6361 7469 6f6e 0a20 2020 2069 6620  fication.    if 
+00006600: 7469 6d65 6f75 743a 0a20 2020 2020 2020  timeout:.       
+00006610: 2070 6179 6c6f 6164 5b22 7469 6d65 6f75   payload["timeou
+00006620: 7422 5d20 3d20 7469 6d65 6f75 740a 2020  t"] = timeout.  
+00006630: 2020 6966 2074 6875 6d62 3a0a 2020 2020    if thumb:.    
+00006640: 2020 2020 6966 206e 6f74 2075 7469 6c2e      if not util.
+00006650: 6973 5f73 7472 696e 6728 7468 756d 6229  is_string(thumb)
+00006660: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00006670: 2066 696c 6573 3a0a 2020 2020 2020 2020   files:.        
+00006680: 2020 2020 2020 2020 6669 6c65 735b 2274          files["t
+00006690: 6875 6d62 225d 203d 2074 6875 6d62 0a20  humb"] = thumb. 
+000066a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000066b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000066c0: 2066 696c 6573 203d 207b 2274 6875 6d62   files = {"thumb
+000066d0: 223a 2074 6875 6d62 7d0a 2020 2020 2020  ": thumb}.      
+000066e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000066f0: 2020 2020 7061 796c 6f61 645b 2274 6875      payload["thu
+00006700: 6d62 225d 203d 2074 6875 6d62 0a20 2020  mb"] = thumb.   
+00006710: 2069 6620 7769 6474 683a 0a20 2020 2020   if width:.     
+00006720: 2020 2070 6179 6c6f 6164 5b22 7769 6474     payload["widt
+00006730: 6822 5d20 3d20 7769 6474 680a 2020 2020  h"] = width.    
+00006740: 6966 2068 6569 6768 743a 0a20 2020 2020  if height:.     
+00006750: 2020 2070 6179 6c6f 6164 5b22 6865 6967     payload["heig
+00006760: 6874 225d 203d 2068 6569 6768 740a 2020  ht"] = height.  
+00006770: 2020 6966 2063 6170 7469 6f6e 5f65 6e74    if caption_ent
+00006780: 6974 6965 733a 0a20 2020 2020 2020 2070  ities:.        p
+00006790: 6179 6c6f 6164 5b22 6361 7074 696f 6e5f  ayload["caption_
+000067a0: 656e 7469 7469 6573 225d 203d 206a 736f  entities"] = jso
+000067b0: 6e2e 6475 6d70 7328 7479 7065 732e 4d65  n.dumps(types.Me
+000067c0: 7373 6167 6545 6e74 6974 792e 746f 5f6c  ssageEntity.to_l
+000067d0: 6973 745f 6f66 5f64 6963 7473 2863 6170  ist_of_dicts(cap
+000067e0: 7469 6f6e 5f65 6e74 6974 6965 7329 290a  tion_entities)).
+000067f0: 2020 2020 6966 2061 6c6c 6f77 5f73 656e      if allow_sen
+00006800: 6469 6e67 5f77 6974 686f 7574 5f72 6570  ding_without_rep
+00006810: 6c79 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ly is not None:.
+00006820: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
+00006830: 2261 6c6c 6f77 5f73 656e 6469 6e67 5f77  "allow_sending_w
+00006840: 6974 686f 7574 5f72 6570 6c79 225d 203d  ithout_reply"] =
+00006850: 2061 6c6c 6f77 5f73 656e 6469 6e67 5f77   allow_sending_w
+00006860: 6974 686f 7574 5f72 6570 6c79 0a20 2020  ithout_reply.   
+00006870: 2069 6620 7072 6f74 6563 745f 636f 6e74   if protect_cont
+00006880: 656e 7420 6973 206e 6f74 204e 6f6e 653a  ent is not None:
+00006890: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+000068a0: 5b22 7072 6f74 6563 745f 636f 6e74 656e  ["protect_conten
+000068b0: 7422 5d20 3d20 7072 6f74 6563 745f 636f  t"] = protect_co
+000068c0: 6e74 656e 740a 2020 2020 5f61 6464 5f6d  ntent.    _add_m
+000068d0: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+000068e0: 2870 6179 6c6f 6164 2c20 6d65 7373 6167  (payload, messag
+000068f0: 655f 7468 7265 6164 5f69 6429 0a20 2020  e_thread_id).   
+00006900: 2069 6620 6861 735f 7370 6f69 6c65 7220   if has_spoiler 
+00006910: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00006920: 2020 2020 2070 6179 6c6f 6164 5b22 6861       payload["ha
+00006930: 735f 7370 6f69 6c65 7222 5d20 3d20 6861  s_spoiler"] = ha
+00006940: 735f 7370 6f69 6c65 720a 2020 2020 7265  s_spoiler.    re
+00006950: 7475 726e 2061 7761 6974 205f 7265 7175  turn await _requ
+00006960: 6573 7428 746f 6b65 6e2c 206d 6574 686f  est(token, metho
+00006970: 645f 7572 6c2c 2070 6172 616d 733d 7061  d_url, params=pa
+00006980: 796c 6f61 642c 2066 696c 6573 3d66 696c  yload, files=fil
+00006990: 6573 2c20 6d65 7468 6f64 3d22 706f 7374  es, method="post
+000069a0: 2229 0a0a 0a61 7379 6e63 2064 6566 2073  ")...async def s
+000069b0: 656e 645f 616e 696d 6174 696f 6e28 0a20  end_animation(. 
+000069c0: 2020 2074 6f6b 656e 2c0a 2020 2020 6368     token,.    ch
+000069d0: 6174 5f69 642c 0a20 2020 2064 6174 612c  at_id,.    data,
+000069e0: 0a20 2020 2064 7572 6174 696f 6e3d 4e6f  .    duration=No
+000069f0: 6e65 2c0a 2020 2020 6361 7074 696f 6e3d  ne,.    caption=
+00006a00: 4e6f 6e65 2c0a 2020 2020 7265 706c 795f  None,.    reply_
+00006a10: 746f 5f6d 6573 7361 6765 5f69 643d 4e6f  to_message_id=No
+00006a20: 6e65 2c0a 2020 2020 7265 706c 795f 6d61  ne,.    reply_ma
+00006a30: 726b 7570 3d4e 6f6e 652c 0a20 2020 2070  rkup=None,.    p
+00006a40: 6172 7365 5f6d 6f64 653d 4e6f 6e65 2c0a  arse_mode=None,.
+00006a50: 2020 2020 6469 7361 626c 655f 6e6f 7469      disable_noti
+00006a60: 6669 6361 7469 6f6e 3d4e 6f6e 652c 0a20  fication=None,. 
+00006a70: 2020 2074 696d 656f 7574 3d4e 6f6e 652c     timeout=None,
+00006a80: 0a20 2020 2074 6875 6d62 3d4e 6f6e 652c  .    thumb=None,
+00006a90: 0a20 2020 2063 6170 7469 6f6e 5f65 6e74  .    caption_ent
+00006aa0: 6974 6965 733d 4e6f 6e65 2c0a 2020 2020  ities=None,.    
+00006ab0: 616c 6c6f 775f 7365 6e64 696e 675f 7769  allow_sending_wi
+00006ac0: 7468 6f75 745f 7265 706c 793d 4e6f 6e65  thout_reply=None
+00006ad0: 2c0a 2020 2020 7769 6474 683d 4e6f 6e65  ,.    width=None
+00006ae0: 2c0a 2020 2020 6865 6967 6874 3d4e 6f6e  ,.    height=Non
+00006af0: 652c 0a20 2020 2070 726f 7465 6374 5f63  e,.    protect_c
+00006b00: 6f6e 7465 6e74 3d4e 6f6e 652c 0a20 2020  ontent=None,.   
+00006b10: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
+00006b20: 6964 3a20 4f70 7469 6f6e 616c 5b69 6e74  id: Optional[int
+00006b30: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6861  ] = None,.    ha
+00006b40: 735f 7370 6f69 6c65 723a 204f 7074 696f  s_spoiler: Optio
+00006b50: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+00006b60: 2c0a 293a 0a20 2020 206d 6574 686f 645f  ,.):.    method_
+00006b70: 7572 6c20 3d20 7222 7365 6e64 416e 696d  url = r"sendAnim
+00006b80: 6174 696f 6e22 0a20 2020 2070 6179 6c6f  ation".    paylo
+00006b90: 6164 203d 207b 2263 6861 745f 6964 223a  ad = {"chat_id":
+00006ba0: 2063 6861 745f 6964 7d0a 2020 2020 6669   chat_id}.    fi
+00006bb0: 6c65 7320 3d20 4e6f 6e65 0a20 2020 2069  les = None.    i
+00006bc0: 6620 6e6f 7420 7574 696c 2e69 735f 7374  f not util.is_st
+00006bd0: 7269 6e67 2864 6174 6129 3a0a 2020 2020  ring(data):.    
+00006be0: 2020 2020 6669 6c65 7320 3d20 7b22 616e      files = {"an
+00006bf0: 696d 6174 696f 6e22 3a20 6461 7461 7d0a  imation": data}.
+00006c00: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00006c10: 2020 7061 796c 6f61 645b 2261 6e69 6d61    payload["anima
+00006c20: 7469 6f6e 225d 203d 2064 6174 610a 2020  tion"] = data.  
+00006c30: 2020 6966 2064 7572 6174 696f 6e3a 0a20    if duration:. 
+00006c40: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+00006c50: 6475 7261 7469 6f6e 225d 203d 2064 7572  duration"] = dur
+00006c60: 6174 696f 6e0a 2020 2020 6966 2063 6170  ation.    if cap
+00006c70: 7469 6f6e 3a0a 2020 2020 2020 2020 7061  tion:.        pa
+00006c80: 796c 6f61 645b 2263 6170 7469 6f6e 225d  yload["caption"]
+00006c90: 203d 2063 6170 7469 6f6e 0a20 2020 2069   = caption.    i
+00006ca0: 6620 7265 706c 795f 746f 5f6d 6573 7361  f reply_to_messa
+00006cb0: 6765 5f69 643a 0a20 2020 2020 2020 2070  ge_id:.        p
+00006cc0: 6179 6c6f 6164 5b22 7265 706c 795f 746f  ayload["reply_to
+00006cd0: 5f6d 6573 7361 6765 5f69 6422 5d20 3d20  _message_id"] = 
+00006ce0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+00006cf0: 5f69 640a 2020 2020 6966 2072 6570 6c79  _id.    if reply
+00006d00: 5f6d 6172 6b75 703a 0a20 2020 2020 2020  _markup:.       
+00006d10: 2070 6179 6c6f 6164 5b22 7265 706c 795f   payload["reply_
+00006d20: 6d61 726b 7570 225d 203d 2061 7761 6974  markup"] = await
+00006d30: 205f 636f 6e76 6572 745f 6d61 726b 7570   _convert_markup
+00006d40: 2872 6570 6c79 5f6d 6172 6b75 7029 0a20  (reply_markup). 
+00006d50: 2020 2069 6620 7061 7273 655f 6d6f 6465     if parse_mode
+00006d60: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+00006d70: 645b 2270 6172 7365 5f6d 6f64 6522 5d20  d["parse_mode"] 
+00006d80: 3d20 7061 7273 655f 6d6f 6465 0a20 2020  = parse_mode.   
+00006d90: 2069 6620 6469 7361 626c 655f 6e6f 7469   if disable_noti
+00006da0: 6669 6361 7469 6f6e 2069 7320 6e6f 7420  fication is not 
+00006db0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
+00006dc0: 796c 6f61 645b 2264 6973 6162 6c65 5f6e  yload["disable_n
+00006dd0: 6f74 6966 6963 6174 696f 6e22 5d20 3d20  otification"] = 
+00006de0: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+00006df0: 7469 6f6e 0a20 2020 2069 6620 7469 6d65  tion.    if time
+00006e00: 6f75 743a 0a20 2020 2020 2020 2070 6179  out:.        pay
+00006e10: 6c6f 6164 5b22 7469 6d65 6f75 7422 5d20  load["timeout"] 
+00006e20: 3d20 7469 6d65 6f75 740a 2020 2020 6966  = timeout.    if
+00006e30: 2074 6875 6d62 3a0a 2020 2020 2020 2020   thumb:.        
+00006e40: 6966 206e 6f74 2075 7469 6c2e 6973 5f73  if not util.is_s
+00006e50: 7472 696e 6728 7468 756d 6229 3a0a 2020  tring(thumb):.  
+00006e60: 2020 2020 2020 2020 2020 6966 2066 696c            if fil
+00006e70: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00006e80: 2020 2020 6669 6c65 735b 2274 6875 6d62      files["thumb
+00006e90: 225d 203d 2074 6875 6d62 0a20 2020 2020  "] = thumb.     
+00006ea0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00006eb0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00006ec0: 6573 203d 207b 2274 6875 6d62 223a 2074  es = {"thumb": t
+00006ed0: 6875 6d62 7d0a 2020 2020 2020 2020 656c  humb}.        el
+00006ee0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00006ef0: 7061 796c 6f61 645b 2274 6875 6d62 225d  payload["thumb"]
+00006f00: 203d 2074 6875 6d62 0a20 2020 2069 6620   = thumb.    if 
+00006f10: 6361 7074 696f 6e5f 656e 7469 7469 6573  caption_entities
+00006f20: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+00006f30: 645b 2263 6170 7469 6f6e 5f65 6e74 6974  d["caption_entit
+00006f40: 6965 7322 5d20 3d20 6a73 6f6e 2e64 756d  ies"] = json.dum
+00006f50: 7073 2874 7970 6573 2e4d 6573 7361 6765  ps(types.Message
+00006f60: 456e 7469 7479 2e74 6f5f 6c69 7374 5f6f  Entity.to_list_o
+00006f70: 665f 6469 6374 7328 6361 7074 696f 6e5f  f_dicts(caption_
+00006f80: 656e 7469 7469 6573 2929 0a20 2020 2069  entities)).    i
+00006f90: 6620 616c 6c6f 775f 7365 6e64 696e 675f  f allow_sending_
+00006fa0: 7769 7468 6f75 745f 7265 706c 7920 6973  without_reply is
+00006fb0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00006fc0: 2020 2070 6179 6c6f 6164 5b22 616c 6c6f     payload["allo
+00006fd0: 775f 7365 6e64 696e 675f 7769 7468 6f75  w_sending_withou
+00006fe0: 745f 7265 706c 7922 5d20 3d20 616c 6c6f  t_reply"] = allo
+00006ff0: 775f 7365 6e64 696e 675f 7769 7468 6f75  w_sending_withou
+00007000: 745f 7265 706c 790a 2020 2020 6966 2077  t_reply.    if w
+00007010: 6964 7468 3a0a 2020 2020 2020 2020 7061  idth:.        pa
+00007020: 796c 6f61 645b 2277 6964 7468 225d 203d  yload["width"] =
+00007030: 2077 6964 7468 0a20 2020 2069 6620 6865   width.    if he
+00007040: 6967 6874 3a0a 2020 2020 2020 2020 7061  ight:.        pa
+00007050: 796c 6f61 645b 2268 6569 6768 7422 5d20  yload["height"] 
+00007060: 3d20 6865 6967 6874 0a20 2020 2069 6620  = height.    if 
+00007070: 7072 6f74 6563 745f 636f 6e74 656e 7420  protect_content 
+00007080: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00007090: 2020 2020 2070 6179 6c6f 6164 5b22 7072       payload["pr
+000070a0: 6f74 6563 745f 636f 6e74 656e 7422 5d20  otect_content"] 
+000070b0: 3d20 7072 6f74 6563 745f 636f 6e74 656e  = protect_conten
+000070c0: 740a 2020 2020 5f61 6464 5f6d 6573 7361  t.    _add_messa
+000070d0: 6765 5f74 6872 6561 645f 6964 2870 6179  ge_thread_id(pay
+000070e0: 6c6f 6164 2c20 6d65 7373 6167 655f 7468  load, message_th
+000070f0: 7265 6164 5f69 6429 0a0a 2020 2020 6966  read_id)..    if
+00007100: 2068 6173 5f73 706f 696c 6572 2069 7320   has_spoiler is 
+00007110: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00007120: 2020 7061 796c 6f61 645b 2268 6173 5f73    payload["has_s
+00007130: 706f 696c 6572 225d 203d 2068 6173 5f73  poiler"] = has_s
+00007140: 706f 696c 6572 0a20 2020 2072 6574 7572  poiler.    retur
+00007150: 6e20 6177 6169 7420 5f72 6571 7565 7374  n await _request
+00007160: 2874 6f6b 656e 2c20 6d65 7468 6f64 5f75  (token, method_u
+00007170: 726c 2c20 7061 7261 6d73 3d70 6179 6c6f  rl, params=paylo
+00007180: 6164 2c20 6669 6c65 733d 6669 6c65 732c  ad, files=files,
+00007190: 206d 6574 686f 643d 2270 6f73 7422 290a   method="post").
+000071a0: 0a0a 6173 796e 6320 6465 6620 7365 6e64  ..async def send
+000071b0: 5f76 6f69 6365 280a 2020 2020 746f 6b65  _voice(.    toke
+000071c0: 6e2c 0a20 2020 2063 6861 745f 6964 2c0a  n,.    chat_id,.
+000071d0: 2020 2020 766f 6963 652c 0a20 2020 2063      voice,.    c
+000071e0: 6170 7469 6f6e 3d4e 6f6e 652c 0a20 2020  aption=None,.   
+000071f0: 2064 7572 6174 696f 6e3d 4e6f 6e65 2c0a   duration=None,.
+00007200: 2020 2020 7265 706c 795f 746f 5f6d 6573      reply_to_mes
+00007210: 7361 6765 5f69 643d 4e6f 6e65 2c0a 2020  sage_id=None,.  
+00007220: 2020 7265 706c 795f 6d61 726b 7570 3d4e    reply_markup=N
+00007230: 6f6e 652c 0a20 2020 2070 6172 7365 5f6d  one,.    parse_m
+00007240: 6f64 653d 4e6f 6e65 2c0a 2020 2020 6469  ode=None,.    di
+00007250: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+00007260: 6f6e 3d4e 6f6e 652c 0a20 2020 2074 696d  on=None,.    tim
+00007270: 656f 7574 3d4e 6f6e 652c 0a20 2020 2063  eout=None,.    c
+00007280: 6170 7469 6f6e 5f65 6e74 6974 6965 733d  aption_entities=
+00007290: 4e6f 6e65 2c0a 2020 2020 616c 6c6f 775f  None,.    allow_
+000072a0: 7365 6e64 696e 675f 7769 7468 6f75 745f  sending_without_
+000072b0: 7265 706c 793d 4e6f 6e65 2c0a 2020 2020  reply=None,.    
+000072c0: 7072 6f74 6563 745f 636f 6e74 656e 743d  protect_content=
+000072d0: 4e6f 6e65 2c0a 2020 2020 6d65 7373 6167  None,.    messag
+000072e0: 655f 7468 7265 6164 5f69 643a 204f 7074  e_thread_id: Opt
+000072f0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00007300: 652c 0a29 3a0a 2020 2020 6d65 7468 6f64  e,.):.    method
+00007310: 5f75 726c 203d 2072 2273 656e 6456 6f69  _url = r"sendVoi
+00007320: 6365 220a 2020 2020 7061 796c 6f61 6420  ce".    payload 
+00007330: 3d20 7b22 6368 6174 5f69 6422 3a20 6368  = {"chat_id": ch
+00007340: 6174 5f69 647d 0a20 2020 2066 696c 6573  at_id}.    files
+00007350: 203d 204e 6f6e 650a 2020 2020 6966 206e   = None.    if n
+00007360: 6f74 2075 7469 6c2e 6973 5f73 7472 696e  ot util.is_strin
+00007370: 6728 766f 6963 6529 3a0a 2020 2020 2020  g(voice):.      
+00007380: 2020 6669 6c65 7320 3d20 7b22 766f 6963    files = {"voic
+00007390: 6522 3a20 766f 6963 657d 0a20 2020 2065  e": voice}.    e
+000073a0: 6c73 653a 0a20 2020 2020 2020 2070 6179  lse:.        pay
+000073b0: 6c6f 6164 5b22 766f 6963 6522 5d20 3d20  load["voice"] = 
+000073c0: 766f 6963 650a 2020 2020 6966 2063 6170  voice.    if cap
+000073d0: 7469 6f6e 3a0a 2020 2020 2020 2020 7061  tion:.        pa
+000073e0: 796c 6f61 645b 2263 6170 7469 6f6e 225d  yload["caption"]
+000073f0: 203d 2063 6170 7469 6f6e 0a20 2020 2069   = caption.    i
+00007400: 6620 6475 7261 7469 6f6e 3a0a 2020 2020  f duration:.    
+00007410: 2020 2020 7061 796c 6f61 645b 2264 7572      payload["dur
+00007420: 6174 696f 6e22 5d20 3d20 6475 7261 7469  ation"] = durati
+00007430: 6f6e 0a20 2020 2069 6620 7265 706c 795f  on.    if reply_
+00007440: 746f 5f6d 6573 7361 6765 5f69 643a 0a20  to_message_id:. 
+00007450: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+00007460: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+00007470: 5f69 6422 5d20 3d20 7265 706c 795f 746f  _id"] = reply_to
+00007480: 5f6d 6573 7361 6765 5f69 640a 2020 2020  _message_id.    
+00007490: 6966 2072 6570 6c79 5f6d 6172 6b75 703a  if reply_markup:
+000074a0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+000074b0: 5b22 7265 706c 795f 6d61 726b 7570 225d  ["reply_markup"]
+000074c0: 203d 2061 7761 6974 205f 636f 6e76 6572   = await _conver
+000074d0: 745f 6d61 726b 7570 2872 6570 6c79 5f6d  t_markup(reply_m
+000074e0: 6172 6b75 7029 0a20 2020 2069 6620 7061  arkup).    if pa
+000074f0: 7273 655f 6d6f 6465 3a0a 2020 2020 2020  rse_mode:.      
+00007500: 2020 7061 796c 6f61 645b 2270 6172 7365    payload["parse
+00007510: 5f6d 6f64 6522 5d20 3d20 7061 7273 655f  _mode"] = parse_
+00007520: 6d6f 6465 0a20 2020 2069 6620 6469 7361  mode.    if disa
+00007530: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+00007540: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00007550: 2020 2020 2020 7061 796c 6f61 645b 2264        payload["d
+00007560: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+00007570: 696f 6e22 5d20 3d20 6469 7361 626c 655f  ion"] = disable_
+00007580: 6e6f 7469 6669 6361 7469 6f6e 0a20 2020  notification.   
+00007590: 2069 6620 7469 6d65 6f75 743a 0a20 2020   if timeout:.   
+000075a0: 2020 2020 2070 6179 6c6f 6164 5b22 7469       payload["ti
+000075b0: 6d65 6f75 7422 5d20 3d20 7469 6d65 6f75  meout"] = timeou
+000075c0: 740a 2020 2020 6966 2063 6170 7469 6f6e  t.    if caption
+000075d0: 5f65 6e74 6974 6965 733a 0a20 2020 2020  _entities:.     
+000075e0: 2020 2070 6179 6c6f 6164 5b22 6361 7074     payload["capt
+000075f0: 696f 6e5f 656e 7469 7469 6573 225d 203d  ion_entities"] =
+00007600: 206a 736f 6e2e 6475 6d70 7328 7479 7065   json.dumps(type
+00007610: 732e 4d65 7373 6167 6545 6e74 6974 792e  s.MessageEntity.
+00007620: 746f 5f6c 6973 745f 6f66 5f64 6963 7473  to_list_of_dicts
+00007630: 2863 6170 7469 6f6e 5f65 6e74 6974 6965  (caption_entitie
+00007640: 7329 290a 2020 2020 6966 2061 6c6c 6f77  s)).    if allow
+00007650: 5f73 656e 6469 6e67 5f77 6974 686f 7574  _sending_without
+00007660: 5f72 6570 6c79 2069 7320 6e6f 7420 4e6f  _reply is not No
+00007670: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
+00007680: 6f61 645b 2261 6c6c 6f77 5f73 656e 6469  oad["allow_sendi
+00007690: 6e67 5f77 6974 686f 7574 5f72 6570 6c79  ng_without_reply
+000076a0: 225d 203d 2061 6c6c 6f77 5f73 656e 6469  "] = allow_sendi
+000076b0: 6e67 5f77 6974 686f 7574 5f72 6570 6c79  ng_without_reply
+000076c0: 0a20 2020 2069 6620 7072 6f74 6563 745f  .    if protect_
+000076d0: 636f 6e74 656e 7420 6973 206e 6f74 204e  content is not N
+000076e0: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
+000076f0: 6c6f 6164 5b22 7072 6f74 6563 745f 636f  load["protect_co
+00007700: 6e74 656e 7422 5d20 3d20 7072 6f74 6563  ntent"] = protec
+00007710: 745f 636f 6e74 656e 740a 2020 2020 5f61  t_content.    _a
+00007720: 6464 5f6d 6573 7361 6765 5f74 6872 6561  dd_message_threa
+00007730: 645f 6964 2870 6179 6c6f 6164 2c20 6d65  d_id(payload, me
+00007740: 7373 6167 655f 7468 7265 6164 5f69 6429  ssage_thread_id)
+00007750: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
+00007760: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
+00007770: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
+00007780: 7261 6d73 3d70 6179 6c6f 6164 2c20 6669  rams=payload, fi
+00007790: 6c65 733d 6669 6c65 732c 206d 6574 686f  les=files, metho
+000077a0: 643d 2270 6f73 7422 290a 0a0a 6173 796e  d="post")...asyn
+000077b0: 6320 6465 6620 7365 6e64 5f76 6964 656f  c def send_video
+000077c0: 5f6e 6f74 6528 0a20 2020 2074 6f6b 656e  _note(.    token
+000077d0: 2c0a 2020 2020 6368 6174 5f69 642c 0a20  ,.    chat_id,. 
+000077e0: 2020 2064 6174 612c 0a20 2020 2064 7572     data,.    dur
+000077f0: 6174 696f 6e3d 4e6f 6e65 2c0a 2020 2020  ation=None,.    
+00007800: 6c65 6e67 7468 3d4e 6f6e 652c 0a20 2020  length=None,.   
+00007810: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
+00007820: 655f 6964 3d4e 6f6e 652c 0a20 2020 2072  e_id=None,.    r
+00007830: 6570 6c79 5f6d 6172 6b75 703d 4e6f 6e65  eply_markup=None
+00007840: 2c0a 2020 2020 6469 7361 626c 655f 6e6f  ,.    disable_no
+00007850: 7469 6669 6361 7469 6f6e 3d4e 6f6e 652c  tification=None,
+00007860: 0a20 2020 2074 696d 656f 7574 3d4e 6f6e  .    timeout=Non
+00007870: 652c 0a20 2020 2074 6875 6d62 3d4e 6f6e  e,.    thumb=Non
+00007880: 652c 0a20 2020 2061 6c6c 6f77 5f73 656e  e,.    allow_sen
+00007890: 6469 6e67 5f77 6974 686f 7574 5f72 6570  ding_without_rep
+000078a0: 6c79 3d4e 6f6e 652c 0a20 2020 2070 726f  ly=None,.    pro
+000078b0: 7465 6374 5f63 6f6e 7465 6e74 3d4e 6f6e  tect_content=Non
+000078c0: 652c 0a20 2020 206d 6573 7361 6765 5f74  e,.    message_t
+000078d0: 6872 6561 645f 6964 3a20 4f70 7469 6f6e  hread_id: Option
+000078e0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
+000078f0: 293a 0a20 2020 206d 6574 686f 645f 7572  ):.    method_ur
+00007900: 6c20 3d20 7222 7365 6e64 5669 6465 6f4e  l = r"sendVideoN
+00007910: 6f74 6522 0a20 2020 2070 6179 6c6f 6164  ote".    payload
+00007920: 203d 207b 2263 6861 745f 6964 223a 2063   = {"chat_id": c
+00007930: 6861 745f 6964 7d0a 2020 2020 6669 6c65  hat_id}.    file
+00007940: 7320 3d20 4e6f 6e65 0a20 2020 2069 6620  s = None.    if 
+00007950: 6e6f 7420 7574 696c 2e69 735f 7374 7269  not util.is_stri
+00007960: 6e67 2864 6174 6129 3a0a 2020 2020 2020  ng(data):.      
+00007970: 2020 6669 6c65 7320 3d20 7b22 7669 6465    files = {"vide
+00007980: 6f5f 6e6f 7465 223a 2064 6174 617d 0a20  o_note": data}. 
+00007990: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000079a0: 2070 6179 6c6f 6164 5b22 7669 6465 6f5f   payload["video_
+000079b0: 6e6f 7465 225d 203d 2064 6174 610a 2020  note"] = data.  
+000079c0: 2020 6966 2064 7572 6174 696f 6e3a 0a20    if duration:. 
+000079d0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+000079e0: 6475 7261 7469 6f6e 225d 203d 2064 7572  duration"] = dur
+000079f0: 6174 696f 6e0a 2020 2020 6966 206c 656e  ation.    if len
+00007a00: 6774 6820 616e 6420 2873 7472 286c 656e  gth and (str(len
+00007a10: 6774 6829 2e69 7364 6967 6974 2829 2061  gth).isdigit() a
+00007a20: 6e64 2069 6e74 286c 656e 6774 6829 203c  nd int(length) <
+00007a30: 3d20 3633 3929 3a0a 2020 2020 2020 2020  = 639):.        
+00007a40: 7061 796c 6f61 645b 226c 656e 6774 6822  payload["length"
+00007a50: 5d20 3d20 6c65 6e67 7468 0a20 2020 2065  ] = length.    e
+00007a60: 6c73 653a 0a20 2020 2020 2020 2070 6179  lse:.        pay
+00007a70: 6c6f 6164 5b22 6c65 6e67 7468 225d 203d  load["length"] =
+00007a80: 2036 3339 2020 2320 7365 656d 7320 6c69   639  # seems li
+00007a90: 6b65 2069 7420 6973 204d 4158 206c 656e  ke it is MAX len
+00007aa0: 6774 6820 7369 7a65 0a20 2020 2069 6620  gth size.    if 
+00007ab0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+00007ac0: 5f69 643a 0a20 2020 2020 2020 2070 6179  _id:.        pay
+00007ad0: 6c6f 6164 5b22 7265 706c 795f 746f 5f6d  load["reply_to_m
+00007ae0: 6573 7361 6765 5f69 6422 5d20 3d20 7265  essage_id"] = re
+00007af0: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
+00007b00: 640a 2020 2020 6966 2072 6570 6c79 5f6d  d.    if reply_m
+00007b10: 6172 6b75 703a 0a20 2020 2020 2020 2070  arkup:.        p
+00007b20: 6179 6c6f 6164 5b22 7265 706c 795f 6d61  ayload["reply_ma
+00007b30: 726b 7570 225d 203d 2061 7761 6974 205f  rkup"] = await _
+00007b40: 636f 6e76 6572 745f 6d61 726b 7570 2872  convert_markup(r
+00007b50: 6570 6c79 5f6d 6172 6b75 7029 0a20 2020  eply_markup).   
+00007b60: 2069 6620 6469 7361 626c 655f 6e6f 7469   if disable_noti
+00007b70: 6669 6361 7469 6f6e 2069 7320 6e6f 7420  fication is not 
+00007b80: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
+00007b90: 796c 6f61 645b 2264 6973 6162 6c65 5f6e  yload["disable_n
+00007ba0: 6f74 6966 6963 6174 696f 6e22 5d20 3d20  otification"] = 
+00007bb0: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+00007bc0: 7469 6f6e 0a20 2020 2069 6620 7469 6d65  tion.    if time
+00007bd0: 6f75 743a 0a20 2020 2020 2020 2070 6179  out:.        pay
+00007be0: 6c6f 6164 5b22 7469 6d65 6f75 7422 5d20  load["timeout"] 
+00007bf0: 3d20 7469 6d65 6f75 740a 2020 2020 6966  = timeout.    if
+00007c00: 2074 6875 6d62 3a0a 2020 2020 2020 2020   thumb:.        
+00007c10: 6966 206e 6f74 2075 7469 6c2e 6973 5f73  if not util.is_s
+00007c20: 7472 696e 6728 7468 756d 6229 3a0a 2020  tring(thumb):.  
+00007c30: 2020 2020 2020 2020 2020 6966 2066 696c            if fil
+00007c40: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00007c50: 2020 2020 6669 6c65 735b 2274 6875 6d62      files["thumb
+00007c60: 225d 203d 2074 6875 6d62 0a20 2020 2020  "] = thumb.     
+00007c70: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00007c80: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00007c90: 6573 203d 207b 2274 6875 6d62 223a 2074  es = {"thumb": t
+00007ca0: 6875 6d62 7d0a 2020 2020 2020 2020 656c  humb}.        el
+00007cb0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00007cc0: 7061 796c 6f61 645b 2274 6875 6d62 225d  payload["thumb"]
+00007cd0: 203d 2074 6875 6d62 0a20 2020 2069 6620   = thumb.    if 
+00007ce0: 616c 6c6f 775f 7365 6e64 696e 675f 7769  allow_sending_wi
+00007cf0: 7468 6f75 745f 7265 706c 7920 6973 206e  thout_reply is n
+00007d00: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00007d10: 2070 6179 6c6f 6164 5b22 616c 6c6f 775f   payload["allow_
+00007d20: 7365 6e64 696e 675f 7769 7468 6f75 745f  sending_without_
+00007d30: 7265 706c 7922 5d20 3d20 616c 6c6f 775f  reply"] = allow_
+00007d40: 7365 6e64 696e 675f 7769 7468 6f75 745f  sending_without_
+00007d50: 7265 706c 790a 2020 2020 6966 2070 726f  reply.    if pro
+00007d60: 7465 6374 5f63 6f6e 7465 6e74 2069 7320  tect_content is 
+00007d70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00007d80: 2020 7061 796c 6f61 645b 2270 726f 7465    payload["prote
+00007d90: 6374 5f63 6f6e 7465 6e74 225d 203d 2070  ct_content"] = p
+00007da0: 726f 7465 6374 5f63 6f6e 7465 6e74 0a20  rotect_content. 
+00007db0: 2020 205f 6164 645f 6d65 7373 6167 655f     _add_message_
+00007dc0: 7468 7265 6164 5f69 6428 7061 796c 6f61  thread_id(payloa
+00007dd0: 642c 206d 6573 7361 6765 5f74 6872 6561  d, message_threa
+00007de0: 645f 6964 290a 2020 2020 7265 7475 726e  d_id).    return
+00007df0: 2061 7761 6974 205f 7265 7175 6573 7428   await _request(
+00007e00: 746f 6b65 6e2c 206d 6574 686f 645f 7572  token, method_ur
+00007e10: 6c2c 2070 6172 616d 733d 7061 796c 6f61  l, params=payloa
+00007e20: 642c 2066 696c 6573 3d66 696c 6573 2c20  d, files=files, 
+00007e30: 6d65 7468 6f64 3d22 706f 7374 2229 0a0a  method="post")..
+00007e40: 0a61 7379 6e63 2064 6566 2073 656e 645f  .async def send_
+00007e50: 6175 6469 6f28 0a20 2020 2074 6f6b 656e  audio(.    token
+00007e60: 2c0a 2020 2020 6368 6174 5f69 642c 0a20  ,.    chat_id,. 
+00007e70: 2020 2061 7564 696f 2c0a 2020 2020 6361     audio,.    ca
+00007e80: 7074 696f 6e3d 4e6f 6e65 2c0a 2020 2020  ption=None,.    
+00007e90: 6475 7261 7469 6f6e 3d4e 6f6e 652c 0a20  duration=None,. 
+00007ea0: 2020 2070 6572 666f 726d 6572 3d4e 6f6e     performer=Non
+00007eb0: 652c 0a20 2020 2074 6974 6c65 3d4e 6f6e  e,.    title=Non
+00007ec0: 652c 0a20 2020 2072 6570 6c79 5f74 6f5f  e,.    reply_to_
+00007ed0: 6d65 7373 6167 655f 6964 3d4e 6f6e 652c  message_id=None,
+00007ee0: 0a20 2020 2072 6570 6c79 5f6d 6172 6b75  .    reply_marku
+00007ef0: 703d 4e6f 6e65 2c0a 2020 2020 7061 7273  p=None,.    pars
+00007f00: 655f 6d6f 6465 3d4e 6f6e 652c 0a20 2020  e_mode=None,.   
+00007f10: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
+00007f20: 6174 696f 6e3d 4e6f 6e65 2c0a 2020 2020  ation=None,.    
+00007f30: 7469 6d65 6f75 743d 4e6f 6e65 2c0a 2020  timeout=None,.  
+00007f40: 2020 7468 756d 623d 4e6f 6e65 2c0a 2020    thumb=None,.  
+00007f50: 2020 6361 7074 696f 6e5f 656e 7469 7469    caption_entiti
+00007f60: 6573 3d4e 6f6e 652c 0a20 2020 2061 6c6c  es=None,.    all
+00007f70: 6f77 5f73 656e 6469 6e67 5f77 6974 686f  ow_sending_witho
+00007f80: 7574 5f72 6570 6c79 3d4e 6f6e 652c 0a20  ut_reply=None,. 
+00007f90: 2020 2070 726f 7465 6374 5f63 6f6e 7465     protect_conte
+00007fa0: 6e74 3d4e 6f6e 652c 0a20 2020 206d 6573  nt=None,.    mes
+00007fb0: 7361 6765 5f74 6872 6561 645f 6964 3a20  sage_thread_id: 
+00007fc0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00007fd0: 4e6f 6e65 2c0a 293a 0a20 2020 206d 6574  None,.):.    met
+00007fe0: 686f 645f 7572 6c20 3d20 7222 7365 6e64  hod_url = r"send
+00007ff0: 4175 6469 6f22 0a20 2020 2070 6179 6c6f  Audio".    paylo
+00008000: 6164 203d 207b 2263 6861 745f 6964 223a  ad = {"chat_id":
+00008010: 2063 6861 745f 6964 7d0a 2020 2020 6669   chat_id}.    fi
+00008020: 6c65 7320 3d20 4e6f 6e65 0a20 2020 2069  les = None.    i
+00008030: 6620 6e6f 7420 7574 696c 2e69 735f 7374  f not util.is_st
+00008040: 7269 6e67 2861 7564 696f 293a 0a20 2020  ring(audio):.   
+00008050: 2020 2020 2066 696c 6573 203d 207b 2261       files = {"a
+00008060: 7564 696f 223a 2061 7564 696f 7d0a 2020  udio": audio}.  
+00008070: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00008080: 7061 796c 6f61 645b 2261 7564 696f 225d  payload["audio"]
+00008090: 203d 2061 7564 696f 0a20 2020 2069 6620   = audio.    if 
+000080a0: 6361 7074 696f 6e3a 0a20 2020 2020 2020  caption:.       
+000080b0: 2070 6179 6c6f 6164 5b22 6361 7074 696f   payload["captio
+000080c0: 6e22 5d20 3d20 6361 7074 696f 6e0a 2020  n"] = caption.  
+000080d0: 2020 6966 2064 7572 6174 696f 6e3a 0a20    if duration:. 
+000080e0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+000080f0: 6475 7261 7469 6f6e 225d 203d 2064 7572  duration"] = dur
+00008100: 6174 696f 6e0a 2020 2020 6966 2070 6572  ation.    if per
+00008110: 666f 726d 6572 3a0a 2020 2020 2020 2020  former:.        
+00008120: 7061 796c 6f61 645b 2270 6572 666f 726d  payload["perform
+00008130: 6572 225d 203d 2070 6572 666f 726d 6572  er"] = performer
+00008140: 0a20 2020 2069 6620 7469 746c 653a 0a20  .    if title:. 
+00008150: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+00008160: 7469 746c 6522 5d20 3d20 7469 746c 650a  title"] = title.
+00008170: 2020 2020 6966 2072 6570 6c79 5f74 6f5f      if reply_to_
+00008180: 6d65 7373 6167 655f 6964 3a0a 2020 2020  message_id:.    
+00008190: 2020 2020 7061 796c 6f61 645b 2272 6570      payload["rep
+000081a0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+000081b0: 225d 203d 2072 6570 6c79 5f74 6f5f 6d65  "] = reply_to_me
+000081c0: 7373 6167 655f 6964 0a20 2020 2069 6620  ssage_id.    if 
+000081d0: 7265 706c 795f 6d61 726b 7570 3a0a 2020  reply_markup:.  
+000081e0: 2020 2020 2020 7061 796c 6f61 645b 2272        payload["r
+000081f0: 6570 6c79 5f6d 6172 6b75 7022 5d20 3d20  eply_markup"] = 
+00008200: 6177 6169 7420 5f63 6f6e 7665 7274 5f6d  await _convert_m
+00008210: 6172 6b75 7028 7265 706c 795f 6d61 726b  arkup(reply_mark
+00008220: 7570 290a 2020 2020 6966 2070 6172 7365  up).    if parse
+00008230: 5f6d 6f64 653a 0a20 2020 2020 2020 2070  _mode:.        p
+00008240: 6179 6c6f 6164 5b22 7061 7273 655f 6d6f  ayload["parse_mo
+00008250: 6465 225d 203d 2070 6172 7365 5f6d 6f64  de"] = parse_mod
+00008260: 650a 2020 2020 6966 2064 6973 6162 6c65  e.    if disable
+00008270: 5f6e 6f74 6966 6963 6174 696f 6e20 6973  _notification is
+00008280: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00008290: 2020 2070 6179 6c6f 6164 5b22 6469 7361     payload["disa
+000082a0: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+000082b0: 225d 203d 2064 6973 6162 6c65 5f6e 6f74  "] = disable_not
+000082c0: 6966 6963 6174 696f 6e0a 2020 2020 6966  ification.    if
+000082d0: 2074 696d 656f 7574 3a0a 2020 2020 2020   timeout:.      
+000082e0: 2020 7061 796c 6f61 645b 2274 696d 656f    payload["timeo
+000082f0: 7574 225d 203d 2074 696d 656f 7574 0a20  ut"] = timeout. 
+00008300: 2020 2069 6620 7468 756d 623a 0a20 2020     if thumb:.   
+00008310: 2020 2020 2069 6620 6e6f 7420 7574 696c       if not util
+00008320: 2e69 735f 7374 7269 6e67 2874 6875 6d62  .is_string(thumb
+00008330: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00008340: 6620 6669 6c65 733a 0a20 2020 2020 2020  f files:.       
+00008350: 2020 2020 2020 2020 2066 696c 6573 5b22           files["
+00008360: 7468 756d 6222 5d20 3d20 7468 756d 620a  thumb"] = thumb.
+00008370: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00008380: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00008390: 2020 6669 6c65 7320 3d20 7b22 7468 756d    files = {"thum
+000083a0: 6222 3a20 7468 756d 627d 0a20 2020 2020  b": thumb}.     
+000083b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000083c0: 2020 2020 2070 6179 6c6f 6164 5b22 7468       payload["th
+000083d0: 756d 6222 5d20 3d20 7468 756d 620a 2020  umb"] = thumb.  
+000083e0: 2020 6966 2063 6170 7469 6f6e 5f65 6e74    if caption_ent
+000083f0: 6974 6965 733a 0a20 2020 2020 2020 2070  ities:.        p
+00008400: 6179 6c6f 6164 5b22 6361 7074 696f 6e5f  ayload["caption_
+00008410: 656e 7469 7469 6573 225d 203d 206a 736f  entities"] = jso
+00008420: 6e2e 6475 6d70 7328 7479 7065 732e 4d65  n.dumps(types.Me
+00008430: 7373 6167 6545 6e74 6974 792e 746f 5f6c  ssageEntity.to_l
+00008440: 6973 745f 6f66 5f64 6963 7473 2863 6170  ist_of_dicts(cap
+00008450: 7469 6f6e 5f65 6e74 6974 6965 7329 290a  tion_entities)).
+00008460: 2020 2020 6966 2061 6c6c 6f77 5f73 656e      if allow_sen
+00008470: 6469 6e67 5f77 6974 686f 7574 5f72 6570  ding_without_rep
+00008480: 6c79 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ly is not None:.
+00008490: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
+000084a0: 2261 6c6c 6f77 5f73 656e 6469 6e67 5f77  "allow_sending_w
+000084b0: 6974 686f 7574 5f72 6570 6c79 225d 203d  ithout_reply"] =
+000084c0: 2061 6c6c 6f77 5f73 656e 6469 6e67 5f77   allow_sending_w
+000084d0: 6974 686f 7574 5f72 6570 6c79 0a20 2020  ithout_reply.   
+000084e0: 2069 6620 7072 6f74 6563 745f 636f 6e74   if protect_cont
+000084f0: 656e 7420 6973 206e 6f74 204e 6f6e 653a  ent is not None:
+00008500: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+00008510: 5b22 7072 6f74 6563 745f 636f 6e74 656e  ["protect_conten
+00008520: 7422 5d20 3d20 7072 6f74 6563 745f 636f  t"] = protect_co
+00008530: 6e74 656e 740a 2020 2020 5f61 6464 5f6d  ntent.    _add_m
+00008540: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+00008550: 2870 6179 6c6f 6164 2c20 6d65 7373 6167  (payload, messag
+00008560: 655f 7468 7265 6164 5f69 6429 0a20 2020  e_thread_id).   
+00008570: 2072 6574 7572 6e20 6177 6169 7420 5f72   return await _r
+00008580: 6571 7565 7374 2874 6f6b 656e 2c20 6d65  equest(token, me
+00008590: 7468 6f64 5f75 726c 2c20 7061 7261 6d73  thod_url, params
+000085a0: 3d70 6179 6c6f 6164 2c20 6669 6c65 733d  =payload, files=
+000085b0: 6669 6c65 732c 206d 6574 686f 643d 2270  files, method="p
+000085c0: 6f73 7422 290a 0a0a 6173 796e 6320 6465  ost")...async de
+000085d0: 6620 7365 6e64 5f64 6174 6128 0a20 2020  f send_data(.   
+000085e0: 2074 6f6b 656e 2c0a 2020 2020 6368 6174   token,.    chat
+000085f0: 5f69 642c 0a20 2020 2064 6174 612c 0a20  _id,.    data,. 
+00008600: 2020 2064 6174 615f 7479 7065 2c0a 2020     data_type,.  
+00008610: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
+00008620: 6765 5f69 643d 4e6f 6e65 2c0a 2020 2020  ge_id=None,.    
+00008630: 7265 706c 795f 6d61 726b 7570 3d4e 6f6e  reply_markup=Non
+00008640: 652c 0a20 2020 2070 6172 7365 5f6d 6f64  e,.    parse_mod
+00008650: 653d 4e6f 6e65 2c0a 2020 2020 6469 7361  e=None,.    disa
+00008660: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+00008670: 3d4e 6f6e 652c 0a20 2020 2074 696d 656f  =None,.    timeo
+00008680: 7574 3d4e 6f6e 652c 0a20 2020 2063 6170  ut=None,.    cap
+00008690: 7469 6f6e 3d4e 6f6e 652c 0a20 2020 2074  tion=None,.    t
+000086a0: 6875 6d62 3d4e 6f6e 652c 0a20 2020 2063  humb=None,.    c
+000086b0: 6170 7469 6f6e 5f65 6e74 6974 6965 733d  aption_entities=
+000086c0: 4e6f 6e65 2c0a 2020 2020 616c 6c6f 775f  None,.    allow_
+000086d0: 7365 6e64 696e 675f 7769 7468 6f75 745f  sending_without_
+000086e0: 7265 706c 793d 4e6f 6e65 2c0a 2020 2020  reply=None,.    
+000086f0: 6469 7361 626c 655f 636f 6e74 656e 745f  disable_content_
+00008700: 7479 7065 5f64 6574 6563 7469 6f6e 3d4e  type_detection=N
+00008710: 6f6e 652c 0a20 2020 2076 6973 6962 6c65  one,.    visible
+00008720: 5f66 696c 655f 6e61 6d65 3d4e 6f6e 652c  _file_name=None,
+00008730: 0a20 2020 2070 726f 7465 6374 5f63 6f6e  .    protect_con
+00008740: 7465 6e74 3d4e 6f6e 652c 0a20 2020 206d  tent=None,.    m
+00008750: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+00008760: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+00008770: 3d20 4e6f 6e65 2c0a 293a 0a20 2020 206d  = None,.):.    m
+00008780: 6574 686f 645f 7572 6c20 3d20 6177 6169  ethod_url = awai
+00008790: 7420 6765 745f 6d65 7468 6f64 5f62 795f  t get_method_by_
+000087a0: 7479 7065 2864 6174 615f 7479 7065 290a  type(data_type).
+000087b0: 2020 2020 7061 796c 6f61 6420 3d20 7b22      payload = {"
+000087c0: 6368 6174 5f69 6422 3a20 6368 6174 5f69  chat_id": chat_i
+000087d0: 647d 0a20 2020 2066 696c 6573 203d 204e  d}.    files = N
+000087e0: 6f6e 650a 2020 2020 6966 206e 6f74 2075  one.    if not u
+000087f0: 7469 6c2e 6973 5f73 7472 696e 6728 6461  til.is_string(da
+00008800: 7461 293a 0a20 2020 2020 2020 2066 696c  ta):.        fil
+00008810: 655f 6461 7461 203d 2064 6174 610a 2020  e_data = data.  
+00008820: 2020 2020 2020 6966 2076 6973 6962 6c65        if visible
+00008830: 5f66 696c 655f 6e61 6d65 3a0a 2020 2020  _file_name:.    
+00008840: 2020 2020 2020 2020 6669 6c65 5f64 6174          file_dat
+00008850: 6120 3d20 2876 6973 6962 6c65 5f66 696c  a = (visible_fil
+00008860: 655f 6e61 6d65 2c20 6461 7461 290a 2020  e_name, data).  
+00008870: 2020 2020 2020 6669 6c65 7320 3d20 7b64        files = {d
+00008880: 6174 615f 7479 7065 3a20 6669 6c65 5f64  ata_type: file_d
+00008890: 6174 617d 0a20 2020 2065 6c73 653a 0a20  ata}.    else:. 
+000088a0: 2020 2020 2020 2070 6179 6c6f 6164 5b64         payload[d
+000088b0: 6174 615f 7479 7065 5d20 3d20 6461 7461  ata_type] = data
+000088c0: 0a20 2020 2069 6620 7265 706c 795f 746f  .    if reply_to
+000088d0: 5f6d 6573 7361 6765 5f69 643a 0a20 2020  _message_id:.   
+000088e0: 2020 2020 2070 6179 6c6f 6164 5b22 7265       payload["re
+000088f0: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
+00008900: 6422 5d20 3d20 7265 706c 795f 746f 5f6d  d"] = reply_to_m
+00008910: 6573 7361 6765 5f69 640a 2020 2020 6966  essage_id.    if
+00008920: 2072 6570 6c79 5f6d 6172 6b75 703a 0a20   reply_markup:. 
+00008930: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+00008940: 7265 706c 795f 6d61 726b 7570 225d 203d  reply_markup"] =
+00008950: 2061 7761 6974 205f 636f 6e76 6572 745f   await _convert_
+00008960: 6d61 726b 7570 2872 6570 6c79 5f6d 6172  markup(reply_mar
+00008970: 6b75 7029 0a20 2020 2069 6620 7061 7273  kup).    if pars
+00008980: 655f 6d6f 6465 2061 6e64 2064 6174 615f  e_mode and data_
+00008990: 7479 7065 203d 3d20 2264 6f63 756d 656e  type == "documen
+000089a0: 7422 3a0a 2020 2020 2020 2020 7061 796c  t":.        payl
+000089b0: 6f61 645b 2270 6172 7365 5f6d 6f64 6522  oad["parse_mode"
+000089c0: 5d20 3d20 7061 7273 655f 6d6f 6465 0a20  ] = parse_mode. 
+000089d0: 2020 2069 6620 6469 7361 626c 655f 6e6f     if disable_no
+000089e0: 7469 6669 6361 7469 6f6e 2069 7320 6e6f  tification is no
+000089f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00008a00: 7061 796c 6f61 645b 2264 6973 6162 6c65  payload["disable
+00008a10: 5f6e 6f74 6966 6963 6174 696f 6e22 5d20  _notification"] 
+00008a20: 3d20 6469 7361 626c 655f 6e6f 7469 6669  = disable_notifi
+00008a30: 6361 7469 6f6e 0a20 2020 2069 6620 7469  cation.    if ti
+00008a40: 6d65 6f75 743a 0a20 2020 2020 2020 2070  meout:.        p
+00008a50: 6179 6c6f 6164 5b22 7469 6d65 6f75 7422  ayload["timeout"
+00008a60: 5d20 3d20 7469 6d65 6f75 740a 2020 2020  ] = timeout.    
+00008a70: 6966 2063 6170 7469 6f6e 3a0a 2020 2020  if caption:.    
+00008a80: 2020 2020 7061 796c 6f61 645b 2263 6170      payload["cap
+00008a90: 7469 6f6e 225d 203d 2063 6170 7469 6f6e  tion"] = caption
+00008aa0: 0a20 2020 2069 6620 7468 756d 623a 0a20  .    if thumb:. 
+00008ab0: 2020 2020 2020 2069 6620 6e6f 7420 7574         if not ut
+00008ac0: 696c 2e69 735f 7374 7269 6e67 2874 6875  il.is_string(thu
+00008ad0: 6d62 293a 0a20 2020 2020 2020 2020 2020  mb):.           
+00008ae0: 2069 6620 6669 6c65 733a 0a20 2020 2020   if files:.     
+00008af0: 2020 2020 2020 2020 2020 2066 696c 6573             files
+00008b00: 5b22 7468 756d 6222 5d20 3d20 7468 756d  ["thumb"] = thum
+00008b10: 620a 2020 2020 2020 2020 2020 2020 656c  b.            el
+00008b20: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00008b30: 2020 2020 6669 6c65 7320 3d20 7b22 7468      files = {"th
+00008b40: 756d 6222 3a20 7468 756d 627d 0a20 2020  umb": thumb}.   
+00008b50: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00008b60: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+00008b70: 7468 756d 6222 5d20 3d20 7468 756d 620a  thumb"] = thumb.
+00008b80: 2020 2020 6966 2063 6170 7469 6f6e 5f65      if caption_e
+00008b90: 6e74 6974 6965 733a 0a20 2020 2020 2020  ntities:.       
+00008ba0: 2070 6179 6c6f 6164 5b22 6361 7074 696f   payload["captio
+00008bb0: 6e5f 656e 7469 7469 6573 225d 203d 206a  n_entities"] = j
+00008bc0: 736f 6e2e 6475 6d70 7328 7479 7065 732e  son.dumps(types.
+00008bd0: 4d65 7373 6167 6545 6e74 6974 792e 746f  MessageEntity.to
+00008be0: 5f6c 6973 745f 6f66 5f64 6963 7473 2863  _list_of_dicts(c
+00008bf0: 6170 7469 6f6e 5f65 6e74 6974 6965 7329  aption_entities)
+00008c00: 290a 2020 2020 6966 2061 6c6c 6f77 5f73  ).    if allow_s
+00008c10: 656e 6469 6e67 5f77 6974 686f 7574 5f72  ending_without_r
+00008c20: 6570 6c79 2069 7320 6e6f 7420 4e6f 6e65  eply is not None
+00008c30: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+00008c40: 645b 2261 6c6c 6f77 5f73 656e 6469 6e67  d["allow_sending
+00008c50: 5f77 6974 686f 7574 5f72 6570 6c79 225d  _without_reply"]
+00008c60: 203d 2061 6c6c 6f77 5f73 656e 6469 6e67   = allow_sending
+00008c70: 5f77 6974 686f 7574 5f72 6570 6c79 0a20  _without_reply. 
+00008c80: 2020 2069 6620 7072 6f74 6563 745f 636f     if protect_co
+00008c90: 6e74 656e 7420 6973 206e 6f74 204e 6f6e  ntent is not Non
+00008ca0: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
+00008cb0: 6164 5b22 7072 6f74 6563 745f 636f 6e74  ad["protect_cont
+00008cc0: 656e 7422 5d20 3d20 7072 6f74 6563 745f  ent"] = protect_
+00008cd0: 636f 6e74 656e 740a 2020 2020 6966 206d  content.    if m
+00008ce0: 6574 686f 645f 7572 6c20 3d3d 2022 7365  ethod_url == "se
+00008cf0: 6e64 446f 6375 6d65 6e74 2220 616e 6420  ndDocument" and 
+00008d00: 6469 7361 626c 655f 636f 6e74 656e 745f  disable_content_
+00008d10: 7479 7065 5f64 6574 6563 7469 6f6e 2069  type_detection i
+00008d20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00008d30: 2020 2020 7061 796c 6f61 645b 2264 6973      payload["dis
+00008d40: 6162 6c65 5f63 6f6e 7465 6e74 5f74 7970  able_content_typ
+00008d50: 655f 6465 7465 6374 696f 6e22 5d20 3d20  e_detection"] = 
+00008d60: 6469 7361 626c 655f 636f 6e74 656e 745f  disable_content_
+00008d70: 7479 7065 5f64 6574 6563 7469 6f6e 0a20  type_detection. 
+00008d80: 2020 205f 6164 645f 6d65 7373 6167 655f     _add_message_
+00008d90: 7468 7265 6164 5f69 6428 7061 796c 6f61  thread_id(payloa
+00008da0: 642c 206d 6573 7361 6765 5f74 6872 6561  d, message_threa
+00008db0: 645f 6964 290a 2020 2020 7265 7475 726e  d_id).    return
+00008dc0: 2061 7761 6974 205f 7265 7175 6573 7428   await _request(
+00008dd0: 746f 6b65 6e2c 206d 6574 686f 645f 7572  token, method_ur
+00008de0: 6c2c 2070 6172 616d 733d 7061 796c 6f61  l, params=payloa
+00008df0: 642c 2066 696c 6573 3d66 696c 6573 2c20  d, files=files, 
+00008e00: 6d65 7468 6f64 3d22 706f 7374 2229 0a0a  method="post")..
+00008e10: 0a61 7379 6e63 2064 6566 2067 6574 5f6d  .async def get_m
+00008e20: 6574 686f 645f 6279 5f74 7970 6528 6461  ethod_by_type(da
+00008e30: 7461 5f74 7970 6529 3a0a 2020 2020 6966  ta_type):.    if
+00008e40: 2064 6174 615f 7479 7065 203d 3d20 2264   data_type == "d
+00008e50: 6f63 756d 656e 7422 3a0a 2020 2020 2020  ocument":.      
+00008e60: 2020 7265 7475 726e 2072 2273 656e 6444    return r"sendD
+00008e70: 6f63 756d 656e 7422 0a20 2020 2069 6620  ocument".    if 
+00008e80: 6461 7461 5f74 7970 6520 3d3d 2022 7374  data_type == "st
+00008e90: 6963 6b65 7222 3a0a 2020 2020 2020 2020  icker":.        
+00008ea0: 7265 7475 726e 2072 2273 656e 6453 7469  return r"sendSti
+00008eb0: 636b 6572 220a 0a0a 6173 796e 6320 6465  cker"...async de
+00008ec0: 6620 6261 6e5f 6368 6174 5f6d 656d 6265  f ban_chat_membe
+00008ed0: 7228 746f 6b65 6e2c 2063 6861 745f 6964  r(token, chat_id
+00008ee0: 2c20 7573 6572 5f69 642c 2075 6e74 696c  , user_id, until
+00008ef0: 5f64 6174 653d 4e6f 6e65 2c20 7265 766f  _date=None, revo
+00008f00: 6b65 5f6d 6573 7361 6765 733d 4e6f 6e65  ke_messages=None
+00008f10: 293a 0a20 2020 206d 6574 686f 645f 7572  ):.    method_ur
+00008f20: 6c20 3d20 2262 616e 4368 6174 4d65 6d62  l = "banChatMemb
+00008f30: 6572 220a 2020 2020 7061 796c 6f61 6420  er".    payload 
+00008f40: 3d20 7b22 6368 6174 5f69 6422 3a20 6368  = {"chat_id": ch
+00008f50: 6174 5f69 642c 2022 7573 6572 5f69 6422  at_id, "user_id"
+00008f60: 3a20 7573 6572 5f69 647d 0a20 2020 2069  : user_id}.    i
+00008f70: 6620 6973 696e 7374 616e 6365 2875 6e74  f isinstance(unt
+00008f80: 696c 5f64 6174 652c 2064 6174 6574 696d  il_date, datetim
+00008f90: 6529 3a0a 2020 2020 2020 2020 7061 796c  e):.        payl
+00008fa0: 6f61 645b 2275 6e74 696c 5f64 6174 6522  oad["until_date"
+00008fb0: 5d20 3d20 756e 7469 6c5f 6461 7465 2e74  ] = until_date.t
+00008fc0: 696d 6573 7461 6d70 2829 0a20 2020 2065  imestamp().    e
+00008fd0: 6c73 653a 0a20 2020 2020 2020 2070 6179  lse:.        pay
+00008fe0: 6c6f 6164 5b22 756e 7469 6c5f 6461 7465  load["until_date
+00008ff0: 225d 203d 2075 6e74 696c 5f64 6174 650a  "] = until_date.
+00009000: 2020 2020 6966 2072 6576 6f6b 655f 6d65      if revoke_me
+00009010: 7373 6167 6573 2069 7320 6e6f 7420 4e6f  ssages is not No
+00009020: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
+00009030: 6f61 645b 2272 6576 6f6b 655f 6d65 7373  oad["revoke_mess
+00009040: 6167 6573 225d 203d 2072 6576 6f6b 655f  ages"] = revoke_
+00009050: 6d65 7373 6167 6573 0a20 2020 2072 6574  messages.    ret
+00009060: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
+00009070: 7374 2874 6f6b 656e 2c20 6d65 7468 6f64  st(token, method
+00009080: 5f75 726c 2c20 7061 7261 6d73 3d70 6179  _url, params=pay
+00009090: 6c6f 6164 2c20 6d65 7468 6f64 3d22 706f  load, method="po
+000090a0: 7374 2229 0a0a 0a61 7379 6e63 2064 6566  st")...async def
+000090b0: 2075 6e62 616e 5f63 6861 745f 6d65 6d62   unban_chat_memb
+000090c0: 6572 2874 6f6b 656e 2c20 6368 6174 5f69  er(token, chat_i
+000090d0: 642c 2075 7365 725f 6964 2c20 6f6e 6c79  d, user_id, only
+000090e0: 5f69 665f 6261 6e6e 6564 293a 0a20 2020  _if_banned):.   
+000090f0: 206d 6574 686f 645f 7572 6c20 3d20 2275   method_url = "u
+00009100: 6e62 616e 4368 6174 4d65 6d62 6572 220a  nbanChatMember".
+00009110: 2020 2020 7061 796c 6f61 6420 3d20 7b22      payload = {"
+00009120: 6368 6174 5f69 6422 3a20 6368 6174 5f69  chat_id": chat_i
+00009130: 642c 2022 7573 6572 5f69 6422 3a20 7573  d, "user_id": us
+00009140: 6572 5f69 647d 0a20 2020 2069 6620 6f6e  er_id}.    if on
+00009150: 6c79 5f69 665f 6261 6e6e 6564 2069 7320  ly_if_banned is 
+00009160: 6e6f 7420 4e6f 6e65 3a20 2023 204e 6f6e  not None:  # Non
+00009170: 6520 2f20 5472 7565 202f 2046 616c 7365  e / True / False
+00009180: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+00009190: 5b22 6f6e 6c79 5f69 665f 6261 6e6e 6564  ["only_if_banned
+000091a0: 225d 203d 206f 6e6c 795f 6966 5f62 616e  "] = only_if_ban
+000091b0: 6e65 640a 2020 2020 7265 7475 726e 2061  ned.    return a
+000091c0: 7761 6974 205f 7265 7175 6573 7428 746f  wait _request(to
+000091d0: 6b65 6e2c 206d 6574 686f 645f 7572 6c2c  ken, method_url,
+000091e0: 2070 6172 616d 733d 7061 796c 6f61 642c   params=payload,
+000091f0: 206d 6574 686f 643d 2270 6f73 7422 290a   method="post").
+00009200: 0a0a 6173 796e 6320 6465 6620 7265 7374  ..async def rest
+00009210: 7269 6374 5f63 6861 745f 6d65 6d62 6572  rict_chat_member
+00009220: 280a 2020 2020 746f 6b65 6e2c 0a20 2020  (.    token,.   
+00009230: 2063 6861 745f 6964 2c0a 2020 2020 7573   chat_id,.    us
+00009240: 6572 5f69 642c 0a20 2020 2070 6572 6d69  er_id,.    permi
+00009250: 7373 696f 6e73 2c0a 2020 2020 756e 7469  ssions,.    unti
+00009260: 6c5f 6461 7465 3d4e 6f6e 652c 0a20 2020  l_date=None,.   
+00009270: 2075 7365 5f69 6e64 6570 656e 6465 6e74   use_independent
+00009280: 5f63 6861 745f 7065 726d 6973 7369 6f6e  _chat_permission
+00009290: 733d 4e6f 6e65 2c0a 293a 0a20 2020 206d  s=None,.):.    m
+000092a0: 6574 686f 645f 7572 6c20 3d20 2272 6573  ethod_url = "res
+000092b0: 7472 6963 7443 6861 744d 656d 6265 7222  trictChatMember"
+000092c0: 0a20 2020 2070 6179 6c6f 6164 203d 207b  .    payload = {
+000092d0: 2263 6861 745f 6964 223a 2063 6861 745f  "chat_id": chat_
+000092e0: 6964 2c20 2275 7365 725f 6964 223a 2075  id, "user_id": u
+000092f0: 7365 725f 6964 2c20 2270 6572 6d69 7373  ser_id, "permiss
+00009300: 696f 6e73 223a 2070 6572 6d69 7373 696f  ions": permissio
+00009310: 6e73 2e74 6f5f 6a73 6f6e 2829 7d0a 2020  ns.to_json()}.  
+00009320: 2020 6966 2075 7365 5f69 6e64 6570 656e    if use_indepen
+00009330: 6465 6e74 5f63 6861 745f 7065 726d 6973  dent_chat_permis
+00009340: 7369 6f6e 7320 6973 206e 6f74 204e 6f6e  sions is not Non
+00009350: 653a 0a20 2020 2020 2020 2070 6572 6d69  e:.        permi
+00009360: 7373 696f 6e73 5b22 7573 655f 696e 6465  ssions["use_inde
+00009370: 7065 6e64 656e 745f 6368 6174 5f70 6572  pendent_chat_per
+00009380: 6d69 7373 696f 6e73 225d 203d 2075 7365  missions"] = use
+00009390: 5f69 6e64 6570 656e 6465 6e74 5f63 6861  _independent_cha
+000093a0: 745f 7065 726d 6973 7369 6f6e 730a 2020  t_permissions.  
+000093b0: 2020 6966 2075 6e74 696c 5f64 6174 6520    if until_date 
+000093c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000093d0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+000093e0: 6365 2875 6e74 696c 5f64 6174 652c 2064  ce(until_date, d
+000093f0: 6174 6574 696d 6529 3a0a 2020 2020 2020  atetime):.      
+00009400: 2020 2020 2020 7061 796c 6f61 645b 2275        payload["u
+00009410: 6e74 696c 5f64 6174 6522 5d20 3d20 756e  ntil_date"] = un
+00009420: 7469 6c5f 6461 7465 2e74 696d 6573 7461  til_date.timesta
+00009430: 6d70 2829 0a20 2020 2020 2020 2065 6c73  mp().        els
+00009440: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+00009450: 6179 6c6f 6164 5b22 756e 7469 6c5f 6461  ayload["until_da
+00009460: 7465 225d 203d 2075 6e74 696c 5f64 6174  te"] = until_dat
+00009470: 650a 2020 2020 7265 7475 726e 2061 7761  e.    return awa
+00009480: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
+00009490: 6e2c 206d 6574 686f 645f 7572 6c2c 2070  n, method_url, p
+000094a0: 6172 616d 733d 7061 796c 6f61 642c 206d  arams=payload, m
+000094b0: 6574 686f 643d 2270 6f73 7422 290a 0a0a  ethod="post")...
+000094c0: 6173 796e 6320 6465 6620 7072 6f6d 6f74  async def promot
+000094d0: 655f 6368 6174 5f6d 656d 6265 7228 0a20  e_chat_member(. 
+000094e0: 2020 2074 6f6b 656e 2c0a 2020 2020 6368     token,.    ch
+000094f0: 6174 5f69 642c 0a20 2020 2075 7365 725f  at_id,.    user_
+00009500: 6964 2c0a 2020 2020 6361 6e5f 6368 616e  id,.    can_chan
+00009510: 6765 5f69 6e66 6f3d 4e6f 6e65 2c0a 2020  ge_info=None,.  
+00009520: 2020 6361 6e5f 706f 7374 5f6d 6573 7361    can_post_messa
+00009530: 6765 733d 4e6f 6e65 2c0a 2020 2020 6361  ges=None,.    ca
+00009540: 6e5f 6564 6974 5f6d 6573 7361 6765 733d  n_edit_messages=
+00009550: 4e6f 6e65 2c0a 2020 2020 6361 6e5f 6465  None,.    can_de
+00009560: 6c65 7465 5f6d 6573 7361 6765 733d 4e6f  lete_messages=No
+00009570: 6e65 2c0a 2020 2020 6361 6e5f 696e 7669  ne,.    can_invi
+00009580: 7465 5f75 7365 7273 3d4e 6f6e 652c 0a20  te_users=None,. 
+00009590: 2020 2063 616e 5f72 6573 7472 6963 745f     can_restrict_
+000095a0: 6d65 6d62 6572 733d 4e6f 6e65 2c0a 2020  members=None,.  
+000095b0: 2020 6361 6e5f 7069 6e5f 6d65 7373 6167    can_pin_messag
+000095c0: 6573 3d4e 6f6e 652c 0a20 2020 2063 616e  es=None,.    can
+000095d0: 5f70 726f 6d6f 7465 5f6d 656d 6265 7273  _promote_members
+000095e0: 3d4e 6f6e 652c 0a20 2020 2069 735f 616e  =None,.    is_an
+000095f0: 6f6e 796d 6f75 733d 4e6f 6e65 2c0a 2020  onymous=None,.  
+00009600: 2020 6361 6e5f 6d61 6e61 6765 5f63 6861    can_manage_cha
+00009610: 743d 4e6f 6e65 2c0a 2020 2020 6361 6e5f  t=None,.    can_
+00009620: 6d61 6e61 6765 5f76 6964 656f 5f63 6861  manage_video_cha
+00009630: 7473 3d4e 6f6e 652c 0a20 2020 2063 616e  ts=None,.    can
+00009640: 5f6d 616e 6167 655f 746f 7069 6373 3d4e  _manage_topics=N
+00009650: 6f6e 652c 0a29 3a0a 2020 2020 6d65 7468  one,.):.    meth
+00009660: 6f64 5f75 726c 203d 2022 7072 6f6d 6f74  od_url = "promot
+00009670: 6543 6861 744d 656d 6265 7222 0a20 2020  eChatMember".   
+00009680: 2070 6179 6c6f 6164 203d 207b 2263 6861   payload = {"cha
+00009690: 745f 6964 223a 2063 6861 745f 6964 2c20  t_id": chat_id, 
+000096a0: 2275 7365 725f 6964 223a 2075 7365 725f  "user_id": user_
+000096b0: 6964 7d0a 2020 2020 6966 2063 616e 5f63  id}.    if can_c
+000096c0: 6861 6e67 655f 696e 666f 2069 7320 6e6f  hange_info is no
+000096d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000096e0: 7061 796c 6f61 645b 2263 616e 5f63 6861  payload["can_cha
+000096f0: 6e67 655f 696e 666f 225d 203d 2063 616e  nge_info"] = can
+00009700: 5f63 6861 6e67 655f 696e 666f 0a20 2020  _change_info.   
+00009710: 2069 6620 6361 6e5f 706f 7374 5f6d 6573   if can_post_mes
+00009720: 7361 6765 7320 6973 206e 6f74 204e 6f6e  sages is not Non
+00009730: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
+00009740: 6164 5b22 6361 6e5f 706f 7374 5f6d 6573  ad["can_post_mes
+00009750: 7361 6765 7322 5d20 3d20 6361 6e5f 706f  sages"] = can_po
+00009760: 7374 5f6d 6573 7361 6765 730a 2020 2020  st_messages.    
+00009770: 6966 2063 616e 5f65 6469 745f 6d65 7373  if can_edit_mess
+00009780: 6167 6573 2069 7320 6e6f 7420 4e6f 6e65  ages is not None
+00009790: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+000097a0: 645b 2263 616e 5f65 6469 745f 6d65 7373  d["can_edit_mess
+000097b0: 6167 6573 225d 203d 2063 616e 5f65 6469  ages"] = can_edi
+000097c0: 745f 6d65 7373 6167 6573 0a20 2020 2069  t_messages.    i
+000097d0: 6620 6361 6e5f 6465 6c65 7465 5f6d 6573  f can_delete_mes
+000097e0: 7361 6765 7320 6973 206e 6f74 204e 6f6e  sages is not Non
+000097f0: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
+00009800: 6164 5b22 6361 6e5f 6465 6c65 7465 5f6d  ad["can_delete_m
+00009810: 6573 7361 6765 7322 5d20 3d20 6361 6e5f  essages"] = can_
+00009820: 6465 6c65 7465 5f6d 6573 7361 6765 730a  delete_messages.
+00009830: 2020 2020 6966 2063 616e 5f69 6e76 6974      if can_invit
+00009840: 655f 7573 6572 7320 6973 206e 6f74 204e  e_users is not N
+00009850: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
+00009860: 6c6f 6164 5b22 6361 6e5f 696e 7669 7465  load["can_invite
+00009870: 5f75 7365 7273 225d 203d 2063 616e 5f69  _users"] = can_i
+00009880: 6e76 6974 655f 7573 6572 730a 2020 2020  nvite_users.    
+00009890: 6966 2063 616e 5f72 6573 7472 6963 745f  if can_restrict_
+000098a0: 6d65 6d62 6572 7320 6973 206e 6f74 204e  members is not N
+000098b0: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
+000098c0: 6c6f 6164 5b22 6361 6e5f 7265 7374 7269  load["can_restri
+000098d0: 6374 5f6d 656d 6265 7273 225d 203d 2063  ct_members"] = c
+000098e0: 616e 5f72 6573 7472 6963 745f 6d65 6d62  an_restrict_memb
+000098f0: 6572 730a 2020 2020 6966 2063 616e 5f70  ers.    if can_p
+00009900: 696e 5f6d 6573 7361 6765 7320 6973 206e  in_messages is n
+00009910: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00009920: 2070 6179 6c6f 6164 5b22 6361 6e5f 7069   payload["can_pi
+00009930: 6e5f 6d65 7373 6167 6573 225d 203d 2063  n_messages"] = c
+00009940: 616e 5f70 696e 5f6d 6573 7361 6765 730a  an_pin_messages.
+00009950: 2020 2020 6966 2063 616e 5f70 726f 6d6f      if can_promo
+00009960: 7465 5f6d 656d 6265 7273 2069 7320 6e6f  te_members is no
+00009970: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00009980: 7061 796c 6f61 645b 2263 616e 5f70 726f  payload["can_pro
+00009990: 6d6f 7465 5f6d 656d 6265 7273 225d 203d  mote_members"] =
+000099a0: 2063 616e 5f70 726f 6d6f 7465 5f6d 656d   can_promote_mem
+000099b0: 6265 7273 0a20 2020 2069 6620 6973 5f61  bers.    if is_a
+000099c0: 6e6f 6e79 6d6f 7573 2069 7320 6e6f 7420  nonymous is not 
+000099d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
+000099e0: 796c 6f61 645b 2269 735f 616e 6f6e 796d  yload["is_anonym
+000099f0: 6f75 7322 5d20 3d20 6973 5f61 6e6f 6e79  ous"] = is_anony
+00009a00: 6d6f 7573 0a20 2020 2069 6620 6361 6e5f  mous.    if can_
+00009a10: 6d61 6e61 6765 5f63 6861 7420 6973 206e  manage_chat is n
+00009a20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00009a30: 2070 6179 6c6f 6164 5b22 6361 6e5f 6d61   payload["can_ma
+00009a40: 6e61 6765 5f63 6861 7422 5d20 3d20 6361  nage_chat"] = ca
+00009a50: 6e5f 6d61 6e61 6765 5f63 6861 740a 2020  n_manage_chat.  
+00009a60: 2020 6966 2063 616e 5f6d 616e 6167 655f    if can_manage_
+00009a70: 7669 6465 6f5f 6368 6174 7320 6973 206e  video_chats is n
+00009a80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00009a90: 2070 6179 6c6f 6164 5b22 6361 6e5f 6d61   payload["can_ma
+00009aa0: 6e61 6765 5f76 6964 656f 5f63 6861 7473  nage_video_chats
+00009ab0: 225d 203d 2063 616e 5f6d 616e 6167 655f  "] = can_manage_
+00009ac0: 7669 6465 6f5f 6368 6174 730a 2020 2020  video_chats.    
+00009ad0: 6966 2063 616e 5f6d 616e 6167 655f 746f  if can_manage_to
+00009ae0: 7069 6373 2069 7320 6e6f 7420 4e6f 6e65  pics is not None
+00009af0: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+00009b00: 645b 2263 616e 5f6d 616e 6167 655f 746f  d["can_manage_to
+00009b10: 7069 6373 225d 203d 2063 616e 5f6d 616e  pics"] = can_man
+00009b20: 6167 655f 746f 7069 6373 0a20 2020 2072  age_topics.    r
+00009b30: 6574 7572 6e20 6177 6169 7420 5f72 6571  eturn await _req
+00009b40: 7565 7374 2874 6f6b 656e 2c20 6d65 7468  uest(token, meth
+00009b50: 6f64 5f75 726c 2c20 7061 7261 6d73 3d70  od_url, params=p
+00009b60: 6179 6c6f 6164 2c20 6d65 7468 6f64 3d22  ayload, method="
+00009b70: 706f 7374 2229 0a0a 0a61 7379 6e63 2064  post")...async d
+00009b80: 6566 2073 6574 5f63 6861 745f 6164 6d69  ef set_chat_admi
+00009b90: 6e69 7374 7261 746f 725f 6375 7374 6f6d  nistrator_custom
+00009ba0: 5f74 6974 6c65 2874 6f6b 656e 2c20 6368  _title(token, ch
+00009bb0: 6174 5f69 642c 2075 7365 725f 6964 2c20  at_id, user_id, 
+00009bc0: 6375 7374 6f6d 5f74 6974 6c65 293a 0a20  custom_title):. 
+00009bd0: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
+00009be0: 2273 6574 4368 6174 4164 6d69 6e69 7374  "setChatAdminist
+00009bf0: 7261 746f 7243 7573 746f 6d54 6974 6c65  ratorCustomTitle
+00009c00: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
+00009c10: 7b22 6368 6174 5f69 6422 3a20 6368 6174  {"chat_id": chat
+00009c20: 5f69 642c 2022 7573 6572 5f69 6422 3a20  _id, "user_id": 
+00009c30: 7573 6572 5f69 642c 2022 6375 7374 6f6d  user_id, "custom
+00009c40: 5f74 6974 6c65 223a 2063 7573 746f 6d5f  _title": custom_
+00009c50: 7469 746c 657d 0a20 2020 2072 6574 7572  title}.    retur
+00009c60: 6e20 6177 6169 7420 5f72 6571 7565 7374  n await _request
+00009c70: 2874 6f6b 656e 2c20 6d65 7468 6f64 5f75  (token, method_u
+00009c80: 726c 2c20 7061 7261 6d73 3d70 6179 6c6f  rl, params=paylo
+00009c90: 6164 2c20 6d65 7468 6f64 3d22 706f 7374  ad, method="post
+00009ca0: 2229 0a0a 0a61 7379 6e63 2064 6566 2062  ")...async def b
+00009cb0: 616e 5f63 6861 745f 7365 6e64 6572 5f63  an_chat_sender_c
+00009cc0: 6861 7428 746f 6b65 6e2c 2063 6861 745f  hat(token, chat_
+00009cd0: 6964 2c20 7365 6e64 6572 5f63 6861 745f  id, sender_chat_
+00009ce0: 6964 293a 0a20 2020 206d 6574 686f 645f  id):.    method_
+00009cf0: 7572 6c20 3d20 2262 616e 4368 6174 5365  url = "banChatSe
+00009d00: 6e64 6572 4368 6174 220a 2020 2020 7061  nderChat".    pa
+00009d10: 796c 6f61 6420 3d20 7b22 6368 6174 5f69  yload = {"chat_i
+00009d20: 6422 3a20 6368 6174 5f69 642c 2022 7365  d": chat_id, "se
+00009d30: 6e64 6572 5f63 6861 745f 6964 223a 2073  nder_chat_id": s
+00009d40: 656e 6465 725f 6368 6174 5f69 647d 0a20  ender_chat_id}. 
+00009d50: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+00009d60: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
+00009d70: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
+00009d80: 6d73 3d70 6179 6c6f 6164 2c20 6d65 7468  ms=payload, meth
+00009d90: 6f64 3d22 706f 7374 2229 0a0a 0a61 7379  od="post")...asy
+00009da0: 6e63 2064 6566 2075 6e62 616e 5f63 6861  nc def unban_cha
+00009db0: 745f 7365 6e64 6572 5f63 6861 7428 746f  t_sender_chat(to
+00009dc0: 6b65 6e2c 2063 6861 745f 6964 2c20 7365  ken, chat_id, se
+00009dd0: 6e64 6572 5f63 6861 745f 6964 293a 0a20  nder_chat_id):. 
+00009de0: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
+00009df0: 2275 6e62 616e 4368 6174 5365 6e64 6572  "unbanChatSender
+00009e00: 4368 6174 220a 2020 2020 7061 796c 6f61  Chat".    payloa
+00009e10: 6420 3d20 7b22 6368 6174 5f69 6422 3a20  d = {"chat_id": 
+00009e20: 6368 6174 5f69 642c 2022 7365 6e64 6572  chat_id, "sender
+00009e30: 5f63 6861 745f 6964 223a 2073 656e 6465  _chat_id": sende
+00009e40: 725f 6368 6174 5f69 647d 0a20 2020 2072  r_chat_id}.    r
+00009e50: 6574 7572 6e20 6177 6169 7420 5f72 6571  eturn await _req
+00009e60: 7565 7374 2874 6f6b 656e 2c20 6d65 7468  uest(token, meth
+00009e70: 6f64 5f75 726c 2c20 7061 7261 6d73 3d70  od_url, params=p
+00009e80: 6179 6c6f 6164 2c20 6d65 7468 6f64 3d22  ayload, method="
+00009e90: 706f 7374 2229 0a0a 0a61 7379 6e63 2064  post")...async d
+00009ea0: 6566 2073 6574 5f63 6861 745f 7065 726d  ef set_chat_perm
+00009eb0: 6973 7369 6f6e 7328 746f 6b65 6e2c 2063  issions(token, c
+00009ec0: 6861 745f 6964 2c20 7065 726d 6973 7369  hat_id, permissi
+00009ed0: 6f6e 732c 2075 7365 5f69 6e64 6570 656e  ons, use_indepen
+00009ee0: 6465 6e74 5f63 6861 745f 7065 726d 6973  dent_chat_permis
+00009ef0: 7369 6f6e 733a 204f 7074 696f 6e61 6c5b  sions: Optional[
+00009f00: 626f 6f6c 5d20 3d20 4e6f 6e65 293a 0a20  bool] = None):. 
+00009f10: 2020 2072 6f75 7465 203d 2022 7365 7443     route = "setC
+00009f20: 6861 7450 6572 6d69 7373 696f 6e73 220a  hatPermissions".
+00009f30: 2020 2020 7061 796c 6f61 6420 3d20 7b22      payload = {"
+00009f40: 6368 6174 5f69 6422 3a20 6368 6174 5f69  chat_id": chat_i
+00009f50: 642c 2022 7065 726d 6973 7369 6f6e 7322  d, "permissions"
+00009f60: 3a20 7065 726d 6973 7369 6f6e 732e 746f  : permissions.to
+00009f70: 5f6a 736f 6e28 297d 0a20 2020 2069 6620  _json()}.    if 
+00009f80: 7573 655f 696e 6465 7065 6e64 656e 745f  use_independent_
+00009f90: 6368 6174 5f70 6572 6d69 7373 696f 6e73  chat_permissions
+00009fa0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00009fb0: 2020 2020 2020 7061 796c 6f61 645b 2275        payload["u
+00009fc0: 7365 5f69 6e64 6570 656e 6465 6e74 5f63  se_independent_c
+00009fd0: 6861 745f 7065 726d 6973 7369 6f6e 7322  hat_permissions"
+00009fe0: 5d20 3d20 7573 655f 696e 6465 7065 6e64  ] = use_independ
+00009ff0: 656e 745f 6368 6174 5f70 6572 6d69 7373  ent_chat_permiss
+0000a000: 696f 6e73 0a20 2020 2072 6574 7572 6e20  ions.    return 
+0000a010: 6177 6169 7420 5f72 6571 7565 7374 2874  await _request(t
+0000a020: 6f6b 656e 2c20 726f 7574 652c 2070 6172  oken, route, par
+0000a030: 616d 733d 7061 796c 6f61 642c 206d 6574  ams=payload, met
+0000a040: 686f 643d 2270 6f73 7422 290a 0a0a 6173  hod="post")...as
+0000a050: 796e 6320 6465 6620 6372 6561 7465 5f63  ync def create_c
+0000a060: 6861 745f 696e 7669 7465 5f6c 696e 6b28  hat_invite_link(
+0000a070: 746f 6b65 6e2c 2063 6861 745f 6964 2c20  token, chat_id, 
+0000a080: 6e61 6d65 2c20 6578 7069 7265 5f64 6174  name, expire_dat
+0000a090: 652c 206d 656d 6265 725f 6c69 6d69 742c  e, member_limit,
+0000a0a0: 2063 7265 6174 6573 5f6a 6f69 6e5f 7265   creates_join_re
+0000a0b0: 7175 6573 7429 3a0a 2020 2020 6d65 7468  quest):.    meth
+0000a0c0: 6f64 5f75 726c 203d 2022 6372 6561 7465  od_url = "create
+0000a0d0: 4368 6174 496e 7669 7465 4c69 6e6b 220a  ChatInviteLink".
+0000a0e0: 2020 2020 7061 796c 6f61 6420 3d20 7b22      payload = {"
+0000a0f0: 6368 6174 5f69 6422 3a20 6368 6174 5f69  chat_id": chat_i
+0000a100: 647d 0a0a 2020 2020 6966 2065 7870 6972  d}..    if expir
+0000a110: 655f 6461 7465 2069 7320 6e6f 7420 4e6f  e_date is not No
+0000a120: 6e65 3a0a 2020 2020 2020 2020 6966 2069  ne:.        if i
+0000a130: 7369 6e73 7461 6e63 6528 6578 7069 7265  sinstance(expire
+0000a140: 5f64 6174 652c 2064 6174 6574 696d 6529  _date, datetime)
+0000a150: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+0000a160: 796c 6f61 645b 2265 7870 6972 655f 6461  yload["expire_da
+0000a170: 7465 225d 203d 2065 7870 6972 655f 6461  te"] = expire_da
+0000a180: 7465 2e74 696d 6573 7461 6d70 2829 0a20  te.timestamp(). 
+0000a190: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000a1a0: 2020 2020 2020 2020 2070 6179 6c6f 6164           payload
+0000a1b0: 5b22 6578 7069 7265 5f64 6174 6522 5d20  ["expire_date"] 
+0000a1c0: 3d20 6578 7069 7265 5f64 6174 650a 2020  = expire_date.  
+0000a1d0: 2020 6966 206d 656d 6265 725f 6c69 6d69    if member_limi
+0000a1e0: 743a 0a20 2020 2020 2020 2070 6179 6c6f  t:.        paylo
+0000a1f0: 6164 5b22 6d65 6d62 6572 5f6c 696d 6974  ad["member_limit
+0000a200: 225d 203d 206d 656d 6265 725f 6c69 6d69  "] = member_limi
+0000a210: 740a 2020 2020 6966 2063 7265 6174 6573  t.    if creates
+0000a220: 5f6a 6f69 6e5f 7265 7175 6573 7420 6973  _join_request is
+0000a230: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000a240: 2020 2070 6179 6c6f 6164 5b22 6372 6561     payload["crea
+0000a250: 7465 735f 6a6f 696e 5f72 6571 7565 7374  tes_join_request
+0000a260: 225d 203d 2063 7265 6174 6573 5f6a 6f69  "] = creates_joi
+0000a270: 6e5f 7265 7175 6573 740a 2020 2020 6966  n_request.    if
+0000a280: 206e 616d 653a 0a20 2020 2020 2020 2070   name:.        p
+0000a290: 6179 6c6f 6164 5b22 6e61 6d65 225d 203d  ayload["name"] =
+0000a2a0: 206e 616d 650a 0a20 2020 2072 6574 7572   name..    retur
+0000a2b0: 6e20 6177 6169 7420 5f72 6571 7565 7374  n await _request
+0000a2c0: 2874 6f6b 656e 2c20 6d65 7468 6f64 5f75  (token, method_u
+0000a2d0: 726c 2c20 7061 7261 6d73 3d70 6179 6c6f  rl, params=paylo
+0000a2e0: 6164 2c20 6d65 7468 6f64 3d22 706f 7374  ad, method="post
+0000a2f0: 2229 0a0a 0a61 7379 6e63 2064 6566 2065  ")...async def e
+0000a300: 6469 745f 6368 6174 5f69 6e76 6974 655f  dit_chat_invite_
+0000a310: 6c69 6e6b 2874 6f6b 656e 2c20 6368 6174  link(token, chat
+0000a320: 5f69 642c 2069 6e76 6974 655f 6c69 6e6b  _id, invite_link
+0000a330: 2c20 6e61 6d65 2c20 6578 7069 7265 5f64  , name, expire_d
+0000a340: 6174 652c 206d 656d 6265 725f 6c69 6d69  ate, member_limi
+0000a350: 742c 2063 7265 6174 6573 5f6a 6f69 6e5f  t, creates_join_
+0000a360: 7265 7175 6573 7429 3a0a 2020 2020 6d65  request):.    me
+0000a370: 7468 6f64 5f75 726c 203d 2022 6564 6974  thod_url = "edit
+0000a380: 4368 6174 496e 7669 7465 4c69 6e6b 220a  ChatInviteLink".
+0000a390: 2020 2020 7061 796c 6f61 6420 3d20 7b22      payload = {"
+0000a3a0: 6368 6174 5f69 6422 3a20 6368 6174 5f69  chat_id": chat_i
+0000a3b0: 642c 2022 696e 7669 7465 5f6c 696e 6b22  d, "invite_link"
+0000a3c0: 3a20 696e 7669 7465 5f6c 696e 6b7d 0a0a  : invite_link}..
+0000a3d0: 2020 2020 6966 2065 7870 6972 655f 6461      if expire_da
+0000a3e0: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  te is not None:.
+0000a3f0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+0000a400: 7461 6e63 6528 6578 7069 7265 5f64 6174  tance(expire_dat
+0000a410: 652c 2064 6174 6574 696d 6529 3a0a 2020  e, datetime):.  
+0000a420: 2020 2020 2020 2020 2020 7061 796c 6f61            payloa
+0000a430: 645b 2265 7870 6972 655f 6461 7465 225d  d["expire_date"]
+0000a440: 203d 2065 7870 6972 655f 6461 7465 2e74   = expire_date.t
+0000a450: 696d 6573 7461 6d70 2829 0a20 2020 2020  imestamp().     
+0000a460: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000a470: 2020 2020 2070 6179 6c6f 6164 5b22 6578       payload["ex
+0000a480: 7069 7265 5f64 6174 6522 5d20 3d20 6578  pire_date"] = ex
+0000a490: 7069 7265 5f64 6174 650a 0a20 2020 2069  pire_date..    i
+0000a4a0: 6620 6d65 6d62 6572 5f6c 696d 6974 2069  f member_limit i
+0000a4b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000a4c0: 2020 2020 7061 796c 6f61 645b 226d 656d      payload["mem
+0000a4d0: 6265 725f 6c69 6d69 7422 5d20 3d20 6d65  ber_limit"] = me
+0000a4e0: 6d62 6572 5f6c 696d 6974 0a20 2020 2069  mber_limit.    i
+0000a4f0: 6620 6e61 6d65 3a0a 2020 2020 2020 2020  f name:.        
+0000a500: 7061 796c 6f61 645b 226e 616d 6522 5d20  payload["name"] 
+0000a510: 3d20 6e61 6d65 0a20 2020 2069 6620 6372  = name.    if cr
+0000a520: 6561 7465 735f 6a6f 696e 5f72 6571 7565  eates_join_reque
+0000a530: 7374 2069 7320 6e6f 7420 4e6f 6e65 3a0a  st is not None:.
 0000a540: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-0000a550: 2265 7870 6972 655f 6461 7465 225d 203d  "expire_date"] =
-0000a560: 2065 7870 6972 655f 6461 7465 2e74 696d   expire_date.tim
-0000a570: 6573 7461 6d70 2829 0a20 2020 2020 2020  estamp().       
-0000a580: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000a590: 2020 2070 6179 6c6f 6164 5b22 6578 7069     payload["expi
-0000a5a0: 7265 5f64 6174 6522 5d20 3d20 6578 7069  re_date"] = expi
-0000a5b0: 7265 5f64 6174 650a 0a20 2020 2069 6620  re_date..    if 
-0000a5c0: 6d65 6d62 6572 5f6c 696d 6974 2069 7320  member_limit is 
-0000a5d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000a5e0: 2020 7061 796c 6f61 645b 226d 656d 6265    payload["membe
-0000a5f0: 725f 6c69 6d69 7422 5d20 3d20 6d65 6d62  r_limit"] = memb
-0000a600: 6572 5f6c 696d 6974 0a20 2020 2069 6620  er_limit.    if 
-0000a610: 6e61 6d65 3a0a 2020 2020 2020 2020 7061  name:.        pa
-0000a620: 796c 6f61 645b 226e 616d 6522 5d20 3d20  yload["name"] = 
-0000a630: 6e61 6d65 0a20 2020 2069 6620 6372 6561  name.    if crea
-0000a640: 7465 735f 6a6f 696e 5f72 6571 7565 7374  tes_join_request
-0000a650: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000a660: 2020 2020 2020 7061 796c 6f61 645b 2263        payload["c
-0000a670: 7265 6174 6573 5f6a 6f69 6e5f 7265 7175  reates_join_requ
-0000a680: 6573 7422 5d20 3d20 6372 6561 7465 735f  est"] = creates_
-0000a690: 6a6f 696e 5f72 6571 7565 7374 0a0a 2020  join_request..  
-0000a6a0: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
-0000a6b0: 7265 7175 6573 7428 746f 6b65 6e2c 206d  request(token, m
-0000a6c0: 6574 686f 645f 7572 6c2c 2070 6172 616d  ethod_url, param
-0000a6d0: 733d 7061 796c 6f61 642c 206d 6574 686f  s=payload, metho
-0000a6e0: 643d 2270 6f73 7422 290a 0a0a 6173 796e  d="post")...asyn
-0000a6f0: 6320 6465 6620 6765 745f 6375 7374 6f6d  c def get_custom
-0000a700: 5f65 6d6f 6a69 5f73 7469 636b 6572 7328  _emoji_stickers(
-0000a710: 746f 6b65 6e2c 2063 7573 746f 6d5f 656d  token, custom_em
-0000a720: 6f6a 695f 6964 7329 3a0a 2020 2020 726f  oji_ids):.    ro
-0000a730: 7574 6520 3d20 7222 6765 7443 7573 746f  ute = r"getCusto
-0000a740: 6d45 6d6f 6a69 5374 6963 6b65 7273 220a  mEmojiStickers".
-0000a750: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-0000a760: 205f 7265 7175 6573 7428 746f 6b65 6e2c   _request(token,
-0000a770: 2072 6f75 7465 2c20 7061 7261 6d73 3d7b   route, params={
-0000a780: 2263 7573 746f 6d5f 656d 6f6a 695f 6964  "custom_emoji_id
-0000a790: 7322 3a20 6375 7374 6f6d 5f65 6d6f 6a69  s": custom_emoji
-0000a7a0: 5f69 6473 7d29 0a0a 0a61 7379 6e63 2064  _ids})...async d
-0000a7b0: 6566 2072 6576 6f6b 655f 6368 6174 5f69  ef revoke_chat_i
-0000a7c0: 6e76 6974 655f 6c69 6e6b 2874 6f6b 656e  nvite_link(token
-0000a7d0: 2c20 6368 6174 5f69 642c 2069 6e76 6974  , chat_id, invit
-0000a7e0: 655f 6c69 6e6b 293a 0a20 2020 2072 6f75  e_link):.    rou
-0000a7f0: 7465 203d 2022 7265 766f 6b65 4368 6174  te = "revokeChat
-0000a800: 496e 7669 7465 4c69 6e6b 220a 2020 2020  InviteLink".    
-0000a810: 7061 796c 6f61 6420 3d20 7b22 6368 6174  payload = {"chat
-0000a820: 5f69 6422 3a20 6368 6174 5f69 642c 2022  _id": chat_id, "
-0000a830: 696e 7669 7465 5f6c 696e 6b22 3a20 696e  invite_link": in
-0000a840: 7669 7465 5f6c 696e 6b7d 0a20 2020 2072  vite_link}.    r
-0000a850: 6574 7572 6e20 6177 6169 7420 5f72 6571  eturn await _req
-0000a860: 7565 7374 2874 6f6b 656e 2c20 726f 7574  uest(token, rout
-0000a870: 652c 2070 6172 616d 733d 7061 796c 6f61  e, params=payloa
-0000a880: 642c 206d 6574 686f 643d 2270 6f73 7422  d, method="post"
-0000a890: 290a 0a0a 6173 796e 6320 6465 6620 6578  )...async def ex
-0000a8a0: 706f 7274 5f63 6861 745f 696e 7669 7465  port_chat_invite
-0000a8b0: 5f6c 696e 6b28 746f 6b65 6e2c 2063 6861  _link(token, cha
-0000a8c0: 745f 6964 293a 0a20 2020 206d 6574 686f  t_id):.    metho
-0000a8d0: 645f 7572 6c20 3d20 2265 7870 6f72 7443  d_url = "exportC
-0000a8e0: 6861 7449 6e76 6974 654c 696e 6b22 0a20  hatInviteLink". 
-0000a8f0: 2020 2070 6179 6c6f 6164 203d 207b 2263     payload = {"c
-0000a900: 6861 745f 6964 223a 2063 6861 745f 6964  hat_id": chat_id
-0000a910: 7d0a 2020 2020 7265 7475 726e 2061 7761  }.    return awa
-0000a920: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
-0000a930: 6e2c 206d 6574 686f 645f 7572 6c2c 2070  n, method_url, p
-0000a940: 6172 616d 733d 7061 796c 6f61 642c 206d  arams=payload, m
-0000a950: 6574 686f 643d 2270 6f73 7422 290a 0a0a  ethod="post")...
-0000a960: 6173 796e 6320 6465 6620 6170 7072 6f76  async def approv
-0000a970: 655f 6368 6174 5f6a 6f69 6e5f 7265 7175  e_chat_join_requ
-0000a980: 6573 7428 746f 6b65 6e2c 2063 6861 745f  est(token, chat_
-0000a990: 6964 2c20 7573 6572 5f69 6429 3a0a 2020  id, user_id):.  
-0000a9a0: 2020 6d65 7468 6f64 5f75 726c 203d 2022    method_url = "
-0000a9b0: 6170 7072 6f76 6543 6861 744a 6f69 6e52  approveChatJoinR
-0000a9c0: 6571 7565 7374 220a 2020 2020 7061 796c  equest".    payl
-0000a9d0: 6f61 6420 3d20 7b22 6368 6174 5f69 6422  oad = {"chat_id"
-0000a9e0: 3a20 6368 6174 5f69 642c 2022 7573 6572  : chat_id, "user
-0000a9f0: 5f69 6422 3a20 7573 6572 5f69 647d 0a20  _id": user_id}. 
-0000aa00: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-0000aa10: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
-0000aa20: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
-0000aa30: 6d73 3d70 6179 6c6f 6164 2c20 6d65 7468  ms=payload, meth
-0000aa40: 6f64 3d22 706f 7374 2229 0a0a 0a61 7379  od="post")...asy
-0000aa50: 6e63 2064 6566 2064 6563 6c69 6e65 5f63  nc def decline_c
-0000aa60: 6861 745f 6a6f 696e 5f72 6571 7565 7374  hat_join_request
-0000aa70: 2874 6f6b 656e 2c20 6368 6174 5f69 642c  (token, chat_id,
-0000aa80: 2075 7365 725f 6964 293a 0a20 2020 206d   user_id):.    m
-0000aa90: 6574 686f 645f 7572 6c20 3d20 2264 6563  ethod_url = "dec
-0000aaa0: 6c69 6e65 4368 6174 4a6f 696e 5265 7175  lineChatJoinRequ
-0000aab0: 6573 7422 0a20 2020 2070 6179 6c6f 6164  est".    payload
-0000aac0: 203d 207b 2263 6861 745f 6964 223a 2063   = {"chat_id": c
-0000aad0: 6861 745f 6964 2c20 2275 7365 725f 6964  hat_id, "user_id
-0000aae0: 223a 2075 7365 725f 6964 7d0a 2020 2020  ": user_id}.    
-0000aaf0: 7265 7475 726e 2061 7761 6974 205f 7265  return await _re
-0000ab00: 7175 6573 7428 746f 6b65 6e2c 206d 6574  quest(token, met
-0000ab10: 686f 645f 7572 6c2c 2070 6172 616d 733d  hod_url, params=
-0000ab20: 7061 796c 6f61 642c 206d 6574 686f 643d  payload, method=
-0000ab30: 2270 6f73 7422 290a 0a0a 6173 796e 6320  "post")...async 
-0000ab40: 6465 6620 7365 745f 6368 6174 5f70 686f  def set_chat_pho
-0000ab50: 746f 2874 6f6b 656e 2c20 6368 6174 5f69  to(token, chat_i
-0000ab60: 642c 2070 686f 746f 293a 0a20 2020 206d  d, photo):.    m
-0000ab70: 6574 686f 645f 7572 6c20 3d20 2273 6574  ethod_url = "set
-0000ab80: 4368 6174 5068 6f74 6f22 0a20 2020 2070  ChatPhoto".    p
-0000ab90: 6179 6c6f 6164 203d 207b 2263 6861 745f  ayload = {"chat_
-0000aba0: 6964 223a 2063 6861 745f 6964 7d0a 2020  id": chat_id}.  
-0000abb0: 2020 6669 6c65 7320 3d20 4e6f 6e65 0a20    files = None. 
-0000abc0: 2020 2069 6620 7574 696c 2e69 735f 7374     if util.is_st
-0000abd0: 7269 6e67 2870 686f 746f 293a 0a20 2020  ring(photo):.   
-0000abe0: 2020 2020 2070 6179 6c6f 6164 5b22 7068       payload["ph
-0000abf0: 6f74 6f22 5d20 3d20 7068 6f74 6f0a 2020  oto"] = photo.  
-0000ac00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000ac10: 6669 6c65 7320 3d20 7b22 7068 6f74 6f22  files = {"photo"
-0000ac20: 3a20 7068 6f74 6f7d 0a20 2020 2072 6574  : photo}.    ret
-0000ac30: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
-0000ac40: 7374 2874 6f6b 656e 2c20 6d65 7468 6f64  st(token, method
-0000ac50: 5f75 726c 2c20 7061 7261 6d73 3d70 6179  _url, params=pay
-0000ac60: 6c6f 6164 2c20 6669 6c65 733d 6669 6c65  load, files=file
-0000ac70: 732c 206d 6574 686f 643d 2270 6f73 7422  s, method="post"
-0000ac80: 290a 0a0a 6173 796e 6320 6465 6620 6465  )...async def de
-0000ac90: 6c65 7465 5f63 6861 745f 7068 6f74 6f28  lete_chat_photo(
-0000aca0: 746f 6b65 6e2c 2063 6861 745f 6964 293a  token, chat_id):
-0000acb0: 0a20 2020 206d 6574 686f 645f 7572 6c20  .    method_url 
-0000acc0: 3d20 2264 656c 6574 6543 6861 7450 686f  = "deleteChatPho
-0000acd0: 746f 220a 2020 2020 7061 796c 6f61 6420  to".    payload 
-0000ace0: 3d20 7b22 6368 6174 5f69 6422 3a20 6368  = {"chat_id": ch
-0000acf0: 6174 5f69 647d 0a20 2020 2072 6574 7572  at_id}.    retur
-0000ad00: 6e20 6177 6169 7420 5f72 6571 7565 7374  n await _request
-0000ad10: 2874 6f6b 656e 2c20 6d65 7468 6f64 5f75  (token, method_u
-0000ad20: 726c 2c20 7061 7261 6d73 3d70 6179 6c6f  rl, params=paylo
-0000ad30: 6164 2c20 6d65 7468 6f64 3d22 706f 7374  ad, method="post
-0000ad40: 2229 0a0a 0a61 7379 6e63 2064 6566 2073  ")...async def s
-0000ad50: 6574 5f63 6861 745f 7469 746c 6528 746f  et_chat_title(to
-0000ad60: 6b65 6e2c 2063 6861 745f 6964 2c20 7469  ken, chat_id, ti
-0000ad70: 746c 6529 3a0a 2020 2020 6d65 7468 6f64  tle):.    method
-0000ad80: 5f75 726c 203d 2022 7365 7443 6861 7454  _url = "setChatT
-0000ad90: 6974 6c65 220a 2020 2020 7061 796c 6f61  itle".    payloa
-0000ada0: 6420 3d20 7b22 6368 6174 5f69 6422 3a20  d = {"chat_id": 
-0000adb0: 6368 6174 5f69 642c 2022 7469 746c 6522  chat_id, "title"
-0000adc0: 3a20 7469 746c 657d 0a20 2020 2072 6574  : title}.    ret
-0000add0: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
-0000ade0: 7374 2874 6f6b 656e 2c20 6d65 7468 6f64  st(token, method
-0000adf0: 5f75 726c 2c20 7061 7261 6d73 3d70 6179  _url, params=pay
-0000ae00: 6c6f 6164 2c20 6d65 7468 6f64 3d22 706f  load, method="po
-0000ae10: 7374 2229 0a0a 0a61 7379 6e63 2064 6566  st")...async def
-0000ae20: 2067 6574 5f6d 795f 636f 6d6d 616e 6473   get_my_commands
-0000ae30: 2874 6f6b 656e 2c20 7363 6f70 653d 4e6f  (token, scope=No
-0000ae40: 6e65 2c20 6c61 6e67 7561 6765 5f63 6f64  ne, language_cod
-0000ae50: 653d 4e6f 6e65 293a 0a20 2020 206d 6574  e=None):.    met
-0000ae60: 686f 645f 7572 6c20 3d20 7222 6765 744d  hod_url = r"getM
-0000ae70: 7943 6f6d 6d61 6e64 7322 0a20 2020 2070  yCommands".    p
-0000ae80: 6179 6c6f 6164 203d 207b 7d0a 2020 2020  ayload = {}.    
-0000ae90: 6966 2073 636f 7065 3a0a 2020 2020 2020  if scope:.      
-0000aea0: 2020 7061 796c 6f61 645b 2273 636f 7065    payload["scope
-0000aeb0: 225d 203d 2073 636f 7065 2e74 6f5f 6a73  "] = scope.to_js
-0000aec0: 6f6e 2829 0a20 2020 2069 6620 6c61 6e67  on().    if lang
-0000aed0: 7561 6765 5f63 6f64 653a 0a20 2020 2020  uage_code:.     
-0000aee0: 2020 2070 6179 6c6f 6164 5b22 6c61 6e67     payload["lang
-0000aef0: 7561 6765 5f63 6f64 6522 5d20 3d20 6c61  uage_code"] = la
-0000af00: 6e67 7561 6765 5f63 6f64 650a 2020 2020  nguage_code.    
-0000af10: 7265 7475 726e 2061 7761 6974 205f 7265  return await _re
-0000af20: 7175 6573 7428 746f 6b65 6e2c 206d 6574  quest(token, met
-0000af30: 686f 645f 7572 6c2c 2070 6172 616d 733d  hod_url, params=
-0000af40: 7061 796c 6f61 6429 0a0a 0a61 7379 6e63  payload)...async
-0000af50: 2064 6566 2073 6574 5f63 6861 745f 6d65   def set_chat_me
-0000af60: 6e75 5f62 7574 746f 6e28 746f 6b65 6e2c  nu_button(token,
-0000af70: 2063 6861 745f 6964 3d4e 6f6e 652c 206d   chat_id=None, m
-0000af80: 656e 755f 6275 7474 6f6e 3d4e 6f6e 6529  enu_button=None)
-0000af90: 3a0a 2020 2020 6d65 7468 6f64 5f75 726c  :.    method_url
-0000afa0: 203d 2072 2273 6574 4368 6174 4d65 6e75   = r"setChatMenu
-0000afb0: 4275 7474 6f6e 220a 2020 2020 7061 796c  Button".    payl
-0000afc0: 6f61 6420 3d20 7b7d 0a20 2020 2069 6620  oad = {}.    if 
-0000afd0: 6368 6174 5f69 643a 0a20 2020 2020 2020  chat_id:.       
-0000afe0: 2070 6179 6c6f 6164 5b22 6368 6174 5f69   payload["chat_i
-0000aff0: 6422 5d20 3d20 6368 6174 5f69 640a 2020  d"] = chat_id.  
-0000b000: 2020 6966 206d 656e 755f 6275 7474 6f6e    if menu_button
-0000b010: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-0000b020: 645b 226d 656e 755f 6275 7474 6f6e 225d  d["menu_button"]
-0000b030: 203d 206d 656e 755f 6275 7474 6f6e 2e74   = menu_button.t
-0000b040: 6f5f 6a73 6f6e 2829 0a0a 2020 2020 7265  o_json()..    re
-0000b050: 7475 726e 2061 7761 6974 205f 7265 7175  turn await _requ
-0000b060: 6573 7428 746f 6b65 6e2c 206d 6574 686f  est(token, metho
-0000b070: 645f 7572 6c2c 2070 6172 616d 733d 7061  d_url, params=pa
-0000b080: 796c 6f61 642c 206d 6574 686f 643d 2270  yload, method="p
-0000b090: 6f73 7422 290a 0a0a 6173 796e 6320 6465  ost")...async de
-0000b0a0: 6620 6765 745f 6368 6174 5f6d 656e 755f  f get_chat_menu_
-0000b0b0: 6275 7474 6f6e 2874 6f6b 656e 2c20 6368  button(token, ch
-0000b0c0: 6174 5f69 643d 4e6f 6e65 293a 0a20 2020  at_id=None):.   
-0000b0d0: 206d 6574 686f 645f 7572 6c20 3d20 7222   method_url = r"
-0000b0e0: 6765 7443 6861 744d 656e 7542 7574 746f  getChatMenuButto
-0000b0f0: 6e22 0a20 2020 2070 6179 6c6f 6164 203d  n".    payload =
-0000b100: 207b 7d0a 2020 2020 6966 2063 6861 745f   {}.    if chat_
-0000b110: 6964 3a0a 2020 2020 2020 2020 7061 796c  id:.        payl
-0000b120: 6f61 645b 2263 6861 745f 6964 225d 203d  oad["chat_id"] =
-0000b130: 2063 6861 745f 6964 0a0a 2020 2020 7265   chat_id..    re
-0000b140: 7475 726e 2061 7761 6974 205f 7265 7175  turn await _requ
-0000b150: 6573 7428 746f 6b65 6e2c 206d 6574 686f  est(token, metho
-0000b160: 645f 7572 6c2c 2070 6172 616d 733d 7061  d_url, params=pa
-0000b170: 796c 6f61 642c 206d 6574 686f 643d 2270  yload, method="p
-0000b180: 6f73 7422 290a 0a0a 6173 796e 6320 6465  ost")...async de
-0000b190: 6620 7365 745f 6d79 5f64 6566 6175 6c74  f set_my_default
-0000b1a0: 5f61 646d 696e 6973 7472 6174 6f72 5f72  _administrator_r
-0000b1b0: 6967 6874 7328 746f 6b65 6e2c 2072 6967  ights(token, rig
-0000b1c0: 6874 733d 4e6f 6e65 2c20 666f 725f 6368  hts=None, for_ch
-0000b1d0: 616e 6e65 6c73 3d4e 6f6e 6529 3a0a 2020  annels=None):.  
-0000b1e0: 2020 6d65 7468 6f64 5f75 726c 203d 2072    method_url = r
-0000b1f0: 2273 6574 4d79 4465 6661 756c 7441 646d  "setMyDefaultAdm
-0000b200: 696e 6973 7472 6174 6f72 5269 6768 7473  inistratorRights
-0000b210: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
-0000b220: 7b7d 0a20 2020 2069 6620 7269 6768 7473  {}.    if rights
-0000b230: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-0000b240: 645b 2272 6967 6874 7322 5d20 3d20 7269  d["rights"] = ri
-0000b250: 6768 7473 2e74 6f5f 6a73 6f6e 2829 0a20  ghts.to_json(). 
-0000b260: 2020 2069 6620 666f 725f 6368 616e 6e65     if for_channe
-0000b270: 6c73 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ls is not None:.
-0000b280: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-0000b290: 2266 6f72 5f63 6861 6e6e 656c 7322 5d20  "for_channels"] 
-0000b2a0: 3d20 666f 725f 6368 616e 6e65 6c73 0a0a  = for_channels..
-0000b2b0: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-0000b2c0: 205f 7265 7175 6573 7428 746f 6b65 6e2c   _request(token,
-0000b2d0: 206d 6574 686f 645f 7572 6c2c 2070 6172   method_url, par
-0000b2e0: 616d 733d 7061 796c 6f61 642c 206d 6574  ams=payload, met
-0000b2f0: 686f 643d 2270 6f73 7422 290a 0a0a 6173  hod="post")...as
-0000b300: 796e 6320 6465 6620 6765 745f 6d79 5f64  ync def get_my_d
-0000b310: 6566 6175 6c74 5f61 646d 696e 6973 7472  efault_administr
-0000b320: 6174 6f72 5f72 6967 6874 7328 746f 6b65  ator_rights(toke
-0000b330: 6e2c 2066 6f72 5f63 6861 6e6e 656c 733d  n, for_channels=
-0000b340: 4e6f 6e65 293a 0a20 2020 206d 6574 686f  None):.    metho
-0000b350: 645f 7572 6c20 3d20 7222 6765 744d 7944  d_url = r"getMyD
-0000b360: 6566 6175 6c74 4164 6d69 6e69 7374 7261  efaultAdministra
-0000b370: 746f 7252 6967 6874 7322 0a20 2020 2070  torRights".    p
-0000b380: 6179 6c6f 6164 203d 207b 7d0a 2020 2020  ayload = {}.    
-0000b390: 6966 2066 6f72 5f63 6861 6e6e 656c 733a  if for_channels:
-0000b3a0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000b3b0: 5b22 666f 725f 6368 616e 6e65 6c73 225d  ["for_channels"]
-0000b3c0: 203d 2066 6f72 5f63 6861 6e6e 656c 730a   = for_channels.
-0000b3d0: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
-0000b3e0: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
-0000b3f0: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
-0000b400: 7261 6d73 3d70 6179 6c6f 6164 2c20 6d65  rams=payload, me
-0000b410: 7468 6f64 3d22 706f 7374 2229 0a0a 0a61  thod="post")...a
-0000b420: 7379 6e63 2064 6566 2073 6574 5f6d 795f  sync def set_my_
-0000b430: 636f 6d6d 616e 6473 2874 6f6b 656e 2c20  commands(token, 
-0000b440: 636f 6d6d 616e 6473 2c20 7363 6f70 653d  commands, scope=
-0000b450: 4e6f 6e65 2c20 6c61 6e67 7561 6765 5f63  None, language_c
-0000b460: 6f64 653d 4e6f 6e65 293a 0a20 2020 206d  ode=None):.    m
-0000b470: 6574 686f 645f 7572 6c20 3d20 7222 7365  ethod_url = r"se
-0000b480: 744d 7943 6f6d 6d61 6e64 7322 0a20 2020  tMyCommands".   
-0000b490: 2070 6179 6c6f 6164 203d 207b 2263 6f6d   payload = {"com
-0000b4a0: 6d61 6e64 7322 3a20 6177 6169 7420 5f63  mands": await _c
-0000b4b0: 6f6e 7665 7274 5f6c 6973 745f 6a73 6f6e  onvert_list_json
-0000b4c0: 5f73 6572 6961 6c69 7a61 626c 6528 636f  _serializable(co
-0000b4d0: 6d6d 616e 6473 297d 0a20 2020 2069 6620  mmands)}.    if 
-0000b4e0: 7363 6f70 653a 0a20 2020 2020 2020 2070  scope:.        p
-0000b4f0: 6179 6c6f 6164 5b22 7363 6f70 6522 5d20  ayload["scope"] 
-0000b500: 3d20 7363 6f70 652e 746f 5f6a 736f 6e28  = scope.to_json(
-0000b510: 290a 2020 2020 6966 206c 616e 6775 6167  ).    if languag
-0000b520: 655f 636f 6465 3a0a 2020 2020 2020 2020  e_code:.        
-0000b530: 7061 796c 6f61 645b 226c 616e 6775 6167  payload["languag
-0000b540: 655f 636f 6465 225d 203d 206c 616e 6775  e_code"] = langu
-0000b550: 6167 655f 636f 6465 0a20 2020 2072 6574  age_code.    ret
-0000b560: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
-0000b570: 7374 2874 6f6b 656e 2c20 6d65 7468 6f64  st(token, method
-0000b580: 5f75 726c 2c20 7061 7261 6d73 3d70 6179  _url, params=pay
-0000b590: 6c6f 6164 2c20 6d65 7468 6f64 3d22 706f  load, method="po
-0000b5a0: 7374 2229 0a0a 0a61 7379 6e63 2064 6566  st")...async def
-0000b5b0: 2064 656c 6574 655f 6d79 5f63 6f6d 6d61   delete_my_comma
-0000b5c0: 6e64 7328 746f 6b65 6e2c 2073 636f 7065  nds(token, scope
-0000b5d0: 3d4e 6f6e 652c 206c 616e 6775 6167 655f  =None, language_
-0000b5e0: 636f 6465 3d4e 6f6e 6529 3a0a 2020 2020  code=None):.    
-0000b5f0: 6d65 7468 6f64 5f75 726c 203d 2072 2264  method_url = r"d
-0000b600: 656c 6574 654d 7943 6f6d 6d61 6e64 7322  eleteMyCommands"
-0000b610: 0a20 2020 2070 6179 6c6f 6164 203d 207b  .    payload = {
-0000b620: 7d0a 2020 2020 6966 2073 636f 7065 3a0a  }.    if scope:.
-0000b630: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-0000b640: 2273 636f 7065 225d 203d 2073 636f 7065  "scope"] = scope
-0000b650: 2e74 6f5f 6a73 6f6e 2829 0a20 2020 2069  .to_json().    i
-0000b660: 6620 6c61 6e67 7561 6765 5f63 6f64 653a  f language_code:
-0000b670: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000b680: 5b22 6c61 6e67 7561 6765 5f63 6f64 6522  ["language_code"
-0000b690: 5d20 3d20 6c61 6e67 7561 6765 5f63 6f64  ] = language_cod
-0000b6a0: 650a 2020 2020 7265 7475 726e 2061 7761  e.    return awa
-0000b6b0: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
-0000b6c0: 6e2c 206d 6574 686f 645f 7572 6c2c 2070  n, method_url, p
-0000b6d0: 6172 616d 733d 7061 796c 6f61 642c 206d  arams=payload, m
-0000b6e0: 6574 686f 643d 2270 6f73 7422 290a 0a0a  ethod="post")...
-0000b6f0: 6173 796e 6320 6465 6620 7365 745f 6368  async def set_ch
-0000b700: 6174 5f64 6573 6372 6970 7469 6f6e 2874  at_description(t
-0000b710: 6f6b 656e 2c20 6368 6174 5f69 642c 2064  oken, chat_id, d
-0000b720: 6573 6372 6970 7469 6f6e 293a 0a20 2020  escription):.   
-0000b730: 206d 6574 686f 645f 7572 6c20 3d20 2273   method_url = "s
-0000b740: 6574 4368 6174 4465 7363 7269 7074 696f  etChatDescriptio
-0000b750: 6e22 0a20 2020 2070 6179 6c6f 6164 203d  n".    payload =
-0000b760: 207b 2263 6861 745f 6964 223a 2063 6861   {"chat_id": cha
-0000b770: 745f 6964 7d0a 2020 2020 6966 2064 6573  t_id}.    if des
-0000b780: 6372 6970 7469 6f6e 2069 7320 6e6f 7420  cription is not 
-0000b790: 4e6f 6e65 3a20 2023 2041 6c6c 6f77 2065  None:  # Allow e
-0000b7a0: 6d70 7479 2073 7472 696e 6773 0a20 2020  mpty strings.   
-0000b7b0: 2020 2020 2070 6179 6c6f 6164 5b22 6465       payload["de
-0000b7c0: 7363 7269 7074 696f 6e22 5d20 3d20 6465  scription"] = de
-0000b7d0: 7363 7269 7074 696f 6e0a 2020 2020 7265  scription.    re
-0000b7e0: 7475 726e 2061 7761 6974 205f 7265 7175  turn await _requ
-0000b7f0: 6573 7428 746f 6b65 6e2c 206d 6574 686f  est(token, metho
-0000b800: 645f 7572 6c2c 2070 6172 616d 733d 7061  d_url, params=pa
-0000b810: 796c 6f61 642c 206d 6574 686f 643d 2270  yload, method="p
-0000b820: 6f73 7422 290a 0a0a 6173 796e 6320 6465  ost")...async de
-0000b830: 6620 7069 6e5f 6368 6174 5f6d 6573 7361  f pin_chat_messa
-0000b840: 6765 2874 6f6b 656e 2c20 6368 6174 5f69  ge(token, chat_i
-0000b850: 642c 206d 6573 7361 6765 5f69 642c 2064  d, message_id, d
-0000b860: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
-0000b870: 696f 6e3d 4e6f 6e65 293a 0a20 2020 206d  ion=None):.    m
-0000b880: 6574 686f 645f 7572 6c20 3d20 2270 696e  ethod_url = "pin
-0000b890: 4368 6174 4d65 7373 6167 6522 0a20 2020  ChatMessage".   
-0000b8a0: 2070 6179 6c6f 6164 203d 207b 2263 6861   payload = {"cha
-0000b8b0: 745f 6964 223a 2063 6861 745f 6964 2c20  t_id": chat_id, 
-0000b8c0: 226d 6573 7361 6765 5f69 6422 3a20 6d65  "message_id": me
-0000b8d0: 7373 6167 655f 6964 7d0a 2020 2020 6966  ssage_id}.    if
-0000b8e0: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
-0000b8f0: 6174 696f 6e20 6973 206e 6f74 204e 6f6e  ation is not Non
-0000b900: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-0000b910: 6164 5b22 6469 7361 626c 655f 6e6f 7469  ad["disable_noti
-0000b920: 6669 6361 7469 6f6e 225d 203d 2064 6973  fication"] = dis
-0000b930: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-0000b940: 6e0a 2020 2020 7265 7475 726e 2061 7761  n.    return awa
-0000b950: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
-0000b960: 6e2c 206d 6574 686f 645f 7572 6c2c 2070  n, method_url, p
-0000b970: 6172 616d 733d 7061 796c 6f61 642c 206d  arams=payload, m
-0000b980: 6574 686f 643d 2270 6f73 7422 290a 0a0a  ethod="post")...
-0000b990: 6173 796e 6320 6465 6620 756e 7069 6e5f  async def unpin_
-0000b9a0: 6368 6174 5f6d 6573 7361 6765 2874 6f6b  chat_message(tok
-0000b9b0: 656e 2c20 6368 6174 5f69 642c 206d 6573  en, chat_id, mes
-0000b9c0: 7361 6765 5f69 6429 3a0a 2020 2020 6d65  sage_id):.    me
-0000b9d0: 7468 6f64 5f75 726c 203d 2022 756e 7069  thod_url = "unpi
-0000b9e0: 6e43 6861 744d 6573 7361 6765 220a 2020  nChatMessage".  
-0000b9f0: 2020 7061 796c 6f61 6420 3d20 7b22 6368    payload = {"ch
-0000ba00: 6174 5f69 6422 3a20 6368 6174 5f69 647d  at_id": chat_id}
-0000ba10: 0a20 2020 2069 6620 6d65 7373 6167 655f  .    if message_
-0000ba20: 6964 3a0a 2020 2020 2020 2020 7061 796c  id:.        payl
-0000ba30: 6f61 645b 226d 6573 7361 6765 5f69 6422  oad["message_id"
-0000ba40: 5d20 3d20 6d65 7373 6167 655f 6964 0a20  ] = message_id. 
-0000ba50: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-0000ba60: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
-0000ba70: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
-0000ba80: 6d73 3d70 6179 6c6f 6164 2c20 6d65 7468  ms=payload, meth
-0000ba90: 6f64 3d22 706f 7374 2229 0a0a 0a61 7379  od="post")...asy
-0000baa0: 6e63 2064 6566 2075 6e70 696e 5f61 6c6c  nc def unpin_all
-0000bab0: 5f63 6861 745f 6d65 7373 6167 6573 2874  _chat_messages(t
-0000bac0: 6f6b 656e 2c20 6368 6174 5f69 6429 3a0a  oken, chat_id):.
-0000bad0: 2020 2020 6d65 7468 6f64 5f75 726c 203d      method_url =
-0000bae0: 2022 756e 7069 6e41 6c6c 4368 6174 4d65   "unpinAllChatMe
-0000baf0: 7373 6167 6573 220a 2020 2020 7061 796c  ssages".    payl
-0000bb00: 6f61 6420 3d20 7b22 6368 6174 5f69 6422  oad = {"chat_id"
-0000bb10: 3a20 6368 6174 5f69 647d 0a20 2020 2072  : chat_id}.    r
-0000bb20: 6574 7572 6e20 6177 6169 7420 5f72 6571  eturn await _req
-0000bb30: 7565 7374 2874 6f6b 656e 2c20 6d65 7468  uest(token, meth
-0000bb40: 6f64 5f75 726c 2c20 7061 7261 6d73 3d70  od_url, params=p
-0000bb50: 6179 6c6f 6164 2c20 6d65 7468 6f64 3d22  ayload, method="
-0000bb60: 706f 7374 2229 0a0a 0a23 2055 7064 6174  post")...# Updat
-0000bb70: 696e 6720 6d65 7373 6167 6573 0a0a 0a61  ing messages...a
-0000bb80: 7379 6e63 2064 6566 2065 6469 745f 6d65  sync def edit_me
-0000bb90: 7373 6167 655f 7465 7874 280a 2020 2020  ssage_text(.    
-0000bba0: 746f 6b65 6e2c 0a20 2020 2074 6578 742c  token,.    text,
-0000bbb0: 0a20 2020 2063 6861 745f 6964 3d4e 6f6e  .    chat_id=Non
-0000bbc0: 652c 0a20 2020 206d 6573 7361 6765 5f69  e,.    message_i
-0000bbd0: 643d 4e6f 6e65 2c0a 2020 2020 696e 6c69  d=None,.    inli
-0000bbe0: 6e65 5f6d 6573 7361 6765 5f69 643d 4e6f  ne_message_id=No
-0000bbf0: 6e65 2c0a 2020 2020 7061 7273 655f 6d6f  ne,.    parse_mo
-0000bc00: 6465 3d4e 6f6e 652c 0a20 2020 2065 6e74  de=None,.    ent
-0000bc10: 6974 6965 733d 4e6f 6e65 2c0a 2020 2020  ities=None,.    
-0000bc20: 6469 7361 626c 655f 7765 625f 7061 6765  disable_web_page
-0000bc30: 5f70 7265 7669 6577 3d4e 6f6e 652c 0a20  _preview=None,. 
-0000bc40: 2020 2072 6570 6c79 5f6d 6172 6b75 703d     reply_markup=
-0000bc50: 4e6f 6e65 2c0a 293a 0a20 2020 206d 6574  None,.):.    met
-0000bc60: 686f 645f 7572 6c20 3d20 7222 6564 6974  hod_url = r"edit
-0000bc70: 4d65 7373 6167 6554 6578 7422 0a20 2020  MessageText".   
-0000bc80: 2070 6179 6c6f 6164 203d 207b 2274 6578   payload = {"tex
-0000bc90: 7422 3a20 7465 7874 7d0a 2020 2020 6966  t": text}.    if
-0000bca0: 2063 6861 745f 6964 3a0a 2020 2020 2020   chat_id:.      
-0000bcb0: 2020 7061 796c 6f61 645b 2263 6861 745f    payload["chat_
-0000bcc0: 6964 225d 203d 2063 6861 745f 6964 0a20  id"] = chat_id. 
-0000bcd0: 2020 2069 6620 6d65 7373 6167 655f 6964     if message_id
-0000bce0: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-0000bcf0: 645b 226d 6573 7361 6765 5f69 6422 5d20  d["message_id"] 
-0000bd00: 3d20 6d65 7373 6167 655f 6964 0a20 2020  = message_id.   
-0000bd10: 2069 6620 696e 6c69 6e65 5f6d 6573 7361   if inline_messa
-0000bd20: 6765 5f69 643a 0a20 2020 2020 2020 2070  ge_id:.        p
-0000bd30: 6179 6c6f 6164 5b22 696e 6c69 6e65 5f6d  ayload["inline_m
-0000bd40: 6573 7361 6765 5f69 6422 5d20 3d20 696e  essage_id"] = in
-0000bd50: 6c69 6e65 5f6d 6573 7361 6765 5f69 640a  line_message_id.
-0000bd60: 2020 2020 6966 2070 6172 7365 5f6d 6f64      if parse_mod
-0000bd70: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-0000bd80: 6164 5b22 7061 7273 655f 6d6f 6465 225d  ad["parse_mode"]
-0000bd90: 203d 2070 6172 7365 5f6d 6f64 650a 2020   = parse_mode.  
-0000bda0: 2020 6966 2065 6e74 6974 6965 733a 0a20    if entities:. 
-0000bdb0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-0000bdc0: 656e 7469 7469 6573 225d 203d 206a 736f  entities"] = jso
-0000bdd0: 6e2e 6475 6d70 7328 7479 7065 732e 4d65  n.dumps(types.Me
-0000bde0: 7373 6167 6545 6e74 6974 792e 746f 5f6c  ssageEntity.to_l
-0000bdf0: 6973 745f 6f66 5f64 6963 7473 2865 6e74  ist_of_dicts(ent
-0000be00: 6974 6965 7329 290a 2020 2020 6966 2064  ities)).    if d
-0000be10: 6973 6162 6c65 5f77 6562 5f70 6167 655f  isable_web_page_
-0000be20: 7072 6576 6965 7720 6973 206e 6f74 204e  preview is not N
-0000be30: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
-0000be40: 6c6f 6164 5b22 6469 7361 626c 655f 7765  load["disable_we
-0000be50: 625f 7061 6765 5f70 7265 7669 6577 225d  b_page_preview"]
-0000be60: 203d 2064 6973 6162 6c65 5f77 6562 5f70   = disable_web_p
-0000be70: 6167 655f 7072 6576 6965 770a 2020 2020  age_preview.    
-0000be80: 6966 2072 6570 6c79 5f6d 6172 6b75 703a  if reply_markup:
-0000be90: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000bea0: 5b22 7265 706c 795f 6d61 726b 7570 225d  ["reply_markup"]
-0000beb0: 203d 2061 7761 6974 205f 636f 6e76 6572   = await _conver
-0000bec0: 745f 6d61 726b 7570 2872 6570 6c79 5f6d  t_markup(reply_m
-0000bed0: 6172 6b75 7029 0a20 2020 2072 6574 7572  arkup).    retur
-0000bee0: 6e20 6177 6169 7420 5f72 6571 7565 7374  n await _request
-0000bef0: 2874 6f6b 656e 2c20 6d65 7468 6f64 5f75  (token, method_u
-0000bf00: 726c 2c20 7061 7261 6d73 3d70 6179 6c6f  rl, params=paylo
-0000bf10: 6164 2c20 6d65 7468 6f64 3d22 706f 7374  ad, method="post
-0000bf20: 2229 0a0a 0a61 7379 6e63 2064 6566 2065  ")...async def e
-0000bf30: 6469 745f 6d65 7373 6167 655f 6361 7074  dit_message_capt
-0000bf40: 696f 6e28 0a20 2020 2074 6f6b 656e 2c0a  ion(.    token,.
-0000bf50: 2020 2020 6361 7074 696f 6e2c 0a20 2020      caption,.   
-0000bf60: 2063 6861 745f 6964 3d4e 6f6e 652c 0a20   chat_id=None,. 
-0000bf70: 2020 206d 6573 7361 6765 5f69 643d 4e6f     message_id=No
-0000bf80: 6e65 2c0a 2020 2020 696e 6c69 6e65 5f6d  ne,.    inline_m
-0000bf90: 6573 7361 6765 5f69 643d 4e6f 6e65 2c0a  essage_id=None,.
-0000bfa0: 2020 2020 7061 7273 655f 6d6f 6465 3d4e      parse_mode=N
-0000bfb0: 6f6e 652c 0a20 2020 2063 6170 7469 6f6e  one,.    caption
-0000bfc0: 5f65 6e74 6974 6965 733d 4e6f 6e65 2c0a  _entities=None,.
-0000bfd0: 2020 2020 7265 706c 795f 6d61 726b 7570      reply_markup
-0000bfe0: 3d4e 6f6e 652c 0a29 3a0a 2020 2020 6d65  =None,.):.    me
-0000bff0: 7468 6f64 5f75 726c 203d 2072 2265 6469  thod_url = r"edi
-0000c000: 744d 6573 7361 6765 4361 7074 696f 6e22  tMessageCaption"
-0000c010: 0a20 2020 2070 6179 6c6f 6164 203d 207b  .    payload = {
-0000c020: 2263 6170 7469 6f6e 223a 2063 6170 7469  "caption": capti
-0000c030: 6f6e 7d0a 2020 2020 6966 2063 6861 745f  on}.    if chat_
-0000c040: 6964 3a0a 2020 2020 2020 2020 7061 796c  id:.        payl
-0000c050: 6f61 645b 2263 6861 745f 6964 225d 203d  oad["chat_id"] =
-0000c060: 2063 6861 745f 6964 0a20 2020 2069 6620   chat_id.    if 
-0000c070: 6d65 7373 6167 655f 6964 3a0a 2020 2020  message_id:.    
-0000c080: 2020 2020 7061 796c 6f61 645b 226d 6573      payload["mes
-0000c090: 7361 6765 5f69 6422 5d20 3d20 6d65 7373  sage_id"] = mess
-0000c0a0: 6167 655f 6964 0a20 2020 2069 6620 696e  age_id.    if in
-0000c0b0: 6c69 6e65 5f6d 6573 7361 6765 5f69 643a  line_message_id:
-0000c0c0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000c0d0: 5b22 696e 6c69 6e65 5f6d 6573 7361 6765  ["inline_message
-0000c0e0: 5f69 6422 5d20 3d20 696e 6c69 6e65 5f6d  _id"] = inline_m
-0000c0f0: 6573 7361 6765 5f69 640a 2020 2020 6966  essage_id.    if
-0000c100: 2070 6172 7365 5f6d 6f64 653a 0a20 2020   parse_mode:.   
-0000c110: 2020 2020 2070 6179 6c6f 6164 5b22 7061       payload["pa
-0000c120: 7273 655f 6d6f 6465 225d 203d 2070 6172  rse_mode"] = par
-0000c130: 7365 5f6d 6f64 650a 2020 2020 6966 2063  se_mode.    if c
-0000c140: 6170 7469 6f6e 5f65 6e74 6974 6965 733a  aption_entities:
-0000c150: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000c160: 5b22 6361 7074 696f 6e5f 656e 7469 7469  ["caption_entiti
-0000c170: 6573 225d 203d 206a 736f 6e2e 6475 6d70  es"] = json.dump
-0000c180: 7328 7479 7065 732e 4d65 7373 6167 6545  s(types.MessageE
-0000c190: 6e74 6974 792e 746f 5f6c 6973 745f 6f66  ntity.to_list_of
-0000c1a0: 5f64 6963 7473 2863 6170 7469 6f6e 5f65  _dicts(caption_e
-0000c1b0: 6e74 6974 6965 7329 290a 2020 2020 6966  ntities)).    if
-0000c1c0: 2072 6570 6c79 5f6d 6172 6b75 703a 0a20   reply_markup:. 
-0000c1d0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-0000c1e0: 7265 706c 795f 6d61 726b 7570 225d 203d  reply_markup"] =
-0000c1f0: 2061 7761 6974 205f 636f 6e76 6572 745f   await _convert_
-0000c200: 6d61 726b 7570 2872 6570 6c79 5f6d 6172  markup(reply_mar
-0000c210: 6b75 7029 0a20 2020 2072 6574 7572 6e20  kup).    return 
-0000c220: 6177 6169 7420 5f72 6571 7565 7374 2874  await _request(t
-0000c230: 6f6b 656e 2c20 6d65 7468 6f64 5f75 726c  oken, method_url
-0000c240: 2c20 7061 7261 6d73 3d70 6179 6c6f 6164  , params=payload
-0000c250: 2c20 6d65 7468 6f64 3d22 706f 7374 2229  , method="post")
-0000c260: 0a0a 0a61 7379 6e63 2064 6566 2065 6469  ...async def edi
-0000c270: 745f 6d65 7373 6167 655f 6d65 6469 6128  t_message_media(
-0000c280: 0a20 2020 2074 6f6b 656e 2c0a 2020 2020  .    token,.    
-0000c290: 6d65 6469 612c 0a20 2020 2063 6861 745f  media,.    chat_
-0000c2a0: 6964 3d4e 6f6e 652c 0a20 2020 206d 6573  id=None,.    mes
-0000c2b0: 7361 6765 5f69 643d 4e6f 6e65 2c0a 2020  sage_id=None,.  
-0000c2c0: 2020 696e 6c69 6e65 5f6d 6573 7361 6765    inline_message
-0000c2d0: 5f69 643d 4e6f 6e65 2c0a 2020 2020 7265  _id=None,.    re
-0000c2e0: 706c 795f 6d61 726b 7570 3d4e 6f6e 652c  ply_markup=None,
-0000c2f0: 0a29 3a0a 2020 2020 6d65 7468 6f64 5f75  .):.    method_u
-0000c300: 726c 203d 2072 2265 6469 744d 6573 7361  rl = r"editMessa
-0000c310: 6765 4d65 6469 6122 0a20 2020 206d 6564  geMedia".    med
-0000c320: 6961 5f6a 736f 6e2c 2066 696c 6520 3d20  ia_json, file = 
-0000c330: 6177 6169 7420 636f 6e76 6572 745f 696e  await convert_in
-0000c340: 7075 745f 6d65 6469 6128 6d65 6469 6129  put_media(media)
-0000c350: 0a20 2020 2070 6179 6c6f 6164 203d 207b  .    payload = {
-0000c360: 226d 6564 6961 223a 206d 6564 6961 5f6a  "media": media_j
-0000c370: 736f 6e7d 0a20 2020 2069 6620 6368 6174  son}.    if chat
-0000c380: 5f69 643a 0a20 2020 2020 2020 2070 6179  _id:.        pay
-0000c390: 6c6f 6164 5b22 6368 6174 5f69 6422 5d20  load["chat_id"] 
-0000c3a0: 3d20 6368 6174 5f69 640a 2020 2020 6966  = chat_id.    if
-0000c3b0: 206d 6573 7361 6765 5f69 643a 0a20 2020   message_id:.   
-0000c3c0: 2020 2020 2070 6179 6c6f 6164 5b22 6d65       payload["me
-0000c3d0: 7373 6167 655f 6964 225d 203d 206d 6573  ssage_id"] = mes
-0000c3e0: 7361 6765 5f69 640a 2020 2020 6966 2069  sage_id.    if i
-0000c3f0: 6e6c 696e 655f 6d65 7373 6167 655f 6964  nline_message_id
-0000c400: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-0000c410: 645b 2269 6e6c 696e 655f 6d65 7373 6167  d["inline_messag
-0000c420: 655f 6964 225d 203d 2069 6e6c 696e 655f  e_id"] = inline_
-0000c430: 6d65 7373 6167 655f 6964 0a20 2020 2069  message_id.    i
-0000c440: 6620 7265 706c 795f 6d61 726b 7570 3a0a  f reply_markup:.
-0000c450: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-0000c460: 2272 6570 6c79 5f6d 6172 6b75 7022 5d20  "reply_markup"] 
-0000c470: 3d20 6177 6169 7420 5f63 6f6e 7665 7274  = await _convert
-0000c480: 5f6d 6172 6b75 7028 7265 706c 795f 6d61  _markup(reply_ma
-0000c490: 726b 7570 290a 2020 2020 7265 7475 726e  rkup).    return
-0000c4a0: 2061 7761 6974 205f 7265 7175 6573 7428   await _request(
-0000c4b0: 746f 6b65 6e2c 206d 6574 686f 645f 7572  token, method_ur
-0000c4c0: 6c2c 2070 6172 616d 733d 7061 796c 6f61  l, params=payloa
-0000c4d0: 642c 2066 696c 6573 3d66 696c 652c 206d  d, files=file, m
-0000c4e0: 6574 686f 643d 2270 6f73 7422 2069 6620  ethod="post" if 
-0000c4f0: 6669 6c65 2065 6c73 6520 2267 6574 2229  file else "get")
-0000c500: 0a0a 0a61 7379 6e63 2064 6566 2065 6469  ...async def edi
-0000c510: 745f 6d65 7373 6167 655f 7265 706c 795f  t_message_reply_
-0000c520: 6d61 726b 7570 2874 6f6b 656e 2c20 6368  markup(token, ch
-0000c530: 6174 5f69 643d 4e6f 6e65 2c20 6d65 7373  at_id=None, mess
-0000c540: 6167 655f 6964 3d4e 6f6e 652c 2069 6e6c  age_id=None, inl
-0000c550: 696e 655f 6d65 7373 6167 655f 6964 3d4e  ine_message_id=N
-0000c560: 6f6e 652c 2072 6570 6c79 5f6d 6172 6b75  one, reply_marku
-0000c570: 703d 4e6f 6e65 293a 0a20 2020 206d 6574  p=None):.    met
-0000c580: 686f 645f 7572 6c20 3d20 7222 6564 6974  hod_url = r"edit
-0000c590: 4d65 7373 6167 6552 6570 6c79 4d61 726b  MessageReplyMark
-0000c5a0: 7570 220a 2020 2020 7061 796c 6f61 6420  up".    payload 
-0000c5b0: 3d20 7b7d 0a20 2020 2069 6620 6368 6174  = {}.    if chat
-0000c5c0: 5f69 643a 0a20 2020 2020 2020 2070 6179  _id:.        pay
-0000c5d0: 6c6f 6164 5b22 6368 6174 5f69 6422 5d20  load["chat_id"] 
-0000c5e0: 3d20 6368 6174 5f69 640a 2020 2020 6966  = chat_id.    if
-0000c5f0: 206d 6573 7361 6765 5f69 643a 0a20 2020   message_id:.   
-0000c600: 2020 2020 2070 6179 6c6f 6164 5b22 6d65       payload["me
-0000c610: 7373 6167 655f 6964 225d 203d 206d 6573  ssage_id"] = mes
-0000c620: 7361 6765 5f69 640a 2020 2020 6966 2069  sage_id.    if i
-0000c630: 6e6c 696e 655f 6d65 7373 6167 655f 6964  nline_message_id
-0000c640: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-0000c650: 645b 2269 6e6c 696e 655f 6d65 7373 6167  d["inline_messag
-0000c660: 655f 6964 225d 203d 2069 6e6c 696e 655f  e_id"] = inline_
-0000c670: 6d65 7373 6167 655f 6964 0a20 2020 2069  message_id.    i
-0000c680: 6620 7265 706c 795f 6d61 726b 7570 3a0a  f reply_markup:.
-0000c690: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-0000c6a0: 2272 6570 6c79 5f6d 6172 6b75 7022 5d20  "reply_markup"] 
-0000c6b0: 3d20 6177 6169 7420 5f63 6f6e 7665 7274  = await _convert
-0000c6c0: 5f6d 6172 6b75 7028 7265 706c 795f 6d61  _markup(reply_ma
-0000c6d0: 726b 7570 290a 2020 2020 7265 7475 726e  rkup).    return
-0000c6e0: 2061 7761 6974 205f 7265 7175 6573 7428   await _request(
-0000c6f0: 746f 6b65 6e2c 206d 6574 686f 645f 7572  token, method_ur
-0000c700: 6c2c 2070 6172 616d 733d 7061 796c 6f61  l, params=payloa
-0000c710: 642c 206d 6574 686f 643d 2270 6f73 7422  d, method="post"
-0000c720: 290a 0a0a 6173 796e 6320 6465 6620 6465  )...async def de
-0000c730: 6c65 7465 5f6d 6573 7361 6765 2874 6f6b  lete_message(tok
-0000c740: 656e 2c20 6368 6174 5f69 642c 206d 6573  en, chat_id, mes
-0000c750: 7361 6765 5f69 642c 2074 696d 656f 7574  sage_id, timeout
-0000c760: 3d4e 6f6e 6529 3a0a 2020 2020 6d65 7468  =None):.    meth
-0000c770: 6f64 5f75 726c 203d 2072 2264 656c 6574  od_url = r"delet
-0000c780: 654d 6573 7361 6765 220a 2020 2020 7061  eMessage".    pa
-0000c790: 796c 6f61 6420 3d20 7b22 6368 6174 5f69  yload = {"chat_i
-0000c7a0: 6422 3a20 6368 6174 5f69 642c 2022 6d65  d": chat_id, "me
-0000c7b0: 7373 6167 655f 6964 223a 206d 6573 7361  ssage_id": messa
-0000c7c0: 6765 5f69 647d 0a20 2020 2069 6620 7469  ge_id}.    if ti
-0000c7d0: 6d65 6f75 743a 0a20 2020 2020 2020 2070  meout:.        p
-0000c7e0: 6179 6c6f 6164 5b22 7469 6d65 6f75 7422  ayload["timeout"
-0000c7f0: 5d20 3d20 7469 6d65 6f75 740a 2020 2020  ] = timeout.    
-0000c800: 7265 7475 726e 2061 7761 6974 205f 7265  return await _re
-0000c810: 7175 6573 7428 746f 6b65 6e2c 206d 6574  quest(token, met
-0000c820: 686f 645f 7572 6c2c 2070 6172 616d 733d  hod_url, params=
-0000c830: 7061 796c 6f61 642c 206d 6574 686f 643d  payload, method=
-0000c840: 2270 6f73 7422 290a 0a0a 2320 4761 6d65  "post")...# Game
-0000c850: 0a0a 0a61 7379 6e63 2064 6566 2073 656e  ...async def sen
-0000c860: 645f 6761 6d65 280a 2020 2020 746f 6b65  d_game(.    toke
-0000c870: 6e2c 0a20 2020 2063 6861 745f 6964 2c0a  n,.    chat_id,.
-0000c880: 2020 2020 6761 6d65 5f73 686f 7274 5f6e      game_short_n
-0000c890: 616d 652c 0a20 2020 2064 6973 6162 6c65  ame,.    disable
-0000c8a0: 5f6e 6f74 6966 6963 6174 696f 6e3d 4e6f  _notification=No
-0000c8b0: 6e65 2c0a 2020 2020 7265 706c 795f 746f  ne,.    reply_to
-0000c8c0: 5f6d 6573 7361 6765 5f69 643d 4e6f 6e65  _message_id=None
-0000c8d0: 2c0a 2020 2020 7265 706c 795f 6d61 726b  ,.    reply_mark
-0000c8e0: 7570 3d4e 6f6e 652c 0a20 2020 2074 696d  up=None,.    tim
-0000c8f0: 656f 7574 3d4e 6f6e 652c 0a20 2020 2061  eout=None,.    a
-0000c900: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
-0000c910: 686f 7574 5f72 6570 6c79 3d4e 6f6e 652c  hout_reply=None,
-0000c920: 0a20 2020 2070 726f 7465 6374 5f63 6f6e  .    protect_con
-0000c930: 7465 6e74 3d4e 6f6e 652c 0a20 2020 206d  tent=None,.    m
-0000c940: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
-0000c950: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-0000c960: 3d20 4e6f 6e65 2c0a 293a 0a20 2020 206d  = None,.):.    m
-0000c970: 6574 686f 645f 7572 6c20 3d20 7222 7365  ethod_url = r"se
-0000c980: 6e64 4761 6d65 220a 2020 2020 7061 796c  ndGame".    payl
-0000c990: 6f61 6420 3d20 7b22 6368 6174 5f69 6422  oad = {"chat_id"
-0000c9a0: 3a20 6368 6174 5f69 642c 2022 6761 6d65  : chat_id, "game
-0000c9b0: 5f73 686f 7274 5f6e 616d 6522 3a20 6761  _short_name": ga
-0000c9c0: 6d65 5f73 686f 7274 5f6e 616d 657d 0a20  me_short_name}. 
-0000c9d0: 2020 2069 6620 6469 7361 626c 655f 6e6f     if disable_no
-0000c9e0: 7469 6669 6361 7469 6f6e 2069 7320 6e6f  tification is no
-0000c9f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000ca00: 7061 796c 6f61 645b 2264 6973 6162 6c65  payload["disable
-0000ca10: 5f6e 6f74 6966 6963 6174 696f 6e22 5d20  _notification"] 
-0000ca20: 3d20 6469 7361 626c 655f 6e6f 7469 6669  = disable_notifi
-0000ca30: 6361 7469 6f6e 0a20 2020 2069 6620 7265  cation.    if re
-0000ca40: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-0000ca50: 643a 0a20 2020 2020 2020 2070 6179 6c6f  d:.        paylo
-0000ca60: 6164 5b22 7265 706c 795f 746f 5f6d 6573  ad["reply_to_mes
-0000ca70: 7361 6765 5f69 6422 5d20 3d20 7265 706c  sage_id"] = repl
-0000ca80: 795f 746f 5f6d 6573 7361 6765 5f69 640a  y_to_message_id.
-0000ca90: 2020 2020 6966 2072 6570 6c79 5f6d 6172      if reply_mar
-0000caa0: 6b75 703a 0a20 2020 2020 2020 2070 6179  kup:.        pay
-0000cab0: 6c6f 6164 5b22 7265 706c 795f 6d61 726b  load["reply_mark
-0000cac0: 7570 225d 203d 2061 7761 6974 205f 636f  up"] = await _co
-0000cad0: 6e76 6572 745f 6d61 726b 7570 2872 6570  nvert_markup(rep
-0000cae0: 6c79 5f6d 6172 6b75 7029 0a20 2020 2069  ly_markup).    i
-0000caf0: 6620 7469 6d65 6f75 743a 0a20 2020 2020  f timeout:.     
-0000cb00: 2020 2070 6179 6c6f 6164 5b22 7469 6d65     payload["time
-0000cb10: 6f75 7422 5d20 3d20 7469 6d65 6f75 740a  out"] = timeout.
-0000cb20: 2020 2020 6966 2061 6c6c 6f77 5f73 656e      if allow_sen
-0000cb30: 6469 6e67 5f77 6974 686f 7574 5f72 6570  ding_without_rep
-0000cb40: 6c79 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ly is not None:.
-0000cb50: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-0000cb60: 2261 6c6c 6f77 5f73 656e 6469 6e67 5f77  "allow_sending_w
-0000cb70: 6974 686f 7574 5f72 6570 6c79 225d 203d  ithout_reply"] =
-0000cb80: 2061 6c6c 6f77 5f73 656e 6469 6e67 5f77   allow_sending_w
-0000cb90: 6974 686f 7574 5f72 6570 6c79 0a20 2020  ithout_reply.   
-0000cba0: 2069 6620 7072 6f74 6563 745f 636f 6e74   if protect_cont
-0000cbb0: 656e 7420 6973 206e 6f74 204e 6f6e 653a  ent is not None:
-0000cbc0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000cbd0: 5b22 7072 6f74 6563 745f 636f 6e74 656e  ["protect_conten
-0000cbe0: 7422 5d20 3d20 7072 6f74 6563 745f 636f  t"] = protect_co
-0000cbf0: 6e74 656e 740a 2020 2020 5f61 6464 5f6d  ntent.    _add_m
-0000cc00: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
-0000cc10: 2870 6179 6c6f 6164 2c20 6d65 7373 6167  (payload, messag
-0000cc20: 655f 7468 7265 6164 5f69 6429 0a20 2020  e_thread_id).   
-0000cc30: 2072 6574 7572 6e20 6177 6169 7420 5f72   return await _r
-0000cc40: 6571 7565 7374 2874 6f6b 656e 2c20 6d65  equest(token, me
-0000cc50: 7468 6f64 5f75 726c 2c20 7061 7261 6d73  thod_url, params
-0000cc60: 3d70 6179 6c6f 6164 290a 0a0a 2320 6874  =payload)...# ht
-0000cc70: 7470 733a 2f2f 636f 7265 2e74 656c 6567  tps://core.teleg
-0000cc80: 7261 6d2e 6f72 672f 626f 7473 2f61 7069  ram.org/bots/api
-0000cc90: 2373 6574 6761 6d65 7363 6f72 650a 6173  #setgamescore.as
-0000cca0: 796e 6320 6465 6620 7365 745f 6761 6d65  ync def set_game
-0000ccb0: 5f73 636f 7265 280a 2020 2020 746f 6b65  _score(.    toke
-0000ccc0: 6e2c 0a20 2020 2075 7365 725f 6964 2c0a  n,.    user_id,.
-0000ccd0: 2020 2020 7363 6f72 652c 0a20 2020 2066      score,.    f
-0000cce0: 6f72 6365 3d4e 6f6e 652c 0a20 2020 2064  orce=None,.    d
-0000ccf0: 6973 6162 6c65 5f65 6469 745f 6d65 7373  isable_edit_mess
-0000cd00: 6167 653d 4e6f 6e65 2c0a 2020 2020 6368  age=None,.    ch
-0000cd10: 6174 5f69 643d 4e6f 6e65 2c0a 2020 2020  at_id=None,.    
-0000cd20: 6d65 7373 6167 655f 6964 3d4e 6f6e 652c  message_id=None,
-0000cd30: 0a20 2020 2069 6e6c 696e 655f 6d65 7373  .    inline_mess
-0000cd40: 6167 655f 6964 3d4e 6f6e 652c 0a29 3a0a  age_id=None,.):.
-0000cd50: 2020 2020 2222 220a 2020 2020 5573 6520      """.    Use 
-0000cd60: 7468 6973 206d 6574 686f 6420 746f 2073  this method to s
-0000cd70: 6574 2074 6865 2073 636f 7265 206f 6620  et the score of 
-0000cd80: 7468 6520 7370 6563 6966 6965 6420 7573  the specified us
-0000cd90: 6572 2069 6e20 6120 6761 6d65 2e20 4f6e  er in a game. On
-0000cda0: 2073 7563 6365 7373 2c20 6966 2074 6865   success, if the
-0000cdb0: 206d 6573 7361 6765 2077 6173 2073 656e   message was sen
-0000cdc0: 7420 6279 2074 6865 2062 6f74 2c20 7265  t by the bot, re
-0000cdd0: 7475 726e 7320 7468 6520 6564 6974 6564  turns the edited
-0000cde0: 204d 6573 7361 6765 2c20 6f74 6865 7277   Message, otherw
-0000cdf0: 6973 6520 7265 7475 726e 7320 5472 7565  ise returns True
-0000ce00: 2e20 5265 7475 726e 7320 616e 2065 7272  . Returns an err
-0000ce10: 6f72 2c20 6966 2074 6865 206e 6577 2073  or, if the new s
-0000ce20: 636f 7265 2069 7320 6e6f 7420 6772 6561  core is not grea
-0000ce30: 7465 7220 7468 616e 2074 6865 2075 7365  ter than the use
-0000ce40: 7227 7320 6375 7272 656e 7420 7363 6f72  r's current scor
-0000ce50: 6520 696e 2074 6865 2063 6861 742e 0a20  e in the chat.. 
-0000ce60: 2020 203a 7061 7261 6d20 746f 6b65 6e3a     :param token:
-0000ce70: 2042 6f74 2773 2074 6f6b 656e 2028 796f   Bot's token (yo
-0000ce80: 7520 646f 6e27 7420 6e65 6564 2074 6f20  u don't need to 
-0000ce90: 6669 6c6c 2074 6869 7329 0a20 2020 203a  fill this).    :
-0000cea0: 7061 7261 6d20 7573 6572 5f69 643a 2055  param user_id: U
-0000ceb0: 7365 7220 6964 656e 7469 6669 6572 0a20  ser identifier. 
-0000cec0: 2020 203a 7061 7261 6d20 7363 6f72 653a     :param score:
-0000ced0: 204e 6577 2073 636f 7265 2c20 6d75 7374   New score, must
-0000cee0: 2062 6520 6e6f 6e2d 6e65 6761 7469 7665   be non-negative
-0000cef0: 0a20 2020 203a 7061 7261 6d20 666f 7263  .    :param forc
-0000cf00: 653a 2028 4f70 7469 6f6e 616c 2920 5061  e: (Optional) Pa
-0000cf10: 7373 2054 7275 652c 2069 6620 7468 6520  ss True, if the 
-0000cf20: 6869 6768 2073 636f 7265 2069 7320 616c  high score is al
-0000cf30: 6c6f 7765 6420 746f 2064 6563 7265 6173  lowed to decreas
-0000cf40: 652e 2054 6869 7320 6361 6e20 6265 2075  e. This can be u
-0000cf50: 7365 6675 6c20 7768 656e 2066 6978 696e  seful when fixin
-0000cf60: 6720 6d69 7374 616b 6573 206f 7220 6261  g mistakes or ba
-0000cf70: 6e6e 696e 6720 6368 6561 7465 7273 0a20  nning cheaters. 
-0000cf80: 2020 203a 7061 7261 6d20 6469 7361 626c     :param disabl
-0000cf90: 655f 6564 6974 5f6d 6573 7361 6765 3a20  e_edit_message: 
-0000cfa0: 284f 7074 696f 6e61 6c29 2050 6173 7320  (Optional) Pass 
-0000cfb0: 5472 7565 2c20 6966 2074 6865 2067 616d  True, if the gam
-0000cfc0: 6520 6d65 7373 6167 6520 7368 6f75 6c64  e message should
-0000cfd0: 206e 6f74 2062 6520 6175 746f 6d61 7469   not be automati
-0000cfe0: 6361 6c6c 7920 6564 6974 6564 2074 6f20  cally edited to 
-0000cff0: 696e 636c 7564 6520 7468 6520 6375 7272  include the curr
-0000d000: 656e 7420 7363 6f72 6562 6f61 7264 0a20  ent scoreboard. 
-0000d010: 2020 203a 7061 7261 6d20 6368 6174 5f69     :param chat_i
-0000d020: 643a 2028 4f70 7469 6f6e 616c 2c20 7265  d: (Optional, re
-0000d030: 7175 6972 6564 2069 6620 696e 6c69 6e65  quired if inline
-0000d040: 5f6d 6573 7361 6765 5f69 6420 6973 206e  _message_id is n
-0000d050: 6f74 2073 7065 6369 6669 6564 2920 556e  ot specified) Un
-0000d060: 6971 7565 2069 6465 6e74 6966 6965 7220  ique identifier 
-0000d070: 666f 7220 7468 6520 7461 7267 6574 2063  for the target c
-0000d080: 6861 7420 286f 7220 7573 6572 6e61 6d65  hat (or username
-0000d090: 206f 6620 7468 6520 7461 7267 6574 2063   of the target c
-0000d0a0: 6861 6e6e 656c 2069 6e20 7468 6520 666f  hannel in the fo
-0000d0b0: 726d 6174 2040 6368 616e 6e65 6c75 7365  rmat @channeluse
-0000d0c0: 726e 616d 6529 0a20 2020 203a 7061 7261  rname).    :para
-0000d0d0: 6d20 6d65 7373 6167 655f 6964 3a20 284f  m message_id: (O
-0000d0e0: 7074 696f 6e61 6c2c 2072 6571 7569 7265  ptional, require
-0000d0f0: 6420 6966 2069 6e6c 696e 655f 6d65 7373  d if inline_mess
-0000d100: 6167 655f 6964 2069 7320 6e6f 7420 7370  age_id is not sp
-0000d110: 6563 6966 6965 6429 2055 6e69 7175 6520  ecified) Unique 
-0000d120: 6964 656e 7469 6669 6572 206f 6620 7468  identifier of th
-0000d130: 6520 7365 6e74 206d 6573 7361 6765 0a20  e sent message. 
-0000d140: 2020 203a 7061 7261 6d20 696e 6c69 6e65     :param inline
-0000d150: 5f6d 6573 7361 6765 5f69 643a 2028 4f70  _message_id: (Op
-0000d160: 7469 6f6e 616c 2c20 7265 7175 6972 6564  tional, required
-0000d170: 2069 6620 6368 6174 5f69 6420 616e 6420   if chat_id and 
-0000d180: 6d65 7373 6167 655f 6964 2061 7265 206e  message_id are n
-0000d190: 6f74 2073 7065 6369 6669 6564 2920 4964  ot specified) Id
-0000d1a0: 656e 7469 6669 6572 206f 6620 7468 6520  entifier of the 
-0000d1b0: 696e 6c69 6e65 206d 6573 7361 6765 0a20  inline message. 
-0000d1c0: 2020 203a 7265 7475 726e 3a0a 2020 2020     :return:.    
-0000d1d0: 2222 220a 2020 2020 6d65 7468 6f64 5f75  """.    method_u
-0000d1e0: 726c 203d 2072 2273 6574 4761 6d65 5363  rl = r"setGameSc
-0000d1f0: 6f72 6522 0a20 2020 2070 6179 6c6f 6164  ore".    payload
-0000d200: 203d 207b 2275 7365 725f 6964 223a 2075   = {"user_id": u
-0000d210: 7365 725f 6964 2c20 2273 636f 7265 223a  ser_id, "score":
-0000d220: 2073 636f 7265 7d0a 2020 2020 6966 2066   score}.    if f
-0000d230: 6f72 6365 2069 7320 6e6f 7420 4e6f 6e65  orce is not None
-0000d240: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-0000d250: 645b 2266 6f72 6365 225d 203d 2066 6f72  d["force"] = for
-0000d260: 6365 0a20 2020 2069 6620 6368 6174 5f69  ce.    if chat_i
-0000d270: 643a 0a20 2020 2020 2020 2070 6179 6c6f  d:.        paylo
-0000d280: 6164 5b22 6368 6174 5f69 6422 5d20 3d20  ad["chat_id"] = 
-0000d290: 6368 6174 5f69 640a 2020 2020 6966 206d  chat_id.    if m
-0000d2a0: 6573 7361 6765 5f69 643a 0a20 2020 2020  essage_id:.     
-0000d2b0: 2020 2070 6179 6c6f 6164 5b22 6d65 7373     payload["mess
-0000d2c0: 6167 655f 6964 225d 203d 206d 6573 7361  age_id"] = messa
-0000d2d0: 6765 5f69 640a 2020 2020 6966 2069 6e6c  ge_id.    if inl
-0000d2e0: 696e 655f 6d65 7373 6167 655f 6964 3a0a  ine_message_id:.
-0000d2f0: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-0000d300: 2269 6e6c 696e 655f 6d65 7373 6167 655f  "inline_message_
-0000d310: 6964 225d 203d 2069 6e6c 696e 655f 6d65  id"] = inline_me
-0000d320: 7373 6167 655f 6964 0a20 2020 2069 6620  ssage_id.    if 
-0000d330: 6469 7361 626c 655f 6564 6974 5f6d 6573  disable_edit_mes
-0000d340: 7361 6765 2069 7320 6e6f 7420 4e6f 6e65  sage is not None
-0000d350: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-0000d360: 645b 2264 6973 6162 6c65 5f65 6469 745f  d["disable_edit_
-0000d370: 6d65 7373 6167 6522 5d20 3d20 6469 7361  message"] = disa
-0000d380: 626c 655f 6564 6974 5f6d 6573 7361 6765  ble_edit_message
-0000d390: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
-0000d3a0: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
-0000d3b0: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
-0000d3c0: 7261 6d73 3d70 6179 6c6f 6164 290a 0a0a  rams=payload)...
-0000d3d0: 2320 6874 7470 733a 2f2f 636f 7265 2e74  # https://core.t
-0000d3e0: 656c 6567 7261 6d2e 6f72 672f 626f 7473  elegram.org/bots
-0000d3f0: 2f61 7069 2367 6574 6761 6d65 6869 6768  /api#getgamehigh
-0000d400: 7363 6f72 6573 0a61 7379 6e63 2064 6566  scores.async def
-0000d410: 2067 6574 5f67 616d 655f 6869 6768 5f73   get_game_high_s
-0000d420: 636f 7265 7328 746f 6b65 6e2c 2075 7365  cores(token, use
-0000d430: 725f 6964 2c20 6368 6174 5f69 643d 4e6f  r_id, chat_id=No
-0000d440: 6e65 2c20 6d65 7373 6167 655f 6964 3d4e  ne, message_id=N
-0000d450: 6f6e 652c 2069 6e6c 696e 655f 6d65 7373  one, inline_mess
-0000d460: 6167 655f 6964 3d4e 6f6e 6529 3a0a 2020  age_id=None):.  
-0000d470: 2020 2222 220a 2020 2020 5573 6520 7468    """.    Use th
-0000d480: 6973 206d 6574 686f 6420 746f 2067 6574  is method to get
-0000d490: 2064 6174 6120 666f 7220 6869 6768 2073   data for high s
-0000d4a0: 636f 7265 2074 6162 6c65 732e 2057 696c  core tables. Wil
-0000d4b0: 6c20 7265 7475 726e 2074 6865 2073 636f  l return the sco
-0000d4c0: 7265 206f 6620 7468 6520 7370 6563 6966  re of the specif
-0000d4d0: 6965 6420 7573 6572 2061 6e64 2073 6576  ied user and sev
-0000d4e0: 6572 616c 206f 6620 6869 7320 6e65 6967  eral of his neig
-0000d4f0: 6862 6f72 7320 696e 2061 2067 616d 652e  hbors in a game.
-0000d500: 204f 6e20 7375 6363 6573 732c 2072 6574   On success, ret
-0000d510: 7572 6e73 2061 6e20 4172 7261 7920 6f66  urns an Array of
-0000d520: 2047 616d 6548 6967 6853 636f 7265 206f   GameHighScore o
-0000d530: 626a 6563 7473 2e0a 2020 2020 5468 6973  bjects..    This
-0000d540: 206d 6574 686f 6420 7769 6c6c 2063 7572   method will cur
-0000d550: 7265 6e74 6c79 2072 6574 7572 6e20 7363  rently return sc
-0000d560: 6f72 6573 2066 6f72 2074 6865 2074 6172  ores for the tar
-0000d570: 6765 7420 7573 6572 2c20 706c 7573 2074  get user, plus t
-0000d580: 776f 206f 6620 6869 7320 636c 6f73 6573  wo of his closes
-0000d590: 7420 6e65 6967 6862 6f72 7320 6f6e 2065  t neighbors on e
-0000d5a0: 6163 6820 7369 6465 2e20 5769 6c6c 2061  ach side. Will a
-0000d5b0: 6c73 6f20 7265 7475 726e 2074 6865 2074  lso return the t
-0000d5c0: 6f70 2074 6872 6565 2075 7365 7273 2069  op three users i
-0000d5d0: 6620 7468 6520 7573 6572 2061 6e64 2068  f the user and h
-0000d5e0: 6973 206e 6569 6768 626f 7273 2061 7265  is neighbors are
-0000d5f0: 206e 6f74 2061 6d6f 6e67 2074 6865 6d2e   not among them.
-0000d600: 2050 6c65 6173 6520 6e6f 7465 2074 6861   Please note tha
-0000d610: 7420 7468 6973 2062 6568 6176 696f 7220  t this behavior 
-0000d620: 6973 2073 7562 6a65 6374 2074 6f20 6368  is subject to ch
-0000d630: 616e 6765 2e0a 2020 2020 3a70 6172 616d  ange..    :param
-0000d640: 2074 6f6b 656e 3a20 426f 7427 7320 746f   token: Bot's to
-0000d650: 6b65 6e20 2879 6f75 2064 6f6e 2774 206e  ken (you don't n
-0000d660: 6565 6420 746f 2066 696c 6c20 7468 6973  eed to fill this
-0000d670: 290a 2020 2020 3a70 6172 616d 2075 7365  ).    :param use
-0000d680: 725f 6964 3a20 5461 7267 6574 2075 7365  r_id: Target use
-0000d690: 7220 6964 0a20 2020 203a 7061 7261 6d20  r id.    :param 
-0000d6a0: 6368 6174 5f69 643a 2028 4f70 7469 6f6e  chat_id: (Option
-0000d6b0: 616c 2c20 7265 7175 6972 6564 2069 6620  al, required if 
-0000d6c0: 696e 6c69 6e65 5f6d 6573 7361 6765 5f69  inline_message_i
-0000d6d0: 6420 6973 206e 6f74 2073 7065 6369 6669  d is not specifi
-0000d6e0: 6564 2920 556e 6971 7565 2069 6465 6e74  ed) Unique ident
-0000d6f0: 6966 6965 7220 666f 7220 7468 6520 7461  ifier for the ta
-0000d700: 7267 6574 2063 6861 7420 286f 7220 7573  rget chat (or us
-0000d710: 6572 6e61 6d65 206f 6620 7468 6520 7461  ername of the ta
-0000d720: 7267 6574 2063 6861 6e6e 656c 2069 6e20  rget channel in 
-0000d730: 7468 6520 666f 726d 6174 2040 6368 616e  the format @chan
-0000d740: 6e65 6c75 7365 726e 616d 6529 0a20 2020  nelusername).   
-0000d750: 203a 7061 7261 6d20 6d65 7373 6167 655f   :param message_
-0000d760: 6964 3a20 284f 7074 696f 6e61 6c2c 2072  id: (Optional, r
-0000d770: 6571 7569 7265 6420 6966 2069 6e6c 696e  equired if inlin
-0000d780: 655f 6d65 7373 6167 655f 6964 2069 7320  e_message_id is 
-0000d790: 6e6f 7420 7370 6563 6966 6965 6429 2055  not specified) U
-0000d7a0: 6e69 7175 6520 6964 656e 7469 6669 6572  nique identifier
-0000d7b0: 206f 6620 7468 6520 7365 6e74 206d 6573   of the sent mes
-0000d7c0: 7361 6765 0a20 2020 203a 7061 7261 6d20  sage.    :param 
-0000d7d0: 696e 6c69 6e65 5f6d 6573 7361 6765 5f69  inline_message_i
-0000d7e0: 643a 2028 4f70 7469 6f6e 616c 2c20 7265  d: (Optional, re
-0000d7f0: 7175 6972 6564 2069 6620 6368 6174 5f69  quired if chat_i
-0000d800: 6420 616e 6420 6d65 7373 6167 655f 6964  d and message_id
-0000d810: 2061 7265 206e 6f74 2073 7065 6369 6669   are not specifi
-0000d820: 6564 2920 4964 656e 7469 6669 6572 206f  ed) Identifier o
-0000d830: 6620 7468 6520 696e 6c69 6e65 206d 6573  f the inline mes
-0000d840: 7361 6765 0a20 2020 203a 7265 7475 726e  sage.    :return
-0000d850: 3a0a 2020 2020 2222 220a 2020 2020 6d65  :.    """.    me
-0000d860: 7468 6f64 5f75 726c 203d 2072 2267 6574  thod_url = r"get
-0000d870: 4761 6d65 4869 6768 5363 6f72 6573 220a  GameHighScores".
-0000d880: 2020 2020 7061 796c 6f61 6420 3d20 7b22      payload = {"
-0000d890: 7573 6572 5f69 6422 3a20 7573 6572 5f69  user_id": user_i
-0000d8a0: 647d 0a20 2020 2069 6620 6368 6174 5f69  d}.    if chat_i
-0000d8b0: 643a 0a20 2020 2020 2020 2070 6179 6c6f  d:.        paylo
-0000d8c0: 6164 5b22 6368 6174 5f69 6422 5d20 3d20  ad["chat_id"] = 
-0000d8d0: 6368 6174 5f69 640a 2020 2020 6966 206d  chat_id.    if m
-0000d8e0: 6573 7361 6765 5f69 643a 0a20 2020 2020  essage_id:.     
-0000d8f0: 2020 2070 6179 6c6f 6164 5b22 6d65 7373     payload["mess
-0000d900: 6167 655f 6964 225d 203d 206d 6573 7361  age_id"] = messa
-0000d910: 6765 5f69 640a 2020 2020 6966 2069 6e6c  ge_id.    if inl
-0000d920: 696e 655f 6d65 7373 6167 655f 6964 3a0a  ine_message_id:.
-0000d930: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-0000d940: 2269 6e6c 696e 655f 6d65 7373 6167 655f  "inline_message_
-0000d950: 6964 225d 203d 2069 6e6c 696e 655f 6d65  id"] = inline_me
-0000d960: 7373 6167 655f 6964 0a20 2020 2072 6574  ssage_id.    ret
-0000d970: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
-0000d980: 7374 2874 6f6b 656e 2c20 6d65 7468 6f64  st(token, method
-0000d990: 5f75 726c 2c20 7061 7261 6d73 3d70 6179  _url, params=pay
-0000d9a0: 6c6f 6164 290a 0a0a 2320 5061 796d 656e  load)...# Paymen
-0000d9b0: 7473 2028 6874 7470 733a 2f2f 636f 7265  ts (https://core
-0000d9c0: 2e74 656c 6567 7261 6d2e 6f72 672f 626f  .telegram.org/bo
-0000d9d0: 7473 2f61 7069 2370 6179 6d65 6e74 7329  ts/api#payments)
-0000d9e0: 0a0a 0a61 7379 6e63 2064 6566 2073 656e  ...async def sen
-0000d9f0: 645f 696e 766f 6963 6528 0a20 2020 2074  d_invoice(.    t
-0000da00: 6f6b 656e 2c0a 2020 2020 6368 6174 5f69  oken,.    chat_i
-0000da10: 642c 0a20 2020 2074 6974 6c65 2c0a 2020  d,.    title,.  
-0000da20: 2020 6465 7363 7269 7074 696f 6e2c 0a20    description,. 
-0000da30: 2020 2069 6e76 6f69 6365 5f70 6179 6c6f     invoice_paylo
-0000da40: 6164 2c0a 2020 2020 7072 6f76 6964 6572  ad,.    provider
-0000da50: 5f74 6f6b 656e 2c0a 2020 2020 6375 7272  _token,.    curr
-0000da60: 656e 6379 2c0a 2020 2020 7072 6963 6573  ency,.    prices
-0000da70: 2c0a 2020 2020 7374 6172 745f 7061 7261  ,.    start_para
-0000da80: 6d65 7465 723d 4e6f 6e65 2c0a 2020 2020  meter=None,.    
-0000da90: 7068 6f74 6f5f 7572 6c3d 4e6f 6e65 2c0a  photo_url=None,.
-0000daa0: 2020 2020 7068 6f74 6f5f 7369 7a65 3d4e      photo_size=N
-0000dab0: 6f6e 652c 0a20 2020 2070 686f 746f 5f77  one,.    photo_w
-0000dac0: 6964 7468 3d4e 6f6e 652c 0a20 2020 2070  idth=None,.    p
-0000dad0: 686f 746f 5f68 6569 6768 743d 4e6f 6e65  hoto_height=None
-0000dae0: 2c0a 2020 2020 6e65 6564 5f6e 616d 653d  ,.    need_name=
-0000daf0: 4e6f 6e65 2c0a 2020 2020 6e65 6564 5f70  None,.    need_p
-0000db00: 686f 6e65 5f6e 756d 6265 723d 4e6f 6e65  hone_number=None
-0000db10: 2c0a 2020 2020 6e65 6564 5f65 6d61 696c  ,.    need_email
-0000db20: 3d4e 6f6e 652c 0a20 2020 206e 6565 645f  =None,.    need_
-0000db30: 7368 6970 7069 6e67 5f61 6464 7265 7373  shipping_address
-0000db40: 3d4e 6f6e 652c 0a20 2020 2073 656e 645f  =None,.    send_
-0000db50: 7068 6f6e 655f 6e75 6d62 6572 5f74 6f5f  phone_number_to_
-0000db60: 7072 6f76 6964 6572 3d4e 6f6e 652c 0a20  provider=None,. 
-0000db70: 2020 2073 656e 645f 656d 6169 6c5f 746f     send_email_to
-0000db80: 5f70 726f 7669 6465 723d 4e6f 6e65 2c0a  _provider=None,.
-0000db90: 2020 2020 6973 5f66 6c65 7869 626c 653d      is_flexible=
-0000dba0: 4e6f 6e65 2c0a 2020 2020 6469 7361 626c  None,.    disabl
-0000dbb0: 655f 6e6f 7469 6669 6361 7469 6f6e 3d4e  e_notification=N
-0000dbc0: 6f6e 652c 0a20 2020 2072 6570 6c79 5f74  one,.    reply_t
-0000dbd0: 6f5f 6d65 7373 6167 655f 6964 3d4e 6f6e  o_message_id=Non
-0000dbe0: 652c 0a20 2020 2072 6570 6c79 5f6d 6172  e,.    reply_mar
-0000dbf0: 6b75 703d 4e6f 6e65 2c0a 2020 2020 7072  kup=None,.    pr
-0000dc00: 6f76 6964 6572 5f64 6174 613d 4e6f 6e65  ovider_data=None
-0000dc10: 2c0a 2020 2020 7469 6d65 6f75 743d 4e6f  ,.    timeout=No
-0000dc20: 6e65 2c0a 2020 2020 616c 6c6f 775f 7365  ne,.    allow_se
-0000dc30: 6e64 696e 675f 7769 7468 6f75 745f 7265  nding_without_re
-0000dc40: 706c 793d 4e6f 6e65 2c0a 2020 2020 6d61  ply=None,.    ma
-0000dc50: 785f 7469 705f 616d 6f75 6e74 3d4e 6f6e  x_tip_amount=Non
-0000dc60: 652c 0a20 2020 2073 7567 6765 7374 6564  e,.    suggested
-0000dc70: 5f74 6970 5f61 6d6f 756e 7473 3d4e 6f6e  _tip_amounts=Non
-0000dc80: 652c 0a20 2020 2070 726f 7465 6374 5f63  e,.    protect_c
-0000dc90: 6f6e 7465 6e74 3d4e 6f6e 652c 0a20 2020  ontent=None,.   
-0000dca0: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
-0000dcb0: 6964 3a20 4f70 7469 6f6e 616c 5b69 6e74  id: Optional[int
-0000dcc0: 5d20 3d20 4e6f 6e65 2c0a 293a 0a20 2020  ] = None,.):.   
-0000dcd0: 2022 2222 0a20 2020 2055 7365 2074 6869   """.    Use thi
-0000dce0: 7320 6d65 7468 6f64 2074 6f20 7365 6e64  s method to send
-0000dcf0: 2069 6e76 6f69 6365 732e 204f 6e20 7375   invoices. On su
-0000dd00: 6363 6573 732c 2074 6865 2073 656e 7420  ccess, the sent 
-0000dd10: 4d65 7373 6167 6520 6973 2072 6574 7572  Message is retur
-0000dd20: 6e65 642e 0a20 2020 203a 7061 7261 6d20  ned..    :param 
-0000dd30: 746f 6b65 6e3a 2042 6f74 2773 2074 6f6b  token: Bot's tok
-0000dd40: 656e 2028 796f 7520 646f 6e27 7420 6e65  en (you don't ne
-0000dd50: 6564 2074 6f20 6669 6c6c 2074 6869 7329  ed to fill this)
-0000dd60: 0a20 2020 203a 7061 7261 6d20 6368 6174  .    :param chat
-0000dd70: 5f69 643a 2055 6e69 7175 6520 6964 656e  _id: Unique iden
-0000dd80: 7469 6669 6572 2066 6f72 2074 6865 2074  tifier for the t
-0000dd90: 6172 6765 7420 7072 6976 6174 6520 6368  arget private ch
-0000dda0: 6174 0a20 2020 203a 7061 7261 6d20 7469  at.    :param ti
-0000ddb0: 746c 653a 2050 726f 6475 6374 206e 616d  tle: Product nam
-0000ddc0: 650a 2020 2020 3a70 6172 616d 2064 6573  e.    :param des
-0000ddd0: 6372 6970 7469 6f6e 3a20 5072 6f64 7563  cription: Produc
-0000dde0: 7420 6465 7363 7269 7074 696f 6e0a 2020  t description.  
-0000ddf0: 2020 3a70 6172 616d 2069 6e76 6f69 6365    :param invoice
-0000de00: 5f70 6179 6c6f 6164 3a20 426f 742d 6465  _payload: Bot-de
-0000de10: 6669 6e65 6420 696e 766f 6963 6520 7061  fined invoice pa
-0000de20: 796c 6f61 642c 2031 2d31 3238 2062 7974  yload, 1-128 byt
-0000de30: 6573 2e20 5468 6973 2077 696c 6c20 6e6f  es. This will no
-0000de40: 7420 6265 2064 6973 706c 6179 6564 2074  t be displayed t
-0000de50: 6f20 7468 6520 7573 6572 2c20 7573 6520  o the user, use 
-0000de60: 666f 7220 796f 7572 2069 6e74 6572 6e61  for your interna
-0000de70: 6c20 7072 6f63 6573 7365 732e 0a20 2020  l processes..   
-0000de80: 203a 7061 7261 6d20 7072 6f76 6964 6572   :param provider
-0000de90: 5f74 6f6b 656e 3a20 5061 796d 656e 7473  _token: Payments
-0000dea0: 2070 726f 7669 6465 7220 746f 6b65 6e2c   provider token,
-0000deb0: 206f 6274 6169 6e65 6420 7669 6120 4042   obtained via @B
-0000dec0: 6f74 6661 7468 6572 0a20 2020 203a 7061  otfather.    :pa
-0000ded0: 7261 6d20 6375 7272 656e 6379 3a20 5468  ram currency: Th
-0000dee0: 7265 652d 6c65 7474 6572 2049 534f 2034  ree-letter ISO 4
-0000def0: 3231 3720 6375 7272 656e 6379 2063 6f64  217 currency cod
-0000df00: 652c 2073 6565 2068 7474 7073 3a2f 2f63  e, see https://c
-0000df10: 6f72 652e 7465 6c65 6772 616d 2e6f 7267  ore.telegram.org
-0000df20: 2f62 6f74 732f 7061 796d 656e 7473 2373  /bots/payments#s
-0000df30: 7570 706f 7274 6564 2d63 7572 7265 6e63  upported-currenc
-0000df40: 6965 730a 2020 2020 3a70 6172 616d 2070  ies.    :param p
-0000df50: 7269 6365 733a 2050 7269 6365 2062 7265  rices: Price bre
-0000df60: 616b 646f 776e 2c20 6120 6c69 7374 206f  akdown, a list o
-0000df70: 6620 636f 6d70 6f6e 656e 7473 2028 652e  f components (e.
-0000df80: 672e 2070 726f 6475 6374 2070 7269 6365  g. product price
-0000df90: 2c20 7461 782c 2064 6973 636f 756e 742c  , tax, discount,
-0000dfa0: 2064 656c 6976 6572 7920 636f 7374 2c20   delivery cost, 
-0000dfb0: 6465 6c69 7665 7279 2074 6178 2c20 626f  delivery tax, bo
-0000dfc0: 6e75 732c 2065 7463 2e29 0a20 2020 203a  nus, etc.).    :
-0000dfd0: 7061 7261 6d20 7374 6172 745f 7061 7261  param start_para
-0000dfe0: 6d65 7465 723a 2055 6e69 7175 6520 6465  meter: Unique de
-0000dff0: 6570 2d6c 696e 6b69 6e67 2070 6172 616d  ep-linking param
-0000e000: 6574 6572 2074 6861 7420 6361 6e20 6265  eter that can be
-0000e010: 2075 7365 6420 746f 2067 656e 6572 6174   used to generat
-0000e020: 6520 7468 6973 2069 6e76 6f69 6365 2077  e this invoice w
-0000e030: 6865 6e20 7573 6564 2061 7320 6120 7374  hen used as a st
-0000e040: 6172 7420 7061 7261 6d65 7465 720a 2020  art parameter.  
-0000e050: 2020 3a70 6172 616d 2070 686f 746f 5f75    :param photo_u
-0000e060: 726c 3a20 5552 4c20 6f66 2074 6865 2070  rl: URL of the p
-0000e070: 726f 6475 6374 2070 686f 746f 2066 6f72  roduct photo for
-0000e080: 2074 6865 2069 6e76 6f69 6365 2e20 4361   the invoice. Ca
-0000e090: 6e20 6265 2061 2070 686f 746f 206f 6620  n be a photo of 
-0000e0a0: 7468 6520 676f 6f64 7320 6f72 2061 206d  the goods or a m
-0000e0b0: 6172 6b65 7469 6e67 2069 6d61 6765 2066  arketing image f
-0000e0c0: 6f72 2061 2073 6572 7669 6365 2e20 5065  or a service. Pe
-0000e0d0: 6f70 6c65 206c 696b 6520 6974 2062 6574  ople like it bet
-0000e0e0: 7465 7220 7768 656e 2074 6865 7920 7365  ter when they se
-0000e0f0: 6520 7768 6174 2074 6865 7920 6172 6520  e what they are 
-0000e100: 7061 7969 6e67 2066 6f72 2e0a 2020 2020  paying for..    
-0000e110: 3a70 6172 616d 2070 686f 746f 5f73 697a  :param photo_siz
-0000e120: 653a 2050 686f 746f 2073 697a 650a 2020  e: Photo size.  
-0000e130: 2020 3a70 6172 616d 2070 686f 746f 5f77    :param photo_w
-0000e140: 6964 7468 3a20 5068 6f74 6f20 7769 6474  idth: Photo widt
-0000e150: 680a 2020 2020 3a70 6172 616d 2070 686f  h.    :param pho
-0000e160: 746f 5f68 6569 6768 743a 2050 686f 746f  to_height: Photo
-0000e170: 2068 6569 6768 740a 2020 2020 3a70 6172   height.    :par
-0000e180: 616d 206e 6565 645f 6e61 6d65 3a20 5061  am need_name: Pa
-0000e190: 7373 2054 7275 652c 2069 6620 796f 7520  ss True, if you 
-0000e1a0: 7265 7175 6972 6520 7468 6520 7573 6572  require the user
-0000e1b0: 2773 2066 756c 6c20 6e61 6d65 2074 6f20  's full name to 
-0000e1c0: 636f 6d70 6c65 7465 2074 6865 206f 7264  complete the ord
-0000e1d0: 6572 0a20 2020 203a 7061 7261 6d20 6e65  er.    :param ne
-0000e1e0: 6564 5f70 686f 6e65 5f6e 756d 6265 723a  ed_phone_number:
-0000e1f0: 2050 6173 7320 5472 7565 2c20 6966 2079   Pass True, if y
-0000e200: 6f75 2072 6571 7569 7265 2074 6865 2075  ou require the u
-0000e210: 7365 7227 7320 7068 6f6e 6520 6e75 6d62  ser's phone numb
-0000e220: 6572 2074 6f20 636f 6d70 6c65 7465 2074  er to complete t
-0000e230: 6865 206f 7264 6572 0a20 2020 203a 7061  he order.    :pa
-0000e240: 7261 6d20 6e65 6564 5f65 6d61 696c 3a20  ram need_email: 
-0000e250: 5061 7373 2054 7275 652c 2069 6620 796f  Pass True, if yo
-0000e260: 7520 7265 7175 6972 6520 7468 6520 7573  u require the us
-0000e270: 6572 2773 2065 6d61 696c 2074 6f20 636f  er's email to co
-0000e280: 6d70 6c65 7465 2074 6865 206f 7264 6572  mplete the order
-0000e290: 0a20 2020 203a 7061 7261 6d20 6e65 6564  .    :param need
-0000e2a0: 5f73 6869 7070 696e 675f 6164 6472 6573  _shipping_addres
-0000e2b0: 733a 2050 6173 7320 5472 7565 2c20 6966  s: Pass True, if
-0000e2c0: 2079 6f75 2072 6571 7569 7265 2074 6865   you require the
-0000e2d0: 2075 7365 7227 7320 7368 6970 7069 6e67   user's shipping
-0000e2e0: 2061 6464 7265 7373 2074 6f20 636f 6d70   address to comp
-0000e2f0: 6c65 7465 2074 6865 206f 7264 6572 0a20  lete the order. 
-0000e300: 2020 203a 7061 7261 6d20 6973 5f66 6c65     :param is_fle
-0000e310: 7869 626c 653a 2050 6173 7320 5472 7565  xible: Pass True
-0000e320: 2c20 6966 2074 6865 2066 696e 616c 2070  , if the final p
-0000e330: 7269 6365 2064 6570 656e 6473 206f 6e20  rice depends on 
-0000e340: 7468 6520 7368 6970 7069 6e67 206d 6574  the shipping met
-0000e350: 686f 640a 2020 2020 3a70 6172 616d 2073  hod.    :param s
-0000e360: 656e 645f 7068 6f6e 655f 6e75 6d62 6572  end_phone_number
-0000e370: 5f74 6f5f 7072 6f76 6964 6572 3a20 5061  _to_provider: Pa
-0000e380: 7373 2054 7275 652c 2069 6620 7573 6572  ss True, if user
-0000e390: 2773 2070 686f 6e65 206e 756d 6265 7220  's phone number 
-0000e3a0: 7368 6f75 6c64 2062 6520 7365 6e74 2074  should be sent t
-0000e3b0: 6f20 7072 6f76 6964 6572 0a20 2020 203a  o provider.    :
-0000e3c0: 7061 7261 6d20 7365 6e64 5f65 6d61 696c  param send_email
-0000e3d0: 5f74 6f5f 7072 6f76 6964 6572 3a20 5061  _to_provider: Pa
-0000e3e0: 7373 2054 7275 652c 2069 6620 7573 6572  ss True, if user
-0000e3f0: 2773 2065 6d61 696c 2061 6464 7265 7373  's email address
-0000e400: 2073 686f 756c 6420 6265 2073 656e 7420   should be sent 
-0000e410: 746f 2070 726f 7669 6465 720a 2020 2020  to provider.    
-0000e420: 3a70 6172 616d 2064 6973 6162 6c65 5f6e  :param disable_n
-0000e430: 6f74 6966 6963 6174 696f 6e3a 2053 656e  otification: Sen
-0000e440: 6473 2074 6865 206d 6573 7361 6765 2073  ds the message s
-0000e450: 696c 656e 746c 792e 2055 7365 7273 2077  ilently. Users w
-0000e460: 696c 6c20 7265 6365 6976 6520 6120 6e6f  ill receive a no
-0000e470: 7469 6669 6361 7469 6f6e 2077 6974 6820  tification with 
-0000e480: 6e6f 2073 6f75 6e64 2e0a 2020 2020 3a70  no sound..    :p
-0000e490: 6172 616d 2072 6570 6c79 5f74 6f5f 6d65  aram reply_to_me
-0000e4a0: 7373 6167 655f 6964 3a20 4966 2074 6865  ssage_id: If the
-0000e4b0: 206d 6573 7361 6765 2069 7320 6120 7265   message is a re
-0000e4c0: 706c 792c 2049 4420 6f66 2074 6865 206f  ply, ID of the o
-0000e4d0: 7269 6769 6e61 6c20 6d65 7373 6167 650a  riginal message.
-0000e4e0: 2020 2020 3a70 6172 616d 2072 6570 6c79      :param reply
-0000e4f0: 5f6d 6172 6b75 703a 2041 204a 534f 4e2d  _markup: A JSON-
-0000e500: 7365 7269 616c 697a 6564 206f 626a 6563  serialized objec
-0000e510: 7420 666f 7220 616e 2069 6e6c 696e 6520  t for an inline 
-0000e520: 6b65 7962 6f61 7264 2e20 4966 2065 6d70  keyboard. If emp
-0000e530: 7479 2c20 6f6e 6520 2750 6179 2074 6f74  ty, one 'Pay tot
-0000e540: 616c 2070 7269 6365 2720 6275 7474 6f6e  al price' button
-0000e550: 2077 696c 6c20 6265 2073 686f 776e 2e20   will be shown. 
-0000e560: 4966 206e 6f74 2065 6d70 7479 2c20 7468  If not empty, th
-0000e570: 6520 6669 7273 7420 6275 7474 6f6e 206d  e first button m
-0000e580: 7573 7420 6265 2061 2050 6179 2062 7574  ust be a Pay but
-0000e590: 746f 6e0a 2020 2020 3a70 6172 616d 2070  ton.    :param p
-0000e5a0: 726f 7669 6465 725f 6461 7461 3a20 4120  rovider_data: A 
-0000e5b0: 4a53 4f4e 2d73 6572 6961 6c69 7a65 6420  JSON-serialized 
-0000e5c0: 6461 7461 2061 626f 7574 2074 6865 2069  data about the i
-0000e5d0: 6e76 6f69 6365 2c20 7768 6963 6820 7769  nvoice, which wi
-0000e5e0: 6c6c 2062 6520 7368 6172 6564 2077 6974  ll be shared wit
-0000e5f0: 6820 7468 6520 7061 796d 656e 7420 7072  h the payment pr
-0000e600: 6f76 6964 6572 2e20 4120 6465 7461 696c  ovider. A detail
-0000e610: 6564 2064 6573 6372 6970 7469 6f6e 206f  ed description o
-0000e620: 6620 7265 7175 6972 6564 2066 6965 6c64  f required field
-0000e630: 7320 7368 6f75 6c64 2062 6520 7072 6f76  s should be prov
-0000e640: 6964 6564 2062 7920 7468 6520 7061 796d  ided by the paym
-0000e650: 656e 7420 7072 6f76 6964 6572 2e0a 2020  ent provider..  
-0000e660: 2020 3a70 6172 616d 2074 696d 656f 7574    :param timeout
-0000e670: 3a0a 2020 2020 3a70 6172 616d 2061 6c6c  :.    :param all
-0000e680: 6f77 5f73 656e 6469 6e67 5f77 6974 686f  ow_sending_witho
-0000e690: 7574 5f72 6570 6c79 3a0a 2020 2020 3a70  ut_reply:.    :p
-0000e6a0: 6172 616d 206d 6178 5f74 6970 5f61 6d6f  aram max_tip_amo
-0000e6b0: 756e 743a 2054 6865 206d 6178 696d 756d  unt: The maximum
-0000e6c0: 2061 6363 6570 7465 6420 616d 6f75 6e74   accepted amount
-0000e6d0: 2066 6f72 2074 6970 7320 696e 2074 6865   for tips in the
-0000e6e0: 2073 6d61 6c6c 6573 7420 756e 6974 7320   smallest units 
-0000e6f0: 6f66 2074 6865 2063 7572 7265 6e63 790a  of the currency.
-0000e700: 2020 2020 3a70 6172 616d 2073 7567 6765      :param sugge
-0000e710: 7374 6564 5f74 6970 5f61 6d6f 756e 7473  sted_tip_amounts
-0000e720: 3a20 4120 4a53 4f4e 2d73 6572 6961 6c69  : A JSON-seriali
-0000e730: 7a65 6420 6172 7261 7920 6f66 2073 7567  zed array of sug
-0000e740: 6765 7374 6564 2061 6d6f 756e 7473 206f  gested amounts o
-0000e750: 6620 7469 7073 2069 6e20 7468 6520 736d  f tips in the sm
-0000e760: 616c 6c65 7374 2075 6e69 7473 206f 6620  allest units of 
-0000e770: 7468 6520 6375 7272 656e 6379 2e0a 2020  the currency..  
-0000e780: 2020 2020 2020 4174 206d 6f73 7420 3420        At most 4 
-0000e790: 7375 6767 6573 7465 6420 7469 7020 616d  suggested tip am
-0000e7a0: 6f75 6e74 7320 6361 6e20 6265 2073 7065  ounts can be spe
-0000e7b0: 6369 6669 6564 2e20 5468 6520 7375 6767  cified. The sugg
-0000e7c0: 6573 7465 6420 7469 7020 616d 6f75 6e74  ested tip amount
-0000e7d0: 7320 6d75 7374 2062 6520 706f 7369 7469  s must be positi
-0000e7e0: 7665 2c20 7061 7373 6564 2069 6e20 6120  ve, passed in a 
-0000e7f0: 7374 7269 6374 6c79 2069 6e63 7265 6173  strictly increas
-0000e800: 6564 206f 7264 6572 2061 6e64 206d 7573  ed order and mus
-0000e810: 7420 6e6f 7420 6578 6365 6564 206d 6178  t not exceed max
-0000e820: 5f74 6970 5f61 6d6f 756e 742e 0a20 2020  _tip_amount..   
-0000e830: 203a 7061 7261 6d20 7072 6f74 6563 745f   :param protect_
-0000e840: 636f 6e74 656e 743a 0a20 2020 203a 7265  content:.    :re
-0000e850: 7475 726e 3a0a 2020 2020 2222 220a 2020  turn:.    """.  
-0000e860: 2020 6d65 7468 6f64 5f75 726c 203d 2072    method_url = r
-0000e870: 2273 656e 6449 6e76 6f69 6365 220a 2020  "sendInvoice".  
-0000e880: 2020 7061 796c 6f61 6420 3d20 7b0a 2020    payload = {.  
-0000e890: 2020 2020 2020 2263 6861 745f 6964 223a        "chat_id":
-0000e8a0: 2063 6861 745f 6964 2c0a 2020 2020 2020   chat_id,.      
-0000e8b0: 2020 2274 6974 6c65 223a 2074 6974 6c65    "title": title
-0000e8c0: 2c0a 2020 2020 2020 2020 2264 6573 6372  ,.        "descr
-0000e8d0: 6970 7469 6f6e 223a 2064 6573 6372 6970  iption": descrip
-0000e8e0: 7469 6f6e 2c0a 2020 2020 2020 2020 2270  tion,.        "p
-0000e8f0: 6179 6c6f 6164 223a 2069 6e76 6f69 6365  ayload": invoice
-0000e900: 5f70 6179 6c6f 6164 2c0a 2020 2020 2020  _payload,.      
-0000e910: 2020 2270 726f 7669 6465 725f 746f 6b65    "provider_toke
-0000e920: 6e22 3a20 7072 6f76 6964 6572 5f74 6f6b  n": provider_tok
-0000e930: 656e 2c0a 2020 2020 2020 2020 2263 7572  en,.        "cur
-0000e940: 7265 6e63 7922 3a20 6375 7272 656e 6379  rency": currency
-0000e950: 2c0a 2020 2020 2020 2020 2270 7269 6365  ,.        "price
-0000e960: 7322 3a20 6177 6169 7420 5f63 6f6e 7665  s": await _conve
-0000e970: 7274 5f6c 6973 745f 6a73 6f6e 5f73 6572  rt_list_json_ser
-0000e980: 6961 6c69 7a61 626c 6528 7072 6963 6573  ializable(prices
-0000e990: 292c 0a20 2020 207d 0a20 2020 2069 6620  ),.    }.    if 
-0000e9a0: 7374 6172 745f 7061 7261 6d65 7465 723a  start_parameter:
-0000e9b0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000e9c0: 5b22 7374 6172 745f 7061 7261 6d65 7465  ["start_paramete
-0000e9d0: 7222 5d20 3d20 7374 6172 745f 7061 7261  r"] = start_para
-0000e9e0: 6d65 7465 720a 2020 2020 6966 2070 686f  meter.    if pho
-0000e9f0: 746f 5f75 726c 3a0a 2020 2020 2020 2020  to_url:.        
-0000ea00: 7061 796c 6f61 645b 2270 686f 746f 5f75  payload["photo_u
-0000ea10: 726c 225d 203d 2070 686f 746f 5f75 726c  rl"] = photo_url
-0000ea20: 0a20 2020 2069 6620 7068 6f74 6f5f 7369  .    if photo_si
-0000ea30: 7a65 3a0a 2020 2020 2020 2020 7061 796c  ze:.        payl
-0000ea40: 6f61 645b 2270 686f 746f 5f73 697a 6522  oad["photo_size"
-0000ea50: 5d20 3d20 7068 6f74 6f5f 7369 7a65 0a20  ] = photo_size. 
-0000ea60: 2020 2069 6620 7068 6f74 6f5f 7769 6474     if photo_widt
-0000ea70: 683a 0a20 2020 2020 2020 2070 6179 6c6f  h:.        paylo
-0000ea80: 6164 5b22 7068 6f74 6f5f 7769 6474 6822  ad["photo_width"
-0000ea90: 5d20 3d20 7068 6f74 6f5f 7769 6474 680a  ] = photo_width.
-0000eaa0: 2020 2020 6966 2070 686f 746f 5f68 6569      if photo_hei
-0000eab0: 6768 743a 0a20 2020 2020 2020 2070 6179  ght:.        pay
-0000eac0: 6c6f 6164 5b22 7068 6f74 6f5f 6865 6967  load["photo_heig
-0000ead0: 6874 225d 203d 2070 686f 746f 5f68 6569  ht"] = photo_hei
-0000eae0: 6768 740a 2020 2020 6966 206e 6565 645f  ght.    if need_
-0000eaf0: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
-0000eb00: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-0000eb10: 645b 226e 6565 645f 6e61 6d65 225d 203d  d["need_name"] =
-0000eb20: 206e 6565 645f 6e61 6d65 0a20 2020 2069   need_name.    i
-0000eb30: 6620 6e65 6564 5f70 686f 6e65 5f6e 756d  f need_phone_num
-0000eb40: 6265 7220 6973 206e 6f74 204e 6f6e 653a  ber is not None:
-0000eb50: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000eb60: 5b22 6e65 6564 5f70 686f 6e65 5f6e 756d  ["need_phone_num
-0000eb70: 6265 7222 5d20 3d20 6e65 6564 5f70 686f  ber"] = need_pho
-0000eb80: 6e65 5f6e 756d 6265 720a 2020 2020 6966  ne_number.    if
-0000eb90: 206e 6565 645f 656d 6169 6c20 6973 206e   need_email is n
-0000eba0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000ebb0: 2070 6179 6c6f 6164 5b22 6e65 6564 5f65   payload["need_e
-0000ebc0: 6d61 696c 225d 203d 206e 6565 645f 656d  mail"] = need_em
-0000ebd0: 6169 6c0a 2020 2020 6966 206e 6565 645f  ail.    if need_
-0000ebe0: 7368 6970 7069 6e67 5f61 6464 7265 7373  shipping_address
-0000ebf0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000ec00: 2020 2020 2020 7061 796c 6f61 645b 226e        payload["n
-0000ec10: 6565 645f 7368 6970 7069 6e67 5f61 6464  eed_shipping_add
-0000ec20: 7265 7373 225d 203d 206e 6565 645f 7368  ress"] = need_sh
-0000ec30: 6970 7069 6e67 5f61 6464 7265 7373 0a20  ipping_address. 
-0000ec40: 2020 2069 6620 7365 6e64 5f70 686f 6e65     if send_phone
-0000ec50: 5f6e 756d 6265 725f 746f 5f70 726f 7669  _number_to_provi
-0000ec60: 6465 7220 6973 206e 6f74 204e 6f6e 653a  der is not None:
-0000ec70: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000ec80: 5b22 7365 6e64 5f70 686f 6e65 5f6e 756d  ["send_phone_num
-0000ec90: 6265 725f 746f 5f70 726f 7669 6465 7222  ber_to_provider"
-0000eca0: 5d20 3d20 7365 6e64 5f70 686f 6e65 5f6e  ] = send_phone_n
-0000ecb0: 756d 6265 725f 746f 5f70 726f 7669 6465  umber_to_provide
-0000ecc0: 720a 2020 2020 6966 2073 656e 645f 656d  r.    if send_em
-0000ecd0: 6169 6c5f 746f 5f70 726f 7669 6465 7220  ail_to_provider 
-0000ece0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000ecf0: 2020 2020 2070 6179 6c6f 6164 5b22 7365       payload["se
-0000ed00: 6e64 5f65 6d61 696c 5f74 6f5f 7072 6f76  nd_email_to_prov
-0000ed10: 6964 6572 225d 203d 2073 656e 645f 656d  ider"] = send_em
-0000ed20: 6169 6c5f 746f 5f70 726f 7669 6465 720a  ail_to_provider.
-0000ed30: 2020 2020 6966 2069 735f 666c 6578 6962      if is_flexib
-0000ed40: 6c65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  le is not None:.
-0000ed50: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-0000ed60: 2269 735f 666c 6578 6962 6c65 225d 203d  "is_flexible"] =
-0000ed70: 2069 735f 666c 6578 6962 6c65 0a20 2020   is_flexible.   
-0000ed80: 2069 6620 6469 7361 626c 655f 6e6f 7469   if disable_noti
-0000ed90: 6669 6361 7469 6f6e 2069 7320 6e6f 7420  fication is not 
-0000eda0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
-0000edb0: 796c 6f61 645b 2264 6973 6162 6c65 5f6e  yload["disable_n
-0000edc0: 6f74 6966 6963 6174 696f 6e22 5d20 3d20  otification"] = 
-0000edd0: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-0000ede0: 7469 6f6e 0a20 2020 2069 6620 7265 706c  tion.    if repl
-0000edf0: 795f 746f 5f6d 6573 7361 6765 5f69 643a  y_to_message_id:
-0000ee00: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-0000ee10: 5b22 7265 706c 795f 746f 5f6d 6573 7361  ["reply_to_messa
-0000ee20: 6765 5f69 6422 5d20 3d20 7265 706c 795f  ge_id"] = reply_
-0000ee30: 746f 5f6d 6573 7361 6765 5f69 640a 2020  to_message_id.  
-0000ee40: 2020 6966 2072 6570 6c79 5f6d 6172 6b75    if reply_marku
-0000ee50: 703a 0a20 2020 2020 2020 2070 6179 6c6f  p:.        paylo
-0000ee60: 6164 5b22 7265 706c 795f 6d61 726b 7570  ad["reply_markup
-0000ee70: 225d 203d 2061 7761 6974 205f 636f 6e76  "] = await _conv
-0000ee80: 6572 745f 6d61 726b 7570 2872 6570 6c79  ert_markup(reply
-0000ee90: 5f6d 6172 6b75 7029 0a20 2020 2069 6620  _markup).    if 
-0000eea0: 7072 6f76 6964 6572 5f64 6174 613a 0a20  provider_data:. 
-0000eeb0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-0000eec0: 7072 6f76 6964 6572 5f64 6174 6122 5d20  provider_data"] 
-0000eed0: 3d20 7072 6f76 6964 6572 5f64 6174 610a  = provider_data.
-0000eee0: 2020 2020 6966 2074 696d 656f 7574 3a0a      if timeout:.
-0000eef0: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-0000ef00: 2274 696d 656f 7574 225d 203d 2074 696d  "timeout"] = tim
-0000ef10: 656f 7574 0a20 2020 2069 6620 616c 6c6f  eout.    if allo
-0000ef20: 775f 7365 6e64 696e 675f 7769 7468 6f75  w_sending_withou
-0000ef30: 745f 7265 706c 7920 6973 206e 6f74 204e  t_reply is not N
-0000ef40: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
-0000ef50: 6c6f 6164 5b22 616c 6c6f 775f 7365 6e64  load["allow_send
-0000ef60: 696e 675f 7769 7468 6f75 745f 7265 706c  ing_without_repl
-0000ef70: 7922 5d20 3d20 616c 6c6f 775f 7365 6e64  y"] = allow_send
-0000ef80: 696e 675f 7769 7468 6f75 745f 7265 706c  ing_without_repl
-0000ef90: 790a 2020 2020 6966 206d 6178 5f74 6970  y.    if max_tip
-0000efa0: 5f61 6d6f 756e 7420 6973 206e 6f74 204e  _amount is not N
-0000efb0: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
-0000efc0: 6c6f 6164 5b22 6d61 785f 7469 705f 616d  load["max_tip_am
-0000efd0: 6f75 6e74 225d 203d 206d 6178 5f74 6970  ount"] = max_tip
-0000efe0: 5f61 6d6f 756e 740a 2020 2020 6966 2073  _amount.    if s
-0000eff0: 7567 6765 7374 6564 5f74 6970 5f61 6d6f  uggested_tip_amo
-0000f000: 756e 7473 2069 7320 6e6f 7420 4e6f 6e65  unts is not None
-0000f010: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-0000f020: 645b 2273 7567 6765 7374 6564 5f74 6970  d["suggested_tip
-0000f030: 5f61 6d6f 756e 7473 225d 203d 206a 736f  _amounts"] = jso
-0000f040: 6e2e 6475 6d70 7328 7375 6767 6573 7465  n.dumps(suggeste
-0000f050: 645f 7469 705f 616d 6f75 6e74 7329 0a20  d_tip_amounts). 
-0000f060: 2020 2069 6620 7072 6f74 6563 745f 636f     if protect_co
-0000f070: 6e74 656e 7420 6973 206e 6f74 204e 6f6e  ntent is not Non
-0000f080: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-0000f090: 6164 5b22 7072 6f74 6563 745f 636f 6e74  ad["protect_cont
-0000f0a0: 656e 7422 5d20 3d20 7072 6f74 6563 745f  ent"] = protect_
-0000f0b0: 636f 6e74 656e 740a 2020 2020 5f61 6464  content.    _add
-0000f0c0: 5f6d 6573 7361 6765 5f74 6872 6561 645f  _message_thread_
-0000f0d0: 6964 2870 6179 6c6f 6164 2c20 6d65 7373  id(payload, mess
-0000f0e0: 6167 655f 7468 7265 6164 5f69 6429 0a20  age_thread_id). 
-0000f0f0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-0000f100: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
-0000f110: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
-0000f120: 6d73 3d70 6179 6c6f 6164 290a 0a0a 6173  ms=payload)...as
-0000f130: 796e 6320 6465 6620 616e 7377 6572 5f73  ync def answer_s
-0000f140: 6869 7070 696e 675f 7175 6572 7928 746f  hipping_query(to
-0000f150: 6b65 6e2c 2073 6869 7070 696e 675f 7175  ken, shipping_qu
-0000f160: 6572 795f 6964 2c20 6f6b 2c20 7368 6970  ery_id, ok, ship
-0000f170: 7069 6e67 5f6f 7074 696f 6e73 3d4e 6f6e  ping_options=Non
-0000f180: 652c 2065 7272 6f72 5f6d 6573 7361 6765  e, error_message
-0000f190: 3d4e 6f6e 6529 3a0a 2020 2020 2222 220a  =None):.    """.
-0000f1a0: 2020 2020 4966 2079 6f75 2073 656e 7420      If you sent 
-0000f1b0: 616e 2069 6e76 6f69 6365 2072 6571 7565  an invoice reque
-0000f1c0: 7374 696e 6720 6120 7368 6970 7069 6e67  sting a shipping
-0000f1d0: 2061 6464 7265 7373 2061 6e64 2074 6865   address and the
-0000f1e0: 2070 6172 616d 6574 6572 2069 735f 666c   parameter is_fl
-0000f1f0: 6578 6962 6c65 2077 6173 2073 7065 6369  exible was speci
-0000f200: 6669 6564 2c20 7468 6520 426f 7420 4150  fied, the Bot AP
-0000f210: 4920 7769 6c6c 2073 656e 6420 616e 2055  I will send an U
-0000f220: 7064 6174 6520 7769 7468 2061 2073 6869  pdate with a shi
-0000f230: 7070 696e 675f 7175 6572 7920 6669 656c  pping_query fiel
-0000f240: 6420 746f 2074 6865 2062 6f74 2e20 5573  d to the bot. Us
-0000f250: 6520 7468 6973 206d 6574 686f 6420 746f  e this method to
-0000f260: 2072 6570 6c79 2074 6f20 7368 6970 7069   reply to shippi
-0000f270: 6e67 2071 7565 7269 6573 2e20 4f6e 2073  ng queries. On s
-0000f280: 7563 6365 7373 2c20 5472 7565 2069 7320  uccess, True is 
-0000f290: 7265 7475 726e 6564 2e0a 2020 2020 3a70  returned..    :p
-0000f2a0: 6172 616d 2074 6f6b 656e 3a20 426f 7427  aram token: Bot'
-0000f2b0: 7320 746f 6b65 6e20 2879 6f75 2064 6f6e  s token (you don
-0000f2c0: 2774 206e 6565 6420 746f 2066 696c 6c20  't need to fill 
-0000f2d0: 7468 6973 290a 2020 2020 3a70 6172 616d  this).    :param
-0000f2e0: 2073 6869 7070 696e 675f 7175 6572 795f   shipping_query_
-0000f2f0: 6964 3a20 556e 6971 7565 2069 6465 6e74  id: Unique ident
-0000f300: 6966 6965 7220 666f 7220 7468 6520 7175  ifier for the qu
-0000f310: 6572 7920 746f 2062 6520 616e 7377 6572  ery to be answer
-0000f320: 6564 0a20 2020 203a 7061 7261 6d20 6f6b  ed.    :param ok
-0000f330: 3a20 5370 6563 6966 7920 5472 7565 2069  : Specify True i
-0000f340: 6620 6465 6c69 7665 7279 2074 6f20 7468  f delivery to th
-0000f350: 6520 7370 6563 6966 6965 6420 6164 6472  e specified addr
-0000f360: 6573 7320 6973 2070 6f73 7369 626c 6520  ess is possible 
-0000f370: 616e 6420 4661 6c73 6520 6966 2074 6865  and False if the
-0000f380: 7265 2061 7265 2061 6e79 2070 726f 626c  re are any probl
-0000f390: 656d 7320 2866 6f72 2065 7861 6d70 6c65  ems (for example
-0000f3a0: 2c20 6966 2064 656c 6976 6572 7920 746f  , if delivery to
-0000f3b0: 2074 6865 2073 7065 6369 6669 6564 2061   the specified a
-0000f3c0: 6464 7265 7373 2069 7320 6e6f 7420 706f  ddress is not po
-0000f3d0: 7373 6962 6c65 290a 2020 2020 3a70 6172  ssible).    :par
-0000f3e0: 616d 2073 6869 7070 696e 675f 6f70 7469  am shipping_opti
-0000f3f0: 6f6e 733a 2052 6571 7569 7265 6420 6966  ons: Required if
-0000f400: 206f 6b20 6973 2054 7275 652e 2041 204a   ok is True. A J
-0000f410: 534f 4e2d 7365 7269 616c 697a 6564 2061  SON-serialized a
-0000f420: 7272 6179 206f 6620 6176 6169 6c61 626c  rray of availabl
-0000f430: 6520 7368 6970 7069 6e67 206f 7074 696f  e shipping optio
-0000f440: 6e73 2e0a 2020 2020 3a70 6172 616d 2065  ns..    :param e
-0000f450: 7272 6f72 5f6d 6573 7361 6765 3a20 5265  rror_message: Re
-0000f460: 7175 6972 6564 2069 6620 6f6b 2069 7320  quired if ok is 
-0000f470: 4661 6c73 652e 2045 7272 6f72 206d 6573  False. Error mes
-0000f480: 7361 6765 2069 6e20 6875 6d61 6e20 7265  sage in human re
-0000f490: 6164 6162 6c65 2066 6f72 6d20 7468 6174  adable form that
-0000f4a0: 2065 7870 6c61 696e 7320 7768 7920 6974   explains why it
-0000f4b0: 2069 7320 696d 706f 7373 6962 6c65 2074   is impossible t
-0000f4c0: 6f20 636f 6d70 6c65 7465 2074 6865 206f  o complete the o
-0000f4d0: 7264 6572 2028 652e 672e 2022 536f 7272  rder (e.g. "Sorr
-0000f4e0: 792c 2064 656c 6976 6572 7920 746f 2079  y, delivery to y
-0000f4f0: 6f75 7220 6465 7369 7265 6420 6164 6472  our desired addr
-0000f500: 6573 7320 6973 2075 6e61 7661 696c 6162  ess is unavailab
-0000f510: 6c65 2729 2e20 5465 6c65 6772 616d 2077  le'). Telegram w
-0000f520: 696c 6c20 6469 7370 6c61 7920 7468 6973  ill display this
-0000f530: 206d 6573 7361 6765 2074 6f20 7468 6520   message to the 
-0000f540: 7573 6572 2e0a 2020 2020 3a72 6574 7572  user..    :retur
-0000f550: 6e3a 0a20 2020 2022 2222 0a20 2020 206d  n:.    """.    m
-0000f560: 6574 686f 645f 7572 6c20 3d20 2261 6e73  ethod_url = "ans
-0000f570: 7765 7253 6869 7070 696e 6751 7565 7279  werShippingQuery
-0000f580: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
-0000f590: 7b22 7368 6970 7069 6e67 5f71 7565 7279  {"shipping_query
-0000f5a0: 5f69 6422 3a20 7368 6970 7069 6e67 5f71  _id": shipping_q
-0000f5b0: 7565 7279 5f69 642c 2022 6f6b 223a 206f  uery_id, "ok": o
-0000f5c0: 6b7d 0a20 2020 2069 6620 7368 6970 7069  k}.    if shippi
-0000f5d0: 6e67 5f6f 7074 696f 6e73 3a0a 2020 2020  ng_options:.    
-0000f5e0: 2020 2020 7061 796c 6f61 645b 2273 6869      payload["shi
-0000f5f0: 7070 696e 675f 6f70 7469 6f6e 7322 5d20  pping_options"] 
-0000f600: 3d20 6177 6169 7420 5f63 6f6e 7665 7274  = await _convert
-0000f610: 5f6c 6973 745f 6a73 6f6e 5f73 6572 6961  _list_json_seria
-0000f620: 6c69 7a61 626c 6528 7368 6970 7069 6e67  lizable(shipping
-0000f630: 5f6f 7074 696f 6e73 290a 2020 2020 6966  _options).    if
-0000f640: 2065 7272 6f72 5f6d 6573 7361 6765 3a0a   error_message:.
-0000f650: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-0000f660: 2265 7272 6f72 5f6d 6573 7361 6765 225d  "error_message"]
-0000f670: 203d 2065 7272 6f72 5f6d 6573 7361 6765   = error_message
-0000f680: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
-0000f690: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
-0000f6a0: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
-0000f6b0: 7261 6d73 3d70 6179 6c6f 6164 290a 0a0a  rams=payload)...
-0000f6c0: 6173 796e 6320 6465 6620 616e 7377 6572  async def answer
-0000f6d0: 5f70 7265 5f63 6865 636b 6f75 745f 7175  _pre_checkout_qu
-0000f6e0: 6572 7928 746f 6b65 6e2c 2070 7265 5f63  ery(token, pre_c
-0000f6f0: 6865 636b 6f75 745f 7175 6572 795f 6964  heckout_query_id
-0000f700: 2c20 6f6b 2c20 6572 726f 725f 6d65 7373  , ok, error_mess
-0000f710: 6167 653d 4e6f 6e65 293a 0a20 2020 2022  age=None):.    "
-0000f720: 2222 0a20 2020 204f 6e63 6520 7468 6520  "".    Once the 
-0000f730: 7573 6572 2068 6173 2063 6f6e 6669 726d  user has confirm
-0000f740: 6564 2074 6865 6972 2070 6179 6d65 6e74  ed their payment
-0000f750: 2061 6e64 2073 6869 7070 696e 6720 6465   and shipping de
-0000f760: 7461 696c 732c 2074 6865 2042 6f74 2041  tails, the Bot A
-0000f770: 5049 2073 656e 6473 2074 6865 2066 696e  PI sends the fin
-0000f780: 616c 2063 6f6e 6669 726d 6174 696f 6e20  al confirmation 
-0000f790: 696e 2074 6865 2066 6f72 6d20 6f66 2061  in the form of a
-0000f7a0: 6e20 5570 6461 7465 2077 6974 6820 7468  n Update with th
-0000f7b0: 6520 6669 656c 6420 7072 655f 6368 6563  e field pre_chec
-0000f7c0: 6b6f 7574 5f71 7565 7279 2e20 5573 6520  kout_query. Use 
-0000f7d0: 7468 6973 206d 6574 686f 6420 746f 2072  this method to r
-0000f7e0: 6573 706f 6e64 2074 6f20 7375 6368 2070  espond to such p
-0000f7f0: 7265 2d63 6865 636b 6f75 7420 7175 6572  re-checkout quer
-0000f800: 6965 732e 204f 6e20 7375 6363 6573 732c  ies. On success,
-0000f810: 2054 7275 6520 6973 2072 6574 7572 6e65   True is returne
-0000f820: 642e 204e 6f74 653a 2054 6865 2042 6f74  d. Note: The Bot
-0000f830: 2041 5049 206d 7573 7420 7265 6365 6976   API must receiv
-0000f840: 6520 616e 2061 6e73 7765 7220 7769 7468  e an answer with
-0000f850: 696e 2031 3020 7365 636f 6e64 7320 6166  in 10 seconds af
-0000f860: 7465 7220 7468 6520 7072 652d 6368 6563  ter the pre-chec
-0000f870: 6b6f 7574 2071 7565 7279 2077 6173 2073  kout query was s
-0000f880: 656e 742e 0a20 2020 203a 7061 7261 6d20  ent..    :param 
-0000f890: 746f 6b65 6e3a 2042 6f74 2773 2074 6f6b  token: Bot's tok
-0000f8a0: 656e 2028 796f 7520 646f 6e27 7420 6e65  en (you don't ne
-0000f8b0: 6564 2074 6f20 6669 6c6c 2074 6869 7329  ed to fill this)
-0000f8c0: 0a20 2020 203a 7061 7261 6d20 7072 655f  .    :param pre_
-0000f8d0: 6368 6563 6b6f 7574 5f71 7565 7279 5f69  checkout_query_i
-0000f8e0: 643a 2055 6e69 7175 6520 6964 656e 7469  d: Unique identi
-0000f8f0: 6669 6572 2066 6f72 2074 6865 2071 7565  fier for the que
-0000f900: 7279 2074 6f20 6265 2061 6e73 7765 7265  ry to be answere
-0000f910: 640a 2020 2020 3a70 6172 616d 206f 6b3a  d.    :param ok:
-0000f920: 2053 7065 6369 6679 2054 7275 6520 6966   Specify True if
-0000f930: 2065 7665 7279 7468 696e 6720 6973 2061   everything is a
-0000f940: 6c72 6967 6874 2028 676f 6f64 7320 6172  lright (goods ar
-0000f950: 6520 6176 6169 6c61 626c 652c 2065 7463  e available, etc
-0000f960: 2e29 2061 6e64 2074 6865 2062 6f74 2069  .) and the bot i
-0000f970: 7320 7265 6164 7920 746f 2070 726f 6365  s ready to proce
-0000f980: 6564 2077 6974 6820 7468 6520 6f72 6465  ed with the orde
-0000f990: 722e 2055 7365 2046 616c 7365 2069 6620  r. Use False if 
-0000f9a0: 7468 6572 6520 6172 6520 616e 7920 7072  there are any pr
-0000f9b0: 6f62 6c65 6d73 2e0a 2020 2020 3a70 6172  oblems..    :par
-0000f9c0: 616d 2065 7272 6f72 5f6d 6573 7361 6765  am error_message
-0000f9d0: 3a20 5265 7175 6972 6564 2069 6620 6f6b  : Required if ok
-0000f9e0: 2069 7320 4661 6c73 652e 2045 7272 6f72   is False. Error
-0000f9f0: 206d 6573 7361 6765 2069 6e20 6875 6d61   message in huma
-0000fa00: 6e20 7265 6164 6162 6c65 2066 6f72 6d20  n readable form 
-0000fa10: 7468 6174 2065 7870 6c61 696e 7320 7468  that explains th
-0000fa20: 6520 7265 6173 6f6e 2066 6f72 2066 6169  e reason for fai
-0000fa30: 6c75 7265 2074 6f20 7072 6f63 6565 6420  lure to proceed 
-0000fa40: 7769 7468 2074 6865 2063 6865 636b 6f75  with the checkou
-0000fa50: 7420 2865 2e67 2e20 2253 6f72 7279 2c20  t (e.g. "Sorry, 
-0000fa60: 736f 6d65 626f 6479 206a 7573 7420 626f  somebody just bo
-0000fa70: 7567 6874 2074 6865 206c 6173 7420 6f66  ught the last of
-0000fa80: 206f 7572 2061 6d61 7a69 6e67 2062 6c61   our amazing bla
-0000fa90: 636b 2054 2d73 6869 7274 7320 7768 696c  ck T-shirts whil
-0000faa0: 6520 796f 7520 7765 7265 2062 7573 7920  e you were busy 
-0000fab0: 6669 6c6c 696e 6720 6f75 7420 796f 7572  filling out your
-0000fac0: 2070 6179 6d65 6e74 2064 6574 6169 6c73   payment details
-0000fad0: 2e20 506c 6561 7365 2063 686f 6f73 6520  . Please choose 
-0000fae0: 6120 6469 6666 6572 656e 7420 636f 6c6f  a different colo
-0000faf0: 7220 6f72 2067 6172 6d65 6e74 2122 292e  r or garment!").
-0000fb00: 2054 656c 6567 7261 6d20 7769 6c6c 2064   Telegram will d
-0000fb10: 6973 706c 6179 2074 6869 7320 6d65 7373  isplay this mess
-0000fb20: 6167 6520 746f 2074 6865 2075 7365 722e  age to the user.
-0000fb30: 0a20 2020 203a 7265 7475 726e 3a0a 2020  .    :return:.  
-0000fb40: 2020 2222 220a 2020 2020 6d65 7468 6f64    """.    method
-0000fb50: 5f75 726c 203d 2022 616e 7377 6572 5072  _url = "answerPr
-0000fb60: 6543 6865 636b 6f75 7451 7565 7279 220a  eCheckoutQuery".
-0000fb70: 2020 2020 7061 796c 6f61 6420 3d20 7b22      payload = {"
-0000fb80: 7072 655f 6368 6563 6b6f 7574 5f71 7565  pre_checkout_que
-0000fb90: 7279 5f69 6422 3a20 7072 655f 6368 6563  ry_id": pre_chec
-0000fba0: 6b6f 7574 5f71 7565 7279 5f69 642c 2022  kout_query_id, "
-0000fbb0: 6f6b 223a 206f 6b7d 0a20 2020 2069 6620  ok": ok}.    if 
-0000fbc0: 6572 726f 725f 6d65 7373 6167 653a 0a20  error_message:. 
-0000fbd0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-0000fbe0: 6572 726f 725f 6d65 7373 6167 6522 5d20  error_message"] 
-0000fbf0: 3d20 6572 726f 725f 6d65 7373 6167 650a  = error_message.
-0000fc00: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-0000fc10: 205f 7265 7175 6573 7428 746f 6b65 6e2c   _request(token,
-0000fc20: 206d 6574 686f 645f 7572 6c2c 2070 6172   method_url, par
-0000fc30: 616d 733d 7061 796c 6f61 6429 0a0a 0a23  ams=payload)...#
-0000fc40: 2049 6e6c 696e 6551 7565 7279 0a0a 0a61   InlineQuery...a
-0000fc50: 7379 6e63 2064 6566 2061 6e73 7765 725f  sync def answer_
-0000fc60: 6361 6c6c 6261 636b 5f71 7565 7279 2874  callback_query(t
-0000fc70: 6f6b 656e 2c20 6361 6c6c 6261 636b 5f71  oken, callback_q
-0000fc80: 7565 7279 5f69 642c 2074 6578 743d 4e6f  uery_id, text=No
-0000fc90: 6e65 2c20 7368 6f77 5f61 6c65 7274 3d4e  ne, show_alert=N
-0000fca0: 6f6e 652c 2075 726c 3d4e 6f6e 652c 2063  one, url=None, c
-0000fcb0: 6163 6865 5f74 696d 653d 4e6f 6e65 293a  ache_time=None):
-0000fcc0: 0a20 2020 2022 2222 0a20 2020 2055 7365  .    """.    Use
-0000fcd0: 2074 6869 7320 6d65 7468 6f64 2074 6f20   this method to 
-0000fce0: 7365 6e64 2061 6e73 7765 7273 2074 6f20  send answers to 
-0000fcf0: 6361 6c6c 6261 636b 2071 7565 7269 6573  callback queries
-0000fd00: 2073 656e 7420 6672 6f6d 2069 6e6c 696e   sent from inlin
-0000fd10: 6520 6b65 7962 6f61 7264 732e 2054 6865  e keyboards. The
-0000fd20: 2061 6e73 7765 7220 7769 6c6c 2062 6520   answer will be 
-0000fd30: 6469 7370 6c61 7965 6420 746f 2074 6865  displayed to the
-0000fd40: 2075 7365 7220 6173 2061 206e 6f74 6966   user as a notif
-0000fd50: 6963 6174 696f 6e20 6174 2074 6865 2074  ication at the t
-0000fd60: 6f70 206f 6620 7468 6520 6368 6174 2073  op of the chat s
-0000fd70: 6372 6565 6e20 6f72 2061 7320 616e 2061  creen or as an a
-0000fd80: 6c65 7274 2e20 4f6e 2073 7563 6365 7373  lert. On success
-0000fd90: 2c20 5472 7565 2069 7320 7265 7475 726e  , True is return
-0000fda0: 6564 2e0a 2020 2020 416c 7465 726e 6174  ed..    Alternat
-0000fdb0: 6976 656c 792c 2074 6865 2075 7365 7220  ively, the user 
-0000fdc0: 6361 6e20 6265 2072 6564 6972 6563 7465  can be redirecte
-0000fdd0: 6420 746f 2074 6865 2073 7065 6369 6669  d to the specifi
-0000fde0: 6564 2047 616d 6520 5552 4c2e 2046 6f72  ed Game URL. For
-0000fdf0: 2074 6869 7320 6f70 7469 6f6e 2074 6f20   this option to 
-0000fe00: 776f 726b 2c20 796f 7520 6d75 7374 2066  work, you must f
-0000fe10: 6972 7374 2063 7265 6174 6520 6120 6761  irst create a ga
-0000fe20: 6d65 2066 6f72 2079 6f75 7220 626f 7420  me for your bot 
-0000fe30: 7669 6120 426f 7446 6174 6865 7220 616e  via BotFather an
-0000fe40: 6420 6163 6365 7074 2074 6865 2074 6572  d accept the ter
-0000fe50: 6d73 2e20 4f74 6865 7277 6973 652c 2079  ms. Otherwise, y
-0000fe60: 6f75 206d 6179 2075 7365 206c 696e 6b73  ou may use links
-0000fe70: 206c 696b 6520 7465 6c65 6772 616d 2e6d   like telegram.m
-0000fe80: 652f 796f 7572 5f62 6f74 3f73 7461 7274  e/your_bot?start
-0000fe90: 3d58 5858 5820 7468 6174 206f 7065 6e20  =XXXX that open 
-0000fea0: 796f 7572 2062 6f74 2077 6974 6820 6120  your bot with a 
-0000feb0: 7061 7261 6d65 7465 722e 0a20 2020 203a  parameter..    :
-0000fec0: 7061 7261 6d20 746f 6b65 6e3a 2042 6f74  param token: Bot
-0000fed0: 2773 2074 6f6b 656e 2028 796f 7520 646f  's token (you do
-0000fee0: 6e27 7420 6e65 6564 2074 6f20 6669 6c6c  n't need to fill
-0000fef0: 2074 6869 7329 0a20 2020 203a 7061 7261   this).    :para
-0000ff00: 6d20 6361 6c6c 6261 636b 5f71 7565 7279  m callback_query
-0000ff10: 5f69 643a 2055 6e69 7175 6520 6964 656e  _id: Unique iden
-0000ff20: 7469 6669 6572 2066 6f72 2074 6865 2071  tifier for the q
-0000ff30: 7565 7279 2074 6f20 6265 2061 6e73 7765  uery to be answe
-0000ff40: 7265 640a 2020 2020 3a70 6172 616d 2074  red.    :param t
-0000ff50: 6578 743a 2028 4f70 7469 6f6e 616c 2920  ext: (Optional) 
-0000ff60: 5465 7874 206f 6620 7468 6520 6e6f 7469  Text of the noti
-0000ff70: 6669 6361 7469 6f6e 2e20 4966 206e 6f74  fication. If not
-0000ff80: 2073 7065 6369 6669 6564 2c20 6e6f 7468   specified, noth
-0000ff90: 696e 6720 7769 6c6c 2062 6520 7368 6f77  ing will be show
-0000ffa0: 6e20 746f 2074 6865 2075 7365 722c 2030  n to the user, 0
-0000ffb0: 2d32 3030 2063 6861 7261 6374 6572 730a  -200 characters.
-0000ffc0: 2020 2020 3a70 6172 616d 2073 686f 775f      :param show_
-0000ffd0: 616c 6572 743a 2028 4f70 7469 6f6e 616c  alert: (Optional
-0000ffe0: 2920 4966 2074 7275 652c 2061 6e20 616c  ) If true, an al
-0000fff0: 6572 7420 7769 6c6c 2062 6520 7368 6f77  ert will be show
-00010000: 6e20 6279 2074 6865 2063 6c69 656e 7420  n by the client 
-00010010: 696e 7374 6561 6420 6f66 2061 206e 6f74  instead of a not
-00010020: 6966 6963 6174 696f 6e20 6174 2074 6865  ification at the
-00010030: 2074 6f70 206f 6620 7468 6520 6368 6174   top of the chat
-00010040: 2073 6372 6565 6e2e 2044 6566 6175 6c74   screen. Default
-00010050: 7320 746f 2066 616c 7365 2e0a 2020 2020  s to false..    
-00010060: 3a70 6172 616d 2075 726c 3a20 284f 7074  :param url: (Opt
-00010070: 696f 6e61 6c29 2055 524c 2074 6861 7420  ional) URL that 
-00010080: 7769 6c6c 2062 6520 6f70 656e 6564 2062  will be opened b
-00010090: 7920 7468 6520 7573 6572 2773 2063 6c69  y the user's cli
-000100a0: 656e 742e 2049 6620 796f 7520 6861 7665  ent. If you have
-000100b0: 2063 7265 6174 6564 2061 2047 616d 6520   created a Game 
-000100c0: 616e 6420 6163 6365 7074 6564 2074 6865  and accepted the
-000100d0: 2063 6f6e 6469 7469 6f6e 7320 7669 6120   conditions via 
-000100e0: 4042 6f74 6661 7468 6572 2c20 7370 6563  @Botfather, spec
-000100f0: 6966 7920 7468 6520 5552 4c20 7468 6174  ify the URL that
-00010100: 206f 7065 6e73 2079 6f75 7220 6761 6d65   opens your game
-00010110: 20e2 8093 206e 6f74 6520 7468 6174 2074   ... note that t
-00010120: 6869 7320 7769 6c6c 206f 6e6c 7920 776f  his will only wo
-00010130: 726b 2069 6620 7468 6520 7175 6572 7920  rk if the query 
-00010140: 636f 6d65 7320 6672 6f6d 2061 2063 616c  comes from a cal
-00010150: 6c62 6163 6b5f 6761 6d65 2062 7574 746f  lback_game butto
-00010160: 6e2e 0a20 2020 204f 7468 6572 7769 7365  n..    Otherwise
-00010170: 2c20 796f 7520 6d61 7920 7573 6520 6c69  , you may use li
-00010180: 6e6b 7320 6c69 6b65 2074 656c 6567 7261  nks like telegra
-00010190: 6d2e 6d65 2f79 6f75 725f 626f 743f 7374  m.me/your_bot?st
-000101a0: 6172 743d 5858 5858 2074 6861 7420 6f70  art=XXXX that op
-000101b0: 656e 2079 6f75 7220 626f 7420 7769 7468  en your bot with
-000101c0: 2061 2070 6172 616d 6574 6572 2e0a 2020   a parameter..  
-000101d0: 2020 3a70 6172 616d 2063 6163 6865 5f74    :param cache_t
-000101e0: 696d 653a 2028 4f70 7469 6f6e 616c 2920  ime: (Optional) 
-000101f0: 5468 6520 6d61 7869 6d75 6d20 616d 6f75  The maximum amou
-00010200: 6e74 206f 6620 7469 6d65 2069 6e20 7365  nt of time in se
-00010210: 636f 6e64 7320 7468 6174 2074 6865 2072  conds that the r
-00010220: 6573 756c 7420 6f66 2074 6865 2063 616c  esult of the cal
-00010230: 6c62 6163 6b20 7175 6572 7920 6d61 7920  lback query may 
-00010240: 6265 2063 6163 6865 6420 636c 6965 6e74  be cached client
-00010250: 2d73 6964 652e 2054 656c 6567 7261 6d20  -side. Telegram 
-00010260: 6170 7073 2077 696c 6c20 7375 7070 6f72  apps will suppor
-00010270: 7420 6361 6368 696e 6720 7374 6172 7469  t caching starti
-00010280: 6e67 2069 6e20 7665 7273 696f 6e20 332e  ng in version 3.
-00010290: 3134 2e20 4465 6661 756c 7473 2074 6f20  14. Defaults to 
-000102a0: 302e 0a20 2020 203a 7265 7475 726e 3a0a  0..    :return:.
-000102b0: 2020 2020 2222 220a 2020 2020 6d65 7468      """.    meth
-000102c0: 6f64 5f75 726c 203d 2022 616e 7377 6572  od_url = "answer
-000102d0: 4361 6c6c 6261 636b 5175 6572 7922 0a20  CallbackQuery". 
-000102e0: 2020 2070 6179 6c6f 6164 203d 207b 2263     payload = {"c
-000102f0: 616c 6c62 6163 6b5f 7175 6572 795f 6964  allback_query_id
-00010300: 223a 2063 616c 6c62 6163 6b5f 7175 6572  ": callback_quer
-00010310: 795f 6964 7d0a 2020 2020 6966 2074 6578  y_id}.    if tex
-00010320: 743a 0a20 2020 2020 2020 2070 6179 6c6f  t:.        paylo
-00010330: 6164 5b22 7465 7874 225d 203d 2074 6578  ad["text"] = tex
-00010340: 740a 2020 2020 6966 2073 686f 775f 616c  t.    if show_al
-00010350: 6572 7420 6973 206e 6f74 204e 6f6e 653a  ert is not None:
-00010360: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00010370: 5b22 7368 6f77 5f61 6c65 7274 225d 203d  ["show_alert"] =
-00010380: 2073 686f 775f 616c 6572 740a 2020 2020   show_alert.    
-00010390: 6966 2075 726c 3a0a 2020 2020 2020 2020  if url:.        
-000103a0: 7061 796c 6f61 645b 2275 726c 225d 203d  payload["url"] =
-000103b0: 2075 726c 0a20 2020 2069 6620 6361 6368   url.    if cach
-000103c0: 655f 7469 6d65 2069 7320 6e6f 7420 4e6f  e_time is not No
-000103d0: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
-000103e0: 6f61 645b 2263 6163 6865 5f74 696d 6522  oad["cache_time"
-000103f0: 5d20 3d20 6361 6368 655f 7469 6d65 0a20  ] = cache_time. 
-00010400: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00010410: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
-00010420: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
-00010430: 6d73 3d70 6179 6c6f 6164 2c20 6d65 7468  ms=payload, meth
-00010440: 6f64 3d22 706f 7374 2229 0a0a 0a61 7379  od="post")...asy
-00010450: 6e63 2064 6566 2061 6e73 7765 725f 696e  nc def answer_in
-00010460: 6c69 6e65 5f71 7565 7279 280a 2020 2020  line_query(.    
-00010470: 746f 6b65 6e2c 0a20 2020 2069 6e6c 696e  token,.    inlin
-00010480: 655f 7175 6572 795f 6964 2c0a 2020 2020  e_query_id,.    
-00010490: 7265 7375 6c74 732c 0a20 2020 2063 6163  results,.    cac
-000104a0: 6865 5f74 696d 653d 4e6f 6e65 2c0a 2020  he_time=None,.  
-000104b0: 2020 6973 5f70 6572 736f 6e61 6c3d 4e6f    is_personal=No
-000104c0: 6e65 2c0a 2020 2020 6e65 7874 5f6f 6666  ne,.    next_off
-000104d0: 7365 743d 4e6f 6e65 2c0a 2020 2020 7377  set=None,.    sw
-000104e0: 6974 6368 5f70 6d5f 7465 7874 3d4e 6f6e  itch_pm_text=Non
-000104f0: 652c 0a20 2020 2073 7769 7463 685f 706d  e,.    switch_pm
-00010500: 5f70 6172 616d 6574 6572 3d4e 6f6e 652c  _parameter=None,
-00010510: 0a29 3a0a 2020 2020 6d65 7468 6f64 5f75  .):.    method_u
-00010520: 726c 203d 2022 616e 7377 6572 496e 6c69  rl = "answerInli
-00010530: 6e65 5175 6572 7922 0a20 2020 2070 6179  neQuery".    pay
-00010540: 6c6f 6164 203d 207b 0a20 2020 2020 2020  load = {.       
-00010550: 2022 696e 6c69 6e65 5f71 7565 7279 5f69   "inline_query_i
-00010560: 6422 3a20 696e 6c69 6e65 5f71 7565 7279  d": inline_query
-00010570: 5f69 642c 0a20 2020 2020 2020 2022 7265  _id,.        "re
-00010580: 7375 6c74 7322 3a20 6177 6169 7420 5f63  sults": await _c
-00010590: 6f6e 7665 7274 5f6c 6973 745f 6a73 6f6e  onvert_list_json
-000105a0: 5f73 6572 6961 6c69 7a61 626c 6528 7265  _serializable(re
-000105b0: 7375 6c74 7329 2c0a 2020 2020 7d0a 2020  sults),.    }.  
-000105c0: 2020 6966 2063 6163 6865 5f74 696d 6520    if cache_time 
-000105d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000105e0: 2020 2020 2070 6179 6c6f 6164 5b22 6361       payload["ca
-000105f0: 6368 655f 7469 6d65 225d 203d 2063 6163  che_time"] = cac
-00010600: 6865 5f74 696d 650a 2020 2020 6966 2069  he_time.    if i
-00010610: 735f 7065 7273 6f6e 616c 2069 7320 6e6f  s_personal is no
-00010620: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00010630: 7061 796c 6f61 645b 2269 735f 7065 7273  payload["is_pers
-00010640: 6f6e 616c 225d 203d 2069 735f 7065 7273  onal"] = is_pers
-00010650: 6f6e 616c 0a20 2020 2069 6620 6e65 7874  onal.    if next
-00010660: 5f6f 6666 7365 7420 6973 206e 6f74 204e  _offset is not N
-00010670: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
-00010680: 6c6f 6164 5b22 6e65 7874 5f6f 6666 7365  load["next_offse
-00010690: 7422 5d20 3d20 6e65 7874 5f6f 6666 7365  t"] = next_offse
-000106a0: 740a 2020 2020 6966 2073 7769 7463 685f  t.    if switch_
-000106b0: 706d 5f74 6578 743a 0a20 2020 2020 2020  pm_text:.       
-000106c0: 2070 6179 6c6f 6164 5b22 7377 6974 6368   payload["switch
-000106d0: 5f70 6d5f 7465 7874 225d 203d 2073 7769  _pm_text"] = swi
-000106e0: 7463 685f 706d 5f74 6578 740a 2020 2020  tch_pm_text.    
-000106f0: 6966 2073 7769 7463 685f 706d 5f70 6172  if switch_pm_par
-00010700: 616d 6574 6572 3a0a 2020 2020 2020 2020  ameter:.        
-00010710: 7061 796c 6f61 645b 2273 7769 7463 685f  payload["switch_
-00010720: 706d 5f70 6172 616d 6574 6572 225d 203d  pm_parameter"] =
-00010730: 2073 7769 7463 685f 706d 5f70 6172 616d   switch_pm_param
-00010740: 6574 6572 0a20 2020 2072 6574 7572 6e20  eter.    return 
-00010750: 6177 6169 7420 5f72 6571 7565 7374 2874  await _request(t
-00010760: 6f6b 656e 2c20 6d65 7468 6f64 5f75 726c  oken, method_url
-00010770: 2c20 7061 7261 6d73 3d70 6179 6c6f 6164  , params=payload
-00010780: 2c20 6d65 7468 6f64 3d22 706f 7374 2229  , method="post")
-00010790: 0a0a 0a61 7379 6e63 2064 6566 2067 6574  ...async def get
-000107a0: 5f73 7469 636b 6572 5f73 6574 2874 6f6b  _sticker_set(tok
-000107b0: 656e 2c20 6e61 6d65 293a 0a20 2020 206d  en, name):.    m
-000107c0: 6574 686f 645f 7572 6c20 3d20 2267 6574  ethod_url = "get
-000107d0: 5374 6963 6b65 7253 6574 220a 2020 2020  StickerSet".    
-000107e0: 7265 7475 726e 2061 7761 6974 205f 7265  return await _re
-000107f0: 7175 6573 7428 746f 6b65 6e2c 206d 6574  quest(token, met
-00010800: 686f 645f 7572 6c2c 2070 6172 616d 733d  hod_url, params=
-00010810: 7b22 6e61 6d65 223a 206e 616d 657d 290a  {"name": name}).
-00010820: 0a0a 6173 796e 6320 6465 6620 7570 6c6f  ..async def uplo
-00010830: 6164 5f73 7469 636b 6572 5f66 696c 6528  ad_sticker_file(
-00010840: 746f 6b65 6e2c 2075 7365 725f 6964 2c20  token, user_id, 
-00010850: 706e 675f 7374 6963 6b65 7229 3a0a 2020  png_sticker):.  
-00010860: 2020 6d65 7468 6f64 5f75 726c 203d 2022    method_url = "
-00010870: 7570 6c6f 6164 5374 6963 6b65 7246 696c  uploadStickerFil
-00010880: 6522 0a20 2020 2070 6179 6c6f 6164 203d  e".    payload =
-00010890: 207b 2275 7365 725f 6964 223a 2075 7365   {"user_id": use
-000108a0: 725f 6964 7d0a 2020 2020 6669 6c65 7320  r_id}.    files 
-000108b0: 3d20 7b22 706e 675f 7374 6963 6b65 7222  = {"png_sticker"
-000108c0: 3a20 706e 675f 7374 6963 6b65 727d 0a20  : png_sticker}. 
-000108d0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-000108e0: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
-000108f0: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
-00010900: 6d73 3d70 6179 6c6f 6164 2c20 6669 6c65  ms=payload, file
-00010910: 733d 6669 6c65 732c 206d 6574 686f 643d  s=files, method=
-00010920: 2270 6f73 7422 290a 0a0a 6173 796e 6320  "post")...async 
-00010930: 6465 6620 6372 6561 7465 5f6e 6577 5f73  def create_new_s
-00010940: 7469 636b 6572 5f73 6574 280a 2020 2020  ticker_set(.    
-00010950: 746f 6b65 6e2c 0a20 2020 2075 7365 725f  token,.    user_
-00010960: 6964 2c0a 2020 2020 6e61 6d65 2c0a 2020  id,.    name,.  
-00010970: 2020 7469 746c 652c 0a20 2020 2065 6d6f    title,.    emo
-00010980: 6a69 732c 0a20 2020 2070 6e67 5f73 7469  jis,.    png_sti
-00010990: 636b 6572 2c0a 2020 2020 7467 735f 7374  cker,.    tgs_st
-000109a0: 6963 6b65 722c 0a20 2020 206d 6173 6b5f  icker,.    mask_
-000109b0: 706f 7369 7469 6f6e 3d4e 6f6e 652c 0a20  position=None,. 
-000109c0: 2020 2077 6562 6d5f 7374 6963 6b65 723d     webm_sticker=
-000109d0: 4e6f 6e65 2c0a 2020 2020 7374 6963 6b65  None,.    sticke
-000109e0: 725f 7479 7065 3d4e 6f6e 652c 0a29 3a0a  r_type=None,.):.
-000109f0: 2020 2020 726f 7574 6520 3d20 2263 7265      route = "cre
-00010a00: 6174 654e 6577 5374 6963 6b65 7253 6574  ateNewStickerSet
-00010a10: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
-00010a20: 7b22 7573 6572 5f69 6422 3a20 7573 6572  {"user_id": user
-00010a30: 5f69 642c 2022 6e61 6d65 223a 206e 616d  _id, "name": nam
-00010a40: 652c 2022 7469 746c 6522 3a20 7469 746c  e, "title": titl
-00010a50: 652c 2022 656d 6f6a 6973 223a 2065 6d6f  e, "emojis": emo
-00010a60: 6a69 737d 0a20 2020 2069 6620 706e 675f  jis}.    if png_
-00010a70: 7374 6963 6b65 723a 0a20 2020 2020 2020  sticker:.       
-00010a80: 2073 7479 7065 203d 2022 706e 675f 7374   stype = "png_st
-00010a90: 6963 6b65 7222 0a20 2020 2065 6c69 6620  icker".    elif 
-00010aa0: 7765 626d 5f73 7469 636b 6572 3a0a 2020  webm_sticker:.  
-00010ab0: 2020 2020 2020 7374 7970 6520 3d20 2277        stype = "w
-00010ac0: 6562 6d5f 7374 6963 6b65 7222 0a20 2020  ebm_sticker".   
-00010ad0: 2065 6c73 653a 0a20 2020 2020 2020 2073   else:.        s
-00010ae0: 7479 7065 203d 2022 7467 735f 7374 6963  type = "tgs_stic
-00010af0: 6b65 7222 0a20 2020 2073 7469 636b 6572  ker".    sticker
-00010b00: 203d 2070 6e67 5f73 7469 636b 6572 206f   = png_sticker o
-00010b10: 7220 7467 735f 7374 6963 6b65 7220 6f72  r tgs_sticker or
-00010b20: 2077 6562 6d5f 7374 6963 6b65 720a 2020   webm_sticker.  
-00010b30: 2020 6669 6c65 7320 3d20 4e6f 6e65 0a20    files = None. 
-00010b40: 2020 2069 6620 6e6f 7420 7574 696c 2e69     if not util.i
-00010b50: 735f 7374 7269 6e67 2873 7469 636b 6572  s_string(sticker
-00010b60: 293a 0a20 2020 2020 2020 2066 696c 6573  ):.        files
-00010b70: 203d 207b 7374 7970 653a 2073 7469 636b   = {stype: stick
-00010b80: 6572 7d0a 2020 2020 656c 7365 3a0a 2020  er}.    else:.  
-00010b90: 2020 2020 2020 7061 796c 6f61 645b 7374        payload[st
-00010ba0: 7970 655d 203d 2073 7469 636b 6572 0a20  ype] = sticker. 
-00010bb0: 2020 2069 6620 6d61 736b 5f70 6f73 6974     if mask_posit
-00010bc0: 696f 6e3a 0a20 2020 2020 2020 2070 6179  ion:.        pay
-00010bd0: 6c6f 6164 5b22 6d61 736b 5f70 6f73 6974  load["mask_posit
-00010be0: 696f 6e22 5d20 3d20 6d61 736b 5f70 6f73  ion"] = mask_pos
-00010bf0: 6974 696f 6e2e 746f 5f6a 736f 6e28 290a  ition.to_json().
-00010c00: 2020 2020 6966 2077 6562 6d5f 7374 6963      if webm_stic
-00010c10: 6b65 723a 0a20 2020 2020 2020 2070 6179  ker:.        pay
-00010c20: 6c6f 6164 5b22 7765 626d 5f73 7469 636b  load["webm_stick
-00010c30: 6572 225d 203d 2077 6562 6d5f 7374 6963  er"] = webm_stic
-00010c40: 6b65 720a 2020 2020 6966 2073 7469 636b  ker.    if stick
-00010c50: 6572 5f74 7970 653a 0a20 2020 2020 2020  er_type:.       
-00010c60: 2070 6179 6c6f 6164 5b22 7374 6963 6b65   payload["sticke
-00010c70: 725f 7479 7065 225d 203d 2073 7469 636b  r_type"] = stick
-00010c80: 6572 5f74 7970 650a 2020 2020 7265 7475  er_type.    retu
-00010c90: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
-00010ca0: 7428 746f 6b65 6e2c 2072 6f75 7465 2c20  t(token, route, 
-00010cb0: 7061 7261 6d73 3d70 6179 6c6f 6164 2c20  params=payload, 
-00010cc0: 6669 6c65 733d 6669 6c65 732c 206d 6574  files=files, met
-00010cd0: 686f 643d 2270 6f73 7422 290a 0a0a 6173  hod="post")...as
-00010ce0: 796e 6320 6465 6620 6164 645f 7374 6963  ync def add_stic
-00010cf0: 6b65 725f 746f 5f73 6574 2874 6f6b 656e  ker_to_set(token
-00010d00: 2c20 7573 6572 5f69 642c 206e 616d 652c  , user_id, name,
-00010d10: 2065 6d6f 6a69 732c 2070 6e67 5f73 7469   emojis, png_sti
-00010d20: 636b 6572 2c20 7467 735f 7374 6963 6b65  cker, tgs_sticke
-00010d30: 722c 206d 6173 6b5f 706f 7369 7469 6f6e  r, mask_position
-00010d40: 2c20 7765 626d 5f73 7469 636b 6572 293a  , webm_sticker):
-00010d50: 0a20 2020 206d 6574 686f 645f 7572 6c20  .    method_url 
-00010d60: 3d20 2261 6464 5374 6963 6b65 7254 6f53  = "addStickerToS
-00010d70: 6574 220a 2020 2020 7061 796c 6f61 6420  et".    payload 
-00010d80: 3d20 7b22 7573 6572 5f69 6422 3a20 7573  = {"user_id": us
-00010d90: 6572 5f69 642c 2022 6e61 6d65 223a 206e  er_id, "name": n
-00010da0: 616d 652c 2022 656d 6f6a 6973 223a 2065  ame, "emojis": e
-00010db0: 6d6f 6a69 737d 0a20 2020 2069 6620 706e  mojis}.    if pn
-00010dc0: 675f 7374 6963 6b65 723a 0a20 2020 2020  g_sticker:.     
-00010dd0: 2020 2073 7479 7065 203d 2022 706e 675f     stype = "png_
-00010de0: 7374 6963 6b65 7222 0a20 2020 2065 6c69  sticker".    eli
-00010df0: 6620 7765 626d 5f73 7469 636b 6572 3a0a  f webm_sticker:.
-00010e00: 2020 2020 2020 2020 7374 7970 6520 3d20          stype = 
-00010e10: 2277 6562 6d5f 7374 6963 6b65 7222 0a20  "webm_sticker". 
-00010e20: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00010e30: 2073 7479 7065 203d 2022 7467 735f 7374   stype = "tgs_st
-00010e40: 6963 6b65 7222 0a20 2020 2066 696c 6573  icker".    files
-00010e50: 203d 204e 6f6e 650a 2020 2020 7374 6963   = None.    stic
-00010e60: 6b65 7220 3d20 706e 675f 7374 6963 6b65  ker = png_sticke
-00010e70: 7220 6f72 2074 6773 5f73 7469 636b 6572  r or tgs_sticker
-00010e80: 206f 7220 7765 626d 5f73 7469 636b 6572   or webm_sticker
-00010e90: 0a0a 2020 2020 6966 206e 6f74 2075 7469  ..    if not uti
-00010ea0: 6c2e 6973 5f73 7472 696e 6728 7374 6963  l.is_string(stic
-00010eb0: 6b65 7229 3a0a 2020 2020 2020 2020 6669  ker):.        fi
-00010ec0: 6c65 7320 3d20 7b73 7479 7065 3a20 7374  les = {stype: st
-00010ed0: 6963 6b65 727d 0a20 2020 2065 6c73 653a  icker}.    else:
-00010ee0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00010ef0: 5b73 7479 7065 5d20 3d20 7374 6963 6b65  [stype] = sticke
-00010f00: 720a 2020 2020 6966 206d 6173 6b5f 706f  r.    if mask_po
-00010f10: 7369 7469 6f6e 3a0a 2020 2020 2020 2020  sition:.        
-00010f20: 7061 796c 6f61 645b 226d 6173 6b5f 706f  payload["mask_po
-00010f30: 7369 7469 6f6e 225d 203d 206d 6173 6b5f  sition"] = mask_
-00010f40: 706f 7369 7469 6f6e 2e74 6f5f 6a73 6f6e  position.to_json
-00010f50: 2829 0a0a 2020 2020 6966 2077 6562 6d5f  ()..    if webm_
-00010f60: 7374 6963 6b65 723a 0a20 2020 2020 2020  sticker:.       
-00010f70: 2070 6179 6c6f 6164 5b22 7765 626d 5f73   payload["webm_s
-00010f80: 7469 636b 6572 225d 203d 2077 6562 6d5f  ticker"] = webm_
-00010f90: 7374 6963 6b65 720a 2020 2020 7265 7475  sticker.    retu
-00010fa0: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
-00010fb0: 7428 746f 6b65 6e2c 206d 6574 686f 645f  t(token, method_
-00010fc0: 7572 6c2c 2070 6172 616d 733d 7061 796c  url, params=payl
-00010fd0: 6f61 642c 2066 696c 6573 3d66 696c 6573  oad, files=files
-00010fe0: 2c20 6d65 7468 6f64 3d22 706f 7374 2229  , method="post")
-00010ff0: 0a0a 0a61 7379 6e63 2064 6566 2073 6574  ...async def set
-00011000: 5f73 7469 636b 6572 5f70 6f73 6974 696f  _sticker_positio
-00011010: 6e5f 696e 5f73 6574 2874 6f6b 656e 2c20  n_in_set(token, 
-00011020: 7374 6963 6b65 722c 2070 6f73 6974 696f  sticker, positio
-00011030: 6e29 3a0a 2020 2020 6d65 7468 6f64 5f75  n):.    method_u
-00011040: 726c 203d 2022 7365 7453 7469 636b 6572  rl = "setSticker
-00011050: 506f 7369 7469 6f6e 496e 5365 7422 0a20  PositionInSet". 
-00011060: 2020 2070 6179 6c6f 6164 203d 207b 2273     payload = {"s
-00011070: 7469 636b 6572 223a 2073 7469 636b 6572  ticker": sticker
-00011080: 2c20 2270 6f73 6974 696f 6e22 3a20 706f  , "position": po
-00011090: 7369 7469 6f6e 7d0a 2020 2020 7265 7475  sition}.    retu
-000110a0: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
-000110b0: 7428 746f 6b65 6e2c 206d 6574 686f 645f  t(token, method_
-000110c0: 7572 6c2c 2070 6172 616d 733d 7061 796c  url, params=payl
-000110d0: 6f61 642c 206d 6574 686f 643d 2270 6f73  oad, method="pos
-000110e0: 7422 290a 0a0a 6173 796e 6320 6465 6620  t")...async def 
-000110f0: 6465 6c65 7465 5f73 7469 636b 6572 5f66  delete_sticker_f
-00011100: 726f 6d5f 7365 7428 746f 6b65 6e2c 2073  rom_set(token, s
-00011110: 7469 636b 6572 293a 0a20 2020 206d 6574  ticker):.    met
-00011120: 686f 645f 7572 6c20 3d20 2264 656c 6574  hod_url = "delet
-00011130: 6553 7469 636b 6572 4672 6f6d 5365 7422  eStickerFromSet"
-00011140: 0a20 2020 2070 6179 6c6f 6164 203d 207b  .    payload = {
-00011150: 2273 7469 636b 6572 223a 2073 7469 636b  "sticker": stick
-00011160: 6572 7d0a 2020 2020 7265 7475 726e 2061  er}.    return a
-00011170: 7761 6974 205f 7265 7175 6573 7428 746f  wait _request(to
-00011180: 6b65 6e2c 206d 6574 686f 645f 7572 6c2c  ken, method_url,
-00011190: 2070 6172 616d 733d 7061 796c 6f61 642c   params=payload,
-000111a0: 206d 6574 686f 643d 2270 6f73 7422 290a   method="post").
-000111b0: 0a0a 6173 796e 6320 6465 6620 6372 6561  ..async def crea
-000111c0: 7465 5f69 6e76 6f69 6365 5f6c 696e 6b28  te_invoice_link(
-000111d0: 0a20 2020 2074 6f6b 656e 2c0a 2020 2020  .    token,.    
-000111e0: 7469 746c 652c 0a20 2020 2064 6573 6372  title,.    descr
-000111f0: 6970 7469 6f6e 2c0a 2020 2020 7061 796c  iption,.    payl
-00011200: 6f61 642c 0a20 2020 2070 726f 7669 6465  oad,.    provide
-00011210: 725f 746f 6b65 6e2c 0a20 2020 2063 7572  r_token,.    cur
-00011220: 7265 6e63 792c 0a20 2020 2070 7269 6365  rency,.    price
-00011230: 732c 0a20 2020 206d 6178 5f74 6970 5f61  s,.    max_tip_a
-00011240: 6d6f 756e 743d 4e6f 6e65 2c0a 2020 2020  mount=None,.    
-00011250: 7375 6767 6573 7465 645f 7469 705f 616d  suggested_tip_am
-00011260: 6f75 6e74 733d 4e6f 6e65 2c0a 2020 2020  ounts=None,.    
-00011270: 7072 6f76 6964 6572 5f64 6174 613d 4e6f  provider_data=No
-00011280: 6e65 2c0a 2020 2020 7068 6f74 6f5f 7572  ne,.    photo_ur
-00011290: 6c3d 4e6f 6e65 2c0a 2020 2020 7068 6f74  l=None,.    phot
-000112a0: 6f5f 7369 7a65 3d4e 6f6e 652c 0a20 2020  o_size=None,.   
-000112b0: 2070 686f 746f 5f77 6964 7468 3d4e 6f6e   photo_width=Non
-000112c0: 652c 0a20 2020 2070 686f 746f 5f68 6569  e,.    photo_hei
-000112d0: 6768 743d 4e6f 6e65 2c0a 2020 2020 6e65  ght=None,.    ne
-000112e0: 6564 5f6e 616d 653d 4e6f 6e65 2c0a 2020  ed_name=None,.  
-000112f0: 2020 6e65 6564 5f70 686f 6e65 5f6e 756d    need_phone_num
-00011300: 6265 723d 4e6f 6e65 2c0a 2020 2020 6e65  ber=None,.    ne
-00011310: 6564 5f65 6d61 696c 3d4e 6f6e 652c 0a20  ed_email=None,. 
-00011320: 2020 206e 6565 645f 7368 6970 7069 6e67     need_shipping
-00011330: 5f61 6464 7265 7373 3d4e 6f6e 652c 0a20  _address=None,. 
-00011340: 2020 2073 656e 645f 7068 6f6e 655f 6e75     send_phone_nu
-00011350: 6d62 6572 5f74 6f5f 7072 6f76 6964 6572  mber_to_provider
-00011360: 3d4e 6f6e 652c 0a20 2020 2073 656e 645f  =None,.    send_
-00011370: 656d 6169 6c5f 746f 5f70 726f 7669 6465  email_to_provide
-00011380: 723d 4e6f 6e65 2c0a 2020 2020 6973 5f66  r=None,.    is_f
-00011390: 6c65 7869 626c 653d 4e6f 6e65 2c0a 293a  lexible=None,.):
-000113a0: 0a20 2020 2072 6f75 7465 203d 2072 2263  .    route = r"c
-000113b0: 7265 6174 6549 6e76 6f69 6365 4c69 6e6b  reateInvoiceLink
-000113c0: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
-000113d0: 7b0a 2020 2020 2020 2020 2274 6974 6c65  {.        "title
-000113e0: 223a 2074 6974 6c65 2c0a 2020 2020 2020  ": title,.      
-000113f0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00011400: 2064 6573 6372 6970 7469 6f6e 2c0a 2020   description,.  
-00011410: 2020 2020 2020 2270 6179 6c6f 6164 223a        "payload":
-00011420: 2070 6179 6c6f 6164 2c0a 2020 2020 2020   payload,.      
-00011430: 2020 2270 726f 7669 6465 725f 746f 6b65    "provider_toke
-00011440: 6e22 3a20 7072 6f76 6964 6572 5f74 6f6b  n": provider_tok
-00011450: 656e 2c0a 2020 2020 2020 2020 2263 7572  en,.        "cur
-00011460: 7265 6e63 7922 3a20 6375 7272 656e 6379  rency": currency
-00011470: 2c0a 2020 2020 2020 2020 2270 7269 6365  ,.        "price
-00011480: 7322 3a20 6177 6169 7420 5f63 6f6e 7665  s": await _conve
-00011490: 7274 5f6c 6973 745f 6a73 6f6e 5f73 6572  rt_list_json_ser
-000114a0: 6961 6c69 7a61 626c 6528 7072 6963 6573  ializable(prices
-000114b0: 292c 0a20 2020 207d 0a20 2020 2069 6620  ),.    }.    if 
-000114c0: 6d61 785f 7469 705f 616d 6f75 6e74 3a0a  max_tip_amount:.
-000114d0: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-000114e0: 226d 6178 5f74 6970 5f61 6d6f 756e 7422  "max_tip_amount"
-000114f0: 5d20 3d20 6d61 785f 7469 705f 616d 6f75  ] = max_tip_amou
-00011500: 6e74 0a20 2020 2069 6620 7375 6767 6573  nt.    if sugges
-00011510: 7465 645f 7469 705f 616d 6f75 6e74 733a  ted_tip_amounts:
-00011520: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00011530: 5b22 7375 6767 6573 7465 645f 7469 705f  ["suggested_tip_
-00011540: 616d 6f75 6e74 7322 5d20 3d20 6a73 6f6e  amounts"] = json
-00011550: 2e64 756d 7073 2873 7567 6765 7374 6564  .dumps(suggested
-00011560: 5f74 6970 5f61 6d6f 756e 7473 290a 2020  _tip_amounts).  
-00011570: 2020 6966 2070 726f 7669 6465 725f 6461    if provider_da
-00011580: 7461 3a0a 2020 2020 2020 2020 7061 796c  ta:.        payl
-00011590: 6f61 645b 2270 726f 7669 6465 725f 6461  oad["provider_da
-000115a0: 7461 225d 203d 2070 726f 7669 6465 725f  ta"] = provider_
-000115b0: 6461 7461 0a20 2020 2069 6620 7068 6f74  data.    if phot
-000115c0: 6f5f 7572 6c3a 0a20 2020 2020 2020 2070  o_url:.        p
-000115d0: 6179 6c6f 6164 5b22 7068 6f74 6f5f 7572  ayload["photo_ur
-000115e0: 6c22 5d20 3d20 7068 6f74 6f5f 7572 6c0a  l"] = photo_url.
-000115f0: 2020 2020 6966 2070 686f 746f 5f73 697a      if photo_siz
-00011600: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-00011610: 6164 5b22 7068 6f74 6f5f 7369 7a65 225d  ad["photo_size"]
-00011620: 203d 2070 686f 746f 5f73 697a 650a 2020   = photo_size.  
-00011630: 2020 6966 2070 686f 746f 5f77 6964 7468    if photo_width
-00011640: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-00011650: 645b 2270 686f 746f 5f77 6964 7468 225d  d["photo_width"]
-00011660: 203d 2070 686f 746f 5f77 6964 7468 0a20   = photo_width. 
-00011670: 2020 2069 6620 7068 6f74 6f5f 6865 6967     if photo_heig
-00011680: 6874 3a0a 2020 2020 2020 2020 7061 796c  ht:.        payl
-00011690: 6f61 645b 2270 686f 746f 5f68 6569 6768  oad["photo_heigh
-000116a0: 7422 5d20 3d20 7068 6f74 6f5f 6865 6967  t"] = photo_heig
-000116b0: 6874 0a20 2020 2069 6620 6e65 6564 5f6e  ht.    if need_n
-000116c0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-000116d0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-000116e0: 5b22 6e65 6564 5f6e 616d 6522 5d20 3d20  ["need_name"] = 
-000116f0: 6e65 6564 5f6e 616d 650a 2020 2020 6966  need_name.    if
-00011700: 206e 6565 645f 7068 6f6e 655f 6e75 6d62   need_phone_numb
-00011710: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-00011720: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-00011730: 226e 6565 645f 7068 6f6e 655f 6e75 6d62  "need_phone_numb
-00011740: 6572 225d 203d 206e 6565 645f 7068 6f6e  er"] = need_phon
-00011750: 655f 6e75 6d62 6572 0a20 2020 2069 6620  e_number.    if 
-00011760: 6e65 6564 5f65 6d61 696c 2069 7320 6e6f  need_email is no
-00011770: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00011780: 7061 796c 6f61 645b 226e 6565 645f 656d  payload["need_em
-00011790: 6169 6c22 5d20 3d20 6e65 6564 5f65 6d61  ail"] = need_ema
-000117a0: 696c 0a20 2020 2069 6620 6e65 6564 5f73  il.    if need_s
-000117b0: 6869 7070 696e 675f 6164 6472 6573 7320  hipping_address 
-000117c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000117d0: 2020 2020 2070 6179 6c6f 6164 5b22 6e65       payload["ne
-000117e0: 6564 5f73 6869 7070 696e 675f 6164 6472  ed_shipping_addr
-000117f0: 6573 7322 5d20 3d20 6e65 6564 5f73 6869  ess"] = need_shi
-00011800: 7070 696e 675f 6164 6472 6573 730a 2020  pping_address.  
-00011810: 2020 6966 2073 656e 645f 7068 6f6e 655f    if send_phone_
-00011820: 6e75 6d62 6572 5f74 6f5f 7072 6f76 6964  number_to_provid
-00011830: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-00011840: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-00011850: 2273 656e 645f 7068 6f6e 655f 6e75 6d62  "send_phone_numb
-00011860: 6572 5f74 6f5f 7072 6f76 6964 6572 225d  er_to_provider"]
-00011870: 203d 2073 656e 645f 7068 6f6e 655f 6e75   = send_phone_nu
-00011880: 6d62 6572 5f74 6f5f 7072 6f76 6964 6572  mber_to_provider
-00011890: 0a20 2020 2069 6620 7365 6e64 5f65 6d61  .    if send_ema
-000118a0: 696c 5f74 6f5f 7072 6f76 6964 6572 2069  il_to_provider i
-000118b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000118c0: 2020 2020 7061 796c 6f61 645b 2273 656e      payload["sen
-000118d0: 645f 656d 6169 6c5f 746f 5f70 726f 7669  d_email_to_provi
-000118e0: 6465 7222 5d20 3d20 7365 6e64 5f65 6d61  der"] = send_ema
-000118f0: 696c 5f74 6f5f 7072 6f76 6964 6572 0a20  il_to_provider. 
-00011900: 2020 2069 6620 6973 5f66 6c65 7869 626c     if is_flexibl
-00011910: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00011920: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
-00011930: 6973 5f66 6c65 7869 626c 6522 5d20 3d20  is_flexible"] = 
-00011940: 6973 5f66 6c65 7869 626c 650a 2020 2020  is_flexible.    
-00011950: 7265 7475 726e 2061 7761 6974 205f 7265  return await _re
-00011960: 7175 6573 7428 746f 6b65 6e2c 2072 6f75  quest(token, rou
-00011970: 7465 2c20 7061 7261 6d73 3d70 6179 6c6f  te, params=paylo
-00011980: 6164 2c20 6d65 7468 6f64 3d22 706f 7374  ad, method="post
-00011990: 2229 0a0a 0a23 206e 6f69 6e73 7065 6374  ")...# noinspect
-000119a0: 696f 6e20 5079 5368 6164 6f77 696e 6742  ion PyShadowingB
-000119b0: 7569 6c74 696e 730a 6173 796e 6320 6465  uiltins.async de
-000119c0: 6620 7365 6e64 5f70 6f6c 6c28 0a20 2020  f send_poll(.   
-000119d0: 2074 6f6b 656e 2c0a 2020 2020 6368 6174   token,.    chat
-000119e0: 5f69 642c 0a20 2020 2071 7565 7374 696f  _id,.    questio
-000119f0: 6e2c 0a20 2020 206f 7074 696f 6e73 2c0a  n,.    options,.
-00011a00: 2020 2020 6973 5f61 6e6f 6e79 6d6f 7573      is_anonymous
-00011a10: 3d4e 6f6e 652c 0a20 2020 2074 7970 653d  =None,.    type=
-00011a20: 4e6f 6e65 2c0a 2020 2020 616c 6c6f 7773  None,.    allows
-00011a30: 5f6d 756c 7469 706c 655f 616e 7377 6572  _multiple_answer
-00011a40: 733d 4e6f 6e65 2c0a 2020 2020 636f 7272  s=None,.    corr
-00011a50: 6563 745f 6f70 7469 6f6e 5f69 643d 4e6f  ect_option_id=No
-00011a60: 6e65 2c0a 2020 2020 6578 706c 616e 6174  ne,.    explanat
-00011a70: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 6578  ion=None,.    ex
-00011a80: 706c 616e 6174 696f 6e5f 7061 7273 655f  planation_parse_
-00011a90: 6d6f 6465 3d4e 6f6e 652c 0a20 2020 206f  mode=None,.    o
-00011aa0: 7065 6e5f 7065 7269 6f64 3d4e 6f6e 652c  pen_period=None,
-00011ab0: 0a20 2020 2063 6c6f 7365 5f64 6174 653d  .    close_date=
-00011ac0: 4e6f 6e65 2c0a 2020 2020 6973 5f63 6c6f  None,.    is_clo
-00011ad0: 7365 643d 4e6f 6e65 2c0a 2020 2020 6469  sed=None,.    di
-00011ae0: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
-00011af0: 6f6e 3d46 616c 7365 2c0a 2020 2020 7265  on=False,.    re
-00011b00: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00011b10: 643d 4e6f 6e65 2c0a 2020 2020 616c 6c6f  d=None,.    allo
-00011b20: 775f 7365 6e64 696e 675f 7769 7468 6f75  w_sending_withou
-00011b30: 745f 7265 706c 793d 4e6f 6e65 2c0a 2020  t_reply=None,.  
-00011b40: 2020 7265 706c 795f 6d61 726b 7570 3d4e    reply_markup=N
-00011b50: 6f6e 652c 0a20 2020 2074 696d 656f 7574  one,.    timeout
-00011b60: 3d4e 6f6e 652c 0a20 2020 2065 7870 6c61  =None,.    expla
-00011b70: 6e61 7469 6f6e 5f65 6e74 6974 6965 733d  nation_entities=
-00011b80: 4e6f 6e65 2c0a 2020 2020 7072 6f74 6563  None,.    protec
-00011b90: 745f 636f 6e74 656e 743d 4e6f 6e65 2c0a  t_content=None,.
-00011ba0: 2020 2020 6d65 7373 6167 655f 7468 7265      message_thre
-00011bb0: 6164 5f69 643a 204f 7074 696f 6e61 6c5b  ad_id: Optional[
-00011bc0: 696e 745d 203d 204e 6f6e 652c 0a29 3a0a  int] = None,.):.
-00011bd0: 2020 2020 6d65 7468 6f64 5f75 726c 203d      method_url =
-00011be0: 2072 2273 656e 6450 6f6c 6c22 0a20 2020   r"sendPoll".   
-00011bf0: 2070 6179 6c6f 6164 203d 207b 0a20 2020   payload = {.   
-00011c00: 2020 2020 2022 6368 6174 5f69 6422 3a20       "chat_id": 
-00011c10: 7374 7228 6368 6174 5f69 6429 2c0a 2020  str(chat_id),.  
-00011c20: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
-00011c30: 3a20 7175 6573 7469 6f6e 2c0a 2020 2020  : question,.    
-00011c40: 2020 2020 226f 7074 696f 6e73 223a 206a      "options": j
-00011c50: 736f 6e2e 6475 6d70 7328 6177 6169 7420  son.dumps(await 
-00011c60: 5f63 6f6e 7665 7274 5f70 6f6c 6c5f 6f70  _convert_poll_op
-00011c70: 7469 6f6e 7328 6f70 7469 6f6e 7329 292c  tions(options)),
-00011c80: 0a20 2020 207d 0a0a 2020 2020 6966 2069  .    }..    if i
-00011c90: 735f 616e 6f6e 796d 6f75 7320 6973 206e  s_anonymous is n
-00011ca0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00011cb0: 2070 6179 6c6f 6164 5b22 6973 5f61 6e6f   payload["is_ano
-00011cc0: 6e79 6d6f 7573 225d 203d 2069 735f 616e  nymous"] = is_an
-00011cd0: 6f6e 796d 6f75 730a 2020 2020 6966 2074  onymous.    if t
-00011ce0: 7970 6520 6973 206e 6f74 204e 6f6e 653a  ype is not None:
-00011cf0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00011d00: 5b22 7479 7065 225d 203d 2074 7970 650a  ["type"] = type.
-00011d10: 2020 2020 6966 2061 6c6c 6f77 735f 6d75      if allows_mu
-00011d20: 6c74 6970 6c65 5f61 6e73 7765 7273 2069  ltiple_answers i
-00011d30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00011d40: 2020 2020 7061 796c 6f61 645b 2261 6c6c      payload["all
-00011d50: 6f77 735f 6d75 6c74 6970 6c65 5f61 6e73  ows_multiple_ans
-00011d60: 7765 7273 225d 203d 2061 6c6c 6f77 735f  wers"] = allows_
-00011d70: 6d75 6c74 6970 6c65 5f61 6e73 7765 7273  multiple_answers
-00011d80: 0a20 2020 2069 6620 636f 7272 6563 745f  .    if correct_
-00011d90: 6f70 7469 6f6e 5f69 6420 6973 206e 6f74  option_id is not
-00011da0: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
-00011db0: 6179 6c6f 6164 5b22 636f 7272 6563 745f  ayload["correct_
-00011dc0: 6f70 7469 6f6e 5f69 6422 5d20 3d20 636f  option_id"] = co
-00011dd0: 7272 6563 745f 6f70 7469 6f6e 5f69 640a  rrect_option_id.
-00011de0: 2020 2020 6966 2065 7870 6c61 6e61 7469      if explanati
-00011df0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
-00011e00: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-00011e10: 2265 7870 6c61 6e61 7469 6f6e 225d 203d  "explanation"] =
-00011e20: 2065 7870 6c61 6e61 7469 6f6e 0a20 2020   explanation.   
-00011e30: 2069 6620 6578 706c 616e 6174 696f 6e5f   if explanation_
-00011e40: 7061 7273 655f 6d6f 6465 2069 7320 6e6f  parse_mode is no
-00011e50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00011e60: 7061 796c 6f61 645b 2265 7870 6c61 6e61  payload["explana
-00011e70: 7469 6f6e 5f70 6172 7365 5f6d 6f64 6522  tion_parse_mode"
-00011e80: 5d20 3d20 6578 706c 616e 6174 696f 6e5f  ] = explanation_
-00011e90: 7061 7273 655f 6d6f 6465 0a20 2020 2069  parse_mode.    i
-00011ea0: 6620 6f70 656e 5f70 6572 696f 6420 6973  f open_period is
-00011eb0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00011ec0: 2020 2070 6179 6c6f 6164 5b22 6f70 656e     payload["open
-00011ed0: 5f70 6572 696f 6422 5d20 3d20 6f70 656e  _period"] = open
-00011ee0: 5f70 6572 696f 640a 2020 2020 6966 2063  _period.    if c
-00011ef0: 6c6f 7365 5f64 6174 6520 6973 206e 6f74  lose_date is not
-00011f00: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
-00011f10: 6620 6973 696e 7374 616e 6365 2863 6c6f  f isinstance(clo
-00011f20: 7365 5f64 6174 652c 2064 6174 6574 696d  se_date, datetim
-00011f30: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00011f40: 7061 796c 6f61 645b 2263 6c6f 7365 5f64  payload["close_d
-00011f50: 6174 6522 5d20 3d20 636c 6f73 655f 6461  ate"] = close_da
-00011f60: 7465 2e74 696d 6573 7461 6d70 2829 0a20  te.timestamp(). 
-00011f70: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00011f80: 2020 2020 2020 2020 2070 6179 6c6f 6164           payload
-00011f90: 5b22 636c 6f73 655f 6461 7465 225d 203d  ["close_date"] =
-00011fa0: 2063 6c6f 7365 5f64 6174 650a 2020 2020   close_date.    
-00011fb0: 6966 2069 735f 636c 6f73 6564 2069 7320  if is_closed is 
-00011fc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00011fd0: 2020 7061 796c 6f61 645b 2269 735f 636c    payload["is_cl
-00011fe0: 6f73 6564 225d 203d 2069 735f 636c 6f73  osed"] = is_clos
-00011ff0: 6564 0a0a 2020 2020 6966 2064 6973 6162  ed..    if disab
-00012000: 6c65 5f6e 6f74 6966 6963 6174 696f 6e3a  le_notification:
-00012010: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00012020: 5b22 6469 7361 626c 655f 6e6f 7469 6669  ["disable_notifi
-00012030: 6361 7469 6f6e 225d 203d 2064 6973 6162  cation"] = disab
-00012040: 6c65 5f6e 6f74 6966 6963 6174 696f 6e0a  le_notification.
-00012050: 2020 2020 6966 2072 6570 6c79 5f74 6f5f      if reply_to_
-00012060: 6d65 7373 6167 655f 6964 2069 7320 6e6f  message_id is no
-00012070: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00012080: 7061 796c 6f61 645b 2272 6570 6c79 5f74  payload["reply_t
-00012090: 6f5f 6d65 7373 6167 655f 6964 225d 203d  o_message_id"] =
-000120a0: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
-000120b0: 655f 6964 0a20 2020 2069 6620 616c 6c6f  e_id.    if allo
-000120c0: 775f 7365 6e64 696e 675f 7769 7468 6f75  w_sending_withou
-000120d0: 745f 7265 706c 7920 6973 206e 6f74 204e  t_reply is not N
-000120e0: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
-000120f0: 6c6f 6164 5b22 616c 6c6f 775f 7365 6e64  load["allow_send
-00012100: 696e 675f 7769 7468 6f75 745f 7265 706c  ing_without_repl
-00012110: 7922 5d20 3d20 616c 6c6f 775f 7365 6e64  y"] = allow_send
-00012120: 696e 675f 7769 7468 6f75 745f 7265 706c  ing_without_repl
-00012130: 790a 2020 2020 6966 2072 6570 6c79 5f6d  y.    if reply_m
-00012140: 6172 6b75 7020 6973 206e 6f74 204e 6f6e  arkup is not Non
-00012150: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
-00012160: 6164 5b22 7265 706c 795f 6d61 726b 7570  ad["reply_markup
-00012170: 225d 203d 2061 7761 6974 205f 636f 6e76  "] = await _conv
-00012180: 6572 745f 6d61 726b 7570 2872 6570 6c79  ert_markup(reply
-00012190: 5f6d 6172 6b75 7029 0a20 2020 2069 6620  _markup).    if 
-000121a0: 7469 6d65 6f75 743a 0a20 2020 2020 2020  timeout:.       
-000121b0: 2070 6179 6c6f 6164 5b22 7469 6d65 6f75   payload["timeou
-000121c0: 7422 5d20 3d20 7469 6d65 6f75 740a 2020  t"] = timeout.  
-000121d0: 2020 6966 2065 7870 6c61 6e61 7469 6f6e    if explanation
-000121e0: 5f65 6e74 6974 6965 733a 0a20 2020 2020  _entities:.     
-000121f0: 2020 2070 6179 6c6f 6164 5b22 6578 706c     payload["expl
-00012200: 616e 6174 696f 6e5f 656e 7469 7469 6573  anation_entities
-00012210: 225d 203d 206a 736f 6e2e 6475 6d70 7328  "] = json.dumps(
-00012220: 7479 7065 732e 4d65 7373 6167 6545 6e74  types.MessageEnt
-00012230: 6974 792e 746f 5f6c 6973 745f 6f66 5f64  ity.to_list_of_d
-00012240: 6963 7473 2865 7870 6c61 6e61 7469 6f6e  icts(explanation
-00012250: 5f65 6e74 6974 6965 7329 290a 2020 2020  _entities)).    
-00012260: 6966 2070 726f 7465 6374 5f63 6f6e 7465  if protect_conte
-00012270: 6e74 3a0a 2020 2020 2020 2020 7061 796c  nt:.        payl
-00012280: 6f61 645b 2270 726f 7465 6374 5f63 6f6e  oad["protect_con
-00012290: 7465 6e74 225d 203d 2070 726f 7465 6374  tent"] = protect
-000122a0: 5f63 6f6e 7465 6e74 0a20 2020 205f 6164  _content.    _ad
-000122b0: 645f 6d65 7373 6167 655f 7468 7265 6164  d_message_thread
-000122c0: 5f69 6428 7061 796c 6f61 642c 206d 6573  _id(payload, mes
-000122d0: 7361 6765 5f74 6872 6561 645f 6964 290a  sage_thread_id).
-000122e0: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-000122f0: 205f 7265 7175 6573 7428 746f 6b65 6e2c   _request(token,
-00012300: 206d 6574 686f 645f 7572 6c2c 2070 6172   method_url, par
-00012310: 616d 733d 7061 796c 6f61 6429 0a0a 0a61  ams=payload)...a
-00012320: 7379 6e63 2064 6566 2063 7265 6174 655f  sync def create_
-00012330: 666f 7275 6d5f 746f 7069 6328 746f 6b65  forum_topic(toke
-00012340: 6e2c 2063 6861 745f 6964 2c20 6e61 6d65  n, chat_id, name
-00012350: 2c20 6963 6f6e 5f63 6f6c 6f72 3d4e 6f6e  , icon_color=Non
-00012360: 652c 2069 636f 6e5f 6375 7374 6f6d 5f65  e, icon_custom_e
-00012370: 6d6f 6a69 5f69 643d 4e6f 6e65 293a 0a20  moji_id=None):. 
-00012380: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
-00012390: 7222 6372 6561 7465 466f 7275 6d54 6f70  r"createForumTop
-000123a0: 6963 220a 2020 2020 7061 796c 6f61 6420  ic".    payload 
-000123b0: 3d20 7b22 6368 6174 5f69 6422 3a20 6368  = {"chat_id": ch
-000123c0: 6174 5f69 642c 2022 6e61 6d65 223a 206e  at_id, "name": n
-000123d0: 616d 657d 0a20 2020 2069 6620 6963 6f6e  ame}.    if icon
-000123e0: 5f63 6f6c 6f72 3a0a 2020 2020 2020 2020  _color:.        
-000123f0: 7061 796c 6f61 645b 2269 636f 6e5f 636f  payload["icon_co
-00012400: 6c6f 7222 5d20 3d20 6963 6f6e 5f63 6f6c  lor"] = icon_col
-00012410: 6f72 0a20 2020 2069 6620 6963 6f6e 5f63  or.    if icon_c
-00012420: 7573 746f 6d5f 656d 6f6a 695f 6964 3a0a  ustom_emoji_id:.
-00012430: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
-00012440: 2269 636f 6e5f 6375 7374 6f6d 5f65 6d6f  "icon_custom_emo
-00012450: 6a69 5f69 6422 5d20 3d20 6963 6f6e 5f63  ji_id"] = icon_c
-00012460: 7573 746f 6d5f 656d 6f6a 695f 6964 0a20  ustom_emoji_id. 
-00012470: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00012480: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
-00012490: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
-000124a0: 6d73 3d70 6179 6c6f 6164 290a 0a0a 6173  ms=payload)...as
-000124b0: 796e 6320 6465 6620 6564 6974 5f66 6f72  ync def edit_for
-000124c0: 756d 5f74 6f70 6963 2874 6f6b 656e 2c20  um_topic(token, 
-000124d0: 6368 6174 5f69 642c 206d 6573 7361 6765  chat_id, message
-000124e0: 5f74 6872 6561 645f 6964 2c20 6e61 6d65  _thread_id, name
-000124f0: 3d4e 6f6e 652c 2069 636f 6e5f 6375 7374  =None, icon_cust
-00012500: 6f6d 5f65 6d6f 6a69 5f69 643d 4e6f 6e65  om_emoji_id=None
-00012510: 293a 0a20 2020 206d 6574 686f 645f 7572  ):.    method_ur
-00012520: 6c20 3d20 7222 6564 6974 466f 7275 6d54  l = r"editForumT
-00012530: 6f70 6963 220a 2020 2020 7061 796c 6f61  opic".    payloa
-00012540: 6420 3d20 7b22 6368 6174 5f69 6422 3a20  d = {"chat_id": 
-00012550: 6368 6174 5f69 642c 2022 6d65 7373 6167  chat_id, "messag
-00012560: 655f 7468 7265 6164 5f69 6422 3a20 6d65  e_thread_id": me
-00012570: 7373 6167 655f 7468 7265 6164 5f69 647d  ssage_thread_id}
-00012580: 0a20 2020 2069 6620 6e61 6d65 2069 7320  .    if name is 
-00012590: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000125a0: 2020 7061 796c 6f61 645b 226e 616d 6522    payload["name"
-000125b0: 5d20 3d20 6e61 6d65 0a20 2020 2069 6620  ] = name.    if 
-000125c0: 6963 6f6e 5f63 7573 746f 6d5f 656d 6f6a  icon_custom_emoj
-000125d0: 695f 6964 2069 7320 6e6f 7420 4e6f 6e65  i_id is not None
-000125e0: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
-000125f0: 645b 2269 636f 6e5f 6375 7374 6f6d 5f65  d["icon_custom_e
-00012600: 6d6f 6a69 5f69 6422 5d20 3d20 6963 6f6e  moji_id"] = icon
-00012610: 5f63 7573 746f 6d5f 656d 6f6a 695f 6964  _custom_emoji_id
-00012620: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
-00012630: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
-00012640: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
-00012650: 7261 6d73 3d70 6179 6c6f 6164 290a 0a0a  rams=payload)...
-00012660: 6173 796e 6320 6465 6620 636c 6f73 655f  async def close_
-00012670: 666f 7275 6d5f 746f 7069 6328 746f 6b65  forum_topic(toke
-00012680: 6e2c 2063 6861 745f 6964 2c20 6d65 7373  n, chat_id, mess
-00012690: 6167 655f 7468 7265 6164 5f69 6429 3a0a  age_thread_id):.
-000126a0: 2020 2020 6d65 7468 6f64 5f75 726c 203d      method_url =
-000126b0: 2072 2263 6c6f 7365 466f 7275 6d54 6f70   r"closeForumTop
-000126c0: 6963 220a 2020 2020 7061 796c 6f61 6420  ic".    payload 
-000126d0: 3d20 7b22 6368 6174 5f69 6422 3a20 6368  = {"chat_id": ch
-000126e0: 6174 5f69 642c 2022 6d65 7373 6167 655f  at_id, "message_
-000126f0: 7468 7265 6164 5f69 6422 3a20 6d65 7373  thread_id": mess
-00012700: 6167 655f 7468 7265 6164 5f69 647d 0a20  age_thread_id}. 
-00012710: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00012720: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
-00012730: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
-00012740: 6d73 3d70 6179 6c6f 6164 290a 0a0a 6173  ms=payload)...as
-00012750: 796e 6320 6465 6620 7265 6f70 656e 5f66  ync def reopen_f
-00012760: 6f72 756d 5f74 6f70 6963 2874 6f6b 656e  orum_topic(token
-00012770: 2c20 6368 6174 5f69 642c 206d 6573 7361  , chat_id, messa
-00012780: 6765 5f74 6872 6561 645f 6964 293a 0a20  ge_thread_id):. 
-00012790: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
-000127a0: 7222 7265 6f70 656e 466f 7275 6d54 6f70  r"reopenForumTop
-000127b0: 6963 220a 2020 2020 7061 796c 6f61 6420  ic".    payload 
-000127c0: 3d20 7b22 6368 6174 5f69 6422 3a20 6368  = {"chat_id": ch
-000127d0: 6174 5f69 642c 2022 6d65 7373 6167 655f  at_id, "message_
-000127e0: 7468 7265 6164 5f69 6422 3a20 6d65 7373  thread_id": mess
-000127f0: 6167 655f 7468 7265 6164 5f69 647d 0a20  age_thread_id}. 
-00012800: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00012810: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
-00012820: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
-00012830: 6d73 3d70 6179 6c6f 6164 290a 0a0a 6173  ms=payload)...as
-00012840: 796e 6320 6465 6620 6465 6c65 7465 5f66  ync def delete_f
-00012850: 6f72 756d 5f74 6f70 6963 2874 6f6b 656e  orum_topic(token
-00012860: 2c20 6368 6174 5f69 642c 206d 6573 7361  , chat_id, messa
-00012870: 6765 5f74 6872 6561 645f 6964 293a 0a20  ge_thread_id):. 
-00012880: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
-00012890: 7222 6465 6c65 7465 466f 7275 6d54 6f70  r"deleteForumTop
-000128a0: 6963 220a 2020 2020 7061 796c 6f61 6420  ic".    payload 
-000128b0: 3d20 7b22 6368 6174 5f69 6422 3a20 6368  = {"chat_id": ch
-000128c0: 6174 5f69 642c 2022 6d65 7373 6167 655f  at_id, "message_
-000128d0: 7468 7265 6164 5f69 6422 3a20 6d65 7373  thread_id": mess
-000128e0: 6167 655f 7468 7265 6164 5f69 647d 0a20  age_thread_id}. 
-000128f0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00012900: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
-00012910: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
-00012920: 6d73 3d70 6179 6c6f 6164 290a 0a0a 6173  ms=payload)...as
-00012930: 796e 6320 6465 6620 756e 7069 6e5f 616c  ync def unpin_al
-00012940: 6c5f 666f 7275 6d5f 746f 7069 635f 6d65  l_forum_topic_me
-00012950: 7373 6167 6573 2874 6f6b 656e 2c20 6368  ssages(token, ch
-00012960: 6174 5f69 642c 206d 6573 7361 6765 5f74  at_id, message_t
-00012970: 6872 6561 645f 6964 293a 0a20 2020 206d  hread_id):.    m
-00012980: 6574 686f 645f 7572 6c20 3d20 7222 756e  ethod_url = r"un
-00012990: 7069 6e41 6c6c 466f 7275 6d54 6f70 6963  pinAllForumTopic
-000129a0: 4d65 7373 6167 6573 220a 2020 2020 7061  Messages".    pa
-000129b0: 796c 6f61 6420 3d20 7b22 6368 6174 5f69  yload = {"chat_i
-000129c0: 6422 3a20 6368 6174 5f69 642c 2022 6d65  d": chat_id, "me
-000129d0: 7373 6167 655f 7468 7265 6164 5f69 6422  ssage_thread_id"
-000129e0: 3a20 6d65 7373 6167 655f 7468 7265 6164  : message_thread
-000129f0: 5f69 647d 0a20 2020 2072 6574 7572 6e20  _id}.    return 
-00012a00: 6177 6169 7420 5f72 6571 7565 7374 2874  await _request(t
-00012a10: 6f6b 656e 2c20 6d65 7468 6f64 5f75 726c  oken, method_url
-00012a20: 2c20 7061 7261 6d73 3d70 6179 6c6f 6164  , params=payload
-00012a30: 290a 0a0a 6173 796e 6320 6465 6620 6765  )...async def ge
-00012a40: 745f 666f 7275 6d5f 746f 7069 635f 6963  t_forum_topic_ic
-00012a50: 6f6e 5f73 7469 636b 6572 7328 746f 6b65  on_stickers(toke
-00012a60: 6e29 3a0a 2020 2020 6d65 7468 6f64 5f75  n):.    method_u
-00012a70: 726c 203d 2072 2267 6574 466f 7275 6d54  rl = r"getForumT
-00012a80: 6f70 6963 4963 6f6e 5374 6963 6b65 7273  opicIconStickers
-00012a90: 220a 2020 2020 7265 7475 726e 2061 7761  ".    return awa
-00012aa0: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
-00012ab0: 6e2c 206d 6574 686f 645f 7572 6c29 0a0a  n, method_url)..
-00012ac0: 0a61 7379 6e63 2064 6566 2065 6469 745f  .async def edit_
-00012ad0: 6765 6e65 7261 6c5f 666f 7275 6d5f 746f  general_forum_to
-00012ae0: 7069 6328 746f 6b65 6e2c 2063 6861 745f  pic(token, chat_
-00012af0: 6964 2c20 6e61 6d65 293a 0a20 2020 206d  id, name):.    m
-00012b00: 6574 686f 645f 7572 6c20 3d20 7222 6564  ethod_url = r"ed
-00012b10: 6974 4765 6e65 7261 6c46 6f72 756d 546f  itGeneralForumTo
-00012b20: 7069 6322 0a20 2020 2070 6179 6c6f 6164  pic".    payload
-00012b30: 203d 207b 2263 6861 745f 6964 223a 2063   = {"chat_id": c
-00012b40: 6861 745f 6964 2c20 226e 616d 6522 3a20  hat_id, "name": 
-00012b50: 6e61 6d65 7d0a 2020 2020 7265 7475 726e  name}.    return
-00012b60: 2061 7761 6974 205f 7265 7175 6573 7428   await _request(
-00012b70: 746f 6b65 6e2c 206d 6574 686f 645f 7572  token, method_ur
-00012b80: 6c2c 2070 6172 616d 733d 7061 796c 6f61  l, params=payloa
-00012b90: 6429 0a0a 0a61 7379 6e63 2064 6566 2063  d)...async def c
-00012ba0: 6c6f 7365 5f67 656e 6572 616c 5f66 6f72  lose_general_for
-00012bb0: 756d 5f74 6f70 6963 2874 6f6b 656e 2c20  um_topic(token, 
-00012bc0: 6368 6174 5f69 6429 3a0a 2020 2020 6d65  chat_id):.    me
-00012bd0: 7468 6f64 5f75 726c 203d 2072 2263 6c6f  thod_url = r"clo
-00012be0: 7365 4765 6e65 7261 6c46 6f72 756d 546f  seGeneralForumTo
-00012bf0: 7069 6322 0a20 2020 2070 6179 6c6f 6164  pic".    payload
-00012c00: 203d 207b 2263 6861 745f 6964 223a 2063   = {"chat_id": c
-00012c10: 6861 745f 6964 7d0a 2020 2020 7265 7475  hat_id}.    retu
-00012c20: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
-00012c30: 7428 746f 6b65 6e2c 206d 6574 686f 645f  t(token, method_
-00012c40: 7572 6c2c 2070 6172 616d 733d 7061 796c  url, params=payl
-00012c50: 6f61 6429 0a0a 0a61 7379 6e63 2064 6566  oad)...async def
-00012c60: 2072 656f 7065 6e5f 6765 6e65 7261 6c5f   reopen_general_
-00012c70: 666f 7275 6d5f 746f 7069 6328 746f 6b65  forum_topic(toke
-00012c80: 6e2c 2063 6861 745f 6964 293a 0a20 2020  n, chat_id):.   
-00012c90: 206d 6574 686f 645f 7572 6c20 3d20 7222   method_url = r"
-00012ca0: 7265 6f70 656e 4765 6e65 7261 6c46 6f72  reopenGeneralFor
-00012cb0: 756d 546f 7069 6322 0a20 2020 2070 6179  umTopic".    pay
-00012cc0: 6c6f 6164 203d 207b 2263 6861 745f 6964  load = {"chat_id
-00012cd0: 223a 2063 6861 745f 6964 7d0a 2020 2020  ": chat_id}.    
-00012ce0: 7265 7475 726e 2061 7761 6974 205f 7265  return await _re
-00012cf0: 7175 6573 7428 746f 6b65 6e2c 206d 6574  quest(token, met
-00012d00: 686f 645f 7572 6c2c 2070 6172 616d 733d  hod_url, params=
-00012d10: 7061 796c 6f61 6429 0a0a 0a61 7379 6e63  payload)...async
-00012d20: 2064 6566 2068 6964 655f 6765 6e65 7261   def hide_genera
-00012d30: 6c5f 666f 7275 6d5f 746f 7069 6328 746f  l_forum_topic(to
-00012d40: 6b65 6e2c 2063 6861 745f 6964 293a 0a20  ken, chat_id):. 
-00012d50: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
-00012d60: 7222 6869 6465 4765 6e65 7261 6c46 6f72  r"hideGeneralFor
-00012d70: 756d 546f 7069 6322 0a20 2020 2070 6179  umTopic".    pay
-00012d80: 6c6f 6164 203d 207b 2263 6861 745f 6964  load = {"chat_id
-00012d90: 223a 2063 6861 745f 6964 7d0a 2020 2020  ": chat_id}.    
-00012da0: 7265 7475 726e 2061 7761 6974 205f 7265  return await _re
-00012db0: 7175 6573 7428 746f 6b65 6e2c 206d 6574  quest(token, met
-00012dc0: 686f 645f 7572 6c2c 2070 6172 616d 733d  hod_url, params=
-00012dd0: 7061 796c 6f61 6429 0a0a 0a61 7379 6e63  payload)...async
-00012de0: 2064 6566 2075 6e68 6964 655f 6765 6e65   def unhide_gene
-00012df0: 7261 6c5f 666f 7275 6d5f 746f 7069 6328  ral_forum_topic(
-00012e00: 746f 6b65 6e2c 2063 6861 745f 6964 293a  token, chat_id):
-00012e10: 0a20 2020 206d 6574 686f 645f 7572 6c20  .    method_url 
-00012e20: 3d20 7222 756e 6869 6465 4765 6e65 7261  = r"unhideGenera
-00012e30: 6c46 6f72 756d 546f 7069 6322 0a20 2020  lForumTopic".   
-00012e40: 2070 6179 6c6f 6164 203d 207b 2263 6861   payload = {"cha
-00012e50: 745f 6964 223a 2063 6861 745f 6964 7d0a  t_id": chat_id}.
-00012e60: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-00012e70: 205f 7265 7175 6573 7428 746f 6b65 6e2c   _request(token,
-00012e80: 206d 6574 686f 645f 7572 6c2c 2070 6172   method_url, par
-00012e90: 616d 733d 7061 796c 6f61 6429 0a0a 0a61  ams=payload)...a
-00012ea0: 7379 6e63 2064 6566 205f 636f 6e76 6572  sync def _conver
-00012eb0: 745f 6c69 7374 5f6a 736f 6e5f 7365 7269  t_list_json_seri
-00012ec0: 616c 697a 6162 6c65 2872 6573 756c 7473  alizable(results
-00012ed0: 293a 0a20 2020 2072 6574 203d 2022 220a  ):.    ret = "".
-00012ee0: 2020 2020 666f 7220 7220 696e 2072 6573      for r in res
-00012ef0: 756c 7473 3a0a 2020 2020 2020 2020 6966  ults:.        if
-00012f00: 2069 7369 6e73 7461 6e63 6528 722c 2074   isinstance(r, t
-00012f10: 7970 6573 2e4a 736f 6e53 6572 6961 6c69  ypes.JsonSeriali
-00012f20: 7a61 626c 6529 3a0a 2020 2020 2020 2020  zable):.        
-00012f30: 2020 2020 7265 7420 3d20 7265 7420 2b20      ret = ret + 
-00012f40: 722e 746f 5f6a 736f 6e28 2920 2b20 222c  r.to_json() + ",
-00012f50: 220a 2020 2020 6966 206c 656e 2872 6574  ".    if len(ret
-00012f60: 2920 3e20 303a 0a20 2020 2020 2020 2072  ) > 0:.        r
-00012f70: 6574 203d 2072 6574 5b3a 2d31 5d0a 2020  et = ret[:-1].  
-00012f80: 2020 7265 7475 726e 2022 5b22 202b 2072    return "[" + r
-00012f90: 6574 202b 2022 5d22 0a0a 0a61 7379 6e63  et + "]"...async
-00012fa0: 2064 6566 205f 636f 6e76 6572 745f 656e   def _convert_en
-00012fb0: 7469 7465 7328 656e 7469 7465 7329 3a0a  tites(entites):.
-00012fc0: 2020 2020 6966 2065 6e74 6974 6573 2069      if entites i
-00012fd0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00012fe0: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
-00012ff0: 656c 6966 206c 656e 2865 6e74 6974 6573  elif len(entites
-00013000: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
-00013010: 7265 7475 726e 205b 5d0a 2020 2020 656c  return [].    el
-00013020: 6966 2069 7369 6e73 7461 6e63 6528 656e  if isinstance(en
-00013030: 7469 7465 735b 305d 2c20 7479 7065 732e  tites[0], types.
-00013040: 4a73 6f6e 5365 7269 616c 697a 6162 6c65  JsonSerializable
-00013050: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00013060: 6e20 5b65 6e74 6974 792e 746f 5f6a 736f  n [entity.to_jso
-00013070: 6e28 2920 666f 7220 656e 7469 7479 2069  n() for entity i
-00013080: 6e20 656e 7469 7465 735d 0a20 2020 2065  n entites].    e
-00013090: 6c73 653a 0a20 2020 2020 2020 2072 6574  lse:.        ret
-000130a0: 7572 6e20 656e 7469 7465 730a 0a0a 6173  urn entites...as
-000130b0: 796e 6320 6465 6620 5f63 6f6e 7665 7274  ync def _convert
-000130c0: 5f70 6f6c 6c5f 6f70 7469 6f6e 7328 706f  _poll_options(po
-000130d0: 6c6c 5f6f 7074 696f 6e73 293a 0a20 2020  ll_options):.   
-000130e0: 2069 6620 706f 6c6c 5f6f 7074 696f 6e73   if poll_options
-000130f0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00013100: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
-00013110: 2020 656c 6966 206c 656e 2870 6f6c 6c5f    elif len(poll_
-00013120: 6f70 7469 6f6e 7329 203d 3d20 303a 0a20  options) == 0:. 
-00013130: 2020 2020 2020 2072 6574 7572 6e20 5b5d         return []
-00013140: 0a20 2020 2065 6c69 6620 6973 696e 7374  .    elif isinst
-00013150: 616e 6365 2870 6f6c 6c5f 6f70 7469 6f6e  ance(poll_option
-00013160: 735b 305d 2c20 7374 7229 3a0a 2020 2020  s[0], str):.    
-00013170: 2020 2020 2320 436f 6d70 6174 6962 696c      # Compatibil
-00013180: 6974 7920 6d6f 6465 2077 6974 6820 7072  ity mode with pr
-00013190: 6576 696f 7573 2062 7567 2077 6865 6e20  evious bug when 
-000131a0: 6f6e 6c79 206c 6973 7420 6f66 2073 7472  only list of str
-000131b0: 696e 6720 7761 7320 6163 6365 7074 6564  ing was accepted
-000131c0: 2061 7320 706f 6c6c 5f6f 7074 696f 6e73   as poll_options
-000131d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000131e0: 706f 6c6c 5f6f 7074 696f 6e73 0a20 2020  poll_options.   
-000131f0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-00013200: 2870 6f6c 6c5f 6f70 7469 6f6e 735b 305d  (poll_options[0]
-00013210: 2c20 7479 7065 732e 506f 6c6c 4f70 7469  , types.PollOpti
-00013220: 6f6e 293a 0a20 2020 2020 2020 2072 6574  on):.        ret
-00013230: 7572 6e20 5b6f 7074 696f 6e2e 7465 7874  urn [option.text
-00013240: 2066 6f72 206f 7074 696f 6e20 696e 2070   for option in p
-00013250: 6f6c 6c5f 6f70 7469 6f6e 735d 0a20 2020  oll_options].   
-00013260: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
-00013270: 6574 7572 6e20 706f 6c6c 5f6f 7074 696f  eturn poll_optio
-00013280: 6e73 0a0a 0a61 7379 6e63 2064 6566 2063  ns...async def c
-00013290: 6f6e 7665 7274 5f69 6e70 7574 5f6d 6564  onvert_input_med
-000132a0: 6961 286d 6564 6961 293a 0a20 2020 2069  ia(media):.    i
-000132b0: 6620 6973 696e 7374 616e 6365 286d 6564  f isinstance(med
-000132c0: 6961 2c20 7479 7065 732e 496e 7075 744d  ia, types.InputM
-000132d0: 6564 6961 293a 0a20 2020 2020 2020 2072  edia):.        r
-000132e0: 6574 7572 6e20 6d65 6469 612e 636f 6e76  eturn media.conv
-000132f0: 6572 745f 696e 7075 745f 6d65 6469 6128  ert_input_media(
-00013300: 290a 2020 2020 7265 7475 726e 204e 6f6e  ).    return Non
-00013310: 652c 204e 6f6e 650a 0a0a 6173 796e 6320  e, None...async 
-00013320: 6465 6620 636f 6e76 6572 745f 696e 7075  def convert_inpu
-00013330: 745f 6d65 6469 615f 6172 7261 7928 6172  t_media_array(ar
-00013340: 7261 7929 3a0a 2020 2020 6d65 6469 6120  ray):.    media 
-00013350: 3d20 5b5d 0a20 2020 2066 696c 6573 203d  = [].    files =
-00013360: 207b 7d0a 2020 2020 666f 7220 696e 7075   {}.    for inpu
-00013370: 745f 6d65 6469 6120 696e 2061 7272 6179  t_media in array
-00013380: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
-00013390: 6e73 7461 6e63 6528 696e 7075 745f 6d65  nstance(input_me
-000133a0: 6469 612c 2074 7970 6573 2e49 6e70 7574  dia, types.Input
-000133b0: 4d65 6469 6129 3a0a 2020 2020 2020 2020  Media):.        
-000133c0: 2020 2020 6d65 6469 615f 6469 6374 203d      media_dict =
-000133d0: 2069 6e70 7574 5f6d 6564 6961 2e74 6f5f   input_media.to_
-000133e0: 6469 6374 2829 0a20 2020 2020 2020 2020  dict().         
-000133f0: 2020 2069 6620 6d65 6469 615f 6469 6374     if media_dict
-00013400: 5b22 6d65 6469 6122 5d2e 7374 6172 7473  ["media"].starts
-00013410: 7769 7468 2822 6174 7461 6368 3a2f 2f22  with("attach://"
-00013420: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00013430: 2020 206b 6579 203d 206d 6564 6961 5f64     key = media_d
-00013440: 6963 745b 226d 6564 6961 225d 2e72 6570  ict["media"].rep
-00013450: 6c61 6365 2822 6174 7461 6368 3a2f 2f22  lace("attach://"
-00013460: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
-00013470: 2020 2020 2020 6669 6c65 735b 6b65 795d        files[key]
-00013480: 203d 2069 6e70 7574 5f6d 6564 6961 2e6d   = input_media.m
-00013490: 6564 6961 0a20 2020 2020 2020 2020 2020  edia.           
-000134a0: 206d 6564 6961 2e61 7070 656e 6428 6d65   media.append(me
-000134b0: 6469 615f 6469 6374 290a 2020 2020 7265  dia_dict).    re
-000134c0: 7475 726e 206a 736f 6e2e 6475 6d70 7328  turn json.dumps(
-000134d0: 6d65 6469 6129 2c20 6669 6c65 730a 0a0a  media), files...
-000134e0: 6173 796e 6320 6465 6620 5f6e 6f5f 656e  async def _no_en
-000134f0: 636f 6465 2866 756e 6329 3a0a 2020 2020  code(func):.    
-00013500: 6465 6620 7772 6170 7065 7228 6b65 792c  def wrapper(key,
-00013510: 2076 616c 293a 0a20 2020 2020 2020 2069   val):.        i
-00013520: 6620 6b65 7920 3d3d 2022 6669 6c65 6e61  f key == "filena
-00013530: 6d65 223a 0a20 2020 2020 2020 2020 2020  me":.           
-00013540: 2072 6574 7572 6e20 227b 307d 3d7b 317d   return "{0}={1}
-00013550: 222e 666f 726d 6174 286b 6579 2c20 7661  ".format(key, va
-00013560: 6c29 0a20 2020 2020 2020 2065 6c73 653a  l).        else:
-00013570: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00013580: 7572 6e20 6675 6e63 286b 6579 2c20 7661  urn func(key, va
-00013590: 6c29 0a0a 2020 2020 7265 7475 726e 2077  l)..    return w
-000135a0: 7261 7070 6572 0a0a 0a61 7379 6e63 2064  rapper...async d
-000135b0: 6566 2073 746f 705f 706f 6c6c 2874 6f6b  ef stop_poll(tok
-000135c0: 656e 2c20 6368 6174 5f69 642c 206d 6573  en, chat_id, mes
-000135d0: 7361 6765 5f69 642c 2072 6570 6c79 5f6d  sage_id, reply_m
-000135e0: 6172 6b75 703d 4e6f 6e65 293a 0a20 2020  arkup=None):.   
-000135f0: 206d 6574 686f 645f 7572 6c20 3d20 7222   method_url = r"
-00013600: 7374 6f70 506f 6c6c 220a 2020 2020 7061  stopPoll".    pa
-00013610: 796c 6f61 6420 3d20 7b22 6368 6174 5f69  yload = {"chat_i
-00013620: 6422 3a20 7374 7228 6368 6174 5f69 6429  d": str(chat_id)
-00013630: 2c20 226d 6573 7361 6765 5f69 6422 3a20  , "message_id": 
-00013640: 6d65 7373 6167 655f 6964 7d0a 2020 2020  message_id}.    
-00013650: 6966 2072 6570 6c79 5f6d 6172 6b75 703a  if reply_markup:
-00013660: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
-00013670: 5b22 7265 706c 795f 6d61 726b 7570 225d  ["reply_markup"]
-00013680: 203d 2061 7761 6974 205f 636f 6e76 6572   = await _conver
-00013690: 745f 6d61 726b 7570 2872 6570 6c79 5f6d  t_markup(reply_m
-000136a0: 6172 6b75 7029 0a20 2020 2072 6574 7572  arkup).    retur
-000136b0: 6e20 6177 6169 7420 5f72 6571 7565 7374  n await _request
-000136c0: 2874 6f6b 656e 2c20 6d65 7468 6f64 5f75  (token, method_u
-000136d0: 726c 2c20 7061 7261 6d73 3d70 6179 6c6f  rl, params=paylo
-000136e0: 6164 290a 0a0a 636c 6173 7320 4170 6945  ad)...class ApiE
-000136f0: 7863 6570 7469 6f6e 2845 7863 6570 7469  xception(Excepti
-00013700: 6f6e 293a 0a20 2020 2022 2222 0a20 2020  on):.    """.   
-00013710: 2054 6869 7320 636c 6173 7320 7265 7072   This class repr
-00013720: 6573 656e 7473 2061 2062 6173 6520 4578  esents a base Ex
-00013730: 6365 7074 696f 6e20 7468 726f 776e 2077  ception thrown w
-00013740: 6865 6e20 6120 6361 6c6c 2074 6f20 7468  hen a call to th
-00013750: 6520 5465 6c65 6772 616d 2041 5049 2066  e Telegram API f
-00013760: 6169 6c73 2e0a 2020 2020 4974 2063 6f6e  ails..    It con
-00013770: 7461 696e 7320 6169 6f68 7474 7020 636c  tains aiohttp cl
-00013780: 6965 6e74 2072 6573 706f 6e73 6520 696e  ient response in
-00013790: 2063 6173 6520 796f 7520 7761 6e74 2074   case you want t
-000137a0: 6f20 646f 2073 6f6d 6520 6164 7661 6e63  o do some advanc
-000137b0: 6564 2065 7272 6f72 2068 616e 646c 696e  ed error handlin
-000137c0: 672e 0a20 2020 2022 2222 0a0a 2020 2020  g..    """..    
-000137d0: 4150 495f 5552 4c5f 5245 4745 5820 3d20  API_URL_REGEX = 
-000137e0: 7265 2e63 6f6d 7069 6c65 2872 2261 7069  re.compile(r"api
-000137f0: 5c2e 7465 6c65 6772 616d 5c2e 6f72 672f  \.telegram\.org/
-00013800: 626f 7428 3f50 3c74 6f6b 656e 3e2e 2a3f  bot(?P<token>.*?
-00013810: 292f 2e2a 2229 0a0a 2020 2020 6465 6620  )/.*")..    def 
-00013820: 5f5f 696e 6974 5f5f 2873 656c 662c 206d  __init__(self, m
-00013830: 7367 3a20 7374 722c 2072 6573 706f 6e73  sg: str, respons
-00013840: 653a 2061 696f 6874 7470 2e43 6c69 656e  e: aiohttp.Clien
-00013850: 7452 6573 706f 6e73 6529 3a0a 2020 2020  tResponse):.    
-00013860: 2020 2020 6d61 7463 6820 3d20 7365 6c66      match = self
-00013870: 2e41 5049 5f55 524c 5f52 4547 4558 2e73  .API_URL_REGEX.s
-00013880: 6561 7263 6828 6d73 6729 0a20 2020 2020  earch(msg).     
-00013890: 2020 2069 6620 6d61 7463 6820 6973 206e     if match is n
-000138a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000138b0: 2020 2020 2062 6f74 5f74 6f6b 656e 203d       bot_token =
-000138c0: 206d 6174 6368 2e67 726f 7570 2822 746f   match.group("to
-000138d0: 6b65 6e22 290a 2020 2020 2020 2020 2020  ken").          
-000138e0: 2020 6d61 736b 6564 5f74 6f6b 656e 203d    masked_token =
-000138f0: 2062 6f74 5f74 6f6b 656e 5b3a 335d 202b   bot_token[:3] +
-00013900: 2022 2a22 202a 2028 6c65 6e28 626f 745f   "*" * (len(bot_
-00013910: 746f 6b65 6e29 202d 2033 290a 2020 2020  token) - 3).    
-00013920: 2020 2020 2020 2020 6d73 6720 3d20 6d73          msg = ms
-00013930: 672e 7265 706c 6163 6528 626f 745f 746f  g.replace(bot_to
-00013940: 6b65 6e2c 206d 6173 6b65 645f 746f 6b65  ken, masked_toke
-00013950: 6e29 0a0a 2020 2020 2020 2020 7375 7065  n)..        supe
-00013960: 7228 292e 5f5f 696e 6974 5f5f 286d 7367  r().__init__(msg
-00013970: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-00013980: 6573 706f 6e73 6520 3d20 7265 7370 6f6e  esponse = respon
-00013990: 7365 0a0a 0a63 6c61 7373 2041 7069 4854  se...class ApiHT
-000139a0: 5450 4578 6365 7074 696f 6e28 4170 6945  TPException(ApiE
-000139b0: 7863 6570 7469 6f6e 293a 0a20 2020 2022  xception):.    "
-000139c0: 2222 0a20 2020 2054 6869 7320 636c 6173  "".    This clas
-000139d0: 7320 7265 7072 6573 656e 7473 2061 6e20  s represents an 
-000139e0: 4578 6365 7074 696f 6e20 7468 726f 776e  Exception thrown
-000139f0: 2077 6865 6e20 6120 6361 6c6c 2074 6f20   when a call to 
-00013a00: 7468 650a 2020 2020 5465 6c65 6772 616d  the.    Telegram
-00013a10: 2041 5049 2073 6572 7665 7220 7265 7475   API server retu
-00013a20: 726e 7320 4854 5450 2063 6f64 6520 7468  rns HTTP code th
-00013a30: 6174 2069 7320 6e6f 7420 3230 302e 0a20  at is not 200.. 
-00013a40: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
-00013a50: 5f5f 696e 6974 5f5f 2873 656c 662c 2065  __init__(self, e
-00013a60: 7272 6f72 5f64 6573 6372 6970 7469 6f6e  rror_description
-00013a70: 3a20 7374 722c 2072 6573 706f 6e73 653a  : str, response:
-00013a80: 2061 696f 6874 7470 2e43 6c69 656e 7452   aiohttp.ClientR
-00013a90: 6573 706f 6e73 6529 3a0a 2020 2020 2020  esponse):.      
-00013aa0: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-00013ab0: 5f5f 280a 2020 2020 2020 2020 2020 2020  __(.            
-00013ac0: 6622 7b65 7272 6f72 5f64 6573 6372 6970  f"{error_descrip
-00013ad0: 7469 6f6e 7d20 287b 7265 7370 6f6e 7365  tion} ({response
-00013ae0: 2e75 726c 7d20 7265 7370 6f6e 6465 6420  .url} responded 
-00013af0: 7769 7468 207b 7265 7370 6f6e 7365 2e73  with {response.s
-00013b00: 7461 7475 737d 207b 7265 7370 6f6e 7365  tatus} {response
-00013b10: 2e72 6561 736f 6e7d 2922 2c0a 2020 2020  .reason})",.    
-00013b20: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00013b30: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00013b40: 2020 2020 7365 6c66 2e65 7272 6f72 5f64      self.error_d
-00013b50: 6573 6372 6970 7469 6f6e 203d 2065 7272  escription = err
-00013b60: 6f72 5f64 6573 6372 6970 7469 6f6e 0a0a  or_description..
-00013b70: 0a63 6c61 7373 2041 7069 496e 7661 6c69  .class ApiInvali
-00013b80: 644a 534f 4e45 7863 6570 7469 6f6e 2841  dJSONException(A
-00013b90: 7069 4578 6365 7074 696f 6e29 3a0a 2020  piException):.  
-00013ba0: 2020 2222 220a 2020 2020 5468 6973 2063    """.    This c
-00013bb0: 6c61 7373 2072 6570 7265 7365 6e74 7320  lass represents 
-00013bc0: 616e 2045 7863 6570 7469 6f6e 2074 6872  an Exception thr
-00013bd0: 6f77 6e20 7768 656e 2061 2063 616c 6c20  own when a call 
-00013be0: 746f 2074 6865 0a20 2020 2054 656c 6567  to the.    Teleg
-00013bf0: 7261 6d20 4150 4920 7365 7276 6572 2072  ram API server r
-00013c00: 6574 7572 6e73 2069 6e76 616c 6964 206a  eturns invalid j
-00013c10: 736f 6e2e 0a20 2020 2022 2222 0a0a 2020  son..    """..  
-00013c20: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00013c30: 656c 662c 2072 6573 706f 6e73 653a 2061  elf, response: a
-00013c40: 696f 6874 7470 2e43 6c69 656e 7452 6573  iohttp.ClientRes
-00013c50: 706f 6e73 652c 206a 736f 6e5f 7061 7273  ponse, json_pars
-00013c60: 696e 675f 6572 726f 723a 2045 7863 6570  ing_error: Excep
-00013c70: 7469 6f6e 293a 0a20 2020 2020 2020 2073  tion):.        s
-00013c80: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-00013c90: 0a20 2020 2020 2020 2020 2020 2022 5468  .            "Th
-00013ca0: 6520 7365 7276 6572 2072 6574 7572 6e65  e server returne
-00013cb0: 6420 616e 2069 6e76 616c 6964 204a 534f  d an invalid JSO
-00013cc0: 4e20 7265 7370 6f6e 7365 2e20 5265 7370  N response. Resp
-00013cd0: 6f6e 7365 2062 6f64 793a 220a 2020 2020  onse body:".    
-00013ce0: 2020 2020 2020 2020 2b20 6622 5c6e 5b7b          + f"\n[{
-00013cf0: 7265 7370 6f6e 7365 7d5d 5c6e 4a53 4f4e  response}]\nJSON
-00013d00: 2070 6172 7369 6e67 2065 7272 6f72 3a20   parsing error: 
-00013d10: 7b6a 736f 6e5f 7061 7273 696e 675f 6572  {json_parsing_er
-00013d20: 726f 727d 222c 0a20 2020 2020 2020 2020  ror}",.         
-00013d30: 2020 2072 6573 706f 6e73 652c 0a20 2020     response,.   
-00013d40: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-00013d50: 656c 662e 6a73 6f6e 5f70 6172 7369 6e67  elf.json_parsing
-00013d60: 5f65 7272 6f72 203d 206a 736f 6e5f 7061  _error = json_pa
-00013d70: 7273 696e 675f 6572 726f 720a            rsing_error.
+0000a550: 2263 7265 6174 6573 5f6a 6f69 6e5f 7265  "creates_join_re
+0000a560: 7175 6573 7422 5d20 3d20 6372 6561 7465  quest"] = create
+0000a570: 735f 6a6f 696e 5f72 6571 7565 7374 0a0a  s_join_request..
+0000a580: 2020 2020 7265 7475 726e 2061 7761 6974      return await
+0000a590: 205f 7265 7175 6573 7428 746f 6b65 6e2c   _request(token,
+0000a5a0: 206d 6574 686f 645f 7572 6c2c 2070 6172   method_url, par
+0000a5b0: 616d 733d 7061 796c 6f61 642c 206d 6574  ams=payload, met
+0000a5c0: 686f 643d 2270 6f73 7422 290a 0a0a 6173  hod="post")...as
+0000a5d0: 796e 6320 6465 6620 6765 745f 6375 7374  ync def get_cust
+0000a5e0: 6f6d 5f65 6d6f 6a69 5f73 7469 636b 6572  om_emoji_sticker
+0000a5f0: 7328 746f 6b65 6e2c 2063 7573 746f 6d5f  s(token, custom_
+0000a600: 656d 6f6a 695f 6964 7329 3a0a 2020 2020  emoji_ids):.    
+0000a610: 726f 7574 6520 3d20 7222 6765 7443 7573  route = r"getCus
+0000a620: 746f 6d45 6d6f 6a69 5374 6963 6b65 7273  tomEmojiStickers
+0000a630: 220a 2020 2020 7265 7475 726e 2061 7761  ".    return awa
+0000a640: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
+0000a650: 6e2c 2072 6f75 7465 2c20 7061 7261 6d73  n, route, params
+0000a660: 3d7b 2263 7573 746f 6d5f 656d 6f6a 695f  ={"custom_emoji_
+0000a670: 6964 7322 3a20 6375 7374 6f6d 5f65 6d6f  ids": custom_emo
+0000a680: 6a69 5f69 6473 7d29 0a0a 0a61 7379 6e63  ji_ids})...async
+0000a690: 2064 6566 2072 6576 6f6b 655f 6368 6174   def revoke_chat
+0000a6a0: 5f69 6e76 6974 655f 6c69 6e6b 2874 6f6b  _invite_link(tok
+0000a6b0: 656e 2c20 6368 6174 5f69 642c 2069 6e76  en, chat_id, inv
+0000a6c0: 6974 655f 6c69 6e6b 293a 0a20 2020 2072  ite_link):.    r
+0000a6d0: 6f75 7465 203d 2022 7265 766f 6b65 4368  oute = "revokeCh
+0000a6e0: 6174 496e 7669 7465 4c69 6e6b 220a 2020  atInviteLink".  
+0000a6f0: 2020 7061 796c 6f61 6420 3d20 7b22 6368    payload = {"ch
+0000a700: 6174 5f69 6422 3a20 6368 6174 5f69 642c  at_id": chat_id,
+0000a710: 2022 696e 7669 7465 5f6c 696e 6b22 3a20   "invite_link": 
+0000a720: 696e 7669 7465 5f6c 696e 6b7d 0a20 2020  invite_link}.   
+0000a730: 2072 6574 7572 6e20 6177 6169 7420 5f72   return await _r
+0000a740: 6571 7565 7374 2874 6f6b 656e 2c20 726f  equest(token, ro
+0000a750: 7574 652c 2070 6172 616d 733d 7061 796c  ute, params=payl
+0000a760: 6f61 642c 206d 6574 686f 643d 2270 6f73  oad, method="pos
+0000a770: 7422 290a 0a0a 6173 796e 6320 6465 6620  t")...async def 
+0000a780: 6578 706f 7274 5f63 6861 745f 696e 7669  export_chat_invi
+0000a790: 7465 5f6c 696e 6b28 746f 6b65 6e2c 2063  te_link(token, c
+0000a7a0: 6861 745f 6964 293a 0a20 2020 206d 6574  hat_id):.    met
+0000a7b0: 686f 645f 7572 6c20 3d20 2265 7870 6f72  hod_url = "expor
+0000a7c0: 7443 6861 7449 6e76 6974 654c 696e 6b22  tChatInviteLink"
+0000a7d0: 0a20 2020 2070 6179 6c6f 6164 203d 207b  .    payload = {
+0000a7e0: 2263 6861 745f 6964 223a 2063 6861 745f  "chat_id": chat_
+0000a7f0: 6964 7d0a 2020 2020 7265 7475 726e 2061  id}.    return a
+0000a800: 7761 6974 205f 7265 7175 6573 7428 746f  wait _request(to
+0000a810: 6b65 6e2c 206d 6574 686f 645f 7572 6c2c  ken, method_url,
+0000a820: 2070 6172 616d 733d 7061 796c 6f61 642c   params=payload,
+0000a830: 206d 6574 686f 643d 2270 6f73 7422 290a   method="post").
+0000a840: 0a0a 6173 796e 6320 6465 6620 6170 7072  ..async def appr
+0000a850: 6f76 655f 6368 6174 5f6a 6f69 6e5f 7265  ove_chat_join_re
+0000a860: 7175 6573 7428 746f 6b65 6e2c 2063 6861  quest(token, cha
+0000a870: 745f 6964 2c20 7573 6572 5f69 6429 3a0a  t_id, user_id):.
+0000a880: 2020 2020 6d65 7468 6f64 5f75 726c 203d      method_url =
+0000a890: 2022 6170 7072 6f76 6543 6861 744a 6f69   "approveChatJoi
+0000a8a0: 6e52 6571 7565 7374 220a 2020 2020 7061  nRequest".    pa
+0000a8b0: 796c 6f61 6420 3d20 7b22 6368 6174 5f69  yload = {"chat_i
+0000a8c0: 6422 3a20 6368 6174 5f69 642c 2022 7573  d": chat_id, "us
+0000a8d0: 6572 5f69 6422 3a20 7573 6572 5f69 647d  er_id": user_id}
+0000a8e0: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
+0000a8f0: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
+0000a900: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
+0000a910: 7261 6d73 3d70 6179 6c6f 6164 2c20 6d65  rams=payload, me
+0000a920: 7468 6f64 3d22 706f 7374 2229 0a0a 0a61  thod="post")...a
+0000a930: 7379 6e63 2064 6566 2064 6563 6c69 6e65  sync def decline
+0000a940: 5f63 6861 745f 6a6f 696e 5f72 6571 7565  _chat_join_reque
+0000a950: 7374 2874 6f6b 656e 2c20 6368 6174 5f69  st(token, chat_i
+0000a960: 642c 2075 7365 725f 6964 293a 0a20 2020  d, user_id):.   
+0000a970: 206d 6574 686f 645f 7572 6c20 3d20 2264   method_url = "d
+0000a980: 6563 6c69 6e65 4368 6174 4a6f 696e 5265  eclineChatJoinRe
+0000a990: 7175 6573 7422 0a20 2020 2070 6179 6c6f  quest".    paylo
+0000a9a0: 6164 203d 207b 2263 6861 745f 6964 223a  ad = {"chat_id":
+0000a9b0: 2063 6861 745f 6964 2c20 2275 7365 725f   chat_id, "user_
+0000a9c0: 6964 223a 2075 7365 725f 6964 7d0a 2020  id": user_id}.  
+0000a9d0: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
+0000a9e0: 7265 7175 6573 7428 746f 6b65 6e2c 206d  request(token, m
+0000a9f0: 6574 686f 645f 7572 6c2c 2070 6172 616d  ethod_url, param
+0000aa00: 733d 7061 796c 6f61 642c 206d 6574 686f  s=payload, metho
+0000aa10: 643d 2270 6f73 7422 290a 0a0a 6173 796e  d="post")...asyn
+0000aa20: 6320 6465 6620 7365 745f 6368 6174 5f70  c def set_chat_p
+0000aa30: 686f 746f 2874 6f6b 656e 2c20 6368 6174  hoto(token, chat
+0000aa40: 5f69 642c 2070 686f 746f 293a 0a20 2020  _id, photo):.   
+0000aa50: 206d 6574 686f 645f 7572 6c20 3d20 2273   method_url = "s
+0000aa60: 6574 4368 6174 5068 6f74 6f22 0a20 2020  etChatPhoto".   
+0000aa70: 2070 6179 6c6f 6164 203d 207b 2263 6861   payload = {"cha
+0000aa80: 745f 6964 223a 2063 6861 745f 6964 7d0a  t_id": chat_id}.
+0000aa90: 2020 2020 6669 6c65 7320 3d20 4e6f 6e65      files = None
+0000aaa0: 0a20 2020 2069 6620 7574 696c 2e69 735f  .    if util.is_
+0000aab0: 7374 7269 6e67 2870 686f 746f 293a 0a20  string(photo):. 
+0000aac0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+0000aad0: 7068 6f74 6f22 5d20 3d20 7068 6f74 6f0a  photo"] = photo.
+0000aae0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000aaf0: 2020 6669 6c65 7320 3d20 7b22 7068 6f74    files = {"phot
+0000ab00: 6f22 3a20 7068 6f74 6f7d 0a20 2020 2072  o": photo}.    r
+0000ab10: 6574 7572 6e20 6177 6169 7420 5f72 6571  eturn await _req
+0000ab20: 7565 7374 2874 6f6b 656e 2c20 6d65 7468  uest(token, meth
+0000ab30: 6f64 5f75 726c 2c20 7061 7261 6d73 3d70  od_url, params=p
+0000ab40: 6179 6c6f 6164 2c20 6669 6c65 733d 6669  ayload, files=fi
+0000ab50: 6c65 732c 206d 6574 686f 643d 2270 6f73  les, method="pos
+0000ab60: 7422 290a 0a0a 6173 796e 6320 6465 6620  t")...async def 
+0000ab70: 6465 6c65 7465 5f63 6861 745f 7068 6f74  delete_chat_phot
+0000ab80: 6f28 746f 6b65 6e2c 2063 6861 745f 6964  o(token, chat_id
+0000ab90: 293a 0a20 2020 206d 6574 686f 645f 7572  ):.    method_ur
+0000aba0: 6c20 3d20 2264 656c 6574 6543 6861 7450  l = "deleteChatP
+0000abb0: 686f 746f 220a 2020 2020 7061 796c 6f61  hoto".    payloa
+0000abc0: 6420 3d20 7b22 6368 6174 5f69 6422 3a20  d = {"chat_id": 
+0000abd0: 6368 6174 5f69 647d 0a20 2020 2072 6574  chat_id}.    ret
+0000abe0: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
+0000abf0: 7374 2874 6f6b 656e 2c20 6d65 7468 6f64  st(token, method
+0000ac00: 5f75 726c 2c20 7061 7261 6d73 3d70 6179  _url, params=pay
+0000ac10: 6c6f 6164 2c20 6d65 7468 6f64 3d22 706f  load, method="po
+0000ac20: 7374 2229 0a0a 0a61 7379 6e63 2064 6566  st")...async def
+0000ac30: 2073 6574 5f63 6861 745f 7469 746c 6528   set_chat_title(
+0000ac40: 746f 6b65 6e2c 2063 6861 745f 6964 2c20  token, chat_id, 
+0000ac50: 7469 746c 6529 3a0a 2020 2020 6d65 7468  title):.    meth
+0000ac60: 6f64 5f75 726c 203d 2022 7365 7443 6861  od_url = "setCha
+0000ac70: 7454 6974 6c65 220a 2020 2020 7061 796c  tTitle".    payl
+0000ac80: 6f61 6420 3d20 7b22 6368 6174 5f69 6422  oad = {"chat_id"
+0000ac90: 3a20 6368 6174 5f69 642c 2022 7469 746c  : chat_id, "titl
+0000aca0: 6522 3a20 7469 746c 657d 0a20 2020 2072  e": title}.    r
+0000acb0: 6574 7572 6e20 6177 6169 7420 5f72 6571  eturn await _req
+0000acc0: 7565 7374 2874 6f6b 656e 2c20 6d65 7468  uest(token, meth
+0000acd0: 6f64 5f75 726c 2c20 7061 7261 6d73 3d70  od_url, params=p
+0000ace0: 6179 6c6f 6164 2c20 6d65 7468 6f64 3d22  ayload, method="
+0000acf0: 706f 7374 2229 0a0a 0a61 7379 6e63 2064  post")...async d
+0000ad00: 6566 2067 6574 5f6d 795f 636f 6d6d 616e  ef get_my_comman
+0000ad10: 6473 2874 6f6b 656e 2c20 7363 6f70 653d  ds(token, scope=
+0000ad20: 4e6f 6e65 2c20 6c61 6e67 7561 6765 5f63  None, language_c
+0000ad30: 6f64 653d 4e6f 6e65 293a 0a20 2020 206d  ode=None):.    m
+0000ad40: 6574 686f 645f 7572 6c20 3d20 7222 6765  ethod_url = r"ge
+0000ad50: 744d 7943 6f6d 6d61 6e64 7322 0a20 2020  tMyCommands".   
+0000ad60: 2070 6179 6c6f 6164 203d 207b 7d0a 2020   payload = {}.  
+0000ad70: 2020 6966 2073 636f 7065 3a0a 2020 2020    if scope:.    
+0000ad80: 2020 2020 7061 796c 6f61 645b 2273 636f      payload["sco
+0000ad90: 7065 225d 203d 2073 636f 7065 2e74 6f5f  pe"] = scope.to_
+0000ada0: 6a73 6f6e 2829 0a20 2020 2069 6620 6c61  json().    if la
+0000adb0: 6e67 7561 6765 5f63 6f64 653a 0a20 2020  nguage_code:.   
+0000adc0: 2020 2020 2070 6179 6c6f 6164 5b22 6c61       payload["la
+0000add0: 6e67 7561 6765 5f63 6f64 6522 5d20 3d20  nguage_code"] = 
+0000ade0: 6c61 6e67 7561 6765 5f63 6f64 650a 2020  language_code.  
+0000adf0: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
+0000ae00: 7265 7175 6573 7428 746f 6b65 6e2c 206d  request(token, m
+0000ae10: 6574 686f 645f 7572 6c2c 2070 6172 616d  ethod_url, param
+0000ae20: 733d 7061 796c 6f61 6429 0a0a 0a61 7379  s=payload)...asy
+0000ae30: 6e63 2064 6566 2073 6574 5f63 6861 745f  nc def set_chat_
+0000ae40: 6d65 6e75 5f62 7574 746f 6e28 746f 6b65  menu_button(toke
+0000ae50: 6e2c 2063 6861 745f 6964 3d4e 6f6e 652c  n, chat_id=None,
+0000ae60: 206d 656e 755f 6275 7474 6f6e 3d4e 6f6e   menu_button=Non
+0000ae70: 6529 3a0a 2020 2020 6d65 7468 6f64 5f75  e):.    method_u
+0000ae80: 726c 203d 2072 2273 6574 4368 6174 4d65  rl = r"setChatMe
+0000ae90: 6e75 4275 7474 6f6e 220a 2020 2020 7061  nuButton".    pa
+0000aea0: 796c 6f61 6420 3d20 7b7d 0a20 2020 2069  yload = {}.    i
+0000aeb0: 6620 6368 6174 5f69 643a 0a20 2020 2020  f chat_id:.     
+0000aec0: 2020 2070 6179 6c6f 6164 5b22 6368 6174     payload["chat
+0000aed0: 5f69 6422 5d20 3d20 6368 6174 5f69 640a  _id"] = chat_id.
+0000aee0: 2020 2020 6966 206d 656e 755f 6275 7474      if menu_butt
+0000aef0: 6f6e 3a0a 2020 2020 2020 2020 7061 796c  on:.        payl
+0000af00: 6f61 645b 226d 656e 755f 6275 7474 6f6e  oad["menu_button
+0000af10: 225d 203d 206d 656e 755f 6275 7474 6f6e  "] = menu_button
+0000af20: 2e74 6f5f 6a73 6f6e 2829 0a0a 2020 2020  .to_json()..    
+0000af30: 7265 7475 726e 2061 7761 6974 205f 7265  return await _re
+0000af40: 7175 6573 7428 746f 6b65 6e2c 206d 6574  quest(token, met
+0000af50: 686f 645f 7572 6c2c 2070 6172 616d 733d  hod_url, params=
+0000af60: 7061 796c 6f61 642c 206d 6574 686f 643d  payload, method=
+0000af70: 2270 6f73 7422 290a 0a0a 6173 796e 6320  "post")...async 
+0000af80: 6465 6620 6765 745f 6368 6174 5f6d 656e  def get_chat_men
+0000af90: 755f 6275 7474 6f6e 2874 6f6b 656e 2c20  u_button(token, 
+0000afa0: 6368 6174 5f69 643d 4e6f 6e65 293a 0a20  chat_id=None):. 
+0000afb0: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
+0000afc0: 7222 6765 7443 6861 744d 656e 7542 7574  r"getChatMenuBut
+0000afd0: 746f 6e22 0a20 2020 2070 6179 6c6f 6164  ton".    payload
+0000afe0: 203d 207b 7d0a 2020 2020 6966 2063 6861   = {}.    if cha
+0000aff0: 745f 6964 3a0a 2020 2020 2020 2020 7061  t_id:.        pa
+0000b000: 796c 6f61 645b 2263 6861 745f 6964 225d  yload["chat_id"]
+0000b010: 203d 2063 6861 745f 6964 0a0a 2020 2020   = chat_id..    
+0000b020: 7265 7475 726e 2061 7761 6974 205f 7265  return await _re
+0000b030: 7175 6573 7428 746f 6b65 6e2c 206d 6574  quest(token, met
+0000b040: 686f 645f 7572 6c2c 2070 6172 616d 733d  hod_url, params=
+0000b050: 7061 796c 6f61 642c 206d 6574 686f 643d  payload, method=
+0000b060: 2270 6f73 7422 290a 0a0a 6173 796e 6320  "post")...async 
+0000b070: 6465 6620 7365 745f 6d79 5f64 6566 6175  def set_my_defau
+0000b080: 6c74 5f61 646d 696e 6973 7472 6174 6f72  lt_administrator
+0000b090: 5f72 6967 6874 7328 746f 6b65 6e2c 2072  _rights(token, r
+0000b0a0: 6967 6874 733d 4e6f 6e65 2c20 666f 725f  ights=None, for_
+0000b0b0: 6368 616e 6e65 6c73 3d4e 6f6e 6529 3a0a  channels=None):.
+0000b0c0: 2020 2020 6d65 7468 6f64 5f75 726c 203d      method_url =
+0000b0d0: 2072 2273 6574 4d79 4465 6661 756c 7441   r"setMyDefaultA
+0000b0e0: 646d 696e 6973 7472 6174 6f72 5269 6768  dministratorRigh
+0000b0f0: 7473 220a 2020 2020 7061 796c 6f61 6420  ts".    payload 
+0000b100: 3d20 7b7d 0a20 2020 2069 6620 7269 6768  = {}.    if righ
+0000b110: 7473 3a0a 2020 2020 2020 2020 7061 796c  ts:.        payl
+0000b120: 6f61 645b 2272 6967 6874 7322 5d20 3d20  oad["rights"] = 
+0000b130: 7269 6768 7473 2e74 6f5f 6a73 6f6e 2829  rights.to_json()
+0000b140: 0a20 2020 2069 6620 666f 725f 6368 616e  .    if for_chan
+0000b150: 6e65 6c73 2069 7320 6e6f 7420 4e6f 6e65  nels is not None
+0000b160: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+0000b170: 645b 2266 6f72 5f63 6861 6e6e 656c 7322  d["for_channels"
+0000b180: 5d20 3d20 666f 725f 6368 616e 6e65 6c73  ] = for_channels
+0000b190: 0a0a 2020 2020 7265 7475 726e 2061 7761  ..    return awa
+0000b1a0: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
+0000b1b0: 6e2c 206d 6574 686f 645f 7572 6c2c 2070  n, method_url, p
+0000b1c0: 6172 616d 733d 7061 796c 6f61 642c 206d  arams=payload, m
+0000b1d0: 6574 686f 643d 2270 6f73 7422 290a 0a0a  ethod="post")...
+0000b1e0: 6173 796e 6320 6465 6620 6765 745f 6d79  async def get_my
+0000b1f0: 5f64 6566 6175 6c74 5f61 646d 696e 6973  _default_adminis
+0000b200: 7472 6174 6f72 5f72 6967 6874 7328 746f  trator_rights(to
+0000b210: 6b65 6e2c 2066 6f72 5f63 6861 6e6e 656c  ken, for_channel
+0000b220: 733d 4e6f 6e65 293a 0a20 2020 206d 6574  s=None):.    met
+0000b230: 686f 645f 7572 6c20 3d20 7222 6765 744d  hod_url = r"getM
+0000b240: 7944 6566 6175 6c74 4164 6d69 6e69 7374  yDefaultAdminist
+0000b250: 7261 746f 7252 6967 6874 7322 0a20 2020  ratorRights".   
+0000b260: 2070 6179 6c6f 6164 203d 207b 7d0a 2020   payload = {}.  
+0000b270: 2020 6966 2066 6f72 5f63 6861 6e6e 656c    if for_channel
+0000b280: 733a 0a20 2020 2020 2020 2070 6179 6c6f  s:.        paylo
+0000b290: 6164 5b22 666f 725f 6368 616e 6e65 6c73  ad["for_channels
+0000b2a0: 225d 203d 2066 6f72 5f63 6861 6e6e 656c  "] = for_channel
+0000b2b0: 730a 0a20 2020 2072 6574 7572 6e20 6177  s..    return aw
+0000b2c0: 6169 7420 5f72 6571 7565 7374 2874 6f6b  ait _request(tok
+0000b2d0: 656e 2c20 6d65 7468 6f64 5f75 726c 2c20  en, method_url, 
+0000b2e0: 7061 7261 6d73 3d70 6179 6c6f 6164 2c20  params=payload, 
+0000b2f0: 6d65 7468 6f64 3d22 706f 7374 2229 0a0a  method="post")..
+0000b300: 0a61 7379 6e63 2064 6566 2073 6574 5f6d  .async def set_m
+0000b310: 795f 636f 6d6d 616e 6473 2874 6f6b 656e  y_commands(token
+0000b320: 2c20 636f 6d6d 616e 6473 2c20 7363 6f70  , commands, scop
+0000b330: 653d 4e6f 6e65 2c20 6c61 6e67 7561 6765  e=None, language
+0000b340: 5f63 6f64 653d 4e6f 6e65 293a 0a20 2020  _code=None):.   
+0000b350: 206d 6574 686f 645f 7572 6c20 3d20 7222   method_url = r"
+0000b360: 7365 744d 7943 6f6d 6d61 6e64 7322 0a20  setMyCommands". 
+0000b370: 2020 2070 6179 6c6f 6164 203d 207b 2263     payload = {"c
+0000b380: 6f6d 6d61 6e64 7322 3a20 6177 6169 7420  ommands": await 
+0000b390: 5f63 6f6e 7665 7274 5f6c 6973 745f 6a73  _convert_list_js
+0000b3a0: 6f6e 5f73 6572 6961 6c69 7a61 626c 6528  on_serializable(
+0000b3b0: 636f 6d6d 616e 6473 297d 0a20 2020 2069  commands)}.    i
+0000b3c0: 6620 7363 6f70 653a 0a20 2020 2020 2020  f scope:.       
+0000b3d0: 2070 6179 6c6f 6164 5b22 7363 6f70 6522   payload["scope"
+0000b3e0: 5d20 3d20 7363 6f70 652e 746f 5f6a 736f  ] = scope.to_jso
+0000b3f0: 6e28 290a 2020 2020 6966 206c 616e 6775  n().    if langu
+0000b400: 6167 655f 636f 6465 3a0a 2020 2020 2020  age_code:.      
+0000b410: 2020 7061 796c 6f61 645b 226c 616e 6775    payload["langu
+0000b420: 6167 655f 636f 6465 225d 203d 206c 616e  age_code"] = lan
+0000b430: 6775 6167 655f 636f 6465 0a20 2020 2072  guage_code.    r
+0000b440: 6574 7572 6e20 6177 6169 7420 5f72 6571  eturn await _req
+0000b450: 7565 7374 2874 6f6b 656e 2c20 6d65 7468  uest(token, meth
+0000b460: 6f64 5f75 726c 2c20 7061 7261 6d73 3d70  od_url, params=p
+0000b470: 6179 6c6f 6164 2c20 6d65 7468 6f64 3d22  ayload, method="
+0000b480: 706f 7374 2229 0a0a 0a61 7379 6e63 2064  post")...async d
+0000b490: 6566 2064 656c 6574 655f 6d79 5f63 6f6d  ef delete_my_com
+0000b4a0: 6d61 6e64 7328 746f 6b65 6e2c 2073 636f  mands(token, sco
+0000b4b0: 7065 3d4e 6f6e 652c 206c 616e 6775 6167  pe=None, languag
+0000b4c0: 655f 636f 6465 3d4e 6f6e 6529 3a0a 2020  e_code=None):.  
+0000b4d0: 2020 6d65 7468 6f64 5f75 726c 203d 2072    method_url = r
+0000b4e0: 2264 656c 6574 654d 7943 6f6d 6d61 6e64  "deleteMyCommand
+0000b4f0: 7322 0a20 2020 2070 6179 6c6f 6164 203d  s".    payload =
+0000b500: 207b 7d0a 2020 2020 6966 2073 636f 7065   {}.    if scope
+0000b510: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+0000b520: 645b 2273 636f 7065 225d 203d 2073 636f  d["scope"] = sco
+0000b530: 7065 2e74 6f5f 6a73 6f6e 2829 0a20 2020  pe.to_json().   
+0000b540: 2069 6620 6c61 6e67 7561 6765 5f63 6f64   if language_cod
+0000b550: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
+0000b560: 6164 5b22 6c61 6e67 7561 6765 5f63 6f64  ad["language_cod
+0000b570: 6522 5d20 3d20 6c61 6e67 7561 6765 5f63  e"] = language_c
+0000b580: 6f64 650a 2020 2020 7265 7475 726e 2061  ode.    return a
+0000b590: 7761 6974 205f 7265 7175 6573 7428 746f  wait _request(to
+0000b5a0: 6b65 6e2c 206d 6574 686f 645f 7572 6c2c  ken, method_url,
+0000b5b0: 2070 6172 616d 733d 7061 796c 6f61 642c   params=payload,
+0000b5c0: 206d 6574 686f 643d 2270 6f73 7422 290a   method="post").
+0000b5d0: 0a0a 6173 796e 6320 6465 6620 7365 745f  ..async def set_
+0000b5e0: 6368 6174 5f64 6573 6372 6970 7469 6f6e  chat_description
+0000b5f0: 2874 6f6b 656e 2c20 6368 6174 5f69 642c  (token, chat_id,
+0000b600: 2064 6573 6372 6970 7469 6f6e 293a 0a20   description):. 
+0000b610: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
+0000b620: 2273 6574 4368 6174 4465 7363 7269 7074  "setChatDescript
+0000b630: 696f 6e22 0a20 2020 2070 6179 6c6f 6164  ion".    payload
+0000b640: 203d 207b 2263 6861 745f 6964 223a 2063   = {"chat_id": c
+0000b650: 6861 745f 6964 7d0a 2020 2020 6966 2064  hat_id}.    if d
+0000b660: 6573 6372 6970 7469 6f6e 2069 7320 6e6f  escription is no
+0000b670: 7420 4e6f 6e65 3a20 2023 2041 6c6c 6f77  t None:  # Allow
+0000b680: 2065 6d70 7479 2073 7472 696e 6773 0a20   empty strings. 
+0000b690: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+0000b6a0: 6465 7363 7269 7074 696f 6e22 5d20 3d20  description"] = 
+0000b6b0: 6465 7363 7269 7074 696f 6e0a 2020 2020  description.    
+0000b6c0: 7265 7475 726e 2061 7761 6974 205f 7265  return await _re
+0000b6d0: 7175 6573 7428 746f 6b65 6e2c 206d 6574  quest(token, met
+0000b6e0: 686f 645f 7572 6c2c 2070 6172 616d 733d  hod_url, params=
+0000b6f0: 7061 796c 6f61 642c 206d 6574 686f 643d  payload, method=
+0000b700: 2270 6f73 7422 290a 0a0a 6173 796e 6320  "post")...async 
+0000b710: 6465 6620 7069 6e5f 6368 6174 5f6d 6573  def pin_chat_mes
+0000b720: 7361 6765 2874 6f6b 656e 2c20 6368 6174  sage(token, chat
+0000b730: 5f69 642c 206d 6573 7361 6765 5f69 642c  _id, message_id,
+0000b740: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
+0000b750: 6174 696f 6e3d 4e6f 6e65 293a 0a20 2020  ation=None):.   
+0000b760: 206d 6574 686f 645f 7572 6c20 3d20 2270   method_url = "p
+0000b770: 696e 4368 6174 4d65 7373 6167 6522 0a20  inChatMessage". 
+0000b780: 2020 2070 6179 6c6f 6164 203d 207b 2263     payload = {"c
+0000b790: 6861 745f 6964 223a 2063 6861 745f 6964  hat_id": chat_id
+0000b7a0: 2c20 226d 6573 7361 6765 5f69 6422 3a20  , "message_id": 
+0000b7b0: 6d65 7373 6167 655f 6964 7d0a 2020 2020  message_id}.    
+0000b7c0: 6966 2064 6973 6162 6c65 5f6e 6f74 6966  if disable_notif
+0000b7d0: 6963 6174 696f 6e20 6973 206e 6f74 204e  ication is not N
+0000b7e0: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
+0000b7f0: 6c6f 6164 5b22 6469 7361 626c 655f 6e6f  load["disable_no
+0000b800: 7469 6669 6361 7469 6f6e 225d 203d 2064  tification"] = d
+0000b810: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+0000b820: 696f 6e0a 2020 2020 7265 7475 726e 2061  ion.    return a
+0000b830: 7761 6974 205f 7265 7175 6573 7428 746f  wait _request(to
+0000b840: 6b65 6e2c 206d 6574 686f 645f 7572 6c2c  ken, method_url,
+0000b850: 2070 6172 616d 733d 7061 796c 6f61 642c   params=payload,
+0000b860: 206d 6574 686f 643d 2270 6f73 7422 290a   method="post").
+0000b870: 0a0a 6173 796e 6320 6465 6620 756e 7069  ..async def unpi
+0000b880: 6e5f 6368 6174 5f6d 6573 7361 6765 2874  n_chat_message(t
+0000b890: 6f6b 656e 2c20 6368 6174 5f69 642c 206d  oken, chat_id, m
+0000b8a0: 6573 7361 6765 5f69 6429 3a0a 2020 2020  essage_id):.    
+0000b8b0: 6d65 7468 6f64 5f75 726c 203d 2022 756e  method_url = "un
+0000b8c0: 7069 6e43 6861 744d 6573 7361 6765 220a  pinChatMessage".
+0000b8d0: 2020 2020 7061 796c 6f61 6420 3d20 7b22      payload = {"
+0000b8e0: 6368 6174 5f69 6422 3a20 6368 6174 5f69  chat_id": chat_i
+0000b8f0: 647d 0a20 2020 2069 6620 6d65 7373 6167  d}.    if messag
+0000b900: 655f 6964 3a0a 2020 2020 2020 2020 7061  e_id:.        pa
+0000b910: 796c 6f61 645b 226d 6573 7361 6765 5f69  yload["message_i
+0000b920: 6422 5d20 3d20 6d65 7373 6167 655f 6964  d"] = message_id
+0000b930: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
+0000b940: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
+0000b950: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
+0000b960: 7261 6d73 3d70 6179 6c6f 6164 2c20 6d65  rams=payload, me
+0000b970: 7468 6f64 3d22 706f 7374 2229 0a0a 0a61  thod="post")...a
+0000b980: 7379 6e63 2064 6566 2075 6e70 696e 5f61  sync def unpin_a
+0000b990: 6c6c 5f63 6861 745f 6d65 7373 6167 6573  ll_chat_messages
+0000b9a0: 2874 6f6b 656e 2c20 6368 6174 5f69 6429  (token, chat_id)
+0000b9b0: 3a0a 2020 2020 6d65 7468 6f64 5f75 726c  :.    method_url
+0000b9c0: 203d 2022 756e 7069 6e41 6c6c 4368 6174   = "unpinAllChat
+0000b9d0: 4d65 7373 6167 6573 220a 2020 2020 7061  Messages".    pa
+0000b9e0: 796c 6f61 6420 3d20 7b22 6368 6174 5f69  yload = {"chat_i
+0000b9f0: 6422 3a20 6368 6174 5f69 647d 0a20 2020  d": chat_id}.   
+0000ba00: 2072 6574 7572 6e20 6177 6169 7420 5f72   return await _r
+0000ba10: 6571 7565 7374 2874 6f6b 656e 2c20 6d65  equest(token, me
+0000ba20: 7468 6f64 5f75 726c 2c20 7061 7261 6d73  thod_url, params
+0000ba30: 3d70 6179 6c6f 6164 2c20 6d65 7468 6f64  =payload, method
+0000ba40: 3d22 706f 7374 2229 0a0a 0a23 2055 7064  ="post")...# Upd
+0000ba50: 6174 696e 6720 6d65 7373 6167 6573 0a0a  ating messages..
+0000ba60: 0a61 7379 6e63 2064 6566 2065 6469 745f  .async def edit_
+0000ba70: 6d65 7373 6167 655f 7465 7874 280a 2020  message_text(.  
+0000ba80: 2020 746f 6b65 6e2c 0a20 2020 2074 6578    token,.    tex
+0000ba90: 742c 0a20 2020 2063 6861 745f 6964 3d4e  t,.    chat_id=N
+0000baa0: 6f6e 652c 0a20 2020 206d 6573 7361 6765  one,.    message
+0000bab0: 5f69 643d 4e6f 6e65 2c0a 2020 2020 696e  _id=None,.    in
+0000bac0: 6c69 6e65 5f6d 6573 7361 6765 5f69 643d  line_message_id=
+0000bad0: 4e6f 6e65 2c0a 2020 2020 7061 7273 655f  None,.    parse_
+0000bae0: 6d6f 6465 3d4e 6f6e 652c 0a20 2020 2065  mode=None,.    e
+0000baf0: 6e74 6974 6965 733d 4e6f 6e65 2c0a 2020  ntities=None,.  
+0000bb00: 2020 6469 7361 626c 655f 7765 625f 7061    disable_web_pa
+0000bb10: 6765 5f70 7265 7669 6577 3d4e 6f6e 652c  ge_preview=None,
+0000bb20: 0a20 2020 2072 6570 6c79 5f6d 6172 6b75  .    reply_marku
+0000bb30: 703d 4e6f 6e65 2c0a 293a 0a20 2020 206d  p=None,.):.    m
+0000bb40: 6574 686f 645f 7572 6c20 3d20 7222 6564  ethod_url = r"ed
+0000bb50: 6974 4d65 7373 6167 6554 6578 7422 0a20  itMessageText". 
+0000bb60: 2020 2070 6179 6c6f 6164 203d 207b 2274     payload = {"t
+0000bb70: 6578 7422 3a20 7465 7874 7d0a 2020 2020  ext": text}.    
+0000bb80: 6966 2063 6861 745f 6964 3a0a 2020 2020  if chat_id:.    
+0000bb90: 2020 2020 7061 796c 6f61 645b 2263 6861      payload["cha
+0000bba0: 745f 6964 225d 203d 2063 6861 745f 6964  t_id"] = chat_id
+0000bbb0: 0a20 2020 2069 6620 6d65 7373 6167 655f  .    if message_
+0000bbc0: 6964 3a0a 2020 2020 2020 2020 7061 796c  id:.        payl
+0000bbd0: 6f61 645b 226d 6573 7361 6765 5f69 6422  oad["message_id"
+0000bbe0: 5d20 3d20 6d65 7373 6167 655f 6964 0a20  ] = message_id. 
+0000bbf0: 2020 2069 6620 696e 6c69 6e65 5f6d 6573     if inline_mes
+0000bc00: 7361 6765 5f69 643a 0a20 2020 2020 2020  sage_id:.       
+0000bc10: 2070 6179 6c6f 6164 5b22 696e 6c69 6e65   payload["inline
+0000bc20: 5f6d 6573 7361 6765 5f69 6422 5d20 3d20  _message_id"] = 
+0000bc30: 696e 6c69 6e65 5f6d 6573 7361 6765 5f69  inline_message_i
+0000bc40: 640a 2020 2020 6966 2070 6172 7365 5f6d  d.    if parse_m
+0000bc50: 6f64 653a 0a20 2020 2020 2020 2070 6179  ode:.        pay
+0000bc60: 6c6f 6164 5b22 7061 7273 655f 6d6f 6465  load["parse_mode
+0000bc70: 225d 203d 2070 6172 7365 5f6d 6f64 650a  "] = parse_mode.
+0000bc80: 2020 2020 6966 2065 6e74 6974 6965 733a      if entities:
+0000bc90: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+0000bca0: 5b22 656e 7469 7469 6573 225d 203d 206a  ["entities"] = j
+0000bcb0: 736f 6e2e 6475 6d70 7328 7479 7065 732e  son.dumps(types.
+0000bcc0: 4d65 7373 6167 6545 6e74 6974 792e 746f  MessageEntity.to
+0000bcd0: 5f6c 6973 745f 6f66 5f64 6963 7473 2865  _list_of_dicts(e
+0000bce0: 6e74 6974 6965 7329 290a 2020 2020 6966  ntities)).    if
+0000bcf0: 2064 6973 6162 6c65 5f77 6562 5f70 6167   disable_web_pag
+0000bd00: 655f 7072 6576 6965 7720 6973 206e 6f74  e_preview is not
+0000bd10: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
+0000bd20: 6179 6c6f 6164 5b22 6469 7361 626c 655f  ayload["disable_
+0000bd30: 7765 625f 7061 6765 5f70 7265 7669 6577  web_page_preview
+0000bd40: 225d 203d 2064 6973 6162 6c65 5f77 6562  "] = disable_web
+0000bd50: 5f70 6167 655f 7072 6576 6965 770a 2020  _page_preview.  
+0000bd60: 2020 6966 2072 6570 6c79 5f6d 6172 6b75    if reply_marku
+0000bd70: 703a 0a20 2020 2020 2020 2070 6179 6c6f  p:.        paylo
+0000bd80: 6164 5b22 7265 706c 795f 6d61 726b 7570  ad["reply_markup
+0000bd90: 225d 203d 2061 7761 6974 205f 636f 6e76  "] = await _conv
+0000bda0: 6572 745f 6d61 726b 7570 2872 6570 6c79  ert_markup(reply
+0000bdb0: 5f6d 6172 6b75 7029 0a20 2020 2072 6574  _markup).    ret
+0000bdc0: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
+0000bdd0: 7374 2874 6f6b 656e 2c20 6d65 7468 6f64  st(token, method
+0000bde0: 5f75 726c 2c20 7061 7261 6d73 3d70 6179  _url, params=pay
+0000bdf0: 6c6f 6164 2c20 6d65 7468 6f64 3d22 706f  load, method="po
+0000be00: 7374 2229 0a0a 0a61 7379 6e63 2064 6566  st")...async def
+0000be10: 2065 6469 745f 6d65 7373 6167 655f 6361   edit_message_ca
+0000be20: 7074 696f 6e28 0a20 2020 2074 6f6b 656e  ption(.    token
+0000be30: 2c0a 2020 2020 6361 7074 696f 6e2c 0a20  ,.    caption,. 
+0000be40: 2020 2063 6861 745f 6964 3d4e 6f6e 652c     chat_id=None,
+0000be50: 0a20 2020 206d 6573 7361 6765 5f69 643d  .    message_id=
+0000be60: 4e6f 6e65 2c0a 2020 2020 696e 6c69 6e65  None,.    inline
+0000be70: 5f6d 6573 7361 6765 5f69 643d 4e6f 6e65  _message_id=None
+0000be80: 2c0a 2020 2020 7061 7273 655f 6d6f 6465  ,.    parse_mode
+0000be90: 3d4e 6f6e 652c 0a20 2020 2063 6170 7469  =None,.    capti
+0000bea0: 6f6e 5f65 6e74 6974 6965 733d 4e6f 6e65  on_entities=None
+0000beb0: 2c0a 2020 2020 7265 706c 795f 6d61 726b  ,.    reply_mark
+0000bec0: 7570 3d4e 6f6e 652c 0a29 3a0a 2020 2020  up=None,.):.    
+0000bed0: 6d65 7468 6f64 5f75 726c 203d 2072 2265  method_url = r"e
+0000bee0: 6469 744d 6573 7361 6765 4361 7074 696f  ditMessageCaptio
+0000bef0: 6e22 0a20 2020 2070 6179 6c6f 6164 203d  n".    payload =
+0000bf00: 207b 2263 6170 7469 6f6e 223a 2063 6170   {"caption": cap
+0000bf10: 7469 6f6e 7d0a 2020 2020 6966 2063 6861  tion}.    if cha
+0000bf20: 745f 6964 3a0a 2020 2020 2020 2020 7061  t_id:.        pa
+0000bf30: 796c 6f61 645b 2263 6861 745f 6964 225d  yload["chat_id"]
+0000bf40: 203d 2063 6861 745f 6964 0a20 2020 2069   = chat_id.    i
+0000bf50: 6620 6d65 7373 6167 655f 6964 3a0a 2020  f message_id:.  
+0000bf60: 2020 2020 2020 7061 796c 6f61 645b 226d        payload["m
+0000bf70: 6573 7361 6765 5f69 6422 5d20 3d20 6d65  essage_id"] = me
+0000bf80: 7373 6167 655f 6964 0a20 2020 2069 6620  ssage_id.    if 
+0000bf90: 696e 6c69 6e65 5f6d 6573 7361 6765 5f69  inline_message_i
+0000bfa0: 643a 0a20 2020 2020 2020 2070 6179 6c6f  d:.        paylo
+0000bfb0: 6164 5b22 696e 6c69 6e65 5f6d 6573 7361  ad["inline_messa
+0000bfc0: 6765 5f69 6422 5d20 3d20 696e 6c69 6e65  ge_id"] = inline
+0000bfd0: 5f6d 6573 7361 6765 5f69 640a 2020 2020  _message_id.    
+0000bfe0: 6966 2070 6172 7365 5f6d 6f64 653a 0a20  if parse_mode:. 
+0000bff0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+0000c000: 7061 7273 655f 6d6f 6465 225d 203d 2070  parse_mode"] = p
+0000c010: 6172 7365 5f6d 6f64 650a 2020 2020 6966  arse_mode.    if
+0000c020: 2063 6170 7469 6f6e 5f65 6e74 6974 6965   caption_entitie
+0000c030: 733a 0a20 2020 2020 2020 2070 6179 6c6f  s:.        paylo
+0000c040: 6164 5b22 6361 7074 696f 6e5f 656e 7469  ad["caption_enti
+0000c050: 7469 6573 225d 203d 206a 736f 6e2e 6475  ties"] = json.du
+0000c060: 6d70 7328 7479 7065 732e 4d65 7373 6167  mps(types.Messag
+0000c070: 6545 6e74 6974 792e 746f 5f6c 6973 745f  eEntity.to_list_
+0000c080: 6f66 5f64 6963 7473 2863 6170 7469 6f6e  of_dicts(caption
+0000c090: 5f65 6e74 6974 6965 7329 290a 2020 2020  _entities)).    
+0000c0a0: 6966 2072 6570 6c79 5f6d 6172 6b75 703a  if reply_markup:
+0000c0b0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+0000c0c0: 5b22 7265 706c 795f 6d61 726b 7570 225d  ["reply_markup"]
+0000c0d0: 203d 2061 7761 6974 205f 636f 6e76 6572   = await _conver
+0000c0e0: 745f 6d61 726b 7570 2872 6570 6c79 5f6d  t_markup(reply_m
+0000c0f0: 6172 6b75 7029 0a20 2020 2072 6574 7572  arkup).    retur
+0000c100: 6e20 6177 6169 7420 5f72 6571 7565 7374  n await _request
+0000c110: 2874 6f6b 656e 2c20 6d65 7468 6f64 5f75  (token, method_u
+0000c120: 726c 2c20 7061 7261 6d73 3d70 6179 6c6f  rl, params=paylo
+0000c130: 6164 2c20 6d65 7468 6f64 3d22 706f 7374  ad, method="post
+0000c140: 2229 0a0a 0a61 7379 6e63 2064 6566 2065  ")...async def e
+0000c150: 6469 745f 6d65 7373 6167 655f 6d65 6469  dit_message_medi
+0000c160: 6128 0a20 2020 2074 6f6b 656e 2c0a 2020  a(.    token,.  
+0000c170: 2020 6d65 6469 612c 0a20 2020 2063 6861    media,.    cha
+0000c180: 745f 6964 3d4e 6f6e 652c 0a20 2020 206d  t_id=None,.    m
+0000c190: 6573 7361 6765 5f69 643d 4e6f 6e65 2c0a  essage_id=None,.
+0000c1a0: 2020 2020 696e 6c69 6e65 5f6d 6573 7361      inline_messa
+0000c1b0: 6765 5f69 643d 4e6f 6e65 2c0a 2020 2020  ge_id=None,.    
+0000c1c0: 7265 706c 795f 6d61 726b 7570 3d4e 6f6e  reply_markup=Non
+0000c1d0: 652c 0a29 3a0a 2020 2020 6d65 7468 6f64  e,.):.    method
+0000c1e0: 5f75 726c 203d 2072 2265 6469 744d 6573  _url = r"editMes
+0000c1f0: 7361 6765 4d65 6469 6122 0a20 2020 206d  sageMedia".    m
+0000c200: 6564 6961 5f6a 736f 6e2c 2066 696c 6520  edia_json, file 
+0000c210: 3d20 6177 6169 7420 636f 6e76 6572 745f  = await convert_
+0000c220: 696e 7075 745f 6d65 6469 6128 6d65 6469  input_media(medi
+0000c230: 6129 0a20 2020 2070 6179 6c6f 6164 203d  a).    payload =
+0000c240: 207b 226d 6564 6961 223a 206d 6564 6961   {"media": media
+0000c250: 5f6a 736f 6e7d 0a20 2020 2069 6620 6368  _json}.    if ch
+0000c260: 6174 5f69 643a 0a20 2020 2020 2020 2070  at_id:.        p
+0000c270: 6179 6c6f 6164 5b22 6368 6174 5f69 6422  ayload["chat_id"
+0000c280: 5d20 3d20 6368 6174 5f69 640a 2020 2020  ] = chat_id.    
+0000c290: 6966 206d 6573 7361 6765 5f69 643a 0a20  if message_id:. 
+0000c2a0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+0000c2b0: 6d65 7373 6167 655f 6964 225d 203d 206d  message_id"] = m
+0000c2c0: 6573 7361 6765 5f69 640a 2020 2020 6966  essage_id.    if
+0000c2d0: 2069 6e6c 696e 655f 6d65 7373 6167 655f   inline_message_
+0000c2e0: 6964 3a0a 2020 2020 2020 2020 7061 796c  id:.        payl
+0000c2f0: 6f61 645b 2269 6e6c 696e 655f 6d65 7373  oad["inline_mess
+0000c300: 6167 655f 6964 225d 203d 2069 6e6c 696e  age_id"] = inlin
+0000c310: 655f 6d65 7373 6167 655f 6964 0a20 2020  e_message_id.   
+0000c320: 2069 6620 7265 706c 795f 6d61 726b 7570   if reply_markup
+0000c330: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+0000c340: 645b 2272 6570 6c79 5f6d 6172 6b75 7022  d["reply_markup"
+0000c350: 5d20 3d20 6177 6169 7420 5f63 6f6e 7665  ] = await _conve
+0000c360: 7274 5f6d 6172 6b75 7028 7265 706c 795f  rt_markup(reply_
+0000c370: 6d61 726b 7570 290a 2020 2020 7265 7475  markup).    retu
+0000c380: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
+0000c390: 7428 746f 6b65 6e2c 206d 6574 686f 645f  t(token, method_
+0000c3a0: 7572 6c2c 2070 6172 616d 733d 7061 796c  url, params=payl
+0000c3b0: 6f61 642c 2066 696c 6573 3d66 696c 652c  oad, files=file,
+0000c3c0: 206d 6574 686f 643d 2270 6f73 7422 2069   method="post" i
+0000c3d0: 6620 6669 6c65 2065 6c73 6520 2267 6574  f file else "get
+0000c3e0: 2229 0a0a 0a61 7379 6e63 2064 6566 2065  ")...async def e
+0000c3f0: 6469 745f 6d65 7373 6167 655f 7265 706c  dit_message_repl
+0000c400: 795f 6d61 726b 7570 2874 6f6b 656e 2c20  y_markup(token, 
+0000c410: 6368 6174 5f69 643d 4e6f 6e65 2c20 6d65  chat_id=None, me
+0000c420: 7373 6167 655f 6964 3d4e 6f6e 652c 2069  ssage_id=None, i
+0000c430: 6e6c 696e 655f 6d65 7373 6167 655f 6964  nline_message_id
+0000c440: 3d4e 6f6e 652c 2072 6570 6c79 5f6d 6172  =None, reply_mar
+0000c450: 6b75 703d 4e6f 6e65 293a 0a20 2020 206d  kup=None):.    m
+0000c460: 6574 686f 645f 7572 6c20 3d20 7222 6564  ethod_url = r"ed
+0000c470: 6974 4d65 7373 6167 6552 6570 6c79 4d61  itMessageReplyMa
+0000c480: 726b 7570 220a 2020 2020 7061 796c 6f61  rkup".    payloa
+0000c490: 6420 3d20 7b7d 0a20 2020 2069 6620 6368  d = {}.    if ch
+0000c4a0: 6174 5f69 643a 0a20 2020 2020 2020 2070  at_id:.        p
+0000c4b0: 6179 6c6f 6164 5b22 6368 6174 5f69 6422  ayload["chat_id"
+0000c4c0: 5d20 3d20 6368 6174 5f69 640a 2020 2020  ] = chat_id.    
+0000c4d0: 6966 206d 6573 7361 6765 5f69 643a 0a20  if message_id:. 
+0000c4e0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+0000c4f0: 6d65 7373 6167 655f 6964 225d 203d 206d  message_id"] = m
+0000c500: 6573 7361 6765 5f69 640a 2020 2020 6966  essage_id.    if
+0000c510: 2069 6e6c 696e 655f 6d65 7373 6167 655f   inline_message_
+0000c520: 6964 3a0a 2020 2020 2020 2020 7061 796c  id:.        payl
+0000c530: 6f61 645b 2269 6e6c 696e 655f 6d65 7373  oad["inline_mess
+0000c540: 6167 655f 6964 225d 203d 2069 6e6c 696e  age_id"] = inlin
+0000c550: 655f 6d65 7373 6167 655f 6964 0a20 2020  e_message_id.   
+0000c560: 2069 6620 7265 706c 795f 6d61 726b 7570   if reply_markup
+0000c570: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+0000c580: 645b 2272 6570 6c79 5f6d 6172 6b75 7022  d["reply_markup"
+0000c590: 5d20 3d20 6177 6169 7420 5f63 6f6e 7665  ] = await _conve
+0000c5a0: 7274 5f6d 6172 6b75 7028 7265 706c 795f  rt_markup(reply_
+0000c5b0: 6d61 726b 7570 290a 2020 2020 7265 7475  markup).    retu
+0000c5c0: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
+0000c5d0: 7428 746f 6b65 6e2c 206d 6574 686f 645f  t(token, method_
+0000c5e0: 7572 6c2c 2070 6172 616d 733d 7061 796c  url, params=payl
+0000c5f0: 6f61 642c 206d 6574 686f 643d 2270 6f73  oad, method="pos
+0000c600: 7422 290a 0a0a 6173 796e 6320 6465 6620  t")...async def 
+0000c610: 6465 6c65 7465 5f6d 6573 7361 6765 2874  delete_message(t
+0000c620: 6f6b 656e 2c20 6368 6174 5f69 642c 206d  oken, chat_id, m
+0000c630: 6573 7361 6765 5f69 642c 2074 696d 656f  essage_id, timeo
+0000c640: 7574 3d4e 6f6e 6529 3a0a 2020 2020 6d65  ut=None):.    me
+0000c650: 7468 6f64 5f75 726c 203d 2072 2264 656c  thod_url = r"del
+0000c660: 6574 654d 6573 7361 6765 220a 2020 2020  eteMessage".    
+0000c670: 7061 796c 6f61 6420 3d20 7b22 6368 6174  payload = {"chat
+0000c680: 5f69 6422 3a20 6368 6174 5f69 642c 2022  _id": chat_id, "
+0000c690: 6d65 7373 6167 655f 6964 223a 206d 6573  message_id": mes
+0000c6a0: 7361 6765 5f69 647d 0a20 2020 2069 6620  sage_id}.    if 
+0000c6b0: 7469 6d65 6f75 743a 0a20 2020 2020 2020  timeout:.       
+0000c6c0: 2070 6179 6c6f 6164 5b22 7469 6d65 6f75   payload["timeou
+0000c6d0: 7422 5d20 3d20 7469 6d65 6f75 740a 2020  t"] = timeout.  
+0000c6e0: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
+0000c6f0: 7265 7175 6573 7428 746f 6b65 6e2c 206d  request(token, m
+0000c700: 6574 686f 645f 7572 6c2c 2070 6172 616d  ethod_url, param
+0000c710: 733d 7061 796c 6f61 642c 206d 6574 686f  s=payload, metho
+0000c720: 643d 2270 6f73 7422 290a 0a0a 2320 4761  d="post")...# Ga
+0000c730: 6d65 0a0a 0a61 7379 6e63 2064 6566 2073  me...async def s
+0000c740: 656e 645f 6761 6d65 280a 2020 2020 746f  end_game(.    to
+0000c750: 6b65 6e2c 0a20 2020 2063 6861 745f 6964  ken,.    chat_id
+0000c760: 2c0a 2020 2020 6761 6d65 5f73 686f 7274  ,.    game_short
+0000c770: 5f6e 616d 652c 0a20 2020 2064 6973 6162  _name,.    disab
+0000c780: 6c65 5f6e 6f74 6966 6963 6174 696f 6e3d  le_notification=
+0000c790: 4e6f 6e65 2c0a 2020 2020 7265 706c 795f  None,.    reply_
+0000c7a0: 746f 5f6d 6573 7361 6765 5f69 643d 4e6f  to_message_id=No
+0000c7b0: 6e65 2c0a 2020 2020 7265 706c 795f 6d61  ne,.    reply_ma
+0000c7c0: 726b 7570 3d4e 6f6e 652c 0a20 2020 2074  rkup=None,.    t
+0000c7d0: 696d 656f 7574 3d4e 6f6e 652c 0a20 2020  imeout=None,.   
+0000c7e0: 2061 6c6c 6f77 5f73 656e 6469 6e67 5f77   allow_sending_w
+0000c7f0: 6974 686f 7574 5f72 6570 6c79 3d4e 6f6e  ithout_reply=Non
+0000c800: 652c 0a20 2020 2070 726f 7465 6374 5f63  e,.    protect_c
+0000c810: 6f6e 7465 6e74 3d4e 6f6e 652c 0a20 2020  ontent=None,.   
+0000c820: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
+0000c830: 6964 3a20 4f70 7469 6f6e 616c 5b69 6e74  id: Optional[int
+0000c840: 5d20 3d20 4e6f 6e65 2c0a 293a 0a20 2020  ] = None,.):.   
+0000c850: 206d 6574 686f 645f 7572 6c20 3d20 7222   method_url = r"
+0000c860: 7365 6e64 4761 6d65 220a 2020 2020 7061  sendGame".    pa
+0000c870: 796c 6f61 6420 3d20 7b22 6368 6174 5f69  yload = {"chat_i
+0000c880: 6422 3a20 6368 6174 5f69 642c 2022 6761  d": chat_id, "ga
+0000c890: 6d65 5f73 686f 7274 5f6e 616d 6522 3a20  me_short_name": 
+0000c8a0: 6761 6d65 5f73 686f 7274 5f6e 616d 657d  game_short_name}
+0000c8b0: 0a20 2020 2069 6620 6469 7361 626c 655f  .    if disable_
+0000c8c0: 6e6f 7469 6669 6361 7469 6f6e 2069 7320  notification is 
+0000c8d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000c8e0: 2020 7061 796c 6f61 645b 2264 6973 6162    payload["disab
+0000c8f0: 6c65 5f6e 6f74 6966 6963 6174 696f 6e22  le_notification"
+0000c900: 5d20 3d20 6469 7361 626c 655f 6e6f 7469  ] = disable_noti
+0000c910: 6669 6361 7469 6f6e 0a20 2020 2069 6620  fication.    if 
+0000c920: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+0000c930: 5f69 643a 0a20 2020 2020 2020 2070 6179  _id:.        pay
+0000c940: 6c6f 6164 5b22 7265 706c 795f 746f 5f6d  load["reply_to_m
+0000c950: 6573 7361 6765 5f69 6422 5d20 3d20 7265  essage_id"] = re
+0000c960: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
+0000c970: 640a 2020 2020 6966 2072 6570 6c79 5f6d  d.    if reply_m
+0000c980: 6172 6b75 703a 0a20 2020 2020 2020 2070  arkup:.        p
+0000c990: 6179 6c6f 6164 5b22 7265 706c 795f 6d61  ayload["reply_ma
+0000c9a0: 726b 7570 225d 203d 2061 7761 6974 205f  rkup"] = await _
+0000c9b0: 636f 6e76 6572 745f 6d61 726b 7570 2872  convert_markup(r
+0000c9c0: 6570 6c79 5f6d 6172 6b75 7029 0a20 2020  eply_markup).   
+0000c9d0: 2069 6620 7469 6d65 6f75 743a 0a20 2020   if timeout:.   
+0000c9e0: 2020 2020 2070 6179 6c6f 6164 5b22 7469       payload["ti
+0000c9f0: 6d65 6f75 7422 5d20 3d20 7469 6d65 6f75  meout"] = timeou
+0000ca00: 740a 2020 2020 6966 2061 6c6c 6f77 5f73  t.    if allow_s
+0000ca10: 656e 6469 6e67 5f77 6974 686f 7574 5f72  ending_without_r
+0000ca20: 6570 6c79 2069 7320 6e6f 7420 4e6f 6e65  eply is not None
+0000ca30: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+0000ca40: 645b 2261 6c6c 6f77 5f73 656e 6469 6e67  d["allow_sending
+0000ca50: 5f77 6974 686f 7574 5f72 6570 6c79 225d  _without_reply"]
+0000ca60: 203d 2061 6c6c 6f77 5f73 656e 6469 6e67   = allow_sending
+0000ca70: 5f77 6974 686f 7574 5f72 6570 6c79 0a20  _without_reply. 
+0000ca80: 2020 2069 6620 7072 6f74 6563 745f 636f     if protect_co
+0000ca90: 6e74 656e 7420 6973 206e 6f74 204e 6f6e  ntent is not Non
+0000caa0: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
+0000cab0: 6164 5b22 7072 6f74 6563 745f 636f 6e74  ad["protect_cont
+0000cac0: 656e 7422 5d20 3d20 7072 6f74 6563 745f  ent"] = protect_
+0000cad0: 636f 6e74 656e 740a 2020 2020 5f61 6464  content.    _add
+0000cae0: 5f6d 6573 7361 6765 5f74 6872 6561 645f  _message_thread_
+0000caf0: 6964 2870 6179 6c6f 6164 2c20 6d65 7373  id(payload, mess
+0000cb00: 6167 655f 7468 7265 6164 5f69 6429 0a20  age_thread_id). 
+0000cb10: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+0000cb20: 5f72 6571 7565 7374 2874 6f6b 656e 2c20  _request(token, 
+0000cb30: 6d65 7468 6f64 5f75 726c 2c20 7061 7261  method_url, para
+0000cb40: 6d73 3d70 6179 6c6f 6164 290a 0a0a 2320  ms=payload)...# 
+0000cb50: 6874 7470 733a 2f2f 636f 7265 2e74 656c  https://core.tel
+0000cb60: 6567 7261 6d2e 6f72 672f 626f 7473 2f61  egram.org/bots/a
+0000cb70: 7069 2373 6574 6761 6d65 7363 6f72 650a  pi#setgamescore.
+0000cb80: 6173 796e 6320 6465 6620 7365 745f 6761  async def set_ga
+0000cb90: 6d65 5f73 636f 7265 280a 2020 2020 746f  me_score(.    to
+0000cba0: 6b65 6e2c 0a20 2020 2075 7365 725f 6964  ken,.    user_id
+0000cbb0: 2c0a 2020 2020 7363 6f72 652c 0a20 2020  ,.    score,.   
+0000cbc0: 2066 6f72 6365 3d4e 6f6e 652c 0a20 2020   force=None,.   
+0000cbd0: 2064 6973 6162 6c65 5f65 6469 745f 6d65   disable_edit_me
+0000cbe0: 7373 6167 653d 4e6f 6e65 2c0a 2020 2020  ssage=None,.    
+0000cbf0: 6368 6174 5f69 643d 4e6f 6e65 2c0a 2020  chat_id=None,.  
+0000cc00: 2020 6d65 7373 6167 655f 6964 3d4e 6f6e    message_id=Non
+0000cc10: 652c 0a20 2020 2069 6e6c 696e 655f 6d65  e,.    inline_me
+0000cc20: 7373 6167 655f 6964 3d4e 6f6e 652c 0a29  ssage_id=None,.)
+0000cc30: 3a0a 2020 2020 2222 220a 2020 2020 5573  :.    """.    Us
+0000cc40: 6520 7468 6973 206d 6574 686f 6420 746f  e this method to
+0000cc50: 2073 6574 2074 6865 2073 636f 7265 206f   set the score o
+0000cc60: 6620 7468 6520 7370 6563 6966 6965 6420  f the specified 
+0000cc70: 7573 6572 2069 6e20 6120 6761 6d65 2e20  user in a game. 
+0000cc80: 4f6e 2073 7563 6365 7373 2c20 6966 2074  On success, if t
+0000cc90: 6865 206d 6573 7361 6765 2077 6173 2073  he message was s
+0000cca0: 656e 7420 6279 2074 6865 2062 6f74 2c20  ent by the bot, 
+0000ccb0: 7265 7475 726e 7320 7468 6520 6564 6974  returns the edit
+0000ccc0: 6564 204d 6573 7361 6765 2c20 6f74 6865  ed Message, othe
+0000ccd0: 7277 6973 6520 7265 7475 726e 7320 5472  rwise returns Tr
+0000cce0: 7565 2e20 5265 7475 726e 7320 616e 2065  ue. Returns an e
+0000ccf0: 7272 6f72 2c20 6966 2074 6865 206e 6577  rror, if the new
+0000cd00: 2073 636f 7265 2069 7320 6e6f 7420 6772   score is not gr
+0000cd10: 6561 7465 7220 7468 616e 2074 6865 2075  eater than the u
+0000cd20: 7365 7227 7320 6375 7272 656e 7420 7363  ser's current sc
+0000cd30: 6f72 6520 696e 2074 6865 2063 6861 742e  ore in the chat.
+0000cd40: 0a20 2020 203a 7061 7261 6d20 746f 6b65  .    :param toke
+0000cd50: 6e3a 2042 6f74 2773 2074 6f6b 656e 2028  n: Bot's token (
+0000cd60: 796f 7520 646f 6e27 7420 6e65 6564 2074  you don't need t
+0000cd70: 6f20 6669 6c6c 2074 6869 7329 0a20 2020  o fill this).   
+0000cd80: 203a 7061 7261 6d20 7573 6572 5f69 643a   :param user_id:
+0000cd90: 2055 7365 7220 6964 656e 7469 6669 6572   User identifier
+0000cda0: 0a20 2020 203a 7061 7261 6d20 7363 6f72  .    :param scor
+0000cdb0: 653a 204e 6577 2073 636f 7265 2c20 6d75  e: New score, mu
+0000cdc0: 7374 2062 6520 6e6f 6e2d 6e65 6761 7469  st be non-negati
+0000cdd0: 7665 0a20 2020 203a 7061 7261 6d20 666f  ve.    :param fo
+0000cde0: 7263 653a 2028 4f70 7469 6f6e 616c 2920  rce: (Optional) 
+0000cdf0: 5061 7373 2054 7275 652c 2069 6620 7468  Pass True, if th
+0000ce00: 6520 6869 6768 2073 636f 7265 2069 7320  e high score is 
+0000ce10: 616c 6c6f 7765 6420 746f 2064 6563 7265  allowed to decre
+0000ce20: 6173 652e 2054 6869 7320 6361 6e20 6265  ase. This can be
+0000ce30: 2075 7365 6675 6c20 7768 656e 2066 6978   useful when fix
+0000ce40: 696e 6720 6d69 7374 616b 6573 206f 7220  ing mistakes or 
+0000ce50: 6261 6e6e 696e 6720 6368 6561 7465 7273  banning cheaters
+0000ce60: 0a20 2020 203a 7061 7261 6d20 6469 7361  .    :param disa
+0000ce70: 626c 655f 6564 6974 5f6d 6573 7361 6765  ble_edit_message
+0000ce80: 3a20 284f 7074 696f 6e61 6c29 2050 6173  : (Optional) Pas
+0000ce90: 7320 5472 7565 2c20 6966 2074 6865 2067  s True, if the g
+0000cea0: 616d 6520 6d65 7373 6167 6520 7368 6f75  ame message shou
+0000ceb0: 6c64 206e 6f74 2062 6520 6175 746f 6d61  ld not be automa
+0000cec0: 7469 6361 6c6c 7920 6564 6974 6564 2074  tically edited t
+0000ced0: 6f20 696e 636c 7564 6520 7468 6520 6375  o include the cu
+0000cee0: 7272 656e 7420 7363 6f72 6562 6f61 7264  rrent scoreboard
+0000cef0: 0a20 2020 203a 7061 7261 6d20 6368 6174  .    :param chat
+0000cf00: 5f69 643a 2028 4f70 7469 6f6e 616c 2c20  _id: (Optional, 
+0000cf10: 7265 7175 6972 6564 2069 6620 696e 6c69  required if inli
+0000cf20: 6e65 5f6d 6573 7361 6765 5f69 6420 6973  ne_message_id is
+0000cf30: 206e 6f74 2073 7065 6369 6669 6564 2920   not specified) 
+0000cf40: 556e 6971 7565 2069 6465 6e74 6966 6965  Unique identifie
+0000cf50: 7220 666f 7220 7468 6520 7461 7267 6574  r for the target
+0000cf60: 2063 6861 7420 286f 7220 7573 6572 6e61   chat (or userna
+0000cf70: 6d65 206f 6620 7468 6520 7461 7267 6574  me of the target
+0000cf80: 2063 6861 6e6e 656c 2069 6e20 7468 6520   channel in the 
+0000cf90: 666f 726d 6174 2040 6368 616e 6e65 6c75  format @channelu
+0000cfa0: 7365 726e 616d 6529 0a20 2020 203a 7061  sername).    :pa
+0000cfb0: 7261 6d20 6d65 7373 6167 655f 6964 3a20  ram message_id: 
+0000cfc0: 284f 7074 696f 6e61 6c2c 2072 6571 7569  (Optional, requi
+0000cfd0: 7265 6420 6966 2069 6e6c 696e 655f 6d65  red if inline_me
+0000cfe0: 7373 6167 655f 6964 2069 7320 6e6f 7420  ssage_id is not 
+0000cff0: 7370 6563 6966 6965 6429 2055 6e69 7175  specified) Uniqu
+0000d000: 6520 6964 656e 7469 6669 6572 206f 6620  e identifier of 
+0000d010: 7468 6520 7365 6e74 206d 6573 7361 6765  the sent message
+0000d020: 0a20 2020 203a 7061 7261 6d20 696e 6c69  .    :param inli
+0000d030: 6e65 5f6d 6573 7361 6765 5f69 643a 2028  ne_message_id: (
+0000d040: 4f70 7469 6f6e 616c 2c20 7265 7175 6972  Optional, requir
+0000d050: 6564 2069 6620 6368 6174 5f69 6420 616e  ed if chat_id an
+0000d060: 6420 6d65 7373 6167 655f 6964 2061 7265  d message_id are
+0000d070: 206e 6f74 2073 7065 6369 6669 6564 2920   not specified) 
+0000d080: 4964 656e 7469 6669 6572 206f 6620 7468  Identifier of th
+0000d090: 6520 696e 6c69 6e65 206d 6573 7361 6765  e inline message
+0000d0a0: 0a20 2020 203a 7265 7475 726e 3a0a 2020  .    :return:.  
+0000d0b0: 2020 2222 220a 2020 2020 6d65 7468 6f64    """.    method
+0000d0c0: 5f75 726c 203d 2072 2273 6574 4761 6d65  _url = r"setGame
+0000d0d0: 5363 6f72 6522 0a20 2020 2070 6179 6c6f  Score".    paylo
+0000d0e0: 6164 203d 207b 2275 7365 725f 6964 223a  ad = {"user_id":
+0000d0f0: 2075 7365 725f 6964 2c20 2273 636f 7265   user_id, "score
+0000d100: 223a 2073 636f 7265 7d0a 2020 2020 6966  ": score}.    if
+0000d110: 2066 6f72 6365 2069 7320 6e6f 7420 4e6f   force is not No
+0000d120: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
+0000d130: 6f61 645b 2266 6f72 6365 225d 203d 2066  oad["force"] = f
+0000d140: 6f72 6365 0a20 2020 2069 6620 6368 6174  orce.    if chat
+0000d150: 5f69 643a 0a20 2020 2020 2020 2070 6179  _id:.        pay
+0000d160: 6c6f 6164 5b22 6368 6174 5f69 6422 5d20  load["chat_id"] 
+0000d170: 3d20 6368 6174 5f69 640a 2020 2020 6966  = chat_id.    if
+0000d180: 206d 6573 7361 6765 5f69 643a 0a20 2020   message_id:.   
+0000d190: 2020 2020 2070 6179 6c6f 6164 5b22 6d65       payload["me
+0000d1a0: 7373 6167 655f 6964 225d 203d 206d 6573  ssage_id"] = mes
+0000d1b0: 7361 6765 5f69 640a 2020 2020 6966 2069  sage_id.    if i
+0000d1c0: 6e6c 696e 655f 6d65 7373 6167 655f 6964  nline_message_id
+0000d1d0: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+0000d1e0: 645b 2269 6e6c 696e 655f 6d65 7373 6167  d["inline_messag
+0000d1f0: 655f 6964 225d 203d 2069 6e6c 696e 655f  e_id"] = inline_
+0000d200: 6d65 7373 6167 655f 6964 0a20 2020 2069  message_id.    i
+0000d210: 6620 6469 7361 626c 655f 6564 6974 5f6d  f disable_edit_m
+0000d220: 6573 7361 6765 2069 7320 6e6f 7420 4e6f  essage is not No
+0000d230: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
+0000d240: 6f61 645b 2264 6973 6162 6c65 5f65 6469  oad["disable_edi
+0000d250: 745f 6d65 7373 6167 6522 5d20 3d20 6469  t_message"] = di
+0000d260: 7361 626c 655f 6564 6974 5f6d 6573 7361  sable_edit_messa
+0000d270: 6765 0a20 2020 2072 6574 7572 6e20 6177  ge.    return aw
+0000d280: 6169 7420 5f72 6571 7565 7374 2874 6f6b  ait _request(tok
+0000d290: 656e 2c20 6d65 7468 6f64 5f75 726c 2c20  en, method_url, 
+0000d2a0: 7061 7261 6d73 3d70 6179 6c6f 6164 290a  params=payload).
+0000d2b0: 0a0a 2320 6874 7470 733a 2f2f 636f 7265  ..# https://core
+0000d2c0: 2e74 656c 6567 7261 6d2e 6f72 672f 626f  .telegram.org/bo
+0000d2d0: 7473 2f61 7069 2367 6574 6761 6d65 6869  ts/api#getgamehi
+0000d2e0: 6768 7363 6f72 6573 0a61 7379 6e63 2064  ghscores.async d
+0000d2f0: 6566 2067 6574 5f67 616d 655f 6869 6768  ef get_game_high
+0000d300: 5f73 636f 7265 7328 746f 6b65 6e2c 2075  _scores(token, u
+0000d310: 7365 725f 6964 2c20 6368 6174 5f69 643d  ser_id, chat_id=
+0000d320: 4e6f 6e65 2c20 6d65 7373 6167 655f 6964  None, message_id
+0000d330: 3d4e 6f6e 652c 2069 6e6c 696e 655f 6d65  =None, inline_me
+0000d340: 7373 6167 655f 6964 3d4e 6f6e 6529 3a0a  ssage_id=None):.
+0000d350: 2020 2020 2222 220a 2020 2020 5573 6520      """.    Use 
+0000d360: 7468 6973 206d 6574 686f 6420 746f 2067  this method to g
+0000d370: 6574 2064 6174 6120 666f 7220 6869 6768  et data for high
+0000d380: 2073 636f 7265 2074 6162 6c65 732e 2057   score tables. W
+0000d390: 696c 6c20 7265 7475 726e 2074 6865 2073  ill return the s
+0000d3a0: 636f 7265 206f 6620 7468 6520 7370 6563  core of the spec
+0000d3b0: 6966 6965 6420 7573 6572 2061 6e64 2073  ified user and s
+0000d3c0: 6576 6572 616c 206f 6620 6869 7320 6e65  everal of his ne
+0000d3d0: 6967 6862 6f72 7320 696e 2061 2067 616d  ighbors in a gam
+0000d3e0: 652e 204f 6e20 7375 6363 6573 732c 2072  e. On success, r
+0000d3f0: 6574 7572 6e73 2061 6e20 4172 7261 7920  eturns an Array 
+0000d400: 6f66 2047 616d 6548 6967 6853 636f 7265  of GameHighScore
+0000d410: 206f 626a 6563 7473 2e0a 2020 2020 5468   objects..    Th
+0000d420: 6973 206d 6574 686f 6420 7769 6c6c 2063  is method will c
+0000d430: 7572 7265 6e74 6c79 2072 6574 7572 6e20  urrently return 
+0000d440: 7363 6f72 6573 2066 6f72 2074 6865 2074  scores for the t
+0000d450: 6172 6765 7420 7573 6572 2c20 706c 7573  arget user, plus
+0000d460: 2074 776f 206f 6620 6869 7320 636c 6f73   two of his clos
+0000d470: 6573 7420 6e65 6967 6862 6f72 7320 6f6e  est neighbors on
+0000d480: 2065 6163 6820 7369 6465 2e20 5769 6c6c   each side. Will
+0000d490: 2061 6c73 6f20 7265 7475 726e 2074 6865   also return the
+0000d4a0: 2074 6f70 2074 6872 6565 2075 7365 7273   top three users
+0000d4b0: 2069 6620 7468 6520 7573 6572 2061 6e64   if the user and
+0000d4c0: 2068 6973 206e 6569 6768 626f 7273 2061   his neighbors a
+0000d4d0: 7265 206e 6f74 2061 6d6f 6e67 2074 6865  re not among the
+0000d4e0: 6d2e 2050 6c65 6173 6520 6e6f 7465 2074  m. Please note t
+0000d4f0: 6861 7420 7468 6973 2062 6568 6176 696f  hat this behavio
+0000d500: 7220 6973 2073 7562 6a65 6374 2074 6f20  r is subject to 
+0000d510: 6368 616e 6765 2e0a 2020 2020 3a70 6172  change..    :par
+0000d520: 616d 2074 6f6b 656e 3a20 426f 7427 7320  am token: Bot's 
+0000d530: 746f 6b65 6e20 2879 6f75 2064 6f6e 2774  token (you don't
+0000d540: 206e 6565 6420 746f 2066 696c 6c20 7468   need to fill th
+0000d550: 6973 290a 2020 2020 3a70 6172 616d 2075  is).    :param u
+0000d560: 7365 725f 6964 3a20 5461 7267 6574 2075  ser_id: Target u
+0000d570: 7365 7220 6964 0a20 2020 203a 7061 7261  ser id.    :para
+0000d580: 6d20 6368 6174 5f69 643a 2028 4f70 7469  m chat_id: (Opti
+0000d590: 6f6e 616c 2c20 7265 7175 6972 6564 2069  onal, required i
+0000d5a0: 6620 696e 6c69 6e65 5f6d 6573 7361 6765  f inline_message
+0000d5b0: 5f69 6420 6973 206e 6f74 2073 7065 6369  _id is not speci
+0000d5c0: 6669 6564 2920 556e 6971 7565 2069 6465  fied) Unique ide
+0000d5d0: 6e74 6966 6965 7220 666f 7220 7468 6520  ntifier for the 
+0000d5e0: 7461 7267 6574 2063 6861 7420 286f 7220  target chat (or 
+0000d5f0: 7573 6572 6e61 6d65 206f 6620 7468 6520  username of the 
+0000d600: 7461 7267 6574 2063 6861 6e6e 656c 2069  target channel i
+0000d610: 6e20 7468 6520 666f 726d 6174 2040 6368  n the format @ch
+0000d620: 616e 6e65 6c75 7365 726e 616d 6529 0a20  annelusername). 
+0000d630: 2020 203a 7061 7261 6d20 6d65 7373 6167     :param messag
+0000d640: 655f 6964 3a20 284f 7074 696f 6e61 6c2c  e_id: (Optional,
+0000d650: 2072 6571 7569 7265 6420 6966 2069 6e6c   required if inl
+0000d660: 696e 655f 6d65 7373 6167 655f 6964 2069  ine_message_id i
+0000d670: 7320 6e6f 7420 7370 6563 6966 6965 6429  s not specified)
+0000d680: 2055 6e69 7175 6520 6964 656e 7469 6669   Unique identifi
+0000d690: 6572 206f 6620 7468 6520 7365 6e74 206d  er of the sent m
+0000d6a0: 6573 7361 6765 0a20 2020 203a 7061 7261  essage.    :para
+0000d6b0: 6d20 696e 6c69 6e65 5f6d 6573 7361 6765  m inline_message
+0000d6c0: 5f69 643a 2028 4f70 7469 6f6e 616c 2c20  _id: (Optional, 
+0000d6d0: 7265 7175 6972 6564 2069 6620 6368 6174  required if chat
+0000d6e0: 5f69 6420 616e 6420 6d65 7373 6167 655f  _id and message_
+0000d6f0: 6964 2061 7265 206e 6f74 2073 7065 6369  id are not speci
+0000d700: 6669 6564 2920 4964 656e 7469 6669 6572  fied) Identifier
+0000d710: 206f 6620 7468 6520 696e 6c69 6e65 206d   of the inline m
+0000d720: 6573 7361 6765 0a20 2020 203a 7265 7475  essage.    :retu
+0000d730: 726e 3a0a 2020 2020 2222 220a 2020 2020  rn:.    """.    
+0000d740: 6d65 7468 6f64 5f75 726c 203d 2072 2267  method_url = r"g
+0000d750: 6574 4761 6d65 4869 6768 5363 6f72 6573  etGameHighScores
+0000d760: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
+0000d770: 7b22 7573 6572 5f69 6422 3a20 7573 6572  {"user_id": user
+0000d780: 5f69 647d 0a20 2020 2069 6620 6368 6174  _id}.    if chat
+0000d790: 5f69 643a 0a20 2020 2020 2020 2070 6179  _id:.        pay
+0000d7a0: 6c6f 6164 5b22 6368 6174 5f69 6422 5d20  load["chat_id"] 
+0000d7b0: 3d20 6368 6174 5f69 640a 2020 2020 6966  = chat_id.    if
+0000d7c0: 206d 6573 7361 6765 5f69 643a 0a20 2020   message_id:.   
+0000d7d0: 2020 2020 2070 6179 6c6f 6164 5b22 6d65       payload["me
+0000d7e0: 7373 6167 655f 6964 225d 203d 206d 6573  ssage_id"] = mes
+0000d7f0: 7361 6765 5f69 640a 2020 2020 6966 2069  sage_id.    if i
+0000d800: 6e6c 696e 655f 6d65 7373 6167 655f 6964  nline_message_id
+0000d810: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+0000d820: 645b 2269 6e6c 696e 655f 6d65 7373 6167  d["inline_messag
+0000d830: 655f 6964 225d 203d 2069 6e6c 696e 655f  e_id"] = inline_
+0000d840: 6d65 7373 6167 655f 6964 0a20 2020 2072  message_id.    r
+0000d850: 6574 7572 6e20 6177 6169 7420 5f72 6571  eturn await _req
+0000d860: 7565 7374 2874 6f6b 656e 2c20 6d65 7468  uest(token, meth
+0000d870: 6f64 5f75 726c 2c20 7061 7261 6d73 3d70  od_url, params=p
+0000d880: 6179 6c6f 6164 290a 0a0a 2320 5061 796d  ayload)...# Paym
+0000d890: 656e 7473 2028 6874 7470 733a 2f2f 636f  ents (https://co
+0000d8a0: 7265 2e74 656c 6567 7261 6d2e 6f72 672f  re.telegram.org/
+0000d8b0: 626f 7473 2f61 7069 2370 6179 6d65 6e74  bots/api#payment
+0000d8c0: 7329 0a0a 0a61 7379 6e63 2064 6566 2073  s)...async def s
+0000d8d0: 656e 645f 696e 766f 6963 6528 0a20 2020  end_invoice(.   
+0000d8e0: 2074 6f6b 656e 2c0a 2020 2020 6368 6174   token,.    chat
+0000d8f0: 5f69 642c 0a20 2020 2074 6974 6c65 2c0a  _id,.    title,.
+0000d900: 2020 2020 6465 7363 7269 7074 696f 6e2c      description,
+0000d910: 0a20 2020 2069 6e76 6f69 6365 5f70 6179  .    invoice_pay
+0000d920: 6c6f 6164 2c0a 2020 2020 7072 6f76 6964  load,.    provid
+0000d930: 6572 5f74 6f6b 656e 2c0a 2020 2020 6375  er_token,.    cu
+0000d940: 7272 656e 6379 2c0a 2020 2020 7072 6963  rrency,.    pric
+0000d950: 6573 2c0a 2020 2020 7374 6172 745f 7061  es,.    start_pa
+0000d960: 7261 6d65 7465 723d 4e6f 6e65 2c0a 2020  rameter=None,.  
+0000d970: 2020 7068 6f74 6f5f 7572 6c3d 4e6f 6e65    photo_url=None
+0000d980: 2c0a 2020 2020 7068 6f74 6f5f 7369 7a65  ,.    photo_size
+0000d990: 3d4e 6f6e 652c 0a20 2020 2070 686f 746f  =None,.    photo
+0000d9a0: 5f77 6964 7468 3d4e 6f6e 652c 0a20 2020  _width=None,.   
+0000d9b0: 2070 686f 746f 5f68 6569 6768 743d 4e6f   photo_height=No
+0000d9c0: 6e65 2c0a 2020 2020 6e65 6564 5f6e 616d  ne,.    need_nam
+0000d9d0: 653d 4e6f 6e65 2c0a 2020 2020 6e65 6564  e=None,.    need
+0000d9e0: 5f70 686f 6e65 5f6e 756d 6265 723d 4e6f  _phone_number=No
+0000d9f0: 6e65 2c0a 2020 2020 6e65 6564 5f65 6d61  ne,.    need_ema
+0000da00: 696c 3d4e 6f6e 652c 0a20 2020 206e 6565  il=None,.    nee
+0000da10: 645f 7368 6970 7069 6e67 5f61 6464 7265  d_shipping_addre
+0000da20: 7373 3d4e 6f6e 652c 0a20 2020 2073 656e  ss=None,.    sen
+0000da30: 645f 7068 6f6e 655f 6e75 6d62 6572 5f74  d_phone_number_t
+0000da40: 6f5f 7072 6f76 6964 6572 3d4e 6f6e 652c  o_provider=None,
+0000da50: 0a20 2020 2073 656e 645f 656d 6169 6c5f  .    send_email_
+0000da60: 746f 5f70 726f 7669 6465 723d 4e6f 6e65  to_provider=None
+0000da70: 2c0a 2020 2020 6973 5f66 6c65 7869 626c  ,.    is_flexibl
+0000da80: 653d 4e6f 6e65 2c0a 2020 2020 6469 7361  e=None,.    disa
+0000da90: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+0000daa0: 3d4e 6f6e 652c 0a20 2020 2072 6570 6c79  =None,.    reply
+0000dab0: 5f74 6f5f 6d65 7373 6167 655f 6964 3d4e  _to_message_id=N
+0000dac0: 6f6e 652c 0a20 2020 2072 6570 6c79 5f6d  one,.    reply_m
+0000dad0: 6172 6b75 703d 4e6f 6e65 2c0a 2020 2020  arkup=None,.    
+0000dae0: 7072 6f76 6964 6572 5f64 6174 613d 4e6f  provider_data=No
+0000daf0: 6e65 2c0a 2020 2020 7469 6d65 6f75 743d  ne,.    timeout=
+0000db00: 4e6f 6e65 2c0a 2020 2020 616c 6c6f 775f  None,.    allow_
+0000db10: 7365 6e64 696e 675f 7769 7468 6f75 745f  sending_without_
+0000db20: 7265 706c 793d 4e6f 6e65 2c0a 2020 2020  reply=None,.    
+0000db30: 6d61 785f 7469 705f 616d 6f75 6e74 3d4e  max_tip_amount=N
+0000db40: 6f6e 652c 0a20 2020 2073 7567 6765 7374  one,.    suggest
+0000db50: 6564 5f74 6970 5f61 6d6f 756e 7473 3d4e  ed_tip_amounts=N
+0000db60: 6f6e 652c 0a20 2020 2070 726f 7465 6374  one,.    protect
+0000db70: 5f63 6f6e 7465 6e74 3d4e 6f6e 652c 0a20  _content=None,. 
+0000db80: 2020 206d 6573 7361 6765 5f74 6872 6561     message_threa
+0000db90: 645f 6964 3a20 4f70 7469 6f6e 616c 5b69  d_id: Optional[i
+0000dba0: 6e74 5d20 3d20 4e6f 6e65 2c0a 293a 0a20  nt] = None,.):. 
+0000dbb0: 2020 2022 2222 0a20 2020 2055 7365 2074     """.    Use t
+0000dbc0: 6869 7320 6d65 7468 6f64 2074 6f20 7365  his method to se
+0000dbd0: 6e64 2069 6e76 6f69 6365 732e 204f 6e20  nd invoices. On 
+0000dbe0: 7375 6363 6573 732c 2074 6865 2073 656e  success, the sen
+0000dbf0: 7420 4d65 7373 6167 6520 6973 2072 6574  t Message is ret
+0000dc00: 7572 6e65 642e 0a20 2020 203a 7061 7261  urned..    :para
+0000dc10: 6d20 746f 6b65 6e3a 2042 6f74 2773 2074  m token: Bot's t
+0000dc20: 6f6b 656e 2028 796f 7520 646f 6e27 7420  oken (you don't 
+0000dc30: 6e65 6564 2074 6f20 6669 6c6c 2074 6869  need to fill thi
+0000dc40: 7329 0a20 2020 203a 7061 7261 6d20 6368  s).    :param ch
+0000dc50: 6174 5f69 643a 2055 6e69 7175 6520 6964  at_id: Unique id
+0000dc60: 656e 7469 6669 6572 2066 6f72 2074 6865  entifier for the
+0000dc70: 2074 6172 6765 7420 7072 6976 6174 6520   target private 
+0000dc80: 6368 6174 0a20 2020 203a 7061 7261 6d20  chat.    :param 
+0000dc90: 7469 746c 653a 2050 726f 6475 6374 206e  title: Product n
+0000dca0: 616d 650a 2020 2020 3a70 6172 616d 2064  ame.    :param d
+0000dcb0: 6573 6372 6970 7469 6f6e 3a20 5072 6f64  escription: Prod
+0000dcc0: 7563 7420 6465 7363 7269 7074 696f 6e0a  uct description.
+0000dcd0: 2020 2020 3a70 6172 616d 2069 6e76 6f69      :param invoi
+0000dce0: 6365 5f70 6179 6c6f 6164 3a20 426f 742d  ce_payload: Bot-
+0000dcf0: 6465 6669 6e65 6420 696e 766f 6963 6520  defined invoice 
+0000dd00: 7061 796c 6f61 642c 2031 2d31 3238 2062  payload, 1-128 b
+0000dd10: 7974 6573 2e20 5468 6973 2077 696c 6c20  ytes. This will 
+0000dd20: 6e6f 7420 6265 2064 6973 706c 6179 6564  not be displayed
+0000dd30: 2074 6f20 7468 6520 7573 6572 2c20 7573   to the user, us
+0000dd40: 6520 666f 7220 796f 7572 2069 6e74 6572  e for your inter
+0000dd50: 6e61 6c20 7072 6f63 6573 7365 732e 0a20  nal processes.. 
+0000dd60: 2020 203a 7061 7261 6d20 7072 6f76 6964     :param provid
+0000dd70: 6572 5f74 6f6b 656e 3a20 5061 796d 656e  er_token: Paymen
+0000dd80: 7473 2070 726f 7669 6465 7220 746f 6b65  ts provider toke
+0000dd90: 6e2c 206f 6274 6169 6e65 6420 7669 6120  n, obtained via 
+0000dda0: 4042 6f74 6661 7468 6572 0a20 2020 203a  @Botfather.    :
+0000ddb0: 7061 7261 6d20 6375 7272 656e 6379 3a20  param currency: 
+0000ddc0: 5468 7265 652d 6c65 7474 6572 2049 534f  Three-letter ISO
+0000ddd0: 2034 3231 3720 6375 7272 656e 6379 2063   4217 currency c
+0000dde0: 6f64 652c 2073 6565 2068 7474 7073 3a2f  ode, see https:/
+0000ddf0: 2f63 6f72 652e 7465 6c65 6772 616d 2e6f  /core.telegram.o
+0000de00: 7267 2f62 6f74 732f 7061 796d 656e 7473  rg/bots/payments
+0000de10: 2373 7570 706f 7274 6564 2d63 7572 7265  #supported-curre
+0000de20: 6e63 6965 730a 2020 2020 3a70 6172 616d  ncies.    :param
+0000de30: 2070 7269 6365 733a 2050 7269 6365 2062   prices: Price b
+0000de40: 7265 616b 646f 776e 2c20 6120 6c69 7374  reakdown, a list
+0000de50: 206f 6620 636f 6d70 6f6e 656e 7473 2028   of components (
+0000de60: 652e 672e 2070 726f 6475 6374 2070 7269  e.g. product pri
+0000de70: 6365 2c20 7461 782c 2064 6973 636f 756e  ce, tax, discoun
+0000de80: 742c 2064 656c 6976 6572 7920 636f 7374  t, delivery cost
+0000de90: 2c20 6465 6c69 7665 7279 2074 6178 2c20  , delivery tax, 
+0000dea0: 626f 6e75 732c 2065 7463 2e29 0a20 2020  bonus, etc.).   
+0000deb0: 203a 7061 7261 6d20 7374 6172 745f 7061   :param start_pa
+0000dec0: 7261 6d65 7465 723a 2055 6e69 7175 6520  rameter: Unique 
+0000ded0: 6465 6570 2d6c 696e 6b69 6e67 2070 6172  deep-linking par
+0000dee0: 616d 6574 6572 2074 6861 7420 6361 6e20  ameter that can 
+0000def0: 6265 2075 7365 6420 746f 2067 656e 6572  be used to gener
+0000df00: 6174 6520 7468 6973 2069 6e76 6f69 6365  ate this invoice
+0000df10: 2077 6865 6e20 7573 6564 2061 7320 6120   when used as a 
+0000df20: 7374 6172 7420 7061 7261 6d65 7465 720a  start parameter.
+0000df30: 2020 2020 3a70 6172 616d 2070 686f 746f      :param photo
+0000df40: 5f75 726c 3a20 5552 4c20 6f66 2074 6865  _url: URL of the
+0000df50: 2070 726f 6475 6374 2070 686f 746f 2066   product photo f
+0000df60: 6f72 2074 6865 2069 6e76 6f69 6365 2e20  or the invoice. 
+0000df70: 4361 6e20 6265 2061 2070 686f 746f 206f  Can be a photo o
+0000df80: 6620 7468 6520 676f 6f64 7320 6f72 2061  f the goods or a
+0000df90: 206d 6172 6b65 7469 6e67 2069 6d61 6765   marketing image
+0000dfa0: 2066 6f72 2061 2073 6572 7669 6365 2e20   for a service. 
+0000dfb0: 5065 6f70 6c65 206c 696b 6520 6974 2062  People like it b
+0000dfc0: 6574 7465 7220 7768 656e 2074 6865 7920  etter when they 
+0000dfd0: 7365 6520 7768 6174 2074 6865 7920 6172  see what they ar
+0000dfe0: 6520 7061 7969 6e67 2066 6f72 2e0a 2020  e paying for..  
+0000dff0: 2020 3a70 6172 616d 2070 686f 746f 5f73    :param photo_s
+0000e000: 697a 653a 2050 686f 746f 2073 697a 650a  ize: Photo size.
+0000e010: 2020 2020 3a70 6172 616d 2070 686f 746f      :param photo
+0000e020: 5f77 6964 7468 3a20 5068 6f74 6f20 7769  _width: Photo wi
+0000e030: 6474 680a 2020 2020 3a70 6172 616d 2070  dth.    :param p
+0000e040: 686f 746f 5f68 6569 6768 743a 2050 686f  hoto_height: Pho
+0000e050: 746f 2068 6569 6768 740a 2020 2020 3a70  to height.    :p
+0000e060: 6172 616d 206e 6565 645f 6e61 6d65 3a20  aram need_name: 
+0000e070: 5061 7373 2054 7275 652c 2069 6620 796f  Pass True, if yo
+0000e080: 7520 7265 7175 6972 6520 7468 6520 7573  u require the us
+0000e090: 6572 2773 2066 756c 6c20 6e61 6d65 2074  er's full name t
+0000e0a0: 6f20 636f 6d70 6c65 7465 2074 6865 206f  o complete the o
+0000e0b0: 7264 6572 0a20 2020 203a 7061 7261 6d20  rder.    :param 
+0000e0c0: 6e65 6564 5f70 686f 6e65 5f6e 756d 6265  need_phone_numbe
+0000e0d0: 723a 2050 6173 7320 5472 7565 2c20 6966  r: Pass True, if
+0000e0e0: 2079 6f75 2072 6571 7569 7265 2074 6865   you require the
+0000e0f0: 2075 7365 7227 7320 7068 6f6e 6520 6e75   user's phone nu
+0000e100: 6d62 6572 2074 6f20 636f 6d70 6c65 7465  mber to complete
+0000e110: 2074 6865 206f 7264 6572 0a20 2020 203a   the order.    :
+0000e120: 7061 7261 6d20 6e65 6564 5f65 6d61 696c  param need_email
+0000e130: 3a20 5061 7373 2054 7275 652c 2069 6620  : Pass True, if 
+0000e140: 796f 7520 7265 7175 6972 6520 7468 6520  you require the 
+0000e150: 7573 6572 2773 2065 6d61 696c 2074 6f20  user's email to 
+0000e160: 636f 6d70 6c65 7465 2074 6865 206f 7264  complete the ord
+0000e170: 6572 0a20 2020 203a 7061 7261 6d20 6e65  er.    :param ne
+0000e180: 6564 5f73 6869 7070 696e 675f 6164 6472  ed_shipping_addr
+0000e190: 6573 733a 2050 6173 7320 5472 7565 2c20  ess: Pass True, 
+0000e1a0: 6966 2079 6f75 2072 6571 7569 7265 2074  if you require t
+0000e1b0: 6865 2075 7365 7227 7320 7368 6970 7069  he user's shippi
+0000e1c0: 6e67 2061 6464 7265 7373 2074 6f20 636f  ng address to co
+0000e1d0: 6d70 6c65 7465 2074 6865 206f 7264 6572  mplete the order
+0000e1e0: 0a20 2020 203a 7061 7261 6d20 6973 5f66  .    :param is_f
+0000e1f0: 6c65 7869 626c 653a 2050 6173 7320 5472  lexible: Pass Tr
+0000e200: 7565 2c20 6966 2074 6865 2066 696e 616c  ue, if the final
+0000e210: 2070 7269 6365 2064 6570 656e 6473 206f   price depends o
+0000e220: 6e20 7468 6520 7368 6970 7069 6e67 206d  n the shipping m
+0000e230: 6574 686f 640a 2020 2020 3a70 6172 616d  ethod.    :param
+0000e240: 2073 656e 645f 7068 6f6e 655f 6e75 6d62   send_phone_numb
+0000e250: 6572 5f74 6f5f 7072 6f76 6964 6572 3a20  er_to_provider: 
+0000e260: 5061 7373 2054 7275 652c 2069 6620 7573  Pass True, if us
+0000e270: 6572 2773 2070 686f 6e65 206e 756d 6265  er's phone numbe
+0000e280: 7220 7368 6f75 6c64 2062 6520 7365 6e74  r should be sent
+0000e290: 2074 6f20 7072 6f76 6964 6572 0a20 2020   to provider.   
+0000e2a0: 203a 7061 7261 6d20 7365 6e64 5f65 6d61   :param send_ema
+0000e2b0: 696c 5f74 6f5f 7072 6f76 6964 6572 3a20  il_to_provider: 
+0000e2c0: 5061 7373 2054 7275 652c 2069 6620 7573  Pass True, if us
+0000e2d0: 6572 2773 2065 6d61 696c 2061 6464 7265  er's email addre
+0000e2e0: 7373 2073 686f 756c 6420 6265 2073 656e  ss should be sen
+0000e2f0: 7420 746f 2070 726f 7669 6465 720a 2020  t to provider.  
+0000e300: 2020 3a70 6172 616d 2064 6973 6162 6c65    :param disable
+0000e310: 5f6e 6f74 6966 6963 6174 696f 6e3a 2053  _notification: S
+0000e320: 656e 6473 2074 6865 206d 6573 7361 6765  ends the message
+0000e330: 2073 696c 656e 746c 792e 2055 7365 7273   silently. Users
+0000e340: 2077 696c 6c20 7265 6365 6976 6520 6120   will receive a 
+0000e350: 6e6f 7469 6669 6361 7469 6f6e 2077 6974  notification wit
+0000e360: 6820 6e6f 2073 6f75 6e64 2e0a 2020 2020  h no sound..    
+0000e370: 3a70 6172 616d 2072 6570 6c79 5f74 6f5f  :param reply_to_
+0000e380: 6d65 7373 6167 655f 6964 3a20 4966 2074  message_id: If t
+0000e390: 6865 206d 6573 7361 6765 2069 7320 6120  he message is a 
+0000e3a0: 7265 706c 792c 2049 4420 6f66 2074 6865  reply, ID of the
+0000e3b0: 206f 7269 6769 6e61 6c20 6d65 7373 6167   original messag
+0000e3c0: 650a 2020 2020 3a70 6172 616d 2072 6570  e.    :param rep
+0000e3d0: 6c79 5f6d 6172 6b75 703a 2041 204a 534f  ly_markup: A JSO
+0000e3e0: 4e2d 7365 7269 616c 697a 6564 206f 626a  N-serialized obj
+0000e3f0: 6563 7420 666f 7220 616e 2069 6e6c 696e  ect for an inlin
+0000e400: 6520 6b65 7962 6f61 7264 2e20 4966 2065  e keyboard. If e
+0000e410: 6d70 7479 2c20 6f6e 6520 2750 6179 2074  mpty, one 'Pay t
+0000e420: 6f74 616c 2070 7269 6365 2720 6275 7474  otal price' butt
+0000e430: 6f6e 2077 696c 6c20 6265 2073 686f 776e  on will be shown
+0000e440: 2e20 4966 206e 6f74 2065 6d70 7479 2c20  . If not empty, 
+0000e450: 7468 6520 6669 7273 7420 6275 7474 6f6e  the first button
+0000e460: 206d 7573 7420 6265 2061 2050 6179 2062   must be a Pay b
+0000e470: 7574 746f 6e0a 2020 2020 3a70 6172 616d  utton.    :param
+0000e480: 2070 726f 7669 6465 725f 6461 7461 3a20   provider_data: 
+0000e490: 4120 4a53 4f4e 2d73 6572 6961 6c69 7a65  A JSON-serialize
+0000e4a0: 6420 6461 7461 2061 626f 7574 2074 6865  d data about the
+0000e4b0: 2069 6e76 6f69 6365 2c20 7768 6963 6820   invoice, which 
+0000e4c0: 7769 6c6c 2062 6520 7368 6172 6564 2077  will be shared w
+0000e4d0: 6974 6820 7468 6520 7061 796d 656e 7420  ith the payment 
+0000e4e0: 7072 6f76 6964 6572 2e20 4120 6465 7461  provider. A deta
+0000e4f0: 696c 6564 2064 6573 6372 6970 7469 6f6e  iled description
+0000e500: 206f 6620 7265 7175 6972 6564 2066 6965   of required fie
+0000e510: 6c64 7320 7368 6f75 6c64 2062 6520 7072  lds should be pr
+0000e520: 6f76 6964 6564 2062 7920 7468 6520 7061  ovided by the pa
+0000e530: 796d 656e 7420 7072 6f76 6964 6572 2e0a  yment provider..
+0000e540: 2020 2020 3a70 6172 616d 2074 696d 656f      :param timeo
+0000e550: 7574 3a0a 2020 2020 3a70 6172 616d 2061  ut:.    :param a
+0000e560: 6c6c 6f77 5f73 656e 6469 6e67 5f77 6974  llow_sending_wit
+0000e570: 686f 7574 5f72 6570 6c79 3a0a 2020 2020  hout_reply:.    
+0000e580: 3a70 6172 616d 206d 6178 5f74 6970 5f61  :param max_tip_a
+0000e590: 6d6f 756e 743a 2054 6865 206d 6178 696d  mount: The maxim
+0000e5a0: 756d 2061 6363 6570 7465 6420 616d 6f75  um accepted amou
+0000e5b0: 6e74 2066 6f72 2074 6970 7320 696e 2074  nt for tips in t
+0000e5c0: 6865 2073 6d61 6c6c 6573 7420 756e 6974  he smallest unit
+0000e5d0: 7320 6f66 2074 6865 2063 7572 7265 6e63  s of the currenc
+0000e5e0: 790a 2020 2020 3a70 6172 616d 2073 7567  y.    :param sug
+0000e5f0: 6765 7374 6564 5f74 6970 5f61 6d6f 756e  gested_tip_amoun
+0000e600: 7473 3a20 4120 4a53 4f4e 2d73 6572 6961  ts: A JSON-seria
+0000e610: 6c69 7a65 6420 6172 7261 7920 6f66 2073  lized array of s
+0000e620: 7567 6765 7374 6564 2061 6d6f 756e 7473  uggested amounts
+0000e630: 206f 6620 7469 7073 2069 6e20 7468 6520   of tips in the 
+0000e640: 736d 616c 6c65 7374 2075 6e69 7473 206f  smallest units o
+0000e650: 6620 7468 6520 6375 7272 656e 6379 2e0a  f the currency..
+0000e660: 2020 2020 2020 2020 4174 206d 6f73 7420          At most 
+0000e670: 3420 7375 6767 6573 7465 6420 7469 7020  4 suggested tip 
+0000e680: 616d 6f75 6e74 7320 6361 6e20 6265 2073  amounts can be s
+0000e690: 7065 6369 6669 6564 2e20 5468 6520 7375  pecified. The su
+0000e6a0: 6767 6573 7465 6420 7469 7020 616d 6f75  ggested tip amou
+0000e6b0: 6e74 7320 6d75 7374 2062 6520 706f 7369  nts must be posi
+0000e6c0: 7469 7665 2c20 7061 7373 6564 2069 6e20  tive, passed in 
+0000e6d0: 6120 7374 7269 6374 6c79 2069 6e63 7265  a strictly incre
+0000e6e0: 6173 6564 206f 7264 6572 2061 6e64 206d  ased order and m
+0000e6f0: 7573 7420 6e6f 7420 6578 6365 6564 206d  ust not exceed m
+0000e700: 6178 5f74 6970 5f61 6d6f 756e 742e 0a20  ax_tip_amount.. 
+0000e710: 2020 203a 7061 7261 6d20 7072 6f74 6563     :param protec
+0000e720: 745f 636f 6e74 656e 743a 0a20 2020 203a  t_content:.    :
+0000e730: 7265 7475 726e 3a0a 2020 2020 2222 220a  return:.    """.
+0000e740: 2020 2020 6d65 7468 6f64 5f75 726c 203d      method_url =
+0000e750: 2072 2273 656e 6449 6e76 6f69 6365 220a   r"sendInvoice".
+0000e760: 2020 2020 7061 796c 6f61 6420 3d20 7b0a      payload = {.
+0000e770: 2020 2020 2020 2020 2263 6861 745f 6964          "chat_id
+0000e780: 223a 2063 6861 745f 6964 2c0a 2020 2020  ": chat_id,.    
+0000e790: 2020 2020 2274 6974 6c65 223a 2074 6974      "title": tit
+0000e7a0: 6c65 2c0a 2020 2020 2020 2020 2264 6573  le,.        "des
+0000e7b0: 6372 6970 7469 6f6e 223a 2064 6573 6372  cription": descr
+0000e7c0: 6970 7469 6f6e 2c0a 2020 2020 2020 2020  iption,.        
+0000e7d0: 2270 6179 6c6f 6164 223a 2069 6e76 6f69  "payload": invoi
+0000e7e0: 6365 5f70 6179 6c6f 6164 2c0a 2020 2020  ce_payload,.    
+0000e7f0: 2020 2020 2270 726f 7669 6465 725f 746f      "provider_to
+0000e800: 6b65 6e22 3a20 7072 6f76 6964 6572 5f74  ken": provider_t
+0000e810: 6f6b 656e 2c0a 2020 2020 2020 2020 2263  oken,.        "c
+0000e820: 7572 7265 6e63 7922 3a20 6375 7272 656e  urrency": curren
+0000e830: 6379 2c0a 2020 2020 2020 2020 2270 7269  cy,.        "pri
+0000e840: 6365 7322 3a20 6177 6169 7420 5f63 6f6e  ces": await _con
+0000e850: 7665 7274 5f6c 6973 745f 6a73 6f6e 5f73  vert_list_json_s
+0000e860: 6572 6961 6c69 7a61 626c 6528 7072 6963  erializable(pric
+0000e870: 6573 292c 0a20 2020 207d 0a20 2020 2069  es),.    }.    i
+0000e880: 6620 7374 6172 745f 7061 7261 6d65 7465  f start_paramete
+0000e890: 723a 0a20 2020 2020 2020 2070 6179 6c6f  r:.        paylo
+0000e8a0: 6164 5b22 7374 6172 745f 7061 7261 6d65  ad["start_parame
+0000e8b0: 7465 7222 5d20 3d20 7374 6172 745f 7061  ter"] = start_pa
+0000e8c0: 7261 6d65 7465 720a 2020 2020 6966 2070  rameter.    if p
+0000e8d0: 686f 746f 5f75 726c 3a0a 2020 2020 2020  hoto_url:.      
+0000e8e0: 2020 7061 796c 6f61 645b 2270 686f 746f    payload["photo
+0000e8f0: 5f75 726c 225d 203d 2070 686f 746f 5f75  _url"] = photo_u
+0000e900: 726c 0a20 2020 2069 6620 7068 6f74 6f5f  rl.    if photo_
+0000e910: 7369 7a65 3a0a 2020 2020 2020 2020 7061  size:.        pa
+0000e920: 796c 6f61 645b 2270 686f 746f 5f73 697a  yload["photo_siz
+0000e930: 6522 5d20 3d20 7068 6f74 6f5f 7369 7a65  e"] = photo_size
+0000e940: 0a20 2020 2069 6620 7068 6f74 6f5f 7769  .    if photo_wi
+0000e950: 6474 683a 0a20 2020 2020 2020 2070 6179  dth:.        pay
+0000e960: 6c6f 6164 5b22 7068 6f74 6f5f 7769 6474  load["photo_widt
+0000e970: 6822 5d20 3d20 7068 6f74 6f5f 7769 6474  h"] = photo_widt
+0000e980: 680a 2020 2020 6966 2070 686f 746f 5f68  h.    if photo_h
+0000e990: 6569 6768 743a 0a20 2020 2020 2020 2070  eight:.        p
+0000e9a0: 6179 6c6f 6164 5b22 7068 6f74 6f5f 6865  ayload["photo_he
+0000e9b0: 6967 6874 225d 203d 2070 686f 746f 5f68  ight"] = photo_h
+0000e9c0: 6569 6768 740a 2020 2020 6966 206e 6565  eight.    if nee
+0000e9d0: 645f 6e61 6d65 2069 7320 6e6f 7420 4e6f  d_name is not No
+0000e9e0: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
+0000e9f0: 6f61 645b 226e 6565 645f 6e61 6d65 225d  oad["need_name"]
+0000ea00: 203d 206e 6565 645f 6e61 6d65 0a20 2020   = need_name.   
+0000ea10: 2069 6620 6e65 6564 5f70 686f 6e65 5f6e   if need_phone_n
+0000ea20: 756d 6265 7220 6973 206e 6f74 204e 6f6e  umber is not Non
+0000ea30: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
+0000ea40: 6164 5b22 6e65 6564 5f70 686f 6e65 5f6e  ad["need_phone_n
+0000ea50: 756d 6265 7222 5d20 3d20 6e65 6564 5f70  umber"] = need_p
+0000ea60: 686f 6e65 5f6e 756d 6265 720a 2020 2020  hone_number.    
+0000ea70: 6966 206e 6565 645f 656d 6169 6c20 6973  if need_email is
+0000ea80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000ea90: 2020 2070 6179 6c6f 6164 5b22 6e65 6564     payload["need
+0000eaa0: 5f65 6d61 696c 225d 203d 206e 6565 645f  _email"] = need_
+0000eab0: 656d 6169 6c0a 2020 2020 6966 206e 6565  email.    if nee
+0000eac0: 645f 7368 6970 7069 6e67 5f61 6464 7265  d_shipping_addre
+0000ead0: 7373 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ss is not None:.
+0000eae0: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
+0000eaf0: 226e 6565 645f 7368 6970 7069 6e67 5f61  "need_shipping_a
+0000eb00: 6464 7265 7373 225d 203d 206e 6565 645f  ddress"] = need_
+0000eb10: 7368 6970 7069 6e67 5f61 6464 7265 7373  shipping_address
+0000eb20: 0a20 2020 2069 6620 7365 6e64 5f70 686f  .    if send_pho
+0000eb30: 6e65 5f6e 756d 6265 725f 746f 5f70 726f  ne_number_to_pro
+0000eb40: 7669 6465 7220 6973 206e 6f74 204e 6f6e  vider is not Non
+0000eb50: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
+0000eb60: 6164 5b22 7365 6e64 5f70 686f 6e65 5f6e  ad["send_phone_n
+0000eb70: 756d 6265 725f 746f 5f70 726f 7669 6465  umber_to_provide
+0000eb80: 7222 5d20 3d20 7365 6e64 5f70 686f 6e65  r"] = send_phone
+0000eb90: 5f6e 756d 6265 725f 746f 5f70 726f 7669  _number_to_provi
+0000eba0: 6465 720a 2020 2020 6966 2073 656e 645f  der.    if send_
+0000ebb0: 656d 6169 6c5f 746f 5f70 726f 7669 6465  email_to_provide
+0000ebc0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
+0000ebd0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+0000ebe0: 7365 6e64 5f65 6d61 696c 5f74 6f5f 7072  send_email_to_pr
+0000ebf0: 6f76 6964 6572 225d 203d 2073 656e 645f  ovider"] = send_
+0000ec00: 656d 6169 6c5f 746f 5f70 726f 7669 6465  email_to_provide
+0000ec10: 720a 2020 2020 6966 2069 735f 666c 6578  r.    if is_flex
+0000ec20: 6962 6c65 2069 7320 6e6f 7420 4e6f 6e65  ible is not None
+0000ec30: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+0000ec40: 645b 2269 735f 666c 6578 6962 6c65 225d  d["is_flexible"]
+0000ec50: 203d 2069 735f 666c 6578 6962 6c65 0a20   = is_flexible. 
+0000ec60: 2020 2069 6620 6469 7361 626c 655f 6e6f     if disable_no
+0000ec70: 7469 6669 6361 7469 6f6e 2069 7320 6e6f  tification is no
+0000ec80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000ec90: 7061 796c 6f61 645b 2264 6973 6162 6c65  payload["disable
+0000eca0: 5f6e 6f74 6966 6963 6174 696f 6e22 5d20  _notification"] 
+0000ecb0: 3d20 6469 7361 626c 655f 6e6f 7469 6669  = disable_notifi
+0000ecc0: 6361 7469 6f6e 0a20 2020 2069 6620 7265  cation.    if re
+0000ecd0: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
+0000ece0: 643a 0a20 2020 2020 2020 2070 6179 6c6f  d:.        paylo
+0000ecf0: 6164 5b22 7265 706c 795f 746f 5f6d 6573  ad["reply_to_mes
+0000ed00: 7361 6765 5f69 6422 5d20 3d20 7265 706c  sage_id"] = repl
+0000ed10: 795f 746f 5f6d 6573 7361 6765 5f69 640a  y_to_message_id.
+0000ed20: 2020 2020 6966 2072 6570 6c79 5f6d 6172      if reply_mar
+0000ed30: 6b75 703a 0a20 2020 2020 2020 2070 6179  kup:.        pay
+0000ed40: 6c6f 6164 5b22 7265 706c 795f 6d61 726b  load["reply_mark
+0000ed50: 7570 225d 203d 2061 7761 6974 205f 636f  up"] = await _co
+0000ed60: 6e76 6572 745f 6d61 726b 7570 2872 6570  nvert_markup(rep
+0000ed70: 6c79 5f6d 6172 6b75 7029 0a20 2020 2069  ly_markup).    i
+0000ed80: 6620 7072 6f76 6964 6572 5f64 6174 613a  f provider_data:
+0000ed90: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+0000eda0: 5b22 7072 6f76 6964 6572 5f64 6174 6122  ["provider_data"
+0000edb0: 5d20 3d20 7072 6f76 6964 6572 5f64 6174  ] = provider_dat
+0000edc0: 610a 2020 2020 6966 2074 696d 656f 7574  a.    if timeout
+0000edd0: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+0000ede0: 645b 2274 696d 656f 7574 225d 203d 2074  d["timeout"] = t
+0000edf0: 696d 656f 7574 0a20 2020 2069 6620 616c  imeout.    if al
+0000ee00: 6c6f 775f 7365 6e64 696e 675f 7769 7468  low_sending_with
+0000ee10: 6f75 745f 7265 706c 7920 6973 206e 6f74  out_reply is not
+0000ee20: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
+0000ee30: 6179 6c6f 6164 5b22 616c 6c6f 775f 7365  ayload["allow_se
+0000ee40: 6e64 696e 675f 7769 7468 6f75 745f 7265  nding_without_re
+0000ee50: 706c 7922 5d20 3d20 616c 6c6f 775f 7365  ply"] = allow_se
+0000ee60: 6e64 696e 675f 7769 7468 6f75 745f 7265  nding_without_re
+0000ee70: 706c 790a 2020 2020 6966 206d 6178 5f74  ply.    if max_t
+0000ee80: 6970 5f61 6d6f 756e 7420 6973 206e 6f74  ip_amount is not
+0000ee90: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
+0000eea0: 6179 6c6f 6164 5b22 6d61 785f 7469 705f  ayload["max_tip_
+0000eeb0: 616d 6f75 6e74 225d 203d 206d 6178 5f74  amount"] = max_t
+0000eec0: 6970 5f61 6d6f 756e 740a 2020 2020 6966  ip_amount.    if
+0000eed0: 2073 7567 6765 7374 6564 5f74 6970 5f61   suggested_tip_a
+0000eee0: 6d6f 756e 7473 2069 7320 6e6f 7420 4e6f  mounts is not No
+0000eef0: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
+0000ef00: 6f61 645b 2273 7567 6765 7374 6564 5f74  oad["suggested_t
+0000ef10: 6970 5f61 6d6f 756e 7473 225d 203d 206a  ip_amounts"] = j
+0000ef20: 736f 6e2e 6475 6d70 7328 7375 6767 6573  son.dumps(sugges
+0000ef30: 7465 645f 7469 705f 616d 6f75 6e74 7329  ted_tip_amounts)
+0000ef40: 0a20 2020 2069 6620 7072 6f74 6563 745f  .    if protect_
+0000ef50: 636f 6e74 656e 7420 6973 206e 6f74 204e  content is not N
+0000ef60: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
+0000ef70: 6c6f 6164 5b22 7072 6f74 6563 745f 636f  load["protect_co
+0000ef80: 6e74 656e 7422 5d20 3d20 7072 6f74 6563  ntent"] = protec
+0000ef90: 745f 636f 6e74 656e 740a 2020 2020 5f61  t_content.    _a
+0000efa0: 6464 5f6d 6573 7361 6765 5f74 6872 6561  dd_message_threa
+0000efb0: 645f 6964 2870 6179 6c6f 6164 2c20 6d65  d_id(payload, me
+0000efc0: 7373 6167 655f 7468 7265 6164 5f69 6429  ssage_thread_id)
+0000efd0: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
+0000efe0: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
+0000eff0: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
+0000f000: 7261 6d73 3d70 6179 6c6f 6164 290a 0a0a  rams=payload)...
+0000f010: 6173 796e 6320 6465 6620 616e 7377 6572  async def answer
+0000f020: 5f73 6869 7070 696e 675f 7175 6572 7928  _shipping_query(
+0000f030: 746f 6b65 6e2c 2073 6869 7070 696e 675f  token, shipping_
+0000f040: 7175 6572 795f 6964 2c20 6f6b 2c20 7368  query_id, ok, sh
+0000f050: 6970 7069 6e67 5f6f 7074 696f 6e73 3d4e  ipping_options=N
+0000f060: 6f6e 652c 2065 7272 6f72 5f6d 6573 7361  one, error_messa
+0000f070: 6765 3d4e 6f6e 6529 3a0a 2020 2020 2222  ge=None):.    ""
+0000f080: 220a 2020 2020 4966 2079 6f75 2073 656e  ".    If you sen
+0000f090: 7420 616e 2069 6e76 6f69 6365 2072 6571  t an invoice req
+0000f0a0: 7565 7374 696e 6720 6120 7368 6970 7069  uesting a shippi
+0000f0b0: 6e67 2061 6464 7265 7373 2061 6e64 2074  ng address and t
+0000f0c0: 6865 2070 6172 616d 6574 6572 2069 735f  he parameter is_
+0000f0d0: 666c 6578 6962 6c65 2077 6173 2073 7065  flexible was spe
+0000f0e0: 6369 6669 6564 2c20 7468 6520 426f 7420  cified, the Bot 
+0000f0f0: 4150 4920 7769 6c6c 2073 656e 6420 616e  API will send an
+0000f100: 2055 7064 6174 6520 7769 7468 2061 2073   Update with a s
+0000f110: 6869 7070 696e 675f 7175 6572 7920 6669  hipping_query fi
+0000f120: 656c 6420 746f 2074 6865 2062 6f74 2e20  eld to the bot. 
+0000f130: 5573 6520 7468 6973 206d 6574 686f 6420  Use this method 
+0000f140: 746f 2072 6570 6c79 2074 6f20 7368 6970  to reply to ship
+0000f150: 7069 6e67 2071 7565 7269 6573 2e20 4f6e  ping queries. On
+0000f160: 2073 7563 6365 7373 2c20 5472 7565 2069   success, True i
+0000f170: 7320 7265 7475 726e 6564 2e0a 2020 2020  s returned..    
+0000f180: 3a70 6172 616d 2074 6f6b 656e 3a20 426f  :param token: Bo
+0000f190: 7427 7320 746f 6b65 6e20 2879 6f75 2064  t's token (you d
+0000f1a0: 6f6e 2774 206e 6565 6420 746f 2066 696c  on't need to fil
+0000f1b0: 6c20 7468 6973 290a 2020 2020 3a70 6172  l this).    :par
+0000f1c0: 616d 2073 6869 7070 696e 675f 7175 6572  am shipping_quer
+0000f1d0: 795f 6964 3a20 556e 6971 7565 2069 6465  y_id: Unique ide
+0000f1e0: 6e74 6966 6965 7220 666f 7220 7468 6520  ntifier for the 
+0000f1f0: 7175 6572 7920 746f 2062 6520 616e 7377  query to be answ
+0000f200: 6572 6564 0a20 2020 203a 7061 7261 6d20  ered.    :param 
+0000f210: 6f6b 3a20 5370 6563 6966 7920 5472 7565  ok: Specify True
+0000f220: 2069 6620 6465 6c69 7665 7279 2074 6f20   if delivery to 
+0000f230: 7468 6520 7370 6563 6966 6965 6420 6164  the specified ad
+0000f240: 6472 6573 7320 6973 2070 6f73 7369 626c  dress is possibl
+0000f250: 6520 616e 6420 4661 6c73 6520 6966 2074  e and False if t
+0000f260: 6865 7265 2061 7265 2061 6e79 2070 726f  here are any pro
+0000f270: 626c 656d 7320 2866 6f72 2065 7861 6d70  blems (for examp
+0000f280: 6c65 2c20 6966 2064 656c 6976 6572 7920  le, if delivery 
+0000f290: 746f 2074 6865 2073 7065 6369 6669 6564  to the specified
+0000f2a0: 2061 6464 7265 7373 2069 7320 6e6f 7420   address is not 
+0000f2b0: 706f 7373 6962 6c65 290a 2020 2020 3a70  possible).    :p
+0000f2c0: 6172 616d 2073 6869 7070 696e 675f 6f70  aram shipping_op
+0000f2d0: 7469 6f6e 733a 2052 6571 7569 7265 6420  tions: Required 
+0000f2e0: 6966 206f 6b20 6973 2054 7275 652e 2041  if ok is True. A
+0000f2f0: 204a 534f 4e2d 7365 7269 616c 697a 6564   JSON-serialized
+0000f300: 2061 7272 6179 206f 6620 6176 6169 6c61   array of availa
+0000f310: 626c 6520 7368 6970 7069 6e67 206f 7074  ble shipping opt
+0000f320: 696f 6e73 2e0a 2020 2020 3a70 6172 616d  ions..    :param
+0000f330: 2065 7272 6f72 5f6d 6573 7361 6765 3a20   error_message: 
+0000f340: 5265 7175 6972 6564 2069 6620 6f6b 2069  Required if ok i
+0000f350: 7320 4661 6c73 652e 2045 7272 6f72 206d  s False. Error m
+0000f360: 6573 7361 6765 2069 6e20 6875 6d61 6e20  essage in human 
+0000f370: 7265 6164 6162 6c65 2066 6f72 6d20 7468  readable form th
+0000f380: 6174 2065 7870 6c61 696e 7320 7768 7920  at explains why 
+0000f390: 6974 2069 7320 696d 706f 7373 6962 6c65  it is impossible
+0000f3a0: 2074 6f20 636f 6d70 6c65 7465 2074 6865   to complete the
+0000f3b0: 206f 7264 6572 2028 652e 672e 2022 536f   order (e.g. "So
+0000f3c0: 7272 792c 2064 656c 6976 6572 7920 746f  rry, delivery to
+0000f3d0: 2079 6f75 7220 6465 7369 7265 6420 6164   your desired ad
+0000f3e0: 6472 6573 7320 6973 2075 6e61 7661 696c  dress is unavail
+0000f3f0: 6162 6c65 2729 2e20 5465 6c65 6772 616d  able'). Telegram
+0000f400: 2077 696c 6c20 6469 7370 6c61 7920 7468   will display th
+0000f410: 6973 206d 6573 7361 6765 2074 6f20 7468  is message to th
+0000f420: 6520 7573 6572 2e0a 2020 2020 3a72 6574  e user..    :ret
+0000f430: 7572 6e3a 0a20 2020 2022 2222 0a20 2020  urn:.    """.   
+0000f440: 206d 6574 686f 645f 7572 6c20 3d20 2261   method_url = "a
+0000f450: 6e73 7765 7253 6869 7070 696e 6751 7565  nswerShippingQue
+0000f460: 7279 220a 2020 2020 7061 796c 6f61 6420  ry".    payload 
+0000f470: 3d20 7b22 7368 6970 7069 6e67 5f71 7565  = {"shipping_que
+0000f480: 7279 5f69 6422 3a20 7368 6970 7069 6e67  ry_id": shipping
+0000f490: 5f71 7565 7279 5f69 642c 2022 6f6b 223a  _query_id, "ok":
+0000f4a0: 206f 6b7d 0a20 2020 2069 6620 7368 6970   ok}.    if ship
+0000f4b0: 7069 6e67 5f6f 7074 696f 6e73 3a0a 2020  ping_options:.  
+0000f4c0: 2020 2020 2020 7061 796c 6f61 645b 2273        payload["s
+0000f4d0: 6869 7070 696e 675f 6f70 7469 6f6e 7322  hipping_options"
+0000f4e0: 5d20 3d20 6177 6169 7420 5f63 6f6e 7665  ] = await _conve
+0000f4f0: 7274 5f6c 6973 745f 6a73 6f6e 5f73 6572  rt_list_json_ser
+0000f500: 6961 6c69 7a61 626c 6528 7368 6970 7069  ializable(shippi
+0000f510: 6e67 5f6f 7074 696f 6e73 290a 2020 2020  ng_options).    
+0000f520: 6966 2065 7272 6f72 5f6d 6573 7361 6765  if error_message
+0000f530: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+0000f540: 645b 2265 7272 6f72 5f6d 6573 7361 6765  d["error_message
+0000f550: 225d 203d 2065 7272 6f72 5f6d 6573 7361  "] = error_messa
+0000f560: 6765 0a20 2020 2072 6574 7572 6e20 6177  ge.    return aw
+0000f570: 6169 7420 5f72 6571 7565 7374 2874 6f6b  ait _request(tok
+0000f580: 656e 2c20 6d65 7468 6f64 5f75 726c 2c20  en, method_url, 
+0000f590: 7061 7261 6d73 3d70 6179 6c6f 6164 290a  params=payload).
+0000f5a0: 0a0a 6173 796e 6320 6465 6620 616e 7377  ..async def answ
+0000f5b0: 6572 5f70 7265 5f63 6865 636b 6f75 745f  er_pre_checkout_
+0000f5c0: 7175 6572 7928 746f 6b65 6e2c 2070 7265  query(token, pre
+0000f5d0: 5f63 6865 636b 6f75 745f 7175 6572 795f  _checkout_query_
+0000f5e0: 6964 2c20 6f6b 2c20 6572 726f 725f 6d65  id, ok, error_me
+0000f5f0: 7373 6167 653d 4e6f 6e65 293a 0a20 2020  ssage=None):.   
+0000f600: 2022 2222 0a20 2020 204f 6e63 6520 7468   """.    Once th
+0000f610: 6520 7573 6572 2068 6173 2063 6f6e 6669  e user has confi
+0000f620: 726d 6564 2074 6865 6972 2070 6179 6d65  rmed their payme
+0000f630: 6e74 2061 6e64 2073 6869 7070 696e 6720  nt and shipping 
+0000f640: 6465 7461 696c 732c 2074 6865 2042 6f74  details, the Bot
+0000f650: 2041 5049 2073 656e 6473 2074 6865 2066   API sends the f
+0000f660: 696e 616c 2063 6f6e 6669 726d 6174 696f  inal confirmatio
+0000f670: 6e20 696e 2074 6865 2066 6f72 6d20 6f66  n in the form of
+0000f680: 2061 6e20 5570 6461 7465 2077 6974 6820   an Update with 
+0000f690: 7468 6520 6669 656c 6420 7072 655f 6368  the field pre_ch
+0000f6a0: 6563 6b6f 7574 5f71 7565 7279 2e20 5573  eckout_query. Us
+0000f6b0: 6520 7468 6973 206d 6574 686f 6420 746f  e this method to
+0000f6c0: 2072 6573 706f 6e64 2074 6f20 7375 6368   respond to such
+0000f6d0: 2070 7265 2d63 6865 636b 6f75 7420 7175   pre-checkout qu
+0000f6e0: 6572 6965 732e 204f 6e20 7375 6363 6573  eries. On succes
+0000f6f0: 732c 2054 7275 6520 6973 2072 6574 7572  s, True is retur
+0000f700: 6e65 642e 204e 6f74 653a 2054 6865 2042  ned. Note: The B
+0000f710: 6f74 2041 5049 206d 7573 7420 7265 6365  ot API must rece
+0000f720: 6976 6520 616e 2061 6e73 7765 7220 7769  ive an answer wi
+0000f730: 7468 696e 2031 3020 7365 636f 6e64 7320  thin 10 seconds 
+0000f740: 6166 7465 7220 7468 6520 7072 652d 6368  after the pre-ch
+0000f750: 6563 6b6f 7574 2071 7565 7279 2077 6173  eckout query was
+0000f760: 2073 656e 742e 0a20 2020 203a 7061 7261   sent..    :para
+0000f770: 6d20 746f 6b65 6e3a 2042 6f74 2773 2074  m token: Bot's t
+0000f780: 6f6b 656e 2028 796f 7520 646f 6e27 7420  oken (you don't 
+0000f790: 6e65 6564 2074 6f20 6669 6c6c 2074 6869  need to fill thi
+0000f7a0: 7329 0a20 2020 203a 7061 7261 6d20 7072  s).    :param pr
+0000f7b0: 655f 6368 6563 6b6f 7574 5f71 7565 7279  e_checkout_query
+0000f7c0: 5f69 643a 2055 6e69 7175 6520 6964 656e  _id: Unique iden
+0000f7d0: 7469 6669 6572 2066 6f72 2074 6865 2071  tifier for the q
+0000f7e0: 7565 7279 2074 6f20 6265 2061 6e73 7765  uery to be answe
+0000f7f0: 7265 640a 2020 2020 3a70 6172 616d 206f  red.    :param o
+0000f800: 6b3a 2053 7065 6369 6679 2054 7275 6520  k: Specify True 
+0000f810: 6966 2065 7665 7279 7468 696e 6720 6973  if everything is
+0000f820: 2061 6c72 6967 6874 2028 676f 6f64 7320   alright (goods 
+0000f830: 6172 6520 6176 6169 6c61 626c 652c 2065  are available, e
+0000f840: 7463 2e29 2061 6e64 2074 6865 2062 6f74  tc.) and the bot
+0000f850: 2069 7320 7265 6164 7920 746f 2070 726f   is ready to pro
+0000f860: 6365 6564 2077 6974 6820 7468 6520 6f72  ceed with the or
+0000f870: 6465 722e 2055 7365 2046 616c 7365 2069  der. Use False i
+0000f880: 6620 7468 6572 6520 6172 6520 616e 7920  f there are any 
+0000f890: 7072 6f62 6c65 6d73 2e0a 2020 2020 3a70  problems..    :p
+0000f8a0: 6172 616d 2065 7272 6f72 5f6d 6573 7361  aram error_messa
+0000f8b0: 6765 3a20 5265 7175 6972 6564 2069 6620  ge: Required if 
+0000f8c0: 6f6b 2069 7320 4661 6c73 652e 2045 7272  ok is False. Err
+0000f8d0: 6f72 206d 6573 7361 6765 2069 6e20 6875  or message in hu
+0000f8e0: 6d61 6e20 7265 6164 6162 6c65 2066 6f72  man readable for
+0000f8f0: 6d20 7468 6174 2065 7870 6c61 696e 7320  m that explains 
+0000f900: 7468 6520 7265 6173 6f6e 2066 6f72 2066  the reason for f
+0000f910: 6169 6c75 7265 2074 6f20 7072 6f63 6565  ailure to procee
+0000f920: 6420 7769 7468 2074 6865 2063 6865 636b  d with the check
+0000f930: 6f75 7420 2865 2e67 2e20 2253 6f72 7279  out (e.g. "Sorry
+0000f940: 2c20 736f 6d65 626f 6479 206a 7573 7420  , somebody just 
+0000f950: 626f 7567 6874 2074 6865 206c 6173 7420  bought the last 
+0000f960: 6f66 206f 7572 2061 6d61 7a69 6e67 2062  of our amazing b
+0000f970: 6c61 636b 2054 2d73 6869 7274 7320 7768  lack T-shirts wh
+0000f980: 696c 6520 796f 7520 7765 7265 2062 7573  ile you were bus
+0000f990: 7920 6669 6c6c 696e 6720 6f75 7420 796f  y filling out yo
+0000f9a0: 7572 2070 6179 6d65 6e74 2064 6574 6169  ur payment detai
+0000f9b0: 6c73 2e20 506c 6561 7365 2063 686f 6f73  ls. Please choos
+0000f9c0: 6520 6120 6469 6666 6572 656e 7420 636f  e a different co
+0000f9d0: 6c6f 7220 6f72 2067 6172 6d65 6e74 2122  lor or garment!"
+0000f9e0: 292e 2054 656c 6567 7261 6d20 7769 6c6c  ). Telegram will
+0000f9f0: 2064 6973 706c 6179 2074 6869 7320 6d65   display this me
+0000fa00: 7373 6167 6520 746f 2074 6865 2075 7365  ssage to the use
+0000fa10: 722e 0a20 2020 203a 7265 7475 726e 3a0a  r..    :return:.
+0000fa20: 2020 2020 2222 220a 2020 2020 6d65 7468      """.    meth
+0000fa30: 6f64 5f75 726c 203d 2022 616e 7377 6572  od_url = "answer
+0000fa40: 5072 6543 6865 636b 6f75 7451 7565 7279  PreCheckoutQuery
+0000fa50: 220a 2020 2020 7061 796c 6f61 6420 3d20  ".    payload = 
+0000fa60: 7b22 7072 655f 6368 6563 6b6f 7574 5f71  {"pre_checkout_q
+0000fa70: 7565 7279 5f69 6422 3a20 7072 655f 6368  uery_id": pre_ch
+0000fa80: 6563 6b6f 7574 5f71 7565 7279 5f69 642c  eckout_query_id,
+0000fa90: 2022 6f6b 223a 206f 6b7d 0a20 2020 2069   "ok": ok}.    i
+0000faa0: 6620 6572 726f 725f 6d65 7373 6167 653a  f error_message:
+0000fab0: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+0000fac0: 5b22 6572 726f 725f 6d65 7373 6167 6522  ["error_message"
+0000fad0: 5d20 3d20 6572 726f 725f 6d65 7373 6167  ] = error_messag
+0000fae0: 650a 2020 2020 7265 7475 726e 2061 7761  e.    return awa
+0000faf0: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
+0000fb00: 6e2c 206d 6574 686f 645f 7572 6c2c 2070  n, method_url, p
+0000fb10: 6172 616d 733d 7061 796c 6f61 6429 0a0a  arams=payload)..
+0000fb20: 0a23 2049 6e6c 696e 6551 7565 7279 0a0a  .# InlineQuery..
+0000fb30: 0a61 7379 6e63 2064 6566 2061 6e73 7765  .async def answe
+0000fb40: 725f 6361 6c6c 6261 636b 5f71 7565 7279  r_callback_query
+0000fb50: 2874 6f6b 656e 2c20 6361 6c6c 6261 636b  (token, callback
+0000fb60: 5f71 7565 7279 5f69 642c 2074 6578 743d  _query_id, text=
+0000fb70: 4e6f 6e65 2c20 7368 6f77 5f61 6c65 7274  None, show_alert
+0000fb80: 3d4e 6f6e 652c 2075 726c 3d4e 6f6e 652c  =None, url=None,
+0000fb90: 2063 6163 6865 5f74 696d 653d 4e6f 6e65   cache_time=None
+0000fba0: 293a 0a20 2020 2022 2222 0a20 2020 2055  ):.    """.    U
+0000fbb0: 7365 2074 6869 7320 6d65 7468 6f64 2074  se this method t
+0000fbc0: 6f20 7365 6e64 2061 6e73 7765 7273 2074  o send answers t
+0000fbd0: 6f20 6361 6c6c 6261 636b 2071 7565 7269  o callback queri
+0000fbe0: 6573 2073 656e 7420 6672 6f6d 2069 6e6c  es sent from inl
+0000fbf0: 696e 6520 6b65 7962 6f61 7264 732e 2054  ine keyboards. T
+0000fc00: 6865 2061 6e73 7765 7220 7769 6c6c 2062  he answer will b
+0000fc10: 6520 6469 7370 6c61 7965 6420 746f 2074  e displayed to t
+0000fc20: 6865 2075 7365 7220 6173 2061 206e 6f74  he user as a not
+0000fc30: 6966 6963 6174 696f 6e20 6174 2074 6865  ification at the
+0000fc40: 2074 6f70 206f 6620 7468 6520 6368 6174   top of the chat
+0000fc50: 2073 6372 6565 6e20 6f72 2061 7320 616e   screen or as an
+0000fc60: 2061 6c65 7274 2e20 4f6e 2073 7563 6365   alert. On succe
+0000fc70: 7373 2c20 5472 7565 2069 7320 7265 7475  ss, True is retu
+0000fc80: 726e 6564 2e0a 2020 2020 416c 7465 726e  rned..    Altern
+0000fc90: 6174 6976 656c 792c 2074 6865 2075 7365  atively, the use
+0000fca0: 7220 6361 6e20 6265 2072 6564 6972 6563  r can be redirec
+0000fcb0: 7465 6420 746f 2074 6865 2073 7065 6369  ted to the speci
+0000fcc0: 6669 6564 2047 616d 6520 5552 4c2e 2046  fied Game URL. F
+0000fcd0: 6f72 2074 6869 7320 6f70 7469 6f6e 2074  or this option t
+0000fce0: 6f20 776f 726b 2c20 796f 7520 6d75 7374  o work, you must
+0000fcf0: 2066 6972 7374 2063 7265 6174 6520 6120   first create a 
+0000fd00: 6761 6d65 2066 6f72 2079 6f75 7220 626f  game for your bo
+0000fd10: 7420 7669 6120 426f 7446 6174 6865 7220  t via BotFather 
+0000fd20: 616e 6420 6163 6365 7074 2074 6865 2074  and accept the t
+0000fd30: 6572 6d73 2e20 4f74 6865 7277 6973 652c  erms. Otherwise,
+0000fd40: 2079 6f75 206d 6179 2075 7365 206c 696e   you may use lin
+0000fd50: 6b73 206c 696b 6520 7465 6c65 6772 616d  ks like telegram
+0000fd60: 2e6d 652f 796f 7572 5f62 6f74 3f73 7461  .me/your_bot?sta
+0000fd70: 7274 3d58 5858 5820 7468 6174 206f 7065  rt=XXXX that ope
+0000fd80: 6e20 796f 7572 2062 6f74 2077 6974 6820  n your bot with 
+0000fd90: 6120 7061 7261 6d65 7465 722e 0a20 2020  a parameter..   
+0000fda0: 203a 7061 7261 6d20 746f 6b65 6e3a 2042   :param token: B
+0000fdb0: 6f74 2773 2074 6f6b 656e 2028 796f 7520  ot's token (you 
+0000fdc0: 646f 6e27 7420 6e65 6564 2074 6f20 6669  don't need to fi
+0000fdd0: 6c6c 2074 6869 7329 0a20 2020 203a 7061  ll this).    :pa
+0000fde0: 7261 6d20 6361 6c6c 6261 636b 5f71 7565  ram callback_que
+0000fdf0: 7279 5f69 643a 2055 6e69 7175 6520 6964  ry_id: Unique id
+0000fe00: 656e 7469 6669 6572 2066 6f72 2074 6865  entifier for the
+0000fe10: 2071 7565 7279 2074 6f20 6265 2061 6e73   query to be ans
+0000fe20: 7765 7265 640a 2020 2020 3a70 6172 616d  wered.    :param
+0000fe30: 2074 6578 743a 2028 4f70 7469 6f6e 616c   text: (Optional
+0000fe40: 2920 5465 7874 206f 6620 7468 6520 6e6f  ) Text of the no
+0000fe50: 7469 6669 6361 7469 6f6e 2e20 4966 206e  tification. If n
+0000fe60: 6f74 2073 7065 6369 6669 6564 2c20 6e6f  ot specified, no
+0000fe70: 7468 696e 6720 7769 6c6c 2062 6520 7368  thing will be sh
+0000fe80: 6f77 6e20 746f 2074 6865 2075 7365 722c  own to the user,
+0000fe90: 2030 2d32 3030 2063 6861 7261 6374 6572   0-200 character
+0000fea0: 730a 2020 2020 3a70 6172 616d 2073 686f  s.    :param sho
+0000feb0: 775f 616c 6572 743a 2028 4f70 7469 6f6e  w_alert: (Option
+0000fec0: 616c 2920 4966 2074 7275 652c 2061 6e20  al) If true, an 
+0000fed0: 616c 6572 7420 7769 6c6c 2062 6520 7368  alert will be sh
+0000fee0: 6f77 6e20 6279 2074 6865 2063 6c69 656e  own by the clien
+0000fef0: 7420 696e 7374 6561 6420 6f66 2061 206e  t instead of a n
+0000ff00: 6f74 6966 6963 6174 696f 6e20 6174 2074  otification at t
+0000ff10: 6865 2074 6f70 206f 6620 7468 6520 6368  he top of the ch
+0000ff20: 6174 2073 6372 6565 6e2e 2044 6566 6175  at screen. Defau
+0000ff30: 6c74 7320 746f 2066 616c 7365 2e0a 2020  lts to false..  
+0000ff40: 2020 3a70 6172 616d 2075 726c 3a20 284f    :param url: (O
+0000ff50: 7074 696f 6e61 6c29 2055 524c 2074 6861  ptional) URL tha
+0000ff60: 7420 7769 6c6c 2062 6520 6f70 656e 6564  t will be opened
+0000ff70: 2062 7920 7468 6520 7573 6572 2773 2063   by the user's c
+0000ff80: 6c69 656e 742e 2049 6620 796f 7520 6861  lient. If you ha
+0000ff90: 7665 2063 7265 6174 6564 2061 2047 616d  ve created a Gam
+0000ffa0: 6520 616e 6420 6163 6365 7074 6564 2074  e and accepted t
+0000ffb0: 6865 2063 6f6e 6469 7469 6f6e 7320 7669  he conditions vi
+0000ffc0: 6120 4042 6f74 6661 7468 6572 2c20 7370  a @Botfather, sp
+0000ffd0: 6563 6966 7920 7468 6520 5552 4c20 7468  ecify the URL th
+0000ffe0: 6174 206f 7065 6e73 2079 6f75 7220 6761  at opens your ga
+0000fff0: 6d65 20e2 8093 206e 6f74 6520 7468 6174  me ... note that
+00010000: 2074 6869 7320 7769 6c6c 206f 6e6c 7920   this will only 
+00010010: 776f 726b 2069 6620 7468 6520 7175 6572  work if the quer
+00010020: 7920 636f 6d65 7320 6672 6f6d 2061 2063  y comes from a c
+00010030: 616c 6c62 6163 6b5f 6761 6d65 2062 7574  allback_game but
+00010040: 746f 6e2e 0a20 2020 204f 7468 6572 7769  ton..    Otherwi
+00010050: 7365 2c20 796f 7520 6d61 7920 7573 6520  se, you may use 
+00010060: 6c69 6e6b 7320 6c69 6b65 2074 656c 6567  links like teleg
+00010070: 7261 6d2e 6d65 2f79 6f75 725f 626f 743f  ram.me/your_bot?
+00010080: 7374 6172 743d 5858 5858 2074 6861 7420  start=XXXX that 
+00010090: 6f70 656e 2079 6f75 7220 626f 7420 7769  open your bot wi
+000100a0: 7468 2061 2070 6172 616d 6574 6572 2e0a  th a parameter..
+000100b0: 2020 2020 3a70 6172 616d 2063 6163 6865      :param cache
+000100c0: 5f74 696d 653a 2028 4f70 7469 6f6e 616c  _time: (Optional
+000100d0: 2920 5468 6520 6d61 7869 6d75 6d20 616d  ) The maximum am
+000100e0: 6f75 6e74 206f 6620 7469 6d65 2069 6e20  ount of time in 
+000100f0: 7365 636f 6e64 7320 7468 6174 2074 6865  seconds that the
+00010100: 2072 6573 756c 7420 6f66 2074 6865 2063   result of the c
+00010110: 616c 6c62 6163 6b20 7175 6572 7920 6d61  allback query ma
+00010120: 7920 6265 2063 6163 6865 6420 636c 6965  y be cached clie
+00010130: 6e74 2d73 6964 652e 2054 656c 6567 7261  nt-side. Telegra
+00010140: 6d20 6170 7073 2077 696c 6c20 7375 7070  m apps will supp
+00010150: 6f72 7420 6361 6368 696e 6720 7374 6172  ort caching star
+00010160: 7469 6e67 2069 6e20 7665 7273 696f 6e20  ting in version 
+00010170: 332e 3134 2e20 4465 6661 756c 7473 2074  3.14. Defaults t
+00010180: 6f20 302e 0a20 2020 203a 7265 7475 726e  o 0..    :return
+00010190: 3a0a 2020 2020 2222 220a 2020 2020 6d65  :.    """.    me
+000101a0: 7468 6f64 5f75 726c 203d 2022 616e 7377  thod_url = "answ
+000101b0: 6572 4361 6c6c 6261 636b 5175 6572 7922  erCallbackQuery"
+000101c0: 0a20 2020 2070 6179 6c6f 6164 203d 207b  .    payload = {
+000101d0: 2263 616c 6c62 6163 6b5f 7175 6572 795f  "callback_query_
+000101e0: 6964 223a 2063 616c 6c62 6163 6b5f 7175  id": callback_qu
+000101f0: 6572 795f 6964 7d0a 2020 2020 6966 2074  ery_id}.    if t
+00010200: 6578 743a 0a20 2020 2020 2020 2070 6179  ext:.        pay
+00010210: 6c6f 6164 5b22 7465 7874 225d 203d 2074  load["text"] = t
+00010220: 6578 740a 2020 2020 6966 2073 686f 775f  ext.    if show_
+00010230: 616c 6572 7420 6973 206e 6f74 204e 6f6e  alert is not Non
+00010240: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
+00010250: 6164 5b22 7368 6f77 5f61 6c65 7274 225d  ad["show_alert"]
+00010260: 203d 2073 686f 775f 616c 6572 740a 2020   = show_alert.  
+00010270: 2020 6966 2075 726c 3a0a 2020 2020 2020    if url:.      
+00010280: 2020 7061 796c 6f61 645b 2275 726c 225d    payload["url"]
+00010290: 203d 2075 726c 0a20 2020 2069 6620 6361   = url.    if ca
+000102a0: 6368 655f 7469 6d65 2069 7320 6e6f 7420  che_time is not 
+000102b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
+000102c0: 796c 6f61 645b 2263 6163 6865 5f74 696d  yload["cache_tim
+000102d0: 6522 5d20 3d20 6361 6368 655f 7469 6d65  e"] = cache_time
+000102e0: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
+000102f0: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
+00010300: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
+00010310: 7261 6d73 3d70 6179 6c6f 6164 2c20 6d65  rams=payload, me
+00010320: 7468 6f64 3d22 706f 7374 2229 0a0a 0a61  thod="post")...a
+00010330: 7379 6e63 2064 6566 2061 6e73 7765 725f  sync def answer_
+00010340: 696e 6c69 6e65 5f71 7565 7279 280a 2020  inline_query(.  
+00010350: 2020 746f 6b65 6e2c 0a20 2020 2069 6e6c    token,.    inl
+00010360: 696e 655f 7175 6572 795f 6964 2c0a 2020  ine_query_id,.  
+00010370: 2020 7265 7375 6c74 732c 0a20 2020 2063    results,.    c
+00010380: 6163 6865 5f74 696d 653d 4e6f 6e65 2c0a  ache_time=None,.
+00010390: 2020 2020 6973 5f70 6572 736f 6e61 6c3d      is_personal=
+000103a0: 4e6f 6e65 2c0a 2020 2020 6e65 7874 5f6f  None,.    next_o
+000103b0: 6666 7365 743d 4e6f 6e65 2c0a 2020 2020  ffset=None,.    
+000103c0: 7377 6974 6368 5f70 6d5f 7465 7874 3d4e  switch_pm_text=N
+000103d0: 6f6e 652c 0a20 2020 2073 7769 7463 685f  one,.    switch_
+000103e0: 706d 5f70 6172 616d 6574 6572 3d4e 6f6e  pm_parameter=Non
+000103f0: 652c 0a29 3a0a 2020 2020 6d65 7468 6f64  e,.):.    method
+00010400: 5f75 726c 203d 2022 616e 7377 6572 496e  _url = "answerIn
+00010410: 6c69 6e65 5175 6572 7922 0a20 2020 2070  lineQuery".    p
+00010420: 6179 6c6f 6164 203d 207b 0a20 2020 2020  ayload = {.     
+00010430: 2020 2022 696e 6c69 6e65 5f71 7565 7279     "inline_query
+00010440: 5f69 6422 3a20 696e 6c69 6e65 5f71 7565  _id": inline_que
+00010450: 7279 5f69 642c 0a20 2020 2020 2020 2022  ry_id,.        "
+00010460: 7265 7375 6c74 7322 3a20 6177 6169 7420  results": await 
+00010470: 5f63 6f6e 7665 7274 5f6c 6973 745f 6a73  _convert_list_js
+00010480: 6f6e 5f73 6572 6961 6c69 7a61 626c 6528  on_serializable(
+00010490: 7265 7375 6c74 7329 2c0a 2020 2020 7d0a  results),.    }.
+000104a0: 2020 2020 6966 2063 6163 6865 5f74 696d      if cache_tim
+000104b0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000104c0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+000104d0: 6361 6368 655f 7469 6d65 225d 203d 2063  cache_time"] = c
+000104e0: 6163 6865 5f74 696d 650a 2020 2020 6966  ache_time.    if
+000104f0: 2069 735f 7065 7273 6f6e 616c 2069 7320   is_personal is 
+00010500: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00010510: 2020 7061 796c 6f61 645b 2269 735f 7065    payload["is_pe
+00010520: 7273 6f6e 616c 225d 203d 2069 735f 7065  rsonal"] = is_pe
+00010530: 7273 6f6e 616c 0a20 2020 2069 6620 6e65  rsonal.    if ne
+00010540: 7874 5f6f 6666 7365 7420 6973 206e 6f74  xt_offset is not
+00010550: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
+00010560: 6179 6c6f 6164 5b22 6e65 7874 5f6f 6666  ayload["next_off
+00010570: 7365 7422 5d20 3d20 6e65 7874 5f6f 6666  set"] = next_off
+00010580: 7365 740a 2020 2020 6966 2073 7769 7463  set.    if switc
+00010590: 685f 706d 5f74 6578 743a 0a20 2020 2020  h_pm_text:.     
+000105a0: 2020 2070 6179 6c6f 6164 5b22 7377 6974     payload["swit
+000105b0: 6368 5f70 6d5f 7465 7874 225d 203d 2073  ch_pm_text"] = s
+000105c0: 7769 7463 685f 706d 5f74 6578 740a 2020  witch_pm_text.  
+000105d0: 2020 6966 2073 7769 7463 685f 706d 5f70    if switch_pm_p
+000105e0: 6172 616d 6574 6572 3a0a 2020 2020 2020  arameter:.      
+000105f0: 2020 7061 796c 6f61 645b 2273 7769 7463    payload["switc
+00010600: 685f 706d 5f70 6172 616d 6574 6572 225d  h_pm_parameter"]
+00010610: 203d 2073 7769 7463 685f 706d 5f70 6172   = switch_pm_par
+00010620: 616d 6574 6572 0a20 2020 2072 6574 7572  ameter.    retur
+00010630: 6e20 6177 6169 7420 5f72 6571 7565 7374  n await _request
+00010640: 2874 6f6b 656e 2c20 6d65 7468 6f64 5f75  (token, method_u
+00010650: 726c 2c20 7061 7261 6d73 3d70 6179 6c6f  rl, params=paylo
+00010660: 6164 2c20 6d65 7468 6f64 3d22 706f 7374  ad, method="post
+00010670: 2229 0a0a 0a61 7379 6e63 2064 6566 2067  ")...async def g
+00010680: 6574 5f73 7469 636b 6572 5f73 6574 2874  et_sticker_set(t
+00010690: 6f6b 656e 2c20 6e61 6d65 293a 0a20 2020  oken, name):.   
+000106a0: 206d 6574 686f 645f 7572 6c20 3d20 2267   method_url = "g
+000106b0: 6574 5374 6963 6b65 7253 6574 220a 2020  etStickerSet".  
+000106c0: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
+000106d0: 7265 7175 6573 7428 746f 6b65 6e2c 206d  request(token, m
+000106e0: 6574 686f 645f 7572 6c2c 2070 6172 616d  ethod_url, param
+000106f0: 733d 7b22 6e61 6d65 223a 206e 616d 657d  s={"name": name}
+00010700: 290a 0a0a 6173 796e 6320 6465 6620 7570  )...async def up
+00010710: 6c6f 6164 5f73 7469 636b 6572 5f66 696c  load_sticker_fil
+00010720: 6528 746f 6b65 6e2c 2075 7365 725f 6964  e(token, user_id
+00010730: 2c20 706e 675f 7374 6963 6b65 7229 3a0a  , png_sticker):.
+00010740: 2020 2020 6d65 7468 6f64 5f75 726c 203d      method_url =
+00010750: 2022 7570 6c6f 6164 5374 6963 6b65 7246   "uploadStickerF
+00010760: 696c 6522 0a20 2020 2070 6179 6c6f 6164  ile".    payload
+00010770: 203d 207b 2275 7365 725f 6964 223a 2075   = {"user_id": u
+00010780: 7365 725f 6964 7d0a 2020 2020 6669 6c65  ser_id}.    file
+00010790: 7320 3d20 7b22 706e 675f 7374 6963 6b65  s = {"png_sticke
+000107a0: 7222 3a20 706e 675f 7374 6963 6b65 727d  r": png_sticker}
+000107b0: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
+000107c0: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
+000107d0: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
+000107e0: 7261 6d73 3d70 6179 6c6f 6164 2c20 6669  rams=payload, fi
+000107f0: 6c65 733d 6669 6c65 732c 206d 6574 686f  les=files, metho
+00010800: 643d 2270 6f73 7422 290a 0a0a 6173 796e  d="post")...asyn
+00010810: 6320 6465 6620 6372 6561 7465 5f6e 6577  c def create_new
+00010820: 5f73 7469 636b 6572 5f73 6574 280a 2020  _sticker_set(.  
+00010830: 2020 746f 6b65 6e2c 0a20 2020 2075 7365    token,.    use
+00010840: 725f 6964 2c0a 2020 2020 6e61 6d65 2c0a  r_id,.    name,.
+00010850: 2020 2020 7469 746c 652c 0a20 2020 2065      title,.    e
+00010860: 6d6f 6a69 732c 0a20 2020 2070 6e67 5f73  mojis,.    png_s
+00010870: 7469 636b 6572 2c0a 2020 2020 7467 735f  ticker,.    tgs_
+00010880: 7374 6963 6b65 722c 0a20 2020 206d 6173  sticker,.    mas
+00010890: 6b5f 706f 7369 7469 6f6e 3d4e 6f6e 652c  k_position=None,
+000108a0: 0a20 2020 2077 6562 6d5f 7374 6963 6b65  .    webm_sticke
+000108b0: 723d 4e6f 6e65 2c0a 2020 2020 7374 6963  r=None,.    stic
+000108c0: 6b65 725f 7479 7065 3d4e 6f6e 652c 0a29  ker_type=None,.)
+000108d0: 3a0a 2020 2020 726f 7574 6520 3d20 2263  :.    route = "c
+000108e0: 7265 6174 654e 6577 5374 6963 6b65 7253  reateNewStickerS
+000108f0: 6574 220a 2020 2020 7061 796c 6f61 6420  et".    payload 
+00010900: 3d20 7b22 7573 6572 5f69 6422 3a20 7573  = {"user_id": us
+00010910: 6572 5f69 642c 2022 6e61 6d65 223a 206e  er_id, "name": n
+00010920: 616d 652c 2022 7469 746c 6522 3a20 7469  ame, "title": ti
+00010930: 746c 652c 2022 656d 6f6a 6973 223a 2065  tle, "emojis": e
+00010940: 6d6f 6a69 737d 0a20 2020 2069 6620 706e  mojis}.    if pn
+00010950: 675f 7374 6963 6b65 723a 0a20 2020 2020  g_sticker:.     
+00010960: 2020 2073 7479 7065 203d 2022 706e 675f     stype = "png_
+00010970: 7374 6963 6b65 7222 0a20 2020 2065 6c69  sticker".    eli
+00010980: 6620 7765 626d 5f73 7469 636b 6572 3a0a  f webm_sticker:.
+00010990: 2020 2020 2020 2020 7374 7970 6520 3d20          stype = 
+000109a0: 2277 6562 6d5f 7374 6963 6b65 7222 0a20  "webm_sticker". 
+000109b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000109c0: 2073 7479 7065 203d 2022 7467 735f 7374   stype = "tgs_st
+000109d0: 6963 6b65 7222 0a20 2020 2073 7469 636b  icker".    stick
+000109e0: 6572 203d 2070 6e67 5f73 7469 636b 6572  er = png_sticker
+000109f0: 206f 7220 7467 735f 7374 6963 6b65 7220   or tgs_sticker 
+00010a00: 6f72 2077 6562 6d5f 7374 6963 6b65 720a  or webm_sticker.
+00010a10: 2020 2020 6669 6c65 7320 3d20 4e6f 6e65      files = None
+00010a20: 0a20 2020 2069 6620 6e6f 7420 7574 696c  .    if not util
+00010a30: 2e69 735f 7374 7269 6e67 2873 7469 636b  .is_string(stick
+00010a40: 6572 293a 0a20 2020 2020 2020 2066 696c  er):.        fil
+00010a50: 6573 203d 207b 7374 7970 653a 2073 7469  es = {stype: sti
+00010a60: 636b 6572 7d0a 2020 2020 656c 7365 3a0a  cker}.    else:.
+00010a70: 2020 2020 2020 2020 7061 796c 6f61 645b          payload[
+00010a80: 7374 7970 655d 203d 2073 7469 636b 6572  stype] = sticker
+00010a90: 0a20 2020 2069 6620 6d61 736b 5f70 6f73  .    if mask_pos
+00010aa0: 6974 696f 6e3a 0a20 2020 2020 2020 2070  ition:.        p
+00010ab0: 6179 6c6f 6164 5b22 6d61 736b 5f70 6f73  ayload["mask_pos
+00010ac0: 6974 696f 6e22 5d20 3d20 6d61 736b 5f70  ition"] = mask_p
+00010ad0: 6f73 6974 696f 6e2e 746f 5f6a 736f 6e28  osition.to_json(
+00010ae0: 290a 2020 2020 6966 2077 6562 6d5f 7374  ).    if webm_st
+00010af0: 6963 6b65 723a 0a20 2020 2020 2020 2070  icker:.        p
+00010b00: 6179 6c6f 6164 5b22 7765 626d 5f73 7469  ayload["webm_sti
+00010b10: 636b 6572 225d 203d 2077 6562 6d5f 7374  cker"] = webm_st
+00010b20: 6963 6b65 720a 2020 2020 6966 2073 7469  icker.    if sti
+00010b30: 636b 6572 5f74 7970 653a 0a20 2020 2020  cker_type:.     
+00010b40: 2020 2070 6179 6c6f 6164 5b22 7374 6963     payload["stic
+00010b50: 6b65 725f 7479 7065 225d 203d 2073 7469  ker_type"] = sti
+00010b60: 636b 6572 5f74 7970 650a 2020 2020 7265  cker_type.    re
+00010b70: 7475 726e 2061 7761 6974 205f 7265 7175  turn await _requ
+00010b80: 6573 7428 746f 6b65 6e2c 2072 6f75 7465  est(token, route
+00010b90: 2c20 7061 7261 6d73 3d70 6179 6c6f 6164  , params=payload
+00010ba0: 2c20 6669 6c65 733d 6669 6c65 732c 206d  , files=files, m
+00010bb0: 6574 686f 643d 2270 6f73 7422 290a 0a0a  ethod="post")...
+00010bc0: 6173 796e 6320 6465 6620 6164 645f 7374  async def add_st
+00010bd0: 6963 6b65 725f 746f 5f73 6574 2874 6f6b  icker_to_set(tok
+00010be0: 656e 2c20 7573 6572 5f69 642c 206e 616d  en, user_id, nam
+00010bf0: 652c 2065 6d6f 6a69 732c 2070 6e67 5f73  e, emojis, png_s
+00010c00: 7469 636b 6572 2c20 7467 735f 7374 6963  ticker, tgs_stic
+00010c10: 6b65 722c 206d 6173 6b5f 706f 7369 7469  ker, mask_positi
+00010c20: 6f6e 2c20 7765 626d 5f73 7469 636b 6572  on, webm_sticker
+00010c30: 293a 0a20 2020 206d 6574 686f 645f 7572  ):.    method_ur
+00010c40: 6c20 3d20 2261 6464 5374 6963 6b65 7254  l = "addStickerT
+00010c50: 6f53 6574 220a 2020 2020 7061 796c 6f61  oSet".    payloa
+00010c60: 6420 3d20 7b22 7573 6572 5f69 6422 3a20  d = {"user_id": 
+00010c70: 7573 6572 5f69 642c 2022 6e61 6d65 223a  user_id, "name":
+00010c80: 206e 616d 652c 2022 656d 6f6a 6973 223a   name, "emojis":
+00010c90: 2065 6d6f 6a69 737d 0a20 2020 2069 6620   emojis}.    if 
+00010ca0: 706e 675f 7374 6963 6b65 723a 0a20 2020  png_sticker:.   
+00010cb0: 2020 2020 2073 7479 7065 203d 2022 706e       stype = "pn
+00010cc0: 675f 7374 6963 6b65 7222 0a20 2020 2065  g_sticker".    e
+00010cd0: 6c69 6620 7765 626d 5f73 7469 636b 6572  lif webm_sticker
+00010ce0: 3a0a 2020 2020 2020 2020 7374 7970 6520  :.        stype 
+00010cf0: 3d20 2277 6562 6d5f 7374 6963 6b65 7222  = "webm_sticker"
+00010d00: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00010d10: 2020 2073 7479 7065 203d 2022 7467 735f     stype = "tgs_
+00010d20: 7374 6963 6b65 7222 0a20 2020 2066 696c  sticker".    fil
+00010d30: 6573 203d 204e 6f6e 650a 2020 2020 7374  es = None.    st
+00010d40: 6963 6b65 7220 3d20 706e 675f 7374 6963  icker = png_stic
+00010d50: 6b65 7220 6f72 2074 6773 5f73 7469 636b  ker or tgs_stick
+00010d60: 6572 206f 7220 7765 626d 5f73 7469 636b  er or webm_stick
+00010d70: 6572 0a0a 2020 2020 6966 206e 6f74 2075  er..    if not u
+00010d80: 7469 6c2e 6973 5f73 7472 696e 6728 7374  til.is_string(st
+00010d90: 6963 6b65 7229 3a0a 2020 2020 2020 2020  icker):.        
+00010da0: 6669 6c65 7320 3d20 7b73 7479 7065 3a20  files = {stype: 
+00010db0: 7374 6963 6b65 727d 0a20 2020 2065 6c73  sticker}.    els
+00010dc0: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
+00010dd0: 6164 5b73 7479 7065 5d20 3d20 7374 6963  ad[stype] = stic
+00010de0: 6b65 720a 2020 2020 6966 206d 6173 6b5f  ker.    if mask_
+00010df0: 706f 7369 7469 6f6e 3a0a 2020 2020 2020  position:.      
+00010e00: 2020 7061 796c 6f61 645b 226d 6173 6b5f    payload["mask_
+00010e10: 706f 7369 7469 6f6e 225d 203d 206d 6173  position"] = mas
+00010e20: 6b5f 706f 7369 7469 6f6e 2e74 6f5f 6a73  k_position.to_js
+00010e30: 6f6e 2829 0a0a 2020 2020 6966 2077 6562  on()..    if web
+00010e40: 6d5f 7374 6963 6b65 723a 0a20 2020 2020  m_sticker:.     
+00010e50: 2020 2070 6179 6c6f 6164 5b22 7765 626d     payload["webm
+00010e60: 5f73 7469 636b 6572 225d 203d 2077 6562  _sticker"] = web
+00010e70: 6d5f 7374 6963 6b65 720a 2020 2020 7265  m_sticker.    re
+00010e80: 7475 726e 2061 7761 6974 205f 7265 7175  turn await _requ
+00010e90: 6573 7428 746f 6b65 6e2c 206d 6574 686f  est(token, metho
+00010ea0: 645f 7572 6c2c 2070 6172 616d 733d 7061  d_url, params=pa
+00010eb0: 796c 6f61 642c 2066 696c 6573 3d66 696c  yload, files=fil
+00010ec0: 6573 2c20 6d65 7468 6f64 3d22 706f 7374  es, method="post
+00010ed0: 2229 0a0a 0a61 7379 6e63 2064 6566 2073  ")...async def s
+00010ee0: 6574 5f73 7469 636b 6572 5f70 6f73 6974  et_sticker_posit
+00010ef0: 696f 6e5f 696e 5f73 6574 2874 6f6b 656e  ion_in_set(token
+00010f00: 2c20 7374 6963 6b65 722c 2070 6f73 6974  , sticker, posit
+00010f10: 696f 6e29 3a0a 2020 2020 6d65 7468 6f64  ion):.    method
+00010f20: 5f75 726c 203d 2022 7365 7453 7469 636b  _url = "setStick
+00010f30: 6572 506f 7369 7469 6f6e 496e 5365 7422  erPositionInSet"
+00010f40: 0a20 2020 2070 6179 6c6f 6164 203d 207b  .    payload = {
+00010f50: 2273 7469 636b 6572 223a 2073 7469 636b  "sticker": stick
+00010f60: 6572 2c20 2270 6f73 6974 696f 6e22 3a20  er, "position": 
+00010f70: 706f 7369 7469 6f6e 7d0a 2020 2020 7265  position}.    re
+00010f80: 7475 726e 2061 7761 6974 205f 7265 7175  turn await _requ
+00010f90: 6573 7428 746f 6b65 6e2c 206d 6574 686f  est(token, metho
+00010fa0: 645f 7572 6c2c 2070 6172 616d 733d 7061  d_url, params=pa
+00010fb0: 796c 6f61 642c 206d 6574 686f 643d 2270  yload, method="p
+00010fc0: 6f73 7422 290a 0a0a 6173 796e 6320 6465  ost")...async de
+00010fd0: 6620 6465 6c65 7465 5f73 7469 636b 6572  f delete_sticker
+00010fe0: 5f66 726f 6d5f 7365 7428 746f 6b65 6e2c  _from_set(token,
+00010ff0: 2073 7469 636b 6572 293a 0a20 2020 206d   sticker):.    m
+00011000: 6574 686f 645f 7572 6c20 3d20 2264 656c  ethod_url = "del
+00011010: 6574 6553 7469 636b 6572 4672 6f6d 5365  eteStickerFromSe
+00011020: 7422 0a20 2020 2070 6179 6c6f 6164 203d  t".    payload =
+00011030: 207b 2273 7469 636b 6572 223a 2073 7469   {"sticker": sti
+00011040: 636b 6572 7d0a 2020 2020 7265 7475 726e  cker}.    return
+00011050: 2061 7761 6974 205f 7265 7175 6573 7428   await _request(
+00011060: 746f 6b65 6e2c 206d 6574 686f 645f 7572  token, method_ur
+00011070: 6c2c 2070 6172 616d 733d 7061 796c 6f61  l, params=payloa
+00011080: 642c 206d 6574 686f 643d 2270 6f73 7422  d, method="post"
+00011090: 290a 0a0a 6173 796e 6320 6465 6620 6372  )...async def cr
+000110a0: 6561 7465 5f69 6e76 6f69 6365 5f6c 696e  eate_invoice_lin
+000110b0: 6b28 0a20 2020 2074 6f6b 656e 2c0a 2020  k(.    token,.  
+000110c0: 2020 7469 746c 652c 0a20 2020 2064 6573    title,.    des
+000110d0: 6372 6970 7469 6f6e 2c0a 2020 2020 7061  cription,.    pa
+000110e0: 796c 6f61 642c 0a20 2020 2070 726f 7669  yload,.    provi
+000110f0: 6465 725f 746f 6b65 6e2c 0a20 2020 2063  der_token,.    c
+00011100: 7572 7265 6e63 792c 0a20 2020 2070 7269  urrency,.    pri
+00011110: 6365 732c 0a20 2020 206d 6178 5f74 6970  ces,.    max_tip
+00011120: 5f61 6d6f 756e 743d 4e6f 6e65 2c0a 2020  _amount=None,.  
+00011130: 2020 7375 6767 6573 7465 645f 7469 705f    suggested_tip_
+00011140: 616d 6f75 6e74 733d 4e6f 6e65 2c0a 2020  amounts=None,.  
+00011150: 2020 7072 6f76 6964 6572 5f64 6174 613d    provider_data=
+00011160: 4e6f 6e65 2c0a 2020 2020 7068 6f74 6f5f  None,.    photo_
+00011170: 7572 6c3d 4e6f 6e65 2c0a 2020 2020 7068  url=None,.    ph
+00011180: 6f74 6f5f 7369 7a65 3d4e 6f6e 652c 0a20  oto_size=None,. 
+00011190: 2020 2070 686f 746f 5f77 6964 7468 3d4e     photo_width=N
+000111a0: 6f6e 652c 0a20 2020 2070 686f 746f 5f68  one,.    photo_h
+000111b0: 6569 6768 743d 4e6f 6e65 2c0a 2020 2020  eight=None,.    
+000111c0: 6e65 6564 5f6e 616d 653d 4e6f 6e65 2c0a  need_name=None,.
+000111d0: 2020 2020 6e65 6564 5f70 686f 6e65 5f6e      need_phone_n
+000111e0: 756d 6265 723d 4e6f 6e65 2c0a 2020 2020  umber=None,.    
+000111f0: 6e65 6564 5f65 6d61 696c 3d4e 6f6e 652c  need_email=None,
+00011200: 0a20 2020 206e 6565 645f 7368 6970 7069  .    need_shippi
+00011210: 6e67 5f61 6464 7265 7373 3d4e 6f6e 652c  ng_address=None,
+00011220: 0a20 2020 2073 656e 645f 7068 6f6e 655f  .    send_phone_
+00011230: 6e75 6d62 6572 5f74 6f5f 7072 6f76 6964  number_to_provid
+00011240: 6572 3d4e 6f6e 652c 0a20 2020 2073 656e  er=None,.    sen
+00011250: 645f 656d 6169 6c5f 746f 5f70 726f 7669  d_email_to_provi
+00011260: 6465 723d 4e6f 6e65 2c0a 2020 2020 6973  der=None,.    is
+00011270: 5f66 6c65 7869 626c 653d 4e6f 6e65 2c0a  _flexible=None,.
+00011280: 293a 0a20 2020 2072 6f75 7465 203d 2072  ):.    route = r
+00011290: 2263 7265 6174 6549 6e76 6f69 6365 4c69  "createInvoiceLi
+000112a0: 6e6b 220a 2020 2020 7061 796c 6f61 6420  nk".    payload 
+000112b0: 3d20 7b0a 2020 2020 2020 2020 2274 6974  = {.        "tit
+000112c0: 6c65 223a 2074 6974 6c65 2c0a 2020 2020  le": title,.    
+000112d0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+000112e0: 223a 2064 6573 6372 6970 7469 6f6e 2c0a  ": description,.
+000112f0: 2020 2020 2020 2020 2270 6179 6c6f 6164          "payload
+00011300: 223a 2070 6179 6c6f 6164 2c0a 2020 2020  ": payload,.    
+00011310: 2020 2020 2270 726f 7669 6465 725f 746f      "provider_to
+00011320: 6b65 6e22 3a20 7072 6f76 6964 6572 5f74  ken": provider_t
+00011330: 6f6b 656e 2c0a 2020 2020 2020 2020 2263  oken,.        "c
+00011340: 7572 7265 6e63 7922 3a20 6375 7272 656e  urrency": curren
+00011350: 6379 2c0a 2020 2020 2020 2020 2270 7269  cy,.        "pri
+00011360: 6365 7322 3a20 6177 6169 7420 5f63 6f6e  ces": await _con
+00011370: 7665 7274 5f6c 6973 745f 6a73 6f6e 5f73  vert_list_json_s
+00011380: 6572 6961 6c69 7a61 626c 6528 7072 6963  erializable(pric
+00011390: 6573 292c 0a20 2020 207d 0a20 2020 2069  es),.    }.    i
+000113a0: 6620 6d61 785f 7469 705f 616d 6f75 6e74  f max_tip_amount
+000113b0: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+000113c0: 645b 226d 6178 5f74 6970 5f61 6d6f 756e  d["max_tip_amoun
+000113d0: 7422 5d20 3d20 6d61 785f 7469 705f 616d  t"] = max_tip_am
+000113e0: 6f75 6e74 0a20 2020 2069 6620 7375 6767  ount.    if sugg
+000113f0: 6573 7465 645f 7469 705f 616d 6f75 6e74  ested_tip_amount
+00011400: 733a 0a20 2020 2020 2020 2070 6179 6c6f  s:.        paylo
+00011410: 6164 5b22 7375 6767 6573 7465 645f 7469  ad["suggested_ti
+00011420: 705f 616d 6f75 6e74 7322 5d20 3d20 6a73  p_amounts"] = js
+00011430: 6f6e 2e64 756d 7073 2873 7567 6765 7374  on.dumps(suggest
+00011440: 6564 5f74 6970 5f61 6d6f 756e 7473 290a  ed_tip_amounts).
+00011450: 2020 2020 6966 2070 726f 7669 6465 725f      if provider_
+00011460: 6461 7461 3a0a 2020 2020 2020 2020 7061  data:.        pa
+00011470: 796c 6f61 645b 2270 726f 7669 6465 725f  yload["provider_
+00011480: 6461 7461 225d 203d 2070 726f 7669 6465  data"] = provide
+00011490: 725f 6461 7461 0a20 2020 2069 6620 7068  r_data.    if ph
+000114a0: 6f74 6f5f 7572 6c3a 0a20 2020 2020 2020  oto_url:.       
+000114b0: 2070 6179 6c6f 6164 5b22 7068 6f74 6f5f   payload["photo_
+000114c0: 7572 6c22 5d20 3d20 7068 6f74 6f5f 7572  url"] = photo_ur
+000114d0: 6c0a 2020 2020 6966 2070 686f 746f 5f73  l.    if photo_s
+000114e0: 697a 653a 0a20 2020 2020 2020 2070 6179  ize:.        pay
+000114f0: 6c6f 6164 5b22 7068 6f74 6f5f 7369 7a65  load["photo_size
+00011500: 225d 203d 2070 686f 746f 5f73 697a 650a  "] = photo_size.
+00011510: 2020 2020 6966 2070 686f 746f 5f77 6964      if photo_wid
+00011520: 7468 3a0a 2020 2020 2020 2020 7061 796c  th:.        payl
+00011530: 6f61 645b 2270 686f 746f 5f77 6964 7468  oad["photo_width
+00011540: 225d 203d 2070 686f 746f 5f77 6964 7468  "] = photo_width
+00011550: 0a20 2020 2069 6620 7068 6f74 6f5f 6865  .    if photo_he
+00011560: 6967 6874 3a0a 2020 2020 2020 2020 7061  ight:.        pa
+00011570: 796c 6f61 645b 2270 686f 746f 5f68 6569  yload["photo_hei
+00011580: 6768 7422 5d20 3d20 7068 6f74 6f5f 6865  ght"] = photo_he
+00011590: 6967 6874 0a20 2020 2069 6620 6e65 6564  ight.    if need
+000115a0: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
+000115b0: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
+000115c0: 6164 5b22 6e65 6564 5f6e 616d 6522 5d20  ad["need_name"] 
+000115d0: 3d20 6e65 6564 5f6e 616d 650a 2020 2020  = need_name.    
+000115e0: 6966 206e 6565 645f 7068 6f6e 655f 6e75  if need_phone_nu
+000115f0: 6d62 6572 2069 7320 6e6f 7420 4e6f 6e65  mber is not None
+00011600: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+00011610: 645b 226e 6565 645f 7068 6f6e 655f 6e75  d["need_phone_nu
+00011620: 6d62 6572 225d 203d 206e 6565 645f 7068  mber"] = need_ph
+00011630: 6f6e 655f 6e75 6d62 6572 0a20 2020 2069  one_number.    i
+00011640: 6620 6e65 6564 5f65 6d61 696c 2069 7320  f need_email is 
+00011650: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00011660: 2020 7061 796c 6f61 645b 226e 6565 645f    payload["need_
+00011670: 656d 6169 6c22 5d20 3d20 6e65 6564 5f65  email"] = need_e
+00011680: 6d61 696c 0a20 2020 2069 6620 6e65 6564  mail.    if need
+00011690: 5f73 6869 7070 696e 675f 6164 6472 6573  _shipping_addres
+000116a0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+000116b0: 2020 2020 2020 2070 6179 6c6f 6164 5b22         payload["
+000116c0: 6e65 6564 5f73 6869 7070 696e 675f 6164  need_shipping_ad
+000116d0: 6472 6573 7322 5d20 3d20 6e65 6564 5f73  dress"] = need_s
+000116e0: 6869 7070 696e 675f 6164 6472 6573 730a  hipping_address.
+000116f0: 2020 2020 6966 2073 656e 645f 7068 6f6e      if send_phon
+00011700: 655f 6e75 6d62 6572 5f74 6f5f 7072 6f76  e_number_to_prov
+00011710: 6964 6572 2069 7320 6e6f 7420 4e6f 6e65  ider is not None
+00011720: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+00011730: 645b 2273 656e 645f 7068 6f6e 655f 6e75  d["send_phone_nu
+00011740: 6d62 6572 5f74 6f5f 7072 6f76 6964 6572  mber_to_provider
+00011750: 225d 203d 2073 656e 645f 7068 6f6e 655f  "] = send_phone_
+00011760: 6e75 6d62 6572 5f74 6f5f 7072 6f76 6964  number_to_provid
+00011770: 6572 0a20 2020 2069 6620 7365 6e64 5f65  er.    if send_e
+00011780: 6d61 696c 5f74 6f5f 7072 6f76 6964 6572  mail_to_provider
+00011790: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000117a0: 2020 2020 2020 7061 796c 6f61 645b 2273        payload["s
+000117b0: 656e 645f 656d 6169 6c5f 746f 5f70 726f  end_email_to_pro
+000117c0: 7669 6465 7222 5d20 3d20 7365 6e64 5f65  vider"] = send_e
+000117d0: 6d61 696c 5f74 6f5f 7072 6f76 6964 6572  mail_to_provider
+000117e0: 0a20 2020 2069 6620 6973 5f66 6c65 7869  .    if is_flexi
+000117f0: 626c 6520 6973 206e 6f74 204e 6f6e 653a  ble is not None:
+00011800: 0a20 2020 2020 2020 2070 6179 6c6f 6164  .        payload
+00011810: 5b22 6973 5f66 6c65 7869 626c 6522 5d20  ["is_flexible"] 
+00011820: 3d20 6973 5f66 6c65 7869 626c 650a 2020  = is_flexible.  
+00011830: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
+00011840: 7265 7175 6573 7428 746f 6b65 6e2c 2072  request(token, r
+00011850: 6f75 7465 2c20 7061 7261 6d73 3d70 6179  oute, params=pay
+00011860: 6c6f 6164 2c20 6d65 7468 6f64 3d22 706f  load, method="po
+00011870: 7374 2229 0a0a 0a23 206e 6f69 6e73 7065  st")...# noinspe
+00011880: 6374 696f 6e20 5079 5368 6164 6f77 696e  ction PyShadowin
+00011890: 6742 7569 6c74 696e 730a 6173 796e 6320  gBuiltins.async 
+000118a0: 6465 6620 7365 6e64 5f70 6f6c 6c28 0a20  def send_poll(. 
+000118b0: 2020 2074 6f6b 656e 2c0a 2020 2020 6368     token,.    ch
+000118c0: 6174 5f69 642c 0a20 2020 2071 7565 7374  at_id,.    quest
+000118d0: 696f 6e2c 0a20 2020 206f 7074 696f 6e73  ion,.    options
+000118e0: 2c0a 2020 2020 6973 5f61 6e6f 6e79 6d6f  ,.    is_anonymo
+000118f0: 7573 3d4e 6f6e 652c 0a20 2020 2074 7970  us=None,.    typ
+00011900: 653d 4e6f 6e65 2c0a 2020 2020 616c 6c6f  e=None,.    allo
+00011910: 7773 5f6d 756c 7469 706c 655f 616e 7377  ws_multiple_answ
+00011920: 6572 733d 4e6f 6e65 2c0a 2020 2020 636f  ers=None,.    co
+00011930: 7272 6563 745f 6f70 7469 6f6e 5f69 643d  rrect_option_id=
+00011940: 4e6f 6e65 2c0a 2020 2020 6578 706c 616e  None,.    explan
+00011950: 6174 696f 6e3d 4e6f 6e65 2c0a 2020 2020  ation=None,.    
+00011960: 6578 706c 616e 6174 696f 6e5f 7061 7273  explanation_pars
+00011970: 655f 6d6f 6465 3d4e 6f6e 652c 0a20 2020  e_mode=None,.   
+00011980: 206f 7065 6e5f 7065 7269 6f64 3d4e 6f6e   open_period=Non
+00011990: 652c 0a20 2020 2063 6c6f 7365 5f64 6174  e,.    close_dat
+000119a0: 653d 4e6f 6e65 2c0a 2020 2020 6973 5f63  e=None,.    is_c
+000119b0: 6c6f 7365 643d 4e6f 6e65 2c0a 2020 2020  losed=None,.    
+000119c0: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+000119d0: 7469 6f6e 3d46 616c 7365 2c0a 2020 2020  tion=False,.    
+000119e0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+000119f0: 5f69 643d 4e6f 6e65 2c0a 2020 2020 616c  _id=None,.    al
+00011a00: 6c6f 775f 7365 6e64 696e 675f 7769 7468  low_sending_with
+00011a10: 6f75 745f 7265 706c 793d 4e6f 6e65 2c0a  out_reply=None,.
+00011a20: 2020 2020 7265 706c 795f 6d61 726b 7570      reply_markup
+00011a30: 3d4e 6f6e 652c 0a20 2020 2074 696d 656f  =None,.    timeo
+00011a40: 7574 3d4e 6f6e 652c 0a20 2020 2065 7870  ut=None,.    exp
+00011a50: 6c61 6e61 7469 6f6e 5f65 6e74 6974 6965  lanation_entitie
+00011a60: 733d 4e6f 6e65 2c0a 2020 2020 7072 6f74  s=None,.    prot
+00011a70: 6563 745f 636f 6e74 656e 743d 4e6f 6e65  ect_content=None
+00011a80: 2c0a 2020 2020 6d65 7373 6167 655f 7468  ,.    message_th
+00011a90: 7265 6164 5f69 643a 204f 7074 696f 6e61  read_id: Optiona
+00011aa0: 6c5b 696e 745d 203d 204e 6f6e 652c 0a29  l[int] = None,.)
+00011ab0: 3a0a 2020 2020 6d65 7468 6f64 5f75 726c  :.    method_url
+00011ac0: 203d 2072 2273 656e 6450 6f6c 6c22 0a20   = r"sendPoll". 
+00011ad0: 2020 2070 6179 6c6f 6164 203d 207b 0a20     payload = {. 
+00011ae0: 2020 2020 2020 2022 6368 6174 5f69 6422         "chat_id"
+00011af0: 3a20 7374 7228 6368 6174 5f69 6429 2c0a  : str(chat_id),.
+00011b00: 2020 2020 2020 2020 2271 7565 7374 696f          "questio
+00011b10: 6e22 3a20 7175 6573 7469 6f6e 2c0a 2020  n": question,.  
+00011b20: 2020 2020 2020 226f 7074 696f 6e73 223a        "options":
+00011b30: 206a 736f 6e2e 6475 6d70 7328 6177 6169   json.dumps(awai
+00011b40: 7420 5f63 6f6e 7665 7274 5f70 6f6c 6c5f  t _convert_poll_
+00011b50: 6f70 7469 6f6e 7328 6f70 7469 6f6e 7329  options(options)
+00011b60: 292c 0a20 2020 207d 0a0a 2020 2020 6966  ),.    }..    if
+00011b70: 2069 735f 616e 6f6e 796d 6f75 7320 6973   is_anonymous is
+00011b80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00011b90: 2020 2070 6179 6c6f 6164 5b22 6973 5f61     payload["is_a
+00011ba0: 6e6f 6e79 6d6f 7573 225d 203d 2069 735f  nonymous"] = is_
+00011bb0: 616e 6f6e 796d 6f75 730a 2020 2020 6966  anonymous.    if
+00011bc0: 2074 7970 6520 6973 206e 6f74 204e 6f6e   type is not Non
+00011bd0: 653a 0a20 2020 2020 2020 2070 6179 6c6f  e:.        paylo
+00011be0: 6164 5b22 7479 7065 225d 203d 2074 7970  ad["type"] = typ
+00011bf0: 650a 2020 2020 6966 2061 6c6c 6f77 735f  e.    if allows_
+00011c00: 6d75 6c74 6970 6c65 5f61 6e73 7765 7273  multiple_answers
+00011c10: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00011c20: 2020 2020 2020 7061 796c 6f61 645b 2261        payload["a
+00011c30: 6c6c 6f77 735f 6d75 6c74 6970 6c65 5f61  llows_multiple_a
+00011c40: 6e73 7765 7273 225d 203d 2061 6c6c 6f77  nswers"] = allow
+00011c50: 735f 6d75 6c74 6970 6c65 5f61 6e73 7765  s_multiple_answe
+00011c60: 7273 0a20 2020 2069 6620 636f 7272 6563  rs.    if correc
+00011c70: 745f 6f70 7469 6f6e 5f69 6420 6973 206e  t_option_id is n
+00011c80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00011c90: 2070 6179 6c6f 6164 5b22 636f 7272 6563   payload["correc
+00011ca0: 745f 6f70 7469 6f6e 5f69 6422 5d20 3d20  t_option_id"] = 
+00011cb0: 636f 7272 6563 745f 6f70 7469 6f6e 5f69  correct_option_i
+00011cc0: 640a 2020 2020 6966 2065 7870 6c61 6e61  d.    if explana
+00011cd0: 7469 6f6e 2069 7320 6e6f 7420 4e6f 6e65  tion is not None
+00011ce0: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+00011cf0: 645b 2265 7870 6c61 6e61 7469 6f6e 225d  d["explanation"]
+00011d00: 203d 2065 7870 6c61 6e61 7469 6f6e 0a20   = explanation. 
+00011d10: 2020 2069 6620 6578 706c 616e 6174 696f     if explanatio
+00011d20: 6e5f 7061 7273 655f 6d6f 6465 2069 7320  n_parse_mode is 
+00011d30: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00011d40: 2020 7061 796c 6f61 645b 2265 7870 6c61    payload["expla
+00011d50: 6e61 7469 6f6e 5f70 6172 7365 5f6d 6f64  nation_parse_mod
+00011d60: 6522 5d20 3d20 6578 706c 616e 6174 696f  e"] = explanatio
+00011d70: 6e5f 7061 7273 655f 6d6f 6465 0a20 2020  n_parse_mode.   
+00011d80: 2069 6620 6f70 656e 5f70 6572 696f 6420   if open_period 
+00011d90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00011da0: 2020 2020 2070 6179 6c6f 6164 5b22 6f70       payload["op
+00011db0: 656e 5f70 6572 696f 6422 5d20 3d20 6f70  en_period"] = op
+00011dc0: 656e 5f70 6572 696f 640a 2020 2020 6966  en_period.    if
+00011dd0: 2063 6c6f 7365 5f64 6174 6520 6973 206e   close_date is n
+00011de0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00011df0: 2069 6620 6973 696e 7374 616e 6365 2863   if isinstance(c
+00011e00: 6c6f 7365 5f64 6174 652c 2064 6174 6574  lose_date, datet
+00011e10: 696d 6529 3a0a 2020 2020 2020 2020 2020  ime):.          
+00011e20: 2020 7061 796c 6f61 645b 2263 6c6f 7365    payload["close
+00011e30: 5f64 6174 6522 5d20 3d20 636c 6f73 655f  _date"] = close_
+00011e40: 6461 7465 2e74 696d 6573 7461 6d70 2829  date.timestamp()
+00011e50: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00011e60: 2020 2020 2020 2020 2020 2070 6179 6c6f             paylo
+00011e70: 6164 5b22 636c 6f73 655f 6461 7465 225d  ad["close_date"]
+00011e80: 203d 2063 6c6f 7365 5f64 6174 650a 2020   = close_date.  
+00011e90: 2020 6966 2069 735f 636c 6f73 6564 2069    if is_closed i
+00011ea0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00011eb0: 2020 2020 7061 796c 6f61 645b 2269 735f      payload["is_
+00011ec0: 636c 6f73 6564 225d 203d 2069 735f 636c  closed"] = is_cl
+00011ed0: 6f73 6564 0a0a 2020 2020 6966 2064 6973  osed..    if dis
+00011ee0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00011ef0: 6e3a 0a20 2020 2020 2020 2070 6179 6c6f  n:.        paylo
+00011f00: 6164 5b22 6469 7361 626c 655f 6e6f 7469  ad["disable_noti
+00011f10: 6669 6361 7469 6f6e 225d 203d 2064 6973  fication"] = dis
+00011f20: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00011f30: 6e0a 2020 2020 6966 2072 6570 6c79 5f74  n.    if reply_t
+00011f40: 6f5f 6d65 7373 6167 655f 6964 2069 7320  o_message_id is 
+00011f50: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00011f60: 2020 7061 796c 6f61 645b 2272 6570 6c79    payload["reply
+00011f70: 5f74 6f5f 6d65 7373 6167 655f 6964 225d  _to_message_id"]
+00011f80: 203d 2072 6570 6c79 5f74 6f5f 6d65 7373   = reply_to_mess
+00011f90: 6167 655f 6964 0a20 2020 2069 6620 616c  age_id.    if al
+00011fa0: 6c6f 775f 7365 6e64 696e 675f 7769 7468  low_sending_with
+00011fb0: 6f75 745f 7265 706c 7920 6973 206e 6f74  out_reply is not
+00011fc0: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
+00011fd0: 6179 6c6f 6164 5b22 616c 6c6f 775f 7365  ayload["allow_se
+00011fe0: 6e64 696e 675f 7769 7468 6f75 745f 7265  nding_without_re
+00011ff0: 706c 7922 5d20 3d20 616c 6c6f 775f 7365  ply"] = allow_se
+00012000: 6e64 696e 675f 7769 7468 6f75 745f 7265  nding_without_re
+00012010: 706c 790a 2020 2020 6966 2072 6570 6c79  ply.    if reply
+00012020: 5f6d 6172 6b75 7020 6973 206e 6f74 204e  _markup is not N
+00012030: 6f6e 653a 0a20 2020 2020 2020 2070 6179  one:.        pay
+00012040: 6c6f 6164 5b22 7265 706c 795f 6d61 726b  load["reply_mark
+00012050: 7570 225d 203d 2061 7761 6974 205f 636f  up"] = await _co
+00012060: 6e76 6572 745f 6d61 726b 7570 2872 6570  nvert_markup(rep
+00012070: 6c79 5f6d 6172 6b75 7029 0a20 2020 2069  ly_markup).    i
+00012080: 6620 7469 6d65 6f75 743a 0a20 2020 2020  f timeout:.     
+00012090: 2020 2070 6179 6c6f 6164 5b22 7469 6d65     payload["time
+000120a0: 6f75 7422 5d20 3d20 7469 6d65 6f75 740a  out"] = timeout.
+000120b0: 2020 2020 6966 2065 7870 6c61 6e61 7469      if explanati
+000120c0: 6f6e 5f65 6e74 6974 6965 733a 0a20 2020  on_entities:.   
+000120d0: 2020 2020 2070 6179 6c6f 6164 5b22 6578       payload["ex
+000120e0: 706c 616e 6174 696f 6e5f 656e 7469 7469  planation_entiti
+000120f0: 6573 225d 203d 206a 736f 6e2e 6475 6d70  es"] = json.dump
+00012100: 7328 7479 7065 732e 4d65 7373 6167 6545  s(types.MessageE
+00012110: 6e74 6974 792e 746f 5f6c 6973 745f 6f66  ntity.to_list_of
+00012120: 5f64 6963 7473 2865 7870 6c61 6e61 7469  _dicts(explanati
+00012130: 6f6e 5f65 6e74 6974 6965 7329 290a 2020  on_entities)).  
+00012140: 2020 6966 2070 726f 7465 6374 5f63 6f6e    if protect_con
+00012150: 7465 6e74 3a0a 2020 2020 2020 2020 7061  tent:.        pa
+00012160: 796c 6f61 645b 2270 726f 7465 6374 5f63  yload["protect_c
+00012170: 6f6e 7465 6e74 225d 203d 2070 726f 7465  ontent"] = prote
+00012180: 6374 5f63 6f6e 7465 6e74 0a20 2020 205f  ct_content.    _
+00012190: 6164 645f 6d65 7373 6167 655f 7468 7265  add_message_thre
+000121a0: 6164 5f69 6428 7061 796c 6f61 642c 206d  ad_id(payload, m
+000121b0: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+000121c0: 290a 2020 2020 7265 7475 726e 2061 7761  ).    return awa
+000121d0: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
+000121e0: 6e2c 206d 6574 686f 645f 7572 6c2c 2070  n, method_url, p
+000121f0: 6172 616d 733d 7061 796c 6f61 6429 0a0a  arams=payload)..
+00012200: 0a61 7379 6e63 2064 6566 2063 7265 6174  .async def creat
+00012210: 655f 666f 7275 6d5f 746f 7069 6328 746f  e_forum_topic(to
+00012220: 6b65 6e2c 2063 6861 745f 6964 2c20 6e61  ken, chat_id, na
+00012230: 6d65 2c20 6963 6f6e 5f63 6f6c 6f72 3d4e  me, icon_color=N
+00012240: 6f6e 652c 2069 636f 6e5f 6375 7374 6f6d  one, icon_custom
+00012250: 5f65 6d6f 6a69 5f69 643d 4e6f 6e65 293a  _emoji_id=None):
+00012260: 0a20 2020 206d 6574 686f 645f 7572 6c20  .    method_url 
+00012270: 3d20 7222 6372 6561 7465 466f 7275 6d54  = r"createForumT
+00012280: 6f70 6963 220a 2020 2020 7061 796c 6f61  opic".    payloa
+00012290: 6420 3d20 7b22 6368 6174 5f69 6422 3a20  d = {"chat_id": 
+000122a0: 6368 6174 5f69 642c 2022 6e61 6d65 223a  chat_id, "name":
+000122b0: 206e 616d 657d 0a20 2020 2069 6620 6963   name}.    if ic
+000122c0: 6f6e 5f63 6f6c 6f72 3a0a 2020 2020 2020  on_color:.      
+000122d0: 2020 7061 796c 6f61 645b 2269 636f 6e5f    payload["icon_
+000122e0: 636f 6c6f 7222 5d20 3d20 6963 6f6e 5f63  color"] = icon_c
+000122f0: 6f6c 6f72 0a20 2020 2069 6620 6963 6f6e  olor.    if icon
+00012300: 5f63 7573 746f 6d5f 656d 6f6a 695f 6964  _custom_emoji_id
+00012310: 3a0a 2020 2020 2020 2020 7061 796c 6f61  :.        payloa
+00012320: 645b 2269 636f 6e5f 6375 7374 6f6d 5f65  d["icon_custom_e
+00012330: 6d6f 6a69 5f69 6422 5d20 3d20 6963 6f6e  moji_id"] = icon
+00012340: 5f63 7573 746f 6d5f 656d 6f6a 695f 6964  _custom_emoji_id
+00012350: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
+00012360: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
+00012370: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
+00012380: 7261 6d73 3d70 6179 6c6f 6164 290a 0a0a  rams=payload)...
+00012390: 6173 796e 6320 6465 6620 6564 6974 5f66  async def edit_f
+000123a0: 6f72 756d 5f74 6f70 6963 2874 6f6b 656e  orum_topic(token
+000123b0: 2c20 6368 6174 5f69 642c 206d 6573 7361  , chat_id, messa
+000123c0: 6765 5f74 6872 6561 645f 6964 2c20 6e61  ge_thread_id, na
+000123d0: 6d65 3d4e 6f6e 652c 2069 636f 6e5f 6375  me=None, icon_cu
+000123e0: 7374 6f6d 5f65 6d6f 6a69 5f69 643d 4e6f  stom_emoji_id=No
+000123f0: 6e65 293a 0a20 2020 206d 6574 686f 645f  ne):.    method_
+00012400: 7572 6c20 3d20 7222 6564 6974 466f 7275  url = r"editForu
+00012410: 6d54 6f70 6963 220a 2020 2020 7061 796c  mTopic".    payl
+00012420: 6f61 6420 3d20 7b22 6368 6174 5f69 6422  oad = {"chat_id"
+00012430: 3a20 6368 6174 5f69 642c 2022 6d65 7373  : chat_id, "mess
+00012440: 6167 655f 7468 7265 6164 5f69 6422 3a20  age_thread_id": 
+00012450: 6d65 7373 6167 655f 7468 7265 6164 5f69  message_thread_i
+00012460: 647d 0a20 2020 2069 6620 6e61 6d65 2069  d}.    if name i
+00012470: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00012480: 2020 2020 7061 796c 6f61 645b 226e 616d      payload["nam
+00012490: 6522 5d20 3d20 6e61 6d65 0a20 2020 2069  e"] = name.    i
+000124a0: 6620 6963 6f6e 5f63 7573 746f 6d5f 656d  f icon_custom_em
+000124b0: 6f6a 695f 6964 2069 7320 6e6f 7420 4e6f  oji_id is not No
+000124c0: 6e65 3a0a 2020 2020 2020 2020 7061 796c  ne:.        payl
+000124d0: 6f61 645b 2269 636f 6e5f 6375 7374 6f6d  oad["icon_custom
+000124e0: 5f65 6d6f 6a69 5f69 6422 5d20 3d20 6963  _emoji_id"] = ic
+000124f0: 6f6e 5f63 7573 746f 6d5f 656d 6f6a 695f  on_custom_emoji_
+00012500: 6964 0a20 2020 2072 6574 7572 6e20 6177  id.    return aw
+00012510: 6169 7420 5f72 6571 7565 7374 2874 6f6b  ait _request(tok
+00012520: 656e 2c20 6d65 7468 6f64 5f75 726c 2c20  en, method_url, 
+00012530: 7061 7261 6d73 3d70 6179 6c6f 6164 290a  params=payload).
+00012540: 0a0a 6173 796e 6320 6465 6620 636c 6f73  ..async def clos
+00012550: 655f 666f 7275 6d5f 746f 7069 6328 746f  e_forum_topic(to
+00012560: 6b65 6e2c 2063 6861 745f 6964 2c20 6d65  ken, chat_id, me
+00012570: 7373 6167 655f 7468 7265 6164 5f69 6429  ssage_thread_id)
+00012580: 3a0a 2020 2020 6d65 7468 6f64 5f75 726c  :.    method_url
+00012590: 203d 2072 2263 6c6f 7365 466f 7275 6d54   = r"closeForumT
+000125a0: 6f70 6963 220a 2020 2020 7061 796c 6f61  opic".    payloa
+000125b0: 6420 3d20 7b22 6368 6174 5f69 6422 3a20  d = {"chat_id": 
+000125c0: 6368 6174 5f69 642c 2022 6d65 7373 6167  chat_id, "messag
+000125d0: 655f 7468 7265 6164 5f69 6422 3a20 6d65  e_thread_id": me
+000125e0: 7373 6167 655f 7468 7265 6164 5f69 647d  ssage_thread_id}
+000125f0: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
+00012600: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
+00012610: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
+00012620: 7261 6d73 3d70 6179 6c6f 6164 290a 0a0a  rams=payload)...
+00012630: 6173 796e 6320 6465 6620 7265 6f70 656e  async def reopen
+00012640: 5f66 6f72 756d 5f74 6f70 6963 2874 6f6b  _forum_topic(tok
+00012650: 656e 2c20 6368 6174 5f69 642c 206d 6573  en, chat_id, mes
+00012660: 7361 6765 5f74 6872 6561 645f 6964 293a  sage_thread_id):
+00012670: 0a20 2020 206d 6574 686f 645f 7572 6c20  .    method_url 
+00012680: 3d20 7222 7265 6f70 656e 466f 7275 6d54  = r"reopenForumT
+00012690: 6f70 6963 220a 2020 2020 7061 796c 6f61  opic".    payloa
+000126a0: 6420 3d20 7b22 6368 6174 5f69 6422 3a20  d = {"chat_id": 
+000126b0: 6368 6174 5f69 642c 2022 6d65 7373 6167  chat_id, "messag
+000126c0: 655f 7468 7265 6164 5f69 6422 3a20 6d65  e_thread_id": me
+000126d0: 7373 6167 655f 7468 7265 6164 5f69 647d  ssage_thread_id}
+000126e0: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
+000126f0: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
+00012700: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
+00012710: 7261 6d73 3d70 6179 6c6f 6164 290a 0a0a  rams=payload)...
+00012720: 6173 796e 6320 6465 6620 6465 6c65 7465  async def delete
+00012730: 5f66 6f72 756d 5f74 6f70 6963 2874 6f6b  _forum_topic(tok
+00012740: 656e 2c20 6368 6174 5f69 642c 206d 6573  en, chat_id, mes
+00012750: 7361 6765 5f74 6872 6561 645f 6964 293a  sage_thread_id):
+00012760: 0a20 2020 206d 6574 686f 645f 7572 6c20  .    method_url 
+00012770: 3d20 7222 6465 6c65 7465 466f 7275 6d54  = r"deleteForumT
+00012780: 6f70 6963 220a 2020 2020 7061 796c 6f61  opic".    payloa
+00012790: 6420 3d20 7b22 6368 6174 5f69 6422 3a20  d = {"chat_id": 
+000127a0: 6368 6174 5f69 642c 2022 6d65 7373 6167  chat_id, "messag
+000127b0: 655f 7468 7265 6164 5f69 6422 3a20 6d65  e_thread_id": me
+000127c0: 7373 6167 655f 7468 7265 6164 5f69 647d  ssage_thread_id}
+000127d0: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
+000127e0: 7420 5f72 6571 7565 7374 2874 6f6b 656e  t _request(token
+000127f0: 2c20 6d65 7468 6f64 5f75 726c 2c20 7061  , method_url, pa
+00012800: 7261 6d73 3d70 6179 6c6f 6164 290a 0a0a  rams=payload)...
+00012810: 6173 796e 6320 6465 6620 756e 7069 6e5f  async def unpin_
+00012820: 616c 6c5f 666f 7275 6d5f 746f 7069 635f  all_forum_topic_
+00012830: 6d65 7373 6167 6573 2874 6f6b 656e 2c20  messages(token, 
+00012840: 6368 6174 5f69 642c 206d 6573 7361 6765  chat_id, message
+00012850: 5f74 6872 6561 645f 6964 293a 0a20 2020  _thread_id):.   
+00012860: 206d 6574 686f 645f 7572 6c20 3d20 7222   method_url = r"
+00012870: 756e 7069 6e41 6c6c 466f 7275 6d54 6f70  unpinAllForumTop
+00012880: 6963 4d65 7373 6167 6573 220a 2020 2020  icMessages".    
+00012890: 7061 796c 6f61 6420 3d20 7b22 6368 6174  payload = {"chat
+000128a0: 5f69 6422 3a20 6368 6174 5f69 642c 2022  _id": chat_id, "
+000128b0: 6d65 7373 6167 655f 7468 7265 6164 5f69  message_thread_i
+000128c0: 6422 3a20 6d65 7373 6167 655f 7468 7265  d": message_thre
+000128d0: 6164 5f69 647d 0a20 2020 2072 6574 7572  ad_id}.    retur
+000128e0: 6e20 6177 6169 7420 5f72 6571 7565 7374  n await _request
+000128f0: 2874 6f6b 656e 2c20 6d65 7468 6f64 5f75  (token, method_u
+00012900: 726c 2c20 7061 7261 6d73 3d70 6179 6c6f  rl, params=paylo
+00012910: 6164 290a 0a0a 6173 796e 6320 6465 6620  ad)...async def 
+00012920: 6765 745f 666f 7275 6d5f 746f 7069 635f  get_forum_topic_
+00012930: 6963 6f6e 5f73 7469 636b 6572 7328 746f  icon_stickers(to
+00012940: 6b65 6e29 3a0a 2020 2020 6d65 7468 6f64  ken):.    method
+00012950: 5f75 726c 203d 2072 2267 6574 466f 7275  _url = r"getForu
+00012960: 6d54 6f70 6963 4963 6f6e 5374 6963 6b65  mTopicIconSticke
+00012970: 7273 220a 2020 2020 7265 7475 726e 2061  rs".    return a
+00012980: 7761 6974 205f 7265 7175 6573 7428 746f  wait _request(to
+00012990: 6b65 6e2c 206d 6574 686f 645f 7572 6c29  ken, method_url)
+000129a0: 0a0a 0a61 7379 6e63 2064 6566 2065 6469  ...async def edi
+000129b0: 745f 6765 6e65 7261 6c5f 666f 7275 6d5f  t_general_forum_
+000129c0: 746f 7069 6328 746f 6b65 6e2c 2063 6861  topic(token, cha
+000129d0: 745f 6964 2c20 6e61 6d65 293a 0a20 2020  t_id, name):.   
+000129e0: 206d 6574 686f 645f 7572 6c20 3d20 7222   method_url = r"
+000129f0: 6564 6974 4765 6e65 7261 6c46 6f72 756d  editGeneralForum
+00012a00: 546f 7069 6322 0a20 2020 2070 6179 6c6f  Topic".    paylo
+00012a10: 6164 203d 207b 2263 6861 745f 6964 223a  ad = {"chat_id":
+00012a20: 2063 6861 745f 6964 2c20 226e 616d 6522   chat_id, "name"
+00012a30: 3a20 6e61 6d65 7d0a 2020 2020 7265 7475  : name}.    retu
+00012a40: 726e 2061 7761 6974 205f 7265 7175 6573  rn await _reques
+00012a50: 7428 746f 6b65 6e2c 206d 6574 686f 645f  t(token, method_
+00012a60: 7572 6c2c 2070 6172 616d 733d 7061 796c  url, params=payl
+00012a70: 6f61 6429 0a0a 0a61 7379 6e63 2064 6566  oad)...async def
+00012a80: 2063 6c6f 7365 5f67 656e 6572 616c 5f66   close_general_f
+00012a90: 6f72 756d 5f74 6f70 6963 2874 6f6b 656e  orum_topic(token
+00012aa0: 2c20 6368 6174 5f69 6429 3a0a 2020 2020  , chat_id):.    
+00012ab0: 6d65 7468 6f64 5f75 726c 203d 2072 2263  method_url = r"c
+00012ac0: 6c6f 7365 4765 6e65 7261 6c46 6f72 756d  loseGeneralForum
+00012ad0: 546f 7069 6322 0a20 2020 2070 6179 6c6f  Topic".    paylo
+00012ae0: 6164 203d 207b 2263 6861 745f 6964 223a  ad = {"chat_id":
+00012af0: 2063 6861 745f 6964 7d0a 2020 2020 7265   chat_id}.    re
+00012b00: 7475 726e 2061 7761 6974 205f 7265 7175  turn await _requ
+00012b10: 6573 7428 746f 6b65 6e2c 206d 6574 686f  est(token, metho
+00012b20: 645f 7572 6c2c 2070 6172 616d 733d 7061  d_url, params=pa
+00012b30: 796c 6f61 6429 0a0a 0a61 7379 6e63 2064  yload)...async d
+00012b40: 6566 2072 656f 7065 6e5f 6765 6e65 7261  ef reopen_genera
+00012b50: 6c5f 666f 7275 6d5f 746f 7069 6328 746f  l_forum_topic(to
+00012b60: 6b65 6e2c 2063 6861 745f 6964 293a 0a20  ken, chat_id):. 
+00012b70: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
+00012b80: 7222 7265 6f70 656e 4765 6e65 7261 6c46  r"reopenGeneralF
+00012b90: 6f72 756d 546f 7069 6322 0a20 2020 2070  orumTopic".    p
+00012ba0: 6179 6c6f 6164 203d 207b 2263 6861 745f  ayload = {"chat_
+00012bb0: 6964 223a 2063 6861 745f 6964 7d0a 2020  id": chat_id}.  
+00012bc0: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
+00012bd0: 7265 7175 6573 7428 746f 6b65 6e2c 206d  request(token, m
+00012be0: 6574 686f 645f 7572 6c2c 2070 6172 616d  ethod_url, param
+00012bf0: 733d 7061 796c 6f61 6429 0a0a 0a61 7379  s=payload)...asy
+00012c00: 6e63 2064 6566 2068 6964 655f 6765 6e65  nc def hide_gene
+00012c10: 7261 6c5f 666f 7275 6d5f 746f 7069 6328  ral_forum_topic(
+00012c20: 746f 6b65 6e2c 2063 6861 745f 6964 293a  token, chat_id):
+00012c30: 0a20 2020 206d 6574 686f 645f 7572 6c20  .    method_url 
+00012c40: 3d20 7222 6869 6465 4765 6e65 7261 6c46  = r"hideGeneralF
+00012c50: 6f72 756d 546f 7069 6322 0a20 2020 2070  orumTopic".    p
+00012c60: 6179 6c6f 6164 203d 207b 2263 6861 745f  ayload = {"chat_
+00012c70: 6964 223a 2063 6861 745f 6964 7d0a 2020  id": chat_id}.  
+00012c80: 2020 7265 7475 726e 2061 7761 6974 205f    return await _
+00012c90: 7265 7175 6573 7428 746f 6b65 6e2c 206d  request(token, m
+00012ca0: 6574 686f 645f 7572 6c2c 2070 6172 616d  ethod_url, param
+00012cb0: 733d 7061 796c 6f61 6429 0a0a 0a61 7379  s=payload)...asy
+00012cc0: 6e63 2064 6566 2075 6e68 6964 655f 6765  nc def unhide_ge
+00012cd0: 6e65 7261 6c5f 666f 7275 6d5f 746f 7069  neral_forum_topi
+00012ce0: 6328 746f 6b65 6e2c 2063 6861 745f 6964  c(token, chat_id
+00012cf0: 293a 0a20 2020 206d 6574 686f 645f 7572  ):.    method_ur
+00012d00: 6c20 3d20 7222 756e 6869 6465 4765 6e65  l = r"unhideGene
+00012d10: 7261 6c46 6f72 756d 546f 7069 6322 0a20  ralForumTopic". 
+00012d20: 2020 2070 6179 6c6f 6164 203d 207b 2263     payload = {"c
+00012d30: 6861 745f 6964 223a 2063 6861 745f 6964  hat_id": chat_id
+00012d40: 7d0a 2020 2020 7265 7475 726e 2061 7761  }.    return awa
+00012d50: 6974 205f 7265 7175 6573 7428 746f 6b65  it _request(toke
+00012d60: 6e2c 206d 6574 686f 645f 7572 6c2c 2070  n, method_url, p
+00012d70: 6172 616d 733d 7061 796c 6f61 6429 0a0a  arams=payload)..
+00012d80: 0a61 7379 6e63 2064 6566 205f 636f 6e76  .async def _conv
+00012d90: 6572 745f 6c69 7374 5f6a 736f 6e5f 7365  ert_list_json_se
+00012da0: 7269 616c 697a 6162 6c65 2872 6573 756c  rializable(resul
+00012db0: 7473 293a 0a20 2020 2072 6574 203d 2022  ts):.    ret = "
+00012dc0: 220a 2020 2020 666f 7220 7220 696e 2072  ".    for r in r
+00012dd0: 6573 756c 7473 3a0a 2020 2020 2020 2020  esults:.        
+00012de0: 6966 2069 7369 6e73 7461 6e63 6528 722c  if isinstance(r,
+00012df0: 2074 7970 6573 2e4a 736f 6e53 6572 6961   types.JsonSeria
+00012e00: 6c69 7a61 626c 6529 3a0a 2020 2020 2020  lizable):.      
+00012e10: 2020 2020 2020 7265 7420 3d20 7265 7420        ret = ret 
+00012e20: 2b20 722e 746f 5f6a 736f 6e28 2920 2b20  + r.to_json() + 
+00012e30: 222c 220a 2020 2020 6966 206c 656e 2872  ",".    if len(r
+00012e40: 6574 2920 3e20 303a 0a20 2020 2020 2020  et) > 0:.       
+00012e50: 2072 6574 203d 2072 6574 5b3a 2d31 5d0a   ret = ret[:-1].
+00012e60: 2020 2020 7265 7475 726e 2022 5b22 202b      return "[" +
+00012e70: 2072 6574 202b 2022 5d22 0a0a 0a61 7379   ret + "]"...asy
+00012e80: 6e63 2064 6566 205f 636f 6e76 6572 745f  nc def _convert_
+00012e90: 656e 7469 7465 7328 656e 7469 7465 7329  entites(entites)
+00012ea0: 3a0a 2020 2020 6966 2065 6e74 6974 6573  :.    if entites
+00012eb0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00012ec0: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
+00012ed0: 2020 656c 6966 206c 656e 2865 6e74 6974    elif len(entit
+00012ee0: 6573 2920 3d3d 2030 3a0a 2020 2020 2020  es) == 0:.      
+00012ef0: 2020 7265 7475 726e 205b 5d0a 2020 2020    return [].    
+00012f00: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+00012f10: 656e 7469 7465 735b 305d 2c20 7479 7065  entites[0], type
+00012f20: 732e 4a73 6f6e 5365 7269 616c 697a 6162  s.JsonSerializab
+00012f30: 6c65 293a 0a20 2020 2020 2020 2072 6574  le):.        ret
+00012f40: 7572 6e20 5b65 6e74 6974 792e 746f 5f6a  urn [entity.to_j
+00012f50: 736f 6e28 2920 666f 7220 656e 7469 7479  son() for entity
+00012f60: 2069 6e20 656e 7469 7465 735d 0a20 2020   in entites].   
+00012f70: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
+00012f80: 6574 7572 6e20 656e 7469 7465 730a 0a0a  eturn entites...
+00012f90: 6173 796e 6320 6465 6620 5f63 6f6e 7665  async def _conve
+00012fa0: 7274 5f70 6f6c 6c5f 6f70 7469 6f6e 7328  rt_poll_options(
+00012fb0: 706f 6c6c 5f6f 7074 696f 6e73 293a 0a20  poll_options):. 
+00012fc0: 2020 2069 6620 706f 6c6c 5f6f 7074 696f     if poll_optio
+00012fd0: 6e73 2069 7320 4e6f 6e65 3a0a 2020 2020  ns is None:.    
+00012fe0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00012ff0: 2020 2020 656c 6966 206c 656e 2870 6f6c      elif len(pol
+00013000: 6c5f 6f70 7469 6f6e 7329 203d 3d20 303a  l_options) == 0:
+00013010: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013020: 5b5d 0a20 2020 2065 6c69 6620 6973 696e  [].    elif isin
+00013030: 7374 616e 6365 2870 6f6c 6c5f 6f70 7469  stance(poll_opti
+00013040: 6f6e 735b 305d 2c20 7374 7229 3a0a 2020  ons[0], str):.  
+00013050: 2020 2020 2020 2320 436f 6d70 6174 6962        # Compatib
+00013060: 696c 6974 7920 6d6f 6465 2077 6974 6820  ility mode with 
+00013070: 7072 6576 696f 7573 2062 7567 2077 6865  previous bug whe
+00013080: 6e20 6f6e 6c79 206c 6973 7420 6f66 2073  n only list of s
+00013090: 7472 696e 6720 7761 7320 6163 6365 7074  tring was accept
+000130a0: 6564 2061 7320 706f 6c6c 5f6f 7074 696f  ed as poll_optio
+000130b0: 6e73 0a20 2020 2020 2020 2072 6574 7572  ns.        retur
+000130c0: 6e20 706f 6c6c 5f6f 7074 696f 6e73 0a20  n poll_options. 
+000130d0: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+000130e0: 6365 2870 6f6c 6c5f 6f70 7469 6f6e 735b  ce(poll_options[
+000130f0: 305d 2c20 7479 7065 732e 506f 6c6c 4f70  0], types.PollOp
+00013100: 7469 6f6e 293a 0a20 2020 2020 2020 2072  tion):.        r
+00013110: 6574 7572 6e20 5b6f 7074 696f 6e2e 7465  eturn [option.te
+00013120: 7874 2066 6f72 206f 7074 696f 6e20 696e  xt for option in
+00013130: 2070 6f6c 6c5f 6f70 7469 6f6e 735d 0a20   poll_options]. 
+00013140: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00013150: 2072 6574 7572 6e20 706f 6c6c 5f6f 7074   return poll_opt
+00013160: 696f 6e73 0a0a 0a61 7379 6e63 2064 6566  ions...async def
+00013170: 2063 6f6e 7665 7274 5f69 6e70 7574 5f6d   convert_input_m
+00013180: 6564 6961 286d 6564 6961 293a 0a20 2020  edia(media):.   
+00013190: 2069 6620 6973 696e 7374 616e 6365 286d   if isinstance(m
+000131a0: 6564 6961 2c20 7479 7065 732e 496e 7075  edia, types.Inpu
+000131b0: 744d 6564 6961 293a 0a20 2020 2020 2020  tMedia):.       
+000131c0: 2072 6574 7572 6e20 6d65 6469 612e 636f   return media.co
+000131d0: 6e76 6572 745f 696e 7075 745f 6d65 6469  nvert_input_medi
+000131e0: 6128 290a 2020 2020 7265 7475 726e 204e  a().    return N
+000131f0: 6f6e 652c 204e 6f6e 650a 0a0a 6173 796e  one, None...asyn
+00013200: 6320 6465 6620 636f 6e76 6572 745f 696e  c def convert_in
+00013210: 7075 745f 6d65 6469 615f 6172 7261 7928  put_media_array(
+00013220: 6172 7261 7929 3a0a 2020 2020 6d65 6469  array):.    medi
+00013230: 6120 3d20 5b5d 0a20 2020 2066 696c 6573  a = [].    files
+00013240: 203d 207b 7d0a 2020 2020 666f 7220 696e   = {}.    for in
+00013250: 7075 745f 6d65 6469 6120 696e 2061 7272  put_media in arr
+00013260: 6179 3a0a 2020 2020 2020 2020 6966 2069  ay:.        if i
+00013270: 7369 6e73 7461 6e63 6528 696e 7075 745f  sinstance(input_
+00013280: 6d65 6469 612c 2074 7970 6573 2e49 6e70  media, types.Inp
+00013290: 7574 4d65 6469 6129 3a0a 2020 2020 2020  utMedia):.      
+000132a0: 2020 2020 2020 6d65 6469 615f 6469 6374        media_dict
+000132b0: 203d 2069 6e70 7574 5f6d 6564 6961 2e74   = input_media.t
+000132c0: 6f5f 6469 6374 2829 0a20 2020 2020 2020  o_dict().       
+000132d0: 2020 2020 2069 6620 6d65 6469 615f 6469       if media_di
+000132e0: 6374 5b22 6d65 6469 6122 5d2e 7374 6172  ct["media"].star
+000132f0: 7473 7769 7468 2822 6174 7461 6368 3a2f  tswith("attach:/
+00013300: 2f22 293a 0a20 2020 2020 2020 2020 2020  /"):.           
+00013310: 2020 2020 206b 6579 203d 206d 6564 6961       key = media
+00013320: 5f64 6963 745b 226d 6564 6961 225d 2e72  _dict["media"].r
+00013330: 6570 6c61 6365 2822 6174 7461 6368 3a2f  eplace("attach:/
+00013340: 2f22 2c20 2222 290a 2020 2020 2020 2020  /", "").        
+00013350: 2020 2020 2020 2020 6669 6c65 735b 6b65          files[ke
+00013360: 795d 203d 2069 6e70 7574 5f6d 6564 6961  y] = input_media
+00013370: 2e6d 6564 6961 0a20 2020 2020 2020 2020  .media.         
+00013380: 2020 206d 6564 6961 2e61 7070 656e 6428     media.append(
+00013390: 6d65 6469 615f 6469 6374 290a 2020 2020  media_dict).    
+000133a0: 7265 7475 726e 206a 736f 6e2e 6475 6d70  return json.dump
+000133b0: 7328 6d65 6469 6129 2c20 6669 6c65 730a  s(media), files.
+000133c0: 0a0a 6173 796e 6320 6465 6620 5f6e 6f5f  ..async def _no_
+000133d0: 656e 636f 6465 2866 756e 6329 3a0a 2020  encode(func):.  
+000133e0: 2020 6465 6620 7772 6170 7065 7228 6b65    def wrapper(ke
+000133f0: 792c 2076 616c 293a 0a20 2020 2020 2020  y, val):.       
+00013400: 2069 6620 6b65 7920 3d3d 2022 6669 6c65   if key == "file
+00013410: 6e61 6d65 223a 0a20 2020 2020 2020 2020  name":.         
+00013420: 2020 2072 6574 7572 6e20 227b 307d 3d7b     return "{0}={
+00013430: 317d 222e 666f 726d 6174 286b 6579 2c20  1}".format(key, 
+00013440: 7661 6c29 0a20 2020 2020 2020 2065 6c73  val).        els
+00013450: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00013460: 6574 7572 6e20 6675 6e63 286b 6579 2c20  eturn func(key, 
+00013470: 7661 6c29 0a0a 2020 2020 7265 7475 726e  val)..    return
+00013480: 2077 7261 7070 6572 0a0a 0a61 7379 6e63   wrapper...async
+00013490: 2064 6566 2073 746f 705f 706f 6c6c 2874   def stop_poll(t
+000134a0: 6f6b 656e 2c20 6368 6174 5f69 642c 206d  oken, chat_id, m
+000134b0: 6573 7361 6765 5f69 642c 2072 6570 6c79  essage_id, reply
+000134c0: 5f6d 6172 6b75 703d 4e6f 6e65 293a 0a20  _markup=None):. 
+000134d0: 2020 206d 6574 686f 645f 7572 6c20 3d20     method_url = 
+000134e0: 7222 7374 6f70 506f 6c6c 220a 2020 2020  r"stopPoll".    
+000134f0: 7061 796c 6f61 6420 3d20 7b22 6368 6174  payload = {"chat
+00013500: 5f69 6422 3a20 7374 7228 6368 6174 5f69  _id": str(chat_i
+00013510: 6429 2c20 226d 6573 7361 6765 5f69 6422  d), "message_id"
+00013520: 3a20 6d65 7373 6167 655f 6964 7d0a 2020  : message_id}.  
+00013530: 2020 6966 2072 6570 6c79 5f6d 6172 6b75    if reply_marku
+00013540: 703a 0a20 2020 2020 2020 2070 6179 6c6f  p:.        paylo
+00013550: 6164 5b22 7265 706c 795f 6d61 726b 7570  ad["reply_markup
+00013560: 225d 203d 2061 7761 6974 205f 636f 6e76  "] = await _conv
+00013570: 6572 745f 6d61 726b 7570 2872 6570 6c79  ert_markup(reply
+00013580: 5f6d 6172 6b75 7029 0a20 2020 2072 6574  _markup).    ret
+00013590: 7572 6e20 6177 6169 7420 5f72 6571 7565  urn await _reque
+000135a0: 7374 2874 6f6b 656e 2c20 6d65 7468 6f64  st(token, method
+000135b0: 5f75 726c 2c20 7061 7261 6d73 3d70 6179  _url, params=pay
+000135c0: 6c6f 6164 290a 0a0a 636c 6173 7320 4170  load)...class Ap
+000135d0: 6945 7863 6570 7469 6f6e 2845 7863 6570  iException(Excep
+000135e0: 7469 6f6e 293a 0a20 2020 2022 2222 0a20  tion):.    """. 
+000135f0: 2020 2054 6869 7320 636c 6173 7320 7265     This class re
+00013600: 7072 6573 656e 7473 2061 2062 6173 6520  presents a base 
+00013610: 4578 6365 7074 696f 6e20 7468 726f 776e  Exception thrown
+00013620: 2077 6865 6e20 6120 6361 6c6c 2074 6f20   when a call to 
+00013630: 7468 6520 5465 6c65 6772 616d 2041 5049  the Telegram API
+00013640: 2066 6169 6c73 2e0a 2020 2020 4974 2063   fails..    It c
+00013650: 6f6e 7461 696e 7320 6169 6f68 7474 7020  ontains aiohttp 
+00013660: 636c 6965 6e74 2072 6573 706f 6e73 6520  client response 
+00013670: 696e 2063 6173 6520 796f 7520 7761 6e74  in case you want
+00013680: 2074 6f20 646f 2073 6f6d 6520 6164 7661   to do some adva
+00013690: 6e63 6564 2065 7272 6f72 2068 616e 646c  nced error handl
+000136a0: 696e 672e 0a20 2020 2022 2222 0a0a 2020  ing..    """..  
+000136b0: 2020 4150 495f 5552 4c5f 5245 4745 5820    API_URL_REGEX 
+000136c0: 3d20 7265 2e63 6f6d 7069 6c65 2872 2261  = re.compile(r"a
+000136d0: 7069 5c2e 7465 6c65 6772 616d 5c2e 6f72  pi\.telegram\.or
+000136e0: 672f 626f 7428 3f50 3c74 6f6b 656e 3e2e  g/bot(?P<token>.
+000136f0: 2a3f 292f 2e2a 2229 0a0a 2020 2020 6465  *?)/.*")..    de
+00013700: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00013710: 206d 7367 3a20 7374 722c 2072 6573 706f   msg: str, respo
+00013720: 6e73 653a 2061 696f 6874 7470 2e43 6c69  nse: aiohttp.Cli
+00013730: 656e 7452 6573 706f 6e73 6529 3a0a 2020  entResponse):.  
+00013740: 2020 2020 2020 6d61 7463 6820 3d20 7365        match = se
+00013750: 6c66 2e41 5049 5f55 524c 5f52 4547 4558  lf.API_URL_REGEX
+00013760: 2e73 6561 7263 6828 6d73 6729 0a20 2020  .search(msg).   
+00013770: 2020 2020 2069 6620 6d61 7463 6820 6973       if match is
+00013780: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00013790: 2020 2020 2020 2062 6f74 5f74 6f6b 656e         bot_token
+000137a0: 203d 206d 6174 6368 2e67 726f 7570 2822   = match.group("
+000137b0: 746f 6b65 6e22 290a 2020 2020 2020 2020  token").        
+000137c0: 2020 2020 6d61 736b 6564 5f74 6f6b 656e      masked_token
+000137d0: 203d 2062 6f74 5f74 6f6b 656e 5b3a 335d   = bot_token[:3]
+000137e0: 202b 2022 2a22 202a 2028 6c65 6e28 626f   + "*" * (len(bo
+000137f0: 745f 746f 6b65 6e29 202d 2033 290a 2020  t_token) - 3).  
+00013800: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
+00013810: 6d73 672e 7265 706c 6163 6528 626f 745f  msg.replace(bot_
+00013820: 746f 6b65 6e2c 206d 6173 6b65 645f 746f  token, masked_to
+00013830: 6b65 6e29 0a0a 2020 2020 2020 2020 7375  ken)..        su
+00013840: 7065 7228 292e 5f5f 696e 6974 5f5f 286d  per().__init__(m
+00013850: 7367 290a 2020 2020 2020 2020 7365 6c66  sg).        self
+00013860: 2e72 6573 706f 6e73 6520 3d20 7265 7370  .response = resp
+00013870: 6f6e 7365 0a0a 0a40 6461 7461 636c 6173  onse...@dataclas
+00013880: 730a 636c 6173 7320 4572 726f 7252 6573  s.class ErrorRes
+00013890: 706f 6e73 6550 6172 616d 6574 6572 733a  ponseParameters:
+000138a0: 0a20 2020 2022 2222 6874 7470 733a 2f2f  .    """https://
+000138b0: 636f 7265 2e74 656c 6567 7261 6d2e 6f72  core.telegram.or
+000138c0: 672f 626f 7473 2f61 7069 2372 6573 706f  g/bots/api#respo
+000138d0: 6e73 6570 6172 616d 6574 6572 7322 2222  nseparameters"""
+000138e0: 0a0a 2020 2020 6d69 6772 6174 655f 746f  ..    migrate_to
+000138f0: 5f63 6861 745f 6964 3a20 4f70 7469 6f6e  _chat_id: Option
+00013900: 616c 5b69 6e74 5d0a 2020 2020 7265 7472  al[int].    retr
+00013910: 795f 6166 7465 723a 204f 7074 696f 6e61  y_after: Optiona
+00013920: 6c5b 696e 745d 0a0a 2020 2020 4063 6c61  l[int]..    @cla
+00013930: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+00013940: 2070 6172 7365 2863 6c73 2c20 7261 773a   parse(cls, raw:
+00013950: 2041 6e79 2920 2d3e 204f 7074 696f 6e61   Any) -> Optiona
+00013960: 6c5b 2245 7272 6f72 5265 7370 6f6e 7365  l["ErrorResponse
+00013970: 5061 7261 6d65 7465 7273 225d 3a0a 2020  Parameters"]:.  
+00013980: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+00013990: 6e73 7461 6e63 6528 7261 772c 2064 6963  nstance(raw, dic
+000139a0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+000139b0: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
+000139c0: 2020 2020 6d69 6772 6174 655f 746f 5f63      migrate_to_c
+000139d0: 6861 745f 6964 203d 2072 6177 2e67 6574  hat_id = raw.get
+000139e0: 2822 6d69 6772 6174 655f 746f 5f63 6861  ("migrate_to_cha
+000139f0: 745f 6964 2229 0a20 2020 2020 2020 2069  t_id").        i
+00013a00: 6620 6e6f 7420 286d 6967 7261 7465 5f74  f not (migrate_t
+00013a10: 6f5f 6368 6174 5f69 6420 6973 204e 6f6e  o_chat_id is Non
+00013a20: 6520 6f72 2069 7369 6e73 7461 6e63 6528  e or isinstance(
+00013a30: 6d69 6772 6174 655f 746f 5f63 6861 745f  migrate_to_chat_
+00013a40: 6964 2c20 696e 7429 293a 0a20 2020 2020  id, int)):.     
+00013a50: 2020 2020 2020 206c 6f67 6765 722e 6572         logger.er
+00013a60: 726f 7228 6622 496e 7661 6c69 6420 6572  ror(f"Invalid er
+00013a70: 726f 7220 7265 7370 6f6e 7365 2070 6172  ror response par
+00013a80: 616d 6574 6572 733a 207b 7261 777d 2229  ameters: {raw}")
+00013a90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00013aa0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
+00013ab0: 2020 7265 7472 795f 6166 7465 7220 3d20    retry_after = 
+00013ac0: 7261 772e 6765 7428 2272 6574 7279 5f61  raw.get("retry_a
+00013ad0: 6674 6572 2229 0a20 2020 2020 2020 2069  fter").        i
+00013ae0: 6620 6e6f 7420 2872 6574 7279 5f61 6674  f not (retry_aft
+00013af0: 6572 2069 7320 4e6f 6e65 206f 7220 6973  er is None or is
+00013b00: 696e 7374 616e 6365 2872 6574 7279 5f61  instance(retry_a
+00013b10: 6674 6572 2c20 696e 7429 293a 0a20 2020  fter, int)):.   
+00013b20: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00013b30: 6572 726f 7228 6622 496e 7661 6c69 6420  error(f"Invalid 
+00013b40: 6572 726f 7220 7265 7370 6f6e 7365 2070  error response p
+00013b50: 6172 616d 6574 6572 733a 207b 7261 777d  arameters: {raw}
+00013b60: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+00013b70: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
+00013b80: 2020 2020 7265 7475 726e 2045 7272 6f72      return Error
+00013b90: 5265 7370 6f6e 7365 5061 7261 6d65 7465  ResponseParamete
+00013ba0: 7273 286d 6967 7261 7465 5f74 6f5f 6368  rs(migrate_to_ch
+00013bb0: 6174 5f69 643d 6d69 6772 6174 655f 746f  at_id=migrate_to
+00013bc0: 5f63 6861 745f 6964 2c20 7265 7472 795f  _chat_id, retry_
+00013bd0: 6166 7465 723d 7265 7472 795f 6166 7465  after=retry_afte
+00013be0: 7229 0a0a 0a63 6c61 7373 2041 7069 4854  r)...class ApiHT
+00013bf0: 5450 4578 6365 7074 696f 6e28 4170 6945  TPException(ApiE
+00013c00: 7863 6570 7469 6f6e 293a 0a20 2020 2022  xception):.    "
+00013c10: 2222 0a20 2020 2054 6869 7320 636c 6173  "".    This clas
+00013c20: 7320 7265 7072 6573 656e 7473 2061 6e20  s represents an 
+00013c30: 4578 6365 7074 696f 6e20 7468 726f 776e  Exception thrown
+00013c40: 2077 6865 6e20 6120 6361 6c6c 2074 6f20   when a call to 
+00013c50: 7468 650a 2020 2020 5465 6c65 6772 616d  the.    Telegram
+00013c60: 2041 5049 2073 6572 7665 7220 7265 7475   API server retu
+00013c70: 726e 7320 4854 5450 2063 6f64 6520 7468  rns HTTP code th
+00013c80: 6174 2069 7320 6e6f 7420 3230 302e 0a20  at is not 200.. 
+00013c90: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
+00013ca0: 5f5f 696e 6974 5f5f 2873 656c 662c 2072  __init__(self, r
+00013cb0: 6573 706f 6e73 655f 6a73 6f6e 3a20 416e  esponse_json: An
+00013cc0: 792c 2072 6573 706f 6e73 653a 2061 696f  y, response: aio
+00013cd0: 6874 7470 2e43 6c69 656e 7452 6573 706f  http.ClientRespo
+00013ce0: 6e73 6529 3a0a 2020 2020 2020 2020 7365  nse):.        se
+00013cf0: 6c66 2e65 7272 6f72 5f70 6172 616d 6574  lf.error_paramet
+00013d00: 6572 7320 3d20 4572 726f 7252 6573 706f  ers = ErrorRespo
+00013d10: 6e73 6550 6172 616d 6574 6572 732e 7061  nseParameters.pa
+00013d20: 7273 6528 7265 7370 6f6e 7365 5f6a 736f  rse(response_jso
+00013d30: 6e2e 6765 7428 2270 6172 616d 6574 6572  n.get("parameter
+00013d40: 7322 2929 0a0a 2020 2020 2020 2020 6966  s"))..        if
+00013d50: 2069 7369 6e73 7461 6e63 6528 7265 7370   isinstance(resp
+00013d60: 6f6e 7365 5f6a 736f 6e2c 2064 6963 7429  onse_json, dict)
+00013d70: 2061 6e64 2022 6465 7363 7269 7074 696f   and "descriptio
+00013d80: 6e22 2069 6e20 7265 7370 6f6e 7365 5f6a  n" in response_j
+00013d90: 736f 6e3a 0a20 2020 2020 2020 2020 2020  son:.           
+00013da0: 2073 656c 662e 6572 726f 725f 6465 7363   self.error_desc
+00013db0: 7269 7074 696f 6e3a 204f 7074 696f 6e61  ription: Optiona
+00013dc0: 6c5b 7374 725d 203d 2073 7472 2872 6573  l[str] = str(res
+00013dd0: 706f 6e73 655f 6a73 6f6e 5b22 6465 7363  ponse_json["desc
+00013de0: 7269 7074 696f 6e22 5d29 0a20 2020 2020  ription"]).     
+00013df0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00013e00: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
+00013e10: 6465 7363 7269 7074 696f 6e20 3d20 4e6f  description = No
+00013e20: 6e65 0a0a 2020 2020 2020 2020 6572 726f  ne..        erro
+00013e30: 725f 7469 746c 6520 3d20 280a 2020 2020  r_title = (.    
+00013e40: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
+00013e50: 6f72 5f64 6573 6372 6970 7469 6f6e 0a20  or_description. 
+00013e60: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00013e70: 6c66 2e65 7272 6f72 5f64 6573 6372 6970  lf.error_descrip
+00013e80: 7469 6f6e 2069 7320 6e6f 7420 4e6f 6e65  tion is not None
+00013e90: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00013ea0: 6520 6622 4a53 4f4e 2072 6573 706f 6e73  e f"JSON respons
+00013eb0: 6520 6d69 7373 6573 2027 6465 7363 7269  e misses 'descri
+00013ec0: 7074 696f 6e27 2066 6965 6c64 3a20 7b72  ption' field: {r
+00013ed0: 6573 706f 6e73 655f 6a73 6f6e 7d22 0a20  esponse_json}". 
+00013ee0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00013ef0: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+00013f00: 5f28 0a20 2020 2020 2020 2020 2020 2066  _(.            f
+00013f10: 227b 6572 726f 725f 7469 746c 657d 2028  "{error_title} (
+00013f20: 7b72 6573 706f 6e73 652e 7572 6c7d 2072  {response.url} r
+00013f30: 6573 706f 6e64 6564 2077 6974 6820 7b72  esponded with {r
+00013f40: 6573 706f 6e73 652e 7374 6174 7573 7d20  esponse.status} 
+00013f50: 7b72 6573 706f 6e73 652e 7265 6173 6f6e  {response.reason
+00013f60: 7d29 222c 0a20 2020 2020 2020 2020 2020  })",.           
+00013f70: 2072 6573 706f 6e73 652c 0a20 2020 2020   response,.     
+00013f80: 2020 2029 0a0a 0a63 6c61 7373 2041 7069     )...class Api
+00013f90: 496e 7661 6c69 644a 534f 4e45 7863 6570  InvalidJSONExcep
+00013fa0: 7469 6f6e 2841 7069 4578 6365 7074 696f  tion(ApiExceptio
+00013fb0: 6e29 3a0a 2020 2020 2222 220a 2020 2020  n):.    """.    
+00013fc0: 5468 6973 2063 6c61 7373 2072 6570 7265  This class repre
+00013fd0: 7365 6e74 7320 616e 2045 7863 6570 7469  sents an Excepti
+00013fe0: 6f6e 2074 6872 6f77 6e20 7768 656e 2061  on thrown when a
+00013ff0: 2063 616c 6c20 746f 2074 6865 0a20 2020   call to the.   
+00014000: 2054 656c 6567 7261 6d20 4150 4920 7365   Telegram API se
+00014010: 7276 6572 2072 6574 7572 6e73 2069 6e76  rver returns inv
+00014020: 616c 6964 206a 736f 6e2e 0a20 2020 2022  alid json..    "
+00014030: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
+00014040: 6974 5f5f 2873 656c 662c 2072 6573 706f  it__(self, respo
+00014050: 6e73 653a 2061 696f 6874 7470 2e43 6c69  nse: aiohttp.Cli
+00014060: 656e 7452 6573 706f 6e73 652c 206a 736f  entResponse, jso
+00014070: 6e5f 7061 7273 696e 675f 6572 726f 723a  n_parsing_error:
+00014080: 2045 7863 6570 7469 6f6e 293a 0a20 2020   Exception):.   
+00014090: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
+000140a0: 6e69 745f 5f28 0a20 2020 2020 2020 2020  nit__(.         
+000140b0: 2020 2022 5468 6520 7365 7276 6572 2072     "The server r
+000140c0: 6574 7572 6e65 6420 616e 2069 6e76 616c  eturned an inval
+000140d0: 6964 204a 534f 4e20 7265 7370 6f6e 7365  id JSON response
+000140e0: 2e20 5265 7370 6f6e 7365 2062 6f64 793a  . Response body:
+000140f0: 220a 2020 2020 2020 2020 2020 2020 2b20  ".            + 
+00014100: 6622 5c6e 5b7b 7265 7370 6f6e 7365 7d5d  f"\n[{response}]
+00014110: 5c6e 4a53 4f4e 2070 6172 7369 6e67 2065  \nJSON parsing e
+00014120: 7272 6f72 3a20 7b6a 736f 6e5f 7061 7273  rror: {json_pars
+00014130: 696e 675f 6572 726f 727d 222c 0a20 2020  ing_error}",.   
+00014140: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+00014150: 652c 0a20 2020 2020 2020 2029 0a20 2020  e,.        ).   
+00014160: 2020 2020 2073 656c 662e 6a73 6f6e 5f70       self.json_p
+00014170: 6172 7369 6e67 5f65 7272 6f72 203d 206a  arsing_error = j
+00014180: 736f 6e5f 7061 7273 696e 675f 6572 726f  son_parsing_erro
+00014190: 720a                                     r.
```

### Comparing `telebot_against_war-0.6.3/telebot/callback_data.py` & `telebot_against_war-0.6.4/telebot/callback_data.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/check_text.py` & `telebot_against_war-0.6.4/telebot/check_text.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/filters.py` & `telebot_against_war-0.6.4/telebot/filters.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/formatting.py` & `telebot_against_war-0.6.4/telebot/formatting.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/graceful_shutdown.py` & `telebot_against_war-0.6.4/telebot/graceful_shutdown.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/helpers.py` & `telebot_against_war-0.6.4/telebot/helpers.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/metrics.py` & `telebot_against_war-0.6.4/telebot/metrics.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/runner.py` & `telebot_against_war-0.6.4/telebot/runner.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/storages/base_storage.py` & `telebot_against_war-0.6.4/telebot/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/storages/memory_storage.py` & `telebot_against_war-0.6.4/telebot/storages/memory_storage.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/storages/pickle_storage.py` & `telebot_against_war-0.6.4/telebot/storages/pickle_storage.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/storages/redis_storage.py` & `telebot_against_war-0.6.4/telebot/storages/redis_storage.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/test_util.py` & `telebot_against_war-0.6.4/telebot/test_util.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/types/__init__.py` & `telebot_against_war-0.6.4/telebot/types/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/types/constants.py` & `telebot_against_war-0.6.4/telebot/types/constants.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/types/service.py` & `telebot_against_war-0.6.4/telebot/types/service.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/util.py` & `telebot_against_war-0.6.4/telebot/util.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/telebot/webhook.py` & `telebot_against_war-0.6.4/telebot/webhook.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.3/PKG-INFO` & `telebot_against_war-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebot-against-war
-Version: 0.6.3
+Version: 0.6.4
 Summary: Async-first fork of pyTelegramBotApi
 Home-page: https://github.com/bots-against-war/telebot
 License: GPL-2.0-only
 Author: Igor Vaiman
 Author-email: gosha.vaiman@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: telebot-against-war Version: 0.6.3 Summary: Async-
+Metadata-Version: 2.1 Name: telebot-against-war Version: 0.6.4 Summary: Async-
 first fork of pyTelegramBotApi Home-page: https://github.com/bots-against-war/
 telebot License: GPL-2.0-only Author: Igor Vaiman Author-email:
 gosha.vaiman@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v2 (GPLv2) Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-
```

