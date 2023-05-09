# Comparing `tmp/diffcord-1.0.1.tar.gz` & `tmp/diffcord-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffcord-1.0.1.tar", last modified: Tue May  9 00:52:34 2023, max compression
+gzip compressed data, was "diffcord-1.0.2.tar", last modified: Tue May  9 20:08:00 2023, max compression
```

## Comparing `diffcord-1.0.1.tar` & `diffcord-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 00:52:34.852626 diffcord-1.0.1/
--rw-rw-rw-   0        0        0     1094 2023-03-12 19:55:56.000000 diffcord-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2607 2023-05-09 00:52:34.851624 diffcord-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-05-08 22:12:05.000000 diffcord-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 00:52:34.834626 diffcord-1.0.1/diffcord/
--rw-rw-rw-   0        0        0       86 2023-03-12 21:51:54.000000 diffcord-1.0.1/diffcord/__init__.py
--rw-rw-rw-   0        0        0     2228 2023-05-07 20:08:24.000000 diffcord-1.0.1/diffcord/api.py
--rw-rw-rw-   0        0        0     6751 2023-05-09 00:50:52.000000 diffcord-1.0.1/diffcord/client.py
--rw-rw-rw-   0        0        0     2111 2023-03-20 16:51:23.000000 diffcord-1.0.1/diffcord/error.py
--rw-rw-rw-   0        0        0     3397 2023-05-08 22:11:45.000000 diffcord-1.0.1/diffcord/vote.py
-drwxrwxrwx   0        0        0        0 2023-05-09 00:52:34.845626 diffcord-1.0.1/diffcord.egg-info/
--rw-rw-rw-   0        0        0     2607 2023-05-09 00:52:34.000000 diffcord-1.0.1/diffcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-05-09 00:52:34.000000 diffcord-1.0.1/diffcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 00:52:34.000000 diffcord-1.0.1/diffcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-09 00:52:34.000000 diffcord-1.0.1/diffcord.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2023-05-09 00:52:34.000000 diffcord-1.0.1/diffcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-09 00:52:34.000000 diffcord-1.0.1/diffcord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 00:52:34.852626 diffcord-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      727 2023-05-09 00:52:33.000000 diffcord-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 00:52:34.849625 diffcord-1.0.1/tests/
--rw-rw-rw-   0        0        0      108 2023-03-20 14:33:45.000000 diffcord-1.0.1/tests/test_client.py
--rw-rw-rw-   0        0        0     4232 2023-05-08 19:50:49.000000 diffcord-1.0.1/tests/test_webhook_listener.py
--rw-rw-rw-   0        0        0      183 2023-05-09 00:51:33.000000 diffcord-1.0.1/tests/testing_main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:08:00.342915 diffcord-1.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-03-12 19:55:56.000000 diffcord-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2607 2023-05-09 20:08:00.341915 diffcord-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-05-08 22:12:05.000000 diffcord-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 20:08:00.326913 diffcord-1.0.2/diffcord/
+-rw-rw-rw-   0        0        0       86 2023-03-12 21:51:54.000000 diffcord-1.0.2/diffcord/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-05-07 20:08:24.000000 diffcord-1.0.2/diffcord/api.py
+-rw-rw-rw-   0        0        0     7224 2023-05-09 20:02:04.000000 diffcord-1.0.2/diffcord/client.py
+-rw-rw-rw-   0        0        0     2111 2023-03-20 16:51:23.000000 diffcord-1.0.2/diffcord/error.py
+-rw-rw-rw-   0        0        0     3397 2023-05-08 22:11:45.000000 diffcord-1.0.2/diffcord/vote.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:08:00.335912 diffcord-1.0.2/diffcord.egg-info/
+-rw-rw-rw-   0        0        0     2607 2023-05-09 20:08:00.000000 diffcord-1.0.2/diffcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-05-09 20:08:00.000000 diffcord-1.0.2/diffcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 20:08:00.000000 diffcord-1.0.2/diffcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-09 20:08:00.000000 diffcord-1.0.2/diffcord.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       27 2023-05-09 20:08:00.000000 diffcord-1.0.2/diffcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 20:08:00.000000 diffcord-1.0.2/diffcord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 20:08:00.342915 diffcord-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      727 2023-05-09 20:07:55.000000 diffcord-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:08:00.340915 diffcord-1.0.2/tests/
+-rw-rw-rw-   0        0        0      108 2023-03-20 14:33:45.000000 diffcord-1.0.2/tests/test_client.py
+-rw-rw-rw-   0        0        0     4232 2023-05-08 19:50:49.000000 diffcord-1.0.2/tests/test_webhook_listener.py
+-rw-rw-rw-   0        0        0      216 2023-05-09 20:03:08.000000 diffcord-1.0.2/tests/testing_main.py
```

### Comparing `diffcord-1.0.1/LICENSE` & `diffcord-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.1/PKG-INFO` & `diffcord-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffcord
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python wrapper for the Diffcord API written in Python.
 Author: jadelasmar4@gmail.com
 Project-URL: Github, https://github.com/diff-cord/python-sdk
 Keywords: diffcord,diffcord-api,diffcord-api-wrapper,diffcord-api-python-wrapper,diffcord-api-python
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `diffcord-1.0.1/README.md` & `diffcord-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.1/diffcord/api.py` & `diffcord-1.0.2/diffcord/api.py`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.1/diffcord/client.py` & `diffcord-1.0.2/diffcord/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from asyncio import Task
 from typing import Union
 import asyncio
 import datetime
 from typing import Any, Callable, Awaitable
 
 from diffcord import InvalidTokenException
 from diffcord.api import HTTPApi
@@ -102,16 +103,19 @@
 class Client(HTTPApi):
     """ Represents a client connection to the Diffcord API.
     """
     __SEND_STATS_SLEEP_DURATION = datetime.timedelta(hours=1)
 
     def __init__(self, bot: Any, token: str, vote_listener: VoteWebhookListener, send_stats: bool = True,
                  send_stats_success: Callable[[], Awaitable[None]] = None,
-                 send_stats_failure: Callable[[Exception], Awaitable[None]] = None, base_url: str = None) -> None:
-        super().__init__(token, "https://www.diffcord.com/api" if base_url is None else base_url)
+                 send_stats_failure: Callable[[Exception], Awaitable[None]] = None,
+                 base_url: str = None,
+                 send_stats_interval: datetime.timedelta = None,
+                 ) -> None:
+        super().__init__(token, "https://diffcord.com/api" if base_url is None else base_url)
 
         self.bot: Any = bot
         """ The bot object. """
 
         self.token: str = token
         """ The Diffcord API token. """
 
@@ -123,14 +127,17 @@
 
         self.send_stats_success: Callable[[], Awaitable[None]] = send_stats_success
         """ A function to call when sending stats to Diffcord is successful (must be async). """
 
         self.send_stats_failure: Callable[[Exception], Awaitable[None]] = send_stats_failure
         """ A function to call when sending stats to Diffcord fails (must be async). """
 
+        self.send_stats_interval: datetime.timedelta = self.__SEND_STATS_SLEEP_DURATION if send_stats_interval is None else send_stats_interval
+        """ The interval between each stat update request. """
+
     async def get_user_vote_info(self, user_id: Union[str, int]) -> UserVoteInformation:
         """ Get the vote information for a user.
         :param: user_id: The id of the user whose vote information is being fetched
         :return: A UserVoteInformation object
         """
         vote_info: dict = await self.make_request("GET", f"/v1/users/{user_id}/votes")
         return UserVoteInformation(**vote_info)
@@ -144,15 +151,15 @@
 
     async def __update_bot_stats(self, guild_count: int) -> None:
         """ Update bot stats
         :param: guild_count: The new guild count
         """
         await self.make_request("POST", "/v1/stats", params={"guilds": guild_count})
 
-    async def start(self) -> None:
+    async def __start(self) -> None:
         """ Start the client
         """
         # start listener for incoming votes
         if self.vote_listener is not None:
             await self.vote_listener.start()
 
         # make a request to validate the token
@@ -172,14 +179,19 @@
                 except Exception as e:
                     if self.send_stats_failure is not None:
                         await self.send_stats_failure(e)
                 else:
                     if self.send_stats_success is not None:
                         await self.send_stats_success()
 
-                await asyncio.sleep(Client.__SEND_STATS_SLEEP_DURATION.total_seconds())
+                await asyncio.sleep(self.send_stats_interval.total_seconds())
+
+    def start(self) -> Task:
+        """ Start the client synchronously.
+        """
+        return asyncio.ensure_future(self.__start())
 
     def __repr__(self):
         return f"<Client bot={self.bot} token={self.token}>"
 
     def __str__(self):
         return self.__repr__()
```

### Comparing `diffcord-1.0.1/diffcord/error.py` & `diffcord-1.0.2/diffcord/error.py`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.1/diffcord/vote.py` & `diffcord-1.0.2/diffcord/vote.py`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.1/diffcord.egg-info/PKG-INFO` & `diffcord-1.0.2/diffcord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffcord
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python wrapper for the Diffcord API written in Python.
 Author: jadelasmar4@gmail.com
 Project-URL: Github, https://github.com/diff-cord/python-sdk
 Keywords: diffcord,diffcord-api,diffcord-api-wrapper,diffcord-api-python-wrapper,diffcord-api-python
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `diffcord-1.0.1/setup.py` & `diffcord-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='diffcord',
-    version='1.0.1',
+    version='1.0.2',
     description="A Python wrapper for the Diffcord API written in Python.",
     packages=find_packages(),
     author='jadelasmar4@gmail.com',
     zip_safe=False,
     install_requires=requirements,
     python_requires='>=3.7.0',
     long_description_content_type="text/markdown",
```

### Comparing `diffcord-1.0.1/tests/test_webhook_listener.py` & `diffcord-1.0.2/tests/test_webhook_listener.py`

 * *Files identical despite different names*

