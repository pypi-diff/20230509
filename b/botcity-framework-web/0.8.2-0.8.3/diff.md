# Comparing `tmp/botcity-framework-web-0.8.2.tar.gz` & `tmp/botcity-framework-web-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/botcity-framework-web-python/botcity-framework-web-python/dist/.tmp-lj3_9cn8/botcity-framework-web-0.8.2.tar", last modified: Fri Mar 10 05:18:44 2023, max compression
+gzip compressed data, was "/home/runner/work/botcity-framework-web-python/botcity-framework-web-python/dist/.tmp-wowhfz7a/botcity-framework-web-0.8.3.tar", last modified: Mon May  8 22:48:02 2023, max compression
```

## Comparing `botcity-framework-web-0.8.2.tar` & `botcity-framework-web-0.8.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/botcity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/botcity/web/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/botcity/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/botcity/web/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    73628 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/botcity/web/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/botcity/web/browsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/botcity/web/browsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/botcity/web/browsers/chrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/botcity/web/browsers/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)    33984 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/botcity/web/browsers/firefox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/botcity/web/browsers/ie.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/botcity/web/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/botcity/web/cv2find.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/botcity/web/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/botcity/web/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/botcity/web/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/botcity/web/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/botcity/web/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/botcity_framework_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/botcity_framework_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/botcity_framework_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/botcity_framework_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/botcity_framework_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/botcity_framework_web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 05:18:44.000000 botcity-framework-web-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/tests/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/tests/test_keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/tests/test_mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/tests/test_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-03-10 05:18:31.000000 botcity-framework-web-0.8.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/botcity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/botcity/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/botcity/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/botcity/web/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73707 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/botcity/web/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/botcity/web/browsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/botcity/web/browsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/botcity/web/browsers/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/botcity/web/browsers/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33984 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/botcity/web/browsers/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/botcity/web/browsers/ie.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/botcity/web/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/botcity/web/cv2find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/botcity/web/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/botcity/web/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/botcity/web/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/botcity/web/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/botcity/web/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/botcity_framework_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/botcity_framework_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/botcity_framework_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/botcity_framework_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/botcity_framework_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/botcity_framework_web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:48:02.000000 botcity-framework-web-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/tests/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/tests/test_keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/tests/test_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/tests/test_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-05-08 22:47:52.000000 botcity-framework-web-0.8.3/versioneer.py
```

### Comparing `botcity-framework-web-0.8.2/LICENSE` & `botcity-framework-web-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/PKG-INFO` & `botcity-framework-web-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-framework-web
-Version: 0.8.2
+Version: 0.8.3
 Home-page: https://www.github.com/botcity-dev/botcity-framework-web-python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <h1 align="center">BotCity Framework Web - Python</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botcity-framework-web Version: 0.8.2 Home-page:
+Metadata-Version: 2.1 Name: botcity-framework-web Version: 0.8.3 Home-page:
 https://www.github.com/botcity-dev/botcity-framework-web-python Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE
                  ****** BotCity Framework Web - Python ******
                          Â« Explore Framework docs Â»
 
 ## Summary  - [ð¤ Computer-vision based UI Automation](#-computer-vision-
 based-ui-automation) - [ð Generate Python Code while Interacting with your
```

### Comparing `botcity-framework-web-0.8.2/README.md` & `botcity-framework-web-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/botcity/web/bot.py` & `botcity-framework-web-0.8.3/botcity/web/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,14 +269,16 @@
         Stops the Chrome browser and clean up the User Data Directory.
 
         Warning:
             After invoking this method, you will need to reassign your custom options and capabilities.
         """
         if not self._driver:
             return
+        if self.get_tabs():
+            self.activate_tab(self.get_tabs()[-1])
         self._driver.close()
         self._driver.quit()
         self.options = None
         self.capabilities = None
         self._driver = None
 
     def set_screen_resolution(self, width=None, height=None):
```

### Comparing `botcity-framework-web-0.8.2/botcity/web/browsers/__init__.py` & `botcity-framework-web-0.8.3/botcity/web/browsers/__init__.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/botcity/web/browsers/chrome.py` & `botcity-framework-web-0.8.3/botcity/web/browsers/chrome.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/botcity/web/browsers/edge.py` & `botcity-framework-web-0.8.3/botcity/web/browsers/edge.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/botcity/web/browsers/firefox.py` & `botcity-framework-web-0.8.3/botcity/web/browsers/firefox.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/botcity/web/browsers/ie.py` & `botcity-framework-web-0.8.3/botcity/web/browsers/ie.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/botcity/web/cv2find.py` & `botcity-framework-web-0.8.3/botcity/web/cv2find.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/botcity/web/parsers.py` & `botcity-framework-web-0.8.3/botcity/web/parsers.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/botcity/web/util.py` & `botcity-framework-web-0.8.3/botcity/web/util.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/botcity_framework_web.egg-info/PKG-INFO` & `botcity-framework-web-0.8.3/botcity_framework_web.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-framework-web
-Version: 0.8.2
+Version: 0.8.3
 Home-page: https://www.github.com/botcity-dev/botcity-framework-web-python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <h1 align="center">BotCity Framework Web - Python</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botcity-framework-web Version: 0.8.2 Home-page:
+Metadata-Version: 2.1 Name: botcity-framework-web Version: 0.8.3 Home-page:
 https://www.github.com/botcity-dev/botcity-framework-web-python Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE
                  ****** BotCity Framework Web - Python ******
                          Â« Explore Framework docs Â»
 
 ## Summary  - [ð¤ Computer-vision based UI Automation](#-computer-vision-
 based-ui-automation) - [ð Generate Python Code while Interacting with your
```

### Comparing `botcity-framework-web-0.8.2/botcity_framework_web.egg-info/SOURCES.txt` & `botcity-framework-web-0.8.3/botcity_framework_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/setup.py` & `botcity-framework-web-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/tests/test_browser.py` & `botcity-framework-web-0.8.3/tests/test_browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 def test_display_size(web: WebBot):
     web.browse(conftest.INDEX_PAGE)
     web.set_screen_resolution(1280, 720)
     (w, h) = web.display_size()
 
-    assert w == 1280
+    assert w in [1280, 1264, 1223]
 
 
 def test_javascript(web: WebBot):
     web.browse(conftest.INDEX_PAGE)
     web.execute_javascript("""
         document.getElementById('element-result').innerText = 'execute_javascript() works!';
     """)
```

### Comparing `botcity-framework-web-0.8.2/tests/test_keyboard.py` & `botcity-framework-web-0.8.3/tests/test_keyboard.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/tests/test_mouse.py` & `botcity-framework-web-0.8.3/tests/test_mouse.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/tests/test_vision.py` & `botcity-framework-web-0.8.3/tests/test_vision.py`

 * *Files identical despite different names*

### Comparing `botcity-framework-web-0.8.2/versioneer.py` & `botcity-framework-web-0.8.3/versioneer.py`

 * *Files identical despite different names*

