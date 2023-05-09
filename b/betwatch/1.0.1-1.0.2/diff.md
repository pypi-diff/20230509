# Comparing `tmp/betwatch-1.0.1.tar.gz` & `tmp/betwatch-1.0.2.tar.gz`

## Comparing `betwatch-1.0.1.tar` & `betwatch-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.0.1/Makefile
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.0.1/betwatch/__about__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.0.1/betwatch/__init__.py
--rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.0.1/betwatch/client.py
--rw-r--r--   0        0        0    26499 2020-02-02 00:00:00.000000 betwatch-1.0.1/betwatch/client_async.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.0.1/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.0.1/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 betwatch-1.0.1/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 betwatch-1.0.1/betwatch/types/filters.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.0.1/betwatch/types/markets.py
--rw-r--r--   0        0        0    11720 2020-02-02 00:00:00.000000 betwatch-1.0.1/betwatch/types/race.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.0.1/betwatch/types/updates.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 betwatch-1.0.1/examples/get_race_prices.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.0.1/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.0.1/examples/get_races.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.0.1/examples/get_races_async.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 betwatch-1.0.1/examples/subscriptions.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.0.1/examples/update_rated_prices.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.0.1/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.0.1/tests/test_get_race.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.0.1/tests/test_get_race_async.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.0.1/tests/test_get_races.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.0.1/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 betwatch-1.0.1/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.0.1/README.md
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.0.2/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.0.2/betwatch/__about__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.0.2/betwatch/__init__.py
+-rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.0.2/betwatch/client.py
+-rw-r--r--   0        0        0    26499 2020-02-02 00:00:00.000000 betwatch-1.0.2/betwatch/client_async.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.0.2/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.0.2/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 betwatch-1.0.2/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 betwatch-1.0.2/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.0.2/betwatch/types/markets.py
+-rw-r--r--   0        0        0    11720 2020-02-02 00:00:00.000000 betwatch-1.0.2/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.0.2/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 betwatch-1.0.2/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.0.2/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.0.2/examples/get_races.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.0.2/examples/get_races_async.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 betwatch-1.0.2/examples/subscriptions.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.0.2/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.0.2/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.0.2/tests/test_get_race.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.0.2/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.0.2/tests/test_get_races.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.0.2/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 betwatch-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.0.2/README.md
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.0.2/PKG-INFO
```

### Comparing `betwatch-1.0.1/.github/workflows/test.yml` & `betwatch-1.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/betwatch/__init__.py` & `betwatch-1.0.2/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/betwatch/client.py` & `betwatch-1.0.2/betwatch/client.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/betwatch/client_async.py` & `betwatch-1.0.2/betwatch/client_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,15 +506,15 @@
                     self._subscription_queue.put_nowait(update)
         except TransportError as e:
             logging.debug(f"Error subscribing to bookmaker updates: {e}")
         except asyncio.CancelledError:
             await self.unsubscribe_bookmaker_updates(race_id)
             return
         except Exception as e:
-            logging.error(f"Error subscribing to bookmaker updates: {e}")
+            logging.debug(f"Error subscribing to bookmaker updates: {e}")
 
     async def unsubscribe_betfair_updates(self, race_id: str):
         if race_id not in self._subscriptions_betfair:
             logging.info(
                 f"Not subscribed to {race_id if race_id else 'all races'} betfair updates"
             )
             return
@@ -615,15 +615,15 @@
                     update = SubscriptionUpdate(
                         race_id=ru.id,
                         race_update=ru,
                     )
                     self._subscription_queue.put_nowait(update)
 
         except TransportError as e:
-            logging.error(f"Error subscribing to race updates: {e}")
+            logging.debug(f"Error subscribing to race updates: {e}")
         except asyncio.CancelledError:
             await self.unsubscribe_race_updates(date_from, date_to)
             return
 
     @backoff.on_exception(backoff.expo, Exception, max_time=60, max_tries=5)
     async def _get_race_by_id(
         self,
```

### Comparing `betwatch-1.0.1/betwatch/queries.py` & `betwatch-1.0.2/betwatch/queries.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/betwatch/types/bookmakers.py` & `betwatch-1.0.2/betwatch/types/bookmakers.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/betwatch/types/filters.py` & `betwatch-1.0.2/betwatch/types/filters.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/betwatch/types/markets.py` & `betwatch-1.0.2/betwatch/types/markets.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/betwatch/types/race.py` & `betwatch-1.0.2/betwatch/types/race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/examples/get_race_prices.py` & `betwatch-1.0.2/examples/get_race_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/examples/get_race_prices_async.py` & `betwatch-1.0.2/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/examples/get_races.py` & `betwatch-1.0.2/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/examples/get_races_async.py` & `betwatch-1.0.2/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/examples/subscriptions.py` & `betwatch-1.0.2/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/examples/update_rated_prices.py` & `betwatch-1.0.2/examples/update_rated_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/tests/test_get_race.py` & `betwatch-1.0.2/tests/test_get_race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/tests/test_get_race_async.py` & `betwatch-1.0.2/tests/test_get_race_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/tests/test_get_races.py` & `betwatch-1.0.2/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/tests/test_get_races_async.py` & `betwatch-1.0.2/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/.gitignore` & `betwatch-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/LICENSE.txt` & `betwatch-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/README.md` & `betwatch-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.1/pyproject.toml` & `betwatch-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "gql[aiohttp,websockets,requests]==3.5.0b3",
+    "gql[aiohttp,websockets,requests]==3.5.0b4",
     "typedload==2.22",
     "aiohttp==3.8.3",
     "python-dateutil==2.8.2",
     "urllib3>=1.26,<2",
 ]
 dynamic = ["version"]
```

### Comparing `betwatch-1.0.1/PKG-INFO` & `betwatch-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betwatch
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
 License-File: LICENSE.txt
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: aiohttp==3.8.3
-Requires-Dist: gql[aiohttp,requests,websockets]==3.5.0b3
+Requires-Dist: gql[aiohttp,requests,websockets]==3.5.0b4
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: typedload==2.22
 Requires-Dist: urllib3<2,>=1.26
 Description-Content-Type: text/markdown
 
 # Betwatch Python SDK
```

