# Comparing `tmp/datoso-0.2.6.tar.gz` & `tmp/datoso-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso-0.2.6.tar", last modified: Mon May  8 22:50:17 2023, max compression
+gzip compressed data, was "datoso-0.2.7.tar", last modified: Mon May  8 22:55:35 2023, max compression
```

## Comparing `datoso-0.2.6.tar` & `datoso-0.2.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 22:50:01.000000 datoso-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-08 22:50:01.000000 datoso-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-08 22:50:17.008467 datoso-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-08 22:50:01.000000 datoso-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-08 22:50:01.000000 datoso-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 22:50:17.008467 datoso-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.004467 datoso-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.004467 datoso-0.2.6/src/datoso/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/actions/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/commands/doctor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/commands/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/configuration/folder_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/configuration/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/database/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/database/models/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/database/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/database/models/datfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/database/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/database/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/database/seeds/dat_repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/database/seeds/dat_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/datoso.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/helpers/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/helpers/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/repositories/dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/repositories/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/seeds/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/seeds/unknown_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/seeds.txt
--rw-r--r--   0 runner    (1001) docker     (123)    42230 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/systems.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-08 22:50:16.000000 datoso-0.2.6/src/datoso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 22:50:17.000000 datoso-0.2.6/src/datoso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:50:16.000000 datoso-0.2.6/src/datoso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 22:50:16.000000 datoso-0.2.6/src/datoso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-08 22:50:16.000000 datoso-0.2.6/src/datoso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 22:50:16.000000 datoso-0.2.6/src/datoso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 22:55:23.000000 datoso-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-08 22:55:23.000000 datoso-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-08 22:55:35.167677 datoso-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-08 22:55:23.000000 datoso-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-08 22:55:23.000000 datoso-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 22:55:35.171677 datoso-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.159677 datoso-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.163677 datoso-0.2.7/src/datoso/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18809 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/actions/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/commands/doctor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/commands/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/configuration/folder_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/configuration/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/database/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/database/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/database/models/datfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/database/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/database/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/database/seeds/dat_repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/database/seeds/dat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/datoso.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/helpers/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/helpers/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/repositories/dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/repositories/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/seeds/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/seeds/unknown_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/seeds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42230 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/systems.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-08 22:55:35.000000 datoso-0.2.7/src/datoso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 22:55:35.000000 datoso-0.2.7/src/datoso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:55:35.000000 datoso-0.2.7/src/datoso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 22:55:35.000000 datoso-0.2.7/src/datoso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-08 22:55:35.000000 datoso-0.2.7/src/datoso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 22:55:35.000000 datoso-0.2.7/src/datoso.egg-info/top_level.txt
```

### Comparing `datoso-0.2.6/LICENSE` & `datoso-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/PKG-INFO` & `datoso-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso-0.2.6/README.md` & `datoso-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/pyproject.toml` & `datoso-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/__main__.py` & `datoso-0.2.7/src/datoso/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
 
 
 def command_seed(args) -> None:
     """ Commands with the seed (must be installed) """
     if args.seed == 'all':
         for seed, _ in installed_seeds().items():
             seed = get_seed_name(seed)
-            if seed in args.exclude:
+            if args.exclude and seed in args.exclude:
                 continue
             if args.only and seed not in args.only:
                 continue
             if config['PROCESS'].get('SeedIgnoreRegEx'):
                 ignore_regex = re.compile(config['PROCESS']['SeedIgnoreRegEx'])
                 if ignore_regex.match(seed):
                     continue
```

### Comparing `datoso-0.2.6/src/datoso/actions/processor.py` & `datoso-0.2.7/src/datoso/actions/processor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/commands/doctor.py` & `datoso-0.2.7/src/datoso/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/commands/seed.py` & `datoso-0.2.7/src/datoso/commands/seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/configuration/folder_helper.py` & `datoso-0.2.7/src/datoso/configuration/folder_helper.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/configuration/logger.py` & `datoso-0.2.7/src/datoso/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/database/__init__.py` & `datoso-0.2.7/src/datoso/database/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/database/models/datfile.py` & `datoso-0.2.7/src/datoso/database/models/datfile.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/database/seeds/dat_repos.py` & `datoso-0.2.7/src/datoso/database/seeds/dat_repos.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/database/seeds/dat_rules.py` & `datoso-0.2.7/src/datoso/database/seeds/dat_rules.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/datoso.ini` & `datoso-0.2.7/src/datoso/datoso.ini`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/helpers/__init__.py` & `datoso-0.2.7/src/datoso/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/helpers/executor.py` & `datoso-0.2.7/src/datoso/helpers/executor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/helpers/plugins.py` & `datoso-0.2.7/src/datoso/helpers/plugins.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/repositories/dat.py` & `datoso-0.2.7/src/datoso/repositories/dat.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/repositories/dedupe.py` & `datoso-0.2.7/src/datoso/repositories/dedupe.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/seeds/unknown_seed.py` & `datoso-0.2.7/src/datoso/seeds/unknown_seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/seeds.txt` & `datoso-0.2.7/src/datoso/seeds.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso/systems.json` & `datoso-0.2.7/src/datoso/systems.json`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso.egg-info/PKG-INFO` & `datoso-0.2.7/src/datoso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso-0.2.6/src/datoso.egg-info/SOURCES.txt` & `datoso-0.2.7/src/datoso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.2.6/src/datoso.egg-info/requires.txt` & `datoso-0.2.7/src/datoso.egg-info/requires.txt`

 * *Files identical despite different names*

