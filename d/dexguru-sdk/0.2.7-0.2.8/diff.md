# Comparing `tmp/dexguru-sdk-0.2.7.tar.gz` & `tmp/dexguru-sdk-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexguru-sdk-0.2.7.tar", last modified: Thu Feb 23 15:01:34 2023, max compression
+gzip compressed data, was "dexguru-sdk-0.2.8.tar", last modified: Tue May  9 16:28:44 2023, max compression
```

## Comparing `dexguru-sdk-0.2.7.tar` & `dexguru-sdk-0.2.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-02-23 15:01:34.561606 dexguru-sdk-0.2.7/
--rw-r--r--   0 shestakoven   (501) staff       (20)     1068 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/LICENSE
--rw-r--r--   0 shestakoven   (501) staff       (20)     3588 2023-02-23 15:01:34.561449 dexguru-sdk-0.2.7/PKG-INFO
--rw-r--r--   0 shestakoven   (501) staff       (20)     3040 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/README.md
-drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-02-23 15:01:34.558157 dexguru-sdk-0.2.7/dexguru_sdk/
--rw-r--r--   0 shestakoven   (501) staff       (20)      445 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/dexguru_sdk/__init__.py
-drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-02-23 15:01:34.559375 dexguru-sdk-0.2.7/dexguru_sdk/client/
--rw-r--r--   0 shestakoven   (501) staff       (20)        0 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/dexguru_sdk/client/__init__.py
--rw-r--r--   0 shestakoven   (501) staff       (20)     4410 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/dexguru_sdk/client/aiohttp_client.py
--rw-r--r--   0 shestakoven   (501) staff       (20)      323 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/dexguru_sdk/client/exceptions.py
-drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-02-23 15:01:34.560442 dexguru-sdk-0.2.7/dexguru_sdk/models/
--rw-r--r--   0 shestakoven   (501) staff       (20)      404 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/dexguru_sdk/models/__init__.py
--rw-r--r--   0 shestakoven   (501) staff       (20)      225 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/dexguru_sdk/models/amm_models.py
--rw-r--r--   0 shestakoven   (501) staff       (20)      339 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/dexguru_sdk/models/chain_models.py
--rw-r--r--   0 shestakoven   (501) staff       (20)     1412 2023-02-23 14:42:41.000000 dexguru-sdk-0.2.7/dexguru_sdk/models/choices.py
--rw-r--r--   0 shestakoven   (501) staff       (20)     1121 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/dexguru_sdk/models/swaps_burns_mints_models.py
--rw-r--r--   0 shestakoven   (501) staff       (20)     1382 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/dexguru_sdk/models/token_models.py
--rw-r--r--   0 shestakoven   (501) staff       (20)      364 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/dexguru_sdk/models/wallet_models.py
-drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-02-23 15:01:34.560659 dexguru-sdk-0.2.7/dexguru_sdk/sdk/
--rw-r--r--   0 shestakoven   (501) staff       (20)       22 2023-02-23 14:44:30.000000 dexguru-sdk-0.2.7/dexguru_sdk/sdk/__init__.py
--rw-r--r--   0 shestakoven   (501) staff       (20)    18146 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/dexguru_sdk/sdk/dg_sdk.py
-drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-02-23 15:01:34.560904 dexguru-sdk-0.2.7/dexguru_sdk/utils/
--rw-r--r--   0 shestakoven   (501) staff       (20)        0 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/dexguru_sdk/utils/__init__.py
--rw-r--r--   0 shestakoven   (501) staff       (20)      227 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/dexguru_sdk/utils/get_query.py
-drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-02-23 15:01:34.559054 dexguru-sdk-0.2.7/dexguru_sdk.egg-info/
--rw-r--r--   0 shestakoven   (501) staff       (20)     3588 2023-02-23 15:01:34.000000 dexguru-sdk-0.2.7/dexguru_sdk.egg-info/PKG-INFO
--rw-r--r--   0 shestakoven   (501) staff       (20)      723 2023-02-23 15:01:34.000000 dexguru-sdk-0.2.7/dexguru_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 shestakoven   (501) staff       (20)        1 2023-02-23 15:01:34.000000 dexguru-sdk-0.2.7/dexguru_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 shestakoven   (501) staff       (20)       50 2023-02-23 15:01:34.000000 dexguru-sdk-0.2.7/dexguru_sdk.egg-info/requires.txt
--rw-r--r--   0 shestakoven   (501) staff       (20)       18 2023-02-23 15:01:34.000000 dexguru-sdk-0.2.7/dexguru_sdk.egg-info/top_level.txt
--rw-r--r--   0 shestakoven   (501) staff       (20)       38 2023-02-23 15:01:34.561645 dexguru-sdk-0.2.7/setup.cfg
--rw-r--r--   0 shestakoven   (501) staff       (20)      862 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/setup.py
-drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-02-23 15:01:34.561111 dexguru-sdk-0.2.7/tests/
--rw-r--r--   0 shestakoven   (501) staff       (20)        0 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/tests/__init__.py
--rw-r--r--   0 shestakoven   (501) staff       (20)    17156 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.7/tests/test_sdk.py
+drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-05-09 16:28:44.708755 dexguru-sdk-0.2.8/
+-rw-r--r--   0 shestakoven   (501) staff       (20)     1068 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.8/LICENSE
+-rw-r--r--   0 shestakoven   (501) staff       (20)     3551 2023-05-09 16:28:44.708602 dexguru-sdk-0.2.8/PKG-INFO
+-rw-r--r--   0 shestakoven   (501) staff       (20)     3040 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/README.md
+drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-05-09 16:28:44.705062 dexguru-sdk-0.2.8/dexguru_sdk/
+-rw-r--r--   0 shestakoven   (501) staff       (20)      445 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/dexguru_sdk/__init__.py
+drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-05-09 16:28:44.706297 dexguru-sdk-0.2.8/dexguru_sdk/client/
+-rw-r--r--   0 shestakoven   (501) staff       (20)        0 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/dexguru_sdk/client/__init__.py
+-rw-r--r--   0 shestakoven   (501) staff       (20)     4484 2023-05-09 16:00:02.000000 dexguru-sdk-0.2.8/dexguru_sdk/client/aiohttp_client.py
+-rw-r--r--   0 shestakoven   (501) staff       (20)      323 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/dexguru_sdk/client/exceptions.py
+drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-05-09 16:28:44.707584 dexguru-sdk-0.2.8/dexguru_sdk/models/
+-rw-r--r--   0 shestakoven   (501) staff       (20)      404 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/dexguru_sdk/models/__init__.py
+-rw-r--r--   0 shestakoven   (501) staff       (20)      225 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/dexguru_sdk/models/amm_models.py
+-rw-r--r--   0 shestakoven   (501) staff       (20)      339 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/dexguru_sdk/models/chain_models.py
+-rw-r--r--   0 shestakoven   (501) staff       (20)     1412 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/dexguru_sdk/models/choices.py
+-rw-r--r--   0 shestakoven   (501) staff       (20)     1121 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/dexguru_sdk/models/swaps_burns_mints_models.py
+-rw-r--r--   0 shestakoven   (501) staff       (20)     1382 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/dexguru_sdk/models/token_models.py
+-rw-r--r--   0 shestakoven   (501) staff       (20)      364 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/dexguru_sdk/models/wallet_models.py
+drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-05-09 16:28:44.707889 dexguru-sdk-0.2.8/dexguru_sdk/sdk/
+-rw-r--r--   0 shestakoven   (501) staff       (20)       22 2023-05-09 14:21:11.000000 dexguru-sdk-0.2.8/dexguru_sdk/sdk/__init__.py
+-rw-r--r--   0 shestakoven   (501) staff       (20)    18146 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/dexguru_sdk/sdk/dg_sdk.py
+drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-05-09 16:28:44.708155 dexguru-sdk-0.2.8/dexguru_sdk/utils/
+-rw-r--r--   0 shestakoven   (501) staff       (20)        0 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/dexguru_sdk/utils/__init__.py
+-rw-r--r--   0 shestakoven   (501) staff       (20)      227 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/dexguru_sdk/utils/get_query.py
+drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-05-09 16:28:44.705863 dexguru-sdk-0.2.8/dexguru_sdk.egg-info/
+-rw-r--r--   0 shestakoven   (501) staff       (20)     3551 2023-05-09 16:28:44.000000 dexguru-sdk-0.2.8/dexguru_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 shestakoven   (501) staff       (20)      723 2023-05-09 16:28:44.000000 dexguru-sdk-0.2.8/dexguru_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shestakoven   (501) staff       (20)        1 2023-05-09 16:28:44.000000 dexguru-sdk-0.2.8/dexguru_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shestakoven   (501) staff       (20)       50 2023-05-09 16:28:44.000000 dexguru-sdk-0.2.8/dexguru_sdk.egg-info/requires.txt
+-rw-r--r--   0 shestakoven   (501) staff       (20)       18 2023-05-09 16:28:44.000000 dexguru-sdk-0.2.8/dexguru_sdk.egg-info/top_level.txt
+-rw-r--r--   0 shestakoven   (501) staff       (20)       38 2023-05-09 16:28:44.708788 dexguru-sdk-0.2.8/setup.cfg
+-rw-r--r--   0 shestakoven   (501) staff       (20)      921 2023-05-09 16:26:32.000000 dexguru-sdk-0.2.8/setup.py
+drwxr-xr-x   0 shestakoven   (501) staff       (20)        0 2023-05-09 16:28:44.708367 dexguru-sdk-0.2.8/tests/
+-rw-r--r--   0 shestakoven   (501) staff       (20)        0 2023-02-23 14:40:25.000000 dexguru-sdk-0.2.8/tests/__init__.py
+-rw-r--r--   0 shestakoven   (501) staff       (20)    17156 2023-03-06 17:19:36.000000 dexguru-sdk-0.2.8/tests/test_sdk.py
```

### Comparing `dexguru-sdk-0.2.7/LICENSE` & `dexguru-sdk-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dexguru-sdk-0.2.7/PKG-INFO` & `dexguru-sdk-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dexguru-sdk
-Version: 0.2.7
-Summary: UNKNOWN
+Version: 0.2.8
 Home-page: https://dex.guru
 License: MIT License
 Project-URL: Documentation, https://docs.dex.guru
 Project-URL: GitHub, https://github.com/dex-guru/dg-sdk-python
 Project-URL: Discord, https://discord.com/invite/dPW8fzwzz9
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -137,9 +135,7 @@
         txs = await sdk.get_wallet_transactions(chain_id=1, wallet_address=wallet)
         result.append(txs)
     return result
 
 if __name__ == '__main__':
     result = asyncio.run(get_txs_from_list_of_wallets(wallets))
 ```
-
-
```

### Comparing `dexguru-sdk-0.2.7/README.md` & `dexguru-sdk-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `dexguru-sdk-0.2.7/dexguru_sdk/client/aiohttp_client.py` & `dexguru-sdk-0.2.8/dexguru_sdk/client/aiohttp_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import logging
+import os
 import ssl
 from typing import AnyStr, Optional
 from urllib.parse import urljoin
 
 import aiohttp
 import ujson
 from aiohttp import ClientTimeout
@@ -23,16 +24,17 @@
 
 
 class HTTPClient:
 
     def __init__(self, headers: dict, domain: HttpUrl):
         headers = headers or {}
         default_headers = {
-            'User-Agent': f"Python DexGuru SDK v{sdk.__version__} ",
+            "User-Agent": f"Python DexGuru SDK v{sdk.__version__} ",
             "Content-Type": "application/json",
+            "x-sys-key": os.environ.get('X_SYS_KEY', 'system'),
         }
         self.headers = {**default_headers, **headers}
         self.timeout = ClientTimeout(total=60 * 60, connect=60 * 60, sock_connect=60 * 60, sock_read=60 * 60)
         self.retries_count = 0
         self.retry_sleep = 1.5
         self.domain = domain
```

### Comparing `dexguru-sdk-0.2.7/dexguru_sdk/models/choices.py` & `dexguru-sdk-0.2.8/dexguru_sdk/models/choices.py`

 * *Files identical despite different names*

### Comparing `dexguru-sdk-0.2.7/dexguru_sdk/models/swaps_burns_mints_models.py` & `dexguru-sdk-0.2.8/dexguru_sdk/models/swaps_burns_mints_models.py`

 * *Files identical despite different names*

### Comparing `dexguru-sdk-0.2.7/dexguru_sdk/models/token_models.py` & `dexguru-sdk-0.2.8/dexguru_sdk/models/token_models.py`

 * *Files identical despite different names*

### Comparing `dexguru-sdk-0.2.7/dexguru_sdk/sdk/dg_sdk.py` & `dexguru-sdk-0.2.8/dexguru_sdk/sdk/dg_sdk.py`

 * *Files identical despite different names*

### Comparing `dexguru-sdk-0.2.7/dexguru_sdk.egg-info/PKG-INFO` & `dexguru-sdk-0.2.8/dexguru_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dexguru-sdk
-Version: 0.2.7
-Summary: UNKNOWN
+Version: 0.2.8
 Home-page: https://dex.guru
 License: MIT License
 Project-URL: Documentation, https://docs.dex.guru
 Project-URL: GitHub, https://github.com/dex-guru/dg-sdk-python
 Project-URL: Discord, https://discord.com/invite/dPW8fzwzz9
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -137,9 +135,7 @@
         txs = await sdk.get_wallet_transactions(chain_id=1, wallet_address=wallet)
         result.append(txs)
     return result
 
 if __name__ == '__main__':
     result = asyncio.run(get_txs_from_list_of_wallets(wallets))
 ```
-
-
```

### Comparing `dexguru-sdk-0.2.7/dexguru_sdk.egg-info/SOURCES.txt` & `dexguru-sdk-0.2.8/dexguru_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dexguru-sdk-0.2.7/setup.py` & `dexguru-sdk-0.2.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,19 @@
     name='dexguru-sdk',
     version=__version__,
     url='https://dex.guru',
     packages=find_packages(),
     license='MIT License',
     long_description_content_type='text/markdown',
     long_description=open(join(dirname(__file__), 'README.md')).read(),
-    install_requires=open('requirements.txt').read(),
+    install_requires=[
+        'pydantic==1.8.2',
+        'aiohttp==3.7.4.post0',
+        'ujson==4.0.2',
+    ],
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
     test_suite='tests',
```

### Comparing `dexguru-sdk-0.2.7/tests/test_sdk.py` & `dexguru-sdk-0.2.8/tests/test_sdk.py`

 * *Files identical despite different names*

