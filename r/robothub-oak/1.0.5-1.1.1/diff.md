# Comparing `tmp/robothub_oak-1.0.5.tar.gz` & `tmp/robothub_oak-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robothub_oak-1.0.5.tar", last modified: Tue Apr 18 09:09:32 2023, max compression
+gzip compressed data, was "robothub_oak-1.1.1.tar", last modified: Tue May  9 09:53:21 2023, max compression
```

## Comparing `robothub_oak-1.0.5.tar` & `robothub_oak-1.1.1.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:09:32.293018 robothub_oak-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-18 09:09:32.293018 robothub_oak-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:09:32.293018 robothub_oak-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:09:32.289018 robothub_oak-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:09:32.289018 robothub_oak-1.0.5/src/robothub_oak/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/app.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2225 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:09:32.293018 robothub_oak-1.0.5/src/robothub_oak/components/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/components/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/components/imu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/components/neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/components/stereo.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/components/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/device.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13321 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/hub_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7990 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/src/robothub_oak/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:09:32.289018 robothub_oak-1.0.5/src/robothub_oak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-18 09:09:32.000000 robothub_oak-1.0.5/src/robothub_oak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-18 09:09:32.000000 robothub_oak-1.0.5/src/robothub_oak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:09:32.000000 robothub_oak-1.0.5/src/robothub_oak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 09:09:32.000000 robothub_oak-1.0.5/src/robothub_oak.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:09:32.293018 robothub_oak-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/tests/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/tests/test_hub_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:09:03.000000 robothub_oak-1.0.5/tests/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:53:21.151706 robothub_oak-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-09 09:53:21.151706 robothub_oak-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:53:21.151706 robothub_oak-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:53:21.139706 robothub_oak-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:53:21.147706 robothub_oak-1.1.1/src/robothub_oak/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:53:21.151706 robothub_oak-1.1.1/src/robothub_oak/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/components/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/components/imu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/components/neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/components/stereo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/components/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/device.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13350 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/hub_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8615 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/src/robothub_oak/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:53:21.147706 robothub_oak-1.1.1/src/robothub_oak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-09 09:53:21.000000 robothub_oak-1.1.1/src/robothub_oak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-09 09:53:21.000000 robothub_oak-1.1.1/src/robothub_oak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:53:21.000000 robothub_oak-1.1.1/src/robothub_oak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 09:53:21.000000 robothub_oak-1.1.1/src/robothub_oak.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:53:21.151706 robothub_oak-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/tests/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/tests/test_hub_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:52:40.000000 robothub_oak-1.1.1/tests/test_manager.py
```

### Comparing `robothub_oak-1.0.5/LICENSE` & `robothub_oak-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.0.5/PKG-INFO` & `robothub_oak-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub_oak
-Version: 1.0.5
+Version: 1.1.1
 Summary: RobotHub-OAK integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub-oak/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub_oak-1.0.5/README.md` & `robothub_oak-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.0.5/setup.py` & `robothub_oak-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 long_description = io.open('README.md', encoding='utf-8').read()
 
 setup(
     name='robothub_oak',
-    version='1.0.5',
+    version='1.1.1',
     description='RobotHub-OAK integration library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.luxonis.com/',
     license='MIT',
     keywords='robothub robot hub connect agent depthai oak sdk',
     author='Luxonis',
```

### Comparing `robothub_oak-1.0.5/src/robothub_oak/callbacks.py` & `robothub_oak-1.1.1/src/robothub_oak/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     Default callback for encoded streams.
 
     :param stream_handle: StreamHandle instance to publish the data to.
     :param packet: Packet instance containing the data.
     """
 
     timestamp = int(time.time() * 1_000)
-    frame_bytes = bytes(packet.imgFrame.getData())
+    frame_bytes = bytes(packet.msg.getData())
     stream_handle.publish_video_data(frame_bytes, timestamp, None)
 
 
 def _default_nn_callback(stream_handle: StreamHandle, packet):
     """
     Default callback for NN streams.
 
@@ -66,9 +66,9 @@
         visualizer.reset()
 
         # temp fix to replace None value that causes errors on frontend
         if not metadata['config']['detection']['color']:
             metadata['config']['detection']['color'] = [255, 0, 0]
 
     timestamp = int(time.time() * 1_000)
-    frame_bytes = bytes(packet.imgFrame.getData())
+    frame_bytes = bytes(packet.msg.getData())
     stream_handle.publish_video_data(frame_bytes, timestamp, metadata)
```

### Comparing `robothub_oak-1.0.5/src/robothub_oak/commands.py` & `robothub_oak-1.1.1/src/robothub_oak/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import asdict
 from typing import Callable
 
 import depthai_sdk.classes.packets as packets
 
 from robothub_oak.components.camera import Camera
 from robothub_oak.components.neural_network import NeuralNetwork
-from robothub_oak.components.stereo import Stereo
+from robothub_oak.components.stereo import Stereo, DepthQuality, DepthRange
 from robothub_oak.hub_camera import HubCamera
 from robothub_oak.packets import HubPacket, DetectionPacket, TrackerPacket, DepthPacket, IMUPacket
 
 __all__ = [
     'CreateCameraCommand',
     'CreateNeuralNetworkCommand',
     'CreateStereoCommand',
@@ -123,14 +123,33 @@
     def execute(self) -> None:
         left = self._stereo.left_camera.camera_component if self._stereo.left_camera else None
         right = self._stereo.right_camera.camera_component if self._stereo.right_camera else None
         stereo_component = self.hub_camera.create_stereo(resolution=self._stereo.resolution,
                                                          fps=self._stereo.fps,
                                                          left=left,
                                                          right=right)
+
+        # Configure stereo component
+        stereo_quality = self._stereo.quality
+        stereo_range = self._stereo.range
+
+        align = self._stereo.align
+        median = 5 if stereo_quality is DepthQuality.DEFAULT else None
+        lr_check = stereo_quality is not DepthQuality.FAST
+        subpixel = stereo_quality is DepthQuality.QUALITY
+        extended_disparity = stereo_range is DepthRange.LONG
+        if extended_disparity:
+            subpixel = False
+
+        stereo_component.config_stereo(align=align,
+                                       lr_check=lr_check,
+                                       subpixel=subpixel,
+                                       median=median,
+                                       extended=extended_disparity)
+
         self._stereo.stereo_component = stereo_component
 
     def get_component(self) -> Stereo:
         return self._stereo
 
 
 class StreamCommand(Command):
```

### Comparing `robothub_oak-1.0.5/src/robothub_oak/components/camera.py` & `robothub_oak-1.1.1/src/robothub_oak/components/camera.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from robothub_oak.components.streamable import Streamable
 
 __all__ = ['Camera']
 
 
 @dataclass
 class CameraConfig:
+    """
+    Dataclass representing the configuration of the camera.
+    """
     interleaved: Optional[bool] = None
     color_order: Union[None, dai.ColorCameraProperties.ColorOrder, str] = None
     manual_focus: Optional[int] = None
     af_mode: Optional[dai.CameraControl.AutoFocusMode] = None
     awb_mode: Optional[dai.CameraControl.AutoWhiteBalanceMode] = None
     scene_mode: Optional[dai.CameraControl.SceneMode] = None
     anti_banding_mode: Optional[dai.CameraControl.AntiBandingMode] = None
@@ -21,15 +24,19 @@
     isp_scale: Optional[Tuple[int, int]] = None
     sharpness: Optional[int] = None
     luma_denoise: Optional[int] = None
     chroma_denoise: Optional[int] = None
 
 
 class Camera(Streamable):
-    def __init__(self, name: str, resolution: str, fps: int) -> None:
+    """
+    This component represents a single camera on the OAK, either color or mono one.
+    The API provides a way to configure the camera, but it is not required to do so.
+    """
+    def __init__(self, name: str, resolution: Optional[str], fps: Optional[int]) -> None:
         super().__init__()
         self.name = name
         self.resolution = resolution
         self.fps = fps
 
         self.camera_component = None  # type: depthai_sdk.components.CameraComponent
         self.camera_config = CameraConfig()
@@ -45,19 +52,38 @@
                   anti_banding_mode: Optional[dai.CameraControl.AntiBandingMode] = None,
                   effect_mode: Optional[dai.CameraControl.EffectMode] = None,
                   # IQ settings
                   isp_scale: Optional[Tuple[int, int]] = None,
                   sharpness: Optional[int] = None,
                   luma_denoise: Optional[int] = None,
                   chroma_denoise: Optional[int] = None,
-                  ):
+                  ) -> None:
+        """
+        Configures the camera component.
+        """
         kwargs = self._process_kwargs(locals())
 
         if len(kwargs) > 0:
             self.camera_config = replace(self.camera_config, **kwargs)
 
+    def set_resolution(self, resolution: str) -> None:
+        """
+        Sets the resolution of the camera.
+
+        :param resolution: String representation of the resolution, e.g. '1080p' or '4K'.
+        """
+        self.resolution = resolution
+
+    def set_fps(self, fps: int) -> None:
+        """
+        Sets the FPS of the camera.
+
+        :param fps: FPS to set as an integer.
+        """
+        self.fps = fps
+
     @staticmethod
     def _process_kwargs(kwargs: Dict[str, Any]) -> Dict[str, Any]:
         """Process the kwargs and remove all None values."""
         kwargs.pop('self')
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
         return kwargs
```

### Comparing `robothub_oak-1.0.5/src/robothub_oak/components/neural_network.py` & `robothub_oak-1.1.1/src/robothub_oak/components/neural_network.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.0.5/src/robothub_oak/device.py` & `robothub_oak-1.1.1/src/robothub_oak/device.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import Callable, Any, Optional
+from typing import Callable, Any, Optional, Dict
 
 from depthai import NNData
 
 from robothub_oak.commands import (
     CreateStereoCommand, CreateCameraCommand, CreateNeuralNetworkCommand,
     StreamCommand, CommandHistory
 )
@@ -26,35 +26,51 @@
         """
         :param id: ID of the device.
         :param name: Name of the device.
         :param mxid: MXID of the device.
         :param ip_address: IP address of the device.
         """
         # Device info
-        self.id = id
-        self.name = name
-        self.mxid = mxid
-        self.ip_address = ip_address
+        self.id = id  # device identifier provided by the user
+        self.name = name  # product name
+        self.mxid = mxid  # mxid of the device
+        self.ip_address = ip_address  # IP address of the device
+
+        self.cameras: Dict[str, Camera] = {}
+        self.stereo: Optional[Stereo] = None
+        self.neural_networks: Dict[str, NeuralNetwork] = {}
+
+        self.hub_camera: Optional[HubCamera] = None
 
         # Callbacks
-        self.disconnect_callback = lambda x: None  # type: Callable[[Any], None]
-        self.connect_callback = lambda x: None  # type: Callable[[Any], None]
+        self.disconnect_callback: Callable[[Any], None] = lambda x: None
+        self.connect_callback: Callable[[Any], None] = lambda x: None
 
         self._command_history = CommandHistory()
 
+    def __eq__(self, other):
+        if isinstance(other, Device):
+            return self.id == other.id or self.name == other.name or self.mxid == other.mxid or self.ip_address == other.ip_address
+        elif isinstance(other, str):
+            return self.id == other or self.name == other or self.mxid == other or self.ip_address == other
+        else:
+            return False
+
     def _start(self, hub_camera: HubCamera) -> bool:
         """
         Internal method to execute all commands.
 
         :param hub_camera: The HubCamera instance to use.
         :return: True if successful, False otherwise.
         """
         if hub_camera.oak_camera is None:
             return False
 
+        self.hub_camera = hub_camera
+
         try:
             for command in self._command_history:
                 if isinstance(command, CreateStereoCommand) and not hub_camera.has_stereo:
                     warnings.warn(f'Device {self.get_device_name()} does not support stereo, skipping stereo creation.')
                     continue
 
                 command.set_camera(hub_camera)
@@ -75,31 +91,54 @@
             if isinstance(component, Streamable) and component.stream_enabled:
                 stream_command = StreamCommand(self, command)
                 stream_command.set_camera(hub_camera)
                 stream_command.execute()
 
         return True
 
-    def get_camera(self, name: str, resolution: str, fps: int) -> Camera:
+    def restart(self) -> bool:
+        """
+        Restarts the device. This will stop all components and streams and recreate them.
+
+        :return: True if successful, False otherwise.
+        """
+        try:
+            if self.hub_camera:
+                self.hub_camera.stop()
+                self.hub_camera.oak_camera = self.hub_camera.init_oak_camera()
+                self._start(hub_camera=self.hub_camera)
+        except Exception as e:
+            warnings.warn(f'Failed to restart device {self.get_device_name()} with error: {e}')
+            return False
+
+        return True
+
+    def get_camera(self, name: str, resolution: str = None, fps: int = None) -> Camera:
         """
         Creates a camera component.
 
         :param name: The name of the camera.
         :param resolution: The resolution of the camera.
         :param fps: The FPS of the camera.
         :return: The camera.
         """
+        # Check if camera already exists
+        if name in self.cameras:
+            return self.cameras[name]
+
         camera = Camera(name, resolution, fps)
+        self.cameras[name] = camera
+
         command = CreateCameraCommand(self, camera)
         self._command_history.push(command)
         return camera
 
     def create_neural_network(self,
                               name: str,
-                              input: Camera,
+                              input: Camera = None,
                               nn_type: str = None,
                               decode_fn: Callable[[NNData], Any] = None,
                               tracker: bool = False,
                               spatial: Optional[bool] = None
                               ) -> NeuralNetwork:
         """
         Creates a neural network.
@@ -108,48 +147,68 @@
         :param input: The input camera.
         :param nn_type: The type of neural network. Either 'yolo' or 'mobilenet'.
         :param decode_fn: The decode function to use. Decoding is done on the host.
         :param tracker: Whether to use tracking.
         :param spatial: Whether to use spatial detection.
         :return: The neural network.
         """
+        if name in self.neural_networks:
+            return self.neural_networks[name]
+        elif not input:
+            raise ValueError('Neural network must have an input')
+
         if isinstance(input, NeuralNetwork):
             raise NotImplementedError('Neural networks cannot be used as input for other neural networks yet')
 
-        neural_network = NeuralNetwork(name=name, input=input, nn_type=nn_type, decode_fn=decode_fn,
-                                       tracker=tracker, spatial=spatial)
+        neural_network = NeuralNetwork(name=name,
+                                       input=input,
+                                       nn_type=nn_type,
+                                       decode_fn=decode_fn,
+                                       tracker=tracker,
+                                       spatial=spatial)
         command = CreateNeuralNetworkCommand(self, neural_network)
         self._command_history.push(command)
         return neural_network
 
-    def get_stereo_camera(self, resolution: str, fps: int, left_camera: Camera = None, right_camera: Camera = None):
+    def get_stereo_camera(self,
+                          resolution: str = None,
+                          fps: int = None,
+                          left_camera: Camera = None,
+                          right_camera: Camera = None
+                          ) -> Stereo:
         """
         Creates a stereo component.
 
         :param resolution: The resolution of the stereo camera.
         :param fps: The FPS of the stereo camera.
+        :param left_camera: The left camera.
+        :param right_camera: The right camera.
         """
-        stereo = Stereo(resolution, fps, left_camera, right_camera)
-        command = CreateStereoCommand(self, stereo)
+        if self.stereo:
+            return self.stereo
+
+        self.stereo = Stereo(resolution, fps, left_camera, right_camera)
+        command = CreateStereoCommand(self, self.stereo)
         self._command_history.push(command)
-        return stereo
+        return self.stereo
 
     def set_connect_callback(self, callback: Callable[[HubCamera], None]) -> None:
         """
         Sets the callback to be called when the device connects.
 
         :param callback: The callback to be called when the device connects.
-        :return: None
         """
         self.connect_callback = callback
 
     def set_disconnect_callback(self, callback: Callable[[HubCamera], None]) -> None:
         """
         Sets the callback to be called when the device disconnects.
 
         :param callback: The callback to be called when the device disconnects.
-        :return: None
         """
         self.disconnect_callback = callback
 
-    def get_device_name(self):
-        return self.id or self.name or self.mxid or self.ip_address
+    def get_device_name(self) -> str:
+        """
+        Returns the name of the device.
+        """
+        return self.id or self.name or self.ip_address or self.mxid
```

### Comparing `robothub_oak-1.0.5/src/robothub_oak/hub_camera.py` & `robothub_oak-1.1.1/src/robothub_oak/hub_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,28 +34,29 @@
         self.state = robothub.DeviceState.UNKNOWN
         self.device_name = device_name
         self.usb_speed = usb_speed
         self.rotation = rotation
 
         self.stop_event = robothub.threading.Event()
         self.streams = {}  # unique_key -> StreamHandle
+        self.available_sensors = []  # self.oak_camera.sensors if self.oak_camera else []
 
-        self.oak_camera = self._init_oak_camera()
-        self.available_sensors = self.oak_camera.sensors if self.oak_camera else []
+        self.oak_camera = self.init_oak_camera()
 
-    def _init_oak_camera(self) -> Optional[OakCamera]:
+    def init_oak_camera(self) -> Optional[OakCamera]:
         """
         Initializes the OakCamera instance. Will try to initialize for 5 seconds before returning None.
 
         :return: OakCamera instance if successful, None otherwise.
         """
         start_time = time.time()
         while not self.stop_event.is_set():
             try:
                 camera = OakCamera(self.device_name, usb_speed=self.usb_speed, rotation=self.rotation)
+                self.available_sensors = camera.sensors
                 return camera
             except Exception:
                 if time.time() - start_time > 10:
                     break
 
                 self.stop_event.wait(1)
 
@@ -90,17 +91,17 @@
         """
         Creates a neural network component.
 
         :param model: Name or path to the model.
         :param input: Input component, either a camera or another neural network.
         :param nn_type: Either 'yolo' or 'mobilenet'. For other types, use None.
         :param tracker: If True, will enable and add a tracker to the output.
-        :param spatial: If True, will enable and add spatial data to the output. If a StereoComponent is provided,
-                        will use that component to calculate the spatial data.
+        :param spatial: If True, will enable and add spatial data to the output. If a StereoComponent is provided, will use that component to calculate the spatial data.
         :param decode_fn: Function to decode the output of the neural network.
+
         :return: Neural network component.
         """
         comp = self.oak_camera.create_nn(model=model, input=input, nn_type=nn_type,
                                          tracker=tracker, spatial=spatial, decode_fn=decode_fn)
         return comp
 
     def create_stereo(self,
@@ -161,15 +162,14 @@
                              ) -> None:
         """
         Selects the correct callback function for the given component and adds it to the stream.
 
         :param stream_handle: Stream handle to add the callback to.
         :param component: Component to create a callback for.
         :param callback: User-defined callback function to be called when a new frame is received.
-        :return: None
         """
         fn = None
         enable_visualizer = False
         if isinstance(component, CameraComponent):
             fn = callback or get_default_color_callback(stream_handle)
         elif isinstance(component, NNComponent):
             fn = callback or get_default_nn_callback(stream_handle)
@@ -183,15 +183,14 @@
     def callback(self, output: Any, callback: Callable, enable_visualizer: bool = False) -> None:
         """
         Sets a callback function for the given output.
 
         :param output: Output to set the callback for.
         :param callback: Callback function to be called when a new frame is received.
         :param enable_visualizer: Whether to enable the visualizer that provides metadata.
-        :return: None
         """
         self.oak_camera.callback(output, callback=callback, enable_visualizer=enable_visualizer)
 
     def poll(self) -> Optional[int]:
         """
         Polls the device for new data.
         """
@@ -231,14 +230,15 @@
 
         self.streams.clear()
 
         if self.oak_camera:
             self.oak_camera.device.close()
 
         self.oak_camera = None
+        self.available_sensors = []
 
     def stats_report(self) -> Dict[str, Any]:
         """
         Returns a dictionary with statistics about the device.
         """
         stats = {'mxid': self.device.getMxId()}
```

### Comparing `robothub_oak-1.0.5/src/robothub_oak/manager.py` & `robothub_oak-1.1.1/src/robothub_oak/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import contextlib
 import logging
 import logging as log
 import os
+from collections import defaultdict
 from typing import Optional, List
 
 import robothub
 
 from robothub_oak.device import Device
 from robothub_oak.hub_camera import HubCamera
 
 __all__ = ['DeviceManager', 'DEVICE_MANAGER']
 
 
-class NoDevicesException(Exception):
-    pass
-
-
 class DeviceManager:
     """
     A manager class to handle multiple HubCamera instances.
     """
     REPORT_FREQUENCY = 10  # seconds
     POLL_FREQUENCY = 0.0005
 
@@ -54,14 +51,15 @@
 
         self.reporting_thread.start()
         log.info('Reporting thread: started successfully.')
 
         self.polling_thread.start()
         log.info('Polling thread: started successfully.')
 
+        # Endless loop to prevent app from exiting, keeps the main thread alive
         while not self.stop_event.is_set():
             self.stop_event.wait(60)
 
     def stop(self) -> None:
         """
         Stop the cameras, stop reporting and polling threads.
         """
@@ -212,29 +210,46 @@
         :param mxid: The mxid of the device.
         :param ip_address: The IP address of the device.
         :return: The device.
         """
         assert id or name or mxid or ip_address, 'Must specify at least one of id, name, mxid or ip_address'
 
         device = Device(id=id, name=name, mxid=mxid, ip_address=ip_address)
-        if device not in DEVICE_MANAGER.devices:
-            DEVICE_MANAGER.add_device(device)
+        device_name = device.get_device_name()
+
+        # Check if device already exists
+        for d in DEVICE_MANAGER.devices:
+            if d == device_name:
+                return d
+
+        # Add device to device manager if it doesn't exist
+        DEVICE_MANAGER.add_device(device)
         return device
 
     @staticmethod
     def get_all_devices() -> List[Device]:
         """
         Returns all devices.
 
         :return: All devices.
         """
         devices = []
         for obj in robothub.DEVICES:
-            device = Device(mxid=obj.oak['serialNumber'])
-            if device not in DEVICE_MANAGER.devices:
-                DEVICE_MANAGER.add_device(device)
-            devices.append(device)
+            device_dict = defaultdict(lambda: None, obj.oak)
+            device = Device(mxid=device_dict['serialNumber'],
+                            name=device_dict['productName'],
+                            id=device_dict['name'],
+                            ip_address=device_dict['ipAddress'])
+
+            exists = False
+            for d in DEVICE_MANAGER.devices:
+                if d == device:
+                    exists = True
+                    break
+
+            if not exists:
+                devices.append(device)
 
         return devices
 
 
-DEVICE_MANAGER = DeviceManager()
+DEVICE_MANAGER = DeviceManager()  # Global device manager
```

### Comparing `robothub_oak-1.0.5/src/robothub_oak/packets.py` & `robothub_oak-1.1.1/src/robothub_oak/packets.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,25 +17,22 @@
 
     def __init__(self, device: 'Device', packet):
         self.device = device
         self._packet = packet
 
         self.frame = self._packet.frame
 
-    def upload_as_detection(self, title: str):
+    def upload_as_event(self, title: str):
         try:
             # convert numpy array to jpg
             frame_bytes = cv2.imencode('.jpg', self._packet.frame)[1].tobytes()
             robothub.DETECTIONS.send_frame_detection(imagedata=frame_bytes, title=title, camera_serial=self.device.mxid)
         except Exception as e:
             warnings.warn(f'Could not upload detection with error: {e}')
 
-    def upload_as_event(self, title):
-        raise NotImplementedError('Not implemented yet')
-
 
 class DepthPacket(HubPacket):
     def __init__(self, device: 'Device', packet):
         super().__init__(device, packet)
 
     def upload_as_event(self, title):
         raise NotImplementedError('Not implemented yet')
```

### Comparing `robothub_oak-1.0.5/src/robothub_oak.egg-info/PKG-INFO` & `robothub_oak-1.1.1/src/robothub_oak.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub-oak
-Version: 1.0.5
+Version: 1.1.1
 Summary: RobotHub-OAK integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub-oak/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub_oak-1.0.5/src/robothub_oak.egg-info/SOURCES.txt` & `robothub_oak-1.1.1/src/robothub_oak.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 src/robothub_oak/__init__.py
-src/robothub_oak/app.py
 src/robothub_oak/callbacks.py
 src/robothub_oak/commands.py
 src/robothub_oak/device.py
 src/robothub_oak/hub_camera.py
 src/robothub_oak/manager.py
 src/robothub_oak/packets.py
 src/robothub_oak/utils.py
@@ -17,11 +16,10 @@
 src/robothub_oak.egg-info/top_level.txt
 src/robothub_oak/components/__init__.py
 src/robothub_oak/components/camera.py
 src/robothub_oak/components/imu.py
 src/robothub_oak/components/neural_network.py
 src/robothub_oak/components/stereo.py
 src/robothub_oak/components/streamable.py
-tests/test_app.py
 tests/test_callback.py
 tests/test_hub_camera.py
 tests/test_manager.py
```

