# Comparing `tmp/datatorch-0.4.6.9.tar.gz` & `tmp/datatorch-0.4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatorch-0.4.6.9.tar", last modified: Wed Mar 15 06:40:52 2023, max compression
+gzip compressed data, was "datatorch-0.4.7.0.tar", last modified: Tue May  9 00:21:00 2023, max compression
```

## Comparing `datatorch-0.4.6.9.tar` & `datatorch-0.4.7.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.165124 datatorch-0.4.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-15 06:40:52.165124 datatorch-0.4.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.153123 datatorch-0.4.6.9/datatorch/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.157123 datatorch-0.4.6.9/datatorch/agent/
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.157123 datatorch-0.4.6.9/datatorch/agent/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.157123 datatorch-0.4.6.9/datatorch/agent/pipelines/action/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/action/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/action/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/action/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.157123 datatorch-0.4.6.9/datatorch/agent/pipelines/job/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/job/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.157123 datatorch-0.4.6.9/datatorch/agent/pipelines/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/runner/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/runner/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/runner/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/runner/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/runner/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/runner/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.157123 datatorch-0.4.6.9/datatorch/agent/pipelines/step/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/step/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/pipelines/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.157123 datatorch-0.4.6.9/datatorch/agent/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.161123 datatorch-0.4.6.9/datatorch/agent/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/utils/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/agent/utils/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.161123 datatorch-0.4.6.9/datatorch/api/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.161123 datatorch-0.4.6.9/datatorch/api/entity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.161123 datatorch-0.4.6.9/datatorch/api/entity/sources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/sources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.161123 datatorch-0.4.6.9/datatorch/api/entity/sources/image/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/sources/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/sources/image/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/sources/image/segmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/sources/image/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/sources/source.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/storage_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/entity/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.161123 datatorch-0.4.6.9/datatorch/api/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/scripts/import_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.161123 datatorch-0.4.6.9/datatorch/api/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/scripts/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/scripts/utils/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/api/where.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.165124 datatorch-0.4.6.9/datatorch/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.165124 datatorch-0.4.6.9/datatorch/cli/action/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/action/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/action/pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/action/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.165124 datatorch-0.4.6.9/datatorch/cli/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/agent/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/agent/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/agent/start.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.165124 datatorch-0.4.6.9/datatorch/cli/import_cmds/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/import_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/import_cmds/coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.165124 datatorch-0.4.6.9/datatorch/cli/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/main/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/main/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/main/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/main/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.165124 datatorch-0.4.6.9/datatorch/cli/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/pipeline/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/pipeline/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/pipeline/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.165124 datatorch-0.4.6.9/datatorch/core/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/core/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.165124 datatorch-0.4.6.9/datatorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/utils/hash_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/utils/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/utils/string_style.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/datatorch/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:40:52.157123 datatorch-0.4.6.9/datatorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-15 06:40:52.000000 datatorch-0.4.6.9/datatorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-03-15 06:40:52.000000 datatorch-0.4.6.9/datatorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 06:40:52.000000 datatorch-0.4.6.9/datatorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-15 06:40:52.000000 datatorch-0.4.6.9/datatorch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 06:40:52.000000 datatorch-0.4.6.9/datatorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-15 06:40:52.000000 datatorch-0.4.6.9/datatorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-15 06:40:52.000000 datatorch-0.4.6.9/datatorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 06:40:52.165124 datatorch-0.4.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-15 06:40:42.000000 datatorch-0.4.6.9/setup.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.194367 datatorch-0.4.7.0/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1738 2023-05-09 00:21:00.194190 datatorch-0.4.7.0/PKG-INFO
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      929 2023-01-24 02:19:43.000000 datatorch-0.4.7.0/README.md
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.150212 datatorch-0.4.7.0/datatorch/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      550 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/__init__.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.155328 datatorch-0.4.7.0/datatorch/agent/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     3963 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/agent/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     2603 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/agent/agent.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     6603 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/agent/client.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     2944 2023-01-23 21:11:43.000000 datatorch-0.4.7.0/datatorch/agent/directory.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      483 2023-02-13 19:25:36.000000 datatorch-0.4.7.0/datatorch/agent/log_handler.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      545 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/agent/logging.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     3047 2023-01-16 19:46:14.000000 datatorch-0.4.7.0/datatorch/agent/monitoring.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.156273 datatorch-0.4.7.0/datatorch/agent/pipelines/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      128 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/__init__.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.157669 datatorch-0.4.7.0/datatorch/agent/pipelines/action/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      933 2023-02-13 19:25:36.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/action/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     4900 2023-01-23 21:34:41.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/action/action.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      627 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/action/cache.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     2764 2023-02-13 19:19:53.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/action/config.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.158114 datatorch-0.4.7.0/datatorch/agent/pipelines/job/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)       40 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/job/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1839 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/job/job.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1140 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/pipeline.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.161321 datatorch-0.4.7.0/datatorch/agent/pipelines/runner/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)       64 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/runner/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      478 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/runner/command.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      709 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/runner/docker.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      908 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/runner/factory.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)       64 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/runner/node.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      883 2023-02-13 19:19:53.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/runner/python.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     2386 2023-01-23 21:32:40.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/runner/runner.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      571 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/runner/shell.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.161817 datatorch-0.4.7.0/datatorch/agent/pipelines/step/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)       44 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/step/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     3737 2023-02-13 19:25:36.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/step/step.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     4524 2023-01-23 21:12:06.000000 datatorch-0.4.7.0/datatorch/agent/pipelines/template.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.162061 datatorch-0.4.7.0/datatorch/agent/services/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)        0 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/agent/services/__init__.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.162319 datatorch-0.4.7.0/datatorch/agent/utils/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)        0 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/agent/utils/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)        0 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/agent/utils/docker.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      268 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/agent/utils/process.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.164176 datatorch-0.4.7.0/datatorch/api/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      793 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/api/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     5847 2023-05-09 00:17:28.000000 datatorch-0.4.7.0/datatorch/api/api.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     5949 2023-05-09 00:19:26.000000 datatorch-0.4.7.0/datatorch/api/client.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.171153 datatorch-0.4.7.0/datatorch/api/entity/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)        0 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/api/entity/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     2079 2023-02-13 19:25:36.000000 datatorch-0.4.7.0/datatorch/api/entity/annotation.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     2550 2023-02-13 19:25:36.000000 datatorch-0.4.7.0/datatorch/api/entity/base.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      961 2023-02-13 19:25:36.000000 datatorch-0.4.7.0/datatorch/api/entity/dataset.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     3557 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/api/entity/file.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      263 2023-02-13 19:25:36.000000 datatorch-0.4.7.0/datatorch/api/entity/label.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     6214 2023-05-09 00:17:28.000000 datatorch-0.4.7.0/datatorch/api/entity/project.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      624 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/api/entity/settings.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.171551 datatorch-0.4.7.0/datatorch/api/entity/sources/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)        0 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/api/entity/sources/__init__.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.173143 datatorch-0.4.7.0/datatorch/api/entity/sources/image/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      183 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/api/entity/sources/image/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      725 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/api/entity/sources/image/bounding_box.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      343 2023-02-13 19:25:36.000000 datatorch-0.4.7.0/datatorch/api/entity/sources/image/segmentations.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      128 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/api/entity/sources/image/typings.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1801 2023-02-13 19:25:36.000000 datatorch-0.4.7.0/datatorch/api/entity/sources/source.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      217 2023-02-13 19:25:36.000000 datatorch-0.4.7.0/datatorch/api/entity/storage_link.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      401 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/api/entity/user.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.173601 datatorch-0.4.7.0/datatorch/api/scripts/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)        1 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/api/scripts/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)    11120 2023-01-16 19:55:02.000000 datatorch-0.4.7.0/datatorch/api/scripts/import_coco.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.174024 datatorch-0.4.7.0/datatorch/api/scripts/utils/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)        0 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/api/scripts/utils/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     2526 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/api/scripts/utils/simplify.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      646 2023-02-13 19:25:36.000000 datatorch-0.4.7.0/datatorch/api/utils.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1289 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/api/where.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.174991 datatorch-0.4.7.0/datatorch/cli/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)       46 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/__init__.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.175666 datatorch-0.4.7.0/datatorch/cli/action/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      240 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/action/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1338 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/action/create.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      102 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/action/pull.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     2132 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/action/run.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.176751 datatorch-0.4.7.0/datatorch/cli/agent/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      238 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/agent/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1858 2023-02-13 19:25:36.000000 datatorch-0.4.7.0/datatorch/cli/agent/create.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      429 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/agent/dir.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      680 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/agent/start.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      676 2023-04-01 01:12:17.000000 datatorch-0.4.7.0/datatorch/cli/groups.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.177179 datatorch-0.4.7.0/datatorch/cli/import_cmds/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      172 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/import_cmds/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1529 2022-11-28 19:57:28.000000 datatorch-0.4.7.0/datatorch/cli/import_cmds/coco.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.178869 datatorch-0.4.7.0/datatorch/cli/main/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)        0 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/main/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     2270 2022-03-18 01:39:02.000000 datatorch-0.4.7.0/datatorch/cli/main/login.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      326 2022-03-17 18:40:15.000000 datatorch-0.4.7.0/datatorch/cli/main/logout.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      887 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/main/upgrade.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      184 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/main/version.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.182496 datatorch-0.4.7.0/datatorch/cli/pipeline/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      271 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/pipeline/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)       57 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/pipeline/generate.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      949 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/cli/pipeline/run.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      673 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/pipeline/upload.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1050 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/cli/spinner.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)        0 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/cli/utils.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.186486 datatorch-0.4.7.0/datatorch/core/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      240 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/core/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      157 2022-11-03 16:00:27.000000 datatorch-0.4.7.0/datatorch/core/env.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      436 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/core/folder.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1966 2023-05-09 00:17:28.000000 datatorch-0.4.7.0/datatorch/core/settings.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.193810 datatorch-0.4.7.0/datatorch/utils/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      275 2023-01-16 18:31:36.000000 datatorch-0.4.7.0/datatorch/utils/__init__.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1211 2023-01-16 18:31:36.000000 datatorch-0.4.7.0/datatorch/utils/converters.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      380 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/utils/files.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      610 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/utils/hash_table.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1221 2022-03-18 01:06:40.000000 datatorch-0.4.7.0/datatorch/utils/objects.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      501 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/utils/package.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1229 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/utils/string_style.py
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      176 2022-03-17 17:13:35.000000 datatorch-0.4.7.0/datatorch/utils/url.py
+drwxr-xr-x   0 ninjeezy   (501) staff       (20)        0 2023-05-09 00:21:00.152881 datatorch-0.4.7.0/datatorch.egg-info/
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1738 2023-05-09 00:20:59.000000 datatorch-0.4.7.0/datatorch.egg-info/PKG-INFO
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     3273 2023-05-09 00:20:59.000000 datatorch-0.4.7.0/datatorch.egg-info/SOURCES.txt
+-rw-r--r--   0 ninjeezy   (501) staff       (20)        1 2023-05-09 00:20:59.000000 datatorch-0.4.7.0/datatorch.egg-info/dependency_links.txt
+-rw-r--r--   0 ninjeezy   (501) staff       (20)       73 2023-05-09 00:20:59.000000 datatorch-0.4.7.0/datatorch.egg-info/entry_points.txt
+-rw-r--r--   0 ninjeezy   (501) staff       (20)        1 2022-03-17 17:15:22.000000 datatorch-0.4.7.0/datatorch.egg-info/not-zip-safe
+-rw-r--r--   0 ninjeezy   (501) staff       (20)      237 2023-05-09 00:20:59.000000 datatorch-0.4.7.0/datatorch.egg-info/requires.txt
+-rw-r--r--   0 ninjeezy   (501) staff       (20)       10 2023-05-09 00:20:59.000000 datatorch-0.4.7.0/datatorch.egg-info/top_level.txt
+-rw-r--r--   0 ninjeezy   (501) staff       (20)       38 2023-05-09 00:21:00.194629 datatorch-0.4.7.0/setup.cfg
+-rw-r--r--   0 ninjeezy   (501) staff       (20)     1756 2023-05-09 00:20:03.000000 datatorch-0.4.7.0/setup.py
```

### Comparing `datatorch-0.4.6.9/PKG-INFO` & `datatorch-0.4.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatorch
-Version: 0.4.6.9
+Version: 0.4.7.0
 Summary: A CLI and library for interacting with DataTorch.
 Home-page: https://github.com/datatorch/python
 Author: DataTorch
 Author-email: support@datatorch.io
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datatorch-0.4.6.9/README.md` & `datatorch-0.4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/__init__.py` & `datatorch-0.4.7.0/datatorch/__init__.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/__init__.py` & `datatorch-0.4.7.0/datatorch/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/agent.py` & `datatorch-0.4.7.0/datatorch/agent/agent.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/client.py` & `datatorch-0.4.7.0/datatorch/agent/client.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/directory.py` & `datatorch-0.4.7.0/datatorch/agent/directory.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/logging.py` & `datatorch-0.4.7.0/datatorch/agent/logging.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/monitoring.py` & `datatorch-0.4.7.0/datatorch/agent/monitoring.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/pipelines/action/__init__.py` & `datatorch-0.4.7.0/datatorch/agent/pipelines/action/__init__.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/pipelines/action/action.py` & `datatorch-0.4.7.0/datatorch/agent/pipelines/action/action.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/pipelines/action/cache.py` & `datatorch-0.4.7.0/datatorch/agent/pipelines/action/cache.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/pipelines/action/config.py` & `datatorch-0.4.7.0/datatorch/agent/pipelines/action/config.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/pipelines/job/job.py` & `datatorch-0.4.7.0/datatorch/agent/pipelines/job/job.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/pipelines/pipeline.py` & `datatorch-0.4.7.0/datatorch/agent/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/pipelines/runner/docker.py` & `datatorch-0.4.7.0/datatorch/agent/pipelines/runner/docker.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/pipelines/runner/factory.py` & `datatorch-0.4.7.0/datatorch/agent/pipelines/runner/factory.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/pipelines/runner/python.py` & `datatorch-0.4.7.0/datatorch/agent/pipelines/runner/python.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/pipelines/runner/runner.py` & `datatorch-0.4.7.0/datatorch/agent/pipelines/runner/runner.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/pipelines/runner/shell.py` & `datatorch-0.4.7.0/datatorch/agent/pipelines/runner/shell.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/pipelines/step/step.py` & `datatorch-0.4.7.0/datatorch/agent/pipelines/step/step.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/agent/pipelines/template.py` & `datatorch-0.4.7.0/datatorch/agent/pipelines/template.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/__init__.py` & `datatorch-0.4.7.0/datatorch/api/__init__.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/api.py` & `datatorch-0.4.7.0/datatorch/api/api.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/client.py` & `datatorch-0.4.7.0/datatorch/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     ):
         self._use_sockets = sockets
         self._is_agent = agent
 
         self._api_token = api_key or user_settings.api_url
         # This is to fix init bugs
         if api_url is None and user_settings.api_url is None:
-            self._api_url = "https://datatorch.io"
+            self._api_url = "https://datatorch.io/api"
         if not api_url is None:
             self._api_url = normalize_api_url(api_url)
         if not user_settings.api_url is None:
             self._api_url = normalize_api_url(user_settings.api_url)
 
         self._graphql_url = f"{self.api_url}/graphql"
```

### Comparing `datatorch-0.4.6.9/datatorch/api/entity/annotation.py` & `datatorch-0.4.7.0/datatorch/api/entity/annotation.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/entity/base.py` & `datatorch-0.4.7.0/datatorch/api/entity/base.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/entity/dataset.py` & `datatorch-0.4.7.0/datatorch/api/entity/dataset.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/entity/file.py` & `datatorch-0.4.7.0/datatorch/api/entity/file.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/entity/project.py` & `datatorch-0.4.7.0/datatorch/api/entity/project.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/entity/settings.py` & `datatorch-0.4.7.0/datatorch/api/entity/settings.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/entity/sources/image/bounding_box.py` & `datatorch-0.4.7.0/datatorch/api/entity/sources/image/bounding_box.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/entity/sources/source.py` & `datatorch-0.4.7.0/datatorch/api/entity/sources/source.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/scripts/import_coco.py` & `datatorch-0.4.7.0/datatorch/api/scripts/import_coco.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/scripts/utils/simplify.py` & `datatorch-0.4.7.0/datatorch/api/scripts/utils/simplify.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/utils.py` & `datatorch-0.4.7.0/datatorch/api/utils.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/api/where.py` & `datatorch-0.4.7.0/datatorch/api/where.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/cli/action/create.py` & `datatorch-0.4.7.0/datatorch/cli/action/create.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/cli/action/run.py` & `datatorch-0.4.7.0/datatorch/cli/action/run.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/cli/agent/create.py` & `datatorch-0.4.7.0/datatorch/cli/agent/create.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/cli/agent/start.py` & `datatorch-0.4.7.0/datatorch/cli/agent/start.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/cli/groups.py` & `datatorch-0.4.7.0/datatorch/cli/groups.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/cli/import_cmds/coco.py` & `datatorch-0.4.7.0/datatorch/cli/import_cmds/coco.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/cli/main/login.py` & `datatorch-0.4.7.0/datatorch/cli/main/login.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/cli/main/upgrade.py` & `datatorch-0.4.7.0/datatorch/cli/main/upgrade.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/cli/pipeline/run.py` & `datatorch-0.4.7.0/datatorch/cli/pipeline/run.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/cli/pipeline/upload.py` & `datatorch-0.4.7.0/datatorch/cli/pipeline/upload.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/cli/spinner.py` & `datatorch-0.4.7.0/datatorch/cli/spinner.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/core/settings.py` & `datatorch-0.4.7.0/datatorch/core/settings.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/utils/converters.py` & `datatorch-0.4.7.0/datatorch/utils/converters.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/utils/hash_table.py` & `datatorch-0.4.7.0/datatorch/utils/hash_table.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/utils/objects.py` & `datatorch-0.4.7.0/datatorch/utils/objects.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch/utils/string_style.py` & `datatorch-0.4.7.0/datatorch/utils/string_style.py`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/datatorch.egg-info/PKG-INFO` & `datatorch-0.4.7.0/datatorch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatorch
-Version: 0.4.6.9
+Version: 0.4.7.0
 Summary: A CLI and library for interacting with DataTorch.
 Home-page: https://github.com/datatorch/python
 Author: DataTorch
 Author-email: support@datatorch.io
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datatorch-0.4.6.9/datatorch.egg-info/SOURCES.txt` & `datatorch-0.4.7.0/datatorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatorch-0.4.6.9/setup.py` & `datatorch-0.4.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "tqdm~=4.65.0",
 ]
 
 requirements_agents = []
 
 setup(
     name="datatorch",
-    version="0.4.6.9",
+    version="0.4.7.0",
     description="A CLI and library for interacting with DataTorch.",
     author="DataTorch",
     author_email="support@datatorch.io",
     entry_points={
         "console_scripts": ["datatorch=datatorch.cli:main", "dt=datatorch.cli:main"]
     },
     url="https://github.com/datatorch/python",
```

