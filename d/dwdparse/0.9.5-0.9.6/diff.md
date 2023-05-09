# Comparing `tmp/dwdparse-0.9.5.tar.gz` & `tmp/dwdparse-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwdparse-0.9.5.tar", last modified: Wed Apr 12 17:51:02 2023, max compression
+gzip compressed data, was "dwdparse-0.9.6.tar", last modified: Tue May  9 09:40:23 2023, max compression
```

## Comparing `dwdparse-0.9.5.tar` & `dwdparse-0.9.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:51:02.405815 dwdparse-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 17:50:54.000000 dwdparse-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-12 17:51:02.405815 dwdparse-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-12 17:50:54.000000 dwdparse-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:51:02.405815 dwdparse-0.9.5/dwdparse/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28182 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/stations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 17:50:54.000000 dwdparse-0.9.5/dwdparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:51:02.405815 dwdparse-0.9.5/dwdparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-12 17:51:02.000000 dwdparse-0.9.5/dwdparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-12 17:51:02.000000 dwdparse-0.9.5/dwdparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:51:02.000000 dwdparse-0.9.5/dwdparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 17:51:02.000000 dwdparse-0.9.5/dwdparse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 17:51:02.000000 dwdparse-0.9.5/dwdparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 17:51:02.000000 dwdparse-0.9.5/dwdparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-12 17:50:54.000000 dwdparse-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:51:02.405815 dwdparse-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-12 17:50:54.000000 dwdparse-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:51:02.405815 dwdparse-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-04-12 17:50:54.000000 dwdparse-0.9.5/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-12 17:50:54.000000 dwdparse-0.9.5/tests/test_stations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-12 17:50:54.000000 dwdparse-0.9.5/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:23.789290 dwdparse-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-09 09:40:16.000000 dwdparse-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-09 09:40:23.789290 dwdparse-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-09 09:40:16.000000 dwdparse-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:23.789290 dwdparse-0.9.6/dwdparse/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30696 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:23.789290 dwdparse-0.9.6/dwdparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-09 09:40:23.000000 dwdparse-0.9.6/dwdparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-09 09:40:23.000000 dwdparse-0.9.6/dwdparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:40:23.000000 dwdparse-0.9.6/dwdparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 09:40:23.000000 dwdparse-0.9.6/dwdparse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 09:40:23.000000 dwdparse-0.9.6/dwdparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 09:40:23.000000 dwdparse-0.9.6/dwdparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-09 09:40:16.000000 dwdparse-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:40:23.789290 dwdparse-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-09 09:40:16.000000 dwdparse-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:23.789290 dwdparse-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-05-09 09:40:16.000000 dwdparse-0.9.6/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-09 09:40:16.000000 dwdparse-0.9.6/tests/test_stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-09 09:40:16.000000 dwdparse-0.9.6/tests/test_units.py
```

### Comparing `dwdparse-0.9.5/LICENSE` & `dwdparse-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.5/PKG-INFO` & `dwdparse-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwdparse
-Version: 0.9.5
+Version: 0.9.6
 Summary: Parsers for DWD's open weather data.
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/
 Project-URL: Tracker, https://github.com/jdemaeyer/dwdparse/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dwdparse Version: 0.9.5 Summary: Parsers for DWD's
+Metadata-Version: 2.1 Name: dwdparse Version: 0.9.6 Summary: Parsers for DWD's
 open weather data. Author: Jakob de Maeyer Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/ Project-URL:
 Tracker, https://github.com/jdemaeyer/dwdparse/issues/ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: lean License-File:
 LICENSE # dwdparse [![Build Status](https://img.shields.io/github/actions/
```

### Comparing `dwdparse-0.9.5/README.md` & `dwdparse-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.5/dwdparse/api.py` & `dwdparse-0.9.6/dwdparse/api.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.5/dwdparse/cli.py` & `dwdparse-0.9.6/dwdparse/cli.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.5/dwdparse/parsers.py` & `dwdparse-0.9.6/dwdparse/parsers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import array
 import bz2
 import csv
 import datetime
 import io
 import itertools
 import json
 import logging
 import re
+import sys
+import tarfile
 import xml.etree.ElementTree as ET
 import zipfile
 from contextlib import suppress
 
 from dwdparse.stations import (
     dwd_id_to_wmo,
     wmo_id_to_dwd,
@@ -771,16 +774,91 @@
             'height': height,
             'station_name': station_name,
             'timestamp': timestamp,
             'solar': solar,
         }
 
 
+class RADOLANParser(Parser):
+
+    PRODUCT = 'RV'
+    WMO_ID = '10000'  # WMO ID for composite products
+    HEIGHT = 1200
+    WIDTH = 1100
+    INTERVAL = 5
+    PRECISION = 'E-02'
+
+    def parse(self, path):
+        with tarfile.open(path, 'r:bz2') as tar:
+            for filename in sorted(tar.getnames()):
+                yield self.parse_single(tar.extractfile(filename))
+
+    def parse_single(self, f):
+        product, timestamp, offset = self.parse_header(f)
+        data = self.parse_data(f)
+        return {
+            'observation_type': 'radar',
+            'source': f'RADOLAN::{product}::{timestamp.isoformat()}',
+            'timestamp': timestamp + offset,
+            **data,
+        }
+
+    def parse_header(self, f):
+        header = ''
+        while (ch := f.read(1)) != b'\x03':
+            header += ch.decode()
+        # Product type
+        product = header[:2]
+        assert product == self.PRODUCT
+        # WMO ID should be 10000 for composite
+        assert header[8:13] == self.WMO_ID
+        timestamp = datetime.datetime.strptime(
+            header[2:8] + header[13:17],
+            '%d%H%M%m%y',
+        ).replace(
+            tzinfo=datetime.timezone.utc,
+        )
+        # 1200 km x 1100 km grid
+        assert f'GP{self.HEIGHT}x{self.WIDTH}' in header
+        # 2 bytes per cell
+        expected_bytes = 2 * self.HEIGHT * self.WIDTH + len(header) + 1
+        assert f'BY{expected_bytes:10d}' in header
+        # Integers represent 0.01 mm
+        assert f'PR{self.PRECISION:>5s}' in header
+        # Five minute interval
+        assert f'INT{self.INTERVAL:4d}' in header
+        offset_minutes = int(re.search(r'VV([ \d]{4})', header).group(1))
+        offset = datetime.timedelta(minutes=offset_minutes)
+        return product, timestamp, offset
+
+    def parse_data(self, f):
+        buf = f.read()
+        assert len(buf) == 2 * self.HEIGHT * self.WIDTH, "Unexpected grid size"
+        raw = array.array('H')
+        raw.frombytes(buf)
+        if sys.byteorder != 'little':
+            raw.byteswap()
+        return {
+            'precipitation_5': self.process_raw_data(raw),
+        }
+
+    def process_raw_data(self, raw):
+        multiplier = float('1' + self.PRECISION)
+        return [
+            [
+                x * multiplier if x < 4096 else None
+                for x in raw[row*self.WIDTH:(row+1)*self.WIDTH]
+            ]
+            for row in reversed(range(self.HEIGHT))
+        ]
+
+
 def get_parser(filename):
     parsers = {
+        r'DE1200_RV': RADOLANParser,
         r'MOSMIX_(S|L)_LATEST(_240)?\.kmz$': MOSMIXParser,
         r'Z__C_EDZW_\d+_.*\.json\.bz2$': SYNOPParser,
         r'\w{5}-BEOB\.csv$': CurrentObservationsParser,
         'stundenwerte_FF_': WindObservationsParser,
         'stundenwerte_N_': CloudCoverObservationsParser,
         'stundenwerte_P0_': PressureObservationsParser,
         'stundenwerte_RR_': PrecipitationObservationsParser,
```

### Comparing `dwdparse-0.9.5/dwdparse/stations.py` & `dwdparse-0.9.6/dwdparse/stations.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.5/dwdparse/units.py` & `dwdparse-0.9.6/dwdparse/units.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.5/dwdparse.egg-info/PKG-INFO` & `dwdparse-0.9.6/dwdparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwdparse
-Version: 0.9.5
+Version: 0.9.6
 Summary: Parsers for DWD's open weather data.
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/
 Project-URL: Tracker, https://github.com/jdemaeyer/dwdparse/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dwdparse Version: 0.9.5 Summary: Parsers for DWD's
+Metadata-Version: 2.1 Name: dwdparse Version: 0.9.6 Summary: Parsers for DWD's
 open weather data. Author: Jakob de Maeyer Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/ Project-URL:
 Tracker, https://github.com/jdemaeyer/dwdparse/issues/ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: lean License-File:
 LICENSE # dwdparse [![Build Status](https://img.shields.io/github/actions/
```

### Comparing `dwdparse-0.9.5/setup.py` & `dwdparse-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.5/tests/test_parsers.py` & `dwdparse-0.9.6/tests/test_parsers.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dwdparse.parsers import (
     CloudCoverObservationsParser,
     CurrentObservationsParser,
     DewPointObservationsParser,
     MOSMIXParser,
     PrecipitationObservationsParser,
     PressureObservationsParser,
+    RADOLANParser,
     SolarRadiationObservationsParser,
     SunshineObservationsParser,
     SYNOPParser,
     TemperatureObservationsParser,
     TenMinutesObservationsParser,
     VisibilityObservationsParser,
     WindGustsObservationsParser,
@@ -401,14 +402,46 @@
         {'timestamp': '2023-04-12 01:00', 'solar': 0.0},
         {'timestamp': '2023-04-12 12:00', 'solar': 674000.},
         meta_path=data_dir / 'Meta_Daten_zehn_min_sd_01766.zip',
         count=12,
     )
 
 
+def test_radolan_parser(data_dir):
+    p = RADOLANParser()
+    records = list(p.parse(data_dir / 'DE1200_RV2305081330.tar.bz2'))
+    assert len(records) == 2
+    assert records[0]['observation_type'] == 'radar'
+    assert records[0]['source'] == 'RADOLAN::RV::2023-05-08T13:30:00+00:00'
+    assert records[0]['timestamp'] == datetime.datetime(
+        2023, 5, 8, 13, 30, tzinfo=utc,
+    )
+    assert records[1]['source'] == 'RADOLAN::RV::2023-05-08T13:30:00+00:00'
+    assert records[1]['timestamp'] == datetime.datetime(
+        2023, 5, 8, 14, 20, tzinfo=utc,
+    )
+    data = records[0]['precipitation_5']
+    data_flat = [x for row in data for x in row]
+    assert len(data) == 1200
+    assert all(len(row) == 1100 for row in data)
+    assert sum(x is None for x in data_flat) == 623059
+    assert round(sum(x or 0 for x in data_flat), 2) == 5640.30
+    clipped = [
+        row[334:339]
+        for row in data[1117:1122]
+    ]
+    assert clipped == [
+        [ .03,  .05,  .02,  .01,  .03],  # noqa: E201
+        [ .02,  .03,  .03,    0,    0],  # noqa: E201
+        [ .03,  .04,  .01,    0,  .03],  # noqa: E201
+        [None,  .08,    0,    0,    0],
+        [None, None, None, None, None],
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
@@ -421,13 +454,14 @@
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

### Comparing `dwdparse-0.9.5/tests/test_stations.py` & `dwdparse-0.9.6/tests/test_stations.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.5/tests/test_units.py` & `dwdparse-0.9.6/tests/test_units.py`

 * *Files identical despite different names*

