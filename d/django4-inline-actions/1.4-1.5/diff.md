# Comparing `tmp/django4-inline-actions-1.4.tar.gz` & `tmp/django4-inline-actions-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django4-inline-actions-1.4.tar", last modified: Wed Apr 12 16:27:38 2023, max compression
+gzip compressed data, was "django4-inline-actions-1.5.tar", last modified: Mon May  8 22:58:39 2023, max compression
```

## Comparing `django4-inline-actions-1.4.tar` & `django4-inline-actions-1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 16:27:38.679001 django4-inline-actions-1.4/
--rw-rw-rw-   0        0        0     1537 2022-10-31 14:36:03.000000 django4-inline-actions-1.4/LICENSE
--rw-rw-rw-   0        0        0    14653 2023-04-12 16:27:38.679001 django4-inline-actions-1.4/PKG-INFO
--rw-rw-rw-   0        0        0    13204 2022-10-31 15:20:55.000000 django4-inline-actions-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 16:27:38.630183 django4-inline-actions-1.4/django4_inline_actions.egg-info/
--rw-rw-rw-   0        0        0    14653 2023-04-12 16:27:38.000000 django4-inline-actions-1.4/django4_inline_actions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2023-04-12 16:27:38.000000 django4-inline-actions-1.4/django4_inline_actions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 16:27:38.000000 django4-inline-actions-1.4/django4_inline_actions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-31 14:48:55.000000 django4-inline-actions-1.4/django4_inline_actions.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-04-12 16:27:38.000000 django4-inline-actions-1.4/django4_inline_actions.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 16:27:38.636183 django4-inline-actions-1.4/inline_actions/
--rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.4/inline_actions/__init__.py
--rw-rw-rw-   0        0        0     1425 2022-10-31 12:02:27.000000 django4-inline-actions-1.4/inline_actions/actions.py
--rw-rw-rw-   0        0        0    10489 2022-10-31 12:02:27.000000 django4-inline-actions-1.4/inline_actions/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:27:38.640795 django4-inline-actions-1.4/inline_actions/templatetags/
--rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.4/inline_actions/templatetags/__init__.py
--rw-rw-rw-   0        0        0      810 2022-10-31 12:02:27.000000 django4-inline-actions-1.4/inline_actions/templatetags/inline_action_tags.py
--rw-rw-rw-   0        0        0     2119 2023-04-12 16:27:31.000000 django4-inline-actions-1.4/pyproject.toml
--rw-rw-rw-   0        0        0      829 2023-04-12 16:27:38.682999 django4-inline-actions-1.4/setup.cfg
--rw-rw-rw-   0        0        0     2003 2023-04-12 16:27:35.000000 django4-inline-actions-1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:27:38.600043 django4-inline-actions-1.4/test_proj/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:27:38.653819 django4-inline-actions-1.4/test_proj/blog/
--rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.4/test_proj/blog/__init__.py
--rw-rw-rw-   0        0        0     4480 2022-10-31 14:58:21.000000 django4-inline-actions-1.4/test_proj/blog/admin.py
--rw-rw-rw-   0        0        0      164 2022-10-31 12:02:27.000000 django4-inline-actions-1.4/test_proj/blog/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:27:38.658817 django4-inline-actions-1.4/test_proj/blog/migrations/
--rw-rw-rw-   0        0        0     1652 2022-10-31 12:02:27.000000 django4-inline-actions-1.4/test_proj/blog/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.4/test_proj/blog/migrations/__init__.py
--rw-rw-rw-   0        0        0      783 2022-10-31 12:02:27.000000 django4-inline-actions-1.4/test_proj/blog/models.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:27:38.675997 django4-inline-actions-1.4/test_proj/blog/tests/
--rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.4/test_proj/blog/tests/__init__.py
--rw-rw-rw-   0        0        0     8292 2022-10-31 14:58:23.000000 django4-inline-actions-1.4/test_proj/blog/tests/test_admin.py
--rw-rw-rw-   0        0        0     1023 2022-10-31 12:02:27.000000 django4-inline-actions-1.4/test_proj/blog/tests/test_form.py
--rw-rw-rw-   0        0        0     7975 2022-10-31 14:58:23.000000 django4-inline-actions-1.4/test_proj/blog/tests/test_inline_admin.py
--rw-rw-rw-   0        0        0     5669 2022-10-31 14:58:24.000000 django4-inline-actions-1.4/test_proj/blog/tests/test_model_admin.py
--rw-rw-rw-   0        0        0     1345 2022-10-31 14:58:25.000000 django4-inline-actions-1.4/test_proj/blog/tests/test_templatetags.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:58:39.935240 django4-inline-actions-1.5/
+-rw-rw-rw-   0        0        0     1537 2022-10-31 14:36:03.000000 django4-inline-actions-1.5/LICENSE
+-rw-rw-rw-   0        0        0    14653 2023-05-08 22:58:39.935240 django4-inline-actions-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    13204 2022-10-31 15:20:55.000000 django4-inline-actions-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 22:58:39.885269 django4-inline-actions-1.5/django4_inline_actions.egg-info/
+-rw-rw-rw-   0        0        0    14653 2023-05-08 22:58:39.000000 django4-inline-actions-1.5/django4_inline_actions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2023-05-08 22:58:39.000000 django4-inline-actions-1.5/django4_inline_actions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 22:58:39.000000 django4-inline-actions-1.5/django4_inline_actions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-10-31 14:48:55.000000 django4-inline-actions-1.5/django4_inline_actions.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-05-08 22:58:39.000000 django4-inline-actions-1.5/django4_inline_actions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 22:58:39.891270 django4-inline-actions-1.5/inline_actions/
+-rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.5/inline_actions/__init__.py
+-rw-rw-rw-   0        0        0     1425 2022-10-31 12:02:27.000000 django4-inline-actions-1.5/inline_actions/actions.py
+-rw-rw-rw-   0        0        0    10501 2023-05-08 22:54:38.000000 django4-inline-actions-1.5/inline_actions/admin.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:58:39.895278 django4-inline-actions-1.5/inline_actions/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.5/inline_actions/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      810 2022-10-31 12:02:27.000000 django4-inline-actions-1.5/inline_actions/templatetags/inline_action_tags.py
+-rw-rw-rw-   0        0        0     2119 2023-05-08 22:55:38.000000 django4-inline-actions-1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      829 2023-05-08 22:58:39.939241 django4-inline-actions-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2003 2023-05-08 22:55:37.000000 django4-inline-actions-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:58:39.858268 django4-inline-actions-1.5/test_proj/
+drwxrwxrwx   0        0        0        0 2023-05-08 22:58:39.909789 django4-inline-actions-1.5/test_proj/blog/
+-rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.5/test_proj/blog/__init__.py
+-rw-rw-rw-   0        0        0     4480 2022-10-31 14:58:21.000000 django4-inline-actions-1.5/test_proj/blog/admin.py
+-rw-rw-rw-   0        0        0      164 2022-10-31 12:02:27.000000 django4-inline-actions-1.5/test_proj/blog/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:58:39.914789 django4-inline-actions-1.5/test_proj/blog/migrations/
+-rw-rw-rw-   0        0        0     1652 2022-10-31 12:02:27.000000 django4-inline-actions-1.5/test_proj/blog/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.5/test_proj/blog/migrations/__init__.py
+-rw-rw-rw-   0        0        0      783 2022-10-31 12:02:27.000000 django4-inline-actions-1.5/test_proj/blog/models.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:58:39.932061 django4-inline-actions-1.5/test_proj/blog/tests/
+-rw-rw-rw-   0        0        0        0 2022-10-31 12:02:27.000000 django4-inline-actions-1.5/test_proj/blog/tests/__init__.py
+-rw-rw-rw-   0        0        0     8292 2022-10-31 14:58:23.000000 django4-inline-actions-1.5/test_proj/blog/tests/test_admin.py
+-rw-rw-rw-   0        0        0     1023 2022-10-31 12:02:27.000000 django4-inline-actions-1.5/test_proj/blog/tests/test_form.py
+-rw-rw-rw-   0        0        0     7975 2022-10-31 14:58:23.000000 django4-inline-actions-1.5/test_proj/blog/tests/test_inline_admin.py
+-rw-rw-rw-   0        0        0     5669 2022-10-31 14:58:24.000000 django4-inline-actions-1.5/test_proj/blog/tests/test_model_admin.py
+-rw-rw-rw-   0        0        0     1345 2022-10-31 14:58:25.000000 django4-inline-actions-1.5/test_proj/blog/tests/test_templatetags.py
```

### Comparing `django4-inline-actions-1.4/LICENSE` & `django4-inline-actions-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.4/PKG-INFO` & `django4-inline-actions-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django4-inline-actions
-Version: 1.4
+Version: 1.5
 Summary: django4-inline-actions adds actions to each row of the ModelAdmin or InlineModelAdmin
 Home-page: https://github.com/HiroshiFuu/django4-inline-actions
 Download-URL: https://pypi.python.org/pypi/django4-inline-actions
 Author: FENG Hao
 Author-email: hiroshifuu@outlook.com
 License: BSD
 Keywords: ModelAdmin inline actions
```

### Comparing `django4-inline-actions-1.4/README.md` & `django4-inline-actions-1.5/README.md`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.4/django4_inline_actions.egg-info/PKG-INFO` & `django4-inline-actions-1.5/django4_inline_actions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django4-inline-actions
-Version: 1.4
+Version: 1.5
 Summary: django4-inline-actions adds actions to each row of the ModelAdmin or InlineModelAdmin
 Home-page: https://github.com/HiroshiFuu/django4-inline-actions
 Download-URL: https://pypi.python.org/pypi/django4-inline-actions
 Author: FENG Hao
 Author-email: hiroshifuu@outlook.com
 License: BSD
 Keywords: ModelAdmin inline actions
```

### Comparing `django4-inline-actions-1.4/django4_inline_actions.egg-info/SOURCES.txt` & `django4-inline-actions-1.5/django4_inline_actions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.4/inline_actions/actions.py` & `django4-inline-actions-1.5/inline_actions/actions.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.4/inline_actions/admin.py` & `django4-inline-actions-1.5/inline_actions/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,21 +128,21 @@
         )
 
     render_inline_actions.short_description = _("Actions")  # type: ignore
     render_inline_actions.allow_tags = True  # type: ignore
 
 
 class InlineActionsMixin(BaseInlineActionsMixin):
-    def render_inline_actions(self, obj=None):
-        html = super().render_inline_actions(obj=obj)
-        # we have to add <p> tags as a workaround for invalid html
-        return mark_safe('</p>{}<p>'.format(html))
+    # def render_inline_actions(self, obj=None):
+    #     html = super().render_inline_actions(obj=obj)
+    #     # we have to add <p> tags as a workaround for invalid html
+    #     return mark_safe('</p>{}<p>'.format(html))
 
-    render_inline_actions.short_description = _("Actions")  # type: ignore
-    render_inline_actions.allow_tags = True  # type: ignore
+    # render_inline_actions.short_description = _("Actions")  # type: ignore
+    # render_inline_actions.allow_tags = True  # type: ignore
 
     def get_fields(self, request, obj=None):
         # store `request` for `get_inline_actions`
         self._request = request
 
         fields = super().get_fields(request, obj)
         if self.inline_actions is not None:  # is it explicitly disabled?
```

### Comparing `django4-inline-actions-1.4/inline_actions/templatetags/inline_action_tags.py` & `django4-inline-actions-1.5/inline_actions/templatetags/inline_action_tags.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.4/pyproject.toml` & `django4-inline-actions-1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django4-inline-actions"
-version = "1.4"
+version = "1.5"
 description = "django4-inline-actions adds actions to each row of the ModelAdmin or InlineModelAdmin."
 authors = [
     "Alexander Frenzel <alex@relatedworks.com>",
     "FENG Hao <hiroshifuu@outlook.com>",
 ]
 
 license = "BSD-3-Clause"
```

### Comparing `django4-inline-actions-1.4/setup.cfg` & `django4-inline-actions-1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.4/setup.py` & `django4-inline-actions-1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     REQUIRES.append('django')
 
 if sys.version_info < (3, 8):
     REQUIRES.append('python >= 3.8')
 
 
 setup(name='django4-inline-actions',
-      version=1.4,
+      version=1.5,
       description='django4-inline-actions adds actions to each row of the ModelAdmin or InlineModelAdmin',
       long_description_content_type='text/markdown',
       long_description=long_description,
       author='FENG Hao',
       author_email='hiroshifuu@outlook.com',
       url='https://github.com/HiroshiFuu/django4-inline-actions',
       download_url='https://pypi.python.org/pypi/django4-inline-actions',
```

### Comparing `django4-inline-actions-1.4/test_proj/blog/admin.py` & `django4-inline-actions-1.5/test_proj/blog/admin.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.4/test_proj/blog/migrations/0001_initial.py` & `django4-inline-actions-1.5/test_proj/blog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.4/test_proj/blog/models.py` & `django4-inline-actions-1.5/test_proj/blog/models.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.4/test_proj/blog/tests/test_admin.py` & `django4-inline-actions-1.5/test_proj/blog/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.4/test_proj/blog/tests/test_form.py` & `django4-inline-actions-1.5/test_proj/blog/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.4/test_proj/blog/tests/test_inline_admin.py` & `django4-inline-actions-1.5/test_proj/blog/tests/test_inline_admin.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.4/test_proj/blog/tests/test_model_admin.py` & `django4-inline-actions-1.5/test_proj/blog/tests/test_model_admin.py`

 * *Files identical despite different names*

### Comparing `django4-inline-actions-1.4/test_proj/blog/tests/test_templatetags.py` & `django4-inline-actions-1.5/test_proj/blog/tests/test_templatetags.py`

 * *Files identical despite different names*

