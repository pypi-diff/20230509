# Comparing `tmp/ops-scenario-2.2.tar.gz` & `tmp/ops-scenario-3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-scenario-2.2.tar", last modified: Mon Apr 24 08:20:26 2023, max compression
+gzip compressed data, was "ops-scenario-3.0a1.tar", last modified: Tue May  9 11:10:22 2023, max compression
```

## Comparing `ops-scenario-2.2.tar` & `ops-scenario-3.0a1.tar`

### file list

```diff
@@ -1,62 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.261593 ops-scenario-2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.249593 ops-scenario-2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.253593 ops-scenario-2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-24 08:20:14.000000 ops-scenario-2.2/.github/workflows/build_wheels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-24 08:20:14.000000 ops-scenario-2.2/.github/workflows/quality_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 08:20:14.000000 ops-scenario-2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 08:20:14.000000 ops-scenario-2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29577 2023-04-24 08:20:26.261593 ops-scenario-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28953 2023-04-24 08:20:14.000000 ops-scenario-2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.253593 ops-scenario-2.2/ops_scenario.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29577 2023-04-24 08:20:26.000000 ops-scenario-2.2/ops_scenario.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-24 08:20:26.000000 ops-scenario-2.2/ops_scenario.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:20:26.000000 ops-scenario-2.2/ops_scenario.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 08:20:26.000000 ops-scenario-2.2/ops_scenario.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 08:20:26.000000 ops-scenario-2.2/ops_scenario.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 08:20:26.000000 ops-scenario-2.2/ops_scenario.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-24 08:20:14.000000 ops-scenario-2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.253593 ops-scenario-2.2/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-04-24 08:20:14.000000 ops-scenario-2.2/resources/state-transition-model.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.257593 ops-scenario-2.2/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/capture_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/consistency_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/fs_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/mocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/ops_main_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.257593 ops-scenario-2.2/scenario/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/scripts/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/scripts/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    29386 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/scripts/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    39970 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/state.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:20:26.261593 ops-scenario-2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.257593 ops-scenario-2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.257593 ops-scenario-2.2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/resources/demo_decorate_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_consistency_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.261593 ops-scenario-2.2/tests/test_e2e/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_builtin_scenes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_custom_event_triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_deferred.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_juju_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_observers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_play_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_rubbish_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_stored_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_vroot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_emitted_events_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-24 08:20:14.000000 ops-scenario-2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.795130 ops-scenario-3.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.787130 ops-scenario-3.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.787130 ops-scenario-3.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/.github/workflows/build_wheels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/.github/workflows/quality_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31728 2023-05-09 11:10:22.795130 ops-scenario-3.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30917 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.791130 ops-scenario-3.0a1/ops_scenario.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31728 2023-05-09 11:10:22.000000 ops-scenario-3.0a1/ops_scenario.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-09 11:10:22.000000 ops-scenario-3.0a1/ops_scenario.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:10:22.000000 ops-scenario-3.0a1/ops_scenario.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 11:10:22.000000 ops-scenario-3.0a1/ops_scenario.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 11:10:22.000000 ops-scenario-3.0a1/ops_scenario.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 11:10:22.000000 ops-scenario-3.0a1/ops_scenario.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.791130 ops-scenario-3.0a1/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/resources/state-transition-model.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.791130 ops-scenario-3.0a1/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/consistency_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/emitted_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/fs_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/ops_main_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.791130 ops-scenario-3.0a1/scenario/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/scripts/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/scripts/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29890 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/scripts/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40177 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:10:22.795130 ops-scenario-3.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.791130 ops-scenario-3.0a1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.791130 ops-scenario-3.0a1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/resources/demo_decorate_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_consistency_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.795130 ops-scenario-3.0a1/tests/test_e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_builtin_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_custom_event_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_deferred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_juju_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_observers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_play_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_rubbish_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_stored_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_vroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_emitted_events_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tox.ini
```

### Comparing `ops-scenario-2.2/.github/workflows/build_wheels.yaml` & `ops-scenario-3.0a1/.github/workflows/build_wheels.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 name: Build
 
 on:
   push:
     branches:
       - main
 
-
 jobs:
   build_wheel:
     name: Build wheel on ubuntu (where else???)
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
@@ -38,24 +37,24 @@
           prerelease: false
           tag_name: ${{ steps.get_version.outputs.VERSION }}
           release_name: ${{ steps.get_version.outputs.VERSION }}
 
         env:
           GITHUB_TOKEN: ${{ github.token }}
 
-#      - name: Setup upterm session
-#        uses: lhotari/action-upterm@v1
+      #      - name: Setup upterm session
+      #        uses: lhotari/action-upterm@v1
 
       - name: upload wheel
         uses: actions/upload-release-asset@v1
         env:
           GITHUB_TOKEN: ${{ github.token }}
         with:
           upload_url: ${{ steps.create_release.outputs.upload_url }}
           asset_path: ./dist/ops_scenario-${{ steps.get_version.outputs.VERSION }}-py3-none-any.whl
           asset_name: ops_scenario-${{ steps.get_version.outputs.VERSION }}-py3-none-any.whl
           asset_content_type: application/wheel
 
       - name: Publish to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
+          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `ops-scenario-2.2/.github/workflows/quality_checks.yaml` & `ops-scenario-3.0a1/.github/workflows/quality_checks.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 name: Tests
 
 on:
   pull_request:
     branches:
       - main
 
-
 jobs:
   linting:
     name: Linting
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v3
```

### Comparing `ops-scenario-2.2/LICENSE.txt` & `ops-scenario-3.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.2/PKG-INFO` & `ops-scenario-3.0a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,108 +1,127 @@
 Metadata-Version: 2.1
 Name: ops-scenario
-Version: 2.2
+Version: 3.0a1
 Summary: Python library providing a Scenario-based testing API for Operator Framework charms.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
-Project-URL: Homepage, https://github.com/PietroPasotti/ops-scenario
-Project-URL: Bug Tracker, https://github.com/PietroPasotti/ops-scenario/issues
+Project-URL: Homepage, https://github.com/canonical/ops-scenario
+Project-URL: Bug Tracker, https://github.com/canonical/ops-scenario/issues
 Keywords: juju,test
 Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-Scenario
-============
+# Scenario
+
+[![Build](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml)
+[![QC](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml)
+[![Discourse Status](https://img.shields.io/discourse/status?server=https%3A%2F%2Fdiscourse.charmhub.io&style=flat&label=CharmHub%20Discourse)](https://discourse.charmhub.io)
+[![foo](https://img.shields.io/badge/everything-charming-blueviolet)](https://github.com/PietroPasotti/jhack) 
+[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://discourse.charmhub.io/t/rethinking-charm-testing-with-ops-scenario/8649)
 
-This is a state transition testing framework for Operator Framework charms.
+Scenario is a state-transition, functional testing framework for Operator Framework charms.
 
-Where the Harness enables you to procedurally mock pieces of the state the charm needs to function, Scenario tests allow
-you to declaratively define the state all at once, and use it as a sort of context against which you can fire a single
-event on the charm and execute its logic.
+Where the Harness enables you to procedurally mock pieces of the state the charm needs to function, Scenario tests allow you to declaratively define the state all at once, and use it as a sort of context against which you can fire a single event on the charm and execute its logic.
 
-This puts scenario tests somewhere in between unit and integration tests.
+This puts scenario tests somewhere in between unit and integration tests: some say 'functional', some say 'contract'.
 
-Scenario tests nudge you into thinking of charms as an input->output function. Input is what we call a `Scene`: the
+Scenario tests nudge you into thinking of a charm as an input->output function. Input is what we call a `Scene`: the
 union of an `Event` (why am I being executed) and a `State` (am I leader? what is my relation data? what is my
-config?...).
-The output is another context instance: the context after the charm has had a chance to interact with the mocked juju
-model.
+config?...). The output is another context instance: the context after the charm has had a chance to interact with the
+mocked juju model and affect the state back.
 
 ![state transition model depiction](resources/state-transition-model.png)
 
 Scenario-testing a charm, then, means verifying that:
 
 - the charm does not raise uncaught exceptions while handling the scene
 - the output state (or the diff with the input state) is as expected.
 
-
 # Core concepts as a metaphor
+
 I like metaphors, so here we go:
+
 - There is a theatre stage.
 - You pick an actor (a Charm) to put on the stage. Not just any actor: an improv one.
 - You arrange the stage with content that the actor will have to interact with. This consists of selecting:
-    - An initial situation (State) in which the actor is, e.g. is the actor the main role or an NPC (is_leader), or what other actors are there around it, what is written in those pebble-shaped books on the table?
-    - Something that has just happened (an Event) and to which the actor has to react (e.g. one of the NPCs leaves the stage (relation-departed), or the content of one of the books changes).
-- How the actor will react to the event will have an impact on the context: e.g. the actor might knock over a table (a container), or write something down into one of the books.
-
+  - An initial situation (State) in which the actor is, e.g. is the actor the main role or an NPC (is_leader), or what
+    other actors are there around it, what is written in those pebble-shaped books on the table?
+  - Something that has just happened (an Event) and to which the actor has to react (e.g. one of the NPCs leaves the
+    stage (relation-departed), or the content of one of the books changes).
+- How the actor will react to the event will have an impact on the context: e.g. the actor might knock over a table (a
+  container), or write something down into one of the books.
 
 # Core concepts not as a metaphor
-Scenario tests are about running assertions on atomic state transitions treating the charm being tested like a black box.
-An initial state goes in, an event occurs (say, `'start'`) and a new state comes out.
-Scenario tests are about validating the transition, that is, consistency-checking the delta between the two states, and verifying the charm author's expectations.
+
+Scenario tests are about running assertions on atomic state transitions treating the charm being tested like a black
+box. An initial state goes in, an event occurs (say, `'start'`) and a new state comes out. Scenario tests are about
+validating the transition, that is, consistency-checking the delta between the two states, and verifying the charm
+author's expectations.
 
 Comparing scenario tests with `Harness` tests:
-- Harness exposes an imperative API: the user is expected to call methods on the Harness driving it to the desired state, then verify its validity by calling charm methods or inspecting the raw data.
-- Harness instantiates the charm once, then allows you to fire multiple events on the charm, which is breeding ground for subtle bugs. Scenario tests are centered around testing single state transitions, that is, one event at a time. This ensures that the execution environment is as clean as possible (for a unit test).
-- Harness maintains a model of the juju Model, which is a maintenance burden and adds complexity. Scenario mocks at the level of hook tools and stores all mocking data in a monolithic data structure (the State), which makes it more lightweight and portable.
-- TODO: Scenario can mock at the level of hook tools. Decoupling charm and context allows us to swap out easily any part of this flow, and even share context data across charms, codebases, teams...
+
+- Harness exposes an imperative API: the user is expected to call methods on the Harness driving it to the desired
+  state, then verify its validity by calling charm methods or inspecting the raw data.
+- Harness instantiates the charm once, then allows you to fire multiple events on the charm, which is breeding ground
+  for subtle bugs. Scenario tests are centered around testing single state transitions, that is, one event at a time.
+  This ensures that the execution environment is as clean as possible (for a unit test).
+- Harness maintains a model of the juju Model, which is a maintenance burden and adds complexity. Scenario mocks at the
+  level of hook tools and stores all mocking data in a monolithic data structure (the State), which makes it more
+  lightweight and portable.
+- TODO: Scenario can mock at the level of hook tools. Decoupling charm and context allows us to swap out easily any part
+  of this flow, and even share context data across charms, codebases, teams...
 
 # Writing scenario tests
+
 A scenario test consists of three broad steps:
 
-- Arrange:
-    - declare the input state
-    - select an event to fire
-- Act:
-    - run the state (i.e. obtain the output state)
-- Assert:
-    - verify that the output state is how you expect it to be
-    - verify that the delta with the input state is what you expect it to be
+- **Arrange**:
+  - declare the input state
+  - select an event to fire
+- **Act**:
+  - run the state (i.e. obtain the output state)
+  - optionally, use pre-event and post-event hooks to get a hold of the charm instance and run assertions on internal APIs
+- **Assert**:
+  - verify that the output state is how you expect it to be
+  - optionally, verify that the delta with the input state is what you expect it to be
 
 The most basic scenario is the so-called `null scenario`: one in which all is defaulted and barely any data is
 available. The charm has no config, no relations, no networks, and no leadership.
 
 With that, we can write the simplest possible scenario test:
 
 ```python
-from scenario.state import State
+from scenario import State, Context
 from ops.charm import CharmBase
 from ops.model import UnknownStatus
 
 class MyCharm(CharmBase):
     pass
 
 
 def test_scenario_base():
-    out = State().trigger(
-        'start', 
-        MyCharm, meta={"name": "foo"})
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', State())
     assert out.status.unit == UnknownStatus()
 ```
 
-Now let's start making it more complicated.
-Our charm sets a special state if it has leadership on 'start':
+Now let's start making it more complicated. Our charm sets a special state if it has leadership on 'start':
 
 ```python
 import pytest
-from scenario.state import State
+from scenario import State, Context
 from ops.charm import CharmBase
 from ops.model import ActiveStatus
 
 
 class MyCharm(CharmBase):
     def __init__(self, ...):
         self.framework.observe(self.on.start, self._on_start)
@@ -112,29 +131,29 @@
             self.unit.status = ActiveStatus('I rule')
         else:
             self.unit.status = ActiveStatus('I am ruled')
 
 
 @pytest.mark.parametrize('leader', (True, False))
 def test_status_leader(leader):
-    out = State(leader=leader).trigger(
-        'start', 
-        MyCharm,
-        meta={"name": "foo"})
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', 
+                  State(leader=leader)
     assert out.status.unit == ActiveStatus('I rule' if leader else 'I am ruled')
 ```
 
-By defining the right state we can programmatically define what answers will the charm get to all the questions it can ask the juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
-
+By defining the right state we can programmatically define what answers will the charm get to all the questions it can
+ask the juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
 
 ## Statuses
 
-One of the simplest types of black-box testing available to charmers is to execute the charm and verify that the charm sets the expected unit/application status.
-We have seen a simple example above including leadership.
-But what if the charm transitions through a sequence of statuses?
+One of the simplest types of black-box testing available to charmers is to execute the charm and verify that the charm
+sets the expected unit/application status. We have seen a simple example above including leadership. But what if the
+charm transitions through a sequence of statuses?
 
 ```python
 from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, BlockedStatus
 
 # charm code:
 def _on_event(self, _event):
     self.unit.status = MaintenanceStatus('determining who the ruler is...')
@@ -150,195 +169,225 @@
 ```
 
 You can verify that the charm has followed the expected path by checking the **unit status history** like so:
 
 ```python
 from charm import MyCharm
 from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, UnknownStatus
-from scenario import State
+from scenario import State, Context
 
 def test_statuses():
-    out = State(leader=False).trigger(
-        'start',
-        MyCharm,
-        meta={"name": "foo"})
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', 
+                  State(leader=False)) 
     assert out.status.unit_history == [
       UnknownStatus(),
       MaintenanceStatus('determining who the ruler is...'),
       WaitingStatus('checking this is right...'),
       ActiveStatus("I am ruled"),
     ]
 ```
 
 Note that the current status is not in the **unit status history**.
 
-Also note that, unless you initialize the State with a preexisting status, the first status in the history will always be `unknown`. That is because, so far as scenario is concerned, each event is "the first event this charm has ever seen".
+Also note that, unless you initialize the State with a preexisting status, the first status in the history will always
+be `unknown`. That is because, so far as scenario is concerned, each event is "the first event this charm has ever
+seen".
 
-If you want to simulate a situation in which the charm already has seen some event, and is in a status other than Unknown (the default status every charm is born with), you will have to pass the 'initial status' to State.
+If you want to simulate a situation in which the charm already has seen some event, and is in a status other than
+Unknown (the default status every charm is born with), you will have to pass the 'initial status' to State.
 
 ```python
 from ops.model import ActiveStatus
 from scenario import State, Status
 State(leader=False, status=Status(unit=ActiveStatus('foo')))
 ```
 
-
 ## Relations
 
 You can write scenario tests to verify the shape of relation data:
 
 ```python
 from ops.charm import CharmBase
 
-from scenario.state import Relation, State
+from scenario import Relation, State, Context
 
 
 # This charm copies over remote app data to local unit data
 class MyCharm(CharmBase):
     ...
 
     def _on_event(self, e):
         rel = e.relation
         assert rel.app.name == 'remote'
         assert rel.data[self.unit]['abc'] == 'foo'
         rel.data[self.unit]['abc'] = rel.data[e.app]['cde']
 
 
 def test_relation_data():
-    out = State(relations=[
+    state_in = State(relations=[
         Relation(
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "foo"},
             remote_app_data={"cde": "baz!"},
         ),
-    ]
-    ).trigger("start", MyCharm, meta={"name": "foo"})
+    ])
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    
+    state_out = ctx.run('start', state_in) 
 
-    assert out.relations[0].local_unit_data == {"abc": "baz!"}
+    assert state_out.relations[0].local_unit_data == {"abc": "baz!"}
     # you can do this to check that there are no other differences:
-    assert out.relations == [
+    assert state_out.relations == [
         Relation(
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "baz!"},
             remote_app_data={"cde": "baz!"},
         ),
     ]
 
 # which is very idiomatic and superbly explicit. Noice.
 ```
 
-The only mandatory argument to `Relation` (and other relation types, see below) is `endpoint`. The `interface` will be derived from the charm's `metadata.yaml`. When fully defaulted, a relation is 'empty'. There are no remote units, the remote application is called `'remote'` and only has a single unit `remote/0`, and nobody has written any data to the databags yet.
+The only mandatory argument to `Relation` (and other relation types, see below) is `endpoint`. The `interface` will be
+derived from the charm's `metadata.yaml`. When fully defaulted, a relation is 'empty'. There are no remote units, the
+remote application is called `'remote'` and only has a single unit `remote/0`, and nobody has written any data to the
+databags yet.
 
 That is typically the state of a relation when the first unit joins it.
 
-When you use `Relation`, you are specifying a regular (conventional) relation. But that is not the only type of relation. There are also
-peer relations and subordinate relations. While in the background the data model is the same, the data access rules and the consistency constraints on them are very different. For example, it does not make sense for a peer relation to have a different 'remote app' than its 'local app', because it's the same application.    
+When you use `Relation`, you are specifying a regular (conventional) relation. But that is not the only type of
+relation. There are also peer relations and subordinate relations. While in the background the data model is the same,
+the data access rules and the consistency constraints on them are very different. For example, it does not make sense
+for a peer relation to have a different 'remote app' than its 'local app', because it's the same application.
 
 ### PeerRelation
-To declare a peer relation, you should use `scenario.state.PeerRelation`.
-The core difference with regular relations is that peer relations do not have a "remote app" (it's this app, in fact).
-So unlike `Relation`, a `PeerRelation` does not have `remote_app_name` or `remote_app_data` arguments. Also, it talks in terms of `peers`:
-- `Relation.remote_unit_ids` maps to `PeerRelation.peers_ids` 
-- `Relation.remote_units_data` maps to `PeerRelation.peers_data` 
+
+To declare a peer relation, you should use `scenario.state.PeerRelation`. The core difference with regular relations is
+that peer relations do not have a "remote app" (it's this app, in fact). So unlike `Relation`, a `PeerRelation` does not
+have `remote_app_name` or `remote_app_data` arguments. Also, it talks in terms of `peers`:
+
+- `Relation.remote_unit_ids` maps to `PeerRelation.peers_ids`
+- `Relation.remote_units_data` maps to `PeerRelation.peers_data`
 
 ```python
 from scenario.state import PeerRelation
 
 relation = PeerRelation(
     endpoint="peers",
     peers_data={1: {}, 2: {}, 42: {'foo': 'bar'}},
 )
 ```
 
-be mindful when using `PeerRelation` not to include **"this unit"**'s ID in `peers_data` or `peers_ids`, as that would be flagged by the Consistency Checker:
+be mindful when using `PeerRelation` not to include **"this unit"**'s ID in `peers_data` or `peers_ids`, as that would
+be flagged by the Consistency Checker:
+
 ```python
-from scenario import State, PeerRelation
+from scenario import State, PeerRelation, Context
 
-State(relations=[
+state_in = State(relations=[
     PeerRelation(
         endpoint="peers",
         peers_data={1: {}, 2: {}, 42: {'foo': 'bar'}},
-    )]).trigger("start", ..., unit_id=1)  # invalid: this unit's id cannot be the ID of a peer.
+    )],
+    unit_id=1)
+
+Context(...).run("start", state_in)  # invalid: this unit's id cannot be the ID of a peer.
 
 
 ```
 
 ### SubordinateRelation
-To declare a subordinate relation, you should use `scenario.state.SubordinateRelation`.
-The core difference with regular relations is that subordinate relations always have exactly one remote unit (there is always exactly one primary unit that this unit can see). 
-So unlike `Relation`, a `SubordinateRelation` does not have a `remote_units_data` argument. Instead, it has a `remote_unit_data` taking a single `Dict[str:str]`, and takes the primary unit ID as a separate argument.
-Also, it talks in terms of `primary`:
-- `Relation.remote_unit_ids` becomes `SubordinateRelation.primary_id` (a single ID instead of a list of IDs) 
-- `Relation.remote_units_data` becomes `SubordinateRelation.remote_unit_data` (a single databag instead of a mapping from unit IDs to databags) 
+
+To declare a subordinate relation, you should use `scenario.state.SubordinateRelation`. The core difference with regular
+relations is that subordinate relations always have exactly one remote unit (there is always exactly one primary unit
+that this unit can see). So unlike `Relation`, a `SubordinateRelation` does not have a `remote_units_data` argument.
+Instead, it has a `remote_unit_data` taking a single `Dict[str:str]`, and takes the primary unit ID as a separate
+argument. Also, it talks in terms of `primary`:
+
+- `Relation.remote_unit_ids` becomes `SubordinateRelation.primary_id` (a single ID instead of a list of IDs)
+- `Relation.remote_units_data` becomes `SubordinateRelation.remote_unit_data` (a single databag instead of a mapping
+  from unit IDs to databags)
 - `Relation.remote_app_name` maps to `SubordinateRelation.primary_app_name`
 
 ```python
 from scenario.state import SubordinateRelation
 
 relation = SubordinateRelation(
     endpoint="peers",
     remote_unit_data={"foo": "bar"},
     primary_app_name="zookeeper",
     primary_id=42
 )
 relation.primary_name  # "zookeeper/42"
 ```
 
-
 ## Triggering Relation Events
-If you want to trigger relation events, the easiest way to do so is get a hold of the Relation instance and grab the event from one of its aptly-named properties:
+
+If you want to trigger relation events, the easiest way to do so is get a hold of the Relation instance and grab the
+event from one of its aptly-named properties:
 
 ```python
 from scenario import Relation
 relation = Relation(endpoint="foo", interface="bar")
 changed_event = relation.changed_event
 joined_event = relation.joined_event
 # ...
 ```
 
 This is in fact syntactic sugar for:
+
 ```python
 from scenario import Relation, Event
 relation = Relation(endpoint="foo", interface="bar")
 changed_event = Event('foo-relation-changed', relation=relation)
 ```
 
-The reason for this construction is that the event is associated with some relation-specific metadata, that Scenario needs to set up the process that will run `ops.main` with the right environment variables.
+The reason for this construction is that the event is associated with some relation-specific metadata, that Scenario
+needs to set up the process that will run `ops.main` with the right environment variables.
 
 ### Additional event parameters
-All relation events have some additional metadata that does not belong in the Relation object, such as, for a relation-joined event, the name of the (remote) unit that is joining the relation. That is what determines what `ops.model.Unit` you get when you get `RelationJoinedEvent().unit` in an event handler.
 
-In order to supply this parameter, you will have to **call** the event object and pass as `remote_unit_id` the id of the remote unit that the event is about.
-The reason that this parameter is not supplied to `Relation` but to relation events, is that the relation already ties 'this app' to some 'remote app' (cfr. the `Relation.remote_app_name` attr), but not to a specific unit. What remote unit this event is about is not a `State` concern but an `Event` one.  
+All relation events have some additional metadata that does not belong in the Relation object, such as, for a
+relation-joined event, the name of the (remote) unit that is joining the relation. That is what determines what
+`ops.model.Unit` you get when you get `RelationJoinedEvent().unit` in an event handler.
+
+In order to supply this parameter, you will have to **call** the event object and pass as `remote_unit_id` the id of the
+remote unit that the event is about. The reason that this parameter is not supplied to `Relation` but to relation
+events, is that the relation already ties 'this app' to some 'remote app' (cfr. the `Relation.remote_app_name` attr),
+but not to a specific unit. What remote unit this event is about is not a `State` concern but an `Event` one.
 
-The `remote_unit_id` will default to the first ID found in the relation's `remote_unit_ids`, but if the test you are writing is close to that domain, you should probably override it and pass it manually.
+The `remote_unit_id` will default to the first ID found in the relation's `remote_unit_ids`, but if the test you are
+writing is close to that domain, you should probably override it and pass it manually.
 
 ```python
 from scenario import Relation, Event
 relation = Relation(endpoint="foo", interface="bar")
 remote_unit_2_is_joining_event = relation.joined_event(remote_unit_id=2)
 
 # which is syntactic sugar for:
 remote_unit_2_is_joining_event = Event('foo-relation-changed', relation=relation, relation_remote_unit_id=2)
 ```
 
-
 ## Containers
 
-When testing a kubernetes charm, you can mock container interactions.
-When using the null state (`State()`), there will be no containers. So if the charm were to `self.unit.containers`, it would get back an empty dict.
+When testing a kubernetes charm, you can mock container interactions. When using the null state (`State()`), there will
+be no containers. So if the charm were to `self.unit.containers`, it would get back an empty dict.
 
 To give the charm access to some containers, you need to pass them to the input state, like so:
 `State(containers=[...])`
 
 An example of a scene including some containers:
+
 ```python
 from scenario.state import Container, State
 state = State(containers=[
     Container(name="foo", can_connect=True),
     Container(name="bar", can_connect=False)
 ])
 ```
@@ -359,28 +408,30 @@
               can_connect=True,
               mounts={'local': Mount('/local/share/config.yaml', local_file)})
 ]
 )
 ```
 
 In this case, if the charm were to:
+
 ```python
 def _on_start(self, _):
     foo = self.unit.get_container('foo')
     content = foo.pull('/local/share/config.yaml').read()
 ```
 
-then `content` would be the contents of our locally-supplied `file.txt`. You can use `tempdir` for nicely wrapping strings and passing them to the charm via the container.
+then `content` would be the contents of our locally-supplied `file.txt`. You can use `tempdir` for nicely wrapping
+strings and passing them to the charm via the container.
 
 `container.push` works similarly, so you can write a test like:
 
 ```python
 import tempfile
 from ops.charm import CharmBase
-from scenario.state import State, Container, Mount
+from scenario import State, Container, Mount, Context
 
 
 class MyCharm(CharmBase):
     def __init__(self, *args):
         super().__init__(*args)
         self.framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
 
@@ -390,39 +441,45 @@
 
 
 def test_pebble_push():
     with tempfile.NamedTemporaryFile() as local_file:
         container = Container(name='foo',
                               can_connect=True,
                               mounts={'local': Mount('/local/share/config.yaml', local_file.name)})
-        out = State(
+        state_in = State(
             containers=[container]
-        ).trigger(
-            container.pebble_ready_event,
+        )
+        Context(
             MyCharm,
-            meta={"name": "foo", "containers": {"foo": {}}},
+            meta={"name": "foo", "containers": {"foo": {}}}).run(
+            "start",
+            state_in,
         )
         assert local_file.read().decode() == "TEST"
 ```
 
-`container.pebble_ready_event` is syntactic sugar for: `Event("foo-pebble-ready", container=container)`. The reason we need to associate the container with the event is that the Framework uses an envvar to determine which container the pebble-ready event is about (it does not use the event name). Scenario needs that information, similarly, for injecting that envvar into the charm's runtime.
-
-`container.exec` is a tad more complicated, but if you get to this low a level of simulation, you probably will have far worse issues to deal with.
-You need to specify, for each possible command the charm might run on the container, what the result of that would be: its return code, what will be written to stdout/stderr.
+`container.pebble_ready_event` is syntactic sugar for: `Event("foo-pebble-ready", container=container)`. The reason we
+need to associate the container with the event is that the Framework uses an envvar to determine which container the
+pebble-ready event is about (it does not use the event name). Scenario needs that information, similarly, for injecting
+that envvar into the charm's runtime.
+
+`container.exec` is a tad more complicated, but if you get to this low a level of simulation, you probably will have far
+worse issues to deal with. You need to specify, for each possible command the charm might run on the container, what the
+result of that would be: its return code, what will be written to stdout/stderr.
 
 ```python
 from ops.charm import CharmBase
 
-from scenario.state import State, Container, ExecOutput
+from scenario import State, Container, ExecOutput, Context
 
 LS_LL = """
-.rw-rw-r--  228 ubuntu ubuntu 18 jan 12:05 -- charmcraft.yaml    
-.rw-rw-r--  497 ubuntu ubuntu 18 jan 12:05 -- config.yaml        
-.rw-rw-r--  900 ubuntu ubuntu 18 jan 12:05 -- CONTRIBUTING.md    
-drwxrwxr-x    - ubuntu ubuntu 18 jan 12:06 -- lib                
+.rw-rw-r--  228 ubuntu ubuntu 18 jan 12:05 -- charmcraft.yaml
+.rw-rw-r--  497 ubuntu ubuntu 18 jan 12:05 -- config.yaml
+.rw-rw-r--  900 ubuntu ubuntu 18 jan 12:05 -- CONTRIBUTING.md
+drwxrwxr-x    - ubuntu ubuntu 18 jan 12:06 -- lib
 """
 
 
 class MyCharm(CharmBase):
     def _on_start(self, _):
         foo = self.unit.get_container('foo')
         proc = foo.exec(['ls', '-ll'])
@@ -435,145 +492,160 @@
         name='foo',
         exec_mock={
             ('ls', '-ll'):  # this is the command we're mocking
                 ExecOutput(return_code=0,  # this data structure contains all we need to mock the call.
                            stdout=LS_LL)
         }
     )
-    out = State(
+    state_in = State(
         containers=[container]
-    ).trigger(
-        container.pebble_ready_event,
+    )
+    state_out = Context(
         MyCharm,
         meta={"name": "foo", "containers": {"foo": {}}},
+    ).run(
+        container.pebble_ready_event,
+        state_in,
     )
 ```
 
-
 # Deferred events
-Scenario allows you to accurately simulate the Operator Framework's event queue. The event queue is responsible for keeping track of the deferred events.
-On the input side, you can verify that if the charm triggers with this and that event in its queue (they would be there because they had been deferred in the previous run), then the output state is valid.
+
+Scenario allows you to accurately simulate the Operator Framework's event queue. The event queue is responsible for
+keeping track of the deferred events. On the input side, you can verify that if the charm triggers with this and that
+event in its queue (they would be there because they had been deferred in the previous run), then the output state is
+valid.
 
 ```python
-from scenario import State, deferred
+from scenario import State, deferred, Context
 
 
 class MyCharm(...):
     ...
+
     def _on_update_status(self, e):
         e.defer()
+
     def _on_start(self, e):
         e.defer()
 
-        
+
 def test_start_on_deferred_update_status(MyCharm):
     """Test charm execution if a 'start' is dispatched when in the previous run an update-status had been deferred."""
-    out = State(
-      deferred=[
-            deferred('update_status', 
+    state_in = State(
+        deferred=[
+            deferred('update_status',
                      handler=MyCharm._on_update_status)
         ]
-    ).trigger('start', MyCharm)
-    assert len(out.deferred) == 1
-    assert out.deferred[0].name == 'start'
+    )
+    state_out = Context(MyCharm).run('start', state_in)
+    assert len(state_out.deferred) == 1
+    assert state_out.deferred[0].name == 'start'
 ```
 
-You can also generate the 'deferred' data structure (called a DeferredEvent) from the corresponding Event (and the handler):
+You can also generate the 'deferred' data structure (called a DeferredEvent) from the corresponding Event (and the
+handler):
 
 ```python
 from scenario import Event, Relation
 
 class MyCharm(...):
     ...
 
 deferred_start = Event('start').deferred(MyCharm._on_start)
 deferred_install = Event('install').deferred(MyCharm._on_start)
 ```
 
 ## relation events:
-```python   
-foo_relation = Relation('foo') 
+
+```python
+foo_relation = Relation('foo')
 deferred_relation_changed_evt = foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
 ```
-On the output side, you can verify that an event that you expect to have been deferred during this trigger, has indeed been deferred.
+
+On the output side, you can verify that an event that you expect to have been deferred during this trigger, has indeed
+been deferred.
 
 ```python
-from scenario import State
+from scenario import State, Context
 
 
 class MyCharm(...):
     ...
     def _on_start(self, e):
         e.defer()
 
-        
+
 def test_defer(MyCharm):
-    out = State().trigger('start', MyCharm)
+    out = Context(MyCharm).run('start', State())
     assert len(out.deferred) == 1
     assert out.deferred[0].name == 'start'
 ```
-    
+
 ## Deferring relation events
-If you want to test relation event deferrals, some extra care needs to be taken. RelationEvents hold references to the Relation instance they are about. So do they in Scenario. You can use the deferred helper to generate the data structure:
+
+If you want to test relation event deferrals, some extra care needs to be taken. RelationEvents hold references to the
+Relation instance they are about. So do they in Scenario. You can use the deferred helper to generate the data
+structure:
 
 ```python
 from scenario import State, Relation, deferred
 
 
 class MyCharm(...):
     ...
     def _on_foo_relation_changed(self, e):
         e.defer()
 
-        
+
 def test_start_on_deferred_update_status(MyCharm):
-    foo_relation = Relation('foo') 
+    foo_relation = Relation('foo')
     State(
       relations=[foo_relation],
       deferred=[
-            deferred('foo_relation_changed', 
+            deferred('foo_relation_changed',
                      handler=MyCharm._on_foo_relation_changed,
                      relation=foo_relation)
         ]
     )
 ```
+
 but you can also use a shortcut from the relation event itself, as mentioned above:
 
 ```python
 
 from scenario import Relation
 
 class MyCharm(...):
     ...
 
-foo_relation = Relation('foo') 
+foo_relation = Relation('foo')
 foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
 ```
 
 ### Fine-tuning
 
-The deferred helper Scenario provides will not support out of the box all custom event subclasses, or events emitted by charm libraries or objects other than the main charm class.
+The deferred helper Scenario provides will not support out of the box all custom event subclasses, or events emitted by
+charm libraries or objects other than the main charm class.
 
 For general-purpose usage, you will need to instantiate DeferredEvent directly.
 
 ```python
 from scenario import DeferredEvent
 
 my_deferred_event = DeferredEvent(
    handle_path='MyCharm/MyCharmLib/on/database_ready[1]',
    owner='MyCharmLib',  # the object observing the event. Could also be MyCharm.
    observer='_on_database_ready'
 )
 ```
 
-
 # StoredState
 
-Scenario can simulate StoredState.
-You can define it on the input side as:
+Scenario can simulate StoredState. You can define it on the input side as:
 
 ```python
 from ops.charm import CharmBase
 from ops.framework import StoredState as Ops_StoredState, Framework
 from scenario import State, StoredState
 
 
@@ -592,129 +664,166 @@
     content={
       'foo': 'bar',
       'baz': {42: 42},
     })
 ])
 ```
 
-And the charm's runtime will see `self.stored_State.foo` and `.baz` as expected.
-Also, you can run assertions on it on the output side the same as any other bit of state.
-
+And the charm's runtime will see `self.stored_State.foo` and `.baz` as expected. Also, you can run assertions on it on
+the output side the same as any other bit of state.
 
 # Emitted events
-If your charm deals with deferred events, custom events, and charm libs that in turn emit their own custom events, it can be hard to examine the resulting control flow.
-In these situations it can be useful to verify that, as a result of a given juju event triggering (say, 'start'), a specific chain of deferred and custom events is emitted on the charm. The resulting state, black-box as it is, gives little insight into how exactly it was obtained. `scenario.capture_events` allows you to open a peephole and intercept any events emitted by the framework. 
 
-Usage: 
+If your charm deals with deferred events, custom events, and charm libs that in turn emit their own custom events, it
+can be hard to examine the resulting control flow. In these situations it can be useful to verify that, as a result of a
+given juju event triggering (say, 'start'), a specific chain of deferred and custom events is emitted on the charm. The
+resulting state, black-box as it is, gives little insight into how exactly it was obtained. 
+
+`scenario`, among many other great things, is also a pytest plugin. It exposes a fixture called `emitted_events` that you can use like so:
+
+```python
+from scenario import Context
+from ops.charm import StartEvent
+
+def test_foo(emitted_events):
+
+  Context(...).run('start', ...)
+
+  assert len(emitted_events) == 1
+  assert isinstance(emitted_events[0], StartEvent)
+```
+
+
+## Customizing: capture_events
+If you need more control over what events are captured (or you're not into pytest), you can use directly the context manager that powers the `emitted_events` fixture: `scenario.capture_events`.
+This context manager allows you to intercept any events emitted by the framework.
+
+Usage:
 
 ```python
 from ops.charm import StartEvent, UpdateStatusEvent
-from scenario import State, DeferredEvent
-from scenario import capture_events
+from scenario import State, Context, DeferredEvent, capture_events
 with capture_events() as emitted:
-    state_out = State(deferred=[DeferredEvent('start', ...)]).trigger('update-status', ...)
+    ctx = Context(...)
+    state_out = ctx.run(
+      "update-status",
+      State(deferred=[DeferredEvent("start", ...)])
+    )
 
 # deferred events get reemitted first
 assert isinstance(emitted[0], StartEvent)
 # the main juju event gets emitted next
 assert isinstance(emitted[1], UpdateStatusEvent)
 # possibly followed by a tail of all custom events that the main juju event triggered in turn
 # assert isinstance(emitted[2], MyFooEvent)
-# ... 
+# ...
 ```
 
-
 You can filter events by type like so:
 
 ```python
 from ops.charm import StartEvent, RelationEvent
 from scenario import capture_events
 with capture_events(StartEvent, RelationEvent) as emitted:
     # capture all `start` and `*-relation-*` events.
-    pass  
+    pass
 ```
 
 Passing no event types, like: `capture_events()`, is equivalent to `capture_events(EventBase)`.
 
-By default, **framework events** (`PreCommit`, `Commit`) are not considered for inclusion in the output list even if they match the instance check. You can toggle that by passing: `capture_events(include_framework=True)`.
-
-By default, **deferred events** are included in the listing if they match the instance check. You can toggle that by passing:
-`capture_events(include_deferred=True)`.
+By default, **framework events** (`PreCommit`, `Commit`) are not considered for inclusion in the output list even if
+they match the instance check. You can toggle that by passing: `capture_events(include_framework=True)`.
 
+By default, **deferred events** are included in the listing if they match the instance check. You can toggle that by
+passing: `capture_events(include_deferred=True)`.
 
 # The virtual charm root
-Before executing the charm, Scenario writes the metadata, config, and actions `yaml`s to a temporary directory. 
-The charm will see that tempdir as its 'root'. This allows us to keep things simple when dealing with metadata that can 
-be either inferred from the charm type being passed to `trigger()` or be passed to it as an argument, thereby overriding
+
+Before executing the charm, Scenario writes the metadata, config, and actions `yaml`s to a temporary directory. The
+charm will see that tempdir as its 'root'. This allows us to keep things simple when dealing with metadata that can be
+either inferred from the charm type being passed to `Context` or be passed to it as an argument, thereby overriding
 the inferred one. This also allows you to test with charms defined on the fly, as in:
 
 ```python
 from ops.charm import CharmBase
-from scenario import State
+from scenario import State, Context
 
 class MyCharmType(CharmBase):
     pass
-
-state = State().trigger(charm_type=MyCharmType, meta={'name': 'my-charm-name'}, event='start')
+ctx = Context(charm_type=MyCharmType, 
+              meta={'name': 'my-charm-name'})
+ctx.run('start', State())
 ```
 
-A consequence of this fact is that you have no direct control over the tempdir that we are
-creating to put the metadata you are passing to trigger (because `ops` expects it to be a file...).
-That is, unless you pass your own:
+A consequence of this fact is that you have no direct control over the tempdir that we are creating to put the metadata
+you are passing to trigger (because `ops` expects it to be a file...). That is, unless you pass your own:
 
 ```python
 from ops.charm import CharmBase
-from scenario import State
+from scenario import State, Context
 import tempfile
 
 
 class MyCharmType(CharmBase):
-  pass
+    pass
 
 
 td = tempfile.TemporaryDirectory()
-state = State().trigger(charm_type=MyCharmType, meta={'name': 'my-charm-name'}, event='start',
-                        charm_root=td.name)
+state = Context(
+    charm_type=MyCharmType,
+    meta={'name': 'my-charm-name'},
+    charm_root=td.name
+).run('start', State())
 ```
 
-Do this, and you will be able to set up said directory as you like before the charm is run, as well 
-as verify its contents after the charm has run. Do keep in mind that the metadata files will 
-be overwritten by Scenario, and therefore ignored.
-
+Do this, and you will be able to set up said directory as you like before the charm is run, as well as verify its
+contents after the charm has run. Do keep in mind that the metadata files will be overwritten by Scenario, and therefore
+ignored.
 
 # Consistency checks
 
-A Scenario, that is, the combination of an event, a state, and a charm, is consistent if it's plausible in JujuLand.
-For example, Juju can't emit a `foo-relation-changed` event on your charm unless your charm has declared a `foo` relation
-endpoint in its `metadata.yaml`. If that happens, that's a juju bug.
-Scenario however assumes that Juju is bug-free, therefore, so far as we're concerned, that can't happen, and therefore we 
-help you verify that the scenarios you create are consistent and raise an exception if that isn't so.
+A Scenario, that is, the combination of an event, a state, and a charm, is consistent if it's plausible in JujuLand. For
+example, Juju can't emit a `foo-relation-changed` event on your charm unless your charm has declared a `foo` relation
+endpoint in its `metadata.yaml`. If that happens, that's a juju bug. Scenario however assumes that Juju is bug-free,
+therefore, so far as we're concerned, that can't happen, and therefore we help you verify that the scenarios you create
+are consistent and raise an exception if that isn't so.
 
-That happens automatically behind the scenes whenever you trigger an event; `scenario.consistency_checker.check_consistency`
-is called and verifies that the scenario makes sense.
+That happens automatically behind the scenes whenever you trigger an event;
+`scenario.consistency_checker.check_consistency` is called and verifies that the scenario makes sense.
 
 ## Caveats:
+
 - False positives: not all checks are implemented yet; more will come.
-- False negatives: it is possible that a scenario you know to be consistent is seen as inconsistent. That is probably a bug in the consistency checker itself, please report it.
-- Inherent limitations: if you have a custom event whose name conflicts with a builtin one, the consistency constraints of the builtin one will apply. For example: if you decide to name your custom event `bar-pebble-ready`, but you are working on a machine charm or don't have either way a `bar` container in your `metadata.yaml`, Scenario will flag that as inconsistent. 
+- False negatives: it is possible that a scenario you know to be consistent is seen as inconsistent. That is probably a
+  bug in the consistency checker itself, please report it.
+- Inherent limitations: if you have a custom event whose name conflicts with a builtin one, the consistency constraints
+  of the builtin one will apply. For example: if you decide to name your custom event `bar-pebble-ready`, but you are
+  working on a machine charm or don't have either way a `bar` container in your `metadata.yaml`, Scenario will flag that
+  as inconsistent.
 
 ## Bypassing the checker
-If you have a clear false negative, are explicitly testing 'edge', inconsistent situations, or for whatever reason the checker is in your way, you can set the `SCENARIO_SKIP_CONSISTENCY_CHECKS` envvar and skip it altogether. Hopefully you don't need that.
 
+If you have a clear false negative, are explicitly testing 'edge', inconsistent situations, or for whatever reason the
+checker is in your way, you can set the `SCENARIO_SKIP_CONSISTENCY_CHECKS` envvar and skip it altogether. Hopefully you
+don't need that.
 
 # Snapshot
 
-Scenario comes with a cli tool called `snapshot`. Assuming you've pip-installed `ops-scenario`, you should be able to reach the entry point by typing `scenario snapshot` in a shell.
+Scenario comes with a cli tool called `snapshot`. Assuming you've pip-installed `ops-scenario`, you should be able to
+reach the entry point by typing `scenario snapshot` in a shell so long as the install dir is in your `PATH`.
+
+Snapshot's purpose is to gather the `State` data structure from a real, live charm running in some cloud your local juju
+client has access to. This is handy in case:
 
-Snapshot's purpose is to gather the State data structure from a real, live charm running in some cloud your local juju client has access to. This is handy in case:
 - you want to write a test about the state the charm you're developing is currently in
-- your charm is bork or in some inconsistent state, and you want to write a test to check the charm will handle it correctly the next time around (aka regression testing)
+- your charm is bork or in some inconsistent state, and you want to write a test to check the charm will handle it
+  correctly the next time around (aka regression testing)
 - you are new to Scenario and want to quickly get started with a real-life example.
 
-Suppose you have a Juju model with a `prometheus-k8s` unit deployed as `prometheus-k8s/0`. If you type `scenario snapshot prometheus-k8s/0`, you will get a printout of the State object. Copy-paste that in some file, import all you need from `scenario`, and you have a working `State` that you can `.trigger()` events from.
-
-You can also pass a `--format json | pytest | state (default=state)` flag to obtain
-- jsonified `State` data structure, for portability
-- a full-fledged pytest test case (with imports and all), where you only have to fill in the charm type and the event that you wish to trigger. 
-
-# TODOS:
-- Recorder
+Suppose you have a Juju model with a `prometheus-k8s` unit deployed as `prometheus-k8s/0`. If you type
+`scenario snapshot prometheus-k8s/0`, you will get a printout of the State object. Pipe that out into some file, import
+all you need from `scenario`, and you have a working `State` that you can `Context.run` events with.
+
+You can also pass a `--format` flag to obtain instead:
+- a jsonified `State` data structure, for portability
+- a full-fledged pytest test case (with imports and all), where you only have to fill in the charm type and the event
+  that you wish to trigger.
```

### Comparing `ops-scenario-2.2/README.md` & `ops-scenario-3.0a1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,107 @@
-Scenario
-============
+# Scenario
 
-This is a state transition testing framework for Operator Framework charms.
+[![Build](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml)
+[![QC](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml)
+[![Discourse Status](https://img.shields.io/discourse/status?server=https%3A%2F%2Fdiscourse.charmhub.io&style=flat&label=CharmHub%20Discourse)](https://discourse.charmhub.io)
+[![foo](https://img.shields.io/badge/everything-charming-blueviolet)](https://github.com/PietroPasotti/jhack) 
+[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://discourse.charmhub.io/t/rethinking-charm-testing-with-ops-scenario/8649)
 
-Where the Harness enables you to procedurally mock pieces of the state the charm needs to function, Scenario tests allow
-you to declaratively define the state all at once, and use it as a sort of context against which you can fire a single
-event on the charm and execute its logic.
+Scenario is a state-transition, functional testing framework for Operator Framework charms.
 
-This puts scenario tests somewhere in between unit and integration tests.
+Where the Harness enables you to procedurally mock pieces of the state the charm needs to function, Scenario tests allow you to declaratively define the state all at once, and use it as a sort of context against which you can fire a single event on the charm and execute its logic.
 
-Scenario tests nudge you into thinking of charms as an input->output function. Input is what we call a `Scene`: the
+This puts scenario tests somewhere in between unit and integration tests: some say 'functional', some say 'contract'.
+
+Scenario tests nudge you into thinking of a charm as an input->output function. Input is what we call a `Scene`: the
 union of an `Event` (why am I being executed) and a `State` (am I leader? what is my relation data? what is my
-config?...).
-The output is another context instance: the context after the charm has had a chance to interact with the mocked juju
-model.
+config?...). The output is another context instance: the context after the charm has had a chance to interact with the
+mocked juju model and affect the state back.
 
 ![state transition model depiction](resources/state-transition-model.png)
 
 Scenario-testing a charm, then, means verifying that:
 
 - the charm does not raise uncaught exceptions while handling the scene
 - the output state (or the diff with the input state) is as expected.
 
-
 # Core concepts as a metaphor
+
 I like metaphors, so here we go:
+
 - There is a theatre stage.
 - You pick an actor (a Charm) to put on the stage. Not just any actor: an improv one.
 - You arrange the stage with content that the actor will have to interact with. This consists of selecting:
-    - An initial situation (State) in which the actor is, e.g. is the actor the main role or an NPC (is_leader), or what other actors are there around it, what is written in those pebble-shaped books on the table?
-    - Something that has just happened (an Event) and to which the actor has to react (e.g. one of the NPCs leaves the stage (relation-departed), or the content of one of the books changes).
-- How the actor will react to the event will have an impact on the context: e.g. the actor might knock over a table (a container), or write something down into one of the books.
-
+  - An initial situation (State) in which the actor is, e.g. is the actor the main role or an NPC (is_leader), or what
+    other actors are there around it, what is written in those pebble-shaped books on the table?
+  - Something that has just happened (an Event) and to which the actor has to react (e.g. one of the NPCs leaves the
+    stage (relation-departed), or the content of one of the books changes).
+- How the actor will react to the event will have an impact on the context: e.g. the actor might knock over a table (a
+  container), or write something down into one of the books.
 
 # Core concepts not as a metaphor
-Scenario tests are about running assertions on atomic state transitions treating the charm being tested like a black box.
-An initial state goes in, an event occurs (say, `'start'`) and a new state comes out.
-Scenario tests are about validating the transition, that is, consistency-checking the delta between the two states, and verifying the charm author's expectations.
+
+Scenario tests are about running assertions on atomic state transitions treating the charm being tested like a black
+box. An initial state goes in, an event occurs (say, `'start'`) and a new state comes out. Scenario tests are about
+validating the transition, that is, consistency-checking the delta between the two states, and verifying the charm
+author's expectations.
 
 Comparing scenario tests with `Harness` tests:
-- Harness exposes an imperative API: the user is expected to call methods on the Harness driving it to the desired state, then verify its validity by calling charm methods or inspecting the raw data.
-- Harness instantiates the charm once, then allows you to fire multiple events on the charm, which is breeding ground for subtle bugs. Scenario tests are centered around testing single state transitions, that is, one event at a time. This ensures that the execution environment is as clean as possible (for a unit test).
-- Harness maintains a model of the juju Model, which is a maintenance burden and adds complexity. Scenario mocks at the level of hook tools and stores all mocking data in a monolithic data structure (the State), which makes it more lightweight and portable.
-- TODO: Scenario can mock at the level of hook tools. Decoupling charm and context allows us to swap out easily any part of this flow, and even share context data across charms, codebases, teams...
+
+- Harness exposes an imperative API: the user is expected to call methods on the Harness driving it to the desired
+  state, then verify its validity by calling charm methods or inspecting the raw data.
+- Harness instantiates the charm once, then allows you to fire multiple events on the charm, which is breeding ground
+  for subtle bugs. Scenario tests are centered around testing single state transitions, that is, one event at a time.
+  This ensures that the execution environment is as clean as possible (for a unit test).
+- Harness maintains a model of the juju Model, which is a maintenance burden and adds complexity. Scenario mocks at the
+  level of hook tools and stores all mocking data in a monolithic data structure (the State), which makes it more
+  lightweight and portable.
+- TODO: Scenario can mock at the level of hook tools. Decoupling charm and context allows us to swap out easily any part
+  of this flow, and even share context data across charms, codebases, teams...
 
 # Writing scenario tests
+
 A scenario test consists of three broad steps:
 
-- Arrange:
-    - declare the input state
-    - select an event to fire
-- Act:
-    - run the state (i.e. obtain the output state)
-- Assert:
-    - verify that the output state is how you expect it to be
-    - verify that the delta with the input state is what you expect it to be
+- **Arrange**:
+  - declare the input state
+  - select an event to fire
+- **Act**:
+  - run the state (i.e. obtain the output state)
+  - optionally, use pre-event and post-event hooks to get a hold of the charm instance and run assertions on internal APIs
+- **Assert**:
+  - verify that the output state is how you expect it to be
+  - optionally, verify that the delta with the input state is what you expect it to be
 
 The most basic scenario is the so-called `null scenario`: one in which all is defaulted and barely any data is
 available. The charm has no config, no relations, no networks, and no leadership.
 
 With that, we can write the simplest possible scenario test:
 
 ```python
-from scenario.state import State
+from scenario import State, Context
 from ops.charm import CharmBase
 from ops.model import UnknownStatus
 
 class MyCharm(CharmBase):
     pass
 
 
 def test_scenario_base():
-    out = State().trigger(
-        'start', 
-        MyCharm, meta={"name": "foo"})
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', State())
     assert out.status.unit == UnknownStatus()
 ```
 
-Now let's start making it more complicated.
-Our charm sets a special state if it has leadership on 'start':
+Now let's start making it more complicated. Our charm sets a special state if it has leadership on 'start':
 
 ```python
 import pytest
-from scenario.state import State
+from scenario import State, Context
 from ops.charm import CharmBase
 from ops.model import ActiveStatus
 
 
 class MyCharm(CharmBase):
     def __init__(self, ...):
         self.framework.observe(self.on.start, self._on_start)
@@ -96,29 +111,29 @@
             self.unit.status = ActiveStatus('I rule')
         else:
             self.unit.status = ActiveStatus('I am ruled')
 
 
 @pytest.mark.parametrize('leader', (True, False))
 def test_status_leader(leader):
-    out = State(leader=leader).trigger(
-        'start', 
-        MyCharm,
-        meta={"name": "foo"})
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', 
+                  State(leader=leader)
     assert out.status.unit == ActiveStatus('I rule' if leader else 'I am ruled')
 ```
 
-By defining the right state we can programmatically define what answers will the charm get to all the questions it can ask the juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
-
+By defining the right state we can programmatically define what answers will the charm get to all the questions it can
+ask the juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
 
 ## Statuses
 
-One of the simplest types of black-box testing available to charmers is to execute the charm and verify that the charm sets the expected unit/application status.
-We have seen a simple example above including leadership.
-But what if the charm transitions through a sequence of statuses?
+One of the simplest types of black-box testing available to charmers is to execute the charm and verify that the charm
+sets the expected unit/application status. We have seen a simple example above including leadership. But what if the
+charm transitions through a sequence of statuses?
 
 ```python
 from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, BlockedStatus
 
 # charm code:
 def _on_event(self, _event):
     self.unit.status = MaintenanceStatus('determining who the ruler is...')
@@ -134,195 +149,225 @@
 ```
 
 You can verify that the charm has followed the expected path by checking the **unit status history** like so:
 
 ```python
 from charm import MyCharm
 from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, UnknownStatus
-from scenario import State
+from scenario import State, Context
 
 def test_statuses():
-    out = State(leader=False).trigger(
-        'start',
-        MyCharm,
-        meta={"name": "foo"})
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', 
+                  State(leader=False)) 
     assert out.status.unit_history == [
       UnknownStatus(),
       MaintenanceStatus('determining who the ruler is...'),
       WaitingStatus('checking this is right...'),
       ActiveStatus("I am ruled"),
     ]
 ```
 
 Note that the current status is not in the **unit status history**.
 
-Also note that, unless you initialize the State with a preexisting status, the first status in the history will always be `unknown`. That is because, so far as scenario is concerned, each event is "the first event this charm has ever seen".
+Also note that, unless you initialize the State with a preexisting status, the first status in the history will always
+be `unknown`. That is because, so far as scenario is concerned, each event is "the first event this charm has ever
+seen".
 
-If you want to simulate a situation in which the charm already has seen some event, and is in a status other than Unknown (the default status every charm is born with), you will have to pass the 'initial status' to State.
+If you want to simulate a situation in which the charm already has seen some event, and is in a status other than
+Unknown (the default status every charm is born with), you will have to pass the 'initial status' to State.
 
 ```python
 from ops.model import ActiveStatus
 from scenario import State, Status
 State(leader=False, status=Status(unit=ActiveStatus('foo')))
 ```
 
-
 ## Relations
 
 You can write scenario tests to verify the shape of relation data:
 
 ```python
 from ops.charm import CharmBase
 
-from scenario.state import Relation, State
+from scenario import Relation, State, Context
 
 
 # This charm copies over remote app data to local unit data
 class MyCharm(CharmBase):
     ...
 
     def _on_event(self, e):
         rel = e.relation
         assert rel.app.name == 'remote'
         assert rel.data[self.unit]['abc'] == 'foo'
         rel.data[self.unit]['abc'] = rel.data[e.app]['cde']
 
 
 def test_relation_data():
-    out = State(relations=[
+    state_in = State(relations=[
         Relation(
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "foo"},
             remote_app_data={"cde": "baz!"},
         ),
-    ]
-    ).trigger("start", MyCharm, meta={"name": "foo"})
+    ])
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    
+    state_out = ctx.run('start', state_in) 
 
-    assert out.relations[0].local_unit_data == {"abc": "baz!"}
+    assert state_out.relations[0].local_unit_data == {"abc": "baz!"}
     # you can do this to check that there are no other differences:
-    assert out.relations == [
+    assert state_out.relations == [
         Relation(
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "baz!"},
             remote_app_data={"cde": "baz!"},
         ),
     ]
 
 # which is very idiomatic and superbly explicit. Noice.
 ```
 
-The only mandatory argument to `Relation` (and other relation types, see below) is `endpoint`. The `interface` will be derived from the charm's `metadata.yaml`. When fully defaulted, a relation is 'empty'. There are no remote units, the remote application is called `'remote'` and only has a single unit `remote/0`, and nobody has written any data to the databags yet.
+The only mandatory argument to `Relation` (and other relation types, see below) is `endpoint`. The `interface` will be
+derived from the charm's `metadata.yaml`. When fully defaulted, a relation is 'empty'. There are no remote units, the
+remote application is called `'remote'` and only has a single unit `remote/0`, and nobody has written any data to the
+databags yet.
 
 That is typically the state of a relation when the first unit joins it.
 
-When you use `Relation`, you are specifying a regular (conventional) relation. But that is not the only type of relation. There are also
-peer relations and subordinate relations. While in the background the data model is the same, the data access rules and the consistency constraints on them are very different. For example, it does not make sense for a peer relation to have a different 'remote app' than its 'local app', because it's the same application.    
+When you use `Relation`, you are specifying a regular (conventional) relation. But that is not the only type of
+relation. There are also peer relations and subordinate relations. While in the background the data model is the same,
+the data access rules and the consistency constraints on them are very different. For example, it does not make sense
+for a peer relation to have a different 'remote app' than its 'local app', because it's the same application.
 
 ### PeerRelation
-To declare a peer relation, you should use `scenario.state.PeerRelation`.
-The core difference with regular relations is that peer relations do not have a "remote app" (it's this app, in fact).
-So unlike `Relation`, a `PeerRelation` does not have `remote_app_name` or `remote_app_data` arguments. Also, it talks in terms of `peers`:
-- `Relation.remote_unit_ids` maps to `PeerRelation.peers_ids` 
-- `Relation.remote_units_data` maps to `PeerRelation.peers_data` 
+
+To declare a peer relation, you should use `scenario.state.PeerRelation`. The core difference with regular relations is
+that peer relations do not have a "remote app" (it's this app, in fact). So unlike `Relation`, a `PeerRelation` does not
+have `remote_app_name` or `remote_app_data` arguments. Also, it talks in terms of `peers`:
+
+- `Relation.remote_unit_ids` maps to `PeerRelation.peers_ids`
+- `Relation.remote_units_data` maps to `PeerRelation.peers_data`
 
 ```python
 from scenario.state import PeerRelation
 
 relation = PeerRelation(
     endpoint="peers",
     peers_data={1: {}, 2: {}, 42: {'foo': 'bar'}},
 )
 ```
 
-be mindful when using `PeerRelation` not to include **"this unit"**'s ID in `peers_data` or `peers_ids`, as that would be flagged by the Consistency Checker:
+be mindful when using `PeerRelation` not to include **"this unit"**'s ID in `peers_data` or `peers_ids`, as that would
+be flagged by the Consistency Checker:
+
 ```python
-from scenario import State, PeerRelation
+from scenario import State, PeerRelation, Context
 
-State(relations=[
+state_in = State(relations=[
     PeerRelation(
         endpoint="peers",
         peers_data={1: {}, 2: {}, 42: {'foo': 'bar'}},
-    )]).trigger("start", ..., unit_id=1)  # invalid: this unit's id cannot be the ID of a peer.
+    )],
+    unit_id=1)
+
+Context(...).run("start", state_in)  # invalid: this unit's id cannot be the ID of a peer.
 
 
 ```
 
 ### SubordinateRelation
-To declare a subordinate relation, you should use `scenario.state.SubordinateRelation`.
-The core difference with regular relations is that subordinate relations always have exactly one remote unit (there is always exactly one primary unit that this unit can see). 
-So unlike `Relation`, a `SubordinateRelation` does not have a `remote_units_data` argument. Instead, it has a `remote_unit_data` taking a single `Dict[str:str]`, and takes the primary unit ID as a separate argument.
-Also, it talks in terms of `primary`:
-- `Relation.remote_unit_ids` becomes `SubordinateRelation.primary_id` (a single ID instead of a list of IDs) 
-- `Relation.remote_units_data` becomes `SubordinateRelation.remote_unit_data` (a single databag instead of a mapping from unit IDs to databags) 
+
+To declare a subordinate relation, you should use `scenario.state.SubordinateRelation`. The core difference with regular
+relations is that subordinate relations always have exactly one remote unit (there is always exactly one primary unit
+that this unit can see). So unlike `Relation`, a `SubordinateRelation` does not have a `remote_units_data` argument.
+Instead, it has a `remote_unit_data` taking a single `Dict[str:str]`, and takes the primary unit ID as a separate
+argument. Also, it talks in terms of `primary`:
+
+- `Relation.remote_unit_ids` becomes `SubordinateRelation.primary_id` (a single ID instead of a list of IDs)
+- `Relation.remote_units_data` becomes `SubordinateRelation.remote_unit_data` (a single databag instead of a mapping
+  from unit IDs to databags)
 - `Relation.remote_app_name` maps to `SubordinateRelation.primary_app_name`
 
 ```python
 from scenario.state import SubordinateRelation
 
 relation = SubordinateRelation(
     endpoint="peers",
     remote_unit_data={"foo": "bar"},
     primary_app_name="zookeeper",
     primary_id=42
 )
 relation.primary_name  # "zookeeper/42"
 ```
 
-
 ## Triggering Relation Events
-If you want to trigger relation events, the easiest way to do so is get a hold of the Relation instance and grab the event from one of its aptly-named properties:
+
+If you want to trigger relation events, the easiest way to do so is get a hold of the Relation instance and grab the
+event from one of its aptly-named properties:
 
 ```python
 from scenario import Relation
 relation = Relation(endpoint="foo", interface="bar")
 changed_event = relation.changed_event
 joined_event = relation.joined_event
 # ...
 ```
 
 This is in fact syntactic sugar for:
+
 ```python
 from scenario import Relation, Event
 relation = Relation(endpoint="foo", interface="bar")
 changed_event = Event('foo-relation-changed', relation=relation)
 ```
 
-The reason for this construction is that the event is associated with some relation-specific metadata, that Scenario needs to set up the process that will run `ops.main` with the right environment variables.
+The reason for this construction is that the event is associated with some relation-specific metadata, that Scenario
+needs to set up the process that will run `ops.main` with the right environment variables.
 
 ### Additional event parameters
-All relation events have some additional metadata that does not belong in the Relation object, such as, for a relation-joined event, the name of the (remote) unit that is joining the relation. That is what determines what `ops.model.Unit` you get when you get `RelationJoinedEvent().unit` in an event handler.
 
-In order to supply this parameter, you will have to **call** the event object and pass as `remote_unit_id` the id of the remote unit that the event is about.
-The reason that this parameter is not supplied to `Relation` but to relation events, is that the relation already ties 'this app' to some 'remote app' (cfr. the `Relation.remote_app_name` attr), but not to a specific unit. What remote unit this event is about is not a `State` concern but an `Event` one.  
+All relation events have some additional metadata that does not belong in the Relation object, such as, for a
+relation-joined event, the name of the (remote) unit that is joining the relation. That is what determines what
+`ops.model.Unit` you get when you get `RelationJoinedEvent().unit` in an event handler.
+
+In order to supply this parameter, you will have to **call** the event object and pass as `remote_unit_id` the id of the
+remote unit that the event is about. The reason that this parameter is not supplied to `Relation` but to relation
+events, is that the relation already ties 'this app' to some 'remote app' (cfr. the `Relation.remote_app_name` attr),
+but not to a specific unit. What remote unit this event is about is not a `State` concern but an `Event` one.
 
-The `remote_unit_id` will default to the first ID found in the relation's `remote_unit_ids`, but if the test you are writing is close to that domain, you should probably override it and pass it manually.
+The `remote_unit_id` will default to the first ID found in the relation's `remote_unit_ids`, but if the test you are
+writing is close to that domain, you should probably override it and pass it manually.
 
 ```python
 from scenario import Relation, Event
 relation = Relation(endpoint="foo", interface="bar")
 remote_unit_2_is_joining_event = relation.joined_event(remote_unit_id=2)
 
 # which is syntactic sugar for:
 remote_unit_2_is_joining_event = Event('foo-relation-changed', relation=relation, relation_remote_unit_id=2)
 ```
 
-
 ## Containers
 
-When testing a kubernetes charm, you can mock container interactions.
-When using the null state (`State()`), there will be no containers. So if the charm were to `self.unit.containers`, it would get back an empty dict.
+When testing a kubernetes charm, you can mock container interactions. When using the null state (`State()`), there will
+be no containers. So if the charm were to `self.unit.containers`, it would get back an empty dict.
 
 To give the charm access to some containers, you need to pass them to the input state, like so:
 `State(containers=[...])`
 
 An example of a scene including some containers:
+
 ```python
 from scenario.state import Container, State
 state = State(containers=[
     Container(name="foo", can_connect=True),
     Container(name="bar", can_connect=False)
 ])
 ```
@@ -343,28 +388,30 @@
               can_connect=True,
               mounts={'local': Mount('/local/share/config.yaml', local_file)})
 ]
 )
 ```
 
 In this case, if the charm were to:
+
 ```python
 def _on_start(self, _):
     foo = self.unit.get_container('foo')
     content = foo.pull('/local/share/config.yaml').read()
 ```
 
-then `content` would be the contents of our locally-supplied `file.txt`. You can use `tempdir` for nicely wrapping strings and passing them to the charm via the container.
+then `content` would be the contents of our locally-supplied `file.txt`. You can use `tempdir` for nicely wrapping
+strings and passing them to the charm via the container.
 
 `container.push` works similarly, so you can write a test like:
 
 ```python
 import tempfile
 from ops.charm import CharmBase
-from scenario.state import State, Container, Mount
+from scenario import State, Container, Mount, Context
 
 
 class MyCharm(CharmBase):
     def __init__(self, *args):
         super().__init__(*args)
         self.framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
 
@@ -374,39 +421,45 @@
 
 
 def test_pebble_push():
     with tempfile.NamedTemporaryFile() as local_file:
         container = Container(name='foo',
                               can_connect=True,
                               mounts={'local': Mount('/local/share/config.yaml', local_file.name)})
-        out = State(
+        state_in = State(
             containers=[container]
-        ).trigger(
-            container.pebble_ready_event,
+        )
+        Context(
             MyCharm,
-            meta={"name": "foo", "containers": {"foo": {}}},
+            meta={"name": "foo", "containers": {"foo": {}}}).run(
+            "start",
+            state_in,
         )
         assert local_file.read().decode() == "TEST"
 ```
 
-`container.pebble_ready_event` is syntactic sugar for: `Event("foo-pebble-ready", container=container)`. The reason we need to associate the container with the event is that the Framework uses an envvar to determine which container the pebble-ready event is about (it does not use the event name). Scenario needs that information, similarly, for injecting that envvar into the charm's runtime.
-
-`container.exec` is a tad more complicated, but if you get to this low a level of simulation, you probably will have far worse issues to deal with.
-You need to specify, for each possible command the charm might run on the container, what the result of that would be: its return code, what will be written to stdout/stderr.
+`container.pebble_ready_event` is syntactic sugar for: `Event("foo-pebble-ready", container=container)`. The reason we
+need to associate the container with the event is that the Framework uses an envvar to determine which container the
+pebble-ready event is about (it does not use the event name). Scenario needs that information, similarly, for injecting
+that envvar into the charm's runtime.
+
+`container.exec` is a tad more complicated, but if you get to this low a level of simulation, you probably will have far
+worse issues to deal with. You need to specify, for each possible command the charm might run on the container, what the
+result of that would be: its return code, what will be written to stdout/stderr.
 
 ```python
 from ops.charm import CharmBase
 
-from scenario.state import State, Container, ExecOutput
+from scenario import State, Container, ExecOutput, Context
 
 LS_LL = """
-.rw-rw-r--  228 ubuntu ubuntu 18 jan 12:05 -- charmcraft.yaml    
-.rw-rw-r--  497 ubuntu ubuntu 18 jan 12:05 -- config.yaml        
-.rw-rw-r--  900 ubuntu ubuntu 18 jan 12:05 -- CONTRIBUTING.md    
-drwxrwxr-x    - ubuntu ubuntu 18 jan 12:06 -- lib                
+.rw-rw-r--  228 ubuntu ubuntu 18 jan 12:05 -- charmcraft.yaml
+.rw-rw-r--  497 ubuntu ubuntu 18 jan 12:05 -- config.yaml
+.rw-rw-r--  900 ubuntu ubuntu 18 jan 12:05 -- CONTRIBUTING.md
+drwxrwxr-x    - ubuntu ubuntu 18 jan 12:06 -- lib
 """
 
 
 class MyCharm(CharmBase):
     def _on_start(self, _):
         foo = self.unit.get_container('foo')
         proc = foo.exec(['ls', '-ll'])
@@ -419,145 +472,160 @@
         name='foo',
         exec_mock={
             ('ls', '-ll'):  # this is the command we're mocking
                 ExecOutput(return_code=0,  # this data structure contains all we need to mock the call.
                            stdout=LS_LL)
         }
     )
-    out = State(
+    state_in = State(
         containers=[container]
-    ).trigger(
-        container.pebble_ready_event,
+    )
+    state_out = Context(
         MyCharm,
         meta={"name": "foo", "containers": {"foo": {}}},
+    ).run(
+        container.pebble_ready_event,
+        state_in,
     )
 ```
 
-
 # Deferred events
-Scenario allows you to accurately simulate the Operator Framework's event queue. The event queue is responsible for keeping track of the deferred events.
-On the input side, you can verify that if the charm triggers with this and that event in its queue (they would be there because they had been deferred in the previous run), then the output state is valid.
+
+Scenario allows you to accurately simulate the Operator Framework's event queue. The event queue is responsible for
+keeping track of the deferred events. On the input side, you can verify that if the charm triggers with this and that
+event in its queue (they would be there because they had been deferred in the previous run), then the output state is
+valid.
 
 ```python
-from scenario import State, deferred
+from scenario import State, deferred, Context
 
 
 class MyCharm(...):
     ...
+
     def _on_update_status(self, e):
         e.defer()
+
     def _on_start(self, e):
         e.defer()
 
-        
+
 def test_start_on_deferred_update_status(MyCharm):
     """Test charm execution if a 'start' is dispatched when in the previous run an update-status had been deferred."""
-    out = State(
-      deferred=[
-            deferred('update_status', 
+    state_in = State(
+        deferred=[
+            deferred('update_status',
                      handler=MyCharm._on_update_status)
         ]
-    ).trigger('start', MyCharm)
-    assert len(out.deferred) == 1
-    assert out.deferred[0].name == 'start'
+    )
+    state_out = Context(MyCharm).run('start', state_in)
+    assert len(state_out.deferred) == 1
+    assert state_out.deferred[0].name == 'start'
 ```
 
-You can also generate the 'deferred' data structure (called a DeferredEvent) from the corresponding Event (and the handler):
+You can also generate the 'deferred' data structure (called a DeferredEvent) from the corresponding Event (and the
+handler):
 
 ```python
 from scenario import Event, Relation
 
 class MyCharm(...):
     ...
 
 deferred_start = Event('start').deferred(MyCharm._on_start)
 deferred_install = Event('install').deferred(MyCharm._on_start)
 ```
 
 ## relation events:
-```python   
-foo_relation = Relation('foo') 
+
+```python
+foo_relation = Relation('foo')
 deferred_relation_changed_evt = foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
 ```
-On the output side, you can verify that an event that you expect to have been deferred during this trigger, has indeed been deferred.
+
+On the output side, you can verify that an event that you expect to have been deferred during this trigger, has indeed
+been deferred.
 
 ```python
-from scenario import State
+from scenario import State, Context
 
 
 class MyCharm(...):
     ...
     def _on_start(self, e):
         e.defer()
 
-        
+
 def test_defer(MyCharm):
-    out = State().trigger('start', MyCharm)
+    out = Context(MyCharm).run('start', State())
     assert len(out.deferred) == 1
     assert out.deferred[0].name == 'start'
 ```
-    
+
 ## Deferring relation events
-If you want to test relation event deferrals, some extra care needs to be taken. RelationEvents hold references to the Relation instance they are about. So do they in Scenario. You can use the deferred helper to generate the data structure:
+
+If you want to test relation event deferrals, some extra care needs to be taken. RelationEvents hold references to the
+Relation instance they are about. So do they in Scenario. You can use the deferred helper to generate the data
+structure:
 
 ```python
 from scenario import State, Relation, deferred
 
 
 class MyCharm(...):
     ...
     def _on_foo_relation_changed(self, e):
         e.defer()
 
-        
+
 def test_start_on_deferred_update_status(MyCharm):
-    foo_relation = Relation('foo') 
+    foo_relation = Relation('foo')
     State(
       relations=[foo_relation],
       deferred=[
-            deferred('foo_relation_changed', 
+            deferred('foo_relation_changed',
                      handler=MyCharm._on_foo_relation_changed,
                      relation=foo_relation)
         ]
     )
 ```
+
 but you can also use a shortcut from the relation event itself, as mentioned above:
 
 ```python
 
 from scenario import Relation
 
 class MyCharm(...):
     ...
 
-foo_relation = Relation('foo') 
+foo_relation = Relation('foo')
 foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
 ```
 
 ### Fine-tuning
 
-The deferred helper Scenario provides will not support out of the box all custom event subclasses, or events emitted by charm libraries or objects other than the main charm class.
+The deferred helper Scenario provides will not support out of the box all custom event subclasses, or events emitted by
+charm libraries or objects other than the main charm class.
 
 For general-purpose usage, you will need to instantiate DeferredEvent directly.
 
 ```python
 from scenario import DeferredEvent
 
 my_deferred_event = DeferredEvent(
    handle_path='MyCharm/MyCharmLib/on/database_ready[1]',
    owner='MyCharmLib',  # the object observing the event. Could also be MyCharm.
    observer='_on_database_ready'
 )
 ```
 
-
 # StoredState
 
-Scenario can simulate StoredState.
-You can define it on the input side as:
+Scenario can simulate StoredState. You can define it on the input side as:
 
 ```python
 from ops.charm import CharmBase
 from ops.framework import StoredState as Ops_StoredState, Framework
 from scenario import State, StoredState
 
 
@@ -576,129 +644,166 @@
     content={
       'foo': 'bar',
       'baz': {42: 42},
     })
 ])
 ```
 
-And the charm's runtime will see `self.stored_State.foo` and `.baz` as expected.
-Also, you can run assertions on it on the output side the same as any other bit of state.
-
+And the charm's runtime will see `self.stored_State.foo` and `.baz` as expected. Also, you can run assertions on it on
+the output side the same as any other bit of state.
 
 # Emitted events
-If your charm deals with deferred events, custom events, and charm libs that in turn emit their own custom events, it can be hard to examine the resulting control flow.
-In these situations it can be useful to verify that, as a result of a given juju event triggering (say, 'start'), a specific chain of deferred and custom events is emitted on the charm. The resulting state, black-box as it is, gives little insight into how exactly it was obtained. `scenario.capture_events` allows you to open a peephole and intercept any events emitted by the framework. 
 
-Usage: 
+If your charm deals with deferred events, custom events, and charm libs that in turn emit their own custom events, it
+can be hard to examine the resulting control flow. In these situations it can be useful to verify that, as a result of a
+given juju event triggering (say, 'start'), a specific chain of deferred and custom events is emitted on the charm. The
+resulting state, black-box as it is, gives little insight into how exactly it was obtained. 
+
+`scenario`, among many other great things, is also a pytest plugin. It exposes a fixture called `emitted_events` that you can use like so:
+
+```python
+from scenario import Context
+from ops.charm import StartEvent
+
+def test_foo(emitted_events):
+
+  Context(...).run('start', ...)
+
+  assert len(emitted_events) == 1
+  assert isinstance(emitted_events[0], StartEvent)
+```
+
+
+## Customizing: capture_events
+If you need more control over what events are captured (or you're not into pytest), you can use directly the context manager that powers the `emitted_events` fixture: `scenario.capture_events`.
+This context manager allows you to intercept any events emitted by the framework.
+
+Usage:
 
 ```python
 from ops.charm import StartEvent, UpdateStatusEvent
-from scenario import State, DeferredEvent
-from scenario import capture_events
+from scenario import State, Context, DeferredEvent, capture_events
 with capture_events() as emitted:
-    state_out = State(deferred=[DeferredEvent('start', ...)]).trigger('update-status', ...)
+    ctx = Context(...)
+    state_out = ctx.run(
+      "update-status",
+      State(deferred=[DeferredEvent("start", ...)])
+    )
 
 # deferred events get reemitted first
 assert isinstance(emitted[0], StartEvent)
 # the main juju event gets emitted next
 assert isinstance(emitted[1], UpdateStatusEvent)
 # possibly followed by a tail of all custom events that the main juju event triggered in turn
 # assert isinstance(emitted[2], MyFooEvent)
-# ... 
+# ...
 ```
 
-
 You can filter events by type like so:
 
 ```python
 from ops.charm import StartEvent, RelationEvent
 from scenario import capture_events
 with capture_events(StartEvent, RelationEvent) as emitted:
     # capture all `start` and `*-relation-*` events.
-    pass  
+    pass
 ```
 
 Passing no event types, like: `capture_events()`, is equivalent to `capture_events(EventBase)`.
 
-By default, **framework events** (`PreCommit`, `Commit`) are not considered for inclusion in the output list even if they match the instance check. You can toggle that by passing: `capture_events(include_framework=True)`.
-
-By default, **deferred events** are included in the listing if they match the instance check. You can toggle that by passing:
-`capture_events(include_deferred=True)`.
+By default, **framework events** (`PreCommit`, `Commit`) are not considered for inclusion in the output list even if
+they match the instance check. You can toggle that by passing: `capture_events(include_framework=True)`.
 
+By default, **deferred events** are included in the listing if they match the instance check. You can toggle that by
+passing: `capture_events(include_deferred=True)`.
 
 # The virtual charm root
-Before executing the charm, Scenario writes the metadata, config, and actions `yaml`s to a temporary directory. 
-The charm will see that tempdir as its 'root'. This allows us to keep things simple when dealing with metadata that can 
-be either inferred from the charm type being passed to `trigger()` or be passed to it as an argument, thereby overriding
+
+Before executing the charm, Scenario writes the metadata, config, and actions `yaml`s to a temporary directory. The
+charm will see that tempdir as its 'root'. This allows us to keep things simple when dealing with metadata that can be
+either inferred from the charm type being passed to `Context` or be passed to it as an argument, thereby overriding
 the inferred one. This also allows you to test with charms defined on the fly, as in:
 
 ```python
 from ops.charm import CharmBase
-from scenario import State
+from scenario import State, Context
 
 class MyCharmType(CharmBase):
     pass
-
-state = State().trigger(charm_type=MyCharmType, meta={'name': 'my-charm-name'}, event='start')
+ctx = Context(charm_type=MyCharmType, 
+              meta={'name': 'my-charm-name'})
+ctx.run('start', State())
 ```
 
-A consequence of this fact is that you have no direct control over the tempdir that we are
-creating to put the metadata you are passing to trigger (because `ops` expects it to be a file...).
-That is, unless you pass your own:
+A consequence of this fact is that you have no direct control over the tempdir that we are creating to put the metadata
+you are passing to trigger (because `ops` expects it to be a file...). That is, unless you pass your own:
 
 ```python
 from ops.charm import CharmBase
-from scenario import State
+from scenario import State, Context
 import tempfile
 
 
 class MyCharmType(CharmBase):
-  pass
+    pass
 
 
 td = tempfile.TemporaryDirectory()
-state = State().trigger(charm_type=MyCharmType, meta={'name': 'my-charm-name'}, event='start',
-                        charm_root=td.name)
+state = Context(
+    charm_type=MyCharmType,
+    meta={'name': 'my-charm-name'},
+    charm_root=td.name
+).run('start', State())
 ```
 
-Do this, and you will be able to set up said directory as you like before the charm is run, as well 
-as verify its contents after the charm has run. Do keep in mind that the metadata files will 
-be overwritten by Scenario, and therefore ignored.
-
+Do this, and you will be able to set up said directory as you like before the charm is run, as well as verify its
+contents after the charm has run. Do keep in mind that the metadata files will be overwritten by Scenario, and therefore
+ignored.
 
 # Consistency checks
 
-A Scenario, that is, the combination of an event, a state, and a charm, is consistent if it's plausible in JujuLand.
-For example, Juju can't emit a `foo-relation-changed` event on your charm unless your charm has declared a `foo` relation
-endpoint in its `metadata.yaml`. If that happens, that's a juju bug.
-Scenario however assumes that Juju is bug-free, therefore, so far as we're concerned, that can't happen, and therefore we 
-help you verify that the scenarios you create are consistent and raise an exception if that isn't so.
+A Scenario, that is, the combination of an event, a state, and a charm, is consistent if it's plausible in JujuLand. For
+example, Juju can't emit a `foo-relation-changed` event on your charm unless your charm has declared a `foo` relation
+endpoint in its `metadata.yaml`. If that happens, that's a juju bug. Scenario however assumes that Juju is bug-free,
+therefore, so far as we're concerned, that can't happen, and therefore we help you verify that the scenarios you create
+are consistent and raise an exception if that isn't so.
 
-That happens automatically behind the scenes whenever you trigger an event; `scenario.consistency_checker.check_consistency`
-is called and verifies that the scenario makes sense.
+That happens automatically behind the scenes whenever you trigger an event;
+`scenario.consistency_checker.check_consistency` is called and verifies that the scenario makes sense.
 
 ## Caveats:
+
 - False positives: not all checks are implemented yet; more will come.
-- False negatives: it is possible that a scenario you know to be consistent is seen as inconsistent. That is probably a bug in the consistency checker itself, please report it.
-- Inherent limitations: if you have a custom event whose name conflicts with a builtin one, the consistency constraints of the builtin one will apply. For example: if you decide to name your custom event `bar-pebble-ready`, but you are working on a machine charm or don't have either way a `bar` container in your `metadata.yaml`, Scenario will flag that as inconsistent. 
+- False negatives: it is possible that a scenario you know to be consistent is seen as inconsistent. That is probably a
+  bug in the consistency checker itself, please report it.
+- Inherent limitations: if you have a custom event whose name conflicts with a builtin one, the consistency constraints
+  of the builtin one will apply. For example: if you decide to name your custom event `bar-pebble-ready`, but you are
+  working on a machine charm or don't have either way a `bar` container in your `metadata.yaml`, Scenario will flag that
+  as inconsistent.
 
 ## Bypassing the checker
-If you have a clear false negative, are explicitly testing 'edge', inconsistent situations, or for whatever reason the checker is in your way, you can set the `SCENARIO_SKIP_CONSISTENCY_CHECKS` envvar and skip it altogether. Hopefully you don't need that.
 
+If you have a clear false negative, are explicitly testing 'edge', inconsistent situations, or for whatever reason the
+checker is in your way, you can set the `SCENARIO_SKIP_CONSISTENCY_CHECKS` envvar and skip it altogether. Hopefully you
+don't need that.
 
 # Snapshot
 
-Scenario comes with a cli tool called `snapshot`. Assuming you've pip-installed `ops-scenario`, you should be able to reach the entry point by typing `scenario snapshot` in a shell.
+Scenario comes with a cli tool called `snapshot`. Assuming you've pip-installed `ops-scenario`, you should be able to
+reach the entry point by typing `scenario snapshot` in a shell so long as the install dir is in your `PATH`.
+
+Snapshot's purpose is to gather the `State` data structure from a real, live charm running in some cloud your local juju
+client has access to. This is handy in case:
 
-Snapshot's purpose is to gather the State data structure from a real, live charm running in some cloud your local juju client has access to. This is handy in case:
 - you want to write a test about the state the charm you're developing is currently in
-- your charm is bork or in some inconsistent state, and you want to write a test to check the charm will handle it correctly the next time around (aka regression testing)
+- your charm is bork or in some inconsistent state, and you want to write a test to check the charm will handle it
+  correctly the next time around (aka regression testing)
 - you are new to Scenario and want to quickly get started with a real-life example.
 
-Suppose you have a Juju model with a `prometheus-k8s` unit deployed as `prometheus-k8s/0`. If you type `scenario snapshot prometheus-k8s/0`, you will get a printout of the State object. Copy-paste that in some file, import all you need from `scenario`, and you have a working `State` that you can `.trigger()` events from.
-
-You can also pass a `--format json | pytest | state (default=state)` flag to obtain
-- jsonified `State` data structure, for portability
-- a full-fledged pytest test case (with imports and all), where you only have to fill in the charm type and the event that you wish to trigger. 
-
-# TODOS:
-- Recorder
+Suppose you have a Juju model with a `prometheus-k8s` unit deployed as `prometheus-k8s/0`. If you type
+`scenario snapshot prometheus-k8s/0`, you will get a printout of the State object. Pipe that out into some file, import
+all you need from `scenario`, and you have a working `State` that you can `Context.run` events with.
+
+You can also pass a `--format` flag to obtain instead:
+- a jsonified `State` data structure, for portability
+- a full-fledged pytest test case (with imports and all), where you only have to fill in the charm type and the event
+  that you wish to trigger.
```

### Comparing `ops-scenario-2.2/ops_scenario.egg-info/PKG-INFO` & `ops-scenario-3.0a1/ops_scenario.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,108 +1,127 @@
 Metadata-Version: 2.1
 Name: ops-scenario
-Version: 2.2
+Version: 3.0a1
 Summary: Python library providing a Scenario-based testing API for Operator Framework charms.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
-Project-URL: Homepage, https://github.com/PietroPasotti/ops-scenario
-Project-URL: Bug Tracker, https://github.com/PietroPasotti/ops-scenario/issues
+Project-URL: Homepage, https://github.com/canonical/ops-scenario
+Project-URL: Bug Tracker, https://github.com/canonical/ops-scenario/issues
 Keywords: juju,test
 Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-Scenario
-============
+# Scenario
+
+[![Build](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml)
+[![QC](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml)
+[![Discourse Status](https://img.shields.io/discourse/status?server=https%3A%2F%2Fdiscourse.charmhub.io&style=flat&label=CharmHub%20Discourse)](https://discourse.charmhub.io)
+[![foo](https://img.shields.io/badge/everything-charming-blueviolet)](https://github.com/PietroPasotti/jhack) 
+[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://discourse.charmhub.io/t/rethinking-charm-testing-with-ops-scenario/8649)
 
-This is a state transition testing framework for Operator Framework charms.
+Scenario is a state-transition, functional testing framework for Operator Framework charms.
 
-Where the Harness enables you to procedurally mock pieces of the state the charm needs to function, Scenario tests allow
-you to declaratively define the state all at once, and use it as a sort of context against which you can fire a single
-event on the charm and execute its logic.
+Where the Harness enables you to procedurally mock pieces of the state the charm needs to function, Scenario tests allow you to declaratively define the state all at once, and use it as a sort of context against which you can fire a single event on the charm and execute its logic.
 
-This puts scenario tests somewhere in between unit and integration tests.
+This puts scenario tests somewhere in between unit and integration tests: some say 'functional', some say 'contract'.
 
-Scenario tests nudge you into thinking of charms as an input->output function. Input is what we call a `Scene`: the
+Scenario tests nudge you into thinking of a charm as an input->output function. Input is what we call a `Scene`: the
 union of an `Event` (why am I being executed) and a `State` (am I leader? what is my relation data? what is my
-config?...).
-The output is another context instance: the context after the charm has had a chance to interact with the mocked juju
-model.
+config?...). The output is another context instance: the context after the charm has had a chance to interact with the
+mocked juju model and affect the state back.
 
 ![state transition model depiction](resources/state-transition-model.png)
 
 Scenario-testing a charm, then, means verifying that:
 
 - the charm does not raise uncaught exceptions while handling the scene
 - the output state (or the diff with the input state) is as expected.
 
-
 # Core concepts as a metaphor
+
 I like metaphors, so here we go:
+
 - There is a theatre stage.
 - You pick an actor (a Charm) to put on the stage. Not just any actor: an improv one.
 - You arrange the stage with content that the actor will have to interact with. This consists of selecting:
-    - An initial situation (State) in which the actor is, e.g. is the actor the main role or an NPC (is_leader), or what other actors are there around it, what is written in those pebble-shaped books on the table?
-    - Something that has just happened (an Event) and to which the actor has to react (e.g. one of the NPCs leaves the stage (relation-departed), or the content of one of the books changes).
-- How the actor will react to the event will have an impact on the context: e.g. the actor might knock over a table (a container), or write something down into one of the books.
-
+  - An initial situation (State) in which the actor is, e.g. is the actor the main role or an NPC (is_leader), or what
+    other actors are there around it, what is written in those pebble-shaped books on the table?
+  - Something that has just happened (an Event) and to which the actor has to react (e.g. one of the NPCs leaves the
+    stage (relation-departed), or the content of one of the books changes).
+- How the actor will react to the event will have an impact on the context: e.g. the actor might knock over a table (a
+  container), or write something down into one of the books.
 
 # Core concepts not as a metaphor
-Scenario tests are about running assertions on atomic state transitions treating the charm being tested like a black box.
-An initial state goes in, an event occurs (say, `'start'`) and a new state comes out.
-Scenario tests are about validating the transition, that is, consistency-checking the delta between the two states, and verifying the charm author's expectations.
+
+Scenario tests are about running assertions on atomic state transitions treating the charm being tested like a black
+box. An initial state goes in, an event occurs (say, `'start'`) and a new state comes out. Scenario tests are about
+validating the transition, that is, consistency-checking the delta between the two states, and verifying the charm
+author's expectations.
 
 Comparing scenario tests with `Harness` tests:
-- Harness exposes an imperative API: the user is expected to call methods on the Harness driving it to the desired state, then verify its validity by calling charm methods or inspecting the raw data.
-- Harness instantiates the charm once, then allows you to fire multiple events on the charm, which is breeding ground for subtle bugs. Scenario tests are centered around testing single state transitions, that is, one event at a time. This ensures that the execution environment is as clean as possible (for a unit test).
-- Harness maintains a model of the juju Model, which is a maintenance burden and adds complexity. Scenario mocks at the level of hook tools and stores all mocking data in a monolithic data structure (the State), which makes it more lightweight and portable.
-- TODO: Scenario can mock at the level of hook tools. Decoupling charm and context allows us to swap out easily any part of this flow, and even share context data across charms, codebases, teams...
+
+- Harness exposes an imperative API: the user is expected to call methods on the Harness driving it to the desired
+  state, then verify its validity by calling charm methods or inspecting the raw data.
+- Harness instantiates the charm once, then allows you to fire multiple events on the charm, which is breeding ground
+  for subtle bugs. Scenario tests are centered around testing single state transitions, that is, one event at a time.
+  This ensures that the execution environment is as clean as possible (for a unit test).
+- Harness maintains a model of the juju Model, which is a maintenance burden and adds complexity. Scenario mocks at the
+  level of hook tools and stores all mocking data in a monolithic data structure (the State), which makes it more
+  lightweight and portable.
+- TODO: Scenario can mock at the level of hook tools. Decoupling charm and context allows us to swap out easily any part
+  of this flow, and even share context data across charms, codebases, teams...
 
 # Writing scenario tests
+
 A scenario test consists of three broad steps:
 
-- Arrange:
-    - declare the input state
-    - select an event to fire
-- Act:
-    - run the state (i.e. obtain the output state)
-- Assert:
-    - verify that the output state is how you expect it to be
-    - verify that the delta with the input state is what you expect it to be
+- **Arrange**:
+  - declare the input state
+  - select an event to fire
+- **Act**:
+  - run the state (i.e. obtain the output state)
+  - optionally, use pre-event and post-event hooks to get a hold of the charm instance and run assertions on internal APIs
+- **Assert**:
+  - verify that the output state is how you expect it to be
+  - optionally, verify that the delta with the input state is what you expect it to be
 
 The most basic scenario is the so-called `null scenario`: one in which all is defaulted and barely any data is
 available. The charm has no config, no relations, no networks, and no leadership.
 
 With that, we can write the simplest possible scenario test:
 
 ```python
-from scenario.state import State
+from scenario import State, Context
 from ops.charm import CharmBase
 from ops.model import UnknownStatus
 
 class MyCharm(CharmBase):
     pass
 
 
 def test_scenario_base():
-    out = State().trigger(
-        'start', 
-        MyCharm, meta={"name": "foo"})
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', State())
     assert out.status.unit == UnknownStatus()
 ```
 
-Now let's start making it more complicated.
-Our charm sets a special state if it has leadership on 'start':
+Now let's start making it more complicated. Our charm sets a special state if it has leadership on 'start':
 
 ```python
 import pytest
-from scenario.state import State
+from scenario import State, Context
 from ops.charm import CharmBase
 from ops.model import ActiveStatus
 
 
 class MyCharm(CharmBase):
     def __init__(self, ...):
         self.framework.observe(self.on.start, self._on_start)
@@ -112,29 +131,29 @@
             self.unit.status = ActiveStatus('I rule')
         else:
             self.unit.status = ActiveStatus('I am ruled')
 
 
 @pytest.mark.parametrize('leader', (True, False))
 def test_status_leader(leader):
-    out = State(leader=leader).trigger(
-        'start', 
-        MyCharm,
-        meta={"name": "foo"})
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', 
+                  State(leader=leader)
     assert out.status.unit == ActiveStatus('I rule' if leader else 'I am ruled')
 ```
 
-By defining the right state we can programmatically define what answers will the charm get to all the questions it can ask the juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
-
+By defining the right state we can programmatically define what answers will the charm get to all the questions it can
+ask the juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
 
 ## Statuses
 
-One of the simplest types of black-box testing available to charmers is to execute the charm and verify that the charm sets the expected unit/application status.
-We have seen a simple example above including leadership.
-But what if the charm transitions through a sequence of statuses?
+One of the simplest types of black-box testing available to charmers is to execute the charm and verify that the charm
+sets the expected unit/application status. We have seen a simple example above including leadership. But what if the
+charm transitions through a sequence of statuses?
 
 ```python
 from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, BlockedStatus
 
 # charm code:
 def _on_event(self, _event):
     self.unit.status = MaintenanceStatus('determining who the ruler is...')
@@ -150,195 +169,225 @@
 ```
 
 You can verify that the charm has followed the expected path by checking the **unit status history** like so:
 
 ```python
 from charm import MyCharm
 from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, UnknownStatus
-from scenario import State
+from scenario import State, Context
 
 def test_statuses():
-    out = State(leader=False).trigger(
-        'start',
-        MyCharm,
-        meta={"name": "foo"})
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', 
+                  State(leader=False)) 
     assert out.status.unit_history == [
       UnknownStatus(),
       MaintenanceStatus('determining who the ruler is...'),
       WaitingStatus('checking this is right...'),
       ActiveStatus("I am ruled"),
     ]
 ```
 
 Note that the current status is not in the **unit status history**.
 
-Also note that, unless you initialize the State with a preexisting status, the first status in the history will always be `unknown`. That is because, so far as scenario is concerned, each event is "the first event this charm has ever seen".
+Also note that, unless you initialize the State with a preexisting status, the first status in the history will always
+be `unknown`. That is because, so far as scenario is concerned, each event is "the first event this charm has ever
+seen".
 
-If you want to simulate a situation in which the charm already has seen some event, and is in a status other than Unknown (the default status every charm is born with), you will have to pass the 'initial status' to State.
+If you want to simulate a situation in which the charm already has seen some event, and is in a status other than
+Unknown (the default status every charm is born with), you will have to pass the 'initial status' to State.
 
 ```python
 from ops.model import ActiveStatus
 from scenario import State, Status
 State(leader=False, status=Status(unit=ActiveStatus('foo')))
 ```
 
-
 ## Relations
 
 You can write scenario tests to verify the shape of relation data:
 
 ```python
 from ops.charm import CharmBase
 
-from scenario.state import Relation, State
+from scenario import Relation, State, Context
 
 
 # This charm copies over remote app data to local unit data
 class MyCharm(CharmBase):
     ...
 
     def _on_event(self, e):
         rel = e.relation
         assert rel.app.name == 'remote'
         assert rel.data[self.unit]['abc'] == 'foo'
         rel.data[self.unit]['abc'] = rel.data[e.app]['cde']
 
 
 def test_relation_data():
-    out = State(relations=[
+    state_in = State(relations=[
         Relation(
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "foo"},
             remote_app_data={"cde": "baz!"},
         ),
-    ]
-    ).trigger("start", MyCharm, meta={"name": "foo"})
+    ])
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    
+    state_out = ctx.run('start', state_in) 
 
-    assert out.relations[0].local_unit_data == {"abc": "baz!"}
+    assert state_out.relations[0].local_unit_data == {"abc": "baz!"}
     # you can do this to check that there are no other differences:
-    assert out.relations == [
+    assert state_out.relations == [
         Relation(
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "baz!"},
             remote_app_data={"cde": "baz!"},
         ),
     ]
 
 # which is very idiomatic and superbly explicit. Noice.
 ```
 
-The only mandatory argument to `Relation` (and other relation types, see below) is `endpoint`. The `interface` will be derived from the charm's `metadata.yaml`. When fully defaulted, a relation is 'empty'. There are no remote units, the remote application is called `'remote'` and only has a single unit `remote/0`, and nobody has written any data to the databags yet.
+The only mandatory argument to `Relation` (and other relation types, see below) is `endpoint`. The `interface` will be
+derived from the charm's `metadata.yaml`. When fully defaulted, a relation is 'empty'. There are no remote units, the
+remote application is called `'remote'` and only has a single unit `remote/0`, and nobody has written any data to the
+databags yet.
 
 That is typically the state of a relation when the first unit joins it.
 
-When you use `Relation`, you are specifying a regular (conventional) relation. But that is not the only type of relation. There are also
-peer relations and subordinate relations. While in the background the data model is the same, the data access rules and the consistency constraints on them are very different. For example, it does not make sense for a peer relation to have a different 'remote app' than its 'local app', because it's the same application.    
+When you use `Relation`, you are specifying a regular (conventional) relation. But that is not the only type of
+relation. There are also peer relations and subordinate relations. While in the background the data model is the same,
+the data access rules and the consistency constraints on them are very different. For example, it does not make sense
+for a peer relation to have a different 'remote app' than its 'local app', because it's the same application.
 
 ### PeerRelation
-To declare a peer relation, you should use `scenario.state.PeerRelation`.
-The core difference with regular relations is that peer relations do not have a "remote app" (it's this app, in fact).
-So unlike `Relation`, a `PeerRelation` does not have `remote_app_name` or `remote_app_data` arguments. Also, it talks in terms of `peers`:
-- `Relation.remote_unit_ids` maps to `PeerRelation.peers_ids` 
-- `Relation.remote_units_data` maps to `PeerRelation.peers_data` 
+
+To declare a peer relation, you should use `scenario.state.PeerRelation`. The core difference with regular relations is
+that peer relations do not have a "remote app" (it's this app, in fact). So unlike `Relation`, a `PeerRelation` does not
+have `remote_app_name` or `remote_app_data` arguments. Also, it talks in terms of `peers`:
+
+- `Relation.remote_unit_ids` maps to `PeerRelation.peers_ids`
+- `Relation.remote_units_data` maps to `PeerRelation.peers_data`
 
 ```python
 from scenario.state import PeerRelation
 
 relation = PeerRelation(
     endpoint="peers",
     peers_data={1: {}, 2: {}, 42: {'foo': 'bar'}},
 )
 ```
 
-be mindful when using `PeerRelation` not to include **"this unit"**'s ID in `peers_data` or `peers_ids`, as that would be flagged by the Consistency Checker:
+be mindful when using `PeerRelation` not to include **"this unit"**'s ID in `peers_data` or `peers_ids`, as that would
+be flagged by the Consistency Checker:
+
 ```python
-from scenario import State, PeerRelation
+from scenario import State, PeerRelation, Context
 
-State(relations=[
+state_in = State(relations=[
     PeerRelation(
         endpoint="peers",
         peers_data={1: {}, 2: {}, 42: {'foo': 'bar'}},
-    )]).trigger("start", ..., unit_id=1)  # invalid: this unit's id cannot be the ID of a peer.
+    )],
+    unit_id=1)
+
+Context(...).run("start", state_in)  # invalid: this unit's id cannot be the ID of a peer.
 
 
 ```
 
 ### SubordinateRelation
-To declare a subordinate relation, you should use `scenario.state.SubordinateRelation`.
-The core difference with regular relations is that subordinate relations always have exactly one remote unit (there is always exactly one primary unit that this unit can see). 
-So unlike `Relation`, a `SubordinateRelation` does not have a `remote_units_data` argument. Instead, it has a `remote_unit_data` taking a single `Dict[str:str]`, and takes the primary unit ID as a separate argument.
-Also, it talks in terms of `primary`:
-- `Relation.remote_unit_ids` becomes `SubordinateRelation.primary_id` (a single ID instead of a list of IDs) 
-- `Relation.remote_units_data` becomes `SubordinateRelation.remote_unit_data` (a single databag instead of a mapping from unit IDs to databags) 
+
+To declare a subordinate relation, you should use `scenario.state.SubordinateRelation`. The core difference with regular
+relations is that subordinate relations always have exactly one remote unit (there is always exactly one primary unit
+that this unit can see). So unlike `Relation`, a `SubordinateRelation` does not have a `remote_units_data` argument.
+Instead, it has a `remote_unit_data` taking a single `Dict[str:str]`, and takes the primary unit ID as a separate
+argument. Also, it talks in terms of `primary`:
+
+- `Relation.remote_unit_ids` becomes `SubordinateRelation.primary_id` (a single ID instead of a list of IDs)
+- `Relation.remote_units_data` becomes `SubordinateRelation.remote_unit_data` (a single databag instead of a mapping
+  from unit IDs to databags)
 - `Relation.remote_app_name` maps to `SubordinateRelation.primary_app_name`
 
 ```python
 from scenario.state import SubordinateRelation
 
 relation = SubordinateRelation(
     endpoint="peers",
     remote_unit_data={"foo": "bar"},
     primary_app_name="zookeeper",
     primary_id=42
 )
 relation.primary_name  # "zookeeper/42"
 ```
 
-
 ## Triggering Relation Events
-If you want to trigger relation events, the easiest way to do so is get a hold of the Relation instance and grab the event from one of its aptly-named properties:
+
+If you want to trigger relation events, the easiest way to do so is get a hold of the Relation instance and grab the
+event from one of its aptly-named properties:
 
 ```python
 from scenario import Relation
 relation = Relation(endpoint="foo", interface="bar")
 changed_event = relation.changed_event
 joined_event = relation.joined_event
 # ...
 ```
 
 This is in fact syntactic sugar for:
+
 ```python
 from scenario import Relation, Event
 relation = Relation(endpoint="foo", interface="bar")
 changed_event = Event('foo-relation-changed', relation=relation)
 ```
 
-The reason for this construction is that the event is associated with some relation-specific metadata, that Scenario needs to set up the process that will run `ops.main` with the right environment variables.
+The reason for this construction is that the event is associated with some relation-specific metadata, that Scenario
+needs to set up the process that will run `ops.main` with the right environment variables.
 
 ### Additional event parameters
-All relation events have some additional metadata that does not belong in the Relation object, such as, for a relation-joined event, the name of the (remote) unit that is joining the relation. That is what determines what `ops.model.Unit` you get when you get `RelationJoinedEvent().unit` in an event handler.
 
-In order to supply this parameter, you will have to **call** the event object and pass as `remote_unit_id` the id of the remote unit that the event is about.
-The reason that this parameter is not supplied to `Relation` but to relation events, is that the relation already ties 'this app' to some 'remote app' (cfr. the `Relation.remote_app_name` attr), but not to a specific unit. What remote unit this event is about is not a `State` concern but an `Event` one.  
+All relation events have some additional metadata that does not belong in the Relation object, such as, for a
+relation-joined event, the name of the (remote) unit that is joining the relation. That is what determines what
+`ops.model.Unit` you get when you get `RelationJoinedEvent().unit` in an event handler.
+
+In order to supply this parameter, you will have to **call** the event object and pass as `remote_unit_id` the id of the
+remote unit that the event is about. The reason that this parameter is not supplied to `Relation` but to relation
+events, is that the relation already ties 'this app' to some 'remote app' (cfr. the `Relation.remote_app_name` attr),
+but not to a specific unit. What remote unit this event is about is not a `State` concern but an `Event` one.
 
-The `remote_unit_id` will default to the first ID found in the relation's `remote_unit_ids`, but if the test you are writing is close to that domain, you should probably override it and pass it manually.
+The `remote_unit_id` will default to the first ID found in the relation's `remote_unit_ids`, but if the test you are
+writing is close to that domain, you should probably override it and pass it manually.
 
 ```python
 from scenario import Relation, Event
 relation = Relation(endpoint="foo", interface="bar")
 remote_unit_2_is_joining_event = relation.joined_event(remote_unit_id=2)
 
 # which is syntactic sugar for:
 remote_unit_2_is_joining_event = Event('foo-relation-changed', relation=relation, relation_remote_unit_id=2)
 ```
 
-
 ## Containers
 
-When testing a kubernetes charm, you can mock container interactions.
-When using the null state (`State()`), there will be no containers. So if the charm were to `self.unit.containers`, it would get back an empty dict.
+When testing a kubernetes charm, you can mock container interactions. When using the null state (`State()`), there will
+be no containers. So if the charm were to `self.unit.containers`, it would get back an empty dict.
 
 To give the charm access to some containers, you need to pass them to the input state, like so:
 `State(containers=[...])`
 
 An example of a scene including some containers:
+
 ```python
 from scenario.state import Container, State
 state = State(containers=[
     Container(name="foo", can_connect=True),
     Container(name="bar", can_connect=False)
 ])
 ```
@@ -359,28 +408,30 @@
               can_connect=True,
               mounts={'local': Mount('/local/share/config.yaml', local_file)})
 ]
 )
 ```
 
 In this case, if the charm were to:
+
 ```python
 def _on_start(self, _):
     foo = self.unit.get_container('foo')
     content = foo.pull('/local/share/config.yaml').read()
 ```
 
-then `content` would be the contents of our locally-supplied `file.txt`. You can use `tempdir` for nicely wrapping strings and passing them to the charm via the container.
+then `content` would be the contents of our locally-supplied `file.txt`. You can use `tempdir` for nicely wrapping
+strings and passing them to the charm via the container.
 
 `container.push` works similarly, so you can write a test like:
 
 ```python
 import tempfile
 from ops.charm import CharmBase
-from scenario.state import State, Container, Mount
+from scenario import State, Container, Mount, Context
 
 
 class MyCharm(CharmBase):
     def __init__(self, *args):
         super().__init__(*args)
         self.framework.observe(self.on.foo_pebble_ready, self._on_pebble_ready)
 
@@ -390,39 +441,45 @@
 
 
 def test_pebble_push():
     with tempfile.NamedTemporaryFile() as local_file:
         container = Container(name='foo',
                               can_connect=True,
                               mounts={'local': Mount('/local/share/config.yaml', local_file.name)})
-        out = State(
+        state_in = State(
             containers=[container]
-        ).trigger(
-            container.pebble_ready_event,
+        )
+        Context(
             MyCharm,
-            meta={"name": "foo", "containers": {"foo": {}}},
+            meta={"name": "foo", "containers": {"foo": {}}}).run(
+            "start",
+            state_in,
         )
         assert local_file.read().decode() == "TEST"
 ```
 
-`container.pebble_ready_event` is syntactic sugar for: `Event("foo-pebble-ready", container=container)`. The reason we need to associate the container with the event is that the Framework uses an envvar to determine which container the pebble-ready event is about (it does not use the event name). Scenario needs that information, similarly, for injecting that envvar into the charm's runtime.
-
-`container.exec` is a tad more complicated, but if you get to this low a level of simulation, you probably will have far worse issues to deal with.
-You need to specify, for each possible command the charm might run on the container, what the result of that would be: its return code, what will be written to stdout/stderr.
+`container.pebble_ready_event` is syntactic sugar for: `Event("foo-pebble-ready", container=container)`. The reason we
+need to associate the container with the event is that the Framework uses an envvar to determine which container the
+pebble-ready event is about (it does not use the event name). Scenario needs that information, similarly, for injecting
+that envvar into the charm's runtime.
+
+`container.exec` is a tad more complicated, but if you get to this low a level of simulation, you probably will have far
+worse issues to deal with. You need to specify, for each possible command the charm might run on the container, what the
+result of that would be: its return code, what will be written to stdout/stderr.
 
 ```python
 from ops.charm import CharmBase
 
-from scenario.state import State, Container, ExecOutput
+from scenario import State, Container, ExecOutput, Context
 
 LS_LL = """
-.rw-rw-r--  228 ubuntu ubuntu 18 jan 12:05 -- charmcraft.yaml    
-.rw-rw-r--  497 ubuntu ubuntu 18 jan 12:05 -- config.yaml        
-.rw-rw-r--  900 ubuntu ubuntu 18 jan 12:05 -- CONTRIBUTING.md    
-drwxrwxr-x    - ubuntu ubuntu 18 jan 12:06 -- lib                
+.rw-rw-r--  228 ubuntu ubuntu 18 jan 12:05 -- charmcraft.yaml
+.rw-rw-r--  497 ubuntu ubuntu 18 jan 12:05 -- config.yaml
+.rw-rw-r--  900 ubuntu ubuntu 18 jan 12:05 -- CONTRIBUTING.md
+drwxrwxr-x    - ubuntu ubuntu 18 jan 12:06 -- lib
 """
 
 
 class MyCharm(CharmBase):
     def _on_start(self, _):
         foo = self.unit.get_container('foo')
         proc = foo.exec(['ls', '-ll'])
@@ -435,145 +492,160 @@
         name='foo',
         exec_mock={
             ('ls', '-ll'):  # this is the command we're mocking
                 ExecOutput(return_code=0,  # this data structure contains all we need to mock the call.
                            stdout=LS_LL)
         }
     )
-    out = State(
+    state_in = State(
         containers=[container]
-    ).trigger(
-        container.pebble_ready_event,
+    )
+    state_out = Context(
         MyCharm,
         meta={"name": "foo", "containers": {"foo": {}}},
+    ).run(
+        container.pebble_ready_event,
+        state_in,
     )
 ```
 
-
 # Deferred events
-Scenario allows you to accurately simulate the Operator Framework's event queue. The event queue is responsible for keeping track of the deferred events.
-On the input side, you can verify that if the charm triggers with this and that event in its queue (they would be there because they had been deferred in the previous run), then the output state is valid.
+
+Scenario allows you to accurately simulate the Operator Framework's event queue. The event queue is responsible for
+keeping track of the deferred events. On the input side, you can verify that if the charm triggers with this and that
+event in its queue (they would be there because they had been deferred in the previous run), then the output state is
+valid.
 
 ```python
-from scenario import State, deferred
+from scenario import State, deferred, Context
 
 
 class MyCharm(...):
     ...
+
     def _on_update_status(self, e):
         e.defer()
+
     def _on_start(self, e):
         e.defer()
 
-        
+
 def test_start_on_deferred_update_status(MyCharm):
     """Test charm execution if a 'start' is dispatched when in the previous run an update-status had been deferred."""
-    out = State(
-      deferred=[
-            deferred('update_status', 
+    state_in = State(
+        deferred=[
+            deferred('update_status',
                      handler=MyCharm._on_update_status)
         ]
-    ).trigger('start', MyCharm)
-    assert len(out.deferred) == 1
-    assert out.deferred[0].name == 'start'
+    )
+    state_out = Context(MyCharm).run('start', state_in)
+    assert len(state_out.deferred) == 1
+    assert state_out.deferred[0].name == 'start'
 ```
 
-You can also generate the 'deferred' data structure (called a DeferredEvent) from the corresponding Event (and the handler):
+You can also generate the 'deferred' data structure (called a DeferredEvent) from the corresponding Event (and the
+handler):
 
 ```python
 from scenario import Event, Relation
 
 class MyCharm(...):
     ...
 
 deferred_start = Event('start').deferred(MyCharm._on_start)
 deferred_install = Event('install').deferred(MyCharm._on_start)
 ```
 
 ## relation events:
-```python   
-foo_relation = Relation('foo') 
+
+```python
+foo_relation = Relation('foo')
 deferred_relation_changed_evt = foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
 ```
-On the output side, you can verify that an event that you expect to have been deferred during this trigger, has indeed been deferred.
+
+On the output side, you can verify that an event that you expect to have been deferred during this trigger, has indeed
+been deferred.
 
 ```python
-from scenario import State
+from scenario import State, Context
 
 
 class MyCharm(...):
     ...
     def _on_start(self, e):
         e.defer()
 
-        
+
 def test_defer(MyCharm):
-    out = State().trigger('start', MyCharm)
+    out = Context(MyCharm).run('start', State())
     assert len(out.deferred) == 1
     assert out.deferred[0].name == 'start'
 ```
-    
+
 ## Deferring relation events
-If you want to test relation event deferrals, some extra care needs to be taken. RelationEvents hold references to the Relation instance they are about. So do they in Scenario. You can use the deferred helper to generate the data structure:
+
+If you want to test relation event deferrals, some extra care needs to be taken. RelationEvents hold references to the
+Relation instance they are about. So do they in Scenario. You can use the deferred helper to generate the data
+structure:
 
 ```python
 from scenario import State, Relation, deferred
 
 
 class MyCharm(...):
     ...
     def _on_foo_relation_changed(self, e):
         e.defer()
 
-        
+
 def test_start_on_deferred_update_status(MyCharm):
-    foo_relation = Relation('foo') 
+    foo_relation = Relation('foo')
     State(
       relations=[foo_relation],
       deferred=[
-            deferred('foo_relation_changed', 
+            deferred('foo_relation_changed',
                      handler=MyCharm._on_foo_relation_changed,
                      relation=foo_relation)
         ]
     )
 ```
+
 but you can also use a shortcut from the relation event itself, as mentioned above:
 
 ```python
 
 from scenario import Relation
 
 class MyCharm(...):
     ...
 
-foo_relation = Relation('foo') 
+foo_relation = Relation('foo')
 foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
 ```
 
 ### Fine-tuning
 
-The deferred helper Scenario provides will not support out of the box all custom event subclasses, or events emitted by charm libraries or objects other than the main charm class.
+The deferred helper Scenario provides will not support out of the box all custom event subclasses, or events emitted by
+charm libraries or objects other than the main charm class.
 
 For general-purpose usage, you will need to instantiate DeferredEvent directly.
 
 ```python
 from scenario import DeferredEvent
 
 my_deferred_event = DeferredEvent(
    handle_path='MyCharm/MyCharmLib/on/database_ready[1]',
    owner='MyCharmLib',  # the object observing the event. Could also be MyCharm.
    observer='_on_database_ready'
 )
 ```
 
-
 # StoredState
 
-Scenario can simulate StoredState.
-You can define it on the input side as:
+Scenario can simulate StoredState. You can define it on the input side as:
 
 ```python
 from ops.charm import CharmBase
 from ops.framework import StoredState as Ops_StoredState, Framework
 from scenario import State, StoredState
 
 
@@ -592,129 +664,166 @@
     content={
       'foo': 'bar',
       'baz': {42: 42},
     })
 ])
 ```
 
-And the charm's runtime will see `self.stored_State.foo` and `.baz` as expected.
-Also, you can run assertions on it on the output side the same as any other bit of state.
-
+And the charm's runtime will see `self.stored_State.foo` and `.baz` as expected. Also, you can run assertions on it on
+the output side the same as any other bit of state.
 
 # Emitted events
-If your charm deals with deferred events, custom events, and charm libs that in turn emit their own custom events, it can be hard to examine the resulting control flow.
-In these situations it can be useful to verify that, as a result of a given juju event triggering (say, 'start'), a specific chain of deferred and custom events is emitted on the charm. The resulting state, black-box as it is, gives little insight into how exactly it was obtained. `scenario.capture_events` allows you to open a peephole and intercept any events emitted by the framework. 
 
-Usage: 
+If your charm deals with deferred events, custom events, and charm libs that in turn emit their own custom events, it
+can be hard to examine the resulting control flow. In these situations it can be useful to verify that, as a result of a
+given juju event triggering (say, 'start'), a specific chain of deferred and custom events is emitted on the charm. The
+resulting state, black-box as it is, gives little insight into how exactly it was obtained. 
+
+`scenario`, among many other great things, is also a pytest plugin. It exposes a fixture called `emitted_events` that you can use like so:
+
+```python
+from scenario import Context
+from ops.charm import StartEvent
+
+def test_foo(emitted_events):
+
+  Context(...).run('start', ...)
+
+  assert len(emitted_events) == 1
+  assert isinstance(emitted_events[0], StartEvent)
+```
+
+
+## Customizing: capture_events
+If you need more control over what events are captured (or you're not into pytest), you can use directly the context manager that powers the `emitted_events` fixture: `scenario.capture_events`.
+This context manager allows you to intercept any events emitted by the framework.
+
+Usage:
 
 ```python
 from ops.charm import StartEvent, UpdateStatusEvent
-from scenario import State, DeferredEvent
-from scenario import capture_events
+from scenario import State, Context, DeferredEvent, capture_events
 with capture_events() as emitted:
-    state_out = State(deferred=[DeferredEvent('start', ...)]).trigger('update-status', ...)
+    ctx = Context(...)
+    state_out = ctx.run(
+      "update-status",
+      State(deferred=[DeferredEvent("start", ...)])
+    )
 
 # deferred events get reemitted first
 assert isinstance(emitted[0], StartEvent)
 # the main juju event gets emitted next
 assert isinstance(emitted[1], UpdateStatusEvent)
 # possibly followed by a tail of all custom events that the main juju event triggered in turn
 # assert isinstance(emitted[2], MyFooEvent)
-# ... 
+# ...
 ```
 
-
 You can filter events by type like so:
 
 ```python
 from ops.charm import StartEvent, RelationEvent
 from scenario import capture_events
 with capture_events(StartEvent, RelationEvent) as emitted:
     # capture all `start` and `*-relation-*` events.
-    pass  
+    pass
 ```
 
 Passing no event types, like: `capture_events()`, is equivalent to `capture_events(EventBase)`.
 
-By default, **framework events** (`PreCommit`, `Commit`) are not considered for inclusion in the output list even if they match the instance check. You can toggle that by passing: `capture_events(include_framework=True)`.
-
-By default, **deferred events** are included in the listing if they match the instance check. You can toggle that by passing:
-`capture_events(include_deferred=True)`.
+By default, **framework events** (`PreCommit`, `Commit`) are not considered for inclusion in the output list even if
+they match the instance check. You can toggle that by passing: `capture_events(include_framework=True)`.
 
+By default, **deferred events** are included in the listing if they match the instance check. You can toggle that by
+passing: `capture_events(include_deferred=True)`.
 
 # The virtual charm root
-Before executing the charm, Scenario writes the metadata, config, and actions `yaml`s to a temporary directory. 
-The charm will see that tempdir as its 'root'. This allows us to keep things simple when dealing with metadata that can 
-be either inferred from the charm type being passed to `trigger()` or be passed to it as an argument, thereby overriding
+
+Before executing the charm, Scenario writes the metadata, config, and actions `yaml`s to a temporary directory. The
+charm will see that tempdir as its 'root'. This allows us to keep things simple when dealing with metadata that can be
+either inferred from the charm type being passed to `Context` or be passed to it as an argument, thereby overriding
 the inferred one. This also allows you to test with charms defined on the fly, as in:
 
 ```python
 from ops.charm import CharmBase
-from scenario import State
+from scenario import State, Context
 
 class MyCharmType(CharmBase):
     pass
-
-state = State().trigger(charm_type=MyCharmType, meta={'name': 'my-charm-name'}, event='start')
+ctx = Context(charm_type=MyCharmType, 
+              meta={'name': 'my-charm-name'})
+ctx.run('start', State())
 ```
 
-A consequence of this fact is that you have no direct control over the tempdir that we are
-creating to put the metadata you are passing to trigger (because `ops` expects it to be a file...).
-That is, unless you pass your own:
+A consequence of this fact is that you have no direct control over the tempdir that we are creating to put the metadata
+you are passing to trigger (because `ops` expects it to be a file...). That is, unless you pass your own:
 
 ```python
 from ops.charm import CharmBase
-from scenario import State
+from scenario import State, Context
 import tempfile
 
 
 class MyCharmType(CharmBase):
-  pass
+    pass
 
 
 td = tempfile.TemporaryDirectory()
-state = State().trigger(charm_type=MyCharmType, meta={'name': 'my-charm-name'}, event='start',
-                        charm_root=td.name)
+state = Context(
+    charm_type=MyCharmType,
+    meta={'name': 'my-charm-name'},
+    charm_root=td.name
+).run('start', State())
 ```
 
-Do this, and you will be able to set up said directory as you like before the charm is run, as well 
-as verify its contents after the charm has run. Do keep in mind that the metadata files will 
-be overwritten by Scenario, and therefore ignored.
-
+Do this, and you will be able to set up said directory as you like before the charm is run, as well as verify its
+contents after the charm has run. Do keep in mind that the metadata files will be overwritten by Scenario, and therefore
+ignored.
 
 # Consistency checks
 
-A Scenario, that is, the combination of an event, a state, and a charm, is consistent if it's plausible in JujuLand.
-For example, Juju can't emit a `foo-relation-changed` event on your charm unless your charm has declared a `foo` relation
-endpoint in its `metadata.yaml`. If that happens, that's a juju bug.
-Scenario however assumes that Juju is bug-free, therefore, so far as we're concerned, that can't happen, and therefore we 
-help you verify that the scenarios you create are consistent and raise an exception if that isn't so.
+A Scenario, that is, the combination of an event, a state, and a charm, is consistent if it's plausible in JujuLand. For
+example, Juju can't emit a `foo-relation-changed` event on your charm unless your charm has declared a `foo` relation
+endpoint in its `metadata.yaml`. If that happens, that's a juju bug. Scenario however assumes that Juju is bug-free,
+therefore, so far as we're concerned, that can't happen, and therefore we help you verify that the scenarios you create
+are consistent and raise an exception if that isn't so.
 
-That happens automatically behind the scenes whenever you trigger an event; `scenario.consistency_checker.check_consistency`
-is called and verifies that the scenario makes sense.
+That happens automatically behind the scenes whenever you trigger an event;
+`scenario.consistency_checker.check_consistency` is called and verifies that the scenario makes sense.
 
 ## Caveats:
+
 - False positives: not all checks are implemented yet; more will come.
-- False negatives: it is possible that a scenario you know to be consistent is seen as inconsistent. That is probably a bug in the consistency checker itself, please report it.
-- Inherent limitations: if you have a custom event whose name conflicts with a builtin one, the consistency constraints of the builtin one will apply. For example: if you decide to name your custom event `bar-pebble-ready`, but you are working on a machine charm or don't have either way a `bar` container in your `metadata.yaml`, Scenario will flag that as inconsistent. 
+- False negatives: it is possible that a scenario you know to be consistent is seen as inconsistent. That is probably a
+  bug in the consistency checker itself, please report it.
+- Inherent limitations: if you have a custom event whose name conflicts with a builtin one, the consistency constraints
+  of the builtin one will apply. For example: if you decide to name your custom event `bar-pebble-ready`, but you are
+  working on a machine charm or don't have either way a `bar` container in your `metadata.yaml`, Scenario will flag that
+  as inconsistent.
 
 ## Bypassing the checker
-If you have a clear false negative, are explicitly testing 'edge', inconsistent situations, or for whatever reason the checker is in your way, you can set the `SCENARIO_SKIP_CONSISTENCY_CHECKS` envvar and skip it altogether. Hopefully you don't need that.
 
+If you have a clear false negative, are explicitly testing 'edge', inconsistent situations, or for whatever reason the
+checker is in your way, you can set the `SCENARIO_SKIP_CONSISTENCY_CHECKS` envvar and skip it altogether. Hopefully you
+don't need that.
 
 # Snapshot
 
-Scenario comes with a cli tool called `snapshot`. Assuming you've pip-installed `ops-scenario`, you should be able to reach the entry point by typing `scenario snapshot` in a shell.
+Scenario comes with a cli tool called `snapshot`. Assuming you've pip-installed `ops-scenario`, you should be able to
+reach the entry point by typing `scenario snapshot` in a shell so long as the install dir is in your `PATH`.
+
+Snapshot's purpose is to gather the `State` data structure from a real, live charm running in some cloud your local juju
+client has access to. This is handy in case:
 
-Snapshot's purpose is to gather the State data structure from a real, live charm running in some cloud your local juju client has access to. This is handy in case:
 - you want to write a test about the state the charm you're developing is currently in
-- your charm is bork or in some inconsistent state, and you want to write a test to check the charm will handle it correctly the next time around (aka regression testing)
+- your charm is bork or in some inconsistent state, and you want to write a test to check the charm will handle it
+  correctly the next time around (aka regression testing)
 - you are new to Scenario and want to quickly get started with a real-life example.
 
-Suppose you have a Juju model with a `prometheus-k8s` unit deployed as `prometheus-k8s/0`. If you type `scenario snapshot prometheus-k8s/0`, you will get a printout of the State object. Copy-paste that in some file, import all you need from `scenario`, and you have a working `State` that you can `.trigger()` events from.
-
-You can also pass a `--format json | pytest | state (default=state)` flag to obtain
-- jsonified `State` data structure, for portability
-- a full-fledged pytest test case (with imports and all), where you only have to fill in the charm type and the event that you wish to trigger. 
-
-# TODOS:
-- Recorder
+Suppose you have a Juju model with a `prometheus-k8s` unit deployed as `prometheus-k8s/0`. If you type
+`scenario snapshot prometheus-k8s/0`, you will get a printout of the State object. Pipe that out into some file, import
+all you need from `scenario`, and you have a working `State` that you can `Context.run` events with.
+
+You can also pass a `--format` flag to obtain instead:
+- a jsonified `State` data structure, for portability
+- a full-fledged pytest test case (with imports and all), where you only have to fill in the charm type and the event
+  that you wish to trigger.
```

### Comparing `ops-scenario-2.2/ops_scenario.egg-info/SOURCES.txt` & `ops-scenario-3.0a1/ops_scenario.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 .gitignore
+.pre-commit-config.yaml
+CODEOWNERS
+CONTRIBUTING.md
 LICENSE.txt
 README.md
 pyproject.toml
 tox.ini
 .github/workflows/build_wheels.yaml
 .github/workflows/quality_checks.yaml
 ops_scenario.egg-info/PKG-INFO
 ops_scenario.egg-info/SOURCES.txt
 ops_scenario.egg-info/dependency_links.txt
 ops_scenario.egg-info/entry_points.txt
 ops_scenario.egg-info/requires.txt
 ops_scenario.egg-info/top_level.txt
 resources/state-transition-model.png
 scenario/__init__.py
-scenario/capture_events.py
 scenario/consistency_checker.py
+scenario/context.py
+scenario/emitted_events.py
 scenario/fs_mocks.py
 scenario/logger.py
 scenario/mocking.py
 scenario/ops_main_mock.py
 scenario/runtime.py
 scenario/sequences.py
 scenario/state.py
 scenario/scripts/errors.py
 scenario/scripts/logger.py
 scenario/scripts/main.py
 scenario/scripts/snapshot.py
 scenario/scripts/utils.py
 tests/test_consistency_checker.py
 tests/test_emitted_events_util.py
+tests/test_plugin.py
 tests/test_runtime.py
 tests/resources/__init__.py
 tests/resources/demo_decorate_class.py
 tests/test_e2e/test_builtin_scenes.py
 tests/test_e2e/test_config.py
 tests/test_e2e/test_custom_event_triggers.py
 tests/test_e2e/test_deferred.py
```

### Comparing `ops-scenario-2.2/resources/state-transition-model.png` & `ops-scenario-3.0a1/resources/state-transition-model.png`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.2/scenario/capture_events.py` & `ops-scenario-3.0a1/scenario/emitted_events.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 #!/usr/bin/env python3
 # Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
+
 import typing
 from contextlib import contextmanager
 from typing import ContextManager, List, Type, TypeVar
 
+import pytest
 from ops.framework import (
     CommitEvent,
     EventBase,
     Framework,
     Handle,
     NoTypeError,
     PreCommitEvent,
 )
 
 _T = TypeVar("_T", bound=EventBase)
 
 
 @contextmanager
 def capture_events(
-    *types: Type[EventBase], include_framework=False, include_deferred=True
+    *types: Type[EventBase],
+    include_framework=False,
+    include_deferred=True,
 ) -> ContextManager[List[EventBase]]:
     """Capture all events of type `*types` (using instance checks).
 
+    Arguments exposed so that you can define your own fixtures if you want to.
+
     Example::
     >>> from ops.charm import StartEvent
     >>> from scenario import Event, State
     >>> from charm import MyCustomEvent, MyCharm  # noqa
     >>>
     >>> def test_my_event():
     >>>     with capture_events(StartEvent, MyCustomEvent) as captured:
-    >>>         State().trigger("start", MyCharm, meta=MyCharm.META)
+    >>>         trigger(State(), ("start", MyCharm, meta=MyCharm.META)
     >>>
     >>>     assert len(captured) == 2
     >>>     e1, e2 = captured
     >>>     assert isinstance(e2, MyCustomEvent)
     >>>     assert e2.custom_attr == 'foo'
     """
     allowed_types = types or (EventBase,)
@@ -56,34 +62,41 @@
         # Framework calls reemit() before emitting the main juju event. We intercept that call
         # and capture all events in storage.
 
         if not include_deferred:
             return _real_reemit(self)
 
         # load all notices from storage as events.
-        for event_path, observer_path, method_name in self._storage.notices():
+        for event_path, _, _ in self._storage.notices():
             event_handle = Handle.from_path(event_path)
             try:
                 event = self.load_snapshot(event_handle)
             except NoTypeError:
                 continue
             event = typing.cast(EventBase, event)
             event.deferred = False
             self._forget(event)  # prevent tracking conflicts
 
             if not include_framework and isinstance(
-                event, (PreCommitEvent, CommitEvent)
+                event,
+                (PreCommitEvent, CommitEvent),
             ):
                 continue
 
             if isinstance(event, allowed_types):
                 captured.append(event)
 
         return _real_reemit(self)
 
-    Framework._emit = _wrapped_emit  # type: ignore # noqa # ugly
-    Framework.reemit = _wrapped_reemit  # type: ignore # noqa # ugly
+    Framework._emit = _wrapped_emit  # type: ignore
+    Framework.reemit = _wrapped_reemit  # type: ignore
 
     yield captured
 
-    Framework._emit = _real_emit  # type: ignore # noqa # ugly
-    Framework.reemit = _real_reemit  # type: ignore # noqa # ugly
+    Framework._emit = _real_emit  # type: ignore
+    Framework.reemit = _real_reemit  # type: ignore
+
+
+@pytest.fixture()
+def emitted_events():
+    with capture_events() as captured:
+        yield captured
```

### Comparing `ops-scenario-2.2/scenario/consistency_checker.py` & `ops-scenario-3.0a1/scenario/consistency_checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,23 +24,25 @@
     state: "State",
     event: "Event",
     charm_spec: "_CharmSpec",
     juju_version: str,
 ):
     """Validate the combination of a state, an event, a charm spec, and a juju version.
 
-    When invoked, it performs a series of checks that validate that the state is consistent with itself, with
-    the event being emitted, the charm metadata, etc...
+    When invoked, it performs a series of checks that validate that the state is consistent with
+    itself, with the event being emitted, the charm metadata, etc...
 
-    This function performs some basic validation of the combination of inputs that goes into a scenario test and
-    determines if the scenario is a realistic/plausible/consistent one.
+    This function performs some basic validation of the combination of inputs that goes into a
+    scenario test and determines if the scenario is a realistic/plausible/consistent one.
 
-    A scenario is inconsistent if it can practically never occur because it contradicts the juju model.
-    For example: juju guarantees that upon calling config-get, a charm will only ever get the keys it declared
-    in its config.yaml. So a State declaring some config keys that are not in the charm's config.yaml is nonsense,
+    A scenario is inconsistent if it can practically never occur because it contradicts
+    the juju model.
+    For example: juju guarantees that upon calling config-get, a charm will only ever get the keys
+    it declared in its config.yaml.
+    So a State declaring some config keys that are not in the charm's config.yaml is nonsense,
     and the combination of the two is inconsistent.
     """
     juju_version: Tuple[int, ...] = tuple(map(int, juju_version.split(".")))
 
     if os.getenv("SCENARIO_SKIP_CONSISTENCY_CHECKS"):
         logger.info("skipping consistency checks.")
         return
@@ -52,91 +54,101 @@
         check_containers_consistency,
         check_config_consistency,
         check_event_consistency,
         check_secrets_consistency,
         check_relation_consistency,
     ):
         results = check(
-            state=state, event=event, charm_spec=charm_spec, juju_version=juju_version
+            state=state,
+            event=event,
+            charm_spec=charm_spec,
+            juju_version=juju_version,
         )
         errors.extend(results.errors)
         warnings.extend(results.warnings)
 
     if errors:
         err_fmt = "\n".join(errors)
         raise InconsistentScenarioError(
-            f"Inconsistent scenario. The following errors were found: {err_fmt}"
+            f"Inconsistent scenario. The following errors were found: {err_fmt}",
         )
     if warnings:
         err_fmt = "\n".join(warnings)
         logger.warning(
-            f"This scenario is probably inconsistent. Double check, and ignore this warning if you're sure. "
-            f"The following warnings were found: {err_fmt}"
+            f"This scenario is probably inconsistent. Double check, and ignore this "
+            f"warning if you're sure. "
+            f"The following warnings were found: {err_fmt}",
         )
 
 
 def check_event_consistency(
-    *, event: "Event", charm_spec: "_CharmSpec", **_kwargs
+    *,
+    event: "Event",
+    charm_spec: "_CharmSpec",
+    **_kwargs,  # noqa: U101
 ) -> Results:
     """Check the internal consistency of the Event data structure.
 
-    For example, it checks that a relation event has a relation instance, and that the relation endpoint
-    name matches the event prefix.
+    For example, it checks that a relation event has a relation instance, and that
+    the relation endpoint name matches the event prefix.
     """
     errors = []
     warnings = []
 
     # custom event: can't make assumptions about its name and its semantics
-    if not event._is_builtin_event(charm_spec):  # noqa
+    if not event._is_builtin_event(charm_spec):
         warnings.append(
             "this is a custom event; if its name makes it look like a builtin one "
             "(e.g. a relation event, or a workload event), you might get some false-negative "
-            "consistency checks."
+            "consistency checks.",
         )
 
-    if event._is_relation_event:  # noqa
+    if event._is_relation_event:
         if not event.relation:
             errors.append(
                 "cannot construct a relation event without the relation instance. "
-                "Please pass one."
+                "Please pass one.",
             )
         else:
             if not event.name.startswith(normalize_name(event.relation.endpoint)):
                 errors.append(
                     f"relation event should start with relation endpoint name. {event.name} does "
-                    f"not start with {event.relation.endpoint}."
+                    f"not start with {event.relation.endpoint}.",
                 )
 
-    if event._is_workload_event:  # noqa
+    if event._is_workload_event:
         if not event.container:
             errors.append(
                 "cannot construct a workload event without the container instance. "
-                "Please pass one."
+                "Please pass one.",
             )
         else:
             if not event.name.startswith(normalize_name(event.container.name)):
                 errors.append(
                     f"workload event should start with container name. {event.name} does "
-                    f"not start with {event.container.name}."
+                    f"not start with {event.container.name}.",
                 )
     return Results(errors, warnings)
 
 
 def check_config_consistency(
-    *, state: "State", charm_spec: "_CharmSpec", **_kwargs
+    *,
+    state: "State",
+    charm_spec: "_CharmSpec",
+    **_kwargs,  # noqa: U101
 ) -> Results:
     """Check the consistency of the state.config with the charm_spec.config (config.yaml)."""
     state_config = state.config
     meta_config = (charm_spec.config or {}).get("options", {})
     errors = []
 
     for key, value in state_config.items():
         if key not in meta_config:
             errors.append(
-                f"config option {key!r} in state.config but not specified in config.yaml."
+                f"config option {key!r} in state.config but not specified in config.yaml.",
             )
             continue
 
         # todo unify with snapshot's when merged.
         converters = {
             "string": str,
             "int": int,
@@ -151,43 +163,51 @@
             errors.append(f"config.yaml invalid; option {key!r} has no 'type'.")
             continue
 
         expected_type = converters.get(expected_type_name)
         if not isinstance(value, expected_type):
             errors.append(
                 f"config invalid; option {key!r} should be of type {expected_type} "
-                f"but is of type {type(value)}."
+                f"but is of type {type(value)}.",
             )
 
     return Results(errors, [])
 
 
 def check_secrets_consistency(
-    *, event: "Event", state: "State", juju_version: Tuple[int, ...], **_kwargs
+    *,
+    event: "Event",
+    state: "State",
+    juju_version: Tuple[int, ...],
+    **_kwargs,  # noqa: U101
 ) -> Results:
     """Check the consistency of Secret-related stuff."""
     errors = []
-    if not event._is_secret_event:  # noqa
+    if not event._is_secret_event:
         return Results(errors, [])
 
     if not state.secrets:
         errors.append(
-            "the event being processed is a secret event; but the state has no secrets."
+            "the event being processed is a secret event; but the state has no secrets.",
         )
     elif juju_version < (3,):
         errors.append(
             f"secrets are not supported in the specified juju version {juju_version}. "
-            f"Should be at least 3.0."
+            f"Should be at least 3.0.",
         )
 
     return Results(errors, [])
 
 
 def check_relation_consistency(
-    *, state: "State", event: "Event", charm_spec: "_CharmSpec", **_kwargs
+    *,
+    state: "State",
+    event: "Event",  # noqa: U100
+    charm_spec: "_CharmSpec",
+    **_kwargs,  # noqa: U101
 ) -> Results:
     errors = []
     nonpeer_relations_meta = chain(
         charm_spec.meta.get("requires", {}).items(),
         charm_spec.meta.get("provides", {}).items(),
     )
     peer_relations_meta = charm_spec.meta.get("peers", {}).items()
@@ -201,75 +221,82 @@
 
     # check relation types
     for endpoint, _ in peer_relations_meta:
         for relation in _get_relations(endpoint):
             if not isinstance(relation, PeerRelation):
                 errors.append(
                     f"endpoint {endpoint} is a peer relation; "
-                    f"expecting relation to be of type PeerRelation, got {type(relation)}"
+                    f"expecting relation to be of type PeerRelation, got {type(relation)}",
                 )
 
     for endpoint, relation_meta in all_relations_meta:
         expected_sub = relation_meta.get("scope", "") == "container"
         relations = _get_relations(endpoint)
         for relation in relations:
             is_sub = isinstance(relation, SubordinateRelation)
             if is_sub and not expected_sub:
                 errors.append(
                     f"endpoint {endpoint} is not a subordinate relation; "
                     f"expecting relation to be of type Relation, "
-                    f"got {type(relation)}"
+                    f"got {type(relation)}",
                 )
             if expected_sub and not is_sub:
                 errors.append(
                     f"endpoint {endpoint} is not a subordinate relation; "
                     f"expecting relation to be of type SubordinateRelation, "
-                    f"got {type(relation)}"
+                    f"got {type(relation)}",
                 )
 
     # check for duplicate endpoint names
     seen_endpoints = set()
-    for endpoint, relation_meta in all_relations_meta:
+    for endpoint, _ in all_relations_meta:
         if endpoint in seen_endpoints:
             errors.append("duplicate endpoint name in metadata.")
             break
         seen_endpoints.add(endpoint)
 
     return Results(errors, [])
 
 
 def check_containers_consistency(
-    *, state: "State", event: "Event", charm_spec: "_CharmSpec", **_kwargs
+    *,
+    state: "State",
+    event: "Event",
+    charm_spec: "_CharmSpec",
+    **_kwargs,  # noqa: U101
 ) -> Results:
-    """Check the consistency of `state.containers` vs. `charm_spec.meta` (metadata.yaml/containers)."""
+    """Check the consistency of `state.containers` vs. `charm_spec.meta`."""
     meta_containers = list(charm_spec.meta.get("containers", {}))
     state_containers = [c.name for c in state.containers]
     errors = []
 
-    # it's fine if you have containers in meta that are not in state.containers (yet), but it's not fine if:
-    # - you're processing a pebble-ready event and that container is not in state.containers or meta.containers
-    if event._is_workload_event:  # noqa
+    # it's fine if you have containers in meta that are not in state.containers (yet), but it's
+    # not fine if:
+    # - you're processing a pebble-ready event and that container is not in state.containers or
+    #   meta.containers
+    if event._is_workload_event:
         evt_container_name = event.name[: -len("-pebble-ready")]
         if evt_container_name not in meta_containers:
             errors.append(
-                f"the event being processed concerns container {evt_container_name!r}, but a container "
-                f"with that name is not declared in the charm metadata"
+                f"the event being processed concerns container {evt_container_name!r}, but a "
+                f"container with that name is not declared in the charm metadata",
             )
         if evt_container_name not in state_containers:
             errors.append(
-                f"the event being processed concerns container {evt_container_name!r}, but a container "
-                f"with that name is not present in the state. It's odd, but consistent, if it cannot "
-                f"connect; but it should at least be there."
+                f"the event being processed concerns container {evt_container_name!r}, but a "
+                f"container with that name is not present in the state. It's odd, but consistent, "
+                f"if it cannot connect; but it should at least be there.",
             )
 
     # - a container in state.containers is not in meta.containers
     if diff := (set(state_containers).difference(set(meta_containers))):
         errors.append(
-            f"some containers declared in the state are not specified in metadata. That's not possible. "
-            f"Missing from metadata: {diff}."
+            f"some containers declared in the state are not specified in metadata. "
+            f"That's not possible. "
+            f"Missing from metadata: {diff}.",
         )
 
     # guard against duplicate container names
     names = Counter(state_containers)
     if dupes := [n for n in names if names[n] > 1]:
         errors.append(f"Duplicate container name(s): {dupes}.")
```

### Comparing `ops-scenario-2.2/scenario/fs_mocks.py` & `ops-scenario-3.0a1/scenario/fs_mocks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pathlib
 from typing import Dict
 
 from ops.testing import _TestingFilesystem, _TestingStorageMount  # noqa
 
 
-# todo consider duplicating the filesystem on State.copy() to be able to diff and have true state snapshots
+# todo consider duplicating the filesystem on State.copy() to be able to diff
+#  and have true state snapshots
 class _MockStorageMount(_TestingStorageMount):
     def __init__(self, location: pathlib.PurePosixPath, src: pathlib.Path):
         """Creates a new simulated storage mount.
 
         Args:
             location: The path within simulated filesystem at which this storage will be mounted.
             src: The temporary on-disk location where the simulated storage will live.
@@ -24,12 +25,12 @@
 
 
 class _MockFileSystem(_TestingFilesystem):
     def __init__(self, mounts: Dict[str, _MockStorageMount]):
         super().__init__()
         self._mounts = mounts
 
-    def add_mount(self, *args, **kwargs):
+    def add_mount(self, *args, **kwargs):  # noqa: U100
         raise NotImplementedError("Cannot mutate mounts; declare them all in State.")
 
-    def remove_mount(self, *args, **kwargs):
+    def remove_mount(self, *args, **kwargs):  # noqa: U100
         raise NotImplementedError("Cannot mutate mounts; declare them all in State.")
```

### Comparing `ops-scenario-2.2/scenario/mocking.py` & `ops-scenario-3.0a1/scenario/mocking.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from scenario.state import PeerRelation
 
 if TYPE_CHECKING:
     from scenario.state import Container as ContainerSpec
     from scenario.state import (
         Event,
         ExecOutput,
-        PeerRelation,
         Relation,
         State,
         SubordinateRelation,
         _CharmSpec,
     )
 
 logger = scenario_logger.getChild("mocking")
@@ -47,16 +46,16 @@
     def wait_output(self):
         out = self._out
         exit_code = out.return_code
         if exit_code != 0:
             raise ExecError(list(self._command), exit_code, None, None)
         return out.stdout, out.stderr
 
-    def send_signal(self, sig: Union[int, str]):
-        pass
+    def send_signal(self, sig: Union[int, str]):  # noqa: U100
+        raise NotImplementedError()
 
 
 class _MockModelBackend(_ModelBackend):
     def __init__(self, state: "State", event: "Event", charm_spec: "_CharmSpec"):
         super().__init__()
         self._state = state
         self._event = event
@@ -67,19 +66,20 @@
             socket_path=socket_path,
             state=self._state,
             event=self._event,
             charm_spec=self._charm_spec,
         )
 
     def _get_relation_by_id(
-        self, rel_id
+        self,
+        rel_id,
     ) -> Union["Relation", "SubordinateRelation", "PeerRelation"]:
         try:
             return next(
-                filter(lambda r: r.relation_id == rel_id, self._state.relations)
+                filter(lambda r: r.relation_id == rel_id, self._state.relations),
             )
         except StopIteration as e:
             raise RuntimeError(f"Not found: relation with id={rel_id}.") from e
 
     def _get_secret(self, id=None, label=None):
         # cleanup id:
         if id and id.startswith("secret:"):
@@ -92,15 +92,15 @@
                 raise RuntimeError(f"not found: secret with id={id}.")
         elif label:
             try:
                 return next(filter(lambda s: s.label == label, self._state.secrets))
             except StopIteration:
                 raise RuntimeError(f"not found: secret with label={label}.")
         else:
-            raise RuntimeError(f"need id or label.")
+            raise RuntimeError("need id or label.")
 
     @staticmethod
     def _generate_secret_id():
         id = "".join(map(str, [random.choice(list(range(10))) for _ in range(20)]))
         return f"secret:{id}"
 
     def relation_get(self, rel_id, obj_name, app):
@@ -131,16 +131,16 @@
 
     def relation_list(self, relation_id: int) -> Tuple[str]:
         relation = self._get_relation_by_id(relation_id)
 
         if isinstance(relation, PeerRelation):
             return tuple(f"{self.app_name}/{unit_id}" for unit_id in relation.peers_ids)
         return tuple(
-            f"{relation._remote_app_name}/{unit_id}"  # noqa
-            for unit_id in relation._remote_unit_ids  # noqa
+            f"{relation._remote_app_name}/{unit_id}"
+            for unit_id in relation._remote_unit_ids
         )
 
     def config_get(self):
         state_config = self._state.config
 
         # add defaults
         charm_config = self._charm_spec.config
@@ -159,18 +159,18 @@
             logger.warning("network-get -r not implemented")
 
         network = next(filter(lambda r: r.name == binding_name, self._state.networks))
         return network.hook_tool_output_fmt()
 
     # setter methods: these can mutate the state.
     def application_version_set(self, version: str):
-        self._state.status._update_app_version(version)  # noqa
+        self._state.status._update_workload_version(version)
 
     def status_set(self, status: str, message: str = "", *, is_app: bool = False):
-        self._state.status._update_status(status, message, is_app)  # noqa
+        self._state.status._update_status(status, message, is_app)
 
     def juju_log(self, level: str, message: str):
         self._state.juju_log.append((level, message))
 
     def relation_set(self, relation_id: int, key: str, value: str, is_app: bool):
         relation = self._get_relation_by_id(relation_id)
         if is_app:
@@ -221,15 +221,18 @@
             revision = max(secret.contents.keys())
             if refresh:
                 secret._set_revision(revision)
 
         return secret.contents[revision]
 
     def secret_info_get(
-        self, *, id: Optional[str] = None, label: Optional[str] = None
+        self,
+        *,
+        id: Optional[str] = None,
+        label: Optional[str] = None,
     ) -> SecretInfo:
         secret = self._get_secret(id, label)
         if not secret.owner:
             raise RuntimeError(f"not the owner of {secret}")
 
         return SecretInfo(
             id=secret.id,
@@ -250,27 +253,21 @@
         expire: Optional[datetime.datetime] = None,
         rotate: Optional[SecretRotate] = None,
     ):
         secret = self._get_secret(id, label)
         if not secret.owner:
             raise RuntimeError(f"not the owner of {secret}")
 
-        revision = max(secret.contents.keys())
-        secret.contents[revision + 1] = content
-        if label:
-            secret.label = label
-        if description:
-            secret.description = description
-        if expire:
-            if isinstance(expire, datetime.timedelta):
-                expire = datetime.datetime.now() + expire
-            secret.expire = expire
-        if rotate:
-            secret.rotate = rotate
-        raise NotImplementedError("secret_set")
+        secret._update_metadata(
+            content=content,
+            label=label,
+            description=description,
+            expire=expire,
+            rotate=rotate,
+        )
 
     def secret_grant(self, id: str, relation_id: int, *, unit: Optional[str] = None):
         secret = self._get_secret(id)
         if not secret.owner:
             raise RuntimeError(f"not the owner of {secret}")
 
         grantee = unit or self._get_relation_by_id(relation_id).remote_app_name
@@ -299,39 +296,39 @@
             secret.contents.clear()
 
     def relation_remote_app_name(self, relation_id: int):
         relation = self._get_relation_by_id(relation_id)
         return relation.remote_app_name
 
     # TODO:
-    def action_set(self, *args, **kwargs):
+    def action_set(self, *args, **kwargs):  # noqa: U100
         raise NotImplementedError("action_set")
 
-    def action_fail(self, *args, **kwargs):
+    def action_fail(self, *args, **kwargs):  # noqa: U100
         raise NotImplementedError("action_fail")
 
-    def action_log(self, *args, **kwargs):
+    def action_log(self, *args, **kwargs):  # noqa: U100
         raise NotImplementedError("action_log")
 
-    def storage_add(self, *args, **kwargs):
+    def storage_add(self, *args, **kwargs):  # noqa: U100
         raise NotImplementedError("storage_add")
 
     def action_get(self):
         raise NotImplementedError("action_get")
 
-    def resource_get(self, *args, **kwargs):
+    def resource_get(self, *args, **kwargs):  # noqa: U100
         raise NotImplementedError("resource_get")
 
-    def storage_list(self, *args, **kwargs):
+    def storage_list(self, *args, **kwargs):  # noqa: U100
         raise NotImplementedError("storage_list")
 
-    def storage_get(self, *args, **kwargs):
+    def storage_get(self, *args, **kwargs):  # noqa: U100
         raise NotImplementedError("storage_get")
 
-    def planned_units(self, *args, **kwargs):
+    def planned_units(self, *args, **kwargs):  # noqa: U100
         raise NotImplementedError("planned_units")
 
 
 class _MockPebbleClient(_TestingPebbleClient):
     def __init__(
         self,
         socket_path: str,
@@ -349,36 +346,36 @@
         return self._container.plan
 
     @property
     def _container(self) -> "ContainerSpec":
         container_name = self.socket_path.split("/")[-2]
         try:
             return next(
-                filter(lambda x: x.name == container_name, self._state.containers)
+                filter(lambda x: x.name == container_name, self._state.containers),
             )
         except StopIteration:
             raise RuntimeError(
                 f"container with name={container_name!r} not found. "
                 f"Did you forget a Container, or is the socket path "
-                f"{self.socket_path!r} wrong?"
+                f"{self.socket_path!r} wrong?",
             )
 
     @property
     def _fs(self):
         return self._container.filesystem
 
     @property
     def _layers(self) -> Dict[str, pebble.Layer]:
         return self._container.layers
 
     @property
     def _service_status(self) -> Dict[str, pebble.ServiceStatus]:
         return self._container.service_status
 
-    def exec(self, *args, **kwargs):
+    def exec(self, *args, **kwargs):  # noqa: U100
         cmd = tuple(args[0])
         out = self._container.exec_mock.get(cmd)
         if not out:
             raise RuntimeError(f"mock for cmd {cmd} not found.")
 
         change_id = out._run()
         return _MockExecProcess(change_id=change_id, command=cmd, out=out)
```

### Comparing `ops-scenario-2.2/scenario/ops_main_mock.py` & `ops-scenario-3.0a1/scenario/ops_main_mock.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,20 +37,23 @@
     """Set up the charm and dispatch the observed event."""
     charm_class = charm_spec.charm_type
     charm_dir = _get_charm_dir()
 
     from scenario.mocking import _MockModelBackend
 
     model_backend = _MockModelBackend(  # pyright: reportPrivateUsage=false
-        state=state, event=event, charm_spec=charm_spec
+        state=state,
+        event=event,
+        charm_spec=charm_spec,
     )
     debug = "JUJU_DEBUG" in os.environ
     setup_root_logging(model_backend, debug=debug)
     logger.debug(
-        "Operator Framework %s up and running.", ops.__version__
+        "Operator Framework %s up and running.",
+        ops.__version__,
     )  # type:ignore
 
     dispatcher = _Dispatcher(charm_dir)
     dispatcher.run_any_legacy_hook()
 
     metadata = (charm_dir / "metadata.yaml").read_text()
     actions_meta = charm_dir / "actions.yaml"
@@ -82,15 +85,15 @@
 
         if pre_event:
             pre_event(charm)
 
         if not getattr(charm.on, dispatcher.event_name, None):
             raise NoObserverError(
                 f"Charm has no registered observers for {dispatcher.event_name!r}. "
-                f"This is probably not what you were looking for."
+                f"This is probably not what you were looking for.",
             )
 
         _emit_charm_event(charm, dispatcher.event_name)
 
         if post_event:
             post_event(charm)
```

### Comparing `ops-scenario-2.2/scenario/runtime.py` & `ops-scenario-3.0a1/scenario/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,40 +16,33 @@
     Optional,
     Type,
     TypeVar,
     Union,
 )
 
 import yaml
-from ops.framework import _event_regex  # noqa
+from ops.framework import _event_regex
 from ops.storage import SQLiteStorage
 
 from scenario.logger import logger as scenario_logger
 from scenario.ops_main_mock import NoObserverError
 from scenario.state import DeferredEvent, PeerRelation, StoredState
 
 if TYPE_CHECKING:
     from ops.testing import CharmType
 
-    from scenario.state import (
-        AnyRelation,
-        DeferredEvent,
-        Event,
-        State,
-        StoredState,
-        _CharmSpec,
-    )
+    from scenario.state import AnyRelation, Event, State, _CharmSpec
 
     _CT = TypeVar("_CT", bound=Type[CharmType])
 
     PathLike = Union[str, Path]
 
 logger = scenario_logger.getChild("runtime")
 STORED_STATE_REGEX = re.compile(
-    r"((?P<owner_path>.*)\/)?(?P<data_type_name>\D+)\[(?P<name>.*)\]"
+    r"((?P<owner_path>.*)\/)?(?P<data_type_name>\D+)\[(?P<name>.*)\]",
 )
 EVENT_REGEX = re.compile(_event_regex)
 
 RUNTIME_MODULE = Path(__file__).parent
 
 
 class ScenarioRuntimeError(RuntimeError):
@@ -57,15 +50,15 @@
 
 
 class UncaughtCharmError(ScenarioRuntimeError):
     """Error raised if the charm raises while handling the event being dispatched."""
 
 
 class DirtyVirtualCharmRootError(ScenarioRuntimeError):
-    """Error raised when the runtime can't initialize the vroot without overwriting existing metadata files."""
+    """Error raised when the runtime can't initialize the vroot without overwriting metadata."""
 
 
 class InconsistentScenarioError(ScenarioRuntimeError):
     """Error raised when the combination of state and event is inconsistent."""
 
 
 class UnitStateDB:
@@ -104,15 +97,17 @@
 
         deferred = []
         for handle_path in db.list_snapshots():
             if EVENT_REGEX.match(handle_path):
                 notices = db.notices(handle_path)
                 for handle, owner, observer in notices:
                     event = DeferredEvent(
-                        handle_path=handle, owner=owner, observer=observer
+                        handle_path=handle,
+                        owner=owner,
+                        observer=observer,
                     )
                     deferred.append(event)
 
         db.close()
         return deferred
 
     def apply_state(self, state: "State"):
@@ -120,15 +115,15 @@
         db = self._open_db()
         for event in state.deferred:
             db.save_notice(event.handle_path, event.owner, event.observer)
             try:
                 marshal.dumps(event.snapshot_data)
             except ValueError as e:
                 raise ValueError(
-                    f"unable to save the data for {event}, it must contain only simple types."
+                    f"unable to save the data for {event}, it must contain only simple types.",
                 ) from e
             db.save_snapshot(event.handle_path, event.snapshot_data)
 
         for stored_state in state.stored_state:
             db.save_snapshot(stored_state.handle_path, stored_state.content)
 
         db.close()
@@ -141,90 +136,88 @@
     """
 
     def __init__(
         self,
         charm_spec: "_CharmSpec",
         charm_root: Optional["PathLike"] = None,
         juju_version: str = "3.0.0",
-        unit_id: int = 0,
     ):
         self._charm_spec = charm_spec
         self._juju_version = juju_version
         self._charm_root = charm_root
 
         app_name = self._charm_spec.meta.get("name")
         if not app_name:
             raise ValueError('invalid metadata: mandatory "name" field is missing.')
 
         self._app_name = app_name
-        self._unit_id = unit_id
-        self._unit_name = f"{app_name}/{unit_id}"
 
     @staticmethod
     def _cleanup_env(env):
         # TODO consider cleaning up env on __delete__, but ideally you should be
         #  running this in a clean venv or a container anyway.
         # cleanup env, in case we'll be firing multiple events, we don't want to accumulate.
         for key in env:
             # os.unsetenv does not work !?
             del os.environ[key]
 
     def _get_event_env(self, state: "State", event: "Event", charm_root: Path):
         if event.name.endswith("_action"):
-            # todo: do we need some special metadata, or can we assume action names are always dashes?
+            # todo: do we need some special metadata, or can we assume action names
+            #  are always dashes?
             action_name = event.name[: -len("_action")].replace("_", "-")
         else:
             action_name = ""
 
         env = {
             "JUJU_VERSION": self._juju_version,
-            "JUJU_UNIT_NAME": self._unit_name,
+            "JUJU_UNIT_NAME": f"{self._app_name}/{state.unit_id}",
             "_": "./dispatch",
             "JUJU_DISPATCH_PATH": f"hooks/{event.name}",
             "JUJU_MODEL_NAME": state.model.name,
             "JUJU_ACTION_NAME": action_name,
             "JUJU_MODEL_UUID": state.model.uuid,
-            "JUJU_CHARM_DIR": str(charm_root.absolute())
+            "JUJU_CHARM_DIR": str(charm_root.absolute()),
             # todo consider setting pwd, (python)path
         }
 
         relation: "AnyRelation"
 
-        if event._is_relation_event and (relation := event.relation):  # noqa
+        if event._is_relation_event and (relation := event.relation):
             if isinstance(relation, PeerRelation):
                 remote_app_name = self._app_name
             else:
-                remote_app_name = relation._remote_app_name  # noqa
+                remote_app_name = relation._remote_app_name
             env.update(
                 {
                     "JUJU_RELATION": relation.endpoint,
                     "JUJU_RELATION_ID": str(relation.relation_id),
                     "JUJU_REMOTE_APP": remote_app_name,
-                }
+                },
             )
 
             remote_unit_id = event.relation_remote_unit_id
             if (
                 remote_unit_id is None
             ):  # don't check truthiness because it could be int(0)
-                remote_unit_ids = relation._remote_unit_ids  # noqa
+                remote_unit_ids = relation._remote_unit_ids  # pyright: ignore
 
                 if len(remote_unit_ids) == 1:
                     remote_unit_id = remote_unit_ids[0]
                     logger.info(
                         "there's only one remote unit, so we set JUJU_REMOTE_UNIT to it, "
                         "but you probably should be parametrizing the event with `remote_unit_id` "
-                        "to be explicit."
+                        "to be explicit.",
                     )
                 else:
                     remote_unit_id = remote_unit_ids[0]
                     logger.warning(
                         "remote unit ID unset, and multiple remote unit IDs are present; "
                         "We will pick the first one and hope for the best. You should be passing "
-                        "`remote_unit_id` to the Event constructor."
+                        "`remote_unit_id` to the Event constructor.",
                     )
 
             if remote_unit_id is not None:
                 remote_unit = f"{remote_app_name}/{remote_unit_id}"
                 env["JUJU_REMOTE_UNIT"] = remote_unit
                 if event.name.endswith("_relation_departed"):
                     env["JUJU_DEPARTING_UNIT"] = remote_unit
@@ -233,15 +226,15 @@
             env.update({"JUJU_WORKLOAD_NAME": container.name})
 
         if secret := event.secret:
             env.update(
                 {
                     "JUJU_SECRET_ID": secret.id,
                     "JUJU_SECRET_LABEL": secret.label or "",
-                }
+                },
             )
 
         return env
 
     @staticmethod
     def _wrap(charm_type: "_CT") -> "_CT":
         # dark sorcery to work around framework using class attrs to hold on to event sources
@@ -256,19 +249,19 @@
             on = WrappedEvents()
 
         WrappedCharm.__name__ = charm_type.__name__
         return WrappedCharm
 
     @contextmanager
     def virtual_charm_root(self):
-        # If we are using runtime on a real charm, we can make some assumptions about the directory structure
-        #  we are going to find.
-        #  If we're, say, dynamically defining charm types and doing tests on them, we'll have to generate
-        #  the metadata files ourselves. To be sure, we ALWAYS use a tempdir. Ground truth is what the user
-        #  passed via the CharmSpec
+        # If we are using runtime on a real charm, we can make some assumptions about the
+        # directory structure we are going to find.
+        # If we're, say, dynamically defining charm types and doing tests on them, we'll have to
+        # generate the metadata files ourselves. To be sure, we ALWAYS use a tempdir. Ground truth
+        # is what the user passed via the CharmSpec
         spec = self._charm_spec
 
         if vroot := self._charm_root:
             vroot_is_custom = True
             virtual_charm_root = Path(vroot)
         else:
             vroot = tempfile.TemporaryDirectory()
@@ -276,35 +269,35 @@
             vroot_is_custom = False
 
         metadata_yaml = virtual_charm_root / "metadata.yaml"
         config_yaml = virtual_charm_root / "config.yaml"
         actions_yaml = virtual_charm_root / "actions.yaml"
 
         metadata_files_present = any(
-            (file.exists() for file in (metadata_yaml, config_yaml, actions_yaml))
+            file.exists() for file in (metadata_yaml, config_yaml, actions_yaml)
         )
 
         if spec.is_autoloaded and vroot_is_custom:
             # since the spec is autoloaded, in theory the metadata contents won't differ, so we can
             # overwrite away even if the custom vroot is the real charm root (the local repo).
             # Still, log it for clarity.
             if metadata_files_present:
                 logger.info(
                     f"metadata files found in custom vroot {vroot}. "
                     f"The spec was autoloaded so the contents should be identical. "
-                    f"Proceeding..."
+                    f"Proceeding...",
                 )
 
         elif not spec.is_autoloaded and metadata_files_present:
             logger.error(
                 f"Some metadata files found in custom user-provided vroot {vroot} "
                 f"while you have passed meta, config or actions to trigger(). "
                 "We don't want to risk overwriting them mindlessly, so we abort. "
                 "You should not include any metadata files in the charm_root. "
-                "Single source of truth are the arguments passed to trigger(). "
+                "Single source of truth are the arguments passed to trigger(). ",
             )
             raise DirtyVirtualCharmRootError(vroot)
 
         metadata_yaml.write_text(yaml.safe_dump(spec.meta))
         config_yaml.write_text(yaml.safe_dump(spec.config or {}))
         actions_yaml.write_text(yaml.safe_dump(spec.actions or {}))
 
@@ -315,35 +308,36 @@
 
     @staticmethod
     def _get_state_db(temporary_charm_root: Path):
         charm_state_path = temporary_charm_root / ".unit-state.db"
         return UnitStateDB(charm_state_path)
 
     def _initialize_storage(self, state: "State", temporary_charm_root: Path):
-        """Before we start processing this event, expose the relevant parts of State through the storage."""
+        """Before we start processing this event, store the relevant parts of State."""
         store = self._get_state_db(temporary_charm_root)
         store.apply_state(state)
 
     def _close_storage(self, state: "State", temporary_charm_root: Path):
-        """Now that we're done processing this event, read the charm state and expose it via State."""
+        """Now that we're done processing this event, read the charm state and expose it."""
         store = self._get_state_db(temporary_charm_root)
         deferred = store.get_deferred_events()
         stored_state = store.get_stored_state()
         return state.replace(deferred=deferred, stored_state=stored_state)
 
     def exec(
         self,
         state: "State",
         event: "Event",
         pre_event: Optional[Callable[["CharmType"], None]] = None,
         post_event: Optional[Callable[["CharmType"], None]] = None,
     ) -> "State":
         """Runs an event with this state as initial state on a charm.
 
-        Returns the 'output state', that is, the state as mutated by the charm during the event handling.
+        Returns the 'output state', that is, the state as mutated by the charm during the
+        event handling.
 
         This will set the environment up and call ops.main.main().
         After that it's up to ops.
         """
         from scenario.consistency_checker import check_consistency  # avoid cycles
 
         check_consistency(state, event, self._charm_spec, self._juju_version)
@@ -360,37 +354,40 @@
             #  generating hook tool executables
 
             logger.info(" - initializing storage")
             self._initialize_storage(state, temporary_charm_root)
 
             logger.info(" - preparing env")
             env = self._get_event_env(
-                state=state, event=event, charm_root=temporary_charm_root
+                state=state,
+                event=event,
+                charm_root=temporary_charm_root,
             )
             os.environ.update(env)
 
             logger.info(" - Entering ops.main (mocked).")
-            # we don't import from ops.main because we need some extras, such as the pre/post_event hooks
+            # we don't import from ops.main because we need some extras, such as the
+            # pre/post_event hooks
             from scenario.ops_main_mock import main as mocked_main
 
             try:
                 mocked_main(
                     pre_event=pre_event,
                     post_event=post_event,
                     state=output_state,
                     event=event,
                     charm_spec=self._charm_spec.replace(
-                        charm_type=self._wrap(charm_type)
+                        charm_type=self._wrap(charm_type),
                     ),
                 )
             except NoObserverError:
                 raise  # propagate along
             except Exception as e:
                 raise UncaughtCharmError(
-                    f"Uncaught error in operator/charm code: {e}."
+                    f"Uncaught exception ({type(e)}) in operator/charm code: {e!r}",
                 ) from e
             finally:
                 logger.info(" - Exited ops.main.")
 
             logger.info(" - Clearing env")
             self._cleanup_env(env)
 
@@ -409,15 +406,14 @@
     post_event: Optional[Callable[["CharmType"], None]] = None,
     # if not provided, will be autoloaded from charm_type.
     meta: Optional[Dict[str, Any]] = None,
     actions: Optional[Dict[str, Any]] = None,
     config: Optional[Dict[str, Any]] = None,
     charm_root: Optional[Dict["PathLike", "PathLike"]] = None,
     juju_version: str = "3.0",
-    unit_id: int = 0,
 ) -> "State":
     """Trigger a charm execution with an Event and a State.
 
     Calling this function will call ops' main() and set up the context according to the specified
     State, then emit the event on the charm.
 
     :arg event: the Event that the charm will respond to. Can be a string or an Event instance.
@@ -431,47 +427,47 @@
     :arg meta: charm metadata to use. Needs to be a valid metadata.yaml format (as a python dict).
         If none is provided, we will search for a ``metadata.yaml`` file in the charm root.
     :arg actions: charm actions to use. Needs to be a valid actions.yaml format (as a python dict).
         If none is provided, we will search for a ``actions.yaml`` file in the charm root.
     :arg config: charm config to use. Needs to be a valid config.yaml format (as a python dict).
         If none is provided, we will search for a ``config.yaml`` file in the charm root.
     :arg juju_version: Juju agent version to simulate.
-    :arg unit_id: The ID of the Juju unit that is charm execution is running on.
     :arg charm_root: virtual charm root the charm will be executed with.
         If the charm, say, expects a `./src/foo/bar.yaml` file present relative to the
         execution cwd, you need to use this. E.g.:
 
         >>> virtual_root = tempfile.TemporaryDirectory()
         >>> local_path = Path(local_path.name)
         >>> (local_path / 'foo').mkdir()
         >>> (local_path / 'foo' / 'bar.yaml').write_text('foo: bar')
-        >>> scenario.State().trigger(... charm_root=virtual_root)
-
+        >>> scenario, State(), (... charm_root=virtual_root)
 
     """
     from scenario.state import Event, _CharmSpec
 
     if isinstance(event, str):
         event = Event(event)
 
     if not any((meta, actions, config)):
         logger.debug("Autoloading charmspec...")
         spec = _CharmSpec.autoload(charm_type)
     else:
         if not meta:
             meta = {"name": str(charm_type.__name__)}
         spec = _CharmSpec(
-            charm_type=charm_type, meta=meta, actions=actions, config=config
+            charm_type=charm_type,
+            meta=meta,
+            actions=actions,
+            config=config,
         )
 
     runtime = Runtime(
         charm_spec=spec,
         juju_version=juju_version,
         charm_root=charm_root,
-        unit_id=unit_id,
     )
 
     return runtime.exec(
         state=state,
         event=event,
         pre_event=pre_event,
         post_event=post_event,
```

### Comparing `ops-scenario-2.2/scenario/scripts/main.py` & `ops-scenario-3.0a1/scenario/scripts/main.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.2/scenario/scripts/snapshot.py` & `ops-scenario-3.0a1/scenario/scripts/snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,28 +64,31 @@
 
 def format_state(state: State):
     """Stringify this State as nicely as possible."""
     return _try_format(repr(state))
 
 
 PYTEST_TEST_TEMPLATE = """
-from scenario.state import *
+from scenario import *
 from charm import {ct}
 
 def test_case():
     # Arrange: prepare the state
     state = {state}
-    
-    #Act: trigger an event on the state 
-    out = state.trigger(
+
+    #Act: trigger an event on the state
+    ctx = Context(
+        {ct},
+        juju_version="{jv}")
+
+    out = ctx.run(
         {en}
-        {ct}
-        juju_version="{jv}"
+        state,
         )
-        
+
     # Assert: verify that the output state is the way you want it to be
     # TODO: add assertions
 """
 
 
 def format_test_case(
     state: State,
@@ -95,15 +98,15 @@
 ):
     """Format this State as a pytest test case."""
     ct = charm_type_name or "CHARM_TYPE,  # TODO: replace with charm type name"
     en = event_name or "EVENT_NAME,  # TODO: replace with event name"
     jv = juju_version or "3.0,  # TODO: check juju version is correct"
     state_fmt = repr(state)
     return _try_format(
-        PYTEST_TEST_TEMPLATE.format(state=state_fmt, ct=ct, en=en, jv=jv)
+        PYTEST_TEST_TEMPLATE.format(state=state_fmt, ct=ct, en=en, jv=jv),
     )
 
 
 def _juju_run(cmd: str, model=None) -> Dict[str, Any]:
     """Execute juju {command} in a given model."""
     _model = f" -m {model}" if model else ""
     cmd = f"juju {cmd}{_model} --format json"
@@ -139,47 +142,48 @@
     logger.info("getting leader...")
     return _juju_exec(target, model, "is-leader") == "True"
 
 
 def get_network(target: JujuUnitName, model: Optional[str], endpoint: str) -> Network:
     """Get the Network data structure for this endpoint."""
     raw = _juju_exec(target, model, f"network-get {endpoint}")
-    jsn = yaml.safe_load(raw)
+    json_data = yaml.safe_load(raw)
 
     bind_addresses = []
-    for raw_bind in jsn["bind-addresses"]:
+    for raw_bind in json_data["bind-addresses"]:
         addresses = []
         for raw_adds in raw_bind["addresses"]:
             addresses.append(
                 Address(
                     hostname=raw_adds["hostname"],
                     value=raw_adds["value"],
                     cidr=raw_adds["cidr"],
                     address=raw_adds.get("address", ""),
-                )
+                ),
             )
 
         bind_addresses.append(
             BindAddress(
-                interface_name=raw_bind.get("interface-name", ""), addresses=addresses
-            )
+                interface_name=raw_bind.get("interface-name", ""),
+                addresses=addresses,
+            ),
         )
     return Network(
         name=endpoint,
         bind_addresses=bind_addresses,
-        egress_subnets=jsn.get("egress-subnets", None),
-        ingress_addresses=jsn.get("ingress-addresses", None),
+        egress_subnets=json_data.get("egress-subnets", None),
+        ingress_addresses=json_data.get("ingress-addresses", None),
     )
 
 
 def get_secrets(
-    target: JujuUnitName,
-    model: Optional[str],
-    metadata: Dict,
-    relations: Tuple[str, ...] = (),
+    target: JujuUnitName,  # noqa: U100
+    model: Optional[str],  # noqa: U100
+    metadata: Dict,  # noqa: U100
+    relations: Tuple[str, ...] = (),  # noqa: U100
 ) -> List[Secret]:
     """Get Secret list from the charm."""
     logger.warning("Secrets snapshotting not implemented yet. Also, are you *sure*?")
     return []
 
 
 def get_networks(
@@ -221,32 +225,38 @@
     return yaml.safe_load(raw_meta)
 
 
 class RemotePebbleClient:
     """Clever little class that wraps calls to a remote pebble client."""
 
     def __init__(
-        self, container: str, target: JujuUnitName, model: Optional[str] = None
+        self,
+        container: str,
+        target: JujuUnitName,
+        model: Optional[str] = None,
     ):
         self.socket_path = f"/charm/containers/{container}/pebble.socket"
         self.container = container
         self.target = target
         self.model = model
 
     def _run(self, cmd: str) -> str:
         _model = f" -m {self.model}" if self.model else ""
-        command = f"juju ssh{_model} --container {self.container} {self.target.unit_name} /charm/bin/pebble {cmd}"
+        command = (
+            f"juju ssh{_model} --container {self.container} {self.target.unit_name} "
+            f"/charm/bin/pebble {cmd}"
+        )
         proc = run(shlex.split(command), capture_output=True, text=True)
         if proc.returncode == 0:
             return proc.stdout
         raise RuntimeError(
             f"error wrapping pebble call with {command}: "
             f"process exited with {proc.returncode}; "
             f"stdout = {proc.stdout}; "
-            f"stderr = {proc.stderr}"
+            f"stderr = {proc.stderr}",
         )
 
     def can_connect(self) -> bool:
         try:
             version = self.get_system_info()
         except Exception:
             return False
@@ -256,30 +266,37 @@
         return self._run("version")
 
     def get_plan(self) -> dict:
         plan_raw = self._run("plan")
         return yaml.safe_load(plan_raw)
 
     def pull(
-        self, path: str, *, encoding: Optional[str] = "utf-8"
+        self,
+        path: str,  # noqa: U100
+        *,
+        encoding: Optional[str] = "utf-8",  # noqa: U100
     ) -> Union[BinaryIO, TextIO]:
         raise NotImplementedError()
 
     def list_files(
-        self, path: str, *, pattern: Optional[str] = None, itself: bool = False
+        self,
+        path: str,  # noqa: U100
+        *,
+        pattern: Optional[str] = None,  # noqa: U100
+        itself: bool = False,  # noqa: U100
     ) -> List[ops.pebble.FileInfo]:
         raise NotImplementedError()
 
     def get_checks(
         self,
         level: Optional[ops.pebble.CheckLevel] = None,
         names: Optional[Iterable[str]] = None,
     ) -> List[ops.pebble.CheckInfo]:
         _level = f" --level={level}" if level else ""
-        _names = (" " + f" ".join(names)) if names else ""
+        _names = (" " + " ".join(names)) if names else ""
         out = self._run(f"checks{_level}{_names}")
         if out == "Plan has no health checks.":
             return []
         raise NotImplementedError()
 
 
 def fetch_file(
@@ -287,33 +304,36 @@
     remote_path: Union[Path, str],
     container_name: str,
     local_path: Union[Path, str],
     model: Optional[str] = None,
 ) -> None:
     """Download a file from a live unit to a local path."""
     model_arg = f" -m {model}" if model else ""
-    scp_cmd = f"juju scp --container {container_name}{model_arg} {target.unit_name}:{remote_path} {local_path}"
+    scp_cmd = (
+        f"juju scp --container {container_name}{model_arg} "
+        f"{target.unit_name}:{remote_path} {local_path}"
+    )
     run(shlex.split(scp_cmd))
 
 
 def get_mounts(
     target: JujuUnitName,
     model: Optional[str],
     container_name: str,
     container_meta: Dict,
     fetch_files: Optional[List[Path]] = None,
     temp_dir_base_path: Path = SNAPSHOT_OUTPUT_DIR,
 ) -> Dict[str, Mount]:
-    """Get named Mounts from a container's metadata, and download specified files from the target unit."""
+    """Get named Mounts from a container's metadata, and download specified files from the unit."""
     mount_meta = container_meta.get("mounts")
 
     if fetch_files and not mount_meta:
         logger.error(
             f"No mounts defined for container {container_name} in metadata.yaml. "
-            f"Cannot fetch files {fetch_files} for this container."
+            f"Cannot fetch files {fetch_files} for this container.",
         )
         return {}
 
     mount_spec = {}
     for mt in mount_meta or ():
         if name := mt.get("storage"):
             mount_spec[name] = mt["location"]
@@ -325,15 +345,16 @@
         found = None
         for mn, mt in mount_spec.items():
             if str(remote_path).startswith(mt):
                 found = mn, mt
 
         if not found:
             logger.error(
-                f"could not find mount corresponding to requested remote_path {remote_path}: skipping..."
+                "could not find mount corresponding to requested remote_path "
+                f"{remote_path}: skipping...",
             )
             continue
 
         mount_name, src = found
         mount = mounts.get(mount_name)
         if not mount:
             # create the mount obj and tempdir
@@ -414,66 +435,66 @@
         containers.append(container)
     return containers
 
 
 def get_juju_status(model: Optional[str]) -> Dict:
     """Return juju status as json."""
     logger.info("getting status...")
-    return _juju_run(f"status --relations", model=model)
+    return _juju_run("status --relations", model=model)
 
 
 def get_status(juju_status: Dict, target: JujuUnitName) -> Status:
     """Parse `juju status` to get the Status data structure and some relation information."""
     app = juju_status["applications"][target.app_name]
 
     app_status_raw = app["application-status"]
     app_status = app_status_raw["current"], app_status_raw.get("message", "")
 
     unit_status_raw = app["units"][target]["workload-status"]
     unit_status = unit_status_raw["current"], unit_status_raw.get("message", "")
 
-    app_version = app.get("version", "")
+    workload_version = app.get("version", "")
     return Status(
         app=_EntityStatus(*app_status),
         unit=_EntityStatus(*unit_status),
-        app_version=app_version,
+        workload_version=workload_version,
     )
 
 
 def get_endpoints(juju_status: Dict, target: JujuUnitName) -> Tuple[str, ...]:
     """Parse `juju status` to get the relation names owned by the target."""
     app = juju_status["applications"][target.app_name]
     relations_raw = app.get("relations", None)
     if not relations_raw:
         return ()
     relations = tuple(relations_raw.keys())
     return relations
 
 
 def get_config(
-    target: JujuUnitName, model: Optional[str]
+    target: JujuUnitName,
+    model: Optional[str],
 ) -> Dict[str, Union[str, int, float, bool]]:
     """Get config dict from target."""
 
     logger.info("getting config...")
-    _model = f" -m {model}" if model else ""
-    jsn = _juju_run(f"config {target.app_name}", model=model)
+    json_data = _juju_run(f"config {target.app_name}", model=model)
 
     # dispatch table for builtin config options
     converters = {
         "string": str,
         "int": int,
         "integer": int,  # fixme: which one is it?
         "number": float,
         "boolean": lambda x: x == "true",
         "attrs": lambda x: x,  # fixme: wot?
     }
 
     cfg = {}
-    for name, option in jsn.get("settings", ()).items():
+    for name, option in json_data.get("settings", ()).items():
         if value := option.get("value"):
             try:
                 converter = converters[option["type"]]
             except KeyError:
                 raise ValueError(f'unrecognized type {option["type"]}')
             cfg[name] = converter(value)
 
@@ -499,32 +520,31 @@
     model: Optional[str],
     metadata: Dict,
     include_juju_relation_data=False,
 ) -> List[Relation]:
     """Get the list of relations active for this target."""
     logger.info("getting relations...")
 
-    _model = f" -m {model}" if model else ""
     try:
-        jsn = _juju_run(f"show-unit {target}", model=model)
+        json_data = _juju_run(f"show-unit {target}", model=model)
     except json.JSONDecodeError as e:
         raise InvalidTargetUnitName(target) from e
 
     def _clean(relation_data: dict):
         if include_juju_relation_data:
             return relation_data
         else:
             for key in JUJU_RELATION_KEYS:
                 del relation_data[key]
         return relation_data
 
     relations = []
-    for raw_relation in jsn[target].get("relation-info", ()):
+    for raw_relation in json_data[target].get("relation-info", ()):
         logger.debug(
-            f"  getting relation data for endpoint {raw_relation.get('endpoint')!r}"
+            f"  getting relation data for endpoint {raw_relation.get('endpoint')!r}",
         )
         related_units = raw_relation.get("related-units")
         if not related_units:
             continue
         #    related-units:
         #      owner/0:
         #        in-scope: true
@@ -532,15 +552,17 @@
         #          egress-subnets: 10.152.183.130/32
         #          ingress-address: 10.152.183.130
         #          private-address: 10.152.183.130
 
         relation_id = raw_relation["relation-id"]
 
         local_unit_data_raw = _juju_exec(
-            target, model, f"relation-get -r {relation_id} - {target} --format json"
+            target,
+            model,
+            f"relation-get -r {relation_id} - {target} --format json",
         )
         local_unit_data = json.loads(local_unit_data_raw)
         local_app_data_raw = _juju_exec(
             target,
             model,
             f"relation-get -r {relation_id} - {target} --format json --app",
         )
@@ -552,51 +574,52 @@
         #  if it's a peer relation or a subordinate, we should use the corresponding
         #  scenario.state types instead of a regular Relation.
 
         relations.append(
             Relation(
                 endpoint=raw_relation["endpoint"],
                 interface=_get_interface_from_metadata(
-                    raw_relation["endpoint"], metadata
+                    raw_relation["endpoint"],
+                    metadata,
                 ),
                 relation_id=relation_id,
                 remote_app_data=raw_relation["application-data"],
                 remote_app_name=some_remote_unit_id.app_name,
                 remote_units_data={
                     JujuUnitName(tgt).unit_id: _clean(val["data"])
                     for tgt, val in related_units.items()
                 },
                 local_app_data=local_app_data,
                 local_unit_data=_clean(local_unit_data),
-            )
+            ),
         )
     return relations
 
 
 def get_model(name: str = None) -> Model:
     """Get the Model data structure."""
     logger.info("getting model...")
 
-    jsn = _juju_run("models")
-    model_name = name or jsn["current-model"]
+    json_data = _juju_run("models")
+    model_name = name or json_data["current-model"]
     try:
         model_info = next(
-            filter(lambda m: m["short-name"] == model_name, jsn["models"])
+            filter(lambda m: m["short-name"] == model_name, json_data["models"]),
         )
     except StopIteration as e:
         raise InvalidTargetModelName(name) from e
 
     model_uuid = model_info["model-uuid"]
     model_type = model_info["type"]
 
     return Model(name=model_name, uuid=model_uuid, type=model_type)
 
 
 def try_guess_charm_type_name() -> Optional[str]:
-    """If we are running this from a charm project root, get the charm type name charm.py is using."""
+    """If we are running this from a charm project root, get the charm type name from charm.py."""
     try:
         charm_path = Path(os.getcwd()) / "src" / "charm.py"
         if charm_path.exists():
             source = charm_path.read_text()
             charms = CHARM_SUBCLASS_REGEX.findall(source)
             if len(charms) < 1:
                 raise RuntimeError(f"Not enough charms at {charm_path}.")
@@ -605,15 +628,16 @@
             return charms[0]
     except Exception as e:
         logger.warning(f"unable to guess charm type: {e}")
     return None
 
 
 class FormatOption(
-    str, Enum
+    str,
+    Enum,
 ):  # Enum for typer support, str for native comparison and ==.
     """Output formatting options for snapshot."""
 
     state = "state"  # the default: will print the python repr of the State dataclass.
     json = "json"
     pytest = "pytest"
 
@@ -622,22 +646,22 @@
     """Get juju agent version from juju status output."""
     return juju_status["model"]["version"]
 
 
 def get_charm_version(target: JujuUnitName, juju_status: Dict) -> str:
     """Get charm version info from juju status output."""
     app_info = juju_status["applications"][target.app_name]
-    channel = app_info["charm-channel"]
-    charm_name = app_info["charm-name"]
-    app_version = app_info["version"]
-    charm_rev = app_info["charm-rev"]
-    charm_origin = app_info["charm-origin"]
+    channel = app_info.get("charm-channel", "<local charm>")
+    charm_name = app_info.get("charm-name", "n/a")
+    workload_version = app_info.get("version", "n/a")
+    charm_rev = app_info.get("charm-rev", "n/a")
+    charm_origin = app_info.get("charm-origin", "n/a")
     return (
         f"charm {charm_name!r} ({channel}/{charm_rev}); "
-        f"origin := {charm_origin}; app version := {app_version}."
+        f"origin := {charm_origin}; app version := {workload_version}."
     )
 
 
 class RemoteUnitStateDB(UnitStateDB):
     """Represents a remote unit's state db."""
 
     def __init__(self, model: Optional[str], target: JujuUnitName):
@@ -681,15 +705,15 @@
     """see snapshot's docstring"""
 
     try:
         target = JujuUnitName(target)
     except InvalidTargetUnitName:
         logger.critical(
             f"invalid target: {target!r} is not a valid unit name. Should be formatted like so:"
-            f"`foo/1`, or `database/0`, or `myapp-foo-bar/42`."
+            f"`foo/1`, or `database/0`, or `myapp-foo-bar/42`.",
         )
         sys.exit(1)
 
     logger.info(f'beginning snapshot of {target} in model {model or "<current>"}...')
 
     def if_include(key, fn, default):
         if include is None or key in include:
@@ -778,23 +802,25 @@
         _model = f"model {model}" or "the current model"
         logger.critical(f"invalid target: {target!r} not found in {_model}")
         sys.exit(1)
     except InvalidTargetModelName:
         logger.critical(f"invalid model: {model!r} not found.")
         sys.exit(1)
 
-    logger.info(f"snapshot done.")
+    logger.info("snapshot done.")
 
     if pprint:
         charm_version = get_charm_version(target, juju_status)
         juju_version = get_juju_version(juju_status)
         if format == FormatOption.pytest:
             charm_type_name = try_guess_charm_type_name()
             txt = format_test_case(
-                state, charm_type_name=charm_type_name, juju_version=juju_version
+                state,
+                charm_type_name=charm_type_name,
+                juju_version=juju_version,
             )
         elif format == FormatOption.state:
             txt = format_state(state)
         elif format == FormatOption.json:
             txt = json.dumps(asdict(state), indent=2)
         else:
             raise ValueError(f"unknown format {format}")
@@ -802,34 +828,37 @@
         controller_timestamp = juju_status["controller"]["timestamp"]
         local_timestamp = datetime.datetime.now().strftime("%m/%d/%Y, %H:%M:%S")
         print(
             f"# Generated by scenario.snapshot. \n"
             f"# Snapshot of {state_model.name}:{target.unit_name} at {local_timestamp}. \n"
             f"# Controller timestamp := {controller_timestamp}. \n"
             f"# Juju version := {juju_version} \n"
-            f"# Charm fingerprint := {charm_version} \n"
+            f"# Charm fingerprint := {charm_version} \n",
         )
         print(txt)
 
     return state
 
 
 def snapshot(
     target: str = typer.Argument(..., help="Target unit."),
     model: Optional[str] = typer.Option(
-        None, "-m", "--model", help="Which model to look at."
+        None,
+        "-m",
+        "--model",
+        help="Which model to look at.",
     ),
     format: FormatOption = typer.Option(
         "state",
         "-f",
         "--format",
         help="How to format the output. "
         "``state``: Outputs a black-formatted repr() of the State object (if black is installed! "
-        "else it will be ugly but valid python code). All you need to do then is import the necessary "
-        "objects from scenario.state, and you should have a valid State object."
+        "else it will be ugly but valid python code). All you need to do then is import the "
+        "necessary objects from scenario.state, and you should have a valid State object. "
         "``json``: Outputs a Jsonified State object. Perfect for storage. "
         "``pytest``: Outputs a full-blown pytest scenario test based on this State. "
         "Pipe it to a file and fill in the blanks.",
     ),
     include: str = typer.Option(
         "rckndt",
         "--include",
@@ -903,9 +932,9 @@
             #     "traefik": [
             #         Path("/opt/traefik/juju/certificates.yaml"),
             #         Path("/opt/traefik/juju/certificate.cert"),
             #         Path("/opt/traefik/juju/certificate.key"),
             #         Path("/etc/traefik/traefik.yaml"),
             #     ]
             # },
-        )
+        ),
     )
```

### Comparing `ops-scenario-2.2/scenario/scripts/utils.py` & `ops-scenario-3.0a1/scenario/scripts/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,9 +15,9 @@
         if not app_name or not unit_id:
             raise InvalidTargetUnitName(f"invalid unit name: {unit_name!r}")
         self.unit_name = unit_name
         self.app_name = app_name
         self.unit_id = int(unit_id)
         self.normalized = f"{app_name}-{unit_id}"
         self.remote_charm_root = Path(
-            f"/var/lib/juju/agents/unit-{self.normalized}/charm"
+            f"/var/lib/juju/agents/unit-{self.normalized}/charm",
         )
```

### Comparing `ops-scenario-2.2/scenario/sequences.py` & `ops-scenario-3.0a1/scenario/sequences.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 import typing
 from itertools import chain
 from typing import Any, Callable, Dict, Iterable, Optional, TextIO, Type, Union
 
+from scenario import trigger
 from scenario.logger import logger as scenario_logger
 from scenario.state import (
     ATTACH_ALL_STORAGES,
     BREAK_ALL_RELATIONS,
     CREATE_ALL_RELATIONS,
     DETACH_ALL_STORAGES,
     META_EVENTS,
@@ -33,15 +34,16 @@
         return
 
     if meta_event.name in [CREATE_ALL_RELATIONS, BREAK_ALL_RELATIONS]:
         for relation in state.relations:
             event = Event(
                 relation.endpoint + META_EVENTS[meta_event.name],
                 args=(
-                    # right now, the Relation object hasn't been created by ops yet, so we can't pass it down.
+                    # right now, the Relation object hasn't been created by ops yet, so we
+                    # can't pass it down.
                     # this will be replaced by a Relation instance before the event is fired.
                     InjectRelation(relation.endpoint, relation.relation_id),
                 ),
             )
             logger.debug(f"decomposed meta {meta_event.name}: {event}")
             yield event, state.copy()
 
@@ -55,15 +57,15 @@
         ((Event("start"), state_template.copy()),),
         decompose_meta_event(Event(CREATE_ALL_RELATIONS), state_template.copy()),
         (
             (
                 Event(
                     "leader_elected"
                     if state_template.leader
-                    else "leader_settings_changed"
+                    else "leader_settings_changed",
                 ),
                 state_template.copy(),
             ),
             (Event("config_changed"), state_template.copy()),
             (Event("install"), state_template.copy()),
         ),
     )
@@ -92,15 +94,14 @@
     charm_type: Type["CharmType"],
     meta: Optional[Dict[str, Any]] = None,
     actions: Optional[Dict[str, Any]] = None,
     config: Optional[Dict[str, Any]] = None,
     template_state: State = None,
     pre_event: Optional[Callable[["CharmType"], None]] = None,
     post_event: Optional[Callable[["CharmType"], None]] = None,
-    unit_id: int = 0,
 ):
     """Test that all the builtin startup and teardown events can fire without errors.
 
     This will play both scenarios with and without leadership, and raise any exceptions.
 
     This is a baseline check that in principle all charms (except specific use-cases perhaps),
     should pass out of the box.
@@ -111,19 +112,19 @@
 
     template = template_state if template_state else State()
 
     for event, state in generate_builtin_sequences(
         (
             template.replace(leader=True),
             template.replace(leader=False),
-        )
+        ),
     ):
-        state.trigger(
+        trigger(
+            state,
             event=event,
             charm_type=charm_type,
             meta=meta,
             actions=actions,
             config=config,
             pre_event=pre_event,
             post_event=post_event,
-            unit_id=unit_id,
         )
```

### Comparing `ops-scenario-2.2/scenario/state.py` & `ops-scenario-3.0a1/scenario/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,51 +106,74 @@
 
     # consumer-only events
     @property
     def changed_event(self):
         """Sugar to generate a secret-changed event."""
         if self.owner:
             raise ValueError(
-                "This unit will never receive secret-changed for a secret it owns."
+                "This unit will never receive secret-changed for a secret it owns.",
             )
         return Event(name="secret_changed", secret=self)
 
     # owner-only events
     @property
     def rotate_event(self):
         """Sugar to generate a secret-rotate event."""
         if not self.owner:
             raise ValueError(
-                "This unit will never receive secret-rotate for a secret it does not own."
+                "This unit will never receive secret-rotate for a secret it does not own.",
             )
         return Event(name="secret_rotate", secret=self)
 
     @property
     def expired_event(self):
         """Sugar to generate a secret-expired event."""
         if not self.owner:
             raise ValueError(
-                "This unit will never receive secret-expire for a secret it does not own."
+                "This unit will never receive secret-expire for a secret it does not own.",
             )
         return Event(name="secret_expire", secret=self)
 
     @property
     def remove_event(self):
         """Sugar to generate a secret-remove event."""
         if not self.owner:
             raise ValueError(
-                "This unit will never receive secret-removed for a secret it does not own."
+                "This unit will never receive secret-removed for a secret it does not own.",
             )
         return Event(name="secret_removed", secret=self)
 
     def _set_revision(self, revision: int):
         """Set a new tracked revision."""
         # bypass frozen dataclass
         object.__setattr__(self, "revision", revision)
 
+    def _update_metadata(
+        self,
+        content: Optional[Dict[str, str]] = None,
+        label: Optional[str] = None,
+        description: Optional[str] = None,
+        expire: Optional[datetime.datetime] = None,
+        rotate: Optional[SecretRotate] = None,
+    ):
+        """Update the metadata."""
+        revision = max(self.contents.keys())
+        # bypass frozen dataclass
+        object.__setattr__(self, "contents"[revision + 1], content)
+        if label:
+            object.__setattr__(self, "label", label)
+        if description:
+            object.__setattr__(self, "description", description)
+        if expire:
+            if isinstance(expire, datetime.timedelta):
+                expire = datetime.datetime.now() + expire
+            object.__setattr__(self, "expire", expire)
+        if rotate:
+            object.__setattr__(self, "rotate", rotate)
+
 
 _RELATION_IDS_CTR = 0
 
 
 def normalize_name(s: str):
     """Event names need underscores instead of dashes."""
     return s.replace("-", "_")
@@ -164,29 +187,29 @@
         self._kwargs = kwargs
 
     def __call__(self, remote_unit: Optional[str] = None) -> "Event":
         """Construct an Event object using the arguments provided at init and any extra params."""
         if remote_unit and "remote_unit" not in self._accept_params:
             raise ValueError(
                 f"cannot pass param `remote_unit` to a "
-                f"{self._category} event constructor."
+                f"{self._category} event constructor.",
             )
 
         return Event(*self._args, *self._kwargs, relation_remote_unit_id=remote_unit)
 
     def deferred(self, handler: Callable, event_id: int = 1) -> "DeferredEvent":
         return self().deferred(handler=handler, event_id=event_id)
 
 
 def _generate_new_relation_id():
     global _RELATION_IDS_CTR
     _RELATION_IDS_CTR += 1
     logger.info(
         f"relation ID unset; automatically assigning {_RELATION_IDS_CTR}. "
-        f"If there are problems, pass one manually."
+        f"If there are problems, pass one manually.",
     )
     return _RELATION_IDS_CTR
 
 
 @dataclasses.dataclass(frozen=True)
 class RelationBase(_DCBase):
     endpoint: str
@@ -212,73 +235,78 @@
         raise NotImplementedError()
 
     @property
     def _remote_unit_ids(self) -> Tuple[int]:
         """Ids of the units on the other end of this relation."""
         raise NotImplementedError()
 
-    def _get_databag_for_remote(self, unit_id: int) -> Dict[str, str]:
+    def _get_databag_for_remote(self, unit_id: int) -> Dict[str, str]:  # noqa: U100
         """Return the databag for some remote unit ID."""
         raise NotImplementedError()
 
     def __post_init__(self):
         if type(self) is RelationBase:
             raise RuntimeError(
                 "RelationBase cannot be instantiated directly; "
-                "please use Relation, PeerRelation, or SubordinateRelation"
+                "please use Relation, PeerRelation, or SubordinateRelation",
             )
 
         for databag in self._databags:
             self._validate_databag(databag)
 
     def _validate_databag(self, databag: dict):
         if not isinstance(databag, dict):
             raise StateValidationError(
-                f"all databags should be dicts, not {type(databag)}"
+                f"all databags should be dicts, not {type(databag)}",
             )
-        for k, v in databag.items():
+        for v in databag.values():
             if not isinstance(v, str):
                 raise StateValidationError(
                     f"all databags should be Dict[str,str]; "
-                    f"found a value of type {type(v)}"
+                    f"found a value of type {type(v)}",
                 )
 
     @property
     def changed_event(self) -> "Event":
         """Sugar to generate a <this relation>-relation-changed event."""
         return Event(
-            name=normalize_name(self.endpoint + "-relation-changed"), relation=self
+            name=normalize_name(self.endpoint + "-relation-changed"),
+            relation=self,
         )
 
     @property
     def joined_event(self) -> "Event":
         """Sugar to generate a <this relation>-relation-joined event."""
         return Event(
-            name=normalize_name(self.endpoint + "-relation-joined"), relation=self
+            name=normalize_name(self.endpoint + "-relation-joined"),
+            relation=self,
         )
 
     @property
     def created_event(self) -> "Event":
         """Sugar to generate a <this relation>-relation-created event."""
         return Event(
-            name=normalize_name(self.endpoint + "-relation-created"), relation=self
+            name=normalize_name(self.endpoint + "-relation-created"),
+            relation=self,
         )
 
     @property
     def departed_event(self) -> "Event":
         """Sugar to generate a <this relation>-relation-departed event."""
         return Event(
-            name=normalize_name(self.endpoint + "-relation-departed"), relation=self
+            name=normalize_name(self.endpoint + "-relation-departed"),
+            relation=self,
         )
 
     @property
     def broken_event(self) -> "Event":
         """Sugar to generate a <this relation>-relation-broken event."""
         return Event(
-            name=normalize_name(self.endpoint + "-relation-broken"), relation=self
+            name=normalize_name(self.endpoint + "-relation-broken"),
+            relation=self,
         )
 
 
 def unify_ids_and_remote_units_data(ids: List[int], data: Dict[int, Any]):
     """Unify and validate a list of unit IDs and a mapping from said ids to databag contents.
 
     This allows the user to pass equivalently:
@@ -304,20 +332,20 @@
 
     ids = [2]
     data = {1: {}}
     """
     if ids and data:
         if not set(ids) == set(data):
             raise StateValidationError(
-                f"{ids} should include any and all IDs from {data}"
+                f"{ids} should include any and all IDs from {data}",
             )
     elif ids:
         data = {x: {} for x in ids}
     elif data:
-        ids = [x for x in data]
+        ids = list(data)
     else:
         ids = [0]
         data = {0: {}}
     return ids, data
 
 
 @dataclasses.dataclass(frozen=True)
@@ -328,22 +356,23 @@
     remote_unit_ids: List[int] = dataclasses.field(default_factory=list)
 
     # local limit
     limit: int = 1
 
     remote_app_data: Dict[str, str] = dataclasses.field(default_factory=dict)
     remote_units_data: Dict[int, Dict[str, str]] = dataclasses.field(
-        default_factory=dict
+        default_factory=dict,
     )
 
     def __post_init__(self):
         super().__post_init__()
 
         remote_unit_ids, remote_units_data = unify_ids_and_remote_units_data(
-            self.remote_unit_ids, self.remote_units_data
+            self.remote_unit_ids,
+            self.remote_units_data,
         )
         # bypass frozen dataclass
         object.__setattr__(self, "remote_unit_ids", remote_unit_ids)
         object.__setattr__(self, "remote_units_data", remote_units_data)
 
     @property
     def _remote_app_name(self) -> str:
@@ -384,15 +413,15 @@
         return self.primary_app_name
 
     @property
     def _remote_unit_ids(self) -> Tuple[int]:
         """Ids of the units on the other end of this relation."""
         return (self.primary_id,)
 
-    def _get_databag_for_remote(self, unit_id: int) -> Dict[str, str]:
+    def _get_databag_for_remote(self, unit_id: int) -> Dict[str, str]:  # noqa: U100
         """Return the databag for some remote unit ID."""
         return self.remote_unit_data
 
     @property
     def _databags(self):
         """Yield all databags in this relation."""
         yield self.local_app_data
@@ -432,15 +461,16 @@
 
     def _get_databag_for_remote(self, unit_id: int) -> Dict[str, str]:
         """Return the databag for some remote unit ID."""
         return self.peers_data[unit_id]
 
     def __post_init__(self):
         peers_ids, peers_data = unify_ids_and_remote_units_data(
-            self.peers_ids, self.peers_data
+            self.peers_ids,
+            self.peers_data,
         )
         # bypass frozen dataclass guards
         object.__setattr__(self, "peers_ids", peers_ids)
         object.__setattr__(self, "peers_data", peers_data)
 
 
 def _random_model_name():
@@ -469,15 +499,15 @@
 
 
 def _generate_new_change_id():
     global _CHANGE_IDS
     _CHANGE_IDS += 1
     logger.info(
         f"change ID unset; automatically assigning {_CHANGE_IDS}. "
-        f"If there are problems, pass one manually."
+        f"If there are problems, pass one manually.",
     )
     return _CHANGE_IDS
 
 
 @dataclasses.dataclass(frozen=True)
 class ExecOutput:
     return_code: int = 0
@@ -502,25 +532,25 @@
 
 @dataclasses.dataclass(frozen=True)
 class Container(_DCBase):
     name: str
     can_connect: bool = False
 
     # This is the base plan. On top of it, one can add layers.
-    # We need to model pebble in this way because it's impossible to retrieve the layers from pebble
-    # or derive them from the resulting plan (which one CAN get from pebble).
-    # So if we are instantiating Container by fetching info from a 'live' charm, the 'layers' will be unknown.
-    # all that we can know is the resulting plan (the 'computed plan').
+    # We need to model pebble in this way because it's impossible to retrieve the layers from
+    # pebble or derive them from the resulting plan (which one CAN get from pebble).
+    # So if we are instantiating Container by fetching info from a 'live' charm, the 'layers'
+    # will be unknown. all that we can know is the resulting plan (the 'computed plan').
     _base_plan: dict = dataclasses.field(default_factory=dict)
     # We expect most of the user-facing testing to be covered by this 'layers' attribute,
     # as all will be known when unit-testing.
     layers: Dict[str, pebble.Layer] = dataclasses.field(default_factory=dict)
 
     service_status: Dict[str, pebble.ServiceStatus] = dataclasses.field(
-        default_factory=dict
+        default_factory=dict,
     )
 
     # this is how you specify the contents of the filesystem: suppose you want to express that your
     # container has:
     # - /home/foo/bar.py
     # - /bin/bash
     # - /bin/baz
@@ -544,30 +574,33 @@
             layer = self.layers[key]
             for name, service in layer.services.items():
                 services[name] = service
         return services
 
     @property
     def plan(self) -> pebble.Plan:
-        """This is the 'computed' pebble plan; i.e. the base plan plus the layers that have been added on top.
+        """The 'computed' pebble plan.
 
-        You should run your assertions on the plan, not so much on the layers, as those are input data.
+        i.e. the base plan plus the layers that have been added on top.
+        You should run your assertions on this plan, not so much on the layers, as those are
+        input data.
         """
 
         # copied over from ops.testing._TestingPebbleClient.get_plan().
         plan = pebble.Plan(yaml.safe_dump(self._base_plan))
         services = self._render_services()
         if not services:
             return plan
         for name in sorted(services.keys()):
             plan.services[name] = services[name]
         return plan
 
     @property
     def services(self) -> Dict[str, pebble.ServiceInfo]:
+        """The pebble services as rendered in the plan."""
         services = self._render_services()
         infos = {}  # type: Dict[str, pebble.ServiceInfo]
         names = sorted(services.keys())
         for name in names:
             try:
                 service = services[name]
             except KeyError:
@@ -576,36 +609,40 @@
                 continue
             status = self.service_status.get(name, pebble.ServiceStatus.INACTIVE)
             if service.startup == "":
                 startup = pebble.ServiceStartup.DISABLED
             else:
                 startup = pebble.ServiceStartup(service.startup)
             info = pebble.ServiceInfo(
-                name, startup=startup, current=pebble.ServiceStatus(status)
+                name,
+                startup=startup,
+                current=pebble.ServiceStatus(status),
             )
             infos[name] = info
         return infos
 
     @property
     def filesystem(self) -> "_MockFileSystem":
+        """Simulated pebble filesystem."""
         mounts = {
             name: _MockStorageMount(
-                src=Path(spec.src), location=PurePosixPath(spec.location)
+                src=Path(spec.src),
+                location=PurePosixPath(spec.location),
             )
             for name, spec in self.mounts.items()
         }
         return _MockFileSystem(mounts=mounts)
 
     @property
     def pebble_ready_event(self):
         """Sugar to generate a <this container's name>-pebble-ready event."""
         if not self.can_connect:
             logger.warning(
                 "you **can** fire pebble-ready while the container cannot connect, "
-                "but that's most likely not what you want."
+                "but that's most likely not what you want.",
             )
         return Event(name=normalize_name(self.name + "-pebble-ready"), container=self)
 
 
 @dataclasses.dataclass(frozen=True)
 class Address(_DCBase):
     hostname: str
@@ -664,17 +701,17 @@
         return cls(
             name=name,
             bind_addresses=[
                 BindAddress(
                     interface_name=interface_name,
                     mac_address=mac_address,
                     addresses=[
-                        Address(hostname=hostname, value=private_address, cidr=cidr)
+                        Address(hostname=hostname, value=private_address, cidr=cidr),
                     ],
-                )
+                ),
             ],
             egress_subnets=list(egress_subnets),
             ingress_addresses=list(ingress_addresses),
         )
 
 
 @dataclasses.dataclass(frozen=True)
@@ -685,22 +722,22 @@
 
     name: Literal["waiting", "blocked", "active", "unknown", "error", "maintenance"]
     message: str = ""
 
     def __eq__(self, other):
         if isinstance(other, Tuple):
             logger.warning(
-                "Comparing Status with Tuples is deprecated and will be removed soon."
+                "Comparing Status with Tuples is deprecated and will be removed soon.",
             )
             return (self.name, self.message) == other
         if isinstance(other, StatusBase):
             return (self.name, self.message) == (other.name, other.message)
         logger.warning(
             f"Comparing Status with {other} is not stable and will be forbidden soon."
-            f"Please compare with StatusBase directly."
+            f"Please compare with StatusBase directly.",
         )
         return super().__eq__(other)
 
     def __iter__(self):
         return iter([self.name, self.message])
 
     def __repr__(self):
@@ -716,49 +753,52 @@
 @dataclasses.dataclass(frozen=True)
 class Status(_DCBase):
     """Represents the 'juju statuses' of the application/unit being tested."""
 
     # the current statuses. Will be cast to _EntitiyStatus in __post_init__
     app: Union[StatusBase, _EntityStatus] = _EntityStatus("unknown")
     unit: Union[StatusBase, _EntityStatus] = _EntityStatus("unknown")
-    app_version: str = ""
+    workload_version: str = ""
 
     # most to least recent statuses; do NOT include the current one.
     app_history: List[_EntityStatus] = dataclasses.field(default_factory=list)
     unit_history: List[_EntityStatus] = dataclasses.field(default_factory=list)
-    previous_app_version: Optional[str] = None
+    previous_workload_version: Optional[str] = None
 
     def __post_init__(self):
         for name in ["app", "unit"]:
             val = getattr(self, name)
             if isinstance(val, _EntityStatus):
                 pass
             elif isinstance(val, StatusBase):
                 object.__setattr__(self, name, _status_to_entitystatus(val))
             elif isinstance(val, tuple):
                 logger.warning(
                     "Initializing Status.[app/unit] with Tuple[str, str] is deprecated "
                     "and will be removed soon. \n"
-                    f"Please pass a StatusBase instance: `StatusBase(*{val})`"
+                    f"Please pass a StatusBase instance: `StatusBase(*{val})`",
                 )
                 object.__setattr__(self, name, _EntityStatus(*val))
             else:
                 raise TypeError(f"Invalid status.{name}: {val!r}")
 
-    def _update_app_version(self, new_app_version: str):
+    def _update_workload_version(self, new_workload_version: str):
         """Update the current app version and record the previous one."""
         # We don't keep a full history because we don't expect the app version to change more
         # than once per hook.
 
         # bypass frozen dataclass
-        object.__setattr__(self, "previous_app_version", self.app_version)
-        object.__setattr__(self, "app_version", new_app_version)
+        object.__setattr__(self, "previous_workload_version", self.workload_version)
+        object.__setattr__(self, "workload_version", new_workload_version)
 
     def _update_status(
-        self, new_status: str, new_message: str = "", is_app: bool = False
+        self,
+        new_status: str,
+        new_message: str = "",
+        is_app: bool = False,
     ):
         """Update the current app/unit status and add the previous one to the history."""
         if is_app:
             self.app_history.append(self.app)
             # bypass frozen dataclass
             object.__setattr__(self, "app", _EntityStatus(new_status, new_message))
         else:
@@ -783,33 +823,34 @@
         return f"{self.owner_path or ''}/{self.data_type_name}[{self.name}]"
 
 
 @dataclasses.dataclass(frozen=True)
 class State(_DCBase):
     """Represents the juju-owned portion of a unit's state.
 
-    Roughly speaking, it wraps all hook-tool- and pebble-mediated data a charm can access in its lifecycle.
-    For example, status-get will return data from `State.status`, is-leader will return data from
-    `State.leader`, and so on.
+    Roughly speaking, it wraps all hook-tool- and pebble-mediated data a charm can access in its
+    lifecycle. For example, status-get will return data from `State.status`, is-leader will
+    return data from `State.leader`, and so on.
     """
 
     config: Dict[str, Union[str, int, float, bool]] = dataclasses.field(
-        default_factory=dict
+        default_factory=dict,
     )
     relations: List["AnyRelation"] = dataclasses.field(default_factory=list)
     networks: List[Network] = dataclasses.field(default_factory=list)
     containers: List[Container] = dataclasses.field(default_factory=list)
     status: Status = dataclasses.field(default_factory=Status)
     leader: bool = False
     model: Model = Model()
     juju_log: List[Tuple[str, str]] = dataclasses.field(default_factory=list)
     secrets: List[Secret] = dataclasses.field(default_factory=list)
 
-    # represents the OF's event queue. These events will be emitted before the event being dispatched,
-    # and represent the events that had been deferred during the previous run.
+    unit_id: int = 0
+    # represents the OF's event queue. These events will be emitted before the event being
+    # dispatched, and represent the events that had been deferred during the previous run.
     # If the charm defers any events during "this execution", they will be appended
     # to this list.
     deferred: List["DeferredEvent"] = dataclasses.field(default_factory=list)
     stored_state: List["StoredState"] = dataclasses.field(default_factory=dict)
 
     # todo:
     #  actions?
@@ -825,16 +866,17 @@
 
     def with_leadership(self, leader: bool) -> "State":
         return self.replace(leader=leader)
 
     def with_unit_status(self, status: StatusBase) -> "State":
         return self.replace(
             status=dataclasses.replace(
-                self.status, unit=_status_to_entitystatus(status)
-            )
+                self.status,
+                unit=_status_to_entitystatus(status),
+            ),
         )
 
     def get_container(self, container: Union[str, Container]) -> Container:
         """Get container from this State, based on an input container or its name."""
         name = container.name if isinstance(container, Container) else container
         try:
             return next(filter(lambda c: c.name == name, self.containers))
@@ -852,66 +894,35 @@
     def jsonpatch_delta(self, other: "State"):
         try:
             import jsonpatch
         except ModuleNotFoundError:
             logger.error(
                 "cannot import jsonpatch: using the .delta() "
                 "extension requires jsonpatch to be installed."
-                "Fetch it with pip install jsonpatch."
+                "Fetch it with pip install jsonpatch.",
             )
             return NotImplemented
         patch = jsonpatch.make_patch(
-            dataclasses.asdict(other), dataclasses.asdict(self)
+            dataclasses.asdict(other),
+            dataclasses.asdict(self),
         ).patch
         return sort_patch(patch)
 
-    def trigger(
-        self,
-        event: Union["Event", str],
-        charm_type: Type["CharmType"],
-        # callbacks
-        pre_event: Optional[Callable[["CharmType"], None]] = None,
-        post_event: Optional[Callable[["CharmType"], None]] = None,
-        # if not provided, will be autoloaded from charm_type.
-        meta: Optional[Dict[str, Any]] = None,
-        actions: Optional[Dict[str, Any]] = None,
-        config: Optional[Dict[str, Any]] = None,
-        charm_root: Optional["PathLike"] = None,
-        juju_version: str = "3.0",
-        unit_id: int = 0,
-    ) -> "State":
-        """Fluent API for trigger. See runtime.trigger's docstring."""
-        from scenario.runtime import trigger as _runtime_trigger
-
-        return _runtime_trigger(
-            state=self,
-            event=event,
-            charm_type=charm_type,
-            pre_event=pre_event,
-            post_event=post_event,
-            meta=meta,
-            actions=actions,
-            config=config,
-            charm_root=charm_root,
-            juju_version=juju_version,
-            unit_id=unit_id,
-        )
-
 
 @dataclasses.dataclass(frozen=True)
 class _CharmSpec(_DCBase):
     """Charm spec."""
 
     charm_type: Type["CharmType"]
     meta: Optional[Dict[str, Any]]
     actions: Optional[Dict[str, Any]] = None
     config: Optional[Dict[str, Any]] = None
 
-    # autoloaded means: trigger() is being invoked on a 'real' charm class, living in some /src/charm.py,
-    # and the metadata files are 'real' metadata files.
+    # autoloaded means: trigger() is being invoked on a 'real' charm class, living in some
+    # /src/charm.py, and the metadata files are 'real' metadata files.
     is_autoloaded: bool = False
 
     @staticmethod
     def autoload(charm_type: Type["CharmType"]):
         charm_source_path = Path(inspect.getfile(charm_type))
         charm_root = charm_source_path.parent.parent
 
@@ -977,15 +988,15 @@
     #  - pebble?
     #  - action?
 
     def __call__(self, remote_unit_id: Optional[int] = None) -> "Event":
         if remote_unit_id and not self._is_relation_event:
             raise ValueError(
                 "cannot pass param `remote_unit_id` to a "
-                "non-relation event constructor."
+                "non-relation event constructor.",
             )
         return self.replace(relation_remote_unit_id=remote_unit_id)
 
     def __post_init__(self):
         if "-" in self.name:
             logger.warning(f"Only use underscores in event names. {self.name!r}")
 
@@ -1008,31 +1019,33 @@
         return any(self.name.endswith(suffix) for suffix in STORAGE_EVENTS_SUFFIX)
 
     @property
     def _is_workload_event(self) -> bool:
         """Whether the event name indicates that this is a workload event."""
         return self.name.endswith("_pebble_ready")
 
-    # this method is private because _CharmSpec is not quite user-facing; also, the user should know.
+    # this method is private because _CharmSpec is not quite user-facing; also,
+    # the user should know.
     def _is_builtin_event(self, charm_spec: "_CharmSpec"):
         """Determine whether the event is a custom-defined one or a builtin one."""
-        evt_name = self.name
+        event_name = self.name
 
         # simple case: this is an event type owned by our charm base.on
-        if hasattr(charm_spec.charm_type.on, evt_name):
-            return hasattr(CharmEvents, evt_name)
+        if hasattr(charm_spec.charm_type.on, event_name):
+            return hasattr(CharmEvents, event_name)
 
         # this could be an event defined on some other Object, e.g. a charm lib.
-        # We don't support (yet) directly emitting those, but they COULD have names that conflict with
-        # events owned by the base charm. E.g. if the charm has a `foo` relation, the charm will get a
-        # charm.on.foo_relation_created. Your charm lib is free to define its own `foo_relation_created`
-        # custom event, because its handle will be `charm.lib.on.foo_relation_created` and therefore be
-        # unique and the Framework is happy. However, our Event data structure ATM has no knowledge
-        # of which Object/Handle it is owned by. So the only thing we can do right now is: check whether
-        # the event name, assuming it is owned by the charm, is that of a builtin event or not.
+        # We don't support (yet) directly emitting those, but they COULD have names that conflict
+        # with events owned by the base charm. E.g. if the charm has a `foo` relation, the charm
+        # will get a  charm.on.foo_relation_created. Your charm lib is free to define its own
+        # `foo_relation_created`  custom event, because its handle will be
+        # `charm.lib.on.foo_relation_created` and therefore be  unique and the Framework is happy.
+        # However, our Event data structure ATM has no knowledge of which Object/Handle it is
+        # owned by. So the only thing we can do right now is: check whether the event name,
+        # assuming it is owned by the charm, is that of a builtin event or not.
         builtins = []
         for relation_name in chain(
             charm_spec.meta.get("requires", ()),
             charm_spec.meta.get("provides", ()),
             charm_spec.meta.get("peers", ()),
         ):
             relation_name = relation_name.replace("-", "_")
@@ -1051,43 +1064,43 @@
             action_name = action_name.replace("-", "_")
             builtins.append(action_name + "_action")
 
         for container_name in charm_spec.meta.get("containers", ()):
             container_name = container_name.replace("-", "_")
             builtins.append(container_name + "_pebble_ready")
 
-        return evt_name in builtins
+        return event_name in builtins
 
     def deferred(self, handler: Callable, event_id: int = 1) -> DeferredEvent:
         """Construct a DeferredEvent from this Event."""
         handler_repr = repr(handler)
         handler_re = re.compile(r"<function (.*) at .*>")
         match = handler_re.match(handler_repr)
         if not match:
             raise ValueError(
-                f"cannot construct DeferredEvent from {handler}; please create one manually."
+                f"cannot construct DeferredEvent from {handler}; please create one manually.",
             )
         owner_name, handler_name = match.groups()[0].split(".")[-2:]
         handle_path = f"{owner_name}/on/{self.name}[{event_id}]"
 
         snapshot_data = {}
 
-        # fixme: at this stage we can't determine if the event is a builtin one or not; if it is not,
-        #  then the coming checks are meaningless: the custom event could be named like a relation event but
-        #  not *be* one.
+        # fixme: at this stage we can't determine if the event is a builtin one or not; if it is
+        #  not, then the coming checks are meaningless: the custom event could be named like a
+        #  relation event but not *be* one.
         if self._is_workload_event:
             # this is a WorkloadEvent. The snapshot:
             snapshot_data = {
                 "container_name": self.container.name,
             }
 
         elif self._is_relation_event:
             if not self.relation:
                 raise ValueError(
-                    "this is a relation event; expected relation attribute"
+                    "this is a relation event; expected relation attribute",
                 )
             # this is a RelationEvent. The snapshot:
             snapshot_data = {
                 "relation_name": self.relation.endpoint,
                 "relation_id": self.relation.relation_id,
                 "app_name": self.relation.remote_app_name,
                 "unit_name": f"{self.relation.remote_app_name}/{self.relation_remote_unit_id}",
@@ -1126,15 +1139,15 @@
     relation_name: str
     relation_id: Optional[int] = None
 
 
 def _derive_args(event_name: str):
     args = []
     for term in RELATION_EVENTS_SUFFIX:
-        # fixme: we can't disambiguate between relation IDs.
+        # fixme: we can't disambiguate between relation id-s.
         if event_name.endswith(term):
             args.append(InjectRelation(relation_name=event_name[: -len(term)]))
 
     return tuple(args)
 
 
 # todo: consider
```

### Comparing `ops-scenario-2.2/tests/test_consistency_checker.py` & `ops-scenario-3.0a1/tests/test_consistency_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,28 @@
 
 
 class MyCharm(CharmBase):
     pass
 
 
 def assert_inconsistent(
-    state: "State", event: "Event", charm_spec: "_CharmSpec", juju_version="3.0"
+    state: "State",
+    event: "Event",
+    charm_spec: "_CharmSpec",
+    juju_version="3.0",
 ):
     with pytest.raises(InconsistentScenarioError):
         check_consistency(state, event, charm_spec, juju_version)
 
 
 def assert_consistent(
-    state: "State", event: "Event", charm_spec: "_CharmSpec", juju_version="3.0"
+    state: "State",
+    event: "Event",
+    charm_spec: "_CharmSpec",
+    juju_version="3.0",
 ):
     check_consistency(state, event, charm_spec, juju_version)
 
 
 def test_base():
     state = State()
     event = Event("update_status")
@@ -64,15 +70,17 @@
         Event("foo"),
         _CharmSpec(MyCharm, {"containers": {"bar": {}}}),
     )
 
 
 def test_container_in_state_but_no_container_in_meta():
     assert_inconsistent(
-        State(containers=[Container("bar")]), Event("foo"), _CharmSpec(MyCharm, {})
+        State(containers=[Container("bar")]),
+        Event("foo"),
+        _CharmSpec(MyCharm, {}),
     )
     assert_consistent(
         State(containers=[Container("bar")]),
         Event("foo"),
         _CharmSpec(MyCharm, {"containers": {"bar": {}}}),
     )
 
@@ -112,15 +120,17 @@
         Event(f"bar{suffix}", relation=Relation("bar")),
         _CharmSpec(MyCharm, {"requires": {"bar": {"interface": "xxx"}}}),
     )
 
 
 def test_config_key_missing_from_meta():
     assert_inconsistent(
-        State(config={"foo": True}), Event("bar"), _CharmSpec(MyCharm, {})
+        State(config={"foo": True}),
+        Event("bar"),
+        _CharmSpec(MyCharm, {}),
     )
     assert_consistent(
         State(config={"foo": True}),
         Event("bar"),
         _CharmSpec(MyCharm, {}, config={"options": {"foo": {"type": "boolean"}}}),
     )
 
@@ -172,22 +182,24 @@
 
 
 def test_sub_relation_consistency():
     assert_inconsistent(
         State(relations=[Relation("foo")]),
         Event("bar"),
         _CharmSpec(
-            MyCharm, {"requires": {"foo": {"interface": "bar", "scope": "container"}}}
+            MyCharm,
+            {"requires": {"foo": {"interface": "bar", "scope": "container"}}},
         ),
     )
     assert_consistent(
         State(relations=[SubordinateRelation("foo")]),
         Event("bar"),
         _CharmSpec(
-            MyCharm, {"requires": {"foo": {"interface": "bar", "scope": "container"}}}
+            MyCharm,
+            {"requires": {"foo": {"interface": "bar", "scope": "container"}}},
         ),
     )
 
 
 def test_relation_sub_inconsistent():
     assert_inconsistent(
         State(relations=[SubordinateRelation("foo")]),
```

### Comparing `ops-scenario-2.2/tests/test_e2e/test_builtin_scenes.py` & `ops-scenario-3.0a1/tests/test_e2e/test_builtin_scenes.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.2/tests/test_e2e/test_config.py` & `ops-scenario-3.0a1/tests/test_e2e/test_config.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.2/tests/test_e2e/test_custom_event_triggers.py` & `ops-scenario-3.0a1/tests/test_e2e/test_custom_event_triggers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import pytest
 from ops.charm import CharmBase, CharmEvents
 from ops.framework import EventBase, EventSource
 
 from scenario import State
-from scenario.runtime import InconsistentScenarioError
+from scenario.runtime import InconsistentScenarioError, trigger
 
 
 def test_custom_event_emitted():
     class FooEvent(EventBase):
         pass
 
     class MyCharmEvents(CharmEvents):
@@ -27,18 +27,18 @@
 
         def _on_foo(self, e):
             MyCharm._foo_called += 1
 
         def _on_start(self, e):
             self.on.foo.emit()
 
-    State().trigger("foo", MyCharm, meta=MyCharm.META)
+    trigger(State(), "foo", MyCharm, meta=MyCharm.META)
     assert MyCharm._foo_called == 1
 
-    State().trigger("start", MyCharm, meta=MyCharm.META)
+    trigger(State(), "start", MyCharm, meta=MyCharm.META)
     assert MyCharm._foo_called == 2
 
 
 def test_funky_named_event_emitted():
     class FooRelationChangedEvent(EventBase):
         pass
 
@@ -55,15 +55,15 @@
             self.framework.observe(self.on.foo_relation_changed, self._on_foo)
 
         def _on_foo(self, e):
             MyCharm._foo_called = True
 
     # we called our custom event like a builtin one. Trouble!
     with pytest.raises(InconsistentScenarioError):
-        State().trigger("foo-relation-changed", MyCharm, meta=MyCharm.META)
+        trigger(State(), "foo-relation-changed", MyCharm, meta=MyCharm.META)
 
     assert not MyCharm._foo_called
 
     os.environ["SCENARIO_SKIP_CONSISTENCY_CHECKS"] = "1"
-    State().trigger("foo-relation-changed", MyCharm, meta=MyCharm.META)
+    trigger(State(), "foo-relation-changed", MyCharm, meta=MyCharm.META)
     assert MyCharm._foo_called
     os.unsetenv("SCENARIO_SKIP_CONSISTENCY_CHECKS")
```

### Comparing `ops-scenario-2.2/tests/test_e2e/test_deferred.py` & `ops-scenario-3.0a1/tests/test_e2e/test_deferred.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     RelationChangedEvent,
     StartEvent,
     UpdateStatusEvent,
     WorkloadEvent,
 )
 from ops.framework import Framework
 
+from scenario import trigger
 from scenario.state import Container, DeferredEvent, Relation, State, deferred
 
 CHARM_CALLED = 0
 
 
 @pytest.fixture(scope="function")
 def mycharm():
@@ -38,25 +39,28 @@
                 return event.defer()
 
     return MyCharm
 
 
 def test_defer(mycharm):
     mycharm.defer_next = True
-    out = State().trigger("start", mycharm, meta=mycharm.META)
+    out = trigger(State(), "start", mycharm, meta=mycharm.META)
     assert len(out.deferred) == 1
     assert out.deferred[0].name == "start"
 
 
 def test_deferred_evt_emitted(mycharm):
     mycharm.defer_next = 2
 
-    out = State(
-        deferred=[deferred(event="update_status", handler=mycharm._on_event)]
-    ).trigger("start", mycharm, meta=mycharm.META)
+    out = trigger(
+        State(deferred=[deferred(event="update_status", handler=mycharm._on_event)]),
+        "start",
+        mycharm,
+        meta=mycharm.META,
+    )
 
     # we deferred the first 2 events we saw: update-status, start.
     assert len(out.deferred) == 2
     assert out.deferred[0].name == "start"
     assert out.deferred[1].name == "update_status"
 
     # we saw start and update-status.
@@ -71,15 +75,17 @@
         deferred(event="foo_relation_changed", handler=mycharm._on_event)
 
 
 def test_deferred_relation_evt(mycharm):
     rel = Relation(endpoint="foo", remote_app_name="remote")
     evt1 = rel.changed_event.deferred(handler=mycharm._on_event)
     evt2 = deferred(
-        event="foo_relation_changed", handler=mycharm._on_event, relation=rel
+        event="foo_relation_changed",
+        handler=mycharm._on_event,
+        relation=rel,
     )
 
     assert asdict(evt2) == asdict(evt1)
 
 
 def test_deferred_workload_evt(mycharm):
     ctr = Container("foo")
@@ -90,22 +96,29 @@
 
 
 def test_deferred_relation_event(mycharm):
     mycharm.defer_next = 2
 
     rel = Relation(endpoint="foo", remote_app_name="remote")
 
-    out = State(
-        relations=[rel],
-        deferred=[
-            deferred(
-                event="foo_relation_changed", handler=mycharm._on_event, relation=rel
-            )
-        ],
-    ).trigger("start", mycharm, meta=mycharm.META)
+    out = trigger(
+        State(
+            relations=[rel],
+            deferred=[
+                deferred(
+                    event="foo_relation_changed",
+                    handler=mycharm._on_event,
+                    relation=rel,
+                )
+            ],
+        ),
+        "start",
+        mycharm,
+        meta=mycharm.META,
+    )
 
     # we deferred the first 2 events we saw: relation-changed, start.
     assert len(out.deferred) == 2
     assert out.deferred[0].name == "foo_relation_changed"
     assert out.deferred[1].name == "start"
 
     # we saw start and relation-changed.
@@ -114,18 +127,23 @@
     assert isinstance(upstat, RelationChangedEvent)
     assert isinstance(start, StartEvent)
 
 
 def test_deferred_relation_event_from_relation(mycharm):
     mycharm.defer_next = 2
     rel = Relation(endpoint="foo", remote_app_name="remote")
-    out = State(
-        relations=[rel],
-        deferred=[rel.changed_event.deferred(handler=mycharm._on_event)],
-    ).trigger("start", mycharm, meta=mycharm.META)
+    out = trigger(
+        State(
+            relations=[rel],
+            deferred=[rel.changed_event.deferred(handler=mycharm._on_event)],
+        ),
+        "start",
+        mycharm,
+        meta=mycharm.META,
+    )
 
     # we deferred the first 2 events we saw: foo_relation_changed, start.
     assert len(out.deferred) == 2
     assert out.deferred[0].name == "foo_relation_changed"
     assert out.deferred[1].name == "start"
 
     # we saw start and foo_relation_changed.
@@ -136,18 +154,23 @@
 
 
 def test_deferred_workload_event(mycharm):
     mycharm.defer_next = 2
 
     ctr = Container("foo")
 
-    out = State(
-        containers=[ctr],
-        deferred=[ctr.pebble_ready_event.deferred(handler=mycharm._on_event)],
-    ).trigger("start", mycharm, meta=mycharm.META)
+    out = trigger(
+        State(
+            containers=[ctr],
+            deferred=[ctr.pebble_ready_event.deferred(handler=mycharm._on_event)],
+        ),
+        "start",
+        mycharm,
+        meta=mycharm.META,
+    )
 
     # we deferred the first 2 events we saw: foo_pebble_ready, start.
     assert len(out.deferred) == 2
     assert out.deferred[0].name == "foo_pebble_ready"
     assert out.deferred[1].name == "start"
 
     # we saw start and foo_pebble_ready.
```

### Comparing `ops-scenario-2.2/tests/test_e2e/test_juju_log.py` & `ops-scenario-3.0a1/tests/test_e2e/test_juju_log.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 
 import pytest
 from ops.charm import CharmBase
 
+from scenario import trigger
 from scenario.state import State
 
 logger = logging.getLogger("testing logger")
 
 
 @pytest.fixture(scope="function")
 def mycharm():
@@ -22,11 +23,11 @@
             print("foo!")
             logger.warning("bar!")
 
     return MyCharm
 
 
 def test_juju_log(mycharm):
-    out = State().trigger("start", mycharm, meta=mycharm.META)
+    out = trigger(State(), "start", mycharm, meta=mycharm.META)
     assert out.juju_log[16] == ("DEBUG", "Emitting Juju event start.")
     # prints are not juju-logged.
     assert out.juju_log[17] == ("WARNING", "bar!")
```

### Comparing `ops-scenario-2.2/tests/test_e2e/test_network.py` & `ops-scenario-3.0a1/tests/test_e2e/test_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         State(
             relations=[
                 Relation(
                     interface="foo",
                     remote_app_name="remote",
                     endpoint="metrics-endpoint",
                     relation_id=1,
-                )
+                ),
             ],
             networks=[Network.default("metrics-endpoint")],
         ),
         "update_status",
         mycharm,
         meta={
             "name": "foo",
```

### Comparing `ops-scenario-2.2/tests/test_e2e/test_pebble.py` & `ops-scenario-3.0a1/tests/test_e2e/test_pebble.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pytest
 import yaml
 from ops import pebble
 from ops.charm import CharmBase
 from ops.framework import Framework
 from ops.pebble import ServiceStartup, ServiceStatus
 
+from scenario import trigger
 from scenario.state import Container, ExecOutput, Mount, State
 
 
 @pytest.fixture(scope="function")
 def charm_cls():
     class MyCharm(CharmBase):
         def __init__(self, framework: Framework):
@@ -25,41 +26,44 @@
     return MyCharm
 
 
 def test_no_containers(charm_cls):
     def callback(self: CharmBase):
         assert not self.unit.containers
 
-    State().trigger(
+    trigger(
+        State(),
         charm_type=charm_cls,
         meta={"name": "foo"},
         event="start",
         post_event=callback,
     )
 
 
 def test_containers_from_meta(charm_cls):
     def callback(self: CharmBase):
         assert self.unit.containers
         assert self.unit.get_container("foo")
 
-    State().trigger(
+    trigger(
+        State(),
         charm_type=charm_cls,
         meta={"name": "foo", "containers": {"foo": {}}},
         event="start",
         post_event=callback,
     )
 
 
 @pytest.mark.parametrize("can_connect", (True, False))
 def test_connectivity(charm_cls, can_connect):
     def callback(self: CharmBase):
         assert can_connect == self.unit.get_container("foo").can_connect()
 
-    State(containers=[Container(name="foo", can_connect=can_connect)]).trigger(
+    trigger(
+        State(containers=[Container(name="foo", can_connect=can_connect)]),
         charm_type=charm_cls,
         meta={"name": "foo", "containers": {"foo": {}}},
         event="start",
         post_event=callback,
     )
 
 
@@ -70,21 +74,24 @@
     pth.write_text(text)
 
     def callback(self: CharmBase):
         container = self.unit.get_container("foo")
         baz = container.pull("/bar/baz.txt")
         assert baz.read() == text
 
-    State(
-        containers=[
-            Container(
-                name="foo", can_connect=True, mounts={"bar": Mount("/bar/baz.txt", pth)}
-            )
-        ]
-    ).trigger(
+    trigger(
+        State(
+            containers=[
+                Container(
+                    name="foo",
+                    can_connect=True,
+                    mounts={"bar": Mount("/bar/baz.txt", pth)},
+                )
+            ]
+        ),
         charm_type=charm_cls,
         meta={"name": "foo", "containers": {"foo": {}}},
         event="start",
         post_event=callback,
     )
 
 
@@ -112,15 +119,16 @@
         containers=[
             Container(
                 name="foo", can_connect=True, mounts={"foo": Mount("/foo", td.name)}
             )
         ]
     )
 
-    out = state.trigger(
+    out = trigger(
+        state,
         charm_type=charm_cls,
         meta={"name": "foo", "containers": {"foo": {}}},
         event="start",
         post_event=callback,
     )
 
     if make_dirs:
@@ -163,38 +171,40 @@
 def test_exec(charm_cls, cmd, out):
     def callback(self: CharmBase):
         container = self.unit.get_container("foo")
         proc = container.exec([cmd])
         proc.wait()
         assert proc.stdout.read() == "hello pebble"
 
-    State(
-        containers=[
-            Container(
-                name="foo",
-                can_connect=True,
-                exec_mock={(cmd,): ExecOutput(stdout="hello pebble")},
-            )
-        ]
-    ).trigger(
+    trigger(
+        State(
+            containers=[
+                Container(
+                    name="foo",
+                    can_connect=True,
+                    exec_mock={(cmd,): ExecOutput(stdout="hello pebble")},
+                )
+            ]
+        ),
         charm_type=charm_cls,
         meta={"name": "foo", "containers": {"foo": {}}},
         event="start",
         post_event=callback,
     )
 
 
 def test_pebble_ready(charm_cls):
     def callback(self: CharmBase):
         foo = self.unit.get_container("foo")
         assert foo.can_connect()
 
     container = Container(name="foo", can_connect=True)
 
-    State(containers=[container]).trigger(
+    trigger(
+        State(containers=[container]),
         charm_type=charm_cls,
         meta={"name": "foo", "containers": {"foo": {}}},
         event=container.pebble_ready_event,
         post_event=callback,
     )
 
 
@@ -247,15 +257,16 @@
         service_status={
             "fooserv": pebble.ServiceStatus.ACTIVE,
             # todo: should we disallow setting status for services that aren't known YET?
             "barserv": starting_service_status,
         },
     )
 
-    out = State(containers=[container]).trigger(
+    out = trigger(
+        State(containers=[container]),
         charm_type=charm_cls,
         meta={"name": "foo", "containers": {"foo": {}}},
         event=container.pebble_ready_event,
         post_event=callback,
     )
 
     serv = lambda name, obj: pebble.Service(name, raw=obj)
```

### Comparing `ops-scenario-2.2/tests/test_e2e/test_play_assertions.py` & `ops-scenario-3.0a1/tests/test_e2e/test_play_assertions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 from ops.charm import CharmBase
 from ops.framework import Framework
 from ops.model import ActiveStatus, BlockedStatus
 
+from scenario import trigger
 from scenario.state import Event, Relation, State, Status, _CharmSpec
 
 
 @pytest.fixture(scope="function")
 def mycharm():
     class MyCharm(CharmBase):
         _call = None
@@ -43,15 +44,16 @@
 
     mycharm._call = call
 
     initial_state = State(
         config={"foo": "bar"}, leader=True, status=Status(unit=BlockedStatus("foo"))
     )
 
-    out = initial_state.trigger(
+    out = trigger(
+        initial_state,
         charm_type=mycharm,
         meta={"name": "foo"},
         config={"options": {"foo": {"type": "string"}}},
         event="start",
         post_event=post_event,
         pre_event=pre_event,
     )
@@ -96,26 +98,28 @@
         assert remote_units_data == {
             "karlos/0": {"foo": "bar"},
             "karlos/1": {"baz": "qux"},
         }
 
         assert remote_app_data == {"yaba": "doodle"}
 
-    State(
+    state_in = State(
         relations=[
             Relation(
                 endpoint="relation_test",
                 interface="azdrubales",
                 relation_id=1,
                 remote_app_name="karlos",
                 remote_app_data={"yaba": "doodle"},
                 remote_units_data={0: {"foo": "bar"}, 1: {"baz": "qux"}},
             )
         ]
-    ).trigger(
+    )
+    trigger(
+        state_in,
         charm_type=mycharm,
         meta={
             "name": "foo",
             "requires": {"relation_test": {"interface": "azdrubales"}},
         },
         event="update_status",
         post_event=check_relation_data,
```

### Comparing `ops-scenario-2.2/tests/test_e2e/test_relations.py` & `ops-scenario-3.0a1/tests/test_e2e/test_relations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Type
 
 import pytest
 from ops.charm import CharmBase, CharmEvents, RelationDepartedEvent
 from ops.framework import EventBase, Framework
 
+from scenario import trigger
 from scenario.state import (
     PeerRelation,
     Relation,
     RelationBase,
     State,
     StateValidationError,
     SubordinateRelation,
@@ -44,22 +45,23 @@
 def test_get_relation(mycharm):
     def pre_event(charm: CharmBase):
         assert charm.model.get_relation("foo")
         assert charm.model.get_relation("bar") is None
         assert charm.model.get_relation("qux")
         assert charm.model.get_relation("zoo") is None
 
-    State(
-        config={"foo": "bar"},
-        leader=True,
-        relations=[
-            Relation(endpoint="foo", interface="foo", remote_app_name="remote"),
-            Relation(endpoint="qux", interface="qux", remote_app_name="remote"),
-        ],
-    ).trigger(
+    trigger(
+        State(
+            config={"foo": "bar"},
+            leader=True,
+            relations=[
+                Relation(endpoint="foo", interface="foo", remote_app_name="remote"),
+                Relation(endpoint="qux", interface="qux", remote_app_name="remote"),
+            ],
+        ),
         "start",
         mycharm,
         meta={
             "name": "local",
             "requires": {
                 "foo": {"interface": "foo"},
                 "bar": {"interface": "bar"},
@@ -77,19 +79,20 @@
     "evt_name", ("changed", "broken", "departed", "joined", "created")
 )
 def test_relation_events(mycharm, evt_name):
     relation = Relation(endpoint="foo", interface="foo", remote_app_name="remote")
 
     mycharm._call = lambda self, evt: None
 
-    State(
-        relations=[
-            relation,
-        ],
-    ).trigger(
+    trigger(
+        State(
+            relations=[
+                relation,
+            ],
+        ),
         getattr(relation, f"{evt_name}_event"),
         mycharm,
         meta={
             "name": "local",
             "requires": {
                 "foo": {"interface": "foo"},
             },
@@ -113,19 +116,20 @@
     )
 
     def callback(charm: CharmBase, _):
         assert charm.model.get_relation("foo").app.name == remote_app_name
 
     mycharm._call = callback
 
-    State(
-        relations=[
-            relation,
-        ],
-    ).trigger(
+    trigger(
+        State(
+            relations=[
+                relation,
+            ],
+        ),
         getattr(relation, f"{evt_name}_event"),
         mycharm,
         meta={
             "name": "local",
             "requires": {
                 "foo": {"interface": "foo"},
             },
@@ -154,19 +158,20 @@
         assert event.app
         assert event.unit
         if isinstance(event, RelationDepartedEvent):
             assert event.departing_unit
 
     mycharm._call = callback
 
-    State(
-        relations=[
-            relation,
-        ],
-    ).trigger(
+    trigger(
+        State(
+            relations=[
+                relation,
+            ],
+        ),
         getattr(relation, f"{evt_name}_event")(remote_unit_id=remote_unit_id),
         mycharm,
         meta={
             "name": "local",
             "requires": {
                 "foo": {"interface": "foo"},
             },
@@ -193,19 +198,20 @@
     def callback(charm: CharmBase, event):
         assert event.app  # that's always present
         assert event.unit
         assert (evt_name == "departed") is bool(getattr(event, "departing_unit", False))
 
     mycharm._call = callback
 
-    State(
-        relations=[
-            relation,
-        ],
-    ).trigger(
+    trigger(
+        State(
+            relations=[
+                relation,
+            ],
+        ),
         getattr(relation, f"{evt_name}_event"),
         mycharm,
         meta={
             "name": "local",
             "requires": {
                 "foo": {"interface": "foo"},
             },
@@ -248,16 +254,19 @@
                 "interface": "i3",
                 # this is a subordinate relation.
                 "scope": "container",
             }
         },
         "peers": {"b": {"interface": "i2"}},
     }
-    state = State(relations=[relation]).trigger(
-        getattr(relation, evt_name + "_event"), mycharm, meta=meta
+    state = trigger(
+        State(relations=[relation]),
+        getattr(relation, evt_name + "_event"),
+        mycharm,
+        meta=meta,
     )
 
 
 def test_trigger_sub_relation(mycharm):
     meta = {
         "name": "mycharm",
         "provides": {
@@ -278,15 +287,19 @@
 
     def post_event(charm: CharmBase):
         b_relations = charm.model.relations["foo"]
         assert len(b_relations) == 2
         for relation in b_relations:
             assert len(relation.units) == 1
 
-    State(relations=[sub1, sub2]).trigger(
-        "update-status", mycharm, meta=meta, post_event=post_event
+    trigger(
+        State(relations=[sub1, sub2]),
+        "update-status",
+        mycharm,
+        meta=meta,
+        post_event=post_event,
     )
 
 
 def test_cannot_instantiate_relationbase():
     with pytest.raises(RuntimeError):
         RelationBase("")
```

### Comparing `ops-scenario-2.2/tests/test_e2e/test_rubbish_events.py` & `ops-scenario-3.0a1/tests/test_e2e/test_rubbish_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 
 import pytest
 from ops.charm import CharmBase, CharmEvents
 from ops.framework import EventBase, EventSource, Framework, Object
 
+from scenario import trigger
 from scenario.ops_main_mock import NoObserverError
 from scenario.state import Container, Event, State, _CharmSpec
 
 
 class QuxEvent(EventBase):
     pass
 
@@ -47,30 +48,30 @@
 def test_rubbish_event_raises(mycharm, evt_name):
     with pytest.raises(NoObserverError):
         if evt_name.startswith("kazoo"):
             os.environ["SCENARIO_SKIP_CONSISTENCY_CHECKS"] = "true"
             # else it will whine about the container not being in state and meta;
             # but if we put the container in meta, it will actually register an event!
 
-        State().trigger(evt_name, mycharm, meta={"name": "foo"})
+        trigger(State(), evt_name, mycharm, meta={"name": "foo"})
 
         if evt_name.startswith("kazoo"):
             os.environ["SCENARIO_SKIP_CONSISTENCY_CHECKS"] = "false"
 
 
 @pytest.mark.parametrize("evt_name", ("qux",))
 def test_custom_events_pass(mycharm, evt_name):
-    State().trigger(evt_name, mycharm, meta={"name": "foo"})
+    trigger(State(), evt_name, mycharm, meta={"name": "foo"})
 
 
 # cfr: https://github.com/PietroPasotti/ops-scenario/pull/11#discussion_r1101694961
 @pytest.mark.parametrize("evt_name", ("sub",))
 def test_custom_events_sub_raise(mycharm, evt_name):
     with pytest.raises(RuntimeError):
-        State().trigger(evt_name, mycharm, meta={"name": "foo"})
+        trigger(State(), evt_name, mycharm, meta={"name": "foo"})
 
 
 @pytest.mark.parametrize(
     "evt_name, expected",
     (
         ("qux", False),
         ("sub", False),
```

### Comparing `ops-scenario-2.2/tests/test_e2e/test_secrets.py` & `ops-scenario-3.0a1/tests/test_e2e/test_secrets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 from ops.charm import CharmBase
 from ops.framework import Framework
 from ops.model import SecretRotate
 
+from scenario import trigger
 from scenario.state import Relation, Secret, State
 
 
 @pytest.fixture(scope="function")
 def mycharm():
     class MyCharm(CharmBase):
         def __init__(self, framework: Framework):
@@ -23,48 +24,58 @@
 def test_get_secret_no_secret(mycharm):
     def post_event(charm: CharmBase):
         with pytest.raises(RuntimeError):
             assert charm.model.get_secret(id="foo")
         with pytest.raises(RuntimeError):
             assert charm.model.get_secret(label="foo")
 
-    State().trigger(
-        "update_status", mycharm, meta={"name": "local"}, post_event=post_event
+    trigger(
+        State(), "update_status", mycharm, meta={"name": "local"}, post_event=post_event
     )
 
 
 def test_get_secret(mycharm):
     def post_event(charm: CharmBase):
         assert charm.model.get_secret(id="foo").get_content()["a"] == "b"
 
-    State(secrets=[Secret(id="foo", contents={0: {"a": "b"}})]).trigger(
-        "update_status", mycharm, meta={"name": "local"}, post_event=post_event
+    trigger(
+        State(secrets=[Secret(id="foo", contents={0: {"a": "b"}})]),
+        "update_status",
+        mycharm,
+        meta={"name": "local"},
+        post_event=post_event,
     )
 
 
 def test_get_secret_peek_update(mycharm):
     def post_event(charm: CharmBase):
         assert charm.model.get_secret(id="foo").get_content()["a"] == "b"
         assert charm.model.get_secret(id="foo").peek_content()["a"] == "c"
         assert charm.model.get_secret(id="foo").get_content()["a"] == "b"
 
         assert charm.model.get_secret(id="foo").get_content(refresh=True)["a"] == "c"
         assert charm.model.get_secret(id="foo").get_content()["a"] == "c"
 
-    State(
-        secrets=[
-            Secret(
-                id="foo",
-                contents={
-                    0: {"a": "b"},
-                    1: {"a": "c"},
-                },
-            )
-        ]
-    ).trigger("update_status", mycharm, meta={"name": "local"}, post_event=post_event)
+    trigger(
+        State(
+            secrets=[
+                Secret(
+                    id="foo",
+                    contents={
+                        0: {"a": "b"},
+                        1: {"a": "c"},
+                    },
+                )
+            ]
+        ),
+        "update_status",
+        mycharm,
+        meta={"name": "local"},
+        post_event=post_event,
+    )
 
 
 def test_secret_changed_owner_evt_fails(mycharm):
     with pytest.raises(ValueError):
         _ = Secret(
             id="foo",
             contents={
@@ -90,16 +101,16 @@
         )
 
 
 def test_add(mycharm):
     def post_event(charm: CharmBase):
         charm.unit.add_secret({"foo": "bar"}, label="mylabel")
 
-    out = State().trigger(
-        "update_status", mycharm, meta={"name": "local"}, post_event=post_event
+    out = trigger(
+        State(), "update_status", mycharm, meta={"name": "local"}, post_event=post_event
     )
     assert out.secrets
     secret = out.secrets[0]
     assert secret.contents[0] == {"foo": "bar"}
     assert secret.label == "mylabel"
 
 
@@ -110,76 +121,89 @@
         secret = charm.model.get_secret(id="foo")
         info = secret.get_info()
 
         assert secret.label is None
         assert info.label == "mylabel"
         assert info.rotation == SecretRotate.HOURLY
 
-    State(
-        secrets=[
-            Secret(
-                owner="unit",
-                id="foo",
-                label="mylabel",
-                description="foobarbaz",
-                rotate=SecretRotate.HOURLY,
-                contents={
-                    0: {"a": "b"},
-                },
-            )
-        ]
-    ).trigger("update_status", mycharm, meta={"name": "local"}, post_event=post_event)
+    trigger(
+        State(
+            secrets=[
+                Secret(
+                    owner="unit",
+                    id="foo",
+                    label="mylabel",
+                    description="foobarbaz",
+                    rotate=SecretRotate.HOURLY,
+                    contents={
+                        0: {"a": "b"},
+                    },
+                )
+            ]
+        ),
+        "update_status",
+        mycharm,
+        meta={"name": "local"},
+        post_event=post_event,
+    )
 
 
 def test_meta_nonowner(mycharm):
     def post_event(charm: CharmBase):
         secret = charm.model.get_secret(id="foo")
         with pytest.raises(RuntimeError):
             info = secret.get_info()
 
-    State(
-        secrets=[
-            Secret(
-                id="foo",
-                label="mylabel",
-                description="foobarbaz",
-                rotate=SecretRotate.HOURLY,
-                contents={
-                    0: {"a": "b"},
-                },
-            )
-        ]
-    ).trigger("update_status", mycharm, meta={"name": "local"}, post_event=post_event)
+    trigger(
+        State(
+            secrets=[
+                Secret(
+                    id="foo",
+                    label="mylabel",
+                    description="foobarbaz",
+                    rotate=SecretRotate.HOURLY,
+                    contents={
+                        0: {"a": "b"},
+                    },
+                )
+            ]
+        ),
+        "update_status",
+        mycharm,
+        meta={"name": "local"},
+        post_event=post_event,
+    )
 
 
 @pytest.mark.parametrize("app", (True, False))
 def test_grant(mycharm, app):
     def post_event(charm: CharmBase):
         secret = charm.model.get_secret(label="mylabel")
         foo = charm.model.get_relation("foo")
         if app:
             secret.grant(relation=foo)
         else:
             secret.grant(relation=foo, unit=foo.units.pop())
 
-    out = State(
-        relations=[Relation("foo", "remote")],
-        secrets=[
-            Secret(
-                owner="unit",
-                id="foo",
-                label="mylabel",
-                description="foobarbaz",
-                rotate=SecretRotate.HOURLY,
-                contents={
-                    0: {"a": "b"},
-                },
-            )
-        ],
-    ).trigger(
+    out = trigger(
+        State(
+            relations=[Relation("foo", "remote")],
+            secrets=[
+                Secret(
+                    owner="unit",
+                    id="foo",
+                    label="mylabel",
+                    description="foobarbaz",
+                    rotate=SecretRotate.HOURLY,
+                    contents={
+                        0: {"a": "b"},
+                    },
+                )
+            ],
+        ),
         "update_status",
         mycharm,
         meta={"name": "local", "requires": {"foo": {"interface": "bar"}}},
         post_event=post_event,
     )
 
     vals = list(out.secrets[0].remote_grants.values())
@@ -190,26 +214,27 @@
     def post_event(charm: CharmBase):
         secret = charm.model.get_secret(id="foo")
         with pytest.raises(RuntimeError):
             secret = charm.model.get_secret(label="mylabel")
             foo = charm.model.get_relation("foo")
             secret.grant(relation=foo)
 
-    out = State(
-        relations=[Relation("foo", "remote")],
-        secrets=[
-            Secret(
-                id="foo",
-                label="mylabel",
-                description="foobarbaz",
-                rotate=SecretRotate.HOURLY,
-                contents={
-                    0: {"a": "b"},
-                },
-            )
-        ],
-    ).trigger(
+    out = trigger(
+        State(
+            relations=[Relation("foo", "remote")],
+            secrets=[
+                Secret(
+                    id="foo",
+                    label="mylabel",
+                    description="foobarbaz",
+                    rotate=SecretRotate.HOURLY,
+                    contents={
+                        0: {"a": "b"},
+                    },
+                )
+            ],
+        ),
         "update_status",
         mycharm,
         meta={"name": "local", "requires": {"foo": {"interface": "bar"}}},
         post_event=post_event,
     )
```

### Comparing `ops-scenario-2.2/tests/test_e2e/test_state.py` & `ops-scenario-3.0a1/tests/test_e2e/test_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,17 @@
 from typing import Type
 
 import pytest
 from ops.charm import CharmBase, CharmEvents
 from ops.framework import EventBase, Framework
 from ops.model import ActiveStatus, UnknownStatus, WaitingStatus
 
+from scenario import trigger
 from scenario.state import Container, Relation, State, sort_patch
 
-# from tests.setup_tests import setup_tests
-#
-# setup_tests()  # noqa & keep this on top
-
-
 CUSTOM_EVT_SUFFIXES = {
     "relation_created",
     "relation_joined",
     "relation_changed",
     "relation_departed",
     "relation_broken",
     "storage_attached",
@@ -55,47 +51,49 @@
 
 @pytest.fixture
 def state():
     return State(config={"foo": "bar"}, leader=True)
 
 
 def test_bare_event(state, mycharm):
-    out = state.trigger("start", mycharm, meta={"name": "foo"})
+    out = trigger(state, "start", mycharm, meta={"name": "foo"})
     out_purged = out.replace(juju_log=[], stored_state=state.stored_state)
     assert state.jsonpatch_delta(out_purged) == []
 
 
 def test_leader_get(state, mycharm):
     def pre_event(charm):
         assert charm.unit.is_leader()
 
-    state.trigger(
+    trigger(
+        state,
         "start",
         mycharm,
         meta={"name": "foo"},
         pre_event=pre_event,
     )
 
 
 def test_status_setting(state, mycharm):
     def call(charm: CharmBase, _):
         assert isinstance(charm.unit.status, UnknownStatus)
         charm.unit.status = ActiveStatus("foo test")
         charm.app.status = WaitingStatus("foo barz")
 
     mycharm._call = call
-    out = state.trigger(
+    out = trigger(
+        state,
         "start",
         mycharm,
         meta={"name": "foo"},
         config={"options": {"foo": {"type": "string"}}},
     )
     assert out.status.unit == ActiveStatus("foo test")
     assert out.status.app == WaitingStatus("foo barz")
-    assert out.status.app_version == ""
+    assert out.status.workload_version == ""
 
     # ignore logging output and stored state in the delta
     out_purged = out.replace(juju_log=[], stored_state=state.stored_state)
     assert out_purged.jsonpatch_delta(state) == sort_patch(
         [
             {"op": "replace", "path": "/status/app/message", "value": "foo barz"},
             {"op": "replace", "path": "/status/app/name", "value": "waiting"},
@@ -119,15 +117,16 @@
 def test_container(connect, mycharm):
     def pre_event(charm: CharmBase):
         container = charm.unit.get_container("foo")
         assert container is not None
         assert container.name == "foo"
         assert container.can_connect() is connect
 
-    State(containers=[Container(name="foo", can_connect=connect)]).trigger(
+    trigger(
+        State(containers=[Container(name="foo", can_connect=connect)]),
         "start",
         mycharm,
         meta={
             "name": "foo",
             "containers": {"foo": {"resource": "bar"}},
         },
         pre_event=pre_event,
@@ -161,15 +160,16 @@
                 remote_unit_ids=[0, 1, 2],
                 remote_app_data={"a": "b"},
                 local_unit_data={"c": "d"},
                 remote_units_data={0: {}, 1: {"e": "f"}, 2: {}},
             )
         ]
     )
-    state.trigger(
+    trigger(
+        state,
         "start",
         mycharm,
         meta={
             "name": "local",
             "requires": {"foo": {"interface": "bar"}},
         },
         pre_event=pre_event,
@@ -214,15 +214,16 @@
     )
     state = State(
         leader=True,
         relations=[relation],
     )
 
     assert not mycharm.called
-    out = state.trigger(
+    out = trigger(
+        state,
         event="start",
         charm_type=mycharm,
         meta={
             "name": "foo",
             "requires": {"foo": {"interface": "bar"}},
         },
         pre_event=pre_event,
```

### Comparing `ops-scenario-2.2/tests/test_e2e/test_status.py` & `ops-scenario-3.0a1/tests/test_e2e/test_status.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 from ops.charm import CharmBase
 from ops.framework import Framework
 from ops.model import ActiveStatus, BlockedStatus, UnknownStatus, WaitingStatus
 
+from scenario import trigger
 from scenario.state import State, Status
 
 
 @pytest.fixture(scope="function")
 def mycharm():
     class MyCharm(CharmBase):
         def __init__(self, framework: Framework):
@@ -20,30 +21,38 @@
     return MyCharm
 
 
 def test_initial_status(mycharm):
     def post_event(charm: CharmBase):
         assert charm.unit.status == UnknownStatus()
 
-    out = State(leader=True).trigger(
-        "update_status", mycharm, meta={"name": "local"}, post_event=post_event
+    out = trigger(
+        State(leader=True),
+        "update_status",
+        mycharm,
+        meta={"name": "local"},
+        post_event=post_event,
     )
 
     assert out.status.unit == UnknownStatus()
 
 
 def test_status_history(mycharm):
     def post_event(charm: CharmBase):
         for obj in [charm.unit, charm.app]:
             obj.status = ActiveStatus("1")
             obj.status = BlockedStatus("2")
             obj.status = WaitingStatus("3")
 
-    out = State(leader=True).trigger(
-        "update_status", mycharm, meta={"name": "local"}, post_event=post_event
+    out = trigger(
+        State(leader=True),
+        "update_status",
+        mycharm,
+        meta={"name": "local"},
+        post_event=post_event,
     )
 
     assert out.status.unit == WaitingStatus("3")
     assert out.status.unit_history == [
         UnknownStatus(),
         ActiveStatus("1"),
         BlockedStatus("2"),
@@ -58,16 +67,23 @@
 
 
 def test_status_history_preservation(mycharm):
     def post_event(charm: CharmBase):
         for obj in [charm.unit, charm.app]:
             obj.status = WaitingStatus("3")
 
-    out = State(
-        leader=True, status=Status(unit=ActiveStatus("foo"), app=ActiveStatus("bar"))
-    ).trigger("update_status", mycharm, meta={"name": "local"}, post_event=post_event)
+    out = trigger(
+        State(
+            leader=True,
+            status=Status(unit=ActiveStatus("foo"), app=ActiveStatus("bar")),
+        ),
+        "update_status",
+        mycharm,
+        meta={"name": "local"},
+        post_event=post_event,
+    )
 
     assert out.status.unit == WaitingStatus("3")
     assert out.status.unit_history == [ActiveStatus("foo")]
 
     assert out.status.app == WaitingStatus("3")
     assert out.status.app_history == [ActiveStatus("bar")]
```

### Comparing `ops-scenario-2.2/tests/test_e2e/test_stored_state.py` & `ops-scenario-3.0a1/tests/test_e2e/test_stored_state.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 from ops.charm import CharmBase
 from ops.framework import Framework
 from ops.framework import StoredState as ops_storedstate
 
+from scenario import trigger
 from scenario.state import State, StoredState
 
 
 @pytest.fixture(scope="function")
 def mycharm():
     class MyCharm(CharmBase):
         META = {"name": "mycharm"}
@@ -26,20 +27,25 @@
             self._read["foo"] = self._stored.foo
             self._read["baz"] = self._stored.baz
 
     return MyCharm
 
 
 def test_stored_state_default(mycharm):
-    out = State().trigger("start", mycharm, meta=mycharm.META)
+    out = trigger(State(), "start", mycharm, meta=mycharm.META)
     assert out.stored_state[0].content == {"foo": "bar", "baz": {12: 142}}
 
 
 def test_stored_state_initialized(mycharm):
-    out = State(
-        stored_state=[
-            StoredState("MyCharm", name="_stored", content={"foo": "FOOX"}),
-        ]
-    ).trigger("start", mycharm, meta=mycharm.META)
+    out = trigger(
+        State(
+            stored_state=[
+                StoredState("MyCharm", name="_stored", content={"foo": "FOOX"}),
+            ]
+        ),
+        "start",
+        mycharm,
+        meta=mycharm.META,
+    )
     # todo: ordering is messy?
     assert out.stored_state[1].content == {"foo": "FOOX", "baz": {12: 142}}
     assert out.stored_state[0].content == {"foo": "bar", "baz": {12: 142}}
```

### Comparing `ops-scenario-2.2/tests/test_e2e/test_vroot.py` & `ops-scenario-3.0a1/tests/test_e2e/test_vroot.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import pytest
 from ops.charm import CharmBase
 from ops.framework import Framework
 from ops.model import ActiveStatus
 
 from scenario import State
-from scenario.runtime import DirtyVirtualCharmRootError
+from scenario.runtime import DirtyVirtualCharmRootError, trigger
 
 
 class MyCharm(CharmBase):
     META = {"name": "my-charm"}
 
     def __init__(self, framework: Framework):
         super().__init__(framework)
@@ -30,15 +30,16 @@
         foobar.write_text("hello")
 
         baz = src / "baz"
         baz.mkdir(parents=True)
         quxcos = baz / "qux.kaboodle"
         quxcos.write_text("world")
 
-        out = State().trigger(
+        out = trigger(
+            State(),
             "start",
             charm_type=MyCharm,
             meta=MyCharm.META,
             charm_root=t,
         )
 
     assert out.status.unit == ("active", "hello world")
@@ -48,13 +49,14 @@
 def test_dirty_vroot_raises(meta_overwrite):
     with tempfile.TemporaryDirectory() as myvroot:
         t = Path(myvroot)
         meta_file = t / f"{meta_overwrite}.yaml"
         meta_file.touch()
 
         with pytest.raises(DirtyVirtualCharmRootError):
-            State().trigger(
+            trigger(
+                State(),
                 "start",
                 charm_type=MyCharm,
                 meta=MyCharm.META,
                 charm_root=t,
             )
```

### Comparing `ops-scenario-2.2/tests/test_emitted_events_util.py` & `ops-scenario-3.0a1/tests/test_emitted_events_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from ops.charm import CharmBase, CharmEvents, StartEvent
 from ops.framework import CommitEvent, EventBase, EventSource, PreCommitEvent
 
-from scenario import Event, State, capture_events
+from scenario import Event, State, capture_events, trigger
 
 
 class Foo(EventBase):
     pass
 
 
 class MyCharmEvents(CharmEvents):
@@ -27,63 +27,69 @@
 
     def _on_foo(self, e):
         pass
 
 
 def test_capture_custom_evt():
     with capture_events(Foo) as emitted:
-        State().trigger("foo", MyCharm, meta=MyCharm.META)
+        trigger(State(), "foo", MyCharm, meta=MyCharm.META)
 
     assert len(emitted) == 1
     assert isinstance(emitted[0], Foo)
 
 
 def test_capture_custom_evt_nonspecific_capture():
     with capture_events() as emitted:
-        State().trigger("foo", MyCharm, meta=MyCharm.META)
+        trigger(State(), "foo", MyCharm, meta=MyCharm.META)
 
     assert len(emitted) == 1
     assert isinstance(emitted[0], Foo)
 
 
 def test_capture_custom_evt_nonspecific_capture_include_fw_evts():
     with capture_events(include_framework=True) as emitted:
-        State().trigger("foo", MyCharm, meta=MyCharm.META)
+        trigger(State(), "foo", MyCharm, meta=MyCharm.META)
 
     assert len(emitted) == 3
     assert isinstance(emitted[0], Foo)
     assert isinstance(emitted[1], PreCommitEvent)
     assert isinstance(emitted[2], CommitEvent)
 
 
 def test_capture_juju_evt():
     with capture_events() as emitted:
-        State().trigger("start", MyCharm, meta=MyCharm.META)
+        trigger(State(), "start", MyCharm, meta=MyCharm.META)
 
     assert len(emitted) == 2
     assert isinstance(emitted[0], StartEvent)
     assert isinstance(emitted[1], Foo)
 
 
 def test_capture_deferred_evt():
     # todo: this test should pass with ops < 2.1 as well
     with capture_events() as emitted:
-        State(deferred=[Event("foo").deferred(handler=MyCharm._on_foo)]).trigger(
-            "start", MyCharm, meta=MyCharm.META
+        trigger(
+            State(deferred=[Event("foo").deferred(handler=MyCharm._on_foo)]),
+            "start",
+            MyCharm,
+            meta=MyCharm.META,
         )
 
     assert len(emitted) == 3
     assert isinstance(emitted[0], Foo)
     assert isinstance(emitted[1], StartEvent)
     assert isinstance(emitted[2], Foo)
 
 
 def test_capture_no_deferred_evt():
     # todo: this test should pass with ops < 2.1 as well
     with capture_events(include_deferred=False) as emitted:
-        State(deferred=[Event("foo").deferred(handler=MyCharm._on_foo)]).trigger(
-            "start", MyCharm, meta=MyCharm.META
+        trigger(
+            State(deferred=[Event("foo").deferred(handler=MyCharm._on_foo)]),
+            "start",
+            MyCharm,
+            meta=MyCharm.META,
         )
 
     assert len(emitted) == 2
     assert isinstance(emitted[0], StartEvent)
     assert isinstance(emitted[1], Foo)
```

### Comparing `ops-scenario-2.2/tests/test_runtime.py` & `ops-scenario-3.0a1/tests/test_runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         meta_file = temppath / "metadata.yaml"
         meta_file.write_text(yaml.safe_dump(meta))
 
         runtime = Runtime(
             _CharmSpec(
                 charm_type(),
                 meta=meta,
-            )
+            ),
         )
 
         pre_event = MagicMock(return_value=None)
         post_event = MagicMock(return_value=None)
         runtime.exec(
             state=State(),
             event=Event("update_status"),
@@ -97,14 +97,15 @@
     my_charm_type = charm_type()
 
     runtime = Runtime(
         _CharmSpec(
             my_charm_type,
             meta=meta,
         ),
-        unit_id=unit_id,
     )
 
     def post_event(charm: CharmBase):
         assert charm.unit.name == f"{app_name}/{unit_id}"
 
-    runtime.exec(state=State(), event=Event("start"), post_event=post_event)
+    runtime.exec(
+        state=State(unit_id=unit_id), event=Event("start"), post_event=post_event
+    )
```

### Comparing `ops-scenario-2.2/tox.ini` & `ops-scenario-3.0a1/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,59 @@
-# Copyright 2022 Canonical
-# See LICENSE file for licensing details.
-
 [tox]
-envlist =
-    {py36,py37,py38,py311}
-    unit, lint
-isolated_build = True
-skip_missing_interpreters = True
-
+requires =
+    tox>=4.2
+env_list =
+    py311
+    py38
+    py37
+    py36
+    unit
+    lint
+    lint-tests
+skip_missing_interpreters = true
 
 [vars]
 src_path = {toxinidir}/scenario
 tst_path = {toxinidir}/tests
+all_path = {[vars]src_path}, {[vars]tst_path}
 
+[testenv:lint]
+description = Format the code base to adhere to our styles, and complain about what we cannot do automatically.
+skip_install = true
+deps =
+    pre-commit>=3.2.2
+commands =
+    pre-commit run --all-files {posargs}
+    python -c 'print(r"hint: run {envbindir}{/}pre-commit install to add checks as pre-commit hook")'
 
 [testenv:unit]
-description =  unit tests
+description = unit tests
 deps =
     coverage[toml]
-    pytest
     jsonpatch
+    pytest
 commands =
     coverage run \
       --source={[vars]src_path} \
       -m pytest -v --tb native --log-cli-level=INFO -s {posargs} {[vars]tst_path}
     coverage report
 
-
-[testenv:lint]
-skip_install=True
-description =  lint
+[testenv:lint-tests]
+description = Lint test files.
+skip_install = true
 deps =
-    coverage[toml]
-    pytest
-    jsonpatch
     black
+    coverage[toml]
     isort
 commands =
     black --check tests scenario
-    isort --check-only --profile black tests scenario
-
+    isort --check-only --profile black {[vars]tst_path}
 
 [testenv:fmt]
-skip_install=True
-description = Format code
+description = Format code.
+skip_install = true
 deps =
     black
     isort
 commands =
     black tests scenario
     isort --profile black tests scenario
```

