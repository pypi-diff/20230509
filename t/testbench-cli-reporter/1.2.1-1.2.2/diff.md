# Comparing `tmp/testbench-cli-reporter-1.2.1.tar.gz` & `tmp/testbench-cli-reporter-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testbench-cli-reporter-1.2.1.tar", last modified: Thu Nov  3 12:48:26 2022, max compression
+gzip compressed data, was "testbench-cli-reporter-1.2.2.tar", last modified: Tue May  9 11:33:47 2023, max compression
```

## Comparing `testbench-cli-reporter-1.2.1.tar` & `testbench-cli-reporter-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-03 12:48:26.452043 testbench-cli-reporter-1.2.1/
--rw-r--r--   0 rener      (502) wheel        (0)    11339 2021-08-03 22:56:57.000000 testbench-cli-reporter-1.2.1/LICENSE
--rw-r--r--   0 rener      (502) wheel        (0)       29 2021-08-03 23:07:08.000000 testbench-cli-reporter-1.2.1/MANIFEST.in
--rw-r--r--   0 rener      (502) wheel        (0)     9189 2022-11-03 12:48:26.451777 testbench-cli-reporter-1.2.1/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)     8434 2022-02-04 09:42:22.000000 testbench-cli-reporter-1.2.1/README.md
--rw-r--r--   0 rener      (502) wheel        (0)      171 2022-09-12 17:05:38.000000 testbench-cli-reporter-1.2.1/createPip_whl_tar.sh
--rw-r--r--   0 rener      (502) wheel        (0)     1338 2022-09-13 17:34:19.000000 testbench-cli-reporter-1.2.1/pyproject.toml
--rw-r--r--   0 rener      (502) wheel        (0)       38 2022-11-03 12:48:26.452130 testbench-cli-reporter-1.2.1/setup.cfg
--rw-r--r--   0 rener      (502) wheel        (0)     1571 2022-09-13 17:34:19.000000 testbench-cli-reporter-1.2.1/setup.py
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-03 12:48:26.442700 testbench-cli-reporter-1.2.1/src/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-03 12:48:26.449309 testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/
--rw-r--r--   0 rener      (502) wheel        (0)      583 2021-08-03 22:56:57.000000 testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/__init__.py
--rw-r--r--   0 rener      (502) wheel        (0)     3742 2022-11-03 12:48:21.000000 testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/__main__.py
--rw-r--r--   0 rener      (502) wheel        (0)    13127 2022-09-13 17:34:19.000000 testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/actions.py
--rw-r--r--   0 rener      (502) wheel        (0)     8297 2022-09-13 17:34:19.000000 testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/config_model.py
--rw-r--r--   0 rener      (502) wheel        (0)     7385 2022-09-13 17:34:19.000000 testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/execution.py
--rw-r--r--   0 rener      (502) wheel        (0)     1048 2022-09-13 17:34:19.000000 testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/log.py
--rw-r--r--   0 rener      (502) wheel        (0)    14283 2022-11-03 12:42:05.000000 testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/questions.py
--rw-r--r--   0 rener      (502) wheel        (0)    16068 2022-09-13 17:34:19.000000 testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/testbench.py
--rw-r--r--   0 rener      (502) wheel        (0)    17744 2022-09-13 17:34:19.000000 testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/util.py
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-03 12:48:26.451369 testbench-cli-reporter-1.2.1/src/testbench_cli_reporter.egg-info/
--rw-r--r--   0 rener      (502) wheel        (0)     9189 2022-11-03 12:48:25.000000 testbench-cli-reporter-1.2.1/src/testbench_cli_reporter.egg-info/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)      706 2022-11-03 12:48:26.000000 testbench-cli-reporter-1.2.1/src/testbench_cli_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 rener      (502) wheel        (0)        1 2022-11-03 12:48:25.000000 testbench-cli-reporter-1.2.1/src/testbench_cli_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 rener      (502) wheel        (0)      136 2022-11-03 12:48:26.000000 testbench-cli-reporter-1.2.1/src/testbench_cli_reporter.egg-info/entry_points.txt
--rw-r--r--   0 rener      (502) wheel        (0)       63 2022-11-03 12:48:26.000000 testbench-cli-reporter-1.2.1/src/testbench_cli_reporter.egg-info/requires.txt
--rw-r--r--   0 rener      (502) wheel        (0)       21 2022-11-03 12:48:26.000000 testbench-cli-reporter-1.2.1/src/testbench_cli_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-09 11:33:47.152586 testbench-cli-reporter-1.2.2/
+-rw-r--r--   0 rener      (502) wheel        (0)    11339 2021-08-03 22:56:57.000000 testbench-cli-reporter-1.2.2/LICENSE
+-rw-r--r--   0 rener      (502) wheel        (0)       29 2021-08-03 23:07:08.000000 testbench-cli-reporter-1.2.2/MANIFEST.in
+-rw-r--r--   0 rener      (502) wheel        (0)     9165 2023-05-09 11:33:47.152397 testbench-cli-reporter-1.2.2/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)     8447 2023-05-09 09:49:19.000000 testbench-cli-reporter-1.2.2/README.md
+-rw-r--r--   0 rener      (502) wheel        (0)      171 2022-09-12 17:05:38.000000 testbench-cli-reporter-1.2.2/createPip_whl_tar.sh
+-rw-r--r--   0 rener      (502) wheel        (0)     2102 2023-05-09 09:49:26.000000 testbench-cli-reporter-1.2.2/pyproject.toml
+-rw-r--r--   0 rener      (502) wheel        (0)       38 2023-05-09 11:33:47.152624 testbench-cli-reporter-1.2.2/setup.cfg
+-rw-r--r--   0 rener      (502) wheel        (0)     1559 2023-05-09 09:56:03.000000 testbench-cli-reporter-1.2.2/setup.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-09 11:33:47.148684 testbench-cli-reporter-1.2.2/src/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-09 11:33:47.151267 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/
+-rw-r--r--   0 rener      (502) wheel        (0)      583 2021-08-03 22:56:57.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/__init__.py
+-rw-r--r--   0 rener      (502) wheel        (0)     3855 2023-05-09 11:19:28.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/__main__.py
+-rw-r--r--   0 rener      (502) wheel        (0)    13223 2023-05-09 11:23:34.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/actions.py
+-rw-r--r--   0 rener      (502) wheel        (0)     8260 2023-05-09 11:21:17.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/config_model.py
+-rw-r--r--   0 rener      (502) wheel        (0)     7297 2023-05-09 11:19:01.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/execution.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1048 2023-05-09 11:19:28.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/log.py
+-rw-r--r--   0 rener      (502) wheel        (0)    14540 2023-05-09 11:25:08.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/questions.py
+-rw-r--r--   0 rener      (502) wheel        (0)    16030 2023-05-09 10:02:34.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/testbench.py
+-rw-r--r--   0 rener      (502) wheel        (0)    17489 2023-05-09 10:00:00.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/util.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-09 11:33:47.152185 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/
+-rw-r--r--   0 rener      (502) wheel        (0)     9165 2023-05-09 11:33:47.000000 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)      706 2023-05-09 11:33:47.000000 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 rener      (502) wheel        (0)        1 2023-05-09 11:33:47.000000 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 rener      (502) wheel        (0)      136 2023-05-09 11:33:47.000000 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/entry_points.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       63 2023-05-09 11:33:47.000000 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/requires.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       21 2023-05-09 11:33:47.000000 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/top_level.txt
```

### Comparing `testbench-cli-reporter-1.2.1/LICENSE` & `testbench-cli-reporter-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `testbench-cli-reporter-1.2.1/PKG-INFO` & `testbench-cli-reporter-1.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: testbench-cli-reporter
-Version: 1.2.1
-Summary: CLI Tool to Export XML-Full-Reports from TestBench
-Home-page: https://github.com/imbus/testbench-cli-reporter
-Author: imbus AG | Zacharias Daum & René Rohner
-Author-email: rene.rohner@imbus.de
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Testing :: Acceptance
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # testbench-cli-reporter
 testbench-cli-reporter is a cli tool to export XML reports from an TestBench instance and import test results back into it.
 
 This can be used for automated test execution with e.g. RobotFramework, triggered by a CI/CD pipeline.
 
 ## Supported Actions
 - __Export XML Report__ from TestBench project
@@ -57,15 +37,15 @@
 2. Enter Credential
 
 Next Step is providing login data the testbench-cli-reporter should use to connect with the TestBench. 
 
 Make sure the user has rights to access the test project you want to work with.
 
 ```
-? Enter your login name: vadaj
+? Enter your login name: testbench-user
 ? Enter your password: ****************
 ```
 
 ### **Select Action**
 
 ```
 ? What do you want to do? (Use arrow keys)
@@ -174,30 +154,30 @@
 
 If you didn't export nor import anything in the current session yet, at least the connection properties are written.
 
 ```json
 {
   "configuration": [
     {
-      "server_url": "https://vadaj:9443/api/1/",
+      "server_url": "https://localhost:9443/api/1/",
       "verify": false,
-      "basicAuth": "dHQtYWRtaW46YWRtaW4=",
+      "basicAuth": "XXXXXXXXXXXX=",
       "actions": []
     },
   ]
 }
 ```
 
 ### Change connection
 Connect to a different TestBench instance so you do not have to exit the testbench-cli-reporter completely.
 
 ```
 ? What do you want to do? Change connection
 ? Enter the TestBench server address and port <host:port>:
-? Enter your login name: vadaj
+? Enter your login name: testbench-user
 ? Enter your password: ****************
 ```
 
 ### Quit
 Exits the testbench-cli-reporter
 
 ----------
@@ -209,17 +189,17 @@
 
 ## Config file structure
 The attribute `projectPath` is not mandatory though. Only using projectKey, tovKey, cycleKey is also more error prone, as they will not change within TestBench.
 ```json
 {
   "configuration": [
     {
-      "server_url": "https://remus:9443/api/1/",
+      "server_url": "https://localhost:9443/api/1/",
       "verify": false,
-      "basicAuth": "dHQtYWRtaW46YWRtaW4=",
+      "basicAuth": "XXXXXXXXXXXXX=",
       "actions": [
         {
           "type": "ExportXMLReport",
           "parameters": {
             "tovKey": "8689447",
             "projectPath": [
               "TestBench Demo Agil",
@@ -295,9 +275,7 @@
                         Test Object Version name to be exported <OPTIONAL if --type is 'i'>.
   -y CYCLE, --cycle CYCLE
                         Test Cycle name to be exported <OPTIONAL>
   -u UID, --uid UID     Root UID to be exported <OPTIONAL, Default = ROOT>
   -t {e,i}, --type {e,i}
                         'e' for Export <default>, 'i' for Import
 ```
-
-
```

### Comparing `testbench-cli-reporter-1.2.1/README.md` & `testbench-cli-reporter-1.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: testbench-cli-reporter
+Version: 1.2.2
+Summary: CLI Tool to Export XML-Full-Reports from TestBench
+Home-page: https://github.com/imbus/testbench-cli-reporter
+Author: imbus AG | Zacharias Daum & René Rohner
+Author-email: rene.rohner@imbus.de
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # testbench-cli-reporter
 testbench-cli-reporter is a cli tool to export XML reports from an TestBench instance and import test results back into it.
 
 This can be used for automated test execution with e.g. RobotFramework, triggered by a CI/CD pipeline.
 
 ## Supported Actions
 - __Export XML Report__ from TestBench project
@@ -37,15 +55,15 @@
 2. Enter Credential
 
 Next Step is providing login data the testbench-cli-reporter should use to connect with the TestBench. 
 
 Make sure the user has rights to access the test project you want to work with.
 
 ```
-? Enter your login name: vadaj
+? Enter your login name: testbench-user
 ? Enter your password: ****************
 ```
 
 ### **Select Action**
 
 ```
 ? What do you want to do? (Use arrow keys)
@@ -154,30 +172,30 @@
 
 If you didn't export nor import anything in the current session yet, at least the connection properties are written.
 
 ```json
 {
   "configuration": [
     {
-      "server_url": "https://vadaj:9443/api/1/",
+      "server_url": "https://localhost:9443/api/1/",
       "verify": false,
-      "basicAuth": "dHQtYWRtaW46YWRtaW4=",
+      "basicAuth": "XXXXXXXXXXXX=",
       "actions": []
     },
   ]
 }
 ```
 
 ### Change connection
 Connect to a different TestBench instance so you do not have to exit the testbench-cli-reporter completely.
 
 ```
 ? What do you want to do? Change connection
 ? Enter the TestBench server address and port <host:port>:
-? Enter your login name: vadaj
+? Enter your login name: testbench-user
 ? Enter your password: ****************
 ```
 
 ### Quit
 Exits the testbench-cli-reporter
 
 ----------
@@ -189,17 +207,17 @@
 
 ## Config file structure
 The attribute `projectPath` is not mandatory though. Only using projectKey, tovKey, cycleKey is also more error prone, as they will not change within TestBench.
 ```json
 {
   "configuration": [
     {
-      "server_url": "https://remus:9443/api/1/",
+      "server_url": "https://localhost:9443/api/1/",
       "verify": false,
-      "basicAuth": "dHQtYWRtaW46YWRtaW4=",
+      "basicAuth": "XXXXXXXXXXXXX=",
       "actions": [
         {
           "type": "ExportXMLReport",
           "parameters": {
             "tovKey": "8689447",
             "projectPath": [
               "TestBench Demo Agil",
```

### Comparing `testbench-cli-reporter-1.2.1/setup.py` & `testbench-cli-reporter-1.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import re
-from os.path import abspath, dirname, join
+from pathlib import Path
 
 from setuptools import find_packages, setup
 
-CURDIR = dirname(abspath(__file__))
+CURDIR = Path(__file__).absolute().parent
 
-with open(join(CURDIR, "src", "TestBenchCliReporter", "__main__.py"), encoding="utf-8") as f:
+with (CURDIR / "src" / "TestBenchCliReporter" / "__main__.py").open(encoding="utf-8") as f:
     VERSION = re.search('\n__version__ = "(.*)"', f.read()).group(1)
 
-with open("README.md", "r") as fh:
+with Path("README.md").open() as fh:
     long_description = fh.read()
 
 setup(
     name="testbench-cli-reporter",
     version=VERSION,
     author="imbus AG | Zacharias Daum & René Rohner",
     author_email="rene.rohner@imbus.de",
```

### Comparing `testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/__init__.py` & `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/__init__.py`

 * *Files identical despite different names*

### Comparing `testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/__main__.py` & `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 from .config_model import (
     CliReporterConfig,
     Configuration,
     ExportAction,
     ExportParameters,
     ImportAction,
     ImportParameters,
+    loggingConfiguration,
 )
 from .execution import run_automatic_mode, run_manual_mode
 from .util import close_program, get_configuration, parser, resolve_server_name
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 
 def main():
     arg = parser.parse_args()
     try:
         if arg.config:
             cli_config = get_configuration(arg.config)
@@ -44,20 +45,19 @@
             server = resolve_server_name(arg.server)
 
             cli_config = CliReporterConfig(
                 configuration=[
                     Configuration(
                         server_url=server,
                         verify=False,
-                        basicAuth=base64.b64encode(
-                            f"{arg.login}:{arg.password}".encode("utf-8")
-                        ).decode(),
+                        basicAuth=base64.b64encode(f"{arg.login}:{arg.password}".encode()).decode(),
                         actions=[],
                     )
-                ]
+                ],
+                loggingConfiguration=loggingConfiguration.from_dict({}),
             )
             if arg.type == "e":
                 cli_config.configuration[0].actions.append(
                     ExportAction(
                         ExportParameters(
                             outputPath=arg.path,
                             projectPath=[e for e in [arg.project, arg.version, arg.cycle] if e],
@@ -90,15 +90,16 @@
                     Configuration(
                         server_url=server,
                         verify=False,
                         loginname=arg.login,
                         password=arg.password,
                         actions=[],
                     )
-                ]
+                ],
+                loggingConfiguration=loggingConfiguration.from_dict({}),
             )
             print("No config file given")
             run_manual_mode(cli_config)
     except KeyboardInterrupt:
         close_program()
```

### Comparing `testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/actions.py` & `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import base64
+import contextlib
 import sys
 import traceback
-from os import path
 from pathlib import Path
 from typing import Any, Dict, Union
-from xml.etree import ElementTree as ET
+from xml.etree import ElementTree
 from zipfile import ZipFile
 
 from . import questions, testbench
 from .config_model import ExportParameters, ImportParameters
 from .log import logger
 from .testbench import ConnectionLog
 from .util import (
@@ -80,22 +80,23 @@
         self.filters = self.parameters.filters
         self.parameters.report_config = questions.ask_to_config_report()
         self.parameters.outputPath = questions.ask_for_output_path()
 
         return True
 
     def trigger(self, connection_log: ConnectionLog) -> Union[bool, str]:
-        if not self.parameters.cycleKey or self.parameters.cycleKey == "0":
-            if not self.parameters.tovKey and len(self.parameters.projectPath) >= 2:
-                all_projects = connection_log.active_connection.get_all_projects()
-                (
-                    project_key,
-                    self.parameters.tovKey,
-                    self.parameters.cycleKey,
-                ) = get_project_keys(all_projects, *self.parameters.projectPath)
+        if (not self.parameters.cycleKey or self.parameters.cycleKey == "0") and (
+            not self.parameters.tovKey and len(self.parameters.projectPath) >= 2  # noqa: PLR2004
+        ):
+            all_projects = connection_log.active_connection.get_all_projects()
+            (
+                project_key,
+                self.parameters.tovKey,
+                self.parameters.cycleKey,
+            ) = get_project_keys(all_projects, *self.parameters.projectPath)
 
         self.job_id = connection_log.active_connection.trigger_xml_report_generation(
             self.parameters.tovKey,
             self.parameters.cycleKey,
             self.parameters.reportRootUID or "ROOT",
             self.parameters.filters or [],
             self.parameters.report_config or XmlExportConfig["Itep Export"],
@@ -116,23 +117,23 @@
         result = connection_log.active_connection.get_exp_job_result(self.job_id)
         if result is not None:
             self.report_tmp_name = result
         return result
 
     def finish(self, connection_log: ConnectionLog) -> bool:
         report = connection_log.active_connection.get_xml_report_data(self.report_tmp_name)
-        with open(self.parameters.outputPath, "wb") as output_file:
+        with Path(self.parameters.outputPath).open("wb") as output_file:
             output_file.write(report)
         pretty_print_success_message(
             "Report", Path(self.parameters.outputPath).resolve(), "was generated"
         )
         return True
 
 
-def Action(class_name: str, parameters: Dict[str, str]) -> AbstractAction:
+def Action(class_name: str, parameters: Dict[str, str]) -> AbstractAction:  # noqa: N802
     try:
         return globals()[class_name](parameters)
     except AttributeError:
         logger.error(f"Failed to create class {class_name}")
         close_program()
 
 
@@ -142,18 +143,17 @@
             parameters = ImportParameters.from_dict(parameters)
         super().__init__()
         self.parameters: ImportParameters = parameters or ImportParameters("result.zip")
 
     def prepare(self, connection_log: ConnectionLog) -> bool:
         self.parameters.inputPath = questions.ask_for_input_path()
         project = version = cycle = None
-        try:
+        with contextlib.suppress(Exception):
             project, version, cycle = self.get_project_path_from_report()
-        except:
-            pass
+
         all_projects = connection_log.active_connection.get_all_projects()
         selected_project = questions.ask_to_select_project(all_projects, default=project)
         selected_tov = questions.ask_to_select_tov(selected_project, default=version)
         selected_cycle = questions.ask_to_select_cycle(selected_tov, default=cycle)
         pretty_print_project_selection(selected_project, selected_tov, selected_cycle)
         self.parameters.cycleKey = selected_cycle["key"]["serial"]
         cycle_structure = connection_log.active_connection.get_test_cycle_structure(
@@ -167,27 +167,27 @@
         all_filters = connection_log.active_connection.get_all_filters()
         self.parameters.filters = questions.ask_to_select_filters(all_filters)
         self.parameters.importConfig = questions.ask_to_config_import()
         return True
 
     def get_project_path_from_report(self):
         with ZipFile(self.parameters.inputPath) as zip_file:
-            xml = ET.fromstring(zip_file.read("report.xml"))
+            xml = ElementTree.fromstring(zip_file.read("report.xml"))
             project = xml.find("./header/project").get("name")
             version = xml.find("./header/version").get("name")
             cycle = xml.find("./header/cycle").get("name")
             return project, version, cycle
 
     def trigger(self, connection_log: ConnectionLog) -> bool:
         if not self.parameters.cycleKey:
-            if len(self.parameters.projectPath or []) != 3:
+            if len(self.parameters.projectPath or []) != 3:  # noqa: PLR2004
                 self.parameters.projectPath = self.get_project_path_from_report()
             self.set_cycle_key_from_path(connection_log)
 
-        with open(self.parameters.inputPath, "rb") as execution_report:
+        with Path(self.parameters.inputPath).open("rb") as execution_report:
             execution_report_base64 = base64.b64encode(execution_report.read()).decode()
 
         serverside_file_name = connection_log.active_connection.upload_execution_results(
             execution_report_base64
         )
         if serverside_file_name:
             self.job_id = connection_log.active_connection.trigger_execution_results_import(
@@ -195,14 +195,15 @@
                 self.parameters.reportRootUID or "ROOT",
                 serverside_file_name,
                 self.parameters.defaultTester,
                 self.parameters.filters or [],
                 self.parameters.importConfig or ImportConfig["Typical"],
             )
             return True
+        return None
 
     def set_cycle_key_from_path(self, connection_log: ConnectionLog):
         all_projects = connection_log.active_connection.get_all_projects()
         (
             project_key,
             tov_key,
             self.parameters.cycleKey,
@@ -226,14 +227,15 @@
 
     def finish(self, connection_log: ConnectionLog) -> bool:
         if self.report_tmp_name:
             pretty_print_success_message(
                 "Report", Path(self.parameters.inputPath).resolve(), "was imported"
             )
             return True
+        return None
 
 
 class BrowseProjects(UnloggedAction):
     def prepare(self, connection_log: ConnectionLog) -> bool:
         arg = parser.parse_args()
         project = arg.project
         version = arg.version
@@ -280,15 +282,15 @@
         self.parameters["outputPath"] = questions.ask_for_output_path("config.json")
         return True
 
     def trigger(self, connection_log: ConnectionLog) -> bool:
         try:
             connection_log.export_as_json(self.parameters["outputPath"])
             pretty_print_success_message(
-                "Config", path.abspath(self.parameters["outputPath"]), "was generated"
+                "Config", str(Path(self.parameters["outputPath"]).resolve()), "was generated"
             )
             return True
         except KeyError as e:
             print(f"{str(e)}")
             return False
```

### Comparing `testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/config_model.py` & `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/config_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     TestCaseSet = "TestCaseSet"
     TestCase = "TestCase"
 
 
 @dataclass
 class FilterInfo:
     name: str
-    type: FilterInfoType
+    type: FilterInfoType  # noqa: A003
     testThemeUID: Optional[str] = None
 
     @classmethod
     def from_dict(cls, dictionary):
         return cls(
             name=dictionary["name"],
             type=FilterInfoType(dictionary["type"]),
@@ -77,15 +77,15 @@
             filters=dictionary.get("filters", []),
         )
 
 
 @dataclass
 class ExportAction:
     parameters: ExportParameters
-    type: str = "ExportXMLReport"
+    type: str = "ExportXMLReport"  # noqa: A003
 
     @classmethod
     def from_dict(cls, dictionary):
         return cls(parameters=ExportParameters.from_dict(dictionary.get("parameters") or {}))
 
 
 @dataclass
@@ -135,15 +135,15 @@
             ),
         )
 
 
 @dataclass
 class ImportAction:
     parameters: ImportParameters
-    type: str = "ImportExecutionResults"
+    type: str = "ImportExecutionResults"  # noqa: A003
 
     @classmethod
     def from_dict(cls, dictionary):
         return cls(parameters=ImportParameters.from_dict(dictionary.get("parameters") or {}))
 
 
 @dataclass
@@ -223,32 +223,30 @@
                 "%(asctime)s - %(filename)s:%(lineno)d - %(levelname)8s - %(message)s",
             ),
             fileName=dictionary.get("fileName", "testbench-cli-reporter.log"),
         )
 
 
 @dataclass
-class loggingConfiguration:
-    console: ConsoleLoggerConfig = ConsoleLoggerConfig(
-        logLevel=LogLevel.INFO, logFormat="%(message)s"
-    )
+class loggingConfiguration:  # noqa: N801
+    console: Optional[ConsoleLoggerConfig] = None
     file: Optional[FileLoggerConfig] = None
 
     @classmethod
     def from_dict(cls, dictionary):
         return cls(
             console=ConsoleLoggerConfig.from_dict(dictionary.get("console") or {}),
             file=FileLoggerConfig.from_dict(dictionary.get("file") or {}),
         )
 
 
 @dataclass
 class CliReporterConfig:
     configuration: List[Configuration]
-    loggingConfiguration: loggingConfiguration = loggingConfiguration()
+    loggingConfiguration: loggingConfiguration
 
     @classmethod
     def from_dict(cls, dictionary):
         return cls(
             configuration=[Configuration.from_dict(c) for c in dictionary.get("configuration", [])],
             loggingConfiguration=loggingConfiguration.from_dict(
                 dictionary.get("loggingConfiguration") or {}
```

### Comparing `testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/execution.py` & `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
                     and next_action.trigger(connection_log)
                     and next_action.wait(connection_log)
                     and next_action.finish(connection_log)
                 ):
                     active_connection.add_action(next_action)
             except KeyError as e:
                 logger.error(f"key {str(e)} not found")
-                logger.info(f"Aborted action")
+                logger.info("Aborted action")
 
-            except ValueError as e:
+            except ValueError:
                 logger.debug(traceback.format_exc())
                 logger.info("Aborted action")
 
             except KeyboardInterrupt:
                 logger.info("Action aborted by user interrupt.")
 
             except Timeout:
@@ -120,17 +120,16 @@
             try:
                 action.trigger(connection_queue)
                 connection_queue.active_connection.actions_to_wait_for.append(action)
                 job_counter += 1
             except requests.exceptions.HTTPError as e:
                 if raise_exceptions:
                     raise e
-                else:
-                    logger.exception("Action trigger failed")
-                    logger.error(e.response.json())
+                logger.exception("Action trigger failed")
+                logger.error(e.response.json())
             finally:
                 connection_queue.active_connection.actions_to_trigger.remove(action_to_trigger)
             sleep(0.05)
         connection_queue.next()
     logger.info(f"{job_counter} jobs started at {len(connection_queue.connections)} server(s).")
 
 
@@ -143,17 +142,16 @@
                 active_connection.actions_to_finish.remove(action_to_finish)
             else:
                 active_connection.actions_to_finish = rotate(active_connection.actions_to_finish)
         except requests.exceptions.HTTPError as e:
             active_connection.actions_to_finish.remove(action_to_finish)
             if raise_exceptions:
                 raise e
-            else:
-                logger.exception("Action finish failed, skipping action.")
-                logger.error(e.response.json())
+            logger.exception("Action finish failed, skipping action.")
+            logger.error(e.response.json())
 
 
 def poll_actions_to_wait_for(active_connection, connection_queue, raise_exceptions):
     for _ in range(len(active_connection.actions_to_wait_for)):
         action_to_wait_for = active_connection.actions_to_wait_for[0]
         try:
             if action_to_wait_for.poll(connection_queue):
@@ -163,17 +161,16 @@
                 active_connection.actions_to_wait_for = rotate(
                     active_connection.actions_to_wait_for
                 )
         except requests.exceptions.HTTPError as e:
             active_connection.actions_to_wait_for.remove(action_to_wait_for)
             if raise_exceptions:
                 raise e
-            else:
-                logger.exception("Action poll failed, skipping action.")
-                logger.error(e.response.json())
+            logger.exception("Action poll failed, skipping action.")
+            logger.error(e.response.json())
 
 
 def active_connection_finished(active_connection):
     return (
         len(active_connection.actions_to_trigger)
         + len(active_connection.actions_to_wait_for)
         + len(active_connection.actions_to_finish)
```

### Comparing `testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/log.py` & `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/log.py`

 * *Files identical despite different names*

### Comparing `testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/questions.py` & `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/questions.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import os
-from os.path import abspath, dirname, isdir, isfile
+from pathlib import Path
 from re import fullmatch, sub
 from typing import Callable, Dict, List, Union
 
-from questionary import Choice, Style, checkbox, confirm
+from questionary import Choice, Style, checkbox, confirm, select, unsafe_prompt
 from questionary import print as pprint
-from questionary import select, unsafe_prompt
 
 from . import actions, util
 from .config_model import ExecutionResultsImportOptions
 from .log import logger
 from .util import ImportConfig, XmlExportConfig
 
 custom_style_fancy = Style(
@@ -38,14 +37,30 @@
         ("instruction", ""),
         ("text", ""),
         ("disabled", "#858585 italic"),
     ]
 )
 
 
+def isfile(filepath: Union[str, Path]) -> bool:
+    return Path(filepath).is_file()
+
+
+def isdir(filepath: Union[str, Path]) -> bool:
+    return Path(filepath).is_dir()
+
+
+def dirname(filepath: Union[str, Path]) -> str:
+    return str(Path(filepath).parent)
+
+
+def abspath(filepath: Union[str, Path]) -> str:
+    return str(Path(filepath).resolve().absolute())
+
+
 def selection_prompt(
     message: str,
     choices: List[Choice],
     no_valid_option_message: str = None,
     style: Style = custom_style_fancy,
     default=None,
 ):
@@ -53,16 +68,15 @@
     if valid_choices:
         return select(
             message=message,
             choices=choices,
             style=style,
             default=default,
         ).unsafe_ask()
-    else:
-        raise ValueError(no_valid_option_message)
+    raise ValueError(no_valid_option_message)
 
 
 def confirm_prompt(
     message: str,
     style: Style = custom_style_fancy,
     default: bool = False,
 ):
@@ -82,26 +96,25 @@
     valid_choices = [choice for choice in choices if not choice.disabled]
     if valid_choices:
         return checkbox(
             message=message,
             choices=choices,
             style=style,
         ).unsafe_ask()
-    else:
-        logger.info(no_valid_option_message)
-        return []
+    logger.info(no_valid_option_message)
+    return []
 
 
 def text_prompt(
     message: str,
-    type: str = "text",
-    validation: Callable[[str], bool] = lambda val: val != "",
+    type: str = "text",  # noqa: A002
+    validation: Callable[[str], bool] = lambda val: bool(val),
     style: Style = custom_style_fancy,
     default: str = "",
-    filter: Callable[[str], str] = lambda val: val,
+    filter: Callable[[str], str] = lambda val: val,  # noqa: A002
 ):
     question = [
         {
             "type": type,
             "name": "sole_question",
             "message": message,
             "validate": validation,
@@ -148,16 +161,15 @@
             Choice("Automatically verify the certificate.", True),
             Choice("Provide a path to a local certificate file for verification.", "path"),
         ],
     )
 
     if verification_option == "path":
         return ask_for_certificate_path()
-    else:
-        return verification_option
+    return verification_option
 
 
 def ask_for_certificate_path() -> str:
     return text_prompt(
         message="Provide the path to the certificate.",
         type="path",
         validation=lambda path: True
@@ -211,21 +223,21 @@
         no_valid_option_message="No test cycle available.",
         default=next((x for x in choices if x.title == default), None),
     )
 
 
 def ask_to_select_filters(all_filters: List[dict]) -> List:
     if selection_prompt("Activate Filters:", choices=[Choice("No", False), Choice("Yes", True)]):
-        all_filters_sorted = sorted(all_filters, key=lambda filter: filter["name"].casefold())
+        all_filters_sorted = sorted(all_filters, key=lambda fltr: fltr["name"].casefold())
 
         return checkbox_prompt(
             message="Provide a set of filters.",
             choices=[
-                Choice(filter["name"], {"name": filter["name"], "type": filter["type"]})
-                for filter in all_filters_sorted
+                Choice(fltr["name"], {"name": fltr["name"], "type": fltr["type"]})
+                for fltr in all_filters_sorted
             ],
             no_valid_option_message="No filters available.",
         )
     return []
 
 
 def ask_to_config_report():
@@ -278,30 +290,30 @@
     output_path = text_prompt(
         message=f"Provide the output path [{default}]:",
         type="path",
         validation=lambda path: True
         if ((isdir(path) or isfile(path)) and os.access(path, os.W_OK))
         or os.access(dirname(abspath(path)), os.W_OK)
         else f"Path '{path}' does not exist or is not writeable.",
-        filter=lambda path: os.path.join(path, default) if isdir(path or ".") else path,
+        filter=lambda path: str(Path(path) / default) if isdir(path or ".") else path,
     )
-    pprint(f"Output Path: ", end=None)
+    pprint("Output Path: ", end=None)
     pprint(f"{output_path}", style="#06c8ff bold italic")
     return abspath(output_path)
 
 
 def ask_for_input_path() -> str:
     return text_prompt(
         message="Provide the input path [report.zip]:",
         type="path",
         validation=lambda path: True
         if (isfile(path) and os.access(path, os.R_OK))
         or (isfile("report.zip") and os.access("report.zip", os.R_OK))
         else f"'{path}' is not a file or not readable.",
-        filter=lambda path: "report.zip" if not path else path,
+        filter=lambda path: path if path else "report.zip",
     )
 
 
 def ask_for_action_after_failed_login() -> str:
     return selection_prompt(
         message="What do you want to do?",
         choices=[
@@ -364,16 +376,15 @@
         ],
         no_valid_option_message="No tester available.",
     )
 
 
 def ask_to_select_report_root_uid(cycle_structure: List[dict]):
     cycle_structure_tree = util.add_numbering_to_cycle(cycle_structure)
-    selected_uid = navigate_in_cycle_stucture(cycle_structure_tree)
-    return selected_uid
+    return navigate_in_cycle_stucture(cycle_structure_tree)
 
 
 def navigate_in_cycle_stucture(theme_structure):
     if "Root_structure" in theme_structure["tse"]:
         choices = [Choice("<SELECT ALL>", "ROOT")]
     else:
         te = theme_structure["tse"][
@@ -406,7 +417,8 @@
             choices=choices,
             no_valid_option_message="No element available to be used as the root of the report.",
         )
         if not isinstance(selection, str):
             selection = navigate_in_cycle_stucture(selection)
         if isinstance(selection, str) and selection != "BACK":
             return selection
+    return None
```

### Comparing `testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/testbench.py` & `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/testbench.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf8
 #  Copyright 2021- imbus AG
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -13,24 +12,35 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import base64
 import dataclasses
 import json
 import traceback
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 import requests
 import urllib3
 from questionary import print as pprint
 
 from . import questions
-from .config_model import CliReporterConfig, Configuration, ExecutionResultsImportOptions
+from .config_model import (
+    CliReporterConfig,
+    Configuration,
+    ExecutionResultsImportOptions,
+)
 from .log import logger
-from .util import AbstractAction, ImportConfig, XmlExportConfig, close_program, spin_spinner
+from .util import (
+    AbstractAction,
+    ImportConfig,
+    XmlExportConfig,
+    close_program,
+    spin_spinner,
+)
 
 
 class Connection:
     def __init__(
         self,
         server_url: str,
         verify: Union[bool, str],
@@ -72,34 +82,31 @@
         self._session.verify = self.verify_ssl
         return self._session
 
     def close(self):
         self.session.close()
 
     def export(self) -> Configuration:
-        basic_auth = base64.b64encode(f"{self.loginname}:{self.password}".encode("utf-8")).decode()
+        basic_auth = base64.b64encode(f"{self.loginname}:{self.password}".encode()).decode()
         return Configuration(
             server_url=self.server_url,
             verify=self.session.verify,
             basicAuth=basic_auth,
             actions=[action.export() for action in self.action_log if action.export() is not None],
         )
 
     def add_action(self, action: AbstractAction):
         self.action_log.append(action)
 
     def check_is_identical(self, other) -> bool:
-        if (
+        return bool(
             self.server_url == other.server_url
             and self.loginname == other.loginname
             and self.password == other.password
-        ):
-            return True
-        else:
-            return False
+        )
 
     def check_is_working(self) -> bool:
         response = self.session.get(
             f"{self.server_url}projects",
             params={
                 "includeTOVs": "false",
                 "includeCycles": "false",
@@ -128,17 +135,15 @@
     def get_xml_report(
         self, tov_key: str, cycle_key: str, reportRootUID: str, filters=None
     ) -> bytes:
         if filters is None:
             filters = []
         job_id = self.trigger_xml_report_generation(tov_key, cycle_key, reportRootUID, filters)
         report_tmp_name = self.wait_for_tmp_xml_report_name(job_id)
-        report = self.get_xml_report_data(report_tmp_name)
-
-        return report
+        return self.get_xml_report_data(report_tmp_name)
 
     def trigger_xml_report_generation(
         self,
         tov_key: str,
         cycle_key: str,
         reportRootUID: str,
         filters=None,
@@ -174,16 +179,15 @@
     def get_exp_job_result(self, job_id):
         report_generation_status = self.get_job_result("job/", job_id)
         if report_generation_status is None:
             return None
         result = report_generation_status["result"]
         if "Right" in result:
             return result["Right"]
-        else:
-            raise AssertionError(result)
+        raise AssertionError(result)
 
     def get_job_result(self, path: str, job_id: str):
         report_generation_status = self.session.get(
             f"{self.server_url}{path}{job_id}",
         )
         return report_generation_status.json()["completion"]
 
@@ -257,36 +261,34 @@
                     break
                 spin_spinner("Waiting until import of execution results is done")
 
             result = import_status["result"]
 
             if "Right" in result:
                 return result["Right"]
-            else:
-                raise AssertionError(result)
+            raise AssertionError(result)
         except requests.exceptions.RequestException as e:
             self.render_import_error(e)
             raise e
 
     def render_import_error(self, e):
         pprint("!!!ERROR DURING IMPORT!!!", style="#ff0e0e italic")
-        pprint(f"Report was NOT imported")
+        pprint("Report was NOT imported")
         pprint(f"Error Code {e.response.status_code}")
         pprint(f"Error Message {e.response.text}")
         pprint(f"URL: {e.response.url}")
 
     def get_imp_job_result(self, job_id):
         report_import_status = self.get_job_result("executionResultsImporterJob/", job_id)
         if report_import_status is None:
             return None
         result = report_import_status["result"]
         if "Right" in result:
             return result["Right"]
-        else:
-            raise AssertionError(result)
+        raise AssertionError(result)
 
     def get_test_cycle_structure(self, cycle_key: str) -> List[dict]:
         test_cycle_structure = self.session.get(
             f"{self.server_url}cycle/{cycle_key}/structure",
         )
         return test_cycle_structure.json()
 
@@ -333,15 +335,15 @@
             f"{self.server_url}testCaseSets/"
             f"{testCaseSetKey}/executions/"
             f"{executionKey}/testCases",
         )
         return exec_test_cases.json()
 
 
-def login(server="", login="", pwd="") -> Connection:
+def login(server="", login="", pwd="") -> Connection:  # noqa: C901, PLR0912
     if server and login and pwd:
         credentials = {
             "server_url": server,
             "verify": False,
             "loginname": login,
             "password": pwd,
         }
@@ -408,31 +410,31 @@
 
 
 class ConnectionLog:
     def __init__(self):
         self.connections: List[Connection] = []
 
     @property
-    def len(self) -> int:
+    def len(self) -> int:  # noqa: A003
         return len(self.connections)
 
     @property
     def active_connection(self) -> Connection:
         return self.connections[-1]
 
-    def next(self):
+    def next(self):  # noqa: A003
         self.connections = self.connections[1:] + self.connections[:1]
 
     def remove(self, connection):
         self.connections.remove(connection)
 
     def add_connection(self, new_connection: Connection):
         self.connections.append(new_connection)
 
     def export_as_json(self, output_file_path: str):
         logger.info("Generating JSON export")
         export_config = CliReporterConfig(
             configuration=[connection.export() for connection in self.connections]
         )
 
-        with open(output_file_path, "w") as output_file:
+        with Path(output_file_path).open("w") as output_file:
             json.dump(dataclasses.asdict(export_config), output_file, indent=2)
```

### Comparing `testbench-cli-reporter-1.2.1/src/TestBenchCliReporter/util.py` & `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import json
 import os
 import sys
 import time
 import traceback
 from abc import ABC, abstractmethod
 from collections import OrderedDict
+from pathlib import Path
 from re import fullmatch
 from typing import Any, Dict, Optional
 
 from questionary import print as pprint
 
 from .config_model import (
     CliReporterConfig,
@@ -172,29 +173,29 @@
     print("Closing program.")
     sys.exit(0)
 
 
 def get_configuration(config_file_path: str):
     logger.info("Trying to read config file")
     try:
-        with open(config_file_path, "r") as config_file:
+        with Path(config_file_path).open() as config_file:
             return CliReporterConfig.from_dict(json.load(config_file))
-    except IOError as e:
+    except OSError:
         logger.error("Could not open file")
         logger.debug(traceback.format_exc())
         close_program()
     except json.JSONDecodeError as e:
         logger.error("Could not parse config file as JSON.")
         logger.debug(e)
         close_program()
 
 
 def add_numbering_to_cycle(cycle_structure):
     root_key = 0
-    tse_dict = dict()
+    tse_dict = {}
     for test_structure_element in cycle_structure:
         if "TestTheme_structure" in test_structure_element:
             key = "TestTheme_structure"
         elif "TestCaseSet_structure" in test_structure_element:
             key = "TestCaseSet_structure"
         elif "Root_structure" in test_structure_element:
             key = "Root_structure"
@@ -203,15 +204,15 @@
         else:
             raise KeyError(f"Unexpected Test Structure Element! : {test_structure_element}")
 
         tse_serial = test_structure_element[key]["key"]["serial"]
         tse_parent_serial = test_structure_element[key]["parentPK"]["serial"]
 
         if tse_serial not in tse_dict:
-            tse_dict[tse_serial] = {"tse": test_structure_element, "childs": dict()}
+            tse_dict[tse_serial] = {"tse": test_structure_element, "childs": {}}
         else:
             tse_dict[tse_serial]["tse"] = test_structure_element
 
         if tse_parent_serial not in tse_dict:
             tse_dict[tse_parent_serial] = {
                 "tse": None,
                 "childs": {int(test_structure_element[key]["orderPos"]): tse_dict[tse_serial]},
@@ -242,31 +243,30 @@
         if len(child["childs"]) > 0:
             add_numbering_to_childs(child["childs"].values(), current_numbering)
 
 
 def rotate(li):
     if len(li) > 1:
         return li[1:] + li[:1]
-    else:
-        return li
+    return li
 
 
 def pretty_print(*print_statements: dict):
     try:
         for statement in print_statements:
             pprint(
                 statement.get("value"),
                 style=statement.get("style", None),
                 end=statement.get("end", "\r\n"),
             )
     except Exception:
         print("".join([statement["value"] for statement in print_statements]))
 
 
-def get_project_keys(
+def get_project_keys(  # noqa: C901
     projects: Dict,
     project_name: str,
     tov_name: str,
     cycle_name: Optional[str] = None,
 ):
     project_key = None
     tov_key = None
@@ -291,56 +291,56 @@
     if not tov_key:
         raise ValueError(f"TOV '{tov_name}' not found in project '{project_name}'.")
     if not cycle_key and cycle_name:
         raise ValueError(
             f"Cycle '{cycle_name}' not found in TOV '{tov_name}' in project '{project_name}'."
         )
     pretty_print(
-        {"value": f"PROJECT_KEY: ", "end": None},
+        {"value": "PROJECT_KEY: ", "end": None},
         {"value": f"{project_key}", "style": BLUE_BOLD_ITALIC, "end": None},
-        {"value": f", TOV_Key: ", "end": None},
+        {"value": ", TOV_Key: ", "end": None},
         {"value": f"{tov_key}", "style": BLUE_BOLD_ITALIC, "end": None},
-        {"value": f", CYCLE_KEY: ", "end": None},
+        {"value": ", CYCLE_KEY: ", "end": None},
         {"value": f"{cycle_key}", "style": BLUE_BOLD_ITALIC},
     )
     return project_key, tov_key, cycle_key
 
 
 def pretty_print_project_selection(selected_project, selected_tov, selected_cycle):
     print("  Selection:")
     pretty_print(
         {
             "value": f"{' ' * 4 + selected_project['name']: <50}",
             "style": BLUE_BOLD_ITALIC,
             "end": None,
         },
-        {"value": f"  projectKey: ", "end": None},
+        {"value": "  projectKey: ", "end": None},
         {
             "value": f"{selected_project['key']['serial']: >15}",
             "style": BLUE_BOLD_ITALIC,
         },
         {
             "value": f"{' ' * 6 + selected_tov['name']: <50}",
             "style": BLUE_BOLD_ITALIC,
             "end": None,
         },
-        {"value": f"  tovKey:     ", "end": None},
+        {"value": "  tovKey:     ", "end": None},
         {
             "value": f"{selected_tov['key']['serial']: >15}",
             "style": BLUE_BOLD_ITALIC,
         },
     )
     if selected_cycle != "NO_EXEC":
         pretty_print(
             {
                 "value": f"{' ' * 8 + selected_cycle['name']: <50}",
                 "style": BLUE_BOLD_ITALIC,
                 "end": None,
             },
-            {"value": f"  cycleKey:   ", "end": None},
+            {"value": "  cycleKey:   ", "end": None},
             {
                 "value": f"{selected_cycle['key']['serial']: >15}",
                 "style": BLUE_BOLD_ITALIC,
             },
         )
 
 
@@ -349,15 +349,15 @@
     if not test_cases.get('equal_lists'):
         _pretty_print_test_cases_spec(test_cases)
     _pretty_print_test_cases_exec(test_cases)
     print()
 
 
 def _pretty_print_test_cases_spec(test_cases):
-    print(f"    Specification:")
+    print("    Specification:")
     pretty_print(
         {
             "value": f"{' Nr.  ': >10}",
             "end": None,
         },
         {
             "value": f"{'UniqueID': <35}",
@@ -381,15 +381,15 @@
                 "value": f"{tc['testCaseSpecificationKey']['serial'] : >25}",
                 "style": BLUE_BOLD_ITALIC,
             },
         )
 
 
 def _pretty_print_test_cases_exec(test_cases):
-    print(f"    Execution:")
+    print("    Execution:")
     pretty_print(
         {
             "value": f"{' Nr.  ': >10}",
             "end": None,
         },
         {
             "value": f"{'UniqueID': <35}",
@@ -497,82 +497,80 @@
     else:
         raise ValueError(f"Server name '{server}' is not valid.")
     return resolved_server
 
 
 def spinner():
     if os.name != "posix":
-        return ["_", "_", "_", "-", "`", "`", "'", "´", "-", "_", "_", "_"]
-    else:
-        return [
-            "⢀⠀",
-            "⡀⠀",
-            "⠄⠀",
-            "⢂⠀",
-            "⡂⠀",
-            "⠅⠀",
-            "⢃⠀",
-            "⡃⠀",
-            "⠍⠀",
-            "⢋⠀",
-            "⡋⠀",
-            "⠍⠁",
-            "⢋⠁",
-            "⡋⠁",
-            "⠍⠉",
-            "⠋⠉",
-            "⠋⠉",
-            "⠉⠙",
-            "⠉⠙",
-            "⠉⠩",
-            "⠈⢙",
-            "⠈⡙",
-            "⢈⠩",
-            "⡀⢙",
-            "⠄⡙",
-            "⢂⠩",
-            "⡂⢘",
-            "⠅⡘",
-            "⢃⠨",
-            "⡃⢐",
-            "⠍⡐",
-            "⢋⠠",
-            "⡋⢀",
-            "⠍⡁",
-            "⢋⠁",
-            "⡋⠁",
-            "⠍⠉",
-            "⠋⠉",
-            "⠋⠉",
-            "⠉⠙",
-            "⠉⠙",
-            "⠉⠩",
-            "⠈⢙",
-            "⠈⡙",
-            "⠈⠩",
-            "⠀⢙",
-            "⠀⡙",
-            "⠀⠩",
-            "⠀⢘",
-            "⠀⡘",
-            "⠀⠨",
-            "⠀⢐",
-            "⠀⡐",
-            "⠀⠠",
-            "⠀⢀",
-            "⠀⡀",
-            "⠀⠀",
-        ]
+        return ["_", "_", "_", "-", "`", "`", "'", "`", "-", "_", "_", "_"]
+    return [
+        "⢀⠀",
+        "⡀⠀",
+        "⠄⠀",
+        "⢂⠀",
+        "⡂⠀",
+        "⠅⠀",
+        "⢃⠀",
+        "⡃⠀",
+        "⠍⠀",
+        "⢋⠀",
+        "⡋⠀",
+        "⠍⠁",
+        "⢋⠁",
+        "⡋⠁",
+        "⠍⠉",
+        "⠋⠉",
+        "⠋⠉",
+        "⠉⠙",
+        "⠉⠙",
+        "⠉⠩",
+        "⠈⢙",
+        "⠈⡙",
+        "⢈⠩",
+        "⡀⢙",
+        "⠄⡙",
+        "⢂⠩",
+        "⡂⢘",
+        "⠅⡘",
+        "⢃⠨",
+        "⡃⢐",
+        "⠍⡐",
+        "⢋⠠",
+        "⡋⢀",
+        "⠍⡁",
+        "⢋⠁",
+        "⡋⠁",
+        "⠍⠉",
+        "⠋⠉",
+        "⠋⠉",
+        "⠉⠙",
+        "⠉⠙",
+        "⠉⠩",
+        "⠈⢙",
+        "⠈⡙",
+        "⠈⠩",
+        "⠀⢙",
+        "⠀⡙",
+        "⠀⠩",
+        "⠀⢘",
+        "⠀⡘",
+        "⠀⠨",
+        "⠀⢐",
+        "⠀⡐",
+        "⠀⠠",
+        "⠀⢀",
+        "⠀⡀",
+        "⠀⠀",
+    ]
 
 
 def delay():
     if os.name == "nt":
         return 0.1
-    else:
-        return 0.02
+    return 0.02
 
 
 def spin_spinner(message: str):
     try:
         for cursor in spinner():
             print(
                 f"{message} {cursor}",
```

### Comparing `testbench-cli-reporter-1.2.1/src/testbench_cli_reporter.egg-info/PKG-INFO` & `testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: testbench-cli-reporter
-Version: 1.2.1
+Version: 1.2.2
 Summary: CLI Tool to Export XML-Full-Reports from TestBench
 Home-page: https://github.com/imbus/testbench-cli-reporter
 Author: imbus AG | Zacharias Daum & René Rohner
 Author-email: rene.rohner@imbus.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
@@ -57,15 +55,15 @@
 2. Enter Credential
 
 Next Step is providing login data the testbench-cli-reporter should use to connect with the TestBench. 
 
 Make sure the user has rights to access the test project you want to work with.
 
 ```
-? Enter your login name: vadaj
+? Enter your login name: testbench-user
 ? Enter your password: ****************
 ```
 
 ### **Select Action**
 
 ```
 ? What do you want to do? (Use arrow keys)
@@ -174,30 +172,30 @@
 
 If you didn't export nor import anything in the current session yet, at least the connection properties are written.
 
 ```json
 {
   "configuration": [
     {
-      "server_url": "https://vadaj:9443/api/1/",
+      "server_url": "https://localhost:9443/api/1/",
       "verify": false,
-      "basicAuth": "dHQtYWRtaW46YWRtaW4=",
+      "basicAuth": "XXXXXXXXXXXX=",
       "actions": []
     },
   ]
 }
 ```
 
 ### Change connection
 Connect to a different TestBench instance so you do not have to exit the testbench-cli-reporter completely.
 
 ```
 ? What do you want to do? Change connection
 ? Enter the TestBench server address and port <host:port>:
-? Enter your login name: vadaj
+? Enter your login name: testbench-user
 ? Enter your password: ****************
 ```
 
 ### Quit
 Exits the testbench-cli-reporter
 
 ----------
@@ -209,17 +207,17 @@
 
 ## Config file structure
 The attribute `projectPath` is not mandatory though. Only using projectKey, tovKey, cycleKey is also more error prone, as they will not change within TestBench.
 ```json
 {
   "configuration": [
     {
-      "server_url": "https://remus:9443/api/1/",
+      "server_url": "https://localhost:9443/api/1/",
       "verify": false,
-      "basicAuth": "dHQtYWRtaW46YWRtaW4=",
+      "basicAuth": "XXXXXXXXXXXXX=",
       "actions": [
         {
           "type": "ExportXMLReport",
           "parameters": {
             "tovKey": "8689447",
             "projectPath": [
               "TestBench Demo Agil",
@@ -295,9 +293,7 @@
                         Test Object Version name to be exported <OPTIONAL if --type is 'i'>.
   -y CYCLE, --cycle CYCLE
                         Test Cycle name to be exported <OPTIONAL>
   -u UID, --uid UID     Root UID to be exported <OPTIONAL, Default = ROOT>
   -t {e,i}, --type {e,i}
                         'e' for Export <default>, 'i' for Import
 ```
-
-
```

### Comparing `testbench-cli-reporter-1.2.1/src/testbench_cli_reporter.egg-info/SOURCES.txt` & `testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

