# Comparing `tmp/OpenAccess-0.2.tar.gz` & `tmp/OpenAccess-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenAccess-0.2.tar", last modified: Tue May  9 14:46:35 2023, max compression
+gzip compressed data, was "OpenAccess-0.3.tar", last modified: Tue May  9 21:09:42 2023, max compression
```

## Comparing `OpenAccess-0.2.tar` & `OpenAccess-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 14:46:35.746033 OpenAccess-0.2/
-drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 14:46:35.746033 OpenAccess-0.2/OpenAccess/
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)      103 2023-05-09 14:46:13.000000 OpenAccess-0.2/OpenAccess/__init__.py
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)    12379 2023-05-09 14:46:08.000000 OpenAccess-0.2/OpenAccess/openaccess.py
-drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 14:46:35.746033 OpenAccess-0.2/OpenAccess.egg-info/
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1579 2023-05-09 14:46:35.000000 OpenAccess-0.2/OpenAccess.egg-info/PKG-INFO
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)      235 2023-05-09 14:46:35.000000 OpenAccess-0.2/OpenAccess.egg-info/SOURCES.txt
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)        1 2023-05-09 14:46:35.000000 OpenAccess-0.2/OpenAccess.egg-info/dependency_links.txt
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)        9 2023-05-09 14:46:35.000000 OpenAccess-0.2/OpenAccess.egg-info/requires.txt
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)       11 2023-05-09 14:46:35.000000 OpenAccess-0.2/OpenAccess.egg-info/top_level.txt
--rw-rw-r--   0 jaiber    (1000) jaiber    (1000)     1579 2023-05-09 14:46:35.746033 OpenAccess-0.2/PKG-INFO
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1249 2023-04-24 21:19:05.000000 OpenAccess-0.2/README.md
--rw-rw-r--   0 jaiber    (1000) jaiber    (1000)       38 2023-05-09 14:46:35.746033 OpenAccess-0.2/setup.cfg
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1392 2023-04-03 16:58:33.000000 OpenAccess-0.2/setup.py
+drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 21:09:42.436089 OpenAccess-0.3/
+drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 21:09:42.436089 OpenAccess-0.3/OpenAccess/
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)      103 2023-05-09 21:09:30.000000 OpenAccess-0.3/OpenAccess/__init__.py
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)    13803 2023-05-09 21:09:06.000000 OpenAccess-0.3/OpenAccess/openaccess.py
+drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 21:09:42.436089 OpenAccess-0.3/OpenAccess.egg-info/
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1579 2023-05-09 21:09:42.000000 OpenAccess-0.3/OpenAccess.egg-info/PKG-INFO
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)      235 2023-05-09 21:09:42.000000 OpenAccess-0.3/OpenAccess.egg-info/SOURCES.txt
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)        1 2023-05-09 21:09:42.000000 OpenAccess-0.3/OpenAccess.egg-info/dependency_links.txt
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)        9 2023-05-09 21:09:42.000000 OpenAccess-0.3/OpenAccess.egg-info/requires.txt
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)       11 2023-05-09 21:09:42.000000 OpenAccess-0.3/OpenAccess.egg-info/top_level.txt
+-rw-rw-r--   0 jaiber    (1000) jaiber    (1000)     1579 2023-05-09 21:09:42.436089 OpenAccess-0.3/PKG-INFO
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1249 2023-04-24 21:19:05.000000 OpenAccess-0.3/README.md
+-rw-rw-r--   0 jaiber    (1000) jaiber    (1000)       38 2023-05-09 21:09:42.436089 OpenAccess-0.3/setup.cfg
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1392 2023-04-03 16:58:33.000000 OpenAccess-0.3/setup.py
```

### Comparing `OpenAccess-0.2/OpenAccess/openaccess.py` & `OpenAccess-0.3/OpenAccess/openaccess.py`

 * *Files 4% similar despite different names*

```diff
@@ -301,8 +301,39 @@
 
         # If a response is recieved, parse it into a dict so its properties can be retrieved easily
         if response.status_code == 200:
             return self.SUCCESS
 
         # If an error occurred on the server side, return its information
         else:
+            return f"A server error occurred during your request. If the status code is available, it is shown below\n{response.status_code}: {response.text}"
+        
+
+
+    def badge_last_location(self, instances_filter=''):
+        """
+        Get de last location using a filter instances_filter(str)
+        i.e. badge_last_location(instalces_filter="BadgeID=1234 AND AccessFlag=1 AND PanelID=10 AND ReaderID=2")
+        i.e. badge_last_location(instalces_filter="AccessFlag=1 AND PanelID=10 AND ReaderID=2 AND EventTime>\"2023-05-09T15:35:00\"")
+
+        GET /api/access/onguard/openaccess/instances
+
+        Get a supported data class against a specific instance of a particular type (Lnl_BadgeLastLocation against a reader and a badgeId in this case)
+        """
+
+        # Data object to be serialized by PostAsJsonAsync
+        em = {
+            "type_name":"Lnl_BadgeLastLocation", 
+            "filter":instances_filter
+        }
+
+        
+        self.client.headers.update({"Session-Token": self.session_token})
+        response = self.client.get(self.build_uri_with_version("instances","1.0"), json=em, verify=self.client.verify)
+
+        # If a response is recieved, parse it into a dict so its properties can be retrieved easily
+        if response.status_code == 200:
+            return self.parse_response(response)
+
+        # If an error occurred on the server side, return its information
+        else:
             return f"A server error occurred during your request. If the status code is available, it is shown below\n{response.status_code}: {response.text}"
```

### Comparing `OpenAccess-0.2/OpenAccess.egg-info/PKG-INFO` & `OpenAccess-0.3/OpenAccess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAccess
-Version: 0.2
+Version: 0.3
 Summary: Librería no oficial para leer comunicarse con un servidor de LENEL OpenAccess 
 Home-page: https://github.com/alejomejia1
 Author: Alejandro Mejia Ayala, Jaiber Camacho
 Author-email: alejandromejia@qaingenieros.com
 License: GNU
 Description-Content-Type: text/markdown
```

### Comparing `OpenAccess-0.2/PKG-INFO` & `OpenAccess-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAccess
-Version: 0.2
+Version: 0.3
 Summary: Librería no oficial para leer comunicarse con un servidor de LENEL OpenAccess 
 Home-page: https://github.com/alejomejia1
 Author: Alejandro Mejia Ayala, Jaiber Camacho
 Author-email: alejandromejia@qaingenieros.com
 License: GNU
 Description-Content-Type: text/markdown
```

### Comparing `OpenAccess-0.2/README.md` & `OpenAccess-0.3/README.md`

 * *Files identical despite different names*

### Comparing `OpenAccess-0.2/setup.py` & `OpenAccess-0.3/setup.py`

 * *Files identical despite different names*

