# Comparing `tmp/hive_builder-3.6.5.tar.gz` & `tmp/hive_builder-3.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive_builder-3.6.5.tar", last modified: Fri Mar 31 07:52:58 2023, max compression
+gzip compressed data, was "hive_builder-3.6.6.tar", max compression
```

## Comparing `hive_builder-3.6.5.tar` & `hive_builder-3.6.6.tar`

### file list

```diff
@@ -1,432 +1,157 @@
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.962674 hive_builder-3.6.5/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.707605 hive_builder-3.6.5/.github/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.758170 hive_builder-3.6.5/.github/workflows/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2448 2021-06-05 05:07:08.000000 hive_builder-3.6.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)      285 2021-09-12 02:08:43.000000 hive_builder-3.6.5/.gitignore
--rw-r--r--   0 mitsuru    (501) staff       (20)     1660 2021-09-13 01:20:17.000000 hive_builder-3.6.5/.readthedocs.yaml
--rw-r--r--   0 mitsuru    (501) staff       (20)     7321 2021-03-08 14:16:19.000000 hive_builder-3.6.5/GITHUB-FLOW-ja.md
--rw-r--r--   0 mitsuru    (501) staff       (20)     5690 2021-03-08 14:16:19.000000 hive_builder-3.6.5/GITHUB-FLOW.md
--rw-r--r--   0 mitsuru    (501) staff       (20)     1074 2018-12-02 00:59:41.000000 hive_builder-3.6.5/LICENSE
--rw-r--r--   0 mitsuru    (501) staff       (20)       76 2019-09-28 00:44:14.000000 hive_builder-3.6.5/MANIFEST.in
--rw-r--r--   0 mitsuru    (501) staff       (20)     1678 2023-03-31 07:52:58.962909 hive_builder-3.6.5/PKG-INFO
--rw-r--r--   0 mitsuru    (501) staff       (20)      915 2022-01-03 07:50:13.000000 hive_builder-3.6.5/Pipfile
--rw-r--r--   0 mitsuru    (501) staff       (20)    75837 2023-03-31 07:51:53.000000 hive_builder-3.6.5/Pipfile.lock
--rw-r--r--   0 mitsuru    (501) staff       (20)     1231 2019-09-23 03:24:38.000000 hive_builder-3.6.5/README.md
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.791531 hive_builder-3.6.5/docs/
--rw-r--r--   0 mitsuru    (501) staff       (20)      634 2019-09-17 06:15:16.000000 hive_builder-3.6.5/docs/Makefile
--rw-r--r--   0 mitsuru    (501) staff       (20)     4117 2021-09-10 07:23:54.000000 hive_builder-3.6.5/docs/aws.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)     2799 2021-09-20 02:12:52.000000 hive_builder-3.6.5/docs/backup.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)     1241 2021-10-28 06:56:07.000000 hive_builder-3.6.5/docs/bashcompletion.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)     8883 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/cashare.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)     5568 2020-07-07 08:20:14.000000 hive_builder-3.6.5/docs/command.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)     2469 2021-09-12 03:36:36.000000 hive_builder-3.6.5/docs/conf.py
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.708121 hive_builder-3.6.5/docs/customize/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.792522 hive_builder-3.6.5/docs/customize/css/
--rw-r--r--   0 mitsuru    (501) staff       (20)      250 2021-09-12 03:36:36.000000 hive_builder-3.6.5/docs/customize/css/my_theme.css
--rw-r--r--   0 mitsuru    (501) staff       (20)    22895 2022-02-01 13:42:36.000000 hive_builder-3.6.5/docs/develop.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)    17632 2022-05-23 09:55:27.000000 hive_builder-3.6.5/docs/example.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)    26918 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/faq.rst
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.825266 hive_builder-3.6.5/docs/imgs/
--rw-r--r--   0 mitsuru    (501) staff       (20)   104207 2019-11-30 02:08:27.000000 hive_builder-3.6.5/docs/imgs/docker_network.png
--rw-r--r--   0 mitsuru    (501) staff       (20)   131504 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/imgs/docker_network_detail.png
--rw-r--r--   0 mitsuru    (501) staff       (20)   191729 2019-09-19 00:11:35.000000 hive_builder-3.6.5/docs/imgs/ha.png
--rw-r--r--   0 mitsuru    (501) staff       (20)   144782 2022-01-22 23:49:08.000000 hive_builder-3.6.5/docs/imgs/ha_nfs.png
--rw-r--r--   0 mitsuru    (501) staff       (20)    52804 2019-09-18 23:30:49.000000 hive_builder-3.6.5/docs/imgs/infra.png
--rw-r--r--   0 mitsuru    (501) staff       (20)    88077 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/imgs/lb_stateless_mesh.png
--rw-r--r--   0 mitsuru    (501) staff       (20)    86609 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/imgs/lb_stateless_sidecar.png
--rw-r--r--   0 mitsuru    (501) staff       (20)    93906 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/imgs/load_balancer.png
--rw-r--r--   0 mitsuru    (501) staff       (20)   134886 2021-03-08 14:16:19.000000 hive_builder-3.6.5/docs/imgs/phase.png
--rw-r--r--   0 mitsuru    (501) staff       (20)    71085 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/imgs/set_client_cert.png
--rw-r--r--   0 mitsuru    (501) staff       (20)    59071 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/imgs/set_server_cert.png
--rw-r--r--   0 mitsuru    (501) staff       (20)    46990 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/imgs/share_ca.png
--rw-r--r--   0 mitsuru    (501) staff       (20)    66336 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/imgs/stateless_mesh.png
--rw-r--r--   0 mitsuru    (501) staff       (20)    45258 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/imgs/stateless_sidecar.png
--rw-r--r--   0 mitsuru    (501) staff       (20)    94060 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/imgs/sticky_load_balancer.png
--rw-r--r--   0 mitsuru    (501) staff       (20)    38884 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/imgs/virtualip.png
--rw-r--r--   0 mitsuru    (501) staff       (20)      610 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/index.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)     9680 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/install.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)    55457 2023-03-31 07:51:53.000000 hive_builder-3.6.5/docs/inventory.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)      795 2019-09-17 06:15:16.000000 hive_builder-3.6.5/docs/make.bat
--rw-r--r--   0 mitsuru    (501) staff       (20)     2643 2021-07-10 04:10:37.000000 hive_builder-3.6.5/docs/migration.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)    12301 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/nfs.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)     6520 2021-06-15 04:31:03.000000 hive_builder-3.6.5/docs/overview.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)    20264 2021-11-17 03:59:53.000000 hive_builder-3.6.5/docs/phases.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)     5633 2021-09-20 02:12:52.000000 hive_builder-3.6.5/docs/proxy.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)    15472 2021-11-27 00:29:51.000000 hive_builder-3.6.5/docs/repair.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)       47 2021-09-13 00:19:43.000000 hive_builder-3.6.5/docs/requirements.txt
--rw-r--r--   0 mitsuru    (501) staff       (20)    29081 2022-11-14 23:07:24.000000 hive_builder-3.6.5/docs/servicepatterns.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)      123 2021-09-13 00:29:51.000000 hive_builder-3.6.5/docs/setuptools.txt
--rw-r--r--   0 mitsuru    (501) staff       (20)     5415 2020-02-07 11:33:26.000000 hive_builder-3.6.5/docs/swarmextender.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)     8388 2021-11-27 00:48:55.000000 hive_builder-3.6.5/docs/tagmapping.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)     8071 2022-05-23 09:55:27.000000 hive_builder-3.6.5/docs/vagrant.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)     4209 2022-12-22 00:09:07.000000 hive_builder-3.6.5/docs/zabbix.rst
--rw-r--r--   0 mitsuru    (501) staff       (20)       47 2019-09-28 00:16:15.000000 hive_builder-3.6.5/entry_points.cfg
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.708599 hive_builder-3.6.5/examples/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.709218 hive_builder-3.6.5/examples/pdns/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.827448 hive_builder-3.6.5/examples/pdns/inventory/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.829353 hive_builder-3.6.5/examples/pdns/inventory/group_vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)      265 2021-12-31 08:08:08.000000 hive_builder-3.6.5/examples/pdns/inventory/group_vars/servers.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)      120 2019-08-14 09:23:55.000000 hive_builder-3.6.5/examples/pdns/inventory/group_vars/services.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     1384 2023-03-31 07:51:53.000000 hive_builder-3.6.5/examples/pdns/inventory/hive.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     4108 2022-11-14 23:07:24.000000 hive_builder-3.6.5/examples/pdns/inventory/powerdns.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.830908 hive_builder-3.6.5/examples/pdns/lib/
--rw-r--r--   0 mitsuru    (501) staff       (20)     9847 2022-05-23 09:55:27.000000 hive_builder-3.6.5/examples/pdns/lib/powerdns_record.py
--rw-r--r--   0 mitsuru    (501) staff       (20)     8646 2022-05-23 09:55:27.000000 hive_builder-3.6.5/examples/pdns/lib/powerdns_zone.py
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.712522 hive_builder-3.6.5/examples/pdns/roles/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.709805 hive_builder-3.6.5/examples/pdns/roles/addon/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.832698 hive_builder-3.6.5/examples/pdns/roles/addon/files/
--rw-r--r--   0 mitsuru    (501) staff       (20)      517 2022-01-22 23:49:08.000000 hive_builder-3.6.5/examples/pdns/roles/addon/files/ddclient.service
--rw-r--r--   0 mitsuru    (501) staff       (20)       54 2022-01-22 23:49:08.000000 hive_builder-3.6.5/examples/pdns/roles/addon/files/sysconfig-ddclient
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.834624 hive_builder-3.6.5/examples/pdns/roles/addon/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2686 2022-04-17 00:22:42.000000 hive_builder-3.6.5/examples/pdns/roles/addon/tasks/ddclient.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)      171 2022-01-22 23:49:08.000000 hive_builder-3.6.5/examples/pdns/roles/addon/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.835440 hive_builder-3.6.5/examples/pdns/roles/addon/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)      959 2021-09-10 07:29:15.000000 hive_builder-3.6.5/examples/pdns/roles/addon/templates/ddclient.conf.j2
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.710375 hive_builder-3.6.5/examples/pdns/roles/certbot-runner/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.836272 hive_builder-3.6.5/examples/pdns/roles/certbot-runner/files/
--rw-r--r--   0 mitsuru    (501) staff       (20)     7115 2019-09-17 11:27:31.000000 hive_builder-3.6.5/examples/pdns/roles/certbot-runner/files/certbot-runner
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.837033 hive_builder-3.6.5/examples/pdns/roles/certbot-runner/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      224 2019-09-03 11:40:35.000000 hive_builder-3.6.5/examples/pdns/roles/certbot-runner/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.711022 hive_builder-3.6.5/examples/pdns/roles/powerdns-admin/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.837909 hive_builder-3.6.5/examples/pdns/roles/powerdns-admin/files/
--rw-r--r--   0 mitsuru    (501) staff       (20)      709 2020-10-18 01:44:39.000000 hive_builder-3.6.5/examples/pdns/roles/powerdns-admin/files/create_admin.py
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.838294 hive_builder-3.6.5/examples/pdns/roles/powerdns-admin/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      439 2020-01-01 03:34:44.000000 hive_builder-3.6.5/examples/pdns/roles/powerdns-admin/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.711668 hive_builder-3.6.5/examples/pdns/roles/powerdns-init/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.838865 hive_builder-3.6.5/examples/pdns/roles/powerdns-init/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1890 2020-07-07 06:26:05.000000 hive_builder-3.6.5/examples/pdns/roles/powerdns-init/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.839733 hive_builder-3.6.5/examples/pdns/roles/powerdns-init/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)       20 2019-11-30 05:05:45.000000 hive_builder-3.6.5/examples/pdns/roles/powerdns-init/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.712324 hive_builder-3.6.5/examples/pdns/roles/powerdns-initdb/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.840274 hive_builder-3.6.5/examples/pdns/roles/powerdns-initdb/files/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2988 2021-09-10 07:23:54.000000 hive_builder-3.6.5/examples/pdns/roles/powerdns-initdb/files/powerdns-init.sql
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.841171 hive_builder-3.6.5/examples/pdns/roles/powerdns-initdb/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)       98 2019-08-14 08:28:17.000000 hive_builder-3.6.5/examples/pdns/roles/powerdns-initdb/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.712824 hive_builder-3.6.5/examples/pdns/roles/proxy-configure/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.841758 hive_builder-3.6.5/examples/pdns/roles/proxy-configure/files/
--rw-r--r--   0 mitsuru    (501) staff       (20)     4332 2021-09-10 07:23:54.000000 hive_builder-3.6.5/examples/pdns/roles/proxy-configure/files/proxy-configure
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.842594 hive_builder-3.6.5/examples/pdns/roles/proxy-configure/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      199 2021-08-05 15:34:38.000000 hive_builder-3.6.5/examples/pdns/roles/proxy-configure/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.846578 hive_builder-3.6.5/hive_builder/
--rw-r--r--   0 mitsuru    (501) staff       (20)     6148 2021-02-13 23:46:39.000000 hive_builder-3.6.5/hive_builder/.DS_Store
--rwxr-xr-x   0 mitsuru    (501) staff       (20)      312 2021-04-10 02:43:58.000000 hive_builder-3.6.5/hive_builder/__init__.py
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.853385 hive_builder-3.6.5/hive_builder/__pycache__/
--rw-r--r--   0 mitsuru    (501) staff       (20)      290 2021-09-12 05:24:15.000000 hive_builder-3.6.5/hive_builder/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 mitsuru    (501) staff       (20)      311 2022-04-05 08:21:42.000000 hive_builder-3.6.5/hive_builder/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mitsuru    (501) staff       (20)    25268 2021-09-12 05:24:15.000000 hive_builder-3.6.5/hive_builder/__pycache__/hive.cpython-37.pyc
--rw-r--r--   0 mitsuru    (501) staff       (20)    29342 2023-01-15 03:21:43.000000 hive_builder-3.6.5/hive_builder/__pycache__/hive.cpython-39.pyc
--rw-r--r--   0 mitsuru    (501) staff       (20)     1031 2021-10-28 06:31:20.000000 hive_builder-3.6.5/hive_builder/hive-completion.sh
--rw-r--r--   0 mitsuru    (501) staff       (20)    26961 2023-03-31 07:51:53.000000 hive_builder-3.6.5/hive_builder/hive.py
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.855065 hive_builder-3.6.5/hive_builder/lib/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.855426 hive_builder-3.6.5/hive_builder/lib/__pycache__/
--rw-r--r--   0 mitsuru    (501) staff       (20)    11331 2019-06-17 14:31:29.000000 hive_builder-3.6.5/hive_builder/lib/__pycache__/vagrant.cpython-37.pyc
--rw-r--r--   0 mitsuru    (501) staff       (20)    14020 2022-01-22 23:49:08.000000 hive_builder-3.6.5/hive_builder/lib/azure_rm_storageshare.py
--rw-r--r--   0 mitsuru    (501) staff       (20)    14954 2020-11-07 23:35:21.000000 hive_builder-3.6.5/hive_builder/lib/hive_vagrant.py
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.865124 hive_builder-3.6.5/hive_builder/playbooks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     6148 2021-02-13 23:46:39.000000 hive_builder-3.6.5/hive_builder/playbooks/.DS_Store
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.865899 hive_builder-3.6.5/hive_builder/playbooks/.hive/
--rw-r--r--   0 mitsuru    (501) staff       (20)      224 2021-07-11 01:09:14.000000 hive_builder-3.6.5/hive_builder/playbooks/.hive/persistents.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     5832 2022-02-07 00:32:52.000000 hive_builder-3.6.5/hive_builder/playbooks/build-images.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     1943 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/build-infra.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     1084 2022-03-19 23:56:40.000000 hive_builder-3.6.5/hive_builder/playbooks/build-networks.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     2447 2022-01-22 23:49:08.000000 hive_builder-3.6.5/hive_builder/playbooks/build-volumes.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.719397 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.715144 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/addon/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.866736 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/addon/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)       81 2019-06-20 00:29:56.000000 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/addon/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.715916 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-certificate/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.867720 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-certificate/files/
--rw-r--r--   0 mitsuru    (501) staff       (20)       40 2022-12-22 00:09:07.000000 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-certificate/files/extfile.cnf
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.868500 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-certificate/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1783 2022-12-22 00:09:07.000000 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-certificate/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.716542 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-syslog/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.869136 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-syslog/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      356 2022-12-24 07:24:36.000000 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-syslog/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.869958 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-syslog/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)      946 2020-11-07 23:35:21.000000 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-syslog/templates/transfer.conf.j2
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.719128 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.874475 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      650 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.717193 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.870731 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      351 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.871950 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)       49 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.717834 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.872582 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      323 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.873038 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)       49 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.718671 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.873538 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      409 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.874035 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)       49 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.719543 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/python-aptk/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.874945 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/python-aptk/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      274 2022-12-02 00:39:10.000000 hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/python-aptk/tasks/main.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     9564 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/deploy-services.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.876466 hive_builder-3.6.5/hive_builder/playbooks/group_vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2558 2022-04-17 00:22:42.000000 hive_builder-3.6.5/hive_builder/playbooks/group_vars/hosts.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)      129 2019-09-19 11:22:44.000000 hive_builder-3.6.5/hive_builder/playbooks/group_vars/mother.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     1015 2019-11-30 03:55:24.000000 hive_builder-3.6.5/hive_builder/playbooks/initialize-services.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     2430 2021-09-10 07:23:54.000000 hive_builder-3.6.5/hive_builder/playbooks/iptables.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     2479 2020-02-07 11:33:26.000000 hive_builder-3.6.5/hive_builder/playbooks/push-image.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.877287 hive_builder-3.6.5/hive_builder/playbooks/roles/
--rw-r--r--   0 mitsuru    (501) staff       (20)     6148 2021-02-13 23:46:33.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/.DS_Store
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.721290 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.881292 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     3107 2022-04-08 12:47:58.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/tasks/build-aws.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     3627 2022-12-02 00:39:10.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/tasks/create_instance.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     2665 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/tasks/destroy-aws.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)      327 2019-09-17 09:18:22.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/tasks/main.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)      217 2019-10-06 03:33:21.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/tasks/stop-aws.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.883917 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)       46 2019-09-07 02:56:08.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/templates/aws_cli_config.j2
--rw-r--r--   0 mitsuru    (501) staff       (20)      102 2019-09-07 02:56:08.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/templates/aws_cli_credentials.j2
--rw-r--r--   0 mitsuru    (501) staff       (20)      138 2019-09-07 02:56:08.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/templates/azure_cli_credentials.j2
--rw-r--r--   0 mitsuru    (501) staff       (20)      138 2019-09-07 02:56:08.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/templates/cloudstack.ini.j2
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.884329 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1497 2022-11-22 12:21:39.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/aws/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.721919 hive_builder-3.6.5/hive_builder/playbooks/roles/azure/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.887100 hive_builder-3.6.5/hive_builder/playbooks/roles/azure/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     3273 2022-01-22 23:49:08.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/azure/tasks/build-azure.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     3434 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/azure/tasks/create_instance.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     1932 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/azure/tasks/destroy-azure.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)      326 2020-01-01 03:34:44.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/azure/tasks/main.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)      297 2021-09-10 07:23:54.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/azure/tasks/stop-azure.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.887824 hive_builder-3.6.5/hive_builder/playbooks/roles/azure/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)      647 2022-04-17 00:22:42.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/azure/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.722521 hive_builder-3.6.5/hive_builder/playbooks/roles/backup-tools/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.888677 hive_builder-3.6.5/hive_builder/playbooks/roles/backup-tools/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      589 2020-11-07 23:35:21.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/backup-tools/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.890293 hive_builder-3.6.5/hive_builder/playbooks/roles/backup-tools/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)      179 2019-09-15 22:05:15.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/backup-tools/templates/backup.service
--rw-r--r--   0 mitsuru    (501) staff       (20)      126 2019-09-11 10:06:21.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/backup-tools/templates/backup.timer
--rw-r--r--   0 mitsuru    (501) staff       (20)     5210 2022-02-01 13:42:36.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/backup-tools/templates/hive-backup.sh
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.723553 hive_builder-3.6.5/hive_builder/playbooks/roles/base/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.723258 hive_builder-3.6.5/hive_builder/playbooks/roles/base/files/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.891055 hive_builder-3.6.5/hive_builder/playbooks/roles/base/files/NetworkManager-wait-online.service.d/
--rw-r--r--   0 mitsuru    (501) staff       (20)       85 2019-09-07 23:05:40.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/base/files/NetworkManager-wait-online.service.d/override.conf
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.892814 hive_builder-3.6.5/hive_builder/playbooks/roles/base/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1210 2021-03-08 14:16:19.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/base/tasks/fixed-yum-url.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     1796 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/base/tasks/growfs.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     6801 2022-12-02 00:39:10.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/base/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.724724 hive_builder-3.6.5/hive_builder/playbooks/roles/ca/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.893542 hive_builder-3.6.5/hive_builder/playbooks/roles/ca/files/
--rw-r--r--   0 mitsuru    (501) staff       (20)       77 2018-12-02 00:59:41.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/ca/files/extfile.cnf
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.894029 hive_builder-3.6.5/hive_builder/playbooks/roles/ca/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1290 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/ca/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.894696 hive_builder-3.6.5/hive_builder/playbooks/roles/ca/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)      268 2019-06-25 01:35:53.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/ca/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.727997 hive_builder-3.6.5/hive_builder/playbooks/roles/docker/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.900435 hive_builder-3.6.5/hive_builder/playbooks/roles/docker/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     4726 2022-05-23 09:55:27.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/docker/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.901584 hive_builder-3.6.5/hive_builder/playbooks/roles/docker/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)      321 2021-09-10 07:23:54.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/docker/templates/daemon.json.j2
--rw-r--r--   0 mitsuru    (501) staff       (20)      331 2022-03-19 23:56:40.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/docker/templates/override.conf
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.726833 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.896774 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2048 2021-09-10 07:23:54.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.898704 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1770 2019-11-11 07:53:20.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client/templates/dcp
--rw-r--r--   0 mitsuru    (501) staff       (20)     1467 2021-04-19 23:53:15.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client/templates/dexec
--rw-r--r--   0 mitsuru    (501) staff       (20)      678 2019-08-14 01:32:02.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client/templates/dsh
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.899302 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)      170 2019-06-22 01:37:06.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.725679 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client-proxy/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.895168 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client-proxy/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1032 2020-11-07 23:35:21.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client-proxy/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.895952 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client-proxy/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)      233 2019-10-29 06:16:18.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client-proxy/templates/config.json.j2
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.727306 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-compose/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.899708 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-compose/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      147 2019-06-27 15:16:06.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/docker-compose/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.730345 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.905204 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd/files/
--rw-r--r--   0 mitsuru    (501) staff       (20)      229 2020-05-02 06:38:14.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd/files/drbd-resource@.service
--rw-r--r--   0 mitsuru    (501) staff       (20)      309 2019-12-05 10:14:59.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd/files/waitdevice
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.906533 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2933 2023-03-31 07:51:53.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd/tasks/main.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     3381 2022-12-22 00:09:07.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd/tasks/vg.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.907290 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)      442 2022-01-22 23:49:08.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.729159 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd-resource/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.902283 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd-resource/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     5426 2021-11-27 00:29:51.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd-resource/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.902984 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd-resource/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1568 2022-01-22 23:49:08.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd-resource/templates/volume.res
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.903679 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd-resource/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)      421 2021-09-10 07:23:54.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/drbd-resource/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.731530 hive_builder-3.6.5/hive_builder/playbooks/roles/follow-swarm-service/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.907881 hive_builder-3.6.5/hive_builder/playbooks/roles/follow-swarm-service/files/
--rw-r--r--   0 mitsuru    (501) staff       (20)    27684 2022-02-01 13:46:42.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/follow-swarm-service/files/follow-swarm-service.py
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.908213 hive_builder-3.6.5/hive_builder/playbooks/roles/follow-swarm-service/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1411 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/follow-swarm-service/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.909061 hive_builder-3.6.5/hive_builder/playbooks/roles/follow-swarm-service/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)      309 2020-12-08 12:48:01.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/follow-swarm-service/templates/follow-swarm-service.service
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.732335 hive_builder-3.6.5/hive_builder/playbooks/roles/gcp/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.913696 hive_builder-3.6.5/hive_builder/playbooks/roles/gcp/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2850 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/gcp/tasks/build-gcp.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     3021 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/gcp/tasks/create_instance.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     3289 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/gcp/tasks/destroy-gcp.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)      314 2019-09-17 09:16:48.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/gcp/tasks/main.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)      396 2022-04-11 10:56:55.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/gcp/tasks/stop-gcp.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.914793 hive_builder-3.6.5/hive_builder/playbooks/roles/gcp/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)      741 2022-04-17 00:22:42.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/gcp/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.732861 hive_builder-3.6.5/hive_builder/playbooks/roles/hostsfile/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.915634 hive_builder-3.6.5/hive_builder/playbooks/roles/hostsfile/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      338 2019-09-15 14:29:48.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/hostsfile/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.733481 hive_builder-3.6.5/hive_builder/playbooks/roles/internal-network/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.916275 hive_builder-3.6.5/hive_builder/playbooks/roles/internal-network/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1403 2019-10-23 23:08:13.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/internal-network/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.733957 hive_builder-3.6.5/hive_builder/playbooks/roles/iptables/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.917107 hive_builder-3.6.5/hive_builder/playbooks/roles/iptables/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      625 2021-09-10 07:23:54.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/iptables/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.735255 hive_builder-3.6.5/hive_builder/playbooks/roles/kickstart/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.918013 hive_builder-3.6.5/hive_builder/playbooks/roles/kickstart/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     4319 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/kickstart/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.918506 hive_builder-3.6.5/hive_builder/playbooks/roles/kickstart/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)     3345 2022-12-22 00:09:07.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/kickstart/templates/kickstart.j2
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.919159 hive_builder-3.6.5/hive_builder/playbooks/roles/kickstart/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)      171 2021-06-15 04:31:03.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/kickstart/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.736250 hive_builder-3.6.5/hive_builder/playbooks/roles/monitor-service-log/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.919959 hive_builder-3.6.5/hive_builder/playbooks/roles/monitor-service-log/handlers/
--rw-r--r--   0 mitsuru    (501) staff       (20)      118 2021-03-08 14:16:19.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/monitor-service-log/handlers/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.920676 hive_builder-3.6.5/hive_builder/playbooks/roles/monitor-service-log/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      875 2021-03-08 14:16:19.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/monitor-service-log/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.921324 hive_builder-3.6.5/hive_builder/playbooks/roles/monitor-service-log/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1017 2021-03-08 14:16:19.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/monitor-service-log/templates/monitor-service-log.j2
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.736555 hive_builder-3.6.5/hive_builder/playbooks/roles/nfs-aws-volumes/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.921774 hive_builder-3.6.5/hive_builder/playbooks/roles/nfs-aws-volumes/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2436 2022-01-23 06:08:12.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/nfs-aws-volumes/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.736912 hive_builder-3.6.5/hive_builder/playbooks/roles/nfs-azure-volumes/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.922516 hive_builder-3.6.5/hive_builder/playbooks/roles/nfs-azure-volumes/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2001 2022-01-22 23:49:08.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/nfs-azure-volumes/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.737451 hive_builder-3.6.5/hive_builder/playbooks/roles/nfs-gcp-volumes/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.923157 hive_builder-3.6.5/hive_builder/playbooks/roles/nfs-gcp-volumes/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2528 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/nfs-gcp-volumes/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.737789 hive_builder-3.6.5/hive_builder/playbooks/roles/ntp-client/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.923586 hive_builder-3.6.5/hive_builder/playbooks/roles/ntp-client/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      531 2020-11-07 23:35:21.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/ntp-client/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.738165 hive_builder-3.6.5/hive_builder/playbooks/roles/pip-venv/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.924306 hive_builder-3.6.5/hive_builder/playbooks/roles/pip-venv/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2650 2022-04-17 00:22:42.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/pip-venv/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.738851 hive_builder-3.6.5/hive_builder/playbooks/roles/prepared/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.925459 hive_builder-3.6.5/hive_builder/playbooks/roles/prepared/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      403 2019-11-24 00:58:57.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/prepared/tasks/main.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)      665 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/prepared/tasks/setup.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.925847 hive_builder-3.6.5/hive_builder/playbooks/roles/prepared/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)       79 2019-10-05 23:41:55.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/prepared/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.739340 hive_builder-3.6.5/hive_builder/playbooks/roles/reboot/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.926414 hive_builder-3.6.5/hive_builder/playbooks/roles/reboot/handlers/
--rw-r--r--   0 mitsuru    (501) staff       (20)      394 2019-12-01 01:00:04.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/reboot/handlers/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.740247 hive_builder-3.6.5/hive_builder/playbooks/roles/registry/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.926926 hive_builder-3.6.5/hive_builder/playbooks/roles/registry/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1712 2020-11-07 23:35:21.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/registry/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.928031 hive_builder-3.6.5/hive_builder/playbooks/roles/registry/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)       57 2018-12-02 00:59:41.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/registry/templates/daemon.json.j2
--rw-r--r--   0 mitsuru    (501) staff       (20)      985 2022-03-19 23:56:40.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/registry/templates/registry.yml.j2
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.928615 hive_builder-3.6.5/hive_builder/playbooks/roles/rsyslogd/
--rw-r--r--   0 mitsuru    (501) staff       (20)     6148 2020-05-17 00:35:27.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/rsyslogd/.DS_Store
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.929161 hive_builder-3.6.5/hive_builder/playbooks/roles/rsyslogd/handlers/
--rw-r--r--   0 mitsuru    (501) staff       (20)      118 2020-05-18 23:52:33.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/rsyslogd/handlers/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.929687 hive_builder-3.6.5/hive_builder/playbooks/roles/rsyslogd/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1338 2022-03-19 23:56:40.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/rsyslogd/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.930178 hive_builder-3.6.5/hive_builder/playbooks/roles/rsyslogd/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)     3162 2021-09-10 07:23:54.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/rsyslogd/templates/services.conf
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.742285 hive_builder-3.6.5/hive_builder/playbooks/roles/service-backup/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.930682 hive_builder-3.6.5/hive_builder/playbooks/roles/service-backup/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      788 2020-11-07 23:35:21.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/service-backup/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.931203 hive_builder-3.6.5/hive_builder/playbooks/roles/service-backup/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)     5337 2022-12-24 02:03:50.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/service-backup/templates/service-backup.sh.j2
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.742754 hive_builder-3.6.5/hive_builder/playbooks/roles/strict-source-ip/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.931724 hive_builder-3.6.5/hive_builder/playbooks/roles/strict-source-ip/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1148 2020-11-07 23:35:21.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/strict-source-ip/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.743190 hive_builder-3.6.5/hive_builder/playbooks/roles/swarm/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.932429 hive_builder-3.6.5/hive_builder/playbooks/roles/swarm/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     6226 2022-03-19 23:56:40.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/swarm/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.743995 hive_builder-3.6.5/hive_builder/playbooks/roles/tls-certificate/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.933149 hive_builder-3.6.5/hive_builder/playbooks/roles/tls-certificate/handlers/
--rw-r--r--   0 mitsuru    (501) staff       (20)      220 2019-06-22 01:20:53.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/tls-certificate/handlers/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.933907 hive_builder-3.6.5/hive_builder/playbooks/roles/tls-certificate/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2912 2021-03-07 03:07:41.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/tls-certificate/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.934612 hive_builder-3.6.5/hive_builder/playbooks/roles/tls-certificate/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)      188 2019-06-22 01:34:16.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/tls-certificate/templates/extfile.cnf
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.935271 hive_builder-3.6.5/hive_builder/playbooks/roles/tls-certificate/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)      508 2019-06-23 06:17:20.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/tls-certificate/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.744471 hive_builder-3.6.5/hive_builder/playbooks/roles/users/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.936493 hive_builder-3.6.5/hive_builder/playbooks/roles/users/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)      433 2019-09-09 06:17:01.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/users/tasks/known-hosts.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     1157 2019-09-09 06:16:45.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/users/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.936963 hive_builder-3.6.5/hive_builder/playbooks/roles/users/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)       40 2018-12-02 00:59:41.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/users/templates/sudoer.j2
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.745325 hive_builder-3.6.5/hive_builder/playbooks/roles/vagrant/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.937846 hive_builder-3.6.5/hive_builder/playbooks/roles/vagrant/files/
--rw-r--r--   0 mitsuru    (501) staff       (20)     3160 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/vagrant/files/Vagrantfile
--rw-r--r--   0 mitsuru    (501) staff       (20)     1078 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/vagrant/files/growfs.sh
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.938268 hive_builder-3.6.5/hive_builder/playbooks/roles/vagrant/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2413 2019-10-24 10:08:14.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/vagrant/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.938682 hive_builder-3.6.5/hive_builder/playbooks/roles/vagrant/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1116 2022-04-17 00:22:42.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/vagrant/templates/vagrant_vars.yml.j2
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.939426 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/
--rw-r--r--   0 mitsuru    (501) staff       (20)     6148 2020-07-22 21:27:18.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/.DS_Store
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.955319 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/files/
--rw-r--r--   0 mitsuru    (501) staff       (20)     3414 2021-04-19 23:53:15.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/files/Template_App_systemd_Services.xml
--rw-r--r--   0 mitsuru    (501) staff       (20)     8115 2021-04-19 23:53:15.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/files/hive-repository-server.xml
--rw-r--r--   0 mitsuru    (501) staff       (20)     1601 2020-11-07 23:35:22.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/files/hive-server-selinux.xml
--rw-r--r--   0 mitsuru    (501) staff       (20)     2337 2021-09-10 07:23:54.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/files/hive-server.xml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.956065 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     4694 2022-02-06 13:33:37.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.956786 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)     2638 2022-03-19 23:56:40.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/templates/zabbix.yml.j2
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.957505 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)      269 2022-03-19 23:56:40.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/vars/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.940245 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/
--rw-r--r--   0 mitsuru    (501) staff       (20)     6148 2021-02-13 23:46:33.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/.DS_Store
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.946552 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/
--rw-r--r--   0 mitsuru    (501) staff       (20)      144 2021-03-08 14:16:19.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/ausearch.conf
--rw-r--r--   0 mitsuru    (501) staff       (20)    14795 2022-03-02 02:57:32.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/docker-service.py
--rw-r--r--   0 mitsuru    (501) staff       (20)     1337 2020-04-29 23:37:01.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/docker-volume-discover.py
--rw-r--r--   0 mitsuru    (501) staff       (20)      269 2020-06-22 09:50:05.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/drbd-resource.conf
--rw-r--r--   0 mitsuru    (501) staff       (20)     6520 2021-09-10 07:23:54.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/hive.te
--rw-r--r--   0 mitsuru    (501) staff       (20)     4960 2021-12-06 23:14:51.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/hive.te.amzn
--rw-r--r--   0 mitsuru    (501) staff       (20)      115 2021-03-08 14:16:19.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/service_discovery_blacklist
--rw-r--r--   0 mitsuru    (501) staff       (20)       62 2020-04-29 23:37:01.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/sudoers.zabbix
--rw-r--r--   0 mitsuru    (501) staff       (20)      360 2021-03-08 14:16:19.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/userparameter_systemd_services.conf
--rw-r--r--   0 mitsuru    (501) staff       (20)      739 2021-03-08 14:16:19.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_discovery.sh
--rw-r--r--   0 mitsuru    (501) staff       (20)      461 2020-11-07 23:35:21.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_restart_check.sh
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.947394 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/handlers/
--rw-r--r--   0 mitsuru    (501) staff       (20)      389 2021-04-13 09:59:19.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/handlers/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.948203 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/tasks/
--rw-r--r--   0 mitsuru    (501) staff       (20)     6203 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/tasks/main.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.951625 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/templates/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1397 2021-03-08 14:16:19.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/templates/docker-service.j2
--rw-r--r--   0 mitsuru    (501) staff       (20)      345 2020-11-07 23:35:22.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/templates/docker-volume.j2
--rw-r--r--   0 mitsuru    (501) staff       (20)      354 2021-04-13 09:59:19.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix-agent-cache-builder.service
--rw-r--r--   0 mitsuru    (501) staff       (20)      196 2021-04-13 09:59:19.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix-agent-cache-builder.timer
--rw-r--r--   0 mitsuru    (501) staff       (20)    10611 2022-03-19 23:56:40.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix_agentd.conf.j2
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.952340 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/vars/
--rw-r--r--   0 mitsuru    (501) staff       (20)      681 2022-03-19 23:56:40.000000 hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/vars/main.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)     2482 2021-09-10 07:23:54.000000 hive_builder-3.6.5/hive_builder/playbooks/setup-hosts.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.958534 hive_builder-3.6.5/hive_builder/plugins/
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.961776 hive_builder-3.6.5/hive_builder/plugins/__pycache__/
--rw-r--r--   0 mitsuru    (501) staff       (20)    10083 2019-09-12 09:08:48.000000 hive_builder-3.6.5/hive_builder/plugins/__pycache__/hive_inventory.cpython-37.pyc
--rw-r--r--   0 mitsuru    (501) staff       (20)    13911 2021-09-17 02:52:35.000000 hive_builder-3.6.5/hive_builder/plugins/__pycache__/hive_inventory.cpython-39.pyc
--rw-r--r--   0 mitsuru    (501) staff       (20)     6687 2019-09-15 22:16:04.000000 hive_builder-3.6.5/hive_builder/plugins/__pycache__/hive_services.cpython-37.pyc
--rw-r--r--   0 mitsuru    (501) staff       (20)     9358 2021-09-03 03:08:19.000000 hive_builder-3.6.5/hive_builder/plugins/__pycache__/hive_services.cpython-39.pyc
--rw-r--r--   0 mitsuru    (501) staff       (20)    19580 2023-03-31 07:51:53.000000 hive_builder-3.6.5/hive_builder/plugins/hive_inventory.py
--rw-r--r--   0 mitsuru    (501) staff       (20)    14761 2022-11-14 23:07:24.000000 hive_builder-3.6.5/hive_builder/plugins/hive_services.py
--rw-r--r--   0 mitsuru    (501) staff       (20)      235 2022-05-23 09:55:27.000000 hive_builder-3.6.5/hive_builder/requirements.yml
--rw-r--r--   0 mitsuru    (501) staff       (20)    11579 2022-12-02 00:39:10.000000 hive_builder-3.6.5/hive_builder/variables_metainf.yml
-drwxr-xr-x   0 mitsuru    (501) staff       (20)        0 2023-03-31 07:52:58.849867 hive_builder-3.6.5/hive_builder.egg-info/
--rw-r--r--   0 mitsuru    (501) staff       (20)     1678 2023-03-31 07:52:58.000000 hive_builder-3.6.5/hive_builder.egg-info/PKG-INFO
--rw-r--r--   0 mitsuru    (501) staff       (20)    12050 2023-03-31 07:52:58.000000 hive_builder-3.6.5/hive_builder.egg-info/SOURCES.txt
--rw-r--r--   0 mitsuru    (501) staff       (20)        1 2023-03-31 07:52:58.000000 hive_builder-3.6.5/hive_builder.egg-info/dependency_links.txt
--rw-r--r--   0 mitsuru    (501) staff       (20)       47 2023-03-31 07:52:58.000000 hive_builder-3.6.5/hive_builder.egg-info/entry_points.txt
--rw-r--r--   0 mitsuru    (501) staff       (20)        1 2023-03-31 07:52:58.000000 hive_builder-3.6.5/hive_builder.egg-info/not-zip-safe
--rw-r--r--   0 mitsuru    (501) staff       (20)      104 2023-03-31 07:52:58.000000 hive_builder-3.6.5/hive_builder.egg-info/requires.txt
--rw-r--r--   0 mitsuru    (501) staff       (20)       13 2023-03-31 07:52:58.000000 hive_builder-3.6.5/hive_builder.egg-info/top_level.txt
--rwxr-xr-x   0 mitsuru    (501) staff       (20)     4390 2021-03-18 05:46:53.000000 hive_builder-3.6.5/release.sh
--rw-r--r--   0 mitsuru    (501) staff       (20)      888 2023-03-31 07:52:58.963958 hive_builder-3.6.5/setup.cfg
--rw-r--r--   0 mitsuru    (501) staff       (20)       64 2019-09-17 13:58:23.000000 hive_builder-3.6.5/setup.py
+-rw-r--r--   0        0        0     1074 2023-05-09 04:17:55.879931 hive_builder-3.6.6/LICENSE
+-rw-r--r--   0        0        0     1231 2023-05-09 04:17:55.879931 hive_builder-3.6.6/README.md
+-rwxr-xr-x   0        0        0      312 2023-05-09 04:17:55.891931 hive_builder-3.6.6/hive_builder/__init__.py
+-rw-r--r--   0        0        0     1031 2023-05-09 04:17:55.891931 hive_builder-3.6.6/hive_builder/hive-completion.sh
+-rw-r--r--   0        0        0    26961 2023-05-09 04:17:55.891931 hive_builder-3.6.6/hive_builder/hive.py
+-rw-r--r--   0        0        0    14020 2023-05-09 04:17:55.891931 hive_builder-3.6.6/hive_builder/lib/azure_rm_storageshare.py
+-rw-r--r--   0        0        0    14954 2023-05-09 04:17:55.891931 hive_builder-3.6.6/hive_builder/lib/hive_vagrant.py
+-rw-r--r--   0        0        0     5832 2023-05-09 04:17:55.891931 hive_builder-3.6.6/hive_builder/playbooks/build-images.yml
+-rw-r--r--   0        0        0     1943 2023-05-09 04:17:55.891931 hive_builder-3.6.6/hive_builder/playbooks/build-infra.yml
+-rw-r--r--   0        0        0     1084 2023-05-09 04:17:55.891931 hive_builder-3.6.6/hive_builder/playbooks/build-networks.yml
+-rw-r--r--   0        0        0     2447 2023-05-09 04:17:55.891931 hive_builder-3.6.6/hive_builder/playbooks/build-volumes.yml
+-rw-r--r--   0        0        0       81 2023-05-09 04:17:55.891931 hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/addon/tasks/main.yml
+-rw-r--r--   0        0        0       40 2023-05-09 04:17:55.891931 hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-certificate/files/extfile.cnf
+-rw-r--r--   0        0        0     1783 2023-05-09 04:17:55.891931 hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-certificate/tasks/main.yml
+-rw-r--r--   0        0        0      356 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-syslog/tasks/main.yml
+-rw-r--r--   0        0        0      946 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-syslog/templates/transfer.conf.j2
+-rw-r--r--   0        0        0      650 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-trust-ca/tasks/main.yml
+-rw-r--r--   0        0        0      351 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/tasks/main.yml
+-rw-r--r--   0        0        0       49 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/vars/main.yml
+-rw-r--r--   0        0        0      323 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/tasks/main.yml
+-rw-r--r--   0        0        0       49 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/vars/main.yml
+-rw-r--r--   0        0        0      409 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/tasks/main.yml
+-rw-r--r--   0        0        0       49 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/vars/main.yml
+-rw-r--r--   0        0        0      274 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/python-aptk/tasks/main.yml
+-rw-r--r--   0        0        0     9564 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/deploy-services.yml
+-rw-r--r--   0        0        0     2558 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/group_vars/hosts.yml
+-rw-r--r--   0        0        0      129 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/group_vars/mother.yml
+-rw-r--r--   0        0        0     1015 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/initialize-services.yml
+-rw-r--r--   0        0        0     2430 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/iptables.yml
+-rw-r--r--   0        0        0     2479 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/push-image.yml
+-rw-r--r--   0        0        0     3107 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/aws/tasks/build-aws.yml
+-rw-r--r--   0        0        0     3627 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/aws/tasks/create_instance.yml
+-rw-r--r--   0        0        0     2665 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/aws/tasks/destroy-aws.yml
+-rw-r--r--   0        0        0      327 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/aws/tasks/main.yml
+-rw-r--r--   0        0        0      217 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/aws/tasks/stop-aws.yml
+-rw-r--r--   0        0        0       46 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/aws/templates/aws_cli_config.j2
+-rw-r--r--   0        0        0      102 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/aws/templates/aws_cli_credentials.j2
+-rw-r--r--   0        0        0      138 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/aws/templates/azure_cli_credentials.j2
+-rw-r--r--   0        0        0      138 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/aws/templates/cloudstack.ini.j2
+-rw-r--r--   0        0        0     1497 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/aws/vars/main.yml
+-rw-r--r--   0        0        0     3273 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/azure/tasks/build-azure.yml
+-rw-r--r--   0        0        0     3434 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/azure/tasks/create_instance.yml
+-rw-r--r--   0        0        0     1932 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/azure/tasks/destroy-azure.yml
+-rw-r--r--   0        0        0      326 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/azure/tasks/main.yml
+-rw-r--r--   0        0        0      297 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/azure/tasks/stop-azure.yml
+-rw-r--r--   0        0        0      647 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/azure/vars/main.yml
+-rw-r--r--   0        0        0      589 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/backup-tools/tasks/main.yml
+-rw-r--r--   0        0        0      179 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/backup-tools/templates/backup.service
+-rw-r--r--   0        0        0      126 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/backup-tools/templates/backup.timer
+-rw-r--r--   0        0        0     5210 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/backup-tools/templates/hive-backup.sh
+-rw-r--r--   0        0        0       85 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/base/files/NetworkManager-wait-online.service.d/override.conf
+-rw-r--r--   0        0        0     1210 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/base/tasks/fixed-yum-url.yml
+-rw-r--r--   0        0        0     1796 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/base/tasks/growfs.yml
+-rw-r--r--   0        0        0     6801 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/base/tasks/main.yml
+-rw-r--r--   0        0        0       77 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/ca/files/extfile.cnf
+-rw-r--r--   0        0        0     1290 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/ca/tasks/main.yml
+-rw-r--r--   0        0        0      268 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/ca/vars/main.yml
+-rw-r--r--   0        0        0     4726 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/docker/tasks/main.yml
+-rw-r--r--   0        0        0      321 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/docker/templates/daemon.json.j2
+-rw-r--r--   0        0        0      331 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/docker/templates/override.conf
+-rw-r--r--   0        0        0     2301 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/docker-client/tasks/main.yml
+-rw-r--r--   0        0        0     1770 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/docker-client/templates/dcp
+-rw-r--r--   0        0        0     1467 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/docker-client/templates/dexec
+-rw-r--r--   0        0        0      678 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/docker-client/templates/dsh
+-rw-r--r--   0        0        0      170 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/docker-client/vars/main.yml
+-rw-r--r--   0        0        0     1032 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/docker-client-proxy/tasks/main.yml
+-rw-r--r--   0        0        0      233 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/docker-client-proxy/templates/config.json.j2
+-rw-r--r--   0        0        0      147 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/docker-compose/tasks/main.yml
+-rw-r--r--   0        0        0      229 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/drbd/files/drbd-resource@.service
+-rw-r--r--   0        0        0      309 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/drbd/files/waitdevice
+-rw-r--r--   0        0        0     3060 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/drbd/tasks/main.yml
+-rw-r--r--   0        0        0     3381 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/drbd/tasks/vg.yml
+-rw-r--r--   0        0        0      442 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/drbd/vars/main.yml
+-rw-r--r--   0        0        0     5426 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/drbd-resource/tasks/main.yml
+-rw-r--r--   0        0        0     1568 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/drbd-resource/templates/volume.res
+-rw-r--r--   0        0        0      421 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/drbd-resource/vars/main.yml
+-rw-r--r--   0        0        0    27684 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/follow-swarm-service/files/follow-swarm-service.py
+-rw-r--r--   0        0        0     1411 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/follow-swarm-service/tasks/main.yml
+-rw-r--r--   0        0        0      309 2023-05-09 04:17:55.895931 hive_builder-3.6.6/hive_builder/playbooks/roles/follow-swarm-service/templates/follow-swarm-service.service
+-rw-r--r--   0        0        0     2850 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/gcp/tasks/build-gcp.yml
+-rw-r--r--   0        0        0     3021 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/gcp/tasks/create_instance.yml
+-rw-r--r--   0        0        0     3289 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/gcp/tasks/destroy-gcp.yml
+-rw-r--r--   0        0        0      314 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/gcp/tasks/main.yml
+-rw-r--r--   0        0        0      396 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/gcp/tasks/stop-gcp.yml
+-rw-r--r--   0        0        0      741 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/gcp/vars/main.yml
+-rw-r--r--   0        0        0      338 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/hostsfile/tasks/main.yml
+-rw-r--r--   0        0        0     1403 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/internal-network/tasks/main.yml
+-rw-r--r--   0        0        0      625 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/iptables/tasks/main.yml
+-rw-r--r--   0        0        0     4319 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/kickstart/tasks/main.yml
+-rw-r--r--   0        0        0     3345 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/kickstart/templates/kickstart.j2
+-rw-r--r--   0        0        0      171 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/kickstart/vars/main.yml
+-rw-r--r--   0        0        0      118 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/monitor-service-log/handlers/main.yml
+-rw-r--r--   0        0        0      875 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/monitor-service-log/tasks/main.yml
+-rw-r--r--   0        0        0     1017 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/monitor-service-log/templates/monitor-service-log.j2
+-rw-r--r--   0        0        0     2436 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/nfs-aws-volumes/tasks/main.yml
+-rw-r--r--   0        0        0     2001 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/nfs-azure-volumes/tasks/main.yml
+-rw-r--r--   0        0        0     2528 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/nfs-gcp-volumes/tasks/main.yml
+-rw-r--r--   0        0        0      531 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/ntp-client/tasks/main.yml
+-rw-r--r--   0        0        0     2650 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/pip-venv/tasks/main.yml
+-rw-r--r--   0        0        0      403 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/prepared/tasks/main.yml
+-rw-r--r--   0        0        0      665 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/prepared/tasks/setup.yml
+-rw-r--r--   0        0        0       79 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/prepared/vars/main.yml
+-rw-r--r--   0        0        0      394 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/reboot/handlers/main.yml
+-rw-r--r--   0        0        0     1712 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/registry/tasks/main.yml
+-rw-r--r--   0        0        0       57 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/registry/templates/daemon.json.j2
+-rw-r--r--   0        0        0      985 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/registry/templates/registry.yml.j2
+-rw-r--r--   0        0        0      118 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/rsyslogd/handlers/main.yml
+-rw-r--r--   0        0        0     1338 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/rsyslogd/tasks/main.yml
+-rw-r--r--   0        0        0     3184 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/rsyslogd/templates/services.conf
+-rw-r--r--   0        0        0      788 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/service-backup/tasks/main.yml
+-rw-r--r--   0        0        0     5337 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/service-backup/templates/service-backup.sh.j2
+-rw-r--r--   0        0        0     1148 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/strict-source-ip/tasks/main.yml
+-rw-r--r--   0        0        0     6226 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/swarm/tasks/main.yml
+-rw-r--r--   0        0        0      220 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/tls-certificate/handlers/main.yml
+-rw-r--r--   0        0        0     2912 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/tls-certificate/tasks/main.yml
+-rw-r--r--   0        0        0      188 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/tls-certificate/templates/extfile.cnf
+-rw-r--r--   0        0        0      508 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/tls-certificate/vars/main.yml
+-rw-r--r--   0        0        0      433 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/users/tasks/known-hosts.yml
+-rw-r--r--   0        0        0     1157 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/users/tasks/main.yml
+-rw-r--r--   0        0        0       40 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/users/templates/sudoer.j2
+-rw-r--r--   0        0        0     3160 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/vagrant/files/Vagrantfile
+-rw-r--r--   0        0        0     1078 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/vagrant/files/growfs.sh
+-rw-r--r--   0        0        0     2413 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/vagrant/tasks/main.yml
+-rw-r--r--   0        0        0     1116 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/vagrant/templates/vagrant_vars.yml.j2
+-rw-r--r--   0        0        0     3414 2023-05-09 04:17:55.903931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix/files/Template_App_systemd_Services.xml
+-rw-r--r--   0        0        0     8115 2023-05-09 04:17:55.903931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix/files/hive-repository-server.xml
+-rw-r--r--   0        0        0     1601 2023-05-09 04:17:55.903931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix/files/hive-server-selinux.xml
+-rw-r--r--   0        0        0     2337 2023-05-09 04:17:55.903931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix/files/hive-server.xml
+-rw-r--r--   0        0        0     4694 2023-05-09 04:17:55.903931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix/tasks/main.yml
+-rw-r--r--   0        0        0     2638 2023-05-09 04:17:55.903931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix/templates/zabbix.yml.j2
+-rw-r--r--   0        0        0      269 2023-05-09 04:17:55.903931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix/vars/main.yml
+-rw-r--r--   0        0        0      144 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/ausearch.conf
+-rw-r--r--   0        0        0    14795 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/docker-service.py
+-rw-r--r--   0        0        0     1337 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/docker-volume-discover.py
+-rw-r--r--   0        0        0      269 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/drbd-resource.conf
+-rw-r--r--   0        0        0     6520 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/hive.te
+-rw-r--r--   0        0        0     4960 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/hive.te.amzn
+-rw-r--r--   0        0        0      115 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/service_discovery_blacklist
+-rw-r--r--   0        0        0       62 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/sudoers.zabbix
+-rw-r--r--   0        0        0      360 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/userparameter_systemd_services.conf
+-rw-r--r--   0        0        0      739 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_discovery.sh
+-rw-r--r--   0        0        0      461 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_restart_check.sh
+-rw-r--r--   0        0        0      389 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/handlers/main.yml
+-rw-r--r--   0        0        0     6203 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/tasks/main.yml
+-rw-r--r--   0        0        0     1397 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/templates/docker-service.j2
+-rw-r--r--   0        0        0      345 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/templates/docker-volume.j2
+-rw-r--r--   0        0        0      354 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix-agent-cache-builder.service
+-rw-r--r--   0        0        0      196 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix-agent-cache-builder.timer
+-rw-r--r--   0        0        0    10611 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix_agentd.conf.j2
+-rw-r--r--   0        0        0      681 2023-05-09 04:17:55.899931 hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/vars/main.yml
+-rw-r--r--   0        0        0     2482 2023-05-09 04:17:55.903931 hive_builder-3.6.6/hive_builder/playbooks/setup-hosts.yml
+-rw-r--r--   0        0        0    20056 2023-05-09 04:17:55.903931 hive_builder-3.6.6/hive_builder/plugins/hive_inventory.py
+-rw-r--r--   0        0        0    14761 2023-05-09 04:17:55.903931 hive_builder-3.6.6/hive_builder/plugins/hive_services.py
+-rw-r--r--   0        0        0      235 2023-05-09 04:17:55.903931 hive_builder-3.6.6/hive_builder/requirements.yml
+-rw-r--r--   0        0        0    11579 2023-05-09 04:17:55.903931 hive_builder-3.6.6/hive_builder/variables_metainf.yml
+-rw-r--r--   0        0        0      633 2023-05-09 04:17:55.903931 hive_builder-3.6.6/pyproject.toml
+-rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 hive_builder-3.6.6/PKG-INFO
```

### Comparing `hive_builder-3.6.5/LICENSE` & `hive_builder-3.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/README.md` & `hive_builder-3.6.6/README.md`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/hive-completion.sh` & `hive_builder-3.6.6/hive_builder/hive-completion.sh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/hive.py` & `hive_builder-3.6.6/hive_builder/hive.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/lib/azure_rm_storageshare.py` & `hive_builder-3.6.6/hive_builder/lib/azure_rm_storageshare.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/lib/hive_vagrant.py` & `hive_builder-3.6.6/hive_builder/lib/hive_vagrant.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/build-images.yml` & `hive_builder-3.6.6/hive_builder/playbooks/build-images.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/build-infra.yml` & `hive_builder-3.6.6/hive_builder/playbooks/build-infra.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/build-networks.yml` & `hive_builder-3.6.6/hive_builder/playbooks/build-networks.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/build-volumes.yml` & `hive_builder-3.6.6/hive_builder/playbooks/build-volumes.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-certificate/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-certificate/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-syslog/templates/transfer.conf.j2` & `hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-syslog/templates/transfer.conf.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/builtin_roles/hive-trust-ca/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/builtin_roles/hive-trust-ca/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/deploy-services.yml` & `hive_builder-3.6.6/hive_builder/playbooks/deploy-services.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/group_vars/hosts.yml` & `hive_builder-3.6.6/hive_builder/playbooks/group_vars/hosts.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/initialize-services.yml` & `hive_builder-3.6.6/hive_builder/playbooks/initialize-services.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/iptables.yml` & `hive_builder-3.6.6/hive_builder/playbooks/iptables.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/push-image.yml` & `hive_builder-3.6.6/hive_builder/playbooks/push-image.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/aws/tasks/build-aws.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/aws/tasks/build-aws.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/aws/tasks/create_instance.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/aws/tasks/create_instance.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/aws/tasks/destroy-aws.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/aws/tasks/destroy-aws.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/aws/vars/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/aws/vars/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/azure/tasks/build-azure.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/azure/tasks/build-azure.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/azure/tasks/create_instance.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/azure/tasks/create_instance.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/azure/tasks/destroy-azure.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/azure/tasks/destroy-azure.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/azure/vars/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/azure/vars/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/backup-tools/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/backup-tools/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/backup-tools/templates/hive-backup.sh` & `hive_builder-3.6.6/hive_builder/playbooks/roles/backup-tools/templates/hive-backup.sh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/base/tasks/fixed-yum-url.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/base/tasks/fixed-yum-url.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/base/tasks/growfs.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/base/tasks/growfs.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/base/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/base/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/ca/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/ca/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/docker/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/docker/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/docker-client/tasks/main.yml`

 * *Files 9% similar despite different names*

```diff
@@ -31,18 +31,22 @@
 # please consult the documentation on ansible_python_interpreter, for example via `pip install docker`
 # or `pip install docker-py` (Python 2.6). The error was: No module named ''six'''
 # The verions when above error occured
 # $ python --version
 # Python 3.7.9
 # $ pip list | grep docker
 # docker           5.0.0
+
+# 2023/05/05 avoid error in docker login task: Error connecting: Error while fetching server API version: request() got an unexpected keyword argument ''chunked''
+# https://github.com/docker/docker-py/issues/3113#issue-1685565058
 - name: install docker python module
   become: False
   pip:
     name:
+    - "requests<2.29"
     - docker
     - six
     state: present
     virtualenv: "{{ hive_home_dir }}/docker"
 - name: install utility comnand
   template:
     dest: /usr/bin/{{ item }}
```

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client/templates/dcp` & `hive_builder-3.6.6/hive_builder/playbooks/roles/docker-client/templates/dcp`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client/templates/dexec` & `hive_builder-3.6.6/hive_builder/playbooks/roles/docker-client/templates/dexec`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client/templates/dsh` & `hive_builder-3.6.6/hive_builder/playbooks/roles/docker-client/templates/dsh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/docker-client-proxy/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/docker-client-proxy/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/drbd/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/drbd/tasks/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
          else '9.0.27/drbd9-rpm-amzn2'  if uname_result.stdout is version('4.14.225', 'lt')
          else '9.1.2/drbd9-rpm-amzn2'  if uname_result.stdout is version('4.14.232', 'lt')
          else '9.1.2-1/drbd9-rpm-amzn2'
         ) if ansible_distribution == 'Amazon' else
         (
          'Latests/drbd-9.1.12-v9.22.0-4.18.0-372.32.1.el8.x86_64' if ansible_distribution_release == 'Ootpa'
          else 'Latests/drbd-9.1.12-v9.22.0-4.18.0-425.3.1.el8.x86_64' if uname_result.stdout == '4.18.0-425.3.1.el8.x86_64'
-         else 'Latests/drbd-9.1.12-v9.22.0-4.18.0-425.13.1.el8_7.x86_64'
+         else 'Latests/drbd-9.1.12-v9.22.0-4.18.0-425.13.1.el8_7.x86_64' if uname_result.stdout == '4.18.0-425.13.1.el8.x86_64'
+         else 'Latests/drbd-9.2.3-v9.22.0-4.18.0-425.19.2.el8_7.x86_64'
         ) ) + '.tar.gz') }}
     dest: /root/drbd9-rpm.tar.gz
 - name: extract drbd rpm files
   unarchive:
     src: /root/drbd9-rpm.tar.gz
     remote_src: yes
     dest: /root/
```

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/drbd/tasks/vg.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/drbd/tasks/vg.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/drbd-resource/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/drbd-resource/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/drbd-resource/templates/volume.res` & `hive_builder-3.6.6/hive_builder/playbooks/roles/drbd-resource/templates/volume.res`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/follow-swarm-service/files/follow-swarm-service.py` & `hive_builder-3.6.6/hive_builder/playbooks/roles/follow-swarm-service/files/follow-swarm-service.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/follow-swarm-service/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/follow-swarm-service/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/gcp/tasks/build-gcp.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/gcp/tasks/build-gcp.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/gcp/tasks/create_instance.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/gcp/tasks/create_instance.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/gcp/tasks/destroy-gcp.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/gcp/tasks/destroy-gcp.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/gcp/vars/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/gcp/vars/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/internal-network/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/internal-network/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/iptables/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/iptables/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/kickstart/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/kickstart/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/kickstart/templates/kickstart.j2` & `hive_builder-3.6.6/hive_builder/playbooks/roles/kickstart/templates/kickstart.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/monitor-service-log/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/monitor-service-log/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/monitor-service-log/templates/monitor-service-log.j2` & `hive_builder-3.6.6/hive_builder/playbooks/roles/monitor-service-log/templates/monitor-service-log.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/nfs-aws-volumes/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/nfs-aws-volumes/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/nfs-azure-volumes/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/nfs-azure-volumes/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/nfs-gcp-volumes/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/nfs-gcp-volumes/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/ntp-client/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/ntp-client/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/pip-venv/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/pip-venv/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/prepared/tasks/setup.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/prepared/tasks/setup.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/registry/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/registry/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/registry/templates/registry.yml.j2` & `hive_builder-3.6.6/hive_builder/playbooks/roles/registry/templates/registry.yml.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/rsyslogd/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/rsyslogd/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/rsyslogd/templates/services.conf` & `hive_builder-3.6.6/hive_builder/playbooks/roles/rsyslogd/templates/services.conf`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 template(name="logFormat" type="string" string="%timegenerated:::date-year%/%timegenerated:::date-month%/%timegenerated:::date-day% %timegenerated:::date-hour%:%timegenerated:::date-minute%:%timegenerated:::date-second% %syslogtag% %msg%\n")
 template(name="logFormatStandalone" type="string" string="%timegenerated:::date-year%/%timegenerated:::date-month%/%timegenerated:::date-day% %timegenerated:::date-hour%:%timegenerated:::date-minute%:%timegenerated:::date-second% %syslogfacility-text%.%syslogseverity-text%: %syslogtag%%msg:::sp-if-no-1st-sp%%msg:::drop-last-lf%\n")
 template(name="logFormatOther" type="string" string="%timegenerated:::date-year%/%timegenerated:::date-month%/%timegenerated:::date-day% %timegenerated:::date-hour%:%timegenerated:::date-minute%:%timegenerated:::date-second% %hostname% %syslogfacility-text%.%syslogseverity-text%: %syslogtag%%msg:::sp-if-no-1st-sp%%msg:::drop-last-lf%\n")
 template(name="logFormatErrorStandalone" type="string" string="%timegenerated:::date-year%/%timegenerated:::date-month%/%timegenerated:::date-day% %timegenerated:::date-hour%:%timegenerated:::date-minute%:%timegenerated:::date-second% /var/log/services/%HOSTNAME%.log %syslogtag%%msg:::sp-if-no-1st-sp%%msg:::drop-last-lf%\n")
 template(name="logFormatErrorApp" type="string" string="%timegenerated:::date-year%/%timegenerated:::date-month%/%timegenerated:::date-day% %timegenerated:::date-hour%:%timegenerated:::date-minute%:%timegenerated:::date-second% /var/log/services/%APP-NAME%.log %syslogtag%%msg:::sp-if-no-1st-sp%%msg:::drop-last-lf%\n")
 template(name="logFormatErrorInner" type="string" string="%timegenerated:::date-year%/%timegenerated:::date-month%/%timegenerated:::date-day% %timegenerated:::date-hour%:%timegenerated:::date-minute%:%timegenerated:::date-second% /var/log/services/%HOSTNAME%.%APP-NAME%.log %syslogtag%%msg:::sp-if-no-1st-sp%%msg:::drop-last-lf%\n")
 
-if not re_match($hostname, '^(localhost|{{ 'p-' if hive_stage == 'private' else 's-' if hive_stage == 'staging' else '' }}hive[0-9]+.{{ hive_name }})$') then {
+if not re_match($hostname, '^(localhost|{{ 'p-' if hive_stage == 'private' else 's-' if hive_stage == 'staging' else '' }}{{ hive_custom_hostname }}[0-9]+.{{ hive_name }})$') then {
   action(type="omfile" dynaFile="pathForStandalone" fileCreateMode="0640" fileGroup="zabbix" template="logFormatStandalone" action.copyMsg="on")
 } else if $syslogfacility-text == 'local0' then {
   action(type="omfile" dynaFile="pathForService" fileCreateMode="0640" fileGroup="zabbix" template="logFormat" action.copyMsg="on")
 }  else if $syslogfacility-text == 'local1' then {
   action(type="omfile" dynaFile="pathForInner" fileCreateMode="0640" fileGroup="zabbix" template="logFormat" action.copyMsg="on")
 } else {
   action(type="omfile" file="/var/log/service-other-facility.log" template="logFormatOther" action.copyMsg="on")
```

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/service-backup/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/service-backup/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/service-backup/templates/service-backup.sh.j2` & `hive_builder-3.6.6/hive_builder/playbooks/roles/service-backup/templates/service-backup.sh.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/strict-source-ip/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/strict-source-ip/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/swarm/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/swarm/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/tls-certificate/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/tls-certificate/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/users/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/users/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/vagrant/files/Vagrantfile` & `hive_builder-3.6.6/hive_builder/playbooks/roles/vagrant/files/Vagrantfile`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/vagrant/files/growfs.sh` & `hive_builder-3.6.6/hive_builder/playbooks/roles/vagrant/files/growfs.sh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/vagrant/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/vagrant/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/vagrant/templates/vagrant_vars.yml.j2` & `hive_builder-3.6.6/hive_builder/playbooks/roles/vagrant/templates/vagrant_vars.yml.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/files/Template_App_systemd_Services.xml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix/files/Template_App_systemd_Services.xml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/files/hive-repository-server.xml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix/files/hive-repository-server.xml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/files/hive-server-selinux.xml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix/files/hive-server-selinux.xml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/files/hive-server.xml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix/files/hive-server.xml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix/templates/zabbix.yml.j2` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix/templates/zabbix.yml.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/docker-service.py` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/docker-service.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/docker-volume-discover.py` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/docker-volume-discover.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/hive.te` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/hive.te`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/hive.te.amzn` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/hive.te.amzn`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_discovery.sh` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_discovery.sh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/tasks/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/templates/docker-service.j2` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/templates/docker-service.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix_agentd.conf.j2` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix_agentd.conf.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/roles/zabbix-agent/vars/main.yml` & `hive_builder-3.6.6/hive_builder/playbooks/roles/zabbix-agent/vars/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/playbooks/setup-hosts.yml` & `hive_builder-3.6.6/hive_builder/playbooks/setup-hosts.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/plugins/hive_inventory.py` & `hive_builder-3.6.6/hive_builder/plugins/hive_inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,14 +256,19 @@
         raise AnsibleParserError('dev cannot be specified when provider is IaaS')
       if 'bridge' in self.stage:
         raise AnsibleParserError('bridge cannot be specified when provider is IaaS')
 
   def add_stage_group(self):
     self.inventory.add_group(self.stage_name)
     self.inventory.set_variable(self.stage_name, 'hive_provider', self.provider)
+    custom_hostname = self.stage.get('custom_hostname', 'hive')
+    hostname_pattern = r'^[a-zA-Z0-9][a-zA-Z0-9-]*[a-zA-Z0-9]$'
+    if not (re.match(hostname_pattern, custom_hostname) and (len(custom_hostname)) + len(self.name) < 55):
+      raise AnsibleParserError('custom_hostname must consist of alphanumeric and hyphens, and custom_hostname + inventory_name be up to 55 in length')
+    self.inventory.set_variable(self.stage_name, 'hive_custom_hostname', custom_hostname)
 
   def set_subnets(self):
     self.subnets = []
     if 'cidr' not in self.stage:
       raise AnsibleParserError('cidr must be specified')
     mother_name = f'{self.stage_prefix}mother.{self.name}'
     self.inventory.add_host(mother_name, group='mother')
```

### Comparing `hive_builder-3.6.5/hive_builder/plugins/hive_services.py` & `hive_builder-3.6.6/hive_builder/plugins/hive_services.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.5/hive_builder/variables_metainf.yml` & `hive_builder-3.6.6/hive_builder/variables_metainf.yml`

 * *Files identical despite different names*

