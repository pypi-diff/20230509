# Comparing `tmp/bsl-0.6.0.tar.gz` & `tmp/bsl-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsl-0.6.0.tar", last modified: Fri May  5 14:27:03 2023, max compression
+gzip compressed data, was "bsl-0.6.1.tar", last modified: Tue May  9 10:59:18 2023, max compression
```

## Comparing `bsl-0.6.0.tar` & `bsl-0.6.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.205540 bsl-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-05 14:26:19.000000 bsl-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-05 14:27:03.201540 bsl-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-05 14:26:19.000000 bsl-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.177540 bsl-0.6.0/bsl/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.181540 bsl-0.6.0/bsl/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/commands/bsl_stream_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/commands/bsl_stream_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/commands/bsl_stream_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/commands/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/commands/sys_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.181540 bsl-0.6.0/bsl/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/datasets/_fetching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/datasets/eeg_auditory_stimuli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/datasets/eeg_resting_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/datasets/eeg_resting_state_short.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/datasets/trigger_def.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.185540 bsl-0.6.0/bsl/lsl/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.189540 bsl-0.6.0/bsl/lsl/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   923264 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/lib/liblsl-1.16.0-20.04_amd64.so
--rwxr-xr-x   0 runner    (1001) docker     (123)  1115480 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/lib/liblsl-1.16.0-22.04_amd64.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   812312 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/lib/liblsl-1.16.0-OSX_amd64.dylib
--rwxr-xr-x   0 runner    (1001) docker     (123)   758048 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/lib/liblsl-1.16.0-OSX_arm64.dylib
--rw-r--r--   0 runner    (1001) docker     (123)   803840 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/lib/liblsl-1.16.0-Win_amd64.dll
--rw-r--r--   0 runner    (1001) docker     (123)   598528 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/lib/liblsl-1.16.0-Win_i386.dll
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/load_liblsl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/stream_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/stream_inlet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/stream_outlet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/lsl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.189540 bsl-0.6.0/bsl/stream_player/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_player/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_player/stream_player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.193540 bsl-0.6.0/bsl/stream_receiver/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_receiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_receiver/_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_receiver/_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_receiver/stream_receiver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.193540 bsl-0.6.0/bsl/stream_recorder/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_recorder/stream_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.193540 bsl-0.6.0/bsl/stream_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_viewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.193540 bsl-0.6.0/bsl/stream_viewer/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_viewer/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_viewer/backends/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_viewer/backends/pyqtgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.197540 bsl-0.6.0/bsl/stream_viewer/control_gui/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_viewer/control_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_viewer/control_gui/_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_viewer/control_gui/_ui_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    13565 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_viewer/control_gui/control_eeg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.197540 bsl-0.6.0/bsl/stream_viewer/control_gui/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_viewer/control_gui/settings/settings_scope_eeg.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.197540 bsl-0.6.0/bsl/stream_viewer/scope/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_viewer/scope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_viewer/scope/_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_viewer/scope/scope_eeg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/stream_viewer/stream_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.197540 bsl-0.6.0/bsl/triggers/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/triggers/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.201540 bsl-0.6.0/bsl/triggers/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/triggers/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/triggers/io/_dlportio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/triggers/io/_inpout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/triggers/io/_linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/triggers/lsl.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/triggers/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/triggers/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/triggers/trigger_def.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.201540 bsl-0.6.0/bsl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/utils/_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/utils/_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/utils/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/utils/_fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/utils/_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/utils/_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/utils/find_event_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/utils/lsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-05 14:26:19.000000 bsl-0.6.0/bsl/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:27:03.177540 bsl-0.6.0/bsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-05 14:27:03.000000 bsl-0.6.0/bsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-05 14:27:03.000000 bsl-0.6.0/bsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:27:03.000000 bsl-0.6.0/bsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-05 14:27:03.000000 bsl-0.6.0/bsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-05 14:27:03.000000 bsl-0.6.0/bsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 14:27:03.000000 bsl-0.6.0/bsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-05 14:26:19.000000 bsl-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:27:03.205540 bsl-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:26:19.000000 bsl-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.208124 bsl-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-09 10:58:20.000000 bsl-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-09 10:59:18.208124 bsl-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-09 10:58:20.000000 bsl-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.196124 bsl-0.6.1/bsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.196124 bsl-0.6.1/bsl/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/commands/bsl_stream_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/commands/bsl_stream_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/commands/bsl_stream_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/commands/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/commands/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.196124 bsl-0.6.1/bsl/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/datasets/_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/datasets/eeg_auditory_stimuli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/datasets/eeg_resting_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/datasets/eeg_resting_state_short.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/datasets/trigger_def.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.196124 bsl-0.6.1/bsl/lsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.204124 bsl-0.6.1/bsl/lsl/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   923264 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/lib/liblsl-1.16.0-20.04_amd64.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1115480 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/lib/liblsl-1.16.0-22.04_amd64.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   812312 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/lib/liblsl-1.16.0-OSX_amd64.dylib
+-rwxr-xr-x   0 runner    (1001) docker     (123)   758048 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/lib/liblsl-1.16.0-OSX_arm64.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)   803840 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/lib/liblsl-1.16.0-Win_amd64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   598528 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/lib/liblsl-1.16.0-Win_i386.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/load_liblsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11882 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/stream_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/stream_inlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/stream_outlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/lsl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.204124 bsl-0.6.1/bsl/stream_player/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_player/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_player/stream_player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.204124 bsl-0.6.1/bsl/stream_receiver/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_receiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_receiver/_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_receiver/_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_receiver/stream_receiver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.204124 bsl-0.6.1/bsl/stream_recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_recorder/stream_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.204124 bsl-0.6.1/bsl/stream_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_viewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.204124 bsl-0.6.1/bsl/stream_viewer/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_viewer/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_viewer/backends/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_viewer/backends/pyqtgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.208124 bsl-0.6.1/bsl/stream_viewer/control_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_viewer/control_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_viewer/control_gui/_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_viewer/control_gui/_ui_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13565 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_viewer/control_gui/control_eeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.208124 bsl-0.6.1/bsl/stream_viewer/control_gui/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_viewer/control_gui/settings/settings_scope_eeg.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.208124 bsl-0.6.1/bsl/stream_viewer/scope/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_viewer/scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_viewer/scope/_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_viewer/scope/scope_eeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/stream_viewer/stream_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.208124 bsl-0.6.1/bsl/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/triggers/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.208124 bsl-0.6.1/bsl/triggers/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/triggers/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/triggers/io/_dlportio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/triggers/io/_inpout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/triggers/io/_linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/triggers/lsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/triggers/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/triggers/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/triggers/trigger_def.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.208124 bsl-0.6.1/bsl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/utils/_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/utils/_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/utils/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/utils/_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/utils/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/utils/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/utils/find_event_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/utils/lsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-09 10:58:20.000000 bsl-0.6.1/bsl/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:59:18.196124 bsl-0.6.1/bsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-09 10:59:18.000000 bsl-0.6.1/bsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-09 10:59:18.000000 bsl-0.6.1/bsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:59:18.000000 bsl-0.6.1/bsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-09 10:59:18.000000 bsl-0.6.1/bsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-09 10:59:18.000000 bsl-0.6.1/bsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-09 10:59:18.000000 bsl-0.6.1/bsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-09 10:58:20.000000 bsl-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:59:18.208124 bsl-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:58:20.000000 bsl-0.6.1/setup.py
```

### Comparing `bsl-0.6.0/LICENSE` & `bsl-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/PKG-INFO` & `bsl-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsl
-Version: 0.6.0
+Version: 0.6.1
 Summary: Real-time framework for online neuroscience research through LSL-compatible devices.
 Author-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>, Arnaud Desvachez <arnaud.desvachez@gmail.com>, Kyuhwa Lee <lee.kyuh@gmail.com>
 Maintainer-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 License: MIT License
         
         Copyright (c) 2022 Mathieu Scheltienne
```

### Comparing `bsl-0.6.0/README.md` & `bsl-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/commands/bsl_stream_player.py` & `bsl-0.6.1/bsl/commands/bsl_stream_player.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/commands/bsl_stream_recorder.py` & `bsl-0.6.1/bsl/commands/bsl_stream_recorder.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/commands/bsl_stream_viewer.py` & `bsl-0.6.1/bsl/commands/bsl_stream_viewer.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/commands/main.py` & `bsl-0.6.1/bsl/commands/main.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/datasets/_fetching.py` & `bsl-0.6.1/bsl/datasets/_fetching.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/datasets/eeg_auditory_stimuli.py` & `bsl-0.6.1/bsl/datasets/eeg_auditory_stimuli.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/datasets/eeg_resting_state.py` & `bsl-0.6.1/bsl/datasets/eeg_resting_state.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/datasets/eeg_resting_state_short.py` & `bsl-0.6.1/bsl/datasets/eeg_resting_state_short.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/datasets/trigger_def.py` & `bsl-0.6.1/bsl/datasets/trigger_def.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/lsl/__init__.py` & `bsl-0.6.1/bsl/lsl/__init__.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/lsl/constants.py` & `bsl-0.6.1/bsl/lsl/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import numpy as np
 
 from .load_liblsl import lib
 
 # -----------------
 # Supported formats
 # -----------------
-# Value formats supported by LSL. LSL data streams are sequences of samples,
-# each of which is a same-size vector of values with one of the below types.
+# Value formats supported by LSL. LSL data streams are sequences of samples, each of
+# which is a same-size vector of values with one of the below types.
 
 string2fmt = {
     "float32": c_float,
     "float64": c_double,
     "string": c_char_p,
     "int8": c_byte,
     "int16": c_short,
```

### Comparing `bsl-0.6.0/bsl/lsl/functions.py` & `bsl-0.6.1/bsl/lsl/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,16 @@
     version : int
         Version of the binary LSL library.
         The major version is version // 100.
         The minor version is version % 100.
 
     Notes
     -----
-    Clients with different minor versions are protocol-compatible with each
-    other, while clients with different major versions will refuse to work
-    together.
+    Clients with different minor versions are protocol-compatible with each other, while
+    clients with different major versions will refuse to work together.
     """
     return lib.lsl_protocol_version()
 
 
 def local_clock() -> float:
     """Obtain a local system timestamp in seconds.
 
@@ -54,49 +53,48 @@
     name: Optional[str] = None,
     stype: Optional[str] = None,
     source_id: Optional[str] = None,
     minimum: int = 1,
 ) -> List[_BaseStreamInfo]:
     """Resolve streams on the network.
 
-    This function returns all currently available streams from any outlet on
-    the network. The network is usually the subnet specified at the local
-    router, but may also include a group of machines visible to each other via
-    multicast packets (given that the network supports it), or list of
-    hostnames. These details may optionally be customized by the experimenter
-    in a configuration file (see Network Connectivity in the LSL wiki).
+    This function returns all currently available streams from any outlet on the
+    network. The network is usually the subnet specified at the local router, but may
+    also include a group of machines visible to each other via multicast packets (given
+    that the network supports it), or list of hostnames. These details may optionally be
+    customized by the experimenter in a configuration file (see Network Connectivity in
+    the LSL wiki).
 
     Parameters
     ----------
     timeout : float
         Timeout (in seconds) of the operation. If this is too short (e.g.
-        ``< 0.5 seconds``) only a subset (or none) of the outlets that are
-        present on the network may be returned.
+        ``< 0.5 seconds``) only a subset (or none) of the outlets that are present on
+        the network may be returned.
     name : str | None
         Restrict the selected streams to this name.
     stype : str | None
         Restrict the selected stream to this type.
     source_id : str | None
         Restrict the selected stream to this source ID.
     minimum : int
-        Minimum number of stream to return where restricting the selection. As
-        soon as this minimum is hit, the search will end.
+        Minimum number of stream to return where restricting the selection. As soon as
+        this minimum is hit, the search will end.
 
     Returns
     -------
     sinfos : list
-        List of `~bsl.lsl.StreamInfo` objects found on the network.
-        While a `~bsl.lsl.StreamInfo` is not bound to an Inlet, the description
-        field remains empty.
+        List of `~bsl.lsl.StreamInfo` objects found on the network. While a
+        `~bsl.lsl.StreamInfo` is not bound to an Inlet, the description field remains
+        empty.
 
     Notes
     -----
-    If multiple restrinction are provided, the network must be queried once for
-    each restriction. Thus, the true timeout is multiplied by the non ``None``
-    restrictions.
+    If multiple restrinction are provided, the network must be queried once for each
+    restriction. Thus, the true timeout is multiplied by the non ``None`` restrictions.
     """
     check_type(timeout, ("numeric",), "timeout")
     if timeout <= 0:
         raise ValueError(
             "The argument 'timeout' must be a strictly positive integer. "
             f"{timeout} is invalid."
         )
```

### Comparing `bsl-0.6.0/bsl/lsl/lib/liblsl-1.16.0-20.04_amd64.so` & `bsl-0.6.1/bsl/lsl/lib/liblsl-1.16.0-20.04_amd64.so`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/lsl/lib/liblsl-1.16.0-22.04_amd64.so` & `bsl-0.6.1/bsl/lsl/lib/liblsl-1.16.0-22.04_amd64.so`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/lsl/lib/liblsl-1.16.0-OSX_amd64.dylib` & `bsl-0.6.1/bsl/lsl/lib/liblsl-1.16.0-OSX_amd64.dylib`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/lsl/lib/liblsl-1.16.0-OSX_arm64.dylib` & `bsl-0.6.1/bsl/lsl/lib/liblsl-1.16.0-OSX_arm64.dylib`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/lsl/lib/liblsl-1.16.0-Win_amd64.dll` & `bsl-0.6.1/bsl/lsl/lib/liblsl-1.16.0-Win_amd64.dll`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/lsl/lib/liblsl-1.16.0-Win_i386.dll` & `bsl-0.6.1/bsl/lsl/lib/liblsl-1.16.0-Win_i386.dll`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/lsl/load_liblsl.py` & `bsl-0.6.1/bsl/lsl/load_liblsl.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,66 +46,65 @@
 
 def _find_liblsl_env() -> Optional[CDLL]:
     """Search for the LSL library in the environment variable LSL_LIB.
 
     Returns
     -------
     lib : CDLL | None
-        Loaded binary LSL library. None if the value retrieved in the
-        environment variable was not valid or yielded an invalid library.
+        Loaded binary LSL library. None if the value retrieved in the environment
+        variable was not valid or yielded an invalid library.
     """
     if "LSL_LIB" not in os.environ:
         return None
 
     libpath = Path(os.environ["LSL_LIB"])
     if libpath.suffix != _PLATFORM_SUFFIXES[platform.system()]:
         logger.error(
-            "The LIBLSL '%s' provided in the environment variable "
-            "'LSL_LIB' ends with '%s' which is different from the expected "
-            "extension for this OS.",
+            "The LIBLSL '%s' provided in the environment variable 'LSL_LIB' ends with "
+            "'%s' which is different from the expected extension for this OS.",
             libpath,
             libpath.suffix,
         )
         return None
     if libpath.exists():
         libpath, version = _attempt_load_liblsl(libpath)
         if version is None:
             logger.error(
-                "The LIBLSL '%s' provided in the environment variable "
-                "'LSL_LIB' can not be loaded.",
+                "The LIBLSL '%s' provided in the environment variable 'LSL_LIB' can "
+                "not be loaded.",
                 libpath,
             )
         elif version < _VERSION_MIN:
             logger.error(
-                "The LIBLSL '%s' provided in the environment variable "
-                "'LSL_LIB' is outdated. The version is %i.%i while the "
-                "minimum version required by BSL is %i.%i.",
+                "The LIBLSL '%s' provided in the environment variable 'LSL_LIB' is "
+                "outdated. The version is %i.%i while the minimum version required by "
+                "BSL is %i.%i.",
                 libpath,
                 version // 100,
                 version % 100,
                 _VERSION_MIN // 100,
                 _VERSION_MIN % 100,
             )
             version = None
         elif _VERSION_MAX < version:
             logger.warning(
-                "The LIBLSL '%s' provided in the environment variable "
-                "'LSL_LIB' is not officially supported. The version is %i.%i "
-                "while the maximum supported version required by BSL is "
-                "%i.%i. Use this version at your own risk.",
+                "The LIBLSL '%s' provided in the environment variable 'LSL_LIB' is not "
+                "officially supported. The version is %i.%i while the maximum "
+                "supported version required by BSL is %i.%i. Use this version at your "
+                "own risk.",
                 libpath,
                 version // 100,
                 version % 100,
                 _VERSION_MIN // 100,
                 _VERSION_MIN % 100,
             )
     else:
         logger.error(
-            "The LIBLSL path '%s' provided in the environment variable "
-            "'LSL_LIB' does not exists.",
+            "The LIBLSL path '%s' provided in the environment variable 'LSL_LIB' does "
+            "not exists.",
             libpath,
         )
         libpath = None
         version = None
     if version is not None:
         assert libpath is not None  # sanity-check
         lib = CDLL(libpath)
@@ -160,26 +159,25 @@
                 if elt in _SUPPORTED_DISTRO:
                     distro_like = elt
                     break
             else:
                 raise RuntimeError(
                     "The liblsl library packaged with BSL supports "
                     f"{', '.join(_SUPPORTED_DISTRO)} based distributions. "
-                    f"{distro.name()} is not supported. Please build the "
-                    "liblsl library from source and provide it in the "
-                    "environment variable LSL_LIB."
+                    f"{distro.name()} is not supported. Please build the liblsl "
+                    "library from source and provide it in the environment variable "
+                    "LSL_LIB."
                 )
         if distro.version() not in _SUPPORTED_DISTRO[distro_like]:
             raise RuntimeError(
                 "The liblsl library packaged with BSL supports distro_like "
                 "based distributions on versions "
                 f"{', '.join(_SUPPORTED_DISTRO[distro_like])}. Version "
-                f"{distro.version()} is not supported. Please build the "
-                "liblsl library from source and provide it in the environment "
-                "variable LSL_LIB."
+                f"{distro.version()} is not supported. Please build the liblsl library "
+                "from source and provide it in the environment variable LSL_LIB."
             )
         libname += f"{distro.version()}_amd64.so"
 
     # check macOS intel vs arm
     elif platform.system() == "Darwin":
         if platform.processor() == "arm":
             libname += "OSX_arm64.dylib"
@@ -328,16 +326,16 @@
         )
     try:
         lib.lsl_create_continuous_resolver.restype = c_void_p
         lib.lsl_create_continuous_resolver_bypred.restype = c_void_p
         lib.lsl_create_continuous_resolver_byprop.restype = c_void_p
     except Exception:
         logger.info(
-            "[LIBLSL] Continuous resolver functions not available in your "
-            "liblsl version."
+            "[LIBLSL] Continuous resolver functions not available in your liblsl "
+            "version."
         )
 
     return lib
 
 
 # load library
 lib = load_liblsl()
```

### Comparing `bsl-0.6.0/bsl/lsl/stream_info.py` & `bsl-0.6.1/bsl/lsl/stream_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 
 class _BaseStreamInfo:
     """Base Stream information object, storing the declaration of a stream.
 
     A StreamInfo contains the following information:
 
-    * Core information (name, number of channels, sampling frequency, channel
-      format, ...)
-    * Optional metadata about the stream content (channel labels, measurement
-      units, ...)
+    * Core information (name, number of channels, sampling frequency, channel format,
+      ...)
+    * Optional metadata about the stream content (channel labels, measurement units,
+      ...)
     * Hosting information (uID, hostname, ...) if bound to an inlet or outlet
     """
 
     def __init__(self, obj):
         self._obj = c_void_p(obj)
         if not self._obj:
             raise RuntimeError(
@@ -109,26 +109,26 @@
         """
         return fmt2string[self._dtype]
 
     @property
     def name(self) -> str:
         """Name of the stream.
 
-        The name of the stream is defined by the application creating the LSL
-        outlet. Streams with identical names can coexist, at the cost of
-        ambiguity for the recording application and/or the experimenter.
+        The name of the stream is defined by the application creating the LSL outlet.
+        Streams with identical names can coexist, at the cost of ambiguity for the
+        recording application and/or the experimenter.
         """
         return lib.lsl_get_name(self._obj).decode("utf-8")
 
     @property
     def n_channels(self) -> int:
         """Number of channels.
 
-        A stream must have at least one channel. The number of channels remains
-        constant for all samples.
+        A stream must have at least one channel. The number of channels remains constant
+        for all samples.
         """
         return lib.lsl_get_channel_count(self._obj)
 
     @property
     def sfreq(self) -> float:
         """Sampling rate of the stream, according to the source (in Hz).
 
@@ -136,154 +136,150 @@
         """
         return lib.lsl_get_nominal_srate(self._obj)
 
     @property
     def source_id(self) -> str:
         """Unique identifier of the stream's source.
 
-        The unique source (or device) identifier is an optional piece of
-        information that, if available, allows endpoints (such as the recording
-        program) to re-acquire a stream automatically once if it came back
-        online.
+        The unique source (or device) identifier is an optional piece of information
+        that, if available, allows endpoints (such as the recording program) to
+        re-acquire a stream automatically once if it came back online.
         """
         return lib.lsl_get_source_id(self._obj).decode("utf-8")
 
     @property
     def stype(self) -> str:
         """Type of the stream.
 
-        The content type is a short string, such as ``"EEG"``, ``"Gaze"``, ...
-        which describes the content carried by the channel. If a stream
-        contains mixed content, this value should be an empty string and the
-        type should be stored in the description of individual channels.
+        The content type is a short string, such as ``"EEG"``, ``"Gaze"``, ... which
+        describes the content carried by the channel. If a stream contains mixed
+        content, this value should be an empty string and the type should be stored in
+        the description of individual channels.
         """
         return lib.lsl_get_type(self._obj).decode("utf-8")
 
     # -- Hosting information, assigned when bound to an outlet/inlet ----------
     @property
     def created_at(self) -> float:
         """Timestamp at which the stream was created.
 
-        This is the time stamps at which the stream was first created, as
-        determined by `~bsl.lsl.local_clock` on the providing machine.
+        This is the time stamps at which the stream was first created, as determined by
+        `~bsl.lsl.local_clock` on the providing machine.
         """
         return lib.lsl_get_created_at(self._obj)
 
     @property
     def hostname(self) -> str:
         """Hostname of the providing machine."""
         return lib.lsl_get_hostname(self._obj).decode("utf-8")
 
     @property
     def session_id(self) -> str:
         """Session ID for the given stream.
 
-        The session ID is an optional human-assigned identifier of the
-        recording session. While it is rarely used, it can be used to prevent
-        concurrent recording activities on the same sub-network (e.g., in
-        multiple experiment areas) from seeing each other's streams
-        (can be assigned in a configuration file read by liblsl, see also
-        Network Connectivity in the LSL wiki).
+        The session ID is an optional human-assigned identifier of the recording
+        session. While it is rarely used, it can be used to prevent concurrent recording
+        activities on the same sub-network (e.g., in multiple experiment areas) from
+        seeing each other's streams (can be assigned in a configuration file read by
+        liblsl, see also Network Connectivity in the LSL wiki).
         """
         return lib.lsl_get_session_id(self._obj).decode("utf-8")
 
     @property
     def uid(self) -> str:
         """Unique ID of the `~bsl.lsl.StreamOutlet` instance.
 
-        This ID is guaranteed to be different across multiple instantiations of
-        the same ~bsl.lsl.StreamOutlet`, e.g. after a re-start.
+        This ID is guaranteed to be different across multiple instantiations of the same
+        `~bsl.lsl.StreamOutlet`, e.g. after a re-start.
         """
         return lib.lsl_get_uid(self._obj).decode("utf-8")
 
     @property
     def protocol_version(self) -> int:
         """Version of the LSL protocol.
 
-        The major version is version // 100.
-        The minor version is version % 100.
+        The major version is ``version // 100``.
+        The minor version is ``version % 100``.
         """
         return lib.lsl_get_version(self._obj)
 
     # -- Data description -----------------------------------------------------
     @property
     def as_xml(self) -> str:
         """Retrieve the entire stream_info in XML format.
 
-        This yields an XML document (in string form) whose top-level element is
-        <info>. The info element contains one element for each field of the
+        This yields an XML document (in string form) whose top-level element is <info>.
+        The info element contains one element for each field of the
         `~bsl.lsl.StreamInfo` class, including:
 
-        * the core elements <name>, <type>, <channel_count>, <nominal_srate>,
-          <channel_format>, <source_id>
-        * the misc elements <version>, <created_at>, <uid>, <session_id>,
-          <v4address>, <v4data_port>, <v4service_port>, <v6address>,
-          <v6data_port>, <v6service_port>
-        * the extended description element <desc> with user-defined
-          sub-elements.
+        * the core elements ``name``, ``type`` (eq. ``stype``), ``channel_count``
+          (eq. ``n_channels``), ``nominal_srate`` (eq. ``sfreq``), ``channel_format``
+          (eq. ``dtype``), ``source_id``
+        * the misc elements ``version``, ``created_at``, ``uid``, ``session_id``,
+          ``v4address``, ``v4data_port``, ``v4service_port``, ``v6address``,
+          ``v6data_port``, ``v6service_port``
+        * the extended description element ``desc`` with user-defined sub-elements.
         """
         return lib.lsl_get_xml(self._obj).decode("utf-8")
 
     @property
     def desc(self) -> XMLElement:
         """Extended description of the stream.
 
-        It is highly recommended that at least the channel labels are described
-        here. See code examples on the LSL wiki. Other information, such
-        as amplifier settings, measurement units if deviating from defaults,
-        setup information, subject information, etc.. can be specified here, as
-        well. Meta-data recommendations follow the XDF file format project
-        (github.com/sccn/xdf/wiki/Meta-Data or web search for: XDF meta-data).
-
-        Important: if you use a stream content type for which meta-data
-        recommendations exist, please try to lay out your meta-data in
-        agreement with these recommendations for compatibility with other
-        applications.
+        It is highly recommended that at least the channel labels are described here.
+        See code examples on the LSL wiki. Other information, such as amplifier
+        settings, measurement units if deviating from defaults, setup information,
+        subject information, etc.. can be specified here, as well. Meta-data
+        recommendations follow the `XDF file format project`_.
+
+        Important: if you use a stream content type for which meta-data recommendations
+        exist, please try to lay out your meta-data in agreement with these
+        recommendations for compatibility with other applications.
+
+        .. _XDF file format project: https://github.com/sccn/xdf/wiki/Meta-Data
         """
         return XMLElement(lib.lsl_get_desc(self._obj))
 
 
 class StreamInfo(_BaseStreamInfo):
     """Base Stream information object, storing the declaration of a stream.
 
     A StreamInfo contains the following information:
 
-    * Core information (name, number of channels, sampling frequency, channel
-      format, ...)
-    * Optional metadata about the stream content (channel labels, measurement
-      units, ...)
-    * Hosting information (uID, hostname, ...) if bound to an
-      `~bsl.lsl.StreamInlet` or `~bsl.lsl.StreamOutlet`
+    * Core information (name, number of channels, sampling frequency, channel format,
+      ...)
+    * Optional metadata about the stream content (channel labels, measurement units,
+      ...)
+    * Hosting information (uID, hostname, ...) if bound to an `~bsl.lsl.StreamInlet` or
+      `~bsl.lsl.StreamOutlet`
 
     Parameters
     ----------
     name : str
         Name of the stream. This field can not be empty.
     stype : str
-        Content type of the stream, e.g. ``"EEG"`` or ``"Gaze"``. If a stream
-        contains mixed content, this value should be empty and the description
-        of each channel should include its type.
+        Content type of the stream, e.g. ``"EEG"`` or ``"Gaze"``. If a stream contains
+        mixed content, this value should be empty and the description of each channel
+        should include its type.
     n_channels : int ``≥ 1``
-        Also called ``channel_count``, represents the number of channels per
-        sample. This number stays constant for the lifetime of the stream.
+        Also called ``channel_count``, represents the number of channels per sample.
+        This number stays constant for the lifetime of the stream.
     sfreq : float ``≥ 0``
         Also called ``nominal_srate``, represents the sampling rate (in Hz) as
-        advertised by the data source. If the sampling rate is irregular (e.g.
-        for a trigger stream), the sampling rate is set to ``0``.
+        advertised by the data source. If the sampling rate is irregular (e.g. for a
+        trigger stream), the sampling rate is set to ``0``.
     dtype : str
-        Format of each channel. If your channels have different formats,
-        consider supplying multiple streams or use the largest type that can
-        hold them all.
+        Format of each channel. If your channels have different formats, consider
+        supplying multiple streams or use the largest type that can hold them all.
         One of ``('string', 'float32', 'float64', 'int8', 'int16', 'int32')``.
         ``'int64'`` is partially supported.
     source_id : str
-        A unique identifier of the device or source of the data. If not empty,
-        this information improves the system robustness since it allows
-        recipients to recover from failure by finding a stream with the same
-        ``source_id`` on the network.
+        A unique identifier of the device or source of the data. If not empty, this
+        information improves the system robustness since it allows recipients to recover
+        from failure by finding a stream with the same ``source_id`` on the network.
     """
 
     def __init__(
         self,
         name: str,
         stype: str,
         n_channels: int,
@@ -292,16 +288,16 @@
         source_id: str,
     ):
         check_type(name, (str,), "name")
         check_type(stype, (str,), "stype")
         n_channels = ensure_int(n_channels, "n_channels")
         if n_channels <= 0:
             raise ValueError(
-                "The number of channels 'n_channels' must be a strictly "
-                f"positive integer. {n_channels} is invalid."
+                "The number of channels 'n_channels' must be a strictly positive "
+                f"integer. {n_channels} is invalid."
             )
         check_type(sfreq, ("numeric",), "sfreq")
         check_type(source_id, (str,), "source_id")
 
         obj = lib.lsl_create_streaminfo(
             c_char_p(str.encode(name)),
             c_char_p(str.encode(stype)),
```

### Comparing `bsl-0.6.0/bsl/lsl/stream_inlet.py` & `bsl-0.6.1/bsl/lsl/stream_inlet.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,27 +22,26 @@
     """An inlet to retrieve data and metadata on the network.
 
     Parameters
     ----------
     sinfo : StreamInfo
         Description of the stream to connect to.
     chunk_size : int ``≥ 1`` | ``0``
-        The desired chunk granularity in samples. By default, the
-        ``chunk_size`` defined by the sender (outlet) is used.
+        The desired chunk granularity in samples. By default, the ``chunk_size`` defined
+        by the sender (outlet) is used.
     max_buffered : float ``≥ 0``
-        The maximum amount of data to buffer in the Outlet.
-        The number of samples buffered is ``max_buffered * 100`` if the
-        sampling rate is irregular, else it's ``max_buffered`` seconds.
+        The maximum amount of data to buffer in the Outlet. The number of samples
+        buffered is ``max_buffered * 100`` if the sampling rate is irregular, else it's
+        ``max_buffered`` seconds.
     recover : bool
-        Attempt to silently recover lost streams that are recoverable (requires
-        a ``source_id`` to be specified in the `~bsl.lsl.StreamInfo`).
+        Attempt to silently recover lost streams that are recoverable (requires a
+        ``source_id`` to be specified in the `~bsl.lsl.StreamInfo`).
     processing_flags : list of str | ``'all'`` | None
-        Set the post-processing options. By default, post-processing is
-        disabled. Any combination of the processing flags is valid. The
-        available flags are:
+        Set the post-processing options. By default, post-processing is disabled. Any
+        combination of the processing flags is valid. The available flags are:
 
         * ``'clocksync'``: Automatic clock synchronization, equivalent to
           manually adding the estimated `~bsl.lsl.StreamInlet.time_correction`.
         * ``'dejitter'``: Remove jitter on the received timestamps with a
           smoothing algorithm.
         * ``'monotize'``: Force the timestamps to be monotically ascending.
           This option should not be enable if ``'dejitter'`` is not enabled.
@@ -87,14 +86,17 @@
                     lambda x, y: x | y, post_processing_flags.values()
                 )
             else:
                 for flag in processing_flags:
                     check_type(flag, (str,), "processing_flag")
                     check_value(flag, post_processing_flags, flag)
                 # bitwise OR between the flags
+                processing_flags = [
+                    post_processing_flags[key] for key in processing_flags
+                ]
                 processing_flags = reduce(lambda x, y: x | y, processing_flags)
             assert processing_flags > 0  # sanity-check
             handle_error(lib.lsl_set_postprocessing(self._obj, processing_flags))
 
         # properties from the StreamInfo
         self._dtype = sinfo._dtype
         self._name = sinfo.name
@@ -117,115 +119,109 @@
             lib.lsl_destroy_inlet(self._obj)
         except Exception:
             pass
 
     def open_stream(self, timeout: Optional[float] = None) -> None:
         """Subscribe to a data stream.
 
-        All samples pushed in at the other end from this moment onwards will be
-        queued and eventually be delivered in response to
-        `~bsl.lsl.StreamInlet.pull_sample` or `~bsl.lsl.StreamInlet.pull_chunk`
-        calls. Pulling a sample without subscribing to the stream with this
-        method is permitted (the stream will be opened implicitly).
+        All samples pushed in at the other end from this moment onwards will be queued
+        and eventually be delivered in response to `~bsl.lsl.StreamInlet.pull_sample` or
+        `~bsl.lsl.StreamInlet.pull_chunk` calls. Pulling a sample without subscribing to
+        the stream with this method is permitted (the stream will be opened implicitly).
 
         Parameters
         ----------
         timeout : float | None
-            Optional timeout (in seconds) of the operation. By default, timeout
-            is disabled.
+            Optional timeout (in seconds) of the operation. By default, timeout is
+            disabled.
 
         Notes
         -----
-        Opening a stream is a non-blocking operation. Thus, samples pushed on
-        an outlet while the stream is not yet open will be missed.
+        Opening a stream is a non-blocking operation. Thus, samples pushed on an outlet
+        while the stream is not yet open will be missed.
         """
         timeout = _check_timeout(timeout)
         errcode = c_int()
         lib.lsl_open_stream(self._obj, c_double(timeout), byref(errcode))
         handle_error(errcode)
         # block a bit longer because of a bug in liblsl
         # this sleep can be removed once the minimum version supported includes
         # a fix for https://github.com/sccn/liblsl/issues/176
         time.sleep(0.5)
 
     def close_stream(self) -> None:
         """Drop the current data stream.
 
         All samples that are still buffered or in flight will be dropped and
-        transmission and buffering of data for this inlet will be stopped.
-        This method is used if an application stops being interested in data
-        from a source (temporarily or not) but keeps the outlet alive, to not
-        waste unnecessary system and network resources.
+        transmission and buffering of data for this inlet will be stopped. This method
+        is used if an application stops being interested in data from a source
+        (temporarily or not) but keeps the outlet alive, to not waste unnecessary system
+        and network resources.
 
         .. warning::
 
             At the moment, ``liblsl`` is released in version 1.16. Closing and
-            re-opening a stream does not work and new samples pushed to the
-            outlet do not arrive at the inlet. c.f. this
+            re-opening a stream does not work and new samples pushed to the outlet do
+            not arrive at the inlet. c.f. this
             `github issue <https://github.com/sccn/liblsl/issues/180>`_.
         """
         lib.lsl_close_stream(self._obj)
 
     def time_correction(self, timeout: Optional[float] = None) -> float:
         """Retrieve an estimated time correction offset for the given stream.
 
-        The first call to this function takes several milliseconds until a
-        reliable first estimate is obtained. Subsequent calls are instantaneous
-        (and rely on periodic background updates). The precision of these
-        estimates should be below 1 ms (empirically within +/-0.2 ms).
+        The first call to this function takes several milliseconds until a reliable
+        first estimate is obtained. Subsequent calls are instantaneous (and rely on
+        periodic background updates). The precision of these estimates should be below
+        1 ms (empirically within +/-0.2 ms).
 
         Parameters
         ----------
         timeout : float | None
-            Optional timeout (in seconds) of the operation. By default, timeout
-            is disabled.
+            Optional timeout (in seconds) of the operation. By default, timeout is
+            disabled.
 
         Returns
         -------
         time_correction : float
-            Current estimate of the time correction. This number needs to be
-            added to a timestamp that was remotely generated via
-            ``local_clock()`` to map it into the local clock domain of the
-            client machine.
+            Current estimate of the time correction. This number needs to be added to a
+            timestamp that was remotely generated via ``local_clock()`` to map it into
+            the local clock domain of the client machine.
         """
         timeout = _check_timeout(timeout)
         errcode = c_int()
         result = lib.lsl_time_correction(self._obj, c_double(timeout), byref(errcode))
         handle_error(errcode)
         return result
 
     def pull_sample(self, timeout: Optional[float] = 0.0):
         """Pull a single sample from the inlet.
 
         Parameters
         ----------
         timeout : float | None
-            Optional timeout (in seconds) of the operation. None correspond to
-            a very large value, effectively disabling the timeout. ``0.`` makes
-            this function non-blocking even if no sample is available. See
-            notes for additional details.
-            Optional timeout (in seconds) of the operation. By default, timeout
-            is disabled.
+            Optional timeout (in seconds) of the operation. None correspond to a very
+            large value, effectively disabling the timeout. ``0.`` makes this function
+            non-blocking even if no sample is available. See notes for additional
+            details.
 
         Returns
         -------
-        sample : list | array of shape (n_channels,) | None
-            If the channel format is ``'string^``, returns a list of values for
-            each channel. Else, returns a numpy array of shape
-            ``(n_channels,)``.
+        sample : list | array of shape (n_channels,)
+            If the channel format is ``'string``, returns a list of values for each
+            channel. Else, returns a numpy array of shape ``(n_channels,)``.
         timestamp : float | None
-            Acquisition timestamp on the remote machine. To map the timestamp
-            to the local clock of the client machine, add the estimated time
-            correction return by `~bsl.lsl.StreamInlet.time_correction`.
-            None if no sample was retrieved.
+            Acquisition timestamp on the remote machine. To map the timestamp to the
+            local clock of the client machine, add the estimated time correction return
+            by `~bsl.lsl.StreamInlet.time_correction`. None if no sample was retrieved.
 
         Notes
         -----
-        Note that if ``timeout`` is reached and no sample is available, empty
-        ``sample`` arrays is returned.
+        Note that if ``timeout`` is reached and no sample is available, an empty
+        ``sample`` is returned and ``timestamp`` is set to None.
         """
         timeout = _check_timeout(timeout)
 
         errcode = c_int()
         timestamp = self._do_pull_sample(
             self._obj,
             byref(self._buffer_data[1]),
@@ -238,55 +234,53 @@
         if timestamp:
             if self._dtype == c_char_p:
                 sample = [v.decode("utf-8") for v in self._buffer_data[1]]
                 _free_char_p_array_memory(self._buffer_data[1])
             else:
                 sample = np.frombuffer(self._buffer_data[1], dtype=self._dtype)
         else:
-            sample = None
+            sample = [] if self._dtype == c_char_p else np.empty(0, dtype=self._dtype)
             timestamp = None
         return sample, timestamp
 
     def pull_chunk(
         self,
         timeout: Optional[float] = 0.0,
         max_samples: int = 1024,
     ):
         """Pull a chunk of samples from the inlet.
 
         Parameters
         ----------
         timeout : float | None
-            Optional timeout (in seconds) of the operation. None correspond to
-            a very large value, effectively disabling the timeout. ``0.`` makes
-            this function non-blocking even if no sample is available. See
-            notes for additional details.
+            Optional timeout (in seconds) of the operation. None correspond to a very
+            large value, effectively disabling the timeout. ``0.`` makes this function
+            non-blocking even if no sample is available. See notes for additional
+            details.
         max_samples : int
-            Maximum number of samples to return. The function is blocking until
-            this number of samples is available or until ``timeout`` is
-            reached. See notes for additional details.
+            Maximum number of samples to return. The function is blocking until this
+            number of samples is available or until ``timeout`` is reached. See notes
+            for additional details.
 
         Returns
         -------
-        samples : list of list | array of shape (n_samples, n_channels) | None
-            If the channel format is ``'string'``, returns a list of list of
-            values for each channel and sample. Each sublist represents an
-            entire channel. Else, returns a numpy array of shape
-            ``(n_samples, n_channels)``.
-        timestamps : array of shape (n_samples,) | None
+        samples : list of list | array of shape (n_samples, n_channels)
+            If the channel format is ``'string'``, returns a list of list of values for
+            each channel and sample. Each sublist represents an entire channel. Else,
+            returns a numpy array of shape ``(n_samples, n_channels)``.
+        timestamps : array of shape (n_samples,)
             Acquisition timestamps on the remote machine.
 
         Notes
         -----
-        The argument ``timeout`` and ``max_samples`` control the blocking
-        behavior of the pull operation. If the number of available sample is
-        inferior to ``n_samples``, the pull operation is blocking until
-        ``timeout`` is reached. Thus, to return all the available samples at a
-        given time, regardless of the number of samples requested, ``timeout``
-        must be set to ``0``.
+        The argument ``timeout`` and ``max_samples`` control the blocking behavior of
+        the pull operation. If the number of available sample is inferior to
+        ``n_samples``, the pull operation is blocking until ``timeout`` is reached.
+        Thus, to return all the available samples at a given time, regardless of the
+        number of samples requested, ``timeout`` must be set to ``0``.
 
         Note that if ``timeout`` is reached and no sample is available, empty
         ``samples`` and ``timestamps`` arrays are returned.
         """
         timeout = _check_timeout(timeout)
         if not isinstance(max_samples, int):
             max_samples = int(max_samples)
@@ -400,16 +394,16 @@
     # -------------------------------------------------------------------------
     def get_sinfo(self, timeout: Optional[float] = None) -> _BaseStreamInfo:
         """`~bsl.lsl.StreamInfo` corresponding to this Inlet.
 
         Parameters
         ----------
         timeout : float | None
-            Optional timeout (in seconds) of the operation. By default, timeout
-            is disabled.
+            Optional timeout (in seconds) of the operation. By default, timeout is
+            disabled.
 
         Returns
         -------
         sinfo : StreamInfo
             Description of the stream connected to the inlet.
         """
         timeout = _check_timeout(timeout)
```

### Comparing `bsl-0.6.0/bsl/lsl/stream_outlet.py` & `bsl-0.6.1/bsl/lsl/stream_outlet.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,25 +103,23 @@
             x = [v.encode("utf-8") for v in x]
         else:
             assert isinstance(
                 x, np.ndarray
             ), "'x' must be an array if numericals are pushed."
             if x.ndim != 1:
                 raise ValueError(
-                    "The sample to push 'x' must contain one element per "
-                    "channel. Thus, the shape should be (n_channels,), "
-                    f"{x.shape} is invalid."
+                    "The sample to push 'x' must contain one element per channel. "
+                    f"Thus, the shape should be (n_channels,), {x.shape} is invalid."
                 )
             npdtype = fmt2numpy[self._dtype]
             x = x if x.dtype == npdtype else x.astype(npdtype)
         if len(x) != self._n_channels:
             raise ValueError(
-                "The sample to push 'x' must contain one element per channel. "
-                f"Thus, {self._n_channels} elements are expected. {len(x)} "
-                "is invalid."
+                "The sample to push 'x' must contain one element per channel. Thus, "
+                f"{self._n_channels} elements are expected. {len(x)} is invalid."
             )
 
         handle_error(
             self._do_push_sample(
                 self._obj,
                 self._buffer_sample(*x),
                 c_double(timestamp),
@@ -154,30 +152,30 @@
         """
         if self._dtype == c_char_p:
             assert isinstance(x, list), "'x' must be a list if strings are pushed."
             x = [v for sample in x for v in sample]  # flatten
             n_samples = len(x)
             if n_samples % self._n_channels != 0:  # quick incomplete test
                 raise ValueError(
-                    "The samples to push 'x' must contain one element per "
-                    "channel at each time-point. Thus, the shape should be "
-                    "(n_samples, n_channels)."
+                    "The samples to push 'x' must contain one element per channel at "
+                    "each time-point. Thus, the shape should be (n_samples, "
+                    "n_channels)."
                 )
             x = [v.encode("utf-8") for v in x]
             n_samples = len(x)
             data_buffer = (self._dtype * n_samples)(*x)
         else:
             assert isinstance(
                 x, np.ndarray
             ), "'x' must be an array if numericals are pushed."
             if x.ndim != 2 or x.shape[1] != self._n_channels:
                 raise ValueError(
                     "The samples to push 'x' must contain one element per channel at "
-                    "each time-point. Thus, the shape should be "
-                    f"(n_samples, n_channels), {x.shape} is invalid."
+                    "each time-point. Thus, the shape should be (n_samples, "
+                    f"n_channels), {x.shape} is invalid."
                 )
             npdtype = fmt2numpy[self._dtype]
             x = x if x.dtype == npdtype else x.astype(npdtype)
             x = x if x.flags["C_CONTIGUOUS"] else np.ascontiguousarray(x)
             n_samples = x.size
             data_buffer = (self._dtype * n_samples).from_buffer(x)
```

### Comparing `bsl-0.6.0/bsl/lsl/utils.py` & `bsl-0.6.1/bsl/lsl/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from .load_liblsl import lib
 
 
 # -- XML tree -----------------------------------------------------------------
 class XMLElement:
     """A lightweight XML element tree modeling the .desc() field of StreamInfo.
 
-    Has a name and can have multiple named children or have text content as
-    value; attributes are omitted. Insider note: The interface is modeled after
-    a subset of pugixml's node type and is compatible with it. See also
-    http://pugixml.googlecode.com/svn/tags/latest/docs/manual/access.html for
-    additional documentation.
+    Has a name and can have multiple named children or have text content as value;
+    attributes are omitted. Insider note: The interface is modeled after a subset of
+    pugixml's node type and is compatible with it. See also
+    http://pugixml.googlecode.com/svn/tags/latest/docs/manual/access.html for additional
+    documentation.
     """
 
     def __init__(self, handle):
         """Construct a new XML element from existing handle."""
         self.e = c_void_p(handle)
 
     # -- Tree Navigation ------------------------------------------------------
@@ -31,27 +31,25 @@
     def child(self, name):
         """Get a child with a specified name."""
         return XMLElement(lib.lsl_child(self.e, str.encode(name)))
 
     def next_sibling(self, name=None):
         """Get the next sibling in the children list of the parent node.
 
-        If a name is provided, the next sibling with the given name is
-        returned.
+        If a name is provided, the next sibling with the given name is returned.
         """
         if name is None:
             return XMLElement(lib.lsl_next_sibling(self.e))
         else:
             return XMLElement(lib.lsl_next_sibling_n(self.e, str.encode(name)))
 
     def previous_sibling(self, name=None):
         """Get the previous sibling in the children list of the parent node.
 
-        If a name is provided, the previous sibling with the given name is
-        returned.
+        If a name is provided, the previous sibling with the given name is returned.
         """
         if name is None:
             return XMLElement(lib.lsl_previous_sibling(self.e))
         else:
             return XMLElement(lib.lsl_previous_sibling_n(self.e, str.encode(name)))
 
     def parent(self):
@@ -77,35 +75,35 @@
     def value(self):
         """Value of the element."""
         return lib.lsl_value(self.e).decode("utf-8")
 
     def child_value(self, name=None):
         """Get child value (value of the first child that is text).
 
-        If a name is provided, then the value of the first child with the
-        given name is returned.
+        If a name is provided, then the value of the first child with the given name is
+        returned.
         """
         if name is None:
             res = lib.lsl_child_value(self.e)
         else:
             res = lib.lsl_child_value_n(self.e, str.encode(name))
         return res.decode("utf-8")
 
     # -- Modification ---------------------------------------------------------
     def append_child_value(self, name, value):  # noqa: D205, D400
-        """Append a child node with a given name, which has a (nameless)
-        plain-text child with the given text value.
+        """Append a child node with a given name, which has a (nameless) plain-text
+        child with the given text value.
         """
         return XMLElement(
             lib.lsl_append_child_value(self.e, str.encode(name), str.encode(value))
         )
 
     def prepend_child_value(self, name, value):  # noqa: D205, D400
-        """Prepend a child node with a given name, which has a (nameless)
-        plain-text child with the given text value.
+        """Prepend a child node with a given name, which has a (nameless) plain-text
+        child with the given text value.
         """
         return XMLElement(
             lib.lsl_prepend_child_value(self.e, str.encode(name), str.encode(value))
         )
 
     def set_child_value(self, name, value):  # noqa: D205, D400
         """Set the text value of the (nameless) plain-text child of a named
@@ -204,24 +202,23 @@
     ----------
     timeout : float | None
         Timeout (in seconds) or None to disable timeout.
 
     Returns
     -------
     timeout : float
-        Timeout (in seconds). If None was provided, a very large float is
-        provided.
+        Timeout (in seconds). If None was provided, a very large float is returned.
     """
     # with check_type, the execution takes 800-900 ns.
     # with the try/except below, the execution takes 110 ns.
     if timeout is None:
         return 32000000.0  # about 1 year
     try:
         raise_ = timeout < 0
     except Exception:
         raise TypeError("The argument 'timeout' must be a strictly positive number.")
     if raise_:
         raise ValueError(
-            "The argument 'timeout' must be a strictly positive number. "
-            f"{timeout} is invalid."
+            f"The argument 'timeout' must be a strictly positive number. {timeout} is "
+            "invalid."
         )
     return timeout
```

### Comparing `bsl-0.6.0/bsl/stream_player/stream_player.py` & `bsl-0.6.1/bsl/stream_player/stream_player.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/stream_receiver/_buffer.py` & `bsl-0.6.1/bsl/stream_receiver/_buffer.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/stream_receiver/_stream.py` & `bsl-0.6.1/bsl/stream_receiver/_stream.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/stream_receiver/stream_receiver.py` & `bsl-0.6.1/bsl/stream_receiver/stream_receiver.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/stream_recorder/stream_recorder.py` & `bsl-0.6.1/bsl/stream_recorder/stream_recorder.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/stream_viewer/backends/_backend.py` & `bsl-0.6.1/bsl/stream_viewer/backends/_backend.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/stream_viewer/backends/pyqtgraph.py` & `bsl-0.6.1/bsl/stream_viewer/backends/pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/stream_viewer/control_gui/_control.py` & `bsl-0.6.1/bsl/stream_viewer/control_gui/_control.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/stream_viewer/control_gui/_ui_control.py` & `bsl-0.6.1/bsl/stream_viewer/control_gui/_ui_control.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/stream_viewer/control_gui/control_eeg.py` & `bsl-0.6.1/bsl/stream_viewer/control_gui/control_eeg.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/stream_viewer/scope/_scope.py` & `bsl-0.6.1/bsl/stream_viewer/scope/_scope.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/stream_viewer/scope/scope_eeg.py` & `bsl-0.6.1/bsl/stream_viewer/scope/scope_eeg.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/stream_viewer/stream_viewer.py` & `bsl-0.6.1/bsl/stream_viewer/stream_viewer.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/triggers/_base.py` & `bsl-0.6.1/bsl/triggers/_base.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/triggers/io/__init__.py` & `bsl-0.6.1/bsl/triggers/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/triggers/io/_dlportio.py` & `bsl-0.6.1/bsl/triggers/io/_dlportio.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/triggers/io/_inpout.py` & `bsl-0.6.1/bsl/triggers/io/_inpout.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/triggers/io/_linux.py` & `bsl-0.6.1/bsl/triggers/io/_linux.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/triggers/lsl.py` & `bsl-0.6.1/bsl/triggers/lsl.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/triggers/parallel.py` & `bsl-0.6.1/bsl/triggers/parallel.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/triggers/trigger_def.py` & `bsl-0.6.1/bsl/triggers/trigger_def.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/utils/_checks.py` & `bsl-0.6.1/bsl/utils/_checks.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/utils/_docs.py` & `bsl-0.6.1/bsl/utils/_docs.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/utils/_fixes.py` & `bsl-0.6.1/bsl/utils/_fixes.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/utils/_imports.py` & `bsl-0.6.1/bsl/utils/_imports.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/utils/_tests.py` & `bsl-0.6.1/bsl/utils/_tests.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/utils/config.py` & `bsl-0.6.1/bsl/utils/config.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/utils/find_event_channel.py` & `bsl-0.6.1/bsl/utils/find_event_channel.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/utils/io.py` & `bsl-0.6.1/bsl/utils/io.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/utils/logs.py` & `bsl-0.6.1/bsl/utils/logs.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/utils/lsl.py` & `bsl-0.6.1/bsl/utils/lsl.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl/utils/timer.py` & `bsl-0.6.1/bsl/utils/timer.py`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl.egg-info/PKG-INFO` & `bsl-0.6.1/bsl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsl
-Version: 0.6.0
+Version: 0.6.1
 Summary: Real-time framework for online neuroscience research through LSL-compatible devices.
 Author-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>, Arnaud Desvachez <arnaud.desvachez@gmail.com>, Kyuhwa Lee <lee.kyuh@gmail.com>
 Maintainer-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 License: MIT License
         
         Copyright (c) 2022 Mathieu Scheltienne
```

### Comparing `bsl-0.6.0/bsl.egg-info/SOURCES.txt` & `bsl-0.6.1/bsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/bsl.egg-info/requires.txt` & `bsl-0.6.1/bsl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bsl-0.6.0/pyproject.toml` & `bsl-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools >= 61.0.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'bsl'
-version = '0.6.0'
+version = '0.6.1'
 description = 'Real-time framework for online neuroscience research through LSL-compatible devices.'
 readme = 'README.md'
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
 authors = [
     {name = 'Mathieu Scheltienne', email = 'mathieu.scheltienne@fcbg.ch'},
     {name = 'Arnaud Desvachez', email = 'arnaud.desvachez@gmail.com'},
```

