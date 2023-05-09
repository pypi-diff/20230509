# Comparing `tmp/nanolab-0.0.1.tar.gz` & `tmp/nanolab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanolab-0.0.1.tar", last modified: Tue May  9 13:34:16 2023, max compression
+gzip compressed data, was "nanolab-0.0.2.tar", last modified: Tue May  9 15:42:44 2023, max compression
```

## Comparing `nanolab-0.0.1.tar` & `nanolab-0.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:34:16.554912 nanolab-0.0.1/
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 22:25:09.000000 nanolab-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-09 13:34:16.554912 nanolab-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1371 2023-05-09 13:33:33.000000 nanolab-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:34:16.554912 nanolab-0.0.1/nanolab/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 21:33:08.000000 nanolab-0.0.1/nanolab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:34:16.554912 nanolab-0.0.1/nanolab/command/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 08:00:48.000000 nanolab-0.0.1/nanolab/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-05-08 13:34:13.000000 nanolab-0.0.1/nanolab/command/command.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-05-07 13:42:34.000000 nanolab-0.0.1/nanolab/command/command_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:34:16.554912 nanolab-0.0.1/nanolab/command/mixins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 13:06:25.000000 nanolab-0.0.1/nanolab/command/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-05-07 19:39:25.000000 nanolab-0.0.1/nanolab/command/mixins/base_mixin.py
--rw-r--r--   0 root         (0) root         (0)      815 2023-05-07 20:03:58.000000 nanolab-0.0.1/nanolab/command/mixins/bash_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-05-07 19:31:15.000000 nanolab-0.0.1/nanolab/command/mixins/python_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-05-07 21:09:14.000000 nanolab-0.0.1/nanolab/command/mixins/snippet_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-05-08 09:49:17.000000 nanolab-0.0.1/nanolab/command/mixins/threaded_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-04-26 22:11:20.000000 nanolab-0.0.1/nanolab/decorators.py
--rwxr-xr-x   0 root         (0) root         (0)      459 2023-05-09 11:04:51.000000 nanolab-0.0.1/nanolab/main.py
--rw-r--r--   0 root         (0) root         (0)    11028 2023-05-08 09:50:05.000000 nanolab-0.0.1/nanolab/node_interaction.py
--rw-r--r--   0 root         (0) root         (0)     6714 2023-05-04 21:26:03.000000 nanolab-0.0.1/nanolab/node_tools.py
--rw-r--r--   0 root         (0) root         (0)     1038 2023-05-04 21:39:19.000000 nanolab-0.0.1/nanolab/pycmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:34:16.554912 nanolab-0.0.1/nanolab/snippets/
--rw-r--r--   0 root         (0) root         (0)     2259 2023-05-09 10:46:49.000000 nanolab-0.0.1/nanolab/snippets/default_snips.json
--rw-r--r--   0 root         (0) root         (0)      984 2023-05-08 13:34:23.000000 nanolab-0.0.1/nanolab/snippets/test_snippets.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:34:16.554912 nanolab-0.0.1/nanolab/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 06:56:43.000000 nanolab-0.0.1/nanolab/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4362 2023-05-09 10:52:35.000000 nanolab-0.0.1/nanolab/src/argparse_commands.py
--rw-r--r--   0 root         (0) root         (0)     6774 2023-05-09 12:53:51.000000 nanolab-0.0.1/nanolab/src/config_handler.py
--rw-r--r--   0 root         (0) root         (0)     5433 2023-05-09 10:31:57.000000 nanolab-0.0.1/nanolab/src/config_loader.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-05-08 12:45:36.000000 nanolab-0.0.1/nanolab/src/github.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-05-08 19:55:35.000000 nanolab-0.0.1/nanolab/src/resolver.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-09 13:01:49.000000 nanolab-0.0.1/nanolab/src/snippet_manager.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-05-09 12:53:54.000000 nanolab-0.0.1/nanolab/src/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:34:16.554912 nanolab-0.0.1/nanolab/xnomin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 21:19:13.000000 nanolab-0.0.1/nanolab/xnomin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-04-24 21:16:18.000000 nanolab-0.0.1/nanolab/xnomin/acctools.py
--rw-r--r--   0 root         (0) root         (0)     7345 2023-05-04 22:16:30.000000 nanolab-0.0.1/nanolab/xnomin/handshake.py
--rw-r--r--   0 root         (0) root         (0)    18867 2023-05-04 22:16:30.000000 nanolab-0.0.1/nanolab/xnomin/peers.py
--rwxr-xr-x   0 root         (0) root         (0)     2438 2023-05-04 22:16:30.000000 nanolab-0.0.1/nanolab/xnomin/telemetry_req.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:34:16.554912 nanolab-0.0.1/nanolab.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-09 13:34:16.000000 nanolab-0.0.1/nanolab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1120 2023-05-09 13:34:16.000000 nanolab-0.0.1/nanolab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 13:34:16.000000 nanolab-0.0.1/nanolab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-09 13:34:16.000000 nanolab-0.0.1/nanolab.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-09 13:34:16.000000 nanolab-0.0.1/nanolab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-09 13:34:16.000000 nanolab-0.0.1/nanolab.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 13:34:16.554912 nanolab-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      646 2023-05-09 13:16:39.000000 nanolab-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:42:44.189192 nanolab-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 22:25:09.000000 nanolab-0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-09 15:42:44.189192 nanolab-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-05-09 13:33:33.000000 nanolab-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:42:44.189192 nanolab-0.0.2/nanolab/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 13:34:16.000000 nanolab-0.0.2/nanolab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:42:44.189192 nanolab-0.0.2/nanolab/command/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 08:00:48.000000 nanolab-0.0.2/nanolab/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-05-08 13:34:13.000000 nanolab-0.0.2/nanolab/command/command.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-05-07 13:42:34.000000 nanolab-0.0.2/nanolab/command/command_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:42:44.189192 nanolab-0.0.2/nanolab/command/mixins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 13:06:25.000000 nanolab-0.0.2/nanolab/command/mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-05-07 19:39:25.000000 nanolab-0.0.2/nanolab/command/mixins/base_mixin.py
+-rw-r--r--   0 root         (0) root         (0)      839 2023-05-09 15:37:47.000000 nanolab-0.0.2/nanolab/command/mixins/bash_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-05-07 19:31:15.000000 nanolab-0.0.2/nanolab/command/mixins/python_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-05-07 21:09:14.000000 nanolab-0.0.2/nanolab/command/mixins/snippet_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-05-08 09:49:17.000000 nanolab-0.0.2/nanolab/command/mixins/threaded_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-26 22:11:20.000000 nanolab-0.0.2/nanolab/decorators.py
+-rwxr-xr-x   0 root         (0) root         (0)      459 2023-05-09 11:04:51.000000 nanolab-0.0.2/nanolab/main.py
+-rw-r--r--   0 root         (0) root         (0)    11028 2023-05-08 09:50:05.000000 nanolab-0.0.2/nanolab/node_interaction.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2023-05-04 21:26:03.000000 nanolab-0.0.2/nanolab/node_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-05-04 21:39:19.000000 nanolab-0.0.2/nanolab/pycmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:42:44.189192 nanolab-0.0.2/nanolab/snippets/
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-05-09 15:33:56.000000 nanolab-0.0.2/nanolab/snippets/default_snips.json
+-rw-r--r--   0 root         (0) root         (0)      984 2023-05-08 13:34:23.000000 nanolab-0.0.2/nanolab/snippets/test_snippets.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:42:44.189192 nanolab-0.0.2/nanolab/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 06:56:43.000000 nanolab-0.0.2/nanolab/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4489 2023-05-09 15:19:18.000000 nanolab-0.0.2/nanolab/src/argparse_commands.py
+-rw-r--r--   0 root         (0) root         (0)     6774 2023-05-09 12:53:51.000000 nanolab-0.0.2/nanolab/src/config_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5433 2023-05-09 10:31:57.000000 nanolab-0.0.2/nanolab/src/config_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-05-08 12:45:36.000000 nanolab-0.0.2/nanolab/src/github.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-05-08 19:55:35.000000 nanolab-0.0.2/nanolab/src/resolver.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-09 13:01:49.000000 nanolab-0.0.2/nanolab/src/snippet_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-05-09 12:53:54.000000 nanolab-0.0.2/nanolab/src/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:42:44.189192 nanolab-0.0.2/nanolab/xnomin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 21:19:13.000000 nanolab-0.0.2/nanolab/xnomin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-04-24 21:16:18.000000 nanolab-0.0.2/nanolab/xnomin/acctools.py
+-rw-r--r--   0 root         (0) root         (0)     7345 2023-05-04 22:16:30.000000 nanolab-0.0.2/nanolab/xnomin/handshake.py
+-rw-r--r--   0 root         (0) root         (0)    18867 2023-05-04 22:16:30.000000 nanolab-0.0.2/nanolab/xnomin/peers.py
+-rwxr-xr-x   0 root         (0) root         (0)     2438 2023-05-04 22:16:30.000000 nanolab-0.0.2/nanolab/xnomin/telemetry_req.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:42:44.189192 nanolab-0.0.2/nanolab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-09 15:42:44.000000 nanolab-0.0.2/nanolab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-05-09 15:42:44.000000 nanolab-0.0.2/nanolab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 15:42:44.000000 nanolab-0.0.2/nanolab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-09 15:42:44.000000 nanolab-0.0.2/nanolab.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-09 15:42:44.000000 nanolab-0.0.2/nanolab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-09 15:42:44.000000 nanolab-0.0.2/nanolab.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 15:42:44.189192 nanolab-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      646 2023-05-09 15:15:50.000000 nanolab-0.0.2/setup.py
```

### Comparing `nanolab-0.0.1/PKG-INFO` & `nanolab-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolab
-Version: 0.0.1
+Version: 0.0.2
 Summary: testing tool using nanomock
 Home-page: https://github.com/gr0vity-dev/nanolab
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 ##NanoLab
```

### Comparing `nanolab-0.0.1/README.md` & `nanolab-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/command/command.py` & `nanolab-0.0.2/nanolab/command/command.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/command/mixins/base_mixin.py` & `nanolab-0.0.2/nanolab/command/mixins/base_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/command/mixins/bash_command_mixin.py` & `nanolab-0.0.2/nanolab/command/mixins/bash_command_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,9 +18,10 @@
                                  capture_output=True)
 
         if process.returncode != 0:
             print(
                 f"Error executing command: {command}\nError: {process.stderr.strip()}"
             )
         else:
-            response = process.stdout.strip() or process.stderr.strip()
+            response = process.stdout.strip() or process.stderr.strip(
+            ) or command
             print(response)
```

### Comparing `nanolab-0.0.1/nanolab/command/mixins/python_command_mixin.py` & `nanolab-0.0.2/nanolab/command/mixins/python_command_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/command/mixins/snippet_command_mixin.py` & `nanolab-0.0.2/nanolab/command/mixins/snippet_command_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/command/mixins/threaded_command_mixin.py` & `nanolab-0.0.2/nanolab/command/mixins/threaded_command_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/decorators.py` & `nanolab-0.0.2/nanolab/decorators.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/node_interaction.py` & `nanolab-0.0.2/nanolab/node_interaction.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/node_tools.py` & `nanolab-0.0.2/nanolab/node_tools.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/pycmd.py` & `nanolab-0.0.2/nanolab/pycmd.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/snippets/default_snips.json` & `nanolab-0.0.2/nanolab/snippets/default_snips.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9839285714285714%*

 * *Differences: {"'setup_easy'": "{'commands': {0: {'command': '[ -f nl_config.toml ] && nanomock down || true'}, "*

 * *                 "1: {'command': 'cp {NL_CONFIG} nl_config.toml'}, 3: {'command': 'nanomock "*

 * *                 'conf_edit --payload \\\'{"nested_path" : "representatives.docker_tag",  "value" '*

 * *                 ': "{{docker_tag}}"}\\\'\'}}}',*

 * * "'setup_ledger_and_config'": "{'commands': {0: {'command': '[ -f nl_config.toml ] && nanomock "*

 * *                              "down || true'}, 1: {'command': 'cp {NL_CO […]*

```diff
@@ -1,24 +1,24 @@
 {
     "setup_easy": {
         "commands": [
             {
-                "command": "nanomock down",
+                "command": "[ -f nl_config.toml ] && nanomock down || true",
                 "type": "bash"
             },
             {
-                "command": "cp {NL_CONFIG} ./nl_config.toml",
+                "command": "cp {NL_CONFIG} nl_config.toml",
                 "type": "bash"
             },
             {
                 "command": "nanomock conf_edit --payload '{\"nested_path\" : \"remote_address\",  \"value\" : \"{{REMOTE_IP}}\"}'",
                 "type": "bash"
             },
             {
-                "command": "#nanomock conf_edit --payload '{\"nested_path\" : \"representatives.docker_tag\",  \"value\" : \"{{docker_tag}}\"}'",
+                "command": "nanomock conf_edit --payload '{\"nested_path\" : \"representatives.docker_tag\",  \"value\" : \"{{docker_tag}}\"}'",
                 "type": "bash"
             },
             {
                 "command": "nanomock create && nanomock reset && nanomock start && nanomock init && nanomock restart_wait_sync",
                 "type": "bash"
             }
         ],
@@ -26,27 +26,27 @@
             "NL_CONFIG",
             "REMOTE_IP"
         ]
     },
     "setup_ledger_and_config": {
         "commands": [
             {
-                "command": "nanomock down",
+                "command": "[ -f nl_config.toml ] && nanomock down || true",
                 "type": "bash"
             },
             {
-                "command": "cp {NL_CONFIG}  ./nl_config.toml",
+                "command": "cp {NL_CONFIG} nl_config.toml",
                 "type": "bash"
             },
             {
                 "command": "nanomock conf_edit --payload '{{\"path\" : \"remote_address\",  \"value\" : \"{REMOTE_IP}\"}}'",
                 "type": "bash"
             },
             {
-                "command": "#nanomock conf_edit --payload '{{\"path\" : \"representatives.docker_tag\",  \"value\" : \"{docker_tag}\"}}'",
+                "command": "nanomock conf_edit --payload '{{\"path\" : \"representatives.docker_tag\",  \"value\" : \"{docker_tag}\"}}'",
                 "type": "bash"
             },
             {
                 "command": "nanomock create && nanomock reset",
                 "type": "bash"
             },
             {
```

### Comparing `nanolab-0.0.1/nanolab/snippets/test_snippets.json` & `nanolab-0.0.2/nanolab/snippets/test_snippets.json`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/src/argparse_commands.py` & `nanolab-0.0.2/nanolab/src/argparse_commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         description="Load configuration and snippets files")
 
     subparsers = parser.add_subparsers(dest="command")
 
     # Run command
     run_parser = subparsers.add_parser("run", help="Run a testcase")
     run_parser.add_argument('-t', '--testcase', type=str, help='Testcase name')
-    run_parser.add_argument('-i', '--image', type=str, help='Docker image')
+    run_parser.add_argument('-i', '--image', nargs='+', help='Docker image(s)')
     run_parser.add_argument('--gh-user',
                             type=str,
                             default='gr0vity-dev',
                             help='GitHub user (default: gr0vity-dev)')
     run_parser.add_argument(
         '--gh-repo',
         type=str,
@@ -103,14 +103,16 @@
         #copy config to disk
         config_path = resource_handler.copy_config_file(
             path_handler.config_copy_file_path)
 
         #resolve and downlaod resources defiend in the config
         resolved_config = resource_handler.download_and_replace_resources(
             config_path, path_handler.downloads_path)
+        #replace docker_tags with commandline
+        if self.args.image: resolved_config["docker_tags"] = self.args.image
 
         self.conf_rw.write_json(path_handler.resolved_config_file_path,
                                 resolved_config)
 
         config_loader = _load_and_validate_configs(
             path_handler.get_snippets_path(),
             path_handler.get_resolved_config_path())
```

### Comparing `nanolab-0.0.1/nanolab/src/config_handler.py` & `nanolab-0.0.2/nanolab/src/config_handler.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/src/config_loader.py` & `nanolab-0.0.2/nanolab/src/config_loader.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/src/github.py` & `nanolab-0.0.2/nanolab/src/github.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/src/resolver.py` & `nanolab-0.0.2/nanolab/src/resolver.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/src/snippet_manager.py` & `nanolab-0.0.2/nanolab/src/snippet_manager.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/src/utils.py` & `nanolab-0.0.2/nanolab/src/utils.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/xnomin/acctools.py` & `nanolab-0.0.2/nanolab/xnomin/acctools.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/xnomin/handshake.py` & `nanolab-0.0.2/nanolab/xnomin/handshake.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/xnomin/peers.py` & `nanolab-0.0.2/nanolab/xnomin/peers.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab/xnomin/telemetry_req.py` & `nanolab-0.0.2/nanolab/xnomin/telemetry_req.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.1/nanolab.egg-info/PKG-INFO` & `nanolab-0.0.2/nanolab.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolab
-Version: 0.0.1
+Version: 0.0.2
 Summary: testing tool using nanomock
 Home-page: https://github.com/gr0vity-dev/nanolab
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 ##NanoLab
```

### Comparing `nanolab-0.0.1/nanolab.egg-info/SOURCES.txt` & `nanolab-0.0.2/nanolab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

