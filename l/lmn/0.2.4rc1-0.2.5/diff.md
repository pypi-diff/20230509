# Comparing `tmp/lmn-0.2.4rc1.tar.gz` & `tmp/lmn-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmn-0.2.4rc1.tar", last modified: Sun Mar 12 16:46:00 2023, max compression
+gzip compressed data, was "lmn-0.2.5.tar", last modified: Tue May  9 16:09:41 2023, max compression
```

## Comparing `lmn-0.2.4rc1.tar` & `lmn-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,16 @@
--rw-r--r--   0        0        0     1005 2023-03-12 16:43:47.659805 lmn-0.2.4rc1/README.md
--rw-r--r--   0        0        0     1170 2023-03-12 16:45:12.478866 lmn-0.2.4rc1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-03-12 16:43:47.645097 lmn-0.2.4rc1/rmx/.DS_Store
--rw-r--r--   0        0        0      685 2023-03-12 16:43:47.646893 lmn-0.2.4rc1/rmx/__init__.py
--rw-r--r--   0        0        0      309 2023-03-12 16:43:47.646590 lmn-0.2.4rc1/rmx/_log_test.py
--rw-r--r--   0        0        0       25 2023-03-12 16:43:47.646112 lmn-0.2.4rc1/rmx/_version.py
--rw-r--r--   0        0        0     6148 2023-03-12 16:43:47.653765 lmn-0.2.4rc1/rmx/cli/.DS_Store
--rw-r--r--   0        0        0     2088 2023-03-12 16:43:47.654420 lmn-0.2.4rc1/rmx/cli/__init__.py
--rw-r--r--   0        0        0     5598 2023-03-12 16:43:47.657315 lmn-0.2.4rc1/rmx/cli/_config_loader.py
--rw-r--r--   0        0        0     2157 2023-03-12 16:43:47.658060 lmn-0.2.4rc1/rmx/cli/_utils.py
--rw-r--r--   0        0        0      411 2023-03-12 16:43:47.657691 lmn-0.2.4rc1/rmx/cli/dummy.py
--rw-r--r--   0        0        0     2939 2023-03-12 16:43:47.654110 lmn-0.2.4rc1/rmx/cli/nv.py
--rw-r--r--   0        0        0    18463 2023-03-12 16:43:47.653472 lmn-0.2.4rc1/rmx/cli/run.py
--rw-r--r--   0        0        0     3442 2023-03-12 16:43:47.653171 lmn-0.2.4rc1/rmx/cli/sync.py
--rw-r--r--   0        0        0     5413 2023-03-12 16:43:47.645616 lmn-0.2.4rc1/rmx/config.py
--rw-r--r--   0        0        0     1003 2023-03-12 16:43:47.647265 lmn-0.2.4rc1/rmx/dockerpty_test.py
--rw-r--r--   0        0        0     8239 2023-03-12 16:43:47.658908 lmn-0.2.4rc1/rmx/helpers.py
--rw-r--r--   0        0        0     3795 2023-03-12 16:43:47.658487 lmn-0.2.4rc1/rmx/machine.py
--rw-r--r--   0        0        0        2 2023-03-12 16:43:47.652341 lmn-0.2.4rc1/rmx/pipx_shared.pth
--rw-r--r--   0        0        0    15066 2023-03-12 16:43:47.644739 lmn-0.2.4rc1/rmx/runner.py
--rw-r--r--   0        0        0        0 2023-03-12 16:43:47.647379 lmn-0.2.4rc1/rmx/types.py
--rw-r--r--   0        0        0      173 2023-03-12 16:43:47.643650 lmn-0.2.4rc1/tests/subp.py
--rw-r--r--   0        0        0     2613 2023-03-12 16:43:47.643943 lmn-0.2.4rc1/tests/test_config.py
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 lmn-0.2.4rc1/PKG-INFO
+-rw-r--r--   0        0        0     1016 2023-05-09 16:09:26.364040 lmn-0.2.5/README.md
+-rw-r--r--   0        0        0      685 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/_version.py
+-rw-r--r--   0        0        0     2088 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/cli/__init__.py
+-rw-r--r--   0        0        0     5598 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/cli/_config_loader.py
+-rw-r--r--   0        0        0     2157 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/cli/_utils.py
+-rw-r--r--   0        0        0    18967 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/cli/run.py
+-rw-r--r--   0        0        0     3442 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/cli/sync.py
+-rw-r--r--   0        0        0     5413 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/config.py
+-rw-r--r--   0        0        0      238 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/const.py
+-rw-r--r--   0        0        0     7584 2023-05-09 16:09:26.368039 lmn-0.2.5/lmn/helpers.py
+-rw-r--r--   0        0        0     3795 2023-05-09 16:09:26.368039 lmn-0.2.5/lmn/machine.py
+-rw-r--r--   0        0        0    16591 2023-05-09 16:09:26.368039 lmn-0.2.5/lmn/runner.py
+-rw-r--r--   0        0        0     1157 2023-05-09 16:09:26.368039 lmn-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2170 2023-05-09 16:09:26.368039 lmn-0.2.5/tests/test_config.py
+-rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 lmn-0.2.5/PKG-INFO
```

### Comparing `lmn-0.2.4rc1/README.md` & `lmn-0.2.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <div align="center">
 
-# RMX - Remote code deployment & execution tool
-<!-- <a href="https://github.com/takuma-yoneda/rmx/actions/workflows/python-publish-pypi.yml"> -->
-<!--     <img src="https://github.com/takuma-yoneda/rmx/actions/workflows/python-publish-pypi.yml/badge.svg" alt="Publish to PyPI" /> -->
+# 🍋 LMN - LaMbda functionality across servers for Noobs
+<!-- <a href="https://github.com/takuma-yoneda/lmn/actions/workflows/python-publish-pypi.yml"> -->
+<!--     <img src="https://github.com/takuma-yoneda/lmn/actions/workflows/python-publish-pypi.yml/badge.svg" alt="Publish to PyPI" /> -->
 <!-- </a> -->
 
 A lightweight tool to rsync and execute local scripts in a remote machine.
 
-<a href="https://github.com/takuma-yoneda/rmx/actions/workflows/python-run-tests.yml">
-    <img src="https://github.com/takuma-yoneda/rmx/actions/workflows/python-run-tests.yml/badge.svg" alt="Test" />
+<a href="https://github.com/takuma-yoneda/lmn/actions/workflows/python-run-tests.yml">
+    <img src="https://github.com/takuma-yoneda/lmn/actions/workflows/python-run-tests.yml/badge.svg" alt="Test" />
 </a>
-<a href="https://github.com/takuma-yoneda/rmx">
-    <img src="https://tokei.rs/b1/github/takuma-yoneda/rmx" alt="Total lines" />
+<a href="https://github.com/takuma-yoneda/lmn">
+    <img src="https://tokei.rs/b1/github/takuma-yoneda/lmn" alt="Total lines" />
 </a>
-<a href="https://pypi.org/project/rmx/">
-    <img src="https://img.shields.io/pypi/v/rmx?logo=python&logoColor=%23cccccc" alt="PyPI" />
+<a href="https://pypi.org/project/lmn/">
+    <img src="https://img.shields.io/pypi/v/lmn?logo=python&logoColor=%23cccccc" alt="PyPI" />
 </a>
 </div>
 
 Inspired by [afdaniele/cpk](https://github.com/afdaniele/cpk) and [geyang/jaynes](https://github.com/geyang/jaynes).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,4 +1,5 @@
-# RMX - Remote code deployment & execution tool    A lightweight tool to rsync
-  and execute local scripts in a remote machine. [Test] [Total_lines] [PyPI]
+  # ð LMN - LaMbda functionality across servers for Noobs    A lightweight
+  tool to rsync and execute local scripts in a remote machine. [Test] [Total
+                                 lines] [PyPI]
 Inspired by [afdaniele/cpk](https://github.com/afdaniele/cpk) and [geyang/
 jaynes](https://github.com/geyang/jaynes).
```

### Comparing `lmn-0.2.4rc1/pyproject.toml` & `lmn-0.2.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "lmn"
-version = "0.2.4rc1"
-description = "Remote code deployment and execution for ML researchers."
+version = "0.2.5"
+description = "LMN: LaMbda functions across servers for Noobs"
 authors = [
     { name = "Takuma Yoneda", email = "takuma-yoneda@users.noreply.github.com" },
     { name = "Takuma Yoneda", email = "takuma.ynd@gmail.com" },
 ]
 dependencies = [
     "colorlog",
     "docker",
@@ -31,18 +31,18 @@
     "Programming Language :: Python :: 3.9",
 ]
 
 [project.license]
 text = "MIT License"
 
 [project.urls]
-Homepage = "https://github.com/takuma-yoneda/rmx"
+Homepage = "https://github.com/takuma-yoneda/lmn"
 
 [project.scripts]
-rmx = "rmx.cli:main"
+lmn = "lmn.cli:main"
 
 [tool.pdm]
 package-dir = "."
 
 [build-system]
 requires = [
     "pdm-pep517>=1.0.0",
```

### Comparing `lmn-0.2.4rc1/rmx/__init__.py` & `lmn-0.2.5/lmn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,9 +20,9 @@
         'WARNING':  'yellow',
         'ERROR':    'red',
         'CRITICAL': 'bold_red',
     }
 ))
 
 
-logger = colorlog.getLogger('rmx')
+logger = colorlog.getLogger('lmn')
 logger.addHandler(handler)
```

### Comparing `lmn-0.2.4rc1/rmx/cli/__init__.py` & `lmn-0.2.5/lmn/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python3
 from __future__ import annotations
-from rmx import __version__
-from rmx import logger
+from lmn import __version__
+from lmn import logger
 import sys
 import argparse
 
 
 def global_parser():
     from . import run, sync, nv
     commands = [run, sync, nv]
 
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-V",
         "--version",
         action="version",
         version="{} - version {}".format(
-            "RMX", __version__
+            "LMN", __version__
         )
     )
     parser.add_argument(
         "--dry-run",
         action="store_true",
         default=False
     )
```

### Comparing `lmn-0.2.4rc1/rmx/cli/_config_loader.py` & `lmn-0.2.5/lmn/cli/_config_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Load config file and fuse it with runtime options"""
 from __future__ import annotations
 from argparse import Namespace
 import os
 import pathlib
 from pathlib import Path
-from rmx import logger
-from rmx.helpers import find_project_root, parse_config
+from lmn import logger
+from lmn.helpers import find_project_root, parse_config
 from posixpath import expandvars
 from dotenv import dotenv_values
 
-from rmx.machine import RemoteConfig
+from lmn.machine import RemoteConfig
 
-DOCKER_ROOT_DIR = '/rmx'
+DOCKER_ROOT_DIR = '/lmn'
 
-# NOTE: I used to set it to /tmp/rmx, but that causes an issue:
-# When multiple users use this directory, the one who used this first set the permission of /tmp/rmx
+# NOTE: I used to set it to /tmp/lmn, but that causes an issue:
+# When multiple users use this directory, the one who used this first set the permission of /tmp/lmn
 # to be his/hers, thus others trying to use it later cannot access it.
 REMOTE_ROOT_DIR = '/tmp'
 
 class Project:
     """Maintains the info specific to the local project"""
     def __init__(self, name, rootdir, outdir=None, exclude=None, startup: str = "", 
                  mount_dirs: dict | None = None, mount_from_host: dict | None = None,
@@ -45,44 +45,44 @@
         return repr(f'<Project {self.name}>')
 
 
 class Machine:
     """Maintains machine configuration.
     - RemoteConfig (user, hostname, uri)
     """
-    def __init__(self, remote_conf: RemoteConfig, rmxdir: str | Path,
+    def __init__(self, remote_conf: RemoteConfig, lmndir: str | Path,
                  parsed_conf: dict,
                  startup: str = "",
                  env: dict | None = None) -> None:
         self.remote_conf = remote_conf
-        self.rmxdir = Path(rmxdir)
+        self.lmndir = Path(lmndir)
         self.env = env if env is not None else {}
         self.startup = startup
         self.parsed_conf = parsed_conf
 
         # aliases
         self.user = remote_conf.user
         self.host = remote_conf.host
         self.base_uri = remote_conf.base_uri
 
     def uri(self, path) -> str:
         """Returns user@hostname:path"""
         return f'{self.remote_conf.base_uri}:{path}'
     
-    def get_rmxdirs(self, project_name: str) -> Namespace:
-        rootdir = self.rmxdir / project_name
+    def get_lmndirs(self, project_name: str) -> Namespace:
+        rootdir = self.lmndir / project_name
         return Namespace(
             codedir=str(rootdir / 'code'),
             mountdir=str(rootdir / 'mount'),
             outdir=str(rootdir / 'output')
         )
 
 
-def get_docker_rmxdirs(rmxdir: Path | str, project_name: str) -> Namespace:
-        rootdir = Path(rmxdir) / project_name
+def get_docker_lmndirs(lmndir: Path | str, project_name: str) -> Namespace:
+        rootdir = Path(lmndir) / project_name
         return Namespace(
             codedir=str(rootdir / 'code'),
             mountdir=str(rootdir / 'mount'),
             outdir=str(rootdir / 'output')
         )
 
 
@@ -144,11 +144,11 @@
                       mount_from_host=mount_from_host)
 
     user, host = mconf['user'], mconf['host']
     remote_conf = RemoteConfig(user, host)
 
     machine = Machine(remote_conf,
                       parsed_conf=mconf,
-                      rmxdir=mconf.get('root_dir', f'{REMOTE_ROOT_DIR}/{remote_conf.user}/rmx'),
+                      lmndir=mconf.get('root_dir', f'{REMOTE_ROOT_DIR}/{remote_conf.user}/lmn'),
                       env=mconf.get('environment', {}))
 
     return project, machine, preset_conf
```

### Comparing `lmn-0.2.4rc1/rmx/cli/_utils.py` & `lmn-0.2.5/lmn/cli/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 import subprocess
-from rmx import logger
+from lmn import logger
 
 def rsync(source_dir, target_dir, options='', exclude=None, dry_run=False, transfer_rootdir=True):
     """
     source_dir: hoge/fuga/source-dir/content-files
     target_dir: Hoge/Fuga/target-dir
 
     if transfer_rootdir is True:
```

### Comparing `lmn-0.2.4rc1/rmx/cli/run.py` & `lmn-0.2.5/lmn/cli/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 from copy import deepcopy
 import os
 from pathlib import Path
 from argparse import ArgumentParser
 from argparse import Namespace
-from rmx import logger
-from rmx.helpers import find_project_root
-from rmx.config import SlurmConfig
-from rmx.helpers import replace_rmx_envvars
-from rmx.cli._config_loader import Project, Machine
-from rmx.machine import SimpleSSHClient
+from lmn import logger
+from lmn.helpers import find_project_root
+from lmn.config import SlurmConfig
+from lmn.helpers import replace_lmn_envvars
+from lmn.cli._config_loader import Project, Machine
+from lmn.machine import SimpleSSHClient
 
-from rmx.runner import SlurmRunner
+from lmn.runner import SlurmRunner
 from .sync import _sync_output, _sync_code
 
 
 def _get_parser() -> ArgumentParser:
     parser = ArgumentParser()
     parser.add_argument(
         "machine",
@@ -94,15 +94,15 @@
         default=1,
         help="number of sequence in Slurm sequential jobs"
     )
     parser.add_argument(
         "--sweep",
         action="store",
         type=str,
-        help="specify sweep range (e.g., --sweep 0-255) this changes the value of $RMX_RUN_SWEEP_IDX"
+        help="specify sweep range (e.g., --sweep 0-255) this changes the value of $LMN_RUN_SWEEP_IDX"
     )
     parser.add_argument(
         "remote_command",
         default=False,
         action="store",
         nargs="+",
         type=str,
@@ -173,79 +173,80 @@
 
     # Sync code first
     if parsed.no_sync:
         logger.warning('--no-sync option is True, local files will not be synced.')
 
     if not parsed.no_sync:
         if parsed.contain:
-            # Generate a unique path and set it to machine.rmxdir
+            # Generate a unique path and set it to machine.lmndir
             # BUG: This generates the same hash every time!! This stack overflow answer is obviously wrong: https://stackoverflow.com/a/6048639/19913466
             # import hashlib
             # import time
             # hashlib.sha1().update(str(time.time()).encode("utf-8"))
             # _hash = hashlib.sha1().hexdigest()
-            from rmx.helpers import get_timestamp
+            from lmn.helpers import get_timestamp
             _hash = get_timestamp()
-            machine.rmxdir = Path(f'{machine.rmxdir}/{_hash}')
+            machine.lmndir = Path(f'{machine.lmndir}/{_hash}')
             runtime_options.name = _hash
-            logger.warning(f'--contain flag is set.\n\tsetting the remote rmxdir to {machine.rmxdir}\n\tsetting jobs suffix to {_hash}')
+            logger.warning(f'--contain flag is set.\n\tsetting the remote lmndir to {machine.lmndir}\n\tsetting jobs suffix to {_hash}')
 
         _sync_code(project, machine, runtime_options.dry_run)
 
     env = {**project.env, **machine.env}
-    rmxdirs = machine.get_rmxdirs(project.name)
+    env_from_host = []
+    lmndirs = machine.get_lmndirs(project.name)
 
     startup = ' && '.join([e for e in [project.startup, machine.startup] if e.strip()])
 
     # If parsed.mode is not set, try to read from the config file.
     mode = parsed.mode or machine.parsed_conf.get('mode')
     if mode is None:
         logger.warning('mode is not set. Setting it to SSH mode')
         mode = 'ssh'
 
     if mode == 'ssh':
-        from rmx.runner import SSHRunner
+        from lmn.runner import SSHRunner
         ssh_client = SimpleSSHClient(machine.remote_conf)
-        ssh_runner = SSHRunner(ssh_client, rmxdirs)
+        ssh_runner = SSHRunner(ssh_client, lmndirs)
         print_conf(mode, machine)
         ssh_runner.exec(runtime_options.cmd,
                         runtime_options.rel_workdir,
                         startup=startup,
                         env=env,
                         dry_run=runtime_options.dry_run)
 
     elif mode == 'docker':
         from docker import DockerClient
-        from rmx.runner import DockerRunner
-        from rmx.config import DockerContainerConfig
+        from lmn.runner import DockerRunner
+        from lmn.config import DockerContainerConfig
         base_url = "ssh://" + machine.base_uri
         # client = DockerClient(base_url=base_url, use_ssh_client=True)
         client = DockerClient(base_url=base_url)  # dockerpty hangs with use_ssh_client=True
 
         # Specify job name
-        name = f'{machine.user}-rmx-{project.name}'
+        name = f'{machine.user}-lmn-{project.name}'
         if runtime_options.name is not None:
             name = f'{name}--{runtime_options.name}'
 
         if runtime_options.dry_run:
             raise ValueError('dry run is not yet supported for Docker mode')
 
         from docker.types import Mount
-        from rmx.cli._config_loader import DOCKER_ROOT_DIR, get_docker_rmxdirs
-        docker_rmxdirs = get_docker_rmxdirs(DOCKER_ROOT_DIR, project.name)
+        from lmn.cli._config_loader import DOCKER_ROOT_DIR, get_docker_lmndirs
+        docker_lmndirs = get_docker_lmndirs(DOCKER_ROOT_DIR, project.name)
 
         if not runtime_options.no_sync:
-            mounts = [Mount(target=docker_rmxdirs.codedir, source=rmxdirs.codedir, type='bind'),
-                    Mount(target=docker_rmxdirs.outdir, source=rmxdirs.outdir, type='bind'),
-                    Mount(target=docker_rmxdirs.mountdir, source=rmxdirs.mountdir, type='bind')]
+            mounts = [Mount(target=docker_lmndirs.codedir, source=lmndirs.codedir, type='bind'),
+                    Mount(target=docker_lmndirs.outdir, source=lmndirs.outdir, type='bind'),
+                    Mount(target=docker_lmndirs.mountdir, source=lmndirs.mountdir, type='bind')]
         else:
             mounts = []
         mounts += [Mount(target=tgt, source=src, type='bind') for src, tgt in project.mount_from_host.items()]
 
-        docker_runner = DockerRunner(client, docker_rmxdirs)
+        docker_runner = DockerRunner(client, docker_lmndirs)
 
         # Docker specific configurations
         docker_pconf = machine.parsed_conf.get('docker', {})
         image = parsed.image or docker_pconf.get('image')
         user_id = docker_pconf.get('user_id', 0)
         group_id = docker_pconf.get('group_id', 0)
 
@@ -272,15 +273,15 @@
             sweep_ind = parse_sweep_idx(runtime_options.sweep)
 
             single_sweep = (len(sweep_ind) == 1)
 
             for sweep_idx in sweep_ind:
                 _name = f'{name}-{sweep_idx}'
                 logger.info(f'Launching sweep {sweep_idx}: {_name}')
-                env.update({'RMX_RUN_SWEEP_IDX': sweep_idx})
+                env.update({'LMN_RUN_SWEEP_IDX': sweep_idx})
                 docker_conf = DockerContainerConfig(
                     image=image,
                     name=_name,
                     mounts=mounts,
                     startup=startup,
                     env=env,
                     user_id=user_id,
@@ -311,43 +312,43 @@
                                docker_conf,
                                interactive=not runtime_options.disown,
                                kill_existing_container=runtime_options.force)
 
 
     elif mode in ['slurm', 'slurm-sing', 'sing-slurm']:
         # Slurm specific configurations
-        from rmx.config import SlurmConfig
+        from lmn.config import SlurmConfig
         import randomname
         import random
         if 'slurm' not in machine.parsed_conf:
             raise ValueError('Configuration must have an entry for "slurm" to use slurm mode.')
 
         # NOTE: slurm seems to be fine with duplicated name.
         proj_name_maxlen = 15
         rand_num = random.randint(0, 100)
-        job_name = f'rmx-{project.name[:proj_name_maxlen]}-{randomname.get_name()}-{rand_num}'
+        job_name = f'lmn-{project.name[:proj_name_maxlen]}-{randomname.get_name()}-{rand_num}'
 
         # Parse from slurm config options (aside from default)
         if parsed.sconf is not None:
             logger.debug('parsed.sconf is specified. Loading custom preset conf.')
             sconf = preset.get('slurm-configs', {}).get(parsed.sconf, {})
             if sconf is None:
                 raise KeyError(f'configuration: {parsed.sconf} cannot be found in "slurm-configs".')
 
         else:
             sconf = machine.parsed_conf['slurm']
         slurm_conf = SlurmConfig(job_name, **sconf)
 
         # logger.info(f'slurm_conf: {machine.sconf}')
         ssh_client = SimpleSSHClient(machine.remote_conf)
-        slurm_runner = SlurmRunner(ssh_client, rmxdirs)
+        slurm_runner = SlurmRunner(ssh_client, lmndirs)
         run_opt = runtime_options
 
         # Specify job name
-        name = f'{machine.user}-rmx-{project.name}'
+        name = f'{machine.user}-lmn-{project.name}'
         if runtime_options.name is not None:
             name = f'{name}--{run_opt.name}'
         slurm_conf.job_name = name
 
         if mode in ['slurm-sing', 'sing-slurm']:
             # Decorate run_opt.cmd for Singularity
 
@@ -355,58 +356,68 @@
             if machine.parsed_conf is None or 'singularity' not in machine.parsed_conf:
                 raise ValueError('Entry "singularity" not found in the config file.')
 
             image = machine.parsed_conf.get('singularity', {}).get('sif_file')
             overlay = machine.parsed_conf.get('singularity', {}).get('overlay')
             writable_tmpfs = machine.parsed_conf.get('singularity', {}).get('writable_tmpfs', False)
 
-            # Overwrite rmx envvars.  Hmm I don't like this...
-            from rmx.cli._config_loader import DOCKER_ROOT_DIR, get_docker_rmxdirs
-            sing_rmxdirs = get_docker_rmxdirs(DOCKER_ROOT_DIR, project.name)
+            # Overwrite lmn envvars.  Hmm I don't like this...
+            from lmn.cli._config_loader import DOCKER_ROOT_DIR, get_docker_lmndirs
+            sing_lmndirs = get_docker_lmndirs(DOCKER_ROOT_DIR, project.name)
 
             # TODO: Do we need this??
             env.update({
-                'RMX_CODE_DIR': sing_rmxdirs.codedir, 
-                'RMX_MOUNT_DIR': sing_rmxdirs.mountdir,
-                'RMX_OUTPUT_DIR': sing_rmxdirs.outdir
+                'LMN_CODE_DIR': sing_lmndirs.codedir, 
+                'LMN_MOUNT_DIR': sing_lmndirs.mountdir,
+                'LMN_OUTPUT_DIR': sing_lmndirs.outdir
+            })
+
+            # Backward compat
+            env.update({
+                'RMX_CODE_DIR': sing_lmndirs.codedir,
+                'RMX_MOUNT_DIR': sing_lmndirs.mountdir,
+                'RMX_OUTPUT_DIR': sing_lmndirs.outdir
             })
 
             # NOTE: Without --containall, nvidia-smi command fails with "couldn't find libnvidia-ml.so library in your system."
             # NOTE: Without bash -c '{cmd}', if you put PYTHONPATH=/foo/bar, it fails with no such file or directory 'PYTHONPATH=/foo/bar'
             # TODO: Will the envvars be taken over to the internal shell (by this extra bash command)?
             # sing_cmd = "singularity run --nv --containall {options} {sif_file} bash -c '{cmd}'"
             sing_cmd = 'singularity run --nv --containall {options} {sif_file} bash -c -- "{cmd}"'
             options = []
 
             # Bind
             bind = '-B {source}:{target}'
             if not runtime_options.no_sync:
-                options += [bind.format(target=sing_rmxdirs.codedir, source=rmxdirs.codedir),
-                        bind.format(target=sing_rmxdirs.outdir, source=rmxdirs.outdir),
-                        bind.format(target=sing_rmxdirs.mountdir, source=rmxdirs.mountdir)]
+                options += [bind.format(target=sing_lmndirs.codedir, source=lmndirs.codedir),
+                            bind.format(target=sing_lmndirs.outdir, source=lmndirs.outdir),
+                            bind.format(target=sing_lmndirs.mountdir, source=lmndirs.mountdir)]
             options += [bind.format(target=tgt, source=src) for src, tgt in project.mount_from_host.items()]
 
             # Overlay
             if overlay:
                 options += [f'--overlay {overlay}']
 
             if writable_tmpfs:
                 # This often solves the following error:
                 # OSError: [Errno 30] Read-only file system
-                options += [f'--writable-tmpfs']
-
-            # TEMP: Only for tticslurm
-            assert 'CUDA_VISIBLE_DEVICES' not in env, 'CUDA_VISIBLE_DEVICES will be automatically set. You should not specify it manually.'
-            env['CUDA_VISIBLE_DEVICES'] = '$CUDA_VISIBLE_DEVICES'  # This let Singularity container use the envvar on the host
+                options += ['--writable-tmpfs']
 
             # Environment variables
+            # TODO: Better to use --env-file option and read from a file
+            # Escaping quotes and commas will be much easier in that way.
             options += ['--env ' + ','.join(f'{key}="{val}"' for key, val in env.items())]
 
+            # NOTE: Since CUDA_VISIBLE_DEVICES is often comma-separated values (i.e., CUDA_VISIBLE_DEVICES=0,1),
+            # and `singularity run --env FOO=BAR,HOGE=PIYO` considers comma to be a separator for envvars,
+            # It fails without special handling.
+            env_from_host = ['CUDA_VISIBLE_DEVICES']
+
             # Workdir
-            _workdir = sing_rmxdirs.codedir / runtime_options.rel_workdir
+            _workdir = sing_lmndirs.codedir / runtime_options.rel_workdir
             options += [f'--pwd {_workdir}']
 
             # Overwrite command
             options = ' '.join(options)
 
             # Trying my best to escape quotations (https://stackoverflow.com/a/18886646/19913466)
             logger.debug(f'run_opt.cmd before escape: {run_opt.cmd}')
@@ -423,30 +434,31 @@
             _slurm_conf = deepcopy(slurm_conf)
             for sweep_idx in sweep_ind:
                 # NOTE: This special prefix "SINGULARITYENV_" is stripped and the rest is passed to singularity container,
                 # even with --containall or --cleanenv !!
                 # Example: (https://docs.sylabs.io/guides/3.1/user-guide/environment_and_metadata.html?highlight=environment%20variable)
                 #     $ SINGULARITYENV_HELLO=world singularity exec centos7.img env | grep HELLO
                 #     HELLO=world
-                env.update({'SINGULARITYENV_RMX_RUN_SWEEP_IDX': sweep_idx})
+                env.update({'SINGULARITYENV_LMN_RUN_SWEEP_IDX': sweep_idx})
 
-                # Oftentimes, a user specifies $RMX_RUN_SWEEP_IDX as an argument to the command, and that will be evaluated right before singularity launches
-                env.update({'RMX_RUN_SWEEP_IDX': sweep_idx})
+                # Oftentimes, a user specifies $LMN_RUN_SWEEP_IDX as an argument to the command,
+                # and that will be evaluated right before singularity launches
+                env.update({'LMN_RUN_SWEEP_IDX': sweep_idx})
 
                 _name = f'{slurm_conf.job_name}-{sweep_idx}'
                 logger.info(f'Launching sweep {sweep_idx}: {_name}')
                 _slurm_conf.job_name = _name
                 slurm_runner.exec(run_opt.cmd, run_opt.rel_workdir, slurm_conf=_slurm_conf,
                                   startup=startup,
                                   interactive=False, num_sequence=run_opt.num_sequence,
-                                  env=env, dry_run=run_opt.dry_run)
+                                  env=env, env_from_host=env_from_host, dry_run=run_opt.dry_run)
         else:
             slurm_runner.exec(run_opt.cmd, run_opt.rel_workdir, slurm_conf=slurm_conf,
                               startup=startup, interactive=not run_opt.disown, num_sequence=run_opt.num_sequence,
-                              env=env, dry_run=run_opt.dry_run)
+                              env=env, env_from_host=env_from_host, dry_run=run_opt.dry_run)
     else:
         raise ValueError(f'Unrecognized mode: {mode}')
 
     # Sync output files
     if not runtime_options.no_sync:
         _sync_output(project, machine, dry_run=parsed.dry_run)
```

### Comparing `lmn-0.2.4rc1/rmx/cli/sync.py` & `lmn-0.2.5/lmn/cli/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from argparse import ArgumentParser, Namespace
-from rmx import logger
-from rmx.cli._utils import rsync
-from rmx.cli._config_loader import Project, Machine
-from rmx.machine import SimpleSSHClient
+from lmn import logger
+from lmn.cli._utils import rsync
+from lmn.cli._config_loader import Project, Machine
+from lmn.machine import SimpleSSHClient
 
 
 RSYNC_DESTINATION_PATH = "/tmp/".rstrip('/')
 
 
 def _get_parser() -> ArgumentParser:
     parser = ArgumentParser()
@@ -24,48 +24,48 @@
     )
     return parser
 
 def _sync_code(project: Project, machine: Machine, dry_run: bool = False):
     # rsync_options = f"--rsync-path='mkdir -p {project.remote_dir} && mkdir -p {project.remote_outdir} && mkdir -p {project.remote_mountdir} && rsync'"
 
     # A trick to create directories right before performing rsync
-    rmxdirs = machine.get_rmxdirs(project.name)
-    rsync_options = f"--rsync-path='mkdir -p {rmxdirs.codedir} && mkdir -p {rmxdirs.outdir} && mkdir -p {rmxdirs.mountdir} && rsync'"
+    lmndirs = machine.get_lmndirs(project.name)
+    rsync_options = f"--rsync-path='mkdir -p {lmndirs.codedir} && mkdir -p {lmndirs.outdir} && mkdir -p {lmndirs.mountdir} && rsync'"
 
     try:
-        rsync(source_dir=project.rootdir, target_dir=machine.uri(rmxdirs.codedir),
+        rsync(source_dir=project.rootdir, target_dir=machine.uri(lmndirs.codedir),
                         exclude=project.exclude, options=rsync_options, dry_run=dry_run, transfer_rootdir=False)
 
         # rsync the directories to mount
         for mount_dir in project.mount_dirs:
-            rsync(source_dir=mount_dir, target_dir=machine.uri(rmxdirs.mountdir),
+            rsync(source_dir=mount_dir, target_dir=machine.uri(lmndirs.mountdir),
                                 exclude=project.exclude, dry_run=dry_run)
     except OSError:
         import traceback
         import sys
         print(traceback.format_exc(0), file=sys.stderr)
         sys.exit(1)
 
 
 
 def _sync_output(project: Project, machine: Machine, dry_run: bool = False):
     # Rsync remote outdir with the local outdir.
     if project.outdir:
         try:
-            rmxdirs = machine.get_rmxdirs(project.name)
+            lmndirs = machine.get_lmndirs(project.name)
             # Check if there's any output file (the first line is always 'total [num-files]')
             ssh_client = SimpleSSHClient(machine.remote_conf)
 
-            result = ssh_client.run(f'ls -l {rmxdirs.outdir} | grep -v "^total" | wc -l', hide=True)
+            result = ssh_client.run(f'ls -l {lmndirs.outdir} | grep -v "^total" | wc -l', hide=True)
             num_output_files = int(result.stdout)
 
             msg = f'{num_output_files} files are in the output directory'
             logger.info(msg)
             if num_output_files > 0:
-                rsync(source_dir=machine.uri(rmxdirs.outdir), target_dir=project.outdir,
+                rsync(source_dir=machine.uri(lmndirs.outdir), target_dir=project.outdir,
                     dry_run=dry_run)
                 logger.info(f'The output files are copied to {str(project.outdir)}')
 
         except OSError:
             # NOTE: Only show the last stack of traceback (If I remember corectly...)
             import traceback
             import sys
```

### Comparing `lmn-0.2.4rc1/rmx/config.py` & `lmn-0.2.5/lmn/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 import os
 from os.path import expandvars
 import docker
-from rmx import logger
+from lmn import logger
 
 class DockerContainerConfig:
     def __init__(self, image, name, env: dict | None = None, remove=True, network='host', ipc_mode='host', mounts=None,
                  startup: str | None = None, tty=True, use_gpus=True, user_id: int = 0, group_id: int = 0, runtime='docker') -> None:
         """
         user_id (int | str): The format is either 2003 for user_id or 2003:4000 to specify user id and group id.
         """
@@ -66,15 +66,15 @@
         if not shutil.which(xhost_command):
             raise OSError('xhost not found. If you are on macOS, you need to install XQuartz.')
 
         # If using XQuartz, the display variables looks
         # something like: /private/tmp/com.apple.launchd.jY5AhC1lFM/org.xquartz:0
         # which doesn't work (??)
         if 'xquartz' in os.environ.get('DISPLAY', ''):
-            from rmx.utils import run_cmd
+            from lmn.utils import run_cmd
             ip = run_cmd('ifconfig en0 | grep inet | awk \'$1=="inet" {print $2}\'', get_output=True, shell=True)
             display = f'{ip}:0'
         else:
             display = os.environ.get('DISPLAY', ':0'),
 
         # TODO: In addition to this, there needs to be a X forwarding from the remote to local
         # paramiko should support that.
```

### Comparing `lmn-0.2.4rc1/rmx/helpers.py` & `lmn-0.2.5/lmn/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -40,104 +40,104 @@
                 else:
                     raise ValueError('Conflict at %s' % '.'.join(path + [str(key)]))
         else:
             a[key] = b[key]
     return a
 
 
-def parse_config(project_root, global_conf_paths=['${HOME}/.rmx.config', '${HOME}/.config/rmx']):
-    """ Parse rmx config (json file)
+def parse_config(project_root):
+    """Parse lmn config (json file).
 
     It looks for config file in this order:
-    1. {project_root}/.rmx.config
-    2. $HOME/.rmx.config
-    3. $HOME/.config/rmx
+    1. {project_root}/.lmn.json5
+    3. $HOME/.config/lmn.json5
     """
     import pyjson5 as json
 
     from os.path import expandvars, isfile
-    from rmx import logger
+    from lmn import logger
+    from lmn.const import global_config_paths, local_config_fnames
 
     def _maybe_load(path):
         if isfile(path):
             with open(path, 'r') as f:
                 return json.load(f)
         return {}
 
     # TODO: Hmmm... a better way to write this config search algorithm?
     path_found = False
-    for path in global_conf_paths:
+    for path in global_config_paths:
         path = expandvars(path)
         if isfile(path):
             path_found = True
             break
 
     if path_found:
         with open(path, 'r') as f:
             global_conf = json.load(f)
     else:
-        logger.warning('rmx global config file cannot be located.')
+        logger.error('lmn global config file cannot be located. Please place the config file at ~/.config/lmn.json5')
         global_conf = {}
+        exit(1)
 
-    local_conf = _maybe_load(f'{project_root}/.rmx.config')
+    # Loop over possible local config file names
+    for local_conf_fname in local_config_fnames:
+        local_conf = _maybe_load(f'{project_root}/{local_conf_fname}')
 
-    global_conf = remove_recursively(global_conf, key='__help')
-    local_conf = remove_recursively(local_conf, key='__help')
+        if local_conf:
+            break
 
     merged_conf = merge_nested_dict(global_conf, local_conf)
     return merged_conf
 
-def remove_recursively(config_dict, key='__help'):
-    """remove entry with the specified key recursively."""
-    for k in list(config_dict.keys()):
-        if k == key:
-            del config_dict[k]
-            continue
-        if isinstance(config_dict[k], dict):
-            config_dict[k] = remove_recursively(config_dict[k], key=key)
-
-    return config_dict
-
 
 def find_project_root():
     """Find a project root (which is rsync-ed with the remote server).
 
-    It first goes up in the directory tree to find ".git" or ".rmx.config" file.
+    It first goes up in the directory tree to find ".git" or ".lmn.json5" file.
     If not found, print warning and just use the current directory
     """
-    from rmx import logger
+    from lmn import logger
+    from lmn.const import local_config_fnames
     def is_proj_root(directory: Path):
         if (directory / '.git').is_dir():
             return True
-        if (directory / '.rmx.config').is_file():
-            return True
+        for local_conf_fname in local_config_fnames:
+            if (directory / local_conf_fname).is_file():
+                return True
         return False
 
     current_dir = Path(os.getcwd()).resolve()
     if is_proj_root(current_dir):
         return current_dir
 
     for directory in yield_parents(current_dir):
         if is_proj_root(directory):
             return directory
 
-    logger.warning('.git directory or .rmx file not found in the ancestor directories.\n'
-                'Setting project root to current directory')
+    logger.warning('.git directory or .lmn.json5 file not found in the ancestor directories.\n'
+                   'Setting project root to current directory')
 
-    assert not is_system_root(current_dir), "project root detected is the system root '/' you never want to rsync your entire disk."
-    assert not is_home_dir(current_dir), "project root detected is home directory. You never want to rsync the entire home directory to a remote machine."
-    return current_dir
+    if is_system_root(current_dir):
+        logger.error("project root detected is the system root '/' you never want to rsync your entire disk.")
+        exit(1)
+
+    if is_home_dir(current_dir):
+        logger.error("project root detected is home directory. You never want to rsync the entire home directory to a remote machine.")
+        exit(1)
 
+    return current_dir
 
 
 TIMESTAMP_FORMAT = '%Y-%m-%d_%H%M%S-%f'
 from datetime import datetime
 def get_timestamp() -> str:
     return datetime.strftime(datetime.now(), TIMESTAMP_FORMAT)
 
+
 def read_timestamp(time_str: str) -> datetime:
     return datetime.strptime(time_str, TIMESTAMP_FORMAT)
 
 
 def wrap_shebang(command, shell='bash'):
     return f"#!/usr/bin/env {shell}\n{command}"
 
@@ -146,15 +146,15 @@
 
 
 def parse_sacct(sacct_output):
     lines = sacct_output.strip().split('\n')
     keys = lines[0].split('|')
     entries = [{key: entry for key, entry in zip(keys, line.split('|'))} for line in lines[1:]]
     # NOTE: For a batch job, sacct shows two entries for one job submission:
-    # {'JobID': '8231686', 'JobName': 'rmx-iti-coped-chief-97', ... 'MaxRSS': ''},
+    # {'JobID': '8231686', 'JobName': 'lmn-iti-coped-chief-97', ... 'MaxRSS': ''},
     # {'JobID': '8231686.batch', 'JobName': 'batch', ... 'MaxRSS': '64844148K'}
     # We should merge these into one.
     # TEMP: Forget about MaxRSS, and just remove all entries with *.batch
     entries = [entry for entry in entries if not entry['JobID'].endswith('.batch')]
     return entries
 
 
@@ -170,47 +170,40 @@
         return obj
 
 
 def defreeze_dict(frozen_dict: frozenset):
     return {key: val for key, val in frozen_dict}
 
 
-def replace_rmx_envvars(query: str, rmxenvs: dict):
+def replace_lmn_envvars(query: str, lmnenvs: dict):
     """
-    Replace RMX_* envvars (i.e., ${RMX_CODE_DIR}, ${RMX_OUTPUT_DIR}, ${RMX_MOUNT_DIR}) with actual path
-    Args
-      query (string): input string to process
-      rmxenvs (dict): map from RMX_* envvars to actual paths
+    Replace LMN_* envvars (i.e., ${LMN_CODE_DIR}, ${LMN_OUTPUT_DIR}, ${LMN_MOUNT_DIR}) with actual path.
+
+    Args:
+      - query (string): input string to process
+      - lmnenvs (dict): map from LMN_* envvars to actual paths
+
     """
     import re
-    rmx_envvars = ['RMX_CODE_DIR', 'RMX_OUTPUT_DIR', 'RMX_MOUNT_DIR']
-    for original in rmx_envvars:
+    lmn_envvars = ['LMN_CODE_DIR', 'LMN_OUTPUT_DIR', 'LMN_MOUNT_DIR']
+
+    # Backward compatibility
+    lmn_envvars += ['RMX_CODE_DIR', 'RMX_OUTPUT_DIR', 'RMX_MOUNT_DIR']
+
+    for original in lmn_envvars:
         # Match "${original}" or "$original"
-        regex = r'{}'.format('(\$\{' + original + '\}' + f'|\$' + original + ')')
-        target = rmxenvs[original]
+        regex = r'{}'.format('(\$\{' + original + '\}' + '|\$' + original + ')')
+        target = lmnenvs[original]
         query = re.sub(regex, str(target), str(query))
     return query
 
 
-# def replace_rmx_envvars(env: dict):
-#     import re
-#     # Replace RMX_* envvars: (${RMX_CODE_DIR}, ${RMX_OUTPUT_DIR}, ${RMX_MOUNT_DIR})
-#     # This cannot happen automatically on remote server side, since we set these envvars exactly at the same time as other envvars.
-#     rmx_envvars = ['RMX_CODE_DIR', 'RMX_OUTPUT_DIR', 'RMX_MOUNT_DIR']
-#     for original in rmx_envvars:
-#         # Match "${original}" or "$original"
-#         regex = r'{}'.format('(\$\{' + original + '\}' + f'|\$' + original + ')')
-#         target = str(env[original])
-#         env = {key: re.sub(regex, target, str(val)) for key, val in env.items()}
-#     return env
-
-
 from os.path import expandvars
 class LaunchLogManager:
-    def __init__(self, path=expandvars('$HOME/.rmx/launched.jsonl')) -> None:
+    def __init__(self, path=expandvars('$HOME/.lmn/launched.jsonl')) -> None:
         self.path = path
 
     def _refresh(self):
         import pyjson5 as json
         from datetime import datetime
         # Read entries from the top (oldest) to bottom (newest)
         with open(self.path, 'r') as f:
```

### Comparing `lmn-0.2.4rc1/rmx/machine.py` & `lmn-0.2.5/lmn/machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 import os
 from os.path import expandvars
-from rmx.helpers import posixpath2str, replace_rmx_envvars
+from lmn.helpers import posixpath2str, replace_lmn_envvars
 import invoke
 
-from rmx import logger
+from lmn import logger
 
-RMX_DOCKER_ROOTDIR = '/rmx'
+LMN_DOCKER_ROOTDIR = '/lmn'
 
 # NOTE: Should I have ssh-conf, slurm-conf and docker-conf separately??
 # I guess RemoteConfig should ONLY store the info on how to login to the host?
 # docker info and slurm info should really reside in project.
 class RemoteConfig:
     """Represents a configuration to connect to a remote server.
     This is used by SimpleSSHClient.
```

### Comparing `lmn-0.2.4rc1/rmx/runner.py` & `lmn-0.2.5/lmn/runner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,77 @@
 from __future__ import annotations
 from argparse import Namespace
-from typing import Iterable
+from typing import Iterable, List, Optional
+from io import StringIO
 import threading
-from rmx import logger
+from lmn import logger
 from docker import DockerClient
-from rmx.config import DockerContainerConfig
-from rmx.machine import SimpleSSHClient
-from rmx.helpers import replace_rmx_envvars
-
-def get_rmxenvs(cmd: str, rmxdirs: Namespace):
-    return {'RMX_CODE_DIR': rmxdirs.codedir, 
-            'RMX_MOUNT_DIR': rmxdirs.mountdir,
-            'RMX_OUTPUT_DIR': rmxdirs.outdir,
-            'RMX_USER_COMMAND': cmd}
+from lmn.config import DockerContainerConfig
+from lmn.machine import SimpleSSHClient
+from lmn.helpers import replace_lmn_envvars
+
+def get_lmnenvs(cmd: str, lmndirs: Namespace):
+    envvars = {
+        "LMN_CODE_DIR": lmndirs.codedir,
+        "LMN_MOUNT_DIR": lmndirs.mountdir,
+        "LMN_OUTPUT_DIR": lmndirs.outdir,
+        "LMN_USER_COMMAND": cmd,
+    }
+
+    # Provide RMX_* envvars for backward compatibility
+    return {
+        **envvars,
+        **{key.replace("LMN", "RMX"): val for key, val in envvars.items()},
+    }
 
 
 class SSHRunner:
-    def __init__(self, client: SimpleSSHClient, rmxdirs: Namespace) -> None:
+    def __init__(self, client: SimpleSSHClient, lmndirs: Namespace) -> None:
         self.client = client
-        self.rmxdirs = rmxdirs
+        self.lmndirs = lmndirs
 
     def exec(self, cmd: str, relative_workdir, env: dict | None = None, startup: str = "", dry_run: bool = False,
              disown: bool = False):
         env = {} if env is None else env
         # if isinstance(cmd, list):
         #     cmd = ' '.join(cmd) if len(cmd) > 1 else cmd[0]
 
         if startup:
             cmd = f'{startup} && {cmd}'
 
         logger.debug(f'ssh run with command: {cmd}')
-        logger.debug(f'cd to {self.rmxdirs.codedir / relative_workdir}')
-        rmxenv = get_rmxenvs(cmd, self.rmxdirs)
-        allenv = {**env, **rmxenv}
-        allenv = {key: replace_rmx_envvars(val, rmxenv) for key, val in allenv.items()}
-        return self.client.run(cmd, directory=(self.rmxdirs.codedir / relative_workdir),
+        logger.debug(f'cd to {self.lmndirs.codedir / relative_workdir}')
+        lmnenv = get_lmnenvs(cmd, self.lmndirs)
+        allenv = {**env, **lmnenv}
+        allenv = {key: replace_lmn_envvars(val, lmnenv) for key, val in allenv.items()}
+        return self.client.run(cmd, directory=(self.lmndirs.codedir / relative_workdir),
                                disown=disown, env=allenv, dry_run=dry_run, pty=True)
 
 
 class DockerRunner:
-    def __init__(self, client: DockerClient, rmxdirs: Namespace) -> None:
+    def __init__(self, client: DockerClient, lmndirs: Namespace) -> None:
         self.client = client
-        self.rmxdirs = rmxdirs
+        self.lmndirs = lmndirs
 
     def exec(self, cmd: str, relative_workdir, docker_conf: DockerContainerConfig,
              kill_existing_container: bool = True, interactive: bool = True, quiet: bool = False,
              log_stderr_background: bool = False, use_cli: bool = True) -> None:
         if log_stderr_background:
             assert not interactive, 'log_stderr_background=True cannot be used with interactive=True'
 
-        rmxenv = get_rmxenvs(cmd, self.rmxdirs)
-        allenv = {**docker_conf.env, **rmxenv}
-        allenv = {key: replace_rmx_envvars(val, rmxenv) for key, val in allenv.items()}
+        lmnenv = get_lmnenvs(cmd, self.lmndirs)
+        allenv = {**docker_conf.env, **lmnenv}
+        allenv = {key: replace_lmn_envvars(val, lmnenv) for key, val in allenv.items()}
 
         # NOTE: target: container, source: remote host
         logger.debug(f'mounts: {docker_conf.mounts}')
         logger.debug(f'docker_conf: {docker_conf}')
 
 
-        logger.debug(f'container codedir: {str(self.rmxdirs.codedir / relative_workdir)}')
+        logger.debug(f'container codedir: {str(self.lmndirs.codedir / relative_workdir)}')
 
         if kill_existing_container:
             from docker.errors import NotFound
             import docker
             try:
                 container = self.client.containers.get(docker_conf.name)
             except NotFound:
@@ -85,15 +94,15 @@
             if docker_conf.startup:
                 docker_conf.startup = ' && '.join((docker_conf.startup, 'sleep 2'))
             else:
                 docker_conf.startup = 'sleep 2'
 
         if docker_conf.startup:
             cmd = ' && '.join((docker_conf.startup, cmd))
-        cmd = f'{cmd} && chmod -R a+rw {str(self.rmxdirs.outdir)}'
+        cmd = f'{cmd} && chmod -R a+rw {str(self.lmndirs.outdir)}'
 
         if interactive:
             assert d.tty
 
             if use_cli:
                 # Use python-on-whales (i.e., docker cli)
                 import python_on_whales
@@ -104,15 +113,15 @@
                 # dockerpty is good but fails when the terminal size changes frantically.
                 # Let's wait for docker team to properly merge dockerpty.
                 # Or I should probably think about migrating to https://github.com/gabrieldemarmiesse/python-on-whales
                 # ^ This one just calls docker cli via Python, rather than using the complicated Docker SDK.
                 # options = [
                 #     '-it',
                 #     '--gpus', 'all',
-                #     '--workdir', str(self.rmxdirs.codedir / relative_workdir),
+                #     '--workdir', str(self.lmndirs.codedir / relative_workdir),
                 #     '--user', d.user_id,
                 #     '--name', d.name,
                 # ]
                 # if d.network:
                 #     options += ['--net', d.network]
                 # if d.ipc_mode:
                 #     options += ['--ipc', d.ipc_mode]
@@ -146,15 +155,15 @@
                         ipc=d.ipc_mode,
                         mounts=[('type=bind', f'source={m["Source"]}', f'destination={m["Target"]}') for m in d.mounts],
                         name=d.name,
                         networks=[d.network],
                         remove=True,
                         tty=True,
                         user=f'{d.user_id}:{d.group_id}',
-                        workdir=str(self.rmxdirs.codedir / relative_workdir),
+                        workdir=str(self.lmndirs.codedir / relative_workdir),
                     )
                 except python_on_whales.exceptions.DockerException as e:
                     # NOTE: hide error as the exception is also raised when the command in the container returns non-zero exit value.
                     import traceback
                     import sys
                     logger.debug(f'python_on_whales failed!!:\n{str(e)}')
                     logger.debug(traceback.format_exc())
@@ -172,15 +181,15 @@
                                                           ipc_mode=d.ipc_mode,
                                                           detach=False,
                                                           tty=True,
                                                           stdin_open=True,
                                                           mounts=d.mounts,
                                                           environment=allenv,
                                                           device_requests=d.device_requests,
-                                                          working_dir=str(self.rmxdirs.codedir / relative_workdir),
+                                                          working_dir=str(self.lmndirs.codedir / relative_workdir),
                                                           user=f'{d.user_id}:{d.group_id}',
                                                           # entrypoint='/bin/bash -c "sleep 10 && xeyes"'  # Use it if you wanna overwrite entrypoint
                                                     )
                 logger.debug(f'container: {container}')
                 import dockerpty
                 dockerpty.start(self.client.api, container.id)
 
@@ -194,15 +203,15 @@
                                                    ipc_mode=d.ipc_mode,
                                                    detach=True,
                                                    tty=(not log_stderr_background),  # If True, stdout/stderr are mixed, but I observed sometimes some stdout are not showing up when tty=False
                                                    stdin_open=True,  # It's useful to keep it open, as you may manually attach the container later
                                                    mounts=d.mounts,
                                                    environment=allenv,
                                                    device_requests=d.device_requests,
-                                                   working_dir=str(self.rmxdirs.codedir / relative_workdir),
+                                                   working_dir=str(self.lmndirs.codedir / relative_workdir),
                                                    user=f'{d.user_id}:{d.group_id}',
                                                 )
             logger.debug(f'container: {container}')
 
             def log_stream(stream: Iterable):
                 """print out log stream"""
                 for char in stream:
@@ -229,24 +238,28 @@
 
 
 class SlurmRunner:
     """Use srun/sbatch to submit the command on a remote machine.
     If your local machine has slurm (i.e., you're on slurm login-node), I guess you don't need this tool.
     Thus SlurmMachine inherits SSHMachine.
     """
-    def __init__(self, client: SimpleSSHClient, rmxdirs: Namespace) -> None:
+    def __init__(self, client: SimpleSSHClient, lmndirs: Namespace) -> None:
         self.client = client
-        self.rmxdirs = rmxdirs
+        self.lmndirs = lmndirs
 
-    def exec(self, cmd: str, relative_workdir, slurm_conf, env: dict | None = None,
+    def exec(self, cmd: str, relative_workdir, slurm_conf, env: Optional[dict] = None,
+             env_from_host: List[str] = [],
              startup: str = "", num_sequence: int = 1,
              interactive: bool = None, dry_run: bool = False):
         from simple_slurm_command import SlurmCommand
         env = {} if env is None else env
 
+        # TODO: Verify env_from_list contains valid environment variable names
+        # (i.e., cannot have spaces or quotes!!)
+
         if isinstance(cmd, list):
             cmd = ' '.join(cmd)
 
         if num_sequence > 1:
             # Use sbatch and set dependency to singleton
             slurm_conf.dependency = 'singleton'
             if interactive:
@@ -265,42 +278,63 @@
                                      output=s.output,
                                      error=s.error)
 
         if interactive and (s.output is not None):
             # User may expect stdout shown on the console.
             logger.info('--output/--error argument for Slurm is ignored in interactive mode.')
 
-        rmxenv = get_rmxenvs(cmd, self.rmxdirs)
-        allenv = {**env, **rmxenv}
-        allenv = {key: replace_rmx_envvars(val, rmxenv) for key, val in allenv.items()}
+        lmnenv = get_lmnenvs(cmd, self.lmndirs)
+        allenv = {**env, **lmnenv}
+        allenv = {key: replace_lmn_envvars(val, lmnenv) for key, val in allenv.items()}
 
         if startup:
             cmd = f'{startup} && {cmd}'
 
+        workdir = self.lmndirs.codedir / relative_workdir
         if interactive:
             # cmd = f'{shell} -i -c \'{cmd}\''
             # Create a temp bash file and put it on the remote server.
-            workdir = self.rmxdirs.codedir / relative_workdir
-            exec_file = f"#!/usr/bin/env {s.shell}\n{cmd}"
+            exec_file = '\n'.join((
+                f'#!/usr/bin/env {s.shell}',
+                *[f'export SINGULARITYENV_{envvar}=${envvar}' for envvar in env_from_host],
+                cmd
+            ))
             logger.debug(f'exec file: {exec_file}')
-            from io import StringIO
-            # file_obj = StringIO(f"#!/usr/bin/env {s.shell}\n{cmd}\n{s.shell}")
             file_obj = StringIO(exec_file)
             self.client.put(file_obj, workdir / '.srun-script.sh')
             cmd = slurm_command.srun('.srun-script.sh', pty=s.shell)
 
             logger.debug(f'srun mode:\n{cmd}')
             logger.debug(f'cd to {workdir}')
             return self.client.run(cmd, directory=workdir,
                                    disown=False, env=allenv, pty=True, dry_run=dry_run)
         else:
-            cmd = slurm_command.sbatch(cmd, shell=f'/usr/bin/env {s.shell}')
-            logger.debug(f'sbatch mode:\n{cmd}')
-            logger.debug(f'cd to {self.rmxdirs.codedir / relative_workdir}')
+            sbatch_cmd = slurm_command.sbatch(cmd, shell=f'/usr/bin/env {s.shell}')
+
+            # HACK: rather than submitting with `sbatch << EOF\n ...\n EOF`,
+            # I use `sbatch file-name` to avoid `$ENVVAR` to be evaluated right at the submission time
+            # I want the `$ENVVAR` to be evaluated after the compute is allocated.
+            sbatch_lines = sbatch_cmd.split('\n')[1:-1]  # Strip `sbatch << EOF` and `EOF`
+
+            if env_from_host:
+                # HACK: Inject `export` for exposing envvars to singularity container,
+                # right after the last line that starts with `#SBATCH`.
+                exports = [f'export SINGULARITYENV_{envvar}=${envvar}' for envvar in env_from_host]
+                sbatch_lines = sbatch_lines[:-1] + exports + sbatch_lines[-1:]
+            exec_file = '\n'.join(sbatch_lines)
+
+            # TODO: If you're running a sweep, the content of the file should stay the same.
+            # thus there shouldn't be a need to run these every time.
+            file_obj = StringIO(exec_file)
+            self.client.put(file_obj, workdir / '.sbatch-script.sh')
+
+            logger.debug(f'sbatch mode\n===============\n{exec_file}\n===============')
+            logger.debug(f'cd to {self.lmndirs.codedir / relative_workdir}')
 
+            cmd = 'sbatch .sbatch-script.sh'
             cmd = '\n'.join([cmd] * num_sequence)
-            result = self.client.run(cmd, directory=(self.rmxdirs.codedir / relative_workdir),
+            result = self.client.run(cmd, directory=workdir,
                                      disown=False, env=allenv, dry_run=dry_run)
             if result.stderr:
                 logger.warning('sbatch job submission failed:', result.stderr)
             jobid = result.stdout.strip().split()[-1]  # stdout format: Submitted batch job 8156833
             logger.debug(f'jobid {jobid}')
```

### Comparing `lmn-0.2.4rc1/tests/test_config.py` & `lmn-0.2.5/tests/test_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 import unittest
-from rmx.helpers import parse_config, merge_nested_dict, remove_recursively
+from lmn.helpers import parse_config, merge_nested_dict
 
 class TestMergeDicts(unittest.TestCase):
     def test_flat_dict(self):
         """Merging flat dictionaries"""
         a = {'apple': 1, 'orange': 2}
         b = {'pearl': 3, 'lemon': 4}
         merged = merge_nested_dict(a, b)
@@ -56,23 +56,9 @@
             'slurm-configs': {'two-cpus': 'yeah'},
             'docker-images': {'image0': ['bar', 'piyo']}
         }
         merged = merge_nested_dict(a, b)
         self.assertDictEqual(gold, merged)
 
 
-class TestRemoveRecursively(unittest.TestCase):
-    def test_remove_recursively(self):
-        a = {
-            '__help': 'hoge',
-            'key1': 'val1',
-            'key2': {'__help': 'fuga', 'key2-1': 'val2-1'}
-        }
-        gold = {
-            'key1': 'val1',
-            'key2': {'key2-1': 'val2-1'}
-        }
-        cleaned = remove_recursively(a, key='__help')
-        self.assertDictEqual(cleaned, gold)
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `lmn-0.2.4rc1/PKG-INFO` & `lmn-0.2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: lmn
-Version: 0.2.4rc1
-Summary: Remote code deployment and execution for ML researchers.
+Version: 0.2.5
+Summary: LMN: LaMbda functions across servers for Noobs
 License: MIT License
 Author-email: Takuma Yoneda <takuma-yoneda@users.noreply.github.com>,Takuma Yoneda <takuma.ynd@gmail.com>
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Project-URL: Homepage, https://github.com/takuma-yoneda/rmx
+Project-URL: Homepage, https://github.com/takuma-yoneda/lmn
 Description-Content-Type: text/markdown
 
 <div align="center">
 
-# RMX - Remote code deployment & execution tool
-<!-- <a href="https://github.com/takuma-yoneda/rmx/actions/workflows/python-publish-pypi.yml"> -->
-<!--     <img src="https://github.com/takuma-yoneda/rmx/actions/workflows/python-publish-pypi.yml/badge.svg" alt="Publish to PyPI" /> -->
+# 🍋 LMN - LaMbda functionality across servers for Noobs
+<!-- <a href="https://github.com/takuma-yoneda/lmn/actions/workflows/python-publish-pypi.yml"> -->
+<!--     <img src="https://github.com/takuma-yoneda/lmn/actions/workflows/python-publish-pypi.yml/badge.svg" alt="Publish to PyPI" /> -->
 <!-- </a> -->
 
 A lightweight tool to rsync and execute local scripts in a remote machine.
 
-<a href="https://github.com/takuma-yoneda/rmx/actions/workflows/python-run-tests.yml">
-    <img src="https://github.com/takuma-yoneda/rmx/actions/workflows/python-run-tests.yml/badge.svg" alt="Test" />
+<a href="https://github.com/takuma-yoneda/lmn/actions/workflows/python-run-tests.yml">
+    <img src="https://github.com/takuma-yoneda/lmn/actions/workflows/python-run-tests.yml/badge.svg" alt="Test" />
 </a>
-<a href="https://github.com/takuma-yoneda/rmx">
-    <img src="https://tokei.rs/b1/github/takuma-yoneda/rmx" alt="Total lines" />
+<a href="https://github.com/takuma-yoneda/lmn">
+    <img src="https://tokei.rs/b1/github/takuma-yoneda/lmn" alt="Total lines" />
 </a>
-<a href="https://pypi.org/project/rmx/">
-    <img src="https://img.shields.io/pypi/v/rmx?logo=python&logoColor=%23cccccc" alt="PyPI" />
+<a href="https://pypi.org/project/lmn/">
+    <img src="https://img.shields.io/pypi/v/lmn?logo=python&logoColor=%23cccccc" alt="PyPI" />
 </a>
 </div>
 
 Inspired by [afdaniele/cpk](https://github.com/afdaniele/cpk) and [geyang/jaynes](https://github.com/geyang/jaynes).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: lmn Version: 0.2.4rc1 Summary: Remote code
-deployment and execution for ML researchers. License: MIT License Author-email:
-Takuma Yoneda
+Metadata-Version: 2.1 Name: lmn Version: 0.2.5 Summary: LMN: LaMbda functions
+across servers for Noobs License: MIT License Author-email: Takuma Yoneda
 users.noreply.github.com>,Takuma Yoneda
 ynd@gmail.com> Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: MacOS Classifier: Operating System
 :: POSIX Classifier: Operating System :: Unix Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Project-URL:
-Homepage, https://github.com/takuma-yoneda/rmx Description-Content-Type: text/
+Homepage, https://github.com/takuma-yoneda/lmn Description-Content-Type: text/
 markdown
-# RMX - Remote code deployment & execution tool    A lightweight tool to rsync
-  and execute local scripts in a remote machine. [Test] [Total_lines] [PyPI]
+  # ð LMN - LaMbda functionality across servers for Noobs    A lightweight
+  tool to rsync and execute local scripts in a remote machine. [Test] [Total
+                                 lines] [PyPI]
 Inspired by [afdaniele/cpk](https://github.com/afdaniele/cpk) and [geyang/
 jaynes](https://github.com/geyang/jaynes).
```

