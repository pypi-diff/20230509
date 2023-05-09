# Comparing `tmp/gridworks_debug_cli-0.2.6.tar.gz` & `tmp/gridworks_debug_cli-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_debug_cli-0.2.6.tar", max compression
+gzip compressed data, was "gridworks_debug_cli-0.2.7.tar", max compression
```

## Comparing `gridworks_debug_cli-0.2.6.tar` & `gridworks_debug_cli-0.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-05-03 21:25:57.107139 gridworks_debug_cli-0.2.6/LICENSE
--rw-r--r--   0        0        0     4476 2023-05-03 21:25:57.107139 gridworks_debug_cli-0.2.6/README.md
--rw-r--r--   0        0        0     2375 2023-05-03 21:26:18.491045 gridworks_debug_cli-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-03 21:25:57.107139 gridworks_debug_cli-0.2.6/src/gwdcli/__init__.py
--rw-r--r--   0        0        0      467 2023-05-03 21:25:57.107139 gridworks_debug_cli-0.2.6/src/gwdcli/__main__.py
--rw-r--r--   0        0        0       63 2023-05-03 21:25:57.107139 gridworks_debug_cli-0.2.6/src/gwdcli/csv/__init__.py
--rw-r--r--   0        0        0     2880 2023-05-03 21:25:57.107139 gridworks_debug_cli-0.2.6/src/gwdcli/csv/__main__.py
--rw-r--r--   0        0        0    11313 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/csv/egauge_download.py
--rw-r--r--   0        0        0     3939 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/csv/settings.py
--rw-r--r--   0        0        0       66 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/events/__init__.py
--rw-r--r--   0        0        0     5553 2023-05-03 21:26:18.491045 gridworks_debug_cli-0.2.6/src/gwdcli/events/__main__.py
--rw-r--r--   0        0        0     9199 2023-05-03 21:26:18.491045 gridworks_debug_cli-0.2.6/src/gwdcli/events/models.py
--rw-r--r--   0        0        0     4578 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/events/mqtt.py
--rw-r--r--   0        0        0     1429 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/events/queue_loop.py
--rw-r--r--   0        0        0     3703 2023-05-03 21:26:18.491045 gridworks_debug_cli-0.2.6/src/gwdcli/events/settings.py
--rw-r--r--   0        0        0     1936 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/events/show_dir.py
--rw-r--r--   0        0        0     5768 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/events/sync.py
--rw-r--r--   0        0        0    18985 2023-05-03 21:26:18.491045 gridworks_debug_cli-0.2.6/src/gwdcli/events/tui.py
--rw-r--r--   0        0        0        0 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/py.typed
--rw-r--r--   0        0        0        0 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/utils/__init__.py
--rw-r--r--   0        0        0      509 2023-05-03 21:25:57.111139 gridworks_debug_cli-0.2.6/src/gwdcli/utils/settings.py
--rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 gridworks_debug_cli-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-09 18:47:52.036259 gridworks_debug_cli-0.2.7/LICENSE
+-rw-r--r--   0        0        0     4476 2023-05-09 18:47:52.036259 gridworks_debug_cli-0.2.7/README.md
+-rw-r--r--   0        0        0     2375 2023-05-09 18:48:07.856343 gridworks_debug_cli-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/__init__.py
+-rw-r--r--   0        0        0      467 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/__main__.py
+-rw-r--r--   0        0        0       63 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/csv/__init__.py
+-rw-r--r--   0        0        0     2880 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/csv/__main__.py
+-rw-r--r--   0        0        0    11313 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/csv/egauge_download.py
+-rw-r--r--   0        0        0     3939 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/csv/settings.py
+-rw-r--r--   0        0        0       66 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/events/__init__.py
+-rw-r--r--   0        0        0     6504 2023-05-09 18:48:07.856343 gridworks_debug_cli-0.2.7/src/gwdcli/events/__main__.py
+-rw-r--r--   0        0        0     9281 2023-05-09 18:48:07.856343 gridworks_debug_cli-0.2.7/src/gwdcli/events/models.py
+-rw-r--r--   0        0        0     4578 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/events/mqtt.py
+-rw-r--r--   0        0        0     1429 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/events/queue_loop.py
+-rw-r--r--   0        0        0     3731 2023-05-09 18:48:07.856343 gridworks_debug_cli-0.2.7/src/gwdcli/events/settings.py
+-rw-r--r--   0        0        0     1936 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/events/show_dir.py
+-rw-r--r--   0        0        0     5768 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/events/sync.py
+-rw-r--r--   0        0        0    20327 2023-05-09 18:48:07.856343 gridworks_debug_cli-0.2.7/src/gwdcli/events/tui.py
+-rw-r--r--   0        0        0        0 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/py.typed
+-rw-r--r--   0        0        0        0 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/utils/__init__.py
+-rw-r--r--   0        0        0      509 2023-05-09 18:47:52.040259 gridworks_debug_cli-0.2.7/src/gwdcli/utils/settings.py
+-rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 gridworks_debug_cli-0.2.7/PKG-INFO
```

### Comparing `gridworks_debug_cli-0.2.6/LICENSE` & `gridworks_debug_cli-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.6/README.md` & `gridworks_debug_cli-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.6/pyproject.toml` & `gridworks_debug_cli-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-debug-cli"
-version = "0.2.6"
+version = "0.2.7"
 description = "Gridworks Debug Cli"
 authors = ["Andrew Schweitzer <schweitz72@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/anschweitzer/gridworks-debug-cli"
 repository = "https://github.com/anschweitzer/gridworks-debug-cli"
 documentation = "https://gridworks-debug-cli.readthedocs.io"
```

### Comparing `gridworks_debug_cli-0.2.6/src/gwdcli/csv/__main__.py` & `gridworks_debug_cli-0.2.7/src/gwdcli/csv/__main__.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.6/src/gwdcli/csv/egauge_download.py` & `gridworks_debug_cli-0.2.7/src/gwdcli/csv/egauge_download.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.6/src/gwdcli/csv/settings.py` & `gridworks_debug_cli-0.2.7/src/gwdcli/csv/settings.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.6/src/gwdcli/events/__main__.py` & `gridworks_debug_cli-0.2.7/src/gwdcli/events/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,15 +46,16 @@
         ),
     ),
     scada: Optional[List[str]] = typer.Option(
         None,
         "--scada",
         help=(
             "Scadas whose [bold]events[/bold] to show. May be specified multiple times. If present, "
-            "an event message Src must contain one of these values to be displayed."
+            "an event message Src must contain one of these values to be displayed. "
+            "NOTE: if present, implies --read-only and --no-sync."
         ),
     ),
     clean: bool = typer.Option(  # noqa
         False, "-c", "--clean", help="Delete the entire data directory."
     ),
     no_sync: bool = typer.Option(
         False,
@@ -62,26 +63,47 @@
         help="Skip downloading data from S3. Only mqtt data will be monitored.",
     ),
     no_mqtt: bool = typer.Option(
         False,
         "--no-mqtt",
         help="Download data from S3 but do no live monitoring of mqtt.",
     ),
+    read_only: bool = typer.Option(
+        False,
+        "-r",
+        "--read-only",
+        help="Skip downloading data from S3. Monitor data from mqtt, but do not write to disk.",
+    ),
 ):
-    """Live display of incoming scada events and status"""
+    """Live display of incoming scada events and status
+
+    To show events for only one scada, run multiple windows. Run one window to download and save all events, and another
+    window for each scada you wish to show. For example, to display only events from scadas 'almond' and 'orange', each
+    in their own window, run the following commands, each in its own window:
+
+        gwd events show
+        gwd events show --scada almond
+        gwd events show --scada orange
+
+    The unfiltered window is necessary to download previous events from S3 and to save arriving events to disk.
+    """
     settings = EventsSettings.load(config_path)
     settings.verbosity += verbose
     settings.scadas += scada
     settings.snaps += snap
+    if settings.scadas:
+        read_only = True
+    if read_only:
+        no_sync = True
     if not settings.snaps:
         settings.snaps = settings.scadas[:]
     if clean:
         rich.print(f"Deleting {settings.paths.data_dir}")
         shutil.rmtree(settings.paths.data_dir)
-    run(show_main, settings, Console(), not no_sync, not no_mqtt)
+    run(show_main, settings, Console(), not no_sync, not no_mqtt, read_only)
 
 
 @app.command()
 def info(config_path: Path = Paths().config_path):  # noqa: B008
     """Print current configuration."""
 
     rich.print("")
@@ -133,14 +155,15 @@
 
 # noinspection PyUnusedLocal
 async def show_main(
     settings: EventsSettings,
     console: Console,
     do_sync: bool = True,
     do_mqtt: bool = True,
+    read_only: bool = False,
 ):
     settings.paths.mkdirs()
     logger = logging.getLogger("gwd.events")
     # if settings.paths.log_path.exists():
     #     settings.paths.log_path.unlink()
     file_handler = logging.FileHandler(settings.paths.log_path)
     file_handler.setFormatter(logging.Formatter("%(asctime)s  %(message)s"))
@@ -152,15 +175,15 @@
     logger.info(
         "\n\n+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++"
     )
     logger.info("Starting gwd events show")
     logger.info(settings.json(sort_keys=True, indent=2))
     async_queue = asyncio.Queue()
     async with create_task_group() as tg:
-        tui = TUI(settings)
+        tui = TUI(settings, read_only=read_only)
         if do_mqtt:
             tg.start_soon(run_mqtt_client, settings.mqtt, async_queue)
         if do_sync:
             tg.start_soon(sync, settings, async_queue)
         tg.start_soon(AsyncQueueLooper.loop_task, settings, async_queue, tui.queue)
         tg.start_soon(tui.tui_task)
```

### Comparing `gridworks_debug_cli-0.2.6/src/gwdcli/events/models.py` & `gridworks_debug_cli-0.2.7/src/gwdcli/events/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 from result import Result
 
 
 class AnyEvent(EventBase, extra=Extra.allow):
     TypeName: str
     _message_src: str = ""
 
+    @property
+    def message_src(self) -> str:
+        return self._message_src
+
     def other_fields(self) -> dict:
         exclude = set(EventBase.__fields__.keys())
         exclude.add("_message_src")
         return self.dict(exclude=exclude)
 
     def as_pandas_record(
         self,
```

### Comparing `gridworks_debug_cli-0.2.6/src/gwdcli/events/mqtt.py` & `gridworks_debug_cli-0.2.7/src/gwdcli/events/mqtt.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.6/src/gwdcli/events/queue_loop.py` & `gridworks_debug_cli-0.2.7/src/gwdcli/events/queue_loop.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.6/src/gwdcli/events/settings.py` & `gridworks_debug_cli-0.2.7/src/gwdcli/events/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     num_dirs_to_sync: int = 4
 
 
 class TUISettings(BaseModel):
     displayed_events: int = 45
     max_other_fields_width: int = 90
     c_to_f: bool = True
+    flush_seconds: int = 10
 
 
 class EventsSettings(BaseSettings):
     verbosity: int = 0
     snaps: list[str] = []
     scadas: list[str] = []
     paths: Paths = Paths()
```

### Comparing `gridworks_debug_cli-0.2.6/src/gwdcli/events/show_dir.py` & `gridworks_debug_cli-0.2.7/src/gwdcli/events/show_dir.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.6/src/gwdcli/events/sync.py` & `gridworks_debug_cli-0.2.7/src/gwdcli/events/sync.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.6/src/gwdcli/events/tui.py` & `gridworks_debug_cli-0.2.7/src/gwdcli/events/tui.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,30 +95,32 @@
                 )
             table.add_row(*renderables)
         return Panel(table, title="[b]Sync", border_style="blue")
 
 
 class TUI:
     settings: EventsSettings
+    read_only: bool
     df: pd.DataFrame
     live_history_df: pd.DataFrame
     display_df: pd.DataFrame
     layout: Layout
     event_table: Table
     sync_table: Table
     sync_spinners: SyncSpinners
     queue: queue.Queue
     gwd_text: Text
     local_tz: timezone
     snaps: dict[str, SnapshotSpaceheat]
     statuses: dict[str, GtShStatus]
     scadas_to_snap: list[str]
 
-    def __init__(self, settings: EventsSettings):
+    def __init__(self, settings: EventsSettings, read_only: bool):
         self.settings = settings
+        self.read_only = read_only
         if self.settings.paths.csv_path.exists():
             self.df = pd.read_csv(
                 self.settings.paths.csv_path,
                 index_col="TimeNS",
                 parse_dates=True,
                 date_parser=functools.partial(pd.to_datetime, utc=True),
             )
@@ -281,50 +283,73 @@
         for _, row in self.display_df.tail(
             self.settings.tui.displayed_events
         ).iterrows():
             i += 1
             self.add_row(row)
         return self.event_table
 
-    def handle_event(self, event: EventBase) -> None:
-        logger.debug("++handle_event")
+    def update_display(self, message_src: str, message_id: str, row_df: pd.DataFrame):
+        logger.debug("++update_display")
         path_dbg = 0
-        if event.TypeName in ["gridworks.event.problem", "gridworks.event.shutdown"]:
-            logger.info(event.json(sort_keys=True, indent=2))
-        any_event = AnyEvent(**event.dict())
-        row_df = any_event.as_dataframe(
-            columns=self.df.columns.values, interpolate_summary=True
-        )
-        display_not_full = len(self.display_df) < self.settings.tui.displayed_events
-        if not (self.display_df["MessageId"] == event.MessageId).any() and (
-            display_not_full or row_df.index[0] >= self.display_df.index[0]
+        # Check if message src is accepted
+        if not self.settings.scadas or any(
+            scada in message_src for scada in self.settings.scadas
         ):
             path_dbg |= 0x00000001
-            self.display_df = (
-                pd.concat([self.display_df, row_df])
-                .sort_index()
-                .tail(self.settings.tui.displayed_events)
-            )
-            self.layout["events"].update(self.make_event_table())
+            # Check if time is in the display window
+            if (
+                len(self.display_df) < self.settings.tui.displayed_events
+                or row_df.index[0] >= self.display_df.index[0]
+            ):
+                path_dbg |= 0x00000002
+                # Check if it is already present
+                if not (self.display_df["MessageId"] == message_id).any():
+                    path_dbg |= 0x00000004
+                    self.display_df = (
+                        pd.concat([self.display_df, row_df])
+                        .sort_index()
+                        .tail(self.settings.tui.displayed_events)
+                    )
+                    self.layout["events"].update(self.make_event_table())
+        logger.debug(f"--update_display: 0x{path_dbg:08X}")
+
+    def flush_live_history(self):
+        concatdf = pd.concat([self.df, self.live_history_df]).sort_index()
+        droppeddf = concatdf.drop_duplicates("MessageId")
+        droppeddf.to_csv(self.settings.paths.csv_path)
+        self.df = droppeddf
+        self.live_history_df = self.df.head(0)
+
+    def update_live_history(self, message_id: str, row_df: pd.DataFrame):
+        logger.debug("++update_live_history")
+        path_dbg = 0
         if (
-            not (self.live_history_df["MessageId"] == event.MessageId).any()
-            and not (self.df["MessageId"] == event.MessageId).any()
+            not self.read_only
+            and not (self.live_history_df["MessageId"] == message_id).any()
+            and not (self.df["MessageId"] == message_id).any()
         ):
-            path_dbg |= 0x00000002
+            path_dbg |= 0x00000001
             self.live_history_df = pd.concat(
                 [self.live_history_df, row_df]
             ).sort_index()
             if len(self.live_history_df) > 100:
-                path_dbg |= 0x00000004
-                concatdf = pd.concat([self.df, self.live_history_df]).sort_index()
-                droppeddf = concatdf.drop_duplicates("MessageId")
-                droppeddf.to_csv(self.settings.paths.csv_path)
-                self.df = droppeddf
-                self.live_history_df = self.df.head(0)
-        logger.debug(f"--handle_event: 0x{path_dbg:08X}")
+                path_dbg |= 0x00000002
+                self.flush_live_history()
+        logger.debug(f"--update_live_history: 0x{path_dbg:08X}")
+
+    def handle_event(self, message_src: str, event: EventBase) -> None:
+        logger.debug("++handle_event")
+        if event.TypeName in ["gridworks.event.problem", "gridworks.event.shutdown"]:
+            logger.info(event.json(sort_keys=True, indent=2))
+        row_df = AnyEvent(**event.dict()).as_dataframe(
+            columns=self.df.columns.values, interpolate_summary=True
+        )
+        self.update_display(message_src, event.MessageId, row_df)
+        self.update_live_history(event.MessageId, row_df)
+        logger.debug("--handle_event")
 
     def handle_pwr(self, pwr: GsPwr):
         pass
 
     def handle_snapshot(self, snap: SnapshotSpaceheat):
         logger.debug("++handle_snapshot")
         path_dbg = 0
@@ -434,15 +459,15 @@
                 path_dbg |= 0x00000008
                 self.handle_status(message.Payload.status)
             case SnapshotSpaceheatEvent():
                 path_dbg |= 0x00000010
                 self.handle_snapshot(message.Payload.snap)
             case EventBase():
                 path_dbg |= 0x00000020
-                self.handle_event(message.Payload)
+                self.handle_event(message.src(), message.Payload)
             case _:
                 path_dbg |= 0x00000040
         logger.debug(f"--handle_message: 0x{path_dbg:08X}")
 
     def handle_other(self, item: Any) -> None:
         pass
 
@@ -462,17 +487,23 @@
                         self.handle_other(item)
                 logger.debug(f"--check_sync_queue: 0x{path_dbg:08X}")
         except queue.Empty:
             pass
 
     def loop(self):
         with Live(self.layout, refresh_per_second=10, screen=False):
+            last_flush = time.time()
             while True:
-                time.sleep(0.1)
+                time.sleep(1)
                 self.check_sync_queue()
+                if not self.read_only and len(self.live_history_df) > 0:
+                    now = time.time()
+                    if now > last_flush + self.settings.tui.flush_seconds:
+                        self.flush_live_history()
+                        last_flush = now
 
     async def tui_task(self):
         await to_thread.run_sync(self.loop)
 
 
 class Header:
     scadas: Sequence[str]
```

### Comparing `gridworks_debug_cli-0.2.6/PKG-INFO` & `gridworks_debug_cli-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-debug-cli
-Version: 0.2.6
+Version: 0.2.7
 Summary: Gridworks Debug Cli
 Home-page: https://github.com/anschweitzer/gridworks-debug-cli
 License: MIT
 Author: Andrew Schweitzer
 Author-email: schweitz72@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

