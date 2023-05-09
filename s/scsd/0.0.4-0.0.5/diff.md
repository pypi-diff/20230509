# Comparing `tmp/scsd-0.0.4.tar.gz` & `tmp/scsd-0.0.5.tar.gz`

## Comparing `scsd-0.0.4.tar` & `scsd-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 scsd-0.0.4/Dockerfile
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scsd-0.0.4/requirements.txt
--rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 scsd-0.0.4/scsd
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scsd-0.0.4/scsd.conf.sample
--rw-r--r--   0        0        0    34178 2020-02-02 00:00:00.000000 scsd-0.0.4/test
--rw-r--r--   0        0        0    27749 2020-02-02 00:00:00.000000 scsd-0.0.4/test.html
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 scsd-0.0.4/docker/cron-root
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scsd-0.0.4/steamCloudSaveDownloader/__init__.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 scsd-0.0.4/steamCloudSaveDownloader/__main__.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 scsd-0.0.4/steamCloudSaveDownloader/args.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 scsd-0.0.4/steamCloudSaveDownloader/config.py
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 scsd-0.0.4/steamCloudSaveDownloader/db.py
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 scsd-0.0.4/steamCloudSaveDownloader/err.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 scsd-0.0.4/steamCloudSaveDownloader/logger.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 scsd-0.0.4/steamCloudSaveDownloader/notifier.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 scsd-0.0.4/steamCloudSaveDownloader/parser.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scsd-0.0.4/steamCloudSaveDownloader/storage.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 scsd-0.0.4/steamCloudSaveDownloader/web.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 scsd-0.0.4/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 scsd-0.0.4/LICENSE
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 scsd-0.0.4/README.md
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 scsd-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 scsd-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scsd-0.0.5/Dockerfile
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scsd-0.0.5/requirements.txt
+-rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 scsd-0.0.5/scsd
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scsd-0.0.5/scsd.conf.sample
+-rw-r--r--   0        0        0    34178 2020-02-02 00:00:00.000000 scsd-0.0.5/test
+-rw-r--r--   0        0        0    27749 2020-02-02 00:00:00.000000 scsd-0.0.5/test.html
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scsd-0.0.5/docker/cron-root
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/__init__.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/__main__.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/args.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/config.py
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/db.py
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/err.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/logger.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/notifier.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/parser.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/storage.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 scsd-0.0.5/steamCloudSaveDownloader/web.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 scsd-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 scsd-0.0.5/LICENSE
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 scsd-0.0.5/README.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 scsd-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 scsd-0.0.5/PKG-INFO
```

### Comparing `scsd-0.0.4/test` & `scsd-0.0.5/test`

 * *Files identical despite different names*

### Comparing `scsd-0.0.4/test.html` & `scsd-0.0.5/test.html`

 * *Files identical despite different names*

### Comparing `scsd-0.0.4/steamCloudSaveDownloader/__main__.py` & `scsd-0.0.5/steamCloudSaveDownloader/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         notifier_ = None
         parsed_args = args.args().parse(sys.argv[1:])
 
         if parsed_args['conf'] is not None:
             parsed_args = config(parsed_args['conf']).get_conf()
 
         logger.setLevel(args.args.convert_log_level(parsed_args['log_level']))
+        logger.debug(parsed_args)
 
         notifier_ = notifier.create_instance(
             parsed_args['notifier'],
             **parsed_args)
 
         main(parsed_args)
     except err as e:
```

### Comparing `scsd-0.0.4/steamCloudSaveDownloader/args.py` & `scsd-0.0.5/steamCloudSaveDownloader/args.py`

 * *Files identical despite different names*

### Comparing `scsd-0.0.4/steamCloudSaveDownloader/config.py` & `scsd-0.0.5/steamCloudSaveDownloader/config.py`

 * *Files identical despite different names*

### Comparing `scsd-0.0.4/steamCloudSaveDownloader/db.py` & `scsd-0.0.5/steamCloudSaveDownloader/db.py`

 * *Files identical despite different names*

### Comparing `scsd-0.0.4/steamCloudSaveDownloader/err.py` & `scsd-0.0.5/steamCloudSaveDownloader/err.py`

 * *Files identical despite different names*

### Comparing `scsd-0.0.4/steamCloudSaveDownloader/notifier.py` & `scsd-0.0.5/steamCloudSaveDownloader/notifier.py`

 * *Files identical despite different names*

### Comparing `scsd-0.0.4/steamCloudSaveDownloader/parser.py` & `scsd-0.0.5/steamCloudSaveDownloader/parser.py`

 * *Files identical despite different names*

### Comparing `scsd-0.0.4/steamCloudSaveDownloader/storage.py` & `scsd-0.0.5/steamCloudSaveDownloader/storage.py`

 * *Files identical despite different names*

### Comparing `scsd-0.0.4/steamCloudSaveDownloader/web.py` & `scsd-0.0.5/steamCloudSaveDownloader/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         if not g_dbg_mode:
             time.sleep(random.randint(g_random_sleep_interval[0], g_random_sleep_interval[1]))
         return func(*args, **kwargs)
     return wrapper
 
 class web:
     def __init__(self, cookie):
-        self.cookie_file = cookie.name
+        self.cookie_file = cookie
         self.cookies = MozillaCookieJar(self.cookie_file)
         try:
             self.cookies.load()
         except:
             raise err.err(err_enum.INVALID_COOKIE_FORMAT)
         self.web_parser = web_parser()
         self.session = requests.Session()
```

### Comparing `scsd-0.0.4/.gitignore` & `scsd-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `scsd-0.0.4/LICENSE` & `scsd-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scsd-0.0.4/README.md` & `scsd-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `scsd-0.0.4/pyproject.toml` & `scsd-0.0.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['hatchling', 'hatch-requirements-txt']
 build-backend = "hatchling.build"
 
 [project]
 name = "scsd"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="hchsu"}
 ]
 description = "Steam Cloud Save Downloader"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `scsd-0.0.4/PKG-INFO` & `scsd-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scsd
-Version: 0.0.4
+Version: 0.0.5
 Summary: Steam Cloud Save Downloader
 Project-URL: Homepage, https://github.com/hhhhhojeihsu/steamCloudSaveDownloader
 Project-URL: Bug Tracker, https://github.com/hhhhhojeihsu/steamCloudSaveDownloader/issues
 Author: hchsu
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

