# Comparing `tmp/mera-1.3.1-py3-none-manylinux_2_27_x86_64.whl.zip` & `tmp/mera-1.4.0-py3-none-manylinux_2_27_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,30 @@
-Zip file size: 58215 bytes, number of entries: 19
--rw-r--r--  2.0 unx     1274 b- defN 23-Feb-22 08:42 mera/__init__.py
--rw-r--r--  2.0 unx     7031 b- defN 23-Feb-22 08:42 mera/deploy.py
--rw-r--r--  2.0 unx     7215 b- defN 23-Feb-22 08:42 mera/deploy_project.py
--rw-r--r--  2.0 unx     6613 b- defN 23-Feb-22 08:42 mera/mera_deployment.py
--rw-r--r--  2.0 unx    13802 b- defN 23-Feb-22 08:42 mera/mera_model.py
--rw-r--r--  2.0 unx     1301 b- defN 23-Feb-22 08:42 mera/mera_platform.py
--rw-r--r--  2.0 unx    16494 b- defN 23-Feb-22 08:42 mera/mera_quantizer.py
--rw-r--r--  2.0 unx    10078 b- defN 23-Feb-22 08:42 mera/quantization_quality.py
--rw-r--r--  2.0 unx     2171 b- defN 23-Feb-22 08:42 mera/version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-22 08:42 mera/bin_utils/__init__.py
--rwxr-xr-x  2.0 unx    47480 b- defN 23-Feb-22 08:48 mera/bin_utils/intel_get_board_id
--rw-r--r--  2.0 unx      648 b- defN 23-Feb-22 08:42 mera/model/__init__.py
--rw-r--r--  2.0 unx     4098 b- defN 23-Feb-22 08:42 mera/model/input_desc.py
--rwxr-xr-x  2.0 unx     1238 b- defN 23-Feb-22 09:01 mera-1.3.1.data/scripts/mera
--rw-rw----  2.0 unx    13101 b- defN 23-Feb-22 09:01 mera-1.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    17243 b- defN 23-Feb-22 09:01 mera-1.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Feb-22 09:01 mera-1.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Feb-22 09:01 mera-1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1483 b- defN 23-Feb-22 09:01 mera-1.3.1.dist-info/RECORD
-19 files, 151385 bytes uncompressed, 55837 bytes compressed:  63.1%
+Zip file size: 637848 bytes, number of entries: 28
+-rw-r--r--  2.0 unx     1323 b- defN 23-May-09 07:52 mera/__init__.py
+-rw-r--r--  2.0 unx     7012 b- defN 23-May-09 07:52 mera/deploy.py
+-rw-r--r--  2.0 unx     7443 b- defN 23-May-09 07:52 mera/deploy_project.py
+-rw-r--r--  2.0 unx     8404 b- defN 23-May-09 07:52 mera/mera_deployment.py
+-rw-r--r--  2.0 unx    13802 b- defN 23-May-09 07:52 mera/mera_model.py
+-rw-r--r--  2.0 unx     1335 b- defN 23-May-09 07:52 mera/mera_platform.py
+-rw-r--r--  2.0 unx    16494 b- defN 23-May-09 07:52 mera/mera_quantizer.py
+-rw-r--r--  2.0 unx    10078 b- defN 23-May-09 07:52 mera/quantization_quality.py
+-rw-r--r--  2.0 unx     2171 b- defN 23-May-09 07:52 mera/version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-09 07:52 mera/app/__init__.py
+-rw-r--r--  2.0 unx     4124 b- defN 23-May-09 07:52 mera/app/mera.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-09 07:52 mera/bin_utils/__init__.py
+-rwxrwx---  2.0 unx    21456 b- defN 23-May-09 07:52 mera/bin_utils/ec_dma_daemon_proc
+-rw-rw----  2.0 unx   492584 b- defN 23-May-09 07:52 mera/bin_utils/ifc_uio_5.15.0-56-generic.ko
+-rwxr-xr-x  2.0 unx    47480 b- defN 23-May-09 07:57 mera/bin_utils/intel_get_board_id
+-rw-rw----  2.0 unx   544656 b- defN 23-May-09 07:52 mera/bin_utils/pcie_sakura_5.15.0-69-generic.ko
+-rw-rw----  2.0 unx   544936 b- defN 23-May-09 07:52 mera/bin_utils/pcie_sakura_5.15.0-71-generic.ko
+-rwxr-xr-x  2.0 unx   257320 b- defN 23-May-09 07:57 mera/bin_utils/sakura_ddr_init
+-rw-r--r--  2.0 unx        0 b- defN 23-May-09 07:52 mera/metrics/__init__.py
+-rw-r--r--  2.0 unx     2869 b- defN 23-May-09 07:52 mera/metrics/power_metrics.py
+-rw-r--r--  2.0 unx      648 b- defN 23-May-09 07:52 mera/model/__init__.py
+-rw-r--r--  2.0 unx     4098 b- defN 23-May-09 07:52 mera/model/input_desc.py
+-rw-rw----  2.0 unx    13101 b- defN 23-May-09 08:06 mera-1.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    16758 b- defN 23-May-09 08:06 mera-1.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-09 08:06 mera-1.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 23-May-09 08:06 mera-1.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-May-09 08:06 mera-1.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2295 b- defN 23-May-09 08:06 mera-1.4.0.dist-info/RECORD
+28 files, 2020547 bytes uncompressed, 634190 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -21,38 +21,65 @@
 
 Filename: mera/quantization_quality.py
 Comment: 
 
 Filename: mera/version.py
 Comment: 
 
+Filename: mera/app/__init__.py
+Comment: 
+
+Filename: mera/app/mera.py
+Comment: 
+
 Filename: mera/bin_utils/__init__.py
 Comment: 
 
+Filename: mera/bin_utils/ec_dma_daemon_proc
+Comment: 
+
+Filename: mera/bin_utils/ifc_uio_5.15.0-56-generic.ko
+Comment: 
+
 Filename: mera/bin_utils/intel_get_board_id
 Comment: 
 
+Filename: mera/bin_utils/pcie_sakura_5.15.0-69-generic.ko
+Comment: 
+
+Filename: mera/bin_utils/pcie_sakura_5.15.0-71-generic.ko
+Comment: 
+
+Filename: mera/bin_utils/sakura_ddr_init
+Comment: 
+
+Filename: mera/metrics/__init__.py
+Comment: 
+
+Filename: mera/metrics/power_metrics.py
+Comment: 
+
 Filename: mera/model/__init__.py
 Comment: 
 
 Filename: mera/model/input_desc.py
 Comment: 
 
-Filename: mera-1.3.1.data/scripts/mera
+Filename: mera-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: mera-1.3.1.dist-info/LICENSE
+Filename: mera-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: mera-1.3.1.dist-info/METADATA
+Filename: mera-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: mera-1.3.1.dist-info/WHEEL
+Filename: mera-1.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: mera-1.3.1.dist-info/top_level.txt
+Filename: mera-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mera-1.3.1.dist-info/RECORD
+Filename: mera-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mera/__init__.py

```diff
@@ -30,7 +30,9 @@
 except ModuleNotFoundError:
     pass
 
 
 from .quantization_quality import QuantizationQualityMetrics, calculate_quantization_quality
 
 from .model.input_desc import InputDescription, InputDescriptionContainer
+
+from .metrics.power_metrics import PowerMetrics
```

## mera/deploy.py

```diff
@@ -43,34 +43,34 @@
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.prj._unlock()
 
 
 class TVMDeployer(_DeployerBase):
-    """Using Mera deployer targetting the TVM compiler stack:"""
+    """Using MERA deployer targetting the TVM compiler stack:"""
 
     def _save_compile_metrics(self, compile_time):
         metrics = {}
         metrics['compile_time'] = compile_time
         metrics['compile_date'] = date.today().strftime("%d/%m/%Y")
         # TODO - Add more metrics
         self.prj.save_artifact('compile_metrics.json', ArtifactFileType.JSON, 'metrics', metrics)
 
     def deploy(self, model : MeraModel, mera_platform : Platform = Platform.DNAF200L0003, build_config = {},
         target : Target = Target.Simulator, host_arch : str = None) -> MeraTvmDeployment:
-        """Launches the compilation of a Mera project for a Mera model using the TVM stack.
+        """Launches the compilation of a MERA project for a MERA model using the TVM stack.
 
         :param model: Model object loaded from mera.ModelLoader
-        :param mera_platform: Mera platform architecture enum value
-        :param build_config: Mera build configuration dict
-        :param target: Mera build target
+        :param mera_platform: MERA platform architecture enum value
+        :param build_config: MERA build configuration dict
+        :param target: MERA build target
         :param host_arch: Host arch to deploy for. If unset, it will pick the current host platform, 
             provide a value to override the setting
-        :return: The object representing the result of a Mera deployment
+        :return: The object representing the result of a MERA deployment
         """
         if not isinstance(model, MeraModel):
             raise ValueError(f'Model is not of MeraModel type.')
 
         if isinstance(target, str):
             target = Target[target]
         elif not isinstance(target, Target):
@@ -118,15 +118,15 @@
         self.prj.save_artifact('mera_cfg.json', ArtifactFileType.JSON, target_str, mera_compiler_cfg)
         mod, params = model._load_model_tvm()
         mera_compiler_cfg['target'] = target_str
         with _mera.build_config(**mera_compiler_cfg):
             logger.info(f'Compiling Mera model...')
             self.prj.pushd('result')
             tm_start = time.time()
-            if target_str == Target.Interpreter.str_val:
+            if target.uses_fp32_flow:
                 _mera.build_fp32(mod, params, target_str, host_arch=host_arch, output_dir=self.prj.get_cwd())
             else:
                 _mera.build(mod, params, output_dir=self.prj.get_cwd(),
                     host_arch=host_arch, layout='NHWC', aux_config=model._get_mera_aux_config())
             tm_end = time.time()
             to_target_artifact = lambda a : (target_str, self.prj.get_cwd() / a)
             self.prj.add_artifact([to_target_artifact(x) for x in ['deploy.so', 'deploy.json', 'deploy.params']])
```

## mera/deploy_project.py

```diff
@@ -33,23 +33,25 @@
     BIN  = "binary"
     TXT  = "text"
     FILE = "file"
 
 
 class Target(Enum):
     """List of possible Mera Target values."""
-    IP = ("IP", False)                                #: Target HW accelerator. Valid for `arm` and `x86` architectures.
-    Interpreter = ("Interpreter", True)               #: Target sw interpretation of the model in floating point. Only valid for `x86`
-    InterpreterHw = ("InterpreterHw", True)           #: Target sw interpretation of the model. Only valid for `x86`
-    Simulator = ("Simulator", True)                   #: Target sw simulation of the IP model. Only valid for `x86`
-    VerilatorSimulator = ("VerilatorSimulator", True) #: Target hw emulation of the IP model. Only valid for `x86`
+    IP = ("IP", False, False)                                #: Target HW accelerator. Valid for `arm` and `x86` architectures.
+    Interpreter = ("Interpreter", True, True)                #: Target sw interpretation of the model in floating point. Only valid for `x86`
+    InterpreterHw = ("InterpreterHw", True, False)           #: Target sw interpretation of the model. Only valid for `x86`
+    Simulator = ("Simulator", True, False)                   #: Target sw simulation of the IP model. Only valid for `x86`
+    VerilatorSimulator = ("VerilatorSimulator", True, False) #: Target hw emulation of the IP model. Only valid for `x86`
+    InterpreterHwBf16 = ("InterpreterHwBf16", True, True)    #: Target sw interpretation of the model in BF16. Only valid for `x86`
 
-    def __init__(self, str_val, x86_only):
+    def __init__(self, str_val, x86_only, uses_fp32_flow):
         self.str_val = str_val
         self.x86_only = x86_only
+        self.uses_fp32_flow = uses_fp32_flow
 
     def __str__(self):
         return self.str_val
 
 
 class Layout(Enum):
     """List of possible data layouts"""
```

## mera/mera_deployment.py

```diff
@@ -13,15 +13,17 @@
 # limitations under the License.
 """Mera Deployment classes"""
 
 import numpy as np
 
 from typing import Dict, List, Union
 from pathlib import Path
+from enum import Enum
 from .deploy_project import is_mera_project, _create_mera_project, Target, logger
+from .metrics.power_metrics import PowerMetrics
 
 
 class MeraTvmModelRunner:
     def __init__(self, rt_mod):
         self.rt_mod = rt_mod
 
     def set_input(self, data : Union[np.ndarray, Dict[str, np.ndarray], List[np.ndarray]]):
@@ -72,40 +74,77 @@
     def get_runtime_metrics(self) -> dict:
         """Gets the runtime metrics reported from Mera after a :func:`run()`
 
         :return: Dictionary of measured metrics
         """
         return self.rt_mod.get_runtime_metrics()
 
+    def get_power_metrics(self) -> PowerMetrics:
+        """Gets the power metrics reported from MERA after a :func:`run()`.
+        Note power measurement mode might need to be enable in order to collect and generate such metrics.
+
+        :return: Container with summary analysis of all collected metrics from MERA.
+        """
+        return PowerMetrics(self.rt_mod['get_power_metrics']())
+
+
+class DeviceTarget(Enum):
+    """List of possible MERA runtime devices for running IP deployments."""
+    SAKURA_1 = ("Sakura-1", 1)         #: Target device is an EdgeCortix's Sakura-1 ASIC.
+    XILINX_U50 = ("AMD Xilinx U50", 2) #: Target device is an AMD Xilinx U50 FPGA board.
+    INTEL_IA420 = ("Intel IA420", 3)   #: Target device is an Intel IA420 FPGA board.
+
+    def __init__(self, str_val, code):
+        self.__str_val = str_val
+        self.__code = code
+
+    def __str__(self):
+        return self.__str_val
+
+    @property
+    def code(self):
+        return self.__code
+
 
 class MeraTvmDeployment:
     def __init__(self, lib_path, params_path, lib_json_path):
         self.lib_path = lib_path
         self.params_path = params_path
         self.lib_json_path = lib_json_path
 
-    def get_runner(self, tvm_debug_mode : bool = False, tvm_debug_dump_path : str = None) -> MeraTvmModelRunner:
+    def get_runner(self, device_target : DeviceTarget = DeviceTarget.SAKURA_1,
+            tvm_debug_mode : bool = False, tvm_debug_dump_path : str = None) -> MeraTvmModelRunner:
         """Prepares the model for running with a given target
 
+        :param device_target: Selects the device run target where the IP deployment will be run. Only applicable for deployments
+            with target=IP. See `DeviceTarget` enum for a detailed list of possible values.
         :param tvm_debug_mode: Whether to create this runner with TVM debugger mode or not. This mode allows a breakdown of
             time spent on each node.
         :param tvm_debug_dump_path: When running with TVM debug mode enabled, allows to set up a directory where the debugging
             results will be kept, otherwise they will be sent to a temporary directory.
 
         :return: Runner object
         """
+        if isinstance(device_target, int):
+            _dt_code = device_target
+        else:
+            if not isinstance(device_target, DeviceTarget):
+                raise ValueError(f'device_target argument is not of type DeviceTarget. Got {type(device_target)}')
+            logger.debug(f'Creating TVM model runner for IP device {str(device_target)}')
+            _dt_code = device_target.code
         from tvm.runtime import load_module as __load_module, cpu as __cpu
         if tvm_debug_mode:
             from tvm.contrib.debugger.debug_executor import create as __create
             logger.info(f'Creating TVM model runner in debugger mode')
             rt_mod = __create(self.lib_json_path.read_text(), __load_module(self.lib_path), __cpu(), tvm_debug_dump_path)
         else:
             from tvm.contrib.graph_executor import create as __create
             rt_mod = __create(self.lib_json_path.read_text(), __load_module(self.lib_path), __cpu())
         rt_mod.load_params(self.params_path.read_bytes())
+        rt_mod["mera_runtime_init_device"](_dt_code)
         logger.info(f'Created TVM model runner')
         return MeraTvmModelRunner(rt_mod)
 
 
 class MeraTvmPrjDeployment(MeraTvmDeployment):
     def __init__(self, lib_path, params_path, lib_json_path, prj):
         super().__init__(lib_path, params_path, lib_json_path)
```

## mera/mera_platform.py

```diff
@@ -7,21 +7,21 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Mera platform selection"""
+"""MERA platform selection"""
 
 from enum import Enum
 
 
 class Platform(Enum):
-    """List of all valid Mera platforms"""
+    """List of all valid MERA platforms"""
     DNAF200L0001 = 'DNAF200L0001'
     DNAF200L0002 = 'DNAF200L0002'
     DNAF200L0003 = 'DNAF200L0003'
 
     DNAF100L0001 = 'DNAF100L0001'
     DNAF100L0002 = 'DNAF100L0002'
     DNAF100L0003 = 'DNAF100L0003'
@@ -37,11 +37,12 @@
 
     DNAF300L0001 = 'DNAF300L0001'
 
     DNAA400L0001 = 'DNAA400L0001'
 
     DNAA600L0001 = 'DNAA600L0001'
     DNAA600L0002 = 'DNAA600L0002'
+    SAKURA_1     = 'DNAA600L0002'
 
 
     def __str__(self):
         return self.value
```

## mera/version.py

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 # Current version, modify this file for release using "bump_version.py"
-__version__ = "1.3.1"
-__release_date__ = "13/02/2023"
+__version__ = "1.4.0"
+__release_date__ = "25/04/2023"
 
 def get_mera_tvm_version() -> str:
     """Gets the version string for mera-tvm module
 
     :return: mera-tvm version
     """
     from tvm import __version__ as __tvm_version__
```

## Comparing `mera-1.3.1.dist-info/LICENSE` & `mera-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mera-1.3.1.dist-info/METADATA` & `mera-1.4.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mera
-Version: 1.3.1
+Version: 1.4.0
 Summary: An heterogeneous deep learning compiler framework.
 Home-page: https://github.com/Edgecortix-Inc/mera
 Author: EdgeCortix Inc.
 Author-email: mera-compiler@edgecortix.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Edgecortix-Inc/mera/issues
 Project-URL: Web Page, https://www.edgecortix.com
@@ -26,21 +26,14 @@
 Provides-Extra: full
 Requires-Dist: mera-tvm-full ; extra == 'full'
 Requires-Dist: onednn-cpu-gomp (==2022.0.2) ; extra == 'full'
 Requires-Dist: tensorflow (<=2.9.0) ; extra == 'full'
 Requires-Dist: tflite (==2.4.0) ; extra == 'full'
 Requires-Dist: torch (<=1.12.1) ; extra == 'full'
 Requires-Dist: torchvision (<=0.13.1) ; extra == 'full'
-Provides-Extra: host-only
-Requires-Dist: mera-tvm-host-only ; extra == 'host-only'
-Requires-Dist: onednn-cpu-gomp (==2022.0.2) ; extra == 'host-only'
-Requires-Dist: tensorflow (<=2.9.0) ; extra == 'host-only'
-Requires-Dist: tflite (==2.4.0) ; extra == 'host-only'
-Requires-Dist: torch (<=1.12.1) ; extra == 'host-only'
-Requires-Dist: torchvision (<=0.13.1) ; extra == 'host-only'
 Provides-Extra: runtime
 Requires-Dist: mera-tvm-runtime ; extra == 'runtime'
 
 # EdgeCortix&reg; MERA&trade; - A heterogeneous deep learning compiler framework
 
 This repository contains the source code for the frontend stack of EdgeCortix&reg; MERA™ compiler framework, developed by [EdgeCortix Inc.](https://www.edgecortix.com/). If you are interested in the latest (bleeding edge) capabilities of MERA™ framework and the different Dynamic Neural Accelerator&reg; architecture configurations, contact [EdgeCortix AI Accelerator Team](mailto:dna-ip@edgecortix.com).
 
@@ -100,43 +93,42 @@
 sudo apt install libstdc++6
 ```
 
 #### MERA Installation
 
 The MERA environment provides 3 different modes depending on the target usage:
 
-* `host-only`: Meant for performing deployments only targetting simulation running on the host.
 * `runtime`: Meant for running inference in HW accelerators using the DNA IP, requires extra system dependencies depending on the HW device.
 * `full`: Meant for users who want the functionality of both `host-only` and `runtime` models
 
 MERA pip packages are available for both Python3.6 and Python3.8 variants. Later python versions allow the usage of more up-to-date
 PyTorch and Tensorflow to use for deployments.
 
 After choosing the desired mode, you can install MERA with the following command:
 
 ```bash
 # Create virtual environment with Python 3.6
 MERA_VENV=mera-env
 virtualenv -p python3.6 $MERA_VENV
 source $MERA_VENV/bin/activate
 
-# Install MERA host-only version
+# Install MERA full version
 pip install --upgrade pip
-pip install mera[host-only]
+pip install mera[full]
 
 # Install extra dependencies. These are needed to run our tutorials and demos
 pip install tqdm easydict wget notebook pandas matplotlib opencv-python gdown seaborn tensorflow_datasets
 
 
 # Test the installation
-$ python -c "mera --version"
+$ mera --version
 >>> Mera Environment Versions:
-      * mera version x.y released on dd/mm/yyyy
-      * mera-tvm version x.y
-      * mera-dna version vx.y+git=<hash>
+      * mera version x.y.z released on dd/mm/yyyy
+      * mera-tvm version x.y.z
+      * mera-dna version vx.y.z+git=<hash>
 ```
 
 `mera` provides packages for installing in both *x86* and *aarch64* architectures.
 The pip command will also install all the necessary dependencies to perform deployments with MERA. Note that some of the tutorials require some extra
 dependencies to be installed. Please check the tutorial's `README.md` file to check which other packages might be needed.
 
 ## MERA Documentation
@@ -186,26 +178,26 @@
 #
 with mera.TVMDeployer(output_dir, overwrite=True) as deployer:
     model = ...
     deploy_ip = deployer.deploy(
         model,
         mera_platform=Platform.DNAA600L0002,
         target=Target.IP,
-        host_arch="x86)
+        host_arch="x86")
 
 #
 # Compilation options example for FPGA IP
 #
 with mera.TVMDeployer(output_dir, overwrite=True) as deployer:
     model = ...
     deploy_ip = deployer.deploy(
         model,
         mera_platform=Platform.DNAF200L0003,
         target=Target.IP,
-        host_arch="x86)
+        host_arch="x86")
 ```
 
 These examples assume some default compiler options, in particular, the Fast scheduling mode,
 which provides fast compilation times but not the best inference times.
 
 > **_NOTE:_**  To facilitate testing of the MERA software stack all the tutorials and scripts use the fast scheduling mode. To get the best latency for production environments please use the high effort scheduling mode instead.
 
@@ -225,15 +217,15 @@
 }
 with mera.TVMDeployer(output_dir, overwrite=True) as deployer:
     model = ...
     deploy_ip = deployer.deploy(
         model,
         mera_platform=Platform.DNAA600L0002,
         target=Target.IP,
-        host_arch="x86,
+        host_arch="x86",
         build_config=build_config)  # new option
 ```
 
 These options provide a trade off between compilation time and inference time but in general higher compilation time should improve the performance of the model being deployed.
 
 > **_NOTE:_**  There are no changes in neither model accuracy or model outputs while using the different scheduling modes. It is guaranteed that the outputs of a model that has been compiled in two different scheduling modes will be exactly the same.
 
@@ -254,41 +246,41 @@
 #
 with mera.TVMDeployer(output_dir, overwrite=True) as deployer:
     model = ...
     deploy_ip = deployer.deploy(
         model,
         mera_platform=Platform.DNAF200L0003,
         target=Target.IP,
-        host_arch="x86)
+        host_arch="x86")
 
 #
 # Compile for FPGA IP C++ simulator
 #
 with mera.TVMDeployer(output_dir, overwrite=True) as deployer:
     model = ...
     deploy_ip = deployer.deploy(
         model,
         mera_platform=Platform.DNAF200L0003,
         target=Target.Simulator,
-        host_arch="x86)
+        host_arch="x86")
 ```
 
 In order to compile a model and do a cycle accurate simulation we should choose the following target:
 
 ```python
 #
 # Compile for verilator simulator using the DNAA600L0002 ASIC architecture (40 TOPs)
 #
 with mera.TVMDeployer(output_dir, overwrite=True) as deployer:
     model = ...
     deploy_ip = deployer.deploy(
         model,
         mera_platform=Platform.DNAA600L0002,
         target=Target.VerilatorSimulator,
-        host_arch="x86)
+        host_arch="x86")
 ```
 
 Note that choosing this target is independent on the scheduler Slow or Fast modes, both can be used for this target but it is recommended to use the Slow (high effort) scheduling mode for the final compilation that will be used to benchmark a model.
 
 In summary, the required configuration to perform a cycle accurate ASIC IP simulation for the DNAA600L0002 architecture, with high effort scheduling mode, are the following changes:
 
 ```python
@@ -304,15 +296,15 @@
 }
 with mera.TVMDeployer(output_dir, overwrite=True) as deployer:
     model = ...
     deploy_ip = deployer.deploy(
         model,
         mera_platform=Platform.DNAA600L0002,
         target=Target.VerilatorSimulator,
-        host_arch="x86,
+        host_arch="x86",
         build_config=build_config)
 ```
 
 The inference times are now more accurate. We observe that in general the Simulator target takes less time to finish a simulation but it will not give us very accurate inference times. While the RTL based simulation will take much longer to complete but will return more accurate inference times. When possible, RTL based simulations in high effort scheduling mode are recommended for model benchmarking.
 
 ## MERA Tutorials
 The [tutorials](tutorials/) folder contains a list of tutorials on how to use the MERA Software Stack to deploy and run inference on typical deep neural network models using both PyTorch and TFLite frameworks. Check the corresponding docs for information about the tutorial contents.
```

