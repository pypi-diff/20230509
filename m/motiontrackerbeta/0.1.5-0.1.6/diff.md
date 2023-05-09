# Comparing `tmp/motiontrackerbeta-0.1.5.tar.gz` & `tmp/motiontrackerbeta-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motiontrackerbeta-0.1.5.tar", max compression
+gzip compressed data, was "motiontrackerbeta-0.1.6.tar", max compression
```

## Comparing `motiontrackerbeta-0.1.5.tar` & `motiontrackerbeta-0.1.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    35823 2022-05-02 09:47:57.811283 motiontrackerbeta-0.1.5/LICENSE
--rw-r--r--   0        0        0     1647 2023-01-26 12:58:01.567762 motiontrackerbeta-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3449 2023-01-26 12:40:13.950514 motiontrackerbeta-0.1.5/README.md
--rw-r--r--   0        0        0      733 2022-08-02 18:18:06.446083 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/__init__.py
--rw-r--r--   0        0        0        0 2022-07-19 17:04:08.412955 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/classes/__init__.py
--rw-r--r--   0        0        0     4767 2023-01-15 21:48:58.203437 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/classes/classes.py
--rw-r--r--   0        0        0        0 2022-07-19 18:37:27.038039 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/functions/__init__.py
--rw-r--r--   0        0        0    24634 2023-01-15 21:40:17.078044 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/functions/differentiate.py
--rw-r--r--   0        0        0     5236 2022-07-19 18:43:41.224967 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/functions/display.py
--rw-r--r--   0        0        0     4773 2022-07-11 14:11:53.906168 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/functions/helper.py
--rw-r--r--   0        0        0     3224 2023-01-15 21:48:58.204436 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/functions/transforms.py
--rw-r--r--   0        0        0      869 2022-03-02 17:40:20.882055 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/backward.svg
--rw-r--r--   0        0        0      548 2022-03-02 17:45:28.151821 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/down.svg
--rw-r--r--   0        0        0     1822 2022-03-04 09:42:49.074276 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/dropdown.png
--rw-r--r--   0        0        0      857 2022-03-04 09:38:35.594632 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/dropdown.svg
--rw-r--r--   0        0        0     1026 2022-04-01 14:15:02.432158 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/end.svg
--rw-r--r--   0        0        0      870 2022-03-02 17:46:07.838611 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/forward.svg
--rw-r--r--   0        0        0      550 2022-03-02 17:56:00.819076 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/left.svg
--rw-r--r--   0        0        0   162817 2022-04-26 10:01:14.712223 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/loader.gif
--rw-r--r--   0        0        0   167230 2022-04-01 15:34:18.158613 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/logo.ico
--rw-r--r--   0        0        0      591 2022-03-02 20:01:32.723120 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/logo.svg
--rw-r--r--   0        0        0      540 2022-03-02 17:49:47.220928 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/pause.svg
--rw-r--r--   0        0        0      694 2022-03-02 17:51:27.272176 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/play.svg
--rw-r--r--   0        0        0      548 2022-03-02 17:52:18.616635 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/right.svg
--rw-r--r--   0        0        0     1030 2022-04-01 14:15:36.853990 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/start.svg
--rw-r--r--   0        0        0      522 2022-03-02 17:54:57.676216 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/stop.svg
--rw-r--r--   0        0        0     1860 2022-03-04 11:14:36.763200 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/tick.png
--rw-r--r--   0        0        0      550 2022-03-02 17:55:24.694566 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/up.svg
--rw-r--r--   0        0        0     1385 2021-11-12 09:48:17.339316 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/video.svg
--rw-r--r--   0        0        0     1395 2022-03-02 17:52:51.961777 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/zoom-in.svg
--rw-r--r--   0        0        0     1267 2022-03-02 17:53:38.600886 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/zoom-out.svg
--rw-r--r--   0        0        0    35823 2022-07-19 19:47:15.215230 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/LICENSE.txt
--rw-r--r--   0        0        0     1313 2022-07-19 19:29:16.180402 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/main.py
--rw-r--r--   0        0        0     1515 2022-10-11 15:32:13.684720 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/export.qss
--rw-r--r--   0        0        0     2756 2022-10-11 15:34:37.598051 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/filter-derivative.qss
--rw-r--r--   0        0        0     5204 2022-10-11 15:27:33.050603 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/main.qss
--rw-r--r--   0        0        0     1180 2022-06-13 18:46:32.847056 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/message.qss
--rw-r--r--   0        0        0     3221 2022-10-11 15:34:40.313381 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/postprocess.qss
--rw-r--r--   0        0        0     1496 2022-06-13 18:46:37.202753 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/progress.qss
--rw-r--r--   0        0        0     2562 2022-10-11 15:34:42.415962 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/rotation.qss
--rw-r--r--   0        0        0     3213 2022-06-13 18:46:27.808747 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/tracking.qss
--rw-r--r--   0        0        0        0 2022-07-19 18:35:42.336450 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/__init__.py
--rw-r--r--   0        0        0    54028 2023-01-15 22:12:56.284920 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/dialogs.py
--rw-r--r--   0        0        0     3670 2023-01-24 12:21:19.754290 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/export.py
--rw-r--r--   0        0        0    84758 2023-01-15 21:48:58.205433 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/gui.py
--rw-r--r--   0        0        0     2296 2022-07-19 18:42:47.441537 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/lists.py
--rw-r--r--   0        0        0     5615 2023-01-15 21:19:40.355990 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/process.py
--rw-r--r--   0        0        0    14261 2022-07-19 18:42:49.875419 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/trackers.py
--rw-r--r--   0        0        0     4295 2022-07-19 18:42:17.984019 motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/video.py
--rw-r--r--   0        0        0     4959 1970-01-01 00:00:00.000000 motiontrackerbeta-0.1.5/setup.py
--rw-r--r--   0        0        0     5090 1970-01-01 00:00:00.000000 motiontrackerbeta-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-05-02 09:47:57.811283 motiontrackerbeta-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1647 2023-05-09 16:46:47.396744 motiontrackerbeta-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3449 2023-01-26 12:40:13.950514 motiontrackerbeta-0.1.6/README.md
+-rw-r--r--   0        0        0      733 2022-08-02 18:18:06.446083 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-19 17:04:08.412955 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/classes/__init__.py
+-rw-r--r--   0        0        0     4767 2023-01-15 21:48:58.203437 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/classes/classes.py
+-rw-r--r--   0        0        0        0 2022-07-19 18:37:27.038039 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/functions/__init__.py
+-rw-r--r--   0        0        0    24634 2023-01-15 21:40:17.078044 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/functions/differentiate.py
+-rw-r--r--   0        0        0     5236 2022-07-19 18:43:41.224967 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/functions/display.py
+-rw-r--r--   0        0        0     4773 2022-07-11 14:11:53.906168 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/functions/helper.py
+-rw-r--r--   0        0        0     3224 2023-01-15 21:48:58.204436 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/functions/transforms.py
+-rw-r--r--   0        0        0      869 2022-03-02 17:40:20.882055 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/backward.svg
+-rw-r--r--   0        0        0      548 2022-03-02 17:45:28.151821 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/down.svg
+-rw-r--r--   0        0        0     1822 2022-03-04 09:42:49.074276 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/dropdown.png
+-rw-r--r--   0        0        0      857 2022-03-04 09:38:35.594632 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/dropdown.svg
+-rw-r--r--   0        0        0     1026 2022-04-01 14:15:02.432158 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/end.svg
+-rw-r--r--   0        0        0      870 2022-03-02 17:46:07.838611 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/forward.svg
+-rw-r--r--   0        0        0      550 2022-03-02 17:56:00.819076 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/left.svg
+-rw-r--r--   0        0        0   162817 2022-04-26 10:01:14.712223 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/loader.gif
+-rw-r--r--   0        0        0   167230 2022-04-01 15:34:18.158613 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/logo.ico
+-rw-r--r--   0        0        0      591 2022-03-02 20:01:32.723120 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/logo.svg
+-rw-r--r--   0        0        0      540 2022-03-02 17:49:47.220928 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/pause.svg
+-rw-r--r--   0        0        0      694 2022-03-02 17:51:27.272176 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/play.svg
+-rw-r--r--   0        0        0      548 2022-03-02 17:52:18.616635 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/right.svg
+-rw-r--r--   0        0        0     1030 2022-04-01 14:15:36.853990 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/start.svg
+-rw-r--r--   0        0        0      522 2022-03-02 17:54:57.676216 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/stop.svg
+-rw-r--r--   0        0        0     1860 2022-03-04 11:14:36.763200 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/tick.png
+-rw-r--r--   0        0        0      550 2022-03-02 17:55:24.694566 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/up.svg
+-rw-r--r--   0        0        0     1385 2021-11-12 09:48:17.339316 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/video.svg
+-rw-r--r--   0        0        0     1395 2022-03-02 17:52:51.961777 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/zoom-in.svg
+-rw-r--r--   0        0        0     1267 2022-03-02 17:53:38.600886 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/zoom-out.svg
+-rw-r--r--   0        0        0    35823 2022-07-19 19:47:15.215230 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/LICENSE.txt
+-rw-r--r--   0        0        0     1313 2022-07-19 19:29:16.180402 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/main.py
+-rw-r--r--   0        0        0     1515 2022-10-11 15:32:13.684720 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/export.qss
+-rw-r--r--   0        0        0     2756 2022-10-11 15:34:37.598051 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/filter-derivative.qss
+-rw-r--r--   0        0        0     5204 2022-10-11 15:27:33.050603 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/main.qss
+-rw-r--r--   0        0        0     1180 2022-06-13 18:46:32.847056 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/message.qss
+-rw-r--r--   0        0        0     3221 2022-10-11 15:34:40.313381 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/postprocess.qss
+-rw-r--r--   0        0        0     1496 2022-06-13 18:46:37.202753 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/progress.qss
+-rw-r--r--   0        0        0     2562 2022-10-11 15:34:42.415962 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/rotation.qss
+-rw-r--r--   0        0        0     3213 2022-06-13 18:46:27.808747 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/tracking.qss
+-rw-r--r--   0        0        0        0 2022-07-19 18:35:42.336450 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/__init__.py
+-rw-r--r--   0        0        0    54028 2023-05-09 16:46:48.421862 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/dialogs.py
+-rw-r--r--   0        0        0     3670 2023-05-09 16:46:49.513100 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/export.py
+-rw-r--r--   0        0        0    84790 2023-05-09 16:46:03.711091 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/gui.py
+-rw-r--r--   0        0        0     2296 2022-07-19 18:42:47.441537 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/lists.py
+-rw-r--r--   0        0        0     5615 2023-01-15 21:19:40.355990 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/process.py
+-rw-r--r--   0        0        0    14261 2022-07-19 18:42:49.875419 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/trackers.py
+-rw-r--r--   0        0        0     4295 2022-07-19 18:42:17.984019 motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/video.py
+-rw-r--r--   0        0        0     4959 1970-01-01 00:00:00.000000 motiontrackerbeta-0.1.6/setup.py
+-rw-r--r--   0        0        0     5090 1970-01-01 00:00:00.000000 motiontrackerbeta-0.1.6/PKG-INFO
```

### Comparing `motiontrackerbeta-0.1.5/LICENSE` & `motiontrackerbeta-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/pyproject.toml` & `motiontrackerbeta-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 224d 6f74 696f 6e54 7261  ame = "MotionTra
 00000020: 636b 6572 4265 7461 220d 0a76 6572 7369  ckerBeta"..versi
-00000030: 6f6e 203d 2022 302e 312e 3522 0d0a 6465  on = "0.1.5"..de
+00000030: 6f6e 203d 2022 302e 312e 3622 0d0a 6465  on = "0.1.6"..de
 00000040: 7363 7269 7074 696f 6e20 3d20 2261 2047  scription = "a G
 00000050: 5549 2062 6173 6564 2c20 6f70 656e 2d73  UI based, open-s
 00000060: 6f75 7263 6520 6d6f 7469 6f6e 2074 7261  ource motion tra
 00000070: 636b 696e 6720 6170 706c 6963 6174 696f  cking applicatio
 00000080: 6e22 0d0a 6175 7468 6f72 7320 3d20 5b22  n"..authors = ["
 00000090: 4b72 6973 746f 6620 466c 6f63 6820 3c6b  Kristof Floch <k
 000000a0: 7269 7374 6f66 2e66 6c6f 6368 4067 6d61  ristof.floch@gma
```

### Comparing `motiontrackerbeta-0.1.5/README.md` & `motiontrackerbeta-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/__init__.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/__init__.py`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/classes/classes.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/classes/classes.py`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/functions/differentiate.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/functions/differentiate.py`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/functions/display.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/functions/display.py`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/functions/helper.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/functions/helper.py`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/functions/transforms.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/functions/transforms.py`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/backward.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/backward.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/down.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/down.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/dropdown.png` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/dropdown.png`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/dropdown.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/dropdown.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/end.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/end.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/forward.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/forward.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/left.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/left.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/loader.gif` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/loader.gif`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/logo.ico` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/logo.ico`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/logo.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/logo.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/pause.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/pause.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/play.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/play.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/right.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/right.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/start.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/start.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/stop.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/stop.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/tick.png` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/tick.png`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/up.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/up.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/video.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/video.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/zoom-in.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/zoom-in.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/images/zoom-out.svg` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/images/zoom-out.svg`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/LICENSE.txt` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/main.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/main.py`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/export.qss` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/export.qss`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/filter-derivative.qss` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/filter-derivative.qss`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/main.qss` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/main.qss`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/message.qss` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/message.qss`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/postprocess.qss` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/postprocess.qss`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/progress.qss` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/progress.qss`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/rotation.qss` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/rotation.qss`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/style/tracking.qss` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/style/tracking.qss`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/dialogs.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/export.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/export.py`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/gui.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -2313,14 +2313,15 @@
             self.plotter = PlotDialog(df, title, get_unit(parameters))
             self.plotter.show()
 
         # export data
         elif parameters["out"] == "EXP":
             unit = get_unit_readable(parameters)
             cols = [f"{item} ({unit})" for item in cols]
+            cols[0]="Time (s)"
             df = pd.DataFrame(data, columns=cols)
             save_name = QFileDialog.getSaveFileName(
                 self,
                 "Save data",
                 "/",
                 "CSV file (*.csv);;Text file (*.txt);;Excel file (*.xlsx)",
             )
```

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/lists.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/lists.py`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/process.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/process.py`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/trackers.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/trackers.py`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/src/MotionTrackerBeta/widgets/video.py` & `motiontrackerbeta-0.1.6/src/MotionTrackerBeta/widgets/video.py`

 * *Files identical despite different names*

### Comparing `motiontrackerbeta-0.1.5/setup.py` & `motiontrackerbeta-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 {'console_scripts': ['MotionTrackerBeta = MotionTrackerBeta.main:MotionTracker',
                      'motiontracker = MotionTrackerBeta.main:MotionTracker',
                      'motiontrackerbeta = '
                      'MotionTrackerBeta.main:MotionTracker']}
 
 setup_kwargs = {
     'name': 'motiontrackerbeta',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'a GUI based, open-source motion tracking application',
     'long_description': '<p align="center">\n  <img src="https://user-images.githubusercontent.com/65981382/166214135-47ecd327-cba8-47c0-a034-9f6f14b777ce.png" alt="Motion Tracker Beta"/>\n</p>\n\n# Motion Tracker Beta\nAn easy-to-use, standalone and open-source motion tracking application for researchers and engineers, written in Python.\n\n## Features\n- Intutitive graphical user interface\n- Capable of handling the most common video formats\n- Capable of tracking various properties of multiple objects simultaneously\n- Diverse set of built in tracking algorithms, based on the `OpenCV` libary\n- Rich selection of numerical differentiation algorithms powered by the `PyNumDiff` libary\n- Built in plotting an exporting features\n\n\nFor the complete list of features please check the [documentation](https://github.com/flochkristof/motiontracker/blob/main/docs/GUIDE.pdf).\n\n## Dependencies\nThe Graphical user interface was created with the [PyQt5](https://www.riverbankcomputing.com/software/pyqt/) framework. For the handling of video files and to do the actual tracking the [OpenCV](https://opencv.org/) library was used with its built in tracking algorithms. Numerical differentiations are carried out using the [PyNumDiff](https://github.com/florisvb/PyNumDiff). Plots and figures are generated by [matplotlib](https://matplotlib.org/). For the complete list of required packages check [pyproject.toml](https://github.com/flochkristof/motiontracker/blob/main/pyproject.toml) or [requirements.txt](https://github.com/flochkristof/motiontracker/blob/main/requirements.txt)\n\n## Installation\n### Download & install via PyPI (recommended)\n```\n$ pip install MotionTrackerBeta\n```\n- Run the application\n```\n$ MotionTrackerBeta\n```\n### Download & install the wheel file\n- Download the `.whl` file from the latest [release](https://github.com/flochkristof/motiontracker/releases)\n- Intall with pip>\n```\n$ pip install <path-to-wheel-file.whl>\n```\n- Run the application\n```\n$ MotionTrackerBeta\n```\n\n### Download & build from source\n- Download the source from the latest [release](https://github.com/flochkristof/motiontracker/releases) or clone the repository\n```\n$ git clone https://github.com/flochkristof/motiontracker.git\n```\n- Build with [poetry](https://python-poetry.org/):\n```\n$ poetry build\n```\n- Install with pip\n```\n$ pip install dist/motiontrackerbeta-<version>-py3-none-any.whl\n```\n- Run the application\n```\n$ MotionTrackerBeta\n```\n\n### Download binaries (Windows)\n- Download the binaries from the latest release\n- Extract it to your specified location\n- Run application with `Motion Tracker Beta.exe`\n### Download the installer (Windows)\n- Download the installer from the latest release\n- Run the installer and follow the instructions\n- After successful installation the software is accessible under the name `Motion Tracker Beta`\n###\n# Usage\nFor a detailed guide about the software check out the [documentation](docs/DOCUMENTATION.pdf). A video that intorduces the main features and functions of the software is also available [online](https://www.youtube.com/watch?v=q3eWOA0FEmk).\n# License\nMotion Tracker Beta is released under the `GNU General Public License v3.0`.\n# Author\nThe software has been developed by Kristof Floch at the Department of Applied Mechanics, Faculty of Mechanical Engineering, Budapest University of Technology and Economics.\n### Contact\n- E-mail: kristof.floch@gmail.com\n',
     'author': 'Kristof Floch',
     'author_email': 'kristof.floch@gmail.com',
     'maintainer': 'Kristof Floch',
     'maintainer_email': 'kristof.floch@gmail.com',
     'url': 'https://github.com/flochkristof/motiontracker',
```

### Comparing `motiontrackerbeta-0.1.5/PKG-INFO` & `motiontrackerbeta-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motiontrackerbeta
-Version: 0.1.5
+Version: 0.1.6
 Summary: a GUI based, open-source motion tracking application
 Home-page: https://github.com/flochkristof/motiontracker
 License: GPL-3.0
 Author: Kristof Floch
 Author-email: kristof.floch@gmail.com
 Maintainer: Kristof Floch
 Maintainer-email: kristof.floch@gmail.com
```

