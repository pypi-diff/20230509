# Comparing `tmp/sr.robot3-2023.0.5.tar.gz` & `tmp/sr_robot3-2023.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sr.robot3-2023.0.5.tar", max compression
+gzip compressed data, was "sr_robot3-2023.2.0.tar", max compression
```

## Comparing `sr.robot3-2023.0.5.tar` & `sr_robot3-2023.2.0.tar`

### file list

```diff
@@ -1,25 +1,23 @@
--rw-r--r--   0        0        0     1073 2022-10-14 20:22:59.993245 sr.robot3-2023.0.5/LICENSE
--rw-r--r--   0        0        0     2144 2022-10-14 20:22:59.993431 sr.robot3-2023.0.5/README.md
--rw-r--r--   0        0        0     1164 2022-10-18 18:46:06.233401 sr.robot3-2023.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-14 20:22:59.994243 sr.robot3-2023.0.5/sr/__init__.py
--rw-r--r--   0        0        0     1518 2022-10-15 01:00:07.623180 sr.robot3-2023.0.5/sr/robot3/__init__.py
--rw-r--r--   0        0        0     5371 2022-10-14 20:22:59.994514 sr.robot3-2023.0.5/sr/robot3/astoria.py
--rw-r--r--   0        0        0     1753 2022-10-15 01:00:07.623341 sr.robot3-2023.0.5/sr/robot3/env.py
--rw-r--r--   0        0        0     1066 2022-10-14 20:22:59.994680 sr.robot3-2023.0.5/sr/robot3/game.py
--rw-r--r--   0        0        0     5702 2022-10-18 17:21:51.465781 sr.robot3-2023.0.5/sr/robot3/kch.py
--rw-r--r--   0        0        0      358 2022-10-14 20:22:59.994837 sr.robot3-2023.0.5/sr/robot3/logging.py
--rw-r--r--   0        0        0       95 2022-10-14 20:22:59.994909 sr.robot3-2023.0.5/sr/robot3/py.typed
--rw-r--r--   0        0        0    12367 2022-10-18 18:46:06.233564 sr.robot3-2023.0.5/sr/robot3/robot.py
--rw-r--r--   0        0        0      641 2022-10-14 20:22:59.995108 sr.robot3-2023.0.5/sr/robot3/timeout.py
--rw-r--r--   0        0        0      110 2022-10-14 20:22:59.995226 sr.robot3-2023.0.5/sr/robot3/vision/__init__.py
--rw-r--r--   0        0        0     4137 2022-10-18 17:21:51.466511 sr.robot3-2023.0.5/sr/robot3/vision/backend.py
--rw-r--r--   0        0        0     1080 2022-10-14 20:22:59.995448 sr.robot3-2023.0.5/sr/robot3/vision/calibrations/FaceTime HD Camera.xml
--rw-r--r--   0        0        0     1174 2022-10-14 20:22:59.995548 sr.robot3-2023.0.5/sr/robot3/vision/calibrations/Logitech B500.xml
--rw-r--r--   0        0        0     1219 2022-10-14 20:22:59.995644 sr.robot3-2023.0.5/sr/robot3/vision/calibrations/Logitech C270.xml
--rw-r--r--   0        0        0     1000 2022-10-14 20:22:59.995746 sr.robot3-2023.0.5/sr/robot3/vision/calibrations/Logitech C905.xml
--rw-r--r--   0        0        0     1080 2022-10-14 20:22:59.995830 sr.robot3-2023.0.5/sr/robot3/vision/calibrations/Logitech C920.xml
--rw-r--r--   0        0        0     1002 2022-10-14 20:22:59.995912 sr.robot3-2023.0.5/sr/robot3/vision/calibrations/Microdia Integrated_Webcam_HD.xml
--rw-r--r--   0        0        0       58 2022-10-14 20:22:59.995988 sr.robot3-2023.0.5/sr/robot3/vision/calibrations/__init__.py
--rw-r--r--   0        0        0     2304 2022-10-14 20:22:59.996073 sr.robot3-2023.0.5/sr/robot3/vision/strategy.py
--rw-r--r--   0        0        0     3097 2022-10-18 19:00:37.249880 sr.robot3-2023.0.5/setup.py
--rw-r--r--   0        0        0     3145 2022-10-18 19:00:37.250087 sr.robot3-2023.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-09 19:23:58.652347 sr_robot3-2023.2.0/LICENSE
+-rw-r--r--   0        0        0     2144 2023-05-09 19:23:58.652646 sr_robot3-2023.2.0/README.md
+-rw-r--r--   0        0        0     1250 2023-05-09 19:23:58.653779 sr_robot3-2023.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-06 10:33:35.215730 sr_robot3-2023.2.0/sr/__init__.py
+-rw-r--r--   0        0        0     1518 2022-11-11 19:17:03.483745 sr_robot3-2023.2.0/sr/robot3/__init__.py
+-rw-r--r--   0        0        0     7549 2022-11-23 22:48:00.676296 sr_robot3-2023.2.0/sr/robot3/astoria.py
+-rw-r--r--   0        0        0     1751 2023-01-11 21:15:06.208205 sr_robot3-2023.2.0/sr/robot3/env.py
+-rw-r--r--   0        0        0     1063 2023-01-11 21:15:06.208705 sr_robot3-2023.2.0/sr/robot3/game.py
+-rw-r--r--   0        0        0     5702 2022-11-11 19:17:07.563408 sr_robot3-2023.2.0/sr/robot3/kch.py
+-rw-r--r--   0        0        0      358 2022-09-06 10:33:35.216394 sr_robot3-2023.2.0/sr/robot3/logging.py
+-rw-r--r--   0        0        0     4589 2023-05-09 19:23:41.913315 sr_robot3-2023.2.0/sr/robot3/mqtt.py
+-rw-r--r--   0        0        0       95 2022-09-06 10:33:35.216506 sr_robot3-2023.2.0/sr/robot3/py.typed
+-rw-r--r--   0        0        0    13791 2023-05-09 19:23:41.914034 sr_robot3-2023.2.0/sr/robot3/robot.py
+-rw-r--r--   0        0        0      641 2022-10-15 13:37:35.899140 sr_robot3-2023.2.0/sr/robot3/timeout.py
+-rw-r--r--   0        0        0       18 2023-05-09 19:23:41.914173 sr_robot3-2023.2.0/sr/robot3/vision/__init__.py
+-rw-r--r--   0        0        0     1118 2023-05-09 19:23:41.914425 sr_robot3-2023.2.0/sr/robot3/vision/calibrations/FaceTime HD Camera.xml
+-rw-r--r--   0        0        0     1132 2023-05-09 19:23:41.914560 sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Logitech B500.xml
+-rw-r--r--   0        0        0     1155 2023-05-09 19:23:41.914683 sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Logitech C270.xml
+-rw-r--r--   0        0        0     1029 2023-05-09 19:23:41.914782 sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Logitech C905.xml
+-rw-r--r--   0        0        0     1133 2023-05-09 19:23:41.914873 sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Logitech C920.xml
+-rw-r--r--   0        0        0     1031 2023-05-09 19:23:41.914965 sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Microdia Integrated_Webcam_HD.xml
+-rw-r--r--   0        0        0       58 2023-05-09 19:23:41.915534 sr_robot3-2023.2.0/sr/robot3/vision/calibrations/__init__.py
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 sr_robot3-2023.2.0/PKG-INFO
```

### Comparing `sr.robot3-2023.0.5/LICENSE` & `sr_robot3-2023.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sr.robot3-2023.0.5/README.md` & `sr_robot3-2023.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sr.robot3-2023.0.5/pyproject.toml` & `sr_robot3-2023.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sr.robot3"
-version = "2023.0.5"
+version = "2023.2.0"
 description = "Student Robotics API for Python 3"
 authors = ["Student Robotics <kit-brain@studentrobotics.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/srobo/sr-robot3"
 homepage = "https://github.com/srobo/sr-robot3"
 documentation = "https://studentrobotics.org/docs"
@@ -14,38 +14,40 @@
 ]
 packages = [
     { include = "sr" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-j5 = "^1.1.0"
-j5-zoloto = "^0.4.0"
+j5 = "^1.1.2"
 pyserial = "^3.4"
-astoria = "^0.9.0"
+astoria = "^0.11.1"
 "RPi.GPIO" = {version = "^0.7.0", optional = true}
+paho-mqtt = "^1.6.1"
+april-vision = {version = "^1.0.0", extras = ["j5"]}
 
 [tool.poetry.extras]
 kch = ["RPi.GPIO"]
 
 [tool.poetry.dev-dependencies]
 flake8 = "*"
 flake8-bugbear = "*"
-flake8-builtins = "*"
+flake8-builtins = "^2.0.1"
 flake8-commas = "*"
 flake8-comprehensions = "*"
 flake8-debugger = "*"
 flake8-docstrings = "*"
 flake8-isort = "*"
 flake8-mutable = "*"
 flake8-print = "*"
 flake8-todo = "*"
 mypy = "*"
 pytest = "*"
 pytest-cov = "*"
 rope = "*"
 isort = {version = "*",extras = ["pyproject"]}
 packaging = "*"
+types-paho-mqtt = "^1.6.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `sr.robot3-2023.0.5/sr/robot3/__init__.py` & `sr_robot3-2023.2.0/sr/robot3/__init__.py`

 * *Files identical despite different names*

### Comparing `sr.robot3-2023.0.5/sr/robot3/astoria.py` & `sr_robot3-2023.2.0/sr/robot3/astoria.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,153 +1,226 @@
 """Integration with Astoria."""
 
-import asyncio
 import logging
 from json import JSONDecodeError, loads
 from pathlib import Path
-from typing import Match, NamedTuple, Optional
+from queue import PriorityQueue
+from threading import Event
+from typing import Any, Generic, NamedTuple, Optional, Type, TypeVar
 
-from astoria.common.components import StateConsumer
+from astoria.common.config import AstoriaConfig
 from astoria.common.ipc import (
+    BroadcastEvent,
     MetadataManagerMessage,
     ProcessManagerMessage,
     StartButtonBroadcastEvent,
 )
 from astoria.common.metadata import Metadata
-from astoria.common.mqtt import BroadcastHelper
-from pydantic import parse_obj_as
+from paho.mqtt.client import Client as MQTT
+from paho.mqtt.client import MQTTMessage
+from pydantic import ValidationError, parse_obj_as
 
-LOGGER = logging.getLogger(__name__)
+from .mqtt import MQTTClient
 
-loop = asyncio.get_event_loop()
+LOGGER = logging.getLogger(__name__)
 
 
 class GetMetadataResult(NamedTuple):
     """Result returned from fetching metadata from astoria."""
 
     metadata: Metadata
     usb_path: Path
 
 
-class GetMetadataConsumer(StateConsumer):
-    """Astoria consumer to fetch metadata."""
+class GetMetadataConsumer:
+    """MQTT consumer to fetch metadata."""
 
     name = "sr-robot3-metadata"
 
-    def _setup_logging(self, verbose: bool, *, welcome_message: bool = True) -> None:
-        """Use the logging from sr-robot3."""
-        # Suppress INFO messages from gmqtt
-        logging.getLogger("gmqtt").setLevel(logging.WARNING)
+    def __init__(self, mqtt_client: MQTTClient) -> None:
+        self._mqtt = mqtt_client
 
-    def _init(self) -> None:
-        """Initialise consumer."""
+        # Initialise consumer data structures.
         self._metadata_message: Optional[MetadataManagerMessage] = None
         self._proc_message: Optional[ProcessManagerMessage] = None
-        self._state_lock = asyncio.Lock()
+        self._astmetad_received = Event()
+        self._astprocd_received = Event()
+
+    def run(self, timeout: Optional[float] = None) -> bool:
+        """Entrypoint for the data component."""
         self._mqtt.subscribe("astmetad", self._handle_astmetad_message)
         self._mqtt.subscribe("astprocd", self._handle_astprocd_message)
 
-    async def _handle_astmetad_message(
+        timeout_step = (timeout / 2) if timeout is not None else None
+
+        # wait for both messages to be received with a timeout
+        # the division of time between each step is irrelevant,
+        # messages can arrive for either during the whole period
+        self._astmetad_received.wait(timeout=timeout_step)
+        metadata_received = self._astprocd_received.wait(timeout=timeout_step)
+
+        self._mqtt.unsubscribe("astmetad")
+        self._mqtt.unsubscribe("astprocd")
+
+        return metadata_received
+
+    def _handle_astmetad_message(
         self,
-        match: Match[str],
-        payload: str,
+        client: MQTT,
+        userdata: Any,
+        msg: MQTTMessage,
     ) -> None:
         """Handle astmetad status messages."""
-        async with self._state_lock:
-            try:
-                message = parse_obj_as(MetadataManagerMessage, loads(payload))
-                if message.status == MetadataManagerMessage.Status.RUNNING:
-                    LOGGER.debug("Received metadata")
-                    self._metadata_message = message
-                else:
-                    LOGGER.warn("Cannot get metadata, astmetad is not running")
-            except JSONDecodeError:
-                LOGGER.error("Could not decode JSON metadata.")
-            if self._metadata_message is not None and self._proc_message is not None:
-                self.halt(silent=True)
+        try:
+            message = parse_obj_as(MetadataManagerMessage, loads(msg.payload))
+            if message.status == MetadataManagerMessage.Status.RUNNING:
+                LOGGER.debug("Received metadata")
+                self._metadata_message = message
+                self._astmetad_received.set()
+            else:
+                LOGGER.warn("Cannot get metadata, astmetad is not running")
+        except JSONDecodeError:
+            LOGGER.error("Could not decode JSON metadata.")
+        except ValidationError as e:
+            LOGGER.error(f"Unable to parse metadata message: {e}")
 
-    async def _handle_astprocd_message(
+    def _handle_astprocd_message(
         self,
-        match: Match[str],
-        payload: str,
+        client: MQTT,
+        userdata: Any,
+        msg: MQTTMessage,
     ) -> None:
         """Handle astprocd status messages."""
-        async with self._state_lock:
-            try:
-                message = parse_obj_as(ProcessManagerMessage, loads(payload))
-                if message.status == ProcessManagerMessage.Status.RUNNING:
-                    LOGGER.debug("Received process info")
-                    self._proc_message = message
-                else:
-                    LOGGER.warn("Cannot get process info, astprocd is not running")
-            except JSONDecodeError:
-                LOGGER.error("Could not decode JSON metadata.")
-            if self._metadata_message is not None and self._proc_message is not None:
-                self.halt(silent=True)
-
-    async def main(self) -> None:
-        """Main method of the command."""
-        await self.wait_loop()
+        try:
+            message = parse_obj_as(ProcessManagerMessage, loads(msg.payload))
+            if message.status == ProcessManagerMessage.Status.RUNNING:
+                LOGGER.debug("Received process info")
+                self._proc_message = message
+                self._astprocd_received.set()
+            else:
+                LOGGER.warn("Cannot get process info, astprocd is not running")
+        except JSONDecodeError:
+            LOGGER.error("Could not decode JSON metadata.")
+        except ValidationError as e:
+            LOGGER.error(f"Unable to parse process message: {e}")
 
     @classmethod
-    def get_metadata(cls) -> GetMetadataResult:
+    def get_metadata(cls, mqtt_client: MQTTClient) -> GetMetadataResult:
         """Get metadata."""
-        gmc = cls(False, None)
+        gmc = cls(mqtt_client)
+        config = AstoriaConfig.load()
 
-        metadata = Metadata.init(gmc.config)
+        metadata = Metadata.init(config)
         path = Path("/dev/null")
 
         try:
-            loop.run_until_complete(asyncio.wait_for(gmc.run(), timeout=0.1))
-            if gmc._metadata_message is not None:
-                metadata = gmc._metadata_message.metadata
-
-            if gmc._proc_message is not None and gmc._proc_message.disk_info is not None:
-                path = gmc._proc_message.disk_info.mount_path
+            metadata_received = gmc.run(timeout=0.1)
+            if metadata_received:
+                if gmc._metadata_message is not None:
+                    metadata = gmc._metadata_message.metadata
+
+                if gmc._proc_message and gmc._proc_message.disk_info:
+                    path = gmc._proc_message.disk_info.mount_path
+            else:
+                LOGGER.warning("Astoria took too long to respond, giving up.")
         except ConnectionRefusedError:
             LOGGER.warning("Unable to connect to MQTT broker")
-        except asyncio.TimeoutError:
-            LOGGER.warning("Astoria took too long to respond, giving up.")
 
         return GetMetadataResult(metadata, path)
 
 
-class WaitForStartButtonBroadcastConsumer(StateConsumer):
-    """Wait for a start button broadcast."""
+class WaitForStartButtonBroadcastConsumer:
+    """MQTT consumer to wait for a start button broadcast."""
+
+    def __init__(self, mqtt_client: MQTTClient, start_event: Event) -> None:
+        self._trigger_event = BroadcastHelper.get_helper(
+            mqtt_client,
+            StartButtonBroadcastEvent,
+            start_event,
+        )
+
+        self._start_event = start_event
+
+    def run(self) -> None:
+        """Entrypoint for the data component."""
+        self._start_event.wait()
+
+    def close(self) -> None:
+        """Tidy up BroadcastHelper subscriptions."""
+        # run BroadcastHelper __del__ routine to unsubscribe
+        del self._trigger_event
+
 
-    name = "sr-robot3-wait-start"
+T = TypeVar("T", bound=BroadcastEvent)
+
+
+class BroadcastHelper(Generic[T]):
+    """
+    Helper class to manage broadcast events.
+
+    Subscribes to broadcast/{name} topic, validates received messages
+    against the supplied schema and puts messages in a queue that can
+    be read by wait_broadcast.
+    """
 
     def __init__(
         self,
-        verbose: bool,
-        config_file: Optional[str],
-        start_event: asyncio.Event,
+        mqtt: 'MQTTClient',
+        name: str,
+        schema: Type[T],
+        message_event: Optional[Event] = None,
     ) -> None:
-        super().__init__(verbose, config_file)
-        self._start_event = start_event
+        self._mqtt = mqtt
+        self._name = name
+        self._schema = schema
+
+        self.message_received = message_event if message_event is not None else Event()
+        self._event_queue: PriorityQueue[T] = PriorityQueue()
+        self._mqtt.subscribe(f"broadcast/{name}", self._handle_broadcast)
+
+    def __del__(self) -> None:
+        """Unsubscribe the broadcast topic on destruction."""
+        self._mqtt.unsubscribe(f"broadcast/{self._name}")
 
-    def _setup_logging(self, verbose: bool, *, welcome_message: bool = True) -> None:
-        """Use the logging from sr-robot3."""
-        # Suppress INFO messages from gmqtt
-        logging.getLogger("gmqtt").setLevel(logging.WARNING)
+    @classmethod
+    def get_helper(
+        cls, mqtt: 'MQTTClient', schema: Type[T], message_event: Optional[Event] = None,
+    ) -> 'BroadcastHelper[T]':
+        """Get the broadcast helper for a given event."""
+        return BroadcastHelper[T](mqtt, schema.name, schema, message_event)
 
-    def _init(self) -> None:
+    def _handle_broadcast(
+        self,
+        client: MQTT,
+        userdata: Any,
+        msg: MQTTMessage,
+    ) -> None:
         """
-        Initialisation of the data component.
+        Handle a broadcast event message.
 
-        Called in the constructor of the parent class.
+        Inserts the event into the priority queue.
         """
-        self._trigger_event = BroadcastHelper.get_helper(
-            self._mqtt,
-            StartButtonBroadcastEvent,
+        try:
+            ev = parse_obj_as(self._schema, loads(msg.payload))
+            LOGGER.debug(
+                f"Received {ev.event_name} broadcast event from {ev.sender_name}",
+            )
+            self._event_queue.put(ev)
+            self.message_received.set()
+        except JSONDecodeError:
+            LOGGER.warning(f"Broadcast event {self._name} contained invalid JSON")
+
+    def send(self, **kwargs: Any) -> None:
+        """Send an event."""
+        data = self._schema(
+            event_name=self._schema.name,
+            sender_name=self._mqtt._client_name,
+            **kwargs,
+        )
+        self._mqtt.publish(
+            f"broadcast/{self._schema.name}",
+            data.json(),
         )
 
-    async def main(self) -> None:
-        """Wait for a trigger event."""
-        while not self._start_event.is_set():
-            # wait_broadcast waits forever until a broadcoast, so we will use a short
-            # timeout to ensure that the loop condition is checked.
-            try:
-                await asyncio.wait_for(self._trigger_event.wait_broadcast(), timeout=0.1)
-                self._start_event.set()
-            except asyncio.TimeoutError:
-                pass
+    def wait_broadcast(self, timeout: Optional[float] = None) -> T:
+        """Wait for an event on the given broadcast."""
+        return self._event_queue.get(timeout=timeout)
```

### Comparing `sr.robot3-2023.0.5/sr/robot3/env.py` & `sr_robot3-2023.2.0/sr/robot3/env.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Environment definitions."""
 
+from april_vision.j5 import AprilTagHardwareBackend
 from j5.backends import Environment
 from j5.backends.console.sr.v4 import (
     SRV4MotorBoardConsoleBackend,
     SRV4PowerBoardConsoleBackend,
     SRV4RuggeduinoConsoleBackend,
     SRV4ServoBoardConsoleBackend,
 )
@@ -15,31 +16,29 @@
 )
 
 __all__ = [
     "HARDWARE_ENVIRONMENT",
     "CONSOLE_ENVIRONMENT",
 ]
 
-from sr.robot3.vision import SRZolotoHardwareBackend
-
 HARDWARE_ENVIRONMENT = Environment("Hardware Environment")
 
 HARDWARE_ENVIRONMENT.register_backend(SRV4PowerBoardHardwareBackend)
 HARDWARE_ENVIRONMENT.register_backend(SRV4ServoBoardHardwareBackend)
 HARDWARE_ENVIRONMENT.register_backend(SRV4MotorBoardHardwareBackend)
 HARDWARE_ENVIRONMENT.register_backend(SRV4RuggeduinoHardwareBackend)
-HARDWARE_ENVIRONMENT.register_backend(SRZolotoHardwareBackend)
+HARDWARE_ENVIRONMENT.register_backend(AprilTagHardwareBackend)
 
 CONSOLE_ENVIRONMENT = Environment("Console Environment")
 
 CONSOLE_ENVIRONMENT.register_backend(SRV4PowerBoardConsoleBackend)
 CONSOLE_ENVIRONMENT.register_backend(SRV4ServoBoardConsoleBackend)
 CONSOLE_ENVIRONMENT.register_backend(SRV4MotorBoardConsoleBackend)
 CONSOLE_ENVIRONMENT.register_backend(SRV4RuggeduinoConsoleBackend)
 
 CONSOLE_ENVIRONMENT_WITH_VISION = Environment("Console Environment with Vision")
 
 CONSOLE_ENVIRONMENT_WITH_VISION.register_backend(SRV4PowerBoardConsoleBackend)
 CONSOLE_ENVIRONMENT_WITH_VISION.register_backend(SRV4ServoBoardConsoleBackend)
 CONSOLE_ENVIRONMENT_WITH_VISION.register_backend(SRV4MotorBoardConsoleBackend)
 CONSOLE_ENVIRONMENT_WITH_VISION.register_backend(SRV4RuggeduinoConsoleBackend)
-CONSOLE_ENVIRONMENT_WITH_VISION.register_backend(SRZolotoHardwareBackend)
+CONSOLE_ENVIRONMENT_WITH_VISION.register_backend(AprilTagHardwareBackend)
```

### Comparing `sr.robot3-2023.0.5/sr/robot3/game.py` & `sr_robot3-2023.2.0/sr/robot3/game.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Game specific code."""
-from typing import Container, Dict
+from typing import Dict, Iterable
 
 
 class UnusedMarkerException(Exception):
     """This marker is not used for the game."""
 
 
-MARKER_SIZES: Dict[Container[int], int] = {
+MARKER_SIZES: Dict[Iterable[int], int] = {
     range(28): 200,  # 0 - 27 for arena boundary
-    range(28, 100): 100,  # Everything else is a token
+    range(28, 100): 80,  # Everything else is a token
 }
 
 
 def marker_used_in_game(marker_id: int) -> bool:
     """
     Determine whether the marker ID is used in the game.
```

### Comparing `sr.robot3-2023.0.5/sr/robot3/kch.py` & `sr_robot3-2023.2.0/sr/robot3/kch.py`

 * *Files identical despite different names*

### Comparing `sr.robot3-2023.0.5/sr/robot3/robot.py` & `sr_robot3-2023.2.0/sr/robot3/robot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 """sr.robot3 Robot class."""
 
-import asyncio
 import logging
 import os
+import threading
+import time
 from datetime import timedelta
 from pathlib import Path
-from typing import Dict, List, Optional, Set, Type
+from typing import Dict, List, Optional, Type, Union
 
+from april_vision.j5 import AprilCameraBoard
 from astoria.common.metadata import Metadata, RobotMode
 from j5 import BaseRobot, Environment
 from j5 import __version__ as j5_version
 from j5.backends import Backend
 from j5.boards import Board, BoardGroup
 from j5.boards.sr.v4 import MotorBoard, PowerBoard, Ruggeduino, ServoBoard
 from j5.components.piezo import Note
-from j5_zoloto import ZolotoCameraBoard, ZolotoHardwareBackend
 from serial.tools.list_ports_common import ListPortInfo
-from zoloto.cameras.camera import find_camera_ids
 
 from .astoria import GetMetadataConsumer, WaitForStartButtonBroadcastConsumer
 from .env import HARDWARE_ENVIRONMENT
+from .game import MARKER_SIZES
 from .kch import KCH
+from .mqtt import init_mqtt
 from .timeout import kill_after_delay
-from .vision import SRZolotoHardwareBackend
 
-__version__ = "2023.0.5"
+__version__ = "2023.2.0"
 
 
 LOGGER = logging.getLogger(__name__)
 
-loop = asyncio.get_event_loop()
-
 
 class Robot(BaseRobot):
     """
     Student Robotics robot.
 
     Inherits from j5 BaseRobot to ensure that all boards are made safe
     in the event of a crash, and to ensure that there is only one instance
@@ -44,49 +43,60 @@
     def __init__(
             self,
             *,
             auto_start: bool = False,
             verbose: bool = False,
             env: Environment = HARDWARE_ENVIRONMENT,
             ignored_ruggeduinos: Optional[List[str]] = None,
+            legacy_camera_axis: bool = True,
     ) -> None:
         """
         Initialise a Robot object.
 
         :param auto_start: Automatically start the robot ignoring the start
             button, defaults to False.
         :param verbose: Turn on verbose logging, defaults to False.
         :param env: The :class:`j5.backends.environment.Environment` to run the
             Robot under. See :ref:`Environments` for more information.
         :param ignored_ruggeduinos: List of Ruggeduino serial numbers to ignore.
             See :ref:`Custom Ruggeduino Firmware` for more information.
+        :param legacy_camera_axis: Use the coordinate systems the camera used
+            prior to SR OS 2023.1.0.
         """
         self._auto_start = auto_start
         self._verbose = verbose
         self._environment = env
 
         if verbose:
-            LOGGER.setLevel(logging.DEBUG)
+            # Set root logger to DEBUG level
+            logging.getLogger().setLevel(logging.DEBUG)
             os.environ["OPENCV_LOG_LEVEL"] = "DEBUG"
         else:
             os.environ["OPENCV_LOG_LEVEL"] = "ERROR"
 
         if ignored_ruggeduinos is None:
             self._ignored_ruggeduino_serials = []
         else:
             self._ignored_ruggeduino_serials = ignored_ruggeduinos
 
         LOGGER.debug("Verbose mode enabled.")
         LOGGER.debug(f"sr.robot3 version {__version__}")
         LOGGER.debug(f"j5 version {j5_version}")
         LOGGER.debug(f"Environment: {self._environment.name}")
 
+        self._mqtt = init_mqtt()
+
         self._init_metadata()
 
         self._init_cameras(self.metadata.marker_offset)
+        if legacy_camera_axis:
+            LOGGER.info("Using legacy coordinate system for vision")
+            os.environ['ZOLOTO_LEGACY_AXIS'] = '1'
+        else:
+            LOGGER.info("Using updated coordinate system for vision")
         self._init_power_board()
         self._init_auxiliary_boards()
 
         self._init_ruggeduinos()
 
         self._log_discovered_boards()
 
@@ -94,37 +104,39 @@
             LOGGER.debug("Auto start is enabled.")
         else:
             LOGGER.debug("Auto start is disabled.")
             self.wait_start()
 
     def _init_cameras(self, marker_offset: int) -> None:
         """Initialise vision system for a single camera."""
-        backend_class: Type[Backend] = self._environment.get_backend(ZolotoCameraBoard)
-
-        # Override the hardware backend with our custom one
-        if backend_class is ZolotoHardwareBackend:
-            backend_class = SRZolotoHardwareBackend
+        def mqtt_publish_callback(topic: str, payload: Union[bytes, str]) -> None:
+            self._mqtt.publish(topic, payload, auto_prefix_topic=False)
 
-        class OffsetZolotoBackend(backend_class):  # type: ignore
-            """A zoloto backend, with marker offsets added."""
-
-            @classmethod
-            def discover(cls) -> Set[Board]:
-                return {
-                    ZolotoCameraBoard(
-                        str(camera_id),
-                        cls(camera_id, marker_offset=marker_offset),
-                    )
-                    for camera_id in find_camera_ids()
-                }
-
-        self._cameras = BoardGroup.get_board_group(
-            ZolotoCameraBoard,
-            OffsetZolotoBackend,
-        )
+        self._cameras: BoardGroup[AprilCameraBoard, Backend]
+        try:
+            # Setup calibration file locations
+            from .vision.calibrations import __file__ as calibrations
+
+            # get any pre-defined calibration locations
+            current_calibrations = os.environ.get('OPENCV_CALIBRATIONS', '')
+            calibration_locs = ':'.join(
+                [current_calibrations, os.path.dirname(calibrations)])
+            os.environ['OPENCV_CALIBRATIONS'] = calibration_locs.strip(':')
+
+            self._cameras = self._environment.get_board_group(AprilCameraBoard)
+            # setup marker sizes
+            for cam in self._cameras:
+                cam._backend.set_marker_sizes(
+                    MARKER_SIZES, marker_offset=marker_offset)
+
+                # Insert a reference to the MQTT client into the camera backend
+                # to allow frames to be sent to the website
+                cam._backend._mqtt_publish = mqtt_publish_callback
+        except NotImplementedError:
+            LOGGER.warning("No camera backend found")
 
     def _init_power_board(self) -> None:
         """
         Find and initialise the power board.
 
         The power board is is the only required board.
         """
@@ -164,35 +176,41 @@
         self._ruggeduinos = BoardGroup.get_board_group(
             Ruggeduino,
             IgnoredRuggeduinoBackend,
         )
 
     def _init_metadata(self) -> None:
         """Fetch metadata from Astoria."""
-        self._metadata, self._code_path = GetMetadataConsumer.get_metadata()
+        self._metadata, self._code_path = GetMetadataConsumer.get_metadata(
+            self._mqtt,
+        )
         offset = self._metadata.marker_offset
         if hasattr(self, '_cameras'):
             for camera in self._cameras:
-                zcam = camera._backend._zcam  # type: ignore[attr-defined]
-                zcam._marker_offset = offset
+                try:
+                    # Update enabled markers
+                    camera._backend.set_marker_sizes(
+                        MARKER_SIZES, marker_offset=offset)
+                except AttributeError:
+                    pass
 
     def _log_discovered_boards(self) -> None:
         """Log all boards that we have discovered."""
         for board in Board.BOARDS:
             LOGGER.info(f"Found {board.name} - {board.serial_number}")
             LOGGER.debug(
                 f"Firmware Version of {board.serial_number}: {board.firmware_version}",
             )
 
     @property
-    def camera(self) -> ZolotoCameraBoard:
+    def camera(self) -> AprilCameraBoard:
         """
         Get the robot's camera interface.
 
-        :returns: a :class:`j5_zoloto.board.ZolotoCameraBoard`.
+        :returns: a :class:`april_vision.j5.AprilCameraBoard`.
         """
         return self._cameras.singular()
 
     @property
     def kch(self) -> KCH:
         """
         Get the KCH.
@@ -317,66 +335,90 @@
         """
         The arena zone that the robot starts in.
 
         :returns: arena zone that the robot starts in.
         """
         return self.metadata.zone
 
+    @property
+    def is_simulated(self) -> bool:
+        """
+        Determine whether the robot is simulated.
+
+        :returns: True if the robot is simulated. False otherwise.
+        """
+        return False
+
     def print_wifi_details(self) -> None:
         """Prints the current WiFi details stored in robot-settings.toml."""
         if not self.metadata.wifi_enabled:
             LOGGER.warn("Could not print WiFi details - WiFi is not enabled")
             return
         LOGGER.info("WiFi credentials:")
         LOGGER.info(f"SSID: {self.metadata.wifi_ssid}")
         LOGGER.info(f"Password: {self.metadata.wifi_psk}")
 
+    def sleep(self, secs: float) -> None:
+        """
+        Wait for the specified amount of time.
+
+        This exists for compatibility with the simulator API only.
+
+        :param secs: the number of seconds to wait for.
+        """
+        return time.sleep(secs)
+
+    def time(self) -> float:
+        """
+        Get the number of seconds since the Unix Epoch.
+
+        This exists for compatibility with the simulator API only.
+
+        :returns: the number of seconds since the Unix Epoch.
+        """
+        return time.time()
+
     def wait_start(self) -> None:
         """
         Wait for a start signal.
 
         Intended for use with `Robot(auto_start=False)`, to allow
         students to run code and setup their robot before the start
         of a match.
         """
         LOGGER.info("Waiting for start signal")
 
-        start_event = asyncio.Event()
+        start_event = threading.Event()
 
         astoria_start = WaitForStartButtonBroadcastConsumer(
-            self._verbose,
-            None,  # Don't pass a config
+            self._mqtt,
             start_event,
         )
 
-        async def wait_for_physical_start() -> None:
-            self.power_board.piezo.buzz(timedelta(seconds=0.1), Note.A6)
-            counter = 0
-            led_state = False
-            _ = self.power_board.start_button.is_pressed
-            while not self.power_board.start_button.is_pressed and not start_event.is_set():  # noqa: E501
-                if counter % 6 == 0:
-                    led_state = not led_state
-                    self.power_board._run_led.state = led_state
-                    self.kch.start = led_state
-                await asyncio.sleep(0.05)
-                counter += 1
-            start_event.set()
-            # Turn on the LED now that we are starting
-            self.power_board._run_led.state = True
-
-            # Turn off the KCH Start LED.
-            self.kch.start = False
-
-        loop.run_until_complete(
-            asyncio.gather(
-                astoria_start.run(),
-                wait_for_physical_start(),
-            ),
-        )
+        self.power_board.piezo.buzz(timedelta(seconds=0.1), Note.A6)
+        counter = 0
+        led_state = False
+        _ = self.power_board.start_button.is_pressed
+        while not self.power_board.start_button.is_pressed and \
+                not start_event.is_set():
+            if counter % 6 == 0:
+                led_state = not led_state
+                self.power_board._run_led.state = led_state
+                self.kch.start = led_state
+            time.sleep(0.05)
+            counter += 1
+
+        # Tidy up wait start subscriptions
+        astoria_start.close()
+
+        # Turn on the LED now that we are starting
+        self.power_board._run_led.state = True
+
+        # Turn off the KCH Start LED.
+        self.kch.start = False
 
         # Reload metadata as a metadata USB may have been inserted.
         # This ensures that the game timeout is observed even if the metadata
         # USB is inserted after usercode execution begins.
         self._init_metadata()
 
         LOGGER.info("Start signal received; continuing.")
```

### Comparing `sr.robot3-2023.0.5/sr/robot3/timeout.py` & `sr_robot3-2023.2.0/sr/robot3/timeout.py`

 * *Files identical despite different names*

### Comparing `sr.robot3-2023.0.5/sr/robot3/vision/calibrations/FaceTime HD Camera.xml` & `sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Logitech C905.xml`

 * *Files 12% similar despite different names*

#### Comparing `sr.robot3-2023.0.5/sr/robot3/vision/calibrations/FaceTime HD Camera.xml` & `sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Logitech C905.xml`

```diff
@@ -1,33 +1,34 @@
 <?xml version="1.0" encoding="utf-8"?>
 <opencv_storage>
-  <calibrationDate>&quot;Sun Oct 10 16:29:49 2021&quot;</calibrationDate>
+  <calibrationDate>&quot;Sun Oct 10 19:10:39 2021&quot;</calibrationDate>
   <framesCount>29</framesCount>
-  <cameraResolution>1280 720</cameraResolution>
+  <cameraResolution>1600 1200</cameraResolution>
   <cameraMatrix type_id="opencv-matrix">
     <rows>3</rows>
     <cols>3</cols>
     <dt>d</dt>
-    <data>1.0059832255301474e+03 0. 6.3600363812582748e+02 0.
-    1.0059832255301474e+03 3.9032987567991756e+02 0. 0. 1.</data>
+    <data>1.3293794025699294e+03 0. 7.8278153644794213e+02 0.
+    1.3293794025699294e+03 5.2330447172180789e+02 0. 0. 1.</data>
   </cameraMatrix>
   <cameraMatrix_std_dev type_id="opencv-matrix">
     <rows>4</rows>
     <cols>1</cols>
     <dt>d</dt>
-    <data>0. 1.8390897483985235e+01 4.9795155412210459e+00
-    5.5464984166225326e+00</data>
+    <data>0. 1.2399372504497897e+01 2.7405288492518323e+00
+    3.4610941491213736e+00</data>
   </cameraMatrix_std_dev>
   <dist_coeffs type_id="opencv-matrix">
     <rows>1</rows>
     <cols>5</cols>
     <dt>d</dt>
-    <data>6.8703433405016029e-02 0. 0. 0. -2.4193185280867940e-01</data>
+    <data>0. 0. 0. 0. 0.</data>
   </dist_coeffs>
   <dist_coeffs_std_dev type_id="opencv-matrix">
     <rows>5</rows>
     <cols>1</cols>
     <dt>d</dt>
-    <data>1.2370831283282813e-02 0. 0. 0. 7.8882690649474521e-02</data>
+    <data>0. 0. 0. 0. 0.</data>
   </dist_coeffs_std_dev>
-  <avg_reprojection_error>4.8677611488489964e-01</avg_reprojection_error>
+  <avg_reprojection_error>9.9915642016590445e-01</avg_reprojection_error>
+  <vidpid>&quot;046d:080a&quot;</vidpid>
 </opencv_storage>
```

### Comparing `sr.robot3-2023.0.5/sr/robot3/vision/calibrations/Logitech B500.xml` & `sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Logitech B500.xml`

 * *Files 19% similar despite different names*

#### Comparing `sr.robot3-2023.0.5/sr/robot3/vision/calibrations/Logitech B500.xml` & `sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Logitech B500.xml`

```diff
@@ -1,35 +1,36 @@
 <?xml version="1.0" encoding="utf-8"?>
 <opencv_storage>
-  <calibrationDate>&quot;Thu 11 Nov 2021 17:34:35 GMT&quot;</calibrationDate>
-  <framesCount>29</framesCount>
+  <calibrationDate>&quot;Wed 23 Nov 2022 21:23:00 GMT&quot;</calibrationDate>
+  <framesCount>15</framesCount>
   <cameraResolution>1280 1024</cameraResolution>
   <cameraMatrix type_id="opencv-matrix">
     <rows>3</rows>
     <cols>3</cols>
     <dt>d</dt>
-    <data>9.3012007264063072e+02 0. 7.0226810811512655e+02 0.
-    9.3012007264063072e+02 4.7705847029705535e+02 0. 0. 1.</data>
+    <data>1.05711133e+03 0. 6.02433099e+02
+    0. 1.06661029e+03 4.51876692e+02
+    0. 0. 1.</data>
   </cameraMatrix>
   <cameraMatrix_std_dev type_id="opencv-matrix">
     <rows>4</rows>
     <cols>1</cols>
     <dt>d</dt>
     <data>0. 1.4841088432691212e+01 4.7206079728271524e+00
     4.2203301535161479e+00</data>
   </cameraMatrix_std_dev>
   <dist_coeffs type_id="opencv-matrix">
     <rows>1</rows>
     <cols>5</cols>
     <dt>d</dt>
-    <data>-9.2701468925095482e-02 2.9255285923072902e-02
-    -7.9310903187861364e-03 1.1943725785898814e-02 0.</data>
+    <data>-0.0930654 0.30046762 -0.00657921 -0.00055965 -0.48481949</data>
   </dist_coeffs>
   <dist_coeffs_std_dev type_id="opencv-matrix">
     <rows>5</rows>
     <cols>1</cols>
     <dt>d</dt>
     <data>4.4573481761620787e-03 4.5353543208646336e-03 9.4635517516124560e-04
     8.7616716255079267e-04 0.</data>
   </dist_coeffs_std_dev>
   <avg_reprojection_error>7.7260806740601118e-01</avg_reprojection_error>
+  <vidpid>&quot;046d:0807&quot;</vidpid>
 </opencv_storage>
```

### Comparing `sr.robot3-2023.0.5/sr/robot3/vision/calibrations/Logitech C270.xml` & `sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Logitech C270.xml`

 * *Files 15% similar despite different names*

#### Comparing `sr.robot3-2023.0.5/sr/robot3/vision/calibrations/Logitech C270.xml` & `sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Logitech C270.xml`

```diff
@@ -1,36 +1,36 @@
 <?xml version="1.0" encoding="utf-8"?>
 <opencv_storage>
-  <calibrationDate>&quot;Sun 10 Oct 2021 18:13:27 BST&quot;</calibrationDate>
+  <calibrationDate>&quot;Tue 22 Nov 2022 18:45:00 GMT&quot;</calibrationDate>
   <framesCount>29</framesCount>
   <cameraResolution>1280 960</cameraResolution>
   <cameraMatrix type_id="opencv-matrix">
     <rows>3</rows>
     <cols>3</cols>
     <dt>d</dt>
-    <data>1.5125977852617134e+03 0. 5.8171757235186294e+02 0.
-    1.5125977852617134e+03 4.3694004497775438e+02 0. 0. 1.</data>
+    <data>1.38752826e+03 0. 6.81279056e+02
+    0. 1.38764512e+03 5.32635142e+02
+    0. 0. 1.</data>
   </cameraMatrix>
   <cameraMatrix_std_dev type_id="opencv-matrix">
     <rows>4</rows>
     <cols>1</cols>
     <dt>d</dt>
     <data>0. 1.1587959248217736e+01 1.0915370551937198e+01
     9.9037897756709690e+00</data>
   </cameraMatrix_std_dev>
   <dist_coeffs type_id="opencv-matrix">
     <rows>1</rows>
     <cols>5</cols>
     <dt>d</dt>
-    <data>7.2702844094386473e-02 -1.0598889277707855e-02
-    -1.1532488282097528e-02 -1.7548754719661115e-02
-    -8.6188802908401987e-02</data>
+    <data>0.01737599  0.36629486 -0.00773113  0.00315102 -1.34355748</data>
   </dist_coeffs>
   <dist_coeffs_std_dev type_id="opencv-matrix">
     <rows>5</rows>
     <cols>1</cols>
     <dt>d</dt>
     <data>1.6799365761642784e-02 1.6619008373341906e-01 1.8815537093406550e-03
     2.6159487405108058e-03 5.3956051795557647e-01</data>
   </dist_coeffs_std_dev>
   <avg_reprojection_error>4.8437875296613170e-01</avg_reprojection_error>
+  <vidpid>&quot;046d:0825&quot;</vidpid>
 </opencv_storage>
```

### Comparing `sr.robot3-2023.0.5/sr/robot3/vision/calibrations/Logitech C905.xml` & `sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Microdia Integrated_Webcam_HD.xml`

 * *Files 20% similar despite different names*

#### Comparing `sr.robot3-2023.0.5/sr/robot3/vision/calibrations/Logitech C905.xml` & `sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Microdia Integrated_Webcam_HD.xml`

```diff
@@ -1,33 +1,34 @@
 <?xml version="1.0" encoding="utf-8"?>
 <opencv_storage>
-  <calibrationDate>&quot;Sun Oct 10 19:10:39 2021&quot;</calibrationDate>
+  <calibrationDate>&quot;Sun 10 Oct 2021 18:00:46 BST&quot;</calibrationDate>
   <framesCount>29</framesCount>
-  <cameraResolution>1600 1200</cameraResolution>
+  <cameraResolution>640 480</cameraResolution>
   <cameraMatrix type_id="opencv-matrix">
     <rows>3</rows>
     <cols>3</cols>
     <dt>d</dt>
-    <data>1.3293794025699294e+03 0. 7.8278153644794213e+02 0.
-    1.3293794025699294e+03 5.2330447172180789e+02 0. 0. 1.</data>
+    <data>6.3676395947858282e+02 0. 3.3237546391724510e+02 0.
+    6.3676395947858282e+02 2.5040026783771296e+02 0. 0. 1.</data>
   </cameraMatrix>
   <cameraMatrix_std_dev type_id="opencv-matrix">
     <rows>4</rows>
     <cols>1</cols>
     <dt>d</dt>
-    <data>0. 1.2399372504497897e+01 2.7405288492518323e+00
-    3.4610941491213736e+00</data>
+    <data>0. 8.0954290827551230e+00 2.4615221566691297e+00
+    3.7496179053522640e+00</data>
   </cameraMatrix_std_dev>
   <dist_coeffs type_id="opencv-matrix">
     <rows>1</rows>
     <cols>5</cols>
     <dt>d</dt>
     <data>0. 0. 0. 0. 0.</data>
   </dist_coeffs>
   <dist_coeffs_std_dev type_id="opencv-matrix">
     <rows>5</rows>
     <cols>1</cols>
     <dt>d</dt>
     <data>0. 0. 0. 0. 0.</data>
   </dist_coeffs_std_dev>
-  <avg_reprojection_error>9.9915642016590445e-01</avg_reprojection_error>
+  <avg_reprojection_error>3.0528763278506471e-01</avg_reprojection_error>
+  <vidpid>&quot;0c45:6713&quot;</vidpid>
 </opencv_storage>
```

### Comparing `sr.robot3-2023.0.5/sr/robot3/vision/calibrations/Logitech C920.xml` & `sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Logitech C920.xml`

 * *Files 7% similar despite different names*

#### Comparing `sr.robot3-2023.0.5/sr/robot3/vision/calibrations/Logitech C920.xml` & `sr_robot3-2023.2.0/sr/robot3/vision/calibrations/Logitech C920.xml`

```diff
@@ -26,8 +26,9 @@
   <dist_coeffs_std_dev type_id="opencv-matrix">
     <rows>5</rows>
     <cols>1</cols>
     <dt>d</dt>
     <data>0. 1.3176496934923674e-02 0. 0. 2.6883843151663960e-02</data>
   </dist_coeffs_std_dev>
   <avg_reprojection_error>6.6683521969915727e-01</avg_reprojection_error>
+  <vidpid>&quot;046d:082d&quot; &quot;046d:0892&quot; &quot;046d:08E5&quot;</vidpid>
 </opencv_storage>
```

### Comparing `sr.robot3-2023.0.5/setup.py` & `sr_robot3-2023.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,88 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sr-robot3
+Version: 2023.2.0
+Summary: Student Robotics API for Python 3
+Home-page: https://github.com/srobo/sr-robot3
+License: MIT
+Author: Student Robotics
+Author-email: kit-brain@studentrobotics.org
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Provides-Extra: kch
+Requires-Dist: RPi.GPIO (>=0.7.0,<0.8.0) ; extra == "kch"
+Requires-Dist: april-vision[j5] (>=1.0.0,<2.0.0)
+Requires-Dist: astoria (>=0.11.1,<0.12.0)
+Requires-Dist: j5 (>=1.1.2,<2.0.0)
+Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
+Requires-Dist: pyserial (>=3.4,<4.0)
+Project-URL: Documentation, https://studentrobotics.org/docs
+Project-URL: Repository, https://github.com/srobo/sr-robot3
+Description-Content-Type: text/markdown
 
-packages = \
-['sr', 'sr.robot3', 'sr.robot3.vision', 'sr.robot3.vision.calibrations']
+# sr.robot3
 
-package_data = \
-{'': ['*']}
+![Tests](https://github.com/srobo/sr-robot3/workflows/Tests/badge.svg)
+[![PyPI version](https://badge.fury.io/py/sr.robot3.svg)](https://pypi.org/project/sr.robot3/)
+[![MIT license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://opensource.org/licenses/MIT)
+![Bees](https://img.shields.io/badge/bees-110%25-yellow.svg)
 
-install_requires = \
-['astoria>=0.9.0,<0.10.0',
- 'j5-zoloto>=0.4.0,<0.5.0',
- 'j5>=1.1.0,<2.0.0',
- 'pyserial>=3.4,<4.0']
-
-extras_require = \
-{'kch': ['RPi.GPIO>=0.7.0,<0.8.0']}
-
-setup_kwargs = {
-    'name': 'sr.robot3',
-    'version': '2023.0.5',
-    'description': 'Student Robotics API for Python 3',
-    'long_description': '# sr.robot3\n\n![Tests](https://github.com/srobo/sr-robot3/workflows/Tests/badge.svg)\n[![PyPI version](https://badge.fury.io/py/sr.robot3.svg)](https://pypi.org/project/sr.robot3/)\n[![MIT license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://opensource.org/licenses/MIT)\n![Bees](https://img.shields.io/badge/bees-110%25-yellow.svg)\n\nStudent Robotics API for Python 3\n\nThis package uses [PEP420](https://www.python.org/dev/peps/pep-0420/)-style namespace packaging.\n\n## Development\n\n### Requirements\n\nThis project uses the [Poetry](https://python-poetry.org) dependency and virtualenv manager.\n\nYou will also need:\n\n- Python 3.6+\n- Make\n\n### Setup\n\n- Clone the repository from GitHub to a folder on your local machine\n- `cd` to that folder, and tell Poetry to install dependencies and set up a virtualenv `poetry install`\n- You can now enter the virtual environment using `poetry shell` and develop using your IDE of choice.\n\n### Tests\n\nThe full type, test and lint suite can be run using make: `make`.\n\nYou can also run parts of the suite.\n\n- Unit tests: `make test`\n- Unit tests with HTML coverage: `make test-cov`\n- Linting: `make lint`\n- Static type checks: `make type`\n\n### Adding camera calibrations\n\nYou will need to print off a [chAruco marker grid](https://docs.opencv.org/4.5.3/charuco_board.png).\n\n`opencv_interactive-calibration -t=charuco -sz=GRID_SIZE`\n\nReplace GRID_SIZE with the length of one of the larger squares (in mm) from the printed marker grid.\n\nUse `-ci=1` for specifying camera index if multiple cameras are connected.\n\nPoint the camera at the marker grid. Until DF is at or below 30 then press S to save.\nThis will output a `cameraParameters.xml` file. Place this file in `sr/robot3/vision/calibrations` named by the camera model.\n\nYou will need to add a detection strategy for the camera in to `sr/robot3/vision/backend.py`.\n\n## Contributions\n\nThis project is released under the MIT Licence. For more information, please see LICENSE.\n\nThe CONTRIBUTORS file can be generated by executing CONTRIBUTORS.gen. This generated file contains a list of people who have contributed to sr.robot3.\n',
-    'author': 'Student Robotics',
-    'author_email': 'kit-brain@studentrobotics.org',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/srobo/sr-robot3',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
+Student Robotics API for Python 3
 
+This package uses [PEP420](https://www.python.org/dev/peps/pep-0420/)-style namespace packaging.
+
+## Development
+
+### Requirements
+
+This project uses the [Poetry](https://python-poetry.org) dependency and virtualenv manager.
+
+You will also need:
+
+- Python 3.6+
+- Make
+
+### Setup
+
+- Clone the repository from GitHub to a folder on your local machine
+- `cd` to that folder, and tell Poetry to install dependencies and set up a virtualenv `poetry install`
+- You can now enter the virtual environment using `poetry shell` and develop using your IDE of choice.
+
+### Tests
+
+The full type, test and lint suite can be run using make: `make`.
+
+You can also run parts of the suite.
+
+- Unit tests: `make test`
+- Unit tests with HTML coverage: `make test-cov`
+- Linting: `make lint`
+- Static type checks: `make type`
+
+### Adding camera calibrations
+
+You will need to print off a [chAruco marker grid](https://docs.opencv.org/4.5.3/charuco_board.png).
+
+`opencv_interactive-calibration -t=charuco -sz=GRID_SIZE`
+
+Replace GRID_SIZE with the length of one of the larger squares (in mm) from the printed marker grid.
+
+Use `-ci=1` for specifying camera index if multiple cameras are connected.
+
+Point the camera at the marker grid. Until DF is at or below 30 then press S to save.
+This will output a `cameraParameters.xml` file. Place this file in `sr/robot3/vision/calibrations` named by the camera model.
+
+You will need to add a detection strategy for the camera in to `sr/robot3/vision/backend.py`.
+
+## Contributions
+
+This project is released under the MIT Licence. For more information, please see LICENSE.
+
+The CONTRIBUTORS file can be generated by executing CONTRIBUTORS.gen. This generated file contains a list of people who have contributed to sr.robot3.
 
-setup(**setup_kwargs)
```

