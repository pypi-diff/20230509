# Comparing `tmp/dxsp-2.1.1.tar.gz` & `tmp/dxsp-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.1.1.tar", max compression
+gzip compressed data, was "dxsp-2.1.2.tar", max compression
```

## Comparing `dxsp-2.1.1.tar` & `dxsp-2.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-09 19:42:26.468027 dxsp-2.1.1/LICENSE
--rw-r--r--   0        0        0     2595 2023-05-09 19:42:26.468027 dxsp-2.1.1/README.md
--rw-r--r--   0        0        0       86 2023-05-09 19:42:27.160035 dxsp-2.1.1/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-09 19:42:26.468027 dxsp-2.1.1/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-09 19:42:26.468027 dxsp-2.1.1/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-09 19:42:26.468027 dxsp-2.1.1/dxsp/config.py
--rw-r--r--   0        0        0     3386 2023-05-09 19:42:26.468027 dxsp-2.1.1/dxsp/default_settings.toml
--rw-r--r--   0        0        0    26104 2023-05-09 19:42:26.468027 dxsp-2.1.1/dxsp/main.py
--rw-r--r--   0        0        0     1790 2023-05-09 19:42:27.160035 dxsp-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 dxsp-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-09 19:58:03.728835 dxsp-2.1.2/LICENSE
+-rw-r--r--   0        0        0     2595 2023-05-09 19:58:03.728835 dxsp-2.1.2/README.md
+-rw-r--r--   0        0        0       86 2023-05-09 19:58:04.660841 dxsp-2.1.2/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-09 19:58:03.728835 dxsp-2.1.2/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-09 19:58:03.728835 dxsp-2.1.2/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-09 19:58:03.728835 dxsp-2.1.2/dxsp/config.py
+-rw-r--r--   0        0        0     3386 2023-05-09 19:58:03.728835 dxsp-2.1.2/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    26016 2023-05-09 19:58:03.728835 dxsp-2.1.2/dxsp/main.py
+-rw-r--r--   0        0        0     1790 2023-05-09 19:58:04.660841 dxsp-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 dxsp-2.1.2/PKG-INFO
```

### Comparing `dxsp-2.1.1/LICENSE` & `dxsp-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.1/README.md` & `dxsp-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.1/dxsp/assets/blockchains.py` & `dxsp-2.1.2/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.1/dxsp/default_settings.toml` & `dxsp-2.1.2/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.1/dxsp/main.py` & `dxsp-2.1.2/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         asset_out_address,
         amount=1
     ):
         try:
             asset_out_amount = self.w3.to_wei(amount, 'ether')
             quote_url = (
                 settings.dex_1inch_url
-                + "/"
                 + str(self.chain_id)
                 + "/quote?fromTokenAddress="
                 + str(asset_in_address)
                 + "&toTokenAddress="
                 + str(asset_out_address)
                 + "&amount="
                 + str(asset_out_amount))
@@ -295,15 +294,14 @@
         self,
         asset_out_address,
         asset_in_address,
         amount
     ):
         swap_url = (
             settings.dex_1inch_url
-            + "/"
             + str(self.chain_id)
             + "/swap?fromTokenAddress="
             + asset_out_address
             + "&toTokenAddress="
             + asset_in_address
             + "&amount="
             + amount
@@ -493,26 +491,24 @@
             self.logger.error("get_approve %s", e)
             return None
 
     async def get_approve_1inch(self, asset_out_address):
         try:
             approval_check_URL = (
                 settings.dex_1inch_url
-                + "/"
                 + str(self.chain_id)
                 + "/approve/allowance?tokenAddress="
                 + str(asset_out_address)
                 + "&walletAddress="
                 + str(self.wallet_address))
             approval_response = await self._get(approval_check_URL)
             approval_check = approval_response['allowance']
             if (approval_check == 0):
                 approval_URL = (
                     settings.dex_1inch_url
-                    + "/"
                     + str(self.chain_id)
                     + "/approve/transaction?tokenAddress="
                     + str(asset_out_address))
                 approval_response = await self._get(approval_URL)
                 return approval_response
         except Exception as e:
             self.logger.error("get_approve_uniswap %s", e)
```

### Comparing `dxsp-2.1.1/pyproject.toml` & `dxsp-2.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.1.1"
+version = "2.1.2"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.1.1/PKG-INFO` & `dxsp-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.1.1
+Version: 2.1.2
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

