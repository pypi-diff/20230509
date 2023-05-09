# Comparing `tmp/gridworks_debug_cli-0.2.7.tar.gz` & `tmp/gridworks_debug_cli-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_debug_cli-0.2.7.tar", max compression
+gzip compressed data, was "gridworks_debug_cli-0.2.8.tar", max compression
```

## Comparing `gridworks_debug_cli-0.2.7.tar` & `gridworks_debug_cli-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-05-09 18:47:52.036259 gridworks_debug_cli-0.2.7/LICENSE
--rw-r--r--   0        0        0     4476 2023-05-09 18:47:52.036259 gridworks_debug_cli-0.2.7/README.md
--rw-r--r--   0        0        0     2375 2023-05-09 18:48:07.856343 gridworks_debug_cli-0.2.7/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/__init__.py
--rw-r--r--   0        0        0      467 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/__main__.py
--rw-r--r--   0        0        0       63 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/csv/__init__.py
--rw-r--r--   0        0        0     2880 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/csv/__main__.py
--rw-r--r--   0        0        0    11313 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/csv/egauge_download.py
--rw-r--r--   0        0        0     3939 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/csv/settings.py
--rw-r--r--   0        0        0       66 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/events/__init__.py
--rw-r--r--   0        0        0     6504 2023-05-09 18:48:07.856343 gridworks_debug_cli-0.2.7/src/gwdcli/events/__main__.py
--rw-r--r--   0        0        0     9281 2023-05-09 18:48:07.856343 gridworks_debug_cli-0.2.7/src/gwdcli/events/models.py
--rw-r--r--   0        0        0     4578 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/events/mqtt.py
--rw-r--r--   0        0        0     1429 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/events/queue_loop.py
--rw-r--r--   0        0        0     3731 2023-05-09 18:48:07.856343 gridworks_debug_cli-0.2.7/src/gwdcli/events/settings.py
--rw-r--r--   0        0        0     1936 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/events/show_dir.py
--rw-r--r--   0        0        0     5768 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/events/sync.py
--rw-r--r--   0        0        0    20327 2023-05-09 18:48:07.856343 gridworks_debug_cli-0.2.7/src/gwdcli/events/tui.py
--rw-r--r--   0        0        0        0 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/py.typed
--rw-r--r--   0        0        0        0 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/utils/__init__.py
--rw-r--r--   0        0        0      509 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/utils/settings.py
--rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 gridworks_debug_cli-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-09 19:31:30.050498 gridworks_debug_cli-0.2.8/LICENSE
+-rw-r--r--   0        0        0     4476 2023-05-09 19:31:30.050498 gridworks_debug_cli-0.2.8/README.md
+-rw-r--r--   0        0        0     2375 2023-05-09 19:31:48.446355 gridworks_debug_cli-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/__init__.py
+-rw-r--r--   0        0        0      467 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/__main__.py
+-rw-r--r--   0        0        0       63 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/csv/__init__.py
+-rw-r--r--   0        0        0     2880 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/csv/__main__.py
+-rw-r--r--   0        0        0    11313 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/csv/egauge_download.py
+-rw-r--r--   0        0        0     3939 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/csv/settings.py
+-rw-r--r--   0        0        0       66 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/events/__init__.py
+-rw-r--r--   0        0        0     6808 2023-05-09 19:31:48.446355 gridworks_debug_cli-0.2.8/src/gwdcli/events/__main__.py
+-rw-r--r--   0        0        0     9281 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/events/models.py
+-rw-r--r--   0        0        0     4578 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/events/mqtt.py
+-rw-r--r--   0        0        0     1429 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/events/queue_loop.py
+-rw-r--r--   0        0        0     3763 2023-05-09 19:31:48.450355 gridworks_debug_cli-0.2.8/src/gwdcli/events/settings.py
+-rw-r--r--   0        0        0     1936 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/events/show_dir.py
+-rw-r--r--   0        0        0     5768 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/events/sync.py
+-rw-r--r--   0        0        0    20408 2023-05-09 19:31:48.450355 gridworks_debug_cli-0.2.8/src/gwdcli/events/tui.py
+-rw-r--r--   0        0        0        0 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/py.typed
+-rw-r--r--   0        0        0        0 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/utils/__init__.py
+-rw-r--r--   0        0        0      509 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/utils/settings.py
+-rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 gridworks_debug_cli-0.2.8/PKG-INFO
```

### Comparing `gridworks_debug_cli-0.2.7/LICENSE` & `gridworks_debug_cli-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.7/README.md` & `gridworks_debug_cli-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.7/pyproject.toml` & `gridworks_debug_cli-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-debug-cli"
-version = "0.2.7"
+version = "0.2.8"
 description = "Gridworks Debug Cli"
 authors = ["Andrew Schweitzer <schweitz72@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/anschweitzer/gridworks-debug-cli"
 repository = "https://github.com/anschweitzer/gridworks-debug-cli"
 documentation = "https://gridworks-debug-cli.readthedocs.io"
```

### Comparing `gridworks_debug_cli-0.2.7/src/gwdcli/csv/__main__.py` & `gridworks_debug_cli-0.2.8/src/gwdcli/csv/__main__.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.7/src/gwdcli/csv/egauge_download.py` & `gridworks_debug_cli-0.2.8/src/gwdcli/csv/egauge_download.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.7/src/gwdcli/csv/settings.py` & `gridworks_debug_cli-0.2.8/src/gwdcli/csv/settings.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.7/src/gwdcli/events/__main__.py` & `gridworks_debug_cli-0.2.8/src/gwdcli/events/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,18 @@
     ),
     read_only: bool = typer.Option(
         False,
         "-r",
         "--read-only",
         help="Skip downloading data from S3. Monitor data from mqtt, but do not write to disk.",
     ),
+    updates_per_second: Optional[int] = typer.Option(
+        None,
+        help="Screen updates per second. Higher rates may cause flickering on some terminals.",
+    ),
 ):
     """Live display of incoming scada events and status
 
     To show events for only one scada, run multiple windows. Run one window to download and save all events, and another
     window for each scada you wish to show. For example, to display only events from scadas 'almond' and 'orange', each
     in their own window, run the following commands, each in its own window:
 
@@ -95,14 +99,16 @@
     if read_only:
         no_sync = True
     if not settings.snaps:
         settings.snaps = settings.scadas[:]
     if clean:
         rich.print(f"Deleting {settings.paths.data_dir}")
         shutil.rmtree(settings.paths.data_dir)
+    if updates_per_second is not None:
+        settings.tui.updates_per_second = updates_per_second
     run(show_main, settings, Console(), not no_sync, not no_mqtt, read_only)
 
 
 @app.command()
 def info(config_path: Path = Paths().config_path):  # noqa: B008
     """Print current configuration."""
 
@@ -156,14 +162,15 @@
 # noinspection PyUnusedLocal
 async def show_main(
     settings: EventsSettings,
     console: Console,
     do_sync: bool = True,
     do_mqtt: bool = True,
     read_only: bool = False,
+    updates_per_second: int = 1,
 ):
     settings.paths.mkdirs()
     logger = logging.getLogger("gwd.events")
     # if settings.paths.log_path.exists():
     #     settings.paths.log_path.unlink()
     file_handler = logging.FileHandler(settings.paths.log_path)
     file_handler.setFormatter(logging.Formatter("%(asctime)s  %(message)s"))
```

### Comparing `gridworks_debug_cli-0.2.7/src/gwdcli/events/models.py` & `gridworks_debug_cli-0.2.8/src/gwdcli/events/models.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.7/src/gwdcli/events/mqtt.py` & `gridworks_debug_cli-0.2.8/src/gwdcli/events/mqtt.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.7/src/gwdcli/events/queue_loop.py` & `gridworks_debug_cli-0.2.8/src/gwdcli/events/queue_loop.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.7/src/gwdcli/events/settings.py` & `gridworks_debug_cli-0.2.8/src/gwdcli/events/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 
 
 class TUISettings(BaseModel):
     displayed_events: int = 45
     max_other_fields_width: int = 90
     c_to_f: bool = True
     flush_seconds: int = 10
+    updates_per_second: int = 2
 
 
 class EventsSettings(BaseSettings):
     verbosity: int = 0
     snaps: list[str] = []
     scadas: list[str] = []
     paths: Paths = Paths()
```

### Comparing `gridworks_debug_cli-0.2.7/src/gwdcli/events/show_dir.py` & `gridworks_debug_cli-0.2.8/src/gwdcli/events/show_dir.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.7/src/gwdcli/events/sync.py` & `gridworks_debug_cli-0.2.8/src/gwdcli/events/sync.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.7/src/gwdcli/events/tui.py` & `gridworks_debug_cli-0.2.8/src/gwdcli/events/tui.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,15 +486,19 @@
                         path_dbg |= 0x00000020
                         self.handle_other(item)
                 logger.debug(f"--check_sync_queue: 0x{path_dbg:08X}")
         except queue.Empty:
             pass
 
     def loop(self):
-        with Live(self.layout, refresh_per_second=10, screen=False):
+        with Live(
+            self.layout,
+            refresh_per_second=self.settings.tui.updates_per_second,
+            screen=False,
+        ):
             last_flush = time.time()
             while True:
                 time.sleep(1)
                 self.check_sync_queue()
                 if not self.read_only and len(self.live_history_df) > 0:
                     now = time.time()
                     if now > last_flush + self.settings.tui.flush_seconds:
```

### Comparing `gridworks_debug_cli-0.2.7/PKG-INFO` & `gridworks_debug_cli-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-debug-cli
-Version: 0.2.7
+Version: 0.2.8
 Summary: Gridworks Debug Cli
 Home-page: https://github.com/anschweitzer/gridworks-debug-cli
 License: MIT
 Author: Andrew Schweitzer
 Author-email: schweitz72@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

