# Comparing `tmp/spatial_summarize_within-0.1.1.tar.gz` & `tmp/spatial_summarize_within-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial_summarize_within-0.1.1.tar", last modified: Sat May  6 23:03:24 2023, max compression
+gzip compressed data, was "spatial_summarize_within-0.1.2.tar", last modified: Mon May  8 23:09:43 2023, max compression
```

## Comparing `spatial_summarize_within-0.1.1.tar` & `spatial_summarize_within-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-06 23:03:24.663974 spatial_summarize_within-0.1.1/
--rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-0.1.1/LICENSE
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-06 23:03:24.663870 spatial_summarize_within-0.1.1/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)     2188 2023-05-06 22:57:53.000000 spatial_summarize_within-0.1.1/README.md
--rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-05-06 23:03:24.664008 spatial_summarize_within-0.1.1/setup.cfg
--rw-r--r--   0 Kenne      (501) staff       (20)      252 2023-05-06 22:58:09.000000 spatial_summarize_within-0.1.1/setup.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-06 23:03:24.663189 spatial_summarize_within-0.1.1/spatial_summarize_within/
--rw-r--r--   0 Kenne      (501) staff       (20)       46 2023-05-06 23:00:41.000000 spatial_summarize_within-0.1.1/spatial_summarize_within/__init__.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2116 2023-05-06 20:55:51.000000 spatial_summarize_within-0.1.1/spatial_summarize_within/summarize_within.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-06 23:03:24.663734 spatial_summarize_within-0.1.1/spatial_summarize_within.egg-info/
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-06 23:03:24.000000 spatial_summarize_within-0.1.1/spatial_summarize_within.egg-info/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)      347 2023-05-06 23:03:24.000000 spatial_summarize_within-0.1.1/spatial_summarize_within.egg-info/SOURCES.txt
--rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-05-06 23:03:24.000000 spatial_summarize_within-0.1.1/spatial_summarize_within.egg-info/dependency_links.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-05-06 23:03:24.000000 spatial_summarize_within-0.1.1/spatial_summarize_within.egg-info/requires.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-05-06 23:03:24.000000 spatial_summarize_within-0.1.1/spatial_summarize_within.egg-info/top_level.txt
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-08 23:09:43.592262 spatial_summarize_within-0.1.2/
+-rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-0.1.2/LICENSE
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-08 23:09:43.592158 spatial_summarize_within-0.1.2/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)     2188 2023-05-06 22:57:53.000000 spatial_summarize_within-0.1.2/README.md
+-rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-05-08 23:09:43.592296 spatial_summarize_within-0.1.2/setup.cfg
+-rw-r--r--   0 Kenne      (501) staff       (20)      252 2023-05-08 23:08:58.000000 spatial_summarize_within-0.1.2/setup.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-08 23:09:43.591436 spatial_summarize_within-0.1.2/spatial_summarize_within/
+-rw-r--r--   0 Kenne      (501) staff       (20)       46 2023-05-06 23:00:41.000000 spatial_summarize_within-0.1.2/spatial_summarize_within/__init__.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2294 2023-05-08 23:09:21.000000 spatial_summarize_within-0.1.2/spatial_summarize_within/summarize_within.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-08 23:09:43.592010 spatial_summarize_within-0.1.2/spatial_summarize_within.egg-info/
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-08 23:09:43.000000 spatial_summarize_within-0.1.2/spatial_summarize_within.egg-info/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)      347 2023-05-08 23:09:43.000000 spatial_summarize_within-0.1.2/spatial_summarize_within.egg-info/SOURCES.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-05-08 23:09:43.000000 spatial_summarize_within-0.1.2/spatial_summarize_within.egg-info/dependency_links.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-05-08 23:09:43.000000 spatial_summarize_within-0.1.2/spatial_summarize_within.egg-info/requires.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-05-08 23:09:43.000000 spatial_summarize_within-0.1.2/spatial_summarize_within.egg-info/top_level.txt
```

### Comparing `spatial_summarize_within-0.1.1/LICENSE` & `spatial_summarize_within-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.1.1/README.md` & `spatial_summarize_within-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.1.1/spatial_summarize_within/summarize_within.py` & `spatial_summarize_within-0.1.2/spatial_summarize_within/summarize_within.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         temp_intersect["intersect_area"] = temp_intersect.area
         # Calculate the percentage overlap of each polygon in the input geodataframe with the current overlay polygon
         temp_intersect["overlap_pct"] = temp_intersect["intersect_area"] / temp_intersect["area"]
         # Calculate the weighted sum
         columns = columns_to_sum
         for column in columns:
             temp_intersect[column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).round(0)
+        # Keep only the relevant columns in the temp_intersect dataframe
+        temp_intersect = temp_intersect[[key_to_group_by] + columns + ['intersect_area', 'overlap_pct']]
         # Group the results
         temp_result = temp_intersect.groupby(key_to_group_by).sum(numeric_only=True).reset_index()
         # Append the results to the result gdf
         result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
     result_gdf = overlay.merge(result_gdf, on=key_to_group_by)
```

