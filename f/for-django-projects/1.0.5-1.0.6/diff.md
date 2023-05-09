# Comparing `tmp/for-django-projects-1.0.5.tar.gz` & `tmp/for-django-projects-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "for-django-projects-1.0.5.tar", last modified: Fri May  5 17:08:50 2023, max compression
+gzip compressed data, was "for-django-projects-1.0.6.tar", last modified: Tue May  9 21:04:24 2023, max compression
```

## Comparing `for-django-projects-1.0.5.tar` & `for-django-projects-1.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 17:08:50.128993 for-django-projects-1.0.5/
--rw-rw-rw-   0        0        0     3510 2023-05-05 17:08:50.128993 for-django-projects-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3037 2023-05-05 15:27:24.000000 for-django-projects-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 17:08:49.968339 for-django-projects-1.0.5/for_django_projects/
--rw-rw-rw-   0        0        0        0 2023-05-04 17:11:49.000000 for-django-projects-1.0.5/for_django_projects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:08:49.998381 for-django-projects-1.0.5/for_django_projects/alertas/
--rw-rw-rw-   0        0        0     1152 2022-11-22 19:35:13.000000 for-django-projects-1.0.5/for_django_projects/alertas/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:08:50.038583 for-django-projects-1.0.5/for_django_projects/form_utils/
--rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/form_utils/__init__.py
--rw-rw-rw-   0        0        0      511 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/form_utils/admin.py
--rw-rw-rw-   0        0        0     2457 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/form_utils/fields.py
--rw-rw-rw-   0        0        0    10772 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/form_utils/forms.py
--rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/form_utils/models.py
--rw-rw-rw-   0        0        0      375 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/form_utils/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:08:50.048590 for-django-projects-1.0.5/for_django_projects/form_utils/templatetags/
--rw-rw-rw-   0        0        0      118 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/form_utils/templatetags/__init__.py
--rw-rw-rw-   0        0        0     3499 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/form_utils/templatetags/form_utils.py
--rw-rw-rw-   0        0        0      555 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/form_utils/utils.py
--rw-rw-rw-   0        0        0     4405 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/form_utils/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:08:50.078542 for-django-projects-1.0.5/for_django_projects/pwa/
--rw-rw-rw-   0        0        0       41 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/pwa/__init__.py
--rw-rw-rw-   0        0        0     4617 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/pwa/app_settings.py
--rw-rw-rw-   0        0        0       86 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/pwa/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:08:50.088591 for-django-projects-1.0.5/for_django_projects/pwa/templatetags/
--rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/pwa/templatetags/__init__.py
--rw-rw-rw-   0        0        0      732 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/pwa/templatetags/pwa.py
--rw-rw-rw-   0        0        0      358 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/pwa/urls.py
--rw-rw-rw-   0        0        0      616 2022-07-11 17:53:14.000000 for-django-projects-1.0.5/for_django_projects/pwa/views.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:08:50.123425 for-django-projects-1.0.5/for_django_projects/utils/
--rw-rw-rw-   0        0        0        0 2023-05-03 20:33:09.000000 for-django-projects-1.0.5/for_django_projects/utils/__init__.py
--rw-rw-rw-   0        0        0    24678 2023-05-05 17:03:01.000000 for-django-projects-1.0.5/for_django_projects/utils/custom_models.py
--rw-rw-rw-   0        0        0     3071 2023-05-04 18:02:08.000000 for-django-projects-1.0.5/for_django_projects/utils/decoradores.py
--rw-rw-rw-   0        0        0    18629 2023-05-04 17:23:25.000000 for-django-projects-1.0.5/for_django_projects/utils/funciones.py
--rw-rw-rw-   0        0        0     4732 2023-05-04 14:32:38.000000 for-django-projects-1.0.5/for_django_projects/utils/funciones_adicionales.py
--rw-rw-rw-   0        0        0     3137 2023-05-04 17:23:25.000000 for-django-projects-1.0.5/for_django_projects/utils/models_utils.py
--rw-rw-rw-   0        0        0     4058 2023-05-02 21:53:32.000000 for-django-projects-1.0.5/for_django_projects/utils/validadores.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:08:49.988384 for-django-projects-1.0.5/for_django_projects.egg-info/
--rw-rw-rw-   0        0        0     3510 2023-05-05 17:08:49.000000 for-django-projects-1.0.5/for_django_projects.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1309 2023-05-05 17:08:49.000000 for-django-projects-1.0.5/for_django_projects.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 17:08:49.000000 for-django-projects-1.0.5/for_django_projects.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-05-05 17:08:49.000000 for-django-projects-1.0.5/for_django_projects.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-05 17:08:49.000000 for-django-projects-1.0.5/for_django_projects.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 17:08:50.128993 for-django-projects-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-05-05 17:08:45.000000 for-django-projects-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:04:24.753992 for-django-projects-1.0.6/
+-rw-rw-rw-   0        0        0     5297 2023-05-09 21:04:24.753992 for-django-projects-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4824 2023-05-09 16:23:57.000000 for-django-projects-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 21:04:24.583492 for-django-projects-1.0.6/for_django_projects/
+-rw-rw-rw-   0        0        0        0 2023-05-04 17:11:49.000000 for-django-projects-1.0.6/for_django_projects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:04:24.613509 for-django-projects-1.0.6/for_django_projects/alertas/
+-rw-rw-rw-   0        0        0     1152 2022-11-22 19:35:13.000000 for-django-projects-1.0.6/for_django_projects/alertas/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:04:24.663500 for-django-projects-1.0.6/for_django_projects/form_utils/
+-rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/form_utils/__init__.py
+-rw-rw-rw-   0        0        0      511 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/form_utils/admin.py
+-rw-rw-rw-   0        0        0     2457 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/form_utils/fields.py
+-rw-rw-rw-   0        0        0    10772 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/form_utils/forms.py
+-rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/form_utils/models.py
+-rw-rw-rw-   0        0        0      375 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/form_utils/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:04:24.681525 for-django-projects-1.0.6/for_django_projects/form_utils/templatetags/
+-rw-rw-rw-   0        0        0      118 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/form_utils/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     3499 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/form_utils/templatetags/form_utils.py
+-rw-rw-rw-   0        0        0      555 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/form_utils/utils.py
+-rw-rw-rw-   0        0        0     4405 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/form_utils/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:04:24.718465 for-django-projects-1.0.6/for_django_projects/pwa/
+-rw-rw-rw-   0        0        0       41 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/pwa/__init__.py
+-rw-rw-rw-   0        0        0     4617 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/pwa/app_settings.py
+-rw-rw-rw-   0        0        0       86 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/pwa/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:04:24.723976 for-django-projects-1.0.6/for_django_projects/pwa/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/pwa/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      732 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/pwa/templatetags/pwa.py
+-rw-rw-rw-   0        0        0      358 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/pwa/urls.py
+-rw-rw-rw-   0        0        0      616 2022-07-11 17:53:14.000000 for-django-projects-1.0.6/for_django_projects/pwa/views.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:04:24.743991 for-django-projects-1.0.6/for_django_projects/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-03 20:33:09.000000 for-django-projects-1.0.6/for_django_projects/utils/__init__.py
+-rw-rw-rw-   0        0        0    24682 2023-05-09 16:16:42.000000 for-django-projects-1.0.6/for_django_projects/utils/custom_models.py
+-rw-rw-rw-   0        0        0     3079 2023-05-09 16:16:42.000000 for-django-projects-1.0.6/for_django_projects/utils/decoradores.py
+-rw-rw-rw-   0        0        0    18629 2023-05-04 17:23:25.000000 for-django-projects-1.0.6/for_django_projects/utils/funciones.py
+-rw-rw-rw-   0        0        0     4732 2023-05-04 14:32:38.000000 for-django-projects-1.0.6/for_django_projects/utils/funciones_adicionales.py
+-rw-rw-rw-   0        0        0     3137 2023-05-04 17:23:25.000000 for-django-projects-1.0.6/for_django_projects/utils/models_utils.py
+-rw-rw-rw-   0        0        0     3898 2023-05-09 16:13:29.000000 for-django-projects-1.0.6/for_django_projects/utils/validadores.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:04:24.603505 for-django-projects-1.0.6/for_django_projects.egg-info/
+-rw-rw-rw-   0        0        0     5297 2023-05-09 21:04:24.000000 for-django-projects-1.0.6/for_django_projects.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1309 2023-05-09 21:04:24.000000 for-django-projects-1.0.6/for_django_projects.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 21:04:24.000000 for-django-projects-1.0.6/for_django_projects.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-05-09 21:04:24.000000 for-django-projects-1.0.6/for_django_projects.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-09 21:04:24.000000 for-django-projects-1.0.6/for_django_projects.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 21:04:24.753992 for-django-projects-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-05-09 21:04:18.000000 for-django-projects-1.0.6/setup.py
```

### Comparing `for-django-projects-1.0.5/for_django_projects/alertas/__init__.py` & `for-django-projects-1.0.6/for_django_projects/alertas/__init__.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.5/for_django_projects/form_utils/fields.py` & `for-django-projects-1.0.6/for_django_projects/form_utils/fields.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.5/for_django_projects/form_utils/forms.py` & `for-django-projects-1.0.6/for_django_projects/form_utils/forms.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.5/for_django_projects/form_utils/templatetags/form_utils.py` & `for-django-projects-1.0.6/for_django_projects/form_utils/templatetags/form_utils.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.5/for_django_projects/form_utils/utils.py` & `for-django-projects-1.0.6/for_django_projects/form_utils/utils.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.5/for_django_projects/form_utils/widgets.py` & `for-django-projects-1.0.6/for_django_projects/form_utils/widgets.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.5/for_django_projects/pwa/app_settings.py` & `for-django-projects-1.0.6/for_django_projects/pwa/app_settings.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.5/for_django_projects/pwa/templatetags/pwa.py` & `for-django-projects-1.0.6/for_django_projects/pwa/templatetags/pwa.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.5/for_django_projects/pwa/views.py` & `for-django-projects-1.0.6/for_django_projects/pwa/views.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.5/for_django_projects/utils/custom_models.py` & `for-django-projects-1.0.6/for_django_projects/utils/custom_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     def __init__(self, searchs=None, *args, **kwargs):
         self.search_fields = searchs
         super().__init__(*args, **kwargs)
 
     def filter_queryset(self, request, term, queryset=None, **dependent_fields):
         return filter_queryset(self, request, term, queryset, **dependent_fields)
 
-class FormError(Exception):
+class FormException(Exception):
     def __init__(self, form, prefix="", sufix=""):
         super().__init__("Error en el formulario")
         alerta = ""
         if isinstance(form, list) or isinstance(form, tuple):
             self.errors = []
             for x in form:
                 for k, v in x.errors.items():
```

### Comparing `for-django-projects-1.0.5/for_django_projects/utils/decoradores.py` & `for-django-projects-1.0.6/for_django_projects/utils/decoradores.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.http import JsonResponse
 from django.shortcuts import redirect
 from django.conf import settings
 from for_django_projects.utils.funciones import redirectAfterPostGet
 
 
 def custom_atomic_request(func):
-    from for_django_projects.utils.custom_models import FormError
+    from for_django_projects.utils.custom_models import FormException
     import sys
     def validate_request(*args, **kwargs):
         res_json = []
         request = args[0]
         has_except = False
         error_message = ""
         if request.method == "POST":
@@ -23,15 +23,15 @@
             except ValueError as ex:
                 res_json.append({'error': True,
                                  "message": str(ex)
                                  })
                 val_func = JsonResponse(res_json, safe=False)
                 has_except = True
                 error_message = str(ex)
-            except FormError as ex:
+            except FormException as ex:
                 res_json.append(ex.dict_error)
                 val_func = JsonResponse(res_json, safe=False)
                 has_except = True
                 error_message = "Formulario no válido"
             except IntegrityError as ex:
                 has_except = True
                 msg = str(ex)
```

### Comparing `for-django-projects-1.0.5/for_django_projects/utils/funciones.py` & `for-django-projects-1.0.6/for_django_projects/utils/funciones.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.5/for_django_projects/utils/funciones_adicionales.py` & `for-django-projects-1.0.6/for_django_projects/utils/funciones_adicionales.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.5/for_django_projects/utils/models_utils.py` & `for-django-projects-1.0.6/for_django_projects/utils/models_utils.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.5/for_django_projects/utils/validadores.py` & `for-django-projects-1.0.6/for_django_projects/utils/validadores.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-from django.core.files.images import get_image_dimensions
-from django.core.exceptions import ValidationError
-
-#para el modelo financiero.models.Constante
-
 from django.core.exceptions import ValidationError
 from django.utils.deconstruct import deconstructible
 
 
 @deconstructible
 class FileMaxSizeInMbValidator:
     message = "Maximum file size is %(maxSize)sMB."
```

### Comparing `for-django-projects-1.0.5/for_django_projects.egg-info/SOURCES.txt` & `for-django-projects-1.0.6/for_django_projects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.5/setup.py` & `for-django-projects-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="for-django-projects",
-    version="1.0.5",
+    version="1.0.6",
     author="Jasmany Sanchez Mendez",
     author_email="jasmanysanchez97@gmail.com",
     description="Package of libraries for Django projects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jasmanysanchez/for-django-projects",
     packages=setuptools.find_packages(),
```

