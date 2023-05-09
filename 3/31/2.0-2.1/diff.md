# Comparing `tmp/31-2.0.tar.gz` & `tmp/31-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "31-2.0.tar", last modified: Tue Dec  6 23:57:01 2022, max compression
+gzip compressed data, was "dist/31-2.1.tar", last modified: Tue May  9 02:31:35 2023, max compression
```

## Comparing `31-2.0.tar` & `31-2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2022-12-06 23:57:01.489849 31-2.0/
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2022-12-06 23:57:01.485849 31-2.0/31.egg-info/
--rw-r--r--   0 kavi      (1000) kavi      (1000)     3643 2022-12-06 23:57:01.000000 31-2.0/31.egg-info/PKG-INFO
--rw-r--r--   0 kavi      (1000) kavi      (1000)      533 2022-12-06 23:57:01.000000 31-2.0/31.egg-info/SOURCES.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)        1 2022-12-06 23:57:01.000000 31-2.0/31.egg-info/dependency_links.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)       38 2022-12-06 23:57:01.000000 31-2.0/31.egg-info/entry_points.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)       87 2022-12-06 23:57:01.000000 31-2.0/31.egg-info/requires.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)       10 2022-12-06 23:57:01.000000 31-2.0/31.egg-info/top_level.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3643 2022-12-06 23:57:01.489849 31-2.0/PKG-INFO
--rw-r--r--   0 kavi      (1000) kavi      (1000)     2217 2020-09-05 23:47:26.000000 31-2.0/README.md
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2022-12-06 23:57:01.485849 31-2.0/s31/
--rw-r--r--   0 kavi      (1000) kavi      (1000)        0 2020-09-05 01:13:23.000000 31-2.0/s31/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      255 2022-12-06 23:56:56.000000 31-2.0/s31/active_process_table.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     1432 2021-01-25 07:31:17.000000 31-2.0/s31/command.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     1601 2020-09-06 04:49:07.000000 31-2.0/s31/config.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     1398 2020-09-06 00:06:27.000000 31-2.0/s31/foreach.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2040 2022-12-06 23:56:56.000000 31-2.0/s31/interruptable_runner.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)      957 2020-09-07 22:21:59.000000 31-2.0/s31/mail.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     8605 2022-12-06 23:56:56.000000 31-2.0/s31/main.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      840 2022-12-06 23:56:56.000000 31-2.0/s31/notify.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1549 2022-12-06 23:56:56.000000 31-2.0/s31/process_manager.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)      660 2021-03-14 22:38:25.000000 31-2.0/s31/screen.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)      824 2020-09-14 09:05:43.000000 31-2.0/s31/utils.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     1213 2020-09-14 09:05:43.000000 31-2.0/s31/workers.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       38 2022-12-06 23:57:01.489849 31-2.0/setup.cfg
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1029 2022-12-06 23:56:56.000000 31-2.0/setup.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2022-12-06 23:57:01.485849 31-2.0/tests/
--rw-r--r--   0 kavi      (1000) kavi      (1000)        0 2020-09-05 01:15:11.000000 31-2.0/tests/__init__.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     2090 2020-09-05 20:36:59.000000 31-2.0/tests/basic_test.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)      478 2020-09-14 22:43:31.000000 31-2.0/tests/buf_test.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     4502 2020-09-06 03:23:32.000000 31-2.0/tests/foreach_test.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     1954 2020-09-14 07:36:14.000000 31-2.0/tests/options_test.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)      871 2020-09-14 22:56:33.000000 31-2.0/tests/test31.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     3840 2020-09-14 23:02:33.000000 31-2.0/tests/workers_test.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-05-09 02:31:35.000000 31-2.1/
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-05-09 02:31:35.000000 31-2.1/31.egg-info/
+-rw-r--r--   0 kavi      (1000) kavi      (1000)     3643 2023-05-09 02:31:34.000000 31-2.1/31.egg-info/PKG-INFO
+-rw-r--r--   0 kavi      (1000) kavi      (1000)      533 2023-05-09 02:31:34.000000 31-2.1/31.egg-info/SOURCES.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        1 2023-05-09 02:31:34.000000 31-2.1/31.egg-info/dependency_links.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       38 2023-05-09 02:31:34.000000 31-2.1/31.egg-info/entry_points.txt
+-rw-r--r--   0 kavi      (1000) kavi      (1000)       87 2023-05-09 02:31:34.000000 31-2.1/31.egg-info/requires.txt
+-rw-r--r--   0 kavi      (1000) kavi      (1000)       10 2023-05-09 02:31:34.000000 31-2.1/31.egg-info/top_level.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3643 2023-05-09 02:31:35.000000 31-2.1/PKG-INFO
+-rw-r--r--   0 kavi      (1000) kavi      (1000)     2217 2020-09-05 23:47:26.000000 31-2.1/README.md
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-05-09 02:31:35.000000 31-2.1/s31/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2020-09-05 01:13:23.000000 31-2.1/s31/__init__.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)      255 2022-12-06 23:56:56.000000 31-2.1/s31/active_process_table.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1432 2021-01-25 07:31:17.000000 31-2.1/s31/command.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)     1601 2020-09-06 04:49:07.000000 31-2.1/s31/config.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)     1398 2020-09-06 00:06:27.000000 31-2.1/s31/foreach.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)     2040 2022-12-06 23:56:56.000000 31-2.1/s31/interruptable_runner.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      957 2020-09-07 22:21:59.000000 31-2.1/s31/mail.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     8974 2023-05-09 02:31:30.000000 31-2.1/s31/main.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)      840 2022-12-06 23:56:56.000000 31-2.1/s31/notify.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1910 2023-05-09 02:31:30.000000 31-2.1/s31/process_manager.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)      660 2021-03-14 22:38:25.000000 31-2.1/s31/screen.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)      824 2020-09-14 09:05:43.000000 31-2.1/s31/utils.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1213 2020-09-14 09:05:43.000000 31-2.1/s31/workers.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       38 2023-05-09 02:31:35.000000 31-2.1/setup.cfg
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1029 2023-05-09 02:31:30.000000 31-2.1/setup.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-05-09 02:31:35.000000 31-2.1/tests/
+-rw-r--r--   0 kavi      (1000) kavi      (1000)        0 2020-09-05 01:15:11.000000 31-2.1/tests/__init__.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)     2090 2020-09-05 20:36:59.000000 31-2.1/tests/basic_test.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)      478 2020-09-14 22:43:31.000000 31-2.1/tests/buf_test.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)     4502 2020-09-06 03:23:32.000000 31-2.1/tests/foreach_test.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)     1954 2020-09-14 07:36:14.000000 31-2.1/tests/options_test.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)      871 2020-09-14 22:56:33.000000 31-2.1/tests/test31.py
+-rw-r--r--   0 kavi      (1000) kavi      (1000)     3840 2020-09-14 23:02:33.000000 31-2.1/tests/workers_test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `31-2.0/31.egg-info/PKG-INFO` & `31-2.1/31.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 31
-Version: 2.0
+Version: 2.1
 Summary: Runs code in a specified environment in the background and notifies you when it is done.
 Home-page: https://github.com/kavigupta/31
 Author: Kavi Gupta
 Author-email: 31@kavigupta.org
 License: UNKNOWN
 Description: 
         # 31
```

### Comparing `31-2.0/31.egg-info/SOURCES.txt` & `31-2.1/31.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `31-2.0/PKG-INFO` & `31-2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 31
-Version: 2.0
+Version: 2.1
 Summary: Runs code in a specified environment in the background and notifies you when it is done.
 Home-page: https://github.com/kavigupta/31
 Author: Kavi Gupta
 Author-email: 31@kavigupta.org
 License: UNKNOWN
 Description: 
         # 31
```

### Comparing `31-2.0/README.md` & `31-2.1/README.md`

 * *Files identical despite different names*

### Comparing `31-2.0/s31/command.py` & `31-2.1/s31/command.py`

 * *Files identical despite different names*

### Comparing `31-2.0/s31/config.py` & `31-2.1/s31/config.py`

 * *Files identical despite different names*

### Comparing `31-2.0/s31/foreach.py` & `31-2.1/s31/foreach.py`

 * *Files identical despite different names*

### Comparing `31-2.0/s31/interruptable_runner.py` & `31-2.1/s31/interruptable_runner.py`

 * *Files identical despite different names*

### Comparing `31-2.0/s31/mail.py` & `31-2.1/s31/mail.py`

 * *Files identical despite different names*

### Comparing `31-2.0/s31/main.py` & `31-2.1/s31/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -117,25 +117,36 @@
     config_parser.add_argument("key", help="The configuration key to modify")
     config_parser.add_argument("value", help="The value to assign the given key to")
     config_parser.set_defaults(action=config_action)
 
     list_parser = subparsers.add_parser("list", help="List all commands", aliases=["l"])
     config_argument(list_parser)
     list_parser.add_argument(
+        "prefix",
+        help="Only list commands whose names start with the given prefix",
+        nargs="?",
+    )
+    list_parser.add_argument(
         "-o",
         "--ordering",
         help="The ordering to use",
         choices=["timestamp", "name"],
         default="timestamp",
     )
     list_parser.set_defaults(action=list_action)
 
     stop_parser = subparsers.add_parser("stop", help="Stop a command", aliases=["s"])
     config_argument(stop_parser)
     stop_parser.add_argument("name", help="The name of the command to stop")
+    stop_parser.add_argument(
+        "-m",
+        "--multi",
+        help="Stop all commands with the given prefix, even if there are multiple or it isn't the full name",
+        action="store_true",
+    )
     stop_parser.set_defaults(action=stop_action)
 
     args = parser.parse_args()
 
     try:
         args.action(args)
     except RuntimeError as e:
@@ -233,12 +244,12 @@
 
 
 def config_action(args):
     update_config(args.config_file, {args.key: args.value})
 
 
 def list_action(args):
-    list_procesess(args.ordering)
+    list_procesess(args.prefix, args.ordering)
 
 
 def stop_action(args):
     stop_process(args.name)
```

### Comparing `31-2.0/s31/notify.py` & `31-2.1/s31/notify.py`

 * *Files identical despite different names*

### Comparing `31-2.0/s31/screen.py` & `31-2.1/s31/screen.py`

 * *Files identical despite different names*

### Comparing `31-2.0/s31/utils.py` & `31-2.1/s31/utils.py`

 * *Files identical despite different names*

### Comparing `31-2.0/s31/workers.py` & `31-2.1/s31/workers.py`

 * *Files identical despite different names*

### Comparing `31-2.0/setup.py` & `31-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="31",
-    version="2.0",
+    version="2.1",
     author="Kavi Gupta",
     author_email="31@kavigupta.org",
     description="Runs code in a specified environment in the background and notifies you when it is done.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kavigupta/31",
     packages=setuptools.find_packages(),
```

### Comparing `31-2.0/tests/basic_test.py` & `31-2.1/tests/basic_test.py`

 * *Files identical despite different names*

### Comparing `31-2.0/tests/foreach_test.py` & `31-2.1/tests/foreach_test.py`

 * *Files identical despite different names*

### Comparing `31-2.0/tests/options_test.py` & `31-2.1/tests/options_test.py`

 * *Files identical despite different names*

### Comparing `31-2.0/tests/test31.py` & `31-2.1/tests/test31.py`

 * *Files identical despite different names*

### Comparing `31-2.0/tests/workers_test.py` & `31-2.1/tests/workers_test.py`

 * *Files identical despite different names*

