# Comparing `tmp/netbox_config_backup-1.4.2.tar.gz` & `tmp/netbox_config_backup-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_config_backup-1.4.2.tar", last modified: Mon May  8 15:26:22 2023, max compression
+gzip compressed data, was "netbox_config_backup-1.4.3.tar", last modified: Tue May  9 15:10:55 2023, max compression
```

## Comparing `netbox_config_backup-1.4.2.tar` & `netbox_config_backup-1.4.3.tar`

### file list

```diff
@@ -1,75 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.663224 netbox_config_backup-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 15:26:22.663224 netbox_config_backup-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.659224 netbox_config_backup-1.4.2/netbox_config_backup/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.659224 netbox_config_backup-1.4.2/netbox_config_backup/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.659224 netbox_config_backup-1.4.2/netbox_config_backup/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/management/commands/enqueue_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/management/commands/fix_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/management/commands/rebuild.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/management/commands/runbackup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.659224 netbox_config_backup-1.4.2/netbox_config_backup/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/migrations/0002_git_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/migrations/0003_primary_model_to_bigid.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/migrations/0004_custom_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/migrations/0005_commit_add_time_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/migrations/0008_backupjob_scheduled_nullable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/migrations/0010_backup_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/migrations/0011_alter_backup_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/migrations/0012_backup_status.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.659224 netbox_config_backup-1.4.2/netbox_config_backup/models/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/models/backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/models/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.655224 netbox_config_backup-1.4.2/netbox_config_backup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.663224 netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/backup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/backups.html
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/diff.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.663224 netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/inc/backup_tables.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/repository.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.655224 netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/switch_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.663224 netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/switch_templates/cisco_iosxe/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/switch_templates/cisco_iosxe/interface.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.663224 netbox_config_backup-1.4.2/netbox_config_backup/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/templatetags/ncb_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.663224 netbox_config_backup-1.4.2/netbox_config_backup/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/utils/backups.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/utils/rq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/netbox_config_backup/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:26:22.659224 netbox_config_backup-1.4.2/netbox_config_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 15:26:22.000000 netbox_config_backup-1.4.2/netbox_config_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-08 15:26:22.000000 netbox_config_backup-1.4.2/netbox_config_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:26:22.000000 netbox_config_backup-1.4.2/netbox_config_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:26:22.000000 netbox_config_backup-1.4.2/netbox_config_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-08 15:26:22.000000 netbox_config_backup-1.4.2/netbox_config_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 15:26:22.000000 netbox_config_backup-1.4.2/netbox_config_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:26:22.663224 netbox_config_backup-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-08 15:26:17.000000 netbox_config_backup-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.264462 netbox_config_backup-1.4.3/netbox_config_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.264462 netbox_config_backup-1.4.3/netbox_config_backup/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.264462 netbox_config_backup-1.4.3/netbox_config_backup/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/management/commands/enqueue_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/management/commands/fix_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/management/commands/rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/management/commands/runbackup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/netbox_config_backup/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0002_git_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0003_primary_model_to_bigid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0004_custom_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0005_commit_add_time_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0008_backupjob_scheduled_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0010_backup_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0011_alter_backup_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/0012_backup_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/netbox_config_backup/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/models/backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/models/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.260462 netbox_config_backup-1.4.3/netbox_config_backup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/backup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/backups.html
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/diff.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/inc/backup_tables.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/repository.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/netbox_config_backup/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/templatetags/ncb_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/netbox_config_backup/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/utils/backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/utils/rq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/netbox_config_backup/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:55.264462 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-09 15:10:55.000000 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-09 15:10:55.000000 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:10:55.000000 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:10:55.000000 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 15:10:55.000000 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 15:10:55.000000 netbox_config_backup-1.4.3/netbox_config_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 15:10:55.268462 netbox_config_backup-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-09 15:10:47.000000 netbox_config_backup-1.4.3/setup.py
```

### Comparing `netbox_config_backup-1.4.2/LICENSE` & `netbox_config_backup-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/PKG-INFO` & `netbox_config_backup-1.4.3/netbox_config_backup.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: netbox_config_backup
-Version: 1.4.2
+Name: netbox-config-backup
+Version: 1.4.3
 Summary: NetBox Configuration Backup
 Home-page: https://github.com/dansheps/netbox-config-backup/
 Download-URL: https://github.com/dansheps/netbox-config-backup/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox_config_backup-1.4.2/README.md` & `netbox_config_backup-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/__init__.py` & `netbox_config_backup-1.4.3/netbox_config_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/choices.py` & `netbox_config_backup-1.4.3/netbox_config_backup/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/filtersets.py` & `netbox_config_backup-1.4.3/netbox_config_backup/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/forms.py` & `netbox_config_backup-1.4.3/netbox_config_backup/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/git.py` & `netbox_config_backup-1.4.3/netbox_config_backup/git.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/management/commands/fix_missing.py` & `netbox_config_backup-1.4.3/netbox_config_backup/management/commands/fix_missing.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/management/commands/rebuild.py` & `netbox_config_backup-1.4.3/netbox_config_backup/management/commands/rebuild.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/management/commands/runbackup.py` & `netbox_config_backup-1.4.3/netbox_config_backup/management/commands/runbackup.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/migrations/0001_initial.py` & `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/migrations/0002_git_models.py` & `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0002_git_models.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/migrations/0003_primary_model_to_bigid.py` & `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0003_primary_model_to_bigid.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py` & `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py` & `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py` & `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/migrations/0010_backup_ip.py` & `netbox_config_backup-1.4.3/netbox_config_backup/migrations/0010_backup_ip.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/models/backups.py` & `netbox_config_backup-1.4.3/netbox_config_backup/models/backups.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/models/jobs.py` & `netbox_config_backup-1.4.3/netbox_config_backup/models/jobs.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/navigation.py` & `netbox_config_backup-1.4.3/netbox_config_backup/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/tables.py` & `netbox_config_backup-1.4.3/netbox_config_backup/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/tasks.py` & `netbox_config_backup-1.4.3/netbox_config_backup/tasks.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/template_content.py` & `netbox_config_backup-1.4.3/netbox_config_backup/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/backup.html` & `netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/backup.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'netbox_config_backup/base.html' %}
+{% extends 'generic/object.html' %}
 {% load helpers %}
 
 {% block subtitle %}
   <div class="object-subtitle"></div>
 {% endblock %}
 
 {% block content %}
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
-{% extends 'netbox_config_backup/base.html' %} {% load helpers %} {% block
-subtitle %}
+{% extends 'generic/object.html' %} {% load helpers %} {% block subtitle %}
 {% endblock %} {% block content %}
 ** Backup Attributes **
 Name       {{ object.name|placeholder }}
 UUID       {{ object.uuid }}
 Device     {{_object.device|placeholder_}} {{ object.device|placeholder }}
 IP Address {{_object.ip|placeholder_}}     {{ object.ip|placeholder }}
 ** Status **
```

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/backups.html` & `netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/backups.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'netbox_config_backup/base.html' %}
+{% extends 'generic/object.html' %}
 {% load helpers %}
 
 {% block subtitle %}
   <div class="object-subtitle"></div>
 {% endblock %}
 
 {%  block extra_controls %}
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
-{% extends 'netbox_config_backup/base.html' %} {% load helpers %} {% block
-subtitle %}
+{% extends 'generic/object.html' %} {% load helpers %} {% block subtitle %}
 {% endblock %} {% block extra_controls %}
 Show_Startup Show_Running Show_All
 {% endblock %} {% block content %} {% include 'inc/table_controls_htmx.html'
 with table_modal="BackupsTable_config" %}
 {% include 'htmx/table.html' %}
 {% endblock %} {% block modals %} {{ block.super }} {% table_config_form table
 %} {% endblock modals %}
```

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/templates/netbox_config_backup/diff.html` & `netbox_config_backup-1.4.3/netbox_config_backup/templates/netbox_config_backup/diff.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'netbox_config_backup/base.html' %}
+{% extends 'generic/object.html' %}
 {% load helpers %}
 
 {% block subtitle %}
   <div class="object-subtitle">
     <span>{{ current.commit.time }}</span>
     <span class="separator">&middot;&middot;&middot;</span>
     <span>{{ previous.commit.time }}</span>
```

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/urls.py` & `netbox_config_backup-1.4.3/netbox_config_backup/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/utils/backups.py` & `netbox_config_backup-1.4.3/netbox_config_backup/utils/backups.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/utils/git.py` & `netbox_config_backup-1.4.3/netbox_config_backup/utils/git.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/utils/rq.py` & `netbox_config_backup-1.4.3/netbox_config_backup/utils/rq.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup/views.py` & `netbox_config_backup-1.4.3/netbox_config_backup/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,14 +158,15 @@
                 previous = backup.changes.filter(file__type=current.file.type, commit__time__lt=current.commit.time).\
                     last()
             except:
                 pass
 
         return render(request, 'netbox_config_backup/config.html', {
             'object': backup,
+            'tab': self.tab,
             'backup_config': config,
             'current': current,
             'previous': previous,
             'active_tab': 'config',
         })
 
 
@@ -173,15 +174,15 @@
 class DiffView(ObjectView):
     queryset = Backup.objects.all()
     template_name = 'netbox_config_backup/diff.html'
     tab = ViewTab(
         label='Diff',
     )
 
-    def get(self, request, pk, current, previous=None):
+    def get(self, request, pk, current=None, previous=None):
         backup = get_object_or_404(Backup.objects.all(), pk=pk)
         if current:
             current = get_object_or_404(BackupCommitTreeChange.objects.all(), pk=current)
         else:
             current = BackupCommitTreeChange.objects.filter(backup=backup, file__isnull=False).last()
             if not current:
                 raise Http404(
@@ -219,12 +220,13 @@
             diff = differ.compare()
 
         for idx, line in enumerate(diff):
             diff[idx] = line.rstrip()
 
         return render(request, 'netbox_config_backup/diff.html', {
             'object': backup,
+            'tab': self.tab,
             'diff': diff,
             'current': current,
             'previous': previous,
             'active_tab': 'diff',
         })
```

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup.egg-info/PKG-INFO` & `netbox_config_backup-1.4.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: netbox-config-backup
-Version: 1.4.2
+Name: netbox_config_backup
+Version: 1.4.3
 Summary: NetBox Configuration Backup
 Home-page: https://github.com/dansheps/netbox-config-backup/
 Download-URL: https://github.com/dansheps/netbox-config-backup/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox_config_backup-1.4.2/netbox_config_backup.egg-info/SOURCES.txt` & `netbox_config_backup-1.4.3/netbox_config_backup.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -41,19 +41,17 @@
 netbox_config_backup/migrations/__init__.py
 netbox_config_backup/models/__init__.py
 netbox_config_backup/models/abstract.py
 netbox_config_backup/models/backups.py
 netbox_config_backup/models/jobs.py
 netbox_config_backup/templates/netbox_config_backup/backup.html
 netbox_config_backup/templates/netbox_config_backup/backups.html
-netbox_config_backup/templates/netbox_config_backup/base.html
 netbox_config_backup/templates/netbox_config_backup/config.html
 netbox_config_backup/templates/netbox_config_backup/diff.html
 netbox_config_backup/templates/netbox_config_backup/repository.html
 netbox_config_backup/templates/netbox_config_backup/inc/backup_tables.html
-netbox_config_backup/templates/netbox_config_backup/switch_templates/cisco_iosxe/interface.tpl
 netbox_config_backup/templatetags/__init__.py
 netbox_config_backup/templatetags/ncb_split.py
 netbox_config_backup/utils/__init__.py
 netbox_config_backup/utils/backups.py
 netbox_config_backup/utils/git.py
 netbox_config_backup/utils/rq.py
```

### Comparing `netbox_config_backup-1.4.2/setup.py` & `netbox_config_backup-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox_config_backup',
-    version='1.4.2',
+    version='1.4.3',
     description='NetBox Configuration Backup',
     long_description='Plugin to backup device configuration',
     url='https://github.com/dansheps/netbox-config-backup/',
     download_url='https://github.com/dansheps/netbox-config-backup/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     maintainer='Daniel Sheppard',
```

