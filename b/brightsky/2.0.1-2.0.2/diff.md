# Comparing `tmp/brightsky-2.0.1.tar.gz` & `tmp/brightsky-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightsky-2.0.1.tar", last modified: Wed Apr 12 18:00:52 2023, max compression
+gzip compressed data, was "brightsky-2.0.2.tar", last modified: Tue May  9 10:05:25 2023, max compression
```

## Comparing `brightsky-2.0.1.tar` & `brightsky-2.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:00:52.467195 brightsky-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 18:00:48.000000 brightsky-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-12 18:00:52.467195 brightsky-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-12 18:00:48.000000 brightsky-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:00:52.463195 brightsky-2.0.1/brightsky/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-12 18:00:48.000000 brightsky-2.0.1/brightsky/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:00:52.463195 brightsky-2.0.1/brightsky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-12 18:00:52.000000 brightsky-2.0.1/brightsky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-12 18:00:52.000000 brightsky-2.0.1/brightsky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:00:52.000000 brightsky-2.0.1/brightsky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 18:00:52.000000 brightsky-2.0.1/brightsky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 18:00:52.000000 brightsky-2.0.1/brightsky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 18:00:48.000000 brightsky-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:00:52.467195 brightsky-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-12 18:00:48.000000 brightsky-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:00:52.467195 brightsky-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-04-12 18:00:48.000000 brightsky-2.0.1/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:05:25.780775 brightsky-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-09 10:05:20.000000 brightsky-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-09 10:05:25.780775 brightsky-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-09 10:05:20.000000 brightsky-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:05:25.776775 brightsky-2.0.2/brightsky/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:05:25.776775 brightsky-2.0.2/brightsky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-09 10:05:25.000000 brightsky-2.0.2/brightsky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-09 10:05:25.000000 brightsky-2.0.2/brightsky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:05:25.000000 brightsky-2.0.2/brightsky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-09 10:05:25.000000 brightsky-2.0.2/brightsky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 10:05:25.000000 brightsky-2.0.2/brightsky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-09 10:05:20.000000 brightsky-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:05:25.780775 brightsky-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-09 10:05:20.000000 brightsky-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:05:25.780775 brightsky-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18743 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_web.py
```

### Comparing `brightsky-2.0.1/LICENSE` & `brightsky-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.1/PKG-INFO` & `brightsky-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.1
+Version: 2.0.2
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.1/README.md` & `brightsky-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.1/brightsky/cli.py` & `brightsky-2.0.2/brightsky/cli.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.1/brightsky/db.py` & `brightsky-2.0.2/brightsky/db.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.1/brightsky/export.py` & `brightsky-2.0.2/brightsky/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         INSERT INTO {weather_table} (timestamp, source_id, {fields})
         VALUES %s
         ON CONFLICT
             ON CONSTRAINT {constraint} DO UPDATE SET
                 {conflict_updates};
     """)
     UPDATE_WEATHER_CONFLICT_UPDATE = '{field} = EXCLUDED.{field}'
+    UPDATE_WEATHER_VALUES_TEMPLATE = '(%(timestamp)s, %(source_id)s, {values})'
     UPDATE_WEATHER_CLEANUP = None
     SOURCE_FIELDS = [
         'observation_type', 'lat', 'lon', 'height', 'dwd_station_id',
         'wmo_station_id', 'station_name']
     ELEMENT_FIELDS = [
         'cloud_cover',
         'condition',
@@ -85,15 +86,16 @@
             if fingerprint:
                 self.update_parsed_files(conn, fingerprint)
 
     def export_batch(self, conn, batch):
         records = self.prepare_records(batch)
         sources = self.prepare_sources(batch)
         source_map = self.update_sources(conn, sources)
-        self.update_weather(conn, source_map, records)
+        self.map_source_ids(records, source_map)
+        self.update_weather(conn, records)
 
     def prepare_records(self, records):
         return records
 
     def prepare_sources(self, records):
         sources = {}
         for r in records:
@@ -123,17 +125,19 @@
                 cur.execute(self.UPDATE_SOURCES_CLEANUP)
                 conn.commit()
         return {
             source_key: row['id']
             for row, source_key in zip(rows, sources)
         }
 
-    def update_weather(self, conn, source_map, records):
+    def map_source_ids(self, records, source_map):
         for r in records:
             r['source_id'] = source_map[r['source']]
+
+    def update_weather(self, conn, records):
         for fields, records in self.make_batches(records).items():
             logger.info(
                 "Exporting %d records with fields %s",
                 len(records), tuple(fields))
             stmt = self.UPDATE_WEATHER_STMT.format(
                 weather_table=sql.Identifier(self.WEATHER_TABLE),
                 constraint=sql.Identifier(f'{self.WEATHER_TABLE}_key'),
@@ -142,15 +146,15 @@
                 conflict_updates=sql.SQL(', ').join(
                     sql.SQL(self.UPDATE_WEATHER_CONFLICT_UPDATE).format(
                         field=sql.Identifier(f),
                         weather_table=sql.Identifier(self.WEATHER_TABLE))
                     for f in fields),
             )
             template = sql.SQL(
-                "(%(timestamp)s, %(source_id)s, {values})"
+                self.UPDATE_WEATHER_VALUES_TEMPLATE,
             ).format(
                 values=sql.SQL(', ').join(
                     sql.Placeholder(f) for f in fields),
             )
             with conn.cursor() as cur:
                 execute_values(cur, stmt, records, template, page_size=1000)
         if self.UPDATE_WEATHER_CLEANUP:
@@ -244,7 +248,28 @@
             if not base.get(k):
                 base[k] = v
         return base
 
     def update_weather(self, *args, **kwargs):
         with self.synop_update_lock:
             super().update_weather(*args, **kwargs)
+
+
+class RADOLANExporter(DBExporter):
+
+    WEATHER_TABLE = 'radar'
+    UPDATE_WEATHER_STMT = sql.SQL("""
+        INSERT INTO {weather_table} (timestamp, {fields})
+        VALUES %s
+        ON CONFLICT
+            ON CONSTRAINT {constraint} DO UPDATE SET
+                {conflict_updates};
+    """)
+    UPDATE_WEATHER_VALUES_TEMPLATE = '(%(timestamp)s, {values})'
+    ELEMENT_FIELDS = [
+        'precipitation_5',
+        'source',
+    ]
+
+    def export_batch(self, conn, batch):
+        records = self.prepare_records(batch)
+        self.update_weather(conn, records)
```

### Comparing `brightsky-2.0.1/brightsky/polling.py` & `brightsky-2.0.2/brightsky/polling.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 class DWDPoller:
 
     urls = [
         'https://opendata.dwd.de/weather/local_forecasts/mos/MOSMIX_L/'
         'all_stations/kml/',
         'https://opendata.dwd.de/weather/local_forecasts/mos/MOSMIX_S/'
         'all_stations/kml/',
+        'https://opendata.dwd.de/weather/radar/composite/rv/',
         'https://opendata.dwd.de/weather/weather_reports/synoptic/germany/'
         'json/',
         'https://opendata.dwd.de/weather/weather_reports/poi/',
     ] + [
         'https://opendata.dwd.de/climate_environment/CDC/observations_germany/'
         f'climate/hourly/{subfolder}/'
         for subfolder in [
```

### Comparing `brightsky-2.0.1/brightsky/query.py` & `brightsky-2.0.2/brightsky/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import datetime
 
+import numpy as np
 from dateutil.tz import tzutc
+from isal import isal_zlib as zlib
 
 from brightsky.db import fetch
 
 
 def _make_dicts(rows):
     return [dict(row) for row in rows]
 
@@ -189,14 +191,61 @@
     }
     return {
         'weather': _make_dicts(fetch(sql, params)),
         'sources': _make_dicts(sources_rows),
     }
 
 
+def radar(date, last_date=None, fmt='compressed', bbox=None):
+    if not last_date:
+        last_date = date + datetime.timedelta(hours=2)
+    sql = """
+        SELECT *
+        FROM radar
+        WHERE timestamp BETWEEN %(date)s AND %(last_date)s
+        ORDER BY timestamp
+        """
+    params = {
+        'date': date,
+        'last_date': last_date,
+    }
+    rows = fetch(sql, params)
+    if fmt == 'plain':
+        for row in rows:
+            row['precipitation_5'] = _load_radar(row['precipitation_5'], bbox)
+    elif fmt == 'bytes':
+        for row in rows:
+            row['precipitation_5'] = memoryview(
+                _load_radar(row['precipitation_5'], bbox),
+            )
+    elif fmt == 'compressed' and bbox:
+        for row in rows:
+            row['precipitation_5'] = zlib.compress(
+                _load_radar(row['precipitation_5'], bbox),
+            )
+    elif fmt != 'compressed':
+        raise ValueError("Unknown format: '%s'" % fmt)
+    return {
+        'radar': _make_dicts(rows),
+    }
+
+
+def _load_radar(raw, bbox, width=1100, height=1200):
+    precip = np.frombuffer(
+        zlib.decompress(raw),
+        dtype='i2',
+    ).reshape((height, width))
+    if bbox:
+        top, left, bottom, right = bbox
+        precip = precip[top:bottom+1, left:right+1]
+        # Arrays must be C-contiguous for orjson and zlib
+        precip = np.ascontiguousarray(precip).reshape(precip.shape)
+    return precip
+
+
 def sources(
         lat=None, lon=None, dwd_station_id=None, wmo_station_id=None,
         source_id=None, observation_types=None, max_dist=50000,
         ignore_type=False, date=None, last_date=None):
     select = "*"
     order_by = "observation_type"
     params = {
```

### Comparing `brightsky-2.0.1/brightsky/settings.py` & `brightsky-2.0.2/brightsky/settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.1/brightsky/tasks.py` & `brightsky-2.0.2/brightsky/tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,16 +60,18 @@
             'forecast': '3 hours',
             'current': '48 hours',
         },
         'synop': {
             'synop': '30 hours',
         },
     }
+    radar_expiry_interval = '6 hours'
     parsed_files_expiry_intervals = {
         '%/Z__C_EDZW_%': '1 week',
+        '%/DE1200_RV%': '1 week',
     }
     with get_connection() as conn:
         with conn.cursor() as cur:
             logger.info(
                 'Deleting expired weather records: %s', expiry_intervals)
             for table, table_expires in expiry_intervals.items():
                 for observation_type, interval in table_expires.items():
@@ -100,14 +102,25 @@
                         MAX(timestamp) AS last_record
                       FROM {table}
                       GROUP BY source_id
                     ) AS record_range
                     WHERE sources.id = record_range.source_id;
                     """)
                 conn.commit()
+            logger.info('Deleting expired radar records')
+            cur.execute(
+                """
+                DELETE FROM radar WHERE
+                    timestamp < current_timestamp - %s::interval;
+                """,
+                (radar_expiry_interval,),
+            )
+            conn.commit()
+            if cur.rowcount:
+                logger.info('Deleted %d outdated radar records', cur.rowcount)
             logger.info(
                 'Deleting expired parsed files: %s',
                 parsed_files_expiry_intervals)
             for filename, interval in parsed_files_expiry_intervals.items():
                 cur.execute(
                     """
                     DELETE FROM parsed_files WHERE
```

### Comparing `brightsky-2.0.1/brightsky/utils.py` & `brightsky-2.0.2/brightsky/utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.1/brightsky/web.py` & `brightsky-2.0.2/brightsky/web.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,45 @@
+import base64
 import importlib
 import sys
 from contextlib import contextmanager
+from functools import partial
 
 import falcon
+import orjson
 from dateutil.tz import gettz
 from dwdparse.units import convert_record, CONVERTERS
+from falcon import media
 from falcon.errors import HTTPInvalidParam
 from gunicorn.app.base import BaseApplication
 from gunicorn.util import import_app
 
 import brightsky
 from brightsky import query
+from brightsky.db import fetch
 from brightsky.settings import settings
 from brightsky.utils import parse_date, sunrise_sunset
 
 
 @contextmanager
 def convert_exceptions():
     try:
         yield
     except ValueError as e:
         raise falcon.HTTPBadRequest(description=str(e))
     except LookupError as e:
         raise falcon.HTTPNotFound(description=str(e))
 
 
+def orjson_encode_default(o):
+    if isinstance(o, (bytes, memoryview)):
+        return base64.b64encode(o).decode('ascii')
+    raise TypeError
+
+
 class BrightskyResource:
 
     ALLOWED_UNITS = ['si'] + list(CONVERTERS)
 
     def parse_location(self, req, required=False):
         lat = req.get_param_as_float(
             'lat', required=required, min_value=-90, max_value=90)
@@ -88,15 +99,14 @@
         return units
 
     def process_timestamp(self, row, key, timezone):
         if not row[key]:
             return
         if timezone:
             row[key] = row[key].astimezone(timezone)
-        row[key] = row[key].isoformat()
 
     def process_sources(self, sources, timezone=None):
         for source in sources:
             self.process_timestamp(source, 'first_record', timezone)
             self.process_timestamp(source, 'last_record', timezone)
 
 
@@ -203,14 +213,81 @@
             description = (
                 "Querying by lat/lon is not supported for the synop endpoint"
             )
             raise falcon.HTTPBadRequest(description=description)
         return query.synop(*args, **kwargs)
 
 
+class RadarResource(BrightskyResource):
+
+    ALLOWED_FORMATS = ['compressed', 'bytes', 'plain']
+
+    def on_get(self, req, resp):
+        fmt = self.parse_format(req)
+        if fmt == 'compressed':
+            # Prevent traefik from gzipping the pre-compressed content
+            resp.set_header('Content-Encoding', 'identity')
+        else:
+            self.force_compression(req)
+        if not req.get_param('date'):
+            date = fetch(
+                "select max(timestamp) - '3 hours'::interval from radar"
+            )[0][0]
+            print(date)
+            last_date = None
+        else:
+            date, last_date = self.parse_date_range(req)
+        timezone = self.parse_timezone(req)
+        if timezone:
+            if not date.tzinfo:
+                date = date.replace(tzinfo=timezone)
+            if last_date and not last_date.tzinfo:
+                last_date = last_date.replace(tzinfo=timezone)
+        bbox = self.parse_bbox(req)
+        with convert_exceptions():
+            result = query.radar(date, last_date=last_date, fmt=fmt, bbox=bbox)
+        for row in result['radar']:
+            self.process_timestamp(row, 'timestamp', timezone)
+        resp.media = result
+
+    def force_compression(self, req):
+        # traefik has no support for brotli or deflate
+        if 'gzip' not in req.headers.get('ACCEPT-ENCODING', ''):
+            description = (
+                "Requests to the radar endpoint with format 'plain' or "
+                "'bytes' must accept gzip encoding"
+            )
+            raise falcon.HTTPBadRequest(description=description)
+
+    def parse_format(self, req):
+        fmt = req.get_param('format', default='compressed').lower()
+        if fmt not in self.ALLOWED_FORMATS:
+            description = "'format' must be in %s" % (self.ALLOWED_FORMATS,)
+            raise falcon.HTTPBadRequest(description=description)
+        return fmt
+
+    def parse_bbox(self, req):
+        if bbox := req.get_param_as_list('bbox'):
+            if len(bbox) == 1 and ',' in bbox[0]:
+                # Request contained URL-encoded commas
+                bbox = bbox[0].split(',')
+            try:
+                if len(bbox) != 4:
+                    raise ValueError
+                bbox = [int(x) for x in bbox]
+                return bbox
+            except ValueError:
+                description = (
+                    "The 'bbox' parameter must be a comma-separated list of "
+                    "four integers: top, left, bottom, right (edges are "
+                    "inclusive)."
+                )
+                raise falcon.HTTPBadRequest(description=description)
+
+
 class SourcesResource(BrightskyResource):
 
     def on_get(self, req, resp):
         lat, lon = self.parse_location(req)
         max_dist = self.parse_max_dist(req)
         source_id, dwd_station_id, wmo_station_id = self.parse_source_ids(req)
         with convert_exceptions():
@@ -251,18 +328,26 @@
         expose_headers=cors_headers,
     )
 
 
 def make_app():
     app = falcon.App(middleware=[make_cors_middleware()])
     app.req_options.auto_parse_qs_csv = True
+    app.resp_options.media_handlers['application/json'] = media.JSONHandler(
+        dumps=partial(
+            orjson.dumps,
+            default=orjson_encode_default,
+            option=orjson.OPT_SERIALIZE_NUMPY,
+        ),
+    )
     app.add_route('/', StatusResource())
     app.add_route('/weather', WeatherResource())
     app.add_route('/current_weather', CurrentWeatherResource())
     app.add_route('/synop', SynopResource())
+    app.add_route('/radar', RadarResource())
     app.add_route('/sources', SourcesResource())
     return app
 
 
 app = make_app()
```

### Comparing `brightsky-2.0.1/brightsky/worker.py` & `brightsky-2.0.2/brightsky/worker.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.1/brightsky.egg-info/PKG-INFO` & `brightsky-2.0.2/brightsky.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.1
+Version: 2.0.2
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.1/brightsky.egg-info/SOURCES.txt` & `brightsky-2.0.2/brightsky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.1/setup.py` & `brightsky-2.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,17 @@
         'astral',
         'click',
         'coloredlogs',
         'dwdparse[lean]',
         'falcon>=3',
         'gunicorn',
         'huey',
+        'isal',
+        'numpy',
+        'orjson',
         'parsel',
         'psycopg2-binary',
         'python-dateutil',
         'redis',
         'requests',
         'sentry-sdk',
     ],
```

### Comparing `brightsky-2.0.1/tests/test_export.py` & `brightsky-2.0.2/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.1/tests/test_parsers.py` & `brightsky-2.0.2/tests/test_parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 import datetime
 
+import numpy as np
 from dateutil.tz import tzutc
+from isal import isal_zlib as zlib
 
 from brightsky.parsers import (
-    CloudCoverObservationsParser, CurrentObservationsParser,
-    DewPointObservationsParser, get_parser, MOSMIXParser,
-    PrecipitationObservationsParser, PressureObservationsParser,
-    SunshineObservationsParser, SYNOPParser, TemperatureObservationsParser,
-    VisibilityObservationsParser, WindGustsObservationsParser,
-    WindObservationsParser)
+    CloudCoverObservationsParser,
+    CurrentObservationsParser,
+    DewPointObservationsParser,
+    get_parser,
+    MOSMIXParser,
+    PrecipitationObservationsParser,
+    PressureObservationsParser,
+    RADOLANParser,
+    SunshineObservationsParser,
+    SYNOPParser,
+    TemperatureObservationsParser,
+    VisibilityObservationsParser,
+    WindGustsObservationsParser,
+    WindObservationsParser,
+)
 
 from .utils import is_subset, settings
 
 
 def test_mosmix_parser(data_dir):
     p = MOSMIXParser()
     records = list(p.parse(data_dir / 'MOSMIX_S.kmz'))
@@ -367,14 +378,34 @@
     p = PressureObservationsParser()
     records = list(p.parse(data_dir / 'observations_recent_P0_hist.zip'))
     # The actual reduced pressure deleted from the test observation file was
     # 1023.0 hPa
     assert records[4]['pressure_msl'] == 102260
 
 
+def test_radolan_parser(data_dir):
+    p = RADOLANParser()
+    records = list(p.parse(data_dir / 'DE1200_RV2305081330.tar.bz2'))
+    assert len(records) == 1
+    data = np.frombuffer(
+        zlib.decompress(records[0]['precipitation_5']),
+        dtype='i2',
+    )
+    assert len(data) == 1200 * 1100
+    assert sum(data) == 564030
+    assert len(np.where(data < 4096)[0]) == len(data)
+    assert data.reshape((1200, 1100))[1117:1122, 334:339].tolist() == [
+        [3, 5, 2, 1, 3],
+        [2, 3, 3, 0, 0],
+        [3, 4, 1, 0, 3],
+        [0, 8, 0, 0, 0],
+        [0, 0, 0, 0, 0],
+    ]
+
+
 def test_get_parser():
     synop_with_timestamp = (
         'Z__C_EDZW_20200617114802_bda01,synop_bufr_GER_999999_999999__MW_617'
         '.json.bz2')
     synop_latest = (
         'Z__C_EDZW_latest_bda01,synop_bufr_GER_999999_999999__MW_XXX.json.bz2')
     expected = {
@@ -386,13 +417,14 @@
         'stundenwerte_P0_00096_akt.zip': PressureObservationsParser,
         'stundenwerte_RR_00102_akt.zip': PrecipitationObservationsParser,
         'stundenwerte_SD_00125_akt.zip': SunshineObservationsParser,
         'stundenwerte_TD_01766.zip': DewPointObservationsParser,
         'stundenwerte_TU_00161_akt.zip': TemperatureObservationsParser,
         'stundenwerte_VV_00161_akt.zip': VisibilityObservationsParser,
         'MOSMIX_S_LATEST_240.kmz': MOSMIXParser,
+        'DE1200_RV2305081330.tar.bz2': RADOLANParser,
         'K611_-BEOB.csv': CurrentObservationsParser,
         synop_with_timestamp: SYNOPParser,
         synop_latest: None,
     }
     for filename, expected_parser in expected.items():
         assert get_parser(filename) is expected_parser
```

### Comparing `brightsky-2.0.1/tests/test_polling.py` & `brightsky-2.0.2/tests/test_polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.1/tests/test_settings.py` & `brightsky-2.0.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.1/tests/test_tasks.py` & `brightsky-2.0.2/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.1/tests/test_utils.py` & `brightsky-2.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.1/tests/test_web.py` & `brightsky-2.0.2/tests/test_web.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+import base64
 import datetime
+import zlib
 
 import falcon
+import numpy as np
 import pytest
 from dateutil.tz import tzutc
 
 import brightsky
-from brightsky.export import DBExporter, SYNOPExporter
+from brightsky.export import DBExporter, RADOLANExporter, SYNOPExporter
+from brightsky.parsers import RADOLANParser
 from brightsky.web import make_app
 
 from .utils import settings
 
 
 SOURCES = [
     # Ordered by their distance to (52, 7.6)
@@ -205,14 +209,20 @@
 
 
 @pytest.fixture
 def synop_data(db):
     SYNOPExporter().export(SYNOP_RECORDS)
 
 
+@pytest.fixture
+def radar_data(db, data_dir):
+    p = RADOLANParser()
+    RADOLANExporter().export(p.parse(data_dir / 'DE1200_RV2305081330.tar.bz2'))
+
+
 def test_sources_required_parameters(data, api):
     assert api.simulate_get('/sources').status_code == 400
     assert api.simulate_get('/sources?lat=52').status_code == 400
     assert api.simulate_get('/sources?lon=7.6').status_code == 400
     assert api.simulate_get('/sources?lat=52&lon=7.6').status_code == 200
     assert api.simulate_get('/sources?wmo_station_id=10315').status_code == 200
     assert api.simulate_get('/sources?dwd_station_id=01766').status_code == 200
@@ -433,14 +443,92 @@
         'sunshine_30': 26,
         'sunshine_60': 50,
     }
     for k, v in expected_weather.items():
         assert resp.json['weather'][k] == v, k
 
 
+def test_radar_response(radar_data, api):
+    resp = api.simulate_get('/radar?date=2023-05-08T11:30')
+    assert resp.status_code == 200
+    assert len(resp.json['radar']) == 1
+
+
+def _get_radar_data(api, fmt, bbox=False):
+    url = f'/radar?date=2023-05-08T13:30&format={fmt}'
+    if bbox:
+        url += '&bbox=1117,334,1121,338'
+    resp = api.simulate_get(url, headers={'Accept-Encoding': 'gzip'})
+    assert resp.status_code == 200
+    return resp.json['radar'][0]['precipitation_5']
+
+
+def _check_radar_data(data):
+    if len(data) == 5:
+        clip = data
+    else:
+        assert sum(sum(row) for row in data) == 564030
+        clip = [
+            row[334:339]
+            for row in data[1117:1122]
+        ]
+    assert clip == [
+        [3, 5, 2, 1, 3],
+        [2, 3, 3, 0, 0],
+        [3, 4, 1, 0, 3],
+        [0, 8, 0, 0, 0],
+        [0, 0, 0, 0, 0],
+    ]
+
+
+def test_radar_response_compressed(radar_data, api):
+    raw = _get_radar_data(api, 'compressed')
+    data = np.frombuffer(
+        zlib.decompress(base64.b64decode(raw)),
+        dtype='i2',
+    ).reshape(
+        (1200, 1100),
+    ).tolist()
+    _check_radar_data(data)
+    raw = _get_radar_data(api, 'compressed', bbox=True)
+    clip = np.frombuffer(
+        zlib.decompress(base64.b64decode(raw)),
+        dtype='i2',
+    ).reshape(
+        (5, 5),
+    ).tolist()
+    _check_radar_data(clip)
+
+
+def test_radar_response_bytes(radar_data, api):
+    raw = _get_radar_data(api, 'bytes')
+    data = np.frombuffer(
+        base64.b64decode(raw),
+        dtype='i2',
+    ).reshape(
+        (1200, 1100),
+    ).tolist()
+    _check_radar_data(data)
+    raw = _get_radar_data(api, 'bytes', bbox=True)
+    clip = np.frombuffer(
+        base64.b64decode(raw),
+        dtype='i2',
+    ).reshape(
+        (5, 5),
+    ).tolist()
+    _check_radar_data(clip)
+
+
+def test_radar_response_plain(radar_data, api):
+    data = _get_radar_data(api, 'plain')
+    _check_radar_data(data)
+    clip = _get_radar_data(api, 'plain', bbox=True)
+    _check_radar_data(clip)
+
+
 def test_status_response(api):
     resp = api.simulate_get('/')
     assert resp.status_code == 200
     assert resp.json['name'] == 'brightsky'
     assert resp.json['version'] == brightsky.__version__
     assert resp.json['status'] == 'ok'
```

