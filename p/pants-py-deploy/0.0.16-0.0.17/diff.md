# Comparing `tmp/pants_py_deploy-0.0.16-py3-none-any.whl.zip` & `tmp/pants_py_deploy-0.0.17-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11394 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-May-06 09:54 pants_py_deploy/__init__.py
--rw-r--r--  2.0 unx     4820 b- defN 23-May-06 09:54 pants_py_deploy/compose_file.py
--rw-r--r--  2.0 unx     7083 b- defN 23-May-06 09:54 pants_py_deploy/export_env.py
--rw-r--r--  2.0 unx     1010 b- defN 23-May-06 09:54 pants_py_deploy/fields.py
--rw-r--r--  2.0 unx     4812 b- defN 23-May-06 09:54 pants_py_deploy/models.py
--rw-r--r--  2.0 unx    10232 b- defN 23-May-06 09:54 pants_py_deploy/plugin.py
--rw-r--r--  2.0 unx      581 b- defN 23-May-06 09:54 pants_py_deploy/register.py
--rw-r--r--  2.0 unx     2250 b- defN 23-May-06 09:54 pants_py_deploy-0.0.16.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-06 09:54 pants_py_deploy-0.0.16.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-06 09:54 pants_py_deploy-0.0.16.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       16 b- defN 23-May-06 09:54 pants_py_deploy-0.0.16.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1028 b- defN 23-May-06 09:54 pants_py_deploy-0.0.16.dist-info/RECORD
-12 files, 31925 bytes uncompressed, 9644 bytes compressed:  69.8%
+Zip file size: 11573 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-May-09 17:51 pants_py_deploy/__init__.py
+-rw-r--r--  2.0 unx     4820 b- defN 23-May-09 17:51 pants_py_deploy/compose_file.py
+-rw-r--r--  2.0 unx     7083 b- defN 23-May-09 17:51 pants_py_deploy/export_env.py
+-rw-r--r--  2.0 unx     1453 b- defN 23-May-09 17:51 pants_py_deploy/fields.py
+-rw-r--r--  2.0 unx     4812 b- defN 23-May-09 17:51 pants_py_deploy/models.py
+-rw-r--r--  2.0 unx    10391 b- defN 23-May-09 17:51 pants_py_deploy/plugin.py
+-rw-r--r--  2.0 unx      581 b- defN 23-May-09 17:51 pants_py_deploy/register.py
+-rw-r--r--  2.0 unx     2179 b- defN 23-May-09 17:51 pants_py_deploy-0.0.17.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-09 17:51 pants_py_deploy-0.0.17.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-09 17:51 pants_py_deploy-0.0.17.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-May-09 17:51 pants_py_deploy-0.0.17.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1028 b- defN 23-May-09 17:51 pants_py_deploy-0.0.17.dist-info/RECORD
+12 files, 32456 bytes uncompressed, 9823 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pants_py_deploy/plugin.py
 Comment: 
 
 Filename: pants_py_deploy/register.py
 Comment: 
 
-Filename: pants_py_deploy-0.0.16.dist-info/METADATA
+Filename: pants_py_deploy-0.0.17.dist-info/METADATA
 Comment: 
 
-Filename: pants_py_deploy-0.0.16.dist-info/WHEEL
+Filename: pants_py_deploy-0.0.17.dist-info/WHEEL
 Comment: 
 
-Filename: pants_py_deploy-0.0.16.dist-info/namespace_packages.txt
+Filename: pants_py_deploy-0.0.17.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.16.dist-info/top_level.txt
+Filename: pants_py_deploy-0.0.17.dist-info/top_level.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.16.dist-info/RECORD
+Filename: pants_py_deploy-0.0.17.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pants_py_deploy/fields.py

```diff
@@ -1,10 +1,12 @@
 from typing import ClassVar
 
 from pants.engine.target import BoolField, DictStringToStringSequenceField, StringField
+from pants.option.option_types import StrListOption
+from pants.option.subsystem import Subsystem
 from pants.util.frozendict import FrozenDict
 
 
 class ComposeEnabledField(BoolField):
     alias = "compose_enabled"
     default = False
     help = "If set to true, it will create a docker-compose file in the same directory"
@@ -25,7 +27,19 @@
 class ComposeEnvExportField(DictStringToStringSequenceField):
     alias = "compose_env_export"
     default: ClassVar[FrozenDict[str, tuple[str]]] = FrozenDict()
     help = "dict(exclude_globs=['some_ignored_prefix*'], include_globs=['*port']), include_globs takes preference over exclude_globs"
 
 
 COMPOSE_NETWORK_NAME = "pants-default"
+
+
+class PyDeploySubsystem(Subsystem):
+    options_scope = "py-deploy"
+    name = "PyDeploy"
+    help = "Control env-vars resolving for docker-compose files"
+
+    env_vars_file_globs = StrListOption(
+        flag_name="--env-vars-globs",
+        default=lambda cls: ["**/settings.py"],
+        help="patterns of files for finding env-vars",
+    )
```

## pants_py_deploy/plugin.py

```diff
@@ -35,14 +35,15 @@
 )
 from pants_py_deploy.export_env import read_env_and_ports
 from pants_py_deploy.fields import (
     ComposeChartField,
     ComposeChartNameField,
     ComposeEnabledField,
     ComposeEnvExportField,
+    PyDeploySubsystem,
 )
 from pants_py_deploy.models import (
     ComposeEnvExport,
     ComposeExportChart,
     ComposeExportChartRequest,
     ComposeFiles,
     ComposeService,
@@ -52,24 +53,28 @@
     HelmChartsExported,
 )
 from zero_3rdparty.file_utils import iter_paths_and_relative
 from zero_3rdparty.str_utils import ensure_suffix
 
 
 class DockerComposeFileFixer(FixFilesRequest):
+    tool_subsystem = PyDeploySubsystem
+
     @classproperty
     def tool_name(cls) -> str:
         return "docker-compose"
 
     @classproperty
     def tool_id(cls) -> str:
         return "dockercompose"
 
 
 class HelmChartFileFixer(FixFilesRequest):
+    tool_subsystem = PyDeploySubsystem
+
     @classproperty
     def tool_name(cls) -> str:
         return "helm-chart"
 
     @classproperty
     def tool_id(cls) -> str:
         return "helmchart"
@@ -155,29 +160,32 @@
     managed_chart_files = list(
         file.path for file in chain.from_iterable(new_exported_charts.charts.values())
     )
     return Partitions.single_partition(managed_chart_files)
 
 
 @rule
-async def find_env_vars(targets: AllTargets) -> FileEnvVars:
+async def find_env_vars(
+    targets: AllTargets, py_deploy: PyDeploySubsystem
+) -> FileEnvVars:
     # don't understand why targets: Targets doesn't work
     sources = await Get(
         SourceFiles,
         SourceFilesRequest(
             [
                 target[PythonSourceField]
                 for target in targets
                 if target.has_field(PythonSourceField)
             ]
         ),
     )
 
     settings_digest = await Get(
-        Digest, DigestSubset(sources.snapshot.digest, PathGlobs(["**/settings.py"]))
+        Digest,
+        DigestSubset(sources.snapshot.digest, PathGlobs(py_deploy.env_vars_file_globs)),
     )
     digest_contents = await Get(DigestContents, Digest, settings_digest)
     file_env_vars_ports = {
         file_content.path: read_env_and_ports(
             py_script=file_content.content.decode("utf-8")
         )
         for file_content in digest_contents
```

## Comparing `pants_py_deploy-0.0.16.dist-info/METADATA` & `pants_py_deploy-0.0.17.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pants-py-deploy
-Version: 0.0.16
+Version: 0.0.17
 Summary: Make it easy to maintain docker-compose files and helm-charts across projects with pants-py-deploy
 Home-page: https://github.com/EspenAlbert/py-libs
 Author: Espen Albert
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: <3.10,>=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: compose-chart-export (==0.0.16)
-Requires-Dist: docker-compose-parser (==0.0.16)
-Requires-Dist: model-lib (==0.0.16)
+Requires-Dist: compose-chart-export (==0.0.17)
+Requires-Dist: docker-compose-parser (==0.0.17)
+Requires-Dist: model-lib (==0.0.17)
 Requires-Dist: pantsbuild.pants (<2.17,>=2.16.0a0)
-Requires-Dist: zero-3rdparty (==0.0.16)
+Requires-Dist: zero-3rdparty (==0.0.17)
 
 # Pants py_deploy plugin
 - Purpose: Make it easy to maintain docker-compose files and helm-charts across projects
 - Goals
   - Support updating services.{service_name}.
     - `environment` by scanning source code
     - `ports` by scanning source code
@@ -48,9 +48,8 @@
   - docker and helm repository = `app-name`
   - tags:, `app-name-amd`, `app-name-arm`, `app-name-chart`
 - Usage in `pants fix ::`
   - `docker-compose.yaml` file & `chart/*` are create if they don't exist
   - if they exist: ensure environment & ports are up-to-date
 
 ## Later ideas
-- support passing `env_config=dict(ignore_globs=[], include_globs=[])`
 - support analyzing env-vars and using them for adding services like postgres/rabbitmq/mongo etc. to the docker-compose file
```

## Comparing `pants_py_deploy-0.0.16.dist-info/RECORD` & `pants_py_deploy-0.0.17.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pants_py_deploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pants_py_deploy/compose_file.py,sha256=jc1kyOuc0XsBISQCm9yNs_yuwTVfwwY1T6HuXjYdp1c,4820
 pants_py_deploy/export_env.py,sha256=z0a7Sa2Lc4_7cFf9oH7rdoHjUqHgU-e6oshAQ9bm1Yg,7083
-pants_py_deploy/fields.py,sha256=2eCnxTqc2MyBzhKrRWJssZ4SoaV3OkZl36CJ41uhbjQ,1010
+pants_py_deploy/fields.py,sha256=EJwG5FndUPw17-AOVaNseZDmRZuVK46u6ZFYUMrAMlo,1453
 pants_py_deploy/models.py,sha256=PJHV-PFCayRC9KxpoTMjpO0iWiaO3H6q85xE6U4hnRs,4812
-pants_py_deploy/plugin.py,sha256=ZthFNhPnDZhjC8nnsGSOljKOOOS9AM_FQLyc8abfQ_c,10232
+pants_py_deploy/plugin.py,sha256=kIFZWHDQq6-jKl9Lnojmize5RR_aPukFEWqyUZEUjJg,10391
 pants_py_deploy/register.py,sha256=S9bQzA268aY9NXSfW-PvRuRKPvuFT-B86A3FvNbK53E,581
-pants_py_deploy-0.0.16.dist-info/METADATA,sha256=v3DZXGivHUc6DJzAP0ZwAH6CVGZSeCaX0Wc7LW0kMcI,2250
-pants_py_deploy-0.0.16.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pants_py_deploy-0.0.16.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pants_py_deploy-0.0.16.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
-pants_py_deploy-0.0.16.dist-info/RECORD,,
+pants_py_deploy-0.0.17.dist-info/METADATA,sha256=0kCmStqcO6pfNLni1_TO2n1rPYO4IzVfqg0ZP4ykJy0,2179
+pants_py_deploy-0.0.17.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pants_py_deploy-0.0.17.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pants_py_deploy-0.0.17.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
+pants_py_deploy-0.0.17.dist-info/RECORD,,
```

