# Comparing `tmp/django-bunny-1.0.4.tar.gz` & `tmp/django-bunny-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bunny-1.0.4.tar", max compression
+gzip compressed data, was "django-bunny-1.0.5.tar", max compression
```

## Comparing `django-bunny-1.0.4.tar` & `django-bunny-1.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-09 02:51:37.446276 django-bunny-1.0.4/django_bunny/__init__.py
--rw-r--r--   0        0        0     6038 2023-05-09 03:52:49.306311 django-bunny-1.0.4/django_bunny/storage.py
--rw-r--r--   0        0        0     1092 2023-05-09 01:04:30.492122 django-bunny-1.0.4/LICENSE
--rw-r--r--   0        0        0      855 2023-05-09 03:48:52.025939 django-bunny-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2243 2023-05-09 02:51:17.790012 django-bunny-1.0.4/README.md
--rw-r--r--   0        0        0     2966 1970-01-01 00:00:00.000000 django-bunny-1.0.4/setup.py
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 django-bunny-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-09 02:51:37.446276 django-bunny-1.0.5/django_bunny/__init__.py
+-rw-r--r--   0        0        0     5948 2023-05-09 04:53:56.669757 django-bunny-1.0.5/django_bunny/storage.py
+-rw-r--r--   0        0        0     1092 2023-05-09 01:04:30.492122 django-bunny-1.0.5/LICENSE
+-rw-r--r--   0        0        0      855 2023-05-09 04:54:13.994038 django-bunny-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2243 2023-05-09 02:51:17.790012 django-bunny-1.0.5/README.md
+-rw-r--r--   0        0        0     2966 1970-01-01 00:00:00.000000 django-bunny-1.0.5/setup.py
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 django-bunny-1.0.5/PKG-INFO
```

### Comparing `django-bunny-1.0.4/django_bunny/storage.py` & `django-bunny-1.0.5/django_bunny/storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,68 +88,68 @@
 
         self.base_url += f"{username}/"
         self.headers = {"AccessKey": password}
 
     def _full_path(self, name) -> str:
         if name == "/":
             name = ""
-        return safe_join(self.base_url, name).replace("\\", "/")
+        return self.base_url + name.replace("\\", "/")
 
     def _save(self, name, content) -> str:
         r = requests.put(
-            safe_join(self.base_url, name), data=content, headers=self.headers
+            self.base_url + name, data=content, headers=self.headers
         )
         return name
 
     def _open(self, name, mode="rb"):
-        r = requests.get(safe_join(self.base_url, name), headers=self.headers)
+        r = requests.get(self.base_url + name, headers=self.headers)
         r.raise_for_status()
 
         return r.raw
 
     def delete(self, name) -> str:
-        r = requests.delete(safe_join(self.base_url, name), headers=self.headers)
+        r = requests.delete(self.base_url + name, headers=self.headers)
 
         return name
 
     def exists(self, name) -> bool:
-        r = requests.head(safe_join(self.base_url, name), headers=self.headers)
+        r = requests.head(self.base_url + name, headers=self.headers)
 
         if r.status_code == 404:
             return False
 
         r.raise_for_status()
 
         return True
 
     def url(self, name: str) -> str:
-        return safe_join(self.hostname, name)
+        return self.hostname + name
 
     def size(self, name: str) -> int:
         r = requests.head(self.url(name))
         r.raise_for_status()
 
         file_size = r.headers.get("Content-Length", 0)
 
         return int(file_size)
 
     def listdir(self, path) -> tuple:
-        r = requests.get(safe_join(self.base_url, path), headers=self.headers)
+        r = requests.get(self.base_url + path, headers=self.headers)
         r.raise_for_status()
 
         objects = r.json()
 
         return (
             [item["ObjectName"] for item in objects if item["IsDirectory"]],
             [item["ObjectName"] for item in objects if not item["IsDirectory"]],
         )
 
     def get_created_time(self, name) -> datetime.datetime:
         r = requests.get(
-            safe_join(self.base_url, name.rsplit("/", 1)[0]), headers=self.headers
+            self.base_url + name.rsplit("/", 1)[0], headers=self.headers
         )
         r.raise_for_status()
 
         iso_date = None
 
         for item in r.json():
             if item["ObjectName"] == name:
@@ -168,15 +168,15 @@
             parsed_date.replace(tzinfo=datetime.timezone.utc)
             parsed_date.astimezone()
             parsed_date.replace(tzinfo=None)
             return parsed_date
 
     def get_modified_time(self, name) -> datetime.datetime:
         r = requests.get(
-            safe_join(self.base_url, name.rsplit("/", 1)[0]), headers=self.headers
+            self.base_url + name.rsplit("/", 1)[0], headers=self.headers
         )
         r.raise_for_status()
 
         iso_date = None
 
         for item in r.json():
             if item["ObjectName"] == name.rsplit("/", 1)[1]:
```

### Comparing `django-bunny-1.0.4/LICENSE` & `django-bunny-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bunny-1.0.4/pyproject.toml` & `django-bunny-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-bunny"
-version = "1.0.4"
+version = "1.0.5"
 description = "A django storage for bunny.net"
 authors = ["Neki <neki@nekidev.com>"]
 maintainers = ["Neki <neki@nekidev.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_bunny"}]
 homepage = "https://github.com/Nekidev/django-bunny/"
```

### Comparing `django-bunny-1.0.4/README.md` & `django-bunny-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `django-bunny-1.0.4/setup.py` & `django-bunny-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Django>=3.0.0', 'python-dateutil>=2.8.2,<3.0.0', 'requests>=2.30.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'django-bunny',
-    'version': '1.0.4',
+    'version': '1.0.5',
     'description': 'A django storage for bunny.net',
     'long_description': '# django-bunny\n\nA bunny.net storage for Django. It was created as a replacement for [django-bunny-storage](https://github.com/willmeyers/django-bunny-storage).\n\n\n## Installation\n\nYou can install the library using `pip`:\n\n```bash\npip install django-bunny\n```\n\n\n## Configuration\n\nFirst, add `django_bunny` to your `INSTALLED_APPS`:\n\n```py\nINSTALLED_APPS = [\n    ...,\n    "django_bunny",\n    ...\n]\n```\n\nNow, create the following variables inside your `settings.py` file. These are required if you are using Django < `4.2`. Otherwise, you can use `OPTIONS` in the `STORAGES` setting.\n\n```py\n# These can be found in your storage\'s dashboard under `FTP & API Access`\nBUNNY_USERNAME = "my-storage-name"\nBUNNY_PASSWORD = "my-storage-password"\n\n# This is the storage region\'s code. E.g. Los Angeles is `la`, Singapore is\n# `sg`, etc. The default is `ny` (New York).\nBUNNY_REGION = "my-storage-region"\n\n# Optional. For example, `https://myzone.b-cdn.net/`. `MEDIA_URL` will be used\n# if this is not set.\nBUNNY_HOSTNAME = "my-pullzone-hostname"\n```\n\nFinally, depending on which version of Django you are using you\'ll need to create one of these variables:\n\n```py\n# Django < 4.2\nDEFAULT_FILE_STORAGE = \'django_bunny.storage.BunnyStorage\'\n\n# Django >= 4.2. Set `BunnyStorage` where you want to use bunny.net\'s storage.\n{\n    "default": {\n        "BACKEND": "django_bunny.storage.BunnyStorage",\n\n        # Add this if you did not create the BUNNY_* settings before. They are\n        # the same as BUNNY_* variables.\n        "OPTIONS": {\n            "username": "my-storage-name",\n            "password": "my-storage-password",\n            \n            # Optional. Defaults to `ny`\n            "region": "my-storage-region",\n            \n            # Optional. `MEDIA_URL` will be used if it is not set\n            "hostname": "my-pullzone-hostname"\n        }\n    },\n}\n```\n\nIn Django >= 4.2 you can set different credentials for the different storages. This allows you to, for example, use a separate storage for static files.\n\n\n## Using in templates\n\nIn templates, you can use `{{ instance.file.url }}` directly. For example:\n\n```html\n<img src="{{ instance.file.url }}" />\n```\n',
     'author': 'Neki',
     'author_email': 'neki@nekidev.com',
     'maintainer': 'Neki',
     'maintainer_email': 'neki@nekidev.com',
     'url': 'https://github.com/Nekidev/django-bunny/',
```

### Comparing `django-bunny-1.0.4/PKG-INFO` & `django-bunny-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bunny
-Version: 1.0.4
+Version: 1.0.5
 Summary: A django storage for bunny.net
 Home-page: https://github.com/Nekidev/django-bunny/
 License: MIT
 Keywords: django,bunnycdn,django-storage
 Author: Neki
 Author-email: neki@nekidev.com
 Maintainer: Neki
```

