# Comparing `tmp/dxsp-2.1.0.tar.gz` & `tmp/dxsp-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.1.0.tar", max compression
+gzip compressed data, was "dxsp-2.1.1.tar", max compression
```

## Comparing `dxsp-2.1.0.tar` & `dxsp-2.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-09 19:27:31.057859 dxsp-2.1.0/LICENSE
--rw-r--r--   0        0        0     2595 2023-05-09 19:27:31.057859 dxsp-2.1.0/README.md
--rw-r--r--   0        0        0       86 2023-05-09 19:27:31.733866 dxsp-2.1.0/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-09 19:27:31.057859 dxsp-2.1.0/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-09 19:27:31.057859 dxsp-2.1.0/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-09 19:27:31.057859 dxsp-2.1.0/dxsp/config.py
--rw-r--r--   0        0        0     3386 2023-05-09 19:27:31.057859 dxsp-2.1.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    26120 2023-05-09 19:27:31.057859 dxsp-2.1.0/dxsp/main.py
--rw-r--r--   0        0        0     1790 2023-05-09 19:27:31.733866 dxsp-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 dxsp-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-09 19:42:26.468027 dxsp-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2595 2023-05-09 19:42:26.468027 dxsp-2.1.1/README.md
+-rw-r--r--   0        0        0       86 2023-05-09 19:42:27.160035 dxsp-2.1.1/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-09 19:42:26.468027 dxsp-2.1.1/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-09 19:42:26.468027 dxsp-2.1.1/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-09 19:42:26.468027 dxsp-2.1.1/dxsp/config.py
+-rw-r--r--   0        0        0     3386 2023-05-09 19:42:26.468027 dxsp-2.1.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    26104 2023-05-09 19:42:26.468027 dxsp-2.1.1/dxsp/main.py
+-rw-r--r--   0        0        0     1790 2023-05-09 19:42:27.160035 dxsp-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 dxsp-2.1.1/PKG-INFO
```

### Comparing `dxsp-2.1.0/LICENSE` & `dxsp-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.0/README.md` & `dxsp-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.0/dxsp/assets/blockchains.py` & `dxsp-2.1.1/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.0/dxsp/default_settings.toml` & `dxsp-2.1.1/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.0/dxsp/main.py` & `dxsp-2.1.1/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         amount=1
     ):
         try:
             asset_out_amount = self.w3.to_wei(amount, 'ether')
             quote_url = (
                 settings.dex_1inch_url
                 + "/"
-                + str(settings.chain_id)
+                + str(self.chain_id)
                 + "/quote?fromTokenAddress="
                 + str(asset_in_address)
                 + "&toTokenAddress="
                 + str(asset_out_address)
                 + "&amount="
                 + str(asset_out_amount))
             quote_response = await self._get(quote_url)
@@ -296,15 +296,15 @@
         asset_out_address,
         asset_in_address,
         amount
     ):
         swap_url = (
             settings.dex_1inch_url
             + "/"
-            + str(settings.chain_id)
+            + str(self.chain_id)
             + "/swap?fromTokenAddress="
             + asset_out_address
             + "&toTokenAddress="
             + asset_in_address
             + "&amount="
             + amount
             + "&fromAddress="
@@ -494,26 +494,26 @@
             return None
 
     async def get_approve_1inch(self, asset_out_address):
         try:
             approval_check_URL = (
                 settings.dex_1inch_url
                 + "/"
-                + str(settings.chain_id)
+                + str(self.chain_id)
                 + "/approve/allowance?tokenAddress="
                 + str(asset_out_address)
                 + "&walletAddress="
                 + str(self.wallet_address))
             approval_response = await self._get(approval_check_URL)
             approval_check = approval_response['allowance']
             if (approval_check == 0):
                 approval_URL = (
                     settings.dex_1inch_url
                     + "/"
-                    + str(settings.chain_id)
+                    + str(self.chain_id)
                     + "/approve/transaction?tokenAddress="
                     + str(asset_out_address))
                 approval_response = await self._get(approval_URL)
                 return approval_response
         except Exception as e:
             self.logger.error("get_approve_uniswap %s", e)
             return None
```

### Comparing `dxsp-2.1.0/pyproject.toml` & `dxsp-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.1.0"
+version = "2.1.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.1.0/PKG-INFO` & `dxsp-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.1.0
+Version: 2.1.1
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

