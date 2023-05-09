# Comparing `tmp/cpggen-1.0.5.tar.gz` & `tmp/cpggen-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.0.5.tar", max compression
+gzip compressed data, was "cpggen-1.0.6.tar", max compression
```

## Comparing `cpggen-1.0.5.tar` & `cpggen-1.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-09 01:03:51.835864 cpggen-1.0.5/LICENSE
--rw-r--r--   0        0        0     9252 2023-05-09 01:03:51.835864 cpggen-1.0.5/README.md
--rw-r--r--   0        0        0        0 2023-05-09 01:03:51.835864 cpggen-1.0.5/cpggen/__init__.py
--rw-r--r--   0        0        0    17081 2023-05-09 01:03:51.835864 cpggen-1.0.5/cpggen/cli.py
--rw-r--r--   0        0        0    35426 2023-05-09 01:03:51.835864 cpggen-1.0.5/cpggen/executor.py
--rw-r--r--   0        0        0     1015 2023-05-09 01:03:51.835864 cpggen-1.0.5/cpggen/logger.py
--rw-r--r--   0        0        0    11547 2023-05-09 01:03:51.835864 cpggen-1.0.5/cpggen/utils.py
--rw-r--r--   0        0        0     1278 2023-05-09 01:03:51.835864 cpggen-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    10532 1970-01-01 00:00:00.000000 cpggen-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 01:37:25.731130 cpggen-1.0.6/LICENSE
+-rw-r--r--   0        0        0     9252 2023-05-09 01:37:25.731130 cpggen-1.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 01:37:25.731130 cpggen-1.0.6/cpggen/__init__.py
+-rw-r--r--   0        0        0    17207 2023-05-09 01:37:25.731130 cpggen-1.0.6/cpggen/cli.py
+-rw-r--r--   0        0        0    35918 2023-05-09 01:37:25.731130 cpggen-1.0.6/cpggen/executor.py
+-rw-r--r--   0        0        0     1015 2023-05-09 01:37:25.731130 cpggen-1.0.6/cpggen/logger.py
+-rw-r--r--   0        0        0    11547 2023-05-09 01:37:25.731130 cpggen-1.0.6/cpggen/utils.py
+-rw-r--r--   0        0        0     1278 2023-05-09 01:37:25.731130 cpggen-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    10532 1970-01-01 00:00:00.000000 cpggen-1.0.6/PKG-INFO
```

### Comparing `cpggen-1.0.5/LICENSE` & `cpggen-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.5/README.md` & `cpggen-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.5/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.6/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.5/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.6/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
```

### Comparing `cpggen-1.0.5/cpggen/cli.py` & `cpggen-1.0.6/cpggen/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,14 +439,17 @@
     languages = args.language
     joern_home = args.joern_home
     use_container = args.use_container
     is_bundled_exe = False
     try:
         if getattr(sys, "_MEIPASS"):
             is_bundled_exe = True
+            # Reset joern_home for bundled exe
+            if not os.path.exists(joern_home):
+                joern_home = ""
     except Exception:
         pass
     if joern_home and not os.path.exists(joern_home) and not is_bundled_exe:
         if utils.check_command("docker") or utils.check_command("podman"):
             use_container = True
         else:
             console.print(
```

### Comparing `cpggen-1.0.5/cpggen/executor.py` & `cpggen-1.0.6/cpggen/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 )
 
 runtimeValues = {}
 svmem = psutil.virtual_memory()
 max_memory = bytes2human(getattr(svmem, "available"), format="%(value).0f%(symbol)s")
 cpu_count = str(psutil.cpu_count())
 
+only_bat_ext = ".bat" if sys.platform == "win32" else ""
 bin_ext = ".bat" if sys.platform == "win32" else ".sh"
 exe_ext = ".exe" if sys.platform == "win32" else ""
 use_shell = True if sys.platform == "win32" else False
 
 
 def resource_path(relative_path):
     try:
@@ -126,36 +127,36 @@
 
 
 cpg_tools_map = {
     "c": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "cpp": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "c-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
     "cpp-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
-    "java": "%(joern_home)sjavasrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "java-with-deps": "%(joern_home)sjavasrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.m2",
-    "java-with-gradle-deps": "%(joern_home)sjavasrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.gradle/caches/modules-2/files-2.1",
-    "binary": "%(joern_home)sghidra2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "java": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "java-with-deps": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.m2",
+    "java-with-gradle-deps": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.gradle/caches/modules-2/files-2.1",
+    "binary": "%(joern_home)sghidra2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "js": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "ts": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin-with-deps": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --download-dependencies",
     "kotlin-with-classpath": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --classpath %(home_dir)s/.m2 --classpath %(home_dir)s/.gradle/caches/modules-2/files-2.1",
-    "php": "%(joern_home)sphp2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "python": "%(joern_home)spysrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "php": "%(joern_home)sphp2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "python": "%(joern_home)spysrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "csharp": "%(joern_home)scsharp2cpg%(exe_ext)s -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-errors --no-log-file --ignore-tests -l error",
     "dotnet": "%(joern_home)scsharp2cpg%(bin_ext)s -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-errors --no-log-file --ignore-tests -l error",
     "go": "%(joern_home)sgo2cpg%(exe_ext)s generate -o %(cpg_out)s ./...",
     "jar": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jar-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "scala": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nojsp --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "sbom": "%(cdxgen_cmd)s%(exe_ext)s%(cdxgen_args)s -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
-    "export": "%(joern_home)sjoern-export%(bin_ext)s --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
-    "slice": "%(joern_home)sjoern-slice%(bin_ext)s -m %(slice_mode)s --out %(slice_out)s %(cpg_out)s",
+    "export": "%(joern_home)sjoern-export%(only_bat_ext)s --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
+    "slice": "%(joern_home)sjoern-slice%(only_bat_ext)s -m %(slice_mode)s --out %(slice_out)s %(cpg_out)s",
     "qwiet": "sl%(exe_ext)s analyze %(policy)s%(vcs_correction)s--tag app.group=%(group)s --app %(app)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
     "dot2png": "dot -Tpng %(dot_file)s -o %(png_out)s",
 }
 
 build_tools_map = {
     "csharp": ["dotnet", "build"],
     "jar": {
@@ -420,14 +421,22 @@
         redirect_stdout=False,
         refresh_per_second=1,
     ) as progress:
         task = None
         lang_build_crashes = {}
         app_manifest_list = []
         tool_lang_simple = tool_lang.split("-")[0]
+        # Set joern_home from environment variable
+        # This is required to handle bundled exe mode
+        if (
+            not joern_home
+            and os.getenv("JOERN_HOME")
+            and os.path.exists(os.getenv("JOERN_HOME"))
+        ):
+            joern_home = os.getenv("JOERN_HOME")
         if cwd:
             if os.path.isfile(cwd):
                 cwd = os.path.dirname(cwd)
             else:
                 cwd = os.path.abspath(cwd)
         if joern_home and not joern_home.endswith(os.path.sep):
             joern_home = f"{joern_home}{os.path.sep}"
@@ -540,14 +549,15 @@
                     memory=os.getenv("CPGGEN_MEMORY", max_memory),
                     tool_lang=tool_lang,
                     sbom_out=sbom_out,
                     slice_out=slice_out,
                     cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
                     bin_ext=bin_ext,
                     exe_ext=exe_ext,
+                    only_bat_ext=only_bat_ext,
                     **extra_args,
                 )
                 sbom_lang = tool_lang_simple
                 if (
                     tool_lang in ("jar", "scala")
                     or tool_lang.startswith("jar")
                     or tool_lang.startswith("jsp")
@@ -557,14 +567,15 @@
                     src=os.path.abspath(src),
                     tool_lang=sbom_lang,
                     cwd=cwd,
                     sbom_out=sbom_out,
                     cdxgen_cmd=cdxgen_cmd,
                     bin_ext=bin_ext,
                     exe_ext=exe_ext,
+                    only_bat_ext=only_bat_ext,
                     cdxgen_args=f' {os.getenv("CDXGEN_ARGS", "").strip()}'
                     if os.getenv("CDXGEN_ARGS")
                     else "",
                     cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
                     **extra_args,
                 )
                 cmd_list_with_args = cmd_with_args.split(" ")
```

### Comparing `cpggen-1.0.5/cpggen/logger.py` & `cpggen-1.0.6/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.5/cpggen/utils.py` & `cpggen-1.0.6/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.5/pyproject.toml` & `cpggen-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.0.5"
+version = "1.0.6"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-1.0.5/PKG-INFO` & `cpggen-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.0.5
+Version: 1.0.6
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
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.5/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.6/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.5/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.6/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
```

