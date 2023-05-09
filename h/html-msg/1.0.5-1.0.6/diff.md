# Comparing `tmp/html_msg-1.0.5.tar.gz` & `tmp/html_msg-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_msg-1.0.5.tar", last modified: Tue May  9 19:31:34 2023, max compression
+gzip compressed data, was "html_msg-1.0.6.tar", last modified: Tue May  9 19:48:37 2023, max compression
```

## Comparing `html_msg-1.0.5.tar` & `html_msg-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 19:31:34.591179 html_msg-1.0.5/
--rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     3935 2023-05-09 19:31:34.591179 html_msg-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3383 2023-05-09 19:29:44.000000 html_msg-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 19:31:34.577205 html_msg-1.0.5/html_msg/
--rw-rw-rw-   0        0        0      115 2023-05-09 18:14:42.000000 html_msg-1.0.5/html_msg/__init__.py
--rw-rw-rw-   0        0        0    12111 2023-05-09 17:31:43.000000 html_msg-1.0.5/html_msg/html_message.py
--rw-rw-rw-   0        0        0    14517 2023-05-09 19:00:47.000000 html_msg-1.0.5/html_msg/html_table.py
-drwxrwxrwx   0        0        0        0 2023-05-09 19:31:34.590372 html_msg-1.0.5/html_msg.egg-info/
--rw-rw-rw-   0        0        0     3935 2023-05-09 19:31:34.000000 html_msg-1.0.5/html_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-09 19:31:34.000000 html_msg-1.0.5/html_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 19:31:34.000000 html_msg-1.0.5/html_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-09 19:31:34.000000 html_msg-1.0.5/html_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-09 19:31:34.000000 html_msg-1.0.5/html_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 19:31:34.591179 html_msg-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      796 2023-05-09 19:30:38.000000 html_msg-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:48:37.768655 html_msg-1.0.6/
+-rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     3963 2023-05-09 19:48:37.767658 html_msg-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3383 2023-05-09 19:29:44.000000 html_msg-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 19:48:37.756013 html_msg-1.0.6/html_msg/
+-rw-rw-rw-   0        0        0      115 2023-05-09 19:47:47.000000 html_msg-1.0.6/html_msg/__init__.py
+-rw-rw-rw-   0        0        0    12111 2023-05-09 17:31:43.000000 html_msg-1.0.6/html_msg/html_message.py
+-rw-rw-rw-   0        0        0    14517 2023-05-09 19:00:47.000000 html_msg-1.0.6/html_msg/html_table.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:48:37.767658 html_msg-1.0.6/html_msg.egg-info/
+-rw-rw-rw-   0        0        0     3963 2023-05-09 19:48:37.000000 html_msg-1.0.6/html_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-09 19:48:37.000000 html_msg-1.0.6/html_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 19:48:37.000000 html_msg-1.0.6/html_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-09 19:48:37.000000 html_msg-1.0.6/html_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 19:48:37.000000 html_msg-1.0.6/html_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 19:48:37.768655 html_msg-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      824 2023-05-09 19:47:55.000000 html_msg-1.0.6/setup.py
```

### Comparing `html_msg-1.0.5/LICENSE.txt` & `html_msg-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.5/PKG-INFO` & `html_msg-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: html_msg
-Version: 1.0.5
+Version: 1.0.6
 Summary: This tool allows to create HTML message via simple methods,      without the need to write HTML code manually.
-Home-page: https://github.com/
-Download-URL: https://pypi.org/project/
+Home-page: https://github.com/Sirakan-B/html_msg/
+Download-URL: https://pypi.org/project/html-msg/
 Author: Sirakan Bagdasarian
 Author-email: bsirak@bk.ru
 License: MIT
 Keywords: HTML,Message
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `html_msg-1.0.5/README.md` & `html_msg-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.5/html_msg/html_message.py` & `html_msg-1.0.6/html_msg/html_message.py`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.5/html_msg/html_table.py` & `html_msg-1.0.6/html_msg/html_table.py`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.5/html_msg.egg-info/PKG-INFO` & `html_msg-1.0.6/html_msg.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: html-msg
-Version: 1.0.5
+Version: 1.0.6
 Summary: This tool allows to create HTML message via simple methods,      without the need to write HTML code manually.
-Home-page: https://github.com/
-Download-URL: https://pypi.org/project/
+Home-page: https://github.com/Sirakan-B/html_msg/
+Download-URL: https://pypi.org/project/html-msg/
 Author: Sirakan Bagdasarian
 Author-email: bsirak@bk.ru
 License: MIT
 Keywords: HTML,Message
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `html_msg-1.0.5/setup.py` & `html_msg-1.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 
 setup_args = dict(
     name='html_msg',
-    version='1.0.5',
+    version='1.0.6',
     description='This tool allows to create HTML message via simple methods, \
      without the need to write HTML code manually.',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n',
     license='MIT',
     packages=find_packages(),
     author='Sirakan Bagdasarian',
     author_email='bsirak@bk.ru',
     keywords=['HTML', 'Message'],
-    url='https://github.com/',
-    download_url='https://pypi.org/project/'
+    url='https://github.com/Sirakan-B/html_msg/',
+    download_url='https://pypi.org/project/html-msg/'
 )
 
 install_requires = [
     'IPython',
     'pandas'
 ]
```

