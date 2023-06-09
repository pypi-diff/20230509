# Comparing `tmp/django-bunny-1.0.7.tar.gz` & `tmp/django-bunny-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bunny-1.0.7.tar", max compression
+gzip compressed data, was "django-bunny-1.0.8.tar", max compression
```

## Comparing `django-bunny-1.0.7.tar` & `django-bunny-1.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-09 02:51:37.446276 django-bunny-1.0.7/django_bunny/__init__.py
--rw-r--r--   0        0        0     5922 2023-05-09 05:11:48.924060 django-bunny-1.0.7/django_bunny/storage.py
--rw-r--r--   0        0        0     1092 2023-05-09 01:04:30.492122 django-bunny-1.0.7/LICENSE
--rw-r--r--   0        0        0      855 2023-05-09 05:11:55.789059 django-bunny-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2243 2023-05-09 02:51:17.790012 django-bunny-1.0.7/README.md
--rw-r--r--   0        0        0     2966 1970-01-01 00:00:00.000000 django-bunny-1.0.7/setup.py
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 django-bunny-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-09 02:51:37.446276 django-bunny-1.0.8/django_bunny/__init__.py
+-rw-r--r--   0        0        0     5934 2023-05-09 05:13:34.957058 django-bunny-1.0.8/django_bunny/storage.py
+-rw-r--r--   0        0        0     1092 2023-05-09 01:04:30.492122 django-bunny-1.0.8/LICENSE
+-rw-r--r--   0        0        0      855 2023-05-09 05:13:51.257059 django-bunny-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2243 2023-05-09 02:51:17.790012 django-bunny-1.0.8/README.md
+-rw-r--r--   0        0        0     2966 1970-01-01 00:00:00.000000 django-bunny-1.0.8/setup.py
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 django-bunny-1.0.8/PKG-INFO
```

### Comparing `django-bunny-1.0.7/django_bunny/storage.py` & `django-bunny-1.0.8/django_bunny/storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -92,50 +92,50 @@
     def _full_path(self, name) -> str:
         if name == "/":
             name = ""
         return self.base_url + name.replace("\\", "/")
 
     def _save(self, name, content) -> str:
         r = requests.put(
-            self.base_url + name, data=content, headers=self.headers
+            self._full_path(name), data=content, headers=self.headers
         )
         return name
 
     def _open(self, name, mode="rb"):
-        r = requests.get(self.base_url + name, headers=self.headers)
+        r = requests.get(self._full_path(name), headers=self.headers)
         r.raise_for_status()
 
         return r.raw
 
     def delete(self, name) -> str:
-        r = requests.delete(self.base_url + name, headers=self.headers)
+        r = requests.delete(self._full_path(name), headers=self.headers)
 
         return name
 
     def exists(self, name) -> bool:
-        r = requests.head(self.base_url + name, headers=self.headers)
+        r = requests.head(self._full_path(name), headers=self.headers)
 
         if r.status_code == 404:
             return False
 
         return True
 
     def url(self, name: str) -> str:
         return self._full_path(name)
 
     def size(self, name: str) -> int:
-        r = requests.head(self.url(name))
+        r = requests.head(self._full_path(name))
         r.raise_for_status()
 
         file_size = r.headers.get("Content-Length", 0)
 
         return int(file_size)
 
     def listdir(self, path) -> tuple:
-        r = requests.get(self.base_url + path, headers=self.headers)
+        r = requests.get(self._full_path(name), headers=self.headers)
         r.raise_for_status()
 
         objects = r.json()
 
         return (
             [item["ObjectName"] for item in objects if item["IsDirectory"]],
             [item["ObjectName"] for item in objects if not item["IsDirectory"]],
```

### Comparing `django-bunny-1.0.7/LICENSE` & `django-bunny-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bunny-1.0.7/pyproject.toml` & `django-bunny-1.0.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-bunny"
-version = "1.0.7"
+version = "1.0.8"
 description = "A django storage for bunny.net"
 authors = ["Neki <neki@nekidev.com>"]
 maintainers = ["Neki <neki@nekidev.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_bunny"}]
 homepage = "https://github.com/Nekidev/django-bunny/"
```

### Comparing `django-bunny-1.0.7/README.md` & `django-bunny-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `django-bunny-1.0.7/setup.py` & `django-bunny-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Django>=3.0.0', 'python-dateutil>=2.8.2,<3.0.0', 'requests>=2.30.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'django-bunny',
-    'version': '1.0.7',
+    'version': '1.0.8',
     'description': 'A django storage for bunny.net',
     'long_description': '# django-bunny\n\nA bunny.net storage for Django. It was created as a replacement for [django-bunny-storage](https://github.com/willmeyers/django-bunny-storage).\n\n\n## Installation\n\nYou can install the library using `pip`:\n\n```bash\npip install django-bunny\n```\n\n\n## Configuration\n\nFirst, add `django_bunny` to your `INSTALLED_APPS`:\n\n```py\nINSTALLED_APPS = [\n    ...,\n    "django_bunny",\n    ...\n]\n```\n\nNow, create the following variables inside your `settings.py` file. These are required if you are using Django < `4.2`. Otherwise, you can use `OPTIONS` in the `STORAGES` setting.\n\n```py\n# These can be found in your storage\'s dashboard under `FTP & API Access`\nBUNNY_USERNAME = "my-storage-name"\nBUNNY_PASSWORD = "my-storage-password"\n\n# This is the storage region\'s code. E.g. Los Angeles is `la`, Singapore is\n# `sg`, etc. The default is `ny` (New York).\nBUNNY_REGION = "my-storage-region"\n\n# Optional. For example, `https://myzone.b-cdn.net/`. `MEDIA_URL` will be used\n# if this is not set.\nBUNNY_HOSTNAME = "my-pullzone-hostname"\n```\n\nFinally, depending on which version of Django you are using you\'ll need to create one of these variables:\n\n```py\n# Django < 4.2\nDEFAULT_FILE_STORAGE = \'django_bunny.storage.BunnyStorage\'\n\n# Django >= 4.2. Set `BunnyStorage` where you want to use bunny.net\'s storage.\n{\n    "default": {\n        "BACKEND": "django_bunny.storage.BunnyStorage",\n\n        # Add this if you did not create the BUNNY_* settings before. They are\n        # the same as BUNNY_* variables.\n        "OPTIONS": {\n            "username": "my-storage-name",\n            "password": "my-storage-password",\n            \n            # Optional. Defaults to `ny`\n            "region": "my-storage-region",\n            \n            # Optional. `MEDIA_URL` will be used if it is not set\n            "hostname": "my-pullzone-hostname"\n        }\n    },\n}\n```\n\nIn Django >= 4.2 you can set different credentials for the different storages. This allows you to, for example, use a separate storage for static files.\n\n\n## Using in templates\n\nIn templates, you can use `{{ instance.file.url }}` directly. For example:\n\n```html\n<img src="{{ instance.file.url }}" />\n```\n',
     'author': 'Neki',
     'author_email': 'neki@nekidev.com',
     'maintainer': 'Neki',
     'maintainer_email': 'neki@nekidev.com',
     'url': 'https://github.com/Nekidev/django-bunny/',
```

### Comparing `django-bunny-1.0.7/PKG-INFO` & `django-bunny-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bunny
-Version: 1.0.7
+Version: 1.0.8
 Summary: A django storage for bunny.net
 Home-page: https://github.com/Nekidev/django-bunny/
 License: MIT
 Keywords: django,bunnycdn,django-storage
 Author: Neki
 Author-email: neki@nekidev.com
 Maintainer: Neki
```

