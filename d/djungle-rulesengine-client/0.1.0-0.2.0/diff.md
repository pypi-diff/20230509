# Comparing `tmp/djungle-rulesengine-client-0.1.0.tar.gz` & `tmp/djungle-rulesengine-client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djungle-rulesengine-client-0.1.0.tar", last modified: Tue May  9 08:19:37 2023, max compression
+gzip compressed data, was "djungle-rulesengine-client-0.2.0.tar", last modified: Tue May  9 10:01:50 2023, max compression
```

## Comparing `djungle-rulesengine-client-0.1.0.tar` & `djungle-rulesengine-client-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 08:19:37.484010 djungle-rulesengine-client-0.1.0/
--rw-r--r--   0 fabio      (501) admin       (80)     1071 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.1.0/LICENSE
--rw-r--r--   0 fabio      (501) admin       (80)     1995 2023-05-09 08:19:37.484103 djungle-rulesengine-client-0.1.0/PKG-INFO
--rw-r--r--   0 fabio      (501) admin       (80)      350 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.1.0/README.md
--rw-r--r--   0 fabio      (501) admin       (80)      259 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.1.0/pyproject.toml
--rw-r--r--   0 fabio      (501) admin       (80)      746 2023-05-09 08:19:37.484581 djungle-rulesengine-client-0.1.0/setup.cfg
--rw-r--r--   0 fabio      (501) admin       (80)       38 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.1.0/setup.py
-drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 08:19:37.479655 djungle-rulesengine-client-0.1.0/src/
-drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 08:19:37.482931 djungle-rulesengine-client-0.1.0/src/djungle_rulesengine_client.egg-info/
--rw-r--r--   0 fabio      (501) admin       (80)     1995 2023-05-09 08:19:37.000000 djungle-rulesengine-client-0.1.0/src/djungle_rulesengine_client.egg-info/PKG-INFO
--rw-r--r--   0 fabio      (501) admin       (80)      448 2023-05-09 08:19:37.000000 djungle-rulesengine-client-0.1.0/src/djungle_rulesengine_client.egg-info/SOURCES.txt
--rw-r--r--   0 fabio      (501) admin       (80)        1 2023-05-09 08:19:37.000000 djungle-rulesengine-client-0.1.0/src/djungle_rulesengine_client.egg-info/dependency_links.txt
--rw-r--r--   0 fabio      (501) admin       (80)        1 2023-05-09 08:19:37.000000 djungle-rulesengine-client-0.1.0/src/djungle_rulesengine_client.egg-info/not-zip-safe
--rw-r--r--   0 fabio      (501) admin       (80)       17 2023-05-09 08:19:37.000000 djungle-rulesengine-client-0.1.0/src/djungle_rulesengine_client.egg-info/requires.txt
--rw-r--r--   0 fabio      (501) admin       (80)       12 2023-05-09 08:19:37.000000 djungle-rulesengine-client-0.1.0/src/djungle_rulesengine_client.egg-info/top_level.txt
-drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 08:19:37.483475 djungle-rulesengine-client-0.1.0/src/rulesengine/
--rw-r--r--   0 fabio      (501) admin       (80)        0 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.1.0/src/rulesengine/__init__.py
--rw-r--r--   0 fabio      (501) admin       (80)      746 2023-05-09 08:06:30.000000 djungle-rulesengine-client-0.1.0/src/rulesengine/client.py
-drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 08:19:37.483796 djungle-rulesengine-client-0.1.0/tests/
--rw-r--r--   0 fabio      (501) admin       (80)     1445 2023-05-09 08:06:30.000000 djungle-rulesengine-client-0.1.0/tests/test_client.py
+drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 10:01:50.416883 djungle-rulesengine-client-0.2.0/
+-rw-r--r--   0 fabio      (501) admin       (80)     1071 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.2.0/LICENSE
+-rw-r--r--   0 fabio      (501) admin       (80)     1995 2023-05-09 10:01:50.417055 djungle-rulesengine-client-0.2.0/PKG-INFO
+-rw-r--r--   0 fabio      (501) admin       (80)      350 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.2.0/README.md
+-rw-r--r--   0 fabio      (501) admin       (80)      259 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.2.0/pyproject.toml
+-rw-r--r--   0 fabio      (501) admin       (80)      746 2023-05-09 10:01:50.417832 djungle-rulesengine-client-0.2.0/setup.cfg
+-rw-r--r--   0 fabio      (501) admin       (80)       38 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.2.0/setup.py
+drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 10:01:50.412107 djungle-rulesengine-client-0.2.0/src/
+drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 10:01:50.415189 djungle-rulesengine-client-0.2.0/src/djungle_rulesengine_client.egg-info/
+-rw-r--r--   0 fabio      (501) admin       (80)     1995 2023-05-09 10:01:50.000000 djungle-rulesengine-client-0.2.0/src/djungle_rulesengine_client.egg-info/PKG-INFO
+-rw-r--r--   0 fabio      (501) admin       (80)      448 2023-05-09 10:01:50.000000 djungle-rulesengine-client-0.2.0/src/djungle_rulesengine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 fabio      (501) admin       (80)        1 2023-05-09 10:01:50.000000 djungle-rulesengine-client-0.2.0/src/djungle_rulesengine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 fabio      (501) admin       (80)        1 2023-05-09 10:01:50.000000 djungle-rulesengine-client-0.2.0/src/djungle_rulesengine_client.egg-info/not-zip-safe
+-rw-r--r--   0 fabio      (501) admin       (80)       17 2023-05-09 10:01:50.000000 djungle-rulesengine-client-0.2.0/src/djungle_rulesengine_client.egg-info/requires.txt
+-rw-r--r--   0 fabio      (501) admin       (80)       12 2023-05-09 10:01:50.000000 djungle-rulesengine-client-0.2.0/src/djungle_rulesengine_client.egg-info/top_level.txt
+drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 10:01:50.415857 djungle-rulesengine-client-0.2.0/src/rulesengine/
+-rw-r--r--   0 fabio      (501) admin       (80)        0 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.2.0/src/rulesengine/__init__.py
+-rw-r--r--   0 fabio      (501) admin       (80)     1175 2023-05-09 09:46:04.000000 djungle-rulesengine-client-0.2.0/src/rulesengine/client.py
+drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 10:01:50.416419 djungle-rulesengine-client-0.2.0/tests/
+-rw-r--r--   0 fabio      (501) admin       (80)     2662 2023-05-09 09:49:36.000000 djungle-rulesengine-client-0.2.0/tests/test_client.py
```

### Comparing `djungle-rulesengine-client-0.1.0/LICENSE` & `djungle-rulesengine-client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djungle-rulesengine-client-0.1.0/PKG-INFO` & `djungle-rulesengine-client-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djungle-rulesengine-client
-Version: 0.1.0
+Version: 0.2.0
 Summary: A client to Djungle Studio rulesengine API
 Home-page: https://github.com/djungle-io/djungle-rulesengine-client
 Author: Djungle s.r.l.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `djungle-rulesengine-client-0.1.0/setup.cfg` & `djungle-rulesengine-client-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djungle-rulesengine-client
-version = 0.1.0
+version = 0.2.0
 description = A client to Djungle Studio rulesengine API
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
 author = Djungle s.r.l.
 url = https://github.com/djungle-io/djungle-rulesengine-client
```

### Comparing `djungle-rulesengine-client-0.1.0/src/djungle_rulesengine_client.egg-info/PKG-INFO` & `djungle-rulesengine-client-0.2.0/src/djungle_rulesengine_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djungle-rulesengine-client
-Version: 0.1.0
+Version: 0.2.0
 Summary: A client to Djungle Studio rulesengine API
 Home-page: https://github.com/djungle-io/djungle-rulesengine-client
 Author: Djungle s.r.l.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `djungle-rulesengine-client-0.1.0/tests/test_client.py` & `djungle-rulesengine-client-0.2.0/tests/test_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,7 +32,38 @@
             engine.push_action("sys-1", "my-action", {"key": "value"})
 
         self.assertEqual(cm.exception.__cause__.response.json(), {"error": "ko"})
 
         request = engine_api_mock.last_request
         self.assertEqual(request.headers["X-Auth-Token"], "abcde")
         self.assertEqual(request.json(), {"payload": {"key": "value"}})
+
+    @requests_mock.Mocker()
+    def test_get_pluggable_props_success(self, engine_api_mock):
+        engine = EngineClient(base_url="https://example.com", token="abcde")
+        engine_api_mock.get(
+            "https://example.com/api/v1/subjects/sys-1/props/?p=my-prop", json={"status": "ok"}
+        )
+
+        ret = engine.get_pluggable_props("sys-1", "my-prop")
+
+        self.assertEqual(ret, {"status": "ok"})
+
+        request = engine_api_mock.last_request
+        self.assertEqual(request.headers["X-Auth-Token"], "abcde")
+
+    @requests_mock.Mocker()
+    def test_get_pluggable_props_failure(self, engine_api_mock):
+        engine = EngineClient(base_url="https://example.com", token="abcde")
+        engine_api_mock.get(
+            "https://example.com/api/v1/subjects/sys-1/props/?p=my-prop&key=value",
+            json={"error": "ko"},
+            status_code=400,
+        )
+
+        with self.assertRaises(EngineClientError) as cm:
+            engine.get_pluggable_props("sys-1", "my-prop", key="value")
+
+        self.assertEqual(cm.exception.__cause__.response.json(), {"error": "ko"})
+
+        request = engine_api_mock.last_request
+        self.assertEqual(request.headers["X-Auth-Token"], "abcde")
```

