# Comparing `tmp/sortinghat_openinfra-0.1.2.tar.gz` & `tmp/sortinghat_openinfra-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortinghat_openinfra-0.1.2.tar", max compression
+gzip compressed data, was "sortinghat_openinfra-0.1.3.tar", max compression
```

## Comparing `sortinghat_openinfra-0.1.2.tar` & `sortinghat_openinfra-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-05-02 22:36:20.344076 sortinghat_openinfra-0.1.2/LICENSE
--rw-r--r--   0        0        0     2244 2023-05-02 22:36:20.344076 sortinghat_openinfra-0.1.2/README.md
--rw-r--r--   0        0        0     1268 2023-05-02 22:36:20.344076 sortinghat_openinfra-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       86 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/sortinghat/core/importer/backends/_version.py
--rw-r--r--   0        0        0     7864 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/sortinghat/core/importer/backends/openinfra.py
--rw-r--r--   0        0        0        0 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     6403 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/tests/data/openinfra_page_1.json
--rw-r--r--   0        0        0     5073 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/tests/data/openinfra_page_2.json
--rw-r--r--   0        0        0     2595 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/tests/data/openinfra_private.json
--rw-r--r--   0        0        0    17771 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/tests/test_openinfra.py
--rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 sortinghat_openinfra-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-09 09:43:46.346635 sortinghat_openinfra-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2244 2023-05-09 09:43:46.346635 sortinghat_openinfra-0.1.3/README.md
+-rw-r--r--   0        0        0     1268 2023-05-09 09:43:46.346635 sortinghat_openinfra-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/sortinghat/core/importer/backends/_version.py
+-rw-r--r--   0        0        0     7865 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/sortinghat/core/importer/backends/openinfra.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     6403 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/tests/data/openinfra_page_1.json
+-rw-r--r--   0        0        0     5073 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/tests/data/openinfra_page_2.json
+-rw-r--r--   0        0        0     2595 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/tests/data/openinfra_private.json
+-rw-r--r--   0        0        0    17770 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/tests/test_openinfra.py
+-rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 sortinghat_openinfra-0.1.3/PKG-INFO
```

### Comparing `sortinghat_openinfra-0.1.2/LICENSE` & `sortinghat_openinfra-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.2/README.md` & `sortinghat_openinfra-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.2/pyproject.toml` & `sortinghat_openinfra-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortinghat-openinfra"
-version = "0.1.2"
+version = "0.1.3"
 description = "SortingHat backend to import identities from OpenInfraID"
 authors = [
     "Bitergia Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `sortinghat_openinfra-0.1.2/sortinghat/core/importer/backends/openinfra.py` & `sortinghat_openinfra-0.1.3/sortinghat/core/importer/backends/openinfra.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     # API path
     MEMBERS_PUBLIC = '/api/public/v1/members'
     MEMBERS_PRIVATE = '/api/v1/members'
 
     # Resource parameters
     PPER_PAGE = 'per_page'
     PPAGE = 'page'
-    PSORT = 'sort'
+    PSORT = 'order'
     PFILTER = 'filter'
     PTOKEN = 'access_token'
 
     def __init__(self, url):
         self.url = url
         self.source = 'openinfra'
         self.client_id = getattr(settings, 'OPENINFRA_CLIENT_ID', None)
@@ -153,15 +153,15 @@
 
         :param from_date: obtain members updated since this date
 
         :returns: a generator of members
         """
         payload = {
             self.PPER_PAGE: 100,
-            self.PSORT: '-last_edited',
+            self.PSORT: 'last_edited',
             self.PPAGE: 1,
         }
 
         if from_date:
             payload[self.PFILTER] = 'last_edited>' + str(int(from_date.timestamp()))
 
         if self.private_api:
@@ -198,15 +198,15 @@
 
             data = r.json()
             yield data
 
             if page >= data['last_page']:
                 break
             page += 1
-            payload['page'] = page
+            payload[self.PPAGE] = page
 
     def _create_access_token(self):
         """Create OpenInfra access token."""
 
         params = {
             'grant_type': 'client_credentials',
             'scope': 'https://openstackid-resources.openstack.org/members/read'
@@ -215,9 +215,9 @@
             'client_id': self.client_id,
             'client_secret': self.client_secret
         }
 
         r = requests.post(url=self.OPENINFRA_TOKEN_URL, data=data, params=params)
         if not r.ok:
             raise LoadError(cause="OpenInfra token can't be created.")
-        access_token = r.json()['access_token']
+        access_token = r.json()[self.PTOKEN]
         return access_token
```

### Comparing `sortinghat_openinfra-0.1.2/tests/data/openinfra_page_1.json` & `sortinghat_openinfra-0.1.3/tests/data/openinfra_page_1.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.2/tests/data/openinfra_page_2.json` & `sortinghat_openinfra-0.1.3/tests/data/openinfra_page_2.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.2/tests/data/openinfra_private.json` & `sortinghat_openinfra-0.1.3/tests/data/openinfra_private.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.2/tests/test_openinfra.py` & `sortinghat_openinfra-0.1.3/tests/test_openinfra.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,27 +161,27 @@
     def test_fetch_items_with_payload(self):
         """Test whether fetch items from date returns paginated items"""
 
         # Set up a mock HTTP server
         requests, bodies = setup_mock_server(public=True)
 
         # Run fetch items
-        payload = {OpenInfraIDParser.PSORT: '-last_edited'}
+        payload = {OpenInfraIDParser.PSORT: 'last_edited'}
         parser = OpenInfraIDParser(OPENINFRA_URL)
         raw_items = parser.fetch_items(OPENINFRA_PUBLIC_MEMBERS_URL, payload=payload)
 
         items = [item for item in raw_items]
         self.assertEqual(len(items), 2)
         self.assertDictEqual(items[0], json.loads(bodies[0]))
         self.assertDictEqual(items[1], json.loads(bodies[1]))
 
         # Check requests
         expected_qs = [
-            {'sort': ['-last_edited']},
-            {'sort': ['-last_edited'], 'page': ['2']}
+            {'order': ['last_edited']},
+            {'order': ['last_edited'], 'page': ['2']}
         ]
         self.assertEqual(len(requests), 2)
         for i, req in enumerate(requests):
             self.assertDictEqual(req.querystring, expected_qs[i])
             self.assertEqual(req.url.split('?')[0], OPENINFRA_PUBLIC_MEMBERS_URL)
 
     @httpretty.activate
@@ -195,16 +195,16 @@
         parser = OpenInfraIDParser(OPENINFRA_URL)
         members = [member for member in parser.fetch_members()]
 
         self.assertEqual(len(members), 15)
 
         # Check requests
         expected_qs = [
-            {'page': ['1'], 'per_page': ['100'], 'sort': ['-last_edited']},
-            {'page': ['2'], 'per_page': ['100'], 'sort': ['-last_edited']}
+            {'page': ['1'], 'per_page': ['100'], 'order': ['last_edited']},
+            {'page': ['2'], 'per_page': ['100'], 'order': ['last_edited']}
         ]
         self.assertEqual(len(requests), 2)
         for i, req in enumerate(requests):
             self.assertDictEqual(req.querystring, expected_qs[i])
             self.assertEqual(req.url.split('?')[0], OPENINFRA_PUBLIC_MEMBERS_URL)
 
     @httpretty.activate
@@ -226,15 +226,15 @@
         parser = OpenInfraIDParser(OPENINFRA_URL)
         members = [member for member in parser.fetch_members()]
 
         self.assertEqual(len(members), 3)
 
         # Check requests
         expected_qs = [
-            {'page': ['1'], 'per_page': ['100'], 'sort': ['-last_edited'], 'access_token': ['test_token']}
+            {'page': ['1'], 'per_page': ['100'], 'order': ['last_edited'], 'access_token': ['test_token']}
         ]
         self.assertEqual(len(requests), 1)
         for i, req in enumerate(requests):
             self.assertDictEqual(req.querystring, expected_qs[i])
             self.assertEqual(req.url.split('?')[0], OPENINFRA_PRIVATE_MEMBERS_URL)
 
     @httpretty.activate
@@ -252,21 +252,21 @@
         self.assertEqual(len(members), 15)
 
         # Check requests
         expected_qs = [
             {
                 'page': ['1'],
                 'per_page': ['100'],
-                'sort': ['-last_edited'],
+                'order': ['last_edited'],
                 'filter': ['last_edited>946684800']
             },
             {
                 'page': ['2'],
                 'per_page': ['100'],
-                'sort': ['-last_edited'],
+                'order': ['last_edited'],
                 'filter': ['last_edited>946684800']
             }
         ]
         self.assertEqual(len(requests), 2)
         for i, req in enumerate(requests):
             self.assertDictEqual(req.querystring, expected_qs[i])
             self.assertEqual(req.url.split('?')[0], OPENINFRA_PUBLIC_MEMBERS_URL)
@@ -349,20 +349,20 @@
         self.assertEqual(indiv.enrollments[0].organization.name, "Technology Org")
 
         # Check requests
         expected_qs = [
             {
                 'page': ['1'],
                 'per_page': ['100'],
-                'sort': ['-last_edited']
+                'order': ['last_edited']
             },
             {
                 'page': ['2'],
                 'per_page': ['100'],
-                'sort': ['-last_edited']
+                'order': ['last_edited']
             }
         ]
         self.assertEqual(len(requests), 2)
         for i, req in enumerate(requests):
             self.assertDictEqual(req.querystring, expected_qs[i])
             self.assertEqual(req.url.split('?')[0], OPENINFRA_PUBLIC_MEMBERS_URL)
 
@@ -431,15 +431,15 @@
         self.assertEqual(indiv.enrollments[0].organization.name, "Technology Org")
 
         # Check requests
         expected_qs = [
             {
                 'page': ['1'],
                 'per_page': ['100'],
-                'sort': ['-last_edited'],
+                'order': ['last_edited'],
                 'access_token': ['test_token']
             }
         ]
         self.assertEqual(len(requests), 1)
         for i, req in enumerate(requests):
             self.assertDictEqual(req.querystring, expected_qs[i])
             self.assertEqual(req.url.split('?')[0], OPENINFRA_PRIVATE_MEMBERS_URL)
```

### Comparing `sortinghat_openinfra-0.1.2/PKG-INFO` & `sortinghat_openinfra-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortinghat-openinfra
-Version: 0.1.2
+Version: 0.1.3
 Summary: SortingHat backend to import identities from OpenInfraID
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab,sortinghat
 Author: Bitergia Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

