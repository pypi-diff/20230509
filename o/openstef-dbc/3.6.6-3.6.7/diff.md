# Comparing `tmp/openstef_dbc-3.6.6.tar.gz` & `tmp/openstef_dbc-3.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstef_dbc-3.6.6.tar", last modified: Fri May  5 12:22:08 2023, max compression
+gzip compressed data, was "openstef_dbc-3.6.7.tar", last modified: Tue May  9 10:02:52 2023, max compression
```

## Comparing `openstef_dbc-3.6.6.tar` & `openstef_dbc-3.6.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:08.284922 openstef_dbc-3.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-05 12:22:08.284922 openstef_dbc-3.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:08.280923 openstef_dbc-3.6.6/openstef_dbc/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/data_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/ktp_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:08.280923 openstef_dbc-3.6.6/openstef_dbc/log/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/log/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/log/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:08.280923 openstef_dbc-3.6.6/openstef_dbc/models/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/models/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/models/switch_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:08.284922 openstef_dbc-3.6.6/openstef_dbc/services/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/ems.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/model_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/services/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/openstef_dbc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:08.280923 openstef_dbc-3.6.6/openstef_dbc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-05 12:22:08.000000 openstef_dbc-3.6.6/openstef_dbc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-05 12:22:08.000000 openstef_dbc-3.6.6/openstef_dbc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:22:08.000000 openstef_dbc-3.6.6/openstef_dbc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-05 12:22:08.000000 openstef_dbc-3.6.6/openstef_dbc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 12:22:08.000000 openstef_dbc-3.6.6/openstef_dbc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-05 12:22:08.284922 openstef_dbc-3.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-05 12:21:51.000000 openstef_dbc-3.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:02:52.328148 openstef_dbc-3.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-09 10:02:52.332147 openstef_dbc-3.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:02:52.328148 openstef_dbc-3.6.7/openstef_dbc/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/data_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/ktp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:02:52.328148 openstef_dbc-3.6.7/openstef_dbc/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/log/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/log/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:02:52.328148 openstef_dbc-3.6.7/openstef_dbc/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/models/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/models/switch_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:02:52.328148 openstef_dbc-3.6.7/openstef_dbc/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/ems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/services/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/openstef_dbc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:02:52.328148 openstef_dbc-3.6.7/openstef_dbc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-09 10:02:52.000000 openstef_dbc-3.6.7/openstef_dbc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-09 10:02:52.000000 openstef_dbc-3.6.7/openstef_dbc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:02:52.000000 openstef_dbc-3.6.7/openstef_dbc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-09 10:02:52.000000 openstef_dbc-3.6.7/openstef_dbc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 10:02:52.000000 openstef_dbc-3.6.7/openstef_dbc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-09 10:02:52.332147 openstef_dbc-3.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-09 10:02:35.000000 openstef_dbc-3.6.7/setup.py
```

### Comparing `openstef_dbc-3.6.6/LICENSE` & `openstef_dbc-3.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/PKG-INFO` & `openstef_dbc-3.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef_dbc
-Version: 3.6.6
+Version: 3.6.7
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.6/README.md` & `openstef_dbc-3.6.7/README.md`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/__init__.py` & `openstef_dbc-3.6.7/openstef_dbc/__init__.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/data_interface.py` & `openstef_dbc-3.6.7/openstef_dbc/data_interface.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/database.py` & `openstef_dbc-3.6.7/openstef_dbc/database.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/ktp_api.py` & `openstef_dbc-3.6.7/openstef_dbc/ktp_api.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/log/logging.py` & `openstef_dbc-3.6.7/openstef_dbc/log/logging.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/log/processors.py` & `openstef_dbc-3.6.7/openstef_dbc/log/processors.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/models/measurement.py` & `openstef_dbc-3.6.7/openstef_dbc/models/measurement.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/services/ems.py` & `openstef_dbc-3.6.7/openstef_dbc/services/ems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/services/model_input.py` & `openstef_dbc-3.6.7/openstef_dbc/services/model_input.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/services/prediction_job.py` & `openstef_dbc-3.6.7/openstef_dbc/services/prediction_job.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/services/predictions.py` & `openstef_dbc-3.6.7/openstef_dbc/services/predictions.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/services/predictor.py` & `openstef_dbc-3.6.7/openstef_dbc/services/predictor.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,38 +60,38 @@
         # convert strings to enums if required
         predictor_groups = [PredictorGroups(p) for p in predictor_groups]
 
         if PredictorGroups.WEATHER_DATA in predictor_groups and location is None:
             raise ValueError(
                 "Need to provide a location when weather data predictors are requested."
             )
-        predictors = pd.DataFrame(index=datetime_index)
+        predictors = []
 
         if PredictorGroups.WEATHER_DATA in predictor_groups:
             weather_data_predictors = self.get_weather_data(
                 datetime_start,
                 datetime_end,
                 location=location,
                 forecast_resolution=forecast_resolution,
             )
-            predictors = pd.concat([predictors, weather_data_predictors], axis=1)
+            predictors.append(weather_data_predictors)
 
         if PredictorGroups.MARKET_DATA in predictor_groups:
             market_data_predictors = self.get_market_data(
                 datetime_start, datetime_end, forecast_resolution=forecast_resolution
             )
-            predictors = pd.concat([predictors, market_data_predictors], axis=1)
+            predictors.append(market_data_predictors)
 
         if PredictorGroups.LOAD_PROFILES in predictor_groups:
             load_profiles_predictors = self.get_load_profiles(
                 datetime_start, datetime_end, forecast_resolution=forecast_resolution
             )
-            predictors = pd.concat([predictors, load_profiles_predictors], axis=1)
+            predictors.append(load_profiles_predictors)
 
-        return predictors
+        return pd.concat(predictors, axis=1)
 
     def get_market_data(
         self,
         datetime_start: datetime.datetime,
         datetime_end: datetime.datetime,
         forecast_resolution: str = None,
     ) -> pd.DataFrame:
@@ -196,20 +196,23 @@
             "E3C_I",
             "E3D_A",
             "E3D_I",
             "E4A_A",
             "E4A_I",
         ]
 
-        field_selection = '" or r._field == "'.join(sjv_profles)
-
+        field_selection = '" or r["_field"] == "'.join(sjv_profles)
         query = f"""
-            from(bucket: "realised/autogen")
-                |> range(start: {bind_params["_start"].strftime('%Y-%m-%dT%H:%M:%SZ')}, stop: {bind_params["_stop"].strftime('%Y-%m-%dT%H:%M:%SZ')}) 
-                |> filter(fn: (r) => r._measurement == "sjv" and r._field == "{field_selection}")
+        from(bucket: "realised/autogen")
+            |> range(start: {bind_params["_start"].strftime('%Y-%m-%dT%H:%M:%SZ')}, stop: {bind_params["_stop"].strftime('%Y-%m-%dT%H:%M:%SZ')}) 
+            |> filter(fn: (r) => r["_measurement"] == "sjv")
+            |> filter(fn: (r) => r["_field"] == "{field_selection}")
+            |> aggregateWindow(every: {forecast_resolution[:-3]}m, fn: mean, createEmpty: false)
+            |> yield(name: "mean")
+        
         """
         result = _DataInterface.get_instance().exec_influx_query(
             query, bind_params=bind_params
         )
         # For multiple Fields a list is returned.
         if isinstance(result, list):
             result = pd.concat(result)[["_value", "_field", "_time"]]
@@ -223,15 +226,15 @@
                 )
             )
 
         if forecast_resolution and load_profiles.empty is False:
             load_profiles = load_profiles.resample(forecast_resolution).interpolate(
                 limit=3
             )
-        return load_profiles
+        return load_profiles.shift(periods=-1, freq=forecast_resolution)
 
     def get_weather_data(
         self,
         datetime_start: datetime.datetime,
         datetime_end: datetime.datetime,
         location: Union[Tuple[float, float], str],
         forecast_resolution: str = None,
```

### Comparing `openstef_dbc-3.6.6/openstef_dbc/services/splitting.py` & `openstef_dbc-3.6.7/openstef_dbc/services/splitting.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/services/systems.py` & `openstef_dbc-3.6.7/openstef_dbc/services/systems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/services/weather.py` & `openstef_dbc-3.6.7/openstef_dbc/services/weather.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/services/write.py` & `openstef_dbc-3.6.7/openstef_dbc/services/write.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc/utils.py` & `openstef_dbc-3.6.7/openstef_dbc/utils.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/openstef_dbc.egg-info/PKG-INFO` & `openstef_dbc-3.6.7/openstef_dbc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef-dbc
-Version: 3.6.6
+Version: 3.6.7
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.6/openstef_dbc.egg-info/SOURCES.txt` & `openstef_dbc-3.6.7/openstef_dbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.6/setup.py` & `openstef_dbc-3.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def read_long_description_from_readme():
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setup(
     name="openstef_dbc",
-    version="3.6.6",
+    version="3.6.7",
     packages=find_packages(include=["openstef_dbc", "openstef_dbc.*"]),
     description="Database Connection for OpenSTEF",
     long_description=read_long_description_from_readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/openstef/openstef-dbc",
     author="Alliander N.V",
     author_email="korte.termijn.prognoses@alliander.com",
```

