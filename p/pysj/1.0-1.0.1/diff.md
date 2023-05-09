# Comparing `tmp/pysj-1.0.tar.gz` & `tmp/pysj-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysj-1.0.tar", last modified: Sat Jan 14 19:30:46 2023, max compression
+gzip compressed data, was "pysj-1.0.1.tar", last modified: Tue May  9 11:01:50 2023, max compression
```

## Comparing `pysj-1.0.tar` & `pysj-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     2779 2022-04-02 07:00:57.140323 pysj-1.0/.gitignore
--rw-r--r--   0        0        0      559 2022-01-16 18:00:32.029533 pysj-1.0/.vscode/launch.json
--rw-r--r--   0        0        0      191 2022-01-16 18:00:32.029533 pysj-1.0/.vscode/settings.json
--rw-r--r--   0        0        0      863 2022-01-16 18:00:32.029533 pysj-1.0/.vscode/tasks.json
--rw-r--r--   0        0        0     1086 2022-04-01 06:05:35.328085 pysj-1.0/LICENSE
--rw-r--r--   0        0        0     3311 2023-01-14 19:27:20.016232 pysj-1.0/README.md
--rw-r--r--   0        0        0      681 2022-11-24 12:22:55.458603 pysj-1.0/dodo.py
--rw-r--r--   0        0        0      815 2022-07-28 10:45:58.822848 pysj-1.0/pyproject.toml
--rw-r--r--   0        0        0      421 2023-01-14 19:30:44.812765 pysj-1.0/pysj/__init__.py
--rw-r--r--   0        0        0     1975 2023-01-14 17:39:57.802289 pysj-1.0/pysj/crypto.py
--rw-r--r--   0        0        0     1524 2022-03-01 18:57:00.446349 pysj-1.0/pysj/formats.py
--rw-r--r--   0        0        0     8079 2023-01-14 13:00:23.147917 pysj-1.0/pysj/main.py
--rw-r--r--   0        0        0     5151 2022-08-19 10:19:23.826017 pysj-1.0/pysj/overengineer.py
--rw-r--r--   0        0        0     1015 2022-04-01 10:10:26.613031 pysj-1.0/tests/test_Crypto.py
--rw-r--r--   0        0        0     1309 2022-11-06 18:41:21.819954 pysj-1.0/tests/test_ExtendedJSONTranscoding.py
--rw-r--r--   0        0        0      469 2021-12-21 08:46:25.350399 pysj-1.0/tests/test_Flatten.py
--rw-r--r--   0        0        0      312 2022-03-13 11:30:51.360579 pysj-1.0/tests/test_Paginate.py
--rw-r--r--   0        0        0      920 2021-12-30 13:26:02.657349 pysj-1.0/tests/test_Seconds.py
--rw-r--r--   0        0        0      857 2022-03-05 11:42:02.511834 pysj-1.0/tests/test_Timer.py
--rw-r--r--   0        0        0      752 2023-01-14 11:43:55.663699 pysj-1.0/tests/test_chunk.py
--rw-r--r--   0        0        0      176 2023-01-14 11:55:22.601104 pysj-1.0/tests/test_first.py
--rw-r--r--   0        0        0      656 2022-03-05 11:42:02.515834 pysj-1.0/tests/test_formats.py
--rw-r--r--   0        0        0      160 2022-01-28 18:38:11.217320 pysj-1.0/tests/test_iso.py
--rw-r--r--   0        0        0      368 2023-01-14 17:41:15.342353 pysj-1.0/tests/test_moving_average.py
--rw-r--r--   0        0        0      832 2022-12-01 18:41:33.748363 pysj-1.0/tests/test_n_wise.py
--rw-r--r--   0        0        0      204 2023-01-14 11:55:22.601104 pysj-1.0/tests/test_take.py
--rw-r--r--   0        0        0      337 2022-11-27 18:34:31.552734 pysj-1.0/tests/test_transpose.py
--rw-r--r--   0        0        0     3746 1970-01-01 00:00:00.000000 pysj-1.0/PKG-INFO
+-rw-r--r--   0        0        0     2779 2022-04-02 07:00:57.140323 pysj-1.0.1/.gitignore
+-rw-r--r--   0        0        0      559 2022-01-16 18:00:32.029533 pysj-1.0.1/.vscode/launch.json
+-rw-r--r--   0        0        0      191 2022-01-16 18:00:32.029533 pysj-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0      863 2022-01-16 18:00:32.029533 pysj-1.0.1/.vscode/tasks.json
+-rw-r--r--   0        0        0     1086 2022-04-01 06:05:35.328085 pysj-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3311 2023-01-14 19:27:20.016232 pysj-1.0.1/README.md
+-rw-r--r--   0        0        0      681 2022-11-24 12:22:55.458603 pysj-1.0.1/dodo.py
+-rw-r--r--   0        0        0      815 2022-07-28 10:45:58.822848 pysj-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      443 2023-05-09 11:01:48.355733 pysj-1.0.1/pysj/__init__.py
+-rw-r--r--   0        0        0     1975 2023-01-14 17:39:57.802289 pysj-1.0.1/pysj/crypto.py
+-rw-r--r--   0        0        0     1524 2022-03-01 18:57:00.446349 pysj-1.0.1/pysj/formats.py
+-rw-r--r--   0        0        0     8772 2023-05-09 11:01:48.355733 pysj-1.0.1/pysj/main.py
+-rw-r--r--   0        0        0     5150 2023-05-09 10:58:36.371421 pysj-1.0.1/pysj/overengineer.py
+-rw-r--r--   0        0        0     1015 2022-04-01 10:10:26.613031 pysj-1.0.1/tests/test_Crypto.py
+-rw-r--r--   0        0        0     1305 2023-05-09 10:58:36.247421 pysj-1.0.1/tests/test_ExtendedJSONTranscoding.py
+-rw-r--r--   0        0        0      466 2023-05-09 10:58:36.227421 pysj-1.0.1/tests/test_Flatten.py
+-rw-r--r--   0        0        0      312 2022-03-13 11:30:51.360579 pysj-1.0.1/tests/test_Paginate.py
+-rw-r--r--   0        0        0      920 2021-12-30 13:26:02.657349 pysj-1.0.1/tests/test_Seconds.py
+-rw-r--r--   0        0        0      854 2023-05-09 10:58:36.247421 pysj-1.0.1/tests/test_Timer.py
+-rw-r--r--   0        0        0      752 2023-01-14 11:43:55.663699 pysj-1.0.1/tests/test_chunk.py
+-rw-r--r--   0        0        0      176 2023-01-14 11:55:22.601104 pysj-1.0.1/tests/test_first.py
+-rw-r--r--   0        0        0      655 2023-05-09 10:58:36.227421 pysj-1.0.1/tests/test_formats.py
+-rw-r--r--   0        0        0      158 2023-05-09 10:58:36.219421 pysj-1.0.1/tests/test_iso.py
+-rw-r--r--   0        0        0      642 2023-05-09 10:58:05.551469 pysj-1.0.1/tests/test_months_in_interval.py
+-rw-r--r--   0        0        0      368 2023-01-14 17:41:15.342353 pysj-1.0.1/tests/test_moving_average.py
+-rw-r--r--   0        0        0      831 2023-05-09 10:58:36.263421 pysj-1.0.1/tests/test_n_wise.py
+-rw-r--r--   0        0        0      204 2023-01-14 11:55:22.601104 pysj-1.0.1/tests/test_take.py
+-rw-r--r--   0        0        0      336 2023-05-09 10:58:36.259421 pysj-1.0.1/tests/test_transpose.py
+-rw-r--r--   0        0        0     3748 1970-01-01 00:00:00.000000 pysj-1.0.1/PKG-INFO
```

### Comparing `pysj-1.0/.gitignore` & `pysj-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pysj-1.0/.vscode/launch.json` & `pysj-1.0.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pysj-1.0/.vscode/tasks.json` & `pysj-1.0.1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `pysj-1.0/LICENSE` & `pysj-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysj-1.0/README.md` & `pysj-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pysj-1.0/dodo.py` & `pysj-1.0.1/dodo.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0/pyproject.toml` & `pysj-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysj-1.0/pysj/crypto.py` & `pysj-1.0.1/pysj/crypto.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0/pysj/formats.py` & `pysj-1.0.1/pysj/formats.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0/pysj/main.py` & `pysj-1.0.1/pysj/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import dataclasses
 import json
 import time
 from datetime import date, datetime, timedelta
 from fractions import Fraction
 from itertools import islice, tee, zip_longest
-from typing import Any, Callable, Iterable, List, Tuple
+from typing import (Any, Callable, Iterable, List, Literal, Optional, Tuple,
+                    Union)
 
 NUMPY_SUPPORT_FLAG = True
 try:
     import numpy as np
 except ImportError:
     NUMPY_SUPPORT_FLAG = False
 
 
 class Timer:
     """Simple class working like a stopwatch."""
 
     def __init__(self) -> None:
-
         self.time = None
         self.start_time = time.perf_counter()
 
     def __enter__(self):
         print("Starting timer")
         self.start()
 
@@ -45,15 +45,16 @@
 
     def total(self):
         return time.perf_counter() - self.start_time
 
 
 def isotime(precision="d", dt=None):
     """Get the current date/time in isoformat. Default precision is day, accepts d(ay), (h)our, (m)inute, (s)econd.
-    Per defualt the current time is used, this can be overriden by supplying a datetime object with the *dt* kwarg"""
+    Per defualt the current time is used, this can be overriden by supplying a datetime object with the *dt* kwarg
+    """
     if not dt:
         dt = datetime.now()
     precision_map = {
         "d": slice(0, 10),
         "h": slice(0, 13),
         "m": slice(0, 16),
         "s": slice(0, 19),
@@ -89,14 +90,38 @@
     return int(
         timedelta(
             days, seconds, microseconds, milliseconds, minutes, hours, weeks
         ).total_seconds()
     )
 
 
+def months_in_interval(
+    start: datetime,
+    end: Optional[datetime] = None,
+):
+    """Yields months and year from the given interval (start -> end).
+
+    start: datetime
+        Start of interval
+    end: datetime
+        Optional, end of interval. Todays date is used if end is not set.
+
+    return: Iterable[Tuple[int, int]]
+    """
+    if end is None:
+        end = datetime.today()
+
+    dt = datetime(start.year, start.month, 1)
+    while dt <= datetime(end.year, end.month, 1):
+        yield dt.month, dt.year
+
+        dt = dt + timedelta(days=40)
+        dt = datetime(dt.year, dt.month, 1)
+
+
 def flatten(iterable: Iterable) -> list:
     """Recursively flattens an iterable (depth first)
 
     Usage
     -----
 
     >>> nested_list = [[(1.3, 3.0), "string", "another string"], [4, 5E2, sorted({"a", "b", "c"})]]
@@ -128,14 +153,15 @@
     -----
     >>> obj = {"timestamp": datetime.today()}
     >>> json.dumps(obj, cls=ExtendedJSONEncoder)
 
     """
 
     def default(self, o):
+        # TODO: Support Decimal type
         if isinstance(o, datetime):
             return o.isoformat(timespec="seconds")
         if isinstance(o, date):
             return o.isoformat()
         if dataclasses.is_dataclass(o):
             return dataclasses.asdict(o)
```

### Comparing `pysj-1.0/pysj/overengineer.py` & `pysj-1.0.1/pysj/overengineer.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         server.allow_reuse_address = True
         server.server_activate()
         server.serve_forever()
 
 
 class SchedulableProcess:
     def __init__(self, target=None, args=None, name=None, **kwargs):
-
         self.target = target
         self.args = args if args else ()
         self.triggers = kwargs
         self.name = name if name else target.__name__
         self.proc = None
         self.last_run = None
```

### Comparing `pysj-1.0/tests/test_Crypto.py` & `pysj-1.0.1/tests/test_Crypto.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0/tests/test_ExtendedJSONTranscoding.py` & `pysj-1.0.1/tests/test_ExtendedJSONTranscoding.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,45 +4,41 @@
 
 import numpy as np
 
 from pysj import ExtendedJSONDecoder, ExtendedJSONEncoder
 
 
 def test_date_json_encoding():
-
     test = json.dumps(
         {"lol": datetime.date(2021, 12, 1)},
         cls=ExtendedJSONEncoder,
     )
 
     assert test == '{"lol": "2021-12-01"}'
 
 
 def test_datetime_json_encoding():
-
     test = json.dumps(
         {"lol": datetime.datetime.fromisoformat("2021-12-01T04:50:00.123456")},
         cls=ExtendedJSONEncoder,
     )
 
     assert test == '{"lol": "2021-12-01T04:50:00"}'
 
 
 def test_datetime_json_decoding():
-
     test = json.loads(
         '{"lol": "2021-12-01T04:50:00"}',
         cls=ExtendedJSONDecoder,
     )
 
     assert test == {"lol": datetime.datetime.fromisoformat("2021-12-01T04:50:00")}
 
 
 def test_numpy_serialization():
-
     test = json.dumps(
         [1, 2, 3, np.int64(10), np.int8(11), np.int32(12)],
         cls=ExtendedJSONEncoder,
     )
 
     assert test == "[1, 2, 3, 10, 11, 12]"
```

### Comparing `pysj-1.0/tests/test_Seconds.py` & `pysj-1.0.1/tests/test_Seconds.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0/tests/test_Timer.py` & `pysj-1.0.1/tests/test_Timer.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,40 +3,37 @@
 import pytest
 from pytest import approx
 
 from pysj import Timer
 
 
 def test_lap_timing():
-
     timer = Timer()
 
     timer.start()
     for i in range(1, 4):
         print(i)
         sleep(0.1)
         assert timer.lap() == approx(i / 10, abs=1e-2)
 
     assert timer.total() == approx(0.3, abs=1e-2)
 
 
 def test_reset_timing():
-
     timer = Timer()
 
     timer.start()
     for _ in range(1, 4):
         sleep(0.1)
         assert timer.reset() == approx(0.1, abs=1e-2)
 
     assert timer.total() == approx(0.3, abs=1e-2)
 
 
 def test_use_as_contextmanager(capsys):
-
     with Timer():
         sleep(0.1)
 
     out, err = capsys.readouterr()
     output_line_1, output_line_2 = out.splitlines()
     assert output_line_1 == "Starting timer"
     assert output_line_2.startswith("Elapsed time")
```

### Comparing `pysj-1.0/tests/test_chunk.py` & `pysj-1.0.1/tests/test_chunk.py`

 * *Files identical despite different names*

### Comparing `pysj-1.0/tests/test_formats.py` & `pysj-1.0.1/tests/test_formats.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pytest
 
 from pysj.formats import all_image_extensions, common_image_extensions
 
 
 def test_common_formats():
-
     assert common_image_extensions == {
         "png",
         "jpg",
         "jpeg",
         "jfif",
         "j2p",
         "jpx",
```

### Comparing `pysj-1.0/tests/test_n_wise.py` & `pysj-1.0.1/tests/test_n_wise.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from pysj import n_wise, triplewise
 
 test_data = (1, 2, 3, 4, 5, 6)
 
 
 def test_n_wise_2_comp_pairwise():
-
     try:
         from itertools import pairwise
 
         #  itertools.pairwise and n_wise with a n of 2 should be equal.
         assert sum(sum((a, b)) for a, b in pairwise(test_data)) == sum(
             sum((a, b)) for a, b in n_wise(2, test_data)
         )
```

### Comparing `pysj-1.0/PKG-INFO` & `pysj-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysj
-Version: 1.0
+Version: 1.0.1
 Summary: Pysj makes Python development more comfortable, with utils, classes and helper
 Author: Sondre S. Ødegård
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Project-URL: Documentation, https://github.com/sondreod/pysj
```

