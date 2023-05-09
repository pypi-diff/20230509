# Comparing `tmp/freva_deployment-2305.0.1.tar.gz` & `tmp/freva_deployment-2305.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freva_deployment-2305.0.1.tar", last modified: Mon May  8 15:03:24 2023, max compression
+gzip compressed data, was "freva_deployment-2305.0.2.tar", last modified: Tue May  9 03:21:18 2023, max compression
```

## Comparing `freva_deployment-2305.0.1.tar` & `freva_deployment-2305.0.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.749595 freva_deployment-2305.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-05-08 15:03:24.745595 freva_deployment-2305.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.737595 freva_deployment-2305.0.1/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.737595 freva_deployment-2305.0.1/assets/config/
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/config/create_tables.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/config/evaluation_system.conf.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/config/inventory.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.737595 freva_deployment-2305.0.1/assets/db_service/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/db_service/password_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/db_service/reset_root_pw.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.741595 freva_deployment-2305.0.1/assets/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/playbooks/core-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/playbooks/db-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/playbooks/server-map-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/playbooks/solr-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/playbooks/vault-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/playbooks/web-server-playbook.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.741595 freva_deployment-2305.0.1/assets/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/scripts/create_cron.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/scripts/create_systemd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/scripts/docker-or-podman
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/scripts/dump_sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.741595 freva_deployment-2305.0.1/assets/servers/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/servers/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.741595 freva_deployment-2305.0.1/assets/servers/freva/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/servers/freva/servers.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/servers/restservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.741595 freva_deployment-2305.0.1/assets/vault/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/vault/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/vault/deploy_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/vault/policy-file.hcl
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/vault/runserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/vault/vault-server-no-tls.hcl
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/vault/vault-server-tls.hcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.741595 freva_deployment-2305.0.1/assets/web/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2305 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/web/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/web/docker_cmd.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/web/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/web/freva_web.conf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:03:24.749595 freva_deployment-2305.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.737595 freva_deployment-2305.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.745595 freva_deployment-2305.0.1/src/freva_deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.745595 freva_deployment-2305.0.1/src/freva_deployment/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/cli/_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/cli/_migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/cli/_server_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/cli/_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.745595 freva_deployment-2305.0.1/src/freva_deployment/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.745595 freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34020 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.745595 freva_deployment-2305.0.1/src/freva_deployment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-05-08 15:03:24.000000 freva_deployment-2305.0.1/src/freva_deployment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-08 15:03:24.000000 freva_deployment-2305.0.1/src/freva_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:03:24.000000 freva_deployment-2305.0.1/src/freva_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-08 15:03:24.000000 freva_deployment-2305.0.1/src/freva_deployment.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-08 15:03:24.000000 freva_deployment-2305.0.1/src/freva_deployment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 15:03:24.000000 freva_deployment-2305.0.1/src/freva_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.988622 freva_deployment-2305.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-05-09 03:21:18.988622 freva_deployment-2305.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.980622 freva_deployment-2305.0.2/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.980622 freva_deployment-2305.0.2/assets/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/config/create_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/config/evaluation_system.conf.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/config/inventory.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.980622 freva_deployment-2305.0.2/assets/db_service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/db_service/password_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/db_service/reset_root_pw.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.980622 freva_deployment-2305.0.2/assets/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/playbooks/core-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/playbooks/db-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/playbooks/server-map-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/playbooks/solr-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/playbooks/vault-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/playbooks/web-server-playbook.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.980622 freva_deployment-2305.0.2/assets/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/scripts/create_cron.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/scripts/create_systemd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/scripts/docker-or-podman
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/scripts/dump_sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.980622 freva_deployment-2305.0.2/assets/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/servers/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.984622 freva_deployment-2305.0.2/assets/servers/freva/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/servers/freva/servers.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/servers/restservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.984622 freva_deployment-2305.0.2/assets/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/vault/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/vault/deploy_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/vault/policy-file.hcl
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/vault/runserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/vault/vault-server-no-tls.hcl
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/vault/vault-server-tls.hcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.984622 freva_deployment-2305.0.2/assets/web/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2305 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/web/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/web/docker_cmd.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/web/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/assets/web/freva_web.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 03:21:18.988622 freva_deployment-2305.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.980622 freva_deployment-2305.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.984622 freva_deployment-2305.0.2/src/freva_deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/src/freva_deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.984622 freva_deployment-2305.0.2/src/freva_deployment/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/src/freva_deployment/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/src/freva_deployment/cli/_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/src/freva_deployment/cli/_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/src/freva_deployment/cli/_server_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/src/freva_deployment/cli/_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/src/freva_deployment/deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.984622 freva_deployment-2305.0.2/src/freva_deployment/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/src/freva_deployment/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.988622 freva_deployment-2305.0.2/src/freva_deployment/ui/deployment_tui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/src/freva_deployment/ui/deployment_tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/src/freva_deployment/ui/deployment_tui/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33822 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/src/freva_deployment/ui/deployment_tui/deploy_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/src/freva_deployment/ui/deployment_tui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-05-09 03:21:08.000000 freva_deployment-2305.0.2/src/freva_deployment/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:21:18.984622 freva_deployment-2305.0.2/src/freva_deployment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-05-09 03:21:18.000000 freva_deployment-2305.0.2/src/freva_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-09 03:21:18.000000 freva_deployment-2305.0.2/src/freva_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:21:18.000000 freva_deployment-2305.0.2/src/freva_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 03:21:18.000000 freva_deployment-2305.0.2/src/freva_deployment.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-09 03:21:18.000000 freva_deployment-2305.0.2/src/freva_deployment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 03:21:18.000000 freva_deployment-2305.0.2/src/freva_deployment.egg-info/top_level.txt
```

### Comparing `freva_deployment-2305.0.1/PKG-INFO` & `freva_deployment-2305.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva_deployment
-Version: 2305.0.1
+Version: 2305.0.2
 Summary: Deploy freva and its services on different machines.
 Home-page: https://github.com/FREVA-CLINT/freva.git
 Author: Martin Bergemann
 Author-email: martin.bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: GPLv3
 Project-URL: Documentation, https://freva-deployment.readthedocs.io/en/latest/
```

### Comparing `freva_deployment-2305.0.1/README.md` & `freva_deployment-2305.0.2/README.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/config/create_tables.sql` & `freva_deployment-2305.0.2/assets/config/create_tables.sql`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/config/evaluation_system.conf.tmpl` & `freva_deployment-2305.0.2/assets/config/evaluation_system.conf.tmpl`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/config/inventory.toml` & `freva_deployment-2305.0.2/assets/config/inventory.toml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/db_service/password_rotate.py` & `freva_deployment-2305.0.2/assets/db_service/password_rotate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/playbooks/core-server-playbook.yml` & `freva_deployment-2305.0.2/assets/playbooks/core-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/playbooks/db-server-playbook.yml` & `freva_deployment-2305.0.2/assets/playbooks/db-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/playbooks/server-map-playbook.yml` & `freva_deployment-2305.0.2/assets/playbooks/server-map-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/playbooks/solr-server-playbook.yml` & `freva_deployment-2305.0.2/assets/playbooks/solr-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/playbooks/vault-server-playbook.yml` & `freva_deployment-2305.0.2/assets/playbooks/vault-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/playbooks/web-server-playbook.yml` & `freva_deployment-2305.0.2/assets/playbooks/web-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/scripts/create_systemd.py` & `freva_deployment-2305.0.2/assets/scripts/create_systemd.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/scripts/docker-or-podman` & `freva_deployment-2305.0.2/assets/scripts/docker-or-podman`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/servers/Dockerfile` & `freva_deployment-2305.0.2/assets/servers/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/servers/restservice.py` & `freva_deployment-2305.0.2/assets/servers/restservice.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/vault/Dockerfile` & `freva_deployment-2305.0.2/assets/vault/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/vault/deploy_vault.py` & `freva_deployment-2305.0.2/assets/vault/deploy_vault.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/vault/runserver.py` & `freva_deployment-2305.0.2/assets/vault/runserver.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/vault/vault-server-tls.hcl` & `freva_deployment-2305.0.2/assets/vault/vault-server-tls.hcl`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/web/Dockerfile` & `freva_deployment-2305.0.2/assets/web/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/assets/web/freva_web.conf` & `freva_deployment-2305.0.2/assets/web/freva_web.conf`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/setup.py` & `freva_deployment-2305.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/src/freva_deployment/cli/_deploy.py` & `freva_deployment-2305.0.2/src/freva_deployment/cli/_deploy.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/src/freva_deployment/cli/_migrate.py` & `freva_deployment-2305.0.2/src/freva_deployment/cli/_migrate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/src/freva_deployment/cli/_server_map.py` & `freva_deployment-2305.0.2/src/freva_deployment/cli/_server_map.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/src/freva_deployment/cli/_service.py` & `freva_deployment-2305.0.2/src/freva_deployment/cli/_service.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/src/freva_deployment/deploy.py` & `freva_deployment-2305.0.2/src/freva_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/__init__.py` & `freva_deployment-2305.0.2/src/freva_deployment/ui/deployment_tui/__init__.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/base.py` & `freva_deployment-2305.0.2/src/freva_deployment/ui/deployment_tui/base.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py` & `freva_deployment-2305.0.2/src/freva_deployment/ui/deployment_tui/deploy_forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,17 +189,15 @@
             core_playbook=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=(
                         f"{self.num}Set the path to the playbook used for"
                         " setting up the system."
                     ),
-                    value=cfg.get(
-                        "core_playbook",
-                    ),
+                    value=cfg.get("core_playbook", ""),
                 ),
                 False,
             ),
             ansible_python_interpreter=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=f"{self.num}Python path on remote machine:",
@@ -238,15 +236,15 @@
         for nn, choice in enumerate(choices):
             if choice == key:
                 return nn
         return 0
 
     def _add_widgets(self) -> None:
         """Add widgets to the screen."""
-        self.list_keys = "imprint", "scheduler_host"
+        self.list_keys = "imprint", "scheduler_host", "allowed_hosts"
         cfg = self.get_config(self.step)
         for key in self.list_keys:
             if key in cfg and isinstance(cfg[key], str):
                 value = cast(str, cfg[key])
                 cfg[key] = [v.strip() for v in value.split(",") if v.strip()]
                 logger.warning(key, cfg[key])
         self.input_fields: dict[str, tuple[npyscreen.TitleText, bool]] = dict(
@@ -548,17 +546,15 @@
             web_playbook=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=(
                         f"{self.num}Set the path to the playbook used for"
                         " setting up the system."
                     ),
-                    value=cfg.get(
-                        "web_playbook",
-                    ),
+                    value=cfg.get("web_playbook", ""),
                 ),
                 False,
             ),
             ansible_python_interpreter=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=f"{self.num}Pythonpath on remote machine:",
@@ -640,30 +636,26 @@
             db_playbook=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=(
                         f"{self.num}Set the path to the db playbook used for"
                         " setting up the system."
                     ),
-                    value=cfg.get(
-                        "db_playbook",
-                    ),
+                    value=cfg.get("db_playbook", ""),
                 ),
                 False,
             ),
             vault_playbook=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=(
                         f"{self.num}Set the path to the vault playbook used for"
                         " setting up the system."
                     ),
-                    value=cfg.get(
-                        "vault_playbook",
-                    ),
+                    value=cfg.get("vault_playbook", ""),
                 ),
                 False,
             ),
             ansible_python_interpreter=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=f"{self.num}Pythonpath on remote machine:",
@@ -736,17 +728,15 @@
             solr_playbook=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=(
                         f"{self.num}Set the path to the playbook used for"
                         " setting up the system."
                     ),
-                    value=cfg.get(
-                        "solr_playbook",
-                    ),
+                    value=cfg.get("solr_playbook", ""),
                 ),
                 False,
             ),
             ansible_python_interpreter=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=f"{self.num}Pythonpath on remote machine:",
```

### Comparing `freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/main_window.py` & `freva_deployment-2305.0.2/src/freva_deployment/ui/deployment_tui/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         npyscreen.setTheme(npyscreen.Themes.ElegantTheme)
         self.cache_dir.mkdir(exist_ok=True, parents=True)
         self.setup: dict[str, Any] = {}
         self._forms: dict[str, BaseForm] = {}
         self.current_form = "core"
         self.init()
         self.thread_stop = threading.Event()
-        # self.start_auto_save()
+        self.start_auto_save()
 
     def init(self) -> None:
         self._steps_lookup = {
             "core": "MAIN",
             "web": "SECOND",
             "solr": "FOURTH",
             "db": "THIRD",
@@ -96,15 +96,19 @@
 
     def check_missing_config(self, stop_at_missing: bool = True) -> str | None:
         """Evaluate all forms."""
         for step, form_obj in self._forms.items():
             cfg = form_obj.check_config(notify=stop_at_missing)
             if cfg is None and stop_at_missing:
                 return self._steps_lookup[step]
-            self.config[step] = cfg
+            try:
+                self.config[step] = cfg
+            except Exception as error:
+                raise ValueError((step, cfg))
+                raise error
         return None
 
     def _auto_save(self) -> None:
         """Auto save the current configuration."""
         while not self.thread_stop.is_set():
             time.sleep(0.5)
             if self.thread_stop.is_set():
@@ -213,18 +217,14 @@
         config_tmpl["project_name"] = project_name
         for step, settings in self.config.items():
             if step in ("certificates", "project_name"):
                 continue
             config_tmpl[step]["hosts"] = settings["hosts"]
             for key, config in settings["config"].items():
                 config_tmpl[step]["config"][key] = config
-                if key == "allowed_hosts" and step == "web":
-                    config_tmpl[step]["config"][key] = list(
-                        set(cast(str, config).split(","))
-                    )
         Path(self.save_file).parent.mkdir(exist_ok=True, parents=True)
         with open(self.save_file, "w") as f:
             toml_string = tomlkit.dumps(config_tmpl)
             f.write(toml_string)
         return Path(self.save_file)
 
     @property
```

### Comparing `freva_deployment-2305.0.1/src/freva_deployment/utils.py` & `freva_deployment-2305.0.2/src/freva_deployment/utils.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.1/src/freva_deployment.egg-info/PKG-INFO` & `freva_deployment-2305.0.2/src/freva_deployment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva-deployment
-Version: 2305.0.1
+Version: 2305.0.2
 Summary: Deploy freva and its services on different machines.
 Home-page: https://github.com/FREVA-CLINT/freva.git
 Author: Martin Bergemann
 Author-email: martin.bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: GPLv3
 Project-URL: Documentation, https://freva-deployment.readthedocs.io/en/latest/
```

### Comparing `freva_deployment-2305.0.1/src/freva_deployment.egg-info/SOURCES.txt` & `freva_deployment-2305.0.2/src/freva_deployment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

