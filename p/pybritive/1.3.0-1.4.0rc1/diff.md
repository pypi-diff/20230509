# Comparing `tmp/pybritive-1.3.0.tar.gz` & `tmp/pybritive-1.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybritive-1.3.0.tar", last modified: Tue Mar 28 17:28:18 2023, max compression
+gzip compressed data, was "pybritive-1.4.0rc1.tar", last modified: Tue May  9 14:43:24 2023, max compression
```

## Comparing `pybritive-1.3.0.tar` & `pybritive-1.4.0rc1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:28:18.212392 pybritive-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-28 17:28:08.000000 pybritive-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-28 17:28:18.212392 pybritive-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-28 17:28:08.000000 pybritive-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-28 17:28:08.000000 pybritive-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-28 17:28:18.212392 pybritive-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:28:18.196392 pybritive-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:28:18.200392 pybritive-1.3.0/src/pybritive/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41054 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/britive_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:28:18.200392 pybritive-1.3.0/src/pybritive/choices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/choices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/choices/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/choices/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/choices/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/choices/output_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/choices/ssh_key_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/cli_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:28:18.204392 pybritive-1.3.0/src/pybritive/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/checkin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/commands/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:28:18.204392 pybritive-1.3.0/src/pybritive/completers/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/completers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/completers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/completers/api_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/completers/bash_gte_42.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/completers/powershell_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/completers/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:28:18.204392 pybritive-1.3.0/src/pybritive/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/helpers/api_method_argument_dectorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/helpers/aws_credential_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/helpers/build_britive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/helpers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/helpers/cloud_credential_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/helpers/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/helpers/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/helpers/profile_argument_dectorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/helpers/split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:28:18.212392 pybritive-1.3.0/src/pybritive/options/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/aws_console_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/aws_credentials_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/aws_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/blocktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/britive_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/checked_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/configure_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/configure_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/configure_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/configure_tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/federation_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/force_renew.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/gcloud_key_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/justification.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/maxpolltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/output_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/passphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/silent.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/ssh_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/ssh_key_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/ssh_port.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/ssh_push_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/ssh_username.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-28 17:28:08.000000 pybritive-1.3.0/src/pybritive/options/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:28:18.200392 pybritive-1.3.0/src/pybritive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-28 17:28:18.000000 pybritive-1.3.0/src/pybritive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-03-28 17:28:18.000000 pybritive-1.3.0/src/pybritive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 17:28:18.000000 pybritive-1.3.0/src/pybritive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-28 17:28:18.000000 pybritive-1.3.0/src/pybritive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-28 17:28:18.000000 pybritive-1.3.0/src/pybritive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-28 17:28:18.000000 pybritive-1.3.0/src/pybritive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:28:18.212392 pybritive-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-28 17:28:08.000000 pybritive-1.3.0/tests/test_0100_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-03-28 17:28:08.000000 pybritive-1.3.0/tests/test_0200_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-28 17:28:08.000000 pybritive-1.3.0/tests/test_0300_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-28 17:28:08.000000 pybritive-1.3.0/tests/test_0400_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-28 17:28:08.000000 pybritive-1.3.0/tests/test_0450_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-03-28 17:28:08.000000 pybritive-1.3.0/tests/test_0500_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-28 17:28:08.000000 pybritive-1.3.0/tests/test_0600_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-28 17:28:08.000000 pybritive-1.3.0/tests/test_0700_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-28 17:28:08.000000 pybritive-1.3.0/tests/test_0800_checkin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-28 17:28:08.000000 pybritive-1.3.0/tests/test_0850_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-28 17:28:08.000000 pybritive-1.3.0/tests/test_0900_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-28 17:28:08.000000 pybritive-1.3.0/tests/test_1000_logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:24.269453 pybritive-1.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-09 14:43:24.269453 pybritive-1.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-09 14:43:24.269453 pybritive-1.4.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:24.241452 pybritive-1.4.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:24.245452 pybritive-1.4.0rc1/src/pybritive/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42134 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/britive_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:24.253452 pybritive-1.4.0rc1/src/pybritive/choices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/choices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/choices/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/choices/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/choices/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/choices/output_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/choices/ssh_key_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/cli_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:24.257452 pybritive-1.4.0rc1/src/pybritive/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/commands/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:24.257452 pybritive-1.4.0rc1/src/pybritive/completers/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/completers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/completers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/completers/api_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/completers/bash_gte_42.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/completers/powershell_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/completers/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:24.261453 pybritive-1.4.0rc1/src/pybritive/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/helpers/api_method_argument_dectorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/helpers/aws_credential_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/helpers/build_britive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/helpers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/helpers/cloud_credential_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/helpers/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/helpers/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/helpers/profile_argument_dectorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/helpers/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:24.265453 pybritive-1.4.0rc1/src/pybritive/options/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/aws_console_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/aws_credentials_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/aws_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/blocktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/britive_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/checked_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/configure_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/configure_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/configure_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/configure_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/federation_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/force_renew.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/gcloud_key_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/justification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/maxpolltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/output_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/passphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/silent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/ssh_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/ssh_key_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/ssh_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/ssh_push_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/ssh_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/src/pybritive/options/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:24.249452 pybritive-1.4.0rc1/src/pybritive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-09 14:43:24.000000 pybritive-1.4.0rc1/src/pybritive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-09 14:43:24.000000 pybritive-1.4.0rc1/src/pybritive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:43:24.000000 pybritive-1.4.0rc1/src/pybritive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-09 14:43:24.000000 pybritive-1.4.0rc1/src/pybritive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-09 14:43:24.000000 pybritive-1.4.0rc1/src/pybritive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 14:43:24.000000 pybritive-1.4.0rc1/src/pybritive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:24.269453 pybritive-1.4.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/tests/test_0100_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/tests/test_0200_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/tests/test_0300_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/tests/test_0400_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/tests/test_0450_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/tests/test_0500_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/tests/test_0600_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/tests/test_0700_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/tests/test_0800_checkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/tests/test_0850_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/tests/test_0900_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-09 14:43:09.000000 pybritive-1.4.0rc1/tests/test_1000_logout.py
```

### Comparing `pybritive-1.3.0/LICENSE` & `pybritive-1.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/PKG-INFO` & `pybritive-1.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybritive
-Version: 1.3.0
+Version: 1.4.0rc1
 Summary: A pure Python CLI for Britive
 Home-page: https://www.britive.com
 Author: Britive Inc.
 Author-email: support@britive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybritive-1.3.0/README.md` & `pybritive-1.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/setup.cfg` & `pybritive-1.4.0rc1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pybritive
-version = 1.3.0
+version = 1.4.0rc1
 author = Britive Inc.
 author_email = support@britive.com
 description = A pure Python CLI for Britive
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.britive.com
 classifiers = 
@@ -22,15 +22,15 @@
 	requests
 	PyYAML
 	merge_args
 	tabulate
 	toml
 	cryptography~=39.0.1
 	python-dateutil
-	britive>=2.18.0
+	britive>=2.19.0
 	jmespath
 	pyjwt
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
```

### Comparing `pybritive-1.3.0/src/pybritive/britive_cli.py` & `pybritive-1.4.0rc1/src/pybritive/britive_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,14 +201,34 @@
             output += f' (alias: {alias})'
         self.print(output, ignore_silent=True)
 
     def list_secrets(self):
         self.login()
         self.print(self.b.my_secrets.list(), ignore_silent=True)
 
+    def list_approvals(self):
+        self.login()
+        approvals = []
+        for approval in self.b.my_access.list_approvals():
+            approval.pop('resource', None)
+            approval.pop('consumer', None)
+            approval.pop('timeToApprove', None)
+            approval.pop('validFor', None)
+            approval.pop('action', None)
+            approval.pop('approvers', None)
+            approval.pop('expirationTimeApproval', None)
+            approval.pop('updatedAt', None)
+            approval.pop('actionBy', None)
+            approval.pop('validForInDays', None)
+            approvals.append(approval)
+
+        approvals = sorted(approvals, key=lambda x: x['createdAt'])
+        approvals.reverse()
+        self.print(approvals, ignore_silent=True)
+
     def list_profiles(self, checked_out: bool = False):
         self.login()
         self._set_available_profiles()
         data = []
         checked_out_profiles = [
             f'{p["papId"]}-{p["environmentId"]}'
             for p in self.b.my_access.list_checked_out_profiles()
@@ -411,15 +431,15 @@
                 raise e
 
     @staticmethod
     def _should_check_force_renew(app, force_renew, console):
         return app in ['AWS', 'AWS Standalone'] and force_renew and not console
 
     def _split_profile_into_parts(self, profile):
-        profile_real = self.config.profile_aliases.get(profile, profile)
+        profile_real = self.config.profile_aliases.get(profile.lower(), profile)
         parts = profile_split(profile_real)
         if len(parts) == 2:  # handle shortcut for profiles where the app and environment name are the same
             parts = [parts[0], parts[0], parts[1]]
         if len(parts) != 3:
             raise click.ClickException('Provided profile string does not have the required parts.')
         parts_dict = {
             'app': parts[0],
@@ -434,15 +454,15 @@
         app_type = None
         credential_process_creds_found = False
         response = None
         self.verbose_checkout = verbose
 
         # these 2 modes implicitly say that console access should be checked out without having to provide
         # the --console flag
-        if mode in ['browser', 'console']:
+        if mode == 'console' or mode.startswith('browser'):
             console = True
 
         self._validate_justification(justification)
 
         if mode == 'awscredentialprocess':
             self.silent = True  # the aws credential process CANNOT output anything other than the expected JSON
             # we need to check the credential process cache for the credentials first
@@ -999,8 +1019,14 @@
         # vs. doing it "manually" - we do not want to actually make a request to the url in python
         # but use the url to pop open a browser
         console_url = requests.Request('GET', url, params=params).prepare().url
 
         browser = webbrowser.get(using=browser)
         browser.open(console_url)
 
+    def request_disposition(self, request_id, decision):
+        self.login()
 
+        if decision == 'approve':
+            self.b.my_access.approve_request(request_id=request_id)
+        if decision == 'reject':
+            self.b.my_access.reject_request(request_id=request_id)
```

### Comparing `pybritive-1.3.0/src/pybritive/choices/mode.py` & `pybritive-1.4.0rc1/src/pybritive/choices/mode.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/choices/output_format.py` & `pybritive-1.4.0rc1/src/pybritive/choices/output_format.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/cli_interface.py` & `pybritive-1.4.0rc1/src/pybritive/cli_interface.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/commands/api.py` & `pybritive-1.4.0rc1/src/pybritive/commands/api.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/commands/aws.py` & `pybritive-1.4.0rc1/src/pybritive/commands/aws.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/commands/cache.py` & `pybritive-1.4.0rc1/src/pybritive/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/commands/checkin.py` & `pybritive-1.4.0rc1/src/pybritive/commands/checkin.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/commands/checkout.py` & `pybritive-1.4.0rc1/src/pybritive/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/commands/configure.py` & `pybritive-1.4.0rc1/src/pybritive/commands/configure.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/commands/login.py` & `pybritive-1.4.0rc1/src/pybritive/commands/login.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/commands/ls.py` & `pybritive-1.4.0rc1/src/pybritive/commands/ls.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,8 +37,13 @@
 @build_britive
 @britive_options(names='format,tenant,token,silent,passphrase,federation_provider')
 def secrets(ctx, output_format, tenant, token, silent, passphrase, federation_provider):
     """List secrets for the currently authenticated identity."""
     ctx.obj.britive.list_secrets()
 
 
-
+@ls.command()
+@build_britive
+@britive_options(names='format,tenant,token,silent,passphrase,federation_provider')
+def approvals(ctx, output_format, tenant, token, silent, passphrase, federation_provider):
+    """List approvals for the currently authenticated identity."""
+    ctx.obj.britive.list_approvals()
```

### Comparing `pybritive-1.3.0/src/pybritive/commands/secret.py` & `pybritive-1.4.0rc1/src/pybritive/commands/secret.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/commands/ssh.py` & `pybritive-1.4.0rc1/src/pybritive/commands/ssh.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/completers/api.py` & `pybritive-1.4.0rc1/src/pybritive/completers/api.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/completers/api_command.py` & `pybritive-1.4.0rc1/src/pybritive/completers/api_command.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/completers/bash_gte_42.py` & `pybritive-1.4.0rc1/src/pybritive/completers/bash_gte_42.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/completers/powershell_completion.py` & `pybritive-1.4.0rc1/src/pybritive/completers/powershell_completion.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/completers/profile.py` & `pybritive-1.4.0rc1/src/pybritive/completers/profile.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/helpers/aws_credential_process.py` & `pybritive-1.4.0rc1/src/pybritive/helpers/aws_credential_process.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/helpers/build_britive.py` & `pybritive-1.4.0rc1/src/pybritive/helpers/build_britive.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/helpers/cache.py` & `pybritive-1.4.0rc1/src/pybritive/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/helpers/cloud_credential_printer.py` & `pybritive-1.4.0rc1/src/pybritive/helpers/cloud_credential_printer.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,51 +27,49 @@
         self.cli = cli
         self.silent = silent
         self.app_type = app_type
         self.profile = profile
         self.console = console
         mode = mode or 'json'  # set a default if nothing is provided via flag --mode/-m
         helper = mode.split('-')
-        env_prefix = helper[1] if 1 < len(helper) else None
         self.mode = helper[0]
+        self.mode_modifier = safe_list_get(mode.split('-', maxsplit=1), 1, None)
         self.credentials = credentials
-        self.on_windows = True if platform.system().lower() == 'windows' else False
-        if env_prefix:
-            self.env_command = env_options[env_prefix]
-        else:
-            self.env_command = env_options['wincmd'] if self.on_windows else env_options['nix']
+        if self.mode == 'env':
+            if self.mode_modifier:
+                self.env_command = env_options[self.mode_modifier]
+            else:
+                self.on_windows = True if platform.system().lower() == 'windows' else False
+                self.env_command = env_options['wincmd'] if self.on_windows else env_options['nix']
 
     def print(self):
         if self.console:
             self.print_console()
             return
-        mode_prefix = self.mode.split('-')[0]
-        if mode_prefix == 'text':
+        if self.mode == 'text':
             self.print_text()
-        if mode_prefix == 'json':
+        if self.mode == 'json':
             self.print_json()
-        if mode_prefix == 'env':
+        if self.mode == 'env':
             self.print_env()
-        if mode_prefix == 'integrate':
+        if self.mode == 'integrate':
             self.print_integrate()
-        if mode_prefix == 'azlogin':
+        if self.mode == 'azlogin':
             self.print_azlogin()
-        if mode_prefix == 'awscredentialprocess':
+        if self.mode == 'awscredentialprocess':
             self.print_awscredentialprocess()
-        if mode_prefix == 'azps':
+        if self.mode == 'azps':
             self.print_azps()
-        if mode_prefix == 'gcloudauth':
+        if self.mode == 'gcloudauth':
             self.print_gcloudauth()
 
     def print_console(self):
         url = self.credentials.get('url', self.credentials)
-
-        if self.mode.startswith('browser'):
-            browser_type = safe_list_get(self.mode.split('-', maxsplit=1), 1, None)
-            webbrowser.get(browser_type).open(url)
+        if self.mode == 'browser':
+            webbrowser.get(self.mode_modifier).open(url)
         else:
             self.cli.print(url, ignore_silent=True)
 
     def print_text(self):
         self._not_implemented()
 
     def print_json(self):
```

### Comparing `pybritive-1.3.0/src/pybritive/helpers/config.py` & `pybritive-1.4.0rc1/src/pybritive/helpers/config.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/helpers/credentials.py` & `pybritive-1.4.0rc1/src/pybritive/helpers/credentials.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/helpers/encryption.py` & `pybritive-1.4.0rc1/src/pybritive/helpers/encryption.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/helpers/split.py` & `pybritive-1.4.0rc1/src/pybritive/helpers/split.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/options/britive_options.py` & `pybritive-1.4.0rc1/src/pybritive/options/britive_options.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/options/browser.py` & `pybritive-1.4.0rc1/src/pybritive/options/browser.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/options/mode.py` & `pybritive-1.4.0rc1/src/pybritive/options/mode.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/options/output_format.py` & `pybritive-1.4.0rc1/src/pybritive/options/output_format.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive/options/version.py` & `pybritive-1.4.0rc1/src/pybritive/options/version.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/src/pybritive.egg-info/PKG-INFO` & `pybritive-1.4.0rc1/src/pybritive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybritive
-Version: 1.3.0
+Version: 1.4.0rc1
 Summary: A pure Python CLI for Britive
 Home-page: https://www.britive.com
 Author: Britive Inc.
 Author-email: support@britive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybritive-1.3.0/src/pybritive.egg-info/SOURCES.txt` & `pybritive-1.4.0rc1/src/pybritive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/tests/test_0100_version.py` & `pybritive-1.4.0rc1/tests/test_0100_version.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/tests/test_0200_configure.py` & `pybritive-1.4.0rc1/tests/test_0200_configure.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/tests/test_0400_ls.py` & `pybritive-1.4.0rc1/tests/test_0400_ls.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/tests/test_0500_secret.py` & `pybritive-1.4.0rc1/tests/test_0500_secret.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/tests/test_0700_checkout.py` & `pybritive-1.4.0rc1/tests/test_0700_checkout.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/tests/test_0850_clear.py` & `pybritive-1.4.0rc1/tests/test_0850_clear.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.3.0/tests/test_0900_login.py` & `pybritive-1.4.0rc1/tests/test_0900_login.py`

 * *Files identical despite different names*

