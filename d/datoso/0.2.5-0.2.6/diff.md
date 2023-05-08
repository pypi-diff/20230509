# Comparing `tmp/datoso-0.2.5.tar.gz` & `tmp/datoso-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso-0.2.5.tar", last modified: Fri May  5 05:02:32 2023, max compression
+gzip compressed data, was "datoso-0.2.6.tar", last modified: Mon May  8 22:50:17 2023, max compression
```

## Comparing `datoso-0.2.5.tar` & `datoso-0.2.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:32.786608 datoso-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 05:02:16.000000 datoso-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 05:02:16.000000 datoso-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-05 05:02:32.786608 datoso-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-05 05:02:16.000000 datoso-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-05 05:02:16.000000 datoso-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 05:02:32.786608 datoso-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:32.778608 datoso-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:32.778608 datoso-0.2.5/src/datoso/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:32.782608 datoso-0.2.5/src/datoso/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/actions/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:32.782608 datoso-0.2.5/src/datoso/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/commands/doctor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/commands/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:32.782608 datoso-0.2.5/src/datoso/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/configuration/folder_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/configuration/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:32.782608 datoso-0.2.5/src/datoso/database/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:32.782608 datoso-0.2.5/src/datoso/database/models/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/database/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/database/models/datfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:32.786608 datoso-0.2.5/src/datoso/database/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/database/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/database/seeds/dat_repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/database/seeds/dat_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/datoso.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:32.786608 datoso-0.2.5/src/datoso/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/helpers/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/helpers/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:32.786608 datoso-0.2.5/src/datoso/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/repositories/dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/repositories/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:32.786608 datoso-0.2.5/src/datoso/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/seeds/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/seeds/unknown_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/seeds.txt
--rw-r--r--   0 runner    (1001) docker     (123)    42230 2023-05-05 05:02:16.000000 datoso-0.2.5/src/datoso/systems.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:02:32.782608 datoso-0.2.5/src/datoso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-05 05:02:32.000000 datoso-0.2.5/src/datoso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-05 05:02:32.000000 datoso-0.2.5/src/datoso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:02:32.000000 datoso-0.2.5/src/datoso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 05:02:32.000000 datoso-0.2.5/src/datoso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-05 05:02:32.000000 datoso-0.2.5/src/datoso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 05:02:32.000000 datoso-0.2.5/src/datoso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 22:50:01.000000 datoso-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-08 22:50:01.000000 datoso-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-08 22:50:17.008467 datoso-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-08 22:50:01.000000 datoso-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-08 22:50:01.000000 datoso-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 22:50:17.008467 datoso-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.004467 datoso-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.004467 datoso-0.2.6/src/datoso/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/actions/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/commands/doctor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/commands/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/configuration/folder_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/configuration/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/database/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/database/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/database/models/datfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/database/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/database/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/database/seeds/dat_repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/database/seeds/dat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/datoso.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/helpers/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/helpers/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/repositories/dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/repositories/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/seeds/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/seeds/unknown_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/seeds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42230 2023-05-08 22:50:01.000000 datoso-0.2.6/src/datoso/systems.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:50:17.008467 datoso-0.2.6/src/datoso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-08 22:50:16.000000 datoso-0.2.6/src/datoso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 22:50:17.000000 datoso-0.2.6/src/datoso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:50:16.000000 datoso-0.2.6/src/datoso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 22:50:16.000000 datoso-0.2.6/src/datoso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-08 22:50:16.000000 datoso-0.2.6/src/datoso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 22:50:16.000000 datoso-0.2.6/src/datoso.egg-info/top_level.txt
```

### Comparing `datoso-0.2.5/LICENSE` & `datoso-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/PKG-INFO` & `datoso-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Emulators
+Classifier: Topic :: System :: Archiving
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: fbneo
 Provides-Extra: md_enhanced
 Provides-Extra: nointro
 Provides-Extra: pleasuredome
```

### Comparing `datoso-0.2.5/README.md` & `datoso-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/pyproject.toml` & `datoso-0.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 requires-python = ">=3.10"
 license     = {text = "MIT License"}
 authors     = [
     {name = 'Lacides Miranda', email = 'laromicas@hotmail.com'},
 ]
 keywords = ["emulators", "roms"]
 classifiers = [
-    'Development Status :: 3 - Alpha',
+    'Development Status :: 4 - Beta',
     "Environment :: Console",
     'License :: OSI Approved :: MIT License',
     "Operating System :: POSIX :: Linux",
     'Programming Language :: Python :: 3',
     'Topic :: System :: Emulators',
+    'Topic :: System :: Archiving',
 ]
 dependencies = [
     "tinydb>=4.7.1",
     "pydantic>=1.10.7",
     "python-dateutil>=2.8.2",
     "xmltodict>=0.13.0",
     "tabulate>=0.9.0",
```

### Comparing `datoso-0.2.5/src/datoso/__main__.py` & `datoso-0.2.6/src/datoso/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
 
     group_dat= parser_dat.add_mutually_exclusive_group(required=True)
     group_dat.add_argument('-d', '--dat-name', help='Select dat to update/check, must be in format "seed:name"')
     group_dat.add_argument('-f', '--find', help='Select dats based on filter, they are "<field><operator><value>;...", valid operators are: =, !=, and ~=')
     group_dat.add_argument('-a', '--all', help='Show all dats', action='store_true')
 
     parser_dat.add_argument('-s', '--set', help='Manually set variable, must be in format "variable=value"')
+    parser_dat.add_argument('--delete', action='store_true', default=False, help='Delete Dat')
+
     parser_dat.add_argument('-on', '--only-names', action='store_true', help='Only show names')
 
     parser_dat.set_defaults(func=command_dat)
 
     # Seed admin commands
     parser_seed = subparser.add_parser('seed', help='Seed admin commands')
     subparser_seed = parser_seed.add_subparsers(help='sub-command help')
@@ -99,14 +101,17 @@
         seed = get_seed_name(seed)
         parser_command = subparser.add_parser(seed, help=f'Update seed {seed}')
         parser_command.set_defaults(func=command_seed, seed=seed)
         parser_command.add_argument('-f', '--fetch', action='store_true', help='Fetch seed')
         parser_command.add_argument('-p', '--process', action='store_true', help='Process dats from seed')
         parser_command.add_argument('-d', '--details', action='store_true', help='Show details of seed')
         parser_command.add_argument('-fd', '--filter', help='Filter dats to process')
+        if seed == 'all':
+            parser_command.add_argument('-e', '--exclude', action='append', help='Exclude seed or seeds (only work with all)')
+            parser_command.add_argument('-o', '--only', action='append', help='Only seed or seeds (only work with all)')
 
     # Common arguments
     subparsers = [subparser, subparser_seed]
     for subpars in subparsers:
         for subpar in subpars.choices.values():
             subpar.add_argument('-v', '--verbose', action='store_true', help='verbose output')
             subpar.add_argument('-q', '--quiet', action='store_true', help='quiet output')
@@ -233,14 +238,19 @@
                     value = int(value)
                 if value.lower() == 'true':
                     value = True
                 table.update({key: value}, doc_ids=[result.doc_id])
                 table.storage.flush()
                 print(f'{Bcolors.OKGREEN}Dat {Bcolors.OKCYAN}{seed}:{name}{Bcolors.OKGREEN} {key} set to {Bcolors.OKBLUE}{value}{Bcolors.ENDC}')
                 sys.exit(0)
+            if args.delete:
+                table.remove(doc_ids=[result.doc_id])
+                table.storage.flush()
+                print(f'{Bcolors.OKGREEN}Dat {Bcolors.OKCYAN}{seed}:{name}{Bcolors.OKGREEN} removed{Bcolors.ENDC}')
+                sys.exit(0)
             print_dats([result])
     elif args.all:
         # Show all dats
         print_dats(table.all())
 
     elif args.find:
         # Find dats TODO: finish
@@ -279,14 +289,18 @@
 
 
 def command_seed(args) -> None:
     """ Commands with the seed (must be installed) """
     if args.seed == 'all':
         for seed, _ in installed_seeds().items():
             seed = get_seed_name(seed)
+            if seed in args.exclude:
+                continue
+            if args.only and seed not in args.only:
+                continue
             if config['PROCESS'].get('SeedIgnoreRegEx'):
                 ignore_regex = re.compile(config['PROCESS']['SeedIgnoreRegEx'])
                 if ignore_regex.match(seed):
                     continue
             args.seed = seed
             command_seed(args)
         sys.exit(0)
```

### Comparing `datoso-0.2.5/src/datoso/actions/processor.py` & `datoso-0.2.6/src/datoso/actions/processor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/commands/doctor.py` & `datoso-0.2.6/src/datoso/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/commands/seed.py` & `datoso-0.2.6/src/datoso/commands/seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/configuration/folder_helper.py` & `datoso-0.2.6/src/datoso/configuration/folder_helper.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/configuration/logger.py` & `datoso-0.2.6/src/datoso/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/database/__init__.py` & `datoso-0.2.6/src/datoso/database/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/database/models/datfile.py` & `datoso-0.2.6/src/datoso/database/models/datfile.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/database/seeds/dat_repos.py` & `datoso-0.2.6/src/datoso/database/seeds/dat_repos.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/database/seeds/dat_rules.py` & `datoso-0.2.6/src/datoso/database/seeds/dat_rules.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/datoso.ini` & `datoso-0.2.6/src/datoso/datoso.ini`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/helpers/__init__.py` & `datoso-0.2.6/src/datoso/helpers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,18 @@
 
     @staticmethod
     def remove(path):
         """ Remove file or folder. """
         try:
             os.unlink(path)
         except IsADirectoryError:
-            shutil.rmtree(path)
+            try:
+                shutil.rmtree(path)
+            except PermissionError:
+                pass
         except FileNotFoundError:
             pass
 
     @staticmethod
     def parse_folder(path):
         """ Get folder from config. """
         if path is not None and path.startswith(('/', '~')):
@@ -119,9 +122,9 @@
 
     @staticmethod
     def move(origin, destination):
         """ Move file to destination. """
         os.makedirs(os.path.dirname(destination), exist_ok=True)
         try:
             shutil.move(origin, destination)
-        except shutil.Error:
+        except shutil.Error as error:
             FileUtils.remove(origin)
```

### Comparing `datoso-0.2.5/src/datoso/helpers/executor.py` & `datoso-0.2.6/src/datoso/helpers/executor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/helpers/plugins.py` & `datoso-0.2.6/src/datoso/helpers/plugins.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/repositories/dat.py` & `datoso-0.2.6/src/datoso/repositories/dat.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/repositories/dedupe.py` & `datoso-0.2.6/src/datoso/repositories/dedupe.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/seeds/unknown_seed.py` & `datoso-0.2.6/src/datoso/seeds/unknown_seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/seeds.txt` & `datoso-0.2.6/src/datoso/seeds.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso/systems.json` & `datoso-0.2.6/src/datoso/systems.json`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso.egg-info/PKG-INFO` & `datoso-0.2.6/src/datoso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Emulators
+Classifier: Topic :: System :: Archiving
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: fbneo
 Provides-Extra: md_enhanced
 Provides-Extra: nointro
 Provides-Extra: pleasuredome
```

### Comparing `datoso-0.2.5/src/datoso.egg-info/SOURCES.txt` & `datoso-0.2.6/src/datoso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.2.5/src/datoso.egg-info/requires.txt` & `datoso-0.2.6/src/datoso.egg-info/requires.txt`

 * *Files identical despite different names*

