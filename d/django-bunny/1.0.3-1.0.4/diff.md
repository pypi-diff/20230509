# Comparing `tmp/django-bunny-1.0.3.tar.gz` & `tmp/django-bunny-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bunny-1.0.3.tar", max compression
+gzip compressed data, was "django-bunny-1.0.4.tar", max compression
```

## Comparing `django-bunny-1.0.3.tar` & `django-bunny-1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-09 02:51:37.446276 django-bunny-1.0.3/django_bunny/__init__.py
--rw-r--r--   0        0        0     5356 2023-05-09 02:58:06.645257 django-bunny-1.0.3/django_bunny/storage.py
--rw-r--r--   0        0        0     1092 2023-05-09 01:04:30.492122 django-bunny-1.0.3/LICENSE
--rw-r--r--   0        0        0      855 2023-05-09 03:31:43.677855 django-bunny-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2243 2023-05-09 02:51:17.790012 django-bunny-1.0.3/README.md
--rw-r--r--   0        0        0     2966 1970-01-01 00:00:00.000000 django-bunny-1.0.3/setup.py
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 django-bunny-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-09 02:51:37.446276 django-bunny-1.0.4/django_bunny/__init__.py
+-rw-r--r--   0        0        0     6038 2023-05-09 03:52:49.306311 django-bunny-1.0.4/django_bunny/storage.py
+-rw-r--r--   0        0        0     1092 2023-05-09 01:04:30.492122 django-bunny-1.0.4/LICENSE
+-rw-r--r--   0        0        0      855 2023-05-09 03:48:52.025939 django-bunny-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2243 2023-05-09 02:51:17.790012 django-bunny-1.0.4/README.md
+-rw-r--r--   0        0        0     2966 1970-01-01 00:00:00.000000 django-bunny-1.0.4/setup.py
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 django-bunny-1.0.4/PKG-INFO
```

### Comparing `django-bunny-1.0.3/django_bunny/storage.py` & `django-bunny-1.0.4/django_bunny/storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,34 +21,52 @@
     region = None
     hostname = None
 
     base_url = None
     headers = None
 
     def __init__(self, **kwargs):
-        username = (
-            kwargs["username"] if "username" in kwargs else settings.BUNNY_USERNAME
-        )
-        password = (
-            kwargs["password"] if "password" in kwargs else settings.BUNNY_PASSWORD
-        )
+        try:
+            username = (
+                kwargs["username"] if "username" in kwargs else settings.BUNNY_USERNAME
+            )
+        except AttributeError:
+            raise ImproperlyConfigured(
+                "Setting BUNNY_USERNAME or `username` option is required."
+            )
+        
+        try:
+            password = (
+                kwargs["password"] if "password" in kwargs else settings.BUNNY_PASSWORD
+            )
+        except AttributeError:
+            raise ImproperlyConfigured(
+                "Setting BUNNY_PASSWORD or `password` option is required."
+            )
+        
         region = (
             kwargs["region"]
             if "region" in kwargs
             else settings.BUNNY_REGION
-            if settings.BUNNY_REGION
+            if hasattr(settings, 'BUNNY_REGION')
             else "ny"
         )
-        hostname = (
-            kwargs["hostname"]
-            if "hostname" in kwargs
-            else settings.BUNNY_HOSTNAME
-            if settings.BUNNY_HOSTNAME
-            else settings.MEDIA_URL
-        )
+        
+        try:
+            hostname = (
+                kwargs["hostname"]
+                if "hostname" in kwargs
+                else settings.BUNNY_HOSTNAME
+                if hasattr(settings, 'BUNNY_HOSTNAME')
+                else settings.MEDIA_URL
+            )
+        except AttributeError:
+            raise ImproperlyConfigured(
+                "Neither `BUNNY_HOSTNAME` or `MEDIA_URL` are configured. django-bunny requires one of them to work."
+            )
 
         if not username:
             raise ImproperlyConfigured(
                 "Setting BUNNY_USERNAME or `username` option is required."
             )
 
         if not password:
```

### Comparing `django-bunny-1.0.3/LICENSE` & `django-bunny-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bunny-1.0.3/pyproject.toml` & `django-bunny-1.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-bunny"
-version = "1.0.3"
+version = "1.0.4"
 description = "A django storage for bunny.net"
 authors = ["Neki <neki@nekidev.com>"]
 maintainers = ["Neki <neki@nekidev.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_bunny"}]
 homepage = "https://github.com/Nekidev/django-bunny/"
```

### Comparing `django-bunny-1.0.3/README.md` & `django-bunny-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django-bunny-1.0.3/setup.py` & `django-bunny-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Django>=3.0.0', 'python-dateutil>=2.8.2,<3.0.0', 'requests>=2.30.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'django-bunny',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': 'A django storage for bunny.net',
     'long_description': '# django-bunny\n\nA bunny.net storage for Django. It was created as a replacement for [django-bunny-storage](https://github.com/willmeyers/django-bunny-storage).\n\n\n## Installation\n\nYou can install the library using `pip`:\n\n```bash\npip install django-bunny\n```\n\n\n## Configuration\n\nFirst, add `django_bunny` to your `INSTALLED_APPS`:\n\n```py\nINSTALLED_APPS = [\n    ...,\n    "django_bunny",\n    ...\n]\n```\n\nNow, create the following variables inside your `settings.py` file. These are required if you are using Django < `4.2`. Otherwise, you can use `OPTIONS` in the `STORAGES` setting.\n\n```py\n# These can be found in your storage\'s dashboard under `FTP & API Access`\nBUNNY_USERNAME = "my-storage-name"\nBUNNY_PASSWORD = "my-storage-password"\n\n# This is the storage region\'s code. E.g. Los Angeles is `la`, Singapore is\n# `sg`, etc. The default is `ny` (New York).\nBUNNY_REGION = "my-storage-region"\n\n# Optional. For example, `https://myzone.b-cdn.net/`. `MEDIA_URL` will be used\n# if this is not set.\nBUNNY_HOSTNAME = "my-pullzone-hostname"\n```\n\nFinally, depending on which version of Django you are using you\'ll need to create one of these variables:\n\n```py\n# Django < 4.2\nDEFAULT_FILE_STORAGE = \'django_bunny.storage.BunnyStorage\'\n\n# Django >= 4.2. Set `BunnyStorage` where you want to use bunny.net\'s storage.\n{\n    "default": {\n        "BACKEND": "django_bunny.storage.BunnyStorage",\n\n        # Add this if you did not create the BUNNY_* settings before. They are\n        # the same as BUNNY_* variables.\n        "OPTIONS": {\n            "username": "my-storage-name",\n            "password": "my-storage-password",\n            \n            # Optional. Defaults to `ny`\n            "region": "my-storage-region",\n            \n            # Optional. `MEDIA_URL` will be used if it is not set\n            "hostname": "my-pullzone-hostname"\n        }\n    },\n}\n```\n\nIn Django >= 4.2 you can set different credentials for the different storages. This allows you to, for example, use a separate storage for static files.\n\n\n## Using in templates\n\nIn templates, you can use `{{ instance.file.url }}` directly. For example:\n\n```html\n<img src="{{ instance.file.url }}" />\n```\n',
     'author': 'Neki',
     'author_email': 'neki@nekidev.com',
     'maintainer': 'Neki',
     'maintainer_email': 'neki@nekidev.com',
     'url': 'https://github.com/Nekidev/django-bunny/',
```

### Comparing `django-bunny-1.0.3/PKG-INFO` & `django-bunny-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bunny
-Version: 1.0.3
+Version: 1.0.4
 Summary: A django storage for bunny.net
 Home-page: https://github.com/Nekidev/django-bunny/
 License: MIT
 Keywords: django,bunnycdn,django-storage
 Author: Neki
 Author-email: neki@nekidev.com
 Maintainer: Neki
```

