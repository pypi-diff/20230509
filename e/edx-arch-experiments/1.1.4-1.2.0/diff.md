# Comparing `tmp/edx-arch-experiments-1.1.4.tar.gz` & `tmp/edx-arch-experiments-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-arch-experiments-1.1.4.tar", last modified: Thu Apr 13 19:43:37 2023, max compression
+gzip compressed data, was "edx-arch-experiments-1.2.0.tar", last modified: Tue May  9 16:31:34 2023, max compression
```

## Comparing `edx-arch-experiments-1.1.4.tar` & `edx-arch-experiments-1.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 19:43:37.497963 edx-arch-experiments-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6626 2023-04-13 19:43:37.497963 edx-arch-experiments-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4463 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 19:43:37.493963 edx-arch-experiments-1.1.4/edx_arch_experiments/
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/edx_arch_experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/edx_arch_experiments/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 19:43:37.497963 edx-arch-experiments-1.1.4/edx_arch_experiments/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/edx_arch_experiments/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/edx_arch_experiments/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/edx_arch_experiments/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 19:43:37.497963 edx-arch-experiments-1.1.4/edx_arch_experiments/summaryhook_aside/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/edx_arch_experiments/summaryhook_aside/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/edx_arch_experiments/summaryhook_aside/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2861 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/edx_arch_experiments/summaryhook_aside/block.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 19:43:37.497963 edx-arch-experiments-1.1.4/edx_arch_experiments/summaryhook_aside/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/edx_arch_experiments/summaryhook_aside/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      553 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/edx_arch_experiments/summaryhook_aside/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/edx_arch_experiments/summaryhook_aside/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/edx_arch_experiments/summaryhook_aside/waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 19:43:37.497963 edx-arch-experiments-1.1.4/edx_arch_experiments/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/edx_arch_experiments/tests/test_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 19:43:37.497963 edx-arch-experiments-1.1.4/edx_arch_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6626 2023-04-13 19:43:37.000000 edx-arch-experiments-1.1.4/edx_arch_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-04-13 19:43:37.000000 edx-arch-experiments-1.1.4/edx_arch_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 19:43:37.000000 edx-arch-experiments-1.1.4/edx_arch_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-04-13 19:43:37.000000 edx-arch-experiments-1.1.4/edx_arch_experiments.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 19:43:37.000000 edx-arch-experiments-1.1.4/edx_arch_experiments.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-13 19:43:37.000000 edx-arch-experiments-1.1.4/edx_arch_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-13 19:43:37.000000 edx-arch-experiments-1.1.4/edx_arch_experiments.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 19:43:37.497963 edx-arch-experiments-1.1.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-04-13 19:43:37.497963 edx-arch-experiments-1.1.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5475 2023-04-13 19:43:34.000000 edx-arch-experiments-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1573 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6769 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4463 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.781480 edx-arch-experiments-1.2.0/edx_arch_experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/edx_arch_experiments/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/settings/production.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/block.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      553 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/waffle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/edx_arch_experiments/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/edx_arch_experiments/tests/test_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6769 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-09 16:31:34.000000 edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-09 16:31:34.785480 edx-arch-experiments-1.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5475 2023-05-09 16:31:30.000000 edx-arch-experiments-1.2.0/setup.py
```

### Comparing `edx-arch-experiments-1.1.4/CHANGELOG.rst` & `edx-arch-experiments-1.2.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 *
 
+[1.2.0] - 2023-05-08
+~~~~~~~~~~~~~~~~~~~~
+
+* Update summary hook to trigger on videos
+* Remove text selection data key from summary hook html
+
 [1.1.4] - 2023-04-14
 ~~~~~~~~~~~~~~~~~~~~
 
 * Add course and block ID to summary hook html
 
 [1.1.3] - 2023-04-05
 ~~~~~~~~~~~~~~~~~~~~
```

### Comparing `edx-arch-experiments-1.1.4/LICENSE.txt` & `edx-arch-experiments-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-arch-experiments-1.1.4/PKG-INFO` & `edx-arch-experiments-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-arch-experiments
-Version: 1.1.4
+Version: 1.2.0
 Summary: A plugin to include applications under development by the architecture team at edx
 Home-page: https://github.com/edx/edx-arch-experiments
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -160,14 +160,20 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 *
 
+[1.2.0] - 2023-05-08
+~~~~~~~~~~~~~~~~~~~~
+
+* Update summary hook to trigger on videos
+* Remove text selection data key from summary hook html
+
 [1.1.4] - 2023-04-14
 ~~~~~~~~~~~~~~~~~~~~
 
 * Add course and block ID to summary hook html
 
 [1.1.3] - 2023-04-05
 ~~~~~~~~~~~~~~~~~~~~
```

### Comparing `edx-arch-experiments-1.1.4/README.rst` & `edx-arch-experiments-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-arch-experiments-1.1.4/edx_arch_experiments/apps.py` & `edx-arch-experiments-1.2.0/edx_arch_experiments/apps.py`

 * *Files identical despite different names*

### Comparing `edx-arch-experiments-1.1.4/edx_arch_experiments/summaryhook_aside/apps.py` & `edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/apps.py`

 * *Files identical despite different names*

### Comparing `edx-arch-experiments-1.1.4/edx_arch_experiments/summaryhook_aside/block.py` & `edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/block.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 summary_fragment = """
 <div>&nbsp;</div>
 <div class="summary-hook">
   <div summary-launch>
     <div id="launch-summary-button"
       data-url-api="{{data_url_api}}"
-      data-text-identifier="{{data_text_identifier}}"
       data-course-id="{{data_course_id}}"
       data-content-id="{{data_content_id}}"
     >
     </div>
   </div>
   <div id="ai-spot-root"></div>
   <script type="text/javascript" src="{{js_url}}" defer="defer"></script>
@@ -33,21 +32,24 @@
 def _children_have_summarizable_content(block):
     """
     Only if a unit contains HTML blocks with sufficient text in them
     is it worth injecting the summarizer.
     """
     children = block.get_children()
     for child in children:
+        category = getattr(child, 'category', None)
         if (
-                getattr(child, 'category', None) == 'html'
+                category == 'html'
                 and hasattr(child, 'get_html')
                 and len(child.get_html()) > settings.SUMMARY_HOOK_MIN_SIZE
         ):
             return True
-
+        # we will eventually require there to be transcripts available to trigger but not yet
+        if category == 'video':
+            return True
     return False
 
 
 class SummaryHookAside(XBlockAside):
     """
     XBlock aside that injects AI summary javascript
     """
@@ -62,15 +64,14 @@
         if not _children_have_summarizable_content(block):
             return fragment
 
         fragment.add_content(
             _render_summary(
                 {
                     'data_url_api': settings.SUMMARY_HOOK_HOST,
-                    'data_text_identifier': '.xblock-student_view-html',
                     'data_course_id': block.scope_ids.usage_id.course_key,
                     'data_content_id': block.scope_ids.usage_id,
                     'js_url': settings.SUMMARY_HOOK_HOST + settings.SUMMARY_HOOK_JS_PATH,
                 }
             )
         )
         return fragment
```

### Comparing `edx-arch-experiments-1.1.4/edx_arch_experiments/summaryhook_aside/settings/devstack.py` & `edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/settings/devstack.py`

 * *Files identical despite different names*

### Comparing `edx-arch-experiments-1.1.4/edx_arch_experiments/summaryhook_aside/waffle.py` & `edx-arch-experiments-1.2.0/edx_arch_experiments/summaryhook_aside/waffle.py`

 * *Files identical despite different names*

### Comparing `edx-arch-experiments-1.1.4/edx_arch_experiments.egg-info/PKG-INFO` & `edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-arch-experiments
-Version: 1.1.4
+Version: 1.2.0
 Summary: A plugin to include applications under development by the architecture team at edx
 Home-page: https://github.com/edx/edx-arch-experiments
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -160,14 +160,20 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 *
 
+[1.2.0] - 2023-05-08
+~~~~~~~~~~~~~~~~~~~~
+
+* Update summary hook to trigger on videos
+* Remove text selection data key from summary hook html
+
 [1.1.4] - 2023-04-14
 ~~~~~~~~~~~~~~~~~~~~
 
 * Add course and block ID to summary hook html
 
 [1.1.3] - 2023-04-05
 ~~~~~~~~~~~~~~~~~~~~
```

### Comparing `edx-arch-experiments-1.1.4/edx_arch_experiments.egg-info/SOURCES.txt` & `edx-arch-experiments-1.2.0/edx_arch_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-arch-experiments-1.1.4/requirements/constraints.txt` & `edx-arch-experiments-1.2.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-arch-experiments-1.1.4/setup.py` & `edx-arch-experiments-1.2.0/setup.py`

 * *Files identical despite different names*

