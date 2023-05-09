# Comparing `tmp/py5paisa-0.7.0.tar.gz` & `tmp/py5paisa-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py5paisa-0.7.0.tar", last modified: Mon Apr 10 07:38:21 2023, max compression
+gzip compressed data, was "py5paisa-0.7.1.tar", last modified: Tue May  9 07:48:06 2023, max compression
```

## Comparing `py5paisa-0.7.0.tar` & `py5paisa-0.7.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:38:21.062077 py5paisa-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-10 07:38:12.000000 py5paisa-0.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-10 07:38:12.000000 py5paisa-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 07:38:12.000000 py5paisa-0.7.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-10 07:38:12.000000 py5paisa-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-04-10 07:38:21.062077 py5paisa-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-10 07:38:12.000000 py5paisa-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:38:21.058077 py5paisa-0.7.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:38:21.062077 py5paisa-0.7.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    48489 2023-04-10 07:38:12.000000 py5paisa-0.7.0/docs/images/5-paisa-img.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:38:21.062077 py5paisa-0.7.0/py5paisa/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/order.py
--rw-r--r--   0 runner    (1001) docker     (123)    32425 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/py5paisa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-10 07:38:12.000000 py5paisa-0.7.0/py5paisa/urlconst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:38:21.062077 py5paisa-0.7.0/py5paisa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-04-10 07:38:21.000000 py5paisa-0.7.0/py5paisa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-10 07:38:21.000000 py5paisa-0.7.0/py5paisa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:38:21.000000 py5paisa-0.7.0/py5paisa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:38:21.000000 py5paisa-0.7.0/py5paisa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-10 07:38:21.000000 py5paisa-0.7.0/py5paisa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 07:38:21.000000 py5paisa-0.7.0/py5paisa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-10 07:38:21.062077 py5paisa-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-10 07:38:12.000000 py5paisa-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:38:21.062077 py5paisa-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 07:38:12.000000 py5paisa-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-10 07:38:12.000000 py5paisa-0.7.0/tests/test_py5paisa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:48:06.001703 py5paisa-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 07:47:46.000000 py5paisa-0.7.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-09 07:47:46.000000 py5paisa-0.7.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-09 07:47:46.000000 py5paisa-0.7.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-09 07:47:46.000000 py5paisa-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-05-09 07:48:06.001703 py5paisa-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-09 07:47:46.000000 py5paisa-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:48:05.997703 py5paisa-0.7.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:48:05.997703 py5paisa-0.7.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    48489 2023-05-09 07:47:46.000000 py5paisa-0.7.1/docs/images/5-paisa-img.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:48:05.997703 py5paisa-0.7.1/py5paisa/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34000 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/py5paisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/urlconst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:48:06.001703 py5paisa-0.7.1/py5paisa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-05-09 07:48:05.000000 py5paisa-0.7.1/py5paisa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 07:48:05.000000 py5paisa-0.7.1/py5paisa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:48:05.000000 py5paisa-0.7.1/py5paisa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:48:05.000000 py5paisa-0.7.1/py5paisa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-09 07:48:05.000000 py5paisa-0.7.1/py5paisa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 07:48:05.000000 py5paisa-0.7.1/py5paisa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-09 07:48:06.001703 py5paisa-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-09 07:47:46.000000 py5paisa-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:48:06.001703 py5paisa-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 07:47:46.000000 py5paisa-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 07:47:46.000000 py5paisa-0.7.1/tests/test_py5paisa.py
```

### Comparing `py5paisa-0.7.0/CONTRIBUTING.rst` & `py5paisa-0.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.0/PKG-INFO` & `py5paisa-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py5paisa
-Version: 0.7.0
+Version: 0.7.1
 Summary:  Python SDK for 5paisa APIs natively written in VB.NET
 Home-page: https://github.com/5paisa/py5paisa
 Author: 5paisa
 Author-email: coreteam@5paisa.com
 Keywords: py5paisa
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 ![PyPI](https://img.shields.io/pypi/v/py5paisa)
 ![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/5paisa/py5paisa/Publish%20package/master)
 
 ![5paisa logo](./docs/images/5-paisa-img.jpg)
 
 #### Documentation
 
-Read the docs hosted [here](https://5paisa.github.io/)
+Read the docs hosted [here](https://www.5paisa.com/developerapi/overview)
 
 #### Features
 
 -   Order placement, modification and cancellation
 -   Fetching user info including holdings, positions, margin and order book.
 -   Fetching live market streaming.
 -   Placing, modifying and deleting Bracket Order.
@@ -66,23 +66,22 @@
 # Pass the token received in the response url after successful login to get an access token (this also sets the token for all the APIs you use)-
 
 # Please note that you need to copy the request token from URL and paste in this code and start the code within 30s.
 
 #This function will automatically take care of generating and sending access token for all your API's
 
 client = FivePaisaClient(cred=cred)
-client.get_access_token('Your Response Token')
 
+# New TOTP based authentication
+client.get_totp_session('Your ClientCode','TOTP from authenticator app','Your Pin')
 
-#AUTH Using UserName and Psw - Not Recommended
-Please keep the cred same as above and pass your email,psw and dob
+# If you have the have the token(OAUTH Approach)
+client.get_oauth_session('Your Response Token')
 
-client = FivePaisaClient(email="youremail@gmail.com", passwd="Password", dob="YYYYMMDD",cred=cred)
-client.login()
-After successful authentication, you should get a `Logged in!!` message
+After successful authentication, you should get a `Logged in!!` message in console
 ```
 
 #### Market Feed
 
 ```py
 #NOTE : Symbol has to be in the same format as specified in the example below.
```

### Comparing `py5paisa-0.7.0/README.rst` & `py5paisa-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.0/docs/images/5-paisa-img.jpg` & `py5paisa-0.7.1/docs/images/5-paisa-img.jpg`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.0/py5paisa/auth.py` & `py5paisa-0.7.1/py5paisa/auth.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.0/py5paisa/const.py` & `py5paisa-0.7.1/py5paisa/const.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.0/py5paisa/order.py` & `py5paisa-0.7.1/py5paisa/order.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.0/py5paisa/py5paisa.py` & `py5paisa-0.7.1/py5paisa/py5paisa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,72 +1,70 @@
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 from .auth import EncryptionClient
 from .const import *
-from .order import Order, Bo_co_order,RequestType,Basket_order
+from .order import Order, Bo_co_order, RequestType, Basket_order
 from .logging import log_response
 import json
 import websocket
 import pandas as pd
-import websocket 
-from .urlconst  import *
+import websocket
+from .urlconst import *
 from enum import Enum
 
 
-
 class FivePaisaClient:
-    
-    
-    def __init__(self, email=None, passwd=None, dob=None,cred=None):
+
+    def __init__(self, email=None, passwd=None, dob=None, cred=None):
         """
         Main constructor for client.
         Expects user's email, password and date of birth in YYYYMMDD format.
         """
         try:
             self.email = email
             self.passwd = passwd
             self.dob = dob
             self.client_code = ""
             self.Jwt_token = ""
             self.Aspx_auth = None
-            self.web_url= None
-            self.market_depth_url= None
-            self.Res_Data= None
-            self.ws= None
-            self.access_token= ""
+            self.web_url = None
+            self.market_depth_url = None
+            self.Res_Data = None
+            self.ws = None
+            self.access_token = ""
+            self.request_token = None
             self.session = requests.Session()
-            self.APP_SOURCE=cred["APP_SOURCE"]
-            self.APP_NAME=cred["APP_NAME"]
-            self.USER_ID=cred["USER_ID"]
-            self.PASSWORD=cred["PASSWORD"]
-            self.USER_KEY=cred["USER_KEY"]
-            self.ENCRYPTION_KEY=cred["ENCRYPTION_KEY"]
+            self.APP_SOURCE = cred["APP_SOURCE"]
+            self.APP_NAME = cred["APP_NAME"]
+            self.USER_ID = cred["USER_ID"]
+            self.PASSWORD = cred["PASSWORD"]
+            self.USER_KEY = cred["USER_KEY"]
+            self.ENCRYPTION_KEY = cred["ENCRYPTION_KEY"]
             self.create_payload()
             self.set_url()
-            
+
         except Exception as e:
             log_response(e)
-    
 
     def login(self):
         try:
             encryption_client = EncryptionClient(self.ENCRYPTION_KEY)
             secret_email = encryption_client.encrypt(self.email)
             secret_passwd = encryption_client.encrypt(self.passwd)
             secret_dob = encryption_client.encrypt(self.dob)
             self.login_payload["body"]["Email_id"] = secret_email
             self.login_payload["body"]["Password"] = secret_passwd
             self.login_payload["body"]["My2PIN"] = secret_dob
             self.login_payload["head"]["requestCode"] = "5PLoginV4"
             self.login_payload["head"]["appName"] = self.APP_NAME
             self.login_payload["head"]["key"] = self.USER_KEY
             self.login_payload["head"]["userId"] = self.USER_ID
-            self.login_payload["head"]["password"] = self.PASSWORD  
+            self.login_payload["head"]["password"] = self.PASSWORD
             res = self._login_request(self.LOGIN_ROUTE)
-            
+
             message = res["body"]["Message"]
             if message == "":
                 log_response("Logged in!!")
             else:
                 log_response(message)
             self._set_client_code(res["body"]["ClientCode"])
         except Exception as e:
@@ -95,18 +93,19 @@
             return self._user_info_request("POSITIONS")
         except Exception as e:
             log_response(e)
 
     def _login_request(self, route):
         try:
             requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
-            res = self.session.post(route, json=self.login_payload, headers=HEADERS)
-            resp=res.json()
-            self.Jwt_token=resp["body"]["JWTToken"]
-            self.access_token=self.Jwt_token
+            res = self.session.post(
+                route, json=self.login_payload, headers=HEADERS)
+            resp = res.json()
+            self.Jwt_token = resp["body"]["JWTToken"]
+            self.access_token = self.Jwt_token
             return res.json()
         except Exception as e:
             log_response(e)
 
     def _set_client_code(self, client_code):
         try:
             self.client_code = client_code
@@ -136,82 +135,83 @@
                 url = self.IDEAS_ROUTE
                 return_type = "Data"
             elif data_type == "IT":
                 url = self.IDEAS_ROUTE
                 return_type = "Data"
             else:
                 raise Exception("Invalid data type requested")
-            response = self.session.post(url, json=payload, headers=HEADERS).json()
+            response = self.session.post(
+                url, json=payload, headers=HEADERS).json()
 
             data = response["body"][return_type]
             return data
         except Exception as e:
             log_response(e)
 
     def order_request(self, req_type) -> None:
         try:
             self.payload["body"]["ClientCode"] = self.client_code
             self.payload["head"]["key"] = self.USER_KEY
             HEADERS["Authorization"] = f'Bearer {self.access_token}'
             if req_type == "OP":
                 url = self.ORDER_PLACEMENT_ROUTE
-                #self.payload["head"]["requestCode"] = "5PPlaceOrdReq"
-                if self.access_token != "" :
+                # self.payload["head"]["requestCode"] = "5PPlaceOrdReq"
+                if self.access_token != "":
                     HEADERS["Authorization"] = f'Bearer {self.Jwt_token}'
             elif req_type == "OC":
                 url = self.ORDER_CANCEL_ROUTE
-                #self.payload["head"]["requestCode"] = "5PCancelOrdReq"
-                if self.access_token != "" :
+                # self.payload["head"]["requestCode"] = "5PCancelOrdReq"
+                if self.access_token != "":
                     HEADERS["Authorization"] = f'Bearer {self.Jwt_token}'
             elif req_type == "OM":
                 url = self.ORDER_MODIFY_ROUTE
-                #self.payload["head"]["requestCode"] = "5PModifyOrdReq"
-                if self.access_token != "" :
+                # self.payload["head"]["requestCode"] = "5PModifyOrdReq"
+                if self.access_token != "":
                     HEADERS["Authorization"] = f'Bearer {self.Jwt_token}'
             elif req_type == "OS":
                 url = self.ORDER_STATUS_ROUTE
                 self.payload["head"]["requestCode"] = "5POrdStatus"
             elif req_type == "TI":
                 url = self.TRADE_INFO_ROUTE
                 self.payload["head"]["requestCode"] = "5PTrdInfo"
             elif req_type == "TH":
                 url = self.TRADE_HISTORY_ROUTE
             elif req_type == "MF":
                 url = self.MARKET_FEED_ROUTE
                 self.payload["head"]["requestCode"] = "5PMF"
-                self.payload["body"]["COUNT"]=self.client_code
+                self.payload["body"]["COUNT"] = self.client_code
             elif req_type == "BM":
                 url = self.BRACKET_MOD_ROUTE
-                #self.payload["head"]["requestCode"] = "5PSModMOOrd"
+                # self.payload["head"]["requestCode"] = "5PSModMOOrd"
                 # self.payload["body"]["legtype"]=0
                 # self.payload["body"]["TMOPartnerOrderID"]=0
             elif req_type == "CM":
                 url = self.COVER_MOD_ROUTE
             elif req_type == "CO":
                 url = self.COVER_ORDER_ROUTE
             elif req_type == "MS":
                 url = self.MARKET_STATUS_ROUTE
             elif req_type == "BO":
                 url = self.BRACKET_ORDER_ROUTE
-           
+
                 # self.payload["head"]["requestCode"] = "5PSMOOrd"
                 # self.payload["body"]["OrderRequesterCode"]=self.client_code
             elif req_type == "BC":
                 url = self.BRACKET_CANCEL_ROUTE
             elif req_type == "CC":
                 url = self.COVER_CANCEL_ROUTE
             elif req_type == "MD":
                 url = self.MARKET_DEPTH_ROUTE
-                #self.payload["head"]["requestCode"] = "5PMD"
+                # self.payload["head"]["requestCode"] = "5PMD"
             elif req_type == "MDS":
                 url = self.MARKET_DEPTH_BY_SYMBOL_ROUTE
-                #self.payload["head"]["requestCode"] = "5PMD"
+                # self.payload["head"]["requestCode"] = "5PMD"
             elif req_type == "TB":
                 url = self.TRADEBOOK_ROUTE
-                #self.payload["head"]["requestCode"] = "5PTrdBkV1"
+                # self.payload["head"]["requestCode"] = "5PTrdBkV1"
             elif req_type == "GB":
                 url = self.GET_BASKET_ROUTE
             elif req_type == "CB":
                 url = self.CREATE_BASKET_ROUTE
             elif req_type == "RB":
                 url = self.RENAME_BASKET_ROUTE
             elif req_type == "DB":
@@ -234,56 +234,57 @@
                 url = self.SQUAREOFF_ROUTE
             elif req_type == "PO":
                 url = self.POSITION_CONVERSION_ROUTE
             else:
                 raise Exception("Invalid request type!")
             res = self.session.post(url, json=self.payload,
                                     headers=HEADERS).json()
-          
+
             if req_type == "MS":
                 log_response(res["head"]["statusDescription"])
             else:
                 log_response(res["body"]["Message"])
             return res["body"]
-            
+
         except Exception as e:
             log_response(e)
 
-    def fetch_order_status(self, req_list:list) :
+    def fetch_order_status(self, req_list: list):
         try:
             self.payload["body"]["OrdStatusReqList"] = req_list
             return self.order_request("OS")
         except Exception as e:
             log_response(e)
 
-    def fetch_trade_info(self, req_list:list) :
+    def fetch_trade_info(self, req_list: list):
         try:
             self.payload["body"]["TradeInformationList"] = req_list
             return self.order_request("TI")
         except Exception as e:
             log_response(e)
 
-    def fetch_market_depth(self, req_list:list):
+    def fetch_market_depth(self, req_list: list):
         try:
-            self.payload["body"]["Count"]="1"
-            self.payload["body"]["Data"]=req_list
-        
+            self.payload["body"]["Count"] = "1"
+            self.payload["body"]["Data"] = req_list
+
             return self.order_request("MD")
         except Exception as e:
             log_response(e)
-    def fetch_market_depth_by_symbol(self, req_list:list):
+
+    def fetch_market_depth_by_symbol(self, req_list: list):
         try:
-            self.payload["body"]["Count"]="1"
-            self.payload["body"]["Data"]=req_list
-        
+            self.payload["body"]["Count"] = "1"
+            self.payload["body"]["Data"] = req_list
+
             return self.order_request("MDS")
         except Exception as e:
             log_response(e)
-    
-    def fetch_market_feed(self, req_list:list) :
+
+    def fetch_market_feed(self, req_list: list):
         """
             market feed api
         """
         try:
             self.payload["body"]["MarketFeedData"] = req_list
             self.payload["body"]["ClientLoginType"] = 0
             self.payload["body"]["LastRequestTime"] = f"/Date({TODAY_TIMESTAMP})/"
@@ -291,20 +292,19 @@
             return self.order_request("MF")
         except Exception as e:
             log_response(e)
 
     def set_payload(self, order) -> None:
         try:
             for key, value in order.items():
-               self.payload["body"][key] = value
+                self.payload["body"][key] = value
         except Exception as e:
             log_response(e)
-        
-        
-    def set_payload_bo(self,boco)-> None:
+
+    def set_payload_bo(self, boco) -> None:
         """
             this is for bo-co order placement
         """
         try:
             self.payload["body"]["RequestType"] = boco.RequestType
             self.payload["body"]["BuySell"] = boco.BuySell
             self.payload["body"]["Qty"] = boco.Qty
@@ -330,15 +330,15 @@
             self.payload["body"]["LocalOrderIDLimit"] = boco.LocalOrderIDLimit
             self.payload["body"]["PublicIP"] = boco.public_ip
             self.payload["body"]["AppSource"] = self.APP_SOURCE
             self.payload["body"]["TradedQty"] = boco.traded_qty
         except Exception as e:
             log_response(e)
 
-    def set_basket_payload(self,basket_order:Basket_order,basket_list:list)-> None:
+    def set_basket_payload(self, basket_order: Basket_order, basket_list: list) -> None:
         """
             this is for Basket order placement
         """
         try:
             self.payload["body"]["Exchange"] = basket_order.Exchange
             self.payload["body"]["ExchangeType"] = basket_order.ExchangeType
             self.payload["body"]["Price"] = basket_order.Price
@@ -348,477 +348,514 @@
             self.payload["body"]["AtMarket"] = basket_order.AtMarket
             self.payload["body"]["StopLossPrice"] = basket_order.StopLossPrice
             self.payload["body"]["IsStopLossOrder"] = basket_order.IsStopLossOrder
             self.payload["body"]["IOCOrder"] = basket_order.IOCOrder
             self.payload["body"]["DelvIntra"] = basket_order.DelvIntra
             self.payload["body"]["AppSource"] = self.APP_SOURCE
             self.payload["body"]["IsIntraday"] = basket_order.IsIntraday
-            self.payload["body"]["ValidTillDate"] =f"/Date({NEXT_DAY_TIMESTAMP})/"
+            self.payload["body"]["ValidTillDate"] = f"/Date({NEXT_DAY_TIMESTAMP})/"
             self.payload["body"]["AHPlaced"] = basket_order.AHPlaced
             self.payload["body"]["PublicIP"] = basket_order.PublicIP
             self.payload["body"]["DisQty"] = basket_order.DisQty
             self.payload["body"]["iOrderValidity"] = basket_order.iOrderValidity
             self.payload["body"]["BasketIDs"] = basket_list
         except Exception as e:
             log_response(e)
 
-
     def place_order(self, **order):
         """
         Places a fresh order
         """
         try:
-            if(order['Price'] >= 0 and order["ScripCode"] and order['Exchange'] and order['OrderType'] and order['Qty'] and order['ExchangeType']):
+            if (order['Price'] >= 0 and order["ScripCode"] and order['Exchange'] and order['OrderType'] and order['Qty'] and order['ExchangeType']):
                 self.set_payload(order)
                 return self.order_request("OP")
             else:
                 return log_response("please enter valid input")
-            
+
         except Exception as e:
             log_response(e)
 
     def modify_order(self, **order):
         """
         Modifies an existing order
         """
         try:
-            if(order['Price'] and order['ExchOrderID']):
+            if (order['Price'] and order['ExchOrderID']):
                 self.set_payload(order)
                 return self.order_request("OM")
         except Exception as e:
             log_response(e)
 
-    def cancel_order(self,exch_order_id:str):
+    def cancel_order(self, exch_order_id: str):
         """
         Cancels an existing order
         """
         try:
-            self.payload["body"]["ExchOrderID"]=exch_order_id
+            self.payload["body"]["ExchOrderID"] = exch_order_id
             return self.order_request("OC")
         except Exception as e:
             log_response(e)
 
-    def bo_order(self,**order):
+    def bo_order(self, **order):
         try:
-            if( order["ScripCode"] and order['Exchange'] and order['OrderType'] and order['Qty'] and order['ExchangeType']):
+            if (order["ScripCode"] and order['Exchange'] and order['OrderType'] and order['Qty'] and order['ExchangeType']):
                 self.set_payload(order)
                 return self.order_request("BO")
         except Exception as e:
             log_response(e)
 
-    def modify_bo_order(self,**order):
+    def modify_bo_order(self, **order):
         try:
-            if(order['ExchangeOrderID']):
+            if (order['ExchangeOrderID']):
                 self.set_payload(order)
                 # self.payload["body"]["TriggerPriceForSL"] = order.stoploss_price
                 return self.order_request("BM")
         except Exception as e:
             log_response(e)
-    
-    def cancel_bo_order(self,**order):
+
+    def cancel_bo_order(self, **order):
         try:
-            if(order['ExchangeOrderID']):
+            if (order['ExchangeOrderID']):
                 self.set_payload(order)
                 # self.payload["body"]["TriggerPriceForSL"] = order.stoploss_price
                 return self.order_request("BC")
         except Exception as e:
             log_response(e)
-    
-    def cover_order(self,**order):
+
+    def cover_order(self, **order):
         try:
             self.set_payload(order)
            # self.payload["body"]["TriggerPriceForSL"] = order.stoploss_price
             return self.order_request("CO")
         except Exception as e:
             log_response(e)
-    
-    def modify_cover_order(self,**order):
+
+    def modify_cover_order(self, **order):
         try:
             self.set_payload(order)
            # self.payload["body"]["TriggerPriceForSL"] = order.stoploss_price
             return self.order_request("CM")
         except Exception as e:
             log_response(e)
-    
-    def cancel_cover_order(self,**order):
+
+    def cancel_cover_order(self, **order):
         try:
             self.set_payload(order)
            # self.payload["body"]["TriggerPriceForSL"] = order.stoploss_price
             return self.order_request("CC")
         except Exception as e:
             log_response(e)
-    def Request_Feed(self,Method:str,Operation:str,req_list:list):
+
+    def Request_Feed(self, Method: str, Operation: str, req_list: list):
         try:
-            Method_dict={"mf":"MarketFeedV3","md":"MarketDepthService","oi":"GetScripInfoForFuture","i":"Indices"}
-            Operation_dict={"s":"Subscribe","u":"Unsubscribe"}
-        
-            self.ws_payload['Method']=Method_dict[Method]
-            self.ws_payload['Operation']=Operation_dict[Operation]
-            self.ws_payload['ClientCode']=self.client_code
-            self.ws_payload['MarketFeedData']=req_list
+            Method_dict = {"mf": "MarketFeedV3", "md": "MarketDepthService",
+                           "oi": "GetScripInfoForFuture", "i": "Indices"}
+            Operation_dict = {"s": "Subscribe", "u": "Unsubscribe"}
+
+            self.ws_payload['Method'] = Method_dict[Method]
+            self.ws_payload['Operation'] = Operation_dict[Operation]
+            self.ws_payload['ClientCode'] = self.client_code
+            self.ws_payload['MarketFeedData'] = req_list
             return self.ws_payload
         except Exception as e:
             log_response(e)
-    
-    def connect(self,wspayload:dict):
+
+    def connect(self, wspayload: dict):
         try:
-            self.web_url=f'wss://openfeed.5paisa.com/Feeds/api/chat?Value1={self.Jwt_token}|{self.client_code}'
-            
+            self.web_url = f'wss://openfeed.5paisa.com/Feeds/api/chat?Value1={self.Jwt_token}|{self.client_code}'
+
             def on_open(ws):
                 log_response("Streaming Started")
-                try: 
+                try:
                     ws.send(json.dumps(wspayload))
                 except Exception as e:
                     log_response(e)
             self.ws = websocket.WebSocketApp(self.web_url)
 
-            self.ws.on_open=on_open
+            self.ws.on_open = on_open
         except Exception as e:
             log_response(e)
-       
-    
-        
-    def send_data(self,open_:any):
+
+    def send_data(self, open_: any):
         try:
-            self.ws.on_open=open_
+            self.ws.on_open = open_
         except Exception as e:
             log_response(e)
 
-    def receive_data(self,msg:any):
+    def receive_data(self, msg: any):
         try:
-            self.ws.on_message=msg
+            self.ws.on_message = msg
             self.ws.run_forever()
         except Exception as e:
             log_response(e)
 
     def close_data(self):
         try:
             self.ws.close()
         except Exception as e:
             log_response(e)
 
-    def error_data(self,err:any):
+    def error_data(self, err: any):
         try:
-            self.ws.on_error=err
+            self.ws.on_error = err
         except Exception as e:
             log_response(e)
-        
+
     def Login_check(self):
         try:
-            self.login_check_payload["head"]["key"]=self.USER_KEY
-            self.login_check_payload["head"]["appName"]=self.APP_NAME
-            self.login_check_payload["head"]["LoginId"]=self.client_code
-            self.login_check_payload["body"]["RegistrationID"]=self.Jwt_token
-            url=self.LOGIN_CHECK_ROUTE
-            resl=requests.post(url, json=self.login_check_payload,headers=HEADERS)
-            self.Aspx_auth = resl.cookies.get('.ASPXAUTH',domain='openfeed.5paisa.com')
-            
+            self.login_check_payload["head"]["key"] = self.USER_KEY
+            self.login_check_payload["head"]["appName"] = self.APP_NAME
+            self.login_check_payload["head"]["LoginId"] = self.client_code
+            self.login_check_payload["body"]["RegistrationID"] = self.Jwt_token
+            url = self.LOGIN_CHECK_ROUTE
+            resl = requests.post(
+                url, json=self.login_check_payload, headers=HEADERS)
+            self.Aspx_auth = resl.cookies.get(
+                '.ASPXAUTH', domain='openfeed.5paisa.com')
+
             return f'.ASPXAUTH={self.Aspx_auth}'
         except Exception as e:
             log_response(e)
 
     def jwt_validate(self):
         try:
-            self.jwt_payload['ClientCode']=self.client_code
-            self.jwt_payload['JwtCode']=self.Jwt_token
-            url=self.JWT_VALIDATION_ROUTE
-            response = self.session.post(url, json=self.jwt_payload, headers=HEADERS).json()
-            
+            self.jwt_payload['ClientCode'] = self.client_code
+            self.jwt_payload['JwtCode'] = self.Jwt_token
+            url = self.JWT_VALIDATION_ROUTE
+            response = self.session.post(
+                url, json=self.jwt_payload, headers=HEADERS).json()
+
             return response['body']['Message']
         except Exception as e:
             log_response(e)
 
-    def historical_data(self,Exch:str,ExchangeSegment:str,ScripCode: int,time: str,From:str,To: str):
+    def historical_data(self, Exch: str, ExchangeSegment: str, ScripCode: int, time: str, From: str, To: str):
         try:
-            self.jwt_headers['x-clientcode']=self.client_code
-            self.jwt_headers['x-auth-token']=self.Jwt_token
-            url=f'{self.HISTORICAL_DATA_ROUTE}{Exch}/{ExchangeSegment}/{ScripCode}/{time}?from={From}&end={To}'
-            timeList=['1m','5m','10m','15m','30m','60m','1d']
+            self.jwt_headers['x-clientcode'] = self.client_code
+            self.jwt_headers['x-auth-token'] = self.Jwt_token
+            url = f'{self.HISTORICAL_DATA_ROUTE}{Exch}/{ExchangeSegment}/{ScripCode}/{time}?from={From}&end={To}'
+            timeList = ['1m', '3m','5m', '10m', '15m', '30m', '60m', '1d']
             if time not in timeList:
                 return 'Invalid Time Frame. it should be within [1m,5m,10m,15m,30m,60m,1d].'
             else:
-                response = self.session.get(url, headers=self.jwt_headers).json()
-                candleList=response['data']['candles']
-                df=pd.DataFrame(candleList)
+                response = self.session.get(
+                    url, headers=self.jwt_headers).json()
+                candleList = response['data']['candles']
+                df = pd.DataFrame(candleList)
                 if df.empty != True:
-                    df.columns=['Datetime','Open','High','Low','Close','Volume']
+                    df.columns = ['Datetime', 'Open',
+                                  'High', 'Low', 'Close', 'Volume']
                 return df
 
         except Exception as e:
             log_response(e)
 
     def get_buy(self):
         try:
-            res=self._user_info_request("IB")
+            res = self._user_info_request("IB")
             if len(res) > 0:
                 message = res[0]["payload"]
                 res1 = json.loads(message)
-                with pd.option_context('display.max_columns',None,'display.max_rows',None):
-                    df=pd.DataFrame(res1)
+                with pd.option_context('display.max_columns', None, 'display.max_rows', None):
+                    df = pd.DataFrame(res1)
                 return df
             else:
-                message ="You don't have an active Ultra-Trader-Pack. Please subscribe to it to avail the services."
+                message = "You don't have an active Ultra-Trader-Pack. Please subscribe to it to avail the services."
                 return message
         except Exception as e:
             log_response(e)
 
     def get_trade(self):
         try:
-            res=self._user_info_request("IT")
+            res = self._user_info_request("IT")
             if len(res) > 0:
                 message = res[1]["payload"]
                 res1 = json.loads(message)
-                with pd.option_context('display.max_columns',None,'display.max_rows',None):
-                    df=pd.DataFrame(res1)
+                with pd.option_context('display.max_columns', None, 'display.max_rows', None):
+                    df = pd.DataFrame(res1)
                 return df
             else:
-                message ="You don't have an active Ultra-Trader-Pack. Please subscribe to it to avail the services."
+                message = "You don't have an active Ultra-Trader-Pack. Please subscribe to it to avail the services."
                 return message
         except Exception as e:
             log_response(e)
 
-
     def get_tradebook(self):
         try:
             return self.order_request("TB")
         except Exception as e:
             log_response(e)
 
     def set_url(self):
         try:
-            self.LOGIN_ROUTE=LOGIN_ROUTE
-            self.MARGIN_ROUTE=MARGIN_ROUTE
-            self.ORDER_BOOK_ROUTE=ORDER_BOOK_ROUTE
-            self.HOLDINGS_ROUTE=HOLDINGS_ROUTE
-            self.POSITIONS_ROUTE=POSITIONS_ROUTE
-            self.ORDER_PLACEMENT_ROUTE=ORDER_PLACEMENT_ROUTE
-            self.ORDER_MODIFY_ROUTE=ORDER_MODIFY_ROUTE
-            self.ORDER_CANCEL_ROUTE=ORDER_CANCEL_ROUTE
-            self.ORDER_STATUS_ROUTE=ORDER_STATUS_ROUTE
-            self.TRADE_INFO_ROUTE=TRADE_INFO_ROUTE
-            self.BRACKET_MOD_ROUTE=BRACKET_MOD_ROUTE
-            self.BRACKET_ORDER_ROUTE=BRACKET_ORDER_ROUTE
-            self.BRACKET_CANCEL_ROUTE=BRACKET_CANCEL_ROUTE
-            self.COVER_MOD_ROUTE=COVER_MOD_ROUTE
-            self.COVER_ORDER_ROUTE=COVER_ORDER_ROUTE
-            self.COVER_CANCEL_ROUTE=COVER_CANCEL_ROUTE
-            self.MARKET_FEED_ROUTE=MARKET_FEED_ROUTE
-            self.LOGIN_CHECK_ROUTE=LOGIN_CHECK_ROUTE
-            self.MARKET_DEPTH_ROUTE=MARKET_DEPTH_ROUTE
-            self.JWT_VALIDATION_ROUTE=JWT_VALIDATION_ROUTE
-            self.HISTORICAL_DATA_ROUTE=HISTORICAL_DATA_ROUTE
-            self.IDEAS_ROUTE=IDEAS_ROUTE
-            self.TRADEBOOK_ROUTE=TRADEBOOK_ROUTE
-            self.ACCESS_TOKEN_ROUTE=ACCESS_TOKEN_ROUTE
-            self.MARKET_STATUS_ROUTE=MARKET_STATUS_ROUTE
-            self.TRADE_HISTORY_ROUTE=TRADE_HISTORY_ROUTE
-            self.GET_BASKET_ROUTE=GET_BASKET_ROUTE
-            self.CREATE_BASKET_ROUTE=CREATE_BASKET_ROUTE
-            self.RENAME_BASKET_ROUTE=RENAME_BASKET_ROUTE
-            self.DELETE_BASKET_ROUTE=DELETE_BASKET_ROUTE
-            self.CLONE_BASKET_ROUTE=CLONE_BASKET_ROUTE
-            self.EXECUTE_BASKET_ROUTE=EXECUTE_BASKET_ROUTE
-            self.GET_ORDER_IN_BASKET_ROUTE=GET_ORDER_IN_BASKET_ROUTE
-            self.ADD_BASKET_ORDER_ROUTE=ADD_BASKET_ORDER_ROUTE
-            self.OPTION_CHAIN_ROUTE=OPTION_CHAIN_ROUTE
-            self.GET_OPTION_CHAIN_ROUTE=GET_OPTION_CHAIN_ROUTE
-            self.CANCEL_BULK_ORDER_ROUTE=CANCEL_BULK_ORDER_ROUTE
-            self.SQUAREOFF_ROUTE=SQUAREOFF_ROUTE
-            self.MARKET_DEPTH_ROUTE_20=MARKET_DEPTH_ROUTE_20
-            self.POSITION_CONVERSION_ROUTE=POSITION_CONVERSION_ROUTE
-            self.MARKET_DEPTH_BY_SYMBOL_ROUTE=MARKET_DEPTH_BY_SYMBOL_ROUTE
+            self.LOGIN_ROUTE = LOGIN_ROUTE
+            self.MARGIN_ROUTE = MARGIN_ROUTE
+            self.ORDER_BOOK_ROUTE = ORDER_BOOK_ROUTE
+            self.HOLDINGS_ROUTE = HOLDINGS_ROUTE
+            self.POSITIONS_ROUTE = POSITIONS_ROUTE
+            self.ORDER_PLACEMENT_ROUTE = ORDER_PLACEMENT_ROUTE
+            self.ORDER_MODIFY_ROUTE = ORDER_MODIFY_ROUTE
+            self.ORDER_CANCEL_ROUTE = ORDER_CANCEL_ROUTE
+            self.ORDER_STATUS_ROUTE = ORDER_STATUS_ROUTE
+            self.TRADE_INFO_ROUTE = TRADE_INFO_ROUTE
+            self.BRACKET_MOD_ROUTE = BRACKET_MOD_ROUTE
+            self.BRACKET_ORDER_ROUTE = BRACKET_ORDER_ROUTE
+            self.BRACKET_CANCEL_ROUTE = BRACKET_CANCEL_ROUTE
+            self.COVER_MOD_ROUTE = COVER_MOD_ROUTE
+            self.COVER_ORDER_ROUTE = COVER_ORDER_ROUTE
+            self.COVER_CANCEL_ROUTE = COVER_CANCEL_ROUTE
+            self.MARKET_FEED_ROUTE = MARKET_FEED_ROUTE
+            self.LOGIN_CHECK_ROUTE = LOGIN_CHECK_ROUTE
+            self.MARKET_DEPTH_ROUTE = MARKET_DEPTH_ROUTE
+            self.JWT_VALIDATION_ROUTE = JWT_VALIDATION_ROUTE
+            self.HISTORICAL_DATA_ROUTE = HISTORICAL_DATA_ROUTE
+            self.IDEAS_ROUTE = IDEAS_ROUTE
+            self.TRADEBOOK_ROUTE = TRADEBOOK_ROUTE
+            self.ACCESS_TOKEN_ROUTE = ACCESS_TOKEN_ROUTE
+            self.GET_REQUEST_TOKEN_ROUTE = GET_REQUEST_TOKEN_ROUTE
+            self.MARKET_STATUS_ROUTE = MARKET_STATUS_ROUTE
+            self.TRADE_HISTORY_ROUTE = TRADE_HISTORY_ROUTE
+            self.GET_BASKET_ROUTE = GET_BASKET_ROUTE
+            self.CREATE_BASKET_ROUTE = CREATE_BASKET_ROUTE
+            self.RENAME_BASKET_ROUTE = RENAME_BASKET_ROUTE
+            self.DELETE_BASKET_ROUTE = DELETE_BASKET_ROUTE
+            self.CLONE_BASKET_ROUTE = CLONE_BASKET_ROUTE
+            self.EXECUTE_BASKET_ROUTE = EXECUTE_BASKET_ROUTE
+            self.GET_ORDER_IN_BASKET_ROUTE = GET_ORDER_IN_BASKET_ROUTE
+            self.ADD_BASKET_ORDER_ROUTE = ADD_BASKET_ORDER_ROUTE
+            self.OPTION_CHAIN_ROUTE = OPTION_CHAIN_ROUTE
+            self.GET_OPTION_CHAIN_ROUTE = GET_OPTION_CHAIN_ROUTE
+            self.CANCEL_BULK_ORDER_ROUTE = CANCEL_BULK_ORDER_ROUTE
+            self.SQUAREOFF_ROUTE = SQUAREOFF_ROUTE
+            self.MARKET_DEPTH_ROUTE_20 = MARKET_DEPTH_ROUTE_20
+            self.POSITION_CONVERSION_ROUTE = POSITION_CONVERSION_ROUTE
+            self.MARKET_DEPTH_BY_SYMBOL_ROUTE = MARKET_DEPTH_BY_SYMBOL_ROUTE
         except Exception as e:
             log_response(e)
-    
 
     def create_payload(self):
         try:
             self.payload = GENERIC_PAYLOAD
             self.login_payload = LOGIN_PAYLOAD
-            self.login_check_payload= LOGIN_CHECK_PAYLOAD
-            self.ws_payload=WS_PAYLOAD
-            self.jwt_headers=JWT_HEADERS
-            self.jwt_payload=JWT_PAYLOAD
-            self.SOCKET_DEPTH_PAYLOAD=SOCKET_DEPTH_PAYLOAD
+            self.login_check_payload = LOGIN_CHECK_PAYLOAD
+            self.ws_payload = WS_PAYLOAD
+            self.jwt_headers = JWT_HEADERS
+            self.jwt_payload = JWT_PAYLOAD
+            self.SOCKET_DEPTH_PAYLOAD = SOCKET_DEPTH_PAYLOAD
         except Exception as e:
             log_response(e)
-        
-    def get_access_token(self,request_token):
+
+    def get_oauth_session(self, request_token):
+        try:
+            return self.get_access_token(request_token)
+        except Exception as e:
+            log_response(e)
+
+    def get_access_token(self, request_token):
         try:
             self.payload["head"]["Key"] = self.USER_KEY
             self.payload["body"]["RequestToken"] = request_token
             self.payload["body"]["EncryKey"] = self.ENCRYPTION_KEY
             self.payload["body"]["UserId"] = self.USER_ID
-            url=ACCESS_TOKEN_ROUTE
+            url = ACCESS_TOKEN_ROUTE
 
             res = self.session.post(url, json=self.payload).json()
             message = res["body"]["Message"]
-         
+
             if message == "Success":
-                self.access_token=res["body"]["AccessToken"]
+                self.access_token = res["body"]["AccessToken"]
                 self.Jwt_token = self.access_token
                 self._set_client_code(res["body"]["ClientCode"])
                 log_response("Logged in!!")
                 return self.access_token
             else:
                 log_response(message)
         except Exception as e:
             log_response(e)
 
+    def get_request_token(self, client_code, totp, pin):
+        try:
+            self.payload["head"]["Key"] = self.USER_KEY
+            self.payload["body"]["Email_ID"] = client_code
+            self.payload["body"]["TOTP"] = totp
+            self.payload["body"]["PIN"] = pin
+            url = GET_REQUEST_TOKEN_ROUTE
+
+            res = self.session.post(url, json=self.payload).json()
+            message = res["body"]["Status"]
+
+            if message == 0:
+                self.request_token = res["body"]["RequestToken"]
+                log_response("RequestToken: "+self.request_token)
+                return self.request_token
+            else:
+                log_response(res["body"])
+        except Exception as e:
+            log_response(e)
+
+    def get_totp_session(self, client_code, totp, pin):
+        try:
+            self.get_request_token(client_code, totp, pin)
+            if self.request_token is not None:
+                return self.get_oauth_session(self.request_token)
+        except Exception as e:
+            log_response(e)
+
     def get_market_status(self):
         try:
-            market_status_response=self.order_request("MS")
+            market_status_response = self.order_request("MS")
             return market_status_response["Data"]
         except Exception as e:
             log_response(e)
 
-    def get_trade_history(self,exchange_id):
+    def get_trade_history(self, exchange_id):
         try:
             self.payload["body"]["ExchOrderID"] = exchange_id
             if self.client_code != None:
                 return self.order_request("TH")
         except Exception as e:
             log_response(e)
 
     def get_basket(self):
         try:
             if self.client_code != None:
-                #self.payload["body"]["ClientCode"] = self.client_code
+                # self.payload["body"]["ClientCode"] = self.client_code
                 return self.order_request("GB")
         except Exception as e:
             log_response(e)
 
-    def create_basket(self,basket_name:str):
+    def create_basket(self, basket_name: str):
         try:
             if self.client_code != None:
                 self.payload["body"]["BasketName"] = basket_name
                 return self.order_request("CB")
         except Exception as e:
             log_response(e)
 
-    def rename_basket(self,basket_name:str,basket_id:int):
+    def rename_basket(self, basket_name: str, basket_id: int):
         try:
             if self.client_code != None:
                 self.payload["body"]["NewBasketName"] = basket_name
                 self.payload["body"]["BasketID"] = basket_id
                 return self.order_request("RB")
         except Exception as e:
             log_response(e)
 
-    def delete_basket(self,basket_id:list):
+    def delete_basket(self, basket_id: list):
         try:
             if self.client_code != None:
                 self.payload["body"]["BasketIDs"] = basket_id
                 return self.order_request("DB")
         except Exception as e:
             log_response(e)
 
-    def clone_basket(self,basket_id:int):
+    def clone_basket(self, basket_id: int):
         try:
             if self.client_code != None:
                 self.payload["body"]["BasketID"] = basket_id
                 return self.order_request("CL")
         except Exception as e:
             log_response(e)
 
-    def execute_basket(self,basket_id:int):
+    def execute_basket(self, basket_id: int):
         try:
             if self.client_code != None:
                 self.payload["body"]["BasketID"] = basket_id
                 return self.order_request("EB")
         except Exception as e:
             log_response(e)
 
-    def get_order_in_basket(self,basket_id:int):
+    def get_order_in_basket(self, basket_id: int):
         try:
             if self.client_code != None:
                 self.payload["body"]["BasketID"] = basket_id
                 return self.order_request("GO")
         except Exception as e:
             log_response(e)
 
-    def add_basket_order(self,basket_order:Basket_order,basket_list:list):
+    def add_basket_order(self, basket_order: Basket_order, basket_list: list):
         try:
             if self.client_code != None:
-                self.set_basket_payload(basket_order,basket_list)
+                self.set_basket_payload(basket_order, basket_list)
                 return self.order_request("AB")
         except Exception as e:
             log_response(e)
 
-    def get_expiry(self,exch:str,symbol:str):
+    def get_expiry(self, exch: str, symbol: str):
         try:
             self.payload["body"]["Exch"] = exch
             self.payload["body"]["Symbol"] = symbol
             return self.order_request("GE")
         except Exception as e:
             log_response(e)
 
-    def get_option_chain(self,exch:str,symbol:str,expire:int):
+    def get_option_chain(self, exch: str, symbol: str, expire: int):
         try:
             self.payload["body"]["Exch"] = exch
             self.payload["body"]["Symbol"] = symbol
             self.payload["body"]["ExpiryDate"] = f"/Date({expire})/"
             return self.order_request("GOC")
         except Exception as e:
             log_response(e)
 
-    def cancel_bulk_order(self,ExchOrderIDs:list):
+    def cancel_bulk_order(self, ExchOrderIDs: list):
         try:
             if self.client_code != None:
                 self.payload["body"]["ExchOrderIDs"] = ExchOrderIDs
             return self.order_request("CBO")
         except Exception as e:
             log_response(e)
 
     def squareoff_all(self):
         try:
             if self.client_code != None:
                 return self.order_request("SO")
         except Exception as e:
             log_response(e)
 
-    def position_convertion(self,Exch:str,ExchType:str,ScripData:str,TradeType:str,ConvertQty:int,ConvertFrom:str,ConvertTo:str):
+    def position_convertion(self, Exch: str, ExchType: str, ScripData: str, TradeType: str, ConvertQty: int, ConvertFrom: str, ConvertTo: str):
         try:
             if self.client_code != None:
                 self.payload["body"]["Exch"] = Exch
                 self.payload["body"]["ExchType"] = ExchType
                 self.payload["body"]["ScripData"] = ScripData
                 self.payload["body"]["TradeType"] = TradeType
                 self.payload["body"]["ConvertQty"] = ConvertQty
                 self.payload["body"]["ConvertFrom"] = ConvertFrom
                 self.payload["body"]["ConvertTo"] = ConvertTo
                 return self.order_request("PO")
         except Exception as e:
             log_response(e)
 
-    def socket_20_depth(self,socket_payload:dict):
+    def socket_20_depth(self, socket_payload: dict):
         try:
-            self.token=self.market_depth_token()
+            self.token = self.market_depth_token()
             """
             self.SOCKET_DEPTH_PAYLOAD["operation"]=operation
             self.SOCKET_DEPTH_PAYLOAD["method"]=method
             self.SOCKET_DEPTH_PAYLOAD["instruments"]=instruments
             """
-            self.subscription_key=SUBSCRIPTION_KEY
-            
+            self.subscription_key = SUBSCRIPTION_KEY
+
+            self.market_depth_url = f'wss://openapi.5paisa.com/ws?subscription-key={self.subscription_key}&access_token={self.token}'
 
-            self.market_depth_url=f'wss://openapi.5paisa.com/ws?subscription-key={self.subscription_key}&access_token={self.token}'
-            
             def on_open(ws):
-                
+
                 try:
                     ws.send(json.dumps(socket_payload))
                 except Exception as e:
                     log_response(e)
-                   
-            self.ws = websocket.WebSocketApp(self.market_depth_url,on_open=on_open)
-            #self.ws.run_forever()
+
+            self.ws = websocket.WebSocketApp(
+                self.market_depth_url, on_open=on_open)
+            # self.ws.run_forever()
         except Exception as e:
             log_response(e)
 
     def market_depth_token(self):
         try:
-            response = self.session.post(self.MARKET_DEPTH_ROUTE_20, headers=self.jwt_headers).json()
+            response = self.session.post(
+                self.MARKET_DEPTH_ROUTE_20, headers=self.jwt_headers).json()
             return response["access_token"]
         except Exception as e:
             log_response(e)
-
```

### Comparing `py5paisa-0.7.0/py5paisa/strategy.py` & `py5paisa-0.7.1/py5paisa/strategy.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.0/py5paisa.egg-info/PKG-INFO` & `py5paisa-0.7.1/py5paisa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py5paisa
-Version: 0.7.0
+Version: 0.7.1
 Summary:  Python SDK for 5paisa APIs natively written in VB.NET
 Home-page: https://github.com/5paisa/py5paisa
 Author: 5paisa
 Author-email: coreteam@5paisa.com
 Keywords: py5paisa
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 ![PyPI](https://img.shields.io/pypi/v/py5paisa)
 ![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/5paisa/py5paisa/Publish%20package/master)
 
 ![5paisa logo](./docs/images/5-paisa-img.jpg)
 
 #### Documentation
 
-Read the docs hosted [here](https://5paisa.github.io/)
+Read the docs hosted [here](https://www.5paisa.com/developerapi/overview)
 
 #### Features
 
 -   Order placement, modification and cancellation
 -   Fetching user info including holdings, positions, margin and order book.
 -   Fetching live market streaming.
 -   Placing, modifying and deleting Bracket Order.
@@ -66,23 +66,22 @@
 # Pass the token received in the response url after successful login to get an access token (this also sets the token for all the APIs you use)-
 
 # Please note that you need to copy the request token from URL and paste in this code and start the code within 30s.
 
 #This function will automatically take care of generating and sending access token for all your API's
 
 client = FivePaisaClient(cred=cred)
-client.get_access_token('Your Response Token')
 
+# New TOTP based authentication
+client.get_totp_session('Your ClientCode','TOTP from authenticator app','Your Pin')
 
-#AUTH Using UserName and Psw - Not Recommended
-Please keep the cred same as above and pass your email,psw and dob
+# If you have the have the token(OAUTH Approach)
+client.get_oauth_session('Your Response Token')
 
-client = FivePaisaClient(email="youremail@gmail.com", passwd="Password", dob="YYYYMMDD",cred=cred)
-client.login()
-After successful authentication, you should get a `Logged in!!` message
+After successful authentication, you should get a `Logged in!!` message in console
 ```
 
 #### Market Feed
 
 ```py
 #NOTE : Symbol has to be in the same format as specified in the example below.
```

### Comparing `py5paisa-0.7.0/setup.py` & `py5paisa-0.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,10 +45,10 @@
     keywords='py5paisa',
     name='py5paisa',
     packages=find_packages(include=['py5paisa', 'py5paisa.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/5paisa/py5paisa',
-    version='0.7.0',
+    version='0.7.1',
     zip_safe=False,
 )
```

