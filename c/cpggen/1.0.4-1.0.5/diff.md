# Comparing `tmp/cpggen-1.0.4.tar.gz` & `tmp/cpggen-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.0.4.tar", max compression
+gzip compressed data, was "cpggen-1.0.5.tar", max compression
```

## Comparing `cpggen-1.0.4.tar` & `cpggen-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-08 18:36:40.291380 cpggen-1.0.4/LICENSE
--rw-r--r--   0        0        0     8804 2023-05-08 18:36:40.291380 cpggen-1.0.4/README.md
--rw-r--r--   0        0        0        0 2023-05-08 18:36:40.291380 cpggen-1.0.4/cpggen/__init__.py
--rw-r--r--   0        0        0    15322 2023-05-08 18:36:40.291380 cpggen-1.0.4/cpggen/cli.py
--rw-r--r--   0        0        0    35417 2023-05-08 18:36:40.291380 cpggen-1.0.4/cpggen/executor.py
--rw-r--r--   0        0        0     1015 2023-05-08 18:36:40.291380 cpggen-1.0.4/cpggen/logger.py
--rw-r--r--   0        0        0    11547 2023-05-08 18:36:40.295380 cpggen-1.0.4/cpggen/utils.py
--rw-r--r--   0        0        0     1278 2023-05-08 18:36:40.295380 cpggen-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    10084 1970-01-01 00:00:00.000000 cpggen-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 01:03:51.835864 cpggen-1.0.5/LICENSE
+-rw-r--r--   0        0        0     9252 2023-05-09 01:03:51.835864 cpggen-1.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 01:03:51.835864 cpggen-1.0.5/cpggen/__init__.py
+-rw-r--r--   0        0        0    17081 2023-05-09 01:03:51.835864 cpggen-1.0.5/cpggen/cli.py
+-rw-r--r--   0        0        0    35426 2023-05-09 01:03:51.835864 cpggen-1.0.5/cpggen/executor.py
+-rw-r--r--   0        0        0     1015 2023-05-09 01:03:51.835864 cpggen-1.0.5/cpggen/logger.py
+-rw-r--r--   0        0        0    11547 2023-05-09 01:03:51.835864 cpggen-1.0.5/cpggen/utils.py
+-rw-r--r--   0        0        0     1278 2023-05-09 01:03:51.835864 cpggen-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    10532 1970-01-01 00:00:00.000000 cpggen-1.0.5/PKG-INFO
```

### Comparing `cpggen-1.0.4/LICENSE` & `cpggen-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.4/README.md` & `cpggen-1.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.4/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.5/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.4/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.5/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -106,14 +106,21 @@
 Or use the nightly to always get the latest joern and tools.
 
 ```
 docker pull ghcr.io/appthreat/cpggen:nightly
 # podman pull ghcr.io/appthreat/cpggen:nightly
 ```
 
+To use the container image with only open-source CPG frontends without any Qwiet.AI support.
+
+```
+docker pull ghcr.io/appthreat/cpggen-oss
+# podman pull ghcr.io/appthreat/cpggen-oss
+```
+
 ## Usage
 
 To auto detect the language from the current directory and generate CPG.
 
 ```
 cpggen
 ```
@@ -194,29 +201,29 @@
 
 ```
 curl "http://127.0.0.1:7072/cpg?url=https://github.com/HooliCorp/vulnerable-aws-koa-app&out_dir=/tmp/cpg_out&lang=js"
 ```
 
 ## Languages supported
 
-| Language    | Requires build |
-| ----------- | -------------- |
-| C           | No             |
-| C++         | No             |
-| Java        | No (\*)        |
-| Scala       | Yes            |
-| Jsp         | Yes            |
-| Jar/War     | No             |
-| JavaScript  | No             |
-| TypeScript  | No             |
-| Kotlin      | No (\*)        |
-| Php         | No             |
-| Python      | No             |
-| C# / dotnet | Yes            |
-| Go          | Yes            |
+| Language    | Requires build | Maturity |
+| ----------- | -------------- | -------- |
+| C           | No             | High     |
+| C++         | No             | High     |
+| Java        | No (\*)        | Medium   |
+| Scala       | Yes            | High     |
+| Jsp         | Yes            | High     |
+| Jar/War     | No             | High     |
+| JavaScript  | No             | Medium   |
+| TypeScript  | No             | Medium   |
+| Kotlin      | No (\*)        | Low      |
+| Php         | No             | Low      |
+| Python      | No             | Low      |
+| C# / dotnet | Yes            | High     |
+| Go          | Yes            | High     |
 
 (\*) - Precision could be improved with dependencies
 
 ## Environment variables
 
 | Name                    | Purpose                                                           |
 | ----------------------- | ----------------------------------------------------------------- |
@@ -229,14 +236,15 @@
 | AT_DEBUG_MODE           | Set to debug to enable debug logging                              |
 | CPG_EXPORT              | Set to true to export CPG graphs in dot format                    |
 | CPG_EXPORT_REPR         | Graph to export. Default all                                      |
 | CPG_EXPORT_FORMAT       | Export format. Default dot                                        |
 | CPG_SLICE               | Set to true to slice CPG                                          |
 | CPG_SLICE_MODE          | Slice mode. Default Usages                                        |
 | SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI      |
+| CDXGEN_ARGS             | Extra arguments to pass to cdxgen                                 |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
 - name: Upload cpg
```

### Comparing `cpggen-1.0.4/cpggen/cli.py` & `cpggen-1.0.5/cpggen/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import argparse
 import json
 import os
 import shutil
 import signal
+import sys
 import tempfile
 from multiprocessing import Pool, freeze_support
 from pathlib import Path, PurePath
 
 from quart import Quart, request
 
 from cpggen import executor, utils
@@ -118,15 +119,15 @@
         dest="export_format",
         choices=["neo4jcsv", "graphml", "graphson", "dot"],
         help="Export format",
     )
     parser.add_argument(
         "--export-out-dir",
         dest="export_out_dir",
-        help="Export output directoru",
+        help="Export output directory",
     )
     parser.add_argument(
         "--verbose",
         action="store_true",
         default=False,
         dest="verbose_mode",
         help="Run cpggen in verbose mode",
@@ -178,37 +179,52 @@
     url = ""
     src = ""
     languages = ""
     cpg_out_dir = None
     is_temp_dir = False
     auto_build = True
     skip_sbom = True
+    slice = False
+    slice_mode = "Usages"
     app_manifest_list = []
+    errors_warnings = []
     if not params:
         params = {}
     if q.get("url"):
         url = q.get("url")
     if q.get("src"):
         src = q.get("src")
     if q.get("out_dir"):
         cpg_out_dir = q.get("out_dir")
     if q.get("lang"):
         languages = q.get("lang")
+    if q.get("slice", "") in ("true", "1"):
+        slice = True
+    if q.get("slice_mode"):
+        slice_mode = q.get("slice_mode")
+    if q.get("auto_build", "") in ("false", "0"):
+        auto_build = False
+    if q.get("skip_sbom", "") in ("false", "0"):
+        skip_sbom = False
     if not url and params.get("url"):
         url = params.get("url")
     if not src and params.get("src"):
         src = params.get("src")
     if not languages and params.get("lang"):
         languages = params.get("lang")
     if not cpg_out_dir and params.get("out_dir"):
         cpg_out_dir = params.get("out_dir")
     if params.get("auto_build", "") in ("false", "0"):
         auto_build = False
     if params.get("skip_sbom", "") in ("false", "0"):
         skip_sbom = False
+    if params.get("slice", "") in ("true", "1"):
+        slice = True
+    if params.get("slice_mode"):
+        slice_mode = params.get("slice_mode")
     if not src and not url:
         return {"error": "true", "message": "path or url is required"}, 500
     # If src contains url, then reassign
     if not url and (src.startswith("http") or src.startswith("git")):
         url = src
     if url.startswith("http") or url.startswith("git"):
         clone_dir = tempfile.mkdtemp(prefix="cpggen")
@@ -230,27 +246,52 @@
             cpg_out_dir,
             src,
             joern_home=os.getenv(
                 "JOERN_HOME", str(Path.home() / "bin" / "joern" / "joern-cli")
             ),
             use_container=False,
             auto_build=auto_build,
-            extra_args={"skip_sbom": skip_sbom},
+            extra_args={"skip_sbom": skip_sbom, "slice_mode": slice_mode},
         )
         if mlist:
             app_manifest_list += mlist
+        if slice and mlist:
+            for ml in mlist:
+                if not os.path.exists(ml.get("cpg")):
+                    errors_warnings.append(
+                        f"""CPG file was not found at {ml.get("cpg")}"""
+                    )
+                    continue
+                executor.exec_tool(
+                    "slice",
+                    ml.get("cpg"),
+                    cpg_out_dir,
+                    src,
+                    joern_home=os.getenv(
+                        "JOERN_HOME", str(Path.home() / "bin" / "joern" / "joern-cli")
+                    ),
+                    use_container=False,
+                    auto_build=False,
+                    extra_args={"slice_mode": slice_mode},
+                )
+                if not os.path.exists(ml.get("slice_out")):
+                    errors_warnings.append(
+                        f"""CPG slice file was not found at {ml.get("slice_out")}"""
+                    )
     if is_temp_dir:
         try:
             os.remove(src)
         except Exception:
             # Ignore cleanup errors
             pass
     return {
-        "success": True,
-        "message": f"CPG generated successfully at {cpg_out_dir}",
+        "success": False if errors_warnings else True,
+        "message": "\n".join(errors_warnings)
+        if errors_warnings
+        else f"CPG generated successfully at {cpg_out_dir}",
         "out_dir": cpg_out_dir,
         "app_manifests": app_manifest_list,
     }
 
 
 def init_worker():
     """
@@ -394,15 +435,21 @@
     if cpg_out_dir:
         cpg_out_dir = str(PurePath(cpg_out_dir))
     if export_out_dir:
         export_out_dir = str(PurePath(export_out_dir))
     languages = args.language
     joern_home = args.joern_home
     use_container = args.use_container
-    if joern_home and not os.path.exists(joern_home):
+    is_bundled_exe = False
+    try:
+        if getattr(sys, "_MEIPASS"):
+            is_bundled_exe = True
+    except Exception:
+        pass
+    if joern_home and not os.path.exists(joern_home) and not is_bundled_exe:
         if utils.check_command("docker") or utils.check_command("podman"):
             use_container = True
         else:
             console.print(
                 "Joern installation was not found. Please install joern by following the instructions at https://joern.io and set the environment variable JOERN_HOME to the directory containing the cli tools"
             )
             console.print(
```

### Comparing `cpggen-1.0.4/cpggen/executor.py` & `cpggen-1.0.5/cpggen/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 runtimeValues = {}
 svmem = psutil.virtual_memory()
 max_memory = bytes2human(getattr(svmem, "available"), format="%(value).0f%(symbol)s")
 cpu_count = str(psutil.cpu_count())
 
 bin_ext = ".bat" if sys.platform == "win32" else ".sh"
+exe_ext = ".exe" if sys.platform == "win32" else ""
 use_shell = True if sys.platform == "win32" else False
 
 
 def resource_path(relative_path):
     try:
         base_path = sys._MEIPASS
     except Exception:
@@ -125,37 +126,37 @@
 
 
 cpg_tools_map = {
     "c": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "cpp": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "c-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
     "cpp-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
-    "java": "%(joern_home)sjavasrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "java-with-deps": "%(joern_home)sjavasrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.m2",
-    "java-with-gradle-deps": "%(joern_home)sjavasrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.gradle/caches/modules-2/files-2.1",
-    "binary": "%(joern_home)sghidra2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "java": "%(joern_home)sjavasrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "java-with-deps": "%(joern_home)sjavasrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.m2",
+    "java-with-gradle-deps": "%(joern_home)sjavasrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.gradle/caches/modules-2/files-2.1",
+    "binary": "%(joern_home)sghidra2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "js": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "ts": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "kotlin": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "kotlin-with-deps": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --download-dependencies",
-    "kotlin-with-classpath": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --classpath %(home_dir)s/.m2 --classpath %(home_dir)s/.gradle/caches/modules-2/files-2.1",
-    "php": "%(joern_home)sphp2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "python": "%(joern_home)spysrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "csharp": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-errors --no-log-file --ignore-tests -l error",
-    "dotnet": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-errors --no-log-file --ignore-tests -l error",
-    "go": "%(joern_home)sgo2cpg generate -o %(cpg_out)s ./...",
+    "kotlin": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "kotlin-with-deps": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --download-dependencies",
+    "kotlin-with-classpath": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --classpath %(home_dir)s/.m2 --classpath %(home_dir)s/.gradle/caches/modules-2/files-2.1",
+    "php": "%(joern_home)sphp2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "python": "%(joern_home)spysrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "csharp": "%(joern_home)scsharp2cpg%(exe_ext)s -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-errors --no-log-file --ignore-tests -l error",
+    "dotnet": "%(joern_home)scsharp2cpg%(bin_ext)s -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-errors --no-log-file --ignore-tests -l error",
+    "go": "%(joern_home)sgo2cpg%(exe_ext)s generate -o %(cpg_out)s ./...",
     "jar": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jar-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "scala": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nojsp --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
-    "sbom": "%(cdxgen_cmd)s -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
-    "export": "%(joern_home)sjoern-export --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
-    "slice": "%(joern_home)sjoern-slice -m %(slice_mode)s --out %(slice_out)s %(cpg_out)s",
-    "qwiet": "sl analyze %(policy)s%(vcs_correction)s--tag app.group=%(group)s --app %(app)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
+    "sbom": "%(cdxgen_cmd)s%(exe_ext)s%(cdxgen_args)s -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
+    "export": "%(joern_home)sjoern-export%(bin_ext)s --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
+    "slice": "%(joern_home)sjoern-slice%(bin_ext)s -m %(slice_mode)s --out %(slice_out)s %(cpg_out)s",
+    "qwiet": "sl%(exe_ext)s analyze %(policy)s%(vcs_correction)s--tag app.group=%(group)s --app %(app)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
     "dot2png": "dot -Tpng %(dot_file)s -o %(png_out)s",
 }
 
 build_tools_map = {
     "csharp": ["dotnet", "build"],
     "jar": {
         "maven": [
@@ -174,19 +175,14 @@
             "compile",
             "package",
             "-Dmaven.test.skip=true",
         ],
         "gradle": [get("GRADLE_CMD", "gradle"), "build"],
     },
     "scala": ["sbt", "stage"],
-    "nodejs": {
-        "npm": ["npm", "install", "--prefer-offline", "--no-audit", "--progress=false"],
-        "yarn": ["yarn", "install"],
-        "rush": ["rush", "install", "--bypass-policy", "--no-link"],
-    },
     "go": {
         "go": ["go", "build", "./..."],
         "make": ["make"],
         "mage": ["mage", "build"],
     },
     "php": {
         "init": ["composer", "init", "--quiet"],
@@ -502,16 +498,14 @@
                 sbom_out = ""
                 manifest_out = ""
                 slice_out = ""
                 if tool_lang == "export":
                     cpg_out = os.path.abspath(cpg_out_dir)
                 elif tool_lang == "slice":
                     cpg_out = src
-                    slice_out = src.replace(".bin.zip", ".slices")
-                    LOG.debug(f"Output file for {tool_lang} is {slice_out}")
                 else:
                     cpg_out = (
                         cpg_out_dir
                         if cpg_out_dir.endswith(".bin.zip")
                         or cpg_out_dir.endswith(".bin")
                         or cpg_out_dir.endswith(".cpg")
                         else os.path.abspath(
@@ -528,27 +522,32 @@
                     )
                     manifest_out = (
                         cpg_out.replace(".bin.zip", ".manifest.json")
                         if cpg_out.endswith(".bin.zip")
                         else f"{cpg_out}.manifest.json"
                     )
                     LOG.debug(f"CPG file for {tool_lang} is {cpg_out}")
+                slice_out = cpg_out.replace(".bin.zip", ".slices")
+                slice_out = slice_out + (
+                    ".json" if extra_args.get("slice_mode") == "Usages" else ".cpg"
+                )
                 cmd_with_args = cmd_with_args % dict(
                     src=os.path.abspath(amodule),
                     cpg_out=cpg_out,
                     joern_home=joern_home,
                     home_dir=str(Path.home()),
                     uber_jar=uber_jar,
                     csharp_artifacts=csharp_artifacts,
                     memory=os.getenv("CPGGEN_MEMORY", max_memory),
                     tool_lang=tool_lang,
                     sbom_out=sbom_out,
                     slice_out=slice_out,
                     cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
                     bin_ext=bin_ext,
+                    exe_ext=exe_ext,
                     **extra_args,
                 )
                 sbom_lang = tool_lang_simple
                 if (
                     tool_lang in ("jar", "scala")
                     or tool_lang.startswith("jar")
                     or tool_lang.startswith("jsp")
@@ -556,14 +555,19 @@
                     sbom_lang = "java"
                 sbom_cmd_with_args = sbom_cmd_with_args % dict(
                     src=os.path.abspath(src),
                     tool_lang=sbom_lang,
                     cwd=cwd,
                     sbom_out=sbom_out,
                     cdxgen_cmd=cdxgen_cmd,
+                    bin_ext=bin_ext,
+                    exe_ext=exe_ext,
+                    cdxgen_args=f' {os.getenv("CDXGEN_ARGS", "").strip()}'
+                    if os.getenv("CDXGEN_ARGS")
+                    else "",
                     cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
                     **extra_args,
                 )
                 cmd_list_with_args = cmd_with_args.split(" ")
                 sbom_cmd_list_with_args = sbom_cmd_with_args.split(" ")
                 lang_cmd = cmd_list_with_args[0]
                 if not check_command(lang_cmd) and not os.path.exists(lang_cmd):
@@ -610,24 +614,15 @@
                                 LOG.info(cp.stderr)
                                 LOG.info("------------------------------")
                                 LOG.info(
                                     f"Command used {' '.join(cmd_list_with_args)}\nPlease report the above error to https://github.com/joernio/joern/issues"
                                 )
                         else:
                             check_dir = (
-                                cpg_out_dir
-                                if tool_lang == "export"
-                                else (
-                                    slice_out
-                                    + (
-                                        ".json"
-                                        if extra_args.get("slice_mode") == "Usages"
-                                        else ".cpg"
-                                    )
-                                )
+                                cpg_out_dir if tool_lang == "export" else slice_out
                             )
                             if os.path.exists(check_dir):
                                 LOG.info(
                                     f"CPG {src} successfully {tool_lang + ('d' if tool_lang.endswith('e') else 'ed')} to {check_dir}"
                                 )
                                 # Convert dot files to png
                                 if tool_lang == "export":
@@ -745,14 +740,15 @@
                             ]
                         app_manifest = {
                             "src": amodule,
                             "group": app_base_name,
                             "app": f"{app_base_name}-{language}",
                             "cpg": cpg_out,
                             "sbom": sbom_out,
+                            "slice_out": slice_out,
                             "language": language,
                             "tool_lang": tool_lang,
                             "cpg_frontend_invocation": " ".join(cmd_list_with_args),
                             "sbom_invocation": " ".join(sbom_cmd_list_with_args),
                         }
                         app_manifest_list.append(app_manifest)
                         if os.getenv("SHIFTLEFT_ACCESS_TOKEN"):
```

### Comparing `cpggen-1.0.4/cpggen/logger.py` & `cpggen-1.0.5/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.4/cpggen/utils.py` & `cpggen-1.0.5/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.4/pyproject.toml` & `cpggen-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.0.4"
+version = "1.0.5"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-1.0.4/PKG-INFO` & `cpggen-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.0.4
+Version: 1.0.5
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8.1,<3.12
@@ -58,23 +58,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.4/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.5/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.4/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.5/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -137,14 +137,21 @@
 Or use the nightly to always get the latest joern and tools.
 
 ```
 docker pull ghcr.io/appthreat/cpggen:nightly
 # podman pull ghcr.io/appthreat/cpggen:nightly
 ```
 
+To use the container image with only open-source CPG frontends without any Qwiet.AI support.
+
+```
+docker pull ghcr.io/appthreat/cpggen-oss
+# podman pull ghcr.io/appthreat/cpggen-oss
+```
+
 ## Usage
 
 To auto detect the language from the current directory and generate CPG.
 
 ```
 cpggen
 ```
@@ -225,29 +232,29 @@
 
 ```
 curl "http://127.0.0.1:7072/cpg?url=https://github.com/HooliCorp/vulnerable-aws-koa-app&out_dir=/tmp/cpg_out&lang=js"
 ```
 
 ## Languages supported
 
-| Language    | Requires build |
-| ----------- | -------------- |
-| C           | No             |
-| C++         | No             |
-| Java        | No (\*)        |
-| Scala       | Yes            |
-| Jsp         | Yes            |
-| Jar/War     | No             |
-| JavaScript  | No             |
-| TypeScript  | No             |
-| Kotlin      | No (\*)        |
-| Php         | No             |
-| Python      | No             |
-| C# / dotnet | Yes            |
-| Go          | Yes            |
+| Language    | Requires build | Maturity |
+| ----------- | -------------- | -------- |
+| C           | No             | High     |
+| C++         | No             | High     |
+| Java        | No (\*)        | Medium   |
+| Scala       | Yes            | High     |
+| Jsp         | Yes            | High     |
+| Jar/War     | No             | High     |
+| JavaScript  | No             | Medium   |
+| TypeScript  | No             | Medium   |
+| Kotlin      | No (\*)        | Low      |
+| Php         | No             | Low      |
+| Python      | No             | Low      |
+| C# / dotnet | Yes            | High     |
+| Go          | Yes            | High     |
 
 (\*) - Precision could be improved with dependencies
 
 ## Environment variables
 
 | Name                    | Purpose                                                           |
 | ----------------------- | ----------------------------------------------------------------- |
@@ -260,14 +267,15 @@
 | AT_DEBUG_MODE           | Set to debug to enable debug logging                              |
 | CPG_EXPORT              | Set to true to export CPG graphs in dot format                    |
 | CPG_EXPORT_REPR         | Graph to export. Default all                                      |
 | CPG_EXPORT_FORMAT       | Export format. Default dot                                        |
 | CPG_SLICE               | Set to true to slice CPG                                          |
 | CPG_SLICE_MODE          | Slice mode. Default Usages                                        |
 | SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI      |
+| CDXGEN_ARGS             | Extra arguments to pass to cdxgen                                 |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
 - name: Upload cpg
```

