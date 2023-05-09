# Comparing `tmp/pure_ocean_breeze-3.9.3.tar.gz` & `tmp/pure_ocean_breeze-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-3.9.3.tar", last modified: Mon Apr 24 06:46:14 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-3.9.4.tar", last modified: Tue May  9 07:52:53 2023, max compression
```

## Comparing `pure_ocean_breeze-3.9.3.tar` & `pure_ocean_breeze-3.9.4.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.968919 pure_ocean_breeze-3.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-24 06:46:14.968919 pure_ocean_breeze-3.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.948919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.948919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31550 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    29530 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    49960 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    49330 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.952919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.952919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.952919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   228179 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.952919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.952919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.952919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.952919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.952919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.956919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.956919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.956919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.956919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.956919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.960919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.960919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.960919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.960919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.960919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.960919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.960919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.964919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.964919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.964919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.964919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.964919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.968919 pure_ocean_breeze-3.9.3/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:46:14.948919 pure_ocean_breeze-3.9.3/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-24 06:46:14.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-24 06:46:14.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:46:14.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 06:46:14.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 06:46:14.000000 pure_ocean_breeze-3.9.3/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 06:46:14.968919 pure_ocean_breeze-3.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-24 06:45:58.000000 pure_ocean_breeze-3.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.188527 pure_ocean_breeze-3.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-09 07:52:53.188527 pure_ocean_breeze-3.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.176527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.176527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31550 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29552 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49960 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49330 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.176527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.176527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.176527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239812 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.188527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.176527 pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-09 07:52:53.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-09 07:52:53.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:52:53.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-09 07:52:53.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 07:52:53.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 07:52:53.188527 pure_ocean_breeze-3.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/setup.py
```

### Comparing `pure_ocean_breeze-3.9.3/LICENSE` & `pure_ocean_breeze-3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/PKG-INFO` & `pure_ocean_breeze-3.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 3.9.3
+Version: 3.9.4
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.3/README.md` & `pure_ocean_breeze-3.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-04-24 13:18:37"
-__version__ = "3.9.3"
+__updated__ = "2023-05-09 15:28:47"
+__version__ = "3.9.4"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/read_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-03-25 19:35:57"
+__updated__ = "2023-05-09 15:39:34"
 
 import os
 import numpy as np
 import pandas as pd
 import datetime
 from typing import Union, Dict, Tuple
 from loguru import logger
@@ -56,15 +56,15 @@
     stop_down: bool = 0,
     zxindustry_dummy_code: bool = 0,
     zxindustry_dummy_name: bool = 0,
     swindustry_dummy: bool = 0,
     hs300_member_weight: bool = 0,
     zz500_member_weight: bool = 0,
     zz1000_member_weight: bool = 0,
-    start: int = STATES["START"],
+    start: Union[int,str] = STATES["START"],
 ) -> pd.DataFrame:
     """直接读取常用的量价读取日频数据，默认为复权价格，
     在 open,close,high,low,tr,sharenum,volume 中选择一个参数指定为1
 
     Parameters
     ----------
     path : str, optional
@@ -145,15 +145,15 @@
         为1则表示读取申万一级行业哑变量, by default 0
     hs300_member_weight : bool, optional
         为1则表示读取沪深300成分股权重（月频）, by default 0
     zz500_member_weight : bool, optional
         为1则表示读取中证500成分股权重（月频）, by default 0
     zz1000_member_weight : bool, optional
         为1则表示读取中证1000成分股权重（月频）, by default 0
-    start : int, optional
+    start : Union[int,str], optional
         起始日期，形如20130101, by default STATES["START"]
 
     Returns
     -------
     `pd.DataFrame`
         一个columns为股票代码，index为时间，values为目标数据的pd.DataFrame
```

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/labor/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-04-24 14:42:09"
+__updated__ = "2023-05-09 15:46:45"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
@@ -22,23 +22,22 @@
 from dateutil.relativedelta import relativedelta
 from loguru import logger
 import datetime
 from collections.abc import Iterable
 import plotly.express as pe
 import plotly.io as pio
 from plotly.tools import FigureFactory as FF
-import plotly.graph_objects as go
-import plotly.tools as plyoo
 import pyfinance.ols as po
 from texttable import Texttable
 from xpinyin import Pinyin
 import tradetime as tt
 import cufflinks as cf
 import deprecation
 from mpire import WorkerPool
+from scipy.optimize import minimize
 from pure_ocean_breeze import __version__
 
 cf.set_config_file(offline=True)
 from typing import Callable, Union, Dict, List, Tuple
 from pure_ocean_breeze.data.read_data import (
     read_daily,
     read_market,
@@ -1505,14 +1504,15 @@
         ages: pd.DataFrame = None,
         sts: pd.DataFrame = None,
         states: pd.DataFrame = None,
         opens: pd.DataFrame = None,
         closes: pd.DataFrame = None,
         capitals: pd.DataFrame = None,
         opens_average_first_day: bool = 0,
+        total_cap: bool = 0,
     ):
         if ages is None:
             ages = read_daily(age=1, start=20100101)
         if sts is None:
             sts = read_daily(st=1, start=20100101)
         if states is None:
             states = read_daily(state=1, start=20100101)
@@ -1520,15 +1520,22 @@
             if opens_average_first_day:
                 opens = read_daily(vwap=1, start=20100101)
             else:
                 opens = read_daily(open=1, start=20100101)
         if closes is None:
             closes = read_daily(close=1, start=20100101)
         if capitals is None:
-            capitals = read_daily(flow_cap=1, start=20100101).resample(cls.freq).last()
+            if total_cap:
+                capitals = (
+                    read_daily(total_cap=1, start=20100101).resample(cls.freq).last()
+                )
+            else:
+                capitals = (
+                    read_daily(flow_cap=1, start=20100101).resample(cls.freq).last()
+                )
         # 上市天数文件
         cls.ages = ages
         # st日子标志文件
         cls.sts = sts.fillna(0)
         # cls.sts = 1 - cls.sts.fillna(0)
         # 交易状态文件
         cls.states = states
@@ -1930,51 +1937,66 @@
 
             def in_g(df):
                 df.cap_value = df.cap_value / df.cap_value.sum()
                 df.ret = df.ret * df.cap_value
                 return df.ret.sum()
 
             self.group_rets = self.data.groupby(["date", "group"]).apply(in_g)
-            self.rets_all=self.data.groupby(['date']).apply(in_g)
+            self.rets_all = self.data.groupby(["date"]).apply(in_g)
             self.group_rets_std = "市值加权暂未设置该功能，敬请期待🌙"
         else:
             self.group_rets = self.data.groupby(["date", "group"]).apply(
                 lambda x: x.ret.mean()
             )
-            self.rets_all=self.data.groupby(['date']).apply(lambda x:x.ret.mean())
+            self.rets_all = self.data.groupby(["date"]).apply(lambda x: x.ret.mean())
             self.group_rets_stds = self.data.groupby(["date", "group"]).apply(
                 lambda x: x.ret.std()
             )
             self.group_rets_std = self.group_rets_stds.groupby("group").mean()
         # dropna是因为如果股票行情数据比因子数据的截止日期晚，而最后一个月发生月初跌停时，会造成最后某组多出一个月的数据
         self.group_rets = self.group_rets.unstack()
         self.group_rets = self.group_rets[
             self.group_rets.index <= self.factors.date.max()
         ]
         self.group_rets.columns = list(map(str, list(self.group_rets.columns)))
         self.group_rets = self.group_rets.add_prefix("group")
         self.group_rets = (
             self.group_rets - self.factor_turnover_rates * trade_cost_double_side
         )
-        self.rets_all=self.rets_all-self.factor_turnover_rates.mean(axis=1)*trade_cost_double_side
+        self.rets_all = (
+            self.rets_all
+            - self.factor_turnover_rates.mean(axis=1) * trade_cost_double_side
+        )
         self.long_short_rets = (
             self.group_rets["group1"] - self.group_rets["group" + str(groups_num)]
         )
-        self.inner_rets_long=self.group_rets.group1-self.rets_all
-        self.inner_rets_short=self.rets_all-self.group_rets["group" + str(groups_num)]
-        self.long_short_net_values = self.make_start_to_one((self.long_short_rets + 1).cumprod())
+        self.inner_rets_long = self.group_rets.group1 - self.rets_all
+        self.inner_rets_short = (
+            self.rets_all - self.group_rets["group" + str(groups_num)]
+        )
+        self.long_short_net_values = self.make_start_to_one(
+            (self.long_short_rets + 1).cumprod()
+        )
         if self.long_short_net_values[-1] <= self.long_short_net_values[0]:
             self.long_short_rets = (
                 self.group_rets["group" + str(groups_num)] - self.group_rets["group1"]
             )
-            self.long_short_net_values = self.make_start_to_one((self.long_short_rets + 1).cumprod())
-            self.inner_rets_long=self.group_rets["group" + str(groups_num)]-self.rets_all
-            self.inner_rets_short=self.rets_all-self.group_rets.group1
-        self.inner_long_net_values = self.make_start_to_one((self.inner_rets_long + 1).cumprod())
-        self.inner_short_net_values = self.make_start_to_one((self.inner_rets_short + 1).cumprod())
+            self.long_short_net_values = self.make_start_to_one(
+                (self.long_short_rets + 1).cumprod()
+            )
+            self.inner_rets_long = (
+                self.group_rets["group" + str(groups_num)] - self.rets_all
+            )
+            self.inner_rets_short = self.rets_all - self.group_rets.group1
+        self.inner_long_net_values = self.make_start_to_one(
+            (self.inner_rets_long + 1).cumprod()
+        )
+        self.inner_short_net_values = self.make_start_to_one(
+            (self.inner_rets_short + 1).cumprod()
+        )
         self.group_rets = self.group_rets.assign(long_short=self.long_short_rets)
         self.group_net_values = self.group_rets.applymap(lambda x: x + 1)
         self.group_net_values = self.group_net_values.cumprod()
         self.group_net_values = self.group_net_values.apply(self.make_start_to_one)
         a = groups_num ** (0.5)
         # 判断是否要两个因子画表格
         if a == int(a):
@@ -2089,15 +2111,18 @@
                     {
                         "评价指标": [
                             self.factor_turnover_rate,
                             self.factor_cover,
                             self.pos_neg_rate,
                             self.factor_cross_skew,
                             self.inner_long_ret_yearly,
-                            self.inner_long_ret_yearly/(self.inner_long_ret_yearly+self.inner_short_ret_yearly),
+                            self.inner_long_ret_yearly
+                            / (
+                                self.inner_long_ret_yearly + self.inner_short_ret_yearly
+                            ),
                             self.corr_itself,
                         ]
                     },
                     index=[
                         f"多头{self.freq_ctrl.comment_name}均换手",
                         "因子覆盖率",
                         "因子正值占比",
@@ -2517,14 +2542,15 @@
         zxindustry_dummy: pd.DataFrame = None,
         no_read_indu: bool = 0,
         only_cap: bool = 0,
         iplot: bool = 1,
         ilegend: bool = 0,
         without_breakpoint: bool = 0,
         opens_average_first_day: bool = 0,
+        total_cap: bool = 0,
     ) -> None:
         """一键回测框架，测试单因子的月频调仓的分组表现
         每月月底计算因子值，月初第一天开盘时买入，月末收盘最后一天收盘时卖出
         剔除上市不足60天的，停牌天数超过一半的，st天数超过一半的
         月末收盘跌停的不卖出，月初开盘涨停的不买入
         由最好组和最差组的多空组合构成多空对冲组
 
@@ -2604,14 +2630,16 @@
             使用cufflinks呈现回测结果, by default 1
         ilegend : bool, optional
             使用cufflinks绘图时，是否显示图例, by default 1
         without_breakpoint : bool, optional
             画图的时候是否去除间断点, by default 0
         opens_average_first_day : bool, optional
             买入时使用第一天的平均价格, by default 0
+        total_cap : bool, optional
+            加权和行业市值中性化时使用总市值, by default 0
         """
 
         if not isinstance(factors, pd.DataFrame):
             factors = factors()
         if comments_writer is None and sheetname is not None:
             from pure_ocean_breeze.state.states import COMMENTS_WRITER
 
@@ -2640,56 +2668,93 @@
             factors = factors[factors.index <= pd.Timestamp(str(time_end))]
         if boxcox + neutralize == 0:
             no_read_indu = 1
         if only_cap + no_read_indu > 0:
             only_cap = no_read_indu = 1
         if iplot:
             print_comments = 0
-        if opens_average_first_day:
-            if freq == "M":
-                self.shen = pure_moon(
-                    freq=freq,
-                    no_read_indu=no_read_indu,
-                    swindustry_dummy=swindustry_dummy,
-                    zxindustry_dummy=zxindustry_dummy,
-                    read_in_swindustry_dummy=swindustry_dummies,
-                )
-            elif freq == "W":
-                self.shen = pure_week(
-                    freq=freq,
-                    no_read_indu=no_read_indu,
-                    swindustry_dummy=swindustry_dummy,
-                    zxindustry_dummy=zxindustry_dummy,
-                    read_in_swindustry_dummy=swindustry_dummies,
-                )
+        if total_cap:
+            if opens_average_first_day:
+                if freq == "M":
+                    self.shen = pure_moon_b(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
+                elif freq == "W":
+                    self.shen = pure_week_b(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
+            else:
+                if freq == "M":
+                    self.shen = pure_moon_c(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
+                elif freq == "W":
+                    self.shen = pure_week_c(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
         else:
-            if freq == "M":
-                self.shen = pure_moon_a(
-                    freq=freq,
-                    no_read_indu=no_read_indu,
-                    swindustry_dummy=swindustry_dummy,
-                    zxindustry_dummy=zxindustry_dummy,
-                    read_in_swindustry_dummy=swindustry_dummies,
-                )
-            elif freq == "W":
-                self.shen = pure_week_a(
-                    freq=freq,
-                    no_read_indu=no_read_indu,
-                    swindustry_dummy=swindustry_dummy,
-                    zxindustry_dummy=zxindustry_dummy,
-                    read_in_swindustry_dummy=swindustry_dummies,
-                )
+            if opens_average_first_day:
+                if freq == "M":
+                    self.shen = pure_moon(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
+                elif freq == "W":
+                    self.shen = pure_week(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
+            else:
+                if freq == "M":
+                    self.shen = pure_moon_a(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
+                elif freq == "W":
+                    self.shen = pure_week_a(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
         self.shen.set_basic_data(
             ages=ages,
             sts=sts,
             states=states,
             opens=opens,
             closes=closes,
             capitals=capitals,
             opens_average_first_day=opens_average_first_day,
+            total_cap=total_cap,
         )
         self.shen.set_factor_df_date_as_index(factors)
         self.shen.prerpare()
         self.shen.run(
             groups_num=groups_num,
             neutralize=neutralize,
             boxcox=boxcox,
@@ -2767,14 +2832,30 @@
     ...
 
 
 class pure_week_a(pure_moon):
     ...
 
 
+class pure_moon_b(pure_moon):
+    ...
+
+
+class pure_week_b(pure_moon):
+    ...
+
+
+class pure_moon_c(pure_moon):
+    ...
+
+
+class pure_week_c(pure_moon):
+    ...
+
+
 class pure_fall(object):
     # DONE：修改为因子文件名可以带“日频_“，也可以不带“日频_“
     def __init__(self, daily_path: str) -> None:
         """一个使用mysql中的分钟数据，来更新因子值的框架
 
         Parameters
         ----------
@@ -4175,23 +4256,24 @@
         )
 
 
 @do_on_dfs
 def follow_tests(
     fac: pd.DataFrame,
     trade_cost_double_side_list: float = [0.001, 0.002, 0.003, 0.004, 0.005],
-    index_member_value_weighted: bool=0,
+    index_member_value_weighted: bool = 1,
     comments_writer: pd.ExcelWriter = None,
     net_values_writer: pd.ExcelWriter = None,
     pos: bool = 0,
     neg: bool = 0,
     swindustry: bool = 0,
     zxindustry: bool = 0,
     nums: List[int] = [3],
     opens_average_first_day: bool = 0,
+    total_cap: bool = 0,
 ):
     """因子完成全A测试后，进行的一些必要的后续测试，包括各个分组表现、相关系数与纯净化、3510的多空和多头、各个行业Rank IC、各个行业买3只超额表现
 
     Parameters
     ----------
     fac : pd.DataFrame
         要进行后续测试的因子值，index是时间，columns是股票代码，values是因子值
@@ -4211,14 +4293,16 @@
         使用申万一级行业, by default 0
     zxindustry : bool, optional
         使用中信一级行业, by default 0
     nums : List[int], optional
         各个行业买几只股票, by default [3]
     opens_average_first_day : bool, optional
         买入时使用第一天的平均价格, by default 0
+    total_cap : bool, optional
+        加权和行业市值中性化时使用总市值, by default 0
 
     Raises
     ------
     IOError
         如果未指定因子正负方向，将报错
     """
     if comments_writer is None:
@@ -4251,25 +4335,27 @@
     print(pure_fac.corr)
     shen = pure_moonnight(
         pure_fac(),
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="纯净",
         opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
     )
     """3510多空和多头"""
     # 300
     fi300 = daily_factor_on300500(fac, hs300=1)
     shen = pure_moonnight(
         fi300,
         value_weighted=index_member_value_weighted,
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="300多空",
         opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
     )
     if pos:
         if comments_writer is not None:
             make_relative_comments(shen.shen.group_rets.group10, hs300=1).to_excel(
                 comments_writer, sheet_name="300超额"
             )
             for i in trade_cost_double_side_list:
@@ -4324,14 +4410,15 @@
     shen = pure_moonnight(
         fi500,
         value_weighted=index_member_value_weighted,
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="500多空",
         opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
     )
     if pos:
         if comments_writer is not None:
             make_relative_comments(shen.shen.group_rets.group10, zz500=1).to_excel(
                 comments_writer, sheet_name="500超额"
             )
             for i in trade_cost_double_side_list:
@@ -4384,14 +4471,15 @@
     shen = pure_moonnight(
         fi1000,
         value_weighted=index_member_value_weighted,
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="1000多空",
         opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
     )
     if pos:
         if comments_writer is not None:
             make_relative_comments(shen.shen.group_rets.group10, zz1000=1).to_excel(
                 comments_writer, sheet_name="1000超额"
             )
             for i in trade_cost_double_side_list:
@@ -4446,21 +4534,22 @@
         fac, nums, pos=pos, neg=neg, swindustry=swindustry, zxindustry=zxindustry
     )
     logger.success("因子后续的必要测试全部完成")
 
 
 def test_on_index_four_out(
     fac: pd.DataFrame,
-    value_weighted: bool=0,
+    value_weighted: bool = 1,
     trade_cost_double_side_list: float = [0.001, 0.002, 0.003, 0.004, 0.005],
     group_num: int = 10,
     boxcox: bool = 1,
     comments_writer: pd.ExcelWriter = None,
     net_values_writer: pd.ExcelWriter = None,
     opens_average_first_day: bool = 0,
+    total_cap: bool = 0,
 ):
     if comments_writer is None:
         from pure_ocean_breeze.state.states import COMMENTS_WRITER
 
         comments_writer = COMMENTS_WRITER
     if net_values_writer is None:
         from pure_ocean_breeze.state.states import NET_VALUES_WRITER
@@ -4489,14 +4578,15 @@
         value_weighted=value_weighted,
         groups_num=group_num,
         boxcox=boxcox,
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="300多空",
         opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
     )
     if pos:
         if comments_writer is not None:
             make_relative_comments(
                 shen.shen.group_rets[f"group{group_num}"], hs300=1
             ).to_excel(comments_writer, sheet_name="300超额")
             for i in trade_cost_double_side_list:
@@ -4555,14 +4645,15 @@
         value_weighted=value_weighted,
         groups_num=group_num,
         boxcox=boxcox,
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="500多空",
         opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
     )
     if pos:
         if comments_writer is not None:
             make_relative_comments(
                 shen.shen.group_rets[f"group{group_num}"], zz500=1
             ).to_excel(comments_writer, sheet_name="500超额")
             for i in trade_cost_double_side_list:
@@ -4619,14 +4710,15 @@
         value_weighted=value_weighted,
         groups_num=group_num,
         boxcox=boxcox,
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="1000多空",
         opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
     )
     if pos:
         if comments_writer is not None:
             make_relative_comments(
                 shen.shen.group_rets[f"group{group_num}"], zz1000=1
             ).to_excel(comments_writer, sheet_name="1000超额")
             for i in trade_cost_double_side_list:
@@ -4747,14 +4839,15 @@
         backsee: int = 20,
         rets: pd.DataFrame = None,
         value_weighted: bool = 1,
         add_market: bool = 1,
         add_market_series: pd.Series = None,
         factors_names: list = None,
         betas_rets: bool = 0,
+        total_cap: bool = 0,
     ) -> None:
         """使用fama三因子的方法，将个股的收益率，拆分出各个因子带来的收益率以及特质的收益率
         分别计算每一期，各个因子收益率的值，超额收益率，因子的暴露，以及特质收益率
 
         Parameters
         ----------
         factors : List[pd.DataFrame]
@@ -4771,14 +4864,16 @@
             是否加入市场收益率因子，默认使用中证全指的每日日间收益率, by default 1
         add_market_series : bool, optional
             加入的市场收益率的数据，如果没指定，则使用中证全指的日间收益率, by default None
         factors_names : list, optional
             各个因子的名字，默认为fac0(市场收益率因子，如果没有，则从fac1开始),fac1,fac2,fac3, by default None
         betas_rets : bool, optional
             是否计算每只个股的由于暴露在每个因子上所带来的收益率, by default 0
+        total_cap : bool, optional
+            加权时使用总市值, by default 0
         """
         start = max(
             [int(datetime.datetime.strftime(i.index.min(), "%Y%m%d")) for i in factors]
         )
         self.backsee = backsee
         self.factors = factors
         self.factors_names = factors_names
@@ -4794,14 +4889,16 @@
         ]
         self.factors_group_long = [(i == 0) + 0 for i in self.factors_group]
         self.factors_group_short = [
             (i == (j - 1)) + 0 for i, j in zip(self.factors_group, self.minus_group)
         ]
         self.value_weighted = value_weighted
         if value_weighted:
+            if total_cap:
+                self.cap=read_daily(total_cap=1,start=start)
             self.cap = read_daily(flow_cap=1, start=start)
             self.factors_group_long = [self.cap * i for i in self.factors_group_long]
             self.factors_group_short = [self.cap * i for i in self.factors_group_short]
             self.factors_group_long = [
                 (i.T / i.T.sum()).T for i in self.factors_group_long
             ]
             self.factors_group_short = [
@@ -5078,22 +5175,23 @@
 
 
 @do_on_dfs
 def test_on_300500(
     df: pd.DataFrame,
     trade_cost_double_side: float = 0,
     group_num: int = 10,
-    value_weighted: bool=0,
+    value_weighted: bool = 1,
     boxcox: bool = 0,
     hs300: bool = 0,
     zz500: bool = 0,
     zz1000: bool = 0,
     gz2000: bool = 0,
     iplot: bool = 1,
     opens_average_first_day: bool = 0,
+    total_cap: bool=0,
 ) -> pd.Series:
     """对因子在指数成分股内进行多空和多头测试
 
     Parameters
     ----------
     df : pd.DataFrame
         因子值，index为时间，columns为股票代码
@@ -5107,18 +5205,20 @@
         在沪深300成分股内测试, by default 0
     zz500 : bool, optional
         在中证500成分股内测试, by default 0
     zz1000 : bool, optional
         在中证1000成分股内测试, by default 0
     gz1000 : bool, optional
         在国证2000成分股内测试, by default 0
-    iplot : bol,optional
+    iplot : bo0l,optional
         多空回测的时候，是否使用cufflinks绘画
     opens_average_first_day : bool, optional
         买入时使用第一天的平均价格, by default 0
+    total_cap : bool, optional
+        加权和行业市值中性化时使用总市值, by default 0
 
     Returns
     -------
     pd.Series
         多头组在该指数上的超额收益序列
     """
     fi300 = daily_factor_on300500(
@@ -5128,14 +5228,15 @@
         fi300,
         value_weighted=value_weighted,
         groups_num=group_num,
         trade_cost_double_side=trade_cost_double_side,
         boxcox=boxcox,
         iplot=iplot,
         opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
     )
     if (
         shen.shen.group_net_values.group1.iloc[-1]
         > shen.shen.group_net_values[f"group{group_num}"].iloc[-1]
     ):
         print(
             make_relative_comments(
@@ -5173,21 +5274,22 @@
         )
         return abrets
 
 
 @do_on_dfs
 def test_on_index_four(
     df: pd.DataFrame,
-    value_weighted: bool=0,
+    value_weighted: bool = 1,
     group_num: int = 10,
     trade_cost_double_side: float = 0,
     iplot: bool = 1,
     gz2000: bool = 0,
     boxcox: bool = 1,
     opens_average_first_day: bool = 0,
+    total_cap: bool = 0,
 ) -> pd.DataFrame:
     """对因子同时在沪深300、中证500、中证1000、国证2000这4个指数成分股内进行多空和多头超额测试
 
     Parameters
     ----------
     df : pd.DataFrame
         因子值，index为时间，columns为股票代码
@@ -5201,14 +5303,16 @@
         多空回测的时候，是否使用cufflinks绘画
     gz2000 : bool, optional
         是否进行国证2000上的测试, by default 0
     boxcox : bool, optional
         是否进行行业市值中性化处理, by default 1
     opens_average_first_day : bool, optional
         买入时使用第一天的平均价格, by default 0
+    total_cap : bool, optional
+        加权和行业市值中性化时使用总市值, by default 0
 
     Returns
     -------
     pd.DataFrame
         多头组在各个指数上的超额收益序列
     """
     fi300 = daily_factor_on300500(df, hs300=1)
@@ -5216,14 +5320,15 @@
         fi300,
         groups_num=group_num,
         value_weighted=value_weighted,
         trade_cost_double_side=trade_cost_double_side,
         iplot=iplot,
         boxcox=boxcox,
         opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
     )
     if (
         shen.shen.group_net_values.group1.iloc[-1]
         > shen.shen.group_net_values[f"group{group_num}"].iloc[-1]
     ):
         com300, net300 = make_relative_comments(
             shen.shen.group_rets.group1, hs300=1, show_nets=1
@@ -5233,40 +5338,43 @@
             fi500,
             groups_num=group_num,
             value_weighted=value_weighted,
             trade_cost_double_side=trade_cost_double_side,
             iplot=iplot,
             boxcox=boxcox,
             opens_average_first_day=opens_average_first_day,
+            total_cap=total_cap,
         )
         com500, net500 = make_relative_comments(
             shen.shen.group_rets.group1, zz500=1, show_nets=1
         )
         fi1000 = daily_factor_on300500(df, zz1000=1)
         shen = pure_moonnight(
             fi1000,
             groups_num=group_num,
             value_weighted=value_weighted,
             trade_cost_double_side=trade_cost_double_side,
             iplot=iplot,
             boxcox=boxcox,
             opens_average_first_day=opens_average_first_day,
+            total_cap=total_cap,
         )
         com1000, net1000 = make_relative_comments(
             shen.shen.group_rets.group1, zz1000=1, show_nets=1
         )
         if gz2000:
             fi2000 = daily_factor_on300500(df, gz2000=1)
             shen = pure_moonnight(
                 fi2000,
                 groups_num=group_num,
                 trade_cost_double_side=trade_cost_double_side,
                 iplot=iplot,
                 boxcox=boxcox,
                 opens_average_first_day=opens_average_first_day,
+                total_cap=total_cap,
             )
             com2000, net2000 = make_relative_comments(
                 shen.shen.group_rets.group1, gz2000=1, show_nets=1
             )
     else:
         com300, net300 = make_relative_comments(
             shen.shen.group_rets[f"group{group_num}"], hs300=1, show_nets=1
@@ -5276,41 +5384,44 @@
             fi500,
             groups_num=group_num,
             value_weighted=value_weighted,
             trade_cost_double_side=trade_cost_double_side,
             iplot=iplot,
             boxcox=boxcox,
             opens_average_first_day=opens_average_first_day,
+            total_cap=total_cap,
         )
         com500, net500 = make_relative_comments(
             shen.shen.group_rets[f"group{group_num}"], zz500=1, show_nets=1
         )
         fi1000 = daily_factor_on300500(df, zz1000=1)
         shen = pure_moonnight(
             fi1000,
             groups_num=group_num,
             value_weighted=value_weighted,
             trade_cost_double_side=trade_cost_double_side,
             iplot=iplot,
             boxcox=boxcox,
             opens_average_first_day=opens_average_first_day,
+            total_cap=total_cap,
         )
         com1000, net1000 = make_relative_comments(
             shen.shen.group_rets[f"group{group_num}"], zz1000=1, show_nets=1
         )
         if gz2000:
             fi2000 = daily_factor_on300500(df, gz2000=1)
             shen = pure_moonnight(
                 fi2000,
                 groups_num=group_num,
                 value_weighted=value_weighted,
                 trade_cost_double_side=trade_cost_double_side,
                 iplot=iplot,
                 boxcox=boxcox,
                 opens_average_first_day=opens_average_first_day,
+                total_cap=total_cap,
             )
             com2000, net2000 = make_relative_comments(
                 shen.shen.group_rets[f"group{group_num}"], gz2000=1, show_nets=1
             )
     com300 = com300.to_frame("300超额")
     com500 = com500.to_frame("500超额")
     com1000 = com1000.to_frame("1000超额")
@@ -5868,7 +5979,240 @@
             self.zz1000_comments.to_excel(comments_writer, sheet_name="中证1000组合优化超额绩效")
         if net_values_writer is not None:
             self.hs300_nets.to_excel(net_values_writer, sheet_name="沪深300组合优化净值")
             self.zz500_nets.to_excel(net_values_writer, sheet_name="中证500组合优化净值")
             self.zz1000_nets.to_excel(net_values_writer, sheet_name="中证1000组合优化净值")
 
         return self.comments.T
+
+
+def symmetrically_orthogonalize(dfs: list[pd.DataFrame]) -> list[pd.DataFrame]:
+    """对多个因子做对称正交，每个因子得到正交其他因子后的结果
+
+    Parameters
+    ----------
+    dfs : list[pd.DataFrame]
+        多个要做正交的因子，每个df都是index为时间，columns为股票代码，values为因子值的df
+
+    Returns
+    -------
+    list[pd.DataFrame]
+        对称正交后的各个因子
+    """
+
+    def sing(dfs: list[pd.DataFrame], date: pd.Timestamp):
+        dds = []
+        for num, i in enumerate(dfs):
+            i = i[i.index == date]
+            i.index = [f"fac{num}"]
+            i = i.T
+            dds.append(i)
+        dds = pd.concat(dds, axis=1)
+        cov = dds.cov()
+        d, u = np.linalg.eig(cov)
+        d = np.diag(d ** (-0.5))
+        new_facs = pd.DataFrame(
+            np.dot(dds, np.dot(np.dot(u, d), u.T)), columns=dds.columns, index=dds.index
+        )
+        new_facs = new_facs.stack().reset_index()
+        new_facs.columns = ["code", "fac_number", "fac"]
+        new_facs = new_facs.assign(date=date)
+        dds = []
+        for num, i in enumerate(dfs):
+            i = new_facs[new_facs.fac_number == f"fac{num}"]
+            i = i.pivot(index="date", columns="code", values="fac")
+            dds.append(i)
+        return dds
+
+    dfs = [standardlize(i) for i in dfs]
+    date_first = max([i.index.min() for i in dfs])
+    date_last = min([i.index.max() for i in dfs])
+    dfs = [i[(i.index >= date_first) & (i.index <= date_last)] for i in dfs]
+    fac_num = len(dfs)
+    ddss = [[] for i in range(fac_num)]
+    for date in tqdm.auto.tqdm(dfs[0].index):
+        dds = sing(dfs, date)
+        for num, i in enumerate(dds):
+            ddss[num].append(i)
+    ds = []
+    for i in tqdm.auto.tqdm(ddss):
+        ds.append(pd.concat(i))
+    return ds
+
+
+def icir_weight(
+    facs: list[pd.DataFrame],
+    backsee: int = 6,
+    boxcox: bool = 0,
+    rank_corr: bool = 0,
+    only_ic: bool = 0,
+) -> pd.DataFrame:
+    """使用icir滚动加权的方式，加权合成几个因子
+
+    Parameters
+    ----------
+    facs : list[pd.DataFrame]
+        要合成的若干因子，每个df都是index为时间，columns为股票代码，values为因子值的df
+    backsee : int, optional
+        用来计算icir的过去期数, by default 6
+    boxcox : bool, optional
+        是否对因子进行行业市值中性化, by default 0
+    rank_corr : bool, optional
+        是否计算rankicir, by default 0
+    only_ic : bool, optional
+        是否只计算IC或Rank IC, by default 0
+
+    Returns
+    -------
+    pd.DataFrame
+        合成后的因子
+
+    Raises
+    ------
+    ValueError
+        因子期数少于回看期数时将报错
+    """
+    date_first_max = max([i.index[0] for i in facs])
+    facs = [i[i.index >= date_first_max] for i in facs]
+    date_last_min = min([i.index[-1] for i in facs])
+    facs = [i[i.index <= date_last_min] for i in facs]
+    facs = [i.shift(1) for i in facs]
+    ret = read_daily(
+        close=1, start=datetime.datetime.strftime(date_first_max, "%Y%m%d")
+    )
+    ret = ret / ret.shift(20) - 1
+    if boxcox:
+        facs = [decap_industry(i) for i in facs]
+    facs = [((i.T - i.T.mean()) / i.T.std()).T for i in facs]
+    dates = list(facs[0].index)
+    fis = []
+    for num, date in tqdm.auto.tqdm(list(enumerate(dates))):
+        if num < backsee:
+            ...
+        else:
+            nears = [i.iloc[num - backsee : num, :] for i in facs]
+            targets = [i[i.index == date] for i in facs]
+            if rank_corr:
+                weights = [
+                    show_corr(
+                        i, ret[ret.index.isin(i.index)], plt_plot=0, show_series=1
+                    )
+                    for i in nears
+                ]
+            else:
+                weights = [
+                    show_corr(
+                        i,
+                        ret[ret.index.isin(i.index)],
+                        plt_plot=0,
+                        show_series=1,
+                        method="pearson",
+                    )
+                    for i in nears
+                ]
+            if only_ic:
+                weights = [i.mean() for i in weights]
+            else:
+                weights = [i.mean() / i.std() for i in weights]
+            fi = sum([i * j for i, j in zip(weights, targets)])
+            fis.append(fi)
+    if len(fis) > 0:
+        return pd.concat(fis).shift(-1)
+    else:
+        raise ValueError("输入的因子值长度不太够吧？")
+
+
+def scipy_weight(
+    facs: list[pd.DataFrame],
+    backsee: int = 6,
+    boxcox: bool = 0,
+    rank_corr: bool = 0,
+    only_ic: bool = 0,
+    upper_bound: float = None,
+    lower_bound: float = 0,
+) -> pd.DataFrame:
+    """使用scipy的minimize优化求解的方式，寻找最优的因子合成权重，默认优化条件为最大ICIR
+
+    Parameters
+    ----------
+    facs : list[pd.DataFrame]
+        要合成的因子，每个df都是index为时间，columns为股票代码，values为因子值的df
+    backsee : int, optional
+        用来计算icir的过去期数, by default 6
+    boxcox : bool, optional
+        是否对因子进行行业市值中性化, by default 0
+    rank_corr : bool, optional
+        是否计算rankicir, by default 0
+    only_ic : bool, optional
+        是否只计算IC或Rank IC, by default 0
+    upper_bound : float, optional
+        每个因子的权重上限，如果不指定，则为每个因子平均权重的2倍，即2除以因子数量, by default None
+    lower_bound : float, optional
+        每个因子的权重下限, by default 0
+
+    Returns
+    -------
+    pd.DataFrame
+        合成后的因子
+    """
+    date_first_max = max([i.index[0] for i in facs])
+    facs = [i[i.index >= date_first_max] for i in facs]
+    date_last_min = min([i.index[-1] for i in facs])
+    facs = [i[i.index <= date_last_min] for i in facs]
+    facs = [i.shift(1) for i in facs]
+    ret = read_daily(
+        close=1, start=datetime.datetime.strftime(date_first_max, "%Y%m%d")
+    )
+    ret = ret / ret.shift(20) - 1
+    if boxcox:
+        facs = [decap_industry(i) for i in facs]
+    facs = [((i.T - i.T.mean()) / i.T.std()).T for i in facs]
+    if upper_bound is None:
+        upper_bound = 2 / len(facs)
+    dates = list(facs[0].index)
+    fis = []
+    for num, date in tqdm.auto.tqdm(list(enumerate(dates))):
+        if num <= backsee:
+            ...
+        else:
+            nears = [i.iloc[num - backsee : num, :] for i in facs]
+            targets = [i[i.index == date] for i in facs]
+            if rank_corr:
+                weights = [
+                    show_corr(
+                        i, ret[ret.index.isin(i.index)], plt_plot=0, show_series=1
+                    )
+                    for i in nears
+                ]
+            else:
+                weights = [
+                    show_corr(
+                        i,
+                        ret[ret.index.isin(i.index)],
+                        plt_plot=0,
+                        show_series=1,
+                        method="pearson",
+                    )
+                    for i in nears
+                ]
+            if only_ic:
+                weights = [i.mean() for i in weights]
+            else:
+                weights = [i.mean() / i.std() for i in weights]
+            weights = pd.concat(weights, axis=1)
+
+            def func(x):
+                w = np.array(x).reshape((-1, 1))
+                y = weights @ w
+                return np.mean(y) / np.std(y)
+
+            cons = {"type": "eq", "fun": lambda x: np.sum(x) - 1}
+            res = minimize(
+                func,
+                np.random.rand(weights.shape[1], 1),
+                constraints=cons,
+                bounds=[(lower_bound, upper_bound)] * weights.shape[1],
+            )
+            xs = res.x.tolist()
+            fac = sum([i * j for i, j in zip(xs, targets)])
+            fis.append(fac)
+    return pd.concat(fis).shift(-1)
```

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 3.9.3
+Version: 3.9.4
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.3/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.3/setup.py` & `pure_ocean_breeze-3.9.4/setup.py`

 * *Files identical despite different names*

