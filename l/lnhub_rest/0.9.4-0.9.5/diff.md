# Comparing `tmp/lnhub_rest-0.9.4.tar.gz` & `tmp/lnhub_rest-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnhub_rest-0.9.4.tar", last modified: Fri Apr 28 05:43:15 2023, max compression
+gzip compressed data, was "lnhub_rest-0.9.5.tar", last modified: Tue May  9 18:05:44 2023, max compression
```

## Comparing `lnhub_rest-0.9.4.tar` & `lnhub_rest-0.9.5.tar`

### file list

```diff
@@ -1,123 +1,201 @@
--rw-r--r--   0        0        0     1259 2023-01-16 08:48:49.546491 lnhub_rest-0.9.4/.dockerignore
--rw-r--r--   0        0        0     3245 2023-04-27 14:20:20.508469 lnhub_rest-0.9.4/.github/workflows/build.yml
--rw-r--r--   0        0        0     5044 2023-04-27 14:20:20.508591 lnhub_rest-0.9.4/.github/workflows/google-cloudrun-docker-prod.yml
--rw-r--r--   0        0        0     5050 2023-04-27 14:20:20.508674 lnhub_rest-0.9.4/.github/workflows/google-cloudrun-docker-staging.yml
--rw-r--r--   0        0        0      133 2023-01-16 08:48:49.546736 lnhub_rest-0.9.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      613 2023-03-09 06:06:53.745806 lnhub_rest-0.9.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1212 2023-03-09 06:06:53.745981 lnhub_rest-0.9.4/.gitignore
--rw-r--r--   0        0        0       73 2023-04-27 14:20:20.508759 lnhub_rest-0.9.4/.gitmodules
--rw-r--r--   0        0        0     1772 2023-02-16 17:07:29.911838 lnhub_rest-0.9.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      157 2023-04-27 14:20:20.508900 lnhub_rest-0.9.4/Dockerfile
--rw-r--r--   0        0        0     2442 2023-04-27 14:20:20.509044 lnhub_rest-0.9.4/README.md
--rw-r--r--   0        0        0     1680 2023-04-27 14:20:20.509168 lnhub_rest-0.9.4/docs/00-migrate.ipynb
--rw-r--r--   0        0        0     1189 2023-04-27 14:20:20.509297 lnhub_rest-0.9.4/docs/01-checks/01-check-break-lndb.ipynb
--rw-r--r--   0        0        0     4487 2023-04-27 14:20:20.509548 lnhub_rest-0.9.4/docs/02-account/02-create-account.ipynb
--rw-r--r--   0        0        0     5566 2023-04-27 14:20:20.509748 lnhub_rest-0.9.4/docs/02-account/03-update-account.ipynb
--rw-r--r--   0        0        0     6111 2023-04-27 14:20:20.509880 lnhub_rest-0.9.4/docs/02-account/04-fetch-account.ipynb
--rw-r--r--   0        0        0     9088 2023-04-27 14:20:20.510008 lnhub_rest-0.9.4/docs/02-account/05-rls.ipynb
--rw-r--r--   0        0        0    11110 2023-04-27 14:20:20.510196 lnhub_rest-0.9.4/docs/03-instance/01-init-instance.ipynb
--rw-r--r--   0        0        0     5293 2023-04-27 14:20:20.510303 lnhub_rest-0.9.4/docs/03-instance/02-load-instance.ipynb
--rw-r--r--   0        0        0     6498 2023-04-27 14:20:20.510391 lnhub_rest-0.9.4/docs/03-instance/03-update-instance.ipynb
--rw-r--r--   0        0        0     8667 2023-04-27 14:20:20.510495 lnhub_rest-0.9.4/docs/03-instance/04-delete-instance.ipynb
--rw-r--r--   0        0        0     7001 2023-04-27 14:20:20.510650 lnhub_rest-0.9.4/docs/03-instance/05-fetch-instance.ipynb
--rw-r--r--   0        0        0    19423 2023-04-27 14:20:20.510749 lnhub_rest-0.9.4/docs/03-instance/06-rls.ipynb
--rw-r--r--   0        0        0     3990 2023-04-27 14:20:20.510943 lnhub_rest-0.9.4/docs/04-storage/01-add-storage.ipynb
--rw-r--r--   0        0        0     9837 2023-04-27 14:20:20.511038 lnhub_rest-0.9.4/docs/04-storage/02-rls.ipynb
--rw-r--r--   0        0        0     3894 2023-04-27 14:20:20.511194 lnhub_rest-0.9.4/docs/05-organization/01-create-organization.ipynb
--rw-r--r--   0        0        0     4749 2023-04-27 14:20:20.511278 lnhub_rest-0.9.4/docs/05-organization/02-manage-members.ipynb
--rw-r--r--   0        0        0     5892 2023-04-27 14:20:20.511366 lnhub_rest-0.9.4/docs/05-organization/03-rls.ipynb
--rw-r--r--   0        0        0     5310 2023-04-27 14:20:20.511490 lnhub_rest-0.9.4/docs/06-integration/01-signup-signin.ipynb
--rw-r--r--   0        0        0      125 2023-04-27 14:20:20.511564 lnhub_rest-0.9.4/docs/README.md
--rw-r--r--   0        0        0    23977 2023-04-28 05:42:32.971886 lnhub_rest-0.9.4/docs/changelog.md
--rw-r--r--   0        0        0      520 2023-02-16 17:07:29.912882 lnhub_rest-0.9.4/docs/migrations.md
--rw-r--r--   0        0        0      162 2023-02-24 08:00:13.149505 lnhub_rest-0.9.4/docs/notes/index.md
--rw-r--r--   0        0        0    26418 2023-04-27 14:20:20.512036 lnhub_rest-0.9.4/docs/notes/multiple-sign-ups-same-email.ipynb
--rw-r--r--   0        0        0      137 2023-01-16 08:48:49.547929 lnhub_rest-0.9.4/lamin-project.yaml
-drwxr-xr-x   0        0        0        0 2023-04-27 14:20:20.512093 lnhub_rest-0.9.4/lndb/
--rw-r--r--   0        0        0      157 2023-04-28 05:42:22.067027 lnhub_rest-0.9.4/lnhub_rest/__init__.py
--rw-r--r--   0        0        0     7054 2023-04-27 14:20:20.512509 lnhub_rest-0.9.4/lnhub_rest/__main__.py
--rw-r--r--   0        0        0       64 2023-01-16 08:48:49.548569 lnhub_rest-0.9.4/lnhub_rest/_assets/__init__.py
--rw-r--r--   0        0        0     1026 2023-01-16 08:48:49.548656 lnhub_rest-0.9.4/lnhub_rest/_assets/_instances.py
--rw-r--r--   0        0        0     1109 2023-04-28 05:42:18.166663 lnhub_rest-0.9.4/lnhub_rest/_assets/_schemas.py
--rw-r--r--   0        0        0     1722 2023-04-27 14:20:20.512832 lnhub_rest-0.9.4/lnhub_rest/_check_breaks_lndb.py
--rw-r--r--   0        0        0     1260 2023-04-27 14:20:20.512930 lnhub_rest-0.9.4/lnhub_rest/_ci.py
--rw-r--r--   0        0        0     5726 2023-04-27 14:20:20.513064 lnhub_rest-0.9.4/lnhub_rest/_clean_ci.py
--rw-r--r--   0        0        0     1620 2023-04-27 14:20:20.513152 lnhub_rest-0.9.4/lnhub_rest/config.py
--rw-r--r--   0        0        0       42 2023-03-09 06:06:53.751483 lnhub_rest-0.9.4/lnhub_rest/core/__init__.py
--rw-r--r--   0        0        0      285 2023-04-27 14:20:20.513315 lnhub_rest-0.9.4/lnhub_rest/core/account/__init__.py
--rw-r--r--   0        0        0     2542 2023-04-27 14:20:20.513464 lnhub_rest-0.9.4/lnhub_rest/core/account/_create_account.py
--rw-r--r--   0        0        0     1062 2023-03-09 06:06:53.751850 lnhub_rest-0.9.4/lnhub_rest/core/account/_crud.py
--rw-r--r--   0        0        0      739 2023-04-27 14:20:20.513609 lnhub_rest-0.9.4/lnhub_rest/core/account/_delete_account.py
--rw-r--r--   0        0        0     3325 2023-04-27 14:20:20.513759 lnhub_rest-0.9.4/lnhub_rest/core/account/_signup_signin.py
--rw-r--r--   0        0        0     1423 2023-04-27 14:20:20.513898 lnhub_rest-0.9.4/lnhub_rest/core/account/_update_account.py
--rw-r--r--   0        0        0       38 2023-03-09 06:06:53.752268 lnhub_rest-0.9.4/lnhub_rest/core/collaborator/__init__.py
--rw-r--r--   0        0        0     3056 2023-04-27 14:20:20.514053 lnhub_rest-0.9.4/lnhub_rest/core/collaborator/_crud.py
--rw-r--r--   0        0        0      243 2023-03-09 06:06:53.752582 lnhub_rest-0.9.4/lnhub_rest/core/instance/__init__.py
--rw-r--r--   0        0        0     1651 2023-03-09 06:06:53.752815 lnhub_rest-0.9.4/lnhub_rest/core/instance/_crud.py
--rw-r--r--   0        0        0     1284 2023-04-27 14:20:20.514234 lnhub_rest-0.9.4/lnhub_rest/core/instance/_delete_instance.py
--rw-r--r--   0        0        0     6096 2023-04-27 14:20:20.514380 lnhub_rest-0.9.4/lnhub_rest/core/instance/_init_instance.py
--rw-r--r--   0        0        0     1532 2023-04-27 14:20:20.514735 lnhub_rest-0.9.4/lnhub_rest/core/instance/_load_instance.py
--rw-r--r--   0        0        0     1067 2023-04-27 14:20:20.514991 lnhub_rest-0.9.4/lnhub_rest/core/instance/_update_instance.py
--rw-r--r--   0        0        0       32 2023-04-27 14:20:20.515128 lnhub_rest-0.9.4/lnhub_rest/core/member/__init__.py
--rw-r--r--   0        0        0     2078 2023-04-27 14:20:20.515226 lnhub_rest-0.9.4/lnhub_rest/core/member/_crud.py
--rw-r--r--   0        0        0       80 2023-03-09 06:06:53.753548 lnhub_rest-0.9.4/lnhub_rest/core/storage/__init__.py
--rw-r--r--   0        0        0     3230 2023-04-27 14:20:20.515413 lnhub_rest-0.9.4/lnhub_rest/core/storage/_add_storage.py
--rw-r--r--   0        0        0     1167 2023-03-09 06:06:53.753832 lnhub_rest-0.9.4/lnhub_rest/core/storage/_crud.py
--rw-r--r--   0        0        0      796 2023-04-27 14:20:20.515554 lnhub_rest-0.9.4/lnhub_rest/main.py
--rw-r--r--   0        0        0       39 2023-04-27 14:20:20.515699 lnhub_rest-0.9.4/lnhub_rest/orm/__init__.py
--rw-r--r--   0        0        0      199 2023-04-27 14:20:20.515824 lnhub_rest-0.9.4/lnhub_rest/orm/_engine.py
--rw-r--r--   0        0        0     1968 2023-04-27 14:20:20.515952 lnhub_rest-0.9.4/lnhub_rest/orm/_sbclient.py
--rw-r--r--   0        0        0      198 2023-04-27 14:20:20.516104 lnhub_rest-0.9.4/lnhub_rest/routers/__init__.py
--rw-r--r--   0        0        0     4661 2023-04-27 14:20:20.516335 lnhub_rest-0.9.4/lnhub_rest/routers/account.py
--rw-r--r--   0        0        0      538 2023-03-09 06:06:53.755603 lnhub_rest-0.9.4/lnhub_rest/routers/ci.py
--rw-r--r--   0        0        0      779 2023-04-27 14:20:20.516441 lnhub_rest-0.9.4/lnhub_rest/routers/collaborator.py
--rw-r--r--   0        0        0      408 2023-03-09 06:06:53.755690 lnhub_rest-0.9.4/lnhub_rest/routers/dev.py
--rw-r--r--   0        0        0     5233 2023-04-27 14:20:20.516574 lnhub_rest-0.9.4/lnhub_rest/routers/instance.py
--rw-r--r--   0        0        0     2617 2023-04-27 14:20:20.516648 lnhub_rest-0.9.4/lnhub_rest/routers/organization.py
--rw-r--r--   0        0        0     1074 2023-04-27 14:20:20.516796 lnhub_rest-0.9.4/lnhub_rest/routers/utils.py
--rw-r--r--   0        0        0      249 2023-04-27 14:20:20.516949 lnhub_rest-0.9.4/lnhub_rest/schema/__init__.py
--rw-r--r--   0        0        0     4986 2023-04-27 14:20:20.517208 lnhub_rest-0.9.4/lnhub_rest/schema/_core.py
--rw-r--r--   0        0        0      270 2023-02-16 17:07:29.915739 lnhub_rest-0.9.4/lnhub_rest/schema/_timestamps.py
--rw-r--r--   0        0        0      262 2023-04-27 14:20:20.517313 lnhub_rest-0.9.4/lnhub_rest/schema/_type.py
--rw-r--r--   0        0        0      252 2023-02-16 17:07:29.915822 lnhub_rest-0.9.4/lnhub_rest/schema/_users.py
--rw-r--r--   0        0        0     1079 2023-02-16 17:07:29.915914 lnhub_rest-0.9.4/lnhub_rest/schema/_versions.py
--rw-r--r--   0        0        0      674 2023-01-16 08:48:49.550548 lnhub_rest-0.9.4/lnhub_rest/schema/alembic.ini
--rw-r--r--   0        0        0       40 2023-04-27 14:20:20.517474 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/__init__.py
--rw-r--r--   0        0        0     6020 2023-04-27 14:20:20.517568 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/clone.py
--rw-r--r--   0        0        0     3033 2023-04-27 14:20:20.517730 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/env.py
--rw-r--r--   0        0        0     1193 2023-04-27 14:20:20.517901 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0     1319 2023-04-27 14:20:20.517994 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1667 2023-04-27 14:20:20.518079 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0       39 2023-04-27 14:20:20.518231 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/function/__init__.py
--rw-r--r--   0        0        0     3940 2023-04-27 14:20:20.518407 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0      639 2023-04-27 14:20:20.518512 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
--rw-r--r--   0        0        0      214 2023-04-27 14:20:20.518625 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
--rw-r--r--   0        0        0      192 2023-04-27 14:20:20.518738 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
--rw-r--r--   0        0        0     7619 2023-04-27 14:20:20.518836 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1408 2023-04-27 14:20:20.518930 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0      880 2023-04-27 14:20:20.519043 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
--rw-r--r--   0        0        0       33 2023-04-27 14:20:20.519134 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/rls/__init__.py
--rw-r--r--   0        0        0      542 2023-01-16 08:48:49.550884 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/script.py.mako
--rw-r--r--   0        0        0     5258 2023-04-27 14:20:20.519313 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/testing.py
--rw-r--r--   0        0        0     9882 2023-04-27 14:20:20.519455 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py
--rw-r--r--   0        0        0      624 2023-04-27 14:20:20.519586 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
--rw-r--r--   0        0        0      918 2023-04-27 14:20:20.519737 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
--rw-r--r--   0        0        0      575 2023-04-27 14:20:20.519839 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
--rw-r--r--   0        0        0      542 2023-04-27 14:20:20.519929 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
--rw-r--r--   0        0        0     1199 2023-04-27 14:20:20.520034 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
--rw-r--r--   0        0        0      733 2023-04-27 14:20:20.520142 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
--rw-r--r--   0        0        0     5143 2023-04-27 14:20:20.520241 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
--rw-r--r--   0        0        0      593 2023-04-27 14:20:20.520330 lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
--rw-r--r--   0        0        0       60 2023-02-16 17:07:29.916209 lnhub_rest-0.9.4/lnhub_rest/schema/versions.py
--rw-r--r--   0        0        0       13 2023-04-27 14:20:20.520500 lnhub_rest-0.9.4/lnhub_rest/utils/__init__.py
--rw-r--r--   0        0        0      212 2023-03-09 06:06:53.757073 lnhub_rest-0.9.4/lnhub_rest/utils/_access_token.py
--rw-r--r--   0        0        0      352 2023-04-27 14:20:20.520665 lnhub_rest-0.9.4/lnhub_rest/utils/_id.py
--rw-r--r--   0        0        0      109 2023-03-09 06:06:53.757269 lnhub_rest-0.9.4/lnhub_rest/utils/_query.py
--rw-r--r--   0        0        0     3820 2023-04-27 14:20:20.520861 lnhub_rest-0.9.4/lnhub_rest/utils/_test.py
--rw-r--r--   0        0        0     1714 2023-04-27 14:20:20.521147 lnhub_rest-0.9.4/noxfile.py
--rw-r--r--   0        0        0     1368 2023-04-27 14:20:20.521378 lnhub_rest-0.9.4/pyproject.toml
--rwxr-xr-x   0        0        0       29 2023-03-09 06:06:53.757786 lnhub_rest-0.9.4/scripts/run.sh
--rw-r--r--   0        0        0       27 2023-02-24 08:00:13.152586 lnhub_rest-0.9.4/supabase/.gitignore
--rw-r--r--   0        0        0     2548 2023-02-24 08:00:13.152659 lnhub_rest-0.9.4/supabase/config.toml
--rw-r--r--   0        0        0     1212 2023-04-27 14:20:20.521580 lnhub_rest-0.9.4/tests/test_notebooks.py
--rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 lnhub_rest-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1259 2023-02-13 09:20:16.808732 lnhub_rest-0.9.5/.dockerignore
+-rw-r--r--   0        0        0     3245 2023-05-09 07:39:52.841154 lnhub_rest-0.9.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0     5417 2023-05-09 17:53:52.208995 lnhub_rest-0.9.5/.github/workflows/google-cloudrun-docker-prod.yml
+-rw-r--r--   0        0        0     5426 2023-05-09 17:53:52.209379 lnhub_rest-0.9.5/.github/workflows/google-cloudrun-docker-staging.yml
+-rw-r--r--   0        0        0      133 2022-12-05 16:31:02.016205 lnhub_rest-0.9.5/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      613 2023-04-12 05:33:51.441718 lnhub_rest-0.9.5/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1218 2023-05-09 18:05:31.381362 lnhub_rest-0.9.5/.gitignore
+-rw-r--r--   0        0        0       73 2023-04-17 19:46:07.717815 lnhub_rest-0.9.5/.gitmodules
+-rw-r--r--   0        0        0     1772 2023-04-12 05:33:51.441994 lnhub_rest-0.9.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      157 2023-04-17 19:46:07.718176 lnhub_rest-0.9.5/Dockerfile
+-rw-r--r--   0        0        0     2442 2023-05-09 07:39:46.055717 lnhub_rest-0.9.5/README.md
+-rw-r--r--   0        0        0     1680 2023-05-09 07:39:46.056027 lnhub_rest-0.9.5/docs/00-migrate.ipynb
+-rw-r--r--   0        0        0     1189 2023-04-27 13:36:02.439632 lnhub_rest-0.9.5/docs/01-checks/01-check-break-lndb.ipynb
+-rw-r--r--   0        0        0     4487 2023-04-27 13:36:02.437074 lnhub_rest-0.9.5/docs/02-account/02-create-account.ipynb
+-rw-r--r--   0        0        0     5566 2023-04-27 13:36:02.439987 lnhub_rest-0.9.5/docs/02-account/03-update-account.ipynb
+-rw-r--r--   0        0        0     6111 2023-04-27 13:36:02.438644 lnhub_rest-0.9.5/docs/02-account/04-fetch-account.ipynb
+-rw-r--r--   0        0        0     9088 2023-04-27 13:36:02.438818 lnhub_rest-0.9.5/docs/02-account/05-rls.ipynb
+-rw-r--r--   0        0        0    11110 2023-05-09 17:53:43.462582 lnhub_rest-0.9.5/docs/03-instance/01-init-instance.ipynb
+-rw-r--r--   0        0        0     5293 2023-05-09 17:53:43.463166 lnhub_rest-0.9.5/docs/03-instance/02-load-instance.ipynb
+-rw-r--r--   0        0        0     6498 2023-04-27 13:36:02.438676 lnhub_rest-0.9.5/docs/03-instance/03-update-instance.ipynb
+-rw-r--r--   0        0        0     8667 2023-05-09 17:53:43.463571 lnhub_rest-0.9.5/docs/03-instance/04-delete-instance.ipynb
+-rw-r--r--   0        0        0     7001 2023-04-27 13:36:02.439957 lnhub_rest-0.9.5/docs/03-instance/05-fetch-instance.ipynb
+-rw-r--r--   0        0        0    19423 2023-04-27 13:36:02.438412 lnhub_rest-0.9.5/docs/03-instance/06-rls.ipynb
+-rw-r--r--   0        0        0     3990 2023-05-09 07:39:52.841652 lnhub_rest-0.9.5/docs/04-storage/01-add-storage.ipynb
+-rw-r--r--   0        0        0     9837 2023-04-27 13:36:02.440625 lnhub_rest-0.9.5/docs/04-storage/02-rls.ipynb
+-rw-r--r--   0        0        0     3894 2023-04-27 13:36:02.435445 lnhub_rest-0.9.5/docs/05-organization/01-create-organization.ipynb
+-rw-r--r--   0        0        0     4749 2023-04-27 13:36:02.437528 lnhub_rest-0.9.5/docs/05-organization/02-manage-members.ipynb
+-rw-r--r--   0        0        0     5892 2023-04-27 13:36:02.435543 lnhub_rest-0.9.5/docs/05-organization/03-rls.ipynb
+-rw-r--r--   0        0        0     5310 2023-05-09 17:53:43.464325 lnhub_rest-0.9.5/docs/06-integration/01-signup-signin.ipynb
+-rw-r--r--   0        0        0      125 2023-04-20 08:36:06.559940 lnhub_rest-0.9.5/docs/README.md
+-rw-r--r--   0        0        0    24448 2023-05-09 17:57:31.375947 lnhub_rest-0.9.5/docs/changelog.md
+-rw-r--r--   0        0        0      520 2023-04-12 05:33:51.446631 lnhub_rest-0.9.5/docs/migrations.md
+-rw-r--r--   0        0        0      162 2023-04-12 05:33:51.446714 lnhub_rest-0.9.5/docs/notes/index.md
+-rw-r--r--   0        0        0    26418 2023-04-12 05:33:51.447158 lnhub_rest-0.9.5/docs/notes/multiple-sign-ups-same-email.ipynb
+-rw-r--r--   0        0        0      137 2022-12-05 16:31:02.018378 lnhub_rest-0.9.5/lamin-project.yaml
+-rw-r--r--   0        0        0     3832 2023-04-12 15:45:55.670360 lnhub_rest-0.9.5/lndb/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-04-03 19:31:19.500521 lnhub_rest-0.9.5/lndb/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-04-03 19:31:19.500584 lnhub_rest-0.9.5/lndb/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-04-03 19:31:19.500654 lnhub_rest-0.9.5/lndb/.gitignore
+-rw-r--r--   0        0        0     1777 2023-04-24 10:07:43.479664 lnhub_rest-0.9.5/lndb/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-04-03 19:31:19.500812 lnhub_rest-0.9.5/lndb/LICENSE
+-rw-r--r--   0        0        0      173 2023-04-03 19:31:19.500865 lnhub_rest-0.9.5/lndb/README.md
+-rw-r--r--   0        0        0       52 2023-04-03 19:31:19.500947 lnhub_rest-0.9.5/lndb/docs/api.md
+-rw-r--r--   0        0        0    48486 2023-05-09 07:19:55.937616 lnhub_rest-0.9.5/lndb/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-04-03 19:31:19.501245 lnhub_rest-0.9.5/lndb/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-04-03 19:31:19.501331 lnhub_rest-0.9.5/lndb/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-04-03 19:31:19.501425 lnhub_rest-0.9.5/lndb/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-04-03 19:31:19.501475 lnhub_rest-0.9.5/lndb/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-04-24 10:07:43.480335 lnhub_rest-0.9.5/lndb/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-04-03 19:31:19.501612 lnhub_rest-0.9.5/lndb/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-12 15:45:55.670784 lnhub_rest-0.9.5/lndb/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-12 15:45:55.670929 lnhub_rest-0.9.5/lndb/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-04-03 19:31:19.501804 lnhub_rest-0.9.5/lndb/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    10238 2023-05-09 07:19:55.937971 lnhub_rest-0.9.5/lndb/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     6419 2023-05-09 07:19:55.938294 lnhub_rest-0.9.5/lndb/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     6390 2023-04-24 10:07:43.480795 lnhub_rest-0.9.5/lndb/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3746 2023-04-24 11:38:30.442472 lnhub_rest-0.9.5/lndb/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-04-03 19:31:19.502118 lnhub_rest-0.9.5/lndb/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     2689 2023-04-20 09:03:40.403720 lnhub_rest-0.9.5/lndb/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-04-03 19:31:19.502231 lnhub_rest-0.9.5/lndb/docs/guide/index.md
+-rw-r--r--   0        0        0     3158 2023-04-24 10:07:43.480911 lnhub_rest-0.9.5/lndb/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-04-03 19:31:19.502354 lnhub_rest-0.9.5/lndb/docs/index.md
+-rw-r--r--   0        0        0      118 2023-04-03 19:31:19.502412 lnhub_rest-0.9.5/lndb/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-05-09 07:19:55.938487 lnhub_rest-0.9.5/lndb/lndb/__init__.py
+-rw-r--r--   0        0        0     4697 2023-05-09 07:19:55.938696 lnhub_rest-0.9.5/lndb/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-04-03 19:31:19.502658 lnhub_rest-0.9.5/lndb/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-12 15:45:55.671219 lnhub_rest-0.9.5/lndb/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-05-09 07:19:55.938851 lnhub_rest-0.9.5/lndb/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-12 15:45:55.671337 lnhub_rest-0.9.5/lndb/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-12 15:45:55.671440 lnhub_rest-0.9.5/lndb/lndb/_delete.py
+-rw-r--r--   0        0        0      329 2023-05-09 07:19:55.939671 lnhub_rest-0.9.5/lndb/lndb/_info.py
+-rw-r--r--   0        0        0     6035 2023-05-09 07:19:55.940140 lnhub_rest-0.9.5/lndb/lndb/_init_instance.py
+-rw-r--r--   0        0        0     6729 2023-05-09 07:19:55.941058 lnhub_rest-0.9.5/lndb/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-12 15:45:55.671792 lnhub_rest-0.9.5/lndb/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-12 15:45:55.671882 lnhub_rest-0.9.5/lndb/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-05-09 07:19:55.941325 lnhub_rest-0.9.5/lndb/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7644 2023-04-24 10:07:43.481621 lnhub_rest-0.9.5/lndb/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-04-03 19:31:19.503530 lnhub_rest-0.9.5/lndb/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      334 2023-05-09 07:19:55.941760 lnhub_rest-0.9.5/lndb/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-12 15:45:55.672114 lnhub_rest-0.9.5/lndb/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      803 2023-05-09 07:19:55.941979 lnhub_rest-0.9.5/lndb/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-04-03 19:31:19.503661 lnhub_rest-0.9.5/lndb/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-04-24 10:07:43.481783 lnhub_rest-0.9.5/lndb/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-20 09:03:40.405705 lnhub_rest-0.9.5/lndb/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-04-03 19:31:19.503836 lnhub_rest-0.9.5/lndb/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-04-03 19:31:19.503900 lnhub_rest-0.9.5/lndb/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3902 2023-04-24 10:07:43.481896 lnhub_rest-0.9.5/lndb/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-12 15:45:55.673128 lnhub_rest-0.9.5/lndb/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-04-03 19:31:19.504115 lnhub_rest-0.9.5/lndb/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-12 15:45:55.673226 lnhub_rest-0.9.5/lndb/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-04-03 19:31:19.504235 lnhub_rest-0.9.5/lndb/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-04-03 19:31:19.504287 lnhub_rest-0.9.5/lndb/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-12 15:45:55.673326 lnhub_rest-0.9.5/lndb/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8946 2023-05-09 07:19:55.942199 lnhub_rest-0.9.5/lndb/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-04-03 19:31:19.504528 lnhub_rest-0.9.5/lndb/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-04-03 19:31:19.504583 lnhub_rest-0.9.5/lndb/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-12 15:45:55.673539 lnhub_rest-0.9.5/lndb/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-04-03 19:31:19.504686 lnhub_rest-0.9.5/lndb/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-04-03 19:31:19.504753 lnhub_rest-0.9.5/lndb/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     7204 2023-04-24 10:07:43.482241 lnhub_rest-0.9.5/lndb/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5288 2023-04-24 10:07:43.482348 lnhub_rest-0.9.5/lndb/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-04-03 19:31:19.504960 lnhub_rest-0.9.5/lndb/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-12 15:45:55.673699 lnhub_rest-0.9.5/lndb/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-12 15:45:55.673790 lnhub_rest-0.9.5/lndb/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-04-03 19:31:19.505138 lnhub_rest-0.9.5/lndb/lndb/test/_env.py
+-rw-r--r--   0        0        0     3911 2023-05-09 07:19:55.942579 lnhub_rest-0.9.5/lndb/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-12 15:45:55.673887 lnhub_rest-0.9.5/lndb/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-04-03 19:31:19.505348 lnhub_rest-0.9.5/lndb/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-04-03 19:31:19.505408 lnhub_rest-0.9.5/lndb/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-12 15:45:55.673980 lnhub_rest-0.9.5/lndb/noxfile.py
+-rw-r--r--   0        0        0     1420 2023-05-09 07:19:55.942917 lnhub_rest-0.9.5/lndb/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-12 15:45:55.674169 lnhub_rest-0.9.5/lndb/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-04-03 19:31:19.505727 lnhub_rest-0.9.5/lndb/tests/test_init_instance.py
+-rw-r--r--   0        0        0      379 2023-05-09 07:19:55.943086 lnhub_rest-0.9.5/lndb/tests/test_notebooks.py
+-rw-r--r--   0        0        0      157 2023-05-09 17:57:24.110901 lnhub_rest-0.9.5/lnhub_rest/__init__.py
+-rw-r--r--   0        0        0     7054 2023-05-09 07:39:46.057772 lnhub_rest-0.9.5/lnhub_rest/__main__.py
+-rw-r--r--   0        0        0       64 2023-02-13 09:20:16.812158 lnhub_rest-0.9.5/lnhub_rest/_assets/__init__.py
+-rw-r--r--   0        0        0     1026 2023-02-13 09:20:16.812240 lnhub_rest-0.9.5/lnhub_rest/_assets/_instances.py
+-rw-r--r--   0        0        0     1109 2023-05-09 17:30:50.125171 lnhub_rest-0.9.5/lnhub_rest/_assets/_schemas.py
+-rw-r--r--   0        0        0     1722 2023-04-19 06:39:29.557169 lnhub_rest-0.9.5/lnhub_rest/_check_breaks_lndb.py
+-rw-r--r--   0        0        0     1260 2023-05-09 07:39:46.057997 lnhub_rest-0.9.5/lnhub_rest/_ci.py
+-rw-r--r--   0        0        0     5726 2023-05-09 17:53:43.464877 lnhub_rest-0.9.5/lnhub_rest/_clean_ci.py
+-rw-r--r--   0        0        0     1620 2023-05-09 07:39:46.058080 lnhub_rest-0.9.5/lnhub_rest/config.py
+-rw-r--r--   0        0        0       42 2023-04-12 05:33:51.449892 lnhub_rest-0.9.5/lnhub_rest/core/__init__.py
+-rw-r--r--   0        0        0      285 2023-04-17 19:46:07.724724 lnhub_rest-0.9.5/lnhub_rest/core/account/__init__.py
+-rw-r--r--   0        0        0     2542 2023-04-23 14:15:16.131687 lnhub_rest-0.9.5/lnhub_rest/core/account/_create_account.py
+-rw-r--r--   0        0        0     1062 2023-04-12 05:33:51.450294 lnhub_rest-0.9.5/lnhub_rest/core/account/_crud.py
+-rw-r--r--   0        0        0      739 2023-04-20 08:36:06.562096 lnhub_rest-0.9.5/lnhub_rest/core/account/_delete_account.py
+-rw-r--r--   0        0        0     3325 2023-05-09 17:53:43.465516 lnhub_rest-0.9.5/lnhub_rest/core/account/_signup_signin.py
+-rw-r--r--   0        0        0     1423 2023-04-20 08:36:06.562595 lnhub_rest-0.9.5/lnhub_rest/core/account/_update_account.py
+-rw-r--r--   0        0        0       38 2023-04-12 05:33:51.451054 lnhub_rest-0.9.5/lnhub_rest/core/collaborator/__init__.py
+-rw-r--r--   0        0        0     3056 2023-04-24 12:41:04.298412 lnhub_rest-0.9.5/lnhub_rest/core/collaborator/_crud.py
+-rw-r--r--   0        0        0      243 2023-04-12 05:33:51.451365 lnhub_rest-0.9.5/lnhub_rest/core/instance/__init__.py
+-rw-r--r--   0        0        0     1651 2023-04-12 05:33:51.451441 lnhub_rest-0.9.5/lnhub_rest/core/instance/_crud.py
+-rw-r--r--   0        0        0     1284 2023-04-20 08:36:06.563067 lnhub_rest-0.9.5/lnhub_rest/core/instance/_delete_instance.py
+-rw-r--r--   0        0        0     6096 2023-05-09 07:39:52.843001 lnhub_rest-0.9.5/lnhub_rest/core/instance/_init_instance.py
+-rw-r--r--   0        0        0     1532 2023-04-20 08:36:06.563609 lnhub_rest-0.9.5/lnhub_rest/core/instance/_load_instance.py
+-rw-r--r--   0        0        0     1067 2023-04-20 08:36:06.563842 lnhub_rest-0.9.5/lnhub_rest/core/instance/_update_instance.py
+-rw-r--r--   0        0        0       32 2023-04-17 19:46:07.726669 lnhub_rest-0.9.5/lnhub_rest/core/member/__init__.py
+-rw-r--r--   0        0        0     2078 2023-04-17 19:46:07.726929 lnhub_rest-0.9.5/lnhub_rest/core/member/_crud.py
+-rw-r--r--   0        0        0       80 2023-04-12 05:33:51.452504 lnhub_rest-0.9.5/lnhub_rest/core/storage/__init__.py
+-rw-r--r--   0        0        0     3230 2023-05-09 07:39:52.843396 lnhub_rest-0.9.5/lnhub_rest/core/storage/_add_storage.py
+-rw-r--r--   0        0        0     1167 2023-04-12 05:33:51.452880 lnhub_rest-0.9.5/lnhub_rest/core/storage/_crud.py
+-rw-r--r--   0        0        0      849 2023-05-09 17:53:52.209990 lnhub_rest-0.9.5/lnhub_rest/main.py
+-rw-r--r--   0        0        0       39 2023-04-20 08:36:06.564287 lnhub_rest-0.9.5/lnhub_rest/orm/__init__.py
+-rw-r--r--   0        0        0      199 2023-05-09 07:39:46.058791 lnhub_rest-0.9.5/lnhub_rest/orm/_engine.py
+-rw-r--r--   0        0        0     1968 2023-05-09 17:53:43.466525 lnhub_rest-0.9.5/lnhub_rest/orm/_sbclient.py
+-rw-r--r--   0        0        0      239 2023-05-09 17:53:52.210262 lnhub_rest-0.9.5/lnhub_rest/routers/__init__.py
+-rw-r--r--   0        0        0     4661 2023-04-24 12:41:04.298691 lnhub_rest-0.9.5/lnhub_rest/routers/account.py
+-rw-r--r--   0        0        0      538 2023-05-09 17:53:43.467343 lnhub_rest-0.9.5/lnhub_rest/routers/ci.py
+-rw-r--r--   0        0        0     2313 2023-05-09 17:53:52.210493 lnhub_rest-0.9.5/lnhub_rest/routers/collaborator.py
+-rw-r--r--   0        0        0      408 2023-04-12 05:33:51.454427 lnhub_rest-0.9.5/lnhub_rest/routers/dev.py
+-rw-r--r--   0        0        0     5233 2023-04-24 12:41:04.298930 lnhub_rest-0.9.5/lnhub_rest/routers/instance.py
+-rw-r--r--   0        0        0     2617 2023-04-17 19:46:07.729123 lnhub_rest-0.9.5/lnhub_rest/routers/organization.py
+-rw-r--r--   0        0        0     1074 2023-04-20 08:36:06.565374 lnhub_rest-0.9.5/lnhub_rest/routers/utils.py
+-rw-r--r--   0        0        0      249 2023-04-19 06:39:29.557427 lnhub_rest-0.9.5/lnhub_rest/schema/__init__.py
+-rw-r--r--   0        0        0     4986 2023-04-17 19:46:07.730209 lnhub_rest-0.9.5/lnhub_rest/schema/_core.py
+-rw-r--r--   0        0        0      270 2023-03-02 11:17:31.752043 lnhub_rest-0.9.5/lnhub_rest/schema/_timestamps.py
+-rw-r--r--   0        0        0      262 2023-04-17 19:46:07.730671 lnhub_rest-0.9.5/lnhub_rest/schema/_type.py
+-rw-r--r--   0        0        0      252 2023-03-02 11:17:31.752112 lnhub_rest-0.9.5/lnhub_rest/schema/_users.py
+-rw-r--r--   0        0        0     1079 2023-04-12 05:33:51.456009 lnhub_rest-0.9.5/lnhub_rest/schema/_versions.py
+-rw-r--r--   0        0        0      674 2023-02-13 09:20:16.814087 lnhub_rest-0.9.5/lnhub_rest/schema/alembic.ini
+-rw-r--r--   0        0        0       40 2023-05-09 07:39:46.059338 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/__init__.py
+-rw-r--r--   0        0        0     6020 2023-04-17 19:46:07.731439 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/clone.py
+-rw-r--r--   0        0        0     3033 2023-05-09 07:39:46.059588 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/env.py
+-rw-r--r--   0        0        0     1193 2023-04-12 05:33:51.456564 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0     1319 2023-04-17 19:46:07.731951 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1667 2023-04-17 19:46:07.732205 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0       39 2023-04-12 05:33:51.457356 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/function/__init__.py
+-rw-r--r--   0        0        0     3940 2023-04-12 05:33:51.457588 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0      639 2023-04-12 05:33:51.457841 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
+-rw-r--r--   0        0        0      214 2023-04-17 19:46:07.732575 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
+-rw-r--r--   0        0        0      192 2023-04-17 19:46:07.732918 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
+-rw-r--r--   0        0        0     7619 2023-04-17 19:46:07.733294 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1408 2023-04-17 19:46:07.733539 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0      880 2023-04-19 06:39:29.557590 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
+-rw-r--r--   0        0        0       33 2023-04-12 05:33:51.459308 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/rls/__init__.py
+-rw-r--r--   0        0        0      542 2023-02-13 09:20:16.814349 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/script.py.mako
+-rw-r--r--   0        0        0     5258 2023-05-09 07:39:46.059864 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/testing.py
+-rw-r--r--   0        0        0     9882 2023-04-20 08:36:06.566134 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py
+-rw-r--r--   0        0        0      624 2023-04-20 08:36:06.566367 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
+-rw-r--r--   0        0        0      918 2023-04-12 05:33:51.460064 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
+-rw-r--r--   0        0        0      575 2023-04-12 05:33:51.460238 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
+-rw-r--r--   0        0        0      542 2023-04-17 19:46:07.734101 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
+-rw-r--r--   0        0        0     1199 2023-04-17 19:46:07.734436 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
+-rw-r--r--   0        0        0      733 2023-04-17 19:46:07.734632 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
+-rw-r--r--   0        0        0     5143 2023-04-17 19:46:07.734875 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
+-rw-r--r--   0        0        0      593 2023-04-19 06:39:29.557744 lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
+-rw-r--r--   0        0        0       60 2023-03-02 11:17:31.752459 lnhub_rest-0.9.5/lnhub_rest/schema/versions.py
+-rw-r--r--   0        0        0       13 2023-04-17 19:46:07.735238 lnhub_rest-0.9.5/lnhub_rest/utils/__init__.py
+-rw-r--r--   0        0        0      212 2023-04-12 05:33:51.461642 lnhub_rest-0.9.5/lnhub_rest/utils/_access_token.py
+-rw-r--r--   0        0        0      352 2023-04-17 19:46:07.735507 lnhub_rest-0.9.5/lnhub_rest/utils/_id.py
+-rw-r--r--   0        0        0      109 2023-04-12 05:33:51.461902 lnhub_rest-0.9.5/lnhub_rest/utils/_query.py
+-rw-r--r--   0        0        0     3820 2023-04-20 08:36:06.566596 lnhub_rest-0.9.5/lnhub_rest/utils/_test.py
+-rw-r--r--   0        0        0     1714 2023-05-09 07:39:46.060173 lnhub_rest-0.9.5/noxfile.py
+-rw-r--r--   0        0        0     1368 2023-05-09 07:39:46.060392 lnhub_rest-0.9.5/pyproject.toml
+-rwxr-xr-x   0        0        0       29 2023-04-12 05:33:51.462685 lnhub_rest-0.9.5/scripts/run.sh
+-rw-r--r--   0        0        0       27 2023-04-12 05:33:51.462759 lnhub_rest-0.9.5/supabase/.gitignore
+-rw-r--r--   0        0        0     2548 2023-04-12 05:33:51.462840 lnhub_rest-0.9.5/supabase/config.toml
+-rw-r--r--   0        0        0     1212 2023-05-09 07:39:46.060630 lnhub_rest-0.9.5/tests/test_notebooks.py
+-rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 lnhub_rest-0.9.5/PKG-INFO
```

### Comparing `lnhub_rest-0.9.4/.dockerignore` & `lnhub_rest-0.9.5/.dockerignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/.github/workflows/build.yml` & `lnhub_rest-0.9.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/.github/workflows/google-cloudrun-docker-prod.yml` & `lnhub_rest-0.9.5/.github/workflows/google-cloudrun-docker-prod.yml`

 * *Files 12% similar despite different names*

```diff
@@ -101,19 +101,27 @@
       - name: Build and Push Container
         run: |-
           docker build -t "${{ env.GAR_LOCATION }}-docker.pkg.dev/${{ env.PROJECT_ID }}/${{ env.REPO_NAME }}/${{ env.SERVICE }}:${{ github.sha }}" ./
           docker push "${{ env.GAR_LOCATION }}-docker.pkg.dev/${{ env.PROJECT_ID }}/${{ env.REPO_NAME }}/${{ env.SERVICE }}:${{ github.sha }}"
 
       # END - Docker auth and build
 
+      - name: Setup environment variables
+        run: echo "${{secrets.LNHUB_REST_PROD_ENV}}" >> $GITHUB_ENV
+
       - name: Deploy to Cloud Run
         id: deploy
         uses: google-github-actions/deploy-cloudrun@v1
         with:
           service: lnhub-rest-cloud-run-main # ${{ env.SERVICE }}
           region: ${{ env.REGION }}
+          env_vars: |
+            SUPABASE_API_URL=${{ env.SUPABASE_API_URL }}
+            SUPABASE_SERVICE_KEY=${{ env.SUPABASE_SERVICE_KEY }}
+            SUPABASE_ANON_KEY=${{ env.SUPABASE_ANON_KEY }}
+            LNHUB_PG_PASSWORD=${{ env.LNHUB_PG_PASSWORD }}
           # NOTE: If using a pre-built image, update the image name here
           image: ${{ env.GAR_LOCATION }}-docker.pkg.dev/${{ env.PROJECT_ID }}/${{ env.REPO_NAME }}/lnhub-rest-cloud-run-main:${{ github.sha }}
 
       # If required, use the Cloud Run url output in later steps
       - name: Show Output
         run: echo ${{ steps.deploy.outputs.url }}
```

### Comparing `lnhub_rest-0.9.4/.github/workflows/google-cloudrun-docker-staging.yml` & `lnhub_rest-0.9.5/.github/workflows/google-cloudrun-docker-staging.yml`

 * *Files 7% similar despite different names*

```diff
@@ -101,19 +101,27 @@
       - name: Build and Push Container
         run: |-
           docker build -t "${{ env.GAR_LOCATION }}-docker.pkg.dev/${{ env.PROJECT_ID }}/${{ env.REPO_NAME }}/${{ env.SERVICE }}:${{ github.sha }}" ./
           docker push "${{ env.GAR_LOCATION }}-docker.pkg.dev/${{ env.PROJECT_ID }}/${{ env.REPO_NAME }}/${{ env.SERVICE }}:${{ github.sha }}"
 
       # END - Docker auth and build
 
+      - name: Setup environment variables
+        run: echo "${{secrets.LNHUB_REST_STAGING_ENV}}" >> $GITHUB_ENV
+
       - name: Deploy to Cloud Run
         id: deploy
         uses: google-github-actions/deploy-cloudrun@v1
         with:
           service: lnhub-rest-cloud-run-staging # ${{ env.SERVICE }}
           region: ${{ env.REGION }}
+          env_vars: |
+            SUPABASE_API_URL=${{ env.SUPABASE_API_URL }}
+            SUPABASE_SERVICE_KEY=${{ env.SUPABASE_SERVICE_KEY }}
+            SUPABASE_ANON_KEY=${{ env.SUPABASE_ANON_KEY }}
+            LNHUB_PG_PASSWORD=${{ env.LNHUB_PG_PASSWORD }}
           # NOTE: If using a pre-built image, update the image name here
           image: ${{ env.GAR_LOCATION }}-docker.pkg.dev/${{ env.PROJECT_ID }}/${{ env.REPO_NAME }}/lnhub-rest-cloud-run-staging:${{ github.sha }}
 
       # If required, use the Cloud Run url output in later steps
       - name: Show Output
         run: echo ${{ steps.deploy.outputs.url }}
```

### Comparing `lnhub_rest-0.9.4/.github/workflows/latest-changes.yml` & `lnhub_rest-0.9.5/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/.gitignore` & `lnhub_rest-0.9.5/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 celerybeat-schedule
 
 # SageMath parsed files
 *.sage.py
 
 # dotenv
 .env
+*.env
 
 # virtualenv
 .venv
 venv/
 ENV/
 
 # mypy
```

### Comparing `lnhub_rest-0.9.4/.pre-commit-config.yaml` & `lnhub_rest-0.9.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/README.md` & `lnhub_rest-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/00-migrate.ipynb` & `lnhub_rest-0.9.5/docs/00-migrate.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/01-checks/01-check-break-lndb.ipynb` & `lnhub_rest-0.9.5/docs/01-checks/01-check-break-lndb.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/02-account/02-create-account.ipynb` & `lnhub_rest-0.9.5/docs/02-account/02-create-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/02-account/03-update-account.ipynb` & `lnhub_rest-0.9.5/docs/02-account/03-update-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/02-account/04-fetch-account.ipynb` & `lnhub_rest-0.9.5/docs/02-account/04-fetch-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/02-account/05-rls.ipynb` & `lnhub_rest-0.9.5/docs/02-account/05-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/03-instance/01-init-instance.ipynb` & `lnhub_rest-0.9.5/docs/03-instance/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/03-instance/02-load-instance.ipynb` & `lnhub_rest-0.9.5/docs/03-instance/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/03-instance/03-update-instance.ipynb` & `lnhub_rest-0.9.5/docs/03-instance/03-update-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/03-instance/04-delete-instance.ipynb` & `lnhub_rest-0.9.5/docs/03-instance/04-delete-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/03-instance/05-fetch-instance.ipynb` & `lnhub_rest-0.9.5/docs/03-instance/05-fetch-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/03-instance/06-rls.ipynb` & `lnhub_rest-0.9.5/docs/03-instance/06-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/04-storage/01-add-storage.ipynb` & `lnhub_rest-0.9.5/docs/04-storage/01-add-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/04-storage/02-rls.ipynb` & `lnhub_rest-0.9.5/docs/04-storage/02-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/05-organization/01-create-organization.ipynb` & `lnhub_rest-0.9.5/docs/05-organization/01-create-organization.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/05-organization/02-manage-members.ipynb` & `lnhub_rest-0.9.5/docs/05-organization/02-manage-members.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/05-organization/03-rls.ipynb` & `lnhub_rest-0.9.5/docs/05-organization/03-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/06-integration/01-signup-signin.ipynb` & `lnhub_rest-0.9.5/docs/06-integration/01-signup-signin.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/changelog.md` & `lnhub_rest-0.9.5/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🔖 Staging version 0.9.5 | [199](https://github.com/laminlabs/lnhub-rest/pull/199) | [bpenteado](https://github.com/bpenteado) | 2023-05-09 | 0.9.5
+👷 Fix deployment in main branch | [201](https://github.com/laminlabs/lnhub-rest/pull/201) | [lawrlee](https://github.com/lawrlee) | 2023-05-09 |
+✨ Create endpoints to update and delete collaborators | [197](https://github.com/laminlabs/lnhub-rest/pull/197) | [bpenteado](https://github.com/bpenteado) | 2023-05-09 |
 🍱 Register trexbio schema | [195](https://github.com/laminlabs/lnhub-rest/pull/195) | [sunnyosun](https://github.com/sunnyosun) | 2023-04-28 | 0.9.4
 Remove build workflow when making a release | [193](https://github.com/laminlabs/lnhub-rest/pull/193) | [lawrlee](https://github.com/lawrlee) | 2023-04-27 |
 ✨ Allow local storage locations | [194](https://github.com/laminlabs/lnhub-rest/pull/194) | [falexwolf](https://github.com/falexwolf) | 2023-04-27 | 0.9.3
 ✨ Add `is_collaborator` endpoint | [191](https://github.com/laminlabs/lnhub-rest/pull/191) | [fredericenard](https://github.com/fredericenard) | 2023-04-25 | 0.9.2
 👷 Refactor environment management  | [180](https://github.com/laminlabs/lnhub-rest/pull/180) | [lawrlee](https://github.com/lawrlee) | 2023-04-24 |
 🔖 Staging version 0.9.0 | [170](https://github.com/laminlabs/lnhub-rest/pull/170) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.9.1
 🎨 Redesign acct-instances endpoint | [190](https://github.com/laminlabs/lnhub-rest/pull/190) | [bpenteado](https://github.com/bpenteado) | 2023-04-23 |
```

### Comparing `lnhub_rest-0.9.4/docs/migrations.md` & `lnhub_rest-0.9.5/docs/migrations.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/docs/notes/multiple-sign-ups-same-email.ipynb` & `lnhub_rest-0.9.5/docs/notes/multiple-sign-ups-same-email.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/__main__.py` & `lnhub_rest-0.9.5/lnhub_rest/__main__.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/_assets/_instances.py` & `lnhub_rest-0.9.5/lnhub_rest/_assets/_instances.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/_assets/_schemas.py` & `lnhub_rest-0.9.5/lnhub_rest/_assets/_schemas.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/_check_breaks_lndb.py` & `lnhub_rest-0.9.5/lnhub_rest/_check_breaks_lndb.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/_ci.py` & `lnhub_rest-0.9.5/lnhub_rest/_ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/_clean_ci.py` & `lnhub_rest-0.9.5/lnhub_rest/_clean_ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/config.py` & `lnhub_rest-0.9.5/lnhub_rest/config.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/account/_create_account.py` & `lnhub_rest-0.9.5/lnhub_rest/core/account/_create_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/account/_crud.py` & `lnhub_rest-0.9.5/lnhub_rest/core/account/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/account/_delete_account.py` & `lnhub_rest-0.9.5/lnhub_rest/core/account/_delete_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/account/_signup_signin.py` & `lnhub_rest-0.9.5/lnhub_rest/core/account/_signup_signin.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/account/_update_account.py` & `lnhub_rest-0.9.5/lnhub_rest/core/account/_update_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/collaborator/_crud.py` & `lnhub_rest-0.9.5/lnhub_rest/core/collaborator/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/instance/_crud.py` & `lnhub_rest-0.9.5/lnhub_rest/core/instance/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/instance/_delete_instance.py` & `lnhub_rest-0.9.5/lnhub_rest/core/instance/_delete_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/instance/_init_instance.py` & `lnhub_rest-0.9.5/lnhub_rest/core/instance/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/instance/_load_instance.py` & `lnhub_rest-0.9.5/lnhub_rest/core/instance/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/instance/_update_instance.py` & `lnhub_rest-0.9.5/lnhub_rest/core/instance/_update_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/member/_crud.py` & `lnhub_rest-0.9.5/lnhub_rest/core/member/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/storage/_add_storage.py` & `lnhub_rest-0.9.5/lnhub_rest/core/storage/_add_storage.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/core/storage/_crud.py` & `lnhub_rest-0.9.5/lnhub_rest/core/storage/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/main.py` & `lnhub_rest-0.9.5/lnhub_rest/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import uvicorn
 from fastapi import FastAPI
 from fastapi.testclient import TestClient
 from starlette.middleware.cors import CORSMiddleware
 
-from lnhub_rest.routers import account, ci, dev, instance, organization
+from lnhub_rest.routers import account, ci, collaborator, dev, instance, organization
 
 ROOT_PATH = "/" + os.getenv("ROOT_PATH", "")
 PORT = int(os.getenv("PORT", 8000))
 
 
 app = FastAPI(openapi_prefix=ROOT_PATH)
 
@@ -17,18 +17,18 @@
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
-
 app.include_router(ci.router)
 app.include_router(account.router)
 app.include_router(instance.router)
+app.include_router(collaborator.router)
 app.include_router(dev.router)
 app.include_router(organization.router)
 
 client = TestClient(app)
 
 if __name__ == "__main__":
     uvicorn.run("main:app", host="0.0.0.0", port=PORT, root_path=ROOT_PATH)
```

### Comparing `lnhub_rest-0.9.4/lnhub_rest/orm/_sbclient.py` & `lnhub_rest-0.9.5/lnhub_rest/orm/_sbclient.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/routers/account.py` & `lnhub_rest-0.9.5/lnhub_rest/routers/account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/routers/ci.py` & `lnhub_rest-0.9.5/lnhub_rest/routers/ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/routers/instance.py` & `lnhub_rest-0.9.5/lnhub_rest/routers/instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/routers/organization.py` & `lnhub_rest-0.9.5/lnhub_rest/routers/organization.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/routers/utils.py` & `lnhub_rest-0.9.5/lnhub_rest/routers/utils.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/_core.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/_core.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/_versions.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/_versions.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/alembic.ini` & `lnhub_rest-0.9.5/lnhub_rest/schema/alembic.ini`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/clone.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/clone.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/env.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/script.py.mako` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/testing.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/testing.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py` & `lnhub_rest-0.9.5/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/lnhub_rest/utils/_test.py` & `lnhub_rest-0.9.5/lnhub_rest/utils/_test.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/noxfile.py` & `lnhub_rest-0.9.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/pyproject.toml` & `lnhub_rest-0.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/supabase/config.toml` & `lnhub_rest-0.9.5/supabase/config.toml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/tests/test_notebooks.py` & `lnhub_rest-0.9.5/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.4/PKG-INFO` & `lnhub_rest-0.9.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnhub_rest
-Version: 0.9.4
+Version: 0.9.5
 Summary: Rest API for the hub.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lamin_logger>=0.2.3
 Requires-Dist: supabase==1.0.2
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
```

