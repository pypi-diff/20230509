# Comparing `tmp/twscrape-0.1.0.tar.gz` & `tmp/twscrape-0.1.1.tar.gz`

## Comparing `twscrape-0.1.0.tar` & `twscrape-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.1.0/.gitattributes
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 twscrape-0.1.0/Makefile
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.1.0/.github/CODEOWNERS
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 twscrape-0.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 twscrape-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 twscrape-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 twscrape-0.1.0/tests/test_parser.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 twscrape-0.1.0/tests/test_pool.py
--rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.1.0/tests/mocked-data/favoriters_raw.json
--rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.1.0/tests/mocked-data/followers_raw.json
--rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.1.0/tests/mocked-data/following_raw.json
--rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.1.0/tests/mocked-data/retweeters_raw.json
--rw-r--r--   0        0        0   177570 2020-02-02 00:00:00.000000 twscrape-0.1.0/tests/mocked-data/search_raw.json
--rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.1.0/tests/mocked-data/tweet_details_raw.json
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.1.0/tests/mocked-data/user_by_id_raw.json
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.1.0/tests/mocked-data/user_by_login_raw.json
--rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.1.0/tests/mocked-data/user_tweets_and_replies_raw.json
--rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.1.0/tests/mocked-data/user_tweets_raw.json
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 twscrape-0.1.0/twscrape/__init__.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 twscrape-0.1.0/twscrape/account.py
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 twscrape-0.1.0/twscrape/accounts_pool.py
--rw-r--r--   0        0        0    13024 2020-02-02 00:00:00.000000 twscrape-0.1.0/twscrape/api.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 twscrape-0.1.0/twscrape/constants.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 twscrape-0.1.0/twscrape/db.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 twscrape-0.1.0/twscrape/imap.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.1.0/twscrape/logger.py
--rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 twscrape-0.1.0/twscrape/login.py
--rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 twscrape-0.1.0/twscrape/models.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 twscrape-0.1.0/twscrape/utils.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.1.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.1.0/LICENSE
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 twscrape-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 twscrape-0.1.0/readme.md
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 twscrape-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.1.1/.gitattributes
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 twscrape-0.1.1/Makefile
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.1.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 twscrape-0.1.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 twscrape-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 twscrape-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/test_parser.py
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/test_pool.py
+-rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/favoriters_raw.json
+-rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/followers_raw.json
+-rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/following_raw.json
+-rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/retweeters_raw.json
+-rw-r--r--   0        0        0   177570 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/search_raw.json
+-rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/tweet_details_raw.json
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/user_by_id_raw.json
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/user_by_login_raw.json
+-rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/user_tweets_and_replies_raw.json
+-rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/user_tweets_raw.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/__init__.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/account.py
+-rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/accounts_pool.py
+-rw-r--r--   0        0        0    12984 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/api.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/constants.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/db.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/imap.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/logger.py
+-rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/login.py
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/models.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/utils.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 twscrape-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 twscrape-0.1.1/readme.md
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 twscrape-0.1.1/PKG-INFO
```

### Comparing `twscrape-0.1.0/tests/test_parser.py` & `twscrape-0.1.1/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,22 @@
     for doc in items:
         assert doc.id is not None
         assert doc.user is not None
 
         obj = doc.dict()
         assert doc.id == obj["id"]
         assert doc.user.id == obj["user"]["id"]
+
         assert "url" in obj
+        assert "_type" in obj
+        assert obj["_type"] == "snscrape.modules.twitter.Tweet"
+
         assert "url" in obj["user"]
+        assert "_type" in obj["user"]
+        assert obj["user"]["_type"] == "snscrape.modules.twitter.User"
 
         txt = doc.json()
         assert isinstance(txt, str)
         assert str(doc.id) in txt
 
 
 async def test_user_by_id():
```

### Comparing `twscrape-0.1.0/tests/mocked-data/favoriters_raw.json` & `twscrape-0.1.1/tests/mocked-data/favoriters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/tests/mocked-data/followers_raw.json` & `twscrape-0.1.1/tests/mocked-data/followers_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/tests/mocked-data/following_raw.json` & `twscrape-0.1.1/tests/mocked-data/following_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/tests/mocked-data/retweeters_raw.json` & `twscrape-0.1.1/tests/mocked-data/retweeters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/tests/mocked-data/search_raw.json` & `twscrape-0.1.1/tests/mocked-data/search_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/tests/mocked-data/tweet_details_raw.json` & `twscrape-0.1.1/tests/mocked-data/tweet_details_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/tests/mocked-data/user_by_id_raw.json` & `twscrape-0.1.1/tests/mocked-data/user_by_id_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/tests/mocked-data/user_by_login_raw.json` & `twscrape-0.1.1/tests/mocked-data/user_by_login_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/tests/mocked-data/user_tweets_and_replies_raw.json` & `twscrape-0.1.1/tests/mocked-data/user_tweets_and_replies_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/tests/mocked-data/user_tweets_raw.json` & `twscrape-0.1.1/tests/mocked-data/user_tweets_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/twscrape/account.py` & `twscrape-0.1.1/twscrape/account.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sqlite3
 from dataclasses import asdict, dataclass
 from datetime import datetime
 
 from httpx import AsyncClient, AsyncHTTPTransport
 
 from .constants import TOKEN
+from .utils import from_utciso
 
 
 @dataclass
 class Account:
     username: str
     password: str
     email: str
@@ -39,15 +40,15 @@
             error_msg TEXT DEFAULT NULL
         );
         """
 
     @staticmethod
     def from_rs(rs: sqlite3.Row):
         doc = dict(rs)
-        doc["locks"] = {k: datetime.fromisoformat(v) for k, v in json.loads(doc["locks"]).items()}
+        doc["locks"] = {k: from_utciso(v) for k, v in json.loads(doc["locks"]).items()}
         doc["headers"] = json.loads(doc["headers"])
         doc["cookies"] = json.loads(doc["cookies"])
         doc["active"] = bool(doc["active"])
         return Account(**doc)
 
     def to_rs(self):
         rs = asdict(self)
```

### Comparing `twscrape-0.1.0/twscrape/accounts_pool.py` & `twscrape-0.1.1/twscrape/accounts_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,15 +84,14 @@
             await self.login(x)
 
     async def set_active(self, username: str, active: bool):
         qs = "UPDATE accounts SET active = :active WHERE username = :username"
         await execute(self._db_file, qs, {"username": username, "active": active})
 
     async def lock_until(self, username: str, queue: str, unlock_at: int):
-        # unlock_at is unix timestamp
         qs = f"""
         UPDATE accounts SET locks = json_set(locks, '$.{queue}', datetime({unlock_at}, 'unixepoch'))
         WHERE username = :username
         """
         await execute(self._db_file, qs, {"username": username})
 
     async def unlock(self, username: str, queue: str):
@@ -137,17 +136,24 @@
     async def stats(self):
         def by_queue(queue: str):
             return f"""
             SELECT COUNT(*) FROM accounts
             WHERE json_extract(locks, '$.{queue}') IS NOT NULL AND json_extract(locks, '$.{queue}') > datetime('now')
             """
 
+        gql_ops = """
+        UserByRestId UserByScreenName TweetDetail Followers Following
+        Retweeters Favoriters UserTweets UserTweetsAndReplies
+        """
+        gql_ops = [x.strip() for x in gql_ops.split(" ") if x.strip()]
+
         config = [
             ("total", "SELECT COUNT(*) FROM accounts"),
             ("active", "SELECT COUNT(*) FROM accounts WHERE active = true"),
             ("inactive", "SELECT COUNT(*) FROM accounts WHERE active = false"),
             ("locked_search", by_queue("search")),
+            *[(f"locked_{x}", by_queue(x)) for x in gql_ops],
         ]
 
         qs = f"SELECT {','.join([f'({q}) as {k}' for k, q in config])}"
         rs = await fetchone(self._db_file, qs)
         return dict(rs) if rs else {}
```

### Comparing `twscrape-0.1.0/twscrape/api.py` & `twscrape-0.1.1/twscrape/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import json
-import time
 from datetime import datetime
 from typing import Awaitable, Callable
 
 from httpx import AsyncClient, HTTPStatusError, Response
 
 from .accounts_pool import AccountsPool
 from .constants import GQL_FEATURES, GQL_URL, SEARCH_PARAMS, SEARCH_URL
 from .logger import logger
 from .models import Tweet, User
-from .utils import encode_params, find_obj, get_by_path, to_old_obj, to_search_like
+from .utils import encode_params, find_obj, get_by_path, to_old_obj, to_old_rep, utc_ts
 
 
 class API:
     def __init__(self, pool: AccountsPool, debug=False):
         self.pool = pool
         self.debug = debug
         self._history: list[Response] = []
@@ -91,16 +90,16 @@
                     logger.debug(f"Rate limit for {log_id}")
                     reset_ts = int(rep.headers.get("x-rate-limit-reset", 0))
                     await self.pool.lock_until(acc.username, queue, reset_ts)
                     continue
 
                 # possible account banned
                 if rep.status_code == 403:
-                    logger.debug(f"Ban for {log_id}")
-                    reset_ts = int(time.time() + 60 * 60)  # 1 hour
+                    logger.warning(f"403 for {log_id}")
+                    reset_ts = utc_ts() + 60 * 60  # + 1 hour
                     await self.pool.lock_until(acc.username, queue, reset_ts)
                     continue
 
                 # twitter can return different types of cursors that not transfers between accounts
                 # just take the next account, the current cursor can work in it
                 if rep.status_code == 400:
                     logger.debug(f"Cursor not valid for {log_id}")
@@ -252,70 +251,70 @@
             "responsive_web_twitter_blue_verified_badge_is_enabled": True,
             "longform_notetweets_richtext_consumption_enabled": True,
         }
         return await self._ql_item(op, kv, ft)
 
     async def tweet_details(self, twid: int):
         rep = await self.tweet_details_raw(twid)
-        obj = to_search_like(rep.json())
+        obj = to_old_rep(rep.json())
         return Tweet.parse(obj["tweets"][str(twid)], obj)
 
     # followers
 
     async def followers_raw(self, uid: int, limit=-1):
         op = "djdTXDIk2qhd4OStqlUFeQ/Followers"
         kv = {"userId": str(uid), "count": 20, "includePromotedContent": False}
         async for x in self._ql_items(op, kv, limit=limit):
             yield x
 
     async def followers(self, uid: int, limit=-1):
         async for rep in self.followers_raw(uid, limit=limit):
-            obj = to_search_like(rep.json())
+            obj = to_old_rep(rep.json())
             for _, v in obj["users"].items():
                 yield User.parse(v)
 
     # following
 
     async def following_raw(self, uid: int, limit=-1):
         op = "IWP6Zt14sARO29lJT35bBw/Following"
         kv = {"userId": str(uid), "count": 20, "includePromotedContent": False}
         async for x in self._ql_items(op, kv, limit=limit):
             yield x
 
     async def following(self, uid: int, limit=-1):
         async for rep in self.following_raw(uid, limit=limit):
-            obj = to_search_like(rep.json())
+            obj = to_old_rep(rep.json())
             for _, v in obj["users"].items():
                 yield User.parse(v)
 
     # retweeters
 
     async def retweeters_raw(self, twid: int, limit=-1):
         op = "U5f_jm0CiLmSfI1d4rGleQ/Retweeters"
         kv = {"tweetId": str(twid), "count": 20, "includePromotedContent": True}
         async for x in self._ql_items(op, kv, limit=limit):
             yield x
 
     async def retweeters(self, twid: int, limit=-1):
         async for rep in self.retweeters_raw(twid, limit=limit):
-            obj = to_search_like(rep.json())
+            obj = to_old_rep(rep.json())
             for _, v in obj["users"].items():
                 yield User.parse(v)
 
     # favoriters
 
     async def favoriters_raw(self, twid: int, limit=-1):
         op = "vcTrPlh9ovFDQejz22q9vg/Favoriters"
         kv = {"tweetId": str(twid), "count": 20, "includePromotedContent": True}
         async for x in self._ql_items(op, kv, limit=limit):
             yield x
 
     async def favoriters(self, twid: int, limit=-1):
         async for rep in self.favoriters_raw(twid, limit=limit):
-            obj = to_search_like(rep.json())
+            obj = to_old_rep(rep.json())
             for _, v in obj["users"].items():
                 yield User.parse(v)
 
     # user_tweets
 
     async def user_tweets_raw(self, uid: int, limit=-1):
         op = "CdG2Vuc1v6F5JyEngGpxVw/UserTweets"
@@ -328,15 +327,15 @@
             "withV2Timeline": True,
         }
         async for x in self._ql_items(op, kv, limit=limit):
             yield x
 
     async def user_tweets(self, uid: int, limit=-1):
         async for rep in self.user_tweets_raw(uid, limit=limit):
-            obj = to_search_like(rep.json())
+            obj = to_old_rep(rep.json())
             for _, v in obj["tweets"].items():
                 yield Tweet.parse(v, obj)
 
     # user_tweets_and_replies
 
     async def user_tweets_and_replies_raw(self, uid: int, limit=-1):
         op = "zQxfEr5IFxQ2QZ-XMJlKew/UserTweetsAndReplies"
@@ -349,10 +348,10 @@
             "withV2Timeline": True,
         }
         async for x in self._ql_items(op, kv, limit=limit):
             yield x
 
     async def user_tweets_and_replies(self, uid: int, limit=-1):
         async for rep in self.user_tweets_and_replies_raw(uid, limit=limit):
-            obj = to_search_like(rep.json())
+            obj = to_old_rep(rep.json())
             for _, v in obj["tweets"].items():
                 yield Tweet.parse(v, obj)
```

### Comparing `twscrape-0.1.0/twscrape/constants.py` & `twscrape-0.1.1/twscrape/constants.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/twscrape/db.py` & `twscrape-0.1.1/twscrape/db.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/twscrape/imap.py` & `twscrape-0.1.1/twscrape/imap.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/twscrape/login.py` & `twscrape-0.1.1/twscrape/login.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/twscrape/models.py` & `twscrape-0.1.1/twscrape/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import email.utils
 import json
 import re
 from dataclasses import asdict, dataclass
 from datetime import datetime
 from typing import Optional
 
-from .logger import logger
 from .utils import find_item, get_or, int_or_none
 
 
 @dataclass
 class JSONTrait:
     def dict(self):
         return asdict(self)
@@ -73,14 +72,15 @@
 
 
 @dataclass
 class UserRef(JSONTrait):
     id: int
     username: str
     displayname: str
+    _type: str = "snscrape.modules.twitter.UserRef"
 
     @staticmethod
     def parse(obj: dict):
         return UserRef(id=int(obj["id_str"]), username=obj["screen_name"], displayname=obj["name"])
 
 
 @dataclass
@@ -98,15 +98,17 @@
     listedCount: int
     mediaCount: int
     location: str
     profileImageUrl: str
     profileBannerUrl: str | None = None
     protected: bool | None = None
     verified: bool | None = None
+    _type: str = "snscrape.modules.twitter.User"
 
+    # todo:
     # descriptionLinks: typing.Optional[typing.List[TextLink]] = None
     # link: typing.Optional[TextLink] = None
     # label: typing.Optional["UserLabel"] = None
 
     @staticmethod
     def parse(obj: dict):
         return User(
@@ -153,15 +155,17 @@
     place: Optional[Place] = None
     coordinates: Optional[Coordinates] = None
     inReplyToTweetId: int | None = None
     inReplyToUser: UserRef | None = None
     source: str | None = None
     sourceUrl: str | None = None
     sourceLabel: str | None = None
+    _type: str = "snscrape.modules.twitter.Tweet"
 
+    # todo:
     # renderedContent: str
     # media: typing.Optional[typing.List["Medium"]] = None
     # card: typing.Optional["Card"] = None
     # vibe: typing.Optional["Vibe"] = None
 
     @staticmethod
     def parse(obj: dict, res: dict):
@@ -207,15 +211,15 @@
         return UserRef.parse(res["users"][user_id])
 
     mentions = get_or(tw_obj, "entities.user_mentions", [])
     mention = find_item(mentions, lambda x: x["id_str"] == tw_obj["in_reply_to_user_id_str"])
     if mention:
         return UserRef.parse(mention)
 
-    logger.debug(f'{tw_obj["in_reply_to_user_id_str"]}\n{json.dumps(res)}')
+    # todo: user not found in reply (probably deleted or hidden)
     return None
 
 
 def _get_source_url(tw_obj: dict):
     source = tw_obj.get("source", None)
     if source and (match := re.search(r'href=[\'"]?([^\'" >]+)', source)):
         return str(match.group(1))
```

### Comparing `twscrape-0.1.0/twscrape/utils.py` & `twscrape-0.1.1/twscrape/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from collections import defaultdict
+from datetime import datetime, timezone
 from typing import Any, AsyncGenerator, Callable, TypeVar
 
 from httpx import HTTPStatusError, Response
 
 from .logger import logger
 
 T = TypeVar("T")
@@ -119,17 +120,25 @@
     return res
 
 
 def to_old_obj(obj: dict):
     return {**obj, **obj["legacy"], "id_str": str(obj["rest_id"]), "id": int(obj["rest_id"])}
 
 
-def to_search_like(obj: dict):
+def to_old_rep(obj: dict):
     tmp = get_typed_object(obj, defaultdict(list))
 
     tweets = [x for x in tmp.get("Tweet", []) if "legacy" in x]
     tweets = {str(x["rest_id"]): to_old_obj(x) for x in tweets}
 
     users = [x for x in tmp.get("User", []) if "legacy" in x and "id" in x]
     users = {str(x["rest_id"]): to_old_obj(x) for x in users}
 
     return {"tweets": tweets, "users": users}
+
+
+def utc_ts() -> int:
+    return int(datetime.utcnow().replace(tzinfo=timezone.utc).timestamp())
+
+
+def from_utciso(iso: str) -> datetime:
+    return datetime.fromisoformat(iso).replace(tzinfo=timezone.utc)
```

### Comparing `twscrape-0.1.0/.gitignore` & `twscrape-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/LICENSE` & `twscrape-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.0/pyproject.toml` & `twscrape-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "twscrape"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{name = "vladkens", email = "v.pronsky@gmail.com"}]
 description = "Twitter GraphQL and Search API implementation with SNScrape data models"
 readme = "readme.md"
 requires-python = ">=3.10"
 keywords = ["twitter", "scrape", "scrapper", "api", "snscrape"]
 license = {text = "MIT"}
 classifiers = [
```

### Comparing `twscrape-0.1.0/readme.md` & `twscrape-0.1.1/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 # twscrape
 
 Twitter GraphQL and Search API implementation with [SNScrape](https://github.com/JustAnotherArchivist/snscrape) data models.
 
 ## Install
 
 ```bash
-pip install https://github.com/vladkens/tw-api
+pip install twscrape
+```
+Or development version:
+```bash
+pip install git+https://github.com/vladkens/twscrape.git
 ```
 
 ## Features
 - Support both Search & GraphQL Twitter API
-- Async / Await functions (can run multiple scrappers in parallel same time)
+- Async/Await functions (can run multiple scrapers in parallel at the same time)
 - Login flow (with receiving verification code from email)
-- Saving / restore accounts sessions
+- Saving/restoring account sessions
 - Raw Twitter API responses & SNScrape models
 - Automatic account switching to smooth Twitter API rate limits
 
 ## Usage
 
 ```python
 import asyncio
 from twscrape import AccountsPool, API, gather
 from twscrape.logger import set_log_level
 
 async def main():
-    pool = AccountsPool()  # or pool = AccountsPool("path-to.db") - default is `accounts.db` 
+    pool = AccountsPool()  # or AccountsPool("path-to.db") - default is `accounts.db` 
     await pool.add_account("user1", "pass1", "user1@example.com", "email_pass1")
     await pool.add_account("user2", "pass2", "user2@example.com", "email_pass2")
 
-    # log in to all fresh accounts
+    # log in to all new accounts
     await pool.login_all()
 
     api = API(pool)
 
-    # search api
+    # search api (latest tab)
     await gather(api.search("elon musk", limit=20))  # list[Tweet]
 
     # graphql api
-    tweet_id = 20
-    user_id, user_login = 2244994945, "twitterdev"
+    tweet_id, user_id, user_login = 20, 2244994945, "twitterdev"
 
     await api.tweet_details(tweet_id)  # Tweet
     await gather(api.retweeters(tweet_id, limit=20))  # list[User]
     await gather(api.favoriters(tweet_id, limit=20))  # list[User]
 
     await api.user_by_id(user_id)  # User
     await api.user_by_login(user_login)  # User
@@ -68,8 +71,17 @@
     doc.dict()  # -> python dict
     doc.json()  # -> json string
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
-You can use `login_all` once in your program to pass the login flow and add the accounts to the database. Re-runs will use the previously activated accounts.
+Note on rate limits:
+- Search API – 250 requests per account / 15 minites
+- GraphQL API – 500 requests per account per operation / 15 minutes
+
+### Models
+- [Tweet](https://github.com/vladkens/twscrape/blob/main/twscrape/models.py#:~:text=class%20Tweet)
+- [User](https://github.com/vladkens/twscrape/blob/main/twscrape/models.py#:~:text=class%20User)
+
+### Related
+- [SNScrape](https://github.com/JustAnotherArchivist/snscrape) – is a scraper for social networking services (SNS)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `twscrape-0.1.0/PKG-INFO` & `twscrape-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twscrape
-Version: 0.1.0
+Version: 0.1.1
 Summary: Twitter GraphQL and Search API implementation with SNScrape data models
 Project-URL: repository, https://github.com/vladkens/twscrape
 Author-email: vladkens <v.pronsky@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: api,scrape,scrapper,snscrape,twitter
 Classifier: Development Status :: 4 - Beta
@@ -27,48 +27,51 @@
 # twscrape
 
 Twitter GraphQL and Search API implementation with [SNScrape](https://github.com/JustAnotherArchivist/snscrape) data models.
 
 ## Install
 
 ```bash
-pip install https://github.com/vladkens/tw-api
+pip install twscrape
+```
+Or development version:
+```bash
+pip install git+https://github.com/vladkens/twscrape.git
 ```
 
 ## Features
 - Support both Search & GraphQL Twitter API
-- Async / Await functions (can run multiple scrappers in parallel same time)
+- Async/Await functions (can run multiple scrapers in parallel at the same time)
 - Login flow (with receiving verification code from email)
-- Saving / restore accounts sessions
+- Saving/restoring account sessions
 - Raw Twitter API responses & SNScrape models
 - Automatic account switching to smooth Twitter API rate limits
 
 ## Usage
 
 ```python
 import asyncio
 from twscrape import AccountsPool, API, gather
 from twscrape.logger import set_log_level
 
 async def main():
-    pool = AccountsPool()  # or pool = AccountsPool("path-to.db") - default is `accounts.db` 
+    pool = AccountsPool()  # or AccountsPool("path-to.db") - default is `accounts.db` 
     await pool.add_account("user1", "pass1", "user1@example.com", "email_pass1")
     await pool.add_account("user2", "pass2", "user2@example.com", "email_pass2")
 
-    # log in to all fresh accounts
+    # log in to all new accounts
     await pool.login_all()
 
     api = API(pool)
 
-    # search api
+    # search api (latest tab)
     await gather(api.search("elon musk", limit=20))  # list[Tweet]
 
     # graphql api
-    tweet_id = 20
-    user_id, user_login = 2244994945, "twitterdev"
+    tweet_id, user_id, user_login = 20, 2244994945, "twitterdev"
 
     await api.tweet_details(tweet_id)  # Tweet
     await gather(api.retweeters(tweet_id, limit=20))  # list[User]
     await gather(api.favoriters(tweet_id, limit=20))  # list[User]
 
     await api.user_by_id(user_id)  # User
     await api.user_by_login(user_login)  # User
@@ -94,8 +97,17 @@
     doc.dict()  # -> python dict
     doc.json()  # -> json string
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
-You can use `login_all` once in your program to pass the login flow and add the accounts to the database. Re-runs will use the previously activated accounts.
+Note on rate limits:
+- Search API – 250 requests per account / 15 minites
+- GraphQL API – 500 requests per account per operation / 15 minutes
+
+### Models
+- [Tweet](https://github.com/vladkens/twscrape/blob/main/twscrape/models.py#:~:text=class%20Tweet)
+- [User](https://github.com/vladkens/twscrape/blob/main/twscrape/models.py#:~:text=class%20User)
+
+### Related
+- [SNScrape](https://github.com/JustAnotherArchivist/snscrape) – is a scraper for social networking services (SNS)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

