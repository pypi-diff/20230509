# Comparing `tmp/getsmarter-api-clients-0.5.3.tar.gz` & `tmp/getsmarter-api-clients-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getsmarter-api-clients-0.5.3.tar", last modified: Mon May  8 18:23:24 2023, max compression
+gzip compressed data, was "getsmarter-api-clients-0.5.4.tar", last modified: Tue May  9 15:19:44 2023, max compression
```

## Comparing `getsmarter-api-clients-0.5.3.tar` & `getsmarter-api-clients-0.5.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:23:24.774820 getsmarter-api-clients-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-05-08 18:23:19.000000 getsmarter-api-clients-0.5.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-08 18:23:19.000000 getsmarter-api-clients-0.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-08 18:23:19.000000 getsmarter-api-clients-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6231 2023-05-08 18:23:24.774820 getsmarter-api-clients-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-05-08 18:23:19.000000 getsmarter-api-clients-0.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:23:24.774820 getsmarter-api-clients-0.5.3/getsmarter_api_clients/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-08 18:23:19.000000 getsmarter-api-clients-0.5.3/getsmarter_api_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9674 2023-05-08 18:23:19.000000 getsmarter-api-clients-0.5.3/getsmarter_api_clients/geag.py
--rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-05-08 18:23:19.000000 getsmarter-api-clients-0.5.3/getsmarter_api_clients/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:23:24.774820 getsmarter-api-clients-0.5.3/getsmarter_api_clients.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6231 2023-05-08 18:23:24.000000 getsmarter-api-clients-0.5.3/getsmarter_api_clients.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-05-08 18:23:24.000000 getsmarter-api-clients-0.5.3/getsmarter_api_clients.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 18:23:24.000000 getsmarter-api-clients-0.5.3/getsmarter_api_clients.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 18:23:24.000000 getsmarter-api-clients-0.5.3/getsmarter_api_clients.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-08 18:23:24.000000 getsmarter-api-clients-0.5.3/getsmarter_api_clients.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-08 18:23:24.000000 getsmarter-api-clients-0.5.3/getsmarter_api_clients.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:23:24.774820 getsmarter-api-clients-0.5.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-08 18:23:19.000000 getsmarter-api-clients-0.5.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-08 18:23:19.000000 getsmarter-api-clients-0.5.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-08 18:23:24.774820 getsmarter-api-clients-0.5.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     4952 2023-05-08 18:23:19.000000 getsmarter-api-clients-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:19:44.621421 getsmarter-api-clients-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6307 2023-05-09 15:19:44.621421 getsmarter-api-clients-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:19:44.621421 getsmarter-api-clients-0.5.4/getsmarter_api_clients/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9862 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients/geag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:19:44.621421 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6307 2023-05-09 15:19:44.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-05-09 15:19:44.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 15:19:44.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 15:19:44.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-09 15:19:44.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-09 15:19:44.000000 getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 15:19:44.621421 getsmarter-api-clients-0.5.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-09 15:19:44.625422 getsmarter-api-clients-0.5.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4952 2023-05-09 15:19:40.000000 getsmarter-api-clients-0.5.4/setup.py
```

### Comparing `getsmarter-api-clients-0.5.3/CHANGELOG.rst` & `getsmarter-api-clients-0.5.4/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 *
 
+[0.5.4]
+~~~~~~~
+* Add `org_id`` as an optional enterprise allocation param
+
 [0.5.3]
 ~~~~~~~
 * Return allocation response objects
 
 [0.5.2]
 ~~~~~~~
 * Include payload in error message
```

### Comparing `getsmarter-api-clients-0.5.3/LICENSE.txt` & `getsmarter-api-clients-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.5.3/PKG-INFO` & `getsmarter-api-clients-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getsmarter-api-clients
-Version: 0.5.3
+Version: 0.5.4
 Summary: Clients to interact with GetSmarter APIs.
 Home-page: https://github.com/edx/getsmarter-api-clients
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -169,14 +169,18 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 *
 
+[0.5.4]
+~~~~~~~
+* Add `org_id`` as an optional enterprise allocation param
+
 [0.5.3]
 ~~~~~~~
 * Return allocation response objects
 
 [0.5.2]
 ~~~~~~~
 * Include payload in error message
```

### Comparing `getsmarter-api-clients-0.5.3/README.rst` & `getsmarter-api-clients-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.5.3/getsmarter_api_clients/geag.py` & `getsmarter-api-clients-0.5.4/getsmarter_api_clients/geag.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,15 +167,16 @@
         postal_code=None,
         state=None,
         state_code=None,
         country=None,
         country_code=None,
         mobile_phone=None,
         work_experience=None,
-        education_highest_level=None
+        education_highest_level=None,
+        org_id=None
     ):
         """
         Create an enterprise_allocation (enrollment) through GEAG.
 
         :Parameters:
           - `payment_reference (str)`: Reference used by enterprise partner
             when payment is made to GetSmarter
@@ -202,14 +203,16 @@
           - `mobile_phone (str)`: Mobile phone number
           - `work_experience (str)`: One of ['None', '1 to 5 years',
             '5 to 15 years', 'More than 15 years']
           - `education_highest_level (str)`: One of ['High school',
             'Bachelor’s degree', 'Master’s degree', 'Doctoral degree',
             'Other tertiary qualification', 'Honours degree',
             'Bachelors degree']
+          - `org_id (str)`: `auth_org_id` from the learner’s
+            `EnterpriseCustomer` record
 
         **Example payload**
           { "paymentReference": "GS-12304",
             "enterpriseCustomerUuid": "69C3E666-4740-4531-9435-A3EDF6D28C01",
             "firstName": "Jan",
             "lastName": "Pan",
             "email": "janpan@gs.com",
@@ -218,15 +221,16 @@
             "currency": "ZAR",
             "orderItems": [{ "productId": "product_id", "quantity": 1,
             "normalPrice": 1000, "discount": 500, "finalPrice": 500 }],
             "addressLine1": "Oak Glen",
             "city": "Cape Town",
             "postalCode": "7570",
             "country": "South Africa",
-            "countryCode": "ZA" }
+            "countryCode": "ZA",
+            "orgId": "12KJ2j9js0" }
 
         """
         url = f'{self.api_url}/enterprise_allocations'
 
         payload = {
             'paymentReference': payment_reference,
             'enterpriseCustomerUuid': enterprise_customer_uuid,
@@ -246,14 +250,15 @@
             'state': state,
             'stateCode': state_code,
             'country': country,
             'countryCode': country_code,
             'mobilePhone': mobile_phone,
             'workExperience': work_experience,
             'educationHighestLevel': education_highest_level,
+            'orgId': org_id,
         }
         # remove keys with empty values
         payload = {k: v for k, v in payload.items() if v is not None}
 
         response = self.post(url, json=payload)
         try:
             response.raise_for_status()
```

### Comparing `getsmarter-api-clients-0.5.3/getsmarter_api_clients/oauth.py` & `getsmarter-api-clients-0.5.4/getsmarter_api_clients/oauth.py`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.5.3/getsmarter_api_clients.egg-info/PKG-INFO` & `getsmarter-api-clients-0.5.4/getsmarter_api_clients.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getsmarter-api-clients
-Version: 0.5.3
+Version: 0.5.4
 Summary: Clients to interact with GetSmarter APIs.
 Home-page: https://github.com/edx/getsmarter-api-clients
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -169,14 +169,18 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 *
 
+[0.5.4]
+~~~~~~~
+* Add `org_id`` as an optional enterprise allocation param
+
 [0.5.3]
 ~~~~~~~
 * Return allocation response objects
 
 [0.5.2]
 ~~~~~~~
 * Include payload in error message
```

### Comparing `getsmarter-api-clients-0.5.3/requirements/constraints.txt` & `getsmarter-api-clients-0.5.4/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.5.3/setup.py` & `getsmarter-api-clients-0.5.4/setup.py`

 * *Files identical despite different names*

