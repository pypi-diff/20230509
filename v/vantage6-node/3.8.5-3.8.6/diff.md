# Comparing `tmp/vantage6-node-3.8.5.tar.gz` & `tmp/vantage6-node-3.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-node-3.8.5.tar", last modified: Tue May  2 14:03:45 2023, max compression
+gzip compressed data, was "vantage6-node-3.8.6.tar", last modified: Tue May  9 07:46:12 2023, max compression
```

## Comparing `vantage6-node-3.8.5.tar` & `vantage6-node-3.8.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:45.735731 vantage6-node-3.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-02 14:03:45.735731 vantage6-node-3.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:03:45.735731 vantage6-node-3.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:45.727731 vantage6-node-3.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/tests/test_ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:45.727731 vantage6-node-3.8.5/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:45.731731 vantage6-node-3.8.5/vantage6/node/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    38328 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:45.731731 vantage6-node-3.8.5/vantage6/node/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/cli/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:45.735731 vantage6-node-3.8.5/vantage6/node/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/docker/docker_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/docker/docker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/docker/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17490 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/docker/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/docker/vpn_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/proxy_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/server_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:45.735731 vantage6-node-3.8.5/vantage6/node/util/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-02 14:03:31.000000 vantage6-node-3.8.5/vantage6/node/util/colorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:45.735731 vantage6-node-3.8.5/vantage6_node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-02 14:03:45.000000 vantage6-node-3.8.5/vantage6_node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-02 14:03:45.000000 vantage6-node-3.8.5/vantage6_node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:03:45.000000 vantage6-node-3.8.5/vantage6_node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-02 14:03:45.000000 vantage6-node-3.8.5/vantage6_node.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-02 14:03:45.000000 vantage6-node-3.8.5/vantage6_node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 14:03:45.000000 vantage6-node-3.8.5/vantage6_node.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:46:12.323949 vantage6-node-3.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-09 07:46:12.323949 vantage6-node-3.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 07:46:12.323949 vantage6-node-3.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:46:12.319949 vantage6-node-3.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/tests/test_ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:46:12.319949 vantage6-node-3.8.6/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:46:12.319949 vantage6-node-3.8.6/vantage6/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    39820 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:46:12.319949 vantage6-node-3.8.6/vantage6/node/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/cli/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:46:12.323949 vantage6-node-3.8.6/vantage6/node/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/docker/docker_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/docker/docker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/docker/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/docker/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/docker/vpn_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/proxy_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/server_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:46:12.323949 vantage6-node-3.8.6/vantage6/node/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-09 07:45:57.000000 vantage6-node-3.8.6/vantage6/node/util/colorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:46:12.323949 vantage6-node-3.8.6/vantage6_node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-09 07:46:12.000000 vantage6-node-3.8.6/vantage6_node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-09 07:46:12.000000 vantage6-node-3.8.6/vantage6_node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:46:12.000000 vantage6-node-3.8.6/vantage6_node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-09 07:46:12.000000 vantage6-node-3.8.6/vantage6_node.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-09 07:46:12.000000 vantage6-node-3.8.6/vantage6_node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 07:46:12.000000 vantage6-node-3.8.6/vantage6_node.egg-info/top_level.txt
```

### Comparing `vantage6-node-3.8.5/PKG-INFO` & `vantage6-node-3.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 3.8.5
+Version: 3.8.6
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.5 Summary: vantage6 node
+Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.6 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-node-3.8.5/setup.py` & `vantage6-node-3.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6/node/__init__.py` & `vantage6-node-3.8.6/vantage6/node/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,20 +242,64 @@
                 self.log.error(e)
 
     def sync_task_queue_with_server(self) -> None:
         """ Get all unprocessed tasks from the server for this node."""
         assert self.server_io.cryptor, "Encrpytion has not been setup"
 
         # request open tasks from the server
-        tasks = self.server_io.get_results(state="open", include_task=True)
-        self.log.debug(tasks)
-        for task in tasks:
-            self.queue.put(task)
+        task_results = self.server_io.get_results(state="open",
+                                                  include_task=True)
+        self.log.debug(task_results)
+
+        # add the tasks to the queue
+        self.__add_tasks_to_queue(task_results)
+        self.log.info(f"Received {self.queue._qsize()} tasks")
 
-        self.log.info(f"received {self.queue._qsize()} tasks")
+    def get_task_and_add_to_queue(self, task_id: int) -> None:
+        """
+        Fetches (open) task with task_id from the server. The `task_id` is
+        delivered by the websocket-connection.
+
+        Parameters
+        ----------
+        task_id : int
+            Task identifier
+        """
+        # fetch (open) result for the node with the task_id
+        task_results = self.server_io.get_results(
+            include_task=True,
+            state='open',
+            task_id=task_id
+        )
+
+        # add the tasks to the queue
+        self.__add_tasks_to_queue(task_results)
+
+    def __add_tasks_to_queue(self, task_results: list[dict]) -> None:
+        """
+        Add a task to the queue.
+
+        Parameters
+        ----------
+        taskresult : list[dict]
+            A list of dictionaries with information required to run the
+            algorithm
+        """
+        for task_result in task_results:
+            try:
+                if not self.__docker.is_running(task_result['id']):
+                    self.queue.put(task_result)
+                else:
+                    self.log.info(
+                        f"Not starting task {task_result['task']['id']} - "
+                        f"{task_result['task']['name']} as it is already "
+                        "running"
+                    )
+            except Exception:
+                self.log.exception("Error while syncing task queue")
 
     def __start_task(self, taskresult: dict) -> None:
         """
         Start the docker image and notify the server that the task has been
         started.
 
         Parameters
@@ -304,14 +348,28 @@
             # set finished_at to now, so that the task is not picked up again
             # (as the task is not started at all, unlike other crashes, it will
             # never finish and hence not be set to finished)
             update['finished_at'] = datetime.datetime.now().isoformat()
         self.server_io.patch_results(
             id=taskresult['id'], result=update
         )
+
+        # ensure that the /tasks namespace is connected. This may take a while
+        # (usually < 5s) when the socket just (re)connected
+        MAX_ATTEMPTS = 30
+        retries = 0
+        while '/tasks' not in self.socketIO.namespaces and \
+                retries < MAX_ATTEMPTS:
+            retries += 1
+            self.log.debug('Waiting for /tasks namespace to connect...')
+            time.sleep(1)
+        self.log.debug('Connected to /tasks namespace')
+        # in case the namespace is still not connected, the socket notification
+        # will not be sent to other nodes, but the task will still be processed
+
         # send socket event to alert everyone of task status change
         self.socketIO.emit(
             'algorithm_status_change',
             data={
                 'node_id': self.server_io.whoami.id_,
                 'status': task_status,
                 'result_id': taskresult['id'],
@@ -814,48 +872,26 @@
             try:
                 self.socketIO.emit('ping', namespace='/tasks')
             except Exception:
                 self.log.exception('Ping thread had an exception')
             # Wait before sending next ping
             time.sleep(PING_INTERVAL_SECONDS)
 
-    def get_task_and_add_to_queue(self, task_id: int) -> None:
-        """
-        Fetches (open) task with task_id from the server. The `task_id` is
-        delivered by the websocket-connection.
-
-        Parameters
-        ----------
-        task_id : int
-            Task identifier
-        """
-        # fetch (open) result for the node with the task_id
-        tasks = self.server_io.get_results(
-            include_task=True,
-            state='open',
-            task_id=task_id
-        )
-
-        # in the current setup, only a single result for a single node
-        # in a task exists.
-        for task in tasks:
-            self.queue.put(task)
-
     def run_forever(self) -> None:
         """Keep checking queue for incoming tasks (and execute them)."""
         kill_listener = ContainerKillListener()
         try:
             while True:
                 # blocking untill a task comes available
                 # timeout specified, else Keyboard interupts are ignored
                 self.log.info("Waiting for new tasks....")
 
                 while not kill_listener.kill_now:
                     try:
-                        task = self.queue.get(timeout=1)
+                        taskresult = self.queue.get(timeout=1)
                         # if no item is returned, the Empty exception is
                         # triggered, thus break statement is not reached
                         break
 
                     except queue.Empty:
                         pass
 
@@ -863,15 +899,15 @@
                         self.log.debug(e)
 
                 if kill_listener.kill_now:
                     raise InterruptedError
 
                 # if task comes available, attempt to execute it
                 try:
-                    self.__start_task(task)
+                    self.__start_task(taskresult)
                 except Exception as e:
                     self.log.exception(e)
 
         except (KeyboardInterrupt, InterruptedError):
             self.log.info("Vnode is interrupted, shutting down...")
             self.cleanup()
             sys.exit()
```

### Comparing `vantage6-node-3.8.5/vantage6/node/_version.py` & `vantage6-node-3.8.6/vantage6/node/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, '__build__')) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = ((( 3, 8, 5, 'final', __build__, 0)))
+version_info = ((( 3, 8, 6, 'final', __build__, 0)))
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
 pre_release = f'' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
 post_release = f'' if not version_info[5] else f'.post{version_info[5]}'
```

### Comparing `vantage6-node-3.8.5/vantage6/node/cli/node.py` & `vantage6-node-3.8.6/vantage6/node/cli/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6/node/context.py` & `vantage6-node-3.8.6/vantage6/node/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6/node/docker/docker_base.py` & `vantage6-node-3.8.6/vantage6/node/docker/docker_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6/node/docker/docker_manager.py` & `vantage6-node-3.8.6/vantage6/node/docker/docker_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6/node/docker/exceptions.py` & `vantage6-node-3.8.6/vantage6/node/docker/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6/node/docker/ssh_tunnel.py` & `vantage6-node-3.8.6/vantage6/node/docker/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6/node/docker/task_manager.py` & `vantage6-node-3.8.6/vantage6/node/docker/task_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         self.docker_input = None
 
         self.labels = {
             f"{APPNAME}-type": "algorithm",
             "node": node_name,
             "result_id": str(result_id)
         }
-        self.helper_labels = self.labels
+        self.helper_labels = self.labels.copy()
         self.helper_labels[f"{APPNAME}-type"] = "algorithm-helper"
 
         # FIXME: these values should be retrieved from DockerNodeContext
         #   in some way.
         self.tmp_folder = "/mnt/tmp"
         self.data_folder = "/mnt/data"
```

### Comparing `vantage6-node-3.8.5/vantage6/node/docker/vpn_manager.py` & `vantage6-node-3.8.6/vantage6/node/docker/vpn_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6/node/globals.py` & `vantage6-node-3.8.6/vantage6/node/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6/node/proxy_server.py` & `vantage6-node-3.8.6/vantage6/node/proxy_server.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6/node/server_io.py` & `vantage6-node-3.8.6/vantage6/node/server_io.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6/node/socket.py` & `vantage6-node-3.8.6/vantage6/node/socket.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6/node/util/__init__.py` & `vantage6-node-3.8.6/vantage6/node/util/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6/node/util/colorer.py` & `vantage6-node-3.8.6/vantage6/node/util/colorer.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.5/vantage6_node.egg-info/PKG-INFO` & `vantage6-node-3.8.6/vantage6_node.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 3.8.5
+Version: 3.8.6
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.5 Summary: vantage6 node
+Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.6 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-node-3.8.5/vantage6_node.egg-info/SOURCES.txt` & `vantage6-node-3.8.6/vantage6_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

