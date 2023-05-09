# Comparing `tmp/duqtools-1.7.0.tar.gz` & `tmp/duqtools-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duqtools-1.7.0.tar", last modified: Tue Apr 11 09:45:53 2023, max compression
+gzip compressed data, was "duqtools-1.8.0.tar", last modified: Tue May  9 08:25:41 2023, max compression
```

## Comparing `duqtools-1.7.0.tar` & `duqtools-1.8.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.290567 duqtools-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 09:45:49.000000 duqtools-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 09:45:49.000000 duqtools-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-11 09:45:53.290567 duqtools-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-11 09:45:49.000000 duqtools-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-11 09:45:49.000000 duqtools-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-11 09:45:53.290567 duqtools-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:45:49.000000 duqtools-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.278567 duqtools-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.282567 duqtools-1.7.0/src/duqtools/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/_click_opt_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/_logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/_plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/apply_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.282567 duqtools-1.7.0/src/duqtools/config/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/config/_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/dash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.282567 duqtools-1.7.0/src/duqtools/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.286567 duqtools-1.7.0/src/duqtools/data/dash/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/dash/_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/dash/dash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.286567 duqtools-1.7.0/src/duqtools/data/dash/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/dash/pages/1_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/dash/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/dash/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/duqtools.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/jetto_tools_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/variables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/variables_core-profiles.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/variables_core-sources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/variables_equilibrium.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/variables_ids2jetto.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/duqmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.286567 duqtools-1.7.0/src/duqtools/ids/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_apply_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_imas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_rebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.286567 duqtools-1.7.0/src/duqtools/jetto/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/jetto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/jetto/_batchfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/jetto/_jettovar_to_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/jetto/_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.286567 duqtools-1.7.0/src/duqtools/large_scale_validation/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/list_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/matrix_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/merge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.286567 duqtools-1.7.0/src/duqtools/models/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/models/_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/models/_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/models/_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/models/_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.290567 duqtools-1.7.0/src/duqtools/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_basemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_description_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_imas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_jetto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/data_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/matrix_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.282567 duqtools-1.7.0/src/duqtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-11 09:45:53.000000 duqtools-1.7.0/src/duqtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-11 09:45:53.000000 duqtools-1.7.0/src/duqtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:45:53.000000 duqtools-1.7.0/src/duqtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 09:45:53.000000 duqtools-1.7.0/src/duqtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:45:52.000000 duqtools-1.7.0/src/duqtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-11 09:45:53.000000 duqtools-1.7.0/src/duqtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 09:45:53.000000 duqtools-1.7.0/src/duqtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.388682 duqtools-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 08:25:33.000000 duqtools-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-09 08:25:33.000000 duqtools-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-09 08:25:41.388682 duqtools-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-09 08:25:33.000000 duqtools-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-09 08:25:33.000000 duqtools-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-09 08:25:41.392682 duqtools-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 08:25:33.000000 duqtools-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.376681 duqtools-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.380682 duqtools-1.8.0/src/duqtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/_click_opt_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/_logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/_plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/apply_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.380682 duqtools-1.8.0/src/duqtools/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/config/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/config/_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/dash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.384682 duqtools-1.8.0/src/duqtools/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.384682 duqtools-1.8.0/src/duqtools/data/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/dash/_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/dash/dash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.384682 duqtools-1.8.0/src/duqtools/data/dash/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/dash/pages/1_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/dash/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/dash/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/duqtools.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/jetto_tools_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/variables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/variables_core-profiles.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/variables_core-sources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/variables_equilibrium.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/variables_ids2jetto.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/duqmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.384682 duqtools-1.8.0/src/duqtools/ids/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_apply_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_imas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_rebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.384682 duqtools-1.8.0/src/duqtools/jetto/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/jetto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/jetto/_batchfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/jetto/_jettovar_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/jetto/_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.384682 duqtools-1.8.0/src/duqtools/large_scale_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/list_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/matrix_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/merge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.388682 duqtools-1.8.0/src/duqtools/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/models/_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/models/_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/models/_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/models/_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.388682 duqtools-1.8.0/src/duqtools/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_description_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_imas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_jetto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/data_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/matrix_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.380682 duqtools-1.8.0/src/duqtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-09 08:25:41.000000 duqtools-1.8.0/src/duqtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-09 08:25:41.000000 duqtools-1.8.0/src/duqtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 08:25:41.000000 duqtools-1.8.0/src/duqtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-09 08:25:41.000000 duqtools-1.8.0/src/duqtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 08:25:40.000000 duqtools-1.8.0/src/duqtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-09 08:25:41.000000 duqtools-1.8.0/src/duqtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 08:25:41.000000 duqtools-1.8.0/src/duqtools.egg-info/top_level.txt
```

### Comparing `duqtools-1.7.0/LICENSE` & `duqtools-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/PKG-INFO` & `duqtools-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duqtools
-Version: 1.7.0
+Version: 1.8.0
 Summary: Dynamic uncertainty quantification for Tokamak reactor simulations modelling
 Home-page: https://github.com/duqtools/duqtools
 Author: Stef Smeets
 Author-email: s.smeets@esciencecenter.nl
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/duqtools/duqtools/issues
 Project-URL: Documentation, https://duqtools.readthedocs.io
```

### Comparing `duqtools-1.7.0/README.md` & `duqtools-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/pyproject.toml` & `duqtools-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/setup.cfg` & `duqtools-1.8.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = duqtools
 project_urls = 
 	Bug Tracker = https://github.com/duqtools/duqtools/issues
 	Documentation = https://duqtools.readthedocs.io
 url = https://github.com/duqtools/duqtools
-version = 1.7.0
+version = 1.8.0
 
 [options]
 zip_safe = False
 packages = find_namespace:
 package_dir = 
 	= src
 include_package_data = True
```

### Comparing `duqtools-1.7.0/src/duqtools/__init__.py` & `duqtools-1.8.0/src/duqtools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,18 +12,16 @@
     import pkg_resources  # noqa
 
 
 fix_dependencies()
 
 __author__ = 'Stef Smeets'
 __email__ = 's.smeets@esciencecenter.nl'
-__version__ = '1.7.0'
+__version__ = '1.8.0'
 
 import logging  # noqa
 import warnings  # noqa
 
-logging.basicConfig(level=logging.INFO)
-
 # https://github.com/duqtools/duqtools/issues/264
 warnings.filterwarnings(
     'ignore',
     'Explicit custom root behavior not yet implemented for pydantic_yaml')
```

### Comparing `duqtools-1.7.0/src/duqtools/_click_opt_groups.py` & `duqtools-1.8.0/src/duqtools/_click_opt_groups.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/_logging_utils.py` & `duqtools-1.8.0/src/duqtools/_logging_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,10 +58,7 @@
 
 
 def initialize_duqlog_screen():
     # Logger for stdout
     stream = logging.StreamHandler()
     stream.setFormatter(logging.Formatter('%(message)s'))
     duqlog_screen.addHandler(stream)
-
-
-initialize_duqlog_screen()
```

### Comparing `duqtools-1.7.0/src/duqtools/_plot_utils.py` & `duqtools-1.8.0/src/duqtools/_plot_utils.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/api.py` & `duqtools-1.8.0/src/duqtools/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,33 +15,36 @@
 Plotting:
 
 - [alt_errorband_chart][duqtools.api.alt_errorband_chart]
 - [alt_line_chart][duqtools.api.alt_line_chart]
 """
 
 from ._plot_utils import alt_errorband_chart, alt_line_chart
+from .create import create_api as create
 from .duqmap import duqmap
 from .ids import (
     IDSMapping,
     ImasHandle,
     rebase_all_coords,
     rebase_on_grid,
     rebase_on_time,
     standardize_grid_and_time,
 )
-from .models import Run, Runs
+from .models import Job, Run, Runs
 from .schema import IDSVariableModel as Variable
 
 __all__ = [
+    'create',
     'duqmap',
     'rebase_on_grid',
     'rebase_on_time',
     'rebase_all_coords',
     'standardize_grid_and_time',
     'ImasHandle',
     'IDSMapping',
+    'Job',
     'Variable',
     'alt_line_chart',
     'alt_errorband_chart',
     'Run',
     'Runs',
 ]
```

### Comparing `duqtools-1.7.0/src/duqtools/apply_model.py` & `duqtools-1.8.0/src/duqtools/apply_model.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/cleanup.py` & `duqtools-1.8.0/src/duqtools/cleanup.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/cli.py` & `duqtools-1.8.0/src/duqtools/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 from sys import exit, stderr, stdout
 from typing import Callable
 
 import click
 from pydantic import ValidationError
 
 from ._click_opt_groups import GroupCmd, GroupOpt
-from ._logging_utils import TermEscapeCodeFormatter, duqlog_screen
-from .config import cfg
+from ._logging_utils import TermEscapeCodeFormatter, duqlog_screen, initialize_duqlog_screen
+from .config import CFG, load_config
 from .operations import op_queue, op_queue_context
 
+logging.basicConfig(level=logging.INFO)
+initialize_duqlog_screen()
+
 logger = logging.getLogger(__name__)
 
 try:
     import coverage
     coverage.process_startup()
 except ImportError:
     pass
@@ -158,22 +161,22 @@
             f'{datetime.now().astimezone().strftime("%Y-%m-%d %H:%M:%S %z")}')
         logger.info('------------------------------------------------')
         logger.info('')
 
     def parse_quiet(self, *, quiet, **kwargs):
         if quiet:
             duqlog_screen.handlers = []  # remove output methods
-            cfg.quiet = True
+            CFG.quiet = True
 
     def parse_dry_run(self, *, dry_run, **kwargs):
         op_queue.dry_run = dry_run
 
     def parse_config(self, *, config, **kwargs):
         try:
-            cfg.parse_file(config)
+            load_config(config)
         except ValidationError as e:
             exit(e)
 
     def parse_yes(self, *, yes, **kwargs):
         op_queue.yes = yes
 
 
@@ -205,14 +208,26 @@
 
 
 @click.group()
 def cli(**kwargs):
     """For more information, check out the documentation:
 
     https://duqtools.readthedocs.io
+
+    \b
+    Example:
+    ```
+    duqtools init
+    duqtools create
+    duqtools submit --array --max_jobs 5
+    duqtools status
+    duqtools merge -i data.csv -t user1/jet/90123/1 -o user2/jet/90123/100
+    duqtools dash
+    ```
+    \f
     """
     pass
 
 
 @cli.command('init', cls=GroupCmd)
 @click.option('-o',
               '--out',
@@ -257,20 +272,23 @@
         setup(**kwargs)
 
 
 @cli.command('create', cls=GroupCmd)
 @click.option('--force',
               is_flag=True,
               help='Overwrite existing run directories and IDS data.')
+@click.option('--no-sampling',
+              is_flag=True,
+              help='Create base run (ignores `dimensions`/`sampler`).')
 @common_options(*all_options)
 def cli_create(**kwargs):
     """Create the UQ run files."""
-    from .create import create
+    from .create import create_entry
     with op_queue_context():
-        create(**kwargs)
+        create_entry(**kwargs)
 
 
 @cli.command('recreate', cls=GroupCmd)
 @click.argument('runs', type=Path, nargs=-1)
 @common_options(*all_options)
 def cli_recreate(**kwargs):
     """Read `runs.yaml` and re-create the given runs.
```

### Comparing `duqtools-1.7.0/src/duqtools/config/_variables.py` & `duqtools-1.8.0/src/duqtools/config/_variables.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/create.py` & `duqtools-1.8.0/src/duqtools/create.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from pathlib import Path
 from typing import Any, Sequence
 
 import pandas as pd
 
 from .apply_model import apply_model
 from .cleanup import remove_run
-from .config import Config, cfg
+from .config import Config
 from .ids import ImasHandle
 from .matrix_samplers import get_matrix_sampler
-from .models import Locations, Run, Runs
+from .models import Job, Locations, Run, Runs
 from .operations import add_to_op_queue, op_queue
 from .system import get_system
 
 logger = logging.getLogger(__name__)
 
 RUN_PREFIX = 'run_'
 
@@ -23,21 +23,23 @@
 class CreateError(Exception):
     ...
 
 
 class CreateManager:
     """Docstring for CreateManager."""
 
-    def __init__(self):
-        self.options = cfg.create
+    def __init__(self, cfg: Config):
+        self.cfg = cfg
 
-        if not self.options:
+        if not self.cfg.create:
             logger.warning('No create options specified.')
             raise CreateError('No create options specified in config.')
 
+        self.options = self.cfg.create
+
         self.template_drc = self.options.template
         self.system = get_system()
         self.runs_dir = self.system.get_runs_dir()
         self.source = self._get_source_handle()
 
         locations = Locations()
         self.runs_yaml = locations.runs_yaml
@@ -49,30 +51,48 @@
         else:
             source = ImasHandle.parse_obj(self.options.template_data)
 
         logger.info('Source data: %s', source)
 
         return source
 
-    def generate_ops_list(self) -> list[Any]:
+    def get_base_ops(self) -> list[Any]:
+        """Generate base operations that are always applied."""
+        base_ops = [op.convert() for op in self.options.operations]
+        return base_ops
+
+    def generate_ops_dict(self,
+                          *,
+                          base_only: bool = False) -> dict[str, list[Any]]:
         """Generate set of operations for a run."""
-        dimensions = self.options.dimensions
+        base_ops = self.get_base_ops()
+
+        if base_only:
+            return {'base': base_ops}
+
+        matrix = tuple(model.expand() for model in self.options.dimensions)
         matrix_sampler = get_matrix_sampler(self.options.sampler.method)
-        matrix = tuple(model.expand() for model in dimensions)
-        ops_list = matrix_sampler(*matrix, **dict(self.options.sampler))
 
-        return ops_list
+        sampled_ops_lists = matrix_sampler(*matrix,
+                                           **dict(self.options.sampler))
+
+        ops_dict = {}
+        for i, ops_list in enumerate(sampled_ops_lists):
+            name = f'{RUN_PREFIX}{i:04d}'
+            ops_dict[name] = [*base_ops, *ops_list]
+
+        return ops_dict
 
-    def make_run_models(self, ops_list: Sequence[Any],
+    def make_run_models(self, *, ops_dict: dict[str, list[Any]],
                         absolute_dirpath: bool) -> list[Run]:
         """Take list of operations and create run models."""
         run_models = []
 
-        for i, operations in enumerate(ops_list):
-            dirname = self.runs_dir / f'{RUN_PREFIX}{i:04d}'
+        for i, (name, operations) in enumerate(ops_dict.items()):
+            dirname = self.runs_dir / name
 
             data_in = self.system.get_data_in_handle(
                 dirname=dirname,
                 seq_number=i,
                 source=self.source,
                 options=self.options.data,
             )
@@ -81,15 +101,15 @@
                 dirname=dirname,
                 seq_number=i,
                 source=self.source,
                 options=self.options.data,
             )
 
             model = Run(dirname=dirname,
-                        shortname=dirname.name,
+                        shortname=name,
                         data_in=data_in,
                         data_out=data_out,
                         operations=operations)
 
             run_models.append(model)
 
         return run_models
@@ -154,34 +174,43 @@
 
             # Only if it is a different directory
             if self._is_runs_dir_different_from_config_dir():
                 with open(self.runs_dir / 'runs.yaml', 'w') as f:
                     runs.yaml(stream=f)
 
     @add_to_op_queue('Writing csv', quiet=True)
-    def write_runs_csv(self, runs: Sequence[Run], cfg: Config):
+    def write_runs_csv(self, runs: Sequence[Run]):
         fname = self.data_csv
 
-        prefix = f'{cfg.tag}.' if cfg.tag else ''
+        prefix = f'{self.cfg.tag}.' if self.cfg.tag else ''
 
         run_map = {
             f'{prefix}{run.shortname}': run.data_out.dict()
             for run in runs
         }
         df = pd.DataFrame.from_dict(run_map, orient='index')
         df.to_csv(fname)
 
         if self._is_runs_dir_different_from_config_dir():
             df.to_csv(self.runs_dir / fname)
 
-    @add_to_op_queue('Storing duqtools.yaml inside runs_dir', quiet=True)
-    def copy_config(self, config):
+    def copy_config(self):
+        if self.cfg._path is None:
+            return
+
         if self._is_runs_dir_different_from_config_dir():
-            shutil.copyfile(Path.cwd() / config,
-                            self.runs_dir / 'duqtools.yaml')
+            op_queue.add(
+                action=shutil.copyfile,
+                args=(
+                    Path.cwd() / self.cfg._path,
+                    self.runs_dir / 'duqtools.yaml',
+                ),
+                description='Copying config to run directory',
+                quiet=True,
+            )
 
     def _is_runs_dir_different_from_config_dir(self) -> bool:
         """Return True if the runs dir is different from the duqtools config
         dir."""
         return Path.cwd().resolve() != self.runs_dir.resolve()
 
     def create_run(self, model: Run, *, force: bool = False):
@@ -196,71 +225,106 @@
 
         self.source.copy_data_to(model.data_in)
 
         self.system.copy_from_template(self.template_drc, model.dirname)
 
         self.apply_operations(model.data_in, model.dirname, model.operations)
 
-        self.system.write_batchfile(model.dirname, cfg)
+        self.system.write_batchfile(model.dirname, self.cfg)
 
         self.system.update_imas_locations(run=model.dirname,
                                           inp=model.data_in,
                                           out=model.data_out)
 
 
-def create(*, force, config, absolute_dirpath: bool = False, **kwargs):
+def create(*,
+           cfg: Config,
+           force: bool = False,
+           no_sampling: bool = False,
+           absolute_dirpath: bool = False,
+           **kwargs) -> list[Run]:
     """Create input for jetto and IDS data structures.
 
     Parameters
     ----------
     force : bool
         Override protection if data and directories already exist.
-    config : Path
-        Config file location
+    cfg : Config
+        Duqtools config
+    no_sampling : bool
+        If true, create base run by ignoring `sampler`/`dimensions`.
 
     **kwargs
         Unused.
     """
-    create_mgr = CreateManager()
+    create_mgr = CreateManager(cfg)
 
-    ops_list = create_mgr.generate_ops_list()
+    ops_dict = create_mgr.generate_ops_dict(base_only=no_sampling)
 
-    runs = create_mgr.make_run_models(ops_list, absolute_dirpath)
+    runs = create_mgr.make_run_models(
+        ops_dict=ops_dict,
+        absolute_dirpath=absolute_dirpath,
+    )
 
     if not force:
 
         target_exists = any([
             create_mgr.runs_yaml_exists(),
             create_mgr.data_locations_exist(runs),
             create_mgr.run_dirs_exist(runs),
         ])
 
         if target_exists:
             create_mgr.warn_no_create_runs()
-            return
+            return []
 
     for model in runs:
         create_mgr.create_run(model, force=force)
 
     create_mgr.write_runs_file(runs)
-    create_mgr.write_runs_csv(runs, cfg)
-    create_mgr.copy_config(config)
+    create_mgr.write_runs_csv(runs)
+    create_mgr.copy_config()
+
+    return runs
+
+
+def create_entry(*args, **kwargs):
+    """Entry point for duqtools cli."""
+    from .config import CFG
+    create(cfg=CFG, *args, **kwargs)
+
+
+def create_api(config: dict, **kwargs) -> tuple[Job, Run]:
+    """Wrapper around create for python api."""
+    cfg = Config.from_dict(config)
+    runs = create(cfg=cfg, **kwargs)
+
+    if len(runs) == 0:
+        raise CreateError('No runs were created, check logs for errors.')
+    elif len(runs) > 1:
+        raise NotImplementedError('Multiple runs in single call not supported')
+
+    run = runs[0]
+    job = Job(run.dirname, cfg=cfg)
+
+    return job, run
 
 
 def recreate(*, runs: Sequence[Path], **kwargs):
     """Create input for jetto and IDS data structures.
 
     Parameters
     ----------
     runs : Sequence[Path]
         Run names to recreate.
     **kwargs
         Unused.
     """
-    create_mgr = CreateManager()
+    from .config import CFG
+    create_mgr = CreateManager(CFG)
 
     run_dict = {run.shortname: run for run in Locations().runs}
 
     run_models = []
     for run in runs:
         if run not in run_dict:
             raise ValueError(f'`{run}` not in `runs.yaml`.')
```

### Comparing `duqtools-1.7.0/src/duqtools/dash.py` & `duqtools-1.8.0/src/duqtools/dash.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/data/dash/_shared.py` & `duqtools-1.8.0/src/duqtools/data/dash/_shared.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/data/dash/dash.py` & `duqtools-1.8.0/src/duqtools/data/dash/dash.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/data/dash/pages/1_merge.py` & `duqtools-1.8.0/src/duqtools/data/dash/pages/1_merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,17 @@
     st.table(df)
 
 with st.sidebar:
     ids_variables = var_lookup.filter_type('IDS-variable')
 
     st.header('Merging options')
 
-    merge_all = st.checkbox('Merge all', help='Try to merge all variables.', value=True)
+    merge_all = st.checkbox('Merge all',
+                            help='Try to merge all variables.',
+                            value=True)
 
     var_names = st.multiselect('Select variables to merge',
                                tuple(ids_variables),
                                default=None,
                                disabled=merge_all)
 
 if merge_all:
@@ -90,25 +92,20 @@
 
     st.markdown('**Target IMAS entry**')
     st.write('The data will be stored in the DB entry given below.')
 
     cols = st.columns((20, 20, 30, 30))
 
     target = {
-        'user':
-        cols[0].text_input('User',
-                           value=getuser(),
-                           key='user_target',
-                           disabled=True),
-        'db':
-        cols[1].text_input('Machine', value=a_run.db, key='db_target'),
-        'shot':
-        cols[2].number_input('Shot', value=a_run.shot, key='shot_target'),
-        'run':
-        cols[3].number_input('Run', step=1, key='run_target'),
+        'user': cols[0].text_input('User', value=getuser(), key='user_target'),
+        'db': cols[1].text_input('Machine', value=a_run.db, key='db_target'),
+        'shot': cols[2].number_input('Shot',
+                                     value=a_run.shot,
+                                     key='shot_target'),
+        'run': cols[3].number_input('Run', step=1, key='run_target'),
     }
 
     target = ImasHandle(**target)
 
     submitted = st.form_submit_button('Save')
 
     if submitted:
```

### Comparing `duqtools-1.7.0/src/duqtools/data/jetto_tools_lookup.json` & `duqtools-1.8.0/src/duqtools/data/jetto_tools_lookup.json`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/data/variables.yaml` & `duqtools-1.8.0/src/duqtools/data/variables.yaml`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/data/variables_core-profiles.yaml` & `duqtools-1.8.0/src/duqtools/data/variables_core-profiles.yaml`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/data/variables_core-sources.yaml` & `duqtools-1.8.0/src/duqtools/data/variables_core-sources.yaml`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/data/variables_equilibrium.yaml` & `duqtools-1.8.0/src/duqtools/data/variables_equilibrium.yaml`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/data/variables_ids2jetto.yaml` & `duqtools-1.8.0/src/duqtools/data/variables_ids2jetto.yaml`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/duqmap.py` & `duqtools-1.8.0/src/duqtools/duqmap.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/ids/__init__.py` & `duqtools-1.8.0/src/duqtools/ids/__init__.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/ids/_apply_model.py` & `duqtools-1.8.0/src/duqtools/ids/_apply_model.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/ids/_copy.py` & `duqtools-1.8.0/src/duqtools/ids/_copy.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/ids/_handle.py` & `duqtools-1.8.0/src/duqtools/ids/_handle.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/ids/_imas.py` & `duqtools-1.8.0/src/duqtools/ids/_imas.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,8 +51,9 @@
     imas.ids = lambda *_, **__: ids
     imas.DBEntry = lambda *_, **__: entry
 
     imasdef = Mock()
 
     Parser = Mock()  # type: ignore
 
-    logger.warning('Could not import IMAS:', exc_info=True)
+if imas_mocked:
+    logger.info('Could not import IMAS, using mocks instead.')
```

### Comparing `duqtools-1.7.0/src/duqtools/ids/_mapping.py` & `duqtools-1.8.0/src/duqtools/ids/_mapping.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/ids/_merge.py` & `duqtools-1.8.0/src/duqtools/ids/_merge.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/ids/_rebase.py` & `duqtools-1.8.0/src/duqtools/ids/_rebase.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/init.py` & `duqtools-1.8.0/src/duqtools/init.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/jetto/_batchfile.py` & `duqtools-1.8.0/src/duqtools/jetto/_batchfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     Parameters
     ----------
     jobs : Sequence[Job]
         List of jobs to run.
     max_jobs : int
         Maximum number of jobs to run at the same time.
     """
-    common_dir = Path(commonpath(job.dir for job in jobs))  # type: ignore
+    common_dir = Path(commonpath(job.path for job in jobs))  # type: ignore
     logs_dir = common_dir / 'logs'
     logs_dir.mkdir(exist_ok=True)
 
     # Get the first jobs submission script as a template
     lines = open(jobs[0].submit_script)
     sbatch_lines = (line for line in lines if line.startswith('#SBATCH'))
     option_lines = (line for line in sbatch_lines
```

### Comparing `duqtools-1.7.0/src/duqtools/jetto/_jettovar_to_json.py` & `duqtools-1.8.0/src/duqtools/jetto/_jettovar_to_json.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/jetto/_system.py` & `duqtools-1.8.0/src/duqtools/jetto/_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pathlib import Path
 from typing import Any, List, Optional
 
 from jetto_tools import config, jset, lookup, namelist, template
 from jetto_tools import job as jetto_job
 from jetto_tools.template import _EXTRA_FILE_REGEXES
 
-from ..config import Config, cfg
+from ..config import CFG, Config
 from ..ids import ImasHandle
 from ..models import AbstractSystem, Job, Locations
 from ..operations import add_to_op_queue
 from ..schema import JettoVar
 from ._batchfile import write_array_batchfile as _write_array_batchfile
 from ._batchfile import write_batchfile as _write_batchfile
 from ._jettovar_to_json import jettovar_to_json
@@ -28,25 +28,47 @@
 
 logger = logging.getLogger(__name__)
 
 lookup_file = files('duqtools.data') / 'jetto_tools_lookup.json'
 jetto_lookup = lookup.from_file(lookup_file)
 
 
+def _get_jetto_extra(filenames: List[str], *, jset):
+    jetto_extra: List[str] = []
+    for regex in _EXTRA_FILE_REGEXES:
+        jetto_extra.extend(filter(regex.match, filenames))
+
+    if not jset.restart:
+        for fname in ('jetto.restart', 'jetto.srestart'):
+            try:
+                jetto_extra.remove(fname)
+            except ValueError:
+                pass
+    else:
+        if 'jetto.restart' in jetto_extra or 'jetto.srestart' in jetto_extra:
+            raise OSError(
+                'Template contains `jetto.restart` and/or `jetto.srestart` files. '
+                'Please remove these or turn "restart off" in JAMS'
+                'before running duqtools again.'
+                'More info: https://github.com/duqtools/duqtools/issues/498')
+
+    return jetto_extra
+
+
 class BaseJettoSystem(AbstractSystem):
     """System that can be used to create runs for jetto.
 
     This system can submit to various backends like docker, prominence
     and the gateway.
     """
 
     @staticmethod
     def get_runs_dir() -> Path:
         path = Locations().jruns_path
-        runs_dir = cfg.create.runs_dir  # type: ignore
+        runs_dir = CFG.create.runs_dir  # type: ignore
         if not runs_dir:
             abs_cwd = str(Path.cwd().resolve())
             abs_jruns = str(path.resolve())
             # Check if jruns is parent dir of current dir
             if abs_cwd.startswith(abs_jruns):
                 runs_dir = Path()
             else:  # jruns is somewhere else
@@ -63,16 +85,16 @@
     def write_batchfile(run_dir: Path, cfg: Config):
         jetto_jset = jset.read(run_dir / 'jetto.jset')
         _write_batchfile(run_dir, jetto_jset, tag=cfg.tag)
 
     @staticmethod
     def submit_job(job: Job):
         # Make sure we get a new correct status
-        if (job.dir / 'jetto.status').exists():
-            os.remove(job.dir / 'jetto.status')
+        if (job.path / 'jetto.status').exists():
+            os.remove(job.path / 'jetto.status')
 
         submit_system = job.cfg.submit.submit_system
 
         if submit_system == 'slurm':
             submit = JettoSystem.submit_slurm
         elif submit_system == 'docker':
             submit = JettoSystem.submit_docker
@@ -97,43 +119,43 @@
         ret = sp.run(cmd, check=True, capture_output=True)
         logger.info('submission returned: ' + str(ret.stdout))
         with open(job.lockfile, 'wb') as f:
             f.write(ret.stdout)
 
     @staticmethod
     def submit_docker(job: Job):
-        jetto_template = template.from_directory(job.dir)
+        jetto_template = template.from_directory(job.path)
         jetto_config = config.RunConfig(jetto_template)
         jetto_manager = jetto_job.JobManager()
         extra_volumes = {
-            job.dir.parent / 'imasdb': {
+            job.path.parent / 'imasdb': {
                 'bind': '/opt/imas/shared/imasdb',
                 'mode': 'rw'
             },
         }
 
         os.environ['RUNS_HOME'] = os.getcwd()
         os.environ['JINTRAC_IMAS_BACKEND'] = 'MDSPLUS'
         container = jetto_manager.submit_job_to_docker(
             jetto_config,
-            job.dir,
+            job.path,
             image=job.cfg.submit.docker_image,
             extra_volumes=extra_volumes)
         job.lockfile.touch()
         with open(job.lockfile, 'w') as f:
             f.write(container.name)
 
     @staticmethod
     def submit_prominence(job: Job):
-        jetto_template = template.from_directory(job.dir)
+        jetto_template = template.from_directory(job.path)
         jetto_config = config.RunConfig(jetto_template)
         jetto_manager = jetto_job.JobManager()
 
         os.environ['RUNS_HOME'] = os.getcwd()
-        _ = jetto_manager.submit_job_to_prominence(jetto_config, job.dir)
+        _ = jetto_manager.submit_job_to_prominence(jetto_config, job.path)
 
     @staticmethod
     def submit_array(jobs: Sequence[Job],
                      max_jobs: int,
                      max_array_size: int = 100):
         if jobs[0].cfg.submit.submit_system == 'slurm':
             JettoSystem.submit_array_slurm(jobs, max_jobs, max_array_size)
@@ -179,23 +201,15 @@
 
         jetto_sanco = None
         if (source_drc / 'jetto.sin').exists():
             jetto_sanco = namelist.read(source_drc / 'jetto.sin')
 
         all_files = os.listdir(source_drc)
 
-        jetto_extra: List[str] = []
-        for regex in _EXTRA_FILE_REGEXES:
-            jetto_extra.extend(filter(regex.match, all_files))
-
-        if 'jetto.restart' in jetto_extra or 'jetto.srestart' in jetto_extra:
-            raise OSError(
-                'Template contains `jetto.restart` and/or `jetto.srestart` files. '
-                'Please remove these before running duqtools again. '
-                'More info: https://github.com/duqtools/duqtools/issues/498')
+        jetto_extra = _get_jetto_extra(all_files, jset=jetto_jset)
 
         jetto_extra = [str(source_drc / file) for file in jetto_extra]
 
         jetto_template = template.Template(jset=jetto_jset,
                                            namelist=jetto_namelist,
                                            lookup=jetto_lookup,
                                            sanco_namelist=jetto_sanco,
```

### Comparing `duqtools-1.7.0/src/duqtools/large_scale_validation/merge.py` & `duqtools-1.8.0/src/duqtools/large_scale_validation/merge.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from typing import Sequence
 
 import pandas as pd
 
 from duqtools.api import ImasHandle
 
-from ..config import cfg
+from ..config import load_config
 from ..merge import _merge, _resolve_variables
 from ..models import Job, Locations
 from ..operations import add_to_op_queue, op_queue
 
 logger = logging.getLogger(__name__)
 
 
@@ -29,15 +29,18 @@
     config_files = cwd.glob('**/duqtools.yaml')
 
     target_handles = {}
 
     for config_file in config_files:
         run_name = config_file.parent.name
 
-        cfg.parse_file(config_file)
+        cfg = load_config(config_file)
+
+        assert cfg.create
+        assert cfg.create.runs_dir
 
         config_dir = config_file.parent
 
         runs = Locations(config_dir).runs
         runs = (run for run in runs if Job(run.dirname).is_completed)
         handles = (ImasHandle.parse_obj(run.data_out) for run in runs)
         handles = [handle for handle in handles if handle.exists()]
```

### Comparing `duqtools-1.7.0/src/duqtools/large_scale_validation/status.py` & `duqtools-1.8.0/src/duqtools/large_scale_validation/status.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 from pathlib import Path
 
 import click
 
-from ..config import cfg
+from ..config import load_config
 from ..models import Job, Locations
 from ..status import Status, StatusError
 
 
-def status(*, progress: bool, detailed: bool, **kwargs):
+def status(*, progress: bool, detailed: bool, pattern: str, **kwargs):
     """Show status of nested runs.
 
     Parameters
     ----------
     progress : bool
         Show progress bar.
     detailed : bool
         Show detailed progress for every job.
+    pattern : str
+        Show status only for subdirectories matching this glob pattern
     """
+    if pattern is None:
+        pattern = '**'
 
     cwd = Path.cwd()
 
-    config_files = cwd.glob('**/duqtools.yaml')
+    config_files = cwd.glob(f'{pattern}/duqtools.yaml')
 
     all_jobs: list[Job] = []
 
     click.echo(Job.status_symbol_help())
     click.echo()
 
     for config_file in config_files:
-        cfg.parse_file(config_file)
+        cfg = load_config(config_file)
 
         if not cfg.status:
             raise StatusError(
                 f'Status field required in config file: {config_file}')
 
         config_dir = config_file.parent
 
         jobs = [Job(run.dirname) for run in Locations(config_dir).runs]
         all_jobs.extend(jobs)
 
-        name = config_file.parent.name
+        dirname = config_file.parent.relative_to(cwd)
         tag = cfg.tag
         status = ''.join(job.status_symbol for job in jobs)
 
-        click.echo(f'{name} ({tag}): {status}')
+        click.echo(f'{dirname} ({tag}): {status}')
 
     click.echo()
 
     tracker = Status(all_jobs)
 
     if detailed:
         tracker.detailed_status()
```

### Comparing `duqtools-1.7.0/src/duqtools/large_scale_validation/submit.py` & `duqtools-1.8.0/src/duqtools/large_scale_validation/submit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,68 @@
 from collections import deque
 from pathlib import Path
 from typing import Deque, Sequence
 
-from ..config import cfg
+from ..config import load_config
 from ..models import Job, Locations
 from ..submit import (
-    SubmitError,
     job_array_submitter,
     job_scheduler,
     job_submitter,
     lockfile_ok,
     status_file_ok,
 )
+from ..utils import read_imas_handles_from_file
 
 
-def submit(*, array, force, max_jobs, schedule, status_filter: Sequence[str],
+def submit(*, array, force, max_jobs, schedule, max_array_size: int,
+           input_file: str, pattern: str, status_filter: Sequence[str],
            **kwargs):
     """Submit nested duqtools configs.
 
     Parameters
     ----------
     force : bool
         Force the submission even in the presence of lockfiles
     max_jobs : int
         Maximum number of jobs to submit at once
     schedule : bool
         Schedule `max_jobs` to run at once, keeps the process alive until
         finished.
+    max_array_size : int
+        Maximum array size for slurm (usually 1001, default = 100)
+    input_file : str
+        Only submit jobs for configs where template_data matches a handle in the data.csv
+    pattern : str
+        Find runs.yaml files only in subdirectories matching this glob pattern
     status_filter : list[str]
         Only submit jobs with this status.
     """
+    if pattern is None:
+        pattern = '**'
+
+    handles = None
+    if input_file:
+        handles = read_imas_handles_from_file(input_file).values()
+
     cwd = Path.cwd()
 
-    dirs = [file.parent for file in cwd.glob('**/runs.yaml')]
+    dirs = [file.parent for file in cwd.glob(f'{pattern}/runs.yaml')]
 
     jobs: list[Job] = []
 
-    for dir in dirs:
-        config_file = dir / 'duqtools.yaml'
-        cfg.parse_file(config_file)
-
-        if not cfg.submit:
-            raise SubmitError(
-                f'Submit field required in config file: {config_file}')
+    for drc in dirs:
+        config_file = drc / 'duqtools.yaml'
+        cfg = load_config(config_file)
+
+        assert cfg.create
+        assert cfg.submit
+
+        if handles and (cfg.create.template_data not in handles):
+            continue
 
         config_dir = config_file.parent
 
         jobs.extend(Job(run.dirname) for run in Locations(config_dir).runs)
 
     job_queue: Deque[Job] = deque()
 
@@ -59,8 +75,8 @@
             continue
         if not lockfile_ok(job, force=force):
             continue
         job_queue.append(job)
 
     submitter = job_scheduler if schedule else job_submitter
     submitter = job_array_submitter if array else submitter
-    submitter(job_queue, max_jobs=max_jobs)
+    submitter(job_queue, max_jobs=max_jobs, max_array_size=max_array_size)
```

### Comparing `duqtools-1.7.0/src/duqtools/list_variables.py` & `duqtools-1.8.0/src/duqtools/list_variables.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 from pydantic import ValidationError
 
-from duqtools.config import cfg, var_lookup
+from duqtools.config import load_config, var_lookup
 
 cs = click.style
 
 ST_ITEMS = {'fg': 'green', 'bold': True}
 ST_HEADER = {'fg': 'red', 'bold': True}
 ST_INFO = {'fg': 'white', 'bold': False}
 
@@ -34,15 +34,15 @@
     ----------
     config : str
         Name of the config file to use
     **kwargs
         Unused.
     """
     try:
-        cfg.parse_file(config)
+        cfg = load_config(config)
     except FileNotFoundError:
         print(f'Could not find: {config}')
     except ValidationError as e:
         exit(e)
         print(f'*: defined by {config}')
     finally:
         extra_variables = cfg.extra_variables.to_variable_dict(
```

### Comparing `duqtools-1.7.0/src/duqtools/matrix_samplers.py` & `duqtools-1.8.0/src/duqtools/matrix_samplers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import itertools
-from typing import Optional
+from typing import Any, Optional
 
 from scipy.stats import qmc
 
 
-def cartesian_product(*iterables, **kwargs):
+def cartesian_product(*iterables, **kwargs) -> list[Any]:
     """Return cartesian product of input iterables.
 
     Uses `itertools.product`
 
     Parameters
     ----------
     *iterables
@@ -18,15 +18,15 @@
     -------
     list[Any]
         List of product of input arguments.
     """
     return list(itertools.product(*iterables))
 
 
-def _sampler(func, *iterables, n_samples: int, **kwargs):
+def _sampler(func, *iterables, n_samples: int, **kwargs) -> list[Any]:
     """Generic sampler."""
     bounds = tuple(len(iterable) for iterable in iterables)
 
     sampler = func(d=len(iterables), **kwargs)
     indices = sampler.integers(l_bounds=bounds, n=n_samples)
 
     samples = []
@@ -35,15 +35,15 @@
 
     return samples
 
 
 def latin_hypercube(*iterables,
                     n_samples: int,
                     seed: Optional[int] = None,
-                    **kwargs):
+                    **kwargs) -> list[Any]:
     """Sample input iterables using Latin hypercube sampling (LHS).
 
     Uses `scipy.stats.qmc.LatinHyperCube`.
 
     Parameters
     ----------
     *iterables
@@ -60,15 +60,18 @@
     """
     return _sampler(qmc.LatinHypercube,
                     *iterables,
                     n_samples=n_samples,
                     seed=seed)
 
 
-def sobol(*iterables, n_samples: int, seed: Optional[int] = None, **kwargs):
+def sobol(*iterables,
+          n_samples: int,
+          seed: Optional[int] = None,
+          **kwargs) -> list[Any]:
     """Sample input iterables using the Sobol sampling method for generating
     low discrepancy sequences.
 
     Uses `scipy.stats.qmc.Sobol`.
 
     Parameters
     ----------
@@ -85,15 +88,18 @@
     -------
     samples : list[Any]
         List of sampled input arguments.
     """
     return _sampler(qmc.Sobol, *iterables, n_samples=n_samples, seed=seed)
 
 
-def halton(*iterables, n_samples: int, seed: Optional[int] = None, **kwargs):
+def halton(*iterables,
+           n_samples: int,
+           seed: Optional[int] = None,
+           **kwargs) -> list[Any]:
     """Sample input iterables using the Halton sampling method.
 
     Uses `scipy.stats.qmc.Halton`.
 
     Parameters
     ----------
     *iterables
```

### Comparing `duqtools-1.7.0/src/duqtools/merge.py` & `duqtools-1.8.0/src/duqtools/merge.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/models/_locations.py` & `duqtools-1.8.0/src/duqtools/models/_locations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os import getenv
 from pathlib import Path
 from typing import Optional
 
-from ..config import cfg
+from ..config import CFG
 from ._run import Run, Runs
 
 
 class Locations:
     """Class that knows about locations within a duqtools config directory.
 
     Defaults to local working directory, but can be initialized with a
@@ -51,13 +51,13 @@
         does not exists, return the current directory `./`.
 
         Returns
         -------
         Path
         """
 
-        if cfg.create.jruns:  # type: ignore
-            return cfg.create.jruns  # type: ignore
+        if CFG.create.jruns:  # type: ignore
+            return CFG.create.jruns  # type: ignore
         elif getenv('JRUNS'):
             return Path(getenv('JRUNS'))  # type: ignore
         else:
             return Path()
```

### Comparing `duqtools-1.7.0/src/duqtools/models/_run.py` & `duqtools-1.8.0/src/duqtools/models/_run.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,16 +31,23 @@
         handle = ImasHandle.parse_obj(self.data_out)
         return handle
 
     @classmethod
     def from_path(cls, path: Path):
         return cls(shortname=path, dirname=path.resolve())
 
+    @property
+    def is_base(self):
+        return self.shortname == 'base'
+
 
 class Runs(BaseModel):
     __root__: list[Run] = []
 
     def __iter__(self):
         yield from self.__root__
 
     def __getitem__(self, index: int):
         return self.__root__[index]
+
+    def __len__(self):
+        return len(self.__root__)
```

### Comparing `duqtools-1.7.0/src/duqtools/models/_system.py` & `duqtools-1.8.0/src/duqtools/models/_system.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/operations.py` & `duqtools-1.8.0/src/duqtools/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from inspect import signature
 from typing import Any, Callable, Optional, Sequence
 
 import click
 from pydantic import Field, validator
 
 from ._logging_utils import duqlog_screen
-from .config import cfg
+from .config import CFG
 from .schema import BaseModel
 
 logger = logging.getLogger(__name__)
 
 OP_STYLE = {'fg': 'green'}
 
 INFO_STYLE = {'fg': 'blue'}
@@ -209,19 +209,17 @@
         """Apply all queued operations and empty the queue.
 
         and show a fancy progress bar while applying
         """
         from tqdm import tqdm
         loginfo(style('Applying Operations', **HEADER_STYLE))  # type: ignore
 
-        if cfg.quiet:
+        if CFG.quiet:
             return self._apply_all()
 
-        print(self.n_actions)
-
         with tqdm(total=self.n_actions, position=1) as pbar:
             pbar.set_description('Progress')
 
             with tqdm(bar_format='{desc}') as dbar:
 
                 def callback(op):
                     if not op.action:
```

### Comparing `duqtools-1.7.0/src/duqtools/plot.py` & `duqtools-1.8.0/src/duqtools/plot.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/schema/__init__.py` & `duqtools-1.8.0/src/duqtools/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/schema/_dimensions.py` & `duqtools-1.8.0/src/duqtools/schema/_dimensions.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,27 +52,23 @@
     """))
 
     def expand(self, *args, **kwargs):
         from duqtools.config import var_lookup
         variable = var_lookup[self.variable]
 
         if isinstance(variable, JettoVariableModel):
-            return JettoOperationDim.expand(self,
-                                            *args,
-                                            variable=variable,
-                                            **kwargs)
+            expand_func = JettoOperationDim.expand
         elif isinstance(variable, IDSVariableModel):
-            return IDSOperationDim.expand(self,
-                                          *args,
-                                          variable=variable,
-                                          **kwargs)
+            expand_func = IDSOperationDim.expand
         else:
             raise NotImplementedError(
                 f'{self.variable} expand not implemented')
 
+        return expand_func(self, *args, variable=variable, **kwargs)
+
 
 class CoupledDim(BaseModel):
     __root__: list[OperationDim]
 
     @validator('__root__')
     def check_dimensions_match(cls, dims):
         if len(dims) > 0:
@@ -97,15 +93,15 @@
             """))
 
 
 class IDSOperation(IDSPathMixin, OperatorMixin, BaseModel):
     """Apply arithmetic operation to IDS."""
 
     value: float = Field(description=f("""
-        Values to use with operator on field to create sampling
+        Value to use with operator on field to create sampling
         space."""))
 
 
 class IDSOperationDim(IDSPathMixin, OperatorMixin, DimMixin, BaseModel):
     """Apply set of arithmetic operations to IDS.
 
     Takes the IDS data and subtracts, adds, multiplies, etc with each
@@ -124,21 +120,44 @@
 
 class JettoPathMixin(BaseModel):
     variable: JettoVariableModel
 
 
 class JettoOperation(JettoPathMixin, OperatorMixin, BaseModel):
     value: float = Field(description=f("""
-        Values to use with operator on field to create sampling
+        Value to use with operator on field to create sampling
         space."""))
 
 
 class JettoOperationDim(JettoPathMixin, OperatorMixin, DimMixin, BaseModel):
 
     def expand(self, *args, variable, **kwargs) -> tuple[JettoOperation, ...]:
         """Expand list of values into operations with its components."""
         return tuple(
             JettoOperation(variable=variable,
                            operator=self.operator,
                            value=value,
                            scale_to_error=self.scale_to_error)
             for value in self.values)
+
+
+class Operation(OperatorMixin, BaseModel):
+    variable: str
+    value: float
+
+    def convert(self):
+        """Expand variable and convert to correct type."""
+        from duqtools.config import var_lookup
+        variable = var_lookup[self.variable]
+
+        if isinstance(variable, JettoVariableModel):
+            cls = JettoOperation
+        elif isinstance(variable, IDSVariableModel):
+            cls = IDSOperation
+        else:
+            raise NotImplementedError(
+                f'{self.variable} convert not implemented')
+
+        mapping = self.dict()
+        mapping['variable'] = variable
+
+        return cls(**mapping)
```

### Comparing `duqtools-1.7.0/src/duqtools/schema/_imas.py` & `duqtools-1.8.0/src/duqtools/schema/_imas.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/schema/_jetto.py` & `duqtools-1.8.0/src/duqtools/schema/_jetto.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/schema/_ranges.py` & `duqtools-1.8.0/src/duqtools/schema/_ranges.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/schema/_variable.py` & `duqtools-1.8.0/src/duqtools/schema/_variable.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/schema/cli.py` & `duqtools-1.8.0/src/duqtools/schema/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,141 +1,153 @@
 from pathlib import Path
 from typing import Literal, Optional, Union
 
-from pydantic import DirectoryPath, Field, validator
+from pydantic import DirectoryPath, Field, PrivateAttr
 
 from ._basemodel import BaseModel
 from ._description_helpers import formatter as f
-from ._dimensions import CoupledDim, OperationDim
+from ._dimensions import CoupledDim, Operation, OperationDim
 from ._imas import ImasBaseModel
 from .data_location import DataLocation
 from .matrix_samplers import CartesianProduct, HaltonSampler, LHSSampler, SobolSampler
 from .variables import VariableConfigModel
 
 
 class CreateConfigModel(BaseModel):
     """The options of the `create` subcommand are stored in the `create` key in
     the config."""
-    dimensions: list[Union[CoupledDim, OperationDim]] = Field(description=f("""
-        The `dimensions` specifies the dimensions of the matrix to sample
-        from. Each dimension is a compound set of operations to apply.
-        From this, a matrix all possible combinations is generated.
-        Essentially, it generates the
-        [Cartesian product](en.wikipedia.org/wiki/Cartesian_product)
-        of all operations. By specifying a different `sampler`, a subset of
-        this hypercube can be efficiently sampled.
+    runs_dir: Optional[Path] = Field(description=f(
+        """Relative location from the workspace, which specifies the folder where to
+        store all the created runs.
+
+        This defaults to `workspace/duqtools_experiment_x`
+        where `x` is a not yet existing integer."""))
+
+    template: DirectoryPath = Field(description=f("""
+        Template directory to modify. Duqtools copies and updates the settings
+        required for the specified system from this directory. This can be a
+        directory with a finished run, or one just stored by JAMS (but not yet
+        started). By default, duqtools extracts the input IMAS database entry
+        from the settings file (e.g. jetto.in) to find the data to modify for
+        the UQ runs.
+        """))
+
+    template_data: Optional[ImasBaseModel] = Field(description=f("""
+        Specify the location of the template data to modify. This overrides the
+        location of the data specified in settings file in the template
+        directory.
         """))
 
+    operations: list[Operation] = Field(default=[],
+                                        description="""
+        These `operations` are always applied to the data.
+        All operations specified here are added to any operations sampled
+        from the dimensions.
+        They can be used to, for example, set the start time for an experiment
+        or update some physical parameters.
+        This parameter is optional.
+        """)
+
     sampler: Union[LHSSampler, HaltonSampler, SobolSampler,
                    CartesianProduct] = Field(default=CartesianProduct(),
                                              discriminator='method',
                                              description=f("""
         For efficient UQ, it may not be necessary to sample the entire matrix
         or hypercube. By default, the cartesian product is taken
         (`method: cartesian-product`). For more efficient sampling of the space,
         the following `method` choices are available:
         [`latin-hypercube`](en.wikipedia.org/wiki/Latin_hypercube_sampling),
         [`sobol`](en.wikipedia.org/wiki/Sobol_sequence),
         [`halton`](en.wikipedia.org/wiki/Halton_sequence).
         Where `n_samples` gives the number of samples to extract.
         """))
 
-    template: DirectoryPath = Field(description=f("""
-        Template directory to modify. Duqtools copies and updates the settings
-        required for the specified system from this directory. This can be a
-        directory with a finished run, or one just stored by JAMS (but not yet
-        started). By default, duqtools extracts the input IMAS database entry
-        from the settings file (e.g. jetto.in) to find the data to modify for
-        the UQ runs.
+    dimensions: list[Union[CoupledDim, OperationDim]] = Field(default=[],
+                                                              description=f("""
+        The `dimensions` specifies the dimensions of the matrix to sample
+        from. Each dimension is a compound set of operations to apply.
+        From this, a matrix all possible combinations is generated.
+        Essentially, it generates the
+        [Cartesian product](en.wikipedia.org/wiki/Cartesian_product)
+        of all operations. By specifying a different `sampler`, a subset of
+        this hypercube can be efficiently sampled. This paramater is optional.
         """))
 
-    template_data: Optional[ImasBaseModel] = Field(description=f("""
-        Specify the location of the template data to modify. This overrides the
-        location of the data specified in settings file in the template
-        directory.
+    jruns: Optional[DirectoryPath] = Field(description=f(
+        """`jruns` defines the the root directory where all simulations are
+        run for the jetto system. Because the jetto system works with relative
+        directories from some root directory.
+
+        This variable is optional. If this variable is not specified,
+        duqtools will look for the `$JRUNS` environment variable,
+        and set it to that. If that fails, `jruns` is set to the current directory `./`
+
+        In this way, duqtools can ensure that the current work directory is
+        a subdirectory of the given root directory. All subdirectories are
+        calculated as relative to the root directory.
+
+        For example, for `rjettov`, the root directory must be set to
+        `/pfs/work/$USER/jetto/runs/`. Any UQ runs must therefore be
+        a subdirectory.
+
         """))
 
     data: Optional[DataLocation] = Field(description=f("""
-        Required for `system: jetto-v210921`, irrelevant for other systems.
+        Required for `system: jetto-v210921`, ignored for other systems.
 
         Where to store the in/output IDS data.
         The data key specifies the machine or imas
         database name where to store the data (`imasdb`). duqtools will write the input
         data files for UQ start with the run number given by `run_in_start_at`.
         The data generated by the UQ runs (e.g. from jetto) will be stored
         starting by the run number given by `run_out_start_at`.
 
         """))
 
-    jruns: Optional[DirectoryPath] = Field(description=f(
-        """`jruns` defines the the root directory where all simulations are
-    run for the jetto system. Because the jettos system works with relative
-    directories from some root directory.
-
-    If this variable is not specified, duqtools will look for the `$JRUNS` environment
-    variable, and set it to that. If that fails, `jruns` is set to the current directory `./`
-
-    In this way, duqtools can ensure that the current work directory is
-    a subdirectory of the given root directory. All subdirectories are
-    calculated as relative to the root directory.
-
-    For example, for `rjettov`, the root directory must be set to
-    `/pfs/work/$USER/jetto/runs/`. Any UQ runs must therefore be
-    a subdirectory.
-
-    """))
-
-    runs_dir: Optional[Path] = Field(description=f(
-        """Relative location from the workspace, which specifies the folder where to
-    store all the created runs.
-
-    This defaults to `workspace/duqtools_experiment_x`
-    where `x` is a not yet existing integer."""))
-
 
 class SubmitConfigModel(BaseModel):
     """The options of the `submit` subcommand are stored under the `submit` key
     in the config.
 
     The config describes the commands to start the UQ runs.
     """
 
+    submit_system: Literal['prominence', 'slurm', 'docker'] = Field(
+        'slurm',
+        description='System to submit jobs to '
+        '[slurm (default), prominence, docker]')
     submit_script_name: str = Field(
         '.llcmd', description='Name of the submission script.')
     submit_command: str = Field('sbatch',
                                 description='Submission command for slurm.')
     docker_image: str = Field('jintrac-imas',
                               description='Docker image used for submission')
-    submit_system: Literal['prominence', 'slurm', 'docker'] = Field(
-        'slurm',
-        description='System to submit jobs to '
-        '[slurm (default), prominence, docker]')
 
 
 class StatusConfigModel(BaseModel):
     """The options of the `status` subcommand are stored under the `status` key
     in the config.
 
     These only need to be changed if the modeling software changes.
     """
-
-    status_file: str = Field('jetto.status',
-                             description='Name of the status file.')
     in_file: str = Field('jetto.in',
                          description=f("""
             Name of the modelling input file, will be used to check
             if the subprocess has started.
             """))
 
     out_file: str = Field('jetto.out',
                           description=f("""
             Name of the modelling output file, will be used to
             check if the software is running.
             """))
 
+    status_file: str = Field('jetto.status',
+                             description='Name of the status file.')
+
     msg_completed: str = Field('Status : Completed successfully',
                                description=f("""
             Parse `status_file` for this message to check for
             completion.
             """))
 
     msg_failed: str = Field('Status : Failed',
@@ -156,38 +168,33 @@
     tag: str = Field(
         '',
         description=
         'Create a tag for the runs to identify them in slurm or `data.csv`')
 
     submit: SubmitConfigModel = Field(
         SubmitConfigModel(),
-        description='Configuration for the submit subcommand')
+        description=
+        'Configuration for the submit subcommand. See model for more info.')
 
     create: Optional[CreateConfigModel] = Field(
-        description='Configuration for the create subcommand')
+        description=
+        'Configuration for the create subcommand. See model for more info.')
 
     status: StatusConfigModel = Field(
         StatusConfigModel(),
-        description='Configuration for the status subcommand')
-
-    workspace: Optional[str] = Field(description='Old field, currently unused')
+        description=
+        'Configuration for the status subcommand. See model for more info.')
 
     extra_variables: Optional[VariableConfigModel] = Field(
         description='Specify extra variables for this run.')
 
-    system: Literal['jetto', 'dummy', 'jetto-v210921',
-                    'jetto-v220922'] = Field(
-                        'jetto', description='backend system to use')
+    system: Literal[
+        'jetto', 'dummy', 'jetto-v210921', 'jetto-v220922'] = Field(
+            'jetto',
+            description='Backend system to use. See model for more info.')
 
     quiet: bool = Field(
         False,
-        description='dont output to stdout, except for mandatory prompts')
+        description=
+        'If true, do not output to stdout, except for mandatory prompts.')
 
-    @validator('workspace', pre=True)
-    def workspace_deprecated(cls, v):
-        if not v:
-            from warnings import warn
-            warn(f("""workspace key is Deprecated and unused, use create->jruns
-            and create->runs_dir to control where runs end up"""),
-                 DeprecationWarning,
-                 stacklevel=2)
-        return None
+    _path: Union[Path, str] = PrivateAttr(None)
```

### Comparing `duqtools-1.7.0/src/duqtools/schema/data_location.py` & `duqtools-1.8.0/src/duqtools/schema/data_location.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/schema/matrix_samplers.py` & `duqtools-1.8.0/src/duqtools/schema/matrix_samplers.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/schema/variables.py` & `duqtools-1.8.0/src/duqtools/schema/variables.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools/setup.py` & `duqtools-1.8.0/src/duqtools/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 from collections import defaultdict
 from pathlib import Path
 from types import SimpleNamespace
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Optional
 
 import yaml
 from jinja2 import Environment, FileSystemLoader
 
 from duqtools.api import ImasHandle
 from duqtools.config import var_lookup
 
@@ -146,65 +146,77 @@
         if value is None:
             raise AttributeError(
                 f'No value matches specifications given by: {spec}')
 
         return value
 
 
-def substitute_templates(*, handles: dict[str, ImasHandle], template_file: str,
-                         force: bool):
+def substitute_templates(
+    *,
+    handles: dict[str, ImasHandle],
+    template_file: str,
+    force: bool,
+    base: bool = False,
+    output: Optional[str] = None,
+):
     """Handle template substitution.
 
     Parameters
     ----------
     handles : dict[str, ImasHandle]
         Dictionary with Imas handles
     template_file : str
         Path to template file.
     force : bool
         Overwrite files if set to true.
+    output : str
+        Output subdirectory.
     """
     cwd = Path.cwd()
 
     template = get_template(template_file)
 
     if _get_key(template_file, key='system') == 'jetto-v210921':
         add_system_attrs = ExtrasV210921(template_file).add_system_attrs
     else:
         add_system_attrs = no_op  # default to no-op
 
     for name, handle in handles.items():
-        run = SimpleNamespace(name=name)
+        run = SimpleNamespace(name=name, output=output)
 
         add_system_attrs(run=run, handle=handle)
 
         variables = Variables(handle=handle)
 
         cfg = template.render(run=run, variables=variables, handle=handle)
 
         Config.parse_raw(cfg)  # make sure config is valid
 
-        out_drc = cwd / name
+        if output:
+            out_drc = cwd / output / name
+        else:
+            out_drc = cwd / name
 
         if out_drc.exists() and not force:
-            op_queue.add_no_op(description='Directory exists',
-                               extra_description=name)
+            op_queue.add_no_op(
+                description='Directory exists',
+                extra_description=f'{name} ({out_drc.relative_to(cwd)})')
             op_queue.warning(description='Warning',
                              extra_description='Some targets already exist, '
                              'use --force to override')
         else:
             op_queue.add(
                 action=_generate_run_dir,
                 kwargs={
                     'drc': out_drc,
                     'cfg': cfg,
                     'force': force
                 },
                 description='Setup run',
-                extra_description=name,
+                extra_description=f'{name} ({out_drc.relative_to(cwd)})',
             )
 
 
 def setup(*, handle, template_file, run_name, force, **kwargs):
     """Setup large scale validation runs for template.
 
     Parameters
```

### Comparing `duqtools-1.7.0/src/duqtools/status.py` & `duqtools-1.8.0/src/duqtools/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess as sp
 from collections import Counter
 from time import sleep
 from typing import Sequence
 
 from jetto_tools import config, template
 
-from .config import cfg
+from .config import CFG
 from .jetto._system import jetto_lookup
 from .models import Job, JobStatus, Locations
 
 logger = logging.getLogger(__name__)
 info, debug = logger.info, logger.debug
 stream = logging.StreamHandler()
 stream.setFormatter(logging.Formatter('%(message)s'))
@@ -108,15 +108,15 @@
     bars."""
 
     def __init__(self, pbar, job):
         self.pbar = pbar
         self.job = job
         self.outfile = None
 
-        jetto_template = template.from_directory(job.dir)
+        jetto_template = template.from_directory(job.path)
         jetto_template.lookup.update(jetto_lookup)
         jetto_config = config.RunConfig(jetto_template)
 
         self.check_kwmain_flag(jetto_config)
 
         infile = job.in_file
         if not infile.exists():
@@ -142,15 +142,15 @@
                ' is not set to 1 in `{self.job.status_file}`')
         if jetto_config['kwmain'] != 1:
             raise StatusError(msg)
 
     def set_status(self):
         status = self.job.status()
 
-        self.pbar.set_description(f'{self.job.dir.name:8s}, {status:12s}')
+        self.pbar.set_description(f'{self.job.path.name:8s}, {status:12s}')
         self.pbar.refresh()
 
         return status
 
     def get_steptime(self):
         if not self.job.out_file.exists():
             debug(
@@ -189,15 +189,15 @@
     Parameters
     ----------
     progress : bool
         Show progress bar.
     detailed : bool
         Show detailed progress for every job.
     """
-    debug('Submit config: %s', cfg.submit)
+    debug('Submit config: %s', CFG.submit)
 
     runs = Locations().runs
     jobs = [Job(run.dirname) for run in runs]
 
     tracker = Status(jobs)
 
     if detailed:
```

### Comparing `duqtools-1.7.0/src/duqtools/submit.py` & `duqtools-1.8.0/src/duqtools/submit.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 from collections import deque
 from itertools import cycle
 from pathlib import Path
 from typing import Deque, Sequence
 
 from ._logging_utils import duqlog_screen
-from .config import cfg
+from .config import CFG
 from .models import Job, Locations
 from .operations import add_to_op_queue, op_queue
 from .system import get_system
 
 logger = logging.getLogger(__name__)
 info, debug = logger.info, logger.debug
 
@@ -185,18 +185,18 @@
     resubmit : Sequence[Path]
         If any jobs need to be resubmitted, this is has a nonzero length, and
         contains a Sequence of Paths which either are the full Path to the run
         that needs to be resubmitted, or the shortname
     status_filter : list[str]
         Only submit jobs with this status.
     """
-    if not cfg.submit:
+    if not CFG.submit:
         raise SubmitError('Submit field required in config file')
 
-    debug('Submit config: %s', cfg.submit)
+    debug('Submit config: %s', CFG.submit)
 
     if resubmit:
         jobs = get_resubmit_jobs(resubmit)
         force = True
     else:
         jobs = [Job(run.dirname) for run in Locations().runs]
```

### Comparing `duqtools-1.7.0/src/duqtools/system.py` & `duqtools-1.8.0/src/duqtools/system.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from .config import Config, cfg
+from .config import CFG, Config
 from .ids import ImasHandle
 from .jetto import JettoSystemV210921, JettoSystemV220922
 from .models import AbstractSystem, Job
 
 
 class DummySystem(AbstractSystem):
     """This is a dummy system that implements the basic interfaces.
@@ -34,20 +34,22 @@
         return ImasHandle(db='', shot='-1', run='-1')
 
     @staticmethod
     def update_imas_locations(run: Path, inp, out):
         pass
 
 
-def get_system():
-    """get_system.
+def get_system(cfg=None):
+    """Get the system to do operations with.
 
-    Get the system to do operations with TODO make it a variable, not a
-    function
+    TODO make it a variable, not a function
     """
+    if cfg is None:
+        cfg = CFG
+
     if (cfg.system in ['jetto', 'jetto-v220922']):
         return JettoSystemV220922
     elif (cfg.system in ['jetto-v210921']):
         return JettoSystemV210921
     elif (cfg.system == 'dummy'):
         return DummySystem
     else:
```

### Comparing `duqtools-1.7.0/src/duqtools/utils.py` & `duqtools-1.8.0/src/duqtools/utils.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools.egg-info/PKG-INFO` & `duqtools-1.8.0/src/duqtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duqtools
-Version: 1.7.0
+Version: 1.8.0
 Summary: Dynamic uncertainty quantification for Tokamak reactor simulations modelling
 Home-page: https://github.com/duqtools/duqtools
 Author: Stef Smeets
 Author-email: s.smeets@esciencecenter.nl
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/duqtools/duqtools/issues
 Project-URL: Documentation, https://duqtools.readthedocs.io
```

### Comparing `duqtools-1.7.0/src/duqtools.egg-info/SOURCES.txt` & `duqtools-1.8.0/src/duqtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duqtools-1.7.0/src/duqtools.egg-info/requires.txt` & `duqtools-1.8.0/src/duqtools.egg-info/requires.txt`

 * *Files identical despite different names*

