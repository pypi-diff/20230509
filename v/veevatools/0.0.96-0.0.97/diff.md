# Comparing `tmp/veevatools-0.0.96.tar.gz` & `tmp/veevatools-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veevatools-0.0.96.tar", last modified: Mon May  8 01:33:45 2023, max compression
+gzip compressed data, was "veevatools-0.0.97.tar", last modified: Tue May  9 05:56:54 2023, max compression
```

## Comparing `veevatools-0.0.96.tar` & `veevatools-0.0.97.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.629585 veevatools-0.0.96/
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      651 2022-10-24 16:14:29.000000 veevatools-0.0.96/LICENSE.txt
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       37 2022-10-24 16:14:29.000000 veevatools-0.0.96/MANIFEST.in
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     6385 2023-05-08 01:33:45.629846 veevatools-0.0.96/PKG-INFO
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     6079 2022-10-24 16:14:29.000000 veevatools-0.0.96/README.md
-drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.612831 veevatools-0.0.96/salesforce/
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       72 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/__init__.py
-drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.614184 veevatools-0.0.96/salesforce/custom_exceptions/
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      139 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/custom_exceptions/__init__.py
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     3345 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/custom_exceptions/salesforce_exceptions.py
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      268 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/decorators.py
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)   104150 2023-05-08 01:26:39.000000 veevatools-0.0.96/salesforce/salesforce.py
-drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.616949 veevatools-0.0.96/salesforce/utilities/
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      295 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/utilities/__init__.py
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      685 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/utilities/async_utils.py
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     3827 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/utilities/df_utils.py
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     2055 2023-05-03 02:20:42.000000 veevatools-0.0.96/salesforce/utilities/sf_query_processors.py
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      757 2023-05-08 01:33:45.631214 veevatools-0.0.96/setup.cfg
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       37 2022-10-24 16:14:29.000000 veevatools-0.0.96/setup.py
-drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.621230 veevatools-0.0.96/veevanetwork/
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       40 2022-10-24 16:14:29.000000 veevatools-0.0.96/veevanetwork/__init__.py
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)        0 2022-10-24 16:14:29.000000 veevatools-0.0.96/veevanetwork/api.py
-drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.622832 veevatools-0.0.96/veevanetwork/custom_exceptions/
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      145 2022-10-24 16:14:29.000000 veevatools-0.0.96/veevanetwork/custom_exceptions/__init__.py
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     3793 2022-10-24 16:14:29.000000 veevatools-0.0.96/veevanetwork/custom_exceptions/veevanetwork_exceptions.py
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)   122066 2022-10-24 16:14:29.000000 veevatools-0.0.96/veevanetwork/network_api_v25.json
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)    80088 2023-01-30 16:08:51.000000 veevatools-0.0.96/veevanetwork/veevanetwork.py
-drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.627445 veevatools-0.0.96/veevatools.egg-info/
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     6385 2023-05-08 01:33:45.000000 veevatools-0.0.96/veevatools.egg-info/PKG-INFO
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      792 2023-05-08 01:33:45.000000 veevatools-0.0.96/veevatools.egg-info/SOURCES.txt
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)        1 2023-05-08 01:33:45.000000 veevatools-0.0.96/veevatools.egg-info/dependency_links.txt
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      166 2023-05-08 01:33:45.000000 veevatools-0.0.96/veevatools.egg-info/requires.txt
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       35 2023-05-08 01:33:45.000000 veevatools-0.0.96/veevatools.egg-info/top_level.txt
-drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.628894 veevatools-0.0.96/veevavault/
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       36 2022-10-24 16:14:29.000000 veevatools-0.0.96/veevavault/__init__.py
--rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     8954 2023-03-06 16:42:47.000000 veevatools-0.0.96/veevavault/veevavault.py
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-09 05:56:54.288769 veevatools-0.0.97/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      651 2022-10-24 16:14:29.000000 veevatools-0.0.97/LICENSE.txt
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       37 2022-10-24 16:14:29.000000 veevatools-0.0.97/MANIFEST.in
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     6385 2023-05-09 05:56:54.289082 veevatools-0.0.97/PKG-INFO
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     6079 2022-10-24 16:14:29.000000 veevatools-0.0.97/README.md
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-09 05:56:54.268674 veevatools-0.0.97/salesforce/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       72 2022-10-24 16:14:29.000000 veevatools-0.0.97/salesforce/__init__.py
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-09 05:56:54.272058 veevatools-0.0.97/salesforce/custom_exceptions/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      139 2022-10-24 16:14:29.000000 veevatools-0.0.97/salesforce/custom_exceptions/__init__.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     3345 2022-10-24 16:14:29.000000 veevatools-0.0.97/salesforce/custom_exceptions/salesforce_exceptions.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      268 2022-10-24 16:14:29.000000 veevatools-0.0.97/salesforce/decorators.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)   105095 2023-05-09 05:55:15.000000 veevatools-0.0.97/salesforce/salesforce.py
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-09 05:56:54.275650 veevatools-0.0.97/salesforce/utilities/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      295 2022-10-24 16:14:29.000000 veevatools-0.0.97/salesforce/utilities/__init__.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      685 2022-10-24 16:14:29.000000 veevatools-0.0.97/salesforce/utilities/async_utils.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     3827 2022-10-24 16:14:29.000000 veevatools-0.0.97/salesforce/utilities/df_utils.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     2055 2023-05-03 02:20:42.000000 veevatools-0.0.97/salesforce/utilities/sf_query_processors.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      757 2023-05-09 05:56:54.290284 veevatools-0.0.97/setup.cfg
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       37 2022-10-24 16:14:29.000000 veevatools-0.0.97/setup.py
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-09 05:56:54.280490 veevatools-0.0.97/veevanetwork/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       40 2022-10-24 16:14:29.000000 veevatools-0.0.97/veevanetwork/__init__.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)        0 2022-10-24 16:14:29.000000 veevatools-0.0.97/veevanetwork/api.py
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-09 05:56:54.282649 veevatools-0.0.97/veevanetwork/custom_exceptions/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      145 2022-10-24 16:14:29.000000 veevatools-0.0.97/veevanetwork/custom_exceptions/__init__.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     3793 2022-10-24 16:14:29.000000 veevatools-0.0.97/veevanetwork/custom_exceptions/veevanetwork_exceptions.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)   122066 2022-10-24 16:14:29.000000 veevatools-0.0.97/veevanetwork/network_api_v25.json
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)    80088 2023-01-30 16:08:51.000000 veevatools-0.0.97/veevanetwork/veevanetwork.py
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-09 05:56:54.286105 veevatools-0.0.97/veevatools.egg-info/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     6385 2023-05-09 05:56:54.000000 veevatools-0.0.97/veevatools.egg-info/PKG-INFO
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      792 2023-05-09 05:56:54.000000 veevatools-0.0.97/veevatools.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)        1 2023-05-09 05:56:54.000000 veevatools-0.0.97/veevatools.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      166 2023-05-09 05:56:54.000000 veevatools-0.0.97/veevatools.egg-info/requires.txt
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       35 2023-05-09 05:56:54.000000 veevatools-0.0.97/veevatools.egg-info/top_level.txt
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-09 05:56:54.287786 veevatools-0.0.97/veevavault/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       36 2022-10-24 16:14:29.000000 veevatools-0.0.97/veevavault/__init__.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     8954 2023-03-06 16:42:47.000000 veevatools-0.0.97/veevavault/veevavault.py
```

### Comparing `veevatools-0.0.96/LICENSE.txt` & `veevatools-0.0.97/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.96/PKG-INFO` & `veevatools-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veevatools
-Version: 0.0.96
+Version: 0.0.97
 Summary: Veeva tools library for accelerating Veeva Systems Internal Tools development
 Home-page: https://github.com/michaelpay
 Author: Michael Pay
 Author-email: monickenish@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `veevatools-0.0.96/README.md` & `veevatools-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.96/salesforce/custom_exceptions/salesforce_exceptions.py` & `veevatools-0.0.97/salesforce/custom_exceptions/salesforce_exceptions.py`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.96/salesforce/salesforce.py` & `veevatools-0.0.97/salesforce/salesforce.py`

 * *Files 1% similar despite different names*

```diff
@@ -934,15 +934,30 @@
                 ps_fls_final = pd.concat([ps_editable, ps_readable])
                 ps_fls_final.columns = ['UserName','Permission Set','Object API Name','Field API Name', 'Permission']
                 
                 return pd.merge(profile_fls_final, ps_fls_final, on=['UserName','Object API Name', 'Field API Name','Permission'], how='outer')
         else:
                 return pd.DataFrame(columns=['UserName', 'Profile', 'Field API Name', 'Object API Name','Permission', 'Permission Set'])
           
-            
+    async def retrieve_user_profile_metadata(self, username: str):
+        profile_metadata = pd.DataFrame(zeep.helpers.serialize_object(self.metadata_list("Profile")))
+        profile_metadata = profile_metadata[['id', 'fullName']].copy()
+        profile_metadata
+        user_profile_id = transform_sf_result_set_rec(self.sf.query_all(f"Select Id, ProfileId FROM User WHERE Username = '{username}'")['records'])
+        if len(profile_metadata[profile_metadata['id'] == user_profile_id['User.ProfileId'].values[0]]['fullName']) == 0:
+            raise Exception("User does not have a retrievable / valid profile")
+        else:
+            user_profile = profile_metadata[profile_metadata['id'] == user_profile_id['User.ProfileId'].values[0]]['fullName'].values[0]
+
+        async_profile_read = async_wrap(self.metadata_read)
+        
+        user_profile_metadata = await async_profile_read('Profile', user_profile)
+
+        return user_profile_metadata
+
     async def retrieve_user_profile_record_type_details(self, username: str, objects: list[str]):
         
         profile_metadata = pd.DataFrame(zeep.helpers.serialize_object(self.metadata_list("Profile")))
         profile_metadata = profile_metadata[['id', 'fullName']].copy()
         profile_metadata
         user_profile_id = transform_sf_result_set_rec(self.sf.query_all(f"Select Id, ProfileId FROM User WHERE Username = '{username}'")['records'])
         if len(profile_metadata[profile_metadata['id'] == user_profile_id['User.ProfileId'].values[0]]['fullName']) == 0:
```

### Comparing `veevatools-0.0.96/salesforce/utilities/async_utils.py` & `veevatools-0.0.97/salesforce/utilities/async_utils.py`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.96/salesforce/utilities/df_utils.py` & `veevatools-0.0.97/salesforce/utilities/df_utils.py`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.96/salesforce/utilities/sf_query_processors.py` & `veevatools-0.0.97/salesforce/utilities/sf_query_processors.py`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.96/setup.cfg` & `veevatools-0.0.97/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = veevatools
-version = 0.0.96
+version = 0.0.97
 description = Veeva tools library for accelerating Veeva Systems Internal Tools development
 author = Michael Pay
 author_email = monickenish@gmail.com
 url = https://github.com/michaelpay
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `veevatools-0.0.96/veevanetwork/custom_exceptions/veevanetwork_exceptions.py` & `veevatools-0.0.97/veevanetwork/custom_exceptions/veevanetwork_exceptions.py`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.96/veevanetwork/network_api_v25.json` & `veevatools-0.0.97/veevanetwork/network_api_v25.json`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.96/veevanetwork/veevanetwork.py` & `veevatools-0.0.97/veevanetwork/veevanetwork.py`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.96/veevatools.egg-info/PKG-INFO` & `veevatools-0.0.97/veevatools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veevatools
-Version: 0.0.96
+Version: 0.0.97
 Summary: Veeva tools library for accelerating Veeva Systems Internal Tools development
 Home-page: https://github.com/michaelpay
 Author: Michael Pay
 Author-email: monickenish@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `veevatools-0.0.96/veevatools.egg-info/SOURCES.txt` & `veevatools-0.0.97/veevatools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.96/veevavault/veevavault.py` & `veevatools-0.0.97/veevavault/veevavault.py`

 * *Files identical despite different names*

