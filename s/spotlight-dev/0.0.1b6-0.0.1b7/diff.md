# Comparing `tmp/spotlight-dev-0.0.1b6.tar.gz` & `tmp/spotlight-dev-0.0.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotlight-dev-0.0.1b6.tar", last modified: Tue May  9 17:15:56 2023, max compression
+gzip compressed data, was "spotlight-dev-0.0.1b7.tar", last modified: Tue May  9 20:53:26 2023, max compression
```

## Comparing `spotlight-dev-0.0.1b6.tar` & `spotlight-dev-0.0.1b7.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.026770 spotlight-dev-0.0.1b6/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-09 17:15:56.026770 spotlight-dev-0.0.1b6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 17:15:56.026770 spotlight-dev-0.0.1b6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1216 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.964765 spotlight-dev-0.0.1b6/spotlight/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.965765 spotlight-dev-0.0.1b6/spotlight/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.967765 spotlight-dev-0.0.1b6/spotlight/api/auth/
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/auth/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/auth/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1726 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/auth/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.972766 spotlight-dev-0.0.1b6/spotlight/api/job/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2640 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.976766 spotlight-dev-0.0.1b6/spotlight/api/job/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/view/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.979766 spotlight-dev-0.0.1b6/spotlight/api/organization/
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.983766 spotlight-dev-0.0.1b6/spotlight/api/organization/user/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/user/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/user/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/user/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/user/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/user/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/user/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.986767 spotlight-dev-0.0.1b6/spotlight/api/organization/view/
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.990767 spotlight-dev-0.0.1b6/spotlight/api/rule/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/rule/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3667 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/rule/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/rule/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/rule/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.993767 spotlight-dev-0.0.1b6/spotlight/api/tag/
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3844 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.997767 spotlight-dev-0.0.1b6/spotlight/api/tag/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.998767 spotlight-dev-0.0.1b6/spotlight/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.003768 spotlight-dev-0.0.1b6/spotlight/core/common/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/base.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2712 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.004768 spotlight-dev-0.0.1b6/spotlight/core/common/date/
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/date/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/date/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.005768 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.007768 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3898 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.009768 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/timeit.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.010769 spotlight-dev-0.0.1b6/spotlight/core/common/metaclass/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/metaclass/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/metaclass/singleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.011768 spotlight-dev-0.0.1b6/spotlight/core/common/requests/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/requests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/requests/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/requests/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.013769 spotlight-dev-0.0.1b6/spotlight/core/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5958 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/decorator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.014769 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.016769 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2154 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/enum.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/sql_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     3413 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.018769 spotlight-dev-0.0.1b6/spotlight/core/pipeline/model/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/model/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/model/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.019769 spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/
--rw-rw-rw-   0 root         (0) root         (0)     6327 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.020769 spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/utils/
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/utils/asynchronously.py
--rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/utils/synchronously.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.022769 spotlight-dev-0.0.1b6/spotlight/pandas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/pandas/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/pandas/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/pandas/runners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.025770 spotlight-dev-0.0.1b6/spotlight_dev.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-09 17:15:55.000000 spotlight-dev-0.0.1b6/spotlight_dev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3859 2023-05-09 17:15:55.000000 spotlight-dev-0.0.1b6/spotlight_dev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 17:15:55.000000 spotlight-dev-0.0.1b6/spotlight_dev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      141 2023-05-09 17:15:55.000000 spotlight-dev-0.0.1b6/spotlight_dev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-09 17:15:55.000000 spotlight-dev-0.0.1b6/spotlight_dev.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.795951 spotlight-dev-0.0.1b7/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-09 20:53:26.794951 spotlight-dev-0.0.1b7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 20:53:26.795951 spotlight-dev-0.0.1b7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.763949 spotlight-dev-0.0.1b7/spotlight/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.764949 spotlight-dev-0.0.1b7/spotlight/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.765949 spotlight-dev-0.0.1b7/spotlight/api/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/auth/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/auth/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/auth/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.766949 spotlight-dev-0.0.1b7/spotlight/api/job/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2909 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.767949 spotlight-dev-0.0.1b7/spotlight/api/job/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/job/view/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.768949 spotlight-dev-0.0.1b7/spotlight/api/organization/
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.770949 spotlight-dev-0.0.1b7/spotlight/api/organization/user/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/user/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/user/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/user/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/user/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/user/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/user/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.772950 spotlight-dev-0.0.1b7/spotlight/api/organization/view/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/organization/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.774950 spotlight-dev-0.0.1b7/spotlight/api/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/rule/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3809 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/rule/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/rule/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/rule/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.774950 spotlight-dev-0.0.1b7/spotlight/api/tag/
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     4466 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4008 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.776950 spotlight-dev-0.0.1b7/spotlight/api/tag/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/api/tag/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.777950 spotlight-dev-0.0.1b7/spotlight/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.779950 spotlight-dev-0.0.1b7/spotlight/core/common/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2712 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.780950 spotlight-dev-0.0.1b7/spotlight/core/common/date/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/date/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/date/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.780950 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.781950 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.782950 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/decorators/timeit.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.783950 spotlight-dev-0.0.1b7/spotlight/core/common/metaclass/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/metaclass/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/metaclass/singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.784950 spotlight-dev-0.0.1b7/spotlight/core/common/requests/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/requests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/requests/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/requests/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/common/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.784950 spotlight-dev-0.0.1b7/spotlight/core/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5958 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/decorator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.784950 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.786951 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2154 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/sql_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     3413 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.787951 spotlight-dev-0.0.1b7/spotlight/core/pipeline/model/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/model/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/model/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.787951 spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/
+-rw-rw-rw-   0 root         (0) root         (0)     6327 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.789951 spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/utils/asynchronously.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/utils/synchronously.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.790951 spotlight-dev-0.0.1b7/spotlight/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/pandas/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/pandas/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-09 20:53:09.000000 spotlight-dev-0.0.1b7/spotlight/pandas/runners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:53:26.793951 spotlight-dev-0.0.1b7/spotlight_dev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-09 20:53:26.000000 spotlight-dev-0.0.1b7/spotlight_dev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3859 2023-05-09 20:53:26.000000 spotlight-dev-0.0.1b7/spotlight_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 20:53:26.000000 spotlight-dev-0.0.1b7/spotlight_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-09 20:53:26.000000 spotlight-dev-0.0.1b7/spotlight_dev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-09 20:53:26.000000 spotlight-dev-0.0.1b7/spotlight_dev.egg-info/top_level.txt
```

### Comparing `spotlight-dev-0.0.1b6/PKG-INFO` & `spotlight-dev-0.0.1b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b6
+Version: 0.0.1b7
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b6/README.md` & `spotlight-dev-0.0.1b7/README.md`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/setup.py` & `spotlight-dev-0.0.1b7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     tag = subprocess.getoutput('git tag --sort=version:refname | tail -n1')
     commits = subprocess.getoutput(f'git rev-list {tag}..HEAD --count')
     return f'{tag}.{commits}'
 
 
 setuptools.setup(
     name="spotlight-dev",
-    version="0.0.1b6",
+    version="0.0.1b7",
     author="Spotlight",
     author_email="hello@spotlight.dev",
     description="Spotlight Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://alpha.dev",
     classifiers=[
@@ -39,10 +39,11 @@
         "aiohttp>=3.8.4",
         "pandas>=2.0.1",
         "duckdb>=0.7.1",
         "trycast>=1.0.0",
         "pydash>=7.0.3",
         "cachetools>=5.3.0",
         "pydantic>=1.10.7",
-        "aiocache>=0.12.1"
+        "aiocache>=0.12.1",
+        "backoff>=2.2.1"
     ]
 )
```

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/auth/__util.py` & `spotlight-dev-0.0.1b7/spotlight/api/auth/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/auth/asynchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/auth/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/auth/synchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/auth/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/job/__util.py` & `spotlight-dev-0.0.1b7/spotlight/api/job/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/job/asynchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/job/asynchronous.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from typing import Dict, Any, List
 
+import aiohttp
+import backoff
+import requests
+
 from spotlight.api.model import SearchRequest
 from spotlight.api.job.__util import (
     _get_job_request_info,
     _get_jobs_request_info,
     _create_job_request_info,
     _update_job_request_info,
     _delete_job_request_info,
@@ -58,14 +62,17 @@
     Returns:
         List[Dict[str, Any]]: List of job responses
     """
     request_info = _search_jobs_request_info(request)
     return await __async_post_request(**request_info)
 
 
+@backoff.on_exception(
+    backoff.expo, (aiohttp.ClientTimeout, aiohttp.ClientConnectionError), max_tries=3
+)
 @async_data_request
 async def async_create_job(request: JobRequest) -> Dict[str, Any]:
     """
     Asynchronously create job.
 
     Args:
         request (JobRequest): Job request
@@ -73,14 +80,17 @@
     Returns:
         Dict[str, Any]: Job response
     """
     request_info = _create_job_request_info(request)
     return await __async_put_request(**request_info)
 
 
+@backoff.on_exception(
+    backoff.expo, (aiohttp.ClientTimeout, aiohttp.ClientConnectionError), max_tries=3
+)
 @async_data_request
 async def async_update_job(id: str, request: JobRequest) -> Dict[str, Any]:
     """
     Asynchronously update job.
 
     NOTE: Tags associated to the job are not updated
```

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/job/model.py` & `spotlight-dev-0.0.1b7/spotlight/api/job/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/job/view/asynchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/job/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/organization/__util.py` & `spotlight-dev-0.0.1b7/spotlight/api/organization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/organization/asynchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/organization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/organization/synchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/organization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/organization/user/__util.py` & `spotlight-dev-0.0.1b7/spotlight/api/organization/user/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/organization/user/asynchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/organization/user/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/organization/user/model.py` & `spotlight-dev-0.0.1b7/spotlight/api/organization/user/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/organization/user/synchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/organization/user/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/organization/view/asynchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/organization/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/organization/view/synchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/organization/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/rule/__util.py` & `spotlight-dev-0.0.1b7/spotlight/api/rule/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/rule/asynchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/rule/asynchronous.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from typing import Dict, Any, List
 
+import aiohttp
+import backoff
+
 from spotlight.api.model import SearchRequest, LookupRequest
 from spotlight.api.rule.__util import (
     _get_rule_request_info,
     _get_rules_request_info,
     _create_rule_request_info,
     _update_rule_request_info,
     _delete_rule_request_info,
@@ -45,14 +48,17 @@
     Returns:
         List[Dict[str, Any]]: List of rule responses
     """
     request_info = _get_rules_request_info()
     return await __async_get_request(**request_info)
 
 
+@backoff.on_exception(
+    backoff.expo, (aiohttp.ClientTimeout, aiohttp.ClientConnectionError), max_tries=3
+)
 @async_data_request
 async def async_get_rules_by_tags(request: LookupRequest) -> List[Dict[str, Any]]:
     """
     Asynchronously get all rules by tags.
 
     Args:
         request (LookupRequest): The tag information used in the rule look up
```

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/rule/model.py` & `spotlight-dev-0.0.1b7/spotlight/api/rule/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/rule/synchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/rule/synchronous.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from typing import Dict, Any, List
 
+import backoff
+import requests
+
 from spotlight.api.model import SearchRequest, LookupRequest
 from spotlight.api.rule.__util import (
     _get_rule_request_info,
     _get_rules_request_info,
     _create_rule_request_info,
     _update_rule_request_info,
     _delete_rule_request_info,
@@ -44,14 +47,19 @@
     Returns:
         List[Dict[str, Any]]: List of rule responses
     """
     request_info = _get_rules_request_info()
     return __get_request(**request_info)
 
 
+@backoff.on_exception(
+    backoff.expo,
+    (requests.exceptions.Timeout, requests.exceptions.ConnectionError),
+    max_tries=3,
+)
 @data_request
 def get_rules_by_tags(request: LookupRequest) -> List[Dict[str, Any]]:
     """
     Get all rules by tags.
 
     Args:
         request (LookupRequest): The tag information used in the rule look up
```

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/tag/__util.py` & `spotlight-dev-0.0.1b7/spotlight/api/tag/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/tag/asynchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/tag/asynchronous.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from typing import Dict, Any, List
 
+import aiohttp
+import backoff
+
 from spotlight.api.model import SearchRequest, LookupRequest
 from spotlight.api.tag.__util import (
     _get_tag_request_info,
     _get_tags_request_info,
     _create_tag_request_info,
     _update_tag_request_info,
     _delete_tag_request_info,
@@ -62,14 +65,17 @@
     Returns:
         List[Dict[str, Any]]: List of tag responses
     """
     request_info = _get_tags_request_info()
     return await __async_get_request(**request_info)
 
 
+@backoff.on_exception(
+    backoff.expo, (aiohttp.ClientTimeout, aiohttp.ClientConnectionError), max_tries=3
+)
 @async_data_request
 async def async_get_tags_by_lookup(request: LookupRequest) -> List[Dict[str, Any]]:
     """
     Asynchronously get all tags by lookup.
 
     Args:
         request (LookupRequest): The tag information used in the tag look up
```

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/tag/synchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/tag/synchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from typing import Dict, Any, List
 
+import backoff
+import requests
+
 from spotlight.api.model import SearchRequest, LookupRequest
 from spotlight.api.tag.__util import (
     _get_tag_request_info,
     _get_tag_by_name_request_info,
     _get_tags_request_info,
     _get_tags_by_rule_id_request_info,
     _search_tags_request_info,
@@ -62,14 +65,19 @@
     Returns:
         List[Dict[str, Any]]: List of tag responses
     """
     request_info = _get_tags_request_info()
     return __get_request(**request_info)
 
 
+@backoff.on_exception(
+    backoff.expo,
+    (requests.exceptions.Timeout, requests.exceptions.ConnectionError),
+    max_tries=3,
+)
 @data_request
 def get_tags_by_lookup(request: LookupRequest) -> List[Dict[str, Any]]:
     """
     Get all tags by lookup.
 
     Args:
         request (LookupRequest): The tag information used in the tag look up
```

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/tag/view/asynchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/tag/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/api/tag/view/synchronous.py` & `spotlight-dev-0.0.1b7/spotlight/api/tag/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/base.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/base.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/config.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/config.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/date/function.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/date/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/__util.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/asynchronous.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/synchronous.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/authorization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/__util.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/asynchronous.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/synchronous.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/timeit.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/decorators/timeit.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/errors.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/errors.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/function.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/metaclass/singleton.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/metaclass/singleton.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/requests/asynchronous.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/requests/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/common/requests/synchronous.py` & `spotlight-dev-0.0.1b7/spotlight/core/common/requests/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/pipeline/abstract.py` & `spotlight-dev-0.0.1b7/spotlight/core/pipeline/abstract.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/pipeline/decorator.py` & `spotlight-dev-0.0.1b7/spotlight/core/pipeline/decorator.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/abstract.py` & `spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/abstract.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/sql_rule.py` & `spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/rule/sql_rule.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/synchronous.py` & `spotlight-dev-0.0.1b7/spotlight/core/pipeline/execution/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/pipeline/model/pipeline.py` & `spotlight-dev-0.0.1b7/spotlight/core/pipeline/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/__init__.py` & `spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/utils/asynchronously.py` & `spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/utils/asynchronously.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/utils/synchronously.py` & `spotlight-dev-0.0.1b7/spotlight/core/pipeline/runner/utils/synchronously.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/pandas/__util.py` & `spotlight-dev-0.0.1b7/spotlight/pandas/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/pandas/pipeline.py` & `spotlight-dev-0.0.1b7/spotlight/pandas/pipeline.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight/pandas/runners.py` & `spotlight-dev-0.0.1b7/spotlight/pandas/runners.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b6/spotlight_dev.egg-info/PKG-INFO` & `spotlight-dev-0.0.1b7/spotlight_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b6
+Version: 0.0.1b7
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b6/spotlight_dev.egg-info/SOURCES.txt` & `spotlight-dev-0.0.1b7/spotlight_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

