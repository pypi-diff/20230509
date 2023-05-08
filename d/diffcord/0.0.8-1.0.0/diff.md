# Comparing `tmp/diffcord-0.0.8.tar.gz` & `tmp/diffcord-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffcord-0.0.8.tar", last modified: Mon May  8 20:25:47 2023, max compression
+gzip compressed data, was "diffcord-1.0.0.tar", last modified: Mon May  8 22:19:07 2023, max compression
```

## Comparing `diffcord-0.0.8.tar` & `diffcord-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 20:25:47.143549 diffcord-0.0.8/
--rw-rw-rw-   0        0        0     1094 2023-03-12 19:55:56.000000 diffcord-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2611 2023-05-08 20:25:47.142547 diffcord-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2202 2023-03-20 23:26:24.000000 diffcord-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 20:25:47.112556 diffcord-0.0.8/diffcord/
--rw-rw-rw-   0        0        0       86 2023-03-12 21:51:54.000000 diffcord-0.0.8/diffcord/__init__.py
--rw-rw-rw-   0        0        0     2228 2023-05-07 20:08:24.000000 diffcord-0.0.8/diffcord/api.py
--rw-rw-rw-   0        0        0     6747 2023-05-08 03:04:14.000000 diffcord-0.0.8/diffcord/client.py
--rw-rw-rw-   0        0        0     2111 2023-03-20 16:51:23.000000 diffcord-0.0.8/diffcord/error.py
--rw-rw-rw-   0        0        0     3333 2023-05-07 19:38:24.000000 diffcord-0.0.8/diffcord/vote.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:25:47.122574 diffcord-0.0.8/diffcord.egg-info/
--rw-rw-rw-   0        0        0     2611 2023-05-08 20:25:46.000000 diffcord-0.0.8/diffcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-05-08 20:25:46.000000 diffcord-0.0.8/diffcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 20:25:46.000000 diffcord-0.0.8/diffcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-20 17:40:35.000000 diffcord-0.0.8/diffcord.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2023-05-08 20:25:46.000000 diffcord-0.0.8/diffcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 20:25:46.000000 diffcord-0.0.8/diffcord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 20:25:47.143549 diffcord-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      727 2023-05-08 20:25:14.000000 diffcord-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 20:25:47.140577 diffcord-0.0.8/tests/
--rw-rw-rw-   0        0        0      108 2023-03-20 14:33:45.000000 diffcord-0.0.8/tests/test_client.py
--rw-rw-rw-   0        0        0     4232 2023-05-08 19:50:49.000000 diffcord-0.0.8/tests/test_webhook_listener.py
--rw-rw-rw-   0        0        0     2103 2023-05-08 19:58:25.000000 diffcord-0.0.8/tests/testing_main.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:19:07.835417 diffcord-1.0.0/
+-rw-rw-rw-   0        0        0     1094 2023-03-12 19:55:56.000000 diffcord-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2607 2023-05-08 22:19:07.834416 diffcord-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-05-08 22:12:05.000000 diffcord-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 22:19:07.816443 diffcord-1.0.0/diffcord/
+-rw-rw-rw-   0        0        0       86 2023-03-12 21:51:54.000000 diffcord-1.0.0/diffcord/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-05-07 20:08:24.000000 diffcord-1.0.0/diffcord/api.py
+-rw-rw-rw-   0        0        0     6747 2023-05-08 03:04:14.000000 diffcord-1.0.0/diffcord/client.py
+-rw-rw-rw-   0        0        0     2111 2023-03-20 16:51:23.000000 diffcord-1.0.0/diffcord/error.py
+-rw-rw-rw-   0        0        0     3397 2023-05-08 22:11:45.000000 diffcord-1.0.0/diffcord/vote.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:19:07.827416 diffcord-1.0.0/diffcord.egg-info/
+-rw-rw-rw-   0        0        0     2607 2023-05-08 22:19:07.000000 diffcord-1.0.0/diffcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-05-08 22:19:07.000000 diffcord-1.0.0/diffcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 22:19:07.000000 diffcord-1.0.0/diffcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 22:19:07.000000 diffcord-1.0.0/diffcord.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       27 2023-05-08 22:19:07.000000 diffcord-1.0.0/diffcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-08 22:19:07.000000 diffcord-1.0.0/diffcord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 22:19:07.835417 diffcord-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      727 2023-05-08 22:14:54.000000 diffcord-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:19:07.832414 diffcord-1.0.0/tests/
+-rw-rw-rw-   0        0        0      108 2023-03-20 14:33:45.000000 diffcord-1.0.0/tests/test_client.py
+-rw-rw-rw-   0        0        0     4232 2023-05-08 19:50:49.000000 diffcord-1.0.0/tests/test_webhook_listener.py
+-rw-rw-rw-   0        0        0     2041 2023-05-08 22:12:21.000000 diffcord-1.0.0/tests/testing_main.py
```

### Comparing `diffcord-0.0.8/LICENSE` & `diffcord-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diffcord-0.0.8/PKG-INFO` & `diffcord-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffcord
-Version: 0.0.8
+Version: 1.0.0
 Summary: A Python wrapper for the Diffcord API written in Python.
 Author: jadelasmar4@gmail.com
 Project-URL: Github, https://github.com/diff-cord/python-sdk
 Keywords: diffcord,diffcord-api,diffcord-api-wrapper,diffcord-api-python-wrapper,diffcord-api-python
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -57,15 +57,15 @@
 
 # "port" represents the port to listen on for incoming vote webhooks from Diffcord, choose any port you would like which is not in use
 diff_webhook_listener = VoteWebhookListener(port=8080, handle_vote=on_vote, verify_code="WEBHOOK_AUTH_CODE_HERE")
 
 diff_client = Client(bot, "YOUR_DIFFCORD_API_TOKEN", diff_webhook_listener,
                      send_stats_success=send_stats_success, send_stats_failure=send_stats_failure)
 
-bot.diffcord_client = diff_client
+bot.diff_client = diff_client
 
 # on startup event
 @bot.event
 async def on_ready():
     # start the webhook listener & start send stats
     await diff_client.start()  # required
```

### Comparing `diffcord-0.0.8/README.md` & `diffcord-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 # "port" represents the port to listen on for incoming vote webhooks from Diffcord, choose any port you would like which is not in use
 diff_webhook_listener = VoteWebhookListener(port=8080, handle_vote=on_vote, verify_code="WEBHOOK_AUTH_CODE_HERE")
 
 diff_client = Client(bot, "YOUR_DIFFCORD_API_TOKEN", diff_webhook_listener,
                      send_stats_success=send_stats_success, send_stats_failure=send_stats_failure)
 
-bot.diffcord_client = diff_client
+bot.diff_client = diff_client
 
 # on startup event
 @bot.event
 async def on_ready():
     # start the webhook listener & start send stats
     await diff_client.start()  # required
```

### Comparing `diffcord-0.0.8/diffcord/api.py` & `diffcord-1.0.0/diffcord/api.py`

 * *Files identical despite different names*

### Comparing `diffcord-0.0.8/diffcord/client.py` & `diffcord-1.0.0/diffcord/client.py`

 * *Files identical despite different names*

### Comparing `diffcord-0.0.8/diffcord/error.py` & `diffcord-1.0.0/diffcord/error.py`

 * *Files identical despite different names*

### Comparing `diffcord-0.0.8/diffcord/vote.py` & `diffcord-1.0.0/diffcord/vote.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+from typing import Union
 
 
 class UserBotVote:
     """  Represents a user vote for a bot.
     """
 
     def __init__(self, vote_id: str, user_id: str, bot_id: str, since_vote: str, rewarded: bool, test: bool,
@@ -45,25 +46,27 @@
         return self.__repr__()
 
 
 class UserVoteInformation:
     """ Represents a user vote information.
     """
 
-    def __init__(self, user_id: str, bot_id: str, monthly_votes: int, since_last_vote: int | None, until_next_vote: int):
+    def __init__(self, user_id: str, bot_id: str, monthly_votes: int, since_last_vote: Union[int, None],
+                 until_next_vote: int):
         self.user_id: str = user_id
         """ The id of the target user. """
 
         self.bot_id: str = bot_id
         """ The id of the bot which the user has voted for. """
 
         self.monthly_votes: int = monthly_votes
         """ The number of votes this user has for the given bot this month. """
 
-        self.since_last_vote: datetime.timedelta = datetime.timedelta(seconds=since_last_vote) if since_last_vote is not None else None
+        self.since_last_vote: datetime.timedelta = datetime.timedelta(
+            seconds=since_last_vote) if since_last_vote is not None else None
         """ Time in seconds since the last vote. """
 
         self.until_next_vote: datetime.timedelta = datetime.timedelta(seconds=until_next_vote)
         """ Time in seconds till the next vote. """
 
         self.last_vote: datetime.datetime = datetime.datetime.now() - self.since_last_vote if self.since_last_vote is not None else None
         """ The last time the user voted. """
```

### Comparing `diffcord-0.0.8/diffcord.egg-info/PKG-INFO` & `diffcord-1.0.0/diffcord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffcord
-Version: 0.0.8
+Version: 1.0.0
 Summary: A Python wrapper for the Diffcord API written in Python.
 Author: jadelasmar4@gmail.com
 Project-URL: Github, https://github.com/diff-cord/python-sdk
 Keywords: diffcord,diffcord-api,diffcord-api-wrapper,diffcord-api-python-wrapper,diffcord-api-python
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -57,15 +57,15 @@
 
 # "port" represents the port to listen on for incoming vote webhooks from Diffcord, choose any port you would like which is not in use
 diff_webhook_listener = VoteWebhookListener(port=8080, handle_vote=on_vote, verify_code="WEBHOOK_AUTH_CODE_HERE")
 
 diff_client = Client(bot, "YOUR_DIFFCORD_API_TOKEN", diff_webhook_listener,
                      send_stats_success=send_stats_success, send_stats_failure=send_stats_failure)
 
-bot.diffcord_client = diff_client
+bot.diff_client = diff_client
 
 # on startup event
 @bot.event
 async def on_ready():
     # start the webhook listener & start send stats
     await diff_client.start()  # required
```

### Comparing `diffcord-0.0.8/setup.py` & `diffcord-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='diffcord',
-    version='0.0.8',
+    version='1.0.0',
     description="A Python wrapper for the Diffcord API written in Python.",
     packages=find_packages(),
     author='jadelasmar4@gmail.com',
     zip_safe=False,
     install_requires=requirements,
     python_requires='>=3.7.0',
     long_description_content_type="text/markdown",
```

### Comparing `diffcord-0.0.8/tests/test_webhook_listener.py` & `diffcord-1.0.0/tests/test_webhook_listener.py`

 * *Files identical despite different names*

### Comparing `diffcord-0.0.8/tests/testing_main.py` & `diffcord-1.0.0/tests/testing_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,8 +57,8 @@
     bot_votes_this_month: int = await diff_client.bot_votes_this_month()
 
     # respond
     message = f"You have voted {user_vote_info.monthly_votes} times this month! This bot has {bot_votes_this_month} votes this month!"
     await ctx.respond(message)
 
 
-bot.run("MTA1MzE1ODc4MDk1MjY0NTY2Mg.GMKTP-.iW4SSYBjLDjKTGyRyUXWOlWEkpUvEJGSJGkUM4")
+bot.run("TOKEN_HERE")
```

