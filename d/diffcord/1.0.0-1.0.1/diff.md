# Comparing `tmp/diffcord-1.0.0.tar.gz` & `tmp/diffcord-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffcord-1.0.0.tar", last modified: Mon May  8 22:19:07 2023, max compression
+gzip compressed data, was "diffcord-1.0.1.tar", last modified: Tue May  9 00:52:34 2023, max compression
```

## Comparing `diffcord-1.0.0.tar` & `diffcord-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 22:19:07.835417 diffcord-1.0.0/
--rw-rw-rw-   0        0        0     1094 2023-03-12 19:55:56.000000 diffcord-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2607 2023-05-08 22:19:07.834416 diffcord-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-05-08 22:12:05.000000 diffcord-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 22:19:07.816443 diffcord-1.0.0/diffcord/
--rw-rw-rw-   0        0        0       86 2023-03-12 21:51:54.000000 diffcord-1.0.0/diffcord/__init__.py
--rw-rw-rw-   0        0        0     2228 2023-05-07 20:08:24.000000 diffcord-1.0.0/diffcord/api.py
--rw-rw-rw-   0        0        0     6747 2023-05-08 03:04:14.000000 diffcord-1.0.0/diffcord/client.py
--rw-rw-rw-   0        0        0     2111 2023-03-20 16:51:23.000000 diffcord-1.0.0/diffcord/error.py
--rw-rw-rw-   0        0        0     3397 2023-05-08 22:11:45.000000 diffcord-1.0.0/diffcord/vote.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:19:07.827416 diffcord-1.0.0/diffcord.egg-info/
--rw-rw-rw-   0        0        0     2607 2023-05-08 22:19:07.000000 diffcord-1.0.0/diffcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-05-08 22:19:07.000000 diffcord-1.0.0/diffcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 22:19:07.000000 diffcord-1.0.0/diffcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 22:19:07.000000 diffcord-1.0.0/diffcord.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2023-05-08 22:19:07.000000 diffcord-1.0.0/diffcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 22:19:07.000000 diffcord-1.0.0/diffcord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 22:19:07.835417 diffcord-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      727 2023-05-08 22:14:54.000000 diffcord-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:19:07.832414 diffcord-1.0.0/tests/
--rw-rw-rw-   0        0        0      108 2023-03-20 14:33:45.000000 diffcord-1.0.0/tests/test_client.py
--rw-rw-rw-   0        0        0     4232 2023-05-08 19:50:49.000000 diffcord-1.0.0/tests/test_webhook_listener.py
--rw-rw-rw-   0        0        0     2041 2023-05-08 22:12:21.000000 diffcord-1.0.0/tests/testing_main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 00:52:34.852626 diffcord-1.0.1/
+-rw-rw-rw-   0        0        0     1094 2023-03-12 19:55:56.000000 diffcord-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2607 2023-05-09 00:52:34.851624 diffcord-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-05-08 22:12:05.000000 diffcord-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 00:52:34.834626 diffcord-1.0.1/diffcord/
+-rw-rw-rw-   0        0        0       86 2023-03-12 21:51:54.000000 diffcord-1.0.1/diffcord/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-05-07 20:08:24.000000 diffcord-1.0.1/diffcord/api.py
+-rw-rw-rw-   0        0        0     6751 2023-05-09 00:50:52.000000 diffcord-1.0.1/diffcord/client.py
+-rw-rw-rw-   0        0        0     2111 2023-03-20 16:51:23.000000 diffcord-1.0.1/diffcord/error.py
+-rw-rw-rw-   0        0        0     3397 2023-05-08 22:11:45.000000 diffcord-1.0.1/diffcord/vote.py
+drwxrwxrwx   0        0        0        0 2023-05-09 00:52:34.845626 diffcord-1.0.1/diffcord.egg-info/
+-rw-rw-rw-   0        0        0     2607 2023-05-09 00:52:34.000000 diffcord-1.0.1/diffcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-05-09 00:52:34.000000 diffcord-1.0.1/diffcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 00:52:34.000000 diffcord-1.0.1/diffcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-09 00:52:34.000000 diffcord-1.0.1/diffcord.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       27 2023-05-09 00:52:34.000000 diffcord-1.0.1/diffcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 00:52:34.000000 diffcord-1.0.1/diffcord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 00:52:34.852626 diffcord-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      727 2023-05-09 00:52:33.000000 diffcord-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 00:52:34.849625 diffcord-1.0.1/tests/
+-rw-rw-rw-   0        0        0      108 2023-03-20 14:33:45.000000 diffcord-1.0.1/tests/test_client.py
+-rw-rw-rw-   0        0        0     4232 2023-05-08 19:50:49.000000 diffcord-1.0.1/tests/test_webhook_listener.py
+-rw-rw-rw-   0        0        0      183 2023-05-09 00:51:33.000000 diffcord-1.0.1/tests/testing_main.py
```

### Comparing `diffcord-1.0.0/LICENSE` & `diffcord-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.0/PKG-INFO` & `diffcord-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffcord
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python wrapper for the Diffcord API written in Python.
 Author: jadelasmar4@gmail.com
 Project-URL: Github, https://github.com/diff-cord/python-sdk
 Keywords: diffcord,diffcord-api,diffcord-api-wrapper,diffcord-api-python-wrapper,diffcord-api-python
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `diffcord-1.0.0/README.md` & `diffcord-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.0/diffcord/api.py` & `diffcord-1.0.1/diffcord/api.py`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.0/diffcord/client.py` & `diffcord-1.0.1/diffcord/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     """ Represents a client connection to the Diffcord API.
     """
     __SEND_STATS_SLEEP_DURATION = datetime.timedelta(hours=1)
 
     def __init__(self, bot: Any, token: str, vote_listener: VoteWebhookListener, send_stats: bool = True,
                  send_stats_success: Callable[[], Awaitable[None]] = None,
                  send_stats_failure: Callable[[Exception], Awaitable[None]] = None, base_url: str = None) -> None:
-        super().__init__(token, "https://diffcord.com/api" if base_url is None else base_url)
+        super().__init__(token, "https://www.diffcord.com/api" if base_url is None else base_url)
 
         self.bot: Any = bot
         """ The bot object. """
 
         self.token: str = token
         """ The Diffcord API token. """
```

### Comparing `diffcord-1.0.0/diffcord/error.py` & `diffcord-1.0.1/diffcord/error.py`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.0/diffcord/vote.py` & `diffcord-1.0.1/diffcord/vote.py`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.0/diffcord.egg-info/PKG-INFO` & `diffcord-1.0.1/diffcord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffcord
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python wrapper for the Diffcord API written in Python.
 Author: jadelasmar4@gmail.com
 Project-URL: Github, https://github.com/diff-cord/python-sdk
 Keywords: diffcord,diffcord-api,diffcord-api-wrapper,diffcord-api-python-wrapper,diffcord-api-python
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `diffcord-1.0.0/setup.py` & `diffcord-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='diffcord',
-    version='1.0.0',
+    version='1.0.1',
     description="A Python wrapper for the Diffcord API written in Python.",
     packages=find_packages(),
     author='jadelasmar4@gmail.com',
     zip_safe=False,
     install_requires=requirements,
     python_requires='>=3.7.0',
     long_description_content_type="text/markdown",
```

### Comparing `diffcord-1.0.0/tests/test_webhook_listener.py` & `diffcord-1.0.1/tests/test_webhook_listener.py`

 * *Files identical despite different names*

