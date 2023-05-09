# Comparing `tmp/fastf1-3.0.1.tar.gz` & `tmp/fastf1-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastf1-3.0.1.tar", last modified: Sun May  7 21:37:40 2023, max compression
+gzip compressed data, was "fastf1-3.0.2.tar", last modified: Tue May  9 20:26:25 2023, max compression
```

## Comparing `fastf1-3.0.1.tar` & `fastf1-3.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-07 21:37:25.000000 fastf1-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 21:37:25.000000 fastf1-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-07 21:37:40.955927 fastf1-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-07 21:37:25.000000 fastf1-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.951927 fastf1-3.0.1/fastf1/
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68847 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/api.py
--rw-r--r--   0 runner    (1001) docker     (123)   132755 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/fastf1/ergast/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/ergast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61147 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/ergast/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/ergast/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/ergast/sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/ergast/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    38668 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/fastf1/livetiming/
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/livetiming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/livetiming/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/livetiming/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/livetiming/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    24975 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/req.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/fastf1/signalr_aio/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/fastf1/signalr_aio/events/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/events/_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/fastf1/signalr_aio/hubs/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/hubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/hubs/_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/fastf1/signalr_aio/transports/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/transports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/transports/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/transports/_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/transports/_queue_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/transports/_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.951927 fastf1-3.0.1/fastf1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-07 21:37:40.000000 fastf1-3.0.1/fastf1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-07 21:37:40.000000 fastf1-3.0.1/fastf1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:37:40.000000 fastf1-3.0.1/fastf1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:37:40.000000 fastf1-3.0.1/fastf1.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-07 21:37:40.000000 fastf1-3.0.1/fastf1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 21:37:40.000000 fastf1-3.0.1/fastf1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-07 21:37:25.000000 fastf1-3.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-07 21:37:40.955927 fastf1-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 21:37:25.000000 fastf1-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 20:26:14.000000 fastf1-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-09 20:26:14.000000 fastf1-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-09 20:26:25.394238 fastf1-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-09 20:26:14.000000 fastf1-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.390237 fastf1-3.0.2/fastf1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68847 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136190 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/fastf1/ergast/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/ergast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61147 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/ergast/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/ergast/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/ergast/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/ergast/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39069 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/fastf1/livetiming/
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/livetiming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/livetiming/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/livetiming/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/livetiming/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/req.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/fastf1/signalr_aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/fastf1/signalr_aio/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/events/_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/fastf1/signalr_aio/hubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/hubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/hubs/_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/fastf1/signalr_aio/transports/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/transports/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/transports/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/transports/_queue_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/transports/_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-09 20:26:15.000000 fastf1-3.0.2/fastf1/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 20:26:15.000000 fastf1-3.0.2/fastf1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.390237 fastf1-3.0.2/fastf1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-09 20:26:25.000000 fastf1-3.0.2/fastf1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-09 20:26:25.000000 fastf1-3.0.2/fastf1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:26:25.000000 fastf1-3.0.2/fastf1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:26:25.000000 fastf1-3.0.2/fastf1.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-09 20:26:25.000000 fastf1-3.0.2/fastf1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 20:26:25.000000 fastf1-3.0.2/fastf1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-09 20:26:15.000000 fastf1-3.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-09 20:26:25.394238 fastf1-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 20:26:15.000000 fastf1-3.0.2/setup.py
```

### Comparing `fastf1-3.0.1/LICENSE` & `fastf1-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/README.md` & `fastf1-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/__init__.py` & `fastf1-3.0.2/fastf1/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/_api.py` & `fastf1-3.0.2/fastf1/_api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/api.py` & `fastf1-3.0.2/fastf1/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/core.py` & `fastf1-3.0.2/fastf1/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,17 @@
      [5, 'VET', 'Aston Martin'], [18, 'STR', 'Aston Martin'],
      [14, 'ALO', 'Alpine'], [31, 'OCO', 'Alpine'],
      [22, 'TSU', 'AlphaTauri'], [10, 'GAS', 'AlphaTauri'],
      [47, 'MSC', 'Haas F1 Team'], [9, 'MAZ', 'Haas F1 Team'],
      [7, 'RAI', 'Alfa Romeo'], [99, 'GIO', 'Alfa Romeo'],
      [6, 'LAT', 'Williams'], [63, 'RUS', 'Williams']]
 
+_RACE_LIKE_SESSIONS = ('Race', 'Sprint', 'Sprint Qualifying')
+_QUALI_LIKE_SESSIONS = ('Qualifying', 'Sprint Shootout')
+
 
 class Telemetry(pd.DataFrame):
     """Multi-channel time series telemetry data
 
     The object can contain multiple telemetry channels. Multiple telemetry
     objects with different channels can be merged on time. Each telemetry
     channel is one dataframe column. Partial telemetry (e.g. for one lap only)
@@ -1233,14 +1236,15 @@
                     "Cannot load laps, telemetry, weather, and message data "
                     "because the relevant API is not supported for this "
                     "session."
                 )
 
         self._fix_missing_laps_retired_on_track()
         self._set_laps_deleted_from_rcm()
+        self._calculate_quali_like_session_results()
 
         _logger.info(f"Finished loading data for {len(self.drivers)} "
                      f"drivers: {self.drivers}")
 
     @soft_exceptions("lap timing data", "Failed to load timing data!", _logger)
     def _load_laps_data(self, livedata=None):
         data, _ = api.timing_data(self.api_path, livedata=livedata)
@@ -1277,16 +1281,15 @@
             if d2.shape[0] != len(d2['Stint'].unique()):
                 # tyre info includes correction messages that need to be
                 # applied before continuing
                 d2 = self.__fix_tyre_info(d2)
 
             is_generated = False
             if not len(d1):
-                if ((self.name in ('Race', 'Sprint', 'Sprint Qualifying'))
-                        and len(d2)):
+                if self.name in _RACE_LIKE_SESSIONS and len(d2):
                     # add data for drivers who crashed on the very first lap
                     # as a downside, this potentially adds a nonexistent lap
                     # for drivers who could not start the race
                     is_generated = True
                     result = d1.copy()
                     result['Driver'] = [driver, ]
                     result['NumberOfLaps'] = 0
@@ -1315,15 +1318,15 @@
             # add flag that indicates if the data for this lap was generated
             # by FastF1
             result['FastF1Generated'] = is_generated
 
             # calculate lap start time by setting it to the 'Time' of the
             # previous lap
             laps_start_time = list(result['Time'])[:-1]
-            if self.name in ('Race', 'Sprint', 'Sprint Qualifying'):
+            if self.name in _RACE_LIKE_SESSIONS:
                 # assumption that the first lap started when the session was
                 # started can only be made for the race
                 laps_start_time.insert(0, self.session_start_time)
             else:
                 laps_start_time.insert(0, pd.NaT)
             laps_start_time = pd.Series(laps_start_time)
 
@@ -1341,16 +1344,15 @@
                         try:
                             restart_index = result.loc[
                                 result['PitOutTime'] > row['Time'],
                                 'PitOutTime'
                             ].index[0]
                         except IndexError:
                             continue  # no pit out, car did not restart
-                        if self.name in ('Sprint Qualifying', 'Sprint',
-                                         'Race'):
+                        if self.name in _RACE_LIKE_SESSIONS:
                             # if this is a race-like session, we can assume the
                             # session restart time as lap start time
                             laps_start_time[restart_index] = row['Time']
                         else:
                             # for other sessions, we cannot make this
                             # assumption set to NaT here, it will be set to
                             # PitOutTime later if possible
@@ -1391,15 +1393,15 @@
         laps['Team'] = laps['DriverNumber'].map(t_map)
         d_map = {r['DriverNumber']: r['Abbreviation']
                  for _, r in self.results.iterrows()}
         laps['Driver'] = laps['DriverNumber'].map(d_map)
 
         # add Position based on lap timing
         laps['Position'] = np.NaN  # create empty column
-        if self.name in ('Race', 'Sprint', 'Sprint Qualifying'):
+        if self.name in _RACE_LIKE_SESSIONS:
             for lap_n in laps['LapNumber'].unique():
                 # get each drivers lap for the current lap number, sorted by
                 # the time when each lap was set
                 laps_eq_n = laps.loc[
                     laps['LapNumber'] == lap_n, ('Time', 'Position')
                 ].reset_index(drop=True).sort_values(by='Time')
 
@@ -1409,14 +1411,18 @@
                     = laps_eq_n.sort_index()['Position'].to_list()
 
         self._add_track_status_to_laps(laps)
 
         self._laps = Laps(laps, session=self, force_default_cols=True)
         self._check_lap_accuracy()
 
+    @soft_exceptions("generate retired laps",
+                     "Failed to generate last laps for drivers that retired"
+                     "on track!",
+                     _logger)
     def _fix_missing_laps_retired_on_track(self):
         # generate a last lap entry with assumed end time for cars that
         # retired on track
 
         if not hasattr(self, '_laps'):
             return
 
@@ -1525,14 +1531,17 @@
 
         if any_new:
             # re-sort and re-index to restore correct order of the laps
             self._laps = self._laps \
                 .sort_values(by=['DriverNumber', 'LapNumber']) \
                 .reset_index(drop=True)
 
+    @soft_exceptions("mark deleted laps from RCM",
+                     "Failed to find deleted laps from race control messages!",
+                     _logger)
     def _set_laps_deleted_from_rcm(self):
         # parse race control messages to find deleted lap times and
         # set the 'Deleted' flag in self._laps
 
         if ((not hasattr(self, '_laps'))
                 or (not hasattr(self, '_race_control_messages'))):
             return
@@ -1555,14 +1564,68 @@
                 reason = timestamp_pattern.sub("", match[3])
                 self._laps.loc[
                     (self._laps['DriverNumber'] == drv)
                     & (self._laps['LapTime'] == deleted_time),
                     ('Deleted', 'IsPersonalBest', 'DeletedReason')
                 ] = (True, False, reason)
 
+    @soft_exceptions("quali results",
+                     "Failed to calculate quali results from lap times!",
+                     _logger)
+    def _calculate_quali_like_session_results(self, force=False):
+        """Try to calculate quali results from lap times if no results are
+        available
+
+        Args:
+            force (bool): Force calculation of quali results even if
+            results are already available, (default: False)"""
+
+        if self.name not in _QUALI_LIKE_SESSIONS:
+            return
+
+        if not hasattr(self, '_laps'):
+            return
+
+        if not self.results['Position'].isna().all() and not force:
+            # Don't do anything if results are already available
+            # unless force is True
+            return
+
+        quali_results = (self._laps.loc[:, ['DriverNumber']].copy()
+                         .drop_duplicates()
+                         .reset_index(drop=True))
+        sessions = self._laps.pick_quicklaps().split_qualifying_sessions()
+
+        for i, session in enumerate(sessions):
+            session_name = f'Q{i + 1}'
+            if session is not None:
+                laps = (
+                    session[~session['LapTime'].isna() & ~session['Deleted']]
+                    .copy()
+                    .groupby(['DriverNumber'])
+                    .agg({'LapTime': 'min'})
+                    .rename(columns={'LapTime': session_name})
+                )
+
+                quali_results = (quali_results
+                                 .merge(laps, on='DriverNumber', how='left'))
+            else:
+                quali_results[session_name] = pd.NaT
+
+        quali_results = (quali_results.sort_values(by=['Q3', 'Q2', 'Q1'])
+                         .reset_index())
+        quali_results['Position'] = quali_results.index + 1
+        quali_results = quali_results.set_index('DriverNumber', drop=True)
+
+        self.results.update(quali_results, overwrite=force)
+        self.results.sort_values(by=['Position'], inplace=True)
+
+    @soft_exceptions("add track status to laps",
+                     "Failed to add track status to Laps!",
+                     _logger)
     def _add_track_status_to_laps(self, laps):
         # add track status information to each lap
 
         track_status = getattr(self, '_track_status')
         if track_status is None:
             return
 
@@ -1668,15 +1731,15 @@
                             "information!")
 
     @soft_exceptions("total lap count", "Failed to load total lap count!",
                      _logger)
     def _load_total_lap_count(self, livedata=None):
         # Get the number of originally scheduled laps
         # Lap count data only exists for race-like sessions.
-        if self.name in ('Race', 'Sprint', 'Sprint Qualifying'):
+        if self.name in _RACE_LIKE_SESSIONS:
             try:
                 lap_count = api.lap_count(self.api_path, livedata=livedata)
                 # A race-like session can have multiple intended total laps,
                 # the first one being the original schedule
                 self._total_laps = lap_count['TotalLaps'][0]
             except IndexError:
                 self._total_laps = None
@@ -1733,14 +1796,17 @@
 
         # reapply original dtypes per column
         for col_name, dtype in zip(df.columns, df.dtypes):
             corrected[col_name] = corrected[col_name].astype(dtype)
 
         return corrected
 
+    @soft_exceptions("lap accuracy check",
+                     "Failed to perform lap accuracy check!",
+                     _logger)
     def _check_lap_accuracy(self):
         """Accuracy validation; simples yes/no validation
         Currently only relies on provided information which can't catch all problems"""
         # TODO: check for outliers in lap start position
         for drv in self.drivers:
             is_accurate = list()
             prev_lap = None
@@ -1871,45 +1937,54 @@
                                        driver_info['LastName']):
                     driver_info['FullName'].append(f"{first} {last}")
         return driver_info
 
     def _drivers_results_from_ergast(
             self, *, load_drivers=False, load_results=False
     ) -> Optional[pd.DataFrame]:
-        if self.name in ('Qualifying', 'Sprint Qualifying', 'Sprint', 'Race'):
+        if self.name in _RACE_LIKE_SESSIONS + _QUALI_LIKE_SESSIONS:
             session_name = self.name
         else:
             # this is a practice session, use drivers from race session but
             # don't load results
             session_name = 'Race'
             load_results = False
 
         @soft_exceptions("ergast result data",
-                         "Failed to load result data from Ergast! (This is "
-                         "expected for recent sessions)",
+                         "Failed to load result data from Ergast!",
                          _logger)
         def _get_data():
             if session_name == 'Race':
                 return self._ergast.get_race_results(
                     self.event.year, self.event.RoundNumber
-                ).content[0]
+                )
             elif session_name == 'Qualifying':
                 return self._ergast.get_qualifying_results(
                     self.event.year, self.event.RoundNumber
-                ).content[0]
-            else:
+                )
+            elif session_name in ('Sprint', 'Sprint Qualifying'):
                 return self._ergast.get_sprint_results(
                     self.event.year, self.event.RoundNumber
-                ).content[0]
-
-        data = _get_data()
-
-        if data is None:
+                )
+            else:
+                # TODO: Use Ergast when/if it supports sprint shootout sessions
+                # return self._ergast.get_sprint_shootout_results(
+                #     self.event.year, self.event.RoundNumber
+                # )
+                return None
+
+        response = _get_data()
+
+        if not response or not response.content:
+            _logger.warning("No result data for this session available on "
+                            "Ergast! (This is expected for recent sessions)")
             return None
 
+        data = response.content[0]
+
         rename_return = {
             'number': 'DriverNumber',
             'driverId': 'DriverId',
             'constructorId': 'TeamId'
         }
 
         if load_drivers:
@@ -1921,24 +1996,24 @@
             })
 
         if load_results:
             rename_return.update({
                 'position': 'Position',
             })
 
-            if session_name in ('Sprint Qualifying', 'Sprint', 'Race'):
+            if session_name in _RACE_LIKE_SESSIONS:
                 rename_return.update({
                     'positionText': 'ClassifiedPosition',
                     'grid': 'GridPosition',
                     'status': 'Status',
                     'points': 'Points',
                     'totalRaceTime': 'Time'
                 })
 
-            if session_name == 'Qualifying':
+            if session_name in _QUALI_LIKE_SESSIONS:
                 rename_return.update({
                     'Q1': 'Q1',
                     'Q2': 'Q2',
                     'Q3': 'Q3',
                 })
 
         d = data.loc[:, list(rename_return.keys())] \
@@ -2153,16 +2228,16 @@
         - **TrackStatus** (str): A string that contains track status numbers
           for all track status that occurred
           during this lap. The meaning of the track status numbers is
           explained in :func:`fastf1.api.track_status_data`.
           For filtering laps by track status, you may want to use
           :func:`Laps.pick_track_status`.
         - **Position** (float): Position of the driver at the end of each lap.
-          This value is NaN for FP1, FP2, FP3 and Qualifying as well as for
-          crash laps.
+          This value is NaN for FP1, FP2, FP3, Sprint Shootout, and Qualifying
+          as well as for crash laps.
         - **Deleted** (Optional[bool]): Indicates that a lap was deleted by
           the stewards, for example because of a track limits violation.
           This data is only available when race control messages are loaded.
         - **DeletedReason** (str): Gives the reason for a lap time deletion.
           This data is only available when race control messages are loaded.
         - **FastF1Generated** (bool): Indicates that this lap was added by
           FastF1. Such a lap will generally have very limited information
@@ -2671,35 +2746,39 @@
 
             q1, q2, q3 = laps.split_qualifying_sessions()
 
         Returns: Three :class:`Laps` objects, one for Q1, Q2 and Q3
             each. If any of these sessions was cancelled, ``None`` will be
             returned instead of :class:`Laps`.
         """
-        if self.session.name != "Qualifying":
+        if self.session.name not in _QUALI_LIKE_SESSIONS:
             raise ValueError("Session is not a qualifying session!")
         elif self.session.session_status is None:
             raise ValueError("Session status data is unavailable!")
 
         # get the timestamps for 'Started' from the session status data
-        # note that after a red flag, a session is 'Started' as well.
+        # note that after a red flag, a session can be 'Started' as well.
         # Therefore, it is necessary to check for red flags and ignore
         # the first 'Started' entry after a red flag.
         split_times = list()
         session_suspended = False
         for _, row in self.session.session_status.iterrows():
             if row['Status'] == 'Started':
                 if not session_suspended:
                     split_times.append(row['Time'])
                 else:
                     session_suspended = False
             elif row['Status'] == 'Aborted':
                 session_suspended = True
+            elif row['Status'] == 'Finished':
+                # This handles the case when a qualifying session isn't
+                # restarted after a red flag.
+                session_suspended = False
 
-        # at the very last timestamp, to get an end for the last interval
+        # add the very last timestamp, to get an end for the last interval
         split_times.append(self.session.session_status['Time'].iloc[-1])
 
         laps = [None, None, None]
         for i in range(len(split_times) - 1):
             laps[i] = self[(self['Time'] > split_times[i])
                            & (self['Time'] < split_times[i + 1])]
         return laps
@@ -2935,49 +3014,51 @@
           The URL to the driver's headshot
 
         - ``CountryCode`` | :class:`str` |
           The driver's country code (e.g. "FRA")
 
         - ``Position`` | :class:`float` |
           The drivers finishing position (values only given if session is
-          'Race', 'Qualifying' or 'Sprint Qualifying').
+          'Race', 'Qualifying', 'Sprint Shootout', 'Sprint', or
+          'Sprint Qualifying').
 
         - ``ClassifiedPosition`` | :class:`str` |
           The official classification result for each driver.
           This is either an integer value if the driver is
           officially classified or one of "R" (retired), "D" (disqualified),
           "E" (excluded), "W" (withdrawn), "F" (failed to qualify) or
           "N" (not classified).
 
         - ``GridPosition`` | :class:`float` |
           The drivers starting position (values only given if session is
-          'Race' or 'Sprint Qualifying')
+          'Race', 'Sprint', or 'Sprint Qualifying')
 
         - ``Q1`` | :class:`pd.Timedelta` |
           The drivers best Q1 time (values only given if session is
-          'Qualifying')
+          'Qualifying' or 'Sprint Shootout')
 
         - ``Q2`` | :class:`pd.Timedelta` |
           The drivers best Q2 time (values only given if session is
-          'Qualifying')
+          'Qualifying' or 'Sprint Shootout')
 
         - ``Q3`` | :class:`pd.Timedelta` |
           The drivers best Q3 time (values only given if session is
-          'Qualifying')
+          'Qualifying' or 'Sprint Shootout')
 
         - ``Time`` | :class:`pd.Timedelta` |
           The drivers total race time (values only given if session is
-          'Race' or 'Sprint Qualifying' and the driver was not more than one
-          lap behind the leader)
+          'Race', 'Sprint', or 'Sprint Qualifying' and the driver was not
+          more than one lap behind the leader)
 
         - ``Status`` | :class:`str` |
           A status message to indicate if and how the driver finished the race
           or to indicate the cause of a DNF. Possible values include but are
           not limited to 'Finished', '+ 1 Lap', 'Crash', 'Gearbox', ...
-          (values only given if session is 'Race' or 'Sprint Qualifying')
+          (values only given if session is 'Race', 'Sprint', or
+          'Sprint Qualifying')
 
         - ``Points`` | :class:`float` |
           The number of points received by each driver for their finishing
           result.
 
     By default, the session results are indexed by driver number and sorted by
     finishing position.
```

### Comparing `fastf1-3.0.1/fastf1/ergast/interface.py` & `fastf1-3.0.2/fastf1/ergast/interface.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/ergast/legacy.py` & `fastf1-3.0.2/fastf1/ergast/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/ergast/sphinx.py` & `fastf1-3.0.2/fastf1/ergast/sphinx.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/ergast/structure.py` & `fastf1-3.0.2/fastf1/ergast/structure.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/events.py` & `fastf1-3.0.2/fastf1/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
 
 
 Event Schedule
 ..............
 
 - 'conventional': Practice 1, Practice 2, Practice 3, Qualifying, Race
 - 'sprint': Practice 1, Qualifying, Practice 2, Sprint, Race
+- 'sprint_shootout': Practice 1, Qualifying, Sprint Shootout, Sprint, Race
 - 'testing': no fixed session order; usually three practice sessions on
   three separate days
 
 
 .. _SessionIdentifier:
 
 Session identifiers
@@ -612,15 +613,18 @@
         # number of events, usually 3 for testing, 5 for race weekends
         # in special cases there are additional unrelated events
 
         if (n_events >= 4) and ('Sprint' in event['Sessions'][3]['Name']):
             if event['Sessions'][3]['Name'] == 'Sprint Qualifying':
                 # fix for 2021 where Sprint was called Sprint Qualifying
                 event['Sessions'][3]['Name'] = 'Sprint'
-            data['EventFormat'].append('sprint')
+            if event['Sessions'][2]['Name'] == 'Sprint Shootout':
+                data['EventFormat'].append('sprint_shootout')
+            else:
+                data['EventFormat'].append('sprint')
             data['RoundNumber'].append(event['Number'])
         elif 'test' in event['Name'].lower():
             data['EventFormat'].append('testing')
             data['RoundNumber'].append(0)
         else:
             data['EventFormat'].append('conventional')
             data['RoundNumber'].append(event['Number'])
@@ -678,22 +682,25 @@
                 f"{rnd.get('date', '')}T{rnd.get('time', '')}",
             ).tz_localize(None)
         except dateutil.parser.ParserError:
             date = pd.NaT
         data['EventDate'].append(date)
 
         if 'Sprint' in rnd:
-            data['EventFormat'].append("sprint")
+            # Ergast doesn't support sprint shootout format yet
+            data['EventFormat'].append(
+                "sprint_shootout" if year == 2023 else "sprint")
             data['Session1'].append('Practice 1')
             data['Session1DateUtc'].append(
                 date.floor('D') - pd.Timedelta(days=2))
             data['Session2'].append('Qualifying')
             data['Session2DateUtc'].append(
                 date.floor('D') - pd.Timedelta(days=2))
-            data['Session3'].append('Practice 2')
+            data['Session3'].append(
+                'Sprint Shootout' if year == 2023 else 'Practice 2')
             data['Session3DateUtc'].append(
                 date.floor('D') - pd.Timedelta(days=1))
             data['Session4'].append('Sprint')
             data['Session4DateUtc'].append(
                 date.floor('D') - pd.Timedelta(days=1))
             data['Session5'].append('Race')
             data['Session5DateUtc'].append(date)
```

### Comparing `fastf1-3.0.1/fastf1/legacy.py` & `fastf1-3.0.2/fastf1/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/livetiming/__init__.py` & `fastf1-3.0.2/fastf1/livetiming/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/livetiming/__main__.py` & `fastf1-3.0.2/fastf1/livetiming/__main__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/livetiming/client.py` & `fastf1-3.0.2/fastf1/livetiming/client.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/livetiming/data.py` & `fastf1-3.0.2/fastf1/livetiming/data.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/logger.py` & `fastf1-3.0.2/fastf1/logger.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/plotting.py` & `fastf1-3.0.2/fastf1/plotting.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/req.py` & `fastf1-3.0.2/fastf1/req.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,16 @@
 
     _requests_session_cached: Optional[_CachedSessionWithRateLimiting] = None
     _requests_session: requests.Session = _SessionWithRateLimiting()
     _default_cache_enabled = False  # flag to ensure that warning about disabled cache is logged once only # noqa: E501
     _tmp_disabled = False
     _ci_mode = False
 
+    _request_counter = 0  # count uncached requests for debugging purposes
+
     @classmethod
     def enable_cache(
             cls, cache_dir: str, ignore_version: bool = False,
             force_renew: bool = False,
             use_requests_cache: bool = True):
         """Enables the API cache.
 
@@ -258,47 +260,51 @@
         All GET requests that require caching should be performed through this
         wrapper. Caching will be done if the module-wide cache has been
         enabled. Else, `requests.Session().get()` will be called without any
         caching.
         """
         cls._enable_default_cache()
         if (cls._requests_session_cached is None) or cls._tmp_disabled:
+            cls._request_counter += 1
             return cls._requests_session.get(*args, **kwargs)
 
         if cls._ci_mode:
             # try to return a cached response first
             resp = cls._requests_session_cached.get(
                 *args, only_if_cached=True, **kwargs)
             # 504 indicates that no cached response was found
             if resp.status_code != 504:
                 return resp
 
+        cls._request_counter += 1
         return cls._requests_session_cached.get(*args, **kwargs)
 
     @classmethod
     def requests_post(cls, *args, **kwargs):
         """Wraps `requests.Session().post()` with caching if enabled.
 
         All POST requests that require caching should be performed through this
         wrapper. Caching will be done if the module-wide cache has been
         enabled. Else, `requests.Session().get()` will be called without any
         caching.
         """
         cls._enable_default_cache()
         if (cls._requests_session_cached is None) or cls._tmp_disabled:
+            cls._request_counter += 1
             return cls._requests_session.post(*args, **kwargs)
 
         if cls._ci_mode:
             # try to return a cached response first
             resp = cls._requests_session_cached.post(
                 *args, only_if_cached=True, **kwargs)
             # 504 indicates that no cached response was found
             if resp.status_code != 504:
                 return resp
 
+        cls._request_counter += 1
         return cls._requests_session_cached.post(*args, **kwargs)
 
     @classmethod
     def delete_response(cls, url):
         """Deletes a single cached response from the cache, if caching is
         enabled. If caching is not enabled, this call is ignored."""
         if cls._requests_session_cached is not None:
```

### Comparing `fastf1-3.0.1/fastf1/signalr_aio/_connection.py` & `fastf1-3.0.2/fastf1/signalr_aio/_connection.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/signalr_aio/hubs/_hub.py` & `fastf1-3.0.2/fastf1/signalr_aio/hubs/_hub.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/signalr_aio/transports/_parameters.py` & `fastf1-3.0.2/fastf1/signalr_aio/transports/_parameters.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/signalr_aio/transports/_transport.py` & `fastf1-3.0.2/fastf1/signalr_aio/transports/_transport.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1/utils.py` & `fastf1-3.0.2/fastf1/utils.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/fastf1.egg-info/SOURCES.txt` & `fastf1-3.0.2/fastf1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.1/setup.cfg` & `fastf1-3.0.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 name = fastf1
 license = MIT
 license_files = LICENSE
 author = Oehrly
 author_email = oehrly@mailbox.org
 home_page = https://github.com/theOehrly/Fast-F1
 description = Wrapper library for F1 data and telemetry API with additional data processing capabilities.
-long_description = file: README.rst
-long_description_content_type = text/x-rst
+long_description = file: README.md
+long_description_content_type = text/markdown
 
 [options]
 zip_safe = False
 packages = 
 	fastf1
 	fastf1.ergast
 	fastf1.livetiming
```

