# Comparing `tmp/ops-scenario-3.0.1.tar.gz` & `tmp/ops-scenario-3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-scenario-3.0.1.tar", last modified: Tue May  9 11:14:05 2023, max compression
+gzip compressed data, was "ops-scenario-3.0a1.tar", last modified: Tue May  9 11:10:22 2023, max compression
```

## Comparing `ops-scenario-3.0.1.tar` & `ops-scenario-3.0a1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:14:05.882728 ops-scenario-3.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:14:05.870728 ops-scenario-3.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:14:05.874728 ops-scenario-3.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/.github/workflows/build_wheels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/.github/workflows/quality_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    31728 2023-05-09 11:14:05.882728 ops-scenario-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30917 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:14:05.874728 ops-scenario-3.0.1/ops_scenario.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31728 2023-05-09 11:14:05.000000 ops-scenario-3.0.1/ops_scenario.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-09 11:14:05.000000 ops-scenario-3.0.1/ops_scenario.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:14:05.000000 ops-scenario-3.0.1/ops_scenario.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 11:14:05.000000 ops-scenario-3.0.1/ops_scenario.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 11:14:05.000000 ops-scenario-3.0.1/ops_scenario.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 11:14:05.000000 ops-scenario-3.0.1/ops_scenario.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:14:05.874728 ops-scenario-3.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/resources/state-transition-model.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:14:05.874728 ops-scenario-3.0.1/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/consistency_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/emitted_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/fs_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/mocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/ops_main_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:14:05.878728 ops-scenario-3.0.1/scenario/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/scripts/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/scripts/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    29890 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/scripts/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    40177 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/scenario/state.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:14:05.882728 ops-scenario-3.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:14:05.878728 ops-scenario-3.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:14:05.878728 ops-scenario-3.0.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/resources/demo_decorate_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_consistency_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:14:05.882728 ops-scenario-3.0.1/tests/test_e2e/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_builtin_scenes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_custom_event_triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_deferred.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_juju_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_observers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_play_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_rubbish_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_stored_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_e2e/test_vroot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_emitted_events_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-09 11:13:56.000000 ops-scenario-3.0.1/tox.ini
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

### Comparing `ops-scenario-3.0.1/.github/workflows/build_wheels.yaml` & `ops-scenario-3.0a1/.github/workflows/build_wheels.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/.github/workflows/quality_checks.yaml` & `ops-scenario-3.0a1/.github/workflows/quality_checks.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/.pre-commit-config.yaml` & `ops-scenario-3.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/CONTRIBUTING.md` & `ops-scenario-3.0a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/LICENSE.txt` & `ops-scenario-3.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/PKG-INFO` & `ops-scenario-3.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-scenario
-Version: 3.0.1
+Version: 3.0a1
 Summary: Python library providing a Scenario-based testing API for Operator Framework charms.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/canonical/ops-scenario
 Project-URL: Bug Tracker, https://github.com/canonical/ops-scenario/issues
 Keywords: juju,test
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ops-scenario-3.0.1/README.md` & `ops-scenario-3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/ops_scenario.egg-info/PKG-INFO` & `ops-scenario-3.0a1/ops_scenario.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-scenario
-Version: 3.0.1
+Version: 3.0a1
 Summary: Python library providing a Scenario-based testing API for Operator Framework charms.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/canonical/ops-scenario
 Project-URL: Bug Tracker, https://github.com/canonical/ops-scenario/issues
 Keywords: juju,test
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ops-scenario-3.0.1/ops_scenario.egg-info/SOURCES.txt` & `ops-scenario-3.0a1/ops_scenario.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/pyproject.toml` & `ops-scenario-3.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools_scm >= 2.0.0, <3"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ops-scenario"
 
-version = "3.0.1"
+version = "3.0a1"
 
 authors = [
     { name = "Pietro Pasotti", email = "pietro.pasotti@canonical.com" }
 ]
 description = "Python library providing a Scenario-based testing API for Operator Framework charms."
 license.text = "Apache-2.0"
 keywords = ["juju", "test"]
```

### Comparing `ops-scenario-3.0.1/resources/state-transition-model.png` & `ops-scenario-3.0a1/resources/state-transition-model.png`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/scenario/__init__.py` & `ops-scenario-3.0a1/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/scenario/consistency_checker.py` & `ops-scenario-3.0a1/scenario/consistency_checker.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/scenario/context.py` & `ops-scenario-3.0a1/scenario/context.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/scenario/emitted_events.py` & `ops-scenario-3.0a1/scenario/emitted_events.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/scenario/fs_mocks.py` & `ops-scenario-3.0a1/scenario/fs_mocks.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/scenario/mocking.py` & `ops-scenario-3.0a1/scenario/mocking.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/scenario/ops_main_mock.py` & `ops-scenario-3.0a1/scenario/ops_main_mock.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/scenario/runtime.py` & `ops-scenario-3.0a1/scenario/runtime.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/scenario/scripts/main.py` & `ops-scenario-3.0a1/scenario/scripts/main.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/scenario/scripts/snapshot.py` & `ops-scenario-3.0a1/scenario/scripts/snapshot.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/scenario/scripts/utils.py` & `ops-scenario-3.0a1/scenario/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/scenario/sequences.py` & `ops-scenario-3.0a1/scenario/sequences.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/scenario/state.py` & `ops-scenario-3.0a1/scenario/state.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_consistency_checker.py` & `ops-scenario-3.0a1/tests/test_consistency_checker.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_builtin_scenes.py` & `ops-scenario-3.0a1/tests/test_e2e/test_builtin_scenes.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_config.py` & `ops-scenario-3.0a1/tests/test_e2e/test_config.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_custom_event_triggers.py` & `ops-scenario-3.0a1/tests/test_e2e/test_custom_event_triggers.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_deferred.py` & `ops-scenario-3.0a1/tests/test_e2e/test_deferred.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_juju_log.py` & `ops-scenario-3.0a1/tests/test_e2e/test_juju_log.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_network.py` & `ops-scenario-3.0a1/tests/test_e2e/test_network.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_observers.py` & `ops-scenario-3.0a1/tests/test_e2e/test_observers.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_pebble.py` & `ops-scenario-3.0a1/tests/test_e2e/test_pebble.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_play_assertions.py` & `ops-scenario-3.0a1/tests/test_e2e/test_play_assertions.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_relations.py` & `ops-scenario-3.0a1/tests/test_e2e/test_relations.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_rubbish_events.py` & `ops-scenario-3.0a1/tests/test_e2e/test_rubbish_events.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_secrets.py` & `ops-scenario-3.0a1/tests/test_e2e/test_secrets.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_state.py` & `ops-scenario-3.0a1/tests/test_e2e/test_state.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_status.py` & `ops-scenario-3.0a1/tests/test_e2e/test_status.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_stored_state.py` & `ops-scenario-3.0a1/tests/test_e2e/test_stored_state.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_e2e/test_vroot.py` & `ops-scenario-3.0a1/tests/test_e2e/test_vroot.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_emitted_events_util.py` & `ops-scenario-3.0a1/tests/test_emitted_events_util.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_plugin.py` & `ops-scenario-3.0a1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tests/test_runtime.py` & `ops-scenario-3.0a1/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.1/tox.ini` & `ops-scenario-3.0a1/tox.ini`

 * *Files identical despite different names*

