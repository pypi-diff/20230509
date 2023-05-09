# Comparing `tmp/dcentrapi-0.2.0.tar.gz` & `tmp/dcentrapi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.2.0.tar", last modified: Fri May  5 09:42:17 2023, max compression
+gzip compressed data, was "dist/dcentrapi-0.2.1.tar", last modified: Tue May  9 14:22:57 2023, max compression
```

## Comparing `dcentrapi-0.2.0.tar` & `dcentrapi-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-05 09:42:17.171879 dcentrapi-0.2.0/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.2.0/LICENSE.rst
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-05-05 09:42:17.171736 dcentrapi-0.2.0/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.2.0/README.md
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-05 09:42:17.170924 dcentrapi-0.2.0/dcentrapi/
--rw-r--r--   0 nivshitrit   (501) staff       (20)      851 2023-03-08 10:39:09.000000 dcentrapi-0.2.0/dcentrapi/Base.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      280 2023-03-08 10:39:09.000000 dcentrapi-0.2.0/dcentrapi/__init__.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)       63 2023-05-05 09:42:13.000000 dcentrapi-0.2.0/dcentrapi/common.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     8597 2023-05-03 13:07:34.000000 dcentrapi-0.2.0/dcentrapi/eventPolling.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      491 2023-03-02 14:02:13.000000 dcentrapi-0.2.0/dcentrapi/gasMonitor.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.2.0/dcentrapi/merkleTree.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3140 2023-04-04 11:41:50.000000 dcentrapi-0.2.0/dcentrapi/rpcAggregation.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1232 2023-05-05 09:41:46.000000 dcentrapi-0.2.0/dcentrapi/web3Index.py
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-05 09:42:17.171566 dcentrapi-0.2.0/dcentrapi.egg-info/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-05-05 09:42:17.000000 dcentrapi-0.2.0/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)      379 2023-05-05 09:42:17.000000 dcentrapi-0.2.0/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-05-05 09:42:17.000000 dcentrapi-0.2.0/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-05-05 09:42:17.000000 dcentrapi-0.2.0/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-05-05 09:42:17.000000 dcentrapi-0.2.0/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-05-05 09:42:17.171919 dcentrapi-0.2.0/setup.cfg
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1167 2023-04-09 07:57:53.000000 dcentrapi-0.2.0/setup.py
+drwxr-xr-x   0 jovanvuleta   (501) staff       (20)        0 2023-05-09 14:22:57.625557 dcentrapi-0.2.1/
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     1073 2022-06-21 11:33:40.000000 dcentrapi-0.2.1/LICENSE.rst
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     6741 2023-05-09 14:22:57.625350 dcentrapi-0.2.1/PKG-INFO
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     6211 2022-09-26 09:54:00.000000 dcentrapi-0.2.1/README.md
+drwxr-xr-x   0 jovanvuleta   (501) staff       (20)        0 2023-05-09 14:22:57.624147 dcentrapi-0.2.1/dcentrapi/
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)      851 2023-05-09 13:35:14.000000 dcentrapi-0.2.1/dcentrapi/Base.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)      280 2023-05-09 13:35:14.000000 dcentrapi-0.2.1/dcentrapi/__init__.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)       63 2023-05-09 14:21:51.000000 dcentrapi-0.2.1/dcentrapi/common.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     8228 2023-05-09 14:21:51.000000 dcentrapi-0.2.1/dcentrapi/eventPolling.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)      491 2023-05-09 13:35:14.000000 dcentrapi-0.2.1/dcentrapi/gasMonitor.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     3078 2023-05-09 13:35:14.000000 dcentrapi-0.2.1/dcentrapi/merkleTree.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     3140 2023-05-09 13:35:14.000000 dcentrapi-0.2.1/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     1232 2023-05-09 13:35:14.000000 dcentrapi-0.2.1/dcentrapi/web3Index.py
+drwxr-xr-x   0 jovanvuleta   (501) staff       (20)        0 2023-05-09 14:22:57.625067 dcentrapi-0.2.1/dcentrapi.egg-info/
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     6741 2023-05-09 14:22:57.000000 dcentrapi-0.2.1/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)      379 2023-05-09 14:22:57.000000 dcentrapi-0.2.1/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)        1 2023-05-09 14:22:57.000000 dcentrapi-0.2.1/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)        9 2023-05-09 14:22:57.000000 dcentrapi-0.2.1/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)       10 2023-05-09 14:22:57.000000 dcentrapi-0.2.1/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)       38 2023-05-09 14:22:57.625621 dcentrapi-0.2.1/setup.cfg
+-rw-r--r--   0 jovanvuleta   (501) staff       (20)     1167 2023-05-09 13:35:14.000000 dcentrapi-0.2.1/setup.py
```

### Comparing `dcentrapi-0.2.0/LICENSE.rst` & `dcentrapi-0.2.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.0/PKG-INFO` & `dcentrapi-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Dcentralab Pypi packages
-Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -105,9 +103,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `dcentrapi-0.2.0/README.md` & `dcentrapi-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.0/dcentrapi/Base.py` & `dcentrapi-0.2.1/dcentrapi/Base.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.0/dcentrapi/eventPolling.py` & `dcentrapi-0.2.1/dcentrapi/eventPolling.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,59 +16,52 @@
         url = self.url + "event_polling/get_latest_contract_version"
         data = {
             "contract_name": contract_name
         }
         response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
-    def set_schema(self, contract_name, contract_version, abi):
-        url = self.url + "event_polling/schema"
-        data = {
-            "contract_name": contract_name,
-            "contract_version": contract_version,
-            "abi": abi
-        }
-        response = requests.post(url, json=data, headers=self.headers)
-        return response.json()
-
-    def add_collection_contract(self, contract_address, schema_id, network_name, collection_name):
-        url = self.url + "event_polling/collection_contract"
+    def register_user(self, user_name: str, collection_name: str):
+        url = self.url + "event_polling/register_user"
         data = {
-            "contract_address": contract_address,
-            "schema_id": schema_id,
-            "network_name": network_name,
-            "collection_name": collection_name
+            "user_name": user_name,
+            "collection_name": collection_name,
         }
         response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
-    def subscribe_contract(self, contract_name, contract_address, network, abi, collection_name, contract_version=None):
+    def subscribe_contract(
+            self, contract_name, contract_address, network,
+            abi, collection_name, contract_version=None, git_tag=None
+    ):
         url = self.url + "event_polling/subscribe_contract"
         data = {
             "contract_name": contract_name,
             "contract_address": contract_address,
             "contract_version": contract_version,
             "network": network,
             "collection_name": collection_name,
-            "abi": abi
-
+            "abi": abi,
+            "git_tag": git_tag
         }
         response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
     def get_schema(self, contract_name, contract_version):
         url = self.url + "event_polling/schema"
         data = {
             "contract_name": contract_name,
             "contract_version": contract_version
         }
         response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
-    def get_events_sum_of_values_in_range(self, collection_name, contract_address, event_name, field_name, start_time, end_time):
+    def get_events_sum_of_values_in_range(
+        self, collection_name, contract_address, event_name, field_name, start_time, end_time
+    ):
         url = self.url + "event_polling/events_sum_of_values_in_range"
         data = {
             "collection_name": collection_name,
             "contract_address": contract_address,
             "event_name": event_name,
             "field_name": field_name,
             "start_time": start_time,
@@ -165,15 +158,18 @@
             "contract_address": contract_address,
             "start_time": start_time,
             "end_time": end_time
         }
         response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
-    def get_contracts_events_info(self, collection_name, contract_addresses, event_names, user_web3_addresses = None, start_time=None, end_time=None):
+    def get_contracts_events_info(
+            self, collection_name, contract_addresses, event_names,
+            user_web3_addresses = None, start_time=None, end_time=None
+    ):
         url = self.url + "event_polling/contracts_events_info"
         data = {
             "collection_name": collection_name,
             "contract_addresses": contract_addresses,
             "start_time": start_time,
             "end_time": end_time,
             "user_web3_addresses": user_web3_addresses,
```

### Comparing `dcentrapi-0.2.0/dcentrapi/merkleTree.py` & `dcentrapi-0.2.1/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.0/dcentrapi/rpcAggregation.py` & `dcentrapi-0.2.1/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.0/dcentrapi/web3Index.py` & `dcentrapi-0.2.1/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.0/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.2.1/dcentrapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Dcentralab Pypi packages
-Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -105,9 +103,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `dcentrapi-0.2.0/setup.py` & `dcentrapi-0.2.1/setup.py`

 * *Files identical despite different names*

