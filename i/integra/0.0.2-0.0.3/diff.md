# Comparing `tmp/integra-0.0.2.tar.gz` & `tmp/integra-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integra-0.0.2.tar", last modified: Tue May  9 14:48:59 2023, max compression
+gzip compressed data, was "integra-0.0.3.tar", last modified: Tue May  9 17:36:39 2023, max compression
```

## Comparing `integra-0.0.2.tar` & `integra-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 14:48:59.400924 integra-0.0.2/
--rw-rw-r--   0 pmus      (1000) pmus      (1000)     1089 2023-05-08 23:32:21.000000 integra-0.0.2/LICENSE
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      405 2023-05-09 14:48:59.400924 integra-0.0.2/PKG-INFO
--rwxrwxr-x   0 pmus      (1000) pmus      (1000)      541 2023-05-09 14:48:39.000000 integra-0.0.2/pyproject.toml
--rw-rw-r--   0 pmus      (1000) pmus      (1000)       38 2023-05-09 14:48:59.400924 integra-0.0.2/setup.cfg
-drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 14:48:59.400924 integra-0.0.2/src/
--rwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-08 23:12:48.000000 integra-0.0.2/src/__init__.py
-drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 14:48:59.400924 integra-0.0.2/src/integra.egg-info/
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      405 2023-05-09 14:48:59.000000 integra-0.0.2/src/integra.egg-info/PKG-INFO
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      193 2023-05-09 14:48:59.000000 integra-0.0.2/src/integra.egg-info/SOURCES.txt
--rw-rw-r--   0 pmus      (1000) pmus      (1000)        1 2023-05-09 14:48:59.000000 integra-0.0.2/src/integra.egg-info/dependency_links.txt
--rw-rw-r--   0 pmus      (1000) pmus      (1000)       17 2023-05-09 14:48:59.000000 integra-0.0.2/src/integra.egg-info/top_level.txt
--rwxrwxr-x   0 pmus      (1000) pmus      (1000)     9198 2023-05-09 13:07:47.000000 integra-0.0.2/src/integra.py
+drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 17:36:39.480740 integra-0.0.3/
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)     1089 2023-05-08 23:32:21.000000 integra-0.0.3/LICENSE
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)      405 2023-05-09 17:36:39.480740 integra-0.0.3/PKG-INFO
+-rwxrwxr-x   0 pmus      (1000) pmus      (1000)      541 2023-05-09 17:36:22.000000 integra-0.0.3/pyproject.toml
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)       38 2023-05-09 17:36:39.480740 integra-0.0.3/setup.cfg
+drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 17:36:39.480740 integra-0.0.3/src/
+-rwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 14:54:31.000000 integra-0.0.3/src/__init__.py
+drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 17:36:39.480740 integra-0.0.3/src/integra.egg-info/
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)      405 2023-05-09 17:36:39.000000 integra-0.0.3/src/integra.egg-info/PKG-INFO
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)      313 2023-05-09 17:36:39.000000 integra-0.0.3/src/integra.egg-info/SOURCES.txt
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)        1 2023-05-09 17:36:39.000000 integra-0.0.3/src/integra.egg-info/dependency_links.txt
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)       23 2023-05-09 17:36:39.000000 integra-0.0.3/src/integra.egg-info/top_level.txt
+-rwxrwxr-x   0 pmus      (1000) pmus      (1000)     8617 2023-05-09 17:33:34.000000 integra-0.0.3/src/integra.py
+drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 17:36:39.480740 integra-0.0.3/src/tests/
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)      823 2023-05-09 14:54:31.000000 integra-0.0.3/src/tests/bench-recv.py
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)      845 2023-05-09 14:54:31.000000 integra-0.0.3/src/tests/infinite-recv.py
+-rwxrwxr-x   0 pmus      (1000) pmus      (1000)      485 2023-05-09 14:54:31.000000 integra-0.0.3/src/tests/receive.py
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)      886 2023-05-09 14:54:31.000000 integra-0.0.3/src/tests/serve-localhost.py
+-rwxrwxr-x   0 pmus      (1000) pmus      (1000)      857 2023-05-09 17:33:30.000000 integra-0.0.3/src/tests/serve.py
```

### Comparing `integra-0.0.2/LICENSE` & `integra-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `integra-0.0.2/pyproject.toml` & `integra-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "loguru==0.7.0", "pyzmq==25.0.2", "zeroconf==0.62.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "integra"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="pmus", email="pmus.me@yandex.ru" },
 ]
 description = "ZeroMQ Zeroconf RPC"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `integra-0.0.2/src/integra.py` & `integra-0.0.3/src/integra.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import zmq, socket, time, json
+import zmq, socket, time, json, uuid
 from loguru import logger
-from uuid import uuid4
 from zeroconf import ServiceInfo, Zeroconf, ServiceBrowser, ServiceStateChange
 from functools import wraps
 from threading import Thread
 
-__version__ = "0.0.2"
 system_hostname: str = socket.gethostname()
 default_short_sleep_sec: float = 0.1
 default_poll_timeout_sec: int = 3
-default_wait_timeout: int = 10
+default_wait_timeout_sec: int = 10
 
 
 def myasync(func) -> None:
 
     @wraps(func)
     def async_func(*args, **kwargs):
         func_hl = Thread(target=func, args=args, kwargs=kwargs)
@@ -22,15 +20,15 @@
         return func_hl
 
     return async_func
 
 
 class ServiceProxy(object):
 
-    def __init__(self, integra_instance, service_name) -> None:
+    def __init__(self, integra_instance: object, service_name: str) -> None:
         self.integra_instance: Integra = integra_instance
         self.service_name: str = service_name
         self.client_update_service_data()
 
     def client_update_service_data(self):
         self.service_data: dict = self.integra_instance.dict_services[self.service_name]
         logger.info(f"Service data: {self.service_data}")
@@ -65,43 +63,41 @@
             "kwargs": kwargs,
         })
 
         self.socket.send_pyobj(request)
         recv: dict = dict()
         poller = zmq.Poller()
         poller.register(self.socket, zmq.POLLIN)
-        if poller.poll(default_poll_timeout_sec * 1000):
+        if poller.poll(default_wait_timeout_sec):
             recv, error = self.socket.recv_pyobj(), recv.get("error", None)
             if error:
                 raise error
 
         else:
-            logger.warning(f"Service {self.service_name} lost.")
+            logger.warning(f"Service {self.service_name} lost, waiting for service.")
             self.integra_instance.forget_service(self.service_name)
-            logger.info(f"Waiting for service {self.service_name}.")
             while not self.service_name in self.integra_instance.dict_services:
                 time.sleep(default_poll_timeout_sec)
             self.client_update_service_data()  # This is service recovery
         return recv["result"] if recv else None
 
 
 class Integra(object):
 
-    def __init__(self, zmq_port: int = 0, local_only=False, debug=False) -> None:
+    def __init__(self, zmq_port: int = 0, local_only=False) -> None:
         with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
-            s.settimeout(0)
-            s.connect(("10.254.254.254", 1))  # on error,
-            self.ip: str = s.getsockname()[0]  # we don't mute it.
+            s.connect(("10.254.254.254", 1))  #s.settimeout(0)
+            self.ip: str = s.getsockname()[0]  # on error, we don't mute it.
         self.run: bool = True
         self.zeroconf: Zeroconf = Zeroconf()
         self.dict_objects: dict = dict()  # What I offer
         self.dict_services: dict = dict()  # What do neighbours offer
         self.zmq_addr: str = "127.0.0.1" if local_only else "*"
         self.zmq_port = zmq_port
-        self.uuid: str = f"{uuid4()}"
+        self.uuid: str = uuid.uuid4()
         self.desc: dict = dict({"uuid": self.uuid, "services": [], "ip": self.ip})
         self.context: zmq.Context = zmq.Context()
         self.socket: zmq.Context.socket = self.context.socket(zmq.REP)
         self.browser: ServiceBrowser = ServiceBrowser(
             self.zeroconf,
             ["_http._tcp.local.", "ipc._http._tcp.local."],
             handlers=[self.on_service_state_change],
@@ -113,35 +109,21 @@
         addr: str = f"tcp://{self.zmq_addr}:*"  # Server-side ZMQ, take a free port
         self.socket.bind(addr)
         real_endpoint = self.socket.getsockopt(zmq.LAST_ENDPOINT).decode()
         logger.success(f"Integra: started. ZMQ serves at {real_endpoint}")
         self.zmq_port = int(real_endpoint.split(":")[2])
         reply: dict = dict()
         while self.run:
-            try:
-                request: object = self.socket.recv_pyobj()
-            except zmq.error.ContextTerminated:
-                break  # It *will* be terminated on exit.
-            service, attr, args, kwargs = (
-                request["service"],
-                request["attr"],
-                request["args"],
-                request["kwargs"],
-            )
-
-            try:
-                service_obj: object = self.dict_objects[service]
-            except Exception as e:
-                reply["error"] = RuntimeError(f"Error {e}: Service object {service} missing.")
-
-            service_attr = getattr(service_obj, attr, None)
-            if not service_attr:
-                reply["error"] = AttributeError(f"No attribute {attr} in {service}.")
-            res = service_attr(*args, **kwargs) if callable(service_attr) else service_attr
-            reply["result"] = res
+            request: object = self.socket.recv_pyobj()
+            service, attr, args, kwargs = (request[key] for key in ["service", "attr", "args", "kwargs"])
+            service_obj: object = self.dict_objects.get(service, None)
+            service_attr: object = getattr(service_obj, attr, None)
+            reply["error"] = RuntimeError(f"Error: Service object {service} missing.") if not service_obj else None
+            reply["error"] = AttributeError(f"No attribute {attr} in {service}.") if not service_attr else None
+            reply["result"] = service_attr(*args, **kwargs) if callable(service_attr) else service_attr
             self.socket.send_pyobj(reply)
 
     def on_service_state_change(
         self,
         zeroconf: Zeroconf,
         service_type: str,
         name: str,
@@ -161,25 +143,22 @@
                 self.dict_services[service_name] = info
 
     def forget_service(self, name) -> None:
         logger.info(f"Deleting {name} from {self.dict_services}")
         del self.dict_services[name]
 
     def service_info_to_dict(self, service_info: ServiceInfo) -> dict:
-        res: dict = {}
-        res["name"] = service_info.name
-        res["port"] = int(service_info.port)
-        res["server"] = service_info.server
+        res: dict = {key: getattr(service_info, key, None) for key in ["name", "port", "server"]}
         properties: dict = service_info.properties
         properties = dict({
             key.decode("utf-8"): value.decode("utf-8")
             for key, value in properties.items()
         })  # Properties transmitted in binary, we decode...
-        properties["services"] = json.loads(properties["services"].replace("'", '"'))
-        # This is not my fault, but zeroconf passes them this way ---------^^^
+        properties["services"] = json.loads(properties["services"].replace(
+            "'", '"'))  # Not my fault, but zeroconf passes them this way
         res.update(properties)
         return res
 
     def add_service(self, service_name: str, some_object: object) -> None:
         self.dict_objects[service_name] = some_object
         self.desc["services"].append(service_name)
         logger.info(f"Registering service '{service_name}'...")
@@ -193,24 +172,19 @@
             server=f"{system_hostname}.local.",
         )
 
         self.zeroconf.register_service(info) if not self.dict_objects else self.zeroconf.update_service(info)
         logger.success(f"Serving '{service_name}' as {self.uuid}...")
 
     def get_service_proxy(self, service_name: str) -> ServiceProxy:
-        if not service_name in self.dict_services:
-            return None
-
         service_item = self.dict_services.get(service_name, None)
-        logger.info(f"Service '{service_name}' found as {service_item}")
-        return ServiceProxy(self, service_name)
+        return ServiceProxy(self, service_name) if service_item else None
 
-    def get_service_wait(self, service_name: str, timeout: int = default_wait_timeout) -> ServiceProxy:
-        time_waited: int = 0
-        res: ServiceProxy = None
+    def get_service_wait(self, service_name: str, timeout: int = default_wait_timeout_sec) -> ServiceProxy:
+        time_waited, res = 0, None
         logger.info(f"Waiting for service {service_name}, timeout={timeout}...")
         while not res and time_waited < timeout:
             res: ServiceProxy = self.get_service_proxy(service_name)
             time.sleep(1) if not res else ...
             time_waited += 1
         if not res:
             raise RuntimeError(f"Service {service_name} not found.")
@@ -219,8 +193,8 @@
     def __setitem__(self, service_name: str, some_object: object) -> None:
         self.add_service(service_name, some_object)
 
     def __getitem__(self, service_name: str) -> ServiceProxy:
         return self.get_service_wait(service_name)
 
 
-ipc: Integra = Integra()  # You can just: from integra import ipc
+ipc: Integra = Integra()  # You can just: from integra import ipc
```

