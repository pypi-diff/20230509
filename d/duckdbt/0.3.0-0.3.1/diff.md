# Comparing `tmp/duckdbt-0.3.0.tar.gz` & `tmp/duckdbt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckdbt-0.3.0.tar", last modified: Mon May  8 20:57:45 2023, max compression
+gzip compressed data, was "duckdbt-0.3.1.tar", last modified: Tue May  9 00:16:03 2023, max compression
```

## Comparing `duckdbt-0.3.0.tar` & `duckdbt-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-08 20:57:45.846511 duckdbt-0.3.0/
--rw-r--r--   0 jwills     (501) staff       (20)       53 2023-01-14 04:58:00.000000 duckdbt-0.3.0/MANIFEST.in
--rw-r--r--   0 jwills     (501) staff       (20)      302 2023-05-08 20:57:45.846402 duckdbt-0.3.0/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)       53 2023-05-08 20:57:22.000000 duckdbt-0.3.0/README.md
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-08 20:57:45.845054 duckdbt-0.3.0/duckdbt/
--rw-r--r--   0 jwills     (501) staff       (20)     1248 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/api.py
--rw-r--r--   0 jwills     (501) staff       (20)     1736 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/extensions.py
--rw-r--r--   0 jwills     (501) staff       (20)      696 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/ipython.py
--rw-r--r--   0 jwills     (501) staff       (20)     1388 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/load_db_profile.py
--rw-r--r--   0 jwills     (501) staff       (20)     1884 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/server.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-08 20:57:45.846078 duckdbt-0.3.0/duckdbt/static/
--rw-r--r--   0 jwills     (501) staff       (20)     1246 2023-01-14 04:58:00.000000 duckdbt-0.3.0/duckdbt/static/dashboard.css
--rw-r--r--   0 jwills     (501) staff       (20)     1406 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/static/favicon.ico
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-08 20:57:45.846219 duckdbt-0.3.0/duckdbt/templates/
--rw-r--r--   0 jwills     (501) staff       (20)     5332 2023-05-08 20:17:37.000000 duckdbt-0.3.0/duckdbt/templates/index.html
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-08 20:57:45.845726 duckdbt-0.3.0/duckdbt.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)      302 2023-05-08 20:57:45.000000 duckdbt-0.3.0/duckdbt.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)      370 2023-05-08 20:57:45.000000 duckdbt-0.3.0/duckdbt.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-05-08 20:57:45.000000 duckdbt-0.3.0/duckdbt.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       79 2023-05-08 20:57:45.000000 duckdbt-0.3.0/duckdbt.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)        8 2023-05-08 20:57:45.000000 duckdbt-0.3.0/duckdbt.egg-info/top_level.txt
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-05-08 20:57:45.846544 duckdbt-0.3.0/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)      954 2023-05-08 20:17:37.000000 duckdbt-0.3.0/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-09 00:16:03.623397 duckdbt-0.3.1/
+-rw-r--r--   0 jwills     (501) staff       (20)       53 2023-01-14 04:58:00.000000 duckdbt-0.3.1/MANIFEST.in
+-rw-r--r--   0 jwills     (501) staff       (20)      302 2023-05-09 00:16:03.623286 duckdbt-0.3.1/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)       53 2023-05-08 20:57:22.000000 duckdbt-0.3.1/README.md
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-09 00:16:03.622033 duckdbt-0.3.1/duckdbt/
+-rw-r--r--   0 jwills     (501) staff       (20)     1248 2023-05-08 20:17:37.000000 duckdbt-0.3.1/duckdbt/api.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1736 2023-05-08 20:17:37.000000 duckdbt-0.3.1/duckdbt/extensions.py
+-rw-r--r--   0 jwills     (501) staff       (20)      696 2023-05-08 20:17:37.000000 duckdbt-0.3.1/duckdbt/ipython.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1786 2023-05-09 00:15:58.000000 duckdbt-0.3.1/duckdbt/load_db_profile.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1884 2023-05-08 20:17:37.000000 duckdbt-0.3.1/duckdbt/server.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-09 00:16:03.622990 duckdbt-0.3.1/duckdbt/static/
+-rw-r--r--   0 jwills     (501) staff       (20)     1246 2023-01-14 04:58:00.000000 duckdbt-0.3.1/duckdbt/static/dashboard.css
+-rw-r--r--   0 jwills     (501) staff       (20)     1406 2023-05-08 20:17:37.000000 duckdbt-0.3.1/duckdbt/static/favicon.ico
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-09 00:16:03.623122 duckdbt-0.3.1/duckdbt/templates/
+-rw-r--r--   0 jwills     (501) staff       (20)     5332 2023-05-08 20:17:37.000000 duckdbt-0.3.1/duckdbt/templates/index.html
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-09 00:16:03.622636 duckdbt-0.3.1/duckdbt.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)      302 2023-05-09 00:16:03.000000 duckdbt-0.3.1/duckdbt.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)      370 2023-05-09 00:16:03.000000 duckdbt-0.3.1/duckdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-05-09 00:16:03.000000 duckdbt-0.3.1/duckdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       87 2023-05-09 00:16:03.000000 duckdbt-0.3.1/duckdbt.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        8 2023-05-09 00:16:03.000000 duckdbt-0.3.1/duckdbt.egg-info/top_level.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-05-09 00:16:03.623430 duckdbt-0.3.1/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)      951 2023-05-09 00:15:58.000000 duckdbt-0.3.1/setup.py
```

### Comparing `duckdbt-0.3.0/duckdbt/api.py` & `duckdbt-0.3.1/duckdbt/api.py`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.0/duckdbt/extensions.py` & `duckdbt-0.3.1/duckdbt/extensions.py`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.0/duckdbt/ipython.py` & `duckdbt-0.3.1/duckdbt/ipython.py`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.0/duckdbt/load_db_profile.py` & `duckdbt-0.3.1/duckdbt/load_db_profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,42 @@
+import os
 from argparse import Namespace
 
 from dbt.adapters.duckdb.credentials import DuckDBCredentials
 from dbt.flags import set_from_args
 from dbt.config.project import load_raw_project
 from dbt.config.profile import read_profile, Profile
 from dbt.config.renderer import ProfileRenderer
 
 
-def load_duckdb_target(project_root: str = ".", profile_dir=".") -> DuckDBCredentials:
+def load_duckdb_target(project_root: str = ".") -> DuckDBCredentials:
     """Load the DuckDBCredentials from the profiles.yml file.
 
     This method was derived from the fal dbt adapter configuration
     defined here:
 
     https://github.com/fal-ai/fal/blob/main/projects/adapter/src/dbt/adapters/fal/load_db_profile.py
     """
     set_from_args(Namespace(STRICT_MODE=True), {})
-
     profile_renderer = ProfileRenderer()
     raw_project = load_raw_project(project_root)
     raw_profile_name = raw_project.get("profile")
     profile_name = profile_renderer.render_value(raw_profile_name)
-    raw_profiles = read_profile(profile_dir)
-    raw_profile = raw_profiles[profile_name]
+    raw_profile = None
+    for profile_dir in (".", os.path.join(os.getenv("HOME"), ".dbt")):
+        path = os.path.join(profile_dir, "profiles.yml")
+        if os.path.isfile(path):
+            raw_profiles = read_profile(profile_dir)
+            if profile_name in raw_profiles:
+                raw_profile = raw_profiles[profile_name]
+    if not raw_profile:
+        raise ValueError(
+            f"Could not find profile '{profile_name}' in ./profiles.yml or ~/.dbt/profiles.yml"
+        )
+
     if "target" in raw_profile:
         target_name = profile_renderer.render_value(raw_profile["target"])
     else:
         target_name = "default"
     target_dict = Profile._get_profile_data(
         profile=raw_profile,
         profile_name=profile_name,
```

### Comparing `duckdbt-0.3.0/duckdbt/server.py` & `duckdbt-0.3.1/duckdbt/server.py`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.0/duckdbt/static/dashboard.css` & `duckdbt-0.3.1/duckdbt/static/dashboard.css`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.0/duckdbt/static/favicon.ico` & `duckdbt-0.3.1/duckdbt/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.0/duckdbt/templates/index.html` & `duckdbt-0.3.1/duckdbt/templates/index.html`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.0/setup.py` & `duckdbt-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,30 +7,29 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 package_name = "duckdbt"
 
 
-package_version = "0.3.0"
+package_version = "0.3.1"
 description = """The Modern Data Stack in a Python Package"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh Wills",
     author_email="joshwills+duckdbt@gmail.com",
     url="https://github.com/jwills/duckdbt",
     packages=find_namespace_packages(include=["duckdbt", "duckdbt.*"]),
     include_package_data=True,
     install_requires=[
-        "buenavista~=0.2.1",
+        "buenavista[duckdb]~=0.2.1",
         "dbt-duckdb~=1.5.0",
         "duckdb~=0.7.0",
         "fastapi[all]",
-        "pyarrow",
-        "sqlglot",
+        "psycopg2-binary",
     ],
 )
```

