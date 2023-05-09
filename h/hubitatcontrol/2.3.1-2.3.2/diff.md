# Comparing `tmp/hubitatcontrol-2.3.1.tar.gz` & `tmp/hubitatcontrol-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubitatcontrol-2.3.1.tar", max compression
+gzip compressed data, was "hubitatcontrol-2.3.2.tar", max compression
```

## Comparing `hubitatcontrol-2.3.1.tar` & `hubitatcontrol-2.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-2.3.1/LICENSE
--rw-r--r--   0        0        0     6311 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.1/README.md
--rw-r--r--   0        0        0     3072 2023-05-09 03:28:26.350568 hubitatcontrol-2.3.1/hubitatcontrol/__init__.py
--rw-r--r--   0        0        0     3824 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.1/hubitatcontrol/__main__.py
--rw-r--r--   0        0        0      172 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.1/hubitatcontrol/environment.py
--rw-r--r--   0        0        0     1060 2023-04-23 03:06:31.104361 hubitatcontrol-2.3.1/hubitatcontrol/generic.py
--rw-r--r--   0        0        0     2984 2023-05-09 04:21:13.229519 hubitatcontrol-2.3.1/hubitatcontrol/hub.py
--rw-r--r--   0        0        0     2774 2023-04-23 03:06:31.104361 hubitatcontrol-2.3.1/hubitatcontrol/lights.py
--rw-r--r--   0        0        0      478 2023-05-09 03:28:26.350568 hubitatcontrol-2.3.1/hubitatcontrol/sensors.py
--rw-r--r--   0        0        0     2606 2023-05-09 04:24:20.755612 hubitatcontrol-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     7193 1970-01-01 00:00:00.000000 hubitatcontrol-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-2.3.2/LICENSE
+-rw-r--r--   0        0        0     6311 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.2/README.md
+-rw-r--r--   0        0        0     3072 2023-05-09 03:28:26.350568 hubitatcontrol-2.3.2/hubitatcontrol/__init__.py
+-rw-r--r--   0        0        0     3824 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.2/hubitatcontrol/__main__.py
+-rw-r--r--   0        0        0      172 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.2/hubitatcontrol/environment.py
+-rw-r--r--   0        0        0     1060 2023-04-23 03:06:31.104361 hubitatcontrol-2.3.2/hubitatcontrol/generic.py
+-rw-r--r--   0        0        0     3073 2023-05-09 06:17:49.007286 hubitatcontrol-2.3.2/hubitatcontrol/hub.py
+-rw-r--r--   0        0        0     2774 2023-04-23 03:06:31.104361 hubitatcontrol-2.3.2/hubitatcontrol/lights.py
+-rw-r--r--   0        0        0      478 2023-05-09 03:28:26.350568 hubitatcontrol-2.3.2/hubitatcontrol/sensors.py
+-rw-r--r--   0        0        0     2606 2023-05-09 06:21:55.280233 hubitatcontrol-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7193 1970-01-01 00:00:00.000000 hubitatcontrol-2.3.2/PKG-INFO
```

### Comparing `hubitatcontrol-2.3.1/LICENSE` & `hubitatcontrol-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.3.1/README.md` & `hubitatcontrol-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.3.1/hubitatcontrol/__init__.py` & `hubitatcontrol-2.3.2/hubitatcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.3.1/hubitatcontrol/__main__.py` & `hubitatcontrol-2.3.2/hubitatcontrol/__main__.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.3.1/hubitatcontrol/generic.py` & `hubitatcontrol-2.3.2/hubitatcontrol/generic.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.3.1/hubitatcontrol/hub.py` & `hubitatcontrol-2.3.2/hubitatcontrol/hub.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,16 +15,17 @@
             self.base_url_prefix = self.host + "/api/" + self.cloud_token + "/apps/" + self.app_id + "/devices"
         else:
             self.base_url_prefix = self.host + "/apps/api/" + self.app_id + "/devices"
 
     @property
     def devices(self) -> list:
         r = requests.get(url=self.base_url_prefix + "/all", params={"access_token": self.token}, timeout=timeout)
-        if r.status_code == 403:
-            raise Exception("Check credentials")
+        err = [401, 403, 404, 405]
+        if r.status_code in err:
+            raise Exception(f"Check credentials - Status code: {r.status_code}, Invalid codes: {err}")
         return r.json()
 
     def get_device(self, name: str):
         for i in self.devices:
             if i["label"] == name:
                 return i
```

### Comparing `hubitatcontrol-2.3.1/hubitatcontrol/lights.py` & `hubitatcontrol-2.3.2/hubitatcontrol/lights.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.3.1/pyproject.toml` & `hubitatcontrol-2.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hubitatcontrol"
-version = "v2.3.1"
+version = "v2.3.2"
 description = "Hubitat Maker API Interface"
 authors = ["Jesse Schoepfer <jelloeater@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/Jelloeater/hubitatcontrol"
 keywords = ["hubitat", "makerapi","requests"]
 classifiers = ["Development Status :: 5 - Production/Stable",
```

### Comparing `hubitatcontrol-2.3.1/PKG-INFO` & `hubitatcontrol-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubitatcontrol
-Version: 2.3.1
+Version: 2.3.2
 Summary: Hubitat Maker API Interface
 Home-page: https://github.com/Jelloeater/hubitatcontrol
 License: MIT
 Keywords: hubitat,makerapi,requests
 Author: Jesse Schoepfer
 Author-email: jelloeater@gmail.com
 Requires-Python: >=3.10,<4.0
```

