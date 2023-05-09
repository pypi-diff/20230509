# Comparing `tmp/django-bcmr-0.1.8.tar.gz` & `tmp/django-bcmr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-bcmr-0.1.8.tar", last modified: Wed May  3 00:45:03 2023, max compression
+gzip compressed data, was "dist/django-bcmr-0.1.9.tar", last modified: Tue May  9 07:42:32 2023, max compression
```

## Comparing `django-bcmr-0.1.8.tar` & `django-bcmr-0.1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/
--rw-rw-r--   0 jethro    (1000) jethro    (1000)     5915 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/PKG-INFO
--rw-rw-r--   0 jethro    (1000) jethro    (1000)       38 2023-02-13 06:18:11.000000 django-bcmr-0.1.8/setup.py
-drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/bcmr/
--rw-rw-r--   0 jethro    (1000) jethro    (1000)       44 2023-02-13 06:16:46.000000 django-bcmr-0.1.8/bcmr/__init__.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)       60 2023-02-13 06:16:46.000000 django-bcmr-0.1.8/bcmr/tests.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)      296 2023-03-29 07:53:29.000000 django-bcmr-0.1.8/bcmr/forms.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)     3137 2023-05-02 09:04:31.000000 django-bcmr-0.1.8/bcmr/models.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)     2169 2023-03-30 01:54:09.000000 django-bcmr-0.1.8/bcmr/auth.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)     5015 2023-05-02 10:52:49.000000 django-bcmr-0.1.8/bcmr/serializers.py
-drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/bcmr/migrations/
--rw-rw-r--   0 jethro    (1000) jethro    (1000)        0 2023-02-13 06:16:46.000000 django-bcmr-0.1.8/bcmr/migrations/__init__.py
--rw-r--r--   0 jethro    (1000) jethro    (1000)      755 2023-02-13 06:16:46.000000 django-bcmr-0.1.8/bcmr/migrations/0003_auto_20230213_0237.py
--rw-r--r--   0 jethro    (1000) jethro    (1000)      844 2023-05-02 08:29:24.000000 django-bcmr-0.1.8/bcmr/migrations/0010_tokenhistory.py
--rw-r--r--   0 jethro    (1000) jethro    (1000)      397 2023-03-31 01:31:44.000000 django-bcmr-0.1.8/bcmr/migrations/0008_auto_20230331_0131.py
--rw-r--r--   0 jethro    (1000) jethro    (1000)      417 2023-03-31 01:33:51.000000 django-bcmr-0.1.8/bcmr/migrations/0009_auto_20230331_0133.py
--rw-r--r--   0 jethro    (1000) jethro    (1000)      334 2023-05-02 08:55:20.000000 django-bcmr-0.1.8/bcmr/migrations/0012_remove_tokenhistory_category.py
--rw-r--r--   0 jethro    (1000) jethro    (1000)      521 2023-02-14 04:01:28.000000 django-bcmr-0.1.8/bcmr/migrations/0004_auto_20230214_0401.py
--rw-r--r--   0 jethro    (1000) jethro    (1000)     1103 2023-03-30 02:03:07.000000 django-bcmr-0.1.8/bcmr/migrations/0006_auto_20230330_0203.py
--rw-r--r--   0 jethro    (1000) jethro    (1000)      490 2023-02-27 06:12:45.000000 django-bcmr-0.1.8/bcmr/migrations/0005_auto_20230227_0612.py
--rw-r--r--   0 jethro    (1000) jethro    (1000)     2071 2023-02-13 06:16:46.000000 django-bcmr-0.1.8/bcmr/migrations/0001_initial.py
--rw-r--r--   0 jethro    (1000) jethro    (1000)      387 2023-05-02 08:39:22.000000 django-bcmr-0.1.8/bcmr/migrations/0011_auto_20230502_0839.py
--rw-r--r--   0 jethro    (1000) jethro    (1000)      453 2023-02-13 06:16:46.000000 django-bcmr-0.1.8/bcmr/migrations/0002_authtoken.py
--rw-r--r--   0 jethro    (1000) jethro    (1000)      558 2023-03-30 02:25:40.000000 django-bcmr-0.1.8/bcmr/migrations/0007_auto_20230330_0225.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)      827 2023-05-02 08:24:30.000000 django-bcmr-0.1.8/bcmr/signals.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)      789 2023-05-02 08:54:19.000000 django-bcmr-0.1.8/bcmr/admin.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)      133 2023-02-13 06:16:46.000000 django-bcmr-0.1.8/bcmr/apps.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)      331 2023-03-29 07:53:29.000000 django-bcmr-0.1.8/bcmr/urls.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)      376 2023-03-29 08:34:25.000000 django-bcmr-0.1.8/bcmr/filters.py
-drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/bcmr/templates/
-drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/bcmr/templates/docs/
--rw-rw-r--   0 jethro    (1000) jethro    (1000)      836 2023-02-13 06:16:46.000000 django-bcmr-0.1.8/bcmr/templates/docs/swagger-ui.html
-drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/bcmr/templates/bcmr/
--rw-rw-r--   0 jethro    (1000) jethro    (1000)     1742 2023-02-27 04:06:46.000000 django-bcmr-0.1.8/bcmr/templates/bcmr/create_token.html
--rw-rw-r--   0 jethro    (1000) jethro    (1000)      810 2023-05-02 10:56:08.000000 django-bcmr-0.1.8/bcmr/utils.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)     5736 2023-05-02 09:22:12.000000 django-bcmr-0.1.8/bcmr/views.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)     1011 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/setup.cfg
--rw-rw-r--   0 jethro    (1000) jethro    (1000)      109 2023-02-13 06:18:42.000000 django-bcmr-0.1.8/pyproject.toml
--rw-rw-r--   0 jethro    (1000) jethro    (1000)     3896 2023-03-06 03:30:30.000000 django-bcmr-0.1.8/README.rst
--rw-rw-r--   0 jethro    (1000) jethro    (1000)      158 2023-02-13 06:18:46.000000 django-bcmr-0.1.8/MANIFEST.in
-drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/django_bcmr.egg-info/
--rw-rw-r--   0 jethro    (1000) jethro    (1000)     5915 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/django_bcmr.egg-info/PKG-INFO
--rw-rw-r--   0 jethro    (1000) jethro    (1000)       26 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/django_bcmr.egg-info/requires.txt
--rw-rw-r--   0 jethro    (1000) jethro    (1000)        1 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/django_bcmr.egg-info/dependency_links.txt
--rw-rw-r--   0 jethro    (1000) jethro    (1000)       17 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/django_bcmr.egg-info/top_level.txt
--rw-rw-r--   0 jethro    (1000) jethro    (1000)     1141 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/django_bcmr.egg-info/SOURCES.txt
--rw-rw-r--   0 jethro    (1000) jethro    (1000)     1062 2023-02-13 06:18:58.000000 django-bcmr-0.1.8/LICENSE
-drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-03 00:45:03.000000 django-bcmr-0.1.8/django-bcmr/
--rw-rw-r--   0 jethro    (1000) jethro    (1000)        0 2023-02-07 09:19:19.000000 django-bcmr-0.1.8/django-bcmr/__init__.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)      392 2023-02-09 08:01:06.000000 django-bcmr-0.1.8/django-bcmr/wsgi.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)      392 2023-02-09 08:01:31.000000 django-bcmr-0.1.8/django-bcmr/asgi.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)     1847 2023-02-27 07:47:00.000000 django-bcmr-0.1.8/django-bcmr/urls.py
--rw-rw-r--   0 jethro    (1000) jethro    (1000)     5552 2023-02-27 04:09:40.000000 django-bcmr-0.1.8/django-bcmr/settings.py
+drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)     5915 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/PKG-INFO
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)       38 2023-02-13 06:18:11.000000 django-bcmr-0.1.9/setup.py
+drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/bcmr/
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)       44 2023-02-13 06:16:46.000000 django-bcmr-0.1.9/bcmr/__init__.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)       60 2023-02-13 06:16:46.000000 django-bcmr-0.1.9/bcmr/tests.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)      296 2023-03-29 07:53:29.000000 django-bcmr-0.1.9/bcmr/forms.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)     3137 2023-05-02 09:04:31.000000 django-bcmr-0.1.9/bcmr/models.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)     2169 2023-03-30 01:54:09.000000 django-bcmr-0.1.9/bcmr/auth.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)     5019 2023-05-09 07:39:37.000000 django-bcmr-0.1.9/bcmr/serializers.py
+drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/bcmr/migrations/
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)        0 2023-02-13 06:16:46.000000 django-bcmr-0.1.9/bcmr/migrations/__init__.py
+-rw-r--r--   0 jethro    (1000) jethro    (1000)      755 2023-02-13 06:16:46.000000 django-bcmr-0.1.9/bcmr/migrations/0003_auto_20230213_0237.py
+-rw-r--r--   0 jethro    (1000) jethro    (1000)      844 2023-05-02 08:29:24.000000 django-bcmr-0.1.9/bcmr/migrations/0010_tokenhistory.py
+-rw-r--r--   0 jethro    (1000) jethro    (1000)      397 2023-03-31 01:31:44.000000 django-bcmr-0.1.9/bcmr/migrations/0008_auto_20230331_0131.py
+-rw-r--r--   0 jethro    (1000) jethro    (1000)      417 2023-03-31 01:33:51.000000 django-bcmr-0.1.9/bcmr/migrations/0009_auto_20230331_0133.py
+-rw-r--r--   0 jethro    (1000) jethro    (1000)      334 2023-05-02 08:55:20.000000 django-bcmr-0.1.9/bcmr/migrations/0012_remove_tokenhistory_category.py
+-rw-r--r--   0 jethro    (1000) jethro    (1000)      521 2023-02-14 04:01:28.000000 django-bcmr-0.1.9/bcmr/migrations/0004_auto_20230214_0401.py
+-rw-r--r--   0 jethro    (1000) jethro    (1000)     1103 2023-03-30 02:03:07.000000 django-bcmr-0.1.9/bcmr/migrations/0006_auto_20230330_0203.py
+-rw-r--r--   0 jethro    (1000) jethro    (1000)      490 2023-02-27 06:12:45.000000 django-bcmr-0.1.9/bcmr/migrations/0005_auto_20230227_0612.py
+-rw-r--r--   0 jethro    (1000) jethro    (1000)     2071 2023-02-13 06:16:46.000000 django-bcmr-0.1.9/bcmr/migrations/0001_initial.py
+-rw-r--r--   0 jethro    (1000) jethro    (1000)      387 2023-05-02 08:39:22.000000 django-bcmr-0.1.9/bcmr/migrations/0011_auto_20230502_0839.py
+-rw-r--r--   0 jethro    (1000) jethro    (1000)      453 2023-02-13 06:16:46.000000 django-bcmr-0.1.9/bcmr/migrations/0002_authtoken.py
+-rw-r--r--   0 jethro    (1000) jethro    (1000)      558 2023-03-30 02:25:40.000000 django-bcmr-0.1.9/bcmr/migrations/0007_auto_20230330_0225.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)      827 2023-05-02 08:24:30.000000 django-bcmr-0.1.9/bcmr/signals.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)      789 2023-05-02 08:54:19.000000 django-bcmr-0.1.9/bcmr/admin.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)      133 2023-02-13 06:16:46.000000 django-bcmr-0.1.9/bcmr/apps.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)      331 2023-03-29 07:53:29.000000 django-bcmr-0.1.9/bcmr/urls.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)      376 2023-03-29 08:34:25.000000 django-bcmr-0.1.9/bcmr/filters.py
+drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/bcmr/templates/
+drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/bcmr/templates/docs/
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)      836 2023-02-13 06:16:46.000000 django-bcmr-0.1.9/bcmr/templates/docs/swagger-ui.html
+drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/bcmr/templates/bcmr/
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)     1742 2023-02-27 04:06:46.000000 django-bcmr-0.1.9/bcmr/templates/bcmr/create_token.html
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)      810 2023-05-02 10:56:08.000000 django-bcmr-0.1.9/bcmr/utils.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)     5744 2023-05-09 07:39:46.000000 django-bcmr-0.1.9/bcmr/views.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)     1011 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/setup.cfg
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)      109 2023-02-13 06:18:42.000000 django-bcmr-0.1.9/pyproject.toml
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)     3896 2023-03-06 03:30:30.000000 django-bcmr-0.1.9/README.rst
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)      158 2023-02-13 06:18:46.000000 django-bcmr-0.1.9/MANIFEST.in
+drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/django_bcmr.egg-info/
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)     5915 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/django_bcmr.egg-info/PKG-INFO
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)       26 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/django_bcmr.egg-info/requires.txt
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)        1 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/django_bcmr.egg-info/dependency_links.txt
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)       17 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/django_bcmr.egg-info/top_level.txt
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)     1141 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/django_bcmr.egg-info/SOURCES.txt
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)     1062 2023-02-13 06:18:58.000000 django-bcmr-0.1.9/LICENSE
+drwxrwxr-x   0 jethro    (1000) jethro    (1000)        0 2023-05-09 07:42:32.000000 django-bcmr-0.1.9/django-bcmr/
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)        0 2023-02-07 09:19:19.000000 django-bcmr-0.1.9/django-bcmr/__init__.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)      392 2023-02-09 08:01:06.000000 django-bcmr-0.1.9/django-bcmr/wsgi.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)      392 2023-02-09 08:01:31.000000 django-bcmr-0.1.9/django-bcmr/asgi.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)     1847 2023-02-27 07:47:00.000000 django-bcmr-0.1.9/django-bcmr/urls.py
+-rw-rw-r--   0 jethro    (1000) jethro    (1000)     5552 2023-02-27 04:09:40.000000 django-bcmr-0.1.9/django-bcmr/settings.py
```

### Comparing `django-bcmr-0.1.8/PKG-INFO` & `django-bcmr-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-bcmr
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Django app for storing, accessing and managing CashToken Bitcoin Cash Metadata Registries
 Home-page: https://github.com/paytaca/django-bcmr
 Author: Paytaca
 Author-email: info@paytaca.com
 License: BSD-3-Clause
 Description: =====
         BCMR
```

### Comparing `django-bcmr-0.1.8/bcmr/models.py` & `django-bcmr-0.1.9/bcmr/models.py`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/bcmr/auth.py` & `django-bcmr-0.1.9/bcmr/auth.py`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/bcmr/serializers.py` & `django-bcmr-0.1.9/bcmr/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         )
         read_only_fields = (
             'date_created',
             'owner',
         )
 
 
-class TokenSerializer(serializers.ModelSerializer):
+class MainTokenSerializer(serializers.ModelSerializer):
     token = serializers.SerializerMethodField()
     uris = serializers.SerializerMethodField()
 
     class Meta:
         model = Token
         fields = (
             'name',
```

### Comparing `django-bcmr-0.1.8/bcmr/migrations/0003_auto_20230213_0237.py` & `django-bcmr-0.1.9/bcmr/migrations/0003_auto_20230213_0237.py`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/bcmr/migrations/0010_tokenhistory.py` & `django-bcmr-0.1.9/bcmr/migrations/0010_tokenhistory.py`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/bcmr/migrations/0004_auto_20230214_0401.py` & `django-bcmr-0.1.9/bcmr/migrations/0004_auto_20230214_0401.py`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/bcmr/migrations/0006_auto_20230330_0203.py` & `django-bcmr-0.1.9/bcmr/migrations/0006_auto_20230330_0203.py`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/bcmr/migrations/0001_initial.py` & `django-bcmr-0.1.9/bcmr/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/bcmr/migrations/0007_auto_20230330_0225.py` & `django-bcmr-0.1.9/bcmr/migrations/0007_auto_20230330_0225.py`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/bcmr/signals.py` & `django-bcmr-0.1.9/bcmr/signals.py`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/bcmr/admin.py` & `django-bcmr-0.1.9/bcmr/admin.py`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/bcmr/templates/docs/swagger-ui.html` & `django-bcmr-0.1.9/bcmr/templates/docs/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/bcmr/templates/bcmr/create_token.html` & `django-bcmr-0.1.9/bcmr/templates/bcmr/create_token.html`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/bcmr/utils.py` & `django-bcmr-0.1.9/bcmr/utils.py`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/bcmr/views.py` & `django-bcmr-0.1.9/bcmr/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,18 @@
     queryset = Token.objects.all()
     filterset_class = TokenFilter
     filter_backends = (filters.DjangoFilterBackend, )
     authentication_classes = (HeaderAuthentication, )
     serializer_class = EmptySerializer
     serializer_classes = {
         'create': CashTokenSerializer,
-        'list': TokenSerializer,
+        'list': MainTokenSerializer,
         'update': CashTokenSerializer,
         'partial_update': CashTokenSerializer,
-        'retrieve': TokenSerializer
+        'retrieve': MainTokenSerializer
     }
 
     def create(self, request, *args, **kwargs):
         serializer = self.get_serializer(data=request.data)
         serializer.is_valid(raise_exception=True)            
         serializer.validated_data['owner'] = get_or_create_owner(request.META.get(settings.AUTH_HEADER))
         self.perform_create(serializer)
```

### Comparing `django-bcmr-0.1.8/setup.cfg` & `django-bcmr-0.1.9/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-bcmr
-version = 0.1.8
+version = 0.1.9
 description = A Django app for storing, accessing and managing CashToken Bitcoin Cash Metadata Registries
 long_description = file: README.rst
 url = https://github.com/paytaca/django-bcmr
 author = Paytaca
 author_email = info@paytaca.com
 license = BSD-3-Clause
 classifiers =
```

### Comparing `django-bcmr-0.1.8/README.rst` & `django-bcmr-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/django_bcmr.egg-info/PKG-INFO` & `django-bcmr-0.1.9/django_bcmr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-bcmr
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Django app for storing, accessing and managing CashToken Bitcoin Cash Metadata Registries
 Home-page: https://github.com/paytaca/django-bcmr
 Author: Paytaca
 Author-email: info@paytaca.com
 License: BSD-3-Clause
 Description: =====
         BCMR
```

### Comparing `django-bcmr-0.1.8/django_bcmr.egg-info/SOURCES.txt` & `django-bcmr-0.1.9/django_bcmr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/LICENSE` & `django-bcmr-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/django-bcmr/urls.py` & `django-bcmr-0.1.9/django-bcmr/urls.py`

 * *Files identical despite different names*

### Comparing `django-bcmr-0.1.8/django-bcmr/settings.py` & `django-bcmr-0.1.9/django-bcmr/settings.py`

 * *Files identical despite different names*

