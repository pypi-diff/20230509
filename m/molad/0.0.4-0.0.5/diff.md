# Comparing `tmp/molad-0.0.4.tar.gz` & `tmp/molad-0.0.5.tar.gz`

## Comparing `molad-0.0.4.tar` & `molad-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 molad-0.0.4/Pipfile
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 molad-0.0.4/Pipfile.lock
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 molad-0.0.4/requirements.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 molad-0.0.4/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 molad-0.0.4/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 molad-0.0.4/.pytest_cache/README.md
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 molad-0.0.4/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     5219 2020-02-02 00:00:00.000000 molad-0.0.4/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 molad-0.0.4/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 molad-0.0.4/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 molad-0.0.4/src/molad/__init__.py
--rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 molad-0.0.4/src/molad/helper.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 molad-0.0.4/tests/test_molad.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 molad-0.0.4/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 molad-0.0.4/LICENSE
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 molad-0.0.4/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 molad-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 molad-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 molad-0.0.5/Pipfile
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 molad-0.0.5/Pipfile.lock
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 molad-0.0.5/requirements.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 molad-0.0.5/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 molad-0.0.5/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 molad-0.0.5/.pytest_cache/README.md
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 molad-0.0.5/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 molad-0.0.5/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 molad-0.0.5/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 molad-0.0.5/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 molad-0.0.5/src/molad/__init__.py
+-rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 molad-0.0.5/src/molad/helper.py
+-rw-r--r--   0        0        0     6724 2020-02-02 00:00:00.000000 molad-0.0.5/tests/test_molad.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 molad-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 molad-0.0.5/LICENSE
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 molad-0.0.5/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 molad-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 molad-0.0.5/PKG-INFO
```

### Comparing `molad-0.0.4/Pipfile.lock` & `molad-0.0.5/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `molad-0.0.4/.pytest_cache/v/cache/nodeids` & `molad-0.0.5/.pytest_cache/v/cache/nodeids`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9186046511627907%*

 * *Differences: {'insert': "[(70, 'tests/test_molad.py::test_molad[Two Day Rosh Chodesh Friday and Shabbos - "*

 * *           "Friday After Sunset-date6-expected6]'), (71, 'tests/test_molad.py::test_molad[Two Day "*

 * *           "Rosh Chodesh Friday and Shabbos - Friday After Sunset-date8-expected8]'), (72, "*

 * *           "'tests/test_molad.py::test_molad[Two Day Rosh Chodesh Friday and Shabbos - Friday "*

 * *           "Before Sunset-date5-expected5]'), (73, 'tests/test_molad.py::test_molad[Two Day Rosh "*

 * *           "Chodesh Friday an […]*

```diff
@@ -65,14 +65,21 @@
     "tests/test_molad.py::TestMoladRegularYear::test_rosh_chodesh_text",
     "tests/test_molad.py::test_molad",
     "tests/test_molad.py::test_molad[Far Future Year-date4-expected4]",
     "tests/test_molad.py::test_molad[Far Past Year-date3-expected3]",
     "tests/test_molad.py::test_molad[Leap Year After Adar-date2-expected2]",
     "tests/test_molad.py::test_molad[Leap Year Before Adar-date1-expected1]",
     "tests/test_molad.py::test_molad[Regular Year-date0-expected0]",
+    "tests/test_molad.py::test_molad[Two Day Rosh Chodesh Friday and Shabbos - Friday After Sunset-date6-expected6]",
+    "tests/test_molad.py::test_molad[Two Day Rosh Chodesh Friday and Shabbos - Friday After Sunset-date8-expected8]",
+    "tests/test_molad.py::test_molad[Two Day Rosh Chodesh Friday and Shabbos - Friday Before Sunset-date5-expected5]",
+    "tests/test_molad.py::test_molad[Two Day Rosh Chodesh Friday and Shabbos - Friday Before Sunset-date7-expected7]",
+    "tests/test_molad.py::test_molad[Two Day Rosh Chodesh Friday and Shabbos - Shabbos Mevorchim - Friday After Sunset-date6-expected6]",
+    "tests/test_molad.py::test_molad[Two Day Rosh Chodesh Friday and Shabbos - Shabbos Mevorchim - Friday Before Sunset-date5-expected5]",
+    "tests/test_molad.py::test_molad[Two Day Rosh Chodesh Friday and Shabbos-date5-expected5]",
     "tests/test_molad.py::test_molad[molad0]",
     "tests/test_molad.py::test_molad[molad1]",
     "tests/test_molad.py::test_molad[molad2]",
     "tests/test_molad.py::test_molad[molad3]",
     "tests/test_molad.py::test_molad[molad4]",
     "tests/test_molad.py::test_molad[n0]",
     "tests/test_molad.py::test_molad_day",
```

### Comparing `molad-0.0.4/src/molad/helper.py` & `molad-0.0.5/src/molad/helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -214,18 +214,23 @@
 
         if month == 14:
             month = 1
             year = year + 1
 
         return {"year": year, "month": month}
 
-    def get_day_of_week(self, numeric_date, day):
+    def get_gdate(self, numeric_date, day):
         hebrew_date = hdate.HebrewDate(numeric_date["year"], numeric_date["month"], day)
         jdn_date = hdate.converters.hdate_to_jdn(hebrew_date)
         gdate = hdate.converters.jdn_to_gdate(jdn_date)
+
+        return gdate;
+
+    def get_day_of_week(self, numeric_date, day):
+        gdate = self.get_gdate(numeric_date, day)
         weekday = gdate.strftime("%A")
 
         if weekday == "Saturday":
             weekday = "Shabbos"
 
         return weekday
 
@@ -255,23 +260,44 @@
         else:
             return RoshChodesh(
                 month = next_month_name,
                 text = first + " & " + second,
                 days = [first, second],
             )
 
+    def get_shabbos_mevorchim_english_date(self, date):
+        this_month = self.get_numeric_month_year(date)
+        gdate = self.get_gdate(this_month, 30)
+
+        idx = (gdate.weekday() + 1) % 7
+        sat_date = gdate - datetime.timedelta(7+idx-6)
+
+        return sat_date
+    
+    def get_shabbos_mevorchim_hebrew_day_of_month(self, date):
+        gdate = self.get_shabbos_mevorchim_english_date(date)
+        j = hdate.converters.gdate_to_jdn(gdate)
+        h = hdate.converters.jdn_to_hdate(j)
+        return h.day
+    
     def is_shabbos_mevorchim(self, date) -> bool:
         loc = self.get_current_location()
         j = hdate.converters.gdate_to_jdn(date)
         h = hdate.converters.jdn_to_hdate(j)
+        hd = h.day
         z = hdate.Zmanim(date=date, location=loc, hebrew=False)
 
+        if (z.time > z.zmanim["sunset"]):
+            hd += 1
+
+        sm = self.get_shabbos_mevorchim_hebrew_day_of_month(date)
+        
         return (
             self.is_actual_shabbat(z)
-            and h.day >= 23
+            and hd == sm
             and h.month != hdate.htables.Months.Elul
         )
 
     def is_actual_shabbat(self, z) -> bool:
         today = hdate.HDate(gdate=z.date, diaspora=z.location.diaspora)
         tomorrow = hdate.HDate(
             gdate=z.date + datetime.timedelta(days=1), diaspora=z.location.diaspora
```

### Comparing `molad-0.0.4/tests/test_molad.py` & `molad-0.0.5/tests/test_molad.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from molad.molad import MoladHelper
-from molad.molad import MoladDetails
-from molad.molad import Molad
-from molad.molad import RoshChodesh
+from molad.helper import MoladHelper
+from molad.helper import MoladDetails
+from molad.helper import Molad
+from molad.helper import RoshChodesh
 import datetime
 import pytest
 
 molads = [
     (
         'Regular Year',
         datetime.datetime(2023, 2, 15),
@@ -101,14 +101,94 @@
             is_shabbos_mevorchim=True,
             rosh_chodesh=RoshChodesh(
                 month="Tevet",
                 days=["Tuesday", "Wednesday"],
                 text="Tuesday & Wednesday",
             )
         )
+    ),
+    (
+    'Two Day Rosh Chodesh Friday and Shabbos - Shabbos Mevorchim - Friday Before Sunset',
+        datetime.datetime(2023, 4, 14, 11),
+        MoladDetails(
+            molad=Molad(
+                friendly="Thursday, 2:08 pm and 13 chalakim",
+                day="Thursday",
+                hours=2,
+                minutes=8,
+                chalakim=13,
+                am_or_pm="pm"
+            ),
+            is_shabbos_mevorchim=False,
+            rosh_chodesh=RoshChodesh(
+                month="Iyyar",
+                days=["Friday", "Shabbos"],
+                text="Friday & Shabbos",
+            )
+        )
+    ),
+    (
+    'Two Day Rosh Chodesh Friday and Shabbos - Shabbos Mevorchim - Friday After Sunset',
+        datetime.datetime(2023, 4, 14, 23),
+        MoladDetails(
+            molad=Molad(
+                friendly="Thursday, 2:08 pm and 13 chalakim",
+                day="Thursday",
+                hours=2,
+                minutes=8,
+                chalakim=13,
+                am_or_pm="pm"
+            ),
+            is_shabbos_mevorchim=True,
+            rosh_chodesh=RoshChodesh(
+                month="Iyyar",
+                days=["Friday", "Shabbos"],
+                text="Friday & Shabbos",
+            )
+        )
+    ),
+    (
+    'Two Day Rosh Chodesh Friday and Shabbos - Friday Before Sunset',
+        datetime.datetime(2023, 4, 21, 11),
+        MoladDetails(
+            molad=Molad(
+                friendly="Thursday, 2:08 pm and 13 chalakim",
+                day="Thursday",
+                hours=2,
+                minutes=8,
+                chalakim=13,
+                am_or_pm="pm"
+            ),
+            is_shabbos_mevorchim=False,
+            rosh_chodesh=RoshChodesh(
+                month="Iyyar",
+                days=["Friday", "Shabbos"],
+                text="Friday & Shabbos",
+            )
+        )
+    ),
+    (
+    'Two Day Rosh Chodesh Friday and Shabbos - Friday After Sunset',
+        datetime.datetime(2023, 4, 21, 23),
+        MoladDetails(
+            molad=Molad(
+                friendly="Thursday, 2:08 pm and 13 chalakim",
+                day="Thursday",
+                hours=2,
+                minutes=8,
+                chalakim=13,
+                am_or_pm="pm"
+            ),
+            is_shabbos_mevorchim=False,
+            rosh_chodesh=RoshChodesh(
+                month="Iyyar",
+                days=["Friday", "Shabbos"],
+                text="Friday & Shabbos",
+            )
+        )
     )
 ]
 
 @pytest.mark.parametrize('name,date,expected', molads)
 def test_molad(name, date, expected):
     calculated = get_molad(date)
```

### Comparing `molad-0.0.4/LICENSE` & `molad-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `molad-0.0.4/pyproject.toml` & `molad-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "molad"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Chaim Chaikin", email="molad@chaimchaikin.com" },
 ]
 description = "Molad for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `molad-0.0.4/PKG-INFO` & `molad-0.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molad
-Version: 0.0.4
+Version: 0.0.5
 Summary: Molad for Python
 Project-URL: Homepage, https://github.com/chaimchaikin/molad
 Project-URL: Bug Tracker, https://github.com/chaimchaikin/molad/issues
 Author-email: Chaim Chaikin <molad@chaimchaikin.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

