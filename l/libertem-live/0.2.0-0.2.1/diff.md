# Comparing `tmp/libertem-live-0.2.0.tar.gz` & `tmp/libertem-live-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libertem-live-0.2.0.tar", last modified: Fri Apr 21 15:26:24 2023, max compression
+gzip compressed data, was "libertem-live-0.2.1.tar", last modified: Tue May  9 15:11:57 2023, max compression
```

## Comparing `libertem-live-0.2.0.tar` & `libertem-live-0.2.1.tar`

### file list

```diff
@@ -1,170 +1,100 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.436473 libertem-live-0.2.0/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-19 12:20:22.000000 libertem-live-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-19 12:20:22.000000 libertem-live-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4494 2023-04-21 15:26:24.436473 libertem-live-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3229 2023-04-20 17:12:41.000000 libertem-live-0.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.424473 libertem-live-0.2.0/libertem_live/
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-21 15:26:24.424473 libertem-live-0.2.0/libertem_live/_baked_revision.py
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-19 12:20:23.000000 libertem-live-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      512 2023-04-21 15:26:24.436473 libertem-live-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4315 2023-04-21 14:43:24.000000 libertem-live-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.424473 libertem-live-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      353 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      345 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)      349 2023-04-19 17:02:51.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-21 15:24:34.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-20 16:50:56.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/__version__.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)      168 2023-04-20 16:28:19.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/__version__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     7632 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/api.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3882 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/hooks.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     3858 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/hooks.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)     3877 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/hooks.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      513 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/versioning.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      503 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/versioning.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)      513 2023-04-19 17:02:51.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/versioning.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 15:18:29.000000 libertem-live-0.2.0/src/libertem_live/__version__.py
--rw-r--r--   0 root         (0) root         (0)     8951 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/detectors/
--rw-r--r--   0 root         (0) root         (0)     1151 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/LICENSE
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/detectors/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      153 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      147 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)      151 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     5348 2023-04-19 17:20:47.000000 libertem-live-0.2.0/src/libertem_live/detectors/__pycache__/common.cpython-39.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/
--rw-r--r--   0 root         (0) root         (0)      291 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      386 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    12360 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/__pycache__/acquisition.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     6767 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/__pycache__/connection.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     8174 2023-04-19 17:21:07.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/__pycache__/sim.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    13374 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/acquisition.py
--rw-r--r--   0 root         (0) root         (0)     5781 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/connection.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/controller.py
--rw-r--r--   0 root         (0) root         (0)     7768 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/sim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/detectors/base/
--rw-r--r--   0 root         (0) root         (0)      139 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      292 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      286 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)      290 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     5149 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/acquisition.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4984 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/acquisition.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)     5082 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/acquisition.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3257 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/connection.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     3268 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/connection.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)     3294 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/connection.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      679 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/controller.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      667 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/controller.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)      679 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/controller.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     6591 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/acquisition.py
--rw-r--r--   0 root         (0) root         (0)     2301 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/connection.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/controller.py
--rw-r--r--   0 root         (0) root         (0)     4930 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.432473 libertem-live-0.2.0/src/libertem_live/detectors/dectris/
--rw-r--r--   0 root         (0) root         (0)    23292 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/DEigerClient.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.432473 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/
--rw-r--r--   0 root         (0) root         (0)    22269 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/DEigerClient.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    22744 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/DEigerClient.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)    22557 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/DEigerClient.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      387 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      387 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)      385 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    16048 2023-04-20 15:42:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/acquisition.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    15740 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/acquisition.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)    16015 2023-04-20 15:49:53.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/acquisition.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2021 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/common.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     2001 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/common.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)     2023 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    13970 2023-04-20 15:42:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/connection.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    13689 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/connection.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)    13793 2023-04-20 15:49:54.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/connection.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     4467 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/controller.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4306 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/controller.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)     4370 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/controller.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    17448 2023-04-21 14:48:39.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/sim.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    18419 2023-04-20 15:19:45.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/acquisition.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/common.py
--rw-r--r--   0 root         (0) root         (0)    14526 2023-04-20 15:19:45.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/connection.py
--rw-r--r--   0 root         (0) root         (0)     5324 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/controller.py
--rw-r--r--   0 root         (0) root         (0)    27867 2023-04-20 17:16:36.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/sim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.432473 libertem-live-0.2.0/src/libertem_live/detectors/memory/
--rw-r--r--   0 root         (0) root         (0)      128 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/memory/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.432473 libertem-live-0.2.0/src/libertem_live/detectors/memory/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      274 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/memory/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     4043 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/memory/__pycache__/acquisition.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3535 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/memory/acquisition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.432473 libertem-live-0.2.0/src/libertem_live/detectors/merlin/
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.436473 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      442 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      442 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)      440 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    12638 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/acquisition.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    12356 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/acquisition.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)    12567 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/acquisition.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     9836 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/connection.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     9678 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/connection.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)     9747 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/connection.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     4657 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/control.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4610 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/control.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)     4635 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/control.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      681 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/controller.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      669 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/controller.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)      681 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/controller.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    16680 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/data.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    16629 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/data.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)    16727 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/data.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     4959 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     5698 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)     5183 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    30373 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_multi_u2-15.py310.1.nbc
--rw-r--r--   0 root         (0) root         (0)     1416 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_multi_u2-15.py310.nbi
--rw-r--r--   0 root         (0) root         (0)    30480 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_multi_u2-15.py37m.1.nbc
--rw-r--r--   0 root         (0) root         (0)     1416 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_multi_u2-15.py37m.nbi
--rw-r--r--   0 root         (0) root         (0)    20187 2023-04-19 17:22:35.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_multi_u2-15.py39.1.nbc
--rw-r--r--   0 root         (0) root         (0)     1415 2023-04-19 17:22:35.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_multi_u2-15.py39.nbi
--rw-r--r--   0 root         (0) root         (0)    26273 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_u2-4.py310.1.nbc
--rw-r--r--   0 root         (0) root         (0)     1366 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_u2-4.py310.nbi
--rw-r--r--   0 root         (0) root         (0)    26528 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_u2-4.py37m.1.nbc
--rw-r--r--   0 root         (0) root         (0)     1366 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_u2-4.py37m.nbi
--rw-r--r--   0 root         (0) root         (0)    18829 2023-04-19 17:22:35.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_u2-4.py39.1.nbc
--rw-r--r--   0 root         (0) root         (0)     1365 2023-04-19 17:22:35.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_u2-4.py39.nbi
--rw-r--r--   0 root         (0) root         (0)    23266 2023-04-19 17:22:20.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/sim.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    14317 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/acquisition.py
--rw-r--r--   0 root         (0) root         (0)     8647 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/connection.py
--rw-r--r--   0 root         (0) root         (0)     4252 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/control.py
--rw-r--r--   0 root         (0) root         (0)      258 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/controller.py
--rw-r--r--   0 root         (0) root         (0)    20418 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/data.py
--rw-r--r--   0 root         (0) root         (0)     8033 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/decoders.py
--rw-r--r--   0 root         (0) root         (0)    29504 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/sim.py
--rw-r--r--   0 root         (0) root         (0)     1342 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/tango_server.py
--rw-r--r--   0 root         (0) root         (0)     3858 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/utils.py
--rw-r--r--   0 root         (0) root         (0)     3657 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.436473 libertem-live-0.2.0/src/libertem_live/udf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.436473 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     3648 2023-04-19 12:43:04.000000 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/monitor.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     3702 2023-04-20 15:26:09.000000 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/monitor.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)     3684 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/monitor.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2194 2023-04-19 12:43:04.000000 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/record.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     2164 2023-04-20 15:26:09.000000 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/record.cpython-37.pyc
--rw-r--r--   0 root         (0) root         (0)     2184 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/record.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2848 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/udf/monitor.py
--rw-r--r--   0 root         (0) root         (0)     1726 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/udf/record.py
--rw-r--r--   0 root         (0) root         (0)      351 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/versioning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4494 2023-04-21 15:26:24.000000 libertem-live-0.2.0/src/libertem_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8600 2023-04-21 15:26:24.000000 libertem-live-0.2.0/src/libertem_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 15:26:24.000000 libertem-live-0.2.0/src/libertem_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      222 2023-04-21 15:26:24.000000 libertem-live-0.2.0/src/libertem_live.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 12:22:49.000000 libertem-live-0.2.0/src/libertem_live.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      165 2023-04-21 15:26:24.000000 libertem-live-0.2.0/src/libertem_live.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-21 15:26:24.000000 libertem-live-0.2.0/src/libertem_live.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.436473 libertem-live-0.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)     1512 2023-04-19 12:20:23.000000 libertem-live-0.2.0/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)      343 2023-04-19 12:20:23.000000 libertem-live-0.2.0/tests/test_smoke.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-02 20:41:58.000000 libertem-live-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      280 2023-05-09 12:49:56.000000 libertem-live-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-05-09 15:11:57.238100 libertem-live-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3229 2023-05-02 20:41:58.000000 libertem-live-0.2.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)     4793 2023-05-05 13:58:09.000000 libertem-live-0.2.1/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.230100 libertem-live-0.2.1/libertem_live/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-05-09 15:11:57.234100 libertem-live-0.2.1/libertem_live/_baked_revision.py
+-rw-r--r--   0 root         (0) root         (0)      363 2023-05-02 20:41:58.000000 libertem-live-0.2.1/override_requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-02 20:41:58.000000 libertem-live-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      931 2023-05-02 20:41:58.000000 libertem-live-0.2.1/pytest.ini
+-rw-r--r--   0 root         (0) root         (0)      513 2023-05-09 15:11:57.242100 libertem-live-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4331 2023-05-02 20:41:58.000000 libertem-live-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.234100 libertem-live-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.234100 libertem-live-0.2.1/src/libertem_live/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 15:04:46.000000 libertem-live-0.2.1/src/libertem_live/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     8951 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.234100 libertem-live-0.2.1/src/libertem_live/detectors/
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/LICENSE
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/src/libertem_live/detectors/asi_tpx3/
+-rw-r--r--   0 root         (0) root         (0)      291 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/asi_tpx3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13375 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/asi_tpx3/acquisition.py
+-rw-r--r--   0 root         (0) root         (0)     5783 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/asi_tpx3/connection.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/asi_tpx3/controller.py
+-rw-r--r--   0 root         (0) root         (0)     9696 2023-05-09 11:20:54.000000 libertem-live-0.2.1/src/libertem_live/detectors/asi_tpx3/sim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/src/libertem_live/detectors/base/
+-rw-r--r--   0 root         (0) root         (0)      139 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6591 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/base/acquisition.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/base/connection.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/base/controller.py
+-rw-r--r--   0 root         (0) root         (0)     4956 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/src/libertem_live/detectors/dectris/
+-rw-r--r--   0 root         (0) root         (0)    23292 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/dectris/DEigerClient.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/dectris/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18419 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/dectris/acquisition.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/dectris/common.py
+-rw-r--r--   0 root         (0) root         (0)    14526 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/dectris/connection.py
+-rw-r--r--   0 root         (0) root         (0)     5324 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/dectris/controller.py
+-rw-r--r--   0 root         (0) root         (0)    29478 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/dectris/sim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/src/libertem_live/detectors/memory/
+-rw-r--r--   0 root         (0) root         (0)      128 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/memory/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/memory/acquisition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/src/libertem_live/detectors/merlin/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/merlin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14317 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/merlin/acquisition.py
+-rw-r--r--   0 root         (0) root         (0)     8647 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/merlin/connection.py
+-rw-r--r--   0 root         (0) root         (0)     4252 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/merlin/control.py
+-rw-r--r--   0 root         (0) root         (0)      258 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/merlin/controller.py
+-rw-r--r--   0 root         (0) root         (0)    20418 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/merlin/data.py
+-rw-r--r--   0 root         (0) root         (0)     8038 2023-05-09 09:06:59.000000 libertem-live-0.2.1/src/libertem_live/detectors/merlin/decoders.py
+-rw-r--r--   0 root         (0) root         (0)    29786 2023-05-04 17:37:55.000000 libertem-live-0.2.1/src/libertem_live/detectors/merlin/sim.py
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/detectors/merlin/tango_server.py
+-rw-r--r--   0 root         (0) root         (0)     3859 2023-05-09 09:06:59.000000 libertem-live-0.2.1/src/libertem_live/detectors/merlin/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/src/libertem_live/udf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/udf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/udf/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/udf/record.py
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-02 20:41:58.000000 libertem-live-0.2.1/src/libertem_live/versioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.234100 libertem-live-0.2.1/src/libertem_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-05-09 15:11:57.000000 libertem-live-0.2.1/src/libertem_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-05-09 15:11:57.000000 libertem-live-0.2.1/src/libertem_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 15:11:57.000000 libertem-live-0.2.1/src/libertem_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-09 15:11:57.000000 libertem-live-0.2.1/src/libertem_live.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 20:43:59.000000 libertem-live-0.2.1/src/libertem_live.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      181 2023-05-09 15:11:57.000000 libertem-live-0.2.1/src/libertem_live.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-09 15:11:57.000000 libertem-live-0.2.1/src/libertem_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      231 2023-05-05 13:58:09.000000 libertem-live-0.2.1/test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/tests/
+-rw-r--r--   0 root         (0) root         (0)       74 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.234100 libertem-live-0.2.1/tests/detectors/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/tests/detectors/asi_tpx3/
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/asi_tpx3/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3247 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/asi_tpx3/test_asi_tpx3.py
+-rw-r--r--   0 root         (0) root         (0)     3233 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/asi_tpx3/test_asi_tpx3_mock.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-05-09 11:20:54.000000 libertem-live-0.2.1/tests/detectors/asi_tpx3/test_asi_tpx3_sim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/tests/detectors/base/
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/base/test_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/tests/detectors/dectris/
+-rw-r--r--   0 root         (0) root         (0)    22909 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/dectris/test_dectris.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/dectris/test_mocked.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/tests/detectors/memory/
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/memory/test_memory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/tests/detectors/merlin/
+-rw-r--r--   0 root         (0) root         (0)    11992 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/merlin/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     4275 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/merlin/test_decoders.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/merlin/test_headers.py
+-rw-r--r--   0 root         (0) root         (0)    13137 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/merlin/test_merlin.py
+-rw-r--r--   0 root         (0) root         (0)     3442 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/merlin/test_merlin_mockds.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/merlin/test_merlin_sim.py
+-rw-r--r--   0 root         (0) root         (0)     2661 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/detectors/merlin/test_server.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/test_smoke.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:11:57.238100 libertem-live-0.2.1/tests/udf/
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/udf/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/udf/test_record.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tests/utils.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-05-02 20:41:58.000000 libertem-live-0.2.1/tox.ini
```

### Comparing `libertem-live-0.2.0/LICENSE` & `libertem-live-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/PKG-INFO` & `libertem-live-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: libertem-live
-Version: 0.2.0
+Version: 0.2.1
 Summary: Live processing with LiberTEM
 Home-page: https://libertem.github.io/LiberTEM-live
 Author: the LiberTEM team
 Author-email: libertem-dev@googlegroups.com
 License: GPL v3
 Keywords: electron microscopy
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
@@ -111,9 +110,7 @@
 We are very grateful for your continuing support for LiberTEM-live!
 
 See `the acknowledgement page
 <https://libertem.github.io/acknowledgements.html#libertem-live>`_ for a list of
 authors and contributors to LiberTEM-live and other LiberTEM projects. See also
 our info on `funding <https://libertem.github.io/#funding>`_ and `industry
 partners <https://libertem.github.io/#industry-partners>`_.
-
-
```

### Comparing `libertem-live-0.2.0/README.rst` & `libertem-live-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/setup.cfg` & `libertem-live-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-license_file = LICENSE
+license_files = LICENSE
 
 [flake8]
 max-line-length = 100
 ignore = E24,E121,E123,E126,E128,E133,E226,E241,E242,E704,W503
 exclude = .git,__pycache__,.tox,build,dist,node_modules,TOXENV
 
 [coverage:run]
```

### Comparing `libertem-live-0.2.0/setup.py` & `libertem-live-0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,16 +81,16 @@
         "libertem>=0.11.0.dev0",
         "numpy",
         "click",
         "tqdm",
         "numba",
         "opentelemetry-api",
         "sparseconverter",
-        "libertem-dectris",
-        "libertem-asi-tpx3",
+        "libertem-dectris>=0.2.10",
+        "libertem-asi-tpx3>=0.2.10",
     ],
     extras_require={
         'sim': ['flask'],
         'pymemfd': 'pymemfd',
         'pytango': 'pytango',
     },
     package_dir={"": "src"},
```

### Comparing `libertem-live-0.2.0/src/libertem_live/__pycache__/hooks.cpython-310.pyc` & `libertem-live-0.2.1/src/libertem_live/hooks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,243 +1,229 @@
-00000000: 6f0d 0d0a 0000 0000 87dc 3f64 490e 0000  o.........?dI...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
-00000040: 6d04 5a04 0100 6503 7214 6400 6402 6c05  m.Z...e.r.d.d.l.
-00000050: 6d06 5a06 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
-00000060: 6502 8303 5a07 4700 6405 6406 8400 6406  e...Z.G.d.d...d.
-00000070: 6502 8303 5a08 4700 6407 6408 8400 6408  e...Z.G.d.d...d.
-00000080: 8302 5a09 6409 5300 290a e900 0000 0029  ..Z.d.S.)......)
-00000090: 04da 0554 7570 6c65 da0a 4e61 6d65 6454  ...Tuple..NamedT
-000000a0: 7570 6c65 da0d 5459 5045 5f43 4845 434b  uple..TYPE_CHECK
-000000b0: 494e 47da 084f 7074 696f 6e61 6c29 01da  ING..Optional)..
-000000c0: 1341 6371 7569 7369 7469 6f6e 5072 6f74  .AcquisitionProt
-000000d0: 6f63 6f6c 6300 0000 0000 0000 0000 0000  ocolc...........
-000000e0: 0000 0000 0003 0000 0040 0000 0073 1a00  .........@...s..
-000000f0: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-00000100: 6402 6504 6403 3c00 6404 5300 2905 da0f  d.e.d.<.d.S.)...
-00000110: 5265 6164 7946 6f72 4461 7461 456e 767a  ReadyForDataEnvz
-00000120: 570a 2020 2020 5061 7261 6d65 7465 7220  W.    Parameter 
-00000130: 6f62 6a65 6374 2075 7365 6420 696e 203a  object used in :
-00000140: 6d65 7468 3a60 7e6c 6962 6572 7465 6d5f  meth:`~libertem_
-00000150: 6c69 7665 2e68 6f6f 6b73 2e48 6f6f 6b73  live.hooks.Hooks
-00000160: 2e6f 6e5f 7265 6164 795f 666f 725f 6461  .on_ready_for_da
-00000170: 7461 600a 2020 2020 7206 0000 00da 0261  ta`.    r......a
-00000180: 714e 2905 da08 5f5f 6e61 6d65 5f5f da0a  qN)...__name__..
-00000190: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000001a0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-000001b0: 5fda 0f5f 5f61 6e6e 6f74 6174 696f 6e73  _..__annotations
-000001c0: 5f5f a900 720e 0000 0072 0e00 0000 fa2f  __..r....r...../
-000001d0: 2f61 7a70 2f61 6765 6e74 2f5f 776f 726b  /azp/agent/_work
-000001e0: 2f31 2f73 2f73 7263 2f6c 6962 6572 7465  /1/s/src/liberte
-000001f0: 6d5f 6c69 7665 2f68 6f6f 6b73 2e70 7972  m_live/hooks.pyr
-00000200: 0700 0000 0800 0000 7308 0000 000a 0004  ........s.......
-00000210: 0108 0404 0172 0700 0000 6300 0000 0000  .....r....c.....
-00000220: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
-00000230: 0000 0073 3000 0000 6500 5a01 6400 5a02  ...s0...e.Z.d.Z.
-00000240: 5500 6401 5a03 6504 6505 6402 3c00 0900  U.d.Z.e.e.d.<...
-00000250: 6506 6507 6504 6403 6602 1900 1900 6505  e.e.e.d.f.....e.
-00000260: 6404 3c00 6405 5300 2906 da14 4465 7465  d.<.d.S.)...Dete
-00000270: 726d 696e 654e 6176 5368 6170 6545 6e76  rmineNavShapeEnv
-00000280: 7a5c 0a20 2020 2050 6172 616d 6574 6572  z\.    Parameter
-00000290: 206f 626a 6563 7420 7573 6564 2069 6e20   object used in 
-000002a0: 3a6d 6574 683a 607e 6c69 6265 7274 656d  :meth:`~libertem
-000002b0: 5f6c 6976 652e 686f 6f6b 732e 486f 6f6b  _live.hooks.Hook
-000002c0: 732e 6f6e 5f64 6574 6572 6d69 6e65 5f6e  s.on_determine_n
-000002d0: 6176 5f73 6861 7065 600a 2020 2020 da07  av_shape`.    ..
-000002e0: 6e69 6d61 6765 732e da0a 7368 6170 655f  nimages...shape_
-000002f0: 6869 6e74 4e29 0872 0900 0000 720a 0000  hintN).r....r...
-00000300: 0072 0b00 0000 720c 0000 00da 0369 6e74  .r....r......int
-00000310: 720d 0000 0072 0500 0000 7202 0000 0072  r....r....r....r
-00000320: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
-00000330: 0000 0072 1000 0000 1300 0000 730c 0000  ...r........s...
-00000340: 000a 0004 0108 0402 0114 0404 0172 1000  .............r..
-00000350: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000360: 0000 0007 0000 0040 0000 0073 3c00 0000  .......@...s<...
-00000370: 6500 5a01 6400 5a02 6401 5a03 6402 6504  e.Z.d.Z.d.Z.d.e.
-00000380: 6602 6403 6404 8404 5a05 6402 6506 6405  f.d.d...Z.d.e.d.
-00000390: 6507 6508 6509 6406 6602 1900 1900 6604  e.e.e.d.f.....f.
-000003a0: 6407 6408 8404 5a0a 6409 5300 290a da05  d.d...Z.d.S.)...
-000003b0: 486f 6f6b 7361 0d02 0000 0a20 2020 2049  Hooksa.....    I
-000003c0: 6e74 6572 6661 6365 2066 6f72 2064 6566  nterface for def
-000003d0: 696e 696e 6720 6163 7469 6f6e 7320 746f  ining actions to
-000003e0: 2070 6572 666f 726d 2069 6e20 7265 6163   perform in reac
-000003f0: 7469 6f6e 2074 6f20 6576 656e 7473 2e0a  tion to events..
-00000400: 2020 2020 5468 6973 2069 7320 7365 7475      This is setu
-00000410: 702d 2061 6e64 2070 6f73 7369 626c 7920  p- and possibly 
-00000420: 6578 7065 7269 6d65 6e74 2d73 7065 6369  experiment-speci
-00000430: 6669 6320 616e 6420 6361 6e2c 2066 6f72  fic and can, for
-00000440: 2065 7861 6d70 6c65 2c20 656e 636f 6465   example, encode
-00000450: 0a20 2020 2068 6f77 2074 6865 206d 6963  .    how the mic
-00000460: 726f 7363 6f70 652c 2073 6361 6e20 656e  roscope, scan en
-00000470: 6769 6e65 2061 6e64 2064 6574 6563 746f  gine and detecto
-00000480: 7220 6172 6520 7379 6e63 6872 6f6e 697a  r are synchroniz
-00000490: 6564 2e0a 0a20 2020 2042 7920 696d 706c  ed...    By impl
-000004a0: 656d 656e 7469 6e67 206d 6574 686f 6473  ementing methods
-000004b0: 206f 6620 7468 6973 2069 6e74 6572 6661   of this interfa
-000004c0: 6365 2c20 796f 7520 6361 6e20 2268 6f6f  ce, you can "hoo
-000004d0: 6b20 696e 746f 2220 7468 6520 6c69 6665  k into" the life
-000004e0: 6379 636c 6520 6f66 0a20 2020 2061 6e20  cycle of.    an 
-000004f0: 6163 7175 6973 6974 696f 6e20 6174 2064  acquisition at d
-00000500: 6966 6665 7265 6e74 2069 6d70 6f72 7461  ifferent importa
-00000510: 6e74 2065 7665 6e74 732e 0a0a 2020 2020  nt events...    
-00000520: 4561 6368 2068 6f6f 6b20 6d65 7468 6f64  Each hook method
-00000530: 2067 6574 7320 6120 7370 6563 6966 6963   gets a specific
-00000540: 2065 6e76 6972 6f6e 6d65 6e74 206f 626a   environment obj
-00000550: 6563 7420 6173 2061 2070 6172 616d 6574  ect as a paramet
-00000560: 6572 2c20 7468 6174 0a20 2020 2069 6e63  er, that.    inc
-00000570: 6c75 6465 7320 616c 6c20 6e65 6365 7373  ludes all necess
-00000580: 6172 7920 636f 6e74 6578 7420 696e 666f  ary context info
-00000590: 726d 6174 696f 6e20 6672 6f6d 2063 7572  rmation from cur
-000005a0: 7265 6e74 2073 7461 7465 206f 6620 7468  rent state of th
-000005b0: 650a 2020 2020 6163 7175 6973 6974 696f  e.    acquisitio
-000005c0: 6e2e 0a20 2020 20da 0365 6e76 6302 0000  n..    ..envc...
-000005d0: 0000 0000 0000 0000 0002 0000 0001 0000  ................
-000005e0: 0043 0000 00f3 0400 0000 6401 5300 2902  .C........d.S.).
-000005f0: 61b5 0100 000a 2020 2020 2020 2020 5468  a.....        Th
-00000600: 6973 2068 6f6f 6b20 6973 2063 616c 6c65  is hook is calle
-00000610: 6420 7768 656e 6576 6572 2077 6520 6172  d whenever we ar
-00000620: 6520 7265 6164 7920 666f 7220 6461 7461  e ready for data
-00000630: 2c20 692e 652e 2074 6865 2064 6574 6563  , i.e. the detec
-00000640: 746f 7220 6973 0a20 2020 2020 2020 2061  tor is.        a
-00000650: 726d 6564 2e0a 0a20 2020 2020 2020 2055  rmed...        U
-00000660: 7375 616c 6c79 2c20 6174 2074 6869 7320  sually, at this 
-00000670: 706f 696e 742c 2074 6865 206e 6578 7420  point, the next 
-00000680: 7374 6570 2069 7320 7472 6967 6765 7269  step is triggeri
-00000690: 6e67 2074 6865 206d 6963 726f 7363 6f70  ng the microscop
-000006a0: 6520 6f72 0a20 2020 2020 2020 2073 6361  e or.        sca
-000006b0: 6e20 6765 6e65 7261 746f 7220 746f 2073  n generator to s
-000006c0: 7461 7274 2061 2073 6361 6e2e 0a0a 2020  tart a scan...  
-000006d0: 2020 2020 2020 4974 2069 7320 6f6e 6c79        It is only
-000006e0: 2063 616c 6c65 6420 696e 2061 6374 6976   called in activ
-000006f0: 6520 6d6f 6465 2c20 7768 6572 6520 7765  e mode, where we
-00000700: 2063 6f6e 7472 6f6c 2077 6865 6e20 7468   control when th
-00000710: 6520 6465 7465 6374 6f72 2069 730a 2020  e detector is.  
-00000720: 2020 2020 2020 6172 6d65 6420 2d20 696e        armed - in
-00000730: 2070 6173 7369 7665 206d 6f64 652c 2074   passive mode, t
-00000740: 6865 2064 6174 6120 6973 2070 6f73 7369  he data is possi
-00000750: 626c 7920 616c 7265 6164 7920 6265 696e  bly already bein
-00000760: 6720 7265 6365 6976 6564 2061 6e64 0a20  g received and. 
-00000770: 2020 2020 2020 2077 6520 646f 6e27 7420         we don't 
-00000780: 636f 6e74 726f 6c20 7768 656e 2074 6869  control when thi
-00000790: 7320 6861 7070 656e 7320 6174 2061 6c6c  s happens at all
-000007a0: 2e0a 2020 2020 2020 2020 4e72 0e00 0000  ..        Nr....
-000007b0: a902 da04 7365 6c66 7215 0000 0072 0e00  ....selfr....r..
-000007c0: 0000 720e 0000 0072 0f00 0000 da11 6f6e  ..r....r......on
-000007d0: 5f72 6561 6479 5f66 6f72 5f64 6174 6136  _ready_for_data6
-000007e0: 0000 0073 0200 0000 040c 7a17 486f 6f6b  ...s......z.Hook
-000007f0: 732e 6f6e 5f72 6561 6479 5f66 6f72 5f64  s.on_ready_for_d
-00000800: 6174 61da 0672 6574 7572 6e2e 6302 0000  ata..return.c...
-00000810: 0000 0000 0000 0000 0002 0000 0001 0000  ................
-00000820: 0043 0000 0072 1600 0000 2902 619d 0500  .C...r....).a...
-00000830: 000a 2020 2020 2020 2020 5468 6973 2068  ..        This h
-00000840: 6f6f 6b20 6973 2063 616c 6c65 6420 746f  ook is called to
-00000850: 2064 6574 6572 6d69 6e65 2074 6865 204e   determine the N
-00000860: 2d44 206e 6176 2073 6861 7065 2066 6f72  -D nav shape for
-00000870: 2074 6865 2061 6371 7569 7369 7469 6f6e   the acquisition
-00000880: 2e0a 2020 2020 2020 2020 5468 6973 2069  ..        This i
-00000890: 7320 6e65 6564 6564 2061 7320 6d61 6e79  s needed as many
-000008a0: 2064 6574 6563 746f 7273 206f 6e6c 7920   detectors only 
-000008b0: 6b6e 6f77 2061 626f 7574 2074 6865 2031  know about the 1
-000008c0: 4420 7368 6170 652c 2069 2e65 2e20 7468  D shape, i.e. th
-000008d0: 650a 2020 2020 2020 2020 6e75 6d62 6572  e.        number
-000008e0: 206f 6620 696d 6167 6573 2074 6f20 6163   of images to ac
-000008f0: 7175 6972 652e 2046 6f72 2073 6f6d 652c  quire. For some,
-00000900: 2074 6865 2063 6f6e 7472 6f6c 6c65 7220   the controller 
-00000910: 6d61 7920 6265 2061 626c 6520 746f 0a20  may be able to. 
-00000920: 2020 2020 2020 2064 6574 6572 6d69 6e65         determine
-00000930: 2074 6865 206e 6176 2073 6861 7065 2c20   the nav shape, 
-00000940: 6275 7420 666f 7220 6f74 6865 7273 2c20  but for others, 
-00000950: 7468 6973 2069 7320 7370 6563 6966 6963  this is specific
-00000960: 2074 6f20 7468 6520 7365 7475 700a 2020   to the setup.  
-00000970: 2020 2020 2020 6f72 2065 7870 6572 696d        or experim
-00000980: 656e 742e 0a0a 2020 2020 2020 2020 5468  ent...        Th
-00000990: 6520 7573 6572 2063 616e 2067 6976 6520  e user can give 
-000009a0: 6120 7368 6170 6520 6869 6e74 2077 6865  a shape hint whe
-000009b0: 6e20 6372 6561 7469 6e67 2074 6865 2061  n creating the a
-000009c0: 6371 7569 7369 7469 6f6e 206f 626a 6563  cquisition objec
-000009d0: 742c 0a20 2020 2020 2020 2066 6f72 2065  t,.        for e
-000009e0: 7861 6d70 6c65 2062 7920 7061 7373 696e  xample by passin
-000009f0: 6720 3a63 6f64 653a 606e 6176 5f73 6861  g :code:`nav_sha
-00000a00: 7065 3d28 2d31 2c20 3235 3629 6020 746f  pe=(-1, 256)` to
-00000a10: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
-00000a20: 7e6c 6962 6572 7465 6d5f 6c69 7665 2e61  ~libertem_live.a
-00000a30: 7069 2e4c 6976 6543 6f6e 7465 7874 2e6d  pi.LiveContext.m
-00000a40: 616b 655f 6163 7175 6973 6974 696f 6e60  ake_acquisition`
-00000a50: 2e0a 0a20 2020 2020 2020 2049 6620 7468  ...        If th
-00000a60: 6520 6465 6661 756c 7420 6265 6861 7669  e default behavi
-00000a70: 6f72 2069 7320 6e6f 7420 776f 726b 696e  or is not workin
-00000a80: 6720 6173 2069 6e74 656e 6465 642c 2074  g as intended, t
-00000a90: 6865 2075 7365 7220 6361 6e20 6f76 6572  he user can over
-00000aa0: 7269 6465 0a20 2020 2020 2020 2074 6869  ride.        thi
-00000ab0: 7320 6d65 7468 6f64 2066 6f72 2074 6865  s method for the
-00000ac0: 6972 2073 7065 6369 6669 6320 7365 7475  ir specific setu
-00000ad0: 702e 2045 7861 6d70 6c65 3a20 6173 6b20  p. Example: ask 
-00000ae0: 7468 6520 6d69 6372 6f73 636f 7065 2076  the microscope v
-00000af0: 6961 2069 7473 0a20 2020 2020 2020 2041  ia its.        A
-00000b00: 5049 2077 6861 7420 7468 6520 6375 7272  PI what the curr
-00000b10: 656e 7420 7363 616e 2073 6574 7469 6e67  ent scan setting
-00000b20: 7320 6172 652e 0a0a 2020 2020 2020 2020  s are...        
-00000b30: 4f6e 6c79 2063 616c 6c65 6420 696e 2070  Only called in p
-00000b40: 6173 7369 7665 206d 6f64 652c 2061 7320  assive mode, as 
-00000b50: 7765 206e 6565 6420 6120 636f 6e63 7265  we need a concre
-00000b60: 7465 2060 6e61 765f 7368 6170 6560 2061  te `nav_shape` a
-00000b70: 7320 7573 6572 0a20 2020 2020 2020 2069  s user.        i
-00000b80: 6e70 7574 2069 6e20 6163 7469 7665 206d  nput in active m
-00000b90: 6f64 652e 0a0a 2020 2020 2020 2020 4f72  ode...        Or
-00000ba0: 6465 7220 6f66 206f 7065 7261 7469 6f6e  der of operation
-00000bb0: 733a 0a0a 2020 2020 2020 2020 2a20 4966  s:..        * If
-00000bc0: 2074 6865 2060 6e61 765f 7368 6170 6560   the `nav_shape`
-00000bd0: 2070 6173 7365 6420 696e 746f 0a20 2020   passed into.   
-00000be0: 2020 2020 2020 203a 6d65 7468 3a60 6c69         :meth:`li
-00000bf0: 6265 7274 656d 5f6c 6976 652e 6170 692e  bertem_live.api.
-00000c00: 4c69 7665 436f 6e74 6578 742e 6d61 6b65  LiveContext.make
-00000c10: 5f61 6371 7569 7369 7469 6f6e 6020 6973  _acquisition` is
-00000c20: 2063 6f6e 6372 6574 652c 2069 2e65 2e0a   concrete, i.e..
-00000c30: 2020 2020 2020 2020 2020 6973 206e 6f74            is not
-00000c40: 2060 4e6f 6e65 6020 616e 6420 646f 6573   `None` and does
-00000c50: 6e27 7420 636f 6e74 6169 6e20 616e 7920  n't contain any 
-00000c60: 602d 3160 2076 616c 7565 732c 2075 7365  `-1` values, use
-00000c70: 2074 6861 740a 2020 2020 2020 2020 2a20   that.        * 
-00000c80: 4966 2074 6869 7320 686f 6f6b 2069 7320  If this hook is 
-00000c90: 696d 706c 656d 656e 7465 6420 616e 6420  implemented and 
-00000ca0: 7265 7475 726e 7320 6120 7475 706c 652c  returns a tuple,
-00000cb0: 2075 7365 2074 6861 740a 2020 2020 2020   use that.      
-00000cc0: 2020 2a20 4966 2074 6865 2063 6f6e 7472    * If the contr
-00000cd0: 6f6c 6c65 7220 666f 7220 7468 6520 7370  oller for the sp
-00000ce0: 6563 6966 6963 2064 6574 6563 746f 7220  ecific detector 
-00000cf0: 7479 7065 2063 616e 2067 6976 6520 7573  type can give us
-00000d00: 0a20 2020 2020 2020 2020 2074 6865 2063  .          the c
-00000d10: 6f6e 6372 6574 6520 606e 6176 5f73 6861  oncrete `nav_sha
-00000d20: 7065 602c 2075 7365 2074 6861 740a 2020  pe`, use that.  
-00000d30: 2020 2020 2020 2a20 4966 206e 6f6e 6520        * If none 
-00000d40: 6f66 2074 6865 2061 626f 7665 2073 7563  of the above suc
-00000d50: 6365 6564 2c20 7472 7920 746f 206d 616b  ceed, try to mak
-00000d60: 6520 6120 7371 7561 7265 206f 7574 206f  e a square out o
-00000d70: 6620 7468 650a 2020 2020 2020 2020 2020  f the.          
-00000d80: 6e75 6d62 6572 206f 6620 6672 616d 6573  number of frames
-00000d90: 0a20 2020 2020 2020 202a 2049 6620 616c  .        * If al
-00000da0: 6c20 6162 6f76 6520 6661 696c 732c 2072  l above fails, r
-00000db0: 6169 7365 2061 2060 5275 6e74 696d 6545  aise a `RuntimeE
-00000dc0: 7272 6f72 600a 2020 2020 2020 2020 4e72  rror`.        Nr
-00000dd0: 0e00 0000 7217 0000 0072 0e00 0000 720e  ....r....r....r.
-00000de0: 0000 0072 0f00 0000 da16 6f6e 5f64 6574  ...r......on_det
-00000df0: 6572 6d69 6e65 5f6e 6176 5f73 6861 7065  ermine_nav_shape
-00000e00: 4400 0000 7302 0000 0004 227a 1c48 6f6f  D...s....."z.Hoo
-00000e10: 6b73 2e6f 6e5f 6465 7465 726d 696e 655f  ks.on_determine_
-00000e20: 6e61 765f 7368 6170 654e 290b 7209 0000  nav_shapeN).r...
-00000e30: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000e40: 7207 0000 0072 1900 0000 7210 0000 0072  r....r....r....r
-00000e50: 0500 0000 7202 0000 0072 1300 0000 721b  ....r....r....r.
-00000e60: 0000 0072 0e00 0000 720e 0000 0072 0e00  ...r....r....r..
-00000e70: 0000 720f 0000 0072 1400 0000 2400 0000  ..r....r....$...
-00000e80: 7310 0000 0008 0004 010e 1102 0e02 0202  s...............
-00000e90: fe0e 030e fd72 1400 0000 4e29 0ada 0674  .....r....N)...t
-00000ea0: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
-00000eb0: 0400 0000 7205 0000 00da 286c 6962 6572  ....r.....(liber
-00000ec0: 7465 6d5f 6c69 7665 2e64 6574 6563 746f  tem_live.detecto
-00000ed0: 7273 2e62 6173 652e 6163 7175 6973 6974  rs.base.acquisit
-00000ee0: 696f 6e72 0600 0000 7207 0000 0072 1000  ionr....r....r..
-00000ef0: 0000 7214 0000 0072 0e00 0000 720e 0000  ..r....r....r...
-00000f00: 0072 0e00 0000 720f 0000 00da 083c 6d6f  .r....r......<mo
-00000f10: 6475 6c65 3e01 0000 0073 0c00 0000 1800  dule>....s......
-00000f20: 0403 0c01 1003 100b 1211                 ..........
+00000000: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000010: 7274 2054 7570 6c65 2c20 4e61 6d65 6454  rt Tuple, NamedT
+00000020: 7570 6c65 2c20 5459 5045 5f43 4845 434b  uple, TYPE_CHECK
+00000030: 494e 472c 204f 7074 696f 6e61 6c0a 0a0a  ING, Optional...
+00000040: 6966 2054 5950 455f 4348 4543 4b49 4e47  if TYPE_CHECKING
+00000050: 3a0a 2020 2020 6672 6f6d 206c 6962 6572  :.    from liber
+00000060: 7465 6d5f 6c69 7665 2e64 6574 6563 746f  tem_live.detecto
+00000070: 7273 2e62 6173 652e 6163 7175 6973 6974  rs.base.acquisit
+00000080: 696f 6e20 696d 706f 7274 2041 6371 7569  ion import Acqui
+00000090: 7369 7469 6f6e 5072 6f74 6f63 6f6c 0a0a  sitionProtocol..
+000000a0: 0a63 6c61 7373 2052 6561 6479 466f 7244  .class ReadyForD
+000000b0: 6174 6145 6e76 284e 616d 6564 5475 706c  ataEnv(NamedTupl
+000000c0: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
+000000d0: 5061 7261 6d65 7465 7220 6f62 6a65 6374  Parameter object
+000000e0: 2075 7365 6420 696e 203a 6d65 7468 3a60   used in :meth:`
+000000f0: 7e6c 6962 6572 7465 6d5f 6c69 7665 2e68  ~libertem_live.h
+00000100: 6f6f 6b73 2e48 6f6f 6b73 2e6f 6e5f 7265  ooks.Hooks.on_re
+00000110: 6164 795f 666f 725f 6461 7461 600a 2020  ady_for_data`.  
+00000120: 2020 2222 220a 0a20 2020 2061 713a 2022    """..    aq: "
+00000130: 4163 7175 6973 6974 696f 6e50 726f 746f  AcquisitionProto
+00000140: 636f 6c22 0a20 2020 2022 2222 0a20 2020  col".    """.   
+00000150: 2054 6865 2061 6371 7569 7369 7469 6f6e   The acquisition
+00000160: 206f 626a 6563 7420 7768 6963 6820 7769   object which wi
+00000170: 6c6c 2072 6563 6569 7665 2074 6865 2064  ll receive the d
+00000180: 6174 612e 0a20 2020 2022 2222 0a0a 0a63  ata..    """...c
+00000190: 6c61 7373 2044 6574 6572 6d69 6e65 4e61  lass DetermineNa
+000001a0: 7653 6861 7065 456e 7628 4e61 6d65 6454  vShapeEnv(NamedT
+000001b0: 7570 6c65 293a 0a20 2020 2022 2222 0a20  uple):.    """. 
+000001c0: 2020 2050 6172 616d 6574 6572 206f 626a     Parameter obj
+000001d0: 6563 7420 7573 6564 2069 6e20 3a6d 6574  ect used in :met
+000001e0: 683a 607e 6c69 6265 7274 656d 5f6c 6976  h:`~libertem_liv
+000001f0: 652e 686f 6f6b 732e 486f 6f6b 732e 6f6e  e.hooks.Hooks.on
+00000200: 5f64 6574 6572 6d69 6e65 5f6e 6176 5f73  _determine_nav_s
+00000210: 6861 7065 600a 2020 2020 2222 220a 0a20  hape`.    """.. 
+00000220: 2020 206e 696d 6167 6573 3a20 696e 740a     nimages: int.
+00000230: 2020 2020 2222 220a 2020 2020 5468 6520      """.    The 
+00000240: 746f 7461 6c20 6e75 6d62 6572 206f 6620  total number of 
+00000250: 696d 6167 6573 2069 6e20 7468 6520 6163  images in the ac
+00000260: 7175 6973 6974 696f 6e2e 0a20 2020 2022  quisition..    "
+00000270: 2222 0a0a 2020 2020 7368 6170 655f 6869  ""..    shape_hi
+00000280: 6e74 3a20 4f70 7469 6f6e 616c 5b54 7570  nt: Optional[Tup
+00000290: 6c65 5b69 6e74 2c20 2e2e 2e5d 5d0a 2020  le[int, ...]].  
+000002a0: 2020 2222 220a 2020 2020 5368 6170 6520    """.    Shape 
+000002b0: 7468 6174 2077 6173 2070 6173 7365 6420  that was passed 
+000002c0: 696e 746f 203a 6d65 7468 3a60 7e6c 6962  into :meth:`~lib
+000002d0: 6572 7465 6d5f 6c69 7665 2e61 7069 2e4c  ertem_live.api.L
+000002e0: 6976 6543 6f6e 7465 7874 2e6d 616b 655f  iveContext.make_
+000002f0: 6163 7175 6973 6974 696f 6e60 2c20 6361  acquisition`, ca
+00000300: 6e20 636f 6e74 6169 6e0a 2020 2020 706c  n contain.    pl
+00000310: 6163 6568 6f6c 6465 7273 2c20 692e 652e  aceholders, i.e.
+00000320: 203a 636f 6465 3a60 282d 312c 2032 3536   :code:`(-1, 256
+00000330: 2960 206f 7220 3a63 6f64 653a 6028 2d31  )` or :code:`(-1
+00000340: 2c20 2d31 2960 2e0a 2020 2020 2222 220a  , -1)`..    """.
+00000350: 0a0a 636c 6173 7320 486f 6f6b 733a 0a20  ..class Hooks:. 
+00000360: 2020 2022 2222 0a20 2020 2049 6e74 6572     """.    Inter
+00000370: 6661 6365 2066 6f72 2064 6566 696e 696e  face for definin
+00000380: 6720 6163 7469 6f6e 7320 746f 2070 6572  g actions to per
+00000390: 666f 726d 2069 6e20 7265 6163 7469 6f6e  form in reaction
+000003a0: 2074 6f20 6576 656e 7473 2e0a 2020 2020   to events..    
+000003b0: 5468 6973 2069 7320 7365 7475 702d 2061  This is setup- a
+000003c0: 6e64 2070 6f73 7369 626c 7920 6578 7065  nd possibly expe
+000003d0: 7269 6d65 6e74 2d73 7065 6369 6669 6320  riment-specific 
+000003e0: 616e 6420 6361 6e2c 2066 6f72 2065 7861  and can, for exa
+000003f0: 6d70 6c65 2c20 656e 636f 6465 0a20 2020  mple, encode.   
+00000400: 2068 6f77 2074 6865 206d 6963 726f 7363   how the microsc
+00000410: 6f70 652c 2073 6361 6e20 656e 6769 6e65  ope, scan engine
+00000420: 2061 6e64 2064 6574 6563 746f 7220 6172   and detector ar
+00000430: 6520 7379 6e63 6872 6f6e 697a 6564 2e0a  e synchronized..
+00000440: 0a20 2020 2042 7920 696d 706c 656d 656e  .    By implemen
+00000450: 7469 6e67 206d 6574 686f 6473 206f 6620  ting methods of 
+00000460: 7468 6973 2069 6e74 6572 6661 6365 2c20  this interface, 
+00000470: 796f 7520 6361 6e20 2268 6f6f 6b20 696e  you can "hook in
+00000480: 746f 2220 7468 6520 6c69 6665 6379 636c  to" the lifecycl
+00000490: 6520 6f66 0a20 2020 2061 6e20 6163 7175  e of.    an acqu
+000004a0: 6973 6974 696f 6e20 6174 2064 6966 6665  isition at diffe
+000004b0: 7265 6e74 2069 6d70 6f72 7461 6e74 2065  rent important e
+000004c0: 7665 6e74 732e 0a0a 2020 2020 4561 6368  vents...    Each
+000004d0: 2068 6f6f 6b20 6d65 7468 6f64 2067 6574   hook method get
+000004e0: 7320 6120 7370 6563 6966 6963 2065 6e76  s a specific env
+000004f0: 6972 6f6e 6d65 6e74 206f 626a 6563 7420  ironment object 
+00000500: 6173 2061 2070 6172 616d 6574 6572 2c20  as a parameter, 
+00000510: 7468 6174 0a20 2020 2069 6e63 6c75 6465  that.    include
+00000520: 7320 616c 6c20 6e65 6365 7373 6172 7920  s all necessary 
+00000530: 636f 6e74 6578 7420 696e 666f 726d 6174  context informat
+00000540: 696f 6e20 6672 6f6d 2063 7572 7265 6e74  ion from current
+00000550: 2073 7461 7465 206f 6620 7468 650a 2020   state of the.  
+00000560: 2020 6163 7175 6973 6974 696f 6e2e 0a20    acquisition.. 
+00000570: 2020 2022 2222 0a0a 2020 2020 2320 4649     """..    # FI
+00000580: 584d 453a 2061 6464 6974 696f 6e61 6c20  XME: additional 
+00000590: 6c69 6665 6379 636c 6520 6d65 7468 6f64  lifecycle method
+000005a0: 733f 0a20 2020 2023 202d 206f 6e5f 7365  s?.    # - on_se
+000005b0: 7475 7020 2d20 6265 666f 7265 2061 726d  tup - before arm
+000005c0: 696e 673f 0a20 2020 2023 202d 206f 6e5f  ing?.    # - on_
+000005d0: 6163 7175 6973 6974 696f 6e5f 646f 6e65  acquisition_done
+000005e0: 202d 2077 6865 6e20 616c 6c20 6461 7461   - when all data
+000005f0: 2068 6173 2062 6565 6e20 7265 6365 6976   has been receiv
+00000600: 6564 2061 6e64 2070 726f 6365 7373 6564  ed and processed
+00000610: 0a0a 2020 2020 6465 6620 6f6e 5f72 6561  ..    def on_rea
+00000620: 6479 5f66 6f72 5f64 6174 6128 7365 6c66  dy_for_data(self
+00000630: 2c20 656e 763a 2052 6561 6479 466f 7244  , env: ReadyForD
+00000640: 6174 6145 6e76 293a 0a20 2020 2020 2020  ataEnv):.       
+00000650: 2022 2222 0a20 2020 2020 2020 2054 6869   """.        Thi
+00000660: 7320 686f 6f6b 2069 7320 6361 6c6c 6564  s hook is called
+00000670: 2077 6865 6e65 7665 7220 7765 2061 7265   whenever we are
+00000680: 2072 6561 6479 2066 6f72 2064 6174 612c   ready for data,
+00000690: 2069 2e65 2e20 7468 6520 6465 7465 6374   i.e. the detect
+000006a0: 6f72 2069 730a 2020 2020 2020 2020 6172  or is.        ar
+000006b0: 6d65 642e 0a0a 2020 2020 2020 2020 5573  med...        Us
+000006c0: 7561 6c6c 792c 2061 7420 7468 6973 2070  ually, at this p
+000006d0: 6f69 6e74 2c20 7468 6520 6e65 7874 2073  oint, the next s
+000006e0: 7465 7020 6973 2074 7269 6767 6572 696e  tep is triggerin
+000006f0: 6720 7468 6520 6d69 6372 6f73 636f 7065  g the microscope
+00000700: 206f 720a 2020 2020 2020 2020 7363 616e   or.        scan
+00000710: 2067 656e 6572 6174 6f72 2074 6f20 7374   generator to st
+00000720: 6172 7420 6120 7363 616e 2e0a 0a20 2020  art a scan...   
+00000730: 2020 2020 2049 7420 6973 206f 6e6c 7920       It is only 
+00000740: 6361 6c6c 6564 2069 6e20 6163 7469 7665  called in active
+00000750: 206d 6f64 652c 2077 6865 7265 2077 6520   mode, where we 
+00000760: 636f 6e74 726f 6c20 7768 656e 2074 6865  control when the
+00000770: 2064 6574 6563 746f 7220 6973 0a20 2020   detector is.   
+00000780: 2020 2020 2061 726d 6564 202d 2069 6e20       armed - in 
+00000790: 7061 7373 6976 6520 6d6f 6465 2c20 7468  passive mode, th
+000007a0: 6520 6461 7461 2069 7320 706f 7373 6962  e data is possib
+000007b0: 6c79 2061 6c72 6561 6479 2062 6569 6e67  ly already being
+000007c0: 2072 6563 6569 7665 6420 616e 640a 2020   received and.  
+000007d0: 2020 2020 2020 7765 2064 6f6e 2774 2063        we don't c
+000007e0: 6f6e 7472 6f6c 2077 6865 6e20 7468 6973  ontrol when this
+000007f0: 2068 6170 7065 6e73 2061 7420 616c 6c2e   happens at all.
+00000800: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00000810: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00000820: 6566 206f 6e5f 6465 7465 726d 696e 655f  ef on_determine_
+00000830: 6e61 765f 7368 6170 6528 0a20 2020 2020  nav_shape(.     
+00000840: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00000850: 2065 6e76 3a20 4465 7465 726d 696e 654e   env: DetermineN
+00000860: 6176 5368 6170 6545 6e76 2c0a 2020 2020  avShapeEnv,.    
+00000870: 2920 2d3e 204f 7074 696f 6e61 6c5b 5475  ) -> Optional[Tu
+00000880: 706c 655b 696e 742c 202e 2e2e 5d5d 3a0a  ple[int, ...]]:.
+00000890: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000008a0: 2020 2020 5468 6973 2068 6f6f 6b20 6973      This hook is
+000008b0: 2063 616c 6c65 6420 746f 2064 6574 6572   called to deter
+000008c0: 6d69 6e65 2074 6865 204e 2d44 206e 6176  mine the N-D nav
+000008d0: 2073 6861 7065 2066 6f72 2074 6865 2061   shape for the a
+000008e0: 6371 7569 7369 7469 6f6e 2e0a 2020 2020  cquisition..    
+000008f0: 2020 2020 5468 6973 2069 7320 6e65 6564      This is need
+00000900: 6564 2061 7320 6d61 6e79 2064 6574 6563  ed as many detec
+00000910: 746f 7273 206f 6e6c 7920 6b6e 6f77 2061  tors only know a
+00000920: 626f 7574 2074 6865 2031 4420 7368 6170  bout the 1D shap
+00000930: 652c 2069 2e65 2e20 7468 650a 2020 2020  e, i.e. the.    
+00000940: 2020 2020 6e75 6d62 6572 206f 6620 696d      number of im
+00000950: 6167 6573 2074 6f20 6163 7175 6972 652e  ages to acquire.
+00000960: 2046 6f72 2073 6f6d 652c 2074 6865 2063   For some, the c
+00000970: 6f6e 7472 6f6c 6c65 7220 6d61 7920 6265  ontroller may be
+00000980: 2061 626c 6520 746f 0a20 2020 2020 2020   able to.       
+00000990: 2064 6574 6572 6d69 6e65 2074 6865 206e   determine the n
+000009a0: 6176 2073 6861 7065 2c20 6275 7420 666f  av shape, but fo
+000009b0: 7220 6f74 6865 7273 2c20 7468 6973 2069  r others, this i
+000009c0: 7320 7370 6563 6966 6963 2074 6f20 7468  s specific to th
+000009d0: 6520 7365 7475 700a 2020 2020 2020 2020  e setup.        
+000009e0: 6f72 2065 7870 6572 696d 656e 742e 0a0a  or experiment...
+000009f0: 2020 2020 2020 2020 5468 6520 7573 6572          The user
+00000a00: 2063 616e 2067 6976 6520 6120 7368 6170   can give a shap
+00000a10: 6520 6869 6e74 2077 6865 6e20 6372 6561  e hint when crea
+00000a20: 7469 6e67 2074 6865 2061 6371 7569 7369  ting the acquisi
+00000a30: 7469 6f6e 206f 626a 6563 742c 0a20 2020  tion object,.   
+00000a40: 2020 2020 2066 6f72 2065 7861 6d70 6c65       for example
+00000a50: 2062 7920 7061 7373 696e 6720 3a63 6f64   by passing :cod
+00000a60: 653a 606e 6176 5f73 6861 7065 3d28 2d31  e:`nav_shape=(-1
+00000a70: 2c20 3235 3629 6020 746f 0a20 2020 2020  , 256)` to.     
+00000a80: 2020 203a 6d65 7468 3a60 7e6c 6962 6572     :meth:`~liber
+00000a90: 7465 6d5f 6c69 7665 2e61 7069 2e4c 6976  tem_live.api.Liv
+00000aa0: 6543 6f6e 7465 7874 2e6d 616b 655f 6163  eContext.make_ac
+00000ab0: 7175 6973 6974 696f 6e60 2e0a 0a20 2020  quisition`...   
+00000ac0: 2020 2020 2049 6620 7468 6520 6465 6661       If the defa
+00000ad0: 756c 7420 6265 6861 7669 6f72 2069 7320  ult behavior is 
+00000ae0: 6e6f 7420 776f 726b 696e 6720 6173 2069  not working as i
+00000af0: 6e74 656e 6465 642c 2074 6865 2075 7365  ntended, the use
+00000b00: 7220 6361 6e20 6f76 6572 7269 6465 0a20  r can override. 
+00000b10: 2020 2020 2020 2074 6869 7320 6d65 7468         this meth
+00000b20: 6f64 2066 6f72 2074 6865 6972 2073 7065  od for their spe
+00000b30: 6369 6669 6320 7365 7475 702e 2045 7861  cific setup. Exa
+00000b40: 6d70 6c65 3a20 6173 6b20 7468 6520 6d69  mple: ask the mi
+00000b50: 6372 6f73 636f 7065 2076 6961 2069 7473  croscope via its
+00000b60: 0a20 2020 2020 2020 2041 5049 2077 6861  .        API wha
+00000b70: 7420 7468 6520 6375 7272 656e 7420 7363  t the current sc
+00000b80: 616e 2073 6574 7469 6e67 7320 6172 652e  an settings are.
+00000b90: 0a0a 2020 2020 2020 2020 4f6e 6c79 2063  ..        Only c
+00000ba0: 616c 6c65 6420 696e 2070 6173 7369 7665  alled in passive
+00000bb0: 206d 6f64 652c 2061 7320 7765 206e 6565   mode, as we nee
+00000bc0: 6420 6120 636f 6e63 7265 7465 2060 6e61  d a concrete `na
+00000bd0: 765f 7368 6170 6560 2061 7320 7573 6572  v_shape` as user
+00000be0: 0a20 2020 2020 2020 2069 6e70 7574 2069  .        input i
+00000bf0: 6e20 6163 7469 7665 206d 6f64 652e 0a0a  n active mode...
+00000c00: 2020 2020 2020 2020 4f72 6465 7220 6f66          Order of
+00000c10: 206f 7065 7261 7469 6f6e 733a 0a0a 2020   operations:..  
+00000c20: 2020 2020 2020 2a20 4966 2074 6865 2060        * If the `
+00000c30: 6e61 765f 7368 6170 6560 2070 6173 7365  nav_shape` passe
+00000c40: 6420 696e 746f 0a20 2020 2020 2020 2020  d into.         
+00000c50: 203a 6d65 7468 3a60 6c69 6265 7274 656d   :meth:`libertem
+00000c60: 5f6c 6976 652e 6170 692e 4c69 7665 436f  _live.api.LiveCo
+00000c70: 6e74 6578 742e 6d61 6b65 5f61 6371 7569  ntext.make_acqui
+00000c80: 7369 7469 6f6e 6020 6973 2063 6f6e 6372  sition` is concr
+00000c90: 6574 652c 2069 2e65 2e0a 2020 2020 2020  ete, i.e..      
+00000ca0: 2020 2020 6973 206e 6f74 2060 4e6f 6e65      is not `None
+00000cb0: 6020 616e 6420 646f 6573 6e27 7420 636f  ` and doesn't co
+00000cc0: 6e74 6169 6e20 616e 7920 602d 3160 2076  ntain any `-1` v
+00000cd0: 616c 7565 732c 2075 7365 2074 6861 740a  alues, use that.
+00000ce0: 2020 2020 2020 2020 2a20 4966 2074 6869          * If thi
+00000cf0: 7320 686f 6f6b 2069 7320 696d 706c 656d  s hook is implem
+00000d00: 656e 7465 6420 616e 6420 7265 7475 726e  ented and return
+00000d10: 7320 6120 7475 706c 652c 2075 7365 2074  s a tuple, use t
+00000d20: 6861 740a 2020 2020 2020 2020 2a20 4966  hat.        * If
+00000d30: 2074 6865 2063 6f6e 7472 6f6c 6c65 7220   the controller 
+00000d40: 666f 7220 7468 6520 7370 6563 6966 6963  for the specific
+00000d50: 2064 6574 6563 746f 7220 7479 7065 2063   detector type c
+00000d60: 616e 2067 6976 6520 7573 0a20 2020 2020  an give us.     
+00000d70: 2020 2020 2074 6865 2063 6f6e 6372 6574       the concret
+00000d80: 6520 606e 6176 5f73 6861 7065 602c 2075  e `nav_shape`, u
+00000d90: 7365 2074 6861 740a 2020 2020 2020 2020  se that.        
+00000da0: 2a20 4966 206e 6f6e 6520 6f66 2074 6865  * If none of the
+00000db0: 2061 626f 7665 2073 7563 6365 6564 2c20   above succeed, 
+00000dc0: 7472 7920 746f 206d 616b 6520 6120 7371  try to make a sq
+00000dd0: 7561 7265 206f 7574 206f 6620 7468 650a  uare out of the.
+00000de0: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
+00000df0: 206f 6620 6672 616d 6573 0a20 2020 2020   of frames.     
+00000e00: 2020 202a 2049 6620 616c 6c20 6162 6f76     * If all abov
+00000e10: 6520 6661 696c 732c 2072 6169 7365 2061  e fails, raise a
+00000e20: 2060 5275 6e74 696d 6545 7272 6f72 600a   `RuntimeError`.
+00000e30: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00000e40: 2020 2020 7061 7373 0a                       pass.
```

### Comparing `libertem-live-0.2.0/src/libertem_live/api.py` & `libertem-live-0.2.1/src/libertem_live/api.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/LICENSE` & `libertem-live-0.2.1/src/libertem_live/detectors/LICENSE`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/acquisition.py` & `libertem-live-0.2.1/src/libertem_live/detectors/asi_tpx3/acquisition.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
         return (depth, *self.meta.shape.sig)
         # return Shape((self._end_idx - self._start_idx, 256, 256), sig_dims=2)
 
     def get_max_io_size(self):
         ""
         # return 12*256*256*8
         # FIXME magic numbers?
-        return 1200000*np.prod(self.meta.shape.sig)*8
+        return 1200000 * prod(self.meta.shape.sig) * 8
 
     def get_base_shape(self, roi):
         ""
         return (1, *self.meta.shape.sig)
 
     def get_partitions(self):
         ""
```

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/connection.py` & `libertem-live-0.2.1/src/libertem_live/detectors/asi_tpx3/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         huge_pages: bool = False,
     ):
         self._passive_started = False
         self._data_host = data_host
         self._data_port = data_port
 
         if bytes_per_chunk is None:
-            bytes_per_chunk = 16*1024
+            bytes_per_chunk = 16 * 1024
 
         # approx:
         slot_size = bytes_per_chunk * chunks_per_stack
         self._num_slots = 1024 * 1024 * buffer_size // slot_size
 
         self._bytes_per_chunk = bytes_per_chunk
         self._huge_pages = huge_pages
```

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/sim.py` & `libertem-live-0.2.1/src/libertem_live/detectors/asi_tpx3/sim.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #!/usr/bin/env python
 import threading
-from typing import Optional, List
+from typing import Optional, List, Tuple
 import logging
 import socket
+import mmap
 import time
 import sys
 import os
 
 import numpy as np
 import click
 
 from libertem_live.detectors.common import (
     ServerThreadMixin,
     UndeadException,
 )
+from libertem.common.math import prod
 
 logger = logging.getLogger(__name__)
 
 
 def send_full_file(cache_fd, total_size, conn):
     os.lseek(cache_fd, 0, 0)
     total_sent = 0
@@ -35,66 +37,71 @@
         raise NotImplementedError()
 
     @property
     def full_size(self) -> int:
         raise NotImplementedError()
 
 
-class MemfdCachedSource(CachedDataSource):
-    def __init__(self, paths: List[str]):
+class BufferedCachedSource(CachedDataSource):
+    def __init__(
+        self,
+        paths: Optional[List[str]] = None,
+        mock_nav_shape: Optional[Tuple[int, int]] = None
+    ):
         self._paths = paths
-        self._cache_data(paths)
-
-    def _cache_data(self, paths: List[str]):
-        import memfd  # local import so it works without it
-        logger.info("populating cache...")
-        cache_fd = memfd.memfd_create("tpx_cache", 0)
-        total_size = 0
-        for path in paths:
-            written = 0
-            logger.info(f"reading {path}")
-            with open(path, "rb") as f:
-                in_bytes = f.read()
-                while written < len(in_bytes):
-                    written += os.write(cache_fd, in_bytes[written:])
-            total_size += written
-        os.lseek(cache_fd, 0, 0)
-        self._cache_fd = cache_fd
+        if paths is not None:
+            self._cache_data(paths)
+        if mock_nav_shape is not None:
+            self._cache_data_mock(mock_nav_shape)
+
+    def _make_cache(self, total_size_bytes: int):
+        self._cache = np.empty(total_size_bytes, dtype=np.uint8)
+
+    def _get_cache_view(self):
+        return memoryview(self._cache)  # type: ignore
+
+    def _cache_data_mock(self, mock_nav_shape: Tuple[int, int]):
+        data = self._make_mock_data(mock_nav_shape)
+        total_size = len(data)
+        self._make_cache(total_size)
+        cache_view = self._get_cache_view()
+        cache_view[:] = data
         self._total_size = total_size
-        logger.info(f"cache populated, total_size={total_size}")
-
-    def send_data(self, conn: socket.socket) -> int:
-        send_full_file(self._cache_fd, self._total_size, conn)
-        return self.full_size
-
-    @property
-    def full_size(self) -> int:
-        return self._total_size
 
-
-class BufferedCachedSource(CachedDataSource):
-    def __init__(self, paths: List[str]):
-        self._paths = paths
-        self._cache_data(paths)
+    def _make_mock_data(self, mock_nav_shape: Tuple[int, int]) -> np.ndarray:
+        import sparse
+        import sparseconverter
+        from libertem_asi_tpx3 import make_sim_data
+        sig_shape = (512, 512)
+        full_shape_flat = (prod(mock_nav_shape), prod(sig_shape))
+        arr = sparse.DOK(shape=full_shape_flat, dtype=np.uint32)
+        sig_size = prod(sig_shape)
+        for idx in range(prod(mock_nav_shape)):
+            arr[idx, idx % sig_size] = idx
+        c = sparseconverter.for_backend(arr, 'scipy.sparse.csr_matrix', strict=True)
+        mock_data = np.array(make_sim_data(
+            mock_nav_shape, c.indptr, c.indices, c.data
+        ), dtype='uint8')
+        return mock_data
 
     def _cache_data(self, paths: List[str]):
         logger.info("populating cache...")
         total_size = 0
         for path in paths:
             total_size += os.stat(path).st_size
 
-        self._cache = np.empty(total_size, dtype=np.uint8)
+        self._make_cache(total_size)
+        cache_view = self._get_cache_view()
 
         for path in paths:
-            cache_view = memoryview(self._cache)  # type: ignore
             offset = 0
             with open(path, "rb") as f:
                 in_bytes = f.read()
                 length = len(in_bytes)
-                cache_view[offset:offset+length] = in_bytes
+                cache_view[offset:offset + length] = in_bytes
                 offset += length
 
         self._total_size = total_size
         logger.info(f"cache populated, total_size={total_size}")
 
     def send_data(self, conn: socket.socket) -> int:
         cache_view = memoryview(self._cache)  # type: ignore
@@ -102,14 +109,49 @@
         return self.full_size
 
     @property
     def full_size(self) -> int:
         return self._total_size
 
 
+class MemfdCachedSource(BufferedCachedSource):
+    def __init__(
+        self,
+        paths: Optional[List[str]] = None,
+        mock_nav_shape: Optional[Tuple[int, int]] = None
+    ):
+        self._mmap = None
+        super().__init__(paths=paths, mock_nav_shape=mock_nav_shape)
+
+    def _make_cache(self, total_size_bytes: int):
+        import memfd  # local import so the other classes work without it
+        cache_fd = memfd.memfd_create("tpx_cache", 0)
+        os.truncate(cache_fd, total_size_bytes)
+        self._cache_fd = cache_fd
+
+    def _get_cache_view(self):
+        if self._mmap is None:
+            self._mmap = mmap.mmap(
+                self._cache_fd,
+                length=0,
+                flags=mmap.MAP_SHARED,
+                prot=mmap.PROT_WRITE | mmap.PROT_READ,
+            )
+        return memoryview(self._mmap)
+
+    def send_data(self, conn: socket.socket) -> int:
+        os.lseek(self._cache_fd, 0, 0)
+        send_full_file(self._cache_fd, self._total_size, conn)
+        return self.full_size
+
+    @property
+    def full_size(self) -> int:
+        return self._total_size
+
+
 class TpxSim:
     def __init__(
         self,
         sleep: float,
         data_source: CachedDataSource,
         stop_event: Optional[threading.Event] = None,
     ):
@@ -129,20 +171,20 @@
                 t0 = time.perf_counter()
                 try:
                     size = self._data_source.send_data(conn)
                 except Exception as e:
                     logger.error("exception while sending data: %s", str(e))
                     raise
                 t1 = time.perf_counter()
-                thp = size / 1024 / 1024 / (t1-t0)
+                thp = size / 1024 / 1024 / (t1 - t0)
                 total_sent_this_conn += size
                 logger.info(f"done in {t1-t0:.3f}s, throughput={thp:.3f}MiB/s")
                 time.sleep(self._sleep)
                 t2 = time.perf_counter()
-                thp_with_sleep = size / 1024 / 1024 / (t2-t0)
+                thp_with_sleep = size / 1024 / 1024 / (t2 - t0)
                 logger.info(f"throughput_with_sleep={thp_with_sleep:.3f}MiB/s")
         finally:
             total = total_sent_this_conn / 1024 / 1024 / 1024
             logger.info(
                 f"connection closed, total_sent = {total:.3f}GiB"
             )
 
@@ -155,24 +197,26 @@
     def handle_conn(self, connection: socket.socket):
         self._sim.handle_conn(connection)
 
 
 class TpxCameraSim:
     def __init__(
         self,
-        paths: List[str],
+        *,
         cached: str,
         port: int,
         sleep: float,
+        paths: Optional[List[str]] = None,
+        mock_nav_shape: Optional[Tuple[int, int]] = None,
     ):
         src: CachedDataSource
         if cached.lower() == 'mem':
-            src = BufferedCachedSource(paths=paths)
+            src = BufferedCachedSource(paths=paths, mock_nav_shape=mock_nav_shape)
         elif cached.lower() == 'memfd':
-            src = MemfdCachedSource(paths=paths)
+            src = MemfdCachedSource(paths=paths, mock_nav_shape=mock_nav_shape)
         else:
             raise ValueError(f"unknown cache type: {cached}")
 
         self.stop_event = threading.Event()
 
         sim = TpxSim(
             sleep=sleep,
@@ -228,24 +272,32 @@
     nargs=-1
 )
 @click.option('--sleep', type=float, default=0.0)
 @click.option('--port', type=int, default=8283)
 @click.option('--cached', default='MEM', type=click.Choice(
     ['MEM', 'MEMFD'], case_sensitive=False)
 )
-def main(cached: str, paths, sleep: float, port: int = 8283):
+@click.option('--mock-nav-shape', type=(int, int), default=None)
+def main(cached: str, paths, sleep: float, port: int = 8283, mock_nav_shape=None):
     logging.basicConfig(level=logging.INFO)
 
     logger.info(f"port={port}")
 
+    if not paths:
+        # Otherwise empty tuple
+        paths = None
+    if paths is None and mock_nav_shape is None:
+        raise ValueError('Need one of paths or mock_nav_shape')
+
     sim = TpxCameraSim(
         paths=paths,
         cached=cached,
         port=port,
         sleep=sleep,
+        mock_nav_shape=mock_nav_shape,
     )
     sim.start()
 
     # This allows us to handle Ctrl-C, and the main program
     # stops in a timely fashion when continuous scanning stops.
     try:
         while sim.is_alive():
```

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/connection.cpython-310.pyc` & `libertem-live-0.2.1/src/libertem_live/detectors/memory/acquisition.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,204 +1,221 @@
-00000000: 6f0d 0d0a 0000 0000 87dc 3f64 fd08 0000  o.........?d....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
-00000040: 0100 6402 6403 6c04 6d05 5a05 0100 4700  ..d.d.l.m.Z...G.
-00000050: 6404 6405 8400 6405 8302 5a06 4700 6406  d.d...d...Z.G.d.
-00000060: 6407 8400 6407 8302 5a07 6408 5300 2909  d...d...Z.d.S.).
-00000070: e900 0000 0029 03da 084f 7074 696f 6e61  .....)...Optiona
-00000080: 6cda 0454 7970 65da 0554 7570 6c65 e901  l..Type..Tuple..
-00000090: 0000 0029 01da 1341 6371 7569 7369 7469  ...)...Acquisiti
-000000a0: 6f6e 5072 6f74 6f63 6f6c 6300 0000 0000  onProtocolc.....
-000000b0: 0000 0000 0000 0000 0000 0006 0000 0040  ...............@
-000000c0: 0000 0073 4000 0000 6500 5a01 6400 5a02  ...s@...e.Z.d.Z.
-000000d0: 6401 5a03 6504 6402 6505 6602 6403 6404  d.Z.e.d.e.f.d.d.
-000000e0: 8404 8301 5a06 6504 6402 6507 6508 6505  ....Z.e.d.e.e.e.
-000000f0: 6405 6602 1900 1900 6602 6406 6407 8404  d.f.....f.d.d...
-00000100: 8301 5a09 6408 5300 2909 da12 5065 6e64  ..Z.d.S.)...Pend
-00000110: 696e 6741 6371 7569 7369 7469 6f6e 6113  ingAcquisitiona.
-00000120: 0100 000a 2020 2020 4120 746f 6b65 6e20  ....    A token 
-00000130: 6f62 6a65 6374 2074 6861 7420 6361 6e20  object that can 
-00000140: 6265 206f 6274 6169 6e65 6420 6672 6f6d  be obtained from
-00000150: 0a20 2020 203a 6d65 7468 3a60 6c69 6265  .    :meth:`libe
-00000160: 7274 656d 5f6c 6976 652e 6465 7465 6374  rtem_live.detect
-00000170: 6f72 732e 6261 7365 2e63 6f6e 6e65 6374  ors.base.connect
-00000180: 696f 6e2e 4465 7465 6374 6f72 436f 6e6e  ion.DetectorConn
-00000190: 6563 7469 6f6e 2e77 6169 745f 666f 725f  ection.wait_for_
-000001a0: 6163 7175 6973 6974 696f 6e60 2e0a 0a20  acquisition`... 
-000001b0: 2020 2050 6173 7320 7468 6973 206f 626a     Pass this obj
-000001c0: 6563 7420 696e 746f 203a 6d65 7468 3a60  ect into :meth:`
-000001d0: 6c69 6265 7274 656d 5f6c 6976 652e 6170  libertem_live.ap
-000001e0: 692e 4c69 7665 436f 6e74 6578 742e 6d61  i.LiveContext.ma
-000001f0: 6b65 5f61 6371 7569 7369 7469 6f6e 600a  ke_acquisition`.
-00000200: 2020 2020 746f 2073 7461 7274 2070 726f      to start pro
-00000210: 6365 7373 696e 6720 7468 6520 696e 636f  cessing the inco
-00000220: 6d69 6e67 2064 6174 6120 7374 7265 616d  ming data stream
-00000230: 2e0a 2020 2020 da06 7265 7475 726e 6301  ..    ..returnc.
-00000240: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00000250: 0000 0043 0000 00f3 0600 0000 7400 8300  ...C........t...
-00000260: 8201 2901 7a53 0a20 2020 2020 2020 2054  ..).zS.        T
-00000270: 6865 2074 6f74 616c 206e 756d 6265 7220  he total number 
-00000280: 6f66 2069 6d61 6765 7320 7468 6174 2061  of images that a
-00000290: 7265 2065 7870 6563 7465 6420 666f 7220  re expected for 
-000002a0: 7468 6973 2061 6371 7569 7369 7469 6f6e  this acquisition
-000002b0: 0a20 2020 2020 2020 20a9 01da 134e 6f74  .        ....Not
-000002c0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-000002d0: a901 da04 7365 6c66 a900 720e 0000 00fa  ....self..r.....
-000002e0: 432f 617a 702f 6167 656e 742f 5f77 6f72  C/azp/agent/_wor
-000002f0: 6b2f 312f 732f 7372 632f 6c69 6265 7274  k/1/s/src/libert
-00000300: 656d 5f6c 6976 652f 6465 7465 6374 6f72  em_live/detector
-00000310: 732f 6261 7365 2f63 6f6e 6e65 6374 696f  s/base/connectio
-00000320: 6e2e 7079 da07 6e69 6d61 6765 730e 0000  n.py..nimages...
-00000330: 0073 0200 0000 0605 7a1a 5065 6e64 696e  .s......z.Pendin
-00000340: 6741 6371 7569 7369 7469 6f6e 2e6e 696d  gAcquisition.nim
-00000350: 6167 6573 2e63 0100 0000 0000 0000 0000  ages.c..........
-00000360: 0000 0100 0000 0100 0000 4300 0000 7304  ..........C...s.
-00000370: 0000 0064 0153 0029 027a 4a0a 2020 2020  ...d.S.).zJ.    
-00000380: 2020 2020 5468 6520 636f 6e63 7265 7465      The concrete
-00000390: 2060 6e61 765f 7368 6170 6560 2c20 6966   `nav_shape`, if
-000003a0: 2069 7420 6973 206b 6e6f 776e 2062 7920   it is known by 
-000003b0: 7468 6520 6465 7465 6374 6f72 0a20 2020  the detector.   
-000003c0: 2020 2020 204e 720e 0000 0072 0c00 0000       Nr....r....
-000003d0: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
-000003e0: 096e 6176 5f73 6861 7065 1500 0000 7302  .nav_shape....s.
-000003f0: 0000 0004 057a 1c50 656e 6469 6e67 4163  .....z.PendingAc
-00000400: 7175 6973 6974 696f 6e2e 6e61 765f 7368  quisition.nav_sh
-00000410: 6170 654e 290a da08 5f5f 6e61 6d65 5f5f  apeN)...__name__
-00000420: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000430: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00000440: 635f 5fda 0870 726f 7065 7274 79da 0369  c__..property..i
-00000450: 6e74 7210 0000 0072 0200 0000 7204 0000  ntr....r....r...
-00000460: 0072 1100 0000 720e 0000 0072 0e00 0000  .r....r....r....
-00000470: 720e 0000 0072 0f00 0000 7207 0000 0006  r....r....r.....
-00000480: 0000 0073 0c00 0000 0800 0401 0207 1001  ...s............
-00000490: 0206 2001 7207 0000 0063 0000 0000 0000  .. .r....c......
-000004a0: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
-000004b0: 0000 7356 0000 0065 005a 0164 005a 0264  ..sV...e.Z.d.Z.d
-000004c0: 015a 0364 0f64 0365 0465 0519 0064 0465  .Z.d.d.e.e...d.e
-000004d0: 0465 0619 0066 0464 0564 0684 055a 0764  .e...f.d.d...Z.d
-000004e0: 0764 0884 005a 0864 0964 0a84 005a 0964  .d...Z.d.d...Z.d
-000004f0: 0b64 0c84 005a 0a64 0465 0b65 0c19 0066  .d...Z.d.e.e...f
-00000500: 0264 0d64 0e84 045a 0d64 0253 0029 10da  .d.d...Z.d.S.)..
-00000510: 1244 6574 6563 746f 7243 6f6e 6e65 6374  .DetectorConnect
-00000520: 696f 6e7a 2e0a 2020 2020 4261 7365 2063  ionz..    Base c
-00000530: 6c61 7373 2066 6f72 2064 6574 6563 746f  lass for detecto
-00000540: 7220 636f 6e6e 6563 7469 6f6e 732e 0a20  r connections.. 
-00000550: 2020 204e da07 7469 6d65 6f75 7472 0800     N..timeoutr..
-00000560: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00000570: 0000 0001 0000 0043 0000 0072 0900 0000  .......C...r....
-00000580: 2901 614d 0200 000a 2020 2020 2020 2020  ).aM....        
-00000590: 5761 6974 2066 6f72 2061 7420 6d6f 7374  Wait for at most
-000005a0: 2060 7469 6d65 6f75 7460 2073 6563 6f6e   `timeout` secon
-000005b0: 6473 2066 6f72 2061 6e20 6163 7175 6973  ds for an acquis
-000005c0: 6974 696f 6e20 746f 2073 7461 7274 2e20  ition to start. 
-000005d0: 5468 6973 0a20 2020 2020 2020 2064 6f65  This.        doe
-000005e0: 7320 6e6f 7420 7065 7266 6f72 6d20 616e  s not perform an
-000005f0: 7920 7472 6967 6765 7269 6e67 2069 7473  y triggering its
-00000600: 656c 6620 616e 6420 6578 7065 6374 7320  elf and expects 
-00000610: 736f 6d65 7468 696e 6720 6578 7465 726e  something extern
-00000620: 616c 0a20 2020 2020 2020 2074 6f20 6172  al.        to ar
-00000630: 6d20 616e 6420 7472 6967 6765 7220 7468  m and trigger th
-00000640: 6520 6163 7175 6973 6974 696f 6e2e 0a0a  e acquisition...
-00000650: 2020 2020 2020 2020 4f6e 6365 2074 6865          Once the
-00000660: 2064 6574 6563 746f 7220 6973 2061 726d   detector is arm
-00000670: 6564 2c20 7468 6973 2066 756e 6374 696f  ed, this functio
-00000680: 6e20 7265 7475 726e 7320 6120 6050 656e  n returns a `Pen
-00000690: 6469 6e67 4163 7175 6973 6974 696f 6e60  dingAcquisition`
-000006a0: 2c0a 2020 2020 2020 2020 7768 6963 6820  ,.        which 
-000006b0: 6361 6e20 6265 2063 6f6e 7665 7274 6564  can be converted
-000006c0: 2074 6f20 6120 6675 6c6c 2060 4163 7175   to a full `Acqu
-000006d0: 6973 6974 696f 6e60 206f 626a 6563 7420  isition` object 
-000006e0: 7573 696e 670a 2020 2020 2020 2020 3a6d  using.        :m
-000006f0: 6574 683a 606c 6962 6572 7465 6d5f 6c69  eth:`libertem_li
-00000700: 7665 2e61 7069 2e4c 6976 6543 6f6e 7465  ve.api.LiveConte
-00000710: 7874 2e6d 616b 655f 6163 7175 6973 6974  xt.make_acquisit
-00000720: 696f 6e60 2e0a 0a20 2020 2020 2020 2054  ion`...        T
-00000730: 6865 2066 756e 6374 696f 6e20 7265 7475  he function retu
-00000740: 726e 7320 604e 6f6e 6560 206f 6e20 7469  rns `None` on ti
-00000750: 6d65 6f75 742e 0a0a 2020 2020 2020 2020  meout...        
-00000760: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00000770: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00000780: 2020 2020 2020 7469 6d65 6f75 740a 2020        timeout.  
-00000790: 2020 2020 2020 2020 2020 5469 6d65 6f75            Timeou
-000007a0: 7420 696e 2073 6563 6f6e 6473 2e20 4966  t in seconds. If
-000007b0: 2060 4e6f 6e65 602c 2077 6169 7420 696e   `None`, wait in
-000007c0: 6465 6669 6e69 7465 6c79 2e0a 2020 2020  definitely..    
-000007d0: 2020 2020 720a 0000 0029 0272 0d00 0000      r....).r....
-000007e0: 7219 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-000007f0: 0f00 0000 da14 7761 6974 5f66 6f72 5f61  ......wait_for_a
-00000800: 6371 7569 7369 7469 6f6e 2100 0000 7302  cquisition!...s.
-00000810: 0000 0006 117a 2744 6574 6563 746f 7243  .....z'DetectorC
-00000820: 6f6e 6e65 6374 696f 6e2e 7761 6974 5f66  onnection.wait_f
-00000830: 6f72 5f61 6371 7569 7369 7469 6f6e 6301  or_acquisitionc.
-00000840: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00000850: 0000 0043 0000 0072 0900 0000 2901 6142  ...C...r....).aB
-00000860: 0100 000a 2020 2020 2020 2020 436c 6f73  ....        Clos
-00000870: 6520 7468 6520 636f 6e6e 6563 7469 6f6e  e the connection
-00000880: 2e20 4974 2773 2069 6d70 6f72 7461 6e74  . It's important
-00000890: 2074 6f20 6361 6c6c 2074 6869 7320 6675   to call this fu
-000008a0: 6e63 7469 6f6e 206f 6e63 650a 2020 2020  nction once.    
-000008b0: 2020 2020 796f 7520 646f 6e27 7420 6e65      you don't ne
-000008c0: 6564 2074 6865 2063 6f6e 6e65 6374 696f  ed the connectio
-000008d0: 6e20 616e 796d 6f72 652c 2061 7320 616e  n anymore, as an
-000008e0: 206f 7065 6e20 636f 6e6e 6563 7469 6f6e   open connection
-000008f0: 0a20 2020 2020 2020 206d 6967 6874 2069  .        might i
-00000900: 6e74 6572 6665 7265 2077 6974 6820 6f74  nterfere with ot
-00000910: 6865 7220 736f 6674 7761 7265 2075 7369  her software usi
-00000920: 6e67 2074 6865 2064 6574 6563 746f 722e  ng the detector.
-00000930: 0a0a 2020 2020 2020 2020 4966 2070 6f73  ..        If pos
-00000940: 7369 626c 652c 2075 7365 2074 6869 7320  sible, use this 
-00000950: 6f62 6a65 6374 2061 7320 6120 636f 6e74  object as a cont
-00000960: 6578 7420 6d61 6e61 6765 7220 696e 7374  ext manager inst
-00000970: 6561 642c 0a20 2020 2020 2020 2075 7369  ead,.        usi
-00000980: 6e67 2061 203a 636f 6465 3a60 7769 7468  ng a :code:`with
-00000990: 602d 7374 6174 656d 656e 742e 0a20 2020  `-statement..   
-000009a0: 2020 2020 2072 0a00 0000 720c 0000 0072       r....r....r
-000009b0: 0e00 0000 720e 0000 0072 0f00 0000 da05  ....r....r......
-000009c0: 636c 6f73 6534 0000 0073 0200 0000 0609  close4...s......
-000009d0: 7a18 4465 7465 6374 6f72 436f 6e6e 6563  z.DetectorConnec
-000009e0: 7469 6f6e 2e63 6c6f 7365 6301 0000 0000  tion.closec.....
-000009f0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00000a00: 0000 0073 0400 0000 7c00 5300 a901 4e72  ...s....|.S...Nr
-00000a10: 0e00 0000 720c 0000 0072 0e00 0000 720e  ....r....r....r.
-00000a20: 0000 0072 0f00 0000 da09 5f5f 656e 7465  ...r......__ente
-00000a30: 725f 5f3f 0000 0073 0200 0000 0401 7a1c  r__?...s......z.
-00000a40: 4465 7465 6374 6f72 436f 6e6e 6563 7469  DetectorConnecti
-00000a50: 6f6e 2e5f 5f65 6e74 6572 5f5f 6304 0000  on.__enter__c...
-00000a60: 0000 0000 0000 0000 0004 0000 0002 0000  ................
-00000a70: 0043 0000 0073 0c00 0000 7c00 a000 a100  .C...s....|.....
-00000a80: 0100 6400 5300 721c 0000 0029 0172 1b00  ..d.S.r....).r..
-00000a90: 0000 2904 720d 0000 00da 0865 7863 5f74  ..).r......exc_t
-00000aa0: 7970 65da 0965 7863 5f76 616c 7565 da09  ype..exc_value..
-00000ab0: 7472 6163 6562 6163 6b72 0e00 0000 720e  tracebackr....r.
-00000ac0: 0000 0072 0f00 0000 da08 5f5f 6578 6974  ...r......__exit
-00000ad0: 5f5f 4200 0000 7302 0000 000c 017a 1b44  __B...s......z.D
-00000ae0: 6574 6563 746f 7243 6f6e 6e65 6374 696f  etectorConnectio
-00000af0: 6e2e 5f5f 6578 6974 5f5f 6301 0000 0000  n.__exit__c.....
-00000b00: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00000b10: 0000 0072 0900 0000 2901 7a53 0a20 2020  ...r....).zS.   
-00000b20: 2020 2020 2052 6574 7572 6e73 2074 6865       Returns the
-00000b30: 206d 6174 6368 696e 6720 6041 6371 7569   matching `Acqui
-00000b40: 7369 7469 6f6e 6020 636c 6173 732e 0a0a  sition` class...
-00000b50: 2020 2020 2020 2020 3a6d 6574 6120 7072          :meta pr
-00000b60: 6976 6174 653a 0a20 2020 2020 2020 2072  ivate:.        r
-00000b70: 0a00 0000 720c 0000 0072 0e00 0000 720e  ....r....r....r.
-00000b80: 0000 0072 0f00 0000 da13 6765 745f 6163  ...r......get_ac
-00000b90: 7175 6973 6974 696f 6e5f 636c 7345 0000  quisition_clsE..
-00000ba0: 0073 0200 0000 0606 7a26 4465 7465 6374  .s......z&Detect
-00000bb0: 6f72 436f 6e6e 6563 7469 6f6e 2e67 6574  orConnection.get
-00000bc0: 5f61 6371 7569 7369 7469 6f6e 5f63 6c73  _acquisition_cls
-00000bd0: 721c 0000 0029 0e72 1200 0000 7213 0000  r....).r....r...
-00000be0: 0072 1400 0000 7215 0000 0072 0200 0000  .r....r....r....
-00000bf0: da05 666c 6f61 7472 0700 0000 721a 0000  ..floatr....r...
-00000c00: 0072 1b00 0000 721d 0000 0072 2100 0000  .r....r....r!...
-00000c10: 7203 0000 0072 0600 0000 7222 0000 0072  r....r....r"...r
-00000c20: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
-00000c30: 0000 0072 1800 0000 1d00 0000 730e 0000  ...r........s...
-00000c40: 0008 0004 011c 0308 1308 0b08 0316 0372  ...............r
-00000c50: 1800 0000 4e29 08da 0674 7970 696e 6772  ....N)...typingr
-00000c60: 0200 0000 7203 0000 0072 0400 0000 da0b  ....r....r......
-00000c70: 6163 7175 6973 6974 696f 6e72 0600 0000  acquisitionr....
-00000c80: 7207 0000 0072 1800 0000 720e 0000 0072  r....r....r....r
-00000c90: 0e00 0000 720e 0000 0072 0f00 0000 da08  ....r....r......
-00000ca0: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
-00000cb0: 0014 000c 020e 0312 17                   .........
+00000000: 6672 6f6d 2063 6f6e 7465 7874 6c69 6220  from contextlib 
+00000010: 696d 706f 7274 2063 6f6e 7465 7874 6d61  import contextma
+00000020: 6e61 6765 720a 6672 6f6d 2074 7970 696e  nager.from typin
+00000030: 6720 696d 706f 7274 2044 6963 742c 204f  g import Dict, O
+00000040: 7074 696f 6e61 6c2c 2054 7570 6c65 2c20  ptional, Tuple, 
+00000050: 5479 7065 0a69 6d70 6f72 7420 6c6f 6767  Type.import logg
+00000060: 696e 670a 0a69 6d70 6f72 7420 6e75 6d70  ing..import nump
+00000070: 7920 6173 206e 700a 0a66 726f 6d20 6c69  y as np..from li
+00000080: 6265 7274 656d 2e69 6f2e 6461 7461 7365  bertem.io.datase
+00000090: 742e 6d65 6d6f 7279 2069 6d70 6f72 7420  t.memory import 
+000000a0: 4d65 6d6f 7279 4461 7461 5365 740a 0a66  MemoryDataSet..f
+000000b0: 726f 6d20 6c69 6265 7274 656d 5f6c 6976  rom libertem_liv
+000000c0: 652e 686f 6f6b 7320 696d 706f 7274 2048  e.hooks import H
+000000d0: 6f6f 6b73 2c20 5265 6164 7946 6f72 4461  ooks, ReadyForDa
+000000e0: 7461 456e 760a 6672 6f6d 206c 6962 6572  taEnv.from liber
+000000f0: 7465 6d5f 6c69 7665 2e64 6574 6563 746f  tem_live.detecto
+00000100: 7273 2e62 6173 652e 6163 7175 6973 6974  rs.base.acquisit
+00000110: 696f 6e20 696d 706f 7274 2041 6371 7569  ion import Acqui
+00000120: 7369 7469 6f6e 4d69 7869 6e0a 6672 6f6d  sitionMixin.from
+00000130: 206c 6962 6572 7465 6d5f 6c69 7665 2e64   libertem_live.d
+00000140: 6574 6563 746f 7273 2e62 6173 652e 636f  etectors.base.co
+00000150: 6e6e 6563 7469 6f6e 2069 6d70 6f72 7420  nnection import 
+00000160: 4465 7465 6374 6f72 436f 6e6e 6563 7469  DetectorConnecti
+00000170: 6f6e 2c20 5065 6e64 696e 6741 6371 7569  on, PendingAcqui
+00000180: 7369 7469 6f6e 0a23 2066 726f 6d20 6c69  sition.# from li
+00000190: 6265 7274 656d 5f6c 6976 652e 6465 7465  bertem_live.dete
+000001a0: 6374 6f72 732e 6261 7365 2e63 6f6e 7472  ctors.base.contr
+000001b0: 6f6c 6c65 7220 696d 706f 7274 2041 6371  oller import Acq
+000001c0: 7569 7369 7469 6f6e 436f 6e74 726f 6c6c  uisitionControll
+000001d0: 6572 0a0a 6c6f 6767 6572 203d 206c 6f67  er..logger = log
+000001e0: 6769 6e67 2e67 6574 4c6f 6767 6572 285f  ging.getLogger(_
+000001f0: 5f6e 616d 655f 5f29 0a0a 0a63 6c61 7373  _name__)...class
+00000200: 204d 656d 6f72 7943 6f6e 6e65 6374 696f   MemoryConnectio
+00000210: 6e28 4465 7465 6374 6f72 436f 6e6e 6563  n(DetectorConnec
+00000220: 7469 6f6e 293a 0a20 2020 2064 6566 205f  tion):.    def _
+00000230: 5f69 6e69 745f 5f28 7365 6c66 2c20 6461  _init__(self, da
+00000240: 7461 3a20 6e70 2e6e 6461 7272 6179 2c20  ta: np.ndarray, 
+00000250: 6578 7472 615f 6b77 6172 6773 3a20 4f70  extra_kwargs: Op
+00000260: 7469 6f6e 616c 5b44 6963 745d 203d 204e  tional[Dict] = N
+00000270: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
+00000280: 6c66 2e5f 6461 7461 203d 2064 6174 610a  lf._data = data.
+00000290: 2020 2020 2020 2020 6966 2065 7874 7261          if extra
+000002a0: 5f6b 7761 7267 7320 6973 204e 6f6e 653a  _kwargs is None:
+000002b0: 0a20 2020 2020 2020 2020 2020 2065 7874  .            ext
+000002c0: 7261 5f6b 7761 7267 7320 3d20 7b7d 0a20  ra_kwargs = {}. 
+000002d0: 2020 2020 2020 2073 656c 662e 5f65 7874         self._ext
+000002e0: 7261 5f6b 7761 7267 7320 3d20 6578 7472  ra_kwargs = extr
+000002f0: 615f 6b77 6172 6773 0a0a 2020 2020 6465  a_kwargs..    de
+00000300: 6620 7761 6974 5f66 6f72 5f61 6371 7569  f wait_for_acqui
+00000310: 7369 7469 6f6e 2873 656c 662c 2074 696d  sition(self, tim
+00000320: 656f 7574 3a20 4f70 7469 6f6e 616c 5b66  eout: Optional[f
+00000330: 6c6f 6174 5d20 3d20 4e6f 6e65 2920 2d3e  loat] = None) ->
+00000340: 204f 7074 696f 6e61 6c5b 5065 6e64 696e   Optional[Pendin
+00000350: 6741 6371 7569 7369 7469 6f6e 5d3a 0a20  gAcquisition]:. 
+00000360: 2020 2020 2020 2072 6574 7572 6e20 5065         return Pe
+00000370: 6e64 696e 674d 656d 4171 2829 0a0a 2020  ndingMemAq()..  
+00000380: 2020 6465 6620 6765 745f 6163 7175 6973    def get_acquis
+00000390: 6974 696f 6e5f 636c 7328 7365 6c66 2920  ition_cls(self) 
+000003a0: 2d3e 2054 7970 655b 4163 7175 6973 6974  -> Type[Acquisit
+000003b0: 696f 6e4d 6978 696e 5d3a 0a20 2020 2020  ionMixin]:.     
+000003c0: 2020 2072 6574 7572 6e20 4d65 6d6f 7279     return Memory
+000003d0: 4163 7175 6973 6974 696f 6e0a 0a20 2020  Acquisition..   
+000003e0: 2064 6566 2063 6c6f 7365 2873 656c 6629   def close(self)
+000003f0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00000400: 0a63 6c61 7373 204d 656d 6f72 7943 6f6e  .class MemoryCon
+00000410: 6e65 6374 696f 6e42 7569 6c64 6572 3a0a  nectionBuilder:.
+00000420: 2020 2020 6465 6620 6f70 656e 2873 656c      def open(sel
+00000430: 662c 2064 6174 613a 206e 702e 6e64 6172  f, data: np.ndar
+00000440: 7261 792c 2065 7874 7261 5f6b 7761 7267  ray, extra_kwarg
+00000450: 733a 204f 7074 696f 6e61 6c5b 4469 6374  s: Optional[Dict
+00000460: 5d20 3d20 4e6f 6e65 293a 0a20 2020 2020  ] = None):.     
+00000470: 2020 2072 6574 7572 6e20 4d65 6d6f 7279     return Memory
+00000480: 436f 6e6e 6563 7469 6f6e 280a 2020 2020  Connection(.    
+00000490: 2020 2020 2020 2020 6461 7461 3d64 6174          data=dat
+000004a0: 612c 0a20 2020 2020 2020 2020 2020 2065  a,.            e
+000004b0: 7874 7261 5f6b 7761 7267 733d 6578 7472  xtra_kwargs=extr
+000004c0: 615f 6b77 6172 6773 2c0a 2020 2020 2020  a_kwargs,.      
+000004d0: 2020 290a 0a0a 636c 6173 7320 5065 6e64    )...class Pend
+000004e0: 696e 674d 656d 4171 2850 656e 6469 6e67  ingMemAq(Pending
+000004f0: 4163 7175 6973 6974 696f 6e29 3a0a 2020  Acquisition):.  
+00000500: 2020 7061 7373 0a0a 0a63 6c61 7373 204d    pass...class M
+00000510: 656d 6f72 7941 6371 7569 7369 7469 6f6e  emoryAcquisition
+00000520: 2841 6371 7569 7369 7469 6f6e 4d69 7869  (AcquisitionMixi
+00000530: 6e2c 204d 656d 6f72 7944 6174 6153 6574  n, MemoryDataSet
+00000540: 293a 0a20 2020 2027 2727 0a20 2020 2041  ):.    '''.    A
+00000550: 6e20 6163 7175 6973 6974 696f 6e20 6261  n acquisition ba
+00000560: 7365 6420 6f6e 206d 656d 6f72 790a 0a20  sed on memory.. 
+00000570: 2020 2043 7572 7265 6e74 6c79 2069 7420     Currently it 
+00000580: 6a75 7374 2073 706c 6963 6573 2074 6865  just splices the
+00000590: 2061 6464 6974 696f 6e61 6c20 6675 6e63   additional func
+000005a0: 7469 6f6e 616c 6974 7920 6672 6f6d 0a20  tionality from. 
+000005b0: 2020 203a 636c 6173 733a 607e 6c69 6265     :class:`~libe
+000005c0: 7274 656d 5f6c 6976 652e 6465 7465 6374  rtem_live.detect
+000005d0: 6f72 732e 6261 7365 2e64 6174 6173 6574  ors.base.dataset
+000005e0: 2e41 6371 7569 7369 7469 6f6e 4d69 7869  .AcquisitionMixi
+000005f0: 6e60 2069 6e74 6f20 7468 650a 2020 2020  n` into the.    
+00000600: 3a63 6c61 7373 3a60 7e6c 6962 6572 7465  :class:`~liberte
+00000610: 6d2e 696f 2e64 6174 6173 6574 2e6d 656d  m.io.dataset.mem
+00000620: 6f72 792e 4d65 6d6f 7279 4461 7461 5365  ory.MemoryDataSe
+00000630: 7460 2075 7369 6e67 206d 756c 7469 706c  t` using multipl
+00000640: 650a 2020 2020 696e 6865 7269 7461 6e63  e.    inheritanc
+00000650: 6520 616e 6420 696d 706c 656d 656e 7473  e and implements
+00000660: 2061 2064 756d 6d79 2066 6f72 2074 6865   a dummy for the
+00000670: 203a 6d65 7468 3a60 6163 7175 6972 6560   :meth:`acquire`
+00000680: 2063 6f6e 7465 7874 206d 616e 6167 6572   context manager
+00000690: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
+000006a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a0a 2020      --------..  
+000006b0: 2020 3e3e 3e20 696d 706f 7274 206e 756d    >>> import num
+000006c0: 7079 2061 7320 6e70 0a20 2020 203e 3e3e  py as np.    >>>
+000006d0: 2066 726f 6d20 6c69 6265 7274 656d 5f6c   from libertem_l
+000006e0: 6976 652e 6170 6920 696d 706f 7274 2048  ive.api import H
+000006f0: 6f6f 6b73 0a20 2020 202e 2e2e 0a20 2020  ooks.    ....   
+00000700: 203e 3e3e 2064 6174 6120 3d20 6e70 2e72   >>> data = np.r
+00000710: 616e 646f 6d2e 7261 6e64 6f6d 2828 3233  andom.random((23
+00000720: 2c20 3432 2c20 3531 2c20 3637 2929 0a20  , 42, 51, 67)). 
+00000730: 2020 202e 2e2e 0a20 2020 203e 3e3e 2063     ....    >>> c
+00000740: 6c61 7373 204d 7948 6f6f 6b73 2848 6f6f  lass MyHooks(Hoo
+00000750: 6b73 293a 0a20 2020 202e 2e2e 2020 2020  ks):.    ...    
+00000760: 2064 6566 206f 6e5f 7265 6164 795f 666f   def on_ready_fo
+00000770: 725f 6461 7461 2873 656c 662c 2065 6e76  r_data(self, env
+00000780: 293a 0a20 2020 202e 2e2e 2020 2020 2020  ):.    ...      
+00000790: 2020 2070 7269 6e74 2866 2254 7269 6767     print(f"Trigg
+000007a0: 6572 696e 6721 207b 656e 762e 6171 2e73  ering! {env.aq.s
+000007b0: 6861 7065 2e6e 6176 7d22 290a 2020 2020  hape.nav}").    
+000007c0: 2e2e 2e0a 2020 2020 3e3e 3e20 636f 6e6e  ....    >>> conn
+000007d0: 203d 2063 7478 2e6d 616b 655f 636f 6e6e   = ctx.make_conn
+000007e0: 6563 7469 6f6e 2827 6d65 6d6f 7279 2729  ection('memory')
+000007f0: 2e6f 7065 6e28 0a20 2020 202e 2e2e 2020  .open(.    ...  
+00000800: 2020 6461 7461 3d64 6174 610a 2020 2020    data=data.    
+00000810: 2e2e 2e20 290a 2020 2020 2e2e 2e0a 2020  ... ).    ....  
+00000820: 2020 3e3e 3e20 6171 203d 2063 7478 2e6d    >>> aq = ctx.m
+00000830: 616b 655f 6163 7175 6973 6974 696f 6e28  ake_acquisition(
+00000840: 0a20 2020 202e 2e2e 2020 2020 2063 6f6e  .    ...     con
+00000850: 6e3d 636f 6e6e 2c0a 2020 2020 2e2e 2e20  n=conn,.    ... 
+00000860: 2020 2020 686f 6f6b 733d 4d79 486f 6f6b      hooks=MyHook
+00000870: 7328 292c 0a20 2020 202e 2e2e 2029 0a20  s(),.    ... ). 
+00000880: 2020 202e 2e2e 0a20 2020 203e 3e3e 2075     ....    >>> u
+00000890: 6466 203d 2053 756d 5544 4628 290a 2020  df = SumUDF().  
+000008a0: 2020 3e3e 3e20 6374 782e 7275 6e5f 7564    >>> ctx.run_ud
+000008b0: 6628 6461 7461 7365 743d 6171 2c20 7564  f(dataset=aq, ud
+000008c0: 663d 7564 662c 2070 6c6f 7473 3d54 7275  f=udf, plots=Tru
+000008d0: 6529 0a20 2020 2054 7269 6767 6572 696e  e).    Triggerin
+000008e0: 6721 2028 3233 2c20 3432 290a 2020 2020  g! (23, 42).    
+000008f0: 7b27 696e 7465 6e73 6974 7927 3a20 3c42  {'intensity': <B
+00000900: 7566 6665 7257 7261 7070 6572 206b 696e  ufferWrapper kin
+00000910: 643d 7369 6720 6474 7970 653d 666c 6f61  d=sig dtype=floa
+00000920: 7436 3420 6578 7472 615f 7368 6170 653d  t64 extra_shape=
+00000930: 2829 3e7d 0a20 2020 2027 2727 0a0a 2020  ()>}.    '''..  
+00000940: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00000950: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00000960: 2020 2020 2020 636f 6e6e 3a20 224d 656d        conn: "Mem
+00000970: 6f72 7943 6f6e 6e65 6374 696f 6e22 2c0a  oryConnection",.
+00000980: 2020 2020 2020 2020 6e61 765f 7368 6170          nav_shap
+00000990: 653a 2054 7570 6c65 5b69 6e74 2c20 2e2e  e: Tuple[int, ..
+000009a0: 2e5d 2c0a 2020 2020 2020 2020 6672 616d  .],.        fram
+000009b0: 6573 5f70 6572 5f70 6172 7469 7469 6f6e  es_per_partition
+000009c0: 3a20 696e 7420 3d20 3132 382c 0a20 2020  : int = 128,.   
+000009d0: 2020 2020 2023 2069 6e20 7061 7373 6976       # in passiv
+000009e0: 6520 6d6f 6465 2c20 7765 2067 6574 2074  e mode, we get t
+000009f0: 6869 733a 0a20 2020 2020 2020 2070 656e  his:.        pen
+00000a00: 6469 6e67 5f61 713a 204f 7074 696f 6e61  ding_aq: Optiona
+00000a10: 6c5b 5065 6e64 696e 674d 656d 4171 5d20  l[PendingMemAq] 
+00000a20: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00000a30: 2320 636f 6e74 726f 6c6c 6572 2069 7320  # controller is 
+00000a40: 756e 7573 6564 2061 7320 6f66 206e 6f77  unused as of now
+00000a50: 2c20 796f 7520 6361 6e20 6f6e 6c79 2070  , you can only p
+00000a60: 6173 7320 696e 2060 4e6f 6e65 603a 0a20  ass in `None`:. 
+00000a70: 2020 2020 2020 2063 6f6e 7472 6f6c 6c65         controlle
+00000a80: 723a 204f 7074 696f 6e61 6c5b 4e6f 6e65  r: Optional[None
+00000a90: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00000aa0: 2020 686f 6f6b 733a 204f 7074 696f 6e61    hooks: Optiona
+00000ab0: 6c5b 486f 6f6b 735d 203d 204e 6f6e 652c  l[Hooks] = None,
+00000ac0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00000ad0: 2320 5858 5820 636f 7079 2f70 6173 7461  # XXX copy/pasta
+00000ae0: 2066 726f 6d20 4163 7175 6973 6974 696f   from Acquisitio
+00000af0: 6e4d 6978 696e 2061 7320 7765 2064 6f20  nMixin as we do 
+00000b00: 6e65 6564 2074 6f0a 2020 2020 2020 2020  need to.        
+00000b10: 2320 7061 7373 2065 7874 7261 206b 7761  # pass extra kwa
+00000b20: 7267 7320 746f 2074 6865 206d 656d 6f72  rgs to the memor
+00000b30: 7920 6461 7461 2073 6574 2075 6e64 6572  y data set under
+00000b40: 6e65 6174 683a 0a20 2020 2020 2020 2073  neath:.        s
+00000b50: 656c 662e 5f63 6f6e 6e20 3d20 636f 6e6e  elf._conn = conn
+00000b60: 0a20 2020 2020 2020 2073 656c 662e 5f6e  .        self._n
+00000b70: 6176 5f73 6861 7065 203d 206e 6176 5f73  av_shape = nav_s
+00000b80: 6861 7065 0a20 2020 2020 2020 2073 656c  hape.        sel
+00000b90: 662e 5f66 7261 6d65 735f 7065 725f 7061  f._frames_per_pa
+00000ba0: 7274 6974 696f 6e20 3d20 6672 616d 6573  rtition = frames
+00000bb0: 5f70 6572 5f70 6172 7469 7469 6f6e 2020  _per_partition  
+00000bc0: 2320 4649 584d 453a 2069 676e 6f72 6564  # FIXME: ignored
+00000bd0: 210a 2020 2020 2020 2020 7365 6c66 2e5f  !.        self._
+00000be0: 636f 6e74 726f 6c6c 6572 203d 2063 6f6e  controller = con
+00000bf0: 7472 6f6c 6c65 720a 2020 2020 2020 2020  troller.        
+00000c00: 7365 6c66 2e5f 7065 6e64 696e 675f 6171  self._pending_aq
+00000c10: 203d 2070 656e 6469 6e67 5f61 710a 2020   = pending_aq.  
+00000c20: 2020 2020 2020 6966 2068 6f6f 6b73 2069        if hooks i
+00000c30: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00000c40: 2020 2020 686f 6f6b 7320 3d20 486f 6f6b      hooks = Hook
+00000c50: 7328 290a 2020 2020 2020 2020 7365 6c66  s().        self
+00000c60: 2e5f 686f 6f6b 7320 3d20 686f 6f6b 730a  ._hooks = hooks.
+00000c70: 0a20 2020 2020 2020 204d 656d 6f72 7944  .        MemoryD
+00000c80: 6174 6153 6574 2e5f 5f69 6e69 745f 5f28  ataSet.__init__(
+00000c90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00000ca0: 662c 0a20 2020 2020 2020 2020 2020 2064  f,.            d
+00000cb0: 6174 613d 636f 6e6e 2e5f 6461 7461 2c0a  ata=conn._data,.
+00000cc0: 2020 2020 2020 2020 2020 2020 6e61 765f              nav_
+00000cd0: 7368 6170 653d 6e61 765f 7368 6170 652c  shape=nav_shape,
+00000ce0: 0a20 2020 2020 2020 2020 2020 202a 2a63  .            **c
+00000cf0: 6f6e 6e2e 5f65 7874 7261 5f6b 7761 7267  onn._extra_kwarg
+00000d00: 732c 0a20 2020 2020 2020 2029 0a0a 2020  s,.        )..  
+00000d10: 2020 4063 6f6e 7465 7874 6d61 6e61 6765    @contextmanage
+00000d20: 720a 2020 2020 6465 6620 6163 7175 6972  r.    def acquir
+00000d30: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00000d40: 2069 6620 7365 6c66 2e5f 7065 6e64 696e   if self._pendin
+00000d50: 675f 6171 2069 7320 4e6f 6e65 3a0a 2020  g_aq is None:.  
+00000d60: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00000d70: 686f 6f6b 732e 6f6e 5f72 6561 6479 5f66  hooks.on_ready_f
+00000d80: 6f72 5f64 6174 6128 0a20 2020 2020 2020  or_data(.       
+00000d90: 2020 2020 2020 2020 2052 6561 6479 466f           ReadyFo
+00000da0: 7244 6174 6145 6e76 2861 713d 7365 6c66  rDataEnv(aq=self
+00000db0: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
+00000dc0: 0a20 2020 2020 2020 2079 6965 6c64 0a    .        yield.
```

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/base/acquisition.py` & `libertem-live-0.2.1/src/libertem_live/detectors/base/acquisition.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/base/connection.py` & `libertem-live-0.2.1/src/libertem_live/detectors/base/connection.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/common.py` & `libertem-live-0.2.1/src/libertem_live/detectors/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                 except BrokenPipeError:
                     if "client_addr" in locals():
                         logger.info(f"BrokenPipeError: {locals()['client_addr']}")
                     else:
                         logger.info("BrokenPipeError")
 
                     continue  # the other end died, but that doesn't mean we have to die
-                except ConnectionResetError:
+                except (ConnectionResetError, ConnectionAbortedError):
                     if "client_addr" in locals():
                         logger.info(f"{self._name}: client {locals()['client_addr']} disconnected")
                     else:
                         logger.info(f"{self._name}: client disconnected")
                 # except BrokenPipeError:
                 #     # catch broken pipe error - allow the server to continue
                 #     # running, even when a client prematurely disconnects
```

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/dectris/DEigerClient.py` & `libertem-live-0.2.1/src/libertem_live/detectors/dectris/DEigerClient.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/dectris/acquisition.py` & `libertem-live-0.2.1/src/libertem_live/detectors/dectris/acquisition.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/dectris/common.py` & `libertem-live-0.2.1/src/libertem_live/detectors/dectris/common.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/dectris/connection.py` & `libertem-live-0.2.1/src/libertem_live/detectors/dectris/connection.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/dectris/controller.py` & `libertem-live-0.2.1/src/libertem_live/detectors/dectris/controller.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/dectris/sim.py` & `libertem-live-0.2.1/src/libertem_live/detectors/dectris/sim.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,14 +95,21 @@
         if data_filter is None:
             def data_filter(data):
                 return data
         self._data_filter = data_filter
         self._verbose = verbose
         self._tolerate_timeouts = tolerate_timeouts
 
+    def read_headers(self):
+        """
+        Get header with type 'dheader-1.0'. Can be called from outside of this
+        thread.
+        """
+        return read_headers(self._path)
+
     @property
     def port(self):
         return self._port
 
     def wait_for_listen(self, timeout=10):
         """
         To be called from the main thread
@@ -250,31 +257,60 @@
 
 class RustedReplay(ZMQReplay):
     def __init__(
         self,
         *args,
         dwelltime: Optional[int] = None,
         tolerate_timeouts=True,
+        num_mock_frames: Optional[int] = None,
         **kwargs
     ):
         super().__init__(*args, **kwargs)
         self.dwelltime = dwelltime
         self._tolerate_timeouts = tolerate_timeouts
+        self._num_mock_frames = num_mock_frames
+        if self._path is None and self._num_mock_frames is None:
+            raise ValueError("Need either `path` or `num_mock_frames`")
+        if self._path is not None and self._num_mock_frames is not None:
+            raise ValueError("Either `path` or `num_mock_frames` must be None")
 
-    def run(self):
-        try:
-            import libertem_dectris
-            set_thread_name("RustedReplay")
+    def read_headers(self):
+        """
+        Get header with type 'dheader-1.0'. Can be called from outside of this
+        thread.
+        """
+        return [
+            json.loads(self.sim.get_dheader_raw()),
+            json.loads(self.sim.get_detector_config_raw()),
+        ]
+
+    @property
+    def sim(self):
+        import libertem_dectris
+        if self._path is None and self._num_mock_frames is not None:
+            _sim = libertem_dectris.DectrisSim.new_mocked(
+                uri=self._uri,
+                num_frames=self._num_mock_frames,
+                dwelltime=self.dwelltime,
+                random_port=self._random_port,
+            )
+        else:
             _sim = libertem_dectris.DectrisSim(
                 uri=self._uri,
                 filename=self._path,
                 dwelltime=self.dwelltime,
                 random_port=self._random_port,
             )
+        return _sim
 
+    def run(self):
+        try:
+            import libertem_dectris
+            set_thread_name("RustedReplay")
+            _sim = self.sim
             real_uri = _sim.get_uri()
             self._port = urllib.parse.urlparse(real_uri).port
             if self._verbose:
                 logger.info(f"RustedReplay listening on {real_uri}")
 
             self.listen_event.set()
             while True:
@@ -581,75 +617,81 @@
     listen_event.set()
     return server.serve_forever()
 
 
 class DectrisSim:
     def __init__(
         self,
-        path: str,
+        *,
         port: int,
         zmqport: int,
+        path: Optional[str] = None,
+        num_mock_frames: Optional[int] = None,
         dwelltime: Optional[int] = None,
         data_filter=None,
         tolerate_timeouts: bool = True,
         verbose: bool = True,
     ) -> None:
         """
         Parameters
         ----------
         path
             _description_
+        num_mock_frames:
+            If path is not given, send this number of mocked frames
         port
             HTTP REST API port
         zmqport
             ZeroMQ port we should bind to
         dwelltime : int
             Take at least this much time for sending each frame, in microseconds
         verbose
             Print progress messages to stdout
         tolerate_timeouts
             If True, raise on timeouts instead of resetting simulator
         """
-        headers = read_headers(path)
-
         arm_event = multiprocessing.Event()
         trigger_event = multiprocessing.Event()
         self.stop_event = multiprocessing.Event()
         self.api_listen_event = multiprocessing.Event()
         self.api_port = multiprocessing.Value('l', -1)
         self.dwelltime = dwelltime
         self.verbose = verbose
+        self._num_mock_frames = num_mock_frames
 
         if data_filter is None:
             self.zmq_replay = RustedReplay(
                 uri=f"tcp://127.0.0.1:{zmqport}" if zmqport else "tcp://127.0.0.1",
                 random_port=not bool(zmqport),
                 path=path,
                 name='zmq_replay',
                 arm_event=arm_event,
                 trigger_event=trigger_event,
                 stop_event=self.stop_event,
                 data_filter=data_filter,
                 dwelltime=dwelltime,
                 tolerate_timeouts=tolerate_timeouts,
                 verbose=verbose,
+                num_mock_frames=num_mock_frames,
             )
         else:
+            assert path is not None
             self.zmq_replay = ZMQReplay(
                 uri=f"tcp://127.0.0.1:{zmqport}" if zmqport else "tcp://127.0.0.1",
                 random_port=not bool(zmqport),
                 path=path,
                 name='zmq_replay',
                 arm_event=arm_event,
                 trigger_event=trigger_event,
                 stop_event=self.stop_event,
                 data_filter=data_filter,
                 tolerate_timeouts=tolerate_timeouts,
                 verbose=verbose,
             )
+        headers = self.zmq_replay.read_headers()
 
         self.zmq_replay.daemon = True
 
         self.api_server = multiprocessing.Process(
             target=run_api,
             kwargs={
                 'port': port,
```

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/connection.cpython-39.pyc` & `libertem-live-0.2.1/src/libertem_live/detectors/merlin/connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,610 +1,541 @@
-00000000: 610d 0d0a 0000 0000 87dc 3f64 c721 0000  a.........?d.!..
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
-00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
-00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
-00000070: 6d0c 5a0c 0100 6406 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000080: 0100 6406 6408 6c0f 6d10 5a10 6d11 5a11  ..d.d.l.m.Z.m.Z.
-00000090: 6d12 5a12 6d13 5a13 0100 6400 6409 6c14  m.Z.m.Z...d.d.l.
-000000a0: 6d15 5a15 0100 6515 a016 6517 a101 5a18  m.Z...e...e...Z.
-000000b0: 6500 a019 6517 a101 5a1a 4700 640a 640b  e...e...Z.G.d.d.
-000000c0: 8400 640b 650a 8303 5a1b 4700 640c 640d  ..d.e...Z.G.d.d.
-000000d0: 8400 640d 6509 8303 5a1c 4700 640e 640f  ..d.e...Z.G.d.d.
-000000e0: 8400 640f 8302 5a1d 6401 5300 2910 e900  ..d...Z.d.S.)...
-000000f0: 0000 004e 2904 da08 4f70 7469 6f6e 616c  ...N)...Optional
-00000100: da04 5479 7065 da09 4765 6e65 7261 746f  ..Type..Generato
-00000110: 72da 0554 7570 6c65 2901 da0e 636f 6e74  r..Tuple)...cont
-00000120: 6578 746d 616e 6167 6572 2902 da12 4465  extmanager)...De
-00000130: 7465 6374 6f72 436f 6e6e 6563 7469 6f6e  tectorConnection
-00000140: da12 5065 6e64 696e 6741 6371 7569 7369  ..PendingAcquisi
-00000150: 7469 6f6e 2901 da13 4163 7175 6973 6974  tion)...Acquisit
-00000160: 696f 6e50 726f 746f 636f 6ce9 0100 0000  ionProtocol.....
-00000170: 2901 da0d 4d65 726c 696e 436f 6e74 726f  )...MerlinContro
-00000180: 6c29 04da 0f4d 6572 6c69 6e52 6177 536f  l)...MerlinRawSo
-00000190: 636b 6574 da11 4d65 726c 696e 4672 616d  cket..MerlinFram
-000001a0: 6553 7472 6561 6dda 1141 6371 7569 7369  eStream..Acquisi
-000001b0: 7469 6f6e 4865 6164 6572 da12 4163 7175  tionHeader..Acqu
-000001c0: 6973 6974 696f 6e54 696d 656f 7574 2901  isitionTimeout).
-000001d0: da05 7472 6163 6563 0000 0000 0000 0000  ..tracec........
-000001e0: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-000001f0: 7338 0000 0065 005a 0164 005a 0265 0364  s8...e.Z.d.Z.e.d
-00000200: 019c 0164 0264 0384 045a 0465 0564 0464  ...d.d...Z.e.d.d
-00000210: 0584 0083 015a 0665 0565 0764 069c 0164  .....Z.e.e.d...d
-00000220: 0764 0884 0483 015a 0864 0953 0029 0ada  .d.....Z.d.S.)..
-00000230: 184d 6572 6c69 6e50 656e 6469 6e67 4163  .MerlinPendingAc
-00000240: 7175 6973 6974 696f 6ea9 01da 0668 6561  quisition....hea
-00000250: 6465 7263 0200 0000 0000 0000 0000 0000  derc............
-00000260: 0200 0000 0200 0000 4300 0000 730a 0000  ........C...s...
-00000270: 007c 017c 005f 0064 0053 00a9 014e a901  .|.|._.d.S...N..
-00000280: da07 5f68 6561 6465 7229 02da 0473 656c  .._header)...sel
-00000290: 6672 1300 0000 a900 7218 0000 00fa 452f  fr......r.....E/
-000002a0: 617a 702f 6167 656e 742f 5f77 6f72 6b2f  azp/agent/_work/
-000002b0: 312f 732f 7372 632f 6c69 6265 7274 656d  1/s/src/libertem
-000002c0: 5f6c 6976 652f 6465 7465 6374 6f72 732f  _live/detectors/
-000002d0: 6d65 726c 696e 2f63 6f6e 6e65 6374 696f  merlin/connectio
-000002e0: 6e2e 7079 da08 5f5f 696e 6974 5f5f 1400  n.py..__init__..
-000002f0: 0000 7302 0000 0000 017a 214d 6572 6c69  ..s......z!Merli
-00000300: 6e50 656e 6469 6e67 4163 7175 6973 6974  nPendingAcquisit
-00000310: 696f 6e2e 5f5f 696e 6974 5f5f 6301 0000  ion.__init__c...
-00000320: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00000330: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
-00000340: 7214 0000 0072 1500 0000 a901 7217 0000  r....r......r...
-00000350: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000360: 7213 0000 0017 0000 0073 0200 0000 0002  r........s......
-00000370: 7a1f 4d65 726c 696e 5065 6e64 696e 6741  z.MerlinPendingA
-00000380: 6371 7569 7369 7469 6f6e 2e68 6561 6465  cquisition.heade
-00000390: 72a9 01da 0672 6574 7572 6e63 0100 0000  r....returnc....
-000003a0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-000003b0: 4300 0000 7308 0000 007c 006a 006a 0153  C...s....|.j.j.S
-000003c0: 0072 1400 0000 2902 7213 0000 00da 1566  .r....).r......f
-000003d0: 7261 6d65 735f 696e 5f61 6371 7569 7369  rames_in_acquisi
-000003e0: 7469 6f6e 721b 0000 0072 1800 0000 7218  tionr....r....r.
-000003f0: 0000 0072 1900 0000 da07 6e69 6d61 6765  ...r......nimage
-00000400: 731b 0000 0073 0200 0000 0002 7a20 4d65  s....s......z Me
-00000410: 726c 696e 5065 6e64 696e 6741 6371 7569  rlinPendingAcqui
-00000420: 7369 7469 6f6e 2e6e 696d 6167 6573 4e29  sition.nimagesN)
-00000430: 09da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000440: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000450: 616d 655f 5f72 0e00 0000 721a 0000 00da  ame__r....r.....
-00000460: 0870 726f 7065 7274 7972 1300 0000 da03  .propertyr......
-00000470: 696e 7472 1f00 0000 7218 0000 0072 1800  intr....r....r..
-00000480: 0000 7218 0000 0072 1900 0000 7211 0000  ..r....r....r...
-00000490: 0013 0000 0073 0a00 0000 0801 0e03 0201  .....s..........
-000004a0: 0a03 0201 7211 0000 0063 0000 0000 0000  ....r....c......
-000004b0: 0000 0000 0000 0000 0000 0700 0000 4000  ..............@.
-000004c0: 0000 73f4 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-000004d0: 015a 0364 0264 0364 0264 0464 0564 069c  .Z.d.d.d.d.d.d..
-000004e0: 0565 0465 0565 0465 0565 0664 069c 0564  .e.e.e.e.e.d...d
-000004f0: 0764 0884 065a 0764 0964 0a84 005a 0864  .d...Z.d.d...Z.d
-00000500: 2665 0965 0a19 0065 0965 0b19 0064 0c9c  &e.e...e.e...d..
-00000510: 0264 0d64 0e84 055a 0c65 0d65 0e65 0f66  .d.d...Z.e.e.e.f
-00000520: 0219 0064 0f9c 0164 1064 1184 045a 1065  ...d...d.d...Z.e
-00000530: 1165 1219 0064 0f9c 0164 1264 1384 045a  .e...d...d.d...Z
-00000540: 1364 1464 1584 005a 1464 1664 1784 005a  .d.d...Z.d.d...Z
-00000550: 1564 2765 0a64 199c 0164 1a64 1b84 055a  .d'e.d...d.d...Z
-00000560: 1665 1764 0f9c 0164 1c64 1d84 045a 1865  .e.d...d.d...Z.e
-00000570: 1965 1a65 1b64 0b64 0b66 0319 0064 0f9c  .e.e.d.d.f...d..
-00000580: 0164 1e64 1f84 0483 015a 1c65 0d65 0565  .d.d.....Z.e.e.e
-00000590: 0566 0219 0064 0f9c 0164 2064 2184 045a  .f...d...d d!..Z
-000005a0: 1d65 0564 0f9c 0164 2264 2384 045a 1e64  .e.d...d"d#..Z.d
-000005b0: 2464 2584 005a 1f64 0b53 0029 28da 184d  $d%..Z.d.S.)(..M
-000005c0: 6572 6c69 6e44 6574 6563 746f 7243 6f6e  erlinDetectorCon
-000005d0: 6e65 6374 696f 6e61 8905 0000 0a20 2020  nectiona.....   
-000005e0: 2054 6869 7320 636c 6173 7320 686f 6c64   This class hold
-000005f0: 7320 6120 7065 726d 616e 656e 7420 6461  s a permanent da
-00000600: 7461 2063 6f6e 6e65 6374 696f 6e20 746f  ta connection to
-00000610: 2074 6865 206d 6572 6c69 6e20 736f 6674   the merlin soft
-00000620: 7761 7265 2e0a 0a20 2020 2043 6f6e 7472  ware...    Contr
-00000630: 6f6c 2063 6f6e 6e65 6374 696f 6e73 2061  ol connections a
-00000640: 7265 2061 6c73 6f20 706f 7373 6962 6c65  re also possible
-00000650: 2074 6f20 6f62 7461 696e 2066 726f 6d20   to obtain from 
-00000660: 7468 6973 2063 6c61 7373 2c0a 2020 2020  this class,.    
-00000670: 6275 7420 6172 6520 6372 6561 7465 6420  but are created 
-00000680: 6f6e 2064 656d 616e 6420 616e 6420 6e6f  on demand and no
-00000690: 7420 6b65 7074 206f 7065 6e2e 0a0a 2020  t kept open...  
-000006a0: 2020 596f 7520 6361 6e20 7573 6520 7468    You can use th
-000006b0: 6520 636f 6e76 656e 6965 6e63 6520 6675  e convenience fu
-000006c0: 6e63 7469 6f6e 0a20 2020 203a 6d65 7468  nction.    :meth
-000006d0: 3a60 6c69 6265 7274 656d 5f6c 6976 652e  :`libertem_live.
-000006e0: 6170 692e 4c69 7665 436f 6e74 6578 742e  api.LiveContext.
-000006f0: 6d61 6b65 5f63 6f6e 6e65 6374 696f 6e60  make_connection`
-00000700: 2074 6f20 6372 6561 7465 2061 6e20 696e   to create an in
-00000710: 7374 616e 6365 2c0a 2020 2020 696e 7374  stance,.    inst
-00000720: 6561 6420 6f66 2063 616c 6c69 6e67 2074  ead of calling t
-00000730: 6869 7320 636f 6e73 7472 7563 746f 7220  his constructor 
-00000740: 6469 7265 6374 6c79 2e0a 0a20 2020 2050  directly...    P
-00000750: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00000760: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2061 7069  --------.    api
-00000770: 5f68 6f73 740a 2020 2020 2020 2020 486f  _host.        Ho
-00000780: 7374 6e61 6d65 206f 6620 7468 6520 4d65  stname of the Me
-00000790: 726c 696e 2063 6f6e 7472 6f6c 2073 6572  rlin control ser
-000007a0: 7665 722c 2064 6566 6175 6c74 2027 3132  ver, default '12
-000007b0: 372e 302e 302e 3127 0a20 2020 2020 2020  7.0.0.1'.       
-000007c0: 2053 686f 756c 6420 696e 206d 6f73 7420   Should in most 
-000007d0: 6361 7365 7320 6265 2074 6865 2073 616d  cases be the sam
-000007e0: 6520 6173 2060 6461 7461 5f68 6f73 7460  e as `data_host`
-000007f0: 2e0a 2020 2020 6170 695f 706f 7274 0a20  ..    api_port. 
-00000800: 2020 2020 2020 2050 6f72 7420 6f66 2074         Port of t
-00000810: 6865 204d 6572 6c69 6e20 636f 6e74 726f  he Merlin contro
-00000820: 6c20 7365 7276 6572 2c20 6465 6661 756c  l server, defaul
-00000830: 7420 3633 3431 0a20 2020 2064 6174 615f  t 6341.    data_
-00000840: 686f 7374 0a20 2020 2020 2020 2048 6f73  host.        Hos
-00000850: 746e 616d 6520 6f66 2074 6865 204d 6572  tname of the Mer
-00000860: 6c69 6e20 6461 7461 2073 6572 7665 722c  lin data server,
-00000870: 2064 6566 6175 6c74 2027 3132 372e 302e   default '127.0.
-00000880: 302e 3127 0a20 2020 2064 6174 615f 706f  0.1'.    data_po
-00000890: 7274 0a20 2020 2020 2020 2044 6174 6120  rt.        Data 
-000008a0: 706f 7274 206f 6620 7468 6520 4d65 726c  port of the Merl
-000008b0: 696e 2064 6174 6120 7365 7276 6572 2c20  in data server, 
-000008c0: 6465 6661 756c 7420 3633 3432 0a20 2020  default 6342.   
-000008d0: 2064 7261 696e 0a20 2020 2020 2020 2044   drain.        D
-000008e0: 7261 696e 2074 6865 2073 6f63 6b65 7420  rain the socket 
-000008f0: 6265 666f 7265 2074 7269 6767 6572 696e  before triggerin
-00000900: 672e 2045 6e61 626c 6520 7468 6973 2077  g. Enable this w
-00000910: 6865 6e0a 2020 2020 2020 2020 7573 696e  hen.        usin
-00000920: 6720 6f6c 6420 7665 7273 696f 6e73 206f  g old versions o
-00000930: 6620 7468 6520 4d65 726c 696e 2073 6f66  f the Merlin sof
-00000940: 7477 6172 652c 2062 7574 206e 6f74 2077  tware, but not w
-00000950: 6865 6e0a 2020 2020 2020 2020 7573 696e  hen.        usin
-00000960: 6720 616e 2069 6e74 6572 6e61 6c20 7472  g an internal tr
-00000970: 6967 6765 722e 0a0a 2020 2020 4578 616d  igger...    Exam
-00000980: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
-00000990: 2d0a 2020 2020 5573 7561 6c6c 792c 2074  -.    Usually, t
-000009a0: 6869 7320 636c 6173 7320 6973 2069 6e73  his class is ins
-000009b0: 7461 6e74 6961 7465 6420 7573 696e 670a  tantiated using.
-000009c0: 2020 2020 3a6d 6574 683a 606c 6962 6572      :meth:`liber
-000009d0: 7465 6d5f 6c69 7665 2e61 7069 2e4c 6976  tem_live.api.Liv
-000009e0: 6543 6f6e 7465 7874 2e6d 616b 655f 636f  eContext.make_co
-000009f0: 6e6e 6563 7469 6f6e 603a 0a0a 2020 2020  nnection`:..    
-00000a00: 3e3e 3e20 7769 7468 2063 7478 2e6d 616b  >>> with ctx.mak
-00000a10: 655f 636f 6e6e 6563 7469 6f6e 2827 6d65  e_connection('me
-00000a20: 726c 696e 2729 2e6f 7065 6e28 0a20 2020  rlin').open(.   
-00000a30: 202e 2e2e 2020 2020 2061 7069 5f68 6f73   ...     api_hos
-00000a40: 743d 2731 3237 2e30 2e30 2e31 272c 0a20  t='127.0.0.1',. 
-00000a50: 2020 202e 2e2e 2020 2020 2061 7069 5f70     ...     api_p
-00000a60: 6f72 743d 4d45 524c 494e 5f41 5049 5f50  ort=MERLIN_API_P
-00000a70: 4f52 542c 0a20 2020 202e 2e2e 2020 2020  ORT,.    ...    
-00000a80: 2064 6174 615f 686f 7374 3d27 3132 372e   data_host='127.
-00000a90: 302e 302e 3127 2c0a 2020 2020 2e2e 2e20  0.0.1',.    ... 
-00000aa0: 2020 2020 6461 7461 5f70 6f72 743d 4d45      data_port=ME
-00000ab0: 524c 494e 5f44 4154 415f 504f 5254 2c0a  RLIN_DATA_PORT,.
-00000ac0: 2020 2020 2e2e 2e20 2920 6173 2063 6f6e      ... ) as con
-00000ad0: 6e3a 0a20 2020 202e 2e2e 2020 2020 2061  n:.    ...     a
-00000ae0: 7120 3d20 6374 782e 6d61 6b65 5f61 6371  q = ctx.make_acq
-00000af0: 7569 7369 7469 6f6e 2863 6f6e 6e3d 636f  uisition(conn=co
-00000b00: 6e6e 2c20 6e61 765f 7368 6170 653d 2833  nn, nav_shape=(3
-00000b10: 322c 2033 3229 290a 2020 2020 2e2e 2e20  2, 32)).    ... 
-00000b20: 2020 2020 6374 782e 7275 6e5f 7564 6628      ctx.run_udf(
-00000b30: 6461 7461 7365 743d 6171 2c20 7564 663d  dataset=aq, udf=
-00000b40: 5375 6d55 4446 2829 290a 2020 2020 7b27  SumUDF()).    {'
-00000b50: 696e 7465 6e73 6974 7927 3a20 2e2e 2e7d  intensity': ...}
-00000b60: 0a20 2020 20fa 0931 3237 2e30 2e30 2e31  .    ..127.0.0.1
-00000b70: e9c5 1800 00e9 c618 0000 46a9 05da 0861  ..........F....a
-00000b80: 7069 5f68 6f73 74da 0861 7069 5f70 6f72  pi_host..api_por
-00000b90: 74da 0964 6174 615f 686f 7374 da09 6461  t..data_host..da
-00000ba0: 7461 5f70 6f72 74da 0564 7261 696e 6301  ta_port..drainc.
-00000bb0: 0000 0000 0000 0005 0000 0006 0000 0002  ................
-00000bc0: 0000 0043 0000 0073 2a00 0000 7c01 7c00  ...C...s*...|.|.
-00000bd0: 5f00 7c02 7c00 5f01 7c03 7c00 5f02 7c04  _.|.|._.|.|._.|.
-00000be0: 7c00 5f03 7c05 7c00 5f04 7c00 a005 a100  |._.|.|._.|.....
-00000bf0: 0100 6400 5300 7214 0000 0029 06da 095f  ..d.S.r....)..._
-00000c00: 6170 695f 686f 7374 da09 5f61 7069 5f70  api_host.._api_p
-00000c10: 6f72 74da 0a5f 6461 7461 5f68 6f73 74da  ort.._data_host.
-00000c20: 0a5f 6461 7461 5f70 6f72 74da 065f 6472  ._data_port.._dr
-00000c30: 6169 6eda 085f 636f 6e6e 6563 74a9 0672  ain.._connect..r
-00000c40: 1700 0000 722a 0000 0072 2b00 0000 722c  ....r*...r+...r,
-00000c50: 0000 0072 2d00 0000 722e 0000 0072 1800  ...r-...r....r..
-00000c60: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000c70: 004b 0000 0073 0c00 0000 0009 0601 0601  .K...s..........
-00000c80: 0601 0601 0601 7a21 4d65 726c 696e 4465  ......z!MerlinDe
-00000c90: 7465 6374 6f72 436f 6e6e 6563 7469 6f6e  tectorConnection
-00000ca0: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00000cb0: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
-00000cc0: 0000 731c 0000 0074 007c 006a 017c 006a  ..s....t.|.j.|.j
-00000cd0: 0264 018d 02a0 03a1 007c 005f 047c 006a  .d.......|._.|.j
-00000ce0: 0453 00a9 024e 2902 da04 686f 7374 da04  .S...N)...host..
-00000cf0: 706f 7274 2905 720c 0000 0072 3100 0000  port).r....r1...
-00000d00: 7232 0000 00da 0763 6f6e 6e65 6374 da0c  r2.....connect..
-00000d10: 5f64 6174 615f 736f 636b 6574 721b 0000  _data_socketr...
-00000d20: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000d30: 7234 0000 005b 0000 0073 0a00 0000 0001  r4...[...s......
-00000d40: 0201 0401 04fe 0c04 7a21 4d65 726c 696e  ........z!Merlin
-00000d50: 4465 7465 6374 6f72 436f 6e6e 6563 7469  DetectorConnecti
-00000d60: 6f6e 2e5f 636f 6e6e 6563 744e 2902 da07  on._connectN)...
-00000d70: 7469 6d65 6f75 7472 1d00 0000 6302 0000  timeoutr....c...
-00000d80: 0000 0000 0000 0000 0003 0000 0008 0000  ................
-00000d90: 0043 0000 0073 5400 0000 7c00 6a00 6401  .C...sT...|.j.d.
-00000da0: 7500 7212 7c00 a001 a100 0100 7c00 6a00  u.r.|.......|.j.
-00000db0: 6401 7501 7320 4a00 8201 7a1a 7c00 6a00  d.u.s J...z.|.j.
-00000dc0: 6a02 7c01 6402 8d01 7d02 7403 7c02 6403  j.|.d...}.t.|.d.
-00000dd0: 8d01 5700 5300 0400 7404 794e 0100 0100  ..W.S...t.yN....
-00000de0: 0100 5900 6401 5300 3000 6401 5300 2904  ..Y.d.S.0.d.S.).
-00000df0: 610a 0500 000a 2020 2020 2020 2020 5761  a.....        Wa
-00000e00: 6974 2066 6f72 2061 7420 6d6f 7374 2060  it for at most `
-00000e10: 7469 6d65 6f75 7460 2073 6563 6f6e 6473  timeout` seconds
-00000e20: 2066 6f72 2061 6e20 6163 7175 6973 6974   for an acquisit
-00000e30: 696f 6e20 746f 2073 7461 7274 2e20 5468  ion to start. Th
-00000e40: 6973 0a20 2020 2020 2020 2064 6f65 7320  is.        does 
-00000e50: 6e6f 7420 7065 7266 6f72 6d20 616e 7920  not perform any 
-00000e60: 7472 6967 6765 7269 6e67 2069 7473 656c  triggering itsel
-00000e70: 6620 616e 6420 6578 7065 6374 7320 736f  f and expects so
-00000e80: 6d65 7468 696e 6720 6578 7465 726e 616c  mething external
-00000e90: 0a20 2020 2020 2020 2074 6f20 6172 6d20  .        to arm 
-00000ea0: 616e 6420 7472 6967 6765 7220 7468 6520  and trigger the 
-00000eb0: 6163 7175 6973 6974 696f 6e2e 0a0a 2020  acquisition...  
-00000ec0: 2020 2020 2020 4f6e 6365 2074 6865 2064        Once the d
-00000ed0: 6574 6563 746f 7220 6973 2061 726d 6564  etector is armed
-00000ee0: 2c20 7468 6973 2066 756e 6374 696f 6e20  , this function 
-00000ef0: 7265 7475 726e 7320 6120 6050 656e 6469  returns a `Pendi
-00000f00: 6e67 4163 7175 6973 6974 696f 6e60 2c0a  ngAcquisition`,.
-00000f10: 2020 2020 2020 2020 7768 6963 6820 6361          which ca
-00000f20: 6e20 6265 2063 6f6e 7665 7274 6564 2074  n be converted t
-00000f30: 6f20 6120 6675 6c6c 2060 4163 7175 6973  o a full `Acquis
-00000f40: 6974 696f 6e60 206f 626a 6563 7420 7573  ition` object us
-00000f50: 696e 670a 2020 2020 2020 2020 3a6d 6574  ing.        :met
-00000f60: 683a 606c 6962 6572 7465 6d5f 6c69 7665  h:`libertem_live
-00000f70: 2e61 7069 2e4c 6976 6543 6f6e 7465 7874  .api.LiveContext
-00000f80: 2e6d 616b 655f 6163 7175 6973 6974 696f  .make_acquisitio
-00000f90: 6e60 2e0a 0a20 2020 2020 2020 2054 6865  n`...        The
-00000fa0: 2066 756e 6374 696f 6e20 7265 7475 726e   function return
-00000fb0: 7320 604e 6f6e 6560 206f 6e20 7469 6d65  s `None` on time
-00000fc0: 6f75 742e 0a0a 2020 2020 2020 2020 5061  out...        Pa
-00000fd0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00000fe0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00000ff0: 2020 2020 7469 6d65 6f75 740a 2020 2020      timeout.    
-00001000: 2020 2020 2020 2020 5469 6d65 6f75 7420          Timeout 
-00001010: 696e 2073 6563 6f6e 6473 2e20 4966 2060  in seconds. If `
-00001020: 4e6f 6e65 602c 2077 6169 7420 696e 6465  None`, wait inde
-00001030: 6669 6e69 7465 6c79 2e0a 0a20 2020 2020  finitely...     
-00001040: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-00001050: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-00001060: 2020 2020 203e 3e3e 2077 6974 6820 6374       >>> with ct
-00001070: 782e 6d61 6b65 5f63 6f6e 6e65 6374 696f  x.make_connectio
-00001080: 6e28 276d 6572 6c69 6e27 292e 6f70 656e  n('merlin').open
-00001090: 280a 2020 2020 2020 2020 2e2e 2e20 2020  (.        ...   
-000010a0: 2020 6170 695f 686f 7374 3d27 3132 372e    api_host='127.
-000010b0: 302e 302e 3127 2c0a 2020 2020 2020 2020  0.0.1',.        
-000010c0: 2e2e 2e20 2020 2020 6170 695f 706f 7274  ...     api_port
-000010d0: 3d4d 4552 4c49 4e5f 4150 495f 504f 5254  =MERLIN_API_PORT
-000010e0: 2c0a 2020 2020 2020 2020 2e2e 2e20 2020  ,.        ...   
-000010f0: 2020 6461 7461 5f68 6f73 743d 2731 3237    data_host='127
-00001100: 2e30 2e30 2e31 272c 0a20 2020 2020 2020  .0.0.1',.       
-00001110: 202e 2e2e 2020 2020 2064 6174 615f 706f   ...     data_po
-00001120: 7274 3d4d 4552 4c49 4e5f 4441 5441 5f50  rt=MERLIN_DATA_P
-00001130: 4f52 542c 0a20 2020 2020 2020 202e 2e2e  ORT,.        ...
-00001140: 2029 2061 7320 636f 6e6e 3a0a 2020 2020   ) as conn:.    
-00001150: 2020 2020 2e2e 2e20 2020 2020 7065 6e64      ...     pend
-00001160: 696e 675f 6171 203d 2063 6f6e 6e2e 7761  ing_aq = conn.wa
-00001170: 6974 5f66 6f72 5f61 6371 7569 7369 7469  it_for_acquisiti
-00001180: 6f6e 2874 696d 656f 7574 3d31 290a 2020  on(timeout=1).  
-00001190: 2020 2020 2020 2e2e 2e20 2020 2020 2320        ...     # 
-000011a0: 6174 2074 6869 7320 706f 696e 742c 2073  at this point, s
-000011b0: 6f6d 6574 6869 6e67 2065 6c73 6520 6973  omething else is
-000011c0: 2061 726d 696e 6720 616e 6420 7472 6967   arming and trig
-000011d0: 6765 7269 6e67 2074 6865 0a20 2020 2020  gering the.     
-000011e0: 2020 202e 2e2e 2020 2020 2023 2064 6574     ...     # det
-000011f0: 6563 746f 723a 0a20 2020 2020 2020 202e  ector:.        .
-00001200: 2e2e 2020 2020 2061 7120 3d20 6374 782e  ..     aq = ctx.
-00001210: 6d61 6b65 5f61 6371 7569 7369 7469 6f6e  make_acquisition
-00001220: 280a 2020 2020 2020 2020 2e2e 2e20 2020  (.        ...   
-00001230: 2020 2020 2020 636f 6e6e 3d63 6f6e 6e2c        conn=conn,
-00001240: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
-00001250: 2020 2020 206e 6176 5f73 6861 7065 3d28       nav_shape=(
-00001260: 3332 2c20 3332 292c 0a20 2020 2020 2020  32, 32),.       
-00001270: 202e 2e2e 2020 2020 2020 2020 2070 656e   ...         pen
-00001280: 6469 6e67 5f61 713d 7065 6e64 696e 675f  ding_aq=pending_
-00001290: 6171 2c0a 2020 2020 2020 2020 2e2e 2e20  aq,.        ... 
-000012a0: 2020 2020 290a 2020 2020 2020 2020 2e2e      ).        ..
-000012b0: 2e20 2020 2020 6374 782e 7275 6e5f 7564  .     ctx.run_ud
-000012c0: 6628 6461 7461 7365 743d 6171 2c20 7564  f(dataset=aq, ud
-000012d0: 663d 5375 6d55 4446 2829 290a 2020 2020  f=SumUDF()).    
-000012e0: 2020 2020 7b27 696e 7465 6e73 6974 7927      {'intensity'
-000012f0: 3a20 2e2e 2e7d 0a20 2020 2020 2020 204e  : ...}.        N
-00001300: 2901 da0e 6361 6e63 656c 5f74 696d 656f  )...cancel_timeo
-00001310: 7574 7212 0000 0029 0572 3a00 0000 7234  utr....).r:...r4
-00001320: 0000 00da 1772 6561 645f 6163 7175 6973  .....read_acquis
-00001330: 6974 696f 6e5f 6865 6164 6572 7211 0000  ition_headerr...
-00001340: 0072 0f00 0000 2903 7217 0000 0072 3b00  .r....).r....r;.
-00001350: 0000 7213 0000 0072 1800 0000 7218 0000  ..r....r....r...
-00001360: 0072 1900 0000 da14 7761 6974 5f66 6f72  .r......wait_for
-00001370: 5f61 6371 7569 7369 7469 6f6e 6200 0000  _acquisitionb...
-00001380: 7310 0000 0000 240a 0108 010e 0102 010e  s.....$.........
-00001390: 010c 010c 017a 2d4d 6572 6c69 6e44 6574  .....z-MerlinDet
-000013a0: 6563 746f 7243 6f6e 6e65 6374 696f 6e2e  ectorConnection.
-000013b0: 7761 6974 5f66 6f72 5f61 6371 7569 7369  wait_for_acquisi
-000013c0: 7469 6f6e 721c 0000 0063 0100 0000 0000  tionr....c......
-000013d0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-000013e0: 0000 7330 0000 007c 006a 0064 0075 0173  ..s0...|.j.d.u.s
-000013f0: 0e4a 0082 017c 006a 00a0 01a1 007d 0174  .J...|.j.....}.t
-00001400: 026a 037c 006a 007c 0164 018d 027d 027c  .j.|.j.|.d...}.|
-00001410: 017c 0266 0253 0029 024e 2902 da0a 7261  .|.f.S.).N)...ra
-00001420: 775f 736f 636b 6574 da12 6163 7175 6973  w_socket..acquis
-00001430: 6974 696f 6e5f 6865 6164 6572 2904 723a  ition_header).r:
-00001440: 0000 0072 3d00 0000 720d 0000 00da 1166  ...r=...r......f
-00001450: 726f 6d5f 6672 616d 655f 6865 6164 6572  rom_frame_header
-00001460: 2903 7217 0000 00da 0a61 6371 5f68 6561  ).r......acq_hea
-00001470: 6465 72da 0673 7472 6561 6d72 1800 0000  der..streamr....
-00001480: 7218 0000 0072 1900 0000 da15 6765 745f  r....r......get_
-00001490: 6865 6164 6572 5f61 6e64 5f73 7472 6561  header_and_strea
-000014a0: 6d8f 0000 0073 0e00 0000 0001 0e01 0a01  m....s..........
-000014b0: 0401 0401 02fe 0604 7a2e 4d65 726c 696e  ........z.Merlin
-000014c0: 4465 7465 6374 6f72 436f 6e6e 6563 7469  DetectorConnecti
-000014d0: 6f6e 2e67 6574 5f68 6561 6465 725f 616e  on.get_header_an
-000014e0: 645f 7374 7265 616d 6301 0000 0000 0000  d_streamc.......
-000014f0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-00001500: 0073 1000 0000 6401 6402 6c00 6d01 7d01  .s....d.d.l.m.}.
-00001510: 0100 7c01 5300 2903 4e72 0a00 0000 2901  ..|.S.).Nr....).
-00001520: da11 4d65 726c 696e 4163 7175 6973 6974  ..MerlinAcquisit
-00001530: 696f 6e29 02da 0b61 6371 7569 7369 7469  ion)...acquisiti
-00001540: 6f6e 7245 0000 0029 0272 1700 0000 7245  onrE...).r....rE
-00001550: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00001560: 0000 da13 6765 745f 6163 7175 6973 6974  ....get_acquisit
-00001570: 696f 6e5f 636c 7398 0000 0073 0400 0000  ion_cls....s....
-00001580: 0001 0c01 7a2c 4d65 726c 696e 4465 7465  ....z,MerlinDete
-00001590: 6374 6f72 436f 6e6e 6563 7469 6f6e 2e67  ctorConnection.g
-000015a0: 6574 5f61 6371 7569 7369 7469 6f6e 5f63  et_acquisition_c
-000015b0: 6c73 6301 0000 0000 0000 0000 0000 0001  lsc.............
-000015c0: 0000 0002 0000 0043 0000 0073 1600 0000  .......C...s....
-000015d0: 7c00 6a00 6400 7500 7212 7c00 a001 a100  |.j.d.u.r.|.....
-000015e0: 0100 7c00 5300 7214 0000 0029 0272 3a00  ..|.S.r....).r:.
-000015f0: 0000 7234 0000 0072 1b00 0000 7218 0000  ..r4...r....r...
-00001600: 0072 1800 0000 7219 0000 00da 095f 5f65  .r....r......__e
-00001610: 6e74 6572 5f5f 9c00 0000 7306 0000 0000  nter__....s.....
-00001620: 010a 0108 017a 224d 6572 6c69 6e44 6574  .....z"MerlinDet
-00001630: 6563 746f 7243 6f6e 6e65 6374 696f 6e2e  ectorConnection.
-00001640: 5f5f 656e 7465 725f 5f63 0100 0000 0000  __enter__c......
-00001650: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00001660: 0000 731e 0000 007c 006a 0064 0075 0172  ..s....|.j.d.u.r
-00001670: 1a7c 006a 00a0 01a1 0001 0064 007c 005f  .|.j.......d.|._
-00001680: 0064 0053 0072 1400 0000 2902 723a 0000  .d.S.r....).r:..
-00001690: 00da 0563 6c6f 7365 721b 0000 0072 1800  ...closer....r..
-000016a0: 0000 7218 0000 0072 1900 0000 7249 0000  ..r....r....rI..
-000016b0: 00a1 0000 0073 0600 0000 0003 0a01 0a01  .....s..........
-000016c0: 7a1e 4d65 726c 696e 4465 7465 6374 6f72  z.MerlinDetector
-000016d0: 436f 6e6e 6563 7469 6f6e 2e63 6c6f 7365  Connection.close
-000016e0: e700 0000 0000 00f0 3f29 0172 3b00 0000  ........?).r;...
-000016f0: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-00001700: 0008 0000 0043 0000 0073 7400 0000 7c00  .....C...st...|.
-00001710: 6a00 6400 7501 730e 4a00 8201 7c00 6a01  j.d.u.s.J...|.j.
-00001720: 7270 7402 a003 6401 a101 8f28 7d02 7c00  rpt...d....(}.|.
-00001730: 6a00 a004 a100 7d03 7c02 a005 6402 7c03  j.....}.|...d.|.
-00001740: 6901 a101 0100 5700 6400 0400 0400 8303  i.....W.d.......
-00001750: 0100 6e10 3100 734c 3000 0100 0100 0100  ..n.1.sL0.......
-00001760: 5900 0100 7c03 6403 6b04 7270 7406 a007  Y...|.d.k.rpt...
-00001770: 6404 7c03 9b00 6405 9d03 a101 0100 6400  d.|...d.......d.
-00001780: 5300 2906 4e72 2e00 0000 7a1b 6c69 6265  S.).Nr....z.libe
-00001790: 7274 656d 5f6c 6976 652e 6472 6169 6e65  rtem_live.draine
-000017a0: 645f 6279 7465 7372 0100 0000 7a08 6472  d_bytesr....z.dr
-000017b0: 6169 6e65 6420 7a11 2062 7974 6573 206f  ained z. bytes o
-000017c0: 6620 6761 7262 6167 6529 0872 3a00 0000  f garbage).r:...
-000017d0: 7233 0000 00da 0674 7261 6365 72da 1573  r3.....tracer..s
-000017e0: 7461 7274 5f61 735f 6375 7272 656e 745f  tart_as_current_
-000017f0: 7370 616e 722e 0000 00da 0e73 6574 5f61  spanr......set_a
-00001800: 7474 7269 6275 7465 73da 066c 6f67 6765  ttributes..logge
-00001810: 72da 0469 6e66 6f29 0472 1700 0000 723b  r..info).r....r;
-00001820: 0000 00da 0473 7061 6e5a 0d64 7261 696e  .....spanZ.drain
-00001830: 6564 5f62 7974 6573 7218 0000 0072 1800  ed_bytesr....r..
-00001840: 0000 7219 0000 00da 0b6d 6179 6265 5f64  ..r......maybe_d
-00001850: 7261 696e a800 0000 7312 0000 0000 010e  rain....s.......
-00001860: 0106 010c 010a 0104 0104 ff24 0308 017a  ...........$...z
-00001870: 244d 6572 6c69 6e44 6574 6563 746f 7243  $MerlinDetectorC
-00001880: 6f6e 6e65 6374 696f 6e2e 6d61 7962 655f  onnection.maybe_
-00001890: 6472 6169 6e63 0100 0000 0000 0000 0000  drainc..........
-000018a0: 0000 0100 0000 0200 0000 4300 0000 7318  ..........C...s.
-000018b0: 0000 007c 006a 0064 0075 0173 124a 0064  ...|.j.d.u.s.J.d
-000018c0: 0183 0182 017c 006a 0053 0029 024e 7a21  .....|.j.S.).Nz!
-000018d0: 6e65 6564 2074 6f20 6265 2063 6f6e 6e65  need to be conne
-000018e0: 6374 6564 2074 6f20 6361 6c6c 2074 6869  cted to call thi
-000018f0: 7329 0172 3a00 0000 721b 0000 0072 1800  s).r:...r....r..
-00001900: 0000 7218 0000 0072 1900 0000 da0f 6765  ..r....r......ge
-00001910: 745f 6461 7461 5f73 6f63 6b65 74b3 0000  t_data_socket...
-00001920: 0073 0400 0000 0001 1201 7a28 4d65 726c  .s........z(Merl
-00001930: 696e 4465 7465 6374 6f72 436f 6e6e 6563  inDetectorConnec
-00001940: 7469 6f6e 2e67 6574 5f64 6174 615f 736f  tion.get_data_so
-00001950: 636b 6574 6301 0000 0000 0000 0000 0000  cketc...........
-00001960: 0002 0000 0008 0000 0063 0000 0073 3a00  .........c...s:.
-00001970: 0000 7400 7c00 6a01 7c00 6a02 6401 8d02  ..t.|.j.|.j.d...
-00001980: 8f16 7d01 7c01 5600 0100 5700 6400 0400  ..}.|.V...W.d...
-00001990: 0400 8303 0100 6e10 3100 732c 3000 0100  ......n.1.s,0...
-000019a0: 0100 0100 5900 0100 6400 5300 7236 0000  ....Y...d.S.r6..
-000019b0: 0029 0372 0b00 0000 722f 0000 0072 3000  .).r....r/...r0.
-000019c0: 0000 a902 7217 0000 00da 0163 7218 0000  ....r......cr...
-000019d0: 0072 1800 0000 7219 0000 00da 0763 6f6e  .r....r......con
-000019e0: 7472 6f6c b700 0000 7304 0000 0000 0212  trol....s.......
-000019f0: 017a 204d 6572 6c69 6e44 6574 6563 746f  .z MerlinDetecto
-00001a00: 7243 6f6e 6e65 6374 696f 6e2e 636f 6e74  rConnection.cont
-00001a10: 726f 6c63 0100 0000 0000 0000 0000 0000  rolc............
-00001a20: 0400 0000 0800 0000 4300 0000 7350 0000  ........C...sP..
-00001a30: 007c 00a0 00a1 008f 347d 0174 017c 01a0  .|......4}.t.|..
-00001a40: 0264 01a1 0183 017d 0274 017c 01a0 0264  .d.....}.t.|...d
-00001a50: 02a1 0183 017d 037c 037c 0266 0257 0002  .....}.|.|.f.W..
-00001a60: 0064 0004 0004 0083 0301 0053 0031 0073  .d.........S.1.s
-00001a70: 4230 0001 0001 0001 0059 0001 0064 0053  B0.......Y...d.S
-00001a80: 0029 034e 5a06 494d 4147 4558 5a06 494d  .).NZ.IMAGEXZ.IM
-00001a90: 4147 4559 a903 7255 0000 0072 2400 0000  AGEY..rU...r$...
-00001aa0: da03 6765 7429 0472 1700 0000 7254 0000  ..get).r....rT..
-00001ab0: 00da 0577 6964 7468 da06 6865 6967 6874  ...width..height
-00001ac0: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00001ad0: 0e72 6561 645f 7369 675f 7368 6170 65bc  .read_sig_shape.
-00001ae0: 0000 0073 0800 0000 0001 0a01 0e01 0e01  ...s............
-00001af0: 7a27 4d65 726c 696e 4465 7465 6374 6f72  z'MerlinDetector
-00001b00: 436f 6e6e 6563 7469 6f6e 2e72 6561 645f  Connection.read_
-00001b10: 7369 675f 7368 6170 6563 0100 0000 0000  sig_shapec......
-00001b20: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
-00001b30: 0000 733a 0000 007c 00a0 00a1 008f 1e7d  ..s:...|.......}
-00001b40: 0174 017c 01a0 0264 01a1 0183 0157 0002  .t.|...d.....W..
-00001b50: 0064 0004 0004 0083 0301 0053 0031 0073  .d.........S.1.s
-00001b60: 2c30 0001 0001 0001 0059 0001 0064 0053  ,0.......Y...d.S
-00001b70: 0029 024e 5a0c 434f 554e 5445 5244 4550  .).NZ.COUNTERDEP
-00001b80: 5448 7256 0000 0072 5300 0000 7218 0000  THrV...rS...r...
-00001b90: 0072 1800 0000 7219 0000 00da 0d72 6561  .r....r......rea
-00001ba0: 645f 6269 7464 6570 7468 c200 0000 7304  d_bitdepth....s.
-00001bb0: 0000 0000 010a 017a 264d 6572 6c69 6e44  .......z&MerlinD
-00001bc0: 6574 6563 746f 7243 6f6e 6e65 6374 696f  etectorConnectio
-00001bd0: 6e2e 7265 6164 5f62 6974 6465 7074 6863  n.read_bitdepthc
-00001be0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001bf0: 0200 0000 4300 0000 7312 0000 0064 0164  ....C...s....d.d
-00001c00: 026c 006d 017d 0101 007c 0183 0053 0029  .l.m.}...|...S.)
-00001c10: 034e 720a 0000 0029 01da 164d 6572 6c69  .Nr....)...Merli
-00001c20: 6e41 6374 6976 6543 6f6e 7472 6f6c 6c65  nActiveControlle
-00001c30: 7229 02da 0a63 6f6e 7472 6f6c 6c65 7272  r)...controllerr
-00001c40: 5c00 0000 2902 7217 0000 0072 5c00 0000  \...).r....r\...
-00001c50: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00001c60: 1567 6574 5f61 6374 6976 655f 636f 6e74  .get_active_cont
-00001c70: 726f 6c6c 6572 c600 0000 7304 0000 0000  roller....s.....
-00001c80: 010c 017a 2e4d 6572 6c69 6e44 6574 6563  ...z.MerlinDetec
-00001c90: 746f 7243 6f6e 6e65 6374 696f 6e2e 6765  torConnection.ge
-00001ca0: 745f 6163 7469 7665 5f63 6f6e 7472 6f6c  t_active_control
-00001cb0: 6c65 7229 014e 2901 724a 0000 0029 2072  ler).N).rJ...) r
-00001cc0: 2000 0000 7221 0000 0072 2200 0000 da07   ...r!...r".....
-00001cd0: 5f5f 646f 635f 5fda 0373 7472 7224 0000  __doc__..strr$..
-00001ce0: 00da 0462 6f6f 6c72 1a00 0000 7234 0000  ...boolr....r4..
-00001cf0: 0072 0200 0000 da05 666c 6f61 7472 0800  .r......floatr..
-00001d00: 0000 723e 0000 0072 0500 0000 720e 0000  ..r>...r....r...
-00001d10: 0072 0d00 0000 7244 0000 0072 0300 0000  .r....rD...r....
-00001d20: 7209 0000 0072 4700 0000 7248 0000 0072  r....rG...rH...r
-00001d30: 4900 0000 7251 0000 0072 0c00 0000 7252  I...rQ...r....rR
-00001d40: 0000 0072 0600 0000 7204 0000 0072 0b00  ...r....r....r..
-00001d50: 0000 7255 0000 0072 5a00 0000 725b 0000  ..rU...rZ...r[..
-00001d60: 0072 5e00 0000 7218 0000 0072 1800 0000  .r^...r....r....
-00001d70: 7218 0000 0072 1900 0000 7225 0000 0020  r....r....r%... 
-00001d80: 0000 0073 3400 0000 0801 042d 0201 0201  ...s4......-....
-00001d90: 0201 0201 02f9 0403 0201 0201 0201 0201  ................
-00001da0: 02f9 0c10 0807 1a2d 1609 1204 0805 0807  .......-........
-00001db0: 100b 0e04 0201 1a04 1606 0e04 7225 0000  ............r%..
-00001dc0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00001dd0: 0000 0800 0000 4000 0000 7336 0000 0065  ......@...s6...e
-00001de0: 005a 0164 005a 0264 015a 0364 0264 0364  .Z.d.Z.d.Z.d.d.d
-00001df0: 0264 0464 0564 069c 0565 0465 0565 0465  .d.d.d...e.e.e.e
-00001e00: 0565 0665 0764 079c 0664 0864 0984 065a  .e.e.d...d.d...Z
-00001e10: 0864 0a53 0029 0bda 174d 6572 6c69 6e43  .d.S.)...MerlinC
-00001e20: 6f6e 6e65 6374 696f 6e42 7569 6c64 6572  onnectionBuilder
-00001e30: 7a90 0a20 2020 2042 7569 6c64 6572 2063  z..    Builder c
-00001e40: 6c61 7373 2074 6861 7420 6361 6e20 636f  lass that can co
-00001e50: 6e73 7472 7563 7420 3a63 6c61 7373 3a60  nstruct :class:`
-00001e60: 4d65 726c 696e 4465 7465 6374 6f72 436f  MerlinDetectorCo
-00001e70: 6e6e 6563 7469 6f6e 6020 696e 7374 616e  nnection` instan
-00001e80: 6365 732e 0a0a 2020 2020 5573 6520 7468  ces...    Use th
-00001e90: 6520 3a6d 6574 683a 606f 7065 6e60 206d  e :meth:`open` m
-00001ea0: 6574 686f 6420 746f 2063 7265 6174 6520  ethod to create 
-00001eb0: 6120 636f 6e6e 6563 7469 6f6e 2e0a 2020  a connection..  
-00001ec0: 2020 7226 0000 0072 2700 0000 7228 0000    r&...r'...r(..
-00001ed0: 0046 7229 0000 0029 0672 2a00 0000 722b  .Fr)...).r*...r+
-00001ee0: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
-00001ef0: 0000 721d 0000 0063 0100 0000 0000 0000  ..r....c........
-00001f00: 0500 0000 0600 0000 0700 0000 4300 0000  ............C...
-00001f10: 7312 0000 0074 007c 017c 027c 037c 047c  s....t.|.|.|.|.|
-00001f20: 0564 018d 0553 0029 0261 cf04 0000 0a20  .d...S.).a..... 
-00001f30: 2020 2020 2020 2043 6f6e 6e65 6374 2074         Connect t
-00001f40: 6f20 6120 4d65 726c 696e 204d 6564 6970  o a Merlin Medip
-00001f50: 6978 2064 6574 6563 746f 7220 7379 7374  ix detector syst
-00001f60: 656d 2e0a 0a20 2020 2020 2020 2050 6172  em...        Par
-00001f70: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00001f80: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00001f90: 2020 2061 7069 5f68 6f73 740a 2020 2020     api_host.    
-00001fa0: 2020 2020 2020 2020 486f 7374 6e61 6d65          Hostname
-00001fb0: 206f 6620 7468 6520 4d65 726c 696e 2063   of the Merlin c
-00001fc0: 6f6e 7472 6f6c 2073 6572 7665 722c 2064  ontrol server, d
-00001fd0: 6566 6175 6c74 2027 3132 372e 302e 302e  efault '127.0.0.
-00001fe0: 3127 0a20 2020 2020 2020 2020 2020 2053  1'.            S
-00001ff0: 686f 756c 6420 696e 206d 6f73 7420 6361  hould in most ca
-00002000: 7365 7320 6265 2074 6865 2073 616d 6520  ses be the same 
-00002010: 6173 2060 6461 7461 5f68 6f73 7460 2e0a  as `data_host`..
-00002020: 2020 2020 2020 2020 6170 695f 706f 7274          api_port
-00002030: 0a20 2020 2020 2020 2020 2020 2050 6f72  .            Por
-00002040: 7420 6f66 2074 6865 204d 6572 6c69 6e20  t of the Merlin 
-00002050: 636f 6e74 726f 6c20 7365 7276 6572 2c20  control server, 
-00002060: 6465 6661 756c 7420 3633 3431 0a20 2020  default 6341.   
-00002070: 2020 2020 2064 6174 615f 686f 7374 0a20       data_host. 
-00002080: 2020 2020 2020 2020 2020 2048 6f73 746e             Hostn
-00002090: 616d 6520 6f66 2074 6865 204d 6572 6c69  ame of the Merli
-000020a0: 6e20 6461 7461 2073 6572 7665 722c 2064  n data server, d
-000020b0: 6566 6175 6c74 2027 3132 372e 302e 302e  efault '127.0.0.
-000020c0: 3127 0a20 2020 2020 2020 2064 6174 615f  1'.        data_
-000020d0: 706f 7274 0a20 2020 2020 2020 2020 2020  port.           
-000020e0: 2044 6174 6120 706f 7274 206f 6620 7468   Data port of th
-000020f0: 6520 4d65 726c 696e 2064 6174 6120 7365  e Merlin data se
-00002100: 7276 6572 2c20 6465 6661 756c 7420 3633  rver, default 63
-00002110: 3432 0a20 2020 2020 2020 2064 7261 696e  42.        drain
-00002120: 0a20 2020 2020 2020 2020 2020 2044 7261  .            Dra
-00002130: 696e 2074 6865 2073 6f63 6b65 7420 6265  in the socket be
-00002140: 666f 7265 2074 7269 6767 6572 696e 672e  fore triggering.
-00002150: 2045 6e61 626c 6520 7468 6973 2077 6865   Enable this whe
-00002160: 6e0a 2020 2020 2020 2020 2020 2020 7573  n.            us
-00002170: 696e 6720 6f6c 6420 7665 7273 696f 6e73  ing old versions
-00002180: 206f 6620 7468 6520 4d65 726c 696e 2073   of the Merlin s
-00002190: 6f66 7477 6172 652c 2062 7574 206e 6f74  oftware, but not
-000021a0: 2077 6865 6e0a 2020 2020 2020 2020 2020   when.          
-000021b0: 2020 7573 696e 6720 616e 2069 6e74 6572    using an inter
-000021c0: 6e61 6c20 7472 6967 6765 722e 0a0a 2020  nal trigger...  
-000021d0: 2020 2020 2020 4578 616d 706c 6573 0a20        Examples. 
-000021e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0a         --------.
-000021f0: 2020 2020 2020 2020 5573 7561 6c6c 792c          Usually,
-00002200: 2074 6869 7320 6d65 7468 6f64 2069 7320   this method is 
-00002210: 6469 7265 6374 6c79 2075 7365 6420 746f  directly used to
-00002220: 6765 7468 6572 2077 6974 680a 2020 2020  gether with.    
-00002230: 2020 2020 3a6d 6574 683a 606c 6962 6572      :meth:`liber
-00002240: 7465 6d5f 6c69 7665 2e61 7069 2e4c 6976  tem_live.api.Liv
-00002250: 6543 6f6e 7465 7874 2e6d 616b 655f 636f  eContext.make_co
-00002260: 6e6e 6563 7469 6f6e 603a 0a0a 2020 2020  nnection`:..    
-00002270: 2020 2020 3e3e 3e20 7769 7468 2063 7478      >>> with ctx
-00002280: 2e6d 616b 655f 636f 6e6e 6563 7469 6f6e  .make_connection
-00002290: 2827 6d65 726c 696e 2729 2e6f 7065 6e28  ('merlin').open(
-000022a0: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
-000022b0: 2061 7069 5f68 6f73 743d 2731 3237 2e30   api_host='127.0
-000022c0: 2e30 2e31 272c 0a20 2020 2020 2020 202e  .0.1',.        .
-000022d0: 2e2e 2020 2020 2061 7069 5f70 6f72 743d  ..     api_port=
-000022e0: 4d45 524c 494e 5f41 5049 5f50 4f52 542c  MERLIN_API_PORT,
-000022f0: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
-00002300: 2064 6174 615f 686f 7374 3d27 3132 372e   data_host='127.
-00002310: 302e 302e 3127 2c0a 2020 2020 2020 2020  0.0.1',.        
-00002320: 2e2e 2e20 2020 2020 6461 7461 5f70 6f72  ...     data_por
-00002330: 743d 4d45 524c 494e 5f44 4154 415f 504f  t=MERLIN_DATA_PO
-00002340: 5254 2c0a 2020 2020 2020 2020 2e2e 2e20  RT,.        ... 
-00002350: 2920 6173 2063 6f6e 6e3a 0a20 2020 2020  ) as conn:.     
-00002360: 2020 202e 2e2e 2020 2020 2061 7120 3d20     ...     aq = 
-00002370: 6374 782e 6d61 6b65 5f61 6371 7569 7369  ctx.make_acquisi
-00002380: 7469 6f6e 2863 6f6e 6e3d 636f 6e6e 2c20  tion(conn=conn, 
-00002390: 6e61 765f 7368 6170 653d 2833 322c 2033  nav_shape=(32, 3
-000023a0: 3229 290a 2020 2020 2020 2020 2e2e 2e20  2)).        ... 
-000023b0: 2020 2020 6374 782e 7275 6e5f 7564 6628      ctx.run_udf(
-000023c0: 6461 7461 7365 743d 6171 2c20 7564 663d  dataset=aq, udf=
-000023d0: 5375 6d55 4446 2829 290a 2020 2020 2020  SumUDF()).      
-000023e0: 2020 7b27 696e 7465 6e73 6974 7927 3a20    {'intensity': 
-000023f0: 2e2e 2e7d 0a20 2020 2020 2020 2072 2900  ...}.        r).
-00002400: 0000 2901 7225 0000 0072 3500 0000 7218  ..).r%...r5...r.
-00002410: 0000 0072 1800 0000 7219 0000 00da 046f  ...r....r......o
-00002420: 7065 6ed1 0000 0073 0e00 0000 002b 0201  pen....s.....+..
-00002430: 0201 0201 0201 0201 02fb 7a1c 4d65 726c  ..........z.Merl
-00002440: 696e 436f 6e6e 6563 7469 6f6e 4275 696c  inConnectionBuil
-00002450: 6465 722e 6f70 656e 4e29 0972 2000 0000  der.openN).r ...
-00002460: 7221 0000 0072 2200 0000 725f 0000 0072  r!...r"...r_...r
-00002470: 6000 0000 7224 0000 0072 6100 0000 7225  `...r$...ra...r%
-00002480: 0000 0072 6400 0000 7218 0000 0072 1800  ...rd...r....r..
-00002490: 0000 7218 0000 0072 1900 0000 7263 0000  ..r....r....rc..
-000024a0: 00cb 0000 0073 1c00 0000 0801 0408 0201  .....s..........
-000024b0: 0201 0201 0201 02f9 0403 0201 0201 0201  ................
-000024c0: 0201 0201 02f8 7263 0000 0029 1eda 076c  ......rc...)...l
-000024d0: 6f67 6769 6e67 da06 7479 7069 6e67 7202  ogging..typingr.
-000024e0: 0000 0072 0300 0000 7204 0000 0072 0500  ...r....r....r..
-000024f0: 0000 da0a 636f 6e74 6578 746c 6962 7206  ....contextlibr.
-00002500: 0000 005a 276c 6962 6572 7465 6d5f 6c69  ...Z'libertem_li
-00002510: 7665 2e64 6574 6563 746f 7273 2e62 6173  ve.detectors.bas
-00002520: 652e 636f 6e6e 6563 7469 6f6e 7207 0000  e.connectionr...
-00002530: 0072 0800 0000 da28 6c69 6265 7274 656d  .r.....(libertem
-00002540: 5f6c 6976 652e 6465 7465 6374 6f72 732e  _live.detectors.
-00002550: 6261 7365 2e61 6371 7569 7369 7469 6f6e  base.acquisition
-00002560: 7209 0000 0072 5500 0000 720b 0000 00da  r....rU...r.....
-00002570: 0464 6174 6172 0c00 0000 720d 0000 0072  .datar....r....r
-00002580: 0e00 0000 720f 0000 00da 0d6f 7065 6e74  ....r......opent
-00002590: 656c 656d 6574 7279 7210 0000 00da 0a67  elemetryr......g
-000025a0: 6574 5f74 7261 6365 7272 2000 0000 724b  et_tracerr ...rK
-000025b0: 0000 00da 0967 6574 4c6f 6767 6572 724e  .....getLoggerrN
-000025c0: 0000 0072 1100 0000 7225 0000 0072 6300  ...r....r%...rc.
-000025d0: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
-000025e0: 0072 1900 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-000025f0: 0100 0000 731a 0000 0008 0118 010c 0210  ....s...........
-00002600: 010c 020c 0118 040c 020a 010a 0310 0d10  ................
-00002610: 7f00 2c                                  ..,
+00000000: 696d 706f 7274 206c 6f67 6769 6e67 0a66  import logging.f
+00000010: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+00000020: 7420 4f70 7469 6f6e 616c 2c20 5479 7065  t Optional, Type
+00000030: 2c20 4765 6e65 7261 746f 722c 2054 7570  , Generator, Tup
+00000040: 6c65 0a66 726f 6d20 636f 6e74 6578 746c  le.from contextl
+00000050: 6962 2069 6d70 6f72 7420 636f 6e74 6578  ib import contex
+00000060: 746d 616e 6167 6572 0a0a 6672 6f6d 206c  tmanager..from l
+00000070: 6962 6572 7465 6d5f 6c69 7665 2e64 6574  ibertem_live.det
+00000080: 6563 746f 7273 2e62 6173 652e 636f 6e6e  ectors.base.conn
+00000090: 6563 7469 6f6e 2069 6d70 6f72 7420 4465  ection import De
+000000a0: 7465 6374 6f72 436f 6e6e 6563 7469 6f6e  tectorConnection
+000000b0: 2c20 5065 6e64 696e 6741 6371 7569 7369  , PendingAcquisi
+000000c0: 7469 6f6e 0a66 726f 6d20 6c69 6265 7274  tion.from libert
+000000d0: 656d 5f6c 6976 652e 6465 7465 6374 6f72  em_live.detector
+000000e0: 732e 6261 7365 2e61 6371 7569 7369 7469  s.base.acquisiti
+000000f0: 6f6e 2069 6d70 6f72 7420 4163 7175 6973  on import Acquis
+00000100: 6974 696f 6e50 726f 746f 636f 6c0a 0a66  itionProtocol..f
+00000110: 726f 6d20 2e63 6f6e 7472 6f6c 2069 6d70  rom .control imp
+00000120: 6f72 7420 4d65 726c 696e 436f 6e74 726f  ort MerlinContro
+00000130: 6c0a 6672 6f6d 202e 6461 7461 2069 6d70  l.from .data imp
+00000140: 6f72 7420 280a 2020 2020 4d65 726c 696e  ort (.    Merlin
+00000150: 5261 7753 6f63 6b65 742c 204d 6572 6c69  RawSocket, Merli
+00000160: 6e46 7261 6d65 5374 7265 616d 2c20 4163  nFrameStream, Ac
+00000170: 7175 6973 6974 696f 6e48 6561 6465 722c  quisitionHeader,
+00000180: 2041 6371 7569 7369 7469 6f6e 5469 6d65   AcquisitionTime
+00000190: 6f75 742c 0a29 0a0a 6672 6f6d 206f 7065  out,.)..from ope
+000001a0: 6e74 656c 656d 6574 7279 2069 6d70 6f72  ntelemetry impor
+000001b0: 7420 7472 6163 650a 0a74 7261 6365 7220  t trace..tracer 
+000001c0: 3d20 7472 6163 652e 6765 745f 7472 6163  = trace.get_trac
+000001d0: 6572 285f 5f6e 616d 655f 5f29 0a6c 6f67  er(__name__).log
+000001e0: 6765 7220 3d20 6c6f 6767 696e 672e 6765  ger = logging.ge
+000001f0: 744c 6f67 6765 7228 5f5f 6e61 6d65 5f5f  tLogger(__name__
+00000200: 290a 0a0a 636c 6173 7320 4d65 726c 696e  )...class Merlin
+00000210: 5065 6e64 696e 6741 6371 7569 7369 7469  PendingAcquisiti
+00000220: 6f6e 2850 656e 6469 6e67 4163 7175 6973  on(PendingAcquis
+00000230: 6974 696f 6e29 3a0a 2020 2020 6465 6620  ition):.    def 
+00000240: 5f5f 696e 6974 5f5f 2873 656c 662c 2068  __init__(self, h
+00000250: 6561 6465 723a 2041 6371 7569 7369 7469  eader: Acquisiti
+00000260: 6f6e 4865 6164 6572 293a 0a20 2020 2020  onHeader):.     
+00000270: 2020 2073 656c 662e 5f68 6561 6465 7220     self._header 
+00000280: 3d20 6865 6164 6572 0a0a 2020 2020 4070  = header..    @p
+00000290: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+000002a0: 6865 6164 6572 2873 656c 6629 3a0a 2020  header(self):.  
+000002b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000002c0: 662e 5f68 6561 6465 720a 0a20 2020 2040  f._header..    @
+000002d0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+000002e0: 206e 696d 6167 6573 2873 656c 6629 202d   nimages(self) -
+000002f0: 3e20 696e 743a 0a20 2020 2020 2020 2072  > int:.        r
+00000300: 6574 7572 6e20 7365 6c66 2e68 6561 6465  eturn self.heade
+00000310: 722e 6672 616d 6573 5f69 6e5f 6163 7175  r.frames_in_acqu
+00000320: 6973 6974 696f 6e0a 0a0a 636c 6173 7320  isition...class 
+00000330: 4d65 726c 696e 4465 7465 6374 6f72 436f  MerlinDetectorCo
+00000340: 6e6e 6563 7469 6f6e 2844 6574 6563 746f  nnection(Detecto
+00000350: 7243 6f6e 6e65 6374 696f 6e29 3a0a 2020  rConnection):.  
+00000360: 2020 2222 220a 2020 2020 5468 6973 2063    """.    This c
+00000370: 6c61 7373 2068 6f6c 6473 2061 2070 6572  lass holds a per
+00000380: 6d61 6e65 6e74 2064 6174 6120 636f 6e6e  manent data conn
+00000390: 6563 7469 6f6e 2074 6f20 7468 6520 6d65  ection to the me
+000003a0: 726c 696e 2073 6f66 7477 6172 652e 0a0a  rlin software...
+000003b0: 2020 2020 436f 6e74 726f 6c20 636f 6e6e      Control conn
+000003c0: 6563 7469 6f6e 7320 6172 6520 616c 736f  ections are also
+000003d0: 2070 6f73 7369 626c 6520 746f 206f 6274   possible to obt
+000003e0: 6169 6e20 6672 6f6d 2074 6869 7320 636c  ain from this cl
+000003f0: 6173 732c 0a20 2020 2062 7574 2061 7265  ass,.    but are
+00000400: 2063 7265 6174 6564 206f 6e20 6465 6d61   created on dema
+00000410: 6e64 2061 6e64 206e 6f74 206b 6570 7420  nd and not kept 
+00000420: 6f70 656e 2e0a 0a20 2020 2059 6f75 2063  open...    You c
+00000430: 616e 2075 7365 2074 6865 2063 6f6e 7665  an use the conve
+00000440: 6e69 656e 6365 2066 756e 6374 696f 6e0a  nience function.
+00000450: 2020 2020 3a6d 6574 683a 606c 6962 6572      :meth:`liber
+00000460: 7465 6d5f 6c69 7665 2e61 7069 2e4c 6976  tem_live.api.Liv
+00000470: 6543 6f6e 7465 7874 2e6d 616b 655f 636f  eContext.make_co
+00000480: 6e6e 6563 7469 6f6e 6020 746f 2063 7265  nnection` to cre
+00000490: 6174 6520 616e 2069 6e73 7461 6e63 652c  ate an instance,
+000004a0: 0a20 2020 2069 6e73 7465 6164 206f 6620  .    instead of 
+000004b0: 6361 6c6c 696e 6720 7468 6973 2063 6f6e  calling this con
+000004c0: 7374 7275 6374 6f72 2064 6972 6563 746c  structor directl
+000004d0: 792e 0a0a 2020 2020 5061 7261 6d65 7465  y...    Paramete
+000004e0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+000004f0: 2d0a 2020 2020 6170 695f 686f 7374 0a20  -.    api_host. 
+00000500: 2020 2020 2020 2048 6f73 746e 616d 6520         Hostname 
+00000510: 6f66 2074 6865 204d 6572 6c69 6e20 636f  of the Merlin co
+00000520: 6e74 726f 6c20 7365 7276 6572 2c20 6465  ntrol server, de
+00000530: 6661 756c 7420 2731 3237 2e30 2e30 2e31  fault '127.0.0.1
+00000540: 270a 2020 2020 2020 2020 5368 6f75 6c64  '.        Should
+00000550: 2069 6e20 6d6f 7374 2063 6173 6573 2062   in most cases b
+00000560: 6520 7468 6520 7361 6d65 2061 7320 6064  e the same as `d
+00000570: 6174 615f 686f 7374 602e 0a20 2020 2061  ata_host`..    a
+00000580: 7069 5f70 6f72 740a 2020 2020 2020 2020  pi_port.        
+00000590: 506f 7274 206f 6620 7468 6520 4d65 726c  Port of the Merl
+000005a0: 696e 2063 6f6e 7472 6f6c 2073 6572 7665  in control serve
+000005b0: 722c 2064 6566 6175 6c74 2036 3334 310a  r, default 6341.
+000005c0: 2020 2020 6461 7461 5f68 6f73 740a 2020      data_host.  
+000005d0: 2020 2020 2020 486f 7374 6e61 6d65 206f        Hostname o
+000005e0: 6620 7468 6520 4d65 726c 696e 2064 6174  f the Merlin dat
+000005f0: 6120 7365 7276 6572 2c20 6465 6661 756c  a server, defaul
+00000600: 7420 2731 3237 2e30 2e30 2e31 270a 2020  t '127.0.0.1'.  
+00000610: 2020 6461 7461 5f70 6f72 740a 2020 2020    data_port.    
+00000620: 2020 2020 4461 7461 2070 6f72 7420 6f66      Data port of
+00000630: 2074 6865 204d 6572 6c69 6e20 6461 7461   the Merlin data
+00000640: 2073 6572 7665 722c 2064 6566 6175 6c74   server, default
+00000650: 2036 3334 320a 2020 2020 6472 6169 6e0a   6342.    drain.
+00000660: 2020 2020 2020 2020 4472 6169 6e20 7468          Drain th
+00000670: 6520 736f 636b 6574 2062 6566 6f72 6520  e socket before 
+00000680: 7472 6967 6765 7269 6e67 2e20 456e 6162  triggering. Enab
+00000690: 6c65 2074 6869 7320 7768 656e 0a20 2020  le this when.   
+000006a0: 2020 2020 2075 7369 6e67 206f 6c64 2076       using old v
+000006b0: 6572 7369 6f6e 7320 6f66 2074 6865 204d  ersions of the M
+000006c0: 6572 6c69 6e20 736f 6674 7761 7265 2c20  erlin software, 
+000006d0: 6275 7420 6e6f 7420 7768 656e 0a20 2020  but not when.   
+000006e0: 2020 2020 2075 7369 6e67 2061 6e20 696e       using an in
+000006f0: 7465 726e 616c 2074 7269 6767 6572 2e0a  ternal trigger..
+00000700: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
+00000710: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2055    --------.    U
+00000720: 7375 616c 6c79 2c20 7468 6973 2063 6c61  sually, this cla
+00000730: 7373 2069 7320 696e 7374 616e 7469 6174  ss is instantiat
+00000740: 6564 2075 7369 6e67 0a20 2020 203a 6d65  ed using.    :me
+00000750: 7468 3a60 6c69 6265 7274 656d 5f6c 6976  th:`libertem_liv
+00000760: 652e 6170 692e 4c69 7665 436f 6e74 6578  e.api.LiveContex
+00000770: 742e 6d61 6b65 5f63 6f6e 6e65 6374 696f  t.make_connectio
+00000780: 6e60 3a0a 0a20 2020 203e 3e3e 2077 6974  n`:..    >>> wit
+00000790: 6820 6374 782e 6d61 6b65 5f63 6f6e 6e65  h ctx.make_conne
+000007a0: 6374 696f 6e28 276d 6572 6c69 6e27 292e  ction('merlin').
+000007b0: 6f70 656e 280a 2020 2020 2e2e 2e20 2020  open(.    ...   
+000007c0: 2020 6170 695f 686f 7374 3d27 3132 372e    api_host='127.
+000007d0: 302e 302e 3127 2c0a 2020 2020 2e2e 2e20  0.0.1',.    ... 
+000007e0: 2020 2020 6170 695f 706f 7274 3d4d 4552      api_port=MER
+000007f0: 4c49 4e5f 4150 495f 504f 5254 2c0a 2020  LIN_API_PORT,.  
+00000800: 2020 2e2e 2e20 2020 2020 6461 7461 5f68    ...     data_h
+00000810: 6f73 743d 2731 3237 2e30 2e30 2e31 272c  ost='127.0.0.1',
+00000820: 0a20 2020 202e 2e2e 2020 2020 2064 6174  .    ...     dat
+00000830: 615f 706f 7274 3d4d 4552 4c49 4e5f 4441  a_port=MERLIN_DA
+00000840: 5441 5f50 4f52 542c 0a20 2020 202e 2e2e  TA_PORT,.    ...
+00000850: 2029 2061 7320 636f 6e6e 3a0a 2020 2020   ) as conn:.    
+00000860: 2e2e 2e20 2020 2020 6171 203d 2063 7478  ...     aq = ctx
+00000870: 2e6d 616b 655f 6163 7175 6973 6974 696f  .make_acquisitio
+00000880: 6e28 636f 6e6e 3d63 6f6e 6e2c 206e 6176  n(conn=conn, nav
+00000890: 5f73 6861 7065 3d28 3332 2c20 3332 2929  _shape=(32, 32))
+000008a0: 0a20 2020 202e 2e2e 2020 2020 2063 7478  .    ...     ctx
+000008b0: 2e72 756e 5f75 6466 2864 6174 6173 6574  .run_udf(dataset
+000008c0: 3d61 712c 2075 6466 3d53 756d 5544 4628  =aq, udf=SumUDF(
+000008d0: 2929 0a20 2020 207b 2769 6e74 656e 7369  )).    {'intensi
+000008e0: 7479 273a 202e 2e2e 7d0a 2020 2020 2222  ty': ...}.    ""
+000008f0: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+00000900: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00000910: 662c 0a20 2020 2020 2020 202a 2c0a 2020  f,.        *,.  
+00000920: 2020 2020 2020 6170 695f 686f 7374 3a20        api_host: 
+00000930: 7374 7220 3d20 2731 3237 2e30 2e30 2e31  str = '127.0.0.1
+00000940: 272c 0a20 2020 2020 2020 2061 7069 5f70  ',.        api_p
+00000950: 6f72 743a 2069 6e74 203d 2036 3334 312c  ort: int = 6341,
+00000960: 0a20 2020 2020 2020 2064 6174 615f 686f  .        data_ho
+00000970: 7374 3a20 7374 7220 3d20 2731 3237 2e30  st: str = '127.0
+00000980: 2e30 2e31 272c 0a20 2020 2020 2020 2064  .0.1',.        d
+00000990: 6174 615f 706f 7274 3a20 696e 7420 3d20  ata_port: int = 
+000009a0: 3633 3432 2c0a 2020 2020 2020 2020 6472  6342,.        dr
+000009b0: 6169 6e3a 2062 6f6f 6c20 3d20 4661 6c73  ain: bool = Fals
+000009c0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+000009d0: 2020 7365 6c66 2e5f 6170 695f 686f 7374    self._api_host
+000009e0: 203d 2061 7069 5f68 6f73 740a 2020 2020   = api_host.    
+000009f0: 2020 2020 7365 6c66 2e5f 6170 695f 706f      self._api_po
+00000a00: 7274 203d 2061 7069 5f70 6f72 740a 2020  rt = api_port.  
+00000a10: 2020 2020 2020 7365 6c66 2e5f 6461 7461        self._data
+00000a20: 5f68 6f73 7420 3d20 6461 7461 5f68 6f73  _host = data_hos
+00000a30: 740a 2020 2020 2020 2020 7365 6c66 2e5f  t.        self._
+00000a40: 6461 7461 5f70 6f72 7420 3d20 6461 7461  data_port = data
+00000a50: 5f70 6f72 740a 2020 2020 2020 2020 7365  _port.        se
+00000a60: 6c66 2e5f 6472 6169 6e20 3d20 6472 6169  lf._drain = drai
+00000a70: 6e0a 2020 2020 2020 2020 7365 6c66 2e5f  n.        self._
+00000a80: 636f 6e6e 6563 7428 290a 0a20 2020 2064  connect()..    d
+00000a90: 6566 205f 636f 6e6e 6563 7428 7365 6c66  ef _connect(self
+00000aa0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00000ab0: 5f64 6174 615f 736f 636b 6574 203d 204d  _data_socket = M
+00000ac0: 6572 6c69 6e52 6177 536f 636b 6574 280a  erlinRawSocket(.
+00000ad0: 2020 2020 2020 2020 2020 2020 686f 7374              host
+00000ae0: 3d73 656c 662e 5f64 6174 615f 686f 7374  =self._data_host
+00000af0: 2c0a 2020 2020 2020 2020 2020 2020 706f  ,.            po
+00000b00: 7274 3d73 656c 662e 5f64 6174 615f 706f  rt=self._data_po
+00000b10: 7274 2c0a 2020 2020 2020 2020 292e 636f  rt,.        ).co
+00000b20: 6e6e 6563 7428 290a 2020 2020 2020 2020  nnect().        
+00000b30: 7265 7475 726e 2073 656c 662e 5f64 6174  return self._dat
+00000b40: 615f 736f 636b 6574 0a0a 2020 2020 6465  a_socket..    de
+00000b50: 6620 7761 6974 5f66 6f72 5f61 6371 7569  f wait_for_acqui
+00000b60: 7369 7469 6f6e 2873 656c 662c 2074 696d  sition(self, tim
+00000b70: 656f 7574 3a20 4f70 7469 6f6e 616c 5b66  eout: Optional[f
+00000b80: 6c6f 6174 5d20 3d20 4e6f 6e65 2920 2d3e  loat] = None) ->
+00000b90: 204f 7074 696f 6e61 6c5b 5065 6e64 696e   Optional[Pendin
+00000ba0: 6741 6371 7569 7369 7469 6f6e 5d3a 0a20  gAcquisition]:. 
+00000bb0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00000bc0: 2020 2057 6169 7420 666f 7220 6174 206d     Wait for at m
+00000bd0: 6f73 7420 6074 696d 656f 7574 6020 7365  ost `timeout` se
+00000be0: 636f 6e64 7320 666f 7220 616e 2061 6371  conds for an acq
+00000bf0: 7569 7369 7469 6f6e 2074 6f20 7374 6172  uisition to star
+00000c00: 742e 2054 6869 730a 2020 2020 2020 2020  t. This.        
+00000c10: 646f 6573 206e 6f74 2070 6572 666f 726d  does not perform
+00000c20: 2061 6e79 2074 7269 6767 6572 696e 6720   any triggering 
+00000c30: 6974 7365 6c66 2061 6e64 2065 7870 6563  itself and expec
+00000c40: 7473 2073 6f6d 6574 6869 6e67 2065 7874  ts something ext
+00000c50: 6572 6e61 6c0a 2020 2020 2020 2020 746f  ernal.        to
+00000c60: 2061 726d 2061 6e64 2074 7269 6767 6572   arm and trigger
+00000c70: 2074 6865 2061 6371 7569 7369 7469 6f6e   the acquisition
+00000c80: 2e0a 0a20 2020 2020 2020 204f 6e63 6520  ...        Once 
+00000c90: 7468 6520 6465 7465 6374 6f72 2069 7320  the detector is 
+00000ca0: 6172 6d65 642c 2074 6869 7320 6675 6e63  armed, this func
+00000cb0: 7469 6f6e 2072 6574 7572 6e73 2061 2060  tion returns a `
+00000cc0: 5065 6e64 696e 6741 6371 7569 7369 7469  PendingAcquisiti
+00000cd0: 6f6e 602c 0a20 2020 2020 2020 2077 6869  on`,.        whi
+00000ce0: 6368 2063 616e 2062 6520 636f 6e76 6572  ch can be conver
+00000cf0: 7465 6420 746f 2061 2066 756c 6c20 6041  ted to a full `A
+00000d00: 6371 7569 7369 7469 6f6e 6020 6f62 6a65  cquisition` obje
+00000d10: 6374 2075 7369 6e67 0a20 2020 2020 2020  ct using.       
+00000d20: 203a 6d65 7468 3a60 6c69 6265 7274 656d   :meth:`libertem
+00000d30: 5f6c 6976 652e 6170 692e 4c69 7665 436f  _live.api.LiveCo
+00000d40: 6e74 6578 742e 6d61 6b65 5f61 6371 7569  ntext.make_acqui
+00000d50: 7369 7469 6f6e 602e 0a0a 2020 2020 2020  sition`...      
+00000d60: 2020 5468 6520 6675 6e63 7469 6f6e 2072    The function r
+00000d70: 6574 7572 6e73 2060 4e6f 6e65 6020 6f6e  eturns `None` on
+00000d80: 2074 696d 656f 7574 2e0a 0a20 2020 2020   timeout...     
+00000d90: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00000da0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00000db0: 0a20 2020 2020 2020 2074 696d 656f 7574  .        timeout
+00000dc0: 0a20 2020 2020 2020 2020 2020 2054 696d  .            Tim
+00000dd0: 656f 7574 2069 6e20 7365 636f 6e64 732e  eout in seconds.
+00000de0: 2049 6620 604e 6f6e 6560 2c20 7761 6974   If `None`, wait
+00000df0: 2069 6e64 6566 696e 6974 656c 792e 0a0a   indefinitely...
+00000e00: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
+00000e10: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00000e20: 2d0a 2020 2020 2020 2020 3e3e 3e20 7769  -.        >>> wi
+00000e30: 7468 2063 7478 2e6d 616b 655f 636f 6e6e  th ctx.make_conn
+00000e40: 6563 7469 6f6e 2827 6d65 726c 696e 2729  ection('merlin')
+00000e50: 2e6f 7065 6e28 0a20 2020 2020 2020 202e  .open(.        .
+00000e60: 2e2e 2020 2020 2061 7069 5f68 6f73 743d  ..     api_host=
+00000e70: 2731 3237 2e30 2e30 2e31 272c 0a20 2020  '127.0.0.1',.   
+00000e80: 2020 2020 202e 2e2e 2020 2020 2061 7069       ...     api
+00000e90: 5f70 6f72 743d 4d45 524c 494e 5f41 5049  _port=MERLIN_API
+00000ea0: 5f50 4f52 542c 0a20 2020 2020 2020 202e  _PORT,.        .
+00000eb0: 2e2e 2020 2020 2064 6174 615f 686f 7374  ..     data_host
+00000ec0: 3d27 3132 372e 302e 302e 3127 2c0a 2020  ='127.0.0.1',.  
+00000ed0: 2020 2020 2020 2e2e 2e20 2020 2020 6461        ...     da
+00000ee0: 7461 5f70 6f72 743d 4d45 524c 494e 5f44  ta_port=MERLIN_D
+00000ef0: 4154 415f 504f 5254 2c0a 2020 2020 2020  ATA_PORT,.      
+00000f00: 2020 2e2e 2e20 2920 6173 2063 6f6e 6e3a    ... ) as conn:
+00000f10: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
+00000f20: 2070 656e 6469 6e67 5f61 7120 3d20 636f   pending_aq = co
+00000f30: 6e6e 2e77 6169 745f 666f 725f 6163 7175  nn.wait_for_acqu
+00000f40: 6973 6974 696f 6e28 7469 6d65 6f75 743d  isition(timeout=
+00000f50: 3129 0a20 2020 2020 2020 202e 2e2e 2020  1).        ...  
+00000f60: 2020 2023 2061 7420 7468 6973 2070 6f69     # at this poi
+00000f70: 6e74 2c20 736f 6d65 7468 696e 6720 656c  nt, something el
+00000f80: 7365 2069 7320 6172 6d69 6e67 2061 6e64  se is arming and
+00000f90: 2074 7269 6767 6572 696e 6720 7468 650a   triggering the.
+00000fa0: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
+00000fb0: 2320 6465 7465 6374 6f72 3a0a 2020 2020  # detector:.    
+00000fc0: 2020 2020 2e2e 2e20 2020 2020 6171 203d      ...     aq =
+00000fd0: 2063 7478 2e6d 616b 655f 6163 7175 6973   ctx.make_acquis
+00000fe0: 6974 696f 6e28 0a20 2020 2020 2020 202e  ition(.        .
+00000ff0: 2e2e 2020 2020 2020 2020 2063 6f6e 6e3d  ..         conn=
+00001000: 636f 6e6e 2c0a 2020 2020 2020 2020 2e2e  conn,.        ..
+00001010: 2e20 2020 2020 2020 2020 6e61 765f 7368  .         nav_sh
+00001020: 6170 653d 2833 322c 2033 3229 2c0a 2020  ape=(32, 32),.  
+00001030: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
+00001040: 2020 7065 6e64 696e 675f 6171 3d70 656e    pending_aq=pen
+00001050: 6469 6e67 5f61 712c 0a20 2020 2020 2020  ding_aq,.       
+00001060: 202e 2e2e 2020 2020 2029 0a20 2020 2020   ...     ).     
+00001070: 2020 202e 2e2e 2020 2020 2063 7478 2e72     ...     ctx.r
+00001080: 756e 5f75 6466 2864 6174 6173 6574 3d61  un_udf(dataset=a
+00001090: 712c 2075 6466 3d53 756d 5544 4628 2929  q, udf=SumUDF())
+000010a0: 0a20 2020 2020 2020 207b 2769 6e74 656e  .        {'inten
+000010b0: 7369 7479 273a 202e 2e2e 7d0a 2020 2020  sity': ...}.    
+000010c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000010d0: 6966 2073 656c 662e 5f64 6174 615f 736f  if self._data_so
+000010e0: 636b 6574 2069 7320 4e6f 6e65 3a0a 2020  cket is None:.  
+000010f0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00001100: 636f 6e6e 6563 7428 290a 2020 2020 2020  connect().      
+00001110: 2020 6173 7365 7274 2073 656c 662e 5f64    assert self._d
+00001120: 6174 615f 736f 636b 6574 2069 7320 6e6f  ata_socket is no
+00001130: 7420 4e6f 6e65 0a20 2020 2020 2020 2074  t None.        t
+00001140: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00001150: 6865 6164 6572 203d 2073 656c 662e 5f64  header = self._d
+00001160: 6174 615f 736f 636b 6574 2e72 6561 645f  ata_socket.read_
+00001170: 6163 7175 6973 6974 696f 6e5f 6865 6164  acquisition_head
+00001180: 6572 2863 616e 6365 6c5f 7469 6d65 6f75  er(cancel_timeou
+00001190: 743d 7469 6d65 6f75 7429 0a20 2020 2020  t=timeout).     
+000011a0: 2020 2020 2020 2072 6574 7572 6e20 4d65         return Me
+000011b0: 726c 696e 5065 6e64 696e 6741 6371 7569  rlinPendingAcqui
+000011c0: 7369 7469 6f6e 2868 6561 6465 723d 6865  sition(header=he
+000011d0: 6164 6572 290a 2020 2020 2020 2020 6578  ader).        ex
+000011e0: 6365 7074 2041 6371 7569 7369 7469 6f6e  cept Acquisition
+000011f0: 5469 6d65 6f75 743a 0a20 2020 2020 2020  Timeout:.       
+00001200: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00001210: 0a0a 2020 2020 6465 6620 6765 745f 6865  ..    def get_he
+00001220: 6164 6572 5f61 6e64 5f73 7472 6561 6d28  ader_and_stream(
+00001230: 7365 6c66 2920 2d3e 2054 7570 6c65 5b41  self) -> Tuple[A
+00001240: 6371 7569 7369 7469 6f6e 4865 6164 6572  cquisitionHeader
+00001250: 2c20 4d65 726c 696e 4672 616d 6553 7472  , MerlinFrameStr
+00001260: 6561 6d5d 3a0a 2020 2020 2020 2020 6173  eam]:.        as
+00001270: 7365 7274 2073 656c 662e 5f64 6174 615f  sert self._data_
+00001280: 736f 636b 6574 2069 7320 6e6f 7420 4e6f  socket is not No
+00001290: 6e65 0a20 2020 2020 2020 2061 6371 5f68  ne.        acq_h
+000012a0: 6561 6465 7220 3d20 7365 6c66 2e5f 6461  eader = self._da
+000012b0: 7461 5f73 6f63 6b65 742e 7265 6164 5f61  ta_socket.read_a
+000012c0: 6371 7569 7369 7469 6f6e 5f68 6561 6465  cquisition_heade
+000012d0: 7228 290a 2020 2020 2020 2020 7374 7265  r().        stre
+000012e0: 616d 203d 204d 6572 6c69 6e46 7261 6d65  am = MerlinFrame
+000012f0: 5374 7265 616d 2e66 726f 6d5f 6672 616d  Stream.from_fram
+00001300: 655f 6865 6164 6572 280a 2020 2020 2020  e_header(.      
+00001310: 2020 2020 2020 7261 775f 736f 636b 6574        raw_socket
+00001320: 3d73 656c 662e 5f64 6174 615f 736f 636b  =self._data_sock
+00001330: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
+00001340: 6163 7175 6973 6974 696f 6e5f 6865 6164  acquisition_head
+00001350: 6572 3d61 6371 5f68 6561 6465 722c 0a20  er=acq_header,. 
+00001360: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00001370: 2072 6574 7572 6e20 6163 715f 6865 6164   return acq_head
+00001380: 6572 2c20 7374 7265 616d 0a0a 2020 2020  er, stream..    
+00001390: 6465 6620 6765 745f 6163 7175 6973 6974  def get_acquisit
+000013a0: 696f 6e5f 636c 7328 7365 6c66 2920 2d3e  ion_cls(self) ->
+000013b0: 2054 7970 655b 4163 7175 6973 6974 696f   Type[Acquisitio
+000013c0: 6e50 726f 746f 636f 6c5d 3a0a 2020 2020  nProtocol]:.    
+000013d0: 2020 2020 6672 6f6d 202e 6163 7175 6973      from .acquis
+000013e0: 6974 696f 6e20 696d 706f 7274 204d 6572  ition import Mer
+000013f0: 6c69 6e41 6371 7569 7369 7469 6f6e 0a20  linAcquisition. 
+00001400: 2020 2020 2020 2072 6574 7572 6e20 4d65         return Me
+00001410: 726c 696e 4163 7175 6973 6974 696f 6e0a  rlinAcquisition.
+00001420: 0a20 2020 2064 6566 205f 5f65 6e74 6572  .    def __enter
+00001430: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+00001440: 2020 6966 2073 656c 662e 5f64 6174 615f    if self._data_
+00001450: 736f 636b 6574 2069 7320 4e6f 6e65 3a0a  socket is None:.
+00001460: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001470: 2e5f 636f 6e6e 6563 7428 290a 2020 2020  ._connect().    
+00001480: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00001490: 0a20 2020 2064 6566 2063 6c6f 7365 2873  .    def close(s
+000014a0: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
+000014b0: 696d 706c 656d 656e 7469 6e67 2022 636c  implementing "cl
+000014c0: 6f73 6522 2061 6e64 205f 5f65 6e74 6572  ose" and __enter
+000014d0: 5f5f 2061 626f 7665 2067 6976 6573 2075  __ above gives u
+000014e0: 7320 636f 6e74 6578 746d 616e 6167 6572  s contextmanager
+000014f0: 2041 5049 0a20 2020 2020 2020 2023 2066   API.        # f
+00001500: 6f72 2066 7265 653a 0a20 2020 2020 2020  or free:.       
+00001510: 2069 6620 7365 6c66 2e5f 6461 7461 5f73   if self._data_s
+00001520: 6f63 6b65 7420 6973 206e 6f74 204e 6f6e  ocket is not Non
+00001530: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00001540: 656c 662e 5f64 6174 615f 736f 636b 6574  elf._data_socket
+00001550: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+00001560: 2020 2020 2073 656c 662e 5f64 6174 615f       self._data_
+00001570: 736f 636b 6574 203d 204e 6f6e 650a 0a20  socket = None.. 
+00001580: 2020 2064 6566 206d 6179 6265 5f64 7261     def maybe_dra
+00001590: 696e 2873 656c 662c 2074 696d 656f 7574  in(self, timeout
+000015a0: 3a20 666c 6f61 7420 3d20 312e 3029 3a0a  : float = 1.0):.
+000015b0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+000015c0: 656c 662e 5f64 6174 615f 736f 636b 6574  elf._data_socket
+000015d0: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+000015e0: 2020 2020 2069 6620 7365 6c66 2e5f 6472       if self._dr
+000015f0: 6169 6e3a 0a20 2020 2020 2020 2020 2020  ain:.           
+00001600: 2077 6974 6820 7472 6163 6572 2e73 7461   with tracer.sta
+00001610: 7274 5f61 735f 6375 7272 656e 745f 7370  rt_as_current_sp
+00001620: 616e 2822 6472 6169 6e22 2920 6173 2073  an("drain") as s
+00001630: 7061 6e3a 0a20 2020 2020 2020 2020 2020  pan:.           
+00001640: 2020 2020 2064 7261 696e 6564 5f62 7974       drained_byt
+00001650: 6573 203d 2073 656c 662e 5f64 6174 615f  es = self._data_
+00001660: 736f 636b 6574 2e64 7261 696e 2829 0a20  socket.drain(). 
+00001670: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001680: 7061 6e2e 7365 745f 6174 7472 6962 7574  pan.set_attribut
+00001690: 6573 287b 0a20 2020 2020 2020 2020 2020  es({.           
+000016a0: 2020 2020 2020 2020 2022 6c69 6265 7274           "libert
+000016b0: 656d 5f6c 6976 652e 6472 6169 6e65 645f  em_live.drained_
+000016c0: 6279 7465 7322 3a20 6472 6169 6e65 645f  bytes": drained_
+000016d0: 6279 7465 732c 0a20 2020 2020 2020 2020  bytes,.         
+000016e0: 2020 2020 2020 207d 290a 2020 2020 2020         }).      
+000016f0: 2020 2020 2020 6966 2064 7261 696e 6564        if drained
+00001700: 5f62 7974 6573 203e 2030 3a0a 2020 2020  _bytes > 0:.    
+00001710: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00001720: 6572 2e69 6e66 6f28 6622 6472 6169 6e65  er.info(f"draine
+00001730: 6420 7b64 7261 696e 6564 5f62 7974 6573  d {drained_bytes
+00001740: 7d20 6279 7465 7320 6f66 2067 6172 6261  } bytes of garba
+00001750: 6765 2229 0a0a 2020 2020 6465 6620 6765  ge")..    def ge
+00001760: 745f 6461 7461 5f73 6f63 6b65 7428 7365  t_data_socket(se
+00001770: 6c66 2920 2d3e 204d 6572 6c69 6e52 6177  lf) -> MerlinRaw
+00001780: 536f 636b 6574 3a0a 2020 2020 2020 2020  Socket:.        
+00001790: 6173 7365 7274 2073 656c 662e 5f64 6174  assert self._dat
+000017a0: 615f 736f 636b 6574 2069 7320 6e6f 7420  a_socket is not 
+000017b0: 4e6f 6e65 2c20 226e 6565 6420 746f 2062  None, "need to b
+000017c0: 6520 636f 6e6e 6563 7465 6420 746f 2063  e connected to c
+000017d0: 616c 6c20 7468 6973 220a 2020 2020 2020  all this".      
+000017e0: 2020 7265 7475 726e 2073 656c 662e 5f64    return self._d
+000017f0: 6174 615f 736f 636b 6574 0a0a 2020 2020  ata_socket..    
+00001800: 4063 6f6e 7465 7874 6d61 6e61 6765 720a  @contextmanager.
+00001810: 2020 2020 6465 6620 636f 6e74 726f 6c28      def control(
+00001820: 7365 6c66 2920 2d3e 2047 656e 6572 6174  self) -> Generat
+00001830: 6f72 5b4d 6572 6c69 6e43 6f6e 7472 6f6c  or[MerlinControl
+00001840: 2c20 4e6f 6e65 2c20 4e6f 6e65 5d3a 0a20  , None, None]:. 
+00001850: 2020 2020 2020 2077 6974 6820 4d65 726c         with Merl
+00001860: 696e 436f 6e74 726f 6c28 686f 7374 3d73  inControl(host=s
+00001870: 656c 662e 5f61 7069 5f68 6f73 742c 2070  elf._api_host, p
+00001880: 6f72 743d 7365 6c66 2e5f 6170 695f 706f  ort=self._api_po
+00001890: 7274 2920 6173 2063 3a0a 2020 2020 2020  rt) as c:.      
+000018a0: 2020 2020 2020 7969 656c 6420 630a 0a20        yield c.. 
+000018b0: 2020 2064 6566 2072 6561 645f 7369 675f     def read_sig_
+000018c0: 7368 6170 6528 7365 6c66 2920 2d3e 2054  shape(self) -> T
+000018d0: 7570 6c65 5b69 6e74 2c20 696e 745d 3a0a  uple[int, int]:.
+000018e0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000018f0: 662e 636f 6e74 726f 6c28 2920 6173 2063  f.control() as c
+00001900: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+00001910: 6474 6820 3d20 696e 7428 632e 6765 7428  dth = int(c.get(
+00001920: 2749 4d41 4745 5827 2929 0a20 2020 2020  'IMAGEX')).     
+00001930: 2020 2020 2020 2068 6569 6768 7420 3d20         height = 
+00001940: 696e 7428 632e 6765 7428 2749 4d41 4745  int(c.get('IMAGE
+00001950: 5927 2929 0a20 2020 2020 2020 2020 2020  Y')).           
+00001960: 2072 6574 7572 6e20 2868 6569 6768 742c   return (height,
+00001970: 2077 6964 7468 290a 0a20 2020 2064 6566   width)..    def
+00001980: 2072 6561 645f 6269 7464 6570 7468 2873   read_bitdepth(s
+00001990: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+000019a0: 2020 2020 2077 6974 6820 7365 6c66 2e63       with self.c
+000019b0: 6f6e 7472 6f6c 2829 2061 7320 633a 0a20  ontrol() as c:. 
+000019c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000019d0: 6e20 696e 7428 632e 6765 7428 2743 4f55  n int(c.get('COU
+000019e0: 4e54 4552 4445 5054 4827 2929 0a0a 2020  NTERDEPTH'))..  
+000019f0: 2020 6465 6620 6765 745f 6163 7469 7665    def get_active
+00001a00: 5f63 6f6e 7472 6f6c 6c65 7228 7365 6c66  _controller(self
+00001a10: 293a 0a20 2020 2020 2020 2066 726f 6d20  ):.        from 
+00001a20: 2e63 6f6e 7472 6f6c 6c65 7220 696d 706f  .controller impo
+00001a30: 7274 204d 6572 6c69 6e41 6374 6976 6543  rt MerlinActiveC
+00001a40: 6f6e 7472 6f6c 6c65 720a 2020 2020 2020  ontroller.      
+00001a50: 2020 7265 7475 726e 204d 6572 6c69 6e41    return MerlinA
+00001a60: 6374 6976 6543 6f6e 7472 6f6c 6c65 7228  ctiveController(
+00001a70: 290a 0a0a 636c 6173 7320 4d65 726c 696e  )...class Merlin
+00001a80: 436f 6e6e 6563 7469 6f6e 4275 696c 6465  ConnectionBuilde
+00001a90: 723a 0a20 2020 2022 2222 0a20 2020 2042  r:.    """.    B
+00001aa0: 7569 6c64 6572 2063 6c61 7373 2074 6861  uilder class tha
+00001ab0: 7420 6361 6e20 636f 6e73 7472 7563 7420  t can construct 
+00001ac0: 3a63 6c61 7373 3a60 4d65 726c 696e 4465  :class:`MerlinDe
+00001ad0: 7465 6374 6f72 436f 6e6e 6563 7469 6f6e  tectorConnection
+00001ae0: 6020 696e 7374 616e 6365 732e 0a0a 2020  ` instances...  
+00001af0: 2020 5573 6520 7468 6520 3a6d 6574 683a    Use the :meth:
+00001b00: 606f 7065 6e60 206d 6574 686f 6420 746f  `open` method to
+00001b10: 2063 7265 6174 6520 6120 636f 6e6e 6563   create a connec
+00001b20: 7469 6f6e 2e0a 2020 2020 2222 220a 2020  tion..    """.  
+00001b30: 2020 6465 6620 6f70 656e 280a 2020 2020    def open(.    
+00001b40: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00001b50: 2020 2a2c 0a20 2020 2020 2020 2061 7069    *,.        api
+00001b60: 5f68 6f73 743a 2073 7472 203d 2027 3132  _host: str = '12
+00001b70: 372e 302e 302e 3127 2c0a 2020 2020 2020  7.0.0.1',.      
+00001b80: 2020 6170 695f 706f 7274 3a20 696e 7420    api_port: int 
+00001b90: 3d20 3633 3431 2c0a 2020 2020 2020 2020  = 6341,.        
+00001ba0: 6461 7461 5f68 6f73 743a 2073 7472 203d  data_host: str =
+00001bb0: 2027 3132 372e 302e 302e 3127 2c0a 2020   '127.0.0.1',.  
+00001bc0: 2020 2020 2020 6461 7461 5f70 6f72 743a        data_port:
+00001bd0: 2069 6e74 203d 2036 3334 322c 0a20 2020   int = 6342,.   
+00001be0: 2020 2020 2064 7261 696e 3a20 626f 6f6c       drain: bool
+00001bf0: 203d 2046 616c 7365 2c0a 2020 2020 2920   = False,.    ) 
+00001c00: 2d3e 204d 6572 6c69 6e44 6574 6563 746f  -> MerlinDetecto
+00001c10: 7243 6f6e 6e65 6374 696f 6e3a 0a20 2020  rConnection:.   
+00001c20: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00001c30: 2043 6f6e 6e65 6374 2074 6f20 6120 4d65   Connect to a Me
+00001c40: 726c 696e 204d 6564 6970 6978 2064 6574  rlin Medipix det
+00001c50: 6563 746f 7220 7379 7374 656d 2e0a 0a20  ector system... 
+00001c60: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00001c70: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00001c80: 2d2d 2d2d 0a20 2020 2020 2020 2061 7069  ----.        api
+00001c90: 5f68 6f73 740a 2020 2020 2020 2020 2020  _host.          
+00001ca0: 2020 486f 7374 6e61 6d65 206f 6620 7468    Hostname of th
+00001cb0: 6520 4d65 726c 696e 2063 6f6e 7472 6f6c  e Merlin control
+00001cc0: 2073 6572 7665 722c 2064 6566 6175 6c74   server, default
+00001cd0: 2027 3132 372e 302e 302e 3127 0a20 2020   '127.0.0.1'.   
+00001ce0: 2020 2020 2020 2020 2053 686f 756c 6420           Should 
+00001cf0: 696e 206d 6f73 7420 6361 7365 7320 6265  in most cases be
+00001d00: 2074 6865 2073 616d 6520 6173 2060 6461   the same as `da
+00001d10: 7461 5f68 6f73 7460 2e0a 2020 2020 2020  ta_host`..      
+00001d20: 2020 6170 695f 706f 7274 0a20 2020 2020    api_port.     
+00001d30: 2020 2020 2020 2050 6f72 7420 6f66 2074         Port of t
+00001d40: 6865 204d 6572 6c69 6e20 636f 6e74 726f  he Merlin contro
+00001d50: 6c20 7365 7276 6572 2c20 6465 6661 756c  l server, defaul
+00001d60: 7420 3633 3431 0a20 2020 2020 2020 2064  t 6341.        d
+00001d70: 6174 615f 686f 7374 0a20 2020 2020 2020  ata_host.       
+00001d80: 2020 2020 2048 6f73 746e 616d 6520 6f66       Hostname of
+00001d90: 2074 6865 204d 6572 6c69 6e20 6461 7461   the Merlin data
+00001da0: 2073 6572 7665 722c 2064 6566 6175 6c74   server, default
+00001db0: 2027 3132 372e 302e 302e 3127 0a20 2020   '127.0.0.1'.   
+00001dc0: 2020 2020 2064 6174 615f 706f 7274 0a20       data_port. 
+00001dd0: 2020 2020 2020 2020 2020 2044 6174 6120             Data 
+00001de0: 706f 7274 206f 6620 7468 6520 4d65 726c  port of the Merl
+00001df0: 696e 2064 6174 6120 7365 7276 6572 2c20  in data server, 
+00001e00: 6465 6661 756c 7420 3633 3432 0a20 2020  default 6342.   
+00001e10: 2020 2020 2064 7261 696e 0a20 2020 2020       drain.     
+00001e20: 2020 2020 2020 2044 7261 696e 2074 6865         Drain the
+00001e30: 2073 6f63 6b65 7420 6265 666f 7265 2074   socket before t
+00001e40: 7269 6767 6572 696e 672e 2045 6e61 626c  riggering. Enabl
+00001e50: 6520 7468 6973 2077 6865 6e0a 2020 2020  e this when.    
+00001e60: 2020 2020 2020 2020 7573 696e 6720 6f6c          using ol
+00001e70: 6420 7665 7273 696f 6e73 206f 6620 7468  d versions of th
+00001e80: 6520 4d65 726c 696e 2073 6f66 7477 6172  e Merlin softwar
+00001e90: 652c 2062 7574 206e 6f74 2077 6865 6e0a  e, but not when.
+00001ea0: 2020 2020 2020 2020 2020 2020 7573 696e              usin
+00001eb0: 6720 616e 2069 6e74 6572 6e61 6c20 7472  g an internal tr
+00001ec0: 6967 6765 722e 0a0a 2020 2020 2020 2020  igger...        
+00001ed0: 4578 616d 706c 6573 0a20 2020 2020 2020  Examples.       
+00001ee0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020   --------.      
+00001ef0: 2020 5573 7561 6c6c 792c 2074 6869 7320    Usually, this 
+00001f00: 6d65 7468 6f64 2069 7320 6469 7265 6374  method is direct
+00001f10: 6c79 2075 7365 6420 746f 6765 7468 6572  ly used together
+00001f20: 2077 6974 680a 2020 2020 2020 2020 3a6d   with.        :m
+00001f30: 6574 683a 606c 6962 6572 7465 6d5f 6c69  eth:`libertem_li
+00001f40: 7665 2e61 7069 2e4c 6976 6543 6f6e 7465  ve.api.LiveConte
+00001f50: 7874 2e6d 616b 655f 636f 6e6e 6563 7469  xt.make_connecti
+00001f60: 6f6e 603a 0a0a 2020 2020 2020 2020 3e3e  on`:..        >>
+00001f70: 3e20 7769 7468 2063 7478 2e6d 616b 655f  > with ctx.make_
+00001f80: 636f 6e6e 6563 7469 6f6e 2827 6d65 726c  connection('merl
+00001f90: 696e 2729 2e6f 7065 6e28 0a20 2020 2020  in').open(.     
+00001fa0: 2020 202e 2e2e 2020 2020 2061 7069 5f68     ...     api_h
+00001fb0: 6f73 743d 2731 3237 2e30 2e30 2e31 272c  ost='127.0.0.1',
+00001fc0: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
+00001fd0: 2061 7069 5f70 6f72 743d 4d45 524c 494e   api_port=MERLIN
+00001fe0: 5f41 5049 5f50 4f52 542c 0a20 2020 2020  _API_PORT,.     
+00001ff0: 2020 202e 2e2e 2020 2020 2064 6174 615f     ...     data_
+00002000: 686f 7374 3d27 3132 372e 302e 302e 3127  host='127.0.0.1'
+00002010: 2c0a 2020 2020 2020 2020 2e2e 2e20 2020  ,.        ...   
+00002020: 2020 6461 7461 5f70 6f72 743d 4d45 524c    data_port=MERL
+00002030: 494e 5f44 4154 415f 504f 5254 2c0a 2020  IN_DATA_PORT,.  
+00002040: 2020 2020 2020 2e2e 2e20 2920 6173 2063        ... ) as c
+00002050: 6f6e 6e3a 0a20 2020 2020 2020 202e 2e2e  onn:.        ...
+00002060: 2020 2020 2061 7120 3d20 6374 782e 6d61       aq = ctx.ma
+00002070: 6b65 5f61 6371 7569 7369 7469 6f6e 2863  ke_acquisition(c
+00002080: 6f6e 6e3d 636f 6e6e 2c20 6e61 765f 7368  onn=conn, nav_sh
+00002090: 6170 653d 2833 322c 2033 3229 290a 2020  ape=(32, 32)).  
+000020a0: 2020 2020 2020 2e2e 2e20 2020 2020 6374        ...     ct
+000020b0: 782e 7275 6e5f 7564 6628 6461 7461 7365  x.run_udf(datase
+000020c0: 743d 6171 2c20 7564 663d 5375 6d55 4446  t=aq, udf=SumUDF
+000020d0: 2829 290a 2020 2020 2020 2020 7b27 696e  ()).        {'in
+000020e0: 7465 6e73 6974 7927 3a20 2e2e 2e7d 0a20  tensity': ...}. 
+000020f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00002100: 2020 2072 6574 7572 6e20 4d65 726c 696e     return Merlin
+00002110: 4465 7465 6374 6f72 436f 6e6e 6563 7469  DetectorConnecti
+00002120: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00002130: 6170 695f 686f 7374 3d61 7069 5f68 6f73  api_host=api_hos
+00002140: 742c 0a20 2020 2020 2020 2020 2020 2061  t,.            a
+00002150: 7069 5f70 6f72 743d 6170 695f 706f 7274  pi_port=api_port
+00002160: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+00002170: 7461 5f68 6f73 743d 6461 7461 5f68 6f73  ta_host=data_hos
+00002180: 742c 0a20 2020 2020 2020 2020 2020 2064  t,.            d
+00002190: 6174 615f 706f 7274 3d64 6174 615f 706f  ata_port=data_po
+000021a0: 7274 2c0a 2020 2020 2020 2020 2020 2020  rt,.            
+000021b0: 6472 6169 6e3d 6472 6169 6e2c 0a20 2020  drain=drain,.   
+000021c0: 2020 2020 2029 0a                             ).
```

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/merlin/acquisition.py` & `libertem-live-0.2.1/src/libertem_live/detectors/merlin/acquisition.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/merlin/control.py` & `libertem-live-0.2.1/src/libertem_live/detectors/merlin/control.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/merlin/data.py` & `libertem-live-0.2.1/src/libertem_live/detectors/merlin/data.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/merlin/decoders.py` & `libertem-live-0.2.1/src/libertem_live/detectors/merlin/decoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numba
 
 
-@numba.jit(cache=True)
+@numba.njit(cache=True)
 def decode_u2(inp, out):
     for y in range(out.shape[0]):
         row_out = out[y]
         row_in = inp[y]
         for i in range(row_in.shape[0] // 2):
             o0 = row_in[i * 2 + 0] << 8
             o1 = row_in[i * 2 + 1] << 0
@@ -30,15 +30,15 @@
     """
     for frame in numba.prange(num_frames):
         in_for_frame = input_bytes[frame]
         out_for_frame = out[frame]
         out_for_frame[:] = in_for_frame
 
 
-@numba.jit(cache=True)
+@numba.njit(cache=True)
 def decode_r1(inp, out):
     """
     Decode a number of 1bit raw encoded rows of input data.
     `inp` and `out` should be of shape `(num_rows, -1)`.
     This function works with non-contiguous input and output arrays.
     """
     for y in range(out.shape[0]):
@@ -49,15 +49,15 @@
             for byte in range(8):
                 inp_byte = row_in[(stripe + 1) * 8 - (byte + 1)]
                 for bitpos in range(8):
                     outpos = 64 * stripe + 8 * byte + bitpos
                     row_out[outpos] = (inp_byte >> bitpos) & 1
 
 
-@numba.jit(nogil=True, cache=True, parallel=False)
+@numba.njit(nogil=True, cache=True, parallel=False)
 def decode_multi_r1(input_bytes, out, header_size_bytes, num_frames):
     """
     input_bytes: shape (num_frames, num_rows, -1), with headers already cut off.
     """
     for frame in numba.prange(num_frames):
         in_for_frame = input_bytes[frame]
         out_for_frame = out[frame]
@@ -114,15 +114,15 @@
         for i in range(out.shape[1]):
             col = i % 8
             pos = i // 8
             out_pos = (pos + 1) * 8 - col - 1
             row_out[out_pos] = row_in[i]
 
 
-@numba.jit(nogil=True, cache=True, parallel=False)
+@numba.njit(nogil=True, cache=True, parallel=False)
 def decode_multi_r6(input_bytes, out, header_size_bytes, num_frames):
     """
     input_bytes: shape (num_frames, num_rows, -1), with headers already cut off.
     """
     for frame in numba.prange(num_frames):
         in_for_frame = input_bytes[frame]
         out_for_frame = out[frame]
@@ -182,15 +182,15 @@
         for i in range(out.shape[1]):
             col = i % 4
             pos = i // 4
             out_pos = (pos + 1) * 4 - col - 1
             row_out[out_pos] = (row_in[i * 2] << 8) + (row_in[i * 2 + 1] << 0)
 
 
-@numba.jit(nogil=True, cache=True, parallel=False)
+@numba.njit(nogil=True, cache=True, parallel=False)
 def decode_multi_r12(input_bytes, out, header_size_bytes, num_frames):
     """
     input_bytes: shape (num_frames, num_rows, -1), with headers already cut off.
     """
     for frame in numba.prange(num_frames):
         in_for_frame = input_bytes[frame]
         out_for_frame = out[frame]
```

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/merlin/sim.py` & `libertem-live-0.2.1/src/libertem_live/detectors/merlin/sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 import select
 from typing import List, Dict
 
 import click
 import numpy as np
 from tqdm import tqdm
 
+# XXX: workaround for https://github.com/numba/numba/issues/8940
+import numba.cuda  # noqa: F401
+
 from libertem.io.dataset.base import TilingScheme
 from libertem.io.dataset.mib import MIBDataSet, is_valid_hdr
 from libertem.common import Shape
 
 from libertem_live.detectors.merlin.data import AcquisitionHeader
 from libertem_live.detectors.common import (
     UndeadException, StopException, ServerThreadMixin,
@@ -639,14 +642,22 @@
 
 class TriggerClient():
     def __init__(self, host='localhost', port=6343):
         self._host = host
         self._port = port
         self._socket = None
 
+    def __enter__(self):
+        if self._socket is None:
+            self.connect()
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.close()
+
     def connect(self):
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         s.connect((self._host, self._port))
         s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         s.settimeout(1)
         self._socket = s
```

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/merlin/tango_server.py` & `libertem-live-0.2.1/src/libertem_live/detectors/merlin/tango_server.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/detectors/merlin/utils.py` & `libertem-live-0.2.1/src/libertem_live/detectors/merlin/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 @numba.njit(cache=True)
 def encode_u1(inp, out):
     for y in range(out.shape[0]):
         out[y] = inp[y]
 
 
-@numba.jit(cache=True)
+@numba.njit(cache=True)
 def encode_u2(inp, out):
     for y in range(out.shape[0]):
         row_out = out[y]
         row_in = inp[y]
         for i in range(row_in.shape[0]):
             in_value = row_in[i]
             row_out[i * 2] = (0xFF00 & in_value) >> 8
```

### Comparing `libertem-live-0.2.0/src/libertem_live/udf/monitor.py` & `libertem-live-0.2.1/src/libertem_live/udf/monitor.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live/udf/record.py` & `libertem-live-0.2.1/src/libertem_live/udf/record.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.2.0/src/libertem_live.egg-info/PKG-INFO` & `libertem-live-0.2.1/src/libertem_live.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: libertem-live
-Version: 0.2.0
+Version: 0.2.1
 Summary: Live processing with LiberTEM
 Home-page: https://libertem.github.io/LiberTEM-live
 Author: the LiberTEM team
 Author-email: libertem-dev@googlegroups.com
 License: GPL v3
 Keywords: electron microscopy
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
@@ -111,9 +110,7 @@
 We are very grateful for your continuing support for LiberTEM-live!
 
 See `the acknowledgement page
 <https://libertem.github.io/acknowledgements.html#libertem-live>`_ for a list of
 authors and contributors to LiberTEM-live and other LiberTEM projects. See also
 our info on `funding <https://libertem.github.io/#funding>`_ and `industry
 partners <https://libertem.github.io/#industry-partners>`_.
-
-
```

### Comparing `libertem-live-0.2.0/tests/test_api.py` & `libertem-live-0.2.1/tests/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 from libertem_live.api import LiveContext, Hooks
 from libertem_live.udf.monitor import SignalMonitorUDF
 
 
 def test_default_ctx():
     data = np.random.random((13, 17, 19, 23))
-    ctx = LiveContext()
-    with ctx.make_connection('memory').open(data=data) as conn:
-        aq = ctx.make_acquisition(conn=conn)
-        udf1 = NoOpUDF()
-        ctx.run_udf(dataset=aq, udf=udf1)
-        for _ in ctx.run_udf_iter(dataset=aq, udf=udf1):
-            pass
+    with LiveContext() as ctx:
+        with ctx.make_connection('memory').open(data=data) as conn:
+            aq = ctx.make_acquisition(conn=conn)
+            udf1 = NoOpUDF()
+            ctx.run_udf(dataset=aq, udf=udf1)
+            for _ in ctx.run_udf_iter(dataset=aq, udf=udf1):
+                pass
 
 
 def test_trigger(ltl_ctx):
     data = np.random.random((13, 17, 19, 23))
     triggered = np.array((False,))
 
     class MyHooks(Hooks):
```

